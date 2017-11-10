---
TOCTitle: Kontrola návrhu služby RMS
Title: Kontrola návrhu služby RMS
ms:assetid: '0ed1dd67-8e07-47c9-9e2e-0104438bd19f'
ms:contentKeyID: 18113287
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc720185(v=WS.10)'
---

Kontrola návrhu služby RMS
==========================

Před realizací nasazení služby RMS v organizaci se přesvědčte, zda jsou v plánu vyřešeny následující položky:

-   Byla vybrána klientská aplikace s podporou služby RMS a k dispozici jsou plány implementace.
-   Byl určen způsob distribuce klienta RMS.
-   Je nainstalován databázový server, který je dostupný.
-   Byla vybrána základní nebo distribuovaná topologie služby RMS.
-   Na řadičích domény, na kterých je nainstalován systém Windows 2000 s aktualizací Service Pack 3 (SP3) či vyšší, je nainstalována služba Active Directory a všem uživatelům byl nakonfigurován kontaktní objekt s e-mailovým atributem. Je nainstalován systém Windows Server 2003 s nejnovějšími aktualizacemi. Jsou povoleny služby Řízení front zpráv, IIS a ASP.NET verze 1.1.

> [!NOTE]
> Pokud budete chtít službu RMS instalovat do 64bitového počítače, projděte si část Softwarové požadavky pro službu RMS tématu Plánování nasazení služby RMS v této sadě dokumentace, kde naleznete pokyny pro speciální konfiguraci. 

-   Jsou definovány způsoby vyrovnávání zatížení a převzetí služeb při selhání serveru.
-   Je nakonfigurována registrace DNS pro servery RMS.
-   K dispozici jsou plány pro zálohování a obnovení.
-   Jsou vypracovány plány zabezpečení odpovídající potřebám a požadavkům organizace.
