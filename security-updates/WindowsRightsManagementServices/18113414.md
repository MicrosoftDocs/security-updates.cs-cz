---
TOCTitle: Odstranění uživatelských účtů
Title: Odstranění uživatelských účtů
ms:assetid: 'bf73b141-d4d1-4807-a773-3aaff58b0db6'
ms:contentKeyID: 18113414
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747653(v=WS.10)'
---

Odstranění uživatelských účtů
=============================

Odstraníte-li ze služby Active Directory uživatelský účet, nebude automaticky odstraněna položka certifikátu účtu práv daného uživatele uložená v tabulce uživatelských klíčů konfigurační databáze clusteru kořenové certifikace. Vzhledem k tomu může tabulka klíčů neomezeně narůstat, protože jsou do ní neustále přidáváni noví uživatelé, ale staří uživatelé nejsou odstraňováni.

Údržbu konfigurační databáze lze provádět spuštěním uložené procedury, která odstraňuje klíče uživatelů na základě jejich identifikátorů zabezpečení (SID) vždy, když je související uživatelský účet odebrán ze služby Active Directory. Případně je možné pravidelně spouštět skript, který z konfigurační databáze odstraní všechny klíče uživatelů, pro něž ve službě Active Directory neexistuje přidružený identifikátor SID. Touto operací je však značně zvýšeno zatížení serveru SQL Server i služby Active Directory.
