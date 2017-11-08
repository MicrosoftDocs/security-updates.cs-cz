---
TOCTitle: Zabezpečení databází používaných službou RMS
Title: Zabezpečení databází používaných službou RMS
ms:assetid: '65802f9a-81bc-4398-968a-00c9b1dca2fa'
ms:contentKeyID: 18113304
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc720285(v=WS.10)'
---

Zabezpečení databází používaných službou RMS
============================================

Služba RMS vytváří a používá následující tři databáze, pro něž je vyžadována různá úroveň zabezpečení:

-   **Adresářové služby**: V této databázi jsou uloženy výsledky dotazů na členství ve skupině služby Active Directory. Vzhledem k tomu, že obsahuje pouze informace služby Active Directory, není kromě zabezpečení automaticky konfigurovaného při zajištění služby RMS třeba další zabezpečení.
-   **Protokolování**: Informace uložené v této databázi jsou citlivější než informace uložené v databázi adresářových služeb, protože jejich zveřejnění by mohlo ohrozit ochranu osobních údajů uživatelů. Společnost Microsoft věnuje zvláštní pozornost tomu, aby nebyly zaznamenávány žádné informace umožňující identifikaci osoby a aby veškeré informace zaznamenané do této databáze byly chráněny vhodnými prostředky zabezpečení. Není-li tato databáze přesunuta na jiný počítač se serverem SQL Server, není třeba provádět žádné změny jejího zabezpečení. Pokud je databáze přesunuta na jiný server, ověřte, že v novém prostředí je použit stejný způsob zabezpečení.
-   **Konfigurace**: Tato databáze je kromě soukromých klíčů serveru nejdůležitějším a nejhodnotnějším prostředkem nasazení služby RMS. Obsahuje citlivé a klíčové informace, které je třeba chránit. Kromě konfiguračních informací tato databáze obsahuje všechny certifikáty a klíče, šifrovaný soukromý klíč serveru (v případě, že nepoužíváte doporučené hardwarové šifrování) a hodnotu hash hesla soukromého klíče.

Při vytvoření konfigurační databáze služba RMS nastaví oprávnění pro omezení přístupu a zabezpečení databáze.

Zvýšení zabezpečení databáze
----------------------------

Následujícím postupem můžete zvýšit celkové zabezpečení uvedených databází umístěných v síti a v okolí serveru:

-   Databázový server spusťte v počítači se systémem Windows Server 2003. Tento operační systém je ve výchozím nastavení zabezpečenější než systém Windows 2000 Server. Počítač se systémem Windows 2000 Server je sice možné uzamknout, tento proces ale může být časově náročný. Při jeho provádění se také můžete dopustit chyb, kterých mohou uživatelé se zlými úmysly využít k získání přístupu k databázi.
-   Omezte fyzický přístup k databázovému serveru.
-   Zajistěte, aby databázová oprávnění a volitelné seznamy řízení přístupu (DACL) v souborech databází umožňovaly přístup pouze oprávněným osobám. Výchozí oprávnění a seznamy DACL konfigurované službou RMS jsou zabezpečené. Při změně výchozích nastavení proto postupujte opatrně.
-   Na databázovém serveru nespouštějte nepotřebné služby, například Internetovou informační službu (IIS) společnosti Microsoft, službu Řízení front zpráv nebo Terminálovou službu.
-   Na databázovém serveru nespouštějte jiné databáze kromě databází služby RMS.

Zabezpečte databáze serveru SQL Server konfigurací protokolu SSL nebo IPSec (Internet Protocol Security) pro zajištění šifrovaných kanálů. Šifrováním databázových komunikací můžete uživatelům se zlými úmysly zabránit v získání nebo ve změně zaznamenaných dat.

Další informace o konfiguraci protokolu SSL pro SQL Server naleznete na webu MSDN ([http://go.microsoft.com/fwlink/?LinkID=17060](http://go.microsoft.com/fwlink/?linkid=17060)) (stránka může být v angličtině).

Další informace o konfiguraci protokolu IPsec pro SQL Server 2000 naleznete na webu MSDN ([http://go.microsoft.com/fwlink/?LinkID=17061](http://go.microsoft.com/fwlink/?linkid=17061)) (stránka může být v angličtině).

Další informace o zabezpečení řady operačních systémů Microsoft Windows Server 2003 získáte v příručce týkající se zabezpečení systému Windows Server 2003, která je dostupná prostřednictvím služby Stažení softwaru ([http://go.microsoft.com/fwlink/?LinkID=36719](http://go.microsoft.com/fwlink/?linkid=36719)) (stránka může být v angličtině).
