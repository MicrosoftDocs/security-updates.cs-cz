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

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th>Název</th>
<th>Typ dat</th>
<th>Hodnoty NULL</th>
<th>Popis</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>ID</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>IDENTITY(100,1) Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>Interní index</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Název</p></td>
<td style="border:1px solid black;"><p>nvarchar(256)</p></td>
<td style="border:1px solid black;"><p>Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>Název aplikace</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>VersionMinMajor</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Minimální hlavní číslo verze aplikace</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>VersionMinMinor</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Minimální dílčí číslo verze aplikace</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>VersionMinBuild</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Minimální číslo verze sestavení aplikace</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>VersionMinRevision</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Minimální číslo verze revize aplikace</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>VersionMaxMajor</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Maximální hlavní číslo verze aplikace</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>VersionMaxMinor</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Maximální dílčí číslo verze aplikace</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>VersionMaxBuild</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Maximální číslo verze sestavení aplikace</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>VersionMaxRevision</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Maximální číslo verze revize aplikace</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Popis</p></td>
<td style="border:1px solid black;"><p>nvarchar(256)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Popis aplikace</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>dt_DateUpdated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Časové razítko aktualizace</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>dt_DateCreated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Časové razítko vytvoření</p></td>
</tr>  
</tbody>  
</table>
  
DRMS\_AsynchronousQueue  
-----------------------
  
V následující tabulce jsou uvedeny informace o frontě zpráv.
  
###  

<p> </p>
<table style="border:1px solid black;">  
<colgroup>  
<col width="25%" />  
<col width="25%" />  
<col width="25%" />  
<col width="25%" />  
</colgroup>  
<thead>  
<tr class="header">  
<th>Název</th>  
<th>Typ dat</th>  
<th>Hodnoty NULL</th>  
<th>Popis</th>  
</tr>  
</thead>  
<tbody>  
<tr class="odd">
<td style="border:1px solid black;"><p>AsyncQueueID</p></td>
<td style="border:1px solid black;"><p>Int (PK)</p></td>
<td style="border:1px solid black;"><p>IDENTITY(100,1) Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>Interní index</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>QueueName</p></td>
<td style="border:1px solid black;"><p>nvarchar(256)</p></td>
<td style="border:1px solid black;"><p>Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>Cesta k frontě zpráv</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>DateUpdated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Časové razítko aktualizace</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>DateCreated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Časové razítko vytvoření</p></td>
</tr>  
</tbody>  
</table>
  
DRMS\_CaType  
------------
  
V následující tabulce jsou uvedeny informace o typu certifikátu vydaného klientovi.
  
###  

<p> </p>
<table style="border:1px solid black;">  
<colgroup>  
<col width="25%" />  
<col width="25%" />  
<col width="25%" />  
<col width="25%" />  
</colgroup>  
<thead>  
<tr class="header">  
<th>Název</th>  
<th>Typ dat</th>  
<th>Hodnoty NULL</th>  
<th>Popis</th>  
</tr>  
</thead>  
<tbody>  
<tr class="odd">
<td style="border:1px solid black;"><p>ID</p></td>
<td style="border:1px solid black;"><p>Int (PK)</p></td>
<td style="border:1px solid black;"><p>Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>ID certifikátu</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>TypeName</p></td>
<td style="border:1px solid black;"><p>nvarchar(256)</p></td>
<td style="border:1px solid black;"><p>Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>Desktop, MobileDevice nebo Server</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>DateUpdated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Časové razítko aktualizace</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>DateCreated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Časové razítko vytvoření</p></td>
</tr>  
</tbody>  
</table>
  
DRMS\_ClusterConfiguration  
--------------------------
  
V následující tabulce jsou uvedeny informace o aktuálním certifikátu serveru pro poskytování licencí, který je v tabulce DRMS\_LicensorCertificate.
  
###  

<p> </p>
<table style="border:1px solid black;">  
<colgroup>  
<col width="25%" />  
<col width="25%" />  
<col width="25%" />  
<col width="25%" />  
</colgroup>  
<thead>  
<tr class="header">  
<th>Název</th>  
<th>Typ dat</th>  
<th>Hodnoty NULL</th>  
<th>Popis</th>  
</tr>  
</thead>  
<tbody>  
<tr class="odd">
<td style="border:1px solid black;"><p>CurrentLicensorCertID</p></td>
<td style="border:1px solid black;"><p>int (FK)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Aktivní certifikát serveru pro poskytování licencí</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>DateUpdated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Časové razítko aktualizace</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>DateCreated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Časové razítko vytvoření</p></td>
</tr>  
</tbody>  
</table>
  
