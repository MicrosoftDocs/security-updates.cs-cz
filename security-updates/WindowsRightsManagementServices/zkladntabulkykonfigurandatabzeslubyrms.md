---
TOCTitle: Základní tabulky konfigurační databáze služby RMS
Title: Základní tabulky konfigurační databáze služby RMS
ms:assetid: '8f9e15a2-92bc-41f7-a4fd-329567afb142'
ms:contentKeyID: 18113423
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747676(v=WS.10)'
---

Základní tabulky konfigurační databáze služby RMS
=================================================

V tomto tématu jsou popsány základní tabulky konfigurační databáze služby RMS.

DRMS\_ApplicationExclusionList
------------------------------

V následující tabulce jsou uvedeny informace o vyloučených aplikacích.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Název</th>
<th style="border:1px solid black;" >Typ dat</th>
<th style="border:1px solid black;" >Hodnoty NULL</th>
<th style="border:1px solid black;" >Popis</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">ID</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">IDENTITY(100,1) Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">Interní index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Název</td>
<td style="border:1px solid black;">nvarchar(256)</td>
<td style="border:1px solid black;">Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">Název aplikace</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">VersionMinMajor</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Minimální hlavní číslo verze aplikace</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">VersionMinMinor</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Minimální dílčí číslo verze aplikace</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">VersionMinBuild</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Minimální číslo verze sestavení aplikace</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">VersionMinRevision</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Minimální číslo verze revize aplikace</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">VersionMaxMajor</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Maximální hlavní číslo verze aplikace</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">VersionMaxMinor</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Maximální dílčí číslo verze aplikace</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">VersionMaxBuild</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Maximální číslo verze sestavení aplikace</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">VersionMaxRevision</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Maximální číslo verze revize aplikace</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Popis</td>
<td style="border:1px solid black;">nvarchar(256)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Popis aplikace</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">dt_DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Časové razítko aktualizace</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">dt_DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Časové razítko vytvoření</td>
</tr>
</tbody>
</table>
  
DRMS\_AsynchronousQueue  
-----------------------
  
V následující tabulce jsou uvedeny informace o frontě zpráv.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Název</th>
<th style="border:1px solid black;" >Typ dat</th>
<th style="border:1px solid black;" >Hodnoty NULL</th>
<th style="border:1px solid black;" >Popis</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">AsyncQueueID</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">IDENTITY(100,1) Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">Interní index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">QueueName</td>
<td style="border:1px solid black;">nvarchar(256)</td>
<td style="border:1px solid black;">Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">Cesta k frontě zpráv</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Časové razítko aktualizace</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Časové razítko vytvoření</td>
</tr>
</tbody>
</table>
  
DRMS\_CaType  
------------
  
V následující tabulce jsou uvedeny informace o typu certifikátu vydaného klientovi.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Název</th>
<th style="border:1px solid black;" >Typ dat</th>
<th style="border:1px solid black;" >Hodnoty NULL</th>
<th style="border:1px solid black;" >Popis</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">ID</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">ID certifikátu</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">TypeName</td>
<td style="border:1px solid black;">nvarchar(256)</td>
<td style="border:1px solid black;">Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">Desktop, MobileDevice nebo Server</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Časové razítko aktualizace</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Časové razítko vytvoření</td>
</tr>
</tbody>
</table>
  
DRMS\_ClusterConfiguration  
--------------------------
  
V následující tabulce jsou uvedeny informace o aktuálním certifikátu serveru pro poskytování licencí, který je v tabulce DRMS\_LicensorCertificate.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Název</th>
<th style="border:1px solid black;" >Typ dat</th>
<th style="border:1px solid black;" >Hodnoty NULL</th>
<th style="border:1px solid black;" >Popis</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">CurrentLicensorCertID</td>
<td style="border:1px solid black;">int (FK)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Aktivní certifikát serveru pro poskytování licencí</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Časové razítko aktualizace</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Časové razítko vytvoření</td>
</tr>
</tbody>
</table>
  
DRMS\_ClusterPolicies  
---------------------
  
V následující tabulce jsou uvedeny informace o umístěních, ve kterých jsou uloženy zásady clusterů.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Název</th>
<th style="border:1px solid black;" >Typ dat</th>
<th style="border:1px solid black;" >Hodnoty NULL</th>
<th style="border:1px solid black;" >Popis</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">PolicyID</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">IDENTITY(100,1) Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">ID zásady</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PolicyName</td>
<td style="border:1px solid black;">nvarchar(64)</td>
<td style="border:1px solid black;">Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">Název zásady</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">PolicyData</td>
<td style="border:1px solid black;">sql_variant</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Data zásady</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Časové razítko aktualizace</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Časové razítko vytvoření</td>
</tr>
</tbody>
</table>
  
