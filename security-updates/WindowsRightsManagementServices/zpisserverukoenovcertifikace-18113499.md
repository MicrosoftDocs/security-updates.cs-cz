---
TOCTitle: Zápis serveru kořenové certifikace
Title: Zápis serveru kořenové certifikace
ms:assetid: 'f08bc919-f090-4843-b2ce-b40d558012ce'
ms:contentKeyID: 18113499
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747734(v=WS.10)'
---

Zápis serveru kořenové certifikace
==================================

Zápis ke službě Microsoft Enrollment Services je nutný u prvního serveru v nasazení služby RMS. Tento server, který je serverem kořenové certifikace, lze automaticky zapsat během zajišťování, pokud má k dispozici připojení k Internetu. Jestliže tvoří součást uzavřené sítě, může být zapsán ručně. Další informace o ručním zápisu serveru získáte v této sadě dokumentace v části Ruční zápis serveru kořenové certifikace tématu Provoz serveru RMS.

Požadavek na zápis vyžaduje následující vstupní parametry:

-   1024bitový veřejný klíč. Jedná se o veřejný klíč služby RMS.
-   Verze, název a adresa URL serveru služby RMS, který vyžaduje zápis.

Služba Microsoft Enrollment Services používá uvedené údaje pouze při vytvoření certifikátu serveru pro poskytování licencí a ukládá je pouze kvůli případnému odvolání.

Služba Microsoft Enrollment Services vrátí řetěz certifikátů, který obsahuje řetěz certifikátů serveru pro poskytování licencí serveru zápisu, a také certifikát podepsaný serverem zápisu. Certifikát obsahuje veřejný klíč serveru podepsaný soukromým klíčem zápisu a verzi a adresu URL zapsaného serveru. Certifikát uděluje serveru kořenové certifikace právo vydávat certifikáty serveru pro poskytování licencí pro servery správy licencí, certifikáty účtů práv, klientské certifikáty pro poskytování licencí a licence k publikování a k použití.

Certifikát serveru pro poskytování licencí je platný po dobu jednoho roku. Doba platnosti započíná okamžikem vydání certifikátu. Po uplynutí doby platnosti lze platnost certifikátu obnovit. Certifikáty a licence vydávané serverem jsou platné po dobu sedmi let. Doba platnosti započíná okamžikem vydání certifikátu nebo licence.

Údaje o odvolání certifikátu jsou přidány do certifikátu serveru pro poskytování licencí specifikovaného v požadavku na zápis. Veřejný klíč služby Microsoft Enrollment Services je přidán do certifikátu jako klíč odvolání. Pokud je zadán klíč odvolání třetí strany, je také přidán do certifikátu jako klíč odvolání.
