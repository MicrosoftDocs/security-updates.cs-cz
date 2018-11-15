---
TOCTitle: Registrace spojovacího bodu služby
Title: Registrace spojovacího bodu služby
ms:assetid: '630cc3c3-9ed9-4423-8874-cbaceb43b353'
ms:contentKeyID: 18113305
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc720283(v=WS.10)'
---

Registrace spojovacího bodu služby
==================================

Registrace spojovacího bodu služby
----------------------------------

Pokud provádíte registraci spojovacího bodu služby ze serveru RMS v subdoméně, může se zobrazit chybová zpráva s upozorněním, že se registrace spojovacího bodu služby nezdařila. V mnoha případech je registrace úspěšná, ale nejdříve je provedena v doméně nejvyšší úrovně a replikace do subdomény, ve které server RMS zjišťuje objekt spojovacího bodu služby, trvá určitou dobu. Po replikaci spojovacího bod služby na všechny servery globálního katalogu v doménové struktuře se již zpráva nezobrazí. Pokud se tato zpráva zobrazí, je nutné před vlastním odstraňováním tohoto problému počkat přiměřenou dobu, zda se nevyřeší sám.

#### Registrace spojovacího bodu služby

1.  Přihlaste se k serveru, na kterém chcete zaregistrovat spojovací bod služby. Použijte doménový účet s dostatečnými oprávněními pro vytvoření kontejnerového objektu pod kontejnerem služeb v rámci kontejneru konfigurace doménové struktury Active Directory. Příkladem účtu s potřebnými oprávněními je předdefinovaná skupina zabezpečení **Enterprise Admins**.

2.  Otevřete stránku **Globální správa** a poté klepněte na odkaz **Spravovat službu RMS na tomto webu**.

3.  Na stránce **Domovská stránka pro správu** klepněte na odkaz **Spojovací bod služby RMS**.

4.  Na stránce **spojovacího bodu služby RMS** klepněte na tlačítko **Registrovat adresu URL**.
