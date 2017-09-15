---
TOCTitle: 'Krok 5: Aktualizace a konfigurace automatických aktualizací'
Title: 'Krok 5: Aktualizace a konfigurace automatických aktualizací'
ms:assetid: '4ac8d574-f48e-4d9d-86c9-9aeb0f57e750'
ms:contentKeyID: 18126523
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc720533(v=WS.10)'
---

Krok 5: Aktualizace a konfigurace automatických aktualizací
===========================================================

Klientské počítače se službou WSUS vyžadují kompatibilní verzi automatických aktualizací. Instalace služby WSUS automaticky konfiguruje službu IIS na distribuci poslední verze automatických aktualizací do jednotlivých klientských počítačů, které kontaktují server WSUS.

| ![](images/Cc720533.note(WS.10).gif)Poznámka                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| I když je možné většinu verzí automatických aktualizací směrovat na server WSUS a ty se budou automaticky samy aktualizovat na verzi kompatibilní se službou WSUS, nemůže se verze automatických aktualizací, která je součástí systému Windows XP, bez aktualizací Service Pack sama automaticky aktualizovat. Pokud máte systém Windows XP bez jakýchkoli aktualizací Service Pack ve vašem prostředí a nikdy jste nepoužívali službu Software Update Services (SUS), přečtěte si pokyny v dokumentu White Paper Deploying Microsoft Windows Server Update Services (Nasazení služby Microsoft Windows Server Update Services). |

Nejvhodnější způsob konfigurace automatických aktualizací závisí na vašem síťovém prostředí. V prostředí služby Active Directory je možné použít objekt zásad skupiny (GPO) založený na službě Active Directory. V prostředí jiném než Active Directory použijte objekt zásad místní skupiny. Ať používáte objekt zásad místní skupiny nebo objekt zásad skupiny uložený v řadiči domény, musíte směrovat klientské počítače na server WSUS a potom konfigurovat automatické aktualizace.

U následujících pokynů se předpokládá, že je ve vaší síti spuštěna služba Active Directory. U těchto postupů se také předpokládá, že jste již nastavili a znáte zásady skupiny a používáte je k řízení sítě. Je třeba, abyste vytvořili nový objekt zásad skupiny pro nastavení služby WSUS a propojili objekt zásad skupiny na úrovni domény.

Další informace o zásadách skupiny naleznete na stránce [Zásady skupiny](http://go.microsoft.com/fwlink/?linkid=47375) na adrese http://go.microsoft.com/fwlink/?LinkID=47375.

Krok 5 obsahuje následující postupy:

-   načtení šablony pro správu služby WSUS,
-   konfigurace automatických aktualizací,
-   směrování klientských počítačů na server WSUS,
-   ruční spuštění rozpoznávání v klientském počítači,

provedení dalších tří postupů u objektu zásad skupiny založeného na službě Active Directory.

**Přidání šablony pro správu WSUS**
1.  V editoru objektů zásad skupiny klepněte na jeden z uzlů **Šablony pro správu**.

2.  V nabídce **Akce** klepněte na příkaz **Přidat nebo odebrat šablony**.

3.  Klepněte na tlačítko **Přidat**.

4.  V dialogovém okně **Šablony zásad** klepněte na položku **wuau.adm** a potom na tlačítko **Otevřít**.

5.  V dialogovém okně **Přidat nebo odebrat šablony** klepněte na tlačítko **Zavřít**.

**Konfigurace chování automatických aktualizací**
1.  V editoru objektů zásad skupiny rozbalte položku **Konfigurace počítače**, dále položku **Šablony pro správu**, položku **Součásti systému Windows** a potom klepněte na položku **Windows Update**.

2.  V podokně podrobností poklepejte na položku **Konfigurace automatických aktualizací**.

3.  Klepněte na možnost **Povoleno** a potom na jednu z následujících možností:

    -   **Upozorňovat na stažení i instalaci:** Tato možnost upozorňuje přihlášeného uživatele s pověřením správce před stažením a před instalací na aktualizace.
    -   **Automaticky stahovat a upozorňovat na instalaci:** Tato možnost automaticky zahajuje stahování aktualizací a potom upozorní přihlášeného uživatele s pověřením správce před instalací aktualizací.
    -   **Automaticky stahovat a plánovat instalaci:** Pokud je u automatických aktualizací konfigurováno provádění plánované instalace, musíte také nastavit den a čas opakované plánované instalace.
    -   **Povolit místnímu správci výběr nastavení:** S touto možností mohou místní správci používat automatické aktualizace v Ovládacích panelech k výběru možnosti konfigurace podle vlastní volby. Mohou si například vybrat vlastní plánovanou dobu instalace. Místní správci nemohou zakazovat automatické aktualizace.

4.  Klepněte na tlačítko **OK**.

| ![](images/Cc720533.note(WS.10).gif)Poznámka                                                                                        |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Nastavení **Povolit místnímu správci výběr nastavení** se zobrazí pouze tehdy, pokud automatické aktualizace aktualizují samy sebe na verzi kompatibilní s WSUS. |

**Směrování klientského počítače na server WSUS**
1.  V editoru objektů zásad skupiny rozbalte položku **Konfigurace počítače**, dále položku **Šablony pro správu**, položku **Součásti systému Windows** a potom klepněte na položku **Windows Update**.

2.  V podokně podrobností poklepejte na položku **Určení umístění intranetového serveru služby Microsoft Update**.

3.  Klepněte na položku **Povoleno** a zadejte adresu HTTP URL stejného serveru WSUS do pole **Nastavení intranetové aktualizační služby pro rozpoznávání aktualizací** a do pole **Nastavení intranetového serveru pro statistiku**. Do obou polí zadejte například **http://***název\_serveru*.

4.  Klepněte na tlačítko **OK**.

| ![](images/Cc720533.note(WS.10).gif)Poznámka                                                                                                                                                                                                     |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Používáte-li objekt zásad místní skupiny ke směrování tohoto počítače na server WSUS, projeví se toto nastavení ihned a tento počítač by se měl zobrazit v konzole pro správu služby WSUS během 20 minut. Tento proces je možné zrychlit ručním spuštěním cyklu rozpoznávání. |

Poté, co klientský počítač nastavíte, bude trvat několik minut, než se zobrazí na stránce **Počítače** v konzole služby WSUS. Pro klientské počítače konfigurované s objektem skupiny zásad založeným na službě Active Directory bude trvat obnovení skupiny zásad skupiny (tedy použití jakéhokoli nového nastavení v klientském počítači) asi dvacet minut. Při výchozím nastavení se zásady skupiny obnoví na pozadí každých 90 minut s náhodným posunem od 0 do 30 minut. Pokud chcete obnovit zásady skupiny dříve, můžete přejít na příkazový řádek v klientském počítači a zadat následující příkaz: **gpupdate /force**.

U klientských počítačů konfigurovaných s místním objektem skupiny zásad je skupina zásad použita ihned a bude to trvat asi 20 minut.

Poté, kdy je skupina zásad použita, je možné spustit rozpoznávání ručně. Pokud provedete tento krok, nemusíte čekat 20 minut, než bude klientský počítač kontaktovat server WSUS.

**Ruční spuštění rozpoznávání serverem WSUS**
1.  V klientském počítači klepněte na tlačítko **Start** a klepněte na příkaz **Spustit**.

2.  Zadejte příkaz **cmd** a klepněte na tlačítko **OK**.

3.  V příkazovém řádku zadejte příkaz **wuauclt.exe /detectnow**. Tato možnost příkazového řádku dává pokyny automatickým aktualizacím, aby ihned kontaktovaly server WSUS.
