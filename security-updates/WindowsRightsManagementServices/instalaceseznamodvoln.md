---
TOCTitle: Instalace seznamů odvolání
Title: Instalace seznamů odvolání
ms:assetid: 'e331338b-66d4-45e4-8d3f-acccf2302ac4'
ms:contentKeyID: 18113479
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747702(v=WS.10)'
---

Instalace seznamů odvolání
==========================

Při implementaci odvolání je třeba instalovat seznamy odvolání. Tyto seznamy určují obsah, aplikace, uživatele nebo jiné zaregistrované objekty, které byly odvolány. Instalovat můžete vlastní seznamy odvolání i seznamy společnosti Microsoft.

Instalace seznamů odvolání organizace
-------------------------------------

Aby bylo možné použít šablonu zásad práv využívající seznam odvolání, je nejprve třeba poskytnout seznam odvolání k dispozici klientským počítačům. Informace o vytváření seznamů odvolání získáte v tomto tématu v části Implementace odvolání uvedené již dříve.

Seznam odvolání organizace můžete instalovat následujícím postupem:

1.  Zkopírujte soubor se seznamem odvolání na veřejně přístupný webový server. Vzhledem k tomu, že uživatelé mohou pracovat s chráněným obsahem mimo danou organizaci, mělo by být určené umístění přístupné pro všechny uživatele v rámci podnikové sítě i mimo ni.
    Distribuce souboru se seznamem odvolání do klientských počítačů může být časově náročná. Může se tedy stát, že uživatelé nebudou mít ve svých klientských počítačích seznam k dispozici v okamžiku, kdy se pokusí otevřít dokument, který daný seznam vyžaduje. Není-li seznam odvolání v klientském počítači k dispozici, může jej stáhnout aplikace s podporou služby RMS z umístění zadaného v licenci k použití.
    V ideálním případě by měl být vytvořen skript, který denně automaticky seznam odvolání podepíše a zkopíruje jej na web. Tak bude zajištěno, že uživatelům nebude zabráněno v práci s obsahem z důvodu neaktuálnosti jejich seznamu odvolání. Ukázkový skript naleznete v tomto tématu v části Práce s nástrojem pro podepisování seznamu odvolaných certifikátů uvedené již dříve.
2.  V šabloně zásad práv určete pro seznam odvolání organizace interval aktualizace větší než nula. Tím zajistíte, že seznam odvolání nebude nepovinný. Pokud seznam nebude aktualizován pravidelně, například při porušení zabezpečení, můžete nastavit delší interval aktualizace a pak v případě potřeby předat seznam odvolání do klientských počítačů na základě nastavení skriptování nebo zásad. Informace o nastavení intervalů obnovení získáte v tomto tématu v části Definice zásad odvolání uvedené již dříve. Další informace týkající se konfigurace šablon zásad práv naleznete v tomto tématu v části Vytvoření a změna šablon zásad práv uvedené již dříve.
3.  V šabloně zásad práv určete adresu URL, na níž je seznam odvolání k dispozici.
4.  Seznam odvolání je také možné do klientských počítačů instalovat automaticky, a to například pomocí zásad skupiny nebo serveru SMS (Systems Management Server).

Instalace seznamů odvolání společnosti Microsoft
------------------------------------------------

Klient Služby správy přístupových práv může použít seznam odvolání společnosti Microsoft pouze v případě, že je tento seznam nainstalován v klientských počítačích. V tomto tématu je popsán postup při instalaci seznamu odvolání společnosti Microsoft v následujících scénářích:

-   Organizace chce instalovat vlastní seznam odvolání a seznam společnosti Microsoft.
-   Organizace chce instalovat pouze seznam odvolání společnosti Microsoft.

Jakmile je seznam odvolání společností Microsoft publikován, můžete jej stáhnout z následujících umístění:

-   Servery RMS budou moci stáhnout seznam odvolání pomocí služby Windows Update.
-   Pokud není server RMS připojen k Internetu, je možné seznam odvolání společnosti Microsoft stáhnout z centra pro stahování Microsoft Download Center.

