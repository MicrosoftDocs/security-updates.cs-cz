---
TOCTitle: 'Krok 4: Konfigurace aktualizací a nastavení synchronizace'
Title: 'Krok 4: Konfigurace aktualizací a nastavení synchronizace'
ms:assetid: '734cc2ed-98be-4772-a42c-8fd38b39d864'
ms:contentKeyID: 18126481
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc708447(v=WS.10)'
---

Krok 4: Konfigurace aktualizací a nastavení synchronizace
=========================================================

Před stažením aktualizací je třeba určit, které aktualizace mají být staženy. Tato část popisuje postup konfigurace sady aktualizací, které chcete stahovat.

V tomto kroku jsou popsány následující postupy:

-   uložení a stažení informací o serveru pro odesílání dat a proxy serveru,
-   výběr jazyka požadovaných aktualizací,
-   výběr produktů, pro které chcete získávat aktualizace,
-   výběr klasifikací požadovaných aktualizací,
-   určení plánu synchronizace pro tento server.

Následujících pět postupů popisuje konfiguraci aktualizací pomocí průvodce konfigurací. Další postupy popisují, jak provést totéž pomocí konzoly Správa služby WSUS výběrem specifických možností.

**Uložení a stažení informací o serveru pro odesílání dat a proxy serveru**
1.  Měli byste mít dokončenu konfiguraci serveru pro odesílání dat a proxy serveru v průvodci konfigurací a měli byste vidět stránku **Připojit k serveru pro odesílání dat**.

2.  Klepněte na tlačítko **Spustit připojování**. Tím uložíte a odešlete nastavení a získáte informace o dostupných aktualizacích.

3.  Během připojování bude dostupné tlačítko **Zastavit připojování**. Dojde-li problémům s připojením, klepněte na tlačítko **Zastavit připojování**, odstraňte problémy a znovu spusťte připojení.

4.  Po úspěšném dokončení stahování pokračujte klepnutím na tlačítko **Další** na stránku **Zvolit jazyky**, případně na levém panelu vyberte jinou stránku.

**Výběr jazyků aktualizací**
1.  Stránka **Vybrat jazyky** umožňuje získat aktualizace ze všech jazyků nebo z určité dílčí sady jazyků. Výběrem jen dílčí sady jazyků lze uspořit místo na disku, je ale důležité vybrat všechny jazyky, které budou potřebovat klienti tohoto serveru WSUS.

2.  Chcete-li stahovat aktualizace pouze pro několik jazyků, vyberte možnost **Stahovat aktualizace pouze v těchto jazycích** a vyberte jazyky, pro které chcete aktualizace. Klepnutím na tlačítko **Další** přejděte na stránku **Vybrat produkty**, případně v levém panelu vyberte jinou stránku.

**Výběr produktů aktualizací**
1.  Stránka **Vybrat produkty** umožňuje určit produkty, pro které chcete aktualizace.

2.  Můžete zaškrtnout kategorie produktů (například Windows) nebo určité produkty (například Windows Server 2003). Výběrem kategorie produktů vyberete všechny produkty v příslušné kategorii. Klepnutím na tlačítko **Další** pokračujte na stránku **Vybrat klasifikace**, případně v levém panelu vyberte jinou stránku.

**Výběr klasifikací aktualizací**
1.  Stránka **Vybrat klasifikace** umožňuje vybrat klasifikace aktualizací, které chcete získávat. Můžete vybrat všechny klasifikace nebo pouze určitou dílčí sadu.

2.  Klepnutím na tlačítko **Další** pokračujte na stránku **Konfigurovat plán synchronizace**, případně v levém panelu vyberte jinou stránku.

**Konfigurace plánu synchronizace**
1.  Zobrazí se stránka **Nastavit plán synchronizace**, která umožňuje vybrat, zda chcete provádět synchronizaci ručně nebo automaticky.

2.  Zvolíte-li na tomto serveru možnost ruční aktualizace, bude třeba spustit proces synchronizace z konzoly Správa služby WSUS.

3.  Zvolíte-li možnost automatické synchronizace, server WSUS bude provádět synchronizaci v určených intervalech. Nastavte čas první synchronizace a určete počet synchronizací za den, které má tento server provést. Pokud například určíte, že za den mají proběhnout čtyři synchronizace se začátkem ve 3:00, dojde k synchronizaci ve 3:00, 9:00, 15:00 a 21:00.

