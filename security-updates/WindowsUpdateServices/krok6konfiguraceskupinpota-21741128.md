---
TOCTitle: 'Krok 6: Konfigurace skupin počítačů'
Title: 'Krok 6: Konfigurace skupin počítačů'
ms:assetid: '70518732-2179-4e41-9609-7f9999867f41'
ms:contentKeyID: 21741128
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Dd939860(v=WS.10)'
---

Krok 6: Konfigurace skupin počítačů
===================================

Skupiny počítačů jsou důležitou částí nasazení aktualizace Windows Server Update Services 3.0 Service Pack 2 (WSUS 3.0 SP2). Skupiny počítačů povolují testování aktualizací a směrování aktualizací na konkrétní počítače. Existují dvě výchozí skupiny počítačů: Všechny počítače a Nezařazené počítače. Ve výchozím nastavení přidá server WSUS každý klientský počítač, který jej poprvé kontaktuje, do obou těchto skupin.

Ke správě aktualizací ve vaší společnosti můžete vytvořit tolik vlastních skupin počítačů, kolik potřebujete. Nejvhodnější je vytvořit alespoň jednu skupinu počítačů k otestování aktualizací před jejich nasazením do jiných počítačů ve vaší společnosti.

Krok 6 – postupy
----------------

1.  Vytvoření testovací skupiny počítačů
2.  Přesunutí alespoň jednoho počítače do testovací skupiny

**Vytvoření testovací skupiny**
1.  V konzole pro správu služby WSUS rozbalte položku **Počítače** a zvolte možnost **Všechny počítače**.

2.  Pravým tlačítkem myši klikněte na položku **Všechny počítače** a potom klikněte na příkaz **Přidat skupinu počítačů**.

3.  V dialogovém okně **Přidat skupinu počítačů** zadejte **Název** nové testovací skupiny a klikněte na tlačítko **Přidat**.

V následujícím postupu přiřadíte klientský počítač do testovací skupiny. Testovací počítač je libovolný počítač se softwarem a hardwarem konzistentním s většinou klientských počítačů v síti, kterému zatím nebyla přiřazena důležitá role. Jakmile budou testy úspěšné, můžete schválit aktualizace pro počítače ve skupinách dle vašeho výběru.

**Přiřazení počítače do testovací skupiny**
1.  V konzole pro správu služby WSUS klikněte na možnost **Počítače**.

2.  Klikněte na skupinu počítače, který chcete přiřadit do testovací skupiny.

3.  V seznamu počítačů vyberte počítač nebo počítače, které chcete přiřadit testovací skupině.

4.  Pravým tlačítkem klikněte na možnost **Změnit členství**.

5.  V dialogovém okně **Nastavit členství ve skupině počítačů** vyberte testovací skupinu, kterou jste dříve vytvořili, a potom klikněte na tlačítko **OK**.

Chcete-li vytvořit co nejvíce dalších skupin počítačů potřebných ke správě aktualizací ve vaší síti, opakujte tyto dva postupy, tzn. vytvořte skupinu a potom jí přiřaďte počítač nebo počítače.

Další krok
----------

[Krok 7: Schválení a nasazení aktualizací služby WSUS](https://technet.microsoft.com/c4e58e17-d5e3-4194-8f26-b459e0c03b86)

Další zdroje informací
----------------------

[Podrobný průvodce aktualizací Windows Server Update Services 3.0 SP2](https://technet.microsoft.com/4b504edc-93b3-45b0-a7e8-d0107f1a4442)
