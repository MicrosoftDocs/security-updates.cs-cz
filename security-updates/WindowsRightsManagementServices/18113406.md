---
TOCTitle: Licence k publikování
Title: Licence k publikování
ms:assetid: '187228fc-370b-4e23-a53a-21bb296b84a1'
ms:contentKeyID: 18113406
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc720211(v=WS.10)'
---

Licence k publikování
=====================

Uživatelé aplikací s podporou služby RMS mohou digitálním souborům a informacím přiřadit specifická práva využití, která jsou v souladu s existujícími podnikovými zásadami. Uvedená práva využití jsou uložena v licencích k publikování. Ty určují uživatele, kteří mohou zobrazit obsah, a také způsob, jakým mohou tento obsah upravovat a distribuovat.

Licenci k publikování může vydat klientská aplikace s podporou služby RMS, server kořenové certifikace nebo server správy licencí služby RMS. Pokud licenci k publikování vydá klientská aplikace s podporou služby RMS, je této aplikaci serverem RMS udělen klientský certifikát pro poskytování licencí. Tento postup je označován jako publikování offline. Jedná se o běžný způsob publikování, protože uživatelům aplikací s podporou služby RMS umožňuje vytvářet chráněný obsah bez nutnosti připojení k serveru RMS. Jestliže klientská aplikace s podporou služby RMS klientský certifikát pro poskytování licencí nepoužívá, vyžaduje získání licence k publikování pro chráněný obsah připojení uživatele k serveru RMS.

Licence k publikování obsahuje symetrický klíč obsahu umožňující dešifrování obsahu šifrovaného pomocí veřejného klíče serveru RMS. To zajišťuje, že šifrování obsahu a vydávání licencí k použití může provádět pouze server.

Licence k publikování je podepsána soukromým klíčem vydávajícího serveru nebo soukromým klíčem klientského certifikátu pro poskytování licencí.
