---
TOCTitle: Změna nastavení mezipaměti služby Active Directory
Title: Změna nastavení mezipaměti služby Active Directory
ms:assetid: '8789a7a5-2065-4fae-9104-e0a70f1f2fb6'
ms:contentKeyID: 18113350
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747586(v=WS.10)'
---

Změna nastavení mezipaměti služby Active Directory
==================================================

Nastavení v registru určuje počet položek, které budou uloženy v mezipaměti služby Active Directory. Chcete-li zlepšit dobu odezvy pro požadavky klienta, můžete toto nastavení změnit. Další informace získáte v tomto tématu v části Optimalizace výkonu adresářových služeb uvedené již dříve. Můžete rovněž zadat dobu platnosti informací uložených v mezipaměti.

V počítačích s 32bitovou verzí systému Windows Server 2003 je úplná cesta podklíče registru pro položky mezipaměti následující:

**HKEY\_LOCAL\_MACHINE\\Software\\Microsoft\\DRMS\\1.0\\DirectoryServices**

V počítačích s 64bitovou verzí systému Windows Server 2003 je úplná cesta podklíče registru pro položky mezipaměti následující:

**HKEY\_LOCAL\_MACHINE\\SoftwareWOW6432Node\\Microsoft\\DRMS\\1.0\\DirectoryServices**

V následující tabulce jsou uvedeny položky, které řídí chování mezipaměti v paměti.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Název</th>
<th style="border:1px solid black;" >Typ</th>
<th style="border:1px solid black;" >Výchozí hodnota</th>
<th style="border:1px solid black;" >Popis</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">PrincipalCacheMax</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">1,000</td>
<td style="border:1px solid black;">Maximální počet zaregistrovaných objektů zabezpečení a jejich e-mailových adres a identifikátorů SID, které lze uložit v mezipaměti.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PrincipalCacheExpireMinutes</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">12</td>
<td style="border:1px solid black;">Doba platnosti informací uložených v mezipaměti pro zaregistrované objekty zabezpečení.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">GroupIDCacheMax</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">1,000</td>
<td style="border:1px solid black;">Maximální počet skupin a jejich e-mailových adres a identifikátorů SID, které lze uložit v mezipaměti.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">GroupIDCacheExpireMinutes</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">12</td>
<td style="border:1px solid black;">Doba platnosti informací uložených v mezipaměti pro členství ve skupinách.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">GroupMembershipCacheMax</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">1,000</td>
<td style="border:1px solid black;">Maximální počet kontaktů, které jsou členy skupiny, již lze uložit v mezipaměti.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">GroupMembershipCacheExpireMinutes</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">12</td>
<td style="border:1px solid black;">Doba platnosti informací uložených v mezipaměti pro kontakty, které jsou členy skupiny.</td>
</tr>
</tbody>
</table>
  
> [!CAUTION]
> Nesprávné úpravy registru mohou způsobit závažné poškození systému. Před provedením jakýchkoli změn registru byste měli vytvořit záložní kopii všech důležitých dat v počítači. 
  
> [!NOTE]
> Položky registru **PrincipalCacheExpireMinutes**, **GroupIDCacheExpireMinutes**, **GroupMembershipCacheExpireMinutes** a **ContactMembersofGroupCacheExpireMinutes** také řídí vypršení platnosti místní mezipaměti služby Active Directory uložené v databázi adresářových služeb na databázovém serveru. 
