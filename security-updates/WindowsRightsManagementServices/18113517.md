---
TOCTitle: Vyhodnocení požadavků migrace
Title: Vyhodnocení požadavků migrace
ms:assetid: 'cec07f45-dc52-4004-860b-5cc33e5fc209'
ms:contentKeyID: 18113517
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747759(v=WS.10)'
---

Vyhodnocení požadavků migrace
=============================

V organizacích nasazujících službu RMS je třeba vytvořit plán migrace, který bude minimalizovat dobu odstavení serveru a umožní podporu scénářů údržby a upgradu serveru bez přerušení přístupu uživatelů k obsahu chráněnému službou RMS. Vzhledem k tomu, že služba RMS může využívat předchozí konfigurační databázi i databázi protokolování, měla by mít migrace služby RMS z jednoho serveru na jiný minimální vliv na organizaci za předpokladu, že bude provedena odpovídajícím způsobem. Scénář migrace předpokládá, že chcete použít existující databáze. V opačném případě by se totiž jednalo o novou instalaci služby RMS.

Pokud server RMS, který nahrazujete, používá hardwarový modul zabezpečení (například nCipher), je nutné přenést konfiguraci tohoto modulu na nový server ještě před tím, než na něm nainstalujete a zajistíte službu RMS. Popis postupu při této operaci naleznete v dokumentaci dodané s hardwarovým modulem zabezpečení.

Kroky před migrací:

-   Ověřte dostupnost databází.
-   Určete, který počítač bude použit k nové instalaci.

Chcete-li migrovat instalaci služby RMS, postupujte následujícím způsobem:

1.  Před zahájením migrace zálohujte všechny součásti, včetně databází, soukromých klíčů a stavu systému.
2.  Zajistěte, aby databáze předchozí instalace služby RMS byly uloženy na databázovém serveru, který je určen pro nové nasazení.
3.  Instalujte a zajistěte službu RMS na zvolených serverech a určete umístění databází.

Obvyklý scénář vyžadující migraci serveru RMS představuje přechod pilotního nasazení služby RMS do provozního prostředí. Další informace týkající se uvedeného scénáře využití získáte v této sadě dokumentace v části Migrace pilotního nasazení služby RMS do provozního prostředí tématu Nasazení služby RMS.
