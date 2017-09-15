---
TOCTitle: Zápis služby RMS
Title: Zápis služby RMS
ms:assetid: '999db3e1-e3ab-4513-87d9-d584ee334c00'
ms:contentKeyID: 18113442
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747698(v=WS.10)'
---

Zápis služby RMS
================

Při zápisu serveru je vytvořen a předán certifikát serveru pro poskytování licencí. Certifikáty serveru pro poskytování licencí ověřují identitu serverů v daném nasazení a zajišťují ověření pověření během využívání obsahu chráněného službou RMS. První server v každém clusteru správy licencí je zapsán u clusteru kořenové certifikace při procesu zajišťování. Pro následující servery v clusteru není prováděn samostatný zápis.

První server clusteru kořenové certifikace (server kořenové certifikace) musí být zapsán ke službě Microsoft Enrollment Services. Pokud je server kořenové certifikace připojen k Internetu, je možné tento proces provést automaticky jako součást zajišťování. Můžete jej také dokončit offline, jestliže exportujete příslušný požadavek do souboru a soubor odešlete službě Microsoft Enrollment Services z jiného počítače připojeného k Internetu. Požadavek na zápis vrátí certifikát serveru pro poskytování licencí určený pro server kořenové certifikace, který lze pak importovat pomocí webových stránek správy služby RMS.

Požadavek na zápis obsahuje následující informace:

-   Informace o odvolání: Údaje o tom, zda bude instalace služby RMS používat standardní nebo vlastní odvolání (třetích stran). Při použití odvolání třetích stran je součástí těchto informací veřejný klíč odvolacího úřadu.
-   Veřejný klíč certifikátu: Veřejný klíč certifikátu serveru pro poskytování licencí. Tento veřejný klíč je generován na serveru RMS a odeslán službě Microsoft Enrollment Services za účelem získání certifikátu serveru pro poskytování licencí.
-   Skladová položka: Oficiální název skladové položky služby RMS.
-   Verze: Číslo verze sestavení služby RMS.
-   Adresa URL: Základní adresa URL clusteru serverů RMS.

Pokud služba Microsoft Enrollment Services odešle na požadavek na zápis odpověď, vrátí serveru RMS následující informace ve formátu XML:

-   Certifikát serveru pro poskytování licencí:
-   Řetěz certifikátů podepisujících úřadů.

Předané informace se u zápisu serveru kořenové certifikace služby RMS provedeného v režimu online a offline neliší. Ani při jednom z uvedených režimů nedochází ke shromažďování dalších informací.

Informace o jednotlivých krocích zápisu serveru offline získáte v této sadě dokumentace v části Zápis serveru kořenové certifikace v režimu offline tématu Provoz serveru RMS.

Při zápisu klienta je vytvořen a předán klientský certifikát pro poskytování licencí, který autorovi umožňuje publikování obsahu chráněného službou RMS z počítače bez připojení k podnikové síti. Autor může vyžadovat klientský certifikát pro poskytování licencí kdykoli. Zápis klienta není povinný.

Požadavky na zápis jsou protokolovány.

Tento oddíl se zabývá následujícími tématy:

-   [Zápis serveru kořenové certifikace](https://technet.microsoft.com/f08bc919-f090-4843-b2ce-b40d558012ce)
-   [Dílčí zápis serveru správy licencí](https://technet.microsoft.com/7bc63397-9186-464c-8824-867038adce9b)
-   [Zápis klienta RMS](https://technet.microsoft.com/9c1d07bf-7235-4694-8291-ac2e5b221f4a)
-   [Aktivace počítače RMS](https://technet.microsoft.com/09a0d631-9860-477f-9d10-df61b3bfe125)
-   [Certifikace účtů služby RMS](https://technet.microsoft.com/c9a385c5-6dbb-47f5-a80f-69718e6f9deb)
