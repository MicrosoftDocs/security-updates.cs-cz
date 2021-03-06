---
TOCTitle: 'MS11-JUL'
Title: 'Souhrnný bulletin zabezpečení společnosti Microsoft, červenec 2011'
ms:assetid: 'ms11-jul'
ms:contentKeyID: 61224011
ms:mtpsurl: 'https://technet.microsoft.com/cs-CZ/library/ms11-jul(v=Security.10)'
---

 

Souhrnný bulletin zabezpečení společnosti Microsoft, červenec 2011
==================================================================

Publikováno: 12. července 2011

**Verze:** 1.0

Tento souhrnný bulletin uvádí bulletiny zabezpečení vydané v červenci 2011.

Spolu s vydáním bulletinů zabezpečení pro červenec 2011 nahrazuje tento souhrnný bulletin předběžné oznámení o bulletinech vydané 7. července 2011. Další informace o službě předběžného oznámení o bulletinech naleznete v části [Předběžné oznámení o bulletinech zabezpečení společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=217213).

Informace o tom, jak dostávat automatická oznámení o vydání nových bulletinů zabezpečení společnosti Microsoft, naleznete na webu [Zasílání technických oznámení o zabezpečení společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=21163).

Pro zodpovězení zákaznických dotazů týkajících se těchto bulletinů uspořádá společnost Microsoft 13. července 2011 v 11:00 časového pásma Tichomoří (USA a Kanada) webové vysílání. [Registrovat se pro webové vysílání týkající se červencových bulletinů zabezpečení](https://msevents.microsoft.com/cui/webcasteventdetails.aspx?eventid=1032487855&eventcategory=4). Po tomto datu je webové vysílání dostupné na požádání. Další informace získáte v [souhrnných bulletinech zabezpečení společnosti Microsoft a webovém vysílání](http://go.microsoft.com/fwlink/?linkid=217214).

Společnost Microsoft se snaží zákazníkům usnadnit upřednostnění měsíčně vydávaných aktualizací zabezpečení s jakýmikoli aktualizacemi nesouvisejícími se zabezpečením, které jsou vydány ve stejný den jako měsíčně vydávané aktualizace zabezpečení. Další informace získáte v části **Další informace**.

### Informace o bulletinech

Shrnutí
-------


Následující tabulka shrnuje podle závažnosti bulletiny zabezpečení pro tento měsíc.

Podrobnosti o softwaru obsahujícím tuto chybu naleznete v následující části **Software obsahující tuto chybu a umístění aktualizací ke stažení**.

 
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
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217102">MS11-053</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení týkající se zásobníku Bluetooth umožňuje vzdálené spuštění kódu (2566220)</strong> <br />
<br />
Tato aktualizace zabezpečení řeší chybu zabezpečení týkající se zásobníku Bluetooth systému Windows oznámenou soukromou osobou. Tato chyba zabezpečení může umožnit vzdálené spuštění kódu, pokud útočník odešle do postiženého systému sérii speciálně vytvořených paketů Bluetooth. Útočník by tak mohl instalovat programy, zobrazovat, měnit či odstraňovat data nebo vytvářet nové účty s úplnými uživatelskými právy. Tato chyba zabezpečení se týká pouze systémů vybavených technologií Bluetooth.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritický</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=220172">MS11-054</a></td>
<td style="border:1px solid black;"><strong>Chyby zabezpečení v ovladačích režimu jádra systému Windows umožňují zvýšení úrovně oprávnění (2555917)</strong> <br />
<br />
Tato aktualizace zabezpečení řeší 15 chyb zabezpečení v systému Microsoft Windows oznámených soukromou osobou. Nejzávažnější z těchto chyb zabezpečení by mohla umožnit zvýšení úrovně oprávnění, pokud by se útočník místně přihlásil k systému a spustil speciálně vytvořenou aplikaci. Tyto chyby zabezpečení může zneužít pouze útočník s platnými pověřeními pro přihlášení, která by mu umožňovala se místně přihlásit.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Vysoký</a><br />
Zvýšení úrovně oprávnění</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217465">MS11-056</a></td>
<td style="border:1px solid black;"><strong>Chyby zabezpečení v podsystému Windows CSRSS (Client/Server Run-time Subsystem) umožňují zvýšení úrovně oprávnění (2507938) </strong><br />
<br />
Tato aktualizace zabezpečení řeší pět chyb zabezpečení v podsystému Microsoft Windows CSRSS (Client/Server Run-time Subsystem) oznámených soukromou osobou. Tyto chyby zabezpečení by mohly způsobit zvýšení úrovně oprávnění, pokud by se útočník přihlásil k systému uživatele a spustil speciálně vytvořenou aplikaci. Tyto chyby zabezpečení může zneužít pouze útočník s platnými pověřeními pro přihlášení, která by mu umožňovala se místně přihlásit.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Vysoký</a><br />
Zvýšení úrovně oprávnění</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=220276">MS11-055</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení v aplikaci Microsoft Visio umožňuje vzdálené spuštění kódu (2560847) </strong><br />
<br />
Tato aktualizace zabezpečení řeší veřejně známou chybu zabezpečení v aplikaci Microsoft Visio. Chyba zabezpečení by mohla umožnit vzdálené spuštění kódu, pokud uživatel otevře legitimní soubor aplikace Visio umístěný ve stejném síťovém adresáři jako speciálně vytvořený soubor knihovny. Útočník, který by úspěšně zneužil tuto chybu zabezpečení, by mohl získat stejná uživatelská práva, jaká má přihlášený uživatel. Uživatelé, jejichž účty jsou konfigurovány tak, aby měli v systému méně uživatelských práv, by byli vystaveni menšímu riziku než uživatelé s uživatelskými právy správce.</td>
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
  

Následující tabulka uvádí hodnocení zneužitelnosti každé chyby zabezpečení uvedené v tomto měsíci. Chyby zabezpečení jsou řazeny podle čísla jednotlivých bulletinů (ID bulletinu) a chyb (ID CVE). Uvedeny jsou pouze chyby zabezpečení ohodnocené stupněm závažnosti Kritický nebo Vysoký.
  
**Jak pracovat s touto tabulkou**
  
V této tabulce zjistíte, jaká je pravděpodobnost zneužití v podobě spuštění kódu a odmítnutí služby během 30 dní od vydání tohoto bulletinu zabezpečení pro všechny aktualizace zabezpečení, které bude třeba nainstalovat. Všechna níže uvedená hodnocení zvažte na základě vaší specifické konfigurace a podle závěrů hodnocení nastavte priority pro zavádění jednotlivých aktualizací vydaných v tomto měsíci. Další informace o významu těchto hodnocení a způsobu jejich stanovení najdete v indexu zneužitelnosti [Microsoft Exploitability Index](http://technet.microsoft.com/en-us/security/cc998259.aspx).
  
Položka nazvaná „Nejnovější vydání softwaru“ odkazuje na příslušný software. Položka nazvaná „Starší vydání softwaru“ odkazuje na všechna starší podporovaná vydání příslušného softwaru, uvedeného v tabulkách bulletinu „Software obsahující tuto chybu“ a „Software neobsahující tuto chybu“.
  
| ID bulletinu                                              | Název chyby zabezpečení                                                        | ID CVE                                                                           | Hodnocení zneužitelnosti spuštění kódu u nejnovějšího vydání softwaru                                                      | Hodnocení zneužitelnosti spuštění kódu u starších vydání softwaru                                                          | Hodnocení zneužitelnosti odmítnutí služby | Hlavní poznámky                                                                                                                                  |  
|-----------------------------------------------------------|--------------------------------------------------------------------------------|----------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------|-------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------|  
| [MS11-053](http://go.microsoft.com/fwlink/?linkid=217102) | Chyba zabezpečení týkající se zásobníku Bluetooth                              | [CVE-2011-1265](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1265) | Žádné ohrožení                                                                                                             | [2](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Je pravděpodobné vytvoření kódu nekonsistentního zneužití | Trvalé                                    | Tato chyba zabezpečení se týká pouze klientských systémů (podporované verze systémů Windows Vista a Windows 7) vybavených technologií Bluetooth. |  
| [MS11-054](http://go.microsoft.com/fwlink/?linkid=220172) | Chyba zabezpečení týkající se použití subsystému Win32k po uvolnění            | [CVE-2011-1874](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1874) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Je pravděpodobné vytvoření kódu konsistentního zneužití   | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Je pravděpodobné vytvoření kódu konsistentního zneužití   | Trvalé                                    | (Žádné)                                                                                                                                          |  
| [MS11-054](http://go.microsoft.com/fwlink/?linkid=220172) | Chyba zabezpečení týkající se použití subsystému Win32k po uvolnění            | [CVE-2011-1875](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1875) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Je pravděpodobné vytvoření kódu konsistentního zneužití   | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Je pravděpodobné vytvoření kódu konsistentního zneužití   | Trvalé                                    | (Žádné)                                                                                                                                          |  
| [MS11-054](http://go.microsoft.com/fwlink/?linkid=220172) | Chyba zabezpečení týkající se použití subsystému Win32k po uvolnění            | [CVE-2011-1876](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1876) | [2](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Je pravděpodobné vytvoření kódu nekonsistentního zneužití | [2](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Je pravděpodobné vytvoření kódu nekonsistentního zneužití | Trvalé                                    | (Žádné)                                                                                                                                          |  
| [MS11-054](http://go.microsoft.com/fwlink/?linkid=220172) | Chyba zabezpečení týkající se použití subsystému Win32k po uvolnění            | [CVE-2011-1877](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1877) | [2](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Je pravděpodobné vytvoření kódu nekonsistentního zneužití | [2](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Je pravděpodobné vytvoření kódu nekonsistentního zneužití | Trvalé                                    | (Žádné)                                                                                                                                          |  
| [MS11-054](http://go.microsoft.com/fwlink/?linkid=220172) | Chyba zabezpečení týkající se použití subsystému Win32k po uvolnění            | [CVE-2011-1878](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1878) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Je pravděpodobné vytvoření kódu konsistentního zneužití   | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Je pravděpodobné vytvoření kódu konsistentního zneužití   | Trvalé                                    | (Žádné)                                                                                                                                          |  
| [MS11-054](http://go.microsoft.com/fwlink/?linkid=220172) | Chyba zabezpečení týkající se použití subsystému Win32k po uvolnění            | [CVE-2011-1879](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1879) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Je pravděpodobné vytvoření kódu konsistentního zneužití   | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Je pravděpodobné vytvoření kódu konsistentního zneužití   | Trvalé                                    | (Žádné)                                                                                                                                          |  
| [MS11-054](http://go.microsoft.com/fwlink/?linkid=220172) | Chyba zabezpečení týkající se vyhodnocování ukazatele Win32k Null              | [CVE-2011-1880](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1880) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Je pravděpodobné vytvoření kódu konsistentního zneužití   | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Je pravděpodobné vytvoření kódu konsistentního zneužití   | Trvalé                                    | (Žádné)                                                                                                                                          |  
| [MS11-054](http://go.microsoft.com/fwlink/?linkid=220172) | Chyba zabezpečení týkající se vyhodnocování ukazatele Win32k Null              | [CVE-2011-1881](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1881) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Je pravděpodobné vytvoření kódu konsistentního zneužití   | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Je pravděpodobné vytvoření kódu konsistentního zneužití   | Trvalé                                    | (Žádné)                                                                                                                                          |  
| [MS11-054](http://go.microsoft.com/fwlink/?linkid=220172) | Chyba zabezpečení týkající se použití subsystému Win32k po uvolnění            | [CVE-2011-1882](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1882) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Je pravděpodobné vytvoření kódu konsistentního zneužití   | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Je pravděpodobné vytvoření kódu konsistentního zneužití   | Trvalé                                    | (Žádné)                                                                                                                                          |  
| [MS11-054](http://go.microsoft.com/fwlink/?linkid=220172) | Chyba zabezpečení týkající se použití subsystému Win32k po uvolnění            | [CVE-2011-1883](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1883) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Je pravděpodobné vytvoření kódu konsistentního zneužití   | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Je pravděpodobné vytvoření kódu konsistentního zneužití   | Trvalé                                    | (Žádné)                                                                                                                                          |  
| [MS11-054](http://go.microsoft.com/fwlink/?linkid=220172) | Chyba zabezpečení týkající se použití subsystému Win32k po uvolnění            | [CVE-2011-1884](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1884) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Je pravděpodobné vytvoření kódu konsistentního zneužití   | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Je pravděpodobné vytvoření kódu konsistentního zneužití   | Trvalé                                    | (Žádné)                                                                                                                                          |  
| [MS11-054](http://go.microsoft.com/fwlink/?linkid=220172) | Chyba zabezpečení týkající se vyhodnocování ukazatele Win32k Null              | [CVE-2011-1885](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1885) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Je pravděpodobné vytvoření kódu konsistentního zneužití   | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Je pravděpodobné vytvoření kódu konsistentního zneužití   | Trvalé                                    | (Žádné)                                                                                                                                          |  
| [MS11-054](http://go.microsoft.com/fwlink/?linkid=220172) | Chyba zabezpečení nesprávného parametru Win32k umožňuje přístup k informacím   | [CVE-2011-1886](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1886) | [3](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Vytvoření kódu funkčního zneužití není pravděpodobné      | [3](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Vytvoření kódu funkčního zneužití není pravděpodobné      | Trvalé                                    | Jedná se o chybu zabezpečení typu zpřístupnění informací.                                                                                        |  
| [MS11-054](http://go.microsoft.com/fwlink/?linkid=220172) | Chyba zabezpečení týkající se vyhodnocování ukazatele Win32k Null              | [CVE-2011-1887](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1887) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Je pravděpodobné vytvoření kódu konsistentního zneužití   | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Je pravděpodobné vytvoření kódu konsistentního zneužití   | Trvalé                                    | (Žádné)                                                                                                                                          |  
| [MS11-054](http://go.microsoft.com/fwlink/?linkid=220172) | Chyba zabezpečení týkající se vyhodnocování ukazatele Win32k Null              | [CVE-2011-1888](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1888) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Je pravděpodobné vytvoření kódu konsistentního zneužití   | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Je pravděpodobné vytvoření kódu konsistentního zneužití   | Trvalé                                    | (Žádné)                                                                                                                                          |  
| [MS11-055](http://go.microsoft.com/fwlink/?linkid=220276) | Chyba zabezpečení nezabezpečeného načítání knihovny v aplikaci Microsoft Visio | [CVE-2010-3148](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3148) | Žádné ohrožení                                                                                                             | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Je pravděpodobné vytvoření kódu konsistentního zneužití   | Netýká se                                 | Tato chyba zabezpečení je veřejně známá.                                                                                                         |  
| [MS11-056](http://go.microsoft.com/fwlink/?linkid=217465) | Chyba zabezpečení CSRSS Local EOP AllocConsole                                 | [CVE-2011-1281](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1281) | [3](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Vytvoření kódu funkčního zneužití není pravděpodobné      | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Je pravděpodobné vytvoření kódu konsistentního zneužití   | Netýká se                                 | (Žádné)                                                                                                                                          |  
| [MS11-056](http://go.microsoft.com/fwlink/?linkid=217465) | Chyba zabezpečení CSRSS Local EOP SrvSetConsoleLocalEUDC                       | [CVE-2011-1282](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1282) | [3](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Vytvoření kódu funkčního zneužití není pravděpodobné      | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Je pravděpodobné vytvoření kódu konsistentního zneužití   | Trvalé                                    | (Žádné)                                                                                                                                          |  
| [MS11-056](http://go.microsoft.com/fwlink/?linkid=217465) | Chyba zabezpečení CSRSS Local EOP SrvSetConsoleNumberOfCommand                 | [CVE-2011-1283](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1283) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Je pravděpodobné vytvoření kódu konsistentního zneužití   | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Je pravděpodobné vytvoření kódu konsistentního zneužití   | Trvalé                                    | (Žádné)                                                                                                                                          |  
| [MS11-056](http://go.microsoft.com/fwlink/?linkid=217465) | Chyba zabezpečení CSRSS Local EOP SrvWriteConsoleOutput                        | [CVE-2011-1284](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1284) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Je pravděpodobné vytvoření kódu konsistentního zneužití   | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Je pravděpodobné vytvoření kódu konsistentního zneužití   | Trvalé                                    | (Žádné)                                                                                                                                          |  
| [MS11-056](http://go.microsoft.com/fwlink/?linkid=217465) | Chyba zabezpečení CSRSS Local EOP SrvWriteConsoleOutputString                  | [CVE-2011-1870](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1870) | [3](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Vytvoření kódu funkčního zneužití není pravděpodobné      | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Je pravděpodobné vytvoření kódu konsistentního zneužití   | Trvalé                                    | (Žádné)                                                                                                                                          |
  
Software obsahující tuto chybu a umístění aktualizací ke stažení  
----------------------------------------------------------------
  

Následující tabulky řadí bulletiny podle kategorie hlavního softwaru a závažnosti.
  
**Jak pracovat s těmito tabulkami?**
  
V těchto tabulkách zjistíte, které aktualizace zabezpečení bude třeba nainstalovat. Přečtěte si seznam všech programů a komponent a zjistěte, zda se některé aktualizace zabezpečení týkají vaší instalace. Pokud se program nebo komponenta v seznamu nachází, je v něm zároveň uveden odkaz na dostupnou aktualizaci softwaru a také stupeň závažnosti aktualizace softwaru.
  
**Poznámka:** Jedna chyba zabezpečení může vyžadovat instalaci více aktualizací. Přečtěte si celý sloupec u každého identifikátoru bulletinu. Zjistíte v něm, které aktualizace je třeba nainstalovat v závislosti na programech nebo součástech nainstalovaných ve vašem systému.
  
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
</tr>
<tr>
<th colspan="4" style="border:1px solid black;">
Windows XP  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS11-053**](http://go.microsoft.com/fwlink/?linkid=217102)
</td>
<td style="border:1px solid black;">
[**MS11-054**](http://go.microsoft.com/fwlink/?linkid=220172)
</td>
<td style="border:1px solid black;">
[**MS11-056**](http://go.microsoft.com/fwlink/?linkid=217465)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Celkový stupeň závažnosti**
</td>
<td style="border:1px solid black;">
Žádný
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
Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=d7a47370-f415-46ea-9a82-a943f743c8b6)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=425c705e-94f2-4fa6-9df2-dc71897215fa)  
(Vysoký)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=db89d88f-d0d4-4ed6-8589-bf27557c0304)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c389fa20-677e-49b6-af44-781e5522d08b)  
(Vysoký)
</td>
</tr>
<tr>
<th colspan="4" style="border:1px solid black;">
Windows Server 2003
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS11-053**](http://go.microsoft.com/fwlink/?linkid=217102)
</td>
<td style="border:1px solid black;">
[**MS11-054**](http://go.microsoft.com/fwlink/?linkid=220172)
</td>
<td style="border:1px solid black;">
[**MS11-056**](http://go.microsoft.com/fwlink/?linkid=217465)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Celkový stupeň závažnosti**
</td>
<td style="border:1px solid black;">
Žádný
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
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7a26a437-a705-4d48-8389-50f159a39891)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=dff4c67a-8c8b-4d7d-84c7-57429becf0ff)  
(Vysoký)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=95393f89-0b05-4243-95ed-17bcdad24bfb)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=1615a995-9a04-440a-ae52-5917738f0ecb)  
(Vysoký)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 SP2 pro systémy s procesorem Itanium
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=3b094bdb-4150-44f2-a638-afd5f41b00a3)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=a81c011d-eeea-4383-9efb-df70515ab357)  
(Vysoký)
</td>
</tr>
<tr>
<th colspan="4" style="border:1px solid black;">
Windows Vista
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS11-053**](http://go.microsoft.com/fwlink/?linkid=217102)
</td>
<td style="border:1px solid black;">
[**MS11-054**](http://go.microsoft.com/fwlink/?linkid=220172)
</td>
<td style="border:1px solid black;">
[**MS11-056**](http://go.microsoft.com/fwlink/?linkid=217465)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Celkový stupeň závažnosti**
</td>
<td style="border:1px solid black;">
[**Kritický**](http://go.microsoft.com/fwlink/?linkid=21140)
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
Windows Vista Service Pack 1 a Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=6bff74ac-45f3-4585-92da-316921b458fa)<sup>[1]</sup>
(KB2561109)  
(Kritický)  
[Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=a1e5aa7d-5f38-4ce2-9575-4b4cb7520160)  
(KB2532531)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 a Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c1fe1e53-34d5-497e-8ba2-50caa8dc1158)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 a Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=a5e192af-dae5-47ef-a9d0-f761a8caa974)  
(Vysoký)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 1 a Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=849d2694-c8b3-4670-8203-912661bccabf)<sup>[1]</sup>
(KB2561109)  
(Kritický)  
[Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4287eeb4-ab29-4727-83f2-260d838b44d4)  
(KB2532531)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 a Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7bc0a285-cc32-4c6b-abee-d92130d459b7)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 a Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=1007f5d3-9be1-4f03-a3f0-12ddb555653c)  
(Vysoký)
</td>
</tr>
<tr>
<th colspan="4" style="border:1px solid black;">
Windows Server 2008
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS11-053**](http://go.microsoft.com/fwlink/?linkid=217102)
</td>
<td style="border:1px solid black;">
[**MS11-054**](http://go.microsoft.com/fwlink/?linkid=220172)
</td>
<td style="border:1px solid black;">
[**MS11-056**](http://go.microsoft.com/fwlink/?linkid=217465)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Celkový stupeň závažnosti**
</td>
<td style="border:1px solid black;">
Žádný
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
Windows Server 2008 pro 32bitové systémy a Windows Server 2008 pro 32bitové systémy Service Pack 2
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro 32bitové systémy a Windows Server 2008 pro 32bitové systémy Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b88d0471-4427-4835-9446-db71116481f0)\*  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro 32bitové systémy a Windows Server 2008 pro 32bitové systémy Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=36e3dbaf-36f5-4c74-8f11-ecbef46f58e1)\*  
(Vysoký)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 pro systémy s procesorem x64 a Windows Server 2008 pro systémy s procesorem x64 Service Pack 2
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem x64 a Windows Server 2008 pro systémy s procesorem x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d3df6184-3e3c-4949-a1ee-293ec68f8149)\*  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem x64 a Windows Server 2008 pro systémy s procesorem x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b43d2ab5-e281-4c6b-bb37-1f1b5d86ac82)\*  
(Vysoký)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 pro systémy s procesorem Itanium a Windows Server 2008 pro systémy s procesorem Itanium Service Pack 2
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem Itanium a Windows Server 2008 pro systémy s procesorem Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=9e021d69-7f0c-457f-af86-07e760d8f421)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem Itanium a Windows Server 2008 pro systémy s procesorem Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b70209f2-1c51-45af-b3c4-3473aebcdb35)  
(Vysoký)
</td>
</tr>
<tr>
<th colspan="4" style="border:1px solid black;">
Windows 7
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS11-053**](http://go.microsoft.com/fwlink/?linkid=217102)
</td>
<td style="border:1px solid black;">
[**MS11-054**](http://go.microsoft.com/fwlink/?linkid=220172)
</td>
<td style="border:1px solid black;">
[**MS11-056**](http://go.microsoft.com/fwlink/?linkid=217465)
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
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 pro 32bitové systémy a Windows 7 pro 32bitové systémy Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows 7 pro 32bitové systémy a Windows 7 pro 32bitové systémy Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=7f811b75-c3ff-411a-aaa9-126dce34cc01)  
(KB2532531)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows 7 pro 32bitové systémy a Windows 7 pro 32bitové systémy Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=41db1b2f-f862-43bb-89bc-4b97737e5cb9)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows 7 pro 32bitové systémy a Windows 7 pro 32bitové systémy Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=ac3b435c-8caf-40cc-8f13-b52261b3b9e6)  
(Vysoký)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 7 pro systémy s procesorem x64 a Windows 7 pro systémy s procesorem x64 Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows 7 pro systémy s procesorem x64 a Windows 7 pro systémy s procesorem x64 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=90b2da71-18f9-46ee-9e3d-b08620ca06aa)  
(KB2532531)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows 7 pro systémy s procesorem x64 a Windows 7 pro systémy s procesorem x64 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=211abdc6-40c7-4bfc-8c2d-be72981f311e)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows 7 pro systémy s procesorem x64 a Windows 7 pro systémy s procesorem x64 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=64e5f889-fa46-4884-9b22-3ba4e2fba1b9)  
(Vysoký)
</td>
</tr>
<tr>
<th colspan="4" style="border:1px solid black;">
Windows Server 2008 R2
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS11-053**](http://go.microsoft.com/fwlink/?linkid=217102)
</td>
<td style="border:1px solid black;">
[**MS11-054**](http://go.microsoft.com/fwlink/?linkid=220172)
</td>
<td style="border:1px solid black;">
[**MS11-056**](http://go.microsoft.com/fwlink/?linkid=217465)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Celkový stupeň závažnosti**
</td>
<td style="border:1px solid black;">
Žádný
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
Windows Server 2008 R2 pro systémy s procesorem x64 a Windows Server 2008 R2 pro systémy s procesorem x64 Service Pack 1
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem x64 a Windows Server 2008 R2 pro systémy s procesorem x64 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=4f54e498-3825-407d-a036-1900a65d34f1)\*  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem x64 a Windows Server 2008 R2 pro systémy s procesorem x64 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=b99a40cf-8a31-43d9-bd0b-a458a533068b)\*  
(Vysoký)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 pro systémy s procesorem Itanium a Windows Server 2008 R2 pro systémy s procesorem Itanium Service Pack 1
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem Itanium a Windows Server 2008 R2 pro systémy s procesorem Itanium Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=e7ae39e8-1154-4a13-8598-29d4a6358762)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem Itanium a Windows Server 2008 R2 pro systémy s procesorem Itanium Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=784efc20-3a41-42ab-b48d-51fd59d71523)  
(Vysoký)
</td>
</tr>
</table>
<p></p>

 
**Poznámka k systémům Windows Server 2008 a Windows Server 2008 R2**

**\*Instalace Server Core obsahující chybu zabezpečení.** Tato aktualizace se stejným hodnocením závažnosti se vztahuje k podporovaným edicím systému Windows Server 2008 nebo Windows Server 2008 R2, jak je uvedeno, s instalací pomocí volby pro instalaci Server Core nebo bez ní. Další informace o této možnosti instalace naleznete v článcích na webu TechNet [Managing a Server Core Installation](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) (Správa instalace Server Core) a [Servicing a Server Core Installation](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx) (Obsluha instalace Server Core). Možnost instalace Server Core se nevztahuje na určité edice systému Windows Server 2008 a Windows Server 2008 R2; další informace naleznete v části [Porovnání možností instalace Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**Poznámka k bulletinu MS11-053**

<sup>[1]</sup>Systém Windows Vista Service Pack 1 je postižen pouze v případě, že byla nainstalována volitelná sada Windows Vista Feature Pack for Wireless.

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
[**MS11-055**](http://go.microsoft.com/fwlink/?linkid=220276)
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
Microsoft Visio 2003 Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Visio 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=1c7b2a5b-4aa6-4006-90bf-89f8b2b7becd)  
(KB2493523)  
(Vysoký)
</td>
</tr>
</table>
<p></p>

 

Nástroje a doporučené postupy zjišťování a nasazení
---------------------------------------------------


**Centrum zabezpečení**

Umožňuje správu aktualizací softwaru a zabezpečení, které je třeba nainstalovat na servery, stolní počítače a přenosné počítače v organizaci. Další informace naleznete na webu [TechNet Update Management Center](http://go.microsoft.com/fwlink/?linkid=69903). Další informace o zabezpečení produktů společnosti Microsoft nabízí web [Centrum zabezpečení TechNet](http://go.microsoft.com/fwlink/?linkid=21171). Tyto informace lze také získat kliknutím na nabídku „Nejnovější aktualizace zabezpečení“ na webu [Zabezpečení doma](http://go.microsoft.com/fwlink/?linkid=85102).

Aktualizace zabezpečení jsou k dispozici na webu [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747) a [Windows Update](http://go.microsoft.com/fwlink/?linkid=21130). Aktualizace zabezpečení jsou také k dispozici na webu [služby Stažení softwaru](http://go.microsoft.com/fwlink/?linkid=21129). Nejsnadněji je naleznete hledáním podle klíčových slov aktualizace zabezpečení.

Zákazníkům systému Microsoft Office for Mac doporučujeme využít funkci Microsoft AutoUpdate for Mac, která udržuje software společnosti Microsoft v aktuálním stavu. Další informace o funkci Microsoft AutoUpdate for Mac naleznete na webu [Check for software updates automatically](http://mac2.microsoft.com/help/office/14/en-us/word/item/ffe35357-8f25-4df8-a0a3-c258526c64ea) (Automatická kontrola aktualizací softwaru).

Aktualizace zabezpečení lze stáhnout z katalogu služby [Microsoft Update Catalog](http://go.microsoft.com/fwlink/?linkid=96155). Služba Microsoft Update Catalog poskytuje katalog s možností vyhledávání obsahu dostupného prostřednictvím služeb Windows Update a Microsoft Update, včetně aktualizací zabezpečení, ovladačů a aktualizací Service Pack. Vyhledáváním pomocí čísla bulletinu zabezpečení (například MS07-036) můžete přidat všechny dostupné aktualizace do košíku (včetně různých jazykových verzí aktualizace) a stáhnout je do vybrané složky. Další informace o službě Microsoft Update Catalog najdete v části [Nejčastější dotazy týkající se služby Microsoft Update Catalog](http://go.microsoft.com/fwlink/?linkid=97900).

**Doporučené postupy zjišťování a nasazení**

Společnost Microsoft poskytuje doporučené postupy zjišťování a nasazení aktualizací zabezpečení. Tyto dokumenty obsahují doporučení a informace, které mohou odborníkům v oblasti IT pomoci porozumět, jak se používají různé nástroje pro detekci a nasazení aktualizací zabezpečení. Další informace získáte v [článku 961747 znalostní báze Microsoft Knowledge Base](http://support.microsoft.com/kb/961747).

**Nástroj Microsoft Baseline Security Analyzer**

Pomocí nástroje Microsoft Baseline Security Analyzer (MBSA) mohou správci prohledávat místní i vzdálené systémy a zjistit tak, jestli v nich nechybí některé aktualizace zabezpečení nebo jestli v nastavení zabezpečení systému nedošlo k některým běžným chybám. Další informace o nástroji MBSA získáte na webu [Microsoft Baseline Security Analyzer](http://go.microsoft.com/fwlink/?linkid=21134).

**Služba Windows Server Update Services**

Pomocí služby Windows Server Update Services (WSUS) mohou správci systémů rychle a spolehlivě nasadit nejnovější důležité aktualizace zabezpečení pro systémy Microsoft Windows 2000 a novější, systém Office XP a novější, Exchange Server 2003 a SQL Server 2000 do systémů Microsoft Windows 2000 a novějších.

Další informace o způsobu instalace této aktualizace zabezpečení pomocí služby Windows Server Update Services získáte na webu služby [Windows Server Update Services](http://technet.microsoft.com/en-us/wsus/default.aspx).

**System Center Configuration Manager 2007**

Služba Software Update Management nástroje Configuration Manager 2007 zjednodušuje složitý proces doručení a správy aktualizací do IT systémů firmy. Pomocí nástroje Configuration Manager 2007 mohou správci informačních technologií doručit aktualizace produktů společnosti Microsoft do řady zařízení, včetně stolních počítačů, notebooků, serverů a mobilních zařízení.

Automatizované hodnocení chyb zabezpečení v nástroji Configuration Manager 2007 odhaluje potřebu aktualizací a hlášení doporučených postupů. Základem služby Software Update Management nástroje Configuration Manager 2007 jsou služby WSUS (Microsoft Windows Software Update Services). Jedná se o časem prověřenou infrastrukturu aktualizací známou správcům informačních technologií po celém světě. Další informace o tom, jak mohou správci používat nástroj Configuration Manager 2007 k nasazení aktualizací, naleznete na webových stránkách [Software Update Management](http://www.microsoft.com/systemcenter/en/us/configuration-manager/cm-software-update-management.aspx). Další informace o nástroji Configuration Manager naleznete na webových stránkách [System Center Configuration Manager](http://www.microsoft.com/systemcenter/en/us/configuration-manager.aspx).

**Systems Management Server 2003**

Microsoft Systems Management Server (SMS) představuje v rozlehlých sítích řešení pro správu aktualizací s rozsáhlými možnostmi konfigurace. Umožňuje správcům identifikovat počítače se systémem Windows, které vyžadují aktualizace zabezpečení, a provést řízenou instalaci těchto aktualizací v celé rozlehlé síti s minimálním dopadem na koncové uživatele.

**Poznámka:** Systems Management Server 2003 není od 12. ledna 2010 součástí tradiční podpory. Další informace o životním cyklu produktů naleznete na webu [Životní cyklus podpory produktů společnosti Microsoft](http://support.microsoft.com/common/international.aspx?rdpath=dm;en-us;lifecycle). K dispozici je nyní nová verze nástroje SMS, System Center Configuration Manager 2007 (viz výše uvedená část **System Center Configuration Manager 2007**).

Další informace o tom, jak mohou správci pomocí serveru SMS 2003 nasazovat aktualizace zabezpečení, naleznete na webových stránkách [Scénáře a postupy pro Microsoft Systems Management Server 2003: Distribuce softwaru a správa oprav](http://www.microsoft.com/downloads/en/details.aspx?familyid=32f2bb4c-42f8-4b8d-844f-2553fd78049f&displaylang=en). Další informace o serveru SMS naleznete na webových stránkách [Microsoft Systems Management Server TechCenter](http://technet.microsoft.com/en-us/systemcenter/bb545936.aspx).

**Poznámka:** Služba SMS pomocí modulu Microsoft Baseline Security Analyzer poskytuje rozsáhlou podporu při zjišťování a nasazení aktualizací bulletinu zabezpečení. Tyto nástroje nemusí některé softwarové aktualizace zjistit. V takovém případě mohou správci použít funkce serveru SMS a nasměrovat aktualizace do určitých systémů. Další informace o tomto postupu najdete na webu [Nasazení aktualizací softwaru pomocí funkce Distribuce softwaru serveru SMS](http://go.microsoft.com/fwlink/?linkid=33341). Některé aktualizace zabezpečení vyžadují po restartování počítače oprávnění správce. Správci mohou k instalaci těchto aktualizací použít nástroj Elevated Rights Deployment Tool (k dispozici v sadě [SMS 2003 Administration Feature Pack](http://www.microsoft.com/downloads/en/details.aspx?familyid=7bd3a16e-1899-4e0b-bb99-1320e816167d&displaylang=en)).

**Nástroj Update Compatibility Evaluator a sada Application Compatibility Toolkit**

Aktualizace často zapisují do stejných souborů a nastavení registru požadovaných pro spouštění aplikací. To může způsobit nekompatibilitu a zvýšit dobu, po kterou trvá nasazení aktualizací zabezpečení. Testování a ověřování aktualizací systému Windows lze usnadnit pomocí součástí nástroje [Update Compatibility Evaluator](http://technet2.microsoft.com/windowsvista/en/library/4279e239-37a4-44aa-aec5-4e70fe39f9de1033.mspx?mfr=true), které jsou dodávány se sadou [Application Compatibility Toolkit](http://www.microsoft.com/downloads/details.aspx?familyid=24da89e9-b581-47b0-b45e-492dd6da2971&displaylang=en).

Sada Application Compatibility Toolkit (ACT) obsahuje nezbytné nástroje a dokumentaci pro posouzení a zmírnění problémů s kompatibilitou aplikací před nasazením systému Microsoft Windows Vista, služby Windows Update, aktualizací zabezpečení společnosti Microsoft nebo nové verze aplikace Windows Internet Explorer ve vašem prostředí.

### Další informace

#### Nástroj pro odstranění škodlivého softwaru systému Microsoft Windows

Společnost Microsoft vydává aktualizovanou verzi Nástroje pro odstranění škodlivého softwaru systému Microsoft Windows na webu Windows Update, Microsoft Update, ve službě Windows Server Update Services a na webu služby Stažení softwaru.

#### Aktualizace nesouvisející se zabezpečením na webu Microsoft Update (MU), Windows Update (WU) a ve službě Windows Server Update Services (WSUS)

Informace o aktualizacích nesouvisejících se zabezpečením na webu Windows Update a Microsoft Update naleznete na webové stránce:

-   [Článek 894199 znalostní báze Microsoft Knowledge Base](http://support.microsoft.com/kb/894199): Popis služeb Software Update Services a Windows Server Update Services se mění v obsahu. Zahrnuje celý obsah systému Windows.
-   [Aktualizace vydané v uplynulých měsících pro službu Windows Server Update Services](http://technet.microsoft.com/en-us/wsus/bb456965.aspx). Obsahuje přehled všech nových, revidovaných a opětovně vydaných aktualizací pro jiné produkty společnosti Microsoft, než je systém Microsoft Windows.

#### Microsoft Active Protections Program (MAPP)

Pro zlepšení ochrany dat svých zákazníků poskytuje společnost Microsoft informace o chybách v zabezpečení všem hlavním dodavatelům softwaru pro zabezpečení, a to vždy ještě před vydáním nové měsíční zprávy o aktualizaci zabezpečení. Dodavatelé softwaru pro zabezpečení tak mohou tyto informace o chybách v zabezpečení využít a poskytnout svým zákazníkům ochranu včasnou aktualizací svých programů a zařízení pro zabezpečení, jako jsou antivirové programy, síťové systémy pro detekci napadení či hostitelské systémy pro prevenci napadení. Informace o dostupnosti aktuálních prostředků aktivní ochrany od jednotlivých dodavatelů softwaru pro zabezpečení naleznete na stránkách aktivní ochrany jednotlivých partnerů programu MAPP. Seznam těchto partnerů naleznete na stránce [Microsoft Active Protections Program (MAPP) Partners](http://go.microsoft.com/fwlink/?linkid=215201).

#### Strategie zabezpečení a komunita

**Strategie instalace aktualizací**

Web [Doporučené postupy zabezpečení pro správu aktualizací (Security Guidance for Update Management)](http://go.microsoft.com/fwlink/?linkid=21168) obsahuje další informace o instalaci aktualizací zabezpečení podle doporučení společnosti Microsoft.

**Získání dalších aktualizací zabezpečení**

Aktualizace odstraňující další problémy se zabezpečením získáte v následujících umístěních:

-   Aktualizace zabezpečení jsou k dispozici na webu služby [Stažení softwaru (Microsoft Download Center)](http://go.microsoft.com/fwlink/?linkid=21129). Nejsnadněji je naleznete hledáním podle klíčových slov aktualizace zabezpečení.
-   Aktualizace pro klientské platformy jsou k dispozici na webu [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747).
-   Aktualizace zabezpečení nabízené tento měsíc na webu Windows Update jsou k dispozici na webu služby Stažení softwaru v souborech obrazu ISO disku CD s vydanými aktualizacemi zabezpečení a kritickými aktualizacemi. Další informace získáte v [článku 913086 znalostní báze Microsoft Knowledge Base](http://support.microsoft.com/kb/913086).

**Komunita odborníků v oblasti zabezpečení**

Můžete se zde naučit, jak zlepšit zabezpečení a jak optimalizovat infrastrukturu IT. Také můžete s dalšími členy komunity IT Pro diskutovat o bezpečnostních tématech na webu [Komunita odborníků v oblasti zabezpečení (IT Pro Security Community)](http://go.microsoft.com/fwlink/?linkid=21164).

#### Poděkování

Společnost Microsoft tímto [děkuje](http://go.microsoft.com/fwlink/?linkid=21127) za spolupráci při ochraně zákazníků:

-   Tarjei Mandtovi ze společnosti [Norman](http://www.norman.com) za oznámení 14 chyb popsaných v bulletinu MS11-054.
-   Liangu Yinovi, profesorům Sihanu Qingovi a Weipingu Wenovi, a Hushengu Zhouovi [z fakulty zabezpečení informací pekingské univerzity](http://www.ss.pku.edu.cn/en/) za oznámení chyby popsané v bulletinu MS11-054.
-   Matthewu 'j00ru' Jurczykovi ze společnosti [Hispasec](http://www.hispasec.com/) [Virustotal](http://www.virustotal.com/) za oznámení pěti chyb popsaných v bulletinu MS11-056.

#### Technická podpora

-   Uvedený software byl testován za účelem zjištění, kterých verzí se chyba týká. U dalších verzí skončila časově omezená podpora. Pokud chcete zjistit dobu, po kterou je pro určitou verzi softwaru poskytována podpora, navštivte web [Zásady poskytování technické podpory pro produkty společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=21742).
-   Zákazníci mohou získat technickou podporu na webu [služby technické podpory společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=21131). Hovory související s aktualizacemi zabezpečení jsou bezplatné. Další informace o dostupných možnostech technické podpory naleznete na webu [Pomoc a podpora společnosti Microsoft](http://support.microsoft.com/).
-   Mezinárodní zákazníci získají podporu u místních zastoupení společnosti Microsoft. Technická podpora související s aktualizacemi zabezpečení je bezplatná. Další informace o možnostech kontaktování společnosti Microsoft v případě potřeby technické podpory získáte na [webu mezinárodní technické podpory](http://go.microsoft.com/fwlink/?linkid=21155).

#### Zřeknutí se záruky

Informace ve znalostní bázi Microsoft Knowledge Base jsou poskytovány tak, jak jsou, bez jakékoli záruky. Společnost Microsoft neposkytuje žádné záruky, výslovně uvedené či mlčky předpokládané, včetně záruk obchodovatelnosti a vhodnosti pro určitý účel. Společnost Microsoft ani její dodavatelé nenesou v žádném případě zodpovědnost za žádné škody, včetně přímých, nepřímých, náhodných či následných škod, ztráty zisku či zvláštních škod, a to ani v případě, že byli na možnost takových škod upozorněni. V některých zemích a právních řádech není dovoleno vyloučit nebo omezit odpovědnost, proto se výše uvedené omezení na vás nemusí vztahovat.

#### Revize

-   V1.0 (12. července 2011): Souhrnný bulletin byl publikován.

*Built at 2014-04-18T01:50:00Z-07:00*
