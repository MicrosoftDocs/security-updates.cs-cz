---
TOCTitle: 'MS08-JAN'
Title: 'Souhrnný bulletin zabezpečení společnosti Microsoft, leden 2008'
ms:assetid: 'ms08-jan'
ms:contentKeyID: 61223974
ms:mtpsurl: 'https://technet.microsoft.com/cs-CZ/library/ms08-jan(v=Security.10)'
---

 

Souhrnný bulletin zabezpečení společnosti Microsoft, leden 2008
===============================================================

Publikováno: 8. ledna 2008 | Aktualizováno: 25. ledna 2008

**Verze:** 1.2

Tento souhrnný bulletin uvádí bulletiny zabezpečení vydané v lednu 2008.

Spolu s vydáním bulletinů pro leden 2008 nahrazuje tento souhrnný bulletin předběžné oznámení o bulletinech vydané 3. ledna 2008. Další informace o službě předběžného oznámení o bulletinech naleznete v části [Předběžné oznámení o bulletinech zabezpečení společnosti Microsoft](http://technet.microsoft.com/security/bulletin/advance).

Informace o tom, jak dostávat automatická oznámení o vydání nových bulletinů zabezpečení společnosti Microsoft, naleznete na webu [Zasílání technických oznámení o zabezpečení společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=21163).

Pro zodpovězení zákaznických dotazů týkajících se těchto bulletinů uspořádá společnost Microsoft webové vysílání 9. ledna 2008 v 11:00 časového pásma Tichomoří (USA a Kanada). [Registrovat se pro webové vysílání týkající se lednových bulletinů zabezpečení](http://msevents.microsoft.com/cui/webcasteventdetails.aspx?eventid=1032357213&eventcategory=4&culture=en-us&countrycode=us). Po tomto datu je webové vysílání dostupné na požádání. Další informace získáte v [souhrnných bulletinech zabezpečení společnosti Microsoft a webovém vysílání](http://technet.microsoft.com/security/bulletin/summary).

Společnost Microsoft se snaží zákazníkům usnadnit upřednostnění měsíčně vydávaných aktualizací zabezpečení před jakýmikoli důležitými aktualizacemi nesouvisejícími se zabezpečením, které jsou vydány ve stejný den jako měsíčně vydávané aktualizace zabezpečení. Další informace získáte v části **Další informace**.

### Informace o bulletinech

#### Shrnutí

Bulletiny zabezpečení podle závažnosti:

Kritický (1)
------------

 
| Identifikátor bulletinu            | Bulletin zabezpečení společnosti Microsoft MS08-001                                                                                                                                                                                                                                                                                                                                                                                        |
|------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Název bulletinu**                | [**Chyby zabezpečení v protokolu TCP/IP systému Windows mohou umožnit vzdálené spuštění kódu (941644)**](http://technet.microsoft.com/security/bulletin/ms08-001)                                                                                                                                                                                                                                                                          |
| **Shrnutí**                        | Tato kritická aktualizace zabezpečení řeší dvě chyby zabezpečení ve zpracování protokolu TCP/IP (Transmission Control Protocol/Internet Protocol), které byly oznámeny soukromými osobami. Útočník, který by tuto chybu zabezpečení zneužil, by mohl získat úplnou kontrolu nad postiženým systémem. Útočník by tak mohl instalovat programy, zobrazovat, měnit či odstraňovat data nebo vytvářet nové účty s úplnými uživatelskými právy. |
| **Stupeň maximální závažnosti**    | [Kritický](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                   |
| **Dopad této chyby zabezpečení**   | Vzdálené spuštění kódu                                                                                                                                                                                                                                                                                                                                                                                                                     |
| **Rozpoznávání**                   | Pomocí nástroje MBSA (Microsoft Baseline Security Analyzer) lze určit, zda počítačový systém potřebuje tuto aktualizaci. Aktualizace bude vyžadovat restartování počítače.                                                                                                                                                                                                                                                                 |
| **Software obsahující tuto chybu** | **Windows.** Další informace získáte v části Software obsahující tuto chybu a umístění aktualizací ke stažení.                                                                                                                                                                                                                                                                                                                             |

Vysoký (1)
----------

 
| Identifikátor bulletinu            | Bulletin zabezpečení společnosti Microsoft MS08-002                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
|------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Název bulletinu**                | [**Chyba zabezpečení služby LSASS umožňuje místní zvýšení úrovně oprávnění (943485)**](http://technet.microsoft.com/security/bulletin/ms08-002)                                                                                                                                                                                                                                                                                                                                                                            |
| **Shrnutí**                        | Tato důležitá aktualizace řeší chybu zabezpečení služby LSASS (Microsoft Windows Local Security Authority Subsystem Service), která byla oznámena soukromou osobou. Tato chyba zabezpečení by mohla útočníkovi umožnit spuštění libovolného kódu se zvýšenými oprávněními. Útočník, který by tuto chybu zabezpečení zneužil, by mohl získat úplnou kontrolu nad postiženým systémem. Útočník by tak mohl instalovat programy, zobrazovat, měnit či odstraňovat data nebo vytvářet nové účty s úplnými uživatelskými právy. |
| **Stupeň maximální závažnosti**    | [Vysoký](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| **Dopad této chyby zabezpečení**   | Zvýšení úrovně oprávnění v místním systému                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| **Rozpoznávání**                   | Pomocí nástroje MBSA (Microsoft Baseline Security Analyzer) lze určit, zda počítačový systém potřebuje tuto aktualizaci. Aktualizace bude vyžadovat restartování počítače.                                                                                                                                                                                                                                                                                                                                                 |
| **Software obsahující tuto chybu** | **Windows.** Další informace získáte v části Software obsahující tuto chybu a umístění aktualizací ke stažení.                                                                                                                                                                                                                                                                                                                                                                                                             |

Software obsahující tuto chybu a umístění aktualizací ke stažení
----------------------------------------------------------------

 
**Jak pracovat s touto tabulkou**

V této tabulce zjistíte, které aktualizace zabezpečení bude třeba nainstalovat. Přečtěte si seznam všech programů a součástí a zjistěte, zda jsou u nich vyžadovány aktualizace zabezpečení. Pokud se program nebo součást v seznamu nachází, je u nich uveden dopad chyby zabezpečení s odkazem na příslušnou aktualizaci.

**Poznámka:** Jedna chyba zabezpečení může vyžadovat instalaci více aktualizací. Přečtěte si celý sloupec u každého identifikátoru bulletinu. Zjistíte v něm, které aktualizace nainstalovat v závislosti na programech nebo součástech nainstalovaných ve vašem systému.

**Software obsahující tuto chybu a umístění aktualizací ke stažení**

 
<p></p>
<table style="border:1px solid black;">
<tr class="thead">
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
Podrobnosti
</th>
<th style="border:1px solid black;" >
Podrobnosti
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS08-001**](http://technet.microsoft.com/security/bulletin/ms08-001)
</td>
<td style="border:1px solid black;">
[**MS08-002**](http://technet.microsoft.com/security/bulletin/ms08-002)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Stupeň maximální závažnosti**
</td>
<td style="border:1px solid black;">
[**Kritický**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Důležité**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<th style="border:1px solid black;" colspan="3">
Operační systém Windows
</th>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Windows 2000 Service Pack 4
</td>
<td style="border:1px solid black;">
[Mírný](http://www.microsoft.com/downloads/details.aspx?familyid=980f5457-c7b5-421c-8643-0e57429ec156)
</td>
<td style="border:1px solid black;">
[Vysoký](http://www.microsoft.com/downloads/details.aspx?familyid=7956632e-17d9-4876-8340-84fe3e43e5cc)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Service Pack 2
</td>
<td style="border:1px solid black;">
[Kritický](http://www.microsoft.com/downloads/details.aspx?familyid=0a766242-2342-4fa0-9b66-8953c54a2211)
</td>
<td style="border:1px solid black;">
[Vysoký](http://www.microsoft.com/downloads/details.aspx?familyid=6a4cf182-8e36-490e-aefe-edb7b3a0df9c)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Professional x64 Edition a Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Kritický](http://www.microsoft.com/downloads/details.aspx?familyid=2e8bc7d5-fe81-4ed5-9efa-360738d160ee)
</td>
<td style="border:1px solid black;">
[Vysoký](http://www.microsoft.com/downloads/details.aspx?familyid=51fc657b-2b4a-4725-a744-d279e027c4a5)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 1 a Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Vysoký](http://www.microsoft.com/downloads/details.aspx?familyid=fda060a5-9a1e-4036-9899-13eb61fdd8be)
</td>
<td style="border:1px solid black;">
[Vysoký](http://www.microsoft.com/downloads/details.aspx?familyid=12397b47-b18f-4d4d-b8d7-adec8ff310d5)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition a Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Vysoký](http://www.microsoft.com/downloads/details.aspx?familyid=19d993f9-06dd-4dc4-b0cc-c59e822eb8fa)
</td>
<td style="border:1px solid black;">
[Vysoký](http://www.microsoft.com/downloads/details.aspx?familyid=f19fd790-a4e6-4a8a-8077-d1bbfe37ecca)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 SP1 pro systémy s procesorem Itanium a Windows Server 2003 SP2 pro systémy s procesorem Itanium
</td>
<td style="border:1px solid black;">
[Vysoký](http://www.microsoft.com/downloads/details.aspx?familyid=2c2264f7-ebbb-40ab-9dbf-9b4e313665a7)
</td>
<td style="border:1px solid black;">
[Vysoký](http://www.microsoft.com/downloads/details.aspx?familyid=0382a195-aa3d-409b-8a79-9fe61588d8a9)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Small Business Server 2003 Service Pack 1, Windows Small Business Server 2003 R2, Windows Small Business Server 2003 R2 Service Pack 2 a Windows Home Server
</td>
<td style="border:1px solid black;">
[Kritický](http://www.microsoft.com/downloads/details.aspx?familyid=fda060a5-9a1e-4036-9899-13eb61fdd8be)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista
</td>
<td style="border:1px solid black;">
[Kritický](http://www.microsoft.com/downloads/details.aspx?familyid=23c0e03a-db66-4618-bce0-af55e5c1b067)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 Edition
</td>
<td style="border:1px solid black;">
[Kritický](http://www.microsoft.com/downloads/details.aspx?familyid=5f6a37b1-c604-47c9-932f-485db2eda133)
</td>
<td style="border:1px solid black;">
</td>
</tr>
</table>
<p></p>
 

Nástroje a doporučené postupy zjišťování a nasazení
---------------------------------------------------

 
**Centrum zabezpečení**

Umožňuje správu aktualizací softwaru a zabezpečení, které je třeba nainstalovat na servery, stolní počítače a přenosné počítače v organizaci. Další informace naleznete na webu [TechNet Update Management Center](http://go.microsoft.com/fwlink/?linkid=69903). Další informace o zabezpečení produktů společnosti Microsoft nabízí web [Centrum zabezpečení TechNet](http://go.microsoft.com/fwlink/?linkid=21171). Tyto informace lze také získat klepnutím na nabídku „Nejnovější aktualizace zabezpečení“ na webu [Zabezpečení doma](http://go.microsoft.com/fwlink/?linkid=85102).

Aktualizace zabezpečení jsou k dispozici na webu [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747), [Windows Update](http://go.microsoft.com/fwlink/?linkid=21130) a [Office Update](http://go.microsoft.com/fwlink/?linkid=21135). Aktualizace zabezpečení jsou také k dispozici na webu [služby Stažení softwaru](http://go.microsoft.com/fwlink/?linkid=21129). Nejsnadněji je naleznete hledáním podle klíčových slov aktualizace zabezpečení.

Aktualizace zabezpečení lze stáhnout z katalogu služby [Microsoft Update Catalog](http://go.microsoft.com/fwlink/?linkid=96155). Služba Microsoft Update Catalog poskytuje katalog s možností vyhledávání obsahu dostupného prostřednictvím služeb Windows Update a Microsoft Update, včetně aktualizací zabezpečení, ovladačů a aktualizací Service Pack. Vyhledáváním pomocí čísla bulletinu zabezpečení (například MS07-036) můžete přidat všechny dostupné aktualizace do košíku (včetně různých jazykových verzí aktualizace) a stáhnout je do vybrané složky. Další informace o službě Microsoft Update Catalog najdete v části [Nejčastější dotazy týkající se služby Microsoft Update Catalog](http://go.microsoft.com/fwlink/?linkid=97900).

**Doporučené postupy zjišťování a instalace**

Společnost Microsoft poskytla doporučené postupy zjišťování a instalace aktualizací zabezpečení vydaných tento měsíc. Tyto doporučené postupy by měly pomoci také odborníkům v oblasti IT při používání různých nástrojů při instalaci aktualizace zabezpečení, např. Windows Update, Microsoft Update, Office Update, nástroj MBSA (Microsoft Baseline Security Analyzer), nástroj pro rozpoznávání sady Office, Microsoft Systems Management Server (SMS) a nástroj Extended Security Update Inventory Tool (ESUIT). Další informace získáte v [článku 910723 znalostní báze Microsoft Knowledge Base](http://support.microsoft.com/kb/910723).

**Nástroj Microsoft Baseline Security Analyzer**

Pomocí nástroje Microsoft Baseline Security Analyzer (MBSA) mohou správci prohledávat místní i vzdálené systémy a zjistit tak, jestli v nich nechybí některé aktualizace zabezpečení nebo jestli v nastavení zabezpečení systému nedošlo k některým běžným chybám. Další informace o nástroji MBSA získáte na webu [Microsoft Baseline Security Analyzer](http://go.microsoft.com/fwlink/?linkid=21134).

**Služba Windows Server Update Services**

Pomocí služby Windows Server Update Services (WSUS) mohou správci systémů rychle a spolehlivě instalovat nejnovější důležité aktualizace zabezpečení pro systémy Windows 2000 a novější, sadu Office XP a novější, Exchange Server 2003 a SQL Server 2000 do systémů Windows 2000 a novějších.

Další informace o způsobu instalace této aktualizace zabezpečení pomocí služby Windows Server Update Services získáte na webu služby [Windows Server Update Services](http://go.microsoft.com/fwlink/?linkid=50120).

**Systems Management Server**

Microsoft Systems Management Server (SMS) představuje v rozlehlých sítích řešení pro správu aktualizací s rozsáhlými možnostmi konfigurace. Umožňuje správcům identifikovat počítače se systémem Windows, které vyžadují aktualizace zabezpečení, a provést řízenou instalaci těchto aktualizací v celé rozlehlé síti s minimálním dopadem na koncové uživatele. K dispozici je nyní nová verze nástroje SMS, System Center Configuration Manager 2007 (viz také webové stránky produktu [System Center Configuration Manager 2007](http://technet.microsoft.com/en-us/library/bb735860.aspx)). Další informace o tom, jak mohou správci pomocí serveru SMS 2003 nasazovat aktualizace zabezpečení, získáte na webu [SMS 2003 Security Patch Management](http://go.microsoft.com/fwlink/?linkid=22939). Uživatelé serveru SMS 2.0 mohou při nasazení aktualizací zabezpečení použít také sadu [Software Updates Services Feature Pack](http://go.microsoft.com/fwlink/?linkid=33340). Další informace o serveru SMS získáte na webu [Microsoft Systems Management Server](http://go.microsoft.com/fwlink/?linkid=21158).

**Poznámka:** Server SMS využívá nástroj MBSA (Microsoft Baseline Security Analyzer) a nástroj pro rozpoznávání sady Microsoft Office, a poskytuje tak širokou podporu pro zjišťování a instalaci aktualizací uvedených v bulletinech zabezpečení. Tyto nástroje nemusí některé softwarové aktualizace zjistit. V takovém případě mohou správci použít funkce serveru SMS a nasměrovat aktualizace do určitých systémů. Další informace o tomto postupu najdete na webu [Nasazení aktualizací softwaru pomocí funkce Distribuce softwaru serveru SMS](http://go.microsoft.com/fwlink/?linkid=33341). Některé aktualizace zabezpečení vyžadují po restartování počítače oprávnění správce. Správci mohou k instalaci těchto aktualizací použít nástroj Elevated Rights Deployment Tool (k dispozici v sadě [SMS 2003 Administration Feature Pack](http://go.microsoft.com/fwlink/?linkid=33387) a [SMS 2.0 Administration Feature Pack](http://go.microsoft.com/fwlink/?linkid=21161)).

### Další informace

#### Nástroj pro odstranění škodlivého softwaru systému Microsoft Windows

Společnost Microsoft vydává aktualizovanou verzi Nástroje pro odstranění škodlivého softwaru systému Microsoft Windows na webu Windows Update, Microsoft Update, ve službě Windows Server Update Services a v centru pro stahování Download Center.

#### Důležité aktualizace nesouvisející se zabezpečením na webu Microsoft Update (MU), Windows Update (WU) a ve službě Windows Server Update Services (WSUS)

Tento měsíc:

-   Společnost Microsoft vydala pět důležitých aktualizací **nesouvisejících se zabezpečením** na webu Microsoft Update (MU) a ve službě Windows Server Update Services (WSUS).
-   Společnost Microsoft vydala dvě důležité aktualizace systému Windows **nesouvisející se zabezpečením** na webu Windows Update (WU) a ve službě Windows Server Update Services (WSUS).

Tato informace se týká **pouze** důležitých aktualizací **nesouvisejících se zabezpečením** na webu Microsoft Update, Windows Update a ve službě Windows Server Update Services vydaných ve stejný den jako souhrnný bulletin zabezpečení. Informace **se netýká** aktualizací **nesouvisejících se zabezpečením** vydaných v jiné dny.

#### Strategie zabezpečení a komunita

**Strategie instalace aktualizací**

Web [Doporučené postupy zabezpečení pro správu oprav (Security Guidance for Patch Management)](http://go.microsoft.com/fwlink/?linkid=21168) obsahuje další informace o instalaci aktualizací zabezpečení podle doporučení společnosti Microsoft.

**Získání dalších aktualizací zabezpečení**

Aktualizace odstraňující další problémy se zabezpečením získáte v následujících umístěních:

-   Aktualizace zabezpečení jsou k dispozici na webu služby [Stažení softwaru (Microsoft Download Center)](http://go.microsoft.com/fwlink/?linkid=21129). Nejsnadněji je naleznete hledáním podle klíčových slov aktualizace zabezpečení.
-   Aktualizace pro klientské platformy jsou k dispozici na webu [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747).
-   Aktualizace zabezpečení nabízené tento měsíc na webu Windows Update jsou k dispozici na webu služby Stažení softwaru v souborech obrazu ISO disku CD s vydanými aktualizacemi zabezpečení a kritickými aktualizacemi. Další informace získáte v [článku 913086 znalostní báze Microsoft Knowledge Base](http://support.microsoft.com/kb/913086).

**Komunita odborníků v oblasti zabezpečení**

Můžete se zde naučit, jak zlepšit zabezpečení a jak optimalizovat infrastrukturu IT. Také můžete s dalšími členy komunity IT Pro diskutovat o bezpečnostních tématech na webu [Komunita odborníků v oblasti zabezpečení (IT Pro Security Community)](http://go.microsoft.com/fwlink/?linkid=21164).

#### Poděkování

Společnost Microsoft tímto [děkuje](http://go.microsoft.com/fwlink/?linkid=21127) za spolupráci při ochraně zákazníků:

-   Alexi Wheelerovi a Ryanu Smithovi ze společnosti [IBM Internet Security Systems X-Force](http://www.iss.net/) za oznámení chyby popsané v bulletinu [MS08-001](http://technet.microsoft.com/security/bulletin/ms08-001).
-   Alexi Wheelerovi a Ryanu Smithovi ze společnosti [IBM Internet Security Systems X-Force](http://www.iss.net/) za oznámení chyby popsané v bulletinu [MS08-001](http://technet.microsoft.com/security/bulletin/ms08-001).
-   Thomasi Garnierovi ze společnosti [SkyRecon](http://www.skyrecon.com/) za oznámení chyby popsané v bulletinu [MS08-002](http://technet.microsoft.com/security/bulletin/ms08-002).

#### Technická podpora

-   Uvedený software byl testován za účelem zjištění, kterých verzí se chyba týká. U dalších verzí skončila časově omezená podpora. Pokud chcete zjistit dobu, po kterou je pro určitou verzi softwaru poskytována podpora, navštivte web [Zásady poskytování technické podpory pro produkty společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=21742).
-   Zákazníci mohou získat technickou podporu na webu [služby technické podpory společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=21131). Hovory související s aktualizacemi zabezpečení jsou bezplatné.
-   Mezinárodní zákazníci získají podporu u místních zastoupení společnosti Microsoft. Technická podpora související s aktualizacemi zabezpečení je bezplatná. Další informace o možnostech kontaktování společnosti Microsoft v případě potřeby technické podpory získáte na [webu mezinárodní technické podpory](http://go.microsoft.com/fwlink/?linkid=21155).

#### Zřeknutí se záruky

Informace ve znalostní bázi Microsoft Knowledge Base jsou poskytovány tak, jak jsou, bez jakékoli záruky. Společnost Microsoft neposkytuje žádné záruky, výslovně uvedené či mlčky předpokládané, včetně záruk obchodovatelnosti a vhodnosti pro určitý účel. Společnost Microsoft ani její dodavatelé nenesou v žádném případě zodpovědnost za žádné škody, včetně přímých, nepřímých, náhodných či následných škod, ztráty zisku či zvláštních škod, a to ani v případě, že byli na možnost takových škod upozorněni. V některých zemích a právních řádech není dovoleno vyloučit nebo omezit odpovědnost, proto se výše uvedené omezení na vás nemusí vztahovat.

#### Revize

-   V1.0 (8. ledna 2008): Souhrnný bulletin byl publikován.
-   V1.1 (23. ledna 2008): Souhrnný bulletin byl aktualizován, aby do seznamu softwaru obsahujícího chybu zabezpečení, uvedeného v bulletinu MS08-001, přidal systém Windows Small Business Server 2003 Service Pack 2.
-   V1.2 (25. ledna 2008): Souhrnný bulletin byl aktualizován, aby do seznamu softwaru obsahujícího chybu zabezpečení uvedenou v bulletinu MS08-001 přidal systém Windows Small Business Server 2003 Service Pack 1, Windows Small Business Server 2003 R2, Windows Small Business Server 2003 R2 Service Pack 2 a Windows Home Server.

*Built at 2014-04-18T01:50:00Z-07:00*
