---
TOCTitle: 'MS11-APR'
Title: 'Souhrnný bulletin zabezpečení společnosti Microsoft, duben 2011'
ms:assetid: 'ms11-apr'
ms:contentKeyID: 61224006
ms:mtpsurl: 'https://technet.microsoft.com/cs-CZ/library/ms11-apr(v=Security.10)'
---

 

Souhrnný bulletin zabezpečení společnosti Microsoft, duben 2011
===============================================================

Publikováno: 12. dubna 2011 | Aktualizováno: 26. října 2011

**Verze:** 6.1

Tento souhrnný bulletin uvádí bulletiny zabezpečení vydané v dubnu 2011.

Spolu s vydáním bulletinů zabezpečení pro duben 2011 nahrazuje tento souhrnný bulletin předběžné oznámení o bulletinech vydané 7. dubna 2011. Další informace o službě předběžného oznámení o bulletinech naleznete v části [Předběžné oznámení o bulletinech zabezpečení společnosti Microsoft](http://technet.microsoft.com/security/bulletin/advance).

Informace o tom, jak dostávat automatická oznámení o vydání nových bulletinů zabezpečení společnosti Microsoft, naleznete na webu [Zasílání technických oznámení o zabezpečení společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=21163).

Pro zodpovězení zákaznických dotazů týkajících se těchto bulletinů uspořádá společnost Microsoft 13. dubna 2011 v 11:00 časového pásma Tichomoří (USA a Kanada) webové vysílání. [Přihlaste se k webovému vysílání týkajícímu se dubnových bulletinů zabezpečení](https://msevents.microsoft.com/cui/webcasteventdetails.aspx?culture=en-us&eventid=1032455069&eventcategory=4). Po tomto datu je webové vysílání dostupné na požádání. Další informace získáte v [souhrnných bulletinech zabezpečení společnosti Microsoft a webovém vysílání](http://technet.microsoft.com/security/bulletin/summary).

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
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=214126">MS11-018</a></td>
<td style="border:1px solid black;"><strong>Kumulativní aktualizace zabezpečení aplikace Internet Explorer (2497640)</strong><br />
<br />
Tato aktualizace zabezpečení řeší čtyři chyby zabezpečení oznámené soukromými osobami a jednu veřejně známou chybu zabezpečení v aplikaci Internet Explorer. Tato aktualizace zabezpečení má kritický stupeň závažnosti pro aplikace Internet Explorer 6, Internet Explorer 7 a Internet Explorer 8 v klientských počítačích se systémem Windows a mírný pro aplikace Internet Explorer 6, Internet Explorer 7 a Internet Explorer 8 na serverech se systémem Windows. Aplikace Internet Explorer 9 není těmito chybami zabezpečení ohrožena.<br />
<br />
Nejzávažnější chyby zabezpečení mohou umožnit vzdálené spuštění kódu, pokud uživatel pomocí aplikace Internet Explorer zobrazí speciálně vytvořenou webovou stránku. Útočník, který by úspěšně zneužil některou z těchto chyb zabezpečení, by mohl získat stejná uživatelská práva, jaká má místní uživatel. Uživatelé, jejichž účty jsou konfigurovány tak, aby měli v systému méně uživatelských práv, by byli vystaveni menšímu riziku než uživatelé s uživatelskými právy správce.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritický</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Internet Explorer</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=212314">MS11-019</a></td>
<td style="border:1px solid black;"><strong>Chyby zabezpečení v klientu SMB umožňují vzdálené spuštění kódu (2511455)</strong><br />
<br />
Tato aktualizace zabezpečení řeší jednu veřejně známou a jednu soukromou osobou oznámenou chybu zabezpečení systému Microsoft Windows. Závažnější z těchto chyb zabezpečení by mohla umožnit vzdálené spuštění kódu, pokud by útočník odeslal speciálně vytvořenou odpověď SMB na požadavek SMB vyvolaný klientem. Chce-li útočník tuto chybu zneužít, musel by přesvědčit uživatele, aby navázal spojení SMB se speciálně vytvořeným serverem SMB.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritický</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=212236">MS11-020</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení v serveru SMB umožňuje vzdálené spuštění kódu (2508429)</strong><br />
<br />
Tato aktualizace zabezpečení řeší chybu zabezpečení v systému Microsoft Windows, kterou oznámila soukromá osoba. Tato chyba zabezpečení by mohla umožnit vzdálené spuštění kódu v případě, že by útočník vytvořil speciálně vytvořený paket SMB a odeslal jej do postiženého systému. Doporučené postupy pro používání brány firewall a standardní konfigurace této brány zajišťují ochranu sítí před útoky pocházejícími z oblasti mimo rozlehlou síť, které by se pokusily zneužít tyto chyby zabezpečení.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritický</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=214005">MS11-027</a></td>
<td style="border:1px solid black;"><strong>Kumulativní aktualizace zabezpečení dezaktivačních bitů ActiveX (2508272)</strong><br />
<br />
Tato aktualizace zabezpečení řeší dvě chyby zabezpečení oznámené soukromými osobami a jednu veřejně známou chybu zabezpečení v softwaru společnosti Microsoft. Tyto chyby zabezpečení mohou umožnit vzdálené spuštění kódu, pokud uživatel pomocí aplikace Internet Explorer zobrazí speciálně vytvořenou webovou stránku, jež vytváří instanci konkrétního ovládacího prvku ActiveX. Uživatelé, jejichž účty jsou konfigurovány tak, aby měli v systému méně uživatelských práv, by byli vystaveni menšímu riziku než uživatelé s uživatelskými právy správce. Tato aktualizace také obsahuje dezaktivační bity pro tři ovládací prvky ActiveX jiných výrobců.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritický</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Může vyžadovat restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=207931">MS11-028</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení v rozhraní .NET Framework umožňuje vzdálené spuštění kódu (2484015)</strong><br />
<br />
Tato aktualizace zabezpečení řeší veřejně oznámenou chybu zabezpečení v rozhraní Microsoft .NET Framework. Tyta chyba zabezpečení by mohla umožnit vzdálené spuštění kódu v klientském systému, pokud by uživatel zobrazil speciálně vytvořenou webovou stránku pomocí webového prohlížeče, v němž lze otevírat aplikace prohlížeče XAML (XBAP). Uživatelé, jejichž účty jsou konfigurovány tak, aby měli v systému méně uživatelských práv, by byli vystaveni menšímu riziku než uživatelé s uživatelskými právy správce. Chyba zabezpečení dále může umožnit vzdálené spuštění kódu na serverovém systému se službou IIS v případě, že tento server umožňuje zpracování stránek ASP.NET a útočníkovi se úspěšně podaří na daném serveru načíst speciálně vytvořenou stránku ASP.NET a poté ji spustit, jako například v případě hostování webu. Tuto chybu zabezpečení mohou zneužít také aplikace Windows .NET k obejití omezení zabezpečení přístupu kódu (CAS).</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritický</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Může vyžadovat restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=208524">MS11-029</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení v rozhraní GDI+ umožňuje vzdálené spuštění kódu (2489979)</strong><br />
<br />
Tato aktualizace zabezpečení řeší chybu zabezpečení v rozhraní GDI+ systému Microsoft Windows, kterou oznámila soukromá osoba. Tato chyba zabezpečení může umožnit vzdálené spuštění kódu, pokud uživatel pomocí postiženého softwaru otevře speciálně vytvořený soubor s obrázkem nebo přejde na web, který obsahuje speciálně vytvořený obsah. Uživatelé, jejichž účty jsou konfigurovány tak, aby měli v systému méně uživatelských práv, by byli vystaveni menšímu riziku než uživatelé s uživatelskými právy správce.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritický</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Může vyžadovat restartování</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Microsoft Office</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=212595">MS11-030</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení v překladu názvů DNS umožňuje vzdálené spuštění kódu (2509553)</strong><br />
<br />
Tato aktualizace zabezpečení řeší chybu zabezpečení v překladu názvů Windows DNS, kterou oznámila soukromá osoba. Tato chyba zabezpečení by mohla povolit vzdálené spuštění kódu, pokud útočník získá přístup do sítě a následně vytvoří vlastní program určený k odeslání speciálně vytvořených dotazů vysílání LLMNR do cílových systémů. Doporučené postupy pro používání brány firewall a standardní konfigurace této brány zajišťují ochranu sítí před útoky pocházejícími z oblasti mimo rozlehlou síť. Je vhodné, aby systémy připojené k Internetu měly přístupný minimální počet portů. V tomto případě by měly být porty LLMNR zablokovány vůči Internetu.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritický</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=212243">MS11-031</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení ve skriptovacích strojích jazyků JScript a VBScript</strong> <strong>umožňuje vzdálené spuštění kódu (2514666)</strong><br />
<br />
Tato aktualizace zabezpečení řeší chybu zabezpečení ve skriptovacích strojích jazyků JScript a VBScript oznámenou soukromou osobou. Tato chyba zabezpečení umožňuje vzdálené spuštění kódu, pokud by uživatel navštívil speciálně vytvořený web. Útočník nemůže žádným způsobem přinutit uživatele k návštěvě takového webu. Místo toho by útočník musel přesvědčit uživatele, aby navštívili takový web. K tomu se obvykle používá odkaz v e-mailu nebo zpráva programu pro zasílání rychlých zpráv, na které uživatelé kliknou, a přejdou tak na útočníkův web.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritický</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Může vyžadovat restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=212224">MS11-032</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení v ovladači písma OpenType formátu CFF (Compact Font Format) umožňuje vzdálené spuštění kódu (2507618)</strong><br />
<br />
Tato aktualizace zabezpečení řeší soukromě oznámenou chybu zabezpečení v ovladači písma OpenType formátu CFF (Compact Font Format). Tato chyba zabezpečení by mohla umožnit vzdálené spuštění kódu, pokud by uživatel zobrazil obsah ve speciálně vytvořeném písmu CFF. Útočník nemůže žádným způsobem přinutit uživatele k zobrazení speciálně vytvořeného obsahu. Místo toho by útočník musel přesvědčit uživatele, aby navštívili takový web. K tomu se obvykle používá odkaz v e-mailu nebo zpráva programu pro zasílání rychlých zpráv, na které uživatelé kliknou a přejdou tak na útočníkův web.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritický</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=210121">MS11-021</a></td>
<td style="border:1px solid black;"><strong>Chyby zabezpečení v aplikaci Microsoft Excel umožňují vzdálené spuštění kódu (2489279)</strong><br />
<br />
Tato aktualizace zabezpečení řeší devět chyb zabezpečení v systému Microsoft Office oznámených soukromými osobami. Chyby umožňují vzdálené spuštění kódu, pokud uživatel otevře speciálně vytvořený soubor aplikace Excel. Útočník, který by úspěšně zneužil některou z těchto chyb zabezpečení, by mohl získat stejná uživatelská práva, jaká má přihlášený uživatel. Uživatelé, jejichž účty jsou konfigurovány tak, aby měli v systému méně uživatelských práv, by byli vystaveni menšímu riziku než uživatelé s uživatelskými právy správce.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Vysoký</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Může vyžadovat restartování</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=210727">MS11-022</a></td>
<td style="border:1px solid black;"><strong>Chyby zabezpečení aplikace Microsoft PowerPoint umožňují vzdálené spuštění kódu (2489283)</strong><br />
<br />
Tato aktualizace zabezpečení řeší tři chyby zabezpečení v aplikaci Microsoft PowerPoint oznámené soukromými osobami. Chyby umožňují vzdálené spuštění kódu, pokud uživatel otevře speciálně vytvořený soubor aplikace PowerPoint. Útočník, který by úspěšně zneužil některou z těchto chyb zabezpečení, by mohl získat stejná uživatelská práva, jaká má místní uživatel. Uživatelé, jejichž účty jsou konfigurovány tak, aby měli v systému méně uživatelských práv, by byli vystaveni menšímu riziku než uživatelé s uživatelskými právy správce. Automatizované řešení <strong>Microsoft Fix It</strong> pro aplikaci PowerPoint 2010 s názvem „Disable Edit in Protected View for PowerPoint 2010“ (Aplikace PowerPoint 2010 neumožňuje úpravy v chráněném zobrazení), dostupné v <a href="http://support.microsoft.com/kb/2501584">článku 2501584 znalostní báze Microsoft Knowledge Base</a>, blokuje způsoby útoku pokoušející se o zneužití chyb zabezpečení CVE-2011-0655 a CVE-2011-0656.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Vysoký</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Může vyžadovat restartování</td>
<td style="border:1px solid black;">Microsoft Office,<br />
Microsoft Server Software</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=210206">MS11-023</a></td>
<td style="border:1px solid black;"><strong>Chyby zabezpečení systému Microsoft Office umožňují vzdálené</strong> <strong>spuštění kódu (2489293)</strong><br />
<br />
Tato aktualizace zabezpečení řeší jednu veřejně známou a jednu soukromou osobou oznámenou chybu zabezpečení systému Microsoft Office. Tyto chyby umožňují vzdálené spuštění kódu, pokud uživatel otevře speciálně vytvořený soubor systému Office nebo pokud otevře legitimní soubor systému Office umístěný ve stejném síťovém adresáři jako speciálně vytvořený soubor knihovny. Útočník, který by úspěšně zneužil některou z těchto chyb zabezpečení, by mohl získat stejná uživatelská práva, jaká má přihlášený uživatel. Uživatelé, jejichž účty jsou konfigurovány tak, aby měli v systému méně uživatelských práv, by byli vystaveni menšímu riziku než uživatelé s uživatelskými právy správce.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Vysoký</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Může vyžadovat restartování</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=212226">MS11-024</a></td>
<td style="border:1px solid black;"><strong>Chyby zabezpečení v editoru titulních stránek faxových zpráv systému Windows umožňují vzdálené spuštění kódu (2527308)</strong><br />
<br />
Tato aktualizace zabezpečení řeší dvě veřejně známé chyby zabezpečení v systému Microsoft Windows. Tyto chyby zabezpečení umožňují vzdálené spuštění kódu, pokud uživatel otevře speciálně vytvořený soubor titulní stránky (s příponou COV) v editoru titulních stránek faxových zpráv systému Windows. Útočník, který by úspěšně zneužil některou z těchto chyb zabezpečení, by mohl získat stejná uživatelská práva, jaká má přihlášený uživatel. Uživatelé, jejichž účty jsou konfigurovány tak, aby měli v systému méně uživatelských práv, by byli vystaveni menšímu riziku než uživatelé s uživatelskými právy správce.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Vysoký</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Může vyžadovat restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=209720">MS11-025</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení v knihovně MFC (Microsoft Foundation Class) umožňuje vzdálené</strong> <strong>spuštění kódu (2500212)</strong><br />
<br />
Tato aktualizace zabezpečení řeší veřejně známou chybu zabezpečení v určitých aplikacích vytvořených pomocí knihovny MFC (Microsoft Foundation Class). Tato chyba zabezpečení by mohla umožnit vzdálené spuštění kódu, pokud by uživatel otevřel legitimní soubor spojený s takto postiženou aplikací a soubor by byl umístěný ve stejné síťové složce jako speciálně vytvořený soubor knihovny. Úspěšný útok by vyžadoval, aby útočník navštívil nedůvěryhodné systémové umístění vzdáleného souboru nebo sdílenou složku protokolu WebDAV a otevřel z tohoto umístění dokument, který by pak načetla postižená aplikace.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Vysoký</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Může vyžadovat restartování</td>
<td style="border:1px solid black;">Vývojářské nástroje a software společnosti Microsoft</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=212523">MS11-026</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení standardu MHTML může umožnit přístup k informacím (2503658)</strong><br />
<br />
Tato aktualizace zabezpečení řeší veřejně známou chybu zabezpečení v popisovači standardu MHTML v systému Microsoft Windows. Uvedená chyba zabezpečení umožňuje zpřístupnění informací, pokud uživatel navštíví speciálně vytvořenou webovou stránku. V případě útoku z webu by určitý web mohl obsahovat speciálně vytvořený odkaz, který by umožňoval zneužití uvedené chyby zabezpečení. Útočník by musel uživatele přesvědčit, aby daný web navštívili a otevřeli speciálně vytvořený odkaz.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Vysoký</a><br />
Přístup k informacím</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=208110">MS11-033</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení textových převaděčů WordPad umožňuje vzdálené spuštění kódu (2485663)</strong><br />
<br />
Tato aktualizace zabezpečení řeší chybu zabezpečení v systému Microsoft Windows, kterou oznámila soukromá osoba. Tato aktualizace zabezpečení je označena jako důležitá pro všechny podporované verze systému Windows XP a Windows Server 2003. Všechny podporované edice systémů Windows Vista, Windows Server 2008, Windows 7 a Windows Server 2008 R2 nejsou postiženy zmíněnou chybou zabezpečení.<br />
<br />
Tato chyba zabezpečení umožňuje vzdálené spuštění kódu, pokud uživatel otevře speciálně vytvořený soubor pomocí programu WordPad. Útočník, který by úspěšně zneužil tuto chybu zabezpečení, by mohl získat stejná uživatelská práva, jako má místní uživatel. Uživatelé, jejichž účty jsou konfigurovány tak, aby měli v systému méně uživatelských práv, by byli vystaveni menšímu riziku než uživatelé s uživatelskými právy správce.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Vysoký</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Může vyžadovat restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;"><strong>Chyby zabezpečení v ovladačích režimu jádra systému Windows umožňují zvýšení úrovně oprávnění (2506223)</strong><br />
<br />
Tato aktualizace zabezpečení řeší třicet chyb zabezpečení v systému Microsoft Windows oznámených soukromou osobou. Tyto chyby zabezpečení by mohly umožnit zvýšení úrovně oprávnění, pokud by se útočník místně přihlásil k systému a spustil speciálně vytvořenou aplikaci. Tyto chyby zabezpečení může zneužít pouze útočník s platnými pověřeními pro přihlášení, která by mu umožňovala se místně přihlásit. Uvedené chyby zabezpečení nemohou zneužít vzdálení ani anonymní uživatelé.</td>
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
  

Následující tabulka uvádí hodnocení zneužitelnosti každé chyby zabezpečení uvedené v tomto měsíci. Chyby zabezpečení jsou řazeny v pořadí zmenšující se úrovně posouzení zneužitelnosti, jinak než tomu je u řazení podle čísla chyb. Uvedeny jsou pouze chyby zabezpečení ohodnocené stupněm závažnosti Kritický nebo Vysoký.
  
**Jak** **pracovat s touto tabulkou**
  
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
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=209720">MS11-025</a></td>
<td style="border:1px solid black;">Chyba zabezpečení nezabezpečeného načítání knihovny MFC</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3190">CVE-2010-3190</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;">Tato chyba zabezpečení je veřejně známá.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=207931">MS11-028</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se poškození zásobníku záznamů rozhraní .NET Framework</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3958">CVE-2010-3958</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;">Tato chyba zabezpečení je veřejně známá.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=212224">MS11-032</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se přetečení zásobníku písma OpenType</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0034">CVE-2011-0034</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=208524">MS11-029</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se přetečení celého čísla GDI+</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0041">CVE-2011-0041</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=214126">MS11-018</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se poškození paměti při zpracování rozložení</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0094">CVE-2011-0094</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;"><strong>V současné době dochází ke zneužití této chyby zabezpečení</strong> <strong>v rámci omezených cílených útoků.</strong></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=210121">MS11-021</a></td>
<td style="border:1px solid black;">Chyba zabezpečení celočíselného přetečení aplikace Excel</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0097">CVE-2011-0097</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=210121">MS11-021</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se přetečení haldy aplikace Excel</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0098">CVE-2011-0098</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=210121">MS11-021</a></td>
<td style="border:1px solid black;">Chyba zabezpečení skriptu WriteAV analýzy záznamu aplikace Excel</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0101">CVE-2011-0101</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=210206">MS11-023</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se nezabezpečeného načítání knihovny součásti systému Office</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0107">CVE-2011-0107</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;">Tato chyba zabezpečení je veřejně známá.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=214126">MS11-018</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se poškození paměti modulu rozložení MSHTML</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0346">CVE-2011-0346</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;">Tato chyba zabezpečení je veřejně známá.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=212314">MS11-019</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se analýzy odpovědi klienta SMB</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0660">CVE-2011-0660</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=212236">MS11-020</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se analýzy transakce SMB</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0661">CVE-2011-0661</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se použití subsystému Win32k po uvolnění</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0662">CVE-2011-0662</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se použití subsystému Win32k po uvolnění</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0665">CVE-2011-0665</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se použití subsystému Win32k po uvolnění</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0666">CVE-2011-0666</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se použití subsystému Win32k po uvolnění</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0667">CVE-2011-0667</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se použití subsystému Win32k po uvolnění</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0670">CVE-2011-0670</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se použití subsystému Win32k po uvolnění</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0671">CVE-2011-0671</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se použití subsystému Win32k po uvolnění</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0672">CVE-2011-0672</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se vyhodnocování ukazatele Win32k Null</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0673">CVE-2011-0673</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se použití subsystému Win32k po uvolnění</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0674">CVE-2011-0674</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se použití subsystému Win32k po uvolnění</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0675">CVE-2011-0675</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se vyhodnocování ukazatele Win32k Null</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0676">CVE-2011-0676</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se vyhodnocování ukazatele Win32k Null</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0677">CVE-2011-0677</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=210727">MS11-022</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se vzdáleného spuštění kódu OfficeArt Atom</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0976">CVE-2011-0976</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=210121">MS11-021</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se indexování pole aplikace Excel</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0978">CVE-2011-0978</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=210121">MS11-021</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se poškození propojeného seznamu aplikace Excel</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0979">CVE-2011-0979</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=210121">MS11-021</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se rozdělovacího ukazatele aplikace Excel</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0980">CVE-2011-0980</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se vyhodnocování ukazatele Win32k Null</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1225">CVE-2011-1225</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se vyhodnocování ukazatele Win32k Null</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1226">CVE-2011-1226</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se vyhodnocování ukazatele Win32k Null</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1227">CVE-2011-1227</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se vyhodnocování ukazatele Win32k Null</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1228">CVE-2011-1228</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se vyhodnocování ukazatele Win32k Null</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1229">CVE-2011-1229</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se vyhodnocování ukazatele Win32k Null</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1230">CVE-2011-1230</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se vyhodnocování ukazatele Win32k Null</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1231">CVE-2011-1231</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se vyhodnocování ukazatele Win32k Null</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1232">CVE-2011-1232</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se vyhodnocování ukazatele Win32k Null</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1233">CVE-2011-1233</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se použití subsystému Win32k po uvolnění</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1235">CVE-2011-1235</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se použití subsystému Win32k po uvolnění</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1236">CVE-2011-1236</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se použití subsystému Win32k po uvolnění</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1237">CVE-2011-1237</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se použití subsystému Win32k po uvolnění</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1239">CVE-2011-1239</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se použití subsystému Win32k po uvolnění</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1240">CVE-2011-1240</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se použití subsystému Win32k po uvolnění</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1241">CVE-2011-1241</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se použití subsystému Win32k po uvolnění</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1242">CVE-2011-1242</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=214126">MS11-018</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se poškození paměti správy objektů</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1345">CVE-2011-1345</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Konsistentní zneužití kódu je pravděpodobné</td>
<td style="border:1px solid black;"><strong>V současné době dochází ke zneužití této chyby zabezpečení v rámci omezených</strong> <strong>cílených útoků.</strong></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=208110">MS11-033</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se analýzy převaděče WordPad</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0028">CVE-2011-0028</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">2</a> – Je pravděpodobné vytvoření kódu nekonsistentního zneužití</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=210121">MS11-021</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se poškození paměti aplikace Excel</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0103">CVE-2011-0103</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">2</a> – Je pravděpodobné vytvoření kódu nekonsistentního zneužití</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=210121">MS11-021</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se přepsání vyrovnávací paměti aplikace Excel</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0104">CVE-2011-0104</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">2</a> – Je pravděpodobné vytvoření kódu nekonsistentního zneužití</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=210121">MS11-021</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se inicializace dat aplikace Excel</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0105">CVE-2011-0105</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">2</a> – Je pravděpodobné vytvoření kódu nekonsistentního zneužití</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=212314">MS11-019</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se poškození fondu prohlížeče</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0654">CVE-2011-0654</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">2</a> – Je pravděpodobné vytvoření kódu nekonsistentního zneužití</td>
<td style="border:1px solid black;">Tato chyba zabezpečení je veřejně známá.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=210727">MS11-022</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se vzdáleného spuštění kódu Floating Point Techno-color Time Bandit</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0655">CVE-2011-0655</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">2</a> – Je pravděpodobné vytvoření kódu nekonsistentního zneužití</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=210727">MS11-022</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se vzdáleného spuštění kódu trvalého adresáře</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0656">CVE-2011-0656</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">2</a> – Je pravděpodobné vytvoření kódu nekonsistentního zneužití</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=212595">MS11-030</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se požadavku DNS</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0657">CVE-2011-0657</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">2</a> – Je pravděpodobné vytvoření kódu nekonsistentního zneužití</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=212243">MS11-031</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se přerozdělení skriptovací paměti</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0663">CVE-2011-0663</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">2</a> – Je pravděpodobné vytvoření kódu nekonsistentního zneužití</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=210206">MS11-023</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se vyhodnocování grafického objektu aplikace Microsoft Office</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0977">CVE-2011-0977</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">2</a> – Je pravděpodobné vytvoření kódu nekonsistentního zneužití</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se použití subsystému Win32k po uvolnění</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1234">CVE-2011-1234</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">2</a> – Je pravděpodobné vytvoření kódu nekonsistentního zneužití</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=212226">MS11-024</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se poškození paměti editoru titulních stránek faxových zpráv</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3974">CVE-2010-3974</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">3</a> – Vytvoření kódu funkčního zneužití není pravděpodobné</td>
<td style="border:1px solid black;">Tato chyba zabezpečení je veřejně známá.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=212226">MS11-024</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se použití titulních stránek faxových zpráv po uvolnění</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-4701">CVE-2010-4701</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">3</a> – Vytvoření kódu funkčního zneužití není pravděpodobné</td>
<td style="border:1px solid black;">Tato chyba zabezpečení je veřejně známá.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=212523">MS11-026</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se požadavku na rozložení ve formátu MHTML Mime</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0096">CVE-2011-0096</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">3</a> – Vytvoření kódu funkčního zneužití není pravděpodobné</td>
<td style="border:1px solid black;">Tato chyba zabezpečení je veřejně známá.<br />
<br />
Jedná se o chybu zabezpečení typu zpřístupnění informací.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se použití subsystému Win32k po uvolnění</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1238">CVE-2011-1238</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">3</a> – Vytvoření kódu funkčního zneužití není pravděpodobné</td>
<td style="border:1px solid black;">(Žádné)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=214126">MS11-018</a></td>
<td style="border:1px solid black;">Chyba zabezpečení týkající se zpřístupnění informací skriptu Javascript</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1245">CVE-2011-1245</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">3</a> – Vytvoření kódu funkčního zneužití není pravděpodobné</td>
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
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
</tr>
<tr>
<th colspan="14" style="border:1px solid black;">
Windows XP  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS11-018**](http://go.microsoft.com/fwlink/?linkid=214126)
</td>
<td style="border:1px solid black;">
[**MS11-019**](http://go.microsoft.com/fwlink/?linkid=212314)
</td>
<td style="border:1px solid black;">
[**MS11-020**](http://go.microsoft.com/fwlink/?linkid=212236)
</td>
<td style="border:1px solid black;">
[**MS11-027**](http://go.microsoft.com/fwlink/?linkid=214005)
</td>
<td style="border:1px solid black;">
[**MS11-028**](http://go.microsoft.com/fwlink/?linkid=207931)
</td>
<td style="border:1px solid black;">
[**MS11-029**](http://go.microsoft.com/fwlink/?linkid=208524)
</td>
<td style="border:1px solid black;">
[**MS11-030**](http://go.microsoft.com/fwlink/?linkid=212595)
</td>
<td style="border:1px solid black;">
[**MS11-031**](http://go.microsoft.com/fwlink/?linkid=212243)
</td>
<td style="border:1px solid black;">
[**MS11-032**](http://go.microsoft.com/fwlink/?linkid=212224)
</td>
<td style="border:1px solid black;">
[**MS11-024**](http://go.microsoft.com/fwlink/?linkid=212226)
</td>
<td style="border:1px solid black;">
[**MS11-026**](http://go.microsoft.com/fwlink/?linkid=212523)
</td>
<td style="border:1px solid black;">
[**MS11-033**](http://go.microsoft.com/fwlink/?linkid=208110)
</td>
<td style="border:1px solid black;">
[**MS11-034**](http://go.microsoft.com/fwlink/?linkid=211826)
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
[**Kritický**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritický**](http://go.microsoft.com/fwlink/?linkid=21140)
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
[Aplikace Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=c3a8cec0-f947-4d4e-a6ae-c7f4f1f311b0)  
(Kritický)  
[Aplikace Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=0b7d0403-8965-4c62-970c-20b561f66713)  
(Kritický)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=689c5496-56c4-48a6-9f3d-b5f5aaf3e566)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=f5378e7b-4619-4c42-9d9f-87b209c6d878)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=ccb08a8a-f4d9-4320-8ffb-3fd4fe217987)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=b031a496-aa74-4367-b2ae-24843c061745)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 Service Pack 2 a Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=ce925e76-cb85-48f6-8c0f-e53fa2b09be6)  
(KB2446704)  
(Kritický)  
[Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=91aa6772-4811-4a58-9bc0-8aa271ed99df)<sup>[1]</sup>
(KB2446708)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=59266a9d-a319-4309-a046-7f15c6da0136)  
(KB2412687)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=2d433adb-bcaf-4c59-9405-a4892f8ccba3)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[JScript 5.7 a VBScript 5.7](http://www.microsoft.com/downloads/details.aspx?familyid=637f4d4c-de07-4c6a-95f8-3bd0cbfe77b2)  
(KB2510581)  
(Kritický)  
[JScript 5.8 a VBScript 5.8](http://www.microsoft.com/downloads/details.aspx?familyid=fbe1e7e3-1d5f-4daf-a4a5-67fe79292963)  
(KB2510531)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=9080c5a1-e638-4047-a70a-9367f1acced7)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=50fc3869-f2fc-43c8-8049-aad62f2cb332)  
(KB2491683)  
(Vysoký)  
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=a8220a21-02fc-4ad6-988d-844276b2fd66)  
(KB2506212)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=7f0a4616-8e3e-4925-9d95-ce6e614e45ae)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=6753ca98-feb4-4c7f-9969-9294038a2bbb)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=39e55bbf-c1c5-4696-bfe7-632e997cd98e)  
(Vysoký)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Aplikace Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=986f07ae-0fdc-4be2-8a74-5eb56d4300ef)  
(Kritický)  
[Aplikace Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=ed88f183-dd06-46f6-ae8a-a594a752f248)  
(Kritický)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=6d3433ee-c2e1-433f-a3d9-c049d66e2190)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c01441da-8933-4f60-923b-d9b00db8ba3d)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7ee202da-a711-42ee-bea3-7202a70e4ea0)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=eddd2964-9765-461d-9df8-2c05402948e8)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 Service Pack 2 a Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=ce925e76-cb85-48f6-8c0f-e53fa2b09be6)  
(KB2446704)  
(Kritický)  
[Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=91aa6772-4811-4a58-9bc0-8aa271ed99df)<sup>[1]</sup>
(KB2446708)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3797009a-b9a4-4e83-8614-e1589c8b5090)  
(KB2412687)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=29ff546e-a232-4f23-a223-c029c71ff1c6)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[JScript 5.6 a VBScript 5.6](http://www.microsoft.com/downloads/details.aspx?familyid=a5586246-2908-4def-9298-c16060098197)  
(KB2510587)  
(Kritický)  
[JScript 5.7 a VBScript 5.7](http://www.microsoft.com/downloads/details.aspx?familyid=3a5f65e0-bb00-4e55-b8b5-77751349a3ec)  
(KB2510581)  
(Kritický)  
[JScript 5.8 a VBScript 5.8](http://www.microsoft.com/downloads/details.aspx?familyid=57aa7ee2-254d-40b5-9ff0-cba969daf45a)  
(KB2510531)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2374e09a-cb3e-4bc3-bb4b-53b611025121)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b93311b4-1b8f-478d-8833-750c5e01e6f8)  
(KB2491683)  
(Vysoký)  
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=0f60fc99-cd88-4237-8b31-a4e618502f7e)  
(KB2506212)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b01fe9a5-66a4-4683-963b-e78aea214579)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3c94bc96-99ea-44a1-9052-e69de5e21f81)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=83771177-284e-4918-86a9-980e8229c7c9)  
(Vysoký)
</td>
</tr>
<tr>
<th colspan="14" style="border:1px solid black;">
Windows Server 2003
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS11-018**](http://go.microsoft.com/fwlink/?linkid=214126)
</td>
<td style="border:1px solid black;">
[**MS11-019**](http://go.microsoft.com/fwlink/?linkid=212314)
</td>
<td style="border:1px solid black;">
[**MS11-020**](http://go.microsoft.com/fwlink/?linkid=212236)
</td>
<td style="border:1px solid black;">
[**MS11-027**](http://go.microsoft.com/fwlink/?linkid=214005)
</td>
<td style="border:1px solid black;">
[**MS11-028**](http://go.microsoft.com/fwlink/?linkid=207931)
</td>
<td style="border:1px solid black;">
[**MS11-029**](http://go.microsoft.com/fwlink/?linkid=208524)
</td>
<td style="border:1px solid black;">
[**MS11-030**](http://go.microsoft.com/fwlink/?linkid=212595)
</td>
<td style="border:1px solid black;">
[**MS11-031**](http://go.microsoft.com/fwlink/?linkid=212243)
</td>
<td style="border:1px solid black;">
[**MS11-032**](http://go.microsoft.com/fwlink/?linkid=212224)
</td>
<td style="border:1px solid black;">
[**MS11-024**](http://go.microsoft.com/fwlink/?linkid=212226)
</td>
<td style="border:1px solid black;">
[**MS11-026**](http://go.microsoft.com/fwlink/?linkid=212523)
</td>
<td style="border:1px solid black;">
[**MS11-033**](http://go.microsoft.com/fwlink/?linkid=208110)
</td>
<td style="border:1px solid black;">
[**MS11-034**](http://go.microsoft.com/fwlink/?linkid=211826)
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
[**Kritický**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Nízký**](http://go.microsoft.com/fwlink/?linkid=21140)
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
[Aplikace Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=b902c58a-9e2f-4352-8d2f-fffda5344598)  
(Mírný)  
[Aplikace Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=5c464287-3dab-4342-a38d-a12719d3b158)  
(Mírný)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=45feb35b-b24e-4160-adb0-d0b7ae530e90)  
(Mírný)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d46fe0bf-28c2-4696-87bc-dd3c8287fc28)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=64c550d4-c927-4382-91e1-473ed6790819)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=53756404-39e4-43af-81e9-81471536aa66)  
(Mírný)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 Service Pack 2 a Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=ce925e76-cb85-48f6-8c0f-e53fa2b09be6)  
(KB2446704)  
(Kritický)  
[Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=91aa6772-4811-4a58-9bc0-8aa271ed99df)<sup>[1]</sup>
(KB2446708)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=fd284233-e177-4064-9b02-f83dcb727dbe)  
(KB2412687)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=753ed6e3-df2e-4b2d-9e9f-7275cd94d214)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[JScript 5.6 a VBScript 5.6](http://www.microsoft.com/downloads/details.aspx?familyid=e026f2ed-8a20-4268-9b29-04a78bde1999)  
(KB2510587)  
(Kritický)  
[JScript 5.7 a VBScript 5.7](http://www.microsoft.com/downloads/details.aspx?familyid=5b0ed0b2-07f9-43da-bb5d-5be5a45969ee)  
(KB2510581)  
(Kritický)  
[JScript 5.8 a VBScript 5.8](http://www.microsoft.com/downloads/details.aspx?familyid=01aa2beb-9fc1-40f0-a2a4-bcd3d9cb31f8)  
(KB2510531)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5d71d3f5-fd6b-4f3b-8389-37c899748d4b)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=edda8cce-b764-4ef1-afbe-391fbd087362)  
(KB2491683)  
(Vysoký)  
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=bf084b4c-aac9-4cc6-bb30-87fc96ba9430)  
(KB2506212)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=0209a004-f23a-40d9-991f-864046f4605f)  
(Nízký)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=9fbfc742-6c74-49a2-b3cc-e1d5d8c84b77)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=af320f27-bb3a-4e76-a279-4632267c8761)  
(Vysoký)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Aplikace Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=5d8f14d1-85cc-478f-8b50-5c355a331f59)  
(Mírný)  
[Aplikace Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=9d8bbea9-c456-4569-ad96-c2cd0f5fae7e)  
(Mírný)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=979d2ec5-5114-4ec7-aa97-e9289c590cbb)  
(Mírný)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ca0fb4d3-7651-4760-83fa-b71c86cbe459)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ef62db94-4f72-4245-ac9f-6391035e2516)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c8d59f49-45ec-4527-b3a8-4925f710bbfd)  
(Mírný)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 Service Pack 2 a Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=ce925e76-cb85-48f6-8c0f-e53fa2b09be6)  
(KB2446704)  
(Kritický)  
[Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=91aa6772-4811-4a58-9bc0-8aa271ed99df)<sup>[1]</sup>
(KB2446708)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d5adaf4e-4cd7-42ea-8202-31b5c856f5e3)  
(KB2412687)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=a0192dbc-4d0d-4555-9ef7-3e10209a6389)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[JScript 5.6 a VBScript 5.6](http://www.microsoft.com/downloads/details.aspx?familyid=83ce6c99-a57d-4ed1-972b-a6b6798e6675)  
(KB2510587)  
(Kritický)  
[JScript 5.7 a VBScript 5.7](http://www.microsoft.com/downloads/details.aspx?familyid=af791715-77a1-405b-a69e-d63f75dd7ccd)  
(KB2510581)  
(Kritický)  
[JScript 5.8 a VBScript 5.8](http://www.microsoft.com/downloads/details.aspx?familyid=bf0a2966-25c4-4717-bcd6-016ce610d220)  
(KB2510531)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3a498ff0-21d9-493a-b127-6bc20f1baf95)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=f04d939a-da11-4a9f-9e03-b6c3bf3ca58b)  
(KB2491683)  
(Vysoký)  
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=12b01f3a-ccf8-41c1-ac5a-e417a6ddbe95)  
(KB2506212)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=6c287571-54ea-4298-8b7d-b98b2c830cc3)  
(Nízký)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=897b97b0-1bab-4b1b-b417-950fab0d4a65)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=9c95f81c-9812-4070-88d7-34422c638e42)  
(Vysoký)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 SP2 pro systémy s procesorem Itanium
</td>
<td style="border:1px solid black;">
[Aplikace Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=8afe86fc-58b4-4a95-b047-c09138fa4f5e)  
(Mírný)  
[Aplikace Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=f1abfb48-3c8a-4b2d-b739-cc61628b387d)  
(Mírný)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=87eb8b93-9829-45ec-9528-52787732044e)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=79aeb3cd-7c73-467b-b91e-02c6ea01e911)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=9c784734-f44f-4a3c-8223-6289f7dc2ad8)  
(Stupeň závažnosti není určen<sup>[1]</sup>)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 Service Pack 2 a Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=ce925e76-cb85-48f6-8c0f-e53fa2b09be6)  
(KB2446704)  
(Kritický)  
[Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=91aa6772-4811-4a58-9bc0-8aa271ed99df)<sup>[1]</sup>
(KB2446708)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=72a513bb-f901-4992-8562-d1afe1afec8a)  
(KB2412687)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=f5ad6963-2d6a-4d59-9e25-4fc088647fcd)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[JScript 5.6 a VBScript 5.6](http://www.microsoft.com/downloads/details.aspx?familyid=b7d36bae-7ca4-4a40-9efb-13f484fa5518)  
(KB2510587)  
(Kritický)  
[JScript 5.7 a VBScript 5.7](http://www.microsoft.com/downloads/details.aspx?familyid=3f519013-ed14-41a8-aa45-cf8b095d3152)  
(KB2510581)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=c71f4398-2e3b-4b81-a650-8806e618db7f)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=efb575c7-3259-49b1-b59c-89d9544e37a6)  
(KB2491683)  
(Vysoký)  
[Windows Server 2003 SP2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=03a7ee49-7bd6-4215-9779-1b48c10d08b9)  
(KB2506212)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=3fb450a0-d087-4f36-9301-05ffbf94cc1a)  
(Nízký)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=ede38974-4e57-4ea1-8731-b91e96534693)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=f58cf64a-bf31-4496-be75-5775a123338b)  
(Vysoký)
</td>
</tr>
<tr>
<th colspan="14" style="border:1px solid black;">
Windows Vista
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS11-018**](http://go.microsoft.com/fwlink/?linkid=214126)
</td>
<td style="border:1px solid black;">
[**MS11-019**](http://go.microsoft.com/fwlink/?linkid=212314)
</td>
<td style="border:1px solid black;">
[**MS11-020**](http://go.microsoft.com/fwlink/?linkid=212236)
</td>
<td style="border:1px solid black;">
[**MS11-027**](http://go.microsoft.com/fwlink/?linkid=214005)
</td>
<td style="border:1px solid black;">
[**MS11-028**](http://go.microsoft.com/fwlink/?linkid=207931)
</td>
<td style="border:1px solid black;">
[**MS11-029**](http://go.microsoft.com/fwlink/?linkid=208524)
</td>
<td style="border:1px solid black;">
[**MS11-030**](http://go.microsoft.com/fwlink/?linkid=212595)
</td>
<td style="border:1px solid black;">
[**MS11-031**](http://go.microsoft.com/fwlink/?linkid=212243)
</td>
<td style="border:1px solid black;">
[**MS11-032**](http://go.microsoft.com/fwlink/?linkid=212224)
</td>
<td style="border:1px solid black;">
[**MS11-024**](http://go.microsoft.com/fwlink/?linkid=212226)
</td>
<td style="border:1px solid black;">
[**MS11-026**](http://go.microsoft.com/fwlink/?linkid=212523)
</td>
<td style="border:1px solid black;">
[**MS11-033**](http://go.microsoft.com/fwlink/?linkid=208110)
</td>
<td style="border:1px solid black;">
[**MS11-034**](http://go.microsoft.com/fwlink/?linkid=211826)
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
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista Service Pack 1 a Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
[Aplikace Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=00c3c176-feff-4022-ac4c-2d4732ca3d78)  
(Kritický)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=5ea94705-4f76-4b0d-bbbc-afb5e75204bf)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 a Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=da8dd55d-6630-484e-836c-9feeab5cc311)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 a Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d6eddff4-a242-4dec-9d84-72891db2b754)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 a Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=80bf050a-9aff-4cd4-8e2f-196b0a92b1c0)  
(Kritický)
</td>
<td style="border:1px solid black;">
Pouze Windows Vista Service Pack 1:  
[Microsoft .NET Framework 2.0 Service Pack 2 a Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=94b6a1b3-e048-437b-a224-2a64b3735bc3)  
(KB2449741)  
(Kritický)  
Pouze Windows Vista Service Pack 2:  
[Microsoft .NET Framework 2.0 Service Pack 2 a Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=1407aaec-b3e0-404c-b84f-0c8e808614c4)  
(KB2449742)  
(Kritický)  
Windows Vista Service Pack 1 a Windows Vista Service Pack 2:  
[Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=91aa6772-4811-4a58-9bc0-8aa271ed99df)<sup>[1]</sup>
(KB2446708)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 a Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4ff2e440-79c2-4045-b225-913d1740fdb9)  
(KB2412687)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 a Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2a17e44f-54aa-423d-b3c7-a4f404f7c28b)  
(Kritický)
</td>
<td style="border:1px solid black;">
[JScript 5.7 a VBScript 5.7](http://www.microsoft.com/downloads/details.aspx?familyid=719e2c86-30e5-4cd5-94f4-d6de54efee5f)  
(KB2510581)  
(Kritický)  
[JScript 5.8 a VBScript 5.8](http://www.microsoft.com/downloads/details.aspx?familyid=21decb84-75ef-4bde-a802-1e661a505e94)<sup>[1]</sup>
(KB2510531)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 a Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e7c4fc81-d1ef-4378-862b-e955d75fb2de)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 a Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=11a8f240-51b3-4e31-a24a-a235179f3396)  
(KB2491683)  
(Vysoký)  
[Windows Vista Service Pack 1 a Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e6cba040-9d7c-4777-a2f7-e4dd11dfb845)  
(KB2506212)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 a Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c8fce0fb-4c90-479b-8ce9-75e60d52d256)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 a Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b4743167-9614-445a-9e91-10efdac505a8)  
(Vysoký)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 1 a Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Aplikace Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=79f52733-44e4-47b6-86ca-1395a095b4e7)  
(Kritický)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=bc63b233-9db0-4fb1-a61c-fa7e9e44ba10)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 a Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=040f8b46-f458-4a72-a1b0-ad8a65a1194c)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 a Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2878c587-6544-40b4-9288-fc3b3ce1128d)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 a Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=a81412d0-2516-4bf4-87f7-3e41ebf6b82b)  
(Kritický)
</td>
<td style="border:1px solid black;">
Pouze Windows Vista x64 Edition Service Pack 1:  
[Microsoft .NET Framework 2.0 Service Pack 2 a Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=94b6a1b3-e048-437b-a224-2a64b3735bc3)  
(KB2449741)  
(Kritický)  
Pouze Windows Vista x64 Edition Service Pack 2:  
[Microsoft .NET Framework 2.0 Service Pack 2 a Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=1407aaec-b3e0-404c-b84f-0c8e808614c4)  
(KB2449742)  
(Kritický)  
Windows Vista x64 Edition Service Pack 1 a Windows Vista x64 Edition Service Pack 2:  
[Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=91aa6772-4811-4a58-9bc0-8aa271ed99df)<sup>[1]</sup>
(KB2446708)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 a Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4d826026-e62a-4cec-8682-49fbe7f65cd6)  
(KB2412687)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 a Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e708d24f-e348-4c4d-99ed-e78dd1689d01)  
(Kritický)
</td>
<td style="border:1px solid black;">
[JScript 5.7 a VBScript 5.7](http://www.microsoft.com/downloads/details.aspx?familyid=89b9d01e-bcbc-4f2c-973b-51051494f406)  
(KB2510581)  
(Kritický)  
[JScript 5.8 a VBScript 5.8](http://www.microsoft.com/downloads/details.aspx?familyid=d4ac199e-7bf8-4661-a4e5-c53719b2673a)<sup>[1]</sup>
(KB2510531)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 a Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8d654a78-0e4f-452c-8874-fbf478813857)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 a Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=61db662e-88d7-4454-b4b7-e987728fb137)  
(KB2491683)  
(Vysoký)  
[Windows Vista x64 Edition Service Pack 1 a Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=1c942282-0f80-46c1-aeef-1ef948e105a3)  
(KB2506212)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 a Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7da10b64-d0a9-4e42-aa3a-87c657122a8c)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 a Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7e410d5c-b9f7-4a63-8300-36b2d57c6128)  
(Vysoký)
</td>
</tr>
<tr>
<th colspan="14" style="border:1px solid black;">
Windows Server 2008
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS11-018**](http://go.microsoft.com/fwlink/?linkid=214126)
</td>
<td style="border:1px solid black;">
[**MS11-019**](http://go.microsoft.com/fwlink/?linkid=212314)
</td>
<td style="border:1px solid black;">
[**MS11-020**](http://go.microsoft.com/fwlink/?linkid=212236)
</td>
<td style="border:1px solid black;">
[**MS11-027**](http://go.microsoft.com/fwlink/?linkid=214005)
</td>
<td style="border:1px solid black;">
[**MS11-028**](http://go.microsoft.com/fwlink/?linkid=207931)
</td>
<td style="border:1px solid black;">
[**MS11-029**](http://go.microsoft.com/fwlink/?linkid=208524)
</td>
<td style="border:1px solid black;">
[**MS11-030**](http://go.microsoft.com/fwlink/?linkid=212595)
</td>
<td style="border:1px solid black;">
[**MS11-031**](http://go.microsoft.com/fwlink/?linkid=212243)
</td>
<td style="border:1px solid black;">
[**MS11-032**](http://go.microsoft.com/fwlink/?linkid=212224)
</td>
<td style="border:1px solid black;">
[**MS11-024**](http://go.microsoft.com/fwlink/?linkid=212226)
</td>
<td style="border:1px solid black;">
[**MS11-026**](http://go.microsoft.com/fwlink/?linkid=212523)
</td>
<td style="border:1px solid black;">
[**MS11-033**](http://go.microsoft.com/fwlink/?linkid=208110)
</td>
<td style="border:1px solid black;">
[**MS11-034**](http://go.microsoft.com/fwlink/?linkid=211826)
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
[**Mírný**](http://go.microsoft.com/fwlink/?linkid=21140)
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
[**Kritický**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Nízký**](http://go.microsoft.com/fwlink/?linkid=21140)
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
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=7d8603b8-bb52-4cf6-be8b-bb3475d30fc5)\*\*  
(Mírný)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=d5d76e90-1cef-47e8-9d8d-2c5a43f42ba3)\*\*  
(Mírný)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro 32bitové systémy a Windows Server 2008 pro 32bitové systémy Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=f8c9390a-5ca1-492a-9e35-a516de48deb5)\*  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro 32bitové systémy a Windows Server 2008 pro 32bitové systémy Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=31c48ba9-7774-4633-862d-5c27c3703584)\*  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro 32bitové systémy a Windows Server 2008 pro 32bitové systémy Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c3247886-76d0-4292-be9d-3e9b0221c46a)\*\*  
(Mírný)
</td>
<td style="border:1px solid black;">
Pouze Windows Server 2008 pro 32bitové systémy:  
[Microsoft .NET Framework 2.0 Service Pack 2 a Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=94b6a1b3-e048-437b-a224-2a64b3735bc3)\*\*  
(KB2449741)  
(Kritický)  
Pouze Windows Server 2008 pro 32bitové systémy s aktualizací Service Pack 2:  
[Microsoft .NET Framework 2.0 Service Pack 2 a Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=1407aaec-b3e0-404c-b84f-0c8e808614c4)\*\*  
(KB2449742)  
(Kritický)  
Windows Server 2008 pro 32bitové systémy a Windows Server 2008 pro 32bitové systémy Service Pack 2:  
[Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=91aa6772-4811-4a58-9bc0-8aa271ed99df)\*\*<sup>[1]</sup>
(KB2446708)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro 32bitové systémy a Windows Server 2008 pro 32bitové systémy Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=fbada866-7d36-4b85-acde-fd856a998737)\*\*\*  
(KB2412687)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro 32bitové systémy a Windows Server 2008 pro 32bitové systémy Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=9894be38-a582-4c15-ad0e-cc3afab2aebc)\*  
(Kritický)
</td>
<td style="border:1px solid black;">
[JScript 5.7 a VBScript 5.7](http://www.microsoft.com/downloads/details.aspx?familyid=d8b33ffd-eff1-4a10-b6fc-3c8f01e0fec5)\*\*  
(KB2510581)  
(Kritický)  
[JScript 5.8 a VBScript 5.8](http://www.microsoft.com/downloads/details.aspx?familyid=afd128ff-717f-4d98-b214-f2c28d59623d)\*\*<sup>[1]</sup>
(KB2510531)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro 32bitové systémy a Windows Server 2008 pro 32bitové systémy Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=9105377e-83c7-4010-8fd6-26e42e98c2cc)\*  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro 32bitové systémy a Windows Server 2008 pro 32bitové systémy Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=90f56368-776b-4d45-ad68-91afbd316d25)\*\*  
(KB2491683)  
(Vysoký)  
[Windows Server 2008 pro 32bitové systémy a Windows Server 2008 pro 32bitové systémy Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=fa972742-1166-4a9e-ab64-6a4f968f9c6d)\*  
(KB2506212)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro 32bitové systémy a Windows Server 2008 pro 32bitové systémy Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=036f1285-7484-4e3b-8799-2c6c08166596)\*\*  
(Nízký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro 32bitové systémy a Windows Server 2008 pro 32bitové systémy Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c6ac26b8-8cc8-40fe-baab-22bf13df1aa8)\*  
(Vysoký)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 pro systémy s procesorem x64 a Windows Server 2008 pro systémy s procesorem x64 Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=c6d58f64-bdd5-4fe6-96f4-9641b8e7b570)\*\*  
(Mírný)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=51203a31-368b-4b47-96a5-9e9e5a55cd76)\*\*  
(Mírný)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem x64 a Windows Server 2008 pro systémy s procesorem x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b0cfd5e0-6de5-4863-b5e4-b223a0e36d72)\*  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem x64 a Windows Server 2008 pro systémy s procesorem x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=de843115-cf98-4511-aa93-f620e4572555)\*  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem x64 a Windows Server 2008 pro systémy s procesorem x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=51521b6b-94a7-4bcf-ad5f-fc304728b10f)\*\*  
(Mírný)
</td>
<td style="border:1px solid black;">
Pouze Windows Server 2008 pro systémy s procesorem x64:  
[Microsoft .NET Framework 2.0 Service Pack 2 a Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=94b6a1b3-e048-437b-a224-2a64b3735bc3)\*\*  
(KB2449741)  
(Kritický)  
Pouze Windows Server 2008 pro systémy s procesorem x64 s aktualizací Service Pack 2:  
[Microsoft .NET Framework 2.0 Service Pack 2 a Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=1407aaec-b3e0-404c-b84f-0c8e808614c4)\*\*  
(KB2449742)  
(Kritický)  
Windows Server 2008 pro systémy s procesorem x64 a Windows Server 2008 pro systémy s procesorem x64 Service Pack 2:  
[Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=91aa6772-4811-4a58-9bc0-8aa271ed99df)\*\*<sup>[1]</sup>
(KB2446708)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem x64 a Windows Server 2008 pro systémy s procesorem x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8f4ddfcb-374d-4cad-8c61-2b988b46f628)\*\*\*  
(KB2412687)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem x64 a Windows Server 2008 pro systémy s procesorem x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2d7d2021-020f-4cc9-a027-258d7e5faec9)\*  
(Kritický)
</td>
<td style="border:1px solid black;">
[JScript 5.7 a VBScript 5.7](http://www.microsoft.com/downloads/details.aspx?familyid=6c2e6b87-afcd-461a-8a43-9a2fb277b18a)\*\*  
(KB2510581)  
(Kritický)  
[JScript 5.8 a VBScript 5.8](http://www.microsoft.com/downloads/details.aspx?familyid=40e8beca-0b5a-43b0-98f8-b32a82ad65d6)\*\*<sup>[1]</sup>
(KB2510531)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem x64 a Windows Server 2008 pro systémy s procesorem x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=060e8b20-edca-4427-9d60-eb57261eb668)\*  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem x64 a Windows Server 2008 pro systémy s procesorem x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=22a001fc-5c2e-4539-85c9-0c2054a1777d)\*\*  
(KB2491683)  
(Vysoký)  
[Windows Server 2008 pro systémy s procesorem x64 a Windows Server 2008 pro systémy s procesorem x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=fc250c8a-ebaf-4264-9393-dc23cc372d9f)\*  
(KB2506212)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem x64 a Windows Server 2008 pro systémy s procesorem x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=1438cec8-8dab-4510-ad75-dc6959dac0d8)\*\*  
(Nízký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem x64 a Windows Server 2008 pro systémy s procesorem x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ac49f5d3-5e2f-4916-99be-a3254278da7e)\*  
(Vysoký)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 pro systémy s procesorem Itanium a Windows Server 2008 pro systémy s procesorem Itanium Service Pack 2
</td>
<td style="border:1px solid black;">
[Aplikace Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=f6f6f22c-fc7f-4e96-b6b5-be3c1acecf6e)  
(Mírný)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem Itanium a Windows Server 2008 pro systémy s procesorem Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8eaf51cd-2f6e-4bbc-bc4f-9deed03649ac)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem Itanium a Windows Server 2008 pro systémy s procesorem Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b89b8e28-cd98-4bcc-8729-5e51d52d1e92)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem Itanium a Windows Server 2008 pro systémy s procesorem Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e7c38b0d-7240-420a-88d3-2749a40e386f)  
(Stupeň závažnosti není určen<sup>[1]</sup>)
</td>
<td style="border:1px solid black;">
Pouze Windows Server 2008 pro systémy s procesorem Itanium:  
[Microsoft .NET Framework 2.0 Service Pack 2 a Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=94b6a1b3-e048-437b-a224-2a64b3735bc3)  
(KB2449741)  
(Kritický)  
Pouze Windows Server 2008 pro systémy s procesorem Itanium s aktualizací Service Pack 2:  
[Microsoft .NET Framework 2.0 Service Pack 2 a Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=1407aaec-b3e0-404c-b84f-0c8e808614c4)  
(KB2449742)  
(Kritický)  
Windows Server 2008 pro systémy s procesorem Itanium a Windows Server 2008 pro systémy s procesorem Itanium Service Pack 2:  
[Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=91aa6772-4811-4a58-9bc0-8aa271ed99df)<sup>[1]</sup>
(KB2446708)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem Itanium a Windows Server 2008 pro systémy s procesorem Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2fd71543-0e18-4907-89b9-355d24d7db69)  
(KB2412687)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem Itanium a Windows Server 2008 pro systémy s procesorem Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c0275df0-10ac-4500-ab86-b7e9a34f8e1d)  
(Kritický)
</td>
<td style="border:1px solid black;">
[JScript 5.7 a VBScript 5.7](http://www.microsoft.com/downloads/details.aspx?familyid=afb49d24-1913-4e5f-a3ea-c6c9642e2017)  
(KB2510581)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem Itanium a Windows Server 2008 pro systémy s procesorem Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2b8571cb-2dae-4bff-9f13-feb89840044c)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem Itanium a Windows Server 2008 pro systémy s procesorem Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=421024f1-aa86-459e-b6de-53851a3fcba2)  
(KB2506212)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem Itanium a Windows Server 2008 pro systémy s procesorem Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=f35ecdd1-6b5c-40e7-a00b-ca083bdf5cba)  
(Nízký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem Itanium a Windows Server 2008 pro systémy s procesorem Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3b93de4f-01f4-4efd-afc1-31d87b92fad2)  
(Vysoký)
</td>
</tr>
<tr>
<th colspan="14" style="border:1px solid black;">
Windows 7
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS11-018**](http://go.microsoft.com/fwlink/?linkid=214126)
</td>
<td style="border:1px solid black;">
[**MS11-019**](http://go.microsoft.com/fwlink/?linkid=212314)
</td>
<td style="border:1px solid black;">
[**MS11-020**](http://go.microsoft.com/fwlink/?linkid=212236)
</td>
<td style="border:1px solid black;">
[**MS11-027**](http://go.microsoft.com/fwlink/?linkid=214005)
</td>
<td style="border:1px solid black;">
[**MS11-028**](http://go.microsoft.com/fwlink/?linkid=207931)
</td>
<td style="border:1px solid black;">
[**MS11-029**](http://go.microsoft.com/fwlink/?linkid=208524)
</td>
<td style="border:1px solid black;">
[**MS11-030**](http://go.microsoft.com/fwlink/?linkid=212595)
</td>
<td style="border:1px solid black;">
[**MS11-031**](http://go.microsoft.com/fwlink/?linkid=212243)
</td>
<td style="border:1px solid black;">
[**MS11-032**](http://go.microsoft.com/fwlink/?linkid=212224)
</td>
<td style="border:1px solid black;">
[**MS11-024**](http://go.microsoft.com/fwlink/?linkid=212226)
</td>
<td style="border:1px solid black;">
[**MS11-026**](http://go.microsoft.com/fwlink/?linkid=212523)
</td>
<td style="border:1px solid black;">
[**MS11-033**](http://go.microsoft.com/fwlink/?linkid=208110)
</td>
<td style="border:1px solid black;">
[**MS11-034**](http://go.microsoft.com/fwlink/?linkid=211826)
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
[**Kritický**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Žádný
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
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=59676b71-8b9d-4230-a9e0-b20db3e3ec7e)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows 7 pro 32bitové systémy a Windows 7 pro 32bitové systémy Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=0dcba089-19f7-46ca-9e52-24eaebad4715)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows 7 pro 32bitové systémy a Windows 7 pro 32bitové systémy Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=d3ef905b-3584-4842-9ec2-cf3856305d49)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows 7 pro 32bitové systémy a Windows 7 pro 32bitové systémy Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=46510959-e4a2-4c21-b33c-fd3d97b3ac3d)  
(Kritický)
</td>
<td style="border:1px solid black;">
Pouze Windows 7 pro 32bitové systémy:  
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=157aa425-953c-4fc9-ab76-4e65d4be8baa)  
(KB2446709)  
(Kritický)  
Pouze Windows 7 pro 32bitové systémy Service Pack 1:  
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=8f87b8aa-1a2a-405e-aee0-9247d553756a)  
(KB2446710)  
(Kritický)  
Windows 7 pro 32bitové systémy a Windows 7 pro 32bitové systémy Service Pack 1:  
[Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=91aa6772-4811-4a58-9bc0-8aa271ed99df)<sup>[1]</sup>
(KB2446708)  
(Kritický)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows 7 pro 32bitové systémy a Windows 7 pro 32bitové systémy Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=8fdae09b-d1bb-4ef5-aa45-2a05f2a5e12d)  
(Kritický)
</td>
<td style="border:1px solid black;">
[JScript 5.8 a VBScript 5.8](http://www.microsoft.com/downloads/details.aspx?familyid=17ebf291-fdae-4e78-9377-871b3103ce16)<sup>[1]</sup>
(KB2510531)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows 7 pro 32bitové systémy a Windows 7 pro 32bitové systémy Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=751c45ea-0943-4948-807f-8716c6ff9198)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows 7 pro 32bitové systémy a Windows 7 pro 32bitové systémy Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=bf762b86-b949-4e84-8ca4-93ebe669c1b8)  
(KB2491683)  
(Vysoký)  
[Windows 7 pro 32bitové systémy a Windows 7 pro 32bitové systémy Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=0f5a122e-dd5e-4b08-881a-f13b38642720)  
(KB2506212)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows 7 pro 32bitové systémy a Windows 7 pro 32bitové systémy Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=aed201c1-f1fb-4df9-8875-6f57ea0eb15b)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows 7 pro 32bitové systémy a Windows 7 pro 32bitové systémy Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=6e7ff003-ff3f-49bb-8e45-d869885dd8d7)  
(Vysoký)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 7 pro systémy s procesorem x64 a Windows 7 pro systémy s procesorem x64 Service Pack 1
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=3a998678-2678-489e-8711-39322663147d)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows 7 pro systémy s procesorem x64 a Windows 7 pro systémy s procesorem x64 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=b7fd356a-56d0-4638-8901-40acfa600f25)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows 7 pro systémy s procesorem x64 a Windows 7 pro systémy s procesorem x64 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=7ddc943b-6868-4e8f-a869-89b47133c287)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows 7 pro systémy s procesorem x64 a Windows 7 pro systémy s procesorem x64 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=432555cf-aed8-4329-a74f-526441521082)  
(Kritický)
</td>
<td style="border:1px solid black;">
Pouze Windows 7 pro systémy s procesorem x64:  
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=157aa425-953c-4fc9-ab76-4e65d4be8baa)  
(KB2446709)  
(Kritický)  
Pouze Windows 7 pro systémy s procesorem x64 Service Pack 1:  
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=8f87b8aa-1a2a-405e-aee0-9247d553756a)  
(KB2446710)  
(Kritický)  
Windows 7 pro systémy s procesorem x64 a Windows 7 pro systémy s procesorem x64 Service Pack 1:  
[Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=91aa6772-4811-4a58-9bc0-8aa271ed99df)<sup>[1]</sup>
(KB2446708)  
(Kritický)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows 7 pro systémy s procesorem x64 a Windows 7 pro systémy s procesorem x64 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=40879dfb-efa4-41ba-8d5c-22e926a55eef)  
(Kritický)
</td>
<td style="border:1px solid black;">
[JScript 5.8 a VBScript 5.8](http://www.microsoft.com/downloads/details.aspx?familyid=c95ad86d-da58-4d7a-9ffd-8441f92baaa5)<sup>[1]</sup>
(KB2510531)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows 7 pro systémy s procesorem x64 a Windows 7 pro systémy s procesorem x64 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=976c882a-bc07-4128-927f-82a2df46cf45)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows 7 pro systémy s procesorem x64 a Windows 7 pro systémy s procesorem x64 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=a6793ecf-a3f6-4989-8e4c-c5c0005f9ac4)  
(KB2491683)  
(Vysoký)  
[Windows 7 pro systémy s procesorem x64 a Windows 7 pro systémy s procesorem x64 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=658301f1-103a-48a2-9b67-61cf8e1dad50)  
(KB2506212)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows 7 pro systémy s procesorem x64 a Windows 7 pro systémy s procesorem x64 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=1a32bf04-7eed-4d27-a8e4-054b4a5b76cb)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows 7 pro systémy s procesorem x64 a Windows 7 pro systémy s procesorem x64 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=0c0aef7e-501c-4ca3-ae7f-497a8c169121)  
(Vysoký)
</td>
</tr>
<tr>
<th colspan="14" style="border:1px solid black;">
Windows Server 2008 R2
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS11-018**](http://go.microsoft.com/fwlink/?linkid=214126)
</td>
<td style="border:1px solid black;">
[**MS11-019**](http://go.microsoft.com/fwlink/?linkid=212314)
</td>
<td style="border:1px solid black;">
[**MS11-020**](http://go.microsoft.com/fwlink/?linkid=212236)
</td>
<td style="border:1px solid black;">
[**MS11-027**](http://go.microsoft.com/fwlink/?linkid=214005)
</td>
<td style="border:1px solid black;">
[**MS11-028**](http://go.microsoft.com/fwlink/?linkid=207931)
</td>
<td style="border:1px solid black;">
[**MS11-029**](http://go.microsoft.com/fwlink/?linkid=208524)
</td>
<td style="border:1px solid black;">
[**MS11-030**](http://go.microsoft.com/fwlink/?linkid=212595)
</td>
<td style="border:1px solid black;">
[**MS11-031**](http://go.microsoft.com/fwlink/?linkid=212243)
</td>
<td style="border:1px solid black;">
[**MS11-032**](http://go.microsoft.com/fwlink/?linkid=212224)
</td>
<td style="border:1px solid black;">
[**MS11-024**](http://go.microsoft.com/fwlink/?linkid=212226)
</td>
<td style="border:1px solid black;">
[**MS11-026**](http://go.microsoft.com/fwlink/?linkid=212523)
</td>
<td style="border:1px solid black;">
[**MS11-033**](http://go.microsoft.com/fwlink/?linkid=208110)
</td>
<td style="border:1px solid black;">
[**MS11-034**](http://go.microsoft.com/fwlink/?linkid=211826)
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
<td style="border:1px solid black;">
[**Mírný**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritický**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Žádný
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
[**Nízký**](http://go.microsoft.com/fwlink/?linkid=21140)
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
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=c7b2482b-44bf-4c01-99d8-f93868659a24)\*\*  
(Mírný)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem x64 a Windows Server 2008 R2 pro systémy s procesorem x64 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=27a3847b-695b-4f60-aea5-86b0dbe68945)\*  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem x64 a Windows Server 2008 R2 pro systémy s procesorem x64 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=c4352802-9c5a-4c07-8303-3a4b78d3f954)\*  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem x64 a Windows Server 2008 R2 pro systémy s procesorem x64 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=e4fa8ed0-acb0-4864-be18-29a27f8501de)\*\*  
(Mírný)
</td>
<td style="border:1px solid black;">
Pouze Windows Server 2008 R2 pro systémy s procesorem x64:  
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=157aa425-953c-4fc9-ab76-4e65d4be8baa)\*  
(KB2446709)  
(Kritický)  
Pouze Windows Server 2008 R2 pro systémy s procesorem x64:  
[Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=91aa6772-4811-4a58-9bc0-8aa271ed99df)<sup>[1]</sup>
(KB2446708)  
(Kritický)  
Pouze Windows Server 2008 R2 pro systémy s procesorem x64 Service Pack 1:  
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=8f87b8aa-1a2a-405e-aee0-9247d553756a)\*  
(KB2446710)  
(Kritický)  
Pouze Windows Server 2008 R2 pro systémy s procesorem x64 Service Pack 1:  
[Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=91aa6772-4811-4a58-9bc0-8aa271ed99df)\*<sup>[1]</sup>
(KB2446708)  
(Kritický)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem x64 a Windows Server 2008 R2 pro systémy s procesorem x64 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=2084c726-187e-41f9-9bea-da18f490d29e)\*  
(Kritický)
</td>
<td style="border:1px solid black;">
[JScript 5.8 a VBScript 5.8](http://www.microsoft.com/downloads/details.aspx?familyid=aecc2c7a-285c-409d-be23-c5b4b5449496)\*\*<sup>[1]</sup>
(KB2510531)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem x64 a Windows Server 2008 R2 pro systémy s procesorem x64 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=6f2a52cc-4833-448d-becc-2eac1a447410)\*  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem x64 a Windows Server 2008 R2 pro systémy s procesorem x64 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=465c0478-6a74-4b00-8608-938cc492549f)\*\*  
(KB2491683)  
(Vysoký)  
[Windows Server 2008 R2 pro systémy s procesorem x64 a Windows Server 2008 R2 pro systémy s procesorem x64 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=4c5c3a0f-0672-49d0-bcbd-c7f40e11d092)\*  
(KB2506212)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem x64 a Windows Server 2008 R2 pro systémy s procesorem x64 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=665faa7e-2368-4421-9dd5-ea6df2c79498)\*\*  
(Nízký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem x64 a Windows Server 2008 R2 pro systémy s procesorem x64 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=2fc66224-45c6-4e8f-ad00-6a1ec30b4505)\*  
(Vysoký)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 pro systémy s procesorem Itanium a Windows Server 2008 R2 pro systémy s procesorem Itanium Service Pack 1
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=af6db318-fbec-4286-a3a7-4081620146e5)  
(Mírný)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem Itanium a Windows Server 2008 R2 pro systémy s procesorem Itanium Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=1e7d3f21-bdbd-4826-855d-85422aa5f836)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem Itanium a Windows Server 2008 R2 pro systémy s procesorem Itanium Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=0005377b-443f-44ca-a890-620b2dcea6f1)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem Itanium a Windows Server 2008 R2 pro systémy s procesorem Itanium Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=d7bcf4d7-b697-4c5f-adbc-a2b3700e0ad5)  
(Mírný)
</td>
<td style="border:1px solid black;">
Pouze Windows Server 2008 R2 pro systémy s procesorem Itanium:  
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=157aa425-953c-4fc9-ab76-4e65d4be8baa)  
(KB2446709)  
(Kritický)  
Pouze Windows Server 2008 R2 pro systémy s procesorem Itanium Service Pack 1:  
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=8f87b8aa-1a2a-405e-aee0-9247d553756a)  
(KB2446710)  
(Kritický)  
Windows Server 2008 R2 pro systémy s procesorem Itanium a Windows Server 2008 R2 pro systémy s procesorem Itanium Service Pack 1:  
[Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=91aa6772-4811-4a58-9bc0-8aa271ed99df)<sup>[1]</sup>
(KB2446708)  
(Kritický)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem Itanium a Windows Server 2008 R2 pro systémy s procesorem Itanium Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=34d2793e-a2cd-49f6-b524-6598ea86175f)  
(Kritický)
</td>
<td style="border:1px solid black;">
[JScript 5.8 a VBScript 5.8](http://www.microsoft.com/downloads/details.aspx?familyid=e1bc0ed8-5a93-4d01-b407-919dfd894b5f)<sup>[1]</sup>
(KB2510531)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem Itanium a Windows Server 2008 R2 pro systémy s procesorem Itanium Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=c6ca0b7c-8151-4d54-aa9b-5ec2b75d8ab6)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem Itanium a Windows Server 2008 R2 pro systémy s procesorem Itanium Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=1a993f8c-d28a-4a95-a3c6-059f06e75461)  
(KB2506212)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem Itanium a Windows Server 2008 R2 pro systémy s procesorem Itanium Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=140ea384-2877-401f-ac3b-f84f6966e970)  
(Nízký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem Itanium a Windows Server 2008 R2 pro systémy s procesorem Itanium Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=485ccf96-27a0-499e-9f52-2836b73d26d2)  
(Vysoký)
</td>
</tr>
</table>
<p></p>

 
**Poznámky k systémům Windows Server 2008 a Windows Server 2008 R2**

