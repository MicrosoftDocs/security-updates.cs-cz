---
TOCTitle: Zabezpečení při běžném provozu služby RMS
Title: Zabezpečení při běžném provozu služby RMS
ms:assetid: '98f3d584-6320-4aa1-9959-7133cfdb6df7'
ms:contentKeyID: 18113380
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747609(v=WS.10)'
---

Zabezpečení při běžném provozu služby RMS
=========================================

Po instalaci a zajištění služby RMS pracují webové služby RMS jako aplikace služby IIS, tj. získávají přístup k různým systémovým prostředkům, které vyžadují ověření a autorizaci. Všechny systémové prostředky vyžadují ověřování a nelze je konfigurovat jinak. Zbývající část této stránky popisuje podobu autorizace ve službě RMS.

Webové služby RMS jsou spuštěny v kontextu fondu aplikací služby IIS. Každý fond aplikací v rámci služby IIS má jedinečnou identitu, která může odpovídat účtu uživatele domény, místnímu uživatelskému účtu, místnímu účtu síťové služby nebo místnímu systémovému účtu. Jednotlivé účty mají v rámci systému různou úroveň ověření. Po zajištění služby RMS můžete zvolit, zda budou webové služby RMS spuštěny jako místní systémový účet nebo jako účet uživatele domény. Tento účet se potom stane identitou fondu aplikací služby RMS. Fondem aplikací pro web Globální správa je Fond aplikací DRMS. Fond aplikací pro zajištěný web je nazván \_DRMSAppPool1. Protokolování služby RMS je spuštěno jako samostatná služba systému Windows pod účtem, který byl také zadán pro identitu fondu aplikací služby RMS.

Mezi prostředky, ke kterým webové služby RMS potřebují získat přístup, patří různé soubory a složky v systému, databáze a uložené procedury na databázovém serveru, místní registr, služba Active Directory, mezipaměť sestavení, paměť a další procesy spuštěné v daném systému. Protokolování služby RMS zároveň vyžaduje přístup k frontě protokolování v místním systému. Každý z těchto prostředků má vlastní seznam DACL, který definuje, kdo je oprávněn k tomuto prostředku přistupovat, a co lze s prostředkem dělat.

Z důvodů zjednodušení přiřazování oprávnění a správy účtů služeb jsou všechna požadovaná oprávnění přiřazena místní skupině RMS Service Group, kterou služba RMS vytvořila v průběhu zajišťování. Vzhledem k tomu, že účet služby RMS je členem uvedené skupiny, může využívat všechna oprávnění k ní přiřazená.

Oprávnění udělená skupině RMS Service Group jsou shrnuta v následujícím seznamu:

-   oprávnění ke čtení pro virtuální kořenové adresáře,
-   oprávnění k zápisu do adresáře mezipaměti sestavení,
-   oprávnění k zápisu do dočasného systémového adresáře,
-   oprávnění k zápisu do fronty protokolování,
-   oprávnění ke čtení pro službu Active Directory.

Pokud jako databázový server používáte Microsoft SQL Server 2000, měli byste vědět, že tento server přiřazuje oprávnění mírně odlišným způsobem než systém Windows Server 2003. Při zajišťování služby RMS je na serveru SQL Server vytvořeno přihlášení pro účet služby RMS. Jestliže jste se rozhodli službu RMS zajistit prostřednictvím místního systémového účtu, je přihlášení k serveru SQL Server vytvořeno ve formátu *DOMÉNA\\název\_počítače*, kde hodnota *DOMÉNA* představuje název domény služby Active Directory, jejímž je daný počítač členem, a hodnota *název\_počítače* je název příslušného serveru. Je vytvořena role SQL s názvem rms\_service, které jsou přiřazena všechna nezbytná oprávnění. Do této skupiny je přidáno přihlášení pro účet služby RMS. Účtu služby RMS není explicitně uděleno žádné oprávnění.

Dále SQL Server přiřadí každé databázi vlastníka. Vlastnictví databáze je přiřazeno během zajišťování, a to následujícím způsobem:

-   Jako vlastník konfigurační databáze je nastaven doménový účet, pomocí kterého byla zajištěna služba RMS.
-   Jako vlastník databáze adresářových služeb a databáze protokolování je nastaven účet služby RMS.

Oprávnění ke všem prostředkům vytvořeným službou RMS byla během vývoje této služby pečlivě vybrána s ohledem na zabezpečení. Změna oprávnění přiřazených v průběhu zajišťování pro libovolný z těchto prostředků by proto neměla být nutná. Změnu účtu nebo hesla uživatele pro účet služby po zajištění můžete provést na webové stránce Globální správa služby RMS. Další informace získáte v této sadě dokumentace v části Změna účtu služby RMS tématu Provoz serveru RMS.
