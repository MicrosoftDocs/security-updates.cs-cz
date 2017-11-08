---
TOCTitle: Přidání serveru do clusteru
Title: Přidání serveru do clusteru
ms:assetid: 'db635238-5528-4bec-9cc6-8244e2b3d733'
ms:contentKeyID: 18113476
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747690(v=WS.10)'
---

Přidání serveru do clusteru
===========================

Provedení tohoto postupu vyžaduje, aby byl uživatel místně přihlášen k webu pro správu v rámci uživatelského účtu, který je členem skupiny Administrators v počítači, k němuž získává přístup. Uvedený postup mohou provést také členové skupiny Domain Admins. Z hlediska zabezpečení je nejvhodnější při provádění tohoto postupu použít příkaz **Spustit jako**.

Chcete-li otevřít webovou stránku **Globální správa**, klepněte na tlačítko **Start**, přejděte na příkaz **Všechny programy**, přejděte na položku **Služba RMS v systému Windows** a klepněte na položku **Správa služby RMS v systému Windows**.

Na každém serveru lze službu RMS zajistit pouze pro jeden web. Chcete-li zajistit službu RMS pro jiný než výchozí web, přidejte požadovaný web pomocí Správce Internetové informační služby dříve, než zahájíte proces zajišťování. Není-li web, pro který chcete službu zajistit, uveden v seznamu webů, zavřete stránku **Globální správa**, přidejte požadovaný web a poté znovu spusťte proces zajišťování.

Pokud nasazujete službu RMS v prostředí, kde je úroveň funkčnosti domény služby Active Directory nastavena na nativní režim systému Microsoft Windows 2000, nemusí být služba RMS při pokusu o rozšíření členství ve skupině schopna načíst atribut **memberOf** objektů služby Active Directory. Chcete-li službě RMS umožnit načtení atributu **memberOf**, musí služba RMS využívat účet domény, který je členem (integrované) skupiny Pre-Windows 2000-Compatible Access obsažené v místní doménové struktuře.

Přidání serveru do clusteru
---------------------------

#### Přidání serveru do clusteru

1.  Po instalaci služby RMS na server, který chcete připojit do clusteru kořenové certifikace nebo správy licencí, otevřete stránku **Globální správa**.

2.  Klepněte na položku **Přidat tento server do clusteru** u webu, pro který chcete zajistit službu RMS. Můžete vybrat výchozí web nebo jiný web, který jste pro tento účel vytvořili v Internetové informační službě (IIS).

    | ![](images/Cc747690.Warning(WS.10).gif)Varování                                                                                                                                                                                                         |
    |--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Spouštění dalších webů a webových služeb na společném serveru se službou RMS není podporováno. Výsledkem by mohl být případ, kdy bude pod stejným účtem jako služba RMS pracovat více aplikací a služeb. V takovém případě hrozí provádění nezaručených operací se soukromými klíči. |

3.  V části **Účet služby RMS** zadejte název účtu ve tvaru název\_domény\\uživatelské\_jméno a heslo účtu služby RMS, pod kterým bude služba RMS zpravidla pracovat za normálního provozu. Musí se jednat o doménový účet. Všechny servery v clusteru by měly pracovat pod stejným účtem služby RMS.

    | ![](images/Cc747690.Important(WS.10).gif)Důležité informace                                                                                                                                                                                                 |
    |------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Z důvodů zabezpečení se doporučuje vytvořit speciální účet uživatele domény, který bude sloužit jako účet služby RMS, a nepřidělovat mu žádná zvláštní oprávnění. Jako účet služby RMS nelze použít doménový účet, který byl použit k instalaci služby RMS s aktualizací Service Pack 1. |

4.  V části **Konfigurační databáze** zadejte název databázového serveru a název konfigurační databáze pro tento cluster. Vybraná databáze určuje cluster, do kterého tento server patří.

5.  V části **Ochrana soukromého klíče** vyberte mechanismus, který tento cluster používá k ochraně soukromého klíče. V případě výchozí softwarové ochrany pomocí soukromého klíče zadejte heslo, které bylo použito k zašifrování soukromého klíče při zajištění prvního serveru v tomto clusteru.

6.  Klepněte na tlačítko **Odeslat**.

    Pokud se zobrazí chybové zprávy, stránku nezavírejte. Opravte chyby, zastavte a znovu spusťte službu IIS z příkazového řádku pomocí příkazu IISReset, vraťte se na předcházející stránku, znovu zadejte informace potřebné k zajištění a poté znovu klepněte na tlačítko **Odeslat**. Pokud se zobrazí chyba Požadavek vypršel, zavřete okno, zkontrolujte, zda systém splňuje minimální hardwarové požadavky a pokud ano, zkuste provést zajištění serveru znovu.
