---
TOCTitle: 'Krok 5: Konfigurace aktualizací klienta'
Title: 'Krok 5: Konfigurace aktualizací klienta'
ms:assetid: '5ae60ead-3e94-456c-a692-c0f193ea5d5a'
ms:contentKeyID: 21741106
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Dd939830(v=WS.10)'
---

Krok 5: Konfigurace aktualizací klienta
=======================================

Instalační program služby WSUS v aktualizaci Windows Server Update Services 3.0 (WSUS 3.0 SP2) automaticky konfiguruje službu ISS tak, aby distribuovala nejnovější verzi automatických aktualizací pro každý klientský počítač, který kontaktuje server WSUS.

Nejvhodnější způsob konfigurace automatických aktualizací závisí na síťovém prostředí. V prostředí, které používá adresářovou službu Active Directory®, je možné použít stávající objekt zásad skupiny (GPO) založený na doméně nebo vytvořit nový objekt GPO. V prostředí bez služby Active Directory použijte místní objekt zásad skupiny. V tomto kroku nakonfigurujete automatické aktualizace a poté nasměrujete klientské počítače na server WSUS.

U následujících postupů se předpokládá, že ve vaší síti je spuštěna služba Active Directory. U těchto postupů se také předpokládá znalost zásad skupiny a jejich používání ke správě sítě.

Další informace o zásadách skupiny naleznete na webu Group Policy Tech Center [http://go.microsoft.com/fwlink/?LinkID=47375](http://go.microsoft.com/fwlink/?linkid=47375) (tato stránka může být v angličtině).

 
-

Krok 5 – postupy
----------------

V kroku 4 jste dokončili konfiguraci aktualizací, které chcete stáhnout. Tuto sadu postupů použijte ke konfiguraci automatických aktualizací pro klientské počítače.

1.  Konfigurace automatických aktualizací v zásadách skupiny
2.  Nasměrování klientského počítače na server WSUS
3.  Ruční spuštění rozpoznávání serverem WSUS

První dva postupy budou provedeny na vámi zvoleném objektu GPO založeném na doméně, třetí postup bude proveden v příkazovém řádku klientského počítače.

**Konfigurace automatických aktualizací**
1.  V konzole pro správu zásad skupiny (GPMC) přejděte na objekt GPO, na kterém chcete konfigurovat službu WSUS, a potom klikněte na možnost **Upravit**.

2.  V konzole GPMC rozbalte položku **Konfigurace počítače**, rozbalte položku **Šablony pro správu**, rozbalte položku **Součásti systému Windows** a potom klikněte na položku **Windows Update**.

3.  V podokně podrobností dvakrát klikněte na položku **Konfigurace automatických aktualizací**.

4.  Klikněte na přepínač **Povoleno** a potom na jednu z následujících možností:

    -   **Upozorňovat na stažení i instalaci**. Tato možnost upozorňuje přihlášeného uživatele s pověřením správce před stažením a před instalací aktualizací.
    -   **Automaticky stahovat, upozorňovat na instalaci**. Tato možnost automaticky zahajuje stahování aktualizací a potom upozorní přihlášeného uživatele s pověřením správce před instalací aktualizací.
    -   **Automaticky stahovat a plánovat instalaci**. Tato možnost automaticky zahájí stahování aktualizací a poté nainstaluje aktualizace ve vámi zadaném dni a čase.
    -   **Povolit místnímu správci změnit nastavení**. Tato možnost umožní místním správcům používat automatické aktualizace v Ovládacích panelech k výběru možností konfigurace. Mohou si například vybrat vlastní plánovanou dobu instalace. Místní správci nemohou zakázat automatické aktualizace.

5.  Klikněte na tlačítko **OK**.

**Nasměrování klientského počítače na server WSUS**
1.  V podokně podrobností **Windows Update** klikněte dvakrát na položku **Určení umístění intranetového serveru služby Microsoft Update**.

2.  Klikněte na přepínač **Povoleno** a zadejte adresu HTTP URL stejného serveru WSUS do pole **Nastavení intranetového serveru pro zjišťování aktualizací** a do pole **Nastavení intranetového serveru pro statistiku**. Do obou polí zadejte například *http://název\_serveru* a potom klikněte na tlačítko **OK**.

 
> [!NOTE]
> Používáte-li místní objekt zásad skupiny ke směrování počítače na server WSUS, projeví se toto nastavení ihned a tento počítač po krátké době zobrazí v konzole pro správu služby WSUS. Tento proces je možné zrychlit ručním spuštěním cyklu rozpoznávání.
 

Poté, co klientský počítač nastavíte, bude trvat několik minut, než se zobrazí na stránce **Počítače** v konzole pro správu služby WSUS. V případě klientských počítačů konfigurovaných pomocí objektu zásad skupiny založeného na doméně bude aktualizace zásad skupiny (tedy použití jakýchkoli nových nastavení zásad v klientském počítači) trvat asi 20 minut. Při výchozím nastavení se zásady skupiny aktualizují na pozadí každých 90 minut s náhodným posunem od 0 do 30 minut. Pokud chcete aktualizovat zásady skupiny dříve, můžete v klientském počítači přejít do příkazového řádku a zadat příkaz **gpupdate /force**.

U klientských počítačů konfigurovaných pomocí místního objektu zásad skupiny se zásady skupiny použijí ihned a aktualizace bude trvat asi 20 minut.

Pokud spustíte rozpoznávání ručně, nemusíte čekat 20 minut, než bude klientský počítač kontaktovat server WSUS.

**Ruční spuštění rozpoznávání serverem WSUS**
1.  V klientském počítači klikněte na tlačítko **Start** a potom klikněte na příkaz **Spustit**.

2.  Do pole **Otevřít** zadejte příkaz **cmd** a klikněte na tlačítko **OK**.

3.  Na příkazovém řádku zadejte příkaz **wuauclt.exe /detectnow**. Tato možnost příkazového řádku dává pokyn automatickým aktualizacím, aby ihned kontaktovaly server WSUS.

Další krok
----------

[Krok 6: Konfigurace skupin počítačů](https://technet.microsoft.com/70518732-2179-4e41-9609-7f9999867f41)

Další zdroje informací
----------------------

[Podrobný průvodce aktualizací Windows Server Update Services 3.0 SP2](https://technet.microsoft.com/4b504edc-93b3-45b0-a7e8-d0107f1a4442)
