---
TOCTitle: Služba vyřazení z provozu RMS
Title: Služba vyřazení z provozu RMS
ms:assetid: '97677e3b-bc83-47ec-b6db-d326cd94566c'
ms:contentKeyID: 18113430
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747695(v=WS.10)'
---

Služba vyřazení z provozu RMS
=============================

Služba vyřazení z provozu je vlastní webovou službou, kterou instaluje instalační program služby RMS. Je spuštěna na kořenovém clusteru i na clusterech vyhrazených pro správu licencí. Pokud tuto službu povolíte, všechny ostatní webové služby RMS na serveru budou zakázány.

Tato služba dešifruje klíč obsahu v licenci k publikování pro obsah chráněný právy a poskytne jej klientovi v odpovědi na požadavek na licencování. Tento postup umožňuje uložení obsahu bez ochrany služby RMS. Služba vyřazení z provozu protokoluje všechny požadavky klientů, které jí byly položeny, a odesílá je službě naslouchání protokolování, kde jsou zaznamenány do databáze protokolování.

Službu vyřazení z provozu lze povolit na stránce **Nastavení zabezpečení** webu pro správu. Jakmile tuto službu povolíte, nelze na serveru obnovit standardní konfiguraci služby RMS.

Po povolení této služby byste měli nastavit volitelný seznam řízení přístupu (DACL) souboru decommission.asmx tak, aby umožňoval přístup podnikovým uživatelům, kteří pomocí daného serveru získali licence pro jejich obsah, a zároveň byste měli do tohoto seznamu přidat skupinu RMS Service Group s oprávněním ke čtení a spouštění, abyste službě RMS umožnili spravovat příslušné operace. Jakmile je zrušena ochrana veškerého obsahu, který je publikován na tomto serveru, je vhodné provést zálohu informací soukromého klíče a odebrat službu RMS ze serveru.

V následující tabulce je znázorněn výchozí seznam řízení přístupu k této službě:

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Uživatel nebo skupina</th>
<th>Výchozí oprávnění</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">SYSTEM</td>
<td style="border:1px solid black;">Úplné řízení</td>
</tr>
</tbody>
</table>
