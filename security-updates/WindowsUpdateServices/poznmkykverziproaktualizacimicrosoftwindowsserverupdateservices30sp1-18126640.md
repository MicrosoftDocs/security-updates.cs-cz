---
TOCTitle: 'Poznámky k verzi pro aktualizaci Microsoft Windows Server Update Services 3.0 SP1'
Title: 'Poznámky k verzi pro aktualizaci Microsoft Windows Server Update Services 3.0 SP1'
ms:assetid: 'a5aa93bf-842b-4ad4-ab0f-fe867843cb02'
ms:contentKeyID: 18126640
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc708525(v=WS.10)'
---

Poznámky k verzi pro aktualizaci Microsoft Windows Server Update Services 3.0 SP1
=================================================================================

Tyto poznámky popisují známé problémy ovlivňující aktualizaci Service Pack 1 služby Microsoft® Windows® Server Update Services (WSUS) 3.0 a obsahují doporučení a požadavky k instalaci aplikace. Poznámky obsahují následující části:

-   Požadavky na systém pro instalaci serveru aktualizace WSUS 3.0 SP1
-   Požadavky na konfiguraci pro instalaci serveru aktualizace WSUS 3.0 SP1
-   Požadavky na systém pro instalaci vzdálené konzoly aktualizace WSUS 3.0 SP1
-   Požadavky na systém pro klientskou instalaci
-   Požadavky na software pro instalaci serveru aktualizace WSUS SP1
-   Požadavky na místo na disku pro instalaci serveru aktualizace WSUS 3.0 SP1
-   Požadavky na upgrade aktualizací WSUS 3.0 SP1
-   Nastavení parametrů příkazového řádku
-   Problémy při instalaci
-   Problémy s upgradem
-   Známé problémy
-   Aktualizace WSUS 3.0 SP1 na serveru Windows Server® 2008
-   Aktualizace WSUS 3.0 SP1 na serveru Windows Small Business Server 2003

Požadavky na systém pro instalaci serveru aktualizace WSUS 3.0 SP1
------------------------------------------------------------------

#### Server aktualizace WSUS 3.0 SP1 je podporován systémy Windows Server 2008 a Windows Server 2003 Service Pack 1.

Server WSUS 3.0 SP1 je podporován v systémech Windows Server 2008 a Windows Server 2003 Service Pack 1.

#### Servery aktualizace WSUS 3.0 SP1 nepodporují systém Windows 2000 Server.

Operační systém Microsoft Windows® 2000 Server není servery aktualizace WSUS 3.0 SP1 podporován.

#### Aktualizace WSUS 3.0 SP1 není podporována na serverech s Terminálovou službou.

Přestože aktualizace WSUS 3.0 SP1 pravděpodobně na serverech s Terminálovou službou poběží, není tato možnost podporována a doporučována. Aktualizace WSUS 3.0 SP1 nepoběží na serveru s Terminálovou službou v konfiguracích využívajících vzdálené implementace serveru SQL Server. Jelikož všechny vzdálené uživatelské akce (včetně instalace) na licenčním serveru Terminálové služby budou spuštěny jako systémový účet a systémový účet serveru nemusí mít oprávnění na vzdáleném serveru SQL Server, instalace se nemusí zdařit.

Požadavky na konfiguraci pro instalaci serveru aktualizace WSUS 3.0 SP1
-----------------------------------------------------------------------

#### Musí být nainstalována služba IIS.

Aktualizace WSUS 3.0 SP1 požaduje službu IIS (Internet Information Services), která není ve výchozím nastavení v systémech Windows Server 2008 a Microsoft Windows Server 2003 nainstalována. Pokud se pokusíte aktualizaci WSUS 3.0 SP1 nainstalovat bez služby IIS, zobrazí instalační program služby Windows Server Update Services chybovou zprávu o nenainstalované službě IIS.

#### Pokud služba IIS běží v režimu izolace služby IIS 5.0, instalace se nezdaří.

Pokud jste provedli upgrade serveru z Windows 2000 Server na Windows Server 2003, služba IIS bude pravděpodobně běžet v režimu kompatibility služby IIS 5.0. Režim izolace služby IIS 5.0 lze také povolit ve Správci služby IIS. Pokud tak učiníte, instalace se nezdaří. Před instalací aktualizace WSUS 3.0 SP1 je nutné zakázat režim izolace služby IIS 5.0.

#### Instalace aktualizace WSUS 3.0 SP1 se pravděpodobně nezdaří, pokud je některá ze součástí služby IIS nainstalována v 32bitovém režimu kompatibility na 64bitové platformě.

Všechny součásti služby IIS by měly být nainstalovány v nativním režimu na 64bitových platformách. Pokud je některá ze součástí služby IIS ve 32bitovém režimu kompatibility, instalace se pravděpodobně nezdaří.

#### Servery proxy pravděpodobně podporují pouze protokol HTTP, nebo protokol HTTP a HTTPS.

V aktualizaci WSUS 3.0 SP1 může server proxy podporovat pouze protokol HTTP. Před konfigurací serveru služby WSUS pomocí Průvodce konfigurací nebo Konzoly pro správu byste měli pomocí příkazového řádku (**wsusutil configuresslproxy**) nakonfigurovat druhý server proxy, na kterém běží protokol HTTPS.

#### Jestliže na portu 80 již běží dva nebo více webů, odstraňte před instalací služby WSUS všechny tyto weby kromě jednoho.

Pokud na portu 80 běží dva nebo více webů (například služba Windows® SharePoint® Services), měli byste před instalací služby WSUS odstranit všechny weby kromě jednoho z nich. Pokud tak neučiníte, automatická aktualizace klientů vašeho serveru se pravděpodobně nezdaří.

#### Během instalace aktualizace WSUS 3.0 SP1 bude pravděpodobně nutné zakázat antivirové programy.

Během instalace aktualizace WSUS 3.0 SP1 bude pravděpodobně k úspěšnému provedení instalace potřeba zakázat antivirové programy. Po zakázání antivirových programů restartujte počítač a až poté nainstalujte službu WSUS. Restartováním počítače zabráníte uzamčení souborů v okamžiku, kdy instalační proces bude potřebovat získat přístup k těmto souborům. Po dokončení instalace nezapomeňte znovu povolit antivirový program. Přesný postup při zakázání a opětovném povolení používané verze antivirového programu naleznete na webu výrobce daného programu.

