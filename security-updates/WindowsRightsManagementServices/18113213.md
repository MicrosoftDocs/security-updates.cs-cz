---
TOCTitle: Skupiny zabezpečení služby RMS
Title: Skupiny zabezpečení služby RMS
ms:assetid: '25749a83-8c12-48ec-96ad-296d31fd55d4'
ms:contentKeyID: 18113213
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc720215(v=WS.10)'
---

Skupiny zabezpečení služby RMS
==============================

Instalační program služby RMS vytvoří dvě skupiny: skupinu RMS Service Group a Super Users.

Skupina RMS Service Group představuje místní skupinu zabezpečení, které jsou udělena dostatečná oprávnění k získání přístupu ke všem prostředkům nezbytným pro provádění operací služby RMS. Během instalace zadá správce uživatelský účet, který bude sloužit jako účet služby RMS. Tento uživatelský účet je automaticky zařazen jako člen do skupiny RMS Service Group, a jsou mu tedy přidělena také příslušná oprávnění. Služba RMS je pod tímto uživatelským účtem obvykle spuštěna za běžného provozu.

Další důležitou skupinou služby RMS je skupina Super Users. Této skupině je umožněno úplné řízení veškerého obsahu, což znamená, že její člen může dešifrovat všechny soubory s obsahem chráněným službou RMS a odebrat z nich veškerou ochranu. Ve výchozím nastavení nemá skupina Super Users žádné členy ani do ní automaticky nepatří správci služby RMS. Správa členství v této skupině je klíčová pro zajištění zabezpečení obsahu chráněného službou RMS. Další informace získáte v této sadě dokumentace v části Práce se skupinou superuživatelů tématu Provoz serveru RMS.
