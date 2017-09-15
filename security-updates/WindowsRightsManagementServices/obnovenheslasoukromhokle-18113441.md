---
TOCTitle: Obnovení hesla soukromého klíče
Title: Obnovení hesla soukromého klíče
ms:assetid: 'ceba927e-a7fd-4b06-bb70-5e5d9d6d099c'
ms:contentKeyID: 18113441
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747675(v=WS.10)'
---

Obnovení hesla soukromého klíče
===============================

Při zajišťování serveru je nutné vybrat metodu ochrany soukromého klíče služby RMS. Pokud jste vybrali výchozí možnost použití softwarové ochrany soukromého klíče, určili jste silné heslo, které bylo použito k zašifrování soukromého klíče serveru v konfigurační databázi. V případě ztráty nebo zapomenutí hesla je může člen skupiny superuživatelů obnovit. Postup při obnovení hesla naleznete v tomto tématu později v části [Vytvoření nového hesla soukromého klíče](https://technet.microsoft.com/f71df255-fe19-4e07-810e-87309a5e8e88).

Používáte-li službu RMS v clusterovaném prostředí, je třeba obnovit soukromý klíč na každém koncovém serveru RMS v dané instalaci. Pokud jej neobnovíte, nebudou tyto servery fungovat, protože nebudou moci dešifrovat klíč serveru v konfigurační databázi.

Další informace týkající se silných hesel naleznete v Centru pro nápovědu a odbornou pomoc systému Windows Server 2003.
