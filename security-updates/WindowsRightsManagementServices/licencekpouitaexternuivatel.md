---
TOCTitle: Licence k použití a externí uživatelé
Title: Licence k použití a externí uživatelé
ms:assetid: '02db9bda-180e-438f-863d-26252083a471'
ms:contentKeyID: 18113220
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc720176(v=WS.10)'
---

Licence k použití a externí uživatelé
=====================================

Služba RMS umožňuje autorům sdílet chráněný obsah s oprávněnými externími uživateli prostřednictvím Internetu. Služba RMS nabízí stejnou ochranu publikovaného obsahu pro interní i externí uživatele, protože na práva spojená s daným obsahem je nutné získat licenci ze serveru RMS. Tímto způsobem je umožněno organizacím sdílet pro společnou práci důvěrné dokumenty, jako jsou například smlouvy, v síti Internet.

Externí uživatel obvykle získává ke službě RMS přístup prostřednictvím Internetu. (Pokud některý uživatel může získat přístup do interní sítě přímo, například pomocí virtuální privátní sítě VPN, je funkčně na shodné úrovni s interními uživateli.) Bez ohledu na to, zda se jedná o interního nebo externího uživatele publikující organizace, odpovídá proces získání licence k použití postupu popsanému již dříve v tomto tématu v části [Získání licence k použití](https://technet.microsoft.com/0b6cde34-418a-4dee-9d27-b65b93b535ac). Pro získání licence k použití není nutné, aby uživatel náležel k síti autora či měl v této síti uživatelský účet.

Vyžadovány jsou pouze následující podmínky:

-   Uživatel má k dispozici platný certifikát účtu práv.

-   Uživatel může získat přístup k serveru správy licencí RMS, který vydal licenci k publikování a který je umístěn na intranetu nebo extranetu.

-   Instalace služby RMS, která vydala certifikát účtu daného uživatele, je uvedena na seznamu důvěryhodných domén uživatelů instalace služby RMS vydávající licenci k použití.

Licenci k použití mohou obdržet následující typy externích uživatelů:

-   Uživatelé, jejichž účty jsou součástí jiné doménové struktury služby Active Directory s další instalací služby RMS. Instalace služby RMS v této jiné doménové struktuře musí být pro první instalaci služby definována jako důvěryhodná doména uživatelů.

-   Uživatelé z jiné organizace, ve které je také spuštěna instalace služby RMS uvedená na seznamu důvěryhodných domén uživatelů pro instalaci první organizace.

-   Uživatelé s certifikátem účtu práv služby .NET Passport v případě, že je služba certifikace RMS společnosti Microsoft uvedena na seznamu důvěryhodných domén uživatelů pro danou instalaci.

Do seznamu důvěryhodných domén je možné přidat jinou organizaci nebo jinou instalaci služby RMS ve vaší organizaci. Po přidání domény můžete definovat, které e-mailové domény mají být v této doméně považovány za důvěryhodné a také určit, zda mají být považovány za důvěryhodné identifikátory zabezpečení (SID) obsažené v této doméně, či nikoli.

Jiná organizace nebo jiná instalace služby RMS ve vaší organizaci mohou přidat vaší instalaci služby RMS do svých seznamu důvěryhodných domén uživatelů, takže jejich servery RMS mohou zpracovávat požadavky na licence k použití od vašich uživatelů.

Další informace o vytvoření důvěryhodných domén uživatelů mezi službou RMS a jinými organizacemi získáte v této sadě dokumentace v části [Důvěryhodné domény uživatelů](https://technet.microsoft.com/a09b883f-f455-4c46-a4fd-d37b689e1d24) uvedené v tomto tématu později a v části Přidání a odebrání důvěryhodných domén publikování tématu Provoz serveru RMS.
