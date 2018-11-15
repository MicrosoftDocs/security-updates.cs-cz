---
TOCTitle: Aktivace počítače RMS
Title: Aktivace počítače RMS
ms:assetid: '09a0d631-9860-477f-9d10-df61b3bfe125'
ms:contentKeyID: 18113275
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc720182(v=WS.10)'
---

Aktivace počítače RMS
=====================

Aktivace počítače představuje předpoklad pro publikování nebo používání obsahu chráněného službou RMS v klientském počítači. Jedná se o proces, při kterém je klientskému počítači vydán jedinečný bezpečnostní modul a odpovídající certifikát počítače RMS. Bezpečnostní modul obsahuje soukromý klíč počítače, zatímco certifikát počítače obsahuje veřejný klíč počítače. Vzhledem k tomu, že bezpečnostní modul obsahuje soukromý klíč počítače, je hlavním zaregistrovaným objektem zabezpečení pro šifrování a dešifrování. Každému uživateli daného počítače bude přiřazen jedinečný certifikát počítače vytvořený během procesu aktivace počítače.

Tento proces se v klientovi RMS s aktualizací Service Pack 1 od stejného procesu ve verzi 1 podstatně liší. Klienti RMS s aktualizací Service Pack 1 se aktivují sami. Jakmile přihlášený uživatel instaluje klienta RMS nebo poprvé použije funkci služby RMS, spustí klient proces aktivace, během kterého je pomocí rozhraní Crypto API dodávaného se systémem Windows generováno několik sad klíčů. Prostřednictvím těchto klíčů se provádí několik šifrování, při kterých je generován certifikát počítače. Ten váže uživatele, počítač a klienta RMS dohromady v rámci hierarchie důvěryhodnosti služby RMS.
