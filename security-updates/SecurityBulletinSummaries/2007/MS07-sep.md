---
TOCTitle: 'MS07-SEP'
Title: 'Souhrnný bulletin zabezpečení společnosti Microsoft, září 2007'
ms:assetid: 'ms07-sep'
ms:contentKeyID: 61223969
ms:mtpsurl: 'https://technet.microsoft.com/cs-CZ/library/ms07-sep(v=Security.10)'
---

Souhrnný bulletin zabezpečení společnosti Microsoft, září 2007
==============================================================

Publikováno: 11. září 2007 | Aktualizováno: 12. září 2007

**Verze:** 1.1

**Verze** 1.1

Tento souhrnný bulletin uvádí bulletiny zabezpečení vydané v září 2007.

Spolu s vydáním bulletinů pro září 2007 nahrazuje tento souhrnný bulletin předběžné oznámení o bulletinech vydané 6. září 2007. Další informace o službě předběžného oznámení o bulletinech naleznete v části [Předběžné oznámení o bulletinech zabezpečení společnosti Microsoft](http://technet.microsoft.com/security/bulletin/advance).

Informace o tom, jak dostávat automatická oznámení o vydání nových bulletinů zabezpečení společnosti Microsoft, naleznete na webu [Zasílání technických oznámení o zabezpečení společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=21163).

Pro zodpovězení zákaznických dotazů týkajících se těchto bulletinů uspořádá společnost Microsoft webové vysílání 12. září 2007 v 11:00 časového pásma Tichomoří (USA a Kanada). [Registrovat se pro webové vysílání týkající se zářijových bulletinů zabezpečení](http://msevents.microsoft.com/cui/webcasteventdetails.aspx?eventid=1032344690&eventcategory=4&culture=en-us&countrycode=us). Po tomto datu je webové vysílání dostupné na požádání. Další informace získáte v [souhrnných bulletinech zabezpečení společnosti Microsoft a webovém vysílání](http://technet.microsoft.com/security/bulletin/summary).

Společnost Microsoft se snaží zákazníkům usnadnit upřednostnění měsíčně vydávaných aktualizací zabezpečení před jakýmikoli důležitými aktualizacemi nesouvisejícími se zabezpečením, které jsou vydány ve stejný den jako měsíčně vydávané aktualizace zabezpečení. Další informace získáte v části **Další informace**.

### Informace o bulletinech

#### Shrnutí

Bulletiny zabezpečení podle závažnosti:

Kritický (1)
------------


| Identifikátor bulletinu            | Bulletin zabezpečení společnosti Microsoft MS07-051                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
|------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Název bulletinu**                | [**Chyba zabezpečení v technologii Microsoft Agent umožňuje vzdálené spuštění kódu (938827)**](http://go.microsoft.com/fwlink/?linkid=94667)                                                                                                                                                                                                                                                                                                                                                                     |
| **Shrnutí**                        | Tato kritická aktualizace zabezpečení řeší chybu zabezpečení oznámenou soukromou osobou. V technologii Microsoft Agent existuje chyba zabezpečení, která umožňuje vzdálené spuštění kódu. Důvodem je způsob zpracování některých adres URL. Tato chyba zabezpečení může útočníkovi umožnit vzdálené spuštění kódu v ohroženém systému. Uživatelé, jejichž účty jsou konfigurovány tak, aby měli v systému méně uživatelských práv, by byli vystaveni menšímu riziku než uživatelé s uživatelskými právy správce. |
| **Stupeň maximální závažnosti**    | [Kritický](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| **Dopad této chyby zabezpečení**   | Vzdálené spuštění kódu                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| **Rozpoznávání**                   | Pomocí nástroje MBSA (Microsoft Baseline Security Analyzer) lze určit, zda počítačový systém potřebuje tuto aktualizaci. Aktualizace bude vyžadovat restartování počítače.                                                                                                                                                                                                                                                                                                                                       |
| **Software obsahující tuto chybu** | **Windows.** Další informace získáte v části Software obsahující tuto chybu a umístění aktualizací ke stažení.                                                                                                                                                                                                                                                                                                                                                                                                   |

Vysoký (3)
----------


| Identifikátor bulletinu            | Bulletin zabezpečení společnosti Microsoft MS07-052                                                                                                                                                                                                                                                                                                |
|------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Název bulletinu**                | [**Chyba zabezpečení nástroje Crystal Reports for Visual Studio umožňuje vzdálené spuštění kódu (941522)**](http://go.microsoft.com/fwlink/?linkid=98460)                                                                                                                                                                                          |
| **Shrnutí**                        | Tato důležitá aktualizace zabezpečení řeší jednu veřejně známou chybu. Tato chyba umožňuje vzdálené spuštění kódu, pokud uživatel otevře speciálně vytvořený soubor RPT. Uživatelé, jejichž účty jsou konfigurovány tak, aby měli v systému méně uživatelských práv, by byli vystaveni menšímu riziku než uživatelé s uživatelskými právy správce. |
| **Stupeň maximální závažnosti**    | [Vysoký](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                             |
| **Dopad této chyby zabezpečení**   | Vzdálené spuštění kódu                                                                                                                                                                                                                                                                                                                             |
| **Rozpoznávání**                   | Nástroj Microsoft Baseline Security Analyzer a nástroj pro vyhledávání aktualizací v rozlehlých sítích (Enterprise Update Scan Tool – EST) rozezná, zda váš počítačový systém vyžaduje tuto aktualizaci. Aktualizace může vyžadovat restartování počítače.                                                                                         |
| **Software obsahující tuto chybu** | **Visual Studio.** Další informace získáte v části Software obsahující tuto chybu a umístění aktualizací ke stažení.                                                                                                                                                                                                                               |

| Identifikátor bulletinu            | Bulletin zabezpečení společnosti Microsoft MS07-053                                                                                                                                                                                                                                                                                                            |
|------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Název bulletinu**                | [**Chyba zabezpečení ve Službách systému Windows pro systém UNIX může způsobit zvýšení úrovně oprávnění (939778)**](http://go.microsoft.com/fwlink/?linkid=94467)                                                                                                                                                                                              |
| **Shrnutí**                        | Tato důležitá aktualizace zabezpečení řeší veřejně oznámenou chybu zabezpečení. Byla zjištěna chyba zabezpečení ve Službách systému Windows pro systém UNIX 3.0, Službách systému Windows pro systém UNIX 3.5 a v Podsystému pro aplikace systému UNIX při spuštění určitých binárních souborů setuid, která může útočníkovi umožnit zvýšení úrovně oprávnění. |
| **Stupeň maximální závažnosti**    | [Vysoký](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                         |
| **Dopad této chyby zabezpečení**   | Zvýšení úrovně oprávnění                                                                                                                                                                                                                                                                                                                                       |
| **Rozpoznávání**                   | Nástroj Microsoft Baseline Security Analyzer a nástroj pro vyhledávání aktualizací v rozlehlých sítích (Enterprise Update Scan Tool – EST) rozezná, zda váš počítačový systém vyžaduje tuto aktualizaci. Aktualizace bude vyžadovat restartování počítače.                                                                                                     |
| **Software obsahující tuto chybu** | **Služby systému Windows pro systém UNIX, Podsystém pro aplikace systému UNIX.** Další informace získáte v části Software obsahující tuto chybu a umístění aktualizací ke stažení.                                                                                                                                                                             |

| Identifikátor bulletinu            | Bulletin zabezpečení společnosti Microsoft MS07-054                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
|------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Název bulletinu**                | [**Chyba zabezpečení v programu MSN Messenger a Windows Live Messenger umožňuje vzdálené spouštění kódu (942099)**](http://go.microsoft.com/fwlink/?linkid=100148)                                                                                                                                                                                                                                                                                                                                                                                                 |
| **Shrnutí**                        | Tato aktualizace zabezpečení řeší veřejně známou chybu zabezpečení v programu MSN Messenger a Windows Live Messenger. Tato chyba zabezpečení by mohla umožnit vzdálené spuštění kódu, pokud by uživatel přijal pozvání k relaci webové kamery nebo k video konverzaci od útočníka. Útočník, který by tuto chybu zabezpečení zneužil, může získat úplnou kontrolu nad ohroženým systémem. Uživatelé, jejichž účty jsou konfigurovány tak, aby měli v systému méně uživatelských práv, by byli vystaveni menšímu riziku než uživatelé s uživatelskými právy správce. |
| **Stupeň maximální závažnosti**    | [Vysoký](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| **Dopad této chyby zabezpečení**   | Vzdálené spuštění kódu                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| **Rozpoznávání**                   | Tyto produkty nabízejí integrovaný mechanismus pro automatické rozpoznávání a nasazování aktualizací. Aktualizace může vyžadovat restartování počítače.                                                                                                                                                                                                                                                                                                                                                                                                            |
| **Software obsahující tuto chybu** | **MSN Messenger, Windows Live Messenger.** Další informace získáte v části Software obsahující tuto chybu a umístění aktualizací ke stažení.                                                                                                                                                                                                                                                                                                                                                                                                                       |

Software obsahující tuto chybu a umístění aktualizací ke stažení
----------------------------------------------------------------


**Jak pracovat s touto tabulkou**

V této tabulce zjistíte, které aktualizace zabezpečení bude třeba nainstalovat. Přečtěte si seznam všech programů a součástí a zjistěte, zda jsou u nich vyžadovány aktualizace zabezpečení. Pokud se program nebo součást v seznamu nachází, je u nich uveden dopad chyby zabezpečení s odkazem na příslušnou aktualizaci.

**Poznámka:** Jedna chyba zabezpečení může vyžadovat instalaci více aktualizací. Přečtěte si celý sloupec u každého identifikátoru bulletinu. Zjistíte v něm, které aktualizace nainstalovat v závislosti na programech nebo součástech nainstalovaných ve vašem systému.

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
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS07-051**](http://go.microsoft.com/fwlink/?linkid=94667)
</td>
<td style="border:1px solid black;">
[**MS07-052**](http://go.microsoft.com/fwlink/?linkid=98460)
</td>
<td style="border:1px solid black;">
[**MS07-053**](http://go.microsoft.com/fwlink/?linkid=94467)
</td>
<td style="border:1px solid black;">
[**MS07-054**](http://go.microsoft.com/fwlink/?linkid=100148)
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
[**Důležité**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Důležité**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<th colspan="5" style="border:1px solid black;">
Operační systém Windows
</th>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Windows 2000 Service Pack 4
</td>
<td style="border:1px solid black;">
[Kritický](http://www.microsoft.com/downloads/details.aspx?familyid=7cd248ed-d154-4dce-89ef-ceefd2700965)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**1.0**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**1.0**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 1
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**1.0**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**1.0**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**1.0**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**1.0**
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
**1.0**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista x64 Edition
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**1.0**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<th colspan="5" style="border:1px solid black;">
Součásti operačního systému Windows
</th>
</tr>
<tr>
<td style="border:1px solid black;">
Služby systému Windows pro systém UNIX 3.0 v systému Windows 2000 Service Pack 4
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Vysoký](http://www.microsoft.com/downloads/details.aspx?familyid=557f89fc-c5d9-4405-9007-1654abf92277)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Služby systému Windows pro systém UNIX 3.5 v systému Windows 2000 Service Pack 4
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Vysoký](http://www.microsoft.com/downloads/details.aspx?familyid=70ae23c2-3ae8-4ea6-ba8d-8ac7e4f82663)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Služby systému Windows pro systém UNIX 3.0 v systému Windows XP Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Vysoký](http://www.microsoft.com/downloads/details.aspx?familyid=557f89fc-c5d9-4405-9007-1654abf92277)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Služby systému Windows pro systém UNIX 3.5 v systému Windows XP Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Vysoký](http://www.microsoft.com/downloads/details.aspx?familyid=70ae23c2-3ae8-4ea6-ba8d-8ac7e4f82663)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Služby systému Windows pro systém UNIX 3.0 v systémech Windows Server 2003 Service Pack 1 a Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Vysoký](http://www.microsoft.com/downloads/details.aspx?familyid=557f89fc-c5d9-4405-9007-1654abf92277)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Služby systému Windows pro systém UNIX 3.5 v systémech Windows Server 2003 Service Pack 1 a Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Vysoký](http://www.microsoft.com/downloads/details.aspx?familyid=70ae23c2-3ae8-4ea6-ba8d-8ac7e4f82663)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Podsystém pro aplikace systému UNIX v systému Windows Server 2003 Service Pack 1 a Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Vysoký](http://www.microsoft.com/downloads/details.aspx?familyid=8ab5cc43-0b9c-45eb-aa51-47568ab6ce3f)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Podsystém pro aplikace systému UNIX v systému Windows Server 2003 x64 Edition a Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Vysoký](http://www.microsoft.com/downloads/details.aspx?familyid=1d21e3e8-b5f6-4044-9db6-054af836492b)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Podsystém pro aplikace systému UNIX v systému Windows Vista
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Vysoký](http://www.microsoft.com/downloads/details.aspx?familyid=4d52e4f4-2888-42df-8163-85c648e65b29)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Podsystém pro aplikace systému UNIX v systému Windows Vista x64 Edition
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Vysoký](http://www.microsoft.com/downloads/details.aspx?familyid=4be667cc-c239-480b-a9a0-939bcd27f0de)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<th colspan="5" style="border:1px solid black;">
Vývojářské nástroje a platformy
</th>
</tr>
<tr>
<td style="border:1px solid black;">
Visual Studio .NET 2002 Service Pack 1  
(KB937057)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Vysoký](http://www.microsoft.com/downloads/details.aspx?familyid=2608c83b-e1b2-4449-9a0e-1e566aac3d76)**<sup>[2]</sup>**
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Visual Studio .NET 2003  
(KB937058)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Vysoký](http://www.microsoft.com/downloads/details.aspx?familyid=d612ad41-5a0d-4e13-99ea-d6a5589786d6)**<sup>[2]</sup>**
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Visual Studio .NET 2003 Service Pack 1  
(KB937059)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Vysoký](http://www.microsoft.com/downloads/details.aspx?familyid=0b10b04b-932c-4bff-9cbc-b3eeb15064b1)**<sup>[2]</sup>**
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Visual Studio 2005  
(KB937060)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Vysoký](http://www.microsoft.com/downloads/details.aspx?familyid=21073cc2-919c-40df-8ebb-aa3db06050d2)**<sup>[2]</sup>**
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Visual Studio 2005 Service Pack 1  
(KB937061)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Vysoký](http://www.microsoft.com/downloads/details.aspx?familyid=967d43c8-efba-4221-beb0-981e7deef33a)**<sup>[2]</sup>**
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<th colspan="5" style="border:1px solid black;">
Další software obsahující tuto chybu
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
MSN Messenger 6.2 v systému Microsoft Windows 2000 Service Pack 4
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Vysoký](http://www.microsoft.com/downloads/details.aspx?familyid=cf49c56c-8b3e-4eae-9904-9505f47bed45&displaylang=en)**<sup>[3]</sup>**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
MSN Messenger 7.0 v systému Windows 2000 Service Pack 4
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Vysoký](http://www.microsoft.com/downloads/details.aspx?familyid=cf49c56c-8b3e-4eae-9904-9505f47bed45&displaylang=en)**<sup>[3]</sup>**
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
MSN Messenger 6.2 v systému Windows XP Service Pack 2, Windows XP Professional x64 Edition, Windows XP Professional x64 Edition Service Pack 2, Windows Server 2003 Service Pack 1, Windows Server 2003 Service Pack 2, Windows Server 2003 x64 Edition, Windows Server 2003 x64 Edition Service Pack 2, Windows Vista a Windows Vista x64 Edition
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Vysoký](http://www.microsoft.com/downloads/details.aspx?familyid=d78f2ff1-79ea-4066-8ba0-ddbed94864fc&displaylang=en)**<sup>[3]</sup>**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
MSN Messenger 7.0 v systému Windows XP Service Pack 2, Windows XP Professional x64 Edition, Windows XP Professional x64 Edition Service Pack 2, Windows Server 2003 Service Pack 1, Windows Server 2003 Service Pack 2, Windows Server 2003 x64 Edition, Windows Server 2003 x64 Edition Service Pack 2, Windows Vista a Windows Vista x64 Edition
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Vysoký](http://www.microsoft.com/downloads/details.aspx?familyid=d78f2ff1-79ea-4066-8ba0-ddbed94864fc&displaylang=en)**<sup>[3]</sup>**
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
MSN Messenger 7.5 v systému Windows XP Service Pack 2, Windows XP Professional x64 Edition, Windows XP Professional x64 Edition Service Pack 2, Windows Server 2003 Service Pack 1, Windows Server 2003 Service Pack 2, Windows Server 2003 x64 Edition, Windows Server 2003 x64 Edition Service Pack 2, Windows Vista a Windows Vista x64 Edition
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Vysoký](http://www.microsoft.com/downloads/details.aspx?familyid=d78f2ff1-79ea-4066-8ba0-ddbed94864fc&displaylang=en)**<sup>[3]</sup>**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Live Messenger 8.0 v systému Windows XP Service Pack 2, Windows XP Professional x64 Edition, Windows XP Professional x64 Edition Service Pack 2, Windows Server 2003 Service Pack 1, Windows Server 2003 Service Pack 2, Windows Server 2003 x64 Edition, Windows Server 2003 x64 Edition Service Pack 2, Windows Vista a Windows Vista x64 Edition
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Vysoký](http://www.microsoft.com/downloads/details.aspx?familyid=d78f2ff1-79ea-4066-8ba0-ddbed94864fc&displaylang=en)**<sup>[3]</sup>**
</td>
</tr>
</table>
 
**Poznámky**

**<sup>[1]</sup>** Pro tento operační systém je k dispozici aktualizace zabezpečení. Další informace získáte v tabulce u softwaru nebo součásti obsahující tuto chybu a v příslušném bulletinu zabezpečení.

**<sup>[2]</sup>** Tato chyba zabezpečení se netýká všech verzí sady Visual Studio. Konkrétní seznam postižených vydání naleznete v příslušném bulletinu zabezpečení.

**<sup>[3]</sup>** U tohoto softwaru je dostupná také možnost provést online upgrade z programu MSN Messenger nebo Windows Live Messenger. Další informace získáte v příslušném bulletinu zabezpečení.

Nástroje a doporučené postupy zjišťování a nasazení
---------------------------------------------------


**Centrum zabezpečení**

Umožňuje správu aktualizací softwaru a zabezpečení, které je třeba nainstalovat na servery, stolní počítače a přenosné počítače v organizaci. Další informace naleznete na webu [TechNet Update Management Center](http://go.microsoft.com/fwlink/?linkid=69903). Další informace o zabezpečení produktů společnosti Microsoft nabízí web [Centrum zabezpečení TechNet](http://go.microsoft.com/fwlink/?linkid=21171). Tyto informace lze také získat klepnutím na nabídku „Nejnovější aktualizace zabezpečení“ na webu [Zabezpečení doma](http://go.microsoft.com/fwlink/?linkid=85102).

Aktualizace zabezpečení jsou k dispozici na webu [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747), [Windows Update](http://go.microsoft.com/fwlink/?linkid=21130) a [Office Update](http://go.microsoft.com/fwlink/?linkid=21135). Aktualizace zabezpečení jsou také k dispozici na webu [služby Stažení softwaru](http://go.microsoft.com/fwlink/?linkid=21129). Nejsnadněji je naleznete hledáním podle klíčového slova oprava\_zabezpečení (security\_patch). Aktualizace zabezpečení lze mimo jiné stáhnout z katalogu služby Windows Update. Další informace o katalogu systému Windows Update získáte v [článku 323166 znalostní báze Microsoft Knowledge Base](http://support.microsoft.com/kb/323166).

**Doporučené postupy zjišťování a instalace**

Společnost Microsoft poskytla doporučené postupy zjišťování a instalace aktualizací zabezpečení vydaných tento měsíc. Tyto doporučené postupy by měly pomoci také odborníkům v oblasti IT při používání různých nástrojů při instalaci aktualizace zabezpečení, např. Windows Update, Microsoft Update, Office Update, nástroj MBSA (Microsoft Baseline Security Analyzer), nástroj pro rozpoznávání sady Office, Microsoft Systems Management Server (SMS), nástroj Extended Security Update Inventory Tool a nástroj pro vyhledávání aktualizací v rozlehlých sítích (Enterprise Update Scanning Tool – EST). Další informace získáte v [článku 910723 znalostní báze Microsoft Knowledge Base](http://support.microsoft.com/kb/910723).

**Nástroj MBSA (Microsoft Baseline Security Analyzer) a** **nástroj pro vyhledávání aktualizací v rozlehlých sítích (Enterprise** **Update Scan Tool**

Pomocí nástroje Microsoft Baseline Security Analyzer (MBSA) mohou správci prohledávat místní i vzdálené systémy a zjistit tak, jestli v nich nechybí některé aktualizace zabezpečení nebo jestli v nastavení zabezpečení systému nedošlo k některým běžným chybám. Další informace o nástroji MBSA získáte na webu [Microsoft Baseline Security Analyzer](http://go.microsoft.com/fwlink/?linkid=21134).

Pokud nástroj MBSA 1.2.1 nepodporuje zjišťování určité aktualizace zabezpečení, společnost Microsoft vydá verzi nástroje pro vyhledávání aktualizací v rozlehlých sítích (Enterprise Update Scan Tool – EST) pro danou aktualizaci zabezpečení. Další informace o nástroji EST najdete na webu [Enterprise Update Scan Tool](http://support.microsoft.com/default.aspx?id=894193).

**Poznámka:** Po 9. říjnu 2007 už nebude aktualizován soubor MSSecure.XML používaný nástrojem MBSA 1.2.1. Po tomto datu nebudou do souboru MSSecure.XML používaného nástrojem MBSA 1.2.1 přidávány žádné nové aktualizace zabezpečení a nebudou vydávány nové verze nástroje EST. Další informace získáte na webu [Microsoft Baseline Security Analyzer](http://go.microsoft.com/fwlink/?linkid=21134).

**Služba Windows Server Update Services**

Pomocí služby Windows Server Update Services (WSUS) mohou správci systémů rychle a spolehlivě instalovat nejnovější důležité aktualizace zabezpečení pro systémy Windows 2000 a novější, sadu Office XP a novější, Exchange Server 2003 a SQL Server 2000 do systémů Windows 2000 a novějších.

Další informace o způsobu instalace této aktualizace zabezpečení pomocí služby Windows Server Update Services získáte na webu služby [Windows Server Update Services](http://go.microsoft.com/fwlink/?linkid=50120).

**Systems Management Server**

Microsoft Systems Management Server (SMS) představuje v rozlehlých sítích řešení pro správu aktualizací s rozsáhlými možnostmi konfigurace. Umožňuje správcům identifikovat počítače se systémem Windows, které vyžadují aktualizace zabezpečení, a provést řízenou instalaci těchto aktualizací v celé rozlehlé síti s minimálním dopadem na koncové uživatele. Další informace o tom, jak mohou správci pomocí serveru SMS 2003 nasazovat aktualizace zabezpečení, získáte na webu [Správa oprav zabezpečení pomocí serveru SMS 2003 (SMS 2003 Security Patch Management)](http://go.microsoft.com/fwlink/?linkid=22939). Uživatelé serveru SMS 2.0 mohou při nasazení aktualizací zabezpečení použít také sadu [Software Updates Services Feature Pack](http://go.microsoft.com/fwlink/?linkid=33340). Další informace o serveru SMS získáte na webu [Microsoft Systems Management Server](http://go.microsoft.com/fwlink/?linkid=21158).

**Poznámka:** Server SMS využívá nástroj MBSA (Microsoft Baseline Security Analyzer) a nástroj pro rozpoznávání sady Microsoft Office, a poskytuje tak širokou podporu pro zjišťování a instalaci aktualizací uvedených v bulletinech zabezpečení. Tyto nástroje nemusí některé softwarové aktualizace zjistit. V takovém případě mohou správci použít funkce serveru SMS a nasměrovat aktualizace do určitých systémů. Další informace o tomto postupu najdete na webu [Nasazení aktualizací softwaru pomocí funkce Distribuce softwaru serveru SMS](http://go.microsoft.com/fwlink/?linkid=33341). Některé aktualizace zabezpečení vyžadují po restartování počítače oprávnění správce. Správci mohou k instalaci těchto aktualizací použít nástroj Elevated Rights Deployment Tool (k dispozici v sadě [SMS 2003 Administration Feature Pack](http://go.microsoft.com/fwlink/?linkid=33387) a [SMS 2.0 Administration Feature Pack](http://go.microsoft.com/fwlink/?linkid=21161)).

### Další informace

#### Nástroj pro odstranění škodlivého softwaru systému Microsoft Windows

Společnost Microsoft vydává aktualizovanou verzi Nástroje pro odstranění škodlivého softwaru systému Microsoft Windows na webu Windows Update, Microsoft Update, ve službě Windows Server Update Services a v centru pro stahování Download Center.

#### Důležité aktualizace nesouvisející se zabezpečením na webu Microsoft Update (MU), Windows Update (WU) a ve službě Windows Server Update Services (WSUS)

Tento měsíc:

-   Společnost Microsoft nevydala žádnou důležitou aktualizaci **nesouvisející se zabezpečením** na webu Microsoft Update (MU) a ve službě Windows Server Update Services (WSUS).
-   Společnost Microsoft nevydala žádnou důležitou aktualizaci systému Windows **nesouvisející se zabezpečením** na webu Windows Update (WU).

Tato informace se týká **pouze** důležitých aktualizací **nesouvisejících se zabezpečením** na webu Microsoft Update, Windows Update a ve službě Windows Server Update Services vydaných ve stejný den jako souhrnný bulletin zabezpečení. Informace **se netýká** aktualizací **nesouvisejících se zabezpečením** vydaných v jiné dny.

#### Strategie zabezpečení a komunita

**Strategie instalace aktualizací**

Web [Doporučené postupy zabezpečení pro správu oprav (Security Guidance for Patch Management)](http://go.microsoft.com/fwlink/?linkid=21168) obsahuje další informace o instalaci aktualizací zabezpečení podle doporučení společnosti Microsoft.

**Získání dalších aktualizací zabezpečení**

Aktualizace odstraňující další problémy se zabezpečením získáte v následujících umístěních:

-   Aktualizace zabezpečení jsou k dispozici na webu služby [Stažení softwaru (Microsoft Download Center)](http://go.microsoft.com/fwlink/?linkid=21129). Nejsnadněji je naleznete vyhledáním klíčového slova security\_patch (oprava\_zabezpečení).
-   Aktualizace pro klientské platformy jsou k dispozici na webu [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747).
-   Aktualizace zabezpečení nabízené tento měsíc na webu Windows Update jsou k dispozici na webu služby Stažení softwaru v souborech obrazu ISO disku CD s vydanými aktualizacemi zabezpečení a kritickými aktualizacemi. Další informace získáte v [článku 913086 znalostní báze Microsoft Knowledge Base](http://support.microsoft.com/kb/913086).

**Komunita odborníků v oblasti zabezpečení**

Můžete se zde naučit, jak zlepšit zabezpečení a jak optimalizovat infrastrukturu IT. Také můžete s dalšími členy komunity IT Pro diskutovat o bezpečnostních tématech na webu [Komunita odborníků v oblasti zabezpečení (IT Pro Security Community)](http://go.microsoft.com/fwlink/?linkid=21164).

#### Poděkování

Společnost Microsoft tímto [děkuje](http://go.microsoft.com/fwlink/?linkid=21127) za spolupráci při ochraně zákazníků:

-   Týmu zaměřenému na chyby zabezpečení ze společnosti [Assurent Secure Technologies](http://www.assurent.com/) za oznámení chyby popsané v bulletinu [MS07-051](http://go.microsoft.com/fwlink/?linkid=94667)
-   Yamatu Liovi ze společnosti [Palo Alto Networks](http://www.paloaltonetworks.com/) za oznámení chyby popsané v bulletinu [MS07-051](http://go.microsoft.com/fwlink/?linkid=94667)
-   Anonymnímu výzkumníkovi spolupracujícímu se společností [iDefense VCP](http://labs.idefense.com/) za oznámení chyby popsané v bulletinu [MS07-051](http://go.microsoft.com/fwlink/?linkid=94667).
-   Brianu A. Reiterovi ze společnosti WolfeReiter za spolupráci na řešení chyby oznámené v bulletinu [MS07-053](http://go.microsoft.com/fwlink/?linkid=94467)
-   Woo Shiovi z [týmu 509](http://www.team509.com/) za oznámení chyby popsané v bulletinu [MS07-054](http://go.microsoft.com/fwlink/?linkid=100148)

#### Technická podpora

-   Uvedený software byl testován za účelem zjištění, kterých verzí se chyba týká. U dalších verzí skončila časově omezená podpora. Pokud chcete zjistit dobu, po kterou je pro určitou verzi softwaru poskytována podpora, navštivte web [Zásady poskytování technické podpory pro produkty společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=21742).
-   Zákazníci mohou získat technickou podporu na webu [služby technické podpory společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=21131). Hovory související s aktualizacemi zabezpečení jsou bezplatné.
-   Mezinárodní zákazníci získají podporu u místních zastoupení společnosti Microsoft. Technická podpora související s aktualizacemi zabezpečení je bezplatná. Další informace o možnostech kontaktování společnosti Microsoft v případě potřeby technické podpory získáte na [webu mezinárodní technické podpory](http://go.microsoft.com/fwlink/?linkid=21155).

#### Zřeknutí se záruky

Informace ve znalostní bázi Microsoft Knowledge Base jsou poskytovány tak, jak jsou, bez jakékoli záruky. Společnost Microsoft neposkytuje žádné záruky, výslovně uvedené či mlčky předpokládané, včetně záruk obchodovatelnosti a vhodnosti pro určitý účel. Společnost Microsoft ani její dodavatelé nenesou v žádném případě zodpovědnost za žádné škody, včetně přímých, nepřímých, náhodných či následných škod, ztráty zisku či zvláštních škod, a to ani v případě, že byli na možnost takových škod upozorněni. V některých zemích a právních řádech není dovoleno vyloučit nebo omezit odpovědnost, proto se výše uvedené omezení na vás nemusí vztahovat.

#### Revize

-   V1.0 (11. září 2007): Souhrnný bulletin byl publikován.
-   V1.1 (12. září 2007): Byla pozměněna informace o nutnosti restartování a přidány odkazy na soubory ke stažení pro bulletin MS07-045.

*Built at 2014-04-18T01:50:00Z-07:00*
