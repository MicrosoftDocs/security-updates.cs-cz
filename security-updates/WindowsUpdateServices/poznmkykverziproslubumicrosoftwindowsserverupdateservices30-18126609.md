---
TOCTitle: 'Poznámky k verzi pro službu Microsoft Windows Server Update Services 3.0'
Title: 'Poznámky k verzi pro službu Microsoft Windows Server Update Services 3.0'
ms:assetid: '94d1385f-4872-4c29-8822-3a4ec5e45ae4'
ms:contentKeyID: 18126609
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc708491(v=WS.10)'
---

Poznámky k verzi pro službu Microsoft Windows Server Update Services 3.0
========================================================================

Tento dokument poznámek k verzi popisuje známé problémy spojené se službou Microsoft® Windows® Server Update Services (WSUS) 3.0 a obsahuje doporučení a požadavky pro instalaci této aplikace. Tyto poznámky obsahují následující části:

-   Požadavky na systém pro instalaci serveru WSUS 3.0
-   Požadavky na konfiguraci pro instalaci serveru WSUS 3.0
-   Požadavky na systém pro instalaci vzdálené konzoly WSUS 3.0
-   Požadavky na konfiguraci pro vzdálené konzoly WSUS 3.0
-   Požadavky na systém pro instalaci klienta
-   Požadavky na software pro instalaci serveru WSUS 3.0
-   Minimální požadavky na místo na disku pro instalaci serveru WSUS 3.0
-   Požadavky na upgrade služby WSUS 3.0
-   Parametry příkazového řádku instalačního programu
-   Problémy s instalací a upgradem
-   Známé problémy
-   Služba WSUS 3.0 v systému Windows Server® 2008
-   Služba WSUS 3.0 na serveru Windows Small Business Server 2003

