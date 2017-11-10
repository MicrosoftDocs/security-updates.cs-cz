---
TOCTitle: Zajištění prvního serveru kořenové certifikace
Title: Zajištění prvního serveru kořenové certifikace
ms:assetid: 'debc42f3-74ff-4c99-b7a4-4921fccdabc2'
ms:contentKeyID: 18113526
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747768(v=WS.10)'
---

Zajištění prvního serveru kořenové certifikace
==============================================

Provedení tohoto postupu vyžaduje, aby byl uživatel místně přihlášen k webu pro správu v rámci uživatelského účtu, který je členem skupiny Administrators v počítači, k němuž získává přístup. Uvedený postup mohou provést také členové skupiny Domain Admins. Pokud používáte vzdálenou databázi SQL Server, musí být tomuto účtu dále přidělena role tvůrce databáze na serveru SQL Server. Z hlediska zabezpečení je nejvhodnější při provádění tohoto postupu použít příkaz **Spustit jako**.

Chcete-li otevřít webovou stránku **Globální správa**, klepněte na tlačítko **Start**, přejděte na příkaz **Všechny programy**, přejděte na položku **Služba RMS v systému Windows** a klepněte na položku **Správa služby RMS v systému Windows**.

Na každém serveru lze službu RMS zajistit pouze pro jeden web. Chcete-li zajistit službu RMS pro jiný než výchozí web, přidejte požadovaný web pomocí Správce Internetové informační služby dříve, než zahájíte proces zajišťování. Není-li web, pro který chcete službu zajistit, uveden v seznamu webů, zavřete stránku **Globální správa**, přidejte požadovaný web a poté znovu spusťte proces zajišťování.

Pokud nasazujete službu RMS v prostředí, kde je úroveň funkčnosti domény služby Active Directory nastavena na nativní režim systému Microsoft Windows 2000, nemusí být služba RMS při pokusu o rozšíření členství ve skupině schopna načíst atribut **memberOf** objektů služby Active Directory. Chcete-li službě RMS umožnit načtení atributu **memberOf**, musí služba RMS využívat účet domény, který je členem (integrované) skupiny Pre-Windows 2000-Compatible Access obsažené v místní doménové struktuře.

Jestliže u clusteru zadáte vlastní adresu URL, zaregistrujte ji ve službě DNS a zkontrolujte, zda funguje. V případě nasazení s podporou Internetu zkontrolujte, zda je adresa URL přístupná jak z Internetu, tak i v rámci organizace. Pokud jste u souborů webových služeb povolili zabezpečení SSL, je nutné v adrese URL clusteru použít protokol HTTPS.

zajištění prvního serveru kořenové certifikace
----------------------------------------------

#### Zajištění prvního serveru kořenové certifikace

1.  Po instalaci služby RMS na server, který bude použit jako první server kořenové certifikace v doménové struktuře Active Directory, otevřete stránku **Globální správa**.

2.  Klepněte na položku **Zajišťovat službu RMS na tomto webu** u webu, pro který chcete službu RMS zajistit. Můžete vybrat výchozí web nebo jiný web, který jste pro tento účel vytvořili v Internetové informační službě (IIS).

    > [!WARNING]
    > Spouštění dalších webů a webových služeb na společném serveru se službou RMS není podporováno. Výsledkem by mohl být případ, kdy bude pod stejným účtem jako služba RMS pracovat více aplikací a služeb. V takovém případě hrozí provádění nezaručených operací se soukromými klíči. 

3.  Výchozí možnost v části **Konfigurační databáze** vytváří konfigurační databázi na místním serveru. Pro místní databázi můžete použít databázový server (například SQL Server™ 2000 s aktualizací SP3) nebo součást Microsoft SQL Server 2000 Desktop Engine (MSDE). Pokud používáte vzdálenou databázi nebo provozujete databázový server na místním serveru, ale instance databázového serveru má jiný název než název tohoto serveru, vyberte možnost **Vzdálená databáze** a zadejte název databázového serveru.

    > [!IMPORTANT]
    > Produkt Microsoft SQL Server Desktop Engine se doporučuje používat k podpoře databází RMS pouze v testovacím prostředí, protože nepodporuje žádná síťová rozhraní. V podmínkách používání součásti MSDE 2000 je navíc uvedeno, že pro obsluhu databáze MSDE 2000 nelze použít klientské nástroje serveru SQL Server. Vzhledem k tomuto omezení by nebylo možné zobrazit informace obsažené v protokolech a změnit data uložená v konfigurační databázi. 

