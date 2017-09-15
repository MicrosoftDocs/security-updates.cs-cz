---
TOCTitle: Odebrání ochrany služby RMS z obsahu
Title: Odebrání ochrany služby RMS z obsahu
ms:assetid: 'c30361e3-50d2-4474-a87d-d38de502cf9e'
ms:contentKeyID: 18113427
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747658(v=WS.10)'
---

Odebrání ochrany služby RMS z obsahu
====================================

S dostatečným předstihem rozhodněte, které soubory je třeba obnovit, a určete kdo a kdy má obnovení provést, aby bylo zajištěno, že po vyřazení služby RMS z provozu budou všechny důležité informace zachovány. Po odebrání ochrany služby RMS u všech požadovaných souborů chráněných službou RMS lze server odebrat z infrastruktury.

Proces odebrání ochrany služby RMS z obsahu probíhá následujícím způsobem:

1.  Uživatel by měl z počítače odebrat všechny existující licence k použití. Tím je zajištěno, že klient RMS odešle na server požadavek na získání licence k otevření obsahu. Licence k použití se v klientském počítači ukládají ve složce %USERPROFILE%\\Local Settings\\Data aplikací\\Microsoft\\DRM a používají před názvem souboru předponu EUL.
2.  Uživatel s přístupem k serveru vyřazení z provozu se pokusí otevřít soubor chráněný službou RMS.
3.  Aplikace se připojí k serveru vyřazení z provozu a získá klíč obsahu.
4.  Obsah je dešifrován a lze jej upravit, uložit, předat dál či vytisknout.
5.  Uživatel uloží obsah bez ochrany službou RMS. Obsah nyní mohou otevírat všichni uživatelé, aniž by se museli připojovat k serveru RMS.
