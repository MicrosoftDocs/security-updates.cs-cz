---
TOCTitle: 'MS11-AUG'
Title: 'Souhrnný bulletin zabezpečení společnosti Microsoft, srpen 2011'
ms:assetid: 'ms11-aug'
ms:contentKeyID: 61224007
ms:mtpsurl: 'https://technet.microsoft.com/cs-CZ/library/ms11-aug(v=Security.10)'
---

 

Souhrnný bulletin zabezpečení společnosti Microsoft, srpen 2011
===============================================================

Publikováno: 9. srpna 2011 | Aktualizováno: 26. října 2011

**Verze:** 1.2

Tento souhrnný bulletin uvádí bulletiny zabezpečení vydané v srpnu 2011.

Spolu s vydáním bulletinů pro srpen 2011 nahrazuje tento souhrnný bulletin předběžné oznámení o bulletinech vydané 4. srpna 2011. Další informace o službě předběžného oznámení o bulletinech naleznete v části [Předběžné oznámení o bulletinech zabezpečení společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=217213).

Informace o tom, jak dostávat automatická oznámení o vydání nových bulletinů zabezpečení společnosti Microsoft, naleznete na webu [Zasílání technických oznámení o zabezpečení společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=21163).

Pro zodpovězení zákaznických dotazů týkajících se těchto bulletinů uspořádá společnost Microsoft webové vysílání 10. srpna 2011 v 11:00 časového pásma Tichomoří (USA a Kanada). [Zaregistrujte se pro webové vysílání týkající se srpnových bulletinů zabezpečení](https://msevents.microsoft.com/cui/eventdetail.aspx?culture=en-us&eventid=1032487857). Po tomto datu je webové vysílání dostupné na požádání. Další informace získáte v [souhrnných bulletinech zabezpečení společnosti Microsoft a webovém vysílání](http://go.microsoft.com/fwlink/?linkid=217214).

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
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=221946">MS11-057</a></td>
<td style="border:1px solid black;"><strong>Kumulativní aktualizace zabezpečení pro aplikaci Internet Explorer (2559049)</strong><br />
<br />
Tato aktualizace zabezpečení řeší pět chyb zabezpečení oznámených soukromými osobami a dvě veřejně známé chyby zabezpečení v aplikaci Internet Explorer. Nejzávažnější chyby zabezpečení mohou umožnit vzdálené spuštění kódu, pokud uživatel pomocí aplikace Internet Explorer zobrazí speciálně vytvořenou webovou stránku. Útočník, který by úspěšně zneužil některou z těchto chyb zabezpečení, by mohl získat stejná uživatelská práva, jaká má místní uživatel. Uživatelé, jejichž účty jsou konfigurovány tak, aby měli v systému méně uživatelských práv, by byli vystaveni menšímu riziku než uživatelé s uživatelskými právy správce.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritický</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Internet Explorer</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=221812">MS11-058</a></td>
<td style="border:1px solid black;"><strong>Chyby zabezpečení v serveru DNS umožňují vzdálené spuštění kódu (2562485)</strong><br />
<br />
Tato aktualizace zabezpečení řeší dvě chyby zabezpečení serveru DNS systému Windows oznámené soukromými osobami. Závažnější z těchto chyb zabezpečení by mohla povolit vzdálené spuštění kódu, pokud si útočník zaregistruje doménu, vytvoří záznam NAPTR zdroje DNS, a poté pošle speciálně vytvořený dotaz NAPTR na cílový server DNS. Servery, které nemají funkci DNS povolenu, nejsou ohroženy.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritický</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=221539">MS11-059</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení v rozhraní DAC (Data Access Components) umožňuje vzdálené spuštění kódu (2560656)</strong><br />
<br />
Tato aktualizace zabezpečení řeší chybu zabezpečení v systému Microsoft Windows, kterou oznámila soukromá osoba. Chyba zabezpečení by mohla umožnit vzdálené spuštění kódu, pokud uživatel otevře legitimní soubor programu Excel (např. soubor s příponou XLSX) umístěný ve stejném síťovém adresáři jako speciálně vytvořený soubor knihovny. Útočník, který by úspěšně zneužil tuto chybu zabezpečení, by mohl získat stejná uživatelská práva, jaká má přihlášený uživatel. Uživatelé, jejichž účty jsou konfigurovány tak, aby měli v systému méně uživatelských práv, by byli vystaveni menšímu riziku než uživatelé s uživatelskými právy správce.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Vysoký</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Může vyžadovat restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=223425">MS11-060</a></td>
<td style="border:1px solid black;"><strong>Chyby zabezpečení v aplikaci Microsoft Visio umožňují vzdálené spuštění kódu (2560978)</strong><br />
<br />
Tato aktualizace zabezpečení řeší dvě soukromými osobami oznámené chyby zabezpečení v aplikaci Microsoft Visio. Chyby umožňují vzdálené spuštění kódu, pokud uživatel otevře speciálně vytvořený soubor aplikace Visio. Útočník, který by úspěšně zneužil tuto chybu zabezpečení, by mohl získat stejná uživatelská práva, jaká má přihlášený uživatel. Uživatelé, jejichž účty jsou konfigurovány tak, aby měli v systému méně uživatelských práv, by byli vystaveni menšímu riziku než uživatelé s uživatelskými právy správce.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Vysoký</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Může vyžadovat restartování</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217099">MS11-061</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení programu Webový přístup ke vzdálené ploše umožňuje zvýšení úrovně oprávnění (2546250)</strong><br />
<br />
Tato aktualizace zabezpečení řeší chybu zabezpečení programu Webový přístup ke vzdálené ploše. Jde o chybu zabezpečení skriptování mezi servery (XSS), která umožňuje zvýšení úrovně oprávnění, což by mohlo útočníkovi umožnit provádět na stránce libovolné příkazy v kontextu cílového uživatele. Uživatele aplikací Internet Explorer 8 a Internet Explorer 9 před tímto útokem při návštěvě serveru s programem Webový přístup ke vzdálené ploše v zóně Internet chrání filtr XSS v těchto aplikacích. Filtr XSS v aplikacích Internet Explorer 8 a Internet Explorer 9 není v zóně Intranet ve výchozím nastavení povolen.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Vysoký</a><br />
Zvýšení úrovně oprávnění</td>
<td style="border:1px solid black;">Může vyžadovat restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=223669">MS11-062</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení ovladače NDISTAPI služby Vzdálený přístup umožňuje zvýšení úrovně oprávnění</strong> <strong>(2566454)</strong><br />
<br />
Tato aktualizace zabezpečení řeší chybu zabezpečení ve všech podporovaných edicích systémů Windows XP a Windows Server 2003 oznámenou soukromou osobou. Tato aktualizace zabezpečení má vysoký stupeň závažnosti pro všechny podporované edice systémů Windows XP a Windows Server 2003. Systémy Windows Vista, Windows Server 2008, Windows 7 a Windows Server 2008 R2 nejsou postiženy zmíněnou chybou zabezpečení.<br />
<br />
Tato chyba zabezpečení umožňuje zvýšit úroveň oprávnění, pokud se útočník připojí k postiženému systému, spustí speciálně vytvořenou aplikaci určenou ke zneužití této chyby zabezpečení a převezme úplnou kontrolu nad postiženým systémem. Tuto chybu může zneužít pouze útočník s platnými pověřeními pro přihlášení, která by mu umožňovala se místně přihlásit.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Vysoký</a><br />
Zvýšení úrovně oprávnění</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=221864">MS11-063</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení v podsystému Windows CSRSS (Client/Server Run-time Subsystem) umožňuje zvýšení úrovně oprávnění (2567680)</strong><br />
<br />
Tato aktualizace zabezpečení řeší chybu zabezpečení v systému Microsoft Windows, kterou oznámila soukromá osoba. Tato chyba zabezpečení umožňuje zvýšit úroveň oprávnění, pokud se útočník připojí k postiženému systému a spustí speciálně vytvořenou aplikaci pro odeslání zprávy o události zařízení procesu s vyšší integritou. Tuto chybu může zneužít pouze útočník s platnými pověřeními pro přihlášení, která by mu umožňovala se místně přihlásit.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Vysoký</a><br />
Zvýšení úrovně oprávnění</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=221808">MS11-064</a></td>
<td style="border:1px solid black;"><strong>Chyby zabezpečení v zásobníku protokolu TCP/IP umožňují odmítnutí služby (2563894)</strong><br />
<br />
Tato aktualizace zabezpečení řeší dvě soukromými osobami oznámené chyby zabezpečení v systému Microsoft Windows. Chyby zabezpečení umožňují odmítnutí služby, pokud útočník odešle řadu speciálně vytvořených zpráv protokolu ICMP (Internet Control Message Protocol) cílovému systému nebo pošle speciálně vytvořený požadavek URL serveru, který nabízí webový obsah a má povolenou technologii Quality of Service (QoS) založenou na URL.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Vysoký</a><br />
Odmítnutí služby</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=221880">MS11-065</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení protokolu RDP (Remote Desktop Protocol) může způsobit odmítnutí služby (2570222)</strong><br />
<br />
Tato aktualizace zabezpečení řeší chybu zabezpečení protokolu RDP (Remote Desktop Protocol) oznámenou soukromou osobou. Tato chyba zabezpečení může způsobit odmítnutí služby, pokud postižený systém obdrží řadu speciálně vytvořených paketů protokolu RDP. Společnost Microsoft má také informace o omezených cílených útocích, které se snažily tuto chybu zabezpečení zneužít. Ve výchozím nastavení není v žádném operačním systému Windows protokol RDP povolen.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Vysoký</a><br />
Odmítnutí služby</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=221536">MS11-066</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení v aplikaci Microsoft Chart Control umožňuje zpřístupnění informací (2567943)</strong><br />
<br />
Tato aktualizace zabezpečení řeší soukromě oznámenou chybu zabezpečení ovládacích prvků ASP.NET Chart. Tato chyba zabezpečení umožňuje zpřístupnění informací, pokud útočník pošle speciálně vytvořený požadavek GET postiženému serveru, který je hostitelem ovládacích prvkůl Chart. Je třeba poznamenat, že tato chyba zabezpečení přímo nepovolí útočníkům spouštět kód nebo zvyšovat svou úroveň uživatelských práv, mohla by však být zneužita k získání informací, pomocí kterých by bylo možné dále ohrozit daný systém. Tímto problémem jsou postiženy pouze webové aplikace, které používají aplikaci Microsoft Chart Control. Výchozí instalace rozhraní .NET Framework postiženy nejsou.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Vysoký</a><br />
Přístup k informacím</td>
<td style="border:1px solid black;">Může vyžadovat restartování</td>
<td style="border:1px solid black;">Microsoft .NET Framework,<br />
Vývojářské nástroje společnosti Microsoft</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=223643">MS11-067</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení aplikace Microsoft Report Viewer umožňuje zpřístupnění informací (2578230)</strong><br />
<br />
Tato aktualizace zabezpečení řeší soukromě oznámenou chybu zabezpečení v aplikaci Microsoft Report Viewer. Uvedená chyba zabezpečení umožňuje zpřístupnění informací, pokud uživatel prohlíží speciálně vytvořenou webovou stránku. Útočník však nemůže žádným způsobem přinutit uživatele k návštěvě takového webu. Namísto toho by útočník musel uživatele přimět k návštěvě takového webu. K tomu se obvykle používá odkaz v e-mailové zprávě nebo zprávě programu pro zasílání rychlých zpráv, na který uživatelé kliknou a přejdou tak na ohrožený web.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Vysoký</a><br />
Přístup k informacím</td>
<td style="border:1px solid black;">Může vyžadovat restartování</td>
<td style="border:1px solid black;">Vývojářské nástroje společnosti Microsoft</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=223578">MS11-068</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení jádra systému Windows může způsobit odmítnutí služby (2556532)</strong><br />
<br />
Tato aktualizace zabezpečení řeší chybu zabezpečení v systému Microsoft Windows, kterou oznámila soukromá osoba. Chyba zabezpečení by mohla způsobit odmítnutí služby, pokud uživatel navštíví sdílenou síťovou složku (nebo navštíví web odkazující na sdílenou síťovou složku) obsahující speciálně vytvořený soubor. Útočník však nemůže žádným způsobem přinutit uživatele k návštěvě takové sdílené síťové složky nebo webové stránky. Namísto toho by útočník musel uživatele přesvědčit, aby tak učinil. K tomu se obvykle používá odkaz v e-mailové zprávě nebo zprávě programu pro zasílání rychlých zpráv, na který uživatel klikne.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Mírný</a><br />
Odmítnutí služby</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=221537">MS11-069</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení v rozhraní .NET Framework může způsobit zpřístupnění informací (2567951)</strong><br />
<br />
Tato aktualizace zabezpečení řeší soukromě oznámenou chybu zabezpečení v rozhraní Microsoft .NET Framework. Tato chyba zabezpečení může způsobit zpřístupnění informací, pokud uživatel speciálně vytvořenou webovou stránku prohlíží ve webovém prohlížeči, který může spouštět aplikace prohlížeče XAML (XBAP). V případě útoku z webu by útočník mohl být hostitelem webu s webovou stránkou, pomocí které lze tuto chybu zabezpečení zneužít. Navíc, dané weby a weby, které přijímají nebo hostují materiál poskytovaný uživateli a reklamu, by mohly obsahovat speciálně vytvořený obsah zneužívající tuto chybu zabezpečení. Útočník však nemůže žádným způsobem přinutit uživatele k návštěvě takových webů. Místo toho by útočník musel přesvědčit uživatele, aby navštívili takový web. K tomu se obvykle používá odkaz v e-mailu nebo zpráva programu pro zasílání rychlých zpráv, na které uživatelé kliknou, a přejdou tak na útočníkův web. Tuto chybu zabezpečení mohou zneužít také aplikace Windows .NET k obejití omezení zabezpečení přístupu kódu (CAS).</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Mírný</a><br />
Přístup k informacím</td>
<td style="border:1px solid black;">Může vyžadovat restartování</td>
<td style="border:1px solid black;">Microsoft .NET Framework</td>
</tr>
</tbody>
</table>
<p></p>
  
Index zneužitelnosti  
--------------------
  

Následující tabulka uvádí hodnocení zneužitelnosti každé chyby zabezpečení uvedené v tomto měsíci. Chyby zabezpečení jsou řazeny podle čísla jednotlivých bulletinů (ID bulletinu) a chyb (ID CVE). Uvedeny jsou pouze chyby zabezpečení ohodnocené stupněm závažnosti Kritický nebo Vysoký.
  
**Jak pracovat s touto tabulkou**
  
V této tabulce zjistíte, jaká je pravděpodobnost zneužití v podobě spuštění kódu a odmítnutí služby během 30 dní od vydání tohoto bulletinu zabezpečení pro všechny aktualizace zabezpečení, které bude třeba nainstalovat. Všechna níže uvedená hodnocení zvažte na základě vaší specifické konfigurace a podle závěrů hodnocení nastavte priority pro zavádění jednotlivých aktualizací vydaných v tomto měsíci. Další informace o významu těchto hodnocení a způsobu jejich stanovení najdete v indexu zneužitelnosti [Microsoft Exploitability Index](http://technet.microsoft.com/en-us/security/cc998259.aspx).
  
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
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=221946">MS11-057</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se konfliktu časování otevření okna</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1257">CVE-2011-1257</a></td>
<td style="border:1px solid black;">Žádné ohrožení</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;">Dočasné</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=221946">MS11-057</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se přístupu k informacím obslužných rutin událostí</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1960">CVE-2011-1960</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">3</a> – Vytvoření kódu funkčního zneužití není pravděpodobné</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">3</a> – Vytvoření kódu funkčního zneužití není pravděpodobné</td>
<td style="border:1px solid black;">Netýká se</td>
<td style="border:1px solid black;">Jedná se o chybu zabezpečení typu zpřístupnění informací.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=221946">MS11-057</a></td>
<td style="border:1px solid black;">Chyba zabezpečení obslužné rutiny služby Telnet umožňující vzdálené spuštění kódu</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1961">CVE-2011-1961</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;">Netýká se</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=221946">MS11-057</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se poškození paměti XSLT</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1963">CVE-2011-1963</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;">Dočasné</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=221946">MS11-057</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se poškození paměti objektu Style</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1964">CVE-2011-1964</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;">Dočasné</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=221812">MS11-058</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se požadavku DNS NAPTR</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1966">CVE-2011-1966</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">3</a> – Vytvoření kódu funkčního zneužití není pravděpodobné</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">3</a> – Vytvoření kódu funkčního zneužití není pravděpodobné</td>
<td style="border:1px solid black;">Trvalé</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=221812">MS11-058</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se poškození neinicializované paměti DNS</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1970">CVE-2011-1970</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">3</a> – Vytvoření kódu funkčního zneužití není pravděpodobné</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">3</a> – Vytvoření kódu funkčního zneužití není pravděpodobné</td>
<td style="border:1px solid black;">Trvalé</td>
<td style="border:1px solid black;">Jedná se o chybu zabezpečení, která způsobuje odmítnutí služby.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=221539">MS11-059</a></td>
<td style="border:1px solid black;">Chyba zabezpečení nezabezpečeného načítání knihovny v rozhraní DAC (Data Access Components)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1975">CVE-2011-1975</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;">Žádné ohrožení</td>
<td style="border:1px solid black;">Netýká se</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=223425">MS11-060</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se vzdáleného spuštění kódu pStream Release</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1972">CVE-2011-1972</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;">Dočasné</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=223425">MS11-060</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se vzdáleného spuštění kódu při pohybu kolem bloku</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1979">CVE-2011-1979</a></td>
<td style="border:1px solid black;">Žádné ohrožení</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;">Dočasné</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217099">MS11-061</a></td>
<td style="border:1px solid black;">Chyba zabezpečení programu Webový přístup ke vzdálené ploše</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1263">CVE-2011-1263</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;">Žádné ohrožení</td>
<td style="border:1px solid black;">Netýká se</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=223669">MS11-062</a></td>
<td style="border:1px solid black;">Chyba zabezpečení umožňující zvýšení úrovně oprávnění subsystému NDISTAPI</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1974">CVE-2011-1974</a></td>
<td style="border:1px solid black;">Žádné ohrožení</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;">Trvalé</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=221864">MS11-063</a></td>
<td style="border:1px solid black;">Chyba zabezpečení CSRSS</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1967">CVE-2011-1967</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;">Netýká se</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=221808">MS11-064</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se odmítnutí služby protokolu ICMP</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1871">CVE-2011-1871</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">3</a> – Vytvoření kódu funkčního zneužití není pravděpodobné</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">3</a> – Vytvoření kódu funkčního zneužití není pravděpodobné</td>
<td style="border:1px solid black;">Trvalé</td>
<td style="border:1px solid black;">Jedná se o chybu zabezpečení, která způsobuje odmítnutí služby.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=221808">MS11-064</a></td>
<td style="border:1px solid black;">Chyba zabezpečení koordinátora TCP/IP QOS typu odmítnutí služby</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1965">CVE-2011-1965</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">3</a> – Vytvoření kódu funkčního zneužití není pravděpodobné</td>
<td style="border:1px solid black;">Žádné ohrožení</td>
<td style="border:1px solid black;">Trvalé</td>
<td style="border:1px solid black;">Jedná se o chybu zabezpečení, která způsobuje odmítnutí služby.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=221880">MS11-065</a></td>
<td style="border:1px solid black;">Chyba zabezpečení protokolu RDP (Remote Desktop Protocol)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1968">CVE-2011-1968</a></td>
<td style="border:1px solid black;">Žádné ohrožení</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">3</a> – Vytvoření kódu funkčního zneužití není pravděpodobné</td>
<td style="border:1px solid black;">Trvalé</td>
<td style="border:1px solid black;">U této chyby zabezpečení jsou hlášeny omezené cílené útoky.<br />
<br />
Jedná se o chybu zabezpečení, která způsobuje odmítnutí služby.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=221536">MS11-066</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se zpřístupnění informací v aplikaci Chart Control</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1977">CVE-2011-1977</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">3</a> – Vytvoření kódu funkčního zneužití není pravděpodobné</td>
<td style="border:1px solid black;">Žádné ohrožení</td>
<td style="border:1px solid black;">Netýká se</td>
<td style="border:1px solid black;">Jedná se o chybu zabezpečení typu zpřístupnění informací.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=223643">MS11-067</a></td>
<td style="border:1px solid black;">Chyba zabezpečení ovládacích prvků XSS aplikace Report Viewer</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1976">CVE-2011-1976</a></td>
<td style="border:1px solid black;">Žádné ohrožení</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">3</a> – Vytvoření kódu funkčního zneužití není pravděpodobné</td>
<td style="border:1px solid black;">Netýká se</td>
<td style="border:1px solid black;">Jedná se o chybu zabezpečení typu zpřístupnění informací.</td>
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
  
**Tabulka 1**

 
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
[**MS11-057**](http://go.microsoft.com/fwlink/?linkid=221946)
</td>
<td style="border:1px solid black;">
[**MS11-058**](http://go.microsoft.com/fwlink/?linkid=221812)
</td>
<td style="border:1px solid black;">
[**MS11-059**](http://go.microsoft.com/fwlink/?linkid=221539)
</td>
<td style="border:1px solid black;">
[**MS11-061**](http://go.microsoft.com/fwlink/?linkid=217099)
</td>
<td style="border:1px solid black;">
[**MS11-062**](http://go.microsoft.com/fwlink/?linkid=223669)
</td>
<td style="border:1px solid black;">
[**MS11-063**](http://go.microsoft.com/fwlink/?linkid=221864)
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
Žádný
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
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Aplikace Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=90312c78-1fbd-4143-b2e6-ae5c48af6f57)  
(Kritický)  
[Aplikace Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=a771c93b-55a4-456f-a315-d0d1f2696960)  
(Kritický)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=5feb8ed7-99d2-4dd6-986f-57a7fd0c6f19)  
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
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=6bc1f0ac-223d-4b0b-86cd-2ba3863955c4)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=0231c103-c0cb-4705-9d92-5356b8cbb265)  
(Vysoký)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Aplikace Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=23d77f3b-13f8-49f3-9c3c-27ad217cd59e)  
(Kritický)  
[Aplikace Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=acb14d82-a801-4ec7-84cc-9f131009ebcb)  
(Kritický)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=272c813b-bd39-4e63-9fa7-c5b8ed0b08d7)  
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
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d5ee6787-408d-4870-af70-9338158b161b)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=09276f6e-e3f4-4b7e-996e-4ec376c103e1)  
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
[**MS11-057**](http://go.microsoft.com/fwlink/?linkid=221946)
</td>
<td style="border:1px solid black;">
[**MS11-058**](http://go.microsoft.com/fwlink/?linkid=221812)
</td>
<td style="border:1px solid black;">
[**MS11-059**](http://go.microsoft.com/fwlink/?linkid=221539)
</td>
<td style="border:1px solid black;">
[**MS11-061**](http://go.microsoft.com/fwlink/?linkid=217099)
</td>
<td style="border:1px solid black;">
[**MS11-062**](http://go.microsoft.com/fwlink/?linkid=223669)
</td>
<td style="border:1px solid black;">
[**MS11-063**](http://go.microsoft.com/fwlink/?linkid=221864)
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
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Aplikace Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=26b5fb48-346a-49f1-840f-03f218a41c20)  
(Vysoký)  
[Aplikace Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=042552ad-f46a-4bfc-9e5c-58f095eba1de)  
(Kritický)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=648596fc-fd97-438a-97be-d5d590f1c561)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c2d4aa38-9241-465d-8d65-aba73e936d0f)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8de0f2db-aa09-48cd-a13b-e26a973e9cdc)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=870fdfdd-16bf-42a2-a23b-ed6045438d5e)  
(Vysoký)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Aplikace Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=9c3d14d8-6716-4423-91a9-a05373227237)  
(Vysoký)  
[Aplikace Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=c9e283d8-d4a2-41e2-a73c-92fae957ba3d)  
(Kritický)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=470d56d1-5789-42cc-a088-a2c8ac934ab3)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2db4098a-f4f9-4211-b55d-5d0df1409c43)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8f208407-4bb3-41fe-b0d6-fc8a5e30e667)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=31af27b8-7b73-4090-94bd-2fb89d3970fc)  
(Vysoký)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 SP2 pro systémy s procesorem Itanium
</td>
<td style="border:1px solid black;">
[Aplikace Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=64496a87-2225-402a-a94a-a8e92b17ac83)  
(Vysoký)  
[Aplikace Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=5aa3a493-4188-48a9-a549-cf9ba01ed32a)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=1934acfa-5637-4ae9-9e9a-fc7e58930b7a)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=ef140089-d022-4ee8-9cc4-7fb25295a39d)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=410c72d8-3b78-4c4a-ad61-acb7f854ffc2)  
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
[**MS11-057**](http://go.microsoft.com/fwlink/?linkid=221946)
</td>
<td style="border:1px solid black;">
[**MS11-058**](http://go.microsoft.com/fwlink/?linkid=221812)
</td>
<td style="border:1px solid black;">
[**MS11-059**](http://go.microsoft.com/fwlink/?linkid=221539)
</td>
<td style="border:1px solid black;">
[**MS11-061**](http://go.microsoft.com/fwlink/?linkid=217099)
</td>
<td style="border:1px solid black;">
[**MS11-062**](http://go.microsoft.com/fwlink/?linkid=223669)
</td>
<td style="border:1px solid black;">
[**MS11-063**](http://go.microsoft.com/fwlink/?linkid=221864)
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
Žádný
</td>
<td style="border:1px solid black;">
Žádný
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
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
[Aplikace Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=66ddc7ce-5280-494d-bb3c-dab06e27fb5c)  
(Kritický)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=a080f36e-c24f-40ac-bb40-b26cb31bcae3)  
(Kritický)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=c82417ec-232f-4f84-ba2c-0ffad77e9bb5)  
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
[Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8f25ced5-ef86-4b9d-91fb-443c9a2c1458)  
(Vysoký)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Aplikace Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=3f119902-8398-4814-8229-9eb9f0980e87)  
(Kritický)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=704c1c9c-d1c1-40cb-97a7-fbb1f195f9f8)  
(Kritický)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=a6ff7b27-bc21-4945-8b2e-757b6f83fa58)  
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
[Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d5b8ff09-237e-49f1-a566-e323ca11fbc3)  
(Vysoký)
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
[**MS11-057**](http://go.microsoft.com/fwlink/?linkid=221946)
</td>
<td style="border:1px solid black;">
[**MS11-058**](http://go.microsoft.com/fwlink/?linkid=221812)
</td>
<td style="border:1px solid black;">
[**MS11-059**](http://go.microsoft.com/fwlink/?linkid=221539)
</td>
<td style="border:1px solid black;">
[**MS11-061**](http://go.microsoft.com/fwlink/?linkid=217099)
</td>
<td style="border:1px solid black;">
[**MS11-062**](http://go.microsoft.com/fwlink/?linkid=223669)
</td>
<td style="border:1px solid black;">
[**MS11-063**](http://go.microsoft.com/fwlink/?linkid=221864)
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
Žádný
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
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 pro 32bitové systémy Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=da9c98d1-973c-44d9-aee5-f5c4a8e8c0e1)\*\*  
(Kritický)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=d65ae4cc-d82a-42da-829f-d9479e23b7a5)\*\*  
(Kritický)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=70065bd0-7c97-4ffc-828f-2cc245d04429)\*\*  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro 32bitové systémy Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ac2d5122-6f9b-46f5-9840-77aa7ff84308)\*  
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
[Windows Server 2008 pro 32bitové systémy Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=1fbaabb9-8601-4760-813d-aeedfdcafb8b)\*  
(Vysoký)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 pro systémy s procesorem x64 Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=9facff69-618f-4a64-8665-5dd6cde07de9)\*\*  
(Kritický)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=00f28d81-3714-403c-bcd7-55f2ac97f75b)\*\*  
(Kritický)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=9ce60689-ca85-4c9f-af96-a73b1e43c10b)\*\*  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5f605f6f-3854-403d-878b-637626aef78f)\*  
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
[Windows Server 2008 pro systémy s procesorem x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2e7253d8-fdc7-4563-9714-21ca3c77e4b1)\*  
(Vysoký)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 pro systémy s procesorem Itanium Service Pack 2
</td>
<td style="border:1px solid black;">
[Aplikace Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=01885624-cfb1-4918-abef-ab0ea765cb04)  
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
[Windows Server 2008 pro systémy s procesorem Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=fe37eb6d-b1fa-496c-a0d3-19a6d35a6cb9)  
(Vysoký)
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
[**MS11-057**](http://go.microsoft.com/fwlink/?linkid=221946)
</td>
<td style="border:1px solid black;">
[**MS11-058**](http://go.microsoft.com/fwlink/?linkid=221812)
</td>
<td style="border:1px solid black;">
[**MS11-059**](http://go.microsoft.com/fwlink/?linkid=221539)
</td>
<td style="border:1px solid black;">
[**MS11-061**](http://go.microsoft.com/fwlink/?linkid=217099)
</td>
<td style="border:1px solid black;">
[**MS11-062**](http://go.microsoft.com/fwlink/?linkid=223669)
</td>
<td style="border:1px solid black;">
[**MS11-063**](http://go.microsoft.com/fwlink/?linkid=221864)
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
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 pro 32bitové systémy a Windows 7 pro 32bitové systémy Service Pack 1
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=7019de24-8c58-4565-ada1-ca8755115096)  
(Kritický)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=12292081-23f7-4968-8cd7-17aaef2aed6a)  
(Kritický)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows 7 pro 32bitové systémy a Windows 7 pro 32bitové systémy Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=6bc168d9-6664-41fb-914f-dbd7514a4b0e)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows 7 pro 32bitové systémy a Windows 7 pro 32bitové systémy Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=f4551b77-eb09-448a-9dc5-66de846035e7)  
(Vysoký)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 7 pro systémy s procesorem x64 a Windows 7 pro systémy s procesorem x64 Service Pack 1
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=fcdb872f-2ee2-4f74-b7ae-1b82daf66761)  
(Kritický)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=ef664114-6582-49d3-b332-078a7d075337)  
(Kritický)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows 7 pro systémy s procesorem x64 a Windows 7 pro systémy s procesorem x64 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=aafeff2d-db9a-4b3b-b620-be4ec5f5bdcc)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows 7 pro systémy s procesorem x64 a Windows 7 pro systémy s procesorem x64 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=0fc9a501-523d-4cbb-8d99-a773089afc4c)  
(Vysoký)
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
[**MS11-057**](http://go.microsoft.com/fwlink/?linkid=221946)
</td>
<td style="border:1px solid black;">
[**MS11-058**](http://go.microsoft.com/fwlink/?linkid=221812)
</td>
<td style="border:1px solid black;">
[**MS11-059**](http://go.microsoft.com/fwlink/?linkid=221539)
</td>
<td style="border:1px solid black;">
[**MS11-061**](http://go.microsoft.com/fwlink/?linkid=217099)
</td>
<td style="border:1px solid black;">
[**MS11-062**](http://go.microsoft.com/fwlink/?linkid=223669)
</td>
<td style="border:1px solid black;">
[**MS11-063**](http://go.microsoft.com/fwlink/?linkid=221864)
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
Žádný
</td>
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 pro systémy s procesorem x64 a Windows Server 2008 R2 pro systémy s procesorem x64 Service Pack 1
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=14fe68eb-2aa6-4a59-b9d8-deeae5236af2)\*\*  
(Kritický)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=dd709da2-4cb1-482f-88eb-dfab4d3c59c6)\*\*  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem x64 a Windows Server 2008 R2 pro systémy s procesorem x64 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=6a86e2cf-4e7d-4012-88c3-6957a3842dd3)\*  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem x64 a Windows Server 2008 R2 pro systémy s procesorem x64 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=c29deec3-4672-4658-a550-dce244434cd4)\*  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem x64 a Windows Server 2008 R2 pro systémy s procesorem x64 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=777f3bbe-094c-411d-879d-34a5a20ae7f3)\*\*  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem x64 a Windows Server 2008 R2 pro systémy s procesorem x64 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=2f4043df-c07c-4611-b06a-7fcbb7416e7d)\*  
(Vysoký)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 pro systémy s procesorem Itanium a Windows Server 2008 R2 pro systémy s procesorem Itanium Service Pack 1
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=82403fd3-ed75-4ea8-aa3f-ed9dda75612a)  
(Kritický)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem Itanium a Windows Server 2008 R2 pro systémy s procesorem Itanium Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=1d6b8036-d38f-408a-a36c-027553faefc1)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem Itanium a Windows Server 2008 R2 pro systémy s procesorem Itanium Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=b420cae3-de30-4c6c-8ed9-7431ad7ab4da)  
(Vysoký)
</td>
</tr>
</table>
<p></p>
 
