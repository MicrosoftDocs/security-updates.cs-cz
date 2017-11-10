---
TOCTitle: Plánování požadavků spojených s clustery pro službu RMS
Title: Plánování požadavků spojených s clustery pro službu RMS
ms:assetid: 'ec4023eb-4d39-4551-9789-c8a2d973a55b'
ms:contentKeyID: 18113542
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747792(v=WS.10)'
---

Plánování požadavků spojených s clustery pro službu RMS
=======================================================

Pokud službu RMS používáte v clusterovém nasazení, nezapomeňte určit způsob řešení následujících situací, se kterými se můžete v organizaci setkat.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Situace</th>
<th style="border:1px solid black;" >Doporučení</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Velký počet stolních počítačů využívajících službu RMS</td>
<td style="border:1px solid black;">Klientský software Služby správy přístupových práv v systému Microsoft Windows můžete nainstalovat a aktivovat pomocí služby Windows Update, skriptu nebo některého způsobu distribuce softwaru, jako je server SMS (Systems Management Server) nebo zásady skupiny.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Velký počet požadavků klientů</td>
<td style="border:1px solid black;">Distribuci požadavků do celého clusteru můžete zajistit prostřednictvím serveru s vyrovnáváním zatížení, služby Vyrovnávání zatížení sítě nebo vyrovnávání zatížení pomocí hardwarového řešení.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Dva síťové adaptéry využívající vytváření virtuálních adres IP ke zpracování požadavků z extranetu i intranetu</td>
<td style="border:1px solid black;">Zajistěte, aby byla každá registrace DNS umožňující používání virtuální adresy IP v extranetu zároveň provedena pro používání této adresy v intranetu.  
<br/><br/>
Jestliže registraci DNS pro intranet neprovedete, nezdaří se interní požadavky na licence k použití. Pokud nemůžete změnit záznamy o prostředcích DNS, můžete změnit tabulku hostitelů každého serveru v clusteru a namapovat adresu URL daného clusteru na jeho virtuální adresu IP. Registraci DNS je nutné provést před zajištěním služby RMS. Jestliže jste službu RMS již zajistili, je třeba její zajištění zrušit a potom proces zajištění opakovat znovu.</td>
</tr>
</tbody>
</table>
