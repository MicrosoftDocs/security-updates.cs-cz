---
TOCTitle: Seznamy odvolání služby RMS
Title: Seznamy odvolání služby RMS
ms:assetid: '688d4dfa-c928-4b2f-8116-2f9e87d2b6f7'
ms:contentKeyID: 18113307
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc720287(v=WS.10)'
---

Seznamy odvolání služby RMS
===========================

Tyto seznamy určují obsah, aplikace, uživatele nebo jiné zaregistrované objekty, které byly odvolány. Entita může být organizací zadána do seznamu odvolání z jednoho nebo z několika z následujících důvodů:

-   Soukromý klíč je známý nebo existuje podezření na jeho ohrožení.
-   Vlastník požaduje odvolání klíče kvůli možnému ohrožení.
-   Zaregistrovaný objekt již není platný (například při propuštění zaměstnance).
-   Byla zaznamenána závada v systému zabezpečení (například došlo ke zneužití certifikátu vydaného pro klientský počítač).
-   Je vyžadována opětovná certifikace kvůli změnám v ověřování.
-   Z důvodu neodpovídajícího zabezpečení aplikace s podporou služby RMS není vhodné v této aplikaci využívat vysoce citlivý obsah, případně žádný chráněný obsah.
-   Dříve distribuovaná část obsahu již není aktuální nebo již není vhodná k použití.

V následující tabulce jsou popsány entity, které lze uvést v seznamu odvolání, spolu s údaji používanými při jejich identifikaci.

###  

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Entita</th>
<th>Identifikátor</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>Skupina licencí nebo certifikátů</p></td>
<td style="border:1px solid black;"><p>Veřejný klíč nebo ID vydavatele</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Skupina manifestů aplikace</p></td>
<td style="border:1px solid black;"><p>Veřejný klíč nebo ID vydavatele</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Specifická licence nebo certifikát</p></td>
<td style="border:1px solid black;"><p>Hodnota hash nebo ID licence</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Specifický manifest aplikace</p></td>
<td style="border:1px solid black;"><p>Hodnota hash nebo ID licence</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Specifický zaregistrovaný objekt</p></td>
<td style="border:1px solid black;"><p>Veřejný klíč nebo ID zaregistrovaného objektu</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Specifická část obsahu</p></td>
<td style="border:1px solid black;"><p>ID obsahu</p></td>
</tr>
</tbody>
</table>
  
| ![](images/Cc720287.note(WS.10).gif)Poznámka                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |  
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| V případě odvolání a vyloučení jsou všechny hodnoty hash vytvořeny algoritmem SHA-1 \[NIS94c\]. Jedná se o revizi algoritmu SHA (Secure Hash Algorithm), který je specifikován ve standardu SHS (Secure Hash Standard, FIPS 180). Algoritmus SHA-1 je popsán ve standardu ANSI X9.30 (část 2). Chcete-li provést odvolání podle manifestu aplikace, je nutné z tohoto manifestu extrahovat ID vydavatele, veřejný klíč vydavatele, ID licence nebo hodnotu hash licence. Manifesty aplikací jsou však kódovány způsobem base64, takže informace nejsou k dispozici v přehledné formě. Pomocí sady SDK klienta Služby správy přístupových práv lze prostřednictvím metod **DRMConstructCertificateChain**, **DRMDeconstructCertificateChain** a **DRMDecode** vytvořit program umožňující dekódování manifestu aplikace a získání požadovaných informací. Chcete-li zabránit některým aplikacím ve využití obsahu chráněného správou přístupových práv, zvažte jejich vyloučení, což serveru RMS znemožní udělování licencí k použití těmto aplikacím. Vyloučení jsou však omezena a nemohou zabránit uživateli s platnou licencí k použití v dešifrování obsahu chráněného správou přístupových práv. Další informace o vyloučení aplikací získáte v této sadě dokumentace v části Vyloučení aplikací tématu Provoz serveru RMS. |
  
Seznamy odvolání jsou ve formě souborů XrML, které určují následující parametry.
  
###  

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Parametr</th>
<th>Popis</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>ISSUEDTIME</p></td>
<td style="border:1px solid black;"><p>Systémový čas v okamžiku vytvoření souboru XrML. Tento parametr používá podmínka REFRESH, pomocí které je v licenci k použití určeno stáří seznamu odvolání.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>ISSUER</p></td>
<td style="border:1px solid black;"><p>Jméno, ID a adresa vydavatele seznamu odvolání.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>PUBLICKEY</p></td>
<td style="border:1px solid black;"><p>Veřejný klíč vydavatele seznamu odvolání.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>REVOCATIONLIST</p></td>
<td style="border:1px solid black;"><p>Název, typ a ID každé odvolané entity.</p></td>
</tr>
</tbody>
</table>
