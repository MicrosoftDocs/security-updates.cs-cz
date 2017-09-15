---
TOCTitle: Podpora databázového serveru pro službu RMS
Title: Podpora databázového serveru pro službu RMS
ms:assetid: 'c9844783-e6c4-49b4-8e7f-0f0377143b44'
ms:contentKeyID: 18113433
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747664(v=WS.10)'
---

Podpora databázového serveru pro službu RMS
===========================================

Služba RMS používá databázový server, jako je například SQL Server nebo Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) verze A, k provozování svých konfiguračních databází, databází protokolování a databází adresářových služeb. Součást MSDE 2000 lze použít pouze u nasazení s jedním serverem. Ochranu převzetím služeb při selhání umožníte implementací clusteru databázových serverů.

Chcete-li také zajistit podporu požadavků na protokolování, můžete spustit konfigurační databázi a databázi protokolování v samostatných instancích databázového serveru nebo nasadit zvláštní instanci databázového serveru (případně cluster) pro server nebo cluster kořenové certifikace a clustery správy licencí. Další informace o těchto možnostech získáte v této sadě dokumentace v tématu Nasazení systému služby RMS.

Ve výchozím nastavení jsou skupině RMS Service Group udělena oprávnění ke spouštění uložených procedur těchto databází. Uživatelský účet, který byl přihlášen při zajišťování, má k těmto databázím oprávnění vlastníka databází.

| ![](images/Cc747664.note(WS.10).gif)Poznámka                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Součást Microsoft SQL Server Desktop Engine je vhodné používat k podpoře databází služby RMS pouze v testovacím prostředí, protože neobsahuje nástroje nezbytné ke komplexnímu provozu a podpoře databáze v rámci celého podniku. Součást MSDE nepodporuje vzdálenou síť, a proto je zároveň nutné nainstalovat ji na stejný server jako službu RMS, přičemž není možné do clusteru služby RMS přidávat další servery RMS. V podmínkách používání součásti Microsoft SQL Server Desktop Engine je navíc uvedeno, že pro obsluhu databáze Microsoft SQL Server Desktop Engine nelze použít klientské nástroje serveru SQL Server. Toto omezení neumožňuje zálohování a obnovování konfigurační databáze služby RMS, prohlížení informací protokolování ani přímou změnu dat uložených v konfigurační databázi. |