| ![](images/Cc708525.Caution(WS.10).gif)Upozornění                                                                                                                                                                                                                                                 |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Uvedený postup může způsobit, že počítač nebo síť budou náchylnější k útokům uživatelů se zlými úmysly nebo k útokům škodlivého softwaru, například virů. Tento postup nedoporučujeme. Uvedené informace poskytujeme, aby uživatel daný postup použil podle vlastního uvážení. Uvedený postup používejte na vlastní nebezpečí. |

| ![](images/Cc708525.note(WS.10).gif)Poznámka                                                                                                                                |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Antivirový program slouží k ochraně počítače před viry. V době, kdy je antivirový program zakázaný, nesmíte stahovat nebo otevírat soubory ze zdrojů, kterým nedůvěřujete, a otevírat e-mailové přílohy. |

#### Aktualizace WSUS 3.0 SP1 vyžaduje, aby na serveru SQL Server byla zapnuta možnost vnořených aktivačních událostí.

Ve výchozím nastavení je možnost vnořených aktivačních událostí zapnuta, může však být vypnuta správcem serveru SQL Server.

Pokud plánujete jako úložiště dat služby Windows Server Update Services použít server SQL Server, měl by správce tohoto serveru ověřit, že možnost vnořených aktivačních událostí je na serveru zapnuta dříve, než správce aktualizace WSUS 3.0 SP1 nainstaluje aktualizaci WSUS 3.0 SP1 a vybere databázi v průběhu instalace.

Instalační program aktualizace WSUS 3.0 SP1 zapne možnost RECURSIVE\_TRIGGERS, která je specifická pro databázi. Nezapne však možnost vnořených aktivačních událostí, což je globální možnost serveru.

Chcete-li zjistit, jestli je možnost vnořených aktivačních položek zapnuta, použijte následující příkaz:

**sp\_configure 'nested triggers'**

Chcete-li zapnout možnost vnořených aktivačních položek na serveru SQL Server, spusťte následující příkaz z dávkového souboru na počítači, na kterém běží server SQL Server.

**sp\_configure 'nested triggers', 1**

**GO**

**RECONFIGURE**

**GO**

