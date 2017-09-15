---
TOCTitle: 'Krok 7: Schválení a nasazení aktualizací'
Title: 'Krok 7: Schválení a nasazení aktualizací'
ms:assetid: '38db25a9-6702-4e43-b536-764e8814afc6'
ms:contentKeyID: 18126495
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc720504(v=WS.10)'
---

Krok 7: Schválení a nasazení aktualizací
========================================

V tomto kroku schválíte aktualizaci pro jakékoli testovací klientské počítače v testovací skupině. Počítače v této skupině budou během následujících 24 hodin provádět přihlášení k serveru WSUS. Po této době můžete použít funkci vytváření zpráv serveru WSUS k zjištění, zda byly tyto aktualizace nasazeny do počítačů. Pokud testování probíhá dobře, můžete potom schválit stejnou aktualizaci pro zbývající počítače ve vaší organizaci.

Krok 7 obsahuje následující postupy:

-   schválení a nasazení aktualizace,
-   kontrola sestavy Stav aktualizací,

**schválení a nasazení aktualizace.**
1.  Na panelu nástrojů konzoly služby WSUS klepněte na tlačítko **Aktualizace**. Při výchozím nastavení se seznam aktualizací filtruje tak, aby se zobrazily pouze kritické aktualizace a aktualizace zabezpečení, u nichž bylo schváleno rozpoznávání v klientských počítačích. Pro tento postup použijte výchozí filtr.

2.  Na seznamu aktualizací vyberte aktualizace, které chcete schválit pro instalaci. Informace o vybrané aktualizaci jsou k dispozici na kartě **Podrobnosti**. Chcete-li vybrat více po sobě jdoucích aktualizací, stiskněte a během jejich výběru podržte stisknutou klávesu SHIFT. Chcete-li vybrat více aktualizací, které nejdou po sobě, stiskněte a během jejich výběru podržte stisknutou klávesu CTRL.

3.  Ve skupinovém rámečku **Úkoly aktualizací** klepněte na možnost **Změnit stav schválení**. Zobrazí se dialogové okno **Schválení aktualizací**.

4.  V seznamu **Skupinové nastavení schvalování pro vybrané aktualizace** klepněte ve sloupci **Schválení** pro testovací skupinu na položku **Nainstalovat** a potom klepněte na tlačítko **OK**.

| ![](images/Cc720504.note(WS.10).gif)Poznámka                                                                                                                                                                                                                   |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Se schvalováním aktualizací souvisí mnoho možností, například nastavení termínů a odinstalace aktualizací. Informace o nich získáte v dokumentu White Paper Microsoft Windows Server Update Services Operations Guide (Průvodce operacemi služby Microsoft Windows Server Update Services). |

Po 24 hodinách můžete použít funkci vytváření zpráv serveru WSUS k zjištění, zda tyto aktualizace byly nasazeny do počítačů.

**Kontrola sestavy Stav aktualizací**
1.  Na panelu nástrojů konzoly služby WSUS klepněte na tlačítko **Sestavy**.

2.  Na stránce **Sestavy** klepněte na možnost **Stav aktualizací**.

3.  Chcete-li filtrovat seznam aktualizací, vyberte ve skupinovém rámečku **Zobrazit** kritéria, která chcete použít, a potom klepněte na tlačítko **Použít**.

4.  Chcete-li zobrazit stav aktualizace podle skupiny počítače a potom podle počítače, rozbalte podle potřeby zobrazení aktualizace.

5.  Chcete-li vytisknout sestavu Stav aktualizací, klepněte ve skupinovém rámečku **Úkoly** na odkaz **Tisk sestavy**.

Pokud byly aktualizace úspěšně nasazeny do testovací skupiny, můžete schválit stejné aktualizace pro zbývající počítače ve vaší organizaci.
