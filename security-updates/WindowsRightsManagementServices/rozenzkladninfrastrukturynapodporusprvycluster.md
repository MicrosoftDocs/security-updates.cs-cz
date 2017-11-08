---
TOCTitle: Rozšíření základní infrastruktury na podporu správy clusterů
Title: Rozšíření základní infrastruktury na podporu správy clusterů
ms:assetid: '78f0f2f0-a075-409c-9f46-26eb62d1d05b'
ms:contentKeyID: 18113335
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747567(v=WS.10)'
---

Rozšíření základní infrastruktury na podporu správy clusterů
============================================================

Implementujete-li clustery v rámci rozsáhlého nasazení, zajistěte, aby byla infrastruktura nastavena na podporu požadavků vytváření clusterů. Plány nasazení by měly obsahovat následující položky.

Registrace DNS
--------------

Zajistěte, aby každá registrace DNS umožňující používání virtuální adresy IP v extranetu zároveň umožňovala její používání v intranetu.

Pokud registrace DNS není provedena pro síť intranet, nezdaří se požadavky na licence interních klientů. Jestliže nemůžete upravit nastavení DNS, lze upravit tabulky hostitelů jednotlivých serverů v clusteru tak, aby byla adresa URL clusteru namapována na virtuální adresu IP clusteru. Registraci DNS je třeba provést ještě před zajištěním služby. Pokud bylo zajištění provedeno, je nutné odebrat službu RMS ze serveru a opakovat proces zajištění.

Vyrovnávání zatížení
--------------------

Nastavte požadovaný hardware a software pro nasazení serverů s vyrovnáváním zatížení, služby Vyrovnávání zatížení sítě nebo vyrovnávání zatížení pomocí hardwarového řešení, které umožňují distribuci požadavků v rámci clusteru.
