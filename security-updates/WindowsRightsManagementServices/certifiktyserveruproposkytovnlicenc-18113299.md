---
TOCTitle: Certifikáty serveru pro poskytování licencí
Title: Certifikáty serveru pro poskytování licencí
ms:assetid: '0b35fbcd-25a9-4587-898d-9a30fd1d3c5b'
ms:contentKeyID: 18113299
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc720184(v=WS.10)'
---

Certifikáty serveru pro poskytování licencí
===========================================

Certifikát serveru pro poskytování licencí uděluje serveru RMS právo vydávat certifikáty a licence. Jakmile je dokončeno zajišťování prvního serveru kořenové certifikace nasazení služby RMS, je tomuto serveru službou Microsoft Enrollment Services odeslán certifikát serveru pro poskytování licencí. Tento proces se nazývá zápis. Tento certifikát obsahuje veřejný klíč serveru kořenové certifikace a je podepsán soukromým klíčem služby zápisu. Další servery přidané do clusteru kořenové certifikace tento certifikát sdílí.

První server správy licencí v clusteru získá během zajišťování certifikát serveru pro poskytování licencí od serveru nebo clusteru kořenové certifikace služby RMS při procesu, kterému se říká dílčí zápis. Tento certifikát obsahuje veřejný klíč serveru správy licencí a je podepsán soukromým klíčem serveru nebo clusteru kořenové certifikace. Ostatní servery, které jsou přidány do clusteru správy licencí, sdílejí tento certifikát.

Seznam práv, které jsou uděleny serverům certifikáty poskytovatele licence serveru, jsou uvedeny v následující tabulce.

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
<th>Objekt, pro jehož vydání jsou přidělena práva</th>
<th>Certifikát poskytovatele licence serveru, který je vydán serveru kořenové certifikace</th>
<th>Certifikát poskytovatele licence serveru, který je vydán serveru správy licencí</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>Certifikáty účtů práv</p></td>
<td style="border:1px solid black;"><p>Ano</p></td>
<td style="border:1px solid black;"><p>Ne</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Licence k publikování</p></td>
<td style="border:1px solid black;"><p>Ano</p></td>
<td style="border:1px solid black;"><p>Ano</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Licence k použití</p></td>
<td style="border:1px solid black;"><p>Ano</p></td>
<td style="border:1px solid black;"><p>Ano</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Podřízené certifikáty serveru pro poskytování licencí</p></td>
<td style="border:1px solid black;"><p>Ano</p></td>
<td style="border:1px solid black;"><p>Ne</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Klientské certifikáty pro poskytování licencí</p></td>
<td style="border:1px solid black;"><p>Ano</p></td>
<td style="border:1px solid black;"><p>Ano</p></td>
</tr>  
</tbody>  
</table>
  
| ![](images/Cc720184.note(WS.10).gif)Poznámka                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |  
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Služba RMS nevyžaduje zvláštní servery nebo clustery správy licencí, ale tyto servery nebo clustery mohou převzít požadavky na licence z clusteru kořenové certifikace. Správci mohou také nastavit servery správy licencí tak, aby vyhovovaly interním požadavkům podniku, například přímé kontrole nad publikováním chráněného obsahu. Obecné zásady podniku, které jsou implementovány v šablonách zásad práv pro server nebo cluster kořenové certifikace, například neurčují některá práva, která vyžaduje určité oddělení. V takovém případě může oddělení implementovat samostatný server nebo cluster správy licencí, který umožní uložení šablon zásad práv a zpracování požadavků na licence. |
