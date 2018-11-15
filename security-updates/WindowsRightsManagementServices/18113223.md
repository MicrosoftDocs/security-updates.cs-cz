---
TOCTitle: Provoz serveru RMS
Title: Provoz serveru RMS
ms:assetid: '1533426b-89c2-43e0-8068-ca97ddab8606'
ms:contentKeyID: 18113223
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc720205(v=WS.10)'
---

Provoz serveru RMS
==================

Provoz serveru RMS představuje úlohy správy prováděné po nasazení služby RMS v organizaci. Toto téma obsahuje informace, které vám usnadní správu serveru RMS, procedury běžných úloh správy, zdroje dalších informací a také doporučené postupy.

Obsah tématu

-   [Správa služby RMS](https://technet.microsoft.com/9b573c55-c14c-436c-b3c5-7ba445de1562)
-   [Postupy pro službu RMS...](https://technet.microsoft.com/82032075-f361-438f-a2c4-93ab29ae6cff)
-   [Informační zdroje služby RMS](https://technet.microsoft.com/d91221cf-e38e-4add-b7b9-50e63aad9a28)

Použitá terminologie
--------------------

**certifikace účtu**  
Proces, který spojí uživatelské účty s páry klíčů v certifikátu účtu práv.

<!-- -->

**služba certifikace účtu**  
Webová služba RMS, která vytváří a zajišťuje distribuci certifikátů účtu s právy. Viz také certifikace účtu.

<!-- -->

**služba aktivačního serveru proxy**  
Webová služba RMS, která podporuje aktivaci klientských počítačů služby RMS verze 1.0. Používá se pro předávání požadavků aktivací počítačů službě Microsoft Activation Service. Aktivační služba vytváří jedinečný bezpečnostní modul a odpovídající certifikát počítače RMS pro klientský počítač, který aktivační služba serveru proxy na serveru RMS následně předává zpět klientovi, který požadavek odeslal. Viz také bezpečnostní modul.

<!-- -->

**služba správy**  
Webová služba RMS, která je hostitelem webu pro správu. Služba umožňuje spravovat službu RMS a aktualizovat konfigurační databázi pro cluster.

<!-- -->

**manifest aplikace**  
Dokument XML, který popisuje moduly přidružené k aplikaci s podporou správy přístupových práv a aplikace, které mohou být spuštěny v prostředí aplikace. Jakákoli aplikace provádějící zápis do rozhraní API klienta služby RMS za účelem vytvoření nebo použití informací chráněných správou přístupových práv musí při spuštění poskytovat manifest.

<!-- -->

**atribut**  
Ve službě Active Directory, vlastnost objektu. Pro každou třídu objektu schéma definuje, které atributy musí instance třídy mít a které dodatečné atributy může mít.

<!-- -->

**vazba**  
Mechanismus, který používá práva v systému RMS. V tomto mechanismu klient služby RMS ověřuje podmínky licence k použití s právy, které byly vyžádány. Jsou-li tyto podmínky splněny, práva jsou udělena.

<!-- -->

**certifikát**  
Digitální dokument, který se obvykle používá pro ověření a zabezpečení informací v otevřených sítích. Certifikát bezpečně váže veřejný klíč na entitu, která vlastní příslušný soukromý klíč. Certifikáty jsou digitálně podepsány vydávajícím certifikačním úřadem (CA) a mohou být vydány pro uživatele, počítač nebo službu. Viz také soukromý klíč nebo veřejný klíč.

<!-- -->

**zápis klienta**  
Proces vytvoření klientského certifikátu pro poskytování licencí, který umožňuje počítači nebo zařízení uživatele vytvořit licenci k publikování.

<!-- -->

**klientský certifikát pro poskytování licencí**  
Certifikát vytvořený serverem RMS a umístěný v klientských počítačích služby RMS, který umožňuje uživatelům publikovat chráněný obsah v režimu offline bez nutnosti připojení k síti s podporou služby RMS. Klientský certifikát pro poskytování licencí obsahuje klíč, který klient služby RMS používá k digitálnímu podepsání licencí k publikování.

<!-- -->

**podmínka**  
Sada omezujících podmínek a parametrů, které jsou součástí skupiny práv shromážděných do licence k publikování. Jsou vynuceny v okamžiku spotřeby. Časová podmínka je běžná podmínka, která uživateli umožňuje nastavit datum vypršení platnosti u informací chráněných službou RMS.

<!-- -->

**konfigurační databáze**  
Databáze obsahující konfigurační informace služby RMS pro server nebo cluster.

<!-- -->

**využití obsahu**  
Dešifrování a uplatnění práv využití na část chráněného obsahu.

<!-- -->

**klíč obsahu**  
Klíč používaný k šifrování a dešifrování chráněného obsahu při publikování a využití. Také se nazývá symetrický klíč. Služba RMS používá 128bitové klíče obsahu AES.

<!-- -->

**vlastník obsahu**  
Osoba nebo organizace, která zřizuje zásady přístupu pro chráněný obsah.

<!-- -->

**dešifrování**  
Proces, kterým se umožní číst šifrovaná data převedením šifrovaného textu na normální text.

<!-- -->

**digitální podpis**  
Způsob svázání identity autorů zprávy, souboru nebo jiných digitálně kódovaných informací s těmito údaji. Digitální podpis informací znamená převedení informací a určitých tajných informací vlastněných odesilatelem do značky nazývané podpis. Digitální podpisy se používají v prostředí s veřejnými klíči a nabízí ověřovací a integrační služby.

<!-- -->

**služba DRMRemote**  
Webová služba RMS, která vystavuje služby prostřednictvím rozhraní .NET Remoting a slouží ke komunikaci mezi různými servery RMS.

<!-- -->

**šifrování**  
Proces převedení informací do formy, kterou může číst pouze určitý příjemce. Šifrování je účinný způsob zabezpečení informací. Pro dešifrování souboru, který byl zašifrován, musí mít příjemce tajný klíč nebo heslo, které jej přeloží. Viz také šifrování veřejným klíčem.

<!-- -->

**zápis**  
Proces, při kterém server kořenové certifikace získá certifikát serveru pro poskytování licencí podepsaný službou Microsoft Enrollment Services.

<!-- -->

**požadavek na zápis**  
Požadavek odeslaný serverem kořenové certifikace služby RMS službě Microsoft Enrollment Services.

<!-- -->

**vyloučení**  
Proces používaný serverem RMS k odmítnutí licence k použití klientovi na základě zásady vyloučení. Viz také seznam vyloučení.

<!-- -->

**seznam vyloučení**  
Seznam zaregistrovaných objektů, kterým má služba správy licencí RMS odmítnout licence.

<!-- -->

**zásada vyloučení**  
Nastavení v konfigurační databázi služby RMS, které řídí způsob vyloučení použitý v organizaci.

<!-- -->

**jazyk XrML (eXtensible rights Markup Language)**  
Formát XML používaný službou RMS pro všechny podporované licence: certifikáty počítače, certifikáty účtů práv, klientské certifikáty pro poskytování licencí, licence k použití, licence k publikování a certifikáty serveru pro poskytování licencí. Jedná se o dokumenty, které určují zásady služby RMS použité u chráněného obsahu.

<!-- -->

**licence k vystavování**  
Data, která určují uplatněnou zásadu správy přístupových práv upravující použití chráněného obsahu.

<!-- -->

**cluster správy licencí**  
Jeden nebo více serverů, na kterých je spuštěna služba správy licencí a služba publikování RMS mimo cluster kořenové certifikace. Tyto servery používají společnou databázi a adresu URL připojení, a pokud se používá více než jeden server, měly by být nasazeny za softwarový nebo hardwarový modul pro rozložení zátěže. Na rozdíl od clusteru certifikace nebo kořenového clusteru nemohou servery RMS v clusteru správy licencí provádět certifikaci uživatelů.

<!-- -->

**server správy licencí**  
Server se spuštěnou službou správy licencí a službou publikování RMS mimo cluster kořenové certifikace.

<!-- -->

**služba správy licencí**  
Webová služba RMS, která vydává licence k použití.

<!-- -->

**bezpečnostní modul**  
Softwarový modul odpovědný za ověření platného použití chráněného obsahu, šifrování a dešifrování informací a ochranu důvěryhodného zpracování softwaru před úpravami a sledováním. Také se nazývá zabezpečené úložiště.

<!-- -->

**služba protokolování**  
Služba naslouchání RMS, která přenáší zaznamenaná data z fronty zpráv do databáze protokolování pro server nebo cluster RMS.

<!-- -->

**aktivace počítače**  
Proces získání jedinečného bezpečnostního modulu a certifikátu počítače pro počítač se službou RMS verze 1.0. Ve verzi RMS 1.0 s aktualizací SP1 představuje aktivace počítače proces získání certifikátu počítače pro každého uživatele tohoto počítače.

<!-- -->

**manifest**  
Podepsaný dokument XML identifikující knihovny nebo programy, které mohou, nemohou či smějí být zavedeny do prostoru zpracování aplikace.

<!-- -->

**služba Microsoft Activation Service**  
Webová služba, jejíž hostitelem je společnost Microsoft, která jako odpověď na požadavky klientů RMS vydává certifikáty počítače a bezpečnostní moduly RMS verze 1.0.

<!-- -->

**služba Microsoft Enrollment Services**  
Webová služba, jejíž hostitelem je společnost Microsoft, která v rámci implementace služby RMS vydává certifikát serveru pro poskytování licencí pro server kořenové certifikace.

<!-- -->

**předběžná certifikace**  
Funkce certifikační služby RMS, která umožňuje aplikaci požádat server RMS jménem uživatele o certifikát účtu práv. Certifikáty účtu práv získané pouze použitím předběžné certifikace obsahují veřejný klíč uživatele.

<!-- -->

**zaregistrovaný objekt**  
Entita (například uživatel, skupina nebo správce chráněného obsahu), která má určenou roli ve schématu zabezpečení RMS a vůči které jsou objekty zabezpečeny.

<!-- -->

**soukromý klíč**  
Tajná polovina páru šifrovacích klíčů, který se používá s algoritmem veřejného klíče. Soukromé klíče se obvykle používají k dešifrování klíče symetrické relace, digitálnímu podpisu dat nebo dešifrování dat, která byla šifrována odpovídajícím veřejným klíčem. Viz také veřejný klíč nebo šifrování veřejným klíčem.

<!-- -->

**zajištění**  
Konfigurace serveru RMS pro práci v organizaci.

<!-- -->

**veřejný klíč**  
Netajná polovina páru šifrovacích klíčů, který se používá s algoritmem veřejného klíče. Veřejné klíče se obvykle používají při šifrování klíče relace, ověření digitálního podpisu nebo šifrování dat, které lze dešifrovat s příslušným soukromým klíčem. Viz také soukromý klíč nebo šifrování veřejným klíčem.

<!-- -->

**šifrování veřejným klíčem**  
Způsob šifrování, který používá dva šifrovací klíče, které spolu matematicky souvisí. Jeden klíč se nazývá soukromý klíč a drží se v tajnosti. Druhý se nazývá veřejný klíč a předává se všem možným korespondentům. V obvyklém případě používá odesilatel veřejný klíč příjemce pro šifrování zprávy. Pouze příjemce má příslušný soukromý klíč pro dešifrování zprávy. Složitost vztahu mezi veřejným a soukromým klíčem, za předpokladu, že jsou klíče dostatečně dlouhé, znamená, že je výpočetně nemožné odvodit jeden od druhého. Také nazýváno asymetrické šifrování. Viz také soukromý klíč nebo veřejný klíč.

<!-- -->

**licence k publikování**  
Licence vytvořená při publikování obsahu chráněného správou přístupových práv. Kromě jiného určuje, kdo má přístup k obsahu, jaká práva jsou udělena a za jakých podmínek lze získat k obsahu přístup. Také se nazývá licence k vystavování.

<!-- -->

**služba publikování**  
Služba RMS, která podepisuje licence k publikování a vydává certifikáty pro poskytování licencí. Viz také klientský certifikát pro poskytování licencí nebo licence k publikování.

<!-- -->

**RAC**  
Viz definice certifikátu účtu práv.

<!-- -->

**odvolání**  
Proces, při kterém jsou vypsány entity s neplatnými licencemi.

<!-- -->

**seznam odvolání**  
Dokument založený na technologii XrML, který obsahuje seznam certifikátů a licencí odvolaných vystavitelem. Viz také odvolání.

<!-- -->

**právo**  
Akce povolená určitým uživatelům pro obsah, který je chráněn technologií RMS. Tato práva lze dále omezit použitím podmínek.

<!-- -->

**Certifikát účtu práv**  
Certifikát, který pomocí certifikátu počítače získaný při aktivaci služby RMS zajišťuje vazbu uživatelského účtu a klíče na určitý počítač nebo skupiny počítačů. Komponenty certifikátu zajišťují uživatelům možnost využití chráněného obsahu. Také se nazývá certifikát identity skupiny (GIC) v sadě RMS SDK.

<!-- -->

**správa práv**  
Technologie, která umožňuje trvalou ochranu digitálních dat použitím šifrování, certifikátů a ověření. Ověření příjemci nebo uživatelé musí získat licenci. která jim umožní využívat chráněné soubory v souladu s právy nebo obchodními pravidly, které určil vlastník obsahu.

<!-- -->

**klient služby správy přístupových práv**  
Sada rozhraní API služby RMS, která musí být instalována na všech klientských počítačích v systému RMS. To je základní předpoklad pro aktivaci počítače, který je vyžadován při použití aplikací s podporou správy přístupových práv.

<!-- -->

**šablona zásad práv**  
Popisuje standardní sadu uživatelů, práv a podmínek, které lze uplatnit na obsah chráněný správou přístupových práv. Pokud uživatel uplatní šablonu zásad práv na část obsahu, práva a podmínky popsané v šabloně se stanou součástí licence k publikování.

<!-- -->

**aktivace RMS**  
Proces umístění bezpečnostního modulu do počítače koncového uživatele u služby RMS verze 1.0. Tuto funkci zajišťuje výhradně aktivační služba RMS a je nezbytná pro použití technologie RMS. U služby RMS 1.0 s aktualizací SP1 se jedná o proces získání certifikátu počítače pro uživatele tohoto počítače, přičemž není vyžadováno připojení k aktivační službě RMS. Také se označuje jako aktivace.

<!-- -->

**služba certifikace RMS**  
Webová služba, jejíž hostitelem je společnost Microsoft, která vydává uživatelům certifikáty účtů práv na základě jejich pověření Microsoft .NET Passport.

<!-- -->

**klient služby RMS**  
Sada rozhraní API služby RMS, která musí být instalována na všech klientských počítačích v systému RMS. To je základní předpoklad pro aktivaci počítače, který je vyžadován při použití aplikací s podporou správy přístupových práv.

<!-- -->

**certifikát počítače RMS**  
Certifikát, který je při aktivaci RMS uložen do počítače koncového uživatele. Veřejný klíč v tomto certifikátu se používá k zašifrování soukromého klíče uživatele obsaženého v certifikátech účtů práv uživatele.

<!-- -->

**aplikace s podporou služby RMS**  
Aplikace, která byla použitím sady SDK Služby správy přístupových práv rozšířena tak, aby umožňovala uživatelům určit práva přidruženého obsahu, který vytvořili.

<!-- -->

**počítač s podporou služby RMS**  
Počítač s instalovanou komponentou klienta RMS, který prošel aktivací počítače RMS a může tedy zpracovávat obsah chráněný službou RMS.

<!-- -->

**obsah chráněný službou RMS**  
Digitální informace, které jsou chráněné technologií RMS.

<!-- -->

**cluster kořenové certifikace**  
Jeden nebo více serverů v implementaci služby RMS, na kterém jsou spuštěny služby správy, zápisu, certifikace účtů, aktivačního serveru proxy, správy licencí a publikací. Tyto servery používají společnou databázi a adresu URL připojení a lze je implementovat za softwarový nebo hardwarový modul pro rozložení zátěže. Na jednu síť Active Directory může být pouze jeden cluster kořenové certifikace.

<!-- -->

**server kořenové certifikace**  
Primární server v implementaci služby RMS, na kterém jsou spuštěny služby správy, zápisu, certifikace účtů, aktivačního serveru proxy, správy licencí a publikací. Na jednu síť Active Directory může být pouze jeden server kořenové certifikace.

<!-- -->

**kořen důvěryhodnosti**  
Důvěryhodná entita, která poskytuje základ pro zřízení vztahu důvěryhodnosti jiných certifikátů. Všichni poskytovatelé certifikátů a koncoví uživatelé musí tomuto kořenu důvěřovat.

<!-- -->

**ID zabezpečení (SID)**  
Struktura dat systému Windows, která identifikuje každého uživatele, skupinu a účet počítače systému Windows. Pro každý účet v síti je při prvním vytvoření vydán jedinečný identifikátor SID. Vnitřní procesy v systému Windows se namísto ke jménu uživatele nebo názvu skupiny účtu vztahují k identifikátoru účtu SID.

<!-- -->

**certifikát serveru pro poskytování licencí**  
Certifikát, který vytváří přístupová pověření serveru RMS a stanovuje jej platnou certifikační službou a službou správy licencí a umožňuje její spuštění. Certifikát pro poskytování licencí obsahuje veřejný klíč, který se používá k zašifrování klíčů obsahu v licencích k publikování.

<!-- -->

**serverová služba**  
Webová služba RMS, kterou má používat jiná služba.

<!-- -->

**spojovací bod služby (SCP, service connection point)**  
Objekt služby Active Directory, který odkazuje na adresu URL clusteru kořenového certifikátu nasazení služby RMS. Klient služby RMS používá tyto informace k vyhledání služeb RMS.

<!-- -->

**dílčí zápis**  
Část procesu zajišťování pro server správy licencí, v rámci kterého server získá certifikát serveru pro poskytování licencí od clusteru kořenové certifikace.

<!-- -->

**požadavek dílčího zápisu**  
Požadavek odeslaný serverem správy licencí clusteru kořenové certifikace pro certifikát serveru pro poskytování licencí.

<!-- -->

**služba dílčího zápisu**  
Webová služba RMS na serveru kořenové certifikace, která odpovídá na požadavky na certifikáty serveru pro poskytování licencí, jež jsou odeslány serverům správy licencí při operaci zajišťování.

<!-- -->

**superuživatel**  
Člen skupiny superuživatelů.

<!-- -->

**skupina superuživatelů**  
Volitelná administrativně definovaná skupina uživatelů pro jednotlivé clustery služby RMS, kterým server RMS přidělí při otevření obsahu publikovaného tímto serverem licence vlastníků.

<!-- -->

**licence k použití**  
Licence obsahující práva a podmínky, za kterých může koncový uživatel používat chráněný obsah. Také se nazývá licence koncového uživatele (EUL, end-user license).
