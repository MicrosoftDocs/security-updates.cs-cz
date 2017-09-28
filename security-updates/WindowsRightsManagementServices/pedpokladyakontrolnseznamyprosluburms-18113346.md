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

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Krok</th>
<th>Odkaz</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>Posouzení informací o plánování a základních pojmů</p></td>
<td style="border:1px solid black;"><p>Příprava nasazení služby RMS tématu <a href="http://go.microsoft.com/fwlink/?linkid=42494">Nasazení systému služby RMS</a></p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Kontrola požadavků na systém a ověření, zda je k dispozici veškerý požadovaný hardware a software</p></td>
<td style="border:1px solid black;"><p>Předpoklady týkající se infrastruktury pro službu RMS tématu <a href="http://go.microsoft.com/fwlink/?linkid=37537">Plánování nasazení služby RMS</a></p>
<p>Plánování infrastruktury databázového serveru tématu <a href="http://go.microsoft.com/fwlink/?linkid=37537">Plánování nasazení služby RMS</a></p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Nastavení infrastruktury včetně požadavků na hardware a software, účtů správce a podpory služby SMS nebo Zásad skupiny (podle potřeby)</p></td>
<td style="border:1px solid black;"><p>Příprava nasazení služby RMS tématu <a href="http://go.microsoft.com/fwlink/?linkid=42494">Nasazení systému služby RMS</a></p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Instalace a konfigurace služby RMS na serveru</p></td>
<td style="border:1px solid black;"><p>Nastavení služby certifikace a správy licencí na prvním serveru tématu <a href="http://go.microsoft.com/fwlink/?linkid=42494">Nasazení systému služby RMS</a></p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Testování implementace</p></td>
<td style="border:1px solid black;"><p>Nastavení testovacího prostředí tématu <a href="http://go.microsoft.com/fwlink/?linkid=42494">Nasazení systému služby RMS</a></p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Implementace služby RMS v provozním prostředí</p></td>
<td style="border:1px solid black;"><p>Definování rozsahu implementace služby RMS tématu <a href="http://go.microsoft.com/fwlink/?linkid=42494">Nasazení systému služby RMS</a></p></td>
</tr>
</tbody>
</table>
  
<span id="BKMK_12"></span>
Nasazení clusterů kořenové certifikace a správy licencí  
-------------------------------------------------------
  
Pro nasazení clusterů kořenové certifikace a správy licencí použijte následující kontrolní seznam.
  
###  

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Krok</th>
<th>Odkaz</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>Posouzení informací o plánování a základních pojmů</p></td>
<td style="border:1px solid black;"><p>Příprava nasazení služby RMS tématu <a href="http://go.microsoft.com/fwlink/?linkid=42494">Nasazení systému služby RMS</a></p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Kontrola požadavků na systém a ověření, zda je k dispozici veškerý požadovaný hardware a software</p></td>
<td style="border:1px solid black;"><p>Předpoklady týkající se infrastruktury pro službu RMS tématu <a href="http://go.microsoft.com/fwlink/?linkid=37537">Plánování nasazení služby RMS</a></p>
<p>Plánování infrastruktury databázového serveru tématu <a href="http://go.microsoft.com/fwlink/?linkid=37537">Plánování nasazení služby RMS</a></p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Posouzení plánu implementace a seznámení se s topologií a instalovanými komponentami</p></td>
<td style="border:1px solid black;"><p>Určení topologie služby RMS tématu <a href="http://go.microsoft.com/fwlink/?linkid=37537">Plánování nasazení služby RMS</a></p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Nastavení infrastruktury včetně požadavků na hardware a software, účtů správce a podpory služby SMS nebo Zásad skupiny (podle potřeby)</p></td>
<td style="border:1px solid black;"><p>Příprava nasazení služby RMS tématu <a href="http://go.microsoft.com/fwlink/?linkid=42494">Nasazení systému služby RMS</a></p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Instalace a konfigurace služby RMS na serverech v clusteru kořenové certifikace</p></td>
<td style="border:1px solid black;"><p>Nastavení služby certifikace a správy licencí na prvním serveru tématu <a href="http://go.microsoft.com/fwlink/?linkid=42494">Nasazení systému služby RMS</a></p>
<p>Přidání serverů pro podporu certifikace a správy licencí tématu <a href="http://go.microsoft.com/fwlink/?linkid=42494">Nasazení systému služby RMS</a></p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Instalace a konfigurace služby RMS na serverech v clusterech správy licencí</p></td>
<td style="border:1px solid black;"><p>Nastavení služby certifikace a správy licencí na prvním serveru tématu <a href="http://go.microsoft.com/fwlink/?linkid=42494">Nasazení systému služby RMS</a></p>
<p>Přidání serverů pro podporu certifikace a správy licencí tématu <a href="http://go.microsoft.com/fwlink/?linkid=42494">Nasazení systému služby RMS</a></p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Nastavení vyrovnávání zatížení</p></td>
<td style="border:1px solid black;"><p>Rozšíření základní infrastruktury na podporu správy clusterů tématu <a href="http://go.microsoft.com/fwlink/?linkid=42494">Nasazení systému služby RMS</a></p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Testování implementace</p></td>
<td style="border:1px solid black;"><p>Nastavení testovacího prostředí tématu <a href="http://go.microsoft.com/fwlink/?linkid=42494">Nasazení systému služby RMS</a></p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Implementace služby RMS v provozním prostředí</p></td>
<td style="border:1px solid black;"><p>Definování rozsahu implementace služby RMS tématu <a href="http://go.microsoft.com/fwlink/?linkid=42494">Nasazení systému služby RMS</a></p></td>
</tr>
</tbody>
</table>
  
