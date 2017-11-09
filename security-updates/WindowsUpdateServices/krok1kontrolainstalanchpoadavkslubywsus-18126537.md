---
TOCTitle: 'Krok 1: Kontrola instalačních požadavků služby WSUS'
Title: 'Krok 1: Kontrola instalačních požadavků služby WSUS'
ms:assetid: '57d7f8ec-1523-4485-9967-604be9ba2aac'
ms:contentKeyID: 18126537
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc720547(v=WS.10)'
---

Krok 1: Kontrola instalačních požadavků služby WSUS
===================================================

Tento průvodce nabízí pokyny pro instalaci služby Microsoft Windows Software Update Services (WSUS) v operačních systémech Microsoft Windows Server 2003 (s výjimkou verze Web Edition a všech 64bitových verzí). Pokud máte server se systémem Microsoft Windows 2000 Server a potřebujete další informace, přečtěte si informace v dokumentu White Paper Deploying Microsoft Windows Server Update Services (Nasazení služby Microsoft Windows Server Update Services).

Dále uvádíme základní požadavky pro instalace, které používají výchozí možnosti. Hardwarové a softwarové požadavky pro další instalace naleznete v dokumentu White Paper Deploying Microsoft Windows Server Update Services.

Hardwarová doporučení pro server až s 500 klienty jsou následující:

-   procesor 1 GHz,
-   paměť RAM 1 GB.

Požadavky na software
---------------------

Chcete-li instalovat službu WSUS s výchozími možnostmi, musíte mít v počítači instalovány následující programy. Další informace o požadavcích na software WSUS naleznete v dokumentu White Paper Deploying Microsoft Windows Server Update Services. Pokud některé z těchto aktualizací vyžadují po dokončení instalace restartování počítače, měli byste restartovat server před instalací služby WSUS.

-   Internetová informační služba (IIS) 6.0: Pokyny pro instalaci Internetové informační služby naleznete v dokumentu White Paper Deploying Microsoft Windows Server Update Services nebo v Nápovědě a odborné pomoci v systému Windows Server 2003.
-   Aktualizace Microsoft .NET Framework 1.1 Service Pack 1 pro Windows Server 2003: Tento software získáte na serveru [Download Center](http://go.microsoft.com/fwlink/?linkid=47358) na adrese http://go.microsoft.com/fwlink/?LinkId=47358.
    Další možností je přejít na web http://www.windowsupdate.com a vyhledat důležité aktualizace a aktualizace Service Pack a potom nainstalovat aktualizaci Microsoft .NET Framework 1.1 Service Pack 1 pro Windows Server 2003.
-   Služba inteligentního přenosu na pozadí (BITS) 2.0: Služba BITS 2.0 pro Windows Server 2003 v současné době není na serveru Download Center k dispozici. Chcete-li získat tento software, přejděte na [web společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=47357) Windows Server Update Services Open Evaluation na adrese http://go.microsoft.com/fwlink/?LinkId=47357.

> [!NOTE]
> Ačkoli je k instalaci služby WSUS požadován databázový software, není zde uveden, protože výchozí instalace služby WSUS na serveru Windows 2003 zahrnuje databázový software Windows SQL Server™ 2000 Desktop Engine (WMSDE). 

Požadavky a doporučení týkající se disku
----------------------------------------

Chcete-li instalovat službu WSUS, musí systém souborů serveru splňovat následující požadavky:

-   Systémový oddíl i oddíl, na který instalujete službu WSUS, je nutné formátovat se systémem souborů NTFS.
-   Nejméně 1 GB volného místa je požadován pro systémový oddíl.
-   Minimálně 6 GB volného místa je požadováno pro svazek, kde služba WSUS ukládá obsah. Doporučuje se 30 GB.
-   Minimálně 2 GB volného místa jsou požadovány na svazku, kde instalační program služby WSUS instaluje software Windows SQL Server™ 2000 Desktop Engine (WMSDE).

Požadavky pro automatické aktualizace
-------------------------------------

Automatické aktualizace jsou klientskou součástí služby WSUS. Automatické aktualizace nemají kromě připojení k síti žádné jiné hardwarové požadavky. Automatické aktualizace je možné použít se službou WSUS u počítačů s kterýmkoli z následujících operačních systémů:

-   Microsoft Windows 2000 Professional s aktualizací Service Pack 3 (SP3) nebo Service Pack 4 (SP4), Windows 2000 Server s aktualizací SP3 nebo SP4 nebo Windows 2000 Advanced Server s aktualizací SP3 nebo SP4;
-   Microsoft Windows XP Professional s aktualizací Service Pack 1 nebo Service Pack 2 či bez nich;
-   Microsoft Windows Server 2003, Standard Edition; Windows Server 2003, Enterprise Edition; Windows Server 2003, Datacenter Edition; nebo Windows Server 2003, Web Edition.
