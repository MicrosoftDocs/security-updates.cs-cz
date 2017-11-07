---
TOCTitle: Úprava šablon zásad práv
Title: Úprava šablon zásad práv
ms:assetid: '9580b934-bd6f-4097-9d3c-4fc14a3147fa'
ms:contentKeyID: 18113426
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747684(v=WS.10)'
---

Úprava šablon zásad práv
========================

Provedení tohoto postupu vyžaduje, aby byl uživatel místně přihlášen k webu pro správu v rámci uživatelského účtu, který je členem skupiny Administrators v počítači, k němuž získává přístup. Uvedený postup mohou provést také členové skupiny Domain Admins. Z hlediska zabezpečení je nejvhodnější při provádění tohoto postupu použít příkaz **Spustit jako**.

Chcete-li otevřít webovou stránku **Globální správa**, klepněte na tlačítko **Start**, přejděte na příkaz **Všechny programy**, přejděte na položku **Služba RMS v systému Windows** a klepněte na položku **Správa služby RMS v systému Windows**.

Úprava šablon zásad práv
------------------------

#### Úprava šablon zásad práv

1.  Otevřete stránku **Globální správa** a klepněte na položku **Spravovat službu RMS na tomto webu** u webu, na kterém chcete upravit šablonu zásad práv.

2.  V části **Odkazy správy** klepněte na odkaz **Šablony zásad práv**.

3.  V seznamu **Název šablony** klepněte na název šablony, kterou chcete upravit.

4.  V části **Identifikace šablony** podle potřeby upravte informace v polích **Název šablony**, **Popis šablony** a **Adresa URL žádosti o práva**.

5.  V části **Uživatelé a skupiny** proveďte nejméně jednu z následujících akcí:

    -   Chcete-li přidat uživatele nebo skupinu, zadejte v části **Přidat uživatele nebo skupiny** platnou e-mailovou adresu konkrétního uživatele nebo skupiny, které chcete přidat, klepněte na tlačítko **Přidat** a poté vyberte jméno v seznamu **Aktuální uživatelé nebo skupiny**. V části **Práva** vyberte všechna práva, která chcete udělit vybranému uživateli nebo skupině.
    -   Chcete-li upravit práva existujícího uživatele nebo skupiny, vyberte příslušné jméno či název v seznamu **Aktuální uživatelé nebo skupiny** a poté podle potřeby zaškrtněte nebo zrušte zaškrtnutí políček u požadovaných práv.
    -   Chcete-li odebrat uživatele nebo skupinu, vyberte příslušnou položku v seznamu **Aktuální uživatelé nebo skupiny** a poté klepněte na tlačítko **Odebrat**.

6.  Chcete-li změnit časový limit vypršení platnosti licencí obsahu, po jehož uplynutí je nutné licence obnovit, upravte příslušné informace v části **Zásady vypršení platnosti**.

7.  V části **Rozšířené zásady** můžete úpravou informací podle potřeby změnit způsob implementace licencí obsahu, včetně doby platnosti autorských práv, možnosti podpory důvěryhodných prohlížečů, doby platnosti licence v rámci příslušného obsahu a vynucení jakýchkoli dat specifických pro aplikace.

8.  V části **Zásady odvolání** určete, zda má být pro obsah vytvořený pomocí této šablony vyžadován seznam odvolání. Pokud vyberete možnost **Požadovat odvolání**, proveďte podle potřeby následující nastavení:

    -   Do pole **URL** zadejte adresu URL, na kterou bude odeslán soubor se seznamem odvolání. Pokud je třeba podporovat také odpojené nebo externí uživatele, měl by být k této adrese URL umožněn přístup z podnikové sítě i z Internetu. Další informace získáte v tomto tématu v části [Implementace odvolání](https://technet.microsoft.com/4735f060-7197-4ae2-830a-f91bcc4de30a)uvedené již dříve.
    -   Do pole **Interval aktualizace seznamu odvolání** zadejte počet dnů, po které zůstává seznam odvolání v platnosti. Uživatel, jehož kopie seznamu odvolání je starší, než určuje tato hodnota, nemůže využívat obsah, dokud nezíská aktualizovaný seznam odvolání.
    -   Do pole **Soubor veřejného klíče** zadejte cestu a název souboru veřejného klíče seznamu odvolání. Další informace o tomto souboru získáte v tomto tématu v části Vložení podpisu do seznamu odvolání uvedené již dříve.

    | ![](images/Cc747684.Caution(WS.10).gif)Upozornění                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
    |-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Při implementaci odvolání postupujte obezřetně. Seznam odvolání je nutné pravidelně obnovovat v souladu se zadaným intervalem aktualizace. V opačném případě automaticky vyprší jeho platnost a uživatelé nebudou moci využívat obsah vyžadující daný seznam. Nechcete-li uživatelům neúmyslně znemožnit využití obsahu, vyhodnoťte pečlivě při stanovení požadovaného intervalu aktualizace seznamu odvolání všechny okolnosti. Další informace získáte v tomto tématu v části [Správa odvolání](https://technet.microsoft.com/df732a7d-1fb0-4845-87ca-fab4bc5f98a0)uvedené již dříve. |

9.  Klepněte na tlačítko **Odeslat**.

Další informace o provádění tohoto postupu naleznete v tomto tématu v části [Vytvoření a změna šablon zásad práv](https://technet.microsoft.com/6014176f-ef71-4d29-b3e3-da129c18563d) uvedené již dříve.
