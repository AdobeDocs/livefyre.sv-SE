---
description: Flytta Livefyre-logotypen på sidan.
seo-description: Flytta Livefyre-logotypen på sidan.
seo-title: Flytta Livefyre-logotypen
solution: Experience Manager
title: Flytta Livefyre-logotypen
uuid: 807304ae-6070-4505-87db-169a925f714c
translation-type: tm+mt
source-git-commit: 67aeb3de964473b326c88c3a3f81ff48a6a12652

---


# Flytta Livefyre-logotypen{#move-the-livefyre-logo}

Flytta Livefyre-logotypen på sidan.

Om ditt avtal med Livefyre tillåter kan du flytta Livefyre-logotypen från innehållsströmmens överkant till dess nederkant.

Lägg till exempel till följande HTML på sidan direkt efter elementet som innehåller Livefyre-appen:

```
<div id="powered_by_livefyre_new"><a href="https://livefyre.com" target="_blank">Powered by Livefyre</a></div>
```

Lägg sedan till följande i sidans formatmall:

```
/* Hide the top logo */ 
.fyre-widget .fyre-logo-drop, .fyre-widget .fyre-logo-help, .fyre-widget .fyre-help { 
    display:none !important; 
} 
  
/* Style the bottom logo */ 
#powered_by_livefyre_new a {    background: url(https://cdn.livefyre.com/libs/fyre.conv/v3.0.0/images/poweredbylivefyre.png) no-repeat left top; 
    display: block; 
    height: 24px; 
    font: 13px "Helvetica Neue", Helvetica, Arial, Geneva, sans-serif; 
    text-decoration: none; 
    color: #404040; 
    padding-left: 28px; 
    padding-top: 4px; 
} 
#powered_by_livefyre_new a:hover { 
    text-decoration: underline; 
}
```

