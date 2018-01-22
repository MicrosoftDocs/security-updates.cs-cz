---
TOCTitle: Odinstalace služby RMS
Title: Odinstalace služby RMS
ms:assetid: '885e3b4f-ea32-466f-9f7f-d8440b0f7c28'
ms:contentKeyID: 18113353
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747587(v=WS.10)'
---

Odinstalace služby RMS
======================

Provedení tohoto postupu vyžaduje, aby byl uživatel místně přihlášen k webu pro správu v rámci uživatelského účtu, který je členem skupiny Administrators v počítači, k němuž získává přístup. Uvedený postup mohou provést také členové skupiny Domain Admins. Z hlediska zabezpečení je nejvhodnější při provádění tohoto postupu použít příkaz **Spustit jako**.

Chcete-li otevřít webovou stránku **Globální správa**, klepněte na tlačítko **Start**, přejděte na příkaz **Všechny programy**, přejděte na položku **Služba RMS v systému Windows** a klepněte na položku **Správa služby RMS v systému Windows**.

Odinstalace služby RMS
----------------------

#### Odinstalace služby RMS

1.  Přihlaste se k serveru, na kterém chcete odinstalovat službu RMS.

    > [!IMPORTANT]
    > Pokud službu RMS odebíráte ze serveru v clusteru kořenové certifikace, je nejprve nutné zrušit jeho zajištění přechodem na stránku **Globální správa** a klepnutím na možnost **Odebrat službu RMS z tohoto webu**. Před odinstalací služby RMS ze serveru správy licencí není třeba zrušit zajištění tohoto serveru. 

2.  V **Ovládacích panelech** otevřete panel **Přidat nebo odebrat programy**.

3.  V dialogovém okně **Přidat nebo odebrat programy** klepněte na položku **Služba správy přístupových práv v systému Windows** a potom klepnutím na tlačítko **Odebrat** odeberte službu RMS s aktualizací SP1.
