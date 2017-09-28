---
TOCTitle: Definice klíčů služby RMS
Title: Definice klíčů služby RMS
ms:assetid: 'b052305c-1db7-434a-bad9-26d704156776'
ms:contentKeyID: 18113469
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747729(v=WS.10)'
---

Definice klíčů služby RMS
=========================

V následující tabulce jsou uvedeny klíče používané v systému služby RMS.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Klíč</th>
<th>Použití</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Serverové klíče</td>
<td style="border:1px solid black;"><strong>Veřejný klíč</strong>
Šifruje klíč obsahu v licenci k publikování, takže pouze server RMS může načíst klíč obsahu a na základě dané licence k publikování vydávat licence k použití.
<strong>Soukromý klíč</strong>
Podepisuje všechny certifikáty a licence, které jsou vydány daným serverem.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Klíče počítače</td>
<td style="border:1px solid black;"><strong>Veřejný klíč</strong>
Šifruje soukromý klíč certifikátu účtu práv.
<strong>Soukromý klíč</strong>
Dešifruje certifikát účtu práv.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Klíče klientských certifikátů pro poskytování licencí</td>
<td style="border:1px solid black;"><strong>Veřejný klíč</strong>
Šifruje symetrický klíč obsahu ve vydávané licenci k publikování.
<strong>Soukromý klíč</strong>
Podepisuje licence k publikování, které jsou vydány lokálně v situaci, kdy uživatel není připojen k síti.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Klíče uživatele</td>
<td style="border:1px solid black;"><strong>Veřejný klíč</strong>
Šifruje klíč obsahu v licenci k použití, takže pomocí této licence může využít obsah chráněný službou RMS pouze určitý uživatel.
<strong>Soukromý klíč</strong>
Umožňuje uživateli využívat obsah chráněný službou RMS.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Klíče obsahu</td>
<td style="border:1px solid black;">Šifruje obsah chráněný službou RMS při publikování autorem.</td>
</tr>
</tbody>
</table>
