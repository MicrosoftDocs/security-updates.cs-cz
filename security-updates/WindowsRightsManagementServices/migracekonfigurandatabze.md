---
TOCTitle: Migrace konfigurační databáze
Title: Migrace konfigurační databáze
ms:assetid: '980e3e94-7d28-40dd-ad01-d34eb3c8d8e6'
ms:contentKeyID: 18113377
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747607(v=WS.10)'
---

Migrace konfigurační databáze
=============================

V některých případech je potřeba databázový server vyřadit z provozu. Jedním z nich je například upgrade hardwaru databázového serveru služby RMS. Před vyřazením databázového serveru z provozu je nutné přesunout konfigurační databázi na jiný databázový server. Za účelem ochrany dat v konfigurační databázi, včetně párů klíčů, které obsahuje, je potřeba migraci plánovat a implementovat velice pečlivě.

Doporučujeme pro databázový server RMS vytvořit alias CNAME a nakonfigurovat službu RMS na používání tohoto aliasu. Není tak potřeba ručně měnit název databázového serveru v konfigurační databázi služby RMS, pokud se změní název serveru. Při používání aliasu CNAME by stačilo aktualizovat záznam aliasu.

Před zahájením migrace konfigurační databáze je potřeba zajistit, abyste měli následující informace:

-   název a heslo účtu, který byl původně použit k zajištění serverů v clusteru služby RMS používajícím tuto databázi;
-   heslo privátního klíče služby RMS, které bylo původně zadáno během zajišťování (pokud se používá softwarový zprostředkovatel kryptografických služeb pro ukládání privátního klíče služby RMS); jestliže se k uložení hesla privátního klíče služby RMS používá hardwarový modul zabezpečení, není tento krok nutný.

| ![](images/Cc747607.note(WS.10).gif)Poznámka                                                                                                                             |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Při migraci konfigurační databáze není nutný nový certifikátu serveru pro poskytování licencí nebo nový privátní klíč serveru, protože služba RMS uchovává nastavení z původní konfigurační databáze. |

