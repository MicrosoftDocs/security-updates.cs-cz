---
TOCTitle: Export důvěryhodné domény uživatelů
Title: Export důvěryhodné domény uživatelů
ms:assetid: '40281ba3-2674-43ca-aa6d-1deb9302eb0e'
ms:contentKeyID: 18113293
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc720259(v=WS.10)'
---

Export důvěryhodné domény uživatelů
===================================

Provedení tohoto postupu vyžaduje, aby byl uživatel místně přihlášen k webu pro správu v rámci uživatelského účtu, který je členem skupiny Administrators v počítači, k němuž získává přístup. Uvedený postup mohou provést také členové skupiny Domain Admins. Z hlediska zabezpečení je nejvhodnější při provádění tohoto postupu použít příkaz **Spustit jako**.

Chcete-li otevřít webovou stránku **Globální správa**, klepněte na tlačítko **Start**, přejděte na příkaz **Všechny programy**, přejděte na položku **Služba RMS v systému Windows** a klepněte na položku **Správa služby RMS v systému Windows**.

Důvěryhodné domény uživatelů umožňují, aby server RMS poskytoval licence uživatelům, jejichž certifikáty účtů práv byly uděleny jiným serverem RMS.

Export důvěryhodné domény uživatelů
-----------------------------------

#### Export důvěryhodné domény uživatelů

1.  Na stránce **Zásady důvěryhodnosti** klepněte v části **Důvěryhodné domény uživatelů** na tlačítko **Exportovat**.

2.  Zobrazí se dialogové okno **Stažení souboru**. Klepněte na tlačítko **Uložit**.

3.  Zobrazí se dialogové okno **Uložit jako**. Doporučujeme upravit název souboru BIN tak, aby obsahoval název příslušného serveru, například RMS\_Server1\_PoskytovLic.bin.

    Soubor je ve výchozím nastavení uložen na plochu. V případě potřeby můžete zadat jiné umístění.

4.  Klepnutím na tlačítko **Uložit** uložte soubor do určeného umístění.

Další informace o provádění tohoto postupu naleznete v tomto tématu v části [Přidání a odebrání důvěryhodných domén uživatelů](https://technet.microsoft.com/7c440b15-01c4-49f1-b43c-00f67f3388c1)uvedené již dříve.
