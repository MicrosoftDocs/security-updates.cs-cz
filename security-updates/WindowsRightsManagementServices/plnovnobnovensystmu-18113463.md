---
TOCTitle: Plánování obnovení systému
Title: Plánování obnovení systému
ms:assetid: 'a7779ffd-7a94-4e13-b846-0ffd00608e02'
ms:contentKeyID: 18113463
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747718(v=WS.10)'
---

Plánování obnovení systému
==========================

K selhání systému dochází z mnoha různých neplánovaných příčin. Může se jednat o selhání hardwaru, záplavy, přepětí, chyby softwaru a další důvody. Součástí úspěšného nasazení jsou také plány na rychlé obnovení systému v případě selhání. V systému služby RMS je primárním požadavkem ochrany funkcí této služby pravidelné zálohování soukromého klíče serveru a databází služby RMS, zvláště konfigurační databáze. Zálohováním této databáze chráníte šablony zásad práv, klíče a další data potřebná pro poskytnutí přístupu k dřívějším licencím a k publikovanému obsahu. Jestliže existující instalace služby RMS přestane být k dispozici, můžete tuto službu nainstalovat na další servery a zajistit ji tak, že jako požadovanou databázi nastavíte záložní konfigurační databázi. Stav nové záložní instalace bude totožný se stavem původní instalace v okamžiku, kdy byla vytvořena poslední záloha.

Tento oddíl se zabývá následujícími tématy:

-   [Příprava obnovení systému](https://technet.microsoft.com/885c047f-1e3b-4bf5-8248-3a4505759cbb)
-   [Zálohování systému pro službu RMS](https://technet.microsoft.com/c29894da-ee00-428c-8d48-80d8e5a83678)
-   [Zálohování a obnovení systému služby RMS](https://technet.microsoft.com/c11f3ac1-e512-402b-bf13-9ff21f5fe745)
-   [Zálohování a obnovení šablon zásad práv](https://technet.microsoft.com/a6ed3328-4128-45e8-9236-3de484b460de)
