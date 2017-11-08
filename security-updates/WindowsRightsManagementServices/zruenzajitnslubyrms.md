---
TOCTitle: Zrušení zajištění služby RMS
Title: Zrušení zajištění služby RMS
ms:assetid: '9fa63daa-5fb9-4afd-8371-b38248619857'
ms:contentKeyID: 18113454
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747706(v=WS.10)'
---

Zrušení zajištění služby RMS
============================

Provedení tohoto postupu vyžaduje, aby byl uživatel místně přihlášen k webu pro správu v rámci uživatelského účtu, který je členem skupiny Administrators v počítači, k němuž získává přístup. Uvedený postup mohou provést také členové skupiny Domain Admins. Z hlediska zabezpečení je nejvhodnější při provádění tohoto postupu použít příkaz **Spustit jako**.

Chcete-li otevřít webovou stránku **Globální správa**, klepněte na tlačítko **Start**, přejděte na příkaz **Všechny programy**, přejděte na položku **Služba RMS v systému Windows** a klepněte na položku **Správa služby RMS v systému Windows**.

Server, jehož zajištění zrušíte, je odebrán z tabulky ClusterServer v konfigurační databázi. Pokud zrušíte zajištění posledního serveru v clusteru, dojde k odstranění databáze adresářových služeb ze serveru SQL Server. Zrušíte-li zajištění posledního serveru kořenové certifikace v clusteru, je nutné ručně zrušit registraci spojovacího bodu certifikační služby (SCP). Zrušení zajištění ani odinstalace nezpůsobí odebrání spojovacího bodu služby ze služby Active Directory.

Pokud se rozhodnete odinstalovat server kořenové certifikace dříve, než jej zajistíte, zobrazí se varování, že zajištění webu nebylo dosud zrušeno a že spojovací bod služby nebude odebrán ze služby Active Directory. Budete-li však pokračovat klepnutím na tlačítko **Ano**, dojde ke zrušení zajištění webu. Odinstalace nezpůsobí odebrání spojovacího bodu služby ze služby Active Directory.

Zrušení zajištění služby RMS
----------------------------

#### Zrušení zajištění služby RMS

1.  Přihlaste se k serveru, na kterém chcete zrušit zajištění služby RMS.

2.  Otevřete stránku **Globální správa.**

3.  Klepněte na položku **Odebrat službu RMS z tohoto webu** u webu, na kterém je zajištěna služba RMS, a pak klepněte na tlačítko **OK**.

4.  Chcete-li zrušit registraci spojení certifikační služby v rámci služby Active Directory, klepněte na webové stránce spojovacího bodu služby RMS na odkaz **Zrušit registraci adresy URL**.
