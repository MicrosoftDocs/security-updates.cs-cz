---
TOCTitle: 'MS10-SEP'
Title: 'Souhrnný bulletin zabezpečení společnosti Microsoft, září 2010'
ms:assetid: 'ms10-sep'
ms:contentKeyID: 61224005
ms:mtpsurl: 'https://technet.microsoft.com/cs-CZ/library/ms10-sep(v=Security.10)'
---

 

Souhrnný bulletin zabezpečení společnosti Microsoft, září 2010
==============================================================

Publikováno: 14. září 2010 | Aktualizováno: 26. října 2011

**Verze:** 6.1

Tento souhrnný bulletin uvádí bulletiny zabezpečení vydané v září 2010.

Spolu s vydáním bulletinů pro září 2010 nahrazuje tento souhrnný bulletin předběžné oznámení o bulletinech vydané 9. září 2010. Další informace o službě předběžného oznámení o bulletinech naleznete v části [Předběžné oznámení o bulletinech zabezpečení společnosti Microsoft](http://technet.microsoft.com/security/bulletin/advance).

Informace o tom, jak dostávat automatická oznámení o vydání nových bulletinů zabezpečení společnosti Microsoft, naleznete na webu [Zasílání technických oznámení o zabezpečení společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=21163).

Pro zodpovězení zákaznických dotazů týkajících se těchto bulletinů uspořádá společnost Microsoft webové vysílání 15. září 2010 v 11:00 časového pásma Tichomoří (USA a Kanada). [Zaregistrujte se pro webové vysílání týkající se zářijových bulletinů zabezpečení](https://msevents.microsoft.com/cui/webcasteventdetails.aspx?eventid=1032454433&eventcategory=4&culture=en-us&countrycode=us). Po tomto datu je webové vysílání dostupné na požádání. Další informace získáte v [souhrnných bulletinech zabezpečení společnosti Microsoft a webovém vysílání](http://technet.microsoft.com/security/bulletin/summary).

Jako součást mimořádného bulletinu zabezpečení MS10-070 přidaného k verzi 3.0 tohoto souhrnného bulletinu uspořádá společnost Microsoft webové vysílání pro zodpovězení zákaznických dotazů týkajících se tohoto bulletinu 28. září 2010 ve 13:00 hodin časového pásma Tichomoří (USA a Kanada). [Zaregistrujte se pro webové vysílání, které se uskuteční 28. září ve 13 hodin](https://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032464130&culture=en-us). Po tomto datu je webové vysílání dostupné na požádání. Další informace získáte v souhrnných bulletinech zabezpečení společnosti Microsoft a webovém vysílání.

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
<th style="border:1px solid black;" >Postižený software</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=200505">MS10-061</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení zařazovací služby tisku by mohla povolit vzdálené spuštění kódu (2347290)</strong><br />
<br />
Tato aktualizace zabezpečení řeší veřejně známou chybu zabezpečení zařazovací služby tisku. Tato chyba zabezpečení může umožnit vzdálené spuštění kódu, pokud útočník odešle do postiženého systému s rozhraním zařazování tisku vystaveným prostřednictvím funkce RPC speciálně vytvořený tiskový požadavek. Tiskárny nejsou sdíleny ve výchozím nastavení žádného aktuálně podporovaného operačního systému Windows.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritický</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=190884">MS10-062</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení kodeku MPEG-4 umožňuje vzdálené spuštění kódu (975558)</strong><br />
<br />
Tato aktualizace zabezpečení řeší chybu zabezpečení v kodeku MPEG-4, kterou oznámila soukromá osoba. Tato chyba zabezpečení může umožnit vzdálené spuštění kódu, pokud uživatel otevře speciálně vytvořený mediální soubor nebo obdrží speciálně vytvořený obsah vysílání datového proudu médií z webové stránky nebo jakékoli aplikace poskytující webový obsah. Útočník, který by úspěšně zneužil tuto chybu zabezpečení, by mohl získat stejná uživatelská práva, jako má místní uživatel. Uživatelé, jejichž účty jsou konfigurovány tak, aby měli v systému méně uživatelských práv, by byli vystaveni menšímu riziku než uživatelé s uživatelskými právy správce.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritický</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Může vyžadovat restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=200378">MS10-063</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení procesoru Unicode Scripts umožňuje vzdálené spuštění kódu (2320113)</strong><br />
<br />
Tato aktualizace zabezpečení řeší chybu zabezpečení procesoru Unicode Scripts oznámenou soukromou osobou. Chyba zabezpečení může umožnit vzdálené spuštění kódu, pokud uživatel zobrazil speciálně vytvořený dokument nebo webovou stránku s aplikací, která podporuje integrovaná písma OpenType. Útočník, který by úspěšně zneužil tuto chybu zabezpečení, by mohl získat stejná uživatelská práva, jako má místní uživatel. Uživatelé, jejichž účty jsou konfigurovány tak, aby měli v systému méně uživatelských práv, by byli vystaveni menšímu riziku než uživatelé s uživatelskými právy správce.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritický</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Může vyžadovat restartování</td>
<td style="border:1px solid black;">Microsoft Windows, Microsoft Office</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=200727">MS10-064</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení v aplikaci Microsoft Outlook umožňuje vzdálené spuštění kódu (2315011)</strong><br />
<br />
Tato aktualizace zabezpečení řeší chybu zabezpečení oznámenou soukromou osobou. Chyba zabezpečení může umožnit vzdálené spuštění kódu, pokud uživatel otevřel nebo zobrazil speciálně vytvořenou e-mailovou zprávu pomocí verze aplikace Microsoft Outlook připojené k serveru Exchange v režimu online. Útočník, který by úspěšně zneužil tuto chybu zabezpečení, by mohl získat stejná uživatelská práva, jako má místní uživatel. Uživatelé, jejichž účty jsou konfigurovány tak, aby měli v systému méně uživatelských práv, by byli vystaveni menšímu riziku než uživatelé s uživatelskými právy správce.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritický</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Může vyžadovat restartování</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=199537">MS10-065</a></td>
<td style="border:1px solid black;"><strong>Chyby zabezpečení</strong> <strong>Internetové informační služby (IIS) umožňují vzdálené spuštění kódu (2267960)</strong><br />
<br />
Tato aktualizace zabezpečení řeší dvě chyby zabezpečení oznámené soukromými osobami a jednu veřejně známou chybu zabezpečení Internetové informační služby (IIS). Nejzávažnější z těchto chyb zabezpečení umožňují vzdálené spuštění kódu, pokud klient odešle na server speciálně vytvořený požadavek HTTP. Útočník, který by tuto chybu zabezpečení zneužil, by mohl získat úplnou kontrolu nad postiženým systémem.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Vysoký</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Může vyžadovat restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=197105">MS10-066</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení služby Vzdáleného volání procedur (RPC) umožňuje</strong> <strong>vzdálené spuštění kódu (982802)</strong><br />
<br />
Tato aktualizace zabezpečení řeší chybu zabezpečení v systému Microsoft Windows, kterou oznámila soukromá osoba. Tato aktualizace zabezpečení je označena jako důležitá pro všechny podporované verze systému Windows XP a Windows Server 2003. Všechny podporované edice systémů Windows Vista, Windows Server 2008, Windows 7 a Windows Server 2008 R2 nejsou postiženy zmíněnou chybou zabezpečení.<br />
<br />
Chyba zabezpečení umožňuje vzdálené spuštění kódu, pokud útočník odeslal speciálně vytvořenou odpověď RPC na požadavek RPC vyvolaný klientem. Útočník, který by tuto chybu zabezpečení úspěšně zneužil, by mohl spustit libovolný kód a získat úplnou kontrolu nad postiženým systémem. Útočník musí přesvědčit uživatele, aby navázal spojení RPC s útočníkem řízeným škodlivým serverem. Tuto chybu zabezpečení nemůže útočník vzdáleně zneužít bez spolupráce uživatele.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Vysoký</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=197102">MS10-067</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení textových převaděčů WordPad umožňuje vzdálené spuštění kódu (2259922)</strong><br />
<br />
Tato aktualizace zabezpečení řeší chybu zabezpečení v systému Microsoft Windows, kterou oznámila soukromá osoba. Tato aktualizace zabezpečení je označena jako důležitá pro všechny podporované verze systému Windows XP a Windows Server 2003. Všechny podporované edice systémů Windows Vista, Windows Server 2008, Windows 7 a Windows Server 2008 R2 nejsou postiženy zmíněnou chybou zabezpečení.<br />
<br />
Tato chyba zabezpečení umožňuje vzdálené spuštění kódu, pokud uživatel otevře speciálně vytvořený soubor pomocí programu WordPad. Útočník, který by úspěšně zneužil tuto chybu zabezpečení, by mohl získat stejná uživatelská práva, jako má místní uživatel. Uživatelé, jejichž účty jsou konfigurovány tak, aby měli v systému méně uživatelských práv, by byli vystaveni menšímu riziku než uživatelé s uživatelskými právy správce.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Vysoký</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Může vyžadovat restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=190509">MS10-068</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení ve službě LSASS (Local Security Authority Subsystem Service) může způsobit zvýšení úrovně oprávnění (983539)</strong><br />
<br />
Tato aktualizace zabezpečení řeší soukromou osobou oznámenou chybu zabezpečení ve službách Active Directory, ADAM (Active Directory Application Mode) a AD LDS (Active Directory Lightweight Directory Service). Tato chyba zabezpečení umožňuje zvýšit úroveň oprávnění, pokud ověřený útočník odešle speciálně vytvořené zprávy protokolu LDAP naslouchajícímu serveru LSASS. Aby mohl útočník tuto chybu zabezpečení zneužít, musí mít členský účet v cílové doméně systému Windows. Útočník však nemusí mít pracovní stanici připojenou k doméně systému Windows.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Vysoký</a><br />
Zvýšení úrovně oprávnění</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=197093">MS10-069</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení v podsystému Windows Client/Server Runtime Subsystem umožňuje zvýšení úrovně oprávnění (2121546)</strong><br />
<br />
Tato aktualizace zabezpečení řeší chybu zabezpečení v systému Microsoft Windows, kterou oznámila soukromá osoba. Tato aktualizace zabezpečení je označena jako důležitá pro všechny podporované verze systému Windows XP a Windows Server 2003. Všechny podporované edice systémů Windows Vista, Windows Server 2008, Windows 7 a Windows Server 2008 R2 nejsou postiženy zmíněnou chybou zabezpečení.<br />
<br />
Chyba zabezpečení může umožnit zvýšení úrovně oprávnění, pokud by se útočník přihlásil k postiženému systému s nastaveným národním prostředím na čínštinu, japonštinu nebo korejštinu. Útočník, který by úspěšně zneužil tuto chybu zabezpečení, by tak mohl následně instalovat programy, zobrazovat, měnit či odstraňovat data nebo vytvářet nové účty s úplnými uživatelskými právy.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Vysoký</a><br />
Zvýšení úrovně oprávnění</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=202409">MS10-070</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení technologie ASP.NET může umožnit přístup k informacím (2418042)</strong><br />
<br />
Tato aktualizace zabezpečení řeší veřejně oznámenou chybu zabezpečení v technologii ASP.NET. Uvedená chyba zabezpečení umožňuje zpřístupnění informací. Útočník, který úspěšně zneužije tuto chybu zabezpečení, by mohl číst data, například stav zobrazení, která byla zašifrována na serveru. Tuto chybu zabezpečení lze zneužít také k manipulaci s daty, která by v případě úspěšného zneužití mohla být použita k dešifrování dat zašifrovaných na serveru, a manipulaci s nimi. Problém zpřístupnění obsahu souborů se netýká verzí rozhraní Microsoft .NET Framework předcházejících verzi Microsoft .NET Framework 3.5 Service Pack 1.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Vysoký</a><br />
Přístup k informacím</td>
<td style="border:1px solid black;">Může vyžadovat restartování</td>
<td style="border:1px solid black;">Microsoft Windows, Microsoft .NET Framework</td>
</tr>
</tbody>
</table>
<p></p>
  
Index zneužitelnosti  
--------------------
  

Následující tabulka uvádí hodnocení zneužitelnosti každé chyby zabezpečení uvedené v tomto měsíci. Chyby zabezpečení jsou řazeny v pořadí zmenšující se úrovně posouzení zneužitelnosti, jinak než tomu je u řazení podle čísla chyb. Uvedeny jsou pouze chyby zabezpečení ohodnocené stupněm závažnosti Kritický nebo Vysoký.
  
**Jak pracovat** **s touto tabulkou**
  
V této tabulce zjistíte, jaká je pravděpodobnost vydání funkčního zneužitelného kódu během 30 dní od vydání tohoto bulletinu zabezpečení pro všechny aktualizace zabezpečení, které bude třeba nainstalovat. Všechna níže uvedená hodnocení zvažte na základě vaší specifické konfigurace a podle závěrů hodnocení nastavte priority pro zavádění jednotlivých aktualizací. Další informace o významu těchto hodnocení a způsobu jejich stanovení najdete v indexu zneužitelnosti [Microsoft Exploitability Index](http://technet.microsoft.com/en-us/security/cc998259.aspx).
  
| ID bulletinu                                              | Název chyby zabezpečení                                                                                  | ID CVE                                                                           | Hodnocení indexu zneužitelnosti                                                                                                | Hlavní poznámky                                                                                    |  
|-----------------------------------------------------------|----------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------|  
| [MS10-062](http://go.microsoft.com/fwlink/?linkid=190884) | Chyba zabezpečení kodeku MPEG-4                                                                          | [CVE-2010-0818](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0818) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní zneužití kódu je pravděpodobné               | Z důvodu dodatečného omezení haldy je menší pravděpodobnost spuštění kódu u systému Windows Vista. |  
| [MS10-068](http://go.microsoft.com/fwlink/?linkid=190509) | Chyba zabezpečení týkající se přetečení haldy LSASS                                                      | [CVE-2010-0820](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0820) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní zneužití kódu je pravděpodobné               | (Žádné)                                                                                            |  
| [MS10-069](http://go.microsoft.com/fwlink/?linkid=197093) | Chyba zabezpečení umožňující místní zvýšení úrovně oprávnění CSRSS                                       | [CVE-2010-1891](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-1891) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní zneužití kódu je pravděpodobné               | (Žádné)                                                                                            |  
| [MS10-067](http://go.microsoft.com/fwlink/?linkid=197102) | Chyba zabezpečení týkající se poškození paměti textového převaděče WordPad pro soubory formátu Word 97   | [CVE-2010-2563](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2563) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní zneužití kódu je pravděpodobné               | (Žádné)                                                                                            |  
| [MS10-066](http://go.microsoft.com/fwlink/?linkid=197105) | Chyba zabezpečení týkající se poškození paměti protokolu RPC                                             | [CVE-2010-2567](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2567) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní zneužití kódu je pravděpodobné               | (Žádné)                                                                                            |  
| [MS10-061](http://go.microsoft.com/fwlink/?linkid=200505) | Chyba zabezpečení týkající se napodobování zařazovací služby tisku                                       | [CVE-2010-2729](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2729) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní zneužití kódu je pravděpodobné               | **V současné době dochází ke zneužití této chyby** **zabezpečení v prostředí Internetu.**          |  
| [MS10-070](http://go.microsoft.com/fwlink/?linkid=202409) | Chyba zabezpečení odsazení Oracle technologie ASP.NET                                                    | [CVE-2010-3332](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3332) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní zneužití kódu je pravděpodobné               | **V současné době dochází ke zneužití této chyby zabezpečení v prostředí Internetu.**              |  
| [MS10-065](http://go.microsoft.com/fwlink/?linkid=199537) | Chyba zabezpečení související s obejitím ověření adresáře                                                | [CVE-2010-2731](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2731) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní zneužití kódu je pravděpodobné               | **Tato chyba zabezpečení je veřejně známá.**                                                       |  
| [MS10-063](http://go.microsoft.com/fwlink/?linkid=200378) | Chyba zabezpečení týkající se poškození paměti modulu pro analýzu písma Uniscribe                        | [CVE-2010-2738](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2738) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní zneužití kódu je pravděpodobné               | (Žádné)                                                                                            |  
| [MS10-064](http://go.microsoft.com/fwlink/?linkid=200727) | Chyba zabezpečení týkající se přetečení vyrovnávací paměti založené na haldě v aplikaci Outlook          | [CVE-2010-2728](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2728) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Je pravděpodobné vytvoření kódu nekonsistentního zneužití | (Žádné)                                                                                            |  
| [MS10-065](http://go.microsoft.com/fwlink/?linkid=199537) | Chyba zabezpečení týkající se přetečení vyrovnávací paměti záhlaví požadavku                             | [CVE-2010-2730](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2730) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Je pravděpodobné vytvoření kódu nekonsistentního zneužití | (Žádné)                                                                                            |  
| [MS10-065](http://go.microsoft.com/fwlink/?linkid=199537) | Chyba zabezpečení týkající se opakovaného požadavku na parametry služby IIS způsobující odmítnutí služby | [CVE-2010-1899](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-1899) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Vytvoření funkčního zneužitelného kódu není pravděpodobné | Tato chyba může způsobit pouze odmítnutí služby.                                                   |
  
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
<th colspan="10" style="border:1px solid black;">
Windows XP  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor** **bulletinu**
</td>
<td style="border:1px solid black;">
[**MS10-061**](http://go.microsoft.com/fwlink/?linkid=200505)
</td>
<td style="border:1px solid black;">
[**MS10-062**](http://go.microsoft.com/fwlink/?linkid=190884)
</td>
<td style="border:1px solid black;">
[**MS10-063**](http://go.microsoft.com/fwlink/?linkid=200378)
</td>
<td style="border:1px solid black;">
[**MS10-065**](http://go.microsoft.com/fwlink/?linkid=199537)
</td>
<td style="border:1px solid black;">
[**MS10-066**](http://go.microsoft.com/fwlink/?linkid=197105)
</td>
<td style="border:1px solid black;">
[**MS10-067**](http://go.microsoft.com/fwlink/?linkid=197102)
</td>
<td style="border:1px solid black;">
[**MS10-068**](http://go.microsoft.com/fwlink/?linkid=190509)
</td>
<td style="border:1px solid black;">
[**MS10-069**](http://go.microsoft.com/fwlink/?linkid=197093)
</td>
<td style="border:1px solid black;">
[**MS10-070**](http://go.microsoft.com/fwlink/?linkid=202409)
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
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=93faba6b-0a85-4acc-b527-a012bbf56b13)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=2084a01c-2a91-4650-8665-7053015f2083)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=a1d47f30-c1fc-4b9d-8829-3bad1224006a)  
(KB981322)  
(Kritický)
</td>
<td style="border:1px solid black;">
IIS ASP:  
[Internetová informační služba 5.1](http://www.microsoft.com/downloads/details.aspx?familyid=555864c3-9114-4988-8526-7bf545a27706)  
(KB2124261)  
(Vysoký)  
Ověřování služby IIS:  
[Internetová informační služba 5.1](http://www.microsoft.com/downloads/details.aspx?familyid=ae55787e-4a5c-48d5-aedf-0abada514938)  
(KB2290570)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=7ad0f2cf-03dc-49a0-a16e-17fed0c01cc6)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=fc4369ec-864a-42ae-a850-b006872241fe)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Služba ADAM (Active Directory Application Mode)](http://www.microsoft.com/downloads/details.aspx?familyid=6554f98f-4dc5-4784-b92c-b0aae1fa22ca)  
(KB982000)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=20091358-7127-4ace-bf96-4319461ad305)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=a7990e61-21fd-4942-9dfe-af7961cb0282)  
(KB2416447)  
(Vysoký)  
[Microsoft .NET Framework 2.0 Service Pack 2 a Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=3d31fd37-eb58-4169-b6b9-4cf854524e46)  
(KB2418241)  
(Vysoký)  
[Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=d284237b-e4d9-460a-98f0-7a18252f5780)  
(KB2416468)  
(Vysoký)  
[Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=00d95a85-f3e8-464d-a10c-85c6d91b4aae)  
(KB2418240)  
(Vysoký)  
[Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=ae42d6cc-6d4e-425a-9b4f-379f66fc506a)  
(KB2416473)  
(Vysoký)  
[Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=6ce703b7-08a5-4eff-a062-d5dc720908f6)<sup>[1]</sup>
(KB2416472)  
(Vysoký)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=9f7f3737-056d-44bd-b644-51093b5b501b)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=284a0e80-fd03-4909-b354-0478f04585a1)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b27f310f-6ecc-4abb-8944-9fc24c66e077)  
(KB981322)  
(Kritický)
</td>
<td style="border:1px solid black;">
IIS ASP:  
[Internetová informační služba 6.0](http://www.microsoft.com/downloads/details.aspx?familyid=0b28bfac-783d-4c89-988b-4123c0343855)  
(KB2124261)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3349b12b-621e-48bc-9c57-489c7a56920d)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7567986a-261d-4def-9fa5-c667994c7844)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Služba ADAM (Active Directory Application Mode)](http://www.microsoft.com/downloads/details.aspx?familyid=5bc00f9a-3028-4c9d-be06-f2b78fa444c4)  
(KB982000)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=107eb958-b60f-40ae-a785-5d5b4d13d8c6)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=a7990e61-21fd-4942-9dfe-af7961cb0282)  
(KB2416447)  
(Vysoký)  
[Microsoft .NET Framework 2.0 Service Pack 2 a Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=3d31fd37-eb58-4169-b6b9-4cf854524e46)  
(KB2418241)  
(Vysoký)  
[Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=d284237b-e4d9-460a-98f0-7a18252f5780)  
(KB2416468)  
(Vysoký)  
[Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=00d95a85-f3e8-464d-a10c-85c6d91b4aae)  
(KB2418240)  
(Vysoký)  
[Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=ae42d6cc-6d4e-425a-9b4f-379f66fc506a)  
(KB2416473)  
(Vysoký)  
[Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=6ce703b7-08a5-4eff-a062-d5dc720908f6)<sup>[1]</sup>
(KB2416472)  
(Vysoký)
</td>
</tr>
<tr>
<th colspan="10" style="border:1px solid black;">
Windows Server 2003
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS10-061**](http://go.microsoft.com/fwlink/?linkid=200505)
</td>
<td style="border:1px solid black;">
[**MS10-062**](http://go.microsoft.com/fwlink/?linkid=190884)
</td>
<td style="border:1px solid black;">
[**MS10-063**](http://go.microsoft.com/fwlink/?linkid=200378)
</td>
<td style="border:1px solid black;">
[**MS10-065**](http://go.microsoft.com/fwlink/?linkid=199537)
</td>
<td style="border:1px solid black;">
[**MS10-066**](http://go.microsoft.com/fwlink/?linkid=197105)
</td>
<td style="border:1px solid black;">
[**MS10-067**](http://go.microsoft.com/fwlink/?linkid=197102)
</td>
<td style="border:1px solid black;">
[**MS10-068**](http://go.microsoft.com/fwlink/?linkid=190509)
</td>
<td style="border:1px solid black;">
[**MS10-069**](http://go.microsoft.com/fwlink/?linkid=197093)
</td>
<td style="border:1px solid black;">
[**MS10-070**](http://go.microsoft.com/fwlink/?linkid=202409)
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
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3d79680b-c071-462f-9cea-551fbd42edf0)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=0a942985-081f-455c-bf9d-4345392c91b0)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7ff7de2f-3e37-4aff-a8e4-5ed21b83575c)  
(KB981322)  
(Kritický)
</td>
<td style="border:1px solid black;">
IIS ASP:  
[Internetová informační služba 6.0](http://www.microsoft.com/downloads/details.aspx?familyid=29e6cf4f-446b-461c-82f7-cfa8478cf739)  
(KB2124261)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=f8b3004b-07db-4638-a9b7-224ff829081c)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3290e7ee-1e4a-464c-abfd-17fc4108601e)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Active Directory](http://www.microsoft.com/downloads/details.aspx?familyid=3fe6e78c-c60a-4903-9273-27b37e129f0a)  
(KB981550)  
(Vysoký)  
[Služba ADAM (Active Directory Application Mode)](http://www.microsoft.com/downloads/details.aspx?familyid=c42731f1-6393-42ed-b59f-5310c832fdc4)  
(KB982000)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=fd46ba66-8ca1-4aa2-b91b-9e5861a173f7)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=71f0daad-e2df-421c-9818-58e1e40cdb65)  
(KB2416451)  
(Vysoký)  
[Microsoft .NET Framework 2.0 Service Pack 2 a Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=3d31fd37-eb58-4169-b6b9-4cf854524e46)  
(KB2418241)  
(Vysoký)  
[Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=d284237b-e4d9-460a-98f0-7a18252f5780)  
(KB2416468)  
(Vysoký)  
[Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=00d95a85-f3e8-464d-a10c-85c6d91b4aae)  
(KB2418240)  
(Vysoký)  
[Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=ae42d6cc-6d4e-425a-9b4f-379f66fc506a)  
(KB2416473)  
(Vysoký)  
[Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=6ce703b7-08a5-4eff-a062-d5dc720908f6)<sup>[1]</sup>
(KB2416472)  
(Vysoký)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=073b3305-4a81-4ef8-b6aa-e53b31a936b4)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=284a0e80-fd03-4909-b354-0478f04585a1)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8382c1f2-e16d-475c-a8a0-e378696808f1)  
(KB981322)  
(Kritický)
</td>
<td style="border:1px solid black;">
IIS ASP:  
[Internetová informační služba 6.0](http://www.microsoft.com/downloads/details.aspx?familyid=750e4a79-11bf-4726-9eb4-5dd3d029a717)  
(KB2124261)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=612b2096-bd82-47ca-8b99-454c2f158d39)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b21570cc-4f90-4ed8-b901-a34584d44a63)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Active Directory](http://www.microsoft.com/downloads/details.aspx?familyid=22412eed-33cd-4dfc-8ef7-b74dcd7c5faf)  
(KB981550)  
(Vysoký)  
[Služba ADAM (Active Directory Application Mode)](http://www.microsoft.com/downloads/details.aspx?familyid=79fb639d-2cc1-4bea-9df6-c67ed95890e3)  
(KB982000)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ff5976e0-579c-4e6e-a225-c0d3913cdc85)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=a7990e61-21fd-4942-9dfe-af7961cb0282)  
(KB2416447)  
(Vysoký)  
[Microsoft .NET Framework 2.0 Service Pack 2 a Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=3d31fd37-eb58-4169-b6b9-4cf854524e46)  
(KB2418241)  
(Vysoký)  
[Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=d284237b-e4d9-460a-98f0-7a18252f5780)  
(KB2416468)  
(Vysoký)  
[Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=00d95a85-f3e8-464d-a10c-85c6d91b4aae)  
(KB2418240)  
(Vysoký)  
[Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=ae42d6cc-6d4e-425a-9b4f-379f66fc506a)  
(KB2416473)  
(Vysoký)  
[Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=6ce703b7-08a5-4eff-a062-d5dc720908f6)<sup>[1]</sup>
(KB2416472)  
(Vysoký)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 SP2 pro systémy s procesorem Itanium
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=ca35a520-c4da-41bb-abcc-d5bc534ff19a)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=be7b3310-ffb7-4528-9c9e-aebe14d264d6)  
(KB981322)  
(Kritický)
</td>
<td style="border:1px solid black;">
IIS ASP:  
[Internetová informační služba 6.0](http://www.microsoft.com/downloads/details.aspx?familyid=f6841057-1745-44e9-a16a-c180dd941ddf)  
(KB2124261)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=1f04f151-330a-4b6c-826e-76def35daa73)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=c9c4427d-54c8-4f3c-9a94-818196cd5180)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Active Directory](http://www.microsoft.com/downloads/details.aspx?familyid=cab75c8a-0d12-4a91-82b2-9f9b70610f67)  
(KB981550)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=e450ca08-1d75-4419-ad9f-c5e5efb55cd5)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=a7990e61-21fd-4942-9dfe-af7961cb0282)  
(KB2416447)  
(Vysoký)  
[Microsoft .NET Framework 2.0 Service Pack 2 a Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=3d31fd37-eb58-4169-b6b9-4cf854524e46)  
(KB2418241)  
(Vysoký)  
[Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=d284237b-e4d9-460a-98f0-7a18252f5780)  
(KB2416468)  
(Vysoký)  
[Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=00d95a85-f3e8-464d-a10c-85c6d91b4aae)  
(KB2418240)  
(Vysoký)  
[Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=ae42d6cc-6d4e-425a-9b4f-379f66fc506a)  
(KB2416473)  
(Vysoký)  
[Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=6ce703b7-08a5-4eff-a062-d5dc720908f6)<sup>[1]</sup>
(KB2416472)  
(Vysoký)
</td>
</tr>
<tr>
<th colspan="10" style="border:1px solid black;">
Windows Vista
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS10-061**](http://go.microsoft.com/fwlink/?linkid=200505)
</td>
<td style="border:1px solid black;">
[**MS10-062**](http://go.microsoft.com/fwlink/?linkid=190884)
</td>
<td style="border:1px solid black;">
[**MS10-063**](http://go.microsoft.com/fwlink/?linkid=200378)
</td>
<td style="border:1px solid black;">
[**MS10-065**](http://go.microsoft.com/fwlink/?linkid=199537)
</td>
<td style="border:1px solid black;">
[**MS10-066**](http://go.microsoft.com/fwlink/?linkid=197105)
</td>
<td style="border:1px solid black;">
[**MS10-067**](http://go.microsoft.com/fwlink/?linkid=197102)
</td>
<td style="border:1px solid black;">
[**MS10-068**](http://go.microsoft.com/fwlink/?linkid=190509)
</td>
<td style="border:1px solid black;">
[**MS10-069**](http://go.microsoft.com/fwlink/?linkid=197093)
</td>
<td style="border:1px solid black;">
[**MS10-070**](http://go.microsoft.com/fwlink/?linkid=202409)
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
[**Kritický**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritický**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Žádný
</td>
<td style="border:1px solid black;">
Žádný
</td>
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Žádný
</td>
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista Service Pack 1 a Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 a Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=028977fd-0f39-42d4-9fee-0d90a2931cfd)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 a Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=84629c25-7827-40c1-86fb-7ffa247202a0)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 a Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ac1b0260-3802-45d4-985e-ac827d784e4f)  
(KB981322)  
(Kritický)
</td>
<td style="border:1px solid black;">
IIS ASP:  
[Internetová informační služba 7.0](http://www.microsoft.com/downloads/details.aspx?familyid=75059175-9c59-45d5-81ce-09b964640e5f)  
(KB2124261)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Pouze Windows Vista Service Pack 2:  
[Active Directory Lightweight Directory Service (AD LDS)](http://www.microsoft.com/downloads/details.aspx?familyid=853a71f3-fb0d-43af-a2b8-45bf8ca1a588)  
(KB981550)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=a7990e61-21fd-4942-9dfe-af7961cb0282)  
(KB2416447)  
(Vysoký)  
[Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=00d95a85-f3e8-464d-a10c-85c6d91b4aae)  
(KB2418240)  
(Vysoký)  
[Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=ae42d6cc-6d4e-425a-9b4f-379f66fc506a)  
(KB2416473)  
(Vysoký)  
[Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=6ce703b7-08a5-4eff-a062-d5dc720908f6)<sup>[1]</sup>
(KB2416472)  
(Vysoký)  
Pouze Windows Vista Service Pack 1:  
[Microsoft .NET Framework 2.0 Service Pack 1 a Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=7ad59265-9dca-4731-ac09-46c162c1832a)  
(KB2416469)  
(Vysoký)  
Pouze Windows Vista Service Pack 1:  
[Microsoft .NET Framework 2.0 Service Pack 2 a Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=ac1c77df-34d5-48d4-9a9d-33dc017ffe93)  
(KB2416474)  
(Vysoký)  
Pouze Windows Vista Service Pack 2:  
[Microsoft .NET Framework 2.0 Service Pack 2, Microsoft .NET Framework 3.5 a Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=45aa5666-3454-443c-a224-2076215fef04)  
(KB2416470)  
(Vysoký)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 1 a Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 a Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c68b9337-883d-4e98-ba0a-90b5cad46184)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 a Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=36e2a74b-e5c6-47d5-9cd9-b9171be63c7d)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 a Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ebfdcd6d-413e-4359-8863-e992327a607f)  
(KB981322)  
(Kritický)
</td>
<td style="border:1px solid black;">
IIS ASP:  
[Internetová informační služba 7.0](http://www.microsoft.com/downloads/details.aspx?familyid=9864c590-10a7-4971-a717-924ed0d6cace)  
(KB2124261)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Pouze Windows Vista x64 Edition Service Pack 2:  
[Active Directory Lightweight Directory Service (AD LDS)](http://www.microsoft.com/downloads/details.aspx?familyid=566f468b-22b6-400a-a656-ae64cfcb52df)  
(KB981550)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=a7990e61-21fd-4942-9dfe-af7961cb0282)  
(KB2416447)  
(Vysoký)  
[Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=00d95a85-f3e8-464d-a10c-85c6d91b4aae)  
(KB2418240)  
(Vysoký)  
[Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=ae42d6cc-6d4e-425a-9b4f-379f66fc506a)  
(KB2416473)  
(Vysoký)  
[Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=6ce703b7-08a5-4eff-a062-d5dc720908f6)<sup>[1]</sup>
(KB2416472)  
(Vysoký)  
Pouze Windows Vista x64 Edition Service Pack 1:  
[Microsoft .NET Framework 2.0 Service Pack 1 a Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=7ad59265-9dca-4731-ac09-46c162c1832a)  
(KB2416469)  
(Vysoký)  
Pouze Windows Vista x64 Edition Service Pack 1:  
[Microsoft .NET Framework 2.0 Service Pack 2 a Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=ac1c77df-34d5-48d4-9a9d-33dc017ffe93)  
(KB2416474)  
(Vysoký)  
Pouze Windows Vista x64 Edition Service Pack 2:  
[Microsoft .NET Framework 2.0 Service Pack 2, Microsoft .NET Framework 3.5 a Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=45aa5666-3454-443c-a224-2076215fef04)  
(KB2416470)  
(Vysoký)
</td>
</tr>
<tr>
<th colspan="10" style="border:1px solid black;">
Windows Server 2008
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS10-061**](http://go.microsoft.com/fwlink/?linkid=200505)
</td>
<td style="border:1px solid black;">
[**MS10-062**](http://go.microsoft.com/fwlink/?linkid=190884)
</td>
<td style="border:1px solid black;">
[**MS10-063**](http://go.microsoft.com/fwlink/?linkid=200378)
</td>
<td style="border:1px solid black;">
[**MS10-065**](http://go.microsoft.com/fwlink/?linkid=199537)
</td>
<td style="border:1px solid black;">
[**MS10-066**](http://go.microsoft.com/fwlink/?linkid=197105)
</td>
<td style="border:1px solid black;">
[**MS10-067**](http://go.microsoft.com/fwlink/?linkid=197102)
</td>
<td style="border:1px solid black;">
[**MS10-068**](http://go.microsoft.com/fwlink/?linkid=190509)
</td>
<td style="border:1px solid black;">
[**MS10-069**](http://go.microsoft.com/fwlink/?linkid=197093)
</td>
<td style="border:1px solid black;">
[**MS10-070**](http://go.microsoft.com/fwlink/?linkid=202409)
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
[**Kritický**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritický**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Žádný
</td>
<td style="border:1px solid black;">
Žádný
</td>
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Žádný
</td>
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 pro 32bitové systémy a Windows Server 2008 pro 32bitové systémy Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro 32bitové systémy a Windows Server 2008 pro 32bitové systémy Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e2e788de-8400-4bf6-b96b-a915154aa20a)\*  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro 32bitové systémy a Windows Server 2008 pro 32bitové systémy Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=fdfc393e-a54d-44dd-ba45-c2a550ffd2a1)\*\*  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro 32bitové systémy a Windows Server 2008 pro 32bitové systémy Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b679fe0c-5498-4fc5-84c8-0cd24b625907)\*  
(KB981322)  
(Kritický)
</td>
<td style="border:1px solid black;">
IIS ASP:  
[Internetová informační služba 7.0](http://www.microsoft.com/downloads/details.aspx?familyid=d798dc8e-ae64-4a1d-abda-f58cf69779d8)\*  
(KB2124261)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Active Directory a Active Directory Lightweight Directory Service (AD LDS)](http://www.microsoft.com/downloads/details.aspx?familyid=1452befe-b7b8-4131-b36f-dded2bd16d5e)\*  
(KB981550)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=a7990e61-21fd-4942-9dfe-af7961cb0282)\*\*  
(KB2416447)  
(Vysoký)  
[Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=00d95a85-f3e8-464d-a10c-85c6d91b4aae)\*\*  
(KB2418240)  
(Vysoký)  
[Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=ae42d6cc-6d4e-425a-9b4f-379f66fc506a)\*\*  
(KB2416473)  
(Vysoký)  
[Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=6ce703b7-08a5-4eff-a062-d5dc720908f6)\*\*<sup>[1]</sup>
(KB2416472)  
(Vysoký)  
Pouze Windows Server 2008 pro 32bitové systémy:  
[Microsoft .NET Framework 2.0 Service Pack 1 a Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=7ad59265-9dca-4731-ac09-46c162c1832a)\*\*  
(KB2416469)  
(Vysoký)  
Pouze Windows Server 2008 pro 32bitové systémy:  
[Microsoft .NET Framework 2.0 Service Pack 2 a Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=ac1c77df-34d5-48d4-9a9d-33dc017ffe93)\*\*  
(KB2416474)  
(Vysoký)  
Pouze Windows Server 2008 pro 32bitové systémy s aktualizací Service Pack 2:  
[Microsoft .NET Framework 2.0 Service Pack 2, Microsoft .NET Framework 3.5 a Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=45aa5666-3454-443c-a224-2076215fef04)\*\*  
(KB2416470)  
(Vysoký)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 pro systémy s procesorem x64 a Windows Server 2008 pro systémy s procesorem x64 Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem x64 a Windows Server 2008 pro systémy s procesorem x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e08d4f49-5a13-4e1d-b0a7-27b314c2edb5)\*  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem x64 a Windows Server 2008 pro systémy s procesorem x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=1b7af424-6286-4a80-827c-c4df4f92fe43)\*\*  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem x64 a Windows Server 2008 pro systémy s procesorem x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e1b38b87-24f6-4aaa-afa9-40f4015d6694)\*  
(KB981322)  
(Kritický)
</td>
<td style="border:1px solid black;">
IIS ASP:  
[Internetová informační služba 7.0](http://www.microsoft.com/downloads/details.aspx?familyid=e29f01dc-b00d-4c12-a13e-63aa0b09d919)\*  
(KB2124261)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Active Directory a Active Directory Lightweight Directory Service (AD LDS)](http://www.microsoft.com/downloads/details.aspx?familyid=38eb875f-1869-401b-b7d3-9f18f4ba4f24)\*  
(KB981550)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=a7990e61-21fd-4942-9dfe-af7961cb0282)\*\*  
(KB2416447)  
(Vysoký)  
[Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=00d95a85-f3e8-464d-a10c-85c6d91b4aae)\*\*  
(KB2418240)  
(Vysoký)  
[Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=ae42d6cc-6d4e-425a-9b4f-379f66fc506a)\*\*  
(KB2416473)  
(Vysoký)  
[Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=6ce703b7-08a5-4eff-a062-d5dc720908f6)\*\*<sup>[1]</sup>
(KB2416472)  
(Vysoký)  
Pouze Windows Server 2008 pro systémy s procesorem x64:  
[Microsoft .NET Framework 2.0 Service Pack 1 a Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=7ad59265-9dca-4731-ac09-46c162c1832a)\*\*  
(KB2416469)  
(Vysoký)  
Pouze Windows Server 2008 pro systémy s procesorem x64:  
[Microsoft .NET Framework 2.0 Service Pack 2 a Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=ac1c77df-34d5-48d4-9a9d-33dc017ffe93)\*\*  
(KB2416474)  
(Vysoký)  
Pouze Windows Server 2008 pro systémy s procesorem x64 s aktualizací Service Pack 2:  
[Microsoft .NET Framework 2.0 Service Pack 2, Microsoft .NET Framework 3.5 a Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=45aa5666-3454-443c-a224-2076215fef04)\*\*  
(KB2416470)  
(Vysoký)  
Pouze Windows Server 2008 pro systémy s procesorem x64 s aktualizací Service Pack 2:  
[Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=00d95a85-f3e8-464d-a10c-85c6d91b4aae)\*\*  
(KB2418240)  
(Vysoký)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 pro systémy s procesorem Itanium a Windows Server 2008 pro systémy s procesorem Itanium Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem Itanium a Windows Server 2008 pro systémy s procesorem Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=098537d5-bf6e-4e04-ad33-1cde697e062f)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem Itanium a Windows Server 2008 pro systémy s procesorem Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ceb856e8-f4a6-4229-bd26-b1a763d7d443)  
(KB981322)  
(Kritický)
</td>
<td style="border:1px solid black;">
IIS ASP:  
[Internetová informační služba 7.0](http://www.microsoft.com/downloads/details.aspx?familyid=d595c8d2-90b1-46e4-bb9f-60efd0bf3a02)  
(KB2124261)  
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
Netýká se
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=a7990e61-21fd-4942-9dfe-af7961cb0282)  
(KB2416447)  
(Vysoký)  
[Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=ae42d6cc-6d4e-425a-9b4f-379f66fc506a)  
(KB2416473)  
(Vysoký)  
[Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=6ce703b7-08a5-4eff-a062-d5dc720908f6)<sup>[1]</sup>
(KB2416472)  
(Vysoký)  
Pouze Windows Server 2008 pro systémy s procesorem Itanium:  
[Microsoft .NET Framework 2.0 Service Pack 1 a Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=7ad59265-9dca-4731-ac09-46c162c1832a)  
(KB2416469)  
(Vysoký)  
Pouze Windows Server 2008 pro systémy s procesorem Itanium:  
[Microsoft .NET Framework 2.0 Service Pack 2 a Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=ac1c77df-34d5-48d4-9a9d-33dc017ffe93)  
(KB2416474)  
(Vysoký)  
Pouze Windows Server 2008 pro systémy s procesorem Itanium s aktualizací Service Pack 2:  
[Microsoft .NET Framework 2.0 Service Pack 2, Microsoft .NET Framework 3.5 a Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=45aa5666-3454-443c-a224-2076215fef04)  
(KB2416470)  
(Vysoký)
</td>
</tr>
<tr>
<th colspan="10" style="border:1px solid black;">
Windows 7
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS10-061**](http://go.microsoft.com/fwlink/?linkid=200505)
</td>
<td style="border:1px solid black;">
[**MS10-062**](http://go.microsoft.com/fwlink/?linkid=190884)
</td>
<td style="border:1px solid black;">
[**MS10-063**](http://go.microsoft.com/fwlink/?linkid=200378)
</td>
<td style="border:1px solid black;">
[**MS10-065**](http://go.microsoft.com/fwlink/?linkid=199537)
</td>
<td style="border:1px solid black;">
[**MS10-066**](http://go.microsoft.com/fwlink/?linkid=197105)
</td>
<td style="border:1px solid black;">
[**MS10-067**](http://go.microsoft.com/fwlink/?linkid=197102)
</td>
<td style="border:1px solid black;">
[**MS10-068**](http://go.microsoft.com/fwlink/?linkid=190509)
</td>
<td style="border:1px solid black;">
[**MS10-069**](http://go.microsoft.com/fwlink/?linkid=197093)
</td>
<td style="border:1px solid black;">
[**MS10-070**](http://go.microsoft.com/fwlink/?linkid=202409)
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
Žádný
</td>
<td style="border:1px solid black;">
Žádný
</td>
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Žádný
</td>
<td style="border:1px solid black;">
Žádný
</td>
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Žádný
</td>
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 pro 32bitové systémy
</td>
<td style="border:1px solid black;">
[Windows 7 pro 32bitové systémy](http://www.microsoft.com/downloads/details.aspx?familyid=34619e9e-1f00-40e4-be6f-5bbf5e3c801b)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
IIS ASP:  
[Internetová informační služba 7.5](http://www.microsoft.com/downloads/details.aspx?familyid=5b2d42da-4dbc-4fbb-be22-09ca7dec5aa3)  
(KB2124261)  
(Vysoký)  
IIS FastCGI:  
[Internetová informační služba 7.5](http://www.microsoft.com/downloads/details.aspx?familyid=c843afd9-b6f2-48de-91cc-1c0d481c2be4)  
(KB2271195)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Active Directory Lightweight Directory Service (AD LDS)](http://www.microsoft.com/downloads/details.aspx?familyid=454fc025-bfa2-4552-9522-3585f523ecb2)  
(KB981550)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=5e7dcf51-74f1-43cc-aece-0cd5df05ddb7)  
(KB2416471)  
(Vysoký)  
[Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=6ce703b7-08a5-4eff-a062-d5dc720908f6)<sup>[1]</sup>
(KB2416472)  
(Vysoký)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 7 pro 32bitové systémy Service Pack 1
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
[Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=6ce703b7-08a5-4eff-a062-d5dc720908f6)<sup>[1]</sup>
(KB2416472)  
(Vysoký)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 pro systémy s procesorem x64
</td>
<td style="border:1px solid black;">
[Windows 7 pro systémy s procesorem x64](http://www.microsoft.com/downloads/details.aspx?familyid=dbb747a5-658d-44cf-bd49-425d1700157f)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
IIS ASP:  
[Internetová informační služba 7.5](http://www.microsoft.com/downloads/details.aspx?familyid=66b64374-95e4-4b99-80e6-98dc63cd272b)  
(KB2124261)  
(Vysoký)  
IIS FastCGI:  
[Internetová informační služba 7.5](http://www.microsoft.com/downloads/details.aspx?familyid=5f0c0454-cbb6-47ed-9227-98aa45b8cbdb)  
(KB2271195)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Active Directory Lightweight Directory Service (AD LDS)](http://www.microsoft.com/downloads/details.aspx?familyid=b15ad533-3cf1-4dcf-847c-05ebffb84e26)  
(KB981550)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=5e7dcf51-74f1-43cc-aece-0cd5df05ddb7)  
(KB2416471)  
(Vysoký)  
[Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=6ce703b7-08a5-4eff-a062-d5dc720908f6)<sup>[1]</sup>
(KB2416472) (Vysoký)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 7 pro systémy s procesorem x64 Service Pack 1
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
[Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=6ce703b7-08a5-4eff-a062-d5dc720908f6)<sup>[1]</sup>
(KB2416472) (Vysoký)
</td>
</tr>
<tr>
<th colspan="10" style="border:1px solid black;">
Windows Server 2008 R2
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS10-061**](http://go.microsoft.com/fwlink/?linkid=200505)
</td>
<td style="border:1px solid black;">
[**MS10-062**](http://go.microsoft.com/fwlink/?linkid=190884)
</td>
<td style="border:1px solid black;">
[**MS10-063**](http://go.microsoft.com/fwlink/?linkid=200378)
</td>
<td style="border:1px solid black;">
[**MS10-065**](http://go.microsoft.com/fwlink/?linkid=199537)
</td>
<td style="border:1px solid black;">
[**MS10-066**](http://go.microsoft.com/fwlink/?linkid=197105)
</td>
<td style="border:1px solid black;">
[**MS10-067**](http://go.microsoft.com/fwlink/?linkid=197102)
</td>
<td style="border:1px solid black;">
[**MS10-068**](http://go.microsoft.com/fwlink/?linkid=190509)
</td>
<td style="border:1px solid black;">
[**MS10-069**](http://go.microsoft.com/fwlink/?linkid=197093)
</td>
<td style="border:1px solid black;">
[**MS10-070**](http://go.microsoft.com/fwlink/?linkid=202409)
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
Žádný
</td>
<td style="border:1px solid black;">
Žádný
</td>
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Žádný
</td>
<td style="border:1px solid black;">
Žádný
</td>
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Žádný
</td>
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 pro systémy s procesorem x64
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem x64](http://www.microsoft.com/downloads/details.aspx?familyid=11e20088-1be2-4166-9c97-234b7e9f1c4f)\*  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
IIS ASP:  
[Internetová informační služba 7.5](http://www.microsoft.com/downloads/details.aspx?familyid=21458cce-f67e-4e95-a067-8311afefc261)\*  
(KB2124261)  
(Vysoký)  
IIS FastCGI:  
[Internetová informační služba 7.5](http://www.microsoft.com/downloads/details.aspx?familyid=9578b1de-f2c1-4b37-9d82-69e929cab6f3)\*  
(KB2271195)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Active Directory a Active Directory Lightweight Directory Service (AD LDS)](http://www.microsoft.com/downloads/details.aspx?familyid=54f36389-8be4-4a0c-9640-dc32addac9d7)\*  
(KB981550)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=5e7dcf51-74f1-43cc-aece-0cd5df05ddb7)\*  
(KB2416471)  
(Vysoký)  
[Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=6ce703b7-08a5-4eff-a062-d5dc720908f6)<sup>[1]</sup>
(KB2416472)  
(Vysoký)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 pro systémy s procesorem x64 Service Pack 1
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
[Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=6ce703b7-08a5-4eff-a062-d5dc720908f6)\*<sup>[1]</sup>
(KB2416472)  
(Vysoký)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 pro systémy s procesorem Itanium
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=d8c635f8-8978-44bf-b457-e07368f08ef4)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
IIS ASP:  
[Internetová informační služba 7.5](http://www.microsoft.com/downloads/details.aspx?familyid=3b8f3fd1-1ef4-4e9f-9bce-0c68f10519d1)  
(KB2124261)  
(Vysoký)  
IIS FastCGI:  
[Internetová informační služba 7.5](http://www.microsoft.com/downloads/details.aspx?familyid=21adf80d-267f-47cd-9c03-4b4854ba159f)  
(KB2271195)  
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
Netýká se
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=5e7dcf51-74f1-43cc-aece-0cd5df05ddb7)  
(KB2416471)  
(Vysoký)  
[Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=6ce703b7-08a5-4eff-a062-d5dc720908f6)<sup>[1]</sup>
(KB2416472)  
(Vysoký)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 pro systémy s procesorem Itanium Service Pack 1
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
[Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=6ce703b7-08a5-4eff-a062-d5dc720908f6)<sup>[1]</sup>
(KB2416472)  
(Vysoký)
</td>
</tr>
</table>
<p></p>
 
**Poznámky k systémům Windows Server 2008 a Windows Server 2008 R2**

**\*Instalace Server Core obsahující** **chybu zabezpečení** Tato aktualizace se stejným hodnocením závažnosti se vztahuje k podporovaným edicím systému Windows Server 2008 nebo Windows Server 2008 R2, jak je uvedeno, s instalací pomocí volby pro instalaci Server Core nebo bez ní. Další informace o této možnosti instalace naleznete v článcích na webu TechNet [Managing a Server Core Installation](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) (Správa instalace Server Core) a [Servicing a Server Core Installation](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx) (Obsluha instalace Server Core). Možnost instalace Server Core se nevztahuje na určité edice systému Windows Server 2008 a Windows Server 2008 R2; další informace naleznete v části [Porovnání možností instalace Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**\*\*Instalace Server Core není touto chybou ovlivněna.** Chyby zabezpečení, které tato aktualizace řeší, nijak neovlivňují podporované edice systému Windows Server 2008 v případě instalace s využitím možnosti instalace Server Core. Další informace o této možnosti instalace naleznete v článcích na webu TechNet [Managing a Server Core Installation](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) (Správa instalace Server Core) a [Servicing a Server Core Installation](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx) (Obsluha instalace Server Core). Možnost instalace Server Core se nevztahuje na určité edice systému Windows Server 2008 a Windows Server 2008 R2; další informace naleznete v části [Porovnání možností instalace Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**Poznámka k bulletinu MS10-063**

Více aktualizovaných souborů v rámci stejného identifikátoru bulletinu naleznete také v dalších kategoriích softwaru v rámci této části Software obsahující tuto chybu a umístění aktualizací ke stažení. Tento bulletin se vztahuje na více kategorií softwaru.

**Poznámka k bulletinu MS10-070**

<sup>[1]</sup>**Rozhraní .NET Framework 4.0 Client Profile není postiženo.** Distribuční balíčky rozhraní .NET Framework verze 4 jsou k dispozici ve dvou profilech: .NET Framework 4.0 a .NET Framework 4.0 Client Profile. Rozhraní .NET Framework 4.0 Client Profile je verzí rozhraní .NET Framework 4.0. Chyba zabezpečení řešená v této aktualizaci se týká pouze rozhraní .NET Framework 4.0, nikoli rozhraní .NET Framework 4.0 Client Profile. Další informace naleznete zde: [Instalace rozhraní .NET Framework](http://msdn.microsoft.com/en-us/library/5a4x27ek.aspx).

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
[**MS10-063**](http://go.microsoft.com/fwlink/?linkid=200378)
</td>
<td style="border:1px solid black;">
[**MS10-064**](http://go.microsoft.com/fwlink/?linkid=200727)
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
[**Kritický**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Office XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=0b56f85f-d39b-410a-857a-799a5d714de7)  
(KB2288608)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Microsoft Outlook 2002 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=d5e85841-9dea-4776-9e0e-3cd272066f37)  
(KB2293422)  
(Kritický)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2003 Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Office 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=bb7783b1-b396-4254-b317-f2292b305cfc)  
(KB2288613)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Microsoft Outlook 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=ec8ed81e-05d0-4c20-b5fb-ebc72230a8bd)  
(KB2293428)  
(Vysoký)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2007 Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft Office 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=44c5bccf-66dd-4796-9089-e6171d8c9785)  
(KB2288621)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Microsoft Outlook 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=6009d507-135c-4ce8-a830-925134f214dc)  
(KB2288953)  
(Vysoký)
</td>
</tr>
</table>
<p></p>
 
**Poznámka k bulletinu MS10-063**

Více aktualizovaných souborů v rámci stejného identifikátoru bulletinu naleznete také v dalších kategoriích softwaru v rámci této části Software obsahující tuto chybu a umístění aktualizací ke stažení. Tento bulletin se vztahuje na více kategorií softwaru.

Nástroje a doporučené postupy zjišťování a nasazení
---------------------------------------------------


**Centrum zabezpečení**

Umožňuje správu aktualizací softwaru a zabezpečení, které je třeba nainstalovat na servery, stolní počítače a přenosné počítače v organizaci. Další informace naleznete na webu [TechNet Update Management Center](http://go.microsoft.com/fwlink/?linkid=69903). Další informace o zabezpečení produktů společnosti Microsoft nabízí web [Centrum zabezpečení TechNet](http://go.microsoft.com/fwlink/?linkid=21171). Tyto informace lze také získat kliknutím na nabídku „Nejnovější aktualizace zabezpečení“ na webu [Zabezpečení doma](http://go.microsoft.com/fwlink/?linkid=85102).

Aktualizace zabezpečení jsou k dispozici na webu [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747) a [Windows Update](http://go.microsoft.com/fwlink/?linkid=21130). Aktualizace zabezpečení jsou také k dispozici na webu [služby Stažení softwaru](http://go.microsoft.com/fwlink/?linkid=21129). Nejsnadněji je naleznete hledáním podle klíčových slov aktualizace zabezpečení.

Aktualizace zabezpečení lze stáhnout z katalogu služby [Microsoft Update Catalog](http://go.microsoft.com/fwlink/?linkid=96155). Služba Microsoft Update Catalog poskytuje katalog s možností vyhledávání obsahu dostupného prostřednictvím služeb Windows Update a Microsoft Update, včetně aktualizací zabezpečení, ovladačů a aktualizací Service Pack. Vyhledáváním pomocí čísla bulletinu zabezpečení (například MS07-036) můžete přidat všechny dostupné aktualizace do košíku (včetně různých jazykových verzí aktualizace) a stáhnout je do vybrané složky. Další informace o službě Microsoft Update Catalog najdete v části [Nejčastější dotazy týkající se služby Microsoft Update Catalog](http://go.microsoft.com/fwlink/?linkid=97900).

**Doporučené postupy zjišťování a instalace**

Společnost Microsoft poskytuje doporučené postupy zjišťování a nasazení aktualizací zabezpečení. Tyto dokumenty obsahují doporučení a informace, které mohou odborníkům v oblasti IT pomoci porozumět, jak se používají různé nástroje pro detekci a nasazení aktualizací zabezpečení. Další informace získáte v [článku 961747 znalostní báze Microsoft Knowledge Base](http://support.microsoft.com/kb/961747).

**Nástroj Microsoft Baseline Security Analyzer**

Pomocí nástroje Microsoft Baseline Security Analyzer (MBSA) mohou správci prohledávat místní i vzdálené systémy a zjistit tak, jestli v nich nechybí některé aktualizace zabezpečení nebo jestli v nastavení zabezpečení systému nedošlo k některým běžným chybám. Další informace o nástroji MBSA získáte na webu [Microsoft Baseline Security Analyzer](http://go.microsoft.com/fwlink/?linkid=21134).

**Služba Windows Server Update Services**

Pomocí služby Windows Server Update Services (WSUS) mohou správci systémů rychle a spolehlivě nasadit nejnovější důležité aktualizace zabezpečení pro systémy Microsoft Windows 2000 a novější, systém Office XP a novější, Exchange Server 2003 a SQL Server 2000 do systémů Microsoft Windows 2000 a novějších.

Další informace o způsobu instalace této aktualizace zabezpečení pomocí služby Windows Server Update Services získáte na webu služby [Windows Server Update Services](http://go.microsoft.com/fwlink/?linkid=50120).

**Systems Management Server**

Microsoft Systems Management Server (SMS) představuje v rozlehlých sítích řešení pro správu aktualizací s rozsáhlými možnostmi konfigurace. Umožňuje správcům identifikovat počítače se systémem Windows, které vyžadují aktualizace zabezpečení, a provést řízenou instalaci těchto aktualizací v celé rozlehlé síti s minimálním dopadem na koncové uživatele. K dispozici je nyní nová verze nástroje SMS, System Center Configuration Manager 2007 (viz také webové stránky produktu [System Center Configuration Manager 2007](http://technet.microsoft.com/en-us/library/bb735860.aspx)). Další informace o tom, jak mohou správci pomocí serveru SMS 2003 nasazovat aktualizace zabezpečení, získáte na webu [SMS 2003 Security Patch Management](http://go.microsoft.com/fwlink/?linkid=22939). Uživatelé služby SMS 2.0 mohou k nasazení aktualizací zabezpečení použít také nástroj SUIT (Security Update Inventory Tool). Další informace o serveru SMS získáte na webu [Microsoft Systems Management Server](http://go.microsoft.com/fwlink/?linkid=21158).

**Poznámka:** Služba SMS pomocí modulu Microsoft Baseline Security Analyzer poskytuje rozsáhlou podporu při zjišťování a nasazení aktualizací bulletinu zabezpečení. Tyto nástroje nemusí některé softwarové aktualizace zjistit. V takovém případě mohou správci použít funkce serveru SMS a nasměrovat aktualizace do určitých systémů. Další informace o tomto postupu naleznete na webu [Nasazení aktualizací softwaru pomocí funkce Distribuce softwaru serveru SMS](http://go.microsoft.com/fwlink/?linkid=33341). Některé aktualizace zabezpečení vyžadují po restartování počítače oprávnění správce. Správci mohou k instalaci těchto aktualizací použít nástroj Elevated Rights Deployment Tool (k dispozici v sadě [SMS 2.0 Administration Feature Pack](http://go.microsoft.com/fwlink/?linkid=21161)).

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

-   Aktualizace zabezpečení jsou k dispozici na webu [služby Stažení softwaru](http://go.microsoft.com/fwlink/?linkid=21129). Nejsnadněji je naleznete hledáním podle klíčových slov aktualizace zabezpečení.
-   Aktualizace pro klientské platformy jsou k dispozici na webu [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747).
-   Aktualizace zabezpečení nabízené tento měsíc na webu Windows Update jsou k dispozici na webu služby Stažení softwaru v souborech obrazu ISO disku CD s vydanými aktualizacemi zabezpečení a kritickými aktualizacemi. Další informace získáte v [článku 913086 znalostní báze Microsoft Knowledge Base](http://support.microsoft.com/kb/913086).

**Komunita odborníků v oblasti zabezpečení**

Na webu [IT Pro Security Community](http://go.microsoft.com/fwlink/?linkid=21164) se můžete naučit, jak zlepšit zabezpečení a optimalizovat infrastrukturu IT, a diskutovat s dalšími členy komunity odborníků o bezpečnostních tématech.

#### Poděkování

Společnost Microsoft tímto [děkuje](http://go.microsoft.com/fwlink/?linkid=21127) za spolupráci při ochraně zákazníků:

-   Sergeji Golovanovi, Alexanderu Gostevovi, Maximu Golovkinovi a Alexeji Monastyrskému ze společnosti [Kaspersky Lab](http://www.kaspersky.com/) a Vitaliji Kiktenkovi a Alexanderu Saprykinovi ze společnosti [Design and Test Lab](http://www.dnt-lab.com/) za oznámení chyby popsané v bulletinu MS10-061.
-   Liamu O. Morchuovi ze společnosti [Symantec](http://www.symantec.com/index.jsp) za oznámení chyby popsané v bulletinu MS10-061.
-   Matthewovi Watchinskému ze společnosti [Sourcefire VRT](http://www.sourcefire.com/services/sf_vrt.html) za oznámení chyby popsané v bulletinu MS10-062.
-   Carstenu Bookovi ze společnosti za oznámení chyby popsané v bulletinu MS10-063.
-   Marcu Schoenefeldovi ze společnosti Red Hat Security Response Team za oznámení chyby popsané v bulletinu MS10-063.
-   Carstenu H. Eiramovi ze společnosti [Secunia](http://secunia.com/) za oznámení informace vedoucí ke změně indexu zneužitelnosti pro chybu zabezpečení CVE-2010-2738 v bulletinu MS10-063.
-   Dyonu Baldingovi ze společnosti [Secunia](http://secunia.com/) za oznámení chyby popsané v bulletinu MS10-064.
-   Jinsik Shimovi za oznámení chyby popsané v bulletinu MS10-065.
-   Travisu Rayboldovi ze společnosti Rubicon West za oznámení chyby popsané v bulletinu MS10-065.
-   Yamatu Liovi ze společnosti [Palo Alto Networks](http://www.paloaltonetworks.com/) za oznámení chyby popsané v bulletinu MS10-066.
-   S0lute ze společnosti [iDefense Labs](http://labs.idefense.com/) za oznámení chyby popsané v bulletinu MS10-067.
-   Společnosti [IBM Japan](http://www.ibm.com/jp/ja/) za oznámení chyby popsané v bulletinu MS10-069.

#### Technická podpora

-   Uvedený software byl testován za účelem zjištění, kterých verzí se chyba týká. U dalších verzí skončila časově omezená podpora. Pokud chcete zjistit dobu, po kterou je pro určitou verzi softwaru poskytována podpora, navštivte web [Zásady poskytování technické podpory pro produkty společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=21742).
-   Zákazníci mohou získat technickou podporu na webu [služby technické podpory společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=21131). Hovory související s aktualizacemi zabezpečení jsou bezplatné. Další informace o dostupných možnostech technické podpory naleznete na webu [Pomoc a podpora společnosti Microsoft](http://support.microsoft.com/).
-   Mezinárodní zákazníci získají podporu u místních zastoupení společnosti Microsoft. Technická podpora související s aktualizacemi zabezpečení je bezplatná. Další informace o možnostech kontaktování společnosti Microsoft v případě potřeby technické podpory získáte na [webu mezinárodní technické podpory](http://go.microsoft.com/fwlink/?linkid=21155).

#### Zřeknutí se záruky

Informace ve znalostní bázi Microsoft Knowledge Base jsou poskytovány tak, jak jsou, bez jakékoli záruky. Společnost Microsoft neposkytuje žádné záruky, výslovně uvedené či mlčky předpokládané, včetně záruk obchodovatelnosti a vhodnosti pro určitý účel. Společnost Microsoft ani její dodavatelé nenesou v žádném případě zodpovědnost za žádné škody, včetně přímých, nepřímých, náhodných či následných škod, ztráty zisku či zvláštních škod, a to ani v případě, že byli na možnost takových škod upozorněni. V některých zemích a právních řádech není dovoleno vyloučit nebo omezit odpovědnost, proto se výše uvedené omezení na vás nemusí vztahovat.

#### Revize

-   V1.0 (14. září 2010): Souhrnný bulletin byl publikován.
-   V2.0 (22. září 2010): Byl zvýšen hodnoticí stupeň indexu zneužitelnosti pro chybu zabezpečení CVE-2010-2738 a snížen hodnoticí stupeň indexu zneužitelnosti pro chybu zabezpečení CVE-2010-2730. Zároveň byla revidována důležitá poznámka týkající se indexu zneužitelnosti pro chybu zabezpečení CVE-2010-0818.
-   V3.0 (28. září 2010): Byl přidán bulletin zabezpečení společnosti Microsoft MS10-070: Chyba zabezpečení technologie ASP.NET může umožnit přístup k informacím (2418042). Také byl přidán odkaz na webové přenosy tohoto mimořádného bulletinu zabezpečení.
-   V4.0 (30. září 2010): Do tohoto souhrnného bulletinu byla přidána informace, že aktualizace pro bulletin zabezpečení MS10-070 jsou nyní k dispozici prostřednictvím všech distribučních kanálů, včetně webů Windows Update a Microsoft Update. Zároveň byly revidovány podrobné informace u aktualizací KB2418240, KB2418241, KB2416470 a KB2416474 určených pro bulletin zabezpečení MS10-070.
-   V4.1 (3. listopadu 2010): V bulletinu MS10-070 bylo do tabulky softwaru obsahujícího chybu přidána poznámka vysvětlující, že rozhraní .NET Framework 4.0 Client Profile není postiženo.
-   V5.0 (14. prosince 2010): Do tohoto souhrnného bulletinu byla přidána informace týkající se bulletinu zabezpečení MS10-070, že jsou k dispozici nové balíčky aktualizací pro rozhraní .NET Framework 4.0 (KB2416472) opravující problém s instalací, který mohl působit potíže při instalaci jiných aktualizací či produktů. Zákazníci, kteří svůj systém již úspěšně aktualizovali, nemusejí podnikat žádná opatření.
-   V6.0 (22. února 2011): Bulletin zabezpečení MS10-070: Změna detekce nyní nabízí balíčky aktualizací rozhraní Microsoft .NET Framework 4.0 (KB2416472) zákazníkům, kteří si po instalaci systému Windows 7 pro 32bitové systémy Service Pack 1, Windows 7 pro systémy s procesorem x64 Service Pack 1, Windows Server 2008 R2 pro systémy s procesorem x64 Service Pack 1 nebo Windows Server 2008 R2 pro systémy s procesorem Itanium Service Pack 1 nainstalují rozhraní Microsoft .NET Framework 4.0. Zákazníci, kteří svůj systém již úspěšně aktualizovali, nemusejí podnikat žádná opatření.
-   V6.1 (26. října 2011): V bulletinu MS10-070 byla opravena informace o použitelnosti instalace Server Core pro rozhraní .NET Framework 4 v systému Windows Server 2008 R2 pro systémy s procesorem x64.

*Built at 2014-04-18T01:50:00Z-07:00*
