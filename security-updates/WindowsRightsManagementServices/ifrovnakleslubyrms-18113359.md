---
TOCTitle: Šifrování a klíče služby RMS
Title: Šifrování a klíče služby RMS
ms:assetid: '6ed69817-dab0-4845-b2a4-74203f95f7cf'
ms:contentKeyID: 18113359
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747615(v=WS.10)'
---

Šifrování a klíče služby RMS
============================

Chráněný obsah je vždy šifrován. Certifikáty a licence používané službou RMS mohou také obsahovat šifrovaný obsah, který lze dešifrovat pouze odpovídající entitou. Aplikace s podporou služby RMS šifruje data pomocí klíče obsahu. Všem serverům, klientským počítačům a uživatelským účtům s aktualizací RMS SP1 je přiřazen pár 1024bitových klíčů RSA. Služba RMS pomocí těchto klíčů šifruje klíč obsahu v licenci k publikování i k použití a podepisuje své certifikáty a licence. Tento proces zajišťuje, že server umožní přístup pouze oprávněným uživatelům a počítačům.

Tento oddíl se zabývá následujícími tématy:

-   [Definice klíčů služby RMS](https://technet.microsoft.com/b052305c-1db7-434a-bad9-26d704156776)
-   [Klíče serveru RMS](https://technet.microsoft.com/5f4100a1-9aa5-42af-85c8-4bc691022f06)
-   [Klíče počítačů RMS](https://technet.microsoft.com/56e59ec2-f681-4ca2-98c7-72218ab9e9d9)
-   [Klíče klientských certifikátů pro poskytování licencí](https://technet.microsoft.com/28781125-2692-4ff9-99b1-e09227d72966)
-   [Klíče uživatelů](https://technet.microsoft.com/12dad6e2-64e7-4bab-bde7-b72f90f5cb05)
-   [Klíče obsahu RMS](https://technet.microsoft.com/63c814bf-2809-477e-a2db-d90370442075)
