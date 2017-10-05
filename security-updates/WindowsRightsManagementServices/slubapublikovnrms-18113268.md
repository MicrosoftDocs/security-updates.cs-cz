---
TOCTitle: Služba publikování RMS
Title: Služba publikování RMS
ms:assetid: '4c0c8fe3-695c-4b2c-a2d3-cab9b52bbb25'
ms:contentKeyID: 18113268
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc720267(v=WS.10)'
---

Služba publikování RMS
======================

Služba publikování, která vydává licence k publikování, je spuštěna na kořenovém clusteru služby RMS a také na každém clusteru vyhrazeném pro správu licencí. Licence k publikování definují zásady, které svazují doručené licence k použití.

Aplikační soubor služby publikování (soubor Publish.asmx) je uložen ve virtuálním adresáři Licensing, který je součástí Internetové informační služby.

V následující tabulce je znázorněn výchozí seznam řízení přístupu k této službě:

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Uživatel nebo skupina</th>
<th style="border:1px solid black;" >Výchozí oprávnění</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Administrators</td>
<td style="border:1px solid black;">Úplné řízení</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">RMS Service Group</td>
<td style="border:1px solid black;">Čtení a spouštění</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">SYSTEM</td>
<td style="border:1px solid black;">Úplné řízení</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Users</td>
<td style="border:1px solid black;">Čtení a spouštění</td>
</tr>
</tbody>
</table>
