---
TOCTitle: Zápis klienta RMS
Title: Zápis klienta RMS
ms:assetid: '9c1d07bf-7235-4694-8291-ac2e5b221f4a'
ms:contentKeyID: 18113382
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747613(v=WS.10)'
---

Zápis klienta RMS
=================

Klientské počítače se mohou zapsat ke službě publikování RMS a získat tak klientský certifikát pro poskytování licencí, což autorům umožní publikovat obsah chráněný službou RMS i v případě, že jejich počítače nejsou připojeny k podnikové síti. Pokud se tak stane, nebudou licence k publikování s informacemi o právech využití pro obsah chráněný službou RMS a publikovaný v klientském počítači podepsány a vydány službou publikování, ale tímto klientským počítačem.

Služba publikování RMS vydává klientské certifikáty pro poskytování licencí.

Zápis klienta obsahuje následující kroky:

1.  Klientský počítač odešle požadavek na zápis s certifikátem účtu práv daného uživatele službě publikování, která je spuštěna na serveru/clusteru kořenové certifikace nebo na serveru/clusteru správy licencí.
2.  Server na základě nastavení správce sítě ověří, zda je zápis klienta povolen, a zkontroluje, zda není certifikát účtu práv uveden na seznamu vyloučení v konfigurační databázi. Další informace o vytváření seznamů vyloučení získáte v této sadě dokumentace v části Správa zásad vyloučení tématu Provoz serveru RMS.
3.  Služba publikování vytvoří pro klientský počítač pár klíčů. Vytvoří klientský certifikát pro poskytování licencí a vloží do něj veřejný klíč. Zašifruje soukromý klíč pomocí veřejného klíče certifikátu účtu práv a vloží jej do certifikátu.
4.  Služba publikování vydá klientský certifikát pro poskytování licencí pro klientský počítač.
