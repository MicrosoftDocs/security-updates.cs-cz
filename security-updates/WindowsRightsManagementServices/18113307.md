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

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Entita</th>
<th style="border:1px solid black;" >Identifikátor</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Skupina licencí nebo certifikátů</td>
<td style="border:1px solid black;">Veřejný klíč nebo ID vydavatele</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Skupina manifestů aplikace</td>
<td style="border:1px solid black;">Veřejný klíč nebo ID vydavatele</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Specifická licence nebo certifikát</td>
<td style="border:1px solid black;">Hodnota hash nebo ID licence</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Specifický manifest aplikace</td>
<td style="border:1px solid black;">Hodnota hash nebo ID licence</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Specifický zaregistrovaný objekt</td>
<td style="border:1px solid black;">Veřejný klíč nebo ID zaregistrovaného objektu</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Specifická část obsahu</td>
<td style="border:1px solid black;">ID obsahu</td>
</tr>
</tbody>
</table>
  
> [!NOTE]
> V případě odvolání a vyloučení jsou všechny hodnoty hash vytvořeny algoritmem SHA-1 \[NIS94c\]. Jedná se o revizi algoritmu SHA (Secure Hash Algorithm), který je specifikován ve standardu SHS (Secure Hash Standard, FIPS 180). Algoritmus SHA-1 je popsán ve standardu ANSI X9.30 (část 2). Chcete-li provést odvolání podle manifestu aplikace, je nutné z tohoto manifestu extrahovat ID vydavatele, veřejný klíč vydavatele, ID licence nebo hodnotu hash licence. Manifesty aplikací jsou však kódovány způsobem base64, takže informace nejsou k dispozici v přehledné formě. Pomocí sady SDK klienta Služby správy přístupových práv lze prostřednictvím metod **DRMConstructCertificateChain**, **DRMDeconstructCertificateChain** a **DRMDecode** vytvořit program umožňující dekódování manifestu aplikace a získání požadovaných informací. Chcete-li zabránit některým aplikacím ve využití obsahu chráněného správou přístupových práv, zvažte jejich vyloučení, což serveru RMS znemožní udělování licencí k použití těmto aplikacím. Vyloučení jsou však omezena a nemohou zabránit uživateli s platnou licencí k použití v dešifrování obsahu chráněného správou přístupových práv. Další informace o vyloučení aplikací získáte v této sadě dokumentace v části Vyloučení aplikací tématu Provoz serveru RMS. 
  
Seznamy odvolání jsou ve formě souborů XrML, které určují následující parametry.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Parametr</th>
<th style="border:1px solid black;" >Popis</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">ISSUEDTIME</td>
<td style="border:1px solid black;">Systémový čas v okamžiku vytvoření souboru XrML. Tento parametr používá podmínka REFRESH, pomocí které je v licenci k použití určeno stáří seznamu odvolání.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">ISSUER</td>
<td style="border:1px solid black;">Jméno, ID a adresa vydavatele seznamu odvolání.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">PUBLICKEY</td>
<td style="border:1px solid black;">Veřejný klíč vydavatele seznamu odvolání.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">REVOCATIONLIST</td>
<td style="border:1px solid black;">Název, typ a ID každé odvolané entity.</td>
</tr>
</tbody>
</table>
