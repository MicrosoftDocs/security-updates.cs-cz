---
TOCTitle: 'Krok 3: Konfigurace síťového připojení'
Title: 'Krok 3: Konfigurace síťového připojení'
ms:assetid: 'cd77566d-7780-4ce4-aa56-41183c65c4a7'
ms:contentKeyID: 18126591
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc708559(v=WS.10)'
---

Krok 3: Konfigurace síťového připojení
======================================

Po instalaci služby WSUS jste připraveni získat přístup ke konzole služby WSUS, aby bylo možné konfigurovat službu WSUS a začít s ní pracovat. Při výchozím nastavení je služba WSUS konfigurována na použití serveru Microsoft Update jako místa pro získávání aktualizací. Pokud máte v síti server proxy, použijte konzolu WSUS ke konfiguraci služby WSUS na použití serveru proxy. Pokud se mezi serverem WSUS a Internetem nachází podniková brána firewall, budete možná k zajištění možnosti získávání aktualizací službou WSUS potřebovat konfigurovat bránu firewall.

| ![](images/Cc708559.note(WS.10).gif)Poznámka                                                                                                                                                                                                                                                                                                     |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Ačkoli musíte mít připojení k Internetu, aby bylo možné stahovat aktualizace ze serveru Microsoft Update, nabízí vám služba WSUS možnost importovat aktualizace do sítí, které k Internetu připojeny nejsou. Další informace naleznete v dokumentu White Paper Deploying Microsoft Windows Server Update Services (Nasazení služby Microsoft Windows Server Update Services). |

Krok 3 obsahuje následující postupy:

-   konfigurace brány firewall tak, aby služba WSUS mohla získávat aktualizace,
-   spuštění konzoly WSUS,
-   konfigurace nastavení serveru proxy tak, aby služba WSUS mohla získávat aktualizace.

**Konfigurace brány firewall**
-   Pokud se mezi serverem WSUS a Internetem nachází podniková brána firewall, bude k zajištění možnosti získávání aktualizací službou WSUS pravděpodobně nutné nakonfigurovat bránu firewall. K získávání aktualizací ze serveru Microsoft Update používá server WSUS port 80 pro protokol HTTP a port 443 pro protokol HTTPS. Tyto možnosti nelze konfigurovat.

-   Pokud vaše organizace nepovoluje otevření těchto portů a protokolů pro všechny adresy, můžete omezit přístup pouze na následující domény tak, aby mohl server WSUS a služba Automatické aktualizace komunikovat se službou Microsoft Updates:

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

| ![](images/Cc708559.note(WS.10).gif)Poznámka                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Výše uvedené kroky pro konfiguraci brány firewall jsou určeny pro podnikovou bránu firewall umístěnou mezi serverem WSUS a Internetem. Protože server WSUS zahajuje veškerý svůj síťový provoz, není na serveru WSUS nutné konfigurovat Bránu firewall systému Windows. Ačkoli připojení serveru Microsoft Update a WSUS vyžaduje, aby byly porty 80 a 443 otevřené, můžete konfigurovat více serverů WSUS pro synchronizaci s vlastním portem. Další informace o synchronizaci serveru WSUS naleznete v dokumentu White Paper Deploying Microsoft Windows Server Update Services (Nasazení služby Microsoft Windows Server Update Services). |

**Spuštění konzoly WSUS**
-   Na serveru WSUS klepněte na tlačítko **Start**, přejděte na položku **Všechny programy**, na položku **Nástroje pro správu** a potom klepněte na možnost **Služba Microsoft Windows Server Update Services**.

| ![](images/Cc708559.note(WS.10).gif)Poznámka                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Abyste mohli použít konzolu služby WSUS, musíte být členem skupiny WSUS Administrators nebo místní skupiny zabezpečení Administrators na serveru, na kterém je nainstalována služba WSUS. Pokud nepřidáte server **http://&lt;***název webového serveru WSUS***&gt;** do seznamu serverů v místní zóně sítě intranet v aplikaci Internet Explorer na serveru Windows Server 2003, může se vám při každém otevření konzoly WSUS zobrazit výzva k zadání pověření. Pokud změníte přiřazení portu ve službě IIS po instalaci služby WSUS, je nutné ručně aktualizovat zástupce v nabídce **Start**. Také můžete otevřít konzolu WSUS z aplikace Internet Explorer na kterémkoli serveru nebo v počítači v síti tak, že zadáte následující adresu URL: **http://***WSUSservername***/WSUSAdmin** |

**Zadání serveru proxy**
1.  Na panelu nástrojů konzoly služby WSUS klepněte na tlačítko **Možnosti** a potom na odkaz **Možnosti synchronizace**.

2.  V části **Server proxy** zaškrtněte políčko **Při synchronizaci použít server proxy** a potom zadejte do příslušných polí název serveru proxy a číslo portu (při výchozím nastavení je to port 80).

3.  Chcete-li se připojit k serveru proxy pomocí specifických uživatelských pověření, zaškrtněte políčko **Pro připojení k serveru proxy použít pověření uživatele** a do příslušných polí zadejte uživatelské jméno, doménu a heslo uživatele. Pokud chcete pro uživatele připojujícího se k serveru proxy povolit základní ověřování, zaškrtněte políčko **Povolit základní ověření (heslo je odesláno jako prostý text)**.

4.  Ve skupinovém rámečku **Úkoly** klepněte na odkaz **Uložit nastavení** a potom klepněte na tlačítko **OK**.
