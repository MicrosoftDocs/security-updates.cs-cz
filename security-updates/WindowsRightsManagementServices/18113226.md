---
TOCTitle: Certifikáty účtů práv
Title: Certifikáty účtů práv
ms:assetid: '2ff315cc-211d-4e6e-85e8-56867c2abd94'
ms:contentKeyID: 18113226
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc720230(v=WS.10)'
---

Certifikáty účtů práv
=====================

Organizace musí určit uživatele, kteří budou v jejich systému služby RMS představovat důvěryhodné entity. Za tímto účelem vydává služba RMS certifikáty účtů práv, které spojují účty uživatelů s konkrétními počítači. Certifikát účtu práv daného uživatele musí být uveden v požadavku na klientské certifikáty pro poskytování licencí a na licence k použití. Klientský certifikát pro poskytování licencí umožňuje autorovi publikovat obsah chráněný službou RMS (například soubory nebo e-mail) v režimu offline. Licence k použití umožňuje uživateli využívat obsah chráněný službou RMS. Každý certifikát účtu práv obsahuje veřejný klíč daného uživatele, pomocí kterého jsou šifrována data určená pro tohoto uživatele.

Existují dva typy certifikátů účtů práv: standardní a dočasný. Pro oba typy můžete určit období platnosti. Standardní certifikáty mají trvání určené ve dnech (výchozí nastavení je 365 dní). Dočasné certifikáty účtů mají trvání, které je určeno v minutách (výchozí nastavení je 15 minut). Certifikáty dočasných účtů umožňují uživatelům dočasně používat obsah například ve veřejných místech, kde nemohou získat přístup k počítači, který obvykle používají. To zabraňuje později jinému uživateli používat obsah ve stejném počítači.
