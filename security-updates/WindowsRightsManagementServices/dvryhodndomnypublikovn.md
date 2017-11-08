---
TOCTitle: Důvěryhodné domény publikování
Title: Důvěryhodné domény publikování
ms:assetid: 'bca1c33a-d3ef-42b5-adbe-6e104979a71f'
ms:contentKeyID: 18113482
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747738(v=WS.10)'
---

Důvěryhodné domény publikování
==============================

Servery RMS ve výchozím nastavení nevydávají licence k použití na základě licencí k publikování vydaných serverem RMS z jiného clusteru. Existují však situace, kdy stejný server či cluster nemůže vydat pro určitou část chráněného obsahu zároveň licenci k publikování a licenci k použití. K tomu může dojít v případě, že je určitý cluster služby RMS vyřazen a nahrazen jiným (například při sloučení dvou společností). V této situaci je nutné umožnit clusteru služby RMS vydávání licencí k použití na základě licencí k publikování vytvořených jiným clusterem služby RMS.

Cluster služby RMS můžete nakonfigurovat tak, aby pokládal za důvěryhodné licence k publikování vydané jiným clusterem této služby a na jejich základě vydával licence k použití, a to implementací důvěryhodné domény publikování. Za tímto účelem importujte certifikát serveru pro poskytování licencí a soukromý klíč z partnerského serveru a poté jej přidejte do seznamu důvěryhodných domén publikování. Importované soukromé klíče slouží pouze k dešifrování podepsaných licencí k publikování a nikoli k podepisování nových licencí.

Další informace o důvěryhodných doménách publikování a podrobné pokyny získáte v této sadě dokumentace v částech Přidání a odebrání důvěryhodných domén publikování a Vytvoření zásad důvěryhodnosti tématu Provoz serveru RMS.
