---
TOCTitle: 'Krok 7: Schválení a nasazení aktualizací ve službě WSUS 3.0'
Title: 'Krok 7: Schválení a nasazení aktualizací ve službě WSUS 3.0'
ms:assetid: '88fac442-a9d3-4e74-92f6-3822b7237af1'
ms:contentKeyID: 18126698
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc708475(v=WS.10)'
---

Krok 7: Schválení a nasazení aktualizací ve službě WSUS 3.0
===========================================================

V tomto kroku schválíte aktualizaci pro jakékoli testovací klientské počítače v testovací skupině. Počítače v této skupině budou během následujících 24 hodin kontaktovat server WSUS. Po této době můžete použít funkci vytváření zpráv serveru WSUS k zjištění, zda byly tyto aktualizace nasazeny do počítačů. Pokud testování proběhne dobře, můžete potom schválit stejné aktualizace pro zbývající počítače v organizaci.

**Krok 7 obsahuje následující postupy**:

-   schválení a nasazení aktualizace,
-   kontrola stavu aktualizace,

**schválení a nasazení aktualizace.**
1.  V konzole Správa služby WSUS klepněte na tlačítko **Aktualizace**. Tím zobrazíte souhrn aktualizací ve výchozích zobrazeních (**Všechny aktualizace**, **Kritické aktualizace**, **Aktualizace zabezpečení** a **Aktualizace služby WSUS**). V tomto postupu použijte možnost **Všechny aktualizace**.

2.  V seznamu aktualizací vyberte aktualizace, které chcete schválit pro instalaci. Informace o vybrané aktualizaci jsou k dispozici v nejspodnějším podokně panelu Aktualizace. Chcete-li vybrat více po sobě jdoucích aktualizací, při klepnutí na aktualizace držte stisknutou klávesu **SHIFT**. Chcete-li vybrat více aktualizací, které nejdou po sobě, držte stisknutou klávesu **CTRL** a postupně klepněte na jednotlivé aktualizace.

3.  Klepněte pravým tlačítkem myši na výběr a klepněte na příkaz **Schválit**. Zobrazí se dialogové okno **Schválení aktualizací**.

4.  Vyberte jednu ze skupin (například **Test**) a klepněte na šipku vlevo od ní. Zobrazí se místní nabídka s možnostmi **Schváleno k instalaci**, **Schváleno k odebrání**, **Neschváleno**, **Termín**, **Stejné jako nadřazené** a **Použít na podřízené**. Klepněte na možnost **Schváleno k instalaci** a potom klepněte na tlačítko **OK**.

5.  Zobrazí se nové okno **Průběh schvalování**, ve kterém se zobrazuje průběh různých úloh, které mají vliv na schvalování aktualizací. Po dokončení schvalování zavřete toto okno klepnutím na tlačítko **Zavřít**.

> [!NOTE]
> Se schvalováním aktualizací souvisí mnoho možností, například nastavení termínů a odinstalace aktualizací. 

Po 24 hodinách můžete použít funkci vytváření zpráv serveru WSUS ke zjištění, zda byly tyto aktualizace nasazeny do počítačů.

**Kontrola stavu aktualizace**
1.  V konzole Správa služby WSUS klepněte na tlačítko **Sestavy** v levém podokně.

2.  Na stránce **Sestavy** bude zobrazeno několik standardizovaných hlášení. Klepněte na hlášení **Souhrn informací o stavu aktualizace**. Zobrazí se okno **Hlášení o aktualizacích**.

3.  Chcete-li filtrovat seznam aktualizací, vyberte kritéria, která chcete použít (například **Zahrnout aktualizace do těchto klasifikací**), a potom klepněte na tlačítko **Spustit hlášení** na panelu nástrojů okna.

4.  Zobrazí se podokno **Hlášení o aktualizacích**. Stav jednotlivých aktualizací můžete zkontrolovat výběrem dané aktualizace v levé části podokna. Poslední část podokna hlášení zobrazuje souhrn stavu dané aktualizace.

5.  Toto hlášení můžete uložit nebo vytisknout klepnutím na příslušnou ikonu na panelu nástrojů.

Pokud byly aktualizace úspěšně nasazeny do testovací skupiny, můžete schválit stejné aktualizace pro zbývající počítače v organizaci.
