---
TOCTitle: Databáze protokolování služby RMS
Title: Databáze protokolování služby RMS
ms:assetid: '8ba147f3-16e4-4d9a-ac8f-f05ba2ba11bb'
ms:contentKeyID: 18113419
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747669(v=WS.10)'
---

Databáze protokolování služby RMS
=================================

V instanci databázového serveru, která je zároveň hostitelem konfigurační databáze, instaluje instalační program služby RMS pro každý cluster kořenové certifikace nebo cluster správy licencí databázi protokolování. Instalační program také v rámci služby Řízení fronty zpráv vytváří soukromou frontu zpráv pro protokolování. Služba naslouchání protokolování přenáší data z této fronty zpráv do databáze protokolování.

Skupina RMS Service Group má oprávnění ke spouštění uložených procedur v databázi protokolování.

Služba naslouchání protokolování odesílá do databáze protokolování velké množství dat. Správci proto mohou vytvořit filtry zajišťující, že v databázi protokolování jsou uchovávány pouze informace, které jsou v organizaci zapotřebí.
