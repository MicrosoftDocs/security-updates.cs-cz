---
TOCTitle: 'MS12-APR'
Title: 'Souhrnný bulletin zabezpečení společnosti Microsoft, duben 2012'
ms:assetid: 'ms12-apr'
ms:contentKeyID: 61224018
ms:mtpsurl: 'https://technet.microsoft.com/cs-CZ/library/ms12-apr(v=Security.10)'
---

 

Souhrnný bulletin zabezpečení společnosti Microsoft, duben 2012
===============================================================

Publikováno: 10. dubna 2012 | Aktualizováno: 26. dubna 2012

**Verze:** 2.0

Tento souhrnný bulletin uvádí bulletiny zabezpečení vydané v dubnu 2012.

Spolu s vydáním bulletinů zabezpečení pro duben 2012 nahrazuje tento souhrnný bulletin předběžné oznámení o bulletinech vydané 5. dubna 2012. Další informace o službě předběžného oznámení o bulletinech naleznete v části [Předběžné oznámení o bulletinech zabezpečení společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=217213).

Informace o tom, jak dostávat automatická oznámení o vydání nových bulletinů zabezpečení společnosti Microsoft, naleznete na webu [Zasílání technických oznámení o zabezpečení společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=21163).

Pro zodpovězení zákaznických dotazů týkajících se těchto bulletinů uspořádá společnost Microsoft webové vysílání 11. dubna 2012 v 11:00 časového pásma Tichomoří (USA a Kanada). [Přihlaste se k webovému vysílání týkajícímu se dubnových bulletinů zabezpečení](https://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032499650). Po tomto datu je webové vysílání dostupné na požádání. Další informace získáte v [souhrnných bulletinech zabezpečení společnosti Microsoft a webovém vysílání](http://go.microsoft.com/fwlink/?linkid=217214).

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
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=242739">MS12-023</a></td>
<td style="border:1px solid black;"><strong>Kumulativní aktualizace zabezpečení pro aplikaci Internet Explorer (2675157)</strong><br />
<br />
Tato aktualizace zabezpečení řeší pět soukromě oznámených chyb zabezpečení aplikace Internet Explorer. Nejzávažnější chyby zabezpečení mohou umožnit vzdálené spuštění kódu, pokud uživatel pomocí aplikace Internet Explorer zobrazí speciálně vytvořenou webovou stránku. Útočník, který by úspěšně zneužil některou z těchto chyb zabezpečení, by mohl získat stejná uživatelská práva, jaká má současný uživatel. Uživatelé, jejichž účty jsou konfigurovány tak, aby měli v systému méně uživatelských práv, by byli vystaveni menšímu riziku než uživatelé s uživatelskými právy správce.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritický</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Internet Explorer</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=238623">MS12-024</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení systému Windows umožňuje vzdálené spuštění kódu (2653956)</strong><br />
<br />
Tato aktualizace zabezpečení řeší chybu zabezpečení v systému Microsoft Windows, kterou oznámila soukromá osoba. Chyba zabezpečení může umožnit vzdálené spuštění kódu, pokud uživatel nebo aplikace spustí nebo nainstaluje speciálně vytvořený a podepsaný přenosný spustitelný soubor (PE) v postiženém systému.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritický</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=242032">MS12-025</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení</strong> <strong>v rozhraní .NET Framework umožňuje vzdálené spuštění kódu (2671605)</strong><br />
<br />
Tato aktualizace zabezpečení řeší soukromě oznámenou chybu zabezpečení v rozhraní Microsoft .NET Framework. Tyta chyba zabezpečení by mohla umožnit vzdálené spuštění kódu v klientském systému, pokud by uživatel zobrazil speciálně vytvořenou webovou stránku pomocí webového prohlížeče, v němž lze otevírat aplikace prohlížeče XAML (XBAP). Uživatelé, jejichž účty jsou konfigurovány tak, aby měli v systému méně uživatelských práv, by byli vystaveni menšímu riziku než uživatelé s uživatelskými právy správce. Chyba zabezpečení dále může umožnit vzdálené spuštění kódu na serverovém systému se službou IIS v případě, že tento server umožňuje zpracování stránek ASP.NET a útočníkovi se úspěšně podaří na daném serveru načíst speciálně vytvořenou stránku ASP.NET a poté ji spustit, jako například v případě hostování webu. Tuto chybu zabezpečení mohou zneužít také aplikace Windows .NET k obejití omezení zabezpečení přístupu kódu (CAS). V případě útoku z webu by útočník mohl být hostitelem webu s webovou stránkou, pomocí které lze tuto chybu zabezpečení zneužít. Navíc dané weby a weby, které přijímají nebo hostují materiál poskytovaný uživateli a reklamu, by mohly obsahovat speciálně vytvořený obsah zneužívající tuto chybu zabezpečení. Útočník však nemůže žádným způsobem přinutit uživatele k návštěvě takových webů. Místo toho by útočník musel přesvědčit uživatele, aby navštívili takový web. K tomu se obvykle používá odkaz v e-mailové zprávě nebo zprávě programu pro zasílání rychlých zpráv, na který uživatelé kliknou, a přejdou tak na útočníkův web.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritický</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Může vyžadovat restartování</td>
<td style="border:1px solid black;">Microsoft Windows, Microsoft .NET Framework</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=246275">MS12-027</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení běžných ovládacích prvků systému Windows umožňuje vzdálené spuštění kódu (2664258)</strong><br />
<br />
Tato aktualizace zabezpečení řeší chybu zabezpečení běžných ovládacích prvků systému Windows, oznámenou soukromou osobou. Tato chyba zabezpečení by mohla umožnit vzdálené spuštění kódu, pokud uživatel navštíví web se speciálně vytvořeným obsahem, který se snaží tuto chybu zabezpečení zneužít. Útočník však nemůže žádným způsobem přinutit uživatele k návštěvě takového webu. Místo toho by útočník musel přesvědčit uživatele, aby navštívili takový web. K tomu se obvykle používá odkaz v e-mailové zprávě nebo zprávě programu pro zasílání rychlých zpráv, na který uživatelé kliknou, a přejdou tak na útočníkův web. Škodlivý soubor je také možné zaslat v příloze e-mailu. Útočník by však musel uživatele přimět k otevření přílohy, aby mohl tuto chybu zabezpečení využít.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritický</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Může vyžadovat restartování</td>
<td style="border:1px solid black;">Microsoft Office,<br />
Microsoft SQL Server,<br />
Microsoft Server Software,<br />
Vývojářské nástroje společnosti Microsoft</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=238519">MS12-026</a></td>
<td style="border:1px solid black;"><strong>Chyby zabezpečení v aplikaci Forefront Unified Access Gateway (UAG) mohou umožnit přístup k informacím (2663860)</strong><br />
<br />
Tato aktualizace zabezpečení řeší dvě chyby zabezpečení aplikace Microsoft Forefront Unified Access Gateway (UAG) oznámené soukromými osobami. Závažnější chyby zabezpečení mohou umožnit zpřístupnění informací, pokud útočník odešle speciálně vytvořený dotaz na server UAG.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Vysoký</a><br />
Přístup k informacím</td>
<td style="border:1px solid black;">Může vyžadovat restartování</td>
<td style="border:1px solid black;">Microsoft Forefront Unified Access Gateway</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=232498">MS12-028</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení v systému Microsoft Office umožňuje vzdálené spuštění kódu (2639185)</strong><br />
<br />
Tato aktualizace zabezpečení řeší chybu zabezpečení v systému Microsoft Office a Microsoft Works, kterou oznámila soukromá osoba. Tato chyba umožňuje vzdálené spuštění kódu, pokud uživatel otevře speciálně vytvořený soubor sady Works. Útočník, který by úspěšně zneužil tuto chybu zabezpečení, by mohl získat stejná uživatelská práva, jaká má současný uživatel. Uživatelé, jejichž účty jsou konfigurovány tak, aby měli v systému méně uživatelských práv, by byli vystaveni menšímu riziku než uživatelé s uživatelskými právy správce.</td>
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
  
 
Následující tabulka uvádí hodnocení zneužitelnosti každé chyby zabezpečení uvedené v tomto měsíci. Chyby zabezpečení jsou řazeny podle čísla jednotlivých bulletinů (ID bulletinu) a chyb (ID CVE). Uvedeny jsou pouze chyby zabezpečení ohodnocené stupněm závažnosti Kritický nebo Vysoký.
  
**Jak pracovat s touto tabulkou**
  
V této tabulce zjistíte, jaká je pravděpodobnost zneužití v podobě spuštění kódu a odmítnutí služby během 30 dní od vydání tohoto bulletinu zabezpečení pro všechny aktualizace zabezpečení, které bude třeba nainstalovat. Všechna níže uvedená hodnocení zvažte na základě vaší specifické konfigurace a podle závěrů hodnocení nastavte priority pro zavádění jednotlivých aktualizací vydaných v tomto měsíci. Další informace o významu těchto hodnocení a způsobu jejich stanovení najdete v indexu zneužitelnosti [Microsoft Exploitability Index](http://technet.microsoft.com/security/cc998259.aspx).
  
Položka nazvaná „Nejnovější vydání softwaru“ odkazuje na příslušný software. Položka nazvaná „Starší vydání softwaru“ odkazuje na všechna starší podporovaná vydání příslušného softwaru, uvedeného v tabulkách bulletinu „Software obsahující tuto chybu“ a „Software neobsahující tuto chybu“.
  
| ID bulletinu                                              | Název chyby zabezpečení                                                          | ID CVE                                                                           | Hodnocení zneužitelnosti u nejnovějšího vydání softwaru                                                          | Hodnocení zneužitelnosti u starších vydání softwaru                                                            | Hodnocení zneužitelnosti odmítnutí služby | Hlavní poznámky                                                                                                        |  
|-----------------------------------------------------------|----------------------------------------------------------------------------------|----------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------|-------------------------------------------|------------------------------------------------------------------------------------------------------------------------|  
| [MS12-023](http://go.microsoft.com/fwlink/?linkid=242739) | Chyba zabezpečení souboru JScript9 umožňující vzdálené spuštění kódu             | [CVE-2012-0169](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0169) | [3](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Vytvoření zneužitelného kódu není pravděpodobné | Žádné ohrožení                                                                                                 | Dočasné                                   | (Žádné)                                                                                                                |  
| [MS12-023](http://go.microsoft.com/fwlink/?linkid=242739) | Chyba zabezpečení metody OnReadyStateChange umožňující vzdálené spuštění kódu    | [CVE-2012-0170](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0170) | Žádné ohrožení                                                                                                   | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Je pravděpodobné vytvoření zneužitelného kódu | Dočasné                                   | (Žádné)                                                                                                                |  
| [MS12-023](http://go.microsoft.com/fwlink/?linkid=242739) | Chyba zabezpečení metody SelectAll (VybratVše) umožňující vzdálené spuštění kódu | [CVE-2012-0171](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0171) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Je pravděpodobné vytvoření zneužitelného kódu   | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Je pravděpodobné vytvoření zneužitelného kódu | Dočasné                                   | (Žádné)                                                                                                                |  
| [MS12-023](http://go.microsoft.com/fwlink/?linkid=242739) | Chyba zabezpečení stylu VML umožňující vzdálené spuštění kódu                    | [CVE-2012-0172](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0172) | Žádné ohrožení                                                                                                   | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Je pravděpodobné vytvoření zneužitelného kódu | Dočasné                                   | (Žádné)                                                                                                                |  
| [MS12-024](http://go.microsoft.com/fwlink/?linkid=238623) | Chyba zabezpečení ověření podpisu funkce WinVerifyTrust                          | [CVE-2012-0151](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0151) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Je pravděpodobné vytvoření zneužitelného kódu   | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Je pravděpodobné vytvoření zneužitelného kódu | Netýká se                                 | (Žádné)                                                                                                                |  
| [MS12-025](http://go.microsoft.com/fwlink/?linkid=242032) | Chyba zabezpečení ověřování parametrů rozhraní .NET Framework                    | [CVE-2012-0163](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0163) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Je pravděpodobné vytvoření zneužitelného kódu   | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Je pravděpodobné vytvoření zneužitelného kódu | Netýká se                                 | (Žádné)                                                                                                                |  
| [MS12-026](http://go.microsoft.com/fwlink/?linkid=238519) | Chyba zabezpečení nefiltrovaného přístupu k výchozí stránce UAG                  | [CVE-2012-0147](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0147) | [3](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Vytvoření zneužitelného kódu není pravděpodobné | Žádné ohrožení                                                                                                 | Netýká se                                 | Jedná se o chybu zabezpečení typu zpřístupnění informací.                                                              |  
| [MS12-027](http://go.microsoft.com/fwlink/?linkid=246275) | Chyba zabezpečení týkající se vzdáleného spuštění kódu prvku MSCOMCTL.OCX        | [CVE-2012-0158](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0158) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Je pravděpodobné vytvoření zneužitelného kódu   | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Je pravděpodobné vytvoření zneužitelného kódu | Netýká se                                 | Společnost Microsoft získala informace o omezeném počtu cílených útoků, které se snaží tuto chybu zabezpečení zneužít. |  
| [MS12-028](http://go.microsoft.com/fwlink/?linkid=232498) | Chyba zabezpečení týkající se přetečení haldy převaděče Office WPS               | [CVE-2012-0177](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0177) | [3](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Vytvoření zneužitelného kódu není pravděpodobné | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Je pravděpodobné vytvoření zneužitelného kódu | Netýká se                                 | Microsoft Office 2007 Service Pack 3 a všechny podporované edice systému Microsoft Office 2010.                        |
  
Software obsahující tuto chybu a umístění aktualizací ke stažení  
----------------------------------------------------------------
  
 
Následující tabulky řadí bulletiny podle kategorie hlavního softwaru a závažnosti.
  
**Jak pracovat s těmito tabulkami?**
  
V těchto tabulkách zjistíte, které aktualizace zabezpečení bude třeba nainstalovat. Přečtěte si seznam všech programů a komponent a zjistěte, zda se některé aktualizace zabezpečení týkají vaší instalace. Pokud se program nebo komponenta v seznamu nachází, je v něm zároveň uveden odkaz na dostupnou aktualizaci softwaru a také stupeň závažnosti aktualizace softwaru.
  
**Poznámka:** Jedna chyba zabezpečení může vyžadovat instalaci více aktualizací. Přečtěte si celý sloupec u každého identifikátoru bulletinu. Zjistíte v něm, které aktualizace je třeba nainstalovat v závislosti na programech nebo součástech nainstalovaných ve vašem systému.
  
#### Operační systém Windows a jeho komponenty

 
<p></p>
<table style="border:1px solid black;">
<tr>
<th colspan="4" style="border:1px solid black;">
Windows XP  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS12-023**](http://go.microsoft.com/fwlink/?linkid=242739)
</td>
<td style="border:1px solid black;">
[**MS12-024**](http://go.microsoft.com/fwlink/?linkid=238623)
</td>
<td style="border:1px solid black;">
[**MS12-025**](http://go.microsoft.com/fwlink/?linkid=242032)
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
Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Aplikace Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=2a490c62-16c4-402a-b2d9-3e8cfb5bcebd)  
(KB2675157)  
(Kritický)  
[Aplikace Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=81b28dd9-87aa-46cc-94c6-2da39d0298db)  
(KB2675157)  
(Kritický)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=74ce0e29-046b-4ac3-89a1-b292a177972f)  
(KB2675157)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=575afd20-cee4-4fa9-b781-9f8dfdd41ebe)  
(KB2653956)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.0 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=1cfeae57-d4e9-4fff-8956-523e7b71453c)  
(KB2656378)  
(pouze Media Center Edition 2005 a Tablet PC Edition 2005)  
(Kritický)  
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=c376fbdc-2289-47b6-950b-4e668cd3a390)  
(KB2656370)  
(Kritický)  
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c1338821-d8b2-4513-aa35-087323188509)  
(KB2656369)  
(Kritický)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=40b1ae34-28ad-41a0-88df-b905517e4acf)<sup>[1]</sup>
(KB2656368)  
(Kritický)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Aplikace Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=a1b7be43-a32e-456b-8df0-c26cdf187682)  
(KB2675157)  
(Kritický)  
[Aplikace Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=29ec7b06-c7aa-4149-bb2c-25af7d38a6a9)  
(KB2675157)  
(Kritický)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=646c6352-4d99-413a-a75b-71289b5d2b25)  
(KB2675157)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=adc31695-1be6-4976-869c-007df8ac8508)  
(KB2653956)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=c376fbdc-2289-47b6-950b-4e668cd3a390)  
(KB2656370)  
(Kritický)  
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c1338821-d8b2-4513-aa35-087323188509)  
(KB2656369)  
(Kritický)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=40b1ae34-28ad-41a0-88df-b905517e4acf)<sup>[1]</sup>
(KB2656368)  
(Kritický)
</td>
</tr>
<tr>
<th colspan="4" style="border:1px solid black;">
Windows Server 2003
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS12-023**](http://go.microsoft.com/fwlink/?linkid=242739)
</td>
<td style="border:1px solid black;">
[**MS12-024**](http://go.microsoft.com/fwlink/?linkid=238623)
</td>
<td style="border:1px solid black;">
[**MS12-025**](http://go.microsoft.com/fwlink/?linkid=242032)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Celkový** **stupeň závažnosti**
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
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Aplikace Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=020e0d68-dd1c-4297-b565-fcc6dcf5f280)  
(KB2675157)  
(Mírný)  
[Aplikace Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=17b0c139-2709-424d-9d17-827af468e858)  
(KB2675157)  
(Mírný)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=3289a80a-d1b1-4494-bede-03d0be579acf)  
(KB2675157)  
(Mírný)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=f79c8940-ca31-4ff7-924e-847f5eef7864)  
(KB2653956)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=ffd26218-e149-44ea-a0b9-f2a1315fce9e)  
(KB2656376)  
(Kritický)  
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c1338821-d8b2-4513-aa35-087323188509)  
(KB2656369)  
(Kritický)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=40b1ae34-28ad-41a0-88df-b905517e4acf)<sup>[1]</sup>
(KB2656368)  
(Kritický)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Aplikace Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=295292d3-01a3-4574-b994-8cdbcf5a0d2e)  
(KB2675157)  
(Mírný)  
[Aplikace Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=04656a93-e958-4764-afe8-27c476855506)  
(KB2675157)  
(Mírný)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=dff4fb63-b319-49ed-8a9d-6b15e43d5bfd)  
(KB2675157)  
(Mírný)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=03ebf111-1e7b-4dc2-b84f-a26c6b5f0d58)  
(KB2653956)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=c376fbdc-2289-47b6-950b-4e668cd3a390)  
(KB2656370)  
(Kritický)  
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c1338821-d8b2-4513-aa35-087323188509)  
(KB2656369)  
(Kritický)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=40b1ae34-28ad-41a0-88df-b905517e4acf)<sup>[1]</sup>
(KB2656368)  
(Kritický)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 SP2 pro systémy s procesorem Itanium
</td>
<td style="border:1px solid black;">
[Aplikace Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=09011393-c7d5-4225-9b8e-5a234d4dbcd1)  
(KB2675157)  
(Mírný)  
[Aplikace Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=a5ef0147-595e-43b5-819f-73780fcef10d)  
(KB2675157)  
(Mírný)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=734ff97a-7d72-4bfe-9557-7fac91902f8e)  
(KB2653956)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=c376fbdc-2289-47b6-950b-4e668cd3a390)  
(KB2656370)  
(Kritický)  
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c1338821-d8b2-4513-aa35-087323188509)  
(KB2656369)  
(Kritický)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=40b1ae34-28ad-41a0-88df-b905517e4acf)<sup>[1]</sup>
(KB2656368)  
(Kritický)
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
[**MS12-023**](http://go.microsoft.com/fwlink/?linkid=242739)
</td>
<td style="border:1px solid black;">
[**MS12-024**](http://go.microsoft.com/fwlink/?linkid=238623)
</td>
<td style="border:1px solid black;">
[**MS12-025**](http://go.microsoft.com/fwlink/?linkid=242032)
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
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
[Aplikace Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=f598cad1-4d1a-40ce-a016-bb58778d5dc0)  
(KB2675157)  
(Kritický)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=44284277-06a7-405d-9187-8f50a042604d)  
(KB2675157)  
(Kritický)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=51088164-13b7-4216-90f1-20c92c8b8ca9)  
(KB2675157)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c7683919-6d46-4b3e-aa98-1bef20141835)  
(KB2653956)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=c376fbdc-2289-47b6-950b-4e668cd3a390)  
(KB2656370)  
(Kritický)  
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8e1c10a1-9cb2-4815-8aa6-e401ced5df80)  
(KB2656374)  
(Kritický)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=40b1ae34-28ad-41a0-88df-b905517e4acf)<sup>[1]</sup>
(KB2656368)  
(Kritický)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Aplikace Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=2717a997-2066-4a83-ae9b-4611a0851101)  
(KB2675157)  
(Kritický)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=19684033-ddeb-464f-9a22-f580a9c19f8e)  
(KB2675157)  
(Kritický)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=bbb99aee-aadd-4ec7-9e27-91cb8d90803e)  
(KB2675157)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4d9f8a6e-17bd-4ed3-8bc7-d5e3b11ca12a)  
(KB2653956)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=c376fbdc-2289-47b6-950b-4e668cd3a390)  
(KB2656370)  
(Kritický)  
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8e1c10a1-9cb2-4815-8aa6-e401ced5df80)  
(KB2656374)  
(Kritický)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=40b1ae34-28ad-41a0-88df-b905517e4acf)<sup>[1]</sup>
(KB2656368)  
(Kritický)
</td>
</tr>
<tr>
<th colspan="4" style="border:1px solid black;">
Windows Server 2008
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS12-023**](http://go.microsoft.com/fwlink/?linkid=242739)
</td>
<td style="border:1px solid black;">
[**MS12-024**](http://go.microsoft.com/fwlink/?linkid=238623)
</td>
<td style="border:1px solid black;">
[**MS12-025**](http://go.microsoft.com/fwlink/?linkid=242032)
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
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 pro 32bitové systémy Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=3e361edd-234b-4053-aa49-278b9fde4d5c)\*\*  
(KB2675157)  
(Mírný)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=6eb6781e-7b38-4679-afbc-4e3bb5747fd8)\*\*  
(KB2675157)  
(Mírný)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=d34d7981-ed63-460d-95e4-e6da1ac41d2f)\*\*  
(KB2675157)  
(Mírný)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro 32bitové systémy Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c36c20f7-a742-4151-b8f2-85ef80479d06)\*  
(KB2653956)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=c376fbdc-2289-47b6-950b-4e668cd3a390)  
(KB2656370)  
(Kritický)  
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8e1c10a1-9cb2-4815-8aa6-e401ced5df80)  
(KB2656374)  
(Kritický)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=40b1ae34-28ad-41a0-88df-b905517e4acf)<sup>[1]</sup>
(KB2656368)  
(Kritický)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 pro systémy s procesorem x64 Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=60b76a3c-4530-4101-931f-45df621e1eed)\*\*  
(KB2675157)  
(Mírný)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=fd657467-a45c-4354-b947-3a3cceb9b690)\*\*  
(KB2675157)  
(Mírný)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=c9d773e9-6a2e-45db-8f30-7da0082d909c)\*\*  
(KB2675157)  
(Mírný)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=330cea47-221d-439e-b106-58a146fc28ee)\*  
(KB2653956)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=c376fbdc-2289-47b6-950b-4e668cd3a390)  
(KB2656370)  
(Kritický)  
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8e1c10a1-9cb2-4815-8aa6-e401ced5df80)  
(KB2656374)  
(Kritický)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=40b1ae34-28ad-41a0-88df-b905517e4acf)<sup>[1]</sup>
(KB2656368)  
(Kritický)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 pro systémy s procesorem Itanium Service Pack 2
</td>
<td style="border:1px solid black;">
[Aplikace Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=3235216f-497f-4934-81b8-1eb9929e98c9)  
(KB2675157)  
(Mírný)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=1ec74522-ec1e-4b3c-bfeb-6a505cc4f11a)  
(KB2653956)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=c376fbdc-2289-47b6-950b-4e668cd3a390)  
(KB2656370)  
(Kritický)  
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8e1c10a1-9cb2-4815-8aa6-e401ced5df80)  
(KB2656374)  
(Kritický)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=40b1ae34-28ad-41a0-88df-b905517e4acf)<sup>[1]</sup>
(KB2656368)  
(Kritický)
</td>
</tr>
<tr>
<th colspan="4" style="border:1px solid black;">
Windows 7
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS12-023**](http://go.microsoft.com/fwlink/?linkid=242739)
</td>
<td style="border:1px solid black;">
[**MS12-024**](http://go.microsoft.com/fwlink/?linkid=238623)
</td>
<td style="border:1px solid black;">
[**MS12-025**](http://go.microsoft.com/fwlink/?linkid=242032)
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
Windows 7 pro 32bitové systémy
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=9a58ca0b-fad7-418e-80ae-ca478168f887)  
(KB2675157)  
(Kritický)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=e6724be3-ff4b-4dea-95f3-0b13998b6758)  
(KB2675157)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows 7 pro 32bitové systémy](http://www.microsoft.com/downloads/details.aspx?familyid=ac183b66-0247-4ae5-bda0-e8d0070917c8)  
(KB2653956)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=c3f521a9-4dc8-46b7-a7f2-696b8759b398)  
(KB2656372)  
(Kritický)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=40b1ae34-28ad-41a0-88df-b905517e4acf)<sup>[1]</sup>
(KB2656368)  
(Kritický)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 7 pro 32bitové systémy Service Pack 1
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=9a58ca0b-fad7-418e-80ae-ca478168f887)  
(KB2675157)  
(Kritický)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=e6724be3-ff4b-4dea-95f3-0b13998b6758)  
(KB2675157)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows 7 pro 32bitové systémy Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=ac183b66-0247-4ae5-bda0-e8d0070917c8)  
(KB2653956)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=efccca8d-1371-4cda-96ab-ceef735742e2)  
(KB2656373)  
(Kritický)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=40b1ae34-28ad-41a0-88df-b905517e4acf)<sup>[1]</sup>
(KB2656368)  
(Kritický)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 pro systémy s procesorem x64
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=7215f707-c536-4d81-ad66-e7bff592e400)  
(KB2675157)  
(Kritický)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=0ff822d0-074a-409c-9174-8100618c6171)  
(KB2675157)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows 7 pro systémy s procesorem x64](http://www.microsoft.com/downloads/details.aspx?familyid=27226e64-266f-499e-8c57-866593fc3430)  
(KB2653956)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=c3f521a9-4dc8-46b7-a7f2-696b8759b398)  
(KB2656372)  
(Kritický)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=40b1ae34-28ad-41a0-88df-b905517e4acf)<sup>[1]</sup>
(KB2656368)  
(Kritický)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 7 pro systémy s procesorem x64 Service Pack 1
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=7215f707-c536-4d81-ad66-e7bff592e400)  
(KB2675157)  
(Kritický)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=0ff822d0-074a-409c-9174-8100618c6171)  
(KB2675157)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows 7 pro systémy s procesorem x64 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=27226e64-266f-499e-8c57-866593fc3430)  
(KB2653956)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=efccca8d-1371-4cda-96ab-ceef735742e2)  
(KB2656373)  
(Kritický)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=40b1ae34-28ad-41a0-88df-b905517e4acf)<sup>[1]</sup>
(KB2656368)  
(Kritický)
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
[**MS12-023**](http://go.microsoft.com/fwlink/?linkid=242739)
</td>
<td style="border:1px solid black;">
[**MS12-024**](http://go.microsoft.com/fwlink/?linkid=238623)
</td>
<td style="border:1px solid black;">
[**MS12-025**](http://go.microsoft.com/fwlink/?linkid=242032)
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
[**Kritický**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 pro systémy s procesorem x64
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=237d94e6-b9b9-4177-81fa-a67df2806b0e)\*\*  
(KB2675157)  
(Mírný)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=d002bfe4-10e9-46d3-a460-06d112201ca5)\*\*  
(KB2675157)  
(Mírný)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 pro systémy s procesorem x64[\*](http://www.microsoft.com/downloads/details.aspx?familyid=54db1495-31bb-4435-a442-74e484630b8a)  
(KB2653956)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=c3f521a9-4dc8-46b7-a7f2-696b8759b398)\*  
(KB2656372)  
(Kritický)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=40b1ae34-28ad-41a0-88df-b905517e4acf)<sup>[1]</sup>
(KB2656368)  
(Kritický)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 pro systémy s procesorem x64 Service Pack 1
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=237d94e6-b9b9-4177-81fa-a67df2806b0e)\*\*  
(KB2675157)  
(Mírný)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=d002bfe4-10e9-46d3-a460-06d112201ca5)\*\*  
(KB2675157)  
(Mírný)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem x64 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=54db1495-31bb-4435-a442-74e484630b8a)\*  
(KB2653956)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=efccca8d-1371-4cda-96ab-ceef735742e2)\*  
(KB2656373)  
(Kritický)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=40b1ae34-28ad-41a0-88df-b905517e4acf)\*<sup>[1]</sup>
(KB2656368)  
(Kritický)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 pro systémy s procesorem Itanium
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=7bdba902-0a6e-451e-a29b-6d0a03ff5664)  
(KB2675157)  
(Mírný)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=9a4115bf-028b-4dcc-8995-d3341fdf42f2)  
(KB2653956)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=c3f521a9-4dc8-46b7-a7f2-696b8759b398)  
(KB2656372)  
(Kritický)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=40b1ae34-28ad-41a0-88df-b905517e4acf)<sup>[1]</sup>
(KB2656368)  
(Kritický)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 pro systémy s procesorem Itanium Service Pack 1
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=7bdba902-0a6e-451e-a29b-6d0a03ff5664)  
(KB2675157)  
(Mírný)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem Itanium Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=9a4115bf-028b-4dcc-8995-d3341fdf42f2)  
(KB2653956)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=efccca8d-1371-4cda-96ab-ceef735742e2)  
(KB2656373)  
(Kritický)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=40b1ae34-28ad-41a0-88df-b905517e4acf)<sup>[1]</sup>
(KB2656368)  
(Kritický)
</td>
</tr>
</table>
<p></p>
 
