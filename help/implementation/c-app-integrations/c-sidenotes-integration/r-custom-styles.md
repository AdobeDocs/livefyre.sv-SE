---
description: Egna format används genom ett objekt som injiceras i Sidenotes-konstruktorn.
title: Egna format för sidenotes
exl-id: 846605b7-a21e-4600-bf17-18841d2ed96d
translation-type: tm+mt
source-git-commit: a2449482e617939cfda7e367da34875bf187c4c9
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 0%

---

# Sidenotes Custom Styles{#sidenotes-custom-styles}

Egna format används genom ett objekt som injiceras i Sidenotes-konstruktorn.

Nycklarna är objektnycklar som representerar DOM-element, medan egenskaper stöds för CSS-egenskaper för den aktuella nyckeln. Om du till exempel vill anpassa formatet för blockBtn (som är den knapp som startar Sidenotes-poveren), skapar du ett objekt som:

```
var styles = { 
   'blockBtn': { 
      'fontColor': '#555', 
      'fontSize': '18px' 
   } 
}; 
new Livefyre.Sidenotes({ 
   customStyles: styles, 
      ...  
})
```

| **Nyckel** | **Egenskaper** | Beskrivning |
|---|---|---|
| `anonymousAvatar` | &quot;height&quot;,&quot;width&quot; | Anonym avatarbild till vänster om textområdesredigeraren. |
| `blockBtn` | &quot;fontColor&quot;,&quot;fontSize&quot;,&quot;left&quot;,&quot;position&quot;,&quot;right&quot;,&quot;top&quot; | &quot;Startikonen&quot; placerad bredvid element som angetts som sidenote-able. |
| `blockBtnActive` | &quot;fontColor&quot;,&quot;fontSize&quot;,&quot;left&quot;,&quot;position&quot;,&quot;right&quot;,&quot;top&quot; | Startikonen i aktivt läge. |
| `commentAvatar` | &quot;height&quot;,&quot;width&quot; | Avatarbild till vänster om anteckningar på den översta nivån. |
| `commentBody` | &quot;fontColor&quot;,&quot;fontFamily&quot;,&quot;fontSize&quot;,&quot;fontWeight&quot;,&quot;lineHeight&quot; | Textinnehåll i kopplade anteckningar. |
| `commentDisplayName` | &quot;fontColor&quot;,&quot;fontFamily&quot;,&quot;fontSize&quot;,&quot;fontWeight&quot;,&quot;lineHeight&quot; | Visa namnet på den användare som har lämnat en anteckning. |
| `commentDownvote` | &quot;fontColor&quot;,&quot;fontSize&quot; | Nedklicka på en anteckning. |
| `commentReplyExpand` | backgroundColor, borderColor, borderWidth, fontColor, fontFamily, fontSize, fontWeight, lineHeight | Knapp för att utöka trådar med ett stort antal svar. |
| `commentTags` | &quot;fontColor&quot;,&quot;fontFamily&quot;,&quot;fontSize&quot;,&quot;fontWeight&quot;,&quot;lineHeight&quot; | Taggar om en användare i en anteckning. |
| `commentUpvote` | &quot;fontColor&quot;,&quot;fontSize&quot; | Knapp för att skicka med en anteckning. |
| `editorTextarea` | &quot;height&quot;,&quot;width&quot;,&quot;fontColor&quot;,&quot;fontFamily&quot;,&quot;fontSize&quot;,&quot;fontWeight&quot;,&quot;lineHeight&quot; | Inmatningsruta för textområde för att lämna anteckningar. |
| `mediaBlockBtn` | &quot;fontColor&quot;,&quot;fontSize&quot;,&quot;left&quot;,&quot;position&quot;,&quot;right&quot;,&quot;top&quot; | Ikonen för att starta media när det ligger ovanpå ett medieobjekt (img, video). |
| `mediaBlockBtnActive` | &quot;fontColor&quot;,&quot;fontSize&quot;,&quot;left&quot;,&quot;position&quot;,&quot;right&quot;,&quot;top&quot; | Ikonen för att starta media i ett aktivt läge. |
| `numSidenotes` | &quot;fontColor&quot;,&quot;fontFamily&quot;,&quot;fontSize&quot;,&quot;fontWeight&quot;,&quot;lineHeight&quot;,&quot;backgroundColor&quot;,&quot;borderColor&quot;,&quot;borderWidth&quot;,&quot;height&quot;,&quot;width&quot; | Klickbar knapp som visar antalet sidotecken i samlingen. |
| `numSidenotesPopover` | &quot;fontColor&quot;,&quot;fontFamily&quot;,&quot;fontSize&quot;,&quot;fontWeight&quot;,&quot;lineHeight&quot;,&quot;backgroundColor&quot;,&quot;borderColor&quot;,&quot;borderWidth&quot;,&quot;height&quot;,&quot;width&quot; | Leverera med en kort förklaring av Sidenotes för användaren. |
| `popover` | &quot;backgroundColor&quot; | Den pover som öppnas när en startikon anropas. |
| `popoverArrowLeft` | &quot;backgroundImage&quot;,&quot;height&quot;,&quot;left&quot;,&quot;right&quot;,&quot;top&quot;,&quot;width&quot; | Vänsterpilselement på povern som pekar på DOM-elementet som innehåller en startikon. |
| `popoverArrorRight` | &quot;backgroundImage&quot;,&quot;height&quot;,&quot;left&quot;,&quot;right&quot;,&quot;top&quot;,&quot;width&quot; | Högerpil på povern som pekar på DOM-elementet som innehåller en startikon. |
| `popoverArrowTop` | &quot;backgroundImage&quot;,&quot;height&quot;,&quot;left&quot;,&quot;right&quot;,&quot;top&quot;,&quot;width&quot; | Det översta pilelementet på povern som pekar på DOM-elementet som innehåller en startikon. |
| `replyAvatar` | &quot;height&quot;,&quot;width&quot; | Avatarbild till vänster om anteckningar på svarsnivå. |
| `streamPoweredBy` | backgroundColor, borderColor, lineHeight | &quot;Powered by&quot; footer on the pover. |
| `streamQueueButton` | backgroundColor, borderColor, borderWidth, fontColor, fontFamily, fontSize, fontWeight, lineHeight | Knapp som anger när nya anteckningar direktuppspelas i en öppen pover. |
| `userAvatar` | &quot;height&quot;,&quot;width&quot; | Autentiserad användares avatarbild, till vänster om textområdesredigeraren. |
