---
TOCTitle: Nastavení skupiny superuživatelů
Title: Nastavení skupiny superuživatelů
ms:assetid: 'f2ef847e-2824-471f-9079-5c343094aba8'
ms:contentKeyID: 18113548
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747798(v=WS.10)'
---

Nastavení skupiny superuživatelů
================================

Provedení tohoto postupu vyžaduje, aby byl uživatel místně přihlášen k webu pro správu v rámci uživatelského účtu, který je členem skupiny Administrators v počítači, k němuž získává přístup. Uvedený postup mohou provést také členové skupiny Domain Admins. Z hlediska zabezpečení je nejvhodnější při provádění tohoto postupu použít příkaz **Spustit jako**.

Chcete-li otevřít webovou stránku **Globální správa**, klepněte na tlačítko **Start**, přejděte na příkaz **Všechny programy**, přejděte na položku **Služba RMS v systému Windows** a klepněte na položku **Správa služby RMS v systému Windows**.

Skupina, kterou chcete označit jako skupinu superuživatelů služby RMS, musí být předem definována ve službě Active Directory a vlastnosti této skupiny musí zahrnovat e-mailovou adresu (zadanou ve tvaru úplného doménového názvu) shodnou s názvem účtu.

Nastavení skupiny superuživatelů
--------------------------------

#### Nastavení skupiny superuživatelů

1.  Otevřete stránku **Globální správa** a klepněte na položku **Spravovat službu RMS na tomto webu** u webu, na kterém chcete nastavit skupinu superuživatelů.

2.  V části **Odkazy správy** klepněte na odkaz **Nastavení zabezpečení**.

3.  Klepnutím na tlačítko **Povolit** v části **Superuživatelé** přidejte skupinu superuživatelů.

4.  Do pole **Název skupiny superuživatelů** zadejte úplný doménový název skupiny (ve tvaru *název\_skupiny*@*název\_domény.com*) existující v této doménové struktuře služby Active Directory, jejímž členům mají být udělena práva vlastníků všech dokumentů chráněných službou RMS, a poté klepněte na tlačítko **Uložit**.

    Chcete-li zakázat udělení práv skupině superuživatelů, klepněte na tlačítko **Zakázat**.

Další informace o provádění tohoto postupu naleznete v tomto tématu v části [Práce se skupinou superuživatelů](https://technet.microsoft.com/0febcb3e-7124-4e51-971a-1013b928d33b) uvedené již dříve.
