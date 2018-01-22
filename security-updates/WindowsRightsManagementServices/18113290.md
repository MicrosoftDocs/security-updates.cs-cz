---
TOCTitle: Změna hesla účtu služby RMS
Title: Změna hesla účtu služby RMS
ms:assetid: '435c9cef-b622-48b3-9d4d-4bf5cac7d52d'
ms:contentKeyID: 18113290
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc720273(v=WS.10)'
---

Změna hesla účtu služby RMS
===========================

Na základě zásad hesla určených pro servery RMS je možné, že heslu účtu služby RMS pravidelně vyprší doba platnosti. V případě, že je heslo neplatné, přestane služba RMS pracovat. Heslo proto musí být změněno před vypršením jeho doby platnosti.

**Použití jednoho účtu služby RMS**

Používáte-li jeden účet služby RMS, můžete změnit heslo na každém serveru této služby následujícím postupem:

1.  Pokud je server v clusteru, vyjměte jej z pořadí střídání.
2.  Přihlaste se na server pomocí přístupových pověření účtu služby RMS.
3.  Změňte heslo účtu služby RMS.
    Na ostatních serverech používajících stejný účet služby RMS přestane služba pracovat, protože pověření uložená na těchto serverech nebudou po změně hesla platná.
4.  Odhlaste se ze serveru.
5.  Znovu se na server přihlaste pomocí pověření správce služby RMS.
6.  Chcete-li provést opětovnou konfiguraci identity uživatele na serveru, klepněte na stránce **Globální správa** na možnost **Změnit účet služby RMS**, a pak na stránce **Změnit účet služby RMS** určete doménu, jméno uživatele a heslo.
7.  Zastavte a znovu spusťte službu IIS.
8.  Vraťte server zpět do pořadí střídání, pokud byl z něj vyjmut.
9.  Kroky 6 až 8 zopakujte pro všechny servery v clusteru.

Tento způsob změny hesla účtu služby RMS je nejjednodušší, může však po určitou dobu způsobit výpadek služby RMS, protože při změně hesla účtu služby RMS na serveru je služba Active Directory aktualizována novým heslem. Služba IIS pravidelně restartuje fondy aplikací a fondy spouštěné pomocí starých pověření bude možné spustit až po změně hesla účtu služby RMS a restartování služby IIS na daném serveru. Služba RMS může pracovat až po opakovaném spuštění fondů aplikací.

**Použití dvou účtů služby RMS**

V případě této metody je nejprve třeba vytvořit dva účty služby RMS s různými zásadami nebo daty konce platnosti. Při běžném provozu je služba RMS spuštěna pod prvním účtem. V případě, kdy je třeba změnit heslo účtu služby pro první účet, proveďte na každém serveru služby RMS následující kroky:

1.  Pokud je server v clusteru, vyjměte jej z pořadí střídání.
2.  Určete druhý účet služby RMS jako účet, pod nímž je spuštěna služba RMS. Další informace týkající se změny účtu naleznete v tomto tématu později v části [Změna účtu služby RMS](https://technet.microsoft.com/f257d66d-b823-41e4-bcb7-7c90eb295238).
3.  Zastavte a znovu spusťte službu IIS.
4.  Vraťte server zpět do pořadí střídání, pokud byl z něj vyjmut.

Jakmile budou všechny servery RMS používat druhý účet služby RMS, můžete změnit heslo u prvního účtu služby RMS, aniž by to mělo vliv na provoz systému RMS. Tímto způsobem můžete střídavě používat oba účty a vyhnout se výpadkům služby RMS.
