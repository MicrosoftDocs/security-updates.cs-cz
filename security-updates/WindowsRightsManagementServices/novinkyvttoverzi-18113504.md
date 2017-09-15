---
TOCTitle: Novinky v této verzi
Title: Novinky v této verzi
ms:assetid: 'c68ec6fd-0ff5-467e-85a8-a53b9f089de3'
ms:contentKeyID: 18113504
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747748(v=WS.10)'
---

Novinky v této verzi
====================

Služba správy přístupových práv (RMS) s aktualizací Service Pack 1 (SP1) podporuje následující funkce:

-   **Zápis serveru RMS bez připojení k Internetu.** V předchozí verzi bylo nutné zajistit připojení serveru RMS k Internetu, aby se mohl zapsat ke službě Microsoft Enrollment Services a získat certifikát serveru pro poskytování licencí pro server kořenové certifikace. V případě služby RMS s aktualizací SP1 je i nadále nutné vyžádat tento certifikát od služby Microsoft Enrollment Services. Uvedený požadavek je však možné provést prostřednictvím jiného počítače, který je připojen k Internetu, a certifikát pak importovat na server RMS po dokončení zajištění.
-   **Klienti se aktivují sami.** V předchozí verzi bylo nutné stahovat certifikáty a bezpečnostní moduly klientských počítačů prostřednictvím služby Microsoft Activation Service. V případě služby RMS s aktualizací SP1 není připojení ke službě Microsoft Activation Service nutné.
-   **Podpora pro další typy klientů**. V této verzi je pomocí serveru RMS možné podporovat klienty mobilních zařízení a serverových služeb. Jako správci serveru RMS budete moci řídit, zda uvedeným klientům poskytnete certifikaci, jakmile budou chtít využít vaše služby.
-   **Podpora vícejazyčných šablon.** V předchozí verzi byly šablony založeny na jazykovém nastavení aplikace Internet Explorer. V této verzi můžete prostřednictvím webové stránky pro správu služby RMS určit jazyk, který použijete k vytvoření šablony.
-   **Podpora ověřování klientů pomocí karet Smart Card.** V této verzi může klient RMS používat pověření uložená v certifikátech x.509 na kartách Smart Card a pomocí nich provádět ověřování na serveru RMS za účelem získání certifikátu účtu práv a licencí k použití.
