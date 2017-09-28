---
TOCTitle: Zabezpečení během zajišťování
Title: Zabezpečení během zajišťování
ms:assetid: '9f1282c5-5642-4870-a9a4-c3a485f8ff76'
ms:contentKeyID: 18113386
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747616(v=WS.10)'
---

Zabezpečení během zajišťování
=============================

Prostředky služby RMS můžete na existujícím webu zajistit pomocí webu správy služby RMS. Během zajišťování se v rámci tohoto webu vytvářejí virtuální adresáře a fondy aplikací a na databázovém serveru dojde k vytvoření a konfiguraci databází služby RMS. Jestliže je daný server připojen k Internetu, může být také během procesu zajišťování zapsán ke službě Microsoft Enrollment Services.

Během zajišťování používá služba RMS účty popsané v následující tabulce.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th>Účet</th>
<th>Účel</th>
<th>Oprávnění</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Účet přihlášeného uživatele</td>
<td style="border:1px solid black;">Vytvoří virtuální adresáře a fondy aplikací. Služba IIS vyžaduje ověřování systému Windows a služba RMS představuje přihlášeného uživatele, který musí být přihlášen místně.</td>
<td style="border:1px solid black;">Úplné řízení (přihlášený uživatel musí být místním správcem)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Systémový účet</td>
<td style="border:1px solid black;">Vytvoří dočasné sestavení pro serializaci.</td>
<td style="border:1px solid black;">Oprávnění pro čtení a zápis pro dočasnou složku systému Windows C:\Windows\Temp.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Účet ASPNET</td>
<td style="border:1px solid black;">Vytvoří dočasné sestavení souborů *.aspx.</td>
<td style="border:1px solid black;">Přístup k dočasnému adresáři mezipaměti sestavení C:\Windows\Microsoft.NET\Framework\v1.1.4322\Dočasné soubory ASP.NET (ve výchozím nastavení).</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Účet Síťové služby</td>
<td style="border:1px solid black;">Registruje spojovací bod služby v rámci služby Active Directory.</td>
<td style="border:1px solid black;"><ul>
<li>Oprávnění pouze pro čtení pro web zajišťování (obvykle C:\Inetpub\Wwwroot\Provisioning).<br />
<br />
</li>
<li>Oprávnění ke čtení a zápisu pro klíč registru <strong>DRMS</strong>. Oprávnění jsou udělena instalačním programem služby RMS, který zároveň vytvoří následující klíč registru.<br />
<br />
Počítače s 32bitovou verzí systému Windows Server 2003<br />
<br />
<code>HKEY_LOCAL_MACHINE\Software\Microsoft\DRMS\1.0</code><br />
<br />
Počítače s 64bitovou verzí systému Windows Server 2003<br />
<br />
<code>HKEY_LOCAL_MACHINE\Software\WOW6432Node\Microsoft\DRMS\1.0</code><br />
<br />
</li>
</ul></td>
</tr>
</tbody>
</table>
 

Během zajišťování provádí služba RMS následující úlohy:

-   Databázový server:
    -   Vytvoří databáze pro konfiguraci, pro adresářové služby a pro protokolování.
    -   Udělí oprávnění pro přihlášení skupině RMS Service Group.
    -   Instaluje uložené procedury v databázích a udělí oprávnění pro spuštění skupině RMS Service Group.
    -   Spustí dotazy v hlavní databázi.
-   Přidá skupinu RMS Service Group do skupiny IIS\_WPG.
-   V adresáři C:\\Inetpub\\Wwwroot\\\_wmcs vytvoří hierarchii virtuálních adresářů, souborů a fondů aplikací pro webové služby a web správy služby RMS.
-   Vytvoří volitelné seznamy řízení přístupu (DACL) pro virtuální adresáře, soubory a fondy aplikací.
-   Skupině RMS Service Group umožní přístup do dočasné složky.
-   Pokud je požadována softwarová ochrana klíče, zašifruje soukromý klíč poskytovatele licence serveru před jeho uložením do databáze. Služba RMS vyžaduje během zajišťování heslo a získá přístup k rozhraní DPAPI na úrovni počítače.
-   Instaluje službu naslouchání protokolování.
-   Vytvoří frontu protokolování zpráv.
-   V případě zajišťování serveru kořenové certifikace nastaví spojovací bod služby v rámci služby Active Directory.
