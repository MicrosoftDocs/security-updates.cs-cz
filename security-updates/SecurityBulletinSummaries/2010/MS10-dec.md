---
TOCTitle: 'MS10-DEC'
Title: 'Souhrnný bulletin zabezpečení společnosti Microsoft, prosinec 2010'
ms:assetid: 'ms10-dec'
ms:contentKeyID: 61223996
ms:mtpsurl: 'https://technet.microsoft.com/cs-CZ/library/ms10-dec(v=Security.10)'
---

 

Souhrnný bulletin zabezpečení společnosti Microsoft, prosinec 2010
==================================================================

Publikováno: 14. prosince 2010 | Aktualizováno: 15. prosince 2010

**Verze:** 1.1

Tento souhrnný bulletin uvádí bulletiny zabezpečení vydané v prosinci 2010.

Spolu s vydáním bulletinů pro prosinec 2010 nahrazuje tento souhrnný bulletin předběžné oznámení o bulletinech vydané 9. prosince 2010. Další informace o službě předběžného oznámení o bulletinech naleznete v části [Předběžné oznámení o bulletinech zabezpečení společnosti Microsoft](http://technet.microsoft.com/security/bulletin/advance).

Informace o tom, jak dostávat automatická oznámení o vydání nových bulletinů zabezpečení společnosti Microsoft, naleznete na webu [Zasílání technických oznámení o zabezpečení společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=21163).

Pro zodpovězení zákaznických dotazů týkajících se těchto bulletinů uspořádá společnost Microsoft webové vysílání 15. prosince 2010 v 11:00 časového pásma Tichomoří (USA a Kanada). [Registrovat se pro webové vysílání týkající se prosincových bulletinů zabezpečení](https://msevents.microsoft.com/cui/webcasteventdetails.aspx?eventid=1032454444&eventcategory=4&culture=en-us&countrycode=us). Po tomto datu je webové vysílání dostupné na požádání. Další informace získáte v [souhrnných bulletinech zabezpečení společnosti Microsoft a webovém vysílání](http://technet.microsoft.com/security/bulletin/summary).

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
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=206495">MS10-090</a></td>
<td style="border:1px solid black;"><strong>Kumulativní aktualizace zabezpečení pro aplikaci Internet Explorer (2416400)</strong><br />
<br />
Tato aktualizace zabezpečení řeší čtyři chyby zabezpečení oznámené soukromými osobami a tři veřejně známé chyby zabezpečení v aplikaci Internet Explorer. Nejzávažnější chyby zabezpečení mohou umožnit vzdálené spuštění kódu, pokud uživatel pomocí aplikace Internet Explorer zobrazí speciálně vytvořenou webovou stránku. Uživatelé, jejichž účty jsou konfigurovány tak, aby měli v systému méně uživatelských práv, by byli vystaveni menšímu riziku než uživatelé s uživatelskými právy správce.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritický</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Internet Explorer</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=203895">MS10-091</a></td>
<td style="border:1px solid black;"><strong>Chyby zabezpečení ovladače písma OpenType (OTF) umožňují vzdálené spuštění kódu (2296199)</strong><br />
<br />
Tato aktualizace zabezpečení řeší chyby zabezpečení oznámené soukromými osobami týkající se ovladače písma OpenType (OTF) v systému Windows, které umožňují vzdálené spuštění kódu. Útočník by mohl být hostitelem speciálně vytvořeného písma OpenType ve sdílené složce na síti. Cesta k postiženému ovládání je aktivována přechodem uživatele ke sdílené složce v programu Průzkumník Windows, což umožní speciálně vytvořenému písmu převzít úplnou kontrolu nad postiženým systémem. Útočník by tak mohl instalovat programy, zobrazovat, měnit či odstraňovat data nebo vytvářet nové účty s úplnými uživatelskými právy.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritický</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=203463">MS10-092</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení služby Plánovač úloh umožňuje zvýšení úrovně oprávnění (2305420)</strong><br />
<br />
Tato aktualizace zabezpečení řeší veřejně známou chybu zabezpečení služby Plánovač úloh v systému Windows. Tato chyba zabezpečení by mohla způsobit zvýšení úrovně oprávnění, pokud by se útočník přihlásil k postiženému systému a spustil speciálně vytvořenou aplikaci. Tuto chybu může zneužít pouze útočník s platnými pověřeními pro přihlášení, která by mu umožňovala se místně přihlásit. Tuto chybu zabezpečení nemohou zneužít vzdálení ani anonymní uživatelé.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Vysoký</a><br />
Zvýšení úrovně oprávnění</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=206698">MS10-093</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení v programu Windows Movie Maker umožňuje vzdálené spuštění kódu (2424434)</strong><br />
<br />
Tato aktualizace zabezpečení řeší veřejně známou chybu zabezpečení programu Windows Movie Maker. Chyba zabezpečení by mohla umožnit vzdálené spuštění kódu, pokud útočník přesvědčí uživatele, aby otevřel legitimní soubor programu Windows Movie Maker umístěný ve stejném síťovém adresáři jako speciálně vytvořený soubor knihovny. Úspěšný útok by vyžadoval, aby útočník navštívil nedůvěryhodné systémové umístění vzdáleného souboru nebo sdílenou složku protokolu WebDAV a otevřel z tohoto umístění dokument, který by pak načetla aplikace obsahující chybu zabezpečení.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Vysoký</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Může vyžadovat restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=206699">MS10-094</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení v programu Windows Media Encoder umožňuje vzdálené spuštění kódu (2447961)</strong><br />
<br />
Tato aktualizace zabezpečení řeší veřejně známou chybu zabezpečení programu Windows Media Encoder. Chyba zabezpečení by mohla umožnit vzdálené spuštění kódu, pokud útočník přesvědčí uživatele, aby otevřel legitimní soubor programu Windows Media Profile (s příponou PRX) umístěný ve stejném síťovém adresáři jako speciálně vytvořený soubor knihovny. Úspěšný útok by vyžadoval, aby útočník navštívil nedůvěryhodné systémové umístění vzdáleného souboru nebo sdílenou složku protokolu WebDAV a otevřel z tohoto umístění dokument, který by pak načetla aplikace obsahující chybu zabezpečení.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Vysoký</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Může vyžadovat restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=206683">MS10-095</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení v systému Microsoft Windows umožňuje vzdálené spuštění kódu (2385678)</strong><br />
<br />
Tato aktualizace zabezpečení řeší chybu zabezpečení v systému Microsoft Windows, kterou oznámila soukromá osoba. Chyba zabezpečení by mohla umožnit vzdálené spuštění kódu, pokud by uživatel otevřel soubor s příponou EML a RSS (Windows Live Mail) nebo WPOST (Microsoft Live Writer) umístěný ve stejné síťové složce jako speciálně vytvořený soubor knihovny. Úspěšný útok by vyžadoval, aby útočník navštívil nedůvěryhodné systémové umístění vzdáleného souboru nebo sdílenou složku protokolu WebDAV a otevřel z tohoto umístění dokument, který by pak načetla aplikace obsahující chybu zabezpečení.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Vysoký</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=206738">MS10-096</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení adresáře systému Windows umožňuje vzdálené spuštění kódu (2423089)</strong><br />
<br />
Tato aktualizace zabezpečení řeší veřejně známou chybu zabezpečení v adresáři systému Windows. Chyba zabezpečení by mohla umožnit vzdálené spuštění kódu, pokud by uživatel otevřel soubor adresáře systému Windows umístěný ve stejné síťové složce jako speciálně vytvořený soubor knihovny. Úspěšný útok by vyžadoval, aby útočník navštívil nedůvěryhodné systémové umístění vzdáleného souboru nebo sdílenou složku protokolu WebDAV a otevřel z tohoto umístění dokument, který by pak načetla aplikace obsahující chybu zabezpečení.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Vysoký</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Může vyžadovat restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=206689">MS10-097</a></td>
<td style="border:1px solid black;"><strong>Nezabezpečené načítání knihovny v Průvodci přihlášením k připojení k internetu by mohlo umožnit vzdálené spuštění kódu (2443105)</strong><br />
<br />
Tato aktualizace zabezpečení řeší veřejně známou chybu zabezpečení v Průvodci přihlášením k připojení k internetu v systému Microsoft Windows. Tato aktualizace zabezpečení je označena jako důležitá pro všechny podporované verze systému Windows XP a Windows Server 2003. Všechny podporované edice systémů Windows Vista, Windows Server 2008, Windows 7 a Windows Server 2008 R2 nejsou postiženy zmíněnou chybou zabezpečení.<br />
<br />
Chyba zabezpečení by mohla umožnit vzdálené spuštění kódu, pokud by uživatel otevřel soubor s příponou INS nebo ISP umístěný ve stejné síťové složce jako speciálně vytvořený soubor knihovny. Úspěšný útok by vyžadoval, aby útočník navštívil nedůvěryhodné systémové umístění vzdáleného souboru nebo sdílenou složku protokolu WebDAV a otevřel z tohoto umístění dokument, který by pak načetla aplikace obsahující chybu zabezpečení.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Vysoký</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Může vyžadovat restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=204869">MS10-098</a></td>
<td style="border:1px solid black;"><strong>Chyby zabezpečení v ovladačích režimu jádra systému Windows umožňují zvýšení úrovně oprávnění (2436673)</strong><br />
<br />
Tato aktualizace zabezpečení řeší jednu veřejně známou a několik soukromou osobou oznámených chyb zabezpečení systému Microsoft Windows. Tyto chyby zabezpečení by mohly umožnit zvýšení úrovně oprávnění, pokud by se útočník místně přihlásil k systému a spustil speciálně vytvořenou aplikaci. Tyto chyby zabezpečení může zneužít pouze útočník s platnými pověřeními pro přihlášení, která by mu umožňovala se místně přihlásit. Uvedené chyby zabezpečení nemohou zneužít vzdálení ani anonymní uživatelé.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Vysoký</a><br />
Zvýšení úrovně oprávnění</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=206365">MS10-099</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení služby Směrování a vzdálený přístup umožňuje zvýšení úrovně oprávnění (2440591)</strong><br />
<br />
Tato aktualizace zabezpečení řeší soukromě oznámenou chybu zabezpečení služby Směrování a vzdálený přístup komponenty NDProxy systému Microsoft Windows. Tato aktualizace zabezpečení je označena jako důležitá pro všechny podporované verze systému Windows XP a Windows Server 2003. Všechny podporované edice systémů Windows Vista, Windows Server 2008, Windows 7 a Windows Server 2008 R2 nejsou postiženy zmíněnou chybou zabezpečení.<br />
<br />
Tato chyba zabezpečení by mohla způsobit zvýšení úrovně oprávnění, pokud by se útočník přihlásil k postiženému systému a spustil speciálně vytvořenou aplikaci. Tuto chybu může zneužít pouze útočník s platnými pověřeními pro přihlášení, která by mu umožňovala se místně přihlásit. Tuto chybu zabezpečení nemohou zneužít vzdálení ani anonymní uživatelé.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Vysoký</a><br />
Zvýšení úrovně oprávnění</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=204906">MS10-100</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení v odsouhlaseném uživatelském rozhraní by mohla umožnit zvýšení úrovně oprávnění (2442962)</strong><br />
<br />
Tato aktualizace zabezpečení řeší chybu zabezpečení odsouhlaseného uživatelského rozhraní oznámenou soukromou osobou. Tato chyba zabezpečení umožňuje zvýšit úroveň oprávnění, pokud útočník spustí v postiženém systému speciálně vytvořenou aplikaci. Tuto chybu může zneužít pouze útočník s platnými pověřeními pro přihlášení a oprávněním SelmpersonatePrivilege, které by mu umožňovaly se místně přihlásit. Tuto chybu zabezpečení nemohou zneužít vzdálení ani anonymní uživatelé.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Vysoký</a><br />
Zvýšení úrovně oprávnění</td>
<td style="border:1px solid black;">Může vyžadovat restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=201319">MS10-101</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení služby Windows Netlogon může způsobit odmítnutí služby (2207559)</strong><br />
<br />
Tato aktualizace zabezpečení řeší soukromě oznámenou chybu zabezpečení služby Netlogon RPC v postižených verzích systému Windows Server konfigurovaných tak, aby sloužily jako řadiče domény. Chyba zabezpečení by mohla umožnit odmítnutí služby, pokud by útočník zaslal speciálně vytvořený paket RPC do rozhraní služby Netlogon RPC postiženého systému. Ke zneužití této chyby zabezpečení by útočník musel mít oprávnění pro správu počítače připojeného ke stejné doméně jako postižený řadič domény.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Vysoký</a><br />
Odmítnutí služby</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=205309">MS10-102</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení technologie Hyper-V může způsobit odmítnutí služby (2345316)</strong><br />
<br />
Tato aktualizace zabezpečení řeší chybu zabezpečení ve funkci Hyper-V systému Windows Server 2008 Hyper-V a Windows Server 2008 R2, kterou oznámila soukromá osoba. Tato chyba zabezpečení by mohla způsobit odmítnutí služby, pokud by ověřený uživatel odeslal do sběrnice VMBus v jednom z virtuálních strojů hosta provozovaných serverem Hyper-V speciálně vytvořený paket. Ke zneužití této chyby zabezpečení by útočník musel mít platná oprávnění pro přihlášení a možnost odeslat speciálně vytvořený obsah z virtuálního stroje hosta. Tuto chybu zabezpečení nemohou zneužít vzdálení ani anonymní uživatelé.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Vysoký</a><br />
Odmítnutí služby</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=198156">MS10-103</a></td>
<td style="border:1px solid black;"><strong>Chyby zabezpečení v aplikaci Microsoft Publisher umožňují vzdálené spuštění kódu (2292970)</strong><br />
<br />
Tato aktualizace zabezpečení řeší pět chyb zabezpečení aplikace Microsoft Publisher oznámených soukromou osobou, které by mohly umožnit vzdálené spuštění kódu v případě, že uživatel otevře speciálně vytvořený soubor aplikace Publisher. Útočník, který by úspěšně zneužil některou z těchto chyb zabezpečení, by mohl převzít úplnou kontrolu nad postiženým systémem. Útočník by tak mohl instalovat programy, zobrazovat, měnit či odstraňovat data nebo vytvářet nové účty s úplnými uživatelskými právy. Uživatelé, jejichž účty jsou konfigurovány tak, aby měli v systému méně uživatelských práv, by byli vystaveni menšímu riziku než uživatelé s uživatelskými právy správce.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Vysoký</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Může vyžadovat restartování</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=206469">MS10-104</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení ve službě Microsoft SharePoint umožňuje vzdálené spuštění kódu (2455005)</strong><br />
<br />
Tato aktualizace zabezpečení řeší chybu zabezpečení ve službě Microsoft SharePoint, kterou oznámila soukromá osoba. Chyba zabezpečení by mohla povolit vzdálené spuštění kódu v kontextu zabezpečení hostujícího uživatele, pokud by útočník odeslal speciálně vytvořený požadavek SOAP do služby Document Conversions Launcher v serverovém prostředí služby SharePoint využívajícím službu Document Conversions Load Balancer. Ve výchozím nastavení nejsou služby Document Conversions Load Balancer a Document Conversions Launcher v systému Microsoft Office SharePoint Server 2007 povolené.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Vysoký</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Může vyžadovat restartování</td>
<td style="border:1px solid black;">Microsoft SharePoint</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=147425">MS10-105</a></td>
<td style="border:1px solid black;"><strong>Chyby zabezpečení v grafických filtrech systému Microsoft Office umožňují vzdálené spuštění kódu (968095)</strong><br />
<br />
Tato aktualizace zabezpečení řeší sedm chyb zabezpečení v systému Microsoft Office oznámených soukromými osobami. Tyto chyby zabezpečení umožňují vzdálené spuštění kódu, pokud uživatel zobrazí v systému Microsoft Office speciálně vytvořený soubor s obrázkem. Útočník, který by úspěšně zneužil některou z těchto chyb zabezpečení, by mohl získat stejná uživatelská práva, jaká má místní uživatel. Uživatelé, jejichž účty jsou konfigurovány tak, aby měli v systému méně uživatelských práv, by byli vystaveni menšímu riziku než uživatelé s uživatelskými právy správce.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Vysoký</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Může vyžadovat restartování</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=204624">MS10-106</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení serveru Microsoft Exchange může způsobit odmítnutí služby (2407132)</strong><br />
<br />
Tato aktualizace zabezpečení řeší chybu zabezpečení na serveru Microsoft Exchange Server oznámenou soukromou osobou. Chyba zabezpečení může způsobit odmítnutí služby, pokud ověřený útočník pošle speciálně vytvořený síťový vzkaz do počítače, v němž je spuštěna služba Exchange. Doporučené postupy pro používání brány firewall a standardní konfigurace této brány zajišťují ochranu sítí před útoky pocházejícími z oblasti mimo rozlehlou síť. Je vhodné, aby systémy připojené k Internetu měly přístupný minimální počet portů.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Mírný</a><br />
Odmítnutí služby</td>
<td style="border:1px solid black;">Může vyžadovat restartování</td>
<td style="border:1px solid black;">Microsoft Exchange</td>
</tr>
</tbody>
</table>
<p></p>

  
Index zneužitelnosti  
--------------------
  
 
Následující tabulka uvádí hodnocení zneužitelnosti každé chyby zabezpečení uvedené v tomto měsíci. Chyby zabezpečení jsou řazeny v pořadí zmenšující se úrovně posouzení zneužitelnosti, jinak než tomu je u řazení podle čísla chyb. Uvedeny jsou pouze chyby zabezpečení ohodnocené stupněm závažnosti Kritický nebo Vysoký.
  
**Jak pracovat s touto tabulkou**
  
V této tabulce zjistíte, jaká je pravděpodobnost vydání funkčního zneužitelného kódu během 30 dní od vydání tohoto bulletinu zabezpečení pro všechny aktualizace zabezpečení, které bude třeba nainstalovat. Všechna níže uvedená hodnocení zvažte na základě vaší specifické konfigurace a podle závěrů hodnocení nastavte priority pro zavádění jednotlivých aktualizací. Další informace o významu těchto hodnocení a způsobu jejich stanovení najdete v indexu zneužitelnosti [Microsoft Exploitability Index](http://technet.microsoft.com/en-us/security/cc998259.aspx).
  
| ID bulletinu                                              | Název chyby zabezpečení                                                                                         | ID CVE                                                                           | Hodnocení indexu zneužitelnosti                                                                                                | Hlavní poznámky                                                                       |  
|-----------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------|  
| [MS10-103](http://go.microsoft.com/fwlink/?linkid=198156) | Chyba zabezpečení týkající se poškození haldy hodnoty velikosti v souboru pubconv.dll                           | [CVE-2010-2569](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2569) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní zneužití kódu je pravděpodobné               | (Žádné)                                                                               |  
| [MS10-103](http://go.microsoft.com/fwlink/?linkid=198156) | Chyba zabezpečení týkající se přetečení haldy v souboru pubconv.dll                                             | [CVE-2010-2570](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2570) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní zneužití kódu je pravděpodobné               | (Žádné)                                                                               |  
| [MS10-097](http://go.microsoft.com/fwlink/?linkid=206689) | Chyba zabezpečení týkající se nezabezpečeného načítání knihovny v Průvodci přihlášením k připojení k internetu  | [CVE-2010-3144](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3144) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní zneužití kódu je pravděpodobné               | **Tato chyba zabezpečení je veřejně známá.**                                          |  
| [MS10-096](http://go.microsoft.com/fwlink/?linkid=206738) | Chyba zabezpečení nezabezpečeného načítání knihovny                                                             | [CVE-2010-3147](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3147) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní zneužití kódu je pravděpodobné               | **Tato chyba zabezpečení je veřejně známá.**                                          |  
| [MS10-092](http://go.microsoft.com/fwlink/?linkid=203463) | Chyba zabezpečení služby Plánovač úloh                                                                          | [CVE-2010-3338](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3338) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní zneužití kódu je pravděpodobné               | **Dochází ke zneužití této chyby zabezpečení v prostředí Internetu**                  |  
| [MS10-090](http://go.microsoft.com/fwlink/?linkid=206495) | Chyba zabezpečení týkající se poškození paměti objektů HTML                                                     | [CVE-2010-3340](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3340) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní zneužití kódu je pravděpodobné               | (Žádné)                                                                               |  
| [MS10-090](http://go.microsoft.com/fwlink/?linkid=206495) | Chyba zabezpečení týkající se poškození paměti objektů HTML                                                     | [CVE-2010-3343](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3343) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní zneužití kódu je pravděpodobné               | (Žádné)                                                                               |  
| [MS10-090](http://go.microsoft.com/fwlink/?linkid=206495) | Chyba zabezpečení týkající se poškození paměti prvku HTML                                                       | [CVE-2010-3345](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3345) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní zneužití kódu je pravděpodobné               | (Žádné)                                                                               |  
| [MS10-090](http://go.microsoft.com/fwlink/?linkid=206495) | Chyba zabezpečení týkající se poškození paměti prvku HTML                                                       | [CVE-2010-3346](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3346) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní zneužití kódu je pravděpodobné               | (Žádné)                                                                               |  
| [MS10-098](http://go.microsoft.com/fwlink/?linkid=204869) | Chyba zabezpečení týkající se přetečení vyrovnávací paměti subsystému Win32k                                    | [CVE-2010-3939](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3939) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní zneužití kódu je pravděpodobné               | **Tato chyba zabezpečení je veřejně známá.**                                          |  
| [MS10-098](http://go.microsoft.com/fwlink/?linkid=204869) | Chyba zabezpečení týkající se dvojitého uvolnění ukazatele PFE subsystému Win32k                                | [CVE-2010-3940](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3940) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní zneužití kódu je pravděpodobné               | (Žádné)                                                                               |  
| [MS10-098](http://go.microsoft.com/fwlink/?linkid=204869) | Chyba zabezpečení týkající se propojení kurzorů v subsystému Win32k                                             | [CVE-2010-3943](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3943) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní zneužití kódu je pravděpodobné               | (Žádné)                                                                               |  
| [MS10-098](http://go.microsoft.com/fwlink/?linkid=204869) | Chyba zabezpečení týkající se poškození paměti subsystému Win32k                                                | [CVE-2010-3944](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3944) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní zneužití kódu je pravděpodobné               | (Žádné)                                                                               |  
| [MS10-105](http://go.microsoft.com/fwlink/?linkid=147425) | Chyba zabezpečení týkající se přetečení vyrovnávací paměti převaděče obrazu FlashPix                            | [CVE-2010-3951](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3951) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní zneužití kódu je pravděpodobné               | (Žádné)                                                                               |  
| [MS10-091](http://go.microsoft.com/fwlink/?linkid=203895) | Chyba zabezpečení týkající se dvojitého uvolnění písma OpenType                                                 | [CVE-2010-3957](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3957) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní zneužití kódu je pravděpodobné               | (Žádné)                                                                               |  
| [MS10-091](http://go.microsoft.com/fwlink/?linkid=203895) | Chyba zabezpečení tabulky CMAP písma OpenType                                                                   | [CVE-2010-3959](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3959) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní zneužití kódu je pravděpodobné               | (Žádné)                                                                               |  
| [MS10-100](http://go.microsoft.com/fwlink/?linkid=204906) | Chyba zabezpečení týkající se zosobnění odsouhlaseného uživatelského rozhraní                                   | [CVE-2010-3961](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3961) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní zneužití kódu je pravděpodobné               | (Žádné)                                                                               |  
| [MS10-090](http://go.microsoft.com/fwlink/?linkid=206495) | Chyba zabezpečení týkající se poškození neinicializované paměti                                                 | [CVE-2010-3962](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3962) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní zneužití kódu je pravděpodobné               | **V současné době dochází ke zneužití této chyby zabezpečení v prostředí Internetu.** |  
| [MS10-099](http://go.microsoft.com/fwlink/?linkid=206365) | Chyba zabezpečení týkající se přetečení vyrovnávací paměti komponenty NDProxy jádra                             | [CVE-2010-3963](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3963) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní zneužití kódu je pravděpodobné               | (Žádné)                                                                               |  
| [MS10-104](http://go.microsoft.com/fwlink/?linkid=206469) | Chyba zabezpečení poškozeného požadavku umožňující spuštění kódu                                                | [CVE-2010-3964](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3964) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní zneužití kódu je pravděpodobné               | (Žádné)                                                                               |  
| [MS10-094](http://go.microsoft.com/fwlink/?linkid=206699) | Chyba zabezpečení nezabezpečeného načítání knihovny                                                             | [CVE-2010-3965](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3965) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní zneužití kódu je pravděpodobné               | **Tato chyba zabezpečení je veřejně známá.**                                          |  
| [MS10-095](http://go.microsoft.com/fwlink/?linkid=206683) | Chyba zabezpečení nezabezpečeného načítání knihovny BranchCache                                                 | [CVE-2010-3966](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3966) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní zneužití kódu je pravděpodobné               | (Žádné)                                                                               |  
| [MS10-093](http://go.microsoft.com/fwlink/?linkid=206698) | Chyba zabezpečení nezabezpečeného načítání knihovny                                                             | [CVE-2010-3967](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3967) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní zneužití kódu je pravděpodobné               | **Tato chyba zabezpečení je veřejně známá.**                                          |  
| [MS10-103](http://go.microsoft.com/fwlink/?linkid=198156) | Chyba zabezpečení týkající se poškození paměti způsobené neplatným indexem v poli v souboru Pubconv.dll         | [CVE-2010-2571](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2571) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Nekonsistentní zneužití kódu je pravděpodobné             | (Žádné)                                                                               |  
| [MS10-098](http://go.microsoft.com/fwlink/?linkid=204869) | Chyba zabezpečení týkající se dvojitého uvolnění subsystému Win32k                                              | [CVE-2010-3941](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3941) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Nekonsistentní zneužití kódu je pravděpodobné             | (Žádné)                                                                               |  
| [MS10-098](http://go.microsoft.com/fwlink/?linkid=204869) | Chyba zabezpečení skriptu WriteAV subsystému Win32k                                                             | [CVE-2010-3942](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3942) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Nekonsistentní zneužití kódu je pravděpodobné             | (Žádné)                                                                               |  
| [MS10-105](http://go.microsoft.com/fwlink/?linkid=147425) | Chyba zabezpečení týkající se přetečení vyrovnávací paměti převaděče obrazu CGM                                 | [CVE-2010-3945](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3945) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Nekonsistentní zneužití kódu je pravděpodobné             | (Žádné)                                                                               |  
| [MS10-105](http://go.microsoft.com/fwlink/?linkid=147425) | Chyba zabezpečení týkající se přetečení celého čísla převaděče obrazu PICT                                      | [CVE-2010-3946](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3946) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Nekonsistentní zneužití kódu je pravděpodobné             | (Žádné)                                                                               |  
| [MS10-105](http://go.microsoft.com/fwlink/?linkid=147425) | Chyba zabezpečení týkající se přetečení haldy převaděče obrazu TIFF                                             | [CVE-2010-3947](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3947) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Nekonsistentní zneužití kódu je pravděpodobné             | (Žádné)                                                                               |  
| [MS10-105](http://go.microsoft.com/fwlink/?linkid=147425) | Chyba zabezpečení týkající se přetečení vyrovnávací paměti převaděče obrazu TIFF                                | [CVE-2010-3949](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3949) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Nekonsistentní zneužití kódu je pravděpodobné             | (Žádné)                                                                               |  
| [MS10-105](http://go.microsoft.com/fwlink/?linkid=147425) | Chyba zabezpečení týkající se poškození paměti převaděče obrazu TIFF                                            | [CVE-2010-3950](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3950) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Nekonsistentní zneužití kódu je pravděpodobné             | (Žádné)                                                                               |  
| [MS10-105](http://go.microsoft.com/fwlink/?linkid=147425) | Chyba zabezpečení týkající se poškození haldy převaděče obrazu FlashPix                                         | [CVE-2010-3952](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3952) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Nekonsistentní zneužití kódu je pravděpodobné             | (Žádné)                                                                               |  
| [MS10-103](http://go.microsoft.com/fwlink/?linkid=198156) | Chyba zabezpečení týkající se poškození paměti při indexování pole                                              | [CVE-2010-3955](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3955) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Nekonsistentní zneužití kódu je pravděpodobné             | (Žádné)                                                                               |  
| [MS10-091](http://go.microsoft.com/fwlink/?linkid=203895) | Chyba zabezpečení indexu písma OpenType                                                                         | [CVE-2010-3956](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3956) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Nekonsistentní zneužití kódu je pravděpodobné             | (Žádné)                                                                               |  
| [MS10-101](http://go.microsoft.com/fwlink/?linkid=201319) | Chyba zabezpečení týkající se vyhodnocování nulového ukazatele služby Netlogon RPC způsobující odmítnutí služby | [CVE-2010-2742](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2742) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Vytvoření funkčního zneužitelného kódu není pravděpodobné | Tato chyba může způsobit pouze odmítnutí služby.                                      |  
| [MS10-106](http://go.microsoft.com/fwlink/?linkid=204624) | Chyba zabezpečení nekonečné smyčky na serveru Exchange Server                                                   | [CVE-2010-3937](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3937) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Vytvoření funkčního zneužitelného kódu není pravděpodobné | Tato chyba může způsobit pouze odmítnutí služby.                                      |  
| [MS10-103](http://go.microsoft.com/fwlink/?linkid=198156) | Chyba zabezpečení týkající se poškození paměti aplikace Microsoft Publisher                                     | [CVE-2010-3954](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3954) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Vytvoření funkčního zneužitelného kódu není pravděpodobné | (Žádné)                                                                               |  
| [MS10-102](http://go.microsoft.com/fwlink/?linkid=205309) | Chyba zabezpečení sběrnice Hyper-V VMBus                                                                        | [CVE-2010-3960](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3960) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Vytvoření funkčního zneužitelného kódu není pravděpodobné | Tato chyba může způsobit pouze odmítnutí služby.                                      |
  
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
[**MS10-090**](http://go.microsoft.com/fwlink/?linkid=206495)
</td>
<td style="border:1px solid black;">
[**MS10-091**](http://go.microsoft.com/fwlink/?linkid=203895)
</td>
<td style="border:1px solid black;">
[**MS10-092**](http://go.microsoft.com/fwlink/?linkid=203463)
</td>
<td style="border:1px solid black;">
[**MS10-093**](http://go.microsoft.com/fwlink/?linkid=206698)
</td>
<td style="border:1px solid black;">
[**MS10-094**](http://go.microsoft.com/fwlink/?linkid=206699)
</td>
<td style="border:1px solid black;">
[**MS10-095**](http://go.microsoft.com/fwlink/?linkid=206683)
</td>
<td style="border:1px solid black;">
[**MS10-096**](http://go.microsoft.com/fwlink/?linkid=206738)
</td>
<td style="border:1px solid black;">
[**MS10-097**](http://go.microsoft.com/fwlink/?linkid=206689)
</td>
<td style="border:1px solid black;">
[**MS10-098**](http://go.microsoft.com/fwlink/?linkid=204869)
</td>
<td style="border:1px solid black;">
[**MS10-099**](http://go.microsoft.com/fwlink/?linkid=206365)
</td>
<td style="border:1px solid black;">
[**MS10-100**](http://go.microsoft.com/fwlink/?linkid=204906)
</td>
<td style="border:1px solid black;">
[**MS10-101**](http://go.microsoft.com/fwlink/?linkid=201319)
</td>
<td style="border:1px solid black;">
[**MS10-102**](http://go.microsoft.com/fwlink/?linkid=205309)
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
Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=6031d98a-cd0f-4dd8-80b6-70a7167e9e55)  
(Kritický)  
[Aplikace Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=922a0835-7f69-4e37-a9f7-c64e976e3513)  
(Kritický)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=a55b8029-9499-4219-99b7-65c30b0b864a)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=cdef3358-ad3e-40a6-9ba5-3be220a56a65)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Media Encoder 9 x86](http://www.microsoft.com/downloads/details.aspx?familyid=ef0ada2c-965f-438f-a1d3-bd45db8460c1)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=46baa431-126c-4fa5-9a7b-525008e2817d)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=fa9a1aac-b9c5-4d4e-9083-a080ad4ccc6f)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=bb9d1657-5beb-4372-b74c-a612a6fff5a8)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=4d0ae558-a4f2-4048-b5fd-ba072ca35e48)  
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
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=5d3a5678-77f8-4ebc-8775-aedd25ef0eb8)  
(Kritický)  
[Aplikace Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=a7c826b0-4aac-41ce-b297-6b6e11105c14)  
(Kritický)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=d5207bf5-7e58-4001-aa8f-f9a4b2c037d8)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=070fef8e-ba09-40f4-abaa-9cebf08983c3)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Media Encoder 9 x86](http://www.microsoft.com/downloads/details.aspx?familyid=dc777e61-e1e3-43bf-a84d-22c4a69c135d)  
(Vysoký)  
[Windows Media Encoder 9 x64](http://www.microsoft.com/downloads/details.aspx?familyid=550957c2-ce66-439f-95ea-681237513f75)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b9ce9d62-2eaa-48d8-bb6d-ea137e63d077)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=6dabc306-c858-46b1-815c-cd8d011ff62e)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=1f277ae4-4f85-4c8a-bfc5-dcdc8afed133)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=238bb885-eae6-464a-bb3d-679025f1cb50)  
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
[**MS10-090**](http://go.microsoft.com/fwlink/?linkid=206495)
</td>
<td style="border:1px solid black;">
[**MS10-091**](http://go.microsoft.com/fwlink/?linkid=203895)
</td>
<td style="border:1px solid black;">
[**MS10-092**](http://go.microsoft.com/fwlink/?linkid=203463)
</td>
<td style="border:1px solid black;">
[**MS10-093**](http://go.microsoft.com/fwlink/?linkid=206698)
</td>
<td style="border:1px solid black;">
[**MS10-094**](http://go.microsoft.com/fwlink/?linkid=206699)
</td>
<td style="border:1px solid black;">
[**MS10-095**](http://go.microsoft.com/fwlink/?linkid=206683)
</td>
<td style="border:1px solid black;">
[**MS10-096**](http://go.microsoft.com/fwlink/?linkid=206738)
</td>
<td style="border:1px solid black;">
[**MS10-097**](http://go.microsoft.com/fwlink/?linkid=206689)
</td>
<td style="border:1px solid black;">
[**MS10-098**](http://go.microsoft.com/fwlink/?linkid=204869)
</td>
<td style="border:1px solid black;">
[**MS10-099**](http://go.microsoft.com/fwlink/?linkid=206365)
</td>
<td style="border:1px solid black;">
[**MS10-100**](http://go.microsoft.com/fwlink/?linkid=204906)
</td>
<td style="border:1px solid black;">
[**MS10-101**](http://go.microsoft.com/fwlink/?linkid=201319)
</td>
<td style="border:1px solid black;">
[**MS10-102**](http://go.microsoft.com/fwlink/?linkid=205309)
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
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=4f1f41fb-368a-42e6-8d17-fca83b64f57b)  
(Kritický)  
[Aplikace Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=a3b57d26-5551-4785-86cf-41b532d78979)  
(Kritický)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=4f5a3677-0990-4702-bf08-af64cf12cb6c)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=9b70334c-490d-446c-988a-a88a75595fd4)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Media Encoder 9 x86](http://www.microsoft.com/downloads/details.aspx?familyid=ef0ada2c-965f-438f-a1d3-bd45db8460c1)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e0b2837c-019b-419b-954d-5bdc71a3a332)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8fa2cfa4-a01d-4910-b69f-736aeb585bab)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4aa39f59-2177-459f-9b8a-9543330d48ec)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c87af292-a068-4089-aab8-115c18b4b024)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ad843b97-2f6e-4406-a17a-627b7db8a926)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=6a9f56a0-230a-4dde-94da-f051ebf51f47)  
(Kritický)  
[Aplikace Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=8b0d2a3a-7fed-4d48-9ec5-8558000e51bb)  
(Kritický)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=1e134e5d-84fb-432b-99b1-593b1be5d5a4)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=08328e82-b012-4ea5-bf89-becb4881084f)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Media Encoder 9 x86](http://www.microsoft.com/downloads/details.aspx?familyid=dc777e61-e1e3-43bf-a84d-22c4a69c135d)  
(Vysoký)  
[Windows Media Encoder 9 x64](http://www.microsoft.com/downloads/details.aspx?familyid=550957c2-ce66-439f-95ea-681237513f75)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4c5cb600-9a39-40a0-be42-1593b1e0b97d)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=17b0b340-73b2-42a7-9d86-1297c63dcc2b)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=bca61d61-d5cf-49a4-ab99-b61e50e8f619)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e17b8878-d065-49cc-bdba-0f24cdf35ea3)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=0b0a06e7-0ae5-41f4-9ff5-d524fc0afbfa)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 SP2 pro systémy s procesorem Itanium
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=7c1cf126-604c-4f70-bbe8-aa4d145eb68f)  
(Kritický)  
[Aplikace Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=96884bfa-00c8-4263-9936-d7c054919dd3)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=15588d6a-f576-4e3d-95e8-d422af8a94de)  
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
[Windows Server 2003 SP2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=9abc8270-f3ac-474d-9ebc-410aaa6262cc)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=04a178cc-1afd-4e47-8cab-05e402e5a568)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=4fce129d-2b4e-4a66-af27-bbbde1e65ba1)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=ad896d80-167f-4e8f-a448-cac93516f4d0)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=7c0c2850-e81d-4347-aeb3-47036caa7c1b)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
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
[**MS10-090**](http://go.microsoft.com/fwlink/?linkid=206495)
</td>
<td style="border:1px solid black;">
[**MS10-091**](http://go.microsoft.com/fwlink/?linkid=203895)
</td>
<td style="border:1px solid black;">
[**MS10-092**](http://go.microsoft.com/fwlink/?linkid=203463)
</td>
<td style="border:1px solid black;">
[**MS10-093**](http://go.microsoft.com/fwlink/?linkid=206698)
</td>
<td style="border:1px solid black;">
[**MS10-094**](http://go.microsoft.com/fwlink/?linkid=206699)
</td>
<td style="border:1px solid black;">
[**MS10-095**](http://go.microsoft.com/fwlink/?linkid=206683)
</td>
<td style="border:1px solid black;">
[**MS10-096**](http://go.microsoft.com/fwlink/?linkid=206738)
</td>
<td style="border:1px solid black;">
[**MS10-097**](http://go.microsoft.com/fwlink/?linkid=206689)
</td>
<td style="border:1px solid black;">
[**MS10-098**](http://go.microsoft.com/fwlink/?linkid=204869)
</td>
<td style="border:1px solid black;">
[**MS10-099**](http://go.microsoft.com/fwlink/?linkid=206365)
</td>
<td style="border:1px solid black;">
[**MS10-100**](http://go.microsoft.com/fwlink/?linkid=204906)
</td>
<td style="border:1px solid black;">
[**MS10-101**](http://go.microsoft.com/fwlink/?linkid=201319)
</td>
<td style="border:1px solid black;">
[**MS10-102**](http://go.microsoft.com/fwlink/?linkid=205309)
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
Žádné
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
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=897351de-9697-4954-aa7e-169e980b932c)  
(Kritický)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=bebf0df0-5ebe-44b4-9ace-b3085a993e58)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 a Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2ddb8a06-c9cc-4d33-b6d1-22dbda2d871f)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 a Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=48f10251-34d8-4149-b4b2-bf3ec28f5846)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Movie Maker 2.6](http://www.microsoft.com/downloads/details.aspx?familyid=55141a02-3ad3-4691-98b9-80dd8ecb14c5)<sup>[1]</sup>
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Media Encoder 9 x86](http://www.microsoft.com/downloads/details.aspx?familyid=e8a57950-43cd-486f-bd97-70b0ad360a0b)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 a Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=a1c7f1b5-e054-4cd6-857d-2ab0a2fe9f62)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 a Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b824d3b9-2ce1-4abc-ae06-68aef1250be9)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 a Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=85265a23-5094-4007-8d33-f402cabd1664)  
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
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=171c02f9-f7d2-42f2-ba31-4c819a43784a)  
(Kritický)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=837b6056-af04-4aed-8afe-cc392770a590)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 a Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=9a245f3c-ffb6-4ccd-956c-e7d1231fca30)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 a Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=099ccc5f-b92f-4d06-bcb5-92e35c49f613)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Movie Maker 2.6](http://www.microsoft.com/downloads/details.aspx?familyid=5b078136-a492-4a2e-939d-82799f774d82)<sup>[1]</sup>
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Media Encoder 9 x86](http://www.microsoft.com/downloads/details.aspx?familyid=f98c3b96-acb5-49f1-be42-3dd44d316408)  
(Vysoký)  
[Windows Media Encoder 9 x64](http://www.microsoft.com/downloads/details.aspx?familyid=e1054088-f484-4f44-ba0e-5cbd21773c0c)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 a Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=73624b68-a69d-4517-b971-f0b7d2ccc9d6)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 a Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=f4c42cfe-b7f2-4436-919e-4bd305a3439a)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 a Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=63c7257a-16bf-4108-80b9-9dfe53528348)  
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
<th colspan="14" style="border:1px solid black;">
Windows Server 2008
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS10-090**](http://go.microsoft.com/fwlink/?linkid=206495)
</td>
<td style="border:1px solid black;">
[**MS10-091**](http://go.microsoft.com/fwlink/?linkid=203895)
</td>
<td style="border:1px solid black;">
[**MS10-092**](http://go.microsoft.com/fwlink/?linkid=203463)
</td>
<td style="border:1px solid black;">
[**MS10-093**](http://go.microsoft.com/fwlink/?linkid=206698)
</td>
<td style="border:1px solid black;">
[**MS10-094**](http://go.microsoft.com/fwlink/?linkid=206699)
</td>
<td style="border:1px solid black;">
[**MS10-095**](http://go.microsoft.com/fwlink/?linkid=206683)
</td>
<td style="border:1px solid black;">
[**MS10-096**](http://go.microsoft.com/fwlink/?linkid=206738)
</td>
<td style="border:1px solid black;">
[**MS10-097**](http://go.microsoft.com/fwlink/?linkid=206689)
</td>
<td style="border:1px solid black;">
[**MS10-098**](http://go.microsoft.com/fwlink/?linkid=204869)
</td>
<td style="border:1px solid black;">
[**MS10-099**](http://go.microsoft.com/fwlink/?linkid=206365)
</td>
<td style="border:1px solid black;">
[**MS10-100**](http://go.microsoft.com/fwlink/?linkid=204906)
</td>
<td style="border:1px solid black;">
[**MS10-101**](http://go.microsoft.com/fwlink/?linkid=201319)
</td>
<td style="border:1px solid black;">
[**MS10-102**](http://go.microsoft.com/fwlink/?linkid=205309)
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
Žádné
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 pro 32bitové systémy a Windows Server 2008 pro 32bitové systémy Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=f3785f3b-64c6-46a4-8e3a-9b9448124a8f)\*\*  
(Kritický)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=98183a76-5642-4e19-b488-029eb7ed3942)\*\*  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro 32bitové systémy a Windows Server 2008 pro 32bitové systémy Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=87149ec2-74a8-4dea-b7e3-873558e0103e)\*  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro 32bitové systémy a Windows Server 2008 pro 32bitové systémy Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=bdc9564a-4091-4cde-963a-239513db6c17)\*  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Media Encoder 9 x86](http://www.microsoft.com/downloads/details.aspx?familyid=a4ea028f-edfc-4237-8325-7ece11fcf437)\*\*  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro 32bitové systémy a Windows Server 2008 pro 32bitové systémy Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=118f528f-bd05-49c2-a4a4-78314cd00992)\*\*  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro 32bitové systémy a Windows Server 2008 pro 32bitové systémy Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=6e2f572a-4169-47f2-a872-5466997122ed)\*  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro 32bitové systémy a Windows Server 2008 pro 32bitové systémy Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=14e079a8-01a4-47c9-bd47-f5c9a6ca070a)\*\*  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro 32bitové systémy a Windows Server 2008 pro 32bitové systémy Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=6793f75b-cdf4-42ef-a53e-a1acb5b662d1)\*  
(Vysoký)
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
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=4b81aae5-6034-4c83-b5d2-e7e472435284)\*\*  
(Kritický)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=d47b457d-e995-4a7e-9bfa-eebab9b3a729)\*\*  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem x64 a Windows Server 2008 pro systémy s procesorem x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=523a47d3-771d-471a-889b-16311c276a00)\*  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem x64 a Windows Server 2008 pro systémy s procesorem x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=dff39bfe-0799-4912-ae22-392562178ae6)\*  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Media Encoder 9 x86](http://www.microsoft.com/downloads/details.aspx?familyid=f468d2b5-f02c-4691-9fb5-a7f69752f126)\*\*  
(Vysoký)  
[Windows Media Encoder 9 x64](http://www.microsoft.com/downloads/details.aspx?familyid=533d91d8-0291-421e-9701-3bd86d18bc45)\*\*  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem x64 a Windows Server 2008 pro systémy s procesorem x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=77e288fb-b51f-4f57-baac-1443d8fbd37b)\*\*  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem x64 a Windows Server 2008 pro systémy s procesorem x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=09a4b646-989d-43ef-a3e8-64af8b380a14)\*  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem x64 a Windows Server 2008 pro systémy s procesorem x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=6baf92b7-a336-45f2-a1ba-c00c34dfb76f)\*\*  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem x64 a Windows Server 2008 pro systémy s procesorem x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=85add876-ca5a-4a92-984e-188a72e349fc)\*  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem x64 a Windows Server 2008 pro systémy s procesorem x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b8c06bbc-6e84-4cf1-89f0-c0d34cfffaed)\*  
(Vysoký)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 pro systémy s procesorem Itanium a Windows Server 2008 pro systémy s procesorem Itanium Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=8ddafaaf-84a0-4325-b06f-4aac7cd61274)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem Itanium a Windows Server 2008 pro systémy s procesorem Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=959146ee-0e70-4e56-9012-72ed59aeb24b)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem Itanium a Windows Server 2008 pro systémy s procesorem Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=cf341a35-32ea-4ff7-aca9-1a4683c100ee)  
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
[Windows Server 2008 pro systémy s procesorem Itanium a Windows Server 2008 pro systémy s procesorem Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=82f71194-6f1f-4f43-8752-4bf5e5f94a93)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem Itanium a Windows Server 2008 pro systémy s procesorem Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=46522323-837e-4a74-9cf0-45f69343e776)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem Itanium a Windows Server 2008 pro systémy s procesorem Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7a4b23d4-f68e-4d5b-8814-d9247145f164)  
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
<th colspan="14" style="border:1px solid black;">
Windows 7
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS10-090**](http://go.microsoft.com/fwlink/?linkid=206495)
</td>
<td style="border:1px solid black;">
[**MS10-091**](http://go.microsoft.com/fwlink/?linkid=203895)
</td>
<td style="border:1px solid black;">
[**MS10-092**](http://go.microsoft.com/fwlink/?linkid=203463)
</td>
<td style="border:1px solid black;">
[**MS10-093**](http://go.microsoft.com/fwlink/?linkid=206698)
</td>
<td style="border:1px solid black;">
[**MS10-094**](http://go.microsoft.com/fwlink/?linkid=206699)
</td>
<td style="border:1px solid black;">
[**MS10-095**](http://go.microsoft.com/fwlink/?linkid=206683)
</td>
<td style="border:1px solid black;">
[**MS10-096**](http://go.microsoft.com/fwlink/?linkid=206738)
</td>
<td style="border:1px solid black;">
[**MS10-097**](http://go.microsoft.com/fwlink/?linkid=206689)
</td>
<td style="border:1px solid black;">
[**MS10-098**](http://go.microsoft.com/fwlink/?linkid=204869)
</td>
<td style="border:1px solid black;">
[**MS10-099**](http://go.microsoft.com/fwlink/?linkid=206365)
</td>
<td style="border:1px solid black;">
[**MS10-100**](http://go.microsoft.com/fwlink/?linkid=204906)
</td>
<td style="border:1px solid black;">
[**MS10-101**](http://go.microsoft.com/fwlink/?linkid=201319)
</td>
<td style="border:1px solid black;">
[**MS10-102**](http://go.microsoft.com/fwlink/?linkid=205309)
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
Žádné
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 pro 32bitové systémy
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=c288fe87-b113-4615-9b02-5e388bcb5241)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows 7 pro 32bitové systémy](http://www.microsoft.com/downloads/details.aspx?familyid=ff590db8-4264-42ba-9e07-88d100e1c4f5)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows 7 pro 32bitové systémy](http://www.microsoft.com/downloads/details.aspx?familyid=cf85cdb6-58c7-4144-82f6-f01a6a4f9c3a)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows 7 pro 32bitové systémy](http://www.microsoft.com/downloads/details.aspx?familyid=75591d37-2cb8-4cdf-acbb-89cd0d1a9290)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows 7 pro 32bitové systémy](http://www.microsoft.com/downloads/details.aspx?familyid=4e8ad5cd-af27-4f00-9378-ad778b8ee7b3)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows 7 pro 32bitové systémy](http://www.microsoft.com/downloads/details.aspx?familyid=aa7de2e4-ba48-4d58-b034-05349f0eb920)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows 7 pro 32bitové systémy](http://www.microsoft.com/downloads/details.aspx?familyid=f7c7d57a-d031-46a3-9613-eae2b9cb6401)  
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
Windows 7 pro systémy s procesorem x64
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=2cf4ac70-88b4-4840-9895-2bcf119312a7)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows 7 pro systémy s procesorem x64](http://www.microsoft.com/downloads/details.aspx?familyid=4ea4e339-9db2-4b99-b567-80ee55ecdf92)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows 7 pro systémy s procesorem x64](http://www.microsoft.com/downloads/details.aspx?familyid=0597018d-39f5-4ca9-b437-63d9e68f264d)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows 7 pro systémy s procesorem x64](http://www.microsoft.com/downloads/details.aspx?familyid=3a0c4dd0-98b4-4e7a-99ed-22b9d9f76cd1)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows 7 pro systémy s procesorem x64](http://www.microsoft.com/downloads/details.aspx?familyid=35a3e821-b463-411c-858b-d01eb5aed42b)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows 7 pro systémy s procesorem x64](http://www.microsoft.com/downloads/details.aspx?familyid=b21db627-91c2-4ebf-b7c0-38ac58ae5b6c)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows 7 pro systémy s procesorem x64](http://www.microsoft.com/downloads/details.aspx?familyid=e52c36f5-637b-4928-83d0-27514c6cc384)  
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
<th colspan="14" style="border:1px solid black;">
Windows Server 2008 R2
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS10-090**](http://go.microsoft.com/fwlink/?linkid=206495)
</td>
<td style="border:1px solid black;">
[**MS10-091**](http://go.microsoft.com/fwlink/?linkid=203895)
</td>
<td style="border:1px solid black;">
[**MS10-092**](http://go.microsoft.com/fwlink/?linkid=203463)
</td>
<td style="border:1px solid black;">
[**MS10-093**](http://go.microsoft.com/fwlink/?linkid=206698)
</td>
<td style="border:1px solid black;">
[**MS10-094**](http://go.microsoft.com/fwlink/?linkid=206699)
</td>
<td style="border:1px solid black;">
[**MS10-095**](http://go.microsoft.com/fwlink/?linkid=206683)
</td>
<td style="border:1px solid black;">
[**MS10-096**](http://go.microsoft.com/fwlink/?linkid=206738)
</td>
<td style="border:1px solid black;">
[**MS10-097**](http://go.microsoft.com/fwlink/?linkid=206689)
</td>
<td style="border:1px solid black;">
[**MS10-098**](http://go.microsoft.com/fwlink/?linkid=204869)
</td>
<td style="border:1px solid black;">
[**MS10-099**](http://go.microsoft.com/fwlink/?linkid=206365)
</td>
<td style="border:1px solid black;">
[**MS10-100**](http://go.microsoft.com/fwlink/?linkid=204906)
</td>
<td style="border:1px solid black;">
[**MS10-101**](http://go.microsoft.com/fwlink/?linkid=201319)
</td>
<td style="border:1px solid black;">
[**MS10-102**](http://go.microsoft.com/fwlink/?linkid=205309)
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
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 pro systémy s procesorem x64
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=99a91ba7-035b-4717-ada5-c1ad6645db64)\*\*  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem x64](http://www.microsoft.com/downloads/details.aspx?familyid=e52f7869-474a-44c8-a102-e766c576fc01)\*  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem x64](http://www.microsoft.com/downloads/details.aspx?familyid=28c832fb-4937-4652-8799-eab6c76d05fb)\*  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem x64](http://www.microsoft.com/downloads/details.aspx?familyid=f58a765f-cea9-456d-b0ab-bfc70b109cbf)\*  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem x64](http://www.microsoft.com/downloads/details.aspx?familyid=9e2c95f6-9381-4484-b11b-814ab9138118)\*\*  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem x64](http://www.microsoft.com/downloads/details.aspx?familyid=d417ebce-7841-4bbb-8abc-b15ef5f4b733)\*  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem x64](http://www.microsoft.com/downloads/details.aspx?familyid=b823a7aa-0eb9-42dd-bf56-8907d94b314a)\*\*  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem x64](http://www.microsoft.com/downloads/details.aspx?familyid=d7307afd-84a0-434e-9658-bf9f8ae4b938)\*  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem x64](http://www.microsoft.com/downloads/details.aspx?familyid=39b7abc7-65a4-4dfd-92ba-c638e3de1118)\*  
(Vysoký)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 pro systémy s procesorem Itanium
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=c26de145-94b8-404a-b946-744988fab83b)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=a21d061a-794a-4012-b3cd-c67445c074f5)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=3ad64d5c-2d81-4ac8-934e-8917b2fcf961)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=13a9f838-ac07-43dc-9aee-a77207998e1e)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=cb4211f3-1082-4245-8f03-7cbac90e9a31)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=7eeac1bb-9f86-4ea5-b30f-980d52be5044)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=66b2506d-80e0-4e32-86e6-0908ef56ae90)  
(Vysoký)
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

 
**Poznámky k systémům Windows Server 2008 a Windows Server 2008 R2**

**\*Instalace Server Core obsahující chybu zabezpečení.** Tato aktualizace se stejným hodnocením závažnosti se vztahuje k podporovaným edicím systému Windows Server 2008 nebo Windows Server 2008 R2, jak je uvedeno, s instalací pomocí volby pro instalaci Server Core nebo bez ní. Další informace o této možnosti instalace naleznete v článcích na webu TechNet [Managing a Server Core Installation](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) (Správa instalace Server Core) a [Servicing a Server Core Installation](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx) (Obsluha instalace Server Core). Možnost instalace Server Core se nevztahuje na určité edice systému Windows Server 2008 a Windows Server 2008 R2; další informace naleznete v části [Porovnání možností instalace Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**\*\*Instalace Server Core není touto chybou ovlivněna.** Chyby zabezpečení, které tato aktualizace řeší, nemají vliv na podporované edice systému Windows Server 2008 nebo Windows Server 2008 R2, jak je uvedeno, v případě instalace s využitím možnosti instalace Server Core. Další informace o této možnosti instalace naleznete v článcích na webu TechNet [Managing a Server Core Installation](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) (Správa instalace Server Core) a [Servicing a Server Core Installation](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx) (Obsluha instalace Server Core). Možnost instalace Server Core se nevztahuje na určité edice systému Windows Server 2008 a Windows Server 2008 R2; další informace naleznete v části [Porovnání možností instalace Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**Poznámka k bulletinu MS10-093**

<sup>[1]</sup>Windows Movie Maker 2.6 je volitelná položka ke stažení, kterou lze nainstalovat ve vyznačených operačních systémech.

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
Sady Microsoft Office a jejich komponenty
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS10-103**](http://go.microsoft.com/fwlink/?linkid=198156)
</td>
<td style="border:1px solid black;">
[**MS10-105**](http://go.microsoft.com/fwlink/?linkid=147425)
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
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Publisher 2002 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=f540692c-e404-4383-8937-4d6a36475da5)  
(KB2284692)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Microsoft Office XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=724d0ad6-ba5f-4dbf-b280-3fb36335d33b)<sup>[1]</sup>
(KB2289162)  
(Vysoký)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2003 Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Publisher 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=e600de65-3e9d-4e37-8906-8b7091ff523e)  
(KB2284695)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=976857e9-77fc-4667-88ca-7637e57536cd)<sup>[1]</sup>
(KB2289163)  
(Vysoký)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2007 Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft Publisher 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=79275011-bdc1-446a-8ea6-56fc31bd9c35)  
(KB2284697)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=676eeed6-f2b7-4265-afc7-a82ffdbeb290)  
(KB2288931)  
(Stupeň závažnosti není určen<sup>[2]</sup>)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2010 (32bitové edice)
</td>
<td style="border:1px solid black;">
[Microsoft Publisher 2010 (32bitové edice)](http://www.microsoft.com/downloads/details.aspx?familyid=99e18990-75e9-497e-9b4f-5d7ef8656ab2)  
(KB2409055)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2010 (32bitové edice)](http://www.microsoft.com/downloads/details.aspx?familyid=6d644494-b530-4b37-bc37-8a8a7edefe53)  
(KB2289078)  
(Stupeň závažnosti není určen<sup>[2]</sup>)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2010 (64bitové edice)
</td>
<td style="border:1px solid black;">
[Microsoft Publisher 2010 (64bitové edice)](http://www.microsoft.com/downloads/details.aspx?familyid=9b27ee11-e563-4152-9691-25eec1ee9966)  
(KB2409055)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2010 (64bitové edice)](http://www.microsoft.com/downloads/details.aspx?familyid=58e54779-aa8f-41b3-9993-8cec12c49082)  
(KB2289078)  
(Stupeň závažnosti není určen<sup>[2]</sup>)
</td>
</tr>
<tr>
<th colspan="3" style="border:1px solid black;">
Jiný software systému Office
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS10-103**](http://go.microsoft.com/fwlink/?linkid=198156)
</td>
<td style="border:1px solid black;">
[**MS10-105**](http://go.microsoft.com/fwlink/?linkid=147425)
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
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office Converter Pack
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Microsoft Office Converter Pack](http://www.microsoft.com/downloads/details.aspx?familyid=dcded2ee-0673-4afe-abe6-04941a2ad306)  
(KB2456849)  
(Vysoký)
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
[Microsoft Works 9](http://www.microsoft.com/downloads/details.aspx?familyid=10f6f330-05d8-4b60-9ebb-822a7321ac0f)  
(KB2431831)  
(Vysoký)
</td>
</tr>
</table>
<p></p>

 
**Poznámky k bulletinu MS10-105**

<sup>[1]</sup>Zákazníci používající uvedený software by si měli také nainstalovat aktualizaci systému Microsoft Office uvedenou v bulletinu MS10-087, která jim zajistí ochranu před chybami zabezpečení popsanými v bulletinu MS10-105.

<sup>[2]</sup>U této aktualizace není určen stupeň závažnosti, neboť chyby zabezpečení uvedené v tomto bulletinu se netýkají tohoto softwaru. Nicméně v rámci zvýšení ochrany proti eventuálním dalším útokům doporučuje společnost Microsoft uživatelům tohoto softwaru tuto aktualizaci zabezpečení použít.

#### Microsoft Server Software

 
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
Microsoft SharePoint Server
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS10-104**](http://go.microsoft.com/fwlink/?linkid=206469)
</td>
<td style="border:1px solid black;">
[**MS10-106**](http://go.microsoft.com/fwlink/?linkid=204624)
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
Žádné
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office SharePoint Server 007 Service Pack 2 (32bitové edice)
</td>
<td style="border:1px solid black;">
[Microsoft Office SharePoint Server 2007 Service Pack 2 (32bitové edice)](http://www.microsoft.com/downloads/details.aspx?familyid=3c8fb9f9-7920-43ea-b618-e26dc3360c60)  
(KB2433089)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office SharePoint Server 2007 Service Pack 2 (64bitové edice)
</td>
<td style="border:1px solid black;">
[Microsoft Office SharePoint Server 2007 Service Pack 2 (64bitové edice)](http://www.microsoft.com/downloads/details.aspx?familyid=3db09280-24bd-42e0-9ae3-02c9bf3e8ee3)  
(KB2433089)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
</tr>
<tr>
<th colspan="3" style="border:1px solid black;">
Microsoft Exchange Server
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS10-104**](http://go.microsoft.com/fwlink/?linkid=206469)
</td>
<td style="border:1px solid black;">
[**MS10-106**](http://go.microsoft.com/fwlink/?linkid=204624)
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
[**Mírný**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Exchange Server 2007 Service Pack 2 pro systémy s procesorem x64
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Microsoft Exchange Server 2007 Service Pack 2 pro systémy s procesorem x64](http://www.microsoft.com/downloads/details.aspx?familyid=7b983156-9e9f-4d29-9e9b-2369747e3b62)  
(KB2407132)  
(Mírný)
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

**Doporučené postupy zjišťování a nasazení**

Společnost Microsoft poskytuje doporučené postupy zjišťování a nasazení aktualizací zabezpečení. Tyto dokumenty obsahují doporučení a informace, které mohou odborníkům v oblasti IT pomoci porozumět, jak se používají různé nástroje pro detekci a nasazení aktualizací zabezpečení. Další informace získáte v [článku 961747 znalostní báze Microsoft Knowledge Base](http://support.microsoft.com/kb/961747).

**Nástroj Microsoft Baseline Security Analyzer**

Pomocí nástroje Microsoft Baseline Security Analyzer (MBSA) mohou správci prohledávat místní i vzdálené systémy a zjistit tak, jestli v nich nechybí některé aktualizace zabezpečení nebo jestli v nastavení zabezpečení systému nedošlo k některým běžným chybám. Další informace o nástroji MBSA získáte na webu [Microsoft Baseline Security Analyzer](http://go.microsoft.com/fwlink/?linkid=21134).

**Služba Windows Server Update Services**

Pomocí služby Windows Server Update Services (WSUS) mohou správci systémů rychle a spolehlivě nasadit nejnovější důležité aktualizace zabezpečení pro systémy Microsoft Windows 2000 a novější, systém Office XP a novější, Exchange Server 2003 a SQL Server 2000 do systémů Microsoft Windows 2000 a novějších.

Další informace o způsobu instalace této aktualizace zabezpečení pomocí služby Windows Server Update Services získáte na webu služby [Windows Server Update Services](http://go.microsoft.com/fwlink/?linkid=50120).

**SystemCenter** **Configuration Manager 2007**

Služba Software Update Management nástroje Configuration Manager 2007 zjednodušuje složitý proces doručení a správy aktualizací do IT systémů firmy. Pomocí nástroje Configuration Manager 2007 mohou správci informačních technologií doručit aktualizace produktů společnosti Microsoft do řady zařízení, včetně stolních počítačů, notebooků, serverů a mobilních zařízení.

Automatizované hodnocení chyb zabezpečení v nástroji Configuration Manager 2007 odhaluje potřebu aktualizací a hlášení doporučených postupů. Základem služby Software Update Management nástroje Configuration Manager 2007 jsou služby WSUS (Microsoft Windows Software Update Services). Jedná se o časem prověřenou infrastrukturu aktualizací známou správcům informačních technologií po celém světě. Další informace o tom, jak mohou správci používat nástroj Configuration Manager 2007 k nasazení aktualizací, naleznete na webových stránkách [Software Update Management](http://www.microsoft.com/systemcenter/en/us/configuration-manager/cm-software-update-management.aspx). Další informace o nástroji Configuration Manager naleznete na webových stránkách [System Center Configuration Manager](http://www.microsoft.com/systemcenter/en/us/configuration-manager.aspx).

**Systems Management Server 2003**

Microsoft Systems Management Server (SMS) představuje v rozlehlých sítích řešení pro správu aktualizací s rozsáhlými možnostmi konfigurace. Umožňuje správcům identifikovat počítače se systémem Windows, které vyžadují aktualizace zabezpečení, a provést řízenou instalaci těchto aktualizací v celé rozlehlé síti s minimálním dopadem na koncové uživatele.

**Poznámka:** Systems Management Server 2003 není od 12. ledna 2010 součástí tradiční podpory. Další informace o životním cyklu produktů naleznete na webu [Životní cyklus podpory produktů společnosti Microsoft](http://support.microsoft.com/common/international.aspx?rdpath=dm;en-us;lifecycle). K dispozici je nyní nová verze nástroje SMS - System Center Configuration Manager 2007 (viz výše uvedená část **SystemCenter** **Configuration Manager 2007**.

Další informace o tom, jak mohou správci pomocí serveru SMS 2003 nasazovat aktualizace zabezpečení, naleznete na webových stránkách [Scénáře a postupy pro Microsoft Systems Management Server 2003: Distribuce softwaru a správa oprav](http://www.microsoft.com/downloads/en/details.aspx?familyid=32f2bb4c-42f8-4b8d-844f-2553fd78049f&displaylang=en). Další informace o serveru SMS naleznete na webových stránkách [Microsoft Systems Management Server TechCenter](http://technet.microsoft.com/en-us/systemcenter/bb545936.aspx).

**Poznámka:** Služba SMS pomocí modulu Microsoft Baseline Security Analyzer poskytuje rozsáhlou podporu při zjišťování a nasazení aktualizací bulletinu zabezpečení. Tyto nástroje nemusí některé softwarové aktualizace zjistit. V takovém případě mohou správci použít funkce serveru SMS a nasměrovat aktualizace do určitých systémů. Další informace o tomto postupu najdete na webu [Nasazení aktualizací softwaru pomocí funkce Distribuce softwaru serveru SMS](http://go.microsoft.com/fwlink/?linkid=33341). Některé aktualizace zabezpečení vyžadují po restartování počítače oprávnění správce. Správci mohou k instalaci těchto aktualizací použít nástroj Elevated Rights Deployment Tool (k dispozici v sadě [SMS 2003 Administration Feature Pack](http://www.microsoft.com/downloads/en/details.aspx?familyid=7bd3a16e-1899-4e0b-bb99-1320e816167d&displaylang=en)).

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

-   Uživateli s pseudonymem Aniway ze společnosti [VeriSign iDefense Labs](http://labs.idefense.com/) za oznámení chyby popsané v bulletinu MS10-090.
-   Nicolasi Jolymu ze skupiny [VUPEN Vulnerability Research Team](http://www.vupen.com/) za oznámení chyby popsané v bulletinu MS10-090.
-   Stephenu Fewerovi, spolupracujícímu s organizací [Zero Day Initiative](http://www.zerodayinitiative.com/) společnosti [Tipping Point](http://www.tippingpoint.com/), za oznámení chyby popsané v bulletinu MS10-090.
-   [Peteru Vreugdenhilovi](http://vreugdenhilresearch.nl/), spolupracujícímu s organizací [Zero Day Initiative](http://www.zerodayinitiative.com/) společnosti [TippingPoint](http://www.tippingpoint.com/), za oznámení chyby popsané v bulletinu MS10-090.
-   Masatoshi Satovi ze společnosti [AZIA CO., LTD.](http://www.azia.jp) za oznámení chyby popsané v bulletinu MS10-090.
-   [Yosukemu Hasegawovi](http://utf-8.jp/) za spolupráci na řešení chyby popsané v bulletinu MS10-090.
-   Jose Antoniu Vazquez Gonzalezovi ze společnosti [Verisign iDefense Labs](http://labs.idefense.com/) za oznámení chyby popsané v bulletinu MS10-090.
-   Marcu Schoenefeldovi ze skupiny [Red Hat Security Response Team](https://www.redhat.com/security/team/), spolupracujímu se skupinou [Opera Security Team](http://www.opera.com/security/), za oznámení chyby popsané v bulletinu MS10-091.
-   Marcu Schoenefeldovi ze skupiny [Red Hat Security Response Team](https://www.redhat.com/security/team/) za oznámení chyby popsané v bulletinu MS10-091.
-   Paul-Kenjimu Cahieru Furuyaovi za oznámení chyby popsané v bulletinu MS10-091.
-   Sergeji Golovanovi, Alexanderu Gostevovi, Maximu Golovkinovi a Alexeji Monastyrskému ze společnosti [Kaspersky Lab](http://usa.kaspersky.com/) a Vitaliji Kiktenkovi a Alexanderu Saprykinovi ze společnosti [Design and Test Lab](http://www.dnt-lab.com/) za oznámení chyby popsané v bulletinu MS10-092.
-   Liamu O Murchuovi ze společnosti [Symantec](http://www.symantec.com/index.jsp) za oznámení chyby popsané v bulletinu MS10-092.
-   Alexandru Matrosovovi, Eugene Rodionovovi, Juraji Malchovi a Davidovi Harleymu ze společnosti [ESET](http://www.eset.com/) za oznámení chyby popsané v bulletinu MS10-092.
-   Haifei Liovi z výzkumného týmu [FortiGuard Labs společnosti Fortinet](http://www.fortiguard.com/) za oznámení chyby popsané v bulletinu MS10-095.
-   Simonu Ranerovi ze společnosti [ACROS Security](http://www.acrossecurity.com/) za oznámení chyby popsané v bulletinu MS10-096.
-   HD Mooreovi ze společnosti [Rapid7](http://www.rapid7.com/) za oznámení chyby popsané v bulletinu MS10-096.
-   Muhaiminu Dzulfakarovi ze společnosti [NGS Software](http://www.ngssoftware.com/) za oznámení chyby popsané v bulletinu MS10-096.
-   Muhaiminu Dzulfakarovi ze společnosti [NGS Software](http://www.ngssoftware.com/) za oznámení chyby popsané v bulletinu MS10-097.
-   Tarjei Mandtovi ze společnosti [Norman](http://www.norman.com/) za oznámení čtyř chyb popsaných v bulletinu MS10-098.
-   Stéfanovi Le Berremu ze společnosti [Sysdream](http://www.sysdream.com/) za oznámení chyby popsané v bulletinu MS10-098.
-   Honggangu Renovi z výzkumného týmu [FortiGuard Labs společnosti Fortinet](http://www.fortiguard.com/) za oznámení chyby popsané v bulletinu MS10-099.
-   Cesaru Cerrudovi ze společnosti [Argeniss](http://www.argeniss.com/) za oznámení chyby popsané v bulletinu MS10-100.
-   Matthiasu Dieteru Wallnöferovi a Andrewu Bartlettovi ze skupiny Samba Team za oznámení chyby popsané v bulletinu MS10-101.
-   Společnostem [HP](http://www.hp.com/) a [techit](http://www.techit.de/) za oznámení chyby popsané v bulletinu MS10-102.
-   Chaoukimu Bekrarovi ze skupiny [VUPEN Vulnerability Research Team](http://www.vupen.com/) za oznámení pěti chyb popsaných v bulletinu MS10-103.
-   Oleksandru Miroshovi, spolupracujícímu s organizací [Zero Day Initiative](http://www.zerodayinitiative.com/) společnosti [TippingPoint](http://www.tippingpoint.com/), za oznámení chyby popsané v bulletinu MS10-104.
-   Yamatu Liovi ze společnosti [Palo Alto Networks](http://www.paloaltonetworks.com/) za oznámení dvou chyb popsaných v bulletinu MS10-105.
-   Alinu Radu Popovi ze společnosti [Secunia Research](http://secunia.com/) za oznámení chyby popsané v bulletinu MS10-105.
-   Carstenu Eiramovi ze společnosti [Secunia Research](http://secunia.com/) za oznámení tří chyb popsaných v bulletinu MS10-105.
-   Dyonu Baldingovi ze společnosti [Secunia Research](http://secunia.com/) za oznámení dvou chyb popsaných v bulletinu MS10-105.
-   Oleksandru Miroshovi, spolupracujícímu s organizací [Zero Day Initiative](http://www.zerodayinitiative.com/) společnosti [TippingPoint](http://www.tippingpoint.com/), za oznámení chyby popsané v bulletinu MS10-106.

#### Technická podpora

-   Uvedený software byl testován za účelem zjištění, kterých verzí se chyba týká. U dalších verzí skončila časově omezená podpora. Pokud chcete zjistit dobu, po kterou je pro určitou verzi softwaru poskytována podpora, navštivte web [Zásady poskytování technické podpory pro produkty společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=21742).
-   Zákazníci mohou získat technickou podporu na webu [služby technické podpory společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=21131). Hovory související s aktualizacemi zabezpečení jsou bezplatné. Další informace o dostupných možnostech technické podpory naleznete na webu [Pomoc a podpora společnosti Microsoft](http://support.microsoft.com/).
-   Mezinárodní zákazníci získají podporu u místních zastoupení společnosti Microsoft. Technická podpora související s aktualizacemi zabezpečení je bezplatná. Další informace o možnostech kontaktování společnosti Microsoft v případě potřeby technické podpory získáte na [webu mezinárodní technické podpory](http://go.microsoft.com/fwlink/?linkid=21155).

#### Zřeknutí se záruky

Informace ve znalostní bázi Microsoft Knowledge Base jsou poskytovány tak, jak jsou, bez jakékoli záruky. Společnost Microsoft neposkytuje žádné záruky, výslovně uvedené či mlčky předpokládané, včetně záruk obchodovatelnosti a vhodnosti pro určitý účel. Společnost Microsoft ani její dodavatelé nenesou v žádném případě zodpovědnost za žádné škody, včetně přímých, nepřímých, náhodných či následných škod, ztráty zisku či zvláštních škod, a to ani v případě, že byli na možnost takových škod upozorněni. V některých zemích a právních řádech není dovoleno vyloučit nebo omezit odpovědnost, proto se výše uvedené omezení na vás nemusí vztahovat.

#### Revize

-   V1.0 (14. prosince 2010): Souhrnný bulletin byl publikován.
-   V1.1 (15. prosince 2010): Bylo přidáno objasnění doporučující uživatelům systémů Microsoft Office XP a Microsoft Office 2003 instalaci aktualizace uvedené v bulletinu MS10-087, která jim zajistí ochranu před chybami zabezpečení popsanými v bulletinu MS10-105.

*Built at 2014-04-18T01:50:00Z-07:00*
