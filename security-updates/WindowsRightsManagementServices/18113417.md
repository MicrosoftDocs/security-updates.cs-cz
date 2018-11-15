---
TOCTitle: Určení topologie služby RMS
Title: Určení topologie služby RMS
ms:assetid: 'bf516f7d-b3a1-4e7f-971f-bfab1db41812'
ms:contentKeyID: 18113417
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747651(v=WS.10)'
---

Určení topologie služby RMS
===========================

V základní topologii služby RMS zajišťuje server nebo cluster kořenové certifikace ve všech doménových strukturách služby Active Directory veškeré služby RMS pro danou organizaci. Tato topologie služby RMS funguje dobře ve velkých i malých organizacích. V distribuované topologii služby RMS může jeden či více serverů správy licencí (někdy označované také jako servery správy licencí pro oddělení) poskytovat některé nebo všechny služby správy licencí pro konkrétní uživatele a skupiny v organizaci. Přestože server (nebo cluster) kořenové certifikace i nadále zajišťuje certifikaci účtů a službu aktivačního serveru proxy pro celou organizaci, je distribuovaná topologie služby RMS určena pro organizace s velmi specifickými požadavky na správu licencí a na řízení služby RMS v určité části dané organizace.

Ačkoli lze u služby RMS použít pouze dvě hlavní topologie, mohou se jejich součásti velmi lišit. Chcete-li definovat součásti odpovídající potřebám organizace a vytvořit správnou topologii nasazení služby RMS, je nutné provést následující kroky:

-   vyhodnotit požadavky a cíle organizace,
-   definovat způsob použití správy práv,
-   analyzovat očekávané trasy a objemy toku dat a implementovat odpovídající úroveň služby.

Definování topologie a rozhodování nutné pro implementaci návrhu představuje proces, který se bude během plánování nasazení služby RMS neustále opakovat.

Toto téma se zabývá následující problematikou:

-   [Určení hlavních součástí](https://technet.microsoft.com/c9ec225b-0e51-42f5-aff6-0aecb62e3b27)
-   [Stanovení cílů topologie](https://technet.microsoft.com/8275a04d-3e5b-40b0-be9d-2f31b7aeca6b)
-   [Definování rozsahu implementace služby RMS](https://technet.microsoft.com/4b5fe1be-643e-47c4-bf9b-50d1e97108fb)
-   [Vyhodnocení požadavků na rozsah](https://technet.microsoft.com/89f0138c-946d-47d7-a286-041d4d9606a8)
-   [Zajištění redundance dat a vyrovnávání zatížení](https://technet.microsoft.com/162d547c-78a7-4848-b43e-58e481832af2)
-   [Vyhodnocení požadavků migrace](https://technet.microsoft.com/cec07f45-dc52-4004-860b-5cc33e5fc209)
-   [Plánování infrastruktury databázového serveru](https://technet.microsoft.com/b12354bd-3143-4d1f-b5aa-450c4550653c)
-   [Plánování nasazení v doménových strukturách](https://technet.microsoft.com/2dfb40b7-95b1-4362-b32e-72867544b705)
-   [Plánování externích uživatelů služby RMS](https://technet.microsoft.com/107e1338-4dcf-4ed5-a49d-e875cc883db1)
-   [Plánování základní topologie služby RMS](https://technet.microsoft.com/fec3201e-201f-4faf-910e-fa44132af83d)
-   [Plánování distribuované topologie služby RMS](https://technet.microsoft.com/8773a1e0-6ac3-41f5-9866-5890cef08d04)
