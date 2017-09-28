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

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th>ID události</th>
<th>Název události</th>
<th>Typ události</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>16</p></td>
<td style="border:1px solid black;"><p>LicensorCertExpiresInOneMonthEvent</p></td>
<td style="border:1px solid black;"><p>Upozornění. Služba nadále funguje normálně.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>17</p></td>
<td style="border:1px solid black;"><p>LicensorCertExpiresInOneWeekEvent</p></td>
<td style="border:1px solid black;"><p>Upozornění. Služba nadále funguje normálně.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>18</p></td>
<td style="border:1px solid black;"><p>LicensorCertExpiredEvent</p></td>
<td style="border:1px solid black;"><p>Chyba. Služba je zakázána.</p></td>
</tr>
</tbody>
</table>
