---
TOCTitle: 'Odebrání webové služby (zrušení zajištění služby RMS)'
Title: 'Odebrání webové služby (zrušení zajištění služby RMS)'
ms:assetid: '68b4e2b0-b1b7-4b0a-8c1a-82ac27c1f12e'
ms:contentKeyID: 18113348
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747602(v=WS.10)'
---

Odebrání webové služby (zrušení zajištění služby RMS)
=====================================================

Po vyřazení serveru RMS z provozu a odstranění veškeré ochrany služby RMS lze webovou službu odebrat pomocí následujících kroků:

-   Na stránce **Globální správa** vyberte možnost **Odebrat službu RMS z tohoto webu**.

Další krok závisí na typu odebíraného serveru, přestože ve všech případech bude server RMS odebrán ze služby IIS.

-   Pokud je server součástí clusteru (a nejedná se o poslední server v clusteru), není třeba provádět žádné další kroky.
-   Jestliže je server pouze serverem správy licencí, odeberte databázi adresářových služeb, ale ponechejte konfigurační databázi a databázi protokolování (ty používá server certifikace, který je stále v provozu).
-   Pokud je server posledním serverem RMS v organizaci, ponechejte konfigurační databázi a databázi protokolování, ale odeberte spojovací bod služby ve službě Active Directory.
