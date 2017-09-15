---
TOCTitle: Vyřazení serverů
Title: Vyřazení serverů
ms:assetid: '52005e2e-9563-4ba0-906c-3cc76f9c378f'
ms:contentKeyID: 18113316
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747568(v=WS.10)'
---

Vyřazení serverů
================

V některých případech může být nutné vyřadit server RMS. Může se například jednat o následující situace:

-   Potíže se zařízením nebo upgrady, jejichž důsledkem je nahrazení některých serverů.
-   Snížení provozu licencování a publikování, v jehož důsledku jsou některé servery vyřazeny z provozu.
-   Zákonné požadavky na odebrání serverů z určitých míst, takže je z provozu vyřazen celý cluster.
-   Sloučení nebo prodej několika částí organizace, což má za následek převod majetku.
-   Sloučení celé organizace s jinou organizací, která také používá službu RMS, čímž se obě instalace služby RMS stanou nadbytečné.

Před vyřazením serveru by měly být vytvořeny záložní kopie všech databází služby RMS používané serverem, zejména konfigurační databáze. Další informace o zálohování databází najdete v této sadě dokumentace v části Zálohování a obnovení systému služby RMS tématu Plánování nasazení služby RMS. .

Po vytvoření záložních kopií databází můžete server odebrat. Průběh odebírání serveru služby RMS záleží na roli serveru a topologii instalace služby RMS:

-   **Odebrání jednoho serveru z clusteru**. Pokud je vyřazovaný server RMS zařazen do clusteru s dalšími servery RMS, které jsou stále aktivní a vyžadované, představuje odebrání jednoho serveru RMS z clusteru zrušení zajištění služby RMS na tomto serveru, její odinstalace, odebrání hardwaru z clusteru a archivace databází.
    | ![](images/Cc747568.note(WS.10).gif)Poznámka                                                                                                  |
    |----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Zajištění je nutné před odinstalací služby RMS zrušit pouze u serverů zařazených do clusteru kořenové certifikace. Pro servery správy licencí není tento postup vyžadován. |

-   **Vyřazení samostatného serveru**. Pokud je vyřazovaný server RMS samostatný (tj. není součástí clusteru obsahujícího několik serverů) a je třeba jej nahradit novým serverem, proveďte následující postup: Zrušte zajištění a odinstalujte existující server RMS, odeberte jej ze sítě a pak okamžitě nainstalujte službu RMS na nový server a zajistěte ji. Nakonfigurujte nový server RMS tak, aby používal stejnou adresu URL a konfigurační databázi jako původní server. Uvědomte si, že dokud není nový server nainstalován a zajištěn, uživatelé nemohou používat obsah publikovaný vyřazeným serverem.
    | ![](images/Cc747568.Important(WS.10).gif)Důležité informace                                                                                                                                                                                                                |
    |---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Pokud vyřazovaný server RMS používá hardwarový modul zabezpečení, je třeba na nový server přenést příslušné prostředky zabezpečení ještě před tím, než na něj nainstalujete službu RMS a zajistíte ji. Popis postupu při této operaci naleznete v dokumentaci dodané s hardwarovým modulem zabezpečení. |

-   **Nahrazení instalace služby RMS jinou existující instalací služby RMS**. V některých případech je třeba vyřadit instalaci služby RMS a nahradit ji jinou existující instalací, například v případě sloučení dvou společností, kdy službu RMS používají obě dvě.

Pokud zrušíte zajištění serveru a odinstalujete jej, je server odebrán z tabulky ClusterServer v konfigurační databázi a ze serveru SQL Server je odstraněna databáze adresářových služeb. Postup při zrušení zajištění a odinstalaci služby RMS naleznete v tomto tématu později v části [Zrušení zajištění služby RMS](https://technet.microsoft.com/9fa63daa-5fb9-4afd-8371-b38248619857) a [Odinstalace služby RMS](https://technet.microsoft.com/885e3b4f-ea32-466f-9f7f-d8440b0f7c28).
