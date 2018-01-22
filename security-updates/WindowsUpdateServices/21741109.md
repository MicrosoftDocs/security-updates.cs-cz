---
TOCTitle: 'Krok 3: Konfigurace síťových připojení'
Title: 'Krok 3: Konfigurace síťových připojení'
ms:assetid: '42a144c5-f08e-4a6e-b360-47ddea77bd24'
ms:contentKeyID: 21741109
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Dd939815(v=WS.10)'
---

Krok 3: Konfigurace síťových připojení
======================================

Po instalaci aktualizace Windows Server Update Services 3.0 Service Pack 2 (WSUS 3.0 SP2) se automaticky spustí průvodce konfigurací. Průvodce je možné také spustit později prostřednictvím stránky **Možnosti** v konzole pro správu služby WSUS.

Před začátkem procesu konfigurace je třeba znát odpovědi na následující otázky:

1. Je brána firewall serveru nakonfigurována tak, že mají klienti k serveru přístup?

2. Může se tento počítač připojit k nadřazenému serveru (například k serveru Microsoft Update)?

3. Znáte název proxy serveru a máte uživatelská pověření k tomuto serveru pro případ potřeby?

Ve výchozím nastavení je aktualizace WSUS 3.0 SP2 nakonfigurována tak, že místem pro získávání aktualizací je web Microsoft Update. Pokud máte v síti proxy server, můžete aktualizaci WSUS 3.0 SP2 nakonfigurovat tak, aby používala proxy server. Je-li mezi serverem WSUS a Internetem podniková brána firewall, měli byste ji pravděpodobně nakonfigurovat tak, aby služba WSUS mohla získávat aktualizace.

 
> [!NOTE]
> I když stahování aktualizací z webu Microsoft Update vyžaduje připojení k Internetu, služba WSUS nabízí možnost importovat aktualizace do sítí, které nejsou připojeny k Internetu.
 

Krok 3 obsahuje následující postupy:

-   Konfigurace brány firewall
-   Určení způsobu, jakým bude tento server získávat aktualizace (buď z webu Microsoft Update, nebo z jiného serveru WSUS)
-   Konfigurace nastavení proxy serveru tak, aby server WSUS mohl získávat aktualizace

**Konfigurace brány firewall**
-   Je-li mezi serverem WSUS a Internetem podniková brána firewall, pravděpodobně bude nutné ji nakonfigurovat tak, aby server WSUS mohl získávat aktualizace. Při získávání aktualizací z webu Microsoft Update používá server WSUS port 80 pro protokol HTTP a port 443 pro protokol HTTPS. Použití těchto portů nelze konfigurovat.

-   Pokud vaše organizace nepovoluje otevření portu 80 nebo 443 pro všechny adresy, můžete omezit přístup pouze na následující domény tak, aby mohl server WSUS a automatické aktualizace komunikovat s webem Microsoft Update:

    -   http://windowsupdate.microsoft.com
    -   http://\*.windowsupdate.microsoft.com
    -   https://\*.windowsupdate.microsoft.com
    -   http://\*.update.microsoft.com
    -   https://\*.update.microsoft.com
    -   http://\*.windowsupdate.com
    -   http://download.windowsupdate.com
    -   http://download.microsoft.com
    -   http://\*.download.windowsupdate.com
    -   http://wustat.windows.com
    -   http://ntservicepack.microsoft.com

 
> [!NOTE]
> Tyto pokyny pro konfiguraci brány firewall jsou určeny pro podnikovou bránu firewall umístěnou mezi serverem WSUS a Internetem. Protože server WSUS spouští veškeré síťové přenosy, není nutné konfigurovat bránu Windows Firewall na serveru WSUS.
 

Ačkoli připojení webu Microsoft Update a serveru WSUS vyžaduje, aby byly porty 80 a 443 otevřené, můžete konfigurovat několik serverů WSUS a synchronizovat je s vlastním portem.

Následující dva postupy předpokládají, že používáte průvodce konfigurací. V další části tohoto kroku bude vysvětleno, jak spustit modul snap-in Správa služby WSUS a konfigurovat server na stránce Možnosti.

**Určení způsobu, jakým bude tento server získávat aktualizace**
1.  Po připojení k Programu zlepšování služby Microsoft Update klikněte v průvodci konfigurací na tlačítko **Další**, abyste mohli vybrat nadřazený server (server pro odesílání dat).

2.  Vyberete-li synchronizaci z webu Microsoft Update, ukončíte postup na stránce Možnosti. Klikněte na tlačítko **Další** nebo vyberte v navigačním podokně možnost **Zadat proxy server**.

3.  Pokud zvolíte možnost synchronizace z jiného serveru WSUS, zadejte název serveru a port, na kterém bude tento server komunikovat s nadřazeným serverem.

