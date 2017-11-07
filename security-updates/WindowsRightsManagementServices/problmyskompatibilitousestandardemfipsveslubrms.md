---
TOCTitle: Problémy s kompatibilitou se standardem FIPS ve službě RMS
Title: Problémy s kompatibilitou se standardem FIPS ve službě RMS
ms:assetid: '720bdace-dcd8-431e-b0fa-01193782fe0b'
ms:contentKeyID: 18113313
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747551(v=WS.10)'
---

Problémy s kompatibilitou se standardem FIPS ve službě RMS
==========================================================

Aktualizace Service Pack 1 (SP1) Služby správy přístupových práv (RMS) verze 1.0 je určena k tomu, aby umožňovala efektivní práci v organizacích, které vyžadují používání kryptografických funkcí kompatibilních se standardem FIPS.

Standard FIPS (Federal Information Processing Standard) 140-1 a jeho následovník FIPS 140-2 jsou standardy vlády USA, které představují referenční srovnání pro implementaci kryptografického softwaru. Určují doporučené postupy pro implementaci kryptografických algoritmů, zpracování klíčových materiálů a vyrovnávacích pamětí dat a také pro práci s operačním systémem.

Službu RMS lze implementovat v rámci systému kompatibilního se standardem FIPS jako prostředek ochrany tajných dat.

-   Zprostředkovatelé kryptografických služeb kompatibilní se standardem FIPS omezují funkce na: **TLS\_RSA\_WITH\_3DES\_EDE\_CBC\_SHA**. Toto omezení nutí zprostředkovatele zabezpečených kanálů vyjednávat pouze silnější protokol TLS (Transport Layer Security) 1.0. Pravděpodobně bude nutné nakonfigurovat aplikaci Internet Explorer tak, aby podporovala protokol TLS, avšak řada webových serverů třetích stran protokol TLS nepodporuje. Další informace o tomto problému naleznete v článku 811834 znalostní báze Knowledge Base na [webu společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=43614).

Pokud budete chtít používat softwarovou ochranu soukromého klíče, zabezpečte soukromý klíč služby RMS pomocí jednoho ze dvou výchozích zprostředkovatelů kryptografických služeb společnosti Microsoft. Tito zprostředkovatelé kryptografických služeb prošli procesem vyhodnocování, při kterém proběhla kontrola kompatibility se standardy FIPS 140-1 nebo FIPS 140-2 (podle účelu) vlády USA. Přestože to není vyžadováno, lze zákazníkům, pro které hraje zabezpečení velkou roli, doporučit, aby k zabezpečení soukromých klíčů serveru RMS nejvyšší úrovně používali hardwarové moduly zabezpečení (například od společnosti nCipher nebo IBM). V případě použití hardwarových modulů zabezpečení je nutné vybrat příslušného zprostředkovatele kryptografických služeb pro daný modul. Je možné, že tento krok bude vyžadovat restartování systému. Další informace o tomto problému naleznete v článku 830690 znalostní báze Knowledge Base na [webu společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=44138).

Při implementaci svého systému služby RMS byste měli provést následující kroky:

-   Postupujte podle pokynů úřadu NSA pro kryptografii kompatibilní se standardem FIPS v systému Windows.
-   Zapněte v místních zásadách zabezpečení kryptografii kompatibilní se standardem FIPS.
-   Nasaďte klienty a servery RMS SP1 ve výše uvedeném prostředí.
-   Povolte na svém serveru RMS protokol TLS (Transport Layer Security) v rámci služby IIS.
-   Povolte pro své klienty protokol TLS (Transport Layer Security) v rámci aplikace Internet Explorer.
-   Povolte protokol SQL TDS (Tabular Data Stream), který se používá se zprostředkovatelem zabezpečení Windows TLS/SSL mezi klienty SQL a serverem SQL na databázovém serveru.
-   Nakonfigurujte na serveru SQL vyžadování protokolu TSL/SSL.
