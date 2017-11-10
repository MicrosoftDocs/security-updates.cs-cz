---
TOCTitle: Potlačení rozpoznání služby Active Directory
Title: Potlačení rozpoznání služby Active Directory
ms:assetid: '9d97e7fb-5b05-4853-ad7b-6cc82b9729f0'
ms:contentKeyID: 18113384
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747614(v=WS.10)'
---

Potlačení rozpoznání služby Active Directory
============================================

Služby RMS a klienti zjišťují umístění služeb tak, že nejprve hledají v místním registru. Pokud určité klíče v registru nemají hodnotu, služby RMS a klienti hledají v adresáři služby Active Directory spojovací bod služby. To znamená, že můžete přepsat výchozí nastavení zjišťování služby Active Directory, pokud zadáte určité klíče v registru serveru nebo klienta.

> [!NOTE]
> Jestliže je váš kořenový cluster služby RMS nakonfigurován tak, že spojovací bod služby není publikován v adresáři služby Active Directory, můžete pomocí těchto klíčů směrovat své klienty služby RMS na správné umístění. 

Tato část popisuje položky registru a podrobnosti o tom, jak je můžete vytvořit.

Konfigurace jiného nastavení zjišťování služeb pro dílčí zápis v clusterech vyhrazených pro správu licencí
----------------------------------------------------------------------------------------------------------

Jestliže zajišťujete cluster vyhrazený pro správu licencí a chcete u něj provést dílčí zápis s jiným kořenovým clusterem, než který jste nasadili do doménové struktury služby Active Directory clusteru vyhrazeného pro správu licencí, je třeba nakonfigurovat jiné nastavení zjišťování jak pro dílčí zápis, tak i pro službu certifikace účtů.

#### Popisy položek registru

Následující položky registru se používají ke konfiguraci jiného nastavení dílčího zápisu a službu certifikace účtů.

-   **SubEnrollmentURL**. Tato položka určuje cestu ke kořenovému clusteru, který server pro správu licencí používá při požadování svého certifikátu serveru pro poskytování licencí.
-   **GicURL**. Tato položka určuje cestu ke službě certifikace účtů pro tento vyhrazený cluster pro správu licencí.

#### Podrobnosti položky

V počítačích s 32bitovou verzí systému Windows Server 2003 je úplná cesta k podklíči registru pro položky zjišťování služby pro dílčí zápis clusteru vyhrazeného pro správu licencí tato:

**HKEY\_LOCAL\_MACHINE\\Software\\Microsoft\\DRMS\\1.0**

V počítačích s 64bitovou verzí systému Windows Server 2003 je úplná cesta k podklíči registru pro položky zjišťování služby pro dílčí zápis clusteru vyhrazeného pro správu licencí tato:

**HKEY\_LOCAL\_MACHINE\\SoftwareWOW6432Node\\Microsoft\\DRMS\\1.0**

Následující tabulka uvádí položky, které můžete přidat za účelem konfigurace jiného nastavení (přepsání) zjišťování služby.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Název</th>
<th style="border:1px solid black;" >Typ</th>
<th style="border:1px solid black;" >Hodnota</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">SubEnrollmentURL</td>
<td style="border:1px solid black;">Řetězec</td>
<td style="border:1px solid black;">http(nebo https)://<em>název_serveru</em>/_wmcs/certification/subenrollservice.asmx</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">GicURL</td>
<td style="border:1px solid black;">Řetězec</td>
<td style="border:1px solid black;">http(nebo https)://<em>název_serveru</em>/_wmcs/certification/certification.asmx</td>
</tr>
</tbody>
</table>
  
Konfigurace jiného nastavení zjišťování služby na straně klienta pro publikování  
--------------------------------------------------------------------------------
  
Jestliže budou vaši uživatelé publikovat obsah ze svých počítačů, můžete nakonfigurovat jiné nastavení umístění serverů používaných pro publikování v závislosti na topologii používané v podniku. Umístění serverů používaných pro publikování jsou standardně zjišťována klientem pomocí služby Active Directory. Přidáním odpovídajících klíčů registru do klientských počítačů klienti tyto metody obejdou a místo toho použijí adresy URL, které zadáte v hodnotě položky registru.
  
