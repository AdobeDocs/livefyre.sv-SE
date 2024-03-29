---
description: Skapa en sekretessförfrågan i Livefyre.
title: Skapa en sekretessförfrågan
exl-id: 117e1edb-becd-45f2-bfe5-12fb19ad01e0
translation-type: tm+mt
source-git-commit: a2449482e617939cfda7e367da34875bf187c4c9
workflow-type: tm+mt
source-wordcount: '609'
ht-degree: 0%

---

# Skapa en sekretessförfrågan{#create-a-privacy-request}

Skapa en sekretessförfrågan i Livefyre.

Ta bort alla data för en användare, generera en rapport över alla data för en användare och gör ändringar av anmälan eller avanmälan med den här processen.

Så här söker du efter och söker efter en användare och skapar en rapport om deras innehåll:

1. Gå till **[!UICONTROL Settings > Privacy]** och klicka sedan på **[!UICONTROL Create Request]**.

   ![](assets/privacypage1.png)

1. Fyll i informationen i **[!UICONTROL Submit Request]**-fönstret:

   * **[!UICONTROL Reference Id]**. Ange en identifierare som ska användas för framtida referens. Du kan till exempel lägga till text, ett biljettnummer, en URL, en e-postadress eller en annan sträng på upp till 255 tecken
   * **[!UICONTROL Type]**

      * **Åtkomst**. Samlar in alla tillgängliga data som är kopplade till kontot. Känsliga detaljer, till exempel lösenord eller sociala referenser, döljs eller utelämnas.

      * **Ta bort**. Ändrar eller döljer alla data som är associerade med kontot. **Om du väljer det här alternativet och klickar på Skicka kan du inte ångra eller avbryta den här åtgärden,  *och du kan inte heller återställa borttagna data.*** Om kontot tillhör en Livefyre Studio-användare bevaras vissa data för att upprätthålla integriteten i dina affärsposter.

         >[!IMPORTANT]
         >
         >Om du tar bort data för ett konto raderas eller förstörs data som är kopplade till kontot permanent. Du kan inte ångra den här åtgärden och inte heller återställa data efter att du har tagit bort den.

      * **Avanmäl dig**. Förhindrar Livefyre från att passivt samla in data eller innehåll från ett socialt konto via Streams eller Social Search. Avanmäl dig och avanmäl dig inte för registrerade användare
      * **Anmäl dig**. Återaktiverar Livefyre för att passivt samla in data eller innehåll från ett socialt konto som tidigare valt ut via Streams eller Social Search. Avanmäl dig och avanmäl dig inte för registrerade användare

      ![](assets/privacypage2.png)

   * **[!UICONTROL Identifier Type]** och  **[!UICONTROL Identifier]**

      * **[!UICONTROL User Account]**

         * Identifierar ett konto för en registrerad användare med det användar-ID som genereras av ditt användarhanteringssystem eller Livefyres Studio-användaridentifierare. Du kan också hitta användar-ID:t i användarinformationen för användaren i **Livefyre** **Användarinställningar** eller i informationen om innehållet i **resursbiblioteket** eller **appinnehåll**

         * Tillåtna värden: Alfanumerisk sträng på upp till 255 tecken. En e-postadress är inte en giltig inmatning
      * **[!UICONTROL Facebook User]**

         * Identifierar ett konto med ett numeriskt ID från Facebook. Den som gjorde begäran bör ange detta. Här finns instruktioner om hur du hittar det numeriska Facebook-id:t [här](https://www.facebook.com/help/1397933243846983?helpref=faq_content)
         * Tillåtna värden: 6-16 numeriska tecken
      * **[!UICONTROL Instagram User]**

         * Identifierar kontot med ett numeriskt ID från Instagram. Den som gjorde begäran bör ange detta. Du kan hitta instruktioner om hur du hittar det numeriska Instagram-id:t på ett Instagram-konto genom att söka online
         * Tillåtna värden: 5-16 numeriska tecken
      * **[!UICONTROL Twitter User]**

         * Identifierar ett konto med ett numeriskt ID från Twitter. Den person som begär ändringen av sekretessen bör tillhandahålla detta. Du kan hitta instruktioner om hur du hittar det numeriska Twitter-id:t för ett Twitter-konto genom att söka online
         * Tillåtna värden: 5-16 numeriska tecken
      * **[!UICONTROL YouTube User]**

         * Identifierar ett konto med ett numeriskt ID från YouTube. Den person som begär ändringen av sekretessen bör tillhandahålla detta. Här finns instruktioner om hur du hittar det numeriska YouTube-id:t på ett YouTube-konto [här](https://support.google.com/youtube/answer/3250431?hl=en)
         * Tillåtna värden: 5-16 numeriska tecken
      * **[!UICONTROL Generic Author]**

         * Identifierar ett konto med ett ID för Livefyre Author ID (JID). Använd det här alternativet för innehåll som har hämtats via RSS, Tumblr eller URL:er. Om du vill hitta det här ID:t söker du efter innehåll som har tilldelats författaren i **App Content** eller **Resursbibliotek** och väljer sedan ett objekt. ID är tillgängligt i **App Content** under **Info** eller i **Resursbibliotek** under **Författare** i avsnittet **Information**

         * Tillåtna värden: Alfanumerisk sträng på upp till 255 tecken

         ![](assets/privacypage3.png)








1. Klicka på **[!UICONTROL Finish]**.

   ![](assets/privacypage4.png)

1. (Endast för borttagningsbegäranden) Bekräfta att du vill ta bort all information för användaren.

   >[!IMPORTANT]
   >
   >Om du tar bort data för ett konto raderas eller förstörs data som är kopplade till kontot permanent. Du kan inte ångra den här åtgärden och inte heller återställa data efter att du har tagit bort den.
