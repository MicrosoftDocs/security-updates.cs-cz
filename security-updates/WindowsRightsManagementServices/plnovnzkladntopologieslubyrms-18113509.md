---
TOCTitle: Plánování základní topologie služby RMS
Title: Plánování základní topologie služby RMS
ms:assetid: 'fec3201e-201f-4faf-910e-fa44132af83d'
ms:contentKeyID: 18113509
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747755(v=WS.10)'
---

Plánování základní topologie služby RMS
=======================================

Základní topologii služby RMS tvoří jeden nebo více fyzických serverů, které slouží jako cluster kořenové certifikace. Tento cluster zajišťuje v organizaci správu certifikátů, licencí a publikování. S výjimkou těch nejmenších implementací připadá na jednu adresu URL vždy cluster tvořený několika fyzickými servery. Cluster lze vytvořit tak, že zajistíte první server a nastavíte jej jako server kořenové certifikace. Potom do clusteru přidáváte další servery, dokud není dosažen počet serverů kořenové certifikace nutný k podpoře plánované činnosti. Tuto topologii ilustruje následující obrázek.

![](images/Cc747755.a3332719-4d25-4694-a89a-7c31fd97ca3b(WS.10).gif)

Servery připojené ke clusteru sdílejí společnou konfigurační databázi a databázi protokolování. K tomuto účelu se používají databáze SQL Server. Databáze SQL Server může být umístěna ve stejném počítači jako server kořenové certifikace nebo na samostatném serveru.

Mezi všemi servery, které jsou součástí clusteru kořenové certifikace, je nastaveno vyrovnávání zatížení. Všechny požadavky na certifikáty a licence jsou clusteru kořenové certifikace předávány prostřednictvím společné adresy URL, kterou zadáte během konfigurace prvního serveru v tomto clusteru.

Jestliže budete podporovat malý počet klientů, můžete službu RMS nainstalovat na jediný server s místní databází. Tento server pak bude zajišťovat veškerou správu certifikátů a licencí v organizaci. V případě selhání však za tento server neexistuje náhrada, a proto se doporučuje provádět pravidelné zálohování.
