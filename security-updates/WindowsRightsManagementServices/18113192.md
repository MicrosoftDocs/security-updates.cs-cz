---
TOCTitle: Plánování externích uživatelů služby RMS
Title: Plánování externích uživatelů služby RMS
ms:assetid: '107e1338-4dcf-4ed5-a49d-e875cc883db1'
ms:contentKeyID: 18113192
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc720190(v=WS.10)'
---

Plánování externích uživatelů služby RMS
========================================

Tato část popisuje topologie, jejichž implementace umožní organizaci i externím uživatelům sdílet obsah chráněný službou RMS prostřednictvím Internetu.

Clustery služby RMS je možné nasadit pro interní i externí využití pomocí některé z následujících možností:

-   Nastavte adresu URL clusteru kořenové certifikace tak, aby k ní bylo možné získat přístup prostřednictvím Internetu. Zajistěte překlad této adresy URL pro stejný cluster také v intranetu na serverech RMS. Po provedení tohoto kroku bude adresa URL licence k publikování, pomocí které počítače koncových uživatelů získávají licence, fungovat v rámci intranetu i Internetu.
-   Nastavte zvláštní cluster služby RMS určený jen pro publikování na Internetu. Veškerý obsah, pro který je třeba získat licence z Internetu, by měl být publikován v tomto clusteru. Je-li třeba zpřístupnit obsah interně i externě, měl by být publikován na obou těchto místech. Jako alternativa musí pro uživatele existovat možnost spojení s internetovým serverem.

Povolení externích uživatelů
----------------------------

Externí uživatele můžete do instalace služby RMS zahrnout tak, že pro tyto uživatele vytvoříte interní účty a povolíte jim přístup do podnikové sítě prostřednictvím virtuální privátní sítě (VPN). Účtu může být přiřazena interní poštovní schránka nebo e-mailová adresa, která odkazuje na externí poštovní schránku.

Pokud nastavíte interní poštovní schránku, musí interní autoři při publikování obsahu chráněného službou RMS zadat e-mailovou adresu, která je spojena s interní poštovní schránkou (namísto jakékoli e-mailové adresy externího uživatele mimo danou organizaci). Pokud nastavíte externí poštovní schránku, musí interní autoři při publikování obsahu chráněného službou RMS zadat externí e-mailovou adresu příslušného účtu.

Chcete-li současně zajistit zabezpečení sítě i podporu síťového přístupu externích uživatelů, můžete vytvořit zvláštní doménovou strukturu služby Active Directory pro partnerské účty. Díky této topologii je možné vytvořit zvláštní cluster kořenové certifikace pro část systému služby RMS, která je vystavena Internetu. Uvedený krok externím uživatelům umožní příjem certifikátu počítače RMS a certifikátu účtu práv z tohoto clusteru kořenové certifikace vystaveného Internetu při prvním přístupu k obsahu chráněnému službou RMS.

Pokud se rozhodnete implementovat zvláštní doménovou strukturu pro externí partnery, která bude obsahovat partnerské účty, je nutné do ní nainstalovat službu RMS. Potom můžete pomocí funkce důvěryhodné domény publikování vytvořit mezi oběma servery RMS vztah důvěryhodnosti. Zároveň je třeba, aby externí záznamy DNS identifikovaly adresu URL externího clusteru instalace služby RMS v doménové struktuře vytvořené pro externí partnery. Vytvoření uvedeného vztahu důvěryhodnosti umožní externímu serveru RMS vydávat licence k použití pro veškerý obsah vydaný interním systémem služby RMS a naopak.

Alternativním řešením k nastavení serveru RMS v externí doménové struktuře by mohlo být filtrování příchozího toku dat pomocí serveru (například serveru ISA) a vracení požadavků na licence serveru proxy služby RMS zpět na interní server RMS.

Použití externích certifikátů
-----------------------------

Přístup k obsahu chráněnému službou RMS můžete externím uživatelům povolit tak, že nastavíte zvláštní server RMS jako server správy licencí vystavený Internetu, publikujete obsah z tohoto serveru správy licencí a zadáte na něm vztah důvěryhodnosti.

Část nasazení služby RMS vystavená Internetu představuje zvláštní server správy licencí, který je určen k použití pro Internet. Jedná se o součást stejného clusteru, do kterého patří i interní instalace správy licencí. Využívá se zde stejná databáze a stejná adresa URL jako u interní instalace správy licencí. Jedná se o jediný server, který může přijímat data přicházející z Internetu.

Pokud budou externí uživatelé z tohoto serveru správy licencí služby RMS požadovat licenci k použití, budou používat certifikát účtu práv z jiné služby certifikace RMS, která je na uvedeném serveru správy licencí nastavena jako důvěryhodná.

#### Nastavení důvěryhodnosti certifikátů účtů práv služby Passport

Organizace může nastavit důvěryhodnost certifikátů účtů práv založených na pověřeních služby Microsoft .NET Passport. Tyto certifikáty účtů vyžadují, aby uživatelé získali certifikáty účtů práv přímo od služby Microsoft Certification Service, která je k dispozici na Internetu.

V případě tohoto modelu obdrží externí uživatelé certifikáty počítače RMS a certifikáty účtů práv od společnosti Microsoft. Po publikování obsahu musí být účet služby Microsoft .NET Passport externího uživatele uveden v licenci k publikování jako příjemce.

Účet služby Microsoft® .NET Passport musí odpovídat účtu této služby použitému v okamžiku, kdy uživatel stahoval certifikát účtů práv od společnosti Microsoft. Je nutné, aby autor tento účet zadal při přidávání příjemců v aplikaci s podporou služby RMS. Pokud se uvedené účty neshodují, nelze obsah využívat.

#### Nastavení důvěryhodnosti jiných externích certifikátů

Jestliže je služba RMS nasazena také ve společnosti externího uživatele, může se stát, že budete chtít nastavit vztah důvěryhodnosti i s touto společností. Chcete-li tento krok provést, požádejte danou společnost, aby exportovala svůj certifikát serveru RMS pro poskytování licencí a odeslala jej vaší organizaci. Certifikát potom můžete naimportovat pomocí konzoly pro správu služby RMS na server správy licencí vystavený Internetu.
