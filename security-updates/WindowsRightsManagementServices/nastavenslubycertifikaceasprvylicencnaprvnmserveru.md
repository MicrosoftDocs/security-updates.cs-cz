---
TOCTitle: Nastavení služby certifikace a správy licencí na prvním serveru
Title: Nastavení služby certifikace a správy licencí na prvním serveru
ms:assetid: 'cce29a2f-984f-48ed-9187-0eb68286ec5b'
ms:contentKeyID: 18113514
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747756(v=WS.10)'
---

Nastavení služby certifikace a správy licencí na prvním serveru
===============================================================

Chcete-li službu RMS nainstalovat v doménové struktuře, je potřeba nejdříve nainstalovat a zajistit jeden server. První server, který nasadíte, je server kořenové certifikace. Tento server poskytuje podporu certifikace i správy licencí a lze jej používat jako jediný server v konfiguraci s jedním serverem nebo jako první server clusteru kořenové certifikace.

Oprávnění, práva a role nutné k instalaci a zajištění dalších serverů RMS
-------------------------------------------------------------------------

Chcete-li nainstalovat službu RMS, je nutné se přihlásit pomocí účtu s oprávněními místního správce. Navíc musíte být přihlášeni k doméně prostřednictvím platného doménového účtu, aby bylo možné službu RMS ověřovat v rámci služby Active Directory. Pokud nasazujete službu RMS v prostředí, kde se v infrastruktuře služby Active Directory používá nativní režim systému Windows 2000, nemusí být služba RMS při pokusu o rozšíření členství ve skupině schopna načíst atribut memberOf objektů služby Active Directory. Chcete-li službě RMS umožnit načtení atributu memberOf, musí služba RMS využívat doménový účet, který je členem skupiny Pre-Windows 2000-compatible access obsažené v místní doménové struktuře. Pokud jste nasadili skupiny se skrytým členstvím, bude také nutné nakonfigurovat účet služby RMS s oprávněními ke čtení skrytého členství.

> [!NOTE]
> Jako účet služby RMS nelze použít doménový účet, který byl použit k instalaci služby RMS. 

Proces instalace a zajištění pro první server
---------------------------------------------

Nasazení serveru RMS probíhá ve dvou krocích. Nejdříve je nutné nainstalovat software serveru RMS společně s veškerým podpůrným softwarem (například služba IIS, Řízení front zpráv a ASP.NET). Další informace o instalaci získáte v této sadě dokumentace v části Instalace služby RMS s aktualizací Service Pack 1 tématu Provoz serveru RMS.

> [!NOTE]
> Službu RMS lze také nainstalovat pomocí příkazového řádku. Další informace najdete v této sadě dokumentace v části Instalace z příkazového řádku tématu Provoz serveru RMS. 

Po instalaci služby RMS na serveru je nutné tuto službu na serveru zajistit, aby se používala na jediném webu na daném serveru. Při zajištění tohoto webu dojde k úpravám mnoha jeho parametrů a k přidání virtuálních adresářů. Další informace o uvedených změnách naleznete v této sadě dokumentace v části Podpora Internetové informační služby pro službu RMS tématu Technické informace týkající se služby RMS.

Můžete použít kterýkoli výchozí web obsažený ve službě IIS nebo vytvořit nový web. Chcete-li službu RMS zajistit na jiném než výchozím webu, je nutné před zahájením procesu zajišťování web vytvořit. Jestliže používáte výchozí web pro jiné účely, měli byste vytvořit nový web pro službu RMS, aby byla pro výchozí web zachována výchozí konfigurace.

Po klepnutí na možnost **Správa služby RMS v systému Windows** v nabídce **Start** se zobrazí stránka **Globální správa**. Na této stránce můžete zahájit proces zajišťování na webu. Chcete-li zajistit první server RMS, je nutné zadat následující informace:

-   Zadejte název databáze používané pro konfigurační databáze, databáze protokolování a databáze adresářových služeb služby RMS.

    Pokud se název instance serveru SQL Server neshoduje s názvem místního serveru, je nutné ji nastavit jako vzdálenou instanci serveru SQL Server, a to i v případě, že jsou všechny součásti instalovány na jeden server.

    Během zajišťování musí být aktuálně přihlášenému uživatelskému účtu přiřazeno oprávnění k vytváření databází na databázovém serveru.
