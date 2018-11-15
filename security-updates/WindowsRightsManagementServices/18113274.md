---
TOCTitle: Vyloučení verzí bezpečnostního modulu
Title: Vyloučení verzí bezpečnostního modulu
ms:assetid: '515e5245-7a0e-414e-ac20-3ae32898179e'
ms:contentKeyID: 18113274
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc720270(v=WS.10)'
---

Vyloučení verzí bezpečnostního modulu
=====================================

Provedení tohoto postupu vyžaduje, aby byl uživatel místně přihlášen k webu pro správu v rámci uživatelského účtu, který je členem skupiny Administrators v počítači, k němuž získává přístup. Uvedený postup mohou provést také členové skupiny Domain Admins. Z hlediska zabezpečení je nejvhodnější při provádění tohoto postupu použít příkaz **Spustit jako**.

Chcete-li otevřít webovou stránku **Globální správa**, klepněte na tlačítko **Start**, přejděte na příkaz **Všechny programy**, přejděte na položku **Služba RMS v systému Windows** a klepněte na položku **Správa služby RMS v systému Windows**.

Podmínky vyloučení jsou vynuceny klientem v době, kdy je licence k použití svázána s chráněným obsahem.

Vyloučení verzí bezpečnostního modulu
-------------------------------------

#### Vyloučení verzí bezpečnostního modulu

1.  Otevřete stránku **Globální správa** a klepněte na položku **Spravovat službu RMS na tomto webu** u webu, na kterém chcete vyloučit verze bezpečnostního modulu.

2.  V části **Odkazy správy** klepněte na odkaz **Zásady vyloučení**.

3.  Klepnutím na možnost **Povolit** v části **Vyloučení bezpečnostního modulu RM** je možné vyloučit verze bezpečnostního modulu.

4.  Klepnutím na tlačítko **Získat verzi** se připojíte k Internetu a zobrazíte minimální verzi bezpečnostního modulu, která byla podepsána službou Microsoft Activation Service. Pokud na serveru RMS není k dispozici připojení k Internetu, můžete přejít přímo na [web služby Activation Service pro službu RMS](http://go.microsoft.com/fwlink/?linkid=12995) (http://go.microsoft.com/fwlink/?LinkID=12995), na kterém zobrazíte minimální verzi bezpečnostního modulu.

5.  Na zobrazené stránce **Aktuální minimální verze bezpečnostního modulu RM** zkopírujte číslo verze a poté klepněte na tlačítko **Zavřít**.

6.  Vložte číslo verze do pole **Minimální požadovaná verze bezpečnostního modulu RM** a pak klepněte na tlačítko **Aktualizovat**.

    > [!NOTE]
    > Chcete-li vypnout vyloučení založené na verzi bezpečnostního modulu, klepněte na možnost **Zakázat**. 

Další informace o tomto postupu naleznete v tomto tématu v části [Vyloučení verzí bezpečnostního modulu](https://technet.microsoft.com/e287f026-aab2-43ab-93bc-48087da82f36) uvedené již dříve.
