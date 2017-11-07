---
TOCTitle: Správa velikosti protokolu
Title: Správa velikosti protokolu
ms:assetid: '431b32b3-02f0-4666-b52c-183eb65154fd'
ms:contentKeyID: 18113289
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc720271(v=WS.10)'
---

Správa velikosti protokolu
==========================

Služba protokolování odesílá velké množství dat do databáze serveru SQL Server. Databázi protokolování pravidelně kontrolujte a ujistěte se, že na disku je dostatek místa pro data. Pokud zjistíte, že množství dat je příliš velké a pro své účely některé informace nepotřebujete, nastavte filtry serveru SQL Server tak, aby byly ukládány pouze protokoly, které jsou třeba. Postup při filtrování informací z protokolů naleznete v nápovědě správce SQL Server Enterprise Manager.

Pokud začne být databáze protokolování příliš velká vzhledem k dostupnému místu na disku, můžete ji přemístit na jiný server podle postupu popsaného v tomto tématu později v části [Přemístění databáze protokolování](https://technet.microsoft.com/34ea8045-dc94-422e-9601-29927cfc1534).

| ![](images/Cc720271.Important(WS.10).gif)Důležité informace                                                                                                                                                                                                                                                     |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Pomocí programu Sledování systému pravidelně sledujte velikost fronty protokolování odchozích zpráv. Pokud velikost fronty výrazně vzroste, ověřte, zda služba naslouchání protokolování pracuje správně. Další informace o použití programu Sledování systému získáte v Centru pro nápovědu a odbornou pomoc k systému Windows Server 2003. |
