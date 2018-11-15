---
TOCTitle: Zapnutí a vypnutí protokolování
Title: Zapnutí a vypnutí protokolování
ms:assetid: '8e672f95-566f-4070-9a2a-2f70f087148f'
ms:contentKeyID: 18113422
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747674(v=WS.10)'
---

Zapnutí a vypnutí protokolování
===============================

Provedení tohoto postupu vyžaduje, aby byl uživatel místně přihlášen k webu pro správu v rámci uživatelského účtu, který je členem skupiny Administrators v počítači, k němuž získává přístup. Uvedený postup mohou provést také členové skupiny Domain Admins. Z hlediska zabezpečení je nejvhodnější při provádění tohoto postupu použít příkaz **Spustit jako**.

Chcete-li otevřít webovou stránku **Globální správa**, klepněte na tlačítko **Start**, přejděte na příkaz **Všechny programy**, přejděte na položku **Služba RMS v systému Windows** a klepněte na položku **Správa služby RMS v systému Windows**.

Před zapnutím protokolování zkontrolujte, zda je server RMS připojen k databázovému serveru a zda je spuštěna databázová služba. Pokud služba Řízení front zpráv nemůže předat protokoly do databáze protokolování, bude data zařazovat do fronty na pevném disku serveru RMS. Bude v tom pokračovat tak dlouho, dokud nedojde k zaplnění úložného prostoru serveru. Služba RMS přitom nezobrazí chybu, protože účelem této funkce je podpora protokolování při přerušení spojení se serverem SQL.

Zapnutí a vypnutí protokolování
-------------------------------

#### Zapnutí a vypnutí protokolování

1.  Otevřete stránku **Globální správa** a klepněte na položku **Spravovat službu RMS na tomto webu** u webu, na kterém chcete zapnout nebo vypnout protokolování.

2.  V části **Odkazy správy** klepněte na odkaz **Nastavení protokolování**.

3.  V části **Databáze a server protokolování** zaškrtněte políčko **Zapnout protokolování** a poté klepněte na tlačítko **Aktualizovat**.

    Chcete-li protokolování vypnout, zrušte zaškrtnutí uvedeného políčka a poté klepněte na tlačítko **Aktualizovat**.

Další informace o provádění tohoto postupu naleznete v tomto tématu v části [Zapnutí a vypnutí protokolování](https://technet.microsoft.com/50ccd827-2d39-41e7-a395-3d5f5836869b) uvedené již dříve.
