---
TOCTitle: Zajištění serveru správy licencí
Title: Zajištění serveru správy licencí
ms:assetid: '4d67b898-0ba9-4eef-ab7d-ee0ca55a688e'
ms:contentKeyID: 18113310
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747563(v=WS.10)'
---

Zajištění serveru správy licencí
================================

Provedení tohoto postupu vyžaduje, aby byl uživatel místně přihlášen k webu pro správu v rámci uživatelského účtu, který je členem skupiny Administrators v počítači, k němuž získává přístup. Uvedený postup mohou provést také členové skupiny Domain Admins. Proces dílčího zápisu dále vyžaduje oprávnění ke čtení a spouštění pro účet uživatele domény i pro skupinu RMS Service Group. Další informace naleznete v tomto tématu v části [Nastavení oprávnění souboru služby dílčího zápisu](https://technet.microsoft.com/737bb69b-fe26-4057-9569-e632f7bbf295) uvedené již dříve. Pokud používáte vzdálenou databázi SQL Server, musí být účtu, pod kterým se přihlašujete, dále přidělena role tvůrce databáze na serveru SQL Server. Z hlediska zabezpečení je nejvhodnější při provádění tohoto postupu použít příkaz **Spustit jako**.

Chcete-li otevřít webovou stránku **Globální správa**, klepněte na tlačítko **Start**, přejděte na příkaz **Všechny programy**, přejděte na položku **Služba RMS v systému Windows** a klepněte na položku **Správa služby RMS v systému Windows**.

Na každém serveru lze službu RMS zajistit pouze pro jeden web. Chcete-li zajistit službu RMS pro jiný než výchozí web, přidejte požadovaný web pomocí Správce Internetové informační služby dříve, než zahájíte proces zajišťování. Není-li web, pro který chcete službu zajistit, uveden v seznamu webů, zavřete stránku **Globální správa**, přidejte požadovaný web a poté znovu spusťte proces zajišťování.

Pokud nasazujete službu RMS v prostředí, kde je úroveň funkčnosti domény služby Active Directory nastavena na nativní režim systému Microsoft Windows 2000, nemusí být služba RMS při pokusu o rozšíření členství ve skupině schopna načíst atribut **memberOf** objektů služby Active Directory. Chcete-li službě RMS umožnit načtení atributu **memberOf**, musí služba RMS využívat účet domény, který je členem (integrované) skupiny Pre-Windows 2000-Compatible Access obsažené v místní doménové struktuře.

Jestliže u clusteru zadáte vlastní adresu URL, zaregistrujte ji ve službě DNS a zkontrolujte, zda funguje. V případě nasazení s podporou Internetu zkontrolujte, zda je adresa URL přístupná jak z Internetu, tak i v rámci organizace. Pokud jste u souborů webových služeb povolili zabezpečení SSL, je nutné v adrese URL clusteru použít protokol HTTPS.

Zajištění serveru správy licencí
--------------------------------

#### Zajištění serveru správy licencí

1.  Otevřete stránku **Globální správa** a klepněte na položku **Zajišťovat službu RMS na tomto webu** u webu, pro který chcete zajistit službu RMS.

    Můžete vybrat výchozí web nebo jiný web, který jste pro tento účel vytvořili v Internetové informační službě (IIS).

    | ![](images/Cc747563.Warning(WS.10).gif)Varování                                                                                                                                                                                                         |
    |--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Spouštění dalších webů a webových služeb na společném serveru se službou RMS není podporováno. Výsledkem by mohl být případ, kdy bude pod stejným účtem jako služba RMS pracovat více aplikací a služeb. V takovém případě hrozí provádění nezaručených operací se soukromými klíči. |

2.  Výchozí možnost v části **Konfigurační databáze** vytváří konfigurační databázi na místním serveru. Pro místní databázi můžete použít databázový server (například SQL Server™ 2000 s aktualizací SP3) nebo součást Microsoft SQL Server 2000 Desktop Engine (MSDE). Pokud používáte vzdálenou databázi nebo provozujete databázový server na místním serveru, ale instance databázového serveru má jiný název než název tohoto serveru, vyberte možnost **Vzdálená databáze** a zadejte název databázového serveru.

    | ![](images/Cc747563.Important(WS.10).gif)Důležité informace                                                                                                                                                                                                                                                                                                                                                                |
    |---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Produkt Microsoft SQL Server Desktop Engine se doporučuje používat k podpoře databází RMS pouze v testovacím prostředí, protože nepodporuje žádná síťová rozhraní. V podmínkách používání součásti MSDE 2000 je navíc uvedeno, že pro obsluhu databáze MSDE 2000 nelze použít klientské nástroje serveru SQL Server. Vzhledem k tomuto omezení by nebylo možné zobrazit informace obsažené v protokolech a změnit data uložená v konfigurační databázi. |

3.  V části **Účet služby RMS** zadejte účet služby RMS, pod kterým bude služba RMS obvykle pracovat za běžného provozu. U instalace na jediný server můžete zadat místní systémový účet nebo doménový účet. U všech ostatních instalací je nutné zadat doménový účet. V případě doménového účtu zadejte název účtu ve tvaru *název\_domény*\\*uživatelské\_jméno* a heslo.

    | ![](images/Cc747563.Warning(WS.10).gif)Varování                                                                                                                                                                                                                                                                                                                                                                                                                   |
    |------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Místní systémový účet umožňuje přístup téměř ke všem prostředkům operačního systému. Z tohoto důvodu by mohly být důsledky jeho zneužití velmi závažné. Vždy, když je to možné, se proto použití místního systémového účtu jako účtu služby RMS vyvarujte. Místo toho vytvořte speciální účet uživatele domény, který bude sloužit jako účet služby RMS, a nepřidělujte mu žádná zvláštní oprávnění. Jako účet služby RMS nelze použít doménový účet, který byl použit k instalaci služby RMS. |

4.  V části **Adresa URL clusteru** zadejte adresu URL serveru nebo clusteru, který bude použit pro klienty v interní síti. Jako výchozí hodnota je použit název serveru, například Contoso-cert. Tuto položku můžete podle potřeby upravit a nastavit například adresu URL clusteru nebo serveru pro vyrovnávání zatížení, který daný cluster obsluhuje. Dále můžete vybrat protokol HTTP nebo HTTPS. Další informace o nastavení adresy URL clusteru naleznete v oddílu **Poznámky**. Po zajištění můžete z webových stránek pro správu konfigurovat externí adresu clusteru, která je určena pro klienty mimo vaši interní síť.

5.  V části **Ochrana soukromého klíče a dílčí zápis** vyberte jeden z následujících mechanismů ochrany soukromého klíče serveru:

    -   **Použijte výchozí softwarovou ochranu soukromého klíče**. Pokud vyberete tento způsob ochrany, bude soukromý klíč uložen do konfigurační databáze služby RMS. Je třeba zadat silné heslo, které bude použito k zašifrování klíče v databázi.

    | ![](images/Cc747563.Important(WS.10).gif)Důležité informace                                                                                                                                                                                                                                                                                                                                                                       |
    |----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Toto heslo uložte do zabezpečeného archivu pro případ pozdějšího využití. Dále uložte do zabezpečeného archivu záložní kopii konfigurační databáze (rovněž zajištěnou stejným heslem). Budete tak mít k dispozici prostředky pro obnovení služby RMS v případě poškození databáze serveru SQL Server. Pokud heslo z nějakého důvodu změníte, vytvořte novou zálohu konfigurační databáze s použitím nového hesla a poté obojí uložte do zabezpečeného archivu. |

    -   **Použijte zprostředkovatele kryptografických služeb (CSP)**. Chcete-li použít zprostředkovatele kryptografických služeb nebo modul hardwarového zabezpečení, zrušte zaškrtnutí políčka **Použít výchozí softwarovou ochranu soukromého klíče**. V seznamu **Vyberte zprostředkovatele kryptografických služeb** vyberte zprostředkovatele kryptografických služeb nebo modul hardwarového zabezpečení, který jste instalovali.

    | ![](images/Cc747563.note(WS.10).gif)Poznámka                                                                                                               |
    |-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Služba RMS vyžaduje použití úplného zprostředkovatele RSA (Rivest-Shamir-Adleman). V seznamu zprostředkovatelů kryptografických služeb je proto uveden jen tento typ zprostředkovatelů. |

    | ![](images/Cc747563.note(WS.10).gif)Poznámka                                                                                                                                                                                                                                                                |
    |------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Doporučujeme používat buď výchozí softwarovou ochranu pomocí soukromého klíče, nebo modul hardwarového zabezpečení. Chcete-li u služby RMS používat jiného softwarového zprostředkovatele kryptografických služeb, je nejprve nutné u něj zajistit řádný chod všech klíčových činností správy (například postupů zálohování a obnovení). |

6.  Tento krok platí pouze pro uživatele, kteří vybrali zprostředkovatele kryptografických služeb. Chcete-li určit, který pár klíčů serveru má být použit, proveďte jednu z následujících akcí:

    -   U nové instalace vyberte možnost **Vytvořit nový pár veřejného a soukromého klíče**.
    -   Pokud obnovujete nebo upgradujete existující server RMS, vyberte možnost **Použít existující pár veřejného a soukromého klíče**. Klepněte na tlačítko **Procházet** u pole Existující kontejner klíčů a poté vyberte kontejner klíčů pro pár klíčů serveru.

    | ![](images/Cc747563.note(WS.10).gif)Poznámka                                                  |
    |----------------------------------------------------------------------------------------------------------------------------|
    | Základní, rozšíření i silní zprostředkovatelé kryptografických služeb společnosti Microsoft sdílejí stejné úložiště klíčů. |

    | ![](images/Cc747563.note(WS.10).gif)Poznámka                                                                                                                                                                                                                                            |
    |----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Pokud při obnovení nebo upgradu existujícího serveru RMS nepoužijete existující pár klíčů, bude nutné vymazat úložiště klíčů u všech existujících klientů RMS (tedy odstranit licence k použití a certifikáty účtů práv), přičemž tito klienti budou muset získat nové licence ze serveru, aby mohli používat obsah. |

7.  Do pole **Název certifikátu serveru pro poskytování licencí** zadejte název, který má být použit v certifikátu serveru pro poskytování licencí. Výchozí hodnotou je název serveru.

8.  Pokud vaše organizace používá pro připojení k Internetu server proxy, zaškrtněte políčko **Tento server používá k připojení k Internetu server proxy** a poté zadejte adresu a port serveru proxy.

    Pokud server proxy vyžaduje ověřování, vyberte typ ověřování a zadejte uživatelské jméno a heslo, která lze serverem proxy ověřit. Používáte-li integrované ověřování systému Windows, je nutné rovněž zadat doménu.

9.  Klepněte na tlačítko **Odeslat**.

    Služba dílčího zápisu RMS vygeneruje pár veřejného a soukromého klíče serveru správy licencí a veřejný klíč podepíše pomocí soukromého klíče serveru kořenové certifikace. Kromě toho vytvoří certifikát serveru pro poskytování licencí pro server správy licencí. Během několika minut budou tyto položky odeslány do konfigurační databáze.

    | ![](images/Cc747563.Important(WS.10).gif)Důležité informace                                                                                                                                                                                                                                                                                                                                                                           |
    |--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Pokud se zobrazí chybové zprávy, stránku nezavírejte. Opravte chyby, zastavte a znovu spusťte službu IIS z příkazového řádku pomocí příkazu IISReset, vraťte se na předcházející stránku, znovu zadejte informace potřebné k zajištění a poté znovu klepněte na tlačítko **Odeslat**. Pokud se zobrazí chyba Požadavek vypršel, zavřete okno, zkontrolujte, zda systém splňuje minimální hardwarové požadavky a pokud ano, zkuste provést zajištění serveru znovu. |

Pokyny k zajištění dalších serverů správy licencí a k jejich přidání do clusteru získáte v tomto tématu později v části [Přidání serveru do clusteru](https://technet.microsoft.com/db635238-5528-4bec-9cc6-8244e2b3d733).
