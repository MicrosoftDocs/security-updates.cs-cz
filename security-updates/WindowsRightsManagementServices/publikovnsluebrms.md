---
TOCTitle: Publikování služeb RMS
Title: Publikování služeb RMS
ms:assetid: '3cca9325-6bd3-49ad-aa3f-e0693205d3f4'
ms:contentKeyID: 18113241
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc720247(v=WS.10)'
---

Publikování služeb RMS
======================

Adresy URL služeb RMS jsou publikovány ve službě Active Directory během zajišťování serveru. Instalační program služby RMS odešle během zajišťování službě Active Directory dotaz a zjišťuje, zda byly v dané doménové struktuře nainstalovány další servery RMS. Jestliže žádné další servery RMS nainstalovány nebyly, nakonfiguruje instalační program služby RMS daný server jako server kořenové certifikace. Před použitím služby RMS je nutné ve službě Active Directory zaregistrovat spojovací bod služby a umožnit tak klientům zjistit adresu URL serveru kořenové certifikace. Klienti požadující spojení se službami spuštěnými na serveru kořenové certifikace zahajují hledání dotazem na adresu URL tohoto serveru kořenové certifikace odeslaným službě Active Directory. Další informace získáte v této sadě dokumentace v části Registrace spojovacího bodu služby tématu Provoz serveru RMS.

| ![](images/Cc720247.note(WS.10).gif)Poznámka                                                                                                                                         |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Pokud daná topologie obsahuje v clusteru serveru kořenové certifikace více serverů, adresa URL odkazuje na server pro vyrovnávání zatížení pro tento cluster, který byl určen správcem během procesu zajišťování. |
