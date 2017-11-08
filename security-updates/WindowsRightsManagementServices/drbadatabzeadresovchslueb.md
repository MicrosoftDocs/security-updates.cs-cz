---
TOCTitle: Údržba databáze adresářových služeb
Title: Údržba databáze adresářových služeb
ms:assetid: '911a62f2-c1d6-4091-99b0-b53211be27a7'
ms:contentKeyID: 18113425
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747680(v=WS.10)'
---

Údržba databáze adresářových služeb
===================================

Součástí služby RMS je databáze adresářových služeb, jejímž hostitelem je váš databázový server. Tato databáze obsahuje informace o uživatelích, identifikátorech (jako jsou například e-mailové adresy), ID zabezpečení (SID), členství ve skupinách a alternativních identifikátorech. Uvedené informace se získávají z dotazů LDAP odesílaných globálnímu katalogu služby Active Directory prostřednictvím služby správy licencí RMS. Potom se v této databázi ukládají v místní mezipaměti, což zkracuje dobu odezvy serveru na požadavky uživatelů na licence k použití.

Vzhledem k tomu, že se data v této databázi často vkládají a odstraňují, může často docházet k jejich fragmentaci. Proto byste měli pravidelně (denně nebo týdně) provádět reorganizaci indexů všech databázových tabulek DRMS\_DirectoryServices. Tímto způsobem vytvoříte indexy znovu a zamezíte fragmentaci dat. Fragmentovaná data mohou být příčinou nízkého výkonu, a dokonce i selhání serveru, jestliže není fragmentace zásahem správce znemožněna.

Pokud jako databázový server používáte SQL Server, můžete reorganizace databáze provádět pomocí průvodce údržbou nebo spuštěním vlastního skriptu prostřednictvím agenta serveru SQL Server.

Jestliže zjistíte, že velikost protokolu transakcí narůstá při vytváření nových indexů do nepřijatelných rozměrů, můžete tento nárůst omezit přepnutím z režimu úplného obnovení do režimu hromadného protokolování ještě před zahájením vytváření nových indexů.
