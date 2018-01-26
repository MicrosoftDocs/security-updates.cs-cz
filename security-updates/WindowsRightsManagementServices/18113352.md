---
TOCTitle: Provádění změn v konfigurační databázi
Title: Provádění změn v konfigurační databázi
ms:assetid: '6a7bec73-09e4-4060-b551-5990836df4bc'
ms:contentKeyID: 18113352
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747606(v=WS.10)'
---

Provádění změn v konfigurační databázi
======================================

Změny konfigurace provedené pomocí webu pro správu se promítají do konfigurační databáze pro server nebo cluster. Doporučuje se neprovádět změny dat ručně přímo v konfigurační databázi, ale raději měnit nastavení konfigurace pomocí webu pro správu. Existují však dvě situace, které pravděpodobně budou ruční změny v databázi vyžadovat:

-   **Přemístění databáze protokolování na jiný server.** Ve výchozím nastavení je databáze protokolování nainstalována na stejný server jako konfigurační databáze. Pokud se rozhodnete přemístit databázi protokolování na jiný server, je třeba změnit konfigurační databázi tak, aby odkazovala na její nové umístění. Další informace týkající se přemístění databáze protokolování, včetně postupu při aktualizaci nového umístění v konfigurační databázi, naleznete v tomto tématu v části [Přemístění databáze protokolování](https://technet.microsoft.com/34ea8045-dc94-422e-9601-29927cfc1534) uvedené již dříve.

-   **Odebrání klíčů uživatelů přidružených k certifikátům účtu práv**. Pokud pomocí webu pro správu odeberete uživatelský účet ze služby Active Directory nebo vyloučíte či odvoláte certifikát účtu práv, nebudou z konfigurační databáze odebrány klíče uživatelů přidružené k certifikátu účtu práv. Neaktivní klíče uživatelů je třeba z konfigurační databáze odebrat ručně. Důvodem je zabezpečení databáze, ale také podpora sledování počtu licencí klientského přístupu (licencí CAL). Další informace o odebrání klíčů uživatelů z konfigurační databáze naleznete v tomto tématu v části [Odstranění uživatelských účtů](https://technet.microsoft.com/bf73b141-d4d1-4807-a773-3aaff58b0db6) uvedené již dříve. Další informace týkající se sledování licencí CAL naleznete v tomto tématu v části [Sledování certifikátů účtů práv](https://technet.microsoft.com/5bb0f3cf-fc44-4e60-a93f-c789d6f8a902) uvedené již dříve.

Pokud potřebujete provést změny přímo v konfigurační databázi, obraťte se na správce databázového serveru.