4.  V části **Účet služby RMS** zadejte účet služby RMS, pod kterým bude služba RMS obvykle pracovat za běžného provozu. U instalace na jediný server můžete zadat místní systémový účet nebo doménový účet. U všech ostatních instalací je nutné zadat doménový účet. V případě doménového účtu zadejte název účtu ve tvaru *název\_domény*\\*uživatelské\_jméno* a heslo.

    > [!WARNING]
    > Místní systémový účet umožňuje přístup téměř ke všem prostředkům operačního systému. Z tohoto důvodu by mohly být důsledky jeho zneužití velmi závažné. Vždy, když je to možné, se proto použití místního systémového účtu jako účtu služby RMS vyvarujte. Místo toho vytvořte speciální účet uživatele domény, který bude sloužit jako účet služby RMS, a nepřidělujte mu žádná zvláštní oprávnění. Jako účet služby RMS nelze použít doménový účet, který byl použit k instalaci služby RMS. 

    > [!IMPORTANT]
    > Z důvodů zabezpečení se doporučuje vytvořit speciální účet uživatele domény, který bude sloužit jako účet služby RMS, a nepřidělovat mu žádná zvláštní oprávnění. Jako účet služby RMS nelze použít doménový účet, který byl použit k instalaci služby RMS s aktualizací Service Pack 1. 

5.  V části **Adresa URL clusteru** zadejte adresu URL serveru nebo clusteru, který bude použit pro klienty v interní síti. Jako výchozí hodnota je použit název serveru, například Contoso-cert. Tuto položku můžete podle potřeby upravit a nastavit například adresu URL clusteru nebo serveru pro vyrovnávání zatížení, který daný cluster obsluhuje. Dále můžete vybrat protokol HTTP nebo HTTPS. Další informace o nastavení adresy URL clusteru naleznete v oddílu **Poznámky**. Po zajištění můžete z webových stránek pro správu konfigurovat externí adresu clusteru, která je určena pro klienty mimo vaši interní síť.

6.  V části **Ochrana soukromého klíče a zápis** vyberte jeden z následujících mechanismů ochrany soukromého klíče serveru:

    -   **Použijte výchozí softwarovou ochranu soukromého klíče**. Pokud vyberete tento způsob ochrany, bude soukromý klíč uložen do konfigurační databáze služby RMS. Je třeba zadat silné heslo, které bude použito k zašifrování klíče v databázi.

    > [!IMPORTANT]
    > Toto heslo uložte do zabezpečeného archivu pro případ pozdějšího využití. Dále uložte do zabezpečeného archivu záložní kopii konfigurační databáze (rovněž zajištěnou stejným heslem). Budete tak mít k dispozici prostředky pro obnovení služby RMS v případě poškození databáze serveru SQL Server. Pokud heslo z nějakého důvodu změníte, vytvořte novou zálohu konfigurační databáze s použitím nového hesla a poté obojí uložte do zabezpečeného archivu. 

    -   **Použijte zprostředkovatele kryptografických služeb (CSP)**. Chcete-li použít zprostředkovatele kryptografických služeb nebo modul hardwarového zabezpečení, zrušte zaškrtnutí políčka **Použít výchozí softwarovou ochranu soukromého klíče**. V seznamu **Vyberte zprostředkovatele kryptografických služeb** vyberte zprostředkovatele kryptografických služeb nebo modul hardwarového zabezpečení, který jste instalovali.

    > [!NOTE]
    > Služba RMS vyžaduje použití úplného zprostředkovatele RSA (Rivest-Shamir-Adleman). V seznamu zprostředkovatelů kryptografických služeb je proto uveden jen tento typ zprostředkovatelů. 

    > [!NOTE]
    > Doporučujeme používat buď výchozí softwarovou ochranu pomocí soukromého klíče, nebo modul hardwarového zabezpečení. Chcete-li u služby RMS používat jiného softwarového zprostředkovatele kryptografických služeb, je nejprve nutné u něj zajistit řádný chod všech klíčových činností správy (například postupů zálohování a obnovení). 

