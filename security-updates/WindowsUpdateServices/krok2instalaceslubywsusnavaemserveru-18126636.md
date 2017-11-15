---
TOCTitle: 'Krok 2: Instalace služby WSUS na vašem serveru'
Title: 'Krok 2: Instalace služby WSUS na vašem serveru'
ms:assetid: 'f593532c-e92e-47f3-914a-38a6c2519e94'
ms:contentKeyID: 18126636
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc708622(v=WS.10)'
---

Krok 2: Instalace služby WSUS na vašem serveru
==============================================

Po kontrole instalačních požadavků jste připraveni instalovat službu WSUS. Musíte se přihlásit k serveru, na který chcete instalovat službu WSUS, pomocí účtu, který je členem místní skupiny Administrators. Instalovat službu WSUS mohou pouze členové místní skupiny Administrators.

Následující postup používá výchozí možnosti instalace služby WSUS pro systém Windows Server 2003, což zahrnuje instalaci softwaru Windows SQL Server™ 2000 Desktop Engine (WMSDE) pro databázový software WSUS, místní ukládání aktualizací a použití výchozího webu služby IIS na portu 80. Postupy pro vlastní možnosti instalace, jako například použití různých operačních systémů, různých databázových softwarů nebo webu pomocí vlastního čísla portu, naleznete v dokumentu White Paper Deploying Microsoft Server Windows Update Services (Nasazení služby Microsoft Windows Server Update Services).

**Instalace služby WSUS na serveru Windows Server 2003**
1.  Poklepejte na instalační soubor **WSUSSetup.exe**.

>Poznámka     
>Nejnovější verze souboru WSUSSetup.exe pro službu Windows Server Update Services je k dispozici na [webu společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=47374) pro službu Windows Server Update Services na adrese http://go.microsoft.com/fwlink/?LinkId=47374. 

2.  Na stránce **Vítáme vás** v průvodci klepněte na tlačítko **Další**.

3.  Pozorně si přečtěte podmínky licenční smlouvy, klepněte na možnost **S podmínkami licenční smlouvy souhlasím** a potom klepněte na tlačítko **Další**.

4.  Na stránce **Vyberte zdroj aktualizace** je možné zadat, kde získávají klienti aktualizace. Pokud zaškrtnete políčko **Ukládat aktualizace místně**, jsou aktualizace uloženy na serveru WSUS a vy vyberete místo v systému souborů pro ukládání aktualizací. Pokud neukládáte aktualizace místně, připojují se klientské počítače k serveru Microsoft Update, kde získávají schválené aktualizace.

    Zachovejte výchozí možnosti a klepněte na tlačítko **Další**.

    ![](images/Cc708622.fa6ac6a6-6814-4b7e-96e8-e08af5e534b8(WS.10).gif)

5.  Na stránce **Možnosti databáze** vyberte software používaný ke správě databáze služby WSUS. Při výchozím nastavení nabízí instalační program služby WSUS instalaci softwaru WMSDE, pokud počítač, ve kterém provádíte instalaci, používá systém Windows Server 2003.

    Pokud nemůžete použít software WMSDE, je třeba poskytnout pro službu WSUS k použití instanci serveru SQL Server tak, že klepnete na možnost **Použít existující databázový server v počítači** a zadáte název instance do pole **Vyberte název instance serveru SQL**. Další informace o možnostech použití databázového softwaru vedle softwaru WMSDE naleznete v dokumentu White Paper Deploying Microsoft Windows Server Update Services (Nasazení služby Microsoft Windows Server Update Services).

    Zachovejte výchozí možnosti a klepněte na tlačítko **Další**.

    ![](images/Cc708622.bc0b73ad-b338-437c-a3c7-0299e819840d(WS.10).gif)

6.  Na stránce **Výběr webového serveru** zadejte webový server, který bude služba WSUS používat. Tato stránka také obsahuje na základě tohoto výběru dvě důležité adresy URL: Adresu URL, na kterou budou směrovány klientské počítače WSUS k získávání aktualizací, a adresu URL pro konzolu WSUS, kde budete konfigurovat službu WSUS.

    Pokud již máte web na portu 80, budete možná muset vytvořit web WSUS na vlastním portu. Další informace o spuštění služby WSUS na vlastním portu naleznete v dokumentu White Paper Deploying Microsoft Windows Server Update Services (Nasazení služby Microsoft Windows Server Update Services).

    Zachovejte výchozí možnost a klepněte na tlačítko **Další**.

    ![](images/Cc708622.64ed7643-a050-4f54-bf9f-04cf7931adc0(WS.10).gif)

7.  Na stránce **Zrcadlení nastavení aktualizací** je možné zadat roli správy pro tento server WSUS. Pokud se jedná o první server WSUS v síti nebo pokud požadujete topologii distribuované správy, vynechejte tuto obrazovku.

    Požadujete-li topologii centrální správy a nejedná se o první server WSUS ve vaší síti, zaškrtněte políčko a zadejte název dalšího serveru WSUS do pole **Název serveru**. Další informace o rolích správy naleznete v dokumentu White Paper Deploying Microsoft Windows Server Update Services (Nasazení služby Microsoft Windows Server Update Services).

    Zachovejte výchozí možnost a klepněte na tlačítko **Další**.

    ![](images/Cc708622.f26e09d5-983c-418d-8511-8960850403ef(WS.10).gif)

8.  Na stránce **Instalace služby Microsoft Windows Server Update Services je připravena** zkontrolujte vybrané možnosti a klepněte na tlačítko **Další**.

    ![](images/Cc708622.20de7d09-3d30-4867-9253-6f353dd1923d(WS.10).gif)

9.  Pokud poslední stránka průvodce potvrdí, že instalace služby WSUS byla úspěšně dokončena, klepněte na tlačítko **Dokončit**.
