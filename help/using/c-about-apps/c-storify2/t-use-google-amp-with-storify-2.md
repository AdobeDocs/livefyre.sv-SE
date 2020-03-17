---
description: Använd Livefyre API:er för att lägga till Google AMP-funktioner på Storify 2-sidan för att hålla innehållet interaktivt och SEO-vänligt.
seo-description: Använd Livefyre API:er för att lägga till Google AMP-funktioner på Storify 2-sidan för att hålla innehållet interaktivt och SEO-vänligt.
seo-title: Använd Google AMP med Storify 2
solution: Experience Manager
title: Använd Google AMP med Storify 2
uuid: 40c9f083-7284-43ba-ae27-53b1ff9e3954
translation-type: tm+mt
source-git-commit: 67aeb3de964473b326c88c3a3f81ff48a6a12652

---


# Använd Google AMP med Storify 2{#use-google-amp-with-storify}

Använd Livefyre API:er för att lägga till Google AMP-funktioner på Storify 2-sidan för att hålla innehållet interaktivt och SEO-vänligt.

Om du vill använda Google AMP med Storify 2 måste du skapa en sida för Storify 2-appen med Google AMP-kod.

AMP-versionen av appen begär uppdateringar från den ursprungliga sidan (använd parametern **pollInterval** i API:t för **amp-live-list** för att ange intervall för uppdateringsbegäranden). För att se till att besökarna på din AMP-sida snabbt får det senaste innehållet bör du ha en låg TTL på Storify 2 AMP-sidorna.

Resurser som inte är bilder (till exempel videor) som ingår som inlägg i en Storify 2-app måste använda HTTPS enligt specifikationen i AMP-specifikationen. AMP-URL:er som använder Google Cloud Content Delivery Network (CDN) använder HTTPS.

Så här använder du Google AMP med Storify 2:

1. Skapa en AMP-validerad mall på din plats.
1. Använd en eller flera av följande Google AMP API:er för att anpassa din Google AMP-sida:
   1. [amp-iframe](https://www.ampproject.org/docs/reference/components/amp-iframe) för att anpassa Storify 2-visningen
   1. [amp-live-list](https://www.ampproject.org/docs/reference/components/amp-live-list) för att anpassa tidsintervallet för uppdateringar
   1. [amp-social-share](https://www.ampproject.org/docs/reference/components/amp-social-share) för att lägga till en knapp för delning via sociala medier
1. Inkludera innehållet på följande Storify 2 AMP-sida i CSS för Storify 2-sidan i <style amp-custom> tagg: [https://cdn.livefyre.com/libs/liveblog-v2-component/amp.min.css](https://cdn.livefyre.com/libs/liveblog-v2-component/amp.min.css)
1. Inkludera innehållet i följande Storify 2 AMP-kod i din Google AMP-mall: `https://api.livefyre.com/app-service/v4/bootstrap/{{APP_ID}}/amp` där {{APP_ID}} är program-ID för Storify 2-appen i Livefyre Studio.
   1. Den enda frågeparametern är **pollInterval**, som är det intervall i vilket programmet söker efter uppdateringar (anges i millisekunder).
   1. URL:en innehåller innehåll från de senaste inläggen (inklusive Tweets, videor osv.)
   1. Utgivarsidan måste hämta innehåll från den här URL:en så ofta du vill att Google AMP-sidan ska uppdateras.