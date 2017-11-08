---
TOCTitle: Certifikáty a licence služby RMS
Title: Certifikáty a licence služby RMS
ms:assetid: '91916ecb-9e5d-49e8-ab65-ef2c56339b83'
ms:contentKeyID: 18113368
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747600(v=WS.10)'
---

Certifikáty a licence služby RMS
================================

Různé součásti instalace služby RMS jsou propojeny vztahem důvěryhodnosti, který je implementován sadou certifikátů. Vynucení platnosti těchto certifikátů představuje hlavní funkci technologie RMS. Každá část obsahu chráněného službou RMS je publikována s licencí obsahující příslušná pravidla využití a každý uživatel, který chce daný obsah využít, získá jedinečnou licenci zajišťující načtení, interpretaci a vynucení uvedených pravidel. V tomto kontextu je licence určitým typem certifikátu.

Služba RMS používá k vyjádření práv využití chráněného obsahu syntaxi jazyka XML, konkrétně jazyk XrML (eXtensible rights Markup Language) verze 1.2.1. Další informace získáte v tomto tématu později v části Jazyky XrML.

Certifikáty a licence používané ve službě RMS jsou propojeny v rámci hierarchie, takže služba RMS může vždy vysledovat daný řetězec od konkrétního certifikátu nebo licence přes důvěryhodné certifikáty až po důvěryhodný pár klíčů. Další informace získáte v tomto tématu později v části [Hierarchie důvěryhodnosti služby RMS](https://technet.microsoft.com/2d44182f-a653-4383-aba1-dade53f7cf9a).

Tento oddíl se zabývá následujícími tématy:

-   [Souhrn certifikátů a licencí služby RMS](https://technet.microsoft.com/637ccfca-318e-4346-85b5-0945b058fb9c)
-   [Certifikáty serveru pro poskytování licencí](https://technet.microsoft.com/0b35fbcd-25a9-4587-898d-9a30fd1d3c5b)
-   [Klientské certifikáty pro poskytování licencí](https://technet.microsoft.com/bfb36387-3e15-4cde-8b8f-482219569a64)
-   [Certifikáty počítače RMS](https://technet.microsoft.com/1841d53e-d01b-47c3-9d43-3805ceefed5a)
-   [Certifikáty účtů práv](https://technet.microsoft.com/2ff315cc-211d-4e6e-85e8-56867c2abd94)
-   [Licence k publikování](https://technet.microsoft.com/187228fc-370b-4e23-a53a-21bb296b84a1)
-   [Licence k použití](https://technet.microsoft.com/6e609db3-49b3-4cac-a34c-8a96da627067)
