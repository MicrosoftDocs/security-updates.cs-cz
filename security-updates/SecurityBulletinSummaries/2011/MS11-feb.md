---
TOCTitle: 'MS11-FEB'
Title: 'Souhrnný bulletin zabezpečení společnosti Microsoft, únor 2011'
ms:assetid: 'ms11-feb'
ms:contentKeyID: 61224009
ms:mtpsurl: 'https://technet.microsoft.com/cs-CZ/library/ms11-feb(v=Security.10)'
---

 

Souhrnný bulletin zabezpečení společnosti Microsoft, únor 2011
==============================================================

Publikováno: 8. února 2011 | Aktualizováno: 18. března 2011

**Verze:** 4.0

Tento souhrnný bulletin uvádí bulletiny zabezpečení vydané v únoru 2011.

Spolu s vydáním bulletinů pro únor 2011 nahrazuje tento souhrnný bulletin předběžné oznámení o bulletinech vydané 3. února 2011. Další informace o službě předběžného oznámení o bulletinech naleznete v části [Předběžné oznámení o bulletinech zabezpečení společnosti Microsoft](http://technet.microsoft.com/security/bulletin/advance).

Informace o tom, jak dostávat automatická oznámení o vydání nových bulletinů zabezpečení společnosti Microsoft, naleznete na webu [Zasílání technických oznámení o zabezpečení společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=21163).

Pro zodpovězení zákaznických dotazů týkajících se těchto bulletinů uspořádá společnost Microsoft 9. února 2011 v 11:00 časového pásma Tichomoří (USA a Kanada) webové vysílání. [Zaregistrujte se pro webové vysílání týkající se únorových bulletinů zabezpečení](https://msevents.microsoft.com/cui/webcasteventdetails.aspx?eventid=1032455047&eventcategory=4). Po tomto datu je webové vysílání dostupné na požádání. Další informace získáte v [souhrnných bulletinech zabezpečení společnosti Microsoft a webovém vysílání](http://technet.microsoft.com/security/bulletin/summary).

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
<th style="border:1px solid black;" >Software obsahující tuto chybu</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=208304">MS11-003</a></td>
<td style="border:1px solid black;"><strong>Kumulativní aktualizace zabezpečení pro aplikaci Internet Explorer (2482017)</strong><br />
<br />
Tato aktualizace zabezpečení řeší dvě chyby zabezpečení oznámené soukromými osobami a dvě veřejně známé chyby zabezpečení v aplikaci Internet Explorer. Tyto chyby zabezpečení umožňují vzdálené spuštění kódu, pokud uživatel zobrazí speciálně vytvořenou webovou stránku v aplikaci Internet Explorer nebo pokud otevře pravý soubor HTML, který načte speciálně vytvořený soubor knihovny. Útočník, který by úspěšně zneužil některou z těchto chyb zabezpečení, by mohl získat stejná uživatelská práva, jaká má místní uživatel. Uživatelé, jejichž účty jsou konfigurovány tak, aby měli v systému méně uživatelských práv, by byli vystaveni menšímu riziku než uživatelé s uživatelskými právy správce.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritický</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Internet Explorer</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=208146">MS11-006</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení grafického zpracování prostředí systému Windows umožňuje vzdálené spuštění kódu (2483185)</strong><br />
<br />
Tato aktualizace zabezpečení řeší veřejně známou chybu zabezpečení v grafickém procesoru prostředí systému Windows. Tato chyba zabezpečení umožňuje vzdálené spuštění kódu, pokud uživatel zobrazí speciálně vytvořený obrázek miniatury. Útočník, který by úspěšně zneužil tuto chybu zabezpečení, by mohl získat stejná uživatelská práva, jaká má přihlášený uživatel. Uživatelé, jejichž účty jsou konfigurovány tak, aby měli v systému méně uživatelských práv, by byli vystaveni menšímu riziku než uživatelé s uživatelskými právy správce.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritický</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=208059">MS11-007</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení v ovladači písma OpenType formátu CFF (Compact Font Format) umožňuje vzdálené spuštění kódu (2485376)</strong><br />
<br />
Tato aktualizace zabezpečení řeší soukromě oznámenou chybu zabezpečení v ovladači písma OpenType formátu (Compact Font Format). Tato chyba zabezpečení by mohla umožnit vzdálené spuštění kódu, pokud by uživatel zobrazil obsah ve speciálně vytvořeném písmu CFF. Útočník nemůže žádným způsobem přinutit uživatele k zobrazení speciálně vytvořeného obsahu. Místo toho by útočník musel přesvědčit uživatele, aby navštívili takový web. K tomu se obvykle používá odkaz v e-mailu nebo zpráva programu pro zasílání rychlých zpráv, na které uživatelé kliknou a přejdou tak na útočníkův web.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritický</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=208522">MS11-004</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení služby FTP v Internetové informační službě (IIS) umožňuje vzdálené spuštění kódu (2489256)</strong><br />
<br />
Tato aktualizace zabezpečení řeší veřejně známou chybu zabezpečení služby FTP v Internetové informační službě Microsoft (IIS). Chyba zabezpečení umožňuje vzdálené spuštění kódu, pokud server FTP obdrží speciálně vytvořený příkaz protokolu FTP. Služba FTP není ve výchozím nastavení v IIS nainstalována.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Vysoký</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Může vyžadovat restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=207843">MS11-005</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení služby Active Directory může způsobit odmítnutí služby (2478953)</strong><br />
<br />
Tato aktualizace zabezpečení řeší veřejně známou chybu zabezpečení služby Active Directory. Tato chyba zabezpečení by mohla způsobit odmítnutí služby, pokud by útočník odeslal na server s ohroženou službou Active Directory speciálně vytvořený paket. Aby mohl útočník tuto chybu zabezpečení zneužít, musí mít platná oprávnění místního správce počítače připojeného do domény.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Vysoký</a><br />
Odmítnutí služby</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=204799">MS11-008</a></td>
<td style="border:1px solid black;"><strong>Chyby zabezpečení v aplikaci Microsoft Visio umožňují vzdálené spuštění kódu (2451879)</strong><br />
<br />
Tato aktualizace zabezpečení řeší dvě soukromými osobami oznámené chyby zabezpečení v aplikaci Microsoft Visio. Chyby umožňují vzdálené spuštění kódu, pokud uživatel otevře speciálně vytvořený soubor aplikace Visio. Útočník, který by úspěšně zneužil některou z těchto chyb zabezpečení, by mohl získat stejná uživatelská práva, jaká má přihlášený uživatel. Uživatelé, jejichž účty jsou konfigurovány tak, aby měli v systému méně uživatelských práv, by byli vystaveni menšímu riziku než uživatelé s uživatelskými právy správce.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Vysoký</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Může vyžadovat restartování</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=207839">MS11-009</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení ve skriptovacích strojích jazyků JScript a VBScript umožňuje přístup k informacím (2475792)</strong><br />
<br />
Tato aktualizace zabezpečení řeší chybu zabezpečení ve skriptovacích strojích jazyků JScript a VBScript oznámenou soukromou osobou. Uvedená chyba zabezpečení umožňuje zpřístupnění informací, pokud uživatel navštíví speciálně vytvořenou webovou stránku. Útočník nemůže žádným způsobem přinutit uživatele k návštěvě takovýchto webů. Místo toho by útočník musel přesvědčit uživatele, aby navštívili takový web. K tomu se obvykle používá odkaz v e-mailu nebo zpráva programu pro zasílání rychlých zpráv, na které uživatelé kliknou, a přejdou tak na útočníkův web.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Vysoký</a><br />
Přístup k informacím</td>
<td style="border:1px solid black;">Může vyžadovat restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=207840">MS11-010</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení v podsystému Windows CSRSS (Client/Server Run-time Subsystem) umožňuje zvýšení úrovně oprávnění (2476687)</strong><br />
<br />
Tato aktualizace zabezpečení řeší soukromou osobou oznámenou chybu zabezpečení v&amp;nbsp;podsystému Microsoft Windows CSRSS (Client/Server Run-time Subsystem) v&amp;nbsp;systémech Windows&amp;nbsp;XP a&amp;nbsp;Windows Server&amp;nbsp;2003.<br />
<br />
Tato chyba zabezpečení umožňuje zvýšit úroveň oprávnění, pokud se útočník přihlásí do systému uživatele a spustí speciálně vytvořenou aplikaci, která běží i po odhlášení útočníka, přičemž získává přihlašovací údaje dalších uživatelů. Tuto chybu může zneužít pouze útočník s platnými pověřeními pro přihlášení, která by mu umožňovala se místně přihlásit. Tuto chybu zabezpečení nemohou zneužít vzdálení ani anonymní uživatelé.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Vysoký</a><br />
Zvýšení úrovně oprávnění</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=208365">MS11-011</a></td>
<td style="border:1px solid black;"><strong>Chyby zabezpečení jádra systému Windows umožňují zvýšení oprávnění (2393802)</strong><br />
<br />
Tato aktualizace zabezpečení řeší jednu veřejně známou a jednu soukromou osobou oznámenou chybu zabezpečení systému Microsoft Windows. Tyto chyby zabezpečení by mohly umožnit zvýšení úrovně oprávnění, pokud by se útočník místně přihlásil k systému a spustil speciálně vytvořenou aplikaci. Tyto chyby zabezpečení může zneužít pouze útočník s platnými pověřeními pro přihlášení, která by mu umožňovala se místně přihlásit. Uvedené chyby zabezpečení nemohou zneužít vzdálení ani anonymní uživatelé.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Vysoký</a><br />
Zvýšení úrovně oprávnění</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=208362">MS11-012</a></td>
<td style="border:1px solid black;"><strong>Chyby zabezpečení v ovladačích režimu jádra systému Windows umožňují zvýšení úrovně oprávnění (2479628)</strong><br />
<br />
Tato aktualizace zabezpečení řeší pět chyb zabezpečení v systému Microsoft Windows oznámených soukromými osobami. Tyto chyby zabezpečení by mohly umožnit zvýšení úrovně oprávnění, pokud by se útočník místně přihlásil k systému a spustil speciálně vytvořenou aplikaci. Tyto chyby zabezpečení může zneužít pouze útočník s platnými pověřeními pro přihlášení, která by mu umožňovala se místně přihlásit. Uvedené chyby zabezpečení nemohou zneužít vzdálení ani anonymní uživatelé.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Vysoký</a><br />
Zvýšení úrovně oprávnění</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=208523">MS11-013</a></td>
<td style="border:1px solid black;"><strong>Chyby zabezpečení v protokolu Kerberos umožňují zvýšení úrovně oprávnění (2496930)</strong><br />
<br />
Tato aktualizace zabezpečení řeší jednu veřejně známou a jednu soukromou osobou oznámenou chybu zabezpečení systému Microsoft Windows. Závažnější z těchto chyb zabezpečení by mohla umožnit zvýšení úrovně oprávnění, pokud by místní ověřený útočník nainstaloval škodlivou službu do počítače připojeného do domény.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Vysoký</a><br />
Zvýšení úrovně oprávnění</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=208395">MS11-014</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení ve službě LSASS (Local Security Authority Subsystem Service) umožňuje zvýšení úrovně místního oprávnění (2478960)</strong><br />
<br />
Tato aktualizace zabezpečení řeší soukromou osobou oznámenou chybu zabezpečení služby LSASS (Local Security Authority Subsystem Service) systémů Windows XP a Windows Server 2003.<br />
<br />
Tato chyba zabezpečení by mohla způsobit zvýšení úrovně oprávnění, pokud by se útočník přihlásil k systému a spustil speciálně vytvořenou aplikaci. Tuto chybu může zneužít pouze útočník s platnými pověřeními pro přihlášení, která by mu umožňovala se místně přihlásit. Tuto chybu zabezpečení nemohou zneužít vzdálení ani anonymní uživatelé.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Vysoký</a><br />
Zvýšení úrovně oprávnění</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
</tbody>
</table>
<p></p>
  
Index zneužitelnosti  
--------------------
  
<span></span>
Následující tabulka uvádí hodnocení zneužitelnosti každé chyby zabezpečení uvedené v tomto měsíci. Chyby zabezpečení jsou řazeny v pořadí zmenšující se úrovně posouzení zneužitelnosti, jinak než tomu je u řazení podle čísla chyb. Uvedeny jsou pouze chyby zabezpečení ohodnocené stupněm závažnosti Kritický nebo Vysoký.
  
**Jak pracovat s touto tabulkou**
  
V této tabulce zjistíte, jaká je pravděpodobnost vydání funkčního zneužitelného kódu během 30 dní od vydání tohoto bulletinu zabezpečení pro všechny aktualizace zabezpečení, které bude třeba nainstalovat. Všechna níže uvedená hodnocení zvažte na základě vaší specifické konfigurace a podle závěrů hodnocení nastavte priority pro zavádění jednotlivých aktualizací. Další informace o významu těchto hodnocení a způsobu jejich stanovení najdete v indexu zneužitelnosti [Microsoft Exploitability Index](http://technet.microsoft.com/en-us/security/cc998259.aspx).

 
<p></p>
<table style="border:1px solid black;">
<thead>
<tr class="header">
<th style="border:1px solid black;" >ID bulletinu</th>
<th style="border:1px solid black;" >Název chyby zabezpečení</th>
<th style="border:1px solid black;" >ID CVE</th>
<th style="border:1px solid black;" >Hodnocení indexu zneužitelnosti</th>
<th style="border:1px solid black;" >Hlavní poznámky</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=208146">MS11-006</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se přetečení při grafickém zpracování prostředí systému Windows</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3970">CVE-2010-3970</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Je pravděpodobné vytvoření kódu konsistentního zneužití</td>
<td style="border:1px solid black;"><strong>Tato chyba zabezpečení je veřejně známá a zneužitelný kód je dostupný</strong></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=208304">MS11-003</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se poškození paměti subsystému CSS</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3971">CVE-2010-3971</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Je pravděpodobné vytvoření kódu konsistentního zneužití</td>
<td style="border:1px solid black;"><strong>Tato chyba zabezpečení je veřejně známá a dochází k jejímu zneužití v prostředí Internetu</strong></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=208365">MS11-011</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se nesprávné interakce ovladače s jádrem systému Windows</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-4398">CVE-2010-4398</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Je pravděpodobné vytvoření kódu konsistentního zneužití</td>
<td style="border:1px solid black;"><strong>Tato chyba zabezpečení je veřejně známá.</strong></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=207840">MS11-010</a></td>
<td style="border:1px solid black;">Chyba zabezpečení umožňující zvýšení úrovně oprávnění subsystému CSRSS</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0030">CVE-2011-0030</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Je pravděpodobné vytvoření kódu konsistentního zneužití</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=208304">MS11-003</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se poškození neinicializované paměti</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0035">CVE-2011-0035</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Je pravděpodobné vytvoření kódu konsistentního zneužití</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=208304">MS11-003</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se poškození neinicializované paměti</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0036">CVE-2011-0036</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Je pravděpodobné vytvoření kódu konsistentního zneužití</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=208395">MS11-014</a></td>
<td style="border:1px solid black;">Chyba zabezpečení při ověřování délky službou LSASS</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0039">CVE-2011-0039</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Je pravděpodobné vytvoření kódu konsistentního zneužití</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=208523">MS11-013</a></td>
<td style="border:1px solid black;">Chyba zabezpečení kontrolního součtu bez klíče protokolu Kerberos</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0043">CVE-2011-0043</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Je pravděpodobné vytvoření kódu konsistentního zneužití</td>
<td style="border:1px solid black;"><strong>Tato chyba zabezpečení je veřejně známá.</strong></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=208365">MS11-011</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se celočíselného oříznutí jádra systému Windows</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0045">CVE-2011-0045</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Je pravděpodobné vytvoření kódu konsistentního zneužití</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=208362">MS11-012</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se nesprávného ověřování vstupu uživatele subsystému Win32k</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0086">CVE-2011-0086</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Je pravděpodobné vytvoření kódu konsistentního zneužití</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=208362">MS11-012</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se nedostatečného ověřování vstupu uživatele subsystému Win32k</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0087">CVE-2011-0087</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Je pravděpodobné vytvoření kódu konsistentního zneužití</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=208362">MS11-012</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se nejasnosti ukazatele třídy okna subsystému Win32k</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0088">CVE-2011-0088</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Je pravděpodobné vytvoření kódu konsistentního zneužití</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=208362">MS11-012</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se nesprávného ověření ukazatele třídy okna subsystému Win32k</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0089">CVE-2011-0089</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Je pravděpodobné vytvoření kódu konsistentního zneužití</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=208362">MS11-012</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se poškození paměti subsystému Win32k</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0090">CVE-2011-0090</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Je pravděpodobné vytvoření kódu konsistentního zneužití</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=204799">MS11-008</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se poškození paměti objektů Visio</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0092">CVE-2011-0092</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Je pravděpodobné vytvoření kódu konsistentního zneužití</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=204799">MS11-008</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se poškození paměti objektů datového typu Visio</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0093">CVE-2011-0093</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Je pravděpodobné vytvoření kódu konsistentního zneužití</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=208522">MS11-004</a></td>
<td style="border:1px solid black;">Chyba zabezpečení typu přetečení haldy vyrovnávací paměti služby IIS FTP</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3972">CVE-2010-3972</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">2</a> - Je pravděpodobné vytvoření kódu nekonsistentního zneužití</td>
<td style="border:1px solid black;"><strong>Tato chyba zabezpečení je veřejně známá a kód PoC může být dostupný</strong></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=208059">MS11-007</a></td>
<td style="border:1px solid black;">Chyba zabezpečení kódování znaků písma OpenType</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0033">CVE-2011-0033</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">2</a> - Je pravděpodobné vytvoření kódu nekonsistentního zneužití</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=207839">MS11-009</a></td>
<td style="border:1px solid black;">Chyba zabezpečení přístupu k informacím ve skriptovacích strojích</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0031">CVE-2011-0031</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">3</a> - Vytvoření kódu funkčního zneužití není pravděpodobné</td>
<td style="border:1px solid black;">Jedná se o chybu zabezpečení typu zpřístupnění informací.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=207843">MS11-005</a></td>
<td style="border:1px solid black;">Chyba zabezpečení při ověřování služby Active Directory SPN</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0040">CVE-2011-0040</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">3</a> - Vytvoření kódu funkčního zneužití není pravděpodobné</td>
<td style="border:1px solid black;"><strong>Tato chyba zabezpečení je veřejně známá.</strong><br />
<br />
Jedná se o chybu zabezpečení, která způsobuje odmítnutí služby.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=208523">MS11-013</a></td>
<td style="border:1px solid black;">Chyba zabezpečení související s falšováním obsahu protokolu Kerberos</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0091">CVE-2011-0091</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">3</a> - Vytvoření kódu funkčního zneužití není pravděpodobné</td>
<td style="border:1px solid black;">Jedná se o chybu zabezpečení umožňující pouze vkládání falešného obsahu.</td>
</tr>
</tbody>
</table>
<p></p>
  
Software obsahující tuto chybu a umístění aktualizací ke stažení  
----------------------------------------------------------------
  
<span></span>
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
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
</tr>
<tr>
<th colspan="12" style="border:1px solid black;">
Windows XP  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS11-003**](http://go.microsoft.com/fwlink/?linkid=208304)
</td>
<td style="border:1px solid black;">
[**MS11-006**](http://go.microsoft.com/fwlink/?linkid=208146)
</td>
<td style="border:1px solid black;">
[**MS11-007**](http://go.microsoft.com/fwlink/?linkid=208059)
</td>
<td style="border:1px solid black;">
[**MS11-004**](http://go.microsoft.com/fwlink/?linkid=208522)
</td>
<td style="border:1px solid black;">
[**MS11-005**](http://go.microsoft.com/fwlink/?linkid=207843)
</td>
<td style="border:1px solid black;">
[**MS11-009**](http://go.microsoft.com/fwlink/?linkid=207839)
</td>
<td style="border:1px solid black;">
[**MS11-010**](http://go.microsoft.com/fwlink/?linkid=207840)
</td>
<td style="border:1px solid black;">
[**MS11-011**](http://go.microsoft.com/fwlink/?linkid=208365)
</td>
<td style="border:1px solid black;">
[**MS11-012**](http://go.microsoft.com/fwlink/?linkid=208362)
</td>
<td style="border:1px solid black;">
[**MS11-013**](http://go.microsoft.com/fwlink/?linkid=208523)
</td>
<td style="border:1px solid black;">
[**MS11-014**](http://go.microsoft.com/fwlink/?linkid=208395)
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
[**Kritický**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Žádné
</td>
<td style="border:1px solid black;">
Žádné
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
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
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
Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=ae343de6-ec61-4891-b136-cfc4234d97d9)  
(Kritický)  
[Aplikace Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=85bf88b7-2dd9-4204-8492-b2c1d8d2264e)  
(Kritický)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=c72fbb97-2313-45f6-842d-99db373822dd)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=bbea7ead-6c5c-4da8-aa03-a40325fd2de3)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=f86e9e64-801a-431a-b24e-772011dfa66d)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=cfa10178-9859-4e03-bedc-e3f5297a0251)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=a511d33a-9ae0-46ee-a225-9d97390de7d1)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=56f4f43e-c313-49dc-a278-e3e8a83a907e)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=486d1969-6814-4556-8dc0-5bfbaee528b0)  
(KB2478971)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=541f228f-79b3-402a-8ff9-366c1e595227)  
(Vysoký)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=d431100d-a627-4ea0-b75b-2d4157e38df2)  
(Kritický)  
[Aplikace Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=a795de21-13f4-4035-a4d5-4257ddc92fe7)  
(Kritický)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=69dfa24b-7c56-4521-850c-1485b062154a)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=bcb7217e-624a-4d61-86a1-f2440a1afd57)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=074396f0-a68c-4190-8dac-0b883d56e3f1)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=9f0b7b77-5b90-4a4b-97a4-0c1ce6a70126)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e7273a85-ce96-464b-8c4f-2710701213e3)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e80db313-b470-4d71-bc34-70bfbfb6579f)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=a210c796-7077-4617-a9a8-9ea99fe11a5e)  
(KB2478971)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=82189bf2-3f34-4949-92da-eea98036d18e)  
(Vysoký)
</td>
</tr>
<tr>
<th colspan="12" style="border:1px solid black;">
Windows Server 2003
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS11-003**](http://go.microsoft.com/fwlink/?linkid=208304)
</td>
<td style="border:1px solid black;">
[**MS11-006**](http://go.microsoft.com/fwlink/?linkid=208146)
</td>
<td style="border:1px solid black;">
[**MS11-007**](http://go.microsoft.com/fwlink/?linkid=208059)
</td>
<td style="border:1px solid black;">
[**MS11-004**](http://go.microsoft.com/fwlink/?linkid=208522)
</td>
<td style="border:1px solid black;">
[**MS11-005**](http://go.microsoft.com/fwlink/?linkid=207843)
</td>
<td style="border:1px solid black;">
[**MS11-009**](http://go.microsoft.com/fwlink/?linkid=207839)
</td>
<td style="border:1px solid black;">
[**MS11-010**](http://go.microsoft.com/fwlink/?linkid=207840)
</td>
<td style="border:1px solid black;">
[**MS11-011**](http://go.microsoft.com/fwlink/?linkid=208365)
</td>
<td style="border:1px solid black;">
[**MS11-012**](http://go.microsoft.com/fwlink/?linkid=208362)
</td>
<td style="border:1px solid black;">
[**MS11-013**](http://go.microsoft.com/fwlink/?linkid=208523)
</td>
<td style="border:1px solid black;">
[**MS11-014**](http://go.microsoft.com/fwlink/?linkid=208395)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Celkový stupeň závažnosti**
</td>
<td style="border:1px solid black;">
[**Mírný**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritický**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
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
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
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
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=5e0f4bf2-f727-483a-af3a-9a2abf0c36bb)  
(Mírný)  
[Aplikace Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=45e504d4-c17d-4b73-b08e-d9c0cb3f4918)  
(Mírný)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=74238e08-fae2-4f17-ac72-681226a53a40)  
(Mírný)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2aa94528-5063-427b-97f7-2a0a55cbb6bf)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=a99c2b13-db81-4f18-9cf7-c20614ba0132)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Active Directory](http://www.microsoft.com/downloads/details.aspx?familyid=651c1f4f-4e69-4d17-8aa2-72681dfc5463)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=aed08b96-24cc-4e23-8fd5-c7e52f8ef41a)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=6bf2eeec-8225-477f-a606-263d3ee434d6)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=54fe2669-8a63-4d96-8b82-5b10f45b293e)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8a1e2675-0bf0-4d94-b48a-6e846dd6d9f5)  
(KB2478971)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4e31e6b1-577e-468e-9c94-67227d2273c2)  
(Vysoký)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=0592b520-88d1-45bc-8b15-d3f0c8fa2181)  
(Mírný)  
[Aplikace Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=29adcfb5-540f-4980-b2ca-9a22aa7bba13)  
(Mírný)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=ebef4869-9812-46ce-9c01-2fb8c866ec90)  
(Mírný)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=6e740922-6ce4-46ec-a35e-e94201a9e398)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=aeed45fb-9395-4c2b-a674-e38b04fe0914)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Active Directory](http://www.microsoft.com/downloads/details.aspx?familyid=ec962b0e-e951-4e70-8d97-8c2afd360c28)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ca7879e1-e295-445d-a658-0a31be1928cc)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ec544894-ee98-4a2b-ac4d-33b0c3754213)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4632e1ce-6ae8-431c-9104-9a8840e5ac63)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e79bbbd4-8d5a-4c4c-8427-21c14400f041)  
(KB2478971)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=76e3c229-d812-433c-ad05-7cbd1f9c6a6d)  
(Vysoký)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 SP2 pro systémy s procesorem Itanium
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=b2298b32-238a-4970-bc1f-2ede51a6c361)  
(Mírný)  
[Aplikace Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=c41a0094-204b-4d05-ab39-a32915201af1)  
(Mírný)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=a4f9ec46-35b2-44c9-abf6-647f7a474b99)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=bc09e42b-2eed-41b3-a03f-cb8cc94adfee)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Active Directory](http://www.microsoft.com/downloads/details.aspx?familyid=4ac66eae-e6d8-4e8b-b4ea-e7a77cc74db0)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=50855101-a15c-4c81-ad81-a7fe3f1d2026)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=fcd48499-1bb4-4304-b9cc-27d9d92e11cd)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=a09c3e6e-c55c-492a-b7ad-3e3d35711643)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=856fbcc2-ead9-4ec1-92dd-988e6d22dae9)  
(KB2478971)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=a0cde8d8-7c85-4fcb-bcf7-205064970b41)  
(Vysoký)
</td>
</tr>
<tr>
<th colspan="12" style="border:1px solid black;">
Windows Vista
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS11-003**](http://go.microsoft.com/fwlink/?linkid=208304)
</td>
<td style="border:1px solid black;">
[**MS11-006**](http://go.microsoft.com/fwlink/?linkid=208146)
</td>
<td style="border:1px solid black;">
[**MS11-007**](http://go.microsoft.com/fwlink/?linkid=208059)
</td>
<td style="border:1px solid black;">
[**MS11-004**](http://go.microsoft.com/fwlink/?linkid=208522)
</td>
<td style="border:1px solid black;">
[**MS11-005**](http://go.microsoft.com/fwlink/?linkid=207843)
</td>
<td style="border:1px solid black;">
[**MS11-009**](http://go.microsoft.com/fwlink/?linkid=207839)
</td>
<td style="border:1px solid black;">
[**MS11-010**](http://go.microsoft.com/fwlink/?linkid=207840)
</td>
<td style="border:1px solid black;">
[**MS11-011**](http://go.microsoft.com/fwlink/?linkid=208365)
</td>
<td style="border:1px solid black;">
[**MS11-012**](http://go.microsoft.com/fwlink/?linkid=208362)
</td>
<td style="border:1px solid black;">
[**MS11-013**](http://go.microsoft.com/fwlink/?linkid=208523)
</td>
<td style="border:1px solid black;">
[**MS11-014**](http://go.microsoft.com/fwlink/?linkid=208395)
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
[**Kritický**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritický**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Žádné
</td>
<td style="border:1px solid black;">
Žádné
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
<td style="border:1px solid black;">
Žádné
</td>
<td style="border:1px solid black;">
Žádné
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista Service Pack 1 a Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=b176777e-4897-4cf1-9fc0-dd608930bb4c)  
(Kritický)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=77971c3c-55ec-4a9c-bcb8-8fb8c61431e3)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 a Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=0c18ecca-afb9-4738-bc7b-76a0e815dfb8)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 a Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d60a2098-7351-4fce-83b2-2c1c3a24faa0)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Služba Microsoft FTP Service 7.0 pro službu IIS 7.0](http://www.microsoft.com/downloads/details.aspx?familyid=c09ccc72-8f94-416b-9a7f-ed16e90342a2)<sup>[1]</sup>
(Vysoký)  
[Služba Microsoft FTP Service 7.5 pro službu IIS 7.0](http://www.microsoft.com/downloads/details.aspx?familyid=da9b7982-1c6b-45ac-8dd0-d7101bb83949)<sup>[1]</sup>
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 a Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=66978514-bb7f-42cc-9360-2fd1c686f4e6)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 a Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=6fb7ebcc-2052-457b-b5bc-1bbcb17696b9)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 1 a Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=20ad0136-c6df-4c7b-811f-d6b3dd9e2c56)  
(Kritický)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=d3580784-aada-4118-b7f2-3a23aec2ed04)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 a Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=62dc454f-4b1e-4ac0-8ffe-6c73112f8d4d)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 a Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=065ad8fe-1caf-488e-a2e1-96db29f2fa57)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Služba Microsoft FTP Service 7.0 pro službu IIS 7.0](http://www.microsoft.com/downloads/details.aspx?familyid=e88d072f-0f5f-4c85-ad2f-91b9b8bf6b3a)<sup>[1]</sup>
(Vysoký)  
[Služba Microsoft FTP Service 7.5 pro službu IIS 7.0](http://www.microsoft.com/downloads/details.aspx?familyid=6e4b9878-b5d2-4025-8839-b41515932cf2)<sup>[1]</sup>
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 a Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8fdb8c37-1b22-457b-bdc0-21f6a5061dd3)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 a Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=88d68757-1ab0-4585-9578-52a474b10882)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
</tr>
<tr>
<th colspan="12" style="border:1px solid black;">
Windows Server 2008
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS11-003**](http://go.microsoft.com/fwlink/?linkid=208304)
</td>
<td style="border:1px solid black;">
[**MS11-006**](http://go.microsoft.com/fwlink/?linkid=208146)
</td>
<td style="border:1px solid black;">
[**MS11-007**](http://go.microsoft.com/fwlink/?linkid=208059)
</td>
<td style="border:1px solid black;">
[**MS11-004**](http://go.microsoft.com/fwlink/?linkid=208522)
</td>
<td style="border:1px solid black;">
[**MS11-005**](http://go.microsoft.com/fwlink/?linkid=207843)
</td>
<td style="border:1px solid black;">
[**MS11-009**](http://go.microsoft.com/fwlink/?linkid=207839)
</td>
<td style="border:1px solid black;">
[**MS11-010**](http://go.microsoft.com/fwlink/?linkid=207840)
</td>
<td style="border:1px solid black;">
[**MS11-011**](http://go.microsoft.com/fwlink/?linkid=208365)
</td>
<td style="border:1px solid black;">
[**MS11-012**](http://go.microsoft.com/fwlink/?linkid=208362)
</td>
<td style="border:1px solid black;">
[**MS11-013**](http://go.microsoft.com/fwlink/?linkid=208523)
</td>
<td style="border:1px solid black;">
[**MS11-014**](http://go.microsoft.com/fwlink/?linkid=208395)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Celkový stupeň závažnosti**
</td>
<td style="border:1px solid black;">
[**Mírný**](http://go.microsoft.com/fwlink/?linkid=21140)
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
<td style="border:1px solid black;">
Žádné
</td>
<td style="border:1px solid black;">
Žádné
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
<td style="border:1px solid black;">
Žádné
</td>
<td style="border:1px solid black;">
Žádné
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 pro 32bitové systémy a Windows Server 2008 pro 32bitové systémy Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=ee61f0dd-9797-4e11-8281-a05b201d0c0b)\*\*  
(Mírný)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=ef1ae382-8835-4f60-83bd-e84a3400d55c)\*\*  
(Mírný)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro 32bitové systémy a Windows Server 2008 pro 32bitové systémy Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=253c47a0-69ac-437a-ad3e-778c37fa37cb)\*\*  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro 32bitové systémy a Windows Server 2008 pro 32bitové systémy Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=88ba83b9-c14e-499a-8335-04bac1c49c0c)\*  
(Kritický)
</td>
<td style="border:1px solid black;">
[Služba Microsoft FTP Service 7.0 pro službu IIS 7.0](http://www.microsoft.com/downloads/details.aspx?familyid=3cc55af7-5cd9-4923-8ec5-462ff201d734)<sup>[1]</sup>\*  
(Vysoký)  
[Služba Microsoft FTP Service 7.5 pro službu IIS 7.0](http://www.microsoft.com/downloads/details.aspx?familyid=4dfa0a25-b7e3-4fb6-a351-58ec3f8a8435)<sup>[1]</sup>\*  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro 32bitové systémy a Windows Server 2008 pro 32bitové systémy Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4b37418a-e044-415e-b566-4507f157934a)\*  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro 32bitové systémy a Windows Server 2008 pro 32bitové systémy Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=80494972-db45-475f-97cd-dac46b9486a1)\*  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 pro systémy s procesorem x64 a Windows Server 2008 pro systémy s procesorem x64 Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=558bc86a-a49d-4d6c-b5e4-f12956f6b61b)\*\*  
(Mírný)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=5607df02-93fa-45fe-a928-e5f6329851f3)\*\*  
(Mírný)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem x64 a Windows Server 2008 pro systémy s procesorem x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ec7101aa-96c2-4931-a3e4-0c55cbc74d9c)\*\*  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem x64 a Windows Server 2008 pro systémy s procesorem x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7c74d7f4-6372-4809-89b8-c79b05e54cdd)\*  
(Kritický)
</td>
<td style="border:1px solid black;">
[Služba Microsoft FTP Service 7.0 pro službu IIS 7.0](http://www.microsoft.com/downloads/details.aspx?familyid=f485b30d-dcaf-47c3-ac62-982b14670a1f)<sup>[1]</sup>\*  
(Vysoký)  
[Služba Microsoft FTP Service 7.5 pro službu IIS 7.0](http://www.microsoft.com/downloads/details.aspx?familyid=a98a74c1-0c91-446d-b822-fe57ff06d90b)<sup>[1]</sup>\*  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem x64 a Windows Server 2008 pro systémy s procesorem x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=163d3aca-3703-452e-b1cb-73932e2bcf8c)\*  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem x64 a Windows Server 2008 pro systémy s procesorem x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5597d449-17e3-440f-8b0e-56a902a96569)\*  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 pro systémy s procesorem Itanium a Windows Server 2008 pro systémy s procesorem Itanium Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=8c2abba5-0597-4565-9b87-a37e574690e0)  
(Mírný)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem Itanium a Windows Server 2008 pro systémy s procesorem Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e62493cb-8d25-4975-bbe6-a368e039872b)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem Itanium a Windows Server 2008 pro systémy s procesorem Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=91d5d34b-9d7e-4e83-89a4-f1aa388dc4e4)  
(Kritický)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem Itanium a Windows Server 2008 pro systémy s procesorem Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=55b07bc0-dff5-4cd7-87c9-c08e5a49197d)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem Itanium a Windows Server 2008 pro systémy s procesorem Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d10eda21-b3c3-4d8e-8596-bc45e4165f93)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
</tr>
<tr>
<th colspan="12" style="border:1px solid black;">
Windows 7
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS11-003**](http://go.microsoft.com/fwlink/?linkid=208304)
</td>
<td style="border:1px solid black;">
[**MS11-006**](http://go.microsoft.com/fwlink/?linkid=208146)
</td>
<td style="border:1px solid black;">
[**MS11-007**](http://go.microsoft.com/fwlink/?linkid=208059)
</td>
<td style="border:1px solid black;">
[**MS11-004**](http://go.microsoft.com/fwlink/?linkid=208522)
</td>
<td style="border:1px solid black;">
[**MS11-005**](http://go.microsoft.com/fwlink/?linkid=207843)
</td>
<td style="border:1px solid black;">
[**MS11-009**](http://go.microsoft.com/fwlink/?linkid=207839)
</td>
<td style="border:1px solid black;">
[**MS11-010**](http://go.microsoft.com/fwlink/?linkid=207840)
</td>
<td style="border:1px solid black;">
[**MS11-011**](http://go.microsoft.com/fwlink/?linkid=208365)
</td>
<td style="border:1px solid black;">
[**MS11-012**](http://go.microsoft.com/fwlink/?linkid=208362)
</td>
<td style="border:1px solid black;">
[**MS11-013**](http://go.microsoft.com/fwlink/?linkid=208523)
</td>
<td style="border:1px solid black;">
[**MS11-014**](http://go.microsoft.com/fwlink/?linkid=208395)
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
[**Kritický**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
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
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
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
Windows 7 pro 32bitové systémy a Windows 7 pro 32bitové systémy Service Pack 1
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=07aa7ffc-47c7-4611-b32c-ecb3fbcad32f)  
(Kritický)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows 7 pro 32bitové systémy a Windows 7 pro 32bitové systémy Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=1da57fbc-9ea4-4fc4-911d-d5c7825e012c)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Služba Microsoft FTP Service 7.5 pro službu IIS 7.5](http://www.microsoft.com/downloads/details.aspx?familyid=9dabd1d1-3f1e-46d1-b171-aafd3f08d291)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[JScript 5.8](http://www.microsoft.com/downloads/details.aspx?familyid=54a64215-e407-4b7b-8536-28817ef23bac)  
(Vysoký)  
[VBScript 5.8](http://www.microsoft.com/downloads/details.aspx?familyid=54a64215-e407-4b7b-8536-28817ef23bac)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows 7 pro 32bitové systémy](http://www.microsoft.com/downloads/details.aspx?familyid=e1224c90-b0bc-4e4b-999a-efae327213b4)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows 7 pro 32bitové systémy a Windows 7 pro 32bitové systémy Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=078fe6c0-1b2c-4896-a345-25cc1b1105e2)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows 7 pro 32bitové systémy a Windows 7 pro 32bitové systémy Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=ffed7c76-0b75-4f57-9b63-3961a8b449f6)  
(KB2425227)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 7 pro systémy s procesorem x64 a Windows 7 pro systémy s procesorem x64 Service Pack 1
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=2b8ffafe-78bb-4fa7-aea2-01208b6a3dfe)  
(Kritický)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows 7 pro systémy s procesorem x64 a Windows 7 pro systémy s procesorem x64 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=587adb89-2f6a-4893-9906-b6d6d9ada2bd)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Služba Microsoft FTP Service 7.5 pro službu IIS 7.5](http://www.microsoft.com/downloads/details.aspx?familyid=66fb4efe-bcd3-4e90-8e35-b013e014a952)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[JScript 5.8](http://www.microsoft.com/downloads/details.aspx?familyid=b854d76e-6891-426d-8c09-0ed8243a3b8d)  
(Vysoký)  
[VBScript 5.8](http://www.microsoft.com/downloads/details.aspx?familyid=b854d76e-6891-426d-8c09-0ed8243a3b8d)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows 7 pro systémy s procesorem x64](http://www.microsoft.com/downloads/details.aspx?familyid=ddcf352e-742c-485e-9ed5-19cdba673562)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows 7 pro systémy s procesorem x64 a Windows 7 pro systémy s procesorem x64 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=b42642b3-fb78-4700-bfe8-bfa997b90c16)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows 7 pro systémy s procesorem x64 a Windows 7 pro systémy s procesorem x64 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=c26cebcf-683f-4a51-be75-76535fb979a7)  
(KB2425227)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
</tr>
<tr>
<th colspan="12" style="border:1px solid black;">
Windows Server 2008 R2
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS11-003**](http://go.microsoft.com/fwlink/?linkid=208304)
</td>
<td style="border:1px solid black;">
[**MS11-006**](http://go.microsoft.com/fwlink/?linkid=208146)
</td>
<td style="border:1px solid black;">
[**MS11-007**](http://go.microsoft.com/fwlink/?linkid=208059)
</td>
<td style="border:1px solid black;">
[**MS11-004**](http://go.microsoft.com/fwlink/?linkid=208522)
</td>
<td style="border:1px solid black;">
[**MS11-005**](http://go.microsoft.com/fwlink/?linkid=207843)
</td>
<td style="border:1px solid black;">
[**MS11-009**](http://go.microsoft.com/fwlink/?linkid=207839)
</td>
<td style="border:1px solid black;">
[**MS11-010**](http://go.microsoft.com/fwlink/?linkid=207840)
</td>
<td style="border:1px solid black;">
[**MS11-011**](http://go.microsoft.com/fwlink/?linkid=208365)
</td>
<td style="border:1px solid black;">
[**MS11-012**](http://go.microsoft.com/fwlink/?linkid=208362)
</td>
<td style="border:1px solid black;">
[**MS11-013**](http://go.microsoft.com/fwlink/?linkid=208523)
</td>
<td style="border:1px solid black;">
[**MS11-014**](http://go.microsoft.com/fwlink/?linkid=208395)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Celkový stupeň závažnosti**
</td>
<td style="border:1px solid black;">
[**Mírný**](http://go.microsoft.com/fwlink/?linkid=21140)
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
<td style="border:1px solid black;">
Žádné
</td>
<td style="border:1px solid black;">
[**Mírný**](http://go.microsoft.com/fwlink/?linkid=21140)
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
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Žádné
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 pro systémy s procesorem x64 a Windows Server 2008 R2 pro systémy s procesorem x64 Service Pack 1
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=38b67efb-dd4b-4e8c-8460-0f40f0367441)\*\*  
(Mírný)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem x64 a Windows Server 2008 R2 pro systémy s procesorem x64 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=638318ed-4000-4b1a-bb4b-65b795f59784)\*  
(Kritický)
</td>
<td style="border:1px solid black;">
[Služba Microsoft FTP Service 7.5 pro službu IIS 7.5](http://www.microsoft.com/downloads/details.aspx?familyid=1e075f57-1723-4933-9b8e-7bce4a44a1c1)\*  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[JScript 5.8](http://www.microsoft.com/downloads/details.aspx?familyid=f482bd40-f0b9-4534-a768-45879f1e7285)\*\*  
(Mírný)  
[VBScript 5.8](http://www.microsoft.com/downloads/details.aspx?familyid=f482bd40-f0b9-4534-a768-45879f1e7285)\*\*  
(Mírný)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem x64](http://www.microsoft.com/downloads/details.aspx?familyid=70f5056a-72ad-46ff-a43f-ee151639b9a7)\*  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem x64 a Windows Server 2008 R2 pro systémy s procesorem x64 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=d2c53f44-12eb-4293-9fa5-2a14075b636e)\*  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem x64 a Windows Server 2008 R2 pro systémy s procesorem x64 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=46bb3ef1-24c3-41cb-8141-0fdbd85093f7)\*  
(KB2425227)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 pro systémy s procesorem Itanium a Windows Server 2008 R2 pro systémy s procesorem Itanium Service Pack 1
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=0e41cbe5-5e5e-4ece-a71a-71f4b6319f0d)  
(Mírný)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem Itanium a Windows Server 2008 R2 pro systémy s procesorem Itanium Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=4688ea0d-a467-4f24-ac52-104d05c8cae8)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Služba Microsoft FTP Service 7.5 pro službu IIS 7.5](http://www.microsoft.com/downloads/details.aspx?familyid=bfddd539-c64f-4467-88ee-6bdfe645b478)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[JScript 5.8](http://www.microsoft.com/downloads/details.aspx?familyid=f05a3de0-381c-4d17-83ee-ca4f6da1bdb0)  
(Mírný)  
[VBScript 5.8](http://www.microsoft.com/downloads/details.aspx?familyid=f05a3de0-381c-4d17-83ee-ca4f6da1bdb0)  
(Mírný)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=1646b3a5-714f-4ea5-b109-566fa9b933b6)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem Itanium a Windows Server 2008 R2 pro systémy s procesorem Itanium Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=8c6bf720-f544-4f58-9b1c-2399957ec43d)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem Itanium a Windows Server 2008 R2 pro systémy s procesorem Itanium Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=01737933-e7de-451b-b02f-b7ca24693965)  
(KB2425227)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
</tr>
</table>
<p></p>
 
**Poznámky k systémům Windows Server 2008 a Windows Server 2008 R2**

**\*Instalace Server Core obsahující chybu zabezpečení.** Tato aktualizace se stejným hodnocením závažnosti se vztahuje k podporovaným edicím systému Windows Server 2008 nebo Windows Server 2008 R2, jak je uvedeno, s instalací pomocí volby pro instalaci Server Core nebo bez ní. Další informace o této možnosti instalace naleznete v článcích na webu TechNet [Managing a Server Core Installation](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) (Správa instalace Server Core) a [Servicing a Server Core Installation](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx) (Obsluha instalace Server Core). Možnost instalace Server Core se nevztahuje na určité edice systému Windows Server 2008 a Windows Server 2008 R2; další informace naleznete v části [Porovnání možností instalace Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**\*\*Instalace Server Core není touto chybou ovlivněna.** Chyby zabezpečení, které tato aktualizace řeší, nemají vliv na podporované edice systému Windows Server 2008 nebo Windows Server 2008 R2, jak je uvedeno, v případě instalace s využitím možnosti instalace Server Core. Další informace o této možnosti instalace naleznete v článcích na webu TechNet [Managing a Server Core Installation](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) (Správa instalace Server Core) a [Servicing a Server Core Installation](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx) (Obsluha instalace Server Core). Možnost instalace Server Core se nevztahuje na určité edice systému Windows Server 2008 a Windows Server 2008 R2; další informace naleznete v části [Porovnání možností instalace Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**Poznámka k bulletinu MS11-004**

<sup>[1]</sup>Nejedná se o výchozí službu FTP v tomto operačním systému

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
Aplikace systému Microsoft Office
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS11-008**](http://go.microsoft.com/fwlink/?linkid=204799)
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
Microsoft Visio 2002 Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft Visio 2002 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=273d8078-0dc7-43d8-bcae-54c811e49e0e)  
(KB2434711)  
(Vysoký)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Visio 2003 Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Visio 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=f1067eaa-d18d-4bff-a02e-1d990c36ca7f)  
(KB2434733)  
(Vysoký)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Visio 2007 Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft Visio 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=097a642b-b786-4724-a907-79f37cded836)  
(KB2434737)  
(Vysoký)
</td>
</tr>
</table>
<p></p>
 

Nástroje a doporučené postupy zjišťování a nasazení
---------------------------------------------------

<span></span>
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

-   Yuki Chenové ze společnosti [Trend Micro](http://www.trendmicro.com) za oznámení chyby popsané v bulletinu MS11-003.
-   Uživateli s pseudonymem SkyLined ze společnosti [Google Inc.](http://www.google.com/) za oznámení chyby popsané v bulletinu MS11-003.
-   Haifei Liovi z výzkumného týmu [FortiGuard Labs společnosti Fortinet](http://www.fortiguard.com/) za oznámení chyby popsané v bulletinu MS11-003.
-   Kobimu Parienteovi a Yanivu Mironovi, spolupracujícím se společností [VeriSign iDefense Labs](http://labs.idefense.com/), za oznámení chyby popsané v bulletinu MS11-006.
-   Uživateli s pseudonymem Procyun, spolupracujícímu s organizací [Zero Day Initiative](http://www.zerodayinitiative.com/) společnosti [TippingPoint](http://www.tippingpoint.com/), za oznámení chyby popsané v bulletinu MS11-008.
-   Xinu Ouyangovi ze společnosti [Palo Alto Networks](http://www.paloaltonetworks.com/) za oznámení dvou chyb popsaných v bulletinu MS11-008.
-   Yamatu Liovi ze společnosti [Palo Alto Networks](http://www.paloaltonetworks.com/) za oznámení chyby popsané v bulletinu MS11-009.
-   Sihanu Qingovi (profesor), Weipingu Wenovi (docent), Liang Yinové a Hushengu Zhouovi (postgraduální studenti) z [fakulty zabezpečení informací pekingské univerzity](http://www.ss.pku.edu.cn/en/) za oznámení chyby popsané v bulletinu MS11-010.
-   Uživateli s pseudonymem Zhengwenbin z organizace [360safe](http://www.360.cn) za oznámení chyby popsané v bulletinu MS11-011.
-   Guo Bojunovi za oznámení chyby popsané v bulletinu MS11-011.
-   Wei Zhangovi za oznámení chyby popsané v bulletinu MS11-011.
-   Marcovi Giulianimu ze společnosti [PrevX](http://www.prevx.com/) za spolupráci na řešení chyby popsané v bulletinu MS11-011.
-   Uživateli s pseudonymem std\_logic, spolupracujícímu s organizací [Zero Day Initiative](http://www.zerodayinitiative.com/) společnosti [TippingPoint](http://www.tippingpoint.com/), za oznámení chyby popsané v bulletinu MS11-011.
-   Tarjei Mandtovi ze společnosti [Norman](http://www.norman.com) za oznámení pěti chyb popsaných v bulletinu MS11-012.
-   [Týmu MIT Kerberos](http://web.mit.edu/kerberos) za oznámení chyby popsané v bulletinu MS11-013.
-   Scottu Stenderovi ze společnosti [iSEC Partners](http://www.isecpartners.com/) za oznámení chyby popsané v bulletinu MS11-013.
-   Testerovi zabezpečení Jorgemu Mouraovi ze společnosti Primavera BSS za oznámení chyby popsané v bulletinu MS11-014.

#### Technická podpora

-   Uvedený software byl testován za účelem zjištění, kterých verzí se chyba týká. U dalších verzí skončila časově omezená podpora. Pokud chcete zjistit dobu, po kterou je pro určitou verzi softwaru poskytována podpora, navštivte web [Zásady poskytování technické podpory pro produkty společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=21742).
-   Zákazníci mohou získat technickou podporu na webu [služby technické podpory společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=21131). Hovory související s aktualizacemi zabezpečení jsou bezplatné. Další informace o dostupných možnostech technické podpory naleznete na webu [Pomoc a podpora společnosti Microsoft](http://support.microsoft.com/).
-   Mezinárodní zákazníci získají podporu u místních zastoupení společnosti Microsoft. Technická podpora související s aktualizacemi zabezpečení je bezplatná. Další informace o možnostech kontaktování společnosti Microsoft v případě potřeby technické podpory získáte na [webu mezinárodní technické podpory](http://go.microsoft.com/fwlink/?linkid=21155).

#### Zřeknutí se záruky

Informace ve znalostní bázi Microsoft Knowledge Base jsou poskytovány tak, jak jsou, bez jakékoli záruky. Společnost Microsoft neposkytuje žádné záruky, výslovně uvedené či mlčky předpokládané, včetně záruk obchodovatelnosti a vhodnosti pro určitý účel. Společnost Microsoft ani její dodavatelé nenesou v žádném případě zodpovědnost za žádné škody, včetně přímých, nepřímých, náhodných či následných škod, ztráty zisku či zvláštních škod, a to ani v případě, že byli na možnost takových škod upozorněni. V některých zemích a právních řádech není dovoleno vyloučit nebo omezit odpovědnost, proto se výše uvedené omezení na vás nemusí vztahovat.

#### Revize

-   V1.0 (8. února 2011): Souhrnný bulletin byl publikován.
-   V1.1 (9. února 2011): V bulletinu MS11-013 bylo opraveno hodnocení indexu zneužitelnosti pro chybu zabezpečení CVE-2011-0091 na index „3 - Vytvoření kódu funkčního zneužití není pravděpodobné.“ Jedná se pouze o změnu informace.
-   V2.0 (8. března 2011): Do seznamu softwaru obsahujícího chybu pro bulletiny MS11-003, MS11-004, MS11-007 a MS11-009 byl přidán systém Windows 7 pro 32bitové systémy Service Pack 1, Windows 7 pro systémy s procesorem x64 Service Pack 1, Windows Server 2008 R2 pro systémy s procesorem x64 Service Pack 1 a Windows Server 2008 R2 pro systémy s procesorem Itanium Service Pack 1. Další informace naleznete v jednotlivých bulletinech v části Nejčastější dotazy související s aktualizacemi.
-   V3.0 (16. března 2011): Do seznamu softwaru obsahujícího chybu pro bulletin MS11-013 byl přidán systém Windows 7 pro 32bitové systémy Service Pack 1, Windows 7 pro systémy s procesorem x64 Service Pack 1, Windows Server 2008 R2 pro systémy s procesorem x64 Service Pack 1 a Windows Server 2008 R2 pro systémy s procesorem Itanium Service Pack 1. Další informace naleznete v tomto bulletinu v části Nejčastější dotazy související s aktualizacemi.
-   V4.0 (18. března 2011): Do seznamu softwaru obsahujícího chybu pro bulletin MS11-012 byl přidán systém Windows 7 pro 32bitové systémy Service Pack 1, Windows 7 pro systémy s procesorem x64 Service Pack 1, Windows Server 2008 R2 pro systémy s procesorem x64 Service Pack 1 a Windows Server 2008 R2 pro systémy s procesorem Itanium Service Pack 1. Další informace naleznete v tomto bulletinu v části Nejčastější dotazy související s aktualizacemi.

*Built at 2014-04-18T01:50:00Z-07:00*
