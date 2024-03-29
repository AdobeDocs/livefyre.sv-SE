---
title: Anpassningar av bildband
description: Anpassningar av bildband
exl-id: 2765699f-7adc-4b17-acfb-ef594ff65e89
translation-type: tm+mt
source-git-commit: a2449482e617939cfda7e367da34875bf187c4c9
workflow-type: tm+mt
source-wordcount: '521'
ht-degree: 0%

---

# Anpassningar av bildband{#filmstrip-customizations}

Alla program använder alternativen **[!UICONTROL Style]** och **[!UICONTROL Config]** i **[!UICONTROL App Designer]**. Mer information om standardalternativen **[!UICONTROL Style]** och **[!UICONTROL Config]** för alla program i **[!UICONTROL App Designer.]** finns i Anpassa appar

Du kan anpassa bildbandet med följande ytterligare alternativ i App Designer:

* **[!UICONTROL Content fit]**. Välj **[!UICONTROL crop]** om du vill beskära innehållet för att fylla kortet eller **[!UICONTROL Aspect Ratio]** om du vill visa en hel bild på kortet, oavsett om det fyller hela kortet eller inte.
* **[!UICONTROL Tile Size]**. Ange rutornas storlek i pixlar.
* **[!UICONTROL Show Notifications]**. Välj om ett meddelande ska visas för nytt innehåll när det direktuppspelas i bildbandsappen.
* **[!UICONTROL Require rights]**. Aktivera det här alternativet om du bara vill visa innehåll med statusen Beviljad för behörighet.
* **[!UICONTROL Hide social branding when rights granted]** Aktivera det här alternativet om du vill ta bort logotypen för det ursprungliga sociala medienätverket (Twitter eller Instagram) när rättigheter beviljas för ett visst innehåll.
* **[!UICONTROL Call-to-action button]** Du kan använda knappen för att ringa upp med en produktkatalog för att dirigera användare till en produkt eller till din plats för ytterligare åtgärder.

   * **[!UICONTROL Call-to-action button]** Växla till om du vill visa knappen för att ringa till åtgärd.
   * **[!UICONTROL Require rights to display products]** Aktivera det här alternativet om du vill kräva att innehållsägaren har beviljat rättigheter för innehållet innan en knapp för att ringa upp visas för innehållet.

      >[!NOTE]
      >
      >Innehållet visas även om rättigheter inte har beviljats för innehållet, men knappen för att ringa upp till åtgärd visas inte med innehållet om inte rättigheter för innehållet har beviljats.

   * **[!UICONTROL Show call-to-action in tile]**. Välj om du vill visa knappen för att ringa upp till åtgärd på en bildbandsplatta i stället för att bara visa knappen för att ringa upp när besökaren klickar på ett kort och öppnar innehållet i ett större fönster.
   * **[!UICONTROL Call-to-action indication text]** Den text som ska visas för att uppmana användaren att klicka på kortet för att öppna modalt anrop till åtgärd.
   * **[!UICONTROL Call-to-action header text]** De ord som ska visas i rubriken ovanför knappen för att ringa upp till åtgärd i det modala innehållet. Standardtexten är&quot;Handla dessa produkter:&quot;.
   * **[!UICONTROL Call-to-action button text]** De ord som ska visas i knappen för att ringa upp till åtgärd i det modala innehållet. Standardtexten är&quot;Köp nu:&quot;.
   * **[!UICONTROL Product display options]** Välj om du vill visa  **[!UICONTROL Photo]** och  **[!UICONTROL Product name]** med knappen för att ringa upp.

      >[!NOTE]
      >
      >Både Foto- och produktnamnsknapparna markerar blått när de är aktiverade.

   * **[!UICONTROL Product URL referral tracking]** Växla till om du vill spåra hänvisningar från den här appen till den associerade produktsidan.
   * **[!UICONTROL Referral tracking key-value pairs]** Lägg till parametrar för att ytterligare specificera hänvisningsspårningen från ditt appinnehåll till den associerade produktsidan.

* **[!UICONTROL Embed App in multiple pages]**.

   * **[!UICONTROL Filter UGC by Product ID]**. Välj det här alternativet om du vill skapa en app för flera produktsidor. Filtrera produktspecifik UGC till appen för varje produktsida. Du kan markera en eller flera mappar som du vill associera specifika samlingar med appen.
   * **[!UICONTROL Select product folders]**. Välj de produktmappar på den översta nivån som ska användas för att filtrera UGC. Använd CTRL/Cmd + klicka för att markera flera mappar. Livefyre använder mappen för att avgöra vilka produkter i den mappen som ska visas i appen på olika sidor.
   * **[!UICONTROL Show related content]**. Växla detta för att visa innehåll som publicerats till appen, men som taggats med ett annat produkt-ID. När det produktspecifika innehållet för appen visas visar Livefyre innehåll för andra produkter och innehåll som inte är kopplat till en produkt. Livefyre prioriterar innehållet med samma produkt-ID först, sedan innehåll som publiceras till appen med andra produkt-ID:n och sedan innehåll som publiceras till appen utan produkt-ID:n.

Se [Bildbandsalternativ](/help/implementation/c-getting-started/c-implementation-process/c-using-livefyre.js-to-create-customize-and-use-apps-on-your-site.md) för mer information om hur du anpassar en bildband med Livefyre.js.
