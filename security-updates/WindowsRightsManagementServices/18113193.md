---
TOCTitle: Přidání extranetové adresy URL clusteru
Title: Přidání extranetové adresy URL clusteru
ms:assetid: '12c83186-ce9e-4100-bbd1-d87a885331c7'
ms:contentKeyID: 18113193
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc720193(v=WS.10)'
---

Přidání extranetové adresy URL clusteru
=======================================

Provedení tohoto postupu vyžaduje, aby byl uživatel místně přihlášen k webu pro správu v rámci uživatelského účtu, který je členem skupiny Administrators v počítači, k němuž získává přístup. Uvedený postup mohou provést také členové skupiny Domain Admins. Z hlediska zabezpečení je nejvhodnější při provádění tohoto postupu použít příkaz **Spustit jako**.

Chcete-li otevřít webovou stránku **Globální správa**, klepněte na tlačítko **Start**, přejděte na příkaz **Všechny programy**, přejděte na položku **Služba RMS v systému Windows** a klepněte na položku **Správa služby RMS v systému Windows**.

Nezapomeňte adresu URL zaregistrovat ve službě DNS a zkontrolujte, zda funguje a zda je dostupná z Internetu i extranetu. Pokud jste u souborů webových služeb povolili zabezpečení SSL, je nutné v adrese URL clusteru použít protokol HTTPS.

Jestliže přidáváte adresu URL pro cluster extranetu na server RMS, který je již v provozu, musí aktuální klienti RMS získat nové certifikáty klienta pro poskytování licencí, aby mohli získat přístup ke clusteru extranetu pro správu licencí.

Přidání extranetové adresy URL clusteru
---------------------------------------

#### Přidání extranetové adresy URL clusteru

1.  Otevřete stránku **Globální správa** a klepněte na položku **Spravovat službu RMS na tomto webu** u webu, pro který chcete přidat adresu URL clusteru extranetu.

2.  V části **Odkazy správy** klepněte na položku **Nastavení extranetové adresy URL clusteru**.

3.  V části **Extranetová adresa URL clusteru** zadejte adresu URL, ze které budou externí uživatelé získávat licence. Dále můžete vybrat protokol HTTP nebo HTTPS.

4.  Klepněte na tlačítko **Odeslat**.
