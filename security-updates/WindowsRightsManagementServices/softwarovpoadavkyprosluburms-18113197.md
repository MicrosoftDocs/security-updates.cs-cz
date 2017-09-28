---
TOCTitle: Softwarové požadavky pro službu RMS
Title: Softwarové požadavky pro službu RMS
ms:assetid: '17faf2ad-2366-4a92-98a5-766e20a0f741'
ms:contentKeyID: 18113197
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc720201(v=WS.10)'
---

Softwarové požadavky pro službu RMS
===================================

Softwarové požadavky pro servery používající službu RMS jsou uvedeny v následující tabulce.

###  

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Software</th>
<th>Požadavek</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>Operační systém</p></td>
<td style="border:1px solid black;"><p>Kterékoli vydání systému Microsoft Windows Server® 2003 kromě verze Web Edition.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Systém souborů</p></td>
<td style="border:1px solid black;"><p>Je doporučen systém souborů NTFS.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Součásti operačního systému</p></td>
<td style="border:1px solid black;"><ul>
<li>Služba Řízení front zpráv (známá také jako MSMQ) s povolenou integrací adresářové služby Active Directory®<br />
<br />
</li>
<li>Internetová informační služba (IIS) s povolenými službami ASP.NET.<br />
<br />
</li>
<li>Rozhraní Microsoft .NET Framework 1.1<br />
<br />
</li>
</ul></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Adresářová služba Active Directory®</p></td>
<td style="border:1px solid black;"><p>Službu RMS je nutné nainstalovat v doméně služby Active Directory s řadiči systému Windows Server 2000 s aktualizací Service Pack 3 (SP3) nebo vyšší. Všichni uživatelé a skupiny využívající službu RMS k získávání a publikování obsahu musí mít e-mailovou adresu konfigurovanou ve službě Active Directory.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Databázový server</p></td>
<td style="border:1px solid black;"><p>K provádění operací vyžaduje služba RMS databázi a uložené procedury. Můžete použít Microsoft SQL Server 2000 s aktualizací SP3a nebo novější či Microsoft SQL Server 2005. Pro testování nebo nasazení v jednom počítači lze použít Microsoft SQL Server Desktop Engine (MSDE 2000) s aktualizací SP3 nebo Microsoft SQL Server 2005 Express Edition.</p></td>
</tr>
</tbody>
</table>
  
Pokud nasazujete službu RMS do prostředí s více doménovými strukturami služby Active Directory, je třeba použít univerzální skupiny služby Active Directory, aby bylo členství ve skupinách replikováno do všech globálních katalogů. Chcete-li vytvořit univerzální skupiny, musí být úroveň funkčnosti domény nastavena nejméně na nativní režim systému Windows 2000 a úroveň funkčnosti doménové struktury musí být zvýšena na Windows Server 2003.
  
MSDE 2000 nebo Microsoft SQL Server 2005 Express Edition je pro podporu databází doporučeno používat pouze v testovacím prostředí, protože MSDE 2000 ani Microsoft SQL Server 2005 Express Edition nepodporují žádná síťová rozhraní. Podmínky používání serveru MSDE 2000 nebo Microsoft SQL Server 2005 Express Edition navíc určují, že klientské nástroje serveru SQL Server nelze používat k práci s databázemi serveru MSDE 2000 nebo Microsoft SQL Server 2005 Express Edition. Vzhledem k tomuto omezení by nebylo možné zobrazit informace obsažené v protokolech a změnit data uložená v konfigurační databázi.
  
Pokud nemáte na serveru nainstalováno rozšíření ASP.NET verze 1.1, bude se proces instalace lišit podle toho, zda používáte 32bitovou verzi systému Windows Server 2003 nebo 64bitovou verzi systému Windows Server 2003.
  
Pokud používáte 32bitovou verzi systému Windows Server 2003, nainstalujte a povolte rozšíření ASP.NET verze 1.1 pomocí následujícího postupu:
  
