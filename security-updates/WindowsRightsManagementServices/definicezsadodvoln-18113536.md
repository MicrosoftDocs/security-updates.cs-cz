---
TOCTitle: Definice zásad odvolání
Title: Definice zásad odvolání
ms:assetid: 'e2fffe9f-def7-439b-a8aa-43f8a065813d'
ms:contentKeyID: 18113536
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747782(v=WS.10)'
---

Definice zásad odvolání
=======================

Definici zásad odvolání v konkrétní organizaci je třeba pečlivě zvážit a naplánovat. Zásady odvolání umožňují vyšší zabezpečení chráněného obsahu, mají však vliv na způsob, jakým mohou uživatelé pracovat s obsahem. Zásady odvolání pro nasazení služby RMS lze definovat z webu pro správu.

Odvolání třetích stran
----------------------

Vzhledem k tomu, že vydavatelem certifikátu serveru pro poskytování licencí pro server kořenové certifikace nasazení služby RMS je služba Microsoft Enrollment Services, může tento certifikát odvolat společnost Microsoft. Společnost Microsoft odvolá certifikát serveru pro poskytování licencí pouze v případě, že je k tomu vyzvána soudem.

Kromě služby Microsoft Enrollment Services je možné určit třetí stranu, která může certifikát serveru pro poskytování licencí pro server služby RMS odvolat. Touto stranou může být entita mimo danou organizaci nebo pár veřejných či soukromých klíčů generovaných správcem jménem organizace. Určený soukromý klíč třetí strany může být použit k podpisu seznamu odvolání, jehož prostřednictvím je odvolán certifikát serveru pro poskytování licencí. Třetí strana je v průběhu zajištění služby RMS určena svým veřejným klíčem. Šablonu zásad práv serveru je také možné konfigurovat tak, aby třetí straně umožňovala odvolat obsah, manifesty aplikací a certifikáty vydané instalací služby RMS. Další informace získáte v tomto tématu později v části [Vytvoření a změna šablon zásad práv](https://technet.microsoft.com/6014176f-ef71-4d29-b3e3-da129c18563d).

| ![](images/Cc747782.Important(WS.10).gif)Důležité informace                                                                                                            |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Pokud se rozhodnete generovat vlastní pár klíčů, který budete chtít použít k odvolání certifikátu serveru pro poskytování licencí pro server kořenové certifikace, uložte jej na zabezpečené místo. |

Odvolání certifikátu serveru pro poskytování licencí je důležité rozhodnutí, protože všechny certifikáty a licence vydané instalací služby RMS budou po jeho odvolání neplatné. Další informace týkající se odvolání certifikátů serverů pro poskytování licencí získáte v tomto tématu později v části [Odvolání certifikátů serveru pro poskytování licencí](https://technet.microsoft.com/8020861d-d196-4431-8282-044675ef5616).

Zvážení způsobu použití seznamů odvolání
----------------------------------------

Je-li pro určitou část chráněného obsahu vyžadováno odvolání, budou použity všechny seznamy odvolání, které jsou registrovány v klientských počítačích, a budou uplatněny při splnění zadané podmínky. Při implementaci odvolání je tedy třeba postupovat opatrně, protože v rámci této implementace jsou v klientských počítačích registrovány seznamy odvolání, které mohou být použity v širším měřítku, než bylo původně zamýšleno. Další informace o konfigurace této možnosti získáte v tomto tématu později v části [Vytvoření a změna šablon zásad práv](https://technet.microsoft.com/6014176f-ef71-4d29-b3e3-da129c18563d).

Vyvážení zabezpečení a použitelnosti
------------------------------------

Při určování zásad odvolání v šabloně zásad práv zvažte potřebu většího zabezpečení dokumentů proti možnosti, že uživatelé budou mít případně potíže při práci s obsahem, jak je například popsáno v následujícím odstavci.

Jako součást nastavení seznamu odvolání by v šabloně zásad práv měl být určen také interval aktualizace seznamu odvolání. Aby bylo možné pracovat s obsahem publikovaným pomocí dané šablony zásad práv, musí v počítači uživatele existovat seznam odvolání a tento seznam nesmí být starší, než je určený interval aktualizace. Jestliže je například nastaven interval aktualizace s hodnotou 10, je nutné, aby byl seznam odvolání vytvořen v období posledních 10 dnů. Pokud v klientském počítači seznam odvolání neexistuje nebo pokud je datum vytvoření seznamu starší než interval aktualizace, bude aplikaci s podporou služby RMS odeslán poslední seznam odvolání z umístění určeného v licenci k použití. Uživatel nepřipojený k síti však aktuální seznam odvolání obdržet nemůže, a proto nebude moci pracovat s obsahem.

Pomocí následujících opatření lze závažnost tohoto problému zmírnit:

-   Interval aktualizace seznamu odvolání určete s rozmyslem a zajistěte, aby byl aktuální seznam obnovení uživatelům vždy k dispozici.
-   Seznamy odvolání uchovávejte na adresách URL, které jsou dostupné z podnikové sítě i mimo ni.
-   Pomocí serveru SMS (Microsoft® Systems Management Server) distribuujte aktualizované kopie seznamů odvolání do klientských počítačů v pravidelných intervalech, například každou noc.
-   Odvolání vyžadujte pouze pro nejcitlivější typy dokumentů.
