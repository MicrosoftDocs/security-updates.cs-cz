---
TOCTitle: Instalace služby RMS s aktualizací Service Pack 1
Title: Instalace služby RMS s aktualizací Service Pack 1
ms:assetid: 'dab20175-a690-43f8-b943-768d289daa0d'
ms:contentKeyID: 18113470
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747689(v=WS.10)'
---

Instalace služby RMS s aktualizací Service Pack 1
=================================================

Provedení tohoto postupu vyžaduje, aby byl uživatel místně přihlášen k webu pro správu v rámci uživatelského účtu, který je členem skupiny Administrators v počítači, k němuž získává přístup. Uvedený postup mohou provést také členové skupiny Domain Admins. Z hlediska zabezpečení je nejvhodnější při provádění tohoto postupu použít příkaz **Spustit jako**.

Počítač, na který instalujete službu RMS, musí být členským serverem domény nebo řadičem domény. Službu RMS nelze instalovat na samostatný server v rámci pracovní skupiny.

| ![](images/Cc747689.Important(WS.10).gif)Důležité informace                                                                                                                                                                                                                                                                                                                                                                                                                       |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Nezajišťujte službu RMS na jiných serverech, dokud nedokončíte instalaci i zajištění prvního serveru kořenové certifikace. Pokyny naleznete v tomto tématu později v částech [Zajištění prvního serveru kořenové certifikace](https://technet.microsoft.com/debc42f3-74ff-4c99-b7a4-4921fccdabc2), [Zajištění serveru správy licencí](https://technet.microsoft.com/4d67b898-0ba9-4eef-ab7d-ee0ca55a688e) a [Přidání serveru do clusteru](https://technet.microsoft.com/db635238-5528-4bec-9cc6-8244e2b3d733). |

| ![](images/Cc747689.Important(WS.10).gif)Důležité informace                                                                                                                                                                                                                    |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Službu RMS s aktualizací SP1 lze nainstalovat na server, na kterém je aktuálně spuštěna předchozí verze služby RMS. Pokud jste však službu RMS vyřadili z provozu, je třeba před instalací služby RMS s aktualizací SP1 původní službu zcela odebrat pomocí ovládacího panelu Přidat nebo odebrat programy. |

Instalace služby RMS s aktualizací Service Pack 1
-------------------------------------------------

#### Instalace služby RMS s aktualizací Service Pack 1

1.  Pomocí doménového účtu, který je členem místní skupiny Administrators, se přihlaste k serveru určenému pro instalaci služby RMS s aktualizací SP1.

2.  Po zobrazení **úvodního** dialogového okna si prohlédněte seznam softwaru, který bude instalován, a poté klepněte na tlačítko **Další**.

3.  V dialogovém okně **Licenční smlouva** se seznamte se zněním licenční smlouvy, vyberte možnost **Souhlasím** a pak klepněte na tlačítko **Další**.

4.  V okně **Složka** přijměte výchozí složku nebo zadejte novou složku a klepněte na tlačítko **Další**.

5.  Spusťte instalaci klepnutím na tlačítko **Instalovat** v dialogovém okně **Potvrzení instalace**.

6.  Po zobrazení dialogového okna **Instalace je dokončena** klepněte na tlačítko **Zavřít**.

    | ![](images/Cc747689.note(WS.10).gif)Poznámka                                                                |
    |------------------------------------------------------------------------------------------------------------------------------------------|
    | Zobrazí-li se chybová zpráva o restartování aplikace, aktualizujte stránku **Globální správa** v prohlížeči Microsoft Internet Explorer. |

Službu RMS můžete také nainstalovat z příkazového řádku. Příslušné pokyny získáte v tomto tématu později v části [Instalace serveru RMS z příkazového řádku](https://technet.microsoft.com/b55b1e2a-dd14-4168-a37f-9cdedbec660b).
