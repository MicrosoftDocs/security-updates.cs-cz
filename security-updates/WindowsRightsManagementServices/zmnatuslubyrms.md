---
TOCTitle: Změna účtu služby RMS
Title: Změna účtu služby RMS
ms:assetid: 'a3e522b0-e23d-49f2-b00a-cff90ac2c36a'
ms:contentKeyID: 18113456
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747713(v=WS.10)'
---

Změna účtu služby RMS
=====================

Provedení tohoto postupu vyžaduje, aby byl uživatel místně přihlášen k webu pro správu v rámci uživatelského účtu, který je členem skupiny Administrators v počítači, k němuž získává přístup. Uvedený postup mohou provést také členové skupiny Domain Admins. Z hlediska zabezpečení je nejvhodnější při provádění tohoto postupu použít příkaz **Spustit jako**.

Chcete-li otevřít webovou stránku **Globální správa**, klepněte na tlačítko **Start**, přejděte na příkaz **Všechny programy**, přejděte na položku **Služba RMS v systému Windows** a klepněte na položku **Správa služby RMS v systému Windows**.

Jako účet služby RMS nelze použít doménový účet, který byl použit k instalaci služby RMS s aktualizací Service Pack 1.

Změna účtu služby RMS
---------------------

#### Změna účtu služby RMS

1.  Otevřete stránku **Globální správa** a klepněte na položku **Změnit účet služby RMS** u webu, na kterém je zajištěna služba RMS.

2.  Zadejte název účtu, pod kterým bude služba RMS obvykle pracovat za běžného provozu. U doménových účtů použijte formát *název\_domény*\\*uživatelské\_jméno*.

3.  Zadejte heslo a poté klepněte na tlačítko **Odeslat**.
