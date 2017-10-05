---
TOCTitle: 'Aktualizace nasazení pomocí aktualizace RMS Service Pack 2 (SP2)'
Title: 'Aktualizace nasazení pomocí aktualizace RMS Service Pack 2 (SP2)'
ms:assetid: '27ee06a1-f467-4a6c-b662-45ddb5f8c13e'
ms:contentKeyID: 18113242
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc720225(v=WS.10)'
---

Aktualizace nasazení pomocí aktualizace RMS Service Pack 2 (SP2)
================================================================

Tato část obsahuje informace, které vám usnadní instalaci Služby správy přístupových práv (RMS) Microsoft® Windows® s aktualizací Service Pack 2 (SP2) v organizaci s existujícím nasazením služby RMS. Aktualizaci nasazení na službu RMS s aktualizací SP2 je nutné provést pouze v organizacích, které již službu RMS nasadily. Organizace nasazující službu RMS poprvé mohou službu RMS s aktualizací SP2 nasadit podle pokynů v tématech Plánování nasazení služby RMS ([http://go.microsoft.com/fwlink/?LinkId=74999](http://go.microsoft.com/fwlink/?linkid=74999)) a Nasazení systému RMS ([http://go.microsoft.com/fwlink/?LinkID=75000](http://go.microsoft.com/fwlink/?linkid=75000)) v této sadě dokumentace.

Službu RMS s aktualizací SP2 je možné nainstalovat, aniž byste odebrali existující instalaci služby RMS s aktualizací SP1. Instalační program služby RMS s aktualizací SP2 zjistí, že je nainstalována služba RMS s aktualizací SP1 a podle potřeby přidá další funkce a nastavení.

| ![](images/Cc720225.note(WS.10).gif)Poznámka                                                                                                                                                                                                                                            |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Upgrade serveru RMS bez aktualizace Service Pack na službu RMS s aktualizací SP2 není podporován. Pokud používáte server RMS bez aktualizace Service Pack, je nutné před upgradem na službu RMS s aktualizací SP2 upgradovat na službu RMS s aktualizací SP1. Klienta RMS lze upgradovat z jakékoli předchozí verze. |

**Obsah tématu**

-   [Příprava na aktualizaci na verzi služby RMS s aktualizací SP2](#bkmk_preparingforsp2update)
-   [Provedení aktualizace na verzi služby RMS s aktualizací SP2](#bkmk_performingsp2update)
-   [Aktualizace clusterů](#bkmk_updateclusters)
-   [Aktualizace klientů RMS](#bkmk_updateclients)
-   [Vzájemná funkční spolupráce se službou RMS verze 1.0](#bkmk_interop)
-   [Odebrání služby RMS s aktualizací SP2](#bkmk_removingrms)

<span id="bkmk_PreparingForSP2Update"></span>
Příprava na aktualizaci na verzi služby RMS s aktualizací SP2
-------------------------------------------------------------

Aktualizace na verzi služby RMS s aktualizací SP2 byla navržena tak, aby vám umožnila provoz služby RMS bez přerušení. Před upgradem clusteru služby RMS však doporučujeme provést následující kroky:

-   Zazálohujte konfigurační databázi a privátní klíč služby RMS. Další informace získáte v tématu týkajícím se zálohování systému pro službu RMS ([http://go.microsoft.com/fwlink/?LinkId=75001](http://go.microsoft.com/fwlink/?linkid=75001)) v této sadě dokumentace.
-   Pokud používáte softwarový privátní klíč služby RMS, zajistěte si jeho heslo.
-   Zazálohujte databázi protokolování, jestliže chcete zachovat předchozí zaprotokolovanou statistiku.
-   Ověřte, zda jsou v klientech a na serverech nainstalovány nejnovější důležité aktualizace a aktualizace zabezpečení operačního systému. Chcete-li ověřit, zda jsou všechny důležité aktualizace a aktualizace zabezpečení nainstalovány, klepněte na tlačítko **Start** a na příkaz **Windows Update**. Pak postupujte podle pokynů na obrazovce.

<span id="bkmk_PerformingSP2Update"></span>
Provedení aktualizace na verzi služby RMS s aktualizací SP2
-----------------------------------------------------------

Jakmile Průvodce instalací Služby správy přístupových práv s aktualizací Service Pack 2 zjistí vaši instalaci služby RMS, zaměří se na aktuální instalaci služby RMS s aktualizací SP1 a pouze přidá nové soubory nebo nahradí soubory, které je třeba pro službu RMS s aktualizací SP2 změnit. Pokud již službu RMS úspěšně používáte, nemusíte ji po instalaci verze RMS s aktualizací SP2 zprovozňovat znovu ani není nutné provádět jakoukoli další konfiguraci, abyste ji mohli i nadále používat.

<span id="bkmk_UpdateClusters"></span>
Aktualizace clusterů
--------------------

Jestliže jste službu RMS nainstalovali v clusterové konfiguraci, měli byste aktualizaci clusterů naplánovat, abyste omezili vliv aktualizace na příslušnou instalaci. Při určování nejvhodnějšího způsobu implementace služby RMS s aktualizací SP2 v organizaci zvažte následující doporučení:

-   Doporučeným postupem je instalace služby RMS s aktualizací SP2 vždy pouze v části clusteru, aby byl upgrade clusteru předvídatelnější a omezilo se riziko snížení výkonu služby během upgradu.
-   Pokud používáte více clusterů služby RMS, měli byste nejprve upgradovat clustery kořenové certifikace, a pak clustery licencování s dílčím zápisem.
-   Jestliže využíváte rozšiřování skupin mezi doménovými strukturami, můžete clustery v doménových strukturách upgradovat nezávisle, aniž byste schopnost serverů RMS rozšiřovat členství ve skupinách mezi doménovými strukturami ovlivnili.
-   Servery RMS s aktualizací SP2, RMS s aktualizací SP1 a RMS verze 1.0 mohou spolu fungovat a vzájemně spolupracovat pouze v případě, že se nacházejí v různých doménových strukturách služby Active Directory. Nedoporučujeme používat různé verze serverů RMS ve stejném clusteru.
-   Pomocí instalačního balíčku služby RMS s aktualizací SP2 lze také nainstalovat nové nasazení služby RMS s aktualizací SP2 na serveru. Není nutná instalace služby RMS s aktualizací SP1.

<span id="bkmk_UpdateClients"></span>
Aktualizace klientů RMS
-----------------------

Nový klient RMS s aktualizací SP2 je k dispozici na webu služby Windows Update nebo služby Stažení softwaru. Pomocí instalačního balíčku klienta RMS s aktualizací SP2 lze také nainstalovat novou verzi klienta RMS s aktualizací SP2 v počítači. Není nutná instalace klienta RMS verze 1.0. Klient RMS s aktualizací SP2 obsahuje funkci zpětné kompatibility, aby jej bylo možné používat s aplikacemi s podporou služby RMS, které vyžadují službu RMS verze 1.0.

Další informace o aktualizaci a instalaci klienta RMS získáte v tématu Distribuce klienta RMS ([http://go.microsoft.com/fwlink/?LinkId=75070](http://go.microsoft.com/fwlink/?linkid=75070)).

<span id="bkmk_InterOp"></span>
Vzájemná funkční spolupráce se službou RMS verze 1.0
----------------------------------------------------

Vzhledem k tomu, že služba RMS s aktualizací SP2 nabízí mnoho zdokonalených funkcí a vylepšení výkonu, měli byste ji nainstalovat během svého nejbližšího cyklu upgradu. Přestože servery a klienti RMS se službou RMS s aktualizací SP2 mohou bez problémů vzájemně spolupracovat se servery a klienty RMS s jinou verzí, je nutné upozornit na následující rozdíly ve fungování ve smíšeném prostředí:

-   Offline dílčí zápis zajistí pouze servery RMS s aktualizací SP1 nebo vyšší.
-   Vlastní aktivaci provádí pouze klienti RMS s aktualizací SP1 nebo vyšší.
-   Následující tabulka popisuje podporované funkce pro smíšená prostředí:

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
<th style="border:1px solid black;" >Verze serveru RMS</th>
<th style="border:1px solid black;" >Funkce podporované klienty verze  1</th>
<th style="border:1px solid black;" >Funkce podporované klienty s aktualizací SP2</th>
<th style="border:1px solid black;" >Funkce podporované ve smíšeném prostředí klientů</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">1.0</td>
<td style="border:1px solid black;">Všechny předchozí funkce.
Není k dispozici offline dílčí zápis serveru. Dílčí zápis serveru je nutné provést prostřednictvím Internetu.
Nejsou k dispozici klienti s vlastní aktivací.</td>
<td style="border:1px solid black;">Všechny předchozí funkce.
Není k dispozici offline dílčí zápis serveru.
Klienti s vlastní aktivací.</td>
<td style="border:1px solid black;">Všechny předchozí funkce.
U verze s aktualizací SP2 se klienti aktivují sami.
U verze 1 se klienti musí aktivovat prostřednictvím Internetu.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">SP2</td>
<td style="border:1px solid black;">Všechny předchozí funkce.
Offline dílčí zápis serveru.
Nejsou k dispozici klienti s vlastní aktivací.</td>
<td style="border:1px solid black;">Všechny funkce verze s aktualizací SP1.
Offline dílčí zápis serveru.
Klienti s vlastní aktivací.
Bezpečnostní modul serveru.
Microsoft SQL Server™ 2005 je podporován ve výchozím nastavení.</td>
<td style="border:1px solid black;">Všechny předchozí funkce a funkce verze s aktualizací SP2.
Offline dílčí zápis serveru.
U verze s aktualizací SP2 se klienti aktivují sami.
U verze 1 se klienti musí aktivovat prostřednictvím Internetu.</td>
</tr>
</tbody>
</table>
 

<span id="bkmk_RemovingRMS"></span>
Odebrání služby RMS s aktualizací SP2
-------------------------------------

Pokud se chcete po instalaci služby RMS s aktualizací SP2 vrátit k předchozí konfiguraci serveru RMS, můžete službu RMS s aktualizací SP2 odebrat pomocí panelu **Přidat nebo odebrat programy** v **Ovládacích panelech**.
