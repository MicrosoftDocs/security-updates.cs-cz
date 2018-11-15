---
TOCTitle: Povolení certifikace mobilních zařízení
Title: Povolení certifikace mobilních zařízení
ms:assetid: '93ec088e-9056-4c3c-bd97-1173fb194578'
ms:contentKeyID: 18113373
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747603(v=WS.10)'
---

Povolení certifikace mobilních zařízení
=======================================

Provedení tohoto postupu vyžaduje, aby byl uživatel místně přihlášen k webu pro správu v rámci uživatelského účtu, který je členem skupiny Administrators v počítači, k němuž získává přístup. Uvedený postup mohou provést také členové skupiny Domain Admins. Z hlediska zabezpečení je nejvhodnější při provádění tohoto postupu použít příkaz **Spustit jako**.

Tento postup lze použít pouze na clusteru kořenové certifikace.

Při provádění uvedeného postupu se předpokládá, že byla vytvořena skupina uživatelů, která obsahuje účty uživatelů mobilních zařízení využívajících obsah chráněný správou přístupových práv.

Povolení certifikace mobilních zařízení
---------------------------------------

#### Povolení certifikace mobilních zařízení

1.  Na serveru kořenové certifikace otevřete prohlížeč souborového systému a přejděte na &lt;systémovou jednotku&gt;: do složky \\Inetpub\\wwwroot\\\_wmcs\\Certification.

2.  Chcete-li u mobilních zařízeních povolit příjem certifikátů účtů práv, klepněte pravým tlačítkem myši na soubor MobileDeviceCertification.asmx a klepněte na příkaz **Vlastnosti**.

3.  Na kartě **Zabezpečení** klepněte na možnost **Přidat** a přidejte skupinu vytvořenou pro tuto kategorii uživatelů a skupinu **RMS Service Group**.

4.  V seznamu **Oprávnění** pro dané skupiny zaškrtněte políčko **Povolit** pro oprávnění ke **čtení** a **čtení & spuštění** a klepněte na tlačítko **OK**.
