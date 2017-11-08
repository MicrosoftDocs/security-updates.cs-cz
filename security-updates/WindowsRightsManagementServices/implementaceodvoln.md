---
TOCTitle: Implementace odvolání
Title: Implementace odvolání
ms:assetid: '4735f060-7197-4ae2-830a-f91bcc4de30a'
ms:contentKeyID: 18113297
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747554(v=WS.10)'
---

Implementace odvolání
=====================

Certifikáty a licence mohou být odvolány libovolným zaregistrovaným objektem zabezpečení, který patří do řetězce důvěryhodných objektů pro daný certifikát nebo licenci. Certifikát nebo licence vydané serverem kořenové certifikace mohou být odvolány tímto serverem. Kromě toho mohou být certifikáty odvolány třetí stranou vybranou správcem služby RMS.

Chcete-li odvolat certifikát nebo licenci udělené serverem služby RMS, můžete vytvořit a distribuovat seznam odvolání a pak vyžadovat daný seznam v šabloně zásad práv, jak je popsáno v následujícím postupu:

1.  Vytvořte seznam odvolání určující zaregistrované objekty zabezpečení, které mají být odvolány. Jedná se textový soubor ve formátu XML, který vyhovuje syntaxi jazyka XrML. Další informace získáte v tomto tématu později v části [Vytvoření seznamů odvolání](https://technet.microsoft.com/1ef75199-3344-4225-84de-a863a777696a).
2.  Vygenerujte pár klíčů pro seznam odvolání. Pomocí nástroje pro podepisování seznamů odvolaných certifikátů dodaného pro tento účel podepište soubor soukromým klíčem. Popis postupu naleznete v tomto tématu později v části Vložení podpisu do seznamu odvolání. Tento postup automatizujte, aby jej bylo možné provádět pravidelně, v optimálním případě denně.
3.  Uložte soubor se seznamem odvolání do umístění přístupného pro všechny uživatele, kteří seznam vyžadují. Je doporučeno uložit soubor do umístění dostupného jak ze sítě, tak z Internetu, například na web. Tím zajistíte, že k souboru budou mít přístup uživatelé z podnikové sítě i mimo ni.
4.  Vytvořte šablonu zásad práv obsahující požadavek na daný seznam odvolání. Další informace naleznete v tomto tématu později v části [Vytvoření a změna šablon zásad práv](https://technet.microsoft.com/6014176f-ef71-4d29-b3e3-da129c18563d).

Můžete také odvolat certifikát serveru pro poskytování licencí pro server kořenové certifikace. Vzhledem k tomu, že tento certifikát byl vydán službou Microsoft Enrollment Services, může jej společnost Microsoft pro server kořenové certifikace odvolat. K tomuto účelu přidá společnost Microsoft certifikát serveru pro poskytování licencí do svého seznamu odvolání a tento seznam zveřejní.

Kromě toho může být certifikát serveru pro poskytování licencí pro server kořenové certifikace odvolán třetí stranou, pokud správce služby RMS tuto možnost nastaví při zajišťování služby. Jestliže tuto možnost nastavíte, měl by být seznam odvolání, který obsahuje tento certifikát serveru pro poskytování licencí a je podepsán soukromým klíčem třetí strany, k dispozici klientům. Další informace naleznete v tomto tématu později v části [Odvolání certifikátů serveru pro poskytování licencí](https://technet.microsoft.com/8020861d-d196-4431-8282-044675ef5616).

| ![](images/Cc747554.Caution(WS.10).gif)Upozornění                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Při implementaci odvolání postupujte opatrně. Na základě určeného intervalu aktualizace je třeba pravidelně obnovovat seznam odvolání nebo jeho platnost automaticky vyprší. V takovém případě by uživatelé nemohli pracovat s obsahem, který daný seznam vyžaduje. Chcete-li zajistit, že uživatelům nebude omylem znemožněna práce s obsahem, vyhodnoťte pečlivě, jaký interval bude pro aktualizaci seznamu odvolání nastaven. Dále zajistěte, aby byl seznam odvolání přístupný ze sítě i z míst mimo ni. Další informace získáte v tomto tématu v části [Definice zásad odvolání](https://technet.microsoft.com/e2fffe9f-def7-439b-a8aa-43f8a065813d)uvedené již dříve. |