**Poznámky k systémům Windows Server 2008 a Windows Server 2008 R2**

**\*Instalace Server Core obsahující chybu zabezpečení** Tato aktualizace se stejným hodnocením závažnosti se vztahuje k podporovaným edicím systému Windows Server 2008 nebo Windows Server 2008 R2, jak je uvedeno, s instalací pomocí volby pro instalaci Server Core nebo bez ní. Další informace o této možnosti instalace naleznete v článcích na webu TechNet [Managing a Server Core Installation](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) (Správa instalace Server Core) a [Servicing a Server Core Installation](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx) (Obsluha instalace Server Core). Možnost instalace Server Core se nevztahuje na určité edice systému Windows Server 2008 a Windows Server 2008 R2; další informace naleznete v části [Porovnání možností instalace Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**\*\*Instalace Server Core neobsahující chybu zabezpečení** Chyby zabezpečení, které tato aktualizace řeší, nemají vliv na podporované edice systému Windows Server 2008 nebo Windows Server 2008 R2, jak je uvedeno, v případě instalace s využitím možnosti instalace Server Core. Další informace o této možnosti instalace naleznete v článcích na webu TechNet [Managing a Server Core Installation](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) (Správa instalace Server Core) a [Servicing a Server Core Installation](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx) (Obsluha instalace Server Core). Možnost instalace Server Core se nevztahuje na určité edice systému Windows Server 2008 a Windows Server 2008 R2; další informace naleznete v části [Porovnání možností instalace Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**Poznámka** **k bulletinu** **MS12-025**

<sup>[1]</sup>**Postižena jsou rozhraní .NET Framework 4 a .NET Framework 4 Client Profile.** Distribuční balíčky rozhraní .NET Framework verze 4 jsou k dispozici ve dvou profilech: .NET Framework 4 a .NET Framework 4 Client Profile. Rozhraní .NET Framework 4 Client Profile je verzí rozhraní .NET Framework 4. Chyba zabezpečení řešená v této aktualizaci se týká jak rozhraní .NET Framework 4, tak rozhraní .NET Framework 4 Client Profile. Další informace získáte v článku [Instalace rozhraní .NET Framework](http://msdn.microsoft.com/en-us/library/5a4x27ek.aspx) na webu MSDN.

#### Sady Microsoft Office a jejich software

 
<p></p>
<table style="border:1px solid black;">
<tr>
<th colspan="3" style="border:1px solid black;">
Sady Microsoft Office a jejich komponenty
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS12-027**](http://go.microsoft.com/fwlink/?linkid=246275)
</td>
<td style="border:1px solid black;">
[**MS12-028**](http://go.microsoft.com/fwlink/?linkid=232498)
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
Microsoft Office 2003 Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Office 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=d0d34b4f-4bcd-4df7-8ebc-87367e889959)  
(Běžné ovládací prvky systému Windows)  
(KB2597112)  
(Kritický)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2007 Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft Office 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=17294713-5c03-4439-bcae-471e9b1e1ac9)  
(Běžné ovládací prvky systému Windows)  
(KB2598041)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=fbf24cc6-89e1-48dd-bb83-23eed30195e1)  
(KB2596871)  
(Vysoký)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2007 Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Office 2007 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=17294713-5c03-4439-bcae-471e9b1e1ac9)  
(Běžné ovládací prvky systému Windows)  
(KB2598041)  
(Kritický)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2010 (32bitové edice)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2010 (32bitové edice)](http://www.microsoft.com/downloads/details.aspx?familyid=23c9d7bf-c9e0-4e01-8b66-da542332a28b)  
(Běžné ovládací prvky systému Windows)  
(KB2598039)  
(Kritický)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2010 Service Pack 1 (32bitové edice)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2010 Service Pack 1 (32bitové edice)](http://www.microsoft.com/downloads/details.aspx?familyid=23c9d7bf-c9e0-4e01-8b66-da542332a28b)  
(Běžné ovládací prvky systému Windows)  
(KB2598039)  
(Kritický)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
</tr>
<tr>
<th colspan="3" style="border:1px solid black;">
Microsoft Office Web Components
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS12-027**](http://go.microsoft.com/fwlink/?linkid=246275)
</td>
<td style="border:1px solid black;">
[**MS12-028**](http://go.microsoft.com/fwlink/?linkid=232498)
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
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2003 Web Components Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Office 2003 Web Components Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=d0d34b4f-4bcd-4df7-8ebc-87367e889959)  
(Běžné ovládací prvky systému Windows)  
(KB2597112)  
(Kritický)
</td>
<td style="border:1px solid black;">
Netýká se
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
[**MS12-027**](http://go.microsoft.com/fwlink/?linkid=246275)
</td>
<td style="border:1px solid black;">
[**MS12-028**](http://go.microsoft.com/fwlink/?linkid=232498)
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
Microsoft Works 9
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Microsoft Works 9](http://www.microsoft.com/downloads/details.aspx?familyid=94e17a66-cf09-4314-89ec-53deadabfa66)  
(KB2680317)  
(Vysoký)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Převaděč souborů sady Microsoft Works 6–9
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Převaděč souborů sady Microsoft Works 6–9](http://www.microsoft.com/downloads/details.aspx?familyid=4605f684-6314-4758-adeb-2a8810dfc8d1)  
(KB2680326)  
(Vysoký)
</td>
</tr>
</table>
<p></p>
 
**Poznámka k bulletinu MS12-027**

Více aktualizovaných souborů v rámci stejného identifikátoru bulletinu naleznete také v dalších kategoriích softwaru v rámci této části **Software obsahující tuto chybu a umístění aktualizací ke stažení**. Tento bulletin se vztahuje na více kategorií softwaru.

#### Microsoft Server Software

 
<p></p>
<table style="border:1px solid black;">
<tr>
<th colspan="2" style="border:1px solid black;">
Microsoft SQL Server
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS12-027**](http://go.microsoft.com/fwlink/?linkid=246275)
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
Microsoft SQL Server 2000 Service Pack 4
</td>
<td style="border:1px solid black;">
[Microsoft SQL Server 2000 Analysis Services Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=198f1819-818b-4b2e-a424-4a45729746eb)  
(KB983807)  
(Kritický)  
Aktualizace GDR:  
[Microsoft SQL Server 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=2a9d97e8-79e0-4997-88fe-1224707e1b37)  
(KB983808)  
(Kritický)  
Aktualizace QFE:  
[Microsoft SQL Server 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=8d0cac2f-f227-4e00-9454-4df62be86407)  
(KB983809)  
(Kritický)
</td>
</tr>
<tr>
<th colspan="2" style="border:1px solid black;">
Komponenty Microsoft SQL Server
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft SQL Server 2005 pro 32bitové systémy Service Pack 4
</td>
<td style="border:1px solid black;">
[Microsoft SQL Server 2005 pro 32bitové systémy Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=d0d34b4f-4bcd-4df7-8ebc-87367e889959)<sup>[1]</sup>
(Běžné ovládací prvky systému Windows)  
(KB2597112)  
(Kritický)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft SQL Server 2005 pro systémy s procesorem Itanium Service Pack 4
</td>
<td style="border:1px solid black;">
[Microsoft SQL Server 2005 pro systémy s procesorem Itanium Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=d0d34b4f-4bcd-4df7-8ebc-87367e889959)<sup>[1]</sup>
(Běžné ovládací prvky systému Windows)  
(KB2597112)  
(Kritický)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft SQL Server 2005 pro systémy s procesorem x64 Service Pack 4
</td>
<td style="border:1px solid black;">
[Microsoft SQL Server 2005 pro systémy s procesorem x64 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=d0d34b4f-4bcd-4df7-8ebc-87367e889959)<sup>[1]</sup>
(Běžné ovládací prvky systému Windows)  
(KB2597112)  
(Kritický)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft SQL Server 2005 Express Edition se službou Advanced Services Service Pack 4
</td>
<td style="border:1px solid black;">
[Microsoft SQL Server 2005 Express Edition se službou Advanced Services Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=d0d34b4f-4bcd-4df7-8ebc-87367e889959)<sup>[1]</sup>
(Běžné ovládací prvky systému Windows)  
(KB2597112)  
(Kritický)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft SQL Server 2008 pro 32bitové systémy Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft SQL Server 2008 pro 32bitové systémy Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=17294713-5c03-4439-bcae-471e9b1e1ac9)<sup>[2]</sup>
(Běžné ovládací prvky systému Windows)  
(KB2598041)  
(Kritický)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft SQL Server 2008 pro 32bitové systémy Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft SQL Server 2008 pro 32bitové systémy Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=17294713-5c03-4439-bcae-471e9b1e1ac9)<sup>[2]</sup>
(Běžné ovládací prvky systému Windows)  
(KB2598041)  
(Kritický)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft SQL Server 2008 pro systémy s procesorem x64 Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft SQL Server 2008 pro systémy s procesorem x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=17294713-5c03-4439-bcae-471e9b1e1ac9)<sup>[2]</sup>
(Běžné ovládací prvky systému Windows)  
(KB2598041)  
(Kritický)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft SQL Server 2008 pro systémy s procesorem x64 Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft SQL Server 2008 pro systémy s procesorem x64 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=17294713-5c03-4439-bcae-471e9b1e1ac9)<sup>[2]</sup>
(Běžné ovládací prvky systému Windows)  
(KB2598041)  
(Kritický)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft SQL Server 2008 pro systémy s procesorem Itanium Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft SQL Server 2008 pro systémy s procesorem Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=17294713-5c03-4439-bcae-471e9b1e1ac9)<sup>[2]</sup>
(Běžné ovládací prvky systému Windows)  
(KB2598041)  
(Kritický)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft SQL Server 2008 pro systémy s procesorem Itanium Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft SQL Server 2008 pro systémy s procesorem Itanium Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=17294713-5c03-4439-bcae-471e9b1e1ac9)<sup>[2]</sup>
(Běžné ovládací prvky systému Windows)  
(KB2598041)  
(Kritický)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft SQL Server 2008 R2 pro 32bitové systémy
</td>
<td style="border:1px solid black;">
[Microsoft SQL Server 2008 R2 pro 32bitové systémy](http://www.microsoft.com/downloads/details.aspx?familyid=17294713-5c03-4439-bcae-471e9b1e1ac9)<sup>[2]</sup>
(Běžné ovládací prvky systému Windows)  
(KB2598041)  
(Kritický)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft SQL Server 2008 R2 pro 32bitové systémy Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft SQL Server 2008 R2 pro 32bitové systémy Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=17294713-5c03-4439-bcae-471e9b1e1ac9)<sup>[2]</sup>
(Běžné ovládací prvky systému Windows)  
(KB2598041)  
(Kritický)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft SQL Server 2008 R2 pro systémy s procesorem x64
</td>
<td style="border:1px solid black;">
[Microsoft SQL Server 2008 R2 pro systémy s procesorem x64](http://www.microsoft.com/downloads/details.aspx?familyid=17294713-5c03-4439-bcae-471e9b1e1ac9)<sup>[2]</sup>
(Běžné ovládací prvky systému Windows)  
(KB2598041)  
(Kritický)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft SQL Server 2008 R2 pro systémy s procesorem x64 Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft SQL Server 2008 R2 pro systémy s procesorem x64 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=17294713-5c03-4439-bcae-471e9b1e1ac9)<sup>[2]</sup>
(Běžné ovládací prvky systému Windows)  
(KB2598041)  
(Kritický)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft SQL Server 2008 R2 pro systémy s procesorem Itanium
</td>
<td style="border:1px solid black;">
[Microsoft SQL Server 2008 R2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=17294713-5c03-4439-bcae-471e9b1e1ac9)<sup>[2]</sup>
(Běžné ovládací prvky systému Windows)  
(KB2598041)  
(Kritický)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft SQL Server 2008 R2 pro systémy s procesorem Itanium Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft SQL Server 2008 R2 pro systémy s procesorem Itanium Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=17294713-5c03-4439-bcae-471e9b1e1ac9)<sup>[2]</sup>
(Běžné ovládací prvky systému Windows)  
(KB2598041)  
(Kritický)
</td>
</tr>
</table>
<p></p>
 
