---
TOCTitle: Sledování front zpráv
Title: Sledování front zpráv
ms:assetid: 'a7109399-3a84-4681-874b-f6ea1646b0a0'
ms:contentKeyID: 18113461
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747716(v=WS.10)'
---

Sledování front zpráv
=====================

Funkce protokolování služby RMS používá službu Řízení front zpráv (známou též pod zkratkou MSMQ) k odesílání událostí do databáze protokolování. Každý koncový server RMS předává zprávy službě Řízení front zpráv a služba naslouchání protokolování na každém koncovém serveru načítá zprávy protokolování z fronty služby Řízení front zpráv a zapisuje je do databáze protokolování. Pokud databáze protokolování či databázový server přestanou být k dispozici nebo pokud je služba naslouchání protokolování zastavena, začne služba Řízení front zpráv ukládat zprávy do fronty. Pokud hodláte ukončit činnost databáze protokolování nebo databázového serveru, je doporučeno nejprve ukončit činnost služby naslouchání protokolování na všech koncových serverech a po restartování databáze protokolování nebo databázového serveru pak tuto službu na koncových serverech restartovat.

Pokud databáze selže a služba naslouchání protokolování je stále spuštěna, nebude tato služba schopna zapisovat zprávy protokolování do databáze. Služba naslouchání protokolování bude zprávy přesouvat do fronty nedoručených zpráv služby Řízení front zpráv, dokud nebude databáze znovu k dispozici. Od tohoto okamžiku budou do databáze zapisovány nové zprávy protokolování. Zprávy z fronty nedoručených zpráv nebudou do databáze protokolování automaticky zapsány. Zprávy z této fronty lze zobrazit a odstranit následujícím postupem:

1.  Spusťte modul snap-in Správa počítače konzoly MMC (Microsoft Management Console). Modul můžete spustit klepnutím na tlačítko **Start**, přechodem na položku **Všechny programy**, na položku **Nástroje pro správu** a klepnutím na příkaz **Správa počítače**.
2.  Pod položkou Služby a aplikace ve stromu konzoly klepněte na položku Řízení front zpráv a pak klepněte na položku Soukromé fronty.
3.  Zobrazí se dvě fronty. Název obou bude začínat řetězcem **drms\_logging** a pokračovat názvem clusteru. Jedna z front bude mít název **drms\_logging***\_&lt;název clusteru&gt;*\_**deadletter**. Jedná se o frontu nedoručených zpráv. Klepněte na název fronty a pak klepněte na frontu Zprávy fronty.
4.  Poklepáním na jednotlivé zprávy zobrazíte vlastnosti těchto zpráv.
5.  Chcete-li frontu odstranit, klepněte pravým tlačítkem na frontu **Zprávy fronty**, vyberte položku **Všechny úkoly** a pak vyberte možnost **Vymazat**.

Ve výchozí konfiguraci bude služba Řízení front zpráv ukládat všechny zprávy až do vyčerpání volného místa na serveru. Jestliže služba Řízení front zpráv zaplní veškeré volné místo na pevném disku, nemůže server RMS zpracovávat požadavky klientů. Chcete-li této situaci předejít, omezte následujícím postupem množství místa na disku, které může služba Řízení front zpráv pro fronty využívat:

1.  Spusťte modul snap-in Správa počítače konzoly MMC (Microsoft Management Console). Modul můžete spustit klepnutím na tlačítko Start, přechodem na položku Všechny programy, na položku Nástroje pro správu a klepnutím na příkaz Správa počítače.
2.  Pod položkou Služby a aplikace ve stromu konzoly klepněte na položku Řízení front zpráv a pak klepněte na položku Soukromé fronty.
3.  Zobrazí se dvě fronty. Název obou bude začínat řetězcem drms\_logging. Pro každou frontu proveďte následující akce:
    -   Klepněte na možnost Vlastnosti.
    -   Zaškrtněte políčko Omezit velikost úložiště zpráv na (kB) a zadejte celkovou velikost (v kilobajtech) všech zpráv fronty, které budou ve frontě uloženy.

Pokud se fronta zaplní, budou zprávy ze služby RMS po přijetí zahozeny a do systémového protokolu událostí bude odeslána následující zpráva o události s ID 48:

Odesílání balíku vlastností do služby Řízení front zpráv se nezdařilo.

Doporučujeme nakonfigurovat nástroje pro sledování systému tak, aby na tuto událost upozorňovaly, protože může znamenat problém s databází protokolování.
