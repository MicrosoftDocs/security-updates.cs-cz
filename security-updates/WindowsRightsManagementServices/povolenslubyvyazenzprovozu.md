---
TOCTitle: Povolení služby vyřazení z provozu
Title: Povolení služby vyřazení z provozu
ms:assetid: '45226e85-b50d-41cc-aca7-0f603f8509d5'
ms:contentKeyID: 18113263
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc720261(v=WS.10)'
---

Povolení služby vyřazení z provozu
==================================

Vyřazení systému služby RMS z provozu vyžaduje zajištění ochrany všech publikovaných informací prostřednictvím soukromého klíče. Tento soukromý klíč je uložen v konfigurační databázi (s šifrováním pomocí rozhraní Data Protection API – DPAPI) a je založen na hesle, které bylo zadáno při procesu zajišťování. Pokud je soukromý klíč služby RMS uložen v hardwarovém modulu zabezpečení (HSM), bude soukromý klíč uložen v modulu HSM, nikoli v konfigurační databázi.

> [!CAUTION]
> Před vyřazením systému RMS z provozu se ujistěte, zda znáte heslo soukromého klíče. Jestliže toto heslo neznáte, je nutné před vyřazením serveru RMS z provozu heslo soukromého klíče obnovit. 

Prvním krokem při odebírání systému RMS je vyřazení serverů v clusteru z provozu. Vzhledem k tomu, že vyřazení z provozu je funkcí správy licencí, lze server v clusteru vyhrazeném pro správu licencí služby RMS s dílčím zápisem vyřadit z provozu, aniž by to mělo vliv na kořenový cluster služby RMS nebo jakýkoli jiný cluster vyhrazený pro správu licencí této služby s dílčím zápisem. Je proto nutné samostatně vyřadit z provozu kořenový cluster služby RMS a jakékoli další clustery vyhrazené pro správu licencí, protože každý cluster vyhrazený pro správu licencí obsahuje svůj vlastní soukromý klíč používaný pro vytváření licencí k publikování.

Chcete-li službu vyřazení z provozu povolit, postupujte následujícím způsobem:

1.  Otevřete web pro správu služby RMS v systému Windows.
2.  Klepněte na možnost **Spravovat službu RMS** a potom na možnost **Nastavení zabezpečení**.
3.  Zaškrtněte políčko **Povolit vyřazení instalace RMS z provozu**.
4.  Jakmile se zobrazí dialogové okno s výzvou k potvrzení procesu vyřazení z provozu, klepněte na tlačítko **OK**.

Po vyřazení serveru z provozu nelze obnovit standardní konfiguraci služby RMS. Tento proces je nevratný.

Po vyřazení služby RMS z provozu je třeba před instalací jiné instance služby RMS tuto službu zcela odebrat pomocí ovládacího panelu **Přidat nebo odebrat programy**.