DRMS\_ClusterServer  
-------------------
  
V následující tabulce jsou uvedeny informace o serverech, které jsou v clusteru.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Název</th>
<th style="border:1px solid black;" >Typ dat</th>
<th style="border:1px solid black;" >Hodnoty NULL</th>
<th style="border:1px solid black;" >Popis</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">ServerID</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">IDENTITY(100,1) Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">ID serveru</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">ServerName</td>
<td style="border:1px solid black;">nvarchar(256)</td>
<td style="border:1px solid black;">Nezadáno</td>
<td style="border:1px solid black;">Název počítače serveru</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Časové razítko aktualizace</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Časové razítko vytvoření</td>
</tr>
</tbody>
</table>
  
DRMS\_GICExclusionList  
----------------------
  
V následující tabulce jsou uvedeny informace o vyloučených certifikátech účtů práv.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Název</th>
<th style="border:1px solid black;" >Typ dat</th>
<th style="border:1px solid black;" >Hodnoty NULL</th>
<th style="border:1px solid black;" >Popis</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">PublicKeyIndex</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">IDENTITY(100,1) Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">Interní index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PublicKey</td>
<td style="border:1px solid black;">PublicKey</td>
<td style="border:1px solid black;">Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">Bajty veřejného klíče</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">UserID</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Index ID uživatele</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">ExpirationDate</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Datum vypršení platnosti certifikátu účtu práv</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Popis</td>
<td style="border:1px solid black;">nvarchar(256)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">NÁZEV přidružený k tomuto klíči vyloučeného certifikátu účtu práv</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">dt_DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">Časové razítko aktualizace</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">dt_DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">Časové razítko vytvoření</td>
</tr>
</tbody>
</table>
  
DRMS\_LicensorCertificate  
-------------------------
  
V následující tabulce jsou uvedeny informace o aktivním certifikátu serveru pro poskytování licencí.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Název</th>
<th style="border:1px solid black;" >Typ dat</th>
<th style="border:1px solid black;" >Hodnoty NULL</th>
<th style="border:1px solid black;" >Popis</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">i_CertID</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">IDENTITY(100,1) Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">ID zásady</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_CertGUIDType</td>
<td style="border:1px solid black;">nvarchar(64)</td>
<td style="border:1px solid black;">Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">Typ ID páru klíčů</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">s_CertGUID</td>
<td style="border:1px solid black;">nvarchar(128)</td>
<td style="border:1px solid black;">Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">Identifikátor GUID páru klíčů</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">i_CertificateID</td>
<td style="border:1px solid black;">int (FK)</td>
<td style="border:1px solid black;">Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">Ukazatel na skutečný certifikát</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">dt_DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Časové razítko aktualizace</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">dt_DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Časové razítko vytvoření</td>
</tr>
</tbody>
</table>
  
DRMS\_LicensorPrivateKey  
------------------------
  
Následující tabulka obsahuje informace o soukromém klíči aktivního certifikátu serveru pro poskytování licencí.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Název</th>
<th style="border:1px solid black;" >Typ dat</th>
<th style="border:1px solid black;" >Hodnoty NULL</th>
<th style="border:1px solid black;" >Popis</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">PrivateKeyID</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">IDENTITY(100,1) Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">Interní index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">CertGUIDType</td>
<td style="border:1px solid black;">nvarchar(64)</td>
<td style="border:1px solid black;">Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">Typ ID páru klíčů</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">CertGUID</td>
<td style="border:1px solid black;">nvarchar(128)</td>
<td style="border:1px solid black;">Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">Identifikátor GUID páru klíčů</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PrivateKey</td>
<td style="border:1px solid black;">varbinary(2048)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Binární reprezentace klíče</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">CSP</td>
<td style="border:1px solid black;">nvarchar(512)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Název zprostředkovatele kryptografických služeb (CSP)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">CSPType</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Typ zprostředkovatele CSP</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">KeyContainerName</td>
<td style="border:1px solid black;">nvarchar(512)</td>
<td style="border:1px solid black;">Nezadáno</td>
<td style="border:1px solid black;">Název kontejneru klíče</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">KeyNumber</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Číslo klíče</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Časové razítko aktualizace</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Časové razítko vytvoření</td>
</tr>
</tbody>
</table>
  
DRMS\_PassportDenyList  
----------------------
  
