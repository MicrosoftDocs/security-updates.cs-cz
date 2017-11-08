---
TOCTitle: Problémy se správou služby RMS
Title: Problémy se správou služby RMS
ms:assetid: '97013c08-d3fa-4ea0-8914-995b6c97f900'
ms:contentKeyID: 18113374
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747605(v=WS.10)'
---

Problémy se správou služby RMS
==============================

Po úspěšném zajištění služby RMS na serveru může při každodenní správě této služby docházet k problémům. Odstranění některých problémů vám usnadní informace v následujících částech.

Při otevření webu pro správu služby RMS se zobrazí zpráva SQL Server neexistuje nebo byl odepřen přístup.
---------------------------------------------------------------------------------------------------------

Pokud jste službu RMS nainstalovali pomocí nové instalace serveru SQL Server 2005 jako databázového serveru, nebude služba serveru SQL pravděpodobně spuštěna. Služba MSSQLSERVER na serveru SQL Server 2005 pravděpodobně není nakonfigurována na automatické spuštění po spuštění daného serveru. Jestliže jste SQL Server po instalaci služby RMS restartovali a nenakonfigurovali jste uvedenou službu na automatické restartování služby RMS, nebude služba RMS fungovat a k dispozici bude pouze stránka Globální správa.

Po spuštění služby MSSQLSERVER je nutné obnovit funkčnost služby RMS restartováním Internetové informační služby na serveru RMS.

Nelze dokončit zápis offline.
-----------------------------

Pokud není soubor požadavku na zápis před odesláním na web služby Enrollment Services úplný nebo pokud dojde k jeho změně, nelze zápis offline dokončit. Soubor požadavku na zápis mohl být poškozen nebezpečným programem, chybou uživatele nebo systémovou chybou.

V závislosti na chybějících informacích může web služby Enrollment Services i přesto soubor přijmout a vrátit certifikát serveru pro poskytování licencí nebo může soubor požadavku odmítnout a zobrazit chybu.

Jestliže je vrácen certifikát serveru pro poskytování licencí, bude upraven na základě chybějících informací nebo chyby v souboru požadavku na zápis a při importu tohoto certifikátu zobrazí služba RMS chybu.

Jestliže proces zápisu nelze dokončit, zkontrolujte, zda počítač s připojením k Internetu není napaden viry, znovu exportujte soubor požadavku na zápis ze serveru RMS a pak jej přeneste do počítače s připojením k Internetu pomocí jiného média. Pokud opět dojde k chybě, obraťte se na oddělení podpory produktů společnosti Microsoft.

Nevytvářejí se soubory protokolu.
---------------------------------

Protokolování služby RMS vyžaduje službu Řízení front zpráv (také známou pod zkratkou MSMQ) i přístup k databázi protokolování. Jestliže k vytvoření souborů protokolu nedošlo, může to znamenat, že součásti nebyly správně nakonfigurovány nebo že byla mezi nimi přerušena komunikace.

Proveďte test síťového propojení serveru RMS a databázového serveru. Pokud je připojení funkční, zkontrolujte pomocí následujícího postupu předpoklady protokolování služby RMS a ověřte, zda jsou správně nakonfigurovány všechny závislosti softwaru.

Nejprve zkontrolujte, zda je správná konfigurace služby Řízení front zpráv. Služba Řízení front zpráv musí být nainstalována s povolenou integrací služby Active Directory.

**Ověření správné instalace a konfigurace služby Řízení front zpráv**
1.  V **Ovládacích panelech** klepněte na položku **Přidat nebo odebrat programy** a pak klepnutím na tlačítko **Přidat nebo odebrat součásti systému** otevřete **Průvodce součástmi systému Windows**.

2.  V **Průvodci součástmi systému Windows** zaškrtněte políčko **Aplikační server** a pak klepněte na tlačítko **Podrobnosti**.

3.  Zaškrtněte políčko **Řízení front zpráv** a pak klepněte na tlačítko **Podrobnosti**.

4.  Pokud je zaškrtnuto políčko **Integrace se službou Active Directory**, přejděte k dalšímu testu a ověřte, zda je služba Řízení front zpráv spuštěna. Jestliže toto zaškrtávací políčko zaškrtnuto není, pokračujte provedením kroků 5 až 9.

5.  Klepněte na tlačítko **Start**, přejděte na příkaz **Všechny programy**, přejděte na položku **Služba Windows RMS** a pak klepnutím na odkaz **Správa služby RMS v systému Windows** otevřete stránku Globální správa.