Jestliže balíček seznamů odvolání stáhnete na server RMS, bude uložen do složky %systémová\_jednotka%\\Program Files\\Windows Rights Management Services Revocation List. Pokud jej stahujete do jiného typu počítače, můžete vybrat umístění, kam bude uložen. Balíček obsahuje spustitelný soubor CRL\_Update.exe, kterým lze všechny klientské seznamy odvolání nainstalovat do úložiště klientských licencí, a soubor se seznamem odvolání Msrl.xml, který můžete zkopírovat na web nebo do veřejné sdílené složky.

**Instalace seznamu odvolání organizace a seznamu odvolání společnosti Microsoft**
1.  Chcete-li instalovat seznam odvolání organizace, postupujte podle pokynů uvedených v tomto tématu již dříve v části [Instalace seznamů odvolání](https://technet.microsoft.com/e331338b-66d4-45e4-8d3f-acccf2302ac4).

2.  Stáhněte balíček seznamů odvolání společnosti Microsoft a nainstalujte jej do všech klientských počítačů v organizaci pomocí vhodné metody, například zásad skupiny nebo serveru SMS (Systems Management Server). Případně můžete položky zkopírovat ze seznamu odvolání společnosti Microsoft do seznamu organizace a instalovat pouze seznam organizace.

| ![](images/Cc747702.Caution(WS.10).gif)Upozornění                                                                                                                                                                                                                                                                                                                                                                      |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Společnost Microsoft je zaregistrovaným objektem zabezpečení v posloupnosti důvěryhodných objektů pro všechny certifikáty a licence vydané službou RMS. Seznam odvolání vydaný společností Microsoft má tedy vliv na všechny požadavky na vazbu, pro které je získána licence k použití na základě šablony zásad práv vyžadující seznam odvolání organizace. Kromě toho je seznam odvolání společnosti Microsoft registrován v klientském počítači. |

**Instalace omezená na seznam odvolání společnosti Microsoft**
1.  Stáhněte balíček seznamů odvolání společnosti Microsoft.

2.  Změňte všechny existující šablony zásad práv tak, aby vyžadovaly odvolání, případně takovou šablonu vytvořte, pokud dosud žádná neexistuje. Při určení podmínky odvolání použijte veřejný klíč společnosti Microsoft.

3.  Pro interval aktualizace použijte velmi vysokou hodnotu, například 50 000. Tím zajistíte, že seznamu odvolání publikovanému společností Microsoft nikdy neskončí doba platnosti. Licence k použití, které distribuujete, tak nebudou vyžadovat novou verzi seznamu odvolání společnosti Microsoft v případě, kdy taková verze nebude k dispozici.

4.  Zkopírujte soubor se seznamem odvolání na veřejně přístupný webový server. Vzhledem k tomu, že uživatelé mohou pracovat s chráněným obsahem mimo danou organizaci, mělo by být určené umístění přístupné pro všechny uživatele v rámci podnikové sítě i mimo ni.

5.  Seznam odvolání je třeba poskytnout uživatelům k dispozici, protože distribuce souboru se seznamem odvolání do klientských počítačů může trvat delší dobu. Může se tedy stát, že uživatel nebude mít ve svém počítači seznam k dispozici v okamžiku, kdy se pokusí otevřít dokument obsahující licenci k publikování, která daný seznam vyžaduje. Není-li seznam odvolání v klientském počítači k dispozici, může jej stáhnout aplikace podporující správu přístupových práv z určeného umístění.

6.  V šabloně zásad práv určete adresu URL, na níž je seznam odvolání k dispozici. Další informace týkající se konfigurace šablon zásad práv naleznete v tomto tématu v části [Vytvoření a změna šablon zásad práv](https://technet.microsoft.com/6014176f-ef71-4d29-b3e3-da129c18563d) uvedené již dříve.

7.  Balíček seznamů odvolání můžete také do klientských počítačů instalovat například pomocí zásad skupiny nebo serveru SMS (Systems Management Server). Uživatelé pak budou moci otevřít obsah chráněný správou přístupových práv vyžadující seznamy odvolání i v případě, kdy nebudou připojeni k síti.
