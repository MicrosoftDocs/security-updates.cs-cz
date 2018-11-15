---
TOCTitle: Zadání kontaktu pro správu
Title: Zadání kontaktu pro správu
ms:assetid: '31777458-5530-4ae0-ac1f-131b3d98dd35'
ms:contentKeyID: 18113257
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc720237(v=WS.10)'
---

Zadání kontaktu pro správu
==========================

Provedení tohoto postupu vyžaduje, aby byl uživatel místně přihlášen k webu pro správu v rámci uživatelského účtu, který je členem skupiny Administrators v počítači, k němuž získává přístup. Uvedený postup mohou provést také členové skupiny Domain Admins. Z hlediska zabezpečení je nejvhodnější při provádění tohoto postupu použít příkaz **Spustit jako**.

Správce určený v tomto postupu by měl být místním správcem serveru kořenové certifikace, protože přihlášený uživatel musí mít oprávnění k souboru SubEnrollService.asmx na serveru kořenové certifikace, aby bylo možné zajistit server správy licencí. Pokud uživatel, který se pokouší o zajištění serveru správy licencí, nemá oprávnění pro práci s tímto souborem, může o poskytnutí potřebných oprávnění uživatelskému účtu požádat správce určeného tímto postupem. Další informace naleznete v tomto tématu v části [Nastavení oprávnění souboru služby dílčího zápisu](https://technet.microsoft.com/737bb69b-fe26-4057-9569-e632f7bbf295) uvedené již dříve.

Chcete-li otevřít webovou stránku **Globální správa**, klepněte na tlačítko **Start**, přejděte na příkaz **Všechny programy**, přejděte na položku **Služba RMS v systému Windows** a klepněte na položku **Správa služby RMS v systému Windows**.

Zadání kontaktu pro správu
--------------------------

#### Zadání kontaktu pro správu

1.  Otevřete stránku **Globální správa** a klepněte na položku **Spravovat službu RMS na tomto webu** u webu, u kterého chcete zadat kontakt pro správu.

2.  V části **Odkazy správy** klepněte na odkaz **Nastavení certifikace**.

3.  V části **Kontakt pro správu** zadejte e-mailovou adresu správce, kterého je možné kontaktovat v případě potíží s dílčím zápisem při zajišťování serveru správy licencí, ve tvaru *uživatelské\_jméno*@*název\_domény.com*.

4.  V dolní části stránky klepněte na tlačítko **Odeslat**.
