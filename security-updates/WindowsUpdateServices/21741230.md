---
TOCTitle: 'Krok 1: Potvrzení instalačních požadavků aktualizace WSUS 3.0 SP2'
Title: 'Krok 1: Potvrzení instalačních požadavků aktualizace WSUS 3.0 SP2'
ms:assetid: 'ec01bd75-5def-4899-8cee-ddab827bbd83'
ms:contentKeyID: 21741230
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Dd939916(v=WS.10)'
---

Krok 1: Potvrzení instalačních požadavků aktualizace WSUS 3.0 SP2
=================================================================

Před instalací nebo upgradem na aktualizaci Windows Server Upgrade Services 3.0 Service Pack 2 (WSUS 3.0 SP2) potvrďte, že server i klientské počítače splňují požadavky na systém aktualizace WSUS 3.0 SP2 a že máte potřebná oprávnění k dokončení instalace.

Požadavky na hardware a software serveru pro instalaci aktualizace WSUS 3.0 SP2
-------------------------------------------------------------------------------

1.  Potvrďte, že server splňuje systémové požadavky aktualizace WSUS 3.0 SP2 na hardware, operační systém a další požadovaný software. Požadavky na systém jsou uvedeny v Poznámkách k verzi aktualizace WSUS 3.0 SP2 na adrese [http://go.microsoft.com/fwlink/?LinkId=139840](http://go.microsoft.com/fwlink/?linkid=139840). Pokud k instalaci serveru WSUS 3.0 SP2 používáte Správce serveru, můžete potvrdit, že splňujete požadavky na systém, pomocí postupu uvedeného v části Příprava na instalaci aktualizace WSUS 3.0 SP2.
2.  Pokud instalujete role nebo aktualizujete software, který po dokončení instalace vyžaduje restartování serveru, restartujte server před instalací aktualizace WSUS 3.0 SP2.

Požadavky na software klienta
-----------------------------

Automatické aktualizace jsou klientem služby WSUS 3.0. Automatické aktualizace nemají kromě připojení k síti žádné další požadavky na hardware.

1.  Potvrďte, že počítač, ve kterém instalujete automatické aktualizace, splňuje systémové požadavky aktualizace WSUS 3.0 SP2 pro klientské počítače. Požadavky na systém jsou uvedeny v Poznámkách k verzi aktualizace WSUS 3.0 SP2 na adrese [http://go.microsoft.com/fwlink/?LinkId=139840](http://go.microsoft.com/fwlink/?linkid=139840).
2.  Pokud instalujete aktualizace softwaru, které vyžadují restartování počítače, restartujte jej před instalací aktualizace WSUS 3.0 SP2.

Oprávnění
---------

Pro zadané uživatele a adresáře jsou vyžadována následující oprávnění:

1.  Účet NT Authority\\Network Service potřebuje mít oprávnění Úplné řízení pro následující adresáře, aby byl modul snap-in Správa služby WSUS zobrazen správně:
    -   %windir%\\Microsoft .NET\\Framework\\v2.0.50727\\Temporary ASP.NET Files
    -   %windir%\\Temp
2.  Potvrďte, že účet, který plánujete použít k instalaci aktualizace WSUS 3.0 SP2, je členem místní skupiny Administrators.

Příprava na instalaci aktualizace WSUS 3.0 SP2
----------------------------------------------

Pokud používáte systém Windows 7 nebo Windows Server 2008 SP2, můžete aktualizaci WSUS 3.0 SP2 nainstalovat ze Správce serveru. Pokud používáte jiný podporovaný operační systém nebo pokud instalujete pouze konzolu pro správu služby WSUS, přejděte k další části tohoto průvodce a nainstalujte aktualizaci WSUS 3.0 SP2 pomocí souboru WUSSetup.exe.

**Příprava na instalaci aktualizace WSUS 3.0 SP2 pomocí Správce serveru**
1.  Přihlaste se k serveru, na který chcete instalovat aktualizaci WSUS 3.0 SP2, pomocí účtu, který je členem místní skupiny Administrators.

2.  Klikněte na tlačítko **Start**, přejděte na položku **Nástroje pro správu** a klikněte na příkaz **Správce serveru**.

3.  V pravém podokně okna Správce serveru klikněte v části Souhrn rolí na možnost **Přidat role**.

4.  Zobrazí-li se stránka Než začnete, klikněte na tlačítko **Další**.

5.  Na stránce Vybrat role serveru potvrďte, že jsou vybrány možnosti **Aplikační server** a **Webový server (IIS)**. Pokud byly tyto možnosti vybrány, použijte zbývající část tohoto kroku a potvrďte, že požadované služby rolí byly vybrány. V opačném případě nainstalujte podle následujícího postupu aplikační server a webový server (IIS).

    1.  Na stránce Vybrat role serveru vyberte možnosti **Aplikační server** a **Webový server (IIS)**. Klikněte na tlačítko **Další**.
    2.  Pokud instalujete služby rolí aplikačního serveru, klikněte na stránce Aplikační server na tlačítko **Další**. Na stránce Služby rolí aplikačního serveru přijměte výchozí nastavení a potom klikněte na tlačítko **Další**.
    3.  Pokud instalujete webový server IIS, klikněte na stránce Webový server (IIS) na tlačítko **Další**. Na stránce Služby rolí webového serveru (IIS) vyberte kromě výchozích nastavení možnosti **ASP.NET**, **Ověřování systému Windows**, **Komprese dynamického obsahu** a **Kompatibilita správy služby IIS 6**. Pokud se zobrazí okno Průvodce přidáním rolí, klikněte na tlačítko **Přidat požadované služby rolí**. Klikněte na tlačítko **Další**.
    4.  Na stránce Potvrdit vybrané možnosti instalace klikněte na tlačítko **Nainstalovat**.
    5.  Na stránce Výsledky instalace se přesvědčte, že se pro služby rolí, které jste v tomto kroku instalovali, zobrazí zpráva potvrzující úspěšnou instalaci, a potom klikněte na tlačítko **Zavřít**.

Další krok
----------

[Krok 2: Instalace serveru WSUS nebo konzoly pro správu](https://technet.microsoft.com/6db6fcb0-c55d-43b9-9b07-4040c6267759)

Další zdroje informací
----------------------

[Podrobný průvodce aktualizací Windows Server Update Services 3.0 SP2](https://technet.microsoft.com/4b504edc-93b3-45b0-a7e8-d0107f1a4442)
