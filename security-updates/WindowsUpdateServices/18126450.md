---
TOCTitle: 'Krok 6: Vytvoření skupiny počítačů'
Title: 'Krok 6: Vytvoření skupiny počítačů'
ms:assetid: '6039e5dc-d2ce-4d4b-b737-17ebcadbd4a7'
ms:contentKeyID: 18126450
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc720536(v=WS.10)'
---

Krok 6: Vytvoření skupiny počítačů
==================================

Skupiny počítačů jsou důležitou částí nasazení služby WSUS, dokonce i základního. Skupiny počítačů umožňují zacílit aktualizace na specifické počítače. Existují dvě výchozí skupiny počítačů: Všechny počítače a Nezařazené počítače. Při výchozím nastavení, když jednotlivé klientské počítače poprvé kontaktují server WSUS, přidá je server do obou těchto skupin.

Můžete vytvářet vlastní skupiny počítačů. Jedním z přínosů vytváření skupin počítačů je, že umožňuje testovat aktualizace před jejich širokým nasazením. Pokud testování probíhá dobře, můžete uvolnit aktualizace pro skupinu Všechny počítače. Neexistuje žádné omezení počtu vlastních skupin, které lze vytvořit.

Proces nastavení skupin počítačů zahrnuje tři kroky. Nejprve zadáte, jak chcete přiřadit počítače do skupin. Existují dvě možnosti: *na straně serveru* a *na straně klienta*. Zařazení na straně serveru představuje ruční přidání jednotlivých počítačů do skupiny pomocí serveru WSUS. Zařazení na straně klienta zahrnuje automatické přidání klientů pomocí skupiny zásad nebo klíčů registru. Za druhé, vytvoříte skupinu počítačů na serveru WSUS. Za třetí, přesunete počítače do skupin pomocí jedné z metod, kterou jste vybrali v prvním kroku.

Tento dokument vysvětluje, jak používat zařazení na straně serveru a ruční přesunutí počítačů do jejich skupin pomocí konzoly WSUS. Pokud byste měli do skupin přiřadit velký počet klientských počítačů, mohli byste použít zařazení na straně klienta, při kterém by bylo přesunutí počítačů do skupin provedeno automaticky.

Nastavit testovací skupinu, která obsahuje alespoň jeden testovací počítač, můžete pomocí kroku 6.

Tento krok obsahuje následující postupy:

-   zadání zařazení na straně serveru,
-   vytvoření skupiny,
-   přesunutí počítačů do skupiny,

**zadání způsobu přiřazení počítačů do skupin.**
1.  Na panelu nástrojů konzoly služby WSUS klepněte na tlačítko **Možnosti** a potom na odkaz **Možnosti počítačů**.

2.  Ve skupinovém rámečku **Možnosti počítačů** klepněte na přepínač **Použít úlohu služby Windows Server Update Services Přesunout počítače**.

3.  Po zobrazení zprávy s potvrzením klepněte ve skupinovém rámečku **Úkoly** na odkaz **Uložit nastavení** a potom na tlačítko **OK**.

**Vytvoření skupiny**
1.  Na panelu nástrojů konzoly služby WSUS klepněte na tlačítko **Počítače**.

2.  Ve skupinovém rámečku **Úkoly** klepněte na odkaz **Vytvořit skupinu počítačů**.

3.  Do pole **Název skupiny** zadejte **Test** a klepněte na tlačítko **OK**.

K přiřazení klientského počítače vhodného pro testování do testovací skupiny použijte následující postup. Klientský počítač vhodný pro testování je jakýkoli počítač se softwarem a hardwarem, které jsou typické pro většinu počítačů v síti, nikoli však počítač, kterému byla přiřazena velmi důležitá role. Tímto způsobem je možné určit, jak dobře budou u počítačů srovnatelných s testovacím počítačem probíhat aktualizace, které schválíte.

**Ruční přidání počítače k testovací skupině**
1.  Na panelu nástrojů konzoly služby WSUS klepněte na tlačítko **Počítače**.

2.  V poli **Skupiny** klepněte na skupinu počítače, který chcete přesunout.

3.  V seznamu počítačů vyberte počítač, který chcete přesunout.

4.  Ve skupinovém rámečku **Úkoly** klepněte na odkaz **Přesunout vybraný počítač**.

5.  V seznamu **Skupina počítače** vyberte skupinu, do které chcete přesunout počítač, a klepněte na tlačítko **OK**.
