---
TOCTitle: 'Krok 4: Konfigurace aktualizací a synchronizace'
Title: 'Krok 4: Konfigurace aktualizací a synchronizace'
ms:assetid: 'deeaa7e1-9b50-45cb-9537-d75f70de3405'
ms:contentKeyID: 21741208
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Dd939924(v=WS.10)'
---

Krok 4: Konfigurace aktualizací a synchronizace
===============================================

Tato část popisuje způsob konfigurace sady aktualizací, které chcete stáhnout pomocí aktualizace Windows Server Update Services 3.0 Service Pack 2 (WSUS 3.0 SP2).

Krok 4 – postupy
----------------

Tyto postupy lze provést pomocí průvodce konfigurací služby WSUS nebo pomocí konzoly pro správu služby WSUS.

1.  Uložení a stažení informací o nadřazeném serveru (serveru pro odesílání dat) a proxy serveru
2.  Volba jazyka aktualizací
3.  Výběr produktů, pro které chcete získávat aktualizace
4.  Volba klasifikací aktualizací
5.  Určení plánu synchronizace pro tento server

Po konfiguraci připojení k síti můžete stahovat aktualizace prostřednictvím synchronizace serveru WSUS. Synchronizace je zahájena při kontaktování služby Microsoft Update serverem WSUS. Po navázání kontaktu určí server WSUS, zda jsou od poslední synchronizace k dispozici nějaké nové aktualizace. Při první synchronizaci serveru WSUS jsou k dispozici všechny aktualizace a jsou připraveny ke schválení k instalaci. Počáteční synchronizace může trvat dlouho.

Postupy v této části popisují synchronizaci s výchozími nastaveními. Aktualizace WSUS 3.0 SP2 také zahrnuje možnosti, které umožňují minimalizovat během synchronizace použití šířky pásma.

Použití průvodce konfigurací služby Windows Server Update Services
------------------------------------------------------------------

V postupech kroku 3 jste dokončili konfiguraci nadřazeného serveru a proxy serveru. Tato další sada postupů začíná na stránce **Připojit k serveru pro odesílání dat** daného průvodce konfigurací.

**Uložení a stažení informací o nadřazeném serveru a proxy serveru**
1.  Na stránce Připojit k nadřazenému serveru v průvodci konfigurací klikněte na tlačítko **Spustit připojování**. Tímto způsobem budou uložena a odeslána vaše nastavení a shromážděny informace o dostupných aktualizacích.

2.  Během připojování bude dostupné tlačítko **Zastavit připojování**. Dojde-li problémům s připojením, klikněte na tlačítko **Zastavit připojování**, odstraňte problémy a znovu spusťte připojení.

3.  Po úspěšném dokončení stahování klikněte na tlačítko **Další**.

**Volba jazyků aktualizací**
1.  Stránka Vybrat jazyky umožňuje získat aktualizace ze všech jazyků nebo z určité dílčí sady jazyků. Výběrem jen dílčí sady jazyků lze uspořit místo na disku, je ale důležité vybrat všechny jazyky, které budou potřebovat klienti tohoto serveru WSUS.

    Chcete-li stahovat aktualizace pouze pro konkrétní jazyky, vyberte možnost **Stahovat aktualizace pouze v těchto jazycích** a vyberte jazyky, pro které chcete aktualizace.

2.  Klikněte na tlačítko **Další**.

**Volba produktů aktualizací**
1.  Stránka Vybrat produkty umožňuje určit produkty, pro které chcete aktualizace. Můžete vybrat kategorie produktů (například Windows) nebo určité produkty (například Windows Server 2008). Výběrem kategorie produktů vyberete všechny produkty v příslušné kategorii.

2.  Klikněte na tlačítko **Další**.

**Volba klasifikací aktualizací**
1.  Stránka Vybrat klasifikace umožňuje určit klasifikace aktualizací, které chcete získávat. Vyberte všechny klasifikace nebo dílčí sadu.

2.  Klikněte na tlačítko **Další**.

**Konfigurace plánu synchronizace**
1.  Na stránce Nastavit plán synchronizace můžete zvolit, zda chcete provést synchronizaci ručně nebo automaticky.

    Pokud vyberete možnost **Synchronizovat ručně**, budete muset spustit proces synchronizace z konzoly pro správu služby WSUS.

    Pokud vyberete možnost **Synchronizovat automaticky**, bude se server WSUS synchronizovat v nastavených intervalech. Nastavte čas **První synchronizace** a určete **Počet synchronizací za den**, které má tento server provést. Pokud například určíte, že za den mají proběhnout čtyři synchronizace se začátkem ve 3:00, dojde k synchronizaci ve 3:00, 9:00, 15:00 a 21:00.

2.  Klikněte na tlačítko **Další**.

