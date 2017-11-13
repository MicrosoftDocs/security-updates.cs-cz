---
TOCTitle: Rozpoznání služby správy licencí
Title: Rozpoznání služby správy licencí
ms:assetid: '4eabbb76-b359-443a-b737-098c5659e9c6'
ms:contentKeyID: 18113269
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc720269(v=WS.10)'
---

Rozpoznání služby správy licencí
================================

Služba správy licencí RMS vydává licence k použití, které ověřeným uživatelům umožňují využívat chráněný obsah.

Tato služba je spuštěna v clusterech nebo na serverech kořenové certifikace a na serverech správy licencí. Při vytváření žádosti o licenci k použití klient nejprve ze služby Active Directory načte adresu URL virtuálního adresáře Licensing clusteru kořenové certifikace, kde je umístěna služba správy licencí. Poté aplikace připojí cestu ke službě správy licencí.

Adresa URL virtuálního adresáře Licensing clusteru kořenové certifikace může být ve službě Active Directory uložena například v následující podobě:

http://*název\_serveru*/\_wmcs/Licensing

Požaduje-li server licenci k použití, připojí k adrese URL název souboru služby správy licencí následujícím způsobem:

http://*název\_serveru*/\_wmcs/Licensing/License.asmx

Umístění služby představuje server RMS nebo účet služby .NET Passport, který vydal licenci k publikování. Příslušnou adresu URL obsahuje daná licence k publikování.

> [!NOTE]
> Jestliže jste na serveru povolili protokol SSL, budou tyto adresy URL používat protokol připojení https://. 
