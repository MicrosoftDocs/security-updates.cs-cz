---
TOCTitle: Instalace řadiče domény a databázového serveru
Title: Instalace řadiče domény a databázového serveru
ms:assetid: 'd20f8305-9f9e-4760-bfbf-82824db60d1f'
ms:contentKeyID: 18113444
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747681(v=WS.10)'
---

Instalace řadiče domény a databázového serveru
==============================================

Před instalací serveru kořenové certifikace nebo serveru správy licencí zkontrolujte, zda je implementována správná doménová a databázová podpora zajištěná službou Active Directory a databázovým serverem, například SQL Server 2000 s aktualizací Service Pack 3 (SP3) nebo Microsoft® SQL Server 2000 Desktop Engine (MSDE 2000) verze A. Přestože je možné, že v provozním prostředí již budou požadované součásti spuštěny, nedoporučujeme používat provozní prostředí k testování.

Pomocí následujících kroků nastavíte řadič domény a databázový server v jednom počítači v izolované síti pro účely testování na serveru.

> [!NOTE]
> V tomto příkladu je databázový server na řadiči domény. V provozním prostředí se obecně nedoporučuje používat řadič domény jako hostitele dalších součástí. Služba Active Directory a databázový server jsou v tomto příkladu nainstalovány ve stejném počítači, aby bylo možné nainstalovat celou infrastrukturu do minimálního počtu počítačů. 

