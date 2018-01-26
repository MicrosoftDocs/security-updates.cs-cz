---
TOCTitle: 'Nejčastější dotazy týkající se služby RMS: Nasazení'
Title: 'Nejčastější dotazy týkající se služby RMS: Nasazení'
ms:assetid: '5559ae65-77ae-4e0b-bfd8-3512409ed29b'
ms:contentKeyID: 18113280
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc720274(v=WS.10)'
---

Nejčastější dotazy týkající se služby RMS: Nasazení
===================================================

Nejčastější dotazy týkající se nasazení služby RMS
--------------------------------------------------

-   [Jestliže jsou objekty zabezpečení použité ve službě RMS členy globálního seznamu adres, existuje jakákoli závislost na verzi produktu Exchange?](#bkmk_20)
-   [Jakou roli ve službě RMS splňuje SQL Server?](#bkmk_21)
-   [Vyžaduje používání služby RMS připojení počítače uživatele ke stejné doméně jako kořenový cluster služby RMS?](#bkmk_22)
-   [Pokud chce zákazník umístit server RMS do hraniční sítě, které porty musí být otevřeny u brány firewall vystavené Internetu a u brány vystavené intranetu pro komunikaci se službou RMS?](#bkmk_23)
-   [Jakým způsobem se provádí zápis podřízených serverů v clusteru vyhrazeném pro správu licencí a je nutné provést nějaký krok v klientech, aby uvedený cluster zjistili?](#bkmk_24)
-   [Jaké jsou výhody použití clusteru vyhrazeného pro správu licencí?](#bkmk_25)
-   [Jak je možné zcela odstranit instalaci služby RMS?](#bkmk_26)
-   [Je nutné po odinstalaci klienta RMS pomocí panelu Přidat nebo odebrat programy odebrat ještě nějaké další soubory?](#bkmk_27)
-   [Pracuje služba RMS se systémem souborů FAT?](#bkmk_28)
-   [Jaká hardwarová konfigurace se obvykle doporučuje pro databázový server používaný službou RMS?](#bkmk_29)
-   [Jak ovlivňuje využívání globálního katalogu službou RMS pro rozšíření skupin výkon serveru tohoto katalogu?](#bkmk_30)
-   [Vyžaduje služba RMS nějaké změny schématu ve službě Active Directory?](#bkmk_31)
-   [Bude spojovací bod služby automaticky replikován mezi různými řadiči domény, v níž je nainstalován cluster služby RMS?](#bkmk_32)
-   [Jestliže uživatelé nemají práva umožňující správu příslušných počítačů, jak lze nainstalovat a nakonfigurovat klienta RMS?](#bkmk_33)
-   [Co je škálovatelnost služby RMS?](#bkmk_35)
-   [Podporuje služba RMS moduly hardwarového zabezpečení za účelem zabezpečení klíčů RMS v hardwaru?](#bkmk_36)

<span id="BKMK_20"></span>
#### Jestliže jsou objekty zabezpečení použité ve službě RMS členy globálního seznamu adres, existuje jakákoli závislost na verzi produktu Exchange?

Služba RMS je závislá na službě Active Directory, ale nikoli na produktu Exchange. Server Exchange 5.5 však udržuje svůj vlastní adresář a službu Active Directory nepoužívá. Přesvědčte se, zda je všem objektům uživatelů a skupin ve službě Active Directory přiřazen platný e-mailový atribut, který obsahuje plně kvalifikovaný název domény. Uvedený krok je proveden automaticky v případě, že používáte server Exchange 2000 nebo vyšší.

<span id="BKMK_21"></span>
#### Jakou roli ve službě RMS splňuje SQL Server?

Služba RMS používá databázi k ukládání dat o konfiguraci všech služeb, informací o objektech zabezpečení v systému a veškerých dat protokolování a k ukládání výsledků vyhledávání během rozšíření seznamů služby Active Directory a distribučních seznamů do mezipaměti. Služba RMS byla řádně testována pro použití se servery SQL Server 2000 a SQL Server 2005.

<span id="BKMK_22"></span>
#### Vyžaduje používání služby RMS připojení počítače uživatele ke stejné doméně jako server RMS?

Počítač uživatele nemusí být členem stejné domény jako cluster služby RMS, ale je nutné, aby mohl uvedený cluster vyhledat. Nejsnadnějším způsobem vyhledání clusteru služby RMS klientským počítačem představuje hledání služby Active Directory prostřednictvím spojovacího bodu služby. V nastavení registru klienta však může být také zadána možnost vyhledání clusteru služby RMS bez hledání služby Active Directory. Přesné nastavení registru závisí na dané aplikaci s podporou služby RMS.

<span id="BKMK_23"></span>
#### Pokud chce zákazník umístit server RMS do hraniční sítě, které porty musí být otevřeny u brány firewall vystavené Internetu a u brány vystavené intranetu pro komunikaci se službou RMS?

Interní uživatelé potřebují získat přístup k serverům RMS, které vydávají certifikáty účtů práv a licence k použití. Podle toho, zda je server RMS nakonfigurován na použití protokolu SSL, naslouchá ve výchozím nastavení na portu protokolu HTTP (port TCP 80) nebo HTTPS (port TCP 443), takže u brány firewall vystavené Internetu je nutné otevřít tyto porty. Bude nutné otevřít další porty u brány firewall vystavené intranetu využívané členskými servery v doméně.

<span id="BKMK_24"></span>
#### Jakým způsobem se provádí zápis podřízených serverů v clusteru vyhrazeném pro správu licencí a je nutné provést nějaký krok v klientech, aby uvedený cluster zjistili?

První vytvořený server RMS v kořenovém clusteru podniku získá serverový certifikát pro vystavování licencí od služby Microsoft Enrollment Service. Jakmile je nainstalován a zajištěn další server RMS, můžete jej připojit do kořenového clusteru nebo zapsat jako server v podřízeném clusteru vyhrazeném pro správu licencí. Jestliže se jej rozhodnete zapsat jako server v podřízeném clusteru vyhrazeném pro správu licencí, odešle kořenovému clusteru služby RMS požadavek na zápis. Aplikace s podporou služby RMS určí umístění, kde bude klientská aplikace hledat daný cluster vyhrazený pro správu licencí. Příkladem aplikace s podporou služby RMS, která ve výchozím nastavení prohledává kořenový cluster, je sada Office 2003. Toto chování lze přepsat v nastavení registru tak, aby aplikace hledala nový podřízený cluster vyhrazený pro správu licencí.

<span id="BKMK_25"></span>
#### Jaké jsou výhody použití podřízeného clusteru vyhrazeného pro správu licencí?

Jednou výhodou je izolace různých oddělení v rámci organizace. Jestliže v rámci clusteru služby RMS není vytvořena důvěryhodná doména publikování, mohou obsah využívat pouze uživatelé s přístupem k danému serveru správy licencí. Tímto způsobem by mohlo právní oddělení znemožnit všem ostatním oddělením čtení svých e-mailů šifrovaných službou RMS. V clusteru vyhrazeném pro správu licencí lze navíc nastavit několik možností, jako jsou šablony práv, protokolování, členství ve skupině Super Users a zásady vyloučení.

<span id="BKMK_26"></span>
#### Jak je možné zcela odstranit instalaci služby RMS?

Chcete-li zcela odstranit instalaci služby RMS, proveďte následující postup.

**Odstranění instalace služby RMS**
1.  Na webu správy služby RMS odeberte spojovací bod služby pro cluster služby RMS.

2.  Na stránce **Globální správa** zrušte zajištění služby RMS na požadovaném serveru klepnutím na možnost **Odebrat službu RMS z tohoto webu**. Nejprve byste měli zrušit zajištění všech serverů s dílčím zápisem v clusterech vyhrazených pro správu licencí, a potom teprve zajištění serverů kořenového clusteru.

3.  V **Ovládacích panelech** klepněte na panel **Přidat nebo odebrat programy** a odeberte **Službu správy přístupových práv**.

4.  Na databázovém serveru odeberte všechny zbývající databáze služby RMS.

5.  Odeberte účet služby RMS ze seznamu autorizovaných přihlášení na databázových serverech, a pak tento účet odeberte ze samotné služby Active Directory.

6.  Jestliže klienti RMS používají systém Windows XP a Windows 2000, odeberte je z klientských počítačů.

> [!IMPORTANT]
> Po dokončení tohoto postupu již nebudete moci otevírat obsah chráněný právy. Pokud jste pomocí služby RMS zabezpečili cenná data, vyřaďte před odstraněním instalace služby RMS nejprve tuto službu z provozu. 

<span id="BKMK_27"></span>
#### Je nutné po odinstalaci klienta RMS pomocí panelu Přidat nebo odebrat programy odebrat ještě nějaké další soubory?

Přestože to není nutné, můžete odstranit bezpečnostní modul ze složky %systemroot%\\system32.

<span id="BKMK_28"></span>
#### Pracuje služba RMS se systémem souborů FAT?

Ano. Ačkoli se doporučuje systém souborů NTFS, pracuje služba RMS i v počítači se systémem FAT.

<span id="BKMK_29"></span>
#### Jaká hardwarová konfigurace se obvykle doporučuje pro databázový server používaný službou RMS?

Velikost databáze protokolování se zvětšuje rychle, zvláště v prostředí, kde se služba RMS používá často. Jestliže chcete jako databázový server použít SQL Server, měli byste zvážit SQL Server 2000 Enterprise Edition nebo SQL Server 2005 Enterprise Edition v systému Windows 2000 Advanced Server nebo Windows Server 2003 Enterprise Edition nakonfigurovaný v clusteru s nastavením aktivního úsporného režimu. V tomto případě se doporučuje následující konfigurace: disky RAID-1 pro protokolování, disky RAID-5 pro data a nejméně 512 MB paměti RAM. Minimální doporučený procesor této konfigurace je Pentium III pracující na frekvenci 1,4 GHz. U vyhrazených databázových serverů není vyžadováno více procesorů.

<span id="BKMK_30"></span>
#### Jak ovlivňuje využívání globálního katalogu službou RMS pro rozšíření skupin výkon serveru tohoto katalogu?

Server RMS ukládá do mezipaměti všechny seznamy rozšíření skupin, což by na serveru globálního katalogu nemělo způsobit žádné velké zatížení. Časté aktualizace členství ve skupinách zvyšuje závislost na serveru globálního katalogu, přestože časový limit pro získání seznamů nových skupin lze nastavit prostřednictvím registru. Výkon sníží časté rozšiřování velkých skupin. Další informace získáte v části Změna nastavení mezipaměti služby Active Directory tématu RMS: Provoz v této sadě dokumentace.

<span id="BKMK_31"></span>
#### Vyžaduje služba RMS nějaké změny schématu ve službě Active Directory?

Aby mohla služba RMS úspěšně rozšířit členství ve skupině určené licencí k publikování přes hranice doménových struktur, musí v místní doménové struktuře Active Directory existovat kontaktní objekt reprezentující skupiny obsažené ve vzdálených doménových strukturách. Služba RMS může zadávat dotazy na atributy kontaktního objektu a zjistit tak, které objekty reprezentují skupinu obsaženou v jiné doménové struktuře.

Pro uvedený krok služby RMS vyžaduje služba Active Directory atribut schématu msExchOriginatingForest serveru Exchange Server 2003 nebo vyšší. Tento atribut je ve výchozím nastavení nainstalován do schématu služby Active Directory, jestliže je v doménové struktuře spuštěn jeden server s produktem Exchange Server 2003. Tento atribut musí obsahovat doménová struktura každého schématu služby Active Directory, které se bude používat v rámci služby RMS. Pokud nepoužíváte produkt Exchange Server 2003, můžete schéma instalovat do struktury služby Active Directory samostatně pomocí sady RMS Administration Toolkit.

<span id="BKMK_32"></span>
#### Bude spojovací bod služby automaticky replikován mezi různými řadiči domény, v níž je nainstalován server RMS?

Po zajištění je nutné první server RMS v doménové struktuře zaregistrovat ve službě Active Directory pomocí doménového účtu s dostatečnými oprávněními pro vytvoření objektu kontejneru pod kontejnerem Služby v kontejneru Konfigurace služby Active Directory. Příkladem účtu s požadovanými oprávněními je integrovaná skupina zabezpečení Enterprise Admins. Při uvedeném kroku je vytvořen spojovací bod služby. Vzhledem k tomu, že byly dané kroky provedeny v kontejneru Služby, replikuje služba Active Directory příslušné informace ve všech řadičích domény této doménové struktury.

<span id="BKMK_33"></span>
#### Jestliže uživatelé nemají práva umožňující správu příslušných počítačů, jak lze nainstalovat a nakonfigurovat klienta RMS?

Klient RMS je souborem Instalační služby systému Windows a lze jej distribuovat prostřednictvím infrastruktury distribuce softwaru, jako je například Systems Management Server 2003. Klienta RMS je zároveň možné distribuovat pomocí objektu zásad skupiny, který používá účet služby s právy pro správu. Pokud klient RMS používá systém Windows Vista, není jej třeba instalovat samostatně, protože je integrován do operačního systému.

<span id="BKMK_35"></span>
#### Co je škálovatelnost služby RMS?

Služba RMS je samostatná webová služba, u níž lze vytvářet clustery a vyrovnávat zatížení jako u každého jiného webu nebo služby. Výkon služby RMS závisí především na možnostech procesoru, takže přidáním procesoru můžete výkon zvýšit.

<span id="BKMK_36"></span>
#### Podporuje služba RMS moduly hardwarového zabezpečení za účelem zabezpečení klíčů RMS v hardwaru?

Ano, služba RMS pracuje s moduly hardwarového zabezpečení kompatibilními s rozhraním CAPI, jako je například modul nCipher.
