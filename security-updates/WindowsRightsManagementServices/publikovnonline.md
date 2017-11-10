---
TOCTitle: Publikování online
Title: Publikování online
ms:assetid: '962c4e83-cf34-4c61-9589-31d24b0299fb'
ms:contentKeyID: 18113428
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747694(v=WS.10)'
---

Publikování online
==================

Následující diagram znázorňuje proces publikování online.

![](images/Cc747694.897e47b6-fffe-4b11-bc9f-be58539b9f19(WS.10).gif)

Proces publikování online obsahuje následující kroky:

1.  Autor obsahu vytvoří dokument a pomocí aplikace s podporou služby RMS zadá uživatele a nastaví pro daný obsah požadovaná práva a podmínky.

2.  Aplikace s podporou služby RMS vygeneruje symetrický klíč obsahu a odešle serveru certifikace nebo serveru správy licencí požadavek na licenci k publikování. Požadavek obsahuje klíč obsahu a parametry použití.

3.  Server správy licencí vygeneruje licenci k publikování, zašifruje klíč obsahu pomocí veřejného klíče serveru a vrátí licenci k publikování aplikaci s podporou služby RMS.

4.  Aplikace zašifruje soubor s použitím klíče obsahu a sváže licenci k publikování se souborem.

5.  Aplikace s podporou služby RMS v počítači uživatele, který chce obsah využít, odešle na server RMS (který vydal příslušnou licenci k publikování) požadavek (s certifikátem účtu práv tohoto uživatele) na licenci k použití pro daný dokument.

6.  Server RMS ověří platnost pověření daného uživatele. V případě úspěšného ověření uživatele je vygenerována licence k použití, která je vrácena aplikaci s podporou služby RMS v počítači uvedeného uživatele.

7.  Tato aplikace otevře příslušný dokument a na základě parametrů definovaných v licenci k použití udělí uživatelská práva.
