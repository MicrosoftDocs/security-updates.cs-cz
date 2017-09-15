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

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Situace</th>
<th>Doporučení</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>Velký počet stolních počítačů využívajících službu RMS</p></td>
<td style="border:1px solid black;"><p>Klientský software Služby správy přístupových práv v systému Microsoft Windows můžete nainstalovat a aktivovat pomocí služby Windows Update, skriptu nebo některého způsobu distribuce softwaru, jako je server SMS (Systems Management Server) nebo zásady skupiny.</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Velký počet požadavků klientů</p></td>
<td style="border:1px solid black;"><p>Distribuci požadavků do celého clusteru můžete zajistit prostřednictvím serveru s vyrovnáváním zatížení, služby Vyrovnávání zatížení sítě nebo vyrovnávání zatížení pomocí hardwarového řešení.</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Dva síťové adaptéry využívající vytváření virtuálních adres IP ke zpracování požadavků z extranetu i intranetu</p></td>
<td style="border:1px solid black;"><p>Zajistěte, aby byla každá registrace DNS umožňující používání virtuální adresy IP v extranetu zároveň provedena pro používání této adresy v intranetu.</p>
<p>Jestliže registraci DNS pro intranet neprovedete, nezdaří se interní požadavky na licence k použití. Pokud nemůžete změnit záznamy o prostředcích DNS, můžete změnit tabulku hostitelů každého serveru v clusteru a namapovat adresu URL daného clusteru na jeho virtuální adresu IP. Registraci DNS je nutné provést před zajištěním služby RMS. Jestliže jste službu RMS již zajistili, je třeba její zajištění zrušit a potom proces zajištění opakovat znovu.</p></td>
</tr>
</tbody>
</table>
