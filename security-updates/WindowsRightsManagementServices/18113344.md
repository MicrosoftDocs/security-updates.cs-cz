---
TOCTitle: Zabezpečení serverů RMS
Title: Zabezpečení serverů RMS
ms:assetid: '7e6c4d3a-6cfb-4e96-9dda-ead83f961a6e'
ms:contentKeyID: 18113344
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747574(v=WS.10)'
---

Zabezpečení serverů RMS
=======================

Pomocí následujících doporučených postupů můžete na serverech RMS spravovat uživatelské účty a nastavení zabezpečení:

-   Virtuální adresáře webu používané ke správě služby RMS obsahují volitelné seznamy řízení přístupu (DACL), které umožňují přístup pouze místním správcům. Místní správce může na webových stránkách pro správu vytvořit další skupinu zabezpečení a řídit přístup přidáváním nebo odebíráním členů této skupiny a nastavením dalších položek řízení přístupu (ACE).

-   Vyššího zabezpečení dosáhnete změnou nastavení seznamů DACL pro webovou stránku Nastavení zabezpečení (SecurityPolicy.aspx). Zajištění je povoleno v případě, že výchozí položka řízení přístupu udělí účtu, který zajišťuje službu RMS, oprávnění k úplnému řízení. Po provedení zajištění by měla být položka řízení přístupu změněna na jednotlivého uživatele nebo na omezenou skupinu zabezpečení.

-   Kromě oprávnění a přístupových práv na jednotlivých serverech RMS věnujte pozornost také zabezpečení konfigurační databáze, které je klíčové pro zabezpečení celého nasazení. Další informace naleznete v tomto tématu později v části [Zabezpečení konfigurační databáze](https://technet.microsoft.com/e023b96f-81d0-45fb-8cc5-becaf6d47ae1).

Další informace týkající se postupu při zabezpečování serveru Microsoft SQL Server™ naleznete na webové stránce **SQL Server Security (Zabezpečení serveru SQL)**, která je k dispozici na [webu společnosti Microsoft](http://www.microsoft.com/) (http://www.microsoft.com/).

Další informace týkající se postupu při zabezpečování počítačů, v nichž je spuštěn některý z operačních systémů řady Microsoft Windows Server 2003, naleznete v příručce Windows Server 2003 Security Guide (Příručka zabezpečení systému Windows Server 2003), kterou je možné získat v centru pro stahování Microsoft Download Center na [webu společnosti Microsoft](http://www.microsoft.com/) (http://www.microsoft.com/).
