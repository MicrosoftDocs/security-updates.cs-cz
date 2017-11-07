---
TOCTitle: Distribuce klienta RMS
Title: Distribuce klienta RMS
ms:assetid: '4b8dd930-4105-4e73-918c-12d2b05d5fb5'
ms:contentKeyID: 18113267
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc720266(v=WS.10)'
---

Distribuce klienta RMS
======================

Klient RMS je integrován do operačního systému Windows Vista® tak, aby již nevyžadoval samostatnou instalaci. Operační systémy předcházející systému Windows Vista vyžadují instalaci softwaru klienta RMS a jeho následnou aktivaci.

Proces aktivace vytvoří bezpečnostní modul a certifikát počítače pro aktuálně přihlášeného uživatele. Aktivace je místní proces, u kterého není nutné připojení k síti. Po úspěšné aktivaci získá aplikace s podporou služby RMS při první žádosti o licenci na používání certifikát uživatele. Klienta RMS lze nainstalovat do všech klientských počítačů v organizaci pomocí zásad skupiny, služby Windows Update nebo pomocí skriptu pro správu.

| ![](images/Cc720266.note(WS.10).gif)Poznámka                                                                                                                                                                                                                                             |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Bez ohledu na použitý způsob distribuce klienta komunikuje klient RMS se serverem RMS ve výchozím nastavení buď prostřednictvím portu 80, nebo portu 443. Měli byste se přesvědčit, zda klientský počítač dokáže na těchto portech vytvářet odchozí požadavky na kořenové nebo pouze licencované clustery služby RMS. |

**Používání zásad skupiny**

Pokud se software v organizaci distribuuje pomocí zásad skupiny, můžete tento způsob použít také k distribuci klienta RMS pomocí zvýšených oprávnění. Jestliže je klient RMS distribuován tímto způsobem, nepotřebuje uživatel oprávnění správce a může klienta RMS instalovat buď pomocí panelu **Přidat nebo odebrat programy** ve složce **Ovládací panely**, nebo otevřením obsahu chráněného právy v aplikaci s podporou služby RMS.

**Použití služby Windows Update**

Služba Windows Update představuje nejjednodušší způsob instalace klienta RMS do počítače. Výhoda této metody spočívá v používání uživatelům známého mechanismu, ale vyžaduje, aby měl uživatel instalující klienta RMS v počítači místní oprávnění správce.

**Instalace pomocí skriptů**

Chcete-li si nad procesem instalace klienta zajistit maximální kontrolu, můžete software získat a ověřit jeho integritu v každém kroku procesu instalace spuštěním skriptu. Tento skript může být zapsán a přidán do objektu GPO (Group Policy Object) jako spouštěcí skript. U této metody nemusí být uživatel místním správcem v počítači a klient RMS bude automaticky nainstalován při spuštění.

        ```
Základní informace o distribuci klienta RMS pomocí zásad skupiny získáte v části [Nastavení serveru SMS nebo zásad skupiny na podporu nasazení klientů](https://technet.microsoft.com/9e37c27b-8cc1-40c6-adb7-0937aa64c8db) dále v tomto tématu.

Pokyny pro nasazení klienta RMS získáte v části [Způsob nasazení klienta RMS](https://technet.microsoft.com/c84f1724-cf71-4385-9003-ff68bc23c927) dále v tomto tématu.
