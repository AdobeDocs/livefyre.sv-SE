---
description: Versionsinformation för 15 november 2018.
title: Versionsinformation
exl-id: 3f904022-b770-4f35-a3b0-790e15748763
source-git-commit: beb224fdccf68c98fc3eff62b0867f22fa52902b
workflow-type: tm+mt
source-wordcount: '370'
ht-degree: 0%

---

# Versionsinformation{#release-notes}

Versionsinformation för 15 november 2018.

## Nya funktioner {#section_syx_mdt_wcb}

Följande nya funktioner släpptes i produktionsversionen av den här versionen:

* **Uppdateringar av Instagram sök- och direktuppspelning.** Du kan använda ett  *Instagram-* företagskonto:

   * Utför en social sökning från Instagram per användare (användaren måste också vara ett Instagram-företagskonto).

   * Skapa Instagram-strömmar från ett specifikt Instagram-användarkonto (kontot måste också vara ett företagskonto), inklusive ditt eget.

   * Begär rättigheter för resurser från Instagram via ett delvis automatiserat arbetsflöde.

   * Information om vilken typ av Instagram-konton du behöver för att ställa in och begära rättigheter från Instagram finns i [Om Instagram-konton](/help/using/c-users-creating-accounts-with-studio-access/t-configure-social-accout-instagram/c-about-instagram-accounts.md).

* **Automatisk övervakning av användningsrättigheter begär svar för företagskontobaserade sökningar.** Endast för företagskontonsbaserade sökningar - möjlighet att automatiskt övervaka svar på förfrågningar om rättigheter och uppdatera aktivitetshistoriken i Livefyre är tillgängligt.

Mer information om hur du begär rättigheter för Instagram-konton finns i [Skicka en begäran om Instagram-rättigheter manuellt](/help/using/c-how-requesting-rights-works/c-send-instagram-manual-rights-request.md) och [Skicka en delvis automatiserad begäran om Instagram-rättigheter](/help/using/c-how-requesting-rights-works/c-send-an-instagram-rights-request-from-the-library.md).

* **Integrering med Adobe Target.** Integreringen med Adobe Target gör att du kan dela Livefyre-appar direkt i ditt Adobe Target Offers Library. Mer information om hur du använder Livefyre med Adobe Target finns i [Måldokumentation](https://experienceleague.adobe.com/docs/livefyre/using/library/livefyre-target.html).

## Problem {#section_ehw_ndt_wcb}

Problemen i följande tabeller löstes i den här versionen.

### Produktionsrelease

| Ärendetyp | Komponent | Versionsinformation |
|--- |--- |--- |
| Problem | AppService: Livefyre-identitet | Korrigerade ett fel där klickningen på [!UICONTROL Reset to Default] inte återställde logotypen under Login Modal i Studio > Integreringsinställningar > Livefyre-identitet till standardbilden. |
| Problem | Bibliotek | Ett problem där en video som överfördes till biblioteket och sedan visades i resursinformationen inte visades korrekt har åtgärdats. |
| Problem | Strömmar | Korrigerade ett problem som förhindrade att produkter visades i en strömregel. |
| Problem | Strömmar | Ett problem har korrigerats där produkttaggar inte var tillgängliga för en strömregel. |
| Förbättring | Studio | Ett problem har korrigerats där produkt-ID inte visades i Livefyre Studio. |
| Problem | Studio: ModQ | Korrigerade ett problem där borttaget innehåll fortfarande visas i ModQ efter att det tagits bort. |

### UAT-release

| **Ärendetyp** | **Komponent** | **Versionsinformation** |
|---|---|---|
| Problem | Social komponent: Carousel | Korrigerade ett problem där länken Dela inte svarade och kopierade URL:en som förväntat i IE11 och Mozilla Firefox. |
