---
TOCTitle: Vyřazení serverů RMS z provozu
Title: Vyřazení serverů RMS z provozu
ms:assetid: '11badb02-62c1-455c-96b7-935bbcb496bc'
ms:contentKeyID: 18113277
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc720200(v=WS.10)'
---

Vyřazení serverů RMS z provozu
==============================

Po vyřazení služby RMS z provozu se chování serveru RMS změní a je možné získat klíč použitý k šifrování obsahu chráněného správou přístupových práv, který byl serverem v minulosti publikován. Tento klíč umožňuje uložit obsah bez ochrany správou přístupových práv. Uvedený krok může být užitečný v případě, že již nechcete v rámci organizace používat ochranu správou přístupových práv.

Server by měl být spuštěn jako vyřazený z provozu dostatečně dlouho, aby měli uživatelé možnost uložit svůj obsah bez ochrany správou přístupových práv a aby mohli správci sítě a systému zakázat používání této služby u klientů podporujících správu přístupových práv.

Vyřazení z provozu je možné zapnout na stránce **Nastavení zabezpečení** webu pro správu. Jakmile je vyřazení z provozu zapnuto, nelze na serveru RMS obnovit standardní konfiguraci. Pokud instalace obsahovala důvěryhodné domény publikování, budou tyto domény také vyřazeny z provozu.

Pokud je zapnuto vyřazení z provozu, bude web pro správu obsahovat pouze stránku **Informace o serveru vyřazeném z provozu** a provádění správy nebude podporováno. Vyřazení serveru z provozu lze provést pomocí následujícího postupu:

1.  Udělte skupině **RMS Service Group** oprávnění pro čtení a spouštění k vyřazovanému virtuálnímu kořenu.
2.  Přidejte skupinu **Everyone** do seznamu DACL souboru decommissioning.asmx s oprávněním ke čtení.
3.  Informujte uživatele, že vyřazujete instalaci služby RMS z provozu, a poraďte jim, aby se připojili k příslušnému serveru a uložili obsah bez ochrany správou přístupových práv.
4.  Nakonfigurujte všechny aplikace s podporou správy přístupových práv v rámci podniku, aby se připojovaly ke stránce decommissioning.asmx. V závislosti na aplikaci s podporou správy přístupových práv může být tato možnost řízena klíčem registru nebo nastavením zásad skupiny.
5.  Pokud daná organizace používá aplikace s podporou správy přístupových práv, které instalaci automaticky používají k publikování, měli byste pomocí zásad skupiny v daných počítačích nastavit položku registru tak, aby aplikace používaly službu vyřazení z provozu.
6.  Po zrušení ochrany veškerého obsahu byste měli vytvořit záložní kopii soukromého klíče serveru a službu RMS ze serveru odinstalovat.
