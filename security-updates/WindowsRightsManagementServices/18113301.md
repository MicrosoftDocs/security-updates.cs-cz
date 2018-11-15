---
TOCTitle: Klíče obsahu RMS
Title: Klíče obsahu RMS
ms:assetid: '63c814bf-2809-477e-a2db-d90370442075'
ms:contentKeyID: 18113301
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc720284(v=WS.10)'
---

Klíče obsahu RMS
================

Jakmile autor publikuje obsah chráněný službou RMS, vytvoří aplikace s podporou služby RMS symetrický klíč obsahu a pomocí něj zašifruje daný obsah. Služba RMS používá k vytvoření klíče obsahu standard AES (Advanced Encryption Standard).

Klíč obsahu je zahrnut v licenci k publikování a je zašifrován pomocí veřejného klíče serveru RMS, který danou licenci vydal.

Když daný server přijme požadavek na licenci k použití, provede dešifrování klíče obsahu pomocí soukromého klíče serveru a pak klíč obsahu znovu zašifruje pomocí veřejného klíče uživatele, který přijme jako součást požadavku. Klíč obsahu je pak vložen do licence k použití.
