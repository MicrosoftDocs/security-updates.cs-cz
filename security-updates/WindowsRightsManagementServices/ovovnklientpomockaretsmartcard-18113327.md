---
TOCTitle: Ověřování klientů pomocí karet Smart Card
Title: Ověřování klientů pomocí karet Smart Card
ms:assetid: '5caacd67-fb16-46f1-b1ad-4aef0a632bf0'
ms:contentKeyID: 18113327
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747579(v=WS.10)'
---

Ověřování klientů pomocí karet Smart Card
=========================================

Pokud k vyššímu zabezpečení a kontrole uživatelských pověření v organizaci používáte karty Smart Card, můžete pomocí těchto karet nyní ze serveru RMS získat certifikáty účtů práv a licence k použití. Chcete-li server RMS nastavit tak, aby vyžadoval ověření klienta, je nutné povolit protokol SSL (Secure Sockets Layer) u webu, na kterém je zajištěna služba RMS, a nakonfigurovat způsob ověřování v Internetové informační službě (IIS). Uvedený úkol je možné provést následujícím způsobem:

1.  Otevřete modul snap-in pro **správu Internetové informační služby**.
2.  Rozbalte položku serveru, klepněte pravým tlačítkem myši na webovou složku a pak klepněte na tlačítko **Vlastnosti**.
3.  Klepněte na kartu **Zabezpečení adresáře** a pak zaškrtněte v části **Zabezpečená komunikace** políčko **Povolit mapování adresářových služeb systému Windows**.
4.  Rozbalte složku webového serveru, otevřete virtuální adresář **\_wmcs** a pak rozbalte virtuální adresář (**Správa licencí** nebo **Certifikát**), pro který chcete konfigurovat ověřování.
    -   Chcete-li konfigurovat ověřování, pokud uživatel vyžaduje licenci k použití, klepněte pravým tlačítkem myši na soubor license.asmx a pak klepněte na příkaz **Vlastnosti**.
    -   Chcete-li konfigurovat ověřování, pokud uživatel vyžaduje certifikát uživatele, klepněte pravým tlačítkem myši na soubor certification.asmx a pak klepněte na příkaz **Vlastnosti**.
5.  Klepněte na kartu **Zabezpečení souboru** a v části **Zabezpečená komunikace** otevřete klepnutím na tlačítko **Upravit** dialogové okno **Zabezpečená komunikace**.
6.  Vyberte možnost **Vyžadovat zabezpečený kanál (SSL)** a klepněte na některou z následujících možností:
    -   **Vyžadovat klientské certifikáty**, pokud chcete, aby se ke službě mohli připojit pouze klienti s certifikáty klienta, například s kartami Smart Card.
    -   **Přijímat klientské certifikáty**, pokud chcete, aby klienti měli možnost poskytnout pověření pomocí certifikátů na kartě Smart Card nebo zadáním uživatelského jména a hesla.
7.  Vyberte možnost **Povolit mapování klientských certifikátů** a pak klepněte na tlačítko **OK**.
8.  Chcete-li použít ověřování klientů pro certifikaci i správu licencí, opakujte tento postup a vyberte přitom druhý virtuální adresář.

Po konfiguraci tohoto nastavení se uživateli, který se pokusí otevřít obsah chráněný službou RMS publikovaný na tomto serveru, zobrazí výzva k zadání ověřovacích pověření, až poté server poskytne uživateli certifikát s oprávněními k účtu nebo licenci k použití.
