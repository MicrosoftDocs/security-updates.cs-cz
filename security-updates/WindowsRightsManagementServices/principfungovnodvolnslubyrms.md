---
TOCTitle: Princip fungování odvolání služby RMS
Title: Princip fungování odvolání služby RMS
ms:assetid: '469e3938-a59b-4c92-9779-ead64e724d00'
ms:contentKeyID: 18113282
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc720263(v=WS.10)'
---

Princip fungování odvolání služby RMS
=====================================

Odvolání znemožňuje vazbu (proces umožňující uživateli používat obsah), pokud se odvolaná entita nachází v požadavku na vazbu. Odvolání je implementováno pomocí seznamů odvolání distribuovaných do klientských počítačů. Tyto seznamy mají formu podepsaných souborů XrML, v nichž je uveden obsah, aplikace, uživatelé nebo další zaregistrované objekty, které byly odvolány objektem, který seznam vydává.

Při každém pokusu uživatele o využití chráněného obsahu odešle příslušná aplikace s podporou služby RMS klientovi RMS požadavek na odpovídající právo v požadavku na vazbu. Pokud se uživatel pokusí například o otevření souboru, aplikace požaduje oprávnění k zobrazení (View) umožňující otevření souboru. Pokud se uživatel pokusí o úpravu souboru, aplikace požaduje oprávnění k úpravě (Edit).

Při zpracování požadavku na vazbu provádí klient RMS následující kroky:

1.  Vyhodnotí licenci k použití pro všechny požadavky seznamu odvolání.
2.  Pokud licence k použití vyžaduje odvolání, klientská komponenta ověří, zda je určený seznam odvolání k dispozici, zda je registrován a zda je aktuální vzhledem k intervalu aktualizace určenému v licenci k použití, či nikoli.
3.  Ověří, zda je zaregistrovaný objekt, který podepsal seznam odvolání, uveden v licenci k použití jako zaregistrovaný objekt, který povolil odejmutí licence.
4.  Proběhnou-li tyto kontroly úspěšně, určí pak klientská součást, zda byly všechny zaregistrované objekty obsažené v původním požadavku na vazbu odvolány, či nikoli. Pokud ano, bude požadavek na vazbu odmítnut.

Seznamy odvolání může klientským počítačům distribuovat správce nebo je může do počítače stáhnout aplikace s podporou služby RMS v okamžiku, kdy to vyžaduje licence k použití. Pokud je seznam odvolání použit ke svázání části obsahu, je zaregistrován a může být po dobu otevření dané aplikace použit pro požadavky na vazbu u dalších licencí k použití. Po ukončení činnosti aplikace je registrace seznamu odvolání zrušena.

V následujícím diagramu je zobrazen proces vazby se znázorněným postupem při odvolání.

![](images/Cc720263.81aa2d70-d261-49ad-b446-96a2eddba1a5(WS.10).gif)

Odvolání je nepovinné. Správce RMS může odvolání požadovat tím, že je zadá v jedné nebo více šablonách zásad práv dané organizace. Je-li požadováno odvolání, nelze pro licenci vytvořit vazbu, pokud není k dispozici požadovaný seznam odvolání, který je registrovaný v počítači daného uživatele a který není starší než interval aktualizace určený v licenci k použití.

Je však důležité poznamenat, že odvolání může pro danou licenci k použití nabýt platnost i tehdy, když je licence k použití nevyžaduje. Odvolání nabude platnost pokaždé, když vydavatel kteréhokoli certifikátu v řetězci důvěryhodnosti, který je obsažen v požadavku na vazbu, vydal seznam odvolání registrovaný v klientském počítači. V tomto scénáři je seznam odvolání použit při zpracování požadavků na vazbu i tehdy, když příslušné licence k použití nevyžadují odvolání. Tento postup platí do doby, než je aplikace s podporou služby RMS ukončena, protože tím dojde ke zrušení registrace seznamu odvolání.

Jestliže uživatel například chce využít část obsahu, jehož licence k použití vydaná entitou A vyžaduje seznam odvolání vydaný stejnou entitou, získá aplikace s podporou služby RMS seznam odvolání z adresy URL zadané v dané licenci k použití a potom jej zaregistruje. Při zpracování požadavku na vazbu, zjišťuje klient RMS v uvedeném seznamu možná odvolání.

Aplikace s podporou služby RMS zůstane otevřená a uživatel bude chtít využít další část obsahu, jehož licence k použití byla také vydána entitou A. Přestože tato licence k použití neobsahuje podmínku odvolání, je seznam odvolání entity A stále zaregistrován v počítači daného uživatele. V této situaci bude klientská součást kontrolovat seznam odvolání před zpracováním požadavku na vazbu.

Uživatel se poté pokusí o použití části obsahu, jejíž licence k použití byla vydána entitou C. Tato licence k použití neobsahuje podmínku odvolání. Vzhledem k tomu, že jediným registrovaným seznamem odvolání v klientském počítači je seznam odvolání vydaný entitou A a entita A není v řetězci důvěryhodnosti pro licenci k použití, nebude pro vazbu uplatněno žádné odvolání.

Nakonec uživatel aplikaci s podporou služby RMS zavře a později znovu otevře druhou část obsahu, která neobsahovala podmínku odvolání. Vzhledem k tomu, že po ukončení aplikace došlo ke zrušení registrace seznamu odvolání vydaného entitou A, nebude jej klient RMS při zpracování požadavku na vazbu kontrolovat.
