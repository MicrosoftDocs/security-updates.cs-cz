---
TOCTitle: Účty a oprávnění potřebné pro službu RMS
Title: Účty a oprávnění potřebné pro službu RMS
ms:assetid: '07a51daa-6823-41e6-b453-92f1a0592361'
ms:contentKeyID: 18113222
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc720178(v=WS.10)'
---

Účty a oprávnění potřebné pro službu RMS
========================================

V následující tabulce jsou uvedena uživatelská práva a oprávnění, která jsou potřebná k nasazení a správě služby RMS.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Činnost</th>
<th style="border:1px solid black;" >Uživatelský účet a oprávnění</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Instalace služby RMS</td>
<td style="border:1px solid black;">Přihlaste se pomocí doménového účtu, který je členem místní skupiny Administrators.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Zajištění služby RMS</td>
<td style="border:1px solid black;">Přihlaste se pomocí doménového účtu, který je členem místní skupiny Administrators. Použitý účet musí mít navíc u databáze serveru SQL Server udělenu roli pro přihlášení k serveru SQL jako správce systému, aby mohla služba RMS zřizovat databáze.
Při zajištění je nutné zadat účet služby RMS a tento účet již musí existovat. Mělo by jít o standardní účet uživatele domény bez jakýchkoli dalších oprávnění. Tento účet bude přidán do skupiny RMS Service Group a služba RMS pod ním bude pracovat za běžného provozu.
U nasazení na jediný server, kde se databáze nachází ve stejném počítači jako server kořenové certifikace, můžete zadat místní systémový účet. Z důvodů zabezpečení se doporučuje používat vždy účet služby RMS, nikoli místní systémový účet. Pokud je databáze umístěna na samostatném serveru, je nutné zadat účet služby RMS.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Správa služby RMS</td>
<td style="border:1px solid black;">Přihlaste se pomocí doménového účtu, který je členem místní skupiny Administrators. Pro účely správy přístupu k webovým stránkám správy lze přizpůsobit nastavení zabezpečení.</td>
</tr>
</tbody>
</table>
  
> [!NOTE]
> Účet použitý pro přihlášení k serveru RMS nemusí být členem žádných dalších doménových skupin, jako je skupina Domain Admins. Některé úlohy správy, jako je například registrace spojovacího bodu služby nebo úpravy zásad zabezpečení, však vyžadují účet s dalšími oprávněními. 