1.  Otevřete panel **Přidat nebo odebrat programy** v **Ovládacích panelech** a pak klepněte na tlačítko **Přidat nebo odebrat součásti systému**.  
2.  Klepněte na možnost **Aplikační server** a pak klepněte na tlačítko **Podrobnosti**.  
3.  V Průvodci součástmi systému Windows vyberte položku **ASP.NET**.  
4.  Pokud je nainstalováno rozšíření ASP.NET 1.1, ale není povoleno jako rozšíření webové služby IIS:  
    -   Otevřete modul snap-in pro správu Internetové informační služby.  
    -   Klepněte na možnost **Rozšíření webové služby IIS**, vyberte položku ASP.NET v1.1.4322 a pak klepněte na tlačítko **Povolit**.
  
Pokud používáte 64bitovou verzi systému Windows Server 2003, pomocí následujícího postupu nainstalujte a povolte rozšíření ASP.NET verze 1.1:
  
1.  Nainstalujte rozhraní .NET Framework 1.1, které nainstaluje rozšíření ASP.NET 1.1. Distribuční balíček rozhraní Microsoft .NET Framework verze 1.1 můžete stáhnout ze služby Stažení softwaru ([http://go.microsoft.com/fwlink/?LinkId=69985](http://go.microsoft.com/fwlink/?linkid=69985)) (stránka může být v angličtině).  
2.  Otevřete modul snap-in pro správu Internetové informační služby.  
3.  Klepněte na možnost Rozšíření webové služby IIS, vyberte položku ASP.NET v1.1.4322 a pak klepněte na tlačítko Povolit.
  
Pokud jste spustili službu RMS v 64bitové verzi systému Windows Server 2003, je třeba pomocí následujícího postupu povolit spolupráci Internetové informační služby se serverem RMS:
  
1.  Klepněte na tlačítko **Start** a pak na příkaz **Spustit**.  
2.  Do pole **Otevřít** zadejte následující příkaz a pak stiskněte klávesu ENTER:
  
**"cscript %SystemDrive%\\inetpub\\AdminScripts\\adsutil.vbs set w3svc/AppPools/Enable32bitAppOnWin64 1"**
  
Služba RMS není určena pro rozhraní .NET Framework verze 2.0. Ačkoli je souběžná instalace podporována, je třeba zajistit, aby bylo rozhraní ASP.NET konfigurováno na používání verze ASP.NET v1.1.4322. Funkčnost souběžné instalace lze zajistit dvěma způsoby:
  
-   Před instalací serveru RMS je třeba nainstalovat rozhraní .NET Framework verze 2.0.  
-   Nastavte rozhraní ASP.NET zpět na verzi 1.1.4322 na výchozím webu služby IIS spuštěním následujícího příkazu:
  
**"%SystemRoot%\\Microsoft.NET\\Framework\\v1.1.4322\\aspnet\_regiis -s w3svc/1/root"**
  
Další informace o službách Active Directory, Řízení front zpráv a IIS získáte v Centru pro nápovědu a odbornou pomoc systému Windows Server 2003.
  
| ![](images/Cc720201.Caution(WS.10).gif)Upozornění                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |  
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Server RMS lze zajistit na výchozím webu nebo na libovolném webu, který jste předem definovali ve službě IIS. Z důvodů zabezpečení nepoužívejte zvolený server k provozování dalších webů a služeb. Pokud byste toto doporučení nerespektovali, mohla by nastat situace, kdy pod stejným účtem jako služba RMS (konkrétně pod místním systémovým účtem) pracují i další aplikace a služby, a soukromé klíče by mohly být vystaveny nezaručeným operacím. Server RMS byste neměli zajišťovat na stejném webu jako Microsoft Office SharePoint Server 2007. Službu RMS nelze kombinovat s ověřováním Kerberos. Při zajišťování serveru RMS na webu bude na tomto serveru zakázáno ověřování Kerberos. Pokud služba RMS není konfigurována na používání rozhraní ASP.NET v1.1.4322, nebudou do databází protokolování zapsány žádné informace, čímž dojde ke ztrátě dat. |
  
Viz také  
--------
  
####  
  
[Plánování infrastruktury databázového serveru](https://technet.microsoft.com/b12354bd-3143-4d1f-b5aa-450c4550653c)
