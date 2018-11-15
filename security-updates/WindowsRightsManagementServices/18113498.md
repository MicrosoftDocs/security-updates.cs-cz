---
TOCTitle: Správa zásad vyloučení
Title: Správa zásad vyloučení
ms:assetid: 'ee31e099-e095-4648-95da-0009fbeb48cb'
ms:contentKeyID: 18113498
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747730(v=WS.10)'
---

Správa zásad vyloučení
======================

Na straně serveru můžete implementovat zásady vyloučení a tímto způsobem odmítnout požadavky na licenci nebo certifikát založené na certifikátu účtu práv nebo verzi bezpečnostního modulu. Na základě zásad vyloučení jsou zamítnuty požadavky licencování nebo certifikaci, které jsou provedeny ohroženými zaregistrovanými objekty zabezpečení, ale na rozdíl od odvolání nezpůsobí zásady vyloučení zrušení platnosti těchto objektů. Správci mohou zároveň vyloučit potenciálně nebezpečné nebo ohrožené aplikace, takže nebudou moci dešifrovat obsah chráněný správou přístupových práv. Kromě toho mohou správci vyloučit určité verze operačního systému Windows a znemožnit tak přístup klientských počítačů s těmito verzemi systému k obsahu chráněnému právy.

Je-li entita vyloučena, bude uvedena v seznamu vyloučení licencí k použití vytvořených serverem RMS. Pokud se po určité době rozhodnete odstranit entitu původně zahrnutou do zásad vyloučení, můžete tento krok provést pomocí stránky Zásady vyloučení na webu pro správu. Entita pak bude ze seznamu vyloučení odebrána. V dalších požadavcích na licenci nebo certifikát pak již tato entita nebude považována za vyloučenou.

Nejedná-li se o neúmyslně vyloučenou entitu, je doporučeno neodebírat entitu ze zásad vyloučení, dokud není zcela jisté, že všem certifikátům vydaným před vytvořením zásady vyloučení již vypršela doba platnosti. V opačném případě bude možné obsah dešifrovat pomocí starých i nových certifikátů, což může být v rozporu se záměry organizace.

Toto téma obsahuje informace o správě zásad vyloučení. Podrobné pokyny týkající se vyloučení entit naleznete v tomto tématu později v části [Povolení zásad vyloučení](https://technet.microsoft.com/bbb1ce50-bc11-41cf-b75b-a6756141908f).

Tento oddíl se zabývá následujícími tématy:

-   [Vyloučení verzí bezpečnostního modulu](https://technet.microsoft.com/e287f026-aab2-43ab-93bc-48087da82f36)
-   [Vyloučení certifikátů účtů práv](https://technet.microsoft.com/cba5e901-942c-4d06-9865-e6c4648c95e6)
-   [Vyloučení verzí operačního systému Windows](https://technet.microsoft.com/8b8a184d-ac0e-4a43-822c-d2fae2faf484)
-   [Vyloučení aplikací](https://technet.microsoft.com/b68ae4b2-b9ba-44ae-90cb-c88df600ec86)
