---
TOCTitle: Průvodce rychlým nasazením
Title: Průvodce rychlým nasazením
ms:assetid: 'b8fb69b6-3e0b-4836-8c05-8bd93f522a7c'
ms:contentKeyID: 18113477
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747735(v=WS.10)'
---

Průvodce rychlým nasazením
==========================

Tento průvodce vám usnadní rychlou instalaci serveru se službou RMS s aktualizací Service Pack 1, abyste jej mohli vyzkoušet a rozhodnout o případném širším nasazení této služby v organizaci.

**Krok 1. Příprava prostředí pro službu RMS**

Služba RMS je závislá na jiných součástech, které je nutné instalovat a konfigurovat před prvním použitím této služby. Aby infrastruktura splňovala základní požadavky služby RMS, je třeba provést následující kroky:

1.  Nastavte konfiguraci počítače se systémem Windows Server 2003 a poté tento počítač připojte k doméně Active Directory. (U malých organizací s jediným serverem může tento počítač sloužit zároveň jako řadič domény Active Directory. V takovém případě však v tomto počítači musí být nainstalován systém Windows Server 2003 Standard Edition, Windows Server 2003 Enterprise Edition nebo Windows Server 2003 Datacenter Edition. Počítač se systémem Windows Server 2003 Web Edition nemůže být řadičem domény.)
2.  Nakonfigurujte server na roli **aplikačního serveru**. Chcete-li uvedený krok provést, klepněte na tlačítko **Start**, poklepejte na příkaz **Ovládací panely** a poklepejte na položku **Přidat nebo odebrat programy**. Na ovládacím panelu **Přidat nebo odebrat programy** klepněte na tlačítko **Přidat nebo odebrat součásti systému** a přesvědčte se, zda jsou v seznamu **Aplikační server** povoleny následující služby:
    -   **ASP.NET,**
    -   **Internetová informační služba (IIS),**
    -   **Řízení front zpráv.**

    U všech služeb potvrďte výchozí možnosti. Není třeba provádět žádné další změny konfigurace.
