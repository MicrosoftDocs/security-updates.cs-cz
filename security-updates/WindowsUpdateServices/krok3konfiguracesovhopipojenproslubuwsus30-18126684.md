---
TOCTitle: 'Krok 3: Konfigurace síťového připojení pro službu WSUS 3.0'
Title: 'Krok 3: Konfigurace síťového připojení pro službu WSUS 3.0'
ms:assetid: 'dbc9d9f7-cf52-4539-9f9e-3e823273218a'
ms:contentKeyID: 18126684
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc708602(v=WS.10)'
---

Krok 3: Konfigurace síťového připojení pro službu WSUS 3.0
==========================================================

Po instalaci služby WSUS 3.0 se automaticky spustí průvodce konfigurací. Je možné jej také spustit později prostřednictvím stránky **Možnosti** v konzole služby WSUS 3.0.

Před začátkem procesu konfigurace je třeba znát odpovědi na následující otázky:

1. Je brána firewall serveru nakonfigurována tak, že mají klienti k serveru přístup?

2. Může se tento počítač připojit k serveru pro odesílání dat (například k serveru Microsoft Update)?

3. Znáte název serveru proxy a uživatelská pověření k tomuto serveru pro případ potřeby?

Ve výchozím nastavení je služba WSUS nakonfigurována tak, že místem pro získávání aktualizací je web Microsoft Update. Pokud máte v síti server proxy, můžete službu WSUS nakonfigurovat tak, aby používala server proxy. Je-li mezi serverem WSUS a Internetem podniková brána firewall, měli byste ji nakonfigurovat tak, aby služba WSUS mohla získávat aktualizace.

| ![](images/Cc708602.note(WS.10).gif)Poznámka                                                                                                           |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| I když stahování aktualizací z webu Microsoft Update vyžaduje připojení k Internetu, služba WSUS nabízí možnost importovat aktualizace do sítí, které nejsou připojeny k Internetu. |

**Krok 3 obsahuje následující postupy**:

-   konfigurace brány firewall,
-   určení způsobu, jakým bude tento server získávat aktualizace (buď z webu Microsoft Update, nebo z jiného serveru WSUS),
-   konfigurace nastavení serveru proxy, které službě WSUS umožní získávat aktualizace.

**Konfigurace brány firewall**
-   Je-li mezi serverem WSUS a Internetem podniková brána firewall, měli byste ji nakonfigurovat tak, aby služba WSUS mohla získávat aktualizace. Při získávání aktualizací z webu Microsoft Update používá server WSUS port 80 pro protokol HTTP a port 443 pro protokol HTTPS. Použití těchto portů nelze konfigurovat.

-   Pokud vaše organizace nepovoluje otevření portu 80 nebo 443 pro všechny adresy, můžete omezit přístup pouze na následující domény tak, aby mohl server WSUS a služba Automatické aktualizace komunikovat s webem Microsoft Update:

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

| ![](images/Cc708602.note(WS.10).gif)Poznámka                                                                                                                                                                                   |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Tyto pokyny pro konfiguraci brány firewall jsou určeny pro podnikovou bránu firewall umístěnou mezi serverem WSUS a Internetem. Protože server WSUS spouští veškeré síťové přenosy, není nutné konfigurovat Bránu firewall systému Windows na serveru WSUS. |

Ačkoli připojení webu Microsoft Update a serveru WSUS vyžaduje, aby byly porty 80 a 443 otevřené, můžete konfigurovat několik serverů WSUS a synchronizovat je s vlastním portem.

Následující dva postupy předpokládají, že používáte průvodce konfigurací. V další části tohoto kroku bude vysvětleno, jak spustit modul snap-in pro správu služby WSUS a konfigurovat server na stránce **Možnosti**.

**Určení způsobu, jakým bude tento server získávat aktualizace**
1.  Po připojení k programu Zlepšování softwaru a služeb společnosti Microsoft klepněte v průvodci konfigurací na tlačítko **Další**, abyste vybrali server pro odesílání dat.

2.  Vyberete-li synchronizaci z webu Microsoft Update, ukončíte postup na této stránce. Klepněte na tlačítko **Další** nebo vyberte v levém panelu možnost **Zadat proxy server**.

3.  Pokud zvolíte možnost synchronizace z jiného serveru WSUS, zadejte název serveru a port, na kterém bude tento server komunikovat se serverem pro odesílání dat.

