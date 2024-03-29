---
description: Lägg till en användartagg i ett konto för att lägga till en användare i en grupp.
title: Lägga till användare i grupper
exl-id: 6e799c77-e815-40c2-ae06-bbd076df9fe7
translation-type: tm+mt
source-git-commit: a2449482e617939cfda7e367da34875bf187c4c9
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 1%

---

# Lägga till användare i grupper{#adding-users-to-groups}

Lägg till en användartagg i ett konto för att lägga till en användare i en grupp.

Användartaggar kan implementeras för både egna system och företagsprofilsystem och kan läggas till på konton på flera sätt:

* Om du skapar ägare och moderatorer via Studio tilldelas användartaggen&quot;Moderator&quot; till kontot.
* När du skapar användargrupper och lägger till användare via Studio, används automatiskt användartaggar med namnet på gruppen för de valda användarna.
* Användartaggar kan även användas direkt på konton med hjälp av HTTP[anropet Lägg till användartagg, eller Ping for Pull.](https://api.livefyre.com/docs#add-user-tag)

>[!NOTE]
>
>Båda API-metoderna, HTTP Add User Tag call och metoden Ping for Pull, skriver över taggar som tidigare tilldelats kontot på andra sätt. Välj därför en metod och använd den konsekvent genom hela processen.

## Lägg till en användare i en grupp från sidan Användare i Studio {#section_qgq_nbw_xz}

* Klicka på **[!UICONTROL Add Group]** eller gruppetiketten under ett användarnamn för att öppna gruppmenyn.
* Bläddra igenom listan och hitta gruppen som du vill lägga till användaren i. Du kan ange ett gruppnamn i rutan **[!UICONTROL Search]** högst upp i listrutan.
* Klicka i kryssrutan bredvid gruppen/grupperna som användaren ska läggas till i och tryck sedan på Retur.

Användarens profil visar antingen namnet på gruppen (om användaren bara är i en grupp) eller antalet grupper som användaren tillhör.

## Lägg till en användare i en grupp med hjälp av anropet Lägg till användartagg {#section_kn3_gbw_xz}

Skicka användarens LFToken och det markerade taggnamnet tillsammans med POSTENS begäran

Exempel:

```
curl -XPOST -d 'tag_name=tag&lftoken=eyJhbGciOiAiA_TOKENcGlyZXMiOiAxMzU3OTY3NTAxLjIzn0.KoyXUVCavt-rdvkVXm2qzQTyMAOSp-crQA1uL1ht9WU' 'https://labs.quill.fyre.co/api/v3.0/author/system@`labs.fyre.co`/tag/'
```


Mer information finns i API-referens > [Lägg till användartagg](https://api.livefyre.com/docs/apis/by-category/user-management#operation=urn:livefyre:apis:quill:operations:api:v3.0:author:tags:method=post).

## Lägg till en användare i en grupp med Ping för pull {#section_kyj_11w_xz}

Använd taggarrayen för att tilldela användare till användargrupper. (Taggar kan innehålla 1-63 alfanumeriska tecken och understreck.)

Exempel:

```
"tags": ["moderator", "brand_advocate"],
```

## Lägga till en användare i en grupp med hjälp av fjärrprofiler {#section_uyn_scv_xz}

Lägg till användartaggar i fjärrprofilen, som används för att synkronisera användardata mellan ditt anpassade profilsystem och Livefyre, för specifika användare.