DRMS\_ClusterPolicies  
---------------------
  
V následující tabulce jsou uvedeny informace o umístěních, ve kterých jsou uloženy zásady clusterů.
  
###  

<p> </p>
<table style="border:1px solid black;">  
<colgroup>  
<col width="25%" />  
<col width="25%" />  
<col width="25%" />  
<col width="25%" />  
</colgroup>  
<thead>  
<tr class="header">  
<th>Název</th>  
<th>Typ dat</th>  
<th>Hodnoty NULL</th>  
<th>Popis</th>  
</tr>  
</thead>  
<tbody>  
<tr class="odd">
<td style="border:1px solid black;"><p>PolicyID</p></td>
<td style="border:1px solid black;"><p>Int (PK)</p></td>
<td style="border:1px solid black;"><p>IDENTITY(100,1) Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>ID zásady</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>PolicyName</p></td>
<td style="border:1px solid black;"><p>nvarchar(64)</p></td>
<td style="border:1px solid black;"><p>Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>Název zásady</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>PolicyData</p></td>
<td style="border:1px solid black;"><p>sql_variant</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Data zásady</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>DateUpdated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Časové razítko aktualizace</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>DateCreated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Časové razítko vytvoření</p></td>
</tr>  
</tbody>  
</table>
  
DRMS\_ClusterServer  
-------------------
  
V následující tabulce jsou uvedeny informace o serverech, které jsou v clusteru.
  
###  

<p> </p>
<table style="border:1px solid black;">  
<colgroup>  
<col width="25%" />  
<col width="25%" />  
<col width="25%" />  
<col width="25%" />  
</colgroup>  
<thead>  
<tr class="header">  
<th>Název</th>  
<th>Typ dat</th>  
<th>Hodnoty NULL</th>  
<th>Popis</th>  
</tr>  
</thead>  
<tbody>  
<tr class="odd">
<td style="border:1px solid black;"><p>ServerID</p></td>
<td style="border:1px solid black;"><p>Int (PK)</p></td>
<td style="border:1px solid black;"><p>IDENTITY(100,1) Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>ID serveru</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>ServerName</p></td>
<td style="border:1px solid black;"><p>nvarchar(256)</p></td>
<td style="border:1px solid black;"><p>Nezadáno</p></td>
<td style="border:1px solid black;"><p>Název počítače serveru</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>DateUpdated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Časové razítko aktualizace</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>DateCreated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Časové razítko vytvoření</p></td>
</tr>  
</tbody>  
</table>
  
DRMS\_GICExclusionList  
----------------------
  
V následující tabulce jsou uvedeny informace o vyloučených certifikátech účtů práv.
  
###  

<p> </p>
<table style="border:1px solid black;">  
<colgroup>  
<col width="25%" />  
<col width="25%" />  
<col width="25%" />  
<col width="25%" />  
</colgroup>  
<thead>  
<tr class="header">  
<th>Název</th>  
<th>Typ dat</th>  
<th>Hodnoty NULL</th>  
<th>Popis</th>  
</tr>  
</thead>  
<tbody>  
<tr class="odd">
<td style="border:1px solid black;"><p>PublicKeyIndex</p></td>
<td style="border:1px solid black;"><p>Int (PK)</p></td>
<td style="border:1px solid black;"><p>IDENTITY(100,1) Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>Interní index</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>PublicKey</p></td>
<td style="border:1px solid black;"><p>PublicKey</p></td>
<td style="border:1px solid black;"><p>Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>Bajty veřejného klíče</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>UserID</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Index ID uživatele</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>ExpirationDate</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Datum vypršení platnosti certifikátu účtu práv</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Popis</p></td>
<td style="border:1px solid black;"><p>nvarchar(256)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>NÁZEV přidružený k tomuto klíči vyloučeného certifikátu účtu práv</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>dt_DateUpdated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>Časové razítko aktualizace</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>dt_DateCreated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>Časové razítko vytvoření</p></td>
</tr>  
</tbody>  
</table>
  
DRMS\_LicensorCertificate  
-------------------------
  
V následující tabulce jsou uvedeny informace o aktivním certifikátu serveru pro poskytování licencí.
  
###  