3.  Konfigurujte databázový server s použitím některé z následujících databázových aplikací:
    -   Microsoft® SQL Server 2000 s aktualizací SP3a. Může se jednat o místní instalaci serveru SQL Server 2000 nebo o vzdálenou instalaci umístěnou ve stejné doméně.
    -   Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) verze A. Musí se jednat o místní instalaci. Server MSDE 2000 lze stáhnout z [webu společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=17799) (http://go.microsoft.com/fwlink/?LinkID=17799).

    Součást Microsoft SQL Server Desktop Engine je vhodné používat k podpoře databází služby RMS pouze v testovacím prostředí, protože neobsahuje nástroje nezbytné ke komplexnímu provozu a podpoře databáze v rámci celého podniku. Součást MSDE nepodporuje vzdálenou síť, a proto je zároveň nutné nainstalovat ji na stejný server jako službu RMS, přičemž není možné do clusteru služby RMS přidávat další servery RMS. V podmínkách používání součásti Microsoft SQL Server Desktop Engine je navíc uvedeno, že pro obsluhu databáze Microsoft SQL Server Desktop Engine nelze použít klientské nástroje serveru SQL Server. Toto omezení neumožňuje zálohování a obnovování konfigurační databáze služby RMS, prohlížení informací protokolování ani přímou změnu dat uložených v konfigurační databázi.
4.  Určete název, který budou při přístupu k této službě používat uživatelé připojující se v rámci intranetu (například http://certification.contoso.com). Nastavte službu DNS tak, aby danou adresu URL převáděla na adresu IP počítače se službou RMS. Pro adresu URL clusteru byste měli používat úplný název domény, aby klienti v ostatních zónách DNS dokázali převádět adresy IP serverů RMS.
5.  Vytvořte účet správce, který chcete používat pro službu RMS.
6.  Nyní jste připraveni k instalaci služby RMS s aktualizací SP1. Další pokyny k tomuto kroku získáte v této sadě dokumentace v části Instalace služby RMS s aktualizací Service Pack 1 tématu Provoz serveru RMS.

**Běžně používané nepovinné funkce**

Použití následujících funkcí je nepovinné. Pokud je budete chtít používat, bude nutné před zahájením instalace a zajišťování služby RMS provést nezbytné přípravné kroky:

-   Službu RMS lze nastavit tak, aby k ukládání soukromých klíčů využívala hardwarový modul zabezpečení. Pokud chcete používat modul hardwarového zabezpečení, zkontrolujte správnost nastavení ovladačů a přesvědčte se, zda je definováno zabezpečené prostředí.
-   Certifikát serveru pro poskytování licencí lze automaticky stáhnout při zajišťování, jestliže je počítač se službou RMS připojen k Internetu. Jestliže vaše organizace používá pro připojení k Internetu server proxy, zkontrolujte nastavení serveru proxy v prohlížeči Internet Explorer, včetně všech požadavků ověřování, a poznamenejte si je pro pozdější použití.
-   Pokud budou služby RMS pracovat v počítači řadiče domény a pokud zároveň plánujete ke spouštění těchto služeb používat uživatelský účet, zkontrolujte, zda konfigurace zásad zabezpečení řadiče domény poskytuje danému uživatelskému účtu oprávnění k místnímu přihlášení. Další informace o nastavení konfigurace zásad zabezpečení řadiče domény naleznete v Centru pro nápovědu a odbornou pomoc systému Windows Server 2003.

**Krok 2. Zajištění prvního serveru RMS**

Pojmem zajištění označujeme proces konfigurace služby RMS na webovém serveru tak, aby ji uživatelé mohli začít využívat. Při zajištění serveru kořenové certifikace v organizaci postupujte takto:

1.  Přihlaste se k počítači jako uživatel domény s oprávněními místního správce. Pokud službu RMS instalujete do počítače řadiče domény, přihlaste se jako správce domény.
2.  Klepněte na tlačítko **Start**, přejděte na položku **Všechny programy**, přejděte na položku **Služba RMS v systému Windows** a pak klepnutím na odkaz **Správa služby RMS v systému Windows** otevřete stránku **Globální správa**. Na této stránce jsou uvedeny weby dostupné na daném serveru.
3.  Klepněte na web, pro který chcete zajistit službu RMS, a poté klepněte na odkaz **Zajišťovat službu RMS na tomto webu**. Při otevření další stránky se na jejím začátku zobrazí text **Zadat server kořenové certifikace služby RMS**.
4.  Zadejte informace o své organizaci.
    -   Do pole **Adresa URL clusteru** zadejte název služby (například certification.contoso.com), který jste nastavili v kroku 4 předcházejícího postupu. Pokud chcete v instalaci využívat zabezpečení SSL, klepněte v seznamu protokolů na položku HTTPS. Provedením tohoto kroku povolíte zabezpečení SSL, jeho použití u webových služeb RMS však nebude vyžadováno. Tento požadavek je nutné nastavit zvlášť pomocí služby IIS.
    -   Jestliže je váš server připojen k Internetu prostřednictvím serveru proxy, doplňte v oblasti **Nastavení serveru proxy služby RMS** informace, které jste si poznamenali v aplikaci Internet Explorer podle kroků popsaných v předchozím postupu v části věnované nepovinným funkcím.
    -   V části **Připojení serveru k Internetu** vyberte možnost **Online**, pokud chcete, aby se server připojil ke službě Microsoft Enrollment Services přes Internet a získal certifikát serveru pro poskytování licencí automaticky při zajišťování. Možnost **Offline** vyberte, jestliže se chcete ke službě Microsoft Enrollment Services připojit ručně a uvedený certifikát stáhnout a importovat až po zajištění serveru RMS.
5.  Klepněte na tlačítko **Odeslat**.
    Během asi 60 až 90 sekund bude zajištění úspěšně provedeno. Poté se můžete vrátit na stránku **Globální správa** a spravovat odtud nově zajištěný server RMS.
6.  Na stránce **Globální správa** otevřete výběrem možnosti **Spravovat službu RMS na tomto webu** domovskou stránku **pro správu** serveru RMS.
    Pokud jste v kroku 4 vybrali možnost Offline pro připojení serveru k Internetu, dokončete před provedením dalších kroků postup Ruční zápis serveru kořenové certifikace.
7.  Na stránce Domovská stránka pro správu klepněte na odkaz **Spojovací bod služby RMS**.

| ![](images/Cc747735.note(WS.10).gif)Poznámka                                                                                                                                                                                                                                                                                             |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Další krok tohoto postupu, registrace spojovacího bodu služby, vyžaduje, aby byl použit doménový účet s dostatečnými oprávněními pro vytvoření kontejnerového objektu pod kontejnerem služeb v rámci kontejneru konfigurace doménové struktury Active Directory. Příkladem účtu s potřebnými oprávněními je předdefinovaná skupina zabezpečení **Enterprise Admins**. |

1.  Na stránce **spojovacího bodu služby RMS** klepněte na tlačítko **Registrovat adresu URL**. Tímto způsobem bude zaregistrován spojovací bod služby RMS v rámci služby Active Directory. Aplikace s podporou správy přístupových práv potom mohou rozpoznávat správu licencí služby RMS, aktivaci serveru proxy a služby certifikace. 

**Krok 3. Testování služby RMS**

Chcete-li službu RMS plně využívat, je nutné do klientských počítačů nejprve nainstalovat klienta Služby správy přístupových práv v systému Microsoft Windows a aplikaci s podporou správy přístupových práv. Uživatelé by měli být členy domény Active Directory a klientské počítače by měly být k této doméně připojeny. Pro uživatele domény by také měly být definovány e-mailové adresy v adresáři Active Directory. Pokud chcete službu RMS otestovat, postupujte následujícím způsobem:

1.  Přihlaste se ke klientskému počítači jako platný uživatel domény.
2.  Nainstalujte klienta služby RMS pro aktualizaci Service Pack 1.
3.  Nainstalujte aplikaci s podporou správy přístupových práv.
4.  Vytvořte soubor chráněný správou přístupových práv, udělte u tohoto souboru všem uživatelům práva jen pro čtení a uložte jej do sdílené složky, k níž mají uživatelé úplný přístup.
5.  Přihlaste se k počítači jako jiný uživatel. Otevřete soubor a pokuste se jej změnit. Pokud je služba RMS správně nainstalována, nebude možné žádné změny provést.
