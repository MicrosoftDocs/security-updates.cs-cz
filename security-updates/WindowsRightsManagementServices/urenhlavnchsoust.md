---
TOCTitle: Určení hlavních součástí
Title: Určení hlavních součástí
ms:assetid: 'c9ec225b-0e51-42f5-aff6-0aecb62e3b27'
ms:contentKeyID: 18113512
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747751(v=WS.10)'
---

Určení hlavních součástí
========================

Chcete-li stanovit odpovídající topologii, měli byste se seznámit se základními součástmi nasazení služby RMS a funkcemi, které tyto součásti plní. V následujícím seznamu jsou uvedeny servery, které se budou účastnit implementace služby RMS:

-   Servery kořenové certifikace. Server kořenové certifikace představuje první součást nasazení služby RMS. Všechny ostatní součásti jsou na něm závislé. Na serveru kořenové certifikace jsou spuštěny všechny služby RMS, včetně služby certifikace účtů, která zajišťuje certifikáty účtů práv klientům RMS v organizaci. V každé doménové struktuře Active Directory se může nacházet pouze jeden server kořenové certifikace. Do instalace však můžete přidat více serverů a vytvořit tak cluster kořenové certifikace umožňující redundanci dat a vyrovnávání zatížení. Všechny servery, které tvoří součást clusteru kořenové certifikace, používají stejnou konfigurační databázi definovanou při zajišťování prvního serveru certifikace v instalaci.
-   Servery správy licencí. Server správy licencí je nepovinný a není součástí clusteru kořenové certifikace. Jedná se však o server s dílčím zápisem k serveru kořenové certifikace. Server správy licencí je na serveru kořenové certifikace závislý z důvodu certifikace a dalších služeb (nemůže poskytovat služby certifikace účtů), jsou však na něm spuštěny služby správy licencí, takže může poskytovat licence k publikování i k použití. Redundanci dat a vyrovnávání zatížení lze nastavit, jestliže do instalace přidáte více serverů a vytvoříte cluster správy licencí. Všechny servery clusteru správy licencí používají stejnou konfigurační databázi definovanou při zajišťování prvního serveru správy licencí daného clusteru.
-   Servery se součástmi infrastruktury. Nezbytnou infrastrukturu včetně součástí, jako je SQL Server 2000 a služba Active Directory, mohou poskytovat další servery, které se účastní implementace. Implementace těchto součástí a potřebný počet serverů závisí na vašich požadavcích.

Topologie služby RMS, kterou pro organizaci navrhujete, musí zahrnovat nasazení každé z těchto součástí.
