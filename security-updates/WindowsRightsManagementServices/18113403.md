---
TOCTitle: Problémy se zajišťováním služby RMS
Title: Problémy se zajišťováním služby RMS
ms:assetid: 'b0e6ef48-ab38-4426-be5b-811cf64c45c0'
ms:contentKeyID: 18113403
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747638(v=WS.10)'
---

Problémy se zajišťováním služby RMS
===================================

Při zajišťování služby RMS jsou vytvořeny a nakonfigurovány soubory prostředků a připojení mezi různými součástmi, na kterých je služba RMS závislá. V případě chyby při nastavení prostředku službou RMS se zajišťování nezdaří a zobrazí se chybová zpráva. Tato část je věnována nejběžnějším příčinám uvedených chyb a měla by vám usnadnit řešení neočekávaných situací, které zajištění služby RMS znemožňují.

Nelze zajistit server kořenové certifikace
------------------------------------------

Může se stát, že nebudete moci zajistit server kořenové certifikace, protože se nezobrazí správné stránky pro zajišťování. K takovému chování může dojít, jestliže na stránce Globální správa klepnete na možnost Zajišťovat službu RMS na tomto webu, protože chcete zajistit první server kořenové certifikace. Namísto stránek pro zajišťování serveru kořenové certifikace se však zobrazí stránky pro zajišťování serveru správy licencí.

K uvedeným potížím dochází, pokud nezrušíte zajištění posledního serveru kořenové certifikace v dané doménové struktuře služby Active Directory ještě před tím, než z ní odinstalujete službu RMS, a potom znovu zajišťujete server kořenové certifikace. Pokud zrušíte zajištění jediného serveru kořenové certifikace v doménové struktuře služby Active Directory, odeberete ze služby Active Directory příslušný spojovací bod služby. Jestliže nezrušíte zajištění posledního serveru kořenové certifikace v dané doménové struktuře ještě před odinstalací služby RMS, nebudete moci server kořenové certifikace dané doménové struktury znovu zajistit, dokud ze služby Active Directory ručně neodeberete příslušný spojovací služby.

Pokud se při zajišťování prvního serveru kořenové certifikace doménové struktury služby Active Directory zobrazí stránky pro server správy licencí, odeberte provedením následujícího postupu příslušný spojovací bod služby ze služby Active Directory:

**Odebrání spojovacího bodu služby pro službu RMS**
1.  V případě potřeby nainstalujte nástroje odborné pomoci systému Windows Server:

    V systému Windows Server 2003 spusťte ze složky \\Support Tools na instalačním disku CD-ROM soubor Suptools.msi.

    V systému Windows 2000 Server spusťte ze složky \\Support Tools na instalačním disku CD soubor Setup.exe.

2.  Pomocí účtu, který je členem skupiny Domain Admins, se přihlaste k řadiči domény, do níž daný server kořenové certifikace náleží.

3.  Do příkazového řádku zadejte následující příkaz a stiskněte klávesu ENTER:

    **ldp**

4.  Klepněte na položku **Připojení** a poté na položku **Připojit**.

5.  Stiskněte klávesu ENTER. Nezadávejte žádné údaje.

6.  Klepněte na položku **Připojení** a poté na položku **Svázat**.

7.  Stiskněte klávesu ENTER. Nezadávejte žádné údaje.

8.  Klepněte na položku **Zobrazit** a poté na položku **Strom**.

9.  Stiskněte klávesu ENTER. Nezadávejte žádné údaje.

    V levém podokně se zobrazí text **dc=Doména,dc=com**.

10. Rozbalte položku **dc=Doména,dc=com**.

11. Rozbalte položku **Konfigurace**.

12. Rozbalte položku **Služby**.

13. Odstraňte položku **RightsManagementServices**.

-nebo-

1.  Stáhněte a nainstalujte sadu RMS Administration Toolkit. Můžete si ji stáhnout z [webu společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=33841).

2.  Otevřete příkazový řádek klepnutím na tlačítko **Start** a na příkaz **Spustit**. V dialogovém okně **Spustit** zadejte příkaz **cmd** a klepněte na tlačítko **OK**.

3.  Na příkazovém řádku zadejte následující příkaz:
    **ADSCPRegister.exeunregisterscp** &lt;*adresa\_URL\_pro\_zrušení\_registrace*&gt;
    
4.  Jako položku &lt;*adresa\_URL\_pro\_zrušení\_registrace*&gt; zadejte adresu URL příslušného spojovacího bodu služby RMS, například https://doména/\_wmcs/Certification.

Po provedení těchto kroků můžete zajistit server kořenové certifikace.

Nelze vytvořit kontext SSPI
---------------------------

Během zajišťování se může zobrazit chybová zpráva Nelze vytvořit kontext SSPI, jestliže účet služby RMS není ověřen při zápisu serveru kořenové certifikace ke službě Microsoft Enrollment Servicess.

Setkáte-li se s touto chybovou zprávou, zkontrolujte, zda je účet služby RMS platným účtem domény. Pokud se jedná o účet skupiny, ověřte, zda je členství ve skupině stále platné, zda je možný překlad všech uživatelských účtů dané skupiny v doméně a zda mají účty oprávnění k databázím SQL.
