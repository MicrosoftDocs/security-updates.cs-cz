---
TOCTitle: Vyřazení šablon zásad práv
Title: Vyřazení šablon zásad práv
ms:assetid: '32bf98c7-edda-4507-a4b8-4c11bddd6e60'
ms:contentKeyID: 18113254
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc720239(v=WS.10)'
---

Vyřazení šablon zásad práv
==========================

Chcete-li šablonu zásad práv vyřadit, odstraňte ji. Tento postup je popsán v tomto tématu později v části [Odstranění šablony zásad práv](https://technet.microsoft.com/9c9a1496-cf55-4c65-a4c6-9fe245edce00). Obvykle by však šablony zásad práv odstraňovány být neměly. Pokud chcete šablonu zásad práv vyřadit, měly by být odstraněny všechny její kopie z počítačů uživatelů. Důvodem tohoto postupu je skutečnost, že pokud autor použije šablonu zásad práv k publikaci obsahu, je na server RMS odeslán požadavek. Služba RMS bude na tento požadavek reagovat pomocí kopie šablony zásad práv uložené v databázi. Pokud šablona v databázi neexistuje, požadavek bude neúspěšný.

> [!NOTE]
> Jednou z možností, jak vyřazení šablony zásad práv provést, je vytvoření skriptu, jehož prostřednictvím je šablona zásad práv odstraněna ze všech počítačů uživatelů. 
