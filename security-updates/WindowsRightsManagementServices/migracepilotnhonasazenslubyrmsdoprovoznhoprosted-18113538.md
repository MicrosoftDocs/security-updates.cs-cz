---
TOCTitle: Migrace pilotního nasazení služby RMS do provozního prostředí
Title: Migrace pilotního nasazení služby RMS do provozního prostředí
ms:assetid: 'ea151946-22fb-4cba-a3ef-fd7a4bf0d292'
ms:contentKeyID: 18113538
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747789(v=WS.10)'
---

Migrace pilotního nasazení služby RMS do provozního prostředí
=============================================================

Před implementací technologie služby RMS v celé organizaci chce řada organizací nejprve vyzkoušet pilotní nasazení této služby. Pilotní program má standardně omezený počet uživatelů a server je udržován místně vyhrazeným správcem, nikoli jako součást datového střediska udržovaného skupinou IT. Pokud organizace po dokončení pilotního projektu implementuje službu RMS v datovém středisku pro všechny klienty, budou nasazeny nové servery RMS za účelem podpory většího počtu možných uživatelů.

Obsah chráněný službou RMS je však svázán se serverem RMS, pomocí kterého byl tento obsah vytvořen. Proto je nutné v případě, že je server odebrán nebo nahrazen, podniknout kroky k tomu, aby byl obsah, který byl šifrován pomocí pilotních serverů RMS, dešifrován a licencován pomocí provozních serverů RMS.

Pokud jste nasadili službu RMS jako pilotní program a chcete server RMS přesunout do provozního prostředí své organizace a zároveň chcete zachovat integritu obsahu chráněného pomocí pilotního serveru RMS, měli byste vytvořit plán migrace, který vám zajistí bezproblémový přechod a umožní přejít zpět do pilotního programu v případě nutnosti obnovení dat.

Následující kroky jsou uvedeny jako příklad některých položek, které by měl váš plán migrace obsahovat. Nasazení ve vašem prostředí však může být spojeno s dalšími požadavky.

