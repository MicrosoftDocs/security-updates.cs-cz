---
TOCTitle: Služba serveru RMS
Title: Služba serveru RMS
ms:assetid: '772d0a89-c9fb-4430-9434-38cd5add1e86'
ms:contentKeyID: 18113334
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747566(v=WS.10)'
---

Služba serveru RMS
==================

Služba serveru je spuštěna pouze na kořenovém clusteru služby RMS. Služba serveru vystavuje požadavek vytvořený klientem pomocí publikování online za účelem získání certifikátu serveru pro poskytování licencí.

Aplikační soubor serverové služby (soubor License.asmx) je uložen ve virtuálním adresáři Certification, který je součástí Internetové informační služby.

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
