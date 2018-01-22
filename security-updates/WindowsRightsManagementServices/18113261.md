---
TOCTitle: Doporučené postupy správy služby RMS
Title: Doporučené postupy správy služby RMS
ms:assetid: '385f8112-da00-417f-a2b8-42dc1e06b717'
ms:contentKeyID: 18113261
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc720245(v=WS.10)'
---

Doporučené postupy správy služby RMS
====================================

Zvažte následující doporučené postupy pro správu služby RMS.

-   **Nenasazujte na servery RMS žádné další služby.**
    Pokud byste na serverech RMS spouštěli i jiné služby než službu RMS, mohlo by dojít ke konfliktům vedoucím k potížím se zabezpečením. Pomocí čítačů výkonu sledujte, zda nedochází ke snížení výkonu služby nebo ke konfliktům.
-   **Provádějte časté zálohy konfiguračních databází.**
    V konfiguračních databázích jsou uloženy informace důležité pro fungování služby RMS. V konfiguračních databázích clusteru kořenové certifikace jsou navíc uloženy páry klíčů pro celou instalaci. Pokud budete provádět pravidelné zálohy, můžete rychle obnovit fungování služby RMS v případě, že dojde k selhání databázového serveru. Kromě provádění pravidelných záloh byste měli také pravidelně testovat platnost těchto záloh obnovením nanečisto (ve zvláštním testovacím prostředí). Další informace najdete v této sadě dokumentace v části Zálohování a obnovení systému služby RMS tématu Plánování nasazení služby RMS.
-   **Pravidelně databázi protokolování pročišťujte.**
-   **Pomocí správce Microsoft Operations Manager (MOM) server RMR sledujte.**
    Pomocí správce MOM a sady RMS MOM Pack můžete zachycovat kritické události nebo sledovat, zda nedochází ke snížení výkonu, a odesílat oznámení o uvedených událostech.