Před prováděním jakýchkoli operací na databázovém serveru byste měli zazálohovat databáze služby RMS. Pokud to není možné, vyexportujte aspoň certifikát serveru pro poskytování licencí. Další informace o exportu certifikátu serveru pro poskytování licencí naleznete v tématu týkajícím se [Export certifikátu serveru pro poskytování licencí do souboru](https://technet.microsoft.com/d683a629-71b3-4b11-932b-4ab0317334af). Jestliže při migraci databází dojde k chybě, můžete certifikát serveru pro poskytování licencí naimportovat do nové instalace služby RMS a použít obsah, který byl chráněn právy, se starší instalací.

Konfigurační databázi můžete migrovat provedením následujících kroků:

-   Aktualizujte konfigurační databázi služby RMS tak, aby obsahovala nový název databázového serveru.
-   Aktualizujte soubory web.config a registr každého serveru v clusteru RMS tak, aby používaly nový název databázového serveru.

| ![](images/Cc747607.Important(WS.10).gif)Důležité informace                                                   |
|--------------------------------------------------------------------------------------------------------------------------------------------|
| V tomto tématu se předpokládá, že databáze RMS již byly zkopírovány na nový databázový server, na kterém jsou uloženy databáze služby RMS. |

Aktualizace konfigurační databáze služby RMS tak, aby používala nový název databázového serveru
-----------------------------------------------------------------------------------------------

Název databázového serveru, na kterém se ukládají databáze služby RMS, je uložen v konfigurační databázi služby RMS. Po migraci databázových souborů na nový databázový server je nutné aktualizovat konfigurační databázi služby RMS. To lze provést pomocí nástroje RMS Config Editor ze sady nástrojů RMS Administration Toolkit nebo pomocí nástroje SQL Management Studio.

Chcete-li aktualizovat název databázového serveru služby RMS pomocí nástroje RMS Config Editor, postupujte takto:

**Aktualizace konfigurační databáze služby RMS pomocí nástroje RMS Config Editor**
1.  Přihlaste se k serveru RMS v clusteru jako člen databázové role System Administrators.

2.  Nainstalujte sadu RMS Administration Toolkit z webu Stažení softwaru ([http://go.microsoft.com/fwlink/?LinkId=98961](http://go.microsoft.com/fwlink/?linkid=98961)).

3.  Přejděte do umístění %SystemDrive%:\\Program Files\\RMS SP2 Administration Toolkit\\RMSConfigEditor a poklepejte na soubor **RMSCONFIGEDITOR.EXE**.

4.  Do pole **Server** zadejte název nového serveru, na kterém je uložena konfigurační databáze služby RMS, a potom klepněte na možnost **Go** (Přejít).

5.  V seznamu **Database** (Databáze) klepněte na možnost **DRMS\_Config\_***&lt;název clusteru služby RMS&gt;***\_***&lt;Port&gt;*, kde *&lt;název clusteru služby RMS&gt;* je název clusteru služby RMS a *&lt;Port&gt;* je port TCP, na kterém služba RMS komunikuje. Potom klepněte na možnost **Go** (Přejít).

6.  Klepněte na možnost **DRMS\_ClusterPolicies**.

7.  V podokně výsledků změňte hodnotu ve sloupci **PolicyData** řádku **LoggingDatabaseServer** na nový název databázového serveru služby RMS.

8.  Klepněte na možnost **Persist** (Trvalé).

9.  Změňte hodnotu ve sloupci **PolicyData** řádku **CertificationUserKeyStorageConnectionString** na nový databázový server. Hodnota by měla být **data source=***&lt;nový název databázového serveru&gt;***;integrated**, kde *&lt;nový název databázového serveru&gt;* je název nového databázového serveru.

10. Klepněte na možnost **Persist** (Trvalé).

11. Opakujte kroky 9 až 10 pro hodnotu ve sloupci **PolicyData** řádku **DirectoryServicesCacheDatabase**.

12. V levém podokně klepněte na možnost **DRMS\_PluginProperties**.

13. Pro **PropertyID** 101 s názvem **PERSISTENT\_STORAGE** změňte ve sloupci **PropertyValue** hodnotu na nový název databázového serveru. Hodnota by měla být **data source=***&lt;nový název databázového serveru&gt;***;integrated**, kde *&lt;nový název databázového serveru&gt;* je název nového databázového serveru.

14. Klepněte na možnost **Persist** (Trvalé).

15. Ukončete nástroj RMS Config Editor.

Chcete-li aktualizovat konfigurační databázi služby SQL pomocí nástroje SQL Server Management Studio, postupujte takto:

**Aktualizace konfigurační databáze služby SQL pomocí nástroje SQL Server Management Studio**
1.  Přihlaste se k serveru konfiguračních databází služby RMS jako místní správce (Administrator) nebo pomocí jiného uživatelského účtu, který je členem místní skupiny Administrators.

2.  Klepněte na tlačítko **Start**, přejděte na příkaz **Všechny programy**, přejděte na příkaz **Microsoft SQL Server 2005** a potom klepněte na příkaz **SQL Server Management Studio**.

3.  Na stránce **Connect to Server** (Připojit k serveru) zajistěte, aby byl nový název databázového serveru uveden v poli **Server name** (Název serveru), a potom klepněte na tlačítko **Connect** (Připojit).

4.  Rozbalte položku **Databases** (Databáze), rozbalte položku **DRMS\_Config\_***&lt;název\_clusteru\_RMS&gt;***\_***&lt;Port&gt;* a potom rozbalte položku **Tables** (Tabulky).

5.  Klepněte pravým tlačítkem na možnost **DRMS\_ClusterPolicies** a potom klepněte na příkaz **Open Table** (Otevřít tabulku).

6.  V podokně výsledků změňte hodnotu ve sloupci **PolicyData** řádku **LoggingDatabaseServer** na nový název databázového serveru služby RMS.

7.  Změňte hodnotu ve sloupci **PolicyData** řádku **CertificationUserKeyStorageConnectionString** na nový databázový server. Hodnota by měla být **data source=***&lt;nový název databázového serveru&gt;***;integrated**, kde *&lt;nový název databázového serveru&gt;* je název nového databázového serveru.

8.  Opakujte kroky 6 až 7 pro hodnotu ve sloupci **PolicyData** řádku **DirectoryServicesCacheDatabase**.

9.  V podokně Object Explorer (Průzkumník objektů) klepněte pravým tlačítkem myši na možnost **DRMS\_PluginProperties** a potom klepněte na možnost **Open Table** (Otevřít tabulku).

10. Pro **PropertyID** 101 s názvem **PERSISTENT\_STORAGE** změňte ve sloupci **PropertyValue** hodnotu na nový název databázového serveru. Hodnota by měla být **data source=***&lt;nový název databázového serveru&gt;***;integrated**, kde *&lt;nový název databázového serveru&gt;* je název nového databázového serveru.

11. Ukončete nástroj Microsoft SQL Server Management Studio.

Konfigurace každého serveru v clusteru služby RMS na používání nového názvu databázového serveru
------------------------------------------------------------------------------------------------

Chcete-li nakonfigurovat každý server v clusteru služby RMS na používání nového názvu databázového serveru, je nutné aktualizovat soubory web.config a aktualizovat tři položky registru. Po dokončení je nutné restartovat Internetovou informační službu, aby se změny projevily.

Aktualizace souborů web.config na každém serveru v clusteru služby RMS:

**Aktualizace souborů web.config na každém serveru v clusteru služby RMS**
1.  Přihlaste se k serveru v clusteru služby RMS jako člen místní skupiny Administrators.

2.  Přejděte do umístění %Systemdrive%\\inetpub\\wwwroot\\\_wmcs\\admin.

3.  Poklepejte na soubor **web.config**, vyberte možnost **Vybrat program ze seznamu** a klepněte na tlačítko **OK**.

4.  Klepněte na možnost **Poznámkový blok**, zaškrtněte políčko **K otevření souborů tohoto typu vždy použít vybraný program** a potom klepněte na tlačítko **OK**.

5.  Klepněte v nabídce **Úpravy** na příkaz **Nahradit**.

6.  Do pole **Najít** zadejte název databázového serveru, na kterém jsou uloženy databáze služby RMS a který chcete vyřadit z provozu.

7.  Do pole **Nahradit** zadejte název nového databázového serveru, na kterém jsou uloženy databáze služby RMS.

8.  Klepněte na tlačítko **Nahradit vše** a potom klepněte na tlačítko **Storno**.

9.  Klepněte na nabídku **Soubor** a potom na příkaz **Uložit**.

10. Ukončete program Poznámkový blok.

11. Opakujte kroky 2 až 9 pro soubory web.config v adresářích %Systemdrive%\\inetpub\\wwwroot\\\_wmcs\\certification a %Systemdrive%\\inetpub\\wwwroot\\\_wmcs\\licensing.

12. Opakujte kroky 1 až 11 pro každý server v clusteru služby RMS.

Nakonec aktualizujte registr na každém serveru v clusteru služby RMS tak, aby používal nový název databázového serveru.

| ![](images/Cc747607.Caution(WS.10).gif)Upozornění                                                          |
|-----------------------------------------------------------------------------------------------------------------------------------------|
| Nesprávná úprava registru může vážně poškodit systém. Před prováděním změn registru byste měli v počítači zálohovat veškerá cenná data. |

**Aktualizace registru na každém serveru v clusteru služby RMS**
1.  Přihlaste se k serveru v clusteru služby RMS jako člen místní skupiny Administrators.

2.  Klepněte na tlačítko **Start** a pak na příkaz **Spustit**.

3.  Zadejte příkaz **regedit.exe** a klepněte na tlačítko **OK**.

4.  Přejděte do umístění **HKEY\_LOCAL\_MACHINE\\Software\\Microsoft\\DRMS\\1.0\\KeyProtection**.

5.  Změňte položku registru s názvem PASSWORDDERIVEDKEY\_*&lt;původní název databázového serveru&gt;*\_DRMS\_CONFIG\_*&lt;název clusteru RMS&gt;*\_*&lt;port&gt;* na:

    PASSWORDDERIVEDKEY\_*&lt;původní název databázového serveru&gt;*\_DRMS\_CONFIG\_*&lt;název clusteru RMS&gt;*\_*&lt;port&gt;*

    kde jednotlivé položky mají tento význam:

    -   *&lt;původní název databázového serveru&gt;* je název původního databázového serveru.
    -   *&lt;název clusteru RMS&gt;* je název clusteru služby RMS.
    -   *&lt;port&gt;* je port TCP, na kterém služba RMS komunikuje.
    -   *&lt;nový název databázového serveru&gt;* je název nového databázového serveru.

6.  Přejděte do umístění **HKEY\_LOCAL\_MACHINE\\System\\CurrentControlSet001\\Services\\DRMS\_Logging\_&lt;název clusteru RMS&gt;\_&lt;port&gt;\\Params**.

7.  Změňte položku registru **ConnectionString** tak, aby hodnota zdroje dat odpovídala novému názvu databázového serveru.

8.  Opakujte kroky 6 až 7 pro položku **HKEY\_LOCAL\_MACHINE\\System\\CurrentControlSet\\Services\\DRMS\_Logging\_&lt;název clusteru RMS&gt;\_&lt;port&gt;\\Params**.

9.  Do příkazového řádku zadejte příkaz **IISRESET** a stiskněte klávesu ENTER.

10. Opakujte kroky 1 až 9 pro každý server v clusteru služby RMS.