V následující tabulce jsou uvedeny informace o účtech služby Microsoft® .NET Passport, kterým mají být odepřeny licence.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Název</th>
<th style="border:1px solid black;" >Typ dat</th>
<th style="border:1px solid black;" >Hodnoty NULL</th>
<th style="border:1px solid black;" >Popis</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">DenyID</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">IDENTITY(100,1) Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">Interní index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DenyAddressPattern</td>
<td style="border:1px solid black;">nvarchar(500)</td>
<td style="border:1px solid black;">Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">Uživatelské jméno/název domény</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Časové razítko aktualizace</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Časové razítko vytvoření</td>
</tr>
</tbody>
</table>
  
DRMS\_Plugin  
------------
  
V následující tabulce jsou uvedeny informace o modulech plug-in.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Název</th>
<th style="border:1px solid black;" >Typ dat</th>
<th style="border:1px solid black;" >Hodnoty NULL</th>
<th style="border:1px solid black;" >Popis</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">PluginID</td>
<td style="border:1px solid black;">Int</td>
<td style="border:1px solid black;">IDENTITY(100,1) Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">Interní index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PluginTypeID</td>
<td style="border:1px solid black;">int (FK)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Typ modulu plug-in</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">NameSpace</td>
<td style="border:1px solid black;">nvarchar(128)</td>
<td style="border:1px solid black;">Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">Obor názvů tohoto modulu plug-in</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PluginName</td>
<td style="border:1px solid black;">nvarchar(128)</td>
<td style="border:1px solid black;">Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">Název tohoto modulu plug-in</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Ordinal</td>
<td style="border:1px solid black;">Int</td>
<td style="border:1px solid black;">Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">Číslo pořadí, v němž je modul plug-in spuštěn</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Path</td>
<td style="border:1px solid black;">nvarchar(512)</td>
<td style="border:1px solid black;">Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">Cesta k souboru DLL</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">ObjectTypeName</td>
<td style="border:1px solid black;">nvarchar(50)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Nepoužito</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DebugMode</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Určuje, zda má být modul plug-in spuštěn v režimu ladění</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">PublicKey</td>
<td style="border:1px solid black;">PublicKey</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Veřejný klíč modulu plug-in</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Version</td>
<td style="border:1px solid black;">nvarchar(64)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Verze modulu plug-in</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Časové razítko aktualizace</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Časové razítko vytvoření</td>
</tr>
</tbody>
</table>
  
DRMS\_AllowedPluginVersions  
---------------------------
  
V následující tabulce jsou uvedeny informace o verzích modulu plug-in, které jsou v systému služby RMS povoleny.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Název</th>
<th style="border:1px solid black;" >Typ dat</th>
<th style="border:1px solid black;" >Hodnoty NULL</th>
<th style="border:1px solid black;" >Popis</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">RowID</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">Interní index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PluginID</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">IDENTITY(100,1) Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">Interní index</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">VersionInfo</td>
<td style="border:1px solid black;">nvarchar(64)</td>
<td style="border:1px solid black;">Nezadáno</td>
<td style="border:1px solid black;">Verze modulu plug-in</td>
</tr>
</tbody>
</table>
  
DRMS\_PluginProperties  
----------------------
  
V následující tabulce jsou uvedeny informace o vlastnostech modulu plug-in.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Název</th>
<th style="border:1px solid black;" >Typ dat</th>
<th style="border:1px solid black;" >Hodnoty NULL</th>
<th style="border:1px solid black;" >Popis</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">PropertyID</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">IDENTITY(100,1) Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">Interní index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PluginID</td>
<td style="border:1px solid black;">int (FK)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">ID modulu plug-in, do něhož vlastnost patří</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">PropertyName</td>
<td style="border:1px solid black;">nvarchar(256)</td>
<td style="border:1px solid black;">Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">Název vlastnosti pro tato konfigurační data</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PropertyValue</td>
<td style="border:1px solid black;">text</td>
<td style="border:1px solid black;">Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">Hodnota vlastnosti pro tato konfigurační data</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Časové razítko aktualizace</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Časové razítko vytvoření</td>
</tr>
</tbody>
</table>
  
DRMS\_PluginType  
----------------
  
V následující tabulce jsou uvedeny informace o typu modulu plug-in.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Název</th>
<th style="border:1px solid black;" >Typ dat</th>
<th style="border:1px solid black;" >Hodnoty NULL</th>
<th style="border:1px solid black;" >Popis</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">PluginTypeID</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">Interní index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PluginTypeName</td>
<td style="border:1px solid black;">nvarchar(256)</td>
<td style="border:1px solid black;">Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">Název tohoto modulu plug-in</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Časové razítko aktualizace</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Časové razítko vytvoření</td>
</tr>
</tbody>
</table>
  
DRMS\_RightsTemplate  
--------------------
  
