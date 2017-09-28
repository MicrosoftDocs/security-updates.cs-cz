---
TOCTitle: 'Poznámky k verzi aktualizace Windows Server Update Services 3.0 SP2'
Title: 'Poznámky k verzi aktualizace Windows Server Update Services 3.0 SP2'
ms:assetid: 'b3723422-489d-47b7-abfa-663353647da0'
ms:contentKeyID: 21741184
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Dd939886(v=WS.10)'
---

Poznámky k verzi aktualizace Windows Server Update Services 3.0 SP2
===================================================================

Tyto poznámky k verzi popisují službu Windows Server Update Services 3.0 Service Pack 2 (WSUS 3.0 SP2). Tento dokument obsahuje následující části:

1.  Co je nového v této verzi
2.  Systémové požadavky pro instalaci aktualizace WSUS 3.0 SP2 na server
3.  Předpoklady pro konfiguraci a doporučení nejvhodnějších postupů pro server WSUS
4.  Předpoklady pro systém Windows Small Business Server
5.  Systémové požadavky pro instalaci vzdálené konzoly služby WSUS 3.0 SP2
6.  Systémové požadavky pro klientskou instalaci
7.  Požadavky a doporučení týkající se upgradu
8.  Instalace aktualizace WSUS 3.0 SP2
9.  Parametry příkazového řádku instalačního programu pro bezobslužné instalace aktualizace WSUS 3.0 SP2
10. Známé problémy

Co je nového v této verzi
-------------------------

