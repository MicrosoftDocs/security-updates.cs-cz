---
TOCTitle: Práce se skupinou superuživatelů
Title: Práce se skupinou superuživatelů
ms:assetid: '0febcb3e-7124-4e51-971a-1013b928d33b'
ms:contentKeyID: 18113214
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc720198(v=WS.10)'
---

Práce se skupinou superuživatelů
================================

Při zajišťování vytvoří služba RMS speciální skupinu superuživatelů, která má právo úplného řízení veškerého obsahu chráněného správou přístupových práv. Členům skupiny superuživatelů jsou udělena úplná práva vlastníků ve všech licencích k použití vydaných serverem nebo clusterem RMS, u kterých je tato skupina nakonfigurována. To znamená, že členové této skupiny mohou dešifrovat libovolné soubory s chráněným obsahem a odstraňovat jejich ochranu. Člen této skupiny může například odstranit ochranu ze souborů publikovaných bývalým zaměstnancem, aby mohl dané soubory publikovat a spravovat nový vlastník.

Ve výchozím nastavení neobsahuje skupina superuživatelů žádné členy, ani správce. Při práci s webem pro správu můžete určit skupinu zabezpečení služby Active Directory, která má být použita jako skupina superuživatelů pro službu RMS. K tomuto účelu můžete použít stávající skupinu služby Active Directory nebo vytvořit novou skupinu. Skupina musí existovat ve stejné doménové struktuře služby Active Directory jako instalace služby RMS. Všem uživatelským účtům, které jsou členy skupiny určené jako skupina superuživatelů služby RMS, je automaticky uděleno oprávnění skupiny superuživatelů.

Další informace týkající se určení skupiny superuživatelů pro službu RMS získáte v tomto tématu později v části [Nastavení skupiny superuživatelů](https://technet.microsoft.com/f2ef847e-2824-471f-9079-5c343094aba8).

> [!NOTE]
> Před označením skupiny jako skupiny superuživatelů služby RMS musí tato skupina existovat ve stejné doménové struktuře služby Active Directory jako instalace služby RMS. Vlastnosti dané skupiny musí obsahovat e-mailovou adresu včetně úplného názvu domény (názvu FQDN), který odpovídá názvu účtu. E-mailová adresa by měla být zadána ve formátu *název\_skupiny*@*název\_domény*. 
