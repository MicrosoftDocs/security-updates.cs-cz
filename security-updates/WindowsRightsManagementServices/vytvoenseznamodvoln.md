---
TOCTitle: Vytvoření seznamů odvolání
Title: Vytvoření seznamů odvolání
ms:assetid: '1ef75199-3344-4225-84de-a863a777696a'
ms:contentKeyID: 18113205
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc720208(v=WS.10)'
---

Vytvoření seznamů odvolání
==========================

Při implementaci odvolání je třeba nainstalovat seznam odvolání, což je dokument XML vyhovující syntaxi jazyka XrML (eXtensible Rights Markup Language) obsahující objekty zabezpečení, které nadále nemají přístup k obsahu chráněnému právy. Pomocí nástroje pro podepisování seznamů odvolání (RLsigner.exe), který je součástí služby RMS, je nutné vytvořit seznamy odvolání označené časovým razítkem a podepsané odpovídajícím způsobem.

> [!IMPORTANT]
> Chcete-li seznam odvolání podepsat pomocí nástroje RLsigner.exe, je nutné soubor seznamu odvolání uložit jako soubor Unicode. 

Příklad seznamu odvolání
------------------------

Toto téma obsahuje příklad úplného seznamu odvolání s ukázkou všech přípustných způsobů odvolání. Tento příklad můžete použít jako vzor při vytváření vlastních seznamů odvolání.

Seznam odvolání představuje soubor XML, který používá jazyk XrML.

Prvek BODY obsahuje čtyři podřízené prvky:

-   **ISSUEDTIME:** Obsahuje datum a čas vydání seznamu odvolání. Nástroj RLsigner.exe vloží uvedený prvek do souboru. Prvek je v příkladu uveden pouze z důvodu znázornění celé struktury souboru seznamu odvolání.
-   **DESCRIPTOR:** Obsahuje data, která soubor identifikují jako seznam odvolání.
-   **ISSUER:** Obsahuje data identifikující entitu, která seznam odvolání vydává.
-   **REVOCATIONLIST:** Obsahuje podřízené prvky REVOKE, které určují entity odvolané daným seznamem.

V následující části najdete ukázkový soubor seznamu odvolání.

> [!NOTE]
>Prvky ISSUEDTIME, PUBLICKEY a SIGNATURE lze vynechat, protože je vkládá nebo přepisuje nástroj RLsigner.exe.
        
```        
<?xml version="1.0" ?> 
<XrML xml:space=”preserve” version=”1.2”>
  <BODY type="LICENSE" version="3.0">
    <ISSUEDTIME>...</ISSUEDTIME> 
    <DESCRIPTOR>
      <OBJECT type="Revocation-List">
        <ID type="MS-GUID">{d6373cba-01f1-4f32-ac58-260f580af0f8}</ID>
      </OBJECT>
    </DESCRIPTOR>
<ISSUER>
      <OBJECT type="Revocation-List">
        <ID type="acsii-tag">External revocation authority</ID>
        <NAME>Revocation list name</NAME>
        <ADDRESS type="URL">https://somedomain.com/revocation_list_file</ADDRESS>
      </OBJECT>
      <PUBLICKEY>...</PUBLICKEY>
    </ISSUER>
  <REVOCATIONLIST>
    <REVOKE>...<\REVOKE>
    <REVOKE>...<\REVOKE>
  </REVOCATIONLIST>
  <SIGNATURE>...</SIGNATURE>
</XrML>
```
> [!CAUTION]
> Při zadávání adresy URL v seznamu odvolání již není ve službě RMS s aktualizací SP1 nebo ve službě RMS s aktualizací SP2 podporována cesta UNC. Je nutné použít adresu URL. 

Po definici prvků REVOKE je seznam odvolání připraven k podpisu.

Použití prvku REVOKE
--------------------

V ukázkovém seznamu odvolání v části Příklad seznamu odvolání určuje každý prvek REVOKE objekt zabezpečení, který má být odvolán. Úvodní značka obsahuje atributy kategorie a typu, které určují typ odvolávaného objektu a kritérium identifikace objektu pro odvolání. V závislosti na akci určené atributy kategorie a typu obsahují různé prvky REVOKE různé podřízené prvky.

Další informace týkající se určování prvků REVOKE naleznete v následujících ukázkách:

