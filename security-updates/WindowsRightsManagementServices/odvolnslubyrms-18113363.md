---
TOCTitle: Odvolání služby RMS
Title: Odvolání služby RMS
ms:assetid: '72689f90-f3c5-4b61-94ea-d825f3199b3b'
ms:contentKeyID: 18113363
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747622(v=WS.10)'
---

Odvolání služby RMS
===================

Odvolání představuje mechanismus umožňující odvolat již vydané pověření, jako je certifikát nebo licence. Hlavním účelem odvolání je znemožnit entitám, které přestaly být důvěryhodné, účast v systému služby RMS. Odvolání lze použít například v následujících scénářích:

-   Je nutné znemožnit využití obsahu, protože došlo ke ztrátě důvěryhodnosti zaregistrovaného objektu nebo identity v řetězci důvěryhodnosti, jako například v případě, kdy jednotlivec ukončí pracovní poměr v organizaci a neměl by mít nadále možnost zobrazit obsah chráněný službou RMS.
-   Je nutné znemožnit otevření části obsahu v určité aplikaci s podporou služby RMS, která již není pokládána za důvěryhodnou.
-   Je nutné znemožnit další distribuci nepřijatelné části obsahu, která již byla distribuována a získala licenci umožňující její využití.

Odvolání je uplatněno u klientů a zabraňuje uživatelům v dalším používání části obsahu, a to i tehdy, pokud již pro ni byla vydána licence k použití. Jakmile odvolání povolíte, projeví se při každém pokusu uživatele o využití chráněného obsahu bez ohledu na to, zda v okamžiku využití má uživatel k dispozici kopii licence k použití uloženou v místním počítači nebo zda požaduje novou licenci k použití od serveru RMS.

Tento oddíl obsahuje přehled základních informací o odvolání. Další informace o použití odvolání ve službě RMS získáte v této sadě dokumentace v části Správa odvolání tématu Provoz serveru RMS.

Tento oddíl se zabývá následujícími tématy:

-   [Princip fungování odvolání služby RMS](https://technet.microsoft.com/469e3938-a59b-4c92-9779-ead64e724d00)
-   [Seznamy odvolání služby RMS](https://technet.microsoft.com/688d4dfa-c928-4b2f-8116-2f9e87d2b6f7)
-   [Odvolání v šablonách zásad práv](https://technet.microsoft.com/287c5b92-fcb5-4295-9c2b-4e37e643beb2)
-   [Odvolání a odpojení autoři](https://technet.microsoft.com/a9cf0541-9101-4e90-9c56-7c1b9a8deca6)
