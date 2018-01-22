---
TOCTitle: Přidání důvěryhodné domény publikování
Title: Přidání důvěryhodné domény publikování
ms:assetid: '731416d8-ddf4-4d4a-9f1a-bbd1ea48fe3c'
ms:contentKeyID: 18113448
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747624(v=WS.10)'
---

Přidání důvěryhodné domény publikování
======================================

Provedení tohoto postupu vyžaduje, aby byl uživatel místně přihlášen k webu pro správu v rámci uživatelského účtu, který je členem skupiny Administrators v počítači, k němuž získává přístup. Uvedený postup mohou provést také členové skupiny Domain Admins. Z hlediska zabezpečení je nejvhodnější při provádění tohoto postupu použít příkaz **Spustit jako**.

Chcete-li otevřít webovou stránku **Globální správa**, klepněte na tlačítko **Start**, přejděte na příkaz **Všechny programy**, přejděte na položku **Služba RMS v systému Windows** a klepněte na položku **Správa služby RMS v systému Windows**.

Jestliže k ochraně soukromého klíče služby RMS používáte hardwarový modul zabezpečení a importujete certifikát serveru pro poskytování licencí z instalace služby RMS používající softwarovou ochranu klíče, je třeba před importem certifikátu určit heslo soukromého klíče na stránce **Nastavení zabezpečení** každého serveru RMS v clusteru.

Přidání důvěryhodných domén publikování
---------------------------------------

#### Přidání důvěryhodné domény publikování

1.  Otevřete stránku **Globální správa** a klepněte na položku **Spravovat službu RMS na tomto webu** u webu, na který chcete přidat důvěryhodnou doménu publikování.

2.  V části **Odkazy správy** klepněte na odkaz **Zásady důvěryhodnosti**.

3.  V části **Důvěryhodné domény publikování** klepněte na tlačítko **Procházet**. Vyhledejte certifikát domény publikování, kterou chcete přidat, a poklepejte na něj. Do pole **Heslo k dešifrování importovaného souboru** zadejte heslo potřebné k dešifrování tohoto souboru a poté klepněte na tlačítko **Importovat**.

    Soubor zašifrovaný pomocí hesla obsahuje certifikát pro poskytování licencí, soukromý klíč (pokud se jedná o softwarově uložený klíč) a šablony zásad práv.

4.  Název domény se objeví v seznamu **Důvěryhodné domény publikování**.

Další informace o provádění tohoto postupu naleznete v tomto tématu v části [Přidání a odebrání důvěryhodných domén publikování](https://technet.microsoft.com/d87b502d-5497-4ccd-badf-f6807d587cee)uvedené již dříve.
