---
TOCTitle: Publikování offline
Title: Publikování offline
ms:assetid: 'f6384ed2-f917-442e-aa63-c1394a1c4d06'
ms:contentKeyID: 18113503
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747741(v=WS.10)'
---

Publikování offline
===================

Publikování offline se od publikování online liší způsobem, jakým aplikace s podporou služby RMS získává licenci k publikování.

Před publikací obsahu v režimu offline musí autoři získat klientský certifikát pro poskytování licencí, dokud mají po síti přístup k serveru kořenové certifikace.

Proces publikování offline obsahuje následující kroky:

1.  Autor vytvoří dokument pomocí aplikace s podporou služby RMS a určí práva a podmínky vztahující se na daný obsah.
2.  Pokud autor uloží soubor, umožní klientský certifikát pro poskytování licencí místnímu počítači nebo klientovi vydat a podepsat pro soubor licenci k publikování.
    Licence k publikování obsahuje dvě kopie klíče obsahu: jedna je zašifrována pomocí veřejného klíče klientského certifikátu pro poskytování licencí a druhá je zašifrována pomocí veřejného klíče serveru, který vydal klientský certifikát pro poskytování licencí. Obsahuje též adresu URL serveru. Tyto dva veřejné klíče spolu s adresou URL pocházejí z klientského certifikátu pro poskytování licencí.
3.  Počítač pomocí klientského certifikátu pro poskytování licencí vytvoří licenci vlastníka, což je zvláštní licence k použití, která autorovi uděluje právo využívat obsah chráněný službou RMS v režimu offline. Klientský certifikát pro poskytování licencí použije příslušný soukromý klíč k dešifrování symetrického klíče obsahu z licence k publikování a poté jej znovu zašifruje do licence vlastníka.
4.  Aplikace zašifruje soubor s použitím klíče obsahu a sváže licenci k publikování se souborem. Licence umožňující dešifrování tohoto souboru může vydávat pouze server RMS, který vydal příslušnou licenci k publikování, nebo server náležící do důvěryhodné domény publikování.
