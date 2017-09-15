---
TOCTitle: Klíče serveru RMS
Title: Klíče serveru RMS
ms:assetid: '5f4100a1-9aa5-42af-85c8-4bc691022f06'
ms:contentKeyID: 18113288
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc720280(v=WS.10)'
---

Klíče serveru RMS
=================

Serveru RMS je přiřazen pár 1024bitových klíčů RSA.

Veřejný klíč serveru slouží k šifrování klíče obsahu v licenci k publikování, takže pouze příslušný server RMS může načíst klíč obsahu a na základě licence k publikování vydat licence k použití. Klientský certifikát pro poskytování licencí obsahuje veřejný klíč serveru.

Soukromý klíč serveru se používá k podpisu všech certifikátů a licencí, které vydal daný server.

Ochrana soukromého klíče serveru
--------------------------------

Ve výchozím nastavení je během procesu zajišťování vytvořen soukromý klíč serveru, který je uložen v databázi služby RMS v zašifrované podobě. Pro zajišťování lze také určit zprostředkovatele kryptografických služeb (CSP), který je již instalován na serveru.

Zprostředkovatele CSP lze použít dvěma způsoby:

-   Vyberte některou ze softwarových implementací zprostředkovatele CSP, které jsou ve výchozím stavu instalovány serverem.
    -nebo-
-   Použijte softwarového zprostředkovatele kryptografických služeb od jiné společnosti než Microsoft, který je na daném serveru již nainstalován.

| ![](images/Cc720280.note(WS.10).gif)Poznámka                                                                           |
|-----------------------------------------------------------------------------------------------------------------------------------------------------|
| Chcete-li použít hardwarový modul zabezpečení, zkontrolujte, zda jste vybrali zprostředkovatele CSP, který podporuje hardwarové moduly zabezpečení. |

Pokud se rozhodnete zabezpečit soukromý klíč serveru pomocí zprostředkovatele kryptografických služeb, uloží služba RMS název tohoto zprostředkovatele a název kontejneru klíčů z konfigurační databáze.
