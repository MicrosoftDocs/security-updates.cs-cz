---
TOCTitle: Vyloučení verzí bezpečnostního modulu
Title: Vyloučení verzí bezpečnostního modulu
ms:assetid: 'e287f026-aab2-43ab-93bc-48087da82f36'
ms:contentKeyID: 18113467
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747700(v=WS.10)'
---

Vyloučení verzí bezpečnostního modulu
=====================================

Používání minimální verze klientského softwaru RMS lze v klientech zajistit pomocí verze bezpečnostního modulu, která byla ke klientovi přidružena za účelem vyloučení předchozích verzí klientského softwaru RMS. Pokud tuto funkci povolíte, zadejte poslední minimální verzi bezpečnostního modulu, která byla podepsána službou Microsoft Activation Service. Vyloučení bezpečnostního modulu povolte na webu pro správu každého clusteru, u kterého chcete toto vyloučení nastavit. U všech požadavků správy licencí a certifikace se zjišťuje, zda bezpečnostní modul splňuje kritérium minimální verze.

Pokud je vyloučení založené na verzi bezpečnostního modulu povoleno, nemohou klienti s nižší verzí modulu, než je určená verze, získat certifikáty účtů práv nebo využívat licence k použití, protože jejich požadavky budou zamítnuty. Tito klienti musí nainstalovat novou verzi klientského softwaru RMS, aby získali nový bezpečnostní modul používající aktuální verzi softwaru.

Klient RMS pro aktualizaci Service Pack 1 (SP1) používá verzi bezpečnostního modulu 5.0.0.0 nebo vyšší. Nastavením vyloučení bezpečnostního modulu na tuto minimální verzi vynutíte u klientů RMS organizace, kteří chtějí používat obsah chráněný správou přístupových práv, upgrade na klienta RMS pro aktualizaci SP1.

Pokud byla uživateli, který používá vyloučenou verzi bezpečnostního modulu, dříve vydána licence pro obsah, bude moci nadále tento obsah používat, aniž by musel získávat nový bezpečnostní modul.
