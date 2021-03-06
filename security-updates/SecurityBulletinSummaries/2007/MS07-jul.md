---
TOCTitle: 'MS07-JUL'
Title: 'Souhrnný bulletin zabezpečení společnosti Microsoft, červenec 2007'
ms:assetid: 'ms07-jul'
ms:contentKeyID: 61223963
ms:mtpsurl: 'https://technet.microsoft.com/cs-CZ/library/ms07-jul(v=Security.10)'
---

Souhrnný bulletin zabezpečení společnosti Microsoft, červenec 2007
==================================================================

Publikováno: 10. července 2007 | Aktualizováno: 25. března 2008

**Verze:** 2.0

Tento souhrnný bulletin uvádí bulletiny zabezpečení vydané v červenci 2007.

Spolu s vydáním bulletinů pro červenec 2007 nahrazuje tento souhrnný bulletin předběžné oznámení o bulletinech vydané 5. července 2007. Další informace o službě předběžného oznámení o bulletinech naleznete v části [Předběžné oznámení o bulletinech zabezpečení společnosti Microsoft](http://technet.microsoft.com/security/bulletin/advance).

Informace o tom, jak dostávat automatická oznámení o vydání nových bulletinů zabezpečení společnosti Microsoft, naleznete na webu [Zasílání technických oznámení o zabezpečení společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=21163).

Pro zodpovězení zákaznických dotazů týkajících se těchto bulletinů uspořádá společnost Microsoft webové vysílání 11. července 2007 v 11:00 časového pásma Tichomoří (USA a Kanada). [Registrovat se pro webové vysílání týkající se červencových bulletinů zabezpečení](http://msevents.microsoft.com/cui/webcasteventdetails.aspx?eventid=1032343783&eventcategory=4&culture=en-us&countrycode=us). Po tomto datu je webové vysílání dostupné na požádání. Další informace získáte v [souhrnných bulletinech zabezpečení společnosti Microsoft a webovém vysílání](http://technet.microsoft.com/security/bulletin/summary).

Společnost Microsoft se snaží zákazníkům usnadnit upřednostnění měsíčně vydávaných aktualizací zabezpečení před jakýmikoli důležitými aktualizacemi nesouvisejícími se zabezpečením, které jsou vydány ve stejný den jako měsíčně vydávané aktualizace zabezpečení. Další informace získáte v části **Další informace**.

### Informace o bulletinech

#### Shrnutí

Bulletiny zabezpečení podle závažnosti:

Kritický (3)
------------


| Identifikátor bulletinu            | Bulletin zabezpečení společnosti Microsoft MS07-036                                                                                                                                                                                                                                                                                                                                                                                                                                             |
|------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Název bulletinu**                | [**Chyby zabezpečení v aplikaci Microsoft Excel umožňují vzdálené spuštění kódu (936542)**](http://technet.microsoft.com/security/bulletin/ms07-036)                                                                                                                                                                                                                                                                                                                                            |
| **Shrnutí**                        | Tato kritická aktualizace zabezpečení řeší jednu veřejně oznámenou chybu zabezpečení a dvě chyby zabezpečení oznámené soukromou osobou a další problémy se zabezpečením zjištěné při jejich přezkoumání. Tyto chyby umožňují vzdálené spuštění kódu, pokud uživatel otevře speciálně vytvořený soubor aplikace Excel. Uživatelé, jejichž účty jsou konfigurovány tak, aby měli v systému méně uživatelských práv, by byli vystaveni menšímu riziku než uživatelé s uživatelskými právy správce. |
| **Stupeň maximální závažnosti**    | [Kritický](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| **Dopad této chyby zabezpečení**   | Vzdálené spuštění kódu                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| **Rozpoznávání**                   | Pomocí nástroje MBSA (Microsoft Baseline Security Analyzer) lze určit, zda počítačový systém potřebuje tuto aktualizaci. Tato aktualizace nevyžaduje restartování.                                                                                                                                                                                                                                                                                                                              |
| **Software obsahující tuto chybu** | **Office, Excel**. Další informace získáte v části Software obsahující tuto chybu a umístění aktualizací ke stažení.                                                                                                                                                                                                                                                                                                                                                                            |

| Identifikátor bulletinu            | Bulletin zabezpečení společnosti Microsoft MS07-039                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
|------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Název bulletinu**                | [**Chyba zabezpečení služby Active Directory systému Windows umožňuje vzdálené spuštění kódu (926122)**](http://technet.microsoft.com/security/bulletin/ms07-039)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| **Shrnutí**                        | Tato kritická aktualizace zabezpečení řeší chybu zabezpečení oznámenou soukromou osobou v implementacích služby Active Directory v systémech Windows 2000 Server a Windows Server 2003, která by mohla způsobit vzdálené spuštění kódu nebo odmítnutí služby. Výsledkem pokusů o zneužití této chyby zabezpečení bude s největší pravděpodobností odmítnutí služby. Mohlo by však dojít ke spuštění vzdáleného kódu. Aby mohl útočník zneužít tuto chybu zabezpečení v systému Windows Server 2003, musel by znát platné přihlašovací údaje. Útočník, který by tuto chybu zabezpečení zneužil, by mohl získat úplnou kontrolu nad postiženým systémem. Útočník by tak mohl instalovat programy, zobrazovat, měnit či odstraňovat data nebo vytvářet nové účty. |
| **Stupeň maximální závažnosti**    | [Kritický](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| **Dopad této chyby zabezpečení**   | Vzdálené spuštění kódu                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| **Rozpoznávání**                   | Pomocí nástroje MBSA (Microsoft Baseline Security Analyzer) lze určit, zda počítačový systém potřebuje tuto aktualizaci. Aktualizace bude vyžadovat restartování počítače.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| **Software obsahující tuto chybu** | **Windows**. Další informace získáte v části Software obsahující tuto chybu a umístění aktualizací ke stažení.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |

| Identifikátor bulletinu            | Bulletin zabezpečení společnosti Microsoft MS07-040                                                                                                                                                                                                                                                                                                                                                                                                                           |
|------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Název bulletinu**                | [**Chyby zabezpečení v rozhraní .NET Framework umožňují vzdálené spuštění kódu (931212)**](http://technet.microsoft.com/security/bulletin/ms07-040)                                                                                                                                                                                                                                                                                                                           |
| **Shrnutí**                        | Tato aktualizace řeší tři soukromě oznámené chyby zabezpečení. Dvě z nich by mohly umožnit vzdálené spuštění kódu v klientských systémech s instalovaným rozhraním .NET Framework, jedna by mohla umožnit přístup k informacím na webech se spuštěnou funkcí ASP.NET. Ve všech případech spuštění vzdáleného kódu mají tyto chyby menší vliv na uživatele s účty konfigurovanými pro méně uživatelských oprávnění v systému než uživatelé pracující s oprávněními pro správu. |
| **Stupeň maximální závažnosti**    | [Kritický](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                      |
| **Dopad této chyby zabezpečení**   | Vzdálené spuštění kódu                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| **Rozpoznávání**                   | Pomocí nástroje MBSA (Microsoft Baseline Security Analyzer) lze určit, zda počítačový systém potřebuje tuto aktualizaci. Aktualizace bude vyžadovat restartování počítače.                                                                                                                                                                                                                                                                                                    |
| **Software obsahující tuto chybu** | **.NET Framework**. Další informace získáte v části Software obsahující tuto chybu a umístění aktualizací ke stažení.                                                                                                                                                                                                                                                                                                                                                         |

Důležité (2)
------------



| Identifikátor bulletinu            | Bulletin zabezpečení společnosti Microsoft MS07-037                                                                                                                                                                                                                                                                                                                                                                                                                        |
|------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Název bulletinu**                | [**Chyba zabezpečení v aplikaci Microsoft Office Publisher umožňuje vzdálené spuštění kódu (936548)**](http://technet.microsoft.com/security/bulletin/ms07-037)                                                                                                                                                                                                                                                                                                            |
| **Shrnutí**                        | Tato důležitá aktualizace zabezpečení řeší jednu veřejně známou chybu. Tato chyba zabezpečení umožňuje vzdálené spuštění kódu, pokud uživatel zobrazí speciálně vytvořený soubor aplikace Microsoft Office Publisher. Uživatelé, jejichž účty jsou konfigurovány tak, aby měli v systému méně uživatelských práv, by byli vystaveni menšímu riziku než uživatelé s uživatelskými právy správce. Zneužití této chyby zabezpečení je možné pouze při interakci s uživatelem. |
| **Stupeň maximální závažnosti**    | [Vysoký](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                     |
| **Dopad této chyby zabezpečení**   | Vzdálené spuštění kódu                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| **Rozpoznávání**                   | Pomocí nástroje MBSA (Microsoft Baseline Security Analyzer) lze určit, zda počítačový systém potřebuje tuto aktualizaci. Aktualizace nevyžaduje restartování.                                                                                                                                                                                                                                                                                                              |
| **Software obsahující tuto chybu** | **Office, Publisher**. Další informace získáte v části Software obsahující tuto chybu a umístění aktualizací ke stažení.                                                                                                                                                                                                                                                                                                                                                   |

| Identifikátor bulletinu            | Bulletin zabezpečení společnosti Microsoft MS07-041                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
|------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Název bulletinu**                | [**Chyba zabezpečení služby Microsoft Internet Information Services umožňuje vzdálené spuštění kódu (939373)**](http://technet.microsoft.com/security/bulletin/ms07-041)                                                                                                                                                                                                                                                                                                                                                                       |
| **Shrnutí**                        | Tato důležitá aktualizace řeší chybu zabezpečení oznámenou soukromou osobou. Tato chyba zabezpečení umožňuje vzdálené spuštění kódu, pokud uživatel odešle speciálně vytvořené požadavky URL webové stránce provozované službou IIS (Internet Information Services) 5.1 v systému Windows XP Professional Service Pack 2. Služba IIS 5.1 není součástí výchozího nastavení instalace systému Windows XP Professional Service Pack 2. Útočník, který by tuto chybu zabezpečení zneužil, by mohl získat úplnou kontrolu nad postiženým systémem. |
| **Stupeň maximální závažnosti**    | [Vysoký](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| **Dopad této chyby zabezpečení**   | Vzdálené spuštění kódu                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| **Rozpoznávání**                   | Pomocí nástroje MBSA (Microsoft Baseline Security Analyzer) lze určit, zda počítačový systém potřebuje tuto aktualizaci. Aktualizace bude vyžadovat restartování počítače.                                                                                                                                                                                                                                                                                                                                                                     |
| **Software obsahující tuto chybu** | **Windows XP Professional**. Další informace získáte v části Software obsahující tuto chybu a umístění aktualizací ke stažení.                                                                                                                                                                                                                                                                                                                                                                                                                 |

Mírný (1)
---------


| Identifikátor bulletinu            | Bulletin zabezpečení společnosti Microsoft MS07-038                                                                                                                                                                                                              |
|------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Název bulletinu**                | [**Chyba zabezpečení brány firewall systému Windows Vista může umožnit přístup k informacím (935807)**](http://technet.microsoft.com/security/bulletin/ms07-038)                                                                                                 |
| **Shrnutí**                        | Tato mírně závažná aktualizace řeší chybu zabezpečení oznámenou soukromou osobou. Tato chyba zabezpečení by mohla nevyžádanému příchozímu síťovému přenosu umožnit přístup k síťovému rozhraní. Útočník by tak mohl shromáždit informace o postiženém hostiteli. |
| **Stupeň maximální závažnosti**    | [Mírný](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                            |
| **Dopad této chyby zabezpečení**   | Přístup k informacím                                                                                                                                                                                                                                             |
| **Rozpoznávání**                   | Pomocí nástroje MBSA (Microsoft Baseline Security Analyzer) lze určit, zda počítačový systém potřebuje tuto aktualizaci. Aktualizace bude vyžadovat restartování počítače.                                                                                       |
| **Software obsahující tuto chybu** | **Windows** **Vista**. Další informace získáte v části Software obsahující tuto chybu a umístění aktualizací ke stažení.                                                                                                                                         |

Software obsahující tuto chybu a umístění aktualizací ke stažení
----------------------------------------------------------------


**Jak pracovat s touto tabulkou**

V této tabulce zjistíte, které aktualizace zabezpečení bude třeba nainstalovat. Přečtěte si seznam všech programů a součástí a zjistěte, zda jsou u nich vyžadovány aktualizace zabezpečení. Pokud se program nebo součást v seznamu nachází, je u nich uveden dopad chyby zabezpečení s odkazem na příslušnou aktualizaci.

**Poznámka:** Jedna chyba zabezpečení může vyžadovat instalaci více aktualizací. Přečtěte si celý sloupec u každého identifikátoru bulletinu. Zjistíte v něm, které aktualizace nainstalovat v závislosti na programech nebo součástech nainstalovaných ve vašem systému.

**Software obsahující tuto chybu a umístění aktualizací ke stažení**

 
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
[**MS07-036**](http://technet.microsoft.com/security/bulletin/ms07-036)
</td>
<td style="border:1px solid black;">
[**MS07-037**](http://technet.microsoft.com/security/bulletin/ms07-037)
</td>
<td style="border:1px solid black;">
[**MS07-038**](http://technet.microsoft.com/security/bulletin/ms07-038)
</td>
<td style="border:1px solid black;">
[**MS07-039**](http://technet.microsoft.com/security/bulletin/ms07-039)
</td>
<td style="border:1px solid black;">
[**MS07-040**](http://technet.microsoft.com/security/bulletin/ms07-040)
</td>
<td style="border:1px solid black;">
[**MS07-041**](http://technet.microsoft.com/security/bulletin/ms07-041)
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
[**Důležité**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Mírný**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritický**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritický**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Důležité**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<th colspan="7" style="border:1px solid black;">
Systémy Windows obsahující tuto chybu
</th>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Windows 2000 Service Pack 4
</td>
<td style="border:1px solid black;">
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
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 2000 Server Service Pack 4
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritický](http://www.microsoft.com/downloads/details.aspx?familyid=812e62c5-6e19-4b3b-8a10-861b871e1b41)
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Service Pack 2
</td>
<td style="border:1px solid black;">
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
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Professional Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Vysoký](http://www.microsoft.com/downloads/details.aspx?familyid=fccbfe90-f838-47df-8310-352e2fb47132)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Professional x64 Edition
</td>
<td style="border:1px solid black;">
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
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
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
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 1
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Vysoký](http://www.microsoft.com/downloads/details.aspx?familyid=28e84603-8159-4429-aaff-a1020531e84f)
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Vysoký](http://www.microsoft.com/downloads/details.aspx?familyid=28e84603-8159-4429-aaff-a1020531e84f)
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Vysoký](http://www.microsoft.com/downloads/details.aspx?familyid=107902f9-be94-457f-a936-519efbd64779)
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Vysoký](http://www.microsoft.com/downloads/details.aspx?familyid=107902f9-be94-457f-a936-519efbd64779)
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 SP1 pro systémy s procesorem Itanium
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Vysoký](http://www.microsoft.com/downloads/details.aspx?familyid=e5e5b425-fe7d-49d5-973f-f3fd7a1e04eb)
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 SP2 pro systémy s procesorem Itanium
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Vysoký](http://www.microsoft.com/downloads/details.aspx?familyid=e5e5b425-fe7d-49d5-973f-f3fd7a1e04eb)
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Mírný](http://www.microsoft.com/downloads/details.aspx?familyid=e9b64746-6afa-4a30-833d-e058e000c821)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista Service Pack 1
</td>
<td style="border:1px solid black;">
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
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 Edition
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Mírný](http://www.microsoft.com/downloads/details.aspx?familyid=0df5d190-3ad7-42d5-8629-43c47ec450cb)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 1
</td>
<td style="border:1px solid black;">
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
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008
</td>
<td style="border:1px solid black;">
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
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 pro systémy s procesorem Itanium
</td>
<td style="border:1px solid black;">
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
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 x64 Edition
</td>
<td style="border:1px solid black;">
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
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<th colspan="7" style="border:1px solid black;">
Součásti operačního systému Windows obsahující tuto chybu
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft .NET Framework 1.0  
(KB928367)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritický](http://www.microsoft.com/downloads/details.aspx?familyid=91d7afe4-069b-4ce8-976e-9a01345a8603)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft .NET Framework 1.0  
(KB930494)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritický](http://www.microsoft.com/downloads/details.aspx?familyid=829a2c5b-11ec-4ed7-91ab-6961034147bc)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft .NET Framework 1.1  
(KB928366)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritický](http://www.microsoft.com/downloads/details.aspx?familyid=281fb2cd-c715-4f05-a01f-0455d2d9ebfb)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft .NET Framework 1.1  
(KB933854)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritický](http://www.microsoft.com/downloads/details.aspx?familyid=2495e656-1e0a-4b83-90da-821e68067a71)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft .NET Framework 1.1  
(KB929729)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritický](http://www.microsoft.com/downloads/details.aspx?familyid=7eea368d-7b82-4583-8537-30351718a4e9)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft .NET Framework 2.0  
(KB928365)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritický](http://www.microsoft.com/downloads/details.aspx?familyid=ba3ceb78-8e1b-4c38-adfd-e8bc95ae548d)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft .NET Framework 2.0  
(KB929916)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritický](http://www.microsoft.com/downloads/details.aspx?familyid=cbc9f3cf-c3c3-45c4-82e3-e11398bc2cd2)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<th colspan="7" style="border:1px solid black;">
Software sady Office obsahující tuto chybu
</th>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2000 Service Pack 3
</td>
<td style="border:1px solid black;">
[Kritický](http://www.microsoft.com/downloads/details.aspx?familyid=83d94d8e-dda6-4d74-b40d-476c2f0a3af4)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
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
Excel 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Vysoký](http://www.microsoft.com/downloads/details.aspx?familyid=9d93c0ce-5124-4234-ba84-3c27005e010f)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
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
Excel 2003 Viewer
</td>
<td style="border:1px solid black;">
[Vysoký](http://www.microsoft.com/downloads/details.aspx?familyid=11f42977-8828-494a-a183-d1aba827b708)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
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
Excel 2007
</td>
<td style="border:1px solid black;">
[Vysoký](http://www.microsoft.com/downloads/details.aspx?familyid=9ab28283-0320-4527-b033-5e80ef32cd34)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
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
Sada Office Compatibility Pack pro formáty souborů aplikací Word, Excel a PowerPoint 2007
</td>
<td style="border:1px solid black;">
[Vysoký](http://www.microsoft.com/downloads/details.aspx?familyid=e592ae5b-09ac-4f5b-b457-a54c9850ad4a)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
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
Publisher 2007
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Vysoký](http://www.microsoft.com/downloads/details.aspx?familyid=25d272e7-f2dd-4342-92be-7ebc2e770b44)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
</table>
 
**Poznámky**

**<sup>[1]</sup>** Pro tento operační systém je k dispozici aktualizace zabezpečení. Další informace získáte v tabulce u softwaru nebo součásti obsahující tuto chybu a v příslušném bulletinu zabezpečení.

****

Nástroje a doporučené postupy zjišťování a nasazení
---------------------------------------------------


**Centrum zabezpečení**

Umožňuje správu aktualizací softwaru a zabezpečení, které je třeba nainstalovat na servery, stolní počítače a přenosné počítače v organizaci. Další informace naleznete na webu [TechNet Update Management Center](http://go.microsoft.com/fwlink/?linkid=69903). Další informace o zabezpečení produktů společnosti Microsoft nabízí web [Centrum zabezpečení TechNet](http://go.microsoft.com/fwlink/?linkid=21171). Tyto informace lze také získat klepnutím na nabídku „Nejnovější aktualizace zabezpečení“ na webu [Zabezpečení doma](http://go.microsoft.com/fwlink/?linkid=85102).

Aktualizace zabezpečení jsou k dispozici na webu [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747), [Windows Update](http://go.microsoft.com/fwlink/?linkid=21130) a [Office Update](http://go.microsoft.com/fwlink/?linkid=21135). Aktualizace zabezpečení jsou také k dispozici na webu [služby Stažení softwaru](http://go.microsoft.com/fwlink/?linkid=21129). Nejsnadněji je naleznete hledáním podle klíčového slova oprava\_zabezpečení (security\_patch). Aktualizace zabezpečení lze mimo jiné stáhnout z katalogu služby Windows Update. Další informace o katalogu systému Windows Update získáte v [článku 323166 znalostní báze Microsoft Knowledge Base](http://support.microsoft.com/kb/323166).

**Doporučené postupy zjišťování a instalace**

Společnost Microsoft poskytla doporučené postupy zjišťování a instalace aktualizací zabezpečení vydaných tento měsíc. Tyto doporučené postupy by měly pomoci také odborníkům v oblasti IT při používání různých nástrojů při instalaci aktualizace zabezpečení, např. Windows Update, Microsoft Update, Office Update, nástroj MBSA (Microsoft Baseline Security Analyzer), nástroj pro rozpoznávání sady Office, Microsoft Systems Management Server (SMS), nástroj Extended Security Update Inventory Tool a nástroj pro vyhledávání aktualizací v rozlehlých sítích (Enterprise Update Scanning Tool - EST). Další informace získáte v [článku 910723 znalostní báze Microsoft Knowledge Base](http://support.microsoft.com/kb/910723).

**Nástroj MBSA (Microsoft Baseline Security Analyzer) a** **nástroje pro vyhledávání aktualizací v rozlehlých sítích (Enterprise** **Update Scan Tool**

Pomocí nástroje Microsoft Baseline Security Analyzer (MBSA) mohou správci prohledávat místní i vzdálené systémy a zjistit tak, jestli v nich nechybí některé aktualizace zabezpečení nebo jestli v nastavení zabezpečení systému nedošlo k některým běžným chybám. Další informace o nástroji MBSA získáte na webu [Microsoft Baseline Security Analyzer](http://go.microsoft.com/fwlink/?linkid=21134).

Pokud nástroj MBSA 1.2.1 nepodporuje zjišťování určité aktualizace zabezpečení, společnost Microsoft vydá verzi nástroje pro vyhledávání aktualizací v rozlehlých sítích (Enterprise Update Scan Tool - EST) pro danou aktualizaci zabezpečení. Další informace o nástroji EST najdete na webu [Enterprise Update Scan Tool](http://support.microsoft.com/default.aspx?id=894193).

**Poznámka:** Po 9. říjnu 2007 už nebude aktualizován soubor MSSecure.XML používaný nástrojem MBSA 1.2.1. Po tomto datu nebudou do souboru MSSecure.XML používaného nástrojem MBSA 1.2.1 přidávány žádné nové aktualizace zabezpečení a nebudou vydávány nové verze nástroje EST. Další informace získáte na webu [Microsoft Baseline Security Analyzer](http://go.microsoft.com/fwlink/?linkid=21134).

**Služba Software Update Services**

Pomocí služby Microsoft Software Update Services (SUS) mohou správci systémů rychle a spolehlivě instalovat nejnovější důležité aktualizace zabezpečení pro servery se systémem Windows 2000 a Windows Server 2003 i pro stolní počítače se systémem Windows 2000 Professional nebo Windows XP Professional.

Další informace o způsobu instalace této aktualizace zabezpečení pomocí služby SUS získáte na webu služby [Software Update Services](http://go.microsoft.com/fwlink/?linkid=21133).

**Služba Windows Server Update Services**

Pomocí služby Windows Server Update Services (WSUS) mohou správci systémů rychle a spolehlivě instalovat nejnovější důležité aktualizace zabezpečení pro systémy Windows 2000 a novější, sadu Office XP a novější, Exchange Server 2003 a SQL Server 2000 do systémů Windows 2000 a novějších.

Další informace o způsobu instalace této aktualizace zabezpečení pomocí služby Windows Server Update Services získáte na webu služby [Windows Server Update Services](http://go.microsoft.com/fwlink/?linkid=50120).

**Systems Management Server**

Microsoft Systems Management Server (SMS) představuje v rozlehlých sítích řešení pro správu aktualizací s rozsáhlými možnostmi konfigurace. Umožňuje správcům identifikovat počítače se systémem Windows, které vyžadují aktualizace zabezpečení, a provést řízenou instalaci těchto aktualizací v celé rozlehlé síti s minimálním dopadem na koncové uživatele. Další informace o tom, jak mohou správci pomocí serveru SMS 2003 nasazovat aktualizace zabezpečení, získáte na webu [Správa oprav zabezpečení pomocí serveru SMS 2003 (SMS 2003 Security Patch Management)](http://go.microsoft.com/fwlink/?linkid=22939). Uživatelé serveru SMS 2.0 mohou při nasazení aktualizací zabezpečení použít také sadu [Software Updates Services Feature Pack](http://go.microsoft.com/fwlink/?linkid=33340). Další informace o serveru SMS získáte na webu [Microsoft Systems Management Server](http://go.microsoft.com/fwlink/?linkid=21158).

**Poznámka:** Server SMS využívá nástroj MBSA (Microsoft Baseline Security Analyzer) a nástroj pro rozpoznávání sady Microsoft Office, a poskytuje tak širokou podporu pro zjišťování a instalaci aktualizací uvedených v bulletinech zabezpečení. Tyto nástroje nemusí některé softwarové aktualizace zjistit. V takovém případě mohou správci použít funkce serveru SMS a nasměrovat aktualizace do určitých systémů. Další informace o tomto postupu najdete na webu [Nasazení aktualizací softwaru pomocí funkce Distribuce softwaru serveru SMS](http://go.microsoft.com/fwlink/?linkid=33341). Některé aktualizace zabezpečení vyžadují po restartování počítače oprávnění správce. Správci mohou k instalaci těchto aktualizací použít nástroj Elevated Rights Deployment Tool (k dispozici v sadě [SMS 2003 Administration Feature Pack](http://go.microsoft.com/fwlink/?linkid=33387) a [SMS 2.0 Administration Feature Pack](http://go.microsoft.com/fwlink/?linkid=21161)).

### Další informace

#### Nástroj pro odstranění škodlivého softwaru systému Microsoft Windows

Společnost Microsoft vydává aktualizovanou verzi Nástroje pro odstranění škodlivého softwaru systému Microsoft Windows na webu Windows Update, Microsoft Update, ve službě Windows Server Update Services a v centru pro stahování Download Center.

Tento nástroj **není** distribuován pomocí služby Software Update Services (SUS).

#### Důležité aktualizace nesouvisející se zabezpečením na webu Microsoft Update (MU), Windows Update (WU), ve službě Windows Server Update Services (WSUS) a Software Update Services (SUS)

Tento měsíc:

-   Společnost Microsoft vydala čtyři důležité aktualizace **nesouvisející se zabezpečením** na webu Microsoft Update (MU) a ve službě Windows Server Update Services (WSUS).
-   Společnost Microsoft vydala jednu důležitou aktualizaci systému Windows **nesouvisející se zabezpečením** na webu Windows Update (WU) a ve službě Software Update Services (SUS).

Tato informace se týká **pouze** důležitých aktualizací **nesouvisejících se zabezpečením** na webu Microsoft Update, Windows Update, ve službě Windows Server Update Services a Software Update Services vydaných ve stejný den jako souhrnný bulletin zabezpečení. Informace **se netýká** aktualizací **nesouvisejících se zabezpečením** vydaných v jiné dny.

#### Strategie zabezpečení a komunita

**Strategie instalace aktualizací**

Web [Doporučené postupy zabezpečení pro správu oprav (Security Guidance for Patch Management)](http://go.microsoft.com/fwlink/?linkid=21168) obsahuje další informace o instalaci aktualizací zabezpečení podle doporučení společnosti Microsoft.

**Získání dalších aktualizací zabezpečení**

Aktualizace odstraňující další problémy se zabezpečením získáte v následujících umístěních:

-   Aktualizace zabezpečení jsou k dispozici na webu služby [Stažení softwaru (Microsoft Download Center)](http://go.microsoft.com/fwlink/?linkid=21129). Nejsnadněji je naleznete vyhledáním klíčového slova security\_patch (oprava\_zabezpečení).
-   Aktualizace pro klientské platformy jsou k dispozici na webu [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747).
-   Aktualizace zabezpečení nabízené tento měsíc na webu Windows Update jsou k dispozici na webu služby Stažení softwaru v souborech obrazu ISO disku CD s vydanými aktualizacemi zabezpečení a kritickými aktualizacemi. Další informace získáte v [článku 913086 znalostní báze Microsoft Knowledge Base](http://support.microsoft.com/kb/913086).

**Komunita odborníků v oblasti zabezpečení**

Můžete se zde naučit, jak zlepšit zabezpečení a jak optimalizovat infrastrukturu IT. Také můžete s dalšími členy komunity IT Pro diskutovat o bezpečnostních tématech na webu [Komunita odborníků v oblasti zabezpečení (IT Pro Security Community)](http://go.microsoft.com/fwlink/?linkid=21164).

#### Poděkování

Společnost Microsoft tímto [děkuje](http://go.microsoft.com/fwlink/?linkid=21127) za spolupráci při ochraně zákazníků:

-   Dinisu Cruzovi ze společnosti [OWASP](http://www.owasp.org/) za oznámení chyby popsané v bulletinu [MS07-040](http://go.microsoft.com/fwlink/?linkid=91233).
-   Paulu Craigovi ze společnosti [Security Assessment](http://www.smsiinc.com/) za oznámení chyby popsané v bulletinu [MS07-040](http://go.microsoft.com/fwlink/?linkid=91233).
-   Jeroenu Frijtersovi ze společnosti [Sumatra](http://www.sumatra.nl/) za oznámení chyby popsané v bulletinu [MS07-040](http://go.microsoft.com/fwlink/?linkid=91233).
-   Společnosti [ProCheckUp](http://www.procheckup.com/) spolupracující s centrem [UK CPNI](http://www.cpni.gov.uk/) za původní oznámení chyby popsané v bulletinu [MS07-040](http://go.microsoft.com/fwlink/?linkid=91233).
-   Ferruhu T. Mavitunovi ze společnosti [Portcullis Computer Security Ltd.](http://www.portcullis-security.com/) za spolupráci se společností Microsoft a poskytnutí dalších informací týkajících se chyby popsané v bulletinu [MS07-040](http://go.microsoft.com/fwlink/?linkid=91233).
-   Johannesu Gumbelovi ze společnosti [TrueSec](http://www.truesec.com/) za spolupráci se společností Microsoft a poskytnutí dalších informací týkajících se chyby popsané v bulletinu [MS07-040](http://go.microsoft.com/fwlink/?linkid=91233).
-   Peteru Winter-Smithovi ze společnosti [NGSSoftware](http://www.nextgenss.com/) za oznámení chyby popsané v bulletinu [MS07-039](http://go.microsoft.com/fwlink/?linkid=93365).
-   Neelu Mehtovi ze společnosti [IBM Internet Security Systems x-Force](http://xforce.iss.net/) za oznámení chyby popsané v bulletinu [MS07-039](http://go.microsoft.com/fwlink/?linkid=93365).
-   Společnosti [eEye](http://www.eeye.com/) za oznámení chyby popsané v bulletinu [MS07-037](http://go.microsoft.com/fwlink/?linkid=93488).
-   Jimu Hoaglandovi a Olliemu Whitehousovi ze společnosti [Symantec](http://www.symantec.com/) za oznámení chyby popsané v bulletinu [MS07-038](http://go.microsoft.com/fwlink/?linkid=91033).
-   Jonathanu Afekovi a Adimu Sharabanimu ze společnosti [Watchfire](http://www.watchfire.com/) za spolupráci se společností Microsoft a poskytnutí dalších informací týkajících se chyby popsané v bulletinu [MS07-041](http://go.microsoft.com/fwlink/?linkid=93706).
-   Peteru Winter-Smithovi ze společnosti [NGSSoftware](http://www.nextgenss.com/) za spolupráci se společností Microsoft a poskytnutí dalších informací týkajících se chyby popsané v bulletinu [MS07-041](http://go.microsoft.com/fwlink/?linkid=93706).

#### Technická podpora

-   Uvedený software byl testován za účelem zjištění, kterých verzí se chyba týká. U dalších verzí skončila časově omezená podpora. Pokud chcete zjistit dobu, po kterou je pro určitou verzi softwaru poskytována podpora, navštivte web [Zásady poskytování technické podpory pro produkty společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=21742).
-   Zákazníci mohou získat technickou podporu na webu [služby technické podpory společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=21131). Hovory související s aktualizacemi zabezpečení jsou bezplatné.
-   Mezinárodní zákazníci získají podporu u místních zastoupení společnosti Microsoft. Technická podpora související s aktualizacemi zabezpečení je bezplatná. Další informace o možnostech kontaktování společnosti Microsoft v případě potřeby technické podpory získáte na [webu mezinárodní technické podpory](http://go.microsoft.com/fwlink/?linkid=21155).

#### Zřeknutí se záruky

Informace ve znalostní bázi Microsoft Knowledge Base jsou poskytovány tak, jak jsou, bez jakékoli záruky. Společnost Microsoft neposkytuje žádné záruky, výslovně uvedené či mlčky předpokládané, včetně záruk obchodovatelnosti a vhodnosti pro určitý účel. Společnost Microsoft ani její dodavatelé nenesou v žádném případě zodpovědnost za žádné škody, včetně přímých, nepřímých, náhodných či následných škod, ztráty zisku či zvláštních škod, a to ani v případě, že byli na možnost takových škod upozorněni. V některých zemích a právních řádech není dovoleno vyloučit nebo omezit odpovědnost, proto se výše uvedené omezení na vás nemusí vztahovat.

#### Revize

-   V1.0 (10. července 2007): Souhrnný bulletin byl publikován.
-   V2.0 (25. března 2008): Do tabulky softwaru obsahujícího chybu zabezpečení byl přidán systém Windows Vista Service Pack 1, Windows Vista x64 Edition Service Pack 1, Windows Server 2008, Windows Server 2008 pro systémy s procesorem Itanium a Windows Server 2008 x64 Edition.

*Built at 2014-04-18T01:50:00Z-07:00*
