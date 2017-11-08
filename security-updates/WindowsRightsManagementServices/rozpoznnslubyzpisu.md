---
TOCTitle: Rozpoznání služby zápisu
Title: Rozpoznání služby zápisu
ms:assetid: 'bbeb00bd-04e0-4df6-8615-76aa8125b620'
ms:contentKeyID: 18113480
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747737(v=WS.10)'
---

Rozpoznání služby zápisu
========================

První server RMS doménové struktury, který chcete zajistit, se musí připojit ke službě Microsoft Enrollment Services, zapsat se k ní a získat certifikát serveru pro poskytování licencí. Za účelem získání adresy URL služby Enrollment Services vytvoří instalační program služby RMS požadavek UDDI na [web Microsoft UDDI](http://go.microsoft.com/fwlink/?linkid=14794) (http://go.microsoft.com/fwlink/?LinkId=14794). Další servery zajišťované jako součást clusteru kořenové certifikace nemusí certifikáty serveru pro poskytování licencí získávat, protože sdílí konfiguraci prvního serveru kořenové certifikace.
