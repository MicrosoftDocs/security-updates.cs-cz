---
TOCTitle: Podpora Internetové informační služby pro službu RMS
Title: Podpora Internetové informační služby pro službu RMS
ms:assetid: 'bd4dc69f-1e4e-4e95-9ae2-c925d8a14d4c'
ms:contentKeyID: 18113420
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747649(v=WS.10)'
---

Podpora Internetové informační služby pro službu RMS
====================================================

Hlavní služby RMS poskytuje sada webových služeb ASP .NET. Tyto webové služby jsou spuštěny na Internetové informační službě společnosti Microsoft® (IIS). Během procesu zajišťování serverů nastaví služba RMS ve službě IIS virtuální adresáře. Do těchto virtuálních adresářů jsou instalovány aplikační soubory pro webové služby.

Při serverovém zajišťování můžete vybrat web, v rámci kterého chcete vytvořit virtuální adresáře, ze seznamu webů, které na serveru existují. Před zajištěním serveru budete pravděpodobně chtít pro službu RMS vytvořit zvláštní web. Jestliže tento krok provedete, můžete nakonfigurovat ověřování a omezení přístupu přímo pro dané nasazení služby RMS.

Ve výchozím nastavení jsou soubory a virtuální adresáře webových služeb chráněny volitelnými seznamy řízení přístupu (DACL), které znemožňují neoprávněný přístup k funkcím těchto služeb. Příslušné položky řízení přístupu (ACE) jsou nastaveny následujícím způsobem:

-   skupina Administrators má úplné řízení,
-   místní systém má úplné řízení,
-   skupina RMS Service Group má oprávnění pro čtení a spuštění,
-   skupiny Guests a Users mají oprávnění pro čtení a spuštění, získání obsahu složky a pro čtení,
-   anonymní přístup není povolen.

V následující tabulce je uveden seznam virtuálních adresářů, které jsou vytvořeny ve službě IIS, a služeb, které jsou instalovány ve virtuálních adresářích.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Virtuální adresář</th>
<th style="border:1px solid black;" >Služba</th>
<th style="border:1px solid black;" >Soubor webové služby</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">_wmcs</td>
<td style="border:1px solid black;">Toto je virtuální adresář správy clusteru RMS.</td>
<td style="border:1px solid black;">Není k dispozici</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Certification</td>
<td style="border:1px solid black;">Tento virtuální adresář obsahuje služby, které podporují certifikaci RMS.</td>
<td style="border:1px solid black;">Není k dispozici</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Aktivační server proxy</td>
<td style="border:1px solid black;">Activation.asmx</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Certifikace účtu</td>
<td style="border:1px solid black;">Certification.asmx</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Předběžná certifikace</td>
<td style="border:1px solid black;">Precertification.asmx</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Lokátor služeb</td>
<td style="border:1px solid black;">ServiceLocator.asmx</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Server</td>
<td style="border:1px solid black;">Server.asmx</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Certifikace serverů</td>
<td style="border:1px solid black;">ServerCertification.asmx</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Certifikace mobilních zařízení</td>
<td style="border:1px solid black;">MobileDeviceCertfication.asmx</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Zápis</td>
<td style="border:1px solid black;">SubEnrollService.asmx</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Správa licencí</td>
<td style="border:1px solid black;">Tento virtuální adresář obsahuje služby, které podporují správu licencí RMS</td>
<td style="border:1px solid black;">Není k dispozici</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Správa licencí</td>
<td style="border:1px solid black;">License.asmx</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Publikování</td>
<td style="border:1px solid black;">Publish.asmx</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Server</td>
<td style="border:1px solid black;">Server.asmx</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Lokátor služeb</td>
<td style="border:1px solid black;">ServiceLocator.asmx</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Admin</td>
<td style="border:1px solid black;">Tento virtuální adresář obsahuje služby, které podporují správu RMS.</td>
<td style="border:1px solid black;">Není k dispozici</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Správa</td>
<td style="border:1px solid black;">AdminSvc.asmx</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Služba DrmRemote</td>
<td style="border:1px solid black;">Rozhraní .NET Remoting</td>
<td style="border:1px solid black;">Není k dispozici</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DirectoryServices</td>
<td style="border:1px solid black;">Jedná se o podadresář služby DrmRemote.</td>
<td style="border:1px solid black;">Není k dispozici</td>
</tr>
</tbody>
</table>
  
| ![](images/Cc747649.note(WS.10).gif)Poznámka                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |  
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Služba správy má těsnější omezení než ostatní webové služby, protože ostatní poskytované služby umožňují konfigurovat služby RMS. Z tohoto důvodu členové skupiny uživatelů nemohou získat přístup ke službě správy. Filtrování IP je navíc povoleno pro přidělení přístupu pouze k místnímu počítači. Virtuální adresář DirectoryServices nepřiděluje přístupová práva pro uživatele Guest. Služba lokátoru služeb také přiděluje úplná přístupová práva k účtu síťové služby. Chcete-li zajistit server správy licencí, je nutné změnit výchozí položky řízení přístupu tak, aby povolovaly přístup správci služby RMS. |