> [!NOTE]
> Jiné hodnoty použité klientem uvedené v těchto částech je potřeba vytvořit jako klíče, nikoli jako jednotlivé položky. Hodnotu těchto klíčů je potřeba vytvořit ve výchozí položce pro každý klíč. 
  
#### Popisy klíčů registru
  
Pomocí následujících klíčů registru lze nastavit jinou hodnotu pro automatické zjišťování clusteru RMS.
  
-   **Activation**. Tento klíč registru definuje adresu URL služby aktivace počítače. Jestliže používáte klienta služby RMS s aktualizací Service Pack 1 nebo novější, tato položka registru se již nepoužívá.  
-   **EnterprisePublishing**. Tento klíč registru definuje adresu URL instalace služby RMS, kterou má tento klient používat pro požadavky na licence.  
-   **CloudPublishing**. Tento klíč registru definuje adresu URL služby správy licencí od společnosti Microsoft, kterou lze využívat, pokud klient nemá přístup k instalaci služby RMS, ale má přístup k Internetu.
  
#### Podrobnosti klíče
  
Úplná cesta k podklíči registru pro položky zjišťování služby na straně klienta pro publikování:
  
**HKEY\_LOCAL\_MACHINE\\Software\\Microsoft\\MSDRM\\ServiceLocation\\**
  
Následující tabulka uvádí klíče registru, které můžete přidat do klientského počítače RMS za účelem konfigurace jiného nastavení (přepsání) zjišťování služby.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Název</th>
<th style="border:1px solid black;" >Typ</th>
<th style="border:1px solid black;" >Hodnota</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Activation</td>
<td style="border:1px solid black;">Řetězec</td>
<td style="border:1px solid black;">http(nebo https)://<em>název_clusteru_RMS</em>/_wmcs/Certification, kde <em>název_clusteru_RMS</em> je název vašeho clusteru RMS.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">EnterprisePublishing</td>
<td style="border:1px solid black;">Řetězec</td>
<td style="border:1px solid black;">http(nebo https)://<em>název_clusteru_RMS</em>/_wmcs/Licensing, kde <em>název_clusteru_RMS</em> je název vašeho clusteru RMS.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">CloudPublishing</td>
<td style="border:1px solid black;">Řetězec</td>
<td style="border:1px solid black;">http(nebo https)://<em>plně kvalifikovaný název domény_clusteru</em>/_wmcs/Licensing, kde <em>plně kvalifikovaný název domény_clusteru</em> je plně kvalifikovaný název domény vašeho clusteru RMS.</td>
</tr>
</tbody>
</table>
  
Doporučujeme implementovat tyto položky registru buď pomocí serveru SMS (Systems Management Server) nebo pomocí zásad skupiny, a zajistit tak, aby všichni klienti ve vašem podniku používali správné servery pro publikování.
  
> [!CAUTION]
> Nesprávná úprava registru může vážně poškodit systém. Před prováděním změn registru byste měli v počítači zálohovat veškerá cenná data. 
  
K importu správných klíčů registru na každém serveru v clusteru služby RMS lze používat ukázkový soubor registru (REG).
  
**Import správných klíčů registru na každém serveru v clusteru služby RMS**  
1.  Zkopírujte následující ukázkový soubor registru do Poznámkového bloku.
  
    ```
    Windows Registry Editor Version 5.00
 
    [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\MSDRM\ServiceLocation]
  
    [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\MSDRM\ServiceLocation\Activation]
  
    @="http://<RMS_cluster_name>/_wmcs/certification"
  
    [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\MSDRM\ServiceLocation\EnterprisePublishing]
  
    @="http://<RMS_cluster_name>/_wmcs/licensing"
    ```
  
2.  Proměnnou &lt;název\_clusteru\_RMS&gt; nahraďte názvem svého clusteru RMS.
  
3.  Uložte soubor s příponou REG.
  
4.  Poklepejte na název souboru v Průzkumníku systému Windows.
  
5.  V dialogovém okně **Řízení uživatelských účtů** potvrďte, že opravdu chcete provést zobrazenou akci, a klepněte na položku **Pokračovat**.. Když se zobrazí dotaz, zda chcete přidat informace do registru, klepněte na tlačítko **Ano**.
