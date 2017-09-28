---
TOCTitle: Zobrazení souborů protokolu
Title: Zobrazení souborů protokolu
ms:assetid: '2dc9ed54-76d8-4721-ba93-194845de726a'
ms:contentKeyID: 18113391
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc720228(v=WS.10)'
---

Zobrazení souborů protokolu
===========================

V závislosti na způsobu nasazení služby RMS jsou soubory protokolu uloženy na databázovém serveru v databázi serveru SQL Server nebo v databázi součásti Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) verze A. Vytvořením filtrů můžete omezit informace ukládané do souborů protokolu. Postup při jejich vytváření naleznete v nápovědě správce SQL Server Enterprise Manager.

Velikost typické položky protokolu je zhruba 300 bajtů. Popis zaznamenaných polí je uveden v následující tabulce.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Pole</th>
<th>Popis</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">HostMachineName</td>
<td style="border:1px solid black;">Počítač, který zpracovával požadavek.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">HostMachineRequestId</td>
<td style="border:1px solid black;">Jedinečný identifikátor požadavku v tomto počítači. Kombinace hodnot z polí HostMachineName a HostMachineRequestId jednoznačně identifikuje požadavek v rámci clusteru.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">RequestTime</td>
<td style="border:1px solid black;">Čas přijetí požadavku (střední čas, GMT).</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">RequestPath</td>
<td style="border:1px solid black;">Relativní adresa URL souboru s příponou ASMX, například: /_wmcs/licensing/License.asmx.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">RequestType</td>
<td style="border:1px solid black;">Název spuštěné webové metody, například: AcquireLicense.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">RequestUserAddress</td>
<td style="border:1px solid black;">Adresa IP zdroje žadatele.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">RequestUserAgent</td>
<td style="border:1px solid black;">Hodnota identifikačního řetězce prohlížeče v hlavičce protokolu HTTP.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">AuthenticatedState</td>
<td style="border:1px solid black;">Informace o tom, zda bylo připojení HTTP ověřeno (True/False).</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">SecureConnectionState</td>
<td style="border:1px solid black;">Informace o tom, zda se jedná o připojení SSL (True/False).</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">AuthenticatedId</td>
<td style="border:1px solid black;">Přihlašovací jméno pro ověřené požadavky. Pokud AuthenticatedState=False, je toto pole prázdné.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">ReceivedXrMLDocument</td>
<td style="border:1px solid black;">Dokument XrML přijatý od žadatele.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">ReceivedXrMLDocumentIssuerChain</td>
<td style="border:1px solid black;">Řetězec vydavatele pro přijatý dokument XrML.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">IssuedXrMLDocument</td>
<td style="border:1px solid black;">Dokument XrML vrácený žadateli.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">IssuedXrMLDocumentIssuerChain</td>
<td style="border:1px solid black;">Řetězec vydavatele pro vydaný dokument XrML.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">SuccessOrFailure</td>
<td style="border:1px solid black;">Informace o tom, zda byl požadavek úspěšný či nikoli (Succeeded/Failed).</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Metadata</td>
<td style="border:1px solid black;">Pole metadat.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">ErrorInformation</td>
<td style="border:1px solid black;">Zpráva s popisem chyby, došlo-li k chybě.</td>
</tr>
</tbody>
</table>
