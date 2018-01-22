---
TOCTitle: Určení požadavků přístupu
Title: Určení požadavků přístupu
ms:assetid: 'eb2ce9a5-0430-4811-bd40-4a94a84426a8'
ms:contentKeyID: 18113540
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747790(v=WS.10)'
---

Určení požadavků přístupu
=========================

Během této části fáze plánování bylo nutné určit rozsah implementace služby RMS. Při posuzování zabezpečení systému RMS byste měli zvážit způsoby, kterými lze omezit možnosti účastníků a zajistit, aby data chráněná prostřednictvím služby RMS byla zároveň zabezpečena tradičními doporučenými postupy zabezpečení informací. Měli byste také zajistit, aby byl přístup k serveru RMS za účelem správy a konfigurace vyhrazen pouze důvěryhodným správcům. Mezi způsoby zabezpečení přístupu, které lze se službou RMS použít, patří následující možnosti:

-   **Seznamy řízení přístupu (ACL)**. Každou webovou službu RMS a web pro správu lze chránit prostřednictvím seznamů řízení přístupu. Chcete-li zajistit, aby službu RMS využívali pouze oprávnění uživatelé, můžete pomocí seznamů řízení přístupu omezit možnost připojení uživatelů ke službám certifikace a licencování služby RMS. Tento postup může být užitečný v případě, že chcete povolit vytváření chráněného obsahu nebo získání licencí na chráněný obsah jen určitým skupinám.

-   **Ověřování klientů**. Jakmile uživatel odešle požadavek na získání licence k použití nebo certifikátu, můžete vyžadovat také ověřování pomocí karet Smart Card či jiný typ ověřování klienta. Tímto způsobem je možné omezit riziko otevření obsahu neoprávněným uživatelem prostřednictvím relace oprávněného uživatele.

-   **Protokol SSL (Secure Sockets Layer)**. Chcete-li zajistit další vrstvu ochrany, můžete také požadovat zabezpečení připojení mezi klienty RMS a serverem RMS pomocí protokolu SSL. U každého souboru webových služeb RMS je vhodné povolit protokol SSL a vyžadovat 128bitové šifrování. Uvedené soubory mají příponu ASMX a najdete je ve virtuálních adresářích Licensing, Certification a Admin. Protokol SSL je nutné povolit, pokud chcete otevřít webové stránky pro **správu služby RMS** z prohlížeče ve vzdáleném počítači. Přestože protokol SSL povolíte, nebude možné ze vzdáleného počítače otevřít stránku **Globální správa**.

    Informace o konfiguraci protokolu SSL na serverech najdete v nápovědě ke službě IIS.

Některé organizace požadují systém správy licencí pro určité oddělení, který je zabezpečený a izolovaný od ostatních oddělení. Server RMS je možné využít i v případě takového scénáře. Zajistí způsob vytvoření zásad správy přístupových práv k informacím. Jestliže je součástí organizace oddělení nebo pobočka, které pracují s velmi citlivým obsahem, je vhodné zvážit instalaci zvláštního serveru či clusteru správy licencí, aby bylo možné spravovat licencování a publikování uvedeného obsahu odděleně od zbývajících částí organizace. Je proveden dílčí zápis serveru správy licencí u serveru (nebo clusteru) kořenové certifikace, který poskytuje certifikaci a další služby každému serveru správy licencí. Servery správy licencí však nabízejí vlastní služby správy licencí a publikování.

Důležitými prvky nasazení jsou uživatelské účty, seznamy řízení přístupu (ACL) a fyzické zabezpečení. Před implementací služby RMS do provozního prostředí zajistěte, aby byly odpovídajícím způsobem vyhodnoceny a zaimplementovány všechny doporučené postupy zabezpečení a příslušný model zabezpečení.
