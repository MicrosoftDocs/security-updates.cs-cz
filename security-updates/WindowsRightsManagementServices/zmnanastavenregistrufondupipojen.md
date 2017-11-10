---
TOCTitle: Změna nastavení registru fondu připojení
Title: Změna nastavení registru fondu připojení
ms:assetid: 'c61d91db-a1ad-4ca5-a492-015da629afbc'
ms:contentKeyID: 18113429
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747660(v=WS.10)'
---

Změna nastavení registru fondu připojení
========================================

Chcete-li zvýšit výkon systému, můžete pomocí položek klíčů registru nastavit vlastnosti fondu připojení LDAP (Lightweight Directory Access Protocol) služby Active Directory, který je používán službou RMS.

V počítačích s 32bitovou verzí systému Windows Server 2003 představuje úplnou cestu podklíče pro položky registru fondu připojení následující klíč registru:

**HKEY\_LOCAL\_MACHINE\\Software\\Microsoft\\DRMS\\1.0**

V počítačích s 64bitovou verzí systému Windows Server 2003 představuje úplnou cestu podklíče pro položky registru fondu připojení následující klíč registru:

**HKEY\_LOCAL\_MACHINE\\SoftwareWOW6432Node\\Microsoft\\DRMS\\1.0**

V následující tabulce jsou uvedeny položky, které lze použít k potlačení výchozího nastavení fondu připojení služby Active Directory. Zobrazeny jsou výchozí hodnoty. Další informace o způsobu, jímž služba RMS vytváří seznam dotazů a používá toto nastavení, získáte v tomto tématu v části Optimalizace nastavení fondu připojení služby Active Directory uvedené již dříve.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Název</th>
<th style="border:1px solid black;" >Typ</th>
<th style="border:1px solid black;" >Výchozí hodnota</th>
<th style="border:1px solid black;" >Popis</th>
<th style="border:1px solid black;" >Poznámky</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">GC</td>
<td style="border:1px solid black;">String</td>
<td style="border:1px solid black;">název-1, ..., název-n</td>
<td style="border:1px solid black;">Seznam globálních katalogů (využívající názvy DNS), oddělený čárkami. Tento klíč omezuje použití globálních katalogů v rámci služby RMS pouze na zadané katalogy.</td>
<td style="border:1px solid black;">Pokud nechcete, aby služba RMS vytvořila seznam dotazů, zadejte pomocí tohoto nastavení globální katalogy, které mají být použity.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">MinGC</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">1</td>
<td style="border:1px solid black;">Minimální počet globálních katalogů, které musí být k dispozici ještě před spuštěním služby RMS.</td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">MaxGC</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">15</td>
<td style="border:1px solid black;">Maximální počet globálních katalogů, které algoritmus pro zjišťování topologie přidá do seznamu dotazů.</td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">ThreshHoldAlive</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">1</td>
<td style="border:1px solid black;">Minimální počet funkčních připojení, než služba DiscoveryServices začne vyhledávat další globální katalogy, které je možné přidat do seznamu dotazů, aby mohla služba RMS přijímat požadavky.</td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">RetryDown</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">5</td>
<td style="border:1px solid black;">Počet pokusů o opakování připojení, než bude deklarováno, že připojení není funkční.</td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">TimeRetryDown</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">300</td>
<td style="border:1px solid black;">Počet sekund, po které je třeba počkat před opakovaným pokusem o připojení.</td>
<td style="border:1px solid black;">Toto výchozí nastavení by nemělo být nutné měnit, s výjimkou neobvyklých okolností.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">TimeRetrySlow</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">30</td>
<td style="border:1px solid black;">Počet sekund, po které je třeba počkat před opakovaným pokusem u pomalého připojení.</td>
<td style="border:1px solid black;">Toto výchozí nastavení by nemělo být nutné měnit, s výjimkou neobvyklých okolností.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">WtRoundRobin</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">1</td>
<td style="border:1px solid black;">Váha kruhového dotazování (round robin) při vyrovnávání zatížení.</td>
<td style="border:1px solid black;">Relativní důležitost kruhového dotazování v rámci vyrovnávání zatížení. Hodnota 1 je nejnižší.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">WtThreadCount</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">100</td>
<td style="border:1px solid black;">Váha počtu podprocesů na jedno připojení při vyrovnávání zatížení.</td>
<td style="border:1px solid black;">Relativní důležitost nízkého počtu podprocesů.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">WtSlow</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">1,000</td>
<td style="border:1px solid black;">Váha pomalého připojení při vyrovnávání zatížení.</td>
<td style="border:1px solid black;">Relativní důležitost toho, že připojení není pomalé.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">TimeOutForGC</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">5</td>
<td style="border:1px solid black;">Počet sekund před vypršením časového limitu požadavku na přidání globálního katalogu k seznamu dotazů.</td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">LdapTimeOut</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">5</td>
<td style="border:1px solid black;">Počet sekund před vypršením časového limitu rozhraní API LDAP.</td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">TopDownExpansionLDAPTimeOut</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">40</td>
<td style="border:1px solid black;">Počet sekund před vypršením časového limitu dotazů rozšíření služby LDAP.</td>
<td style="border:1px solid black;"></td>
</tr>
</tbody>
</table>
  
> [!CAUTION]
> Nesprávné úpravy registru mohou způsobit závažné poškození systému. Před provedením jakýchkoli změn registru byste měli vytvořit záložní kopii všech důležitých dat v počítači. 
