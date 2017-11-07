---
TOCTitle: Registrace spojovacího bodu služby
Title: Registrace spojovacího bodu služby
ms:assetid: '446d83ec-3224-45e2-9697-625e7db338f3'
ms:contentKeyID: 18113262
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc720260(v=WS.10)'
---

Registrace spojovacího bodu služby
==================================

Spojovací bod služby (bod SCP) určuje adresu URL připojení služby RMS pro klienty v rámci organizace, kteří podporují správu přístupových práv. Klienti bez platného spojovacího bodu služby nebudou moci zjistit službu RMS a odesílat požadavky na licence k použití, licence k publikování či certifikáty účtů s právy.

Registraci adresy URL spojovacího bodu služby pro cluster kořenové certifikace je možné provést na stránce **Spojovací bod služby** webu pro správu. Na stránce **Spojovací bod služby** je také možné registraci adresy URL bodu SCP zrušit, je-li ji z nějakého důvodu třeba změnit. Registraci adresy URL nebo její zrušení je možné provádět za předpokladu, že jste přihlášeni k platnému účtu uživatele domény, který má dostatečná oprávnění k vytvoření objektu kontejneru pod kontejnerem Služby.

Pod kontejnerem služeb ve službě Active Directory bude vytvořen nový objekt kontejneru s názvem RightsManagementServices. Pod tímto kontejnerem bude vytvořen objekt bodu SCP nazvaný MSRMRootCluster. Pro tento objekt bodu SCP jsou pro atribut klíčových slov k dispozici dvě hodnoty:

-   MSRMRootCluster
-   1.0

Tyto atributy jsou používány klienty a ostatními servery k nalezení adresy URL kořenového clusteru ve službě Active Directory. Hodnota serviceBindingInformation objektu bodu SCP bude obsahovat adresu URL kořenového clusteru ve tvaru http://*nazev\_clusteru*/\_wmcs/Certification.