**\*Instalace Server Core obsahující chybu zabezpečení.** Tato aktualizace se stejným hodnocením závažnosti se vztahuje k podporovaným edicím systému Windows Server 2008 nebo Windows Server 2008 R2, jak je uvedeno, s instalací pomocí volby pro instalaci Server Core nebo bez ní. Další informace o této možnosti instalace naleznete v článcích na webu TechNet [Managing a Server Core Installation](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) (Správa instalace Server Core) a [Servicing a Server Core Installation](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx) (Obsluha instalace Server Core). Možnost instalace Server Core se nevztahuje na určité edice systému Windows Server 2008 a Windows Server 2008 R2; další informace naleznete v části [Porovnání možností instalace Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**\*\*Instalace Server Core není touto chybou ovlivněna.** Chyby zabezpečení, které tato aktualizace řeší, nemají vliv na podporované edice systému Windows Server 2008 nebo Windows Server 2008 R2, jak je uvedeno, v případě instalace s využitím možnosti instalace Server Core. Další informace o této možnosti instalace naleznete v článcích na webu TechNet [Managing a Server Core Installation](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) (Správa instalace Server Core) a [Servicing a Server Core Installation](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx) (Obsluha instalace Server Core). Možnost instalace Server Core se nevztahuje na určité edice systému Windows Server 2008 a Windows Server 2008 R2; další informace naleznete v části [Porovnání možností instalace Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**\*\*\*Instalace Server Core není touto chybou ovlivněna.** Chyby zabezpečení, které tato aktualizace řeší, nijak neovlivňují podporované edice systémů Windows Server 2008 a Windows Server 2008 R2 v případě instalace s využitím možnosti instalace Server Core, i když se soubory postižené touto chybou zabezpečení mohou v systému vyskytovat. I přesto bude uživatelům se soubory postiženými těmito chybami tato aktualizace stále nabízena, neboť soubory aktualizace jsou novější (s vyššími čísly verze) než soubory, které jsou aktuálně ve vašem systému. Další informace o této možnosti instalace naleznete v článcích na webu TechNet [Managing a Server Core Installation](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) (Správa instalace Server Core) a [Servicing a Server Core Installation](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx) (Obsluha instalace Server Core). Možnost instalace Server Core se nevztahuje na určité edice systému Windows Server 2008 a Windows Server 2008 R2; další informace naleznete v části [Porovnání možností instalace Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**Poznámka k bulletinu MS11-027**

<sup>[1]</sup>Tento konkrétní operační systém není chybami zabezpečení popsanými v tomto bulletinu ohrožen. Dostupná aktualizace nastavuje dezaktivační bity pro ovladače jiných výrobců.

**Poznámka k bulletinu MS11-028**

<sup>[1]</sup>**Postiženo je rozhraní .NET Framework 4.0 a .NET Framework 4.0 Client Profile.** Distribuční balíčky rozhraní .NET Framework verze 4 jsou k dispozici ve dvou profilech: .NET Framework 4.0 a .NET Framework 4.0 Client Profile. Rozhraní .NET Framework 4.0 Client Profile je verzí rozhraní .NET Framework 4.0. Chyba zabezpečení řešená v této aktualizaci se týká obou rozhraní .NET Framework 4.0 a .NET Framework 4.0 Client Profile. Další informace naleznete zde: [Instalace rozhraní .NET Framework](http://msdn.microsoft.com/en-us/library/5a4x27ek.aspx).

**Poznámka k bulletinu MS11-029**

Více aktualizovaných souborů v rámci stejného identifikátoru bulletinu naleznete také v dalších kategoriích softwaru v rámci této části **Software obsahující tuto chybu a umístění aktualizací ke stažení**. Tento bulletin se vztahuje na více kategorií softwaru.

**Poznámka k bulletinu MS11-031**

<sup>[1]</sup>Systémy s nainstalovanou aplikací Internet Explorer 9 nejsou ohroženy a nevyžadují tuto aktualizaci. Systémy, u nichž nebyl proveden upgrade na aplikaci Internet Explorer 9, budou vyžadovat správnou aktualizaci verzí nainstalovaných skriptovacích strojů JScript a VBScript. Pokyny k určení verzí skriptovacích strojů JScript a VBScript nainstalovaných v systému naleznete v bulletinu.

**Poznámka k bulletinu MS11-024**

Pokud jsou pro jeden operační systém k dispozici dvě aktualizace, nainstalujte obě.

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
<th style="border:1px solid black;" >
</th>
</tr>
<tr>
<th colspan="5" style="border:1px solid black;">
Sady Microsoft Office a jejich komponenty
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS11-029**](http://go.microsoft.com/fwlink/?linkid=208524)
</td>
<td style="border:1px solid black;">
[**MS11-021**](http://go.microsoft.com/fwlink/?linkid=210121)
</td>
<td style="border:1px solid black;">
[**MS11-022**](http://go.microsoft.com/fwlink/?linkid=210727)
</td>
<td style="border:1px solid black;">
[**MS11-023**](http://go.microsoft.com/fwlink/?linkid=210206)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Celkový stupeň** **závažnosti**
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
Microsoft Office XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Office XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=6c87c2a9-3705-4680-8a9b-63b6ec83674d)  
(KB2509461)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Microsoft Excel 2002 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=db2c5cfe-588c-4646-b86a-3fb8248f7af4)  
(KB2466169)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Microsoft PowerPoint 2002 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=0d215ab6-c9be-4f43-9501-658bb7ef008e)  
(KB2464617)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Microsoft Office XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=6c87c2a9-3705-4680-8a9b-63b6ec83674d)  
(KB2509461)  
(Vysoký)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2003 Service Pack 3
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Microsoft Excel 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=916a076d-d754-4092-b23d-c8826db7e397)  
(KB2502786)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Microsoft PowerPoint 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=2ce8349f-79b1-41ef-a1c0-cbe40ccf9f20)  
(KB2464588)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=8b68cf68-1606-4649-b860-a64702c6cf33)  
(KB2509503)  
(Vysoký)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2007 Service Pack 2
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Microsoft Excel 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5ae34fe0-03bd-48a9-a7ac-de8f7b1aff90)<sup>[1]</sup>
(KB2464583)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Microsoft PowerPoint 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=6b2526fe-a061-4a17-992e-ac867bef130e)  
(KB2464594)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=dbba0cd4-ab72-4e2b-9524-fd6be27f0b02)  
(KB2509488)  
(Vysoký)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2010 (32bitové edice)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Microsoft Excel 2010 (32bitové edice)](http://www.microsoft.com/downloads/details.aspx?familyid=a427f0e2-b74d-4ef3-bec4-0a101d09bfa3)  
(KB2466146)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Microsoft PowerPoint 2010 (32bitové edice)](http://www.microsoft.com/downloads/details.aspx?familyid=549ca7f0-44bf-4965-a9d2-aa5e8dac2238)  
(KB2519975)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2010 (64bitové edice)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Microsoft Excel 2010 (64bitové edice)](http://www.microsoft.com/downloads/details.aspx?familyid=13dca35d-2209-4c5c-9150-d6db2bb3b496)  
(KB2466146)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Microsoft PowerPoint 2010 (64bitové edice)](http://www.microsoft.com/downloads/details.aspx?familyid=ef62deae-2b07-41c9-a4bf-b746566e59ee)  
(KB2519975)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
</tr>
<tr>
<th colspan="5" style="border:1px solid black;">
Microsoft Office for Mac
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS11-029**](http://go.microsoft.com/fwlink/?linkid=208524)
</td>
<td style="border:1px solid black;">
[**MS11-021**](http://go.microsoft.com/fwlink/?linkid=210121)
</td>
<td style="border:1px solid black;">
[**MS11-022**](http://go.microsoft.com/fwlink/?linkid=210727)
</td>
<td style="border:1px solid black;">
[**MS11-023**](http://go.microsoft.com/fwlink/?linkid=210206)
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
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2004 for Mac
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Microsoft Office 2004 for Mac](http://www.microsoft.com/downloads/details.aspx?familyid=f756d836-6ab2-4adb-9dee-6cb523d7c1f5)  
(KB2505924)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2004 for Mac](http://www.microsoft.com/downloads/details.aspx?familyid=f756d836-6ab2-4adb-9dee-6cb523d7c1f5)  
(KB2505924)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2004 for Mac](http://www.microsoft.com/downloads/details.aspx?familyid=f756d836-6ab2-4adb-9dee-6cb523d7c1f5)  
(KB2505924)  
(Vysoký)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2008 for Mac
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Microsoft Office 2008 for Mac](http://www.microsoft.com/downloads/details.aspx?familyid=84dfe3f4-a2a1-47b9-8da1-29ae67230918)  
(KB2505927)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2008 for Mac](http://www.microsoft.com/downloads/details.aspx?familyid=84dfe3f4-a2a1-47b9-8da1-29ae67230918)  
(KB2505927)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2008 for Mac](http://www.microsoft.com/downloads/details.aspx?familyid=84dfe3f4-a2a1-47b9-8da1-29ae67230918)  
(KB2505927)  
(Vysoký)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office for Mac 2011
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Microsoft Office for Mac 2011](http://www.microsoft.com/downloads/details.aspx?familyid=ef1e612f-d8e3-4628-9fe4-ad136f0debd3)  
(KB2525412)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Microsoft Office for Mac 2011](http://www.microsoft.com/downloads/details.aspx?familyid=ef1e612f-d8e3-4628-9fe4-ad136f0debd3)  
(KB2525412)  
(Vysoký)
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
Netýká se
</td>
<td style="border:1px solid black;">
[Otevření nástroje XML File Format Converter for Mac](http://www.microsoft.com/downloads/details.aspx?familyid=0c323a12-6385-4666-ad39-a9516a8eda14)  
(KB2505935)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Otevření nástroje XML File Format Converter for Mac](http://www.microsoft.com/downloads/details.aspx?familyid=0c323a12-6385-4666-ad39-a9516a8eda14)  
(KB2505935)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Otevření nástroje XML File Format Converter for Mac](http://www.microsoft.com/downloads/details.aspx?familyid=0c323a12-6385-4666-ad39-a9516a8eda14)  
(KB2505935)  
(Vysoký)
</td>
</tr>
<tr>
<th colspan="5" style="border:1px solid black;">
Jiný software systému Office
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS11-029**](http://go.microsoft.com/fwlink/?linkid=208524)
</td>
<td style="border:1px solid black;">
[**MS11-021**](http://go.microsoft.com/fwlink/?linkid=210121)
</td>
<td style="border:1px solid black;">
[**MS11-022**](http://go.microsoft.com/fwlink/?linkid=210727)
</td>
<td style="border:1px solid black;">
[**MS11-023**](http://go.microsoft.com/fwlink/?linkid=210206)
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
<td style="border:1px solid black;">
Žádný
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Excel Viewer Service Pack 2
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Microsoft Excel Viewer Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2d75786a-2368-4ef2-970b-fa2e57d63ca9)  
(KB2466158)  
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
Microsoft PowerPoint Viewer 2007 Service Pack 2
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Microsoft PowerPoint Viewer 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=6e23d3c3-2944-42ea-80b3-0663af60d0f1)  
(KB2464623)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft PowerPoint Viewer
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Microsoft PowerPoint Viewer](http://www.microsoft.com/downloads/details.aspx?familyid=44a703f5-b581-4900-bdbb-0f0e8d9bf0e6)  
(KB2519984)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Sada Microsoft Office Compatibility Pack pro formáty souborů aplikací Word, Excel a PowerPoint 2007 Service Pack 2
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Sada Microsoft Office Compatibility Pack pro formáty souborů aplikací Word, Excel a PowerPoint 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=946cc611-4d75-4728-b9d3-1c8b557b02c2)  
(KB2466156)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Sada Microsoft Office Compatibility Pack pro formáty souborů aplikací Word, Excel a PowerPoint 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=913efc28-7deb-47b8-8c22-8eb5fc2631e4)  
(KB2464635)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
</tr>
</table>
<p></p>

 
**Poznámka k bulletinu MS11-029**

Více aktualizovaných souborů v rámci stejného identifikátoru bulletinu naleznete také v dalších kategoriích softwaru v rámci této části **Software obsahující tuto chybu a umístění aktualizací ke stažení**. Tento bulletin se vztahuje na více kategorií softwaru.

**Poznámka k bulletinu MS11-021**

<sup>[1]</sup>Na ochranu před chybami zabezpečení popsanými v tomto bulletinu je u aplikací Microsoft Excel 2007 Service Pack 2 kromě balíčku aktualizací zabezpečení KB2464583 potřeba nainstalovat také aktualizaci zabezpečení pro sadu Microsoft Office Compatibility Pack pro formáty souborů aplikací Word, Excel a PowerPoint 2007 Service Pack 2 (KB2466156).

**Poznámka k bulletinu MS11-022**

Více aktualizovaných souborů v rámci stejného identifikátoru bulletinu naleznete také v dalších kategoriích softwaru v rámci této části **Software obsahující tuto chybu a umístění aktualizací ke stažení**. Tento bulletin se vztahuje na více kategorií softwaru.

#### Microsoft Server Software

 
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
Microsoft Office Web Apps
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS11-022**](http://go.microsoft.com/fwlink/?linkid=210727)
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
Microsoft Office Web Apps
</td>
<td style="border:1px solid black;">
[Microsoft PowerPoint Web App](http://www.microsoft.com/downloads/details.aspx?familyid=9847dc05-7d4a-4a64-9e6a-622d3fa171f9)  
(KB2520047)  
(Vysoký)
</td>
</tr>
</table>
<p></p>

 
**Poznámka k bulletinu MS11-022**

Více aktualizovaných souborů v rámci stejného identifikátoru bulletinu naleznete také v dalších kategoriích softwaru v rámci této části **Software obsahující tuto chybu a umístění aktualizací ke stažení**. Tento bulletin se vztahuje na více kategorií softwaru.

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
[**MS11-025**](http://go.microsoft.com/fwlink/?linkid=209720)
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
Microsoft Visual Studio .NET 2003 Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft Visual Studio .NET 2003 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=e9501082-a651-452b-8c1a-43987ffd3102)  
(KB2465373)  
(Vysoký)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Visual Studio 2005 Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft Visual Studio 2005 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=ee64d83b-6c06-4ccf-b12d-99e2a7a7b18d)  
(KB2538218)  
(Vysoký)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Visual Studio 2008 Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft Visual Studio 2008 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=e6a8e024-12ee-43d5-9aae-4c721505d6df)  
(KB2538241)  
(Vysoký)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Visual Studio 2010 a Microsoft Visual Studio 2010 Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft Visual Studio 2010](http://www.microsoft.com/downloads/details.aspx?familyid=7fd643a8-8e05-4d27-8853-33f79f01cb26)  
(KB2542054)  
(Vysoký)  
[Microsoft Visual Studio 2010 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=1a21c9db-dfa3-4a07-a1e0-89a8069b7c17)  
(KB2565057)  
(Vysoký)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Visual C++ 2005 Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft Visual C++ 2005 Service Pack 1 Redistributable Package](http://www.microsoft.com/downloads/details.aspx?familyid=ae2e1a40-7b45-4fe9-a20f-2ed2923aca62)  
(KB2538242)  
(Vysoký)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Visual C++ 2008 Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft Visual C++ 2008 Service Pack 1 Redistributable Package](http://www.microsoft.com/downloads/details.aspx?familyid=a821847e-4c44-45c0-9128-61c822bb3280)  
(KB2538243)  
(Vysoký)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Visual C++ 2010 a Microsoft Visual C++ 2010 Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft Visual C++ 2010 Redistributable Package](http://www.microsoft.com/downloads/details.aspx?familyid=fe558aed-9274-415f-8a0f-d9d8622fb35b)  
(KB2467173)  
(Vysoký)  
[Microsoft Visual C++ 2010 Redistributable Package Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=7557d29b-731b-4abb-8815-2b87a4132efb)  
(KB2565063)  
(Vysoký)
</td>
</tr>
</table>
<p></p>

 

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

Další informace o způsobu instalace této aktualizace zabezpečení pomocí služby Windows Server Update Services získáte na webu služby [Windows Server Update Services](http://go.microsoft.com/fwlink/?linkid=50120).

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

-   Anonymnímu výzkumníkovi, spolupracujícímu se společností [VeriSign iDefense Labs](http://labs.idefense.com/), za oznámení chyby popsané v bulletinu MS11-018.
-   Společnosti [MITRE](http://mitre.org/) za spolupráci na řešení chyby popsané v bulletinu MS11-018.
-   Michalovi Zalewskému ze společnosti [Google Inc.](http://www.google.com/) za spolupráci na řešení chyby popsané v bulletinu MS11-018.
-   Davidu Bloomovi ze společnosti [Google Inc.](http://www.google.com/) za oznámení dvou chyb popsaných v bulletinu MS11-018.
-   Stephenu Fewerovi ze společnosti [Harmony Security](http://www.harmonysecurity.com/), spolupracujícímu s organizací [Zero Day Initiative](http://www.zerodayinitiative.com/) společnosti [TippingPoint](http://www.tippingpoint.com/), za oznámení chyby popsané v bulletinu MS11-018.
-   Alinu Radu Popovi ze společnosti [Secunia Research](http://secunia.com/) za oznámení dvou chyb popsaných v bulletinu MS11-021.
-   Muhammadu Junaid Bohiovi ze společnosti [Telus Security Labs](http://www.telussecuritylabs.com) za oznámení chyby popsané v bulletinu MS11-021.
-   Uživateli Aniway, spolupracujícímu s organizací [Zero Day Initiative](http://www.zerodayinitiative.com/) společnosti [TippingPoint](http://www.tippingpoint.com/), za oznámení tří chyb popsaných v bulletinu MS11-021.
-   Anonymnímu výzkumníkovi, spolupracujícímu se společností [VeriSign iDefense Labs](http://labs.idefense.com/), za oznámení chyby popsané v bulletinu MS11-021.
-   Rodrigu Rubira Brancovi z [výzkumného týmu chyb zabezpečení Check Point](http://www.checkpoint.com/) (VDT) za oznámení chyby popsané v bulletinu MS11-021.
-   Anonymnímu výzkumníkovi, spolupracujícímu s organizací [Zero Day Initiative](http://www.zerodayinitiative.com/) společnosti [TippingPoint](http://www.tippingpoint.com/), za oznámení chyby popsané v bulletinu MS11-021.
-   Anonymnímu výzkumníkovi, spolupracujícímu s organizací [Zero Day Initiative](http://www.zerodayinitiative.com/) společnosti [TippingPoint](http://www.tippingpoint.com/), za oznámení chyby popsané v bulletinu MS11-021.
-   Organizaci [Zero Day Initiative](http://www.zerodayinitiative.com/) společnosti [TippingPoint](http://www.tippingpoint.com/) za oznámení tří chyb zabezpečení popsaných v bulletinu MS11-022.
-   Haifei Liovi z výzkumného týmu [FortiGuard Labs společnosti Fortinet](http://www.fortiguard.com/) za oznámení chyby popsané v bulletinu MS11-023.
-   Anonymnímu výzkumníkovi, spolupracujícímu s organizací [Zero Day Initiative](http://www.zerodayinitiative.com/) společnosti [TippingPoint](http://www.tippingpoint.com/), za oznámení chyby popsané v bulletinu MS11-023.
-   Carstenu Eiramovi ze společnosti [Secunia](http://secunia.com/) za spolupráci na řešení chyby popsané v bulletinu MS11-024.
-   Týmu [Google Security Team](http://www.google.com/) za spolupráci na řešení chyby popsané v bulletinu MS11-026.
-   Chrisi Riesovi z pobočky pro zabezpečení informací univerzity Carnegie Mellon za oznámení chyby popsané v bulletinu MS11-027.
-   Uživateli RadLSneak, spolupracujícímu se skupinou [iSIGHT Partners](http://www.isightpartners.com/) Global Vulnerability Partnership, za oznámení chyby popsané v bulletinu MS11-027.
-   Nicolasi Jolymu a Chaoukimu Bekrarovi z programu [VUPEN Threat Protection Program](http://www.vupen.com/english/services/tpp-index.php) za oznámení chyby popsané v bulletinu MS11-029.
-   Neelu Mehtovi ze společnosti [Google Inc.](http://www.google.com/) za oznámení chyby popsané v bulletinu MS11-030.
-   [Jessi Rudermanovi](http://www.squarefree.com/) ze společnosti [Mozilla](http://www.mozilla.org/) za spolupráci na řešení chyby popsané v bulletinu MS11-031.
-   Adamu Twardochovi ze společnosti [Fontlab Ltd.](http://www.fontlab.com/) za oznámení chyby popsané v bulletinu MS11-032.
-   Carstenu Eiramovi ze společnosti [Secunia](http://secunia.com/) za oznámení chyby popsané v bulletinu MS11-033.
-   Tarjei Mandtovi ze společnosti [Norman](http://www.norman.com/) za oznámení 30 chyb popsaných v bulletinu MS11-034.

#### Technická podpora

-   Uvedený software byl testován za účelem zjištění, kterých verzí se chyba týká. U dalších verzí skončila časově omezená podpora. Pokud chcete zjistit dobu, po kterou je pro určitou verzi softwaru poskytována podpora, navštivte web [Zásady poskytování technické podpory pro produkty společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=21742).
-   Zákazníci mohou získat technickou podporu na webu [služby technické podpory společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=21131). Hovory související s aktualizacemi zabezpečení jsou bezplatné. Další informace o dostupných možnostech technické podpory naleznete na webu [Pomoc a podpora společnosti Microsoft](http://support.microsoft.com/).
-   Mezinárodní zákazníci získají podporu u místních zastoupení společnosti Microsoft. Technická podpora související s aktualizacemi zabezpečení je bezplatná. Další informace o možnostech kontaktování společnosti Microsoft v případě potřeby technické podpory získáte na [webu mezinárodní technické podpory](http://go.microsoft.com/fwlink/?linkid=21155).

#### Zřeknutí se záruky

Informace ve znalostní bázi Microsoft Knowledge Base jsou poskytovány tak, jak jsou, bez jakékoli záruky. Společnost Microsoft neposkytuje žádné záruky, výslovně uvedené či mlčky předpokládané, včetně záruk obchodovatelnosti a vhodnosti pro určitý účel. Společnost Microsoft ani její dodavatelé nenesou v žádném případě zodpovědnost za žádné škody, včetně přímých, nepřímých, náhodných či následných škod, ztráty zisku či zvláštních škod, a to ani v případě, že byli na možnost takových škod upozorněni. V některých zemích a právních řádech není dovoleno vyloučit nebo omezit odpovědnost, proto se výše uvedené omezení na vás nemusí vztahovat.

#### Revize

-   V1.0 (12. dubna 2011): Souhrnný bulletin byl publikován.
-   V1.1 (13. dubna 2011): V části Shrnutí došlo k objasnění popisu chyby zabezpečení uvedené v bulletinu MS11-019.
-   V2.0 (15. dubna 2011): V bulletinu MS11-032 byl zvýšen hodnoticí stupeň indexu zneužitelnosti pro chybu CVE-2011-0034 na stupeň „1 – Je pravděpodobné vytvoření kódu konsistentního zneužití“.
-   V3.0 (21. dubna 2011): Revidován tak, aby nabídl nové vydání aktualizace zabezpečení pro bulletin MS11-025.
-   V3.1 (27. dubna 2011): Byl opraven index zneužitelnosti v bulletinu MS11-024 přidáním chyby zabezpečení CVE-2010-4701 mezi chyby řešené touto aktualizací. Jedná se pouze o změnu informace.
-   V4.0 (16. května 2011): Byl znovu vydán bulletin MS11-018, aby znovu nabídl aktualizaci pro aplikaci Internet Explorer 7 v podporovaných edicích systémů Windows XP a Windows Server 2003. Jedná se pouze o změnu detekce. Nebyly provedeny žádné změny binárních souborů. Tato aktualizace bude nabídnuta pouze postiženým zákazníkům. Zákazníci, kteří nainstalovali aktualizaci ručně, a zákazníci používající konfiguraci nepostiženou změnou logiky detekce nemusí podnikat žádná opatření.
-   V5.0 (14. června 2011): Bulletin MS11-025 znovu nabízí aktualizace pro aplikace Microsoft Visual Studio 2005 Service Pack 1, Microsoft Visual Studio 2008 Service Pack 1, Microsoft Visual Studio 2010, Microsoft Visual C++ 2005 Service Pack 1 Redistributable Package a Microsoft Visual C++ 2008 Service Pack 1 Redistributable Package. Zákazníci, kteří tuto aktualizaci dříve nainstalovali v systémech postižených chybou zabezpečení, by měli nainstalovat nové balíčky.
-   V6.0 (9. srpna 2011): Do seznamu softwaru obsahujícího chybu zabezpečení, uvedeného v bulletinu MS11-025, byly přidány aplikace Microsoft Visual Studio 2010 Service Pack 1 (KB2565057) a Microsoft Visual C++ 2010 Redistributable Package Service Pack 1 (KB2565063).
-   V6.1 (26. října 2011): V bulletinu MS11-028 byla opravena informace o použitelnosti instalace Server Core pro rozhraní .NET Framework 4 v systému Windows Server 2008 R2 pro systémy s procesorem x64.

*Built at 2014-04-18T01:50:00Z-07:00*
