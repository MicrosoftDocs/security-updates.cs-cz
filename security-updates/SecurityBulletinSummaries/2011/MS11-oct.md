---
TOCTitle: 'MS11-OCT'
Title: 'Souhrnný bulletin zabezpečení společnosti Microsoft, říjen 2011'
ms:assetid: 'ms11-oct'
ms:contentKeyID: 61224016
ms:mtpsurl: 'https://technet.microsoft.com/cs-CZ/library/ms11-oct(v=Security.10)'
---

 

Souhrnný bulletin zabezpečení společnosti Microsoft, říjen 2011
===============================================================

Publikováno: 11. října 2011 | Aktualizováno: 26. října 2011

**Verze:** 1.1

Tento souhrnný bulletin uvádí bulletiny zabezpečení vydané v říjnu 2011.

Spolu s vydáním bulletinů pro říjen 2011 nahrazuje tento souhrnný bulletin předběžné oznámení o bulletinech vydané 6. října 2011. Další informace o službě předběžného oznámení o bulletinech naleznete v části [Předběžné oznámení o bulletinech zabezpečení společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=217213).

Informace o tom, jak dostávat automatická oznámení o vydání nových bulletinů zabezpečení společnosti Microsoft, naleznete na webu [Zasílání technických oznámení o zabezpečení společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=21163).