> [!NOTE]
> Kopie tohoto dokumentu je k dispozici ke stažení na webu služby [Stažení softwaru](http://go.microsoft.com/fwlink/?linkid=71220) ([http://go.microsoft.com/fwlink/?LinkId=71220](http://go.microsoft.com/fwlink/?linkid=71220)). 

Důležité problémy týkající se konfigurace: Je třeba přepsat heslo proxy serveru v průvodci konfigurací.
-------------------------------------------------------------------------------------------------------

Jestliže používáte proxy server vyžadující ověřování uživatelského jména a hesla, je možné, že se serveru WSUS nepodaří synchronizovat aktualizace, pokud nepřepíšete heslo proxy serveru při spuštění Průvodce konfigurací serveru WSUS. Vzhledem k tomu, že je průvodce konfigurací spuštěn automaticky po skončení instalace, může tento problém způsobit chyby synchronizace po upgradu na službu WSUS 3.0 ze starší verze služby WSUS.

Tomuto problému se můžete vyhnout zrušením průvodce konfigurací po upgradu nebo zadáním správného hesla proxy serveru při spuštění průvodce konfigurací. Pokud již k těmto potížím došlo, můžete je odstranit tak, že přejdete na stránce **Možnosti** na položku **zdroje aktualizací a nastavení proxy serveru**, zadáte znovu heslo proxy serveru a potom nastavení uložíte.

Požadavky na systém pro instalaci serveru WSUS 3.0
--------------------------------------------------

#### Server WSUS 3.0 je podporován v systému Windows Server 2003 Service Pack 1 a Windows Server 2008.

Server WSUS 3.0 je podporován v systému Windows Server 2003 Service Pack 1 a Windows Server 2008.

#### Systém Windows 2000 Server není podporován u serverů služby WSUS 3.0

Servery služby WSUS 3.0 nepodporují operační systém Microsoft Windows® 2000 Server.

#### Služba WSUS 3.0 není podporována na serverech s Terminálovou službou.

Přestože služba WSUS 3.0 může běžet na serverech, na kterých je spuštěna Terminálová služba, není tento postup doporučován ani podporován. Služba WSUS 3.0 nebude běžet na serveru, na kterém je spuštěna Terminálová služba, v konfiguracích využívajících vzdálené implementace serveru SQL Server. Protože budou všechny vzdálené vlastní akce (včetně instalace) spuštěny na licencovaném serveru Terminálové služby v roli systémového účtu a protože tento systémový účet serveru nemusí mít oprávnění ke vzdálenému serveru SQL Server, nemusí se instalace zdařit.

Požadavky na konfiguraci pro instalaci serveru WSUS 3.0
-------------------------------------------------------

#### Musí být nainstalovaná Internetová informační služba.

Služba WSUS 3.0 vyžaduje Internetovou informační službu (IIS), která není ve výchozím nastavení v systému Microsoft Windows Server 2003 nebo Windows Server 2008 nainstalovaná. Pokud se pokusíte nainstalovat službu WSUS 3.0 bez Internetové informační služby, zobrazí instalační program služby WSUS chybovou zprávu, že Internetová informační služba není nainstalována.

#### Pokud je Internetová informační služba (IIS) spuštěna v izolovaném režimu služby IIS 5.0, instalace se nezdaří.

Jestliže jste upgradovali server ze systému Windows 2000 Server na systém Windows Server 2003, je možné, že bude služba IIS běžet v režimu kompatibility se serverem IIS 5.0. Je také možné povolit režim izolace služby IIS 5.0 ve Správci služby IIS. Instalace se tak nezdaří. Před instalací služby WSUS 3.0 bude potřeba zakázat režim izolace služby IIS 5.0.

#### Pokud je jakákoli součást Internetové informační služby nainstalovaná na 64bitové platformě v režimu kompatibility s 32bitovými aplikacemi, instalace služby WSUS 3.0 se nemusí zdařit.

Všechny součásti Internetové informační služby by měly být na 64bitových platformách nainstalované v nativním režimu. Instalace se nemusí zdařit, pokud jakákoli součást Internetové informační služby pracuje v režimu kompatibility s 32bitovými aplikacemi.

#### Proxy servery musí podporovat protokoly HTTP i HTTPS

Když konfigurujete kořenový server WSUS (to je server WSUS, který získává aktualizace přímo z webu Microsoft Update) a mezi serverem WSUS a Internetem bude proxy server, musí tento proxy server podporovat protokoly HTTP i HTTPS.

#### Jestliže na portu 80 již běží dva nebo více webů, odstraňte před instalací služby WSUS všechny tyto weby kromě jednoho.

Pokud na portu 80 běží dva nebo více webů (například služba Windows® SharePoint® Services), měli byste před instalací služby WSUS odstranit všechny weby kromě jednoho z nich. Pokud tak neučiníte, automatická aktualizace klientů vašeho serveru se pravděpodobně nezdaří.

#### Při instalaci služby WSUS 3.0 bude možná nutné zakázat antivirové programy.

Před provedením úspěšné instalace služby WSUS 3.0 bude možná nutné zakázat antivirové programy. Jakmile zakážete antivirový program, restartujte počítač. Teprve potom spusťte instalaci služby WSUS. Restartováním počítače předejdete zamčení souborů, ke kterým instalační proces bude potřebovat přístup. Po dokončení instalace znovu povolte antivirový program. Přesné kroky k zakázání a opětovnému povolení antivirového programu naleznete na webu poskytovatele antivirového programu.

| ![](images/Cc708491.Caution(WS.10).gif)Upozornění                                                                                                                                                                                                                                                                           |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Toto řešení může způsobit, že bude počítač nebo síť náchylnější k útokům ze strany uživatele se zlými úmysly nebo škodlivého softwaru, jako jsou například viry. Společnost Microsoft toto řešení nedoporučuje, ale poskytuje tuto informaci, aby mohlo být toto řešení použito podle vlastního uvážení. Používejte toto řešení pouze na vlastní riziko. |

> [!NOTE]
> Antivirový program je navržen k ochraně počítače před viry. Pokud je antivirový program zakázaný, nesmějí být stahovány ani otvírány soubory pocházející ze zdrojů, kterým nedůvěřujete, nesmí být navštěvovány weby, kterým nedůvěřujete, a ani otevírány přílohy e-mailu. 

#### Služba WSUS 3.0 vyžaduje, aby na serveru SQL Server byla zapnutá možnost vnořených aktivačních událostí.

Možnost vnořených aktivačních událostí je ve výchozím nastavení zapnutá. Správce serveru SQL Server ji však může vypnout.

Jestliže máte v plánu používat databázi serveru SQL Server jako datové úložiště služby Windows Server Update Services, měl by správce serveru SQL Server ověřit, že je možnost vnořených aktivačních událostí na serveru zapnutá, a to ještě před tím, než správce služby WSUS 3.0 nainstaluje službu WSUS 3.0 a zadá při instalaci tuto databázi.

Instalační program pro službu WSUS 3.0 zapne možnost RECURSIVE\_TRIGGERS, která je specifická pro databázi. Nezapne však možnost vnořených aktivačních událostí, což je globální možnost serveru.

Chcete-li zjistit, zda je možnost vnořených aktivačních událostí zapnutá, použijte následující příkaz:

**sp\_configure 'nested triggers'**

Chcete-li zapnout možnost aktivačních událostí na serveru SQL Server, spusťte z dávkového souboru v počítači se serverem SQL Server následující příkaz:

**sp\_configure 'nested triggers', 1**

**GO**

**RECONFIGURE**

**GO**

Pokud není na serveru nainstalovaná aplikace SQL Server Management Studio, bude možná vhodné spustit skripty SQL na příkazovém řádku. Nástroj Microsoft SQL Server 2005 Command Line Query Utility můžete získat na webu služby [Stažení softwaru](http://go.microsoft.com/fwlink/?linkid=70728) (http://go.microsoft.com/fwlink/?LinkId=70728). Spustíte jej příkazem **sqlcmd**.

Pokud chcete spouštět skripty SQL proti databázi Interní databáze systému Windows, je třeba také stáhnout nativního klienta SQL ze stejné stránky.

#### Omezení a požadavky na vzdálený SQL Server

Služba WSUS 3.0 obsahuje podporu pro spouštění databázového softwaru v jiném počítači, než ve kterém běží zbývající části aplikace služby WSUS 3.0. Chcete-li nakonfigurovat instalaci vzdáleného serveru SQL, je potřeba splnit určité požadavky.

-   Server nakonfigurovaný jako řadič domény nelze použít jako počítač back-end vzdálené dvojice SQL.
-   V počítači, který bude použit jako server front-end vzdálené instalace serveru SQL, nesmí běžet Terminálový server.
-   Jako databázový software na serverovém počítači je nutné použít alespoň aplikaci Microsoft SQL Server 2005 s aktualizací Service Pack 1 (k dispozici na webu služby [Stažení softwaru](http://go.microsoft.com/fwlink/?linkid=66143) na adrese http://go.microsoft.com/fwlink/?LinkId=66143), pokud v daném počítači běží systém Windows Server 2003, a alespoň aplikaci SQL Server 2005 s aktualizací Service Pack 2, pokud v daném počítači běží systém Windows Server® 2008.
-   Klientský i serverový počítač musí být přidány do domény služby Active Directory. V opačném případě (pokud jsou v různých doménách) je nutné před spuštěním instalace služby WSUS vytvořit mezi doménami vztah důvěryhodnosti.
-   Pokud je služba WSUS 2.0 již nainstalována ve vzdálené konfiguraci SQL a chcete ji upgradovat na verzi 3.0, měli byste službu WSUS 2.0 odinstalovat (pomocí panelu **Přidat nebo odebrat programy** v Ovládacích panelech) v počítači back-end a přitom zajistit, aby zůstala zachována existující databáze. Pak nainstalujete aktualizaci SQL Server 2005 SP1 nebo SP2 a upgradujte existující databázi. Nakonec byste měli do klientského počítače (front-end) nainstalovat službu WSUS 3.0.

#### Službu WSUS nelze nainstalovat, pokud jsou již nainstalované určité předběžné verze aplikace Internet Explorer 7 s Terminálovou službou.

Instalace služby WSUS se nezdaří, pokud jsou v počítači určité verze RC aplikace Internet Explorer 7 spolu s Terminálovou službou.

Požadavky na systém pro instalaci vzdálené konzoly WSUS 3.0
-----------------------------------------------------------

Vzdálenou konzolu WSUS 3.0 lze nainstalovat na následujících platformách:

-   Windows Server 2008
-   Windows Vista®
-   Windows Server 2003 SP1
-   Windows XP SP2

Požadavky na konfiguraci pro vzdálené konzoly WSUS 3.0
------------------------------------------------------

#### Mezi konzolou pro vzdálenou správu a serverem WSUS 3.0 je nutné používat širokopásmové připojení.

Pokud se připojíte k serveru WSUS 3.0 pomocí konzoly pro vzdálenou správu prostřednictvím připojení WAN s nízkou šířkou pásma, můžete zaznamenat potíže s výkonem. Vyfiltrováním aktualizací a počítačů můžete omezit jejich počet, přesto však doporučujeme mezi konzolou pro vzdálenou správu a servery WSUS 3.0 používat širokopásmové připojení. V případě potíží s výkonem u vzdálené konzoly doporučujeme připojení k serveru pomocí terminálového serveru pro vzdálenou správu.

Požadavky na systém pro instalaci klienta
-----------------------------------------

Automatické aktualizace jsou software klienta služby WSUS. Lze jej používat spolu se službou WSUS v kterémkoli z těchto operačních systémů:

-   Windows Vista
-   Windows Server 2008
-   Microsoft Windows Server 2003, libovolné vydání
-   Microsoft Windows XP Professional SP2
-   Microsoft Windows 2000 Professional SP4, Windows 2000 Server SP4 nebo Windows 2000 Advanced Server s aktualizací SP4

Požadavky na software pro instalaci serveru WSUS 3.0
----------------------------------------------------

Následující tabulka uvádí požadovaný software pro platformy založené na systému Windows Server 2003 SP 1. Požadovaný software pro systém Windows Server 2008 je diskutován v sekci věnované službě WSUS 3.0 v systému Windows Server 2008.

Je nutné, aby server WSUS 3.0 splňoval požadavky uvedené v tomto seznamu dříve, než spustíte instalační program pro službu WSUS 3.0. Pokud některé z těchto aktualizací vyžadují restartování počítače po dokončení instalace, měli byste jej restartovat před instalací služby WSUS 3.0.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Požadavek</th>
<th style="border:1px solid black;" >Podrobnosti</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Internetová informační služba (IIS)</td>
<td style="border:1px solid black;">Instalujte z operačního systému.
Viz problém 1: Musí být nainstalovaná Internetová informační služba.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Balíček Microsoft .NET Framework verze 2.0 Redistributable Package (x86)</td>
<td style="border:1px solid black;">Viz Balíček Microsoft .NET Framework verze 2.0 Redistributable Package (x86) na webu služby <a href="http://go.microsoft.com/fwlink/?linkid=68935">Stažení softwaru</a> (http://go.microsoft.com/fwlink/?LinkId=68935). V případě 64bitové platformy viz Balíček Microsoft .NET Framework verze 2.0 Redistributable Package (x64) na webu služby <a href="http://go.microsoft.com/fwlink/?linkid=70637">Stažení softwaru</a> (http://go.microsoft.com/fwlink/?LinkId=70637)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Konzola Microsoft Management Console 3.0 pro systém Windows Server 2003</td>
<td style="border:1px solid black;">Tato součást je nutná k používání uživatelského rozhraní služby WSUS 3.0. Viz Konzola Microsoft Management Console 3.0 pro systém Windows Server 2003 (KB907265) na webu služby <a href="http://go.microsoft.com/fwlink/?linkid=70412">Stažení softwaru</a> (http://go.microsoft.com/fwlink/?LinkId=70412). V případě 64bitové platformy viz Konzola Microsoft Management Console 3.0 pro systém Windows Server 2003 x64 Edition (KB907265) na webu služby <a href="http://go.microsoft.com/fwlink/?linkid=70638">Stažení softwaru</a> (http://go.microsoft.com/fwlink/?LinkId=70638).</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Prohlížeč Microsoft Report Viewer</td>
<td style="border:1px solid black;">Tato součást je nutná k používání uživatelského rozhraní služby WSUS 3.0. Viz Microsoft Report Viewer Redistributable 2005 na webu služby <a href="http://go.microsoft.com/fwlink/?linkid=70410">Stažení softwaru</a> (http://go.microsoft.com/fwlink/?LinkId=70410).</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">SQL Server 2005 (nepovinné)</td>
<td style="border:1px solid black;">Pokud ještě není kompatibilní verze serveru SQL Server nainstalována, nainstaluje aktualizace WSUS 3.0 databázi služby Interní databáze systému Windows. Pokud plánujete použití úplné databáze serveru SQL Server, je nutné v systému Windows Server 2003 použít (minimálně) verzi SQL Server 2005 SP1 (dostupná ve službě <a href="http://go.microsoft.com/fwlink/?linkid=66143">Stažení softwaru</a> na adrese http://go.microsoft.com/fwlink/?LinkId=66143) a v systému Windows Server 2008 verzi SQL Server 2005 SP2 (dostupná ve službě <a href="http://go.microsoft.com/fwlink/?linkid=84823">Stažení softwaru</a> na adrese http://go.microsoft.com/fwlink/?LinkId=84823).</td>
</tr>
</tbody>
</table>
  
| ![](images/Cc708491.note(WS.10).gif)Poznámka                                                                                                                                                                                                                                                                                                                             |  
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Pokud již byla dříve nainstalována služba WSUS 2.0 a používá databázi serveru SQL Server 2000, SQL Server Desktop Engine 2000 nebo jakoukoli databázi serveru SQL Server před verzí SQL Server 2005 SP1 (nebo SQL Server 2005 SP2 v systému Windows Server 2008), nainstaluje instalační program služby WSUS 3.0 software Interní databáze systému Windows® a provede migraci databáze na tuto verzi. |
  
Požadavky na místo na disku pro instalaci serveru WSUS 3.0  
----------------------------------------------------------
  
K instalaci služby Windows Server Update Services musejí být splněny tyto minimální požadavky na místo na disku:
  
-   1 GB na systémovém oddílu,  
-   2 GB na svazku, kde budou uloženy databázové soubory,  
-   20 GB na svazku, na který bude ukládán obsah.
  
| ![](images/Cc708491.Important(WS.10).gif)Důležité informace                           |  
|--------------------------------------------------------------------------------------------------------------------|  
| Službu WSUS 3.0 nelze nainstalovat na komprimované jednotky. Zkontrolujte, zda vybraná jednotka není komprimovaná. |
  
Požadavky na upgrade služby WSUS 3.0  
------------------------------------
  
#### Ujistěte se, že instalace služby WSUS běží správně, a před upgradem zálohujte databázi služby WSUS.
  
Pokud provádíte upgrade na verzi WSUS 3.0 z předchozí verze, ujistěte se, že aktuální instalace běží správně, a před upgradem zálohujte databázi služby WSUS.
  
1.  Zkontrolujte, zda se v protokolech událostí nevyskytují chyby z nedávné doby, zda nedocházelo k problémům v synchronizaci serverů přijímajících data a odesílajících data nebo k problémům s klienty, kteří se nehlásili. Než budete pokračovat, je nutné tyto problémy vyřešit.  
2.  Je vhodné spustit program DBCC CHECKDB a ujistit se tak, že databáze služby WSUS je správně indexována. Další informace o programu DBCC CHECKDB naleznete zde: [DBCC CHECKDB](http://go.microsoft.com/fwlink/?linkid=86948) (http://go.microsoft.com/fwlink/?LinkId=86948) (stránka může být v angličtině)  
3.  Zálohujte databázi služby WSUS.
  
#### Služba Software Update Services 1.0 by měla být odinstalována.
  
Instalace služby WSUS 3.0 se nezdaří, pokud je ve stejném počítači nainstalovaná služba Software Update Services 1.0. Před instalací služby WSUS 3.0 je nutné odinstalovat službu Software Update Services 1.0.
  
#### Není podporován upgrade z verze beta služby WSUS 3.0 na verzi RTM služby WSUS 3.0. Je však možný upgrade z verze RC na verzi RTM.
  
Pokud máte nainstalovanou verzi beta služby WSUS 3.0, bude nutné ji odinstalovat a odstranit její databázi. Až potom můžete nainstalovat novější verzi služby WSUS 3.0. Upgrade je možný pouze z verze RC na verzi RTM.
  
#### Není možné upgradovat službu WSUS 2.0 na WSUS 3.0 v 64bitovém operačním systému.
  
Služba WSUS 2.0 není podporována v 64bitových operačních systémech. Není možné upgradovat službu WSUS 2.0 na WSUS 3.0 v 64bitových systémech.
  
Parametry příkazového řádku instalačního programu  
-------------------------------------------------
  
Pomocí parametrů příkazového řádku služby WSUS lze provést bezobslužnou instalaci služby WSUS 3.0. Následující tabulka uvádí parametry příkazového řádku pro službu WSUS 3.0.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Parametr</th>
<th style="border:1px solid black;" >Popis</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>/q</strong></td>
<td style="border:1px solid black;">Provede tichou instalaci.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>/u</strong></td>
<td style="border:1px solid black;">Odinstaluje daný produkt. Pokud je nainstalována instance Interní databáze systému Windows, bude také odinstalována.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>/p</strong></td>
<td style="border:1px solid black;">Provede pouze kontrolu nezbytných předpokladů. Neinstaluje produkt, pouze zkontroluje systém a ohlásí případné chybějící předpoklady.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>/?, /h</strong></td>
<td style="border:1px solid black;">Zobrazení parametrů příkazového řádku a jejich popisů.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>/g</strong></td>
<td style="border:1px solid black;">Upgrade z verze 2.0 služby WSUS. Jediným platným parametrem této možnosti je /q (tichá instalace). Jedinou platnou vlastností této možnosti je DEFAULT_WEBSITE.</td>
</tr>
</tbody>
</table>
  
Následující tabulka uvádí vlastnosti příkazového řádku pro službu WSUS 3.0.
  
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
<td style="border:1px solid black;">0 = obsah hostován místně, 1 = obsah na serveru Microsoft Update</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">CONTENT_DIR</td>
<td style="border:1px solid black;">Cesta k adresáři s obsahem. Výchozí cesta je <em>WSUSInstallationDrive</em><strong>\WSUS\WSUSContent</strong>, kde <em>WSUSInstallationDrive</em> je místní jednotka s největším množstvím volného místa.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">WYUKON_DATA_DIR</td>
<td style="border:1px solid black;">Cesta k adresáři dat databáze Interní databáze systému Windows.</td>
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
<td style="border:1px solid black;">0=instalovat server služby WSUS, 1=instalovat pouze konzolu</td>
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
<td style="border:1px solid black;">0=zachovat soubory protokolu, 1=odebrat soubory protokolu (použití s přepínačem instalace /u).</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">CREATE_DATABASE</td>
<td style="border:1px solid black;">0 = použít aktuální databázi, 1 = vytvořit databázi</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">PROGRESS_WINDOW_HANDLE</td>
<td style="border:1px solid black;">Popisovač okna vracející zprávy instalační služby MSI o průběhu</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">MU_ROLLUP</td>
<td style="border:1px solid black;">1 = zapojit se do programu zlepšování služby Microsoft Update, 0 = nezapojovat se</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">FRONTEND_SETUP</td>
<td style="border:1px solid black;">1=nezapisovat umístění obsahu do databáze, 0=zapisovat umístění obsahu do databáze (pro službu Vyrovnávání zatížení sítě)</td>
</tr>
</tbody>
</table>
  
#### Příklad použití
  
```  
WSUSSetup.exe /q DEFAULT_WEBSITE=0  (install in quiet mode using port 8530)
WSUSSetup.exe /q /u (uninstall WSUS)
```  
| ![](images/Cc708491.Important(WS.10).gif)Důležité informace                                                                                                         |  
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Pokud je instalace služby WSUS 3.0 provedena v tichém režimu (/q) a počítač nesplňuje všechny nezbytné předpoklady, instalace vytvoří soubor WSUSPreReqCheck.xml a uloží jej do adresáře %TEMP%. |
  
Problémy při instalaci  
----------------------
  
#### Internetová informační služba bude při instalaci služby WSUS 3.0 restartována.
  
Instalační program pro službu WSUS 3.0 bez upozornění restartuje Internetovou informační službu, což by mohlo mít vliv na současné weby v rámci organizace. Pokud Internetová informační služba neběží, instalační program služby WSUS 3.0 ji spustí.
  
#### Pokud existují otevřená připojení k současné databázi služby WSUS, instalace se nemusí zdařit.
  
Pokud je prováděn upgrade z existující verze služby WSUS na verzi 3.0 a k databázi WSUS existují otevřená připojení (například je spuštěná aplikace SQL Server Management Studio), instalace se nemusí zdařit. Zavřete všechna připojení a znovu spusťte instalaci služby WSUS 3.0.
  
#### Instalační program služby WSUS ukazuje nesprávný adresář pro soubory databáze.
  
V instalačním programu služby WSUS obrazovka **Instalace je připravená** nesprávně uvádí umístění databáze jako nadřazený adresář umístění databáze. Příklad: výchozí umístění je %systemdrive%\\WSUS\\UpdateServicesDbFiles, ale během instalace se zobrazí nesprávné umístění %systemdrive%\\WSUS.
  
#### Pokud je služba WSUS nainstalována v počítači s jazykovými sadami vícejazyčného uživatelského rozhraní MUI a výchozí jazyk není angličtina, nápověda bude místo v angličtině zobrazena v tomto jazyce.
  
Pokud váš počítač obsahuje jazykové sady vícejazyčného uživatelského rozhraní MUI s jiným výchozím jazykem než angličtinou, bude možné službu WSUS nainstalovat, i pokud je národní prostředí aktuálního uživatele anglické. Uživatelské rozhraní bude zobrazeno v angličtině, ale pro zobrazení nápovědy v angličtině je potřeba použít speciální postup. Zkopírujte soubor anglické nápovědy CHM (*WSUSInstallDir*\\documentation\\mui\\0409\\WSUS30Help.chm) do hlavního adresáře dokumentace (*WSUSInstallDir*\\documentation\\WSUS30Help.chm). Nyní by se měla nápověda zobrazovat správně ve všech jazycích.
  
Problémy s upgradem  
-------------------
  
#### Upgrade ze služby WSUS 3.0 RC na službu WSUS 3.0 RTM způsobí, že certifikát SSL nebude přiřazen k webu služby WSUS.
  
Web služby WSUS je během upgradu ze služby WSUS 3.0 RC na službu WSUS 3.0 RTM odstraněn a potom znovu vytvořen. V důsledku toho již certifikát SSL nebude přiřazen webu WSUS. Po upgradu bude nutné certifikát znovu přiřadit.
  
#### Obnovení v případě neúspěšného upgradu
  
Pokud se upgrade služby WSUS z verze 2.0 na verzi 3.0 z jakéhokoli důvodu nezdaří, bude nutné znovu nainstalovat službu WSUS 2.0 a obnovit ze zálohy její databázi.
  
#### Nelze provést upgrade služby WSUS z verze 2.0 na verzi 3.0, pokud existuje databáze WSUS verze 3.0 z předchozí instalace.
  
Pokud již byla nainstalována služba WSUS 3.0 a poté byla znovu nainstalována služba WSUS 2.0, je nutné z počítače odstranit databázi služby WSUS 3.0 před pokusem o opětovnou instalaci služby WSUS 3.0.
  
#### Změna názvu počítače provedená před upgradem na službu WSUS 3.0 může způsobit selhání tohoto upgradu.
  
Pokud změníte název počítače po instalaci služby WSUS 2.0 a před provedením upgradu na službu WSUS 3.0, nemusí se tento upgrade zdařit.
  
Pomocí následujícího skriptu odeberte a znovu přidejte skupiny ASPNET a WSUS Administrators. Poté spusťte upgrade znovu.
  
Bude třeba nahradit řetězec *&lt;DBLocation&gt;* názvem složky, ve které je nainstalovaná databáze, a řetězec *&lt;ContentDirectory&gt;* složkou místního úložiště.
  
```  
sqlcmd.exe -S <DBLocation> -E -Q "USE SUSDB DECLARE @asplogin varchar(200) SELECT @asplogin=name from sysusers WHERE name like '%ASPNET' EXEC sp_revokedbaccess @asplogin"
sqlcmd.exe -S <DBLocation> -E -Q "USE SUSDB DECLARE @wsusadminslogin varchar(200) SELECT @wsusadminslogin=name from sysusers WHERE name like '%WSUS Administrators' EXEC sp_revokedbaccess @wsusadminslogin"
 
sqlcmd.exe -S <DBLocation> -E -Q "USE SUSDB DECLARE @asplogin varchar(200) SELECT @asplogin=HOST_NAME()+'\ASPNET' EXEC sp_grantlogin @asplogin EXEC sp_grantdbaccess @asplogin EXEC sp_addrolemember webService,@asplogin"
sqlcmd.exe -S <DBLocation> -E -Q "USE SUSDB DECLARE @wsusadminslogin varchar(200) SELECT @wsusadminslogin=HOST_NAME()+'\WSUS Administrators' EXEC sp_grantlogin @wsusadminslogin EXEC sp_grantdbaccess @wsusadminslogin EXEC sp_addrolemember webService,@wsusadminslogin"
 
sqlcmd.exe -S <DBLocation> -E -Q "backup database SUSDB to disk=N'<ContentDirectory>\SUSDB.Dat' with init"
```
  
#### Instalační program může přepsat zálohu předchozí databáze.
  
Instalační program služby WSUS 3.0 přidá databázi do adresáře určeného během instalace. Ve výchozím nastavení je to adresář *%systemdrive%*\\WSUS\\UpdateServicesDbFiles. Pokud se v tomto adresáři nachází záloha předchozí databáze, bude přepsána novou databází. Správci by měli zazálohovat soubory databáze před instalací aktualizací do počítače, ve kterém je daná databáze umístěná.
  
#### Pokud jste ve službě WSUS 2.0 provedli migraci ze serveru MSDE na server SQL Server 2000 nebo SQL Server 2005, bude potřeba změnit hodnotu registru.
  
Pokud máte nainstalovanou službu WSUS 2.0 a provedli jste migraci na SQL Server 2000 nebo SQL Server 2005, bude nutné změnit hodnotu registru **HKLM\\SOFTWARE\\Microsoft\\Update Services\\Server\\Setup\\WmsdeInstalled** z 1 na 0. Pokud tak neučiníte před upgradem na verzi WSUS 3.0, upgrade se nezdaří.
  
#### Je-li spuštěn instalační program služby WSUS 2.0 a následně je instalace zrušena, dojde k odstranění klíče registru pro službu WSUS.
  
Spustíte-li instalační program služby WSUS 2.0 a poté zrušíte instalaci, dojde k odstranění klíče registru pro službu WSUS. To může způsobit problémy v případě, že již máte nainstalovanou službu WSUS 3.0. Stejný problém nastane, pokud spustíte odinstalaci služby WSUS 2.0 a potom operaci zrušíte a následně se pokusíte provést upgrade z veze WSUS 2.0 na WSUS 3.0.
  
#### Pokud odinstalujete službu WSUS 3.0 a ponecháte soubory protokolu, nemusí mít tyto soubory po opětovné instalaci služby správná oprávnění.
  
Během odinstalace služby WSUS 3.0 máte možnost ponechat soubory protokolu o instalaci. Když znovu nainstalujete službu WSUS 3.0, ztratí původní soubory protokolu svá oprávnění (většinou pouze pro skupinu WSUS Administrators). Měli byste obnovit oprávnění těchto souborů protokolu.
  
#### Pokud po instalaci služby WSUS 3.0 RC byla nainstalována služba Windows SharePoint Services, při upgradu na verzi WSUS 3.0 RTM je nutné zvláštním postupem obejít jeden problém.
  
Pokud jste nainstalovali službu WSUS 3.0 RC a potom jste do stejného počítače nainstalovali službu Windows SharePoint Services, můžete upgradovat na službu WSUS 3.0 RTM jen za předpokladu, že zvolíte instalaci na vlastní port (port 8530). Chcete-li tuto instalaci provést z příkazového řádku, otevřete prostředí příkazového řádku a zadejte následující příkaz: **WSUSSetup /q / g/ DEFAULT\_WEBSITE=0**. (Chcete-li provést tuto instalaci s použitím uživatelského rozhraní, zadejte **WSUSSetup /g DEFAULT\_WEBSITE=0**.)
  
Pokud je služba WSUS nainstalována v počítači s jazykovými sadami vícejazyčného uživatelského rozhraní MUI, nápověda bude místo ve výchozím jazyce zobrazena v aktuálním jazyce uživatele.
  
#### Jestliže klienti služby WSUS 2.0 mají aktualizace se stavem Nelze použít, bude jejich stav krátce po upgradu na verzi WSUS 3.0 Neznámý.
  
Pokud má server služby WSUS 2.0 klienty s aktualizacemi ve stavu Nelze použít, budou mít tyto aktualizace krátce po upgradu serveru na verzi WSUS 3.0 stav Neznámý. Stav aktualizace bude opět Nelze použít poté, co klient provede prohledání.
  
Známé problémy  
--------------
  
#### Řešení potíží s četnými chybami stahování nebo opakovanými selháními synchronizace klienta
  
Pokud klienti služby WSUS 3.0 hlásí četné chyby stahování nebo pokud se klientům nedaří synchronizovat se serverem WSUS 3.0 po delší časové období, může být poškozená mezipaměť klienta pro stahování. Tento stav lze vyřešit odstraněním mezipaměti klienta pro stahování ze systému souborů.
  
Postup odstranění mezipaměti klienta pro stahování:
  
1.  Odstraňte všechny soubory a podadresáře z tohoto umístění v klientském počítači. **%windir%\\SoftwareDistribution\\Download**  
2.  Zkuste nainstalovat aktualizace opětovnou synchronizací klientského počítače se službou WSUS 3.0. Pokus o instalaci by se neměl zdařit a měla by se zobrazit tato chyba: **WU\_E\_DM\_NOTDOWNLOADED, Aktualizace nebyla stažena.**  
3.  Po tomto selhání klientský počítač automaticky znovu spustí stahování a instalace bude moci pokračovat.
  
#### Pokud se synchronizace nezdaří, opakujte ji.
  
Pokud se synchronizace nezdaří, měli byste nejdříve zkusit novou synchronizaci se serverem. Pokud se i následující synchronizace nezdaří, postupujte podle informací o řešení potíží v [provozní příručce služby WSUS 3.0](http://go.microsoft.com/fwlink/?linkid=81072) (http://go.microsoft.com/fwlink/?LinkId=81072, tato stránka může být v angličtině).
  
#### Změna konfigurace služby WSUS 3.0 přímo v databázi není podporována.
  
Služba Windows Server Update Services ukládá svá konfigurační data do databáze serveru SQL Server. Změna konfiguračních dat přímo v databázi však není podporována. Nepokoušejte se měnit konfiguraci služby WSUS 3.0 přímo v databázi. Konfigurace služby WSUS 3.0 by měla být prováděna pomocí konzoly služby WSUS 3.0 nebo pomocí funkcí rozhraní API této služby.
  
#### Selhání stahování nejsou hlášena ihned, pokud jsou zapnuté diskové kvóty.
  
Pokud jsou zapnuté diskové kvóty a kvóta je dosažena, selhání stahování aktualizací na serveru WSUS nemusí být včas ohlášeno. Tomuto problému se lze vyhnout zakázáním diskových kvót nebo jejich zvýšením.
  
#### Pokud je služba WSUS 3.0 nasazena pomocí protokolu SSL, může se v klientských počítačích zobrazit chybový kód 0x8024400a.
  
V klientských počítačích se někdy může zobrazit chybový kód 0x8024400a během komunikace se serverem WSUS 3.0 pomocí protokolu SSL. Aktualizaci s řešením tohoto problému naleznete v článku [KB 905422](http://go.microsoft.com/fwlink/?linkid=70593) (http://go.microsoft.com/fwlink/?LinkId=70593, tato stránka může být v angličtině).
  
#### Doménový účet správců služby WSUS nebude při odinstalaci služby WSUS odstraněn.
  
Skupina WSUS Administrators je v řadičích domény vytvořena ve formě doménového účtu (nikoli místního účtu), a tak všechny instalace, které používají tento doménový účet, by byly zakázány, pokud by byl účet při odinstalaci služby WSUS odstraněn. Odinstalace služby WSUS proto neodstraní doménový účet WSUS Administrators.
  
#### Pokud je server pro příjem dat převeden na server pro odesílání dat, musí být znovu proveden import aktualizací serveru katalogu.
  
Pokud dojde k převedení serveru pro příjem dat na server pro odesílání dat, je nutné také znovu naimportovat všechny aktualizace serveru katalogu. V opačném případě se nezdaří synchronizace nových revizí aktualizací serveru katalogu na tento server.
  
#### Pokud je používána Internetová informační služba s protokolem SSL, je nešifrovaný přístup stále možný, pokud není zaškrtnuté políčko Vyžadovat zabezpečený kanál.
  
Pokud nastavíte Internetovou informační službu, aby prostřednictvím instalace certifikátu používala protokol SSL, je stále možné k webu získat přístup pomocí nešifrovaného protokolu HTTP, pokud není zaškrtnuté políčko Vyžadovat zabezpečený kanál. Další informace naleznete v článku o [povolení šifrování](http://go.microsoft.com/fwlink/?linkid=70601) (http://go.microsoft.com/fwlink/?LinkId=70601, tato stránka může být v angličtině).
  
#### Import serveru katalogu se nemusí zdařit bez oprávnění ke čtení či zápisu do složky %windir%\\TEMP.
  
Import serveru katalogu se nemusí zdařit a zobrazí se chybová zpráva podobná následující, pokud účet síťové služby nemá oprávnění ke čtení či zápisu do složky %windir%\\TEMP: Server nemohl zpracovat požadavek. ---&gt; Nelze nalézt soubor C:\\WINDOWS\\TEMP\\*tempFileName*.dll.
  
#### Při synchronizaci mezi službou WSUS 3.0 a serverem repliky pro příjem dat se službou WSUS 2.0 se může snížit výkon.
  
Pokud je služba WSUS 3.0 nainstalovaná na serveru pro odesílání dat a dojde k pokusu o synchronizaci se serverem repliky pro příjem dat, na kterém běží služba WSUS 2.0, mohou nastat problémy s výkonem. Řešení tohoto problému naleznete v článku [KB 910847](http://go.microsoft.com/fwlink/?linkid=70669) (http://go.microsoft.com/fwlink/?LinkId=70669, tato stránka může být v angličtině).
  
#### Pokud je poštovní server vypnutý nebo nedostupný, nedojde k upozorňování e-mailem a to bez upozornění.
  
Pokud je síťový poštovní server offline, služba WSUS 3.0 bez upozornění přestane posílat upozornění e-mailem. Zapíše však událost 10052 (HealthCoreEmailNotificationRed) do protokolu událostí.
  
#### Změna nastavení na serveru pro odesílání dat se hned neprojeví na serveru pro příjem dat.
  
Pokud se změní konfigurace serveru pro odesílání dat, může chvíli trvat, než se tyto změny projeví. Pokud se například změní nastavení serveru pro odesílání dat jako třeba výběr nového jazyka a pokud je okamžitě spuštěna synchronizace serveru pro příjem dat, tato změna se neprojeví. Místo toho bude tato změna aktualizována na serveru pro příjem dat až při příští naplánované synchronizaci. Doba čekání se zvyšuje s počtem aktualizací přítomných na serveru pro odesílání dat.
  
#### Odinstalace služby WSUS 3.0 neodinstaluje instanci databáze
  
Při odinstalaci služby WSUS 3.0 nedojde k odinstalaci instance databáze. Instance může být sdílena více aplikacemi a její odebrání by mohlo způsobit selhání jiné aplikace.
  
Pokud je nezbytné server Interní databáze systému Windows odinstalovat, použijte k odinstalaci aplikace následující příkazy:
  
(na 32bitových platformách)
  
```  
msiexec /x {CEB5780F-1A70-44A9-850F-DE6C4F6AA8FB} callerid=ocsetup.exe  
```  
(na 64bitových platformách)
  
```  
msiexec /x {BDD79957-5801-4A2D-B09E-852E7FA64D01} callerid=ocsetup.exe  
```  
Pokud chcete odinstalovat aplikaci Interní databáze systému Windows Service Pack 2 ze serveru Windows Server 2008, můžete to udělat prostřednictvím nástroje Správce serverů.
  
Odebrání aplikace však neodebere výchozí soubory MDB a LDB, které způsobí selhání příštích instalací služby WSUS 3.0. Tyto soubory mohou být odstraněny z adresáře %windir%\\SYSMSI\\SSEE.
  
#### Pokud server pro příjem dat změní svůj server pro odesílání dat, aktualizace se stavem Neznámý jsou hlášeny jako Nelze použít.
  
Pokud se server pro příjem dat začne synchronizovat s jiným serverem pro odesílání dat, aktualizace se stavem Neznámý budou hlášeny na novém serveru pro odesílání dat jako Nelze použít. Tento stav je dočasný a bude opraven při příštím hlášení stavu serveru pro příjem dat poté, co se s ním klienti synchronizovali.
  
#### Pokud server repliky se službou WSUS 3.0 spravuje více než jeden počítač se stejným názvem, nezdaří se souhrn hlášení.
  
Pokud server repliky se službou WSUS 3.0 spravuje více než jeden počítač se stejným názvem, nezdaří se souhrn hlášení. Hlášení dostupná kořenovému serveru služby WSUS tak nebudou kompletní. Tento problém se vyřeší tak, že se na serveru repliky odstraní duplicitní položky počítače (aby zůstal vždy jen jedna, neduplicitní).
  
#### Pokud vyprší časový limit Průvodce vyčištěním serveru na jednom ze serverů v případě, že průvodce běží na více serverech ze vzdálené konzoly, bude ztraceno připojení ke všem serverům.
  
Průvodce vyčištěním serveru je možné spustit na více serverech z jedné vzdálené konzoly. Pokud však časový limit procesu čištění vyprší na jednom ze serverů, ztratí konzola připojení ke všem serverům. Žádná data nebudou ztracena, ale správce bude muset obnovit vzdálená připojení ke každému ze serverů.
  
#### Průvodce vyčištěním serveru odstraní soubory po třiceti dnech, nikoli po třech měsících.
  
Některý text uvedený v Průvodci vyčištěním serveru není přesný. Průvodce obsahuje pokyny k odstranění aktualizací, jejichž platnost vypršela a které nebyly schváleny po dobu tří měsíců, a k odstranění starých revizí aktualizací, které nebyly schváleny po dobu tří měsíců. Správným časovým údajem je však třicet dní, nikoli tři měsíce.
  
#### Spuštění a zastavení připojování v rychlém sledu způsobuje v Průvodci konfigurací zobrazení chybové zprávy, že nedošlo k chybě synchronizace.
  
V průběhu konfigurace služby WSUS jste vyzváni, abyste se připojili k serveru pro odesílání dat (k serveru Microsoft Update nebo k serveru pro odesílání dat v intranetu) za účelem přenosu základních informací o serveru. Pokud klepnete na tlačítko **Spustit připojování** a poté ihned na tlačítko **Zastavit připojování**, zobrazí se nesprávná chybová zpráva: Nedošlo k žádné chybě synchronizace.
  
#### Klienti služby WSUS se systémem Windows Vista RTM mohou nyní vyhledávat aktualizace na webu Microsoft Update.
  
V předchozích verzích služby WSUS mohli klienti se systémem Windows Vista RTM získávat aktualizace pouze ze serveru WSUS. Počínaje verzí WSUS 3.0 RTM mohou klienti se systémem Vista získat aktualizace i z webu Microsoft Update. Klienty se systémem Vista lze nasměrovat na web Microsoft Update tak, že přejdete na ovládací panel Windows Update a klepnete na hypertextový odkaz **Zjišťovat aktualizace na webu Microsoft Update Service**. Je-li povolená možnost zásad skupiny **Odebrat přístup ke všem funkcím programu Windows Update**, na ovládacím panelu Windows Update nebude zobrazen tento hypertextový odkaz.
  
Služba WSUS 3.0 v systému Windows Server 2008  
---------------------------------------------
  
#### Podporované verze
  
Služba WSUS 3.0 podporuje 32bitové a 64bitové verze systému Windows Server 2008.
  
#### Předpoklady
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Požadavek</th>
<th style="border:1px solid black;" >Podrobnosti</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Internetová informační služba (IIS)</td>
<td style="border:1px solid black;">Instalujte z operačního systému. Zkontrolujte, zda jsou povolené následující součásti:
Ověřování systému Windows
Statický obsah
ASP.NET
Kompatibilita správy služby IIS 6.0
Kompatibilita metabáze služby IIS</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Balíček Microsoft .NET Framework verze 2.0 Redistributable Package (x86)</td>
<td style="border:1px solid black;">V systému Windows Server 2008 není nutné, již nainstalováno jako součást operačního systému.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Konzola Microsoft Management Console 3.0</td>
<td style="border:1px solid black;">V systému Windows Server 2008 není nutné, již nainstalováno jako součást operačního systému.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Prohlížeč sestav společnosti Microsoft</td>
<td style="border:1px solid black;">Tato součást je nutná k používání uživatelského rozhraní služby WSUS. Viz Microsoft Report Viewer Redistributable 2005 na webu služby <a href="http://go.microsoft.com/fwlink/?linkid=70410">Stažení softwaru</a> (http://go.microsoft.com/fwlink/?LinkId=70410).</td>
</tr>
</tbody>
</table>
  
#### Problém 1: Před spuštěním služby WSUS 3.0 musí být aktualizován konfigurační soubor Internetové informační služby 7.0.
  
Před spuštěním služby WSUS 3.0 v systému Windows Server 2008 je nutné aktualizovat konfigurační soubor Internetové informační služby. Je třeba provést následující postup:
  
1. Otevřete konfigurační soubor Internetové informační služby: %WINDIR%\\system32\\inetsrv\\applicationhost.config
  
2. Ve značce &lt;System.webServer&gt;&lt;modules&gt; odeberte část &lt;add name="CustomErrorMode"&gt; (pokud existuje).
  
3. Ve značce &lt;System.webServer&gt;&lt;modules&gt; přidejte část &lt;remove name="CustomErrorMode"&gt;.
  
Výsledná značka by měla vypadat takto:
  
```  
      <System.webServer>
<modules>
<remove name="CustomErrorMode">
</modules>
</System.webServer>
```
  
#### Problém 2: Jestliže chcete službu WSUS 3.0 nainstalovat na vlastním portu v systému Windows Server 2008 Beta 3, je potřeba předem vytvořit web.
  
Jestliže budete chtít službu WSUS 3.0 nainstalovat do systému Windows Server 2008 Beta 3 a chcete nakonfigurovat službu WSUS na používání vlastního portu 8530, bude nutné před spuštěním instalačního programu služby WSUS vytvořit web s názvem Správa služby WSUS.
  
Služba WSUS 3.0 na serveru Windows Small Business Server 2003  
-------------------------------------------------------------
  
#### Problém 1: Pokud je virtuální kořen Internetové informační služby omezen pouze na určité adresy IP nebo názvy domén, nebude se moci server WSUS 3.0 sám aktualizovat.
  
Některé instalace serveru Windows Small Business Server mohou mít výchozí web Internetové informační služby nakonfigurovaný na možnost Omezení podle adres IP a názvů domén. V takovém případě se klient služby Windows Update na serveru nebude moci sám aktualizovat.
  
#### Problém 2: Instalace služby WSUS 3.0 na Small Business Server – problémy s integrací
  
-   Pokud Windows Small Business Server 2003 používá k přístupu k Internetu proxy server ISA, musí být v dialogovém okně **nastavení** zadány následující hodnoty: nastavení proxy serveru, název proxy serveru a port.  
-   Pokud server ISA používá ověřování systému Windows, měla by být pověření proxy serveru zadána ve tvaru DOMÉNA\\uživatel a tento uživatel by měl být členem skupiny Internet Users.
  
#### Problém 3: Pokud byla k síti přidána podsíť bez použití průvodců serveru Windows SBS, je nutné provést tento postup.
  
Instalační proces serveru WSUS nainstaluje na server dvě virtuální kořenové složky Internetové informační služby: SelfUpdate a ClientWebService. Instalační program také umístí některé soubory do domovského adresáře výchozího webu (na portu 80), který umožní počítačům klientů vlastní aktualizaci přes výchozí web. Ve výchozím nastavení je výchozí web nakonfigurován tak, aby odmítl přístup k jakékoli adrese IP jiné než localhost nebo konkrétní podsítě připojené k serveru. To způsobí, že počítače klientů umístěné jinde než na adrese localhost nebo v jiné konkrétní podsíti se nemohou samy aktualizovat. Pokud byla k síti přidána podsíť bez použití průvodců serveru Microsoft Windows Small Business Server 2003 (Windows SBS), je nutné provést tento postup.
  
1.  V nástroji Správa serveru rozbalte položky **Rozšířená správa**, **Internetová informační služba**, **Webové servery**, **Výchozí webový server**, klepněte pravým tlačítkem na virtuální adresář **Selfupdate** a potom klepněte na příkaz **Vlastnosti**.  
2.  Klepněte na položku **Zabezpečení adresáře**.  
3.  V části **Omezení podle adres IP a názvů domén** klepněte na tlačítko **Upravit** a potom klepněte na přepínač **Udělit přístup**.  
4.  Klepněte na tlačítko **OK**, klepněte pravým tlačítkem na virtuální adresář **ClientWebService** a poté klepněte na příkaz **Vlastnosti**.  
5.  Klepněte na položku **Zabezpečení adresáře**.  
6.  V části **Omezení podle adres IP a názvů domén** klepněte na tlačítko **Upravit** a potom klepněte na přepínač **Udělit přístup**.
  
#### Autorská práva
  
Tento dokument podporuje předběžné vydání softwarového produktu, který může být před svým konečným komerčním vydáním zásadně změněn, a představuje důvěrnou a chráněnou informaci společnosti Microsoft Corporation. Je odtajněn na základě smlouvy o utajení mezi příjemcem dokumentu a společností Microsoft. Tento dokument je poskytován pouze k informativním účelům a společnost Microsoft v něm neposkytuje žádné záruky, ať už výslovně uvedené nebo odvozené. Informace v tomto dokumentu včetně adres URL a dalších odkazů na web se mohou změnit bez předchozího upozornění. Riziko vzniklé používáním nebo výsledky používání tohoto dokumentu nese uživatel. Pokud není uvedeno jinak, jsou názvy společností, organizací, produktů, názvy domén, e-mailové adresy, loga, osoby, místa či události použité v příkladech smyšlené. Není zamýšleno a nemůže být vyvozováno žádné jejich spojení se skutečnou společností, organizací, produktem, názvem domény, e-mailovou adresou, logem, osobou, místem či událostí. Povinností uživatele je dodržet všechny zákonné normy týkající se autorských práv. Bez omezení práv vyplývajících z autorských práv nesmí být žádná část tohoto dokumentu kopírována, uložena do veřejného systému ani rozšiřována jakýmkoli způsobem (elektronicky, mechanicky, fotokopiemi, záznamem nebo jinak) ani za žádným účelem bez výslovného písemného povolení společnosti Microsoft Corporation.
  
Společnost Microsoft může vlastnit patenty, patentové přihlášky, ochranné známky, autorská práva a další práva týkající se duševního vlastnictví, které se vztahují k předmětu tohoto dokumentu. Není-li výslovně uvedeno jinak v písemné licenční smlouvě se společností Microsoft, neposkytuje tento dokument žádnou licenci na uvedené patenty, ochranné známky, autorská práva nebo jiné duševní vlastnictví.
  
© 2007 Microsoft Corporation. Všechna práva vyhrazena.
  
Microsoft, SQL Server, Windows a Windows Server jsou registrované ochranné známky nebo ochranné známky společnosti Microsoft Corporation ve Spojených státech amerických a v dalších zemích.
  
Všechny ostatní ochranné známky jsou ochrannými známkami příslušných vlastníků.
