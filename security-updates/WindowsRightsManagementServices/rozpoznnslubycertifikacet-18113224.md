---
TOCTitle: Rozpoznání služby certifikace účtů
Title: Rozpoznání služby certifikace účtů
ms:assetid: '293a2f91-4712-45ec-8b74-7533f4144cbd'
ms:contentKeyID: 18113224
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc720224(v=WS.10)'
---

Rozpoznání služby certifikace účtů
==================================

Služba certifikace účtů RMS uděluje certifikáty účtů práv uživatelům. Každý certifikát účtů práv platí pouze pro konkrétní počítač nebo zařízení a vyžaduje, aby uživatel, který jej požaduje, měl k dispozici platný certifikát počítače.

Služba certifikace účtů může být spuštěna pouze na serveru kořenové certifikace nebo v clusteru kořenové certifikace. Pokud chce klient vytvořit požadavek na certifikaci účtu, načte nejprve z adresáře služby Active Directory adresu URL virtuálního adresáře Certification serveru kořenové certifikace, kde je služba certifikace účtů umístěna. Poté připojí cestu ke službě certifikace účtů.

Adresa URL adresáře Certification serveru kořenové certifikace je v adresáři služby Active Directory uložena například v následujícím tvaru:

http://*název\_serveru*/\_wmcs/Certification

V případě, že klient požádá o certifikát účtu práv, připojí k adrese URL název souboru služby certifikace účtů:

http://*název\_serveru*/\_wmcs/Certification/Certification.asmx

| ![](images/Cc720224.note(WS.10).gif)Poznámka                                   |
|-------------------------------------------------------------------------------------------------------------|
| Jestliže jste na serveru povolili protokol SSL, budou tyto adresy URL používat protokol připojení https://. |
