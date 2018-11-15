---
TOCTitle: Alternativy k vyřazení serverů RMS z provozu
Title: Alternativy k vyřazení serverů RMS z provozu
ms:assetid: '4d32f35e-997d-4d10-ab66-efe217e853f7'
ms:contentKeyID: 18113276
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc720268(v=WS.10)'
---

Alternativy k vyřazení serverů RMS z provozu
============================================

Pokud chcete službu RMS v organizaci využívat i nadále, ale z nějakého důvodu potřebujete přestat používat určité servery RMS, zvažte následující alternativy vyřazení z provozu.

**Nastavení důvěryhodné domény publikování**

Všechny informace chráněné službou RMS jsou šifrovány soukromým klíčem serveru RMS. Důvěryhodná doména publikování umožňuje importovat soukromý klíč jednoho serveru RMS na jiný server RMS. Díky tomu může jeden server RMS vydávat licence k použití na základě licencí k publikování vydaných jiným serverem RMS. Po vyexportování klíče lze zajištění serveru zrušit a server odinstalovat.

**Nastavení skupiny superuživatelů**

Pokud nelze obsah chráněný službou RMS otevřít, protože k němu nemají práva žádní uživatelé, můžete udělit oprávnění skupiny superuživatelů k úplnému řízení pro veškerý obsah chráněný službou RMS publikovaný daným serverem. Členům skupiny superuživatelů jsou udělena úplná práva vlastníků ve všech licencích k použití vydaných serverem nebo clusterem RMS, u kterých je tato skupina nakonfigurována. To znamená, že členové této skupiny mohou dešifrovat libovolné soubory s chráněným obsahem a odstraňovat jejich ochranu. Člen této skupiny může například odstranit ochranu ze souborů publikovaných bývalým zaměstnancem, aby mohl dané soubory publikovat a spravovat nový vlastník.

Skupina superuživatelů neobsahuje automaticky žádné členy, ani správce. Tato skupina musí v adresáři služby Active Directory existovat jako distribuční skupina s atributem e-mailové adresy stejné hodnoty jako název skupiny ve formátu *název\_skupiny*@*název\_domény*.com. Název skupiny musí přesně odpovídat atributu e-mailové adresy, včetně rozlišení malých a velkých písmen.