###  

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th>Server</th>
<th>Krok</th>
<th>Poznámky</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>Pilotní</p></td>
<td style="border:1px solid black;"><p>Zálohujte konfigurační databázi služby RMS.</p></td>
<td style="border:1px solid black;"><p>Tento krok vám umožní obnovit pilotní server v případě potřeby.</p>
<p>Konfigurační databáze obsahuje soukromý klíč služby RMS.</p>
<p>Zkontrolujte, zda máte k dispozici heslo soukromého klíče.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Pilotní</p></td>
<td style="border:1px solid black;"><p>Pokud jste pro ochranu soukromého klíče služby RMS použili hardwarový modul zabezpečení, zazálohujte konfiguraci hardwarového modulu zabezpečení podle pokynů výrobce modulu.</p></td>
<td style="border:1px solid black;"><p>Hardwarový modul zabezpečení budete obnovovat na novém serveru.</p>
<p>Přesvědčte se, zda máte k dispozici všechny nezbytné součásti pro instalaci a konfiguraci dostupného hardwarového modulu zabezpečení.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Pilotní</p></td>
<td style="border:1px solid black;"><p>Vyexportujte soubor s důvěryhodnou doménou publikování.</p></td>
<td style="border:1px solid black;"><p>Tento krok umožní jinému serveru RMS dešifrovat licence k publikování vytvořené tímto serverem a vydat licence k použití pro chráněný obsah.</p>
<p>Důvěryhodná doména publikování zahrnuje certifikát serveru pro poskytování licencí, soukromý klíč služby RMS a šablony zásad práv, které byly na tomto serveru vytvořeny.</p>
<p>Soubor s důvěryhodnou doménou publikování je soubor XML šifrovaný silným heslem, které určíte při vytváření souboru. Toto heslo je také nutné pro import souboru s důvěryhodnou doménou publikování.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Pilotní</p></td>
<td style="border:1px solid black;"><p>Vyexportujte důvěryhodnou doménu uživatelů.</p></td>
<td style="border:1px solid black;"><p>Tento krok umožní jinému serveru RMS udělovat licence k použití uživatelům, jejichž certifikáty účtů práv udělil pilotní server RMS.</p>
<p>Důvěryhodná doména uživatelů je vytvořena importem certifikátu serveru pro poskytování z tohoto serveru na druhý server RMS.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Provozní</p></td>
<td style="border:1px solid black;"><p>Připravte nový server tak, aby se stal serverem kořenové certifikace.</p></td>
<td style="border:1px solid black;"><p>Přesvědčte se, zda z něj lze získat přístup k databázovému serveru a zda jsou nainstalovány služby IIS a Řízení front zpráv.</p>
<p>Pokud je to možné, použijte pro tento server stejný název.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Provozní</p></td>
<td style="border:1px solid black;"><p>Jestliže používáte hardwarový modul zabezpečení, nainstalujte jej a obnovte jeho konfiguraci ze zálohy vytvořené na pilotním serveru.</p></td>
<td style="border:1px solid black;"><p>Vytvoří pověření požadovaná k dešifrování soukromého klíče služby RMS.</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Provozní</p></td>
<td style="border:1px solid black;"><p>Nainstalujte službu RMS.</p></td>
<td style="border:1px solid black;"><p>Služba RMS ověří, zda jsou nainstalovány a správně nakonfigurovány všechny požadované služby.</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Provozní</p></td>
<td style="border:1px solid black;"><p>Zajistěte službu RMS pomocí nového soukromého klíče. Pokud používáte zápis online, bude server zapsán během procesu zajišťování, a to připojením ke službě Microsoft Enrollment Services prostřednictvím Internetu. Jestliže na tomto serveru není připojení k Internetu k dispozici, je nutné použít zápis offline.</p></td>
<td style="border:1px solid black;"><p>Pokud se název serveru liší od názvu pilotního serveru, můžete v nastavení adresy URL clusteru nakonfigurovat stejnou adresu URL, jako má pilotní server.</p>
<p>Jestliže uvedený krok neprovedete, bude třeba nastavit přesměrování adresy URL z předchozí adresy URL clusteru na novou adresu URL clusteru, aby mohli uživatelé s již existujícím obsahem získat licence k použití.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Provozní</p></td>
<td style="border:1px solid black;"><p>V případě zápisu offline dokončete proces ručního zápisu pro nový server RMS. Další informace získáte v této sadě dokumentace v části Ruční zápis serveru kořenové certifikace tématu Provoz serveru RMS.</p></td>
<td style="border:1px solid black;"><p>Server RMS lze začít používat až po provedení zápisu.</p>
<p>Stránky pro správu služby RMS lze také používat až po zápisu.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Provozní</p></td>
<td style="border:1px solid black;"><p>Naimportujte soubor s důvěryhodnou doménou publikování, který jste vyexportovali v kroku 3.</p></td>
<td style="border:1px solid black;"><p>Účet služby RMS musí mít oprávnění ke čtení v umístění, ve kterém je soubor uložen. V opačném případě jej nebude možné úspěšně naimportovat.</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Provozní</p></td>
<td style="border:1px solid black;"><p>Podepište znovu každou šablonu, kterou jste naimportovali společně s důvěryhodnou doménou publikování.</p></td>
<td style="border:1px solid black;"><p>Šablony jsou podepsány pomocí soukromého klíče serveru. Vzhledem k tomu, že tento server má nový soukromý klíč, je nutné šablony znovu podepsat, aby byly platné. Další informace získáte v této sadě dokumentace v části Podpis šablony zásad práv tématu Provoz serveru RMS.</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Provozní</p></td>
<td style="border:1px solid black;"><p>Proveďte opětovnou distribuci šablon do klientských počítačů, které se zúčastnily pilotního projektu.</p></td>
<td style="border:1px solid black;"><p>Staré šablony je nutné odebrat a nahradit šablonami podepsanými tímto serverem.</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Provozní</p></td>
<td style="border:1px solid black;"><p>Naimportujte soubor s důvěryhodnou doménou uživatelů, který jste vyexportovali v kroku 4.</p></td>
<td style="border:1px solid black;"><p>Tento krok umožňuje použití starších klientských certifikátů pro poskytování licencí a certifikátů účtů práv.</p>
<p>Pokud v rámci této migrace dochází k přesouvání uživatelských účtů mezi doménovými strukturami, musí mít účty odpovídající servery proxy SMTP.</p></td>
</tr>
</tbody>
</table>
<p> </p>

Po dokončení nastavení serveru v provozním prostředí ověřte, zda uživatelé pilotního prostředí mají stále možnost vytvářet a číst dříve vytvořenou poštu. Do clusteru můžete pak přidat takový počet serverů RMS, jaký je potřeba pro podporu daného počtu uživatelů v organizaci.
