---
TOCTitle: Zadání umístění šablon zásad práv
Title: Zadání umístění šablon zásad práv
ms:assetid: 'e1bee46d-33db-424f-ba45-1dcedcb883ab'
ms:contentKeyID: 18113532
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747781(v=WS.10)'
---

Zadání umístění šablon zásad práv
=================================

Provedení tohoto postupu vyžaduje, aby byl uživatel místně přihlášen k webu pro správu v rámci uživatelského účtu, který je členem skupiny Administrators v počítači, k němuž získává přístup. Uvedený postup mohou provést také členové skupiny Domain Admins. Z hlediska zabezpečení je nejvhodnější při provádění tohoto postupu použít příkaz **Spustit jako**.

Chcete-li otevřít webovou stránku **Globální správa**, klepněte na tlačítko **Start**, přejděte na příkaz **Všechny programy**, přejděte na položku **Služba RMS v systému Windows** a klepněte na položku **Správa služby RMS v systému Windows**.

Jestliže šablony zásad práv uložíte do sdílené složky a potom změníte její umístění, je nutné tyto šablony ručně zkopírovat z původního místa na nové.

Šablony zásad práv se ukládají také do konfigurační databáze. Další informace o distribuci šablon zásad práv naleznete v tomto tématu v části [Distribuce šablon zásad práv](https://technet.microsoft.com/ae6fa26f-d744-4ac9-9eb1-728ffab87bfe) uvedené již dříve.

Používáte-li jako aplikaci s povolenou službou RMS sadu Microsoft Office 2003, je umístění šablon zásad práv řízeno klíčem registru `AdminTemplatePath` a klient RMS se pokusí vyhledat šablony v umístění daném klíčem registru místo v jakémkoli jiném umístění.

Zadání umístění šablon zásad práv
---------------------------------

#### Zadání umístění šablon zásad práv

1.  Otevřete stránku **Globální správa** a klepněte na položku **Spravovat službu RMS na tomto webu** u webu, pro který chcete zadat umístění šablon zásad práv.

2.  V části **Odkazy správy** klepněte na odkaz **Šablony zásad práv**.

3.  V části **Umístění šablony** zadejte název UNC (Universal Naming Convention) sdílené složky, do níž mají být ukládány šablony zásad práv pro tento cluster. Použijte formát \\\\*název\_serveru*\\*název\_sdílené\_složky*. Účet, pod kterým pracuje fond aplikací **správy**, musí mít pro tuto sdílenou složku oprávnění k zápisu. Zajistěte, aby byly šablony uloženy v umístění dostupném v rámci sítě, které vyhovuje požadavkům organizace na zabezpečení. Sdílené složky určené pro ukládání šablon by neměly být vytvářeny v základních složkách využívaných službou RMS, například ve složce Program Files nebo ve složce IISRoot.

4.  Klepněte na tlačítko **Uložit**.

5.  Po vytvoření šablon zásad práv a jejich uložení do definovaného adresáře je třeba zpřístupnit tyto šablony uživatelům. Ve výchozím nastavení hledá klient RMS šablony zásad práv v místním počítači v následujícím adresáři:

    %HOMEPATH%\\Local Settings\\Data aplikací\\Microsoft\\DRM\\templates

    Pro všechny uživatele v dané organizaci, kteří budou využívat službu RMS, je třeba zkopírovat šablony zásad práv z adresáře určeného v kroku 3 do tohoto adresáře.
