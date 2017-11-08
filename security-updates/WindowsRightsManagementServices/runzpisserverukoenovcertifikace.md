---
TOCTitle: Ruční zápis serveru kořenové certifikace
Title: Ruční zápis serveru kořenové certifikace
ms:assetid: 'aecdebb5-b28b-4b58-937a-392bb6ce9643'
ms:contentKeyID: 18113481
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747727(v=WS.10)'
---

Ruční zápis serveru kořenové certifikace
========================================

Provedení tohoto postupu vyžaduje, aby byl uživatel místně přihlášen k webu pro správu v rámci uživatelského účtu, který je členem skupiny Administrators v počítači, k němuž získává přístup. Uvedený postup mohou provést také členové skupiny Domain Admins. Z hlediska zabezpečení je nejvhodnější při provádění tohoto postupu použít příkaz Spustit jako.

Chcete-li otevřít webovou stránku **Globální správa**, klepněte na tlačítko **Start**, přejděte na příkaz **Všechny programy**, přejděte na položku **Služba RMS v systému Windows** a klepněte na položku **Správa služby RMS v systému Windows**.

Pokud jste zvolili zápis offline, měli byste zajistit, aby se klienti RMS nepřipojovali k serveru RMS za účelem získání licencí, dokud nebude proveden zápis. Jestliže se klienti pokusí připojit k serveru RMS, který není zapsán, nastaví webové služby chybový stav a nebude je možné používat. Pokud nemůžete zajistit, aby se klienti k serveru RMS nepřipojovali, bude nejvhodnější po provedení zápisu obnovit službu IIS. Tímto způsobem odstraníte případné chyby.

Pokud jste vybrali zápis offline a používáte počítač s konfigurací rozšířeného zabezpečení prohlížeče, například počítač se systémem Windows Server 2003 nebo Windows XP Service Pack 2, nezapomeňte za účelem připojení k Internetu a vyžádání certifikátu serveru pro poskytování licencí přidat adresu URL webu služby Enrollment Services do zóny důvěryhodných serverů, aby bylo možné daný certifikát stáhnout. Jedná se o následující adresu URL: https://activation.drm.microsoft.com.

Jestliže používáte zápis v režimu offline, musí mít počítač, který používáte k odeslání žádosti o zápis do služby Microsoft Enrollment Services, v úložišti certifikátů nainstalován certifikační úřad GTE Cyber Trust Root. Tento certifikační úřad je ve výchozím nastavení počítačů se systémem Windows Server 2003 považován za důvěryhodný. Pokud počítač používá jinou verzi systému Windows, můžete nastavit důvěryhodnost tohoto certifikačního úřadu instalací nejnovějších aktualizací certifikátů ze služby Windows Update.

Ruční zápis serveru kořenové certifikace
----------------------------------------

#### Ruční zápis serveru kořenové certifikace

1.  Po instalaci služby RMS na serveru, který má být serverem kořenové certifikace, otevřete stránku **Globální správa** a u webu, na který chcete importovat certifikát serveru pro poskytování licencí pro server kořenové certifikace, klepněte na položku **Spravovat službu RMS na tomto webu**.

2.  V části **Prostředky clusteru** klepněte na položku **Zapsat**. Zobrazí se dialogové okno **Zapsat**.

3.  Vyberte možnost **Offline** a klepněte na tlačítko **Exportovat**. Zobrazí se dialogové okno **Stažení souboru**.

4.  Klepněte na tlačítko **Uložit**. Zobrazí se dialogové okno **Uložit jako**.

    | ![](images/Cc747727.note(WS.10).gif)Poznámka                                                                                                          |
    |------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | V dialogovém okně **Stažení souboru** neklepejte na tlačítko **Otevřít**. Při klepnutí na tlačítko **Otevřít** se zobrazí chybová zpráva a soubor s žádostí o zápis nebude uložen. |

5.  Klepnutím na tlačítko **Uložit** exportujte žádost o zápis do souboru. Ve výchozím nastavení bude soubor uložen na plochu pod názvem *název\_serveru*EnrollRequest.xml, kde hodnota *název\_serveru* bude nahrazena názvem serveru RMS. Výběrem požadovaného umístění v rozevíracím seznamu **Uložit do** můžete soubor uložit jinam. Zadáním nového názvu do pole **Název souboru** můžete také změnit výchozí název souboru.

6.  Po uložení souboru s žádostí o zápis se zobrazí dialogové okno **Stahování dokončeno**. Klepnutím na tlačítko **Otevřít** můžete zobrazit kód XML v souboru, neprovádějte však žádné změny. Chcete-li otevřít složku, ve které je soubor uložen, klepněte na tlačítko **Otevřít složku**. Po kontrole souboru a ověření jeho umístění klepněte na tlačítko **Zavřít**.

7.  Přesuňte soubor s požadavkem na zápis ze serveru na počítač připojený k Internetu a přejděte na [web služby Enrollment Services]() (https://go.microsoft.com/fwlink/?LinkId=25828).

8.  Podle pokynů na tomto webu získejte certifikát serveru pro poskytování licencí.

9.  Přesuňte uvedený certifikát zpět na tento server kořenové certifikace.

10. V části **Prostředky clusteru** klepněte na položku **Zapsat**. Zobrazí se dialogové okno **Zapsat**.

11. V dialogovém okně **Zapsat** klepněte na tlačítko **Procházet**, vyhledejte stažený certifikát serveru pro poskytování licencí a klepněte na tlačítko **Importovat**.

12. Klepnutím na tlačítko **Ano** potvrďte import tohoto certifikátu.

13. Certifikát se zobrazí v části **Prostředky clusteru**.
