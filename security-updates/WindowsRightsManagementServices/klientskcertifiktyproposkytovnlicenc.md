---
TOCTitle: Klientské certifikáty pro poskytování licencí
Title: Klientské certifikáty pro poskytování licencí
ms:assetid: 'bfb36387-3e15-4cde-8b8f-482219569a64'
ms:contentKeyID: 18113493
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747744(v=WS.10)'
---

Klientské certifikáty pro poskytování licencí
=============================================

Klientský certifikát pro poskytování licencí uděluje autorovi oprávnění publikovat obsah chráněný službou RMS bez připojení k podnikové síti.

Pokud chce autor získat klientský certifikát pro poskytování licencí, vydá nejprve z klientského počítače požadavek na zápis klienta pro server kořenové certifikace nebo server správy licencí. Server poté vrátí klientský certifikát pro poskytování licencí pro daný počítač.

Klientský certifikát pro poskytování licencí obsahuje veřejný a soukromý klíč klientského certifikátu pro poskytování licencí zašifrované veřejným klíčem autora, který o daný certifikát požádal. Rovněž obsahuje veřejný klíč serveru, který vydal certifikát, který je podepsán soukromým klíčem serveru, který vydal certifikát. Soukromý klíč klientského certifikátu pro poskytování licencí se používá k podpisu licencí k publikování, které autor vytvořil.
