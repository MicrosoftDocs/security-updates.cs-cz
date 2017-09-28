---
TOCTitle: Služba aktivačního proxy serveru RMS
Title: Služba aktivačního proxy serveru RMS
ms:assetid: '6b9d33ef-466b-405b-a768-54e5615d6770'
ms:contentKeyID: 18113354
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747608(v=WS.10)'
---

Služba aktivačního proxy serveru RMS
====================================

Všechny požadavky na aktivaci počítače služby RMS verze 1.0 jsou zpracovávány službou aktivačního proxy serveru, která je spuštěna pouze na kořenovém clusteru služby RMS. Klientský počítač je nutné aktivovat ještě před tím, než v něm budete pomocí služby RMS publikovat nebo používat obsah chráněný právy. Od verze služby RMS s aktualizací Service Pack 1 se klient aktivuje sám, takže nemusí generovat bezpečnostní modul a certifikát počítače pomocí aktivačního proxy serveru nebo služby Microsoft Activation Service.

Služba aktivačního proxy serveru předá požadavky na aktivaci počítače od klientů RMS verze 1.0 službě Microsoft Activation Service. Ta vrátí vlastní vygenerovaný bezpečnostní modul a odpovídající certifikát počítače RMS, který je jedinečný pro konkrétního uživatele a počítač. Služba aktivačního proxy serveru pak tyto položky předá zpět klientovi, který požadavky generoval.

Aplikační soubor služby aktivačního proxy serveru (soubor Activation.asmx) je uložen ve virtuálním adresáři Certification, který je součástí Internetové informační služby. V následující tabulce je znázorněn výchozí seznam řízení přístupu k této službě:

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
<td style="border:1px solid black;">Administrators</td>
<td style="border:1px solid black;">Úplné řízení</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Guests</td>
<td style="border:1px solid black;">Čtení a spouštění</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">RMS Service Group</td>
<td style="border:1px solid black;">Čtení a spouštění</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">SYSTEM</td>
<td style="border:1px solid black;">Úplné řízení</td>
</tr>
</tbody>
</table>