4.  Chcete-li používat protokol SSL, zaškrtněte políčko **Při synchronizaci informací o aktualizacích používat protokol SSL**. V takovém případě budou servery používat pro synchronizaci port 443. (Měli byste ověřit, zda tento server i server pro odesílání dat podporují protokol SSL.)

5.  Jedná-li se o server repliky, zaškrtněte políčko **Tento server je replika serveru pro odesílání dat**.

6.  Konfigurace serveru pro odesílání dat je tímto bodem dokončena. Klepněte na tlačítko **Další** nebo vyberte v levém panelu možnost **Zadat server proxy**.

**Konfigurace nastavení serveru proxy**
1.  Na stránce **Zadat server proxy** průvodce konfigurací zaškrtněte políčko **Při synchronizaci použít server proxy** a potom zadejte do příslušných polí název serveru proxy a číslo portu (ve výchozím nastavení port 80).

2.  Chcete-li se připojit k serveru proxy pomocí zvláštních uživatelských pověření, zaškrtněte políčko **Pro připojení k serveru proxy použít pověření uživatele** a do příslušných polí zadejte uživatelské jméno, doménu a heslo uživatele. Pokud chcete povolit základní ověřování uživatele, který se připojuje k serveru proxy, zaškrtněte políčko **Povolit základní ověření (heslo je odesláno jako prostý text)**.

3.  Konfigurace serveru proxy je tímto bodem dokončena. Kleputím na tlačítko **Další** přejdete na další stránku, která umožňuje nastavení procesu synchronizace.

V následujících dvou postupech se předpokládá, že při konfiguraci používáte modul snap-in Správa služby WSUS. Tyto dva postupy ukazují, jak lze spustit modul snap-in Správa služby WSUS a nakonfigurovat server na stránce **Možnosti**.

**Spuštění konzoly pro správu služby WSUS**
-   Chcete-li spustit konzolu pro správu služby WSUS, přejděte v nabídce **Start** na příkaz **Všechny programy**, přejděte na příkaz **Nástroje pro správu** a potom klepněte na možnost **Microsoft Windows Server Update Services 3.0**.

| ![](images/Cc708602.note(WS.10).gif)Poznámka                                                                                                                                                                                                                             |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Všechny funkce konzoly služby WSUS mohou používat pouze členové skupiny WSUS Administrators nebo místní skupiny zabezpečení Administrators na serveru, na kterém je nainstalována služba WSUS. Členové skupiny zabezpečení Zpravodajové služby WSUS mají ke konzole pro správu přístup jen pro čtení. |

**Zadání zdroje aktualizací a serveru proxy**
1.  V konzole WSUS klepněte na možnost **Možnosti** pod názvem tohoto serveru v levém panelu a pak klepněte na možnost **Zdroj aktualizací a server proxy** ve středním panelu.

2.  Zobrazí se dialogové okno s kartami **Zdroj aktualizací** a **Server proxy**.

3.  Na kartě **Zdroj aktualizací** vyberte umístění, ze kterého bude server získávat aktualizace. Pokud vyberete synchronizaci z webu Microsoft Update (výchozí nastavení), bude postup na této stránce dokončen.

4.  Pokud vyberete synchronizaci z jiného serveru WSUS, je třeba zadat port, na kterém budou servery komunikovat (výchozí nastavení je port 80). Pokud vyberete jiný port, měli byste zkontrolovat, zda ho oba servery mohou používat.

5.  Můžete také zadat, zda má být při synchronizaci ze serveru WSUS pro odesílání dat použit protokol SSL. V takovém případě budou servery používat port 443 pro synchronizaci ze serveru pro odesílání dat.

6.  Pokud je tento server replika jiného serveru WSUS, zaškrtněte políčko **Tento server je replika serveru pro odesílání dat**. V takovém případě je třeba všechny aktualizace schválit pouze na serveru WSUS pro odesílání dat.

7.  Na kartě **Server proxy** zaškrtněte políčko **Při synchronizaci použít server proxy** a potom zadejte do příslušných polí název serveru proxy a číslo portu (ve výchozím nastavení je to port 80).

8.  Chcete-li se připojit k serveru proxy pomocí zvláštních uživatelských pověření, zaškrtněte políčko **Pro připojení k serveru proxy použít pověření uživatele** a do příslušných polí zadejte uživatelské jméno, doménu a heslo uživatele. Pokud chcete pro uživatele připojujícího se k serveru proxy povolit základní ověřování, zaškrtněte políčko **Povolit základní ověření (heslo je odesláno jako prostý text)**.

9.  Nastavení uložte klepnutím na tlačítko **OK**.
