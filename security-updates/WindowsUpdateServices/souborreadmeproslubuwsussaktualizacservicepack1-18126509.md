---
TOCTitle: Soubor Readme pro službu WSUS s aktualizací Service Pack 1
Title: Soubor Readme pro službu WSUS s aktualizací Service Pack 1
ms:assetid: '937ecfe9-e8e0-41ac-85f7-4b65956f3d1e'
ms:contentKeyID: 18126509
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc708486(v=WS.10)'
---

Soubor Readme pro službu WSUS s aktualizací Service Pack 1
==========================================================

Tento dokument popisuje známé problémy ovlivňující službu Windows Server Update Services (WSUS) s aktualizací Service Pack 1. Bezprostředně za informacemi o službě WSUS s aktualizací SP1 následují veškeré informace, které byly dříve součástí původních poznámek v souboru Readme služby WSUS. Patří sem doporučení a požadavky na instalaci služby WSUS. Chcete-li službu WSUS s aktualizací SP1 stáhnout, přejděte na [web Stažení softwaru](http://go.microsoft.com/fwlink/?linkid=67516).

Nové funkce služby WSUS s aktualizací SP1
-----------------------------------------

WSUS SP1 je aktualizace Service Pack vylepšující zabezpečení, spolehlivost, škálovatelnost, kompatibilitu a výkon služby WSUS. Nové funkce a vylepšení jsou následující:

-   Podpora klientů se systémem Windows Vista: Pomocí služby WSUS s aktualizací SP1 lze aktualizovat počítače se systémem Windows Vista.
-   Podpora více jazyků u klientů: Podpora všech jazyků sady Office a systému Windows Vista.
-   Nová verze součásti WMSDE: Instance součásti WMSDE bude službou WSUS s aktualizací SP1 upgradována na WMSDE SP4 (služba WSUS RTM používá součást WMSDE SP3).
-   Vylepšení výkonu: Služba WSUS s aktualizací SP1 obsahuje různá vylepšení výkonu urychlující dobu odezvy uživatelského rozhraní.
-   Všechny opravy hotfix: Služba WSUS s aktualizací SP1 zahrnuje všechny změny a opravy hotfix vydané od verze WSUS RTM.
-   Podpora serveru SQL Server 2005.

Před zahájením upgradu na službu WSUS s aktualizací SP1
-------------------------------------------------------

S upgradem na službu WSUS s aktualizací SP1 jsou spojeny následující problémy. Problémy a požadavky uvedené v části Před zahájením původní verze tohoto tématu nejsou v tomto článku vyřešeny a jsou stále platné. Například stále platí požadavky na instalaci uvedené v původní části Před zahájením.

**Poznámka:**   Po instalaci aktualizace SP1 pro službu WSUS 2.0 není možné tuto aktualizaci Service Pack odinstalovat. Odinstalací aktualizace SP1 odinstalujete celý produkt.

**Důležité:**   Tento dokument obsahuje informace o změně registru. Před změnou nezapomeňte registr zálohovat. Přesvědčte, zda víte, jak registr obnovit v případě, že nastanou potíže. Další informace o zálohování, obnovení a změně registru uvádí následující článek znalostní báze Microsoft Knowledge Base:

[Popis registru systému Microsoft Windows](http://support.microsoft.com/kb/256986) (http://support.microsoft.com/kb/256986/)

#### Problém 1: Ujistěte se, že máte dostatek místa pro zálohování databáze.

Při upgradu z verze WSUS RTM instalační program služby WSUS s aktualizací SP1 vytvoří automaticky zálohu databáze WSUS. Zajistěte, aby byl v souborovém systému serveru WSUS dostatek diskového prostoru pro uložení zálohy databáze služby WSUS, jinak se instalace služby WSUS s aktualizací SP1 nezdaří.

**Určení dostatečné velikosti diskového prostoru**
1.  Otevřete program Průzkumník Windows a přejděte do složky, v níž je umístěna databáze služby WSUS. Ve výchozím nastavení služba WSUS instaluje databázi sem:
    
        ```
		<DriveLetter>:\WSUS\MSSQL$WSUS\Data\
		```
		
2.  Stiskněte a podržte klávesu **CTRL**, vyberte soubory **SUSDB.MDF** a **SUSDB\_log.LDF**, klepněte na ně pravým tlačítkem myši a zvolte příkaz **Vlastnosti**.

3.  V dialogovém okně **Soubory** se podívejte na hodnotu v poli **Velikost na disku**. Na disku musí být nejméně takové množství volného místa pro instalaci služby WSUS s aktualizací SP1.

4.  V nabídce **Start** klepněte na položku **Tento počítač**. Ověřte, zda disk, na kterém je nainstalována služba WSUS, obsahuje požadované množství volného prostoru.

Pokud se instalace služby WSUS s aktualizací SP1 z nějakého důvodu nezdaří, obnovte záložní databázi ručně. Pokyny k obnovení databáze služby WSUS získáte v [Provozní příručce služby WSUS](http://technet2.microsoft.com/windowsserver/en/library/05f2e884-ae62-4c90-9681-6c9f2f3c9fd91033.mspx).

#### Problém 2: Služba WSUS s aktualizací SP1 upgraduje pouze verzi WSUS RTM

Službu WSUS s aktualizací SP1 lze použít pouze pro upgrade verze WSUS RTM. V současné době není k dispozici podpora pro upgrade z verze Release Candidate služby WSUS. Používáte-li verzi Release Candidate služby WSUS nebo jakékoli starší sestavení služby WSUS, je třeba tato sestavení odinstalovat a teprve potom spustit instalaci služby WSUS s aktualizací SP1.

#### Problém 3: Během upgradu na službu WSUS s aktualizací SP1 bude zastavena služba IIS na serveru.

Instalační program služby WSUS s aktualizací SP1 zastaví během upgradu Internetovou instalační službu (IIS) na serveru. To znamená, že všechny weby na serveru, které služba IIS hostuje, budou po dobu trvání upgradu nedostupné. Služba IIS se po skončení upgradu automaticky spustí.

#### Problém 4: Během upgradu byste neměli spouštět aplikace, které volají rozhraní API služby WSUS.

Volání rozhraní API služby WSUS se dostane do konfliktu s instalačním programem služby WSUS s aktualizací SP1, což způsobí selhání upgradu (zobrazí se chybová zpráva s výzvou k restartování serveru, aby bylo možné upgrade dokončit).

#### Problém 5: Při upgradu na službu WSUS s aktualizací SP1 může být nutné zakázat antivirové programy.

Při upgradu služby WSUS instalací aktualizace WSUS SP1 může být nutné zakázat antivirové programy. Teprve potom bude možné úspěšně provést upgrade nebo nainstalovat aktualizaci Service Pack. Po zakázání antivirových programů restartujte počítač se systémem Windows Server. Pak nainstalujte upgrade nebo aktualizaci Service Pack. Tímto procesem zabráníte uzamknutí souborů, s nimiž musí proces aktualizace pracovat. Po dokončení instalace znovu povolte antivirový program. Na webu dodavatele antivirového programu jsou uvedeny přesné kroky pro zakázání a opětovné povolení antivirového programu a verze.

> [!CAUTION]
> Toto zástupné řešení může způsobit, že počítač nebo síť budou zranitelnější vůči útokům uživatelů se zlými úmysly nebo škodlivého softwaru, jako jsou viry. Toto zástupné řešení nedoporučujeme, ale uvádíme tuto informaci pro případ, že byste je chtěli použít. Toto zástupné řešení používáte na vlastní riziko.

> [!NOTE]
> Antivirový program chrání počítač před viry. V době, kdy je antivirový program zakázán, nesmíte stahovat ani otevírat soubory z nedůvěryhodných zdrojů, navštěvovat nedůvěryhodné weby ani otevírat přílohy e-mailů. 

#### Problém 6: Při použití proxy serveru může upgrade na aktualizaci SP1 smazat uživatelské jméno a heslo pro konfiguraci proxy serveru

Pokud používáte proxy server, může upgrade na aktualizaci SP1 smazat uživatelské jméno a heslo pro konfiguraci tohoto proxy serveru. To může způsobit, že synchronizace aktualizací ze serverů Microsoft vygeneruje chybu informující o neplatném parametru. Tento problém vyřešíte obnovením uživatelského jména a hesla pro konfiguraci proxy serveru a opětovnou synchronizací serveru.

#### Problém 7: Jak provést zotavení při selhání upgradu za účelem obnovení konzistentního stavu serveru WSUS a opakování upgradu

Pokud se upgrade na službu WSUS s aktualizací SP1 nezdaří, může u instalace WSUS nastat nekonzistentní nebo nepoužitelný stav. Aby bylo možné tento upgrade opakovat, je třeba uvést instalaci služby WSUS do konzistentního stavu. K tomu můžete použít záložní databázi vytvořenou na začátku procesu upgradu, čímž obnovíte server WSUS do stavu před upgradem.

V případě nezdařeného upgradu opakujte upgrade na službu WSUS s aktualizací SP1 pomocí následujících kroků:

**Opakování upgradu na službu WSUS s aktualizací SP1**
1.  Určete umístění záložní databáze kontrolou obsahu souboru WSUSSetup\_%timestamp%.log. Tento soubor je umístěn v následující složce:

    -   %programfiles%\\Update Services\\LogFiles

2.  Zadáním následujícího příkazu obnovte záložní databázi v počítači se službou WSUS:

    -   osql.exe -S &lt;InstanceDatabáze&gt; -E -Q "USE master ALTER DATABASE SUSDB SET SINGLE\_USER WITH ROLLBACK IMMEDIATE RESTORE DATABASE SUSDB FROM DISK=N'&lt;CestaKZáložníDatabázi&gt;' WITH REPLACE ALTER DATABASE SUSDB SET MULTI\_USER"
    -   Nezapomeňte nahradit hodnoty &lt;InstanceDatabáze&gt; a &lt;CestaKZáložníDatabázi&gt; hodnotami z instalace.
    -   U položky &lt;InstanceDatabáze&gt; použijte hodnotu z následujícího klíče registru:
    -   HKLM\\Software\\Microsoft\\Update Services\\Server\\Setup\\SqlServerName
    -   U položky &lt;CestaKZáložníDatabázi&gt; použijte hodnotu určenou v kroku 1

3.  Odinstalujte službu WSUS, ale ponechejte databázi, soubory protokolu a soubory aktualizací služby WSUS, pokud budete vyzváni k jejich odebrání. (Ujistěte se, zda jsou všechna políčka v části **Odebrat službu Microsoft Windows Server Update Services** nezaškrtnuta.)

4.  Přeinstalujte službu WSUS RTM (původní verze služby WSUS bez aktualizace SP1). Po zobrazení výzvy použijte existující databázi. Tím se systém WSUS vrátí do konzistentního stavu.

5.  Nainstalujte službu WSUS s aktualizací SP1.

**Poznámka:**    Zálohovanou databázi z kroku 1 nelze použít přímo v čisté instalaci služby WSUS s aktualizací SP1. Databázové schéma se změnilo, takže tato databáze nebude kompatibilní bez upgradu na službu WSUS s aktualizací SP1.

#### Problém 8: Upgrade na službu WSUS s aktualizací SP1 může v některých případech po migraci databáze WMSDE selhat

Řešení je různé v závislosti na tom, zda migrujete na místní nebo vzdálený SQL server.

#### Databáze WMSDE migrovaná na místní SQL 2000 server

Je třeba změnit určitý klíč registru, aby balíček instalačního programu služby WSUS s aktualizací SP1 rozpoznal, že neexistuje databáze WMSDE k aktualizaci.

Pokud jste databázi WMSDE migrovali na místní SQL 2000 server, před upgradem na službu WSUS s aktualizací SP1 je třeba provést následující změnu registru:

-   Změňte hodnotu následujícího klíče registru z 1 na 0:
    -   HKLM\\Software\\Microsoft\\Update Services\\Server\\Setup\\WmsdeInstalled  

#### Databáze WMSDE migrovaná na vzdálený SQL 2000 server

Je třeba změnit dvě hodnoty klíče registru, aby balíček instalačního programu služby WSUS s aktualizací SP1 rozpoznal, že neexistuje databáze WMSDE k aktualizaci. Aktualizaci je třeba iniciovat na serveru typu back-end a poté na serveru typu front-end.  

Pokud jste databázi WMSDE migrovali na vzdálený SQL server, před upgradem na službu WSUS s aktualizací SP1 je třeba provést následující změnu registru:

1.  Změňte hodnotu následujícího klíče registru z 1 na 0:
    -   HKLM\\Software\\Microsoft\\Update Services\\Server\\Setup\\WmsdeInstalled 
2.  Změňte hodnotu následujícího klíče registru z "0x80" na "0x20"
    -   HKLM\\Software\\Microsoft\\Update Services\\Server\\Setup\\InstallType 

Po aktualizaci těchto hodnot klíče registru iniciujte upgrade na serveru typu back-end a poté na serveru typu front-end.

#### Problém 9: Služba WSUS s aktualizací SP1 neaktualizuje servery WSUS, které jsou nastaveny pomocí vzdálených nasazení serveru SQL

Balíček instalačního programu služby WSUS s aktualizací SP1 je třeba spustit jak na serveru typu back-end, tak na serveru typu front-end.

**Upgrade na službu WSUS s aktualizací SP1 při použití vzdáleného serveru SQL**
1.  Spusťte instalační balíček na serveru typu front-end bez přepínačů a zvolte upgrade.

2.  Spusťte instalační balíček na serveru typu back-end bez přepínačů a zvolte upgrade.

#### Problém 10: Změna názvu počítače před upgradem na službu WSUS s aktualizací SP1 může způsobit selhání upgradu

Pokud změníte název počítače po instalaci služby WSUS RTM a před upgradem na aktualizaci SP1, může upgrade na službu WSUS s aktualizací SP1 selhat.

Pomocí následujícího skriptu odeberte a znovu přidejte skupiny Administrators pro ASPNET a WSUS. Pak znovu spusťte upgrade.

        ```
		osql.exe -S %computername%\WSUS -E -Q "USE SUSDB DECLARE @asplogin varchar(200) SELECT @asplogin=name from sysusers WHERE name like '%ASPNET' EXEC sp_revokedbaccess @asplogin"
		osql.exe -S %computername%\WSUS -E -Q "USE SUSDB DECLARE @wsusadminslogin varchar(200) SELECT @wsusadminslogin=name from sysusers WHERE name like '%WSUS Administrators' EXEC sp_revokedbaccess @wsusadminslogin"
		 
		osql.exe -S %computername%\WSUS -E -Q "USE SUSDB DECLARE @asplogin varchar(200) SELECT @asplogin=HOST_NAME()+'\ASPNET' EXEC sp_grantlogin @asplogin EXEC sp_grantdbaccess @asplogin EXEC sp_addrolemember webService,@asplogin"
		osql.exe -S %computername%\WSUS -E -Q "USE SUSDB DECLARE @wsusadminslogin varchar(200) SELECT @wsusadminslogin=HOST_NAME()+'\WSUS Administrators' EXEC sp_grantlogin @wsusadminslogin EXEC sp_grantdbaccess @wsusadminslogin EXEC sp_addrolemember webService,@wsusadminslogin"
		 
		osql.exe -S %computername%\WSUS -E -Q "backup database SUSDB to disk=N'<ContentDirectory>\SUSDB.Dat' with init"
		```

		> [!NOTE]
> Může být nutné nahradit hodnotu &lt;ContentDirectory&gt; na posledním řádku cestou ke skutečnému úložišti obsahu. 

V následující části je uveden původní obsah souboru Readme pro službu WSUS
--------------------------------------------------------------------------

Následující text je původním obsahem souboru Readme pro službu WSUS. Služba WSUS s aktualizací SP1 *neřeší* žádný z následujících problémů. Tento obsah je zde uveden pro referenci.

Před zahájením
--------------

#### Problém 1: Musí být instalována služba IIS

Služba Microsoft® Windows Server™ Update Services (WSUS) vyžaduje instalaci Internetové informační služby (IIS). V systémech Microsoft Windows Server 2003 a Microsoft Windows® 2000 Server však služba IIS není ve výchozím nastavení nainstalována, takže instalace služby Windows Server Update Services nemusí pokračovat a zobrazí se chybová zpráva, že služba IIS není instalována.

Instalace služby IIS:

1.  Otevřete Ovládací panely.
2.  Poklepejte na panel **Přidat nebo odebrat programy**.
3.  Klepněte na tlačítko **Přidat nebo odebrat součásti systému Windows**.
4.  V seznamu **Součásti** klepněte na položku **Aplikační server**.
5.  Klepněte na tlačítko **Podrobnosti**.
6.  Zaškrtněte políčko **ASP.NET**. Povolte hodnotu **network COM+ access** a služba IIS bude vybrána automaticky.
7.  Vyberte položku **Internetová informační služba (IIS)** a klepnutím na tlačítko **Podrobnosti** zobrazte seznam volitelných součástí služby IIS.
8.  Vyberte všechny volitelné součásti, které chcete nainstalovat. Volitelné součásti Webové služby zahrnují důležité dílčí součásti, jako například Active Server Pages (ASP) a Vzdálená správa (HTML). Chcete-li tyto dílčí součásti zobrazit a vybrat, klepněte na položku Webová služba a potom na tlačítko Podrobnosti. Klepnutím na tlačítko OK se vraťte k Průvodci součástmi systému Windows.
9.  Klepněte na tlačítko **Další** a dokončete Průvodce součástmi systému Windows.
10. Po instalaci služby IIS spusťte instalační program služby WSUS.

#### Problém 2: U serverů se systémem Windows 2000 Server musí být ve službě IIS před instalací služby WSUS k dispozici nejméně jeden web

Instalačnímu programu služby Windows Server Update Services se nemusí podařit vytvořit web, pokud při spuštění instalačního programu nebyl ve službě ISS k dispozici žádný web. K tomu může například dojít, pokud jste jako jediný web ve službě IIS používali službu Software Update Services (SUS) 1.0 a před instalací služby WSUS jste tento web odstranili.

V takovém případě je nutné vytvořit nový web pomocí modulu snap-in Správce Internetové informační služby (IIS). Potom můžete tento web vybrat nebo zadat během instalace služby WSUS nový web.

Jestliže jste se již pokusili nainstalovat službu WSUS a instalace se nezdařila, protože nebyl k dispozici žádný web, otevřete modul snap-in Správce Internetové informační služby a odstraňte Web \#1. Pak proveďte dříve popsané kroky a znovu spusťte instalační program.

#### Problém 3: Instalace požadovaných součástí

#### Požadavky na software

Následující tabulka uvádí požadovaný software pro jednotlivé podporované operační systémy. Před spuštěním instalačního programu služby WSUS musí server WSUS splňovat požadavky uvedené v následujícím seznamu. Pokud některá z těchto aktualizací vyžaduje restartování počítače po dokončení instalace, restartujte počítač před instalací služby WSUS.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Operační systém</th>
<th style="border:1px solid black;" >Požadavky</th>
<th style="border:1px solid black;" >Soubory ke stažení</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Všechny operační systémy</td>
<td style="border:1px solid black;">Internetová informační služba (IIS) 5.0</td>
<td style="border:1px solid black;">Instalace z operačního systému.
Viz Problém 1: Musí být instalována služba IIS.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Všechny operační systémy</td>
<td style="border:1px solid black;">Služba inteligentního přenosu na pozadí (BITS) 2.0</td>
<td style="border:1px solid black;">Informace týkající se operačních systémů Windows Server 2003 získáte v článcích Aktualizace na Službu inteligentního přenosu na pozadí (BITS) 2.0 a WinHTTP 5.1 Windows Server 2003 (KB842773) na webu služby Stažení softwaru (<a href="http://go.microsoft.com/fwlink/?linkid=47251">http://go.microsoft.com/fwlink/?LinkId=47251</a>).
Informace týkající se operačních systémů Windows Server 2000 získáte v článcích Aktualizace na Službu inteligentního přenosu na pozadí (BITS) 2.0 a WinHTTP 5.1 Windows 2000 (KB842773) na webu služby Stažení softwaru (<a href="http://go.microsoft.com/fwlink/?linkid=46794">http://go.microsoft.com/fwlink/?LinkId=46794</a>).</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Systém Windows Server 2003</td>
<td style="border:1px solid black;">Aktualizace Microsoft .NET Framework 1.1 Service Pack 1 pro systém Windows Server 2003</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=47358">Aktualizace Microsoft .NET Framework 1.1 Service Pack 1 pro systém Windows Server 2003</a>
Případně přejděte na web služby <a href="http://go.microsoft.com/fwlink/?linkid=47370">Windows Update</a> a vyhledejte důležité aktualizace a aktualizace Service Packs; instalace služby Microsoft .NET Framework 1.1 Service Pack 1 pro systém Windows Server 2003.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows Server 2003</td>
<td style="border:1px solid black;">Databázový software, který je stoprocentně kompatibilní se serverem Microsoft SQL</td>
<td style="border:1px solid black;">Neuvedeno</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows 2000 Server</td>
<td style="border:1px solid black;">Databázový software, který je stoprocentně kompatibilní se serverem Microsoft SQL</td>
<td style="border:1px solid black;">Pokud nepoužíváte Microsoft SQL Server 2000, můžete nainstalovat službu MSDE 2000 (Microsoft SQL Server 2000 Desktop Engine). Tento postup sestává z několika kroků. Další informace získáte v následující části Instalace služby MSDE v systému Windows 2000.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows 2000 Server</td>
<td style="border:1px solid black;">Microsoft Internet Explorer 6.0 Service Pack 1</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=47359">Internet Explorer 6 Service Pack 1</a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows 2000 Server</td>
<td style="border:1px solid black;">Microsoft .NET Framework Version 1.1 Redistributable Package</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=47369">Microsoft .NET Framework Version 1.1 Redistributable Package</a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows 2000 Server</td>
<td style="border:1px solid black;">Microsoft .NET Framework 1.1 Service Pack 1</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=47368">Microsoft .NET Framework 1.1 Service Pack 1</a>
Případně přejděte na web služby <a href="http://go.microsoft.com/fwlink/?linkid=47370">Windows Update</a> a vyhledejte důležité aktualizace a aktualizace Service Pack; nainstalujte rozhraní Microsoft .NET Framework 1.1 Service Pack 1 pro systém Windows Server 2000.</td>
</tr>
</tbody>
</table>
 

Kromě těchto požadavků může služba WSUS v případě potřeby na serveru instalovat nebo konfigurovat rozhraní ASP.NET verze 1.1. (Instalační program služby WSUS konfiguruje rozhraní ASP.NET.)

#### Instalace služby MSDE 2000 v systému Windows 2000

Používáte-li pro službu WSUS systém Windows 2000 a nemáte přístup k serveru Microsoft SQL Server 2000, měli byste před spuštěním instalačního programu služby WSUS spustit službu Microsoft SQL Server 2000 Desktop Engine (MSDE). Pokud je na serveru WSUS již nainstalovaná služba MSDE, nemusíte pro službu WSUS zřizovat její speciální instanci. Stačí, když při instalaci služby WSUS pouze označíte název stávající instance.

Postup instalace služby MSDE v systému Windows 2000 Server má čtyři kroky. Nejprve je třeba stáhnout a rozbalit archiv MSDE do složky na serveru WSUS. Pak pomocí příkazového řádku a možností příkazového řádku spusťte instalační program služby MSDE, nastavte heslo SA a jako název instance přiřaďte WSUS. Po dokončení instalace služby MSDE byste měli ověřit, zda je instance služby WSUS spuštěna jako služba NT. Nakonec je třeba zajistit ochranu serveru WSUS přidáním opravy zabezpečení ke službě MSDE.

#### Krok 1: Stažení a rozbalení archivu služby MSDE

Archiv MSDE je třeba stáhnout a rozbalit do složky na serveru WSUS. Viz [Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) verze A](http://go.microsoft.com/fwlink/?linkid=47366).

#### Krok 2: Instalace služby MSDE

Pomocí příkazového řádku a možností příkazového řádku spusťte instalační program služby MSDE, nastavte heslo SA a jako název instance přiřaďte WSUS. Po dokončení instalace služby MSDE byste měli ověřit, zda je instance služby WSUS spuštěna jako služba NT.

Chcete-li nainstalovat službu MSDE, nastavte heslo SA a přiřaďte název instance:

1.  Na příkazovém řádku přejděte do instalační složky služby MSDE zadané v kroku 1: Stažení a rozbalení archivu služby MSDE.
2.  Zadejte následující příkaz: **setup sapwd="***password***" instancename=WSUS***,*
    kde *password* je silné heslo účtu SA v této instanci služby MSDE a **instancename** je název databázové instance. Alternativně můžete pro databázi WSUS použít výchozí název instance (namísto WSUS). Pokud se tak rozhodnete učinit, nemusíte do parametru příkazového zadávat řádku text **název\_instance=WSUS**. Tento příkaz spustí instalační program služby MSDE, nastaví heslo SA a pojmenuje tuto instanci služby MSDE libovolnou zadanou hodnotou.

#### Krok 3: Ověření, zda je instalována instance WSUS služby MSDE

1.  Klepněte na tlačítko **Start** a pak na příkaz **Spustit**.
2.  Do pole **Otevřít** zadejte příkaz **services.msc** a klepněte na tlačítko **OK**.

Procházením seznamu služeb ověřte, zda existuje služba s názvem MSSQL$WSUS (pokud jste pro název instance použili WSUS) nebo MSSQLSERVER (pokud jste použili výchozí název instance).

#### Krok 4: Spuštění instance služby MSDE.

Na konci instalace služby MSDE je třeba spustit instanci. Pokud jste jako název instance zadali WSUS, spustíte instanci MSSQL$WSUS. Pokud jste použili výchozí název instance, spustíte instanci MSSQLSERVER. Jestliže tuto službu nespustíte, služba WSUS nebude moci použít databázovou instanci.

#### Krok 5: Aktualizace služby MSDE

Je třeba stáhnout a nainstalovat opravu zabezpečení popsanou v bulletinu [MS03-031: Kumulativní oprava zabezpečení pro SQL Server](http://go.microsoft.com/fwlink/?linkid=47364).

Informace o stažení opravy zabezpečení získáte v článku [Oprava zabezpečení pro SQL Server 2000 (32bitový) MS03-031](http://go.microsoft.com/fwlink/?linkid=47363).

#### Problém 4: Minimální požadavky na místo na disku

V následující části jsou uvedeny minimální požadavky na místo na disku pro instalaci služby Windows Server Update Services:

-   1 GB na systémovém oddílu,
-   2 GB pro svazek, na němž budou uloženy databázové soubory,
-   6 GB, na základě počtu projekcí obsahu.

#### Problém 5: Před instalací nejnovější verze je třeba odinstalovat dřívější verze služby WSUS pomocí panelu nástrojů Přidat nebo odebrat programy.

Pokud se chystáte instalovat službu Windows Server Update Services na server, na němž je nainstalována služba Windows Update Services verze Beta 1 nebo Beta 2, je třeba nejprve odinstalovat dřívější verzi pomocí ovládacího panelu Přidat nebo odebrat programy.

#### Problém 6: Služba WSUS vyžaduje zapnutí volby vnořených aktivačních procedur na serveru SQL Server

Tato volba je ve výchozím nastavení zapnutá, může ji však vypnout správce serveru SQL.

Pokud se jako úložiště dat služby Windows Server Update Services chystáte použít databázi serveru SQL Server, měl by správce serveru SQL Server ověřit, zda je zapnutá funkce vnořených aktivačních procedur na serveru ještě předtím, než správce služby WSUS nainstaluje službu WSUS a určí během instalace databázi.

Instalační program služby WSUS zapne možnost RECURSIVE\_TRIGGERS, která je specifická pro databázi. Nezapne však volbu vnořených aktivačních procedur, což je globální volba serveru.

Chcete-li se přesvědčit, zda jsou zapnuté vnořené aktivační procedury, použijte následující příkaz:

**sp\_configure 'nested triggers'**

Chcete-li zapnout možnost vnořených aktivačních procedur na serveru SQL Server, spusťte následující příkaz z dávkového souboru v počítači se spuštěným serverem SQL Server:

**sp\_configure 'nested triggers', 1**

**GO**

**RECONFIGURE**

**GO**

#### Problém 7: Parametry příkazového řádku instalačního programu služby WSUS

Můžete provést bezobslužnou instalaci služby WSUS. Další informace a parametry příkazového řádku uvádí Příloha A: Bezobslužná instalace v článku [Nasazení služby Microsoft Windows Server Update Services](http://go.microsoft.com/fwlink/?linkid=41777).

Známé problémy
--------------

#### Problém 1: Průvodce uzamčením zabezpečení služby IIS

Pokud Internetovou informační službu (IIS) provozujete v počítači se systémem Windows 2000 Server, nainstalujte nejnovější verzi Průvodce uzamčením zabezpečení služby IIS (která obsahuje program URLScan) ze stránky nástroje Lockdown služby IIS na webu Microsoft TechNet. Společnost Microsoft důrazně doporučuje instalaci tohoto nástroje, který vám pomůže zachovat zabezpečení serverů IIS. Průvodce uzamčením zabezpečení služby IIS funguje tak, že vypne nepotřebné funkce služby IIS a sníží tak riziko ohrožení zabezpečení.

> [!NOTE]
> Instalační program služby WSUS tyto součásti neinstaluje. Je třeba je nainstalovat ručně. Nástroj IIS Lockdown není nutné instalovat do počítačů se systémem Windows Server 2003, protože tato funkce je integrovaná. 

#### Problém 2: Změna konfigurace služby WSUS přímo v databázi není podporována.

Služba Windows Server Update Services ukládá konfigurační data do databáze (MSDE nebo SQL Server). Změna konfiguračních dat přímým přístupem do databáze však není podporována. Správci by se neměli pokoušet změnit konfiguraci služby WSUS tímto způsobem. Podporovaný způsob změny konfigurace služby WSUS je prostřednictvím konzoly WSUS nebo voláním rozhraní API služby WSUS.

#### Problém 3: K webu pro správu služby WSUS lze získat přístup pouze při povolení aktivního skriptování.

V pracovní stanici správce je třeba konfigurací aplikace Internet Explorer povolit aktivní skriptování. Teprve potom můžete z aplikace Internet Explorer získat přístup k webu pro správu služby WSUS.

#### Problém 4: Služba IIS bude během instalace WSUS restartována

Instalační program služby Windows Server Update Services restartuje službu IIS bez upozornění. To může mít vliv na stávající weby v organizaci.

#### Problém 5: Změna přístupu bodů pro správu (MP) do virtuálního adresáře služby WSUS nebo SMS

Ve výchozím nastavení je virtuální adresář obsahu pro službu Windows Server Update Services nastaven s anonymním přístupem. Pokud toto nastavení změníte tak, aby bylo vyžadováno ověření, při ověřování klientů dojde k chybám a bude jim odepřen přístup ke stahování aktualizací. Jedná se o známý problém, kdy knihovna Winhttp.dll používá chybný kontext ověřování, pokud je požadováno implicitní ověřování, takže výzva k ověření se nezdaří. Abyste tomuto problému zabránili, musí být body MP serveru WSUS a SMS nastaveny s anonymním přístupem do virtuálních adresářů služby IIS.

#### Problém 6: Při instalaci služby WSUS v systému Windows Small Business Server 2003 je třeba změnit výchozí nastavení přístupu k virtuálním kořenovým adresářům služby WSUS tak, aby klienti WSUS sami stahovali aktualizace ze serveru

Server WSUS Server nainstaluje dva virtuální kořenové adresáře, SelfUpdate a ClientWebService a některé soubory v domovském adresáři na výchozím webu (na portu 80). Klienti tak mohou sami provádět aktualizaci prostřednictvím výchozího webu. Ve výchozím nastavení je v systému Windows Small Business Server 2003 výchozí web konfigurován tak, že kromě serveru odepírá přístup všem adresám IP nebo místním hostitelům. To znamená, že k virtuálním kořenovým adresářům SelfUpdate a ClientWebService je odepřen přístup, takže klienti nemohou sami provést aktualizaci. Chcete-li klientům udělit přístup, aby mohli sami provádět aktualizaci, ve virtuálních kořenových adresářích SelfUpdate a ClientWebService výchozího webu proveďte následující postup.

1.  Ve virtuálním kořenovém adresáři klepněte na tlačítko **Vlastnosti**, na položku **Zabezpečení adresáře**, na možnost **Omezení podle adres IP a názvů domén** a potom klepněte na tlačítko **Upravit**.
2.  Klepněte na možnost **Udělen přístup** a potom na tlačítko **OK**. Zavřete všechny stránky vlastností.

#### Problém 7: Instalace služby WSUS v systému Small Business Server - problémy s integrací

-   Pokud systém Windows Small Business Server 2003 používá pro přístup na Internet proxy server ISA, je třeba v uživatelském rozhraní **Nastavení** zadat ručně následující hodnoty: nastavení proxy serveru, název proxy serveru a port.
-   Používá-li služba ISA Ověřování systému Windows, je třeba zadat ověření proxy serveru přímo v podobě DOMÉNA\\uživatel (uživatel patřící do domény Internet Users).

#### Problém 8: Při přesouvání počítače z jedné skupiny počítačů do jiné může trvat až hodinu, než se počítač zobrazí v nové skupině při prohlížení z konzoly pro správu

Pokud je počítač přiřazen k cílové skupině poprvé, jsou data v tomto počítači upravena informacemi o skupině. Tato data jsou aktualizována pravidelně nebo každou hodinu. Při přesouvání počítače z jedné skupiny do jiné proto může aktualizace informací v klientovi a zobrazení těchto změněných informací v konzole pro správu WSUS trvat až hodinu.

#### Problém 9: Při instalaci služby WSUS na členský server a následném povýšení členského serveru na řadič domény je vhodné nejprve odinstalovat službu WSUS

Jestliže službu WSUS instalujete na členský server a následně chcete tento server povýšit na řadič domény, je třeba provést následující kroky:

1.  Odinstalujte službu WSUS.
2.  Povyšte server na řadič domény.
3.  Znovu nainstalujte službu WSUS.

#### Problém 10: Při snížení úrovně serveru WSUS z řadiče domény na členský server je vhodné nejprve odinstalovat službu WSUS

Používáte-li server WSUS v řadiči domény a chcete snížit úroveň řadiče domény na členský server, je třeba provést tyto kroky:

1.  Odinstalujte službu WSUS a zachovejte databázi.
2.  Vytvořte uživatelský účet s názvem ASPNET.
3.  Na příkazovém řádku zadejte příkaz **aspnet\_regiis -i**.
4.  Znovu nainstalujte službu WSUS a použijte zachovanou databázi.

#### Problém 11: Pokud je po instalaci služby WSUS nainstalováno rozhraní .NET Framework 1.0 nebo 2.0, konzola pro správu služby WSUS se nezobrazí

Příčinou je skutečnost, že rozhraní .NET Framework 1.0 je registrováno u služby IIS a server WSUS vyžaduje rozhraní .NET Framework 1.1. Tento problém vyřešíte tak, že otevřete soubor aspnet\_regiis.exe a spustíte následující příkazy, kde *website id* je hodnota obsažená v následujícím klíči registru:

HKLM\\Software\\Microsoft\\WindowsUpdateServices\\Server\\Setup\\IISTargetWebsiteIndex

-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*website id*&gt;\\ROOT\\ReportingWebService
-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*website id*&gt;\\ROOT\\ClientWebService
-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*website id*&gt;\\ROOT\\SimpleAuthWebService
-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*website id*&gt;\\ROOT\\WSUSAdmin
-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*website id*&gt;\\ROOT\\AdministrationWebService
-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*website id*&gt;\\ROOT\\ServrSyncWebService
-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*website id*&gt;\\ROOT\\DssAuthWebService
-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*website id*&gt;\\ROOT\\Content

#### Problém 12: Omezení vzdálené instalace serveru SQL

Služba WSUS nabízí omezenou podporu databázového softwaru, který běží v jiném počítači než zbývající část aplikace WSUS.

-   Počítač se systémem Windows 2000 Server nelze použít jako počítač typu front-end ve vzdálené dvojici SQL.
-   Server nakonfigurovaný jako řadič domény nelze použít jako počítač typu front-end ani back-end vzdálené dvojice SQL.
-   Služby WMSDE nebo MSDE nelze použít pro databázový software v počítači typu back-end.
-   Nastavení vzdáleného serveru SQL Server (pro databázi služby WSUS) se nezdaří, pokud je na vzdáleném serveru instalována Terminálová služba, která je spuštěna v aplikačním režimu. Při instalaci serveru SQL Server na server Terminálové služby je třeba provést následující kroky:
    1.  Před spuštěním instalačního programu otevřete příkazový řádek a zadejte příkaz: change user /install
    2.  Spusťte instalaci serveru SQL Server.
    3.  Po spuštění instalačního programu zadejte na příkazovém řádku příkaz: change user /execute
-   Aby bylo možné nastavit databázi služby WSUS na vzdáleném serveru SQL Server, musíte být členem místní skupiny zabezpečení Administrators v počítači typu front-end i back-end.
-   Další informace o problémech se vzdáleným serverem SQL získáte v Příloze C: Vzdálený server SQL v článku [Nasazení služby Microsoft Windows Server Update Services](http://go.microsoft.com/fwlink/?linkid=41777).

#### Problém 13: Podřízený server repliky může mít méně schválení než nadřazený server

Podřízený server repliky může mít méně schválení než nadřazený server. Důvodem je skutečnost, že schválení instalace nepřecházejí na podřízený server, dokud neskončí stahování obsahu na nadřazeném serveru.

#### Problém 14: Opakování synchronizace při počátečním selhání synchronizace

Pokud se synchronizace nezdaří, měli byste se nejprve pokusit ji zopakovat. Jestliže se nezdaří ani následný pokus o synchronizaci, použijte informace poradce při potížích v Provozní příručce služby WSUS.

#### Problém 15: Při pokusu o přístup do konzoly pro správu služby WSUS se zobrazí chybová zpráva System.IO.FileNotFoundException

Pokud se zobrazí následující chybová zpráva, bude zřejmě nutné nastavit oprávnění u síťové služby nebo účtů služby ASP.NET:

System.IO.FileNotFoundException: Nebyl nalezen soubor nebo sestavení s názvem *xxxxxx*.dll nebo některé z jeho závislostí,

kde *xxxxxx* je náhodný název.

Chcete-li tento problém vyřešit v operačním systému Windows Server 2003, udělte účtu síťové služby oprávnění pro čtení a zápis ke složce %systemroot%\\Temp. V systému Windows 2000 Server udělte účtu ASP.NET síťové služby oprávnění pro čtení a zápis ke složce %systemroot%\\Temp.

#### Problém 16: Aktualizace zabezpečení serveru SQL MS03-031 (KB815495)

Může se zdát, že je tato aktualizace nainstalovaná na serveru WSUS, přestože instalace u klienta se ve skutečnosti nezdařila. To může způsobit, že balíček bude klientovi znovu nabídnut. Tento problém můžete obejít zrušením schválení aktualizace na serveru.

#### Problém 17: Nastavení služby IIS se během upgradu služby RTM ztratí.

Pokud službu WSUS RTM nainstalujete na server s předchozí verzí služby WSUS (například RC), služba WSUS RTM odinstaluje dřívější verzi a pak nainstaluje verzi novou. To znamená, že virtuální kořenové adresáře a soubory spojené se službou WSUS ve službě IIS budou odstraněny.

Pokud jste službu WSUS nainstalovali na výchozím webu, ztratíte veškerá nastavení související se službou WSUS, která jste vytvořili ve virtuálních kořenových adresářích služby WSUS. Jestliže jste například nakonfigurovali virtuální kořenové adresáře služby WSUS pro protokol SSL za účelem zabezpečení služby WSUS, bude nutné je po instalaci verze RTM služby WSUS znovu nakonfigurovat. Poznámka: Obdržíte upozornění konzoly služby WSUS, že protokol SSL není povolen.

Pokud jste službu WSUS nainstalovali na jiný než výchozí web, všechna další nastavení na úrovni webu WSUS se ztratí.

#### Problém 18: Použití záhlaví hostitele

Chcete-li u služby IIS přiřadit výchozímu webu (web WSUS) hodnoty záhlaví hostitele, je třeba do seznamu adres IP pro výchozí web přidat hodnotu Všechny nepřiřazené nebo přiřazenou adresu IP bez hodnoty záhlaví hostitele. Je vhodné přidat je také na web, který není výchozí.

**Varování**: Tím může dojít k porušení funkčnosti serverů Microsoft SharePoint a Exchange.

#### Problém 19: Do zóny webového obsahu Důvěryhodné servery a Místní intranet počítačů, v nichž je povoleno posílení zabezpečení aplikace Internet Explorer, musí být přidána adresa URL konzoly služby WSUS

Pokud je v počítači povoleno posílení zabezpečení aplikace Internet Explorer (známé také jako součást Rozšířené nastavení zabezpečení aplikace Internet Explorer v systému Microsoft Windows Server 2003) a nepřidáte konzolu WSUS do zón obsahu Důvěryhodné servery a Místní intranet, budete vyzváni k zadání ověřovacích údajů uživatele při každém otevření stránky v konzole WSUS.

Přidání konzoly WSUS do zón webového obsahu **Místní intranet** a **Důvěryhodné servery**:

1.  Otevřete nabídku **Možnosti Internetu** (například klepnutím na tlačítko **Start**, položku **Ovládací panely** a panel **Možnosti Internetu**).
2.  Na kartě **Zabezpečení** klepněte na ikonu **Místní intranet**, potom klepněte na tlačítko **Servery**, na tlačítko **Upřesnit**, přidejte adresu URL (http://*NázevServeruWSUS*/WSUSAdmin) a klepněte na tlačítko **OK**.
3.  Klepněte na ikonu **Důvěryhodné servery**, na tlačítko **Servery**, přidejte adresu URL konzoly WSUS, klepněte na tlačítko **OK** a dalším klepnutím na tlačítko **OK** zavřete dialogové okno **Možnosti Internetu**.

#### Autorská práva

Informace obsažené v tomto dokumentu představují aktuální názor společnosti Microsoft na problémy známé k datu vydání. Protože společnost Microsoft musí reagovat na měnící se podmínky trhu, nelze je považovat za závazek ze strany společnosti Microsoft, přičemž společnost Microsoft nemůže zaručit správnost informací zveřejněných po datu vydání.

Tento dokument je určen pouze pro informační účely. SPOLEČNOST MICROSOFT NEPOSKYTUJE NA INFORMACE UVEDENÉ V TOMTO DOKUMENTU ŽÁDNÉ ZÁRUKY, AŤ UŽ VÝSLOVNĚ UVEDENÉ, MLČKY PŘEDPOKLÁDANÉ NEBO VYPLÝVAJÍCÍ ZE ZÁKONA.

Za splnění veškerých požadavků všech příslušných zákonů na ochranu autorských práv odpovídá uživatel. Bez předchozího písemného svolení společnosti Microsoft nesmí být žádná část tohoto dokumentu za žádným účelem reprodukována, ukládána, zaváděna do vyhledávácích systémů nebo přenášena jakoukoli formou (elektronicky, mechanicky, pomocí fotokopií, záznamů nebo jinak). Autorská práva nejsou tímto ustanovením dotčena.

Společnost Microsoft může vlastnit patenty, patentové přihlášky, chráněné známky, autorská práva nebo jiná práva k duševnímu vlastnictví týkající se předmětu tohoto dokumentu. Není-li v písemné licenční smlouvě společnosti Microsoft výslovně uvedeno jinak, nejsou předáním tohoto dokumentu poskytnuty žádné licence na takové patenty, chráněné známky, autorská práva nebo jiné duševní vlastnictví.

Pokud není uvedeno jinak, jsou názvy společností, organizací, produktů, názvy domén, e-mailové adresy, loga, osoby, místa či události použité v ukázkách smyšlené a nemůže být vyvozováno žádné jejich spojení se skutečnou společností, organizací, produktem, názvem domény, e-mailovou adresou, logem, osobou, místem či událostí.

© 2006 Microsoft Corporation. Všechna práva vyhrazena.

Microsoft, SQL Server, Windows a Windows Server jsou registrované ochranné známky nebo ochranné známky společnosti Microsoft Corporation ve Spojených státech amerických a v dalších zemích.

Názvy skutečných společností a produktů uvedené v tomto dokumentu mohou být ochrannými známkami příslušných vlastníků.
