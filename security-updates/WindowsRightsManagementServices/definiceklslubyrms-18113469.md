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

<p> </p>
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
<td style="border:1px solid black;"><p>Serverové klíče</p></td>
<td style="border:1px solid black;"><p><strong>Veřejný klíč</strong></p>
<p>Šifruje klíč obsahu v licenci k publikování, takže pouze server RMS může načíst klíč obsahu a na základě dané licence k publikování vydávat licence k použití.</p>
<p><strong>Soukromý klíč</strong></p>
<p>Podepisuje všechny certifikáty a licence, které jsou vydány daným serverem.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Klíče počítače</p></td>
<td style="border:1px solid black;"><p><strong>Veřejný klíč</strong></p>
<p>Šifruje soukromý klíč certifikátu účtu práv.</p>
<p><strong>Soukromý klíč</strong></p>
<p>Dešifruje certifikát účtu práv.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Klíče klientských certifikátů pro poskytování licencí</p></td>
<td style="border:1px solid black;"><p><strong>Veřejný klíč</strong></p>
<p>Šifruje symetrický klíč obsahu ve vydávané licenci k publikování.</p>
<p><strong>Soukromý klíč</strong></p>
<p>Podepisuje licence k publikování, které jsou vydány lokálně v situaci, kdy uživatel není připojen k síti.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Klíče uživatele</p></td>
<td style="border:1px solid black;"><p><strong>Veřejný klíč</strong></p>
<p>Šifruje klíč obsahu v licenci k použití, takže pomocí této licence může využít obsah chráněný službou RMS pouze určitý uživatel.</p>
<p><strong>Soukromý klíč</strong></p>
<p>Umožňuje uživateli využívat obsah chráněný službou RMS.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Klíče obsahu</p></td>
<td style="border:1px solid black;"><p>Šifruje obsah chráněný službou RMS při publikování autorem.</p></td>
</tr>
</tbody>
</table>
