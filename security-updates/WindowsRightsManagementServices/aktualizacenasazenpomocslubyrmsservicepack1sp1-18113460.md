---
TOCTitle: 'Aktualizace nasazení pomocí služby RMS Service Pack 1 (SP1)'
Title: 'Aktualizace nasazení pomocí služby RMS Service Pack 1 (SP1)'
ms:assetid: 'a562c4b0-15df-46db-9d61-24db74871cfa'
ms:contentKeyID: 18113460
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747714(v=WS.10)'
---

Aktualizace nasazení pomocí služby RMS Service Pack 1 (SP1)
===========================================================

Tato část obsahuje informace, které vám pomohou nainstalovat aktualizaci služby Microsoft® Windows® Rights Management Services (RMS) Service Pack 1 (SP1) v organizaci, ve které je již služba RMS nainstalována. Na službu RMS SP1 musí upgradovat pouze organizace, které již mají službu RMS nasazenou. Organizace, které nasazují službu RMS poprvé, mohou nasadit službu RMS s aktualizací SP1 podle pokynů v části Plánování nasazení služby RMS a Nasazení systému RMS v této sadě dokumentace.

Aktualizaci RMS SP1 můžete nainstalovat, aniž byste museli odebírat existující instalaci služby RMS. Instalační program aktualizace RMS SP1 zjistí, že je služba RMS nainstalována, a přidá další vybrané funkce a nastavení.

**V tomto tématu**

