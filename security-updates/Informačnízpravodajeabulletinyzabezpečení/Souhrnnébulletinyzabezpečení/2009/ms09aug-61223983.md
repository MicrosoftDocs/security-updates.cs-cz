---
TOCTitle: 'MS09-AUG'
Title: 'Souhrnný bulletin zabezpečení společnosti Microsoft, srpen 2009'
ms:assetid: 'ms09-aug'
ms:contentKeyID: 61223983
ms:mtpsurl: 'https://technet.microsoft.com/cs-CZ/library/ms09-aug(v=Security.10)'
---

Security Bulletin Summary

Souhrnný bulletin zabezpečení společnosti Microsoft, srpen 2009
===============================================================

Publikováno: 11. srpna 2009 | Aktualizováno: 27. října 2009

**Verze:** 4.0

Tento souhrnný bulletin uvádí bulletiny zabezpečení vydané v srpnu 2009.

Spolu s vydáním bulletinů pro srpen 2009 nahrazuje tento souhrnný bulletin předběžné oznámení o bulletinech vydané 6. srpna 2009. Další informace o službě předběžného oznámení o bulletinech naleznete v části [Předběžné oznámení o bulletinech zabezpečení společnosti Microsoft](http://technet.microsoft.com/security/bulletin/advance).

Informace o tom, jak dostávat automatická oznámení o vydání nových bulletinů zabezpečení společnosti Microsoft, naleznete na webu [Zasílání technických oznámení o zabezpečení společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=21163).

Pro zodpovězení zákaznických dotazů týkajících se těchto bulletinů uspořádá společnost Microsoft webové vysílání 12. srpna 2009 v 11:00 časového pásma Tichomoří (USA a Kanada). [Registrovat se pro webové vysílání týkající se srpnových bulletinů zabezpečení](http://msevents.microsoft.com/cui/webcasteventdetails.aspx?eventid=1032407484&eventcategory=4&culture=en-us&countrycode=us). Po tomto datu je webové vysílání dostupné na požádání. Další informace získáte v [souhrnných bulletinech zabezpečení společnosti Microsoft a webovém vysílání](http://technet.microsoft.com/security/bulletin/summary).

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
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=128110">MS09-043</a></td>
<td style="border:1px solid black;"><strong>Chyby zabezpečení v součástech Microsoft Office Web Components umožňují vzdálené spuštění kódu (957638)</strong><br />
<br />
Tato aktualizace zabezpečení řeší několik chyb zabezpečení součástí Microsoft Office Web Components oznámených soukromými osobami, které by mohly umožnit vzdálené spuštění kódu v případě, že uživatel otevře speciálně vytvořenou webovou stránku. Útočník, který by úspěšně zneužil tyto chyby zabezpečení, by mohl získat stejná uživatelská práva, jaká má místní uživatel. Uživatelé, jejichž účty jsou konfigurovány tak, aby měli v systému méně uživatelských práv, by byli vystaveni menšímu riziku než uživatelé s uživatelskými právy správce.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritický</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Může vyžadovat restartování</td>
<td style="border:1px solid black;">Microsoft Office, Microsoft Visual Studio, Microsoft ISA Server, Microsoft BizTalk Server</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=157861">MS09-044</a></td>
<td style="border:1px solid black;"><strong>Chyby zabezpečení v programu Připojení ke vzdálené ploše umožňují vzdálené spuštění kódu (970927)</strong><br />
<br />
Tato aktualizace zabezpečení řeší dvě chyby zabezpečení v programu Připojení ke vzdálené ploše, které oznámily soukromé osoby. Tyto chyby zabezpečení by mohly umožnit vzdálené spuštění kódu, kdyby se útočníkovi podařilo přesvědčit uživatele Terminálové služby, aby se připojil ke škodlivému serveru, nebo kdyby uživatel navštívil speciálně vytvořený web, který tuto chybu zabezpečení zneužívá. Uživatelé, jejichž účty jsou konfigurovány tak, aby měli v systému méně uživatelských práv, by byli vystaveni menšímu riziku než uživatelé s uživatelskými právy správce.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritický</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Může vyžadovat restartování</td>
<td style="border:1px solid black;">Microsoft Windows, klient Připojení ke vzdálené ploše pro systém Mac</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=155974">MS09-039</a></td>
<td style="border:1px solid black;"><strong>Chyby zabezpečení v protokolu WINS umožňují vzdálené spuštění kódu (969883)</strong><br />
<br />
Tato aktualizace zabezpečení řeší dvě chyby zabezpečení ve službě WINS (Windows Internet Name Service) oznámené soukromými osobami. Tyto chyby zabezpečení mohou umožnit vzdálené spuštění kódu, pokud by uživatel obdržel speciálně vytvořený replikační paket služby WINS v postiženém systému používajícím službu WINS. Ve výchozím nastavení není služba WINS nainstalována v žádné verzi postiženého operačního systému. Tento problém se týká pouze zákazníků, kteří tuto komponentu nainstalovali ručně.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritický</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=155975">MS09-038</a></td>
<td style="border:1px solid black;"><strong>Chyby zabezpečení při zpracování souborů služby Windows Media umožňují vzdálené spuštění kódu (971557)</strong><br />
<br />
Tato aktualizace zabezpečení řeší dvě chyby zabezpečení při zpracování souborů služby Windows Media oznámené soukromými osobami. Tyto chyby zabezpečení umožňují vzdálené spuštění kódu, pokud uživatel otevře speciálně vytvořený soubor ve formátu AVI. Pokud by byl uživatel přihlášen s uživatelskými právy správce, mohl by útočník, který by tuto chybu zabezpečení zneužil, získat úplnou kontrolu nad postiženým systémem. Útočník by tak mohl instalovat programy, zobrazovat, měnit či odstraňovat data nebo vytvářet nové účty s úplnými uživatelskými právy. Uživatelé, jejichž účty jsou konfigurovány tak, aby měli v systému méně uživatelských práv, by byli vystaveni menšímu riziku než uživatelé s uživatelskými právy správce.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritický</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=158695">MS09-037</a></td>
<td style="border:1px solid black;"><strong>Chyby zabezpečení v knihovně Microsoft Active Template Library (ATL) umožňují vzdálené spuštění kódu (973908)</strong><br />
<br />
Tato aktualizace zabezpečení řeší několik chyb zabezpečení knihovny Microsoft Active Template Library (ATL), které oznámily soukromé osoby. Tyto chyby zabezpečení by mohly umožnit vzdálené spuštění kódu, kdyby uživatel načetl speciálně vytvořenou komponentu nebo ovládací prvek, jehož hostitelem je škodlivý web. Uživatelé, jejichž účty jsou konfigurovány tak, aby měli v systému méně uživatelských práv, by byli vystaveni menšímu riziku než uživatelé s uživatelskými právy správce.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritický</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Může vyžadovat restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=155977">MS09-041</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení služby Pracovní stanice umožňuje zvýšení úrovně oprávnění (971657)</strong><br />
<br />
Tato aktualizace zabezpečení řeší chybu zabezpečení služby Pracovní stanice Windows oznámenou soukromou osobou. Tato chyba zabezpečení by mohla umožnit zvýšení úrovně oprávnění, pokud by útočník vytvořil speciální zprávu RPC a odeslal ji do postiženého systému. Útočník, který by tuto chybu zabezpečení úspěšně zneužil, by mohl spustit libovolný kód a získat úplnou kontrolu nad postiženým systémem. Útočník by tak mohl instalovat programy, zobrazovat, měnit či odstraňovat data nebo vytvářet nové účty s úplnými uživatelskými právy. Tuto chybu může zneužít pouze útočník s platnými pověřeními pro přihlášení k postiženému systému. Tuto chybu zabezpečení nemohou zneužít anonymní uživatelé.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Vysoký</a><br />
Zvýšení úrovně oprávnění</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=155979">MS09-040</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení služby Řízení front zpráv umožňuje zvýšení úrovně oprávnění (971032)</strong><br />
<br />
Tato aktualizace zabezpečení řeší chybu zabezpečení služby Řízení front zpráv oznámenou soukromou osobou. Tato chyba zabezpečení by mohla umožnit zvýšení úrovně oprávnění, pokud by uživatel přijal speciálně vytvořený požadavek v postižené službě MSMQ. Součást Řízení front zpráv se v žádné z verzí operačního systému, které tuto chybu zabezpečení obsahují, ve výchozím nastavení neinstaluje a může ji povolit pouze uživatel s oprávnění pro správu. Touto chybou zabezpečení mohou být ohroženi pouze zákazníci, kteří ručně nainstalovali součást Message Queuing.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Vysoký</a><br />
Zvýšení úrovně oprávnění</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=157296">MS09-036</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení v rozhraní ASP.NET systému Microsoft Windows může způsobit odmítnutí služby (970957)</strong><br />
<br />
Tato aktualizace zabezpečení řeší chybu zabezpečení způsobující odmítnutí služby v součásti Microsoft .NET Framework systému Microsoft Windows, kterou oznámila soukromá osoba. Tuto chybu zabezpečení lze zneužít pouze tehdy, je-li nainstalována Internetová informační služba (IIS) 7.0 a rozhraní ASP.NET je nakonfigurováno tak, aby používalo integrovaný režim v postižených verzích systému Microsoft Windows. Útočník by mohl vytvořit speciální anonymní požadavky HTTP, které by mohly způsobit, že postižený webový server přestane reagovat, dokud nebude restartován přidružený fond aplikací. Touto chybou zabezpečení nejsou ovlivněni zákazníci, kteří používají fondy aplikací služby IIS 7.0 v klasickém režimu.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Vysoký</a><br />
Odmítnutí služby</td>
<td style="border:1px solid black;">Nevyžaduje restart</td>
<td style="border:1px solid black;">Microsoft Windows, Microsoft .NET Framework</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=157140">MS09-042</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení ve službě Telnet umožňuje vzdálené spuštění kódu (960859)</strong><br />
<br />
Tato aktualizace zabezpečení řeší veřejně známou chybu zabezpečení služby Microsoft Telnet. Tato chyba zabezpečení by mohla útočníkovi umožnit získání oprávnění a jejich následné použití pro přihlášení zpět do postižených systémů. Pak by uživatel získal uživatelská práva do systému totožná s uživatelskými právy přihlášeného uživatele. Tento scénář by mohl nevyhnutelně vést ke vzdálenému spuštění kódu v postižených systémech. Útočník, který by úspěšně zneužil tuto chybu zabezpečení, by tak mohl instalovat programy, zobrazovat, měnit či odstraňovat data nebo vytvářet nové účty s úplnými uživatelskými právy. Uživatelé, jejichž účty jsou konfigurovány tak, aby měli v systému méně uživatelských práv, by byli vystaveni menšímu riziku než uživatelé s uživatelskými právy správce.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Vysoký</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Může vyžadovat restartování</td>
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
  
| ID bulletinu                                              | Název bulletinu                                                                                               | ID CVE                                                                           | Hodnocení indexu zneužitelnosti                                                                                                | Hlavní poznámky                                                                                                                                                                                                                                                               |  
|-----------------------------------------------------------|---------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| [MS09-036](http://go.microsoft.com/fwlink/?linkid=157296) | Chyba zabezpečení v rozhraní ASP.NET systému Microsoft Windows může způsobit odmítnutí služby (970957)        | [CVE-2009-1536](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1536) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Vytvoření funkčního zneužitelného kódu není pravděpodobné | Odmítnutí služby je pravděpodobné. Vytvoření funkčního zneužitelného kódu pro vzdálené spuštění kódu ovšem pravděpodobné není.                                                                                                                                                |  
| [MS09-037](http://go.microsoft.com/fwlink/?linkid=158695) | Chyby zabezpečení v knihovně Microsoft Active Template Library (ATL) umožňují vzdálené spuštění kódu (973908) | [CVE-2008-0015](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-0015) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní zneužití kódu je pravděpodobné               | **V současné době dochází ke zneužití této chyby zabezpečení v prostředí Internetu.**                                                                                                                                                                                         |  
| [MS09-037](http://go.microsoft.com/fwlink/?linkid=158695) | Chyby zabezpečení v knihovně Microsoft Active Template Library (ATL) umožňují vzdálené spuštění kódu (973908) | [CVE-2008-0020](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-0020) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní zneužití kódu je pravděpodobné               | (Žádné)                                                                                                                                                                                                                                                                       |  
| [MS09-037](http://go.microsoft.com/fwlink/?linkid=158695) | Chyby zabezpečení v knihovně Microsoft Active Template Library (ATL) umožňují vzdálené spuštění kódu (973908) | [CVE-2009-0901](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0901) | Žádné                                                                                                                          | (Této chybě zabezpečení byl přidělen index zneužitelnosti již v [červencovém souhrnném bulletinu](http://technet.microsoft.com/security/bulletin/ms09-jul). Tato chyba zabezpečení se poprvé objevila v bulletinu [MS09-035](http://go.microsoft.com/fwlink/?linkid=158131).) |  
| [MS09-037](http://go.microsoft.com/fwlink/?linkid=158695) | Chyby zabezpečení v knihovně Microsoft Active Template Library (ATL) umožňují vzdálené spuštění kódu (973908) | [CVE-2009-2493](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2493) | Žádné                                                                                                                          | (Této chybě zabezpečení byl přidělen index zneužitelnosti již v [červencovém souhrnném bulletinu](http://technet.microsoft.com/security/bulletin/ms09-jul). Tato chyba zabezpečení se poprvé objevila v bulletinu [MS09-035](http://go.microsoft.com/fwlink/?linkid=158131).) |  
| [MS09-037](http://go.microsoft.com/fwlink/?linkid=158695) | Chyby zabezpečení v knihovně Microsoft Active Template Library (ATL) umožňují vzdálené spuštění kódu (973908) | [CVE-2009-2494](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2494) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní zneužití kódu je pravděpodobné               | (Žádné)                                                                                                                                                                                                                                                                       |  
| [MS09-038](http://go.microsoft.com/fwlink/?linkid=155975) | Chyby zabezpečení při zpracování souborů služby Windows Media umožňují vzdálené spuštění kódu (971557)        | [CVE-2009-1545](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1545) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Nekonsistentní zneužití kódu je pravděpodobné             | (Žádné)                                                                                                                                                                                                                                                                       |  
| [MS09-038](http://go.microsoft.com/fwlink/?linkid=155975) | Chyby zabezpečení při zpracování souborů služby Windows Media umožňují vzdálené spuštění kódu (971557)        | [CVE-2009-1546](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1546) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Nekonsistentní zneužití kódu je pravděpodobné             | (Žádné)                                                                                                                                                                                                                                                                       |  
| [MS09-039](http://go.microsoft.com/fwlink/?linkid=155974) | Chyby zabezpečení ve službě WINS umožňují vzdálené spuštění kódu (969883)                                     | [CVE-2009-1923](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1923) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní zneužití kódu je pravděpodobné               | (Žádné)                                                                                                                                                                                                                                                                       |  
| [MS09-039](http://go.microsoft.com/fwlink/?linkid=155974) | Chyby zabezpečení ve službě WINS umožňují vzdálené spuštění kódu (969883)                                     | [CVE-2009-1924](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1924) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Nekonsistentní zneužití kódu je pravděpodobné             | Pravděpodobnost zneužití se zvyšuje v systému Windows 2000.                                                                                                                                                                                                                   |  
| [MS09-040](http://go.microsoft.com/fwlink/?linkid=155979) | Chyba zabezpečení služby Řízení front zpráv umožňuje zvýšení úrovně oprávnění (971032)                        | [CVE-2009-1922](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1922) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní zneužití kódu je pravděpodobné               | Vzdálený útok na tuto chybu zabezpečení nelze provést.                                                                                                                                                                                                                        |  
| [MS09-041](http://go.microsoft.com/fwlink/?linkid=155977) | Chyba zabezpečení služby Pracovní stanice umožňuje zvýšení úrovně oprávnění (971657)                          | [CVE-2009-1544](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1544) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní zneužití kódu je pravděpodobné               | Podmínkou pro zneužití této chyby zabezpečení by bylo ověření útočníka.                                                                                                                                                                                                       |  
| [MS09-042](http://go.microsoft.com/fwlink/?linkid=157140) | Chyba zabezpečení ve službě Telnet umožňuje vzdálené spuštění kódu (960859)                                   | [CVE-2009-1930](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1930) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní zneužití kódu je pravděpodobné               | Tato chyba zabezpečení se podobá dřívějším chybám zabezpečení reflexe pověření pro přihlášení NTLM, pro které již zneužitelný kód existuje.                                                                                                                                   |  
| [MS09-043](http://go.microsoft.com/fwlink/?linkid=128110) | Chyby zabezpečení v součástech Microsoft Office Web Components umožňují vzdálené spuštění kódu (957638)       | [CVE-2009-0562](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0562) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní zneužití kódu je pravděpodobné               | (Žádné)                                                                                                                                                                                                                                                                       |  
| [MS09-043](http://go.microsoft.com/fwlink/?linkid=128110) | Chyby zabezpečení v součástech Microsoft Office Web Components umožňují vzdálené spuštění kódu (957638)       | [CVE-2009-1136](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1136) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní zneužití kódu je pravděpodobné               | Zneužitelný kód pro tuto chybu zabezpečení byl veřejně publikován.                                                                                                                                                                                                            |  
| [MS09-043](http://go.microsoft.com/fwlink/?linkid=128110) | Chyby zabezpečení v součástech Microsoft Office Web Components umožňují vzdálené spuštění kódu (957638)       | [CVE-2009-1534](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1534) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní zneužití kódu je pravděpodobné               | (Žádné)                                                                                                                                                                                                                                                                       |  
| [MS09-043](http://go.microsoft.com/fwlink/?linkid=128110) | Chyby zabezpečení v součástech Microsoft Office Web Components umožňují vzdálené spuštění kódu (957638)       | [CVE-2009-2496](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2496) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní zneužití kódu je pravděpodobné               | (Žádné)                                                                                                                                                                                                                                                                       |  
| [MS09-044](http://go.microsoft.com/fwlink/?linkid=157861) | Chyby zabezpečení v programu Připojení ke vzdálené ploše umožňují vzdálené spuštění kódu (970927)             | [CVE-2009-1133](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1133) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Nekonsistentní zneužití kódu je pravděpodobné             | (Žádné)                                                                                                                                                                                                                                                                       |  
| [MS09-044](http://go.microsoft.com/fwlink/?linkid=157861) | Chyby zabezpečení v programu Připojení ke vzdálené ploše umožňují vzdálené spuštění kódu (970927)             | [CVE-2009-1929](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1929) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní zneužití kódu je pravděpodobné               | (Žádné)                                                                                                                                                                                                                                                                       |
  
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
<th style="border:1px solid black;" >
</th>
</tr>
<tr>
<th colspan="9" style="border:1px solid black;">
Microsoft Windows 2000  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS09-044**](http://go.microsoft.com/fwlink/?linkid=157861)
</td>
<td style="border:1px solid black;">
[**MS09-039**](http://go.microsoft.com/fwlink/?linkid=155974)
</td>
<td style="border:1px solid black;">
[**MS09-038**](http://go.microsoft.com/fwlink/?linkid=155975)
</td>
<td style="border:1px solid black;">
[**MS09-037**](http://go.microsoft.com/fwlink/?linkid=158695)
</td>
<td style="border:1px solid black;">
[**MS09-041**](http://go.microsoft.com/fwlink/?linkid=155977)
</td>
<td style="border:1px solid black;">
[**MS09-040**](http://go.microsoft.com/fwlink/?linkid=155979)
</td>
<td style="border:1px solid black;">
[**MS09-036**](http://go.microsoft.com/fwlink/?linkid=157296)
</td>
<td style="border:1px solid black;">
[**MS09-042**](http://go.microsoft.com/fwlink/?linkid=157140)
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
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Windows 2000 Service Pack 4
</td>
<td style="border:1px solid black;">
[RDP verze 5.0](http://www.microsoft.com/downloads/details.aspx?familyid=027e757d-08d5-4932-b8c4-52ee1be1c864)\*\*\*  
(KB958471) a [RDP verze 5.0](http://www.microsoft.com/downloads/details.aspx?familyid=ae72782e-920f-4176-a27b-c3b91d50c7d2) (KB958470)  
(Kritický)  
[RDP verze 5.1](http://www.microsoft.com/downloads/details.aspx?familyid=ae72782e-920f-4176-a27b-c3b91d50c7d2)\*\*\*\*  
(KB958470)  
(Kritický)  
[RDP verze 5.2](http://www.microsoft.com/downloads/details.aspx?familyid=ae72782e-920f-4176-a27b-c3b91d50c7d2)\*\*\*\*  
(KB958470)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Server Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=b5b9228a-66c0-49e6-afde-cc2825a6851f)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=5f80bf0b-898c-46ca-b20c-21e0e729c332)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Microsoft Outlook Express 5.5 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=6f9fcbe9-8496-4d23-8a16-b334157688c2)  
(KB973354)  
(Kritický)  
[Microsoft Outlook Express 6 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=f340af34-b9a0-44fb-b595-dbb346c727bf)  
(KB973354)  
(Kritický)  
[Windows Media Player 9](http://www.microsoft.com/downloads/details.aspx?familyid=bd7c9fc4-61cb-4c23-9961-6d63f234731c)  
(KB973540)  
(Kritický)  
[Komponenta knihovny Windows ATL](http://www.microsoft.com/downloads/details.aspx?familyid=c773149a-f4fc-486a-b718-6b8ff7a36ae2)  
(KB973507)  
(Kritický)  
[Ovládací prvek ActiveX komponenty pro úpravy formátu DHTML](http://www.microsoft.com/downloads/details.aspx?familyid=223e25d2-83d7-4cb7-85c4-46a42b8110e0)  
(KB973869)  
(Kritický)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=8ed8bad7-2885-452c-9c34-3982cd498be8)  
(Důležitý)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=240977d6-3581-4058-b9f1-7847e4edcf8a)  
(Důležitý)
</td>
</tr>
<tr>
<th colspan="9" style="border:1px solid black;">
Windows XP
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS09-044**](http://go.microsoft.com/fwlink/?linkid=157861)
</td>
<td style="border:1px solid black;">
[**MS09-039**](http://go.microsoft.com/fwlink/?linkid=155974)
</td>
<td style="border:1px solid black;">
[**MS09-038**](http://go.microsoft.com/fwlink/?linkid=155975)
</td>
<td style="border:1px solid black;">
[**MS09-037**](http://go.microsoft.com/fwlink/?linkid=158695)
</td>
<td style="border:1px solid black;">
[**MS09-041**](http://go.microsoft.com/fwlink/?linkid=155977)
</td>
<td style="border:1px solid black;">
[**MS09-040**](http://go.microsoft.com/fwlink/?linkid=155979)
</td>
<td style="border:1px solid black;">
[**MS09-036**](http://go.microsoft.com/fwlink/?linkid=157296)
</td>
<td style="border:1px solid black;">
[**MS09-042**](http://go.microsoft.com/fwlink/?linkid=157140)
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
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Žádné
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
[RDP verze 5.1 v systému Windows XP Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2a8830dd-8fb3-4556-a6e7-2c237235357f)  
(KB958470)  
(Kritický)  
[RDP verze 5.2 pro systém Windows XP Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=cf9f9898-10c8-45ab-9df3-85e0b37e6046)\*\*\*\*  
(KB958469)  
(Kritický)  
[RDP verze 5.2 v systému Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=cf9f9898-10c8-45ab-9df3-85e0b37e6046)  
(KB958469)  
(Kritický)  
[RDP verze 6.0 pro systém Windows XP Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d1f82d76-eeb2-4ff4-9d2c-46882f214719)\*\*\*\*  
(KB956744)  
(Důležitý)  
[RDP verze 6.1](http://www.microsoft.com/downloads/details.aspx?familyid=d1f82d76-eeb2-4ff4-9d2c-46882f214719)\*\*\*\*  
(KB956744)  
(Kritický)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 a Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=2e8a68ee-eb24-424c-b084-450636ccaeec)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Microsoft Outlook Express 6](http://www.microsoft.com/downloads/details.aspx?familyid=c67b5506-00ea-47cc-a0e8-897057b7380c)  
(KB973354)  
(Kritický)  
[Windows Media Player 9, Windows Media Player 10 a Windows Media Player 11](http://www.microsoft.com/downloads/details.aspx?familyid=34b2b14d-5811-4635-ba83-f837dcb03d04)  
(KB973540)  
(Kritický)  
(pouze Windows XP Service Pack 2)  
[Windows Media Player 9, Windows Media Player 10 a Windows Media Player 11](http://www.microsoft.com/downloads/details.aspx?familyid=ec84c98b-6bc7-442f-9280-d6e204280b2f)  
(KB973540)  
(Kritický)  
(pouze Windows XP Service Pack 3)  
[Komponenta knihovny Windows ATL](http://www.microsoft.com/downloads/details.aspx?familyid=4b4c6fc5-e8e6-4d89-a181-e231240468f9)  
(KB973507)  
(Kritický)  
[Ovládací prvek ActiveX komponenty pro úpravy formátu DHTML](http://www.microsoft.com/downloads/details.aspx?familyid=bdfcd0c3-7c18-4e63-91dd-d8f82cd89592)  
(KB973869)  
(Kritický)  
[Ovládací prvek Microsoft MSWebDVD ActiveX](http://www.microsoft.com/downloads/details.aspx?familyid=8b71bcc9-5146-4afc-8847-0af21d7fad36)  
(KB973815)  
(Kritický)  
[Ovládací prvek HtmlInput Object ActiveX](http://www.microsoft.com/downloads/details.aspx?familyid=46aa443c-4e7b-4bd5-8b4e-0068c3dc0e79)  
(KB973768)  
(Kritický)  
(pouze Media Center Edition 2005)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 a Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=9c0e5bff-c248-4e87-a83b-82ba52f5299d)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=93490aa7-9985-4658-b0d7-88fb3f27ada0)  
(Důležitý)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 a Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=b3331388-1e52-4924-b512-23275a8fde84)  
(Důležitý)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[RDP verze 5.2 v systému Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=948da99a-44ed-4390-b1b4-7ed3f15a9cda)  
(KB958469)  
(Kritický)  
[RDP verze 6.0 pro systém Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5061615f-fa8f-465f-ac8f-393998b7e91b)\*\*\*\*  
(KB956744)  
(Kritický)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=a1ff2ace-b9dc-4cf3-a151-ac6959bcb3a6)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Microsoft Outlook Express 6](http://www.microsoft.com/downloads/details.aspx?familyid=ede1a73a-e303-435e-a2c7-0281ce2370da)  
(KB973354)  
(Kritický)  
[Windows Media Player 10](http://www.microsoft.com/downloads/details.aspx?familyid=bb98187a-8db9-47e4-88ac-15544c5268f6)  
(KB973540)  
(Kritický)  
[Windows Media Player 11](http://www.microsoft.com/downloads/details.aspx?familyid=9e8b9027-4407-4c31-a2ba-9e094557d467)  
(KB973540)  
(Kritický)  
[Komponenta knihovny Windows ATL](http://www.microsoft.com/downloads/details.aspx?familyid=2f2b93fc-f977-4f23-af90-c27f744fad0a)  
(KB973507)  
(Kritický)  
[Ovládací prvek ActiveX komponenty pro úpravy formátu DHTML](http://www.microsoft.com/downloads/details.aspx?familyid=d04a6959-41a4-4a87-b3ad-7455d8fe8b99)  
(KB973869)  
(Kritický)  
[Ovládací prvek Microsoft MSWebDVD ActiveX](http://www.microsoft.com/downloads/details.aspx?familyid=85b2dcdb-cea9-4c4a-8ebd-50264e781ade)  
(KB973815)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7b64a454-d383-47e3-b469-b87e2b3c1a9f)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=12e6be68-dc87-450e-927b-3c9b6873eb13)  
(Důležitý)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=a6ee7af3-3e39-4866-a893-92bf1c786cd4)  
(Důležitý)
</td>
</tr>
<tr>
<th colspan="9" style="border:1px solid black;">
Windows Server 2003
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS09-044**](http://go.microsoft.com/fwlink/?linkid=157861)
</td>
<td style="border:1px solid black;">
[**MS09-039**](http://go.microsoft.com/fwlink/?linkid=155974)
</td>
<td style="border:1px solid black;">
[**MS09-038**](http://go.microsoft.com/fwlink/?linkid=155975)
</td>
<td style="border:1px solid black;">
[**MS09-037**](http://go.microsoft.com/fwlink/?linkid=158695)
</td>
<td style="border:1px solid black;">
[**MS09-041**](http://go.microsoft.com/fwlink/?linkid=155977)
</td>
<td style="border:1px solid black;">
[**MS09-040**](http://go.microsoft.com/fwlink/?linkid=155979)
</td>
<td style="border:1px solid black;">
[**MS09-036**](http://go.microsoft.com/fwlink/?linkid=157296)
</td>
<td style="border:1px solid black;">
[**MS09-042**](http://go.microsoft.com/fwlink/?linkid=157140)
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
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[RDP verze 5.2](http://www.microsoft.com/downloads/details.aspx?familyid=60c79729-ef01-4630-bd67-ec63e7f8b56b)  
(KB958469)  
(Kritický)  
[RDP verze 6.0](http://www.microsoft.com/downloads/details.aspx?familyid=a37a2d8a-a5ce-4f06-bf07-8cafa16e7a59)\*\*\*\*  
(KB956744)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3a8d8ef9-ad41-4237-9cbb-daecfd8f216c)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=cba78658-899c-428f-8b04-cfe14ce3c255)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Microsoft Outlook Express 6](http://www.microsoft.com/downloads/details.aspx?familyid=3119ab1e-6729-40a1-b28f-0dab50502be6)  
(KB973354)  
(Kritický)  
[Windows Media Player 10](http://www.microsoft.com/downloads/details.aspx?familyid=ab054890-983b-4414-ad0a-da1b2d2a4895)  
(KB973540)  
(Kritický)  
[Komponenta knihovny Windows ATL](http://www.microsoft.com/downloads/details.aspx?familyid=7d9369b5-0c54-4c17-bc62-fba0a7b4728c)  
(KB973507)  
(Kritický)  
[Ovládací prvek ActiveX komponenty pro úpravy formátu DHTML](http://www.microsoft.com/downloads/details.aspx?familyid=bfc474c2-e3c5-40df-85d4-4ac666ff0561)  
(KB973869)  
(Kritický)  
[Ovládací prvek Microsoft MSWebDVD ActiveX](http://www.microsoft.com/downloads/details.aspx?familyid=301ad191-8d3f-41d3-b41c-e2e863893f73)  
(KB973815)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=9cb0477f-0656-47f5-bd35-5716e0572fbd)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=52f59c56-2aba-4626-a90e-311e0e73c813)  
(Důležitý)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3fe9c745-d87c-43b0-9b2a-356fb34282b4)  
(Důležitý)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[RDP verze 5.2](http://www.microsoft.com/downloads/details.aspx?familyid=57393588-dc96-4bda-ab1e-ae550961e5d4)  
(KB958469)  
(Kritický)  
[RDP verze 6.0](http://www.microsoft.com/downloads/details.aspx?familyid=957c2e01-89a1-4550-aacb-de8ff896d762)\*\*\*\*  
(KB956744)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e132d051-4444-4ef1-9b6f-2d7da9d2e88e)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=58a7c8d9-ec36-46a6-a89b-d8dfd989fda4)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Microsoft Outlook Express 6](http://www.microsoft.com/downloads/details.aspx?familyid=17bd00e3-810c-4a72-bd13-1b55ffb52a5e)  
(KB973354)  
(Kritický)  
[Windows Media Player 10](http://www.microsoft.com/downloads/details.aspx?familyid=5890233a-d8f7-490c-8bf5-3ed4bd1c6991)  
(KB973540)  
(Kritický)  
[Komponenta knihovny Windows ATL](http://www.microsoft.com/downloads/details.aspx?familyid=90e0e014-ed7e-498a-9f61-18bb09a384b3)  
(KB973507)  
(Kritický)  
[Ovládací prvek ActiveX komponenty pro úpravy formátu DHTML](http://www.microsoft.com/downloads/details.aspx?familyid=9f502d79-99a8-45dc-9876-2df27e14ffaa)  
(KB973869)  
(Kritický)  
[Ovládací prvek Microsoft MSWebDVD ActiveX](http://www.microsoft.com/downloads/details.aspx?familyid=2ae71a65-5eee-4dd2-bc79-b7c5a73022bc)  
(KB973815)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=96fbf65f-1db2-432d-92a0-6669d8abaeb0)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2f77ef7b-54f8-4260-b6a6-d62a0f85ef45)  
(Důležitý)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e2a788e7-a9d1-4574-b106-f8ab44c6c4a2)  
(Důležitý)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 SP2 pro systémy s procesorem Itanium
</td>
<td style="border:1px solid black;">
[RDP verze 5.2](http://www.microsoft.com/downloads/details.aspx?familyid=8f88a714-b917-4193-9002-19fa65722028)  
(KB958469)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=96c3f496-7b2f-4dbc-b484-216c9943c2b1)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=187b02bd-73d6-4f72-81d1-d9477d495499)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Microsoft Outlook Express 6](http://www.microsoft.com/downloads/details.aspx?familyid=7978b921-c5b5-461f-a284-b9848f568aa9)  
(KB973354)  
(Kritický)  
[Komponenta knihovny Windows ATL](http://www.microsoft.com/downloads/details.aspx?familyid=ad1791b3-8553-4433-a9f7-8b4f857665be)  
(KB973507)  
(Kritický)  
[Ovládací prvek ActiveX komponenty pro úpravy formátu DHTML](http://www.microsoft.com/downloads/details.aspx?familyid=82c0bb02-70ad-4605-a1f4-4698adf9f4ac)  
(KB973869)  
(Kritický)  
[Ovládací prvek Microsoft MSWebDVD ActiveX](http://www.microsoft.com/downloads/details.aspx?familyid=5b8a8958-c3cd-4b24-85a2-1baacf92d218)  
(KB973815)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=11321f48-8997-4b99-982a-3ba4ad3f5992)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=ad55c653-ee6b-4c92-b7f4-3923bb916546)  
(Důležitý)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=4f625d39-29d4-44f9-b4bd-cd99f1ea422d)  
(Důležitý)
</td>
</tr>
<tr>
<th colspan="9" style="border:1px solid black;">
Windows Vista
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS09-044**](http://go.microsoft.com/fwlink/?linkid=157861)
</td>
<td style="border:1px solid black;">
[**MS09-039**](http://go.microsoft.com/fwlink/?linkid=155974)
</td>
<td style="border:1px solid black;">
[**MS09-038**](http://go.microsoft.com/fwlink/?linkid=155975)
</td>
<td style="border:1px solid black;">
[**MS09-037**](http://go.microsoft.com/fwlink/?linkid=158695)
</td>
<td style="border:1px solid black;">
[**MS09-041**](http://go.microsoft.com/fwlink/?linkid=155977)
</td>
<td style="border:1px solid black;">
[**MS09-040**](http://go.microsoft.com/fwlink/?linkid=155979)
</td>
<td style="border:1px solid black;">
[**MS09-036**](http://go.microsoft.com/fwlink/?linkid=157296)
</td>
<td style="border:1px solid black;">
[**MS09-042**](http://go.microsoft.com/fwlink/?linkid=157140)
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
[**Kritický**](http://go.microsoft.com/fwlink/?linkid=21140)
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
[**Mírný**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista, Windows Vista Service Pack 1 a Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
[RDP verze 6.0 v systému Windows Vista](http://www.microsoft.com/downloads/details.aspx?familyid=cf95a552-f6fd-4e35-815a-d16c015cd3ea)  
(KB956744)  
(Důležitý)  
[RDP verze 6.1 pro systém Windows Vista Service Pack 1 a Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=cf95a552-f6fd-4e35-815a-d16c015cd3ea)  
(KB956744)  
(Kritický)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Vista, Windows Vista Service Pack 1 a Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=81fce7bd-f33c-4586-949d-ac40d415f755)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Media Player 11](http://www.microsoft.com/downloads/details.aspx?familyid=3766aed9-93f5-478e-a5bf-b7ee0b577088)  
(KB973540)  
(Kritický)  
[Komponenta knihovny Windows ATL](http://www.microsoft.com/downloads/details.aspx?familyid=80de158d-157e-4c21-9154-c1dbd6e57cb3)  
(KB973507)  
(Kritický)  
[Ovládací prvek HtmlInput Object ActiveX](http://www.microsoft.com/downloads/details.aspx?familyid=59fefa17-0ad4-4a62-82be-e6a2b7a0aec3)  
(KB973768)  
(Kritický)  
(pouze Media Center Edition 2005)
</td>
<td style="border:1px solid black;">
[Windows Vista, Windows Vista Service Pack 1 a Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=979ac9da-940f-49e7-91a2-b12db3708076)  
(Mírný)
</td>
<td style="border:1px solid black;">
[Windows Vista](http://www.microsoft.com/downloads/details.aspx?familyid=00afd94c-b483-4155-884f-b617acca6e7d)  
(Důležitý)
</td>
<td style="border:1px solid black;">
Pouze Windows Vista: [Microsoft .NET Framework 2.0 Service Pack 1 a Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=d42444bb-5030-4b47-87fa-9df3a8c640ff) (KB972591) a [Microsoft .NET Framework 2.0 Service Pack 2 a Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=310f3aa6-c264-45a2-b24a-3f178b41830e)\*\*\*\*\* (KB972592)  
(Důležitý)  
Pouze Windows Vista Service Pack 1:  
[Microsoft .NET Framework 2.0 Service Pack 1 a Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=cbf40800-f3b3-43da-ace1-d942d3378ccd) (KB972593) a [Microsoft .NET Framework 2.0 Service Pack 2 a Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=87c4a868-b3b5-467d-96a4-633532ab548f)\*\*\*\*\* (KB972594)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Windows Vista, Windows Vista Service Pack 1 a Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d77f406d-11cb-4d19-94ec-938b356c3427)  
(Mírný)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 a Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[RDP verze 6.0 v systému Windows Vista x64 Edition](http://www.microsoft.com/downloads/details.aspx?familyid=5e19cef7-2413-4575-9597-c6273a097aad)  
(KB956744)  
(Důležitý)  
[RDP verze 6.1 v systému Windows Vista x64 Edition Service Pack 1 a Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5e19cef7-2413-4575-9597-c6273a097aad)  
(KB956744)  
(Kritický)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 a Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=a6cea61a-4ad9-4e18-bf18-348ae4ae51c4)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Media Player 11](http://www.microsoft.com/downloads/details.aspx?familyid=64edbd64-9faa-4f54-b0d5-836c683ca7cd)  
(KB973540)  
(Kritický)  
[Komponenta knihovny Windows ATL](http://www.microsoft.com/downloads/details.aspx?familyid=82940d30-6a30-47ca-b184-2ac96e35c294)  
(KB973507)  
(Kritický)  
[Ovládací prvek HtmlInput Object ActiveX](http://www.microsoft.com/downloads/details.aspx?familyid=92de8a2e-2d50-4278-937e-ccb862c5ab8f)  
(KB973768)  
(Kritický)  
(pouze Media Center Edition 2005)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 a Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b9aa04cc-a5c5-47ae-bf0f-250cff275d26)  
(Mírný)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition](http://www.microsoft.com/downloads/details.aspx?familyid=a0c698aa-a913-4981-8798-6bbb8cacfb86)  
(Důležitý)
</td>
<td style="border:1px solid black;">
Pouze Windows Vista x64 Edition: [Microsoft .NET Framework 2.0 Service Pack 1 a Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=d42444bb-5030-4b47-87fa-9df3a8c640ff) (KB972591) a [Microsoft .NET Framework 2.0 Service Pack 2 a Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=310f3aa6-c264-45a2-b24a-3f178b41830e)\*\*\*\*\* (KB972592)  
(Důležitý)  
Pouze Windows Vista x64 Edition Service Pack 1:  
[Microsoft .NET Framework 2.0 Service Pack 1 a Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=cbf40800-f3b3-43da-ace1-d942d3378ccd) (KB972593) a [Microsoft .NET Framework 2.0 Service Pack 2 a Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=87c4a868-b3b5-467d-96a4-633532ab548f) (KB972594)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 a Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7a41b8c1-f955-474e-a08e-5e73964327d1)  
(Mírný)
</td>
</tr>
<tr>
<th colspan="9" style="border:1px solid black;">
Windows Server 2008
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS09-044**](http://go.microsoft.com/fwlink/?linkid=157861)
</td>
<td style="border:1px solid black;">
[**MS09-039**](http://go.microsoft.com/fwlink/?linkid=155974)
</td>
<td style="border:1px solid black;">
[**MS09-038**](http://go.microsoft.com/fwlink/?linkid=155975)
</td>
<td style="border:1px solid black;">
[**MS09-037**](http://go.microsoft.com/fwlink/?linkid=158695)
</td>
<td style="border:1px solid black;">
[**MS09-041**](http://go.microsoft.com/fwlink/?linkid=155977)
</td>
<td style="border:1px solid black;">
[**MS09-040**](http://go.microsoft.com/fwlink/?linkid=155979)
</td>
<td style="border:1px solid black;">
[**MS09-036**](http://go.microsoft.com/fwlink/?linkid=157296)
</td>
<td style="border:1px solid black;">
[**MS09-042**](http://go.microsoft.com/fwlink/?linkid=157140)
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
[**Kritický**](http://go.microsoft.com/fwlink/?linkid=21140)
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
[**Mírný**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 pro 32bitové systémy a Windows Server 2008 pro 32bitové systémy Service Pack 2
</td>
<td style="border:1px solid black;">
[RDP verze 6.1](http://www.microsoft.com/downloads/details.aspx?familyid=71c17a87-710b-434d-9b2a-2f471674915a)\*\*  
(KB956744)  
(Kritický)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro 32bitové systémy a Windows Server 2008 pro 32bitové systémy Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=fdc96a07-ed79-4798-8077-b2e9ca64cd0f)\*\*  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Media Player 11](http://www.microsoft.com/downloads/details.aspx?familyid=85d9e69f-99a2-467f-bf37-4b47466a12d4)\*\*  
(KB973540)  
(Kritický)  
[Komponenta knihovny Windows ATL](http://www.microsoft.com/downloads/details.aspx?familyid=ba423491-6c29-49f2-811b-ac3f9bbc58fc)\*  
(KB973507)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro 32bitové systémy a Windows Server 2008 pro 32bitové systémy Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=24c77c27-0b7d-4a35-a871-b453f90e5913)\*  
(Mírný)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Pouze systém Windows Server 2008 pro 32bitové systémy [Microsoft .NET Framework 2.0 Service Pack 1 a Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=cbf40800-f3b3-43da-ace1-d942d3378ccd) (KB972593) a [Microsoft .NET Framework 2.0 Service Pack 2 a Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=87c4a868-b3b5-467d-96a4-633532ab548f) (KB972594)\*\*  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro 32bitové systémy a Windows Server 2008 pro 32bitové systémy Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=62f2e0a6-5e68-41c7-a851-d99bcff6ff3e)\*  
(Mírný)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 pro systémy s procesorem x64 a Windows Server 2008 pro systémy s procesorem x64 Service Pack 2
</td>
<td style="border:1px solid black;">
[RDP verze 6.1](http://www.microsoft.com/downloads/details.aspx?familyid=f095d2d5-4513-4ae1-96c7-cbcf83304261)\*\*  
(KB956744)  
(Kritický)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem x64 a Windows Server 2008 pro systémy s procesorem x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8e3afba4-6761-4b3d-98bb-4b4145e27b7f)\*\*  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Media Player 11](http://www.microsoft.com/downloads/details.aspx?familyid=9501c8c2-a526-4661-8cba-7847bace1aa0)\*\*  
(KB973540)  
(Kritický)  
[Komponenta knihovny Windows ATL](http://www.microsoft.com/downloads/details.aspx?familyid=b9311953-889a-415f-a396-250a005e95cd)\*  
(KB973507)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem x64 a Windows Server 2008 pro systémy s procesorem x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=48d0432e-704a-4bbb-b0a1-cd14069a8e93)\*  
(Mírný)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Pouze systém Windows Server 2008 pro systémy s procesorem x64: [Microsoft .NET Framework 2.0 Service Pack 1 a Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=cbf40800-f3b3-43da-ace1-d942d3378ccd) (KB972593) a [Microsoft .NET Framework 2.0 Service Pack 2 a Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=87c4a868-b3b5-467d-96a4-633532ab548f) (KB972594)\*\*  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem x64 a Windows Server 2008 pro systémy s procesorem x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=6e5d1db9-efef-4112-8138-62f14670cf0d)\*  
(Mírný)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 pro systémy s procesorem Itanium a Windows Server 2008 pro systémy s procesorem Itanium Service Pack 2
</td>
<td style="border:1px solid black;">
[RDP verze 6.1](http://www.microsoft.com/downloads/details.aspx?familyid=65d0af4e-22a2-4524-a003-2f4858012fa8)  
(KB956744)  
(Kritický)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem Itanium a Windows Server 2008 pro systémy s procesorem Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=aa1bb13a-5905-48c4-8e74-a41104593046)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Komponenta knihovny Windows ATL](http://www.microsoft.com/downloads/details.aspx?familyid=e5612bb4-5f37-4b38-bd2e-f198c413371c)  
(KB973507)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem Itanium a Windows Server 2008 pro systémy s procesorem Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c119223c-f4e0-449b-8e7b-a6bf11c98f94)  
(Mírný)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Pouze systém Windows Server 2008 pro systémy s procesorem Itanium: [Microsoft .NET Framework 2.0 Service Pack 1 a Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=cbf40800-f3b3-43da-ace1-d942d3378ccd) (KB972593) a [Microsoft .NET Framework 2.0 Service Pack 2 a Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=87c4a868-b3b5-467d-96a4-633532ab548f) (KB972594)  
(Důležitý
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem Itanium a Windows Server 2008 pro systémy s procesorem Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4b813c74-b2ae-4962-9ebb-1311193d9e2d)  
(Mírný)
</td>
</tr>
</table>
<p></p>
 
**Poznámky k systému Windows Server 2008**

**\*Instalace server core operačního systému Windows Server 2008 obsahující tuto chybu.** Tato aktualizace se týká všech podporovaných vydání systému Windows Server 2008 se stejným stupněm závažnosti, ať už byl systém Windows Server 2008 instalován pomocí možnosti instalace Server Core či nikoli. Více informací o této možnosti instalace naleznete v části [Server Core](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx). Možnost instalace Server Core se nevztahuje na určité edice systému Windows Server 2008. Další informace naleznete v části [Porovnání možností instalace Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**\*\*Instalace Server Core operačního systému Windows Server 2008 neobsahující tuto chybu.** Chyby zabezpečení, které tato aktualizace řeší, nemají vliv na podporované edice systému Windows Server 2008, jestliže byl systém Windows Server 2008 instalován s využitím možnosti instalace Server Core. Více informací o této možnosti instalace naleznete v části [Server Core](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx). Možnost instalace Server Core se nevztahuje na určité edice systému Windows Server 2008. Další informace naleznete v části [Porovnání možností instalace Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**Poznámky k bulletinu MS09-044**

\*\*\*Uživatelé protokolu RDP verze 5.0 v systému Microsoft Windows 2000 Service Pack 4 musí nainstalovat jak aktualizaci KB958471, tak aktualizaci KB958470.

\*\*\*\*Je možné, že správci tento software již nainstalovali ručně.

Viz také podčást Klientský software pro systém Mac v části **Software obsahující tuto chybu a umístění aktualizací ke stažení**, kde získáte více aktualizovaných souborů v rámci stejného identifikátoru bulletinu. Tento bulletin se vztahuje na více kategorií softwaru.

**Poznámka k bulletinu MS09-036**

\*\*\*\*Vzhledem k tomu, že služba IIS 7.0 nefunguje v edicích Windows Vista Starter a Windows Vista Home Basic, nejsou následující edice chybou postiženy: Windows Vista Starter (32bitový), Windows Vista Home Basic (32bitový) a Windows Vista Home Basic (64bitový).

#### Klientský software pro systém Mac

 
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
Vzdálená plocha
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS09-044**](http://go.microsoft.com/fwlink/?linkid=157861)
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
Klient Připojení ke vzdálené ploše pro systém Mac
</td>
<td style="border:1px solid black;">
[Klient Připojení ke vzdálené ploše pro systém Mac 2.0](http://www.microsoft.com/downloads/details.aspx?familyid=cd9ec77e-5b07-4332-849f-046611458871)\* 
(Důležitý)
</td>
</tr>
</table>
<p></p>
 
**Poznámky k bulletinu MS09-044**

\*Tato položka ke stažení řeší chybu zabezpečení upgradem klienta Připojení ke vzdálené ploše pro systém Mac 2.0 na klienta Připojení ke vzdálené ploše pro systém Mac 2.0.1.

Další soubory aktualizace v rámci stejného identifikátoru bulletinu naleznete také v podčásti Operační systém Windows a jeho součásti v části **Software obsahující tuto chybu a umístění aktualizací ke stažení**. Tento bulletin se vztahuje na více kategorií softwaru.

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
Sady Microsoft Office, systémy a komponenty
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS09-043**](http://go.microsoft.com/fwlink/?linkid=128110)
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
Microsoft Office XP
</td>
<td style="border:1px solid black;">
[Microsoft Office XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=60e2e4e7-aa75-441d-b6fc-7e850bf8e580)  
(KB947320)  
(Kritický)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2003
</td>
<td style="border:1px solid black;">
[Microsoft Office 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=95c94c9a-6aca-42fb-9679-3234f06c72f7)  
(KB947319)  
(Kritický)
</td>
</tr>
<tr>
<th colspan="2" style="border:1px solid black;">
Součásti Office Web Components
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS09-043**](http://go.microsoft.com/fwlink/?linkid=128110)
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
Microsoft Office 2000 Web Components
</td>
<td style="border:1px solid black;">
[Microsoft Office 2000 Web Components Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=60e2e4e7-aa75-441d-b6fc-7e850bf8e580)  
(KB947320)  
(Kritický)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office XP Web Components
</td>
<td style="border:1px solid black;">
[Microsoft Office XP Web Components Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=60e2e4e7-aa75-441d-b6fc-7e850bf8e580)  
(KB947320)  
(Kritický)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2003 Web Components
</td>
<td style="border:1px solid black;">
[Microsoft Office 2003 Web Components Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=95c94c9a-6aca-42fb-9679-3234f06c72f7)  
(KB947319)  
(Kritický)  
[Microsoft Office 2003 Web Components Service Pack 1 pro systém Microsoft Office 2007](http://www.microsoft.com/downloads/details.aspx?familyid=644008e0-77c9-4a02-ac9b-e30d0930c4be)\*  
(KB947318)  
(Kritický)
</td>
</tr>
<tr>
<th colspan="2" style="border:1px solid black;">
Jiný software sady Office
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS09-043**](http://go.microsoft.com/fwlink/?linkid=128110)
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
Microsoft Office Small Business Accounting 2006
</td>
<td style="border:1px solid black;">
[Microsoft Office Small Business Accounting 2006](http://www.microsoft.com/downloads/details.aspx?familyid=0d77ddb3-4d34-4cfe-913b-d05981f59a82)  
(KB968377)  
(Kritický)
</td>
</tr>
</table>
<p></p>
 
**Poznámky k bulletinu MS09-043**

\*SQL Server 2008 a Microsoft Forefront Threat Management Gateway Medium Business Edition redistribuují postiženou součást, Office 2003 Web Components, do systému Microsoft Office 2007. Aktualizace součástí Office 2003 Web Components pro systém Microsoft Office 2007 rozpozná server SQL Server 2008 a bránu Microsoft Forefront Threat Management Gateway Medium Business Edition a uživatelům nabídne aktualizaci.

Viz také další podčásti v části **Software obsahující tuto chybu a umístění aktualizací ke stažení**, kde získáte více aktualizovaných souborů v rámci stejného identifikátoru bulletinu. Tento bulletin se vztahuje na více kategorií softwaru.

#### Vývojářské nástroje a software společnosti Microsoft

 
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
Microsoft Visual Studio
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS09-043**](http://go.microsoft.com/fwlink/?linkid=128110)
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
Microsoft Visual Studio .NET 2003
</td>
<td style="border:1px solid black;">
[Microsoft Visual Studio .NET 2003 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=ba2915a0-f5f4-4e18-b0c0-534d2a948585)  
(KB969172)  
(Kritický)
</td>
</tr>
</table>
<p></p>
 
**Poznámka k bulletinu MS09-043**

Viz také další podčásti v části **Software obsahující tuto chybu a umístění aktualizací ke stažení**, kde získáte více aktualizovaných souborů v rámci stejného identifikátoru bulletinu. Tento bulletin se vztahuje na více kategorií softwaru.

#### Microsoft Server and Security Software

 
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
Microsoft Internet Security and Acceleration Server
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS09-043**](http://go.microsoft.com/fwlink/?linkid=128110)
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
Microsoft ISA (Internet Security and Acceleration) Server 2004
</td>
<td style="border:1px solid black;">
[Microsoft Internet Security and Acceleration Server 2004 Standard Edition Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=8f79a073-27e8-46ef-87d8-f09b93521326)\*  
(KB947826)  
(Kritický)  
[Microsoft Internet Security and Acceleration Server 2004 Enterprise Edition Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=8f79a073-27e8-46ef-87d8-f09b93521326)  
(KB947826)  
(Kritický)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Internet Security and Acceleration Server 2006
</td>
<td style="border:1px solid black;">
[Microsoft Internet Security and Acceleration Server 2006 Standard Edition Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=8f79a073-27e8-46ef-87d8-f09b93521326)  
(KB947826)  
(Kritický)  
[Microsoft Internet Security and Acceleration Server 2006 Enterprise Edition Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=8f79a073-27e8-46ef-87d8-f09b93521326)  
(KB947826)  
(Kritický)
</td>
</tr>
<tr>
<th colspan="2" style="border:1px solid black;">
Microsoft BizTalk Server
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS09-043**](http://go.microsoft.com/fwlink/?linkid=128110)
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
Microsoft BizTalk Server 2002
</td>
<td style="border:1px solid black;">
[Microsoft BizTalk Server 2002](http://www.microsoft.com/downloads/details.aspx?familyid=495839b6-0322-4755-997d-4a7762c53333)  
(KB971388)  
(Kritický)
</td>
</tr>
</table>
<p></p>
 
**Poznámky k bulletinu MS09-043**

\*Microsoft ISA Server 2004 Standard Edition je k dispozici jako samostatný produkt. Microsoft ISA Server 2004 Standard Edition je také k dispozici jako součást serveru Windows Small Business Server 2003 Premium Edition Service Pack 1 a serveru Windows Small Business Server 2003 R2 Premium Edition.

Viz také další podčásti v části **Software obsahující tuto chybu a umístění aktualizací ke stažení**, kde získáte více aktualizovaných souborů v rámci stejného identifikátoru bulletinu. Tento bulletin se vztahuje na více kategorií softwaru.

Nástroje a doporučené postupy zjišťování a nasazení
---------------------------------------------------

 
**Centrum zabezpečení**

Umožňuje správu aktualizací softwaru a zabezpečení, které je třeba nainstalovat na servery, stolní počítače a přenosné počítače v organizaci. Další informace naleznete na webu [TechNet Update Management Center](http://go.microsoft.com/fwlink/?linkid=69903). Další informace o zabezpečení produktů společnosti Microsoft nabízí web [Centrum zabezpečení TechNet](http://go.microsoft.com/fwlink/?linkid=21171). Tyto informace lze také získat kliknutím na nabídku „Nejnovější aktualizace zabezpečení“ na webu [Zabezpečení doma](http://go.microsoft.com/fwlink/?linkid=85102).

Aktualizace zabezpečení jsou k dispozici na webu [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747) a [Windows Update](http://go.microsoft.com/fwlink/?linkid=21130). Aktualizace zabezpečení jsou také k dispozici na webu [služby Stažení softwaru](http://go.microsoft.com/fwlink/?linkid=21129). Nejsnadněji je naleznete hledáním podle klíčových slov aktualizace zabezpečení.

Aktualizace zabezpečení lze stáhnout z katalogu služby [Microsoft Update Catalog](http://go.microsoft.com/fwlink/?linkid=96155). Služba Microsoft Update Catalog poskytuje katalog s možností vyhledávání obsahu dostupného prostřednictvím služeb Windows Update a Microsoft Update, včetně aktualizací zabezpečení, ovladačů a aktualizací Service Pack. Vyhledáváním pomocí čísla bulletinu zabezpečení (například MS07-036) můžete přidat všechny dostupné aktualizace do košíku (včetně různých jazykových verzí aktualizace) a stáhnout je do vybrané složky. Další informace o službě Microsoft Update Catalog najdete v části [Nejčastější dotazy týkající se služby Microsoft Update Catalog](http://go.microsoft.com/fwlink/?linkid=97900).

**Poznámka:** K 1. srpnu 2009 ukončí společnost Microsoft podporu webu Office Update a nástroje Office Update Inventory Tool. Nejnovější aktualizace produktů Microsoft Office bude přinášet web [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747). Další informace naleznete v části [O webu Microsoft Office Update: Nejčastější dotazy](http://office.microsoft.com/en-us/downloads/fx010402221033.aspx).

**Doporučené postupy zjišťování a nasazení**

Společnost Microsoft poskytuje doporučené postupy zjišťování a nasazení aktualizací zabezpečení. Tyto dokumenty obsahují doporučení a informace, které mohou odborníkům v oblasti IT pomoci porozumět, jak se používají různé nástroje pro detekci a nasazení aktualizací zabezpečení. Další informace získáte v [článku 961747 znalostní báze Microsoft Knowledge Base](http://support.microsoft.com/kb/961747/cs).

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

-   Alexanderu Pfandtovi ze společnosti [Digitiria](http://www.digitaria.com/) za oznámení chyby popsané v bulletinu MS09-036.
-   Ryanu Smithovi a Alexu Wheelerovi ze společnosti [IBM ISS X-Force](http://www.iss.net/) za brzké oznámení chyby popsané v bulletinu MS09-037.
-   Robertu Freemanovi ze společnosti [IBM ISS X-Force](http://www.iss.net/) za oznámení chyby popsané v bulletinu MS09-037.
-   Davidu Deweymu ze společnosti [IBM ISS X-Force](http://www.iss.net/) za oznámení chyby popsané v bulletinu MS09-037.
-   Ryanu Smithovi ze společnosti [VeriSign iDefense Labs](http://labs.idefense.com/) za oznámení dvou chyb popsaných v bulletinu MS09-037.
-   Vinayi Anantharamanovi ze společnosti [Adobe Systems, Inc.](http://www.adobe.com/) za oznámení dvou chyb popsaných v bulletinu MS09-038.
-   Společnosti [TippingPoint](http://www.tippingpoint.com/) a organizaci [Zero Day Initiative](http://www.zerodayinitiative.com/) za oznámení chyby popsané v bulletinu MS09-039.
-   LiGen z univerzity [National University of Defense Technology](http://english.nudt.edu.cn/) za oznámení chyby popsané v bulletinu MS09-039.
-   Nikitu Tarakanovovi z týmu [Positive Technologies Research Team](http://en.securitylab.ru/lab/) za oznámení chyby popsané v bulletinu MS09-040.
-   Codymu Piercovi ze společnosti [TippingPoint DVLabs](http://dvlabs.tippingpoint.com/) za oznámení chyby popsané v bulletinu MS08-041.
-   Peteru Vreugdenhilovi z organizace [Zero Day Initiative](http://www.zerodayinitiative.com/) za oznámení dvou chyb popsaných v bulletinu MS09-043.
-   Peteru Vreugdenhilovi z organizace [Zero Day Initiative](http://www.zerodayinitiative.com/) a Haifei Liovi z týmu [FortiGuard Global Security Research Team](http://www.fortiguardcenter.com/) společnosti Fortinet za oznámení chyby popsané v bulletinu MS09-043.
-   Seanu Larssonovi ze společnosti [VeriSign iDefense Labs](http://labs.idefense.com/) za oznámení chyby popsané v bulletinu MS09-043.
-   Uživateli wushi ze skupiny [Team509](http://www.team509.com/), spolupracujícímu s organizací Zero Day Initiative, za oznámení chyby popsané v bulletinu MS09-044.
-   Yamatu Liovi ze společnosti [Palo Alto Networks](http://www.paloaltonetworks.com/) za oznámení chyby popsané v bulletinu MS09-044.

#### Technická podpora

-   Uvedený software byl testován za účelem zjištění, kterých verzí se chyba týká. U dalších verzí skončila časově omezená podpora. Pokud chcete zjistit dobu, po kterou je pro určitou verzi softwaru poskytována podpora, navštivte web [Zásady poskytování technické podpory pro produkty společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=21742).
-   Zákazníci mohou získat technickou podporu na webu [služby technické podpory společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=21131). Hovory související s aktualizacemi zabezpečení jsou bezplatné. Další informace o dostupných možnostech technické podpory naleznete na webu [Pomoc a podpora společnosti Microsoft](http://support.microsoft.com/?ln=cs).
-   Mezinárodní zákazníci získají podporu u místních zastoupení společnosti Microsoft. Technická podpora související s aktualizacemi zabezpečení je bezplatná. Další informace o možnostech kontaktování společnosti Microsoft v případě potřeby technické podpory získáte na [webu mezinárodní technické podpory](http://go.microsoft.com/fwlink/?linkid=21155).

#### Zřeknutí se záruky

Informace ve znalostní bázi Microsoft Knowledge Base jsou poskytovány tak, jak jsou, bez jakékoli záruky. Společnost Microsoft neposkytuje žádné záruky, výslovně uvedené či mlčky předpokládané, včetně záruk obchodovatelnosti a vhodnosti pro určitý účel. Společnost Microsoft ani její dodavatelé nenesou v žádném případě zodpovědnost za žádné škody, včetně přímých, nepřímých, náhodných či následných škod, ztráty zisku či zvláštních škod, a to ani v případě, že byli na možnost takových škod upozorněni. V některých zemích a právních řádech není dovoleno vyloučit nebo omezit odpovědnost, proto se výše uvedené omezení na vás nemusí vztahovat.

#### Revize

-   V1.0 (11. srpna 2009): Souhrnný bulletin byl publikován.
-   V1.1 (13. srpna 2009): Byl opraven seznam aktualizací protokolu RDP pro systémy Windows XP Service Pack 2 a Windows XP Service Pack 3 uvedených v bulletinu zabezpečení MS09-044 tak, aby odpovídal obsahu bulletinu. U bulletinů MS09-037, MS09-042 a MS09-044 došlo ke změně požadavků na restartování.
-   V2.0 (25. srpna 2009): V bulletinu MS09-044 byl opraven referenční odkaz ke stažení pro RDP verze 5.2 pro systém Windows XP Service Pack 2 (KB958469). Byla také opravena poznámka předepisující chybnou instalační sekvenci pro aktualizace KB958471 a KB958470. Zákazníci, kteří tyto aktualizace úspěšně nainstalovali, je nemusí instalovat znovu.
-   V3.0 (8. září 2009): Společnost Microsoft znovu vydala bulletin MS09-037, ve kterém nabízí nové aktualizace pro ovládací prvek HtmlInput Object ActiveX v systému Windows XP Media Center Edition 2005 a ve všech podporovaných edicích systému Windows Vista.
-   V4.0 (27. října 2009): Společnost Microsoft znovu vydala bulletin MS09-043, ve kterém znovu nabízí aktualizaci pro systém Microsoft Office 2003 Service Pack 3 a Microsoft Office 2003 Web Components Service Pack 3, sloužící k opravě chyby detekce. Jedná se pouze o změnu detekce, v binárních souborech nedošlo ke změně. Zákazníci, kteří systém úspěšně aktualizovali, nemusí tuto aktualizaci znovu instalovat.

*Built at 2014-04-18T01:50:00Z-07:00*
