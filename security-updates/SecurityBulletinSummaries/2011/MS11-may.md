---
TOCTitle: 'MS11-MAY'
Title: 'Souhrnný bulletin zabezpečení společnosti Microsoft, květen 2011'
ms:assetid: 'ms11-may'
ms:contentKeyID: 61224014
ms:mtpsurl: 'https://technet.microsoft.com/cs-CZ/library/ms11-may(v=Security.10)'
---

 

Souhrnný bulletin zabezpečení společnosti Microsoft, květen 2011
================================================================

Publikováno: 10. května 2011 | Aktualizováno: 14. června 2011

**Verze:** 1.2

Tento souhrnný bulletin uvádí bulletiny zabezpečení vydané v květnu 2011.

Spolu s vydáním bulletinů pro květen 2011 nahrazuje tento souhrnný bulletin předběžné oznámení o bulletinech vydané 5. května 2011. Další informace o službě předběžného oznámení o bulletinech naleznete v části [Předběžné oznámení o bulletinech zabezpečení společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=217213).

Informace o tom, jak dostávat automatická oznámení o vydání nových bulletinů zabezpečení společnosti Microsoft, naleznete na webu [Zasílání technických oznámení o zabezpečení společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=21163).

Pro zodpovězení zákaznických dotazů týkajících se těchto bulletinů uspořádá společnost Microsoft webové vysílání 11. května 2011 v 11:00 časového pásma Tichomoří (USA a Kanada). [Zaregistrujte se pro webové vysílání týkající se květnových bulletinů zabezpečení](https://msevents.microsoft.com/cui/webcasteventdetails.aspx?culture=en-us&eventid=1032455071&eventcategory=4). Po tomto datu je webové vysílání dostupné na požádání. Další informace získáte v [souhrnných bulletinech zabezpečení společnosti Microsoft a webovém vysílání](http://go.microsoft.com/fwlink/?linkid=217214).

Společnost Microsoft se snaží zákazníkům usnadnit upřednostnění měsíčně vydávaných aktualizací zabezpečení s jakýmikoli aktualizacemi nesouvisejícími se zabezpečením, které jsou vydány ve stejný den jako měsíčně vydávané aktualizace zabezpečení. Další informace získáte v části **Další informace**.

### Informace o bulletinech

Shrnutí
-------

 
Následující tabulka shrnuje podle závažnosti bulletiny zabezpečení pro tento měsíc.

Podrobnosti o softwaru obsahujícím tuto chybu naleznete v následující části **Software obsahující tuto chybu a umístění aktualizací ke stažení**.

 
<p></p>
<table style="border:1px solid black;">
<thead>
<tr class="header">
<th style="border:1px solid black;" >ID bulletinu</th>
<th style="border:1px solid black;" >Název bulletinu a shrnutí</th>
<th style="border:1px solid black;" >Maximální stupeň závažnosti a dopad chyby zabezpečení</th>
<th style="border:1px solid black;" >Požadavek na restartování</th>
<th style="border:1px solid black;" >Postižený software</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=214807">MS11-035</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení služby WINS umožňuje vzdálené spuštění kódu (2524426)</strong><br />
<br />
Tato aktualizace zabezpečení řeší soukromou osobou oznámenou chybu zabezpečení ve službě WINS (Windows Internet Name Service). Tato chyba zabezpečení může umožnit vzdálené spuštění kódu, pokud by uživatel obdržel speciálně vytvořený replikační paket služby WINS v postiženém systému používajícím službu WINS. Ve výchozím nastavení není služba WINS nainstalována v žádném postiženém operačním systému. Tento problém se týká pouze zákazníků, kteří tuto komponentu nainstalovali ručně.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritický</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Může vyžadovat restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217670">MS11-036</a></td>
<td style="border:1px solid black;"><strong>Chyby zabezpečení aplikace Microsoft PowerPoint umožňují vzdálené spuštění kódu (2545814)</strong><br />
<br />
Tato aktualizace zabezpečení řeší dvě soukromými osobami oznámené chyby zabezpečení v aplikaci Microsoft PowerPoint. Chyby umožňují vzdálené spuštění kódu, pokud uživatel otevře speciálně vytvořený soubor aplikace PowerPoint. Útočník, který by úspěšně zneužil některou z těchto chyb zabezpečení, by mohl získat stejná uživatelská práva, jaká má přihlášený uživatel. Uživatelé, jejichž účty jsou konfigurovány tak, aby měli v systému méně uživatelských práv, by byli vystaveni menšímu riziku než uživatelé s uživatelskými právy správce. Instalace a konfigurace funkce Ověření souborů systému Office zamezující otevírání podezřelých souborů blokuje způsoby útoku pokoušející se o zneužití chyb zabezpečení CVE-2011-1269 a CVE-2011-1270.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Vysoký</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Může vyžadovat restartování</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
</tbody>
</table>
<p></p>
  
Index zneužitelnosti  
--------------------
  
 
Následující tabulka uvádí hodnocení zneužitelnosti každé chyby zabezpečení uvedené v tomto měsíci. Chyby zabezpečení jsou řazeny v pořadí zmenšující se úrovně posouzení zneužitelnosti, jinak než tomu je u řazení podle čísla chyb. Uvedeny jsou pouze chyby zabezpečení ohodnocené stupněm závažnosti Kritický nebo Vysoký.
  
**Jak pracovat s touto tabulkou**
  
V této tabulce zjistíte, jaká je pravděpodobnost zneužití v podobě spuštění kódu a odmítnutí služby během 30 dní od vydání tohoto bulletinu zabezpečení pro všechny aktualizace zabezpečení, které bude třeba nainstalovat. Všechna níže uvedená hodnocení zvažte na základě vaší specifické konfigurace a podle závěrů hodnocení nastavte priority pro zavádění jednotlivých aktualizací vydaných v tomto měsíci. Další informace o významu těchto hodnocení a způsobu jejich stanovení najdete v indexu zneužitelnosti [Microsoft Exploitability Index](http://technet.microsoft.com/en-us/security/cc998259.aspx).
  
Položka nazvaná „Nejnovější vydání softwaru“ odkazuje na příslušný software. Položka nazvaná „Starší vydání softwaru“ odkazuje na všechna starší podporovaná vydání příslušného softwaru, uvedeného v tabulkách bulletinu „Software obsahující tuto chybu“ a „Software neobsahující tuto chybu“.
  
| ID bulletinu                                              | Název chyby zabezpečení                                                                                   | ID CVE                                                                           | Hodnocení zneužitelnosti spuštění kódu u nejnovějšího vydání softwaru                                                      | Hodnocení zneužitelnosti spuštění kódu u starších vydání softwaru                                                          | Hodnocení zneužitelnosti odmítnutí služby | Hlavní poznámky |  
|-----------------------------------------------------------|-----------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------|-------------------------------------------|-----------------|  
| [MS11-036](http://go.microsoft.com/fwlink/?linkid=217670) | Chyba zabezpečení týkající se poškození paměti pro prezentaci umožňuje vzdálené spuštění kódu             | [CVE-2011-1269](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1269) | Žádné ohrožení                                                                                                             | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Je pravděpodobné vytvoření kódu konsistentního zneužití   | Netýká se                                 | (Žádné)         |  
| [MS11-035](http://go.microsoft.com/fwlink/?linkid=214807) | Chyba zabezpečení týkající se chybné odezvy služby WINS                                                   | [CVE-2011-1248](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1248) | [2](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Je pravděpodobné vytvoření kódu nekonsistentního zneužití | [2](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Je pravděpodobné vytvoření kódu nekonsistentního zneužití | Dočasné                                   | (Žádné)         |  
| [MS11-036](http://go.microsoft.com/fwlink/?linkid=217670) | Chyba zabezpečení týkající se přetečení vyrovnávací paměti pro prezentaci umožňuje vzdálené spuštění kódu | [CVE-2011-1270](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1270) | Žádné ohrožení                                                                                                             | [3](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Vytvoření kódu funkčního zneužití není pravděpodobné      | Netýká se                                 | (Žádné)         |
  
Software obsahující tuto chybu a umístění aktualizací ke stažení  
----------------------------------------------------------------
  
 
Následující tabulky řadí bulletiny podle kategorie hlavního softwaru a závažnosti.
  
**Jak pracovat s těmito tabulkami?**
  
V těchto tabulkách zjistíte, které aktualizace zabezpečení bude třeba nainstalovat. Přečtěte si seznam všech programů a komponent a zjistěte, zda se některé aktualizace zabezpečení týkají vaší instalace. Pokud se program nebo komponenta v seznamu nachází, je v něm zároveň uveden odkaz na dostupnou aktualizaci softwaru a také stupeň závažnosti aktualizace softwaru.
  
**Poznámka:** Jedna chyba zabezpečení může vyžadovat instalaci více aktualizací. Přečtěte si celý sloupec u každého identifikátoru bulletinu. Zjistíte v něm, které aktualizace je třeba nainstalovat v závislosti na programech nebo součástech nainstalovaných ve vašem systému.
  
#### Operační systém Windows a jeho komponenty

 
<p></p>
<table style="border:1px solid black;">
<tr class="thead">
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
</tr>
<tr>
<th colspan="2" style="border:1px solid black;">
Windows Server 2003  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS11-035**](http://go.microsoft.com/fwlink/?linkid=214807)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Celkový stupeň závažnosti**
</td>
<td style="border:1px solid black;">
[**Kritický**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=0d289146-8470-45dd-a886-d1b35a2c6d4b)  
(Kritický)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=0d3e85a9-42ff-447b-ab8c-095a1c0b224c)  
(Kritický)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 SP2 pro systémy s procesorem Itanium
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=4c388fe8-883a-4118-a7ff-50f1e9d0a071)  
(Kritický)
</td>
</tr>
<tr>
<th colspan="2" style="border:1px solid black;">
Windows Server 2008
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS11-035**](http://go.microsoft.com/fwlink/?linkid=214807)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Celkový stupeň závažnosti**
</td>
<td style="border:1px solid black;">
[**Kritický**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 pro 32bitové systémy a Windows Server 2008 pro 32bitové systémy Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro 32bitové systémy a Windows Server 2008 pro 32bitové systémy Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=9019a3ff-d953-4b0b-8c7a-05aa9cf65c92)\*  
(Kritický)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 pro systémy s procesorem x64 a Windows Server 2008 pro systémy s procesorem x64 Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem x64 a Windows Server 2008 pro systémy s procesorem x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=841130fa-4522-4079-b7eb-f8466ac3ef12)\*  
(Kritický)
</td>
</tr>
<tr>
<th colspan="2" style="border:1px solid black;">
Windows Server 2008 R2
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS11-035**](http://go.microsoft.com/fwlink/?linkid=214807)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Celkový stupeň závažnosti**
</td>
<td style="border:1px solid black;">
[**Kritický**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 pro systémy s procesorem x64 a Windows Server 2008 R2 pro systémy s procesorem x64 Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem x64 a Windows Server 2008 R2 pro systémy s procesorem x64 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=8732b41e-2f25-4ee1-a8b7-a8b8b9e22d08)\*  
(Kritický)
</td>
</tr>
</table>
<p></p>
 
**Poznámka k systémům Windows Server 2008 a Windows Server 2008 R2**

**\*Instalace Server Core obsahující chybu zabezpečení.** Tato aktualizace se stejným hodnocením závažnosti se vztahuje k podporovaným edicím systému Windows Server 2008 nebo Windows Server 2008 R2, jak je uvedeno, s instalací pomocí volby pro instalaci Server Core nebo bez ní. Další informace o této možnosti instalace naleznete v článcích na webu TechNet [Managing a Server Core Installation](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) (Správa instalace Server Core) a [Servicing a Server Core Installation](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx) (Obsluha instalace Server Core). Možnost instalace Server Core se nevztahuje na určité edice systému Windows Server 2008 a Windows Server 2008 R2; další informace naleznete v části [Porovnání možností instalace Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

#### Sady Microsoft Office a jejich software

 
<p></p>
<table style="border:1px solid black;">
<tr class="thead">
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
</tr>
<tr>
<th colspan="2" style="border:1px solid black;">
Sady Microsoft Office a jejich komponenty
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS11-036**](http://go.microsoft.com/fwlink/?linkid=217670)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Celkový stupeň závažnosti**
</td>
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft PowerPoint 2002 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=2e8a30ac-bcfe-4535-8ceb-723c25b43d5f)  
(KB2535802)  
(Vysoký)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2003 Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft PowerPoint 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=fc1cfcac-64cc-484a-97f2-3dcfe84cfdcd)  
(KB2535812)  
(Vysoký)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2007 Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft PowerPoint 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=9a181739-709a-4c0d-a97f-f9891c45c04c)  
(KB2535818)  
(Vysoký)
</td>
</tr>
<tr>
<th colspan="2" style="border:1px solid black;">
Microsoft Office for Mac
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS11-036**](http://go.microsoft.com/fwlink/?linkid=217670)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Celkový stupeň závažnosti**
</td>
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2004 for Mac
</td>
<td style="border:1px solid black;">
Microsoft Office 2004 for Mac<sup>[1]</sup>
(Vysoký)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2008 for Mac
</td>
<td style="border:1px solid black;">
Microsoft Office 2008 for Mac<sup>[1]</sup>
(Vysoký)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Otevření nástroje XML File Format Converter for Mac
</td>
<td style="border:1px solid black;">
Otevření nástroje XML File Format Converter for Mac<sup>[1]</sup>
(Vysoký)
</td>
</tr>
<tr>
<th colspan="2" style="border:1px solid black;">
Jiný software systému Office
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS11-036**](http://go.microsoft.com/fwlink/?linkid=217670)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Celkový stupeň závažnosti**
</td>
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Sada Microsoft Office Compatibility Pack pro formáty souborů aplikací Word, Excel a PowerPoint 2007 Service Pack 2
</td>
<td style="border:1px solid black;">
[Sada Microsoft Office Compatibility Pack pro formáty souborů aplikací Word, Excel a PowerPoint 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5be09069-1cac-4b1e-ac94-4fb7024fb4ac)  
(KB2540162)  
(Vysoký)
</td>
</tr>
</table>
<p></p>
 
**Poznámka k bulletinu MS11-036**

<sup>[1]</sup>Od 14. června 2011 jsou k dispozici aktualizace zabezpečení pro systém Microsoft Office 2004 for Mac (KB2555786), Microsoft Office 2008 for Mac (KB2555785) a nástroj Open XML File Format Converter for Mac (KB2555787). Další informace naleznete v bulletinu.

Nástroje a doporučené postupy zjišťování a nasazení
---------------------------------------------------

 
**Centrum zabezpečení**

Umožňuje správu aktualizací softwaru a zabezpečení, které je třeba nainstalovat na servery, stolní počítače a přenosné počítače v organizaci. Další informace naleznete na webu [TechNet Update Management Center](http://go.microsoft.com/fwlink/?linkid=69903). Další informace o zabezpečení produktů společnosti Microsoft nabízí web [Centrum zabezpečení TechNet](http://go.microsoft.com/fwlink/?linkid=21171). Tyto informace lze také získat kliknutím na nabídku „Nejnovější aktualizace zabezpečení“ na webu [Zabezpečení doma](http://go.microsoft.com/fwlink/?linkid=85102).

Aktualizace zabezpečení jsou k dispozici na webu [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747) a [Windows Update](http://go.microsoft.com/fwlink/?linkid=21130). Aktualizace zabezpečení jsou také k dispozici na webu [služby Stažení softwaru](http://go.microsoft.com/fwlink/?linkid=21129). Nejsnadněji je naleznete hledáním podle klíčových slov aktualizace zabezpečení.

Zákazníkům systému Microsoft Office for Mac doporučujeme využít funkci Microsoft AutoUpdate for Mac, která udržuje software společnosti Microsoft v aktuálním stavu. Další informace o funkci Microsoft AutoUpdate for Mac naleznete na webu [Check for software updates automatically](http://mac2.microsoft.com/help/office/14/en-us/word/item/ffe35357-8f25-4df8-a0a3-c258526c64ea) (Automatická kontrola aktualizací softwaru).

Aktualizace zabezpečení lze stáhnout z katalogu služby [Microsoft Update Catalog](http://go.microsoft.com/fwlink/?linkid=96155). Služba Microsoft Update Catalog poskytuje katalog s možností vyhledávání obsahu dostupného prostřednictvím služeb Windows Update a Microsoft Update, včetně aktualizací zabezpečení, ovladačů a aktualizací Service Pack. Vyhledáváním pomocí čísla bulletinu zabezpečení (například MS07-036) můžete přidat všechny dostupné aktualizace do košíku (včetně různých jazykových verzí aktualizace) a stáhnout je do vybrané složky. Další informace o službě Microsoft Update Catalog najdete v části [Nejčastější dotazy týkající se služby Microsoft Update Catalog](http://go.microsoft.com/fwlink/?linkid=97900).

**Doporučené postupy zjišťování a nasazení**

Společnost Microsoft poskytuje doporučené postupy zjišťování a nasazení aktualizací zabezpečení. Tyto dokumenty obsahují doporučení a informace, které mohou odborníkům v oblasti IT pomoci porozumět, jak se používají různé nástroje pro detekci a nasazení aktualizací zabezpečení. Další informace získáte v [článku 961747 znalostní báze Microsoft Knowledge Base](http://support.microsoft.com/kb/961747).

**Nástroj Microsoft Baseline Security Analyzer**

Pomocí nástroje Microsoft Baseline Security Analyzer (MBSA) mohou správci prohledávat místní i vzdálené systémy a zjistit tak, jestli v nich nechybí některé aktualizace zabezpečení nebo jestli v nastavení zabezpečení systému nedošlo k některým běžným chybám. Další informace o nástroji MBSA získáte na webu [Microsoft Baseline Security Analyzer](http://go.microsoft.com/fwlink/?linkid=21134).

**Služba Windows Server Update Services**

Pomocí služby Windows Server Update Services (WSUS) mohou správci systémů rychle a spolehlivě nasadit nejnovější důležité aktualizace zabezpečení pro systémy Microsoft Windows 2000 a novější, systém Office XP a novější, Exchange Server 2003 a SQL Server 2000 do systémů Microsoft Windows 2000 a novějších.

Další informace o způsobu instalace této aktualizace zabezpečení pomocí služby Windows Server Update Services získáte na webu služby [Windows Server Update Services](http://go.microsoft.com/fwlink/?linkid=50120).

**System Center Configuration Manager 2007**

Služba Software Update Management nástroje Configuration Manager 2007 zjednodušuje složitý proces doručení a správy aktualizací do IT systémů firmy. Pomocí nástroje Configuration Manager 2007 mohou správci informačních technologií doručit aktualizace produktů společnosti Microsoft do řady zařízení, včetně stolních počítačů, notebooků, serverů a mobilních zařízení.

Automatizované hodnocení chyb zabezpečení v nástroji Configuration Manager 2007 odhaluje potřebu aktualizací a hlášení doporučených postupů. Základem služby Software Update Management nástroje Configuration Manager 2007 jsou služby WSUS (Microsoft Windows Software Update Services). Jedná se o časem prověřenou infrastrukturu aktualizací známou správcům informačních technologií po celém světě. Další informace o tom, jak mohou správci používat nástroj Configuration Manager 2007 k nasazení aktualizací, naleznete na webových stránkách [Software Update Management](http://www.microsoft.com/systemcenter/en/us/configuration-manager/cm-software-update-management.aspx). Další informace o nástroji Configuration Manager naleznete na webových stránkách [System Center Configuration Manager](http://www.microsoft.com/systemcenter/en/us/configuration-manager.aspx).

**Systems Management Server 2003**

Microsoft Systems Management Server (SMS) představuje v rozlehlých sítích řešení pro správu aktualizací s rozsáhlými možnostmi konfigurace. Umožňuje správcům identifikovat počítače se systémem Windows, které vyžadují aktualizace zabezpečení, a provést řízenou instalaci těchto aktualizací v celé rozlehlé síti s minimálním dopadem na koncové uživatele.

**Poznámka:** Systems Management Server 2003 není od 12. ledna 2010 součástí tradiční podpory. Další informace o životním cyklu produktů naleznete na webu [Životní cyklus podpory produktů společnosti Microsoft](http://support.microsoft.com/common/international.aspx?rdpath=dm;en-us;lifecycle). K dispozici je nyní nová verze nástroje SMS, System Center Configuration Manager 2007 (viz výše uvedená část **System Center Configuration Manager 2007**).

Další informace o tom, jak mohou správci pomocí serveru SMS 2003 nasazovat aktualizace zabezpečení, naleznete na webových stránkách [Scénáře a postupy pro Microsoft Systems Management Server 2003: Distribuce softwaru a správa oprav](http://www.microsoft.com/downloads/en/details.aspx?familyid=32f2bb4c-42f8-4b8d-844f-2553fd78049f&displaylang=en). Další informace o serveru SMS naleznete na webových stránkách [Microsoft Systems Management Server TechCenter](http://technet.microsoft.com/en-us/systemcenter/bb545936.aspx).

**Poznámka:** Služba SMS pomocí modulu Microsoft Baseline Security Analyzer poskytuje rozsáhlou podporu při zjišťování a nasazení aktualizací bulletinu zabezpečení. Tyto nástroje nemusí některé softwarové aktualizace zjistit. V takovém případě mohou správci použít funkce serveru SMS a nasměrovat aktualizace do určitých systémů. Další informace o tomto postupu najdete na webu [Nasazení aktualizací softwaru pomocí funkce Distribuce softwaru serveru SMS](http://go.microsoft.com/fwlink/?linkid=33341). Některé aktualizace zabezpečení vyžadují po restartování počítače oprávnění správce. Správci mohou k instalaci těchto aktualizací použít nástroj Elevated Rights Deployment Tool (k dispozici v sadě [SMS 2003 Administration Feature Pack](http://www.microsoft.com/downloads/en/details.aspx?familyid=7bd3a16e-1899-4e0b-bb99-1320e816167d&displaylang=en)).

**Nástroj Update Compatibility Evaluator a sada Application Compatibility Toolkit**

Aktualizace často zapisují do stejných souborů a nastavení registru požadovaných pro spouštění aplikací. To může způsobit nekompatibilitu a zvýšit dobu, po kterou trvá nasazení aktualizací zabezpečení. Testování a ověřování aktualizací systému Windows lze usnadnit pomocí součástí nástroje [Update Compatibility Evaluator](http://technet2.microsoft.com/windowsvista/en/library/4279e239-37a4-44aa-aec5-4e70fe39f9de1033.mspx?mfr=true), které jsou dodávány se sadou [Application Compatibility Toolkit](http://www.microsoft.com/downloads/details.aspx?familyid=24da89e9-b581-47b0-b45e-492dd6da2971&displaylang=en).

Sada Application Compatibility Toolkit (ACT) obsahuje nezbytné nástroje a dokumentaci pro posouzení a zmírnění problémů s kompatibilitou aplikací před nasazením systému Microsoft Windows Vista, služby Windows Update, aktualizací zabezpečení společnosti Microsoft nebo nové verze aplikace Windows Internet Explorer ve vašem prostředí.

### Další informace

#### Nástroj pro odstranění škodlivého softwaru systému Microsoft Windows

Společnost Microsoft vydává aktualizovanou verzi Nástroje pro odstranění škodlivého softwaru systému Microsoft Windows na webu Windows Update, Microsoft Update, ve službě Windows Server Update Services a na webu služby Stažení softwaru.

#### Aktualizace nesouvisející se zabezpečením na webu Microsoft Update (MU), Windows Update (WU) a ve službě Windows Server Update Services (WSUS)

Informace o aktualizacích nesouvisejících se zabezpečením na webu Windows Update a Microsoft Update naleznete na webové stránce:

-   [Článek 894199 znalostní báze Microsoft Knowledge Base](http://support.microsoft.com/kb/894199): Popis služeb Software Update Services a Windows Server Update Services se mění v obsahu. Zahrnuje celý obsah systému Windows.
-   [Aktualizace vydané v uplynulých měsících pro službu Windows Server Update Services](http://technet.microsoft.com/en-us/wsus/bb456965.aspx). Obsahuje přehled všech nových, revidovaných a opětovně vydaných aktualizací pro jiné produkty společnosti Microsoft, než je systém Microsoft Windows.

#### Microsoft Active Protections Program (MAPP)

Pro zlepšení ochrany dat svých zákazníků poskytuje společnost Microsoft informace o chybách v zabezpečení všem hlavním dodavatelům softwaru pro zabezpečení, a to vždy ještě před vydáním nové měsíční zprávy o aktualizaci zabezpečení. Dodavatelé softwaru pro zabezpečení tak mohou tyto informace o chybách v zabezpečení využít a poskytnout svým zákazníkům ochranu včasnou aktualizací svých programů a zařízení pro zabezpečení, jako jsou antivirové programy, síťové systémy pro detekci napadení či hostitelské systémy pro prevenci napadení. Informace o dostupnosti aktuálních prostředků aktivní ochrany od jednotlivých dodavatelů softwaru pro zabezpečení naleznete na stránkách aktivní ochrany jednotlivých partnerů programu MAPP. Seznam těchto partnerů naleznete na stránce [Microsoft Active Protections Program (MAPP) Partners](http://go.microsoft.com/fwlink/?linkid=215201).

#### Strategie zabezpečení a komunita

**Strategie instalace aktualizací**

Web [Doporučené postupy zabezpečení pro správu aktualizací (Security Guidance for Update Management)](http://go.microsoft.com/fwlink/?linkid=21168) obsahuje další informace o instalaci aktualizací zabezpečení podle doporučení společnosti Microsoft.

**Získání dalších aktualizací zabezpečení**

Aktualizace odstraňující další problémy se zabezpečením získáte v následujících umístěních:

-   Aktualizace zabezpečení jsou k dispozici na webu služby [Stažení softwaru (Microsoft Download Center)](http://go.microsoft.com/fwlink/?linkid=21129). Nejsnadněji je naleznete hledáním podle klíčových slov aktualizace zabezpečení.
-   Aktualizace pro klientské platformy jsou k dispozici na webu [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747).
-   Aktualizace zabezpečení nabízené tento měsíc na webu Windows Update jsou k dispozici na webu služby Stažení softwaru v souborech obrazu ISO disku CD s vydanými aktualizacemi zabezpečení a kritickými aktualizacemi. Další informace získáte v [článku 913086 znalostní báze Microsoft Knowledge Base](http://support.microsoft.com/kb/913086).

**Komunita odborníků v oblasti zabezpečení**

Můžete se zde naučit, jak zlepšit zabezpečení a jak optimalizovat infrastrukturu IT. Také můžete s dalšími členy komunity IT Pro diskutovat o bezpečnostních tématech na webu [Komunita odborníků v oblasti zabezpečení (IT Pro Security Community)](http://go.microsoft.com/fwlink/?linkid=21164).

#### Poděkování

Společnost Microsoft tímto [děkuje](http://go.microsoft.com/fwlink/?linkid=21127) za spolupráci při ochraně zákazníků:

-   Luigimu Auriemmovi, spolupracujícímu s organizací [Zero Day Initiative](http://www.zerodayinitiative.com/) společnosti [TippingPoint](http://www.tippingpoint.com/), za oznámení chyby popsané v bulletinu MS11-035.
-   Willu Dormannovi z centra [CERT/CC](http://www.cert.org/) za spolupráci na řešení dvou chyb popsaných v bulletinu MS11-036.

#### Technická podpora

-   Uvedený software byl testován za účelem zjištění, kterých verzí se chyba týká. U dalších verzí skončila časově omezená podpora. Pokud chcete zjistit dobu, po kterou je pro určitou verzi softwaru poskytována podpora, navštivte web [Zásady poskytování technické podpory pro produkty společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=21742).
-   Zákazníci mohou získat technickou podporu na webu [služby technické podpory společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=21131). Hovory související s aktualizacemi zabezpečení jsou bezplatné. Další informace o dostupných možnostech technické podpory naleznete na webu [Pomoc a podpora společnosti Microsoft](http://support.microsoft.com/).
-   Mezinárodní zákazníci získají podporu u místních zastoupení společnosti Microsoft. Technická podpora související s aktualizacemi zabezpečení je bezplatná. Další informace o možnostech kontaktování společnosti Microsoft v případě potřeby technické podpory získáte na [webu mezinárodní technické podpory](http://go.microsoft.com/fwlink/?linkid=21155).

#### Zřeknutí se záruky

Informace ve znalostní bázi Microsoft Knowledge Base jsou poskytovány tak, jak jsou, bez jakékoli záruky. Společnost Microsoft neposkytuje žádné záruky, výslovně uvedené či mlčky předpokládané, včetně záruk obchodovatelnosti a vhodnosti pro určitý účel. Společnost Microsoft ani její dodavatelé nenesou v žádném případě zodpovědnost za žádné škody, včetně přímých, nepřímých, náhodných či následných škod, ztráty zisku či zvláštních škod, a to ani v případě, že byli na možnost takových škod upozorněni. V některých zemích a právních řádech není dovoleno vyloučit nebo omezit odpovědnost, proto se výše uvedené omezení na vás nemusí vztahovat.

#### Revize

-   V1.0 (10. května 2011): Souhrnný bulletin byl publikován.
-   V1.1 (17. května 2011): Z tabulky Software obsahující tuto chybu byla odstraněna chybná poznámka k bulletinu MS11-036 týkající se aktualizací zabezpečení KB2535818 a KB2540162 pro aplikaci Microsoft PowerPoint 2007 Service Pack 2.
-   V1.2 (14. června 2011): Do tohoto souhrnného bulletinu byla přidána informace pro bulletin MS11-036, že jsou k dispozici aktualizace zabezpečení pro systém Microsoft Office 2004 for Mac (KB2555786), Microsoft Office 2008 for Mac (KB2555785) a nástroj Open XML File Format Converter for Mac (KB2555787). Další informace naleznete v bulletinu MS11-036.

*Built at 2014-04-18T01:50:00Z-07:00*
