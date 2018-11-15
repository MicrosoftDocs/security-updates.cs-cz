---
TOCTitle: 'Krok 1: Kontrola instalačních požadavků služby WSUS 3.0'
Title: 'Krok 1: Kontrola instalačních požadavků služby WSUS 3.0'
ms:assetid: '912b37d7-021e-4c95-b317-49dd15b4611c'
ms:contentKeyID: 18126700
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc708484(v=WS.10)'
---

Krok 1: Kontrola instalačních požadavků služby WSUS 3.0
=======================================================

Tato příručka vysvětluje, jak nainstalovat službu WSUS 3.0. Informace o požadavcích na software a podporovaných platformách pro službu WSUS 3.0 naleznete v poznámkách k verzi ([http://go.microsoft.com/fwlink/?LinkId=71220](http://go.microsoft.com/fwlink/?linkid=71220)) pro operační systém Windows Server 2003 Service Pack 1 a Windows Server® 2008.

Požadavky na software pro instalaci služby WSUS 3.0 v systému Windows Server 2003 Service Pack 1
------------------------------------------------------------------------------------------------

Chcete-li nainstalovat službu WSUS 3.0 v systému Windows Server 2003 Service Pack 1, je nutné, aby byl v počítači nainstalován následující software. Pokud některé z těchto aktualizací vyžadují restartování serveru po dokončení instalace, měli byste jej restartovat před instalací služby WSUS 3.0.

-   Internetová informační služba (IIS) 6.0.
-   Aktualizace pro službu BITS (Background Intelligent Transfer Service) 2.0 a WinHTTP 5.1 systému Windows Server 2003. Chcete-li tento software stáhnout, přejděte na web Stažení softwaru ([http://go.microsoft.com/fwlink/?LinkID=47251](http://go.microsoft.com/fwlink/?linkid=47251)).
-   Balíček Microsoft .NET Framework verze 2.0 Redistributable Package (x86). Chcete-li tento software stáhnout, přejděte na web Stažení softwaru ([http://go.microsoft.com/fwlink/?LinkID=68935](http://go.microsoft.com/fwlink/?linkid=68935)). (V případě 64bitových platforem také použijte web Stažení softwaru \[[http://go.microsoft.com/fwlink/?LinkID=70637](http://go.microsoft.com/fwlink/?linkid=70637)\].)
-   Prohlížeč Microsoft Report Viewer Redistributable 2005. Tento software můžete získat na webu Stažení softwaru ([http://go.microsoft.com/fwlink/?LinkID=70410](http://go.microsoft.com/fwlink/?linkid=70410)).
-   Konzola Microsoft Management Console 3.0 pro systém Windows Server 2003 (KB907265). Chcete-li tento software stáhnout, přejděte na web Stažení softwaru ([http://go.microsoft.com/fwlink/?LinkID=70412](http://go.microsoft.com/fwlink/?linkid=70412)). (V případě 64bitových platforem také použijte web Stažení softwaru \[[http://go.microsoft.com/fwlink/?LinkID=70638](http://go.microsoft.com/fwlink/?linkid=70638)\].)

Požadavky na software pro instalaci služby WSUS 3.0 v systému Windows Server 2008
---------------------------------------------------------------------------------

Chcete-li nainstalovat službu WSUS 3.0 v systému Windows Server 2008, je nutné, aby byly v počítači nainstalovány následující položky. Pokud některé z těchto aktualizací vyžadují restartování serveru po dokončení instalace, měli byste jej restartovat před instalací služby WSUS 3.0.

-   Internetová informační služba (IIS) 7.0. Zkontrolujte, zda jsou povolené následující součásti:
    -   Ověřování systému Windows
    -   ASP.NET
    -   Kompatibilita správy služby IIS 6.0
    -   Kompatibilita metabáze služby IIS
-   Prohlížeč Microsoft Report Viewer Redistributable 2005. Tento software můžete stáhnout z webu Stažení softwaru ([http://go.microsoft.com/fwlink/?LinkID=70410](http://go.microsoft.com/fwlink/?linkid=70410)).
-   Microsoft SQL Server™ 2005 Service Pack 1. Tento software můžete stáhnout z webu Stažení softwaru ([http://go.microsoft.com/fwlink/?LinkID=70410](http://go.microsoft.com/fwlink/?linkid=66143)).

Aktualizace rozhraní .NET Framework 2.0 a služby BITS 2.0 je k dispozici jako součást operačního systému Windows Server 2008.

Požadavky a doporučení týkající se disku
----------------------------------------

Chcete-li instalovat službu WSUS 3.0, musí systém souborů na serveru splňovat následující požadavky:

-   Systémový oddíl i oddíl, na který instalujete službu WSUS 3.0, musí být naformátovány se systémem souborů NTFS.
-   Minimální doporučení pro systémový oddíl je 1 GB volného místa.
-   Minimální doporučení pro svazek, kam bude služba WSUS ukládat obsah, je 20 GB volného místa. Vhodnější je 30 GB volného místa.
-   Minimální doporučení pro svazek, kam instalační program služby WSUS bude instalovat software Interní databáze systému Windows®, je 2 GB volného místa.

Požadavky pouze pro instalaci konzoly
-------------------------------------

Služba WSUS 3.0 nyní umožňuje nainstalovat konzolu Správa služby WSUS ve vzdálených systémech odděleně od serveru WSUS. Instalace pouze konzoly lze provádět v následujících operačních systémech:

-   Windows Server® 2008
-   Windows Vista®
-   Windows Server 2003 Service Pack 1,
-   Windows XP Service Pack 2.

Požadavky na software pro instalaci pouze konzoly

-   Balíček Microsoft .NET Framework verze 2.0 Redistributable Package (x86), k dispozici na webu služby Stažení softwaru ([http://go.microsoft.com/fwlink/?LinkId=68935](http://go.microsoft.com/fwlink/?linkid=68935)). V případě 64bitové platformy viz Balíček Microsoft .NET Framework verze 2.0 Redistributable Package (x64) ([http://go.microsoft.com/fwlink/?LinkId=70637](http://go.microsoft.com/fwlink/?linkid=70637)).
-   Konzola Microsoft Management Console 3.0 pro systém Windows Server 2003 (KB907265) k dispozici na webu Stažení softwaru ([http://go.microsoft.com/fwlink/?LinkId=70412](http://go.microsoft.com/fwlink/?linkid=70412)). V případě 64bitové platformy viz Konzola Microsoft Management Console 3.0 pro systém Windows Server 2003 x64 Edition (KB907265) ([http://go.microsoft.com/fwlink/?LinkId=70638](http://go.microsoft.com/fwlink/?linkid=70638)).
-   Microsoft Report Viewer Redistributable 2005, k dispozici na webu služby Stažení softwaru ([http://go.microsoft.com/fwlink/?LinkId=70410](http://go.microsoft.com/fwlink/?linkid=70410)).

Požadavky pro automatické aktualizace
-------------------------------------

Automatické aktualizace jsou klientskou součástí služby WSUS 3.0. Automatické aktualizace nemají kromě připojení k síti žádné další požadavky na hardware. Automatické aktualizace je možné použít se službou WSUS 3.0 v počítačích s kterýmkoli z následujících operačních systémů:

-   Windows Vista.
-   Windows Server® 2008.
-   Microsoft Windows® Server 2003, všechny verze a aktualizace Service Pack,
-   Microsoft Windows XP Professional Service Pack 1 nebo Service Pack 2,
-   Microsoft Windows 2000 Professional Service Pack 4, Windows 2000 Server Service Pack 4 nebo Windows 2000 Advanced Server Service Pack 4.

Oprávnění
---------

Je třeba přidělit následující disková oprávnění zadaným uživatelům k zadaným adresářům:

1.  Buď vestavěná skupina Uživatelé, nebo účet NT Authority\\Network Service (v systému Windows Server 2003), by měly mít oprávnění pro čtení ke kořenové složce na jednotce, kde se nachází adresář obsahu služby WSUS. Bez tohoto oprávnění se nezdaří stažení službou BITS.
2.  Účet NT Authority\\Network Service by měl mít oprávnění Úplné řízení k adresáři obsahu služby WSUS (obvykle &lt;Ovladač\_systému&gt;:WSUS\\WsusContent). Toto oprávnění je nastaveno při instalaci serveru WSUS, když je vytvořen tento adresář, ale některý zabezpečovací software může toto oprávnění vynulovat. Bez tohoto oprávnění se nezdaří stažení službou BITS.
3.  Aby se správně zobrazil modul snap-in Správy služby WSUS, účet NT Authority\\Network Service by měl mít oprávnění Úplné řízení k následujícím složkám:
    -   %windir%\\Microsoft .NET\\Framework\\v2.0.50727\\Temporary ASP.NET Files
    -   %windir%\\Temp

Další informace o nastavení oprávnění naleznete v dokumentu s popisem, jak proces DCPROMO nezachovává oprávnění k některým složkám Internetové informační služby, na webu http://go.microsoft.com/fwlink/?LinkID=76332 (tato stránka může být v angličtině).
