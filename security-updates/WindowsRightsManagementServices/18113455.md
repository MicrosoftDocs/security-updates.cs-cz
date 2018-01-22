---
TOCTitle: Přidání a odebrání důvěryhodných domén publikování
Title: Přidání a odebrání důvěryhodných domén publikování
ms:assetid: 'd87b502d-5497-4ccd-badf-f6807d587cee'
ms:contentKeyID: 18113455
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747687(v=WS.10)'
---

Přidání a odebrání důvěryhodných domén publikování
==================================================

Ve výchozím nastavení může server RMS vydávat licence k použití pouze na základě licencí k publikování vydaných daným serverem nebo jiným serverem ze stejného clusteru. Pokud je obsah publikovaný pomocí jiného serveru kořenové certifikace buď v organizaci, například místní zastoupení organizace v jiné doménové struktuře, nebo v jiné samostatné organizaci, může server RMS přidělit licence k použití pro tento obsah za předpokladu, že na tomto serveru nakonfigurujete důvěryhodnou doménu publikování. Přidáním důvěryhodné domény publikování nastavíte vztah důvěryhodnosti mezi serverem RMS a jiným serverem kořenové certifikace, a to tak, že budete importovat certifikát serveru pro poskytování licencí druhého serveru. Počet důvěryhodných domén publikování, které lze nakonfigurovat pro server RMS, není omezen.

Přidanou důvěryhodnou doménu publikování můžete kdykoli odebrat odebráním jejího certifikátu ze seznamu certifikátů důvěryhodných domén publikování.

Chcete-li přidat důvěryhodnou doménu publikování, je třeba importovat certifikát serveru pro poskytování licencí, soukromý klíč (pokud není soukromý klíč uložen v hardwarovém, ale v softwarovém modulu zabezpečení) a všechny šablony zásad práv pro přidávaný server nebo cluster RMS. Správce musí nejprve exportovat tyto položky ze serveru nebo clusteru, který má být nastaven jako důvěryhodný, do souboru chráněného heslem a pak nastavit heslo určené k dešifrování tohoto souboru. Soubor je nutné umístit ve sdílené složce a správce vám musí sdělit příslušné heslo. Poté můžete soubor importovat tak, že určíte jeho umístění a zadáte heslo. Chcete-li soubor uložit, musí mít účet, pod kterým je spuštěn fond aplikací **správy**, oprávnění pro sdílenou složku.

Podrobný postup při zavedení důvěryhodných domén publikování naleznete v tomto tématu později v části [Přidání důvěryhodné domény publikování](https://technet.microsoft.com/731416d8-ddf4-4d4a-9f1a-bbd1ea48fe3c).

Pokud je soukromý klíč uložen v hardwarovém modulu zabezpečení, je třeba tento klíč přenést do hardwarového modulu zabezpečení na důvěryhodném serveru podle postupu popsaného v dokumentaci k hardwarovému modulu zabezpečení. V závislosti na typu hardwarových modulů zabezpečení na jednotlivých serverech a konfiguraci zařízení těchto modulů může být přenos soukromého klíče z jednoho modulu na druhý znemožněn. V dokumentaci k hardwarovému modulu zabezpečení vyhledejte, zda je možné přenést soukromý klíč bez ztráty dat uložených v cílovém hardwarovém modulu. Pokud soukromý klíč nelze úspěšně přenést, nelze mezi danými dvěma servery vytvořit důvěryhodnou doménu publikování.

> [!NOTE]
> Jestliže k ochraně soukromého klíče služby RMS používáte hardwarový modul zabezpečení a importujete certifikát serveru pro poskytování licencí z instalace služby RMS používající softwarovou ochranu klíče, je třeba před importem certifikátu určit heslo soukromého klíče na stránce Nastavení zabezpečení každého serveru RMS v clusteru. 
