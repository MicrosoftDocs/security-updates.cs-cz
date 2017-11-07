---
TOCTitle: Podpora služby Active Directory pro službu RMS
Title: Podpora služby Active Directory pro službu RMS
ms:assetid: '9589127d-19b3-44f1-b7a1-01992e78218a'
ms:contentKeyID: 18113372
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747604(v=WS.10)'
---

Podpora služby Active Directory pro službu RMS
==============================================

Služba RMS využívá službu Active Directory k následujícím účelům:

-   **Ověřování uživatelů:** Služba Active Directory poskytuje adresářové služby, pomocí nichž lze ověřovat uživatele služby RMS. Další informace o ověřování a službě RMS získáte v tomto tématu později v části [Model zabezpečení služby RMS](https://technet.microsoft.com/665db831-366d-4dca-9bb3-cc2912481fe1).
-   **Rozpoznání členství ve skupinách a identit účtů jednotlivých uživatelů:** Služba Active Directory poskytuje informace o členství ve skupinách, na jejichž základě služba RMS uděluje licence k použití pro obsah chráněný touto službou v případě, že licence k publikování neuděluje práva účtům jednotlivých uživatelů, ale skupinám. Z důvodu omezení počtu dotazů LDAP odesílaných službě Active Directory ukládá služba RMS informace získané z místní mezipaměti do své mezipaměti a také do centralizované databáze adresářových služeb. Další informace získáte v tomto tématu v částech [Mezipaměť služby Active Directory pro službu RMS](https://technet.microsoft.com/c721a2eb-2fe9-4346-b426-3cc169b97265) a [Databáze adresářových služeb RMS](https://technet.microsoft.com/6f6b8586-5d17-4a40-94a3-4dc738195301) uvedených již dříve
-   **Uložení umístnění služby RMS pro rozpoznání:** Požadavky služby (například požadavky na licenci k použití, licenci k publikování nebo dílčí zápis serveru správy licencí) je nutné odeslat na adresu URL spustitelného modulu webové služby, která daný požadavek zajišťuje. Všechny požadavky služby začínají dotazem Active Directory na adresu URL serverové webové služby (Server.asmx), která dále poskytuje příslušnou adresu URL pro požadavek služby. Další informace získáte v tomto tématu později v části [Publikování a rozpoznání služby RMS](https://technet.microsoft.com/336c0d55-fd7f-4aa9-b3e6-bfd6565b1086).
