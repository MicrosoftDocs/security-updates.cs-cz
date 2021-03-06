---
TOCTitle: 'MS08-MAR'
Title: 'Souhrnný bulletin zabezpečení společnosti Microsoft, březen 2008'
ms:assetid: 'ms08-mar'
ms:contentKeyID: 61223977
ms:mtpsurl: 'https://technet.microsoft.com/cs-CZ/library/ms08-mar(v=Security.10)'
---

 

Souhrnný bulletin zabezpečení společnosti Microsoft, březen 2008
================================================================

Publikováno: 11. března 2008 | Aktualizováno: 16. dubna 2008

**Verze:** 2.0

Tento souhrnný bulletin uvádí bulletiny zabezpečení vydané v březnu 2008.

Spolu s vydáním bulletinů pro březen 2008 nahrazuje tento souhrnný bulletin předběžné oznámení o bulletinech vydané 6. března 2008. Další informace o službě předběžného oznámení o bulletinech naleznete v části [Předběžné oznámení o bulletinech zabezpečení společnosti Microsoft](http://technet.microsoft.com/security/bulletin/advance).

Informace o tom, jak dostávat automatická oznámení o vydání nových bulletinů zabezpečení společnosti Microsoft, naleznete na webu [Zasílání technických oznámení o zabezpečení společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=21163).

Pro zodpovězení zákaznických dotazů týkajících se těchto bulletinů uspořádá společnost Microsoft webové vysílání 12. března 2008 v 11:00 časového pásma Tichomoří (USA a Kanada). [Registrovat se pro webové vysílání týkající se březnových bulletinů zabezpečení](http://msevents.microsoft.com/cui/webcasteventdetails.aspx?eventid=1032357217&eventcategory=4&culture=en-us&countrycode=us). Po tomto datu je webové vysílání dostupné na požádání. Další informace získáte v [souhrnných bulletinech zabezpečení společnosti Microsoft a webovém vysílání](http://technet.microsoft.com/security/bulletin/summary).

Společnost Microsoft se snaží zákazníkům usnadnit upřednostnění měsíčně vydávaných aktualizací zabezpečení před jakýmikoli důležitými aktualizacemi nesouvisejícími se zabezpečením, které jsou vydány ve stejný den jako měsíčně vydávané aktualizace zabezpečení. Další informace získáte v části **Další informace**.

### Informace o bulletinech

#### Shrnutí

Bulletiny zabezpečení podle závažnosti:

Kritický (4)
------------

 
| Identifikátor bulletinu            | Bulletin zabezpečení společnosti Microsoft MS08-014                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
|------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Název bulletinu**                | [**Chyby zabezpečení v aplikaci Microsoft Excel umožňují vzdálené spuštění kódu (949029)**](http://technet.microsoft.com/security/bulletin/ms08-014)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| **Shrnutí**                        | Tato aktualizace zabezpečení řeší několik chyb zabezpečení oznámených soukromými osobami i veřejně známých chyb v aplikaci Microsoft Office Excel, které mohou spustit vzdálený kód v případě, že uživatel otevře speciálně vytvořený soubor aplikace Excel. Útočník, který by tyto chyby zabezpečení zneužil, by mohl získat úplnou kontrolu nad postiženým systémem. Útočník by tak mohl instalovat programy, zobrazovat, měnit či odstraňovat data nebo vytvářet nové účty s úplnými uživatelskými právy. Uživatelé, jejichž účty jsou konfigurovány tak, aby měli v systému méně uživatelských práv, by byli vystaveni menšímu riziku než uživatelé s uživatelskými právy správce. |
| **Stupeň maximální závažnosti**    | [Kritický](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| **Dopad této chyby zabezpečení**   | Vzdálené spuštění kódu                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| **Rozpoznávání**                   | Pomocí nástroje MBSA (Microsoft Baseline Security Analyzer) lze určit, zda počítačový systém potřebuje tuto aktualizaci. Aktualizace nebude vyžadovat restartování.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| **Software obsahující tuto chybu** | **Microsoft Office.** Další informace získáte v části Software obsahující tuto chybu a umístění aktualizací ke stažení.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |

| Identifikátor bulletinu            | Bulletin zabezpečení společnosti Microsoft MS08-015                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
|------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Název bulletinu**                | [**Chyba zabezpečení v aplikaci Microsoft Outlook umožňuje vzdálené spuštění kódu (949031)**](http://technet.microsoft.com/security/bulletin/ms08-015)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| **Shrnutí**                        | Tato aktualizace zabezpečení řeší chybu zabezpečení v aplikaci Microsoft Office Outlook, kterou oznámila soukromá osoba. Tato chyba zabezpečení umožňuje vzdálené spuštění kódu, pokud je aplikaci Outlook předán speciálně vytvořený identifikátor URI protokolu mailto. Útočník by tak mohl instalovat programy, zobrazovat, měnit či odstraňovat data nebo vytvářet nové účty s úplnými uživatelskými právy. Uživatelé, jejichž účty jsou konfigurovány tak, aby měli v systému méně uživatelských práv, by byli vystaveni menšímu riziku než uživatelé s uživatelskými právy správce. Tuto chybu zabezpečení nelze zneužít prostým zobrazením e-mailu prostřednictvím podokna náhledu aplikace Outlook. |
| **Stupeň maximální závažnosti**    | [Kritický](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| **Dopad této chyby zabezpečení**   | Vzdálené spuštění kódu                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| **Rozpoznávání**                   | Pomocí nástroje MBSA (Microsoft Baseline Security Analyzer) lze určit, zda počítačový systém potřebuje tuto aktualizaci. Aktualizace nebude vyžadovat restartování.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| **Software obsahující tuto chybu** | **Microsoft Office.** Další informace získáte v části Software obsahující tuto chybu a umístění aktualizací ke stažení.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |

| Identifikátor bulletinu            | Bulletin zabezpečení společnosti Microsoft MS08-016                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
|------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Název bulletinu**                | [**Chyby zabezpečení v sadě Microsoft Office umožňují vzdálené spuštění kódu (949030)**](http://technet.microsoft.com/security/bulletin/ms08-016)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| **Shrnutí**                        | Tato aktualizace zabezpečení řeší dvě chyby zabezpečení sady Microsoft Office oznámené soukromými osobami, které by mohly umožnit vzdálené spuštění kódu v případě, že uživatel otevře chybně formátovaný soubor sady Office. Útočník, který by tuto chybu zabezpečení zneužil, by mohl získat úplnou kontrolu nad postiženým systémem. Útočník by tak mohl instalovat programy, zobrazovat, měnit či odstraňovat data nebo vytvářet nové účty s úplnými uživatelskými právy. Uživatelé, jejichž účty jsou konfigurovány tak, aby měli v systému méně uživatelských práv, by byli vystaveni menšímu riziku než uživatelé s uživatelskými právy správce. |
| **Stupeň maximální závažnosti**    | [Kritický](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| **Dopad této chyby zabezpečení**   | Vzdálené spuštění kódu                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| **Rozpoznávání**                   | Pomocí nástroje MBSA (Microsoft Baseline Security Analyzer) lze určit, zda počítačový systém potřebuje tuto aktualizaci. Aktualizace nebude vyžadovat restartování.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| **Software obsahující tuto chybu** | **Microsoft Office.** Další informace získáte v části Software obsahující tuto chybu a umístění aktualizací ke stažení.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |

| Identifikátor bulletinu            | Bulletin zabezpečení společnosti Microsoft MS08-017                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
|------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Název bulletinu**                | [**Chyby zabezpečení v součástech Microsoft Office Web Components umožňují vzdálené spuštění kódu (933103)**](http://technet.microsoft.com/security/bulletin/ms08-017)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| **Shrnutí**                        | Tato kritická aktualizace řeší dvě chyby zabezpečení součástí Microsoft Office Web Components oznámené soukromými osobami. Tyto chyby zabezpečení umožňují vzdálené spuštění kódu, pokud uživatel zobrazí speciálně vytvořenou webovou stránku. Útočník, který by tuto chybu zabezpečení zneužil, by mohl získat úplnou kontrolu nad postiženým systémem. Útočník by tak mohl instalovat programy, zobrazovat, měnit či odstraňovat data nebo vytvářet nové účty s úplnými uživatelskými právy. Uživatelé, jejichž účty jsou konfigurovány tak, aby měli v systému méně uživatelských práv, by byli vystaveni menšímu riziku než uživatelé s uživatelskými právy správce. |
| **Stupeň maximální závažnosti**    | [Kritický](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| **Dopad této chyby zabezpečení**   | Vzdálené spuštění kódu                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| **Rozpoznávání**                   | Pomocí nástroje MBSA (Microsoft Baseline Security Analyzer) lze určit, zda počítačový systém potřebuje tuto aktualizaci. Aktualizace může vyžadovat restartování počítače.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| **Software obsahující tuto chybu** | **Microsoft Office Web Components.** Další informace získáte v části Software obsahující tuto chybu a umístění aktualizací ke stažení.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |

Software obsahující tuto chybu a umístění aktualizací ke stažení
----------------------------------------------------------------

 
**Jak pracovat s touto tabulkou**

V této tabulce zjistíte, které aktualizace zabezpečení bude třeba nainstalovat. Přečtěte si seznam všech programů a komponent a zjistěte, zda jsou u nich vyžadovány aktualizace zabezpečení. Pokud se program nebo součást v seznamu nachází, je u nich uveden dopad chyby zabezpečení s odkazem na příslušnou aktualizaci.

**Poznámka:** Jedna chyba zabezpečení může vyžadovat instalaci více aktualizací. Přečtěte si celý sloupec u každého identifikátoru bulletinu. Zjistíte v něm, které aktualizace nainstalovat v závislosti na programech nebo součástech nainstalovaných ve vašem systému.

**Software obsahující tuto chybu a umístění aktualizací ke stažení**

 
<p></p>
<table style="border:1px solid black;">
<tr class="thead">
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
Podrobnosti
</th>
<th style="border:1px solid black;" >
Podrobnosti
</th>
<th style="border:1px solid black;" >
Podrobnosti
</th>
<th style="border:1px solid black;" >
Podrobnosti
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS08-014**](http://technet.microsoft.com/security/bulletin/ms08-014)
</td>
<td style="border:1px solid black;">
[**MS08-015**](http://technet.microsoft.com/security/bulletin/ms08-015)
</td>
<td style="border:1px solid black;">
[**MS08-016**](http://technet.microsoft.com/security/bulletin/ms08-016)
</td>
<td style="border:1px solid black;">
[**MS08-017**](http://technet.microsoft.com/security/bulletin/ms08-017)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Stupeň maximální závažnosti**
</td>
<td style="border:1px solid black;">
[**Kritický**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritický**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritický**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritický**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<th style="border:1px solid black;" colspan="5">
Sady Office a jejich software
</th>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2000 Service Pack 3
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritický](http://www.microsoft.com/downloads/details.aspx?familyid=72735aa1-e22c-40ed-8c79-38fba89979aa)
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office XP Service Pack 3
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Vysoký](http://www.microsoft.com/downloads/details.aspx?familyid=9cf8aafa-71a5-4017-b53c-4e80ef6e1188)
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Vysoký](http://www.microsoft.com/downloads/details.aspx?familyid=9f25922c-d3c2-4ef1-b164-8a21a77d29aa)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office Excel 2000 Service Pack 3
</td>
<td style="border:1px solid black;">
[Kritický](http://www.microsoft.com/downloads/details.aspx?familyid=f7f90c30-1bfd-406b-a77f-612443e30185)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Excel 2002 Service Pack 3
</td>
<td style="border:1px solid black;">
[Vysoký](http://www.microsoft.com/downloads/details.aspx?familyid=907f96d5-d1e9-4471-b41c-3ac811e63038)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office Excel 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Vysoký](http://www.microsoft.com/downloads/details.aspx?familyid=296e5f2c-f594-41c8-a20a-3e4c40ae3948)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Excel Viewer 2003
</td>
<td style="border:1px solid black;">
[Vysoký](http://www.microsoft.com/downloads/details.aspx?familyid=280bb2ac-b21a-46b5-8751-5a50fbebf107)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Vysoký](http://www.microsoft.com/downloads/details.aspx?familyid=9f25922c-d3c2-4ef1-b164-8a21a77d29aa)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office Excel Viewer 2003 Service Pack 3
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Vysoký](http://www.microsoft.com/downloads/details.aspx?familyid=9f25922c-d3c2-4ef1-b164-8a21a77d29aa)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Word Viewer 2003
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Vysoký](http://www.microsoft.com/downloads/details.aspx?familyid=9f25922c-d3c2-4ef1-b164-8a21a77d29aa)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office Word Viewer 2003 Service Pack 3
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Vysoký](http://www.microsoft.com/downloads/details.aspx?familyid=9f25922c-d3c2-4ef1-b164-8a21a77d29aa)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Excel 2007
</td>
<td style="border:1px solid black;">
[Vysoký](http://www.microsoft.com/downloads/details.aspx?familyid=e7634cb5-9531-4284-9554-4168fc488e0c)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Sada Microsoft Office Compatibility Pack pro formáty souborů aplikací Word, Excel a PowerPoint 2007
</td>
<td style="border:1px solid black;">
[Vysoký](http://www.microsoft.com/downloads/details.aspx?familyid=e9251d71-9098-4125-ae91-7d4c83ea58ad)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Outlook 2000 Service Pack 3
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritický](http://www.microsoft.com/downloads/details.aspx?familyid=714a49cd-5bca-4719-96a1-e1077f279533)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office Outlook 2002 Service Pack 3
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritický](http://www.microsoft.com/downloads/details.aspx?familyid=59853687-d885-4059-9460-ee403855dbd8)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Outlook 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritický](http://www.microsoft.com/downloads/details.aspx?familyid=fccc7c4c-8496-4682-bd46-6590503c1bf2)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office Outlook 2003 Service Pack 3
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritický](http://www.microsoft.com/downloads/details.aspx?familyid=fccc7c4c-8496-4682-bd46-6590503c1bf2)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Outlook 2007
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritický](http://www.microsoft.com/downloads/details.aspx?familyid=4e2baf00-88eb-4eb6-961a-54245b363c21)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2004 for Mac
</td>
<td style="border:1px solid black;">
[Vysoký](http://www.microsoft.com/downloads/details.aspx?familyid=95dceb37-b35f-46db-b280-db0f3b298aa9)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Vysoký](http://www.microsoft.com/downloads/details.aspx?familyid=95dceb37-b35f-46db-b280-db0f3b298aa9)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2008 for Mac
</td>
<td style="border:1px solid black;">
[Vysoký](http://www.microsoft.com/downloads/details.aspx?familyid=8fe8c32a-6d7a-482b-97c6-42562f089ee4)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<th style="border:1px solid black;" colspan="5">
Další software
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office Web Components 2000  
(KB931660)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritický](http://www.microsoft.com/downloads/details.aspx?familyid=806c654a-35e3-4385-855a-4b803249bfcf)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Web Components 2000  
(KB932031)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritický](http://www.microsoft.com/downloads/details.aspx?familyid=f54d2a5e-c0ed-4f70-9746-38dd61c8e9d7)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office Web Components 2000  
(KB933367)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritický](http://www.microsoft.com/downloads/details.aspx?familyid=d71b23fa-a873-406d-bad7-e38e565dee39)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Web Components 2000  
(KB933369)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritický](http://www.microsoft.com/downloads/details.aspx?familyid=2fe10ccd-40cb-4090-b83d-eae3d4eca174)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office Web Components 2000  
(KB939714)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritický](http://www.microsoft.com/downloads/details.aspx?familyid=5fddd54f-7a33-4ea3-b68d-b96a9bae509d)  
**<sup>[2]</sup>**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Web Components 2000  
(KB939714)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritický](http://www.microsoft.com/downloads/details.aspx?familyid=5fddd54f-7a33-4ea3-b68d-b96a9bae509d)  
**<sup>[3]</sup>**
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office Web Components 2000  
(KB941305)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritický](http://www.microsoft.com/downloads/details.aspx?familyid=71de76ba-b62c-4a7a-a78a-9317f5255b13)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Web Components 2000  
(KB948257)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritický](http://www.microsoft.com/downloads/details.aspx?familyid=526d87bd-c3da-412e-8765-c15987ae9b01)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Visual Studio .NET 2002 Service Pack 1  
(KB933367)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Visual Studio .NET 2003 Service Pack 1  
(KB933369)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft BizTalk Server 2000  
(KB939714)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft BizTalk Server 2002  
(KB939714)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Commerce Server 2000  
(KB941305)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Internet Security and Acceleration Server 2000 Service Pack 1 (SP1)  
(KB948257)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
</tr>
</table>
<p></p>
 
**Poznámky**

**<sup>[1]</sup>** Pro tento software je k dispozici aktualizace zabezpečení. Další informace získáte v tabulce u softwaru nebo součásti obsahující tuto chybu a v příslušném bulletinu zabezpečení.

**<sup>[2]</sup>** Tato aktualizace zabezpečení souvisí se serverem Microsoft BizTalk Server 2000. Podrobnosti naleznete v příslušném bulletinu zabezpečení.

**<sup>[3]</sup>** Tato aktualizace zabezpečení souvisí se serverem Microsoft BizTalk Server 2002. Podrobnosti naleznete v příslušném bulletinu zabezpečení.

Nástroje a doporučené postupy zjišťování a nasazení
---------------------------------------------------

 
**Centrum zabezpečení**

Umožňuje správu aktualizací softwaru a zabezpečení, které je třeba nainstalovat na servery, stolní počítače a přenosné počítače v organizaci. Další informace naleznete na webu [TechNet Update Management Center](http://go.microsoft.com/fwlink/?linkid=69903). Další informace o zabezpečení produktů společnosti Microsoft nabízí web [Centrum zabezpečení TechNet](http://go.microsoft.com/fwlink/?linkid=21171). Tyto informace lze také získat klepnutím na nabídku „Nejnovější aktualizace zabezpečení“ na webu [Zabezpečení doma](http://go.microsoft.com/fwlink/?linkid=85102).

Aktualizace zabezpečení jsou k dispozici na webu [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747), [Windows Update](http://go.microsoft.com/fwlink/?linkid=21130) a [Office Update](http://go.microsoft.com/fwlink/?linkid=21135). Aktualizace zabezpečení jsou také k dispozici na webu [služby Stažení softwaru](http://go.microsoft.com/fwlink/?linkid=21129). Nejsnadněji je naleznete hledáním podle klíčových slov aktualizace zabezpečení.

Aktualizace zabezpečení lze stáhnout z katalogu služby [Microsoft Update Catalog](http://go.microsoft.com/fwlink/?linkid=96155). Služba Microsoft Update Catalog poskytuje katalog s možností vyhledávání obsahu dostupného prostřednictvím služeb Windows Update a Microsoft Update, včetně aktualizací zabezpečení, ovladačů a aktualizací Service Pack. Vyhledáváním pomocí čísla bulletinu zabezpečení (například MS07-036) můžete přidat všechny dostupné aktualizace do košíku (včetně různých jazykových verzí aktualizace) a stáhnout je do vybrané složky. Další informace o službě Microsoft Update Catalog najdete v části [Nejčastější dotazy týkající se služby Microsoft Update Catalog](http://go.microsoft.com/fwlink/?linkid=97900).

**Doporučené postupy zjišťování a nasazení**

Společnost Microsoft poskytla doporučené postupy zjišťování a instalace aktualizací zabezpečení vydaných tento měsíc. Tyto doporučené postupy by měly pomoci také odborníkům v oblasti IT při používání různých nástrojů při instalaci aktualizace zabezpečení, např. Windows Update, Microsoft Update, Office Update, nástroj MBSA (Microsoft Baseline Security Analyzer), nástroj pro rozpoznávání sady Office, Microsoft Systems Management Server (SMS) a nástroj Extended Security Update Inventory Tool (ESUIT). Další informace získáte v [článku 910723 znalostní báze Microsoft Knowledge Base](http://support.microsoft.com/kb/910723).

**Nástroj Microsoft Baseline Security Analyzer**

Pomocí nástroje Microsoft Baseline Security Analyzer (MBSA) mohou správci prohledávat místní i vzdálené systémy a zjistit tak, jestli v nich nechybí některé aktualizace zabezpečení nebo jestli v nastavení zabezpečení systému nedošlo k některým běžným chybám. Další informace o nástroji MBSA získáte na webu [Microsoft Baseline Security Analyzer](http://go.microsoft.com/fwlink/?linkid=21134).

**Služba Windows Server Update Services**

Pomocí služby Windows Server Update Services (WSUS) mohou správci systémů rychle a spolehlivě instalovat nejnovější důležité aktualizace zabezpečení pro systémy Windows 2000 a novější, sadu Office XP a novější, Exchange Server 2003 a SQL Server 2000 do systémů Windows 2000 a novějších.

Další informace o způsobu instalace této aktualizace zabezpečení pomocí služby Windows Server Update Services získáte na webu služby [Windows Server Update Services](http://go.microsoft.com/fwlink/?linkid=50120).

**Systems Management Server**

Microsoft Systems Management Server (SMS) představuje v rozlehlých sítích řešení pro správu aktualizací s rozsáhlými možnostmi konfigurace. Umožňuje správcům identifikovat počítače se systémem Windows, které vyžadují aktualizace zabezpečení, a provést řízenou instalaci těchto aktualizací v celé rozlehlé síti s minimálním dopadem na koncové uživatele. K dispozici je nyní nová verze nástroje SMS, System Center Configuration Manager 2007 (viz také webové stránky produktu [System Center Configuration Manager 2007](http://technet.microsoft.com/en-us/library/bb735860.aspx)). Další informace o tom, jak mohou správci pomocí serveru SMS 2003 nasazovat aktualizace zabezpečení, získáte na webu [SMS 2003 Security Patch Management](http://go.microsoft.com/fwlink/?linkid=22939). Uživatelé serveru SMS 2.0 mohou při nasazení aktualizací zabezpečení použít také sadu [Software Updates Services Feature Pack](http://go.microsoft.com/fwlink/?linkid=33340). Další informace o serveru SMS získáte na webu [Microsoft Systems Management Server](http://go.microsoft.com/fwlink/?linkid=21158).

**Poznámka:** Server SMS využívá nástroj MBSA (Microsoft Baseline Security Analyzer) a nástroj pro rozpoznávání sady Microsoft Office, a poskytuje tak širokou podporu pro zjišťování a instalaci aktualizací uvedených v bulletinech zabezpečení. Tyto nástroje nemusí některé softwarové aktualizace zjistit. V takovém případě mohou správci použít funkce serveru SMS a nasměrovat aktualizace do určitých systémů. Další informace o tomto postupu najdete na webu [Nasazení aktualizací softwaru pomocí funkce Distribuce softwaru serveru SMS](http://go.microsoft.com/fwlink/?linkid=33341). Některé aktualizace zabezpečení vyžadují po restartování počítače oprávnění správce. Správci mohou k instalaci těchto aktualizací použít nástroj Elevated Rights Deployment Tool (k dispozici v sadě [SMS 2003 Administration Feature Pack](http://go.microsoft.com/fwlink/?linkid=33387) a [SMS 2.0 Administration Feature Pack](http://go.microsoft.com/fwlink/?linkid=21161)).

### Další informace

#### Nástroj pro odstranění škodlivého softwaru systému Microsoft Windows

Společnost Microsoft vydává aktualizovanou verzi Nástroje pro odstranění škodlivého softwaru systému Microsoft Windows na webu Windows Update, Microsoft Update, ve službě Windows Server Update Services a na webu služby Stažení softwaru.

#### Důležité aktualizace nesouvisející se zabezpečením na webu Microsoft Update (MU), Windows Update (WU) a ve službě Windows Server Update Services (WSUS)

Tento měsíc:

-   Společnost Microsoft vydala dvě důležité aktualizace **nesouvisející se zabezpečením** na webu Microsoft Update (MU) a ve službě Windows Server Update Services (WSUS).
-   Společnost Microsoft vydala tři důležité aktualizace systému Windows **nesouvisející se zabezpečením** na webu Windows Update (WU) a ve službě Windows Server Update Services (WSUS).

Tato informace se týká **pouze** důležitých aktualizací **nesouvisejících se zabezpečením** na webu Microsoft Update, Windows Update a ve službě Windows Server Update Services vydaných ve stejný den jako souhrnný bulletin zabezpečení. Informace **se netýká** aktualizací **nesouvisejících se zabezpečením** vydaných v jiné dny.

#### Strategie zabezpečení a komunita

**Strategie instalace aktualizací**

Web [Doporučené postupy zabezpečení pro správu aktualizací (Security Guidance for Update Management)](http://go.microsoft.com/fwlink/?linkid=21168) obsahuje další informace o instalaci aktualizací zabezpečení podle doporučení společnosti Microsoft.

**Získání dalších aktualizací zabezpečení**

Aktualizace odstraňující další problémy se zabezpečením získáte v následujících umístěních:

-   Aktualizace zabezpečení jsou k dispozici na webu služby [Stažení softwaru (Microsoft Download Center)](http://go.microsoft.com/fwlink/?linkid=21129). Nejsnadněji je naleznete hledáním podle klíčových slov aktualizace zabezpečení.
-   Aktualizace pro klientské platformy jsou k dispozici na webu [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747).
-   Aktualizace zabezpečení nabízené tento měsíc na webu Windows Update jsou k dispozici na webu služby Stažení softwaru v souborech obrazu ISO disku CD s vydanými aktualizacemi zabezpečení a kritickými aktualizacemi. Další informace získáte v [článku 913086 znalostní báze Microsoft Knowledge Base](http://support.microsoft.com/kb/913086).

**Komunita odborníků v oblasti zabezpečení**

Můžete se zde naučit, jak zlepšit zabezpečení a jak optimalizovat infrastrukturu IT. Také můžete s dalšími členy komunity IT Pro diskutovat o bezpečnostních tématech na webu [Komunita odborníků v oblasti zabezpečení (IT Pro Security Community)](http://go.microsoft.com/fwlink/?linkid=21164).

#### Poděkování

Společnost Microsoft tímto [děkuje](http://go.microsoft.com/fwlink/?linkid=21127) za spolupráci při ochraně zákazníků:

-   Miku Scottovi ze společnosti [SAIC](http://www.saic.com/) za oznámení chyby popsané v bulletinu MS08-014.
-   Mattu Richardovi ze společnosti [VeriSign](http://www.verisign.com/) za oznámení chyby popsané v bulletinu MS08-014.
-   Gregu MacManusovi ze společnosti [iDefense Labs](http://labs.idefense.com/) za oznámení chyby popsané v bulletinu MS08-014.
-   Yoshiyu Sasakiovi ze společnosti [JFE Systems](http://www.jfe-systems.com/) za oznámení chyby popsané v bulletinu MS08-014.
-   Bingu Liuovi ze společnosti [Fortinet](http://www.fortinet.com/) za oznámení chyby popsané v bulletinu MS08-014.
-   Společnosti [iDefense Labs](http://labs.idefense.com/) za oznámení chyby popsané v bulletinu MS08-014.
-   Codymu Piercovi ze společnosti [TippingPoint DVLabs](http://dvlabs.tippingpoint.com/) za oznámení chyby popsané v bulletinu MS08-014.
-   Motimu Josephovi a Danu Hubbardovi ze společnosti [Websense Security Labs](http://www.websense.com) za oznámení chyby popsané v bulletinu MS08-014.
-   Gregu MacManusovi ze společnosti [iDefense Labs](http://labs.idefense.com/) za oznámení chyby popsané v bulletinu MS08-015.
-   Arnaudu Dovimu, spolupracujícímu se společností [Zero Day Initiative (ZDI)](http://www.zerodayinitiative.com/), za oznámení chyby popsané v bulletinu MS08-016.
-   Anonymnímu nálezci za oznámení chyby popsané v bulletinu MS08-016.
-   Chrisi Riesovi ze společnosti [VigilantMinds Inc.](http://www.vigilantminds.com/) za oznámení chyby popsané v bulletinu MS08-017.
-   Xiao Huiovi ze společnosti [NCNIPC](http://www.nipc.org.cn/) za oznámení chyby popsané v bulletinu MS08-017.
-   Golanu Yosefovi ze společnosti [Finjan](http://www.finjan.com/) za oznámení chyby popsané v bulletinu MS08-017.
-   Yuvalu Ben-Itzhakovi ze společnosti [Finjan](http://www.finjan.com/) za oznámení chyby popsané v bulletinu MS08-017.

#### Technická podpora

-   Uvedený software byl testován za účelem zjištění, kterých verzí se chyba týká. U dalších verzí skončila časově omezená podpora. Pokud chcete zjistit dobu, po kterou je pro určitou verzi softwaru poskytována podpora, navštivte web [Zásady poskytování technické podpory pro produkty společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=21742).
-   Zákazníci mohou získat technickou podporu na webu [služby technické podpory společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=21131). Hovory související s aktualizacemi zabezpečení jsou bezplatné.
-   Mezinárodní zákazníci získají podporu u místních zastoupení společnosti Microsoft. Technická podpora související s aktualizacemi zabezpečení je bezplatná. Další informace o možnostech kontaktování společnosti Microsoft v případě potřeby technické podpory získáte na [webu mezinárodní technické podpory](http://go.microsoft.com/fwlink/?linkid=21155).

#### Zřeknutí se záruky

Informace ve znalostní bázi Microsoft Knowledge Base jsou poskytovány tak, jak jsou, bez jakékoli záruky. Společnost Microsoft neposkytuje žádné záruky, výslovně uvedené či mlčky předpokládané, včetně záruk obchodovatelnosti a vhodnosti pro určitý účel. Společnost Microsoft ani její dodavatelé nenesou v žádném případě zodpovědnost za žádné škody, včetně přímých, nepřímých, náhodných či následných škod, ztráty zisku či zvláštních škod, a to ani v případě, že byli na možnost takových škod upozorněni. V některých zemích a právních řádech není dovoleno vyloučit nebo omezit odpovědnost, proto se výše uvedené omezení na vás nemusí vztahovat.

#### Revize

-   V1.0 (11. března 2008): Souhrnný bulletin byl publikován.
-   V1.1 (12. března 2008): Souhrný bulletin byl aktualizován, aby informoval o novém odkazu ke stažení součástí Microsoft Office Web Components 2000 pro servery BizTalk Server 2000 a 2002.
-   V1.2 (26. března 2008): Souhrnný bulletin byl aktualizován, aby do bulletinu MS08-017 přidal nálezce chyby zabezpečení.
-   V2.0 (16. dubna 2008): Souhrnný bulletin byl aktualizován, aby do seznamu softwaru obsahujícího chybu zabezpečení, uvedeného v bulletinu MS08-016, přidal aplikaci Microsoft Office Word Viewer 2003 a Microsoft Office Word Viewer 2003 Service Pack 3.

*Built at 2014-04-18T01:50:00Z-07:00*
