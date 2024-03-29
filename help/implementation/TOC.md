---
product: livefyre
audience: end-user
user-guide-title: Handbok för Livefyre-implementering
translation-type: tm+mt
source-git-commit: 3664bc1c51d2b372c358385127a1ca9c2f0cfef8
workflow-type: tm+mt
source-wordcount: '543'
ht-degree: 0%

---


# Implementeringshandbok för Livefyre {#implementation}

+ [Handbok för Livefyre-implementering](home.md)
+ Komma igång {#getting-started}
   + [Komma igång med Livefyre-integrering](c-getting-started/c-getting-started.md)
   + Implementeringsprocess {#implementation-process}
      + [Implementeringsprocess](c-getting-started/c-implementation-process/c-implementation-process.md)
      + [Appintegrationstyper](c-getting-started/c-implementation-process/c-app-integration-types.md)
      + [Appimplementering](c-getting-started/designer-app-implementation.md)
      + [Implementera Livefyre med tredjepartsintegrering](c-app-integrations/implement-livefyre-3rd-party.md)
      + [Arkitektur](c-getting-started/c-implementation-process/c-architecture.md)
      + [Bädda in en app](c-getting-started/c-implementation-process/c-using-livefyre.js-to-create-customize-and-use-apps-on-your-site.md)
      + [Lägg till autentisering i ett program med Livefyre.js](c-getting-started/c-implementation-process/c-add-authetication-to-an-app-using-livefyre.js.md)
      + [Bygg token på serversidan](c-getting-started/c-implementation-process/c-build-server-side-tokens.md)
      + [CollectionMeta-token](c-getting-started/c-implementation-process/c-collectionmeta-tokent.md)
      + [Autentiseringstoken för användare](c-getting-started/c-implementation-process/c-user-auth-token.md)
      + [Skapa en samling med CollectionMeta-token](t-create-a-collectionmeta-token.md)
      + [Skapa en kontrollsumma](c-creating-a-checksum.md)
+ Identitetsintegrering {#identity-integration}
   + [Identitetsintegrering](t-about-identity-integration/t-about-identity-integration.md)
   + [Autentiseringspaket](t-about-identity-integration/c-authorization-package.md)
   + [AuthDelegate-objekt](t-about-identity-integration/c-building-an-auth-delegate.md)
   + [Publicera användarbehörigheter till externa system (valfritt)](t-about-identity-integration/c-posting-user-permissions-to-external-systems.md)
   + Implementera enkel inloggning {#implementing-sso}
      + [Implementera SSO](t-about-identity-integration/c-implementing-sso/c-implementing-sso.md)
      + [Felsöka Autentiseringsdelegering](t-about-identity-integration/c-implementing-sso/c-debugging-auth.md)
   + Synkronisera med Livefyre {#sync-ping-for-pull}
      + [Synkronisera med Livefyre med Ping for Pull](t-about-identity-integration/t-sync-with-livefyre-using-ping-for-pull/t-sync-with-livefyre-using-ping-for-pull.md)
      + [Bygg pull-slutpunkten](t-about-identity-integration/t-sync-with-livefyre-using-ping-for-pull/t-build-the-pull-endpoint.md)
      + [Registrera slutpunkten med Studio](t-about-identity-integration/t-sync-with-livefyre-using-ping-for-pull/c-register-the-endpoint-with-studio.md)
      + [Bygg Ping](t-about-identity-integration/t-sync-with-livefyre-using-ping-for-pull/t-build-the-ping.md)
      + [Pull Request Structure](t-about-identity-integration/t-sync-with-livefyre-using-ping-for-pull/t-pull-request-structure.md)
      + [Bygg Ping for Pull Response](t-about-identity-integration/t-sync-with-livefyre-using-ping-for-pull/c-build-the-ping-for-pull-response.md)
+ Livefyre-identitet {#livefyre-identity}
   + [Livefyre-identitet](c-livefyre-identity-comp/c-livefyre-identity-comp.md)
   + [Aktivera Livefyre-identitet](c-livefyre-identity-comp/t-enable-livefyre-identity.md)
   + Använd sociala appar med Livefyre-identitet {#use-social-apps-with-livefyre-identity}
      + [Skapa sociala appar](c-livefyre-identity-comp/t-create-your-social-apps.md)
      + [Skapa en Facebook-app för användning med Livefyre-identitet](c-livefyre-identity-comp/t-create-a-facebook-app-for-use-with-livefyre-identity.md)
      + [Skapa en Twitter-app för användning med Livefyre-identitet](c-livefyre-identity-comp/t-create-a-twitter-app-for-use-with-livefyre-identity.md)
      + [Skapa en Yahoo! App för användning med Livefyre-identitet](c-livefyre-identity-comp/t-create-a-yahoo-app-for-use-with-livefyre-identity.md)
      + [Skapa en Microsoft Live Identity App för användning med Livefyre Identity](c-livefyre-identity-comp/t-create-a-microsoft-live-id-app-for-use-with-livefyre-identity.md)
      + [Skapa en LinkedIn-app för användning med Livefyre-identitet](c-livefyre-identity-comp/t-create-a-linkedin-app-for-use-with-livefyre-identity.md)
      + [Skapa en GitHub-identitetsapp för Livefyre-identitet](c-livefyre-identity-comp/c-create-a-github-identity.md)
      + [Använda Studio för att ansluta sociala appar till Livefyre-implementeringen](c-livefyre-identity-comp/t-using-studio-to-connect-your-social-apps-to-your-livefyre-implementation.md)
   + [Lägg till Livefyre.js på sidan](c-livefyre-identity-comp/t-add-livefyre.js-to-the-page.md)
   + [Initiera Livefyre-identitet](c-livefyre-identity-comp/t-initialize-livefyre-identity.md)
   + [E-post för Livefyre-identitet](c-livefyre-identity-comp/c-emails-for-livefyre-identity.md)
   + [Janrain Capture/Backplane](c-livefyre-identity-comp/c-janrain-capture-backplane-comp.md)
   + Installation {#installation}
      + [Installera bibliotek](c-installing-libraries/c-installing-libraries.md)
      + [Klasser och metoder](c-installing-libraries/c-methods-livefyre.md)
      + [Nätverksmetoder](c-installing-libraries/c-network-methods.md)
      + [setSSL-nätverksmetod](c-installing-libraries/r-setssl-method.md)
      + [buildLivefyreToken - nätverksmetod](c-installing-libraries/r-buildlivefyretoken-method.md)
      + [buildUserAuthToken-nätverksmetod](c-installing-libraries/r-builduserauthtoken-method.md)
      + [validateLivefyreToken-nätverksmetod](c-installing-libraries/c-validatelivefyretoken-network-method.md)
      + [setUserSyncUrl-nätverksmetod](c-installing-libraries/r-setusersyncurl-method.md)
      + [syncUser-nätverksmetod](c-installing-libraries/r-syncuser-method.md)
      + [getUrn-nätverksmetod](c-installing-libraries/r-geturn-method.md)
      + [getUrnForUser-nätverksmetod](c-installing-libraries/r-geturnforuser-method.md)
      + [Nätverksmetoden getNetworkName](c-installing-libraries/r-getnetworkname-method.md)
      + [getSite-nätverksmetod](c-installing-libraries/r-getsite-method.md)
      + [Nätverksklassmetoder](c-installing-libraries/c-network-class-methods.md)
      + [Samlingsklassmetoder](c-installing-libraries/c-collection-methods.md)
      + [createOrUpdate, samlingsmetod](c-installing-libraries/r-createorupdate-collection-method.md)
      + [buildCollectionMetaToken-samlingsmetod](c-installing-libraries/r-buildcollectionmetatoken-collection-method.md)
      + [buildChecksum-samlingsmetod](c-installing-libraries/r-buildchecksum-collection-method.md)
      + [getCollectionContent-samlingsmetod](c-installing-libraries/t-getcollectioncontent-collection-method.md)
      + [getUrn-samlingsmetod](c-installing-libraries/r-geturn-collection-method.md)
      + [Klassmetoder för plats](c-installing-libraries/c-site-methods.md)
      + [buildBlogCollection, webbplatsmetod](c-installing-libraries/r-buildblogcollection-site-method.md)
      + [buildChatCollection-webbplatsmetod](c-installing-libraries/r-buildchatcollection-site-method.md)
      + [buildCommentsCollection, webbplatsmetod](c-installing-libraries/r-buildcommentscollection-site-method.md)
      + [buildCountingCollection, webbplatsmetod](c-installing-libraries/r-buildcountingcollection-site-method.md)
      + [buildRatingsCollection, webbplatsmetod](c-installing-libraries/r-buildratingscollection-site-method.md)
      + [buildReviewsMetod för samlingswebbplats](c-installing-libraries/r-buildreviewscollection-site-method.md)
      + [buildSitenotesCollection, webbplatsmetod](c-installing-libraries/r-buildsitenotescollection-site-method.md)
      + [buildCollection-webbplatsmetod](c-installing-libraries/r-buildcollection-site-method.md)
      + [getUrn-webbplatsmetod](c-installing-libraries/r-geturn-site-method.md)
      + [Exempel](c-installing-libraries/c-libraries-examples.md)
   + SDK för mobiler {#mobile-sdks}
      + [SDK för mobiler](c-mobile-sdks/c-mobile-sdks.md)
      + [Livefyre iOS SDK](c-mobile-sdks/c-livefyre-ios-sdk.md)
      + [Android SDK](c-mobile-sdks/c-android-sdk.md)
+ [Livefyre.js](c-livefyre.js.md)
+ [Skapar Livefyre-token C#](c-creating-livefyre-tokens-c-.md)
+ Programintegreringar {#app-integrations}
   + [Chatt](c-app-integrations/c-app-integratios-chat.md)
   + Kommentarer {#comments}
      + [Kommentarer](c-app-integrations/c-comments-integration/c-comments-integration.md)
   + [Live Blog](c-app-integrations/c-live-blog-integration.md)
   + [Recensioner](c-app-integrations/c-reviews-integration.md)
   + Sidenotes {#sidenotes}
      + [Integrering av sidenotes](c-app-integrations/c-sidenotes-integration/r-sidenotes-integration.md)
      + [Lägga till sidomärken på en sida](c-app-integrations/c-sidenotes-integration/r-adding-sidenotes-to-a-page.md)
      + [Sidenotes App Events](c-app-integrations/c-sidenotes-integration/r-app-events.md)
      + [Konfigurationsalternativ för sidenotes](c-app-integrations/c-sidenotes-integration/r-configuration-options.md)
      + [Egna format för sidenotes](c-app-integrations/c-sidenotes-integration/r-custom-styles.md)
      + [Anpassade sidenotes-strängar](c-app-integrations/c-sidenotes-integration/r-custom-strings.md)
      + [Sidenotes Implementation](c-app-integrations/c-sidenotes-integration/r-sidenotes-implementation.md)
      + [updateAnchors-metod](c-app-integrations/c-sidenotes-integration/update-anchors-method.md)
   + [Karta](c-app-integrations/c-map-integration.md)
   + [Media Wall](c-app-integrations/c-media-wall-integration.md)
   + [Trender](c-app-integrations/c-trending-integration.md)
+ Appanpassningar {#app-customizations}
   + [Appanpassningar](c-app-customizations/c-app-customizations.md)
   + [Ändra visningsalternativ](c-app-customizations/c-change-display-options.md)
   + [CSS-klasser](c-app-customizations/c-css-classes.md)
   + [Storify CSS Classes](c-app-customizations/c-storify-css-classes.md)
   + [Översättningsuppsättningar](c-app-customizations/c-translation-sets.md)
   + [Flytta Livefyre-logotypen](c-app-customizations/c-move-the-livefyre-logo.md)
   + [Begränsa media](c-app-customizations/c-restrict-media.md)
   + [Dölj appelement](c-app-customizations/c-hide-app-elements.md)
   + [Ändra @mention-ikon](c-app-customizations/c-change-mention-icon.md)
   + [Markera innehåll](c-app-customizations/c-highlight-content.md)
   + [Anpassa datum- och tidsstämpeln](c-app-customizations/c-date-time-stamp.md)
   + Funktionsinnehåll {#feature-content}
      + [Innehåll](c-app-customizations/t-feature-content.md)
      + [Aktivera innehåll i Studio](c-app-customizations/t-enable-featuring-content-in-studio.md)
      + [Välj innehåll till funktion från en app](c-app-customizations/t-select-content-to-feature.md)
      + [Välj innehåll från Studio](c-app-customizations/t-select-content-to-feature-from-studio.md)
      + [Använd CSS för att formatera innehåll](c-app-customizations/c-use-css-to-style-featured-content.md)
      + [Funktions-API:er](c-app-customizations/c-feature-apis.md)
   + [Ansluta Janrain till Livefyre med AuthDelegate](c-app-customizations/c-connecting-janrain-to-livefyre-using-authdelegate.md)
   + [Aggregerat innehåll med hjälp av aktuella API:er](c-app-customizations/c-aggregated-featured-content-using-the-featured-apis.md)
   + Formatinnehåll {#style-content}
      + [Formatera användargruppinnehåll](c-app-customizations/c-style-user-group-content.md)
      + [Lägga till användare i grupper](c-app-customizations/c-adding-users-to-groups.md)
   + Använd anpassade format {#apply-custom-styles}
      + [Använda anpassade format](c-app-customizations/c-applying-custom-styles-.md)
      + [Lägg till anpassade knappar](c-app-customizations/t-add-custom-buttons.md)
   + JavaScript-händelser {#javascript-events}
      + [JavaScript Events-definitioner och exempel](c-app-customizations/c-javascript-events.md)
      + [JavaScript-händelser för visualiseringsappar](c-app-customizations/c-javascript-events-for-visualization-apps.md)
      + [JavaScript-händelser för medievägg](c-app-customizations/c-javascript-events-media-wall.md)
      + [JavaScript-händelser för konversationsappar](c-app-customizations/c-javascript-events-for-conversation-apps.md)
   + [Bädda in en kommentarapp](c-app-customizations/c-embed-a-comments-app.md)
   + [Referensspårning](c-app-customizations/c-referral-tracking.md)
   + [Stöd för enheter och webbläsare](c-app-customizations/c-device-and-browser-support.md)
   + [Twitter-krav](c-app-customizations/c-twitter-display-requirements.md)
+ [Princip för stresstest](c-stress-test-policy.md)
+ Analyser {#analytics}
   + [Analyser](livefyre-analytics/livefyre-analytics.md)
   + [Använd Livefyre med Adobe Analytics och Dynamic Tag Manager (DTM)](livefyre-analytics/c-use-livefyre-with-adobe-analytics.md)
   + [Använd Livefyre med andra analysverktyg](livefyre-analytics/c-livefyre-analytics.md)
   + [Livefyre Analytics Events](livefyre-analytics/c-livefyre-analytics-events.md)
+ [Integrera Livefyre med AEM](c-livefyre-aem-integration.md)
+ Avancerade ämnen {#advanced-topics}
   + [Visa antal kommentarer](c-advanced-topics/t-display-comment-count.md)
   + [Aktivera delning via sociala medier](c-advanced-topics/c-enabling-social-sharing.md)
   + [Aktivitetsström](c-advanced-topics/c-activity-stream.md)
   + [Bootstrap HTML](c-advanced-topics/c-bootstrap-html.md)
   + [Ändra samling](c-advanced-topics/c-change-collection.md)
   + [Flera samlingar](c-advanced-topics/c-multiple-collections.md)
   + [Apptyper för switchkärnor](c-advanced-topics/c-switch-core-app-types.md)
   + [Socialräknare](c-advanced-topics/c-social-counter.md)
   + [Använd start- och direktuppspelnings-API med Livefyre-appar](c-advanced-topics/bootstrap-stream-api.md)
