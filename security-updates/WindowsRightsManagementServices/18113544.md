---
TOCTitle: Přidání důvěryhodné domény uživatelů
Title: Přidání důvěryhodné domény uživatelů
ms:assetid: 'ed672e58-6272-4ac0-a434-d1d938037e93'
ms:contentKeyID: 18113544
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747793(v=WS.10)'
---

Přidání důvěryhodné domény uživatelů
====================================

Provedení tohoto postupu vyžaduje, aby byl uživatel místně přihlášen k webu pro správu v rámci uživatelského účtu, který je členem skupiny Administrators v počítači, k němuž získává přístup. Uvedený postup mohou provést také členové skupiny Domain Admins. Z hlediska zabezpečení je nejvhodnější při provádění tohoto postupu použít příkaz **Spustit jako**.

Chcete-li otevřít webovou stránku **Globální správa**, klepněte na tlačítko **Start**, přejděte na příkaz **Všechny programy**, přejděte na položku **Služba RMS v systému Windows** a klepněte na položku **Správa služby RMS v systému Windows**.

Přidání důvěryhodných domén uživatelů
-------------------------------------

#### Přidání důvěryhodné domény uživatelů

1.  Otevřete stránku **Globální správa** a klepněte na položku **Spravovat službu RMS na tomto webu** u webu, na který chcete přidat doménu důvěryhodných uživatelů.

2.  V části odkazů **správy** klepněte na odkaz **Zásady důvěryhodnosti**.

3.  V části **Důvěryhodné domény uživatelů** klepněte na tlačítko **Procházet**, vyhledejte certifikát serveru pro poskytování licencí domény uživatelů, kterou chcete importovat a vytvořit tak vztah důvěryhodnosti, poklepejte na tento certifikát a poté klepněte na tlačítko **Přidat**.

    Název domény se objeví v seznamu **Důvěryhodné domény uživatelů**.

4.  Chcete-li zadat, které e-mailové domény v rámci důvěryhodné domény uživatelů lze považovat za důvěryhodné, otevřete klepnutím na odkaz **Důvěryhodné domény** vedle názvu certifikátu okno **Důvěryhodné e-mailové domény**.

5.  Zvolte jednu z následujících možností:

    -   Chcete-li důvěřovat všem uživatelským účtům, které jsou členy této domény, vyberte možnost **Důvěřovat všem e-mailovým doménám**.

        –nebo-
        
    -   Vyberte možnost **Důvěřovat pouze zadaným e-mailovým doménám**, zadejte název domény, která má být považována za důvěryhodnou, například priklad.com, a klepněte na tlačítko **Přidat**. Doména bude přidána do seznamu Důvěryhodné e-mailové domény. Chcete-li odebrat název ze seznamu, vyberte jej a klepněte na tlačítko **Odebrat**. Uvedením domény zahrnete i všechny její subdomény.

6.  Používáte-li službu RMS v prostředí, v němž je nutné rozšířit členství ve skupinách mezi doménovými strukturami, zaškrtněte políčko **Důvěřovat správě licencí RM pro identifikátory zabezpečení (SID) této uživatelské domény**.

7.  Po provedení všech požadovaných úprav klepněte na odkaz **Zavřít okno a vrátit se k zásadám důvěryhodnosti**.

Další informace o provádění tohoto postupu naleznete v tomto tématu v části [Přidání a odebrání důvěryhodných domén uživatelů](https://technet.microsoft.com/7c440b15-01c4-49f1-b43c-00f67f3388c1) uvedené již dříve.
