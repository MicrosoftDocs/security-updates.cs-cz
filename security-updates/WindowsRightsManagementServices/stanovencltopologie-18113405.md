---
TOCTitle: Stanovení cílů topologie
Title: Stanovení cílů topologie
ms:assetid: '8275a04d-3e5b-40b0-be9d-2f31b7aeca6b'
ms:contentKeyID: 18113405
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747652(v=WS.10)'
---

Stanovení cílů topologie
========================

Jedním z důležitých kroků při návrhu topologie je správné stanovení cílů. Mezi hlavní oblasti, které by měl návrh topologie služby RMS zahrnovat, patří například následující hlediska:

-   **Náklady na správu.** Topologie webu musí minimalizovat náklady na správu. Znamená to centralizaci správy serveru, kdekoli je to možné, a minimalizaci počtu použitých serverů.
-   **Čekací doba v síti.** Čekací doba v síti mezi klientem a serverem se u uživatelů projeví jako zpoždění při otevírání e-mailů a dokumentů. Zajistěte, aby byla čekací doba během nejméně 90 procent požadovaného času nižší než dvě sekundy v každém směru.
-   **Spolehlivost.** Síť mezi klientem a serverem by měla být dostatečně spolehlivá. Poměr chyb (tj. ztráta nebo poškozená transakce) jednoho požadavku a odezvy HTTP by měl být nižší než 5 procent.

Uvedené informace by měly sloužit pouze jako obecná vodítka. Je nutné, abyste si stanovili vlastní cíle založené na požadavcích a prostředcích příslušné organizace. Stanovení cílů je základem pro zjištění, zda určitá topologie vyhovuje daným potřebám. Existuje mnoho faktorů, které ovlivňují splnění daných cílů, jako je například počet uživatelů, požadavky na licence, dotazy, zprávy a další aspekty přenosu dat spojeného se službou RMS. Na dosažení cílů topologie může mít navíc významný vliv strategie nasazení, včetně konkrétních domén a doménových struktur, do nichž chcete službu RMS nasadit. Během celého procesu navrhování topologie byste měli mít své cíle stále na paměti a měli byste určovat, jak je ovlivní jednotlivé procedury návrhu.
