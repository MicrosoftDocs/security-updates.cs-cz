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

<p> </p>
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
<th>Název</th>
<th>Typ</th>
<th>Výchozí hodnota</th>
<th>Popis</th>
<th>Poznámky</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>GC</p></td>
<td style="border:1px solid black;"><p>String</p></td>
<td style="border:1px solid black;"><p>název-1, ..., název-n</p></td>
<td style="border:1px solid black;"><p>Seznam globálních katalogů (využívající názvy DNS), oddělený čárkami. Tento klíč omezuje použití globálních katalogů v rámci služby RMS pouze na zadané katalogy.</p></td>
<td style="border:1px solid black;"><p>Pokud nechcete, aby služba RMS vytvořila seznam dotazů, zadejte pomocí tohoto nastavení globální katalogy, které mají být použity.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>MinGC</p></td>
<td style="border:1px solid black;"><p>DWORD</p></td>
<td style="border:1px solid black;"><p>1</p></td>
<td style="border:1px solid black;"><p>Minimální počet globálních katalogů, které musí být k dispozici ještě před spuštěním služby RMS.</p></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>MaxGC</p></td>
<td style="border:1px solid black;"><p>DWORD</p></td>
<td style="border:1px solid black;"><p>15</p></td>
<td style="border:1px solid black;"><p>Maximální počet globálních katalogů, které algoritmus pro zjišťování topologie přidá do seznamu dotazů.</p></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>ThreshHoldAlive</p></td>
<td style="border:1px solid black;"><p>DWORD</p></td>
<td style="border:1px solid black;"><p>1</p></td>
<td style="border:1px solid black;"><p>Minimální počet funkčních připojení, než služba DiscoveryServices začne vyhledávat další globální katalogy, které je možné přidat do seznamu dotazů, aby mohla služba RMS přijímat požadavky.</p></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>RetryDown</p></td>
<td style="border:1px solid black;"><p>DWORD</p></td>
<td style="border:1px solid black;"><p>5</p></td>
<td style="border:1px solid black;"><p>Počet pokusů o opakování připojení, než bude deklarováno, že připojení není funkční.</p></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>TimeRetryDown</p></td>
<td style="border:1px solid black;"><p>DWORD</p></td>
<td style="border:1px solid black;"><p>300</p></td>
<td style="border:1px solid black;"><p>Počet sekund, po které je třeba počkat před opakovaným pokusem o připojení.</p></td>
<td style="border:1px solid black;"><p>Toto výchozí nastavení by nemělo být nutné měnit, s výjimkou neobvyklých okolností.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>TimeRetrySlow</p></td>
<td style="border:1px solid black;"><p>DWORD</p></td>
<td style="border:1px solid black;"><p>30</p></td>
<td style="border:1px solid black;"><p>Počet sekund, po které je třeba počkat před opakovaným pokusem u pomalého připojení.</p></td>
<td style="border:1px solid black;"><p>Toto výchozí nastavení by nemělo být nutné měnit, s výjimkou neobvyklých okolností.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>WtRoundRobin</p></td>
<td style="border:1px solid black;"><p>DWORD</p></td>
<td style="border:1px solid black;"><p>1</p></td>
<td style="border:1px solid black;"><p>Váha kruhového dotazování (round robin) při vyrovnávání zatížení.</p></td>
<td style="border:1px solid black;"><p>Relativní důležitost kruhového dotazování v rámci vyrovnávání zatížení. Hodnota 1 je nejnižší.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>WtThreadCount</p></td>
<td style="border:1px solid black;"><p>DWORD</p></td>
<td style="border:1px solid black;"><p>100</p></td>
<td style="border:1px solid black;"><p>Váha počtu podprocesů na jedno připojení při vyrovnávání zatížení.</p></td>
<td style="border:1px solid black;"><p>Relativní důležitost nízkého počtu podprocesů.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>WtSlow</p></td>
<td style="border:1px solid black;"><p>DWORD</p></td>
<td style="border:1px solid black;"><p>1,000</p></td>
<td style="border:1px solid black;"><p>Váha pomalého připojení při vyrovnávání zatížení.</p></td>
<td style="border:1px solid black;"><p>Relativní důležitost toho, že připojení není pomalé.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>TimeOutForGC</p></td>
<td style="border:1px solid black;"><p>DWORD</p></td>
<td style="border:1px solid black;"><p>5</p></td>
<td style="border:1px solid black;"><p>Počet sekund před vypršením časového limitu požadavku na přidání globálního katalogu k seznamu dotazů.</p></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>LdapTimeOut</p></td>
<td style="border:1px solid black;"><p>DWORD</p></td>
<td style="border:1px solid black;"><p>5</p></td>
<td style="border:1px solid black;"><p>Počet sekund před vypršením časového limitu rozhraní API LDAP.</p></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>TopDownExpansionLDAPTimeOut</p></td>
<td style="border:1px solid black;"><p>DWORD</p></td>
<td style="border:1px solid black;"><p>40</p></td>
<td style="border:1px solid black;"><p>Počet sekund před vypršením časového limitu dotazů rozšíření služby LDAP.</p></td>
<td style="border:1px solid black;"></td>
</tr>
</tbody>
</table>
  
| ![](images/Cc747660.Caution(WS.10).gif)Upozornění                                                                                                  |  
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Nesprávné úpravy registru mohou způsobit závažné poškození systému. Před provedením jakýchkoli změn registru byste měli vytvořit záložní kopii všech důležitých dat v počítači. |
