---
TOCTitle: Rozpoznání aktivační služby
Title: Rozpoznání aktivační služby
ms:assetid: 'e178d81b-b35c-4958-87ef-e077e2204b32'
ms:contentKeyID: 18113468
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747697(v=WS.10)'
---

Rozpoznání aktivační služby
===========================

Aktivační služba vydává bezpečnostní moduly a certifikáty počítače RMS pro klienty RMS verze 1.0. Je podporována z důvodu zpětné kompatibility se službou RMS verze 1.0. Cluster kořenové certifikace služby RMS poskytuje službu aktivačního serveru proxy, která aktivační službě předává požadavky na aktivaci počítače RMS z klientských počítačů spuštěných v podnikové síti.

Klient RMS verze 1.0 vytvoří požadavek na aktivaci počítače RMS tak, že z adresáře služby Active Directory nejprve načte požadovanou adresu URL pro virtuální adresář Certification serveru kořenové certifikace, na kterém je služba aktivačního serveru proxy umístěna. Poté připojí cestu ke službě aktivačního serveru proxy.

Adresa URL virtuálního adresáře Certification na serveru kořenové certifikace může být ve službě Active Directory uložena například v následující podobě:

http://*název\_serveru*/\_wmcs/Certification

Jakmile klient odesílá požadavek na aktivaci počítače RMS, připojí k adrese URL název souboru služby aktivačního serveru proxy:

http://*název\_serveru*/\_wmcs/Certification/Activation.asmx

Klienti spuštění mimo podnikovou síť vyhledávají aktivační službu pomocí specifikace UDDI pro rozpoznání služby. Další informace získáte v tomto tématu v části [Publikování služeb, jejichž hostitelem je společnost Microsoft](https://technet.microsoft.com/7ee8cb4d-1b46-48be-8a4c-5ff6a458231a) uvedené již dříve.

| ![](images/Cc747697.note(WS.10).gif)Poznámka                                   |
|-------------------------------------------------------------------------------------------------------------|
| Jestliže jste na serveru povolili protokol SSL, budou tyto adresy URL používat protokol připojení https://. |