-   [Příprava na aktualizaci RMS SP1](#bkmk_1)
-   [Provedení aktualizace RMS SP1](#bkmk_2)
-   [Aktualizace clusterů](#bkmk_3)
-   [Aktualizace klientů RMS](#bkmk_4)
-   [Vzájemná spolupráce se službou RMS verze 1.0](#bkmk_5)
-   [Odebrání služby RMS s aktualizací SP1](#bkmk_6)

<span id="BKMK_1"></span>
Příprava na aktualizaci RMS SP1
-------------------------------

Aktualizace RMS SP1 je navržena tak, abyste mohli pokračovat v používání služby RMS bez přerušení. Před upgradem serverů služby RMS však doporučujeme provést následující akce:

-   Zazálohujte databázi konfigurací a privátní klíč služby RMS. Další informace získáte v této sadě dokumentace v části Systémové zálohy pro službu RMS v tématu Plánování nasazení služby RMS.
-   Zkontrolujte, zda znáte heslo k privátnímu klíči služby RMS.
-   Pokud chcete mít uloženou statistiku předchozího protokolování, zazálohujte databázi protokolování.
-   Zkontrolujte, zda máte v klientech a na serverech nainstalovány nejnovější důležité aktualizace a také aktualizace zabezpečení pro operační systém. Můžete to provést tak, že klepnete na tlačítko **Start**, klepnete na příkaz **Windows Update** a potom budete postupovat podle pokynů na obrazovce.

<span id="BKMK_2"></span>
Provedení aktualizace RMS SP1
-----------------------------

Když průvodce instalací aktualizace RMS SP1 detekuje vaší instalaci služby RMS, pouze přidá nové soubory nebo nahradí ty, které je potřeba změnit pro aktualizaci RMS SP1. Pokud je již úspěšně spuštěna služba RMS, není potřeba ji znovu zprovozňovat nebo provádět jakoukoli další konfiguraci po nainstalování aktualizace RMS SP1, aby bylo možné službu RMS dále používat.

<span id="BKMK_3"></span>
Aktualizace clusterů
--------------------

Jestliže jste nainstalovali službu RMS v konfiguraci clusteru, měli byste naplánovat aktualizaci clusterů, abyste minimalizovali dopad aktualizace na existující instalaci. Při určování, jak nejlépe implementovat aktualizaci RMS SP1 ve vaší organizaci, zvažte následující doporučení:

-   Aktualizaci RMS SP1 doporučujeme instalovat vždy jen na část clusteru, aby byl upgrade clusteru předvídatelnější a byla u něj menší pravděpodobnost, že během upgradu způsobí snížení výkonu služby.
-   Pokud máte více clusterů služby RMS, měli byste nejprve upgradovat clustery kořenové certifikace a potom upgradovat clustery pro správu licencí s dílčím zápisem.
-   Jestliže používáte rozšíření skupiny mezi doménovými strukturami, můžete upgradovat clustery v doménových strukturách nezávisle bez dopadu na schopnost serverů RMS rozšířit členství skupiny mezi doménové struktury.
-   Možná je souběžná existence a vzájemná spolupráce serveru s verzí RMS SP1 a RMS 1.0.
-   Instalační balíček aktualizace RMS SP1 lze také používat k instalaci nové verze aktualizace RMS SP1 na serveru. Není nutné, aby byla nainstalována služba RMS verze 1.0.

<span id="BKMK_4"></span>
Aktualizace klientů RMS
-----------------------

Součástí služby RMS s aktualizací SP1 je klient RMS. Instalační balíček klienta RMS SP1 lze také používat k instalaci nové verze klienta RMS SP1 do počítače. Není nutné, aby byl nainstalován klient RMS verze 1.0. Součástí klienta RMS SP1 je funkce zpětné kompatibility, díky které ho lze používat pomocí aplikací podporujících službu RMS, které vyžadují verzi RMS 1.0.

Tento nový klient RMS nabízí následující funkce:

-   Klient se již nemusí připojit k serveru společnosti Microsoft přes Internet a stáhnout bezpečnostní modul.
-   Jestliže nainstalujete klienta RMS pomocí serveru SMS nebo zásad skupiny, nejsou pro instalaci nutná oprávnění pro správu.
-   Klient RMS SP1 obsahuje nový serverový bezpečnostní modul (také známý jako serverový procesor zabezpečení), pomocí kterého lze zajistit pro webové služby a aplikace na straně serveru, například Windows SharePoint® Services a Exchange Server 2003, podporu služby RMS, aby mohla služba používat a distribuovat obsah chráněný pomocí služby RMS. Tento bezpečnostní modul je navržen tak, aby poskytoval co nevyšší výkon a co nejlepší možnosti škálování v důvěryhodných serverových aplikacích.
-   Klient RMS používá šifrovací algoritmy s certifikací FIPS 140-2. To umožňuje nasadit klienta v organizaci kompatibilní se standardem FIPS.

<span id="BKMK_5"></span>
Vzájemná spolupráce se službou RMS verze 1.0
--------------------------------------------

Vzhledem k tomu, že aktualizace RMS SP1 nabízí řadu vylepšení výkonu i celkově, měli byste ji nainstalovat po dokončení testování. Přestože spolu servery a klienti RMS, ve kterých běží služba RMS SP1, mohou vzájemně spolupracovat bez jakýchkoli omezení s klienty a servery RMS, ve kterých služba RMS SP1 neběží, měli byste vědět o následujících rozdílech, jak fungují ve smíšeném prostředí:

-   Offline zápis je možný pouze u serverů, ve kterých běží služba RMS SP1.
-   Automatická aktivace probíhá pouze u klientů, ve kterých běží služba RMS SP1.
-   Následující tabulka uvádí podporované funkce pro smíšená prostředí:

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th>Verze serveru RMS</th>
<th>Funkce podporované u klientů v1</th>
<th>Funkce podporované u klientů SP1</th>
<th>Funkce podporované ve smíšeném prostředí klientů (v1 a SP1)</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">1.0</td>
<td style="border:1px solid black;">Všechny předchozí funkce
Bez offline zápisu serveru Server se musí zapsat přes Internet.
Bez automatické aktivace klientů</td>
<td style="border:1px solid black;">Všechny předchozí funkce
Bez offline zápisu serveru
Automatické aktivace klientů</td>
<td style="border:1px solid black;">Všechny předchozí funkce
V případě klientů SP1 se klienti automaticky aktivují.
V případě klientů v1 je nutné klienty aktivovat přes Internet.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">SP1</td>
<td style="border:1px solid black;">Všechny předchozí funkce
Offline zápis serveru
Bez automatické aktivace klientů</td>
<td style="border:1px solid black;">Všechny funkce SP1
Offline zápis serveru
Automatické aktivace klientů
Bezpečnostní modul serveru</td>
<td style="border:1px solid black;">Všechny předchozí funkce a navíc funkce aktualizace SP1
Offline zápis serveru
V případě klientů SP1 se klienti automaticky aktivují.
V případě klientů v1 je nutné klienty aktivovat přes Internet.</td>
</tr>
</tbody>
</table>
 

<span id="BKMK_6"></span>
Odebrání služby RMS s aktualizací SP1
-------------------------------------

Pokud u serveru RMS obnovíte předchozí konfiguraci po instalaci aktualizace RMS SP1, můžete aktualizaci RMS SP1 odebrat pomocí panelu **Přidat nebo odebrat programy** v **Ovládacích panelech**.

**Poznámka:** Pokud jste před instalací aktualizace RMS SP1 provedli zálohu databáze konfigurace, můžete ji obnovit, a tím zcela zrušit všechny změny související s instalací aktualizace RMS SP1. Jestliže jste databázi konfigurace nezazálohovali, je možné, že budete moci s obnovenou instalací služby RMS použít databázi konfigurace z instalace aktualizace RMS SP1. Obnovená instalace služby RMS bude ignorovat pole navíc, která do databáze konfigurace přidá instalace aktualizace RMS SP1, protože je nepoužívá.
