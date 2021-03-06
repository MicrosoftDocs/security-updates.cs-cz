---
TOCTitle: 'MS09-NOV'
Title: 'Souhrnný bulletin zabezpečení společnosti Microsoft, listopad 2009'
ms:assetid: 'ms09-nov'
ms:contentKeyID: 61223991
ms:mtpsurl: 'https://technet.microsoft.com/cs-CZ/library/ms09-nov(v=Security.10)'
---

 

Souhrnný bulletin zabezpečení společnosti Microsoft, listopad 2009
==================================================================

Publikováno: 10. listopadu 2009 | Aktualizováno: 25. listopadu 2009

**Verze:** 1.1

Tento souhrnný bulletin uvádí bulletiny zabezpečení vydané v listopadu 2009.

Spolu s vydáním bulletinů pro listopad 2009 nahrazuje tento souhrnný bulletin předběžné oznámení o bulletinech vydané 5. listopadu 2009. Další informace o službě předběžného oznámení o bulletinech naleznete v části [Předběžné oznámení o bulletinech zabezpečení společnosti Microsoft](http://technet.microsoft.com/security/bulletin/advance).

Informace o tom, jak dostávat automatická oznámení o vydání nových bulletinů zabezpečení společnosti Microsoft, naleznete na webu [Zasílání technických oznámení o zabezpečení společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=21163).

Pro zodpovězení zákaznických dotazů týkajících se těchto bulletinů uspořádá společnost Microsoft webové vysílání 11. listopadu 2009 v 11:00 časového pásma Tichomoří (USA a Kanada). [Registrovat se pro webové vysílání týkající se listopadových bulletinů zabezpečení](http://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032407490&culture=en-us). Po tomto datu je webové vysílání dostupné na požádání. Další informace získáte v [souhrnných bulletinech zabezpečení společnosti Microsoft a webovém vysílání](http://technet.microsoft.com/security/bulletin/summary).

Společnost Microsoft se snaží zákazníkům usnadnit upřednostnění měsíčně vydávaných aktualizací zabezpečení před jakýmikoli důležitými aktualizacemi nesouvisejícími se zabezpečením, které jsou vydány ve stejný den jako měsíčně vydávané aktualizace zabezpečení. Další informace získáte v části **Další informace**.

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
<th style="border:1px solid black;" >Software obsahující tuto chybu</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=163840">MS09-063</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení webových služeb v rozhraní API zařízení umožňuje vzdálené spuštění kódu (973565)</strong><br />
<br />
Tato aktualizace zabezpečení řeší soukromou osobou oznámenou chybu zabezpečení webových služeb v rozhraní API zařízení (WSDAPI) v operačním systému Windows. Chyba zabezpečení by mohla umožnit vzdálené spuštění kódu, pokud systém Windows obsahující tuto chybu obdrží speciálně vytvořený paket. Jen útočníci v této místní podsíti by mohli zneužít tuto chybu.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritický</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=163841">MS09-064</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení serveru se službou protokolování licence umožňuje vzdálené spuštění kódu (974783)</strong><br />
<br />
Tato aktualizace zabezpečení řeší chybu zabezpečení v systému Microsoft Windows 2000 oznámenou soukromou osobou. Chyba zabezpečení by mohla umožnit vzdálené spuštění kódu, pokud by útočník odeslal speciálně vytvořenou síťovou zprávu do počítače obsahující server se službou protokolování licence. Útočník, který by tuto chybu zabezpečení zneužil, by mohl získat úplnou kontrolu nad systémem. Doporučené postupy pro používání brány firewall a standardní konfigurace této brány zajišťují ochranu sítí před útoky pocházejícími z oblasti mimo rozlehlou síť.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritický</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=162428">MS09-065</a></td>
<td style="border:1px solid black;"><strong>Chyby zabezpečení v ovladačích režimu jádra systému Windows umožňují vzdálené spuštění kódu (969947)</strong><br />
<br />
Tato aktualizace zabezpečení řeší několik chyb zabezpečení jádra systému Windows oznámených soukromými osobami. Nejzávažnější z těchto chyb zabezpečení by mohla způsobit vzdálené spuštění kódu v případě, že by uživatel zobrazil obsah ve speciálně vytvořeném písmu EOT (Embedded OpenType). V případě útoku z webu by útočník musel být hostitelem webu, který obsahuje speciálně vytvořená vložená písma, jejichž pomocí lze tuto chybu zabezpečení zneužít. Navíc, dané weby a weby, které přijímají nebo hostují materiál poskytovaný uživateli, by mohly obsahovat speciálně vytvořený obsah zneužívající tuto chybu zabezpečení. Útočník nemůže žádným způsobem přinutit uživatele k návštěvě speciálně vytvořené webové stránky. Namísto toho by útočník musel uživatele přesvědčit, aby navštívili takový web. K tomu se obvykle používá odkaz v e-mailové zprávě nebo zprávě programu pro zasílání rychlých zpráv, na který uživatelé kliknou, a přejdou tak na útočníkův web.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritický</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=157862">MS09-066</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení služby Active Directory může způsobit odmítnutí služby (973309)</strong><br />
<br />
Tato aktualizace zabezpečení řeší soukromou osobou oznámenou chybu zabezpečení v adresářové službě Active Directory, režimu ADAM (Active Directory Application Mode) a adresářové službě AD LDS (Active Directory Lightweight Directory Service). Chyba zabezpečení může způsobit odmítnutí služby, pokud byl prostor zásobníku vyčerpán během vyřizování určitého typu požadavků LDAP nebo LDAPS. Tato chyba zabezpečení se vztahuje pouze na řadiče domény a systémy konfigurované tak, aby v nich probíhala služba ADAM nebo AD LDS.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Důležité</a><br />
Odmítnutí služby</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=165431">MS09-067</a></td>
<td style="border:1px solid black;"><strong>Chyby zabezpečení v aplikaci Microsoft Office Excel umožňují vzdálené spuštění kódu (972652)</strong><br />
<br />
Tato aktualizace zabezpečení řeší několik chyb zabezpečení v aplikaci Microsoft Office Excel oznámených soukromými osobami. Chyby umožňují vzdálené spuštění kódu, pokud uživatel otevře speciálně vytvořený soubor aplikace Excel. Útočník, který by úspěšně zneužil některou z těchto chyb zabezpečení, by mohl získat stejná uživatelská práva, jaká má místní uživatel. Uživatelé, jejichž účty jsou konfigurovány tak, aby měli v systému méně uživatelských práv, by byli vystaveni menšímu riziku než uživatelé s uživatelskými právy správce.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Důležité</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Může vyžadovat restartování</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=165890">MS09-068</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení v aplikaci Microsoft Office Word umožňuje vzdálené spuštění kódu (976307)</strong><br />
<br />
Tato aktualizace zabezpečení řeší soukromými osobami oznámenou chybu zabezpečení, která by mohla umožnit vzdálené spuštění kódu v případě, že uživatel otevře speciálně vytvořený soubor aplikace Word. Útočník, který by tuto chybu zabezpečení zneužil, by mohl získat úplnou kontrolu nad postiženým systémem. Útočník by tak mohl instalovat programy, zobrazovat, měnit či odstraňovat data nebo vytvářet nové účty s úplnými uživatelskými právy. Uživatelé, jejichž účty jsou konfigurovány tak, aby měli v systému méně uživatelských práv, by byli vystaveni menšímu riziku než uživatelé s uživatelskými právy správce.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Důležité</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Může vyžadovat restartování</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
</tbody>
</table>
<p></p>
  
Index zneužitelnosti  
--------------------
  

Následující tabulka uvádí hodnocení zneužitelnosti každé chyby zabezpečení uvedené v tomto měsíci. Chyby zabezpečení jsou řazeny podle čísla jednotlivých bulletinů (ID bulletinu) a chyb (ID CVE).
  
**Jak pracovat s touto tabulkou**
  
V této tabulce zjistíte, jaká je pravděpodobnost vydání funkčního zneužitelného kódu během 30 dní od vydání tohoto bulletinu zabezpečení pro všechny aktualizace zabezpečení, které bude třeba nainstalovat. Všechna níže uvedená hodnocení zvažte na základě vaší specifické konfigurace a podle závěrů hodnocení nastavte priority pro zavádění jednotlivých aktualizací. Další informace o významu těchto hodnocení a způsobu jejich stanovení najdete v indexu zneužitelnosti [Microsoft Exploitability Index](http://technet.microsoft.com/en-us/security/cc998259.aspx).
  
| ID bulletinu                                              | Název chyby zabezpečení                                                                                 | ID CVE                                                                           | Hodnocení indexu zneužitelnosti                                                                                                | Hlavní poznámky                                                                                                               |  
|-----------------------------------------------------------|---------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------|  
| [MS09-063](http://go.microsoft.com/fwlink/?linkid=163840) | Chyba zabezpečení webových služeb v rozhraní API zařízení týkající se poškození paměti                  | [CVE-2009-2512](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2512) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Nekonsistentní kód zneužití je pravděpodobný              | Scénář umožňuje útok vedoucí k omezenému odmítnutí služby.                                                                    |  
| [MS09-064](http://go.microsoft.com/fwlink/?linkid=163841) | Chyba zabezpečení serveruse službou protokolování licence týkající se přetečení haldy                   | [CVE-2009-2523](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2523) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Nekonsistentní kód zneužití je pravděpodobný              | Útok závisí na konfliktu časování, jehož zneužití je obtížné. Jakákoli jiná zneužití než odmítnutí služby jsou nedůvěryhodná. |  
| [MS09-065](http://go.microsoft.com/fwlink/?linkid=162428) | Chyba zabezpečení týkající se vyhodnocování ukazatele Win32k NULL                                       | [CVE-2009-1127](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1127) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Nekonsistentní kód zneužití je pravděpodobný              | (Žádné)                                                                                                                       |  
| [MS09-065](http://go.microsoft.com/fwlink/?linkid=162428) | Chyba zabezpečení týkající se nedostatečného ověřování dat Win32k                                       | [CVE-2009-2513](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2513) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní kód zneužití je pravděpodobný                | (Žádné)                                                                                                                       |  
| [MS09-065](http://go.microsoft.com/fwlink/?linkid=162428) | Chyba zabezpečení týkající se analýzy Win32k EOT                                                        | [CVE-2009-2514](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2514) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní kód zneužití je pravděpodobný                | (Žádné)                                                                                                                       |  
| [MS09-066](http://go.microsoft.com/fwlink/?linkid=157862) | Chyba zabezpečení týkající se rekurzivního přetečení zásobníku LSASS                                    | [CVE-2009-1928](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1928) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Vytvoření funkčního zneužitelného kódu není pravděpodobné | Existuje podmínka pro odmítnutí služby.                                                                                       |  
| [MS09-067](http://go.microsoft.com/fwlink/?linkid=165431) | Chyba zabezpečení týkající se poškození mezipaměti aplikace Excel                                       | [CVE-2009-3127](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-3127) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Nekonsistentní kód zneužití je pravděpodobný              | (Žádné)                                                                                                                       |  
| [MS09-067](http://go.microsoft.com/fwlink/?linkid=165431) | Chyba zabezpečení týkající se poškození paměti systému SxView aplikace Excel                            | [CVE-2009-3128](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-3128) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Nekonsistentní kód zneužití je pravděpodobný              | (Žádné)                                                                                                                       |  
| [MS09-067](http://go.microsoft.com/fwlink/?linkid=165431) | Chyba zabezpečení týkající se poškození paměti záhlaví sdílené funkce (Featheader) aplikace Excel       | [CVE-2009-3129](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-3129) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní kód zneužití je pravděpodobný                | (Žádné)                                                                                                                       |  
| [MS09-067](http://go.microsoft.com/fwlink/?linkid=165431) | Chyba zabezpečení týkající se přetečení haldy při analýze dokumentů aplikace Excel                      | [CVE-2009-3130](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-3130) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní kód zneužití je pravděpodobný                | (Žádné)                                                                                                                       |  
| [MS09-067](http://go.microsoft.com/fwlink/?linkid=165431) | Chyba zabezpečení týkající se poškození paměti při analýze vzorců aplikace Excel                        | [CVE-2009-3131](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-3131) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní kód zneužití je pravděpodobný                | (Žádné)                                                                                                                       |  
| [MS09-067](http://go.microsoft.com/fwlink/?linkid=165431) | Chyba zabezpečení týkající se analýzy indexu aplikace Excel                                             | [CVE-2009-3132](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-3132) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Nekonsistentní kód zneužití je pravděpodobný              | (Žádné)                                                                                                                       |  
| [MS09-067](http://go.microsoft.com/fwlink/?linkid=165431) | Chyba zabezpečení týkající se poškození paměti při analýze dokumentů aplikace Excel                     | [CVE-2009-3133](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-3133) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Nekonsistentní kód zneužití je pravděpodobný              | (Žádné)                                                                                                                       |  
| [MS09-067](http://go.microsoft.com/fwlink/?linkid=165431) | Chyba zabezpečení týkající se vyčištění pole aplikace Excel                                             | [CVE-2009-3134](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-3134) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Nekonsistentní kód zneužití je pravděpodobný              | (Žádné)                                                                                                                       |  
| [MS09-068](http://go.microsoft.com/fwlink/?linkid=165890) | Chyba zabezpečení týkající se poškození paměti v informacích o souborech aplikace Microsoft Office Word | [CVE-2009-3135](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-3135) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní kód zneužití je pravděpodobný                | (Žádné)                                                                                                                       |
  
Software obsahující tuto chybu a umístění aktualizací ke stažení  
----------------------------------------------------------------
  

Následující tabulky řadí bulletiny podle kategorie hlavního softwaru a závažnosti.
  
**Jak pracovat s těmito tabulkami?**
  
V těchto tabulkách zjistíte, které aktualizace zabezpečení bude třeba nainstalovat. Přečtěte si seznam všech programů a komponent a zjistěte, zda se některé aktualizace zabezpečení týkají vaší instalace. Pokud se program nebo komponenta v seznamu nachází, je v něm zároveň uveden odkaz na dostupnou aktualizaci softwaru a také stupeň závažnosti aktualizace softwaru.
  
**Poznámka:** Jedna chyba zabezpečení může vyžadovat instalaci více aktualizací. Přečtěte si celý sloupec u každého identifikátoru bulletinu. Zjistíte v něm, které aktualizace nainstalovat v závislosti na programech nebo součástech nainstalovaných ve vašem systému.
  
#### Operační systém Windows a jeho komponenty

 
<p></p>
<table style="border:1px solid black;">
<tr class="thead">
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
</tr>
<tr>
<th colspan="5" style="border:1px solid black;">
Microsoft Windows 2000  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS09-063**](http://go.microsoft.com/fwlink/?linkid=163840)
</td>
<td style="border:1px solid black;">
[**MS09-064**](http://go.microsoft.com/fwlink/?linkid=163841)
</td>
<td style="border:1px solid black;">
[**MS09-065**](http://go.microsoft.com/fwlink/?linkid=162428)
</td>
<td style="border:1px solid black;">
[**MS09-066**](http://go.microsoft.com/fwlink/?linkid=157862)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Celkový stupeň závažnosti**
</td>
<td style="border:1px solid black;">
Žádné
</td>
<td style="border:1px solid black;">
[**Kritický**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritický**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Windows 2000 Service Pack 4
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Server Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=365a8dff-2383-42f6-b567-e545461fd135)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=45db8bb1-c81b-4d3f-a658-74f5fa445f81)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Služba Active Directory v systému Microsoft Windows 2000 Server Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=297158cf-374c-45d9-b213-978e1f54d244)  
(KB973037)  
(Důležitý)
</td>
</tr>
<tr>
<th colspan="5" style="border:1px solid black;">
Windows XP
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS09-063**](http://go.microsoft.com/fwlink/?linkid=163840)
</td>
<td style="border:1px solid black;">
[**MS09-064**](http://go.microsoft.com/fwlink/?linkid=163841)
</td>
<td style="border:1px solid black;">
[**MS09-065**](http://go.microsoft.com/fwlink/?linkid=162428)
</td>
<td style="border:1px solid black;">
[**MS09-066**](http://go.microsoft.com/fwlink/?linkid=157862)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Celkový stupeň závažnosti**
</td>
<td style="border:1px solid black;">
Žádné
</td>
<td style="border:1px solid black;">
Žádné
</td>
<td style="border:1px solid black;">
[**Kritický**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Service Pack 2 a Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 a Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=916abdad-44b7-4f9d-986a-0c3558fb8e06)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Služba ADAM (Active Directory Application Mode)](http://www.microsoft.com/downloads/details.aspx?familyid=cbe09780-f288-457a-b254-58c9c8744055)  
(KB973039)  
(Důležitý)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=1d0464c6-5ed8-4064-887e-618a2db09236)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Služba ADAM (Active Directory Application Mode)](http://www.microsoft.com/downloads/details.aspx?familyid=b65ddf36-a02d-4aa2-9b4f-7416dbf59e2a)  
(KB973039)  
(Důležitý)
</td>
</tr>
<tr>
<th colspan="5" style="border:1px solid black;">
Windows Server 2003
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS09-063**](http://go.microsoft.com/fwlink/?linkid=163840)
</td>
<td style="border:1px solid black;">
[**MS09-064**](http://go.microsoft.com/fwlink/?linkid=163841)
</td>
<td style="border:1px solid black;">
[**MS09-065**](http://go.microsoft.com/fwlink/?linkid=162428)
</td>
<td style="border:1px solid black;">
[**MS09-066**](http://go.microsoft.com/fwlink/?linkid=157862)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Celkový stupeň závažnosti**
</td>
<td style="border:1px solid black;">
Žádné
</td>
<td style="border:1px solid black;">
Žádné
</td>
<td style="border:1px solid black;">
[**Kritický**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5cd62750-e269-44ae-8c7c-c335e8545b9a)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Active Directory](http://www.microsoft.com/downloads/details.aspx?familyid=28f1c494-4e16-43b6-93d2-49e15f142ac9)  
(KB973037)  
(Důležitý)  
[Služba ADAM (Active Directory Application Mode)](http://www.microsoft.com/downloads/details.aspx?familyid=44cb9029-4b19-4bad-8fc9-3efe285adb0e)  
(KB973039)  
(Důležitý)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=04a7f817-f330-4003-8b25-d3e744905b12)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Active Directory](http://www.microsoft.com/downloads/details.aspx?familyid=509aeec0-112b-44ab-8686-43f381b61940)  
(KB973037)  
(Důležitý)  
[Služba ADAM (Active Directory Application Mode)](http://www.microsoft.com/downloads/details.aspx?familyid=87f2109e-5129-467c-930f-70af31ebf5de)  
(KB973039)  
(Důležitý)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 SP2 pro systémy s procesorem Itanium
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=b95daac0-4c99-47a4-b0ca-9429997ea3d9)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Active Directory](http://www.microsoft.com/downloads/details.aspx?familyid=040e691b-1ef0-4b73-bef7-a1d77b84b0ca)  
(KB973037)  
(Důležitý)
</td>
</tr>
<tr>
<th colspan="5" style="border:1px solid black;">
Windows Vista
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS09-063**](http://go.microsoft.com/fwlink/?linkid=163840)
</td>
<td style="border:1px solid black;">
[**MS09-064**](http://go.microsoft.com/fwlink/?linkid=163841)
</td>
<td style="border:1px solid black;">
[**MS09-065**](http://go.microsoft.com/fwlink/?linkid=162428)
</td>
<td style="border:1px solid black;">
[**MS09-066**](http://go.microsoft.com/fwlink/?linkid=157862)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Celkový stupeň závažnosti**
</td>
<td style="border:1px solid black;">
[**Kritický**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Žádné
</td>
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Žádné
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista, Windows Vista Service Pack 1 a Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Vista, Windows Vista Service Pack 1 a Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ebf0c294-cd99-445a-a741-78253e47189f)  
(Kritický)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Vista, Windows Vista Service Pack 1 a Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=54562103-1d99-42d7-8f7f-c0cbcdce90db)  
(Důležitý)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 a Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 a Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d9645fc9-f524-43f1-8b8c-94b3b4312158)  
(Kritický)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 a Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=fcb87cc8-6fd7-4f16-93d6-552999462fb1)  
(Důležitý)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
</tr>
<tr>
<th colspan="5" style="border:1px solid black;">
Windows Server 2008
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS09-063**](http://go.microsoft.com/fwlink/?linkid=163840)
</td>
<td style="border:1px solid black;">
[**MS09-064**](http://go.microsoft.com/fwlink/?linkid=163841)
</td>
<td style="border:1px solid black;">
[**MS09-065**](http://go.microsoft.com/fwlink/?linkid=162428)
</td>
<td style="border:1px solid black;">
[**MS09-066**](http://go.microsoft.com/fwlink/?linkid=157862)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Celkový stupeň závažnosti**
</td>
<td style="border:1px solid black;">
[**Kritický**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Žádné
</td>
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 pro 32bitové systémy a Windows Server 2008 pro 32bitové systémy Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro 32bitové systémy a Windows Server 2008 pro 32bitové systémy Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d6a60883-b103-459a-a91b-cd6ed946cefe)\*  
(Kritický)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro 32bitové systémy a Windows Server 2008 pro 32bitové systémy Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b97d48de-0f6d-4bca-b990-acf543fdb8b7)\*  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Active Directory a Active Directory Lightweight Directory Service (AD LDS)](http://www.microsoft.com/downloads/details.aspx?familyid=701abf15-7f93-41de-8d09-13404fd79a7e)\*  
(KB973037)  
(Důležitý)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 pro systémy s procesorem x64 a Windows Server 2008 pro systémy s procesorem x64 Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem x64 a Windows Server 2008 pro systémy s procesorem x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3dde1587-42d3-438f-8344-696a5657b9b1)\*  
(Kritický)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem x64 a Windows Server 2008 pro systémy s procesorem x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=0e2b8607-10fa-406a-96a5-18290f479c48)\*  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Active Directory a Active Directory Lightweight Directory Service (AD LDS)](http://www.microsoft.com/downloads/details.aspx?familyid=17f5f9e0-5869-41da-9b3b-6e67540af1f0)\*  
(KB973037)  
(Důležitý)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 pro systémy s procesorem Itanium a Windows Server 2008 pro systémy s procesorem Itanium Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem Itanium a Windows Server 2008 pro systémy s procesorem Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=841a027f-22fa-42de-93b3-57a3fe92a1d3)  
(Kritický)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem Itanium a Windows Server 2008 pro systémy s procesorem Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=28eba3f3-99a5-424c-bc8d-a718c716699e)  
(Důležitý)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
</tr>
</table>
<p></p>
 
**Poznámka k systémům Windows Server 2008 a Windows Server 2008 R2**

**\*Instalace Server Core obsahující chybu zabezpečení.** Tato aktualizace se stejným hodnocením závažnosti se vztahuje k podporovaným edicím systému Windows Server 2008 nebo Windows Server 2008 R2, jak je uvedeno, s instalací pomocí volby pro instalaci Server Core nebo bez ní. Další informace o této možnosti instalace naleznete v článcích na webu služby MSDN, [Server Core](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx) a [Server Core for Windows Server 2008 R2](http://msdn.microsoft.com/en-us/library/ee391631(vs.85).aspx). Možnost instalace Server Core se nevztahuje na určité edice systému Windows Server 2008 a Windows Server 2008 R2; další informace naleznete v části [Porovnání možností instalace Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

#### Sady Microsoft Office a jejich software

 
<p></p>
<table style="border:1px solid black;">
<tr class="thead">
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
</tr>
<tr>
<th colspan="3" style="border:1px solid black;">
Sady Microsoft Office, systémy a komponenty
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS09-067**](http://go.microsoft.com/fwlink/?linkid=165431)
</td>
<td style="border:1px solid black;">
[**MS09-068**](http://go.microsoft.com/fwlink/?linkid=165890)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Celkový stupeň závažnosti**
</td>
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office XP
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel 2002 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=5672c8fc-8509-4962-ad86-ebc0f2575043)  
(KB973471)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Microsoft Office Word 2002 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=0369fae5-958b-4eba-83a4-9c07e701c273)  
(KB973444)  
(Důležitý)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2003
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=6a6a0f5d-17dc-4a34-b9a0-0774aa287ba5)  
(KB973475)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Microsoft Office Word 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=6b77bc62-bcbb-4b9a-97d1-a49ca0582e54)  
(KB973443)  
(Důležitý)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Systém Microsoft Office 2007
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel 2007 Service Pack 1 a Microsoft Office Excel 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=322b24ca-aff6-4ca0-acf1-440cae0f9693)<sup>[1]</sup>
(KB973593)  
(Důležitý)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
</tr>
<tr>
<th colspan="3" style="border:1px solid black;">
Microsoft Office for Mac
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS09-067**](http://go.microsoft.com/fwlink/?linkid=165431)
</td>
<td style="border:1px solid black;">
[**MS09-068**](http://go.microsoft.com/fwlink/?linkid=165890)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Celkový stupeň závažnosti**
</td>
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
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
[Microsoft Office 2004 for Mac](http://www.microsoft.com/downloads/details.aspx?familyid=8f115b1c-1e28-4ecf-937c-99c4b60c7c8e)  
(KB976830)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2004 for Mac](http://www.microsoft.com/downloads/details.aspx?familyid=8f115b1c-1e28-4ecf-937c-99c4b60c7c8e)  
(KB976830)  
(Důležitý)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2008 for Mac
</td>
<td style="border:1px solid black;">
[Microsoft Office 2008 for Mac](http://www.microsoft.com/downloads/details.aspx?familyid=b84fe57d-ddda-451e-9ead-69e10aee7928)  
(KB976828)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2008 for Mac](http://www.microsoft.com/downloads/details.aspx?familyid=b84fe57d-ddda-451e-9ead-69e10aee7928)  
(KB976828)  
(Důležitý)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Otevření nástroje XML File Format Converter for Mac
</td>
<td style="border:1px solid black;">
[Otevření nástroje XML File Format Converter for Mac](http://www.microsoft.com/downloads/details.aspx?familyid=4dd4bc05-1217-497e-8f65-4347f2544ed6)  
(KB976831)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Otevření nástroje XML File Format Converter for Mac](http://www.microsoft.com/downloads/details.aspx?familyid=4dd4bc05-1217-497e-8f65-4347f2544ed6)  
(KB976831)  
(Důležitý)
</td>
</tr>
<tr>
<th colspan="3" style="border:1px solid black;">
Další software sady Microsoft Office
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS09-067**](http://go.microsoft.com/fwlink/?linkid=165431)
</td>
<td style="border:1px solid black;">
[**MS09-068**](http://go.microsoft.com/fwlink/?linkid=165890)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Celkový stupeň závažnosti**
</td>
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Excel Viewer 2003
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel Viewer 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=19151e22-5642-456c-bd39-298574369cdb)  
(KB973484)  
(Důležitý)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office Excel Viewer
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel Viewer Service Pack 1 a Microsoft Office Excel Viewer Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=fb36df5e-ebef-46bf-9edd-67f2c76dbdb3)  
(KB973707)  
(Důležitý)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Word Viewer 2003
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Microsoft Office Word Viewer 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=4cc5e6c5-7efb-4180-9a9b-0788115c91e1)  
(KB973866)  
(Důležitý)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office Word Viewer
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Microsoft Office Word Viewer](http://www.microsoft.com/downloads/details.aspx?familyid=4cc5e6c5-7efb-4180-9a9b-0788115c91e1)  
(KB973866)  
(Důležitý)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Sada Microsoft Office Compatibility Pack pro formáty souborů aplikací Word, Excel a PowerPoint 2007
</td>
<td style="border:1px solid black;">
[Sada Microsoft Office Compatibility Pack pro formáty souborů aplikací Word, Excel a PowerPoint 2007 Service Pack 1 a sada Microsoft Office Compatibility Pack pro formáty souborů aplikací Word, Excel a PowerPoint 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c4c92d2e-e87d-446f-8d3e-8f4be10c70aa)  
(KB973704)  
(Důležitý)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
</tr>
</table>
<p></p>
 
**Poznámka k bulletinu MS09-067**

<sup>[1]</sup>Chtějí-li se zákazníci používající aplikaci Microsoft Office Excel 2007 Service Pack 1 či Microsoft Office Excel 2007 Service Pack 2 chránit před chybami zabezpečení popsanými v tomto bulletinu, je nutné, aby si vedle aktualizace uvedené v článku KB973593 znalostní báze nainstalovali také aktualizaci zabezpečení pro sadu [Microsoft Office Compatibility Pack pro formáty souborů aplikací Word, Excel a PowerPoint 2007 Service Pack 1 a Microsoft Office Compatibility Pack pro formáty souborů aplikací Word, Excel a PowerPoint 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c4c92d2e-e87d-446f-8d3e-8f4be10c70aa) (KB973704).

Nástroje a doporučené postupy zjišťování a nasazení
---------------------------------------------------


**Centrum zabezpečení**

Umožňuje správu aktualizací softwaru a zabezpečení, které je třeba nainstalovat na servery, stolní počítače a přenosné počítače v organizaci. Další informace naleznete na webu [TechNet Update Management Center](http://go.microsoft.com/fwlink/?linkid=69903). Další informace o zabezpečení produktů společnosti Microsoft nabízí web [Centrum zabezpečení TechNet](http://go.microsoft.com/fwlink/?linkid=21171). Tyto informace lze také získat kliknutím na nabídku „Nejnovější aktualizace zabezpečení“ na webu [Zabezpečení doma](http://go.microsoft.com/fwlink/?linkid=85102).

Aktualizace zabezpečení jsou k dispozici na webu [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747) a [Windows Update](http://go.microsoft.com/fwlink/?linkid=21130). Aktualizace zabezpečení jsou také k dispozici na webu [služby Stažení softwaru](http://go.microsoft.com/fwlink/?linkid=21129). Nejsnadněji je naleznete hledáním podle klíčových slov aktualizace zabezpečení.

Aktualizace zabezpečení lze stáhnout z katalogu služby [Microsoft Update Catalog](http://go.microsoft.com/fwlink/?linkid=96155). Služba Microsoft Update Catalog poskytuje katalog s možností vyhledávání obsahu dostupného prostřednictvím služeb Windows Update a Microsoft Update, včetně aktualizací zabezpečení, ovladačů a aktualizací Service Pack. Vyhledáváním pomocí čísla bulletinu zabezpečení (například MS07-036) můžete přidat všechny dostupné aktualizace do košíku (včetně různých jazykových verzí aktualizace) a stáhnout je do vybrané složky. Další informace o službě Microsoft Update Catalog najdete v části [Nejčastější dotazy týkající se služby Microsoft Update Catalog](http://go.microsoft.com/fwlink/?linkid=97900).

**Poznámka:** K 1. srpnu 2009 ukončí společnost Microsoft podporu webu Office Update a nástroje Office Update Inventory Tool. Nejnovější aktualizace produktů Microsoft Office bude přinášet web [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747). Další informace naleznete v části [O webu Microsoft Office Update: Nejčastější dotazy](http://office.microsoft.com/en-us/downloads/fx010402221033.aspx).

**Doporučené postupy zjišťování a instalace**

Společnost Microsoft poskytuje doporučené postupy zjišťování a nasazení aktualizací zabezpečení. Tyto dokumenty obsahují doporučení a informace, které mohou odborníkům v oblasti IT pomoci porozumět, jak se používají různé nástroje pro detekci a nasazení aktualizací zabezpečení. Další informace získáte v [článku 961747 znalostní báze Microsoft Knowledge Base](http://support.microsoft.com/kb/961747).

**Nástroj Microsoft Baseline Security Analyzer**

Pomocí nástroje Microsoft Baseline Security Analyzer (MBSA) mohou správci prohledávat místní i vzdálené systémy a zjistit tak, jestli v nich nechybí některé aktualizace zabezpečení nebo jestli v nastavení zabezpečení systému nedošlo k některým běžným chybám. Další informace o nástroji MBSA získáte na webu [Microsoft Baseline Security Analyzer](http://go.microsoft.com/fwlink/?linkid=21134).

**Služba Windows Server Update Services**

Pomocí služby Windows Server Update Services (WSUS) mohou správci systémů rychle a spolehlivě instalovat nejnovější důležité aktualizace zabezpečení pro systémy Windows 2000 a novější, sadu Office XP a novější, Exchange Server 2003 a SQL Server 2000 do systémů Windows 2000 a novějších.

Další informace o způsobu instalace této aktualizace zabezpečení pomocí služby Windows Server Update Services získáte na webu služby [Windows Server Update Services](http://go.microsoft.com/fwlink/?linkid=50120).

**Systems Management Server**

Microsoft Systems Management Server (SMS) představuje v rozlehlých sítích řešení pro správu aktualizací s rozsáhlými možnostmi konfigurace. Umožňuje správcům identifikovat počítače se systémem Windows, které vyžadují aktualizace zabezpečení, a provést řízenou instalaci těchto aktualizací v celé rozlehlé síti s minimálním dopadem na koncové uživatele. K dispozici je nyní nová verze nástroje SMS, System Center Configuration Manager 2007 (viz také webové stránky produktu [System Center Configuration Manager 2007](http://technet.microsoft.com/en-us/library/bb735860.aspx)). Další informace o tom, jak mohou správci pomocí serveru SMS 2003 nasazovat aktualizace zabezpečení, získáte na webu [SMS 2003 Security Patch Management](http://go.microsoft.com/fwlink/?linkid=22939). Uživatelé služby SMS 2.0 mohou k nasazení aktualizací zabezpečení použít také nástroj SUIT (Security Update Inventory Tool). Další informace o serveru SMS získáte na webu [Microsoft Systems Management Server](http://go.microsoft.com/fwlink/?linkid=21158).

**Poznámka:** Služba SMS pomocí modulu Microsoft Baseline Security Analyzer poskytuje rozsáhlou podporu při zjišťování a nasazení aktualizací bulletinu zabezpečení. Tyto nástroje nemusí některé softwarové aktualizace zjistit. V takovém případě mohou správci použít funkce serveru SMS a nasměrovat aktualizace do určitých systémů. Další informace o tomto postupu najdete na webu [Nasazení aktualizací softwaru pomocí funkce Distribuce softwaru serveru SMS](http://go.microsoft.com/fwlink/?linkid=33341). Některé aktualizace zabezpečení vyžadují po restartování počítače oprávnění správce. Správci mohou k instalaci těchto aktualizací použít nástroj Elevated Rights Deployment Tool (k dispozici v sadě [SMS 2003 Administration Feature Pack](http://go.microsoft.com/fwlink/?linkid=33387) a [SMS 2.0 Administration Feature Pack](http://go.microsoft.com/fwlink/?linkid=21161)).

**Nástroj Update Compatibility Evaluator a sada Application Compatibility Toolkit**

Aktualizace často zapisují do stejných souborů a nastavení registru požadovaných pro spouštění aplikací. To může způsobit nekompatibilitu a zvýšit dobu, po kterou trvá nasazení aktualizací zabezpečení. Testování a ověřování aktualizací systému Windows lze usnadnit pomocí součástí nástroje [Update Compatibility Evaluator](http://technet2.microsoft.com/windowsvista/en/library/4279e239-37a4-44aa-aec5-4e70fe39f9de1033.mspx?mfr=true), které jsou dodávány se sadou [Application Compatibility Toolkit](http://www.microsoft.com/downloads/details.aspx?familyid=24da89e9-b581-47b0-b45e-492dd6da2971&displaylang=en).

Sada Application Compatibility Toolkit (ACT) obsahuje nezbytné nástroje a dokumentaci pro posouzení a zmírnění problémů s kompatibilitou aplikací před nasazením systému Microsoft Windows Vista, služby Windows Update, aktualizací zabezpečení společnosti Microsoft nebo nové verze aplikace Windows Internet Explorer ve vašem prostředí.

### Další informace

#### Nástroj pro odstranění škodlivého softwaru systému Microsoft Windows

Společnost Microsoft vydává aktualizovanou verzi Nástroje pro odstranění škodlivého softwaru systému Microsoft Windows na webu Windows Update, Microsoft Update, ve službě Windows Server Update Services a na webu služby Stažení softwaru.

#### Důležité aktualizace nesouvisející se zabezpečením na webu Microsoft Update (MU), Windows Update (WU) a ve službě Windows Server Update Services (WSUS)

Informace o aktualizacích nesouvisejících se zabezpečením na webu Windows Update a Microsoft Update naleznete na webové stránce:

-   [Článek 894199 znalostní báze Microsoft Knowledge Base](http://support.microsoft.com/kb/894199): Popis služeb Software Update Services a Windows Server Update Services se mění v obsahu. Zahrnuje celý obsah systému Windows.
-   [Aktualizace vydané v uplynulých měsících pro službu Windows Server Update Services](http://technet.microsoft.com/en-us/wsus/bb456965.aspx). Obsahuje přehled všech nových, revidovaných a opětovně vydaných aktualizací pro jiné produkty společnosti Microsoft, než je systém Microsoft Windows.

#### Microsoft Active Protections Program (MAPP)

Pro zlepšení ochrany dat svých zákazníků poskytuje společnost Microsoft informace o chybách v zabezpečení všem hlavním dodavatelům softwaru pro zabezpečení, a to vždy ještě před vydáním nové měsíční zprávy o aktualizaci zabezpečení. Dodavatelé softwaru pro zabezpečení tak mohou tyto informace o chybách v zabezpečení využít a poskytnout svým zákazníkům ochranu včasnou aktualizací svých programů a zařízení pro zabezpečení, jako jsou antivirové programy, síťové systémy pro detekci napadení či hostitelské systémy pro prevenci napadení. Informace o dostupnosti aktuálních prostředků aktivní ochrany od jednotlivých dodavatelů softwaru pro zabezpečení naleznete na stránkách aktivní ochrany jednotlivých partnerů programu MAPP. Seznam těchto partnerů naleznete na stránce [Microsoft Active Protections Program (MAPP) Partners](http://www.microsoft.com/security/msrc/mapp/partners.mspx).

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

-   Neelu Mehtovi ze společnosti [Google Inc.](http://www.google.com/) za oznámení chyby popsané v bulletinu MS09-063.
-   Codymu Piercovi ze společnosti [TippingPoint DVLabs](http://dvlabs.tippingpoint.com/) za oznámení chyby popsané v bulletinu MS09-064.
-   Aginu Sunovi za oznámení chyby popsané v bulletinu MS09-065.
-   Tavisu Ormandymu ze společnosti [Google Inc.](http://www.google.com/) za oznámení chyby popsané v bulletinu MS09-065.
-   Bingu Liuovi z výzkumného týmu [FortiGuard Labs](http://www.fortiguard.com/) společnosti Fortinet za oznámení tří chyb popsaných v bulletinu MS09-067.
-   Společnosti [TippingPoint](http://www.tippingpoint.com/) a organizaci [Zero Day Initiative](http://www.zerodayinitiative.com/) za oznámení chyby popsané v bulletinu MS09-067.
-   Seanu Larssonovi ze společnosti [VeriSign iDefense Labs](http://labs.idefense.com/) za oznámení chyby popsané v bulletinu MS09-067.
-   Anonymnímu výzkumníkovi spolupracujícímu se společností [TippingPoint](http://www.tippingpoint.com/) a organizací [Zero Day Initiative](http://www.zerodayinitiative.com/) za oznámení chyby popsané v bulletinu MS09-067.
-   Nicolasi Jolymu ze společnosti [VUPEN Security](http://www.vupen.com/) za oznámení čtyř chyb popsaných v bulletinu MS09-067.
-   Junu Maovi ze společnosti [VeriSign iDefense Labs](http://labs.idefense.com/) za oznámení chyby popsané v bulletinu MS09-068.

#### Technická podpora

-   Uvedený software byl testován za účelem zjištění, kterých verzí se chyba týká. U dalších verzí skončila časově omezená podpora. Pokud chcete zjistit dobu, po kterou je pro určitou verzi softwaru poskytována podpora, navštivte web [Zásady poskytování technické podpory pro produkty společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=21742).
-   Zákazníci mohou získat technickou podporu na webu [služby technické podpory společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=21131). Hovory související s aktualizacemi zabezpečení jsou bezplatné. Další informace o dostupných možnostech technické podpory naleznete na webu [Pomoc a podpora společnosti Microsoft](http://support.microsoft.com/).
-   Mezinárodní zákazníci získají podporu u místních zastoupení společnosti Microsoft. Technická podpora související s aktualizacemi zabezpečení je bezplatná. Další informace o možnostech kontaktování společnosti Microsoft v případě potřeby technické podpory získáte na [webu mezinárodní technické podpory](http://go.microsoft.com/fwlink/?linkid=21155).

#### Zřeknutí se záruky

Informace ve znalostní bázi Microsoft Knowledge Base jsou poskytovány tak, jak jsou, bez jakékoli záruky. Společnost Microsoft neposkytuje žádné záruky, výslovně uvedené či mlčky předpokládané, včetně záruk obchodovatelnosti a vhodnosti pro určitý účel. Společnost Microsoft ani její dodavatelé nenesou v žádném případě zodpovědnost za žádné škody, včetně přímých, nepřímých, náhodných či následných škod, ztráty zisku či zvláštních škod, a to ani v případě, že byli na možnost takových škod upozorněni. V některých zemích a právních řádech není dovoleno vyloučit nebo omezit odpovědnost, proto se výše uvedené omezení na vás nemusí vztahovat.

#### Revize

-   V1.0 (10. listopadu 2009): Souhrnný bulletin byl publikován.
-   V1.1 (25. listopadu 2009): Byla přidána důležitá poznámka týkající se indexu zneužitelnosti pro chybu zabezpečení CVE-2009-2523.

*Built at 2014-04-18T01:50:00Z-07:00*
