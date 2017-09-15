---
TOCTitle: 'Krok 5: Konfigurace automatických aktualizací'
Title: 'Krok 5: Konfigurace automatických aktualizací'
ms:assetid: '5da6d10a-6ff1-4de8-b53a-4893bf8bd9fa'
ms:contentKeyID: 18126448
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc720532(v=WS.10)'
---

Krok 5: Konfigurace automatických aktualizací
=============================================

Klientské počítače se službou WSUS vyžadují kompatibilní verzi automatických aktualizací. Instalace služby WSUS automaticky konfiguruje službu IIS na distribuci poslední verze automatických aktualizací do jednotlivých klientských počítačů, které kontaktují server WSUS.

Nejvhodnější způsob konfigurace automatických aktualizací závisí na vašem síťovém prostředí. V prostředí se službou Active Directory je možné použít objekt zásad skupiny (GPO) založený na doméně. V prostředí bez služby Active Directory použijte místní objekt zásad skupiny. Ať již používáte místní objekt zásad skupiny nebo objekt zásad skupiny založený na doméně, je třeba nasměrovat klientské počítače na server WSUS a potom nakonfigurovat automatické aktualizace.

U následujících pokynů se předpokládá, že ve vaší síti běží služba Active Directory. U těchto postupů se také předpokládá, že znáte zásady skupiny a používáte je k řízení sítě. Je třeba, abyste pro nastavení služby WSUS vytvořili nový objekt zásad skupiny a propojili tento objekt s doménou.

Další informace o zásadách skupiny naleznete na webu odborného centra zásad skupiny ([http://go.microsoft.com/fwlink/?LinkID=47375](http://go.microsoft.com/fwlink/?linkid=47375), tato stránka může být v angličtině).

**Krok 5 obsahuje následující postupy**:

-   přidání šablony pro správu služby WSUS,
-   konfigurace automatických aktualizací,
-   směrování klientského počítače na server WSUS,
-   ruční spuštění rozpoznávání serverem WSUS.

První tři postupy proveďte na objektu zásad skupiny založeného na doméně. Bude třeba vytvořit nový objekt zásad skupiny nebo použít již existující objekt. Pokud pro správu objektů zásad skupiny používáte konzolu správy zásad skupiny (GPMC), přejděte na objekt zásad skupiny, který chcete upravit, a potom klepněte na tlačítko **Upravit**.

V případě, že chcete zobrazit nastavení zásad pro správu služby WSUS, je nutné, aby v modulu snap-in Editor objektů Zásady skupiny byl přidán soubor šablony pro správu služby WSUS (wuau.adm). Soubor wuau.adm je ve výchozím nastavení vydán s operačním systémem, a měl by tedy již být v modulu snap-in Editor objektů Zásady skupiny.

**Přidání šablony pro správu WSUS**
1.  V modulu snap-in Editor objektů Zásady skupiny klepněte na jeden z uzlů **Šablony pro správu**.

2.  V nabídce **Akce** klepněte na příkaz **Přidat nebo odebrat šablony** a potom na tlačítko **Přidat**.

3.  V dialogovém okně **Šablony zásad** klepněte na položku **wuau.adm** a potom na tlačítko **Otevřít**.

4.  V dialogovém okně **Přidat nebo odebrat šablony** klepněte na tlačítko **Zavřít**.

**Konfigurace automatických aktualizací**
1.  V modulu snap-in Editor objektů Zásady skupiny rozbalte položku **Konfigurace počítače**, dále položku **Šablony pro správu**, položku **Součásti systému Windows** a potom klepněte na položku **Windows Update**.

2.  V podokně podrobností poklepejte na položku **Konfigurace automatických aktualizací**.

3.  Klepněte na přepínač **Povoleno** a potom na jednu z následujících možností:

    -   **Upozorňovat na stažení i instalaci**: Tato možnost upozorňuje přihlášeného uživatele s pověřením správce před stažením a před instalací na aktualizace.
    -   **Automaticky stahovat, upozorňovat na instalaci**: Tato možnost automaticky zahajuje stahování aktualizací a potom upozorní přihlášeného uživatele s pověřením správce před instalací aktualizací.
    -   **Automaticky stahovat a plánovat instalaci**: Pokud je u automatických aktualizací nakonfigurováno provádění plánované instalace, je třeba také nastavit den a čas opakované plánované instalace.
    -   **Povolit místnímu správci změnit nastavení**: S touto možností mohou místní správci používat ovládací panel Automatické aktualizace a vybrat možnosti konfigurace. Mohou si například vybrat vlastní plánovanou dobu instalace. Místní správci nemohou zakázat automatické aktualizace.

4.  Klepněte na tlačítko **OK**.

| ![](images/Cc720532.note(WS.10).gif)Poznámka                                                                                                      |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Nastavení **Povolit místnímu správci změnit nastavení** se zobrazí pouze tehdy, pokud je funkce automatických aktualizací aktualizována na verzi kompatibilní se službou WSUS. |

**Směrování klientského počítače na server WSUS**
1.  V modulu snap-in Editor objektů Zásady skupiny rozbalte položku **Konfigurace počítače**, dále položku **Šablony pro správu**, položku **Součásti systému Windows** a potom klepněte na položku **Windows Update**.

2.  V podokně podrobností poklepejte na položku **Určení umístění intranetového serveru služby Microsoft Update**.

3.  Klepněte na přepínač **Povoleno** a zadejte adresu HTTP URL stejného serveru WSUS do pole **Nastavení intranetového serveru pro zjišťování aktualizací** a do pole **Nastavení intranetového serveru pro statistiku**. Do obou polí zadejte například *http://název\_serveru* a potom klepněte na tlačítko **OK**.

| ![](images/Cc720532.note(WS.10).gif)Poznámka                                                                                                                                                                                                     |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Používáte-li místní objekt zásad skupiny ke směrování tohoto počítače na server WSUS, projeví se toto nastavení ihned a tento počítač by se měl po krátké době zobrazit v konzole pro správu služby WSUS. Tento proces je možné zrychlit ručním spuštěním cyklu rozpoznávání. |

Poté, co klientský počítač nastavíte, bude trvat několik minut, než se zobrazí na stránce **Počítače** v konzole služby WSUS. V případě klientských počítačů konfigurovaných pomocí objektu zásad skupiny založeného na doméně bude aktualizace zásad skupiny (tedy použití jakýchkoli nových nastavení zásad v klientském počítači) trvat asi 20 minut. Při výchozím nastavení se zásady skupiny aktualizují na pozadí každých 90 minut s náhodným posunem od 0 do 30 minut. Pokud chcete obnovit zásady skupiny dříve, můžete v klientském počítači přejít na příkazový řádek a zadat následující příkaz: **gpupdate /force**.

U klientských počítačů konfigurovaných pomocí místního objektu zásad skupiny se zásady skupiny použijí ihned a aktualizace bude trvat asi 20 minut.

Po použití zásad skupiny je možné spustit rozpoznávání ručně. Pokud spustíte rozpoznávání ručně, nemusíte čekat 20 minut, než bude klientský počítač kontaktovat server WSUS.

**Ruční spuštění rozpoznávání serverem WSUS**
1.  V klientském počítači klepněte na tlačítko **Start** a potom klepněte na příkaz **Spustit**.

2.  Do pole **Otevřít** zadejte příkaz **cmd** a klepněte na tlačítko **OK**.

3.  Na příkazovém řádku zadejte příkaz **wuauclt.exe /detectnow**. Tato možnost příkazového řádku dává pokyn automatickým aktualizacím, aby ihned kontaktovaly server WSUS.
