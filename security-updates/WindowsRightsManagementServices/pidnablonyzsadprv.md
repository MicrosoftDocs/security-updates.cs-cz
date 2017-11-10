---
TOCTitle: Přidání šablony zásad práv
Title: Přidání šablony zásad práv
ms:assetid: '1a5555cd-6d39-4078-a879-4106864674be'
ms:contentKeyID: 18113202
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc720206(v=WS.10)'
---

Přidání šablony zásad práv
==========================

Provedení tohoto postupu vyžaduje, aby byl uživatel místně přihlášen k webu pro správu v rámci uživatelského účtu, který je členem skupiny Administrators v počítači, k němuž získává přístup. Uvedený postup mohou provést také členové skupiny Domain Admins. Z hlediska zabezpečení je nejvhodnější při provádění tohoto postupu použít příkaz **Spustit jako**.

Chcete-li otevřít webovou stránku **Globální správa**, klepněte na tlačítko **Start**, přejděte na příkaz **Všechny programy**, přejděte na položku **Služba RMS v systému Windows** a klepněte na položku **Správa služby RMS v systému Windows**.

Přidání šablony zásad práv
--------------------------

#### Přidání šablony zásad práv

1.  Otevřete stránku **Globální správa** a klepněte na položku **Spravovat službu RMS na tomto webu** u webu, na který chcete přidat šablonu zásad práv.

2.  V části **Odkazy správy** klepněte na odkaz **Šablony zásad práv**.

3.  V části **Jazyk** klepněte na jazyk, který má šablona používat.

4.  Klepněte na položku **Přidat šablonu zásad práv**.

5.  V části **Identifikace šablony** zadejte název, popis a adresu žádosti o práva požadované šablony.

6.  V oblasti **Uživatelé a skupiny** v části **Přidat uživatele nebo skupiny** zadejte platnou e-mailovou adresu uživatele nebo skupiny, které chcete přidat, a poté klepněte na tlačítko **Přidat**. Opakováním tohoto kroku podle potřeby přidejte další uživatele nebo skupiny.

7.  V části **Aktuální uživatelé nebo skupiny** vyberte e-mailovou adresu uživatele nebo skupiny, kterým chcete přiřadit práva.

8.  Zaškrtněte políčka u všech práv, která chcete udělit vybranému uživateli nebo skupině. Podle potřeby tento krok opakujte a udělte práva ostatním uživatelům a skupinám.

9.  V části **Zásady vypršení platnosti** vyberte jednu ze tří možností pro vypršení platnosti a poté zadejte datum nebo čas vypršení platnosti podle vybrané možnosti. V případě potřeby vyberte možnost **Licence k použití obsahu musí být obnoveny vždy po** a zadejte počet dní mezi dvěma operacemi obnovení.

10. Vyberte jednu nebo více ze čtyř možností v části **Rozšířené zásady**. Pokud vyberete možnost **Vynutit data specifická pro aplikaci**, zadejte název a hodnotu vynucovaných dat a poté klepněte na tlačítko **Přidat**.

11. Pokud chcete implementovat odvolávání, zaškrtněte v části **Zásady odvolání** políčko **Požadovat odvolání** a poté proveďte následující kroky:

    1.  V části **URL nebo UNC** zadejte adresu URL, na kterou bude odeslán soubor se seznamem odvolání. Pokud je třeba podporovat také odpojené nebo externí uživatele, měl by být k této adrese URL umožněn přístup z podnikové sítě i z Internetu.
    2.  Do pole **Interval aktualizace seznamu odvolání** zadejte počet dnů, po které zůstává seznam odvolání v platnosti. Uživatel, jehož kopie seznamu odvolání je starší, než určuje tato hodnota, nemůže využívat obsah, dokud nezíská aktualizovaný seznam odvolání.
    3.  Do pole **Soubor veřejného klíče** zadejte cestu a název souboru nebo klepněte na tlačítko **Procházet** a vyhledejte soubor veřejného klíče seznamu odvolání. Další informace o tomto souboru získáte v tomto tématu v části Vložení podpisu do seznamu odvolání uvedené již dříve.

    > [!CAUTION]
    > Při implementaci odvolání postupujte obezřetně. Seznam odvolání je nutné pravidelně obnovovat v souladu se zadaným intervalem aktualizace. V opačném případě automaticky vyprší jeho platnost a uživatelé nebudou moci využívat obsah vyžadující daný seznam. Nechcete-li uživatelům neúmyslně znemožnit využití obsahu, vyhodnoťte pečlivě při stanovení požadovaného intervalu aktualizace seznamu odvolání všechny okolnosti. Další informace získáte v tomto tématu v části [Správa odvolání](https://technet.microsoft.com/df732a7d-1fb0-4845-87ca-fab4bc5f98a0)uvedené již dříve. 

12. Klepněte na tlačítko **Odeslat**.

Další informace o odvolání získáte v tomto tématu v části [Správa odvolání](https://technet.microsoft.com/df732a7d-1fb0-4845-87ca-fab4bc5f98a0) uvedené již dříve.

Přehled aspektů ovlivňujících výběr možností odvolávání naleznete v tomto tématu v části [Definice zásad odvolání](https://technet.microsoft.com/e2fffe9f-def7-439b-a8aa-43f8a065813d)uvedené již dříve.

Další informace o provádění tohoto postupu naleznete v tomto tématu v části [Vytvoření a změna šablon zásad práv](https://technet.microsoft.com/6014176f-ef71-4d29-b3e3-da129c18563d) uvedené již dříve.
