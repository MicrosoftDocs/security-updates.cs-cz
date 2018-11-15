---
TOCTitle: Údržba databáze protokolování
Title: Údržba databáze protokolování
ms:assetid: 'de55058b-0d1a-4997-8a45-e14678ddd13f'
ms:contentKeyID: 18113464
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747691(v=WS.10)'
---

Údržba databáze protokolování
=============================

Položky protokolu obsahují také kopie licencí vydaných pro různé operace služby RMS, jako je zápis uživatelů a přiřazení licencí k použití. V nejhorším případě (kdy každá položka protokolu představuje úspěšný zápis uživatele nebo úspěšný pokus o získání licence k použití) znamená každá položka protokolu nárůst velikosti databáze protokolování asi o 200 kB.

Předpokládejme například, že všem zaměstnancům společnosti, která zaměstnává 50 000 uživatelů, byla odeslána e-mailová zpráva chráněná službou RMS a že každý zaměstnanec ji otevře. Jestliže by všichni zaměstnanci tuto e-mailovou zprávu otevřeli během jednoho dne, zvětšila by se velikost databáze protokolování o 10 GB. Je možné nakonfigurovat službu naslouchání tak, aby nebyla protokolována skutečná data XrML, což sníží množství protokolovaných informací.

Zvažte možnost vytvoření skriptů umožňujících archivaci starších informací databáze protokolování do sekundární databáze. Příklady skriptů protokolování jsou k dispozici ke stažení zdarma v sadě RMS Toolkit na [webu společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=26724) (http://go.microsoft.com/fwlink/?LinkId=26724).

Proměnné ovlivňující růst databáze protokolování
------------------------------------------------

Odhad velikosti databáze protokolování závisí na daném prostředí. Lze odhadnout několik položek, které budou do protokolu zapsány po zahájení provozu. Jedná se o následující položky:

-   zápis serveru RMS,
-   zápis uživatele (jedinečný požadavek pro každý počítač používaný jednotlivými uživateli),
-   automatické požadavky uživatelů na certifikáty pro publikování offline.

Skupina položek zapsaná do databáze protokolování po položkách spojených se zahájením provozu souvisí s vydáváním licencí k použití na chráněný obsah. Růst databáze ovlivňuje mnoho faktorů:

-   Vyžadování nové licence při každém přístupu uživatele k chráněnému obsahu. Nejedná se o výchozí možnost práce s chráněnými dokumenty, ale o nepovinné nastavení. Pokud zvolíte implementaci tohoto požadavku, bude se velikost databáze zvětšovat rychleji.
-   Očekávaný počet chráněných e-mailových zpráv, které každý uživatel denně odešle.
-   Očekávaný počet jedinečných uživatelů, kteří budou chráněné e-mailové zprávy číst.
-   Očekávaný počet chráněných dokumentů sady Microsoft Office 2003 (aplikace Word, PowerPoint nebo Excel), které každý uživatel denně vytvoří.
-   Očekávaný počet příjemců chráněných dokumentů.

Počáteční velikost databáze protokolování bude přibližně 1,7 MB, což zahrnuje požadavek na certifikát serveru RMS. Při zápisu získá každý nový uživatel certifikát účtu práv a klientský certifikát pro poskytování licencí. Tyto dvě akce jsou zaprotokolovány a dohromady zvýší velikost databáze o 0,06 MB. Vždy když uživatel úspěšně získá licenci na chráněný obsah, vzroste velikost databáze o 0,19 MB.

Následuje názorný příklad postupu určení odhadované velikosti: Představte si organizaci s 5 000 uživateli, ve které budou nasazení služby RMS používat všichni. Každý uživatel pracuje s jedním počítačem a organizace používá dva servery RMS. Po nasazení vytvoří každý uživatel v průměru jednu e-mailovou zprávu chráněnou službou RMS denně a odešle ji pěti dalším uživatelům. Každý uživatel zároveň během dne vytvoří jeden dokument chráněný službou RMS, k němuž budou chtít získat přístup tři další uživatelé. V následující tabulce najdete odhad vlivu uvedených činností na zvýšení velikosti databáze protokolování.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Akce</th>
<th style="border:1px solid black;" >Nárůst protokolu</th>
<th style="border:1px solid black;" >Kumulativní velikost protokolu</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Úspěšné zajištění serveru RMS</td>
<td style="border:1px solid black;">1,7 MB</td>
<td style="border:1px solid black;">1,7 MB</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Zápis 5 000 zaměstnanců (5000*0,06)</td>
<td style="border:1px solid black;">300 MB</td>
<td style="border:1px solid black;">301,7 MB</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Přístup k chráněné e-mailové zprávě (25000*0,19)</td>
<td style="border:1px solid black;">4 750 MB</td>
<td style="border:1px solid black;">5 051,7 MB</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Přístup k chráněným dokumentům (15000*0,19)</td>
<td style="border:1px solid black;">2 850 MB</td>
<td style="border:1px solid black;">7 901,7 MB</td>
</tr>
</tbody>
</table>
  
Z toho vyplývá, že po zápisu je statická velikost databáze protokolování přibližně 300 MB. Denní nárůst v tomto příkladu je však 7,6 GB, což se blíží hodnotě 8 GB, která představuje limit výchozí instalace služby Řízení front zpráv. Jestliže nebude databáze protokolování k dispozici po dobu delší než jeden den, začne docházet ke ztrátám položek protokolu.
  
Řízení velikosti databáze protokolování  
---------------------------------------
  
Do plánu nasazení je nutné zahrnout způsob správy databáze protokolování. Následují příklady nejobvyklejších postupů.
  
-   **Snížení velikosti a archivace**  
    Tento způsob představuje archivaci vybraných informací databáze protokolování do sekundární databáze pomocí skriptů serveru SQL Server v okamžiku, kdy položky protokolu dosáhnou určitého stáří. Zároveň jsou z databáze filtrovány nepodstatné informace, aby zbytečně nezabíraly místo.  
-   **Omezení protokolovaných informací**  
    Databázi protokolování tvoří tři hlavní tabulky. Jednou z nich je tabulka **DRMS\_Log\_Filter** označující pole hlavní tabulky, která by měla být zaprotokolována v případě povolení filtrování protokolu.  
    Položky tabulky s hodnotou pro povolení nebo zákaz určují pole hlavní tabulky, která budou službou naslouchání protokolování na serveru RMS skutečně zaprotokolována. U dvou z těchto polí (souvisejících s daty XrML) již byla nastavena hodnota 0 zakazující protokolování, protože tato pole tvoří kolem 99% velikosti každého řádku požadavku na licenci.  
    V rámci databáze **DRMS\_Config\_ServerName\_Port** existuje další tabulka s názvem **DRMS\_ClusterPolicies**, která obsahuje položku **PolicyName** možnosti **LoggingFiltering**. Možnost **LoggingFiltering** není ve výchozím nastavení povolena. Jestliže změníte nastavení možnosti **LoggingFiltering** na hodnotu 1 a restartujete službu naslouchání protokolování, poklesne denní nárůst velikosti databáze v uvedeném příkladu z hodnoty 7,6 GB denně na asi 160 MB denně.  
-   **Přesunutí databáze protokolování**  
    Další možností správy rostoucí databáze protokolování je její přesunutí na server s větším množstvím volného místa na disku. Databáze protokolování může být umístěna na jiném databázovém serveru než konfigurační databáze. Databází protokolování je možné na jiný server přesunout pomocí následujícího postupu:  
    1.  Zastavte na každém serveru RMS službu naslouchání protokolování.  
    2.  Zkopírujte databázi na jiný server (nebo vytvořte novou).  
    3.  Upravte databázi **DRMS\_Config\_ServerName\_Port** služby RMS výběrem tabulky **DRMS\_ClusterPolicies** a úpravou hodnot pro položku **LoggingDatabaseName** (název databáze) a **LoggingDatabaseServer** (název databázového serveru).  
    4.  Spuštěním programu IISRESET.exe z příkazového řádku restartujte službu IIS.
