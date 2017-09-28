---
TOCTitle: Služba lokátoru služeb RMS
Title: Služba lokátoru služeb RMS
ms:assetid: '6f410cc9-5d5b-4df3-bf4f-7b13811eb52f'
ms:contentKeyID: 18113315
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747548(v=WS.10)'
---

Služba lokátoru služeb RMS
==========================

Služba lokátoru služeb je spuštěna na kořenových clusterech služby RMS i na clusterech vyhrazených pro správu licencí. Tato služba poskytuje adresu URL připojení služeb ke službě Active Directory určenou pro cluster, aby ji mohli rozpoznat klienti s podporou služby RMS.

Aplikační soubor služby lokátoru služeb (soubor ServiceLocator.asmx) je umístěn ve virtuálních adresářích Certification a Licensing služby IIS.

V následující tabulce je znázorněn výchozí seznam řízení přístupu k této službě:

###  

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Uživatel nebo skupina</th>
<th>Výchozí oprávnění</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>Administrators</p></td>
<td style="border:1px solid black;"><p>Úplné řízení</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>RMS Service Group</p></td>
<td style="border:1px solid black;"><p>Čtení a spouštění</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>SYSTEM</p></td>
<td style="border:1px solid black;"><p>Úplné řízení</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Users</p></td>
<td style="border:1px solid black;"><p>Čtení a spouštění</p></td>
</tr>
</tbody>
</table>
