---
TOCTitle: Platforma služby RMS
Title: Platforma služby RMS
ms:assetid: '73b5bfdd-2e30-4310-aff7-a5efc9c4c887'
ms:contentKeyID: 18113378
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747630(v=WS.10)'
---

Platforma služby RMS
====================

Platforma služby RMS se skládá z následujících základních prvků, které umožňují správu práv:

-   **Důvěryhodná entita pro vydání kořenového certifikátu**. Tuto entitu zajišťuje společnost Microsoft. Další informace najdete v této sadě dokumentace v části Hierarchie důvěryhodnosti tématu Technické informace týkající se služby RMS.

-   **RMS**. RMS je serverová technologie pro systém Windows Server 2003, která certifikuje důvěryhodné entity, licencuje informace chráněné službou RMS, zapisuje servery a uživatele a spravuje funkce správy práv. Technologie RMS usnadňuje kroky nastavení, díky kterým mohou důvěryhodné entity používat informace chráněné službou RMS. Pomocí sady SDK Služby správy přístupových práv lze službu RMS rozšířit na podporu dalších funkcí.

-   **Klient Služby správy přístupových práv**. Aby bylo možné nainstalovat a používat aplikace s podporou služby RMS, musí mít uživatelé, kteří jsou v systému služby RMS, klientský počítač, v němž je nainstalován a aktivován klientský software Služby správy přístupových práv v systému Microsoft Windows. Klienta RMS SP1 je možné stáhnout ze serveru Windows Update na [webu společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=18134).

-   **Aplikace s podporou služby RMS**. Tyto aplikace uživatelům umožňují zadat práva využití pro obsah, který vytvoří a distribuují. Aplikace s podporou služby RMS můžete vyvíjet pro systém Microsoft Windows 2000 a vyšší. Existující aplikace můžete rozšířit tak, aby podporovaly službu RMS. Jako příklad aplikace s podporou služby RMS, která byla rozšířena, aby podporovala službu RMS, lze uvést aplikaci Microsoft Internet Explorer. Doplněk Správa práv pro aplikaci Internet Explorer můžete stáhnout z [webu společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=14450). Tento doplněk můžete používat v aplikaci Internet Explorer verze 5.01 nebo vyšší za účelem povolení zobrazování obsahu chráněného službou RMS. Aplikace s podporou služby RMS můžete vyvíjet pomocí sady SDK Služby správy přístupových práv.
