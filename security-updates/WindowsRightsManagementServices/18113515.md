---
TOCTitle: Sledování pomocí správce Microsoft Operations Manager
Title: Sledování pomocí správce Microsoft Operations Manager
ms:assetid: 'ce372598-7421-4f1f-b8eb-f62da26e85d1'
ms:contentKeyID: 18113515
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747758(v=WS.10)'
---

Sledování pomocí správce Microsoft Operations Manager
=====================================================

Služba RMS zahrnuje sadu Management Pack, kterou lze použít v rámci správce Microsoft® Operations Manager (MOM). Pomocí správce MOM můžete sledovat provoz serverů v rámci vaší organizace. K dispozici jsou následující možnosti:

-   sledování událostí, které služba RMS umístila do protokolu událostí aplikací,
-   zvýraznění událostí, které mohou indikovat možné výpadky služeb nebo konfigurační potíže, aby bylo možné rychle uskutečnit opravné nebo preventivní akce,
-   upozornění na varování a chyby, jako je například konec platnosti certifikátu serveru pro poskytování licencí nebo chybu webové služby.

Sada RMS Management Pack (RMS\_MOMPack.akm) je nainstalována společně se službou RMS do složky %programfiles%\\Windows Rights Management Services\\Tools.

Tato sada obsahuje následující sady pravidel, které mohou správcům služby RMS usnadnit správu nasazení serveru RMS.

**Pravidla sady RMS Management Pack pro správce MOM**

1.  Opatření PMC – Celkový počet selhání aktivačního serveru proxy
2.  Opatření PMC – Celková doba aktivačního serveru proxy
3.  Opatření PMC – Celková doba zpracování aktivace
4.  Opatření PMC – Celkový počet požadavků na aktivaci
5.  Opatření PMC – Celkový počet požadavků směrovaných na aktivační server proxy
6.  Opatření PMC – Úspěšné přístupy k mezipaměti služby Active Directory (mezipaměti databáze)
7.  Opatření PMC – Neúspěšné přístupy k mezipaměti služby Active Directory (mezipaměti databáze)
8.  Opatření PMC – Průměrná doba zpracování licence
9.  Událost – Poškození informací o konfiguraci
10. Opatření PMC – Zablokovaná připojení GC
11. Opatření PMC – Selhání zápisu
12. Událost – Obecná chyba
13. Událost – Selhání inicializace
14. Událost – Konec platnosti certifikátu serveru pro poskytování licencí
15. Událost – Neúspěšný požadavek na certifikát serveru pro poskytování licencí
16. Událost – Selhání služby protokolování
17. Opatření PMC – Maximální počet dostupných připojení GC
18. Událost – Chybějící modul plug-in umožňující generování bodů pro získání licence
19. Opatření PMC – Délka fronty služby Řízení front zpráv na všech serverech správy přístupových práv
20. Událost – Připojení GC nejsou k dispozici
21. Událost – Selhání inicializace modulu plug-in
22. Událost – Změněné heslo ochrany PrivateKey
23. Událost – Vypnutí serveru správy přístupových práv
24. Událost – Neúspěšné vypnutí serveru správy přístupových práv
25. Událost – Neúspěšné zapnutí serveru
26. Opatření PMC – Selhání dílčího zápisu
27. Událost – Spuštění možnosti přepisu vyžadující oprávnění skupiny SuperUser
28. Prahové hodnoty PMC – Příliš mnoho chyb typu GetLicensorCert
29. Událost – Blížící se konec platnosti certifikátu serveru pro poskytování licencí – 1 měsíc
30. Událost – Blížící se konec platnosti certifikátu serveru pro poskytování licencí – 1 týden

Další informace o způsobu nasazení sad Management Pack pro správce MOM v rámci organizace naleznete na [webu společnosti Microsoft](http://www.microsoft.com/) (http://www.microsoft.com/).
