---
TOCTitle: Nastavení serveru SMS nebo zásad skupiny na podporu nasazení klientů
Title: Nastavení serveru SMS nebo zásad skupiny na podporu nasazení klientů
ms:assetid: '9e37c27b-8cc1-40c6-adb7-0937aa64c8db'
ms:contentKeyID: 18113450
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747703(v=WS.10)'
---

Nastavení serveru SMS nebo zásad skupiny na podporu nasazení klientů
====================================================================

Při nasazení služby RMS musí být v počítačích uživatelů nainstalována aplikace s podporou služby RMS, aby uživatelé mohli chránit obsah a využívat obsah chráněný službou RMS.

Aplikace službu RMS podporuje pouze v případě, že integruje klienta RMS do svých operací. V systémech předcházejících systému Windows Vista® je klient RMS k dispozici jako samostatná součást ke stažení ze služby Stažení softwaru. Pokud však nechcete klienta stahovat do jednotlivých klientských počítačů v podniku, můžete tento krok automatizovat pomocí serveru SMS (Microsoft Systems Management Server), zásad skupin nebo skriptů.

| ![](images/Cc747703.Important(WS.10).gif)Důležité informace                |
|---------------------------------------------------------------------------------------------------------|
| Klient RMS je integrován do systému Windows Vista. Proto již není nutné provádět samostatnou instalaci. |

Distribuce klienta RMS pomocí serveru SMS vyžaduje následující kroky:

-   Vytvořte nový definiční soubor balíku.
-   Extrahujte soubory Instalační služby systému Windows ze souboru WindowsRightsManagementServicesSP2-KB917275-Client-ENU.exe. Pro tento účel je třeba soubor WindowsRightsManagementServicesSP2-KB917275-Client-ENU.exe nejprve uložit. Neinstalujte ho. U tohoto příkladu budeme předpokládat, že je soubor uložen ve složce c:\\název\_složky. Otevřete okno příkazového řádku a zadejte následující příkaz:
    `c:\folder_name\WindowsRightsManagementServicesSP2-KB917275-Client-ENU.exe /x/t:c:\folder_name`
    Tento příkaz extrahuje soubory MSDrmClient.msi a RMClientBackCompat.msi ze souboru EXE a umístí je do složky c:\\*název\_složky*.
-   Použijte soubory Instalační služby systému Windows pro definici a zdroj balíčku.
-   Inzerujte dostupnost balíčků v síti.

| ![](images/Cc747703.note(WS.10).gif)Poznámka                                                                                 |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------|
| K instalaci softwaru jsou nutná práva pro správu. Zásady zabezpečení organizace mohou vyžadovat, aby klientský software RMS nainstaloval správce systému. |

Další informace o distribuci softwaru pomocí serveru SMS najdete v příručce Systems Management Server 2003 Concepts, Planning, and Deployment Guide (Příručka pro koncepci, plánování a nasazení serveru Systems Management Server 2003) ([http://go.microsoft.com/fwlink/?LinkId=17401](http://go.microsoft.com/fwlink/?linkid=17401)) (stránka může být v angličtině).

Další informace o nasazení klientského softwaru pomocí zásad skupiny získáte v tématech věnovaných nasazení softwaru pomocí zásad skupiny ([http://go.microsoft.com/fwlink/?LinkId=38997](http://go.microsoft.com/fwlink/?linkid=38997)) (stránka může být v angličtině).
