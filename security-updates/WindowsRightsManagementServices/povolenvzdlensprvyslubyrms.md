---
TOCTitle: Povolení vzdálené správy služby RMS
Title: Povolení vzdálené správy služby RMS
ms:assetid: '00f17054-5f5d-47e2-89c1-7a593b930bb3'
ms:contentKeyID: 18113198
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc720181(v=WS.10)'
---

Povolení vzdálené správy služby RMS
===================================

V počítači pro vzdálenou správu služby RMS musí být nainstalována aplikace Internet Explorer 6.0 nebo novější.

Povolení vzdálené správy služby RMS
-----------------------------------

#### Povolení vzdálené správy služby RMS

1.  Přihlaste se k serveru, u kterého chcete mít možnost vzdálené správy.

2.  Ze seznamu položky **Nástroje pro správu** otevřete modul snap-in **pro správu Internetové informační služby (IIS**).

3.  Rozbalte položku pro web, na kterém jste zajistili službu RMS.

4.  Klepněte pravým tlačítkem myši na složku **\_wmcs** a poté klepněte na příkaz **Vlastnosti**. Na kartě **Zabezpečení adresáře** klepněte v části **Zabezpečená komunikace** na tlačítko **Upravit**, klepněte na možnost **Vyžadovat zabezpečený kanál** a poté klepněte na tlačítko **OK**. Tímto způsobem u webových služeb RMS nastavíte ochranu prostřednictvím protokolu SSL (Secure Sockets Layer). Další informace o správě webů pomocí Internetové informační služby naleznete v nápovědě ke službě IIS.

    | ![](images/Cc720181.Important(WS.10).gif)Důležité informace                                                                                                                                                                                       |
    |--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Zabezpečení webových služeb RMS lze posílit zavedením protokolu SSL, které zároveň umožní vzdálený přístup HTTP k webovým stránkám správy služby RMS. Pokud chcete u webových služeb RMS povolit protokol SSL, získejte a nainstalujte platný certifikát SSL webového serveru. |

5.  Klepněte pravým tlačítkem myši na složku **Admin** a poté klepněte na příkaz **Vlastnosti**. Na kartě **Zabezpečení adresáře** v části **Omezení podle adres IP a názvů domén** klepněte na tlačítko **Upravit** a poté klepnutím na možnost **Udělit přístup** v části **Omezení přístupu podle adres IP** povolte všem počítačům žádat o spojení s tímto webem.
