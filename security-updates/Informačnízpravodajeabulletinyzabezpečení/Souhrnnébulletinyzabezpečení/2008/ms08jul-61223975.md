---
TOCTitle: 'MS08-JUL'
Title: 'Souhrnný bulletin zabezpečení společnosti Microsoft, červenec 2008'
ms:assetid: 'ms08-jul'
ms:contentKeyID: 61223975
ms:mtpsurl: 'https://technet.microsoft.com/cs-CZ/library/ms08-jul(v=Security.10)'
---

Security Bulletin Summary

Souhrnný bulletin zabezpečení společnosti Microsoft, červenec 2008
==================================================================

Publikováno: 8. července 2008 | Aktualizováno: 11. února 2009

**Verze:** 1.1

Tento souhrnný bulletin uvádí bulletiny zabezpečení vydané v červenci 2008.

Spolu s vydáním bulletinů pro červenec 2008 nahrazuje tento souhrnný bulletin předběžné oznámení o bulletinech vydané 3. července 2008. Další informace o službě předběžného oznámení o bulletinech naleznete v části [Předběžné oznámení o bulletinech zabezpečení společnosti Microsoft](http://technet.microsoft.com/security/bulletin/advance).

Informace o tom, jak dostávat automatická oznámení o vydání nových bulletinů zabezpečení společnosti Microsoft, naleznete na webu [Zasílání technických oznámení o zabezpečení společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=21163).

Pro zodpovězení zákaznických dotazů týkajících se těchto bulletinů uspořádá společnost Microsoft webové vysílání 9. července 2008 v 11:00 časového pásma Tichomoří (USA a Kanada). [Registrovat se pro webové vysílání týkající se červencových bulletinů zabezpečení](http://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032374629&culture=en-us). Po tomto datu je webové vysílání dostupné na požádání. Další informace získáte v [souhrnných bulletinech zabezpečení společnosti Microsoft a webovém vysílání](http://technet.microsoft.com/security/bulletin/summary).

Společnost Microsoft se snaží zákazníkům usnadnit upřednostnění měsíčně vydávaných aktualizací zabezpečení před jakýmikoli důležitými aktualizacemi nesouvisejícími se zabezpečením, které jsou vydány ve stejný den jako měsíčně vydávané aktualizace zabezpečení. Další informace získáte v části **Další informace**.

### Informace o bulletinech

#### Shrnutí

Bulletiny zabezpečení podle závažnosti:

Vysoký (4)
----------

 

| Identifikátor bulletinu            | Bulletin zabezpečení společnosti Microsoft MS08-040                                                                                                                                                                                                                                                                                                           |
|------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Název bulletinu**                | [**Chyby zabezpečení serveru Microsoft SQL Server umožňují zvýšení úrovně oprávnění (941203)**](http://go.microsoft.com/fwlink/?linkid=113725)                                                                                                                                                                                                                |
| **Shrnutí**                        | Tato aktualizace zabezpečení řeší čtyři chyby zabezpečení oznámené soukromými osobami. Závažnější z těchto chyb zabezpečení mohou útočníkovi umožnit spuštění kódu a převzetí úplné kontroly nad postiženým systémem. Ověřený útočník by tak mohl instalovat programy, zobrazovat, měnit či odstraňovat data nebo vytvářet nové účty s úplnými právy správce. |
| **Stupeň maximální závažnosti**    | [Vysoký](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                        |
| **Dopad této chyby zabezpečení**   | Zvýšení úrovně oprávnění                                                                                                                                                                                                                                                                                                                                      |
| **Rozpoznávání**                   | Pomocí nástroje MBSA (Microsoft Baseline Security Analyzer) lze určit, zda počítačový systém potřebuje tuto aktualizaci. Aktualizace může vyžadovat restartování počítače.                                                                                                                                                                                    |
| **Software obsahující tuto chybu** | **Microsoft Windows, Microsoft SQL Server.** Další informace získáte v části Software obsahující tuto chybu a umístění aktualizací ke stažení.                                                                                                                                                                                                                |

| Identifikátor bulletinu            | Bulletin zabezpečení společnosti Microsoft MS08-038                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
|------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Název bulletinu**                | [**Chyba zabezpečení v programu Průzkumník Windows umožňuje vzdálené spuštění kódu (950582)**](http://go.microsoft.com/fwlink/?linkid=117296)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| **Shrnutí**                        | Tato aktualizace zabezpečení řeší veřejně oznámenou chybu zabezpečení týkající se programu Průzkumník Windows, která může způsobit vzdálené spuštění kódu, jakmile je otevřen a uložen speciálně vytvořený soubor uložených výsledků hledání. Pokud by byl uživatel přihlášen s uživatelskými právy správce, mohl by útočník, který by tuto chybu zabezpečení zneužil, získat úplnou kontrolu nad postiženým systémem. Útočník by tak mohl instalovat programy, zobrazovat, měnit či odstraňovat data nebo vytvářet nové účty s úplnými uživatelskými právy. Uživatelé, jejichž účty jsou konfigurovány tak, aby měli v systému méně uživatelských práv, by byli vystaveni menšímu riziku než uživatelé s uživatelskými právy správce. |
| **Stupeň maximální závažnosti**    | [Vysoký](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| **Dopad této chyby zabezpečení**   | Vzdálené spuštění kódu                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| **Rozpoznávání**                   | Pomocí nástroje MBSA (Microsoft Baseline Security Analyzer) lze určit, zda počítačový systém potřebuje tuto aktualizaci. Tato aktualizace vyžaduje restartování.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| **Software obsahující tuto chybu** | **Microsoft Windows.** Další informace získáte v části Software obsahující tuto chybu a umístění aktualizací ke stažení.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |

| Identifikátor bulletinu            | Bulletin zabezpečení společnosti Microsoft MS08-037                                                                                                                                                                                                                                                                                                                                              |
|------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Název bulletinu**                | [**Chyby zabezpečení serveru DNS umožňují umístění falešného obsahu (953230)**](http://go.microsoft.com/fwlink/?linkid=119620)                                                                                                                                                                                                                                                                   |
| **Shrnutí**                        | Tato aktualizace zabezpečení řeší dvě chyby zabezpečení služby DNS (Domain Name System) systému Windows oznámené soukromými osobami, které by mohly umožňovat umístění falešného obsahu. Tyto chyby zabezpečení existují jak u klienta, tak i serveru DNS a mohly by umožnit vzdálenému útočníkovi přesměrovat síťovou komunikaci určenou pro systémy v Internetu do vlastních systémů útočníka. |
| **Stupeň maximální závažnosti**    | [Vysoký](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                           |
| **Dopad této chyby zabezpečení**   | Vkládání falešného obsahu                                                                                                                                                                                                                                                                                                                                                                        |
| **Rozpoznávání**                   | Pomocí nástroje MBSA (Microsoft Baseline Security Analyzer) lze určit, zda počítačový systém potřebuje tuto aktualizaci. Tato aktualizace vyžaduje restartování.                                                                                                                                                                                                                                 |
| **Software obsahující tuto chybu** | **Microsoft Windows.** Další informace získáte v části Software obsahující tuto chybu a umístění aktualizací ke stažení.                                                                                                                                                                                                                                                                         |

| Identifikátor bulletinu            | Bulletin zabezpečení společnosti Microsoft MS08-039                                                                                                                                                                                                                                                                                                                                                                                                                                 |
|------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Název bulletinu**                | [**Chyby zabezpečení v aplikaci Outlook Web Access pro Exchange Server umožňují zvýšení úrovně oprávnění (953747)**](http://go.microsoft.com/fwlink/?linkid=120820)                                                                                                                                                                                                                                                                                                                 |
| **Shrnutí**                        | Tato aktualizace zabezpečení řeší dvě chyby zabezpečení v aplikaci Outlook Web Access (OWA) pro Microsoft Exchange Server oznámené soukromou osobou. Útočník, který by tyto chyby zabezpečení úspěšně zneužil, by mohl získat přístup k datům relace samostatného klienta aplikace Outlook Web Access, což by umožnilo zvýšení úrovně oprávnění. Útočník by pak mohl provést libovolné akce, které může v relaci samostatného klienta aplikace Outlook Web Access provést uživatel. |
| **Stupeň maximální závažnosti**    | [Vysoký](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                              |
| **Dopad této chyby zabezpečení**   | Zvýšení úrovně oprávnění                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| **Rozpoznávání**                   | Pomocí nástroje MBSA (Microsoft Baseline Security Analyzer) lze určit, zda počítačový systém potřebuje tuto aktualizaci. Aktualizace může vyžadovat restartování počítače.                                                                                                                                                                                                                                                                                                          |
| **Software obsahující tuto chybu** | **Microsoft Windows.** Další informace získáte v části Software obsahující tuto chybu a umístění aktualizací ke stažení.                                                                                                                                                                                                                                                                                                                                                            |

Software obsahující tuto chybu a umístění aktualizací ke stažení
----------------------------------------------------------------

 
**Jak pracovat s touto tabulkou**

V této tabulce zjistíte, které aktualizace zabezpečení bude třeba nainstalovat. Přečtěte si seznam všech programů a komponent a zjistěte, zda jsou u nich vyžadovány aktualizace zabezpečení. Pokud se program nebo komponenta v seznamu nachází, je v něm zároveň uveden odkaz na dostupnou aktualizaci softwaru a také stupeň závažnosti aktualizace softwaru.

**Poznámka:** Jedna chyba zabezpečení může vyžadovat instalaci více aktualizací. Přečtěte si celý sloupec u každého identifikátoru bulletinu. Zjistíte v něm, které aktualizace nainstalovat v závislosti na programech nebo součástech nainstalovaných ve vašem systému.

#### Operační systém Windows

 
<p></p>
<table style="border:1px solid black;">
<tr class="thead">
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
</tr>
<tr>
<th style="border:1px solid black;" colspan="4" >
Microsoft Windows 2000
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS08-040**](http://go.microsoft.com/fwlink/?linkid=113725)
</td>
<td style="border:1px solid black;">
[**MS08-038**](http://go.microsoft.com/fwlink/?linkid=117296)
</td>
<td style="border:1px solid black;">
[**MS08-037**](http://go.microsoft.com/fwlink/?linkid=119620)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Stupeň maximální závažnosti bulletinu**
</td>
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Windows 2000 Service Pack 4
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Aktualizace klienta DNS:  
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=269c219c-9d6b-4b12-b621-c70cd07cdd22)  
(Důležitý)  
Aktualizace serveru DNS:  
[Microsoft Windows 2000 Server Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=332aa92f-a1ad-42a0-87d0-485d2d41335b)  
(Důležitý)
</td>
</tr>
<tr>
<th style="border:1px solid black;" colspan="4" >
Windows XP
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS08-040**](http://go.microsoft.com/fwlink/?linkid=113725)
</td>
<td style="border:1px solid black;">
[**MS08-038**](http://go.microsoft.com/fwlink/?linkid=117296)
</td>
<td style="border:1px solid black;">
[**MS08-037**](http://go.microsoft.com/fwlink/?linkid=119620)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Stupeň maximální závažnosti**
</td>
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Service Pack 2 a Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Aktualizace klienta DNS:  
[Windows XP Service Pack 2 a Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=ed989a33-7a9e-4423-93a8-b38907467cdf)  
(Důležitý)  
Serveru DNS se žádná aktualizace netýká
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Professional x64 Edition a Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Aktualizace klienta DNS:  
[Windows XP Professional x64 Edition a Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=a2b016fa-b108-4e8e-b41b-4ca89002907b)  
(Důležitý)  
Serveru DNS se žádná aktualizace netýká
</td>
</tr>
<tr>
<th style="border:1px solid black;" colspan="4" >
Windows Server 2003
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS08-040**](http://go.microsoft.com/fwlink/?linkid=113725)
</td>
<td style="border:1px solid black;">
[**MS08-038**](http://go.microsoft.com/fwlink/?linkid=117296)
</td>
<td style="border:1px solid black;">
[**MS08-037**](http://go.microsoft.com/fwlink/?linkid=119620)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Stupeň maximální závažnosti bulletinu**
</td>
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 1 a Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft SQL Server 2000 Desktop Engine (WMSDE)](http://www.microsoft.com/downloads/details.aspx?familyid=1c0ae18b-1f17-44b3-a337-b36e7de437a7)  
(KB948110)  
(Důležitý)  
[Interní databáze systému Windows (WYukon) Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=48f6aaa5-49fc-4a16-bc34-8514e214b8cf)  
(KB948109)  
(Důležitý)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Aktualizace klienta DNS:  
[Windows Server 2003 Service Pack 1 a Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4ef5033c-9843-4e0b-bfad-fcaf05d7dab9)  
(Důležitý)  
Aktualizace serveru DNS:  
[Windows Server 2003 Service Pack 1 a Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d1fcb794-e6a5-4c28-b3b3-9cd88f468a42)  
(Důležitý)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition a Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft SQL Server 2000 Desktop Engine (WMSDE)](http://www.microsoft.com/downloads/details.aspx?familyid=1c0ae18b-1f17-44b3-a337-b36e7de437a7)  
(KB948110)  
(Důležitý)  
[Interní databáze systému Windows (WYukon) x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=48f6aaa5-49fc-4a16-bc34-8514e214b8cf)  
(KB948109)  
(Důležitý)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Aktualizace klienta DNS:  
[Windows Server 2003 x64 Edition and Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=66624a1f-38bf-4af7-936d-3131474ffe1f)  
(Důležitý)  
Aktualizace serveru DNS:  
[Windows Server 2003 x64 Edition and Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=040a1ba8-21b0-439e-bf21-1acd1c43b162)  
(Důležitý)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 SP1 pro systémy s procesorem Itanium a Windows Server 2003 SP2 pro systémy s procesorem Itanium
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Aktualizace klienta DNS:  
[Windows Server 2003 SP1 pro systémy s procesorem Itanium a Windows Server 2003 SP2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=facc80da-61d6-49c5-872d-a1980b66ae3e)  
(Důležitý)  
Aktualizace serveru DNS:  
[Windows Server 2003 SP1 pro systémy s procesorem Itanium a Windows Server 2003 SP2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=c63e3ee6-6055-4313-b0f1-fec7408886bb)  
(Důležitý)
</td>
</tr>
<tr>
<th style="border:1px solid black;" colspan="4" >
Windows Vista
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS08-040**](http://go.microsoft.com/fwlink/?linkid=113725)
</td>
<td style="border:1px solid black;">
[**MS08-038**](http://go.microsoft.com/fwlink/?linkid=117296)
</td>
<td style="border:1px solid black;">
[**MS08-037**](http://go.microsoft.com/fwlink/?linkid=119620)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Stupeň maximální závažnosti bulletinu**
</td>
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista a Windows Vista Service Pack 1
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Vista a Windows Vista Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=06739ca6-7368-4acb-bb67-7e8146071a29)  
(Důležitý)
</td>
<td style="border:1px solid black;">
Klienta DNS se žádná aktualizace netýká  
Serveru DNS se žádná aktualizace netýká
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista x64 Edition a Windows Vista x64 Edition Service Pack 1
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition a Windows Vista x64 Edition Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=74ea0893-7c2f-4fad-ad27-588ad953b046)  
(Důležitý)
</td>
<td style="border:1px solid black;">
Klienta DNS se žádná aktualizace netýká  
Serveru DNS se žádná aktualizace netýká
</td>
</tr>
<tr>
<th style="border:1px solid black;" colspan="4" >
Windows Server 2008
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS08-040**](http://go.microsoft.com/fwlink/?linkid=113725)
</td>
<td style="border:1px solid black;">
[**MS08-038**](http://go.microsoft.com/fwlink/?linkid=117296)
</td>
<td style="border:1px solid black;">
[**MS08-037**](http://go.microsoft.com/fwlink/?linkid=119620)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Stupeň maximální závažnosti bulletinu**
</td>
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 pro 32bitové systémy
</td>
<td style="border:1px solid black;">
[Interní databáze systému Windows (WYukon) Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=48f6aaa5-49fc-4a16-bc34-8514e214b8cf)\*  
(KB948109)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro 32bitové systémy](http://www.microsoft.com/downloads/details.aspx?familyid=189a4170-b495-4904-9cbd-209e7494d303)\*  
(Důležitý)
</td>
<td style="border:1px solid black;">
Klienta DNS se žádná aktualizace netýká  
Aktualizace serveru DNS:  
[Windows Server 2008 pro 32bitové systémy](http://www.microsoft.com/downloads/details.aspx?familyid=1fcea8f4-b233-42e1-b913-c4fcae276c7b)\*  
(Důležitý)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 pro systémy s procesorem x64
</td>
<td style="border:1px solid black;">
[Interní databáze systému Windows (WYukon) x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=48f6aaa5-49fc-4a16-bc34-8514e214b8cf)\*  
(KB948109)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem x64](http://www.microsoft.com/downloads/details.aspx?familyid=85d8701d-f8c7-4079-8a21-a3a9d5ba71ce)\*  
(Důležitý)
</td>
<td style="border:1px solid black;">
Klienta DNS se žádná aktualizace netýká  
Aktualizace serveru DNS:  
[Windows Server 2008 pro systémy s procesorem x64](http://www.microsoft.com/downloads/details.aspx?familyid=afac5bbc-71fa-457b-8b0a-f5902d37bfd0)\*  
(Důležitý)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 pro systémy s procesorem Itanium
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=b30ee4f0-850f-4ff3-86a4-663603a0a802)  
(Důležitý)
</td>
<td style="border:1px solid black;">
Klienta DNS se žádná aktualizace netýká  
Serveru DNS se žádná aktualizace netýká
</td>
</tr>
</table>
<p></p>
 
**\*Instalace Server Core operačního systému Windows Server 2008 obsahující tuto chybu.** Tato aktualizace se týká všech podporovaných vydání systému Windows Server 2008 se stejným stupněm závažnosti, ať už byl systém Windows Server 2008 instalován pomocí možnosti instalace Server Core či nikoli. Více informací o této možnosti instalace naleznete v části [Server Core](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx). Možnost instalace Server Core se nevztahuje na určité edice systému Windows Server 2008. Další informace naleznete v části [Porovnání možností instalace Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

#### Microsoft Server Software

 
<p></p>
<table style="border:1px solid black;">
<caption>Microsoft SQL Server</caption>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Identifikátor bulletinu</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=113725"><strong>MS08-040</strong></a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Stupeň maximální závažnosti bulletinu</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Vysoký</strong></a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">SQL Server 7.0 Service Pack 4</td>
<td style="border:1px solid black;">Aktualizace GDR:<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=c95b2cb3-51a4-44e4-b9f4-9416e9ce16a0">SQL Server 7.0 Service Pack 4</a><br />
(KB948113)<br />
(Důležitý)<br />
<br />
Aktualizace QFE:<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=c95b2cb3-51a4-44e4-b9f4-9416e9ce16a0">SQL Server 7.0 Service Pack 4</a><br />
(KB948113)<br />
(Důležitý)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">SQL Server 2000 Service Pack 4</td>
<td style="border:1px solid black;">Aktualizace GDR:<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=4fd1f86a-94a2-43d8-9b0a-774c81426d9e">SQL Server 2000 Service Pack 4</a><br />
(KB948110)<br />
(Důležitý)<br />
<br />
Aktualizace QFE:<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=8316bc5e-8c2d-4710-8acc-b815ccc81cd4">SQL Server 2000 Service Pack 4</a><br />
(KB948111)<br />
(Důležitý)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">SQL Server 2000 pro systémy s procesorem Itanium Service Pack 4</td>
<td style="border:1px solid black;">Aktualizace GDR:<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=4fd1f86a-94a2-43d8-9b0a-774c81426d9e">SQL Server 2000 pro systémy s procesorem Itanium Service Pack 4</a><br />
(KB948110)<br />
(Důležitý)<br />
<br />
Aktualizace QFE:<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=8316bc5e-8c2d-4710-8acc-b815ccc81cd4">SQL Server 2000 pro systémy s procesorem Itanium Service Pack 4</a><br />
(KB948111)<br />
(Důležitý)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">SQL Server 2005 Service Pack 2</td>
<td style="border:1px solid black;">Aktualizace GDR:<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=4c9851cc-2c4c-4190-872c-84993a7623b7">SQL Server 2005 Service Pack 2</a><br />
(KB948109)<br />
(Důležitý)<br />
<br />
Aktualizace QFE:<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=a60bb7e7-ef4e-4cbd-b63a-0ad7bd1402b3">SQL Server 2005 Service Pack 2</a><br />
(KB948108)<br />
(Důležitý)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">SQL Server 2005 x64 Edition Service Pack 2</td>
<td style="border:1px solid black;">Aktualizace GDR:<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=4c9851cc-2c4c-4190-872c-84993a7623b7">SQL Server 2005 x64 Edition Service Pack 2</a><br />
(KB948109)<br />
(Důležitý)<br />
<br />
Aktualizace QFE:<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=a60bb7e7-ef4e-4cbd-b63a-0ad7bd1402b3">SQL Server 2005 x64 Edition Service Pack 2</a><br />
(KB948108)<br />
(Důležitý)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">SQL Server 2005 SP2 pro systémy s procesorem Itanium</td>
<td style="border:1px solid black;">Aktualizace GDR:<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=4c9851cc-2c4c-4190-872c-84993a7623b7">SQL Server 2005 SP2 pro systémy s procesorem Itanium</a><br />
(KB948109)<br />
(Důležitý)<br />
<br />
Aktualizace QFE:<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=a60bb7e7-ef4e-4cbd-b63a-0ad7bd1402b3">SQL Server 2005 SP2 pro systémy s procesorem Itanium</a><br />
(KB948108)<br />
(Důležitý)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Microsoft Data Engine (MSDE) 1.0 Service Pack 4</td>
<td style="border:1px solid black;">Aktualizace GDR:<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=c95b2cb3-51a4-44e4-b9f4-9416e9ce16a0">Microsoft Data Engine (MSDE) 1.0 Service Pack 4</a><br />
(KB948113)<br />
(Důležitý)<br />
<br />
Aktualizace QFE:<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=c95b2cb3-51a4-44e4-b9f4-9416e9ce16a0">Microsoft Data Engine (MSDE) 1.0 Service Pack 4</a><br />
(KB948113)<br />
(Důležitý)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) Service Pack 4</td>
<td style="border:1px solid black;">Aktualizace GDR:<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=4fd1f86a-94a2-43d8-9b0a-774c81426d9e">Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) Service Pack 4</a><br />
(KB948110)<br />
(Důležitý)<br />
<br />
Aktualizace QFE:<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=8316bc5e-8c2d-4710-8acc-b815ccc81cd4">Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) Service Pack 4</a><br />
(KB948111)<br />
(Důležitý)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Microsoft SQL Server 2005 Express Edition Service Pack 2</td>
<td style="border:1px solid black;">Aktualizace GDR:<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=4c9851cc-2c4c-4190-872c-84993a7623b7">Microsoft SQL Server 2005 Express Edition Service Pack 2</a><br />
(KB948109)<br />
(Důležitý)<br />
<br />
Aktualizace QFE:<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=a60bb7e7-ef4e-4cbd-b63a-0ad7bd1402b3">Microsoft SQL Server 2005 Express Edition Service Pack 2</a><br />
(KB948108)<br />
(Důležitý)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Microsoft SQL Server 2005 Express Edition se službou Advanced Services Service Pack 2</td>
<td style="border:1px solid black;">Aktualizace GDR:<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=4c9851cc-2c4c-4190-872c-84993a7623b7">Microsoft SQL Server 2005 Express Edition se službou Advanced Services Service Pack 2</a><br />
(KB948109)<br />
(Důležitý)<br />
<br />
Aktualizace QFE:<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=a60bb7e7-ef4e-4cbd-b63a-0ad7bd1402b3">Microsoft SQL Server 2005 Express Edition se službou Advanced Services Service Pack 2</a><br />
(KB948108)<br />
(Důležitý)</td>
</tr>
</tbody>
</table>
<p></p>
 

 
<p></p>
<table style="border:1px solid black;">
<caption>Microsoft Exchange Server</caption>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Identifikátor bulletinu</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=120820"><strong>MS08-039</strong></a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Stupeň maximální závažnosti bulletinu</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Vysoký</strong></a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Microsoft Exchange Server 2003 Service Pack 2</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=e099c1d1-5af6-4d6c-b735-9599412b3131">Microsoft Exchange Server 2003 Service Pack 2</a><br />
(Důležitý)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Microsoft Exchange Server 2007</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=086a2a13-a1de-4b1d-bd12-b148bfd2dafa">Microsoft Exchange Server 2007</a><br />
(Důležitý)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Microsoft Exchange Server 2007 Service Pack 1</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=63e7f26c-92a8-4264-882d-f96b348c96ab">Microsoft Exchange Server 2007 Service Pack 1</a><br />
(Důležitý)</td>
</tr>
</tbody>
</table>
<p></p>
 

Nástroje a doporučené postupy zjišťování a nasazení
---------------------------------------------------

 
**Centrum zabezpečení**

Umožňuje správu aktualizací softwaru a zabezpečení, které je třeba nainstalovat na servery, stolní počítače a přenosné počítače v organizaci. Další informace naleznete na webu [TechNet Update Management Center](http://go.microsoft.com/fwlink/?linkid=69903). Další informace o zabezpečení produktů společnosti Microsoft nabízí web [Centrum zabezpečení TechNet](http://go.microsoft.com/fwlink/?linkid=21171). Tyto informace lze také získat kliknutím na nabídku „Nejnovější aktualizace zabezpečení“ na webu [Zabezpečení doma](http://go.microsoft.com/fwlink/?linkid=85102).

Aktualizace zabezpečení jsou k dispozici na webu [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747), [Windows Update](http://go.microsoft.com/fwlink/?linkid=21130) a [Office Update](http://go.microsoft.com/fwlink/?linkid=21135). Aktualizace zabezpečení jsou také k dispozici na webu [služby Stažení softwaru](http://go.microsoft.com/fwlink/?linkid=21129). Nejsnadněji je naleznete hledáním podle klíčových slov aktualizace zabezpečení.

Aktualizace zabezpečení lze stáhnout z katalogu služby [Microsoft Update Catalog](http://go.microsoft.com/fwlink/?linkid=96155). Služba Microsoft Update Catalog poskytuje katalog s možností vyhledávání obsahu dostupného prostřednictvím služeb Windows Update a Microsoft Update, včetně aktualizací zabezpečení, ovladačů a aktualizací Service Pack. Vyhledáváním pomocí čísla bulletinu zabezpečení (například MS07-036) můžete přidat všechny dostupné aktualizace do košíku (včetně různých jazykových verzí aktualizace) a stáhnout je do vybrané složky. Další informace o službě Microsoft Update Catalog najdete v části [Nejčastější dotazy týkající se služby Microsoft Update Catalog](http://go.microsoft.com/fwlink/?linkid=97900).

**Doporučené postupy zjišťování a instalace**

Společnost Microsoft poskytla doporučené postupy zjišťování a instalace aktualizací zabezpečení vydaných tento měsíc. Tyto doporučené postupy by měly pomoci také odborníkům v oblasti IT při používání různých nástrojů při instalaci aktualizace zabezpečení, např. Windows Update, Microsoft Update, Office Update, nástroj MBSA (Microsoft Baseline Security Analyzer), nástroj pro rozpoznávání sady Office, Microsoft Systems Management Server (SMS) a nástroj Extended Security Update Inventory Tool (ESUIT). Další informace získáte v [článku 910723 znalostní báze Microsoft Knowledge Base](http://support.microsoft.com/kb/910723).

**Nástroj Microsoft Baseline Security Analyzer**

Pomocí nástroje Microsoft Baseline Security Analyzer (MBSA) mohou správci prohledávat místní i vzdálené systémy a zjistit tak, jestli v nich nechybí některé aktualizace zabezpečení nebo jestli v nastavení zabezpečení systému nedošlo k některým běžným chybám. Další informace o nástroji MBSA získáte na webu [Microsoft Baseline Security Analyzer](http://go.microsoft.com/fwlink/?linkid=21134).

**Služba Windows Server Update Services**

Pomocí služby Windows Server Update Services (WSUS) mohou správci systémů rychle a spolehlivě instalovat nejnovější důležité aktualizace zabezpečení pro systémy Windows 2000 a novější, sadu Office XP a novější, Exchange Server 2003 a SQL Server 2000 do systémů Windows 2000 a novějších.

Další informace o způsobu instalace této aktualizace zabezpečení pomocí služby Windows Server Update Services získáte na webu služby [Windows Server Update Services](http://go.microsoft.com/fwlink/?linkid=50120).

**Systems Management Server**

Microsoft Systems Management Server (SMS) představuje v rozlehlých sítích řešení pro správu aktualizací s rozsáhlými možnostmi konfigurace. Umožňuje správcům identifikovat počítače se systémem Windows, které vyžadují aktualizace zabezpečení, a provést řízenou instalaci těchto aktualizací v celé rozlehlé síti s minimálním dopadem na koncové uživatele. K dispozici je nyní nová verze nástroje SMS, System Center Configuration Manager 2007 (viz také webové stránky produktu [System Center Configuration Manager 2007](http://technet.microsoft.com/en-us/library/bb735860.aspx)). Další informace o tom, jak mohou správci pomocí serveru SMS 2003 nasazovat aktualizace zabezpečení, získáte na webu [SMS 2003 Security Patch Management](http://go.microsoft.com/fwlink/?linkid=22939). Uživatelé serveru SMS 2.0 mohou při nasazení aktualizací zabezpečení použít také sadu [Software Updates Services Feature Pack](http://go.microsoft.com/fwlink/?linkid=33340). Další informace o serveru SMS získáte na webu [Microsoft Systems Management Server](http://go.microsoft.com/fwlink/?linkid=21158).

**Poznámka:** Server SMS využívá nástroj MBSA (Microsoft Baseline Security Analyzer) a nástroj pro rozpoznávání sady Microsoft Office, a poskytuje tak širokou podporu pro zjišťování a instalaci aktualizací uvedených v bulletinech zabezpečení. Tyto nástroje nemusí některé softwarové aktualizace zjistit. V takovém případě mohou správci použít funkce serveru SMS a nasměrovat aktualizace do určitých systémů. Další informace o tomto postupu najdete na webu [Nasazení aktualizací softwaru pomocí funkce Distribuce softwaru serveru SMS](http://go.microsoft.com/fwlink/?linkid=33341). Některé aktualizace zabezpečení vyžadují po restartování počítače oprávnění správce. Správci mohou k instalaci těchto aktualizací použít nástroj Elevated Rights Deployment Tool (k dispozici v sadě [SMS 2003 Administration Feature Pack](http://go.microsoft.com/fwlink/?linkid=33387) a [SMS 2.0 Administration Feature Pack](http://go.microsoft.com/fwlink/?linkid=21161)).

**Nástroj Update Compatibility Evaluator a sada Application Compatibility Toolkit**

Aktualizace často zapisují do stejných souborů a nastavení registru požadovaných pro spouštění aplikací. To může způsobit nekompatibilitu a zvýšit dobu, po kterou trvá nasazení aktualizací zabezpečení. Testování a ověřování aktualizací systému Windows lze usnadnit pomocí součástí nástroje [Update Compatibility Evaluator](http://technet2.microsoft.com/windowsvista/en/library/4279e239-37a4-44aa-aec5-4e70fe39f9de1033.mspx?mfr=true), které jsou dodávány se sadou [Application Compatibility Toolkit 5.0](http://www.microsoft.com/downloads/details.aspx?familyid=24da89e9-b581-47b0-b45e-492dd6da2971&displaylang=en).

Sada Application Compatibility Toolkit (ACT) obsahuje nezbytné nástroje a dokumentaci pro posouzení a zmírnění problémů s kompatibilitou aplikací před nasazením systému Microsoft Windows Vista, služby Windows Update, aktualizací zabezpečení společnosti Microsoft nebo nové verze aplikace Windows Internet Explorer ve vašem prostředí.

### Další informace

#### Nástroj pro odstranění škodlivého softwaru systému Microsoft Windows

Společnost Microsoft vydává aktualizovanou verzi Nástroje pro odstranění škodlivého softwaru systému Microsoft Windows na webu Windows Update, Microsoft Update, ve službě Windows Server Update Services a na webu služby Stažení softwaru.

#### Důležité aktualizace nesouvisející se zabezpečením na webu Microsoft Update (MU), Windows Update (WU) a ve službě Windows Server Update Services (WSUS)

Informace o aktualizacích nesouvisejících se zabezpečením na webu Windows Update a Microsoft Update naleznete na webové stránce:

-   [Článek 894199 znalostní báze Microsoft Knowledge Base](http://support.microsoft.com/kb/894199): Popis služeb Software Update Services a Windows Server Update Services se mění v obsahu pro rok 2008. Zahrnuje celý obsah systému Windows.
-   [Nové, revidované a vydané aktualizace pro jiné produkty společnosti Microsoft, než je systém Microsoft Windows](http://technet.microsoft.com/en-us/wsus/bb466214.aspx).

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

-   Danovi Kaminskymu ze společnosti [IOActive](http://www.ioactive.com/) za oznámení chyby popsané v bulletinu MS08-037.
-   Michaelu Jordanovi ze společnosti [Context Information Security](http://www.contextis.co.uk/) za oznámení dvou chyb popsaných v bulletinu MS08-039.
-   Anonymnímu nálezci za oznámení chyby popsané v bulletinu MS08-040.
-   Anonymnímu nálezci za oznámení chyby popsané v bulletinu MS08-040.
-   Brettu Mooreovi ze společnosti [Insomnia Security](http://www.insomniasec.com/) spolupracujícímu se společností [iDefense VCP](http://labs.idefense.com/) za oznámení chyby popsané v bulletinu MS08-040.
-   Anonymnímu nálezci za oznámení chyby popsané v bulletinu MS08-040.

#### Technická podpora

-   Uvedený software byl testován za účelem zjištění, kterých verzí se chyba týká. U dalších verzí skončila časově omezená podpora. Pokud chcete zjistit dobu, po kterou je pro určitou verzi softwaru poskytována podpora, navštivte web [Zásady poskytování technické podpory pro produkty společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=21742).
-   Zákazníci mohou získat technickou podporu na webu [služby technické podpory společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=21131). Hovory související s aktualizacemi zabezpečení jsou bezplatné.
-   Mezinárodní zákazníci získají podporu u místních zastoupení společnosti Microsoft. Technická podpora související s aktualizacemi zabezpečení je bezplatná. Další informace o možnostech kontaktování společnosti Microsoft v případě potřeby technické podpory získáte na [webu mezinárodní technické podpory](http://go.microsoft.com/fwlink/?linkid=21155).

#### Zřeknutí se záruky

Informace ve znalostní bázi Microsoft Knowledge Base jsou poskytovány tak, jak jsou, bez jakékoli záruky. Společnost Microsoft neposkytuje žádné záruky, výslovně uvedené či mlčky předpokládané, včetně záruk obchodovatelnosti a vhodnosti pro určitý účel. Společnost Microsoft ani její dodavatelé nenesou v žádném případě zodpovědnost za žádné škody, včetně přímých, nepřímých, náhodných či následných škod, ztráty zisku či zvláštních škod, a to ani v případě, že byli na možnost takových škod upozorněni. V některých zemích a právních řádech není dovoleno vyloučit nebo omezit odpovědnost, proto se výše uvedené omezení na vás nemusí vztahovat.

#### Revize

-   V1.0 (8. července 2008): Souhrnný bulletin byl publikován.
-   V1.1 (11. února 2009): Z tabulky Software obsahující tuto chybu a umístění aktualizací ke stažení, jež je součástí bulletinu MS08-040, byl odebrán chybný odkaz na modul Microsoft SQL Server 2000 Desktop Engine (WMSDE) v systému Microsoft Windows 2000 Service Pack 4.

*Built at 2014-04-18T01:50:00Z-07:00*
