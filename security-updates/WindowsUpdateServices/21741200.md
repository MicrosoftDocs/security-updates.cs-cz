---
TOCTitle: 'Krok 7: Schválení a nasazení aktualizací služby WSUS'
Title: 'Krok 7: Schválení a nasazení aktualizací služby WSUS'
ms:assetid: 'c4e58e17-d5e3-4194-8f26-b459e0c03b86'
ms:contentKeyID: 21741200
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Dd939909(v=WS.10)'
---

Krok 7: Schválení a nasazení aktualizací služby WSUS
====================================================

V tomto kroku schválíte aktualizaci pro jakékoli počítače v testovací skupině pro aktualizaci Windows Server Update Services 3.0 Service Pack 2 (WSUS 3.0 SP2). Počítače v této skupině budou během následujících 24 hodin automaticky kontaktovat server WSUS, aby získaly tuto aktualizaci. Chcete-li zjistit, zda byly tyto aktualizace nasazeny do testovacích počítačů, můžete použít funkci vytváření zpráv služby WSUS. Jakmile budou tyto testy úspěšně dokončeny, můžete aktualizace schválit pro příslušné skupiny počítačů ve vaší společnosti.

Krok 7 – postupy
----------------

-   Schválení a nasazení aktualizace
-   Kontrola stavu aktualizace

**Schválení a nasazení aktualizace**
1.  V konzole pro správu služby WSUS klikněte na tlačítko **Aktualizace**. Souhrnné hlášení o stavu aktualizace je zobrazeno pro **Všechny aktualizace**, **Kritické aktualizace**, **Aktualizace zabezpečení** a **Aktualizace služby WSUS**.

2.  V části **Všechny aktualizace** klikněte na možnost **Aktualizace vyžadované počítači**.

3.  V seznamu aktualizací vyberte aktualizace, které chcete schválit k instalaci v testovací skupině počítačů. Informace o vybrané aktualizaci jsou k dispozici v dolním podokně panelu Aktualizace. Chcete-li vybrat více po sobě jdoucích aktualizací, při kliknutí na aktualizace držte stisknutou klávesu **SHIFT**. Chcete-li vybrat více aktualizací, které nejdou po sobě, držte stisknutou klávesu **CTRL** a postupně klikněte na jednotlivé aktualizace.

4.  Klikněte pravým tlačítkem myši na výběr a klikněte na příkaz **Schválit**.

5.  V dialogovém okně **Schválení aktualizací** vyberte testovací skupinu a potom klikněte na šipku dolů.

6.  Klikněte na možnost **Schváleno k instalaci** a potom klikněte na tlačítko **OK**.

7.  Zobrazí se okno Průběh schvalování, které zobrazuje průběh úkolů ovlivňujících schválení aktualizace. Jakmile bude schválení dokončeno, klikněte na tlačítko **Zavřít**.

Po 24 hodinách můžete použít funkci vytváření zpráv služby WSUS ke zjištění, zda byly tyto aktualizace nasazeny do počítačů testovací skupiny.

**Kontrola stavu aktualizace**
1.  V navigačním podokně konzoly pro správu služby WSUS klikněte na položku **Hlášení**.

2.  Na stránce **Hlášení** klikněte na hlášení **Souhrnné hlášení o stavu aktualizace**. Zobrazí se okno **Hlášení o aktualizacích**.

3.  Chcete-li filtrovat seznam aktualizací, vyberte kritéria, která chcete použít (například **Zahrnout aktualizace do těchto klasifikací**), a potom klikněte na tlačítko **Spustit hlášení** na panelu nástrojů okna.

4.  Zobrazí se podokno **Hlášení o aktualizacích**. Stav jednotlivých aktualizací můžete zkontrolovat výběrem dané aktualizace v levé části podokna. Poslední část podokna hlášení zobrazuje souhrn stavu dané aktualizace.

5.  Toto hlášení můžete uložit nebo vytisknout kliknutím na příslušnou ikonu na panelu nástrojů.

6.  Jakmile aktualizace otestujete, můžete je schválit k instalaci v příslušných skupinách počítačů ve vaší společnosti.

Další zdroje informací
----------------------

[Podrobný průvodce aktualizací Windows Server Update Services 3.0 SP2](https://technet.microsoft.com/4b504edc-93b3-45b0-a7e8-d0107f1a4442)

Další informace o použití aktualizace WSUS 3.0 SP2 naleznete v tématech:

Příručka pro nasazení služby WSUS na adrese [http://go.microsoft.com/fwlink/?LinkId=139832](http://go.microsoft.com/fwlink/?linkid=139832) (stránka může být v angličtině)

Provozní příručka služby WSUS na adrese [http://go.microsoft.com/fwlink/?LinkId=139838](http://go.microsoft.com/fwlink/?linkid=139838) (stránka může být v angličtině)
