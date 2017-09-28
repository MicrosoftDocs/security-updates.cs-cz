---
TOCTitle: Webové služby RMS
Title: Webové služby RMS
ms:assetid: 'ed8dbb2e-0590-4502-afc4-54f66b96d515'
ms:contentKeyID: 18113497
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747728(v=WS.10)'
---

Webové služby RMS
=================

Služba RMS zajišťuje serverovou součást systému RMS. Základní funkce této součásti jsou implementovány jako sada webových služeb Microsoft® ASP.NET, které běží na serveru Internetové informační služby. Webové služby RMS lze využívat prostřednictvím rozhraní SOAP nebo .NET Remoting.

Webové služby zajišťují:

-   dílčí zápis serverů,
-   certifikace účtu důvěryhodných entit,
-   licencování informací chráněných pomocí práv,
-   funkce RMS pro správu.

Webové služby RMS jsou popsány v následující tabulce.

###  

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Služba</th>
<th>Popis</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>Dílčí zápis</p></td>
<td style="border:1px solid black;"><p>Poskytuje podřízené serverové certifikáty pro vystavování licencí serverům v clusterech vyhrazených pro správu licencí. Tyto certifkáty umožňují clusteru vyhrazenému pro správu licencí vystavovat licence k publikování a k použití.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Certifikace účtu</p></td>
<td style="border:1px solid black;"><p>Zajišťuje pro uživatele certifikáty účtů práv. Tyto certifikáty potřebují uživatelé k tomu, aby mohli získat licence k publikování a používání za účelem vytváření a používání obsahu chráněného právy.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Služba Activation Proxy</p></td>
<td style="border:1px solid black;"><p>Tato služba byla zachována z důvodu kompatibility s klientem RMS verze 1. Předává požadavky na aktivaci počítače službě Microsoft Activation Service a vrací bezpečnostní moduly a certifikáty počítače RMS klientům RMS verze 1. Tato služba se nepoužívá klienty RMS s aktualizací Service Pack 1 (SP1) nebo vyšší.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Publikování</p></td>
<td style="border:1px solid black;"><p>Vystavuje licence k publikování, které umožňují autorům vytvářet a distribuovat obsah chráněný právy. Také vystavuje klientské certifikáty pro vystavování licencí, které umožňují uživatelům publikovat obsah chráněný právy, aniž by byli připojeni k interní síti hostující služby RMS.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Licence</p></td>
<td style="border:1px solid black;"><p>Vystavuje licence k použití, které uživatele opravňují k používání obsahu chráněného právy.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Správa</p></td>
<td style="border:1px solid black;"><p>Umožňuje správci spravovat služby RMS.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>DrmRemote</p></td>
<td style="border:1px solid black;"><p>Umožňuje webovým službám komunikovat spolu a s dalšími součástmi systému RMS prostřednictvím technologie .NET Remoting.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Vyřazování z provozu</p></td>
<td style="border:1px solid black;"><p>Zruší ochranu pomocí práv u obsahu a vrátí obsah klientovi. Tuto službu instaluje instalační program služby RMS, ale služba nemá odpovídající virtuální kořen v Internetové informační službě, dokud ji nepovolí správce. Povolením této služby zakážete všechny ostatní služby.</p></td>
</tr>
</tbody>
</table>
  
Kromě webových služeb nainstaluje služba RMS také službu naslouchání protokolování. Každá webová služba odesílá protokolovaná data do fronty zpráv protokolování. Služba naslouchání protokolování potom přenese zaprotokolovaná data z fronty zpráv do databáze protokolování.
  
Aplikace webových služeb se nacházejí ve virtuálních adresářích služby IIS. Tyto virtuální adresáře jsou nainstalovány na každém serveru RMS na webu, který jste vybrali při zajišťování.
  
Ověřování a přístup se konfigurují zvlášť pro každý virtuální adresář. Přístup se také konfiguruje zvlášť pro každou webovou službu. Informace o nastavení zabezpečení u virtuálních aresářů a souborů webových služeb naleznete v části [Podpora Internetové informační služby pro službu RMS](https://technet.microsoft.com/bd4dc69f-1e4e-4e95-9ae2-c925d8a14d4c) dále v tomto tématu.
  
Další informace o každé webové službě naleznete v části [Softwarové součásti služby RMS](https://technet.microsoft.com/e38a840e-f390-48fd-8354-50108a64f5ca) dále v tomto tématu.
