---
TOCTitle: Zabezpečení během instalace služby RMS
Title: Zabezpečení během instalace služby RMS
ms:assetid: '0a3d40b2-f27e-4e63-baff-a9c8433f5f91'
ms:contentKeyID: 18113209
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc720192(v=WS.10)'
---

Zabezpečení během instalace služby RMS
======================================

Instalační program služby RMS používá k instalaci a konfiguraci souborů služby RMS pověření přihlášeného uživatele. Z tohoto důvodu je nutné, aby se správce spouštějící proceduru instalace přihlásil v rámci uživatelského účtu, který je členem místní skupiny správců. Při všech instalacích, s výjimkou instalací na samostatné počítače, se musí navíc jednat o účet uživatele domény.

Během procedury instalace dojde ke spuštění Instalační služby systému Windows (Msiexec.exe). Tato služba zdědí token nadřazeného uživatele. Teprve později v rámci vlastních akcí prováděných po dokončení procesu (pokud existují) použije služba Msiexec.exe identifikační údaje aktuálně přihlášeného uživatele. Tento postup nezávisí na tom, zda byl proces spuštěn z prohlížeče nebo z příkazového řádku.

Instalační program služby RMS provádí následující úlohy:

-   Zkopíruje soubory do složky C:\\Program Files\\RMS. Tato složka obvykle umožňuje přístup členům skupin Administrators i Power Users. Jednotku a složku pro umístění souborů lze při instalaci konfigurovat.

-   Ve výchozím nastavení vytvoří na portu 5720 web správy služby RMS, který slouží k zajišťování. Tento webový server odkazuje na instalované soubory.

-   Vytvoří fond aplikací WMCSProvisioningAppPool a přidruží jej k webu správy služby RMS. Jako účet služeb používá tento fond aplikací účet Síťové služby.
-   Nainstaluje čítače výkonu.

-   Udělí skupině RMS Service Group oprávnění ke čtení i zápisu pro následující klíč registru.
    Počítače s 32bitovou verzí systému Windows Server 2003

    `HKEY_LOCAL_MACHINE\Software\Microsoft\DRMS\1.0`

    Počítače s 64bitovou verzí systému Windows Server 2003

    `HKEY_LOCAL_MACHINE\Software\WOW6432Node\Microsoft\DRMS\1.0`