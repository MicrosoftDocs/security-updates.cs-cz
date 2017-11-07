---
TOCTitle: Vyloučení certifikátů účtů práv
Title: Vyloučení certifikátů účtů práv
ms:assetid: 'cba5e901-942c-4d06-9865-e6c4648c95e6'
ms:contentKeyID: 18113438
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747670(v=WS.10)'
---

Vyloučení certifikátů účtů práv
===============================

Pokud je určitý uživatel důvěryhodný, ale jeho pověření RMS byla ohrožena, můžete vyloučit certifikát účtu práv daného uživatele vyloučením jeho veřejného klíče. V takovém případě služba RMS odmítne nové požadavky na licence k použití pro daný certifikát účtu práv. Po vyloučení certifikátu účtu práv bude při příštím pokusu příslušného uživatele o získání licence k použití pro nový obsah jeho požadavek zamítnut. Licenci k použití bude moci získat až po získání nového certifikátu účtu práv s novým párem klíčů.

Certifikáty účtů práv lze vyloučit pomocí stránky **Zásady vyloučení** webu pro správu. Po vyloučení certifikátu účtu práv určitého uživatele přidá služba RMS vyloučený klíč, název uživatelského účtu a datum a čas vyloučení do tabulky DRMS\_GicExclusionList konfigurační databáze clusteru kořenové certifikace. Tyto informace jsou zobrazeny také na stránce **Zásady vyloučení** webu pro správu. Kromě toho služba RMS odstraní z tabulky UD\_Users konfigurační databáze veřejný i soukromý klíč přiřazený vyloučenému certifikátu účtu.

Chcete-li vyloučit certifikát účtu práv na serveru nebo v clusteru kořenové certifikace, určete na stránce **Zásady vyloučení** serveru kořenové certifikace uživatelský účet domény. Certifikát účtu práv by měl být na webu pro správu každého serveru vyloučen u všech serverů s dílčím zápisem. Chcete-li uživatele vyloučit na serveru nebo v clusteru správy licencí s dílčím zápisem, zadejte na stránce **Zásady vyloučení** webu pro správu daného serveru správy licencí hodnotu veřejného klíče certifikátu účtu práv. Tuto hodnotu získáte na stránce **Zásady vyloučení** webu pro správu clusteru kořenové certifikace.

Chcete-li zjednodušit vyloučení certifikátu účtu práv při nasazení služby RMS s více clustery, můžete replikovat tabulku DRMS\_GicExclusionList z konfigurační databáze clusteru kořenové certifikace do konfiguračních databází všech clusterů správy licencí. V takovém případě není třeba na každém serveru ručně zadávat hodnotu veřejného klíče.
