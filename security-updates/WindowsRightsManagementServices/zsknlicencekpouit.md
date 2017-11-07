---
TOCTitle: Získání licence k použití
Title: Získání licence k použití
ms:assetid: '0b6cde34-418a-4dee-9d27-b65b93b535ac'
ms:contentKeyID: 18113210
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc720194(v=WS.10)'
---

Získání licence k použití
=========================

Jestliže chce uživatel používat obsah chráněný službou RMS, musí od služby správy licencí RMS získat licenci k použití. Proces odeslání požadavku na licenci k použití a následného získání licence je znázorněn na následujícím obrázku.

![](images/Cc720194.37b8d28c-9749-4e81-bc6a-22692fefb8b6(WS.10).gif)

Proces získání licence k použití zahrnuje následující kroky:

1.  Uživatel obdrží chráněný soubor obvyklým distribučním kanálem a otevře jej v aplikaci s podporou služby RMS. Jestliže v aktuálním počítači nebo zařízení uživatele není k dispozici certifikát účtu práv, je nutné, aby jej uživatel získal.
2.  Aplikace s podporou služby RMS odešle požadavek na licenci k použití na server, který pro daný chráněný obsah vydal licenci k publikování. Požadavek obsahuje certifikát účtu práv daného uživatele (zahrnující veřejný klíč uživatele) a licenci k publikování (zahrnující symetrický klíč obsahu).
    Licence k publikování vydaná pomocí certifikátu poskytovatele licence klienta obsahuje adresu URL serveru, který vydal certifikát. V daném příkladu je požadavek na licenci k použití odeslána na server, který vydal klientský certifikát pro poskytování licencí, a nikoli do počítače, který vydal licenci k publikování.
3.  Server správy licencí zkontroluje ověření uživatele, dále zkontroluje, zda je uživatel uveden v licenci k publikování, a poté vytvoří licenci k použití. Server ověří certifikát účtu uživatele a poté určí, která oprávnění byla uživateli udělena, ať už přímo či nepřímo prostřednictvím členství ve skupině s udělenými oprávněními.
    Server dešifruje symetrický klíč obsahu s použitím soukromého klíče serveru, znovu jej zašifruje s použitím veřejného klíče příjemce a přidá jej do licence k použití. V tomto kroku je zajištěno, že klíč obsahu může dešifrovat a přístup k chráněnému obsahu může získat pouze oprávněný uživatel.
    Server přidá do licence k použití všechny relevantní podmínky, jako například vyloučení některé verze systému Windows nebo aplikace. Uvedené podmínky jsou vynuceny klientem v době, kdy je licence k použití svázána s obsahem chráněným službou RMS.
4.  Pokud je ověření úplné, server správy licencí navrátí licenci k použití klientskému počítači uživatele.
