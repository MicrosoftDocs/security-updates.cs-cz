---
TOCTitle: Vytvoření účtu služby RMS
Title: Vytvoření účtu služby RMS
ms:assetid: '6eb38729-f0f0-431a-bc8c-17102cf175d8'
ms:contentKeyID: 18113314
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747546(v=WS.10)'
---

Vytvoření účtu služby RMS
=========================

V průběhu instalace vytvoří služba RMS v místním počítači skupinu zabezpečení **RMS Service Group** a udělí jí odpovídající oprávnění ke všem prostředkům nezbytným pro správný provoz služby RMS.

Po zajištění služby RMS na serveru zadáte uživatelský účet jako účet služby RMS. Zadaný účet se stane členem skupiny RMS Service Group a jsou mu udělena oprávnění této skupiny. Při běžném provozu je ve většině případů služba RMS spuštěna pod účtem služby RMS.

| ![](images/Cc747546.note(WS.10).gif)Poznámka                 |
|-------------------------------------------------------------------------------------------|
| Jako účet služby RMS nelze použít doménový účet, který byl použit k instalaci služby RMS. |

Z důvodů zabezpečení se důrazně doporučuje vytvořit zvláštní uživatelský účet a používat jej výhradně jako účet služby RMS a k žádným jiným účelům. Tomuto účtu byste zároveň neměli udělovat žádná další oprávnění.

| ![](images/Cc747546.Important(WS.10).gif)Důležité informace    |
|---------------------------------------------------------------------------------------------|
| Tento zvláštní uživatelský účet byste měli vytvořit před instalací a zajištěním služby RMS. |

Další informace o oprávněních udělených skupině RMS Service Group a účtech, v rámci kterých je služba RMS spuštěna, získáte v této sadě dokumentace v části Model zabezpečení služby RMS tématu Technické informace týkající se služby RMS.
