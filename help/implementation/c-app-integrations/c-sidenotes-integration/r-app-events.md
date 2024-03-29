---
description: Du kan lyssna på händelser på en instans av Sidenotes.
title: Sidenotes App Events
exl-id: e341ca76-002d-425c-8d1a-35c3253fb254
translation-type: tm+mt
source-git-commit: a2449482e617939cfda7e367da34875bf187c4c9
workflow-type: tm+mt
source-wordcount: '235'
ht-degree: 0%

---

# Sidenotes App Events {#sidenotes-app-events}

Du kan lyssna på händelser på en instans av Sidenotes.

Återanrop kan registreras med `onmethod` och avregistreras med metoden `removeListener`. En `once`-metod är tillgänglig för enkelhet om återanropet bara ska anropas en gång och sedan avregistreras.

```
var app = Livefyre.Sidenotes(convConfig); 
   app.once('sidenotes.initialized', function () { 
     // Sidenotes initialized!  
});
```

Mer information om Livefyre-händelser finns på JavaScript-händelsesidan i referensavsnittet.

| Nyckel | Beskrivning |
|--- |--- |
| sidenotes.initialized | Utlöses när appen instansieras, innehåller data och finns på sidan. |
| sidenotes.commentFlagged | Utlöses när en kommentar har flaggats. Data innehåller: <br><ul><li>`targetId`: ID för kommentaren som flaggats</li><li>`type`: flaggtypsträng  `(offensive, off-topic, spam, disagree)`</li></ul> |
| `sidenotes.commentPosted` | Utlöses när en kommentar har bokförts. Data innehåller: <br><ul><li> `authorId`: ID för författaren till kommentaren </li><li>`bodyHtml`: kommentarens brödtext </li><li> `parent`: ID för kommentarens överordnade, eller null</li></ul> |
| `sidenotes.commentShared` | Utlöses när en kommentar har delats. Data innehåller: <br><ul><li>`targetId`: ID för kommentaren som delades </li><li> `sharedToFacebook`: om kommentaren delades till Facebook </li><li>`sharedToTwitter`: om kommentaren delades till Twitter</li></ul> |
| `sidenotes.commentVoted` | Utlöses när en omröstning om en kommentar har gjorts. Data innehåller: <br><ul><li>`targetId`: id för kommentaren som röstades om </li><li> `targetAuthorId`: id för författaren vars kommentar röstades om</li><li> `type`: numerisk rösttyp: 0: &quot;klar&quot;, 1: &quot;upvoice&quot;, eller 2: nedröst</li></ul> |
| `sidenotes.userLoggedIn` | Utlöses när en användare loggar in. Data innehåller: <br><ul><li>`avatar`: avatar-URL för användaren </li><li>`displayName`: visningsnamn för användaren</li><li>`id`: användarens ID</li><li> `isModerator`: om användaren är moderator för den aktuella samlingen</li></ul> |
| `sidenotes.userLoggedOut` | Utlöses när en användare loggar ut |
