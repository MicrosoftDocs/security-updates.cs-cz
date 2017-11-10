---
TOCTitle: Zápis serveru kořenové certifikace
Title: Zápis serveru kořenové certifikace
ms:assetid: '3f69d25e-ecae-447f-b741-a819c8cf6227'
ms:contentKeyID: 18113252
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc720250(v=WS.10)'
---

Zápis serveru kořenové certifikace
==================================

Každá instalace služby RMS musí obsahovat nejméně jeden server kořenové certifikace a nepovinně může obsahovat další servery kořenové certifikace v clusteru. První nainstalovaný server kořenové certifikace musí být zapsán ke službě Microsoft Enrollment Services, aby získal certifikát serveru pro poskytování licencí. Tento certifikát slouží jako základ hierarchie důvěryhodnosti v implementaci služby RMS.

Certifikát serveru pro poskytování licencí je možné pro server kořenové certifikace získat některým z následujících způsobů. Požadovaný způsob můžete vybrat při zadávání informací týkajících se zajištění serveru RMS:

-   **Zápis online**. Pokud se může server kořenové certifikace připojit k Internetu, je možné získat certifikát serveru pro poskytování licencí automaticky během zajišťování. Tento způsob je výchozí.
-   **Zápis offline**. Pokud je server kořenové certifikace izolován od Internetu, je možné provést zápis ručně po dokončení zajišťování. Tento krok provedete, jestliže z daného serveru exportujete požadavek na zápis do souboru, který lze přenést do jiného počítače s připojením k Internetu, a odešlete jej službě Microsoft Enrollment Services za účelem získání certifikátu serveru pro poskytování licencí. Pokud je při zajišťování vybrán zápis offline, dokončí služba RMS zajišťování, ale nebude ji možné používat, dokud nebude importován certifikát serveru pro poskytování licencí získaný uvedeným počítačem s připojením. Další informace získáte později v tomto tématu v části [Ruční zápis serveru kořenové certifikace](https://technet.microsoft.com/aecdebb5-b28b-4b58-937a-392bb6ce9643).

Žádost o zápis obsahuje následující informace:

-   Informace o odvolání: Údaje o tom, zda bude instalace služby RMS používat standardní nebo vlastní odvolání (třetích stran). V případě použití odvolání třetích stran nebo odvolání společnosti Microsoft je součástí těchto informací veřejný klíč odvolacího úřadu.
-   Veřejný klíč certifikátu: Veřejný klíč certifikátu poskytovatele licence serveru. Tento veřejný klíč je generován na serveru RMS a odeslán službě Microsoft Enrollment Services za účelem získání certifikátu poskytovatele licence serveru.
-   Skladová položka: Oficiální název skladové položky služby RMS.
-   Verze: Číslo verze sestavení služby RMS.
-   Adresa URL: Základní adresa clusteru serverů RMS.

Pokud služba Microsoft Enrollment Services poskytne odpověď na žádost o zápis, vrátí serveru RMS následující informace ve formátu XML:

-   Certifikát serveru pro poskytování licencí:
-   Řetěz certifikátů podepisujících úřadů.

Stejné informace jsou přeneseny také v případě, že je server kořenové certifikace služby RMS zapsán způsobem online nebo offline. Při použití těchto způsobů nejsou shromážděny žádné další informace.

> [!NOTE]
> Pokud jste vybrali zápis offline a používáte počítač s konfigurací rozšířeného zabezpečení prohlížeče, například počítač se systémem Windows Server 2003 nebo Windows XP Service Pack 2, nezapomeňte za účelem připojení k Internetu a vyžádání certifikátu serveru pro poskytování licencí přidat adresu URL webu služby Enrollment Services do zóny důvěryhodných serverů, aby bylo možné daný certifikát stáhnout. Jedná se o následující adresu URL: https://activation.drm.microsoft.com. Pokud používáte zápis offline, ujistěte se, že jsou v počítači, pomocí kterého službě Microsoft Enrollment Services odesíláte požadavek na zápis, nainstalovány všechny poslední aktualizace certifikátů. Certifikát SSL služby Microsoft Enrollment Services představuje certifikační úřad GTE Cyber Trust Root, který je ve výchozím nastavení důvěryhodný ve všech počítačích se systémem Windows Server 2003. Pokud jste zvolili zápis offline, měli byste zajistit, aby se klienti RMS nepřipojovali k serveru RMS za účelem získání licencí, dokud nebude proveden zápis. Jestliže se klienti budou připojovat k serveru RMS, který není zapsán, dojde u webových služeb k chybě a nebude možné je využívat. Pokud nemůžete zajistit, aby se klienti k serveru RMS nepřipojovali, bude nejvhodnější po provedení zápisu obnovit službu IIS. Tímto způsobem odstraníte případné chyby. 
