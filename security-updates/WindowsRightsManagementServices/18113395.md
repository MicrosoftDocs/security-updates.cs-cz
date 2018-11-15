---
TOCTitle: Novinky v aktualizaci Service Pack 2
Title: Novinky v aktualizaci Service Pack 2
ms:assetid: 'a944cb73-d900-42bb-b7aa-92916dead408'
ms:contentKeyID: 18113395
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747629(v=WS.10)'
---

Novinky v aktualizaci Service Pack 2
====================================

Služba správy přístupových práv (RMS) s aktualizací Service Pack 2 (SP2) zajišťuje podporu následujících funkcí:

-   **Nativní podpora pro Microsoft® SQL Server™ 2005:** V předchozích verzích služby RMS vyžadovalo její použití se serverem SQL Server 2005 zvláštní postup. Informace o tomto zvláštním postupu získáte v článku 913372 znalostní báze Microsoft Knowledge Base ([http://go.microsoft.com/fwlink/?LinkId=68638](http://go.microsoft.com/fwlink/?linkid=68638)) (stránka může být v angličtině). Ve službě RMS s aktualizací SP2 byl uvedený problém vyřešen.

-   **Microsoft Office SharePoint® Server 2007:** Tato verze podporuje Office SharePoint Server 2007. Knihovna dokumentů serveru Office SharePoint Server 2007 automaticky používá oprávnění služby RMS u dokumentů na základě práv tohoto serveru při jejich stahování. Uvedený postup zajišťuje instalace klienta RMS s aktualizací SP2 na serveru Office SharePoint Server 2007. Nedoporučujeme instalovat server RMS s aktualizací SP2 a Office SharePoint Server 2007 do stejného počítače.

-   **Zvýšené zabezpečení zpráv pro databázi protokolování:** Všechny zprávy služby Řízení front zpráv odesílané ze serverů RMS do databáze protokolování služby RMS obsahují v této verzi digitální podpis.

-   **Větší velikost dávek na serveru:** V této verzi již aplikace s podporou služby RMS dokáže načíst více licencí k použití pro různé uživatelské účty z jediného požadavku na licenci pro server RMS. V důsledku se pak zvýší výkon omezením režie zpracování mnoha požadavků na licence pro stejnou část obsahu chráněného právy.

-   **Zdokonalené rozšiřování skupin mezi doménovými strukturami:** V této verzi se rozšiřování skupin mezi doménovými strukturami ve službě RMS provádí prostřednictvím požadavku SOAP (Simple Object Access Protocol) odeslaného nové webové službě ASP.NET, která je spuštěna na serveru RMS.
