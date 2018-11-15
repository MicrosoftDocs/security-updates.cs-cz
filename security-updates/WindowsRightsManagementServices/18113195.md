---
TOCTitle: Zajištění redundance dat a vyrovnávání zatížení
Title: Zajištění redundance dat a vyrovnávání zatížení
ms:assetid: '162d547c-78a7-4848-b43e-58e481832af2'
ms:contentKeyID: 18113195
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc720199(v=WS.10)'
---

Zajištění redundance dat a vyrovnávání zatížení
===============================================

Chcete-li zajistit, aby uživatelé mohli získávat licence a publikovat obsah, kdykoli potřebují, je velmi vhodné nasadit redundantní servery RMS prostřednictvím clusterů. Minimální požadavek představuje nasazení clusteru kořenové certifikace, který je tvořen nejméně dvěma servery. Pokud zároveň nasazujete zvláštní server správy licencí za účelem podpory specifických potřeb správy licencí vyžadovaných individuální skupinou v organizaci, měli byste tento server také nasadit jako cluster s nejméně dvěma servery.

Více fyzických serverů clusteru kořenové certifikace nebo libovolného clusteru správy licencí tvoří webovou farmu v rámci sdílené adresy URL nebo virtuální adresy. Jestliže organizace využívá serverovou farmu, můžete službu RMS integrovat do každého používaného mechanismu virtuálního adresování, jako je například kruhové dotazování (round robin) DNS, služba Vyrovnávání zatížení sítě nebo přizpůsobené hardwarové řešení.

Kromě vyrovnávání zatížení přináší virtuální adresování další výhody, pokud je použijete se službou RMS, protože odstraňuje závislost na jakémkoli fyzickém serveru určeném pro služby certifikace nebo správy licencí. Žádný z počítačů koncových uživatelů nepotřebuje přímý přístup k jednotlivým počítačům obsaženým v clusteru.
