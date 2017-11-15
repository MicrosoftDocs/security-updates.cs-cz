---
TOCTitle: Práce se stránkou pro globální správu
Title: Práce se stránkou pro globální správu
ms:assetid: '57bbf402-2351-4dee-823c-27f4dd32447c'
ms:contentKeyID: 18113323
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747575(v=WS.10)'
---

Práce se stránkou pro globální správu
=====================================

Na stránce **Globální správa** webu pro správu můžete zajistit server služby RMS nebo jeho zajištění zrušit a změnit účet služby RMS.

Následujícím postupem můžete k této webové stránce získat přístup ze serveru, který chcete spravovat:

1.  Přihlaste se jako místní správce.

2.  Klepněte na tlačítko **Start**, přejděte na příkaz **Všechny programy**, na položku **Služba RMS v systému Windows** a pak klepněte na položku **Správa služby RMS v systému Windows**.

Na stránku **Globální správa** nelze přejít z prohlížeče ve vzdáleném počítači.

Pokud server, z něhož na stránku **Globální správa** přistupujete, nebyl dosud zajištěn, zobrazí se pro každý web spuštěný na serveru následující možnosti:

-   **Zajišťovat službu RMS na tomto webu:** Na tento odkaz klepněte v případě, že se jedná o první server, který chcete v tomto clusteru zajistit. Spustí se proces zajištění, v jehož rámci jsou nainstalovány prostředky služby RMS, například virtuální adresáře. Dále jsou nainstalovány databáze na databázový server. Další informace získáte později v tomto tématu v části [Zajištění prvního serveru kořenové certifikace](https://technet.microsoft.com/debc42f3-74ff-4c99-b7a4-4921fccdabc2).

-   **Přidat tento server do clusteru:** Na tento odkaz klepněte, chcete-li zajistit server a přidat jej do existujícího clusteru. Server můžete přidat do clusteru kořenové certifikace nebo do clusteru správy licencí. Budou nainstalovány prostředky služby RMS, například virtuální adresáře. Databáze však vytvořeny nebudou, protože server bude používat databáze clusteru. Další informace naleznete v tomto tématu později v části [Přidání serveru do clusteru](https://technet.microsoft.com/db635238-5528-4bec-9cc6-8244e2b3d733).

Pokud na stránku **Globální správa** přistupujete ze serveru, který již byl zajištěn, zobrazí se následující možnosti:

-   **Spravovat službu RMS na tomto webu:** Klepnutím na tento odkaz zobrazíte stránku Správa clusteru. Další informace naleznete v tomto tématu později v části [Práce s domovskou stránkou pro správu](https://technet.microsoft.com/6c155977-bd0e-47d6-ac65-1746cddb505e).

-   **Změnit účet služby RMS:** Na tento odkaz klepněte, chcete-li určit jiný účet služby RMS, pod nímž má být tato služba spuštěna. Další informace získáte v tomto tématu později v části [Změna účtu služby RMS](https://technet.microsoft.com/f257d66d-b823-41e4-bcb7-7c90eb295238).

-   **Odebrat službu RMS z tohoto webu:** Na tento odkaz klepněte, chcete-li zrušit zajištění služby RMS. Pokud zrušíte zajištění služby RMS, budou ze serveru odebrány virtuální adresáře a aplikace služby RMS, služba však nebude odinstalována. Další informace získáte v tomto tématu později v části [Odinstalace služby RMS](https://technet.microsoft.com/885e3b4f-ea32-466f-9f7f-d8440b0f7c28).

> [!NOTE]
> Ke konfiguraci některých funkcí využívá web pro správu služby RMS překryvná okna. Jestliže u webového prohlížeče používáte blokování překryvných oken, měli byste nastavení prohlížeče nakonfigurovat tak, aby překryvná okna z tohoto webu povolovalo. 