<span id="BKMK_13"></span>
Nasazení služby RMS v doménových strukturách  
--------------------------------------------
  
Pro nasazení kořenové služby RMS v doménových strukturách použijte následující kontrolní seznam.
  
###  

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Krok</th>
<th>Odkaz</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>Posouzení informací o plánování a základních pojmů</p></td>
<td style="border:1px solid black;"><p>Příprava nasazení služby RMS tématu <a href="http://go.microsoft.com/fwlink/?linkid=42494">Nasazení systému služby RMS</a></p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Konfigurace požadovaných oprávnění na základě modelu důvěryhodnosti</p></td>
<td style="border:1px solid black;"><p>Nasazení služby RMS v doménových strukturách tématu <a href="http://go.microsoft.com/fwlink/?linkid=42494">Nasazení systému služby RMS</a></p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Nastavení odpovídajících atributů služby Active Directory pro doménové struktury</p></td>
<td style="border:1px solid black;"><p>Nasazení služby RMS v doménových strukturách tématu <a href="http://go.microsoft.com/fwlink/?linkid=42494">Nasazení systému služby RMS</a></p></td>
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

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Krok</th>
<th>Odkaz</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>Nastudování příslušných základních pojmů</p></td>
<td style="border:1px solid black;"><p>Šablony zásad práv tématu <a href="http://go.microsoft.com/fwlink/?linkid=42496">Technické informace týkající se služby RMS</a></p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Zadání umístění šablony zásad práv</p></td>
<td style="border:1px solid black;"><p>Zadání umístění šablon zásad práv tématu <a href="http://go.microsoft.com/fwlink/?linkid=42495">Provoz serveru RMS</a></p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Vytvoření šablony zásad práv</p></td>
<td style="border:1px solid black;"><p>Vytvoření a změna šablon zásad práv tématu <a href="http://go.microsoft.com/fwlink/?linkid=42495">Provoz serveru RMS</a></p>
<p>Přidání šablony zásad práv tématu <a href="http://go.microsoft.com/fwlink/?linkid=42495">Provoz serveru RMS</a></p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Distribuce šablony zásad práv</p></td>
<td style="border:1px solid black;"><p>Distribuce šablon zásad práv tématu <a href="http://go.microsoft.com/fwlink/?linkid=42495">Provoz serveru RMS</a></p></td>
</tr>
</tbody>
</table>
  
<span id="BKMK_16"></span>
Nasazení nového klienta služby RMS  
----------------------------------
  
Pro nasazení nové verze klienta RMS použijte následující kontrolní seznam.
  
###  

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Krok</th>
<th>Odkaz</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>Nastudování příslušných základních pojmů</p></td>
<td style="border:1px solid black;"><p>Plánování distribuce klientů tématu <a href="http://go.microsoft.com/fwlink/?linkid=42494">Nasazení systému služby RMS</a></p>
<p>Vyloučení verzí bezpečnostního modulu tématu <a href="http://go.microsoft.com/fwlink/?linkid=42495">Provoz serveru RMS</a></p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Chcete-li u všech klientů vynutit upgrade na nejnovější verzi klienta, vylučte zastaralou verzi bezpečnostního modulu.</p></td>
<td style="border:1px solid black;"><p>Vyloučení verzí bezpečnostního modulu tématu <a href="http://go.microsoft.com/fwlink/?linkid=42495">Provoz serveru RMS</a></p></td>
</tr>
</tbody>
</table>
  
<span id="BKMK_17"></span>
Přidání důvěryhodných domén uživatelů  
-------------------------------------
  
Pro přidání důvěryhodných domén uživatelů použijte následující kontrolní seznam.
  
###  

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Krok</th>
<th>Odkaz</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>Nastudování příslušných základních pojmů</p></td>
<td style="border:1px solid black;"><p>Důvěryhodné domény uživatelů tématu <a href="http://go.microsoft.com/fwlink/?linkid=42496">Technické informace týkající se služby RMS</a></p>
<p>Přidání a odebrání důvěryhodných domén uživatelů tématu <a href="http://go.microsoft.com/fwlink/?linkid=42495">Provoz serveru RMS</a></p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Získejte certifikát serveru pro poskytování licencí domény uživatelů, kterou chcete přidat (od správce instalace, která má být považována za důvěryhodnou). Potom tuto doménu uživatelů přidejte do své instalace.</p></td>
<td style="border:1px solid black;"><p>Přidání důvěryhodné domény uživatelů tématu <a href="http://go.microsoft.com/fwlink/?linkid=42495">Provoz serveru RMS</a></p></td>
</tr>
</tbody>
</table>
  
<span id="BKMK_18"></span>
Přidání důvěryhodných domén publikování  
---------------------------------------
  
Pro přidání důvěryhodných domén publikování použijte následující kontrolní seznam.
  
###  

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Krok</th>
<th>Odkaz</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>Nastudování příslušných základních pojmů</p></td>
<td style="border:1px solid black;"><p>Důvěryhodné domény publikování tématu <a href="http://go.microsoft.com/fwlink/?linkid=42496">Technické informace týkající se služby RMS</a></p>
<p>Přidání a odebrání důvěryhodných domén publikování tématu <a href="http://go.microsoft.com/fwlink/?linkid=42495">Provoz serveru RMS</a></p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Získání šifrovaného certifikátu serveru pro poskytování licencí a soukromého klíče požadované domény publikování a následné přidání domény publikování k instalaci</p></td>
<td style="border:1px solid black;"><p>Přidání důvěryhodné domény publikování tématu <a href="http://go.microsoft.com/fwlink/?linkid=42495">Provoz serveru RMS</a></p></td>
</tr>
</tbody>
</table>
