---
TOCTitle: Vyloučení verzí operačního systému Windows
Title: Vyloučení verzí operačního systému Windows
ms:assetid: '8b8a184d-ac0e-4a43-822c-d2fae2faf484'
ms:contentKeyID: 18113360
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747590(v=WS.10)'
---

Vyloučení verzí operačního systému Windows
==========================================

Klient Služby správy přístupových práv v systému Microsoft® Windows® (RMS) 1.0 je podporován v počítačích se systémem Microsoft Windows 98 Druhé vydání nebo Windows Millennium Edition. Tyto systémy však nepodporují ověřování NTLM. Z důvodu zvýšení zabezpečení obsahu může být proto nutné znemožnit uživatelům počítačů, v nichž je spuštěn jeden z těchto systémů, používání obsahu chráněného správou přístupových práv a požadovat po nich přechod na verzi systému Windows vyšší než Windows Millennium Edition.

Pokud nastavíte zásady vyloučení uživatelů založené na verzi systému Windows, je do všech licencí k použití vložena podmínka, která znemožňuje použití těchto licencí v klientech se systémem Windows 98 Druhé vydání a Windows Millennium Edition. Vyloučení verze systému Windows je třeba nastavit na stránce **Zásady vyloučení** webu pro správu všech clusterů, na nichž má být použita.
