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
<td style="border:1px solid black;"><p>i_MachineId</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>IDENTITY(1,1) Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>Interní index</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>b_PubKeyHash</p></td>
<td style="border:1px solid black;"><p>binary(20)</p></td>
<td style="border:1px solid black;"><p>(20) Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>Hodnota hash ID hardwaru</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>dt_CreateDate</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>Datum a čas, kdy byla položka přidána do tabulky</p></td>
</tr>  
</tbody>  
</table>
  
UD\_PassportAuthIdentities  
--------------------------
  
V následující tabulce jsou uvedeny informace o informacích služby Microsoft® .NET Passport pro uživatele.
  
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
<td style="border:1px solid black;"><p>i_UserId</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>Interní index</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>i64_Puid</p></td>
<td style="border:1px solid black;"><p>bigint</p></td>
<td style="border:1px solid black;"><p>(50) NULL</p></td>
<td style="border:1px solid black;"><p>ID uživatele služby .NET Passport</p></td>
</tr>  
</tbody>  
</table>
  
UD\_UserMachine  
---------------
  
V následující tabulce jsou certifikovaní uživatelé propojeni s odpovídajícími informacemi o počítačích.
  
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
<td style="border:1px solid black;"><p>i_MachineId</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>Interní index</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>i_UserId</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>Interní index</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>dt_CreateDate</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>Datum a čas, kdy byla položka přidána do tabulky</p></td>
</tr>  
</tbody>  
</table>
  
UD\_Users  
---------
  
V následující tabulce jsou uvedeny informace o uživatelských datech.
  
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
<td style="border:1px solid black;"><p>i_UserId</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>IDENTITY(1,1) Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>Interní index</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>b_KeyData</p></td>
<td style="border:1px solid black;"><p>varbinary(2000)</p></td>
<td style="border:1px solid black;"><p>(2000) Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>Šifrovaný veřejný/soukromý klíč uživatele</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>i_KeyDataLength</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>Délka nešifrovaného veřejného/soukromého klíče</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>b_PublicKey</p></td>
<td style="border:1px solid black;"><p>PublicKey</p></td>
<td style="border:1px solid black;"><p>Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>Veřejný klíč uživatele</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>i_EncryptionDbId</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>Index certifikátu poskytovatele licence k šifrování páru veřejného a soukromého klíče</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>s_Certificate</p></td>
<td style="border:1px solid black;"><p>ntext</p></td>
<td style="border:1px solid black;"><p>Nezadáno</p></td>
<td style="border:1px solid black;"><p>Nepoužito</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>dt_Expiration</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>Datum vypršení platnosti uživatelského klíče</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>dt_TemporaryExpiration</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>Datum a čas vypršení platnosti dočasného použití klíče</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>f_Modified</p></td>
<td style="border:1px solid black;"><p>bit</p></td>
<td style="border:1px solid black;"><p>Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>Nepoužito</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>i_Quota</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>Aktuální úroveň kvóty pro uživatele</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>i_WaitDays</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>Počet dní do úspěšného splnění žádostí o další kvótu</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>dt_LastConsumption</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>Datum a čas poslední dodatečné certifikace uživatele</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>dt_CreateDate</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>Datum a čas, kdy byla položka přidána do tabulky</p></td>
</tr>  
</tbody>  
</table>
  
UD\_Windows AuthIdentities  
--------------------------
  
V následující tabulce jsou uvedena ID všech ověřených a certifikovaných uživatelů v systému Windows.
  
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
<td style="border:1px solid black;"><p>i_UserId</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>Interní index</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>s_Sid</p></td>
<td style="border:1px solid black;"><p>Sid</p></td>
<td style="border:1px solid black;"><p>Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>ID zabezpečení (SID) uživatele</p></td>
</tr>  
</tbody>  
</table>