6.  Klepněte na položku **Odebrat službu RMS z tohoto webu** u webu, na kterém je zajištěna služba RMS, a pak klepněte na tlačítko **OK**.

7.  V okně **Přidat nebo odebrat programy**, do kterého jste přešli z **Ovládacích panelů**, klepněte na položku **Přidat nebo odebrat součásti systému**, klepněte na možnost **Aplikační server** a pak klepněte na položku **Řízení front zpráv**.

8.  Chcete-li povolit **integraci se službou Active Directory**, klepněte na tlačítko **Podrobnosti**, zaškrtněte políčko **Integrace se službou Active Directory** a pak klepněte na tlačítko **OK**.

9.  Otevřete stránku **Globální správa.** Klepněte na položku **Zajišťovat službu RMS na tomto webu** u názvu webu, pro který chcete službu RMS zajistit.

Dále ověřte, zda je služba Řízení front zpráv spuštěna na příslušném serveru.

**Ověření spuštění služby Řízení front zpráv na serveru**
1.  V **Ovládacích panelech** klepněte na položku **Nástroje pro správu** a pak klepněte na položku **Služby**.

2.  Procházejte seznam služeb, dokud nenaleznete službu **Řízení front zpráv**.

3.  Ve sloupci **Stav** by se u této služby měla zobrazit hodnota **Spuštěno**. Pokud tomu tak není, klepněte pravým tlačítkem myši na službu a pak klepněte na příkaz **Spustit**.

Potom ověřte, zda má služba protokolování oprávnění k zápisu událostí do databáze protokolování. Protokolování služby RMS se spouští pomocí účtu služby RMS. Ověřte, zda má účet služby RMS platné přihlašovací údaje k databázovému serveru a zda mu byla udělena potřebná oprávnění pro vytváření databází a zápis informací do souborů.

Po splnění všech uvedených předpokladů ukončete a restartujte službu protokolování služby RMS prostřednictvím modulu snap-in Služby. Po restartování protokolování služby RMS by měly být na databázovém serveru vytvořeny soubory protokolu. Používáte-li jako databázový server produkt SQL Server, můžete pomocí následujících kroků ověřit, zda se soubory protokolu vytvářejí.

**Ověření vytváření souborů protokolu na serveru SQL Server**
1.  Ve správci SQL Server Enterprise Manager přejděte k databázi protokolování, rozbalte položku **Databases** (Databáze) a poté rozbalte databázi obsahující databázi protokolování služby RMS.

2.  Klepněte na databázi protokolování, vyberte položku **Tables** (Tabulky), pravým tlačítkem myši klepněte na položku **DRMS\_log\_master** a poté klepněte na možnost **Open table – return all rows** (Otevřít tabulku – vrátit všechny řádky). Pokud jsou vytvářeny soubory protokolů, zobrazí se jeden nebo více těchto souborů.

Obnovení konfigurační databáze
------------------------------

Služba RMS nemůže pracovat bez funkční konfigurační databáze. Pokud došlo k potížím s konfigurační databází, jako je například poškození databáze nebo selhání pevného disku u databázového serveru, můžete funkčnost služby RMS obnovit pomocí zálohy konfigurační databáze. Chcete-li obnovit konfigurační databázi služby RMS ze zálohy, budete potřebovat následující informace:

-   název nejaktuálnější zálohy databáze;
-   název počítače, ve kterém bude záložní databáze obnovena;
-   název účtu a heslo, které byly původně použity k zajištění služby RMS;
-   heslo, které bylo původně zadáno pro softwarovou ochranu soukromého klíče (pokud byla nastavena).

Obnovení záložní databáze nevyžaduje nový certifikát serveru pro poskytování licencí ani nový soukromý klíč, protože ve službě RMS zůstala zachována všechna nastavení (načítají se ze záložní konfigurační databáze).

Záložní databázi můžete obnovit pomocí následujícího postupu.

**Obnovení záložní databáze**
1.  Klepněte na tlačítko **Start**, přejděte na položku **Všechny programy**, přejděte na položku **Služba Windows RMS** a pak klepnutím na odkaz **Správa služby RMS v systému Windows** otevřete stránku **Globální správa**.

2.  Klepněte na položku **Odebrat službu RMS z tohoto webu** u webu, na kterém je zajištěna služba RMS, a pak klepněte na tlačítko **OK**.

