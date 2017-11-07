---
TOCTitle: 'Nejčastější dotazy týkající se služby RMS: Témata zabezpečení'
Title: 'Nejčastější dotazy týkající se služby RMS: Témata zabezpečení'
ms:assetid: 'ff433834-79aa-481f-bd39-3393be12a26f'
ms:contentKeyID: 18113511
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747757(v=WS.10)'
---

Nejčastější dotazy týkající se služby RMS: Témata zabezpečení
=============================================================

Nejčastější dotazy týkající se zabezpečení služby RMS
-----------------------------------------------------

-   [Co je účet superuživatelů?](#bkmk_43)
-   [Představuje služba RMS řešení zabezpečení?](#bkmk_44)
-   [Jakým způsobem lze příjemcům znemožnit posunutí hodin v klientských počítačích zpět za účelem prodloužení přístupu k dokumentu chráněnému právy po vypršení platnosti příslušné licence k použití?](#bkmk_45)
-   [Mohou členové skupiny Domain Admins číst dokumenty určené pro jiného uživatele ve stejné doméně?](#bkmk_46)
-   [Každý bezpečnostní modul může ověřit každý certifikát nebo licenci generované v rámci systému jako by pocházely od služby zaregistrované u společnosti Microsoft. Proti jakému ohrožení je tato ochrana zaměřena?](#bkmk_47)
-   [Pokud nějaký uživatel dokáže otevřít některý dokument násilím, bude moci pomocí příslušného klíče otevřít také jiné dokumenty?](#bkmk_48)
-   [Jsou některé části klíčů díky omezením exportu vztahujícím se na technologie šifrování zveřejněny mimo podnik, který je nasadil?](#bkmk_49)
-   [Jakým způsobem je útočníkům se zlými úmysly znemožněno vzdálené zapnutí funkce vyřazení z provozu?](#bkmk_50)
-   [Může uživatel vytvořit kopii obrazovky s obsahem chráněným právy?](#bkmk_51)
-   [Mohou správci, kteří zálohují soubory spojené se službou RMS, získat přístup k obsahu chráněnému právy?](#bkmk_52)
-   [Obsahuje stránkovací soubor, který používá systém Windows, v určitém okamžiku nešifrovaný obsah, čímž by teoreticky mohlo dojít ke zveřejnění obsahu?](#bkmk_53)
-   [Je možné omezit přístup konkrétních správců k různým funkcím správy služby RMS?](#bkmk_54)
-   [Může služba RMS chránit jednotlivé dokumenty na pevném disku uživatele nebo ve sdílené složce bezprostředně po jejich vytvoření?](#bkmk_55)
-   [V případě otevření souboru jsou šifrovány automaticky ukládané a dočasné soubory?](#bkmk_56)
-   [V doručeném e-mailu chráněném právy je připojena příloha. Tuto přílohu je možné uložit, přestože poštu pravděpodobně uložit nelze. Došlo k narušení služby RMS?](#bkmk_562)

<span id="BKMK_43"></span>
#### Co je účet superuživatelů?

Sužba RMS podporuje speciální skupinu superuživatelů (Super Users), která má právo úplného řízení veškerého obsahu chráněného právy. Členům skupiny superuživatelů jsou udělena úplná práva vlastníků ve všech licencích k použití jim vydaných clusterem služby RMS, u kterého je tato skupina nakonfigurována. To znamená, že členové této skupiny mohou dešifrovat libovolné chráněné soubory a odstraňovat jejich ochranu. Člen této skupiny může například odstranit ochranu ze souborů publikovaných bývalým zaměstnancem, aby mohl dané soubory publikovat a spravovat nový vlastník.

<span id="BKMK_44"></span>
#### Představuje služba RMS řešení zabezpečení?

Ne, služba RMS není řešením zabezpečení. V případě použití s aplikací s podporou služby RMS, jako je sada Office 2007, může být považována za řešení pro vynucení zásad. Jestliže uživatel není oprávněn zobrazit určitá data, mohl by se pokusit o rozšifrování násilím. Přestože je šifrování silné, může být stejně jako všechna schémata softwarového šifrování rozšifrováno. Pokud však uživatel získal právo k zobrazení dat, mohl by je zkopírovat ručně nebo vytvořit digitální obrázek a poskytnout tyto informace neoprávněným uživatelům.

<span id="BKMK_45"></span>
#### Jakým způsobem lze příjemcům znemožnit posunutí hodin v klientských počítačích zpět za účelem prodloužení přístupu k dokumentu chráněnému právy po vypršení platnosti příslušné licence k použití?

Služba RMS zjistí, zda byly hodiny v systému klienta posunuty vpřed nebo vzad, a znemožní uživateli obsah využít. Služba RMS navíc zjistí, zda je mezi serverem RMS a klientem zjevný časový rozdíl.

<span id="BKMK_46"></span>
#### Mohou členové skupiny Domain Admins číst dokumenty určené pro jiného uživatele ve stejné doméně?

Členové skupiny Domain Admins mohou číst chráněný obsah pro určitý uživatelský účet, jestliže jsou členy skupiny superuživatelů služby RMS nebo jestliže daný uživatelský účet zosobňují. Vzhledem k tomu, že členové skupiny Domain Admins řídí uživatelské účty domény, není možné žádným způsobem zmírnit riziko v případě situace s nedůvěryhodným členem této skupiny.

Členy skupiny Domain Admins je doporučeno přidávat do skupiny superuživatelů v případě, že potřebují přístup k obsahu chráněnému právy. Pokud je licence udělena členovi skupiny superuživatelů, bude do protokolu událostí aplikací na serveru RMS zaprotokolována událost s ID 49. Událost s ID 49 uvádí: **Byla udělena licence uživateli ze skupiny Super Users. E-mailová adresa uživatele: &lt;alias uživatele&gt;,** kde hodnota **alias uživatele** je nahrazena e-mailovým účtem uživatele.

Stejně jako u ostatních skupin, pomocí nichž je omezen přístup k prostředkům, byste měli definovat výstrahy a provádět kontroly zabezpečení. Tímto postupem můžete uživatelům zabránit připojit se ke skupině superuživatelů bez oprávnění.

<span id="BKMK_47"></span>
#### Každý bezpečnostní modul může ověřit každý certifikát nebo licenci generované v rámci systému jako by pocházely od služby zaregistrované u společnosti Microsoft. Proti jakému ohrožení je tato ochrana zaměřena?

Jestliže by nebylo možné ověřit integritu certifikátů, mohl by některý uživatel zfalšovat certifikát účtu práv vydaný jinému uživateli a získat licenci k použití pro obsah nebo vytvořit aplikaci, která by z dokumentu ochranu odebrala.

<span id="BKMK_48"></span>
#### Pokud nějaký uživatel dokáže otevřít některý dokument násilím, bude moci pomocí příslušného klíče otevřít také jiné dokumenty?

Každá část obsahu chráněného právy je šifrována jiným náhodně generovaným symetrickým klíčem. Proto je klíč pro každý dokument jedinečný a neumožňuje rozšifrování ostatních dokumentů.

<span id="BKMK_49"></span>
#### Jsou některé části klíčů díky omezením exportu vztahujícím se na technologie šifrování zveřejněny mimo podnik, který je nasadil?

Aplikace zapsané u kořenové autority společnosti Microsoft podléhají kořenové autoritě pro podpis klíčů této společnosti, ale dále nedochází ke zveřejnění žádných dalších klíčů společností Microsoft ani prostřednictvím nasazení zákazníka.

<span id="BKMK_50"></span>
#### Jakým způsobem je útočníkům se zlými úmysly znemožněno vzdálené zapnutí funkce vyřazení z provozu?

Útočník by musel získat pověření uživatelského účtu s právy pro správu clusteru služby RMS. Ve výchozím nastavení je rozhraní pro správu služby RMS k dispozici pouze místně na serveru RMS. Závažnost rizika zmírníte, pokud zajistíte, že se toto nastavení nezmění, protokol RDP (Remote Desktop Protocol) zůstane zakázán a server bude fyzicky zabezpečen.

<span id="BKMK_51"></span>
#### Může uživatel vytvořit kopii obrazovky s obsahem chráněným právy?

Jestliže jsou práva služby RMS nastavena na zákaz funkce kopírování, je službou RMS klávesová zkratka ALT+PRINT SCREEN systému Windows zakázána. V prostředí se stolními počítači bez správy by však uživatel mohl vytvořit snímek obsahu pomocí produktů od jiných společností než Microsoft.

<span id="BKMK_52"></span>
#### Mohou správci, kteří zálohují soubory spojené se službou RMS, získat přístup k obsahu chráněnému právy?

Ne, mohou provést zálohování, ale přístup jim nebyl udělen.

<span id="BKMK_53"></span>
#### Obsahuje stránkovací soubor, který používá systém Windows, v určitém okamžiku nešifrovaný obsah, čímž by teoreticky mohlo dojít ke zveřejnění obsahu?

Jakmile klient RMS odešle dešifrovaný obsah zpět aplikaci, mohl by se tento obsah zobrazit ve stránkovacím souboru. Část doporučení pro vývoj aplikací služby RMS v sadě SDK Služby správy přístupových práv (RMS) obsahuje kroky, které uvedené chování znemožňují. Riziko takové možnosti však závisí na aplikaci s podporou služby RMS.

<span id="BKMK_54"></span>
#### Je možné omezit přístup konkrétních správců k různým funkcím správy služby RMS?

Ano, ve službě Active Directory můžete vytvořit různé skupiny správců služby RMS, přidat uživatele a potom vytvořit odpovídající seznamy řízení přístupu (ACL) pro stránky správy. Výchozí konfigurace seznamů řízení přístupu pro webovou stránku správy služby RMS například určuje, že stránka Nastavení zabezpečení je přístupná pouze uživateli, který zajišťoval daný server.

<span id="BKMK_55"></span>
#### Může služba RMS chránit jednotlivé dokumenty na pevném disku uživatele nebo ve sdílené složce bezprostředně po jejich vytvoření?

Přestože pomocí služby RMS je možné chránit dokumenty uložené v místním počítači uživatele, představuje doporučenou možnost systém souborů EFS (Encrypting File System). Systém EFS transparentně chrání dokumenty, zatímco služba RMS vyžaduje k nastavení ochrany dokumentu ruční zásah (několik klepnutí myší).

<span id="BKMK_56"></span>
#### V případě otevření souboru jsou šifrovány automaticky ukládané a dočasné soubory?

Ano, všechny dočasné soubory jsou šifrovány.

<span id="BKMK_562"></span>
#### V doručeném e-mailu chráněném právy je připojena příloha. Tuto přílohu je možné uložit, přestože poštu pravděpodobně uložit nelze. Došlo k narušení služby RMS?

Ne. Takové chování je správné. Zobrazená příloha je šifrovanou zprávou, než ji klient RMS dešifruje. Je i nadále chráněná právy a po dešifrování ji nebude možné uložit.
