---
TOCTitle: Služba správy licencí RMS
Title: Služba správy licencí RMS
ms:assetid: '5cad1baf-0304-4e82-b62d-83a4aac2140b'
ms:contentKeyID: 18113285
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc720278(v=WS.10)'
---

Služba správy licencí RMS
=========================

Služba správy licencí, která vydává licence k použití, je spuštěna na kořenovém clusteru služby RMS a také na každém clusteru vyhrazeném pro správu licencí. Licence k použití uživatelům umožňují využívat obsah chráněný právy.

Aplikační soubor služby správy licencí (soubor License.asmx) je uložen ve virtuálním adresáři Licensing, který je součástí Internetové informační služby.

| ![](images/Cc720278.note(WS.10).gif)Poznámka                                                                                                                                                                                                                                                                                                                                                                            |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Můžete nasadit samostatný cluster vyhrazený pro správu licencí, který kořenovému clusteru odebere zatížení způsobené požadavky na licencování. Je také možné implementovat samostatný server nebo cluster správy licencí pro oddělení, například pro oddělení, které definuje vlastní zásady práv. Další informace o těchto aspektech najdete v části Určení hlavních součástí v tématu Plánování a architektura služby RMS v této sadě dokumentace. |

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
