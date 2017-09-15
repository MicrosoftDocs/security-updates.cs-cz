---
TOCTitle: 'Nejčastější dotazy týkající se služby RMS: Interní a externí přístup'
Title: 'Nejčastější dotazy týkající se služby RMS: Interní a externí přístup'
ms:assetid: '59c2c51f-6c20-450c-a334-0e1486292074'
ms:contentKeyID: 18113321
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747577(v=WS.10)'
---

Nejčastější dotazy týkající se služby RMS: Interní a externí přístup
====================================================================

Nejčastější dotazy týkající se interního a externího přístupu ke službě RMS
---------------------------------------------------------------------------

-   [Jaké změny brány firewall je nutné provést, aby k serverům RMS mohli získat přístup klienti za touto bránou?](#bkmk_37)
-   [Jak vypadá extranetový scénář?](#bkmk_38)
-   [Jestliže uživatel vytvoří obsah chráněný právy a poskytne jej uživateli bez přístupu k instalaci služby RMS, může příjemce obsah využít?](#bkmk_39)
-   [Pokud některému zákazníkovi odešlu pomocí aplikace Outlook 2003 nebo Outlook 2007 e-mail chráněný právy, co potřebuje příjemce k jeho přečtení?](#bkmk_40)
-   [Jestliže organizace používají vlastní servery RMS, jakým způsobem si mohou obsah chráněný právy navzájem vyměňovat?](#bkmk_41)
-   [Pokud je odeslán e-mail chráněný službou RMS do jiné organizace, která nepodporuje aplikaci Outlook, může příjemce na přečtený e-mail odpovědět pomocí doplňku pro správu práv pro aplikaci Internet Explorer?](#bkmk_42)

<span id="BKMK_37"></span>
#### Jaké změny brány firewall je nutné provést, aby k serverům RMS mohli získat přístup klienti za touto bránou?

Brána firewall musí počítačům na druhé straně umožnit odesílání požadavků SOAP (Simple Object Access Protocol) na server RMS prostřednictvím protokolu HTTP (port TCP 80) nebo protokolu HTTPS (port TCP 443).

<span id="BKMK_38"></span>
#### Jak vypadá extranetový scénář?

Licence k publikování svázaná s určitým obsahem obsahuje dvě adresy URL. První je intranetová adresa URL nastavená při zajišťování clusteru služby RMS. Druhou představuje extranetová adresa URL, kterou může nastavit správce služby RMS. Tato extranetová adresa URL umožňuje klientovi získat licence k použití vně brány firewall. Extranetovou adresu URL nelze použít při vytváření nového obsahu chráněného právy. V takovém případě je vyžadován přepis registru klienta RMS.

<span id="BKMK_39"></span>
#### Jestliže uživatel vytvoří obsah chráněný právy a poskytne jej uživateli bez přístupu k instalaci služby RMS, může příjemce obsah využít?

Pokud uživatel není k dané instalaci služby RMS připojen při prvním otevření chráněného obsahu, nemůže tento obsah využít.

Sada Office 2003 a vyšší automaticky získává licence k použití pro e-maily chráněné právy při synchronizaci, takže tyto e-maily lze číst i bez připojení k síti. Zatímco však aplikace Outlook 2003 a vyšší automaticky ukládá licence k použití pro e-mail do mezipaměti, budou každému dokumentu aplikace Excel 2007, Excel 2003, Word 2007, Word 2003, PowerPoint 2007 a PowerPoint 2003 přiřazena stejná práva jako e-mailu, se kterým byly odeslány ve formě přílohy. Při stažení e-mailu nedochází automaticky k jejich synchronizaci, takže musí být otevřeny jednotlivě v okamžiku, kdy je počítač připojen k síti, aby bylo možné získat licenci k použití.

<span id="BKMK_40"></span>
#### Pokud některému zákazníkovi odešlu pomocí aplikace Outlook 2003 nebo Outlook 2007 chráněný e-mail, co potřebuje příjemce k jeho přečtení?

Příjemce potřebuje aplikaci Outlook 2003, Outlook 2007 nebo doplněk pro správu práv pro aplikaci Internet Explorer. Jestliže organizace příjemce vytvořila vztah důvěryhodnosti mezi svou a vaší instalací služby RMS, může příjemce daný e-mail číst bez nutnosti dalších kroků. Vztah důvěryhodnosti lze vytvořit vzájemnou výměnou certifikátů serveru pro poskytování licencí služby RMS, které obsahují odpovídající veřejné klíče.

Pokud organizace příjemce nemá vlastní infrastrukturu služby RMS nebo nedošlo k vytvoření žádného vztahu důvěryhodnosti, můžete svého zákazníka požádat o vytvoření účtu služby Windows Live ID a odeslat e-mail konkrétnímu příjemci zadáním práv, která jsou přiřazena pověřením účtu služby Windows Live ID tohoto zákazníka. Tento postup využívá při získávání licence k použití technologii IRM společnosti Microsoft, která je k dispozici na Internetu. Technologie IRM je uživatelům poskytována bezplatně pro zkušební provoz a je určena pouze pro testování služby RMS. Rozhodnete-li se chránit obsah prostřednictvím této služby, mějte na paměti, že v budoucnosti může bez oznámení dojít k ukončení jejího provozu.

<span id="BKMK_41"></span>
#### Jestliže organizace používají vlastní servery RMS, jakým způsobem si mohou obsah chráněný právy navzájem vyměňovat?

Služba RMS používá důvěryhodné domény uživatelů, v rámci kterých jsou certifikáty uživatelů generované jednou instalací služby RMS pokládány za důvěryhodné také druhou instalací.

<span id="BKMK_42"></span>
#### Pokud je odeslán e-mail chráněný službou RMS do jiné organizace, která nepodporuje aplikaci Outlook, může příjemce na přečtený e-mail odpovědět pomocí doplňku pro správu práv pro aplikaci Internet Explorer?

Příjemce může na e-mail chráněný právy odpovědět stejně jako na každý jiný e-mail, ale původní text přijatého e-mailu zůstane pro původní příjemce chráněn právy. Způsob zabalení tohoto e-mailu určuje příslušná klientská aplikace. Původní e-mail může být do odpovědi připojen jako šifrovaná příloha nebo může být úplně odebrán (jako například v aplikaci Outlook 2003 nebo Outlook 2007).
