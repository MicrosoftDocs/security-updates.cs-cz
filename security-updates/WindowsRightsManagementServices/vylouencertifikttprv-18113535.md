---
TOCTitle: Vyloučení certifikátů účtů práv
Title: Vyloučení certifikátů účtů práv
ms:assetid: 'e5cd9dec-ac29-437e-8515-dc697ec75edf'
ms:contentKeyID: 18113535
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747785(v=WS.10)'
---

Vyloučení certifikátů účtů práv
===============================

Provedení tohoto postupu vyžaduje, aby byl uživatel místně přihlášen k webu pro správu v rámci uživatelského účtu, který je členem skupiny Administrators v počítači, k němuž získává přístup. Uvedený postup mohou provést také členové skupiny Domain Admins. Z hlediska zabezpečení je nejvhodnější při provádění tohoto postupu použít příkaz **Spustit jako**.

Chcete-li otevřít webovou stránku **Globální správa**, klepněte na tlačítko **Start**, přejděte na příkaz **Všechny programy**, přejděte na položku **Služba RMS v systému Windows** a klepněte na položku **Správa služby RMS v systému Windows**.

Uvedené podmínky jsou vynuceny klientem v době, kdy je licence k použití svázána s chráněným obsahem.

Vyloučení certifikátů účtů práv
-------------------------------

#### Vyloučení certifikátů účtů práv

1.  Otevřete stránku **Globální správa** a klepněte na položku **Spravovat službu RMS na tomto webu** u webu, na kterém chcete vyloučit certifikáty účtů práv.

2.  V části **Odkazy správy** klepněte na odkaz **Zásady vyloučení**.

3.  Klepnutím na možnost **Povolit** v části pro vyloučení certifikátů účtů práv můžete vyloučit certifikát účtu práv uživatele.

4.  Vyberte metodu určení certifikátu účtu, který chcete vyloučit:

    -   Chcete-li vyloučit certifikát účtu podle uživatelského jména, klepněte na pole **Uživatelské jméno** pro certifikát účtu práv, který má být vyloučen, zadejte jméno uživatele, kterého chcete vyloučit (ve tvaru *uživatelské\_jméno*@*název\_domény*.com), a klepněte na tlačítko **Přidat**. Tato možnost slouží k vyloučení certifikátů účtů interních uživatelů, kteří mají uživatelské účty služby Active Directory.
    -   Chcete-li vyloučit certifikát účtu podle veřejného klíče, klepněte na pole **Řetězec veřejného klíče** pro certifikát účtu práv, který má být vyloučen, zadejte řetězec veřejného klíče požadovaného certifikátu účtu práv a poté klepněte na tlačítko **Přidat**. Tato možnost slouží k vyloučení certifikátů externích uživatelů, kteří nemají uživatelské účty služby Active Directory.

    > [!NOTE]
    > Chcete-li odstranit vyloučený certifikát účtu práv ze seznamu vyloučení, klepněte na něj v seznamu a poté klepněte na odkaz **Odstranit vybrané veřejné klíče ze seznamu vyloučení**. Uživatel s daným certifikátem účtu nyní bude moci získat z tohoto serveru licenci pro obsah chráněný správou přístupových práv. 

    > [!NOTE]
    > Chcete-li zakázat vyloučení certifikátů účtů práv, klepněte na možnost **Zakázat**. 

Další informace o tomto postupu naleznete v tomto tématu v části [Vyloučení certifikátů účtů práv](https://technet.microsoft.com/cba5e901-942c-4d06-9865-e6c4648c95e6) uvedené již dříve.
