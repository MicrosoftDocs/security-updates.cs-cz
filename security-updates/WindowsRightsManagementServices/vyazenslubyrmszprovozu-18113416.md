---
TOCTitle: Vyřazení služby RMS z provozu
Title: Vyřazení služby RMS z provozu
ms:assetid: '8b563c25-17cd-4b9b-ae42-695497ab6439'
ms:contentKeyID: 18113416
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747665(v=WS.10)'
---

Vyřazení služby RMS z provozu
=============================

Provedení tohoto postupu vyžaduje, aby byl uživatel místně přihlášen k webu pro správu v rámci uživatelského účtu, který je členem skupiny Administrators v počítači, k němuž získává přístup. Uvedený postup mohou provést také členové skupiny Domain Admins. Z hlediska zabezpečení je nejvhodnější při provádění tohoto postupu použít příkaz **Spustit jako**.

Chcete-li otevřít webovou stránku **Globální správa**, klepněte na tlačítko **Start**, přejděte na příkaz **Všechny programy**, přejděte na položku **Služba RMS v systému Windows** a klepněte na položku **Správa služby RMS v systému Windows**.

| ![](images/Cc747665.Warning(WS.10).gif)Varování                             |
|----------------------------------------------------------------------------------------------------------|
| Po vyřazení serveru z provozu nelze obnovit standardní konfiguraci služby RMS. Tento proces je nevratný. |

| ![](images/Cc747665.Warning(WS.10).gif)Varování                                                                                       |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Po vyřazení služby RMS z provozu je třeba před instalací jiné instance služby RMS tuto službu zcela odebrat pomocí ovládacího panelu Přidat nebo odebrat programy. |

Vyřazení služby RMS z provozu
-----------------------------

#### Vyřazení služby RMS z provozu

1.  Přihlaste se k serveru, na kterém chcete vyřadit službu RMS z provozu.

2.  Otevřete stránku **Globální správa** a poté klepněte na odkaz **Spravovat službu RMS na tomto webu**.

3.  Na stránce **Domovská stránka pro správu** klepněte na odkaz **Nastavení zabezpečení**.

4.  V části **Vyřazení služby RMS z provozu** zaškrtněte políčko **Povolit vyřazení instalace RMS z provozu** a poté klepněte na tlačítko **Vyřadit z provozu**.

5.  Po zobrazení výzvy klepněte na tlačítko **OK**. Tím potvrdíte, že chcete trvale vyřadit instalaci služby RMS z provozu.
