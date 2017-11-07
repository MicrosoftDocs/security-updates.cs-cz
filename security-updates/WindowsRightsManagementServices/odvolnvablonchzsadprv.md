---
TOCTitle: Odvolání v šablonách zásad práv
Title: Odvolání v šablonách zásad práv
ms:assetid: '287c5b92-fcb5-4295-9c2b-4e37e643beb2'
ms:contentKeyID: 18113245
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc720226(v=WS.10)'
---

Odvolání v šablonách zásad práv
===============================

V šablonách zásad práv jsou určeny podmínky odvolání. Hodnoty podmínek odvolání zadané v šabloně zásad práv jsou zaznamenány pomocí značky REFRESH jazyka XrML v licenci k publikování vydané na základě dané šablony. Výsledná licence k použití vydaná serverem bude též obsahovat značku REFRESH.

V následující tabulce jsou uvedeny parametry zaznamenané pomocí značky REFRESH.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Parametr</th>
<th style="border:1px solid black;" >Popis</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">ID</td>
<td style="border:1px solid black;">ID seznamu odvolání.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">ADDRESS</td>
<td style="border:1px solid black;">Adresa URL nebo cesta UNC, kde lze získat seznam odvolání.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">PUBLICKEY</td>
<td style="border:1px solid black;">Veřejný klíč vydavatele seznamu odvolání. Tento veřejný klíč odpovídá soukromému klíči použitému k podpisu seznamu odvolání.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">INTERVALTIME</td>
<td style="border:1px solid black;">Maximální stáří seznamu odvolání uvedené ve dnech. Pokud je seznam odvolání v mezipaměti starší než doba povolená hodnotou INTERVALTIME, získá klient RMS nejnovější seznam odvolání z adresy URL uvedené v hodnotě ADDRESS. Tímto způsobem je zajištěno použití aktuálního seznamu odvolání.</td>
</tr>
</tbody>
</table>
  
Další informace o vytvoření šablon zásad práv získáte v této sadě dokumentace v části Vytvoření a změna šablon zásad práv tématu Provoz serveru RMS.
