---
TOCTitle: Souhrn certifikátů a licencí služby RMS
Title: Souhrn certifikátů a licencí služby RMS
ms:assetid: '637ccfca-318e-4346-85b5-0945b058fb9c'
ms:contentKeyID: 18113339
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747595(v=WS.10)'
---

Souhrn certifikátů a licencí služby RMS
=======================================

Následující tabulka obsahuje certifikáty a licence používané službou RMS. Jejich podrobný popis najdete ve zbývajících tématech tohoto oddílu.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th>Certifikát nebo licence</th>
<th>Účel</th>
<th>Obsah</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Certifikáty serveru pro poskytování licencí</td>
<td style="border:1px solid black;">Certifikát serveru pro poskytování licencí vydaný serverům správy licencí zajišťuje práva k vydání následujících objektů:
<ul>
<li>Licence k publikování<br />
<br />
</li>
<li>Licence k použití<br />
<br />
</li>
<li>Klientské certifikáty pro poskytování licencí<br />
<br />
</li>
<li>Šablony zásad práv<br />
<br />
</li>
</ul>
Certifikát serveru pro poskytování licencí vydaný clusteru kořenové certifikace zajišťuje práva k vydání následujících objektů:
<ul>
<li>Certifikáty účtů práv pro klienty<br />
<br />
</li>
<li>Certifikáty serveru pro poskytování licencí pro servery správy licencí<br />
<br />
</li>
</ul></td>
<td style="border:1px solid black;">Certifikát serveru pro poskytování licencí vydaný serveru správy licencí obsahuje veřejný klíč serveru správy licencí.
Certifikát serveru pro poskytování licencí vydaný serveru kořenové certifikace obsahuje veřejný klíč serveru kořenové certifikace.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Klientské certifikáty pro poskytování licencí</td>
<td style="border:1px solid black;">Udělují uživateli právo publikovat obsah chráněný službou RMS bez připojení k podnikové síti.</td>
<td style="border:1px solid black;">Obsahují veřejný klíč certifikátu a soukromý klíč certifikátu šifrovaný veřejným klíčem uživatele, který si certifikát vyžádal. Obsahují také veřejný klíč serveru, který vydal certifikát.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Certifikáty počítače RMS</td>
<td style="border:1px solid black;">Určují počítač nebo zařízení, které jsou systémem služby RMS považovány za důvěryhodné.</td>
<td style="border:1px solid black;">Obsahují veřejný klíč aktivovaného počítače. Odpovídající soukromý klíč je obsažen v bezpečnostním modulu daného počítače.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Certifikáty účtů práv</td>
<td style="border:1px solid black;">Identifikují uživatele v kontextu určitého počítače nebo zařízení.</td>
<td style="border:1px solid black;">Obsahují veřejný klíč uživatele a soukromý klíč uživatele, které jsou šifrovány veřejným klíčem aktivovaného počítače.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Licence k publikování</td>
<td style="border:1px solid black;">Zadejte práva, která se vztahují na obsah chráněný službou RMS.</td>
<td style="border:1px solid black;">Obsahují symetrický klíč obsahu umožňující dešifrování obsahu šifrovaného pomocí veřejného klíče serveru, který danou licenci vydal.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Licence k použití</td>
<td style="border:1px solid black;">Zadejte práva, která se vztahují na daný obsah chráněný službou RMS v kontextu konkrétního ověřeného uživatele.</td>
<td style="border:1px solid black;">Obsahují symetrický klíč pro dešifrování obsahu, který je šifrován veřejným klíčem uživatele.</td>
</tr>
</tbody>
</table>
