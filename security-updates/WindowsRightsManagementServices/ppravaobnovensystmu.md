---
TOCTitle: Příprava obnovení systému
Title: Příprava obnovení systému
ms:assetid: '885c047f-1e3b-4bf5-8248-3a4505759cbb'
ms:contentKeyID: 18113413
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747659(v=WS.10)'
---

Příprava obnovení systému
=========================

Selhání jakékoli součásti systému služby RMS, včetně připojení k Internetu nebo intranetu využívaného serverem RMS, serveru certifikace, jakéhokoli serveru správy licencí s dílčím zápisem nebo databázových serverů, které jsou hostiteli konfiguračních databází služby RMS, může způsobit neočekávaný výpadek služby. Při instalaci systému služby RMS je důležité zvážit možný vliv případného výpadku služby RMS na systémy IT a citlivá data a připravit co nejrychlejší obnovení dané součásti.

Selhání databázových serverů, které jsou hostiteli konfiguračních databází služby RMS, by mohlo přímo znemožnit nepřetržitý přístup k informacím chráněným službou RMS. Tato část je věnována důležitým aspektům a faktorům přípravy obnovení systému spojeného se službou RMS, včetně následujících součástí:

-   [Připojení k Internetu](#bkmk_1)
-   [Připojení k intranetu](#bkmk_2)
-   [Služby certifikace a správy licencí](#bkmk_3)
-   [Databázové servery](#bkmk_4)
-   [Služba Active Directory](#bkmk_5)

<span id="BKMK_1"></span>
Připojení k Internetu
---------------------

V případě zápisu online vyžaduje server RMS během zajišťování připojení k Internetu, aby mohl získat certifikát serveru pro poskytování licencí a zajistit jeho každoroční obnovení. Jakmile se v daném roce blíží datum obnovení, upozorní server certifikace na nutnost obnovení certifikátu zaprotokolováním událostí do systémového protokolu událostí. Události jsou zaprotokolovány měsíc před datem vypršení platnosti certifikátu serveru pro poskytování licencí (ID události 16), týden před datem vypršení platnosti tohoto certifikátu (ID události 17) a v den vypršení jeho platnosti (ID události 18). Na blížící se konec platnosti certifikátu serveru pro poskytování licencí vás také upozorní webová stránka Globální správa služby RMS na webu pro správu této služby. Pokud používáte sadu RMS Management Pack pro správce Microsoft Operations Manager (MOM), budou události vypršení platnosti aktivovat výstrahu. Jestliže na serveru RMS není připojení k Internetu k dispozici, nelze certifikát serveru pro poskytování licencí obnovit na webu pro správu služby RMS pomocí tlačítka **Obnovit** a aktualizovaný certifikát je nutné vyžádat prostřednictvím procesu zápisu offline.

Certifikát serveru pro poskytování licencí je vhodné obnovit dostatečně dlouho před datem vypršení platnosti, aby nedošlo ke komplikacím, pokud by v okamžiku vypršení platnosti certifikátu nebylo k dispozici připojení k Internetu. Server RMS nemůže zajišťovat služby RMS bez platného certifikátu serveru pro poskytování licencí, což znamená, že uživatelé nemohou publikovat informace chráněné službou RMS ani získat licence k použití a certifikáty účtů práv nutné ke zobrazení informací chráněných službou RMS. Uživatelé, kteří již dříve získali licence k použití a certifikáty účtů práv na části obsahu chráněného službou RMS mohou i nadále získávat k těmto informacím přístup, dokud nevyprší platnost daných licencí nebo certifikátů.

<span id="BKMK_2"></span>
Připojení k intranetu
---------------------

Služba RMS představuje technologii založenou na klientech a serverech, která je závislá na propojené infrastruktuře. Bez fungující intranetové sítě se servery RMS nemohou připojit k požadovaným službám v rámci podniku ani k uživatelům, pro které zajišťují služby. Bez připojení k intranetu nemohou uživatelé ze serverů RMS získávat certifikáty účtů práv, klientské certifikáty pro poskytování licencí ani licence k použití.

Jako nejvhodnější je organizacím doporučeno zvážit redundantní architektury směrování a odkazy na převzetí služeb ze vzdálených webů na weby serverů RMS.

Jakmile uživatel pro svůj počítač získá klientský certifikát pro poskytování licencí, může publikovat informace chráněné službou RMS v režimu offline, jestliže není k dispozici přístup k serveru RMS. Některé e-mailové aplikace s podporou služby RMS byly nakonfigurovány na automatické stahování licencí k použití pro příslušné e-mailové zprávy chráněné službou RMS při synchronizaci poštovní schránky, takže uživatel může tyto zprávy číst, přestože připojení k intranetu již není k dispozici.

<span id="BKMK_3"></span>
Služby certifikace a správy licencí
-----------------------------------

Systém služby RMS je velmi závislý na dvou virtuálních adresářích v rámci Internetové informační služby (IIS) 6.0. Jedná se o služby certifikace a správy licencí. Uvedené služby umožňují uživatelům a jejich počítačům zápis do prostředí služby RMS a k aplikacím s podporou služby RMS za účelem přístupu k informacím chráněným službou RMS a jejich publikování. Jestliže tyto služby přestanou být k dispozici, bude uživatelům odmítnuta obsluha, dokud nedojde k obnovení služeb.

Chcete-li se připravit na možný výpadek služby, zvažte vytvoření clusterů serverů certifikace a serverů správy licencí s dílčím zápisem, aby selhání žádného uzlu v clusteru neovlivnilo dostupnost služby.

Doporučeným postupem je navýšení kapacity v clusterech tak, aby chyby jakéhokoli uzlu neovlivnily celkový výkon. Při instalaci prvního serveru certifikace a každého serveru správy licencí s dílčím zápisem nebo prvního serveru správy licencí s dílčím zápisem v clusteru si pečlivě poznamenejte možnosti konfigurace a data zadaná během zajišťování.

<span id="BKMK_4"></span>
Databázové servery
------------------

Nejdůležitější součásti systému služby RMS představují databázové servery s konfiguračními databázemi. Každý server RMS nebo cluster serverů RMS využívá databáze k ukládání informací o konfiguraci a protokolování. Informace o konfiguraci jsou pro provoz služby RMS zásadní. V těchto databázích je uložen certifikát serveru pro poskytování licencí, vytvořené šablony zásad služby RMS a seznam uživatelů zapsaných v systému služby RMS. Jestliže server RMS nepoužívá hardwarový modul zabezpečení, obsahují také soukromý a veřejný klíč serveru RMS. Pomocí záloh databází služby RMS je možné obnovit předchozí instalaci této služby na novém serveru a znovu vytvořit její systém. Vliv výpadku databáze se liší podle konkrétní databáze. Následující seznam popisuje vliv selhání jednotlivých databází:

-   **Konfigurační databáze.** Pokud během provozu serveru RMS přestane být tato databáze dostupná, mohou jednotlivé služby RMS i nadále pracovat, protože služba RMS ukládá požadované informace do místní mezipaměti. Jestliže však dojde k události, která vyžaduje interakci mezi službou RMS a konfigurační databází (jako je například zápis nového uživatele), zjistí služba RMS chybu a nový uživatel nebude moci pracovat s obsahem chráněným službou RMS. Dojde-li k operaci, která na serveru RMS způsobí odstranění uložených informací z mezipaměti (například restartování služby IIS nebo plánované obnovení místní mezipaměti), přestane služba RMS pracovat. Server RMS se nevrátí ke standardnímu provozu, dokud nebude konfigurační databáze znovu k dispozici.

    Jestliže je konfigurační databáze poškozená nebo trvale nedostupná, přestanou servery RMS pracovat.

-   **Databáze adresářových služeb.** Obsahuje informace z mezipaměti týkající se názvů skupin a souvisejících podrobností o členství získané ze serveru globálního katalogu. V případě, že tato tabulka není k dispozici po krátké časové období, nedojde ke zjevnému omezení služeb RMS. Hlavním účelem této databáze je zajišťování redundance dat a omezování zatížení služeb pro server globálního katalogu.

-   **Databáze protokolování.** Jestliže je na serveru RMS povoleno protokolování, bude se příslušný protokol ukládat právě do této databáze. Pokud není k dispozici, budou se položky protokolu hromadit ve službě Řízení front zpráv (označované také zkratkou MSMQ) na serveru RMS a budou zaplňovat veškerý volný prostor disku (není-li toto chování znemožněno konfigurací).

Doporučeným postupem je seskupit databázové servery do clusteru a zajistit tak aktivní ochranu převzetím služeb při selhání. Zároveň je vhodné pravidelně zálohovat databáze serverů a clusterů certifikace služby RMS i serverů a clusterů správy licencí.

Dalším doporučeným postupem je použití dodávání protokolu transakcí jako prostředku údržby stále připravené záložní databáze. Přestože tento postup může vyžadovat doplňkový hardware, umožňuje organizacím rychlejší obnovení databází. Oddělení IT společnosti Microsoft uvedený způsob implementovalo pro obnovení konfigurační databáze služby RMS. Chcete-li tento krok provést, vyberte při zajišťování služby RMS virtuální název SQL. Virtuální název SQL umožňuje namapovat skutečný název SQL pomocí služby DNS (Domain Name System). Pokud přestane pracovat původní SQL Server, bude možné snadno přepnout na záložní SQL Server změnou mapování názvu DNS z původního serveru na záložní. Další informace o interní implementaci tohoto řešení ve společnosti Microsoft Corporation získáte v případové studii této společnosti na [webu](http://go.microsoft.com/fwlink/?linkid=42070) (http://go.microsoft.com/fwlink/?LinkId=42070).

<span id="BKMK_5"></span>
Služba Active Directory
-----------------------

Služba RMS je na službě Active Directory závislá, protože využívá dvě důležité služby: ověřování uživatelů a službu globálního katalogu. Jestliže služba Active Directory nebude k dispozici, nebude možné ověřování uživatelů a uživatelé a jejich počítače se nebudou moci zapsat v systému služby RMS. Získání certifikátu účtu práv vyžaduje kanál certifikace a tento kanál vyžaduje ověřování. Jakmile uživatel obdrží certifikát účtu práv, může získat licence k použití bez dalšího ověřování, protože kanál správy licencí je ve výchozím nastavení anonymní.

Vzhledem k tomu, že podnikové entity určují přístup jednotlivců k informacím chráněným službou RMS prostřednictvím členství ve skupinách ve službě Active Directory, výpadek této služby by uživatelům znemožnil získání licencí k použití. Ve výchozím nastavení jsou informace o členství ve skupinách uloženy v mezipaměti serveru RMS po dobu 15 minut, takže dočasný výpadek služby globálního katalogu lze tolerovat. Jestliže chcete zvýšit nebo snížit dobu mezi jednotlivými aktualizacemi mezipaměti, můžete změnit klíč registru, kterým je řízena daná doba platnosti. Další informace získáte v této sadě dokumentace v části Změna nastavení mezipaměti služby Active Directory tématu Provoz serveru RMS.
