---
TOCTitle: Příprava k instalaci serveru kořenové certifikace
Title: Příprava k instalaci serveru kořenové certifikace
ms:assetid: 'ed51605e-8b17-4155-8d83-f6777f499b7b'
ms:contentKeyID: 18113496
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747726(v=WS.10)'
---

Příprava k instalaci serveru kořenové certifikace
=================================================

Ukázková zkušební instalace zahrnuje pouze jeden server kořenové certifikace. V případě potřeby můžete nainstalovat další servery, a to buď jako součást clusteru kořenové certifikace nebo jako samostatný cluster serverů správy licencí. Příprava infrastruktury probíhá u všech uvedených serverů stejně, takže postup uvedený v tomto tématu bude třeba provést u každého z nich.

Po instalaci řadiče domény a databázových serverů (viz informace v předchozí části) a provedení kroků v následující tabulce bude vše připraveno k instalaci služby RMS.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Součást infrastruktury</th>
<th style="border:1px solid black;" >Příprava serveru na instalaci služby RMS</th>
<th style="border:1px solid black;" >Poznámky pro nasazení v provozním prostředí</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Operační systém</td>
<td style="border:1px solid black;">Do počítače, který splňuje požadavky na hardware služby RMS, ale není ještě připojen k síti, nainstalujte systém Windows Server 2003. Diskový oddíl naformátujte systémem souborů NTFS.</td>
<td style="border:1px solid black;">Doporučuje se vždy instalovat nejnovější aktualizace a opravy. Používejte oddíly formátované pro systém souborů NTFS.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Připojení k Internetu
(nepovinné)</td>
<td style="border:1px solid black;">Vytvořte ethernetové spojení se sítí poskytující možnost připojení k Internetu, která je však oddělena od provozního prostředí. Pokud chcete v rámci procesu zajišťování použít pro server RMS zápis online, musí být server připojen k Internetu.</td>
<td style="border:1px solid black;">Jestliže používáte zápis online, zkontrolujte, zda je součástí připojení k Internetu odpovídající brána firewall.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Adresa IP</td>
<td style="border:1px solid black;">Přiřaďte tomuto počítači statickou adresu IP.</td>
<td style="border:1px solid black;">Pro servery používejte zásadně statické adresy IP.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Připojení počítače k doméně</td>
<td style="border:1px solid black;">Přihlaste se k počítači jako místní správce. Klepněte na tlačítko <strong>Start</strong>, pravým tlačítkem myši klepněte na položku <strong>Tento počítač</strong>, klepněte na příkaz <strong>Vlastnosti</strong>, vyberte kartu <strong>Název počítače</strong> a klepněte na tlačítko <strong>Změnit</strong>.</td>
<td style="border:1px solid black;">U všech serverů použijte stejnou doménu.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Ponechte název počítače beze změny, klepněte na tlačítko <strong>Doména</strong> a poté zadejte název domény, například Contoso.com, a klepněte na tlačítko <strong>OK</strong>. Zadejte pověření uživatele, které používáte pro připojení k doméně, klepněte na tlačítko <strong>OK</strong> a po zobrazení příslušné výzvy restartujte počítač. Po restartování počítače se zobrazí výzva k zadání pověření k přihlášení. Zadejte odpovídající doménu, uživatelské jméno a heslo.</td>
<td style="border:1px solid black;"> </td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Uživatel a přihlášení</td>
<td style="border:1px solid black;">Klepněte pravým tlačítkem myši na ikonu <strong>Tento počítač</strong>, klepněte na příkaz <strong>Spravovat</strong>, rozbalte položku <strong>Místní uživatelé a skupiny</strong>, klepněte na položku <strong>Skupiny</strong> a poklepejte na položku <strong>Správci</strong>.
<br/><br/>
Klepněte na tlačítko <strong>Přidat</strong>, zadejte název uživatelského účtu, který chcete přidat (například Michael@contoso.com), a klepněte na tlačítko <strong>OK</strong>. Poskytněte uživatelskému účtu oprávnění správce. Po zobrazení výzvy zadejte odpovídající pověření, jako například Contoso\Administrator.
<br/><br/>
Přihlaste se jako uživatel domény s oprávněními správce daného počítače.</td>
<td style="border:1px solid black;">Pro přidávání součástí do tohoto počítače je třeba mít práva správce. Některé kroky instalace nelze provést z účtu místního správce. Na tomto serveru musí existovat alespoň jeden uživatel domény, který je zároveň správcem. Služba SQL Server kromě toho vyžaduje práva správce systému pro vytváření nových databází.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Připojení k Internetu
(nepovinné)</td>
<td style="border:1px solid black;">Ověřte přístup k Internetu přechodem na adresu http://uddi.microsoft.com ve webovém prohlížeči. V počítačích se systémem Windows Server 2003 bude pravděpodobně třeba změnit soubory Lmhosts a Hosts tak, aby zahrnovaly řadič domény.</td>
<td style="border:1px solid black;">Ověřte přístup k Internetu přechodem na adresu http://uddi.microsoft.com.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Aktivace systému Windows</td>
<td style="border:1px solid black;">Pomocí Průvodce aktivací můžete aktivovat systém Windows u společnosti Microsoft pomocí internetového připojení nebo se můžete na společnost Microsoft obrátit s žádostí o aktivaci systému Windows prostřednictvím telefonu. Další informace o aktivaci systému Windows Server 2003 naleznete v Centru pro nápovědu a odbornou pomoc systému Windows Server 2003.</td>
<td style="border:1px solid black;">Systém Windows Server 2003 je nutné aktivovat do 14 dnů od instalace.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Aktualizace softwaru</td>
<td style="border:1px solid black;">Nainstalujte nejnovější aktualizace softwaru nainstalovaného v tomto počítači.</td>
<td style="border:1px solid black;">Nainstalujte nejnovější aktualizace softwaru.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Konfigurace aplikace Internet Explorer</td>
<td style="border:1px solid black;">Služba RMS používá pro správu webové rozhraní. Je možné, že některá výchozí nastavení zabezpečení budou bránit správnému zobrazení stránek. Ke konfiguraci některých možností využívají některé stránky webu správy služby RMS překryvná okna.</td>
<td style="border:1px solid black;"> </td>
</tr>
</tbody>
</table>
  
Po dokončení všech předchozích kroků na obou serverech je vše připraveno k instalaci a zajištění služby RMS na serverech.
