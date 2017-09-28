---
TOCTitle: Databáze adresářových služeb RMS
Title: Databáze adresářových služeb RMS
ms:assetid: '6f6b8586-5d17-4a40-94a3-4dc738195301'
ms:contentKeyID: 18113361
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747617(v=WS.10)'
---

Databáze adresářových služeb RMS
================================

Databázový server je hostitelem databáze adresářových služeb, která obsahuje informace o uživatelích, identifikátorech (například e-mailové adresy), ID zabezpečení (SID), členství ve skupinách a alternativních identifikátorech. Uvedené informace se získávají z dotazů LDAP odesílaných globálnímu katalogu služby Active Directory prostřednictvím služby správy licencí RMS. Další informace o tomto procesu a jeho účelu získáte v tomto tématu později v části [Mezipaměť služby Active Directory pro službu RMS](https://technet.microsoft.com/c721a2eb-2fe9-4346-b426-3cc169b97265).

Skupina RMS Service Group má pro uložené procedury, které jsou uloženy v databázi adresářových služeb, oprávnění pro spuštění.

Atributy adresářových služeb, které jsou uloženy v databázových tabulkách adresářových služeb, jsou uvedeny v následující tabulce.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Tabulka</th>
<th>Atribut</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">GroupAliases</td>
<td style="border:1px solid black;"><ul>
<li>GroupName: alias pro skupinu<br />
<br />
</li>
<li>GroupID: jedinečný ID pro tuto skupinu<br />
<br />
</li>
</ul></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">GroupIdentifiers</td>
<td style="border:1px solid black;"><ul>
<li>GroupDN: rozlišující název adresářových služeb pro tuto skupinu<br />
<br />
</li>
<li>GroupID: jedinečný ID pro tuto skupinu<br />
<br />
</li>
<li>Expiration: datum a čas vypršení údajů, které jsou uloženy pro tuto skupinu<br />
<br />
</li>
</ul></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">GroupMembership</td>
<td style="border:1px solid black;"><ul>
<li>GroupID: jedinečný ID pro tuto skupinu<br />
<br />
</li>
<li>ParentID: jedinečný ID pro skupinu, jejímž členem je tato skupina<br />
<br />
</li>
</ul></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PrincipalAliases</td>
<td style="border:1px solid black;"><ul>
<li>PrincipalName: název aliasu pro zaregistrovaný objekt<br />
<br />
</li>
<li>PrincipalID: jedinečný ID pro tento zaregistrovaný objekt<br />
<br />
</li>
</ul></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">PrincipalIdentifiers</td>
<td style="border:1px solid black;"><ul>
<li>PrincipalID: jedinečný ID pro tento zaregistrovaný objekt<br />
<br />
</li>
<li>Expiration: datum a čas vypršení údajů, které jsou uloženy pro tento zaregistrovaný objekt<br />
<br />
</li>
</ul></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PrincipalMembership</td>
<td style="border:1px solid black;">Každý řádek této tabulky obsahuje jedinečný ID zaregistrovaného objektu a jedinečný ID skupiny, jejímž členem je tento objekt.
<ul>
<li>PrincipalID: jedinečný ID pro tento zaregistrovaný objekt<br />
<br />
</li>
<li>ParentID: jedinečný ID skupiny, jejímž členem je zaregistrovaný objekt<br />
<br />
</li>
</ul></td>
</tr>
</tbody>
</table>