-   Zadejte účet, který chcete nastavit jako účet služby RMS. U místní konfigurace můžete použít místní systémový účet, ačkoli se tento postup nedoporučuje vzhledem ke skrytému oslabení zabezpečení spojenému se spuštěním služby s oprávněními k místnímu systému.

    V případě instalace, jejíž součástí je vzdálená instance serveru SQL Server nebo více než jeden server RMS, je nutné zadat doménový účet. Doménový účet, který použijete, musí mít oprávnění pro vyhledávání v adresáři služby Active Directory. Bude použit k vytvoření fondu aplikací IIS, pod nímž pracuje konzola správy. Pokud neupgradujete nebo nepoužíváte existující databázi, vyžaduje účet služby RMS oprávnění k vytváření databází. Jestliže používáte existující databáze, je nutné, aby byla účtu u jednotlivých databází služby RMS přiřazena oprávnění ke čtení i zápisu.

-   Zadejte adresu URL, kterou chcete používat pro přístup k tomuto webu. Výchozí hodnotou je název zajišťovaného webu (například Výchozí server WWW, pokud zajišťujete server s výchozí instalací služby IIS). Zadáním vlastní adresy URL můžete zajistit přístup k jinému webu. Může jít například o adresu URL serveru pro vyrovnávání zatížení nebo o podporu přístupu k intranetu i Internetu. Je nutné ověřit, zda vlastní adresa URL funguje. Navíc je potřeba přidat název webu v rámci služby DNS, aby bylo zajištěno, že stránka **Globální správa** i stránka pro **zajišťování** najde virtuální kořeny. U adres URL určených k nasazení přístupu k Internetu zkontrolujte, zda je nová adresa URL dostupná z Internetu i z podnikové sítě.

-   Vyberte způsob ochrany soukromého klíče kořenové instalace používaného pro zápis. Ve výchozím nastavení se používá softwarové šifrování a šifrovaný soukromý klíč je uložen v konfigurační databázi služby RMS. Pokud použijete výchozí konfiguraci, je nutné k zašifrování hodnoty v databázi zadat silné heslo.

    Jestliže jste však v počítači nainstalovali a nakonfigurovali hardwarový modul zabezpečení, můžete také vybrat zprostředkovatele kryptografických služeb pro použití s hardwarovým modulem zabezpečení a ukládat soukromé klíče v hardwaru, například pomocí karet Smart Card. Služba RMS vyžaduje použití úplného zprostředkovatele RSA. V seznamu zprostředkovatelů kryptografických služeb je proto uveden jen tento typ zprostředkovatelů. K ochraně soukromého klíče služby RMS doporučujeme používat modul hardwarového zabezpečení.

    Pokud k zabezpečení soukromého klíče služby RMS pomocí hesla použijete možnost softwarového zprostředkovatele kryptografických služeb, měli byste zadané heslo uložit do zabezpečeného archivu, kde je v případě potřeby kdykoli naleznete. Spolu s heslem byste měli uložit i záložní kopii konfigurační databáze. Uvedený krok vám umožní obnovit službu RMS v případě, že dojde k poškození databáze SQL. Jestliže heslo z nějakého důvodu změníte, vytvořte novou záložní kopii konfigurační databáze, v níž je uložen soukromý klíč zabezpečený pomocí nového hesla, a poté obojí uložte do zabezpečeného archivu. Další informace o tom, jak zálohovat a obnovovat konfigurační databázi, získáte v této sadě dokumentace v části Zálohování a obnovení systému služby RMS tématu Plánování nasazení služby RMS.
-   Zadejte název, který se bude používat v rámci certifikátu serveru pro poskytování licencí. Výchozí hodnotou je název serveru.
-   V případě potřeby zadejte server proxy (včetně adresy a portu), který má být použit pro přístup k Internetu.
-   Zadejte e-mailovou adresu, kterou mohou ostatní správci služby RMS používat jako kontakt na správce v případě, že dojde k potížím, pokud se správce pokusí provést dílčí zápis serveru správy licencí. Po zajištění kořenové instalace lze změnit adresu.
-   Vyberte způsob odvolání certifikátu serveru pro poskytování licencí umožňující určit, kdo kromě služby Microsoft Enrollment Services může odvolat certifikát serveru pro poskytování licencí kořenové instalace. Chcete-li používat odvolání třetí stranou, je nutné zadat cestu a název souboru obsahujícího veřejný klíč pro entitu třetí strany.

