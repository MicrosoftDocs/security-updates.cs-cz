---
TOCTitle: Služba správy RMS
Title: Služba správy RMS
ms:assetid: '4bd3e142-f0f6-40e9-a160-deab28ce5b88'
ms:contentKeyID: 18113306
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747560(v=WS.10)'
---

Služba správy RMS
=================

Služba správy je spuštěna na kořenovém clusteru služby RMS a také na každém clusteru správy licencí. Služba správy je hostitelem webu správy a umožňuje spravovat službu RMS.

Aplikační soubor služby správy (soubor Default.aspx) je umístěn ve virtuálním adresáři Admin: *web služby RMS*\\\_wmcs\\Admin, kde je položka *web služby RMS* nahrazena názvem webu, na kterém jste zajistili službu RMS.

V následující tabulce je znázorněn výchozí seznam řízení přístupu k této službě:

###  

 
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
</tbody>
</table>
