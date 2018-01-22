---
TOCTitle: 'Krok 2: Instalace služby WSUS 3.0 na vašem serveru'
Title: 'Krok 2: Instalace služby WSUS 3.0 na vašem serveru'
ms:assetid: '191e62a0-7671-41eb-9841-17c64313fa68'
ms:contentKeyID: 18126464
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc720469(v=WS.10)'
---

Krok 2: Instalace služby WSUS 3.0 na vašem serveru
==================================================

Po ověření, zda server splňuje instalační požadavky, můžete začít instalovat službu WSUS 3.0. Je třeba se přihlásit k serveru, na který chcete instalovat službu WSUS 3.0, pomocí účtu, který je členem místní skupiny Administrators. Nainstalovat službu WSUS 3.0 mohou pouze členové místní skupiny Administrators.

Následující postup používá výchozí možnosti instalace služby WSUS, což zahrnuje instalaci softwaru Interní databáze systému Windows pro databázi služby WSUS 3.0, místní ukládání aktualizací a použití výchozího webového serveru Internetové informační služby na portu 80.

**Instalace služby WSUS 3.0**
1.  Poklepejte na instalační soubor **WSUSSetup.exe**.

2.  Na stránce **Vítáme vás** v průvodci instalací klepněte na tlačítko **Další**.

3.  Na stránce **Výběr režimu instalace** klepněte na možnost **Úplná instalace na serveru včetně konzoly pro správu** (pokud do počítače chcete nainstalovat server) nebo **Pouze konzola pro správu** (pokud chcete nainstalovat pouze konzolu pro správu).

4.  Na stránce **Licenční smlouva** si pozorně přečtěte podmínky licenční smlouvy, klepněte na možnost **S podmínkami licenční smlouvy souhlasím** a potom klepněte na tlačítko **Další**.

    ![](images/Cc720469.fa6ac6a6-6814-4b7e-96e8-e08af5e534b8(WS.10).gif)

5.  Na stránce průvodce instalací **Vyberte zdroj aktualizace** je možné zadat, odkud mají klienti získávat aktualizace. Pokud zaškrtnete políčko **Ukládat aktualizace místně**, jsou aktualizace uloženy na serveru WSUS 3.0 a vyberete umístění v systému souborů pro ukládání aktualizací. Pokud neukládáte aktualizace místně, připojují se klientské počítače k serveru Microsoft Update, kde získávají schválené aktualizace. Zachovejte výchozí možnosti a klepněte na tlačítko **Další**.

    ![](images/Cc720469.c8bac396-ca39-4491-8b0c-742a0e470535(WS.10).gif)

6.  Na stránce **Možnosti databáze** vyberte software používaný ke správě databáze služby WSUS 3.0. Při výchozím nastavení nabízí instalační program služby WSUS instalaci softwaru Interní databáze systému Windows, pokud počítač, ve kterém provádíte instalaci, používá systém Windows Server 2003.

7.  Pokud nechcete používat software Interní databáze systému Windows, je třeba poskytnout službě WSUS instanci serveru SQL Server, kterou má používat. Tuto instanci zadáte tak, že klepnete na možnost **Použít** **existující databázový server v počítači** a zadáte název instance do příslušného pole. Název instance se zadává ve formátu &lt;*Název\_Serveru*&gt;\\&lt;*Název\_Instance*&gt;, kde *Název\_Serveru* je název daného serveru a *Název\_Instance* je název instance SQL. Proveďte výběr a klepněte na tlačítko **Další**.

8.  Na stránce **Připojování k instanci serveru SQL** se služba WSUS pokusí připojit k příslušné instanci serveru SQL Server. Až připojení proběhne úspěšně, pokračujte klepnutím na tlačítko **Další**.

    ![](images/Cc720469.36c6af0c-a61e-4151-ae50-c754a106cb1b(WS.10).gif)

9.  Na stránce **Výběr webového serveru** zadejte webový server, který bude služba WSUS 3.0 používat. Pokud si přejete použít výchozí webový server Internetové informační služby na portu 80, zvolte první možnost. Pokud již na portu 80 nějaký webový server máte, lze výběrem druhé možnosti vytvořit alternativní webový server na portu 8530. Zachovejte výchozí možnost a klepněte na tlačítko **Další**.

10. Na stránce **Instalace služby Microsoft Windows Server Update Services je připravena** zkontrolujte vybrané možnosti a potom klepněte na tlačítko **Další**.

11. Poslední stránka průvodce instalací vám sdělí, zda byla instalace služby WSUS 3.0 dokončena úspěšně. Po klepnutí na tlačítko **Dokončit** se spustí průvodce konfigurací.
