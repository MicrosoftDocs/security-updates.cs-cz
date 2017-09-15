---
TOCTitle: Vyloučení aplikací
Title: Vyloučení aplikací
ms:assetid: '422f2ddd-bcf4-45f1-905a-b8bad30fd7dd'
ms:contentKeyID: 18113286
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc720262(v=WS.10)'
---

Vyloučení aplikací
==================

Provedení tohoto postupu vyžaduje, aby byl uživatel místně přihlášen k webu pro správu v rámci uživatelského účtu, který je členem skupiny Administrators v počítači, k němuž získává přístup. Uvedený postup mohou provést také členové skupiny Domain Admins. Z hlediska zabezpečení je nejvhodnější při provádění tohoto postupu použít příkaz **Spustit jako**.

Chcete-li otevřít webovou stránku **Globální správa**, klepněte na tlačítko **Start**, přejděte na příkaz **Všechny programy**, přejděte na položku **Služba RMS v systému Windows** a klepněte na položku **Správa služby RMS v systému Windows**.

Zásady vyloučení jsou vynuceny klientem v době, kdy je licence k použití svázána s chráněným obsahem.

Vyloučení aplikací nebo ukončení vyloučení aplikací
---------------------------------------------------

#### Vyloučení aplikací

1.  Otevřete stránku **Globální správa** a klepněte na položku **Spravovat službu RMS na tomto webu** u webu, pro který chcete určit verze aplikací, které lze použít s obsahem chráněným správou přístupových práv.

2.  V části **Odkazysprávy** klepněte na odkaz **Zásady vyloučení**.

3.  Klepnutím na možnost **Povolit** v části **Vyloučení aplikací** můžete vyloučit aplikaci nebo součást s podporou správy přístupových práv.

    Chcete-li vyloučení aplikací zakázat, klepněte na možnost **Zakázat**.

4.  Zadejte název souboru aplikace nebo součásti, kterou chcete vyloučit, minimální a maximální verzi pro vyloučení (ve tvaru *x*.*x*.*x*.*x*) a klepněte na tlačítko **Vyloučit tuto aplikaci**.

    Chcete-li ze seznamu vyloučení odstranit určitou aplikaci (nebo součást), vyberte název souboru a poté klepněte na možnost **Odstranit vybrané aplikace ze seznamu vyloučení**.

    | ![](images/Cc720262.note(WS.10).gif)Poznámka                                                                                                                                                                                                                                                      |
    |--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Server RMS vyžaduje zadání verze aplikace ve formátu čtyřmístného čísla odděleného tečkami (\#.\#.\#.\# ). U některých aplikací je však číslo verze určeno dvoumístnými nebo třímístnými čísly oddělenými tečkou. V takovém případě je vhodné přidat hodnotu .0, aby číslo verze odpovídalo formátu vyžadovanému serverem RMS. |

#### Ukončení vyloučení aplikací

1.  Otevřete stránku **Globální správa** a klepněte na položku **Spravovat službu RMS na tomto webu** u webu, pro který chcete určit verze aplikací, které lze použít s obsahem chráněným správou přístupových práv.

2.  V části **Odkazysprávy** klepněte na odkaz **Zásady vyloučení**.

3.  V části **Vyloučení aplikací** klepněte na položku **Zakázat**.

Další informace o tomto postupu naleznete v tomto tématu v části [Vyloučení aplikací](https://technet.microsoft.com/b68ae4b2-b9ba-44ae-90cb-c88df600ec86) uvedené již dříve.