-   Integrace se systémem Windows Server 2008 R2
-   Podpora služby BranchCache v systému Windows Server 2008 R2.
-   Podpora pro klienty systému Windows 7.
-   Zdokonalení klientů služby Agent webu Windows Update (WUA). Nový klient služby WUA nabízí lepší výkon, lepší možnosti použití pro uživatele a řadu oprav chyb, na které nás upozornili zákazníci.
    -   Doba kontroly klientů je kratší, než tomu bylo u předchozích verzí.
    -   U počítačů spravovaných servery WSUS nyní lze provádět namísto úplných kontrol kontroly omezené. Výsledkem bude několikanásobně rychlejší zjišťování aplikací používajících rozhraní API služby Microsoft Update, jako je například program Windows Defender.
    -   Vylepšení možností používání služby WUA pomáhá uživatelům lépe organizovat aktualizace a získat lepší přehled o hodnotě a chování aktualizace.
    -   Počítače s bitovými kopiemi budou na konzole služby WSUS zřetelněji zobrazeny. Další podrobnosti naleznete v článku [Počítače se systémem Windows 2000, Windows Server 2003 nebo Windows XP, které byly nastaveny pomocí bitové kopie systému Windows 2000, Windows Server 2003 nebo Windows XP a nezobrazují se v konzole služby WSUS](http://go.microsoft.com/fwlink/?linkid=159749) (stránka může být v angličtině).
-   Nové funkce:
    -   Pravidla automatického schvalování nyní obsahují schopnost specifikovat datum a čas termínu schválení pro všechny počítače nebo určité skupiny počítačů.
    -   Vylepšené zpracování výběru jazyka pro podřízené servery obsahuje nové dialogové okno s upozorněním, které se zobrazí ve chvíli, kdy se rozhodnete stahovat aktualizace pouze pro určité jazyky.
    -   Nové sestavy o stavu aktualizace a počítače umožňují filtrování aktualizací schválených pro instalaci. Tyto sestavy můžete spouštět z konzoly služby WSUS nebo funkci můžete začlenit do svých sestav pomocí rozhraní API.
-   Uživatelské rozhraní je kompatibilní pro klienta i server služby WSUS 3.0 s aktualizací Service Pack 1 i Service Pack 2.
-   Aktualizace softwaru
-   V této verzi jsou vyřešeny známé potíže s agentem služby Windows Update:
    1.  Služba WSUS 3.0 SP2 a systém Windows 7 obsahují novou verzi služby WUA (pro systémy Windows XP, Windows Vista, Windows Server 2000, Windows Server 2003 a Windows Server 2008). V této verzi je opraven následující problém: Rozhraní API volaná volajícími jiných než místních systémů v neinteraktivní relaci selžou.
    2.  Problém vyřešený verzí 7.2.6001.788 agenta služby Windows Update. V této aktualizaci je opraven následující problém: Při pokusu o instalaci 80 a více aktualizací z webu Windows Update nebo Microsoft Update najednou se může zobrazit chybový kód 0x80070057.
    3.  Vylepšení a potíže vyřešené verzí 7.2.6001.784 agenta služby Windows Update Agent. Do této aktualizace patří například následující: Vylepšení doby vyhledávání ve službě Windows Update, zvýšení rychlosti doručování aktualizací podpisů, povolení podpory pro funkci přeinstalace instalační služby systému Windows a vylepšení chybových zpráv.

<span id="BKMK_SysReqWSUS30SP2"></span>
Systémové požadavky pro instalaci aktualizace WSUS 3.0 SP2 na server
--------------------------------------------------------------------

Tato část popisuje softwarové a hardwarové požadavky pro instalaci aktualizace WSUS 3.0 SP2.

### Předpoklady pro software serveru WSUS

-   Musíte mít nainstalovaný jeden z následujících podporovaných operačních systémů:
    -   Windows Server 2008 R2
    -   Windows Server 2008 SP1 nebo novější
 
        <table style="border:1px solid black;">
        <colgroup>
        <col width="100%" />
        </colgroup>
        <thead>
        <tr class="header">
        <th><img src="images/Dd939886.Warning(WS.10).gif" />Upozornění</th>
        </tr>
        </thead>
        <tbody>
        <tr class="odd">
        <td style="border:1px solid black;">Jestliže bude aktualizace WSUS 3.0 SP2 nainstalovaná v systému Windows Server 2008 před provedením upgradu na systém Windows Server 2008 R2, upgrade na systém Windows Server 2008 R2 se nezdaří. Další informace naleznete v tématu <a href="#bkmk_knownissues">Známé problémy</a>.
        </td>
        </tr>
        </tbody>
        </table>
 

    -   Windows Server 2003 SP1 nebo novější
    -   Windows Small Business Server 2008
    -   Windows Small Business Server 2003

    Pozor, další předpoklady se vztahují na systém Windows Small Business Server. Další informace získáte v části Předpoklady pro systém Windows Small Business Server.
-   Internetová informační služba (IIS) 6.0 nebo novější verze
-   Microsoft .NET Framework 2.0 nebo novější verze
-   Musíte mít nainstalovanou jednu z následujících podporovaných databází:
    -   Microsoft SQL Server 2008 Standard nebo Enterprise Edition
    -   Microsoft SQL Server 2005 SP3 nebo novější verze
    -   Interní databáze systému Windows

    Pokud není nainstalována jedna z podporovaných verzí systému SQL Server, průvodce instalací služby WSUS 3.0 SP2 nainstaluje interní databázi systému Windows.
-   Konzola Microsoft Management Console 3.0
-   Prohlížeč Microsoft Report Viewer Redistributable 2008

 
<table style="border:1px solid black;">
<colgroup>
<col width="100%" />
</colgroup>
<thead>
<tr class="header">
<th><img src="images/Dd939886.Important(WS.10).gif" />Důležité</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Windows Server 2008 R2 vyžaduje službu WSUS 3.0 SP2. Pokud instalujete Windows Server 2008 R2, měli byste nainstalovat službu WSUS 3.0 SP2. Do systému Windows Server 2008 R2 neinstalujte službu WSUS 3.0 SP1.

U služby WSUS 3.0 SP2 není podporováno použití s Terminálovou službou na front-end serveru ve vzdálené konfiguraci SQL.
</td>
</tr>
</tbody>
</table>
 

### Softwarové předpoklady konzoly pro správu služby WSUS

-   Jeden z následujících podporovaných operačních systémů: Windows Server 2008 R2, Windows Server 2008, Windows Server 2003 SP2 nebo novější verze, Windows Small Business Server 2008 nebo Windows Small Business Server 2003, Windows Vista nebo Windows XP SP2
-   Microsoft .NET Framework 2.0 nebo novější
-   Konzola Microsoft Management Console 3.0
-   Prohlížeč Microsoft Report Viewer Redistributable 2008

### Minimální hardwarové požadavky serveru WSUS

V následujícím seznamu jsou uvedeny minimální hardwarové požadavky, kterým je třeba vyhovět u základní instalace na serveru. Podrobný seznam podporovaných konfigurací hardwaru naleznete v průvodci nasazením služby WSUS 3.0 SP2 na adrese [http://go.microsoft.com/fwlink/?LinkId=139832](http://go.microsoft.com/fwlink/?linkid=139832) (stránka může být v angličtině).

-   Systémový oddíl i oddíl, do kterého instalujete službu WSUS 3.0 SP2, musí být formátovány pomocí systému souborů NTFS.
-   Minimálně 1 GB volného místa v systémovém oddílu.
-   Minimálně 2 GB volného místa ve svazku, ve kterém budou uloženy soubory databáze.
-   Minimálně 20 GB volného místa je vyžadováno ve svazku, ve kterém je uložen obsah. Doporučeno je 30 GB.

 
<table style="border:1px solid black;">
<colgroup>
<col width="100%" />
</colgroup>
<thead>
<tr class="header">
<th><img src="images/Dd939886.Important(WS.10).gif" />Důležité</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Službu WSUS 3.0 SP2 nelze nainstalovat do komprimovaných jednotek.
</td>
</tr>
</tbody>
</table>
 

Předpoklady pro konfiguraci a doporučení nejvhodnějších postupů pro server WSUS
-------------------------------------------------------------------------------

Před instalací služby WSUS 3.0 SP2 proveďte potřebné úlohy v této části.

### Internetová informační služba

-   Na stránce služeb rolí webového serveru (IIS) správce serveru nainstalujte všechny požadované funkce, všechny výchozí služby role služby IIS a následující služby rolí: **ASP.NET**, **Ověřování systému Windows**, **Komprese dynamického obsahu** a **Kompatibilita správy služby IIS 6**.
-   Pokud internetová informační služba běží v režimu izolace služby IIS 5.0, instalace se nezdaří. Před instalací služby WSUS 3.0 SP2 zakažte režim izolace služby IIS 5.0.
-   Pokud je jakákoli součást služby IIS nainstalovaná na 64bitové platformě v režimu kompatibility s 32bitovými aplikacemi, nemusí se instalace služby WSUS 3.0 SP2 zdařit. Všechny součásti internetové informační služby by měly být na 64bitových platformách nainstalované v nativním režimu.

### Proxy servery

Služba WSUS 3.0 SP2 umožňuje proxy serverům podporovat pouze protokol HTTP. Před konfigurací serveru služby WSUS pomocí Průvodce konfigurací nebo Konzoly pro správu je vhodné pomocí příkazového řádku (**wsusutil configuresslproxy**) nakonfigurovat druhý proxy server s protokolem HTTPS.

### Webové servery spuštěné na portu 80

Pokud na portu 80 běží dva nebo více webových serverů (například služba Windows SharePoint Services), odstraňte před instalací služby WSUS všechny weby s výjimkou jednoho. Pokud tak neučiníte, automatická aktualizace klientů serveru se pravděpodobně nezdaří.

### Antivirové programy

Aby bylo možné úspěšně nainstalovat službu WSUS 3.0 SP2, bude pravděpodobně nutné zakázat antivirové programy. Po zákazu antivirových programů restartujte počítač a až poté nainstalujte službu WSUS. Restartováním počítače zabráníte uzamčení souborů v okamžiku, kdy instalační proces bude potřebovat získat přístup k těmto souborům. Po dokončení instalace nezapomeňte znovu povolit antivirový software. Přesný postup při zakázání a opětovném povolení používané verze antivirového softwaru naleznete na webu výrobce daného softwaru.

 
<table style="border:1px solid black;">
<colgroup>
<col width="100%" />
</colgroup>
<thead>
<tr class="header">
<th><img src="images/Dd939886.Caution(WS.10).gif" />Upozornění</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Uvedený postup může způsobit, že počítač nebo síť budou náchylnější k útokům uživatelů se zlými úmysly nebo k útokům škodlivého softwaru, například virů. Společnost Microsoft toto řešení nedoporučuje, ale poskytuje tuto informaci, aby mohlo být toto řešení použito podle vlastního uvážení. Používejte toto řešení pouze na vlastní riziko.

Antivirový software pomáhá chránit počítač proti virům. V době, kdy je antivirový program zakázaný, nestahujte nebo neotevírejte soubory ze zdrojů, kterým nedůvěřujete, a neotevírejte e-mailové přílohy.
</td>
</tr>
</tbody>
</table>
 

### Možnost vnořených aktivačních událostí v systému SQL Server

Jestliže máte v plánu používat databázi systému SQL Server jako datové úložiště služby Windows Server Update Services, měl by správce systému SQL Server ověřit, že je na serveru zapnutá možnost vnořených aktivačních událostí, a to ještě před tím, než správce služby WSUS nainstaluje aktualizaci WSUS 3.0 SP2. Ve výchozím nastavení je možnost vnořených aktivačních událostí zapnutá. Správce systému SQL Server ji však může vypnout. Instalace aktualizace WSUS 3.0 SP2 zapne možnost RECURSIVE\_TRIGGERS, která je specifická pro konkrétní databázi. Nezapne však možnost vnořených aktivačních událostí, což je globální možnost serveru.

### Omezení a požadavky vzdáleného serveru SQL

Služba WSUS 3.0 SP2 podporuje běh kompatibilní verze softwaru systému SQL Server v počítači, který je oddělený od počítače se spuštěnou aplikací služby WSUS 3.0 SP2. Na vzdálenou instalaci serveru SQL se vztahují následující požadavky.

-   Jako serverovou část v páru klient-server vzdáleného serveru SQL nelze použít server nakonfigurovaný jako řadič domény.
-   V počítači, který bude použit jako server front-end vzdálené instalace systému SQL, nesmí běžet Terminálová služba.
-   Klientský i serverový počítač musí být přidány do domény služby Active Directory. Pokud jsou klientský i serverový počítač v různých doménách, je nutné před spuštěním instalace služby WSUS vytvořit mezi doménami vztah důvěryhodnosti.
-   V případě, že již máte nainstalovanou službu WSUS 2.0 v konfiguraci se vzdáleným systémem SQL a chcete provést upgrade na verzi WSUS 3.0 SP2, měli byste před instalací služby WSUS postupovat podle následujících pokynů:
    1.  Odinstalovat službu WSUS 2.0 (pomocí ovládacího panelu **Přidat nebo odebrat programy**) a zároveň zajistit, aby existující databáze zůstala nezměněna.
    2.  Nainstalovat SQL Server 2005 SP2 nebo SQL Server 2008 a provést upgrade existující databáze.

### Internetová informační služba bude při instalaci aktualizace WSUS 3.0 SP2 restartována.

Instalační program pro aktualizaci WSUS 3.0 SP2 bez upozornění restartuje službu IIS, což by mohlo mít vliv na současné weby ve vaší organizaci. Před touto instalací je vhodné strany, kterých se to týká, informovat. Pokud není služba IIS spuštěná, instalační program aktualizace WSUS 3.0 SP2 ji během instalace spustí.

Předpoklady pro systém Windows Small Business Server
----------------------------------------------------

Pokud instalujete aktualizaci WSUS 3.0 SP2 do systému Windows Small Business Server, je nutné splnit následující předpoklady.

### Když je virtuální kořenový adresář internetové informační služby omezen na určité IP adresy nebo na názvy domén.

Některé instalace serveru Windows Small Business Server mohou mít výchozí web služby IIS nakonfigurován na omezení **IP adres a názvů domény**. Je-li tomu tak, klient služby Windows Update na serveru se možná nebude moci aktualizovat. Před instalací aktualizace WSUS 3.0 SP2 toto omezení odstraňte.

### Pokud používáte proxy server ISA

-   Pokud Windows Small Business Server využívá pro přístup k Internetu proxy server ISA, zadejte v uživatelském rozhraní **Nastavenínastavení proxy serveru, název proxy serveru a port**.
-   Pokud server ISA používá ověření systému Windows, pověření proxy serveru by měla být zadána ve tvaru *DOMÉNA*\\*uživatel*. Uživatel by měl být členem skupiny Internet Users.

### Pokud jste do své sítě přidali podsíť a nepoužili jste průvodce systému Windows Small Business Server.

Instalační proces serveru WSUS nainstaluje na server dvě virtuální kořenové složky Internetové informační služby: SelfUpdate a ClientWebService. Instalační program také umístí některé soubory do kořenového adresáře výchozího webu (na portu 80), což umožní klientským počítačům automatickou aktualizaci prostřednictvím výchozího webu. Ve výchozím nastavení je výchozí web nakonfigurován tak, aby odmítl přístup ke každé IP adrese jiné než localhost nebo ke konkrétním podsítím připojeným k serveru. V důsledku toho se klientské počítače, které nejsou počítačem localhost ani některou z určených podsítí, nemohou samy aktualizovat. Pokud jste do sítě přidali podsíť bez použití průvodce systému Microsoft Windows Small Business Server, je nutné provést následující kroky:

1.  V nástroji Správa serveru rozbalte položky **Rozšířená správa**, **Internetová informační služba**, **Webové servery**, **Výchozí webový server**, klikněte pravým tlačítkem na virtuální adresář **Selfupdate** a potom klikněte na příkaz **Vlastnosti**.
2.  Klikněte na položku **Zabezpečení adresáře**.
3.  V části **Omezení podle adres IP a názvů domén** klikněte na tlačítko **Upravit** a potom klikněte na přepínač **Udělit přístup**.
4.  Klikněte na tlačítko **OK**, klikněte pravým tlačítkem na virtuální adresář **ClientWebService** a poté klikněte na příkaz **Vlastnosti**.
5.  Klikněte na položku **Zabezpečení adresáře**.
6.  V části **Omezení podle adres IP a názvů domén** klikněte na tlačítko **Upravit** a potom klikněte na přepínač **Udělit přístup**.

Systémové požadavky pro instalaci vzdálené konzoly služby WSUS 3.0 SP2
----------------------------------------------------------------------

Vzdálenou konzolu služby WSUS 3.0 SP2 lze nainstalovat do libovolného z následujících operačních systémů:

-   Windows Server 2008 R2, Windows Server 2008 SP1 a novější verze, Windows Server 2003 SP2 a novější verze, Windows Small Business Server 2003, Windows Small Business Server 2005 nebo Windows Small Business Server 2008, Windows Vista nebo Windows XP Professional SP2 a novější verze.

Systémové požadavky pro klientskou instalaci služby WSUS
--------------------------------------------------------

Automatické aktualizace, klientský software služby WSUS, lze nainstalovat na libovolný z následujících operačních systémů:

-   Windows Server 2008 R2, Windows Server 2008 SP1 a novější verze, Windows Server 2003 SP2 a novější verze, Windows Small Business Server 2003, Windows Small Business Server 2005 nebo Windows Small Business Server 2008, Windows Vista, Windows XP Professional RTM, Windows XP Professional SP1, Windows XP Professional SP2, Windows XP Professional SP3 a novější verze, Windows 2000 SP4 nebo klient systému Windows 7.

Požadavky a doporučení týkající se upgradu
------------------------------------------

Následující verze služby WSUS lze upgradovat na službu WSUS 3.0 SP2 a nevyžadují odinstalaci předchozí verze:

-   WSUS 2.0, 2.0 SP1, 3.0 a 3.0 SP1.

Upgrady z verze služby WSUS 1.0 na verzi 3.0 SP2 nejsou podporovány. Před instalací aktualizace WSUS 3.0 SP2 odinstalujte službu SUS 1.0.

Windows Server 2008 R2 vyžaduje službu WSUS 3.0 SP2. Pokud instalujete Windows Server 2008 R2, měli byste nainstalovat službu WSUS 3.0 SP2. Do systému Windows Server 2008 R2 neinstalujte službu WSUS 3.0 SP1.

#### Postup před provedením upgradu na službu WSUS 3.0 SP2

1.  Zkontrolujte, zda se v protokolech událostí nevyskytují chyby z nedávné doby, zda nedocházelo k problémům v synchronizaci serverů přijímajících data a odesílajících data nebo k problémům s klienty, kteří hlásili potíže. Před provedením upgradu tyto potíže vyřešte.

2.  Můžete také spustit příkaz DBCC CHECKDB a přesvědčit se, zda je databáze WSUS správně indexována. Další informace o příkazu DBCC CHECKDB naleznete zde: [DBCC CHECKDB](http://go.microsoft.com/fwlink/?linkid=86948).

3.  Zálohujte databázi služby WSUS. Instalace aktualizace WSUS 3.0 SP2 přidá novou databázi do výchozího adresáře, což je *jednotka*\\WSUS (kde *jednotka* je místní jednotka NTFS s největším množstvím volného místa). Pokud se již v tomto adresáři nachází záloha databáze, bude pravděpodobně přepsána. Před upgradem na verzi WSUS 3.0 SP2 je vhodné uložit zálohu databáze aktuální verze služby WSUS do jiného umístění.

4.  Pokud ručně změníte port používaný službou WSUS (v případě, že nepoužíváte nástroj Wsusutil) a máte právě spuštěnou službu SUS 1.0 nebo WSUS 2.0, spusťte před odinstalací služby SUS 1.0 nebo 64bitové verze služby WSUS 2.0 výchozí web.

5.  Pokud jsou otevřena spojení do stávající databáze služby WSUS (například, když je spuštěna aplikace SQL Server Management Studio), může instalace selhat. Před instalací aktualizace WSUS 3.0 SP2 všechna spojení uzavřete.

### Obnovení z neúspěšného upgradu

Pokud provádíte upgrade z předchozí verze služby WSUS na verzi WSUS 3.0 SP2 a upgrade se nezdaří (z jakéhokoli důvodu jiného, než je pokus o nepodporovaný upgrade ze služby SUS 1.0), postupujte takto:

1.  Přeinstalujte předchozí verzi služby WSUS.
2.  Obnovte databázi ze zálohy, kterou jste vytvořili před pokusem o upgrade. Upgrade nelze provést, pokud existuje databáze služby WSUS 3.0 SP2 z předchozí instalace. Ve většině případů také služba WSUS automaticky vytvoří zálohu. Její umístění zjistíte v souboru WSUSSetup.log.
3.  Pomocí protokolů určete příčinu neúspěchu upgradu a vyřešte problém.
4.  Nainstalujte aktualizaci WSUS 3.0 SP2.

### Změna názvu počítače provedená před upgradem na službu WSUS 3.0 SP2 může způsobit selhání tohoto upgradu.

Pokud změníte název počítače po instalaci služby WSUS 2.0 a před provedením upgradu na službu WSUS 3.0 SP2, nemusí se upgrade zdařit.

Pomocí následujícího skriptu odeberte a znovu přidejte skupiny ASPNET a WSUS Administrators. Poté spusťte upgrade znovu.

        ```

### Pokud jste ve službě WSUS 2.0 provedli migraci ze serveru MSDE na SQL Server 2008 nebo SQL Server 2005, bude potřeba změnit hodnotu registru.

Pokud máte nainstalovanou službu WSUS 2.0 a provedli jste migraci na SQL Server 2008 nebo SQL Server 2005, bude nutné změnit hodnotu registru **HKLM\\SOFTWARE\\Microsoft\\Update Services\\Server\\Setup\\WmsdeInstalled** z 1 na 0. Pokud tak neučiníte před upgradem na verzi WSUS 3.0 SP2, upgrade se nezdaří.

### Pokud odinstalujete aktualizaci WSUS 3.0 SP2 a zachováte soubory protokolu, budou tyto soubory mít po opětovné instalaci pravděpodobně nesprávná oprávnění.

Během odinstalace aktualizace WSUS 3.0 SP2 máte možnost uchovat soubory protokolu o instalaci. Když znovu nainstalujete aktualizaci WSUS 3.0 SP2, mohou původní soubory protokolu ztratit svá oprávnění (většinou pouze pro skupinu WSUS Administrators). Po instalaci je vhodné na těchto souborech protokolu potvrdit oprávnění.

### Jestliže mají klienti služby WSUS 2.0 aktualizace se stavem Nelze použít, bude jejich stav krátce po upgradu na verzi WSUS 3.0 SP2 označen jako Neznámý.

Pokud má server se službou WSUS 2.0 klienty s aktualizacemi ve stavu **Nelze použít**, mohou mít tyto aktualizace krátce po upgradu serveru na verzi WSUS 3.0 SP2 stav **Neznámý**. Stav aktualizace se poté, co klient provede prohledání, vrátí na **Nelze použít**.

Instalace aktualizace WSUS 3.0 SP2
----------------------------------

Podrobný průvodce instalací služby WSUS na adrese [http://go.microsoft.com/fwlink/?LinkId=139836](http://go.microsoft.com/fwlink/?linkid=139836) obsahuje pokyny k instalaci aktualizace WSUS 3.0 SP2 s použitím Správce serveru Windows nebo souboru WSUSSetup.exe (stránka může být v angličtině).

Kompletní informace o instalaci a použití služby WSUS naleznete zde:

Příručka pro nasazení služby WSUS na adrese [http://go.microsoft.com/fwlink/?LinkId=139832](http://go.microsoft.com/fwlink/?linkid=139832) (stránka může být v angličtině)

Provozní příručka služby WSUS na adrese [http://go.microsoft.com/fwlink/?LinkId=139838](http://go.microsoft.com/fwlink/?linkid=139838) (stránka může být v angličtině)

Parametry příkazového řádku instalačního programu pro bezobslužné instalace aktualizace WSUS 3.0 SP2
----------------------------------------------------------------------------------------------------

Pomocí instalačního programu služby WSUS s příkazovým řádkem lze provádět bezobslužné instalace aktualizace WSUS 3.0 SP2. Následující tabulka obsahuje parametry příkazového řádku pro instalaci aktualizace WSUS 3.0 SP2.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Možnost</th>
<th>Popis</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>/q</strong></td>
<td style="border:1px solid black;">Tichá instalace</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>/u</strong></td>
<td style="border:1px solid black;">Odinstalace</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>/p</strong></td>
<td style="border:1px solid black;">Kontrola předpokladů Zkontroluje systém a ohlásí případné chybějící předpoklady.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>/?, /h</strong></td>
<td style="border:1px solid black;">Zobrazení parametrů příkazového řádku a jejich popisů</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>/g</strong></td>
<td style="border:1px solid black;">Upgrade z předchozí verze služby WSUS (Aktualizace ze služby SUS 1.0 nejsou podporovány.) Jediným platným parametrem této možnosti je /q (tichá instalace). Jedinou platnou vlastností této možnosti je DEFAULT_WEBSITE.</td>
</tr>
</tbody>
</table>
  
Následující tabulka uvádí vlastnosti příkazového řádku pro aktualizaci WSUS 3.0 SP2.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Vlastnost</th>
<th>Popis</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">CONTENT_LOCAL</td>
<td style="border:1px solid black;">0 = obsah hostován místně, 1 = obsah na serveru Microsoft Update</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">CONTENT_DIR</td>
<td style="border:1px solid black;">Cesta k adresáři obsahu. Výchozí cesta je <em>Instalační_jednotka_WSUS\WSUS\WSUSContent</em>, kde <em>Instalační_jednotka_WSUS</em> je místní jednotka s největším množstvím volného místa.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">WYUKON_DATA_DIR</td>
<td style="border:1px solid black;">Cesta k adresáři interní databáze systému Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">SQLINSTANCE_NAME</td>
<td style="border:1px solid black;">Tento název by měl být ve formátu <em>Nazev_serveru</em>\<em>Nazev_instance_SQL</em>. Pokud je instance databáze v místním počítači, použijte proměnnou prostředí %COMPUTERNAME%. Pokud není k dispozici existující instance, výchozí hodnota je %COMPUTERNAME%\WSUS.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DEFAULT_WEBSITE</td>
<td style="border:1px solid black;">0=port 8530, 1=port 80</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PREREQ_CHECK_LOG</td>
<td style="border:1px solid black;">Cesta k souboru protokolu a název tohoto souboru</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">CONSOLE_INSTALL</td>
<td style="border:1px solid black;">0 = instalovat server služby WSUS, 1 = instalovat pouze konzolu</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">ENABLE_INVENTORY</td>
<td style="border:1px solid black;">0 = neinstalovat funkce inventarizace, 1 = instalovat funkce inventarizace</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DELETE_DATABASE</td>
<td style="border:1px solid black;">0 = zachovat databázi, 1 = odebrat databázi</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DELETE_CONTENT</td>
<td style="border:1px solid black;">0 = zachovat soubory obsahu, 1 = odebrat soubory obsahu</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DELETE_LOGS</td>
<td style="border:1px solid black;">0 = zachovat soubory protokolu, 1 = odebrat soubory protokolu (použití s přepínačem instalace /u)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">CREATE_DATABASE</td>
<td style="border:1px solid black;">0 = použít aktuální databázi, 1 = vytvořit databázi</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">PROGRESS_WINDOW_HANDLE</td>
<td style="border:1px solid black;">Popisovač okna vracející zprávy o průběhu Instalační služby systému Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">MU_ROLLUP</td>
<td style="border:1px solid black;">1 = zapojit se do programu zlepšování služby Microsoft Update, 0 = nezapojit se do programu zlepšování služby Microsoft Update</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">FRONTEND_SETUP</td>
<td style="border:1px solid black;">1 = nezapisovat umístění obsahu do databáze, 0 = zapisovat umístění obsahu do databáze (pro službu Vyrovnávání zatížení sítě)</td>
</tr>
</tbody>
</table>
  
### Příklad použití
  
```  
WSUSSetup.exe /q DEFAULT\_WEBSITE=0 (instalovat v tichém režimu s použitím portu 8530) WSUSSetup.exe /q /u (odinstalovat službu WSUS)  
```
 
<table style="border:1px solid black;">
<colgroup>
<col width="100%" />
</colgroup>
<thead>
<tr class="header">
<th><img src="images/Dd939886.Important(WS.10).gif" />Důležité</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Pokud instalujete aktualizaci WSUS 3.0 SP2 v tichém režimu (/q) a v počítači nejsou nainstalovány všechny nezbytné předpoklady, vygeneruje se v průběhu instalace soubor WSUSPreReqCheck.xml a uloží se do adresáře %TEMP%.
</td>
</tr>
</tbody>
</table>
 

<span id="BKMK_KnownIssues"></span>
Známé problémy
--------------

-   Po úspěšném dokončení průvodce instalací služby WSUS se uživateli zobrazí výzva, aby kliknul na tlačítko **Dokončit**. Ve výjimečných případech se zobrazí chybové dialogové okno se zprávou **Během komunikace se serverem došlo k chybě a tento průvodce musí být ukončen. Průvodce konfigurací serveru služby WSUS můžete znovu spustit ze stránky Možnosti v konzole služby WSUS.** Abyste měli jistotu, že byly vybrané možnosti instalace uloženy, otevřete stránku **Možnosti** v konzole pro správu služby WSUS a ve všech částech potvrďte nastavení.
-   **Lokalizované verze klienta WUA budou vydány později než aktualizace WSUS 3.0 SP2**. Tato situace nastala v důsledku závislosti na plánu lokalizace systému Windows 7. V době mezi verzí WSUS 3.0 SP2 a lokalizovanou verzí klienta WUA bude klient WUA podporovat pouze pět jazyků (angličtinu, němčinu, francouzštinu, španělštinu a japonštinu).
-   **Nové sestavy o stavu aktualizace a počítače, které přinesla tato verze SP2, nejsou funkční v prostředí, kde jsou servery pro příjem dat s dřívější verzí služby WSUS 3.0 SP1 spravovány ze serveru se službou WSUS 3.0 SP2**. Pokud jsou pro server s aktualizací SP1 spuštěny nové sestavy, zobrazí se zpráva „Během vytváření hlášení došlo k chybě. Zkuste spustit hlášení znovu nebo kontaktujte správce sítě, pokud potíže přetrvávají.“ Opakovaným spuštěním sestavy tento problém nevyřešíte. Problém nemá ani žádnou souvislost se sítí. Nové sestavy jsou závislé na funkcích rozhraní API, které ve verzi SP1 neexistují. Konzola pro správu s verzí SP2 však nebude blokovat nové sestavy při správě serveru s verzí SP1.
-   **Upgrade na verzi WSUS 3.0 SP2 se nezdaří, když je protokol SSL konfigurován bez názvu certifikátu**. Pro konfiguraci protokolu SSL je požadován název certifikátu.
-   **Interní databáze systému Windows spuštěná se službou WSUS 3.0 SP2 a nainstalovaná v systému Windows Server 2008 zabrání upgradu na systém Windows Server 2008 R2**. Než budete pokračovat s upgradem na systém Windows Server 2008 R2, zobrazí se chybová zpráva o kompatibilitě s pokynem, že máte vypnout Interní databáze systému Windows. Je nutné nejdříve provést upgrade Interní databáze systému Windows a teprve potom může pokračovat upgrade na systém Windows Server 2008 R2. Pokyny a další informace o upgradu Interní databáze systému Windows získáte v tématu s informacemi [Jak získat nejnovější verzi aktualizace Service Pack pro interní databázi systému Windows](http://go.microsoft.com/fwlink/?linkid=162104) (http://go.microsoft.com/fwlink/?LinkId=162104) (stránka může být v angličtině).

Informace o autorských právech
------------------------------

Informace v tomto dokumentu včetně adres URL a dalších odkazů na web se mohou změnit bez předchozího upozornění. Pokud není uvedeno jinak, jsou názvy společností, organizací, produktů, názvy domén, e-mailové adresy, loga, osoby, místa či události použité v příkladech smyšlené. Není zamýšleno a nemůže být vyvozováno žádné jejich spojení se skutečnou společností, organizací, produktem, názvem domény, e-mailovou adresou, logem, osobou, místem či událostí. Povinností uživatele je dodržet všechny zákonné normy týkající se autorských práv. Bez omezení práv vyplývajících z autorských práv nesmí být žádná část tohoto dokumentu kopírována, uložena do veřejného systému ani rozšiřována jakýmkoli způsobem (elektronicky, mechanicky, fotokopiemi, záznamem nebo jinak) ani za žádným účelem bez výslovného písemného povolení společnosti Microsoft Corporation.

Společnost Microsoft může vlastnit patenty, patentové přihlášky, ochranné známky, autorská práva a další práva týkající se duševního vlastnictví, které se vztahují k předmětu tohoto dokumentu. Není-li výslovně uvedeno jinak v písemné licenční smlouvě se společností Microsoft, neposkytuje tento dokument žádnou licenci na uvedené patenty, ochranné známky, autorská práva nebo jiné duševní vlastnictví.

© 2009 Microsoft Corporation. Všechna práva vyhrazena.

Microsoft, Active Directory, ActiveX, Authenticode, Excel, InfoPath, Internet Explorer, MSDN, Outlook, Visual Studio, Win32, Windows, Windows Server a Windows Vista jsou ochranné známky skupiny společností Microsoft.

Všechny ostatní ochranné známky jsou ochrannými známkami příslušných vlastníků.
