---
TOCTitle: 'MS04-NOV'
Title: 'Souhrnný bulletin zabezpečení společnosti Microsoft, listopad 2004'
ms:assetid: 'ms04-nov'
ms:contentKeyID: 61223934
ms:mtpsurl: 'https://technet.microsoft.com/cs-CZ/library/ms04-nov(v=Security.10)'
---

 

Souhrnný bulletin zabezpečení společnosti Microsoft, listopad 2004
==================================================================

Publikováno: 9. listopadu 2004

**Verze:** 1.0

**Vydáno:** 9. listopadu 2004  
**Číslo verze:** 1.0

Verze tohoto článku pro koncové uživatele je k dispozici na následujícím [webu](http://www.microsoft.com/security/default.mspx).

**Chraňte svůj počítač:** V následujících umístěních získáte informace společnosti Microsoft týkající se zlepšení ochrany počítače:

-   web [Chraňte svůj počítač](http://www.microsoft.com/cze/athome/security/protect/windowsxpsp2/default.mspx) pro koncové uživatele,
-   web [Security Guidance Center](http://go.microsoft.com/fwlink/?linkid=21171) pro odborníky v oblasti IT.

**Strategie instalace aktualizací:** Web [Patch Management, Security Updates, and Downloads](http://go.microsoft.com/fwlink/?linkid=21168) obsahuje další informace o instalaci aktualizací zabezpečení podle doporučení společnosti Microsoft.

**Komunita odborníků v oblasti zabezpečení:** Na webu [IT Pro Security Zone](http://go.microsoft.com/fwlink/?linkid=21164) se dozvíte, jak zlepšit zabezpečení a optimalizovat svou infrastrukturu IT, a diskutovat s dalšími členy komunity odborníků o tématech týkajících se zabezpečení.

**Služba zasílání oznámení o zabezpečení společnosti Microsoft:** Pokud chcete e-mailem dostávat automatická oznámení o vydání nových bulletinů zabezpečení společnosti Microsoft, přihlaste se k jejich odběru na adrese [Microsoft Security Notification Service](http://go.microsoft.com/fwlink/?linkid=21163).

#### Shrnutí

Součástí tohoto informačního zpravodaje jsou opravy nově zjištěných chyb zabezpečení. Tyto chyby jsou, podle stupně závažnosti, uvedeny níže:

Vysoký (1)
----------

<span></span>
| Identifikátor bulletinu             | Bulletin zabezpečení společnosti MS04-039                                                                                |
|-------------------------------------|--------------------------------------------------------------------------------------------------------------------------|
| **Název bulletinu**                 | Chyba zabezpečení v serveru ISA Server 2000 a Proxy Server 2.0 umožňuje vkládání falešného internetového obsahu (888258) |
| **Hlavní závěry:**                  | Tato chyba zabezpečení útočníkovi umožňuje nahradit důvěryhodný internetový obsah falešným obsahem.                      |
| **Stupeň maximální závažnosti**     | [Vysoký](http://go.microsoft.com/fwlink/?linkid=21140)                                                                   |
| **Dopad této chyby zabezpečení**    | Vkládání falešného obsahu                                                                                                |
| **Software obsahující tuto chybu:** | **Windows** Další informace získáte v části Software obsahující tuto chybu a umístění aktualizací ke stažení.            |

Software obsahující tuto chybu a umístění aktualizací ke stažení
----------------------------------------------------------------

<span></span>
**Jak pracovat s touto tabulkou**

V této tabulce zjistíte, které aktualizace zabezpečení bude třeba nainstalovat. Přečtěte si seznam všech programů a součástí a zjistěte, zda jsou u nich uvedeny aktualizace zabezpečení. Pokud se program nebo součást v seznamu nachází, je u nich uveden dopad chyby zabezpečení s odkazem na příslušnou aktualizaci.

**Software obsahující tuto chybu a umístění aktualizací ke stažení**

|                                                                                                                                                   | Podrobnosti                                                                                             |
|---------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------|
| **Identifikátor bulletinu**                                                                                                                       | **MS04-039**                                                                                            |
| **Stupeň maximální závažnosti**                                                                                                                   | [**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)                                              |
| **Programy systému Windows obsahující tuto chybu:**                                                                                               |                                                                                                         |
| Microsoft Internet Security and Acceleration Server 2000 Service Pack 1 a Microsoft Internet Security and Acceleration Server 2000 Service Pack 2 | [Vysoký](http://www.microsoft.com/downloads/details.aspx?familyid=7a4c318f-5ac9-4cf2-8792-a4a62076ebe7) |
| Microsoft Small Business Server 2000 (obsahuje Microsoft Internet Security and Acceleration Server 2000)                                          | [Vysoký](http://www.microsoft.com/downloads/details.aspx?familyid=7a4c318f-5ac9-4cf2-8792-a4a62076ebe7) |
| Microsoft Small Business Server 2003 Premium Edition (obsahuje Microsoft Internet Security and Acceleration Server 2000)                          | [Vysoký](http://www.microsoft.com/downloads/details.aspx?familyid=7a4c318f-5ac9-4cf2-8792-a4a62076ebe7) |
| Microsoft Proxy Server 2.0 Service Pack 1                                                                                                         | [Vysoký](http://www.microsoft.com/downloads/details.aspx?familyid=7a4c318f-5ac9-4cf2-8792-a4a62076ebe7) |

Instalace
---------

<span></span>
**Systems Management Server:**

Microsoft Systems Management Server (SMS) představuje podnikové řešení pro správu aktualizací s rozsáhlými možnostmi konfigurace. Umožňuje správcům identifikovat počítače se systémem Windows, které vyžadují aktualizace zabezpečení, a provést řízenou instalaci těchto aktualizací v celém podniku, a to s minimálním dopadem na koncové uživatele. Další informace o tom, jak mohou správci pomocí serveru SMS 2003 instalovat aktualizace zabezpečení, získáte na webu [SMS 2003 Security Patch Management](http://go.microsoft.com/fwlink/?linkid=22939). Uživatelé serveru SMS 2.0 mohou při instalaci aktualizací zabezpečení použít také sadu [Software Updates Service Feature Pack](http://go.microsoft.com/fwlink/?linkid=33340). Další informace o serveru SMS získáte na [webu serveru SMS](http://go.microsoft.com/fwlink/?linkid=21158).

**Poznámka:** Server SMS využívá nástroj MBSA (Microsoft Baseline Security Analyzer) a nástroj pro rozpoznávání sady Microsoft Office, a poskytuje tak širokou podporu pro zjišťování a instalaci aktualizací uvedených v bulletinech zabezpečení. Tyto nástroje nemusí některé softwarové aktualizace zjistit. V takovém případě mohou správci použít funkce serveru SMS a nasměrovat aktualizace do určitých systémů. Další informace o tomto postupu najdete na následujícím [webu](http://go.microsoft.com/fwlink/?linkid=33341). Některé aktualizace zabezpečení vyžadují po restartování počítače oprávnění správce. Správci mohou k instalaci těchto aktualizací použít nástroj Elevated Rights Deployment Tool (k dispozici v sadě [SMS 2003 Administration Feature Pack](http://go.microsoft.com/fwlink/?linkid=33387) a [SMS 2.0 Administration Feature Pack](http://go.microsoft.com/fwlink/?linkid=21161)).

#### Další informace:

**Poděkování**

Společnost Microsoft tímto [děkuje](http://go.microsoft.com/fwlink/?linkid=21127) za spolupráci při ochraně zákazníků:

-   Martijnu de Vriesovi ze společnosti Info Support za odhalení a Thomasi de Klerkovi ze společnosti Info Support za oznámení chyby zabezpečení umožňující vkládání falešného obsahu (CAN-2004-0892).

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
-   Katalog systému Windows Update: Další informace o katalogu systému Windows Update získáte ve znalostní bázi Microsoft Knowledge Base v článku [323166](http://support.microsoft.com/default.aspx?scid=kb;en-us;323166).
-   [Office Update](http://go.microsoft.com/fwlink/?linkid=21135)

**Zřeknutí** **se záruky:**

Informace ve znalostní bázi Microsoft Knowledge Base jsou poskytovány tak, jak jsou, bez jakékoli záruky. Společnost Microsoft neposkytuje žádné záruky, výslovně uvedené či mlčky předpokládané, včetně záruk obchodovatelnosti a vhodnosti pro určitý účel. Společnost Microsoft ani její dodavatelé nenesou v žádném případě zodpovědnost za žádné škody, včetně přímých, nepřímých, náhodných či následných škod, ztráty zisku či zvláštních škod, a to ani v případě, že byli na možnost takových škod upozorněni. V některých zemích a právních řádech není dovoleno vyloučit nebo omezit odpovědnost, proto se výše uvedené omezení na vás nemusí vztahovat.

**Revize:**

-   V1.0 (9. listopadu 2004): Bulletin byl publikován

*Built at 2014-04-18T01:50:00Z-07:00*