Pokud na serveru nemáte program SQL Server Management Studio, můžete spustit skripty SQL z příkazového řádku. Nástroj Microsoft SQL Server 2005 Command Line Query Utility lze získat z webu služby [Stažení softwaru](http://go.microsoft.com/fwlink/?linkid=70728) (http://go.microsoft.com/fwlink/?LinkId=70728). Začněte spuštěním nástroje **sqlcmd**.

Jestliže chcete skripty SQL spustit zacílené na databázi Interní databáze systému Windows, je také nutné stáhnout ze stejné stránky nástroj SQL Server Native Client.

#### Omezení a požadavky vzdáleného serveru SQL

Aktualizace WSUS 3.0 SP1 podporuje spuštění databázového softwaru na jiném počítači, než na kterém je zbytek aplikace aktualizace WSUS 3.0 SP1. Chcete-li nakonfigurovat instalaci vzdáleného serveru SQL, je potřeba splnit určité požadavky:

-   Jako serverovou část v páru klient-server vzdáleného serveru SQL nelze použít server nakonfigurovaný jako řadič domény.
-   Na počítači, který bude použit jako server front-end vzdálené instalace serveru SQL, nesmí běžet Terminálový server.
-   Jako databázový software na serverovém počítači je nutné použít alespoň aplikaci Microsoft SQL Server 2005 s aktualizací Service Pack 1 (k dispozici na webu služby [Stažení softwaru](http://go.microsoft.com/fwlink/?linkid=66143) na adrese http://go.microsoft.com/fwlink/?LinkId=66143), pokud v daném počítači běží systém Windows Server 2003, a alespoň aplikaci SQL Server 2005 s aktualizací Service Pack 2, pokud v daném počítači běží systém Windows Server® 2008.
-   Klientský i serverový počítač musí být přidány do domény služby Active Directory. V opačném případě (pokud jsou v různých doménách) je nutné před spuštěním instalace služby WSUS vytvořit mezi doménami vztah důvěryhodnosti.
-   V případě, že již máte nainstalovanou službu WSUS 2.0 v konfiguraci se vzdáleným serverem SQL a chcete provést upgrade na verzi WSUS 3.0 SP1, měli byste odinstalovat službu WSUS 2.0 (pomocí příkazu **Přidat nebo odebrat programy** v Ovládacích panelech) v serverovém počítači a zároveň zajistit, aby existující databáze zůstala nezměněna. Poté byste měli nainstalovat server SQL Server 2005 s aktualizací SP1 nebo SP2 a provést upgrade existující databáze. Nakonec byste měli na klientském počítači (front-end) nainstalovat aktualizaci WSUS 3.0 SP1.

Požadavky na systém pro instalaci vzdálené konzoly aktualizace WSUS 3.0 SP1
---------------------------------------------------------------------------

Vzdálenou konzolu aktualizace WSUS 3.0 SP1 lze nainstalovat na následujících platformách:

-   Windows Server 2008
-   Windows Vista® a novější,
-   Windows Server 2003 SP1 a novější,
-   Windows XP SP2 a novější.

Požadavky na systém pro klientskou instalaci
--------------------------------------------

Automatické aktualizace je klientský software služby WSUS. Lze jej používat spolu se službou WSUS na libovolném z následujících operačních systémů:

-   Windows Vista a novější,
-   Windows Server 2008 a novější,
-   Microsoft Windows Server 2003, libovolné vydání,
-   Microsoft Windows XP Professional SP2 a novější,
-   Microsoft Windows 2000 Professional SP4, Windows 2000 Server SP4 nebo Windows 2000 Advanced Server s aktualizací SP4.

Požadavky na software pro instalaci serveru aktualizace WSUS 3.0 SP1
--------------------------------------------------------------------

Následující tabulka obsahuje přehled softwaru požadovaného pro platformy systému Windows Server 2003 SP1. Software požadovaný pro systém Windows Server 2008 bude popsán v části, která se zabývá aktualizací WSUS 3.0 SP1 v systému Windows Server 2008.

Před spuštěním instalačního programu aktualizace WSUS 3.0 SP1 se ujistěte, že server aktualizace WSUS 3.0 SP1 splňuje uvedený seznam požadavků. Pokud některá z těchto aktualizací vyžaduje po dokončení instalace restartování počítače, měli byste jej provést před instalací aktualizace WSUS 3.0 SP1.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Požadavky</th>
<th style="border:1px solid black;" >Podrobnosti</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Internetová informační služba (IIS) společnosti Microsoft</td>
<td style="border:1px solid black;">Instaluje se z operačního systému.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Microsoft .NET Framework Version 2.0 Redistributable Package</td>
<td style="border:1px solid black;">Viz balíček Microsoft .NET Framework Version 2.0 Redistributable Package (x86) na webu služby <a href="http://go.microsoft.com/fwlink/?linkid=68935">Stažení softwaru</a> (http://go.microsoft.com/fwlink/?LinkId=68935). Pro 64bitové platformy viz balíček Microsoft .NET Framework Version 2.0 Redistributable Package (x64) na webu služby <a href="http://go.microsoft.com/fwlink/?linkid=70637">Stažení softwaru</a> (http://go.microsoft.com/fwlink/?LinkId=70637).</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Konzola Microsoft Management Console 3.0 pro systém Windows Server 2003</td>
<td style="border:1px solid black;">Jedná se o nezbytný předpoklad pro použití uživatelského rozhraní aktualizace WSUS 3.0 SP1. Viz Konzola Microsoft Management Console 3.0 pro systém Windows Server 2003 (KB907265) na webu služby <a href="http://go.microsoft.com/fwlink/?linkid=70412">Stažení softwaru</a> (http://go.microsoft.com/fwlink/?LinkId=70412). Pro 64bitové platformy viz Konzola Microsoft Management Console 3.0 pro systém Windows Server 2003 x64 Edition (KB907265) na webu služby <a href="http://go.microsoft.com/fwlink/?linkid=70638">Stažení softwaru</a> (http://go.microsoft.com/fwlink/?LinkId=70638).</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Prohlížeč sestav společnosti Microsoft</td>
<td style="border:1px solid black;">Jedná se o nezbytný předpoklad pro použití uživatelského rozhraní aktualizace WSUS 3.0 SP1. Viz Microsoft Report Viewer Redistributable 2005 na webu služby <a href="http://go.microsoft.com/fwlink/?linkid=70410">Stažení softwaru</a> (http://go.microsoft.com/fwlink/?LinkId=70410).</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">SQL Server 2005 (nepovinné)</td>
<td style="border:1px solid black;">Pokud již není kompatibilní verze serveru SQL Server nainstalována, nainstaluje aktualizace WSUS 3.0 SP1 databázi služby Interní databáze systému Windows. Pokud plánujete použití úplné databáze serveru SQL Server, je nutné v systému Windows Server 2003 použít (minimálně) verzi SQL Server 2005 SP1 (k dispozici na webu služby <a href="http://go.microsoft.com/fwlink/?linkid=66143">Stažení softwaru</a> na adrese http://go.microsoft.com/fwlink/?LinkId=66143) a v systému Windows Server 2008 verzi SQL Server 2005 SP2 (k dispozici na webu služby <a href="http://go.microsoft.com/fwlink/?linkid=84823">Stažení softwaru</a> na adrese http://go.microsoft.com/fwlink/?LinkId=84823).</td>
</tr>
</tbody>
</table>
  
| ![](images/Cc708525.note(WS.10).gif)Poznámka                                                                                                                                                                                                                                                                                                                                         |  
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Pokud již máte nainstalovanou službu WSUS 2.0 používající aplikaci SQL Server 2000, SQL Server Desktop Engine 2000 nebo jinou databázi serveru SQL Server starší než SQL Server 2005 SP1 (nebo starší než SQL Server 2005 SP2, pokud je použit systém Windows Server 2008), nainstaluje instalační program aktualizace WSUS 3.0 SP1 databázi Interní databáze systému Windows® a migruje do ní použitou databázi. |
  
Požadavky na místo na disku pro instalaci serveru aktualizace WSUS 3.0 SP1  
--------------------------------------------------------------------------
  
Zde jsou uvedeny požadavky na místo na disku pro instalaci služby Windows Server Update Services:
  
-   1 GB na systémovém oddílu,  
-   2 GB na svazku, na kterém budou uloženy soubory databáze,  
-   20 GB na svazku, na kterém bude uložen obsah.
  
| ![](images/Cc708525.Important(WS.10).gif)Důležité informace                                  |  
|---------------------------------------------------------------------------------------------------------------------------|  
| Aktualizaci WSUS 3.0 SP1 nelze nainstalovat na komprimované jednotky. Ujistěte se, že zvolená jednotka není komprimovaná. |
  
Požadavky na upgrade aktualizací WSUS 3.0 SP1  
---------------------------------------------
  
#### Ujistěte se, že instalace služby WSUS běží správně, a před upgradem zálohujte databázi služby WSUS.
  
Pokud provádíte upgrade na verzi WSUS 3.0 SP1 z předchozí verze, ujistěte se, že aktuální instalace běží správně, a před upgradem zálohujte databázi služby WSUS.
  
1.  Zkontrolujte, zda se v protokolech událostí nevyskytují chyby z nedávné doby, zda nedocházelo k problémům v synchronizaci serverů přijímajících data a odesílajících data nebo k problémům s klienty, kteří se nehlásili. Než budete pokračovat, je nutné tyto problémy vyřešit.  
2.  Je vhodné spustit program DBCC CHECKDB a ujistit se tak, že databáze služby WSUS je správně indexována. Další informace o programu DBCC CHECKDB naleznete zde: [DBCC CHECKDB](http://go.microsoft.com/fwlink/?linkid=86948) (http://go.microsoft.com/fwlink/?LinkId=86948).  
3.  Zálohujte databázi služby WSUS.
  
#### Pokud jste ručně upravili port používaný službou WSUS, službu před upgradem odinstalujte.
  
Pokud upravujete port pro službu WSUS, nesnažte se jej upravit ručně a používejte vždy nástroj wsusutil. Pokud jste port upravili ručně a provedli jste upgrade ze služby Software Update Services 1.0 na verzi WSUS 2.0, postupujte následovně:
  
1.  Pokud jste dosud nenainstalovali službu WSUS 3.0, odinstalujte službu WSUS 2.0 a zachovejte databázi a obsah. (Pokud jste již nainstalovali službu WSUS 3.0, odinstalujte ji a zachovejte databázi a obsah.)  
2.  Spuštěním výchozího webu dočasně povolte službu SUS 1.0 a zpřístupněte ji tak k odinstalaci.  
3.  Odinstalujte službu SUS 1.0.  
4.  Nainstalujte službu WSUS 3.0.
  
#### Služba Software Update Services 1.0 by měla být odinstalována.
  
Pokud bude služba Software Update Services 1.0 nainstalována v počítači, instalace aktualizace WSUS 3.0 SP1 se na tomto počítači nezdaří. Před instalací aktualizace WSUS 3.0 SP1 byste měli službu Software Update Services 1.0 odinstalovat.
  
#### V 64bitovém operačním systému není upgrade ze služby WSUS 2.0 na službu WSUS 3.0 SP1 možný.
  
Služba WSUS 2.0 není v 64bitových operačních systémech podporována. V 64bitových operačních systémech není upgrade ze služby WSUS 2.0 na službu WSUS 3.0 SP1 možný.
  
Nastavení parametrů příkazového řádku  
-------------------------------------
  
Pomocí příkazového řádku lze instalační program služby WSUS spustit v režimu bezobslužné instalace a provádět bezobslužné instalace aktualizace WSUS 3.0 SP1. Následující tabulka obsahuje parametry příkazového řádku pro instalaci aktualizace WSUS 3.0 SP1.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Možnost</th>
<th style="border:1px solid black;" >Popis</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>/q</strong></td>
<td style="border:1px solid black;">Tichá instalace</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>/u</strong></td>
<td style="border:1px solid black;">Odinstalace produktu. Pokud je nainstalována databáze Interní databáze systému Windows, odinstaluje se také tato databáze.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>/p</strong></td>
<td style="border:1px solid black;">Kontrola předpokladů. Neinstaluje produkt, pouze zkontroluje systém a ohlásí případné chybějící předpoklady.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>/?, /h</strong></td>
<td style="border:1px solid black;">Zobrazení parametrů příkazového řádku a jejich popisů.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>/g</strong></td>
<td style="border:1px solid black;">Upgrade z předchozí verze služby WSUS. (Nezkoušejte provést upgrade z verze SUS 1.0.) Jediným platným parametrem této možnosti je /q (tichá instalace). Jedinou platnou vlastností této možnosti je DEFAULT_WEBSITE.</td>
</tr>
</tbody>
</table>
  
Následující tabulka obsahuje vlastnosti příkazového řádku pro aktualizaci WSUS 3.0 SP1.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Vlastnost</th>
<th style="border:1px solid black;" >Popis</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">CONTENT_LOCAL</td>
<td style="border:1px solid black;">0=obsah hostován místně, 1=obsah na serveru Microsoft Update</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">CONTENT_DIR</td>
<td style="border:1px solid black;">Cesta k adresáři obsahu. Výchozí cesta je <em>WSUSInstallationDrive</em><strong>\WSUS\WSUSContent</strong>, kde <em>WSUSInstallationDrive</em> je místní jednotka s největším množstvím volného místa.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">WYUKON_DATA_DIR</td>
<td style="border:1px solid black;">Cesta k adresáři dat databáze Interní databáze systému Windows.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">SQLINSTANCE_NAME</td>
<td style="border:1px solid black;">Název by měl být ve formátu <em>Název_serveru</em>\<em>Název_instance_SQL</em>. Pokud je instance databáze na místním počítači, použijte proměnnou prostředí %COMPUTERNAME%. Pokud se zde nevyskytuje existující instance, výchozí hodnota je %COMPUTERNAME%\WSUS.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DEFAULT_WEBSITE</td>
<td style="border:1px solid black;">0=port 8530, 1=port 80</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PREREQ_CHECK_LOG</td>
<td style="border:1px solid black;">Cesta a název souboru pro soubor protokolu</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">CONSOLE_INSTALL</td>
<td style="border:1px solid black;">0=instalovat server služby WSUS, 1=instalovat pouze konzolu</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">ENABLE_INVENTORY</td>
<td style="border:1px solid black;">0=neinstalovat funkce inventáře, 1=instalovat funkce inventáře</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DELETE_DATABASE</td>
<td style="border:1px solid black;">0=zachovat databázi, 1=odebrat databázi</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DELETE_CONTENT</td>
<td style="border:1px solid black;">0=zachovat soubory obsahu, 1=odebrat soubory obsahu</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DELETE_LOGS</td>
<td style="border:1px solid black;">0=zachovat soubory protokolu, 1=odebrat soubory protokolu (použití s přepínačem instalace /u).</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">CREATE_DATABASE</td>
<td style="border:1px solid black;">0=použít aktuální databázi, 1=vytvořit databázi</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">PROGRESS_WINDOW_HANDLE</td>
<td style="border:1px solid black;">Popisovač okna pro vracení zpráv služby MSI o průběhu instalace</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">MU_ROLLUP</td>
<td style="border:1px solid black;">1=zapojit se do programu zlepšování služby Microsoft Update, 0=nezapojit se do programu zlepšování služby Microsoft Update</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">FRONTEND_SETUP</td>
<td style="border:1px solid black;">1=nezapsat umístění obsahu do databáze, 0=zapsat umístění obsahu do databáze (pro službu NLB)</td>
</tr>
</tbody>
</table>
  
#### Příklad použití
  
```  
WSUSSetup.exe /q DEFAULT\_WEBSITE=0 (install in quiet mode using port 8530) WSUSSetup.exe /q /u (uninstall WSUS)  
```  
| ![](images/Cc708525.Important(WS.10).gif)Důležité informace                                                                                                                                    |  
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Pokud instalujete aktualizaci WSUS 3.0 SP1 v tichém režimu (/q) a v počítači nejsou nainstalovány všechny nezbytné předpoklady, vygeneruje se v průběhu instalace soubor WSUSPreReqCheck.xml a uloží se do adresáře %TEMP%. |
  
Problémy při instalaci  
----------------------
  
#### Služba IIS se v průběhu instalace aktualizace WSUS 3.0 SP1 restartuje.
  
Instalační program aktualizace WSUS 3.0 SP1 restartuje službu IIS bez předchozího upozornění, což může ovlivnit existující weby v rámci organizace. Pokud služba IIS neběží, aktualizace WSUS 3.0 SP1 ji spustí.
  
#### Pokud jsou otevřená připojení k existující databázi služby WSUS, instalace se pravděpodobně nezdaří.
  
Jestliže provádíte upgrade na verzi WSUS 3.0 SP1 z existující instalace a připojení ke stávající databázi služby WSUS jsou stále otevřená (například pokud běží program SQL Server Management Studio), instalace se pravděpodobně nezdaří. Uzavřete všechna připojení a spusťte instalaci aktualizace WSUS 3.0 SP1 znovu.
  
#### Instalační program služby WSUS zobrazuje nesprávný adresář pro soubory databáze.
  
V instalačním programu služby WSUS uvádí obrazovka **Připraveno k instalaci** nesprávnou informaci, že umístění databáze je v adresáři nadřazeném umístění databáze. Výchozí umístění je například %systemdrive%\\WSUS\\UpdateServicesDbFiles, ale uváděno je umístění %systemdrive%\\WSUS.
  
#### Pokud je služba WSUS nainstalována na počítači s jazykovými sadami vícejazyčného uživatelského rozhraní MUI a výchozí jazyk není angličtina, nápověda bude místo v angličtině zobrazena v tomto jazyce.
  
Pokud váš počítač obsahuje jazykové sady vícejazyčného uživatelského rozhraní MUI s jiným výchozím jazykem než angličtinou, bude možné službu WSUS nainstalovat i pokud je národní prostředí aktuálního uživatele anglické. Uživatelské rozhraní bude zobrazeno v angličtině, ale pro zobrazení nápovědy v angličtině je potřeba použít speciální postup. Zkopírujte soubor anglické nápovědy CHM (*WSUSInstallDir*\\documentation\\mui\\0409\\WSUS30Help.chm) do hlavního adresáře dokumentace (*WSUSInstallDir*\\documentation\\WSUS30Help.chm). Nyní by se měla nápověda zobrazovat správně ve všech jazycích.
  
Problémy s upgradem  
-------------------
  
#### Obnovení z neúspěšného upgradu
  
Pokud provádíte upgrade z předchozí verze služby WSUS (WSUS 3.0, WSUS 2.0 SP1 nebo WSUS 2.0) na verzi WSUS 3.0 SP1 a upgrade se z určitého důvodu nezdaří, postupujte následovně:
  
1.  Přeinstalujte předchozí verzi služby WSUS.  
2.  Obnovte databázi ze zálohy, kterou jste vytvořili před pokusem o upgrade. (Ve většině případů také služba WSUS automaticky vytvoří zálohu. Její umístění zjistíte v souboru WSUSSetup.log.)  
3.  Pomocí protokolů určete příčinu neúspěchu upgradu a opravte problém.  
4.  Pokuste se službu WSUS znovu upgradovat.
  
#### Upgrade z verze WSUS 2.0 na verzi WSUS 3.0 SP1 není možný, pokud stále existuje databáze služby WSUS 3.0 SP1 z předchozí instalace.
  
Pokud jste dříve nainstalovali aktualizaci WSUS 3.0 SP1 a potom znovu nainstalovali službu WSUS 2.0, je potřeba před opětovnou instalací aktualizace WSUS 3.0 SP1 odstranit z počítače databázi této verze služby.
  
#### Změna názvu počítače před upgradem na verzi WSUS 3.0 SP1 může způsobit neúspěch upgradu.
  
Pokud po instalaci služby WSUS 2.0 a před upgradem na verzi WSUS 3.0 SP1 změníte název počítače, upgrade se nemusí zdařit.
  
Pomocí následujícího skriptu odstraňte a znovu přidejte skupiny správců ASPNET a WSUS. Potom znovu spusťte upgrade.
  
Řetězec *&lt;umístění\_DB&gt;* nahraďte složkou, ve které je databáze nainstalována, a řetězec *&lt;adresář\_obsahu&gt;* nahraďte místní složkou pro ukládání.
  
```  
sqlcmd.exe -S *&lt;DBLocation&gt;* -E -Q "USE SUSDB DECLARE @asplogin varchar(200) SELECT @asplogin=name from sysusers WHERE name like '%ASPNET' EXEC sp\_revokedbaccess @asplogin" sqlcmd.exe -S *&lt;DBLocation&gt;* -E -Q "USE SUSDB DECLARE @wsusadminslogin varchar(200) SELECT @wsusadminslogin=name from sysusers WHERE name like '%WSUS Administrators' EXEC sp\_revokedbaccess @wsusadminslogin"   sqlcmd.exe -S *&lt;DBLocation&gt;* -E -Q "USE SUSDB DECLARE @asplogin varchar(200) SELECT @asplogin=HOST\_NAME()+'\\ASPNET' EXEC sp\_grantlogin @asplogin EXEC sp\_grantdbaccess @asplogin EXEC sp\_addrolemember webService,@asplogin" sqlcmd.exe -S *&lt;DBLocation&gt;* -E -Q "USE SUSDB DECLARE @wsusadminslogin varchar(200) SELECT @wsusadminslogin=HOST\_NAME()+'\\WSUS Administrators' EXEC sp\_grantlogin @wsusadminslogin EXEC sp\_grantdbaccess @wsusadminslogin EXEC sp\_addrolemember webService,@wsusadminslogin"   sqlcmd.exe -S *&lt;DBLocation&gt;* -E -Q "backup database SUSDB to disk=N'*&lt;ContentDirectory&gt;*\\SUSDB.Dat' with init"  
```
  
#### Instalační program přepíše zálohu předchozí databáze.
  
Aktualizace WSUS 3.0 SP1 přidá databázi do výchozího adresáře, což je *jednotka*\\WSUS (kde *jednotka* je místní jednotka NTFS s největším množstvím volného místa). Pokud se v tomto adresáři nachází záloha databáze, bude pravděpodobně přepsána. Před upgradem na verzi WSUS 3.0 SP1 by správci měli uložit zálohu databáze aktuální verze do jiného umístění.
  
#### Pokud jste ve službě WSUS 2.0 provedli migraci ze serveru MSDE na server SQL Server 2000 nebo SQL Server 2005, bude potřeba změnit hodnotu registru.
  
Pokud máte nainstalovanou službu WSUS 2.0 a provedli jste migraci na SQL Server 2000 nebo SQL Server 2005, bude nutné změnit hodnotu registru **HKLM\\SOFTWARE\\Microsoft\\Update Services\\Server\\Setup\\WmsdeInstalled** z 1 na 0. Pokud tak neučiníte před upgradem na verzi WSUS 3.0 SP1, upgrade se nezdaří.
  
#### Pokud je instalační program služby WSUS 2.0 spuštěn a poté zrušen, odstraní se klíč registru služby WSUS.
  
Spustíte-li instalační program WSUS 2.0 a následně jej zrušíte, klíč registru služby WSUS bude odstraněn. To může způsobit potíže, pokud již máte nainstalovanou aktualizaci WSUS 3.0 SP1. Ke stejnému problému dojde, pokud začnete odinstalovávat službu WSUS 2.0, potom tuto operaci přerušíte a následně se pokusíte provést upgrade ze služby WSUS 2.0 na verzi WSUS 3.0 SP1.
  
#### Pokud odinstalujete aktualizaci WSUS 3.0 SP1 a zachováte soubory protokolu, budou tyto soubory mít po opětovné instalaci pravděpodobně nesprávná oprávnění.
  
Při odinstalaci aktualizace WSUS 3.0 SP1 máte možnost zachovat soubory protokolu dané instalace. Pokud odinstalujete aktualizaci WSUS 3.0 SP1, staré soubory protokolu přijdou o svá oprávnění (obvykle pouze pro správce služby WSUS). Oprávnění na těchto souborech protokolu byste měli proto obnovit.
  
#### Jestliže klienti služby WSUS 2.0 mají aktualizace se stavem „Nelze použít“, bude jejich stav krátce po upgradu na verzi WSUS 3.0 SP1 „Neznámý“.
  
Pokud má server služby WSUS 2.0 klienty s aktualizacemi ve stavu **Nelze použít**, budou mít tyto aktualizace krátce po upgradu serveru na verzi WSUS 3.0 SP1 stav **Neznámý**. Stav aktualizace bude opět **Nelze použít** poté, co klient provede prohledání.
  
Známé problémy  
--------------
  
#### Řešení vícenásobných problémů se stahováním a opakovaného selhání synchronizace klienta
  
Jestliže klienti aktualizace WSUS 3.0 SP1 hlásí více chyb ve stahování, nebo pokud se klientům nedaří delší dobu synchronizace se serverem aktualizace WSUS 3.0 SP1, je pravděpodobně poškozena mezipaměť stahování. Tento stav může pomoci napravit odstranění mezipaměti stahování klienta ze systému souborů.
  
Chcete-li odstranit mezipaměť stahování klienta:
  
1.  Odstraňte všechny soubory a podadresáře v tomto umístění na klientském počítači: **%windir%\\SoftwareDistribution\\Download**  
2.  Pokuste se znovu nainstalovat aktualizaci synchronizací klientského počítače se službou WSUS 3.0 SP1. Tento pokus o instalaci by se neměl zdařit a měla by nastat následující chyba: **WU\_E\_DM\_NOTDOWNLOADED, "Aktualizace nebyla stažena."**  
3.  Po této chybě klientský počítač automaticky restartuje stahování a instalace bude moci pokračovat.
  
#### Pokud se synchronizace nezdaří, zkuste provést synchronizaci znovu.
  
Jestliže se synchronizace nezdaří, prvním krokem k vyřešení tohoto problému by mělo být zkusit server znovu synchronizovat. Pokud se nezdaří ani následná synchronizace, použijte informace o řešení potíží v příručce [Windows Server Update Services 3.0 Operations Guide](http://go.microsoft.com/fwlink/?linkid=81072) (http://go.microsoft.com/fwlink/?LinkId=81072).
  
#### Změna konfigurace aktualizace WSUS 3.0 SP1 přímo v databázi není podporována.
  
Služba Windows Server Update Services ukládá svá konfigurační data v databázi serveru SQL Server. Změna konfiguračních dat přímým přístupem do databáze však není podporována. Nepokoušejte se upravit konfiguraci aktualizace WSUS 3.0 SP1 přímým přístupem do databáze. Konfiguraci aktualizace WSUS 3.0 SP1 byste měli měnit pomocí konzoly aktualizace WSUS 3.0 SP1 nebo zavoláním rozhraní API aktualizace WSUS 3.0 SP1.
  
#### Chyby ve stahování nejsou oznamovány dostatečně rychle, pokud jsou zapnuty diskové kvóty.
  
Jsou-li zapnuty diskové kvóty a dojde k dosažení kvóty, chyby ve stahování aktualizací na serveru služby WSUS nemusí být oznámeny včas. Chcete-li se tomuto problému vyhnout, zakažte diskové kvóty nebo kvótu zvyšte.
  
#### Je-li aktualizace WSUS 3.0 SP1 nasazena pomocí protokolu SSL, může dojít k selhání klientských počítačů s kódem chyby 0x8024400a.
  
Klientské počítače mohou někdy v průběhu komunikace se serverem aktualizace WSUS 3.0 SP1 pomocí protokolu SSL selhat s kódem chyby 0x8024400a. Aktualizaci řešící tento problém naleznete zde: [KB 905422](http://go.microsoft.com/fwlink/?linkid=70593) (http://go.microsoft.com/fwlink/?LinkId=70593).
  
#### Při odinstalaci služby WSUS nedojde k odstranění účtu domény Administrators služby WSUS.
  
Skupina Administrators služby WSUS je vytvořena jako účet domény (nikoli místní účet) na řadičích domény, takže po odstranění tohoto účtu při odinstalaci služby WSUS by všechny instalace používající tento účet domény byly zakázány. Z toho důvodu služba WSUS neodstraní účet domény Administrators služby WSUS.
  
#### Jestliže je server přijímající data převeden na server odesílající data, aktualizace katalogového webu je nutné znovu importovat.
  
Pokud převedete server přijímající data na server odesílající data, je také nutné znovu importovat všechny aktualizace katalogového webu. V opačném případě se webu nezdaří synchronizace nových revizí aktualizací katalogového webu na tento server.
  
#### Používáte-li službu IIS s protokolem SSL a není zaškrtnuté políčko „Vyžadovat zabezpečený kanál“, nešifrovaný přístup je možný.
  
Jestliže instalací certifikátu nastavíte službu IIS, aby používala protokol SSL, je stále možné získat přístup k webu prostřednictvím nešifrovaného protokolu HTTP, pokud však není zaškrtnuto políčko **Vyžadovat zabezpečený kanál**. Další informace naleznete v dokumentaci pro službu [IIS](http://go.microsoft.com/fwlink/?linkid=98084) (http://go.microsoft.com/fwlink/?LinkId=98084).
  
#### Bez oprávnění čtení/zápis ke složce %windir%\\TEMP se import katalogového webu pravděpodobně nezdaří.
  
Provádíte-li import katalogového webu a účet Síťové služby nemá oprávnění čtení/zápis ke složce %windir%\\TEMP, import se pravděpodobně nezdaří s chybovou zprávou, jako je například tato: Server nemohl zpracovat požadavek. ---&gt; Soubor C:\\WINDOWS\\TEMP\\*název\_dočasného\_souboru*.dll nelze nalézt.
  
#### Během synchronizace mezi aktualizací WSUS 3.0 SP1 a serverem repliky pro příjem dat se službou WSUS 2.0 může dojít k poklesu výkonu.
  
Instalujete-li aktualizaci WSUS 3.0 SP1 na nadřazeném serveru a pokusíte se provést synchronizaci se serverem repliky pro příjem dat se službou WSUS 2.0, může dojít k problémům s výkonem. Řešení tohoto problému naleznete zde: [KB 910847](http://go.microsoft.com/fwlink/?linkid=70669) (http://go.microsoft.com/fwlink/?LinkId=70669).
  
#### Jestliže e-mailový server nepracuje nebo není dostupný, oznámení e-mailem se bez předchozího upozornění nezdaří.
  
Pokud je e-mailový server v síti v režimu offline, odesílání oznámení e-mailem aktualizací WSUS 3.0 SP1 se bez předchozího upozornění nebude dařit. Do protokolu událostí se však zapíše událost 10052 (HealthCoreEmailNotificationRed).
  
#### Změněná nastavení na nadřazeném serveru nejsou okamžitě odeslána na server pro příjem dat.
  
Dojde-li ke změně konfigurace nadřazeného serveru, může určitou dobu trvat, než se tyto změny projeví. Pokud například na nadřazeném serveru změníte nastavení, například vyberete nový jazyk a okamžitě spustíte synchronizaci na serveru pro příjem dat, změna se neprojeví. Namísto toho bude odeslána na server pro příjem dat během další plánované synchronizace. Doba čekání se prodlužuje v závislosti na počtu aktualizací na nadřazeném serveru.
  
#### Odinstalací aktualizace WSUS 3.0 SP1 se neodinstaluje instance databáze.
  
Pokud odinstalujete aktualizaci WSUS 3.0 SP1, instance databáze zůstane nainstalována. Instanci může sdílet více než jedna aplikace a její odstranění by způsobilo selhání těchto aplikací.
  
Pokud je nezbytné odinstalovat databázi Interní databáze systému Windows, použijte následující příkazy:
  
(na 32bitových platformách)
  
```  
msiexec /x {CEB5780F-1A70-44A9-850F-DE6C4F6AA8FB} callerid=ocsetup.exe  
```  
(na 64bitových platformách)
  
```  
msiexec /x {BDD79957-5801-4A2D-B09E-852E7FA64D01} callerid=ocsetup.exe  
```  
Pokud chcete odinstalovat Interní databáze systému Windows Service Pack 2 ze serveru Windows Server 2008, lze tak učinit pomocí Správce serveru.
  
Odstranění aplikace však nutně nemusí odstranit výchozí soubory MDF a LDF, což způsobí, že následná instalace aktualizace WSUS 3.0 SP1 se nezdaří. Tyto soubory lze odstranit z adresáře %windir%\\SYSMSI\\SSEE.
  
#### Jestliže server pro příjem dat změní svůj nadřazený server, aktualizace ve stavu „Neznámé“ jsou označeny jako „Nelze použít“.
  
Pokud server pro příjem dat začne synchronizovat z jiného nadřazeného serveru, budou aktualizace, které jsou ve stavu **Neznámé**, označeny na novém nadřazeném serveru jako **Nelze použít**. Tento stav je dočasný a bude opraven při příštím oznámení stavu serveru pro příjem dat poté, co s ním jeho klienti provedou synchronizaci.
  
#### Pokud vyprší časový limit Průvodce vyčištěním serveru na jednom serveru po jeho spuštění na více serverech pomocí vzdálené konzoly, připojení ke všem serverům bude ztraceno.
  
Průvodce vyčištěním serveru je možné spustit na více serverech z jedné vzdálené konzoly. Pokud však vyprší časový limit procesu čištění na jednom ze serverů, konzola ztratí připojení ke všem serverům. Žádná data nebudou ztracena. Správci však budou muset obnovit vzdálené připojení ke všem těmto serverům.
  
#### Spuštění a zastavení připojení v rychlém sledu po sobě vyvolá v Průvodci konfigurací chybovou zprávu „Nedošlo k žádné chybě synchronizace“.
  
Během konfigurace služby WSUS je potřeba připojit se k nadřazenému serveru (buď Microsoft Update nebo intranetový nadřazený server) za účelem přenosu základních informací o serveru. Pokud klepnete na tlačítko **Spustit připojování** a ihned poté klepnete na tlačítko **Zastavit připojování**, zobrazí se nesprávná chybová zpráva „Nedošlo k žádné chybě synchronizace“.
  
Aktualizace WSUS 3.0 SP1 v systému Windows Server® 2008  
-------------------------------------------------------
  
#### Podporované verze
  
Aktualizace WSUS 3.0 SP1 podporuje systém Windows Server 2008 v 32bitové i 64bitové verzi.
  
#### Předpoklady
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Požadavky</th>
<th style="border:1px solid black;" >Podrobnosti</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Internetová informační služba (IIS) společnosti Microsoft</td>
<td style="border:1px solid black;">Instaluje se z operačního systému. Ujistěte se, že jsou povoleny následující součásti:
<ul>
<li>Ověřování systému Windows,<br />
<br />
</li>
<li>Statický obsah,<br />
<br />
</li>
<li>ASP.NET,<br />
<br />
</li>
<li>Kompatibilita správy verze 6.0,<br />
<br />
</li>
<li>Kompatibilita metabáze služby IIS 6.0.<br />
<br />
</li>
</ul></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Microsoft .NET Framework Version 2.0 Redistributable Package (x86)</td>
<td style="border:1px solid black;">V systému Windows Server 2008 není nutné instalovat, je nainstalována jako součást operačního systému.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Konzola Microsoft Management Console 3.0</td>
<td style="border:1px solid black;">V systému Windows Server 2008 není nutné instalovat, je nainstalována jako součást operačního systému.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Prohlížeč sestav společnosti Microsoft</td>
<td style="border:1px solid black;">Jedná se o nezbytný předpoklad pro použití uživatelského rozhraní služby WSUS. Viz Microsoft Report Viewer Redistributable 2005 na webu služby <a href="http://go.microsoft.com/fwlink/?linkid=70410">Stažení softwaru</a> (http://go.microsoft.com/fwlink/?LinkId=70410).</td>
</tr>
</tbody>
</table>
  
#### Používání Průvodce konfigurací zabezpečení
  
V systému Windows Server 2008 můžete při spuštění Průvodce konfigurací zabezpečení vybrat roli WSUS a povolit její závislosti. Chcete-li spustit Průvodce konfigurací zabezpečení, klepněte na tlačítko **Start**, přejděte na příkaz **Nástroje pro správu** a potom klepněte na položku **Průvodce konfigurací zabezpečení**.
  
Při používání Průvodce konfigurací zabezpečení společně s rolí WSUS dochází k následujícím známým problémům:
  
-   **Služba Windows Internal Database je povolena, přestože ji služba WSUS nemusí používat.** Nakonfigurujte službu WSUS na používání databáze, a to buď databáze služby Windows Internal Database, nebo databáze serveru SQL Server. Pokud je služba WSUS nainstalována v rámci serveru SQL Server a v Průvodci konfigurací zabezpečení vyberete roli WSUS, je služba Windows Internal Database povolena, pokud je nainstalována v počítači, nepoužívá se však službou WSUS. Jestliže místo databáze služby Windows Internal Database používáte databázi SQL Server, měli byste službu Windows Internal Database zakázat.  
-   **Pravidla brány firewall pro službu WSUS na vlastním webu nejsou ve výchozím nastavení vybrána.** Pokud nainstalujete službu WSUS na vlastní web (port 8530 nebo 8531), nejsou požadovaná pravidla brány firewall automaticky vybrána, a to ani v případě, že v Průvodci konfigurací zabezpečení vyberete roli WSUS. Měli byste pro službu WSUS povolit odpovídající pravidla brány firewall, a to podle toho, zda je pro server WSUS nakonfigurováno zabezpečení SSL (Secure Sockets Layer).
  
Aktualizace WSUS 3.0 SP1 na serveru Windows Small Business Server 2003  
----------------------------------------------------------------------
  
#### Pokud je virtuální kořenový adresář služby IIS omezen na určité adresy IP nebo názvy domén, nebude se moci server aktualizace WSUS 3.0 SP1 aktualizovat.
  
Některé instalace serveru Windows Small Business Server mohou mít výchozí web služby IIS nakonfigurován na omezení **adres IP a názvů domény**. Je-li tomu tak, klient služby Windows Update na serveru se možná nebude moci aktualizovat.
  
#### Instalace aktualizace WSUS 3.0 SP1 na serveru Small Business Server – problémy s integrací
  
-   Pokud server Windows Small Business Server 2003 používá k přístupu k Internetu server proxy ISA, musí být v uživatelském rozhraní **Nastavení** zadány následující hodnoty: **nastavení serveru proxy, název serveru proxy, port**.  
-   Pokud server ISA používá ověření systému Windows, pověření serveru proxy by měla být zadána ve tvaru *DOMÉNA*\\*uživatel* a uživatel by měl být členem skupiny Internet Users.
  
#### Pokud jste do vaší sítě přidali podsíť bez použití průvodců SBS, je nutné provést tento postup.
  
Instalační program serveru služby WSUS nainstaluje na serveru dva virtuální kořenové adresáře služby IIS: SelfUpdate a ClientWebService. Instalační program také umístí některé soubory do domovského adresáře výchozího webu (na portu 80), což umožní klientským počítačům se prostřednictvím výchozího webu aktualizovat. Ve výchozím nastavení je výchozí web nakonfigurován tak, aby odmítnul přístup všem adresám IP kromě počítače localhost nebo určitých podsítí připojených k serveru. V důsledku toho se klientské počítače, které nejsou počítačem localhost ani některou z určených podsítí, nemohou samy aktualizovat. Pokud jste do vaší sítě přidali podsíť bez použití serveru Windows Small Business Server 2003, je nutné provést tento postup:
  
1.  Ve Správci serveru rozbalte nabídku **Pokročilá správa**, rozbalte nabídku **Služba Internet Information Services**, rozbalte nabídku **Weby** a následně **Výchozí web**, klepněte pravým tlačítkem myši na virtuální adresář **Selfupdate** a potom klepněte na příkaz **Vlastnosti**.  
2.  Klepněte na tlačítko **Zabezpečení adresáře**.  
3.  V části **Omezení adres IP a názvů domény** klepněte na příkaz **Upravit** a potom klepněte na položku **Udělený přístup**.  
4.  Klepněte na tlačítko **OK**, klepněte pravým tlačítkem na virtuální adresář **ClientWebService** a potom klepněte na příkaz **Vlastnosti**.  
5.  Klepněte na tlačítko **Zabezpečení adresáře**.  
6.  V části **Omezení adres IP a názvů domény** klepněte na příkaz **Upravit** a potom klepněte na položku **Udělený přístup**.
  
Autorská práva  
--------------
  
Informace obsažené v tomto dokumentu, včetně adres URL a jiných odkazů na webové servery, mohou podléhat změnám bez předchozího upozornění. Není-li uvedeno jinak, jsou společnosti, organizace, produkty, názvy domén, e-mailové adresy, loga, osoby, místa a události použité v příkladech smyšlené. Nemůže být vyvozováno žádné jejich spojení se skutečnou společností, organizací, produktem, názvem domény, emailovou adresou, logem, osobou nebo událostí. Povinností uživatele je dodržet všechny zákonné normy týkající se autorských práv. Aniž by byla omezena práva uživatele vyplývající z autorských práv, žádná část tohoto dokumentu nesmí být kopírována, uložena do veřejného systému ani rozšiřována jakýmkoli způsobem (elektronicky, mechanicky, fotokopiemi, záznamem nebo jinak) ani za žádným účelem bez výslovného písemného povolení společnosti Microsoft Corporation.
  
Společnost Microsoft může vlastnit patenty, patentové přihlášky, ochranné známky, autorská práva a další práva týkající se duševního vlastnictví, kterým podléhá předmět tohoto dokumentu. Není-li výslovně uvedeno v písemné licenční smlouvě se společností Microsoft jinak, neposkytuje tento dokument žádnou licenci na uvedené patenty, ochranné známky, autorská práva nebo jiné duševní vlastnictví.
  
© 2007 Microsoft Corporation. Všechna práva vyhrazena.
  
Microsoft, SQL Server, Windows a Windows Server jsou registrované ochranné známky nebo ochranné známky společnosti Microsoft Corporation ve Spojených státech amerických a v dalších zemích.
  
Všechny ostatní ochranné známky jsou majetkem příslušných vlastníků.
