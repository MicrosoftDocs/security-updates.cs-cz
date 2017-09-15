---
TOCTitle: Služba předběžné certifikace RMS
Title: Služba předběžné certifikace RMS
ms:assetid: '09957294-167f-4f98-88e9-ae90fbeb26c1'
ms:contentKeyID: 18113206
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc720191(v=WS.10)'
---

Služba předběžné certifikace RMS
================================

Služba předběžné certifikace je spuštěna pouze na kořenovém clusteru služby RMS. Tato služba umožňuje serveru odeslat jménem uživatele požadavek na certifikát účtu práv a zároveň ji lze využít k vývoji vlastních aplikací. Mezi příklady součástí využívajících tuto službu patří Microsoft Exchange Server 2007 a Microsoft Office SharePoint Server 2007.

Aplikační soubor služby předběžné certifikace (soubor Precertification.asmx) je uložen ve virtuálním adresáři Certification, který je součástí Internetové informační služby.

Další informace o vývoji vlastních aplikací získáte v knihovně MSDN v článku Windows Rights Management Services Technology Documentation (Dokumentace k technologii Služby přístupových práv) na webu společnosti Microsoft [http://go.microsoft.com/fwlink/?LinkId=32972](http://go.microsoft.com/fwlink/?linkid=32972) (stránka může být v angličtině).

V následující tabulce je znázorněn výchozí seznam řízení přístupu k této službě:

###  

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Uživatel nebo skupina</th>
<th>Výchozí oprávnění</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>Administrators</p></td>
<td style="border:1px solid black;"><p>Úplné řízení</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>RMS Service Group</p></td>
<td style="border:1px solid black;"><p>Čtení a spouštění</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>SYSTEM</p></td>
<td style="border:1px solid black;"><p>Úplné řízení</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Users</p></td>
<td style="border:1px solid black;"><p>Čtení a spouštění</p></td>
</tr>  
</tbody>  
</table>
