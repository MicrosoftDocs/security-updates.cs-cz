---
TOCTitle: 'Nejčastější dotazy týkající se služby RMS: Šablony zásad práv'
Title: 'Nejčastější dotazy týkající se služby RMS: Šablony zásad práv'
ms:assetid: '01515f08-9844-4c1a-9ab5-a5a60a901b50'
ms:contentKeyID: 18113216
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc720175(v=WS.10)'
---

Nejčastější dotazy týkající se služby RMS: Šablony zásad práv
=============================================================

Nejčastější dotazy týkající se šablon služby RMS
------------------------------------------------

-   [Je možné vynutit výchozí šablonu služby RMS u veškerého obsahu vytvořeného v rámci organizace, aby byla v podniku zajištěna minimální sada práv?](#bkmk_57)
-   [Kde jsou umístěny šablony zásad služby RMS?](#bkmk_58)
-   [Při vytvoření jsou se šablonami svázány aliasy uživatelů a distribuční seznamy. Jak může organizace s mnoha odděleními vytvořit šablony se stejnými základními právy a zároveň udělit tato práva různým skupinám v závislosti na obsahu?](#bkmk_59)
-   [Jsou práva přiřazená k dokumentům neměnná? Pokud je odeslán soubor a později je nutné změnit práva k němu přiřazená, lze tento krok provést za předpokladu, že licence k publikování není uložena na serveru zásad služby RMS, ale je vložena v rámci daného souboru?](#bkmk_60)

<span id="BKMK_57"></span>
#### Je možné vynutit výchozí šablonu služby RMS u veškerého obsahu vytvořeného v rámci organizace, aby byla v podniku zajištěna minimální sada práv?

Ano. Pomocí sady SDK Služby správy přístupových práv lze vytvořit vlastní aplikaci, která podle potřeby vynutí jakékoli šablony. Implementace technologie IRM (Správa přístupových práv k informacím) v sadě Office 2003 a vyšší však vynucení šablon u obsahu nepodporuje.

<span id="BKMK_58"></span>
#### Kde jsou umístěny šablony zásad služby RMS?

Umístění šablon je určeno aplikací s podporou služby RMS. U sady Office 2003 a vyšší jsou uloženy v následujícím umístění určeném uživatelským nastavením v registru:

**HKEY\_CURRENT\_USER\\Software\\Microsoft\\Office\\11.0\\Common\\DRM\\AdminTemplatePath**

-nebo-

**HKEY\_CURRENT\_USER\\Software\\Microsoft\\Office\\12.0\\Common\\DRM\\AdminTemplatePath** v případě sady Microsoft Office 2007.

| ![](images/Cc720175.note(WS.10).gif)Poznámka                                                                                                                                                 |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Pokud tato položka odkazuje na místní složku v klientovi, je nutné soubory šablon do klienta zkopírovat. Jestliže položka odkazuje na síťovou sdílenou složku, nebude k dispozici v případě, že uživatel pracuje offline. |

<span id="BKMK_59"></span>
#### Při vytvoření jsou se šablonami svázány aliasy uživatelů a distribuční seznamy. Jak může organizace s mnoha odděleními vytvořit šablony se stejnými základními právy a zároveň udělit tato práva různým skupinám v závislosti na obsahu?

Pro tento scénář existují dvě řešení:

-   Vytvořte jednu šablonu s názvem Podnikové důvěrné informace, jejíž licence je udělena všem zaměstnancům dané provozní jednotky, a pak tuto šablonu použijte v e-mailu, který budete adresovat konkrétním uživatelům. Výhodou je, že pro každou provozní jednotku stačí jedna šablona pro e-mail, jejíž uživatele lze omezit podle toho, komu e-mail odešlete. Nevýhodou je, že ji i přesto může přečíst kdokoli mimo skupinu, jíž byla původně odeslána.
-   Další možností je vytvoření více šablon, a to i jedné šablony pro každý distribuční seznam. Přestože tento postup zajišťuje přesnější řízení, znamená zároveň pro oddělení IT nutnost podpory mnoha šablon.

<span id="BKMK_60"></span>
#### Jsou práva přiřazená k dokumentům neměnná? Pokud je odeslán soubor a později je nutné změnit práva k němu přiřazená, lze tento krok provést za předpokladu, že licence k publikování není uložena na serveru zásad služby RMS, ale je vložena v rámci daného souboru?

Ano, je to možné, jestliže byla použita šablona zásad služby RMS: Pokud je obsah publikován pomocí šablony zásad služby RMS, zůstává definice příslušné zásady na serveru a může být po publikování obsahu změněna správcem. Jestliže uživatel požaduje pro daný obsah licenci, udělí tato licence práva na základě aktuální zásady definované na serveru. Dojde-li ke změně práv po vydání licence k použití uživateli, budou tomuto uživateli i nadále udělena práva platná v době vydání licence. Chcete-li získat možnost použít novou šablonu zásad práv po publikování obsahu, povolte u šablony zásadu konce doby platnosti a zadejte možnost **Licence k použití obsahu musí být obnoveny vždy po: n dnech**. Místo hodnoty n zadejte počet dnů, po jejichž uplynutí musí uživatel požádat o novou licenci k použití.
