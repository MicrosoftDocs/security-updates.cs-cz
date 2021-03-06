---
TOCTitle: 'MS09-DEC'
Title: 'Souhrnný bulletin zabezpečení společnosti Microsoft, prosinec 2009'
ms:assetid: 'ms09-dec'
ms:contentKeyID: 61223984
ms:mtpsurl: 'https://technet.microsoft.com/cs-CZ/library/ms09-dec(v=Security.10)'
---

 

Souhrnný bulletin zabezpečení společnosti Microsoft, prosinec 2009
==================================================================

Publikováno: 8. prosince 2009 | Aktualizováno: 13. ledna 2010

**Verze:** 2.0

Tento souhrnný bulletin uvádí bulletiny zabezpečení vydané v prosinci 2009.

Spolu s vydáním bulletinů pro prosinec 2009 nahrazuje tento souhrnný bulletin předběžné oznámení o bulletinech vydané 3. prosince 2009. Další informace o službě předběžného oznámení o bulletinech naleznete v části [Předběžné oznámení o bulletinech zabezpečení společnosti Microsoft](http://technet.microsoft.com/security/bulletin/advance).

Informace o tom, jak dostávat automatická oznámení o vydání nových bulletinů zabezpečení společnosti Microsoft, naleznete na webu [Zasílání technických oznámení o zabezpečení společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=21163).

Pro zodpovězení zákaznických dotazů týkajících se těchto bulletinů uspořádá společnost Microsoft webové vysílání 9. prosince 2009 v 11:00 časového pásma Tichomoří (USA a Kanada). [Registrovat se pro webové vysílání týkající se prosincových bulletinů zabezpečení](http://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032407802&culture=en-us). Po tomto datu je webové vysílání dostupné na požádání. Další informace získáte v [souhrnných bulletinech zabezpečení společnosti Microsoft a webovém vysílání](http://technet.microsoft.com/security/bulletin/summary).

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
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=177727">MS09-071</a></td>
<td style="border:1px solid black;"><strong>Chyby zabezpečení ve Službě ověřování v Internetu by mohly umožnit vzdálené spuštění kódu (974318)</strong><br />
<br />
Tato aktualizace zabezpečení řeší dvě soukromými osobami oznámené chyby zabezpečení v systému Microsoft Windows. Závažnější chyby zabezpečení mohou umožnit vzdálené spuštění kódu, pokud při zpracování pokusu o ověření protokolu PEAP dochází k nesprávnému kopírování zpráv, obdržených serverem používajícím Službu ověřování v Internetu, do paměti. V systému Windows Server 2008 je Služba ověřování v Internetu nahrazena serverem NPS (Network Policy Server). Útočník, který by úspěšně zneužil některou z těchto chyb zabezpečení, by mohl převzít úplnou kontrolu nad postiženým systémem. Servery používající Službu ověřování v Internetu nebo server NPS (Network Policy Server) jsou postiženy pouze tehdy, pokud používají protokol PEAP s ověřením MS-CHAP v2.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritický</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=141642">MS09-074</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení v aplikaci Microsoft Office Project umožňuje vzdálené spuštění kódu (967183)</strong><br />
<br />
Tato aktualizace zabezpečení řeší chybu zabezpečení v aplikaci Microsoft Office Project, kterou oznámila soukromá osoba. Tato chyba umožňuje vzdálené spuštění kódu, pokud uživatel otevře speciálně vytvořený soubor aplikace Project. Útočník, který by tuto chybu zabezpečení zneužil, by mohl získat úplnou kontrolu nad postiženým systémem. Útočník by tak mohl instalovat programy, zobrazovat, měnit či odstraňovat data nebo vytvářet nové účty s úplnými uživatelskými právy. Uživatelé, jejichž účty jsou konfigurovány tak, aby měli v systému méně uživatelských práv, by byli vystaveni menšímu riziku než uživatelé s uživatelskými právy správce.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritický</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Může vyžadovat restartování</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=169404">MS09-072</a></td>
<td style="border:1px solid black;"><strong>Kumulativní aktualizace zabezpečení pro aplikaci Internet Explorer (976325)</strong><br />
<br />
Tato aktualizace zabezpečení řeší čtyři chyby zabezpečení oznámené soukromými osobami a jednu veřejně známou chybu zabezpečení v aplikaci Internet Explorer. Tyto chyby zabezpečení mohou umožňovat vzdálené spuštění kódu, pokud uživatel pomocí aplikace Internet Explorer zobrazí speciálně vytvořenou webovou stránku. Uživatelé, jejichž účty jsou konfigurovány tak, aby měli v systému méně uživatelských práv, by byli vystaveni menšímu riziku než uživatelé s uživatelskými právy správce. Ovládací prvek ActiveX vytvořený pomocí záhlaví knihovny Microsoft Active Template Library (ATL) by také mohl umožnit vzdálené spuštění kódu. Tato chyba zabezpečení byla popsána v informačním zpravodaji zabezpečení společnosti Microsoft 973882 a bulletinu zabezpečení společnosti Microsoft MS09-035.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritický</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=177555">MS09-069</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení ve službě LSASS (Local Security Authority Subsystem Service) může způsobit odmítnutí služby (974392)</strong><br />
<br />
Tato aktualizace zabezpečení řeší chybu zabezpečení v systému Microsoft Windows, kterou oznámila soukromá osoba. Tato chyba zabezpečení by mohla způsobit odmítnutí služby, pokud by vzdálený ověřený útočník komunikující prostřednictvím protokolu IPsec (Internet Protocol security) odeslal speciálně vytvořenou zprávu ISAKMP do služby LSASS (Local Security Authority Subsystem Service) v postiženém systému.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Důležité</a><br />
Odmítnutí služby</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=163844">MS09-070</a></td>
<td style="border:1px solid black;"><strong>Chyby zabezpečení ve službě AD FS (Active Directory Federation Services) umožňují vzdálené spuštění kódu (971726)</strong><br />
<br />
Tato aktualizace zabezpečení řeší dvě soukromými osobami oznámené chyby zabezpečení v systému Microsoft Windows. Závažnější chyby zabezpečení mohou umožnit vzdálené spuštění kódu, pokud útočník odešle speciálně vytvořený požadavek HTTP webovému serveru s povolenou službou AD FS. Chce-li útočník zneužít těchto chyb zabezpečení, musí se jednat o ověřeného uživatele.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Důležité</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=163833">MS09-073</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení v převaděči WordPad a převaděčích textu systému Office umožňuje vzdálené spuštění kódu (975539)</strong><br />
<br />
Tato aktualizace zabezpečení řeší soukromou osobou oznámenou chybu zabezpečení převaděče Microsoft WordPad a převaděčů textu systému Microsoft Office. Chyba zabezpečení umožňuje vzdálené spuštění kódu v případě, že dojde k otevření speciálně vytvořeného souboru formátu Word 97 v převaděči WordPad nebo aplikaci Microsoft Office Word. Útočník, který by dokázal tuto chybu zabezpečení zneužít, by mohl získat stejná oprávnění, jako má uživatel. Uživatelé, jejichž účty jsou konfigurovány tak, aby měly v systému méně oprávnění, by byli vystaveni menšímu riziku než uživatelé s oprávněními správce.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Důležité</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Může vyžadovat restartování</td>
<td style="border:1px solid black;">Microsoft Windows, Microsoft Office</td>
</tr>
</tbody>
</table>
<p></p>
  
Index zneužitelnosti  
--------------------
  
 
Následující tabulka uvádí hodnocení zneužitelnosti každé chyby zabezpečení uvedené v tomto měsíci. Chyby zabezpečení jsou řazeny podle čísla jednotlivých bulletinů (ID bulletinu) a chyb (ID CVE).
  
**Jak pracovat s touto tabulkou**
  
V této tabulce zjistíte, jaká je pravděpodobnost vydání funkčního zneužitelného kódu během 30 dní od vydání tohoto bulletinu zabezpečení pro všechny aktualizace zabezpečení, které bude třeba nainstalovat. Všechna níže uvedená hodnocení zvažte na základě vaší specifické konfigurace a podle závěrů hodnocení nastavte priority pro zavádění jednotlivých aktualizací. Další informace o významu těchto hodnocení a způsobu jejich stanovení najdete v indexu zneužitelnosti [Microsoft Exploitability Index](http://technet.microsoft.com/en-us/security/cc998259.aspx).
  
| ID bulletinu                                              | Název chyby zabezpečení                                                                                                                   | ID CVE                                                                           | Hodnocení indexu zneužitelnosti                                                                                                | Hlavní poznámky                                                                                                                                                                                                                                                                |  
|-----------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| [MS09-069](http://go.microsoft.com/fwlink/?linkid=177555) | Chyba zabezpečení týkající se vyčerpání zdrojů služby LSASS (Local Security Authority Subsystem Service)                                  | [CVE-2009-3675](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-3675) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Vytvoření funkčního zneužitelného kódu není pravděpodobné | Tato chyba zabezpečení neumožňuje vzdálené spuštění kódu, způsobuje pouze odmítnutí služby, které se může vzdálený ověřený útočník pokusit zneužít.                                                                                                                            |  
| [MS09-070](http://go.microsoft.com/fwlink/?linkid=163844) | Chyba zabezpečení týkající se vkládání falešného obsahu ve službě AD FS (Active Directory Federation Services) při jednotném přihlašování | [CVE-2009-2508](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2508) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Vytvoření funkčního zneužitelného kódu není pravděpodobné | Tato chyba zabezpečení neumožňuje vzdálené spuštění kódu, umožňuje pouze vkládání falešného obsahu.                                                                                                                                                                            |  
| [MS09-070](http://go.microsoft.com/fwlink/?linkid=163844) | Chyba zabezpečení ve službě AD FS umožňující vzdálené spuštění kódu                                                                       | [CVE-2009-2509](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2509) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní kód zneužití je pravděpodobný                | Chybu zabezpečení může zneužít pouze ověřený útočník.                                                                                                                                                                                                                          |  
| [MS09-071](http://go.microsoft.com/fwlink/?linkid=177727) | Chyba zabezpečení týkající se poškození paměti Služby ověřování v Internetu                                                               | [CVE-2009-2505](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2505) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Nekonsistentní kód zneužití je pravděpodobný              | Omezená možnost vzdáleného spuštění kódu. Nejpravděpodobnějším výsledkem je odmítnutí služby.                                                                                                                                                                                  |  
| [MS09-071](http://go.microsoft.com/fwlink/?linkid=177727) | Chyba zabezpečení související s obejitím ověření protokolu MS-CHAP                                                                        | [CVE-2009-3677](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-3677) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Vytvoření funkčního zneužitelného kódu není pravděpodobné | Tato chyba zabezpečení neumožňuje vzdálené spuštění kódu, umožňuje pouze zvýšení úrovně oprávnění způsobené obejitím ověřování sítě.                                                                                                                                           |  
| [MS09-072](http://go.microsoft.com/fwlink/?linkid=169404) | Chyba zabezpečení inicializace ATL COM                                                                                                    | [CVE-2009-2493](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2493) | Žádné                                                                                                                          | (Této chybě zabezpečení byl přidělen index zneužitelnosti již v [červencovém souhrnném bulletinu](http://technet.microsoft.com/security/bulletin/ms09-jul). Tato chyba zabezpečení byla poprvé popsána v bulletinu [MS09-035](http://go.microsoft.com/fwlink/?linkid=158131).) |  
| [MS09-072](http://go.microsoft.com/fwlink/?linkid=169404) | Chyba zabezpečení týkající se poškození neinicializované paměti                                                                           | [CVE-2009-3671](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-3671) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní kód zneužití je pravděpodobný                | (Žádné)                                                                                                                                                                                                                                                                        |  
| [MS09-072](http://go.microsoft.com/fwlink/?linkid=169404) | Chyba zabezpečení týkající se poškození paměti objektů HTML                                                                               | [CVE-2009-3672](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-3672) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní kód zneužití je pravděpodobný                | (Žádné)                                                                                                                                                                                                                                                                        |  
| [MS09-072](http://go.microsoft.com/fwlink/?linkid=169404) | Chyba zabezpečení týkající se poškození neinicializované paměti                                                                           | [CVE-2009-3673](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-3673) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní kód zneužití je pravděpodobný                | (Žádné)                                                                                                                                                                                                                                                                        |  
| [MS09-072](http://go.microsoft.com/fwlink/?linkid=169404) | Chyba zabezpečení týkající se poškození neinicializované paměti                                                                           | [CVE-2009-3674](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-3674) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní kód zneužití je pravděpodobný                | (Žádné)                                                                                                                                                                                                                                                                        |  
| [MS09-073](http://go.microsoft.com/fwlink/?linkid=163833) | Chyba zabezpečení týkající se poškození paměti v převaděči WordPad a převaděči textu systému Office                                       | [CVE-2009-2506](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2506) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Nekonsistentní kód zneužití je pravděpodobný              | (Žádné)                                                                                                                                                                                                                                                                        |  
| [MS09-074](http://go.microsoft.com/fwlink/?linkid=141642) | Chyba zabezpečení týkající se ověřování paměti aplikace Project                                                                           | [CVE-2009-0102](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0102) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Nekonsistentní kód zneužití je pravděpodobný              | (Žádné)                                                                                                                                                                                                                                                                        |
  
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
</tr>
<tr>
<th colspan="6" style="border:1px solid black;">
Microsoft Windows 2000  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS09-071**](http://go.microsoft.com/fwlink/?linkid=177727)
</td>
<td style="border:1px solid black;">
[**MS09-072**](http://go.microsoft.com/fwlink/?linkid=169404)
</td>
<td style="border:1px solid black;">
[**MS09-069**](http://go.microsoft.com/fwlink/?linkid=177555)
</td>
<td style="border:1px solid black;">
[**MS09-070**](http://go.microsoft.com/fwlink/?linkid=163844)
</td>
<td style="border:1px solid black;">
[**MS09-073**](http://go.microsoft.com/fwlink/?linkid=163833)
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
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=5b02d10d-1abd-4d68-826b-71dad543657a)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Internet Explorer 5.01 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=0cf37247-505a-4dc2-aad7-c8cb1a63b57a)  
(Kritický)  
[Internet Explorer 6 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=7fb6261c-6895-4f79-be2c-bb110874a19c)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=560e01db-5f59-4ef1-9406-f5d7e0fd4128)  
(Důležitý)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=50936f51-b0a9-4e94-85bf-93f9ad74fdd1)  
(KB973904)  
(Důležitý)
</td>
</tr>
<tr>
<th colspan="6" style="border:1px solid black;">
Windows XP
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS09-071**](http://go.microsoft.com/fwlink/?linkid=177727)
</td>
<td style="border:1px solid black;">
[**MS09-072**](http://go.microsoft.com/fwlink/?linkid=169404)
</td>
<td style="border:1px solid black;">
[**MS09-069**](http://go.microsoft.com/fwlink/?linkid=177555)
</td>
<td style="border:1px solid black;">
[**MS09-070**](http://go.microsoft.com/fwlink/?linkid=163844)
</td>
<td style="border:1px solid black;">
[**MS09-073**](http://go.microsoft.com/fwlink/?linkid=163833)
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
[Windows XP Service Pack 2 a Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=4d294be6-19d1-43b5-9c75-f9d30699a2e7)  
(Mírný)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=facab13f-ea31-4c71-be4c-24e44ded174f)  
(Kritický)  
[Aplikace Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=def2c038-3b03-4162-a563-a6ebec756f37)  
(Kritický)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=6c003629-77bf-4735-bd4a-c37c4386f869)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 a Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=5448b168-6bf7-4bae-9627-b88d76c4d5c5)  
(Mírný)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 a Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=c090c4c2-c277-4d8c-91e1-28286bc5443e)  
(KB973904)  
(Důležitý)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=17b5206d-61e9-4663-afc7-80e98bf4d618)  
(Mírný)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=a253c19a-c808-4115-8bd0-cf312d396abd)  
(Kritický)  
[Aplikace Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=98a56425-4f88-4f0f-963b-dada8dc0d8f8)  
(Kritický)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=0c9af3b5-d015-4025-bbb4-1a5113e9113f)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c2bbf515-f81a-436b-947b-cbf2db85fdd9)  
(Důležitý)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4b9bf156-cd34-460f-b4ad-571e37f54659)  
(KB973904)  
(Důležitý)
</td>
</tr>
<tr>
<th colspan="6" style="border:1px solid black;">
Windows Server 2003
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS09-071**](http://go.microsoft.com/fwlink/?linkid=177727)
</td>
<td style="border:1px solid black;">
[**MS09-072**](http://go.microsoft.com/fwlink/?linkid=169404)
</td>
<td style="border:1px solid black;">
[**MS09-069**](http://go.microsoft.com/fwlink/?linkid=177555)
</td>
<td style="border:1px solid black;">
[**MS09-070**](http://go.microsoft.com/fwlink/?linkid=163844)
</td>
<td style="border:1px solid black;">
[**MS09-073**](http://go.microsoft.com/fwlink/?linkid=163833)
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
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3d49b386-133a-4d51-b6f0-cec0c70ef93e)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=6659fc40-71ee-44a9-9656-8d3ee02b5bc0)  
(Kritický)  
[Aplikace Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=7bdba030-e2c6-44ac-bb5f-24ae8ec372a2)  
(Mírný)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=0dd50357-64f2-4286-86ba-c512e65eed2a)  
(Mírný)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=a779aae1-7724-4458-94fb-a2343356ecae)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=31351b9e-b5bb-4618-990b-1089ea5a3bc2)<sup>[1]</sup>
(Důležitý)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b9678229-2473-4aae-a814-eca9ea556d17)  
(KB973904)  
(Důležitý)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5a273b47-8a18-4778-9b60-8b560a1ce089)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=287e7921-8aab-42a6-b647-551d0a9adc15)  
(Kritický)  
[Aplikace Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=4de4bbcd-b1b8-4482-8ef7-0d9b4a730e0c)  
(Mírný)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=e62aba15-5eeb-46a2-a142-bfca94016c55)  
(Mírný)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=a8a9bf12-4ad6-49fd-b2b7-f379dc3309d2)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b6eb9d9b-1a43-4b30-a033-19a1db786244)<sup>[2]</sup>
(Důležitý)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=257facf3-20a1-49e2-ab4c-c1ae67fe05a0)  
(KB973904)  
(Důležitý)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 SP2 pro systémy s procesorem Itanium
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=498f5eeb-d03e-42ee-ad6a-9d6f98c66acb)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=9ce1a721-0c6a-4775-9407-9633d817d716)  
(Kritický)  
[Aplikace Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=72d44de7-dfc5-4667-a59f-2ee73d0e3708)  
(Mírný)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=f5b003ad-af25-488a-91fb-98835a0bfeac)  
(Důležitý)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=1a7784ef-5d25-4de1-a293-f742b5a3473d)  
(KB973904)  
(Důležitý)
</td>
</tr>
<tr>
<th colspan="6" style="border:1px solid black;">
Windows Vista
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS09-071**](http://go.microsoft.com/fwlink/?linkid=177727)
</td>
<td style="border:1px solid black;">
[**MS09-072**](http://go.microsoft.com/fwlink/?linkid=169404)
</td>
<td style="border:1px solid black;">
[**MS09-069**](http://go.microsoft.com/fwlink/?linkid=177555)
</td>
<td style="border:1px solid black;">
[**MS09-070**](http://go.microsoft.com/fwlink/?linkid=163844)
</td>
<td style="border:1px solid black;">
[**MS09-073**](http://go.microsoft.com/fwlink/?linkid=163833)
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
Žádné
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
[Windows Vista a Windows Vista Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=3e4ae4d0-1060-4867-82c5-7e20ea93c2c6)  
(Mírný)  
[Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3e4ae4d0-1060-4867-82c5-7e20ea93c2c6)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=40d26d40-4203-4013-b3f9-912a5b209fbd)  
(Kritický)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=47d5ada1-1d60-4233-bdd3-64918b5e1245)  
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
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 a Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition a Windows Vista x64 Edition Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=2ca62ea8-67cb-40da-8a65-db6f3607bbab)  
(Mírný)  
[Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2ca62ea8-67cb-40da-8a65-db6f3607bbab)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=3140527a-aa33-462b-b3a6-bfcd78b5aa0c)  
(Kritický)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=1e466b48-422f-4c80-8fdf-ba61111942b1)  
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
</tr>
<tr>
<th colspan="6" style="border:1px solid black;">
Windows Server 2008
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS09-071**](http://go.microsoft.com/fwlink/?linkid=177727)
</td>
<td style="border:1px solid black;">
[**MS09-072**](http://go.microsoft.com/fwlink/?linkid=169404)
</td>
<td style="border:1px solid black;">
[**MS09-069**](http://go.microsoft.com/fwlink/?linkid=177555)
</td>
<td style="border:1px solid black;">
[**MS09-070**](http://go.microsoft.com/fwlink/?linkid=163844)
</td>
<td style="border:1px solid black;">
[**MS09-073**](http://go.microsoft.com/fwlink/?linkid=163833)
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
[**Mírný**](http://go.microsoft.com/fwlink/?linkid=21140)
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
Windows Server 2008 pro 32bitové systémy a Windows Server 2008 pro 32bitové systémy Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro 32bitové systémy](http://www.microsoft.com/downloads/details.aspx?familyid=582a1b15-214e-4f5e-bb5b-95677f4d5968)\*  
(Důležitý)  
[Windows Server 2008 pro 32bitové systémy Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=582a1b15-214e-4f5e-bb5b-95677f4d5968)\*  
(Kritický)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=d0570536-756e-4fda-883d-f2a3c4ac5bbd)\*  
(Mírný)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=43660133-43e1-41f3-8a82-98c4a739914f)\*  
(Mírný)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro 32bitové systémy a Windows Server 2008 pro 32bitové systémy Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=f6715abb-fd93-44ba-9854-2ecc672622da)\*  
(Důležitý)
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
[Windows Server 2008 pro systémy s procesorem x64](http://www.microsoft.com/downloads/details.aspx?familyid=77e774b4-ec0c-481c-9e93-eee9f44ec71b)\*  
(Důležitý)  
[Windows Server 2008 pro systémy s procesorem x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=77e774b4-ec0c-481c-9e93-eee9f44ec71b)\*  
(Kritický)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=0e72d0f1-2ce7-4650-b72c-bb303351aafc)\*  
(Mírný)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=22972970-740f-4c50-93ec-f6d49dd1b360)\*  
(Mírný)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem x64 a Windows Server 2008 pro systémy s procesorem x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7d1f5e9e-a7de-4f96-89c8-510fd51f16e7)\*  
(Důležitý)
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
[Windows Server 2008 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=89defe77-7e82-4bfa-9693-66c93b930da1)  
(Mírný)  
[Windows Server 2008 pro systémy s procesorem Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=89defe77-7e82-4bfa-9693-66c93b930da1)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=2c7765a2-3117-4dd8-94b4-0060ca16871b)  
(Mírný)
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
</tr>
<tr>
<th colspan="6" style="border:1px solid black;">
Windows 7
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS09-071**](http://go.microsoft.com/fwlink/?linkid=177727)
</td>
<td style="border:1px solid black;">
[**MS09-072**](http://go.microsoft.com/fwlink/?linkid=169404)
</td>
<td style="border:1px solid black;">
[**MS09-069**](http://go.microsoft.com/fwlink/?linkid=177555)
</td>
<td style="border:1px solid black;">
[**MS09-070**](http://go.microsoft.com/fwlink/?linkid=163844)
</td>
<td style="border:1px solid black;">
[**MS09-073**](http://go.microsoft.com/fwlink/?linkid=163833)
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
[**Kritický**](http://go.microsoft.com/fwlink/?linkid=21140)
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
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 7 pro 32bitové systémy
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=5af3be0b-2dd2-4039-90e1-2278e9c5aee5)  
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
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 pro systémy s procesorem x64
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=9d9a04c8-a019-4943-8e93-c6bfd77c8960)  
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
</tr>
<tr>
<th colspan="6" style="border:1px solid black;">
Windows Server 2008 R2
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS09-071**](http://go.microsoft.com/fwlink/?linkid=177727)
</td>
<td style="border:1px solid black;">
[**MS09-072**](http://go.microsoft.com/fwlink/?linkid=169404)
</td>
<td style="border:1px solid black;">
[**MS09-069**](http://go.microsoft.com/fwlink/?linkid=177555)
</td>
<td style="border:1px solid black;">
[**MS09-070**](http://go.microsoft.com/fwlink/?linkid=163844)
</td>
<td style="border:1px solid black;">
[**MS09-073**](http://go.microsoft.com/fwlink/?linkid=163833)
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
[**Mírný**](http://go.microsoft.com/fwlink/?linkid=21140)
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
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 pro systémy s procesorem x64
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=bcb38127-787f-49b0-b3fb-62f6a8628d89)\*  
(Mírný)
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
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 pro systémy s procesorem Itanium
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=2c1b96f2-b3c3-4711-a9ad-b2133ea7bf81)  
(Mírný)
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
</tr>
</table>
<p></p>
 
**Poznámka k systémům Windows Server 2008 a Windows Server 2008 R2**

**\*Instalace Server Core není touto chybou ovlivněna.** Chyby zabezpečení, které tato aktualizace řeší, nemají vliv na podporované edice systému Windows Server 2008 nebo Windows Server 2008 R2, jak je uvedeno, v případě instalace s využitím možnosti instalace Server Core. Další informace o této možnosti instalace naleznete v článcích na webu služby MSDN, [Server Core](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx) a [Server Core for Windows Server 2008 R2](http://msdn.microsoft.com/en-us/library/ee391631(vs.85).aspx). Možnost instalace Server Core se nevztahuje na určité edice systému Windows Server 2008 a Windows Server 2008 R2; další informace naleznete v části [Porovnání možností instalace Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**Poznámky k bulletinu MS09-070**

<sup>[1]</sup> Postižení chybou zabezpečení nastává pouze tehdy, je-li nainstalován systém Windows Server 2003 R2, který používá službu AD FS (Active Directory Federation Services).

<sup>[2]</sup> Postižení chybou zabezpečení nastává pouze tehdy, je-li nainstalován systém Windows Server 2003 R2 x64 Edition, který používá službu AD FS (Active Directory Federation Services).

**Poznámka k bulletinu MS09-073**

Více aktualizovaných souborů v rámci stejného identifikátoru bulletinu naleznete také v dalších kategoriích softwaru v rámci této části **Software obsahující tuto chybu a umístění aktualizací ke stažení**. Tento bulletin se vztahuje na více kategorií softwaru.

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
[**MS09-074**](http://go.microsoft.com/fwlink/?linkid=141642)
</td>
<td style="border:1px solid black;">
[**MS09-073**](http://go.microsoft.com/fwlink/?linkid=163833)
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
Microsoft Office XP
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Microsoft Office XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=bc3ec3ba-2cec-43ab-b184-c222794231f2)  
(KB975008)  
(Důležitý)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2003
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Microsoft Office 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=b4a4126c-b0b3-4db2-b6f5-0e67519c2a5f)  
(KB975051)  
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
[**MS09-074**](http://go.microsoft.com/fwlink/?linkid=141642)
</td>
<td style="border:1px solid black;">
[**MS09-073**](http://go.microsoft.com/fwlink/?linkid=163833)
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
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Project 2000
</td>
<td style="border:1px solid black;">
[Microsoft Project 2000 Service Release 1](http://www.microsoft.com/downloads/details.aspx?familyid=135c010a-55f4-4385-b67d-96ea06ef881a)  
(KB961083)  
(Kritický)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Project 2002
</td>
<td style="border:1px solid black;">
[Microsoft Project 2002 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=c55ef8fe-8f66-42fc-a298-de6f8886b3e4)  
(KB961079)  
(Důležitý)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Project 2003
</td>
<td style="border:1px solid black;">
[Microsoft Office Project 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=2ea8ca39-f130-439a-92d5-77e9ef050105)  
(KB961082)  
(Důležitý)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Works 8.5
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Microsoft Works 8.5](http://www.microsoft.com/downloads/details.aspx?familyid=807426a1-8b78-4681-a606-dc39f4d7b64a)  
(KB977304)  
(Důležitý)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Converter Pack
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Microsoft Office Converter Pack](http://www.microsoft.com/downloads/details.aspx?familyid=f3ff8bb6-d047-42f1-9331-b6df85fff9fd)  
(KB974882)  
(Důležitý)
</td>
</tr>
</table>
<p></p>
 
**Poznámka k bulletinu MS09-073**

Více aktualizovaných souborů v rámci stejného identifikátoru bulletinu naleznete také v dalších kategoriích softwaru v rámci této části **Software obsahující tuto chybu a umístění aktualizací ke stažení**. Tento bulletin se vztahuje na více kategorií softwaru.

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

-   Ryanu Smithovi ze společnosti [VeriSign iDefense Labs](http://labs.idefense.com/) za oznámení chyby popsané v bulletinu MS09-072.
-   Samu Thomasovi ze společnosti eshu.co.uk, spolupracujícímu se společností [TippingPoint](http://www.tippingpoint.com/) a organizací [Zero Day Initiative](http://www.zerodayinitiative.com/), za oznámení chyby popsané v bulletinu MS09-072.
-   Skupině [team 509](http://www.team509.com/), spolupracující se společností [VeriSign iDefense Labs](http://labs.idefense.com/), za oznámení chyby popsané v bulletinu MS09-072.
-   Anonymnímu výzkumníkovi spolupracujícímu se společností [TippingPoint](http://www.tippingpoint.com/) a organizací [Zero Day Initiative](http://www.zerodayinitiative.com/) za oznámení chyby popsané v bulletinu MS09-072.
-   Anonymnímu výzkumníkovi spolupracujícímu se společností [TippingPoint](http://www.tippingpoint.com/) a organizací [Zero Day Initiative](http://www.zerodayinitiative.com/) za oznámení jiné chyby popsané v bulletinu MS09-072.
-   Seanu Larssonovi a Junu Maovi ze společnosti [VeriSign iDefense Labs](http://labs.idefense.com/) za oznámení chyby popsané v bulletinu MS09-073.
-   Bingu Liuovi z výzkumného týmu [FortiGuard Labs společnosti Fortinet](http://www.fortiguard.com/) za oznámení chyby popsané v bulletinu MS09-074.

#### Technická podpora

-   Uvedený software byl testován za účelem zjištění, kterých verzí se chyba týká. U dalších verzí skončila časově omezená podpora. Pokud chcete zjistit dobu, po kterou je pro určitou verzi softwaru poskytována podpora, navštivte web [Zásady poskytování technické podpory pro produkty společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=21742).
-   Zákazníci mohou získat technickou podporu na webu [služby technické podpory společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=21131). Hovory související s aktualizacemi zabezpečení jsou bezplatné. Další informace o dostupných možnostech technické podpory naleznete na webu [Pomoc a podpora společnosti Microsoft](http://support.microsoft.com/).
-   Mezinárodní zákazníci získají podporu u místních zastoupení společnosti Microsoft. Technická podpora související s aktualizacemi zabezpečení je bezplatná. Další informace o možnostech kontaktování společnosti Microsoft v případě potřeby technické podpory získáte na [webu mezinárodní technické podpory](http://go.microsoft.com/fwlink/?linkid=21155).

#### Zřeknutí se záruky

Informace ve znalostní bázi Microsoft Knowledge Base jsou poskytovány tak, jak jsou, bez jakékoli záruky. Společnost Microsoft neposkytuje žádné záruky, výslovně uvedené či mlčky předpokládané, včetně záruk obchodovatelnosti a vhodnosti pro určitý účel. Společnost Microsoft ani její dodavatelé nenesou v žádném případě zodpovědnost za žádné škody, včetně přímých, nepřímých, náhodných či následných škod, ztráty zisku či zvláštních škod, a to ani v případě, že byli na možnost takových škod upozorněni. V některých zemích a právních řádech není dovoleno vyloučit nebo omezit odpovědnost, proto se výše uvedené omezení na vás nemusí vztahovat.

#### Revize

-   V1.0 (8. prosince 2009): Souhrnný bulletin byl publikován.
-   V1.1 (9. prosince 2009): V tabulce Shrnutí byl aktualizován popis bulletinu MS09-071. U bulletinu MS09-073 došlo k opravě požadavku na restartování.
-   V2.0 (13. ledna 2010): Balíčky aktualizací **Microsoft Office Word 2002 Service Pack 3 (KB975008)** a **Microsoft Office Word 2003 Service Pack 3 (KB975051)** byly v bulletinu MS09-073 přejmenovány na **Microsoft Office XP Service Pack 3 (KB975008)** a **Microsoft Office 2003 Service Pack 3 (KB975051)**.

*Built at 2014-04-18T01:50:00Z-07:00*