3.  Obnovte soubory záložní databáze pro konfigurační databázi. Pokud jste během procesu zálohování zálohovali také databázi protokolování a chcete zachovat kontinuitu dat, obnovte zároveň databázi protokolování.

    -   Jestliže tento systém obnovujete po úplném selhání, obnovte před soubory záložní databáze také registr, a to pomocí zálohy stavu systému.

4.  Je-li obnovovaná databáze určena pro jeden server kořenové certifikace, upravte před novým zajištěním služby následující klíč registru:

    -   Počítače s 32bitovou verzí systému Windows Server 2003
        `HKEY_LOCAL_MACHINE\Software\Microsoft\DRMS\1.0\`
    -   Počítače s 64bitovou verzí systému Windows Server 2003
        `HKEY_LOCAL_MACHINE\Software\WOW6432Node\Microsoft\DRMS\1.0\`

    Přidejte následující položku jako hodnotu řetězce a ponechte danou hodnotu prázdnou:

    `GicURL`

    Uvedeným krokem bude potlačeno rozpoznání služby Active Directory serveru kořenové certifikace a bude možné získat přístup ke stránkám zajištění serveru kořenové certifikace.

5.  Pokud jste zabezpečili soukromý klíč služby RMS pomocí hardwarového modulu zabezpečení, obnovte zálohované prostředí zabezpečení, aby bylo možné načíst klíče.

6.  Proveďte jeden z následujících kroků:

    -   Chcete-li obnovit databázi u jediného serveru (nikoli pro celý cluster), klepněte u webu, na němž chcete službu RMS zajistit, na možnost Zajišťovat službu RMS na tomto webu.
        -nebo-
    -   Chcete-li obnovit databázi pro celý cluster, klepněte u webu, na němž chcete službu RMS zajistit, na možnost Přidat tento server do clusteru.

7.  Zadejte účet služby RMS, který byl původně použit k zajištění serveru.

8.  Zadejte požadovanou záložní konfigurační databázi (včetně názvu databáze a názvu počítače, v němž je databáze uložena).

9.  Zadejte heslo, které jste použili při původním zajištění daného serveru.

10. Klepněte na tlačítko **Odeslat**.

Spustí se proces zajištění a služba RMS bude na serveru znovu zajištěna.

Další informace najdete v této sadě dokumentace v části Plánování obnovení systému a Zálohování a obnovení systému služby RMS tématu Plánování nasazení služby RMS.

Konec platnosti hesla účtu služby RMS
-------------------------------------

Pokud služba RMS přestane pracovat, může být důvodem konec platnosti hesla účtu služby RMS. Otevřete okno Správce Internetové informační služby. Jestliže jsou zastaveny fondy aplikací služby RMS a nelze je restartovat, došlo pravděpodobně k ukončení platnosti hesla účtu služby RMS.

Pokud vyprší platnost hesla účtu služby RMS, je třeba změnit heslo u všech serverů RMS používajících již neplatné heslo a pak restartovat Internetovou informační službu. Další informace najdete v této sadě dokumentace v části Změna hesla účtu služby RMS tématu Provoz serveru RMS.

Obnovení předchozí instalace služby RMS
---------------------------------------

Jestliže dojde k selhání hardwaru nebo softwaru serveru RMS, můžete tento server obnovit pomocí již nainstalované konfigurační databáze a zajistit tak novou instanci serveru.

| ![](images/Cc747605.note(WS.10).gif)Poznámka                                                                                                                                                                                                                                                                                                    |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Tento postup platí pouze v případě selhání serveru, na kterém je spuštěna služba RMS. Pokud dojde k selhání serveru, na kterém je spuštěna konfigurační databáze, najdete potřebné informace v tomto tématu v části Obnovení konfigurační databáze uvedené již dříve. Jestliže je server RMS současně databázovým serverem, bude nutné obnovit celý server ze záložní kopie. |

Pomocí následujícího postupu přejděte ke stejné konfigurační databázi, která byla použita pro původní instalaci.

**Obnovení předchozí instalace služby RMS**
1.  Prostřednictvím účtu s oprávněními správce se přihlaste k počítači, který chcete konfigurovat jako server RMS. Tento počítač musí splňovat minimální požadavky na systém pro službu RMS. Další informace o požadavcích na systém pro službu RMS najdete v této sadě dokumentace v části Hardwarové požadavky tématu Plánování nasazení služby RMS.

2.  Pokud k ochraně soukromých klíčů služby RMS používáte hardwarový modul zabezpečení, zkontrolujte, zda je správně nakonfigurován pomocí stejného nastavení a zabezpečení, jaké bylo použito u předchozí instalace služby RMS.

3.  Nainstalujte službu RMS do počítače.

4.  Po dokončení instalace služby RMS klepněte na tlačítko **Start**, přejděte na příkaz **Všechny programy**, přejděte na položku **Služba Windows RMS** a pak klepnutím na položku **Správa služby RMS v systému Windows** otevřete stránku **Globální správa**.

5.  Klepněte na položku **Přidat tento server do clusteru** u webu, pro který chcete zajistit službu RMS.

6.  V části **Účet služby RMS** zadejte název účtu služby RMS ve tvaru název\_domény\\uživatelské\_jméno a heslo účtu služby RMS, pod kterým bude služba RMS zpravidla pracovat za běžného provozu. Musí se jednat o doménový účet.

7.  V části **Konfigurační databáze** zadejte název databázového serveru a název konfigurační databáze pro původní instalaci služby RMS, kterou chcete obnovit.

8.  V části **Ochrana soukromého klíče** vyberte způsob ochrany soukromého klíče v tomto clusteru. Jestliže jste nastavili softwarovou ochranu soukromého klíče, je nutné zadat heslo, které bylo použito k zašifrování soukromého klíče při původním zajištění tohoto clusteru.

9.  Klepněte na tlačítko **Odeslat**.

Klienti nemohou otevřít obsah chráněný službou RMS z důvodu ukončené platnosti oprávnění
----------------------------------------------------------------------------------------

V případě, že vypršela platnost oprávnění uživatele, nemůže tento uživatel využívat obsah chráněný službou RMS. Pokud systémové hodiny na serveru RMS předcházejí systémové hodiny v klientovi RMS, nebude uživatel pravděpodobně moci využívat obsah chráněný službou RMS ani v případě, že platnost oprávnění dosud nevypršela. Vzhledem k tomu, že systémové hodiny nejsou v těchto dvou počítačích synchronizovány, může se při otevření obsahu v klientovi zobrazit následující chybová zpráva:

**Nemáte oprávnění k otevření této zprávy, protože jeho platnost skončila. Chcete zprávu otevřít pomocí jiné sady pověření?**

Licence klienta i licence obsahu jsou platné, ale v důsledku časového rozdílu klient považuje licenci obsahu za neplatnou a vrátí uživateli tuto chybu. Z tohoto důvodu se může uživatel domnívat, že došlo k problému s certifikátem účtu služby RMS nebo s právy udělenými pro daný dokument. Jakmile hodiny v klientovi přejdou do časového rozsahu platnosti licence k publikování obsahu, bude uživatel moci obsah otevřít.

Doporučeným postupem je synchronizovat klienty i servery v systému služby RMS na stejnou časovou službu.

Chyba Přístup byl odepřen, pokud se služba RMS pokusí zaprotokolovat události do protokolu událostí aplikací
------------------------------------------------------------------------------------------------------------

Ve výchozím nastavení jsou součásti (například služba RMS), které jsou spouštěny ze stránky ASP, vytvářeny pod účtem IUSR\_COMPUTERNAME. Tento účet je členem skupiny Guests a oprávnění zabezpečení požadovaná pro zápis do protokolu událostí aplikací znemožňují účtům skupiny Guests zápis do protokolu událostí.

Chcete-li tyto potíže odstranit, můžete pomocí editoru registru upravit klíč registru řídící toto chování.

| ![](images/Cc747605.Caution(WS.10).gif)Upozornění                                                                                                  |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Nesprávné úpravy registru mohou způsobit závažné poškození systému. Před provedením jakýchkoli změn registru byste měli vytvořit záložní kopii všech důležitých dat v počítači. |

Nastavte následující klíč registru z hodnoty 1 na hodnotu 0 a pak restartuje počítač, aby se změny projevily.

`HKEY_LOCAL_MACHINE\System\CurrentControlSet\Services\EventLog\Application`

Název: `RestrictGuestAccess`

Typ: `REG_DWORD`

| ![](images/Cc747605.note(WS.10).gif)Poznámka                  |
|--------------------------------------------------------------------------------------------|
| Uvedeným postupem umožníte všem účtům skupiny Guests zápis do protokolu událostí aplikací. |

Další informace o příčině této chyby najdete v článku týkajícím se povolení protokolování ze stránek ASP ve znalostní bázi [Microsoft Knowledge Base](http://go.microsoft.com/fwlink/?linkid=44167).
