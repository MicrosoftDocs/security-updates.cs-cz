---
TOCTitle: Certifikační tabulky konfigurační databáze služby RMS
Title: Certifikační tabulky konfigurační databáze služby RMS
ms:assetid: 'd392663a-1a46-42f6-a71d-f0f2c1843566'
ms:contentKeyID: 18113519
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747760(v=WS.10)'
---

Certifikační tabulky konfigurační databáze služby RMS
=====================================================

V tomto tématu jsou popsány certifikační tabulky, které obsahuje konfigurační databáze služby RMS. Tabulky obsahují informace o certifikátech účtů práv, které jsou vydány pro uživatele této instalace.

UD\_Machines
------------

V následující tabulce jsou uvedeny informace o ID hardwaru pro všechny počítače.

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
<th>Název</th>
<th>Typ dat</th>
<th>Hodnoty NULL</th>
<th>Popis</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">i_MachineId</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">IDENTITY(1,1) Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">Interní index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">b_PubKeyHash</td>
<td style="border:1px solid black;">binary(20)</td>
<td style="border:1px solid black;">(20) Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">Hodnota hash ID hardwaru</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">dt_CreateDate</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">Datum a čas, kdy byla položka přidána do tabulky</td>
</tr>
</tbody>
</table>
  
UD\_PassportAuthIdentities  
--------------------------
  
V následující tabulce jsou uvedeny informace o informacích služby Microsoft® .NET Passport pro uživatele.
  
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
<th>Název</th>
<th>Typ dat</th>
<th>Hodnoty NULL</th>
<th>Popis</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">i_UserId</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">Interní index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">i64_Puid</td>
<td style="border:1px solid black;">bigint</td>
<td style="border:1px solid black;">(50) NULL</td>
<td style="border:1px solid black;">ID uživatele služby .NET Passport</td>
</tr>
</tbody>
</table>
  
UD\_UserMachine  
---------------
  
V následující tabulce jsou certifikovaní uživatelé propojeni s odpovídajícími informacemi o počítačích.
  
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
<th>Název</th>
<th>Typ dat</th>
<th>Hodnoty NULL</th>
<th>Popis</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">i_MachineId</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">Interní index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">i_UserId</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">Interní index</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">dt_CreateDate</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">Datum a čas, kdy byla položka přidána do tabulky</td>
</tr>
</tbody>
</table>
  
UD\_Users  
---------
  
V následující tabulce jsou uvedeny informace o uživatelských datech.
  
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
<th>Název</th>
<th>Typ dat</th>
<th>Hodnoty NULL</th>
<th>Popis</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">i_UserId</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">IDENTITY(1,1) Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">Interní index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">b_KeyData</td>
<td style="border:1px solid black;">varbinary(2000)</td>
<td style="border:1px solid black;">(2000) Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">Šifrovaný veřejný/soukromý klíč uživatele</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">i_KeyDataLength</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">Délka nešifrovaného veřejného/soukromého klíče</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">b_PublicKey</td>
<td style="border:1px solid black;">PublicKey</td>
<td style="border:1px solid black;">Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">Veřejný klíč uživatele</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">i_EncryptionDbId</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">Index certifikátu poskytovatele licence k šifrování páru veřejného a soukromého klíče</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_Certificate</td>
<td style="border:1px solid black;">ntext</td>
<td style="border:1px solid black;">Nezadáno</td>
<td style="border:1px solid black;">Nepoužito</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">dt_Expiration</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">Datum vypršení platnosti uživatelského klíče</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">dt_TemporaryExpiration</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">Datum a čas vypršení platnosti dočasného použití klíče</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">f_Modified</td>
<td style="border:1px solid black;">bit</td>
<td style="border:1px solid black;">Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">Nepoužito</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">i_Quota</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">Aktuální úroveň kvóty pro uživatele</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">i_WaitDays</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">Počet dní do úspěšného splnění žádostí o další kvótu</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">dt_LastConsumption</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">Datum a čas poslední dodatečné certifikace uživatele</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">dt_CreateDate</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">Datum a čas, kdy byla položka přidána do tabulky</td>
</tr>
</tbody>
</table>
  
UD\_Windows AuthIdentities  
--------------------------
  
V následující tabulce jsou uvedena ID všech ověřených a certifikovaných uživatelů v systému Windows.
  
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
<th>Název</th>
<th>Typ dat</th>
<th>Hodnoty NULL</th>
<th>Popis</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">i_UserId</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">Interní index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_Sid</td>
<td style="border:1px solid black;">Sid</td>
<td style="border:1px solid black;">Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">ID zabezpečení (SID) uživatele</td>
</tr>
</tbody>
</table>
