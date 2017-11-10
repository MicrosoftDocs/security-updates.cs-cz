---
TOCTitle: 'Instalace součásti Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) pro poskytování databázové podpory službě RMS'
Title: 'Instalace součásti Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) pro poskytování databázové podpory službě RMS'
ms:assetid: 'c9b9cd08-98c4-424f-b3fc-d685f57c002e'
ms:contentKeyID: 18113435
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747667(v=WS.10)'
---

Instalace součásti Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) pro poskytování databázové podpory službě RMS
=====================================================================================================================

Instalace součásti Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) pro poskytování databázové podpory službě RMS
---------------------------------------------------------------------------------------------------------------------

#### Instalace součásti Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) pro poskytování databázové podpory službě RMS

1.  Přihlaste se pomocí doménového účtu, který je členem místní skupiny Administrators na serveru určeném k instalaci součásti Microsoft SQL Server Desktop Engine (MSDE 2000).

2.  Stáhněte součást MSDE 2000 z [webu společnosti Microsoft](http://www.microsoft.com/) (http://www.microsoft.com/) a uložte ji do počítače.

3.  Spuštěním souboru MSDE2000A.exe extrahujte instalační balíček součásti MSDE 2000 do složky. Ve výchozím nastavení má tato složka název MSDERelA, můžete však určit jiný název.

4.  Spusťte příkazový řádek a přejděte do umístění, kam jste uložili instalaci součásti MSDE 2000.

5.  Nainstalujte součást Microsoft SQL Server 2000 Desktop Engine se správnou konfigurací pro spolupráci se službou RMS zadáním následujícího příkazu, ve kterém nahradíte text *heslo* silným heslem podle vlastního výběru:

    **Setup.exe /i setup\\sqlrun10.msi INSTANCENAME=RMS DISABLEAGENTSTARTUP=1 SAPWD***=heslo*

    > [!IMPORTANT]
    > Po instalaci je třeba službu MSDE spustit. Službu můžete spustit pomocí panelu **Služby** v **Ovládacích panelech**. Doporučujeme nastavit automatické spuštění této služby, aby byla při spuštění služby RMS vždy zajištěna dostupnost databáze součásti MSDE. 

Nezajišťujte službu RMS na serveru, dokud není nainstalován databázový systém, který bude poskytovat podporu konfigurační databázi služby RMS.

Součást Microsoft SQL Server Desktop Engine je vhodné používat k podpoře databází služby RMS pouze v testovacím prostředí, protože neobsahuje nástroje nezbytné ke komplexnímu provozu a podpoře databáze v rámci celého podniku. Součást MSDE nepodporuje vzdálenou síť, a proto je zároveň nutné nainstalovat ji na stejný server jako službu RMS, přičemž není možné do clusteru služby RMS přidávat další servery RMS. V podmínkách používání součásti Microsoft SQL Server Desktop Engine je navíc uvedeno, že pro obsluhu databáze Microsoft SQL Server Desktop Engine nelze použít klientské nástroje serveru SQL Server. Toto omezení neumožňuje zálohování a obnovování konfigurační databáze služby RMS, prohlížení informací protokolování ani přímou změnu dat uložených v konfigurační databázi.
