---
TOCTitle: Předpoklady a kontrolní seznamy pro službu RMS
Title: Předpoklady a kontrolní seznamy pro službu RMS
ms:assetid: '836d96ef-d0fd-4935-b595-e8dec19cbb2b'
ms:contentKeyID: 18113346
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747582(v=WS.10)'
---

Předpoklady a kontrolní seznamy pro službu RMS
==============================================

Než začnete instalovat službu RMS, zkontrolujte technologické předpoklady pro její používání. Jednotlivé technologie uvedené v seznamu jsou nedílnou součástí služby RMS a porozumění jejich základním principům je důležité pro úspěšné nasazení této služby. Následující kontrolní seznamy vám umožní vytvořit seznamy úloh a plány pro nasazení a správu služby RMS:

-   [Předpoklady týkající se technologií](#bkmk_9)
-   [Kontrolní seznamy týkající se nasazení služby RMS](#bkmk_10)
-   [Kontrolní seznamy týkající se správy služby RMS](#bkmk_14)

<span id="BKMK_9"></span>
Předpoklady týkající se technologií
-----------------------------------

Tato sada dokumentace obsahuje informace, které vám pomohou pochopit, jakým způsobem funguje služba RMS systému Windows, jak plánovat a realizovat nasazení v organizaci a jak každodenně spravovat svůj systém. Předpokládají se znalosti v následujících oblastech:

-   implementace a správa systému Windows Server 2003,
-   implementace a správa služby Active Directory,
-   nasazení a správa Internetové informační služby 6.0 (IIS) společnosti Microsoft®,
-   správa serveru Microsoft® SQL Server™ 2000,
-   základní pojmy infrastruktury veřejných klíčů (PKI),
-   použití serverů v síti a jejich zabezpečení.

Další informace o těchto tématech získáte v této sadě dokumentace v části Další informační zdroje tématu [Provoz serveru RMS](http://go.microsoft.com/fwlink/?linkid=42495).

<span id="BKMK_10"></span>
Kontrolní seznamy týkající se nasazení služby RMS
-------------------------------------------------

Tato část obsahuje kontrolní seznamy pro následující úlohy nasazení:

-   [Nasazení instalace s jedním serverem](#bkmk_11)
-   [Nasazení clusterů kořenové certifikace a správy licencí](#bkmk_12)
-   [Nasazení služby RMS v doménových strukturách](#bkmk_13)

Další informace o nasazení služby RMS získáte v této sadě dokumentace v části [Nasazení systému služby RMS](http://go.microsoft.com/fwlink/?linkid=42494).

<span id="BKMK_11"></span>
Nasazení instalace s jedním serverem
------------------------------------

Pro nasazení jediného serveru služby RMS použijte následující kontrolní seznam.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Krok</th>
<th style="border:1px solid black;" >Odkaz</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Posouzení informací o plánování a základních pojmů</td>
<td style="border:1px solid black;">Příprava nasazení služby RMS tématu <a href="http://go.microsoft.com/fwlink/?linkid=42494">Nasazení systému služby RMS</a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Kontrola požadavků na systém a ověření, zda je k dispozici veškerý požadovaný hardware a software</td>
<td style="border:1px solid black;">Předpoklady týkající se infrastruktury pro službu RMS tématu <a href="http://go.microsoft.com/fwlink/?linkid=37537">Plánování nasazení služby RMS</a>
Plánování infrastruktury databázového serveru tématu <a href="http://go.microsoft.com/fwlink/?linkid=37537">Plánování nasazení služby RMS</a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Nastavení infrastruktury včetně požadavků na hardware a software, účtů správce a podpory služby SMS nebo Zásad skupiny (podle potřeby)</td>
<td style="border:1px solid black;">Příprava nasazení služby RMS tématu <a href="http://go.microsoft.com/fwlink/?linkid=42494">Nasazení systému služby RMS</a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Instalace a konfigurace služby RMS na serveru</td>
<td style="border:1px solid black;">Nastavení služby certifikace a správy licencí na prvním serveru tématu <a href="http://go.microsoft.com/fwlink/?linkid=42494">Nasazení systému služby RMS</a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Testování implementace</td>
<td style="border:1px solid black;">Nastavení testovacího prostředí tématu <a href="http://go.microsoft.com/fwlink/?linkid=42494">Nasazení systému služby RMS</a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Implementace služby RMS v provozním prostředí</td>
<td style="border:1px solid black;">Definování rozsahu implementace služby RMS tématu <a href="http://go.microsoft.com/fwlink/?linkid=42494">Nasazení systému služby RMS</a></td>
</tr>
</tbody>
</table>
  
<span id="BKMK_12"></span>
Nasazení clusterů kořenové certifikace a správy licencí  
-------------------------------------------------------
  
Pro nasazení clusterů kořenové certifikace a správy licencí použijte následující kontrolní seznam.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Krok</th>
<th style="border:1px solid black;" >Odkaz</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Posouzení informací o plánování a základních pojmů</td>
<td style="border:1px solid black;">Příprava nasazení služby RMS tématu <a href="http://go.microsoft.com/fwlink/?linkid=42494">Nasazení systému služby RMS</a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Kontrola požadavků na systém a ověření, zda je k dispozici veškerý požadovaný hardware a software</td>
<td style="border:1px solid black;">Předpoklady týkající se infrastruktury pro službu RMS tématu <a href="http://go.microsoft.com/fwlink/?linkid=37537">Plánování nasazení služby RMS</a>
Plánování infrastruktury databázového serveru tématu <a href="http://go.microsoft.com/fwlink/?linkid=37537">Plánování nasazení služby RMS</a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Posouzení plánu implementace a seznámení se s topologií a instalovanými komponentami</td>
<td style="border:1px solid black;">Určení topologie služby RMS tématu <a href="http://go.microsoft.com/fwlink/?linkid=37537">Plánování nasazení služby RMS</a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Nastavení infrastruktury včetně požadavků na hardware a software, účtů správce a podpory služby SMS nebo Zásad skupiny (podle potřeby)</td>
<td style="border:1px solid black;">Příprava nasazení služby RMS tématu <a href="http://go.microsoft.com/fwlink/?linkid=42494">Nasazení systému služby RMS</a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Instalace a konfigurace služby RMS na serverech v clusteru kořenové certifikace</td>
<td style="border:1px solid black;">Nastavení služby certifikace a správy licencí na prvním serveru tématu <a href="http://go.microsoft.com/fwlink/?linkid=42494">Nasazení systému služby RMS</a>
Přidání serverů pro podporu certifikace a správy licencí tématu <a href="http://go.microsoft.com/fwlink/?linkid=42494">Nasazení systému služby RMS</a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Instalace a konfigurace služby RMS na serverech v clusterech správy licencí</td>
<td style="border:1px solid black;">Nastavení služby certifikace a správy licencí na prvním serveru tématu <a href="http://go.microsoft.com/fwlink/?linkid=42494">Nasazení systému služby RMS</a>
Přidání serverů pro podporu certifikace a správy licencí tématu <a href="http://go.microsoft.com/fwlink/?linkid=42494">Nasazení systému služby RMS</a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Nastavení vyrovnávání zatížení</td>
<td style="border:1px solid black;">Rozšíření základní infrastruktury na podporu správy clusterů tématu <a href="http://go.microsoft.com/fwlink/?linkid=42494">Nasazení systému služby RMS</a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Testování implementace</td>
<td style="border:1px solid black;">Nastavení testovacího prostředí tématu <a href="http://go.microsoft.com/fwlink/?linkid=42494">Nasazení systému služby RMS</a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Implementace služby RMS v provozním prostředí</td>
<td style="border:1px solid black;">Definování rozsahu implementace služby RMS tématu <a href="http://go.microsoft.com/fwlink/?linkid=42494">Nasazení systému služby RMS</a></td>
</tr>
</tbody>
</table>
  
<span id="BKMK_13"></span>
Nasazení služby RMS v doménových strukturách  
--------------------------------------------
  
Pro nasazení kořenové služby RMS v doménových strukturách použijte následující kontrolní seznam.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Krok</th>
<th style="border:1px solid black;" >Odkaz</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Posouzení informací o plánování a základních pojmů</td>
<td style="border:1px solid black;">Příprava nasazení služby RMS tématu <a href="http://go.microsoft.com/fwlink/?linkid=42494">Nasazení systému služby RMS</a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Konfigurace požadovaných oprávnění na základě modelu důvěryhodnosti</td>
<td style="border:1px solid black;">Nasazení služby RMS v doménových strukturách tématu <a href="http://go.microsoft.com/fwlink/?linkid=42494">Nasazení systému služby RMS</a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Nastavení odpovídajících atributů služby Active Directory pro doménové struktury</td>
<td style="border:1px solid black;">Nasazení služby RMS v doménových strukturách tématu <a href="http://go.microsoft.com/fwlink/?linkid=42494">Nasazení systému služby RMS</a></td>
</tr>
</tbody>
</table>
  
<span id="BKMK_14"></span>
Kontrolní seznamy týkající se správy služby RMS  
-----------------------------------------------
  
Tato část obsahuje kontrolní seznamy pro následující úlohy správy:
  
-   [Implementace šablony zásad práv](#bkmk_15)  
-   [Nasazení nového klienta služby RMS](#bkmk_16)  
-   [Přidání důvěryhodných domén uživatelů](#bkmk_17)  
-   [Přidání důvěryhodných domén publikování](#bkmk_18)
  
Další informace o správě služby RMS získáte v této sadě dokumentace v tématu [Provoz serveru RMS](http://go.microsoft.com/fwlink/?linkid=42495).
  
<span id="BKMK_15"></span>
Implementace šablony zásad práv  
-------------------------------
  
Pro implementaci šablony zásad práv použijte následující kontrolní seznam.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Krok</th>
<th style="border:1px solid black;" >Odkaz</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Nastudování příslušných základních pojmů</td>
<td style="border:1px solid black;">Šablony zásad práv tématu <a href="http://go.microsoft.com/fwlink/?linkid=42496">Technické informace týkající se služby RMS</a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Zadání umístění šablony zásad práv</td>
<td style="border:1px solid black;">Zadání umístění šablon zásad práv tématu <a href="http://go.microsoft.com/fwlink/?linkid=42495">Provoz serveru RMS</a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Vytvoření šablony zásad práv</td>
<td style="border:1px solid black;">Vytvoření a změna šablon zásad práv tématu <a href="http://go.microsoft.com/fwlink/?linkid=42495">Provoz serveru RMS</a>
Přidání šablony zásad práv tématu <a href="http://go.microsoft.com/fwlink/?linkid=42495">Provoz serveru RMS</a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Distribuce šablony zásad práv</td>
<td style="border:1px solid black;">Distribuce šablon zásad práv tématu <a href="http://go.microsoft.com/fwlink/?linkid=42495">Provoz serveru RMS</a></td>
</tr>
</tbody>
</table>
  
<span id="BKMK_16"></span>
Nasazení nového klienta služby RMS  
----------------------------------
  
Pro nasazení nové verze klienta RMS použijte následující kontrolní seznam.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Krok</th>
<th style="border:1px solid black;" >Odkaz</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Nastudování příslušných základních pojmů</td>
<td style="border:1px solid black;">Plánování distribuce klientů tématu <a href="http://go.microsoft.com/fwlink/?linkid=42494">Nasazení systému služby RMS</a>
Vyloučení verzí bezpečnostního modulu tématu <a href="http://go.microsoft.com/fwlink/?linkid=42495">Provoz serveru RMS</a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Chcete-li u všech klientů vynutit upgrade na nejnovější verzi klienta, vylučte zastaralou verzi bezpečnostního modulu.</td>
<td style="border:1px solid black;">Vyloučení verzí bezpečnostního modulu tématu <a href="http://go.microsoft.com/fwlink/?linkid=42495">Provoz serveru RMS</a></td>
</tr>
</tbody>
</table>
  
<span id="BKMK_17"></span>
Přidání důvěryhodných domén uživatelů  
-------------------------------------
  
Pro přidání důvěryhodných domén uživatelů použijte následující kontrolní seznam.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Krok</th>
<th style="border:1px solid black;" >Odkaz</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Nastudování příslušných základních pojmů</td>
<td style="border:1px solid black;">Důvěryhodné domény uživatelů tématu <a href="http://go.microsoft.com/fwlink/?linkid=42496">Technické informace týkající se služby RMS</a>
Přidání a odebrání důvěryhodných domén uživatelů tématu <a href="http://go.microsoft.com/fwlink/?linkid=42495">Provoz serveru RMS</a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Získejte certifikát serveru pro poskytování licencí domény uživatelů, kterou chcete přidat (od správce instalace, která má být považována za důvěryhodnou). Potom tuto doménu uživatelů přidejte do své instalace.</td>
<td style="border:1px solid black;">Přidání důvěryhodné domény uživatelů tématu <a href="http://go.microsoft.com/fwlink/?linkid=42495">Provoz serveru RMS</a></td>
</tr>
</tbody>
</table>
  
<span id="BKMK_18"></span>
Přidání důvěryhodných domén publikování  
---------------------------------------
  
Pro přidání důvěryhodných domén publikování použijte následující kontrolní seznam.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Krok</th>
<th style="border:1px solid black;" >Odkaz</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Nastudování příslušných základních pojmů</td>
<td style="border:1px solid black;">Důvěryhodné domény publikování tématu <a href="http://go.microsoft.com/fwlink/?linkid=42496">Technické informace týkající se služby RMS</a>
Přidání a odebrání důvěryhodných domén publikování tématu <a href="http://go.microsoft.com/fwlink/?linkid=42495">Provoz serveru RMS</a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Získání šifrovaného certifikátu serveru pro poskytování licencí a soukromého klíče požadované domény publikování a následné přidání domény publikování k instalaci</td>
<td style="border:1px solid black;">Přidání důvěryhodné domény publikování tématu <a href="http://go.microsoft.com/fwlink/?linkid=42495">Provoz serveru RMS</a></td>
</tr>
</tbody>
</table>
