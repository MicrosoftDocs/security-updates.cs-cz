---
TOCTitle: 'Krok 2: Instalace serveru WSUS nebo konzoly pro správu'
Title: 'Krok 2: Instalace serveru WSUS nebo konzoly pro správu'
ms:assetid: '6db6fcb0-c55d-43b9-9b07-4040c6267759'
ms:contentKeyID: 21741124
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Dd939859(v=WS.10)'
---

Krok 2: Instalace serveru WSUS nebo konzoly pro správu
======================================================

Jakmile se ujistíte, že server splňuje minimální požadavky na systém a že byla udělena potřebná oprávnění účtu, jste připraveni k instalaci aktualizace Windows Server Upgrade Services 3.0 Service Pack 2 (WSUS 3.0 SP2). Spusťte instalaci aktualizace WSUS 3.0 SP2 pomocí postupu vhodného pro váš operační systém a druh instalace (pomocí Správce serveru nebo souboru WUSSetup.exe).

Použití Správce serveru
-----------------------

**Spuštění instalace aktualizace WSUS 3.0 SP2 pomocí Správce serveru**
1.  Přihlaste se k serveru, na který chcete instalovat aktualizaci WSUS 3.0 SP2, pomocí účtu, který je členem místní skupiny Administrators.

2.  Klikněte na tlačítko **Start**, přejděte na položku **Nástroje pro správu** a klikněte na příkaz **Správce serveru**.

3.  V pravém podokně okna Správce serveru klikněte v části Souhrn rolí na možnost **Přidat role**.

4.  Zobrazí-li se stránka Než začnete, klikněte na tlačítko **Další**.

5.  Na stránce Vybrat role serveru vyberte možnost **Windows Server Update Services**.

6.  Na stránce Windows Server Update Services klikněte na tlačítko **Další**.

7.  Na stránce Potvrdit vybrané možnosti instalace klikněte na tlačítko **Nainstalovat**.

8.  Po spuštění průvodce instalací aktualizace WSUS 3.0 SP2 vynechejte další část a zobrazte postup Pokračování v instalaci aktualizace WSUS 3.0 SP2.

Použití souboru WUSSetup.exe
----------------------------

**Spuštění instalace serveru WSUS 3.0 SP2 nebo konzoly pro správu služby WSUS 3.0 SP2 pomocí souboru WUSSetup.exe**
1.  Přihlaste se k serveru, na který chcete instalovat aktualizaci WSUS 3.0 SP2, pomocí účtu, který je členem místní skupiny Administrators.

2.  Dvakrát klikněte na instalační soubor **WSUSSetup.exe**.

3.  Po spuštění průvodce instalací aktualizace Windows Server Update Services 3.0 SP2 zobrazte postup Pokračování v instalaci aktualizace WSUS 3.0 SP2.

Použití průvodce instalací aktualizace WSUS 3.0 SP2
---------------------------------------------------

Průvodce instalací služby WSUS je spuštěn pomocí Správce serveru nebo pomocí souboru WUSSetup.exe.

**Pokračování v instalaci aktualizace WSUS 3.0 SP2**
1.  Na úvodní stránce průvodce instalací aktualizace Windows Server Update Services 3.0 klikněte na tlačítko **Další**.

2.  Na stránce Výběr režimu instalace klikněte na možnost **Úplná instalace na serveru včetně konzoly pro správu** (pokud do počítače chcete nainstalovat server WSUS) nebo **Pouze konzola pro správu** (pokud chcete nainstalovat pouze konzolu pro správu).

3.  Na stránce Licenční smlouva si přečtěte podmínky licenční smlouvy, klikněte na možnost **S podmínkami licenční smlouvy souhlasím** a potom klikněte na tlačítko **Další**.

4.  Na stránce Vybrat zdroj aktualizace v průvodci instalací můžete určit, odkud budou klienti získávat aktualizace. Ve výchozím nastavení je zaškrtnuto políčko **Ukládat aktualizace místně** a aktualizace budou ukládány do vámi zadaného umístění na serveru WSUS. Pokud zrušíte zaškrtnutí políčka **Ukládat aktualizace místně**, budou klientské počítače získávat schválené aktualizace připojením ke službě Microsoft Update. Proveďte výběr a klikněte na tlačítko **Další**.

5.  Na stránce Možnosti databáze vyberte software používaný ke správě databáze služby WSUS 3.0. Průvodce instalací ve výchozím nastavení nabídne instalaci interní databáze systému Windows.

    Pokud nechcete použít interní databázi systému Windows, zadejte instanci serveru SQL pro službu WSUS výběrem možnosti **Použít existující databázový server v tomto počítači** nebo **Použít existující databázový server ve vzdáleném počítači**. Do příslušného pole zadejte název instance. Název instance se zadává ve formátu &lt;*Název\_Serveru*&gt;\\&lt;*Název\_Instance*&gt;, kde *Název\_Serveru* je název daného serveru a *Název\_Instance* je název instance SQL. Proveďte výběr a klikněte na tlačítko **Další**.

6.  Pokud jste se rozhodli připojit k serveru SQL, pokusí se služba WSUS na stránce **Připojování k instanci serveru SQL** připojit k příslušné instanci serveru SQL. Až připojení proběhne úspěšně, pokračujte kliknutím na tlačítko **Další**.

7.  Na stránce Výběr webového serveru zadejte webový server, který bude služba WSUS používat. Pokud chcete používat výchozí web na portu 80, vyberte možnost **Použít existující výchozí web služby IIS**. Pokud web na portu 80 již existuje, můžete vytvořit alternativní web na portu 8530 výběrem možnosti **Vytvořit web služby Windows Server Update Services 3.0 SP2**. Klikněte na tlačítko **Další**.

8.  Na stránce **Instalace služby Microsoft Windows Server Update Services je připravena** zkontrolujte vybrané možnosti a potom klikněte na tlačítko **Další**.

9.  Na poslední stránce průvodce instalací se dozvíte, zda byla instalace služby WSUS úspěšně dokončena. Po kliknutí na tlačítko **Dokončit** se spustí průvodce konfigurací.

Další krok
----------

[Krok 3: Konfigurace síťových připojení](https://technet.microsoft.com/42a144c5-f08e-4a6e-b360-47ddea77bd24)

Další zdroje informací
----------------------

[Podrobný průvodce aktualizací Windows Server Update Services 3.0 SP2](https://technet.microsoft.com/4b504edc-93b3-45b0-a7e8-d0107f1a4442)
