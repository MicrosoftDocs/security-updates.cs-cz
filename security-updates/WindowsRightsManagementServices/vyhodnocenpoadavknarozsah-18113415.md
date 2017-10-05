---
TOCTitle: Vyhodnocení požadavků na rozsah
Title: Vyhodnocení požadavků na rozsah
ms:assetid: '89f0138c-946d-47d7-a286-041d4d9606a8'
ms:contentKeyID: 18113415
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747663(v=WS.10)'
---

Vyhodnocení požadavků na rozsah
===============================

Chcete-li rozhodnout, zda budete nasazovat jediný server nebo více serverů, určete počet uživatelů, kteří budou nasazení služby RMS používat, a počet souborů, u nichž budou tito uživatelé chtít nastavit ochranu.

Tímto způsobem zjistíte průměrné požadavky na využití. Určete maximální požadavky na využití, které pravděpodobně budou třikrát vyšší než průměrné požadavky.

Zároveň je třeba zohlednit odolnost systému společnosti proti chybám a standardy dostupnosti služby.

Jen pro srovnání: Služba RMS byla testována na serveru s duálním procesorem Pentium 4 2,4 GHz s 1 GB paměti RAM. Při této konfiguraci server RMS dodával přibližně 50 licencí za sekundu.

Při plánování kapacity můžete k odhadu požadavků na systém RMS z hlediska využití použít hodnoty uvedené v následující tabulce.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Transakce</th>
<th style="border:1px solid black;" >Výskyt</th>
<th style="border:1px solid black;" >Využití šířky pásma na trase klient-server (kB)</th>
<th style="border:1px solid black;" >Využití šířky pásma na trase server-klient (kB)</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Požadavek na licenci</td>
<td style="border:1px solid black;">Opakovaně pro každého uživatele a každou položku obsahu</td>
<td style="border:1px solid black;">64</td>
<td style="border:1px solid black;">18</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Certifikace účtu práv</td>
<td style="border:1px solid black;">Pouze počáteční tok dat služby RMS</td>
<td style="border:1px solid black;">12</td>
<td style="border:1px solid black;">16</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Zápis klienta</td>
<td style="border:1px solid black;">Pouze počáteční tok dat služby RMS</td>
<td style="border:1px solid black;">17</td>
<td style="border:1px solid black;">16</td>
</tr>
</tbody>
</table>
  
Propustnost sítě může být dále ovlivněna tokem dat souvisejícím s dotazy služby Active Directory. Tímto vlivem se však obvykle není nutné zabývat, pokud servery RMS nasazujete v těsné blízkosti serverů globálního katalogu. Výjimkou by byl případ, kdy by selhání všech serverů globálního katalogu na webu způsobilo převzetí služeb jiným webem prostřednictvím připojení, které nepodporuje stejnou kapacitu.
  
Následující tabulka obsahuje základní data týkající se využití šířky pásma transakcemi služby RMS, díky nimž je možné vyhodnotit vliv toku dat souvisejícího s dotazy služby Active Directory na síť organizace.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Transakce</th>
<th style="border:1px solid black;" >Využití šířky pásma na trase služba RMS-globální katalog (bajty)</th>
<th style="border:1px solid black;" >Využití šířky pásma na trase globálního katalog-služba RMS (bajty)</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Vytvoření připojení služby RMS (ldap_bind)</td>
<td style="border:1px solid black;">1600</td>
<td style="border:1px solid black;">200</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Vyhodnocení členství ve skupinách služby RMS (ldap_search)</td>
<td style="border:1px solid black;">200</td>
<td style="border:1px solid black;">100</td>
</tr>
</tbody>
</table>
  
Při práci s referenčními tabulkami aplikujte čísla na obsah daného nasazení. Pokud je například uživatel členem 15 skupin, bude požadavek služby RMS na vyhledávání vyžadovat 200 bajtů a odpověď globálního katalogu bude vyžadovat 1 500 bajtů (100 bajtů x 15).
  
Plánování kapacity by mělo být založeno na očekávaném zatížení požadavky na licence pro obsah, protože toto zatížení představuje hlavní část operací prováděných službou RMS. Vstupní a výstupní rychlost a výkon diskové jednotky nemají pro službu RMS podstatný význam, protože požadavky na licence neobsahují mnoho dat a zcela vystačí s informacemi v mezipaměti.
  
