---
TOCTitle: 'MS05-MAY'
Title: 'Souhrnný bulletin zabezpečení společnosti Microsoft, květen 2005'
ms:assetid: 'ms05-may'
ms:contentKeyID: 61223944
ms:mtpsurl: 'https://technet.microsoft.com/cs-CZ/library/ms05-may(v=Security.10)'
---

Souhrnný bulletin zabezpečení společnosti Microsoft, květen 2005
================================================================

Publikováno: 10. května 2005

**Verze:** 1.0

**Vydáno:** 10. května 2005  
**Verze:** 1.0

Verze tohoto článku pro koncové uživatele je k dispozici na následujícím [webu](http://www.microsoft.com/security/default.mspx).

**Chraňte svůj počítač:** V následujících umístěních získáte informace společnosti Microsoft týkající se zlepšení ochrany počítače:

-   web [Chraňte svůj počítač](http://www.microsoft.com/cze/security/protect/) pro koncové uživatele,
-   web [Security Guidance Center](http://www.microsoft.com/cze/security/guidance/) pro odborníky v oblasti IT.

**Strategie instalace aktualizací:** Web [Patch Management, Security Updates, and Downloads](http://go.microsoft.com/fwlink/?linkid=21168) obsahuje další informace o instalaci aktualizací zabezpečení podle doporučení společnosti Microsoft.

**Komunita odborníků v oblasti zabezpečení:** Na webu [IT Pro Security Zone](http://go.microsoft.com/fwlink/?linkid=21164) se dozvíte, jak zlepšit zabezpečení a optimalizovat svou infrastrukturu IT, a diskutovat s dalšími členy komunity odborníků o tématech týkajících se zabezpečení.

**Služba zasílání oznámení o zabezpečení společnosti Microsoft:** Pokud chcete e-mailem dostávat automatická oznámení o vydání nových bulletinů zabezpečení společnosti Microsoft, přihlaste se k jejich odběru na adrese [Microsoft Security Notification Service](http://go.microsoft.com/fwlink/?linkid=21163).

#### Shrnutí

Součástí tohoto informačního zpravodaje jsou opravy nově zjištěné chyby zabezpečení.

Vysoký (1)
----------


| Identifikátor bulletinu             | Bulletin zabezpečení společnosti Microsoft MS05-024                                                                                                 |
|-------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------|
| **Název bulletinu**                 | [**Chyba zabezpečení ve webovém zobrazení může způsobit vzdálené spuštění kódu (894320)**](http://technet.microsoft.com/security/bulletin/ms05_024) |
| **Základní shrnutí**                | Byla zjištěna chyba zabezpečení vkládání skriptu ve webovém zobrazení při zpracování atributů souboru.                                              |
| **Stupeň maximální závažnosti**     | [Vysoký](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                              |
| **Dopad této chyby zabezpečení**    | Vzdálené spuštění kódu                                                                                                                              |
| **Software obsahující tuto chybu:** | **Windows**                                                                                                                                         |

Software obsahující tuto chybu a umístění aktualizací ke stažení
----------------------------------------------------------------


**Jak pracovat s touto tabulkou**

V této tabulce zjistíte, které aktualizace zabezpečení bude třeba nainstalovat. Přečtěte si seznam všech programů a součástí a zjistěte, zda jsou u nich uvedeny aktualizace zabezpečení. Pokud se program nebo součást v seznamu nachází, je u nich uveden dopad chyby zabezpečení s odkazem na příslušnou aktualizaci.

**Software obsahující tuto chybu a umístění aktualizací ke stažení**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" ></th>
<th style="border:1px solid black;" >Podrobnosti        </th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Identifikátor bulletinu</strong></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms05_024"><strong>MS05-024</strong></a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Stupeň maximální závažnosti</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Vysoký</strong></a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Systémy Windows obsahující tuto chybu:</strong></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows 2000 Service Pack 2</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=67581d32-743f-44ff-9b53-30277c196923">Vysoký</a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Microsoft Windows 2000 Service Pack 4</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=67581d32-743f-44ff-9b53-30277c196923">Vysoký</a></td>
</tr>
</tbody>
</table>
  
Instalace  
---------
  

**Služba Software Update Services:**
  
Pomocí služby Microsoft Software Update Services (SUS) mohou správci systémů rychle a spolehlivě instalovat nejnovější důležité aktualizace zabezpečení pro servery se systémem Windows 2000 a Windows Server 2003 i pro stolní počítače se systémem Windows 2000 Professional nebo Windows XP Professional.
  
Další informace o způsobu instalace této aktualizace zabezpečení pomocí služby SUS získáte na [webu služby Software Update Services](http://go.microsoft.com/fwlink/?linkid=21133).
  
**Systems Management Server:**
  
Microsoft Systems Management Server (SMS) představuje podnikové řešení pro správu aktualizací s rozsáhlými možnostmi konfigurace. Umožňuje správcům identifikovat počítače se systémem Windows, které vyžadují aktualizace zabezpečení, a provést řízenou instalaci těchto aktualizací v celém podniku, a to s minimálním dopadem na koncové uživatele. Další informace o tom, jak mohou správci pomocí serveru SMS 2003 instalovat aktualizace zabezpečení, získáte na webu [SMS 2003 Security Patch Management](http://go.microsoft.com/fwlink/?linkid=22939). Uživatelé serveru SMS 2.0 mohou při instalaci aktualizací zabezpečení použít také sadu [Software Updates Service Feature Pack](http://go.microsoft.com/fwlink/?linkid=33340). Další informace o serveru SMS získáte na [webu serveru SMS](http://go.microsoft.com/fwlink/?linkid=21158).
  
**Poznámka:** Server SMS využívá nástroj MBSA (Microsoft Baseline Security Analyzer) a nástroj pro rozpoznávání sady Microsoft Office, a poskytuje tak širokou podporu pro zjišťování a instalaci aktualizací uvedených v bulletinech zabezpečení. Tyto nástroje nemusí některé softwarové aktualizace zjistit. V takovém případě mohou správci použít funkce serveru SMS a nasměrovat aktualizace do určitých systémů. Další informace o tomto postupu najdete na následujícím [webu](http://go.microsoft.com/fwlink/?linkid=33341). Některé aktualizace zabezpečení vyžadují po restartování počítače oprávnění správce. Správci mohou k instalaci těchto aktualizací použít nástroj Elevated Rights Deployment Tool (k dispozici v sadě [SMS 2003 Administration Feature Pack](http://go.microsoft.com/fwlink/?linkid=33387) a [SMS 2.0 Administration Feature Pack](http://go.microsoft.com/fwlink/?linkid=21161)).
  
**Nástroje QChain.exe a Update.exe:**
  
Společnost Microsoft vydala nástroj QChain.exe, který je možné spustit z příkazového řádku. Jeho pomocí může správce systému bezpečně zřetězit aktualizace zabezpečení. *Zřetězení* je termín pro instalaci více aktualizací bez restartování počítače mezi jednotlivými instalacemi. Funkce zřetězení je integrována v nástroji Update.exe, který je používán v aktualizacích popsaných v tomto informačním zpravodaji. V případě systémů Windows 2000 s aktualizací Service Pack 2 nebo vyšší, Windows XP nebo Windows Server 2003 není nutné aktualizace pomocí nástroje Qchain.exe řetězit. přesto však aktualizace těchto systémů podporuje, a umožňuje tak vytvoření konzistentního instalačního skriptu pro všechny platformy. Další informace o nástroji QChain získáte na tomto [webu](http://go.microsoft.com/fwlink/?linkid=21156).
  
**Nástroj MBSA (Microsoft Baseline Security Analyzer):**
  
Pomocí nástroje Microsoft Baseline Security Analyzer (MBSA) mohou správci prohledávat místní i vzdálené systémy a zjistit tak, jestli v nich nechybí některé aktualizace zabezpečení nebo jestli v nastavení zabezpečení systému nedošlo k některým běžným chybám. Další informace o nástroji MBSA získáte na webu [Microsoft Baseline Security Analyzer](http://go.microsoft.com/fwlink/?linkid=21134).
  
#### Další informace:
  
**Získání dalších aktualizací zabezpečení:**
  
Aktualizace odstraňující další problémy se zabezpečením získáte v následujících umístěních:
  
-   Aktualizace zabezpečení jsou k dispozici v centru pro stahování [Microsoft Download Center](http://go.microsoft.com/fwlink/?linkid=21129). Nejsnadněji je naleznete vyhledáním klíčového slova security\_patch (oprava\_zabezpečení).  
-   Aktualizace pro klientské platformy jsou k dispozici na webu [Windows Update](http://go.microsoft.com/fwlink/?linkid=21130).
  
**Technická podpora:**
  
-   Zákazníci v USA a Kanadě mohou získat technickou podporu prostřednictvím služeb [Microsoft Product Support Services](http://go.microsoft.com/fwlink/?linkid=21131) na čísle 1-866-PCSAFETY. Hovory související s aktualizacemi zabezpečení jsou bezplatné.  
-   Ostatní zákazníci získají technickou podporu u místních zastoupení společnosti Microsoft. Technická podpora související s aktualizacemi zabezpečení je bezplatná. Další informace o možnostech kontaktování společnosti Microsoft v případě potřeby technické podpory naleznete na webu [mezinárodní technické podpory](http://go.microsoft.com/fwlink/?linkid=21155).
  
**Zdroje informací o zabezpečení:**
  
-   Další informace o zabezpečení produktů společnosti Microsoft nabízí web [Microsoft TechNet Security](http://go.microsoft.com/fwlink/?linkid=21132).  
-   [Služba Microsoft Software Update Services](http://go.microsoft.com/fwlink/?linkid=21133)  
-   [Nástroj MBSA](http://go.microsoft.com/fwlink/?linkid=21134) (Microsoft Baseline Security Analyzer)  
-   [Windows Update](http://go.microsoft.com/fwlink/?linkid=21130)  
-   Katalog systému Windows Update: Další informace o katalogu systému Windows Update získáte v článku [323166](http://support.microsoft.com/default.aspx?scid=kb;en-us;323166) znalostní báze Microsoft Knowledge Base.  
-   [Office Update](http://go.microsoft.com/fwlink/?linkid=21135)
  
**Zřeknutí se záruky:**
  
Informace ve znalostní bázi Microsoft Knowledge Base jsou poskytovány tak, jak jsou, bez jakékoli záruky. Společnost Microsoft neposkytuje žádné záruky, výslovně uvedené či mlčky předpokládané, včetně záruk obchodovatelnosti a vhodnosti pro určitý účel. Společnost Microsoft ani její dodavatelé nenesou v žádném případě zodpovědnost za žádné škody, včetně přímých, nepřímých, náhodných či následných škod, ztráty zisku či zvláštních škod, a to ani v případě, že byli na možnost takových škod upozorněni. V některých zemích a právních řádech není dovoleno vyloučit nebo omezit odpovědnost, proto se výše uvedené omezení na vás nemusí vztahovat.
  
**Revize:**
  
-   V1.0 (10. května 2005): Bulletin byl publikován.
  
*Built at 2014-04-18T01:50:00Z-07:00*
