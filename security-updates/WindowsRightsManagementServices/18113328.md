---
TOCTitle: Rozpoznání služby publikování
Title: Rozpoznání služby publikování
ms:assetid: '5d500841-a202-4865-b5d2-d0775d4e1bbc'
ms:contentKeyID: 18113328
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747580(v=WS.10)'
---

Rozpoznání služby publikování
=============================

Služba publikování RMS vydává licence k publikování, které slouží k ochraně obsahu. Vydává také klientské certifikáty pro poskytování licencí, které umožňují uživatelům publikovat obsah v situacích, kdy nejsou připojeni k podnikové síti.

Služba publikování je dostupná z clusteru kořenové certifikace nebo prostřednictvím serverů správy licencí. Aplikace s podporou služby RMS vyžaduje tuto službu v okamžiku, kdy autor publikuje obsah chráněný službou RMS. Aplikace vytvoří požadavek pro službu publikování tak, že z adresáře služby Active Directory nejprve načte požadovanou adresu URL pro virtuální adresář Licensing na serveru, na kterém je služba publikování umístěna. Potom ke službě publikování připojí cestu.

Adresa URL pro virtuální adresář Licensing na serveru je například v adresáři služby Active Directory uložena v následující podobě:

http://*název\_serveru*/\_wmcs/Licensing

Požaduje-li server licenci k publikování, připojí k adrese URL název souboru služby publikování následujícím způsobem:

http://*název\_serveru*/\_wmcs/Licensing/Publish.asmx

Jestliže služba RMS zjistí, že certifikát účtu práv je založen na ověřování uživatelů systému Windows, je umístění služby publikování určeno doménovou strukturou služby Active Directory. To se týká interních i externích uživatelů, kteří se připojují k podnikové síti prostřednictvím virtuální privátní sítě (VPN).

Pokud služba RMS zjistí, že certifikát účtu práv je založen na službě Microsoft® .NET Passport, bude umístění služby publikování představovat účet služby .NET Passport zadaný v obsahu chráněném službou RMS.

> [!NOTE]
> Jestliže jste na serveru povolili protokol SSL, budou tyto adresy URL používat protokol připojení https://. 
