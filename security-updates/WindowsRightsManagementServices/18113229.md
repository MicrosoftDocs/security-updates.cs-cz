---
TOCTitle: Aplikace s podporou služby RMS
Title: Aplikace s podporou služby RMS
ms:assetid: '30bb5565-81d3-43d9-a64d-cf0c5b990712'
ms:contentKeyID: 18113229
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc720231(v=WS.10)'
---

Aplikace s podporou služby RMS
==============================

Chtějí-li uživatelé vytvořit nebo využít obsah chráněný službou RMS, musí si nainstalovat aplikaci s podporou služby RMS, které je věnováno toto téma. Dále je nutné nainstalovat klienta RMS a aktivovat počítače, se kterými uživatelé pracují. Další informace získáte v tomto tématu později v částech [Klient RMS](https://technet.microsoft.com/03294fa2-8350-430d-b4b0-03d5169937c2) a [Aktivace počítače RMS](https://technet.microsoft.com/09a0d631-9860-477f-9d10-df61b3bfe125).

Aplikace s podporou služby RMS umožňují autorům obsahu připojit k souborům, které vytvářejí, práva využití v podobě licencí k publikování. Tímto způsobem lze řídit způsob využití daného obsahu. Uvedené aplikace zároveň zpracovávají šifrované informace souboru a umožňují uživatelům využít daný obsah podle oprávnění definovaných v licenci k publikování.

Pomocí sady SDK klienta Služby správy přístupových práv mohou vývojáři vytvořit aplikace s podporou služby RMS, které licencují, publikují a využívají obsah chráněný uvedenou službou. Aplikace s podporou služby RMS lze vytvořit pro počítače se systémem Microsoft® Windows® 98 Druhé vydání nebo vyšší.

Sada SDK klienta Služby správy přístupových práv vývojářům umožňuje vytvářet také serverové aplikace s podporou služby RMS. Tyto aplikace mohou obsah publikovat ale nikoli využívat.

Uživatelé, kteří nemají k dispozici další aplikaci s podporou služby RMS pro využití obsahu chráněného touto službou v e-mailech a na webových stránkách, mohou získat a používat doplněk Správa práv pro aplikaci Microsoft® Internet Explorer. Zákazníci používající aplikaci Outlook Web Access (OWA) mohou například pomocí doplňku Správa práv pro aplikaci Internet Explorer využívat e-mailové zprávy chráněné službou RMS.

Doplněk Správa práv pro aplikaci Internet Explorer můžete stáhnout z [webu společnosti Microsoft](http://go.microsoft.com/fwlink/?linkid=14450) (http://go.microsoft.com/fwlink/?LinkId=14450).

> [!NOTE]
> Pokud uvedený doplněk používáte v systému s aktualizací Windows XP Service Pack 2, může rozšířená konfigurace zabezpečení způsobit určité potíže s kompatibilitou aplikace. 

Jestliže adresa URL připojení k extranetu pro každou doménu v organizaci není přidána na weby místního intranetu v aplikaci Internet Explorer, bude se uživatelům využívajícím doplněk Správa práv pro aplikaci Internet Explorer opakovaně zobrazovat zpráva s dotazem, zda se opravdu chtějí k těmto webům připojit. Nesprávná odpověď na tyto zprávy by mohla způsobit, že klient RMS získá pro účet daného uživatele nový certifikát účtu práv.

Chcete-li v organizaci nastavit uvedené weby správně, zadejte pomocí skriptu požadované adresy URL do registru jako součást zóny Místní intranet. Zóna Místní intranet poskytuje ve výchozím nastavení dostatečně vysokou úroveň zabezpečení, takže se uvedené zprávy nezobrazí.
