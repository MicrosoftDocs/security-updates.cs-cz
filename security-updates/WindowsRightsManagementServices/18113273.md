---
TOCTitle: Správa certifikátů serveru pro poskytování licencí
Title: Správa certifikátů serveru pro poskytování licencí
ms:assetid: '549979ad-13ee-4abc-8281-3e002a5a9561'
ms:contentKeyID: 18113273
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc720272(v=WS.10)'
---

Správa certifikátů serveru pro poskytování licencí
==================================================

Platnost certifikátů serveru pro poskytování licencí končí po uplynutí určené doby, obvykle po jednom roce. Chcete-li certifikát serveru pro poskytování licencí obnovit, musíte se přihlásit jako místní správce. Jestliže tento certifikát obnovujete pro cluster kořenové certifikace, odešle služba RMS požadavek na obnovení certifikátu serveru pro poskytování licencí službě Microsoft Enrollment Services. Pokud certifikát obnovujete pro server správy licencí, odešle služba RMS požadavek na server kořenové certifikace, který certifikát s končící platností vydal.

Existují tři události, které služba RMS odešle do protokolu systémových událostí a které by měly být sledovány. Tyto události slouží k oznámení, že certifikátu serveru pro poskytování licencí končí nebo skončila platnost. V následující tabulce jsou uvedeny ID a názvy těchto událostí.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >ID události</th>
<th style="border:1px solid black;" >Název události</th>
<th style="border:1px solid black;" >Typ události</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">16</td>
<td style="border:1px solid black;">LicensorCertExpiresInOneMonthEvent</td>
<td style="border:1px solid black;">Upozornění. Služba nadále funguje normálně.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">17</td>
<td style="border:1px solid black;">LicensorCertExpiresInOneWeekEvent</td>
<td style="border:1px solid black;">Upozornění. Služba nadále funguje normálně.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">18</td>
<td style="border:1px solid black;">LicensorCertExpiredEvent</td>
<td style="border:1px solid black;">Chyba. Služba je zakázána.</td>
</tr>
</tbody>
</table>