<p> </p>
<table style="border:1px solid black;">  
<colgroup>  
<col width="25%" />  
<col width="25%" />  
<col width="25%" />  
<col width="25%" />  
</colgroup>  
<thead>  
<tr class="header">  
<th>Název</th>  
<th>Typ dat</th>  
<th>Hodnoty NULL</th>  
<th>Popis</th>  
</tr>  
</thead>  
<tbody>  
<tr class="odd">
<td style="border:1px solid black;"><p>i_CertID</p></td>
<td style="border:1px solid black;"><p>Int (PK)</p></td>
<td style="border:1px solid black;"><p>IDENTITY(100,1) Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>ID zásady</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>s_CertGUIDType</p></td>
<td style="border:1px solid black;"><p>nvarchar(64)</p></td>
<td style="border:1px solid black;"><p>Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>Typ ID páru klíčů</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>s_CertGUID</p></td>
<td style="border:1px solid black;"><p>nvarchar(128)</p></td>
<td style="border:1px solid black;"><p>Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>Identifikátor GUID páru klíčů</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>i_CertificateID</p></td>
<td style="border:1px solid black;"><p>int (FK)</p></td>
<td style="border:1px solid black;"><p>Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>Ukazatel na skutečný certifikát</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>dt_DateUpdated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Časové razítko aktualizace</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>dt_DateCreated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Časové razítko vytvoření</p></td>
</tr>  
</tbody>  
</table>
  
DRMS\_LicensorPrivateKey  
------------------------
  
Následující tabulka obsahuje informace o soukromém klíči aktivního certifikátu serveru pro poskytování licencí.
  
###  

<p> </p>
<table style="border:1px solid black;">  
<colgroup>  
<col width="25%" />  
<col width="25%" />  
<col width="25%" />  
<col width="25%" />  
</colgroup>  
<thead>  
<tr class="header">  
<th>Název</th>  
<th>Typ dat</th>  
<th>Hodnoty NULL</th>  
<th>Popis</th>  
</tr>  
</thead>  
<tbody>  
<tr class="odd">
<td style="border:1px solid black;"><p>PrivateKeyID</p></td>
<td style="border:1px solid black;"><p>Int (PK)</p></td>
<td style="border:1px solid black;"><p>IDENTITY(100,1) Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>Interní index</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>CertGUIDType</p></td>
<td style="border:1px solid black;"><p>nvarchar(64)</p></td>
<td style="border:1px solid black;"><p>Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>Typ ID páru klíčů</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>CertGUID</p></td>
<td style="border:1px solid black;"><p>nvarchar(128)</p></td>
<td style="border:1px solid black;"><p>Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>Identifikátor GUID páru klíčů</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>PrivateKey</p></td>
<td style="border:1px solid black;"><p>varbinary(2048)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Binární reprezentace klíče</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>CSP</p></td>
<td style="border:1px solid black;"><p>nvarchar(512)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Název zprostředkovatele kryptografických služeb (CSP)</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>CSPType</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Typ zprostředkovatele CSP</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>KeyContainerName</p></td>
<td style="border:1px solid black;"><p>nvarchar(512)</p></td>
<td style="border:1px solid black;"><p>Nezadáno</p></td>
<td style="border:1px solid black;"><p>Název kontejneru klíče</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>KeyNumber</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Číslo klíče</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>DateUpdated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Časové razítko aktualizace</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>DateCreated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Časové razítko vytvoření</p></td>
</tr>  
</tbody>  
</table>
  
DRMS\_PassportDenyList  
----------------------
  
V následující tabulce jsou uvedeny informace o účtech služby Microsoft® .NET Passport, kterým mají být odepřeny licence.
  
###  

<p> </p>
<table style="border:1px solid black;">  
<colgroup>  
<col width="25%" />  
<col width="25%" />  
<col width="25%" />  
<col width="25%" />  
</colgroup>  
<thead>  
<tr class="header">  
<th>Název</th>  
<th>Typ dat</th>  
<th>Hodnoty NULL</th>  
<th>Popis</th>  
</tr>  
</thead>  
<tbody>  
<tr class="odd">
<td style="border:1px solid black;"><p>DenyID</p></td>
<td style="border:1px solid black;"><p>Int (PK)</p></td>
<td style="border:1px solid black;"><p>IDENTITY(100,1) Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>Interní index</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>DenyAddressPattern</p></td>
<td style="border:1px solid black;"><p>nvarchar(500)</p></td>
<td style="border:1px solid black;"><p>Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>Uživatelské jméno/název domény</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>DateUpdated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Časové razítko aktualizace</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>DateCreated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Časové razítko vytvoření</p></td>
</tr>  
</tbody>  
</table>
  
