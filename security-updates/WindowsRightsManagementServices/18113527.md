---
TOCTitle: Vyřazení služby RMS z provozu
Title: Vyřazení služby RMS z provozu
ms:assetid: 'dbcacce7-434d-48a7-a11d-ef9690d78b44'
ms:contentKeyID: 18113527
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747767(v=WS.10)'
---

Vyřazení služby RMS z provozu
=============================

Pojem vyřazení z provozu označuje celý proces odebírání serveru RMS a souvisejících databází z organizace. Tímto způsobem lze server RMS odebrat z infrastruktury bez ztráty přístupu k informacím chráněných službou RMS. Následují možné důvody, proč organizace může potřebovat odebrat server RMS ze své infrastruktury:

-   migrace serveru RMS ze zkušebního pilotního prostředí do provozního prostředí,
-   zjednodušení architektury odebráním serverů správy licencí a jejich konsolidací do kořenového clusteru služby RMS,
-   sloučení serverů RMS (například v důsledku slučování společností či akvizicí) integrací dvou infrastruktur RMS do jedné,
-   rozhodnutí přestat používat ochranu obsahu pomocí služby RMS.

Vzhledem k tomu, že je aktivní server RMS integrován s databázovým serverem i se službou Active Directory a ponechává velkou část obsahu chráněnou klíčem obsaženým na serveru RMS, vyžaduje odebrání serveru RMS z organizace více kroků než jen odebrání programu ze serveru. V této části najdete popis uvedených kroků, takže v případě potřeby můžete server RMS vyřadit z provozu.

Tento oddíl se zabývá následujícími tématy:

-   [Princip procesu vyřazení z provozu](https://technet.microsoft.com/57bd9949-9433-437b-93ed-ffb2dff9992e)
-   [Povolení služby vyřazení z provozu](https://technet.microsoft.com/45226e85-b50d-41cc-aca7-0f603f8509d5)
-   [Nastavení oprávnění k virtuálním adresářům](https://technet.microsoft.com/45112111-9608-45b1-9a86-7b313d0a1579)
-   [Odebrání ochrany služby RMS z obsahu](https://technet.microsoft.com/c30361e3-50d2-4474-a87d-d38de502cf9e)
-   [Odebrání webové služby (zrušení zajištění služby RMS)](https://technet.microsoft.com/68b4e2b0-b1b7-4b0a-8c1a-82ac27c1f12e)
-   [Odebrání programových souborů služby RMS](https://technet.microsoft.com/d1dc8a8b-f8de-487f-87b4-2174d449f0bc)
-   [Alternativy k vyřazení serverů RMS z provozu](https://technet.microsoft.com/4d32f35e-997d-4d10-ab66-efe217e853f7)
