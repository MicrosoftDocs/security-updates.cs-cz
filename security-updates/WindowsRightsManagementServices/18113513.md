---
TOCTitle: Odinstalace a zrušení zajištění služby RMS
Title: Odinstalace a zrušení zajištění služby RMS
ms:assetid: 'cae1ed5b-f716-41f0-8e14-7cbfef405331'
ms:contentKeyID: 18113513
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747753(v=WS.10)'
---

Odinstalace a zrušení zajištění služby RMS
==========================================

Službu RMS může být z různých důvodů nutné ze serveru odebrat. V případě serveru kořenové certifikace je prvním krokem zrušení zajištění služby RMS na serveru. Tuto operaci lze provést ze stránky **Globální správa** serveru, pro který chcete zrušit zajištění, klepnutím na možnost **Odebrat službu RMS z tohoto webu**. Před odinstalací služby RMS ze serveru správy licencí není třeba zrušit zajištění tohoto serveru.

> [!NOTE]
> Pokud zrušíte zajištění posledního serveru kořenové certifikace v doménové struktuře služby Active Directory, je ze služby Active Directory odebrán spojovací bod služby. Pokud před odinstalací služby RMS nezrušíte zajištění tohoto serveru, nelze zajistit nový server kořenové certifikace v dané doménové struktuře, dokud nebude spojovací bod služby ze služby Active Directory odebrán ručně. 

Další krok představuje odinstalace služby RMS.

V případě zrušení zajištění a odinstalace služby RMS ze samostatného serveru nebo z posledního serveru clusteru bude odstraněna databáze adresářových služeb. Konfigurační databáze a databáze protokolování odstraněny nebudou. Jestliže však na serveru provedete upgrade nebo přeinstalaci služby RMS, bude databáze protokolování přepsána novou databází.

Konfigurační databáze, databáze protokolování ani databáze adresářových služeb odstraněny nebudou ani v případě zrušení zajištění a odinstalace služby RMS ze serveru zařazeného do clusteru. Tabulka DRMS\_ClusterServer konfigurační databáze bude ovšem aktualizována a bude v ní zohledněno odebrání serveru z clusteru.

Další informace týkající se vyřazení serverů a souvisejících aspektů naleznete v tomto tématu v části [Vyřazení serverů](https://technet.microsoft.com/52005e2e-9563-4ba0-906c-3cc76f9c378f) uvedené již dříve.
