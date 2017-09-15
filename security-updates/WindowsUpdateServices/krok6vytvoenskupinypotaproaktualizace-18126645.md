---
TOCTitle: 'Krok 6: Vytvoření skupiny počítačů pro aktualizace'
Title: 'Krok 6: Vytvoření skupiny počítačů pro aktualizace'
ms:assetid: 'fe219654-eae8-45ca-a44b-c1e05c3c3e93'
ms:contentKeyID: 18126645
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc708629(v=WS.10)'
---

Krok 6: Vytvoření skupiny počítačů pro aktualizace
==================================================

Skupiny počítačů jsou důležitou částí nasazení služby WSUS, dokonce i základního. Skupiny počítačů umožňují zacílit aktualizace na specifické počítače. Existují dvě výchozí skupiny počítačů: Všechny počítače a Nezařazené počítače. Ve výchozím nastavení přidá server WSUS jednotlivé klientské počítače, které jej poprvé kontaktují, do obou těchto skupin.

Můžete vytvářet vlastní skupiny počítačů. Jedním z přínosů vytváření skupin počítačů je, že umožňují testovat aktualizace před jejich širokým nasazením. Pokud testování probíhá dobře, můžete aktualizace zařadit do skupiny Všechny počítače. Neexistuje žádné omezení počtu vlastních skupin, které lze vytvořit.

**Nastavení skupin počítačů**
1.  Zadejte způsob, jakým chcete počítače přiřazovat do skupin. Existují dvě možnosti: na straně serveru a na straně klienta. Zařazení na straně serveru zahrnuje ruční přidávání jednotlivých počítačů do skupiny pomocí služby WSUS. Zařazení na straně klienta zahrnuje automatické přidávání klientů buď pomocí zásad skupiny, nebo klíčů registru.

2.  Vytvoření skupiny počítačů na serveru WSUS

3.  Přesuňte počítače do skupin pomocí metody, kterou jste vybrali v kroku 1.

Tato část vysvětluje jak používat zařazení na straně serveru a ručně přesouvat počítače do skupin pomocí konzoly pro správu služby WSUS. Pokud máte do skupin přiřadit několik klientských počítačů, lze použít zařazení na straně klienta, které automaticky přesouvá počítače do skupin.

Pomocí kroku 6 můžete nastavit testovací skupinu, která obsahuje alespoň jeden testovací počítač.

**Krok 6 obsahuje následující postupy:**

-   vytvoření skupiny,
-   přidání počítače do skupiny.

**Vytvoření skupiny**
1.  V konzole pro správu služby WSUS rozbalte položku **Počítače** a zvolte možnost **Všechny počítače.**

2.  Klepněte pravým tlačítkem na možnost **Všechny počítače** nebo přejděte do podokna **Akce** a potom klepněte na možnost **Přidat skupinu počítačů**.

3.  Zobrazí se dialogové okno **Přidat skupinu počítačů**. Zadejte název nové skupiny.

K přiřazení klientského počítače do testovací skupiny použijte následující postup. Klientským počítačem vhodným pro testování může být libovolný počítač se softwarem a hardwarem, které jsou typické pro většinu počítačů v síti, ale nemůže jím být počítač, kterému byla přiřazena důležitá role. Tímto způsobem lze určit, s jakým výsledkem budou provedeny schválené aktualizace počítačů podobných testovacímu počítači.

**Přidání počítače do skupiny**
1.  V konzole pro správu služby WSUS klepněte na možnost **Počítače**.

2.  Klepněte na skupinu, do které chcete počítač přesunout.

3.  V seznamu počítačů zvolte počítač, který chcete přesunout.

4.  Pravým tlačítkem klepněte na možnost **Změnit členství**.

5.  Zobrazí se dialogové okno **Nastavit členství ve skupině počítačů** se seznamem skupin.

6.  Zaškrtněte skupinu, do které chcete přidat počítač, a klepněte na tlačítko **OK**.
