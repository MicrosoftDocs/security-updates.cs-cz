---
TOCTitle: Nastavení testovacího prostředí
Title: Nastavení testovacího prostředí
ms:assetid: 'cdd96b05-49e2-4b6f-bfae-40b5c028ec66'
ms:contentKeyID: 18113437
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747673(v=WS.10)'
---

Nastavení testovacího prostředí
===============================

Služba RMS je integrována v rámci existující infrastruktury služby Active Directory a databázových serverů (například s nainstalovaným serverem Microsoft SQL Server™ 2000). Vzhledem k důležitosti těchto podpůrných součástí byste měli službu RMS důkladně otestovat v izolovaném testovacím prostředí a teprve potom ji nasadit v organizaci. K tomu je nutné, abyste v testovacím prostředí nainstalovali samostatnou instalaci služby Active Directory a databázového serveru.

Začněte s nejzákladnější konfigurací serveru RMS v doménové struktuře s databázovým serverem a klientem. Jakmile se se službou RMS seznámíte, můžete konfiguraci rozšiřovat tak, aby lépe odpovídala topologii, kterou budete nasazovat v provozním prostředí organizace, a to přidáním dalších požadovaných doménových struktur a externího přístupu. Přestože testovací prostředí pravděpodobně nebude zahrnovat všechny konfigurace redundance dat a seskupení webů plánu nasazení v organizaci, měl by jeho součástí být aspoň jeden server pro jednotlivé podpůrné součásti, které bude nutné nasadit.

Následující seznam popisuje možnou minimální konfiguraci pro testovací prostředí, pomocí které lze testovat základní konfiguraci pro službu RMS:

-   Řadič domény se systémem Windows 2000 Server s aktualizací Service Pack 3 (SP3) nebo vyšší a také s nainstalovaným serverem SQL Server 2000 s aktualizací SP3a. SQL Server je hostitelem konfigurační databáze, databáze protokolování a databáze adresářových služeb služby RMS. Službu RMS lze používat buď se součástí Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) verze A, nebo se součástí SQL Server, pokud bude databáze uložena na stejném serveru jako služba RMS. Pokud budete používat podporu databází ze vzdáleného serveru, je nutné zvolit systém SQL Server. Součást MSDE 2000 MSDE 2000 lze stáhnout z webu společnosti Microsoft.

> [!NOTE]
> Minimálním požadavkem na řadič domény je systém Windows 2000 Server s aktualizací Service Pack 3 (SP3). Doporučujeme však používat systém Windows Server 2003, a to kvůli vylepšením v oblasti rozšiřování skupin služby Active Directory. Součást MSDE 2000 je vhodné používat pouze pro podporu databází služby RMS v testovacích prostředích, protože tato součást nepodporuje žádná síťová rozhraní. V podmínkách používání součásti MSDE 2000 je navíc uvedeno, že pro obsluhu databáze MSDE 2000 nelze použít klientské nástroje serveru SQL Server. Vzhledem k tomuto omezení by nebylo možné zobrazit informace obsažené v protokolech a změnit data uložená v konfigurační databázi. 

-   Je nainstalován server kořenové certifikace se systémem Windows Server 2003, na kterém je nainstalována a zajištěna služba RMS. V případě potřeby můžete v průběhu testování přidat další servery k vytvoření clusteru kořenové certifikace.
-   Klientský počítač se systémem Windows XP Professional, klient RMS a aplikace s podporou služby RMS.
-   Uživatelské účty, které mají atributy e-mailové adresy v adresáři služby Active Directory.

Informace o instalaci a konfiguraci základní infrastruktury služby RMS a také o tom, jak aplikovat požadavky na infrastrukturu do provozního prostředí, získáte v tomto tématu později v části [Nastavení základní infrastruktury](https://technet.microsoft.com/3a0a3a47-e755-4455-bb22-0e05053723e4).
