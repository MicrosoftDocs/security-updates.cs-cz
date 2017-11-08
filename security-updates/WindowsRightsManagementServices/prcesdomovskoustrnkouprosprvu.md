---
TOCTitle: Práce s domovskou stránkou pro správu
Title: Práce s domovskou stránkou pro správu
ms:assetid: '6c155977-bd0e-47d6-ac65-1746cddb505e'
ms:contentKeyID: 18113311
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc720290(v=WS.10)'
---

Práce s domovskou stránkou pro správu
=====================================

Na webové stránce **Domovská stránka pro správu** můžete zobrazit informace o serveru nebo clusteru a pracovat s možnostmi správy. Tato stránka je k dispozici pouze v případě, že server je zajištěn.

Následujícím postupem můžete k této webové stránce získat přístup ze serveru, který chcete spravovat:

1.  Přihlaste se jako místní správce.
2.  Klepněte na tlačítko **Start**, přejděte na příkaz **Všechny programy**, na položku **Služba RMS v systému Windows** a pak klepněte na položku **Správa služby RMS v systému Windows**.
3.  Na stránce **Globální správa** klepněte na možnost **Spravovat službu RMS na tomto webu**.

Pokud byla povolena vzdálená správa prostřednictvím protokolu SSL (Secure Sockets Layer), lze na stránku **Domovská stránka pro správu** přejít také z jiného počítače provedením následujícího postupu:

1.  Do adresního řádku webového prohlížeče zadejte následující adresu URL:
    https://*název\_clusteru:číslo\_portu*/\_wmcs/admin
    Parametr *název\_clusteru:číslo\_portu* je adresa URL určená pro daný cluster při jeho zajišťování. Číslo portu zadejte pouze v případě, že jste určili jiné nastavení než výchozí port 80.
2.  Po zobrazení výzvy zadejte pověření místního správce na serveru, k němuž přistupujete.

Na stránce **Domovská stránka pro správu** se zobrazí informace o clusteru, například adresa URL clusteru, název a umístění konfigurační databáze, datum vypršení platnosti certifikátu serveru pro poskytování licencí atd. Dále jsou zde zobrazeny odkazy na stránky, na nichž lze pro cluster konfigurovat následující možnosti správy:

-   **Zásady důvěryhodnosti:** Přidání a odebrání důvěryhodných domén. Další informace naleznete v tomto tématu později v části [Správa důvěryhodných domén a zásad důvěryhodnosti](https://technet.microsoft.com/1c96ee74-fd28-4511-be21-087e2b04c3ee).
-   **Šablony zásad práv:** Vytvoření a změna šablon zásad práv. Další informace naleznete v tomto tématu později v části [Správa šablon zásad práv](https://technet.microsoft.com/718286dc-3399-4556-96c9-ec3a33d31877).
-   **Nastavení protokolování:** Zapnutí nebo vypnutí protokolování a zobrazení názvu serveru a databáze protokolování. Další informace získáte v tomto tématu později v části [Správa protokolování](https://technet.microsoft.com/8fccfc57-2135-494e-8e44-f6191bf5e4a0).
-   **Nastavení extranetové adresy URL clusteru:** Určení adresy URL dostupné z externích umístění, která je určena pro požadavky na licence a certifikace účtů. Další informace získáte v tomto tématu později v části [Konfigurace extranetové adresy URL](https://technet.microsoft.com/88fec9ff-c96c-4d20-8856-0485e7507572).
-   **Nastavení serveru proxy služby RMS:** Určení adresy serveru proxy, typu ověřování a uživatelského jména, které má být použito, pokud se server RMS připojuje k Internetu prostřednictvím serveru proxy. Další informace získáte v tomto tématu později v části [Konfigurace nastavení serveru proxy služby RMS](https://technet.microsoft.com/179d2970-62e9-4487-aa5b-f4334234991e).
-   **Nastavení zabezpečení:** Obnovení hesla soukromého klíče, zadání skupiny superuživatelů, kteří mohou dešifrovat veškerý licencovaný obsah, a vyřazení služby RMS z provozu. Další informace naleznete v tomto tématu později v části [Správa zabezpečení při provozu služby RMS](https://technet.microsoft.com/62050812-de4f-4392-8d63-f2f89aa01ed4).
-   **Nastavení certifikace:** Určení doby platnosti certifikátů účtů práv a kontaktu na správce. (Tato možnost je k dispozici pouze na clusteru kořenové certifikace, nikoli na serverech správy licencí.) Další informace naleznete v tomto tématu později v části [Správa certifikátů účtů práv](https://technet.microsoft.com/49c5c2ba-e197-4e4b-b3b3-b3248f068bcc).
-   **Zásady vyloučení:** Určení vyloučení na základě verze bezpečnostního modulu, certifikátu účtu práv, verze systému Windows nebo aplikace s podporou správy přístupových práv. Další informace naleznete v tomto tématu později v části [Správa zásad vyloučení](https://technet.microsoft.com/ee31e099-e095-4648-95da-0009fbeb48cb).
-   **Sestava certifikace účtů RM:** Zobrazení počtu vydaných certifikátů účtů práv. (Tato možnost je k dispozici pouze na clusteru kořenové certifikace, nikoli na serverech správy licencí.) Další informace naleznete v tomto tématu později v části [Sledování certifikátů účtů práv](https://technet.microsoft.com/5bb0f3cf-fc44-4e60-a93f-c789d6f8a902).

Ve zbývajících tématech této části je popsáno, jak s těmito vlastnostmi pracovat. Podrobné pokyny naleznete v tomto tématu později v části [Postupy pro službu RMS...](https://technet.microsoft.com/82032075-f361-438f-a2c4-93ab29ae6cff).

| ![](images/Cc720290.note(WS.10).gif)Poznámka                                                                                                                                                                               |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Ke konfiguraci některých funkcí využívá web pro správu služby RMS překryvná okna. Jestliže u webového prohlížeče používáte blokování překryvných oken, měli byste nastavení prohlížeče nakonfigurovat tak, aby překryvná okna z tohoto webu povolovalo. |
