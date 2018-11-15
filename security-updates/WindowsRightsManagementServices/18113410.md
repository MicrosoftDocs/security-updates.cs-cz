---
TOCTitle: Rozpoznání služby dílčího zápisu
Title: Rozpoznání služby dílčího zápisu
ms:assetid: 'b159953a-af38-4a9e-8c87-1aff5fb4e366'
ms:contentKeyID: 18113410
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747641(v=WS.10)'
---

Rozpoznání služby dílčího zápisu
================================

Samostatný server správy licencí nebo první server správy licencí v clusteru musí serveru kořenové certifikace služby RMS odeslat požadavek na dílčí zápis a získat certifikát serveru pro poskytování licencí. Server správy licencí následujícím způsobem získá adresu URL služby dílčího zápisu na serveru kořenové certifikace, aby byl uvedený krok možný.

Během zajišťování serveru správy licencí odešle instalační program služby RMS dotaz na službu Active Directory a zjišťuje spojovací bod služby pro cluster kořenové certifikace. Služba RMS pomocí adresy URL uložené v daném spojovacím bodě služby vyhledá cluster kořenové certifikace a potom ze služby dílčího zápisu na serveru kořenové certifikace odešle požadavek na certifikát serveru pro poskytování licencí.

Server správy licencí vytvoří požadavek na službu dílčího zápisu tak, že z adresáře služby Active Directory nejprve načte požadovanou adresu URL pro virtuální adresář Certification serveru kořenové certifikace, na kterém je služba dílčího zápisu umístěna. Potom ke službě dílčího zápisu připojí cestu.

Adresa URL virtuálního adresáře Certification na serveru kořenové certifikace může být ve službě Active Directory uložena například v následující podobě:

http://*název\_serveru*/\_wmcs/Certification

Jakmile server správy licencí odesílá požadavek na službu dílčího zápisu, připojí k adrese URL příslušný název souboru služby:

http://název\_serveru/\_wmcs/Certification/SubEnrollService.asmx

> [!NOTE]
> Jestliže jste na serveru povolili protokol SSL, budou tyto adresy URL používat protokol připojení https://. 
