---
TOCTitle: Dílčí zápis serveru správy licencí
Title: Dílčí zápis serveru správy licencí
ms:assetid: '7bc63397-9186-464c-8824-867038adce9b'
ms:contentKeyID: 18113381
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747640(v=WS.10)'
---

Dílčí zápis serveru správy licencí
==================================

Servery správy licencí jsou automaticky zapsány během zajišťování při procesu označovaném jako dílčí zápis. Jestliže však do clusteru serverů správy licencí přidáte nový server, nebude u něj dílčí zápis explicitně proveden, protože používá certifikát serveru pro poskytování licencí a konfigurační databázi daného clusteru.

Server správy licencí neodešle požadavek na dílčí zápis službě Microsoft Enrollment Services, ale serveru kořenové certifikace. Požadavek na dílčí zápis serveru správy licencí je stejný jako požadavek na zápis serveru kořenové certifikace.

Jakmile server kořenové certifikace obdrží požadavek na dílčí zápis, ověří, zda je správně vytvořen, a vrátí řetězec certifikátů, který obsahuje řetězec certifikátů pro poskytování licencí serveru kořenové certifikace a certifikát podepsaný tímto serverem. Certifikát obsahuje veřejný klíč serveru podepsaný s použitím soukromého klíče serveru kořenové certifikace. Opravňuje server správy licencí k vydávání licencí k použití a licencí k publikování.

Certifikát serveru pro poskytování licencí je platný po dobu jednoho roku. Doba platnosti započíná okamžikem vydání certifikátu. Po uplynutí doby platnosti lze platnost certifikátu obnovit. Certifikáty a licence vydávané serverem jsou platné po dobu sedmi let. Doba platnosti započíná okamžikem vydání certifikátu nebo licence.

Ve výchozím nastavení je služba SubEnrollService.asmx, po níž je požadováno zpracování požadavku na dílčí zápis na serveru kořenové certifikace, konfigurována tak, že je veškerý přístup odmítán. Chcete-li povolit přístup správci služby RMS ještě před zpracováním požadavku, je nutné změnit volitelné seznamy řízení přístupu (DACL).
