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
