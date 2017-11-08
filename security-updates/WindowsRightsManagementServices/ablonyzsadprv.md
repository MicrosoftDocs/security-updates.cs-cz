---
TOCTitle: Šablony zásad práv
Title: Šablony zásad práv
ms:assetid: 'eee931c8-7c98-48e9-9e2c-d0b7bd4f2b96'
ms:contentKeyID: 18113500
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747732(v=WS.10)'
---

Šablony zásad práv
==================

Šablony zásad práv popisují standardní sadu uživatelů, práv a podmínek, které lze zadat pro obsah chráněný službou RMS. Pokud uživatel uplatní šablonu zásad práv na část obsahu, práva popsaná v šabloně se stanou součástí licence k publikování. 

Šablony zásad práv je možné vytvářet na webu správy služby RMS, kde také lze odstraňovat nebo měnit existující šablony. Šablony zásad práv mohou obsahovat různé podmínky, jako například konkrétní příjemce nebo skupiny služby Active Directory, dobu platnosti licence k použití pro daný obsah, dobu po publikování, po kterou lze daný obsah využít, a dokonce i vlastní hodnoty s významem pro určitou aplikaci s podporou služby RMS. Některé šablony mohou vyžadovat určení seznamu odvolání. Šablona určuje adresu URL souboru se seznamem a počet dní, po které je seznam platný. Jestliže příjemce na základě dané šablony požádá o licenci k použití, zkontroluje systém seznam odvolání ještě před tím, než uživatel může obsah chráněný službou RMS využít. Další informace získáte v tomto tématu později v části [Odvolání služby RMS](https://technet.microsoft.com/72689f90-f3c5-4b61-94ea-d825f3199b3b).

Jako příklady práv stanovených v šablonách zásad práv lze uvést následující práva:

-   Kdokoli může zobrazit obsah, avšak upravit jej může pouze autor.
-   Obsah může zobrazit kdokoli v daném podniku, avšak pouze po dobu jednoho měsíce po publikování.
-   Obsah může zobrazit kdokoli v daném podniku, avšak nemohou jej zobrazit žádní externí partneři ani klienti.
-   Obsah mohou zobrazit pouze určení příjemci.
-   Obsah může zobrazit a upravit pouze určený příjemce.

Šablony mohou obsahovat různé podmínky, jako jsou například následující:

-   Určení příjemci nebo skupiny Active Directory vybavení právy pro daný obsah.
-   Doba platnosti licence k použití pro daný obsah.
-   Doba po publikování, po kterou je daný obsah možné využívat.
-   Zda licence k použití vyžaduje seznam odvolání a jak často má být tento seznam aktualizován.
-   Vlastní hodnoty, které mají význam pro určitou aplikaci s podporou služby RMS.

Šablony zásad práv jsou ukládány do konfigurační databáze i do sdílené složky. Správce služby RMS je zodpovědný za jejich distribuci ze sdílené složky do klientských počítačů, aby je autoři mohli používat. Další informace najdete v této sadě dokumentace v části Distribuce šablon zásad práv tématu Provoz serveru RMS.

V aplikaci s podporou služby RMS mohou autoři vybrat požadovanou šablonu zásad práv, která obvykle určuje skupinu, jejíž členové mohou příslušný obsah využít. Pokud příjemce požaduje licenci k použití, server použije šablonu zásad práv z databáze. Tímto způsobem je zajištěno, že podmínky licence k použití vždy odrážejí aktuální verzi šablony.
