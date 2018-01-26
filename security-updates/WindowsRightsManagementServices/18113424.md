---
TOCTitle: Nastavení důvěryhodnosti certifikátů účtů práv založených na službě Passport
Title: Nastavení důvěryhodnosti certifikátů účtů práv založených na službě Passport
ms:assetid: 'c096fa36-c40d-4b28-843c-e9cbbe8eef70'
ms:contentKeyID: 18113424
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747655(v=WS.10)'
---

Nastavení důvěryhodnosti certifikátů účtů práv založených na službě Passport
============================================================================

Společnost Microsoft poskytuje službu certifikace účtů, která používá pověření služby Microsoft .NET Passport k vytvoření certifikátu účtu práv pro uživatele. Pokud chcete umožnit uživatelům s certifikáty účtů práv od této služby získávat licence na používání z clusteru RMS, je třeba nastavit důvěryhodnou uživatelskou doménu, která bude přijímat pověření uživatelů ze služby certifikace účtů společnosti Microsoft.

Tato funkce vyžaduje, aby byl vhodnou konfigurací Internetové informační služby povolen anonymní přístup ke službě správy licenci RMS. Tento krok je nezbytný pro externí uživatele, neboť služba správy licencí ve výchozím nastavení používá Integrované ověřování systému Windows. Jestliže anonymní přístup není nastaven, nebudou moci externí uživatelé s certifikáty účtů práv služby Passport získávat licence.

Nastavení důvěryhodnosti certifikátů účtů práv služby Passport
--------------------------------------------------------------

#### Povolení anonymního přístupu ke službě správy licencí RMS

1.  Otevřete modul snap-in **Správce internetové informační služby** a rozbalte server, který je hostitelem služby RMS.

2.  Ve stromu konzoly rozbalte položku **Weby** a rozbalte web, na kterém jste konfigurovali službu RMS. Ve výchozím nastavení je to **Výchozí web**.

3.  Ve stromu konzoly rozbalte web **\_wmcs** a vyberte virtuální adresář **správy licencí**.

4.  Pravým tlačítkem myši klepněte na virtuální adresář **správy licencí** a klepněte na příkaz **Vlastnosti**.

5.  V dialogovém okně **Vlastnosti správy licencí** klepněte na kartu **Zabezpečení adresářů**.

6.  Klepněte na položku **Úpravy** v oblasti **Ověřování a řízení přístupu**.

7.  Zaškrtněte políčko **Povolit anonymní přístup**.

#### Nastavení důvěryhodnosti certifikátů účtů práv založených na službě Passport

1.  Otevřete stránku **Globální správa** a klepněte na položku **Spravovat službu RMS na tomto webu** u webu, na kterém chcete nastavit důvěryhodnost certifikátů účtů práv služby Passport.

2.  V části **Odkazy správy** klepněte na odkaz **Zásady důvěryhodnosti**.

3.  V části **Důvěryhodné domény uživatelů** klepněte na položku **Důvěřovat certifikátům RAC služby Passport**. V seznamu **Důvěryhodné domény uživatelů** se objeví položka Microsoft RM Certification Service.

4.  Nepovinně lze vyloučit uživatele na základě e-mailových adres. Chcete-li to provést, klepněte na položku **Vyloučené identity** a zadejte e-mailovou adresu uživatele, kterému nedůvěřujete.
