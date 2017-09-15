---
TOCTitle: Zálohování a obnovení systému služby RMS
Title: Zálohování a obnovení systému služby RMS
ms:assetid: 'c11f3ac1-e512-402b-bf13-9ff21f5fe745'
ms:contentKeyID: 18113486
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747745(v=WS.10)'
---

Zálohování a obnovení systému služby RMS
========================================

Při plánování obnovení systému byste měli ve svých plánech počítat se selháním databázového serveru a serveru služby RMS. V případě selhání databázového serveru je možné funkčnost serveru nebo clusteru služby RMS obnovit ze záložní kopie konfigurační databáze. Není nutné získat nový certifikát serveru pro poskytování licencí nebo soukromý klíč serveru RMS, protože tyto položky jsou uloženy v konfigurační databázi.

Plánování zálohování systému služby RMS
---------------------------------------

Kromě klíče serveru jsou v konfigurační databázi uložena data o uživatelích včetně informací o veřejném klíči. Aby byly důležité údaje o klíčích chráněny, vytvořte záložní kopii konfigurační databáze na médium a uložte je na zabezpečené místo. Konfigurační databáze pro cluster kořenové certifikace se často mění, proto se doporučuje pravidelně vytvářet její záložní kopie. Čím častěji jsou do vaší organizace přidáváni noví uživatelé, tím častěji by měla být záložní kopie vytvořena. Při zálohování serveru kořenové certifikace nezapomeňte do zálohy zahrnout také tabulku **sysmessages** z hlavní databáze. Pokud tato tabulka neobsahuje zprávy určené pro službu RMS, nebude moci server kořenové certifikace pracovat a vrátí chybu. Jestliže tabulku do zálohy nezahrnete, můžete ji vytvořit znovu opakováním procesu zajišťování pomocí existující databáze.

Databáze protokolování služby RMS obsahuje protokoly, ve kterých můžete najít zajímavé informace pro řešení potíží nebo statistiku, ale obvykle se nejedná o zásadní součást systému služby RMS. Databáze adresářových služeb je místní mezipamětí databáze služby Active Directory, takže se znovu automaticky vytvoří během obnovení systému služby RMS. Při plánování zálohování databází služby RMS se poraďte se správcem serveru SQL Server.

Pokud k ochraně soukromých klíčů služby RMS používáte hardwarový modul zabezpečení, je třeba zálohovat také konfiguraci tohoto modulu. Další informace týkající se zálohování a obnovení konfigurace hardwarového modulu zabezpečení naleznete v dokumentaci k tomuto modulu.

| ![](images/Cc747745.note(WS.10).gif)Poznámka                                                                                                                                                                                                                                |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Pokud k šifrování soukromých klíčů služby RMS používáte jiného než výchozího softwarového zprostředkovatele kryptografických služeb (CSP), zajistěte v organizaci před použitím tohoto zprostředkovatele ve službě RMS vytvoření postupů při správě klíčů (například postupů při zálohování a obnovení). |

Plánování obnovení systému služby RMS
-------------------------------------

Jestliže obnovujete databázový server ze zálohy, přesvědčte se, zda je verze spuštěné služby RMS stejná jako verze spuštěná při vytváření zálohy. Informujte uživatele o tom, že pokud začali systém služby RMS používat po datu vytvoření zálohy, budou muset získat nový certifikát účtu práv. Nedojde však ke ztrátě žádného chráněného obsahu.

Chcete-li obnovit jeden server RMS určitého clusteru, přeinstalujte službu RMS a potom daný server přidejte do clusteru pomocí existující databáze. Tento krok nijak neovlivní uživatele systému služby RMS, protože servery seskupené do clusteru pracují jako celek.
