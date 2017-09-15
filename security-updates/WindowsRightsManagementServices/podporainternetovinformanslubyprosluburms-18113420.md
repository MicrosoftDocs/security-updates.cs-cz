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

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th>Virtuální adresář</th>
<th>Služba</th>
<th>Soubor webové služby</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>_wmcs</p></td>
<td style="border:1px solid black;"><p>Toto je virtuální adresář správy clusteru RMS.</p></td>
<td style="border:1px solid black;"><p>Není k dispozici</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Certification</p></td>
<td style="border:1px solid black;"><p>Tento virtuální adresář obsahuje služby, které podporují certifikaci RMS.</p></td>
<td style="border:1px solid black;"><p>Není k dispozici</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>Aktivační server proxy</p></td>
<td style="border:1px solid black;"><p>Activation.asmx</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>Certifikace účtu</p></td>
<td style="border:1px solid black;"><p>Certification.asmx</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>Předběžná certifikace</p></td>
<td style="border:1px solid black;"><p>Precertification.asmx</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>Lokátor služeb</p></td>
<td style="border:1px solid black;"><p>ServiceLocator.asmx</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>Server</p></td>
<td style="border:1px solid black;"><p>Server.asmx</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>Certifikace serverů</p></td>
<td style="border:1px solid black;"><p>ServerCertification.asmx</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>Certifikace mobilních zařízení</p></td>
<td style="border:1px solid black;"><p>MobileDeviceCertfication.asmx</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>Zápis</p></td>
<td style="border:1px solid black;"><p>SubEnrollService.asmx</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Správa licencí</p></td>
<td style="border:1px solid black;"><p>Tento virtuální adresář obsahuje služby, které podporují správu licencí RMS</p></td>
<td style="border:1px solid black;"><p>Není k dispozici</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>Správa licencí</p></td>
<td style="border:1px solid black;"><p>License.asmx</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>Publikování</p></td>
<td style="border:1px solid black;"><p>Publish.asmx</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>Server</p></td>
<td style="border:1px solid black;"><p>Server.asmx</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>Lokátor služeb</p></td>
<td style="border:1px solid black;"><p>ServiceLocator.asmx</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Admin</p></td>
<td style="border:1px solid black;"><p>Tento virtuální adresář obsahuje služby, které podporují správu RMS.</p></td>
<td style="border:1px solid black;"><p>Není k dispozici</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>Správa</p></td>
<td style="border:1px solid black;"><p>AdminSvc.asmx</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Služba DrmRemote</p></td>
<td style="border:1px solid black;"><p>Rozhraní .NET Remoting</p></td>
<td style="border:1px solid black;"><p>Není k dispozici</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>DirectoryServices</p></td>
<td style="border:1px solid black;"><p>Jedná se o podadresář služby DrmRemote.</p></td>
<td style="border:1px solid black;"><p>Není k dispozici</p></td>
</tr>  
</tbody>  
</table>
  
| ![](images/Cc747649.note(WS.10).gif)Poznámka                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |  
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Služba správy má těsnější omezení než ostatní webové služby, protože ostatní poskytované služby umožňují konfigurovat služby RMS. Z tohoto důvodu členové skupiny uživatelů nemohou získat přístup ke službě správy. Filtrování IP je navíc povoleno pro přidělení přístupu pouze k místnímu počítači. Virtuální adresář DirectoryServices nepřiděluje přístupová práva pro uživatele Guest. Služba lokátoru služeb také přiděluje úplná přístupová práva k účtu síťové služby. Chcete-li zajistit server správy licencí, je nutné změnit výchozí položky řízení přístupu tak, aby povolovaly přístup správci služby RMS. |
