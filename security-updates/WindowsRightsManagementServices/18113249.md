---
TOCTitle: Plánování nasazení v doménových strukturách
Title: Plánování nasazení v doménových strukturách
ms:assetid: '2dfb40b7-95b1-4362-b32e-72867544b705'
ms:contentKeyID: 18113249
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc720233(v=WS.10)'
---

Plánování nasazení v doménových strukturách
===========================================

Jestliže službu RMS nasazujete v prostředí s mnoha doménovými strukturami, je nutné určit způsob podpory uživatelů nebo skupin mimo doménovou strukturu, ve které službu RMS nasazujete. S objekty uživatelů nebo skupin z jiných doménových struktur totiž obvykle nejsou spojeny zástupné objekty, které obsahuje doménová struktura s nasazenou službou RMS. Chcete-li pomocí služby RMS omezit oprávnění uživatelů nebo skupin z jiných doménových struktur, je třeba odpovídajícím způsobem nakonfigurovat doménovou strukturu s uvedenou službou tak, aby umožňovala rozšíření skupin mezi doménovými strukturami.

Podporu rozšíření skupin mezi doménovými strukturami je možné u služby RMS implementovat dvěma způsoby:

-   Nasaďte službu RMS v doménové struktuře, ve které jsou definovány požadované skupiny a kde bude využita k rozšíření členství v těchto skupinách.
-   Synchronizujte definice skupin ve všech doménových strukturách. Tento krok umožní instalaci služby RMS správně určit členství každého uživatele v jednotlivých skupinách. Pokud uživatel, který požaduje licenci k použití, využívá účet systému Windows v oddělené doménové struktuře, je nutné v místní doménové struktuře vytvořit zástupný kontaktní objekt také pro členství daného uživatele ve skupinách. Zcela spolehlivou synchronizaci objektů skupin mezi doménovými strukturami lze zajistit pomocí metaadresářů, jako jsou například produkty Microsoft® Identity Integration Server (MIIS) 2003 nebo Identity Integration Feature Pack (IIFP).

Jestliže chcete službu RMS využívat pouze v jedné doménové struktuře, můžete optimalizovat proces vydávání licencí k použití změnou zásady clusteru **MaxCrossForestCalls** v konfigurační databázi služby RMS. Tato zásada určuje maximální počet případů, kdy členství ve skupině může překročit hranice doménové struktury. Výchozí je hodnota 10. Chcete-li ji změnit na hodnotu 0, zadejte následující příkaz SQL:

`update DRMS_ClusterPolicies set PolicyData=0 where PolicyName='MaxCrossForestCalls'`
