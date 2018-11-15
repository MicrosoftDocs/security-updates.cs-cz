---
TOCTitle: Vyloučení aplikací
Title: Vyloučení aplikací
ms:assetid: 'b68ae4b2-b9ba-44ae-90cb-c88df600ec86'
ms:contentKeyID: 18113407
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747644(v=WS.10)'
---

Vyloučení aplikací
==================

Můžete určit verzi aplikace s podporou správy přístupových práv, s níž budou porovnány všechny požadavky licencování. V případě vyloučení aplikací je u každé licence k použití nastavena podmínka, že licenci lze svázat pouze s obsahem chráněným správou přístupových práv, pro který je vydána, není-li aplikace požadující licenci uvedena na seznamu vyloučení.

To může být užitečné například v případě, že společnost nasazuje aktualizaci zabezpečení aplikace. Správci systému mohou aktualizaci zabezpečení v klientských počítačích instalovat obvyklým způsobem. Pak mohou nastavit zásady vyloučení aplikací definované prostřednictvím informací o verzi aplikace, která používá web pro správu. Tyto zásady vyloučení znemožňují službě RMS vydávat licence pro klienty s předchozí verzí daného softwaru.

Aplikace s podporou správy přístupových práv jsou vyloučeny na základě názvu souboru a čísla verze. Tímto postupem můžete zajistit, že si uživatelé nainstalují novější a zabezpečenější verzi aplikace v okamžiku, kdy bude k dispozici. V organizaci může být například nasazována verze 1.0.4.2315 aplikace s podporou správy přístupových práv. Dodavatel aplikace pak objeví chybu v zabezpečení a vydá verzi 1.0.4.4200, v níž je daná chyba odstraněna. Kromě přechodu na novou verzi aplikace můžete vytvořit zásadu vyloučení, která uživatelům znemožní používat chráněný obsah pomocí předchozí verze aplikace.

Podobně jako v případě dalších typů vyloučení je třeba vyloučení aplikace konfigurovat na každém clusteru, na němž má být použito.

Pokud uvedené zásady vyloučení nastavíte na serveru, nebudou klienti moci použít vyloučenou aplikaci k zadání požadavku na obsah chráněný správou přístupových práv a k svázání nových licencí k použití s tímto obsahem. Vyloučené aplikace ovšem budou moci použít k práci se soubory licencovanými dříve.

> [!NOTE]
> Server RMS vyžaduje zadání verze aplikace ve formátu čtyřmístného čísla odděleného tečkami (\#.\#.\#.\# ). U některých aplikací je však číslo verze určeno dvoumístnými nebo třímístnými čísly oddělenými tečkou. V takovém případě je vhodné přidat hodnotu .0, aby číslo verze odpovídalo formátu vyžadovanému serverem RMS. 
