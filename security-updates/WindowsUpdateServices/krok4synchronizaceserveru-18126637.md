---
TOCTitle: 'Krok 4: Synchronizace serveru'
Title: 'Krok 4: Synchronizace serveru'
ms:assetid: 'a5514e46-a50b-46a6-9e5b-33c87c5b7cef'
ms:contentKeyID: 18126637
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc708523(v=WS.10)'
---

Krok 4: Synchronizace serveru
=============================

Po konfiguraci síťového připojení můžete získat aktualizace. Při výchozím nastavení je služba WSUS konfigurována na stahování kritických aktualizací a aktualizací zabezpečení pro všechny produkty společnosti Microsoft. Chcete-li získat aktualizace, musíte *synchronizovat* server WSUS.

Synchronizace zahrnuje kontaktování serveru Microsoft Update serverem WSUS. Po vytvoření kontaktu určí server WSUS, zda jsou od poslední synchronizace k dispozici nějaké nové aktualizace. Protože se jedná o první synchronizaci serveru WSUS, jsou všechny aktualizace k dispozici a připraveny ke schválení pro instalaci.

| ![](images/Cc708523.note(WS.10).gif)Poznámka                                                                                                                                                                                                                                                                   |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Tento dokument popisuje synchronizaci pomocí výchozího nastavení, ale server WSUS zahrnuje možnosti, které umožňují minimalizovat během synchronizace použití šířky pásma. Další informace naleznete v dokumentu White Paper Deploying Microsoft Server Windows Update Services (Nasazení služby Microsoft Windows Server Update Services). |

**Synchronizace serveru WSUS**
1.  Na panelu nástrojů konzoly služby WSUS klepněte na tlačítko **Možnosti** a potom na odkaz **Možnosti synchronizace**.

2.  Ve skupinovém rámečku **Úkoly** klepněte na odkaz **Synchronizovat nyní**.

Po dokončení synchronizace zobrazte klepnutím na možnost **Aktualizace** na panelu nástrojů konzoly služby WSUS seznam aktualizací.
