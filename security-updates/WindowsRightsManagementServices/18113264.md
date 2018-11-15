---
TOCTitle: Využití obsahu chráněného službou RMS
Title: Využití obsahu chráněného službou RMS
ms:assetid: '3cf6d64b-1187-433c-bbb2-c68069bc3c30'
ms:contentKeyID: 18113264
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc720251(v=WS.10)'
---

Využití obsahu chráněného službou RMS
=====================================

Při využití chráněného obsahu uživateli jsou provedeny dva procesy, které jsou pro uživatele transparentní. V prvním případě aplikace s podporou služby RMS požaduje při otevření dokumentu uživatelem licenci k použití. Ve druhém případě uvedená aplikace zjišťuje, zda je licencí k použití vyžadován seznam odvolání, a ověřuje, zda nebyl odvolán žádný certifikát v řetězci důvěryhodnosti ani certifikát účtu práv. Pokud to všechna práva a odvolání umožní, zobrazí aplikace s podporou služby RMS po dokončení obou procesů obsah chráněný touto službou.

Je-li požadován seznam odvolání, aplikace vyhledá místní kopii seznamu odvolání, jejíž doba platnosti nevypršela. V případě potřeby načte aktuální kopii seznamu odvolání. Aplikace poté použije všechny podmínky odvolání, které jsou relevantní v aktuálním kontextu.

Pokud přístup k obsahu není blokován žádnou podmínkou odvolání, aplikace poskytne obsah a uživatel může uplatnit práva, která mu byla udělena.

Službu RMS je možné nakonfigurovat na zpracování požadavků na licence k použití od oprávněných externích uživatelů. Tímto způsobem je uživatelům umožněno sdílet chráněný obsah v síti Internet.

Tento oddíl obsahuje následující témata:

-   [Získání licence k použití](https://technet.microsoft.com/0b6cde34-418a-4dee-9d27-b65b93b535ac)
-   [Licence k použití a externí uživatelé](https://technet.microsoft.com/02db9bda-180e-438f-863d-26252083a471)
