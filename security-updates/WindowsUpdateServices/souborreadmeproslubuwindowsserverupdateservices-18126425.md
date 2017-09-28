---
TOCTitle: Soubor ReadMe pro službu Windows Server Update Services
Title: Soubor ReadMe pro službu Windows Server Update Services
ms:assetid: '4244109a-395a-4ff8-9989-ea55ab0964a3'
ms:contentKeyID: 18126425
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc720505(v=WS.10)'
---

Soubor ReadMe pro službu Windows Server Update Services
=======================================================

Tento dokument popisuje známé problémy ovlivňující službu Windows Server Update Services (WSUS). Obsahuje doporučení a požadavky na instalaci služby WSUS.

| ![](images/Cc720505.note(WS.10).gif)Poznámka                                                                                                                |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Kopie tohoto dokumentu je k dispozici ke stažení na webu služby Stažení softwaru na adrese [http://go.microsoft.com/fwlink/?LinkId=48126](http://go.microsoft.com/fwlink/?linkid=48126). |

Před zahájením
--------------

#### Problém 1: Musí být instalována služba IIS

Služba Microsoft® Windows Server™ Update Services (WSUS) vyžaduje instalaci Internetové informační služby (IIS). V systémech Microsoft Windows Server 2003 a Microsoft Windows® 2000 Server však služba IIS není ve výchozím nastavení nainstalována, takže instalace služby Windows Server Update Services nemusí pokračovat a zobrazí se chybová zpráva, že služba IIS není instalována.

Instalace služby IIS:

1.  Otevřete Ovládací panely.
2.  Poklepejte na panel **Přidat nebo odebrat programy**.
3.  Klepněte na tlačítko **Přidat nebo odebrat součásti systému**.
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

Jestliže jste se již pokusili nainstalovat službu WSUS a instalace se nezdařila, protože nebyl k dispozici žádný web, otevřete modul snap-in Správce Internetové informační služby a odstraňte web č. 1. Pak proveďte dříve popsané kroky a znovu spusťte instalační program.

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
<th>Operační systém</th>
<th>Požadavky</th>
<th>Soubory ke stažení</th>
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
<td style="border:1px solid black;">Informace týkající se operačních systémů Windows Server 2003 získáte v článku <a href="http://go.microsoft.com/fwlink/?linkid=47251">Aktualizace služby inteligentního přenosu na pozadí (BITS) na verzi 2.0 a protokolu WinHTTP 5.1 pro systém Windows Server 2003</a> (KB842773) na webu služby Stažení softwaru (http://go.microsoft.com/fwlink/?LinkId=47251).
Informace týkající se operačních systémů Windows Server 2000 získáte v článku <a href="http://go.microsoft.com/fwlink/?linkid=46794">Aktualizace služby inteligentního přenosu na pozadí (BITS) na verzi 2.0 a protokolu WinHTTP 5.1 pro systém Windows 2000</a> (KB842773) na webu služby Stažení softwaru (http://go.microsoft.com/fwlink/?LinkId=46794).</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows Server 2003</td>
<td style="border:1px solid black;">Aktualizace Microsoft .NET Framework 1.1 Service Pack 1 pro systém Windows Server 2003</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=47358">Aktualizace Microsoft .NET Framework 1.1 Service Pack 1 pro systém Windows Server 2003</a>
Případně přejděte na web služby <a href="http://go.microsoft.com/fwlink/?linkid=47370">Windows Update</a> a vyhledejte důležité aktualizace a aktualizace Service Pack; nainstalujte aktualizaci Microsoft .NET Framework 1.1 Service Pack 1 pro systém Windows Server 2003.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows Server 2003</td>
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
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=47359">Internet Explorer 6 Service Pack 1</a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows 2000 Server</td>
<td style="border:1px solid black;">Microsoft .NET Framework Version 1.1 Redistributable Package</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=47369">Microsoft .NET Framework Version 1.1 Redistributable Package</a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows 2000 Server</td>
<td style="border:1px solid black;">Microsoft .NET Framework 1.1 Service Pack 1</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=47368">Microsoft .NET Framework 1.1 Service Pack 1</a>
Případně přejděte na web služby <a href="http://go.microsoft.com/fwlink/?linkid=47370">Windows Update</a> a vyhledejte důležité aktualizace a aktualizace Service Pack; nainstalujte aktualizaci Microsoft .NET Framework 1.1 Service Pack 1 pro systém Windows Server 2000.</td>
</tr>
</tbody>
</table>
 

Kromě těchto požadavků může služba WSUS v případě potřeby na serveru nainstalovat nebo nakonfigurovat rozhraní ASP.NET verze 1.1. (Instalační program služby WSUS konfiguruje rozhraní ASP.NET.)

#### Instalace služby MSDE 2000 v systému Windows 2000

Používáte-li pro službu WSUS systém Windows 2000 a nemáte přístup k serveru Microsoft SQL Server 2000, měli byste před spuštěním instalačního programu služby WSUS spustit službu Microsoft SQL Server 2000 Desktop Engine (MSDE). Pokud je služba MSDE na serveru WSUS již nainstalována, nemusíte pro službu WSUS nastavovat její zvláštní instanci. Stačí, když při instalaci služby WSUS pouze označíte název stávající instance.

Postup instalace služby MSDE v systému Windows 2000 Server má čtyři kroky. Nejprve je třeba stáhnout a rozbalit archiv MSDE do složky na serveru WSUS. Pak pomocí příkazového řádku a parametrů příkazového řádku spusťte instalační program služby MSDE, nastavte heslo správce systému a jako název instance přiřaďte hodnotu WSUS. Po dokončení instalace služby MSDE byste měli ověřit, zda je instance služby WSUS spuštěna jako služba NT. Nakonec je třeba zajistit ochranu serveru WSUS přidáním aktualizace zabezpečení ke službě MSDE.

#### Krok 1: Stažení a rozbalení archivu služby MSDE

Archiv MSDE je třeba stáhnout a rozbalit do složky na serveru WSUS. Viz [Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) verze A](http://go.microsoft.com/fwlink/?linkid=47366).

#### Krok 2: Instalace služby MSDE

Pomocí příkazového řádku a parametrů příkazového řádku spusťte instalační program služby MSDE, nastavte heslo správce systému a jako název instance přiřaďte hodnotu WSUS. Po dokončení instalace služby MSDE byste měli ověřit, zda je instance služby WSUS spuštěna jako služba NT.

Chcete-li nainstalovat službu MSDE, nastavte heslo správce systému a přiřaďte název instance:

1.  Na příkazovém řádku přejděte do instalační složky služby MSDE zadané v kroku 1: Stažení a rozbalení archivu služby MSDE.
2.  Zadejte následující příkaz: **setup sapwd="***heslo***" instancename=WSUS***,*
    kde *heslo* je silné heslo účtu správce systému v této instanci služby MSDE a **instancename** je název databázové instance. Pro databázi WSUS můžete také použít výchozí název instance (namísto hodnoty WSUS). Pokud se rozhodnete pro tuto možnost, nemusíte do parametru příkazového řádku zadávat text **instancename=WSUS**. Příkaz spustí instalační program služby MSDE, nastaví heslo správce systému a pojmenuje danou instanci služby MSDE libovolnou zadanou hodnotou.

#### Krok 3: Ověření, zda je nainstalována instance WSUS služby MSDE

Měli byste ověřit, zda se instance WSUS služby MSDE zobrazuje.

1.  Klepněte na tlačítko **Start** a pak na příkaz **Spustit**.
2.  Do pole **Otevřít** zadejte příkaz **services.msc** a klepněte na tlačítko **OK**.

Procházením seznamu služeb ověřte, zda existuje služba s názvem MSSQL$WSUS (pokud jste jako název instance zadali hodnotu WSUS) nebo MSSQLSERVER (pokud jste použili výchozí název instance).

#### Krok 4: Spuštění instance služby MSDE

Na konci instalace služby MSDE je třeba spustit instanci. Pokud jste jako název instance zadali hodnotu WSUS, spustíte instanci MSSQL$WSUS. Pokud jste použili výchozí název instance, spustíte instanci MSSQLSERVER. Jestliže tuto službu nespustíte, služba WSUS nebude moci použít databázovou instanci.

#### Krok 5: Aktualizace služby MSDE

Je třeba stáhnout a nainstalovat aktualizaci zabezpečení popsanou v bulletinu [MS03-031: Kumulativní oprava zabezpečení pro SQL Server](http://go.microsoft.com/fwlink/?linkid=47364).

Informace o stažení aktualizace zabezpečení získáte v článku [SQL Server 2000 (32-bit) Security Patch MS03-031](http://go.microsoft.com/fwlink/?linkid=47363) (Oprava zabezpečení pro SQL Server 2000 \[32bitový\] MS03-031) (stránka může být v angličtině).

#### Problém 4: Minimální požadavky na místo na disku

V následující části jsou uvedeny minimální požadavky na místo na disku pro instalaci služby Windows Server Update Services:

-   1 GB na systémovém oddílu,
-   2 GB pro svazek, na němž budou uloženy databázové soubory,
-   6 GB, na základě počtu projekcí obsahu.

#### Problém 5: Před instalací nejnovější verze je třeba odinstalovat dřívější verze služby WSUS pomocí panelu nástrojů Přidat nebo odebrat programy.

Pokud se chystáte instalovat službu Windows Server Update Services na server, na němž je nainstalována služba Windows Update Services verze Beta 1 nebo Beta 2, je třeba nejprve odinstalovat dřívější verzi pomocí ovládacího panelu Přidat nebo odebrat programy.

#### Problém 6: Služba WSUS vyžaduje zapnutí možnosti vnořených aktivačních procedur na serveru SQL Server

Tato možnost je ve výchozím nastavení zapnuta. Může ji však vypnout správce serveru SQL.

Pokud se jako úložiště dat služby Windows Server Update Services chystáte použít databázi serveru SQL Server, měl by správce serveru SQL Server ověřit, zda je zapnuta funkce vnořených aktivačních procedur na serveru ještě předtím, než správce služby WSUS nainstaluje službu WSUS a určí během instalace databázi.

Instalační program služby WSUS zapne možnost RECURSIVE\_TRIGGERS, která je specifická pro databázi. Nezapne však možnost vnořených aktivačních procedur, což je globální možnost serveru.

Chcete-li se přesvědčit, zda jsou vnořené aktivační procedury zapnuty, použijte následující příkaz:

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

Pokud Internetovou informační službu (IIS) provozujete v počítači se systémem Windows 2000 Server, nainstalujte nejnovější verzi Průvodce uzamčením zabezpečení služby IIS (která obsahuje program URLScan) ze stránky nástroje Lockdown služby IIS na webu Microsoft TechNet. Společnost Microsoft důrazně doporučuje instalaci tohoto nástroje, který vám pomůže zachovat zabezpečení serverů IIS. Průvodce uzamčením zabezpečení služby IIS funguje tak, že vypne nepotřebné funkce služby IIS a tímto způsobem sníží riziko ohrožení zabezpečení.

| ![](images/Cc720505.note(WS.10).gif)Poznámka                                                                                                                                                    |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Instalační program služby WSUS tyto součásti neinstaluje. Je třeba je nainstalovat ručně. Nástroj Lockdown služby IIS není nutné instalovat do počítačů se systémem Windows Server 2003, protože tato funkce je integrovaná. |

#### Problém 2: Změna konfigurace služby WSUS přímo v databázi není podporována

Služba Windows Server Update Services ukládá konfigurační data do databáze (MSDE nebo SQL Server). Změna konfiguračních dat přímým přístupem do databáze však není podporována. Správci by se neměli pokoušet změnit konfiguraci služby WSUS tímto způsobem. Podporovaný způsob změny konfigurace služby WSUS je prostřednictvím konzoly WSUS nebo voláním rozhraní API služby WSUS.

#### Problém 3: K webu pro správu služby WSUS lze získat přístup pouze při povolení aktivního skriptování

V pracovní stanici správce je třeba konfigurací aplikace Internet Explorer povolit aktivní skriptování. Teprve potom můžete z aplikace Internet Explorer získat přístup k webu pro správu služby WSUS.

#### Problém 4: Služba IIS bude během instalace služby WSUS restartována

Instalační program služby Windows Server Update Services restartuje službu IIS bez upozornění. To může mít vliv na stávající weby v organizaci.

#### Problém 5: Změna přístupu bodů pro správu (MP) do virtuálního adresáře služby WSUS nebo SMS

Ve výchozím nastavení je u virtuálního adresáře obsahu pro službu Windows Server Update Services nastaven anonymní přístup. Jestliže toto nastavení změníte tak, aby bylo vyžadováno ověření, dojde při ověřování klientů k chybám a bude jim odepřen přístup ke stahování aktualizací. Jedná se o známý problém, kdy knihovna Winhttp.dll používá chybný kontext ověřování, pokud je požadováno implicitní ověřování, takže výzva k ověření se nezdaří. Abyste tomuto problému zabránili, musí být body MP serveru WSUS a SMS nastaveny na anonymní přístup do virtuálních adresářů služby IIS.

#### Problém 6: Při instalaci služby WSUS v systému Windows Small Business Server 2003 je třeba změnit výchozí nastavení přístupu k virtuálním kořenovým adresářům služby WSUS tak, aby klienti WSUS sami stahovali aktualizace ze serveru

Server WSUS nainstaluje dva virtuální kořenové adresáře (SelfUpdate a ClientWebService) a některé soubory v domovském adresáři na výchozím webu (na portu 80). Klienti tak mohou sami provádět aktualizaci prostřednictvím výchozího webu. Ve výchozím nastavení je v systému Windows Small Business Server 2003 výchozí web nakonfigurován tak, že kromě serveru odepírá přístup všem ostatním IP adresám nebo místním hostitelům. To znamená, že k virtuálním kořenovým adresářům SelfUpdate a ClientWebService je odepřen přístup, takže klienti nemohou sami provést aktualizaci. Chcete-li klientům udělit přístup, aby mohli sami provádět aktualizaci, proveďte ve virtuálních kořenových adresářích SelfUpdate a ClientWebService výchozího webu následující postup.

1.  Ve virtuálním kořenovém adresáři klepněte na možnost **Vlastnosti**, na položku **Zabezpečení adresáře**, na možnost **Omezení podle adres IP a názvů domén**, a potom klepněte na tlačítko **Upravit**.
2.  Klepněte na možnost **Udělit přístup** a potom na tlačítko **OK**. Zavřete všechny stránky vlastností.

#### Problém 7: Instalace služby WSUS v systému Small Business Server - problémy s integrací

-   Pokud systém Windows Small Business Server 2003 používá pro přístup na Internet proxy server ISA, je třeba v uživatelském rozhraní **Nastavení** zadat ručně následující hodnoty: nastavení proxy serveru, název proxy serveru a port.
-   Používá-li služba ISA Ověřování systému Windows, je třeba zadat ověření proxy serveru přímo v podobě DOMÉNA\\uživatel (uživatel patřící do domény Internet Users).

#### Problém 8: Při přesouvání počítače z jedné skupiny počítačů do jiné může trvat až hodinu, než se počítač zobrazí v nové skupině při prohlížení z konzoly pro správu

Pokud je počítač přiřazen k cílové skupině poprvé, jsou data v tomto počítači upravena informacemi o skupině. Tato data jsou aktualizována pravidelně nebo každou hodinu. Při přesouvání počítače z jedné skupiny do jiné proto může aktualizace informací v klientovi a zobrazení těchto změněných informací v konzole pro správu služby WSUS trvat až hodinu.

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

Příčinou je skutečnost, že rozhraní .NET Framework 1.0 je registrováno u služby IIS a server WSUS vyžaduje rozhraní .NET Framework 1.1. Tento problém vyřešíte tak, že otevřete soubor aspnet\_regiis.exe a spustíte následující příkazy, kde *id\_webu* je hodnota obsažená v následujícím klíči registru:

HKLM\\Software\\Microsoft\\WindowsUpdateServices\\Server\\Setup\\IISTargetWebsiteIndex

-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*id\_webu*&gt;\\ROOT\\ReportingWebService
-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*id\_webu*&gt;\\ROOT\\ClientWebService
-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*id\_webu*&gt;\\ROOT\\SimpleAuthWebService
-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*id\_webu*&gt;\\ROOT\\WSUSAdmin
-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*id\_webu*&gt;\\ROOT\\AdministrationWebService
-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*id\_webu*&gt;\\ROOT\\ServrSyncWebService
-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*id\_webu*&gt;\\ROOT\\DssAuthWebService
-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*id\_webu*&gt;\\ROOT\\Content

#### Problém 12: Omezení vzdálené instalace serveru SQL

Služba WSUS nabízí omezenou podporu databázového softwaru, který běží v jiném počítači než zbývající část aplikace WSUS.

-   Počítač se systémem Windows 2000 Server nelze použít jako počítač front-end ve vzdálené dvojici SQL.
-   Server nakonfigurovaný jako řadič domény nelze použít jako počítač front-end ani back-end vzdálené dvojice SQL.
-   Služby WMSDE nebo MSDE nelze použít pro databázový software v počítači back-end.
-   Nastavení vzdáleného serveru SQL Server (pro databázi služby WSUS) se nezdaří, pokud je na vzdáleném serveru nainstalována Terminálová služba, která je spuštěna v aplikačním režimu. Při instalaci serveru SQL Server na server Terminálové služby je třeba provést následující kroky:
    1.  Před spuštěním instalačního programu otevřete příkazový řádek a zadejte příkaz: **change user /install**
    2.  Spusťte instalaci serveru SQL Server.
    3.  Po spuštění instalačního programu zadejte na příkazovém řádku příkaz: **change user /execute**
-   Aby bylo možné nastavit databázi služby WSUS na vzdáleném serveru SQL Server, musíte být členem místní skupiny zabezpečení Administrators v počítači front-end i back-end.
-   Další informace o problémech se vzdáleným serverem SQL získáte v Příloze C: Vzdálený server SQL v článku [Nasazení služby Microsoft Windows Server Update Services](http://go.microsoft.com/fwlink/?linkid=41777).

#### Problém 13: Server repliky pro příjem dat může mít méně schválení než nadřazený server pro odesílání dat

Server repliky pro příjem dat může mít méně schválení než nadřazený server pro odesílání dat. Důvodem je skutečnost, že schválení instalace nepřecházejí na server pro příjem dat, dokud neskončí stahování obsahu na serveru pro odesílání dat.

#### Problém 14: Pokud se synchronizace nezdaří, opakujte ji

Jestliže se synchronizace nezdaří, zobrazí se pravděpodobně chybová zpráva. Pokud k tomu dojde, měli byste se nejprve znovu pokusit o synchronizaci.

#### Problém 15: Při pokusu o přístup do konzoly pro správu služby WSUS se zobrazí chybová zpráva System.IO.FileNotFoundException

Pokud se zobrazí následující chybová zpráva, bude zřejmě nutné nastavit oprávnění u síťové služby nebo účtů služby ASP.NET:

System.IO.FileNotFoundException: Nebyl nalezen soubor nebo sestavení s názvem *xxxxxx*.dll nebo některé z jeho závislostí,

kde *xxxxxx* je náhodný název.

Chcete-li tento problém vyřešit v operačním systému Windows Server 2003, udělte účtu síťové služby oprávnění pro čtení a zápis ke složce %systemroot%\\Temp. V systému Windows 2000 Server udělte účtu ASP.NET oprávnění pro čtení a zápis ke složce %systemroot%\\Temp.

#### Problém 16: Aktualizace zabezpečení serveru SQL MS03-031 (KB815495)

Může se zdát, že je tato aktualizace nainstalována na serveru WSUS, přestože instalace u klienta se ve skutečnosti nezdařila. To může způsobit, že balíček bude klientovi znovu nabídnut. Tento problém můžete obejít zrušením schválení aktualizace na serveru.

#### Problém 17: Nastavení služby IIS se během upgradu předprodejní verze ztratí

Pokud nainstalujete předprodejní verzi služby WSUS na server s předchozí verzí služby WSUS (například RC), odinstaluje předprodejní verze služby WSUS dřívější verzi, a pak nainstaluje verzi novou. To znamená, že virtuální kořenové adresáře a soubory spojené se službou WSUS ve službě IIS budou odstraněny.

Pokud jste službu WSUS nainstalovali na výchozím webu, ztratíte veškerá nastavení související se službou WSUS, která jste vytvořili ve virtuálních kořenových adresářích služby WSUS. Jestliže jste například nakonfigurovali virtuální kořenové adresáře služby WSUS pro protokol SSL za účelem zabezpečení služby WSUS, bude je nutné po instalaci předprodejní verze služby WSUS znovu nakonfigurovat. Poznámka: Obdržíte upozornění konzoly služby WSUS, že protokol SSL není povolen.

Pokud jste službu WSUS nainstalovali na jiný než výchozí web, všechna další nastavení na úrovni webu WSUS se ztratí.

#### Problém 18: Použití hlavičky hostitele

Chcete-li u služby IIS přiřadit výchozímu webu (web služby WSUS) hodnoty hlavičky hostitele, je třeba do seznamu IP adres pro výchozí web přidat hodnotu Všechny nepřiřazené nebo přiřazenou IP adresu bez hodnoty hlavičky hostitele. Je vhodné přidat je také na web, který není výchozí.

**Varování**: Uvedený krok může způsobit narušení funkčnosti serverů Windows® SharePoint® Services a Exchange.

#### Problém 19: Do zóny webového obsahu Důvěryhodné servery a Místní intranet počítačů, v nichž je povoleno posílení zabezpečení aplikace Internet Explorer, musí být přidána adresa URL konzoly služby WSUS

Pokud je v počítači povoleno posílení zabezpečení aplikace Internet Explorer (známé také jako součást Rozšířené nastavení zabezpečení aplikace Internet Explorer v systému Microsoft Windows Server 2003) a nepřidáte konzolu služby WSUS do zón webového obsahu Důvěryhodné servery a Místní intranet, budete vyzváni k zadání pověření uživatele při každém otevření stránky v konzole služby WSUS.

Přidání konzoly služby WSUS do zón webového obsahu **Místní intranet** a **Důvěryhodné servery**:

1.  Otevřete nabídku **Možnosti Internetu** (například klepnutím na tlačítko **Start**, položku **Ovládací panely** a panel **Možnosti Internetu**).
2.  Na kartě **Zabezpečení** klepněte na ikonu **Místní intranet**, potom klepněte na tlačítko **Servery**, na tlačítko **Upřesnit**, přidejte adresu URL (http://*Název\_serveru\_WSUS*/WSUSAdmin) a klepněte na tlačítko **OK**.
3.  Klepněte na ikonu **Důvěryhodné servery**, na tlačítko **Servery**, přidejte adresu URL konzoly služby WSUS, klepněte na tlačítko **OK** a dalším klepnutím na tlačítko **OK** zavřete dialogové okno **Možnosti Internetu**.

#### Problém 20: Upgrade z verze Release Candidate služby WSUS se nezdaří

Upgrade z verze Release Candidate služby WSUS by mohl selhat z důvodu potíží s automatickou aktualizací stromové struktury. K tomu může dojít v případě automatické aktualizace více klientů ve stejnou dobu, kdy se pokusíte provést upgrade.

Řešení tohoto problému:

1.  Odpojte server WSUS od sítě, aby se k ní nemohli připojovat klienti.
2.  Na příkazový řádek zadejte příkaz: **iisrestart /reset** a potom stiskněte klávesu ENTER.
3.  Spusťte upgrade.

#### Problém 21: Některá schválení ze služby SUS 1.0 se nepodaří migrovat na server služby WSUS.

Při migraci ze služby SUS 1.0 na službu WSUS se nepodaří některá schválení na serveru SUS 1.0 migrovat na server služby WSUS. Důvodem je to, že řada aktualizací, které byly k dispozici pro službu SUS 1.0, již není k dispozici pro službu WSUS. Navíc vzhledem k tomu, že služba WSUS podporuje více aktualizací než služba SUS, je možné, že po dokončení migrace mohou na vašem serveru WSUS zůstat důležité aktualizace, které nebyly schváleny.

Společnost Microsoft doporučuje projít si po migraci ze služby SUS 1.0 všechny neschválené aktualizace na serveru WSUS.

Další informace o migraci ze služby SUS 1.0 na službu WSUS naleznete v článku [Step-by-Step Guide to Migrating from Software Update Services to Windows Server Update Services](http://go.microsoft.com/fwlink/?linkid=48042) (Podrobný průvodce migrací ze služby SUS na službu WSUS) na adrese http://go.microsoft.com/fwlink/?LinkId=48042.

#### Problém 22: Tuto položku registru opravte před upgradem na službu WSUS 2.0 Service Pack 1 (pokud jste migrovali službu WMSDE na SQL Server).

Pokud budete chtít upgradovat službu WSUS 2.0 pomocí aktualizace Service Pack 1 a migrovali jste instalaci služby WMSDE na SQL Server (vzdálený nebo místní), změňte následující položku registru:

HKLM\\Software\\Microsoft\\Update Services\\Server\\Setup\\WmsdeInstalled

Hodnotu je třeba změnit z 1 na 0.

#### Problém 23: Migrace vzdálené instalace SQL na službu WSUS 2.0 Service Pack 1

Při migraci na službu WSUS 2.0 Service Pack 1 se vzdálenou konfigurací SQL proveďte následující kroky:

1) Spusťte instalační balíček na serveru front-end bez přepínačů a zvolte upgrade.

2) Spusťte instalační balíček na serveru back-end bez přepínačů a zvolte upgrade.

#### Autorská práva

Informace obsažené v tomto dokumentu představují aktuální názor společnosti Microsoft na problémy známé k datu vydání. Protože společnost Microsoft musí reagovat na měnící se podmínky trhu, nelze je považovat za závazek ze strany společnosti Microsoft, přičemž společnost Microsoft nemůže zaručit správnost informací zveřejněných po datu vydání.

Tento dokument je určen pouze pro informační účely. SPOLEČNOST MICROSOFT NEPOSKYTUJE NA INFORMACE UVEDENÉ V TOMTO DOKUMENTU ŽÁDNÉ ZÁRUKY, AŤ UŽ VÝSLOVNĚ UVEDENÉ, MLČKY PŘEDPOKLÁDANÉ NEBO VYPLÝVAJÍCÍ ZE ZÁKONA.

Za splnění veškerých požadavků všech příslušných zákonů na ochranu autorských práv odpovídá uživatel. Bez předchozího písemného svolení společnosti Microsoft nesmí být žádná část tohoto dokumentu za žádným účelem reprodukována, ukládána, zaváděna do vyhledávácích systémů nebo přenášena jakoukoli formou (elektronicky, mechanicky, pomocí fotokopií, záznamů nebo jinak). Autorská práva nejsou tímto ustanovením dotčena.

Společnost Microsoft může vlastnit patenty, patentové přihlášky, chráněné známky, autorská práva nebo jiná práva k duševnímu vlastnictví týkající se předmětu tohoto dokumentu. Není-li v písemné licenční smlouvě společnosti Microsoft výslovně uvedeno jinak, nejsou předáním tohoto dokumentu poskytnuty žádné licence na takové patenty, chráněné známky, autorská práva nebo jiné duševní vlastnictví.

Pokud není uvedeno jinak, jsou názvy společností, organizací, produktů, názvy domén, e-mailové adresy, loga, osoby, místa či události použité v ukázkách smyšlené a nemůže být vyvozováno žádné jejich spojení se skutečnou společností, organizací, produktem, názvem domény, e-mailovou adresou, logem, osobou, místem či událostí.

© 2005 Microsoft Corporation. Všechna práva vyhrazena.

Microsoft, SQL Server, Windows a Windows Server jsou registrované ochranné známky nebo ochranné známky společnosti Microsoft Corporation ve Spojených státech amerických a v dalších zemích.

Názvy skutečných společností a produktů, uvedené v tomto dokumentu, mohou být ochrannými známkami jejich příslušných vlastníků.
