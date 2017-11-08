---
TOCTitle: Certifikace účtů služby RMS
Title: Certifikace účtů služby RMS
ms:assetid: 'c9a385c5-6dbb-47f5-a80f-69718e6f9deb'
ms:contentKeyID: 18113516
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747750(v=WS.10)'
---

Certifikace účtů služby RMS
===========================

Při certifikaci účtů se vytváří certifikát účtu práv, který spojuje účet určitého uživatele s konkrétním počítačem a umožňuje danému uživateli v tomto počítači využít obsah chráněný službou RMS. Jakmile uživatel poprvé publikuje obsah chráněný službou RMS nebo se pokusí o využití takového obsahu v klientském počítači, odešle aplikace s podporou služby RMS požadavek na certifikát účtu práv službě certifikace účtů RMS.

Služba certifikace může daného uživatele ověřit prostřednictvím ověřování systému Windows nebo prostřednictvím certifikátu x.509 uloženého v hardwarovém šifrovacím zařízení, jako je karta Smart Card. Po ověření vytvoří server RMS pro daného uživatele certifikát účtu práv, který je založen na ověřených pověřeních tohoto uživatele. Zašifruje soukromý klíč uživatele pomocí veřejného klíče certifikátu počítače RMS příslušného klientského počítače a vloží jej do daného certifikátu účtu práv. Potom odešle certifikát účtu práv aplikaci, která si jej vyžádala. Ta jej uloží v počítači nebo zařízení, aby byl k dispozici pro další publikování nebo požadavky na licence k použití. Certifikát účtu práv je zároveň uložen v konfigurační databázi.

Certifikace účtů následuje po procesu aktivace počítače, protože požadavek na certifikát účtu práv vyžaduje certifikát počítače RMS příslušného klientského počítače.

Uživatelé musí certifikát účtu práv získat pro každý počítač, který používají. Pokud uživatel pracuje s více počítači, je pro každý z nich vydán jedinečný certifikát účtu práv, ale všechny počítače obsahují stejný pár klíčů daného uživatele.

Aplikace s podporou služby RMS požadující licenci k použití vkládá certifikát účtu práv do příslušného požadavku. Služba správy licencí pomocí veřejného klíče certifikátu účtu práv šifruje klíč obsahu. Tímto způsobem je zajištěno, že danou licenci k použití může využít pouze odpovídající ověřený uživatel.

Proces certifikace účtu obsahuje následující kroky:

1.  Jakmile uživatel poprvé publikuje obsah chráněný službou RMS nebo se pokusí o využití takového obsahu v daném počítači, odešle aplikace s podporou služby RMS požadavek na certifikát účtu práv službě certifikace účtů na serveru kořenové certifikace.
2.  Služba certifikace účtů ověří uživatele pomocí služby ověřování systému Windows.
3.  Služba certifikace účtů vytvoří pro daného uživatele certifikát účtu práv založený na ověřených pověřeních tohoto uživatele. Zašifruje soukromý klíč uživatele pomocí veřejného klíče certifikátu počítače RMS a vloží jej do certifikátu. Potom odešle certifikát účtu práv aplikaci, která si jej vyžádala.
4.  Ta jej uloží v počítači nebo zařízení, aby byl k dispozici pro další publikování nebo požadavky na licence k použití.

Služba certifikace účtů, od níž klient požaduje certifikát účtu práv, závisí na typu počítače, ve kterém je klient RMS nainstalován. Standardní stolní počítače se připojují ke službě certifikace účtů (certification.asmx). Serverové služby, u kterých byla povolena služba RMS SP1, získávají certifikáty účtů práv od služby certifikace serverů (ServeCertfication.asmx). Mobilní zařízení, u nichž byla povolena služba RMS SP1, získávají certifikáty účtů práv od služby certifikace mobilních zařízení (MobileDeviceCertfication.asmx). Ve výchozí instalaci služby RMS SP1 je povolena pouze služba certifikace účtů.

Další informace o používání služby RMS SP1 u mobilních zařízení a serverových služeb získáte v této sadě dokumentace v části Povolení podpory serveru RMS pro mobilní zařízení a serverové služby tématu Provoz serveru RMS.
