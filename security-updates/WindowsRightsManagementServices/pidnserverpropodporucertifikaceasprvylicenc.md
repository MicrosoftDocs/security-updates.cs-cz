---
TOCTitle: Přidání serverů pro podporu certifikace a správy licencí
Title: Přidání serverů pro podporu certifikace a správy licencí
ms:assetid: '089ceb62-2a96-444f-ab42-1d5deaabd0c3'
ms:contentKeyID: 18113203
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc720189(v=WS.10)'
---

Přidání serverů pro podporu certifikace a správy licencí
========================================================

Po instalaci a zajištění prvního serveru a vytvoření kořenové instalace služby RMS můžete nainstalovat další servery, které zajistí rozšířenou podporu pro služby certifikace a správy licencí, jako v následujících případech:

-   Můžete přidat server jako člena clusteru kořenové certifikace, který bude zajišťovat další podporu certifikace a správy licencí. Server přidaný do tohoto clusteru používá stejnou konfiguraci a stejné databáze jako server kořenové certifikace.
-   Můžete instalovat server správy licencí, který bude pracovat samostatně nebo jako člen clusteru serverů správy licencí. Proběhne jeho dílčí zápis v clusteru kořenové certifikace a server získá certifikát serveru pro poskytování licencí prostřednictvím služeb certifikace serveru kořenové certifikace. Všechny požadavky klientů na služby certifikace adresované serveru správy licencí jsou postoupeny serveru certifikace. Server správy licencí může vydávat licence k použití a k publikování, aniž by bylo nutné odesílat požadavky serveru kořenové certifikace.

Možnost, kterou se rozhodnete nasadit, závisí na velikosti organizace a na požadovaném způsobu implementace redundance, škálovatelnosti, podpory vyrovnávání zatížení a zabezpečení. V případě nasazení doplňujících serverů RMS, které mají vyhovět rostoucím požadavkům na certifikaci, správu licencí a publikování, byste měli servery RMS nasadit jako součást clusteru kořenové certifikace, abyste mohli nastavit redundanci a vyrovnávání zatížení pro všechny servery. Můžete vytvářet clustery serverů certifikace a převzít zpracování požadavků na služby správy licencí a publikování prostřednictvím dílčího zápisu serverů správy licencí (z nichž lze také vytvářet clustery za účelem vyrovnávání zatížení). Nelze však vyrovnávat zatížení clusteru správy licencí s dílčím zápisem pomocí clusteru kořenové certifikace.

Informace o této úloze získáte z následujících témat:

