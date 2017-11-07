---
TOCTitle: Obnovení certifikátu serveru pro poskytování licencí
Title: Obnovení certifikátu serveru pro poskytování licencí
ms:assetid: 'affce9cf-8b46-4293-8e1c-ee06f2ca6537'
ms:contentKeyID: 18113402
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747636(v=WS.10)'
---

Obnovení certifikátu serveru pro poskytování licencí
====================================================

Provedení tohoto postupu vyžaduje, aby byl uživatel místně přihlášen k webu pro správu v rámci uživatelského účtu, který je členem skupiny Administrators v počítači, k němuž získává přístup. Uvedený postup mohou provést také členové skupiny Domain Admins. Z hlediska zabezpečení je nejvhodnější při provádění tohoto postupu použít příkaz **Spustit jako**.

Chcete-li otevřít webovou stránku **Globální správa**, klepněte na tlačítko **Start**, přejděte na příkaz **Všechny programy**, přejděte na položku **Služba RMS v systému Windows** a klepněte na položku **Správa služby RMS v systému Windows**.

Pokud jste zvolili obnovení v režimu offline a používáte počítač rozšířeného zabezpečení prohlížeče, například počítač se systémem Windows Server 2003 nebo Windows XP s aktualizací Service Pack 2, nezapomeňte za účelem připojení k Internetu a vyžádání certifikátu serveru pro poskytování licencí přidat adresu URL webu služby Enrollment Services do zóny důvěryhodných serverů, aby bylo možné daný certifikát stáhnout. Jedná se o následující adresu URL: https://activation.drm.microsoft.com.

Jestliže používáte zápis v režimu offline, musí mít počítač, který používáte k odeslání žádosti o zápis do služby Microsoft Enrollment Services, v úložišti certifikátů nainstalován certifikační úřad GTE Cyber Trust Root. Tento certifikační úřad je ve výchozím nastavení počítačů se systémem Windows Server 2003 považován za důvěryhodný. Pokud počítač používá jinou verzi systému Windows, můžete nastavit důvěryhodnost tohoto certifikačního úřadu instalací nejnovějších aktualizací certifikátů ze služby Windows Update.

Obnovení certifikátu serveru pro poskytování licencí
----------------------------------------------------

#### Obnovení certifikátu serveru pro poskytování licencí

1.  Otevřete stránku **Globální správa** a klepněte na položku **Spravovat službu RMS na tomto webu** u webu, na kterém chcete obnovit certifikát.

2.  Na stránce **Správa** klepněte v části **Prostředky clusteru** na tlačítko **Obnovit**. Zobrazí se dialogové okno Obnovit.

3.  Pokud je server připojen k Internetu, vyberte možnost **Online** a klepnutím na tlačítko **Obnovit** automaticky obnovte certifikát serveru pro poskytování licencí.

4.  Jestliže server k Internetu připojen není, vyberte možnost **Offline** a klepněte na tlačítko **Exportovat**. Zobrazí se dialogové okno **Stažení souboru**.

5.  Klepněte na tlačítko **Uložit**. Zobrazí se dialogové okno **Uložit jako**.

    | ![](images/Cc747636.note(WS.10).gif)Poznámka                                                                                                          |
    |------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | V dialogovém okně **Stažení souboru** neklepejte na tlačítko **Otevřít**. Při klepnutí na tlačítko **Otevřít** se zobrazí chybová zpráva a soubor s žádostí o zápis nebude uložen. |

6.  Klepnutím na tlačítko **Uložit** exportujte požadavek na obnovení do souboru. Ve výchozím nastavení bude soubor uložen na plochu pod názvem *název\_serveru*RenewalRequest.xml, kde hodnota *název\_serveru* bude nahrazena názvem serveru RMS. Výběrem požadovaného umístění v rozevíracím seznamu Uložit do můžete soubor uložit jinam. Zadáním nového názvu do pole **Název souboru** můžete také změnit výchozí název souboru.

7.  Po uložení souboru s požadavkem na obnovení se zobrazí dialogové okno **Stahování dokončeno**. Klepnutím na tlačítko **Otevřít** můžete zobrazit kód XML v souboru, neprovádějte však žádné změny. Chcete-li otevřít složku, ve které je soubor uložen, klepněte na tlačítko **Otevřít složku**. Po kontrole souboru a ověření jeho umístění klepněte na tlačítko **Zavřít**.

8.  Přesuňte soubor s požadavkem na obnovení ze serveru na počítač připojený k Internetu a přejděte na web služby (https://go.microsoft.com/fwlink/?LinkId=25828).

9.  Podle pokynů na tomto webu získejte certifikát serveru pro poskytování licencí.

10. Přesuňte uvedený certifikát zpět na tento server kořenové certifikace.

11. V části **Cluster** klepněte na položku **Obnovit**. Zobrazí se dialogové okno **Obnovit**.

12. V dialogovém okně **Obnovit** klepněte na tlačítko **Procházet**, vyhledejte stažený certifikát serveru pro poskytování licencí a klepněte na tlačítko **Importovat**.

13. Klepnutím na tlačítko **Ano** potvrďte import tohoto certifikátu.

14. Po úspěšném obnovení certifikátu serveru pro poskytování licencí se v části **Prostředky clusteru** zobrazí jeho nové datum vypršení platnosti.

Další informace o obnovení certifikátů serveru pro poskytování licencí získáte v tomto tématu v části [Správa certifikátů serveru pro poskytování licencí](https://technet.microsoft.com/549979ad-13ee-4abc-8281-3e002a5a9561) uvedené již dříve.