4.  Chcete-li používat protokol SSL, zaškrtněte políčko **Při synchronizaci informací o aktualizacích používat protokol SSL**. V takovém případě budou servery používat pro synchronizaci port 443. (Ujistěte se, zda tento server i nadřazený server podporují protokol SSL.)

5.  Jedná-li se o server repliky, zaškrtněte políčko **Toto je replika serveru pro odesílání dat** (tj. nadřazeného serveru).

6.  Konfigurace nadřazeného serveru je tímto bodem dokončena. Klikněte na tlačítko **Další** nebo vyberte v navigačním podokně možnost **Zadat proxy server**.

**Konfigurace nastavení serveru proxy**
1.  Na stránce **Zadat server proxy** průvodce konfigurací zaškrtněte políčko **Při synchronizaci použít server proxy** a potom zadejte do příslušných polí název serveru proxy a číslo portu (ve výchozím nastavení port 80).

2.  Chcete-li se připojit k serveru proxy pomocí zvláštních uživatelských pověření, zaškrtněte políčko **Pro připojení k serveru proxy použít pověření uživatele** a do příslušných polí zadejte uživatelské jméno, doménu a heslo uživatele. Pokud chcete povolit základní ověřování uživatele, který se připojuje k serveru proxy, zaškrtněte políčko **Povolit základní ověření (heslo je odesláno jako prostý text)**.

3.  Konfigurace proxy serveru je tímto bodem dokončena. Kliknutím na tlačítko **Další** přejdete na další stránku, která umožňuje nastavení procesu synchronizace.

V následujících dvou postupech se předpokládá, že při konfiguraci používáte modul snap-in Správa služby WSUS. Tyto dva postupy ukazují, jak lze spustit modul snap-in Správa služby WSUS a nakonfigurovat server na stránce **Možnosti**.

**Spuštění konzoly pro správu služby WSUS**
-   Chcete-li spustit konzolu pro správu služby WSUS, přejděte v nabídce **Start** na příkaz **Všechny programy**, přejděte na příkaz **Nástroje pro správu** a potom klikněte na možnost **Microsoft Windows Server Update Services 3.0**.

 
> [!NOTE]
> Chcete-li používat všechny funkce konzoly, přihlaste se jako člen skupiny Administrators služby WSUS nebo místní skupiny zabezpečení Administrators na serveru, na kterém je nainstalována služba WSUS. Členové skupiny zabezpečení Reporters služby WSUS mají ke konzole přístup jen pro čtení.
 

**Zadání zdroje aktualizací a serveru proxy**
1.  V konzole WSUS klikněte na možnost **Možnosti** pod názvem tohoto serveru v levém podokně a pak klikněte na možnost **Zdroj aktualizací a proxy server** ve středním podokně.

    Zobrazí se dialogové okno s kartami **Zdroj aktualizací** a **Server proxy**.

2.  Na kartě **Zdroj aktualizací** vyberte umístění, ze kterého bude server získávat aktualizace. Pokud vyberete synchronizaci z webu Microsoft Update (výchozí nastavení), bude postup na této stránce dokončen.

3.  Pokud vyberete synchronizaci z jiného serveru WSUS, je třeba zadat port, na kterém budou servery komunikovat (výchozí nastavení je port 80). Pokud vyberete jiný port, měli byste zkontrolovat, zda ho oba servery mohou používat.

4.  Můžete také zadat, zda má být při synchronizaci z nadřazeného serveru WSUS použit protokol SSL. V takovém případě budou servery používat port 443 pro synchronizaci z nadřazeného serveru.

5.  Pokud je tento server replika jiného serveru WSUS, zaškrtněte políčko **Tento server je replika serveru pro odesílání dat**. V takovém případě je třeba všechny aktualizace schválit pouze na nadřazeném serveru WSUS.

6.  Na kartě **Server proxy** zaškrtněte políčko **Při synchronizaci použít server proxy** a potom zadejte do příslušných polí název serveru proxy a číslo portu (ve výchozím nastavení je to port 80).

7.  Chcete-li se připojit k serveru proxy pomocí zvláštních uživatelských pověření, zaškrtněte políčko **Pro připojení k serveru proxy použít pověření uživatele** a do příslušných polí zadejte uživatelské jméno, doménu a heslo uživatele. Pokud chcete pro uživatele připojujícího se k serveru proxy povolit základní ověřování, zaškrtněte políčko **Povolit základní ověření (heslo je odesláno jako prostý text)**.

8.  Nastavení uložte kliknutím na tlačítko **OK**.

Další krok
----------

[Krok 4: Konfigurace aktualizací a synchronizace](https://technet.microsoft.com/deeaa7e1-9b50-45cb-9537-d75f70de3405).

Další zdroje informací
----------------------

[Podrobný průvodce aktualizací Windows Server Update Services 3.0 SP2](https://technet.microsoft.com/4b504edc-93b3-45b0-a7e8-d0107f1a4442)
