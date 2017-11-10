---
TOCTitle: Přemístění databáze protokolování
Title: Přemístění databáze protokolování
ms:assetid: '34ea8045-dc94-422e-9601-29927cfc1534'
ms:contentKeyID: 18113233
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc720238(v=WS.10)'
---

Přemístění databáze protokolování
=================================

Ve výchozí konfiguraci služby RMS jsou konfigurační databáze a databáze protokolování umístěny na stejný server. Pravidelně kontrolujte, zda je na serveru SQL Server dostatek volného místa pro obě databáze.

Pokud velikost databáze protokolování výrazně vzroste, můžete ji kdykoli přemístit na jiný server. Databázi protokolování však není možné přemístit pomocí webu pro správu. Namísto toho je třeba přemístění provést ručně následujícím postupem:

1.  Vypněte protokolování postupem popsaným v tomto tématu později v části [Zapnutí a vypnutí protokolování](https://technet.microsoft.com/8e672f95-566f-4070-9a2a-2f70f087148f).
2.  Pomocí správce SQL Server Enterprise Manager zkopírujte databázi protokolování ze zdrojového serveru na cílový server. Ujistěte se, že v nové databázi jsou vytvořeny tabulky a uložené procedury. Jeden ze způsobů kopírování databáze je použití Průvodce kopírováním databáze správce SQL Server Enterprise Manager.
3.  Změňte konfigurační databázi tak, aby v ní byl zohledněn nový název serveru a databáze. V tabulce DRMS\_ClusterPolicies konfigurační databáze pro cluster, pro nějž je databáze přemisťována, proveďte následující úpravy:
    -   Změňte hodnotu zásady LoggingDatabaseServer podle nového názvu databázového serveru.
    -   Změňte hodnotu zásady LoggingDatabaseName podle nového názvu databáze.

    > [!NOTE]
    > Správce SQL Server Enterprise Manager nepracuje s poli typu db\_variant, k provedení této úlohy jej tedy nelze použít. Je však možné použít nástroj Query Analyzer dodávaný se serverem SQL Server nebo jiný nástroj pro provádění úprav databáze. 

4.  Restartujte službu IIS na všech serverech v clusteru.
5.  Znovu zapněte protokolování.
