---
TOCTitle: Definice zásad důvěryhodnosti
Title: Definice zásad důvěryhodnosti
ms:assetid: 'e8d78300-4b26-4f15-9e4f-5ae9eb827ef9'
ms:contentKeyID: 18113485
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747711(v=WS.10)'
---

Definice zásad důvěryhodnosti
=============================

Následujícím postupem můžete definovat důvěryhodné uživatele a domény publikování:

-   **Důvěryhodné domény uživatelů**. Pokud přidáte doménu uživatelů, může služba RMS zpracovávat požadavky na licence k použití od uživatelů, jejichž certifikáty účtů práv byly vydány instalací služby RMS z jiné doménové struktury služby Active Directory, tj. jiného clusteru kořenové certifikace. Důvěryhodnou doménu uživatelů přidáte pomocí importu certifikátu poskytovatele licence serveru instalace, kterou chcete pokládat za důvěryhodnou.
-   **Důvěryhodné domény publikování**. Přidáním domény publikování umožníte, aby jeden server RMS vydával licence k použití na základě licencí k publikování vydaných jiným serverem RMS. Důvěryhodnou doménu publikování přidáte pomocí importu certifikátu poskytovatele licence serveru a soukromého klíče serveru, který chcete pokládat za důvěryhodný.

Další informace naleznete v tomto tématu později v části [Přidání a odebrání důvěryhodných domén uživatelů](https://technet.microsoft.com/7c440b15-01c4-49f1-b43c-00f67f3388c1) a [Přidání a odebrání důvěryhodných domén publikování](https://technet.microsoft.com/d87b502d-5497-4ccd-badf-f6807d587cee). Podrobné pokyny naleznete v tomto tématu později v části [Vytvoření zásad důvěryhodnosti](https://technet.microsoft.com/6c2be3c2-1837-4de4-a72e-3ba3eec3321d).