**Poznámky** **k bulletinu** **MS12-027**

<sup>[1]</sup>Tato aktualizace je totožná s aktualizací KB2597112 pro systém Microsoft Office 2003

<sup>[2]</sup>Tato aktualizace je totožná s aktualizací KB2598041 pro systém Microsoft Office 2007

Více aktualizovaných souborů v rámci stejného identifikátoru bulletinu naleznete také v dalších kategoriích softwaru v rámci této části **Software obsahující tuto chybu a umístění aktualizací ke stažení**. Tento bulletin se vztahuje na více kategorií softwaru.

 
<p></p>
<table style="border:1px solid black;">
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
[**MS12-027**](http://go.microsoft.com/fwlink/?linkid=246275)
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
Microsoft BizTalk Server 2002 Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft BizTalk Server 2002 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=d90b78d2-551b-499b-9bd2-85b40646dbc7)  
(KB2645025)  
(Kritický)
</td>
</tr>
<tr>
<th colspan="2" style="border:1px solid black;">
Microsoft Commerce Server
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS12-027**](http://go.microsoft.com/fwlink/?linkid=246275)
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
Microsoft Commerce Server 2002 Service Pack 4
</td>
<td style="border:1px solid black;">
[Microsoft Commerce Server 2002 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=35de8833-50ae-482d-aa07-497bf68fb38e)  
(KB2658674)  
(Kritický)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Commerce Server 2007 Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft Commerce Server 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3f04fb90-8f11-4392-a4bc-800903091f04)  
(KB2658677)  
(Kritický)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Commerce Server 2009
</td>
<td style="border:1px solid black;">
[Microsoft Commerce Server 2009](http://www.microsoft.com/downloads/details.aspx?familyid=a8998b6b-e9a4-457e-a34f-0458dda81f2f)  
(KB2655547)  
(Kritický)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Commerce Server 2009 R2
</td>
<td style="border:1px solid black;">
[Microsoft Commerce Server 2009 R2](http://www.microsoft.com/downloads/details.aspx?familyid=e9221811-8913-412b-ae04-21a55ce7c4c5)  
(KB2658676)  
(Kritický)
</td>
</tr>
</table>
<p></p>
 
**Poznámka k bulletinu MS12-027**

Více aktualizovaných souborů v rámci stejného identifikátoru bulletinu naleznete také v dalších kategoriích softwaru v rámci této části **Software obsahující tuto chybu a umístění aktualizací ke stažení**. Tento bulletin se vztahuje na více kategorií softwaru.

#### Vývojářské nástroje a software společnosti Microsoft

 
<p></p>
<table style="border:1px solid black;">
<tr>
<th colspan="2" style="border:1px solid black;">
Microsoft Visual FoxPro
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS12-027**](http://go.microsoft.com/fwlink/?linkid=246275)
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
Microsoft Visual FoxPro 8.0 Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft Visual FoxPro 8.0 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=3a7ff474-f1e0-4c86-9555-64e8e7357890)  
(KB2647488)  
(Kritický)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Visual FoxPro 9.0 Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft Visual FoxPro 9.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=53c0132e-7724-4e94-abe9-e79b76ce35d7)  
(KB2647490)  
(Kritický)
</td>
</tr>
<tr>
<th colspan="2" style="border:1px solid black;">
Visual Basic
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS12-027**](http://go.microsoft.com/fwlink/?linkid=246275)
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
Visual Basic 6.0 Runtime
</td>
<td style="border:1px solid black;">
[Visual Basic 6.0 Runtime](http://www.microsoft.com/downloads/details.aspx?familyid=0afe933a-1e62-45c4-910c-ea94b203df5a)  
(KB2641426)  
(Kritický)
</td>
</tr>
</table>
<p></p>
 
**Poznámka k bulletinu MS12-027**

Více aktualizovaných souborů v rámci stejného identifikátoru bulletinu naleznete také v dalších kategoriích softwaru v rámci této části **Software obsahující tuto chybu a umístění aktualizací ke stažení**. Tento bulletin se vztahuje na více kategorií softwaru.

#### Software společnosti Microsoft pro vzdálenný přístup

 
<p></p>
<table style="border:1px solid black;">
<tr>
<th colspan="2" style="border:1px solid black;">
Microsoft Forefront Unified Access Gateway
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS12-026**](http://go.microsoft.com/fwlink/?linkid=238519)
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
Microsoft Forefront Unified Access Gateway
</td>
<td style="border:1px solid black;">
[Microsoft Forefront Unified Access Gateway 2010 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=d4b4ecc4-8bc6-43d0-b872-93673e0d9a6f)<sup>[1]</sup>
(KB2649261)  
(Vysoký)  
[Microsoft Forefront Unified Access Gateway 2010 Service Pack 1 Update 1](http://www.microsoft.com/downloads/details.aspx?familyid=e0f9acab-bfb8-4758-b60d-64e68a84fba0)<sup>[1]</sup>
(KB2649262)  
(Vysoký)
</td>
</tr>
</table>
<p></p>
 
**Poznámka** **k bulletinu** **MS12-026**

<sup>[1]</sup>Tato aktualizace je dostupná pouze prostřednictvím webu služby Stažení softwaru.

Nástroje a doporučené postupy zjišťování a nasazení
---------------------------------------------------

 
**Centrum zabezpečení**

Umožňuje správu aktualizací softwaru a zabezpečení, které je třeba nainstalovat na servery, stolní počítače a přenosné počítače v organizaci. Další informace naleznete na webu [TechNet Update Management Center](http://go.microsoft.com/fwlink/?linkid=69903). Další informace o zabezpečení produktů společnosti Microsoft nabízí web [Centrum zabezpečení TechNet](http://go.microsoft.com/fwlink/?linkid=21171). Tyto informace lze také získat kliknutím na nabídku „Nejnovější aktualizace zabezpečení“ na webu [Zabezpečení doma](http://go.microsoft.com/fwlink/?linkid=85102).

Aktualizace zabezpečení jsou k dispozici na webu [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747) a [Windows Update](http://go.microsoft.com/fwlink/?linkid=21130). Aktualizace zabezpečení jsou také k dispozici na webu [služby Stažení softwaru](http://go.microsoft.com/fwlink/?linkid=21129). Nejsnadněji je naleznete hledáním podle klíčových slov aktualizace zabezpečení.

Zákazníkům systému Microsoft Office for Mac doporučujeme využít funkci Microsoft AutoUpdate for Mac, která udržuje software společnosti Microsoft v aktuálním stavu. Další informace o funkci Microsoft AutoUpdate for Mac naleznete na webu [Check for software updates automatically](http://mac2.microsoft.com/help/office/14/en-us/word/item/ffe35357-8f25-4df8-a0a3-c258526c64ea) (Automatická kontrola aktualizací softwaru).

Aktualizace zabezpečení lze stáhnout z katalogu služby [Microsoft Update Catalog](http://go.microsoft.com/fwlink/?linkid=96155). Služba Microsoft Update Catalog poskytuje katalog s možností vyhledávání obsahu dostupného prostřednictvím služeb Windows Update a Microsoft Update, včetně aktualizací zabezpečení, ovladačů a aktualizací Service Pack. Vyhledáváním pomocí čísla bulletinu zabezpečení (například MS07-036) můžete přidat všechny dostupné aktualizace do košíku (včetně různých jazykových verzí aktualizace) a stáhnout je do vybrané složky. Další informace o službě Microsoft Update Catalog najdete v části [Nejčastější dotazy týkající se služby Microsoft Update Catalog](http://go.microsoft.com/fwlink/?linkid=97900).

**Doporučené postupy zjišťování a instalace**

Společnost Microsoft poskytuje doporučené postupy zjišťování a nasazení aktualizací zabezpečení. Tyto dokumenty obsahují doporučení a informace, které mohou odborníkům v oblasti IT pomoci porozumět, jak se používají různé nástroje pro detekci a nasazení aktualizací zabezpečení. Další informace získáte v [článku 961747 znalostní báze Microsoft Knowledge Base](http://support.microsoft.com/kb/961747).

**Nástroj MBSA (Microsoft Baseline Security Analyzer)**

Pomocí nástroje Microsoft Baseline Security Analyzer (MBSA) mohou správci prohledávat místní i vzdálené systémy a zjistit tak, jestli v nich nechybí některé aktualizace zabezpečení nebo jestli v nastavení zabezpečení systému nedošlo k některým běžným chybám. Další informace o nástroji MBSA získáte na webu [Microsoft Baseline Security Analyzer](http://go.microsoft.com/fwlink/?linkid=21134).

**Služba Windows Server Update Services**

Pomocí služby Windows Server Update Services (WSUS) mohou správci systémů rychle a spolehlivě nasadit nejnovější důležité aktualizace zabezpečení pro systémy Microsoft Windows 2000 a novější, systém Office XP a novější, Exchange Server 2003 a SQL Server 2000 do systémů Microsoft Windows 2000 a novějších.

Další informace o způsobu instalace této aktualizace zabezpečení pomocí služby Windows Server Update Services získáte na webu služby [Windows Server Update Services](http://technet.microsoft.com/en-us/wsus/default.aspx).

**System Center Configuration Manager 2007**

Služba Software Update Management nástroje Configuration Manager 2007 zjednodušuje složitý proces doručení a správy aktualizací do IT systémů firmy. Pomocí nástroje Configuration Manager 2007 mohou správci informačních technologií doručit aktualizace produktů společnosti Microsoft do řady zařízení, včetně stolních počítačů, notebooků, serverů a mobilních zařízení.

Automatizované hodnocení chyb zabezpečení v nástroji Configuration Manager 2007 odhaluje potřebu aktualizací a hlášení doporučených postupů. Základem služby Software Update Management nástroje Configuration Manager 2007 jsou služby WSUS (Microsoft Windows Software Update Services). Jedná se o časem prověřenou infrastrukturu aktualizací známou správcům informačních technologií po celém světě. Další informace o tom, jak mohou správci používat nástroj Configuration Manager 2007 k nasazení aktualizací, naleznete na webových stránkách [Software Update Management](http://www.microsoft.com/systemcenter/en/us/configuration-manager/cm-software-update-management.aspx). Další informace o nástroji Configuration Manager naleznete na webových stránkách [System Center Configuration Manager](http://www.microsoft.com/systemcenter/en/us/configuration-manager.aspx).

**Systems Management Server 2003**

Microsoft Systems Management Server (SMS) představuje v rozlehlých sítích řešení pro správu aktualizací s rozsáhlými možnostmi konfigurace. Umožňuje správcům identifikovat počítače se systémem Windows, které vyžadují aktualizace zabezpečení, a provést řízenou instalaci těchto aktualizací v celé rozlehlé síti s minimálním dopadem na koncové uživatele.

**Poznámka:** Systems Management Server 2003 není od 12. ledna 2010 součástí tradiční podpory. Další informace o životním cyklu produktů naleznete na webu [Životní cyklus podpory produktů společnosti Microsoft](http://support.microsoft.com/common/international.aspx?rdpath=dm;en-us;lifecycle). K dispozici je nyní nová verze nástroje SMS, System Center Configuration Manager 2007 (viz výše uvedená část **System Center Configuration Manager 2007**).

Další informace o tom, jak mohou správci pomocí serveru SMS 2003 nasazovat aktualizace zabezpečení, naleznete na webových stránkách [Scénáře a postupy pro Microsoft Systems Management Server 2003: Distribuce softwaru a správa oprav](http://www.microsoft.com/downloads/en/details.aspx?familyid=32f2bb4c-42f8-4b8d-844f-2553fd78049f&displaylang=en). Další informace o serveru SMS naleznete na webových stránkách [Microsoft Systems Management Server TechCenter](http://technet.microsoft.com/en-us/systemcenter/bb545936.aspx).

**Poznámka:** Služba SMS pomocí modulu Microsoft Baseline Security Analyzer poskytuje rozsáhlou podporu při zjišťování a nasazení aktualizací bulletinu zabezpečení. Tyto nástroje nemusí některé softwarové aktualizace zjistit. V takovém případě mohou správci použít funkce serveru SMS a nasměrovat aktualizace do určitých systémů. Další informace o tomto postupu naleznete na webu [Nasazení aktualizací softwaru pomocí funkce Distribuce softwaru serveru SMS](http://go.microsoft.com/fwlink/?linkid=33341). Některé aktualizace zabezpečení vyžadují po restartování počítače oprávnění správce. Správci mohou k instalaci těchto aktualizací použít nástroj Elevated Rights Deployment Tool (k dispozici v sadě [SMS 2003 Administration Feature Pack](http://www.microsoft.com/downloads/en/details.aspx?familyid=7bd3a16e-1899-4e0b-bb99-1320e816167d&displaylang=en)).

**Nástroj Update Compatibility Evaluator a sada Application Compatibility Toolkit**

Aktualizace často zapisují do stejných souborů a nastavení registru požadovaných pro spouštění aplikací. To může způsobit nekompatibilitu a zvýšit dobu, po kterou trvá nasazení aktualizací zabezpečení. Testování a ověřování aktualizací systému Windows lze usnadnit pomocí součástí nástroje [Update Compatibility Evaluator](http://technet2.microsoft.com/windowsvista/en/library/4279e239-37a4-44aa-aec5-4e70fe39f9de1033.mspx?mfr=true), které jsou dodávány se sadou [Application Compatibility Toolkit](http://www.microsoft.com/downloads/details.aspx?familyid=24da89e9-b581-47b0-b45e-492dd6da2971&displaylang=en).

Sada Application Compatibility Toolkit (ACT) obsahuje nezbytné nástroje a dokumentaci pro posouzení a zmírnění problémů s kompatibilitou aplikací před nasazením systému Windows Vista, služby Windows Update, aktualizací zabezpečení společnosti Microsoft nebo nové verze aplikace Windows Internet Explorer ve vašem prostředí.

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

-   Aktualizace zabezpečení jsou k dispozici na webu [služby Stažení softwaru](http://go.microsoft.com/fwlink/?linkid=21129). Nejsnadněji je naleznete hledáním podle klíčových slov aktualizace zabezpečení.
-   Aktualizace pro klientské platformy jsou k dispozici na webu [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747).
-   Aktualizace zabezpečení nabízené tento měsíc na webu Windows Update jsou k dispozici na webu služby Stažení softwaru v souborech obrazu ISO disku CD s vydanými aktualizacemi zabezpečení a kritickými aktualizacemi. Další informace získáte v [článku 913086 znalostní báze Microsoft Knowledge Base](http://support.microsoft.com/kb/913086).

**Komunita odborníků v oblasti zabezpečení**

Na webu [IT Pro Security Community](http://go.microsoft.com/fwlink/?linkid=21164) se můžete naučit, jak zlepšit zabezpečení a optimalizovat infrastrukturu IT, a diskutovat s dalšími členy komunity odborníků o bezpečnostních tématech.

#### Poděkování

Společnost Microsoft tímto [děkuje](http://go.microsoft.com/fwlink/?linkid=21127) za spolupráci při ochraně zákazníků:

-   Uživateli linx2008 ze společnosti [AISec](http://www.aisec.cn/) za oznámení chyby popsané v bulletinu MS12-023.
-   Roelu Spilkerovi ze společnosti [TOPdesk](http://www.topdesk.com) za oznámení chyby popsané v bulletinu MS12-023.
-   Josemu Antoniu Vazquezi Gonzalezovi, spolupracujícímu se společností [VeriSign iDefense Labs](http://labs.idefense.com), za oznámení chyby popsané v bulletinu MS12-023.
-   Anonymnímu výzkumníkovi, spolupracujícímu s organizací [Zero Day Initiative](http://www.zerodayinitiative.com) společnosti [TippingPoint](http://www.tippingpoint.com), za oznámení chyby popsané v bulletinu MS12-023.
-   Anonymnímu výzkumníkovi, spolupracujícímu s organizací [Zero Day Initiative](http://www.zerodayinitiative.com) společnosti [TippingPoint](http://www.tippingpoint.com), za oznámení chyby popsané v bulletinu MS12-023.
-   Masatu Kinugawovi za spolupráci na prvcích rozšíření ochrany zahrnutých v bulletinu MS12-023.
-   Robertu Zackovi a Igoru Glucksmannovi ze společnosti [Avast Software](http://www.avast.com/) za oznámení chyby popsané v bulletinu MS12-024.
-   Vitaliji Toropovovi, spolupracujícímu se společností [VeriSign iDefense Labs](http://labs.idefense.com/), za oznámení chyby popsané v bulletinu MS12-025.
-   Shaunu Colleymu ze společnosti [IOActive, Ltd.](http://ioactive.co.uk/) za oznámení chyby popsané v bulletinu MS12-028.

#### Technická podpora

-   Uvedený software byl testován za účelem zjištění, kterých verzí se chyba týká. U dalších verzí skončila časově omezená podpora. Pokud chcete zjistit dobu, po kterou je pro určitou verzi softwaru poskytována podpora, navštivte web [Zásady poskytování technické podpory pro produkty společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=21742).
-   Řešení zabezpečení pro odborníky v oboru informačních technologií: [Řešení potíží a podpora zabezpečení na webu TechNet](http://technet.microsoft.com/security/bb980617.aspx)
-   Ochraňte svůj počítač se systémem Windows před hrozbou virů a malwaru: [Centrum pomoci o bezpečnosti a ochraně před viry](http://support.microsoft.com/contactus/cu_sc_virsec_master)
-   Místní podpora dostupná ve vaší zemi: [Mezinárodní podpora](http://support.microsoft.com/common/international.aspx)

#### Zřeknutí se záruky

Informace ve znalostní bázi Microsoft Knowledge Base jsou poskytovány tak, jak jsou, bez jakékoli záruky. Společnost Microsoft neposkytuje žádné záruky, výslovně uvedené či mlčky předpokládané, včetně záruk obchodovatelnosti a vhodnosti pro určitý účel. Společnost Microsoft ani její dodavatelé nenesou v žádném případě zodpovědnost za žádné škody, včetně přímých, nepřímých, náhodných či následných škod, ztráty zisku či zvláštních škod, a to ani v případě, že byli na možnost takových škod upozorněni. V některých zemích a právních řádech není dovoleno vyloučit nebo omezit odpovědnost, proto se výše uvedené omezení na vás nemusí vztahovat.

#### Revize

-   V1.0 (10. dubna 2012): Souhrnný bulletin byl publikován.
-   V2.0 (26. dubna 2012): Do části „Software obsahující tuto chybu“ bulletinu MS12-027 byly přidány verze Service Pack 1 serveru SQL Server 2008 R2. Dále bylo přidáno vysvětlení, že se aktualizace týká všech instalací serveru Microsoft SQL Server 2000 Analysis Services Service Pack 4, neboť verze QFE a GDR se netýkají tohoto produktu. Jedná se pouze o změny informací. Nebyly provedeny žádné změny souborů nebo logiky detekce aktualizace zabezpečení. Vzhledem k tomu, že aktualizace byly nabízeny od původního vydání správně, zákazníci, kteří již aktualizace v minulosti úspěšně nainstalovali, nemusejí podnikat žádná opatření.

*Built at 2014-04-18T01:50:00Z-07:00*
