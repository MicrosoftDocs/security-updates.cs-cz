---
TOCTitle: Přemisťování uživatelských účtů mezi doménami
Title: Přemisťování uživatelských účtů mezi doménami
ms:assetid: '0010b0ea-07c0-41c9-81f7-5881343d1d55'
ms:contentKeyID: 18113194
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc720179(v=WS.10)'
---

Přemisťování uživatelských účtů mezi doménami
=============================================

Po instalaci a zajištění serveru kořenové certifikace v organizaci je tento server ve službě Active Directory v nastavení doménové struktury zaregistrován jako zprostředkovatel služby RMS. Pro jednu doménovou strukturu služby Active Directory může existovat pouze jeden cluster kořenové certifikace.

Při přemístění uživatelského účtu z jedné domény do jiné v rámci stejné doménové struktury je pro uživatelský účet v nové doméně vytvořen nový identifikátor SID. Pokud se pak uživatel pokusí ze serveru získat nový certifikát účtu práv, bude jej server vzhledem k novému identifikátoru SID pokládat za nového uživatele. Server pro uživatele vygeneruje nové klíče a pomocí původní e-mailové adresy uživatele vydá nový certifikát účtu práv. Pokud uživatel použije nový certifikát účtu práv pro existující licenci, nebudou si identifikátor SID a klíč navzájem odpovídat a uživatel bude muset získat novou licenci. Stejný princip platí i v případě přemístění uživatelského účtu do domény v jiné doménové struktuře.
