---
TOCTitle: Optimalizace výkonu
Title: Optimalizace výkonu
ms:assetid: '24dc9ca4-652b-41a6-9a99-95fdeca9120b'
ms:contentKeyID: 18113240
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc720220(v=WS.10)'
---

Optimalizace výkonu
===================

Témata tohoto oddílu obsahují informace o optimalizaci výkonu nasazení služby RMS.

Optimalizace výkonu adresářových služeb
---------------------------------------

Můžete sledovat čítače výkonu adresářových služeb, které jsou součástí služby RMS. V případě potřeby můžete výkon optimalizovat změnou nastavení registru řídících atributy mezipaměti služby Active Directory.

Nastavení registru řídí následující atributy mezipaměti služby Active Directory:

-   Maximální počet zaregistrovaných objektů uložených do mezipaměti
-   Doba platnosti informací uložených v mezipaměti pro zaregistrované objekty zabezpečení
-   Maximální počet skupin uložených do mezipaměti
-   Doba platnosti informací uložených v mezipaměti pro skupiny
-   Maximální počet položek členství ve skupinách
-   Doba platnosti informací uložených v mezipaměti pro členství ve skupinách

Obecně platí, že čím delší je platnost položek v mezipaměti nebo čím více je těchto položek, tím rychleji je služba RMS schopna reagovat na požadavky vyžadující získání informací adresářových služeb. Pokud jsou tyto informace uloženy v mezipaměti služby Active Directory, není třeba přechod do služby Active Directory za účelem provedení hledání. Tím je zkrácena doba odpovědi na požadavek.

Nevýhodou většího množství informací uloženého v mezipaměti služby Active Directory je vyšší potřeba systémových paměťových prostředků. Při konfiguraci nastavení registru je dále třeba uvážit, že čím delší je platnost položek v mezipaměti, tím pravděpodobnější je, že některé výsledky vrácené z mezipaměti služby Active Directory budou neplatné. K tomu může dojít v případě, kdy jsou informace změněny ve službě Active Directory, ale tato změna nebyla dosud zohledněna v mezipaměti služby Active Directory. Pokud se obsah služby Active Directory často mění, je vhodné nastavit kratší dobu platnosti informací uložených v mezipaměti. Určená hodnota by měla odpovídat frekvenci změn ve službě.

Čítače výkonu adresářových služeb jsou popsány v tomto tématu později v části [RMS: Čítače výkonu služby DirectoryServices](https://technet.microsoft.com/37afea1d-f320-4040-96d8-57c0b45e6d46). Další informace týkající se jejich použití naleznete v tomto tématu v části [Použití čítačů výkonu](https://technet.microsoft.com/096c3b17-c082-46c4-939c-4373af0c9dec) uvedené již dříve. Čítače sledují „zásahy“ a „neúspěšné pokusy“. V případě každého neúspěšného pokusu musí služba RMS provést hledání ve službě Active Directory.

Další informace týkající se nastavení registru a postupu při jejich změně naleznete v tomto tématu později v části [Změna nastavení mezipaměti služby Active Directory](https://technet.microsoft.com/8789a7a5-2065-4fae-9104-e0a70f1f2fb6).

Optimalizace nastavení fondu připojení služby Active Directory
--------------------------------------------------------------

Chcete-li zvýšit výkon systému, můžete přidat a změnit klíče registru, které řídí nastavení fondu připojení LDAP (Lightweight Directory Access Protocol) služby Active Directory. Konfigurace klíčů registru je popsána v tomto tématu později v části [Změna nastavení registru fondu připojení](https://technet.microsoft.com/c61d91db-a1ad-4ca5-a492-015da629afbc).

Služba RMS je navržena pro optimalizaci připojení LDAP. Tato služba vytváří jedno připojení pro každý globální katalog služby Active Directory, přičemž každé připojení může obsluhovat několik podprocesů. Aby byla zajištěna robustnost systému, je udržován fond připojení pro obsluhu požadavků. Aby nedocházelo k příliš velkému zatížení jednoho globálního katalogu, používá služba RMS algoritmus pro rozdělení požadavků založený na provádění vyrovnávání zatížení mezi globálními katalogy uvedenými v seznamu globálních katalogů určených k dotazování. Dále automaticky zpracovává chyby LDAP a podle potřeby směruje požadavky do jiného globálního katalogu.

Služba RMS vytváří seznam globálních katalogů určených k dotazování pomocí algoritmu pro zjišťování topologie. Je možné určit minimální a maximální počet dostupných globálních katalogů, které musí algoritmus pro zjišťování topologie najít, než je možné službu RMS spustit. Algoritmus pro zjišťování topologie nejprve hledá globální katalogy v aktuální síti. Pokud jsou třeba další globální katalogy, hledá je v jiných sítích. Je také možné určit maximální počet připojení, která mohou být nedostupná, než služba RMS přestane přijímat požadavky. Pokud jeden nebo několik globálních katalogů přestane být později k dispozici, algoritmus pro zjišťování topologie začne hledat náhradní globální katalogy pro přidání do seznamu dotazů.

Globální katalogy, které má služba RMS používat, můžete také zadat sami. V takovém případě nebude nástroj zjišťování topologie katalogy pro přidání do seznamu dotazů hledat.

Dále je možné konfigurovat nastavení způsobu, jakým služba RMS provádí vyrovnávání zatížení mezi globálními katalogy. Můžete určit, jak důležité (relativně vůči sobě) jsou následující hlediska při rozhodování, zda odeslat určitý požadavek do určitého globálního katalogu:

-   **Kruhové dotazování (WtRoundRobin)**. Tento parametr určuje relativní důležitost vyrovnávání zatížení využívajícího princip kruhového dotazování. Výchozím nastavením váhy je hodnota 1, což znamená, že se jedná o nejméně důležité hledisko, které server bere v potaz při výběru globálního katalogu.
-   **Počet podprocesů v rámci připojení (WtThreadCount)**. Tento parametr určuje relativní důležitost počtu podprocesů přidělených připojení. Výchozím nastavením váhy je hodnota 100, což znamená, že při výběru připojení je 100krát důležitější nízký počet podprocesů globálního katalogu než skutečnost, že zatížení je vyrovnáváno pomocí kruhového dotazování.
-   **Pomalé připojení (WtSlow)**. Tento parametr určuje relativní důležitost pomalého připojení. Výchozím nastavením váhy je hodnota 1 000, což znamená, že při výběru připojení je 10krát důležitější, aby připojení ke globálnímu katalogu nebylo pomalé, než skutečnost, že počet podprocesů je nízký.
