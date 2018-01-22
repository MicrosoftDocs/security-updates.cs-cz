---
TOCTitle: Import a použití sady RMS Management Pack
Title: Import a použití sady RMS Management Pack
ms:assetid: 'd9a73ef0-2f81-48c2-97cc-deb7bf477389'
ms:contentKeyID: 18113462
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747688(v=WS.10)'
---

Import a použití sady RMS Management Pack
=========================================

Import a použití sady RMS Management Pack
-----------------------------------------

#### Import a použití sady RMS Management Pack

1.  Zkopírujte sadu RMS Management Pack (RMS\_MOMPack.akm) ze složky %ProgramFiles%\\Windows Rights Management Services\\Tools na server MOM (Microsoft Operations Manager).

2.  Otevřete konzolu správce MOM a importujte sadu RMS Management Pack následujícím postupem:

    1.  Ve stromu konzoly správce MOM rozbalte položku **Rules** (Pravidla) a klepněte pravým tlačítkem myši na položku **Processing Rule Groups** (Skupiny pravidel zpracování).
    2.  V místní nabídce klepněte na položku **Import Management Pack** (Import sady správy). Zobrazí se dialogové okno **Import Management Pack** (Import sady správy).
    3.  Klepněte na tlačítko **Browse** (Procházet) a vyberte soubor RMS\_MOMPack.akm.

3.  Zadejte možnosti sloučení nebo nahrazení. Další informace o možnostech sloučení a nahrazení naleznete na stránce Exporting and Importing Management Packs (Export a import sad správy) na webu společnosti Microsoft (http://www.microsoft.com/).

    Klepněte na tlačítko **Replace** (Nahradit). Pokud nastavíte nahrazování, importovaná sada správy přepíše stávající skupiny pravidel zpracování. Nebudou zachovány žádné poznámky uživatelů. Chcete-li tuto sadu správy sloučit s existující sadou správy, měli byste to provést v testovacím prostředí a při nasazení sady správy do provozního prostředí pak použít možnost **Replace** (Nahradit).

4.  Importujte sadu správy klepnutím na tlačítko **Import**.

5.  V konzole **správce MOM** vyberte položku **Configuration** (Konfigurace) a poté klepněte na složku **Agent Managers** (Správci agentů).

6.  Pravým tlačítkem myši klepněte na název serveru, na který jste importovali sadu RMS Management Pack, a klepněte na položku **Scan Managed Computers Now** (Skenovat spravované počítače).
