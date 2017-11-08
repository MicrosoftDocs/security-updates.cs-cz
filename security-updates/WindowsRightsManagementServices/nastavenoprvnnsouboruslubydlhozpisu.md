---
TOCTitle: Nastavení oprávnění souboru služby dílčího zápisu
Title: Nastavení oprávnění souboru služby dílčího zápisu
ms:assetid: '737bb69b-fe26-4057-9569-e632f7bbf295'
ms:contentKeyID: 18113367
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747627(v=WS.10)'
---

Nastavení oprávnění souboru služby dílčího zápisu
=================================================

Služba dílčího zápisu je spuštěna na serveru kořenové certifikace a při zajišťování zapisuje na server správy licencí. Ve výchozím nastavení umožňuje služba dílčího zápisu přístup pouze místnímu systémovému účtu na serveru kořenové certifikace. Chcete-li zajistit server správy licencí, musíte se přihlásit na server správy licencí pomocí tohoto účtu. Místní správce na serveru kořenové certifikace může také změnit seznam DACL v souboru služby dílčího zápisu SubEnrollService.asmx a udělit oprávnění k přístupu uživatelskému účtu použitému k provedení zajištění na serveru správy licencí. Soubor SubEnrollService.asmx je umístěn ve virtuálním adresáři Certification na serveru kořenové certifikace.
