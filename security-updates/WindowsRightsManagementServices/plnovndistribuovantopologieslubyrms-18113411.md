---
TOCTitle: Plánování distribuované topologie služby RMS
Title: Plánování distribuované topologie služby RMS
ms:assetid: '8773a1e0-6ac3-41f5-9866-5890cef08d04'
ms:contentKeyID: 18113411
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747657(v=WS.10)'
---

Plánování distribuované topologie služby RMS
============================================

Může se stát, že v některých případech bude nutné nasadit nejméně jeden server správy licencí, který nebude členem clusteru kořenové certifikace. Tímto postupem je obvykle zajišťována podpora oddělení vyžadujících přímou kontrolu nad vydáváním licencí k publikování i k použití. Může se například jednat o právní oddělení s požadavky na zabezpečení, které vyžadují řízení na úrovni oddělení. Cluster kořenové certifikace poskytuje serverům správy licencí službu certifikace účtů. Kombinace clusteru kořenové certifikace a nejméně jedné instalace serveru správy licencí je označována jako distribuovaná topologie.

Servery správy licencí lze podobně jako server kořenové certifikace nasadit v clusteru. Cluster správy licencí také stejně jako cluster kořenové certifikace využívá vlastní službu vyrovnávání zatížení. Každý server nebo cluster správy licencí využívá zvláštní instanci databázového systému SQL Server, ve kterém jsou umístěny konfigurační databáze a databáze protokolování daného serveru nebo clusteru.

Přestože můžete instalaci služby RMS nastavit na spuštění služeb certifikace pouze z kořenové instalace a spuštění celé služby správy licencí z jednoho či více serverů nebo clusterů správy licencí, není taková konfigurace obvyklá. Potřebujete-li zvýšit výkon nebo redundanci dat, bude obecně vhodnější zvyšovat počet fyzických serverů v clusteru kořenové certifikace, než implementovat samostatné servery správy licencí (pokud ovšem nechcete zavést podporu správy licencí v rámci oddělení). Tento způsob implementace ilustruje následující diagram.

![](images/Cc747657.01fa5a85-5711-41aa-932a-124049d34186(WS.10).gif)

Vytvoření distribuované topologie může zvýšit náklady organizace na správu, protože tato topologie je ve své podstatě komplexnější. Pokud organizace používá více clusterů správy licencí a více doménových struktur, bude pravděpodobně nutné přepsat registr v klientských počítačích služby RMS a zajistit tak, aby své požadavky na licencování vytvářeli pomocí správného serveru RMS. Mezi doménami dále mohou vyvstat problémy s důvěryhodností. To vyžaduje další konfiguraci domén na povolení využívání obsahu chráněného službou RMS.

Spojovací body služby v distribuované topologii
-----------------------------------------------

Při zajišťování serveru RMS je adresa URL clusteru přidána do doménové struktury služby Active Directory ve spojovacím bodu služby. Spojovací bod služby je vytvořen pro cluster kořenové certifikace a pro každý cluster správy licencí, který jste v doménové struktuře zajistili. Spojovací bod služby clusteru kořenové certifikace je nutné zaregistrovat ještě před zajištěním clusteru správy licencí. Při zajišťování clusteru správy licencí je během dílčího zápisu prostřednictvím této adresy URL vyhledán cluster kořenové certifikace v dané síti a získán certifikát serveru pro poskytování licencí.

Pokud místo jediného serveru kořenové certifikace nasazujete cluster kořenové certifikace, je nutné pro každý server v tomto clusteru vytvořit virtuální adresu v rámci sdílené adresy URL.

K dispozici je několik způsobů implementace virtuálního adresování, jako například kruhové dotazování (round robin) DNS, služba Vyrovnávání zatížení sítě, hardwarová řešení a další. Virtuální adresování slouží k vyrovnávání zatížení mezi servery a odstraňuje závislost správy licencí a publikování na jediném serveru.

Služba RMS používá sdílenou adresu URL pro adresu URL umožňující získávání licencí a také pro publikovanou hodnotu, pomocí které počítače koncových uživatelů vyhledávají svůj cluster služby RMS ve službě Active Directory nebo v registru. Žádný z počítačů koncových uživatelů nepotřebuje přímý přístup k jednotlivým počítačům obsaženým v clusteru.