Pro zodpovězení zákaznických dotazů týkajících se těchto bulletinů uspořádá společnost Microsoft webové vysílání 12. října 2011 v 11:00 časového pásma Tichomoří (USA a Kanada). [Zaregistrujte se pro webové vysílání týkající se říjnových bulletinů zabezpečení](https://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032487956). Po tomto datu je webové vysílání dostupné na požádání. Další informace získáte v [souhrnných bulletinech zabezpečení společnosti Microsoft a webovém vysílání](http://go.microsoft.com/fwlink/?linkid=217214).

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
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=227075">MS11-078</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení v rozhraní .NET Framework a programu Microsoft Silverlight umožňuje vzdálené spuštění kódu (2604930)</strong><br />
<br />
Tato aktualizace zabezpečení řeší soukromou osobou oznámenou chybu zabezpečení rozhraní Microsoft .NET Framework a programu Microsoft Silverlight. Tato chyba zabezpečení by mohla umožnit vzdálené spuštění kódu v klientském systému, pokud by uživatel zobrazil speciálně vytvořenou webovou stránku pomocí webového prohlížeče, v němž lze otevírat aplikace prohlížeče XAML (XBAP) nebo Silverlight. Uživatelé, jejichž účty jsou konfigurovány tak, aby měli v systému méně uživatelských práv, by byli vystaveni menšímu riziku než uživatelé s uživatelskými právy správce. Chyba zabezpečení dále může umožnit vzdálené spuštění kódu na serverovém systému se službou IIS v případě, že tento server umožňuje zpracování stránek ASP.NET a útočníkovi se úspěšně podaří na daném serveru načíst speciálně vytvořenou stránku ASP.NET a poté ji spustit, jako například v případě hostování webu. Tuto chybu zabezpečení mohou zneužít také aplikace Windows .NET k obejití omezení zabezpečení přístupu kódu (CAS).</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritický</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Může vyžadovat restartování</td>
<td style="border:1px solid black;">Microsoft .NET Framework, Microsoft Silverlight</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=226382">MS11-081</a></td>
<td style="border:1px solid black;"><strong>Kumulativní aktualizace zabezpečení pro aplikaci Internet Explorer (2586448)</strong><br />
<br />
Tato aktualizace zabezpečení řeší osm soukromě oznámených chyb zabezpečení aplikace Internet Explorer. Nejzávažnější chyby zabezpečení mohou umožnit vzdálené spuštění kódu, pokud uživatel pomocí aplikace Internet Explorer zobrazí speciálně vytvořenou webovou stránku. Útočník, který by úspěšně zneužil některou z těchto chyb zabezpečení, by mohl získat stejná uživatelská práva, jaká má místní uživatel. Uživatelé, jejichž účty jsou konfigurovány tak, aby měli v systému méně uživatelských práv, by byli vystaveni menšímu riziku než uživatelé s uživatelskými právy správce.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritický</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Internet Explorer</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=221538">MS11-075</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení technologie MSAA (Microsoft Active Accessibility) umožňuje vzdálené spuštění kódu (2623699)</strong><br />
<br />
Tato aktualizace zabezpečení řeší chybu zabezpečení v součásti MSAA (Microsoft Active Accessibility) oznámenou soukromou osobou. Chyba zabezpečení by mohla umožnit vzdálené spuštění kódu, pokud útočník přesvědčí uživatele, aby otevřel legitimní soubor umístěný ve stejném síťovém adresáři jako speciálně vytvořený soubor knihovny DLL. Součást MSAA (Microsoft Active Accessibility) by se poté při otevírání tohoto legitimního souboru mohla pokusit o načtení souboru DLL a o spuštění jakéhokoli v něm obsaženého kódu. Úspěšný útok by vyžadoval, aby útočník navštívil nedůvěryhodné systémové umístění vzdáleného souboru nebo sdílenou složku protokolu WebDAV a otevřel z tohoto umístění dokument, který by pak načetla aplikace obsahující chybu zabezpečení.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Vysoký</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=227073">MS11-076</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení programu Windows Media Center umožňuje vzdálené spuštění kódu (2604926)</strong><br />
<br />
Tato aktualizace zabezpečení řeší veřejně známou chybu zabezpečení programu Windows Media Center. Chyba zabezpečení by mohla umožnit vzdálené spuštění kódu, pokud útočník přesvědčí uživatele, aby otevřel legitimní soubor umístěný ve stejném síťovém adresáři jako speciálně vytvořený soubor knihovny DLL. Program Windows Media Center by se poté při otevírání tohoto legitimního souboru mohl pokusit o načtení souboru DLL a o spuštění jakéhokoli v něm obsaženého kódu. Úspěšný útok by vyžadoval, aby uživatel navštívil umístění v nedůvěryhodném vzdáleném systému souborů nebo nedůvěryhodnou sdílenou složku protokolu WebDAV a otevřel legitimní soubor z tohoto umístění.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Vysoký</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Může vyžadovat restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=225915">MS11-077</a></td>
<td style="border:1px solid black;"><strong>Chyby zabezpečení v ovladačích režimu jádra systému Windows umožňují vzdálené spuštění kódu (2567053)</strong><br />
<br />
Tato aktualizace zabezpečení řeší čtyři soukromými osobami oznámené chyby zabezpečení v systému Microsoft Windows. Nejzávažnější z těchto chyb zabezpečení by mohla způsobit vzdálené spuštění kódu, pokud by uživatel otevřel speciálně vytvořený soubor písma (např. soubor FON) ve sdílené síťové složce, umístění UNC či WebDAV nebo v e-mailové příloze. Úspěšný útok by vyžadoval, aby uživatel navštívil umístění v nedůvěryhodném vzdáleném systému souborů nebo nedůvěryhodnou sdílenou složku protokolu WebDAV a otevřel speciálně vytvořený soubor písma, případně aby tento soubor otevřel jako e-mailovou přílohu.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Vysoký</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217472">MS11-079</a></td>
<td style="border:1px solid black;"><strong>Chyby zabezpečení v aplikaci Microsoft Forefront Unified Access Gateway umožňují vzdálené spuštění kódu (2544641)</strong><br />
<br />
Tato aktualizace zabezpečení řeší pět chyb zabezpečení aplikace Forefront Unified Access Gateway (UAG) oznámených soukromými osobami. Nejzávažnější z těchto chyb zabezpečení by mohla způsobit vzdálené spuštění kódu, pokud by uživatel navštívil postižený web prostřednictvím speciálně vytvořené adresy URL. Útočník však nemůže žádným způsobem přinutit uživatele k návštěvě takového webu. Místo toho by útočník musel přesvědčit uživatele, aby navštívili takový web. K tomu se obvykle používá odkaz v e-mailu nebo zpráva programu pro zasílání rychlých zpráv, na kterou uživatelé kliknou, a přejdou tak na útočníkův web.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Vysoký</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Může vyžadovat restartování</td>
<td style="border:1px solid black;">Microsoft Forefront Unified Access Gateway</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=227486">MS11-080</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení v ovladači pomocných funkcí Ancillary Function Driver umožňuje zvýšení úrovně oprávnění (2592799)</strong><br />
<br />
Tato aktualizace zabezpečení řeší chybu zabezpečení v ovladači Microsoft Windows Ancillary Function Driver (AFD), kterou oznámila soukromá osoba. Tato chyba zabezpečení by mohla způsobit zvýšení úrovně oprávnění, pokud by se útočník přihlásil k systému uživatele a spustil speciálně vytvořenou aplikaci. Tuto chybu může zneužít pouze útočník s platnými pověřeními pro přihlášení, která by mu umožňovala se místně přihlásit.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Vysoký</a><br />
Zvýšení úrovně oprávnění</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=228596">MS11-082</a></td>
<td style="border:1px solid black;"><strong>Chyby zabezpečení na serveru Host Integration Server umožňují odmítnutí služby (2607670)</strong><br />
<br />
Tato aktualizace zabezpečení řeší dvě veřejně známé chyby zabezpečení na serveru Host Integration Server. Tyto chyby zabezpečení by mohly způsobit odmítnutí služby, pokud vzdálený útočník odešle na Host Integration Server, naslouchající na portu UDP 1478 nebo portech TCP 1477 a 1478, speciálně vytvořené pakety. Doporučené postupy pro používání brány firewall a standardní konfigurace této brány zajišťují ochranu sítí před útoky pocházejícími z oblasti mimo rozlehlou síť. Je vhodné, aby systémy připojené k Internetu měly přístupný minimální počet portů. V tomto případě by měly být porty serveru Host Integration Server zablokovány vůči Internetu.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Vysoký</a><br />
Odmítnutí služby</td>
<td style="border:1px solid black;">Může vyžadovat restartování</td>
<td style="border:1px solid black;">Microsoft Host Integration Server</td>
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

 
<p></p>
<table style="border:1px solid black;">
<thead>
<tr class="header">
<th style="border:1px solid black;" >ID bulletinu</th>
<th style="border:1px solid black;" >Název chyby zabezpečení</th>
<th style="border:1px solid black;" >ID CVE</th>
<th style="border:1px solid black;" >Hodnocení zneužitelnosti spuštění kódu u nejnovějšího vydání softwaru</th>
<th style="border:1px solid black;" >Hodnocení zneužitelnosti spuštění kódu u starších vydání softwaru</th>
<th style="border:1px solid black;" >Hodnocení zneužitelnosti odmítnutí služby</th>
<th style="border:1px solid black;" >Hlavní poznámky</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=221538">MS11-075</a></td>
<td style="border:1px solid black;">Chyba zabezpečení nezabezpečeného načítání knihovny v technologii Active Accessibility</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1247">CVE-2011-1247</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">2</a> – Je pravděpodobné vytvoření kódu nekonsistentního zneužití</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;">Netýká se</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=227073">MS11-076</a></td>
<td style="border:1px solid black;">Chyba zabezpečení nezabezpečeného načítání knihovny v programu Media Center</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-2009">CVE-2011-2009</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;">Netýká se</td>
<td style="border:1px solid black;">Tato chyba zabezpečení je veřejně známá.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=225915">MS11-077</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se vyhodnocování ukazatele Win32k Null</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1985">CVE-2011-1985</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;">Trvalé</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=225915">MS11-077</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se přetečení vyrovnávací paměti souboru knihovny fontů</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-2003">CVE-2011-2003</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;">Dočasné</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=225915">MS11-077</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se použití subsystému Win32k po uvolnění</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-2011">CVE-2011-2011</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">2</a> – Je pravděpodobné vytvoření kódu nekonsistentního zneužití</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">2</a> – Je pravděpodobné vytvoření kódu nekonsistentního zneužití</td>
<td style="border:1px solid black;">Trvalé</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=227075">MS11-078</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se dědičnosti tříd rozhraní .NET Framework</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1253">CVE-2011-1253</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">3</a> – Vytvoření funkčního zneužitelného kódu není pravděpodobné</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;">Netýká se</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217472">MS11-079</a></td>
<td style="border:1px solid black;">Chyba zabezpečení XSS týkající se rozdělování odezvy tabulky aplikace Excel</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1895">CVE-2011-1895</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;">Netýká se</td>
<td style="border:1px solid black;">Zpřístupnění informací na určitých platformách uvedených v bulletinu</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217472">MS11-079</a></td>
<td style="border:1px solid black;">Chyba zabezpečení XSS reflektování tabulky aplikace Excel</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1896">CVE-2011-1896</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;">Netýká se</td>
<td style="border:1px solid black;">Zpřístupnění informací na určitých platformách uvedených v bulletinu</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217472">MS11-079</a></td>
<td style="border:1px solid black;">Chyba zabezpečení XSS výchozího reflektování</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1897">CVE-2011-1897</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;">Netýká se</td>
<td style="border:1px solid black;">Zpřístupnění informací na určitých platformách uvedených v bulletinu</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217472">MS11-079</a></td>
<td style="border:1px solid black;">Chyba zabezpečení umožňující spuštění kódu ve formě Poisoned Cup</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1969">CVE-2011-1969</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;">Netýká se</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217472">MS11-079</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se selhání souboru cookie prázdné relace</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-2012">CVE-2011-2012</a></td>
<td style="border:1px solid black;">Žádné ohrožení</td>
<td style="border:1px solid black;">Žádné ohrožení</td>
<td style="border:1px solid black;">Trvalé</td>
<td style="border:1px solid black;">Jedná se o chybu zabezpečení, která způsobuje odmítnutí služby.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=227486">MS11-080</a></td>
<td style="border:1px solid black;">Chyba zabezpečení v pomocném ovladači umožňující zvýšení úrovně oprávnění</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-2005">CVE-2011-2005</a></td>
<td style="border:1px solid black;">Žádné ohrožení</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;">Netýká se</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=226382">MS11-081</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se události Scroll umožňující vzdálené spuštění kódu</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1993">CVE-2011-1993</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;">Dočasné</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=226382">MS11-081</a></td>
<td style="border:1px solid black;">Chyba zabezpečení souboru OLEAuto32.dll umožňující vzdálené spuštění kódu</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1995">CVE-2011-1995</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;">Dočasné</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=226382">MS11-081</a></td>
<td style="border:1px solid black;">Chyba zabezpečení volitelného elementu umožňující vzdálené spuštění kódu</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1996">CVE-2011-1996</a></td>
<td style="border:1px solid black;">Žádné ohrožení</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;">Dočasné</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=226382">MS11-081</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se události OnLoad umožňující vzdálené spuštění kódu</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1997">CVE-2011-1997</a></td>
<td style="border:1px solid black;">Žádné ohrožení</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;">Dočasné</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=226382">MS11-081</a></td>
<td style="border:1px solid black;">Chyba zabezpečení souboru Jscript9.dll umožňující vzdálené spuštění kódu</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1998">CVE-2011-1998</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;">Žádné ohrožení</td>
<td style="border:1px solid black;">Dočasné</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=226382">MS11-081</a></td>
<td style="border:1px solid black;">Chyba zabezpečení vybraného elementu umožňující vzdálené spuštění kódu</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1999">CVE-2011-1999</a></td>
<td style="border:1px solid black;">Žádné ohrožení</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">2</a> – Je pravděpodobné vytvoření kódu nekonsistentního zneužití</td>
<td style="border:1px solid black;">Dočasné</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=226382">MS11-081</a></td>
<td style="border:1px solid black;">Chyba zabezpečení základního elementu umožňující vzdálené spuštění kódu</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-2000">CVE-2011-2000</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;">Dočasné</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=226382">MS11-081</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se poškození tabulky virtuálních funkcí umožňující vzdálené spuštění kódu</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-2001">CVE-2011-2001</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;">Dočasné</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=228596">MS11-082</a></td>
<td style="border:1px solid black;">Chyba zabezpečení nekonečné smyčky v souboru snabase.exe způsobující odmítnutí služby</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-2007">CVE-2011-2007</a></td>
<td style="border:1px solid black;">Žádné ohrožení</td>
<td style="border:1px solid black;">Žádné ohrožení</td>
<td style="border:1px solid black;">Trvalé</td>
<td style="border:1px solid black;">Jedná se o chybu zabezpečení, která způsobuje odmítnutí služby.<br />
<br />
Tato chyba zabezpečení je veřejně známá.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=228596">MS11-082</a></td>
<td style="border:1px solid black;">Chyba zabezpečení přístupu k nepřidělené paměti způsobující odmítnutí služby</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-2008">CVE-2011-2008</a></td>
<td style="border:1px solid black;">Žádné ohrožení</td>
<td style="border:1px solid black;">Žádné ohrožení</td>
<td style="border:1px solid black;">Trvalé</td>
<td style="border:1px solid black;">Jedná se o chybu zabezpečení, která způsobuje odmítnutí služby.<br />
<br />
Tato chyba zabezpečení je veřejně známá.</td>
</tr>
</tbody>
</table>
<p></p>
 

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
</tr>
<tr>
<th colspan="7" style="border:1px solid black;">
Windows XP
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS11-078**](http://go.microsoft.com/fwlink/?linkid=227075)
</td>
<td style="border:1px solid black;">
[**MS11-081**](http://go.microsoft.com/fwlink/?linkid=226382)
</td>
<td style="border:1px solid black;">
[**MS11-075**](http://go.microsoft.com/fwlink/?linkid=221538)
</td>
<td style="border:1px solid black;">
[**MS11-076**](http://go.microsoft.com/fwlink/?linkid=227073)
</td>
<td style="border:1px solid black;">
[**MS11-077**](http://go.microsoft.com/fwlink/?linkid=225915)
</td>
<td style="border:1px solid black;">
[**MS11-080**](http://go.microsoft.com/fwlink/?linkid=227486)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Celkový stupeň** **závažnosti**
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
[Microsoft .NET Framework 1.0 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=a54a7ad5-0504-4cc6-9eca-ba9f31c35a17)  
(KB2572066)  
(pouze Media Center Edition 2005 a Tablet PC Edition 2005)  
(Kritický)  
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=6100e577-deb5-4395-b851-e19e0ca79507)  
(KB2572067)  
(Kritický)  
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=719b3da5-52ca-4d56-a2c5-69711039e59d)  
(KB2572073)  
(Kritický)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=770e7b58-6544-4f59-9893-b3eadf6d6c8a)<sup>[1]</sup>
(KB2572078)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Aplikace Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=822f91f5-bf92-42c4-ad33-b971be37d772)  
(Kritický)  
[Aplikace Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=e942554d-6cb6-4e48-a876-3470671a95a2)  
(Kritický)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=a911b5b0-5e46-4a37-83e7-595e20585c56)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=96af60b9-4b8d-4a9b-b125-10775bb48252)  
(KB2564958)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=9157e677-ab3f-44b0-9735-192bc7421ba7)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=f1b2dceb-5bef-4522-9001-8dff0545d805)  
(Vysoký)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=6100e577-deb5-4395-b851-e19e0ca79507)  
(KB2572067)  
(Kritický)  
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=719b3da5-52ca-4d56-a2c5-69711039e59d)  
(KB2572073)  
(Kritický)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=770e7b58-6544-4f59-9893-b3eadf6d6c8a)<sup>[1]</sup>
(KB2572078)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Aplikace Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=6260318c-e579-4cdf-93e3-4608892bc79e)  
(Kritický)  
[Aplikace Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=f04ad852-1418-4fc4-bd57-f47895bbf3a8)  
(Kritický)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=67ebf641-1341-4642-96ba-bab5446d7b5d)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c8fcf427-17d0-4caa-b406-50703f980862)  
(KB2564958)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=0f2444ac-61bd-47cf-9c1e-da86a2b0cfb5)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=9a37864e-8543-4c52-aa73-e3c190860d76)  
(Vysoký)
</td>
</tr>
<tr>
<th colspan="7" style="border:1px solid black;">
Windows Server 2003
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS11-078**](http://go.microsoft.com/fwlink/?linkid=227075)
</td>
<td style="border:1px solid black;">
[**MS11-081**](http://go.microsoft.com/fwlink/?linkid=226382)
</td>
<td style="border:1px solid black;">
[**MS11-075**](http://go.microsoft.com/fwlink/?linkid=221538)
</td>
<td style="border:1px solid black;">
[**MS11-076**](http://go.microsoft.com/fwlink/?linkid=227073)
</td>
<td style="border:1px solid black;">
[**MS11-077**](http://go.microsoft.com/fwlink/?linkid=225915)
</td>
<td style="border:1px solid black;">
[**MS11-080**](http://go.microsoft.com/fwlink/?linkid=227486)
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
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
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
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=b968b0bd-577b-4ea2-a192-a80fe7c20791)  
(KB2572069)  
(Kritický)  
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=719b3da5-52ca-4d56-a2c5-69711039e59d)  
(KB2572073)  
(Kritický)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=770e7b58-6544-4f59-9893-b3eadf6d6c8a)<sup>[1]</sup>
(KB2572078)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Aplikace Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=172c55f3-6249-4ba3-a4a4-677a03262ff3)  
(Mírný)  
[Aplikace Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=6ffbdb93-7b92-4197-bb6c-5c305e8072a8)  
(Mírný)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=14ef20d4-3530-49b2-91b7-d278d9098023)  
(Mírný)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=09e178f8-2bd2-46e1-b975-4938ee1f304d)  
(KB2564958)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3bd62bf6-3400-4c03-95fe-148112b341e8)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=29228167-b811-43d7-b4a0-91e385b598a5)  
(Vysoký)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=6100e577-deb5-4395-b851-e19e0ca79507)  
(KB2572067)  
(Kritický)  
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=719b3da5-52ca-4d56-a2c5-69711039e59d)  
(KB2572073)  
(Kritický)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=770e7b58-6544-4f59-9893-b3eadf6d6c8a)<sup>[1]</sup>
(KB2572078)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Aplikace Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=f5a0a8db-34d4-4f0a-ab6b-7b2fb420ab91)  
(Mírný)  
[Aplikace Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=7379b3bf-6af0-43cb-bf8b-505e8563fc84)  
(Mírný)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=b35c95f5-30b0-43a9-aa6a-6db63cab0dcb)  
(Mírný)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=9b8030db-1f47-4666-8cb5-1c56577f2340)  
(KB2564958)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b73f4e87-9655-46d5-beb2-ea245dcd280d)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=0816d729-6769-4ca6-a14e-71750eca8d29)  
(Vysoký)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 SP2 pro systémy s procesorem Itanium
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=6100e577-deb5-4395-b851-e19e0ca79507)  
(KB2572067)  
(Kritický)  
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=719b3da5-52ca-4d56-a2c5-69711039e59d)  
(KB2572073)  
(Kritický)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=770e7b58-6544-4f59-9893-b3eadf6d6c8a)<sup>[1]</sup>
(KB2572078)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Aplikace Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=5825cb4a-47d5-423f-b4c5-2d0fc50856c0)  
(Mírný)  
[Aplikace Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=11c4878e-df58-4369-b9c0-cb0a230c92dd)  
(Mírný)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=82653b8c-0e58-440d-9702-8847f599caed)  
(KB2605295)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=a618cc19-5ebc-462e-a518-d9bfe41ed98e)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=42465652-2664-4fd5-9a22-ae847b08e7c8)  
(Vysoký)
</td>
</tr>
<tr>
<th colspan="7" style="border:1px solid black;">
Windows Vista
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS11-078**](http://go.microsoft.com/fwlink/?linkid=227075)
</td>
<td style="border:1px solid black;">
[**MS11-081**](http://go.microsoft.com/fwlink/?linkid=226382)
</td>
<td style="border:1px solid black;">
[**MS11-075**](http://go.microsoft.com/fwlink/?linkid=221538)
</td>
<td style="border:1px solid black;">
[**MS11-076**](http://go.microsoft.com/fwlink/?linkid=227073)
</td>
<td style="border:1px solid black;">
[**MS11-077**](http://go.microsoft.com/fwlink/?linkid=225915)
</td>
<td style="border:1px solid black;">
[**MS11-080**](http://go.microsoft.com/fwlink/?linkid=227486)
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
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Žádný
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=6100e577-deb5-4395-b851-e19e0ca79507)  
(KB2572067)  
(Kritický)  
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7c27128d-eaf9-4416-b8b1-9edab9102feb)  
(KB2572075)  
(Kritický)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=770e7b58-6544-4f59-9893-b3eadf6d6c8a)<sup>[1]</sup>
(KB2572078)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Aplikace Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=630335ac-5a30-46b4-acc1-c4d8bd289668)  
(Kritický)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=76c8124e-81b9-4a6a-bd53-fbdaf45189aa)  
(Kritický)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=7de276a3-a20d-49de-82b0-51cb22ad73af)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=96b089c0-a2e7-44cb-9fc4-9569b3993afa)  
(KB2564958)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=44f7f10b-86ff-470f-996a-d4aa51c4d18f)  
(KB2579686)  
(Vysoký)  
[Sada programu Windows Media Center TV pro systém Windows Vista (32bitové edice)](http://www.microsoft.com/downloads/details.aspx?familyid=60e50f72-4001-423c-831c-8ff1f1b8f090)<sup>[1]</sup>
(KB2579692)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ff53d01b-97b7-40d2-af88-4978f1099a7c)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=6100e577-deb5-4395-b851-e19e0ca79507)  
(KB2572067)  
(Kritický)  
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7c27128d-eaf9-4416-b8b1-9edab9102feb)  
(KB2572075)  
(Kritický)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=770e7b58-6544-4f59-9893-b3eadf6d6c8a)<sup>[1]</sup>
(KB2572078)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Aplikace Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=9aabd7a2-0b2f-4c42-a9cf-2ec69ae6b82d)  
(Kritický)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=3454940c-acc2-4e09-8154-075b4be1b697)  
(Kritický)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=3df0c31b-344a-4163-93d2-79df1653b339)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b79a389c-8340-4dd2-9ab1-a0943c5a220f)  
(KB2564958)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=cbb66cd7-2688-410f-8a03-fd28e6ef5b01)  
(KB2579686)  
(Vysoký)  
[Sada programu Windows Media Center TV pro systém Windows Vista (64bitové edice)](http://www.microsoft.com/downloads/details.aspx?familyid=371c7dab-5aa6-4502-80ee-ae69b736b972)<sup>[1]</sup>
(KB2579692)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=47322e11-f1cf-4f70-b939-8cac9bbfc2bc)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
</tr>
<tr>
<th colspan="7" style="border:1px solid black;">
Windows Server 2008
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS11-078**](http://go.microsoft.com/fwlink/?linkid=227075)
</td>
<td style="border:1px solid black;">
[**MS11-081**](http://go.microsoft.com/fwlink/?linkid=226382)
</td>
<td style="border:1px solid black;">
[**MS11-075**](http://go.microsoft.com/fwlink/?linkid=221538)
</td>
<td style="border:1px solid black;">
[**MS11-076**](http://go.microsoft.com/fwlink/?linkid=227073)
</td>
<td style="border:1px solid black;">
[**MS11-077**](http://go.microsoft.com/fwlink/?linkid=225915)
</td>
<td style="border:1px solid black;">
[**MS11-080**](http://go.microsoft.com/fwlink/?linkid=227486)
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
[**Mírný**](http://go.microsoft.com/fwlink/?linkid=21140)
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
<td style="border:1px solid black;">
Žádný
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 pro 32bitové systémy Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=6100e577-deb5-4395-b851-e19e0ca79507)\*\*  
(KB2572067)  
(Kritický)  
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7c27128d-eaf9-4416-b8b1-9edab9102feb)\*\*  
(KB2572075)  
(Kritický)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=770e7b58-6544-4f59-9893-b3eadf6d6c8a)\*\*<sup>[1]</sup>
(KB2572078)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=5660e23c-13a3-4275-ac69-38f03f17491a)\*\*  
(Mírný)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=bd144435-1afd-4d6e-a100-fbd613eee409)\*\*  
(Mírný)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=1a7f9855-20ce-4fe0-a903-bd1f145075df)\*\*  
(Mírný)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro 32bitové systémy Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7cd1ecec-8a3f-4cb2-833c-a177c9602ff5)\*  
(KB2564958)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro 32bitové systémy Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7c7498ee-eba4-44fd-8846-0b2e96c96705)\*  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 pro systémy s procesorem x64 Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=6100e577-deb5-4395-b851-e19e0ca79507)\*\*  
(KB2572067)  
(Kritický)  
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7c27128d-eaf9-4416-b8b1-9edab9102feb)\*\*  
(KB2572075)  
(Kritický)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=770e7b58-6544-4f59-9893-b3eadf6d6c8a)\*\*<sup>[1]</sup>
(KB2572078)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=415b1c59-f3dc-4f4f-b2eb-68692d6efc05)\*\*  
(Mírný)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=b0c4949f-bce0-4255-a5f2-cf5ecf7416da)\*\*  
(Mírný)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=28a09e42-5865-48b2-af26-ebc8162c3286)\*\*  
(Mírný)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=456e450c-3928-4130-8127-e4d3f482c1ca)\*  
(KB2564958)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=40386742-f397-402e-8810-63d3d6ba12a6)\*  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 pro systémy s procesorem Itanium Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=6100e577-deb5-4395-b851-e19e0ca79507)  
(KB2572067)  
(Kritický)  
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7c27128d-eaf9-4416-b8b1-9edab9102feb)  
(KB2572075)  
(Kritický)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=770e7b58-6544-4f59-9893-b3eadf6d6c8a)<sup>[1]</sup>
(KB2572078)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Aplikace Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=31e68c7f-4db5-463f-a315-92f574af080b)  
(Mírný)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2e9930d3-ba13-446d-bfa0-60720c48203b)  
(KB2564958)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3633402b-96cb-4f36-b137-d07d1baf28c7)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
</tr>
<tr>
<th colspan="7" style="border:1px solid black;">
Windows 7
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS11-078**](http://go.microsoft.com/fwlink/?linkid=227075)
</td>
<td style="border:1px solid black;">
[**MS11-081**](http://go.microsoft.com/fwlink/?linkid=226382)
</td>
<td style="border:1px solid black;">
[**MS11-075**](http://go.microsoft.com/fwlink/?linkid=221538)
</td>
<td style="border:1px solid black;">
[**MS11-076**](http://go.microsoft.com/fwlink/?linkid=227073)
</td>
<td style="border:1px solid black;">
[**MS11-077**](http://go.microsoft.com/fwlink/?linkid=225915)
</td>
<td style="border:1px solid black;">
[**MS11-080**](http://go.microsoft.com/fwlink/?linkid=227486)
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
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Žádný
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 pro 32bitové systémy a Windows 7 pro 32bitové systémy Service Pack 1
</td>
<td style="border:1px solid black;">
Pouze Windows 7 pro 32bitové systémy:  
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=81be7ff1-3ba2-430c-9edf-619cc246daf2)  
(KB2572076)  
(Kritický)  
Pouze Windows 7 pro 32bitové systémy Service Pack 1:  
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=98403988-7438-4260-95b5-a4796dbe0618)  
(KB2572077)  
(Kritický)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=770e7b58-6544-4f59-9893-b3eadf6d6c8a)<sup>[1]</sup>
(KB2572078)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=4de175be-bbb7-4912-ba4e-d6fe96606c9e)  
(Kritický)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=b49876c7-7c65-4b6d-be9a-9f18be23037b)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows 7 pro 32bitové systémy a Windows 7 pro 32bitové systémy Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=02d28e59-b38f-433a-a568-e86f9d43dd42)  
(KB2564958)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows 7 pro 32bitové systémy a Windows 7 pro 32bitové systémy Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=76fcf0ec-9062-4090-acb2-401355341a2b)  
(KB2579686)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows 7 pro 32bitové systémy a Windows 7 pro 32bitové systémy Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=9e40bc26-f77f-4b57-9b3d-9d053c19ac56)  
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
Pouze Windows 7 pro systémy s procesorem x64:  
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=81be7ff1-3ba2-430c-9edf-619cc246daf2)  
(KB2572076)  
(Kritický)  
Pouze Windows 7 pro systémy s procesorem x64 Service Pack 1:  
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=98403988-7438-4260-95b5-a4796dbe0618)  
(KB2572077)  
(Kritický)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=770e7b58-6544-4f59-9893-b3eadf6d6c8a)<sup>[1]</sup>
(KB2572078)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=16fd238e-6f65-4d38-88ae-2689817588e1)  
(Kritický)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=cc0773f2-6099-4d55-9971-ee6546369c7f)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows 7 pro systémy s procesorem x64 a Windows 7 pro systémy s procesorem x64 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=904dec69-e8b9-4b23-a5ea-d3e7e9b9df07)  
(KB2564958)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows 7 pro systémy s procesorem x64 a Windows 7 pro systémy s procesorem x64 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=78c099b7-4bcb-4da7-8967-512c6541c541)  
(KB2579686)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows 7 pro systémy s procesorem x64 a Windows 7 pro systémy s procesorem x64 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=219554e6-eb5a-42d0-90c0-42b4d0772cfd)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
</tr>
<tr>
<th colspan="7" style="border:1px solid black;">
Windows Server 2008 R2
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS11-078**](http://go.microsoft.com/fwlink/?linkid=227075)
</td>
<td style="border:1px solid black;">
[**MS11-081**](http://go.microsoft.com/fwlink/?linkid=226382)
</td>
<td style="border:1px solid black;">
[**MS11-075**](http://go.microsoft.com/fwlink/?linkid=221538)
</td>
<td style="border:1px solid black;">
[**MS11-076**](http://go.microsoft.com/fwlink/?linkid=227073)
</td>
<td style="border:1px solid black;">
[**MS11-077**](http://go.microsoft.com/fwlink/?linkid=225915)
</td>
<td style="border:1px solid black;">
[**MS11-080**](http://go.microsoft.com/fwlink/?linkid=227486)
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
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
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
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 pro systémy s procesorem x64 a Windows Server 2008 R2 pro systémy s procesorem x64 Service Pack 1
</td>
<td style="border:1px solid black;">
Pouze Windows Server 2008 R2 pro systémy s procesorem x64:  
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=81be7ff1-3ba2-430c-9edf-619cc246daf2)\*  
(KB2572076)  
(Kritický)  
Pouze Windows Server 2008 R2 pro systémy s procesorem x64:  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=770e7b58-6544-4f59-9893-b3eadf6d6c8a)<sup>[1]</sup>
(KB2572078)  
(Kritický)  
Pouze Windows Server 2008 R2 pro systémy s procesorem x64 Service Pack 1:  
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=98403988-7438-4260-95b5-a4796dbe0618)\*  
(KB2572077)  
(Kritický)  
Pouze Windows Server 2008 R2 pro systémy s procesorem x64 Service Pack 1:  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=770e7b58-6544-4f59-9893-b3eadf6d6c8a)\*<sup>[1]</sup>
(KB2572078)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=8435781e-0f77-41d0-abb9-9b70f5b02d33)\*\*  
(Mírný)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=646a9a56-c343-45cb-a255-303602aa5a64)\*\*  
(Mírný)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem x64 a Windows Server 2008 R2 pro systémy s procesorem x64 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=c7bd50b7-03f1-4ea4-ad71-d428822c62f8)\*  
(KB2564958)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem x64 a Windows Server 2008 R2 pro systémy s procesorem x64 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=39bd4cfb-fe61-41b8-a5a2-73a9e720fc72)\*  
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
Pouze Windows Server 2008 R2 pro systémy s procesorem Itanium:  
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=81be7ff1-3ba2-430c-9edf-619cc246daf2)  
(KB2572076)  
(Kritický)  
Pouze Windows Server 2008 R2 pro systémy s procesorem Itanium Service Pack 1:  
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=98403988-7438-4260-95b5-a4796dbe0618)  
(KB2572077)  
(Kritický)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=770e7b58-6544-4f59-9893-b3eadf6d6c8a)<sup>[1]</sup>
(KB2572078)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=2676597e-c1d4-4397-8dc4-515ce3d0c5fd)  
(Mírný)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem Itanium a Windows Server 2008 R2 pro systémy s procesorem Itanium Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=aa816682-9652-433c-b1b4-5d0bc17b6a87)  
(KB2564958)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem Itanium a Windows Server 2008 R2 pro systémy s procesorem Itanium Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=0d35c6d0-6d2d-42bf-a97f-4c5e01b1937e)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
</tr>
</table>
<p></p>
 