Pokud jste vybrali možnost zápisu online, vygeneruje služba RMS po klepnutí na tlačítko **Odeslat** na stránce pro **zajišťování** (po dokončení konfigurace všech příslušných možností) pár klíčů a odešle veřejný klíč službě Microsoft Enrollment Services. (Zobrazí-li se chybové zprávy, nezavírejte stránku, na které jsou chyby uvedeny. Po odstranění chyb otevřete okno příkazového řádku a zastavte a znovu spusťte službu IIS zadáním příkazu IISReset. Pak se vraťte na předchozí obrazovku, zadejte znovu informace na obrazovce zajišťování a potom znovu klepněte na tlačítko **Odeslat**.) Služba Microsoft Enrollment Services vytvoří certifikát serveru pro poskytování licencí a během několika minut jej vrátí konfigurační databázi. Vzhledem k tomu, že se jedná o první server v doméně, na kterém je služba RMS nainstalována, představuje tento krok zápis serveru kořenové certifikace.

Jestliže jste vybrali možnost zápisu offline, provedete zápis serveru ke službě Microsoft Enrollment Services ručně po dokončení procesu zajišťování. Server je možné začít používat až po dokončení procesu zápisu. Další informace získáte v této sadě dokumentace v části Ruční zápis serveru kořenové certifikace tématu Provoz serveru RMS.

Po dokončení zajišťování a zápisu serveru dojde ke změně odkazů na stránce **Globální správa**. Odkaz **Zajišťovat službu RMS na tomto webu** se změní na odkaz **Spravovat službu RMS na tomto webu**, odkaz **Přidat tento server do clusteru** bude nahrazen odkazem **Změnit účet služby RMS** a na stránku bude přidán odkaz **Odebrat službu RMS z tohoto webu**.

Tento první server vytvoří kořenovou instalaci služby RMS. Kořenová instalace se může skládat z jediného serveru nebo ji může tvořit cluster. Po dokončení instalace a zajištění prvního serveru můžete nastavit další servery poskytující redundanci a podporu vyrovnávání zatížení u služeb správy certifikátů a licencí.

Po dokončení konfigurace je nutné zaregistrovat spojovací bod služby clusteru kořenové certifikace v adresáři služby Active Directory, aby mohli klienti s podporou služby RMS službu zjistit. Další informace získáte v této sadě dokumentace v části Registrace spojovacího bodu služby tématu Provoz serveru RMS. Pokud není spojovací bod služby zaregistrován, nebude možné se službou RMS používat klienta RMS.

> [!IMPORTANT]
> Před instalací služby RMS na dalších serverech je nutné kompletně nainstalovat a zajistit službu RMS na prvním serveru. Služba RMS podporuje ochranu obsahu skupin služby Active Directory, které jsou členy více doménových struktur. Pokud organizace nepoužívá více doménových struktur nebo skupin ve více doménových strukturách, můžete optimalizovat výkon procesu vydávání licencí k použití na serveru RMS, a to změnou zásad clusteru **MaxCrossForestCalls** v konfigurační databázi služby RMS. Tato zásada určuje maximální počet případů, kdy členství ve skupině může překročit hranice doménové struktury. Výchozí je hodnota 10. Chcete-li ji změnit na hodnotu 0, zadejte následující příkaz SQL:`update DRMS_ClusterPolicies set PolicyData=0 where PolicyName='MaxCrossForestCalls'` 

Následující témata obsahují podrobné kroky nutné k provedení úloh dostupných na stránce Globální správa služby RMS:

-   Informace o tom, jak pomocí průvodce instalací nainstalovat první server, získáte v této sadě dokumentace v části Instalace služby RMS s aktualizací Service Pack 1 tématu Provoz serveru RMS.

-   Informace o tom, jak zajistit první server, získáte v této sadě dokumentace v části Zajištění prvního serveru kořenové certifikace tématu Provoz serveru RMS.

-   Informace o tom, jak přidávat servery do kořenové instalace za účelem vytvoření clusteru, získáte v tomto tématu později v části [Přidání serverů pro podporu certifikace a správy licencí](https://technet.microsoft.com/089ceb62-2a96-444f-ab42-1d5deaabd0c3).
