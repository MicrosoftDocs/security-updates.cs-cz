---
TOCTitle: Důvěryhodné domény uživatelů
Title: Důvěryhodné domény uživatelů
ms:assetid: 'a09b883f-f455-4c46-a4fd-d37b689e1d24'
ms:contentKeyID: 18113388
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747618(v=WS.10)'
---

Důvěryhodné domény uživatelů
============================

Služba RMS ve výchozím nastavení nevydává licence k použití uživatelům, jejichž certifikáty účtů práv byly vydány jinou doménou uživatelů. Doména uživatelů je instalace služby RMS, kterou tvoří cluster kořenové certifikace, nepovinné servery nebo clustery správy licencí a příslušné databáze.

Službu RMS můžete nakonfigurovat na zpracování tohoto typu požadavků, jestliže naimportujete certifikát serveru pro poskytování licencí jiné domény uživatelů a přidáte jej do seznamu důvěryhodných domén uživatelů. Pokud je provedena tato operace, mohou uživatelé, jejichž certifikáty účtů byly vydány důvěryhodnou uživatelskou doménou, odesílat požadavky na licence k použití do vaší instalace. Tyto licence k použití budou zpracovány stejným způsobem, jako kdyby byly požadovány interními uživateli.

> [!NOTE]
> Cluster kořenové certifikace je do seznamu důvěryhodných domén uživatelů přidán automaticky u všech serverů RMS ve stejné instalaci. 

Uživatelům z jiných uživatelských domén můžete povolit sdílení chráněného obsahu. Tato možnost je ilustrována v následujících příkladech:

-   Daná organizace úzce spolupracuje s jinou organizací na důvěrných dokumentech, které chcete sdílet a zároveň chránit. Druhá organizace také používá službu RMS. Obě organizace mohou přidat instalaci služby RMS té druhé do svého seznamu důvěryhodných domén uživatelů, takže uživatelé obou organizací mohou společně pracovat s chráněným obsahem a vyměňovat si jej prostřednictvím Internetu nebo extranetu.
-   Každá doménová struktura služby Active Directory může obsahovat pouze jednu instalaci služby RMS. Organizace nasadila více doménových struktur služby Active Directory a v každé je spuštěna služba RMS. Uživatelé chtějí sdílet chráněný obsah s jinými uživateli bez ohledu na doménovou strukturu, ke které náleží. Chcete-li to umožnit, můžete přidat instalaci služby RMS ostatních doménových struktur do seznamu důvěryhodných domén uživatelů v každé doménové struktuře.
-   Uživatelé v dané organizaci spolupracují s uživateli v partnerské organizaci na důvěrných dokumentech, které je třeba chránit. Druhá organizace nepoužívá službu RMS. Uživatelé druhé organizace si mohou vytvořit účty služby .NET Passport. Potom službu .NET Passport přidáte do seznamu důvěryhodných domén uživatelů své instalace RMS. Uživatelé v obou společnostech mohou nyní spolupracovat na chráněném obsahu a vyměňovat si jej prostřednictvím sítě Internet.

Další informace o důvěryhodných doménách uživatelů a podrobné pokyny získáte v této sadě dokumentace v částech Přidání a odebrání důvěryhodných domén uživatelů a Vytvoření zásad důvěryhodnosti tématu Provoz serveru RMS.
