---
TOCTitle: Odhad růstu databáze
Title: Odhad růstu databáze
ms:assetid: '87652cc2-b886-4797-8d40-356669768089'
ms:contentKeyID: 18113349
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747585(v=WS.10)'
---

Odhad růstu databáze
====================

Při odhadování požadované velikosti úložiště databází služby RMS počítejte s minimální kapacitou 10 MB a pak s dalším 1 MB na každých 500 uživatelů konfigurační databáze služby RMS. Databáze protokolování může být umístěna na jiném databázovém serveru než konfigurační databáze.

Jestliže využíváte funkci protokolování služby RMS, je nutné, aby databáze protokolování během počáteční fáze certifikace uživatele, kdy dochází k protokolování mnoha informací, podporovala růst v rozsahu přibližně 1 MB na každého uživatele. Pokud například bude dané nasazení podporovat 1 000 uživatelů, vzroste velikost databáze protokolování po aktivaci a certifikaci každého uživatele pomocí serveru certifikace služby RMS na 1 GB. Při běžném provozu může velikost databáze protokolování vzrůstat o 200 kB na každého uživatele za den (v případě implementace ve fázích se odhaduje další 1 MB na každého nového uživatele přidaného do systému).
