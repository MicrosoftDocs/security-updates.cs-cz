---
TOCTitle: Nasazení služby RMS v doménových strukturách
Title: Nasazení služby RMS v doménových strukturách
ms:assetid: 'd531dfdc-efff-4eb0-8d99-f1fd19d7a963'
ms:contentKeyID: 18113451
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747685(v=WS.10)'
---

Nasazení služby RMS v doménových strukturách
============================================

Pokud se ve vaší organizaci používá více doménových struktur služby Active Directory a chcete v organizaci povolit používání služby RMS, Zkontrolujte, zda jste síť nakonfigurovali tak, aby služba RMS dokázala identifikovat a ověřovat účty uživatelů a distribuční skupiny v různých doménových strukturách.

Služba RMS používá službu Active Directory k identifikaci uživatelů a distribučních skupin. Pokud nasazení služby Active Directory v organizaci obsahuje více doménových struktur, používá služba RMS kontaktní objekty k získání ID skupin a uživatelů patřících do jiné doménové struktury než server RMS. K tomu je nutné provést tři kroky:

1.  Ve druhé doménové struktuře musí existovat servery certifikace služby RMS a pro jednotlivé vzdálené skupiny musí být definovány kontaktní objekty.
2.  V doménových strukturách musí existovat rozšíření schémat obsahující kontaktní objekty, která by jim umožňovala odkazovat zpět do doménových struktur obsahujících vlastní objekty.
3.  Atributy v kontaktních objektech musí být synchronizovány tak, aby odkazovaly na doménové struktury obsahující vlastní objekt.

Předpokládejme například, že skupiny jsou definovány a spravovány v jedné doménové struktuře a uživatelé jsou definováni a spravováni v jiné doménové struktuře. Uživatel potřebuje přiřadit práva k obsahu na základě členství v určité skupině. *RMS\_Server\_U* je v tomto scénáři server v doménové struktuře, která obsahuje uživatelské účty, a *RMS\_Server\_S* je server v doménové struktuře obsahující účty skupin. Mezi oběma servery RMS byla vytvořena důvěryhodná doména uživatelů. Aby bylo možné na serveru *RMS\_Server\_U* úspěšně rozšířit členství ve skupinách uvedené v licenci k publikování do jiných doménových struktur, musí v místní doménové struktuře služby Active Directory existovat kontaktní objekt reprezentující skupinu ve vzdálené doménové struktuře. Server RMS může zadávat dotazy na atributy kontaktního objektu a zjistit, zda tento objekt představuje skupinu v jiné doménové struktuře. V této doménové struktuře potom dokáže vyhledat server RMS a zjistit, zda mezi ním a druhým serverem RMS existuje vztah důvěryhodnosti. Pokud server *RMS\_Server\_U* zadá dotaz službě Active Directory na skupinu uvedenou v licenci k publikování, bude kontaktní objekt určovat, že skupina patří do jiné doménové struktury. Pokud server *RMS\_Server\_U* požadavek předá serveru RMS uvedenému ve spojovacím bodu služby pro danou doménu, určí spojovací bod služby server *RMS\_Server\_S* jako server certifikace služby RMS pro danou doménu. *RMS\_Server\_U* potom zadá dotaz na server *RMS\_Server\_S* za účelem získání členství v dané skupině.

Atributem, na který služba RMS zadává dotaz, aby získala tyto informace, je **msExchOriginatingForest**. Tento atribut je ve výchozím nastavení nainstalován do schématu služby Active Directory, jestliže je v doménové struktuře nainstalován produkt Exchange Server 2003. Tento atribut musí obsahovat doménová struktura každého schématu služby Active Directory, které se bude používat v rámci služby RMS. Pokud nepoužíváte Exchange Server 2003, můžete tato rozšíření schémat přidat stažením sady RMS Administration Toolkit. Tato sada obsahuje soubor schématu a pokyny, jak jej přidat do adresáře služby Active Directory.

Tyto atributy je nutné synchronizovat, aby kontaktní objekt odkazoval na vlastní objekt v ostatních doménových strukturách. Po přidání atributu do schématu služby Active Directory je nutné nakonfigurovat jeho hodnotu na úplný název domény doménové struktury, ve které se skupina nachází, například corp.fabrikam.com.

To lze provést pomocí produktu Microsoft Identity Integration Server (MIIS) 2003 nebo Identity Integration Feature Pack (IIFP) a agenta pro správu globálního seznamu adres služby Active Directory.

Je nutné nastavit, aby měl místní server RMS dostatečná oprávnění k prohledávání vzdáleného adresáře služby Active Directory a k volání rozhraní .NET Remoting na vzdáleném serveru RMS.

Aby bylo možné rozšiřovat skupiny za hranice doménových struktur, musí mít účet používaný pro účet služby RMS v každé doménové struktuře také oprávnění pro čtení a spouštění v adresáři služby Active Directory. Služba RMS automaticky udělí oprávnění ke čtení adresáře Active Directory všem ověřeným uživatelům s pověřeními domény. Pokud chcete zvýšit zabezpečení, můžete toto oprávnění odebrat z volitelných seznamů řízení přístupu (DACL) a nahradit ho individuálními účty služeb z jiných doménových struktur.

