---
TOCTitle: Přidání a odebrání důvěryhodných domén uživatelů
Title: Přidání a odebrání důvěryhodných domén uživatelů
ms:assetid: '7c440b15-01c4-49f1-b43c-00f67f3388c1'
ms:contentKeyID: 18113338
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747571(v=WS.10)'
---

Přidání a odebrání důvěryhodných domén uživatelů
================================================

Ve výchozím nastavení služba RMS nezpracovává požadavky uživatelů, jejichž certifikáty účtů práv byly vydány jinou instalací služby RMS. Je však možné přidat domény uživatelů do seznamu důvěryhodných domén uživatelů. Služba RMS pak bude tyto požadavky zpracovávat.

Pro každou důvěryhodnou doménu lze také přidávat a odebírat konkrétní uživatele a skupiny uživatelů. Dále lze odebrat důvěryhodnou doménu uživatelů, není však možné odebrat cluster kořenové certifikace pro danou doménovou strukturu služby Active Directory z důvěryhodných domén uživatelů. Každý server RMS v nasazení, včetně serveru kořenové certifikace, pokládá cluster kořenové certifikace ve vlastní doménové struktuře za důvěryhodný.

Následujícím postupem můžete spravovat důvěryhodné domény uživatelů:

-   Chcete-li obecně podporovat externí uživatele, můžete do seznamu důvěryhodných domén přidat službu Microsoft® .NET Passport. Tímto způsobem mohou servery RMS ve vaší společnosti zpracovávat požadavky na licencování zahrnující certifikáty účtů práv vydané službou Microsoft .NET Passport.
-   Chcete-li za důvěryhodné pokládat externí uživatele z instalace služby RMS v jiné organizaci, můžete tuto organizaci přidat do seznamu důvěryhodných domén uživatelů. Uvedený postup umožňuje serveru RMS zpracovávat požadavky na licencování zahrnující certifikáty účtů práv vydané serverem RMS této organizace.
-   Pokud chcete zpracovávat požadavky na licencování od uživatelů vlastní organizace, kteří náleží do jiné doménové struktury služby Active Directory, můžete stejným způsobem do seznamu důvěryhodných domén uživatelů přidat instalaci služby RMS dané doménové struktury. Uvedený postup umožňuje serveru RMS z aktuální doménové struktury zpracovávat požadavky na licencování zahrnující certifikáty účtů práv vydané serverem RMS v jiné doménové struktuře.
-   Pro každou důvěryhodnou doménu uživatelů můžete určit, které e-mailové domény jsou důvěryhodné. Pro důvěryhodné domény služby Passport můžete určit, kteří uživatelé e-mailů a domény nejsou důvěryhodné.

Chcete-li do seznamu důvěryhodných domén uživatelů přidat určitou instalaci služby RMS, je třeba pro ni importovat certifikát serveru pro poskytování licencí. Správce musí nejprve exportovat tento certifikát ze serveru nebo clusteru, který má být pokládán za důvěryhodný, a soubor certifikátu vám odeslat. Potom můžete soubor importovat zadáním jeho umístění. Chcete-li soubor uložit, musí mít přihlášený uživatel oprávnění pro přístup do sdílené složky. Při nastavení důvěryhodné domény uživatelů nejsou přeneseny informace soukromého klíče.

Podrobný postup nastavení důvěryhodných domén uživatelů naleznete v tomto tématu později v části [Přidání důvěryhodné domény uživatelů](https://technet.microsoft.com/ed672e58-6272-4ac0-a434-d1d938037e93).
