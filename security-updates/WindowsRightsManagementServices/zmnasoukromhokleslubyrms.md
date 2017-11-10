---
TOCTitle: Změna soukromého klíče služby RMS
Title: Změna soukromého klíče služby RMS
ms:assetid: 'da32137e-394a-42b2-9552-ba20f4547c23'
ms:contentKeyID: 18113522
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747765(v=WS.10)'
---

Změna soukromého klíče služby RMS
=================================

Při zajišťování vytvoří služba RMS soukromý klíč pro server RMS. Soukromý klíč serveru RMS je zašifrován a uložen do konfigurační databáze. Je vhodné jej zálohovat a uložit v zabezpečeném umístění. Navíc můžete zvážit zabezpečení soukromého klíče serveru RMS pomocí hardwarového modulu zabezpečení, protože se tento klíč používá v šifrovacím schématu pro veškerý obsah chráněný serverem RMS. Pokud by jakýmkoli způsobem došlo k odhalení soukromého klíče serveru RMS, je nutné zrušit zajištění služby RMS na serveru a potom novým zajištěním služby RMS získat nový soukromý klíč serveru RMS.

Jestliže byl pomocí daného serveru chráněn obsah, měli by být upozorněni všichni vlastníci obsahu a obsah by měl být znovu publikován prostřednictvím serveru RMS s novým soukromým klíčem. Všechny kopie obsahu chráněného odhaleným soukromým klíčem by měly být zničeny, protože již nemají dostatečnou ochranu.

> [!IMPORTANT]
> Bez ohledu na to, zda byl daný server zapsán ke službě Microsoft Enrollment Services, je nutné u něj opakovat proces zajištění, aby bylo možné získat nový soukromý klíč. Pokud budete server RMS pouze znovu zapisovat, bude použit jeho předchozí soukromý klíč. 
