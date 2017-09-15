---
TOCTitle: Změna nastavení serveru proxy služby RMS
Title: Změna nastavení serveru proxy služby RMS
ms:assetid: '8f50bd4d-26b1-4996-b361-722ee21607f3'
ms:contentKeyID: 18113364
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747594(v=WS.10)'
---

Změna nastavení serveru proxy služby RMS
========================================

Provedení tohoto postupu vyžaduje, aby byl uživatel místně přihlášen k webu pro správu v rámci uživatelského účtu, který je členem skupiny Administrators v počítači, k němuž získává přístup. Uvedený postup mohou provést také členové skupiny Domain Admins. Z hlediska zabezpečení je nejvhodnější při provádění tohoto postupu použít příkaz **Spustit jako**.

Další informace o způsobech ověřování serveru proxy a jejich funkci v systému Windows Server 2003 naleznete v nápovědě k Internetové informační službě.

Změna nastavení serveru proxy služby RMS
----------------------------------------

#### Změna nastavení serveru proxy služby RMS

1.  Otevřete stránku **Globální správa** a poté klepněte na položku **Spravovat službu RMS na tomto webu**.

2.  V části **Správa clusteru** klepněte na položku **Nastavení zabezpečení**.

3.  Pokud jste dosud server proxy v rámci služby RMS nepoužívali, zaškrtněte políčko **Tento server používá k připojení k Internetu server proxy**. Na stránce se zobrazí další nastavení, která je nutné zadat.

4.  Do pole **Adresa** zadejte adresu IP nebo název DNS požadovaného serveru proxy.

5.  Do pole **Port** zadejte číslo portu, který server proxy používá k připojení k Internetu.

6.  Pokud server proxy nepoužíváte pro připojení k místním prostředkům, zaškrtněte políčko **Nepoužívat server proxy pro adresy vnitřní sítě**.

7.  V případě potřeby zaškrtněte políčko **Tento server proxy vyžaduje ověřování**.

    -   V seznamu vyberte požadovanou možnost ověřování. K dispozici jsou možnosti **Základní**, **Algoritmus Digest** a **Integrované ověřování systému Windows**.
    -   Do pole **Uživatelské jméno** zadejte uživatelské jméno, které by mělo být zadáváno jako odpověď na výzvy serveru proxy.
    -   Do pole **Heslo** zadejte heslo, které by mělo být zadáváno jako odpověď na výzvy serveru proxy.
    -   Do pole **Potvrzení hesla** znovu zadejte již zadané heslo. Ověříte tak, zda jste je zadali správně.
    -   Pokud server proxy používá integrované ověřování systému Windows, zadejte do pole **Doména** doménu, do níž uživatel patří.

8.  Klepněte na tlačítko **Odeslat**.