**Poznámky k systémům Windows Server 2008 a Windows Server 2008 R2**

**\*Instalace Server Core obsahující chybu zabezpečení.** Tato aktualizace se stejným hodnocením závažnosti se vztahuje k podporovaným edicím systému Windows Server 2008 nebo Windows Server 2008 R2, jak je uvedeno, s instalací pomocí volby pro instalaci Server Core nebo bez ní. Další informace o této možnosti instalace naleznete v článcích na webu TechNet [Managing a Server Core Installation](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) (Správa instalace Server Core) a [Servicing a Server Core Installation](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx) (Obsluha instalace Server Core). Možnost instalace Server Core se nevztahuje na určité edice systému Windows Server 2008 a Windows Server 2008 R2; další informace naleznete v části [Porovnání možností instalace Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**\*\*Instalace Server Core není touto chybou ovlivněna.** Chyby zabezpečení, které tato aktualizace řeší, nemají vliv na podporované edice systému Windows Server 2008 nebo Windows Server 2008 R2, jak je uvedeno, v případě instalace s využitím možnosti instalace Server Core. Další informace o této možnosti instalace naleznete v článcích na webu TechNet [Managing a Server Core Installation](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) (Správa instalace Server Core) a [Servicing a Server Core Installation](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx) (Obsluha instalace Server Core). Možnost instalace Server Core se nevztahuje na určité edice systému Windows Server 2008 a Windows Server 2008 R2; další informace naleznete v části [Porovnání možností instalace Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**Tabulka 2**

 
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
<th colspan="6">
Windows XP
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS11-064**](http://go.microsoft.com/fwlink/?linkid=221808)
</td>
<td style="border:1px solid black;">
[**MS11-065**](http://go.microsoft.com/fwlink/?linkid=221880)
</td>
<td style="border:1px solid black;">
[**MS11-066**](http://go.microsoft.com/fwlink/?linkid=221536)
</td>
<td style="border:1px solid black;">
[**MS11-068**](http://go.microsoft.com/fwlink/?linkid=223578)
</td>
<td style="border:1px solid black;">
[**MS11-069**](http://go.microsoft.com/fwlink/?linkid=221537)
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
[**Mírný**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Žádný
</td>
<td style="border:1px solid black;">
[**Mírný**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=c07e1630-43ba-491e-bd59-9eb53105986c)  
(Mírný)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=6ca837f7-eda1-4ebe-b48a-8c77f949ebfd)<sup>[1]</sup>
(KB2487367)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=14fdbaa4-b42b-499c-819f-bb239b48a4cc)  
(KB2539631)  
(Mírný)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=e2069b12-d78b-420c-84b7-46bba12827c8)<sup>[1]</sup>
(KB2539636)  
(Mírný)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=797a01dc-39fb-4511-832a-42d2975133f5)  
(Mírný)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=6ca837f7-eda1-4ebe-b48a-8c77f949ebfd)<sup>[1]</sup>
(KB2487367)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=14fdbaa4-b42b-499c-819f-bb239b48a4cc)  
(KB2539631)  
(Mírný)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=e2069b12-d78b-420c-84b7-46bba12827c8)<sup>[1]</sup>
(KB2539636)  
(Mírný)
</td>
</tr>
<tr>
<th colspan="6">
Windows Server 2003
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS11-064**](http://go.microsoft.com/fwlink/?linkid=221808)
</td>
<td style="border:1px solid black;">
[**MS11-065**](http://go.microsoft.com/fwlink/?linkid=221880)
</td>
<td style="border:1px solid black;">
[**MS11-066**](http://go.microsoft.com/fwlink/?linkid=221536)
</td>
<td style="border:1px solid black;">
[**MS11-068**](http://go.microsoft.com/fwlink/?linkid=223578)
</td>
<td style="border:1px solid black;">
[**MS11-069**](http://go.microsoft.com/fwlink/?linkid=221537)
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
<td style="border:1px solid black;">
Žádný
</td>
<td style="border:1px solid black;">
[**Mírný**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=694ba1a6-7512-497d-a572-646a6e07b13b)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=6ca837f7-eda1-4ebe-b48a-8c77f949ebfd)<sup>[1]</sup>
(KB2487367)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=14fdbaa4-b42b-499c-819f-bb239b48a4cc)  
(KB2539631)  
(Mírný)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=e2069b12-d78b-420c-84b7-46bba12827c8)<sup>[1]</sup>
(KB2539636)  
(Mírný)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=308da543-d49d-4591-8bbc-d65c524bb0ad)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=6ca837f7-eda1-4ebe-b48a-8c77f949ebfd)<sup>[1]</sup>
(KB2487367)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=14fdbaa4-b42b-499c-819f-bb239b48a4cc)  
(KB2539631)  
(Mírný)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=e2069b12-d78b-420c-84b7-46bba12827c8)<sup>[1]</sup>
(KB2539636)  
(Mírný)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 SP2 pro systémy s procesorem Itanium
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=3b459bf0-7844-4740-895c-d149d56e781f)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=6ca837f7-eda1-4ebe-b48a-8c77f949ebfd)<sup>[1]</sup>
(KB2487367)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=14fdbaa4-b42b-499c-819f-bb239b48a4cc)  
(KB2539631)  
(Mírný)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=e2069b12-d78b-420c-84b7-46bba12827c8)<sup>[1]</sup>
(KB2539636)  
(Mírný)
</td>
</tr>
<tr>
<th colspan="6">
Windows Vista
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS11-064**](http://go.microsoft.com/fwlink/?linkid=221808)
</td>
<td style="border:1px solid black;">
[**MS11-065**](http://go.microsoft.com/fwlink/?linkid=221880)
</td>
<td style="border:1px solid black;">
[**MS11-066**](http://go.microsoft.com/fwlink/?linkid=221536)
</td>
<td style="border:1px solid black;">
[**MS11-068**](http://go.microsoft.com/fwlink/?linkid=223578)
</td>
<td style="border:1px solid black;">
[**MS11-069**](http://go.microsoft.com/fwlink/?linkid=221537)
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
Žádný
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
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=114c2835-921a-4d3e-be91-dfd217fd26a9)  
(Mírný)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=6ca837f7-eda1-4ebe-b48a-8c77f949ebfd)<sup>[1]</sup>
(KB2487367)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=9713b7b8-f260-440d-a994-845f17683fe9)  
(Mírný)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2f7348c0-a036-4d86-b7bb-bd6810cdc834)  
(KB2539633)  
(Mírný)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=e2069b12-d78b-420c-84b7-46bba12827c8)<sup>[1]</sup>
(KB2539636)  
(Mírný)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=0fcee476-8d7e-49a7-b6ea-89043304a653)  
(Mírný)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=6ca837f7-eda1-4ebe-b48a-8c77f949ebfd)<sup>[1]</sup>
(KB2487367)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4d67ec00-e86a-49b6-a9a2-85b2520fa4bb)  
(Mírný)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2f7348c0-a036-4d86-b7bb-bd6810cdc834)  
(KB2539633)  
(Mírný)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=e2069b12-d78b-420c-84b7-46bba12827c8)<sup>[1]</sup>
(KB2539636)  
(Mírný)
</td>
</tr>
<tr>
<th colspan="6">
Windows Server 2008
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS11-064**](http://go.microsoft.com/fwlink/?linkid=221808)
</td>
<td style="border:1px solid black;">
[**MS11-065**](http://go.microsoft.com/fwlink/?linkid=221880)
</td>
<td style="border:1px solid black;">
[**MS11-066**](http://go.microsoft.com/fwlink/?linkid=221536)
</td>
<td style="border:1px solid black;">
[**MS11-068**](http://go.microsoft.com/fwlink/?linkid=223578)
</td>
<td style="border:1px solid black;">
[**MS11-069**](http://go.microsoft.com/fwlink/?linkid=221537)
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
Žádný
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
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 pro 32bitové systémy Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro 32bitové systémy Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c01d9132-af5f-4039-8195-95f6761f2d0e)\*  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=6ca837f7-eda1-4ebe-b48a-8c77f949ebfd)\*\*<sup>[1]</sup>
(KB2487367)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro 32bitové systémy Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=da219735-b8b7-4f97-b8a8-7c253838de6b)\*\*\*  
(Mírný)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2f7348c0-a036-4d86-b7bb-bd6810cdc834)\*\*  
(KB2539633)  
(Mírný)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=e2069b12-d78b-420c-84b7-46bba12827c8)\*\*<sup>[1]</sup>
(KB2539636)  
(Mírný)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 pro systémy s procesorem x64 Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=70797adb-d693-4102-9e7c-ba1ea8fb07d0)\*  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=6ca837f7-eda1-4ebe-b48a-8c77f949ebfd)\*\*<sup>[1]</sup>
(KB2487367)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8e077af5-5823-4377-a997-44b022a694d8)\*\*\*  
(Mírný)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2f7348c0-a036-4d86-b7bb-bd6810cdc834)\*\*  
(KB2539633)  
(Mírný)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=e2069b12-d78b-420c-84b7-46bba12827c8)\*\*<sup>[1]</sup>
(KB2539636)  
(Mírný)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 pro systémy s procesorem Itanium Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=9babf81a-8b21-42ae-a65c-f414793516ab)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=6ca837f7-eda1-4ebe-b48a-8c77f949ebfd)<sup>[1]</sup>
(KB2487367)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=560efa6f-c956-47cb-a2f4-a1f45278b7cd)  
(Mírný)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2f7348c0-a036-4d86-b7bb-bd6810cdc834)  
(KB2539633)  
(Mírný)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=e2069b12-d78b-420c-84b7-46bba12827c8)<sup>[1]</sup>
(KB2539636)  
(Mírný)
</td>
</tr>
<tr>
<th colspan="6">
Windows 7
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS11-064**](http://go.microsoft.com/fwlink/?linkid=221808)
</td>
<td style="border:1px solid black;">
[**MS11-065**](http://go.microsoft.com/fwlink/?linkid=221880)
</td>
<td style="border:1px solid black;">
[**MS11-066**](http://go.microsoft.com/fwlink/?linkid=221536)
</td>
<td style="border:1px solid black;">
[**MS11-068**](http://go.microsoft.com/fwlink/?linkid=223578)
</td>
<td style="border:1px solid black;">
[**MS11-069**](http://go.microsoft.com/fwlink/?linkid=221537)
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
Žádný
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
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 pro 32bitové systémy a Windows 7 pro 32bitové systémy Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows 7 pro 32bitové systémy a Windows 7 pro 32bitové systémy Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=814bbdfa-7cbc-40e5-8ca3-8fed9d13ff00)  
(Mírný)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=6ca837f7-eda1-4ebe-b48a-8c77f949ebfd)<sup>[1]</sup>
(KB2487367)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows 7 pro 32bitové systémy a Windows 7 pro 32bitové systémy Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=6c8dd72b-abf8-4e1f-aafc-777c1a3ef3db)  
(Mírný)
</td>
<td style="border:1px solid black;">
Pouze Windows 7 pro 32bitové systémy:  
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=b8c628c6-5dcc-4c8f-b379-e2249a44f12c)  
(KB2539634)  
(Mírný)  
Pouze Windows 7 pro 32bitové systémy:  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=e2069b12-d78b-420c-84b7-46bba12827c8)<sup>[1]</sup>
(KB2539636)  
(Mírný)  
Pouze Windows 7 pro 32bitové systémy Service Pack 1:  
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=e1f84749-77bb-42bf-a539-fb647cacff8b)  
(KB2539635)  
(Mírný)  
Pouze Windows 7 pro 32bitové systémy Service Pack 1:  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=e2069b12-d78b-420c-84b7-46bba12827c8)<sup>[1]</sup>
(KB2539636)  
(Mírný)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 7 pro systémy s procesorem x64 a Windows 7 pro systémy s procesorem x64 Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows 7 pro systémy s procesorem x64 a Windows 7 pro systémy s procesorem x64 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=085ee785-b6ad-4c68-835a-e17bc8f12a53)  
(Mírný)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=6ca837f7-eda1-4ebe-b48a-8c77f949ebfd)<sup>[1]</sup>
(KB2487367)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows 7 pro systémy s procesorem x64 a Windows 7 pro systémy s procesorem x64 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=d90c07c1-3c07-4989-825c-fb8453541a0e)  
(Mírný)
</td>
<td style="border:1px solid black;">
Pouze Windows 7 pro systémy s procesorem x64:  
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=b8c628c6-5dcc-4c8f-b379-e2249a44f12c)  
(KB2539634)  
(Mírný)  
Pouze Windows 7 pro systémy s procesorem x64:  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=e2069b12-d78b-420c-84b7-46bba12827c8)<sup>[1]</sup>
(KB2539636)  
(Mírný)  
Pouze Windows 7 pro systémy s procesorem x64 Service Pack 1:  
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=e1f84749-77bb-42bf-a539-fb647cacff8b)  
(KB2539635)  
(Mírný)  
Pouze Windows 7 pro systémy s procesorem x64 Service Pack 1:  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=e2069b12-d78b-420c-84b7-46bba12827c8)<sup>[1]</sup>
(KB2539636)  
(Mírný)
</td>
</tr>
<tr>
<th colspan="6">
Windows Server 2008 R2
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS11-064**](http://go.microsoft.com/fwlink/?linkid=221808)
</td>
<td style="border:1px solid black;">
[**MS11-065**](http://go.microsoft.com/fwlink/?linkid=221880)
</td>
<td style="border:1px solid black;">
[**MS11-066**](http://go.microsoft.com/fwlink/?linkid=221536)
</td>
<td style="border:1px solid black;">
[**MS11-068**](http://go.microsoft.com/fwlink/?linkid=223578)
</td>
<td style="border:1px solid black;">
[**MS11-069**](http://go.microsoft.com/fwlink/?linkid=221537)
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
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Mírný**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Mírný**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 pro systémy s procesorem x64 a Windows Server 2008 R2 pro systémy s procesorem x64 Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem x64 a Windows Server 2008 R2 pro systémy s procesorem x64 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=9fd2b4ba-d98e-4ad6-99f2-c471335042d3)\*  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Pouze Windows Server 2008 R2 pro systémy s procesorem x64:  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=6ca837f7-eda1-4ebe-b48a-8c77f949ebfd)<sup>[1]</sup>
(KB2487367)  
(Vysoký)  
Pouze Windows Server 2008 R2 pro systémy s procesorem x64 Service Pack 1:  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=6ca837f7-eda1-4ebe-b48a-8c77f949ebfd)\*<sup>[1]</sup>
(KB2487367)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem x64 a Windows Server 2008 R2 pro systémy s procesorem x64 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=67cccd09-5b82-4546-884a-d2a9e2400820)\*\*\*  
(Mírný)
</td>
<td style="border:1px solid black;">
Pouze Windows Server 2008 R2 pro systémy s procesorem x64:  
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=b8c628c6-5dcc-4c8f-b379-e2249a44f12c)\*  
(KB2539634)  
(Mírný)  
Pouze Windows Server 2008 R2 pro systémy s procesorem x64:  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=e2069b12-d78b-420c-84b7-46bba12827c8)<sup>[1]</sup>
(KB2539636)  
(Mírný)  
Pouze Windows Server 2008 R2 pro systémy s procesorem x64 Service Pack 1:  
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=e1f84749-77bb-42bf-a539-fb647cacff8b)\*  
(KB2539635)  
(Mírný)  
Pouze Windows Server 2008 R2 pro systémy s procesorem x64 Service Pack 1:  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=e2069b12-d78b-420c-84b7-46bba12827c8)\*<sup>[1]</sup>
(KB2539636)  
(Mírný)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 pro systémy s procesorem Itanium a Windows Server 2008 R2 pro systémy s procesorem Itanium Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem Itanium a Windows Server 2008 R2 pro systémy s procesorem Itanium Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=93752c8f-5461-4e6f-9cab-6401b985ef17)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=6ca837f7-eda1-4ebe-b48a-8c77f949ebfd)<sup>[1]</sup>
(KB2487367)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem Itanium a Windows Server 2008 R2 pro systémy s procesorem Itanium Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=a1edf843-9a2a-4334-a95f-78e75a9b3ef1)  
(Mírný)
</td>
<td style="border:1px solid black;">
Pouze Windows Server 2008 R2 pro systémy s procesorem Itanium:  
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=b8c628c6-5dcc-4c8f-b379-e2249a44f12c)  
(KB2539634)  
(Mírný)  
Pouze Windows Server 2008 R2 pro systémy s procesorem Itanium:  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=e2069b12-d78b-420c-84b7-46bba12827c8)<sup>[1]</sup>
(KB2539636)  
(Mírný)  
Pouze Windows Server 2008 R2 pro systémy s procesorem Itanium Service Pack 1:  
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=e1f84749-77bb-42bf-a539-fb647cacff8b)  
(KB2539635)  
(Mírný)  
Pouze Windows Server 2008 R2 pro systémy s procesorem Itanium Service Pack 1:  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=e2069b12-d78b-420c-84b7-46bba12827c8)<sup>[1]</sup>
(KB2539636)  
(Mírný)
</td>
</tr>
</table>
<p></p>
 
