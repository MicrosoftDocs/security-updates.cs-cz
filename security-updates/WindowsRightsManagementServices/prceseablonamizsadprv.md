---
TOCTitle: Práce se šablonami zásad práv
Title: Práce se šablonami zásad práv
ms:assetid: 'ff4f1143-f6b9-4dd8-aa4c-c2cbbf6fdf06'
ms:contentKeyID: 18113552
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747804(v=WS.10)'
---

Práce se šablonami zásad práv
=============================

Po vytvoření šablony zásad práv můžete prostřednictvím řízení její distribuce autorům určit způsob, jakým je v organizaci použita.

Šablony zásad práv jsou ve službě RMS uloženy v konfigurační databázi. Kromě toho je kopie všech šablon zásad práv uložena v zadané sdílené složce, jak je popsáno v tomto tématu později v části [Zadání umístění šablon zásad práv](https://technet.microsoft.com/e1bee46d-33db-424f-ba45-1dcedcb883ab). Zajistěte, aby byly šablony uloženy v umístění dostupném v rámci sítě, které vyhovuje požadavkům organizace na zabezpečení. Sdílené složky určené pro ukládání šablon by neměly být vytvářeny v základních složkách využívaných službou RMS, například ve složce Program Files nebo ve složce IISRoot.

Při publikování chráněného obsahu autor vybírá šablonu zásad práv ze šablon, které jsou k dispozici v místním počítači. Šablony je možné používat pouze v případě, že je správce nainstaluje ze sdílené složky do počítačů uživatelů.

Pokud se uživatel pokusí pracovat s chráněným obsahem, získá aplikace s podporou správy přístupových práv z konfigurační databáze poslední verzi šablony zásad práv použité při publikaci daného obsahu. Aplikace pak uplatní nastavení šablony na obsah. Pokud upravíte šablonu zásad práv na serveru RMS, aktualizuje služba RMS šablonu v konfigurační databázi a ve sdílené složce (pokud je server RMS konfigurován k zadání umístění souboru pro ukládání kopií šablon zásad práv). Při změně šablony zásad práv je vhodné ji znovu nasadit do klientských systémů, aby uživatelé měli v počítačích k dispozici její aktuální verzi.

Pokud je šablona zásad práv odstraněna, je odebrána z konfigurační databáze a také z umístění sdílené složky (která je zadána jako umístění souborů pro ukládání kopií šablon). Není však odstraněna z počítačů uživatelů. Z těchto počítačů je třeba šablonu odstranit ručně. Odstraněná šablona zásad práv by měla být odebrána ze všech počítačů uživatelů. Jestliže uvedený krok neprovedete a odstraněná šablona zásad práv bude použita k publikování obsahu, nebude služba RMS moci vydat pro daný obsah žádnou licenci k použití, protože určenou šablonu nebude možné vyhledat v konfigurační databázi.

Při práci se šablonami zásad práv lze provádět následující úlohy:

-   **Určení sdílené složky:** Před vytvořením první šablony zásad práv je třeba určit sdílenou složku, ve které budou všechny šablony zásad práv uloženy. Další informace získáte v tomto tématu později v části [Zadání umístění šablon zásad práv](https://technet.microsoft.com/e1bee46d-33db-424f-ba45-1dcedcb883ab).

-   **Vytvoření a úprava šablon zásad práv:** Můžete vytvořit tolik šablon zásad práv, kolik vyžaduje správa práv v organizaci. Při vytvoření šablon zásad práv jsou definováni uživatelé a práva, na něž se šablona vztahuje. Dále je definován způsob, jakým má být šablona použita u obsahu. V případě potřeby aktualizace lze šablony zásad práv později upravit. Další informace získáte v tomto tématu později v části [Vytvoření a změna šablon zásad práv](https://technet.microsoft.com/6014176f-ef71-4d29-b3e3-da129c18563d).

-   **Distribuce šablon zásad práv:** Aby mohl autor danou šablonu zásad práv použít na obsah, musí být v jeho počítači uložena kopie této šablony. Prostřednictvím správy distribuce šablon lze řídit, kteří autoři budou používat konkrétní šablony zásad práv. Další informace získáte v tomto tématu později v části [Distribuce šablon zásad práv](https://technet.microsoft.com/ae6fa26f-d744-4ac9-9eb1-728ffab87bfe).

-   **Vyřazení šablon zásad práv:** Pokud šablona zásad práv není nadále vyhovující, může být odstraněna. V takovém případě by šablona měla být odstraněna také z počítačů uživatelů, aby bylo zabráněno potížím, které by měli uživatelé při pokusu o práci s obsahem publikovaným pomocí vyřazené šablony zásad práv. Další informace získáte v tomto tématu později v části [Vyřazení šablon zásad práv](https://technet.microsoft.com/32bf98c7-edda-4507-a4b8-4c11bddd6e60).
