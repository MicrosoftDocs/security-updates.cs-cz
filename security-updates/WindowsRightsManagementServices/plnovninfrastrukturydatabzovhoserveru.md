---
TOCTitle: Plánování infrastruktury databázového serveru
Title: Plánování infrastruktury databázového serveru
ms:assetid: 'b12354bd-3143-4d1f-b5aa-450c4550653c'
ms:contentKeyID: 18113475
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747731(v=WS.10)'
---

Plánování infrastruktury databázového serveru
=============================================

Vzhledem k tomu, že služba RMS využívá k podpoře svých operací databáze a uložené procedury, vyžaduje její používání v organizaci vytvoření databázové infrastruktury. Databázový server lze nainstalovat na stejný server jako službu RMS nebo na jiný server. Pokud infrastruktura neobsahuje žádný databázový server pro podporu služby RMS, můžete tuto službu testovat pomocí součásti Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) verze A.

Součást Microsoft SQL Server Desktop Engine je vhodné používat k podpoře databází služby RMS pouze v testovacím prostředí, protože neobsahuje nástroje nezbytné ke komplexnímu provozu a podpoře databáze v rámci celého podniku. Součást MSDE nepodporuje vzdálenou síť, a proto je zároveň nutné nainstalovat ji na stejný server jako službu RMS, přičemž není možné do clusteru služby RMS přidávat další servery RMS. V podmínkách používání součásti Microsoft SQL Server Desktop Engine je navíc uvedeno, že pro obsluhu databáze Microsoft SQL Server Desktop Engine nelze použít klientské nástroje serveru SQL Server. Toto omezení neumožňuje zálohování a obnovování konfigurační databáze služby RMS, prohlížení informací protokolování ani přímou změnu dat uložených v konfigurační databázi.

Jestliže chcete databáze umístit na jiném serveru, než je server s instalací služby RMS, budete k zajištění databázové podpory potřebovat plnohodnotný databázový server, jako je například produkt SQL Server. Účtu služby RMS je nutné udělit příslušná oprávnění ke čtení, zápisu a vytváření databází pro databázový server zajišťující podporu služby RMS.

Ačkoli je služba RMS určena a testována pro databázové servery se serverem SQL Server 2000 a součástí MSDE, přičemž společnost Microsoft nepodporuje používání služby RMS s jinými zprostředkovateli databáze, než je SQL Server 2000 nebo MSDE, lze službu RMS spustit na jiných databázových serverech využívajících rozhraní ADO.NET, která jsou poskytována rozhraním Microsoft .NET Framework. Je proto možné, že jiní výrobci vyvinuli pro službu RMS kompatibilní zprostředkovatele databáze. Se službou RMS lze použít libovolného zprostředkovatele databáze za předpokladu, že odpovídající databázový server splňuje následující kritéria:

-   Databázový server musí být kompatibilní s jazykem Transact-SQL, protože inicializační skripty a uložené procedury služby RMS tento jazyk využívají.
-   Databázový server musí podporovat všechna rozšíření specifická pro Microsoft SQL Server.

Zprostředkovatel databáze musí splňovat následující podmínky:

-   odpovídat na volání oboru názvů System.Data.SqlClient rozhraní .NET Framework,
-   poskytovat odpovídající funkčnost oboru názvů System.Data.SqlClient,
-   používat ověřování systému Windows, nikoli ověřování SQL.

Pokud službu RMS provozujete při jakékoli jiné konfiguraci, obraťte se na příslušného dodavatele databáze nebo poskytovatele řešení, jehož zprostředkovatele databáze ve vlastním nasazení používáte.

> [!CAUTION]
> U všech databází služby RMS je při vytváření jako výchozí nastavena možnost úplného obnovení. Nevytvářejí se však žádné úlohy zálohování protokolu transakcí. Z tohoto důvodu může dojít k zaplnění pevného disku serveru, což může vést k chybě databázového serveru. Úplné obnovení se doporučuje u databáze DRMS\_configuration. Ostatní databáze DRMS mohou být nakonfigurovány na jiný model obnovení, který odpovídá potřebám organizace. 

Tento oddíl se zabývá následujícími tématy:

-   [Odhad růstu databáze](https://technet.microsoft.com/87652cc2-b886-4797-8d40-356669768089)
-   [Údržba databáze adresářových služeb](https://technet.microsoft.com/911a62f2-c1d6-4091-99b0-b53211be27a7)
-   [Údržba databáze protokolování](https://technet.microsoft.com/de55058b-0d1a-4997-8a45-e14678ddd13f)
