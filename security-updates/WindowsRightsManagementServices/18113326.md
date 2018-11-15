---
TOCTitle: Zabezpečení nasazení služby RMS
Title: Zabezpečení nasazení služby RMS
ms:assetid: '6de8b636-a824-4844-aefc-f26347abfc14'
ms:contentKeyID: 18113326
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc720291(v=WS.10)'
---

Zabezpečení nasazení služby RMS
===============================

Nasazení služby RMS je aktivem organizace, která vyžaduje stejná fyzická a síťová bezpečnostní opatření jako jiné důležité servery v infrastruktuře. V rámci nasazení byste měli určit hrozby a protiopatření pro servery RMS.

Služba RMS je implementována jako webová služba, takže přístup k ní je možné řídit stejným způsobem jako u ostatních webových služeb, a to pomocí seznamů řízení přístupu a protokolu SSL (Secure Sockets Layer).

**Omezení přístupu k webovým službám RMS pomocí seznamů řízení přístupu**

Přístup ke službám RMS můžete omezit pomocí seznamů řízení přístupu. Každý z virtuálních kořenů vytvořených při zajišťování služby RMS na webu obsahuje odpovídající strukturu složek, kterou lze zabezpečit. Struktura složek je ve výchozím nastavení umístěna v adresáři &lt;systémová jednotka&gt;:\\&lt;*kořenová\_složka\_webu*&gt;\\\_wmcs, kde *kořenová\_složka\_webu* je název složky, která je přiřazena k webu zajišťujícímu službu RMS. Některé webové služby (například služba dílčího zápisu, služba certifikace mobilních zařízení a služba certifikace serverové služby) jsou omezeny ve výchozím nastavení a uživatele nebo skupiny, kterým chcete používání dané služby povolit, je nutné explicitně přidat do seznamu řízení přístupu.

Služba certifikace serverové služby poskytuje certifikáty účtů práv, pomocí nichž mohou k obsahu chráněnému službou RMS získat přístup služby, jako jsou služby pro webovou spolupráci, poštovní servery a servery pro správu dokumentů, za účelem podpory rozšíření systému služby RMS, například:

-   Server pro spolupráci na dokumentech, na který mohou uživatelé odesílat nezabezpečené dokumenty. U stažených dokumentů však bude automaticky nastavena ochrana službou RMS v souladu se zásadami práv pro daný typ obsahu. Jedním z příkladů je Microsoft Office SharePoint Server 2007.
-   Systém správy dokumentů jako obecné úložiště a archiv chráněných i nechráněných dokumentů. Systém bude umožňovat indexování dokumentů chráněných právy, aby je bylo možné vyhledávat, přičemž budou zachovány zásady práv definované autorem obsahu.
-   Poštovní server bude schopen rychle otevírat obsah chráněný právy za účelem kontroly virů, spamu nebo jako součást zákonných požadavků nebo zásad společnosti pro práci s poštou.

Protože tyto situace vyžadují licence jménem uživatelů, je třeba vyžadovat, aby byla možnost získávat certifikáty účtu práv omezena pouze na servery ve vaší organizaci, které byly schváleny pro tuto funkci a jsou příslušně zabezpečeny.

**Omezení přístupu k webovým službám RMS pomocí protokolu SSL**

U každého souboru webových služeb RMS je doporučeno povolit protokol SSL (Secure Sockets Layer) a vyžadovat 128bitové šifrování. Uvedené soubory mají příponu ASMX a najdete je ve virtuálních adresářích Licensing, Certification a Admin. Protokol SSL vyžaduje, aby byl na příslušném serveru nainstalován platný certifikát SSL pro daný web. Pokud použijete protokol SSL pro složku \_wmcs instalace RMS, zdědí toto nastavení také podsložky a soubory. Další informace o souborech a virtuálních adresářích webových služeb získáte v části Internetová informační služba tématu Technické informace týkající se služby RMS v této sadě dokumentace.

> [!NOTE]
> Chcete-li otevřít webové stránky pro správu služby RMS v systému Windows v prohlížeči vzdáleného počítače, je nutné povolit protokol SSL. Přestože protokol SSL povolíte, nebude možné ze vzdáleného počítače otevřít stránku **Globální správa**. Další informace o vzdálené správě služby RMS získáte v tématu Práce s domovskou stránkou v části RMS: Provoz této sady dokumentace. 

**Nastavení silného hesla soukromého klíče**

Heslo soukromého klíče slouží ke generování a zabezpečenému uložení soukromého klíče v konfigurační databázi služby RMS. Za účelem zajištění maximálního zabezpečení se doporučuje silné heslo. Pokud je nutné si heslo poznamenat, uložte ho na fyzicky zabezpečeném místě.

> [!CAUTION]
> Pokud při ztrátě nebo zapomenutí hesla soukromého klíče přejde server RMS neočekávaně do režimu offline, bude nutné dešifrovat všechny dokumenty RMS, znovu vytvořit prostředí RMS a znovu vše zašifrovat pomocí nového soukromého klíče. 