-   [Odvolání objektů zabezpečení na základě veřejného klíče](#bkmk_1)
-   [Odvolání certifikátů a licencí na základě identifikátoru GUID](#bkmk_2)
-   [Odvolání certifikátů a licencí na základě hodnoty hash](#bkmk_3)
-   [Odvolání certifikátů a licencí na základě veřejného klíče vydavatele](#bkmk_4)
-   [Odvolání certifikátů a licencí na základě ID vydavatele](#bkmk_5)
-   [Odvolání obsahu na základě ID obsahu](#bkmk_6)
-   [Odvolání certifikátů na základě ID objektu zabezpečení](#bkmk_10)
-   [Odvolání objektů zabezpečení na základě identifikátoru služby Windows Live ID](#bkmk_7)

<span id="BKMK_1"></span>
#### Odvolání objektů zabezpečení na základě veřejného klíče
V tomto příkladu je odvolán objekt zabezpečení na základě svého veřejného klíče. Obsah značky &lt;PUBLICKEY&gt; pochází z uzlu &lt;BODY&gt;&lt;ISSUEDPRINCIPALS&gt;&lt;PRINCIPAL&gt;&lt;PUBLICKEY&gt; certifikátu, který klíč vydal.

```
      <REVOKE category="principal" type="principal-key">
        <PUBLICKEY>
          <ALGORITHM>RSA-1024</ALGORITHM>
          <PARAMETER name="public exponent">
            <VALUE encoding="integer32">65537</VALUE>
          </PARAMETER>
          <PARAMETER name="modulus">
            <VALUE encoding="base64" size="1024">
6Jn0kEAWU+1AFWtuUmBYL8Jza8tLhUv/BCmgcq/Pc08Au3DvXkH65s+0MEyZjM+71j3F1xaXUSst+wH2FjApkY1RxgL8VAKIuEvIy9hRrvY1YhJx/0Ite5fZeg2crUFrmoQgZzaJ50FvoakA2QMgZZgxoQmwiGE0y40cEJtIlE0=
            </VALUE>
          </PARAMETER>
        </PUBLICKEY>
      </REVOKE>
```

<span id="BKMK_2"></span>
#### Odvolání certifikátů a licencí na základě identifikátoru GUID
V tomto příkladu jsou odvolány certifikát nebo licence na základě identifikátoru GUID (globálně jedinečného identifikátoru). Pokud je nastaven tento seznam odvolání, není možné použít certifikát či licenci s odpovídajícím identifikátorem GUID. Obsah značky &lt;ID&gt; pochází z uzlu &lt;BODY&gt;&lt;DESCRIPTOR&gt;&lt;OBJECT&gt;&lt;ID&gt; odvolávaného certifikátu nebo licence. (Tímto způsobem je také možné odvolat aplikace, a to určením ID manifestu aplikace.)

```
<REVOKE category="license" type="license-id">
        <OBJECT>
          <ID type="MS-GUID">{06BCB94D-43E5-419f-B180-AA9FD321ED7A}</ID>
        </OBJECT>
      </REVOKE>
```

#### Odvolání podle manifestu aplikace

Chcete-li provést odvolání podle manifestu aplikace, je nutné z tohoto manifestu extrahovat ID vydavatele, veřejný klíč vydavatele, ID licence nebo hodnotu hash licence. U manifestů aplikací je však použito kódování base64, takže informace nejsou k dispozici ve formátu prostého textu. Pomocí sady SDK Služby správy přístupových práv lze prostřednictvím metod DRMConstructCertificateChain, DRMDeconstructCertificateChain a DRMDecode vytvořit program umožňující dekódování manifestu aplikace a získání požadovaných informací.

Chcete-li zabránit některým aplikacím ve využití obsahu chráněného právy, zvažte jejich vyloučení, což clusteru služby RMS znemožní udělování licencí k použití těmto aplikacím. Vyloučení však nemůže zabránit uživateli s platnou licencí k použití v dešifrování obsahu chráněného právy. Další informace o vyloučení aplikací získáte v tomto tématu v části [Vyloučení aplikací](https://technet.microsoft.com/b68ae4b2-b9ba-44ae-90cb-c88df600ec86) uvedené již dříve.

<span id="BKMK_3"></span>
#### Odvolání certifikátů a licencí na základě hodnoty hash
V tomto příkladu jsou odvolány certifikát nebo licence na základě hodnoty hash. Obsah značky &lt;VALUE&gt; odpovídá hodnotě hash SHA-1 znaků UNICODE z části mezi značkami &lt;BODY&gt; a &lt;/BODY&gt; (včetně těchto znaků) v certifikátu nebo licenci. Tuto hodnotu hash je možné nalézt v části &lt;SIGNATURE&gt; certifikátu nebo licence. (Tímto způsobem je také možné odvolat aplikace, a to určením hodnoty hash manifestu aplikace.)

```
<REVOKE category="license" type="license-hash">
        <DIGEST>
          <ALGORITHM>SHA1</ALGORITHM>
          <VALUE encoding="base64" size="160">
            ABfB4mcEslVCMEZR9reACqXHCoQ=
          </VALUE>
        </DIGEST>
      </REVOKE>
```

#### Odvolání podle manifestu aplikace

Chcete-li provést odvolání podle manifestu aplikace, je nutné z tohoto manifestu extrahovat ID vydavatele, veřejný klíč vydavatele, ID licence nebo hodnotu hash licence. U manifestů aplikací je však použito kódování base64, takže informace nejsou k dispozici ve formátu prostého textu. Pomocí sady SDK Služby správy přístupových práv lze prostřednictvím metod DRMConstructCertificateChain, DRMDeconstructCertificateChain a DRMDecode vytvořit program umožňující dekódování manifestu aplikace a získání požadovaných informací.

Chcete-li zabránit některým aplikacím ve využití obsahu chráněného právy, zvažte jejich vyloučení, což clusteru služby RMS znemožní udělování licencí k použití těmto aplikacím. Vyloučení jsou však omezena a nemohou zabránit uživateli s platnou licencí k použití v dešifrování obsahu chráněného správou přístupových práv. Další informace o vyloučení aplikací získáte v tomto tématu v části [Vyloučení aplikací](https://technet.microsoft.com/b68ae4b2-b9ba-44ae-90cb-c88df600ec86) uvedené již dříve.

<span id="BKMK_4"></span>
#### Odvolání certifikátů a licencí na základě veřejného klíče vydavatele
V tomto příkladu jsou odvolány všechny certifikáty a licence vydané vlastníkem určeného veřejného klíče. Obsah značky &lt;PUBLICKEY&gt; pochází z uzlu &lt;BODY&gt;&lt;ISSUER&gt;&lt;PUBLICKEY&gt; odvolávaného certifikátu nebo licence.
```
<REVOKE category="license" type="issuer-key">
        <PUBLICKEY>
          <ALGORITHM>RSA-1024</ALGORITHM>
          <PARAMETER name="public exponent">
            <VALUE encoding="integer32">65537</VALUE>
          </PARAMETER>
          <PARAMETER name="modulus">
            <VALUE encoding="base64" size="1024">
AAn0kEAWU+1AFWtuUmBYL8Jza8tLhUv/BCmgcq/Pc08Au3DvXkH65s+0MEyZjM+71j3F1xaXUSst+wH2FjApkY1RxgL8VAKIuEvIy9hRrvY1YhJx/0Ite5fZeg2crUFrmoQgZzaJ50FvoakA2QMgZZgxoQmwiGE0y40cEJtIlE0=
            </VALUE>
          </PARAMETER>
        </PUBLICKEY>
      </REVOKE>
```

<span id="BKMK_5"></span>
#### Odvolání certifikátů a licencí na základě ID vydavatele
V tomto příkladu je odvolána sada certifikátů nebo licencí na základě ID vydavatele. Obsah značky &lt;ID&gt; pochází z uzlu &lt;BODY&gt;&lt;ISSUER&gt;&lt;OBJECT&gt;&lt;ID&gt; odvolávaného certifikátu nebo licence.
```
      <REVOKE category="license" type="issuer-id">
        <OBJECT type="MS-DRM-Server">
          <ID type="MS-GUID">{2BE9E200-3040-41B9-8832-D4D0445EBBD6}</ID> 
        </OBJECT>
      </REVOKE>
```

> [!NOTE]
> Při určování typu ID se ujistěte, že mezi identifikátorem GUID a uzavírací značkou není žádný znak konce stránky. Pokud dojde k náhodnému přidání znaku konce stránky, klient RMS nebude moci analyzovat seznam odvolání. 

<span id="BKMK_6"></span>
#### Odvolání obsahu na základě ID obsahu
V tomto příkladu je odvolán chráněný obsah na základě ID obsahu. Tento způsob je pro odvolání obsahu doporučen, protože ID obsahu je stejné ve všech licencích k použití vytvořených z dané licence k publikování. Hodnotu uzlu &lt;OBJECT&gt; je možné nalézt v uzlu &lt;BODY&gt;&lt;WORK&gt;&lt;OBJECT&gt; licence k publikování nebo licence k použití pro daný obsah.
```
<REVOKE category="content" type="content-id">
        <OBJECT type="Microsoft Office Document">
          <ID type="MS-GUID">{8702641D-3512-4AA4-A584-84C703A5B5C0}</ID>
        </OBJECT>
      </REVOKE>
```

> [!NOTE]
> Při určování typu ID se ujistěte, že mezi identifikátorem GUID a uzavírací značkou není žádný znak konce stránky. Pokud dojde k náhodnému přidání znaku konce stránky, klient RMS nebude moci analyzovat seznam odvolání. 

<span id="BKMK_10"></span>
#### Odvolání objektů zabezpečení na základě účtu systému Windows
V tomto příkladu je odvolán uživatel nebo povolující objekt zabezpečení na základě svého účtu systému Windows. Obsah prvku &lt;OBJECT&gt; pochází z uzlu &lt;BODY&gt;&lt;ISSUEDPRINCIPALS&gt;&lt;PRINCIPAL&gt;&lt;OBJECT&gt; certifikátu účtu práv nebo licence k použití.
```
<REVOKE category="principal" type="principal-id">
        <OBJECT type="Group-Identity">
          <ID type="Windows">{Windows account SID}</ID> 
          <NAME>{E-mail address}</NAME> 
        </OBJECT>
      </REVOKE>
```

> [!NOTE]
> Při určování typu ID se ujistěte, že mezi identifikátorem SID účtu systému Windows a uzavírací značkou není žádný znak konce stránky. Pokud dojde k náhodnému přidání znaku konce stránky, klient RMS nebude moci analyzovat seznam odvolání. 

<span id="BKMK_7"></span>
#### Odvolání objektů zabezpečení na základě identifikátoru služby Windows Live ID
V tomto příkladu je odvolán uživatel nebo povolující objekt zabezpečení na základě svého identifikátoru služby Windows Live ID. Obsah prvku &lt;OBJECT&gt; pochází z uzlu &lt;BODY&gt;&lt;ISSUEDPRINCIPALS&gt;&lt;PRINCIPAL&gt;&lt;OBJECT&gt; certifikátu účtu práv nebo licence k použití.
```
<REVOKE category="principal" type="principal-id">
        <OBJECT type="Group-Identity">
          <ID type="Passport">{PUID}</ID> 
          <NAME>michael@contoso.com</NAME> 
        </OBJECT>
      </REVOKE>
```

> [!NOTE]
> Při určování typu ID se ujistěte, že mezi identifikátorem PUID a uzavírací značkou není žádný znak konce stránky. Pokud dojde k náhodnému přidání znaku konce stránky, klient RMS nebude moci analyzovat seznam odvolání. 

<span id="BKMK_8"></span>
Vložení podpisu do seznamu odvolání
-----------------------------------

Po vytvoření seznamu odvolání je třeba postupem popsaným v tomto tématu vložit do seznamu podpis. Potom můžete seznam odvolání poskytnout k dispozici uživatelům na adrese URL určené v přidružené šabloně zásad práv.

V prvním kroku vkládání podpisu je třeba pomocí nástroje pro vytváření silných názvů (Sn.exe) vygenerovat pár klíčů a soubor klíčů pro seznam odvolání. Nástroj Sn.exe je součástí sady Microsoft .NET Framework SDK 1.1, která je k dispozici na webu společnosti Microsoft [http://go.microsoft.com/fwlink/?LinkId=104796](http://go.microsoft.com/fwlink/?linkid=104796) (stránka může být v angličtině).

Soubor seznamu odvolání je nutné uložit jako soubor Unicode, aby jej bylo možné podepsat pomocí nástroje RLsigner.exe.

**Následujícím postupem vygenerujete pomocí nástroje Sn.exe nový pár klíčů a uložíte jej do souboru:**
1.  Vytvořte privátní klíč. Na příkazovém řádku zadejte následující příkaz a stiskněte klávesu ENTER:

    **sn -k***soubor\_privátního\_klíče***.snk**,

    kde hodnota *soubor\_privátního\_klíče* představuje název daného souboru klíče.

2.  Pomocí nástroje Sn.exe extrahujte veřejný klíč ze souboru páru klíčů vytvořeného v kroku 1 a vyexportujte jej do samostatného souboru. Zadejte následující příkaz a stiskněte klávesu ENTER:

    **sn -p***soubor\_privátního\_klíče soubor\_veřejného\_klíče*,

    kde hodnota *soubor\_privátního\_klíče* představuje soubor privátního klíče vytvořený v kroku 1 a hodnota *soubor\_veřejného\_klíče* představuje název souboru, do kterého bude uložen exportovaný veřejný klíč.

3.  Změňte příponu souboru privátního klíče (vytvořeného v kroku 1) z hodnoty SNK na DAT, aby jej mohl použít nástroj RLsigner.exe.

4.  Pomocí nástroje RLsigner.exe vložte podpis do souboru seznamu odvolání. Tento nástroj je součástí služby RMS. Ve výchozím nastavení je uložen v adresáři %systemdrive%\\Program Files\\Windows Rights Management Services\\Tools.

> [!NOTE]
> Nástroj RLsigner.exe nepodporuje názvy souborů obsahující mezery.         

<span id="BKMK_9"></span>
Použití nástroje RLsigner.exe
-----------------------------

Nástroj RLsigner.exe po spuštění nejprve vytvoří podpis pomocí privátního klíče získaného ze souboru klíčů. Pak vytvoří výstupní soubor založený na poskytnutém souboru seznamu odvolání.

> [!IMPORTANT]
> Soubor seznamu odvolání je nutné uložit jako soubor Unicode, aby jej mohl nástroj RLsigner.exe použít. 

Chcete-li seznam odvolání podepsat pomocí nástroje RLsigner.exe, zadejte na příkazový řádek následující příkaz:

**rlsigner.exe** *vstupní\_soubor* **{-f** *soubor\_klíčů* **| -h** *název\_kontejneru* **CSP}** *výstupní\_soubor*

Parametry příkazu zadejte na základě následujících informací:

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Parametr</th>
<th style="border:1px solid black;" >Popis</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><em>vstupní_soubor</em></td>
<td style="border:1px solid black;">Název připraveného souboru seznamu odvolání, který vyhovuje syntaxi jazyka XrML</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><em>soubor_klíčů</em></td>
<td style="border:1px solid black;">Název souboru obsahujícího generovaný privátní a veřejný klíč</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><em>název_kontejneru</em></td>
<td style="border:1px solid black;">Název kontejneru klíče</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><em>výstupní_soubor</em></td>
<td style="border:1px solid black;">Název podepsaného souboru seznamu odvolání, který nástroj vytvoří</td>
</tr>
</tbody>
</table>
  
| ![](images/Cc720208.note(WS.10).gif)Poznámka |  
|---------------------------------------------------------------------------|  
| Nástroj RLsigner.exe nepodporuje názvy souborů obsahující mezery.         |
  
V následujících příkladech je popsáno, jak lze nástroj RLsigner.exe použít na příkazovém řádku pro různé zprostředkovatele kryptografických služeb:
  
-   Příklad syntaxe příkazového řádku se souborem klíčů:  

    **rlsigner.exe rl.xml -f key.dat output.xml**  
-   Příklad syntaxe příkazového řádku s modulem hardwarového zabezpečení:  

    **rlsigner.exe rl.xml -h Container CSP output.xml**
  
Nástroj RLsigner.exe v návratovém kódu vrací informace o základních chybách nebo úspěšném provedení operací. Možné návratové kódy jsou popsány v následující tabulce.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Návratový kód</th>
<th style="border:1px solid black;" >Popis</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">0</td>
<td style="border:1px solid black;">Úspěšné provedení</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">-1</td>
<td style="border:1px solid black;">Nelze číst zdrojový soubor</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">-2</td>
<td style="border:1px solid black;">Nelze číst soubor klíčů</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">-3</td>
<td style="border:1px solid black;">Neplatný soubor klíčů</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">-4</td>
<td style="border:1px solid black;">Neplatný zdrojový soubor</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">-5</td>
<td style="border:1px solid black;">Nelze zapisovat do cílového souboru</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">-6</td>
<td style="border:1px solid black;">Neznámá chyba</td>
</tr>
</tbody>
</table>
  
Podepisování seznamů odvolání je vhodné naplánovat na základě intervalu aktualizace, který byl pro server určen.
  
Postup podepisování seznamů odvolání lze automatizovat pomocí skriptů. Následující ukázkový skript jazyka VBScript zavolá program RLsigner.exe a zapíše výsledek do protokolu systémových událostí.
  
```VB
const EVT_SUCCESS       = 0
const EVT_ERROR         = 1
const EVT_WARNING       = 2
const EVT_INFORMATION   = 4
const EVT_AUDIT_SUCCESS = 8
const EVT_AUDIT_FAILURE = 16

Dim WshShell, oExec

Set WshShell = CreateObject( "WScript.Shell" )
Set oExec = WshShell.Exec("rlsigner.exe input_file key_file output_file")
Do While oExec.Status = 0
     WScript.Sleep 100
Loop

if WshShell.ExitCode <> 0 Then
    WshShell.LogEvent EVT_ERROR, "RLsigner failed with error """ + WshShell.ExitCode + """"
else
    WshShell.LogEvent EVT_SUCCESS, "RLsigner completed successfully"
end if
```
