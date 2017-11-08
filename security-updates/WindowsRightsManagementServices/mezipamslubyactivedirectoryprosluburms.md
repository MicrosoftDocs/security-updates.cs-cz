---
TOCTitle: Mezipaměť služby Active Directory pro službu RMS
Title: Mezipaměť služby Active Directory pro službu RMS
ms:assetid: 'c721a2eb-2fe9-4346-b426-3cc169b97265'
ms:contentKeyID: 18113432
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747662(v=WS.10)'
---

Mezipaměť služby Active Directory pro službu RMS
================================================

Každý server nebo cluster kořenové certifikace a server správy licencí služby RMS má k dispozici místní mezipaměť služby Active Directory s výsledky vyhledávání členství ve skupinách v globálním katalogu služby Active Directory. Kromě mezipaměti každého serveru je k dispozici také sdílená mezipaměť pro každý cluster uložená v databázi adresářových služeb. Účelem těchto mezipamětí je snížit počet dotazů, které jsou odeslány do globálního katalogu, a zkrátit dobu odezvy pro požadavky správy licencí.

Pokud uživatel vyžádá licenci k použití, odpovídající server musí vyhodnotit, zda má uživateli přidělit nezbytná práva v licenci k publikování nebo zda mají být tato práva odepřena. V nejjednodušším případě je uživatel, který licenci vyžaduje, explicitně uveden v licenci k publikování. V mnoha scénářích však autor místo jednotlivých uživatelů uděluje práva skupině.

Pokud není v licenci k publikování explicitně uveden žádající uživatel, ale práva jsou přidělena celé skupině, musí server vyhodnotit členství uživatele ve skupině a určit, zda uživatel je nebo není členem skupiny, která danými právy disponuje. Toho server docílí odesláním dotazu LDAP globálnímu katalogu.

Servery RMS ukládají všechny výsledky dotazů na členství ve skupinách do místní mezipaměti služby Active Directory i do mezipaměti databáze adresářových služeb clusteru. Servery pak mohou načíst informace o členství ve skupinách z těchto mezipamětí, což snižuje počet dotazů předávaných do globálního katalogu. Ve výchozím nastavení jsou dotazy odesílány na nejbližší server. Můžete však nakonfigurovat klíč registru globálního katalogu tak, že dotazy budou odesílány na servery globálního katalogu. Další informace o uvedeném nastavení získáte v této sadě dokumentace v části Změna nastavení registru fondu připojení tématu Provoz serveru RMS.

Za účelem vyhodnocení členství uživatele ve skupině server nejprve zkontroluje mezipaměť, zda již pro daného uživatele neobsahuje informace o členství ve skupině. Není-li tomu tak, server kontroluje databázi adresářových služeb pro cluster. Nejsou-li v databázi uloženy informace o členství ve skupině, server odešle dotaz globálnímu katalogu.

Pro uživatele a skupiny jsou do mezipaměti ukládány následující atributy služby Active Directory:

-   mail,
-   ProxyAddresses (pouze e-mailové adresy SMTP),
-   objectSID,
-   sidHistory,
-   memberOf (identifikátory GUID skupin, jejichž je uživatel nebo skupina členem).

Položky v mezipaměti služby Active Directory jsou označeny časovým razítkem. Nastavení registru určuje období platnosti položek uložených v mezipaměti a celkový počet položek, které lze do mezipaměti uložit. Uvedené možnosti nastavení ovlivňují výkon serverů. Další informace získáte v této sadě dokumentace v části Změna nastavení mezipaměti služby Active Directory tématu Provoz serveru RMS.
