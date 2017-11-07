---
TOCTitle: 'Nejčastější dotazy týkající se služby RMS: Certifikáty, klíče a šifrování'
Title: 'Nejčastější dotazy týkající se služby RMS: Certifikáty, klíče a šifrování'
ms:assetid: 'ad8cc088-1dea-44c2-be68-9091129f0f12'
ms:contentKeyID: 18113465
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747725(v=WS.10)'
---

Nejčastější dotazy týkající se služby RMS: Certifikáty, klíče a šifrování
=========================================================================

Nejčastější dotazy týkající se certifikátů, klíčů a šifrování služby RMS
------------------------------------------------------------------------

-   [Jaké algoritmy šifrování služba RMS používá?](#bkmk_10)
-   [Používá služba RMS certifikované šifrování FIPS?](#bkmk_11)
-   [Jsou licence k použití spojené s licencemi k publikování nebo šablonami, které neudělují oprávnění jednotlivým uživatelům, ale distribučním seznamům, zpracovány jiným způsobem, aby bylo zajištěno dynamické vyhodnocení členů?](#bkmk_12)
-   [Pokud je služba RMS použita z veřejného terminálu, je vydán dočasný certifikát účtu práv. Jak se liší dočasný certifikát účtu práv od standardního certifikátu účtu práv? Jak služba RMS zjistí, že je používána z veřejného terminálu?](#bkmk_13)
-   [Kdy se používá dočasný certifikát účtu práv?](#bkmk_14)
-   [Vydává služba RMS certifikáty X.509v3?](#bkmk_15)
-   [Kde jsou uloženy certifikáty XrML?](#bkmk_16)
-   [Kde je uložen pár privátního a veřejného klíče počítače?](#bkmk_17)
-   [Kde je uložen pár privátního a veřejného klíče klienta?](#bkmk_18)
-   [Algoritmus AES je symetrický. Jak je zajištěno zabezpečení při předávání klíče mezi serverem a uživatelem?](#bkmk_19)

<span id="BKMK_10"></span>
#### Jaké algoritmy šifrování služba RMS používá?

Služba RMS používá 2048bitové klíče RSA u serverů RMS a 1024bitové klíče RSA u páru klíčů uživatele a počítače.

<span id="BKMK_11"></span>
#### Používá služba RMS certifikované šifrování FIPS?

U služby RMS s aktualizací Service Pack 1 a vyšší používají bezpečnostní moduly generované klientskou aplikací služby RMS certifikované šifrování AES standardu FIPS. To platí, pokud je klient nainstalován v počítači se systémem Windows XP nebo Windows Server 2003. Jestliže je však klient RMS nainstalován v počítačích se systémem Windows 2000, není knihovna pro certifikované šifrování AES standardu FIPS nainstalována, takže bezpečnostní moduly nejsou s tímto standardem kompatibilní.

<span id="BKMK_12"></span>
#### Jsou licence k použití spojené s licencemi k publikování nebo šablonami, které neudělují oprávnění jednotlivým uživatelům, ale distribučním seznamům, zpracovány jiným způsobem, aby bylo zajištěno dynamické vyhodnocení členů?

Licence k použití se vždy vydávají jednotlivým uživatelům. Jestliže je v licenci k publikování nebo šabloně uvedena skupina, vyhodnotí služba RMS členství ve skupinách v okamžiku vydání licence k použití. Pokud je uživatel požadující licenci členem uvedené skupiny, je licence k použití vydána pro identitu daného uživatele.

<span id="BKMK_13"></span>
#### Pokud je služba RMS použita z veřejného terminálu, je vydán dočasný certifikát účtu práv. Jak se liší dočasný certifikát účtu práv od standardního certifikátu účtu práv? Jak služba RMS zjistí, že je používána z veřejného terminálu?

Aplikace s podporou služby RMS musí určit, zda by měl klient RMS požadovat pro uživatele dočasný nebo standardní certifikát účtu práv. Pro tuto situaci není k dispozici žádný způsob detekce. Příkladem aplikace s podporou služby RMS, která uživateli umožňuje vybrat odpovídající certifikát účtu práv, je sada Microsoft Office 2003.

Hlavní rozdíl mezi dočasným a standardním certifikátem účtu práv je zahrnutí identifikátoru zabezpečení uživatele a rozsah doby platnosti. Dočasný certifikát účtu práv neobsahuje identifikátor zabezpečení (SID) uživatele a jeho doba platnosti je určena počtem minut. Výchozí doba platnosti tohoto certifikátu je 15 minut. Standardní certifikát účtu práv identifikátor zabezpečení uživatele naopak obsahuje a jeho doba platnosti je určena počtem dnů. Výchozí doba platnosti tohoto certifikátu je 365 dnů.

<span id="BKMK_14"></span>
#### Kdy se používá dočasný certifikát účtu práv?

Dočasný certifikát účtu práv umožňuje uživatelům využívat obsah chráněný službou RMS v počítačích, které splňují kterékoli z následujících kritérií:

-   Počítač není členem stejné doménové struktury jako instalace služby RMS, ze které byl certifikát účtu práv získán.
-   Počítač není členem stejné doménové struktury, v níž je umístěn příslušný uživatelský účet.
-   Uživatel předpokládá, že později nebude pracovat se stejným počítačem.

Příklady počítačů, které uvedená kritéria splňují, můžete najít na letištích, ve veřejných knihovnách nebo v internetových kavárnách.

<span id="BKMK_15"></span>
#### Vydává služba RMS certifikáty X.509v3?

Ne. Služba RMS vydává certifikáty XrML, které by měly reprezentovat vyjádření uživatelů a zásad mimo rozsah certifikátů X.509v3.

<span id="BKMK_16"></span>
#### Kde jsou uloženy certifikáty XrML?

Systém služby RMS používá následující certifikáty a licence, které jsou uloženy ve formátu XrML v klientském počítači.

-   Certifikát počítače
    Název souboru: CERT-Machine.drm
    Umístění: %USERPROFILE%\\Local Settings\\Data aplikací\\Microsoft\\DRM\\
-   Certifikát účtu práv
    Předpona názvu souboru: GIC
    Umístění: %USERPROFILE%\\Local Settings\\Data aplikací\\Microsoft\\DRM
-   Klientský certifikát pro poskytování licencí
    Předpona názvu souboru: CLC
    Umístění: %USERPROFILE%\\Local Settings\\Data aplikací\\Microsoft\\DRM
-   Licence k použití
    Předpona názvu souboru: EUL
    Umístění: %USERPROFILE%\\Local Settings\\Data aplikací\\Microsoft\\DRM

| ![](images/Cc747725.note(WS.10).gif)Poznámka                                                                                  |
|------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Uživatelskému účtu je přiřazen jeden certifikát počítače, soubor GIC a soubor CLC a mnoho souborů EUL na každou část obsahu, k němuž je požadován přístup. |

| ![](images/Cc747725.note(WS.10).gif)Poznámka                                                           |
|-------------------------------------------------------------------------------------------------------------------------------------|
| Pro klienta RMS integrovaného se systémem Windows Vista® platí následující umístění: %USERPROFILE%\\AppData\\Local\\Microsoft\\DRM. |

<span id="BKMK_17"></span>
#### Kde je uložen pár privátního a veřejného klíče počítače?

Privátní klíč počítače je uložen na zabezpečeném místě a je chráněn kryptografickými klíči spojenými s pověřeními pro přihlášení daného uživatele a s konfigurací počítače.

<span id="BKMK_18"></span>
#### Kde je uložen pár privátního a veřejného klíče klienta?

Pár klíčů pro uživatelský účet je uložen v certifikátu účtu práv.

<span id="BKMK_19"></span>
#### Algoritmus AES je symetrický. Jak je zajištěno zabezpečení při předávání klíče mezi serverem a uživatelem?

V systému se používají symetrické klíče i veřejné a privátní klíče. Obsah je šifrován symetrickým klíčem, ale další klíče v systému (klíče uživatele, počítače a serveru) představují veřejné a privátní klíče RSA. Symetrický klíč obsahu je vždy šifrován v různých licencích: buď na veřejný klíč RSA serveru RMS v licenci k publikování, nebo na veřejný klíč RSA uživatele v licenci k použití.
