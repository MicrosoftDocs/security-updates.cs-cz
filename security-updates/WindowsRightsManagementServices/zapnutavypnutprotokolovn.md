---
TOCTitle: Zapnutí a vypnutí protokolování
Title: Zapnutí a vypnutí protokolování
ms:assetid: '50ccd827-2d39-41e7-a395-3d5f5836869b'
ms:contentKeyID: 18113325
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747565(v=WS.10)'
---

Zapnutí a vypnutí protokolování
===============================

Protokolování pro aktuální cluster nebo server lze zapnout nebo vypnout na stránce **Nastavení protokolování**. Po vypnutí protokolování přestanou webové služby RMS odesílat zaznamenané údaje do fronty zpráv protokolování. Dále je zastavena služba naslouchání protokolování. Vypnutí protokolování pomocí nástroje pro správu služeb systému Windows Server 2003 není podporováno.

Protokoly služby RMS jsou odesílány do databázového serveru službou Řízení front zpráv. Pokud není k dispozici připojení k databázovému serveru, bude služba Řízení front zpráv ukládat protokoly do místní mezipaměti, dokud nebude připojení obnoveno. Před povolením protokolování zkontrolujte, zda je server RMS připojen k databázovému serveru a zda je spuštěna databázová služba. Pokud jako databázový server používáte SQL Server, můžete pomocí následujícího postupu zjistit, zda jsou protokoly zapisovány do databáze:

-   Ve správci SQL Server Enterprise Manager přejděte k databázi protokolování, rozbalte položku **Databases** (Databáze) a poté rozbalte databázi obsahující databázi protokolování služby RMS.
-   Klepněte na databázi protokolování, vyberte položku **Tables** (Tabulky), pravým tlačítkem myši klepněte na položku **DRMS\_log\_master** a poté klepněte na možnost **Open table - return all rows** (Otevřít tabulku – vrátit všechny řádky). Pokud jsou vytvářeny soubory protokolů, zobrazí se jeden nebo více těchto souborů.
