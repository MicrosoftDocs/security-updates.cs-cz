---
TOCTitle: Model zabezpečení služby RMS
Title: Model zabezpečení služby RMS
ms:assetid: '665db831-366d-4dca-9bb3-cc2912481fe1'
ms:contentKeyID: 18113343
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747598(v=WS.10)'
---

Model zabezpečení služby RMS
============================

Během jednotlivých operací získává služba RMS přístup k různým prostředkům, včetně databázového serveru, služby Active Directory, fronty zpráv a místního pevného disku. Instalační program služby RMS navíc vytváří a poskytuje určité prostředky nutné k provádění operací, jako jsou například položky protokolu SOAP, webové stránky, fronty zpráv protokolování a další. Tento program také nakonfiguruje volitelné seznamy řízení přístupu (DACL) u prostředků, které vytváří a poskytuje, a zároveň pro každý prostředek nastaví ověřování služby IIS.

V tomto oddílu najdete informace o tom, jak služba RMS konfiguruje zabezpečení využívaných prostředků a jak k nim získává přístup během následujících fází operací: konfigurace, zajišťování a běžné operace.

Tento oddíl se zabývá následujícími tématy:

-   [Skupiny zabezpečení služby RMS](https://technet.microsoft.com/25749a83-8c12-48ec-96ad-296d31fd55d4)
-   [Režimy zabezpečení služby RMS](https://technet.microsoft.com/d7792293-5bb2-4232-9d48-e81e87ab6219)
-   [Zabezpečení během instalace služby RMS](https://technet.microsoft.com/0a3d40b2-f27e-4e63-baff-a9c8433f5f91)
-   [Zabezpečení během zajišťování](https://technet.microsoft.com/9f1282c5-5642-4870-a9a4-c3a485f8ff76)
-   [Zabezpečení při běžném provozu služby RMS](https://technet.microsoft.com/98f3d584-6320-4aa1-9959-7133cfdb6df7)
