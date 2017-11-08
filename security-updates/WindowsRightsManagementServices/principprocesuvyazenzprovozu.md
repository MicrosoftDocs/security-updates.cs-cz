---
TOCTitle: Princip procesu vyřazení z provozu
Title: Princip procesu vyřazení z provozu
ms:assetid: '57bd9949-9433-437b-93ed-ffb2dff9992e'
ms:contentKeyID: 18113283
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc720276(v=WS.10)'
---

Princip procesu vyřazení z provozu
==================================

Služba RMS vystavuje různé služby, které nabízí, prostřednictvím Internetové informační služby (IIS). Služba certifikace například zapisuje uživatele a jejich počítače a služba správy licencí publikuje obsah a zajišťuje přístup k informacím chráněným službou RMS. Na serveru RMS musí být navíc povolena služba vyřazení z provozu, aby bylo možné zahájit proces vyřazování z provozu. V případě, že je tato služba povolena, jsou zakázány všechny ostatní služby RMS poskytované serverem.

Jakmile bylo na serveru RMS povoleno vyřazování z provozu, mohou aplikace od služby vyřazování z provozu získat klíč obsahu, který umožňuje aplikaci trvale dešifrovat obsah chráněný službou RMS.

Pokud server RMS pracuje v režimu vyřazení z provozu, může klíč obsahu získat každý uživatel bez ohledu na to, zda mu byla nebo nebyla udělena práva na původní obsah chráněný službou RMS, a může tak získat plná práva na obsah.

Po dešifrování by měl uživatel obsah uložit bez ochrany služby RMS. Měli byste vědět, že k tomu, aby uživatel mohl používat službu vyřazení z provozu, musí být zapsán v rámci infrastruktury služby RMS. Přístup k obsahu chráněnému službou RMS nemůže pomocí služby vyřazení z provozu získat uživatel bez aktivovaného klienta RMS.