Po dokončení všech uvedených kroků konfigurace vyberte v průvodci konfigurací stránku **Dokončeno**. Konzolu Správa služby WSUS lze spustit tím, že ponecháte zaškrtnuté políčko **Spustit modul snap-in Správa služby Windows Server Update Services**. První synchronizaci lze spustit tím, že ponecháte zaškrtnuté políčko **Spustit počáteční synchronizaci**.

| ![](images/Cc708447.note(WS.10).gif)Poznámka                                                        |
|----------------------------------------------------------------------------------------------------------------------------------|
| Změny konfigurace provedené během synchronizace serveru nelze uložit. Počkejte na dokončení synchronizace a poté proveďte změny. |

![](images/Cc708447.3f774fd1-af87-47d8-8f50-a5d585687d70(WS.10).gif)

Následující postupy vysvětlují provedení výše uvedených kroků konfigurace prostřednictvím stránky **Možnosti** v konzole Správa služby WSUS:

-   Výběr produktů a klasifikací
-   Jazyky a soubory aktualizací

**Výběr produktů a klasifikací**
1.  Spusťte konzolu Správa služby WSUS: Klepněte na tlačítko **Start**, přejděte na příkaz **Všechny programy**, potom na položku **Nástroje pro správu** a pak klepněte na položku **Microsoft Windows Server Update Services**.

2.  V levém podokně u svého serveru WSUS vyberte položku **Možnosti**.

3.  V prostřední podokně vyberte možnost **Produkty a klasifikace**.

4.  Zobrazí se dialogové okno se dvěma kartami: **Produkty** a **Klasifikace**.

5.  Na kartě **Produkty** vyberte kategorii produktů nebo určitý produkt, pro který má tento server získávat aktualizace, případně vyberte možnost **Všechny produkty**.

6.  Na kartě **Klasifikace** vyberte požadované klasifikace aktualizací, případně vyberte možnost **Všechny klasifikace**.

7.  Vybrané možnosti uložíte klepnutím na tlačítko **OK**.

**Jazyky a soubory aktualizací**
1.  Na stránce **Možnosti** vyberte možnost **Jazyky a soubory aktualizací**.

2.  Zobrazí se dialogové okno se dvěma kartami: **Soubory aktualizací** a **Jazyky aktualizací**.

3.  Na kartě **Soubory aktualizací** můžete vybrat, zda se mají soubory aktualizací ukládat místně, nebo zda je mají všechny klientské počítače instalovat ze serveru Microsoft Update. Zvolíte-li možnost ukládání souborů aktualizací na tomto serveru, můžete si vybrat mezi stahováním pouze schválených aktualizací nebo stahováním souborů rychlé aktualizace.

4.  Na kartě **Jazyky aktualizací** můžete zvolit, zda chcete získávat aktualizace pro všechny jazyky (výchozí nastavení) nebo pouze pro určené jazyky. Má-li server WSUS servery pro příjem dat, budou tyto servery získávat aktualizace pouze v jazycích určených serverem pro odesílání dat.

5.  Nastavení uložíte klepnutím na tlačítko **OK**.

Po konfiguraci připojení k síti můžete stahovat aktualizace prostřednictvím synchronizace serveru WSUS.

Synchronizace zahrnuje kontaktování serveru Microsoft Update serverem WSUS. Po navázání kontaktu určí server WSUS, zda jsou od poslední synchronizace k dispozici nějaké nové aktualizace. Jelikož nyní jde o první synchronizaci serveru WSUS, jsou všechny aktualizace k dispozici a připraveny ke schválení pro instalaci. Počáteční synchronizace může trvat poměrně dlouho.

| ![](images/Cc708447.note(WS.10).gif)Poznámka                                                                                             |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Tento dokument popisuje synchronizaci s výchozím nastavením, ale služba WSUS zahrnuje možnosti, které umožňují minimalizovat použití šířky pásma během synchronizace. |

**Synchronizace serveru WSUS**
1.  V konzole Správa služby WSUS vyberte možnost **Synchronizace**.

2.  Klepněte pravým tlačítkem myši nebo přejděte do podokna **Akce** na pravé straně a potom klepněte na příkaz **Synchronizovat nyní**.

| ![](images/Cc708447.note(WS.10).gif)Poznámka                                                                                                                      |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Není-li zobrazeno podokno **Akce** na pravé straně konzoly, klepněte na panelu nástrojů konzoly na položku **Zobrazit**, klepněte na příkaz **Vlastní** a zaškrtněte políčko **Podokno Akce**. |

Po dokončení synchronizace klepněte na tlačítko **Aktualizace** na levém panelu. Zobrazíte tak seznam aktualizací.
