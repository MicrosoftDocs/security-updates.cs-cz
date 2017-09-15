---
TOCTitle: Konfigurační databáze služby RMS
Title: Konfigurační databáze služby RMS
ms:assetid: '769adbdc-f32f-464b-85c4-e8b160036187'
ms:contentKeyID: 18113370
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747634(v=WS.10)'
---

Konfigurační databáze služby RMS
================================

Informace o konfiguraci a zásadách ukládá služba RMS na databázovém serveru, jako je například Microsoft® SQL Server nebo Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) verze A. Pro každý server nebo cluster služby RMS je k dispozici jedna konfigurační databáze, která ukládá, sdílí a načítá konfigurační a jiná data.

Konfigurační databáze serveru nebo clusteru kořenové certifikace obsahuje seznam identit uživatelů systému Windows a jejich certifikátů účtů práv. Pár klíčů certifikátu je před uložením do databáze šifrován veřejným klíčem serveru RMS. Konfigurační databáze serverů správy licencí tyto informace neobsahují.

Skupina RMS Service Group má pro uložené procedury databáze oprávnění pro spuštění.

**Důležité: **Součást MSDE 2000 je vhodné používat pouze pro podporu databází služby RMS v testovacích prostředích, protože tato součást nepodporuje žádná síťová rozhraní. V podmínkách používání součásti MSDE 2000 je navíc uvedeno, že pro obsluhu databáze MSDE 2000 nelze použít klientské nástroje serveru SQL Server. Vzhledem k tomuto omezení by nebylo možné zobrazit informace obsažené v protokolech a změnit data uložená v konfigurační databázi.
