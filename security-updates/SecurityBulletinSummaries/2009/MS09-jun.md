---
TOCTitle: 'MS09-JUN'
Title: 'Souhrnný bulletin zabezpečení společnosti Microsoft, červen 2009'
ms:assetid: 'ms09-jun'
ms:contentKeyID: 61223988
ms:mtpsurl: 'https://technet.microsoft.com/cs-CZ/library/ms09-jun(v=Security.10)'
---

Security Bulletin Summary

Souhrnný bulletin zabezpečení společnosti Microsoft, červen 2009
================================================================

Publikováno: 9. června 2009

**Verze:** 1.0

Tento souhrnný bulletin uvádí bulletiny zabezpečení vydané v červnu 2009.

Spolu s vydáním bulletinů v červnu 2009 nahrazuje tento souhrnný bulletin předběžné oznámení o bulletinech vydané 4. června 2009. Další informace o službě předběžného oznámení o bulletinech naleznete v části [Předběžné oznámení o bulletinech zabezpečení společnosti Microsoft](http://technet.microsoft.com/security/bulletin/advance).

Informace o tom, jak dostávat automatická oznámení o vydání nových bulletinů zabezpečení společnosti Microsoft, naleznete na webu [Zasílání technických oznámení o zabezpečení společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=21163).

Pro zodpovězení zákaznických dotazů týkajících se těchto bulletinů uspořádá společnost Microsoft webové vysílání 10. června 2009 v 11:00 časového pásma Tichomoří (USA a Kanada). [Zaregistrovat pro webové vysílání týkající se červnových bulletinů zabezpečení](http://msevents.microsoft.com/cui/webcasteventdetails.aspx?culture=en-us&eventid=1032395225). Po tomto datu je webové vysílání dostupné na požádání. Další informace získáte v [souhrnných bulletinech zabezpečení společnosti Microsoft a webovém vysílání](http://technet.microsoft.com/security/bulletin/summary).

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
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=151361">MS09-018</a></td>
<td style="border:1px solid black;"><strong>Chyby zabezpečení služby Active Directory umožňují vzdálené spuštění kódu (971055)</strong><br />
<br />
Tato aktualizace zabezpečení řeší dvě soukromými osobami oznámené chyby zabezpečení v implementacích služby Active Directory v systémech Microsoft Windows 2000 Server a Windows Server 2003; a služby ADAM (Active Directory Application Mode) při instalaci v systémech Windows XP Professional a Windows Server 2003. Závažnější chyba zabezpečení by mohla umožnit vzdálené spuštění kódu. Útočník, který by úspěšně zneužil tuto chybu zabezpečení, by mohl vzdáleně převzít úplnou kontrolu nad postiženým systémem. Útočník by tak mohl instalovat programy, zobrazovat, měnit či odstraňovat data nebo vytvářet nové účty s úplnými uživatelskými právy. Doporučené postupy pro používání brány firewall a standardní konfigurace této brány zajišťují ochranu sítí před útoky pocházejícími z oblasti mimo rozlehlou síť. Je vhodné, aby systémy připojené k Internetu měly přístupný minimální počet portů.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritický</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=141786">MS09-022</a></td>
<td style="border:1px solid black;"><strong>Chyby zabezpečení zařazovací služby tisku systému Windows umožňují vzdálené spuštění kódu (961501)</strong><br />
<br />
Tato aktualizace zabezpečení řeší tři soukromými osobami oznámené chyby zabezpečení zařazovací služby tisku systému Windows. Nejzávažnější chyba zabezpečení by mohla umožnit vzdálené spuštění kódu, pokud by postižený server obdržel speciálně vytvořený požadavek RPC. Doporučené postupy pro používání brány firewall a standardní konfigurace této brány zajišťují ochranu sítí před útoky pocházejícími z oblasti mimo rozlehlou síť. Je vhodné, aby systémy připojené k Internetu měly přístupný minimální počet portů.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritický</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=150860">MS09-019</a></td>
<td style="border:1px solid black;"><strong>Kumulativní aktualizace zabezpečení pro aplikaci Internet Explorer (969897)</strong><br />
<br />
Tato aktualizace zabezpečení řeší sedm chyb zabezpečení oznámených soukromými osobami a jednu veřejně známou chybu zabezpečení v aplikaci Internet Explorer. Závažnější chyby zabezpečení mohou umožnit vzdálené spuštění kódu, pokud uživatel pomocí aplikace Internet Explorer zobrazí speciálně vytvořenou webovou stránku. Uživatelé, jejichž účty jsou konfigurovány tak, aby měli v systému méně uživatelských práv, by byli vystaveni menšímu riziku než uživatelé s uživatelskými právy správce.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritický</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows, Internet Explorer</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=147416">MS09-027</a></td>
<td style="border:1px solid black;"><strong>Chyby zabezpečení v aplikaci Microsoft Office Word umožňují vzdálené spuštění kódu (969514)</strong><br />
<br />
Tato aktualizace zabezpečení řeší dvě soukromými osobami oznámené chyby zabezpečení, které by mohly umožnit vzdálené spuštění kódu v případě, že uživatel otevře speciálně vytvořený soubor aplikace Word. Útočník, který by některou z těchto chyb zabezpečení zneužil, by mohl získat úplnou kontrolu nad postiženým systémem. Útočník by tak mohl instalovat programy, zobrazovat, měnit či odstraňovat data nebo vytvářet nové účty s úplnými uživatelskými právy.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritický</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Může vyžadovat restartování</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=147294">MS09-021</a></td>
<td style="border:1px solid black;"><strong>Chyby zabezpečení v aplikaci Microsoft Office Excel umožňují vzdálené spuštění kódu (969462)</strong><br />
<br />
Tato aktualizace zabezpečení řeší několik soukromými osobami oznámených chyb zabezpečení, které by mohly umožnit vzdálené spuštění kódu v případě, že uživatel otevře speciálně vytvořený soubor aplikace Excel obsahující chybně formátovaný objekt. Útočník, který by úspěšně zneužil některou z těchto chyb zabezpečení, by mohl převzít úplnou kontrolu nad postiženým systémem. Útočník by tak mohl instalovat programy, zobrazovat, měnit či odstraňovat data nebo vytvářet nové účty s úplnými uživatelskými právy.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritický</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Může vyžadovat restartování</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=128104">MS09-024</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení převaděčů sady Microsoft Works umožňuje vzdálené spuštění kódu (957632)</strong><br />
<br />
Tato aktualizace zabezpečení řeší chybu zabezpečení převaděčů sady Microsoft Works oznámenou soukromou osobou. Tato chyba umožňuje vzdálené spuštění kódu, pokud uživatel otevře speciálně vytvořený soubor sady Works. Útočník, který by úspěšně zneužil tuto chybu zabezpečení, by mohl získat stejná uživatelská práva, jako má místní uživatel. Uživatelé, jejichž účty jsou konfigurovány tak, aby měli v systému méně uživatelských práv, by byli vystaveni menšímu riziku než uživatelé s uživatelskými právy správce.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritický</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Může vyžadovat restartování</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=150174">MS09-026</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení protokolu RPC umožňuje zvýšení úrovně oprávnění (970238)</strong><br />
<br />
Tato aktualizace zabezpečení řeší veřejně známou chybu zabezpečení protokolu RPC (Vzdálené volání procedur) systému Windows, kde zařazovací modul RPC nesprávně aktualizuje svůj vnitřní stav. Tato chyba zabezpečení může útočníkovi umožnit spuštění libovolného kódu a převzetí úplné kontroly nad postiženým systémem. Podporované edice systému Microsoft Windows nejsou dodávány se servery ani klienty RPC, které by mohly obsahovat tuto chybu. Ve výchozí konfiguraci by uživatelé neměli být touto chybou zabezpečení ohroženi. Tato chyba se však vyskytuje za běhu v protokolu Microsoft Windows RPC a mohla by ohrozit aplikace RPC jiných výrobců.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Důležité</a><br />
Zvýšení úrovně oprávnění</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=150248">MS09-025</a></td>
<td style="border:1px solid black;"><strong>Chyby zabezpečení jádra systému Windows umožňují zvýšení oprávnění (968537)</strong><br />
<br />
Tato aktualizace zabezpečení řeší dvě veřejně známé a dvě soukromými osobami oznámené chyby zabezpečení jádra systému Windows, které by mohly vést ke zvýšení úrovně oprávnění. Útočník, který by některou z těchto chyb zabezpečení úspěšně zneužil, by mohl spustit libovolný kód a získat úplnou kontrolu nad postiženým systémem. Útočník by tak mohl instalovat programy, zobrazovat, měnit či odstraňovat data nebo vytvářet nové účty s úplnými uživatelskými právy. Tyto chyby zabezpečení může zneužít pouze útočník s platnými pověřeními pro přihlášení, která by mu umožňovala se místně přihlásit. Uvedené chyby zabezpečení nemohou zneužít vzdálení ani anonymní uživatelé.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Důležité</a><br />
Zvýšení úrovně oprávnění</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=150568">MS09-020</a></td>
<td style="border:1px solid black;"><strong>Chyby zabezpečení Internetové informační služby (IIS) umožňují zvýšení úrovně oprávnění (970483)</strong><br />
<br />
Tato aktualizace zabezpečení řeší jednu veřejně známou a jednu soukromou osobou oznámenou chybu zabezpečení Internetové informační služby (IIS). Chyby zabezpečení by mohly vést ke zvýšení úrovně oprávnění, pokud by útočník odeslal speciálně vytvořený požadavek HTTP na web, který vyžaduje ověření. Tyto chyby zabezpečení umožňují útočníkovi obejít konfiguraci služby IIS, která specifikuje, jaké ověření je povoleno, nikoli však kontrolu seznamu řízení přístupu (ACL) v souborovém systému, jež ověřuje, zda má k souboru daný uživatel přístup. Úspěšné zneužití těchto chyb zabezpečení by útočníkovi znemožnilo přístup k oprávněním k účtu anonymního uživatele, uděleným seznamy řízení přístupu v souborovém systému.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Důležité</a><br />
Zvýšení úrovně oprávnění</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=143550">MS09-023</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení v programu Windows Search může umožnit přístup k informacím (963093)</strong><br />
<br />
Tato aktualizace zabezpečení řeší chybu zabezpečení v programu Windows Search, kterou oznámila soukromá osoba. Uvedená chyba zabezpečení umožňuje zpřístupnění informací, pokud uživatel provede hledání, jehož prvním výsledkem bude speciálně vytvořený soubor, nebo pokud uživatel ve výsledcích hledání zobrazí speciálně vytvořený soubor. Ve výchozím nastavení není součást Windows Search nainstalována v systémech Microsoft Windows XP a Windows Server 2003. Jedná se o volitelnou součást, kterou lze stáhnout. Služba Windows Search nainstalovaná v podporovaných edicích systémů Windows Vista a Windows Server 2008 není touto chybou zabezpečení postižena.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Mírný</a><br />
Přístup k informacím</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
</tbody>
</table>
<p></p>
  
Index zneužitelnosti  
--------------------
  
 
Následující tabulka uvádí hodnocení zneužitelnosti každé chyby zabezpečení uvedené v tomto měsíci. Chyby zabezpečení jsou řazeny podle čísla jednotlivých bulletinů (ID bulletinu) a chyb (ID CVE).
  
**Jak pracovat s touto tabulkou**
  
V této tabulce zjistíte, jaká je pravděpodobnost vydání funkčního zneužitelného kódu během 30 dní od vydání tohoto bulletinu zabezpečení pro všechny aktualizace zabezpečení, které bude třeba nainstalovat. Všechna níže uvedená hodnocení zvažte na základě vaší specifické konfigurace a podle závěrů hodnocení nastavte priority pro zavádění jednotlivých aktualizací. Další informace o významu těchto hodnocení a způsobu jejich stanovení najdete v indexu zneužitelnosti [Microsoft Exploitability Index](http://technet.microsoft.com/en-us/security/cc998259.aspx).
  
| ID bulletinu                                              | Název bulletinu                                                                                    | ID CVE                                                                           | Hodnocení indexu zneužitelnosti                                                                                                | Hlavní poznámky                                                                                                                                                                                                                                                                      |  
|-----------------------------------------------------------|----------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| [MS09-018](http://go.microsoft.com/fwlink/?linkid=151361) | Chyby zabezpečení služby Active Directory umožňují vzdálené spuštění kódu (971055)                 | [CVE-2009-1138](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1138) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní kód zneužití je pravděpodobný                | V serverech Windows 2000 existuje možnost vzdáleného spuštění kódu mající za následek zneužití služby LDAP (default tcp/389) v síti.                                                                                                                                                 |  
| [MS09-018](http://go.microsoft.com/fwlink/?linkid=151361) | Chyby zabezpečení služby Active Directory umožňují vzdálené spuštění kódu (971055)                 | [CVE-2009-1139](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1139) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Vytvoření funkčního zneužitelného kódu není pravděpodobné | Bezpečnostním efektem této chyby zabezpečení je nevrácení paměti, což může případně vést k odmítnutí služby. Kód nelze spustit.                                                                                                                                                      |  
| [MS09-019](http://go.microsoft.com/fwlink/?linkid=150860) | Kumulativní aktualizace zabezpečení pro aplikaci Internet Explorer (969897)                        | [CVE-2007-3091](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2007-3091) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Vytvoření funkčního zneužitelného kódu není pravděpodobné | (Žádné)                                                                                                                                                                                                                                                                              |  
| [MS09-019](http://go.microsoft.com/fwlink/?linkid=150860) | Kumulativní aktualizace zabezpečení pro aplikaci Internet Explorer (969897)                        | [CVE-2009-1140](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1140) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Vytvoření funkčního zneužitelného kódu není pravděpodobné | Jedná se o chybu zabezpečení týkající se přístupu k informacím při přechodu mezi doménami, která s největší pravděpodobností povede k zpřístupnění informací, nikoli spuštění kódu.                                                                                                  |  
| [MS09-019](http://go.microsoft.com/fwlink/?linkid=150860) | Kumulativní aktualizace zabezpečení pro aplikaci Internet Explorer (969897)                        | [CVE-2009-1141](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1141) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní kód zneužití je pravděpodobný                | (Žádné)                                                                                                                                                                                                                                                                              |  
| [MS09-019](http://go.microsoft.com/fwlink/?linkid=150860) | Kumulativní aktualizace zabezpečení pro aplikaci Internet Explorer (969897)                        | [CVE-2009-1528](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1528) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Vytvoření funkčního zneužitelného kódu není pravděpodobné | (Žádné)                                                                                                                                                                                                                                                                              |  
| [MS09-019](http://go.microsoft.com/fwlink/?linkid=150860) | Kumulativní aktualizace zabezpečení pro aplikaci Internet Explorer (969897)                        | [CVE-2009-1529](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1529) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Nekonsistentní kód zneužití je pravděpodobný              | (Žádné)                                                                                                                                                                                                                                                                              |  
| [MS09-019](http://go.microsoft.com/fwlink/?linkid=150860) | Kumulativní aktualizace zabezpečení pro aplikaci Internet Explorer (969897)                        | [CVE-2009-1530](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1530) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Nekonsistentní kód zneužití je pravděpodobný              | (Žádné)                                                                                                                                                                                                                                                                              |  
| [MS09-019](http://go.microsoft.com/fwlink/?linkid=150860) | Kumulativní aktualizace zabezpečení pro aplikaci Internet Explorer (969897)                        | [CVE-2009-1531](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1531) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Vytvoření funkčního zneužitelného kódu není pravděpodobné | (Žádné)                                                                                                                                                                                                                                                                              |  
| [MS09-019](http://go.microsoft.com/fwlink/?linkid=150860) | Kumulativní aktualizace zabezpečení pro aplikaci Internet Explorer (969897)                        | [CVE-2009-1532](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1532) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Vytvoření funkčního zneužitelného kódu není pravděpodobné | (Žádné)                                                                                                                                                                                                                                                                              |  
| [MS09-020](http://go.microsoft.com/fwlink/?linkid=150568) | Chyby zabezpečení Internetové informační služby (IIS) umožňují zvýšení úrovně oprávnění (970483)   | [CVE-2009-1122](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1122) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Vytvoření funkčního zneužitelného kódu není pravděpodobné | Nízká pravděpodobnost spuštění kódu, ale velká pravděpodobnost zpřístupnění informací z důvodu obejití ověření.                                                                                                                                                                      |  
| [MS09-020](http://go.microsoft.com/fwlink/?linkid=150568) | Chyby zabezpečení Internetové informační služby (IIS) umožňují zvýšení úrovně oprávnění (970483)   | [CVE-2009-1535](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1535) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní kód zneužití je pravděpodobný                | Pro zpřístupnění informací je k dispozici veřejný kód.                                                                                                                                                                                                                               |  
| [MS09-021](http://go.microsoft.com/fwlink/?linkid=147294) | Chyby zabezpečení v aplikaci Microsoft Office Excel umožňují vzdálené spuštění kódu (969462)       | [CVE-2009-0549](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0549) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Nekonsistentní kód zneužití je pravděpodobný              | (Žádné)                                                                                                                                                                                                                                                                              |  
| [MS09-021](http://go.microsoft.com/fwlink/?linkid=147294) | Chyby zabezpečení v aplikaci Microsoft Office Excel umožňují vzdálené spuštění kódu (969462)       | [CVE-2009-0557](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0557) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní kód zneužití je pravděpodobný                | (Žádné)                                                                                                                                                                                                                                                                              |  
| [MS09-021](http://go.microsoft.com/fwlink/?linkid=147294) | Chyby zabezpečení v aplikaci Microsoft Office Excel umožňují vzdálené spuštění kódu (969462)       | [CVE-2009-0558](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0558) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Nekonsistentní kód zneužití je pravděpodobný              | (Žádné)                                                                                                                                                                                                                                                                              |  
| [MS09-021](http://go.microsoft.com/fwlink/?linkid=147294) | Chyby zabezpečení v aplikaci Microsoft Office Excel umožňují vzdálené spuštění kódu (969462)       | [CVE-2009-0559](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0559) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní kód zneužití je pravděpodobný                | Nebezpečení spuštění kódu se týká pouze systému Office 2000. Útoky na novější verze systému Office spuštěním kódu téměř jistě neskončí.                                                                                                                                              |  
| [MS09-021](http://go.microsoft.com/fwlink/?linkid=147294) | Chyby zabezpečení v aplikaci Microsoft Office Excel umožňují vzdálené spuštění kódu (969462)       | [CVE-2009-0560](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0560) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Vytvoření funkčního zneužitelného kódu není pravděpodobné | (Žádné)                                                                                                                                                                                                                                                                              |  
| [MS09-021](http://go.microsoft.com/fwlink/?linkid=147294) | Chyby zabezpečení v aplikaci Microsoft Office Excel umožňují vzdálené spuštění kódu (969462)       | [CVE-2009-0561](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0561) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní kód zneužití je pravděpodobný                | (Žádné)                                                                                                                                                                                                                                                                              |  
| [MS09-021](http://go.microsoft.com/fwlink/?linkid=147294) | Chyby zabezpečení v aplikaci Microsoft Office Excel umožňují vzdálené spuštění kódu (969462)       | [CVE-2009-1134](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1134) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní kód zneužití je pravděpodobný                | (Žádné)                                                                                                                                                                                                                                                                              |  
| [MS09-022](http://go.microsoft.com/fwlink/?linkid=141786) | Chyby zabezpečení zařazovací služby tisku systému Windows umožňují vzdálené spuštění kódu (961501) | [CVE-2009-0228](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0228) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní kód zneužití je pravděpodobný                | (Žádné)                                                                                                                                                                                                                                                                              |  
| [MS09-022](http://go.microsoft.com/fwlink/?linkid=141786) | Chyby zabezpečení zařazovací služby tisku systému Windows umožňují vzdálené spuštění kódu (961501) | [CVE-2009-0229](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0229) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Vytvoření funkčního zneužitelného kódu není pravděpodobné | Jedná se o chybu zabezpečení typu zpřístupnění informací bez možnosti spuštění kódu.                                                                                                                                                                                                 |  
| [MS09-022](http://go.microsoft.com/fwlink/?linkid=141786) | Chyby zabezpečení zařazovací služby tisku systému Windows umožňují vzdálené spuštění kódu (961501) | [CVE-2009-0230](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0230) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní kód zneužití je pravděpodobný                | (Žádné)                                                                                                                                                                                                                                                                              |  
| [MS09-023](http://go.microsoft.com/fwlink/?linkid=143550) | Chyba zabezpečení v programu Windows Search může umožnit přístup k informacím (963093)             | [CVE-2009-0239](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0239) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Vytvoření funkčního zneužitelného kódu není pravděpodobné | (Žádné)                                                                                                                                                                                                                                                                              |  
| [MS09-024](http://go.microsoft.com/fwlink/?linkid=128104) | Chyba zabezpečení převaděčů sady Microsoft Works umožňuje vzdálené spuštění kódu (957632)          | [CVE-2009-1533](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1533) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní kód zneužití je pravděpodobný                | (Žádné)                                                                                                                                                                                                                                                                              |  
| [MS09-025](http://go.microsoft.com/fwlink/?linkid=150248) | Chyby zabezpečení jádra systému Windows umožňují zvýšení oprávnění (968537)                        | [CVE-2009-1123](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1123) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Nekonsistentní kód zneužití je pravděpodobný              | (Žádné)                                                                                                                                                                                                                                                                              |  
| [MS09-025](http://go.microsoft.com/fwlink/?linkid=150248) | Chyby zabezpečení jádra systému Windows umožňují zvýšení oprávnění (968537)                        | [CVE-2009-1124](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1124) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní kód zneužití je pravděpodobný                | (Žádné)                                                                                                                                                                                                                                                                              |  
| [MS09-025](http://go.microsoft.com/fwlink/?linkid=150248) | Chyby zabezpečení jádra systému Windows umožňují zvýšení oprávnění (968537)                        | [CVE-2009-1125](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1125) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní kód zneužití je pravděpodobný                | (Žádné)                                                                                                                                                                                                                                                                              |  
| [MS09-025](http://go.microsoft.com/fwlink/?linkid=150248) | Chyby zabezpečení jádra systému Windows umožňují zvýšení oprávnění (968537)                        | [CVE-2009-1126](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1126) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní kód zneužití je pravděpodobný                | Konsistentní zneužití kódu je nejpravděpodobnější u systému Windows 2000. Pravděpodobnost spuštění kódu u této chyby zabezpečení týkající se přetečení vyrovnávací paměti zásobníku je díky ochraně /GS u systémů Windows XP a Windows Server 2003 nižší.                            |  
| [MS09-026](http://go.microsoft.com/fwlink/?linkid=150174) | Chyba zabezpečení služby RPC umožňuje zvýšení úrovně oprávnění (970238)                            | [CVE-2009-0568](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0568) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Nekonsistentní kód zneužití je pravděpodobný              | Tato chyba zabezpečení neohrožuje přímo žádný software společnosti Microsoft. Nicméně pokud nedojde k instalaci této aktualizace zabezpečení, mohou být vzdáleným spuštěním kódu ohroženy pracovní stanice, do nichž jsou služby RPC implementovány nezávislými dodavateli softwaru. |  
| [MS09-027](http://go.microsoft.com/fwlink/?linkid=147416) | Chyby zabezpečení v aplikaci Microsoft Office Word umožňují vzdálené spuštění kódu (969514)        | [CVE-2009-0563](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0563) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Nekonsistentní kód zneužití je pravděpodobný              | (Žádné)                                                                                                                                                                                                                                                                              |  
| [MS09-027](http://go.microsoft.com/fwlink/?linkid=147416) | Chyby zabezpečení v aplikaci Microsoft Office Word umožňují vzdálené spuštění kódu (969514)        | [CVE-2009-0565](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0565) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní kód zneužití je pravděpodobný                | (Žádné)                                                                                                                                                                                                                                                                              |
  
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
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
</tr>
<tr>
<th colspan="8" style="border:1px solid black;">
Microsoft Windows 2000  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS09-018**](http://go.microsoft.com/fwlink/?linkid=151361)
</td>
<td style="border:1px solid black;">
[**MS09-022**](http://go.microsoft.com/fwlink/?linkid=141786)
</td>
<td style="border:1px solid black;">
[**MS09-019**](http://go.microsoft.com/fwlink/?linkid=150860)
</td>
<td style="border:1px solid black;">
[**MS09-026**](http://go.microsoft.com/fwlink/?linkid=150174)
</td>
<td style="border:1px solid black;">
[**MS09-025**](http://go.microsoft.com/fwlink/?linkid=150248)
</td>
<td style="border:1px solid black;">
[**MS09-020**](http://go.microsoft.com/fwlink/?linkid=150568)
</td>
<td style="border:1px solid black;">
[**MS09-023**](http://go.microsoft.com/fwlink/?linkid=143550)
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
[**Kritický**](http://go.microsoft.com/fwlink/?linkid=21140)
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
Microsoft Windows 2000 Service Pack 4
</td>
<td style="border:1px solid black;">
[Služba Active Directory v systému Microsoft Windows 2000 Server Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=bba6e20a-0345-46ae-a6f1-fd27fdee7c21)  
(KB969805)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=86378753-db24-44c2-a27d-cc0239f40ab8)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 5.01 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=d645ad82-13c3-4030-808b-834e86ed3298)  
(Kritický)  
[Microsoft Internet Explorer 6 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=fe8b3796-a407-4f41-89eb-35b4bcc24ff6)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=155a79c1-e5e4-4f62-b4b0-53aca59f20ac)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=79b0481d-a3d7-477b-928a-a98cc79374af)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Internetová informační služba 5.0](http://www.microsoft.com/downloads/details.aspx?familyid=8515a294-4f25-4dc5-860a-e7ad9b6c1c01)  
(Důležitý)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
</tr>
<tr>
<th colspan="8" style="border:1px solid black;">
Windows XP
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS09-018**](http://go.microsoft.com/fwlink/?linkid=151361)
</td>
<td style="border:1px solid black;">
[**MS09-022**](http://go.microsoft.com/fwlink/?linkid=141786)
</td>
<td style="border:1px solid black;">
[**MS09-019**](http://go.microsoft.com/fwlink/?linkid=150860)
</td>
<td style="border:1px solid black;">
[**MS09-026**](http://go.microsoft.com/fwlink/?linkid=150174)
</td>
<td style="border:1px solid black;">
[**MS09-025**](http://go.microsoft.com/fwlink/?linkid=150248)
</td>
<td style="border:1px solid black;">
[**MS09-020**](http://go.microsoft.com/fwlink/?linkid=150568)
</td>
<td style="border:1px solid black;">
[**MS09-023**](http://go.microsoft.com/fwlink/?linkid=143550)
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
[**Mírný**](http://go.microsoft.com/fwlink/?linkid=21140)
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
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Mírný**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Service Pack 2 a Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Služba ADAM (Active Directory Application Mode) v systémech Windows XP Professional Service Pack 2 a Windows XP Professional Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=cb2c9b76-0c65-4754-9941-d45a7c74a29a)  
(KB970437)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 a Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=f2119aca-a98e-4810-be52-f38241443baf)  
(Mírný)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=3d7f63ee-d7c3-48a5-902e-60625405e97d)  
(Kritický)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=827b735c-660b-4723-b688-3297e107153a)  
(Kritický)  
[Windows Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=d9e27ce1-4e7c-437f-9477-e7805a33da08)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 a Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=f033fa78-c451-44f8-aa6c-a49622c37f40)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 a Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=6349e046-a3f8-4ae5-b8c3-c9879cc99e8f)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Internetová informační služba 5.1 v systému Windows XP Professional Service Pack 2 a Windows XP Professional Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=97da589f-4534-42f6-9f29-967b5a33c542)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Windows Search 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=759f22cb-ea7f-49dd-a200-19cb83fffd8d)  
(Mírný)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Služba ADAM (Active Directory Application Mode)](http://www.microsoft.com/downloads/details.aspx?familyid=2ef3aaf0-a2a9-4c17-99ab-a0dc3d3f7e86)  
(KB970437)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=22699d09-1e68-456a-8733-bfad6667ebf5)  
(Mírný)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=088f70eb-c5c5-426a-880a-18ed386d0b56)  
(Kritický)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=e5d2c81e-ffab-4e3b-a59a-a55000597213)  
(Kritický)  
[Windows Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=a24aedf0-7a31-4ee8-a9a6-998f1160c700)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=20734b70-37f1-47dd-bc09-d56f93577a55)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3769800e-af93-4a44-8a1e-b30cc54b226f)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Internetová informační služba 6.0](http://www.microsoft.com/downloads/details.aspx?familyid=8982e6d2-e1f7-4208-88e3-80b159a8e21a)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Windows Search 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=50c56dd6-c34d-4632-a779-8bcf8fdb341b)  
(Mírný)
</td>
</tr>
<tr>
<th colspan="8" style="border:1px solid black;">
Windows Server 2003
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS09-018**](http://go.microsoft.com/fwlink/?linkid=151361)
</td>
<td style="border:1px solid black;">
[**MS09-022**](http://go.microsoft.com/fwlink/?linkid=141786)
</td>
<td style="border:1px solid black;">
[**MS09-019**](http://go.microsoft.com/fwlink/?linkid=150860)
</td>
<td style="border:1px solid black;">
[**MS09-026**](http://go.microsoft.com/fwlink/?linkid=150174)
</td>
<td style="border:1px solid black;">
[**MS09-025**](http://go.microsoft.com/fwlink/?linkid=150248)
</td>
<td style="border:1px solid black;">
[**MS09-020**](http://go.microsoft.com/fwlink/?linkid=150568)
</td>
<td style="border:1px solid black;">
[**MS09-023**](http://go.microsoft.com/fwlink/?linkid=143550)
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
[**Mírný**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Mírný**](http://go.microsoft.com/fwlink/?linkid=21140)
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
[**Mírný**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Active Directory](http://www.microsoft.com/downloads/details.aspx?familyid=d814ce65-a193-4027-a6cd-106d388830a6)  
(KB969805)  
(Důležitý)  
[Služba ADAM (Active Directory Application Mode)](http://www.microsoft.com/downloads/details.aspx?familyid=f6f99957-f74f-4446-8734-a468283eebae)  
(KB970437)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=865414f8-3f77-4fee-acc6-6684a3dc0aa4)  
(Mírný)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=72a23752-86fb-4cc9-ab8e-63ffdfae5bec)  
(Mírný)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=a980b867-c67f-4c61-b6db-e55c2ca68dc0)  
(Mírný)  
[Windows Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=298143f2-f37a-4a2c-86ac-9804d4ff1dad)  
(Mírný)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=62bb9e22-4f4b-4ffc-ba76-f626e94c79d5)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=9356404c-d89a-4de0-b9b4-f6e1bdadf745)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Internetová informační služba 6.0](http://www.microsoft.com/downloads/details.aspx?familyid=2bd4e410-dbd8-431a-b316-e1e2f1825c3a)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Windows Search 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=e72ef31f-5161-4fe6-8ed3-6206e02cef31)  
(Mírný)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Active Directory](http://www.microsoft.com/downloads/details.aspx?familyid=0d1f23c8-06eb-4996-92eb-0eb635fd6a42)  
(KB969805)  
(Důležitý)  
[Služba ADAM (Active Directory Application Mode)](http://www.microsoft.com/downloads/details.aspx?familyid=1a2badc7-c0a5-4032-a009-73ebe9d76313)  
(KB970437)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=197a6cc7-4ba3-4d2e-b621-0ef3da645ef2)  
(Mírný)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=2a03d3c4-e39d-43a3-8d42-216e9551be96)  
(Mírný)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=5e7d6372-9c8c-449d-88fd-afd4f92ad9e6)  
(Mírný)  
[Windows Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=4a5401d7-ca97-4734-a0e9-d7ffe0777e34)  
(Mírný)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=888b8dd8-d76c-42f5-a377-1f1750d3cf56)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5a3123af-173d-49eb-9997-14e82e764aee)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Internetová informační služba 6.0](http://www.microsoft.com/downloads/details.aspx?familyid=ea363223-535d-4142-9aba-3890960c6259)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Windows Search 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=7ffc3680-f9bf-423b-96a7-102f4cc9c240)  
(Mírný)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 SP2 pro systémy s procesorem Itanium
</td>
<td style="border:1px solid black;">
[Active Directory](http://www.microsoft.com/downloads/details.aspx?familyid=92e7808b-92ff-449d-bb73-ee8638e9ccd1)  
(KB969805)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=719efd62-fb33-447d-b6dd-2aaafbbad881)  
(Mírný)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=58efde2c-e0b8-4259-b19e-80564b834882)  
(Mírný)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=a2d2907e-67ae-44a4-a805-8670e659ea57)  
(Mírný)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=3084f46e-02b9-4d99-a7a1-033817f9bd9f)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=13b50993-410f-4e7a-a33a-6d9b48dbb4d1)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Internetová informační služba 6.0](http://www.microsoft.com/downloads/details.aspx?familyid=e6b806eb-e2c4-4436-8964-720db593055d)  
(Důležitý)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
</tr>
<tr>
<th colspan="8" style="border:1px solid black;">
Windows Vista
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS09-018**](http://go.microsoft.com/fwlink/?linkid=151361)
</td>
<td style="border:1px solid black;">
[**MS09-022**](http://go.microsoft.com/fwlink/?linkid=141786)
</td>
<td style="border:1px solid black;">
[**MS09-019**](http://go.microsoft.com/fwlink/?linkid=150860)
</td>
<td style="border:1px solid black;">
[**MS09-026**](http://go.microsoft.com/fwlink/?linkid=150174)
</td>
<td style="border:1px solid black;">
[**MS09-025**](http://go.microsoft.com/fwlink/?linkid=150248)
</td>
<td style="border:1px solid black;">
[**MS09-020**](http://go.microsoft.com/fwlink/?linkid=150568)
</td>
<td style="border:1px solid black;">
[**MS09-023**](http://go.microsoft.com/fwlink/?linkid=143550)
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
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
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
<td style="border:1px solid black;">
Žádné
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
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Vista, Windows Vista Service Pack 1 a Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3ad8f037-2434-4dea-bfc3-9d3b4008b828)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=e60215c3-b8b9-4e45-9d9f-b3fb0b47cce1)  
(Kritický)  
[Windows Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=6f2730e9-b4fc-4f20-96cf-73f1be63f374)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Vista, Windows Vista Service Pack 1 a Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5ca227c0-f2dd-429c-a542-e08e93527214)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Windows Vista, Windows Vista Service Pack 1 a Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c31b36f8-330c-4a0c-9a3d-7cbe9a1ab8c8)  
(Důležitý)
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
Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 a Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 a Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=85c317cd-2a14-4747-9f50-3af3ddd3ae1b)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=88185088-8c2c-4bc6-89b2-87f4d4849cf7)  
(Kritický)  
[Windows Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=5edb14f7-11ec-4180-9f0f-b2673f1c8d83)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 a Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=188adafe-1feb-46ad-b237-a88d35104dcd)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 a Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7d70a65f-07ce-4992-8bec-28fefd7587bc)  
(Důležitý)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
</tr>
<tr>
<th colspan="8" style="border:1px solid black;">
Windows Server 2008
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS09-018**](http://go.microsoft.com/fwlink/?linkid=151361)
</td>
<td style="border:1px solid black;">
[**MS09-022**](http://go.microsoft.com/fwlink/?linkid=141786)
</td>
<td style="border:1px solid black;">
[**MS09-019**](http://go.microsoft.com/fwlink/?linkid=150860)
</td>
<td style="border:1px solid black;">
[**MS09-026**](http://go.microsoft.com/fwlink/?linkid=150174)
</td>
<td style="border:1px solid black;">
[**MS09-025**](http://go.microsoft.com/fwlink/?linkid=150248)
</td>
<td style="border:1px solid black;">
[**MS09-020**](http://go.microsoft.com/fwlink/?linkid=150568)
</td>
<td style="border:1px solid black;">
[**MS09-023**](http://go.microsoft.com/fwlink/?linkid=143550)
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
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Mírný**](http://go.microsoft.com/fwlink/?linkid=21140)
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
<tr>
<td style="border:1px solid black;">
Windows Server 2008 pro 32bitové systémy a Windows Server 2008 pro 32bitové systémy Service Pack 2
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro 32bitové systémy a Windows Server 2008 pro 32bitové systémy Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=0f18356d-9f09-4d24-8361-970c0d1ccac4)\*  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=a0e3f975-57da-43fa-ac12-3d14fd6ce939)\*\*  
(Mírný)  
[Windows Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=aaad301c-d232-4733-a0df-8e5d41bbfde8)\*\*  
(Mírný)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro 32bitové systémy a Windows Server 2008 pro 32bitové systémy Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=eaa26c6c-5bf7-4099-bb21-1e03de3a25ca)\*  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro 32bitové systémy a Windows Server 2008 pro 32bitové systémy Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=98ba52b2-da1a-4939-a10e-d43b3a7e7ed4)\*  
(Důležitý)
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
Windows Server 2008 pro systémy s procesorem x64 a Windows Server 2008 pro systémy s procesorem x64 Service Pack 2
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem x64 a Windows Server 2008 pro systémy s procesorem x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7d0a6e8d-a31d-4f3d-a7d7-e61215bfebed)\*  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=758edce7-2a82-4b2e-bd71-5b7075cc4b17)\*\*  
(Mírný)  
[Windows Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=faac92d4-4a2b-4bb5-8bd1-1519a9fa8147)\*\*  
(Mírný)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem x64 a Windows Server 2008 pro systémy s procesorem x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=447aaa4f-946b-4f23-b151-dcf46ea9f80e)\*  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem x64 a Windows Server 2008 pro systémy s procesorem x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=dbaa5a72-c267-4907-a207-525c2803d7b9)\*  
(Důležitý)
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
Windows Server 2008 pro systémy s procesorem Itanium a Windows Server 2008 pro systémy s procesorem Itanium Service Pack 2
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem Itanium a Windows Server 2008 pro systémy s procesorem Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=bbac3deb-6c93-45aa-832c-02b915ac7f44)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=67d4c189-030d-42eb-98b9-7957ccd92592)  
(Mírný)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem Itanium a Windows Server 2008 pro systémy s procesorem Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=f33012b9-5d5b-4f72-8d49-a8e1c8bc1337)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem Itanium a Windows Server 2008 pro systémy s procesorem Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e0e3ad56-a363-44ba-af4d-b7f551c88afd)  
(Důležitý)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
</tr>
</table>
<p></p>
 
**Poznámky k systému Windows Server 2008**

**\*Instalace Server Core operačního systému Windows Server 2008 obsahující tuto chybu.** Tato aktualizace se týká všech podporovaných vydání systému Windows Server 2008 se stejným stupněm závažnosti, ať už byl systém Windows Server 2008 instalován pomocí možnosti instalace Server Core či nikoli. Více informací o této možnosti instalace naleznete v části [Server Core](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx). Možnost instalace Server Core se nevztahuje na určité edice systému Windows Server 2008. Další informace naleznete v části [Porovnání možností instalace Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**\*\*Instalace Server Core operačního systému Windows Server 2008 neobsahující tuto chybu.** Chyby zabezpečení, které tato aktualizace řeší, nemají vliv na podporované edice systému Windows Server 2008, jestliže byl systém Windows Server 2008 instalován s využitím možnosti instalace Server Core. Více informací o této možnosti instalace naleznete v části [Server Core](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx). Možnost instalace Server Core se nevztahuje na určité edice systému Windows Server 2008. Další informace naleznete v části [Porovnání možností instalace Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

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
<th style="border:1px solid black;" >
</th>
</tr>
<tr>
<th colspan="4" style="border:1px solid black;">
Sady Microsoft Office, systémy a komponenty
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS09-027**](http://go.microsoft.com/fwlink/?linkid=147416)
</td>
<td style="border:1px solid black;">
[**MS09-021**](http://go.microsoft.com/fwlink/?linkid=147294)
</td>
<td style="border:1px solid black;">
[**MS09-024**](http://go.microsoft.com/fwlink/?linkid=128104)
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
[**Kritický**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2000 Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Office Word 2000 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=3663e9f2-a952-4238-b902-90b5b09feb38)  
(KB969600)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel 2000 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=dd16e243-b8e2-4afb-86b6-4d60214598eb)  
(KB969683)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Microsoft Office Word 2000 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=4bf95806-3d32-411b-9779-a81aebad45e9)  
(KB957838)  
(Kritický)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Office Word 2002 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=f1323be1-15f2-491b-abae-c03ba1394398)  
(KB969602)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel 2002 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=dd80ce95-0aec-4493-b9d1-c3dad95c3415)  
(KB969680)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Microsoft Office Word 2002 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=b0ba8c9e-75ee-46bd-9e92-d4e6599309ad)  
(KB957646)  
(Důležitý)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2003 Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Office Word 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=7cbc2587-2c8c-49b4-9f40-e4cdccb61ecd)  
(KB969603)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=10156044-a5a4-4312-98a7-1b1ced625ddb)  
(KB969681)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Microsoft Office Word 2003 Service Pack 3 s převaděčem souborů sady Microsoft Works 6-9](http://www.microsoft.com/downloads/details.aspx?familyid=a7ba3ea7-d06a-4c14-9107-9b92ef68fcae)\*\*\*  
(KB968326)  
(Důležitý)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Systém Microsoft Office 2007 Service Pack 1 a systém Microsoft Office 2007 Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft Office Word 2007 Service Pack 1 a Microsoft Office Word 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7e205108-4c28-4cab-a4d0-4ed3fd696473)  
(KB969604)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel 2007 Service Pack 1 a Microsoft Office Excel 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2bcd565a-6acb-407d-80da-0398526ddf99)\*  
(KB969682)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Microsoft Office Word 2007 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=bd47e1e5-cd2e-4c08-9864-471e97f38ca3)  
(KB969559)  
(Důležitý)
</td>
</tr>
<tr>
<th colspan="4" style="border:1px solid black;">
Microsoft Office for Mac
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS09-027**](http://go.microsoft.com/fwlink/?linkid=147416)
</td>
<td style="border:1px solid black;">
[**MS09-021**](http://go.microsoft.com/fwlink/?linkid=147294)
</td>
<td style="border:1px solid black;">
[**MS09-024**](http://go.microsoft.com/fwlink/?linkid=128104)
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
<td style="border:1px solid black;">
Žádné
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2004 for Mac
</td>
<td style="border:1px solid black;">
[Microsoft Office 2004 for Mac](http://www.microsoft.com/downloads/details.aspx?familyid=5557bfb7-ebb4-4c42-8042-41e830c4e550)  
(KB969661)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2004 for Mac](http://www.microsoft.com/downloads/details.aspx?familyid=5557bfb7-ebb4-4c42-8042-41e830c4e550)  
(KB969661)  
(Důležitý)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2008 for Mac
</td>
<td style="border:1px solid black;">
[Microsoft Office 2008 for Mac](http://www.microsoft.com/downloads/details.aspx?familyid=58326da2-eb75-4b42-b1bc-e70319defb58)  
(KB971822)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2008 for Mac](http://www.microsoft.com/downloads/details.aspx?familyid=58326da2-eb75-4b42-b1bc-e70319defb58)  
(KB971822)  
(Důležitý)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Otevření nástroje XML File Format Converter for Mac
</td>
<td style="border:1px solid black;">
[Otevření nástroje XML File Format Converter for Mac](http://www.microsoft.com/downloads/details.aspx?familyid=9d6d9eaa-8442-4184-8886-faab2803bde6)  
(KB971824)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Otevření nástroje XML File Format Converter for Mac](http://www.microsoft.com/downloads/details.aspx?familyid=9d6d9eaa-8442-4184-8886-faab2803bde6)  
(KB971824)  
(Důležitý)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
</tr>
<tr>
<th colspan="4" style="border:1px solid black;">
Jiný software sady Office
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS09-027**](http://go.microsoft.com/fwlink/?linkid=147416)
</td>
<td style="border:1px solid black;">
[**MS09-021**](http://go.microsoft.com/fwlink/?linkid=147294)
</td>
<td style="border:1px solid black;">
[**MS09-024**](http://go.microsoft.com/fwlink/?linkid=128104)
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
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office Excel Viewer
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel Viewer 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=20e6933d-85f8-4cec-9534-893789cd053e)  
(KB969685)  
(Důležitý)  
[Microsoft Office Excel Viewer](http://www.microsoft.com/downloads/details.aspx?familyid=ac0530dc-7f63-4ad0-85c1-784ad28156cf)  
(KB969686)  
(Důležitý)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Word Viewer
</td>
<td style="border:1px solid black;">
[Microsoft Office Word Viewer 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=82980a40-f10c-4f02-b06c-3a12d4434a6b)  
(KB969614)  
(Důležitý)  
[Microsoft Office Word Viewer](http://www.microsoft.com/downloads/details.aspx?familyid=82980a40-f10c-4f02-b06c-3a12d4434a6b)  
(KB969614)  
(Důležitý)
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
Sada Microsoft Office Compatibility Pack pro formáty souborů aplikací Word, Excel a PowerPoint 2007
</td>
<td style="border:1px solid black;">
[Sada Microsoft Office Compatibility Pack pro formáty souborů aplikací Word, Excel a PowerPoint 2007 Service Pack 1 a sada Microsoft Office Compatibility Pack pro formáty souborů aplikací Word, Excel a PowerPoint 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=63bd8f14-e736-46ce-af66-d30f17461e5a)  
(KB969613)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Sada Microsoft Office Compatibility Pack pro formáty souborů aplikací Word, Excel a PowerPoint 2007 Service Pack 1 a sada Microsoft Office Compatibility Pack pro formáty souborů aplikací Word, Excel a PowerPoint 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=a8be8457-b0b6-455e-907e-d13be883adf2)  
(KB969679)  
(Důležitý)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Works 8.5
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Microsoft Works 8.5](http://www.microsoft.com/downloads/details.aspx?familyid=628280fe-e035-4274-85f2-393d9bad543c)  
(KB967043)  
(Důležitý)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Works 9
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Microsoft Works 9](http://www.microsoft.com/downloads/details.aspx?familyid=f6fa110e-45c6-450f-ae47-c89a06e3f762)  
(KB967044)  
(Důležitý)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office SharePoint Server
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Microsoft Office SharePoint Server 2007 Service Pack 1 a Microsoft Office SharePoint Server 2007 Service Pack 2 (32bitové edice)](http://www.microsoft.com/downloads/details.aspx?familyid=862e6ad1-8124-4060-93b1-2b882ef5ce3d)\*\*  
(KB969737)  
(Důležitý)  
[Microsoft Office SharePoint Server 2007 Service Pack 1 a Microsoft Office SharePoint Server 2007 Service Pack 2 (64bitové edice)](http://www.microsoft.com/downloads/details.aspx?familyid=b7b6e611-2c5d-4639-add9-972055789ecd)\*\*  
(KB969737)  
(Důležitý)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
</tr>
</table>
<p></p>
 
**Poznámky k bulletinu MS09-021**

\*Chtějí-li se zákazníci používající aplikaci Microsoft Office Excel 2007 Service Pack 1 či Microsoft Office Excel 2007 Service Pack 2 chránit před chybami zabezpečení popsanými v tomto bulletinu, je nutné, aby si vedle aktualizace uvedené v článku KB969682 znalostní báze nainstalovali také aktualizaci zabezpečení pro sadu [Microsoft Office Compatibility Pack pro formáty souborů aplikací Word, Excel a PowerPoint 2007 Service Pack 1 a Microsoft Office Compatibility Pack pro formáty souborů aplikací Word, Excel a PowerPoint 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=a8be8457-b0b6-455e-907e-d13be883adf2) (KB969679).

\*\*Tato aktualizace se týká serverů, které mají naistalovánu službu Excel Services, jak je tomu například u aplikací Microsoft Office SharePoint Server 2007 Enterprise a Microsoft Office SharePoint Server 2007 For Internet Sites ve výchozí konfiguraci. Aplikace Microsoft Office SharePoint Server 2007 Standard neobsahuje službu Excel Services.

**Poznámka k bulletinu MS09-024**

\*\*\*Aplikace Microsoft Office Word 2003 je postižena, pokud je nainstalován převaděč sady Works obsahující chybu zabezpečení. Převaděče sady Works jsou k dispozici ke stažení pro aplikaci Microsoft Office Word 2003 z webu [převaděč souborů sady Microsoft Works 6-9](http://www.microsoft.com/downloads/details.aspx?familyid=bf41401e-70fa-465d-ae2e-cf44dbf05297&displaylang=en).

Nástroje a doporučené postupy zjišťování a nasazení
---------------------------------------------------

 
**Centrum zabezpečení**

Umožňuje správu aktualizací softwaru a zabezpečení, které je třeba nainstalovat na servery, stolní počítače a přenosné počítače v organizaci. Další informace naleznete na webu [TechNet Update Management Center](http://go.microsoft.com/fwlink/?linkid=69903). Další informace o zabezpečení produktů společnosti Microsoft nabízí web [Centrum zabezpečení TechNet](http://go.microsoft.com/fwlink/?linkid=21171). Tyto informace lze také získat kliknutím na nabídku „Nejnovější aktualizace zabezpečení“ na webu [Zabezpečení doma](http://go.microsoft.com/fwlink/?linkid=85102).

Aktualizace zabezpečení jsou k dispozici na webu [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747), [Windows Update](http://go.microsoft.com/fwlink/?linkid=21130) a [Office Update](http://go.microsoft.com/fwlink/?linkid=21135). Aktualizace zabezpečení jsou také k dispozici na webu [služby Stažení softwaru](http://go.microsoft.com/fwlink/?linkid=21129). Nejsnadněji je naleznete hledáním podle klíčových slov aktualizace zabezpečení.

Aktualizace zabezpečení lze stáhnout z katalogu služby [Microsoft Update Catalog](http://go.microsoft.com/fwlink/?linkid=96155). Služba Microsoft Update Catalog poskytuje katalog s možností vyhledávání obsahu dostupného prostřednictvím služeb Windows Update a Microsoft Update, včetně aktualizací zabezpečení, ovladačů a aktualizací Service Pack. Vyhledáváním pomocí čísla bulletinu zabezpečení (například MS07-036) můžete přidat všechny dostupné aktualizace do košíku (včetně různých jazykových verzí aktualizace) a stáhnout je do vybrané složky. Další informace o službě Microsoft Update Catalog najdete v části [Nejčastější dotazy týkající se služby Microsoft Update Catalog](http://go.microsoft.com/fwlink/?linkid=97900).

**Doporučené postupy zjišťování a instalace**

Společnost Microsoft poskytla doporučené postupy zjišťování a instalace aktualizací zabezpečení vydaných tento měsíc. Tyto doporučené postupy by měly pomoci také odborníkům v oblasti IT při používání různých nástrojů při instalaci aktualizace zabezpečení, např. Windows Update, Microsoft Update, Office Update, nástroj MBSA (Microsoft Baseline Security Analyzer), nástroj pro rozpoznávání sady Office, Microsoft Systems Management Server (SMS) a nástroj Extended Security Update Inventory Tool (ESUIT). Další informace získáte v [článku 910723 znalostní báze Microsoft Knowledge Base](http://support.microsoft.com/kb/910723/cs).

**Nástroj Microsoft Baseline Security Analyzer**

Pomocí nástroje Microsoft Baseline Security Analyzer (MBSA) mohou správci prohledávat místní i vzdálené systémy a zjistit tak, jestli v nich nechybí některé aktualizace zabezpečení nebo jestli v nastavení zabezpečení systému nedošlo k některým běžným chybám. Další informace o nástroji MBSA získáte na webu [Microsoft Baseline Security Analyzer](http://go.microsoft.com/fwlink/?linkid=21134).

**Služba Windows Server Update Services**

Pomocí služby Windows Server Update Services (WSUS) mohou správci systémů rychle a spolehlivě instalovat nejnovější důležité aktualizace zabezpečení pro systémy Windows 2000 a novější, sadu Office XP a novější, Exchange Server 2003 a SQL Server 2000 do systémů Windows 2000 a novějších.

Další informace o způsobu instalace této aktualizace zabezpečení pomocí služby Windows Server Update Services získáte na webu služby [Windows Server Update Services](http://go.microsoft.com/fwlink/?linkid=50120).

**Systems Management Server**

Microsoft Systems Management Server (SMS) představuje v rozlehlých sítích řešení pro správu aktualizací s rozsáhlými možnostmi konfigurace. Umožňuje správcům identifikovat počítače se systémem Windows, které vyžadují aktualizace zabezpečení, a provést řízenou instalaci těchto aktualizací v celé rozlehlé síti s minimálním dopadem na koncové uživatele. K dispozici je nyní nová verze nástroje SMS, System Center Configuration Manager 2007 (viz také webové stránky produktu [System Center Configuration Manager 2007](http://technet.microsoft.com/en-us/library/bb735860.aspx)). Další informace o tom, jak mohou správci pomocí serveru SMS 2003 nasazovat aktualizace zabezpečení, získáte na webu [SMS 2003 Security Patch Management](http://go.microsoft.com/fwlink/?linkid=22939). Uživatelé serveru SMS 2.0 mohou při nasazení aktualizací zabezpečení použít také sadu [Software Updates Services Feature Pack](http://go.microsoft.com/fwlink/?linkid=33340). Další informace o serveru SMS získáte na webu [Microsoft Systems Management Server](http://go.microsoft.com/fwlink/?linkid=21158).

**Poznámka:** Server SMS využívá nástroj MBSA (Microsoft Baseline Security Analyzer) a nástroj pro rozpoznávání sady Microsoft Office, a poskytuje tak širokou podporu pro zjišťování a instalaci aktualizací uvedených v bulletinech zabezpečení. Tyto nástroje nemusí některé softwarové aktualizace zjistit. V takovém případě mohou správci použít funkce serveru SMS a nasměrovat aktualizace do určitých systémů. Další informace o tomto postupu najdete na webu [Nasazení aktualizací softwaru pomocí funkce Distribuce softwaru serveru SMS](http://go.microsoft.com/fwlink/?linkid=33341). Některé aktualizace zabezpečení vyžadují po restartování počítače oprávnění správce. Správci mohou k instalaci těchto aktualizací použít nástroj Elevated Rights Deployment Tool (k dispozici v sadě [SMS 2003 Administration Feature Pack](http://go.microsoft.com/fwlink/?linkid=33387) a [SMS 2.0 Administration Feature Pack](http://go.microsoft.com/fwlink/?linkid=21161)).

**Nástroj Update Compatibility Evaluator a sada Application Compatibility Toolkit**

Aktualizace často zapisují do stejných souborů a nastavení registru požadovaných pro spouštění aplikací. To může způsobit nekompatibilitu a zvýšit dobu, po kterou trvá nasazení aktualizací zabezpečení. Testování a ověřování aktualizací systému Windows lze usnadnit pomocí součástí nástroje [Update Compatibility Evaluator](http://technet2.microsoft.com/windowsvista/en/library/4279e239-37a4-44aa-aec5-4e70fe39f9de1033.mspx?mfr=true), které jsou dodávány se sadou [Application Compatibility Toolkit 5.0](http://www.microsoft.com/downloads/details.aspx?familyid=24da89e9-b581-47b0-b45e-492dd6da2971&displaylang=en).

Sada Application Compatibility Toolkit (ACT) obsahuje nezbytné nástroje a dokumentaci pro posouzení a zmírnění problémů s kompatibilitou aplikací před nasazením systému Microsoft Windows Vista, služby Windows Update, aktualizací zabezpečení společnosti Microsoft nebo nové verze aplikace Windows Internet Explorer ve vašem prostředí.

### Další informace

#### Nástroj pro odstranění škodlivého softwaru systému Microsoft Windows

Společnost Microsoft vydává aktualizovanou verzi Nástroje pro odstranění škodlivého softwaru systému Microsoft Windows na webu Windows Update, Microsoft Update, ve službě Windows Server Update Services a na webu služby Stažení softwaru.

#### Důležité aktualizace nesouvisející se zabezpečením na webu Microsoft Update (MU), Windows Update (WU) a ve službě Windows Server Update Services (WSUS)

Informace o aktualizacích nesouvisejících se zabezpečením na webu Windows Update a Microsoft Update naleznete na webové stránce:

-   [Článek 894199 znalostní báze Microsoft Knowledge Base](http://support.microsoft.com/kb/894199/cs): Popis služeb Software Update Services a Windows Server Update Services se mění v obsahu. Zahrnuje celý obsah systému Windows.
-   [Nové, revidované a vydané aktualizace pro jiné produkty společnosti Microsoft, než je systém Microsoft Windows](http://technet.microsoft.com/en-us/wsus/dd573344.aspx).

#### Microsoft Active Protections Program (MAPP)

Pro zlepšení ochrany dat svých zákazníků poskytuje společnost Microsoft informace o chybách v zabezpečení všem hlavním dodavatelům softwaru pro zabezpečení, a to vždy ještě před vydáním nové měsíční zprávy o aktualizaci zabezpečení. Dodavatelé softwaru pro zabezpečení tak mohou tyto informace o chybách v zabezpečení využít a poskytnout svým zákazníkům ochranu včasnou aktualizací svých programů a zařízení pro zabezpečení, jako jsou antivirové programy, síťové systémy pro detekci napadení či hostitelské systémy pro prevenci napadení. Informace o dostupnosti aktuálních prostředků aktivní ochrany od jednotlivých dodavatelů softwaru pro zabezpečení naleznete na stránkách aktivní ochrany jednotlivých partnerů programu MAPP. Seznam těchto partnerů naleznete na stránce [Microsoft Active Protections Program (MAPP) Partners](http://www.microsoft.com/security/msrc/mapp/partners.mspx).

#### Strategie zabezpečení a komunita

**Strategie instalace aktualizací**

Web [Doporučené postupy zabezpečení pro správu aktualizací (Security Guidance for Update Management)](http://go.microsoft.com/fwlink/?linkid=21168) obsahuje další informace o instalaci aktualizací zabezpečení podle doporučení společnosti Microsoft.

**Získání dalších aktualizací zabezpečení**

Aktualizace odstraňující další problémy se zabezpečením získáte v následujících umístěních:

-   Aktualizace zabezpečení jsou k dispozici na webu služby [Stažení softwaru (Microsoft Download Center)](http://go.microsoft.com/fwlink/?linkid=21129). Nejsnadněji je naleznete hledáním podle klíčových slov aktualizace zabezpečení.
-   Aktualizace pro klientské platformy jsou k dispozici na webu [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747).
-   Aktualizace zabezpečení nabízené tento měsíc na webu Windows Update jsou k dispozici na webu služby Stažení softwaru v souborech obrazu ISO disku CD s vydanými aktualizacemi zabezpečení a kritickými aktualizacemi. Další informace získáte v [článku 913086 znalostní báze Microsoft Knowledge Base](http://support.microsoft.com/kb/913086/cs).

**Komunita odborníků v oblasti zabezpečení**

Můžete se zde naučit, jak zlepšit zabezpečení a jak optimalizovat infrastrukturu IT. Také můžete s dalšími členy komunity IT Pro diskutovat o bezpečnostních tématech na webu [Komunita odborníků v oblasti zabezpečení (IT Pro Security Community)](http://go.microsoft.com/fwlink/?linkid=21164).

#### Poděkování

Společnost Microsoft tímto [děkuje](http://go.microsoft.com/fwlink/?linkid=21127) za spolupráci při ochraně zákazníků:

-   Joshuovi J. Drakeovi ze společnosti [Verisign iDefense Labs](http://labs.idefense.com/) za oznámení chyby popsané v bulletinu MS09-018.
-   Justinu Wyattovi ze [školního okrsku Beaverton](http://www.beaverton.k12.or.us/home/) za oznámení chyby popsané v bulletinu MS09-018.
-   Davidu Bloomovi ze společnosti [Google Inc.](http://www.google.com/) za spolupráci na řešení chyby popsané v bulletinu MS09-019.
-   Jorge Luisovi Alvarez Medinovi ze společnosti [Core Security Technologies](http://www.coresecurity.com/) za oznámení chyby popsané v bulletinu MS09-019.
-   Haifei Liovi ze společnosti [Fortinet](http://www.fortinet.com/) za oznámení chyby popsané v bulletinu MS09-019.
-   Společnosti [TippingPoint](http://www.tippingpoint.com/) a organizaci [Zero Day Initiative](http://www.zerodayinitiative.com/) za oznámení chyby popsané v bulletinu MS09-019.
-   Peteru Vreugdenhilovi, spolupracujícímu se společností [TippingPoint](http://www.tippingpoint.com/) a organizací [Zero Day Initiative](http://www.zerodayinitiative.com/), za oznámení chyby popsané v bulletinu MS09-019.
-   Wushimu, spolupracujícímu se společností [TippingPoint](http://www.tippingpoint.com/) a organizací [Zero Day Initiative](http://www.zerodayinitiative.com/), za oznámení dvou chyb popsaných v bulletinu MS09-019.
-   Nilsovi, spolupracujícímu se společností [TippingPoint](http://www.tippingpoint.com/) a organizací [Zero Day Initiative](http://www.zerodayinitiative.com/), za oznámení chyby popsané v bulletinu MS09-019.
-   Yamatu Liovi ze společnosti [Palo Alto Networks](http://www.paloaltonetworks.com/) za oznámení chyby popsané v bulletinu MS09-020.
-   Bingu Liuovi z výzkumného týmu [FortiGuard Global Security Research Team](http://www.fortiguardcenter.com/) společnosti Fortinet za oznámení tří chyb popsaných v bulletinu MS09-021.
-   Carstenu H. Eiramovi ze společnosti [Secunia](http://secunia.com/) za oznámení dvou chyb popsaných v bulletinu MS09-021.
-   [Výzkumnému týmu chyb zabezpečení společnosti TELUS Security Labs](http://telussecuritylabs.com/) za oznámení chyby popsané v bulletinu MS09-021.
-   Seanu Larssonovi a Joshua Drakeovi ze společnosti [VeriSign iDefense Labs](http://labs.idefense.com/) za oznámení chyby popsané v bulletinu MS09-021.
-   Společnosti [TippingPoint](http://www.tippingpoint.com/) a organizaci [Zero Day Initiative](http://www.zerodayinitiative.com/) za oznámení chyby popsané v bulletinu MS09-021.
-   Junu Maovi ze společnosti [VeriSign iDefense Labs](http://labs.idefense.com/) za oznámení chyby popsané v bulletinu MS09-022.
-   Yairu Amitovi z oddělení [IBM Rational Application Security](http://blog.watchfire.com/) za oznámení chyby popsané v bulletinu MS09-023.
-   Shaunu Colleymu ze společnosti [NGS Software](http://www.ngssoftware.com/) za oznámení chyby popsané v bulletinu MS09-024.
-   Thomasi Garnierovi za oznámení dvou chyb popsaných v bulletinu MS09-025.
-   Wushimu ze skupiny [team509](http://www.team509.com/), spolupracujícímu s organizací [Zero Day Initiative](http://www.zerodayinitiative.com/), za oznámení chyby popsané v bulletinu MS09-027.
-   Nicolasi Jolymu ze společnosti [VUPEN Security](http://www.vupen.com/) za oznámení chyby popsané v bulletinu MS09-027.

#### Technická podpora

-   Uvedený software byl testován za účelem zjištění, kterých verzí se chyba týká. U dalších verzí skončila časově omezená podpora. Pokud chcete zjistit dobu, po kterou je pro určitou verzi softwaru poskytována podpora, navštivte web [Zásady poskytování technické podpory pro produkty společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=21742).
-   Zákazníci mohou získat technickou podporu na webu [služby technické podpory společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=21131). Hovory související s aktualizacemi zabezpečení jsou bezplatné. Další informace o dostupných možnostech technické podpory naleznete na webu [Pomoc a podpora společnosti Microsoft](http://support.microsoft.com/?ln=cs).
-   Mezinárodní zákazníci získají podporu u místních zastoupení společnosti Microsoft. Technická podpora související s aktualizacemi zabezpečení je bezplatná. Další informace o možnostech kontaktování společnosti Microsoft v případě potřeby technické podpory získáte na [webu mezinárodní technické podpory](http://go.microsoft.com/fwlink/?linkid=21155).

#### Zřeknutí se záruky

Informace ve znalostní bázi Microsoft Knowledge Base jsou poskytovány tak, jak jsou, bez jakékoli záruky. Společnost Microsoft neposkytuje žádné záruky, výslovně uvedené či mlčky předpokládané, včetně záruk obchodovatelnosti a vhodnosti pro určitý účel. Společnost Microsoft ani její dodavatelé nenesou v žádném případě zodpovědnost za žádné škody, včetně přímých, nepřímých, náhodných či následných škod, ztráty zisku či zvláštních škod, a to ani v případě, že byli na možnost takových škod upozorněni. V některých zemích a právních řádech není dovoleno vyloučit nebo omezit odpovědnost, proto se výše uvedené omezení na vás nemusí vztahovat.

#### Revize

-   V1.0 (9. června 2009): Souhrnný bulletin byl publikován.

*Built at 2014-04-18T01:50:00Z-07:00*
