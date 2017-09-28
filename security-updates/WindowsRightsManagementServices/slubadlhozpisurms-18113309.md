---
TOCTitle: Služba dílčího zápisu RMS
Title: Služba dílčího zápisu RMS
ms:assetid: '6b05e71c-5e7d-467c-9e13-35ac14d3718a'
ms:contentKeyID: 18113309
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc720289(v=WS.10)'
---

Služba dílčího zápisu RMS
=========================

Služba dílčího zápisu je spuštěna pouze na kořenovém clusteru služby RMS. Odpovídá na požadavky na certifikáty serveru pro poskytování licencí, které jsou při zajišťování odesílány servery clusterů vyhrazených pro správu licencí.

Aplikační soubor služby dílčího zápisu (soubor SubEnrollService.asmx) je umístěn ve virtuálním adresáři Certification: *web\_služby\_RMS*\\\_wmcs\\Certification\\, kde položka *web\_služby\_RMS* je nahrazena názvem webu, na kterém jste zajistili službu RMS.

Ve výchozím nastavení je přístup k této službě omezen na účet SYSTEM v místním počítači. Chcete-li zajistit a zapsat podřízený server v clusteru vyhrazeném pro správu licencí, musí být uživatelský účet správce serveru poskytujícího licenci přidán do volitelného seznamu přístupu SubEnrollService.asmx s oprávněním pro úplné řízení.

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
<td style="border:1px solid black;"><p>SYSTEM</p></td>
<td style="border:1px solid black;"><p>Úplné řízení</p></td>
</tr>
</tbody>
</table>
