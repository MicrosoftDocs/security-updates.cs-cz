---
TOCTitle: Zálohování systému pro službu RMS
Title: Zálohování systému pro službu RMS
ms:assetid: 'c29894da-ee00-428c-8d48-80d8e5a83678'
ms:contentKeyID: 18113491
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747746(v=WS.10)'
---

Zálohování systému pro službu RMS
=================================

Před nastavením infrastruktury a instalací služby RMS zálohujte odpovídajícím způsobem následující součásti:

-   Pokud bude hostitelem konfigurační databáze a databáze protokolování existující SQL Server, zálohujte všechny databáze a veškeré nastavení serveru. V případě upgradu předchozí verze služby RMS nebo přeinstalace této služby zajistěte zálohování předchozí konfigurace a databází protokolování.
-   Zálohujte stav systému serveru, na který chcete službu RMS instalovat. V této záloze budou uloženy klíče a hodnoty registru obsahující informace nutné k obnovení serveru v případě potřeby.
-   Vyexportujte své certifikáty do souboru pomocí modulu snap-in Certifikáty. Tento modulu snap-in lze také využít k zálohování dat soukromého klíče služby RMS do heslem zašifrovaného souboru PKCS \#12. Pokud jste při upgradu nebo přeinstalaci služby RMS zabezpečili její soukromý klíč prostřednictvím výchozího softwarového šifrování, je tento klíč zašifrován a uložen v záloze konfigurační databáze.
-   Jestliže k zabezpečení soukromého klíče používáte hardwarový modul zabezpečení, měli byste zálohovat jeho konfiguraci způsobem doporučeným jeho výrobcem.

Záložní soubory je třeba uložit na bezpečné místo spolu s heslem použitým k zašifrování soukromých klíčů.
