---
TOCTitle: Povolení certifikace serverových služeb
Title: Povolení certifikace serverových služeb
ms:assetid: '0ed78c85-7acb-4e3b-a594-613f8ccb5b14'
ms:contentKeyID: 18113212
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc720196(v=WS.10)'
---

Povolení certifikace serverových služeb
=======================================

Provedení tohoto postupu vyžaduje, aby byl uživatel místně přihlášen k webu pro správu v rámci doménového uživatelského účtu, který je členem skupiny Administrators. Z hlediska zabezpečení je nejvhodnější při provádění tohoto postupu použít příkaz **Spustit jako**.

Tento postup lze použít pouze na kořenovém clusteru.

Při provádění uvedeného postupu se předpokládá, že byla vytvořena skupina uživatelů obsahující uživatelské účty, které budou služby serveru zosobňovat při používání obsahu chráněného právy.

Povolení certifikace serverových služeb
---------------------------------------

#### Povolení certifikace serverových služeb

1.  Přihlaste se k počítači jako člen místní skupiny Administrators.

2.  Spusťte prohlížeč systému souborů a přejděte do složky &lt;systémová\_jednotka&gt;:\\Inetpub\\wwwroot\\\_wmcs\\Certification.

3.  Chcete-li u služeb serveru povolit příjem certifikátů účtů práv, klepněte pravým tlačítkem myši na soubor ServerCertification.asmx a klepněte na příkaz **Vlastnosti**.

4.  Na kartě **Zabezpečení** klepněte na možnost **Přidat** a přidejte skupinu vytvořenou pro tuto kategorii uživatelů a skupinu **RMS Service Group**.

5.  V seznamech **Oprávnění** pro dané skupiny zaškrtněte políčko **Povolit** pro oprávnění ke **čtení & spouštění** a klepněte na tlačítko **OK**.

6.  Kroky 1-4 je třeba provést u každého serveru v clusteru.

| ![](images/Cc720196.note(WS.10).gif)Poznámka                                                                                                                                                                                                                                                                                                                                                                                                                          |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| U serveru Microsoft Exchange Server 2007 je třeba přidat každý objekt počítače služby Active Directory serveru předmostí do volitelného seznamu řízení přístupu (DACL) souboru ServerCertification.asmx. Podobně je u serveru Microsoft Office SharePoint Server 2007 nutné do tohoto seznamu DACL přidat objekt počítače služby Active Directory serveru Office SharePoint Server 2007. Doporučujeme přidat do tohoto seznamu DACL skupinu zabezpečení a přidat do ní příslušné objekty počítačů. |
