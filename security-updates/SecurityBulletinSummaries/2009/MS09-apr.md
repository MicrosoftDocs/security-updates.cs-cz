---
TOCTitle: 'MS09-APR'
Title: 'Souhrnný bulletin zabezpečení společnosti Microsoft, duben 2009'
ms:assetid: 'ms09-apr'
ms:contentKeyID: 61223982
ms:mtpsurl: 'https://technet.microsoft.com/cs-CZ/library/ms09-apr(v=Security.10)'
---

Security Bulletin Summary

Souhrnný bulletin zabezpečení společnosti Microsoft, duben 2009
===============================================================

Publikováno: 14. dubna 2009 | Aktualizováno: 16. dubna 2009

**Verze:** 1.1

Tento souhrnný bulletin uvádí bulletiny zabezpečení vydané v dubnu 2009.

Spolu s vydáním bulletinů pro duben 2009 nahrazuje tento souhrnný bulletin předběžné oznámení o bulletinech vydané 9. dubna 2009. Další informace o službě předběžného oznámení o bulletinech naleznete v části [Předběžné oznámení o bulletinech zabezpečení společnosti Microsoft](http://technet.microsoft.com/security/bulletin/advance).

Informace o tom, jak dostávat automatická oznámení o vydání nových bulletinů zabezpečení společnosti Microsoft, naleznete na webu [Zasílání technických oznámení o zabezpečení společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=21163).

Pro zodpovězení zákaznických dotazů týkajících se těchto bulletinů uspořádá společnost Microsoft webové vysílání 15. dubna 2009 v 11:00 časového pásma Tichomoří (USA a Kanada). [Registrovat se pro webové vysílání týkající se dubnových bulletinů zabezpečení](http://msevents.microsoft.com/cui/webcasteventdetails.aspx?eventid=1032395126). Po tomto datu je webové vysílání dostupné na požádání. Další informace získáte v [souhrnných bulletinech zabezpečení společnosti Microsoft a webovém vysílání](http://technet.microsoft.com/security/bulletin/summary).

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
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=139849">MS09-010</a></td>
<td style="border:1px solid black;"><strong>Chyby zabezpečení v převaděči WordPad a převaděčích textu systému Office umožňují vzdálené spuštění kódu (960477)</strong><br />
<br />
Tato aktualizace zabezpečení řeší dvě veřejně známé a dvě soukromými osobami oznámené chyby zabezpečení v převaděči Microsoft WordPad a převaděčích textu systému Microsoft Office. Tyto chyby zabezpečení umožňují vzdálené spuštění kódu v případě, že dojde k otevření speciálně vytvořeného souboru v převaděči WordPad nebo aplikaci Microsoft Office Word. Neotvírejte soubory systému Microsoft Office, soubory ve formátu RTF nebo soubory aplikace Write či WordPerfect z nedůvěryhodných zdrojů pomocí verzí převaděče WordPad nebo aplikace Microsoft Office Word, které obsahují tuto chybu.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritický</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows, Microsoft Office</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=139852">MS09-013</a></td>
<td style="border:1px solid black;"><strong>Chyby zabezpečení služby Windows HTTP Services umožňují vzdálené spuštění kódu (960803)</strong><br />
<br />
Tato aktualizace zabezpečení řeší jednu veřejně známou a dvě soukromými osobami oznámené chyby zabezpečení ve službě Microsoft Windows HTTP Services (WinHTTP). Nejzávažnější chyba zabezpečení by mohla umožnit vzdálené spuštění kódu. Útočník, který by tuto chybu zabezpečení zneužil, by mohl získat úplnou kontrolu nad postiženým systémem. Útočník by tak mohl instalovat programy, zobrazovat, měnit či odstraňovat data nebo vytvářet nové účty s úplnými uživatelskými právy. Uživatelé, jejichž účty jsou konfigurovány tak, aby měli v systému méně uživatelských práv, by byli vystaveni menšímu riziku než uživatelé s uživatelskými právy správce.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritický</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=139107">MS09-011</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení v rozhraní Microsoft DirectShow umožňuje vzdálené spuštění kódu (961373)</strong><br />
<br />
Tato aktualizace zabezpečení řeší chybu zabezpečení v rozhraní Microsoft DirectX, kterou oznámila soukromá osoba. Tato chyba zabezpečení umožňuje vzdálené spuštění kódu, pokud uživatel otevře speciálně vytvořený soubor MJPEG. Útočník, který by tuto chybu zabezpečení zneužil, by mohl získat úplnou kontrolu nad postiženým systémem. Útočník by tak mohl instalovat programy, zobrazovat, měnit či odstraňovat data nebo vytvářet nové účty s úplnými uživatelskými právy. Uživatelé, jejichž účty jsou konfigurovány tak, aby měli v systému méně uživatelských práv, by byli vystaveni menšímu riziku než uživatelé s uživatelskými právy správce.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritický</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Může vyžadovat restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=146659">MS09-014</a></td>
<td style="border:1px solid black;"><strong>Kumulativní aktualizace zabezpečení pro aplikaci Internet Explorer (963027)</strong><br />
<br />
Tato aktualizace zabezpečení řeší čtyři chyby zabezpečení oznámené soukromými osobami a dvě veřejně známé chyby zabezpečení v aplikaci Internet Explorer. Tyto chyby zabezpečení mohou umožňovat vzdálené spuštění kódu, pokud uživatel pomocí aplikace Internet Explorer zobrazí speciálně vytvořenou webovou stránku nebo pokud se připojí k serveru útočníka prostřednictvím protokolu HTTP. Uživatelé, jejichž účty jsou konfigurovány tak, aby měli v systému méně uživatelských práv, by byli vystaveni menšímu riziku než uživatelé s uživatelskými právy správce.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritický</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows, Internet Explorer</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=143568">MS09-009</a></td>
<td style="border:1px solid black;"><strong>Chyby zabezpečení v aplikaci Microsoft Office Excel umožňují vzdálené spuštění kódu (968557)</strong><br />
<br />
Tato aktualizace zabezpečení řeší jednu chybu zabezpečení oznámenou soukromou osobou a jednu veřejně známou chybu zabezpečení aplikace Microsoft Office Excel. Tyto chyby zabezpečení umožňují vzdálené spuštění kódu, pokud uživatel otevře speciálně vytvořený soubor aplikace Excel. Útočník, který by tyto chyby zabezpečení zneužil, by mohl získat úplnou kontrolu nad postiženým systémem. Útočník by tak mohl instalovat programy, zobrazovat, měnit či odstraňovat data nebo vytvářet nové účty s úplnými uživatelskými právy. Uživatelé, jejichž účty jsou konfigurovány tak, aby měli v systému méně uživatelských práv, by byli vystaveni menšímu riziku než uživatelé s uživatelskými právy správce.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritický</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Může vyžadovat restartování</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=132587">MS09-012</a></td>
<td style="border:1px solid black;"><strong>Chyby zabezpečení systému Windows umožňují zvýšení úrovně oprávnění (959454)</strong><br />
<br />
Tato aktualizace zabezpečení řeší čtyři veřejně známé chyby zabezpečení v systému Microsoft Windows. Chyby zabezpečení by mohly vést ke zvýšení úrovně oprávnění, pokud by se útočník směl přihlásit k systému a následně spustil speciálně vytvořenou aplikaci. Útočník by musel mít možnost spustit kód v místním počítači, aby mohl zneužít tuto chybu zabezpečení. Útočník, který by úspěšně zneužil některou z těchto chyb zabezpečení, by mohl převzít úplnou kontrolu nad postiženým systémem.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Důležité</a><br />
Zvýšení úrovně oprávnění</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=141639">MS09-016</a></td>
<td style="border:1px solid black;"><strong>Chyby zabezpečení serveru Microsoft ISA Server a brány Forefront Threat Management Gateway (Medium Business Edition) mohou způsobit odmítnutí služby (961759)</strong><br />
<br />
Tato aktualizace zabezpečení řeší jednu chybu zabezpečení oznámenou soukromou osobou a jednu veřejně známou chybu zabezpečení na serveru Microsoft ISA (Internet Security and Acceleration) Server a v bráně Microsoft Forefront Threat Management Gateway (TMG), Medium Business Edition (MBE). Tyto chyby zabezpečení by mohly způsobit odmítnutí služby v případě, že by útočník do postiženého systému odeslal speciálně vytvořené síťové pakety, nebo přístup k informacím v případě, že by uživatel kliknul na škodlivou adresu URL nebo navštívil web s obsahem řízeným útočníkem.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Důležité</a><br />
Odmítnutí služby</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Forefront Edge Security</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=146803">MS09-015</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení se smíšeným ohrožením ve funkci SearchPath umožňuje zvýšení úrovně oprávnění (959426)</strong><br />
<br />
Tato aktualizace zabezpečení řeší jednu veřejně známou chybu zabezpečení ve funkci Windows SearchPath, která by mohla umožnit zvýšení úrovně oprávnění, pokud by si uživatel stáhnul speciálně vytvořený soubor do konkrétního umístění a potom za určitých okolností spustil aplikaci, která by tento soubor mohla načíst.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Mírný</a><br />
Zvýšení úrovně oprávnění</td>
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
  
| ID bulletinu                                              | Název bulletinu                                                                                                                                               | ID CVE                                                                               | Hodnocení indexu zneužitelnosti                                                                                                | Hlavní poznámky                                                                                                                                                                                                                                     |  
|-----------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| [MS09-009](http://go.microsoft.com/fwlink/?linkid=143568) | Chyby zabezpečení v aplikaci Microsoft Office Excel umožňují vzdálené spuštění kódu (968557)                                                                  | [CVE-2009-0100](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0100)     | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Nekonsistentní kód zneužití je pravděpodobný              | (Žádné)                                                                                                                                                                                                                                             |  
| [MS09-009](http://go.microsoft.com/fwlink/?linkid=143568) | Chyby zabezpečení v aplikaci Microsoft Office Excel umožňují vzdálené spuštění kódu (968557)                                                                  | [CVE-2009-0238](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0238)     | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní kód zneužití je pravděpodobný                | **V současné době dochází ke zneužití této chyby zabezpečení v prostředí Internetu.**                                                                                                                                                               |  
| [MS09-010](http://go.microsoft.com/fwlink/?linkid=139849) | Chyby zabezpečení v převaděči WordPad a převaděčích textu systému Office umožňují vzdálené spuštění kódu (960477)                                             | [CVE-2008-4841](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-4841)     | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní kód zneužití je pravděpodobný                | **V současné době dochází ke zneužití této chyby zabezpečení v prostředí Internetu.**                                                                                                                                                               |  
| [MS09-010](http://go.microsoft.com/fwlink/?linkid=139849) | Chyby zabezpečení v převaděči WordPad a převaděčích textu systému Office umožňují vzdálené spuštění kódu (960477)                                             | [CVE-2009-0087](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0087)     | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Nekonsistentní kód zneužití je pravděpodobný              | Jedná se o komplexní chybu zabezpečení způsobenou různými cestami kódu. U většiny kódů zneužití budou zaznamenány nekonsistentní výsledky. Výchozí faktory snižující závažnost rizika tomuto jevu zabraňují.                                        |  
| [MS09-010](http://go.microsoft.com/fwlink/?linkid=139849) | Chyby zabezpečení v převaděči WordPad a převaděčích textu systému Office umožňují vzdálené spuštění kódu (960477)                                             | [CVE-2009-0088](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0088)     | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní kód zneužití je pravděpodobný                | Tato chyba zabezpečení je zneužitelná, postihuje však pouze starší verze a starší, méně obvyklý formát souborů. Novější verze, například systém Microsoft Office 2007 či Microsoft Office 2003 Service Pack 3, nejsou touto chybou postiženy.       |  
| [MS09-010](http://go.microsoft.com/fwlink/?linkid=139849) | Chyby zabezpečení v převaděči WordPad a převaděčích textu systému Office umožňují vzdálené spuštění kódu (960477)                                             | [CVE-2009-0235](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0235)     | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní kód zneužití je pravděpodobný                | Tuto chybu zabezpečení týkající se poškození paměti lze snadno zneužít.                                                                                                                                                                             |  
| [MS09-011](http://go.microsoft.com/fwlink/?linkid=139107) | Chyba zabezpečení v rozhraní Microsoft DirectShow umožňuje vzdálené spuštění kódu (961373)                                                                    | [CVE-2009-0084](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0084)     | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Nekonsistentní kód zneužití je pravděpodobný              | (Žádné)                                                                                                                                                                                                                                             |  
| [MS09-012](http://go.microsoft.com/fwlink/?linkid=132587) | Chyby zabezpečení systému Windows umožňují zvýšení úrovně oprávnění (959454)                                                                                  | [CVE-2008-1436](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-1436)     | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní kód zneužití je pravděpodobný                | **V současné době dochází ke zneužití této chyby zabezpečení v prostředí Internetu.**                                                                                                                                                               |  
| [MS09-012](http://go.microsoft.com/fwlink/?linkid=132587) | Chyby zabezpečení systému Windows umožňují zvýšení úrovně oprávnění (959454)                                                                                  | [CVE-2009-0078](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0078)     | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní kód zneužití je pravděpodobný                | **V současné době dochází ke zneužití této chyby zabezpečení v prostředí Internetu.**                                                                                                                                                               |  
| [MS09-012](http://go.microsoft.com/fwlink/?linkid=132587) | Chyby zabezpečení systému Windows umožňují zvýšení úrovně oprávnění (959454)                                                                                  | [CVE-2009-0079](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0079)     | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní kód zneužití je pravděpodobný                | **V současné době dochází ke zneužití této chyby zabezpečení v prostředí Internetu.**                                                                                                                                                               |  
| [MS09-012](http://go.microsoft.com/fwlink/?linkid=132587) | Chyby zabezpečení systému Windows umožňují zvýšení úrovně oprávnění (959454)                                                                                  | [CVE-2009-0080](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0080)     | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní kód zneužití je pravděpodobný                | **V současné době dochází ke zneužití této chyby zabezpečení v prostředí Internetu.**                                                                                                                                                               |  
| [MS09-013](http://go.microsoft.com/fwlink/?linkid=139852) | Chyby zabezpečení služby Windows HTTP Services umožňují vzdálené spuštění kódu (960803)                                                                       | [CVE-2009-0086](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0086)     | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní kód zneužití je pravděpodobný                | Jedná se o chybu zabezpečení paměti, kterou lze z důvodu rozšířeného použití této technologie snadno zneužít, k čemuž slouží množství různých způsobů útoku a příležitostí k zneužití.                                                              |  
| [MS09-013](http://go.microsoft.com/fwlink/?linkid=139852) | Chyby zabezpečení služby Windows HTTP Services umožňují vzdálené spuštění kódu (960803)                                                                       | [CVE-2009-0089](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0089)     | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní kód zneužití je pravděpodobný                | (Žádné)                                                                                                                                                                                                                                             |  
| [MS09-013](http://go.microsoft.com/fwlink/?linkid=139852) | Chyby zabezpečení služby Windows HTTP Services umožňují vzdálené spuštění kódu (960803)                                                                       | [CVE-2009-0550](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0550)\*\* | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní kód zneužití je pravděpodobný                | Byl zveřejněn kód zneužití.                                                                                                                                                                                                                         |  
| [MS09-014](http://go.microsoft.com/fwlink/?linkid=146659) | Kumulativní aktualizace zabezpečení pro aplikaci Internet Explorer (963027)                                                                                   | [CVE-2008-2540](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-2540)\*   | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Vytvoření funkčního zneužitelného kódu není pravděpodobné | Byly zveřejněny podrobnosti o útoku, nicméně v současné době neexistují žádné známé formy útoku. Zneužití této chyby je možné tehdy, pokud útočník i uživatel provedou řadu složitých kroků, mezi něž patří uložení určitých souborů do počítače.   |  
| [MS09-014](http://go.microsoft.com/fwlink/?linkid=146659) | Kumulativní aktualizace zabezpečení pro aplikaci Internet Explorer (963027)                                                                                   | [CVE-2009-0550](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0550)\*\* | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní kód zneužití je pravděpodobný                | Byl zveřejněn kód zneužití.                                                                                                                                                                                                                         |  
| [MS09-014](http://go.microsoft.com/fwlink/?linkid=146659) | Kumulativní aktualizace zabezpečení pro aplikaci Internet Explorer (963027)                                                                                   | [CVE-2009-0551](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0551)     | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Nekonsistentní kód zneužití je pravděpodobný              | (Žádné)                                                                                                                                                                                                                                             |  
| [MS09-014](http://go.microsoft.com/fwlink/?linkid=146659) | Kumulativní aktualizace zabezpečení pro aplikaci Internet Explorer (963027)                                                                                   | [CVE-2009-0552](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0552)     | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Vytvoření funkčního zneužitelného kódu není pravděpodobné | Skutečnosti snižující závažnost rizika pro aplikaci Internet Explorer 7 zabraňují spuštění kódu. Větší pravděpodobnost zneužití je u aplikace Internet Explorer 6 a starších verzí, nejsou-li pravidelně udržovány všemi aktualizacemi zabezpečení. |  
| [MS09-014](http://go.microsoft.com/fwlink/?linkid=146659) | Kumulativní aktualizace zabezpečení pro aplikaci Internet Explorer (963027)                                                                                   | [CVE-2009-0553](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0553)     | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Vytvoření funkčního zneužitelného kódu není pravděpodobné | (Žádné)                                                                                                                                                                                                                                             |  
| [MS09-014](http://go.microsoft.com/fwlink/?linkid=146659) | Kumulativní aktualizace zabezpečení pro aplikaci Internet Explorer (963027)                                                                                   | [CVE-2009-0554](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0554)     | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní kód zneužití je pravděpodobný                | (Žádné)                                                                                                                                                                                                                                             |  
| [MS09-015](http://go.microsoft.com/fwlink/?linkid=146803) | Chyba zabezpečení se smíšeným ohrožením ve funkci SearchPath umožňuje zvýšení úrovně oprávnění (959426)                                                       | [CVE-2008-2540](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-2540)\*   | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Nekonsistentní kód zneužití je pravděpodobný              | Byly zveřejněny podrobnosti o útoku, nicméně v současné době neexistují žádné známé formy útoku. Zneužití této chyby je možné tehdy, pokud útočník i uživatel provedou řadu složitých kroků, mezi něž patří uložení určitých souborů do počítače.   |  
| [MS09-016](http://go.microsoft.com/fwlink/?linkid=141639) | Chyby zabezpečení serveru Microsoft ISA Server a brány Forefront Threat Management Gateway (Medium Business Edition) mohou způsobit odmítnutí služby (961759) | [CVE-2009-0077](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0077)     | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Vytvoření funkčního zneužitelného kódu není pravděpodobné | S velkou pravděpodobností dojde k odmítnutí služby. Přesto však nelze spustit kód.                                                                                                                                                                  |  
| [MS09-016](http://go.microsoft.com/fwlink/?linkid=141639) | Chyby zabezpečení serveru Microsoft ISA Server a brány Forefront Threat Management Gateway (Medium Business Edition) mohou způsobit odmítnutí služby (961759) | [CVE-2009-0237](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-0237)          | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Vytvoření funkčního zneužitelného kódu není pravděpodobné | Je umožněn přístup k informacím. Spuštění kódu je velice nepravděpodobné.                                                                                                                                                                           |
  
\*Tuto dvojici chyb zabezpečení, jimž je přiřazeno stejné číslo CVE, řeší dvě aktualizace zabezpečení. Další informace naleznete v příslušných bulletinech.
  
\*\*Tuto dvojici chyb zabezpečení, jimž je přiřazeno stejné číslo CVE, řeší dvě aktualizace zabezpečení. Další informace naleznete v příslušných bulletinech.
  
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
</tr>
<tr>
<th colspan="7" style="border:1px solid black;">
Microsoft Windows 2000  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS09-010**](http://go.microsoft.com/fwlink/?linkid=139849)
</td>
<td style="border:1px solid black;">
[**MS09-013**](http://go.microsoft.com/fwlink/?linkid=139852)
</td>
<td style="border:1px solid black;">
[**MS09-011**](http://go.microsoft.com/fwlink/?linkid=139107)
</td>
<td style="border:1px solid black;">
[**MS09-014**](http://go.microsoft.com/fwlink/?linkid=146659)
</td>
<td style="border:1px solid black;">
[**MS09-012**](http://go.microsoft.com/fwlink/?linkid=132587)
</td>
<td style="border:1px solid black;">
[**MS09-015**](http://go.microsoft.com/fwlink/?linkid=146803)
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
[**Kritický**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
(Stupeň závažnosti není určen)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Windows 2000 Service Pack 4
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=552d322a-5282-42c7-9c1e-1d8c494a7318)  
(KB923561)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=39d5468e-5733-4c3e-9e75-3adac8ac8cb9)  
(Kritický)
</td>
<td style="border:1px solid black;">
[DirectX 8.1](http://www.microsoft.com/downloads/details.aspx?familyid=0ec5b7c7-13d3-467a-b24e-3cc6fb47adf6)  
(Kritický)  
[DirectX 9.0](http://www.microsoft.com/downloads/details.aspx?familyid=8b98ed5c-a3ab-45a7-a61e-349eae304bc6)\*\*\*  
(Kritický)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 5.01 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=7799fd05-5b26-449f-8a14-50227c9164d1)  
(Kritický)  
[Microsoft Internet Explorer 6 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=87f0c380-5c31-4099-a6a9-c12f9d69b03b)  
(Kritický)
</td>
<td style="border:1px solid black;">
Aktualizace nástroje pro koordinaci transakcí MSDTC:  
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=52b756e7-636f-4d9e-8a17-dbf467bfbe4d)  
(KB952004)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=c4e408d7-6716-4a12-ad3a-8029667f5c84)  
(Stupeň závažnosti není určen)
</td>
</tr>
<tr>
<th colspan="7" style="border:1px solid black;">
Windows XP
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS09-010**](http://go.microsoft.com/fwlink/?linkid=139849)
</td>
<td style="border:1px solid black;">
[**MS09-013**](http://go.microsoft.com/fwlink/?linkid=139852)
</td>
<td style="border:1px solid black;">
[**MS09-011**](http://go.microsoft.com/fwlink/?linkid=139107)
</td>
<td style="border:1px solid black;">
[**MS09-014**](http://go.microsoft.com/fwlink/?linkid=146659)
</td>
<td style="border:1px solid black;">
[**MS09-012**](http://go.microsoft.com/fwlink/?linkid=132587)
</td>
<td style="border:1px solid black;">
[**MS09-015**](http://go.microsoft.com/fwlink/?linkid=146803)
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
[**Kritický**](http://go.microsoft.com/fwlink/?linkid=21140)
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
[Windows XP Service Pack 2 a Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=50a8519a-503e-43dd-a78a-c1bc764fd213)  
(KB923561)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 a Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=35af4151-1858-4c9a-85e4-9ff45feca1a4)  
(Kritický)
</td>
<td style="border:1px solid black;">
[DirectX 9.0](http://www.microsoft.com/downloads/details.aspx?familyid=feb5d821-f210-40e8-b1aa-2ca3170df8df)\*\*\*  
(Kritický)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=052c29fc-e8df-402c-9ab1-1079bc738e1b)  
(Kritický)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=55d6729a-9f96-4da4-b564-676c0a0c9390)  
(Kritický)
</td>
<td style="border:1px solid black;">
Aktualizace nástroje pro koordinaci transakcí MSDTC:  
[Windows XP Service Pack 2 a Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=90fe715e-8190-43e9-9c43-df5be564d923)  
(KB952004)  
(Důležitý)  
Aktualizace izolace služeb systému Windows:  
[Windows XP Service Pack 2 a Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=73d2324f-be59-4b0c-b1ac-9876a13c2c03)  
(KB956572)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 a Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=3de0684d-605c-489b-bdc7-08bce9b2d4f6)  
(Mírný)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Professional x64 Edition a Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition a Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=323f4211-5add-4e02-bce1-e5a1b489982c)  
(KB923561)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition a Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=49b16f0f-f6c3-4ca8-8041-392f4f7b5bbb)  
(Kritický)
</td>
<td style="border:1px solid black;">
[DirectX 9.0](http://www.microsoft.com/downloads/details.aspx?familyid=f1be8b7c-4874-4342-99b3-76ff725fbb9a)\*\*\*  
(Kritický)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=84c62211-2e82-4ccc-9f9b-26462b026d86)  
(Kritický)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=191c2f20-89ae-4e1c-bdd4-24b4abfe6b6c)  
(Kritický)
</td>
<td style="border:1px solid black;">
Aktualizace nástroje pro koordinaci transakcí MSDTC:  
[Windows XP Professional x64 Edition a Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=a794c32a-9a0c-47d9-9c57-ff5d4a8e4944)  
(KB952004)  
(Důležitý)  
Aktualizace izolace služeb systému Windows:  
[Windows XP Professional x64 Edition a Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b2f12ae5-0e46-47e1-ac5b-93550d030189)  
(KB956572)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition a Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b743a7fe-7bf4-420d-a72e-39471e5659fa)  
(Mírný)
</td>
</tr>
<tr>
<th colspan="7" style="border:1px solid black;">
Windows Server 2003
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS09-010**](http://go.microsoft.com/fwlink/?linkid=139849)
</td>
<td style="border:1px solid black;">
[**MS09-013**](http://go.microsoft.com/fwlink/?linkid=139852)
</td>
<td style="border:1px solid black;">
[**MS09-011**](http://go.microsoft.com/fwlink/?linkid=139107)
</td>
<td style="border:1px solid black;">
[**MS09-014**](http://go.microsoft.com/fwlink/?linkid=146659)
</td>
<td style="border:1px solid black;">
[**MS09-012**](http://go.microsoft.com/fwlink/?linkid=132587)
</td>
<td style="border:1px solid black;">
[**MS09-015**](http://go.microsoft.com/fwlink/?linkid=146803)
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
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Mírný**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 1 a Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 1 a Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2233a4d2-7c8a-4c89-b020-100d9afb43c8)  
(KB923561)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 1 a Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=42509f5a-d0f9-444a-9445-5eabdb555011)  
(Kritický)
</td>
<td style="border:1px solid black;">
[DirectX 9.0](http://www.microsoft.com/downloads/details.aspx?familyid=c1b4cd76-1dd6-43fa-bb9a-20c428985bfd)\*\*\*  
(Kritický)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=f73a3669-c17f-4b18-8456-96cb7d52ed86)  
(Důležitý)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=6a45dbd0-0520-4d9b-b76e-3f5109dd310d)  
(Důležitý)
</td>
<td style="border:1px solid black;">
Aktualizace nástroje pro koordinaci transakcí MSDTC:  
[Windows Server 2003 Service Pack 1 a Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=25adec10-db8c-4cac-bf74-2c784678150a)  
(KB952004)  
(Důležitý)  
Aktualizace izolace služeb systému Windows:  
[Windows Server 2003 Service Pack 1 a Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=42aba890-8b76-4c5a-8fb6-609797d19831)  
(KB956572)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 1 a Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=992bb0cd-fbc7-4a7c-9088-f7f9d9a3ead0)  
(Mírný)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition a Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition a Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=323f4211-5add-4e02-bce1-e5a1b489982c)  
(KB923561)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition a Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7373ea32-bc2e-49f1-8b9f-4eeda5acc74c)  
(Kritický)
</td>
<td style="border:1px solid black;">
[DirectX 9.0](http://www.microsoft.com/downloads/details.aspx?familyid=f0e1e1db-94a5-451c-ab11-6b431fa065f1)\*\*\*  
(Kritický)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=03a9d581-2bd5-4151-9826-17b96e16f606)  
(Důležitý)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=60ccc1d6-ea31-420c-b630-d7878a8dc527)  
(Důležitý)
</td>
<td style="border:1px solid black;">
Aktualizace nástroje pro koordinaci transakcí MSDTC:  
[Windows Server 2003 x64 Edition and Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b014c399-f404-4cb2-8f9d-864df382efeb)  
(KB952004)  
(Důležitý)  
Aktualizace izolace služeb systému Windows:  
[Windows Server 2003 x64 Edition and Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=a0609f65-82d9-4d82-9f48-f3266e8de123)  
(KB956572)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition a Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=f0a58e8c-7d63-4d7d-ba95-b3787cf408f0)  
(Mírný)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 SP1 pro systémy s procesorem Itanium a Windows Server 2003 SP2 pro systémy s procesorem Itanium
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP1 pro systémy s procesorem Itanium a Windows Server 2003 SP2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=e840b9cb-f1f4-482a-aa07-eb6b42b477c4)  
(KB923561)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP1 pro systémy s procesorem Itanium a Windows Server 2003 SP2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=05e33cc5-cff6-4c71-be71-285f66a95e01)  
(Kritický)
</td>
<td style="border:1px solid black;">
[DirectX 9.0](http://www.microsoft.com/downloads/details.aspx?familyid=8f36c215-fa8a-40c2-b680-6b1fece03b8d)\*\*\*  
(Kritický)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=53d13c07-80b0-4f05-b372-a2dac17e6157)  
(Důležitý)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=0abaa2fb-7c4f-4149-993d-1575888bfc84)  
(Důležitý)
</td>
<td style="border:1px solid black;">
Aktualizace nástroje pro koordinaci transakcí MSDTC:  
[Windows Server 2003 SP1 pro systémy s procesorem Itanium a Windows Server 2003 SP2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=6ada372b-ba17-433e-b022-d2c57b35af8a)  
(KB952004)  
(Důležitý)  
Aktualizace izolace služeb systému Windows:  
[Windows Server 2003 SP1 pro systémy s procesorem Itanium a Windows Server 2003 SP2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=fda8837c-e5d2-4489-9b44-4c24a1102e77)  
(KB956572)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP1 pro systémy s procesorem Itanium a Windows Server 2003 SP2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=00c6479d-f81f-445d-b8e4-7b71d77d540a)  
(Mírný)
</td>
</tr>
<tr>
<th colspan="7" style="border:1px solid black;">
Windows Vista
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS09-010**](http://go.microsoft.com/fwlink/?linkid=139849)
</td>
<td style="border:1px solid black;">
[**MS09-013**](http://go.microsoft.com/fwlink/?linkid=139852)
</td>
<td style="border:1px solid black;">
[**MS09-011**](http://go.microsoft.com/fwlink/?linkid=139107)
</td>
<td style="border:1px solid black;">
[**MS09-014**](http://go.microsoft.com/fwlink/?linkid=146659)
</td>
<td style="border:1px solid black;">
[**MS09-012**](http://go.microsoft.com/fwlink/?linkid=132587)
</td>
<td style="border:1px solid black;">
[**MS09-015**](http://go.microsoft.com/fwlink/?linkid=146803)
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
Žádné
</td>
<td style="border:1px solid black;">
[**Kritický**](http://go.microsoft.com/fwlink/?linkid=21140)
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
Windows Vista a Windows Vista Service Pack 1
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Vista a Windows Vista Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=f071d770-3b6b-4040-9911-d4de8cde4c68)  
(Kritický)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=d743849d-f3b5-4114-adef-ade2716d55ac)  
(Kritický)
</td>
<td style="border:1px solid black;">
Aktualizace nástroje pro koordinaci transakcí MSDTC:  
[Windows Vista a Windows Vista Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=f111b99a-e555-4f29-8d1f-e9ec03d5cf1f)  
(KB952004)  
(Důležitý)  
Aktualizace izolace služeb systému Windows:  
[Windows Vista a Windows Vista Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=d0ea1598-45cb-4c79-8945-caae98969675)  
(KB956572)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Windows Vista a Windows Vista Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=2b672d45-f33b-4edc-9f22-2f2c8c726a8b)  
(Mírný)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista x64 Edition a Windows Vista x64 Edition Service Pack 1
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition a Windows Vista x64 Edition Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=7ceef2d0-f316-48d1-aecc-d74f91cc5e1f)  
(Kritický)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=d191c8dc-a965-4a6a-b6d8-1470505eb55f)  
(Kritický)
</td>
<td style="border:1px solid black;">
Aktualizace nástroje pro koordinaci transakcí MSDTC:  
[Windows Vista x64 Edition a Windows Vista x64 Edition Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=fa153bdc-6b48-4df2-9e5e-abacd6da782c)  
(KB952004)  
(Důležitý)  
Aktualizace izolace služeb systému Windows:  
[Windows Vista x64 Edition a Windows Vista x64 Edition Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=6dd82f4b-bb33-41ec-90a7-9ef91329b240)  
(KB956572)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition a Windows Vista x64 Edition Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=7576e7d5-5bb1-4a53-b568-1ee0500ce721)  
(Mírný)
</td>
</tr>
<tr>
<th colspan="7" style="border:1px solid black;">
Windows Server 2008
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS09-010**](http://go.microsoft.com/fwlink/?linkid=139849)
</td>
<td style="border:1px solid black;">
[**MS09-013**](http://go.microsoft.com/fwlink/?linkid=139852)
</td>
<td style="border:1px solid black;">
[**MS09-011**](http://go.microsoft.com/fwlink/?linkid=139107)
</td>
<td style="border:1px solid black;">
[**MS09-014**](http://go.microsoft.com/fwlink/?linkid=146659)
</td>
<td style="border:1px solid black;">
[**MS09-012**](http://go.microsoft.com/fwlink/?linkid=132587)
</td>
<td style="border:1px solid black;">
[**MS09-015**](http://go.microsoft.com/fwlink/?linkid=146803)
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
Žádné
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
Windows Server 2008 pro 32bitové systémy
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro 32bitové systémy](http://www.microsoft.com/downloads/details.aspx?familyid=4c36548f-c8c9-4318-91e2-9e0501339548)\*  
(Kritický)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=e2c6313c-3ba9-4f7c-b259-b4582a390146)\*\*  
(Důležitý)
</td>
<td style="border:1px solid black;">
Aktualizace nástroje pro koordinaci transakcí MSDTC:  
[Windows Server 2008 pro 32bitové systémy](http://www.microsoft.com/downloads/details.aspx?familyid=9e3c7b52-65a7-42fb-beb5-1b374934737f)\*  
(KB952004)  
(Důležitý)  
Aktualizace izolace služeb systému Windows:  
[Windows Server 2008 pro 32bitové systémy](http://www.microsoft.com/downloads/details.aspx?familyid=d58702af-bbf8-4f1b-ae72-ced9ef23d581)\*  
(KB956572)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro 32bitové systémy](http://www.microsoft.com/downloads/details.aspx?familyid=6b73cf5e-66fe-4b7d-95fc-91a1c262c1e5)\*  
(Mírný)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 pro systémy s procesorem x64
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem x64](http://www.microsoft.com/downloads/details.aspx?familyid=1c3f0997-a8a9-4340-ae0c-2c4d6792c65c)\*  
(Kritický)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=ebbade9d-704c-440b-8796-6d64225ac01a)\*\*  
(Důležitý)
</td>
<td style="border:1px solid black;">
Aktualizace nástroje pro koordinaci transakcí MSDTC:  
[Windows Server 2008 pro systémy s procesorem x64](http://www.microsoft.com/downloads/details.aspx?familyid=eebb4d4d-29d2-4247-8cbb-63a3b17585ec)\*  
(KB952004)  
(Důležitý)  
Aktualizace izolace služeb systému Windows:  
[Windows Server 2008 pro systémy s procesorem x64](http://www.microsoft.com/downloads/details.aspx?familyid=20bf4e9b-909b-4bc3-ae43-322d74a4f1c3)\*  
(KB956572)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem x64](http://www.microsoft.com/downloads/details.aspx?familyid=7e60847c-b341-4c38-bc25-2e3cf2d4ae14)\*  
(Mírný)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 pro systémy s procesorem Itanium
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=0885b3b0-b78e-4980-902d-dff3886bcaac)  
(Kritický)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=1b04aa6f-b787-4122-bf82-0d150618fe7a)  
(Důležitý)
</td>
<td style="border:1px solid black;">
Aktualizace nástroje pro koordinaci transakcí MSDTC:  
[Windows Server 2008 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=cc383c24-b0f6-47c1-9e89-6a378b09e82f)  
(KB952004)  
(Důležitý)  
Aktualizace izolace služeb systému Windows:  
[Windows Server 2008 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=bcc2b18f-67db-4109-a9f4-764f985423ee)  
(KB956572)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=de1c2b4b-af47-4b9a-8363-720e5527573c)  
(Mírný)
</td>
</tr>
</table>
<p></p>
 
**Poznámky k systému Windows Server 2008**

**\*Instalace Server Core operačního systému Windows Server 2008 obsahující tuto chybu.** Tato aktualizace se týká všech podporovaných vydání systému Windows Server 2008 se stejným stupněm závažnosti, ať už byl systém Windows Server 2008 instalován pomocí možnosti instalace Server Core či nikoli. Více informací o této možnosti instalace naleznete v části [Server Core](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx). Možnost instalace Server Core se nevztahuje na určité edice systému Windows Server 2008. Další informace naleznete v části [Porovnání možností instalace Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**\*\*Instalace Server Core operačního systému Windows Server 2008 neobsahující tuto chybu.** Chyby zabezpečení, které tato aktualizace řeší, nemají vliv na podporované edice systému Windows Server 2008, jestliže byl systém Windows Server 2008 instalován s využitím možnosti instalace Server Core. Více informací o této možnosti instalace naleznete v části [Server Core](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx). Možnost instalace Server Core se nevztahuje na určité edice systému Windows Server 2008. Další informace naleznete v části [Porovnání možností instalace Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**Poznámka k bulletinu MS09-010**

Další soubory aktualizace naleznete také v části **Sady Microsoft Office a jejich software**. Tento bulletin pokrývá operační systém Windows a jeho součásti i systémy Microsoft Office a příslušný software.

**Poznámka k bulletinu MS09-011**

\*\*\*Aktualizace rozhraní DirectX 9.0 se týká rovněž verzí DirectX 9.0a, DirectX 9.0b a DirectX 9.0c.

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
[**MS09-010**](http://go.microsoft.com/fwlink/?linkid=139849)
</td>
<td style="border:1px solid black;">
[**MS09-009**](http://go.microsoft.com/fwlink/?linkid=143568)
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
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2000 Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Office Word 2000 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=95876927-e612-414c-bdec-3632a3100415)  
(KB921606)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel 2000 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=3dc8b670-25a5-4f46-b7de-12bc693b628a)  
(KB959964)  
(Kritický)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Office Word 2002 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=e1db55c6-78fb-498d-89a5-9ad54d971546)  
(KB933399)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel 2002 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=9a52bf4b-05f6-4b73-94b9-28ed7e20f86c)  
(KB959988)  
(Důležitý)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2003 Service Pack 3
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=d9dbfa63-c0cb-4c84-9b8a-6e52568045b0)  
(KB959995)  
(Důležitý)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Systém Microsoft Office 2007 Service Pack 1
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel 2007 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=50d8630b-1365-4007-81a0-18c0d6d4b86e)\*  
(KB959997)  
(Důležitý)
</td>
</tr>
<tr>
<th colspan="3" style="border:1px solid black;">
Microsoft Office for Mac
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS09-010**](http://go.microsoft.com/fwlink/?linkid=139849)
</td>
<td style="border:1px solid black;">
[**MS09-009**](http://go.microsoft.com/fwlink/?linkid=143568)
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
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2004 for Mac
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Microsoft Office 2004 for Mac](http://www.microsoft.com/downloads/details.aspx?familyid=52271140-89be-4b9c-baa2-cea09097d703)  
(KB968695)  
(Důležitý)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2008 for Mac
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Microsoft Office 2008 for Mac](http://www.microsoft.com/downloads/details.aspx?familyid=f6e407eb-11a5-433f-8006-4b822953ca98)  
(KB968694)  
(Důležitý)
</td>
</tr>
<tr>
<th colspan="3" style="border:1px solid black;">
Jiný software sady Office
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS09-010**](http://go.microsoft.com/fwlink/?linkid=139849)
</td>
<td style="border:1px solid black;">
[**MS09-009**](http://go.microsoft.com/fwlink/?linkid=143568)
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
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Excel Viewer
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel Viewer 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=c72e6087-b48f-4d2d-8366-01d9f5ff6b6c)  
(KB959993)  
(Důležitý)  
[Microsoft Office Excel Viewer](http://www.microsoft.com/downloads/details.aspx?familyid=58b3929c-5373-47a4-aa97-66d179758792)  
(KB960000)  
(Důležitý)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Sada Microsoft Office Compatibility Pack pro formáty souborů aplikací Word, Excel a PowerPoint 2007
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Sada Microsoft Office Compatibility Pack pro formáty souborů Word, Excel a PowerPoint 2007 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=05f7c517-e551-4dcd-b24a-5d548f2d09cf)  
(KB960003)  
(Důležitý)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Converter Pack
</td>
<td style="border:1px solid black;">
[Microsoft Office Converter Pack](http://www.microsoft.com/downloads/details.aspx?familyid=d763fae3-b2af-47f9-a554-ec786766b3c3)  
(KB960476)  
(Důležitý)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
</tr>
</table>
<p></p>
 
**Poznámka k bulletinu MS09-010**

Další soubory aktualizace naleznete také v části **Operační systém Windows a jeho součásti**. Tento bulletin pokrývá operační systém Windows a jeho součásti i Microsoft Server Software.

**Poznámka k bulletinu MS09-009**

\*Na ochranu před chybami zabezpečení popsanými v tomto bulletinu je u aplikace Microsoft Office Excel 2007 Service Pack 1 potřeba nainstalovat také aktualizaci zabezpečení pro sadu Microsoft Office Compatibility Pack pro formáty souborů aplikací Word, Excel a PowerPoint 2007 Service Pack 1.

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
Microsoft Forefront
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS09-016**](http://go.microsoft.com/fwlink/?linkid=141639)
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
Microsoft Forefront Threat Management Gateway
</td>
<td style="border:1px solid black;">
[Microsoft Forefront Threat Management Gateway, Medium Business Edition](http://www.microsoft.com/downloads/details.aspx?familyid=6abf9fb4-42d0-4c67-935f-8dc67850148b)\*  
(KB968075)  
(Důležitý)
</td>
</tr>
<tr>
<th colspan="2" style="border:1px solid black;">
Internet Security and Acceleration Server
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS09-016**](http://go.microsoft.com/fwlink/?linkid=141639)
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
Microsoft ISA (Internet Security and Acceleration) Server 2004
</td>
<td style="border:1px solid black;">
[Microsoft Internet Security and Acceleration Server 2004 Standard Edition Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=adf623fa-2d74-4f2a-9835-4b8debdb0e1b)\*\*  
(KB960995)  
(Důležitý)  
[Microsoft Internet Security and Acceleration Server 2004 Enterprise Edition Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=d1d55ab6-3de5-4811-9693-8d43f49f5fe8)  
(KB960995)  
(Důležitý)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Internet Security and Acceleration Server 2006
</td>
<td style="border:1px solid black;">
[Microsoft Internet Security and Acceleration Server 2006](http://www.microsoft.com/downloads/details.aspx?familyid=eda30bcc-0582-4f60-a4c5-ea5000b7c770)  
(KB968078)  
(Důležitý)  
[Microsoft Internet Security and Acceleration Server 2006 Supportability Update](http://www.microsoft.com/downloads/details.aspx?familyid=eda30bcc-0582-4f60-a4c5-ea5000b7c770)  
(KB968078)  
(Důležitý)  
[Microsoft Internet Security and Acceleration Server 2006 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=eda30bcc-0582-4f60-a4c5-ea5000b7c770)  
(KB968078)  
(Důležitý)
</td>
</tr>
</table>
<p></p>
 
**Poznámka k bulletinu MS09-016**

\*Brána Microsoft Forefront Threat Management Gateway, Medium Business Edition je k dispozici jako samostatný produkt i jako součást serveru Windows Essential Business Server 2008.

\*\*Microsoft ISA Server 2004 Standard Edition je k dispozici jako samostatný produkt. Microsoft ISA Server 2004 Standard Edition je také k dispozici jako součást serveru Windows Small Business Server 2003 Enterprise Edition Service Pack 1 a serveru Windows Small Business Server 2003 R2 Enterprise Edition.

Nástroje a doporučené postupy zjišťování a nasazení
---------------------------------------------------

 
**Centrum zabezpečení**

Umožňuje správu aktualizací softwaru a zabezpečení, které je třeba nainstalovat na servery, stolní počítače a přenosné počítače v organizaci. Další informace naleznete na webu [TechNet Update Management Center](http://go.microsoft.com/fwlink/?linkid=69903). Další informace o zabezpečení produktů společnosti Microsoft nabízí web [Centrum zabezpečení TechNet](http://go.microsoft.com/fwlink/?linkid=21171). Tyto informace lze také získat kliknutím na nabídku „Nejnovější aktualizace zabezpečení“ na webu [Zabezpečení doma](http://go.microsoft.com/fwlink/?linkid=85102).

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

**Nástroj Update Compatibility Evaluator a sada Application Compatibility Toolkit**

Aktualizace často zapisují do stejných souborů a nastavení registru požadovaných pro spouštění aplikací. To může způsobit nekompatibilitu a zvýšit dobu, po kterou trvá nasazení aktualizací zabezpečení. Testování a ověřování aktualizací systému Windows lze usnadnit pomocí součástí nástroje [Update Compatibility Evaluator](http://technet2.microsoft.com/windowsvista/en/library/4279e239-37a4-44aa-aec5-4e70fe39f9de1033.mspx?mfr=true), které jsou dodávány se sadou [Application Compatibility Toolkit 5.0](http://www.microsoft.com/downloads/details.aspx?familyid=24da89e9-b581-47b0-b45e-492dd6da2971&displaylang=en).

Sada Application Compatibility Toolkit (ACT) obsahuje nezbytné nástroje a dokumentaci pro posouzení a zmírnění problémů s kompatibilitou aplikací před nasazením systému Microsoft Windows Vista, služby Windows Update, aktualizací zabezpečení společnosti Microsoft nebo nové verze aplikace Windows Internet Explorer ve vašem prostředí.

### Další informace

#### Nástroj pro odstranění škodlivého softwaru systému Microsoft Windows

Společnost Microsoft vydává aktualizovanou verzi Nástroje pro odstranění škodlivého softwaru systému Microsoft Windows na webu Windows Update, Microsoft Update, ve službě Windows Server Update Services a na webu služby Stažení softwaru.

#### Důležité aktualizace nesouvisející se zabezpečením na webu Microsoft Update (MU), Windows Update (WU) a ve službě Windows Server Update Services (WSUS)

Informace o aktualizacích nesouvisejících se zabezpečením na webu Windows Update a Microsoft Update naleznete na webové stránce:

-   [Článek 894199 znalostní báze Microsoft Knowledge Base](http://support.microsoft.com/kb/894199): Popis služeb Software Update Services a Windows Server Update Services se mění v obsahu. Zahrnuje celý obsah systému Windows.
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
-   Aktualizace zabezpečení nabízené tento měsíc na webu Windows Update jsou k dispozici na webu služby Stažení softwaru v souborech obrazu ISO disku CD s vydanými aktualizacemi zabezpečení a kritickými aktualizacemi. Další informace získáte v [článku 913086 znalostní báze Microsoft Knowledge Base](http://support.microsoft.com/kb/913086).

**Komunita odborníků v oblasti zabezpečení**

Můžete se zde naučit, jak zlepšit zabezpečení a jak optimalizovat infrastrukturu IT. Také můžete s dalšími členy komunity IT Pro diskutovat o bezpečnostních tématech na webu [Komunita odborníků v oblasti zabezpečení (IT Pro Security Community)](http://go.microsoft.com/fwlink/?linkid=21164).

#### Poděkování

Společnost Microsoft tímto [děkuje](http://go.microsoft.com/fwlink/?linkid=21127) za spolupráci při ochraně zákazníků:

-   Haifei Liovi z týmu [FortiGuard Global Security Research Team](http://www.fortiguardcenter.com/) společnosti Fortinet za oznámení chyby popsané v bulletinu MS09-009.
-   Seanu Larssonovi a Junu Maovi ze společnosti [VeriSign iDefense Labs](http://labs.idefense.com/) za oznámení chyby popsané v bulletinu MS09-010.
-   Výzkumníkovi z týmu [FortiGuard Global Security Research Team](http://www.fortiguardcenter.com/) společnosti Fortinet za oznámení chyby popsané v bulletinu MS09-010.
-   Výzkumníkovi ze společnosti [VeriSign iDefense Labs](http://labs.idefense.com/) za oznámení chyby popsané v bulletinu MS09-010.
-   Piotru Baniovi ze společnosti [Kryptos Logic](http://www.kryptoslogic.com/) za oznámení chyby popsané v bulletinu MS09-011.
-   Cesaru Cerrudovi ze společnosti [Argeniss](http://www.argeniss.com/) za oznámení několika chyb popsaných v bulletinu MS09-012.
-   Gregu MacManusovi ze společnosti [iSIGHT Partners Labs](http://www.isightpartners.com/) za oznámení chyby popsané v bulletinu MS09-013.
-   Wan-Teh Changovi a Cemu Payovi ze společnosti [Google Inc.](http://www.google.com/) za oznámení chyby popsané v bulletinu MS09-013.
-   [Avivu Raffovi](http://aviv.raffon.net/) za oznámení chyby popsané v bulletinu MS09-014.
-   Michalu Zalewskému ze společnosti [Google Inc.](http://www.google.com/) za oznámení chyby popsané v bulletinu MS09-014.
-   Ivanu Fratricovi ze společnosti [iSIGHT Partners Labs](http://www.isightpartners.com/) za oznámení chyby popsané v bulletinu MS09-014.
-   Uživateli s pseudonymem Skylined ze společnosti [Google Inc.](http://www.google.com/) za oznámení chyby popsané v bulletinu MS09-014.
-   Divizi ADLab společnosti [VenusTech](http://www.venustech.com.cn/) za oznámení chyby popsané v bulletinu MS09-014.
-   [Avivu Raffovi](http://aviv.raffon.net/) za oznámení chyby popsané v bulletinu MS09-015.
-   Vedoucímu informatiky a celému technologickému oddělení na úřadu státu New York za oznámení chyby popsané v bulletinu MS09-016.

#### Technická podpora

-   Uvedený software byl testován za účelem zjištění, kterých verzí se chyba týká. U dalších verzí skončila časově omezená podpora. Pokud chcete zjistit dobu, po kterou je pro určitou verzi softwaru poskytována podpora, navštivte web [Zásady poskytování technické podpory pro produkty společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=21742).
-   Zákazníci mohou získat technickou podporu na webu [služby technické podpory společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=21131). Hovory související s aktualizacemi zabezpečení jsou bezplatné. Další informace o dostupných možnostech technické podpory naleznete na webu [Pomoc a podpora společnosti Microsoft](http://support.microsoft.com/).
-   Mezinárodní zákazníci získají podporu u místních zastoupení společnosti Microsoft. Technická podpora související s aktualizacemi zabezpečení je bezplatná. Další informace o možnostech kontaktování společnosti Microsoft v případě potřeby technické podpory získáte na [webu mezinárodní technické podpory](http://go.microsoft.com/fwlink/?linkid=21155).

#### Zřeknutí se záruky

Informace ve znalostní bázi Microsoft Knowledge Base jsou poskytovány tak, jak jsou, bez jakékoli záruky. Společnost Microsoft neposkytuje žádné záruky, výslovně uvedené či mlčky předpokládané, včetně záruk obchodovatelnosti a vhodnosti pro určitý účel. Společnost Microsoft ani její dodavatelé nenesou v žádném případě zodpovědnost za žádné škody, včetně přímých, nepřímých, náhodných či následných škod, ztráty zisku či zvláštních škod, a to ani v případě, že byli na možnost takových škod upozorněni. V některých zemích a právních řádech není dovoleno vyloučit nebo omezit odpovědnost, proto se výše uvedené omezení na vás nemusí vztahovat.

#### Revize

-   V1.0 (14. dubna 2009): Souhrnný bulletin byl publikován.
-   V1.1 (16. dubna 2009): Proběhla aktualizace indexu zneužitelnosti: byly odebrány hlavní poznámky pro chybu CVE-2009-0089 a změněny hlavní poznámky pro chybu CVE-2008-2540 v bulletinech zabezpečení MS09-014 a MS09-015.

*Built at 2014-04-18T01:50:00Z-07:00*
