---
TOCTitle: Služba certifikace účtů RMS
Title: Služba certifikace účtů RMS
ms:assetid: 'fb294969-850e-44b4-8f6a-ca5d5cec1bf1'
ms:contentKeyID: 18113549
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747802(v=WS.10)'
---

Služba certifikace účtů RMS
===========================

Služba certifikace je spuštěna pouze na kořenovém clusteru. Služba certifikace účtů vytváří certifikáty účtů práv, které spojují uživatelské účty s určitými počítači. Certifikát účtu práv umožňuje uživateli publikovat nebo využívat obsah chráněný právy v určitém počítači.

Aplikační soubor služby certifikace účtů (soubor Certification.asmx) je uložen ve virtuálním adresáři Certification, který je součástí Internetové informační služby.

V následující tabulce je znázorněn výchozí seznam řízení přístupu k této službě:

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
