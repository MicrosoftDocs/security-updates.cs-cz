---
TOCTitle: Klíče klientských certifikátů pro poskytování licencí
Title: Klíče klientských certifikátů pro poskytování licencí
ms:assetid: '28781125-2692-4ff9-99b1-e09227d72966'
ms:contentKeyID: 18113217
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc720221(v=WS.10)'
---

Klíče klientských certifikátů pro poskytování licencí
=====================================================

Autoři mohou získat klientské certifikáty pro poskytování licencí za účelem publikování obsahu chráněného službou RMS i v případě, že nejsou připojeni k síti s podporou služby RMS. Klientskému certifikátu pro poskytování licencí je přiřazen pár 1024bitových klíčů RSA.

Klient RMS používá veřejný klíč klientského certifikátu pro poskytování licencí při vydávání licence k publikování, a to k následujícím úlohám:

-   k šifrování symetrického klíče obsahu,
-   k podpisu licence k publikování, které jsou vydány lokálně v situaci, kdy uživatel není připojen k síti.