-   [Oprávnění, práva a role nutné k instalaci a zajištění](#bkmk_1)
-   [Procesy zajištění pro další servery certifikace a správy licencí](#bkmk_2)
-   [Instalace clusterů a vyrovnávání zatížení](#bkmk_3)

<span id="BKMK_1"></span>
Oprávnění, práva a role nutné k instalaci a zajištění
-----------------------------------------------------

Chcete-li instalovat a zajistit další servery, budete potřebovat stejné role, oprávnění a práva jako při instalaci prvního serveru. Navíc je nutné získat také oprávnění ze serveru kořenové certifikace k nastavení samostatného serveru správy licencí, čemuž se říká dílčí zápis. Server kořenové certifikace je řízen volitelným seznamem řízení přístupu souboru SubEnrollService.asmx. Členové skupiny RMS Service Group, včetně účtu služby RMS, který zadáte během zajišťování serveru kořenové certifikace, mají oprávnění k provádění dílčího zápisu. Další informace získáte v tomto tématu v části [Nastavení služby certifikace a správy licencí na prvním serveru](https://technet.microsoft.com/cce29a2f-984f-48ed-9187-0eb68286ec5b) uvedené již dříve.

<span id="BKMK_2"></span>
Procesy zajištění pro další servery certifikace a správy licencí
----------------------------------------------------------------

Podmínkou přidání serveru do clusteru certifikace nebo správy licencí je provedení procesu zajištění na tomto serveru. Konkrétní postup zajištění závisí na typu zajišťovaného serveru.

-   Pokud zajišťujete samostatný server správy licencí, zadejte konfigurační databázi, účet služby RMS, adresu URL clusteru a informace o ochraně soukromého klíče stejným způsobem, jakým jste tyto informace zadali pro server kořenové certifikace. Nebudete však uvádět zásady odvolání certifikátu serveru pro poskytování licencí, tyto zásady jsou řízeny serverem kořenové certifikace.
-   Pokud zajišťujete server, který bude členem clusteru, je nutné během zajišťování zadat pouze účet služby RMS, konfigurační databázi a heslo pro ochranu soukromého klíče (nebo použijte stejného zprostředkovatele kryptografických služeb a soukromý klíč jako pro existující cluster). Všechny servery v clusteru sdílí stejný certifikát serveru pro poskytování licencí a stejný pár klíčů serveru.

> [!IMPORTANT]
> Nespouštějte instalaci služby RMS na žádném jiném serveru, dokud nebude dokončena instalace uvedené služby na prvním serveru, včetně instalace i zajištění tohoto serveru. 

Po instalaci a zajištění dalšího serveru je tento server automaticky nakonfigurován jako člen clusteru. Jestliže jste však implementovali vyrovnávání zatížení, je nutné nakonfigurovat software vyrovnávání zatížení tak, aby s novým serverem spolupracoval.

<span id="BKMK_3"></span>
Instalace clusterů a vyrovnávání zatížení
-----------------------------------------

Služba RMS je vytvořena tak, aby podporovala clustery serverů. Vytváření clusterů serverů RMS zajišťuje větší škálovatelnost, spolehlivost a vyrovnávání zatížení daného nasazení služby RMS.

**Vytváření clusterů**

Chcete-li instalovat cluster, začněte se serverem kořenové certifikace nebo serverem správy licencí. U druhého a všech dalších serverů v každém clusteru nainstalujte službu RMS na novém serveru, přejděte na stránku **Globální správa** a klepněte na položku **Přidat tento server do clusteru** k zajištění nezbytných prostředků a přidání serveru do clusteru kořenové certifikace nebo clusteru správy licencí.

Zadejte název databáze pro cluster, ke kterému se chcete připojit.

**Vyrovnávání zatížení clusterů**

Služba RMS neimplementuje vyrovnávání zatížení automaticky. Zatížení mezi všemi servery RMS je možné vyrovnávat pomocí hardwarového nebo softwarového řešení pro vyrovnávání zatížení, včetně služby Vyrovnávání zatížení sítě.

Další podrobnosti o této problematice naleznete v následujících tématech:

-   Další informace o rozdílech mezi službami certifikace a správy licencí získáte v této sadě dokumentace v části Přehled systému služby RMS tématu Technické informace týkající se služby RMS.
-   Další informace o tom, jak přizpůsobit nasazení serverů požadavkům organizace na dostupnost a výkon, získáte v této sadě dokumentace v části Zajištění redundance dat a vyrovnávání zatížení tématu Plánování nasazení služby RMS .
-   Další informace o tom, jak určit počet serverů nutných pro podporu nasazení serveru RMS v organizaci, získáte v této sadě dokumentace v části Vyhodnocení požadavků na rozsah tématu Plánování nasazení služby RMS.
-   Další informace o tom, jak implementovat zabezpečení IT do nasazení služby RMS, naleznete v tomto tématu později v části [Zabezpečení nasazení služby RMS](https://technet.microsoft.com/6de8b636-a824-4844-aefc-f26347abfc14).
-   Informace o postupu instalace služby RMS získáte v této sadě dokumentace v části Instalace služby RMS s aktualizací Service Pack 1 tématu Provoz serveru RMS.
    Službu RMS můžete také nainstalovat z příkazového řádku. Další informace najdete v této sadě dokumentace v části Instalace z příkazového řádku tématu Provoz serveru RMS.
-   Informace o tom, jak zajistit server správy licencí získáte v této sadě dokumentace v části Zajištění serveru správy licencí tématu Provoz serveru RMS.
-   Informace o postupu zajištění dalších serverů v clusteru získáte v této sadě dokumentace v části Přidání serveru do clusteru tématu Provoz serveru RMS.
