---
TOCTitle: Poznámky k verzi pro Službu správy přístupových práv v systému Windows s aktualizací Service Pack 2
Title: Poznámky k verzi pro Službu správy přístupových práv v systému Windows s aktualizací Service Pack 2
ms:assetid: '78067886-681f-49a6-b43d-bfd08a369b69'
ms:contentKeyID: 18113379
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747637(v=WS.10)'
---

Poznámky k verzi pro Službu správy přístupových práv v systému Windows s aktualizací Service Pack 2
===================================================================================================

*Datum vydání: Prosinec 2006*

Před zahájením
--------------

Před instalací Služby správy přístupových práv (RMS) Microsoft® Windows® s aktualizací Service Pack 2 (SP2) prostudujte následující informace. Informace obsažené v těchto poznámkách k verzi platí pro server RMS s aktualizací SP2, nikoli pro klienta RMS. Informace o klientech RMS najdete v části Služba správy přístupových práv ([http://go.microsoft.com/fwlink/?LinkId=68637](http://go.microsoft.com/fwlink/?linkid=68637)) (stránka může být v angličtině).

#### Požadavky na systém

Hardwarové požadavky na spuštění služby RMS s aktualizací SP2 jsou uvedeny v následující tabulce.

###  

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Požadavek</th>
<th>Doporučení</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>Počítač s jedním procesorem Pentium III (800 MHz nebo rychlejší)</p></td>
<td style="border:1px solid black;"><p>Počítač se dvěma procesory Pentium 4 (1500 MHz nebo rychlejší)</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>256 MB paměti RAM</p></td>
<td style="border:1px solid black;"><p>512 MB paměti RAM</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>20 GB volného místa na pevném disku</p></td>
<td style="border:1px solid black;"><p>40 GB volného místa na pevném disku</p></td>
</tr>
</tbody>
</table>
  
| ![](images/Cc747637.note(WS.10).gif)Poznámka                                                                |  
|------------------------------------------------------------------------------------------------------------------------------------------|  
| Server RMS s aktualizací SP2 byl navržen pro 32bitový počítač. V případě instalace do 64bitového počítače bude spuštěn v režimu emulace. |
  
Softwarové požadavky pro servery používající službu RMS s aktualizací SP2 jsou uvedeny v následující tabulce.
  
###  

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Součást</th>
<th>Požadavek</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>Operační systém</p></td>
<td style="border:1px solid black;"><p>Microsoft Windows Server® 2003, s výjimkou verze Web Edition, pro službu RMS s aktualizací SP2.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Služba Správa přístupových práv s aktualizací SP2</p></td>
<td style="border:1px solid black;"><p>Před upgradem na službu RMS s aktualizací SP2 musí být nainstalována služba RMS s aktualizací Service Pack 1 (SP1). Pro klienta RMS s aktualizací SP2 tento požadavek neplatí.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Systém souborů</p></td>
<td style="border:1px solid black;"><p>Je doporučen systém souborů NTFS.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Požadované součásti</p></td>
<td style="border:1px solid black;"><ul>
<li>Řízení front zpráv (označované také jako MSMQ) s povolenou integrací adresářové služby Active Directory®.<br />
<br />
</li>
<li>Internetová informační služba (IIS) s povolenými službami ASP.NET.<br />
<br />
</li>
<li>Rozhraní Microsoft .NET Framework 1.1<br />
<br />
</li>
</ul></td>
</tr>
</tbody>
</table>
<p> </p>

| ![](images/Cc747637.note(WS.10).gif)Poznámka                                                                                                                                 |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Pokud u služby RMS s aktualizací SP2 povolíte vzdálenou správu, pak počítač, který se připojuje ke službě správy služby RMS s aktualizací SP2, musí používat aplikaci Internet Explorer 6.0 nebo novější. |

Požadavky na infrastrukturu pro servery používající službu RMS s aktualizací SP2 jsou uvedeny v následující tabulce.

###  

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Součást</th>
<th>Požadavky</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>Adresářové služby</p></td>
<td style="border:1px solid black;"><p>Služba Active Directory na řadičích domény se systémem Windows Server 2000 s aktualizací Service Pack 3 (SP3) nebo novějším, která patří do stejné domény jako služba RMS. Všichni uživatelé a skupiny využívající službu RMS k získávání licencí a k publikování obsahu musí mít e-mailovou adresu konfigurovanou ve službě Active Directory.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Databázový server</p></td>
<td style="border:1px solid black;"><p>K provádění operací vyžaduje služba RMS s aktualizací SP2 databázi a uložené procedury. Můžete použít Microsoft SQL Server™ 2000 s aktualizací SP3 nebo novější či Microsoft SQL Server 2005. Pro testování nebo nasazení v jednom počítači lze použít Microsoft SQL Server Desktop Engine (MSDE 2000) verze A nebo Microsoft SQL Server 2005 Express Edition.</p></td>
</tr>
</tbody>
</table>
  
Služba RMS je navržena a testována pro databázové servery používající Microsoft SQL Server 2000 a Microsoft SQL Server 2005. Službu RMS lze spustit na jiných databázových serverech, pokud splňují následující kritéria:
  
-   podpora rozhraní ADO.NET poskytovaná rozhraním Microsoft .NET Framework 1.1,  
-   kompatibilita s jazykem Transact-SQL, což je strukturovaný jazyk dotazů používaný serverem Microsoft SQL Server, protože inicializační skripty a uložené procedury služby RMS používají jazyk Transact-SQL,  
-   podpora všech specifických rozšíření serveru Microsoft SQL Server,  
-   odpovědi na volání metod oboru názvů System.Data.SqlClient rozhraní .NET Framework,  
-   poskytování odpovídající funkčnosti oboru názvů System.Data.SqlClient,  
-   používání režimu ověřování systému Windows.
  
Chcete-li zjistit, zda databázový server podporuje předchozí kritéria, obraťte se na příslušného dodavatele databází.
  
V následující tabulce jsou uvedena uživatelská práva a oprávnění požadovaná při provádění různých činností v rámci služby RMS.
  
###  

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Činnost</th>
<th>Požadavky na účet</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>Instalace služby RMS</p></td>
<td style="border:1px solid black;"><p>Uživatel domény s pověřeními správce místního počítače</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Zajišťování kořenového clusteru služby RMS</p></td>
<td style="border:1px solid black;"><p>Uživatel domény s pověřeními správce místního počítače a s oprávněními k vyhledávání a zápisu do služby Active Directory</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Zajišťování vyhrazeného clusteru pro správu licencí služby RMS</p></td>
<td style="border:1px solid black;"><p>Uživatel domény s pověřeními správce místního počítače a s oprávněními k vyhledávání ve službě Active Directory</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Zajišťování při používání nové konfigurační databáze</p></td>
<td style="border:1px solid black;"><p>Uživatel domény s pověřeními správce místního počítače a s oprávněními ke čtení, zápisu a vytváření v počítači se serverem SQL Server</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Zajišťování při používání existující konfigurační databáze</p></td>
<td style="border:1px solid black;"><p>Uživatel domény s pověřeními správce místního počítače a s oprávněními ke čtení a zápisu v počítači s databázovým serverem</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Správa služby RMS</p></td>
<td style="border:1px solid black;"><p>Uživatel domény s pověřeními správce místního počítače</p></td>
</tr>
</tbody>
</table>
  
| ![](images/Cc747637.note(WS.10).gif)Poznámka                                                                                                                                                                                                                                                 |  
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Další informace o konfiguraci serveru Windows Server, službě Active Directory, službě Řízení front zpráv, službě IIS a systémech souborů naleznete na webu Windows Server 2003 TechCenter ([http://go.microsoft.com/fwlink/?LinkId=78135](http://go.microsoft.com/fwlink/?linkid=78135)) (stránka může být v angličtině). |
  
Používáte-li Službu správy přístupových práv při nasazení clusterů, zajistěte vyřešení bodů uvedených v následující tabulce.
  
###  

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Situace</th>
<th>Doporučení</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>Velký počet počítačů využívajících Službu správy přístupových práv</p></td>
<td style="border:1px solid black;"><p>K instalaci klientů RMS s aktualizací SP2 použijte server SMS nebo zásady skupiny.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Velký počet požadavků klientů</p></td>
<td style="border:1px solid black;"><p>Použijte server pro vyrovnávání zatížení, službu Vyrovnávání zatížení sítě operačního systému Windows Server nebo hardwarové vyrovnávání zatížení a rozdělte požadavky klientů do celého clusteru.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Dva síťové adaptéry, které používají virtuální IP adresování ke zpracování požadavků z extranetu i intranetu</p></td>
<td style="border:1px solid black;"><p>Zajistěte, aby každá registrace DNS (Domain Name System), která vystavuje svou virtuální IP adresu do extranetu, tuto adresu vystavila také do intranetu.</p></td>
</tr>
</tbody>
</table>
  
| ![](images/Cc747637.Important(WS.10).gif)Důležité informace                                                                                                                                                                                                                                                                                                                                                                                                                 |  
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Není-li provedena registrace DNS pro intranet, nebude možné zpracovávat požadavky na licence od interních klientů. Potřebujete-li namapovat adresu URL clusteru na jeho virtuální IP adresu a nemůžete upravit nastavení DNS, můžete potřebné položky doplnit do tabulky hostitelů na jednotlivých serverech v clusteru. Registraci DNS je třeba provést před zajištěním služby RMS. Pokud jste již provedli zajištění služby, je nutné odinstalovat službu RMS ze serveru a zopakovat proces zajištění. |
  
#### Podporovaní klienti pro tuto verzi
  
Klienta RMS bez aktualizace Service Pack, klienta RMS s aktualizací SP1 nebo klienta RMS s aktualizací SP2 lze nainstalovat do libovolného počítače se systémem Microsoft Windows 2000, Windows XP nebo Windows Server 2003. Starší verze operačních systémů Windows nejsou touto verzí podporovány.
  
| ![](images/Cc747637.Caution(WS.10).gif)Upozornění                                                                              |  
|-------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Pokud používáte klienta RMS bez aktualizace Service Pack, nebude tento klient moci využívat online publikování na serveru RMS s aktualizací SP1 nebo vyšší. |
  
Změny funkcí  
------------
  
Služba RMS s aktualizací SP2 obsahuje několik nových funkcí:
  
-   [Zdokonalené rozšiřování skupin mezi doménovými strukturami](#bkmk_cif1)  
-   [Změny protokolování databáze](#bkmk_cif2)  
-   [Větší velikost dávek na serveru](#bkmk_cif3)  
-   [Kompatibilita se serverem Microsoft SQL Server 2005](#bkmk_cif4)
  
<span id="BKMK_CIF1"></span>
#### Zdokonalené rozšiřování skupin mezi doménovými strukturami
  
#### K čemu tato funkce slouží?
  
Ve službě RMS zajišťuje rozšíření skupiny mezi doménovými strukturami schopnost této služby rozšířit členství v univerzální skupině služby Active Directory do jiných doménových struktur, kde členství ve skupině nejsou replikována mezi dvěma doménovými strukturami. Pokud uživatel v jedné doménové struktuře odešle obsah chráněný právy uživateli v jiné doménové struktuře, proběhne ve službě RMS proces zjišťování, který ověří, zda má tento uživatel k obsahu povolen přístup. Tento proces ověření se provádí pomocí dotazu protokolu LDAP odeslaného z jedné doménové struktury do druhé za účelem vyhledání spojovacího bodu služby RMS ve vzdálené doménové struktuře. Po vyhledání spojovacího bodu služby pro vzdálenou doménovou strukturu odešle účet služby RMS požadavek na kanál rozšíření skupiny. Tento požadavek se dotáže vzdálené doménové struktury, zda je uživatel členem skupiny.
  
#### Komu je tato funkce určena?
  
Tato nová funkce bude zajímavá pro zákazníky služby RMS v prostředí více doménových struktur služby Active Directory, v níž nejsou členství v univerzálních skupinách replikována mezi doménovými strukturami.
  
#### Proč je tato změna důležitá?
  
Tento nový protokol rozšíření důvěryhodnosti doménové struktury zvýší spolehlivost pro zákazníky, kteří nasazují prostředí s více doménovými strukturami služby Active Directory.
  
#### V čem spočívá rozdíl?
  
Před verzí služby RMS s aktualizací SP2 bylo rozšíření skupiny v doménových strukturách prováděno pomocí vzdálených volání služby .NET. V této verzi byl protokol rozšíření skupiny v doménových strukturách změněn na webovou službu ASP.NET používající požadavky protokolu SOAP/HTTP odesílané do kanálu rozšíření důvěryhodných skupin doménové struktury.
  
| ![](images/Cc747637.note(WS.10).gif)Poznámka                                                                                                                                                                                                                            |  
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Z důvodu zpětné kompatibility služba RMS s aktualizací SP2 stále podporuje vzdálená volání služby .NET. Abyste však mohli plně využívat výhody nového protokolu rozšíření skupiny v doménových strukturách, musí být na všech clusterech služby RMS spuštěna minimálně služba RMS s aktualizací SP2. |
  
#### Jaké možnosti nastavení jsou přidány nebo změněny ve službě RMS s aktualizací SP2?
  
Nový kanál rozšíření skupiny služby RMS je ve výchozím nastavení služby RMS s aktualizací SP2 konfigurován s maximálním zabezpečením, kdy je přístup povolen pouze pro místní skupiny RMS Service a Administrators. Chcete-li poskytnout přístup pro účet, je nutné změnit seznam řízení přístupu u kanálu rozšíření skupiny v umístění wwwroot\\\_wmcs\\GroupExpansion\\GroupExpansion.asmx.
  
| ![](images/Cc747637.Important(WS.10).gif)Důležité informace                                                                                                                                                                                                                                                                                                                              |  
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Zajistěte, aby měl účet služby RMS v každé doménové struktuře služby Active Directory přístup ke kanálu rozšíření skupiny na každém serveru RMS v clusteru. Pokud účty nemají přístup povolen, rozšíření skupiny se nezdaří. Druhou možností je vytvořit stejný účet v každé doménové struktuře a přiřadit všem účtům stejná hesla. V takovém případě bude nutné přidat do kanálu rozšíření skupiny pouze jeden účet. |
  
Do služby RMS s aktualizací SP2 byly přidány nové události informující o problémových zprávách, které nebyly přidány do služby Řízení front zpráv. Tyto nové protokoly událostí zahrnují události, které vás upozorní, pokud zprávu nelze digitálně podepsat nebo pokud zprávu nelze ověřit. Mezi příklady problémů s ověřením patří chybně vytvořené zprávy, chybějící algoritmus hash či podpis nebo nesprávný algoritmus hash či podpis.
  
<span id="BKMK_CIF2"></span>
#### Změny protokolování databáze
  
#### K čemu tato funkce slouží?
  
Služba RMS používá službu naslouchání protokolování, která odesílá veškerou komunikaci služby RMS do databáze protokolování pomocí služby Řízení front zpráv. Cluster služby RMS odešle zprávy do služby Řízení front zpráv a služba naslouchání protokolování načte tyto zprávy z fronty služby Řízení front zpráv a zapíše je do databáze protokolování.
  
#### Komu je tato funkce určena?
  
Tato funkce je určena aktuálním uživatelům služby RMS používajícím službu naslouchání protokolování RMS a novým uživatelům služby RMS s aktualizací SP2, kteří uvažují o používání služby naslouchání protokolování RMS.
  
#### Proč je tato změna důležitá?
  
V předchozích verzích služby RMS byla fronta protokolování této služby chráněna pomocí seznamů řízení přístupu, avšak nebylo povoleno ověřování. Bez ověřování by uživatel se zlými úmysly mohl potenciálně zapsat chybné zprávy do fronty protokolování služby RMS.
  
#### V čem spočívá rozdíl?
  
Ve službě RMS s aktualizací SP2 je u zpráv odesílaných clusterem RMS pomocí služby Řízení front zpráv poskytováno dodatečné ověřování. Kromě seznamů řízení přístupu, které zabraňují neoprávněnému přístupu k frontě zpráv, je fronta služby Řízení front zpráv chráněna také mechanismem ověřování pravosti zprávy. Po odeslání zprávy do služby Řízení front zpráv vygenerují kanály služby RMS algoritmus hash zprávy a digitálně ji podepíší pomocí privátního klíče clusteru služby RMS. Služba naslouchání protokolování nejprve vypočítá svůj vlastní algoritmus hash zprávy a porovná jej s algoritmem hash zahrnutým do zprávy. Pokud se tyto algoritmy hash shodují, ověří služba naslouchání protokolování podpis pomocí veřejného klíče clusteru a algoritmu hash ve zprávě. Jestliže se algoritmy hash shodují a podpis je ověřen, bude zpráva odeslána do databáze protokolování. Pokud tyto kroky ověření neproběhnou úspěšně, bude zpráva trvale odstraněna z fronty služby Řízení front zpráv a do aplikačního protokolu v Prohlížeči událostí bude zapsána událost varování.
  
#### Jaké možnosti nastavení jsou přidány nebo změněny ve službě RMS s aktualizací SP2?
  
Do služby RMS s aktualizací SP2 byly přidány nové události informující o problémových zprávách, které nebyly přidány do fronty služby Řízení front zpráv. Tyto nové událostí jsou zapsány do aplikačního protokolu a zahrnují zprávy, které nelze digitálně podepsat nebo jejichž digitální podpisy nelze ověřit. Mezi příklady problémů s ověřením patří chybně vytvořené zprávy, chybějící algoritmus hash či podpis nebo nesprávný algoritmus hash či podpis.
  
<span id="BKMK_CIF3"></span>
#### Větší velikost dávek na serveru
  
#### K čemu tato funkce slouží?
  
Dávkování ve službě RMS zvyšuje výkon, neboť umožňuje odeslání více licenčních požadavků clusteru služby RMS jako jediný požadavek, na rozdíl od vytváření jednoho požadavku pro každou licenci.
  
#### Komu je tato funkce určena?
  
Podpora větších velikostí dávek na serveru bude zajímavá pro aplikace podporující službu RMS, které potřebují získávat více licencí na obsah chráněný právy současně.
  
#### Proč je tato změna důležitá?
  
Dávkování ve službě RMS umožňuje vydání jediného požadavku pro kanál AcquireLicense služby RMS za účelem získání licencí na používání pro více certifikátů účtů práv (RAC) u jedné či více licencí k publikování. Bez velikosti dávky větší než 1 by si aplikace podporující službu RMS musela vyžádat licenci na používání jednotlivě pro každého uživatele.
  
#### V čem spočívá rozdíl?
  
Ve verzích předcházejících službě RMS s aktualizací SP2 podporoval cluster RMS maximální velikost dávky 1. Pokud byla maximální velikost nastavena na hodnotu větší než 1, cluster ji ignoroval. U služby RMS s aktualizací SP2 může mít maximální velikost dávky hodnotu 100.
  
| ![](images/Cc747637.note(WS.10).gif)Poznámka |  
|---------------------------------------------------------------------------|  
| Dávkové požadavky podporuje pouze kanál AcquireLicense služby RMS.        |
  
Zasílání zpráv o chybách bylo ve službě RMS s aktualizací SP2 zdokonaleno tak, aby zahrnovalo dávkové požadavky. Pokud například odešlete dávku deseti požadavků a druhý a třetí požadavek je chybný, bude do protokolu událostí zapsána událost pro každou chybu.
  
<span id="BKMK_CIF4"></span>
#### Kompatibilita se serverem Microsoft SQL Server 2005
  
#### K čemu tato funkce slouží?
  
Ve službě RMS s aktualizací SP2 lze pro podporu konfigurace služby RMS a databází protokolování jako databázový server použít Microsoft SQL Server 2005, a to bez nutnosti dodatečné konfigurace.
  
#### Komu je tato funkce určena?
  
Podpora serveru Microsoft SQL Server 2005 se službou RMS s aktualizací SP2 bude zajímavá pro zákazníky služby RMS, kteří chtějí používat Microsoft SQL Server 2005 jako databázi služby RMS.
  
#### Proč je tato změna důležitá?
  
V předchozích verzích služby RMS nebyly datové typy některých parametrů používaných v tabulce sysmessages kompatibilní se specifikací formátu serveru Microsoft SQL Server 2005. Další informace najdete v článku 913372 znalostní báze Microsoft Knowledge Base ([http://go.microsoft.com/fwlink/?LinkId=68638](http://go.microsoft.com/fwlink/?linkid=68638)) (stránka může být v angličtině).
  
#### V čem spočívá rozdíl?
  
Ve verzích předcházejících verzi RMS s aktualizací SP2 se příkazy SQL RAISERROR používaly k upozornění uživatele služby RMS, že došlo k chybě. Příkaz RAISERROR odesílá dotaz do tabulky sysmessages za účelem načtení chybových zpráv služby RMS uložených v této tabulce. Služba RMS s aktualizací SP2 používá k předávání chyb SQL jiné postupy, proto již nezávisí na tabulce sysmessages.
  
| ![](images/Cc747637.note(WS.10).gif)Poznámka                                                                                                                                                                                                                                                     |  
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Pokud upgradujete ze služby RMS s aktualizací SP1 na službu RMS s aktualizací SP2, není již tabulka sysmessages dotazována na chybové zprávy, avšak samotné chybové zprávy zůstanou v tabulce sysmessages uloženy. Při čisté instalaci služby RMS s aktualizací SP2 nejsou do tabulky sysmessages přidány žádné nové položky. |
  
Známé problémy  
--------------
  
V následujících oddílech jsou uvedeny známé problémy s touto verzí služby RMS.
  
#### Soubor nápovědy stále odkazuje na službu RMS s aktualizací Service Pack 1
  
Soubor nápovědy, který je součástí instalace služby RMS s aktualizací SP2, stále odkazuje na službu RMS s aktualizací SP1. Informace o službě RMS s aktualizací SP2 najdete v tématu Služba správy přístupových práv ([http://go.microsoft.com/fwlink/?LinkId=68637](http://go.microsoft.com/fwlink/?linkid=68637)) (stránka může být v angličtině).
  
#### Služba Windows Update nemůže nainstalovat klienta služby RMS s aktualizací SP2 do počítačů s procesorem x64 nebo do počítačů s procesorem Itanium
  
Pokud je klient RMS nebo klient RMS s aktualizací SP1 nainstalován v počítači s procesorem x64 a pokusíte se ho upgradovat na verzi služby RMS s aktualizací SP2 (x64) z webu služby Windows Update, instalace se nezdaří. Ačkoli předchozí klienti služby RMS, kteří byli vytvořeni pro 32bitové systémy, fungovali v počítačích s procesory x64, nelze je upgradovat na klienta služby RMS s aktualizací SP2 (x64). Je nutné nejprve odinstalovat předchozího klienta služby RMS a pak upgrade spustit znovu. Systém Windows Update zjistí verzi operačního systému a nabídne příslušného klienta služby RMS s aktualizací SP2. To stejné platí pro počítače s procesory Itanium.
  
#### Opakované zajištění vždy způsobí chybu při spouštění služby naslouchání protokolování
  
Pokud cluster není zajištěn, nepodaří se službě naslouchání protokolování ponechat službu v zastaveném stavu. Chcete-li službu úplně zastavit, bude nutné restartovat počítač.
  
#### Nelze odebrat nesoftwarovou důvěryhodnou doménu publikování
  
Po importu důvěryhodné domény publikování s implementací nesoftwarového privátního klíče není možné tuto doménu odstranit. Import nesoftwarového privátního klíče by neměl být prováděn pomocí konzoly pro správu Služby správy přístupových práv systému Windows. Pokyny pro export a import privátního klíče vám poskytne příslušný poskytovatel hardwaru.
  
#### Rozhraní Microsoft .NET Framework 2.0 změní při instalaci na server RMS virtuální kořenové adresáře služby IIS
  
Služba RMS s aktualizací SP2 používá mapování skriptu ASP.NET, které je součástí rozhraní .NET Framework verze 1.1. Mapování dodávané s novějšími verzemi není kompatibilní se službou RMS s aktualizací SP2. Obě verze rozhraní však mohou být nainstalovány současně, aniž dojde ke kolizím s existujícími aplikacemi. Pokud je na serveru nainstalováno rozhraní .NET Framework 1.1 a současně .NET Framework 2.0 nebo novější, nemusí po zdánlivě úspěšné instalaci a zajištění služby RMS s aktualizací SP2 správně fungovat cluster RMS. Důvodem je skutečnost, že virtuální kořenové adresáře služby RMS musí být registrovány s mapováním skriptů ASP.NET verze 1.1, nikoli verze 2.0. Registraci virtuálních kořenových adresářů služby RMS s mapováním skriptů ASP.NET verze 1.1 provedete spuštěním následujícího příkazu na příkazovém řádku:
  
**%windir%\\Microsoft.NET\\Framework\\v1.1.4322&gt;aspnet\_regiis.exe -s W3SVC/1/ROOT/\_wmcs**
  
Tento příkaz správně zaregistruje virtuální kořenové adresáře služby RMS a umožní spuštění služby RMS s aktualizací SP2 na serveru.
  
#### Při používání nativní úrovně funkčnosti služby Active Directory v systému Windows 2000 mohou chybět členství ve skupinách
  
Pokud nasazujete službu RMS v prostředí, kde byla úroveň infrastruktury služby Active Directory zvýšena na nativní úroveň funkčnosti systému Windows 2000, nemusí být služba RMS při pokusu o rozšíření členství ve skupině skrytých distribučních seznamů schopna načíst atribut memberOf objektů služby Active Directory. Chcete-li Službě správy přístupových práv umožnit načtení atributu memberOf, musí služba RMS využívat účet domény, který je členem přístupové skupiny kompatibilní s přístupovými skupinami systémů starších než Windows 2000. Další informace najdete v článku 812841 znalostní báze Microsoft Knowledge Base ([http://go.microsoft.com/fwlink/?LinkId=78152](http://go.microsoft.com/fwlink/?linkid=78152)) (stránka může být v angličtině).
  
#### Služba naslouchání protokolování odešle zprávy služby Řízení front zpráv do fronty nedoručených zpráv, pokud k databázi nelze získat přístup
  
Existují případy (například při vypnutí databáze, problémech s připojením atd.), kdy služba naslouchání protokolování nemůže k databázi získat přístup. V takovém případě bude zpráva odeslána do fronty nedoručených zpráv. Jediným způsobem, jak tyto zprávy obnovit (to znamená odeslat je do databáze protokolování) je použít nástroj RMS Queue Recovery dodávaný v rámci sady RMS Administration Toolkit. Chcete-li stáhnout sadu RMS Administration Toolkit, navštivte web [http://go.microsoft.com/fwlink/?LinkId=33841](http://go.microsoft.com/fwlink/?linkid=33841) (stránka může být v angličtině).
  
| ![](images/Cc747637.note(WS.10).gif)Poznámka                                                                                                                                         |  
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Příkazy Recover a RecoverandPurge byly odebrány z procesu LogRecoveryCmd. Tak zajistíte, že všechny zprávy budou před odesláním do databáze protokolování směrovány zpět do služby Řízení fronty zpráv a ověřeny. |
  
#### Před upgradem na Microsoft SQL Server 2005 je třeba upgradovat na službu RMS s aktualizací SP2
  
Při upgradu na službu RMS s aktualizací SP2 a ze serveru Microsoft SQL Server 2000 na server Microsoft SQL Server 2005 je třeba nejprve upgradovat službu RMS. Tím se vyhnete potížím s kompatibilitou při upgradu serveru Microsoft SQL Server.
  
#### Službu RMS s aktualizací SP2 nelze zajistit na webech, jejichž název obsahuje apostrof (')
  
Pokud se pokusíte zajistit službu RMS s aktualizací SP2 na webu, jehož název obsahuje apostrof ('), proces zajištění se nezdaří a zobrazí se chybová zpráva **Neplatný parametr**. Chcete-li službu RMS s aktualizací  SP2 na webu zajistit, odstraňte apostrof z názvu webu.
  
#### Povolení služeb ASP.NET verze 1.1 na serverech s 64bitovou verzí systému Windows Server 2003
  
Téma Požadavky na systém v nápovědě služby RMS obsahuje informace o instalaci rozhraní .NET Framework 1.1 a povolení služeb ASP.NET 1.1 po instalaci Internetové informační služby (IIS). Pokud je však rozhraní .NET Framework 1.1 nainstalováno před službou IIS, nebude služba ASP.NET 1.1 uvedena v rozšířeních webových služeb a uvedený postup nebude možné použít. Pokud byla služba IIS nainstalována po instalaci rozhraní .NET Framework 1.1, můžete službu ASP.NET povolit spuštěním následujícího příkazu na příkazovém řádku:
  
**%SystemRoot%\\Microsoft.NET\\Framework\\v1.1.4322\\aspnet\_regiis.exe -i –enable**
  
Při používání novější verze rozhraní .NET Framework než 1.1 nahraďte v tomto příkazu příponu **-i** příponou **-ir**, aby nedošlo k obnovení stávajících mapování skriptů služby IIS.
  
#### Účet služby RMS vzdálené doménové struktury musí být přidán do místního kanálu rozšíření skupiny
  
Byla opravena chyba zabezpečení, která odstraní uživatele BUILTIN\\users ze seznamu řízení přístupu u kanálu rozšíření skupiny. Tím by mohlo dojít k narušení plánů rozšíření skupin v doménových strukturách. Tento problém vyřešíte následujícím postupem:
  
**Přidejte účet služby RMS do vzdálené doménové struktury.**  
1.  V Doménové\_struktuře\_1, kde Doménová\_struktura\_1 je kořenový cluster služby RMS v první doménové struktuře, přejděte do umístění inetpub\\wwwroot\\\_wmcs.
  
2.  Klepněte pravým tlačítkem myši na složku **GroupExpansion** a klepněte na příkaz **Vlastnosti**.
  
3.  V okně **GroupExpansion – vlastnosti** klepněte na kartu **Zabezpečení**, přidejte položku pro *Doménová\_struktura\_2\\Účet\_služby\_Rms* (například rmil31\\rmsvc), kde Doménová\_struktura\_2 je kořenový cluster služby RMS ve druhé doméně.
  
4.  Klepněte na tlačítko **OK**.
  
5.  Klepněte na tlačítko **Spustit**, zadejte příkaz **iisreset** a pak klepněte na tlačítko**OK**.
  
#### Upgrade rozhraní .NET Framework může způsobit ztrátu dat
  
Pokud je rozhraní .NET Framework (CLR) verze 1.1 upgradováno po instalaci a zajištění služby RMS, budou virtuální kořenové adresáře nastaveny na používání rozhraní .NET Framework verze 2.0. Pokud k této situaci dojde, nebudou do databáze protokolování zapisovány žádné informace. Tím dojde ke ztrátě dat. Proveďte jednu z následujících akcí:
  
-   Před instalací a zajištěním služby RMS upgradujte rozhraní .NET Framework.  
-   Po upgradu rozhraní .NET Framework obnovte virtuální kořenové adresáře tak, aby používaly verzi 1.1.
  
Změny dokumentace v této verzi  
------------------------------
  
Následuje seznam témat, která byla v této verzi změněna:
  
-   To Trust Passport-Based Rights Account Certificates (Nastavení důvěryhodnosti certifikátů účtů práv založených na službě Passport) ([http://go.microsoft.com/fwlink/?LinkId=70369](http://go.microsoft.com/fwlink/?linkid=70369)) (stránka může být v angličtině)  
-   Software Requirement for RMS (Softwarové požadavky pro službu RMS) ([http://go.microsoft.com/fwlink/?LinkId=70371](http://go.microsoft.com/fwlink/?linkid=70371)) (stránka může být v angličtině)  
-   How to Deploy the RMS Client (Způsob nasazení klienta RMS) ([http://go.microsoft.com/fwlink/?LinkId=70373](http://go.microsoft.com/fwlink/?linkid=70373)) (stránka může být v angličtině)  
-   RMS Command Prompt Installation (Instalace služby RMS z příkazového řádku) ([http://go.microsoft.com/fwlink/?LinkId=70374](http://go.microsoft.com/fwlink/?linkid=70374)) (stránka může být v angličtině)  
-   RMS Core Configuration Database Tables (Základní tabulky konfigurační databáze služby RMS) ([http://go.microsoft.com/fwlink/?LinkId=70375](http://go.microsoft.com/fwlink/?linkid=70375)) (stránka může být v angličtině)  
-   RMS Configuration Database Certification Tables (Základní tabulky certifikátů konfigurační databáze služby RMS) ([http://go.microsoft.com/fwlink/?LinkId=70376](http://go.microsoft.com/fwlink/?linkid=70376)) (stránka může být v angličtině)  
-   RMS Logging Database Tables (Tabulky databáze protokolování služby RMS) ([http://go.microsoft.com/fwlink/?LinkId=70377](http://go.microsoft.com/fwlink/?linkid=70377)) (stránka může být v angličtině)  
-   Evaluating Scaling Requirements (Vyhodnocení požadavků na škálování) ([http://go.microsoft.com/fwlink/?LinkId=70378](http://go.microsoft.com/fwlink/?linkid=70378)) (stránka může být v angličtině)  
-   Securing the RMS Deployment (Zabezpečení nasazení služby RMS) ([http://go.microsoft.com/fwlink/?LinkId=70379](http://go.microsoft.com/fwlink/?linkid=70379)) (stránka může být v angličtině)  
-   Enabling the Decommissioning Service (Povolení služby vyřazení z provozu) ([http://go.microsoft.com/fwlink/?LinkId=70380](http://go.microsoft.com/fwlink/?linkid=70380)) (stránka může být v angličtině)  
-   Planning for External RMS Users (Plánování pro externí uživatele služby RMS) ([http://go.microsoft.com/fwlink/?LinkId=70381](http://go.microsoft.com/fwlink/?linkid=70381)) (stránka může být v angličtině)  
-   Enabling RMS Server Support for Mobile Devices and Server Services (Povolení podpory serveru RMS pro mobilní zařízení a serverové služby) ([http://go.microsoft.com/fwlink/?LinkId=70382](http://go.microsoft.com/fwlink/?linkid=70382)) (stránka může být v angličtině)
  
#### Autorská práva
  
*Informace obsažené v tomto dokumentu představují aktuální názor společnosti Microsoft na problémy známé k datu vydání. Protože společnost Microsoft musí reagovat na měnící se podmínky trhu, nelze je považovat za závazek ze strany společnosti Microsoft, přičemž společnost Microsoft nemůže zaručit správnost informací zveřejněných po datu vydání.*
  
*Tento dokument je určen pouze pro informační účely. SPOLEČNOST MICROSOFT NEPOSKYTUJE NA INFORMACE UVEDENÉ V TOMTO DOKUMENTU ŽÁDNÉ ZÁRUKY, AŤ UŽ VÝSLOVNĚ UVEDENÉ, IMPLICITNĚ PŘEDPOKLÁDANÉ NEBO VYPLÝVAJÍCÍ ZE ZÁKONA.*
  
*Za splnění veškerých požadavků všech příslušných zákonů na ochranu autorských práv odpovídá uživatel. Bez předchozího písemného svolení společnosti Microsoft nesmí být žádná část tohoto dokumentu za žádným účelem reprodukována, ukládána, zaváděna do vyhledávácích systémů nebo přenášena jakoukoli formou (elektronicky, mechanicky, pomocí fotokopií, záznamů nebo jinak). Autorská práva nejsou tímto ustanovením dotčena.*
  
*Společnost Microsoft může vlastnit patenty, patentové přihlášky, chráněné známky, autorská práva nebo jiná práva k duševnímu vlastnictví týkající se předmětu tohoto dokumentu. Není-li v písemné licenční smlouvě společnosti Microsoft výslovně uvedeno jinak, nejsou předáním tohoto dokumentu poskytnuty žádné licence na takové patenty, chráněné známky, autorská práva nebo jiné duševní vlastnictví.*
  
*Není-li uvedeno jinak, jsou použité příklady společností, organizací, produktů, názvů domén, e-mailových adres, log, osob, míst a událostí fiktivní a nemají žádný skutečný nebo mlčky předpokládaný vztah ke skutečným společnostem, organizacím, produktům, názvům domén, e-mailovým adresám, logům, osobám, místům a událostem.*
  
*© 2006 Microsoft Corporation. Všechna práva vyhrazena.*
  
*Active Directory, Microsoft, MS-DOS, Visual Studio, Windows, Windows Server, SQL Server a Windows NT jsou registrované ochranné známky nebo ochranné známky společnosti Microsoft Corporation ve Spojených státech amerických a v dalších zemích.*
  
*Názvy skutečných společností a produktů, uvedené v tomto dokumentu, mohou být ochrannými známkami jejich příslušných vlastníků.*
