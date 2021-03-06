---
TOCTitle: 'MS04-JUL'
Title: 'Souhrnný bulletin zabezpečení společnosti Microsoft, červenec 2004'
ms:assetid: 'ms04-jul'
ms:contentKeyID: 61223932
ms:mtpsurl: 'https://technet.microsoft.com/cs-CZ/library/ms04-jul(v=Security.10)'
---

 

Souhrnný bulletin zabezpečení společnosti Microsoft, červenec 2004
==================================================================

Publikováno: 13. července 2004

**Verze:** 1.0

**Vydáno:** 13. července 2004  
**Číslo verze:** 1.0

Verze tohoto článku pro koncové uživatele je k dispozici na následujícím [webu](http://www.microsoft.com/security/default.mspx).

**Ochrana počítače:** V následujících umístěních získáte informace společnosti Microsoft týkající se zlepšení ochrany:

-   web [Chraňte svůj počítač](http://www.microsoft.com/cze/security/protect/) pro koncové uživatele,
-   web [Security Guidance Center](http://go.microsoft.com/fwlink/?linkid=21171) pro odborníky v oblasti IT.

**Strategie instalace aktualizací:** Web [Patch Management, Security Updates, and Downloads](http://go.microsoft.com/fwlink/?linkid=21168) obsahuje další informace o instalaci aktualizací zabezpečení podle doporučení společnosti Microsoft.

**Komunita odborníků v oblasti zabezpečení:** Na webu [IT Pro Security Zone](http://go.microsoft.com/fwlink/?linkid=21164) se můžete naučit, jak zlepšit zabezpečení a optimalizovat svou infrastrukturu IT, a diskutovat s dalšími členy komunity odborníků o tématech týkajících se zabezpečení.

**Služba zasílání oznámení o zabezpečení společnosti Microsoft:** Pokud chcete e-mailem dostávat automatická oznámení o vydání nových bulletinů zabezpečení společnosti Microsoft, přihlaste se k jejich odběru na této adrese: [Microsoft Security Notification Service](http://go.microsoft.com/fwlink/?linkid=21163).

#### Shrnutí

Součástí tohoto informačního zpravodajství jsou opravy nově zjištěných chyb zabezpečení. Tyto chyby jsou, podle stupně závažnosti, uvedeny níže:

Kritický (2)
------------

<span></span>
| Identifikátor bulletinu                  | Bulletin zabezpečení společnosti Microsoft MS04-022                                                                                      |
|------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------|
| **Název bulletinu**                      | [**Chyba zabezpečení ve službě Plánovač úloh umožňuje spuštění kódu (841873)**](http://technet.microsoft.com/security/bulletin/ms04-022) |
| **Základní shrnutí**                     | Ve službě Plánovač úloh existuje chyba zabezpečení umožňující vzdálené spuštění kódu. Důvodem je způsob ověřování názvů aplikací.        |
| **Stupeň maximální závažnosti**          | [Kritický](http://technet.microsoft.com/security/bulletin/rating)                                                                        |
| **Dopad této chyby zabezpečení**         | Vzdálené spuštění kódu                                                                                                                   |
| **Software, který obsahuje tuto chybu:** | **Windows**. Další informace získáte v části Software, který obsahuje tuto chybu, a umístění aktualizací ke stažení.                     |

| Identifikátor bulletinu                  | Bulletin zabezpečení společnosti Microsoft MS04-023                                                                                     |
|------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------|
| **Název bulletinu**                      | [**Chyba zabezpečení v nápovědě HTML umožňuje spuštění kódu (840315)**](http://technet.microsoft.com/security/bulletin/ms04-023)        |
| **Základní shrnutí**                     | Při zpracování speciálně vytvořené adresy URL otevírané metodou showHelp dochází k chybě zabezpečení umožňující vzdálené spuštění kódu. |
| **Stupeň maximální závažnosti**          | [Kritický](http://technet.microsoft.com/security/bulletin/rating)                                                                       |
| **Dopad této chyby zabezpečení**         | Vzdálené spuštění kódu                                                                                                                  |
| **Software, který obsahuje tuto chybu:** | **Windows**. Další informace získáte v části Software, který obsahuje tuto chybu, a umístění aktualizací ke stažení.                    |

Vysoký (4)
----------

<span></span>
| Identifikátor bulletinu                  | Bulletin zabezpečení společnosti Microsoft MS04-019                                                                                                                                                               |
|------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Název bulletinu**                      | [**Chyba zabezpečení ve Správci nástrojů umožňuje spuštění kódu (842526)**](http://technet.microsoft.com/security/bulletin/ms04-019)                                                                              |
| **Základní shrnutí**                     | Při spouštění aplikací Správcem nástrojů dochází k chybě zabezpečení, která způsobuje zvýšení úrovně oprávnění. Přihlášený uživatel může přimět Správce nástrojů ke spuštění aplikace se systémovými oprávněními. |
| **Stupeň maximální závažnosti**          | [Vysoký](http://technet.microsoft.com/security/bulletin/rating)                                                                                                                                                   |
| **Dopad této chyby zabezpečení**         | Zvýšení úrovně oprávnění v místním systému                                                                                                                                                                        |
| **Software, který obsahuje tuto chybu:** | **Windows**. Další informace získáte v části Software, který obsahuje tuto chybu, a umístění aktualizací ke stažení.                                                                                              |

| Identifikátor bulletinu                  | Bulletin zabezpečení společnosti Microsoft MS04-020                                                                                      |
|------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------|
| **Název bulletinu**                      | [**Chyba zabezpečení v systému POSIX umožňuje spuštění kódu (841872)**](http://technet.microsoft.com/security/bulletin/ms04-020)         |
| **Základní shrnutí**                     | Chyba zabezpečení v podsystému POSIX způsobující zvýšení oprávnění umožňuje přihlášenému uživateli převzít úplnou kontrolu nad systémem. |
| **Stupeň maximální závažnosti**          | [Vysoký](http://technet.microsoft.com/security/bulletin/rating)                                                                          |
| **Dopad této chyby zabezpečení**         | Zvýšení úrovně oprávnění v místním systému                                                                                               |
| **Software, který obsahuje tuto chybu:** | **Windows**. Další informace získáte v části Software, který obsahuje tuto chybu, a umístění aktualizací ke stažení.                     |

| Identifikátor bulletinu                  | Bulletin zabezpečení společnosti Microsoft MS04-021                                                                  |
|------------------------------------------|----------------------------------------------------------------------------------------------------------------------|
| **Název bulletinu**                      | [**Aktualizace zabezpečení pro IIS 4.0 (841373)**](http://technet.microsoft.com/security/bulletin/ms04-021)          |
| **Základní shrnutí**                     | V produktu Internet Information Server 4.0 se vyskytuje chyba zabezpečení způsobující přetečení paměti.              |
| **Stupeň maximální závažnosti**          | [Vysoký](http://technet.microsoft.com/security/bulletin/rating)                                                      |
| **Dopad této chyby zabezpečení**         | Vzdálené spuštění kódu                                                                                               |
| **Software, který obsahuje tuto chybu:** | **Windows**. Další informace získáte v části Software, který obsahuje tuto chybu, a umístění aktualizací ke stažení. |

| Identifikátor bulletinu                  | Bulletin zabezpečení společnosti Microsoft MS04-024                                                                                                                                          |
|------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Název bulletinu**                      | [**Chyba zabezpečení v prostředí systému Windows může umožnit vzdálené spuštění kódu (839645)**](http://go.microsoft.com/fwlink/?linkid=30585)                                               |
| **Základní shrnutí**                     | Při spouštění aplikací v prostředí systému Windows dochází k chybě zabezpečení umožňující vzdálené spuštění kódu. Zneužití této chyby zabezpečení je možné pouze při interakci s uživatelem. |
| **Stupeň maximální závažnosti**          | [Vysoký](http://technet.microsoft.com/security/bulletin/rating)                                                                                                                              |
| **Dopad této chyby zabezpečení**         | Vzdálené spuštění kódu                                                                                                                                                                       |
| **Software, který obsahuje tuto chybu:** | **Windows**. Další informace získáte v části Software, který obsahuje tuto chybu, a umístění aktualizací ke stažení.                                                                         |

Mírný (1)
---------

<span></span>
| Identifikátor bulletinu                  | Bulletin zabezpečení společnosti Microsoft MS04-018                                                                                                        |
|------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Název bulletinu**                      | [**Kumulativní oprava zabezpečení pro aplikaci Outlook Express (823353)**](http://technet.microsoft.com/security/bulletin/ms04-018)                        |
| **Základní shrnutí**                     | Chyba zabezpečení způsobující odmítnutí služby může umožnit útočníkovi odeslat speciálně vytvořený e-mail, který způsobí selhání aplikace Outlook Express. |
| **Stupeň maximální závažnosti**          | [Mírný](http://technet.microsoft.com/security/bulletin/rating)                                                                                             |
| **Dopad této chyby zabezpečení**         | Odmítnutí služby                                                                                                                                           |
| **Software, který obsahuje tuto chybu:** | **Windows, Outlook Express**. Další informace získáte v části Software, který obsahuje tuto chybu, a umístění aktualizací ke stažení.                      |

Software, který obsahuje tuto chybu, a umístění aktualizací ke stažení
----------------------------------------------------------------------

<span></span>
**Jak pracovat s touto tabulkou**

V této tabulce zjistíte, které aktualizace zabezpečení bude třeba nainstalovat. Přečtěte si seznam všech programů a součástí a zjistěte, zda jsou u nich aktualizace zabezpečení uvedeny. Pokud se program nebo součást v seznamu nachází, je u nich uveden dopad chyby zabezpečení s odkazem na příslušnou aktualizaci.

Čísla v závorce \[x\], která v tabulce vidíte, označují, že problém je vysvětlen dodatečnou poznámkou. Tyto poznámky jsou umístěny na konci tabulky.

**Poznámka:** Jedna chyba zabezpečení může vyžadovat instalaci více aktualizací. Přečtěte si celý sloupec u každého identifikátoru bulletinu. Zjistíte v něm, které aktualizace nainstalovat v závislosti na programech nebo součástech nainstalovaných ve vašem systému.

**Software, který obsahuje tuto chybu, a umístění aktualizací ke stažení**

 
<table style="border:1px solid black;">
<colgroup>
<col width="12%" />
<col width="12%" />
<col width="12%" />
<col width="12%" />
<col width="12%" />
<col width="12%" />
<col width="12%" />
<col width="12%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" ></th>
<th style="border:1px solid black;" >Podrobnosti</th>
<th style="border:1px solid black;" >Podrobnosti</th>
<th style="border:1px solid black;" >Podrobnosti</th>
<th style="border:1px solid black;" >Podrobnosti</th>
<th style="border:1px solid black;" >Podrobnosti</th>
<th style="border:1px solid black;" >Podrobnosti</th>
<th style="border:1px solid black;" >Podrobnosti</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Identifikátor bulletinu</strong></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms04-018"><strong>MS04-018</strong></a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms04-019"><strong>MS04-019</strong></a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms04-020"><strong>MS04-020</strong></a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms04-021"><strong>MS04-021</strong></a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms04-022"><strong>MS04-022</strong></a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms04-023"><strong>MS04-023</strong></a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms04-024"><strong>MS04-024</strong></a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Stupeň maximální závažnosti</strong></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/rating"><strong>Mírný</strong></a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/rating"><strong>Vysoký</strong></a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/rating"><strong>Vysoký</strong></a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/rating"><strong>Vysoký</strong></a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/rating"><strong>Kritický</strong></a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/rating"><strong>Kritický</strong></a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/rating"><strong>Vysoký</strong></a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Systémy Windows, které obsahují tuto chybu:</strong></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows Server™ 2003</td>
<td style="border:1px solid black;"><strong>[3]</strong></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=8b53c35d-e9ed-46ad-936c-30c8e3a7e606&amp;displaylang=en">Kritický</a></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=41c7bb26-3500-4492-a447-33440c404e4f&amp;displaylang=en">Vysoký</a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows Server 2003 64-Bit Edition</td>
<td style="border:1px solid black;"><strong>[3]</strong></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=df0c5c4e-d986-4ad5-95e0-e87106d7c019&amp;displaylang=en">Kritický</a></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=79cca663-5b72-4345-a3ee-404b466731bc&amp;displaylang=en">Vysoký</a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows XP</td>
<td style="border:1px solid black;"><strong>[3]</strong></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=8e8d0a2d-d3b9-4de8-8b6f-fc27715bc0cf&amp;displaylang=en">Kritický</a></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=8b412c7f-44ad-4e77-8973-fd3e84cc496a&amp;displaylang=en">Kritický</a></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=c3365b8e-666b-4c82-a9ed-fc0f84f107ba&amp;displaylang=en">Vysoký</a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows XP a aktualizací Service Pack 1</td>
<td style="border:1px solid black;"><strong>[3]</strong></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=8e8d0a2d-d3b9-4de8-8b6f-fc27715bc0cf&amp;displaylang=en">Kritický</a></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=8b412c7f-44ad-4e77-8973-fd3e84cc496a&amp;displaylang=en">Kritický</a></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=c3365b8e-666b-4c82-a9ed-fc0f84f107ba&amp;displaylang=en">Vysoký</a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows XP 64-Bit Edition s aktualizací Service Pack 1</td>
<td style="border:1px solid black;"><strong>[3]</strong></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=7b4ac0fa-7954-4993-85a1-85298f122ce0&amp;displaylang=en">Kritický</a></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=0042db67-c58b-412c-a24f-9d2aa8071897&amp;displaylang=en">Kritický</a></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=3fee07f5-9e31-481e-9f89-2549f51147af&amp;displaylang=en">Vysoký</a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows XP 64-Bit Edition, verze 2003</td>
<td style="border:1px solid black;"><strong>[3]</strong></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=df0c5c4e-d986-4ad5-95e0-e87106d7c019&amp;displaylang=en">Kritický</a></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=79cca663-5b72-4345-a3ee-404b466731bc&amp;displaylang=en">Vysoký</a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows 2000 s aktualizací Service Pack 2</td>
<td style="border:1px solid black;"><strong>[3]</strong></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=94cd9925-d99b-4cb6-b51e-248d4fd8af07&amp;displaylang=en">Vysoký</a></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=05203a7e-4a11-4f88-aa73-75a6c81466b8&amp;displaylang=en">Vysoký</a></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=bbf3c8a1-7d72-4ce9-a586-7c837b499c08&amp;displaylang=cs">Kritický</a></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=3f2f1a7d-5cf2-4791-a7ee-07f20f75796c&amp;displaylang=cs">Kritický</a></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=397be12b-a026-41a6-8e98-b4027bc6a110&amp;displaylang=en">Vysoký</a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows 2000 s aktualizací Service Pack 3</td>
<td style="border:1px solid black;"><strong>[3]</strong></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=94cd9925-d99b-4cb6-b51e-248d4fd8af07&amp;displaylang=cs">Vysoký</a></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=05203a7e-4a11-4f88-aa73-75a6c81466b8&amp;displaylang=cs">Vysoký</a></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=bbf3c8a1-7d72-4ce9-a586-7c837b499c08&amp;displaylang=cs">Kritický</a></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=3f2f1a7d-5cf2-4791-a7ee-07f20f75796c&amp;displaylang=cs">Kritický</a></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=397be12b-a026-41a6-8e98-b4027bc6a110&amp;displaylang=cs">Vysoký</a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows 2000 s aktualizací Service Pack 4</td>
<td style="border:1px solid black;"><strong>[3]</strong></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=94cd9925-d99b-4cb6-b51e-248d4fd8af07&amp;displaylang=en">Vysoký</a></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=05203a7e-4a11-4f88-aa73-75a6c81466b8&amp;displaylang=cs">Vysoký</a></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=bbf3c8a1-7d72-4ce9-a586-7c837b499c08&amp;displaylang=cs">Kritický</a></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=3f2f1a7d-5cf2-4791-a7ee-07f20f75796c&amp;displaylang=cs">Kritický</a></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=397be12b-a026-41a6-8e98-b4027bc6a110&amp;displaylang=cs">Vysoký</a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows NT® Workstation 4.0 s aktualizací Service Pack 6a</td>
<td style="border:1px solid black;"><strong>[3]</strong></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=25993f70-191b-4e35-aa1b-0aa1a7027880&amp;displaylang=cs">Vysoký</a></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=3a2b38c5-fa73-49ec-9eef-06fe8d6495c0&amp;displaylang=en">Vysoký</a></td>
<td style="border:1px solid black;"><strong>[1]</strong></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=18d026d3-3d93-4845-94ad-4f2656500d7a&amp;displaylang=cs">Kritický</a></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=53f0c9c1-d72f-48e8-8f70-b29a70a618e2&amp;displaylang=cs">Vysoký</a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows NT Server 4.0 s aktualizací Service Pack 6a</td>
<td style="border:1px solid black;"><strong>[3]</strong></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=c2018a81-446c-4930-a6cc-ea5b5960ff05&amp;displaylang=en">Vysoký</a></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=3a2b38c5-fa73-49ec-9eef-06fe8d6495c0&amp;displaylang=en">Vysoký</a></td>
<td style="border:1px solid black;"><strong>[1]</strong></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=e64081d5-2ea2-49a9-b175-4e39cce169b0&amp;displaylang=en">Kritický</a></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=58906e66-064c-4358-9bf9-bc67b1f57bc5&amp;displaylang=en">Vysoký</a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows NT Workstation 4.0 s aktualizací Service Pack 6a a Windows NT Server 4.0 s aktualizací Service Pack 6a se systémem Active Desktop</td>
<td style="border:1px solid black;"><strong>[3]</strong></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=87096271-9716-4a46-93f3-d41fcbdf989a&amp;displaylang=cs">Vysoký</a> <strong>[5]</strong></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows NT Server 4.0, Terminal Server Edition, s aktualizací Service Pack 6</td>
<td style="border:1px solid black;"><strong>[3]</strong></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=9cfc4af3-b0bc-4798-bc23-f45739e3b802&amp;displaylang=en">Vysoký</a></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"><strong>[1]</strong></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=3509d5a4-1bb1-4d90-bce6-9b178bda14eb&amp;displaylang=en">Kritický</a></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=34035ce3-1998-4693-8330-c4515a13407d&amp;displaylang=en">Vysoký</a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows Millennium Edition (Windows ME)</td>
<td style="border:1px solid black;"><strong>[2]</strong></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=a71faa02-d34c-47cb-bc99-820013211463&amp;displaylang=cs">Kritický</a></td>
<td style="border:1px solid black;"><strong>[2]</strong></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows 98 Druhé vydání</td>
<td style="border:1px solid black;"><strong>[2]</strong></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=a71faa02-d34c-47cb-bc99-820013211463&amp;displaylang=cs">Kritický</a></td>
<td style="border:1px solid black;"><strong>[2]</strong></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows 98</td>
<td style="border:1px solid black;"><strong>[2]</strong></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=a71faa02-d34c-47cb-bc99-820013211463&amp;displaylang=cs">Kritický</a></td>
<td style="border:1px solid black;"><strong>[2]</strong></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Součásti operačního systému Windows, které obsahují tuto chybu:</strong></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Outlook Express 5.5 s aktualizací Service Pack 2</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=9a8d1bf2-93c5-41a9-b79a-31d54743ba0e&amp;displaylang=cs">Žádný</a> <strong>[4]</strong></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Outlook Express 6</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=d5900df1-10ab-4850-9064-3070ce1f948a&amp;displaylang=cs">Mírný</a></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Outlook Express 6 s aktualizací Service Pack 1</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=ad6a96bc-daf0-4eab-89b8-bd702b3e3e5d&amp;displaylang=cs">Žádný</a> <strong>[4]</strong></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Outlook Express 6 s aktualizací Service Pack 1 (64-Bit Edition)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=adccf304-6cfc-48d6-9a3f-2a601c3a04a5&amp;displaylang=en">Žádný</a> <strong>[4]</strong></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Outlook Express 6 v systému Windows Server 2003</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=c99aafcd-b99b-4b13-a366-5f8edc83633f&amp;displaylang=cs">Žádný</a> <strong>[4]</strong></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Microsoft Outlook Express 6 v systému Windows Server 2003 (64-Bit Edition)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=10d1aad0-0313-4beb-a174-84cf573f31fd&amp;displaylang=en">Žádný</a> <strong>[4]</strong></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Internet Explorer 6 s aktualizací Service Pack 1</td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=d4f57f82-d2ba-411a-8b40-77a3d80e58ac&amp;displaylang=cs">Vysoký</a></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
</tr>
</tbody>
</table>
  
**Poznámky**
  
**\[1\]** Ve výchozí instalaci není tento operační systém touto chybou ohrožen. Jestliže jsou v něm však nainstalovány další programy nebo součásti, může tuto chybu obsahovat. V tomto konkrétním případě je systém Windows NT4 ohrožen, pokud je v něm nainstalována aplikace Internet Explorer 6 s aktualizací Service Pack 1. Další informace získáte v příslušném bulletinu zabezpečení.
  
**\[2\]** Tento operační systém je touto chybou zabezpečení ohrožen. Není však ohrožen kriticky. Pro tento operační systém nejsou obvykle vyvíjeny aktualizace zabezpečení pro nekritické potíže. Další informace o Zásadách společnosti Microsoft pro poskytování technické podpory pro operační systém naleznete na tomto[webu](http://support.microsoft.com/default.aspx?pr=lifean1). Další informace získáte v příslušném bulletinu zabezpečení.
  
**\[3\]** Pro tento operační systém je k dispozici aktualizace zabezpečení. Další informace získáte v tabulce u součásti, která tuto chybu obsahuje (Microsoft Outlook Express), a v příslušném bulletinu zabezpečení.
  
**\[4\]** Aktualizace zabezpečení obsažená v tomto bulletinu neřeší žádné chyby zabezpečení této verze aplikace Outlook Express, ale omezuje výchozí nastavení zabezpečení aplikace Outlook Express 5.5 s aktualizací Service Pack 2 a řeší chování aplikace uvedené v bulletinu MS04-013 pro aplikaci Outlook Express 6 s aktualizací SP1 a vyšší, kde vytváří kopii Adresáře systému Windows v předvídatelném umístění s názvem souboru “~”.
  
**\[5\]** Přečtěte si bulletin popisující jak zjistit, zda je nainstalován systém Active Desktop.
  
Instalace  
---------
  
<span></span>
**Služba Microsoft Software Update Services (SUS):**
  
Pomocí služby SUS mohou správci systému rychle a spolehlivě instalovat nejnovější důležité aktualizace zabezpečení pro servery se systémem Windows 2000 a Windows Server 2003 i pro stolní počítače se systémem Windows 2000 Professional nebo Windows XP Professional.
  
Další informace o způsobu instalace této aktualizace zabezpečení pomocí služby SUS získáte na webu služby [Software Update Services](http://www.microsoft.com/cze/windowsserversystem/sus/).
  
**Systems Management Server (SMS):**
  
Server SMS představuje podnikové řešení pro správu aktualizací s rozsáhlými možnostmi konfigurace. Umožňuje správcům identifikovat systémy Windows, které potřebují aktualizace zabezpečení, a provést řízenou instalaci těchto aktualizací v celém podniku, a to s minimálním dopadem na koncové uživatele. Další informace o tom, jak mohou správci pomocí serveru SMS instalovat aktualizace zabezpečení, získáte na webu [SMS 2003 Security Patch Management](http://www.microsoft.com/smserver/evaluation/capabilities/patch.asp). Uživatelé serveru SMS 2.0 mohou při instalaci aktualizací zabezpečení použít také sadu [Software Updates Service Feature Pack](http://www.microsoft.com/technet/prodtechnol/sms/sms2/downloads/featurepacks/suspack/default.mspx). Další informace o serveru SMS získáte na [webu tohoto produktu](http://www.microsoft.com/cze/servers/smserver/).
  
**Poznámka:** Server SMS využívá nástroj MBSA (Microsoft Baseline Security Analyzer) a nástroj pro rozpoznávání sady Microsoft Office, a poskytuje tak širokou podporu pro zjišťování a instalaci aktualizací uvedených v bulletinech zabezpečení. Tyto nástroje nemusí některé aktualizace softwaru zjistit. V těchto případech mohou správci směrovat aktualizace do určitých počítačů pomocí funkcí pro soupisy serveru SMS. Další informace o tomto postupu najdete na následujícím [webu](http://www.microsoft.com/technet/prodtechnol/sms/sms2003/patchupdate.mspx). Některé aktualizace zabezpečení vyžadují po restartování počítače oprávnění správce. Správci mohou k instalaci těchto aktualizací použít nástroj Elevated Rights Deployment Tool (k dispozici v sadě [**SMS 2003 Administration Feature Pack**](http://www.microsoft.com/technet/prodtechnol/sms/sms2003/downloads/featurepacks/adminpack.mspx) a [SMS 2.0 Administration Feature Pack](http://www.microsoft.com/technet/prodtechnol/sms/sms2/downloads/featurepacks/adminpack/default.mspx)).
  
**Nástroje QChain.exe a Update.exe:**
  
Společnost Microsoft vydala nástroj QChain.exe, který je možné spustit z příkazového řádku. Jeho pomocí může správce systému bezpečně zřetězit aktualizace zabezpečení.*Zřetězení*je termín pro instalaci více aktualizací bez restartování počítače mezi jednotlivými instalacemi. Nástroj Update.exe, který používají aktualizace popsané v tomto informačním zpravodaji, má funkci zřetězení integrovánu. U systémů Windows 2000 Service Pack 2 nebo vyšších, Windows XP a Windows Server 2003 není ke zřetězení těchto aktualizací nástroj QChain.exe třeba, přesto však aktualizace těchto systémů podporuje, a umožňuje tak vytvoření konzistentního instalačního skriptu pro všechny platformy. Další informace o nástroji QChain získáte na tomto [webu](http://go.microsoft.com/fwlink/?linkid=21156).
  
**Nástroj Microsoft Baseline Security Analyzer (MBSA):**
  
Pomocí nástroje MBSA mohou správci kontrolovat místní i vzdálené systémy, a zjišťovat tak, jestli v nich nechybí některé aktualizace zabezpečení nebo jestli v nastavení zabezpečení systému nedošlo k některým běžným chybám. Další informace o nástroji MBSA získáte na webu [Microsoft Baseline Security Analyzer](http://go.microsoft.com/fwlink/?linkid=21134).
  
#### Další informace:
  
**Poděkování**
  
Společnost Microsoft tímto [děkuje](http://go.microsoft.com/fwlink/?linkid=21127) za spolupráci při ochraně zákazníků:
  
-   Cesaru Cerrudovi ze společnosti [Application Security Inc.](http://www.appsecinc.com/) za oznámení chyby popsané v bulletinu [MS04-019](http://technet.microsoft.com/security/bulletin/ms04-019).  
-   Rafalu Wojtczukovi spolupracujícímu se společností [Network Associates](http://www.nai.com/) za oznámení chyby popsané v bulletinu [MS04-020](http://technet.microsoft.com/security/bulletin/ms04-020).  
-   Brettu Mooreovi ze společnosti [Security-Assessment.com](http://www.security-assessment.com/) za oznámení chyby popsané v bulletinu [MS04-022](http://technet.microsoft.com/security/bulletin/ms04-022).  
-   [Dustinu Schneiderovi](https://technet.microsoft.com/cs-CZ/mailto:dschn@verizon.net) za oznámení chyby popsané v bulletinu [MS04-022](http://technet.microsoft.com/security/bulletin/ms04-022).  
-   Peteru Winter-Smithovi ze společnosti [Next Generation Security Software Ltd.](http://www.ngssoftware.com/) za oznámení chyby popsané v bulletinu [MS04-022](http://technet.microsoft.com/security/bulletin/ms04-022).  
-   Brettu Mooreovi ze společnosti Security-Assessment.com za oznámení chyby popsané v bulletinu [MS04-023](http://technet.microsoft.com/security/bulletin/ms04-023).  
-   **Získání dalších aktualizací zabezpečení:**
  
    Aktualizace odstraňující další problémy se zabezpečením získáte v následujících umístěních:
  
    -   Aktualizace zabezpečení jsou k dispozici v centru pro stahování [Microsoft Download Center](http://go.microsoft.com/fwlink/?linkid=21129), kde je nejsnáze naleznete hledáním podle klíčového slova oprava\_zabezpečení (security\_patch).  
    -   Aktualizace pro klientské platformy jsou k dispozici na webu [Windows Update](http://go.microsoft.com/fwlink/?linkid=21130).
  
    **Technická podpora:**
  
    -   Zákazníci v USA a Kanadě mohou získat technickou podporu prostřednictvím služeb [Microsoft Product Support Services](http://go.microsoft.com/fwlink/?linkid=21131) na čísle 1-866-PCSAFETY. Hovory související s aktualizacemi zabezpečení jsou bezplatné.  
    -   Zákazníci v ostatních zemích mohou získat technickou podporu od místních poboček společnosti Microsoft. Technická podpora související s aktualizacemi zabezpečení je bezplatná. Další informace o možnostech kontaktování společnosti Microsoft v případě potřeby pomoci naleznete na webu [mezinárodní podpory](http://go.microsoft.com/fwlink/?linkid=21155).
  
    **Zdroje informací o zabezpečení:**
  
    -   Další informace o zabezpečení produktů společnosti Microsoft nabízí web [Microsoft TechNet Security](http://go.microsoft.com/fwlink/?linkid=21132).  
    -   [Microsoft Software Update Services](http://www.microsoft.com/cze/windowsserversystem/sus/)  
    -   [Microsoft Baseline Security Analyzer](http://go.microsoft.com/fwlink/?linkid=21134) (MBSA)  
    -   [Windows Update](http://go.microsoft.com/fwlink/?linkid=21130)  
    -   Katalog systému Windows Update: Další informace o katalogu systému Windows Update získáte v článku [323166](http://support.microsoft.com/default.aspx?scid=kb;cs;323166) znalostní báze Microsoft Knowledge Base.  
    -   [Office Update](http://go.microsoft.com/fwlink/?linkid=21135)
  
    **Zřeknutí se záruky:**
  
    Informace ve znalostní bázi Microsoft Knowledge Base jsou poskytovány tak, jak jsou, bez jakékoli záruky. Společnost Microsoft neposkytuje žádné záruky, výslovně uvedené či mlčky předpokládané, včetně záruk obchodovatelnosti a vhodnosti pro určitý účel. Společnost Microsoft ani její dodavatelé nenesou v žádném případě zodpovědnost za žádné škody, včetně přímých, nepřímých, náhodných či následných škod, ztráty zisku či zvláštních škod, a to ani v případě, že byli na možnost takových škod upozorněni. V některých zemích či právních řádech není dovoleno vyloučit nebo omezit odpovědnost, proto se výše uvedené omezení na vás nemusí vztahovat.
  
    **Revize:**
  
    -   Verze 1.0 (13. července 2004): Bulletin byl publikován.
  
*Built at 2014-04-18T01:50:00Z-07:00*