Pokud se rozhodnete jako databázový server používat součást MSDE 2000, měli byste vědět, že nepodporuje žádná síťová rozhraní a že v podmínkách používání součásti MSDE 2000 je uvedeno, že pro obsluhu databáze MSDE 2000 nelze použít klientské nástroje serveru SQL Server. Vzhledem k tomuto omezení by nebylo možné zobrazit informace obsažené v protokolech a změnit data uložená v konfigurační databázi. Doporučujeme proto součást MSDE 2000 používat pouze pro podporu databází služby RMS v testovacích prostředích.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Součást infrastruktury</th>
<th style="border:1px solid black;" >Kroky instalace řadiče domény a databázového serveru</th>
<th style="border:1px solid black;" >Poznámky pro nasazení v provozním prostředí</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Operační systém</td>
<td style="border:1px solid black;">Do počítače, který splňuje požadavky na hardware služby RMS, ale není ještě připojen k síti, nainstalujte systém Windows 2000 Server s aktualizací SP3 či vyšší nebo systém Windows Server 2003. Diskový oddíl naformátujte systémem souborů NTFS.</td>
<td style="border:1px solid black;">Doporučujeme vždy nainstalovat nejnovější sadu Service Pack a další aktualizace. Používejte oddíly formátované pro systém souborů NTFS.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Síťové připojení</td>
<td style="border:1px solid black;">Vytvořte připojení k síti, které zajišťuje připojení k Internetu, ale které je izolované od provozního prostředí.</td>
<td style="border:1px solid black;">Připojení k Internetu by mělo být zabezpečeno bránou firewall.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Adresa IP</td>
<td style="border:1px solid black;">Přiřaďte tomuto počítači statickou adresu IP.</td>
<td style="border:1px solid black;">Pro servery používejte zásadně statické adresy IP.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Služba Active Directory</td>
<td style="border:1px solid black;">Přihlaste se jako místní správce.</td>
<td style="border:1px solid black;"> </td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Klepněte na tlačítko <strong>Start</strong>, na příkaz <strong>Spustit</strong>, do pole <strong>Otevřít</strong> zadejte příkaz <code>dcpromo</code> a potom klepněte na tlačítko <strong>OK</strong>.</td>
<td style="border:1px solid black;"> </td>
</tr>
<tr class="even">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Pomocí spuštěného Průvodce instalací služby Active Directory vytvořte novou doménu v nové doménové struktuře. Ponechejte zvolené výchozí nastavení, kromě následujících možností:
Zadejte název domény, například contoso.com.
Nechte průvodce konfigurovat v počítači službu DNS.
Pokud je na všech řadičích domény spuštěn systém Windows 2000 nebo vyšší, vyberte možnost <strong>Oprávnění kompatibilní pouze s operačními systémy řady Windows 2000 Server nebo Windows Server 2003</strong>.
Nastavte silné heslo pro místního správce.</td>
<td style="border:1px solid black;">Pokud je nutné v nových doménách implementovat službu RMS, nastavte je v adresáři služby Active Directory.
U všech účtů používejte vždy silná hesla.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Po zobrazení příslušné výzvy restartujte počítač.</td>
<td style="border:1px solid black;"> </td>
</tr>
<tr class="even">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Ověřte funkční úroveň tak, že otevřete modul snap-in <strong>Uživatelé a počítače služby Active Directory</strong>, klepnete pravým tlačítkem myši na název domény, klepnete na příkaz <strong>Vlastnosti</strong> a zkontrolujete nastavení uvedené v poli <strong>Operační režim domény</strong>. Pokud se v síti nenacházejí žádné řadiče domény starší než řadiče se systémem Windows 2000, přepněte doménu do <strong>nativního režimu</strong> klepnutím na tlačítko <strong>Změnit režim</strong>.
Poznámka: V systému Windows Server 2003 je nastavení <strong>režimu domény</strong> nahrazeno nastavením <strong>úrovně funkčnosti domény</strong>.</td>
<td style="border:1px solid black;">Z důvodu optimálního zabezpečení a správy byste neměli pro podporu služby RMS používat kombinovaný režim systému Windows 2000.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Uživatelské účty</td>
<td style="border:1px solid black;">Vytvořte standardní účet uživatele, který se bude používat jako účet služby RMS, například ContosoRMS@contoso.com. Nastavte silné heslo. Nezapomeňte zadat e-mailovou adresu uživatele. Pokud není e-mailová adresa zadána v adresáři služby Active Directory, nebude moci uživatel získat licence a certifikáty ze služby RMS.
Poznámka: Jako účet služby RMS nelze použít doménový účet, který byl použit k instalaci služby RMS.</td>
<td style="border:1px solid black;">Účet, který bude využíván jako účet služby RMS, byste měli v adresáři Active Directory vytvořit zvlášť. Uveďte e-mailovou adresu. Tomuto účtu nepřidělujte žádná zvláštní oprávnění.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">SQL Server 2000</td>
<td style="border:1px solid black;">Přihlaste se k serveru, na kterém chcete nainstalovat databázi. V případě, že se jedná o server totožný s řadičem domény, je nutné přihlásit se jako správce domény.</td>
<td style="border:1px solid black;"> </td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Podle pokynů k databázovému softwaru nainstalujte software databázového serveru.</td>
<td style="border:1px solid black;"> </td>
</tr>
<tr class="even">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Pro instalaci databázového serveru použijte doporučené postupy, například:
<ul>
<li>Zadejte název účtu správce databázového systému a název organizace, například Contoso.<br />
<br />
</li>
<li>Nastavte silné heslo správce systému.<br />
<br />
</li>
<li>Používejte metody integrovaného ověřování systému Windows.<br />
<br />
</li>
</ul></td>
<td style="border:1px solid black;">Měli byste používat režim integrovaného ověřování systému Windows. Pokud nelze databázový server v tomto režimu spustit, zeptejte se správce domény a správce databáze, jaké změny bude nutné v instalaci služby RMS provést.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Ověřte, zda je databázová služba zastavena.</td>
<td style="border:1px solid black;"> </td>
</tr>
<tr class="even">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Nainstalujte všechny aktualizace softwaru databázového serveru. Při zobrazení dotazu na zadání hesla použijte stejné heslo, které jste zadali během instalace.</td>
<td style="border:1px solid black;"> </td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Restartujte počítač. Ověřte, zda je databázová služba spuštěna.</td>
<td style="border:1px solid black;"> </td>
</tr>
<tr class="even">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Ověřte, zda mají uživatelské účty v adresáři služby Active Directory platné atributy e-mailové adresy.</td>
<td style="border:1px solid black;"> </td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Zkontrolujte, zda má uživatel domény, který bude spravovat službu RMS (a zajišťovat servery kořenové certifikace a správy licencí) požadovaná oprávnění k databázovému serveru. Pokud jako databázový server používáte SQL Server, můžete pro uživatele používajícího modul snap-in <strong>SQL Server Enterprise Manager</strong> přidat identifikátor přihlášení. V modulu snap-in rozbalte uzel serveru a skupiny server a potom rozbalte položku <strong>Security</strong> (Zabezpečení). Klepněte na položku <strong>Logins</strong> (Přihlášení), přidejte nové přihlášení pro účet domény uživatele, klepněte na kartu <strong>Server Roles</strong> (Role serveru) a potom zaškrtněte políčko <strong>Server Administrators</strong> (Správci serveru).</td>
<td style="border:1px solid black;">Důležité: Všichni uživatelé a všechny skupiny používající službu RMS k získání licencí a publikování obsahu musí mít pro svůj účet v modulu snap-in Uživatelé a počítače služby Active Directory konzoly MMC na kartě <strong>Obecné</strong> ve <strong>vlastnostech</strong> uživatele nakonfigurovánu e-mailovou adresu.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Připojení k Internetu
(nepovinné)</td>
<td style="border:1px solid black;">Ověřte, zda jsou prohlížeč a server (včetně všech konfigurací vyžadujících použití serveru proxy), nastavení TCP/IP a LMHOSTS/HOSTS nakonfigurovány správně na přístup k Internetu. To vyzkoušíte tak, že přejdete na adresu http://uddi.microsoft.com. Pokud je možné tuto stránku otevřít, může se služba RMS připojit ke službě Microsoft Enrollment Services.</td>
<td style="border:1px solid black;">Ověřte přístup k Internetu přechodem na adresu http://uddi.microsoft.com.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Aktualizace softwaru</td>
<td style="border:1px solid black;">Stáhněte a nainstalujte nejnovější aktualizace softwaru nainstalovaného v tomto počítači (včetně nejnovějších aktualizací systému Windows z webu www.microsoft.com).</td>
<td style="border:1px solid black;">Zajistěte, aby byla vždy nainstalována nejnovější aktualizace Service Pack.</td>
</tr>
</tbody>
</table>
  
Po provedení všech předchozích kroků je vše připraveno k počáteční instalaci (včetně instalace základního softwaru) do počítačů, ve kterých bude spuštěna služba RMS.
