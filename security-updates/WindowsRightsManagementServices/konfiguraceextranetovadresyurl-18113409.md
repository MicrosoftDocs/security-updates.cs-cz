---
TOCTitle: Konfigurace extranetové adresy URL
Title: Konfigurace extranetové adresy URL
ms:assetid: '88fec9ff-c96c-4d20-8856-0485e7507572'
ms:contentKeyID: 18113409
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747661(v=WS.10)'
---

Konfigurace extranetové adresy URL
==================================

Chcete-li v instalaci služby RMS podporovat extranetové uživatele, můžete přidat server správy licencí nebo cluster správy licencí vyhrazený pro použití v extranetu.

Při zajištění extranetového serveru správy licencí je nutné pro něj určit adresu URL clusteru, stejně jako u ostatních serverů RMS. Určená adresa URL je obvykle vnitřní adresou URL, která není pro extranetové uživatele dostupná. Jedná se o adresu URL, kterou služba RMS používá pro zjišťování služeb. Musí se jednat o platnou adresu URL.

Pokud přidáváte adresu URL clusteru extranetu na server RMS, který je již v provozu, je nutné získat pro aktuální klienty RMS nové klientské certifikáty pro poskytování licencí a zajistit tak jejich přístup ke clusteru extranetu pro správu licencí.

Další informace získáte v tomto tématu později v části [Přidání extranetové adresy URL clusteru](https://technet.microsoft.com/12c83186-ce9e-4100-bbd1-d87a885331c7).
