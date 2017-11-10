---
TOCTitle: 'Nejčastější dotazy týkající se služby RMS: Správa'
Title: 'Nejčastější dotazy týkající se služby RMS: Správa'
ms:assetid: '43f77336-5e62-4405-9efb-55417a402d62'
ms:contentKeyID: 18113291
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747547(v=WS.10)'
---

Nejčastější dotazy týkající se služby RMS: Správa
=================================================

Nejčastější dotazy týkající se správy služby RMS
------------------------------------------------

-   [Jaký je nejvhodnější způsob odvolání oprávnění k dokumentům udělených uživateli, který s organizací ukončil pracovní poměr?](#bkmk_1)
-   [V případě vytváření vztahů důvěryhodnosti mezi dvěma organizacemi za účelem vzájemné výměny obsahu chráněného službou RMS vyžaduje certifikát licence XrML předávaný důvěřující společnosti zvláštní zpracování?](#bkmk_2)
-   [Jak služba RMS spolupracuje s cestovními profily uživatelů?](#bkmk_3)
-   [Proč by mohla organizace chtít vyřadit službu RMS z provozu?](#bkmk_4)
-   [Jak probíhá celý proces vyřazení z provozu?](#bkmk_5)
-   [Je možné vyřadit server RMS z provozu tak, aby mohli obnovit dokumenty pouze někteří uživatelé?](#bkmk_6)
-   [Co znamená chybová zpráva s upozorněním, že server nemá přístup k adresáři aplikací?](#bkmk_7)
-   [Lze na serveru RMS používat trasování?](#bkmk_8)
-   [Co je posunutí hodin a jak je vyřešit?](#bkmk_9)

<span id="BKMK_1"></span>
#### Jaký je nejvhodnější způsob odvolání oprávnění k dokumentům udělených uživateli, který s organizací ukončil pracovní poměr?

Obecně je vhodnější udělovat licence na dokumenty skupinám uživatelů definovaným ve službě Active Directory, spíše než jednotlivým uživatelským účtům. Tento postup se doporučuje, protože v případě, že uživatel ukončí pracovní poměr s organizací, můžete jej odebrat ze skupiny služby Active Directory, takže nemůže číst dokumenty odeslané této skupině. Daný uživatel však i nadále může číst dokumenty spojené s existujícími licencemi k použití, pokud však u těchto dokumentů nejsou nastavena práva vyžadující získání licence k použití při každém otevření dokumentu. Jestliže takové právo definováno není, představuje jediný způsob, kterým můžete uživateli otevření dokumentů spojených s existující licencí k použití znemožnit, odstranění licencí z úložiště v počítači uživatele.

<span id="BKMK_2"></span>
#### V případě vytváření vztahů důvěryhodnosti mezi dvěma organizacemi za účelem vzájemné výměny obsahu chráněného službou RMS vyžaduje certifikát licence XrML předávaný důvěřující společnosti zvláštní zpracování?

Pokud vytváříte důvěryhodnou doménu uživatelů nebo důvěryhodnou doménu publikování, nastavujete důvěryhodnost pro partnerskou organizaci, se kterou budete spolupracovat v rámci systému správy přístupových práv. Při tomto kroku podstupujete určité riziko, že důvěřování druhé organizaci ohrozí zabezpečení vašich informací. Doporučeným postupem je požádat partnerskou organizaci o odeslání jejího certifikátu serveru pro poskytování licencí služby RMS prostřednictvím ověřeného kanálu, jako je například e-mail S/MIME, a omezit tak riziko, že bude tento certifikát zfalšován ještě před importem na váš server RMS.

<span id="BKMK_3"></span>
#### Jak služba RMS spolupracuje s cestovními profily uživatelů?

Certifikáty účtu práv, pomocí nichž lze identifikovat uživatele, jsou udělovány pro určitý počítač. V případě použití cestovních profilů bude při prvním využití služby RMS v daném počítači vytvořen nový certifikát účtu práv pro uživatele tohoto počítače.

<span id="BKMK_4"></span>
#### Proč by mohla organizace chtít vyřadit službu RMS z provozu?

Vyřazením služby RMS z provozu bude odebrán server RMS z příslušné infrastruktury, což uživatelům umožní uložit obsah chráněný právy bez ochrany. Existují tři hlavní důvody, proč organizace chtějí k tomuto kroku přistoupit:

-   zjednodušení architektury, jako například konsolidace serverů do clusteru,
-   migrace zkušebního pilotního prostředí do provozního prostředí,
-   sloučení serverů RMS, například po akvizici.

<span id="BKMK_5"></span>
#### Jak probíhá celý proces vyřazení z provozu?

Proces vyřazení z provozu začíná u kořenového clusteru služby RMS povolením služby vyřazení z provozu. Jakmile je tato služba povolena, jsou zakázány všechny ostatní služby (například správa licencí a certifikace). Dále je nutné přesměrovat aplikaci s podporou služby RMS každého uživatele na připojení ke službě vyřazení z provozu v případě, že je použita funkce služby RMS. Příkladem takové aplikace je sada Microsoft Office 2003. V sadě Office 2003 je klient RMS směrován na služby RMS pomocí klíčů registru. Jeden specifický klíč registru je určen také pro službu vyřazení z provozu. V případě nastavení uvedeného klíče tak, aby byl klient směrován na službu vyřazení z provozu, udělí cluster služby RMS uživateli tohoto obsahu licence k použití s úplným oprávněním (čtení, zápis, kopírování, tisk, úpravy atd.) bez ohledu na to, zda byla taková oprávnění uživateli původně udělena. Uživatelé by pak měli odebrat veškerou ochranu právy ze všech dokumentů, které chtějí zachovat i po úplném vyřazení clusteru služby RMS z provozu. Jakmile k tomu dojde, může být provoz clusteru služby RMS zcela ukončen.

Je vhodné zálohovat konfigurační databázi daného clusteru služby RMS pro případ, že po jeho vyřazení budete potřebovat některý dokument chráněný právy obnovit. Po odebrání serveru bude moci otevřít obsah chráněný právy bez privátního klíče kořenového clusteru služby RMS pouze autor dokumentu.

<span id="BKMK_6"></span>
#### Je možné vyřadit server RMS z provozu tak, aby mohli obnovit dokumenty pouze někteří uživatelé?

U webové služby vyřazení z provozu (decommission.asmx) můžete nastavit seznam řízení přístupu (ACL) a řídit tak přístup k této službě, takže dešifrovací klíč k obsahu chráněnému právy mohou získat pouze někteří uživatelé.

<span id="BKMK_7"></span>
#### Co znamená chybová zpráva s upozorněním, že server nemá přístup k adresáři aplikací?

Tato chyba se někdy zobrazí, jestliže poprvé po instalaci služby RMS otevřete web správy této služby. Po jejím zobrazení není možné službu RMS konfigurovat ani spravovat.

K této chybě obvykle dochází, pokud je Internetová informační služba (IIS) spuštěna v izolovaném režimu služby IIS 5.0. Pomocí následujícího postupu je možné uvedené nastavení na serveru zakázat. Potom službu IIS restartujte a problém bude odstraněn.

**Zakázání izolovaného režimu služby IIS 5.0**
1.  Přihlaste se k serveru RMS jako člen místní skupiny Administrators.

2.  Klepněte na tlačítko **Start**, přejděte na položku **Nástroje pro správu** a poté klepněte na položku **Správce Internetové informační služby**.

3.  Ve **Správci služby IIS** rozbalte složku s místním počítačem, klepněte pravým tlačítkem na položku **Webové servery** a klepněte na příkaz **Vlastnosti**.

4.  Klepněte na kartu **Služba**, zrušte zaškrtnutí políčka **Spustit webovou službu v izolovaném režimu služby IIS 5.0** a klepněte na tlačítko **OK**.

5.  Tato změna vyžaduje restartování služby IIS. Po zobrazení výzvy k restartování služby IIS klepněte na tlačítko **Ano**.

<span id="BKMK_8"></span>
#### Lze na serveru RMS používat trasování?

Vzhledem k tomu že Služba správy přístupových práv byla vytvořena pomocí rozhraní Microsoft® .NET Framework, můžete trasování povolit a usnadnit tak sledování systémových událostí a řešení problémů.

Trasování je možné implementovat, jestliže změníte soubor Web.config nebo Machine.config. Pokud trasování implementujete v souboru Machine.config, spustí se u každé softwarové součásti v počítači. Jestliže však trasování implementujete v souboru Web.config, budou trasovány pouze události u webových služeb.

**Povolení trasování**
1.  Otevřete soubor Machine.config nebo Web.config a přidejte do něj v části &lt;system.diagnostics&gt; následující řádky:
    ```
    <system.diagnostics>
    <switches>
    <add name="Microsoft Windows Rights Management Services-Global" value="4" />
    <add name="Microsoft Windows Rights Management Services-TimeStamps" value="1" /> 
    <add name="Microsoft Windows Rights Management Services-Indents" value="0" /> 
    </switches>
    <trace autoflush="false" indentsize="4"/>
    </system.diagnostics>
    ```
2.  Restartujte službu IIS spuštěním příkazu IISRESET na příkazovém řádku.

3.  Po shromáždění potřebných dat odeberte z příslušného souboru .config řádky, které jste do něj přidali v kroku 1.

4.  Restartujte službu IIS spuštěním příkazu IISRESET na příkazovém řádku.

> [!IMPORTANT]
> Pokud na serveru RMS nastavíte trasování, může dojít k problémům s výkonem, jako jsou například delší prodlevy při získávání licencí k použití nebo při vydávání certifikátů účtů práv. Používejte trasování pouze výjimečně, a to pouze ke zjištění a odstranění existujících problémů. 

<span id="BKMK_9"></span>
#### Co je posunutí hodin a jak je vyřešit?

Posunutí hodin je případ, kdy se čas hodin v jednom počítači liší od času hodin v jiném počítači. Tato situace je zcela běžná, stejně jako situace, kdy se mírně rozcházejí náramkové hodinky dvou osob v místnosti. Posunutí hodin může způsobovat potíže při zadávání doby platnosti licencí.

Doba platnosti je v licenci nastavena podle hodin jejího vydavatele. Posunutí hodin u těchto časů může způsobit potíže ve dvou bodech cyklu publikování a využití obsahu:

-   Aplikace chce získat licenci k použití na základě licence k publikování, jejíž doba platnosti podle hodin serveru RMS skončila v minulosti nebo začíná v budoucnosti. V takovém případě se požadavek nezdaří. Může k tomu dojít u koncového uživatele požadujícího licenci k použití nebo u aplikace, která chce získat předběžnou licenci na dokument (za účelem získání licence k použití jménem uživatele).
-   Pokud platnost licence skončila (nebo dosud nezačala), nezdaří se použití této licence. V opačném případě nebudou k dispozici pouze práva, jejichž platnost vypršela (nebo dosud nezačala).

Jestliže jsou například hodiny publikujícího počítače o 15 minut pozadu za hodinami počítače, ve kterém má být obsah využit, a vydavatel vytvoří licenci k publikování, v níž je uvedeno, že platnost obsahu vyprší za 15 minut, získá uživatel, který chce obsah využít, ze serveru nepoužitelnou licenci k použití, protože platnost práv k zobrazení obsahu udělených licencí k použití již vypršela.

Potíže s posunutím hodin nelze jednoduše vyřešit. Vhodným řešením je nastavit počáteční čas platnosti práva na čas předcházející aktuálnímu času v počítačích uživatelů s hodinami jdoucími pozadu a (pokud je to možné) rozšířit dobu platnosti licence u uživatelů s hodinami jdoucími popředu. Je vhodné brát potíže s posunutím hodin v úvahu, zvláště při vytváření licencí s krátkodobou platností.
