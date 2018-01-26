---
TOCTitle: Web správy služby RMS
Title: Web správy služby RMS
ms:assetid: 'f003c1d9-9a17-4e50-9e1e-5d67677552a0'
ms:contentKeyID: 18113546
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747796(v=WS.10)'
---

Web správy služby RMS
=====================

Každý kořenový cluster nebo cluster vyhrazený pro správu licencí je hostitelem webu správy, pomocí kterého můžete spravovat službu RMS. Tento web je k dispozici pouze na serveru RMS, který spravujete prostřednictvím připojení ke vzdálené ploše.

Toto téma popisuje funkce webu správy. Pokyny pro správu služby RMS pomocí uvedeného webu získáte v této sadě dokumentace v částech Postupy pro službu RMS... a Správa služby RMS v tématu Provoz služby RMS v této sadě dokumentace.

**Poznámka:** Konfigurace clusteru je globální. Konfiguraci clusteru je možné spravovat z webu správy libovolného serveru v daném clusteru.

Otevřete stránku **Globální správa**, abyste mohli provést následující úkoly.

-   zajištění služby RMS na webu,
-   zajištění serveru a jeho přidání do clusteru,
-   odebrání služby RMS z webu.
-   Přejděte na stránky správy daného clusteru.

Pomocí stránky **Správa** clusteru můžete provést následující úlohy:

-   **Zobrazení informací o clusteru** Můžete zobrazit informace o clusteru, jako je například adresa URL instalace, adresa URL serveru, název certifikátu, server konfigurační databáze, název konfigurační databáze nebo datum vypršení platnosti certifikátu.

-   **Zápis nebo obnovení certifikátu serveru pro poskytování licencí.** Můžete zapsat nebo obnovit certifikát serveru pro poskytování licencí pro daný cluster.

-   **Vytvoření zásad důvěryhodnosti.** Klepnutím na odkaz otevřete webovou stránku Zásady důvěryhodnosti, na které můžete přidat nebo odebrat důvěryhodné domény uživatelů a důvěryhodné domény publikování. Je možné přidat nebo odebrat uživatele v seznamu vyloučení, který je uložen v důvěryhodné doméně uživatelů. Můžete exportovat certifikát serveru pro poskytování licencí do souboru za účelem jeho importu jinou instalací služby RMS.

-   **Konfigurace šablon zásad práv.** Klepnutím na odkaz otevřete webovou stránku Šablony zásad práv, na které můžete vytvořit nebo změnit podnikové šablony zásad práv.

-   **Konfigurace protokolování.** Klepnutím na odkaz otevřete webovou stránku Nastavení protokolování, na které můžete zapnout nebo vypnout protokolování a zobrazit server a databázi protokolování.

-   **Zadání extranetové adresy URL clusteru.** Klepnutím na odkaz otevřete webovou stránku pro nastavení extranetové adresy URL clusteru, na které můžete zadat adresu URL umožňující přístup k serverům certifikace a správy licencí kořenového clusteru z extranetu.

-   **Zadání nastavení serveru proxy služby RMS.** Klepnutím na odkaz otevřete webovou stránku Nastavení serveru proxy služby RMS, na které můžete zadat adresu serveru proxy, typ ověřování a jméno uživatele použité v případě připojení serveru RMS k Internetu prostřednictvím serveru proxy.

-   **Sledování počtu distribuovaných certifikátů účtů práv.** Klepnutím na odkaz otevřete webovou stránku sledování certifikátů účtů práv, na které můžete zjistit, kolik certifikátů účtů práv bylo kořenovým clusterem vydáno. Pomocí tohoto čísla lze odhadnout počet požadovaných licencí klientského přístupu.

-   **Správa nastavení zabezpečení.** Klepnutím na odkaz otevřete webovou stránku Nastavení zabezpečení, na které můžete přidat nebo odebrat členy skupiny Super Users s úplným řízením veškerého licencovaného obsahu a také znovu nastavit heslo soukromého klíče.

-   **Zobrazení a konfigurace nastavení certifikátů účtů.** Klepnutím na odkaz otevřete webovou stránku Nastavení certifikace, na které můžete nastavit dobu trvání platnosti certifikátu a zadat kontakt na správce.

-   **Povolení zásad vyloučení.** Klepnutím na odkaz otevřete webovou stránku Zásady vyloučení, na které můžete povolit zásady vyloučení na základě verzí bezpečnostního modulu, verze systému Windows, certifikátů účtů a aplikací.

-   **Registrace spojovacího bodu služby.** Klepnutím na odkaz otevřete webovou stránku Spojovací bod služby, na které můžete zaregistrovat a zrušit registraci spojovacího bodu služby daného clusteru.

Správci mohou provádět další úkoly, včetně sledování událostí a správy služby Active Directory, Internetové informační služby (IIS) a serveru SQL Server, použitím konzoly Microsoft Management Console (MMC).