**Poznámky** **k systémům Windows Server 2008 a Windows Server 2008 R2**

**\*Instalace Server Core obsahující chybu zabezpečení.** Tato aktualizace se stejným hodnocením závažnosti se vztahuje k podporovaným edicím systému Windows Server 2008 nebo Windows Server 2008 R2, jak je uvedeno, s instalací pomocí volby pro instalaci Server Core nebo bez ní. Další informace o této možnosti instalace naleznete v článcích na webu TechNet [Managing a Server Core Installation](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) (Správa instalace Server Core) a [Servicing a Server Core Installation](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx) (Obsluha instalace Server Core). Možnost instalace Server Core se nevztahuje na určité edice systému Windows Server 2008 a Windows Server 2008 R2; další informace naleznete v části [Porovnání možností instalace Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**\*\*Instalace Server Core není touto chybou ovlivněna.** Chyby zabezpečení, které tato aktualizace řeší, nemají vliv na podporované edice systému Windows Server 2008 nebo Windows Server 2008 R2, jak je uvedeno, v případě instalace s využitím možnosti instalace Server Core. Další informace o této možnosti instalace naleznete v článcích na webu TechNet [Managing a Server Core Installation](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) (Správa instalace Server Core) a [Servicing a Server Core Installation](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx) (Obsluha instalace Server Core). Možnost instalace Server Core se nevztahuje na určité edice systému Windows Server 2008 a Windows Server 2008 R2; další informace naleznete v části [Porovnání možností instalace Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**Poznámky k bulletinu MS11-078**

<sup>[1]</sup>**Postižena jsou rozhraní .NET Framework 4 a .NET Framework 4 Client Profile.** Distribuční balíčky rozhraní .NET Framework verze 4 jsou k dispozici ve dvou profilech: .NET Framework 4 a .NET Framework 4 Client Profile. Rozhraní .NET Framework 4 Client Profile je verzí rozhraní .NET Framework 4. Chyba zabezpečení řešená v této aktualizaci se týká jak rozhraní .NET Framework 4, tak rozhraní .NET Framework 4 Client Profile. Další informace získáte v článku [Instalace rozhraní .NET Framework](http://msdn.microsoft.com/en-us/library/5a4x27ek.aspx) na webu MSDN.

Více aktualizovaných souborů v rámci stejného identifikátoru bulletinu naleznete také v dalších kategoriích softwaru v rámci této části **Software obsahující tuto chybu a umístění aktualizací ke stažení**. Tento bulletin se vztahuje na více kategorií softwaru.

**Poznámka k bulletinu MS11-076**

<sup>[1]</sup>Sada programu Windows Media Center TV pro systém Windows Vista je k dispozici jako volitelná součást pouze v instalacích OEM (originální výrobce zařízení) systémů Windows Vista Home Premium a Windows Vista Ultimate. Zákazníci, kteří mají v systému s procesorem x64 tuto součást nainstalovanou, by měli nainstalovat obě aktualizace. V souladu s doporučenými postupy doporučuje společnost Microsoft nejprve nainstalovat aktualizaci operačního systému (KB2579686) a až poté aktualizaci sady programu Windows Media Center TV (KB2579692). Zákazníci, kteří mají sadu programu Media Center TV nainstalovanou v 32bitových systémech, by měli nainstalovat aktualizaci KB2579692.

#### Microsoft Server Software

 
<p></p>
<table style="border:1px solid black;">
<tr>
<th colspan="2" style="border:1px solid black;">
Microsoft Host Integration Server
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS11-082**](http://go.microsoft.com/fwlink/?linkid=228596)
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
Microsoft Host Integration Server 2004
</td>
<td style="border:1px solid black;">
[Microsoft Host Integration Server 2004 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=b7536139-63ea-482a-8d1c-0faad1fcfaa4)  
(KB2578757)  
(Vysoký)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Host Integration Server 2006
</td>
<td style="border:1px solid black;">
[Microsoft Host Integration Server 2006 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=3bc0c89c-56b2-4463-b671-2a58bed9667b)  
(KB2579597)  
(Vysoký)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Host Integration Server 2009
</td>
<td style="border:1px solid black;">
[Microsoft Host Integration Server 2009](http://www.microsoft.com/downloads/details.aspx?familyid=28716ed4-f215-4c69-b6b8-63fbeecefc5b)  
(KB2579598)  
(Vysoký)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Host Integration Server 2010
</td>
<td style="border:1px solid black;">
[Microsoft Host Integration Server 2010](http://www.microsoft.com/downloads/details.aspx?familyid=dbbd67d8-68aa-424d-8eaf-a273a71624d1)  
(KB2579599)  
(Vysoký)
</td>
</tr>
</table>
<p></p>
 

#### Vývojářské nástroje a software společnosti Microsoft

 
<p></p>
<table style="border:1px solid black;">
<tr>
<th colspan="2" style="border:1px solid black;">
Microsoft Silverlight
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS11-078**](http://go.microsoft.com/fwlink/?linkid=227075)
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
Microsoft Silverlight 4
</td>
<td style="border:1px solid black;">
[Microsoft Silverlight 4](http://www.microsoft.com/downloads/details.aspx?familyid=8bde4992-bdf7-4345-835a-4e1fbfcd8c5f) při instalaci v systému Mac  
(KB2617986)  
[Microsoft Silverlight 4](http://www.microsoft.com/downloads/details.aspx?familyid=8bde4992-bdf7-4345-835a-4e1fbfcd8c5f) při instalaci ve všech podporovaných vydáních klientů se systémem Microsoft Windows  
(KB2617986)  
[Microsoft Silverlight 4](http://www.microsoft.com/downloads/details.aspx?familyid=8bde4992-bdf7-4345-835a-4e1fbfcd8c5f) při instalaci ve všech podporovaných vydáních serverů se systémem Microsoft Windows\*\*  
(KB2617986)
</td>
</tr>
</table>
<p></p>
 
**Poznámky** **k bulletinu MS11-078**

**\*\*Instalace Server Core není touto chybou ovlivněna.** Chyby zabezpečení, které tato aktualizace řeší, nemají vliv na podporované edice systému Windows Server 2008 nebo Windows Server 2008 R2, jak je uvedeno, v případě instalace s využitím možnosti instalace Server Core. Další informace o této možnosti instalace naleznete v článcích na webu TechNet [Managing a Server Core Installation](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) (Správa instalace Server Core) a [Servicing a Server Core Installation](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx) (Obsluha instalace Server Core). Možnost instalace Server Core se nevztahuje na určité edice systému Windows Server 2008 a Windows Server 2008 R2; další informace naleznete v části [Porovnání možností instalace Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

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
[**MS11-079**](http://go.microsoft.com/fwlink/?linkid=217472)
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
[Microsoft Forefront Unified Access Gateway 2010](http://www.microsoft.com/downloads/details.aspx?familyid=770ad8ba-4d9a-404e-9515-6ed1e41682df)<sup>[1]</sup>
(KB2522482)  
(Vysoký)  
[Microsoft Forefront Unified Access Gateway 2010 Update 1](http://www.microsoft.com/downloads/details.aspx?familyid=b0de8d20-9c25-41c0-9c02-d263b9ed22fa)<sup>[1]</sup>
(KB2522483)  
(Vysoký)  
[Microsoft Forefront Unified Access Gateway 2010 Update 2](http://www.microsoft.com/downloads/details.aspx?familyid=166bdfcb-5088-4471-9d51-a3071ac13b73)<sup>[1]</sup>
(KB2522484)  
(Vysoký)  
[Microsoft Forefront Unified Access Gateway 2010 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=8b6ad2ae-e168-45d9-bd3f-5590e0cbd2b5)<sup>[1]</sup>
(KB2522485)  
(Vysoký)
</td>
</tr>
</table>
<p></p>
 
**Poznámka** **k bulletinu MS11-079**

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

**Nástroj Microsoft Baseline Security Analyzer**

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

-   Aktualizace zabezpečení jsou k dispozici na webu [služby Stažení softwaru](http://go.microsoft.com/fwlink/?linkid=21129). Nejsnadněji je naleznete hledáním podle klíčových slov aktualizace zabezpečení.
-   Aktualizace pro klientské platformy jsou k dispozici na webu [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747).
-   Aktualizace zabezpečení nabízené tento měsíc na webu Windows Update jsou k dispozici na webu služby Stažení softwaru v souborech obrazu ISO disku CD s vydanými aktualizacemi zabezpečení a kritickými aktualizacemi. Další informace získáte v [článku 913086 znalostní báze Microsoft Knowledge Base](http://support.microsoft.com/kb/913086).

**Komunita odborníků v oblasti zabezpečení**

Na webu [IT Pro Security Community](http://go.microsoft.com/fwlink/?linkid=21164) se můžete naučit, jak zlepšit zabezpečení a optimalizovat infrastrukturu IT, a diskutovat s dalšími členy komunity odborníků o bezpečnostních tématech.

#### Poděkování

Společnost Microsoft tímto [děkuje](http://go.microsoft.com/fwlink/?linkid=21127) za spolupráci při ochraně zákazníků:

-   [Mile Parkourové](http://contagiodump.com), spolupracující s Anshulem Kotharim a Nishantem Kaushikem ze společnosti [Adobe Systems, Inc.](http://www.adobe.com), za oznámení chyby popsané v bulletinu MS11-075.
-   Andrei Lutasovi ze společnosti [BitDefender](http://www.bitdefender.com/) za oznámení chyby popsané v bulletinu MS11-077.
-   Tarjei Mandtovi ze společnosti [Norman](http://www.norman.com/) za oznámení chyby popsané v bulletinu MS11-077.
-   Maikovi Wellmannovi za oznámení chyby popsané v bulletinu MS11-077.
-   Willovi Dormanovi ze společnosti [CERT/CC](http://www.cert.org/) za oznámení chyby popsané v bulletinu MS11-077.
-   Anonymnímu přispěvateli pracujícímu v programu [Beyond Security's SecuriTeam Secure Disclosure](http://www.beyondsecurity.com/ssd.html) za oznámení chyby popsané v bulletinu MS11-078.
-   Společnosti [Tenable Network Security](http://www.tenable.com/) za oznámení chyby popsané v bulletinu MS11-079.
-   Elisabeth Demeterové ze společnosti [SEC Consult Unternehmensberatung GmbH](http://www.sec-consult.com/) za oznámení chyby popsané v bulletinu MS11-079.
-   Bo Zhouovi z univerzity [National University of Defense Technology](http://www.nudt.edu.cn/) za oznámení chyby popsané v bulletinu MS11-080.
-   Vishwasovi Sharmovi ze společnosti McAfee Labs za oznámení chyby popsané v bulletinu MS11-081.
-   Davidu Bloomovi ze společnosti [Greplin](https://www.greplin.com) za oznámení dvou chyb popsaných v bulletinu MS11-081.
-   Ivanu Fratricovi, spolupracujícímu s organizací [TippingPoint](http://www.tippingpoint.com) v rámci iniciativy [Zero Day Initiative](http://www.zerodayinitiative.com), za oznámení dvou chyb popsaných v bulletinu MS11-081.
-   Společnosti [GWSlabs](http://www.gwslabs.com), spolupracující se společností [VeriSign iDefense Labs](http://labs.idefense.com), za oznámení chyby popsané v bulletinu MS11-081.
-   Sebastianu Apeltovi, spolupracujícímu s organizací [TippingPoint](http://www.tippingpoint.com) v rámci iniciativy [Zero Day Initiative](http://www.zerodayinitiative.com), za oznámení chyby popsané v bulletinu MS11-081.
-   Anonymnímu výzkumníkovi, spolupracujícímu s organizací [TippingPoint](http://www.tippingpoint.com) v rámci iniciativy [Zero Day Initiative](http://www.zerodayinitiative.com), za oznámení chyby popsané v bulletinu MS11-081.
-   Eduardu Vela Navovi ze společnosti [Google Inc.](http://www.google.com) a Davidu Bloomovi ze společnosti [Greplin](https://www.greplin.com) za spolupráci na prvcích rozšíření ochrany zahrnutých v bulletinu MS11-081.
-   [Soroushi Dalilimu](http://www.secproject.com) za spolupráci na prvcích rozšíření ochrany zahrnutých v bulletinu MS11-081.
-   Billymu Riosovi ze společnosti [Google Inc.](http://www.google.com) za spolupráci na prvcích rozšíření ochrany zahrnutých v bulletinu MS11-081.

#### Technická podpora

-   Uvedený software byl testován za účelem zjištění, kterých verzí se chyba týká. U dalších verzí skončila časově omezená podpora. Pokud chcete zjistit dobu, po kterou je pro určitou verzi softwaru poskytována podpora, navštivte web [Zásady poskytování technické podpory pro produkty společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=21742).
-   Zákazníci mohou získat technickou podporu na webu [služby technické podpory společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=21131). Hovory související s aktualizacemi zabezpečení jsou bezplatné. Další informace o dostupných možnostech technické podpory naleznete na webu [Pomoc a podpora společnosti Microsoft](http://support.microsoft.com/).
-   Mezinárodní zákazníci získají podporu u místních zastoupení společnosti Microsoft. Technická podpora související s aktualizacemi zabezpečení je bezplatná. Další informace o možnostech kontaktování společnosti Microsoft v případě potřeby technické podpory získáte na [webu mezinárodní technické podpory](http://go.microsoft.com/fwlink/?linkid=21155).

#### Zřeknutí se záruky

Informace ve znalostní bázi Microsoft Knowledge Base jsou poskytovány tak, jak jsou, bez jakékoli záruky. Společnost Microsoft neposkytuje žádné záruky, výslovně uvedené či mlčky předpokládané, včetně záruk obchodovatelnosti a vhodnosti pro určitý účel. Společnost Microsoft ani její dodavatelé nenesou v žádném případě zodpovědnost za žádné škody, včetně přímých, nepřímých, náhodných či následných škod, ztráty zisku či zvláštních škod, a to ani v případě, že byli na možnost takových škod upozorněni. V některých zemích a právních řádech není dovoleno vyloučit nebo omezit odpovědnost, proto se výše uvedené omezení na vás nemusí vztahovat.

#### Revize

-   V1.0 (11. října 2011): Souhrnný bulletin byl publikován.
-   V1.1 (26. října 2011): V bulletinu MS11-078 byla opravena informace o použitelnosti instalace Server Core pro rozhraní .NET Framework 4 v systému Windows Server 2008 R2 pro systémy s procesorem x64.

*Built at 2014-04-18T01:50:00Z-07:00*
