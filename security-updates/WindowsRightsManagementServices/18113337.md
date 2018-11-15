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
<td style="border:1px solid black;">i_LogID</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">IDENTITY(100,1) Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">Jedinečné ID pro tento záznam protokolování</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_HostMachineName</td>
<td style="border:1px solid black;">nvarchar(64)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Server, který vytvořil tento záznam</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">s_HostMachineRequestId</td>
<td style="border:1px solid black;">nvarchar(64)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">ID požadavku</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">dt_RequestTime</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Datum a čas požadavku</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">s_RequestPath</td>
<td style="border:1px solid black;">nvarchar(128)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Cesta URL požadavku</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_RequestType</td>
<td style="border:1px solid black;">nvarchar(64)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Typ požadavku</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">s_RequestUserAddress</td>
<td style="border:1px solid black;">nvarchar(32)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Adresa IP klienta</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_RequestUserAgent</td>
<td style="border:1px solid black;">nvarchar(128)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Záhlaví identifikačního řetězce prohlížeče klienta</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">s_AuthenticatedState</td>
<td style="border:1px solid black;">nvarchar(64)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Stav ověření požadavku</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_SecureConnectionState</td>
<td style="border:1px solid black;">nvarchar(64)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Ochrana SSL požadavku</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">s_AuthenticatedId</td>
<td style="border:1px solid black;">nvarchar(128)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">ID ověřeného uživatele</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_ReceivedXrML</td>
<td style="border:1px solid black;">ntext</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Kód XrML přijatý v rámci požadavku od klienta</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">s_IssuedXrML</td>
<td style="border:1px solid black;">ntext</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Licence XrML vydaná v požadavku</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_Metadata</td>
<td style="border:1px solid black;">ntext</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Metadata</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">s_SuccessOrFailure</td>
<td style="border:1px solid black;">nvarchar(32)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Úspěch nebo neúspěch požadavku</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_ErrorInformation</td>
<td style="border:1px solid black;">ntext</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Údaje o chybě</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">dt_LogCreateTime</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">Čas vytvoření protokolu</td>
</tr>
</tbody>
</table>
  
DRMS\_Log\_Detail  
-----------------
  
V následující tabulce jsou uvedena další data pro záznam protokolování. V této tabulce jsou zpravidla zaznamenávána data XrML.
  
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
<td style="border:1px solid black;">i_LogDetailID</td>
<td style="border:1px solid black;">int (PK)</td>
<td style="border:1px solid black;">IDENTITY(100,1)</td>
<td style="border:1px solid black;">Interní index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">i_LogID</td>
<td style="border:1px solid black;">int (FK)</td>
<td style="border:1px solid black;">Nepovoleny hodnoty NULL (FK)</td>
<td style="border:1px solid black;">ID nadřazeného záznamu protokolování</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">s_Name</td>
<td style="border:1px solid black;">nvarchar(128)</td>
<td style="border:1px solid black;">Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">Název vlastnosti</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_Value</td>
<td style="border:1px solid black;">ntext</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Hodnota vlastnosti</td>
</tr>
</tbody>
</table>
  
DRMS\_Log\_Filter  
-----------------
  
V následující tabulce jsou uvedena pole, která zaznamenává služba naslouchání protokolování.
  
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
<td style="border:1px solid black;">i_ID</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">IDENTITY(100,1) Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">Interní index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_FieldName</td>
<td style="border:1px solid black;">nvarchar(255)</td>
<td style="border:1px solid black;">Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">Název pole</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">s_FieldDescription</td>
<td style="border:1px solid black;">nvarchar(1024)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Popis pole</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">i_IsIncluded</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Nepovoleny hodnoty NULL</td>
<td style="border:1px solid black;">Určení, zda je pole protokolováno</td>
</tr>
</tbody>
</table>