Oprávnění požadovaná pro účet služby RMS se mohou lišit v závislosti na tom, zda mezi místními a vzdálenými doménovými strukturami existují vztahy důvěryhodnosti služby Active Directory. V následujícím seznamu jsou uvedeny modely vztahů důvěryhodnosti a požadovaná oprávnění:

-   **Existuje obousměrný vztah důvěryhodnosti**. Místní doménová struktura RMS důvěřuje doménové struktuře, z níž skupina pochází, a naopak. Účtem služby RMS pro server RMS v každé doménové struktuře může být jakýkoli platný účet domény v doménové struktuře. Místní účet služby RMS je nutné přidat do volitelného seznamu řízení přístupu složky \\Inetpub\\wwwroot\\\_wmcs\\drmRemote na všech serverech RMS, které jsou v doménové struktuře, ze které skupina pocházela.
-   **Existuje jednosměrný vztah důvěryhodnosti**. Místní doménová struktura RMS důvěřuje doménové struktuře, z níž skupina pochází, ale tato doménová struktura místní struktuře nedůvěřuje. Účet služby RMS pro všechny servery RMS v organizaci by měl být platným účtem domény v důvěryhodné doménové struktuře. Tento účet přidejte do volitelného seznamu řízení přístupu složky \\Inetpub\\wwwroot\\\_wmcs\\drmRemote na všech serverech RMS, které jsou v doménové struktuře, ze které skupina pocházela.
-   **Neexistuje žádný vztah důvěryhodnosti**. Doménové struktury v organizaci nemohou ověřovat uživatele a skupiny pocházející z jiných doménových struktur. Doporučujeme nerozšiřovat skupiny do dalších doménových struktur, pokud příslušné domény nemají mezi sebou vztah důvěryhodnosti. Pokud je však taková situace nutná z provozního hlediska, můžete tento scénář povolit nakonfigurováním účtu služby RMS jako platného účtu domény v obou doménových strukturách. Navíc je třeba v obou doménových strukturách používat stejné uživatelské jméno a heslo. Dále je nutné vytvořit na každém koncovém serveru RMS místní účet počítače se stejným uživatelským jménem a heslem jako u účtů domén, které se používají pro účet služby RMS v obou doménových strukturách. To automaticky umožní místní službě získat dostatečná oprávnění k ověření jak na vzdáleném adresáři služby Active Directory, tak i na vzdáleném serveru RMS.

Používání zásad důvěryhodnosti služby RMS
-----------------------------------------

Při nasazení služby RMS v organizaci s více doménovými strukturami musí být v každé doménové struktuře, která je hostitelem účtů uživatele, nasazen server certifikace služby RMS tvořící součást systému RMS. Pokud chcete, aby mohli uživatelé v různých doménových strukturách sdílet obsah chráněný službou RMS, bude nutné nakonfigurovat zásady důvěryhodnosti služby RMS tak, aby bylo možné certifikáty a licence generované druhým serverem RMS považovat za důvěryhodné. U služby RMS lze používat dvě různé zásady důvěryhodnosti: důvěryhodné domény uživatelů a důvěryhodné domény publikování. Důvěryhodné domény uživatelů umožňují serveru RMS považovat za důvěryhodné certifikáty účtů práv generované jiným serverem certifikace služby RMS a vydávat licence k použití uživatelům s certifikáty účtů práv z tohoto druhého serveru. Důvěryhodné domény publikování umožňují serveru RMS generovat licence k použití na základě licencí k publikování, které určují druhý server správy licencí.

Příklady některých možností, jak používat zásady důvěryhodnosti pro podporu více doménových struktur:

-   Cluster certifikace služby RMS v každé doménové struktuře s jedním clusterem správy licencí sdíleným všemi uživateli. Cluster správy licencí služby RMS by byl nakonfigurován s důvěryhodnou doménou uživatelů zahrnující všechny clustery certifikace služby RMS. Klienti RMS by byli pomocí klíče registru pro připojení ke clusteru správy licencí nakonfigurováni na získání licencí k použití.
-   Cluster certifikace nebo správy licencí služby RMS v rámci každé doménové struktury s důvěryhodnou doménou uživatelů nakonfigurovanou na jednotlivých clusterech tak, aby byly servery RMS v ostatních doménových strukturách považovány důvěryhodné. Každý uživatel by používal server RMS ve své doménové struktuře k získání licencí k použití a mohl by zjišťovat příslušný server správy licencí prostřednictvím spojovacího bodu služby v adresáři služby Active Directory.
-   Pokud jsou uživatelé obsahu chráněného službou RMS součástí doménové struktury, která nemá přístup k doménové struktuře, z níž byl obsah publikován, lze důvěryhodnou doménu publikování nastavit tak, aby bylo možné obsah licencovat a používat. U důvěryhodných domén publikování je nutné publikovat soukromý klíč serveru RMS použitý k publikování obsahu.

Další informace o konfiguraci zásad důvěryhodnosti získáte v této sadě dokumentace v části Správa důvěryhodných domén a zásad důvěryhodnosti tématu Provoz serveru RMS.