3.  Konzolu pro správu služby WSUS lze spustit tím, že na závěrečné stránce ponecháte zaškrtnuté políčko **Spustit modul snap-in Správa služby Windows Server Update Services**. První synchronizaci lze spustit tím, že ponecháte zaškrtnuté políčko **Spustit počáteční synchronizaci**.

4.  Klikněte na tlačítko **Dokončit**.

 
    <table style="border:1px solid black;">
    <colgroup>
    <col width="100%" />
    </colgroup>
    <thead>
    <tr class="header">
    <th><img src="images/Dd939924.Important(WS.10).gif" />Důležité</th>
    </tr>
    </thead>
    <tbody>
    <tr class="odd">
    <td style="border:1px solid black;">Změny konfigurace provedené během synchronizace serveru nelze uložit. Počkejte na dokončení synchronizace a poté proveďte změny.
    </td>
    </tr>
    </tbody>
    </table>
 

Použití konzoly pro správu služby WSUS
--------------------------------------

Následující postupy vysvětlují způsob provedení kroků konfigurace pomocí konzoly pro správu služby WSUS.

**Výběr produktů a klasifikací aktualizací**
1.  V panelu **Možnosti** klikněte na položku **Produkty a klasifikace**. Zobrazí se dialogové okno s kartami **Produkty** a **Klasifikace**.

2.  Na kartě **Produkty** vyberte kategorii produktů nebo určité produkty, pro které má tento server získávat aktualizace, případně vyberte možnost **Všechny produkty**.

3.  Na kartě **Klasifikace** vyberte požadované klasifikace aktualizací, případně vyberte možnost **Všechny klasifikace**.

4.  Vybrané možnosti uložíte kliknutím na tlačítko **OK**.

**Výběr souborů a jazyků aktualizací**
1.  V panelu **Možnosti** klikněte na tlačítko **Jazyky a soubory aktualizací**. Zobrazí se dialogové okno s kartami **Soubory aktualizací** a **Jazyky aktualizací**.

2.  Na kartě **Soubory aktualizací** můžete vybrat, zda se mají **Ukládat soubory aktualizací místně na tomto serveru**, nebo zda je mají všechny klientské počítače instalovat ze služby Microsoft Update. Pokud se rozhodnete ukládat soubory aktualizací na tomto serveru, můžete se rozhodnout mezi stahováním pouze schválených aktualizací nebo stahováním souborů rychlé aktualizace.

3.  Pokud jsou soubory aktualizací ukládány místně, vyberte na kartě **Jazyky aktualizací** možnost **Stáhnout aktualizace pro všechny jazyky** (výchozí nastavení) nebo možnost **Stahovat aktualizace pouze v určených jazycích**. Má-li server WSUS podřízené servery, budou tyto servery získávat aktualizace pouze v jazycích určených nadřízeným serverem.

4.  Nastavení uložíte kliknutím na tlačítko **OK**.

**Postup synchronizace serveru WSUS**
1.  V panelu **Možnosti** klikněte na položku **Plán synchronizace**.

2.  Na kartě **Plán synchronizace** můžete zvolit, zda chcete provést synchronizaci ručně nebo automaticky.

    Pokud vyberete možnost **Synchronizovat ručně**, budete muset spustit proces synchronizace z konzoly pro správu služby WSUS.

    Pokud vyberete možnost **Synchronizovat automaticky**, bude se server WSUS synchronizovat v nastavených intervalech. Nastavte čas **První synchronizace** a určete **Počet synchronizací za den**, které má tento server provést. Pokud například určíte, že za den mají proběhnout čtyři synchronizace se začátkem ve 3:00, dojde k synchronizaci ve 3:00, 9:00, 15:00 a 21:00.

3.  Vybrané možnosti uložíte kliknutím na tlačítko **OK**.

4.  V navigačním podokně konzoly pro správu služby WSUS vyberte možnost **Synchronizace**.

5.  Klikněte pravým tlačítkem myši nebo přejděte do podokna **Akce** na pravé straně a potom klikněte na příkaz **Synchronizovat nyní**.

    Není-li zobrazeno podokno **Akce** na pravé straně konzoly, klikněte na panelu nástrojů konzoly na položku **Zobrazit**, klikněte na příkaz **Vlastní** a zaškrtněte políčko **Podokno Akce**.

6.  Po dokončení synchronizace klikněte na tlačítko **Aktualizace** na levém panelu. Zobrazíte tak seznam aktualizací.

Další krok
----------

[Krok 5: Konfigurace aktualizací klienta](https://technet.microsoft.com/5ae60ead-3e94-456c-a692-c0f193ea5d5a)

Další zdroje informací
----------------------

[Podrobný průvodce aktualizací Windows Server Update Services 3.0 SP2](https://technet.microsoft.com/4b504edc-93b3-45b0-a7e8-d0107f1a4442)
