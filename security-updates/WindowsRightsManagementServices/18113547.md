---
TOCTitle: Definování požadavků správy klíčů
Title: Definování požadavků správy klíčů
ms:assetid: 'f0e08fb8-bf5e-4278-a09f-daa57696e786'
ms:contentKeyID: 18113547
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747797(v=WS.10)'
---

Definování požadavků správy klíčů
=================================

Služba RMS zajišťuje ochranu obsahu a vynucení práv pomocí šifrovacích klíčů. Šifrovací klíče jsou důležité informační celky, které umožňují systému pružnou a bezpečnou práci. Správci musí věnovat zvýšenou pozornost vhodné správě těchto klíčů a ochraně před ztrátou dat, selháním systému a zcizením dat.

Ve výchozí konfiguraci ukládá služba RMS pár klíčů serveru a související identifikátor GUID do tabulky v konfigurační databázi. Pár klíčů serveru je zašifrován heslem, které zadáte během procesu zajišťování.

Chcete-li zvýšit zabezpečení páru klíčů serveru a souvisejícího identifikátoru GUID, zálohujte konfigurační databázi na médium (například disk CD-ROM) a uložte toto zálohovací médium na bezpečné místo (například do trezoru mimo pracoviště). Plánování zálohování závisí na tom, jak často provádíte změny spojené se správou, a na přijatelné úrovni rizika ztráty dat z důvodu snížení kvality média nebo dalších možných ohrožujících faktorů vyplývajících z jeho použití. Zajistěte si způsob, pomocí kterého zjistíte heslo soukromého klíče použitého u záložní konfigurační databáze. Bez příslušného hesla nebudete moci obnovit zálohu serveru RMS.

Jestliže jako databázový server používáte SQL Server, můžete pomocí správce SQL Server Enterprise Manager zkopírovat hodnotu šifrovaného soukromého klíče a identifikátoru GUID přímo na zabezpečenou disketu nebo jiné médium. Vzhledem k tomu, že je soukromý klíč chráněn, musí být instalace služby RMS spuštěna pod stejným účtem této služby jako záloha (pokud zálohu obnovujete ze zabezpečeného média do instalace služby RMS).

Jestliže jste ochranu soukromého klíče serveru zajistili prostřednictvím softwarového nebo hardwarového zprostředkovatele kryptografických služeb, je nutné kontejner klíče i klíč zálohovat ručně. Pokud použijete modul hardwarového zabezpečení, dosáhnete vyššího zabezpečení soukromých klíčů, protože soukromé klíče budou uchovávány v hardwarových zařízeních a software k nim nebude mít přístup. Data, která je třeba dešifrovat nebo podepsat, se předávají modulu hardwarového zabezpečení, kde dojde k jejich dešifrování či podepsání a následně k jejich vrácení.

Každý zprostředkovatel kryptografických služeb (hardwarový i softwarový) používá specifické procedury zabezpečeného zálohování klíče. Jestliže danou proceduru neznáte, získáte další informace v dokumentaci k danému zprostředkovateli.
