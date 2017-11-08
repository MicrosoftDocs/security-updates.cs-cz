---
TOCTitle: Plánování zabezpečení pro službu RMS
Title: Plánování zabezpečení pro službu RMS
ms:assetid: 'eb0fa784-1246-44aa-be31-2c332db7d09c'
ms:contentKeyID: 18113490
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747719(v=WS.10)'
---

Plánování zabezpečení pro službu RMS
====================================

Stejně jako u ostatních serverů v organizaci musí zabezpečení tvořit nedílnou součást plánování nasazení. Služba RMS je implementována jako webová služba, takže přístup k ní je možné řídit stejným způsobem jako u ostatních webových služeb, a to pomocí seznamů řízení přístupu a protokolu SSL (Secure Sockets Layer).

Službu RMS lze také implementovat jako součást domény s řízeným přístupem, jestliže část daného nasazení volá službu RMS za účelem zajištění další vrstvy řízení citlivých informací.

Vzhledem k tomu, že služba RMS šifruje obsah prostřednictvím systému soukromých klíčů, je nutné do plánu zabezpečení zahrnout také zálohování a správu soukromého klíče této služby.

Tato část obsahuje následující témata:

-   [Určení požadavků přístupu](https://technet.microsoft.com/eb2ce9a5-0430-4811-bd40-4a94a84426a8)
-   [Definování požadavků správy klíčů](https://technet.microsoft.com/f0e08fb8-bf5e-4278-a09f-daa57696e786)
