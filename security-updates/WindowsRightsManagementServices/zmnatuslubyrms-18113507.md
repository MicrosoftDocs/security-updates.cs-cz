---
TOCTitle: Změna účtu služby RMS
Title: Změna účtu služby RMS
ms:assetid: 'f257d66d-b823-41e4-bcb7-7c90eb295238'
ms:contentKeyID: 18113507
ms:mtpsurl: 'https://technet.microsoft.com/cs-cz/library/Cc747736(v=WS.10)'
---

Změna účtu služby RMS
=====================

V průběhu instalace vytvoří služba RMS v místním počítači skupinu RMS Service Group a udělí jí odpovídající oprávnění ke všem prostředkům nezbytným pro správný provoz služby RMS. Při zajištění služby RMS na serveru je účet služby RMS definován pomocí účtu domény. Jako účet služby RMS nelze použít doménový účet, který jste použili k instalaci služby RMS. Tento účet se stane členem skupiny RMS Service Group a jsou mu udělena oprávnění této skupiny. Při běžném provozu je služba RMS spuštěna pod účtem služby RMS.

Účet služby RMS je možné kdykoli změnit. Pokud účet změníte, bude předchozí zadaný účet automaticky ze skupiny RMS Service Group odebrán a jejím členem se stane nový účet.

> [!IMPORTANT]
> Z bezpečnostních důvodů je doporučeno vytvořit pro účet služby RMS zvláštní uživatelský účet a používat jej pouze k tomuto účelu. Tomuto účtu byste zároveň neměli udělovat žádná další oprávnění. 

> [!NOTE]
> Účtem služby RMS nemůže být účet domény použitý k instalaci služby RMS s aktualizací Service Pack 1. 