Při určování propustnosti serveru je nejpodstatnější proměnnou využití procesoru a záleží tedy na správné volbě procesorů. Požadavky na paměť serverů RMS se zvyšují zároveň s tím, jak se zvyšuje zatížení daného serveru a jak se pohybuje nad hodnotou maximálního výkonu serveru. V takovém případě internetová informační služba (IIS) řadí příchozí požadavky do fronty v paměti, odkud je přebírá server ke zpracování. Na základě limitu fronty nastaveného ve službě IIS mohou být příchozí žádosti po dosažení určité maximální délky fronty namísto zařazení do fronty odmítány.
  
Požadavky služby RMS na paměť (pracovní nastavení) pro určitý model zatížení by měly zcela odpovídat omezením velikosti fyzické paměti. Celková velikost paměti je ovlivňována především potřebami ukládání do mezipaměti při expanzi skupin. Pro každý server se službou RMS je doporučeno nejméně 1 GB paměti RAM.
  
Každý server RMS dokáže zpracovat stanovený počet požadavků klientů ve stanoveném čase (přibližně 30 až 50 licencí za sekundu). Přidáváním serverů lze tedy dosáhnout lineárního růstu celkové kapacity clusteru při vystavování licencí za současného zvýšení spolehlivosti. Ve výsledku lze říci, že rozšiřování se nemusí vztahovat jen na jednotlivé servery, ale také na počet implementovaných serverů. V následujících příkladech konfigurace zjistíte, jakým způsobem lze pomocí těchto odhadů vypočítat požadavky na rozsah nasazení služby RMS.
  
-   Konfigurace pro nízké využití  
    Některé organizace mají poměrně nízké požadavky na podporu služby RMS. Organizace s přibližně 5 000 uživateli, ve které službu RMS k ochraně obsahu e-mailů pravidelně využívá 10 procent uživatelů, například odhadne, že průměrný uživatel bude chtít nastavit ochranu u 3 e-mailových zpráv za hodinu. Na základě těchto požadavků bude nutné, aby servery RMS dodaly 1 500 licencí za hodinu, což se rovná 0,42 licencí za sekundu. Tímto způsobem jsme vypočítali průměrný požadavek na využití. Vynásobením zjištěného čísla hodnotou 3 získáme odhadované maximálního využití v počtu 1,25 licencí za sekundu.  
    Z těchto výpočtů vyplývá, že zatížení služby je velice nízké. Pro pokrytí požadavků této organizace postačí jediný server RMS.  
-   Konfigurace pro střední využití  
    V mnoha organizacích nalezneme velmi rozsáhlé skupiny uživatelů se středními požadavky na využití. Organizace s přibližně 40 000 uživateli, ve které službu RMS k ochraně obsahu pravidelně využívá 50 procent uživatelů, například odhadne, že průměrný uživatel bude chtít nastavit ochranu u 7 e-mailových zpráv a 1 dokumentu nebo jiného souboru za hodinu. Na základě těchto požadavků bude nutné, aby servery RMS dodaly 160 000 licencí za hodinu, což se rovná 44,4 licencí za sekundu. Tato hodnota představuje průměrné požadavky na využití. Vynásobíme-li ji třemi, dostaneme odhadované maximální využití v počtu 133,3 licencí za sekundu.  
    Z tohoto výpočtu vyplývá, že využití bude středně vysoké a aktuální požadavky uživatelů stačí zpracovat 3 servery RMS. Bude-li serverů 6, pokryjí nejen aktuální požadavky, ale i jejich další nárůst.  
-   Konfigurace pro vysoké využití  
    Ve větších organizacích se často setkáme s extrémně rozsáhlými skupinami uživatelů, jejichž nároky na využití jsou velmi vysoké. Organizace s přibližně 150 000 uživateli, ve které službu RMS k ochraně obsahu pravidelně využívá 70 procent uživatelů, například odhadne, že průměrný uživatel bude chtít nastavit ochranu u 15 e-mailových zpráv a 3 dokumentů nebo jiných souborů za hodinu. Na základě těchto požadavků bude nutné, aby servery RMS dodaly 1 890 000 licencí za hodinu, což se rovná 525 licencí za sekundu. Tato hodnota představuje průměrné požadavky na využití. Vynásobíme-li ji třemi, dostaneme odhadované maximální využití v počtu 1575 licencí za sekundu.  
    Z tohoto výpočtu vyplývá, že využití bude velmi vysoké, aktuální požadavky uživatelů stačí zpracovat 32 serverů RMS a bude-li serverů 51, pokryjí nejen aktuální požadavky, ale i jejich další nárůst.
  
Pokud z vašich výpočtů vyplývá, že na jeden server připadá 30 až 50 licencí za sekundu, obvykle to znamená, že je třeba instalovat další server RMS.
