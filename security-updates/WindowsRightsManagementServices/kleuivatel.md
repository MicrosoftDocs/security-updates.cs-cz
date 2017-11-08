---
TOCTitle: Klíče uživatelů
Title: Klíče uživatelů
ms:assetid: '12dad6e2-64e7-4bab-bde7-b72f90f5cb05'
ms:contentKeyID: 18113221
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc720202(v=WS.10)'
---

Klíče uživatelů
===============

Uživateli služby RMS je přiřazen pár 1024bitových klíčů RSA. Pár klíčů uživatele je uložen v konfigurační databázi služby RMS, takže daný uživatel v celém systému služby RMS používá vždy stejný pár klíčů.

Veřejný klíč uživatele je obsažen v certifikátu účtu práv. Pomocí tohoto klíče je šifrován klíč obsahu v licenci k použití, takže na základě této licence může obsah chráněný službou RMS využívat pouze určitý uživatel.

Stejný certifikát účtu práv obsahuje také soukromý klíč daného uživatele, který je šifrován pomocí veřejného klíče klientského počítače. Tímto způsobem je zajištěno, že certifikát účtu práv lze použít pouze v počítači, pro který byl vydán. Každý certifikát účtu práv daného uživatele však bude obsahovat stejný pár klíčů. Soukromý klíč uživatele je nezbytný k využití jakéhokoli obsahu chráněného službou RMS.
