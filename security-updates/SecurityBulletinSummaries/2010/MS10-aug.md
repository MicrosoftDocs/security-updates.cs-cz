---
TOCTitle: 'MS10-AUG'
Title: 'Souhrnný bulletin zabezpečení společnosti Microsoft, srpen 2010'
ms:assetid: 'ms10-aug'
ms:contentKeyID: 61223995
ms:mtpsurl: 'https://technet.microsoft.com/cs-CZ/library/ms10-aug(v=Security.10)'
---

Security Bulletin Summary

Souhrnný bulletin zabezpečení společnosti Microsoft, srpen 2010
===============================================================

Publikováno: 2. srpna 2010 | Aktualizováno: 1. září 2010

**Verze:** 2.1

Tento souhrnný bulletin uvádí bulletiny zabezpečení vydané v srpnu 2010.

Spolu s vydáním bulletinů pro srpen 2010 nahrazuje tento souhrnný bulletin předběžné oznámení o bulletinech vydané 5. srpna 2010. Další informace o službě předběžného oznámení o bulletinech naleznete v části [Předběžné oznámení o bulletinech zabezpečení společnosti Microsoft](http://technet.microsoft.com/security/bulletin/advance).

Informace o tom, jak dostávat automatická oznámení o vydání nových bulletinů zabezpečení společnosti Microsoft, naleznete na webu [Zasílání technických oznámení o zabezpečení společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=21163).

Pro zodpovězení zákaznických dotazů týkajících se těchto bulletinů uspořádá společnost Microsoft webové vysílání 11. srpna 2010 v 11:00 časového pásma Tichomoří (USA a Kanada). Zaregistrujte se pro [webové vysílání týkající se srpnových bulletinů zabezpečení](https://msevents.microsoft.com/cui/webcasteventdetails.aspx?eventid=1032454431&eventcategory=4&culture=en-us&countrycode=us). Po tomto datu je webové vysílání dostupné na požádání. Další informace získáte v [souhrnných bulletinech zabezpečení společnosti Microsoft a webovém vysílání](http://technet.microsoft.com/security/bulletin/summary).

Pro mimořádný bulletin zabezpečení [MS10-046](http://go.microsoft.com/fwlink/?linkid=197393), který byl původně oznámen ve verzi 1.0 tohoto souhrnu bulletinů, vydala společnost Microsoft příslušné předběžné oznámení 30. července 2010 a uspořádala webové vysílání 2. srpna 2010. Toto [webové vysílání z 2. srpna 2010](https://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032456779&culture=en-us) je dostupné na požádání. Další informace získáte v [souhrnných bulletinech zabezpečení společnosti Microsoft a webovém vysílání](http://technet.microsoft.com/security/bulletin/summary).

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
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=197393">MS10-046</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení prostředí systému Windows může způsobit vzdálené spuštění kódu (2286198)</strong><br />
<br />
Tato aktualizace zabezpečení řeší veřejně známou chybu zabezpečení v prostředí systému Windows. Chyba zabezpečení může umožnit vzdálené spuštění kódu, pokud dojde k zobrazení ikony speciálně vytvořeného zástupce. Útočník, který by úspěšně zneužil tuto chybu zabezpečení, by mohl získat stejná uživatelská práva, jako má místní uživatel. Uživatelé, jejichž účty jsou konfigurovány tak, aby měli v systému méně uživatelských práv, by byli vystaveni menšímu riziku než uživatelé s uživatelskými právy správce.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritický</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=197104">MS10-049</a></td>
<td style="border:1px solid black;"><strong>Chyby zabezpečení ve zprostředkovateli SChannel umožňují vzdálené spuštění kódu (980436)</strong><br />
<br />
Tato aktualizace zabezpečení řeší jednu veřejně známou a jednu soukromou osobou oznámenou chybu zabezpečení v balíčku zabezpečení Secure Channel (SChannel) v systému Windows. Závažnější chyby zabezpečení mohou umožnit vzdálené spuštění kódu, pokud uživatel navštíví speciálně vytvořený web určený ke zneužití těchto chyb zabezpečení prostřednictvím webového prohlížeče. Útočník však nemůže žádným způsobem přinutit uživatele k návštěvě takových webů. Místo toho by útočník musel přesvědčit uživatele, aby navštívili takový web. K tomu se obvykle používá odkaz v e-mailu nebo ve zprávě v programu pro zasílání rychlých zpráv, na který uživatelé kliknou, a přejdou tak na útočníkův web.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritický</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=196268">MS10-051</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení specifikace Microsoft XML Core Services umožňuje vzdálené spuštění kódu (2079403)</strong><br />
<br />
Tato aktualizace zabezpečení řeší soukromě oznámenou chybu zabezpečení ve specifikaci Microsoft XML Core Services. Tato chyba zabezpečení umožňuje vzdálené spuštění kódu, pokud uživatel zobrazí pomocí aplikace Internet Explorer speciálně vytvořenou webovou stránku. Útočník nemůže žádným způsobem přinutit uživatele k návštěvě takovýchto webů. Místo toho by útočník musel přesvědčit uživatele, aby navštívili takový web. K tomu se obvykle používá odkaz v e-mailu nebo zpráva programu pro zasílání rychlých zpráv, na kterou uživatelé kliknou, a přejdou tak na útočníkův web.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritický</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=194432">MS10-052</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení kodeků Microsoft MPEG Layer-3 umožňuje vzdálené spuštění kódu (2115168)</strong><br />
<br />
Tato aktualizace zabezpečení řeší chybu zabezpečení zvukových kodeků Microsoft MPEG Layer-3 oznámenou soukromou osobou. Tato chyba zabezpečení může umožnit vzdálené spuštění kódu, pokud uživatel otevře speciálně vytvořený mediální soubor nebo obdrží speciálně vytvořený obsah vysílání datového proudu médií z webové stránky nebo jakékoli aplikace poskytující webový obsah. Útočník, který by úspěšně zneužil tuto chybu zabezpečení, by mohl získat stejná uživatelská práva, jako má místní uživatel. Uživatelé, jejichž účty jsou konfigurovány tak, aby měli v systému méně uživatelských práv, by byli vystaveni menšímu riziku než uživatelé s uživatelskými právy správce.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritický</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Může vyžadovat restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=196549">MS10-053</a></td>
<td style="border:1px solid black;"><strong>Kumulativní aktualizace zabezpečení pro aplikaci Internet Explorer (2183461)</strong><br />
<br />
Tato aktualizace zabezpečení řeší šest soukromě oznámených chyb zabezpečení aplikace Internet Explorer. Nejzávažnější chyby zabezpečení mohou umožnit vzdálené spuštění kódu, pokud uživatel pomocí aplikace Internet Explorer zobrazí speciálně vytvořenou webovou stránku. Uživatelé, jejichž účty jsou konfigurovány tak, aby měli v systému méně uživatelských práv, by byli vystaveni menšímu riziku než uživatelé s uživatelskými právy správce.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritický</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows, Internet Explorer</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=190318">MS10-054</a></td>
<td style="border:1px solid black;"><strong>Chyby zabezpečení v serveru SMB umožňují vzdálené spuštění kódu (982214)</strong><br />
<br />
Tato aktualizace zabezpečení řeší několik chyb zabezpečení v systému Microsoft Windows oznámených soukromými osobami. Nejzávažnější z těchto chyb zabezpečení by mohla umožnit vzdálené spuštění kódu v případě, že by útočník vytvořil speciálně vytvořený paket SMB a odeslal jej do postiženého systému. Doporučené postupy pro používání brány firewall a standardní konfigurace této brány zajišťují ochranu sítí před útoky pocházejícími z oblasti mimo rozlehlou síť, které by se pokusily zneužít tyto chyby zabezpečení.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritický</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=194906">MS10-055</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení v kodeku Cinepak umožňuje vzdálené spuštění kódu (982665)</strong><br />
<br />
Tato aktualizace zabezpečení řeší chybu zabezpečení v kodeku Cinepak, kterou oznámila soukromá osoba. Tato chyba zabezpečení může umožnit vzdálené spuštění kódu, pokud uživatel otevře speciálně vytvořený mediální soubor nebo obdrží speciálně vytvořený obsah vysílání datového proudu médií z webové stránky nebo jakékoli aplikace poskytující webový obsah. Útočník, který by úspěšně zneužil tuto chybu zabezpečení, by mohl získat stejná uživatelská práva, jako má místní uživatel. Uživatelé, jejichž účty jsou konfigurovány tak, aby měli v systému méně uživatelských práv, by byli vystaveni menšímu riziku než uživatelé s uživatelskými právy správce.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritický</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Může vyžadovat restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=196938">MS10-056</a></td>
<td style="border:1px solid black;"><strong>Chyby zabezpečení v aplikaci Microsoft Office Word umožňují vzdálené spuštění kódu (2269638)</strong><br />
<br />
Tato aktualizace zabezpečení řeší čtyři soukromými osobami oznámené chyby zabezpečení v systému Microsoft Office. Nejzávažnější chyby zabezpečení mohou umožnit vzdálené spuštění kódu, pokud uživatel otevře speciálně vytvořenou e-mailovou zprávu ve formátu RTF nebo zobrazí její náhled. Útočník, který by úspěšně zneužil některou z těchto chyb zabezpečení, by mohl získat stejná uživatelská práva, jaká má místní uživatel. Uživatelé, jejichž účty jsou konfigurovány tak, aby měli v systému méně uživatelských práv, by byli vystaveni menšímu riziku než uživatelé s uživatelskými právy správce.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritický</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Může vyžadovat restartování</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=179830">MS10-060</a></td>
<td style="border:1px solid black;"><strong>Chyby zabezpečení ve společném jazykovém modulu runtime rozhraní Microsoft .NET a v programu Microsoft Silverlight umožňují vzdálené spuštění kódu (2265906)</strong><br />
<br />
Tato aktualizace zabezpečení řeší dvě soukromými osobami oznámené chyby zabezpečení rozhraní Microsoft .NET Framework a programu Microsoft Silverlight. Tyto chyby zabezpečení by mohly umožnit vzdálené spuštění kódu v klientském systému, pokud by uživatel zobrazil speciálně vytvořenou webovou stránku pomocí webového prohlížeče, v němž lze otevírat aplikace prohlížeče XAML (XBAP) nebo aplikace Silverlight, popř. pokud by útočník přesvědčil uživatele, aby spustil speciálně vytvořenou aplikaci Microsoft .NET. Uživatelé, jejichž účty jsou konfigurovány tak, aby měli v systému méně uživatelských práv, by byli vystaveni menšímu riziku než uživatelé s uživatelskými právy správce. Chyby zabezpečení dále mohou umožnit vzdálené spuštění kódu na serverovém systému se službou IIS v případě, že tento server umožňuje zpracování stránek ASP.NET a útočníkovi se úspěšně podaří na daném serveru načíst speciálně vytvořenou stránku ASP.NET a spustit ji, jako například v případě hostování webu.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritický</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Může vyžadovat restartování</td>
<td style="border:1px solid black;">Microsoft Windows, Microsoft .NET Framework, Microsoft Silverlight</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=195812">MS10-047</a></td>
<td style="border:1px solid black;"><strong>Chyby zabezpečení jádra systému Windows umožňují zvýšení oprávnění (981852)</strong><br />
<br />
Tato aktualizace zabezpečení řeší několik chyb zabezpečení v systému Microsoft Windows oznámených soukromými osobami. Nejzávažnější z těchto chyb zabezpečení by mohla umožnit zvýšení úrovně oprávnění, pokud by se útočník místně přihlásil k systému a spustil speciálně vytvořenou aplikaci. Tyto chyby zabezpečení může zneužít pouze útočník s platnými pověřeními pro přihlášení, která by mu umožňovala se místně přihlásit. Uvedené chyby zabezpečení nemohou zneužít vzdálení ani anonymní uživatelé.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Vysoký</a><br />
Zvýšení úrovně oprávnění</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=194552">MS10-048</a></td>
<td style="border:1px solid black;"><strong>Chyby zabezpečení v ovladačích režimu jádra systému Windows umožňují zvýšení úrovně oprávnění (2160329)</strong><br />
<br />
Tato aktualizace zabezpečení řeší jednu veřejně známou a čtyři soukromou osobou oznámené chyby zabezpečení ovladačů režimu jádra systému Windows. Nejzávažnější z těchto chyb zabezpečení by mohla způsobit zvýšení úrovně oprávnění, pokud by se útočník přihlásil k postiženému systému a spustil speciálně vytvořenou aplikaci. Tuto chybu může zneužít pouze útočník s platnými pověřeními pro přihlášení, která by mu umožňovala se místně přihlásit. Tuto chybu zabezpečení nemohou zneužít vzdálení ani anonymní uživatelé.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Vysoký</a><br />
Zvýšení úrovně oprávnění</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=197103">MS10-050</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení v programu Windows Movie Maker umožňuje vzdálené spuštění kódu (981997)</strong><br />
<br />
Tato aktualizace zabezpečení řeší chybu zabezpečení v programu Windows Movie Maker, kterou oznámila soukromá osoba. Tato chyba zabezpečení může umožnit vzdálené spuštění kódu, pokud útočník odešle speciálně vytvořený soubor projektu programu Movie Maker a přesvědčí uživatele k jeho otevření. Uživatelé, jejichž účty jsou konfigurovány tak, aby měli v systému méně uživatelských práv, by byli vystaveni menšímu riziku než uživatelé s uživatelskými právy správce.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Vysoký</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Může vyžadovat restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=196275">MS10-057</a></td>
<td style="border:1px solid black;"><strong>Chyba zabezpečení v aplikaci Microsoft Office Excel umožňuje vzdálené spuštění kódu (2269707)</strong><br />
<br />
Tato aktualizace zabezpečení řeší chybu zabezpečení v sadě Microsoft Office, kterou oznámila soukromá osoba. Tato chyba umožňuje vzdálené spuštění kódu, pokud uživatel otevře speciálně vytvořený soubor aplikace Excel. Útočník, který by úspěšně zneužil tuto chybu zabezpečení, by mohl získat stejná uživatelská práva, jaká má přihlášený uživatel. Uživatelé, jejichž účty jsou konfigurovány tak, aby měli v systému méně uživatelských práv, by byli vystaveni menšímu riziku než uživatelé s uživatelskými právy správce.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Vysoký</a><br />
Vzdálené spuštění kódu</td>
<td style="border:1px solid black;">Může vyžadovat restartování</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=194562">MS10-058</a></td>
<td style="border:1px solid black;"><strong>Chyby zabezpečení v protokolu TCP/IP umožňují zvýšení úrovně oprávnění (978886)</strong><br />
<br />
Tato aktualizace zabezpečení řeší dvě soukromými osobami oznámené chyby zabezpečení v systému Microsoft Windows. Závažnější z těchto chyb zabezpečení by mohla umožnit zvýšení úrovně oprávnění z důvodu chyby ve zpracování konkrétní vstupní vyrovnávací paměti. Útočník s možností přihlášení do cílového systému by mohl tuto chybu zabezpečení zneužít a spustit libovolný kód s oprávněními na úrovni systému. Útočník by tak mohl instalovat programy, zobrazovat, měnit či odstraňovat data nebo vytvářet nové účty s úplnými uživatelskými právy.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Vysoký</a><br />
Zvýšení úrovně oprávnění</td>
<td style="border:1px solid black;">Vyžaduje restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=196444">MS10-059</a></td>
<td style="border:1px solid black;"><strong>Chyby zabezpečení ve funkci pro trasování služeb mohou způsobit zvýšení úrovně oprávnění (982799)</strong><br />
<br />
Tato aktualizace zabezpečení řeší jednu veřejně známou a jednu soukromou osobou oznámenou chybu zabezpečení ve funkci pro trasování služeb. Tyto chyby zabezpečení umožňují zvýšení úrovně oprávnění, pokud útočník spustí speciálně vytvořenou aplikaci. Tuto chybu může zneužít pouze útočník s platnými pověřeními pro přihlášení, která by mu umožňovala se místně přihlásit. Tuto chybu zabezpečení nemohou zneužít vzdálení ani anonymní uživatelé.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Vysoký</a><br />
Zvýšení úrovně oprávnění</td>
<td style="border:1px solid black;">Může vyžadovat restartování</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
</tbody>
</table>
<p></p>
  
Index zneužitelnosti  
--------------------
  
 
Následující tabulka uvádí hodnocení zneužitelnosti každé chyby zabezpečení uvedené v tomto měsíci. Chyby zabezpečení jsou řazeny v pořadí zmenšující se úrovně posouzení zneužitelnosti, jinak než tomu je u řazení podle čísla chyb. Uvedeny jsou pouze chyby zabezpečení ohodnocené stupněm závažnosti Kritický nebo Vysoký.
  
**Jak pracovat s touto tabulkou**
  
V této tabulce zjistíte, jaká je pravděpodobnost vydání funkčního zneužitelného kódu během 30 dní od vydání tohoto bulletinu zabezpečení pro všechny aktualizace zabezpečení, které bude třeba nainstalovat. Všechna níže uvedená hodnocení zvažte na základě vaší specifické konfigurace a podle závěrů hodnocení nastavte priority pro zavádění jednotlivých aktualizací. Další informace o významu těchto hodnocení a způsobu jejich stanovení najdete v indexu zneužitelnosti [Microsoft Exploitability Index](http://technet.microsoft.com/en-us/security/cc998259.aspx).
  
| ID bulletinu                                              | Název chyby zabezpečení                                                                                                                   | ID CVE                                                                           | Hodnocení indexu zneužitelnosti                                                                                                | Hlavní poznámky                                                                                                                                                                                                        |  
|-----------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| [MS10-060](http://go.microsoft.com/fwlink/?linkid=179830) | Chyba zabezpečení týkající se poškození paměti programu Microsoft Silverlight                                                             | [CVE-2010-0019](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0019) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní zneužití kódu je pravděpodobné               | (Žádné)                                                                                                                                                                                                                |  
| [MS10-052](http://go.microsoft.com/fwlink/?linkid=194432) | Chyba zabezpečení týkající se přetečení vyrovnávací paměti zvukového dekodéru MPEG Layer-3                                                | [CVE-2010-1882](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-1882) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní zneužití kódu je pravděpodobné               | (Žádné)                                                                                                                                                                                                                |  
| [MS10-047](http://go.microsoft.com/fwlink/?linkid=195812) | Chyba zabezpečení jádra systému Windows týkající se inicializace dat                                                                      | [CVE-2010-1888](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-1888) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní zneužití kódu je pravděpodobné               | (Žádné)                                                                                                                                                                                                                |  
| [MS10-058](http://go.microsoft.com/fwlink/?linkid=194562) | Chyba zabezpečení týkající se přetečení celého čísla v síti Windows                                                                       | [CVE-2010-1893](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-1893) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní zneužití kódu je pravděpodobné               | (Žádné)                                                                                                                                                                                                                |  
| [MS10-048](http://go.microsoft.com/fwlink/?linkid=194552) | Chyba zabezpečení týkající se zpracování výjimek subsystému Win32k                                                                        | [CVE-2010-1894](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-1894) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní zneužití kódu je pravděpodobné               | **Tato chyba zabezpečení je veřejně známá.**                                                                                                                                                                           |  
| [MS10-048](http://go.microsoft.com/fwlink/?linkid=194552) | Chyba zabezpečení týkající se přetečení fondu subsystému Win32k                                                                           | [CVE-2010-1895](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-1895) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní zneužití kódu je pravděpodobné               | (Žádné)                                                                                                                                                                                                                |  
| [MS10-048](http://go.microsoft.com/fwlink/?linkid=194552) | Chyba zabezpečení týkající se ověřování vstupu uživatele subsystému Win32k                                                                | [CVE-2010-1896](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-1896) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní zneužití kódu je pravděpodobné               | (Žádné)                                                                                                                                                                                                                |  
| [MS10-048](http://go.microsoft.com/fwlink/?linkid=194552) | Chyba zabezpečení při vytváření oken subsystému Win32k                                                                                    | [CVE-2010-1897](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-1897) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní zneužití kódu je pravděpodobné               | (Žádné)                                                                                                                                                                                                                |  
| [MS10-060](http://go.microsoft.com/fwlink/?linkid=179830) | Chyba zabezpečení týkající se delegování virtuální metody jazyka CLR v programu Microsoft Silverlight a rozhraní Microsoft .NET Framework | [CVE-2010-1898](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-1898) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní zneužití kódu je pravděpodobné               | (Žádné)                                                                                                                                                                                                                |  
| [MS10-056](http://go.microsoft.com/fwlink/?linkid=196938) | Chyba zabezpečení při analýze záznamu v aplikaci Word                                                                                     | [CVE-2010-1900](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-1900) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní zneužití kódu je pravděpodobné               | (Žádné)                                                                                                                                                                                                                |  
| [MS10-056](http://go.microsoft.com/fwlink/?linkid=196938) | Chyba zabezpečení týkající se poškození paměti modulu pro analýzu formátu RTF aplikace Word                                               | [CVE-2010-1901](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-1901) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní zneužití kódu je pravděpodobné               | (Žádné)                                                                                                                                                                                                                |  
| [MS10-055](http://go.microsoft.com/fwlink/?linkid=194906) | Chyba zabezpečení při dekompresi kodeku Cinepak                                                                                           | [CVE-2010-2553](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2553) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní zneužití kódu je pravděpodobné               | (Žádné)                                                                                                                                                                                                                |  
| [MS10-059](http://go.microsoft.com/fwlink/?linkid=196444) | Chyba zabezpečení týkající se poškození paměti při trasování                                                                              | [CVE-2010-2555](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2555) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní zneužití kódu je pravděpodobné               | (Žádné)                                                                                                                                                                                                                |  
| [MS10-053](http://go.microsoft.com/fwlink/?linkid=196549) | Chyba zabezpečení týkající se poškození neinicializované paměti                                                                           | [CVE-2010-2557](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2557) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní zneužití kódu je pravděpodobné               | Tato chyba zabezpečení je z důvodu chybějící funkce Zabránění spuštění dat nejsnáze zneužitelná v aplikaci Internet Explorer 6.                                                                                        |  
| [MS10-053](http://go.microsoft.com/fwlink/?linkid=196549) | Chyba zabezpečení týkající se poškození paměti při rozložení prvků ve formátu HTML                                                        | [CVE-2010-2560](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2560) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní zneužití kódu je pravděpodobné               | (Žádné)                                                                                                                                                                                                                |  
| [MS10-057](http://go.microsoft.com/fwlink/?linkid=196275) | Chyba zabezpečení týkající se poškození paměti aplikace Excel                                                                             | [CVE-2010-2562](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2562) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní zneužití kódu je pravděpodobné               | (Žádné)                                                                                                                                                                                                                |  
| [MS10-050](http://go.microsoft.com/fwlink/?linkid=197103) | Chyba zabezpečení týkající se poškození paměti v programu Movie Maker                                                                     | [CVE-2010-2564](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2564) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní zneužití kódu je pravděpodobné               | (Žádné)                                                                                                                                                                                                                |  
| [MS10-046](http://go.microsoft.com/fwlink/?linkid=197393) | Chyba zabezpečení týkající se načtení ikony zástupce                                                                                      | [CVE-2010-2568](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2568) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Konsistentní zneužití kódu je pravděpodobné               | **V současné době dochází ke zneužití této chyby zabezpečení v prostředí Internetu.**                                                                                                                                  |  
| [MS10-047](http://go.microsoft.com/fwlink/?linkid=195812) | Chyba zabezpečení týkající se dvojitého uvolnění jádra systému Windows                                                                    | [CVE-2010-1889](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-1889) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Nekonsistentní zneužití kódu je pravděpodobné             | (Žádné)                                                                                                                                                                                                                |  
| [MS10-056](http://go.microsoft.com/fwlink/?linkid=196938) | Chyba zabezpečení týkající se přetečení vyrovnávací paměti při analýze formátu RTF aplikace Word                                          | [CVE-2010-1902](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-1902) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Nekonsistentní zneužití kódu je pravděpodobné             | Z důvodu dodatečného omezení haldy je menší pravděpodobnost zneužití u systémů Windows Vista a Windows 7.                                                                                                              |  
| [MS10-056](http://go.microsoft.com/fwlink/?linkid=196938) | Chyba zabezpečení týkající se poškození paměti propojených objektů HTML aplikace Word                                                     | [CVE-2010-1903](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-1903) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Nekonsistentní zneužití kódu je pravděpodobné             | (Žádné)                                                                                                                                                                                                                |  
| [MS10-054](http://go.microsoft.com/fwlink/?linkid=190318) | Chyba zabezpečení týkající se přetečení fondu protokolu SMB                                                                               | [CVE-2010-2550](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2550) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Nekonsistentní zneužití kódu je pravděpodobné             | Zneužití spíše povede k odmítnutí služby než spuštění kódu.                                                                                                                                                            |  
| [MS10-053](http://go.microsoft.com/fwlink/?linkid=196549) | Chyba zabezpečení týkající se poškození neinicializované paměti                                                                           | [CVE-2010-2556](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2556) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Nekonsistentní zneužití kódu je pravděpodobné             | (Žádné)                                                                                                                                                                                                                |  
| [MS10-053](http://go.microsoft.com/fwlink/?linkid=196549) | Chyba zabezpečení týkající se poškození paměti konfliktu časování                                                                         | [CVE-2010-2558](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2558) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Nekonsistentní zneužití kódu je pravděpodobné             | (Žádné)                                                                                                                                                                                                                |  
| [MS10-053](http://go.microsoft.com/fwlink/?linkid=196549) | Chyba zabezpečení týkající se poškození neinicializované paměti                                                                           | [CVE-2010-2559](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2559) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Nekonsistentní zneužití kódu je pravděpodobné             | (Žádné)                                                                                                                                                                                                                |  
| [MS10-051](http://go.microsoft.com/fwlink/?linkid=196268) | Chyba zabezpečení týkající se poškození paměti při zpracování odpovědi na chybu Msxml2.XMLHTTP.3.0                                        | [CVE-2010-2561](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2561) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Nekonsistentní zneužití kódu je pravděpodobné             | (Žádné)                                                                                                                                                                                                                |  
| [MS10-049](http://go.microsoft.com/fwlink/?linkid=197104) | Chyba zabezpečení umožňující vzdálené spuštění kódu při požadavku chybně formátovaného certifikátu zprostředkovatele SChannel             | [CVE-2010-2566](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2566) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Nekonsistentní zneužití kódu je pravděpodobné             | Zneužití nejspíše povede k odmítnutí služby. Vzdálené spuštění kódu je nepravděpodobné.                                                                                                                                |  
| [MS10-049](http://go.microsoft.com/fwlink/?linkid=197104) | Chyba zabezpečení týkající se opětovného vyjednávání protokolu TLS/SSL                                                                    | [CVE-2009-3555](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-3555) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Vytvoření funkčního zneužitelného kódu není pravděpodobné | Jedná se o chybu zabezpečení umožňující vkládání falešného obsahu. Tato chyba byla popsána v [Informačním zpravodaji zabezpečení společnosti Microsoft 977377](http://technet.microsoft.com/security/advisory/977377). |  
| [MS10-053](http://go.microsoft.com/fwlink/?linkid=196549) | Chyba zabezpečení týkající se zpracování událostí při přechodu mezi doménami                                                              | [CVE-2010-1258](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-1258) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Vytvoření funkčního zneužitelného kódu není pravděpodobné | Jedná se o chybu zabezpečení typu zpřístupnění informací.                                                                                                                                                              |  
| [MS10-058](http://go.microsoft.com/fwlink/?linkid=194562) | Chyba zabezpečení týkající se poškození paměti protokolu IPv6                                                                             | [CVE-2010-1892](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-1892) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Vytvoření funkčního zneužitelného kódu není pravděpodobné | Jedná se o chybu zabezpečení, která způsobuje odmítnutí služby (DoS).                                                                                                                                                  |  
| [MS10-054](http://go.microsoft.com/fwlink/?linkid=190318) | Chyba zabezpečení týkající se ověřování proměnné protokolu SMB                                                                            | [CVE-2010-2551](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2551) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Vytvoření funkčního zneužitelného kódu není pravděpodobné | Jedná se o chybu zabezpečení, která způsobuje odmítnutí služby (DoS).                                                                                                                                                  |  
| [MS10-054](http://go.microsoft.com/fwlink/?linkid=190318) | Chyba zabezpečení týkající se vyčerpání zásobníku protokolu SMB                                                                           | [CVE-2010-2552](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2552) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Vytvoření funkčního zneužitelného kódu není pravděpodobné | Jedná se o chybu zabezpečení, která způsobuje odmítnutí služby (DoS).                                                                                                                                                  |
  
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
[**MS10-046**](http://go.microsoft.com/fwlink/?linkid=197393)
</td>
<td style="border:1px solid black;">
[**MS10-049**](http://go.microsoft.com/fwlink/?linkid=197104)
</td>
<td style="border:1px solid black;">
[**MS10-051**](http://go.microsoft.com/fwlink/?linkid=196268)
</td>
<td style="border:1px solid black;">
[**MS10-052**](http://go.microsoft.com/fwlink/?linkid=194432)
</td>
<td style="border:1px solid black;">
[**MS10-053**](http://go.microsoft.com/fwlink/?linkid=196549)
</td>
<td style="border:1px solid black;">
[**MS10-054**](http://go.microsoft.com/fwlink/?linkid=190318)
</td>
<td style="border:1px solid black;">
[**MS10-055**](http://go.microsoft.com/fwlink/?linkid=194906)
</td>
<td style="border:1px solid black;">
[**MS10-060**](http://go.microsoft.com/fwlink/?linkid=179830)
</td>
<td style="border:1px solid black;">
[**MS10-047**](http://go.microsoft.com/fwlink/?linkid=195812)
</td>
<td style="border:1px solid black;">
[**MS10-048**](http://go.microsoft.com/fwlink/?linkid=194552)
</td>
<td style="border:1px solid black;">
[**MS10-050**](http://go.microsoft.com/fwlink/?linkid=197103)
</td>
<td style="border:1px solid black;">
[**MS10-058**](http://go.microsoft.com/fwlink/?linkid=194562)
</td>
<td style="border:1px solid black;">
[**MS10-059**](http://go.microsoft.com/fwlink/?linkid=196444)
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
Žádné
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=12361875-b453-45e8-852b-90f2727894fd)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=ff00381c-e74b-48e5-9dd9-34dbedd906a2)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Microsoft XML Core Services 3.0](http://www.microsoft.com/downloads/details.aspx?familyid=dbdbbe5e-2ef9-4704-80c4-27ef28fd95ef)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=08159149-17de-4640-8818-cb7bd4811531)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=bc949915-4e16-4897-a295-2f99102548ab)  
(Kritický)  
[Aplikace Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=4b489f8c-ada0-4051-8284-0a941c04d2ed)  
(Kritický)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=1662780f-370a-425b-9917-c601eb54a375)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=6e5e16f8-c140-4a1d-b898-8417a6bfd4d8)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=5ddb5e34-f97a-47c6-96c8-ba2ed06ccb77)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=648cfca5-19eb-4658-a6ad-fe546c4c44b9)  
(KB983582)  
(Kritický)  
[Microsoft .NET Framework 2.0 Service Pack 2 a Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=1e53f250-2d4b-4f61-86ee-9f9f3a9c0b48)  
(KB983583)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=e3574047-5ce5-4461-94aa-4eb3258d5e71)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=deeac521-d3a2-4019-8176-c9228e733cf4)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Movie Maker 2.1](http://www.microsoft.com/downloads/details.aspx?familyid=b211664b-434d-4626-816f-c77510cfd44d)<sup>[1]</sup>
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
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3b44bd67-48e2-497f-9165-42a702e2cc0d)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=eaffa70c-6f2b-4e66-b1bc-64bdbbbcd34f)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Microsoft XML Core Services 3.0](http://www.microsoft.com/downloads/details.aspx?familyid=4d4e8eeb-a0b2-41c6-9ee4-3f4beb44195e)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b7f28d7a-6b27-4059-865b-5fd55edb6299)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=96b7a562-af16-4f0d-840c-838fb12e7419)  
(Kritický)  
[Aplikace Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=5296fb82-c446-4681-a9a0-0f80a2e248be)  
(Kritický)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=f8ae3978-bad6-4201-8357-2d212ab703ef)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=fd6cc359-e72e-46ec-a08b-763934e3e115)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/my%20documents/release/5cff5d6e-11a5-40ed-92ac-e12d287919e6)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=648cfca5-19eb-4658-a6ad-fe546c4c44b9)  
(KB983582)  
(Kritický)  
[Microsoft .NET Framework 2.0 Service Pack 2 a Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=1e53f250-2d4b-4f61-86ee-9f9f3a9c0b48)  
(KB983583)  
(Kritický)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d6c5455e-bc31-4842-aef4-ebff92324323)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Movie Maker 2.1](http://www.microsoft.com/downloads/details.aspx?familyid=decb1fe6-adc8-44f7-89c5-f25767f0cefe)<sup>[1]</sup>
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
Windows Server 2003
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS10-046**](http://go.microsoft.com/fwlink/?linkid=197393)
</td>
<td style="border:1px solid black;">
[**MS10-049**](http://go.microsoft.com/fwlink/?linkid=197104)
</td>
<td style="border:1px solid black;">
[**MS10-051**](http://go.microsoft.com/fwlink/?linkid=196268)
</td>
<td style="border:1px solid black;">
[**MS10-052**](http://go.microsoft.com/fwlink/?linkid=194432)
</td>
<td style="border:1px solid black;">
[**MS10-053**](http://go.microsoft.com/fwlink/?linkid=196549)
</td>
<td style="border:1px solid black;">
[**MS10-054**](http://go.microsoft.com/fwlink/?linkid=190318)
</td>
<td style="border:1px solid black;">
[**MS10-055**](http://go.microsoft.com/fwlink/?linkid=194906)
</td>
<td style="border:1px solid black;">
[**MS10-060**](http://go.microsoft.com/fwlink/?linkid=179830)
</td>
<td style="border:1px solid black;">
[**MS10-047**](http://go.microsoft.com/fwlink/?linkid=195812)
</td>
<td style="border:1px solid black;">
[**MS10-048**](http://go.microsoft.com/fwlink/?linkid=194552)
</td>
<td style="border:1px solid black;">
[**MS10-050**](http://go.microsoft.com/fwlink/?linkid=197103)
</td>
<td style="border:1px solid black;">
[**MS10-058**](http://go.microsoft.com/fwlink/?linkid=194562)
</td>
<td style="border:1px solid black;">
[**MS10-059**](http://go.microsoft.com/fwlink/?linkid=196444)
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
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=32fe91ef-5a8d-4095-90ee-2ca216696b09)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=f76d68df-97e5-489c-a5f6-0c378c1f62ae)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Microsoft XML Core Services 3.0](http://www.microsoft.com/downloads/details.aspx?familyid=31ce233e-4d2d-404b-84a8-683319ba8ef7)  
(Mírný)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=9c2110ec-7e6c-4e73-9785-0a8196095ea0)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=b0370e1e-dedf-4fe8-a06c-0e0f0a674205)  
(Kritický)  
[Aplikace Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=8753ae27-60a4-475a-b8bc-6a7764480295)  
(Kritický)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=772e765d-0502-4b0b-bde8-d4f62b96db64)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=230e8559-e6df-49d5-acb5-b0cd4bde0bf4)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=648cfca5-19eb-4658-a6ad-fe546c4c44b9)  
(KB983582)  
(Kritický)  
[Microsoft .NET Framework 2.0 Service Pack 2 a Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=1e53f250-2d4b-4f61-86ee-9f9f3a9c0b48)  
(KB983583)  
(Kritický)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=59395f00-90f4-4b68-8dd3-03ff611c1bc8)  
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
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=923de214-c4fa-41e6-8307-2c5a37f13e8e)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4543bcf0-3505-407b-a5a9-6250ece6fbac)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Microsoft XML Core Services 3.0](http://www.microsoft.com/downloads/details.aspx?familyid=4d784b57-8564-4e7e-8f61-f897398e7ea5)  
(Mírný)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=fdfad4ca-37c4-4ac5-bebc-a5ad61299503)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=d92f5e69-43cf-4615-aa3b-41f9f40bb57b)  
(Kritický)  
[Aplikace Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=fd3e9d06-1f8b-4ef7-84f6-61e85a1767b8)  
(Kritický)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=863edf45-0d3b-4408-a47c-258dc4a4fd94)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=03804f59-748e-4832-98e4-2d88564bd10a)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=648cfca5-19eb-4658-a6ad-fe546c4c44b9)  
(KB983582)  
(Kritický)  
[Microsoft .NET Framework 2.0 Service Pack 2 a Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=1e53f250-2d4b-4f61-86ee-9f9f3a9c0b48)  
(KB983583)  
(Kritický)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=9ef1c600-bb93-4800-81b8-8c64b369c194)  
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
<td style="border:1px solid black;">
Windows Server 2003 SP2 pro systémy s procesorem Itanium
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=63aa5f8a-fe47-4892-b905-b54e4f3b6580)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=9ef992c3-96e9-4533-b844-07424a6054b3)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Microsoft XML Core Services 3.0](http://www.microsoft.com/downloads/details.aspx?familyid=d87ac8b3-41fb-4cdd-b305-181a0024d85c)  
(Mírný)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=782e2963-4a52-4a1d-b99a-34ba841038a7)  
(Kritický)  
[Aplikace Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=5e730064-8270-4d63-b497-c5ebeddea1fc)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=e4f4f8b3-7a39-4d77-a46b-02c86ad159c3)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=648cfca5-19eb-4658-a6ad-fe546c4c44b9)  
(KB983582)  
(Kritický)  
[Microsoft .NET Framework 2.0 Service Pack 2 a Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=1e53f250-2d4b-4f61-86ee-9f9f3a9c0b48)  
(KB983583)  
(Kritický)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=f96b8154-9976-41b0-b9d7-d79887fe9364)  
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
Windows Vista
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS10-046**](http://go.microsoft.com/fwlink/?linkid=197393)
</td>
<td style="border:1px solid black;">
[**MS10-049**](http://go.microsoft.com/fwlink/?linkid=197104)
</td>
<td style="border:1px solid black;">
[**MS10-051**](http://go.microsoft.com/fwlink/?linkid=196268)
</td>
<td style="border:1px solid black;">
[**MS10-052**](http://go.microsoft.com/fwlink/?linkid=194432)
</td>
<td style="border:1px solid black;">
[**MS10-053**](http://go.microsoft.com/fwlink/?linkid=196549)
</td>
<td style="border:1px solid black;">
[**MS10-054**](http://go.microsoft.com/fwlink/?linkid=190318)
</td>
<td style="border:1px solid black;">
[**MS10-055**](http://go.microsoft.com/fwlink/?linkid=194906)
</td>
<td style="border:1px solid black;">
[**MS10-060**](http://go.microsoft.com/fwlink/?linkid=179830)
</td>
<td style="border:1px solid black;">
[**MS10-047**](http://go.microsoft.com/fwlink/?linkid=195812)
</td>
<td style="border:1px solid black;">
[**MS10-048**](http://go.microsoft.com/fwlink/?linkid=194552)
</td>
<td style="border:1px solid black;">
[**MS10-050**](http://go.microsoft.com/fwlink/?linkid=197103)
</td>
<td style="border:1px solid black;">
[**MS10-058**](http://go.microsoft.com/fwlink/?linkid=194562)
</td>
<td style="border:1px solid black;">
[**MS10-059**](http://go.microsoft.com/fwlink/?linkid=196444)
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
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
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
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista Service Pack 1 a Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 a Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=52748886-6280-4247-8cbd-f64db229ee66)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 a Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=aca69406-f795-4398-968f-959fe3a74e89)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Microsoft XML Core Services 3.0](http://www.microsoft.com/downloads/details.aspx?familyid=bbfaadf8-ab38-456c-956a-ea18c64236c9)  
(Kritický)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=535c563e-cdac-4e3d-96b0-9947ea22deca)  
(Kritický)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=2062566b-8b81-43c2-875d-9c06d4e3fa82)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 a Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=9087a3aa-aa55-41f6-8c4c-f322e4aa8681)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 a Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=60c81415-b61e-44a4-8dd9-cedec99eb70f)  
(Kritický)
</td>
<td style="border:1px solid black;">
Pouze Windows Vista Service Pack 1:  
[Microsoft .NET Framework 2.0 Service Pack 1 a Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=616c39f7-137a-40b9-b691-bc33c0aef7e1)  
(KB983587)  
(Kritický)  
Pouze Windows Vista Service Pack 1:  
[Microsoft .NET Framework 2.0 Service Pack 2 a Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=155bbb5c-247e-4bed-a287-527d978b7967)  
(KB983588)  
(Kritický)  
Pouze Windows Vista Service Pack 2:  
[Microsoft .NET Framework 2.0 Service Pack 2 a Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=7712e8ad-dea4-4a43-8a7b-dc154510c104)  
(KB983589)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 a Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4486f97c-4cf8-4236-bfc3-b50e72e2a5c1)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 a Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c9345207-7242-4b71-bf80-b52031e08f8c)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Movie Maker 6.0](http://www.microsoft.com/downloads/details.aspx?familyid=8aded9dd-08d6-4b19-955f-0d8414868cf9)<sup>[1]</sup>
(Vysoký)  
[Movie Maker 2.6](http://www.microsoft.com/downloads/details.aspx?familyid=a1d8ed0d-a3b5-416a-ab8b-77501da62132)<sup>[2]</sup>
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 a Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4684c4df-0a5c-4dba-82e5-059378737118)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 a Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=dfb31aa2-7457-4581-9e28-7984a360edf4)  
(Vysoký)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 1 a Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 a Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=37648e95-05c2-4802-9a0f-660200baa229)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 a Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e2835ed1-5ca6-4347-8ff1-e694b1ac49ff)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Microsoft XML Core Services 3.0](http://www.microsoft.com/downloads/details.aspx?familyid=577131cd-1229-4746-89d7-84d75f29e1f0)  
(Kritický)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=cd1185e3-ca22-4197-a53b-e7a2806ac352)  
(Kritický)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=65b04e29-8e39-46de-94e8-b653969b1ffd)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 a Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=10c9d5f1-53ed-459b-a663-e69bdb845a6b)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 a Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=469b732d-ca62-4a48-bb55-99f2ae4ddcf5)  
(Kritický)
</td>
<td style="border:1px solid black;">
Pouze Windows Vista x64 Edition Service Pack 1:  
[Microsoft .NET Framework 2.0 Service Pack 1 a Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=616c39f7-137a-40b9-b691-bc33c0aef7e1)  
(KB983587)  
(Kritický)  
Pouze Windows Vista x64 Edition Service Pack 1:  
[Microsoft .NET Framework 2.0 Service Pack 2 a Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=155bbb5c-247e-4bed-a287-527d978b7967)  
(KB983588)  
(Kritický)  
Pouze Windows Vista x64 Edition Service Pack 2:  
[Microsoft .NET Framework 2.0 Service Pack 2 a Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=7712e8ad-dea4-4a43-8a7b-dc154510c104)  
(KB983589)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 a Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b547898e-f8a9-49dc-b49d-cffec5a001bc)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 a Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=1620e7ac-3913-478d-8120-e9f46d98f453)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Movie Maker 6.0](http://www.microsoft.com/downloads/details.aspx?familyid=4baff9ae-dd25-4942-b45e-f281d0e1f4ac)<sup>[1]</sup>
(Vysoký)  
[Movie Maker 2.6](http://www.microsoft.com/downloads/details.aspx?familyid=0a226592-8f98-4f67-ac60-1d00cbc56598)<sup>[2]</sup>
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 a Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=18152cd4-815f-425f-8694-fbabcbe80609)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 a Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=110f932f-d13c-4486-a295-e6068d5d8d7a)  
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
[**MS10-046**](http://go.microsoft.com/fwlink/?linkid=197393)
</td>
<td style="border:1px solid black;">
[**MS10-049**](http://go.microsoft.com/fwlink/?linkid=197104)
</td>
<td style="border:1px solid black;">
[**MS10-051**](http://go.microsoft.com/fwlink/?linkid=196268)
</td>
<td style="border:1px solid black;">
[**MS10-052**](http://go.microsoft.com/fwlink/?linkid=194432)
</td>
<td style="border:1px solid black;">
[**MS10-053**](http://go.microsoft.com/fwlink/?linkid=196549)
</td>
<td style="border:1px solid black;">
[**MS10-054**](http://go.microsoft.com/fwlink/?linkid=190318)
</td>
<td style="border:1px solid black;">
[**MS10-055**](http://go.microsoft.com/fwlink/?linkid=194906)
</td>
<td style="border:1px solid black;">
[**MS10-060**](http://go.microsoft.com/fwlink/?linkid=179830)
</td>
<td style="border:1px solid black;">
[**MS10-047**](http://go.microsoft.com/fwlink/?linkid=195812)
</td>
<td style="border:1px solid black;">
[**MS10-048**](http://go.microsoft.com/fwlink/?linkid=194552)
</td>
<td style="border:1px solid black;">
[**MS10-050**](http://go.microsoft.com/fwlink/?linkid=197103)
</td>
<td style="border:1px solid black;">
[**MS10-058**](http://go.microsoft.com/fwlink/?linkid=194562)
</td>
<td style="border:1px solid black;">
[**MS10-059**](http://go.microsoft.com/fwlink/?linkid=196444)
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
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Mírný**](http://go.microsoft.com/fwlink/?linkid=21140)
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
Žádné
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
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 pro 32bitové systémy a Windows Server 2008 pro 32bitové systémy Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro 32bitové systémy a Windows Server 2008 pro 32bitové systémy Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3aabd189-7d4c-4c9f-8854-f33127b1c309)\*  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro 32bitové systémy a Windows Server 2008 pro 32bitové systémy Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=6e0253d4-f0c0-4f28-ba08-6907c2fcb339)\*  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Microsoft XML Core Services 3.0](http://www.microsoft.com/downloads/details.aspx?familyid=73b5f45c-c9d6-491f-8483-98838b2a7c04)\*  
(Mírný)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=8239cb9e-bb5a-4157-8038-33d0b329eaee)\*\*  
(Kritický)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=409b9298-1e7d-48cf-9872-ffbdc56ebe53)\*\*  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro 32bitové systémy a Windows Server 2008 pro 32bitové systémy Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=a94e2e38-116a-4b63-9328-6c33e63bbbfe)\*  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Pouze systém Windows Server 2008 pro 32bitové systémy  
[Microsoft .NET Framework 2.0 Service Pack 1 a Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=616c39f7-137a-40b9-b691-bc33c0aef7e1)\*\*  
(KB983587)  
(Kritický)  
Pouze systém Windows Server 2008 pro 32bitové systémy  
[Microsoft .NET Framework 2.0 Service Pack 2 a Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=155bbb5c-247e-4bed-a287-527d978b7967)\*\*  
(KB983588)  
(Kritický)  
Pouze Windows Server 2008 pro 32bitové systémy s aktualizací Service Pack 2:  
[Microsoft .NET Framework 2.0 Service Pack 2 a Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=7712e8ad-dea4-4a43-8a7b-dc154510c104)\*\*  
(KB983589)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro 32bitové systémy a Windows Server 2008 pro 32bitové systémy Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=611765ab-b3f3-45db-92b2-ee040b9cfd27)\*  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro 32bitové systémy a Windows Server 2008 pro 32bitové systémy Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=a8b1a3f7-7147-494e-bfc0-b1979b9578e6)\*  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro 32bitové systémy a Windows Server 2008 pro 32bitové systémy Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=844404be-f2e8-47bc-9650-9e2bbe383814)\*  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro 32bitové systémy a Windows Server 2008 pro 32bitové systémy Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4c9b3e60-e166-40c9-8938-3cba0a399c47)\*  
(Vysoký)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 pro systémy s procesorem x64 a Windows Server 2008 pro systémy s procesorem x64 Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem x64 a Windows Server 2008 pro systémy s procesorem x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=29c6fc2d-d318-4a63-9ab2-82e84272aaf2)\*  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem x64 a Windows Server 2008 pro systémy s procesorem x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=a96891ff-8771-47b3-81bb-8640adb6c098)\*  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Microsoft XML Core Services 3.0](http://www.microsoft.com/downloads/details.aspx?familyid=43ece408-4aa7-4819-b3f6-7f0719ed3213)\*  
(Mírný)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=5ef8abf0-c89e-4911-8d77-42400d9a398f)\*\*  
(Kritický)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=9b869bab-0797-4f83-8c64-23dda9983c8d)\*\*  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem x64 a Windows Server 2008 pro systémy s procesorem x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=602dd3f6-0d09-4546-b1db-d7b6b04edb66)\*  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Pouze systém Windows Server 2008 pro systémy s procesorem x64:  
[Microsoft .NET Framework 2.0 Service Pack 1 a Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=616c39f7-137a-40b9-b691-bc33c0aef7e1)\*\*  
(KB983587)  
(Kritický)  
Pouze systém Windows Server 2008 pro systémy s procesorem x64:  
[Microsoft .NET Framework 2.0 Service Pack 2 a Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=155bbb5c-247e-4bed-a287-527d978b7967)\*\*  
(KB983588)  
(Kritický)  
Pouze Windows Server 2008 pro systémy s procesorem x64 s aktualizací Service Pack 2:  
[Microsoft .NET Framework 2.0 Service Pack 2 a Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=7712e8ad-dea4-4a43-8a7b-dc154510c104)\*\*  
(KB983589)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem x64 a Windows Server 2008 pro systémy s procesorem x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=131f3512-1585-462e-a4f1-3f359aac44bd)\*  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem x64 a Windows Server 2008 pro systémy s procesorem x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c1c25cb7-7e82-4c14-9666-aff52dd308b4)\*  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem x64 a Windows Server 2008 pro systémy s procesorem x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=08491c73-66b1-4c4c-8740-ea596a730fc1)\*  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem x64 a Windows Server 2008 pro systémy s procesorem x64 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=fa84e547-2190-402f-9467-2450deeff565)\*  
(Vysoký)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 pro systémy s procesorem Itanium a Windows Server 2008 pro systémy s procesorem Itanium Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem Itanium a Windows Server 2008 pro systémy s procesorem Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=cfe227b5-6660-49f8-9d71-a997dd83de0b)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem Itanium a Windows Server 2008 pro systémy s procesorem Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3b16a422-0ee9-4eab-9cfe-e7688ffa0d76)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Microsoft XML Core Services 3.0](http://www.microsoft.com/downloads/details.aspx?familyid=b6faee94-e821-432d-bfa2-9008664566af)  
(Mírný)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=2f1eee63-2cca-4ec5-b196-36de3c0054cf)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem Itanium a Windows Server 2008 pro systémy s procesorem Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=24d8f0a3-51a9-46c1-b870-a2239bf600e4)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Pouze systém Windows Server 2008 pro systémy s procesorem Itanium:  
[Microsoft .NET Framework 2.0 Service Pack 1 a Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=616c39f7-137a-40b9-b691-bc33c0aef7e1)  
(KB983587)  
(Kritický)  
Pouze systém Windows Server 2008 pro systémy s procesorem Itanium:  
[Microsoft .NET Framework 2.0 Service Pack 2 a Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=155bbb5c-247e-4bed-a287-527d978b7967)  
(KB983588)  
(Kritický)  
Pouze Windows Server 2008 pro systémy s procesorem Itanium s aktualizací Service Pack 2:  
[Microsoft .NET Framework 2.0 Service Pack 2 a Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=7712e8ad-dea4-4a43-8a7b-dc154510c104)  
(KB983589)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem Itanium a Windows Server 2008 pro systémy s procesorem Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=972efd3a-ec1e-49b2-835e-76f4b21b5b79)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem Itanium a Windows Server 2008 pro systémy s procesorem Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=45fe5135-aa89-4f60-8cdb-ec0edc9a7e77)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem Itanium a Windows Server 2008 pro systémy s procesorem Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8aa12902-c234-4fd9-bba3-6767eafc38fc)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem Itanium a Windows Server 2008 pro systémy s procesorem Itanium Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=84f89dca-108c-4956-9aa2-866e17a872fc)  
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
[**MS10-046**](http://go.microsoft.com/fwlink/?linkid=197393)
</td>
<td style="border:1px solid black;">
[**MS10-049**](http://go.microsoft.com/fwlink/?linkid=197104)
</td>
<td style="border:1px solid black;">
[**MS10-051**](http://go.microsoft.com/fwlink/?linkid=196268)
</td>
<td style="border:1px solid black;">
[**MS10-052**](http://go.microsoft.com/fwlink/?linkid=194432)
</td>
<td style="border:1px solid black;">
[**MS10-053**](http://go.microsoft.com/fwlink/?linkid=196549)
</td>
<td style="border:1px solid black;">
[**MS10-054**](http://go.microsoft.com/fwlink/?linkid=190318)
</td>
<td style="border:1px solid black;">
[**MS10-055**](http://go.microsoft.com/fwlink/?linkid=194906)
</td>
<td style="border:1px solid black;">
[**MS10-060**](http://go.microsoft.com/fwlink/?linkid=179830)
</td>
<td style="border:1px solid black;">
[**MS10-047**](http://go.microsoft.com/fwlink/?linkid=195812)
</td>
<td style="border:1px solid black;">
[**MS10-048**](http://go.microsoft.com/fwlink/?linkid=194552)
</td>
<td style="border:1px solid black;">
[**MS10-050**](http://go.microsoft.com/fwlink/?linkid=197103)
</td>
<td style="border:1px solid black;">
[**MS10-058**](http://go.microsoft.com/fwlink/?linkid=194562)
</td>
<td style="border:1px solid black;">
[**MS10-059**](http://go.microsoft.com/fwlink/?linkid=196444)
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
Žádné
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
Windows 7 pro 32bitové systémy
</td>
<td style="border:1px solid black;">
[Windows 7 pro 32bitové systémy](http://www.microsoft.com/downloads/details.aspx?familyid=22e62b5c-e4c1-47d0-ae4a-8bd2d70d0a0a)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows 7 pro 32bitové systémy](http://www.microsoft.com/downloads/details.aspx?familyid=71716507-7080-4102-991e-6afc7cc377d5)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Microsoft XML Core Services 3.0](http://www.microsoft.com/downloads/details.aspx?familyid=31d0f5ac-2cff-42a1-8f18-128bbfc4e57d)  
(Kritický)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=ecaf42e0-a288-40c1-8602-21e967a87408)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows 7 pro 32bitové systémy](http://www.microsoft.com/downloads/details.aspx?familyid=8d58ebc4-a5f9-4318-a6f1-168c1bcdae3c)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows 7 pro 32bitové systémy](http://www.microsoft.com/downloads/details.aspx?familyid=2e782ac9-b5d5-490e-a01a-7d4481eab224)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=77d0c428-237c-4dab-9645-6400dd9e65f8)  
(KB983590)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows 7 pro 32bitové systémy](http://www.microsoft.com/downloads/details.aspx?familyid=a7d60864-5942-47ed-a6f3-1c07b4833a14)  
(Mírný)
</td>
<td style="border:1px solid black;">
[Windows 7 pro 32bitové systémy](http://www.microsoft.com/downloads/details.aspx?familyid=68bddf4b-b597-477e-80e4-9293d7160496)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows 7 pro 32bitové systémy](http://www.microsoft.com/downloads/details.aspx?familyid=3a5a088e-644a-4a0e-9a09-0370bcd97688)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows 7 pro 32bitové systémy](http://www.microsoft.com/downloads/details.aspx?familyid=ce6233f3-2ee5-4329-908d-ba9b28ecc553)  
(Vysoký)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 7 pro systémy s procesorem x64
</td>
<td style="border:1px solid black;">
[Windows 7 pro systémy s procesorem x64](http://www.microsoft.com/downloads/details.aspx?familyid=9499f771-c388-4de3-a5c7-8cc8b00b4395)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows 7 pro systémy s procesorem x64](http://www.microsoft.com/downloads/details.aspx?familyid=c457d8ec-83b7-446f-b77c-e47d4187e616)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Microsoft XML Core Services 3.0](http://www.microsoft.com/downloads/details.aspx?familyid=a4f6d7c2-b475-4900-82f0-75f5be0b7b63)  
(Kritický)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=ca57a47a-9111-4abe-9356-4962ca2c1d65)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows 7 pro systémy s procesorem x64](http://www.microsoft.com/downloads/details.aspx?familyid=ad1ddf94-d714-4b36-8256-42bf79d03a90)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows 7 pro systémy s procesorem x64](http://www.microsoft.com/downloads/details.aspx?familyid=24751193-592f-4c44-a8d6-f4112d4f011b)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=77d0c428-237c-4dab-9645-6400dd9e65f8)  
(KB983590)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows 7 pro systémy s procesorem x64](http://www.microsoft.com/downloads/details.aspx?familyid=b00ec47c-402e-4207-a4c9-6c1900f254f8)  
(Mírný)
</td>
<td style="border:1px solid black;">
[Windows 7 pro systémy s procesorem x64](http://www.microsoft.com/downloads/details.aspx?familyid=5ff09e03-d662-4b23-ab26-d25ca2ba58df)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows 7 pro systémy s procesorem x64](http://www.microsoft.com/downloads/details.aspx?familyid=163fe2bd-f999-47c1-9a35-c4fc868bda51)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows 7 pro systémy s procesorem x64](http://www.microsoft.com/downloads/details.aspx?familyid=146270fa-cd6f-440a-aa3e-e93af0bff447)  
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
[**MS10-046**](http://go.microsoft.com/fwlink/?linkid=197393)
</td>
<td style="border:1px solid black;">
[**MS10-049**](http://go.microsoft.com/fwlink/?linkid=197104)
</td>
<td style="border:1px solid black;">
[**MS10-051**](http://go.microsoft.com/fwlink/?linkid=196268)
</td>
<td style="border:1px solid black;">
[**MS10-052**](http://go.microsoft.com/fwlink/?linkid=194432)
</td>
<td style="border:1px solid black;">
[**MS10-053**](http://go.microsoft.com/fwlink/?linkid=196549)
</td>
<td style="border:1px solid black;">
[**MS10-054**](http://go.microsoft.com/fwlink/?linkid=190318)
</td>
<td style="border:1px solid black;">
[**MS10-055**](http://go.microsoft.com/fwlink/?linkid=194906)
</td>
<td style="border:1px solid black;">
[**MS10-060**](http://go.microsoft.com/fwlink/?linkid=179830)
</td>
<td style="border:1px solid black;">
[**MS10-047**](http://go.microsoft.com/fwlink/?linkid=195812)
</td>
<td style="border:1px solid black;">
[**MS10-048**](http://go.microsoft.com/fwlink/?linkid=194552)
</td>
<td style="border:1px solid black;">
[**MS10-050**](http://go.microsoft.com/fwlink/?linkid=197103)
</td>
<td style="border:1px solid black;">
[**MS10-058**](http://go.microsoft.com/fwlink/?linkid=194562)
</td>
<td style="border:1px solid black;">
[**MS10-059**](http://go.microsoft.com/fwlink/?linkid=196444)
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
[**Mírný**](http://go.microsoft.com/fwlink/?linkid=21140)
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
Žádné
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
Žádné
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
[Windows Server 2008 R2 pro systémy s procesorem x64](http://www.microsoft.com/downloads/details.aspx?familyid=0d9dd09b-db40-462b-88b0-4dbb8180e81f)\*  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem x64](http://www.microsoft.com/downloads/details.aspx?familyid=c9aeea25-ca14-4b42-9018-a27c9d8899c4)\*  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Microsoft XML Core Services 3.0](http://www.microsoft.com/downloads/details.aspx?familyid=a48cdac5-4d78-49b5-a6d8-ecf6c58cace2)\*  
(Mírný)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=e7757bbc-3ef0-421d-ab57-0083a302c77b)\*\*  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem x64](http://www.microsoft.com/downloads/details.aspx?familyid=52642a8d-1081-4496-848e-9b03baf3fdac)\*  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=77d0c428-237c-4dab-9645-6400dd9e65f8)\*  
(KB983590)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem x64](http://www.microsoft.com/downloads/details.aspx?familyid=c1ad1248-07f1-42d4-baa4-8a20837ec7b4)\*  
(Mírný)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem x64](http://www.microsoft.com/downloads/details.aspx?familyid=6bbc9cb1-0b59-4473-adf9-2ce2f0f94c0a)\*  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem x64](http://www.microsoft.com/downloads/details.aspx?familyid=a1f95600-34e5-44b3-b2cb-b2b2cbf645cb)\*  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem x64](http://www.microsoft.com/downloads/details.aspx?familyid=333fb6e4-f867-4dcb-beb3-2d88e428ca2e)\*  
(Vysoký)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 pro systémy s procesorem Itanium
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=ce2bb5d4-f661-44e3-ac28-0b81f7b72670)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=b7c2e91f-ca8a-4237-99c8-ca53c91cf73e)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Microsoft XML Core Services 3.0](http://www.microsoft.com/downloads/details.aspx?familyid=b4d3210e-f3ad-4dbb-9390-6e98eeb99eaa)  
(Mírný)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=7b457d04-03a9-4eb0-ba6a-ab45267e4f74)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=783fb42c-3698-4b1d-a692-3ff319578931)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=77d0c428-237c-4dab-9645-6400dd9e65f8)  
(KB983590)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=f23dec0f-a33b-4d8c-a86d-0e9368ae7ff5)  
(Mírný)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=2543191a-09cb-4417-bbb2-aac4d9a2a756)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=c3cd7f2f-e198-4fbd-a65d-21a1bf51eb61)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=62034ecb-a6bd-46c5-a03d-9642880bc2d6)  
(Vysoký)
</td>
</tr>
</table>
<p></p>
 
**Poznámky k systémům Windows Server 2008 a Windows Server 2008 R2**

**\*Instalace Server Core obsahující chybu zabezpečení.** Tato aktualizace se stejným hodnocením závažnosti se vztahuje k podporovaným edicím systému Windows Server 2008 nebo Windows Server 2008 R2, jak je uvedeno, s instalací pomocí volby pro instalaci Server Core nebo bez ní. Další informace o této možnosti instalace naleznete v článcích na webu TechNet [Managing a Server Core Installation](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) (Správa instalace Server Core) a [Servicing a Server Core Installation](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx) (Obsluha instalace Server Core). Možnost instalace Server Core se nevztahuje na určité edice systému Windows Server 2008 a Windows Server 2008 R2; další informace naleznete v části [Porovnání možností instalace Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**\*\*Instalace Server Core není touto chybou ovlivněna.** Chyby zabezpečení, které tato aktualizace řeší, nemají vliv na podporované edice systému Windows Server 2008 nebo Windows Server 2008 R2, jak je uvedeno, v případě instalace s využitím možnosti instalace Server Core. Další informace o této možnosti instalace naleznete v článcích na webu TechNet [Managing a Server Core Installation](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) (Správa instalace Server Core) a [Servicing a Server Core Installation](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx) (Obsluha instalace Server Core). Možnost instalace Server Core se nevztahuje na určité edice systému Windows Server 2008 a Windows Server 2008 R2; další informace naleznete v části [Porovnání možností instalace Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**Poznámky k bulletinu MS10-050**

<sup>[1]</sup>Tyto verze programu Windows Movie Maker jsou dodávány s vyznačenými operačními systémy.

<sup>[2]</sup>Windows Movie Maker 2.6 je volitelná položka ke stažení, kterou lze nainstalovat ve vyznačených operačních systémech.

**Poznámka k bulletinu MS10-060**

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
[**MS10-056**](http://go.microsoft.com/fwlink/?linkid=196938)
</td>
<td style="border:1px solid black;">
[**MS10-057**](http://go.microsoft.com/fwlink/?linkid=196275)
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
Microsoft Office XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Office Word 2002 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=978eb887-25b6-4dde-a2ec-d2d1e7f1a434)  
(KB2251389)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel 2002 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=032e1530-8736-4e1c-a704-967679227619)  
(KB2264397)  
(Vysoký)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2003 Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Office Word 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=4360bcec-0731-4d4a-89eb-7d28a4607f06)  
(KB2251399)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=7cecbce3-bbb7-47d1-bda3-64d7e0f69f62)  
(KB2264403)  
(Vysoký)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Systém Microsoft Office 2007 Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft Office Word 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=0d7210a3-662e-41e7-affc-ae94f9d89388)<sup>[1]</sup>
(KB2251419)  
(Kritický)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
</tr>
<tr>
<th colspan="3" style="border:1px solid black;">
Microsoft Office for Mac
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS10-056**](http://go.microsoft.com/fwlink/?linkid=196938)
</td>
<td style="border:1px solid black;">
[**MS10-057**](http://go.microsoft.com/fwlink/?linkid=196275)
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
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2004 for Mac
</td>
<td style="border:1px solid black;">
[Microsoft Office 2004 for Mac](http://www.microsoft.com/downloads/details.aspx?familyid=d2f44d4a-7cd8-4514-b3ff-1770bc47d595)  
(KB2284171)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2004 for Mac](http://www.microsoft.com/downloads/details.aspx?familyid=d2f44d4a-7cd8-4514-b3ff-1770bc47d595)  
(KB2284171)  
(Vysoký)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2008 for Mac
</td>
<td style="border:1px solid black;">
[Microsoft Office 2008 for Mac](http://www.microsoft.com/downloads/details.aspx?familyid=6ece112f-0ca7-4b1f-ad20-603950edee66)  
(KB2284162)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2008 for Mac](http://www.microsoft.com/downloads/details.aspx?familyid=6ece112f-0ca7-4b1f-ad20-603950edee66)  
(KB2284162)  
(Vysoký)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Otevření nástroje XML File Format Converter for Mac
</td>
<td style="border:1px solid black;">
[Otevření nástroje XML File Format Converter for Mac](http://www.microsoft.com/downloads/details.aspx?familyid=a7b834a3-5a44-42d4-afe9-6ef207333834)  
(KB2284179)  
(Vysoký)
</td>
<td style="border:1px solid black;">
[Otevření nástroje XML File Format Converter for Mac](http://www.microsoft.com/downloads/details.aspx?familyid=a7b834a3-5a44-42d4-afe9-6ef207333834)  
(KB2284179)  
(Vysoký)
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
[**MS10-056**](http://go.microsoft.com/fwlink/?linkid=196938)
</td>
<td style="border:1px solid black;">
[**MS10-057**](http://go.microsoft.com/fwlink/?linkid=196275)
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
Microsoft Office Word Viewer
</td>
<td style="border:1px solid black;">
[Microsoft Office Word Viewer](http://www.microsoft.com/downloads/details.aspx?familyid=39fe2229-9201-4270-bdc1-20bc8e30a766)  
(KB2251437)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Sada Microsoft Office Compatibility Pack pro formáty souborů aplikací Word, Excel a PowerPoint 2007 Service Pack 2
</td>
<td style="border:1px solid black;">
[Sada Microsoft Office Compatibility Pack pro formáty souborů aplikací Word, Excel a PowerPoint 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ed5b9671-651d-41f3-aed3-93ee8a28657f)  
(KB2277947)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Works 9
</td>
<td style="border:1px solid black;">
[Microsoft Works 9](http://www.microsoft.com/downloads/details.aspx?familyid=feb121ad-e5f6-40e2-bf12-045ae5c2a754)  
(KB2092914)  
(Vysoký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
</tr>
</table>
<p></p>
 
**Poznámka k bulletinu MS10-056**

<sup>[1]</sup>Na ochranu před chybami zabezpečení popsanými v bulletinu MS10-056 je u aplikace Microsoft Office Word 2007 Service Pack 2 kromě balíčku aktualizací zabezpečení KB2251419 potřeba nainstalovat také aktualizaci zabezpečení pro sadu Microsoft Office Compatibility Pack pro formáty souborů aplikací Word, Excel a PowerPoint 2007 s aktualizací Service Pack 2 (KB2277947).

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
Microsoft Silverlight
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS10-060**](http://go.microsoft.com/fwlink/?linkid=179830)
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
Microsoft Silverlight 2
</td>
<td style="border:1px solid black;">
[Microsoft Silverlight 2](http://www.microsoft.com/getsilverlight/get-started/install/default.aspx)<sup>[1]</sup> při instalaci v systému Mac OS  
(KB982926)  
(Kritický)  
[Microsoft Silverlight 2](http://www.microsoft.com/getsilverlight/get-started/install/default.aspx)<sup>[1]</sup> při instalaci ve všech vydáních klientů Microsoft Windows  
(KB982926)  
(Kritický)  
[Microsoft Silverlight 2](http://www.microsoft.com/getsilverlight/get-started/install/default.aspx)<sup>[1]</sup> při instalaci ve všech vydáních serverů Microsoft Windows\*\*  
(KB982926)  
(Kritický)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Silverlight 3
</td>
<td style="border:1px solid black;">
[Microsoft Silverlight 3](http://www.microsoft.com/downloads/details.aspx?familyid=7e3f6c16-1339-49bc-a60c-ddc6c3a54850)<sup>[2]</sup> při instalaci v systému Mac  
(KB978464)  
(Kritický)  
[Microsoft Silverlight 3](http://www.microsoft.com/downloads/details.aspx?familyid=7e3f6c16-1339-49bc-a60c-ddc6c3a54850)<sup>[2]</sup> při instalaci ve všech vydáních klientů Microsoft Windows  
(KB978464)  
(Kritický)  
[Microsoft Silverlight 3](http://www.microsoft.com/downloads/details.aspx?familyid=7e3f6c16-1339-49bc-a60c-ddc6c3a54850)<sup>[2]</sup> při instalaci ve všech vydáních serverů Microsoft Windows\*\*  
(KB978464)  
(Kritický)
</td>
</tr>
</table>
<p></p>
 
**Poznámky k bulletinu MS10-060**

**\*\*Instalace Server Core není touto chybou ovlivněna.** Chyby zabezpečení, které tato aktualizace řeší, nemají vliv na podporované edice systému Windows Server 2008 nebo Windows Server 2008 R2, jak je uvedeno, v případě instalace s využitím možnosti instalace Server Core. Další informace o této možnosti instalace naleznete v článcích na webu TechNet [Managing a Server Core Installation](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) (Správa instalace Server Core) a [Servicing a Server Core Installation](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx) (Obsluha instalace Server Core). Možnost instalace Server Core se nevztahuje na určité edice systému Windows Server 2008 a Windows Server 2008 R2; další informace naleznete v části [Porovnání možností instalace Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

<sup>[1]</sup>Tato položka ke stažení upgraduje program Microsoft Silverlight 2 na novou verzi, která není postižena chybami zabezpečení popsanými v tomto bulletinu.

<sup>[2]</sup>Tato aktualizace upgraduje program Microsoft Silverlight na novější sestavení, které není postiženo chybami zabezpečení popsanými v tomto bulletinu.

Více aktualizovaných souborů v rámci stejného identifikátoru bulletinu naleznete také v dalších kategoriích softwaru v rámci této části **Software obsahující tuto chybu a umístění aktualizací ke stažení**. Tento bulletin se vztahuje na více kategorií softwaru.

Nástroje a doporučené postupy zjišťování a nasazení
---------------------------------------------------

 
**Centrum zabezpečení**

Umožňuje správu aktualizací softwaru a zabezpečení, které je třeba nainstalovat na servery, stolní počítače a přenosné počítače v organizaci. Další informace naleznete na webu [TechNet Update Management Center](http://go.microsoft.com/fwlink/?linkid=69903). Další informace o zabezpečení produktů společnosti Microsoft nabízí web [Centrum zabezpečení TechNet](http://go.microsoft.com/fwlink/?linkid=21171). Tyto informace lze také získat kliknutím na nabídku „Nejnovější aktualizace zabezpečení“ na webu [Zabezpečení doma](http://go.microsoft.com/fwlink/?linkid=85102).

Aktualizace zabezpečení jsou k dispozici na webu [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747) a [Windows Update](http://go.microsoft.com/fwlink/?linkid=21130). Aktualizace zabezpečení jsou také k dispozici na webu [služby Stažení softwaru](http://go.microsoft.com/fwlink/?linkid=21129). Nejsnadněji je naleznete hledáním podle klíčových slov aktualizace zabezpečení.

Aktualizace zabezpečení lze stáhnout z katalogu služby [Microsoft Update Catalog](http://go.microsoft.com/fwlink/?linkid=96155). Služba Microsoft Update Catalog poskytuje katalog s možností vyhledávání obsahu dostupného prostřednictvím služeb Windows Update a Microsoft Update, včetně aktualizací zabezpečení, ovladačů a aktualizací Service Pack. Vyhledáváním pomocí čísla bulletinu zabezpečení (například MS07-036) můžete přidat všechny dostupné aktualizace do košíku (včetně různých jazykových verzí aktualizace) a stáhnout je do vybrané složky. Další informace o službě Microsoft Update Catalog najdete v části [Nejčastější dotazy týkající se služby Microsoft Update Catalog](http://go.microsoft.com/fwlink/?linkid=97900).

**Poznámka:** K 1. srpnu 2009 ukončí společnost Microsoft podporu webu Office Update a nástroje Office Update Inventory Tool. Nejnovější aktualizace produktů Microsoft Office bude přinášet web [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747). Další informace naleznete v části [O webu Microsoft Office Update: Nejčastější dotazy](http://office.microsoft.com/en-us/downloads/fx010402221033.aspx).

**Doporučené postupy zjišťování a nasazení**

Společnost Microsoft poskytuje doporučené postupy zjišťování a nasazení aktualizací zabezpečení. Tyto dokumenty obsahují doporučení a informace, které mohou odborníkům v oblasti IT pomoci porozumět, jak se používají různé nástroje pro detekci a nasazení aktualizací zabezpečení. Další informace získáte v [článku 961747 znalostní báze Microsoft Knowledge Base](http://support.microsoft.com/kb/961747).

**Nástroj Microsoft Baseline Security Analyzer**

Pomocí nástroje Microsoft Baseline Security Analyzer (MBSA) mohou správci prohledávat místní i vzdálené systémy a zjistit tak, jestli v nich nechybí některé aktualizace zabezpečení nebo jestli v nastavení zabezpečení systému nedošlo k některým běžným chybám. Další informace o nástroji MBSA získáte na webu [Microsoft Baseline Security Analyzer](http://go.microsoft.com/fwlink/?linkid=21134).

**Služba Windows Server Update Services**

Služba WSUS (Windows Server Update Services) umožňuje správcům IT nasazovat nejnovější aktualizace produktů Microsoft do počítačů používajících operační systém Windows. Další informace o způsobu nasazení aktualizací zabezpečení pomocí služby Windows Server Update Services získáte v článku na webu TechNet [Windows Server Update Services](http://technet.microsoft.com/en-us/wsus/default.aspx).

**Systems Management Server**

Microsoft Systems Management Server (SMS) představuje v rozlehlých sítích řešení pro správu aktualizací s rozsáhlými možnostmi konfigurace. Umožňuje správcům identifikovat počítače se systémem Windows, které vyžadují aktualizace zabezpečení, a provést řízenou instalaci těchto aktualizací v celé rozlehlé síti s minimálním dopadem na koncové uživatele. K dispozici je nyní nová verze nástroje SMS, System Center Configuration Manager 2007 (viz také webové stránky produktu [System Center Configuration Manager 2007](http://technet.microsoft.com/en-us/library/bb735860.aspx)). Další informace o tom, jak mohou správci pomocí serveru SMS 2003 nasazovat aktualizace zabezpečení, získáte na webu [SMS 2003 Security Patch Management](http://go.microsoft.com/fwlink/?linkid=22939). Uživatelé služby SMS 2.0 mohou k nasazení aktualizací zabezpečení použít také nástroj SUIT (Security Update Inventory Tool). Další informace o serveru SMS získáte na webu [Microsoft Systems Management Server](http://go.microsoft.com/fwlink/?linkid=21158).

**Poznámka:** Služba SMS pomocí modulu Microsoft Baseline Security Analyzer poskytuje rozsáhlou podporu při zjišťování a nasazení aktualizací bulletinu zabezpečení. Tyto nástroje nemusí některé softwarové aktualizace zjistit. V takovém případě mohou správci použít funkce serveru SMS a nasměrovat aktualizace do určitých systémů. Další informace o tomto postupu najdete na webu [Nasazení aktualizací softwaru pomocí funkce Distribuce softwaru serveru SMS](http://go.microsoft.com/fwlink/?linkid=33341). Některé aktualizace zabezpečení vyžadují po restartování počítače oprávnění správce. Správci mohou k instalaci těchto aktualizací použít nástroj Elevated Rights Deployment Tool (k dispozici v sadě [SMS 2.0 Administration Feature Pack](http://go.microsoft.com/fwlink/?linkid=21161)).

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

-   Sergeyi I. Ulasenovi a Olegu Kupreevovi ze společnosti [VirusBlokAda](http://www.anti-virus.by/) za oznámení chyby popsané v bulletinu MS10-046.
-   Andreasi Marxovi a Maiku Morgensternovi ze společnosti [AV-Test](http://www.av-test.org/) za oznámení chyby popsané v bulletinu MS10-046.
-   Willu Dormannovi ze společnosti [CERT/CC](http://www.cert.org) za spolupráci na řešení chyby popsané v bulletinu MS10-046.
-   Nielsu Teusinkovi za spolupráci na řešení chyby popsané v bulletinu MS10-046.
-   Stefanu Kanthakovi za spolupráci na řešení chyby popsané v bulletinu MS10-046.
-   Tavisovi Ormandymu ze společnosti [Google Inc.](http://www.google.com/) za oznámení tří chyb popsaných v bulletinu MS10-047.
-   Tavisovi Ormandymu ze společnosti [Google Inc.](http://www.google.com/) za oznámení chyby popsané v bulletinu MS10-048.
-   Matthieu Suichemu ze společnosti [MoonSols](http://moonsols.com/) za oznámení dvou chyb popsaných v bulletinu MS10-048.
-   Matthieu Suichemu ze společnosti [MoonSols](http://moonsols.com/) za spolupráci na změnách zvyšujících zabezpečení popsaných v bulletinu MS10-048.
-   Nicolási Economou ze společnosti [Core Security Technologies](http://www.coresecurity.com/) za oznámení chyby popsané v bulletinu MS10-048.
-   Marshi Rayovi a Steveu Dispensaovi ze společnosti [PhoneFactor](http://www.phonefactor.com/) za oznámení chyby popsané v bulletinu MS10-049.
-   Dyonu Baldingovi ze společnosti [Secunia](http://secunia.com/) za oznámení chyby popsané v bulletinu MS10-050.
-   Uživateli s pseudonymem SkyLined ze společnosti [Google Inc.](http://www.google.com/) za oznámení chyby popsané v bulletinu MS10-051.
-   Moritzu Jodeitovi ze společnosti n.runs AG, spolupracujícímu s organizací [Zero Day Initiative](http://www.zerodayinitiative.com/) společnosti [TippingPoint](http://www.tippingpoint.com/), za oznámení chyby popsané v bulletinu MS10-052.
-   Davidu Bloomovi ze společnosti [Google Inc.](http://www.google.com/) za oznámení chyby popsané v bulletinu MS10-053.
-   Nicolasi Jolymu ze skupiny [VUPEN Vulnerability Research Team](http://www.vupen.com) za oznámení čtyř chyb popsaných v bulletinu MS10-053.
-   Gambinu ZaDarkSideovi za oznámení chyby popsané v bulletinu MS10-053.
-   Laurentovi Gaffiému ze společnosti [stratsec](http://www.stratsec.net/) za oznámení chyby popsané v bulletinu MS10-054.
-   Toddovi Weasemu a Richardu Johnsonovi ze společnosti [Sourcefire VRT](http://www.sourcefire.com/services/sf_vrt.html) za oznámení chyby popsané v bulletinu MS10-054.
-   Riku Hietamakimu a Joshua Morinovi ze společnosti [Codenomicon](http://www.codenomicon.com/) za oznámení chyby popsané v bulletinu MS10-054.
-   Anonymnímu výzkumníkovi spolupracujícímu s organizací [Zero Day Initiative](http://www.zerodayinitiative.com/) společnosti [TippingPoint](http://www.tippingpoint.com/) za oznámení chyby popsané v bulletinu MS10-055.
-   Uživateli s pseudonymem L.W.Z ze skupiny [team509](http://www.team509.com/), spolupracujícímu s organizací [Zero Day Initiative](http://www.zerodayinitiative.com/) společnosti [TippingPoint](http://www.tippingpoint.com/), za oznámení chyby popsané v bulletinu MS10-056.
-   Uživateli s pseudonymem wushi ze skupiny [team509](http://www.team509.com/), spolupracujímu se společností [VeriSign iDefense Labs](http://labs.idefense.com/), za oznámení chyby popsané v bulletinu MS10-056.
-   Skupině [team509](http://www.team509.com/), spolupracující se společností [VeriSign iDefense Labs](http://labs.idefense.com/), za oznámení chyby popsané v bulletinu MS10-056.
-   Rodrigu Rubira Brancovi z výzkumného týmu IPS společnosti [Check Point](http://www.checkpoint.com/) za oznámení chyby popsané v bulletinu MS10-056.
-   Anonymnímu výzkumníkovi spolupracujícímu s organizací [Zero Day Initiative](http://www.zerodayinitiative.com/) společnosti [TippingPoint](http://www.tippingpoint.com/) za oznámení chyby popsané v bulletinu MS10-056.
-   Damiánu Frizzovi ze společnosti [Core Security Technologies](http://www.coresecurity.com/) za oznámení chyby popsané v bulletinu MS10-057.
-   Darrenu Willisovi ze společnosti [Fourteenforty Research Institute, Inc.](http://www.fourteenforty.jp/) za oznámení chyby popsané v bulletinu MS10-058.
-   Matthieu Suichemu ze společnosti [MoonSols](http://moonsols.com/) za oznámení chyby popsané v bulletinu MS10-058.
-   Cesaru Cerrudovi ze společnosti [Argeniss](http://www.argeniss.com/) za spolupráci na řešení dvou chyb popsaných v bulletinu MS10-059.
-   Carstenu Bookovi ze společnosti za oznámení chyby popsané v bulletinu MS10-060.
-   [Eamonovi Nerbonnemu](http://eamon.nerbonne.org/) za oznámení chyby popsané v bulletinu MS10-060.

#### Technická podpora

-   Uvedený software byl testován za účelem zjištění, kterých verzí se chyba týká. U dalších verzí skončila časově omezená podpora. Pokud chcete zjistit dobu, po kterou je pro určitou verzi softwaru poskytována podpora, navštivte web [Zásady poskytování technické podpory pro produkty společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=21742).
-   Zákazníci mohou získat technickou podporu na webu [služby technické podpory společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=21131). Hovory související s aktualizacemi zabezpečení jsou bezplatné. Další informace o dostupných možnostech technické podpory naleznete na webu [Pomoc a podpora společnosti Microsoft](http://support.microsoft.com/).
-   Mezinárodní zákazníci získají podporu u místních zastoupení společnosti Microsoft. Technická podpora související s aktualizacemi zabezpečení je bezplatná. Další informace o možnostech kontaktování společnosti Microsoft v případě potřeby technické podpory získáte na [webu mezinárodní technické podpory](http://go.microsoft.com/fwlink/?linkid=21155).

#### Zřeknutí se záruky

Informace ve znalostní bázi Microsoft Knowledge Base jsou poskytovány tak, jak jsou, bez jakékoli záruky. Společnost Microsoft neposkytuje žádné záruky, výslovně uvedené či mlčky předpokládané, včetně záruk obchodovatelnosti a vhodnosti pro určitý účel. Společnost Microsoft ani její dodavatelé nenesou v žádném případě zodpovědnost za žádné škody, včetně přímých, nepřímých, náhodných či následných škod, ztráty zisku či zvláštních škod, a to ani v případě, že byli na možnost takových škod upozorněni. V některých zemích a právních řádech není dovoleno vyloučit nebo omezit odpovědnost, proto se výše uvedené omezení na vás nemusí vztahovat.

#### Revize

-   V1.0 (2. srpna 2010): Souhrnný bulletin byl publikován.
-   V2.0 (10. srpna 2010): Byly přidány bulletiny MS10-047 až MS10-060.
-   V2.1 (1. září 2010): Byla přidána poznámka k bulletinu MS10-056 informující zákazníky používající aplikaci Word 2007, že je třeba vedle balíčku aktualizací zabezpečení KB2251419 nainstalovat také balíček aktualizací zabezpečení KB2277947.

*Built at 2014-04-18T01:50:00Z-07:00*
