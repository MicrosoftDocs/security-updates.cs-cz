---
TOCTitle: 'MS08-AUG'
Title: 'Souhrnný bulletin zabezpečení společnosti Microsoft, srpen 2008'
ms:assetid: 'ms08-aug'
ms:contentKeyID: 61223971
ms:mtpsurl: 'https://technet.microsoft.com/cs-CZ/library/ms08-aug(v=Security.10)'
---

Souhrnný bulletin zabezpečení společnosti Microsoft, srpen 2008
===============================================================

Publikováno: 12. srpna 2008 | Aktualizováno: 15. října 2008

**Verze:** 3.0

Tento souhrnný bulletin uvádí bulletiny zabezpečení vydané v srpnu 2008.

Spolu s vydáním bulletinů pro srpen 2008 nahrazuje tento souhrnný bulletin předběžné oznámení o bulletinech vydané 7. srpna 2008. Další informace o službě předběžného oznámení o bulletinech naleznete v části [Předběžné oznámení o bulletinech zabezpečení společnosti Microsoft](http://technet.microsoft.com/security/bulletin/advance).

Informace o tom, jak dostávat automatická oznámení o vydání nových bulletinů zabezpečení společnosti Microsoft, naleznete na webu [Zasílání technických oznámení o zabezpečení společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=21163).

Pro zodpovězení zákaznických dotazů týkajících se těchto bulletinů uspořádá společnost Microsoft webové vysílání 13. srpna 2008 v 11:00 časového pásma Tichomoří (USA a Kanada). [Registrovat se pro webové vysílání týkající se srpnových bulletinů zabezpečení](http://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032374631&culture=en-us). Po tomto datu je webové vysílání dostupné na požádání. Další informace získáte v [souhrnných bulletinech zabezpečení společnosti Microsoft a webovém vysílání](http://technet.microsoft.com/security/bulletin/summary).

Společnost Microsoft se snaží zákazníkům usnadnit upřednostnění měsíčně vydávaných aktualizací zabezpečení před jakýmikoli důležitými aktualizacemi nesouvisejícími se zabezpečením, které jsou vydány ve stejný den jako měsíčně vydávané aktualizace zabezpečení. Další informace získáte v části **Další informace**.

### Informace o bulletinech

#### Shrnutí

Bulletiny zabezpečení podle závažnosti:

Kritický (6)
------------



| Identifikátor bulletinu            | Bulletin zabezpečení společnosti Microsoft MS08-046                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
|------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Název bulletinu**                | [**Chyba zabezpečení systému ICM (Image Color Management) v systému Microsoft Windows umožňuje vzdálené spuštění kódu (952954)**](http://go.microsoft.com/fwlink/?linkid=120576)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| **Shrnutí**                        | Tato aktualizace řeší chybu zabezpečení systému ICM (Microsoft Image Color Management), která by mohla umožnit vzdálené spuštění kódu v kontextu aktuálního uživatele. Uvedená chyba byla oznámena soukromou osobou. Pokud by byl uživatel přihlášen s uživatelskými právy správce, mohl by útočník, který by tuto chybu zabezpečení zneužil, získat úplnou kontrolu nad postiženým systémem. Útočník by tak mohl instalovat programy, zobrazovat, měnit či odstraňovat data nebo vytvářet nové účty s úplnými uživatelskými právy. Uživatelé, jejichž účty jsou konfigurovány tak, aby měli v systému méně uživatelských práv, by byli vystaveni menšímu riziku než uživatelé s uživatelskými právy správce. |
| **Stupeň maximální závažnosti**    | [Kritický](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| **Dopad této chyby zabezpečení**   | Vzdálené spuštění kódu                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| **Rozpoznávání**                   | Pomocí nástroje MBSA (Microsoft Baseline Security Analyzer) lze určit, zda počítačový systém potřebuje tuto aktualizaci. Tato aktualizace vyžaduje restartování.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| **Software obsahující tuto chybu** | **Microsoft Windows.** Další informace získáte v části Software obsahující tuto chybu a umístění aktualizací ke stažení.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |

| Identifikátor bulletinu            | Bulletin zabezpečení společnosti Microsoft MS08-045                                                                                                                                                                                                                                                                                                                                                                                                                         |
|------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Název bulletinu**                | [**Kumulativní aktualizace zabezpečení pro aplikaci Internet Explorer (953838)**](http://go.microsoft.com/fwlink/?linkid=122772)                                                                                                                                                                                                                                                                                                                                            |
| **Shrnutí**                        | Tato kritická aktualizace zabezpečení řeší pět chyb zabezpečení oznámených soukromými osobami a jednu veřejně známou chybu. Všechny tyto chyby zabezpečení mohou umožňovat vzdálené spuštění kódu, pokud uživatel zobrazí pomocí aplikace Internet Explorer speciálně vytvořenou webovou stránku. Uživatelé, jejichž účty jsou konfigurovány tak, aby měli v systému méně uživatelských práv, by byli vystaveni menšímu riziku než uživatelé s uživatelskými právy správce. |
| **Stupeň maximální závažnosti**    | [Kritický](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                    |
| **Dopad této chyby zabezpečení**   | Vzdálené spuštění kódu                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| **Rozpoznávání**                   | Pomocí nástroje MBSA (Microsoft Baseline Security Analyzer) lze určit, zda počítačový systém potřebuje tuto aktualizaci. Tato aktualizace vyžaduje restartování.                                                                                                                                                                                                                                                                                                            |
| **Software obsahující tuto chybu** | **Microsoft Windows, Internet Explorer.** Další informace získáte v části Software obsahující tuto chybu a umístění aktualizací ke stažení.                                                                                                                                                                                                                                                                                                                                 |

| Identifikátor bulletinu            | Bulletin zabezpečení společnosti Microsoft MS08-041                                                                                                                                                                                                                                                                                                                                                                                                                                            |
|------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Název bulletinu**                | [**Chyba zabezpečení ovládacího prvku ActiveX pro program Snapshot Viewer v aplikaci Microsoft Access umožňuje vzdálené spuštění kódu (955617)**](http://go.microsoft.com/fwlink/?linkid=122912)                                                                                                                                                                                                                                                                                               |
| **Shrnutí**                        | Tato aktualizace zabezpečení řeší chybu zabezpečení oznámenou soukromou osobou v ovládacím prvku ActiveX pro program Snapshot Viewer pro aplikaci Microsoft Access. Útočník by mohl tuto chybu zabezpečení zneužít vytvořením speciální webové stránky. Když uživatel zobrazí tuto webovou stránku, chyba zabezpečení by mohla umožnit vzdálené spuštění kódu. Útočník, který by úspěšně zneužil tuto chybu zabezpečení, by mohl získat stejná uživatelská práva, jaká má přihlášený uživatel. |
| **Stupeň maximální závažnosti**    | [Kritický](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| **Dopad této chyby zabezpečení**   | Vzdálené spuštění kódu                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| **Rozpoznávání**                   | Pomocí nástroje MBSA (Microsoft Baseline Security Analyzer) lze určit, zda počítačový systém potřebuje tuto aktualizaci. Aktualizace nevyžaduje restartování.                                                                                                                                                                                                                                                                                                                                  |
| **Software obsahující tuto chybu** | **Microsoft Office.** Další informace získáte v části Software obsahující tuto chybu a umístění aktualizací ke stažení.                                                                                                                                                                                                                                                                                                                                                                        |

| Identifikátor bulletinu            | Bulletin zabezpečení společnosti Microsoft MS08-043                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
|------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Název bulletinu**                | [**Chyby zabezpečení v aplikaci Microsoft Excel umožňují vzdálené spuštění kódu (954066)**](http://go.microsoft.com/fwlink/?linkid=124306)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| **Shrnutí**                        | Tato aktualizace zabezpečení řeší čtyři chyby zabezpečení aplikace Microsoft Office Excel oznámené soukromými osobami, které by mohly umožnit vzdálené spuštění kódu v případě, že uživatel otevře speciálně vytvořený soubor aplikace Excel. Útočník, který by tyto chyby zabezpečení zneužil, by mohl získat úplnou kontrolu nad postiženým systémem. Útočník by tak mohl instalovat programy, zobrazovat, měnit či odstraňovat data nebo vytvářet nové účty s úplnými uživatelskými právy. Uživatelé, jejichž účty jsou konfigurovány tak, aby měli v systému méně uživatelských práv, by byli vystaveni menšímu riziku než uživatelé s uživatelskými právy správce. |
| **Stupeň maximální závažnosti**    | [Kritický](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| **Dopad této chyby zabezpečení**   | Vzdálené spuštění kódu                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| **Rozpoznávání**                   | Pomocí nástroje MBSA (Microsoft Baseline Security Analyzer) lze určit, zda počítačový systém potřebuje tuto aktualizaci. Aktualizace nevyžaduje restartování.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| **Software obsahující tuto chybu** | **Microsoft Office.** Další informace získáte v části Software obsahující tuto chybu a umístění aktualizací ke stažení.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |

| Identifikátor bulletinu            | Bulletin zabezpečení společnosti Microsoft MS08-051                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
|------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Název bulletinu**                | [**Chyby zabezpečení v aplikaci Microsoft PowerPoint umožňují vzdálené spuštění kódu (949785)**](http://go.microsoft.com/fwlink/?linkid=120394)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| **Shrnutí**                        | Tato aktualizace zabezpečení řeší tři chyby zabezpečení v aplikaci Microsoft Office PowerPoint a Microsoft Office PowerPoint Viewer, které by mohly umožnit vzdálené spuštění kódu v případě, že uživatel otevře speciálně vytvořený soubor aplikace PowerPoint. Uvedené chyby byly oznámeny soukromými osobami. Útočník, který by úspěšně zneužil některou z těchto chyb zabezpečení, by mohl převzít úplnou kontrolu nad postiženým systémem. Útočník by tak mohl instalovat programy, zobrazovat, měnit či odstraňovat data nebo vytvářet nové účty s úplnými uživatelskými právy. Uživatelé, jejichž účty jsou konfigurovány tak, aby měli v systému méně uživatelských práv, by byli vystaveni menšímu riziku než uživatelé s uživatelskými právy správce. |
| **Stupeň maximální závažnosti**    | [Kritický](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| **Dopad této chyby zabezpečení**   | Vzdálené spuštění kódu                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| **Rozpoznávání**                   | Pomocí nástroje MBSA (Microsoft Baseline Security Analyzer) lze určit, zda počítačový systém potřebuje tuto aktualizaci. Aktualizace nevyžaduje restartování.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| **Software obsahující tuto chybu** | **Microsoft Office.** Další informace získáte v části Software obsahující tuto chybu a umístění aktualizací ke stažení.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |

| Identifikátor bulletinu            | Bulletin zabezpečení společnosti Microsoft MS08-044                                                                                                                                                                                                                                                                                                                                                           |
|------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Název bulletinu**                | [**Chyby zabezpečení ve filtrech sady Microsoft Office umožňují vzdálené spuštění kódu (924090)**](http://go.microsoft.com/fwlink/?linkid=120819)                                                                                                                                                                                                                                                             |
| **Shrnutí**                        | Tato aktualizace zabezpečení řeší pět chyb zabezpečení oznámených soukromými osobami. Tyto chyby zabezpečení umožňují vzdálené spuštění kódu, pokud uživatel zobrazí v sadě Microsoft Office speciálně vytvořený soubor s obrázkem. Uživatelé, jejichž účty jsou konfigurovány tak, aby měli v systému méně uživatelských práv, by byli vystaveni menšímu riziku než uživatelé s uživatelskými právy správce. |
| **Stupeň maximální závažnosti**    | [Kritický](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                      |
| **Dopad této chyby zabezpečení**   | Vzdálené spuštění kódu                                                                                                                                                                                                                                                                                                                                                                                        |
| **Rozpoznávání**                   | Pomocí nástroje MBSA (Microsoft Baseline Security Analyzer) lze určit, zda počítačový systém potřebuje tuto aktualizaci. Aktualizace nevyžaduje restartování.                                                                                                                                                                                                                                                 |
| **Software obsahující tuto chybu** | **Microsoft Office.** Další informace získáte v části Software obsahující tuto chybu a umístění aktualizací ke stažení.                                                                                                                                                                                                                                                                                       |

Vysoký (5)
----------



| Identifikátor bulletinu            | Bulletin zabezpečení společnosti Microsoft MS08-047                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
|------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Název bulletinu**                | [**Chyba zabezpečení ve zpracování zásad protokolu IPsec umožňuje přístup k informacím (953733)**](http://go.microsoft.com/fwlink/?linkid=120577)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| **Shrnutí**                        | Tato aktualizace řeší chybu zabezpečení oznámenou soukromou osobou ve způsobu, jakým se používají určitá pravidla protokolu Windows Internet Protocol Security (IPsec). Tato chyba zabezpečení by mohla způsobit, že systém bude ignorovat zásady protokolu IPsec a přenášet síťovou komunikaci jako čistý text. To může zpřístupnit informace určené k šifrování v síti. Útočník sledující síťové přenosy by si mohl prohlížet a pravděpodobně i upravovat obsah těchto přenosů. Poznámka: Tato chyba zabezpečení nepovolí útočníkovi spouštět kód ani přímo zvyšovat uživatelská práva. Lze ji použít ke shromažďování užitečných informací nebo k pokusu o další ohrožení daného systému nebo sítě. |
| **Stupeň maximální závažnosti**    | [Vysoký](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| **Dopad této chyby zabezpečení**   | Přístup k informacím                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| **Rozpoznávání**                   | Pomocí nástroje MBSA (Microsoft Baseline Security Analyzer) lze určit, zda počítačový systém potřebuje tuto aktualizaci. Tato aktualizace vyžaduje restartování.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| **Software obsahující tuto chybu** | **Microsoft Windows.** Další informace získáte v části Software obsahující tuto chybu a umístění aktualizací ke stažení.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |

| Identifikátor bulletinu            | Bulletin zabezpečení společnosti Microsoft MS08-049                                                                                                                                                                                                                                                                                                                                                                                            |
|------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Název bulletinu**                | [**Chyby zabezpečení v Systému událostí umožňují vzdálené spuštění kódu (950974)**](http://go.microsoft.com/fwlink/?linkid=104923)                                                                                                                                                                                                                                                                                                             |
| **Shrnutí**                        | Tato aktualizace umožňuje odstranit dvě chyby zabezpečení Systému událostí v systému Microsoft Windows, které by mohly umožnit vzdálené spuštění kódu. Uvedené chyby byly oznámeny soukromou osobou. Útočník, který by tyto chyby zabezpečení zneužil, by mohl získat úplnou kontrolu nad postiženým systémem. Útočník by tak mohl instalovat programy, zobrazovat, měnit či odstraňovat data nebo vytvářet nové účty s úplnými právy správce. |
| **Stupeň maximální závažnosti**    | [Vysoký](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                         |
| **Dopad této chyby zabezpečení**   | Vzdálené spuštění kódu                                                                                                                                                                                                                                                                                                                                                                                                                         |
| **Rozpoznávání**                   | Pomocí nástroje MBSA (Microsoft Baseline Security Analyzer) lze určit, zda počítačový systém potřebuje tuto aktualizaci. Tato aktualizace vyžaduje restartování.                                                                                                                                                                                                                                                                               |
| **Software obsahující tuto chybu** | **Microsoft Windows.** Další informace získáte v části Software obsahující tuto chybu a umístění aktualizací ke stažení.                                                                                                                                                                                                                                                                                                                       |

| Identifikátor bulletinu            | Bulletin zabezpečení společnosti Microsoft MS08-048                                                                                                                                                                                                                                                                                                                                                                                                                 |
|------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Název bulletinu**                | [**Aktualizace zabezpečení pro aplikace Outlook Express a Windows Mail (951066)**](http://go.microsoft.com/fwlink/?linkid=117705)                                                                                                                                                                                                                                                                                                                                   |
| **Shrnutí**                        | Tato aktualizace zabezpečení řeší chybu zabezpečení oznámenou soukromou osobou, týkající se aplikací Outlook Express a Windows Mail. Chyba zabezpečení může umožnit přístup k informacím, pokud uživatel navštíví pomocí aplikace Internet Explorer speciálně vytvořenou webovou stránku. Uživatelé, jejichž účty jsou konfigurovány tak, aby měli v systému méně uživatelských práv, by byli vystaveni menšímu riziku než uživatelé s uživatelskými právy správce. |
| **Stupeň maximální závažnosti**    | [Vysoký](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                              |
| **Dopad této chyby zabezpečení**   | Přístup k informacím                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| **Rozpoznávání**                   | Pomocí nástroje MBSA (Microsoft Baseline Security Analyzer) lze určit, zda počítačový systém potřebuje tuto aktualizaci. Aktualizace může vyžadovat restartování počítače.                                                                                                                                                                                                                                                                                          |
| **Software obsahující tuto chybu** | **Microsoft Windows, Outlook Express, Windows Mail.** Další informace získáte v části Software obsahující tuto chybu a umístění aktualizací ke stažení.                                                                                                                                                                                                                                                                                                             |

| Identifikátor bulletinu            | Bulletin zabezpečení společnosti Microsoft MS08-050                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
|------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Název bulletinu**                | [**Chyba zabezpečení ve službě Windows Messenger může umožnit přístup k informacím (955702)**](http://go.microsoft.com/fwlink/?linkid=108245)                                                                                                                                                                                                                                                                                                                                                                                                                          |
| **Shrnutí**                        | Tato aktualizace zabezpečení řeší veřejně oznámenou chybu zabezpečení v podporovaných verzích služby Windows Messenger. V důsledku této chyby zabezpečení by mohlo skriptování ovládacího prvku ActiveX umožnit přístup k informacím v kontextu přihlášeného uživatele. Útočník by mohl změnit stav, získat kontaktní informace a zahájit relace audiokonverzace a videokonverzace bez vědomí přihlášeného uživatele. Zároveň by mohl zaznamenat ID přihlášení uživatele a vzdáleně se přihlásit k jeho klientovi služby Messenger v rámci zosobnění daného uživatele. |
| **Stupeň maximální závažnosti**    | [Vysoký](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| **Dopad této chyby zabezpečení**   | Přístup k informacím                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| **Rozpoznávání**                   | Nástroj Microsoft Baseline Security Analyzer rozpozná, zda váš počítačový systém vyžaduje tuto aktualizaci pouze pro službu Windows Messenger 4.7 v podporovaných edicích systému Windows XP. Tato aktualizace vyžaduje restartování.                                                                                                                                                                                                                                                                                                                                  |
| **Software obsahující tuto chybu** | **Microsoft Windows, Windows Messenger.** Další informace získáte v části Software obsahující tuto chybu a umístění aktualizací ke stažení.                                                                                                                                                                                                                                                                                                                                                                                                                            |

| Identifikátor bulletinu            | Bulletin zabezpečení společnosti Microsoft MS08-042                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
|------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Název bulletinu**                | [**Chyba zabezpečení v aplikaci Microsoft Word umožňuje vzdálené spuštění kódu (955048)**](http://go.microsoft.com/fwlink/?linkid=123160)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| **Shrnutí**                        | Tato aktualizace zabezpečení řeší veřejně oznámenou chybu zabezpečení aplikace Microsoft Word. Tato chyba umožňuje vzdálené spuštění kódu, pokud uživatel otevře speciálně vytvořený soubor aplikace Word. Útočník, který by tuto chybu zabezpečení zneužil, by mohl získat úplnou kontrolu nad postiženým systémem. Útočník by tak mohl instalovat programy, zobrazovat, měnit či odstraňovat data nebo vytvářet nové účty s úplnými uživatelskými právy. Uživatelé, jejichž účty jsou konfigurovány tak, aby měli v systému méně uživatelských práv, by byli vystaveni menšímu riziku než uživatelé s uživatelskými právy správce. |
| **Stupeň maximální závažnosti**    | [Vysoký](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| **Dopad této chyby zabezpečení**   | Vzdálené spuštění kódu                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| **Rozpoznávání**                   | Pomocí nástroje MBSA (Microsoft Baseline Security Analyzer) lze určit, zda počítačový systém potřebuje tuto aktualizaci. Aktualizace nevyžaduje restartování.                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| **Software obsahující tuto chybu** | **Microsoft Office.** Další informace získáte v části Software obsahující tuto chybu a umístění aktualizací ke stažení.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |

Software obsahující tuto chybu a umístění aktualizací ke stažení
----------------------------------------------------------------


**Jak pracovat s touto tabulkou**

V této tabulce zjistíte, které aktualizace zabezpečení bude třeba nainstalovat. Přečtěte si seznam všech programů a komponent a zjistěte, zda jsou u nich vyžadovány aktualizace zabezpečení. Pokud se program nebo komponenta v seznamu nachází, je v něm zároveň uveden odkaz na dostupnou aktualizaci softwaru a také stupeň závažnosti aktualizace softwaru.

**Poznámka:** Jedna chyba zabezpečení může vyžadovat instalaci více aktualizací. Přečtěte si celý sloupec u každého identifikátoru bulletinu. Zjistíte v něm, které aktualizace nainstalovat v závislosti na programech nebo součástech nainstalovaných ve vašem systému.

#### Operační systém Windows

 
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
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
</tr>
<tr>
<th colspan="7" style="border:1px solid black;">
Microsoft Windows 2000
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS08-046**](http://go.microsoft.com/fwlink/?linkid=120576)
</td>
<td style="border:1px solid black;">
[**MS08-045**](http://go.microsoft.com/fwlink/?linkid=122772)
</td>
<td style="border:1px solid black;">
[**MS08-047**](http://go.microsoft.com/fwlink/?linkid=120577)
</td>
<td style="border:1px solid black;">
[**MS08-049**](http://go.microsoft.com/fwlink/?linkid=104923)
</td>
<td style="border:1px solid black;">
[**MS08-048**](http://go.microsoft.com/fwlink/?linkid=117705)
</td>
<td style="border:1px solid black;">
[**MS08-050**](http://go.microsoft.com/fwlink/?linkid=108245)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Stupeň maximální závažnosti bulletinu**
</td>
<td style="border:1px solid black;">
[**Kritický**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritický**](http://go.microsoft.com/fwlink/?linkid=21140)
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
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Windows 2000 Service Pack 4
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=db455d17-435f-46d7-b2dd-5babb5a1eeb3)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 5.01 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=1557b93b-ecba-4f42-b89d-db0ee067d65b)  
(Kritický)  
[Microsoft Internet Explorer 6 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=aa780735-5928-4c46-89a4-63a814954796)  
(Kritický)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=1b2ad648-7dc9-407a-99f6-f39922746027)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Microsoft Outlook Express 5.5 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=6257bfae-35f0-4c0e-b960-bca7aa6f86f7)  
(Důležitý)  
[Microsoft Outlook Express 6 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=dab178f7-c282-41f4-acb1-a86e6aa4c91b)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Windows Messenger 5.1](http://www.microsoft.com/downloads/details.aspx?familyid=a8d9eb73-5f8c-4b9a-940f-9157a3b3d774)  
(KB899283)  
(Důležitý)
</td>
</tr>
<tr>
<th colspan="7" style="border:1px solid black;">
Windows XP
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS08-046**](http://go.microsoft.com/fwlink/?linkid=120576)
</td>
<td style="border:1px solid black;">
[**MS08-045**](http://go.microsoft.com/fwlink/?linkid=122772)
</td>
<td style="border:1px solid black;">
[**MS08-047**](http://go.microsoft.com/fwlink/?linkid=120577)
</td>
<td style="border:1px solid black;">
[**MS08-049**](http://go.microsoft.com/fwlink/?linkid=104923)
</td>
<td style="border:1px solid black;">
[**MS08-048**](http://go.microsoft.com/fwlink/?linkid=117705)
</td>
<td style="border:1px solid black;">
[**MS08-050**](http://go.microsoft.com/fwlink/?linkid=108245)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Stupeň maximální závažnosti bulletinu**
</td>
<td style="border:1px solid black;">
[**Kritický**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritický**](http://go.microsoft.com/fwlink/?linkid=21140)
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
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Service Pack 2 a Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 a Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=d313f42c-f43f-48ea-82ef-3bc33077c7fa)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=69af2f30-138e-4b15-ab8d-4fce44cc0bc2)  
(Kritický)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=8e2125c7-52cb-4052-82a3-2d3c6a953752)  
(Kritický)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 a Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=01a34aa4-a456-4efc-a93a-c3c682b0181c)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Microsoft Outlook Express 6](http://www.microsoft.com/downloads/details.aspx?familyid=91469f2f-461c-4a67-8738-d42520427f6b)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Windows Messenger 4.7](http://www.microsoft.com/downloads/details.aspx?familyid=8f588f7e-c4ed-42a0-b157-54b1eda60474)  
(KB946648)  
(Důležitý)  
[Windows Messenger 5.1](http://www.microsoft.com/downloads/details.aspx?familyid=a8d9eb73-5f8c-4b9a-940f-9157a3b3d774)  
(KB899283)  
(Důležitý)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Professional x64 Edition a Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition a Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3150c6b8-f50b-4b84-a7ce-c8daf77c080c)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=4780b89e-9735-4d3f-8def-34e7337ff604)  
(Kritický)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=39b41e4b-3237-409d-a818-ab0517c5e7cf)  
(Kritický)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition a Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=246b2686-e330-47a2-b4d4-68f218ad4021)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Microsoft Outlook Express 6](http://www.microsoft.com/downloads/details.aspx?familyid=2220aece-79d2-426f-90ec-24a17470567a)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Windows Messenger 4.7](http://www.microsoft.com/downloads/details.aspx?familyid=a5fc5457-832f-4ee8-be60-4cc8518d1c10)  
(KB946648)  
(Důležitý)  
[Windows Messenger 5.1](http://www.microsoft.com/downloads/details.aspx?familyid=a8d9eb73-5f8c-4b9a-940f-9157a3b3d774)  
(KB899283)  
(Důležitý)
</td>
</tr>
<tr>
<th colspan="7" style="border:1px solid black;">
Windows Server 2003
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS08-046**](http://go.microsoft.com/fwlink/?linkid=120576)
</td>
<td style="border:1px solid black;">
[**MS08-045**](http://go.microsoft.com/fwlink/?linkid=122772)
</td>
<td style="border:1px solid black;">
[**MS08-047**](http://go.microsoft.com/fwlink/?linkid=120577)
</td>
<td style="border:1px solid black;">
[**MS08-049**](http://go.microsoft.com/fwlink/?linkid=104923)
</td>
<td style="border:1px solid black;">
[**MS08-048**](http://go.microsoft.com/fwlink/?linkid=117705)
</td>
<td style="border:1px solid black;">
[**MS08-050**](http://go.microsoft.com/fwlink/?linkid=108245)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Stupeň maximální závažnosti bulletinu**
</td>
<td style="border:1px solid black;">
[**Kritický**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritický**](http://go.microsoft.com/fwlink/?linkid=21140)
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
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 1 a Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 1 a Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=828d8fdc-8534-4621-85a5-08aec255496f)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=0617a5dd-dce9-4de0-b0a0-ce38efe13524)  
(Kritický)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=b3c2e2fd-1cb9-491b-937c-053dd59a65bf)  
(Kritický)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 1 a Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=92a3d08f-c117-4b24-bc78-2b913d270df6)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Microsoft Outlook Express 6](http://www.microsoft.com/downloads/details.aspx?familyid=30f2244a-f6fd-4fc1-a871-abf6958cb660)  
(Nízký)
</td>
<td style="border:1px solid black;">
[Windows Messenger 4.7](http://www.microsoft.com/downloads/details.aspx?familyid=302315a8-ccb2-47c2-9104-b8e1d1f49aa0)  
(KB954723)  
(Mírný)  
[Windows Messenger 5.1](http://www.microsoft.com/downloads/details.aspx?familyid=a8d9eb73-5f8c-4b9a-940f-9157a3b3d774)  
(KB899283)  
(Mírný)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition a Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition a Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=0a13776f-d543-41df-b904-d51e368c81cc)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=32a63f52-9fe6-48e3-bb4e-7d4dda5e0a90)  
(Kritický)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=88a26b76-f7df-45c9-8ed0-7d3cd71c1987)  
(Kritický)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition a Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=6bfbb6d8-5106-4adf-83cb-35ffc6e8eaf8)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Microsoft Outlook Express 6](http://www.microsoft.com/downloads/details.aspx?familyid=3287f006-cbb2-4c6d-820c-32833e08035a)  
(Nízký)
</td>
<td style="border:1px solid black;">
[Windows Messenger 4.7](http://www.microsoft.com/downloads/details.aspx?familyid=be94d138-7d7b-489e-baa6-e214950be6b9)  
(KB954723)  
(Mírný)  
[Windows Messenger 5.1](http://www.microsoft.com/downloads/details.aspx?familyid=a8d9eb73-5f8c-4b9a-940f-9157a3b3d774)  
(KB899283)  
(Mírný)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 SP1 pro systémy s procesorem Itanium a Windows Server 2003 SP2 pro systémy s procesorem Itanium
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP1 pro systémy s procesorem Itanium a Windows Server 2003 SP2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=9566493f-4260-4072-947a-527887d2cd63)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=1855997e-a3be-46b1-a0bc-bb55eb0045fe)  
(Kritický)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=97d0d37d-5d76-4bc3-8cbd-1e3976c82acf)  
(Kritický)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Server 2003 SP1 pro systémy s procesorem Itanium a Windows Server 2003 SP2 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=45356565-697f-41b3-9879-3edd11dbcb7e)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Microsoft Outlook Express 6](http://www.microsoft.com/downloads/details.aspx?familyid=c8570e40-355b-4a9b-933d-53ae021cbda5)  
(Nízký)
</td>
<td style="border:1px solid black;">
[Windows Messenger 4.7](http://www.microsoft.com/downloads/details.aspx?familyid=e4b72618-536b-4a21-bd91-d91be9ca24e5)  
(KB954723)  
(Mírný)  
[Windows Messenger 5.1](http://www.microsoft.com/downloads/details.aspx?familyid=a8d9eb73-5f8c-4b9a-940f-9157a3b3d774)  
(KB899283)  
(Mírný)
</td>
</tr>
<tr>
<th colspan="7" style="border:1px solid black;">
Windows Vista
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS08-046**](http://go.microsoft.com/fwlink/?linkid=120576)
</td>
<td style="border:1px solid black;">
[**MS08-045**](http://go.microsoft.com/fwlink/?linkid=122772)
</td>
<td style="border:1px solid black;">
[**MS08-047**](http://go.microsoft.com/fwlink/?linkid=120577)
</td>
<td style="border:1px solid black;">
[**MS08-049**](http://go.microsoft.com/fwlink/?linkid=104923)
</td>
<td style="border:1px solid black;">
[**MS08-048**](http://go.microsoft.com/fwlink/?linkid=117705)
</td>
<td style="border:1px solid black;">
[**MS08-050**](http://go.microsoft.com/fwlink/?linkid=108245)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Stupeň maximální závažnosti bulletinu**
</td>
<td style="border:1px solid black;">
[**Kritický**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritický**](http://go.microsoft.com/fwlink/?linkid=21140)
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
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=13cba012-dd20-48f9-8e44-e4cb104c4cad)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Vista a Windows Vista Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=3f21a8a2-9861-4fef-9d1e-caf5f7822c1a)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Windows Vista a Windows Vista Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=6418c78f-f008-4028-beb1-5a5ea8e797a1)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Windows Mail](http://www.microsoft.com/downloads/details.aspx?familyid=3851bcf8-f971-4d38-b27f-97396854aac0)  
(Důležitý)
</td>
<td style="border:1px solid black;">
Netýká se
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
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=ead919c2-d548-47b7-9cd6-80f991266428)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition a Windows Vista x64 Edition Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=aa04a754-fbfb-42a7-89d2-14373e3f4742)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition a Windows Vista x64 Edition Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=e03ccfb0-3ea3-4c59-adcf-9882d7086013)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Windows Mail](http://www.microsoft.com/downloads/details.aspx?familyid=3bf7eb8a-b347-4661-be2d-682adc713769)  
(Důležitý)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
</tr>
<tr>
<th colspan="7" style="border:1px solid black;">
Windows Server 2008
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS08-046**](http://go.microsoft.com/fwlink/?linkid=120576)
</td>
<td style="border:1px solid black;">
[**MS08-045**](http://go.microsoft.com/fwlink/?linkid=122772)
</td>
<td style="border:1px solid black;">
[**MS08-047**](http://go.microsoft.com/fwlink/?linkid=120577)
</td>
<td style="border:1px solid black;">
[**MS08-049**](http://go.microsoft.com/fwlink/?linkid=104923)
</td>
<td style="border:1px solid black;">
[**MS08-048**](http://go.microsoft.com/fwlink/?linkid=117705)
</td>
<td style="border:1px solid black;">
[**MS08-050**](http://go.microsoft.com/fwlink/?linkid=108245)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Stupeň maximální závažnosti bulletinu**
</td>
<td style="border:1px solid black;">
[**Kritický**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritický**](http://go.microsoft.com/fwlink/?linkid=21140)
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
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 pro 32bitové systémy
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=4b52ff2f-d2f5-4c20-b6cf-86d86c56b0f8)\*\*  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro 32bitové systémy](http://www.microsoft.com/downloads/details.aspx?familyid=c3363df6-39dc-4910-9ce5-66553155378e)\*  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro 32bitové systémy](http://www.microsoft.com/downloads/details.aspx?familyid=0640f95e-1eee-4dd1-b4dd-2b82b7e984b9)\*  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Windows Mail](http://www.microsoft.com/downloads/details.aspx?familyid=dc3c4b63-acd3-4469-8d47-e0562d99ee65)\*\*  
(Nízký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 pro systémy s procesorem x64
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=df9814a6-5be0-4ac1-a767-a0eae8d5ee5d)\*\*  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem x64](http://www.microsoft.com/downloads/details.aspx?familyid=39dd1722-412b-469d-a475-b6513764838c)\*  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem x64](http://www.microsoft.com/downloads/details.aspx?familyid=51a93538-5e94-4f81-a6e0-d497a7b4899d)\*  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Windows Mail](http://www.microsoft.com/downloads/details.aspx?familyid=5f973f54-2322-4b41-8c1a-3e712c0da8ae)\*\*  
(Nízký)
</td>
<td style="border:1px solid black;">
Netýká se
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
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=ffc3cfcb-73fe-4a6d-9595-e9d7a5b3d3f7)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=e9c6cd46-30ad-46ee-9c8b-d0b446e660c4)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 pro systémy s procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=390da130-749d-4890-aad7-be91e15b32bb)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Windows Mail](http://www.microsoft.com/downloads/details.aspx?familyid=9226cd85-1445-4976-a126-757c5d142ffd)  
(Nízký)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
</tr>
</table>
 
**\*Instalace Server Core operačního systému Windows Server 2008 obsahující tuto chybu.** Tato aktualizace se týká všech podporovaných vydání systému Windows Server 2008 se stejným stupněm závažnosti, ať už byl systém Windows Server 2008 instalován pomocí možnosti instalace Server Core či nikoli. Více informací o této možnosti instalace naleznete v části [Server Core](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx). Možnost instalace Server Core se nevztahuje na určité edice systému Windows Server 2008. Další informace naleznete v části [Porovnání možností instalace Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**\*\*Instalace Server Core operačního systému Windows Server 2008 neobsahující tuto chybu.** Chyba zabezpečení, kterou řeší tato aktualizace, nepostihuje podporovaná vydání systému Windows Server 2008, jestliže byl systém Windows Server 2008 instalován s využitím možnosti instalace Server Core. Více informací o této možnosti instalace naleznete v části [Server Core](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx). Možnost instalace Server Core se nevztahuje na určité edice systému Windows Server 2008. Další informace naleznete v části [Porovnání možností instalace Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

#### Sady Microsoft Office a jejich software

 
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
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
</tr>
<tr>
<th colspan="6" style="border:1px solid black;">
Sady Microsoft Office, systémy a komponenty
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS08-041**](http://go.microsoft.com/fwlink/?linkid=122912)
</td>
<td style="border:1px solid black;">
[**MS08-043**](http://go.microsoft.com/fwlink/?linkid=124306)
</td>
<td style="border:1px solid black;">
[**MS08-051**](http://go.microsoft.com/fwlink/?linkid=120394)
</td>
<td style="border:1px solid black;">
[**MS08-044**](http://go.microsoft.com/fwlink/?linkid=120819)
</td>
<td style="border:1px solid black;">
[**MS08-042**](http://go.microsoft.com/fwlink/?linkid=123160)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Stupeň maximální závažnosti bulletinu**
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
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Works 8
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Microsoft Works 8](http://www.microsoft.com/downloads/details.aspx?familyid=458985c3-9c6f-4049-81cd-0d0389c81f11)  
(KB955428)  
(Důležitý)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2000 Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Office Access 2000 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=54e4031d-298f-480c-88d5-0ad3b2b62ba9)  
(KB955441)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Excel 2000 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=4bf8688e-e5b9-4e53-a1a1-8cf1acfdb80b)  
(KB951582)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Microsoft Office PowerPoint 2000 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=e7c044d8-778a-4985-b25b-4f7f6e4abadd)  
(KB949007)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2000 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=3ab323ec-9f92-453c-b7c7-9a95a9efcaea)  
(KB921595)  
(Kritický)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Office Access 2002 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=34b655f8-1922-4246-94ca-ed381c3e3b13)  
(KB955440)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Excel 2002 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=9bbf7550-f5c4-4b9b-bd86-1e7be6c42eb5)  
(KB951551)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Microsoft Office PowerPoint 2002 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=f8921074-7985-4d42-ac2b-d2f3b1d466ba)  
(KB948995)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Microsoft Office XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=bf566ce6-23da-45e5-9c2b-c47331d30e79)  
(KB921596)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Microsoft Word 2002 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=c7146dfc-e1be-4d13-877b-1d9bcacc4a64)  
(KB954463)  
(Důležitý)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2003 Service Pack 2 a Microsoft Office 2003 Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Office Access 2003 Service Pack 2 a Microsoft Office Access 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=fd698517-a504-427d-9e5f-fde8f102142c)  
(KB955439)  
(Kritický)
</td>
<td style="border:1px solid black;">
[Excel 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=fc612e9a-bdf3-4952-8ada-0de5a50973f0)  
(KB951548)  
(Důležitý)  
[Excel 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=fc612e9a-bdf3-4952-8ada-0de5a50973f0)  
(KB951548)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Microsoft Office PowerPoint 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7a7c21f0-5e0e-4dee-9710-1ce3d565913f)\*\*  
(KB948988)  
(Důležitý)  
[Microsoft Office PowerPoint 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=7a7c21f0-5e0e-4dee-9710-1ce3d565913f)\*\*  
(KB948988)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e0df2f6e-1102-461d-829f-5f3e2d7eb4b3)  
(KB921598)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Microsoft Word 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=13a37b76-9fec-426f-8176-3c95f934efe0)  
(KB954464)  
(Důležitý)  
[Microsoft Word 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=13a37b76-9fec-426f-8176-3c95f934efe0)  
(KB954464)  
(Důležitý)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Systém Microsoft Office 2007 a systém Microsoft Office 2007 Service Pack 1
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Excel 2007](http://www.microsoft.com/downloads/details.aspx?familyid=2753e8d6-e156-49ef-af2d-4c521c808ffd)  
(KB951546)  
(Důležitý)  
[Excel 2007 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=2753e8d6-e156-49ef-af2d-4c521c808ffd)  
(KB951546)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Microsoft Office PowerPoint 2007](http://www.microsoft.com/downloads/details.aspx?familyid=55fd618a-e9c5-4f1e-b9a5-b2e47ec98ef1)  
(KB951338)  
(Důležitý)  
[Microsoft Office PowerPoint 2007 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=55fd618a-e9c5-4f1e-b9a5-b2e47ec98ef1)  
(KB951338)  
(Důležitý)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
</tr>
<tr>
<th colspan="6" style="border:1px solid black;">
Jiný software sady Office
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS08-041**](http://go.microsoft.com/fwlink/?linkid=122912)
</td>
<td style="border:1px solid black;">
[**MS08-043**](http://go.microsoft.com/fwlink/?linkid=124306)
</td>
<td style="border:1px solid black;">
[**MS08-051**](http://go.microsoft.com/fwlink/?linkid=120394)
</td>
<td style="border:1px solid black;">
[**MS08-044**](http://go.microsoft.com/fwlink/?linkid=120819)
</td>
<td style="border:1px solid black;">
[**MS08-042**](http://go.microsoft.com/fwlink/?linkid=123160)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Stupeň maximální závažnosti bulletinu**
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
<td style="border:1px solid black;">
[**Vysoký**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office Project 2002 Service Pack 1
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Microsoft Office Project 2002 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=bf566ce6-23da-45e5-9c2b-c47331d30e79)  
(KB921596)  
(Důležitý)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Program SnapShot Viewer pro aplikaci Microsoft Access
</td>
<td style="border:1px solid black;">
[Program SnapShot Viewer pro aplikaci Microsoft Access](http://www.microsoft.com/downloads/details.aspx?familyid=7c22bb32-7ce3-4ff2-8366-ba2eb5135833)  
(KB957198)  
(Kritický)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office PowerPoint Viewer 2003
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Microsoft Office PowerPoint Viewer 2003](http://www.microsoft.com/downloads/details.aspx?familyid=911c8872-dec8-4b8e-9708-93dcabd3e036)  
(KB949041)  
(Důležitý)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Excel Viewer 2003 a Microsoft Office Excel Viewer 2003 Service Pack 3
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel Viewer 2003](http://www.microsoft.com/downloads/details.aspx?familyid=d7ed9e75-15f2-4950-98b3-93023ba0f4c1)  
(KB951589)  
(Důležitý)  
[Microsoft Office Excel Viewer 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=d7ed9e75-15f2-4950-98b3-93023ba0f4c1)  
(KB951589)  
(Důležitý)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office Excel Viewer
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel Viewer](http://www.microsoft.com/downloads/details.aspx?familyid=b574d906-7f09-49b0-80bf-e84dee8c4583)  
(KB955472)  
(Důležitý)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Converter Pack
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Microsoft Office Converter Pack](http://www.microsoft.com/downloads/details.aspx?familyid=199b08c7-6d79-4930-8f0c-31034629c485)  
(KB925256)  
(Důležitý)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Sada Microsoft Office Compatibility Pack pro formáty souborů aplikací Word, Excel a PowerPoint 2007 a sada Microsoft Office Compatibility Pack pro formáty souborů aplikací Word, Excel a PowerPoint 2007 Service Pack 1
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Sada Microsoft Office Compatibility Pack pro formáty souborů aplikací Word, Excel a PowerPoint 2007](http://www.microsoft.com/downloads/details.aspx?familyid=7afdae9b-9c74-4af7-9844-0e54221ea3b9)  
(KB951596)  
(Důležitý)  
[Sada Microsoft Office Compatibility Pack pro formáty souborů aplikací Word, Excel a PowerPoint 2007 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=7afdae9b-9c74-4af7-9844-0e54221ea3b9)  
(KB951596)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Sada Microsoft Office Compatibility Pack pro formáty souborů aplikací Word, Excel a PowerPoint 2007](http://www.microsoft.com/downloads/details.aspx?familyid=84ce5d58-0010-4945-bce9-67a41f898f2f) (KB954038)  
(Důležitý)  
[Sada Microsoft Office Compatibility Pack pro formáty souborů Word, Excel a PowerPoint 2007 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=84ce5d58-0010-4945-bce9-67a41f898f2f) (KB954038)  
(Důležitý)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office SharePoint Server 2007 a Microsoft Office SharePoint Server 2007 Service Pack 1
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Microsoft Office SharePoint Server 2007](http://www.microsoft.com/downloads/details.aspx?familyid=a7731749-b026-4765-808a-e151b990f0e1)\*  
(KB953397)  
(Důležitý)  
[Microsoft Office SharePoint Server 2007 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=a7731749-b026-4765-808a-e151b990f0e1)\*  
(KB953397)  
(Důležitý)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office SharePoint Server 2007 x64 Edition a Microsoft Office SharePoint Server 2007 x64 Edition Service Pack 1
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Microsoft Office SharePoint Server 2007 x64 Edition](http://www.microsoft.com/downloads/details.aspx?familyid=fc95ab88-2d31-44e1-a702-7cb10e83695b)\*  
(KB953397)  
(Důležitý)  
[Microsoft Office SharePoint Server 2007 x64 Edition Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=fc95ab88-2d31-44e1-a702-7cb10e83695b)\*  
(KB953397)  
(Důležitý)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
</tr>
<tr>
<th colspan="6" style="border:1px solid black;">
Microsoft Office for Mac
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identifikátor bulletinu**
</td>
<td style="border:1px solid black;">
[**MS08-041**](http://go.microsoft.com/fwlink/?linkid=122912)
</td>
<td style="border:1px solid black;">
[**MS08-043**](http://go.microsoft.com/fwlink/?linkid=124306)
</td>
<td style="border:1px solid black;">
[**MS08-051**](http://go.microsoft.com/fwlink/?linkid=120394)
</td>
<td style="border:1px solid black;">
[**MS08-044**](http://go.microsoft.com/fwlink/?linkid=120819)
</td>
<td style="border:1px solid black;">
[**MS08-042**](http://go.microsoft.com/fwlink/?linkid=123160)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Stupeň maximální závažnosti bulletinu**
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
<td style="border:1px solid black;">
[**Kritický**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2004 for Mac
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Microsoft Office 2004 for Mac](http://www.microsoft.com/downloads/details.aspx?familyid=ebd3af0c-3f62-4d18-bf45-881655683bd5)  
(KB956343)  
(Důležitý)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2004 for Mac](http://www.microsoft.com/downloads/details.aspx?familyid=ebd3af0c-3f62-4d18-bf45-881655683bd5)  
(KB956343)  
(Důležitý)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2008 for Mac
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
[Microsoft Office 2008 for Mac](http://www.microsoft.com/downloads/details.aspx?familyid=9515c70d-be80-4ade-856a-ea542f7d84e1)  
(KB956344)  
(Důležitý)
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
<td style="border:1px solid black;">
Netýká se
</td>
</tr>
</table>
 
**\*Poznámka pro aplikace Microsoft Office SharePoint Server 2007, Microsoft Office SharePoint Server 2007 Service Pack 1, Microsoft Office SharePoint Server 2007 x64 Edition a Microsoft Office SharePoint Server 2007 x64 Edition Service Pack 1 (MS08-043):** Aktualizace obsažená v bulletinu zabezpečení MS08-043 se týká serverů, které mají naistalovánu službu Excel Services, jak je tomu například u apliací Microsoft Office SharePoint Server 2007 Enterprise a Microsoft Office SharePoint Server 2007 For Internet Sites ve výchozí konfiguraci. Aplikace Microsoft Office SharePoint Server 2007 Standard neobsahuje službu Excel Services.

**\*\*Poznámka pro aplikace Microsoft Office PowerPoint 2003 Service Pack 2 a Microsoft Office PowerPoint 2003 Service Pack 3 (MS08-051):** Společnost Microsoft zveřejnila na webu služby Stažení softwaru nové aktualizační balíčky označené jako Verze 2. Zákazníci, kteří již ručně nainstalovali Verzi 1 této aktualizace z webu služby Stažení softwaru, musí přeinstalovat Verzi 2 této aktualizace. Zákazníci, kteří tuto aktualizaci nainstalovali pomocí služeb Microsoft Update nebo Office Update, nemusí provádět přeinstalaci. Další informace včetně jiných možností instalace nebo zástupných řešení naleznete v bulletinu [MS08-051](http://go.microsoft.com/fwlink/?linkid=120394).

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

-   Společnosti [ISC/SANS](http://isc.sans.org/) za oznámení chyby popsané v bulletinu MS08-042.
-   Společnosti [VeriSign iDefense VCP](http://www.idefense.com/vcp) za oznámení chyby popsané v bulletinu MS08-043.
-   Společnosti [TippingPoint](http://www.tippingpoint.com/) a organizaci [Zero Day Initiative](http://www.zerodayinitiative.com/) za oznámení chyby popsané v bulletinu MS08-043.
-   Jeremymu Funkovi za oznámení chyby popsané v bulletinu MS08-043.
-   Shaunu Colleyovi ze společnosti [NGS Software](http://www.nextgenss.com/) za oznámení chyby popsané v bulletinu MS08-044.
-   Damianu Putovi spolupracujícímu s organizací [Zero Day Initiative (ZDI)](http://www.zerodayinitiative.com/) za oznámení chyby popsané v bulletinu MS08-044.
-   Anonymnímu výzkumníkovi spolupracujícímu se společností [iDefense VCP](http://labs.idefense.com/) za oznámení chyby popsané v bulletinu MS08-044.
-   Damianu Putovi spolupracujícímu se společností [iDefense VCP](http://labs.idefense.com/) za oznámení chyby popsané v bulletinu MS08-044.
-   Yamatu Liovi ze společnosti [Palo Alto Networks](http://www.paloaltonetworks.com/) za oznámení chyby popsané v bulletinu MS08-045.
-   Tavisi Ormandymu z týmu [Google Security Team](http://www.google.com/) za oznámení chyby popsané v bulletinu MS08-045.
-   Samu Thomasovi spolupracujícímu se společností [TippingPoint](http://www.tippingpoint.com/) a organizací [Zero Day Initiative](http://www.zerodayinitiative.com/) za oznámení chyby popsané v bulletinu MS08-045.
-   Společnosti [TippingPoint](http://www.tippingpoint.com/) a organizaci [Zero Day Initiative](http://www.zerodayinitiative.com/) za oznámení chyby popsané v bulletinu MS08-045.
-   Junu Maovi ze společnosti [VeriSign iDefense Labs](http://labs.idefense.com/) za oznámení chyby popsané v bulletinu MS08-046.
-   Jorge Luisovi Alvarez Medinovi ze společnosti [Core Security Technologies](http://www.coresecurity.com/) za oznámení chyby popsané v bulletinu MS08-048.
-   Yamatu Liovi ze společnosti [Palo Alto Networks](http://www.paloaltonetworks.com/) za oznámení chyby popsané v bulletinu MS08-049.
-   Haifei Liovi z týmu [FortiGuard Global Security Research Team](http://www.fortiguardcenter.com) společnosti Fortinet za oznámení chyby popsané v bulletinu MS08-050.
-   Vadimovi Pogulievskymu z centra [Malicious Code Research Center](http://www.finjan.com/securitylab.aspx?id=547) společnosti Finjan za oznámení chyby popsané v bulletinu MS08-050.
-   Rubenu Santamartovi ze společnosti [Reversemode.com](http://reversemode.com/) spolupracujícímu se společností [iDefense Labs](http://labs.idefense.com/) za oznámení chyby popsané v bulletinu MS08-051.
-   Divizi ADLab společnosti [Venustech](http://www.venustech.com.cn/) za oznámení chyby popsané v bulletinu MS08-051.

#### Technická podpora

-   Uvedený software byl testován za účelem zjištění, kterých verzí se chyba týká. U dalších verzí skončila časově omezená podpora. Pokud chcete zjistit dobu, po kterou je pro určitou verzi softwaru poskytována podpora, navštivte web [Zásady poskytování technické podpory pro produkty společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=21742).
-   Zákazníci mohou získat technickou podporu na webu [služby technické podpory společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=21131). Hovory související s aktualizacemi zabezpečení jsou bezplatné.
-   Mezinárodní zákazníci získají podporu u místních zastoupení společnosti Microsoft. Technická podpora související s aktualizacemi zabezpečení je bezplatná. Další informace o možnostech kontaktování společnosti Microsoft v případě potřeby technické podpory získáte na [webu mezinárodní technické podpory](http://go.microsoft.com/fwlink/?linkid=21155).

#### Zřeknutí se záruky

Informace ve znalostní bázi Microsoft Knowledge Base jsou poskytovány tak, jak jsou, bez jakékoli záruky. Společnost Microsoft neposkytuje žádné záruky, výslovně uvedené či mlčky předpokládané, včetně záruk obchodovatelnosti a vhodnosti pro určitý účel. Společnost Microsoft ani její dodavatelé nenesou v žádném případě zodpovědnost za žádné škody, včetně přímých, nepřímých, náhodných či následných škod, ztráty zisku či zvláštních škod, a to ani v případě, že byli na možnost takových škod upozorněni. V některých zemích a právních řádech není dovoleno vyloučit nebo omezit odpovědnost, proto se výše uvedené omezení na vás nemusí vztahovat.

#### Revize

-   V1.0 (12. srpna 2008): Souhrnný bulletin byl publikován.
-   V2.0 (20. srpna 2008): Do bulletinu MS08-043 byla v části Software obsahující tuto chybu a umístění aktualizací ke stažení přidána poznámka, která vysvětluje, že se tato aktualizace týká serverů, které mají naistalovánu službu Excel Services, jak je tomu například u apliací Microsoft Office SharePoint Server 2007 Enterprise a Microsoft Office SharePoint Server 2007 For Internet Sites ve výchozí konfiguraci. Aplikace Microsoft Office SharePoint Server 2007 Standard neobsahuje službu Excel Services. Do bulletinu MS08-051 byla v části Software obsahující tuto chybu a umístění aktualizací ke stažení přidána také poznámka, že společnost Microsoft zveřejnila na webu služby Stažení softwaru nové aktualizační balíčky označené jako Verze 2, které jsou určeny pro aplikace Microsoft Office PowerPoint 2003 Service Pack 2 a Microsoft Office PowerPoint 2003 Service Pack 3. Zákazníci, kteří již ručně nainstalovali Verzi 1 této aktualizace z webu služby Stažení softwaru, musí přeinstalovat Verzi 2 této aktualizace. Zákazníci, kteří tuto aktualizaci nainstalovali pomocí služeb Microsoft Update nebo Office Update, nemusí provádět přeinstalaci.
-   V3.0 (15. října 2008): Zahrnuje aktualizaci pro program Snapshot Viewer pro aplikaci Microsoft Access (MS08-041). Uživatelé, kteří úspěšně nainstalovali aktualizaci pro aplikaci Microsoft Office 2000 Service Pack 3, Office XP Service Pack 2, Office 2003 Service Pack 2 nebo Office 2003 Service Pack 3, nemusí znovu instalovat aktualizaci samostatného programu Snapshot Viewer pro aplikaci Microsoft Access.

*Built at 2014-04-18T01:50:00Z-07:00*
