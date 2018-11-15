---
TOCTitle: Přehled systému služby RMS
Title: Přehled systému služby RMS
ms:assetid: 'cbd14635-e17e-42b8-9fd8-6fdce42ffe07'
ms:contentKeyID: 18113439
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747671(v=WS.10)'
---

Přehled systému služby RMS
==========================

Toto téma obsahuje informace o vzájemné spolupráci webových služeb RMS a technologií klientů RMS v systému služby RMS.

V následující tabulce jsou uvedeny typy serverů zahrnutých do nasazení služby RMS a popis jejich funkcí. Podrobné informace o nasazení získáte v této sadě dokumentace v tématu Nasazení systému služby RMS.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Server nebo cluster</th>
<th style="border:1px solid black;" >Funkce</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Kořenová certifikace</td>
<td style="border:1px solid black;">Spustí následující služby RMS:
<ul>
<li><strong>Dílčí zápis</strong>. Provede dílčí zápis serverů správy licencí.<br />
<br />
</li>
<li><strong>Aktivační server proxy</strong>. Funguje jako internetový server proxy pro požadavky klientů na bezpečnostní moduly a certifikáty počítače RMS.<br />
<br />
</li>
<li><strong>Certifikace</strong>. Vydává certifikáty účtů práv.<br />
<br />
</li>
<li><strong>Publikování</strong>. Vydává licence k publikování.<br />
<br />
</li>
<li><strong>Licencování</strong>. Vydává licence k použití.<br />
<br />
</li>
</ul>
Každá implementace musí obsahovat alespoň jeden server nebo cluster kořenové certifikace. V každé síti Active Directory může být pouze jeden cluster kořenové certifikace.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Licencování (nepovinné)</td>
<td style="border:1px solid black;">Spustí následující služby RMS:
<ul>
<li><strong>Publikování</strong>. Vydává licence k publikování.<br />
<br />
</li>
<li><strong>Licencování</strong>. Vydává licence k použití.<br />
<br />
</li>
</ul>
Servery správy licencí jsou často implementovány za účelem podpory jednotlivých oddělení nebo snížení zátěže požadavků na licencování na clusteru kořenové certifikace. Servery správy licencí jsou nepovinné.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Databázový server, například SQL Server</td>
<td style="border:1px solid black;"><ul>
<li>Provozuje konfigurační databáze, databáze protokolování a databáze adresářových služeb služby RMS.<br />
<br />
</li>
<li>Ukládá certifikáty účtů práv do konfigurační databáze clusteru kořenové certifikace.<br />
<br />
</li>
</ul></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Řadič domény a globální katalog</td>
<td style="border:1px solid black;"><ul>
<li>Zajišťuje ověření uživatelů a adresářové služby.<br />
<br />
</li>
<li>Ukládá umístění zjišťování služeb pro cluster kořenové certifikace.<br />
<br />
</li>
</ul></td>
</tr>
</tbody>
</table>
 

Pomocí služeb Enrollment Services a Activation Service, jejichž hostitelem je společnost Microsoft, zajišťuje služba RMS pro svůj systém společný kořen důvěryhodnosti. Další informace získáte v tomto tématu později v části [Hierarchie důvěryhodnosti služby RMS](https://technet.microsoft.com/2d44182f-a653-4383-aba1-dade53f7cf9a).

Následující diagram znázorňuje různé součásti systému služby RMS a jejich role v tomto systému. Šipky představují požadavky a odpovědi, které jsou předávány mezi jednotlivými součástmi.

![](images/Cc747671.29138741-d45c-459b-8ead-b9bc3f708dd5(WS.10).gif)

Další informace o každé součásti získáte v tomto tématu později v části [Softwarové součásti služby RMS](https://technet.microsoft.com/e38a840e-f390-48fd-8354-50108a64f5ca).