DRMS\_Plugin  
------------
  
V následující tabulce jsou uvedeny informace o modulech plug-in.
  
###  

<p> </p>
<table style="border:1px solid black;">  
<colgroup>  
<col width="25%" />  
<col width="25%" />  
<col width="25%" />  
<col width="25%" />  
</colgroup>  
<thead>  
<tr class="header">  
<th>Název</th>  
<th>Typ dat</th>  
<th>Hodnoty NULL</th>  
<th>Popis</th>  
</tr>  
</thead>  
<tbody>  
<tr class="odd">
<td style="border:1px solid black;"><p>PluginID</p></td>
<td style="border:1px solid black;"><p>Int</p></td>
<td style="border:1px solid black;"><p>IDENTITY(100,1) Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>Interní index</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>PluginTypeID</p></td>
<td style="border:1px solid black;"><p>int (FK)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Typ modulu plug-in</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>NameSpace</p></td>
<td style="border:1px solid black;"><p>nvarchar(128)</p></td>
<td style="border:1px solid black;"><p>Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>Obor názvů tohoto modulu plug-in</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>PluginName</p></td>
<td style="border:1px solid black;"><p>nvarchar(128)</p></td>
<td style="border:1px solid black;"><p>Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>Název tohoto modulu plug-in</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Ordinal</p></td>
<td style="border:1px solid black;"><p>Int</p></td>
<td style="border:1px solid black;"><p>Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>Číslo pořadí, v němž je modul plug-in spuštěn</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Path</p></td>
<td style="border:1px solid black;"><p>nvarchar(512)</p></td>
<td style="border:1px solid black;"><p>Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>Cesta k souboru DLL</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>ObjectTypeName</p></td>
<td style="border:1px solid black;"><p>nvarchar(50)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Nepoužito</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>DebugMode</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Určuje, zda má být modul plug-in spuštěn v režimu ladění</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>PublicKey</p></td>
<td style="border:1px solid black;"><p>PublicKey</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Veřejný klíč modulu plug-in</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Version</p></td>
<td style="border:1px solid black;"><p>nvarchar(64)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Verze modulu plug-in</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>DateUpdated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Časové razítko aktualizace</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>DateCreated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Časové razítko vytvoření</p></td>
</tr>  
</tbody>  
</table>
  
DRMS\_AllowedPluginVersions  
---------------------------
  
V následující tabulce jsou uvedeny informace o verzích modulu plug-in, které jsou v systému služby RMS povoleny.
  
###  

<p> </p>
<table style="border:1px solid black;">  
<colgroup>  
<col width="25%" />  
<col width="25%" />  
<col width="25%" />  
<col width="25%" />  
</colgroup>  
<thead>  
<tr class="header">  
<th>Název</th>  
<th>Typ dat</th>  
<th>Hodnoty NULL</th>  
<th>Popis</th>  
</tr>  
</thead>  
<tbody>  
<tr class="odd">
<td style="border:1px solid black;"><p>RowID</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>Interní index</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>PluginID</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>IDENTITY(100,1) Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>Interní index</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>VersionInfo</p></td>
<td style="border:1px solid black;"><p>nvarchar(64)</p></td>
<td style="border:1px solid black;"><p>Nezadáno</p></td>
<td style="border:1px solid black;"><p>Verze modulu plug-in</p></td>
</tr>  
</tbody>  
</table>
  
DRMS\_PluginProperties  
----------------------
  
V následující tabulce jsou uvedeny informace o vlastnostech modulu plug-in.
  
###  

<p> </p>
<table style="border:1px solid black;">  
<colgroup>  
<col width="25%" />  
<col width="25%" />  
<col width="25%" />  
<col width="25%" />  
</colgroup>  
<thead>  
<tr class="header">  
<th>Název</th>  
<th>Typ dat</th>  
<th>Hodnoty NULL</th>  
<th>Popis</th>  
</tr>  
</thead>  
<tbody>  
<tr class="odd">
<td style="border:1px solid black;"><p>PropertyID</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>IDENTITY(100,1) Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>Interní index</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>PluginID</p></td>
<td style="border:1px solid black;"><p>int (FK)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>ID modulu plug-in, do něhož vlastnost patří</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>PropertyName</p></td>
<td style="border:1px solid black;"><p>nvarchar(256)</p></td>
<td style="border:1px solid black;"><p>Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>Název vlastnosti pro tato konfigurační data</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>PropertyValue</p></td>
<td style="border:1px solid black;"><p>text</p></td>
<td style="border:1px solid black;"><p>Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>Hodnota vlastnosti pro tato konfigurační data</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>DateUpdated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Časové razítko aktualizace</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>DateCreated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Časové razítko vytvoření</p></td>
</tr>  
</tbody>  
</table>
  