V následující tabulce jsou uvedeny informace o šablonách zásad práv.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Název</th>
<th style="border:1px solid black;" >Typ dat</th>
<th style="border:1px solid black;" >Hodnoty NULL</th>
<th style="border:1px solid black;" >Popis</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Guid</td>
<td style="border:1px solid black;">nvarchar(128) (PK)</td>
<td style="border:1px solid black;">Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">Identifikátor GUID šablony zásad práv</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">TemplateData</td>
<td style="border:1px solid black;">ntext</td>
<td style="border:1px solid black;">Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">Toto pole obsahuje data šablony XrML.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Časové razítko aktualizace</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Časové razítko vytvoření</td>
</tr>
</tbody>
</table>
  
DRMS\_TrustedCertificateAuthorities  
-----------------------------------
  
V následující tabulce jsou uvedeny informace o důvěryhodných certifikačních autoritách.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Název</th>
<th style="border:1px solid black;" >Typ dat</th>
<th style="border:1px solid black;" >Hodnoty NULL</th>
<th style="border:1px solid black;" >Popis</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">ID</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">IDENTITY(1,1) Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">Interní index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">CertificateID</td>
<td style="border:1px solid black;">int (FK)</td>
<td style="border:1px solid black;">Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">ID certifikátu</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">CertificateGUID</td>
<td style="border:1px solid black;">nvarchar(128)</td>
<td style="border:1px solid black;">Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">Identifikátor GUID certifikátu</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">CaTypeID</td>
<td style="border:1px solid black;">int (FK)</td>
<td style="border:1px solid black;">Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">Typ certifikační autority</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Časové razítko aktualizace</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Časové razítko vytvoření</td>
</tr>
</tbody>
</table>
  
DRMS\_TrustedEmailDomains  
-------------------------
  
V následující tabulce jsou uvedeny informace o e-mailových doménách, které jsou důvěryhodné v prostředí služby RMS.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Název</th>
<th style="border:1px solid black;" >Typ dat</th>
<th style="border:1px solid black;" >Hodnoty NULL</th>
<th style="border:1px solid black;" >Popis</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">ID</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">IDENTITY(100,1) Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">Interní index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">i_TrustedIdentityDomainID</td>
<td style="border:1px solid black;">int (FK)t</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Interní index</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">s_EmailDomainName</td>
<td style="border:1px solid black;">nvarchar(256)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Seznam názvů e-mailových domén, které jsou platné pro důvěryhodnou doménu uživatelů.</td>
</tr>
</tbody>
</table>
  
DRMS\_TrustedIdentityDomain  
---------------------------
  
V následující tabulce jsou uvedeny informace o důvěryhodných doménách uživatelů a důvěryhodných doménách publikování.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Název</th>
<th style="border:1px solid black;" >Typ dat</th>
<th style="border:1px solid black;" >Hodnoty NULL</th>
<th style="border:1px solid black;" >Popis</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">i_TrustedIdentityDomainID</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">IDENTITY(100,1) Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">Interní index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_DomainType</td>
<td style="border:1px solid black;">nvarchar(64)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Typ domény</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">CertGUIDType</td>
<td style="border:1px solid black;">nvarchar(64)</td>
<td style="border:1px solid black;">Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">Typ identifikátoru GUID certifikátu</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">CertGUID</td>
<td style="border:1px solid black;">nvarchar(128)</td>
<td style="border:1px solid black;">Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">Identifikátor GUID certifikátu</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">i_CertificateID</td>
<td style="border:1px solid black;">int (FK)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">ID certifikátu</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">i_allowSID</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">Identifikátor SID domény</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">S_friendlyname</td>
<td style="border:1px solid black;">nvarchar(255)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Popisný název certifikátu</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">dt_DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Časové razítko aktualizace</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">dt_DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Časové razítko vytvoření</td>
</tr>
</tbody>
</table>
  
DRMS\_XrML\_Certificate  
-----------------------
  
V následující tabulce jsou uvedeny informace o certifikátech serveru pro poskytování licencí XrML, na které odkazuje tabulka DRMS\_LicensorCertificate. Rovněž mapuje řetěz certifikátů.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Název</th>
<th style="border:1px solid black;" >Typ dat</th>
<th style="border:1px solid black;" >Hodnoty NULL</th>
<th style="border:1px solid black;" >Popis</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">i_CertificateID</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">IDENTITY(100,1) Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">Ukazatel na skutečný certifikát</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_Certificate</td>
<td style="border:1px solid black;">ntext</td>
<td style="border:1px solid black;">Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">Ukazatel na skutečný certifikát</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">i_ParentCertificateID</td>
<td style="border:1px solid black;">int (FK)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Ukazatel na skutečný certifikát</td>
</tr>
</tbody>
</table>
