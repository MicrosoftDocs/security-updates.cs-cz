---
TOCTitle: Povolení podpory služby RMS pro serverové služby
Title: Povolení podpory služby RMS pro serverové služby
ms:assetid: '6288323c-0638-41b6-bef8-67a7c9433424'
ms:contentKeyID: 18113332
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747593(v=WS.10)'
---

Povolení podpory služby RMS pro serverové služby
================================================

Služba RMS může poskytovat certifikáty účtu práv a licence na používání také serverovým aplikacím s podporou služby RMS. Při konfiguraci serverových služeb byste si měli uvědomit několik věcí:

-   Volitelné seznamy řízení přístupu (DACL) u kanálů RMS používají ve výchozím nastavení nejvíce zabezpečené nastavení. Při používání serverových služeb RMS je třeba seznamy DACL změnit.
-   Pokud je klient RMS nainstalován na serveru se systémem Windows Server 2003 a je povolena Konfigurace rozšířeného zabezpečení aplikace Internet Explorer, je třeba přidat adresu URL clusteru RMS do zóny Důvěryhodné servery aplikace Internet Explorer.
-   Mnoho serverových služeb používá rozšířené funkce adresářových služeb Active Directory, které jsou k dispozici, pouze pokud všechny řadiče domény služby Active Directory používají systém Windows Server 2003. Jestliže používáte některé serverové služby (například Microsoft Office SharePoint Server 2007 nebo Microsoft Exchange Server 2007), doporučujeme používat systém Windows Server 2003 na všech řadičích domény a nastavit úroveň funkčnosti domény i doménové struktury služby Active Directory na úroveň systému Windows Sever 2003.

Výchozí volitelný seznam řízení přístupu (DACL) u kanálu certifikace serverů
----------------------------------------------------------------------------

Některé aplikace, například Microsoft Office SharePoint Server 2007 nebo Microsoft Exchange Server 2007, podporují službu RMS za účelem vyžadování licencí na používání jménem uživatelů. Ve výchozí instalaci služby RMS je seznam DACL kanálu certifikace serverů RMS omezen, což znamená, že aplikace nemůže získat certifikáty a licence pro své uživatele. Pokud je však pro počítače k dispozici aplikace s podporou služby RMS, umožníte jim zapojení do systému RMS konfigurací seznamů řízení přístupu (DACL) u kanálu certifikace serveru RMS.

Serverové aplikace s podporou služby RMS se připojí ke službě certifikace RMS pomocí souboru ServerCertification.asmx.

Jakmile služba RMS tyto soubory vytvoří, jsou seznamy DACL těchto souborů nastaveny tak, že umožňují přístup pouze systémovým procesům. Doporučujeme vytvořit skupinu zabezpečení služby Active Directory pro serverové služby a pak do této skupiny načíst objekty služby Active Directory počítačů, které požadují licence na používání jménem svých uživatelů.

Po vytvoření skupiny můžete změnit seznam DACL pro soubor ServerCertification.asmx tak, aby této skupině poskytoval oprávnění pro čtení & spouštění dané služby. Zároveň je nutné do seznamu DACL přidat skupinu RMS Service Group s oprávněními pro čtení & spouštění.

| ![](images/Cc747593.note(WS.10).gif)Poznámka                                                              |
|----------------------------------------------------------------------------------------------------------------------------------------|
| Pokud cluster obsahuje více serverů RMS, je třeba seznam DACL pro soubor ServerCertification.asmx změnit u každého serveru v clusteru. |

Pro Microsoft Exchange Server 2007 je do této skupiny serverových služeb nutné přidat objekt počítače služby Active Directory pro každý server Exchange předmostí. Pokud tento krok nepovedete, nebude server Exchange předmostí moci požádat o licence jménem uživatelů, kteří obdrželi e-mail.

Pro Office SharePoint Server 2007 je třeba do skupiny serverových služeb přidat objekt počítače služby Active Directory serveru, na němž je Office SharePoint Server 2007 spuštěn. Jestliže je Office SharePoint Server 2007 konfigurován na používání výchozího serveru ve službě Active Directory, je nutné přidat skupinu RMS Service Group a skupinu vytvořenou pro serverové služby do souboru ServiceLocater.asmx a povolit oprávnění ke čtení & spouštění.

| ![](images/Cc747593.Important(WS.10).gif)Důležité informace                                                                                                                                  |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Po změně seznamu DACL pro soubory ServerCertification.asmx a ServiceLocater.asmx. je třeba restartovat Internetovou informační službu (IIS). Tuto službu restartujete spuštěním příkazu **iisreset** na příkazovém řádku. |
