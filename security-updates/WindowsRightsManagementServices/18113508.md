---
TOCTitle: Sledování certifikátů účtů práv
Title: Sledování certifikátů účtů práv
ms:assetid: 'f9efac9f-c725-4bce-a89f-7691b0d8ffc0'
ms:contentKeyID: 18113508
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747752(v=WS.10)'
---

Sledování certifikátů účtů práv
===============================

Provedení tohoto postupu vyžaduje, aby byl uživatel místně přihlášen k webu pro správu v rámci uživatelského účtu, který je členem skupiny Administrators v počítači, k němuž získává přístup. Uvedený postup mohou provést také členové skupiny Domain Admins. Z hlediska zabezpečení je nejvhodnější při provádění tohoto postupu použít příkaz **Spustit jako**.

Chcete-li otevřít webovou stránku **Globální správa**, klepněte na tlačítko **Start**, přejděte na příkaz **Všechny programy**, přejděte na položku **Služba RMS v systému Windows** a klepněte na položku **Správa služby RMS v systému Windows**.

Tato funkce je dostupná pouze u clusteru kořenové certifikace, nikoli u serverů a clusterů správy licencí.

Uvedený postup lze použít pouze k odhadu počtu licencí k použití a jeho použití má smysl pouze u účtovatelných licencí. Číslo, které se zobrazuje na stránce Sestava certifikace účtů RM, je pouze přibližné. Pokud jste neprovedli aktualizaci konfigurační databáze a neodstranili uživatele, kteří již nejsou aktivní, nebude toto číslo odpovídat skutečnosti. Také v případě, že některým uživatelům bylo vydáno více licencí ve více doménových strukturách, nejsou tyto další licence zahrnuty do zobrazené hodnoty.

Sledování certifikátů účtů práv
-------------------------------

#### Sledování certifikátů účtů práv

1.  Otevřete stránku **Globální správa** a klepněte na položku **Spravovat službu RMS na tomto webu** u webu, na kterém chcete sledovat certifikáty.

2.  V části **Odkazy správy** klepněte na odkaz Sestava certifikace účtů RM.

3.  V části **Celkový počet certifikovaných uživatelů** je uveden počet uživatelů, kteří obdrželi certifikáty účtů práv z tohoto clusteru kořenové certifikace.

Další informace naleznete v tomto tématu v části [Sledování certifikátů účtů práv](https://technet.microsoft.com/5bb0f3cf-fc44-4e60-a93f-c789d6f8a902) uvedené již dříve.
