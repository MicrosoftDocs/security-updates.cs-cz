---
TOCTitle: Přidání serverů do existující instalace
Title: Přidání serverů do existující instalace
ms:assetid: '7f3598ff-cd19-4daa-aa65-877f7f95a8ec'
ms:contentKeyID: 18113396
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747648(v=WS.10)'
---

Přidání serverů do existující instalace
=======================================

Do instalace služby RMS můžete podle potřeby přidávat servery. Můžete tak například zajistit zvýšené požadavky nebo nahradit servery určené k vyřazení. Každá instalace služby RMS musí obsahovat nejméně jeden server kořenové certifikace a nepovinně může obsahovat další servery kořenové certifikace v clusteru. Každá instalace služby RMS může také obsahovat samostatné nebo clusterované servery správy licencí.

Servery je možné do instalace služby RMS přidávat kterýmkoli z následujících způsobů:

-   přidání jednoho nebo několika serverů RMS do clusteru kořenové certifikace,
-   přidání nového samostatného serveru správy licencí,
-   přidání jednoho nebo několika serverů RMS do clusteru správy licencí.

**Přidání serverů kořenové certifikace**

Přidání jednoho nebo několika serverů RMS do clusteru kořenové certifikace představuje ve většině případů nejvhodnější způsob zajištění vyšší dostupnosti a redundance daného nasazení. Cluster kořenové certifikace tvoří jeden nebo několik serverů kořenové certifikace. Na rozdíl od serverů správy licencí, které poskytují pouze služby licencování a publikování, zajišťují servery kořenové certifikace všechny funkce služby RMS.

Během instalace a zajištění můžete určit, aby byl server přidán do clusteru. Pokud tak učiníte, bude nový server RMS automaticky nakonfigurován jako člen clusteru. Podrobné pokyny k instalaci a zajištění serveru RMS, který má být přidán do clusteru kořenové certifikace, naleznete v tomto tématu později v části [Instalace služby RMS s aktualizací Service Pack 1](https://technet.microsoft.com/dab20175-a690-43f8-b943-768d289daa0d) a [Přidání serveru do clusteru](https://technet.microsoft.com/db635238-5528-4bec-9cc6-8244e2b3d733).

Kromě zajištění je při prvním vytváření clusteru třeba podle potřeby nastavit také software nebo hardware řízení clusterů a vyrovnávání zatížení. Pokud byl již cluster implementován, je třeba konfigurovat software nebo hardware vyrovnávání zatížení pro práci s novým členem.

**Přidání serverů správy licencí**

Na rozdíl od serverů kořenové certifikace, které zajišťují všechny funkce služby RMS, poskytují servery správy licencí pouze služby licencování a publikování.

Použití serverů správy licencí je nepovinné a nejčastěji jsou tyto servery implementovány za účelem řešení určitých licenčních požadavků, například:

-   Podpora požadavků specifické správy práv v určitém oddělení. Některá skupina v rámci organizace může mít například nestandardní požadavky zabezpečení správy práv a může mít zájem na úplném řízení implementace správy svých licencí. Vzhledem k tomu, že v doménové struktuře může být pouze jeden server kořenové certifikace, nastavení samostatného serveru kořenové certifikace zřejmě není vhodným řešením. V tomto případě lze nastavit jeden server nebo cluster správy licencí, který bude vyhrazen pro potřeby této skupiny. Pro tento server nebo cluster je pak možné nastavit zásady práv odděleně.
-   Podpora správy práv pro externí obchodní partnery jako součásti extranetu, v němž je pro jednotlivé obchodní partnery vyžadováno striktní oddělení a sledování prostředků. Další informace získáte v tomto tématu později v části [Konfigurace extranetové adresy URL](https://technet.microsoft.com/88fec9ff-c96c-4d20-8856-0485e7507572).
-   Převzetí úloh správy licencí ze serveru kořenové certifikace. Tím je možné dosáhnout vyššího výkonu v organizacích, které mají jediný server kořenové certifikace (namísto clusteru kořenové certifikace).

Ve většině případů se doporučuje přidat servery RMS do clusteru kořenové certifikace, aby bylo možné nastavit redundanci dat a vyrovnávání zatížení pro všechny nasazené servery. Přesto, že servery správy licencí mohou být také použity ke zpracování požadavků licencování a publikování, nelze je použít k vyrovnávání zatížení clusteru kořenové certifikace. Neexistuje-li konkrétní důvod k nasazení zvláštních serverů správy licencí, je vhodnější vyrovnat zatížení všech serverů RMS tak, že je nastavíte jako členy clusteru kořenové certifikace.

Podrobné pokyny k instalaci a zajištění serveru správy licencí služby RMS naleznete v tomto tématu později v části [Instalace služby RMS s aktualizací Service Pack 1](https://technet.microsoft.com/dab20175-a690-43f8-b943-768d289daa0d) a [Zajištění serveru správy licencí](https://technet.microsoft.com/4d67b898-0ba9-4eef-ab7d-ee0ca55a688e).