DRMS\_PluginType  
----------------
  
V následující tabulce jsou uvedeny informace o typu modulu plug-in.
  
###  

<p> </p>
<table style="border:1px solid black;">  
<colgroup>  
<col width="25%" />  
<col width="25%" />  
<col width="25%" />  
<col width="25%" />  
</colgroup>  
<thead>  
<tr class="header">  
<th>Název</th>  
<th>Typ dat</th>  
<th>Hodnoty NULL</th>  
<th>Popis</th>  
</tr>  
</thead>  
<tbody>  
<tr class="odd">
<td style="border:1px solid black;"><p>PluginTypeID</p></td>
<td style="border:1px solid black;"><p>Int (PK)</p></td>
<td style="border:1px solid black;"><p>Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>Interní index</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>PluginTypeName</p></td>
<td style="border:1px solid black;"><p>nvarchar(256)</p></td>
<td style="border:1px solid black;"><p>Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>Název tohoto modulu plug-in</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>DateUpdated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Časové razítko aktualizace</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>DateCreated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Časové razítko vytvoření</p></td>
</tr>  
</tbody>  
</table>
  
DRMS\_RightsTemplate  
--------------------
  
V následující tabulce jsou uvedeny informace o šablonách zásad práv.
  
###  

<p> </p>
<table style="border:1px solid black;">  
<colgroup>  
<col width="25%" />  
<col width="25%" />  
<col width="25%" />  
<col width="25%" />  
</colgroup>  
<thead>  
<tr class="header">  
<th>Název</th>  
<th>Typ dat</th>  
<th>Hodnoty NULL</th>  
<th>Popis</th>  
</tr>  
</thead>  
<tbody>  
<tr class="odd">
<td style="border:1px solid black;"><p>Guid</p></td>
<td style="border:1px solid black;"><p>nvarchar(128) (PK)</p></td>
<td style="border:1px solid black;"><p>Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>Identifikátor GUID šablony zásad práv</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>TemplateData</p></td>
<td style="border:1px solid black;"><p>ntext</p></td>
<td style="border:1px solid black;"><p>Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>Toto pole obsahuje data šablony XrML.</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>DateUpdated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Časové razítko aktualizace</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>DateCreated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Časové razítko vytvoření</p></td>
</tr>  
</tbody>  
</table>
  
DRMS\_TrustedCertificateAuthorities  
-----------------------------------
  
V následující tabulce jsou uvedeny informace o důvěryhodných certifikačních autoritách.
  
###  

<p> </p>
<table style="border:1px solid black;">  
<colgroup>  
<col width="25%" />  
<col width="25%" />  
<col width="25%" />  
<col width="25%" />  
</colgroup>  
<thead>  
<tr class="header">  
<th>Název</th>  
<th>Typ dat</th>  
<th>Hodnoty NULL</th>  
<th>Popis</th>  
</tr>  
</thead>  
<tbody>  
<tr class="odd">
<td style="border:1px solid black;"><p>ID</p></td>
<td style="border:1px solid black;"><p>Int (PK)</p></td>
<td style="border:1px solid black;"><p>IDENTITY(1,1) Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>Interní index</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>CertificateID</p></td>
<td style="border:1px solid black;"><p>int (FK)</p></td>
<td style="border:1px solid black;"><p>Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>ID certifikátu</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>CertificateGUID</p></td>
<td style="border:1px solid black;"><p>nvarchar(128)</p></td>
<td style="border:1px solid black;"><p>Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>Identifikátor GUID certifikátu</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>CaTypeID</p></td>
<td style="border:1px solid black;"><p>int (FK)</p></td>
<td style="border:1px solid black;"><p>Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>Typ certifikační autority</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>DateUpdated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Časové razítko aktualizace</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>DateCreated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Časové razítko vytvoření</p></td>
</tr>  
</tbody>  
</table>
  
DRMS\_TrustedEmailDomains  
-------------------------
  
