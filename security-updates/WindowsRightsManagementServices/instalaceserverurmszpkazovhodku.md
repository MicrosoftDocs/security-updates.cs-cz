---
TOCTitle: Instalace serveru RMS z příkazového řádku
Title: Instalace serveru RMS z příkazového řádku
ms:assetid: 'b55b1e2a-dd14-4168-a37f-9cdedbec660b'
ms:contentKeyID: 18113473
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747733(v=WS.10)'
---

Instalace serveru RMS z příkazového řádku
=========================================

Službu RMS s aktualizací Service Pack 2 (SP2) můžete nainstalovat z příkazového řádku, což umožňuje instalaci automatizovat. Automatizaci instalace lze provést dvěma způsoby: provedením bezobslužné instalace pomocí staženého klienta EXE nebo použitím extrahovaných souborů MSI ze staženého souboru EXE pro instalaci klienta RMS. K instalaci staženého souboru EXE použijte následující syntaxi:

**WindowsRightsManagementServicesSP2-KB917275-Client-ENU.exe -override 1 /I MsDrmClient.msi REBOOT=ReallySuppress /q -override 2 /I RmClientBackCompat.msi REBOOT=ReallySuppress /q**

Chcete-li instalaci provést pomocí souborů Instalační služby systému Windows® (MSI), je třeba soubory MSI nejprve extrahovat ze spustitelného souboru služby RMS s aktualizací SP2. Spuštěním následujícího příkazu na příkazovém řádku extrahujete soubory msdrmclient.msi a RmClientBackCompat.msi:

**WindowsRightsManagementServiceSP2-KB917275-Server-ENU.exe /X:C:\\***umístění\_instalace*

Po extrahování souborů MSI můžete k instalaci služby RMS použít následující příkazy:

**msiexec.exe /I MSDrmClient.msi /qn ALLUSERS=2 /m MSIDHOG /lei logfile.log DISPLYPAGE="NO" TARGETDIR=c:\\***umístění\_instalace*

**msiexec.exe /I RMClientBackCompat.msi /qn ALLUSERS=2 /m MSIDHOG /lei logfile.log DISPLYPAGE="NO" TARGETDIR=c:\\***umístění\_instalace*

V následující tabulce je popsána syntaxe jednotlivých příkazů.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Parametr</th>
<th style="border:1px solid black;" >Definice</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">

**/I MSDrmClient.msi** nebo **/I RMClientBackCompat.msi**</td>
<td style="border:1px solid black;">

Povinný parametr. Určuje produkt, který má být nainstalován.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">

**/qn**</td>
<td style="border:1px solid black;">

Nepovinný parametr. Určuje tichou instalaci, bez interakce s uživatelem.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">

**/lei** <em>logfile.log</em></td>
<td style="border:1px solid black;">

Nepovinný parametr. Určuje soubor, do kterého budou protokolovány chybové zprávy a zprávy o stavu.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">

**DISPLAYPAGE=”NO”**</td>
<td style="border:1px solid black;">

Nepovinný parametr. Určuje, že po dokončení instalace nebude zobrazena stránka **Globální správa**.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">

**TARGETDIR=c:\\**<em>umístění_instalace</em></td>
<td style="border:1px solid black;">

Nepovinný parametr. Určuje adresář, do kterého má být služba RMS s aktualizací Service Pack 2 nainstalována. Pokud umístění nezadáte, bude použito výchozí umístění instalace.</td>
</tr>
</tbody>
</table>
  
| ![](images/Cc747733.note(WS.10).gif)Poznámka                                                                                                                                                   |  
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Bez ohledu na to, který způsob instalace zvolíte, je nutné úspěšně nainstalovat oba soubory MSI. Pokud by došlo k chybě, která by znemožnila instalaci souboru MSDrmClient.msi, neinstalujte soubor RMClientBackCompat.msi. |