7.  Tento krok platí pouze pro uživatele, kteří vybrali zprostředkovatele kryptografických služeb. Chcete-li určit, který pár klíčů serveru má být použit, proveďte jednu z následujících akcí:

    -   U nové instalace vyberte možnost **Vytvořit nový pár veřejného a soukromého klíče**.
    -   Pokud obnovujete nebo upgradujete existující server RMS, vyberte možnost **Použít existující pár veřejného a soukromého klíče**. Klepněte na tlačítko **Procházet** u pole **Existující kontejner klíčů** a poté vyberte kontejner klíčů pro pár klíčů serveru.

    > [!NOTE]
    > Základní, rozšíření i silní zprostředkovatelé kryptografických služeb společnosti Microsoft sdílejí stejné úložiště klíčů. 

    > [!NOTE]
    > Pokud při obnovení nebo upgradu existujícího serveru RMS nepoužijete existující pár klíčů, bude nutné vymazat úložiště klíčů u všech existujících klientů RMS (tedy odstranit licence k použití a certifikáty účtů práv), přičemž tito klienti budou muset získat nové licence ze serveru, aby mohli používat obsah. 

8.  V části **Připojení serveru k Internetu** určete, zda se tento server připojí k Internetu za účelem získání certifikátu serveru pro poskytování licencí.

    -   Při výběru možnosti **Online** se server během procesu zajišťování automaticky připojí ke službě Microsoft Enrollment Services a získá certifikát serveru pro poskytování licencí.
    -   Možnost **Offline** vyberte v případě, že server RMS není připojen k Internetu, nebo pokud chcete získat certifikát serveru pro poskytování licencí ručně a naimportovat jej na server RMS po dokončení zajišťování.

9.  Do pole **Název certifikátu serveru pro poskytování licencí** zadejte název, který má být použit v certifikátu serveru pro poskytování licencí. Výchozí hodnotou je název serveru.

10. Pokud vaše organizace používá pro připojení k Internetu server proxy, zaškrtněte políčko **Tento server používá k připojení k Internetu server proxy** a poté zadejte adresu a port serveru proxy.

    Pokud server proxy vyžaduje ověřování, vyberte typ ověřování a zadejte uživatelské jméno a heslo, která lze serverem proxy ověřit. Používáte-li integrované ověřování systému Windows, je nutné rovněž zadat doménu.

    > [!NOTE]
    > Po zajištění lze toto nastavení upravit na stránce **Nastavení zabezpečení** na webu pro správu služby RMS. Tato stránka však není dostupná, dokud není server zapsán ke službě Microsoft Enrollment Services. Pokud organizace vyžaduje, abyste pro připojení k Internetu použili server proxy, přičemž tento server proxy není nakonfigurován, protože jste v části **Připojení serveru k Internetu** zvolili možnost **Offline**, nebude možné změnit nastavení procesu zápisu ani serveru proxy, dokud nedokončíte ruční zápis nebo opětovné zajištění služby RMS. 

11. Do pole **Kontakt pro správu** zadejte e-mailovou adresu správce, kterého lze kontaktovat v případě problémů se zajišťováním dalších serverů. Po zajištění můžete tuto e-mailovou adresu změnit.

12. V části **Odvolání** určete, zda chcete umožnit třetí straně odvolat certifikát serveru pro poskytování licencí pro tento server. Pokud tuto možnost vyberete, zadejte cestu a název souboru veřejného klíče třetí strany.

13. Klepněte na tlačítko **Odeslat**.

    Klepnutím na tlačítko **Odeslat** dojde k zajištění služby. Pokud jste vybrali zápis online, bude také proveden zápis pro server kořenové certifikace. Služba RMS přitom vygeneruje pár veřejného a soukromého klíče a veřejný klíč odešle službě Microsoft Enrollment Services. Služba Microsoft Enrollment Services vytvoří certifikát serveru pro poskytování licencí a během několika minut jej vrátí konfigurační databázi. Používáte-li zápis offline, je před konfigurací serveru RMS nutné dokončit postup popsaný v části [Ruční zápis serveru kořenové certifikace](https://technet.microsoft.com/aecdebb5-b28b-4b58-937a-392bb6ce9643) uvedené v tomto tématu později.

    > [!NOTE]
    > Tento server bude připraven k použití až po registraci spojovacího bodu (SCP) služby RMS v rámci služby Active Directory. K dokončení tohoto postupu použijte kroky uvedené v části [Registrace spojovacího bodu služby](https://technet.microsoft.com/630cc3c3-9ed9-4423-8874-cbaceb43b353). 

Pokyny k zajištění dalších serverů kořenové certifikace a k jejich přidání do clusteru naleznete v části [Přidání serveru do clusteru](https://technet.microsoft.com/db635238-5528-4bec-9cc6-8244e2b3d733) uvedené v tomto tématu později.
