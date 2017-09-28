---
TOCTitle: Tabulky databáze protokolování služby RMS
Title: Tabulky databáze protokolování služby RMS
ms:assetid: '7ab2104c-b12d-4807-8a4b-bcabb145ff9b'
ms:contentKeyID: 18113337
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747569(v=WS.10)'
---

Tabulky databáze protokolování služby RMS
=========================================

V této části jsou popsány tabulky databáze protokolování služby RMS.

DRMS\_Log\_Master
-----------------

V následující tabulce je uvedena položka pro každý záznam protokolování.

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
<td style="border:1px solid black;"><p>i_LogID</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>IDENTITY(100,1) Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>Jedinečné ID pro tento záznam protokolování</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>s_HostMachineName</p></td>
<td style="border:1px solid black;"><p>nvarchar(64)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Server, který vytvořil tento záznam</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>s_HostMachineRequestId</p></td>
<td style="border:1px solid black;"><p>nvarchar(64)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>ID požadavku</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>dt_RequestTime</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Datum a čas požadavku</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>s_RequestPath</p></td>
<td style="border:1px solid black;"><p>nvarchar(128)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Cesta URL požadavku</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>s_RequestType</p></td>
<td style="border:1px solid black;"><p>nvarchar(64)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Typ požadavku</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>s_RequestUserAddress</p></td>
<td style="border:1px solid black;"><p>nvarchar(32)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Adresa IP klienta</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>s_RequestUserAgent</p></td>
<td style="border:1px solid black;"><p>nvarchar(128)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Záhlaví identifikačního řetězce prohlížeče klienta</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>s_AuthenticatedState</p></td>
<td style="border:1px solid black;"><p>nvarchar(64)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Stav ověření požadavku</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>s_SecureConnectionState</p></td>
<td style="border:1px solid black;"><p>nvarchar(64)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Ochrana SSL požadavku</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>s_AuthenticatedId</p></td>
<td style="border:1px solid black;"><p>nvarchar(128)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>ID ověřeného uživatele</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>s_ReceivedXrML</p></td>
<td style="border:1px solid black;"><p>ntext</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Kód XrML přijatý v rámci požadavku od klienta</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>s_IssuedXrML</p></td>
<td style="border:1px solid black;"><p>ntext</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Licence XrML vydaná v požadavku</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>s_Metadata</p></td>
<td style="border:1px solid black;"><p>ntext</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Metadata</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>s_SuccessOrFailure</p></td>
<td style="border:1px solid black;"><p>nvarchar(32)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Úspěch nebo neúspěch požadavku</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>s_ErrorInformation</p></td>
<td style="border:1px solid black;"><p>ntext</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Údaje o chybě</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>dt_LogCreateTime</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>Čas vytvoření protokolu</p></td>
</tr>
</tbody>
</table>
  
DRMS\_Log\_Detail  
-----------------
  
V následující tabulce jsou uvedena další data pro záznam protokolování. V této tabulce jsou zpravidla zaznamenávána data XrML.
  
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
<td style="border:1px solid black;"><p>i_LogDetailID</p></td>
<td style="border:1px solid black;"><p>int (PK)</p></td>
<td style="border:1px solid black;"><p>IDENTITY(100,1)</p></td>
<td style="border:1px solid black;"><p>Interní index</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>i_LogID</p></td>
<td style="border:1px solid black;"><p>int (FK)</p></td>
<td style="border:1px solid black;"><p>Nepovoleny hodnoty NULL (FK)</p></td>
<td style="border:1px solid black;"><p>ID nadřazeného záznamu protokolování</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>s_Name</p></td>
<td style="border:1px solid black;"><p>nvarchar(128)</p></td>
<td style="border:1px solid black;"><p>Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>Název vlastnosti</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>s_Value</p></td>
<td style="border:1px solid black;"><p>ntext</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Hodnota vlastnosti</p></td>
</tr>
</tbody>
</table>
  
DRMS\_Log\_Filter  
-----------------
  
V následující tabulce jsou uvedena pole, která zaznamenává služba naslouchání protokolování.
  
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
<td style="border:1px solid black;"><p>i_ID</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>IDENTITY(100,1) Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>Interní index</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>s_FieldName</p></td>
<td style="border:1px solid black;"><p>nvarchar(255)</p></td>
<td style="border:1px solid black;"><p>Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>Název pole</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>s_FieldDescription</p></td>
<td style="border:1px solid black;"><p>nvarchar(1024)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Popis pole</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>i_IsIncluded</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>Nepovoleny hodnoty NULL</p></td>
<td style="border:1px solid black;"><p>Určení, zda je pole protokolováno</p></td>
</tr>
</tbody>
</table>
