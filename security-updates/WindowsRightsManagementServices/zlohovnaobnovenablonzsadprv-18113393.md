---
TOCTitle: Zálohování a obnovení šablon zásad práv
Title: Zálohování a obnovení šablon zásad práv
ms:assetid: 'a6ed3328-4128-45e8-9236-3de484b460de'
ms:contentKeyID: 18113393
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747625(v=WS.10)'
---

Zálohování a obnovení šablon zásad práv
=======================================

Aby byly důležité šablony zásad práv chráněny, pravidelně vytvářejte záložní kopii šablony uložené v konfigurační databázi na médium uložené na zabezpečeném místě. V případě selhání systému je pak možné obnovit šablony zásad práv ze záložní kopie.

Proveďte jednu z následujících akcí:

-   Vytvořte záložní kopii celé konfigurační databáze obsahující údaje o šablonách zásad práv. Další informace týkající se zálohování databáze serveru SQL Server naleznete v dokumentaci k serveru SQL Server.
    -nebo-
-   Vytvořte záložní kopii údajů o šablonách zásad práv uložených v konfigurační databázi. To lze provést exportováním identifikátorů GUID a informací TemplateData z tabulky DRMS\_RightsTemplate do nového textového souboru. Další informace týkající se exportování dat z databáze serveru SQL Server naleznete v dokumentaci k serveru SQL Server.

Pokud je třeba obnovit údaje o šablonách zásad práv v konfigurační databázi, můžete extrahovat identifikátory GUID a informace TemplateData z tabulky DRMS\_RightsTemplate v záložní kopii konfigurační databáze nebo importovat data z textového souboru. Další informace týkající se těchto úloh naleznete v dokumentaci k serveru SQL Server.

| ![](images/Cc747625.note(WS.10).gif)Poznámka             |
|---------------------------------------------------------------------------------------|
| Při plánování zálohování šablon zásad práv se poraďte se správcem serveru SQL Server. |
