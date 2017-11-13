---
TOCTitle: Nastavení oprávnění k virtuálním adresářům
Title: Nastavení oprávnění k virtuálním adresářům
ms:assetid: '45112111-9608-45b1-9a86-7b313d0a1579'
ms:contentKeyID: 18113292
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747549(v=WS.10)'
---

Nastavení oprávnění k virtuálním adresářům
==========================================

Jakmile bylo povoleno vyřazení z provozu, je k dispozici jako služba. Služba vyřazení z provozu je však virtuálním adresářem služby IIS s přiřazenými oprávněními k přístupu. Uživatelé mohou tuto službu používat pouze v případě, že nastavíte oprávnění k virtuálnímu adresáři a také k vlastnímu souboru, decommission.asmx.

Ve výchozím nastavení je pro virtuální adresář povoleno integrované ověřování systému Windows, k vlastnímu souboru však má přístup pouze systémový účet a účet správce. Po zadání oprávnění pro volitelný seznam řízení přístupu (DACL) souboru decommission.asmx můžete udělit přístup konkrétní skupině důvěryhodných uživatelů, kteří budou moci odebírat vlastní ochranu službou RMS, nebo můžete přístup ke službě povolit všem uživatelům.

Než uživatelé začnou službu vyřazení z provozu používat, je nutné upravit jejich aplikace tak, aby požadavky na licence k použití bylo možné odesílat do tohoto nového kanálu pro vyřazování z provozu. Pro sadu Microsoft Office System 2003 lze uvedený krok provést přidáním položky registru v počítači uživatele. Pokud sadu Office 2003 používáte, lze tento krok provést pomocí následujícího postupu:

1.  Spusťte Editor registru.

2.  Přejděte ke klíči HKEY_CURRENT_USER\Software\Microsoft\Office\11.0\Common\DRM a přidejte nový klíč s názvem Decommissioning.

3.  V klíči Decommissioning přidejte následující novou **řetězcovou hodnotu**, přičemž nahraďte hodnotu *váš-licenční-server* názvem svého serveru RMS:

    `http://váš-licenční-server/_wmcs/licensing`

4.  Potom klepněte na položku pravým tlačítkem myši a po výběru příkazu **Změnit** zadejte údaj hodnoty, která bude odkazovat na službu vyřazení z provozu:

    `http://váš-licenční-server/_wmcs/decommission`

> [!NOTE]
> Pro tento klíč může existovat více položek, pokud je v režimu vyřazování z provozu více serverů RMS organizace. 
