---
TOCTitle: Odvolání certifikátů serveru pro poskytování licencí
Title: Odvolání certifikátů serveru pro poskytování licencí
ms:assetid: '8020861d-d196-4431-8282-044675ef5616'
ms:contentKeyID: 18113357
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747578(v=WS.10)'
---

Odvolání certifikátů serveru pro poskytování licencí
====================================================

V některých případech může být v organizaci vzhledem k nepředvídatelným okolnostem, které vedou k ohrožení serveru RMS, nutné odvolat certifikát serveru pro poskytování licencí. Soukromý klíč, který není uchováván v hardwarovém modulu zabezpečení, může být ukraden. V organizaci může dojít k ohrožení zabezpečení certifikátu serveru pro poskytování licencí a klíče, například v důsledku útoku uživatelů se zlými úmysly, kteří převezmou řízení serveru nebo certifikát či klíč zkopírují nebo zničí. Odvolání představuje jednu z možností, jak omezit ztráty a znemožnit činnost uživateli se zlými úmysly.

Ve výchozím nastavení mohou být licence či certifikát odvolány zaregistrovaným objektem zabezpečení, který je vydal. Vzhledem k tomu, že licence a certifikáty k vašemu chráněnému obsahu vydávají servery RMS, můžete je v případě potřeby kdykoli odvolat. Dojde-li k ohrožení zabezpečení serveru správy licencí, můžete odvolat jeho certifikát pro poskytování licencí. Pokud odvoláte certifikáty serveru pro poskytování licencí, budou všechny certifikáty a licence vydané daným serverem neplatné. Postup při odvolání licencí a certifikátů naleznete v tomto tématu v části [Implementace odvolání](https://technet.microsoft.com/4735f060-7197-4ae2-830a-f91bcc4de30a)uvedené již dříve.

V případě clusteru kořenové certifikace se však jedná o speciální případ. Certifikát poskytovatele licence clusteru kořenové certifikace je vydán službou Microsoft Enrollment Services a podle výchozího nastavení může odvolání certifikátu poskytovatele licence serveru provést pouze tato služba.

Společnost Microsoft může certifikát serveru pro poskytování licencí pro server kořenové certifikace odvolat pouze v případě, že získáte soudní příkaz a poskytnete soudu veřejný klíč serveru. Jakmile soud uvědomí společnost Microsoft, že byl vydán příkaz k odvolání, zadá společnost Microsoft na základě veřejného klíče certifikát serveru pro poskytování licencí do seznamu odvolání a tento seznam zveřejní. Příkaz k odvolání můžete u soudu vyžádat, je-li u serveru, jehož licenci chcete odvolat, splněna jedna z následujících podmínek:

-   jste vlastníkem serveru a došlo k ohrožení soukromého klíče,
-   vlastníte obsah, který je serverem publikován, a publikování tohoto obsahu představuje porušení vašich autorských práv.

Postupem popsaným v tomto tématu v části [Instalace seznamů odvolání](https://technet.microsoft.com/e331338b-66d4-45e4-8d3f-acccf2302ac4) uvedené již dříve můžete získat a distribuovat seznamy odvolání společnosti Microsoft obsahující odvolaný certifikát serveru pro poskytování licencí pro server kořenové certifikace.

Při zajišťování serveru kořenové certifikace můžete určit veřejný klíč, který má oprávnění k odvolání certifikátu serveru pro poskytování licencí pro cluster kořenové certifikace. Může se jednat o veřejný klíč objektu v rámci organizace nebo objektu třetí strany. Prostřednictvím seznamu odvolání podepsaného odpovídajícím soukromým klíčem pak může být certifikát serveru pro poskytování licencí odvolán.

Chcete-li odvolat certifikát serveru pro poskytování licencí pro server kořenové certifikace, můžete vytvořit seznam odvolání, ve kterém je tento certifikát zahrnut, podepsat uvedený seznam soukromým klíčem dané organizace nebo třetí strany a distribuovat jej všem uživatelům. Další postup naleznete v tomto oddíle v části Instalace seznamů odvolání organizace tématu [Instalace seznamů odvolání](https://technet.microsoft.com/e331338b-66d4-45e4-8d3f-acccf2302ac4) uvedené již dříve.

Certifikát serveru pro poskytování licencí můžete v seznamu odvolání odvolat prostřednictvím následujících parametrů:

-   **Identifikátor GUID**. Certifikát serveru pro poskytování licencí lze odvolat pomocí jeho identifikátoru GUID. Informace týkající se použití tohoto parametru v seznamu odvolání naleznete v tomto oddíle v části Odvolání certifikátů a licencí na základě identifikátoru GUID tématu [Vytvoření seznamů odvolání](https://technet.microsoft.com/1ef75199-3344-4225-84de-a863a777696a) uvedené již dříve.
-   **Hodnota hash**. Certifikát serveru pro poskytování licencí může být odvolán na základě hodnoty hash SHA-1 znaků Unicode obsažených v hlavní části certifikátu. Informace týkající se použití tohoto parametru v seznamu odvolání naleznete v tomto oddíle v části Odvolání certifikátů a licencí na základě hodnoty hash tématu [Vytvoření seznamů odvolání](https://technet.microsoft.com/1ef75199-3344-4225-84de-a863a777696a) uvedené již dříve.

Chcete-li získat certifikát serveru pro poskytování licencí instalace služby RMS, je třeba zadat dotaz v konfigurační databázi služby RMS. Následujícím postupem získáte tyto informace z konfigurační databáze SQL a uložíte je do souboru, který lze snadno zobrazit v prohlížeči:

1.  Spusťte nástroj SQL Query Analyzer a připojte se ke konfigurační databázi serveru kořenové certifikace.
2.  V nabídce **Query** (Dotaz) vyberte příkaz **Results in Text** (Výsledky v textu).
3.  V nabídce **Tools** (Nástroje) vyberte příkaz **Options** (Možnosti). Zobrazí se dialogové okno **Options** (Možnosti). Klepněte na kartu **Results** (Výsledky) a nastavte možnost **Maximum characters per column** (Maximální počet znaků sloupce) na hodnotu **8 192**.
        ```
1.  Zkopírujte výsledky z okna **Results** (Výsledky) a vložte je do textového editoru, například do programu Poznámkový blok. Výsledky uložte do souboru s příponou XML.

Další informace týkající se práce s těmito informacemi v seznamech odvolání naleznete v tomto tématu v části [Vytvoření seznamů odvolání](https://technet.microsoft.com/1ef75199-3344-4225-84de-a863a777696a) uvedené již dříve.

Jakmile jsou informace certifikátu serveru pro poskytování licencí uloženy jako soubor XML, můžete pomocí následujícího postupu provést extrakci veřejného klíče:

1.  Otevřete soubor XML certifikátu serveru pro poskytování licencí v editoru XML nebo v textovém editoru.
2.  V části &lt;ISSUEDPRINCIPALS&gt; zkopírujte prvek &lt;PUBLICKEY&gt;.
3.  Uložte tyto informace do souboru, který můžete předat soudu nebo umístit na podnikový seznam odvolání.

Je-li certifikát serveru pro poskytování licencí pro cluster kořenové certifikace odvolán, budou všechny certifikáty a licence vydané instalací služby RMS neplatné pro obsah, který vyžaduje seznam odvolání, a obsah nebude přístupný. Tento proces není ovlivněn typem licence, kterou má uživatel k dispozici. Chcete-li uchovat obsah publikovaný serverem, jehož licence je odvolávána, je nutné před zahájením implementace seznamu odvolání provést jednu z následujících akcí:

-   uložit obsah bez ochrany správou přístupových práv,
-   publikovat obsah znovu, tentokrát bez požadavku seznamu odvolání.

V obou případech (tedy v případě odvolání provedeného společností Microsoft nebo třetí stranou) má seznam odvolání vliv na všechny požadavky na vytvoření vazby, protože byl podepsán soukromým klíčem zaregistrovaného objektu zabezpečení v posloupnosti důvěryhodných objektů licence k použití. Všechny požadavky na vytvoření vazby týkající se licencí vydaných instalací služby RMS prostřednictvím odvolaného certifikátu serveru pro poskytování licencí tedy budou neúspěšné.

| ![](images/Cc747578.note(WS.10).gif)Poznámka                                            |
|----------------------------------------------------------------------------------------------------------------------|
| Společnost Microsoft odvolá certifikát serveru pro poskytování licencí pouze v případě, že je k tomu vyzvána soudem. |
