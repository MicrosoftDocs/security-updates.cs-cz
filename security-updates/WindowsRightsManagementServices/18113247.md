---
TOCTitle: Hierarchie důvěryhodnosti služby RMS
Title: Hierarchie důvěryhodnosti služby RMS
ms:assetid: '2d44182f-a653-4383-aba1-dade53f7cf9a'
ms:contentKeyID: 18113247
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc720232(v=WS.10)'
---

Hierarchie důvěryhodnosti služby RMS
====================================

Mezi součásti systému služby RMS patří služba Microsoft Enrollment Services, servery RMS organizace, klientské počítače a uživatelé systému. Pro každou součást je vydán certifikát, který určuje její identitu v systému. Hierarchie důvěryhodnosti definuje vztahy důvěryhodnosti mezi těmito certifikáty a následně také mezi entitami, které jim odpovídají. Hierarchie definuje také vztahy důvěryhodnosti mezi důvěryhodnými entitami a licencemi, které jsou vydávány pro další důvěryhodné entity.

Hierarchie důvěryhodnosti propojuje certifikáty a licence v řetězec důvěryhodnosti, který může služba RMS vždy vysledovat od konkrétního certifikátu nebo licence až po důvěryhodný pár klíčů. Řetězec důvěryhodnosti obsahuje aktuální certifikát, certifikát entity, která jej vydala, dále certifikát entity, která vydala certifikát této entity, a takto podél řetězce dále, až po kořen důvěryhodnosti.

Pro službu RMS je kořenem důvěryhodnosti pár klíčů společnosti Microsoft. Tento společný kořen důvěryhodnosti umožňuje společnostem a organizacím vytvořit ekosystém zahrnující důvěryhodné entity, jako jsou například uživatelé a partneři, uvnitř i vně dané společnosti či organizace.

V následujícím diagramu je zobrazena hierarchie důvěryhodnosti v určité organizaci. Řetězec důvěryhodnosti lze sledovat směrem zpět až ke službám společnosti Microsoft, které vydávají základní certifikáty.

![](images/Cc720232.6c169175-94fb-4ec0-93bc-12748aae3ac4(WS.10).gif)
1.  Každému klientskému počítači je vydán jedinečný bezpečnostní modul, který obsahuje kořenový veřejný klíč společnosti Microsoft.
2.  Jakmile obdrží požadavek na licenci, ověří služba RMS zaregistrované objekty zabezpečení podle cesty v hierarchii důvěryhodnosti až ke kořenu důvěryhodnosti.
3.  Služba RMS ověří pravost důvěryhodné entity uvedené v licenci.
4.  Ověří také, zda byl certifikát důvěryhodné entity vydán serverem z hierarchie důvěryhodnosti.

Na každé úrovni řetězce certifikátů pak ověřuje platnost dané licence nebo certifikátu a také jejich propojení se známým kořenem důvěryhodnosti v řetězci důvěryhodnosti. U každé licence nebo certifikátu v řetězci ověřuje služba RMS platnost následujících podmínek:

-   Příslušný kód XrML je platný.
-   Podpis vydavatele je platný.
-   Sémantický obsah licence odpovídá požadovanému použití.
-   Jsou splněny požadované podmínky (například data platnosti).
-   Licence nebyla odejmuta.
-   Klíč podpisu licence a klíč certifikovaného vydavatele si navzájem odpovídají.