V následující tabulce jsou uvedeny informace o e-mailových doménách, které jsou důvěryhodné v prostředí služby RMS.
  
###  

<p> </p>
<table style="border:1px solid black;">  
<colgroup>  
<col width="25%" />  
<col width="25%" />  
<col width="25%" />  
<col width="25%" />  
</colgroup>  
<thead>  
<tr class="header">  
<th>Název</th>  
<th>Typ dat</th>  
<th>Hodnoty NULL</th>  
<th>Popis</th>  
</tr>  
</thead>  
<tbody>  
<tr class="odd">
<td style="border:1px solid black;"><p>ID</p></td>
<td style="border:1px solid black;"><p>Int (PK)</p></td>
<td style="border:1px solid black;"><p>IDENTITY(100,1) Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>Interní index</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>i_TrustedIdentityDomainID</p></td>
<td style="border:1px solid black;"><p>int (FK)t</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Interní index</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>s_EmailDomainName</p></td>
<td style="border:1px solid black;"><p>nvarchar(256)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Seznam názvů e-mailových domén, které jsou platné pro důvěryhodnou doménu uživatelů.</p></td>
</tr>  
</tbody>  
</table>
  
DRMS\_TrustedIdentityDomain  
---------------------------
  
V následující tabulce jsou uvedeny informace o důvěryhodných doménách uživatelů a důvěryhodných doménách publikování.
  
###  

<p> </p>
<table style="border:1px solid black;">  
<colgroup>  
<col width="25%" />  
<col width="25%" />  
<col width="25%" />  
<col width="25%" />  
</colgroup>  
<thead>  
<tr class="header">  
<th>Název</th>  
<th>Typ dat</th>  
<th>Hodnoty NULL</th>  
<th>Popis</th>  
</tr>  
</thead>  
<tbody>  
<tr class="odd">
<td style="border:1px solid black;"><p>i_TrustedIdentityDomainID</p></td>
<td style="border:1px solid black;"><p>Int (PK)</p></td>
<td style="border:1px solid black;"><p>IDENTITY(100,1) Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>Interní index</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>s_DomainType</p></td>
<td style="border:1px solid black;"><p>nvarchar(64)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Typ domény</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>CertGUIDType</p></td>
<td style="border:1px solid black;"><p>nvarchar(64)</p></td>
<td style="border:1px solid black;"><p>Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>Typ identifikátoru GUID certifikátu</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>CertGUID</p></td>
<td style="border:1px solid black;"><p>nvarchar(128)</p></td>
<td style="border:1px solid black;"><p>Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>Identifikátor GUID certifikátu</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>i_CertificateID</p></td>
<td style="border:1px solid black;"><p>int (FK)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>ID certifikátu</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>i_allowSID</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>Identifikátor SID domény</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>S_friendlyname</p></td>
<td style="border:1px solid black;"><p>nvarchar(255)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Popisný název certifikátu</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>dt_DateUpdated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Časové razítko aktualizace</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>dt_DateCreated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Časové razítko vytvoření</p></td>
</tr>  
</tbody>  
</table>
  
DRMS\_XrML\_Certificate  
-----------------------
  
V následující tabulce jsou uvedeny informace o certifikátech serveru pro poskytování licencí XrML, na které odkazuje tabulka DRMS\_LicensorCertificate. Rovněž mapuje řetěz certifikátů.
  
###  

<p> </p>
<table style="border:1px solid black;">  
<colgroup>  
<col width="25%" />  
<col width="25%" />  
<col width="25%" />  
<col width="25%" />  
</colgroup>  
<thead>  
<tr class="header">  
<th>Název</th>  
<th>Typ dat</th>  
<th>Hodnoty NULL</th>  
<th>Popis</th>  
</tr>  
</thead>  
<tbody>  
<tr class="odd">
<td style="border:1px solid black;"><p>i_CertificateID</p></td>
<td style="border:1px solid black;"><p>Int (PK)</p></td>
<td style="border:1px solid black;"><p>IDENTITY(100,1) Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>Ukazatel na skutečný certifikát</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>s_Certificate</p></td>
<td style="border:1px solid black;"><p>ntext</p></td>
<td style="border:1px solid black;"><p>Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>Ukazatel na skutečný certifikát</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>i_ParentCertificateID</p></td>
<td style="border:1px solid black;"><p>int (FK)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Ukazatel na skutečný certifikát</p></td>
</tr>  
</tbody>  
</table>