**Poznámky k systémům Windows Server 2008 a Windows Server 2008 R2**

**\*Instalace Server Core obsahující chybu zabezpečení.** Tato aktualizace se stejným hodnocením závažnosti se vztahuje k podporovaným edicím systému Windows Server 2008 nebo Windows Server 2008 R2, jak je uvedeno, s instalací pomocí volby pro instalaci Server Core nebo bez ní. Další informace o této možnosti instalace naleznete v článcích na webu TechNet [Managing a Server Core Installation](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) (Správa instalace Server Core) a [Servicing a Server Core Installation](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx) (Obsluha instalace Server Core). Možnost instalace Server Core se nevztahuje na určité edice systému Windows Server 2008 a Windows Server 2008 R2; další informace naleznete v části [Porovnání možností instalace Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**\*\*Instalace Server Core není touto chybou ovlivněna.** Chyby zabezpečení, které tato aktualizace řeší, nemají vliv na podporované edice systému Windows Server 2008 nebo Windows Server 2008 R2, jak je uvedeno, v případě instalace s využitím možnosti instalace Server Core. Další informace o této možnosti instalace naleznete v článcích na webu TechNet [Managing a Server Core Installation](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) (Správa instalace Server Core) a [Servicing a Server Core Installation](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx) (Obsluha instalace Server Core). Možnost instalace Server Core se nevztahuje na určité edice systému Windows Server 2008 a Windows Server 2008 R2; další informace naleznete v části [Porovnání možností instalace Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**\*\*\*Instalace Server Core není touto chybou ovlivněna.** Chyba zabezpečení, kterou tato aktualizace řeší, nijak neovlivňuje podporované edice systémů Windows Server 2008 a Windows Server 2008 R2 v případě instalace s využitím možnosti instalace Server Core, i když se soubory postižené touto chybou zabezpečení mohou v systému vyskytovat. I přesto bude uživatelům se soubory postiženými těmito chybami tato aktualizace stále nabízena, neboť soubory aktualizace jsou novější (s vyššími čísly verze) než soubory, které jsou aktuálně ve vašem systému. Další informace o této možnosti instalace naleznete v článcích na webu TechNet [Managing a Server Core Installation](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) (Správa instalace Server Core) a [Servicing a Server Core Installation](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx) (Obsluha instalace Server Core). Možnost instalace Server Core se nevztahuje na určité edice systému Windows Server 2008 a Windows Server 2008 R2; další informace naleznete v části [Porovnání možností instalace Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**Poznámky k bulletinu MS11-066**

<sup>[1]</sup>**Rozhraní .NET Framework 4 Client Profile není postiženo.** Distribuční balíčky rozhraní .NET Framework verze 4 jsou k dispozici ve dvou profilech: .NET Framework 4 a .NET Framework 4 Client Profile. .NET Framework 4 Client Profile je verzí rozhraní .NET Framework 4. Chyba zabezpečení řešená v této aktualizaci se týká pouze rozhraní .NET Framework 4 a nikoli rozhraní .NET Framework 4 Client Profile. Další informace získáte v článku [Instalace rozhraní .NET Framework](http://msdn.microsoft.com/en-us/library/5a4x27ek.aspx) na webu MSDN.

Více aktualizovaných souborů v rámci stejného identifikátoru bulletinu naleznete také v dalších kategoriích softwaru v rámci této části **Software obsahující tuto chybu a umístění aktualizací ke stažení**. Tento bulletin se vztahuje na více kategorií softwaru.

**Poznámky k bulletinu MS11-069**

<sup>[1]</sup>**Postižena jsou rozhraní .NET Framework 4 a .NET Framework 4 Client Profile.** Distribuční balíčky rozhraní .NET Framework verze 4 jsou k dispozici ve dvou profilech: .NET Framework 4 a .NET Framework 4 Client Profile. Rozhraní .NET Framework 4 Client Profile je verzí rozhraní .NET Framework 4. Chyba zabezpečení řešená v této aktualizaci se týká jak rozhraní .NET Framework 4, tak rozhraní .NET Framework 4 Client Profile. Další informace získáte v článku [Instalace rozhraní .NET Framework](http://msdn.microsoft.com/en-us/library/5a4x27ek.aspx) na webu MSDN.

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
Microsoft Visio
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS11-060**](http://go.microsoft.com/fwlink/?linkid=223425)
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
Microsoft Visio 2003 Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Visio 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=866d64b3-7147-4b5f-80fe-4d3317f140df)  
(KB2553009)  
(Vysoký)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Visio 2007 Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft Visio 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=a0eeabde-5a92-45ae-aef6-81b7bdb4e0cd)  
(KB2553010)  
(Vysoký)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Visio 2010 a Microsoft Visio 2010 Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft Visio 2010 a Microsoft Visio 2010 Service Pack 1 (32bitové edice)](http://www.microsoft.com/downloads/details.aspx?familyid=6da236c2-0ef5-4c13-8393-673b70298a77)  
(KB2553008)  
(Vysoký)  
[Microsoft Visio 2010 a Microsoft Visio 2010 Service Pack 1 (64bitové edice)](http://www.microsoft.com/downloads/details.aspx?familyid=b7f5f2a9-116a-41ef-a19e-a7dd0947d2cb)  
(KB2553008)  
(Vysoký)
</td>
</tr>
</table>
<p></p>
 

#### Vývojářské nástroje a software společnosti Microsoft

 
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
Chart Control
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS11-066**](http://go.microsoft.com/fwlink/?linkid=221536)
</td>
<td style="border:1px solid black;">
[**MS11-067**](http://go.microsoft.com/fwlink/?linkid=223643)
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
</tr>
<tr>
<td style="border:1px solid black;">
Chart Control pro rozhraní Microsoft .NET Framework 3.5 Service Pack 1
</td>
<td style="border:1px solid black;">
[Chart Control pro rozhraní Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=8a80cc03-0db9-4446-9ce6-159ad02cab52)  
(KB2500170)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
</tr>
<tr>
<th colspan="3" style="border:1px solid black;">
Microsoft Visual Studio a Microsoft Report Viewer
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS11-066**](http://go.microsoft.com/fwlink/?linkid=221536)
</td>
<td style="border:1px solid black;">
[**MS11-067**](http://go.microsoft.com/fwlink/?linkid=223643)
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
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Visual Studio 2005 Service Pack 1
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Microsoft Visual Studio 2005 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=59231988-5413-4238-a3aa-32a127871430)  
(KB2548826)  
(Vysoký)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Report Viewer 2005 Service Pack 1 Redistributable Package
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Microsoft Report Viewer 2005 Service Pack 1 Redistributable Package](http://www.microsoft.com/downloads/details.aspx?familyid=28bf2ae0-9e21-4201-b7f1-a207abc2866f)  
(KB2579115)  
(Vysoký)
</td>
</tr>
</table>
<p></p>
 
**Poznámky k bulletinu MS11-066**

Více aktualizovaných souborů v rámci stejného identifikátoru bulletinu naleznete také v dalších kategoriích softwaru v rámci této části **Software obsahující tuto chybu a umístění aktualizací ke stažení**. Tento bulletin se vztahuje na více kategorií softwaru.

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

-   Yngve N. Pettersenovi ze společnosti [Opera Software ASA](http://www.opera.com/) za oznámení chyby popsané v bulletinu MS11-057.
-   Skupině [Lostmon Lords](http://lostmon.blogspot.com) za oznámení chyby popsané v bulletinu MS11-057.
-   Makoto Shiotsukimu ze společnosti [Security Professionals Network Inc.](http://www.sec-pro.net/) za oznámení chyby popsané v bulletinu MS11-057.
-   Anonymnímu výzkumníkovi, spolupracujícímu s organizací [TippingPoint](http://www.tippingpoint.com/) v rámci iniciativy [Zero Day Initiative](http://www.zerodayinitiative.com/), za oznámení chyby popsané v bulletinu MS11-057.
-   Stephenu Fewerovi ze společnosti [Harmony Security](http://www.harmonysecurity.com/), spolupracujícímu se společností [TippingPoint](http://www.tippingpoint.com/) v rámci iniciativy [Zero Day Initiative](http://www.zerodayinitiative.com/), za oznámení dvou chyb popsaných v bulletinu MS11-057.
-   Michalovi Zalewskému ze společnosti [Google Inc.](http://www.google.com/) za spolupráci na prvcích rozšíření ochrany zahrnutých v bulletinu MS11-057.
-   Grischovi Zengelovi ([Zengel Medizintechnik GmbH](http://www.zmt.info/)) za oznámení chyby popsané v bulletinu MS11-058.
-   Linlinu Zhaovi z [týmu zabezpečení společnosti Baidu](http://www.baidu.com) za oznámení dvou chyb popsaných v bulletinu MS11-060.
-   Svenovi Tautemu za oznámení chyby popsané v bulletinu MS11-061.
-   Lufeng Liovi ze společnosti za oznámení chyby popsané v bulletinu MS11-062.
-   Alexovi Ionescu ze společnosti Winsider Seminars & Solutions Inc. za oznámení chyby popsané v bulletinu MS11-063.
-   Nico Leideckerovi a Jamesi Forshawovi ze společnosti Context Information Security za oznámení chyby popsané v bulletinu MS11-066.
-   Adamovi Bixbymu ze společnosti [Gotham Digital Science](http://www.gdssecurity.com/) za oznámení chyby popsané v bulletinu MS11-067.
-   Zhengu Wenbinovi z [centra zabezpečení společnosti Qihoo 360](http://www.360.cn/) za oznámení chyby popsané v bulletinu MS11-068.
-   Michaelu J. Liuovi za oznámení chyby popsané v bulletinu MS11-069.

#### Technická podpora

-   Uvedený software byl testován za účelem zjištění, kterých verzí se chyba týká. U dalších verzí skončila časově omezená podpora. Pokud chcete zjistit dobu, po kterou je pro určitou verzi softwaru poskytována podpora, navštivte web [Zásady poskytování technické podpory pro produkty společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=21742).
-   Zákazníci mohou získat technickou podporu na webu [služby technické podpory společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=21131). Hovory související s aktualizacemi zabezpečení jsou bezplatné. Další informace o dostupných možnostech technické podpory naleznete na webu [Pomoc a podpora společnosti Microsoft](http://support.microsoft.com/).
-   Mezinárodní zákazníci získají podporu u místních zastoupení společnosti Microsoft. Technická podpora související s aktualizacemi zabezpečení je bezplatná. Další informace o možnostech kontaktování společnosti Microsoft v případě potřeby technické podpory získáte na [webu mezinárodní technické podpory](http://go.microsoft.com/fwlink/?linkid=21155).

#### Zřeknutí se záruky

Informace ve znalostní bázi Microsoft Knowledge Base jsou poskytovány tak, jak jsou, bez jakékoli záruky. Společnost Microsoft neposkytuje žádné záruky, výslovně uvedené či mlčky předpokládané, včetně záruk obchodovatelnosti a vhodnosti pro určitý účel. Společnost Microsoft ani její dodavatelé nenesou v žádném případě zodpovědnost za žádné škody, včetně přímých, nepřímých, náhodných či následných škod, ztráty zisku či zvláštních škod, a to ani v případě, že byli na možnost takových škod upozorněni. V některých zemích a právních řádech není dovoleno vyloučit nebo omezit odpovědnost, proto se výše uvedené omezení na vás nemusí vztahovat.

#### Revize

-   V1.0 (9. srpna 2011): Souhrnný bulletin byl publikován.
-   V1.1 (10. srpna 2011): U bulletinu MS11-059 došlo v části **Shrnutí** k opravě informace ohledně požadavku na restartování. U bulletinu MS11-065 došlo k opravě důležité poznámky týkající se **indexu zneužitelnosti** pro chybu zabezpečení CVE-2011-1968. U bulletinu MS11-068 došlo k revidování záznamu o jádrech serveru (Server Core) systémů Windows Server 2008 a Windows Server 2008 R2.
-   V1.2 (26. října 2011): V bulletinu MS11-066 a MS11-069 byla opravena informace o použitelnosti instalace Server Core pro rozhraní .NET Framework 4 v systému Windows Server 2008 R2 pro systémy s procesorem x64.

*Built at 2014-04-18T01:50:00Z-07:00*
