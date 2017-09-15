---
TOCTitle: Způsob nasazení klienta RMS
Title: Způsob nasazení klienta RMS
ms:assetid: 'c84f1724-cf71-4385-9003-ff68bc23c927'
ms:contentKeyID: 18113505
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747749(v=WS.10)'
---

Způsob nasazení klienta RMS
===========================

Používáte-li systém Microsoft Windows XP nebo Microsoft Windows 2000, je třeba nainstalovat klienta Služby správy přístupových práv (RMS), aby bylo možné používat funkce služby RMS, například technologii IRM (Správa přístupových práv k informacím) v sadě Office 2003 a doplněk Správa práv pro aplikaci Internet Explorer. Klient RMS je integrován do systému Windows Vista®.

Řada organizací chce řídit nasazování klientského softwaru sama. K nasazení klienta RMS s aktualizací Service Pack 2 (SP2) lze použít server SMS (Systems Management Server) nebo zásady skupiny.

Před zahájením nasazení stáhněte klienta RMS z webu [http://go.microsoft.com/fwlink/?LinkId=67736](http://go.microsoft.com/fwlink/?linkid=67736) (stránka může být v angličtině).

| ![](images/Cc747749.Important(WS.10).gif)Důležité informace                 |
|----------------------------------------------------------------------------------------------------------|
| Klient RMS byl integrován do systému Windows Vista. Proto již není nutné provádět samostatnou instalaci. |

Extrahování a instalace souborů
-------------------------------

Po stažení souboru WindowsRightsManagementServicesSP2-KB917275-Client-CSY.exe je nutné ze spustitelného balíčku extrahovat soubory Instalační služby systému Microsoft® Windows®.

Uvedený krok můžete provést zadáním následujícího příkazu na příkazovém řádku:

`WindowsRightsManagementServicesSP2-KB917275-Client-ENU.exe /x <path>`

kde &lt;cesta&gt; je cílový adresář, do kterého budete chtít uložit extrahované soubory.

Spuštěním tohoto příkazu budou do zvoleného cílového adresáře extrahovány následující soubory:

-   Bootstrap.exe
    Jedná se o soubor balíčku používaný spustitelným souborem k instalaci ostatních zahrnutých souborů. Nepoužívá se k instalaci klienta RMS s aktualizací SP2 pomocí serveru SMS nebo zásad skupiny.
-   MSDrmClient.msi
    Jedná se o instalační soubor pro klienta RMS s aktualizací SP2. Odinstaluje všechny předchozí verze klienta RMS v počítači. Tento program je potřeba nejdříve nainstalovat do klientských počítačů.
-   RMClientBackCompat.msi
    Jedná se o instalační soubor umožňující zjistit nového klienta RMS s aktualizací SP2 v aplikacích s podporou služby RMS (například v sadě Microsoft Office Professional 2003 nebo v systému Microsoft Office 2007), které jsou závislé na předchozí verzi klienta RMS, aby bylo možné místo něj použít klienta RMS s aktualizací SP2. Tento program by měl být nainstalován do klientských počítačů po úspěšné instalaci souboru MSDrmClient.msi.

| ![](images/Cc747749.note(WS.10).gif)Poznámka                                                                                                                                                                                 |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Bez ohledu na to, který způsob instalace zvolíte, je nutné úspěšně nainstalovat oba soubory Instalační služby systému Windows. Pokud by došlo k chybě, která by znemožnila instalaci souboru MSDrmClient.msi, neinstalujte soubor RMClientBackCompat.msi. |

Nasazení klienta RMS Client pomocí bezobslužné instalace
--------------------------------------------------------

Extrahování souborů pro instalaci Instalační služby systému Windows je nepovinné. Klienta RMS můžete nasadit také pomocí metody bezobslužné instalace. Uvedený krok můžete provést zadáním následujícího příkazu na příkazovém řádku:

`WindowsRightsManagementServicesSP2-KB917275-Client-ENU.exe -override 1 /I MsDrmClient.msi REBOOT=ReallySuppress /q -override 2 /I RmClientBackCompat.msi REBOOT=ReallySuppress /q`

Tento příkaz spustí bezobslužnou instalaci klienta RMS.

| ![](images/Cc747749.note(WS.10).gif)Poznámka                                                                                                                       |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Protože se jedná o bezobslužnou instalaci, nebude vás instalační služba informovat o dokončení instalace. Bezobslužné instalace se obvykle spouštějí v dávkovém souboru nebo v souboru skriptu. |

Nasazení klienta RMS pomocí serveru SMS
---------------------------------------

**Nasazení klienta RMS pomocí serveru SMS**
1.  Otevřete konzolu pro správu serveru SMS.

2.  Rozbalte databázi webu, kterou chcete použít.

3.  V levém podokně klepněte pravým tlačítkem myši na položku **Balíčky**, zvolte příkaz **Nový** a potom klepněte na položku **Balíček z definice**.

4.  Vytvořte balíčky ze souboru MSDRMClient.msi a RMClientBackCompat.msi. Tyto balíčky by měly mít následující vlastnosti:

    **Obecné**:

    -   Na **příkazový řádek** zadejte následující příkaz:
        `msiexec.exe /q ALLUSERS=2 /m MSIDGHOG /i "<file_name>.msi"`
        | ![](images/Cc747749.note(WS.10).gif)Poznámka                                                                                               |
        |-------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
        | MSIDGHOG je náhodná hodnota. Hodnotu &lt;název\_souboru&gt; nahraďte názvem souboru Instalační služby systému Windows, který se bude v rámci tohoto balíčku instalovat. |

    -   U možnosti **Spustit** vyberte položku **Skryté**.
    -   U možnosti **Po spuštění** vyberte položku **Není požadována žádná akce**.
    -   U možnosti **Kategorie** vyberte položku **Software pro správu**.

    **Požadavky:**

    -   U možnosti **Odhadované místo na disku** zadejte hodnotu **445 kB**.
    -   U možnosti **Maximální povolená doba spuštění** vyberte položku **Neznámé**.
    -   Zaškrtněte políčko **Tento program lze spustit na libovolné platformě**.

    **Prostředí:**

    -   U možnosti **Program lze spustit** vyberte položku **Bez ohledu na to, zda jsou přihlášeni uživatelé**.
    -   U možnosti **Režim spuštění** vyberte položku **Spustit s právy pro správu**.
    -   U možnosti **Režim jednotky** vyberte položku **Spustit s názvem UNC**.

    **Upřesnit:**

    -   Zrušte zaškrtnutí políčka **Spustit nejprve jiný program**.
    -   Zrušte zaškrtnutí políčka **Potlačit upozornění programu** v části **Pokud je program přiřazen k počítači**.
    -   Zrušte zaškrtnutí políčka **Zakázat tento program v počítačích, ve kterých je inzerován**.

5.  Nastavte možnost **Přístupové účty a distribuční body** podle požadavků organizace.

6.  Vytvořte inzerování příslušné kolekce. V nasazení SMS doporučujeme používat program **Systém – bez obsluhy**.

7.  Naplánujte tuto inzerci podle potřeb organizace.

Nasazení klienta RMS pomocí zásad skupiny
-----------------------------------------

Klienta RMS můžete do cílových počítačů nainstalovat pomocí funkce zásad skupiny Instalace a údržba softwaru.

Použití zásad skupiny je doporučeným způsobem pro aktivní správu nasazení klientů RMS v malých a středně velkých organizacích, ve kterých se ještě nepoužívá podnikové řešení pro správu aktualizací, jakým je například Systems Management Server 2003.

Pokud pro distribuci programu použijete zásady skupiny, můžete program přiřadit k počítačům. Program je nainstalován, jakmile je počítač spuštěn, a je dostupný všem uživatelům, kteří se k počítači přihlásí. Další informace o zásadách skupiny získáte v tématu Vytvoření návrhu infrastruktury zásad skupiny (<http://go.microsoft.com/fwlink/?linkid=24328>) (stránka může být v angličtině). U tohoto postupu se předpokládá, že používáte konzolu GPMC (Group Policy Management Console). Chcete-li si konzolu GPMC stáhnout, naleznete další informace v části týkající se konzoly GPMC s aktualizací Service Pack 1 (<http://go.microsoft.com/fwlink/?linkid=21813>) (stránka může být v angličtině).

Následující postup je rychlým průvodcem pro správce, kteří nemají příliš velké zkušenosti s distribucí softwaru podle zásad skupin. Tyto kroky můžete podle potřeby upravit tak, aby vyhovovaly potřebám vaší organizace.

**Nasazení klienta RMS pomocí zásad skupiny**
1.  Na řadiči domény otevřete modul snap-in konzoly MMC **Uživatelé a počítače služby Active Directory**.

2.  Vytvořte novou organizační jednotku (OU) nebo vyberte existující organizační jednotku.

    Pokud jste vytvořili novou organizační jednotku, přidejte počítače, do kterých chcete nainstalovat klienta RMS.

3.  Klepněte na organizační jednotku pravým tlačítkem myši a zvolte příkaz **Vlastnosti**.

4.  Vyberte kartu **Zásady skupiny**.

5.  Klepnutím na možnost **Nový** vytvořte nový objekt zásad skupiny.

6.  Klepnutím na možnost **Upravit** můžete nový objekt zásad skupiny upravit.

7.  Ve stromu konzoly rozbalte položky **Konfigurace počítače, Nastavení softwaru** a potom vyberte možnost **Instalace softwaru**.

8.  Pravým tlačítkem myši klepněte do podokna podrobností, klepněte na tlačítko **Nový** a pak na položku **Balíček**.

9.  Zadejte cestu k souboru MSDRMclient.msi v síťové sdílené složce, ke které mají klientské počítače přístup.

10. Klepnutím na tlačítko **OK** balíček přiřaďte.

11. Opakováním kroků 5 až 10 vytvořte objekt zásad skupiny, který nainstaluje soubor RMClientBackCompat.msi.

| ![](images/Cc747749.note(WS.10).gif)Poznámka                                                                                                                                                                                                                                                                                                                                         |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Tyto kroky jsou určeny jen jako vodítko pro uživatele, kteří nemají zkušenosti s používáním zásad skupiny. Správci, kteří s používáním zásad skupiny zkušenosti mají, mohou balíček MSDrmClient.msi distribuovat vlastními postupy. Ještě je potřeba zdůraznit, že tyto kroky jsou určeny pro řadič domény se systémem Windows Server 2003 — proces a terminologie se může lišit pro doménu systému Windows 2000. |

Upgrade z předchozí verze
-------------------------

        ```
| ![](images/Cc747749.note(WS.10).gif)Poznámka                                    |
|--------------------------------------------------------------------------------------------------------------|
| Tento skript není funkční se systémem Windows Vista, protože klient RMS je integrován do operačního systému. |
