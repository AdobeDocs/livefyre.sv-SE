---
description: Gör communityinnehåll tillgängligt för sökmotorcrawler.
title: Bootstrap HTML
exl-id: 22ab4f2d-f433-4805-b0dd-16d4531e425d
translation-type: tm+mt
source-git-commit: a2449482e617939cfda7e367da34875bf187c4c9
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 0%

---

# Bootstrap HTML

Gör communityinnehåll tillgängligt för sökmotorcrawler.

En fullständig lista över tillgängliga slutpunkter finns i avsnittet Livefyre [API Reference](https://api.livefyre.com/docs).

Livefyre Apps kräver att du kör JavaScript på sidan för att visa innehåll för dina samlingar. Eftersom de flesta crawler för sökmotorer inte kan köra JavaScript, kan de inte se innehållet som dina communityn skickar. Använd Bootstrap HTML API för att lägga till sökbara fragment av det här innehållet till det inledande HTTP-svaret på sidan, så att innehållet och nyckelorden kan optimeras i sökmotorn.

>[!NOTE]
>
>Detta API är bara tillgängligt för kommentarerna och Live Blog Collection-typerna.

## Integrering

Livefyres Bootstrap HTML-API returnerar ett HTML-fragment av ditt användarinnehåll, som kan inkluderas i sidans HTTP-svar. Svaret kan läsas av sökmotorcrawler utan att JavaScript körs. När sidan är live i en användares webbläsare ersätts HTML-fragmentet med den fullständiga, interaktiva widgeten och användaren kan publicera innehållet.

Så här implementerar du Bootstrap HTML API:

1. Gör en server till server-API-begäran till Bootstrap HTML-slutpunkten som beskrivs nedan.

   >[!NOTE]
   >
   >Om du försöker hämta Bootstrap HTML för en konversation som ännu inte finns (d.v.s. om du ännu inte bäddat in appen eller skapat samlingen) får du 200, men med innehåll som ser ut ungefär så här: `<!- HTTP 404 example.fyre.co/000000/MTEwMTo2NDEyOD1RS/bootstrap.html ->`

1. Om returen inte innehåller innehåll med värdet 404 sparar du den i en sträng. Du kan cachelagra det här svaret för senare bruk för att undvika att begära Bootstrap HTML API för varje sidinläsning.
1. Infoga HTML-strängen Bootstrap på webbsidan där du vill att innehållet ska visas.
1. Skicka webbsidan till webbläsaren (eller sökmotorns crawler).

## Resurs

```
GET https://{networkName}.bootstrap.fyre.co/bs3/{networkName}.fyre.co/{siteId}/{base64 encoded article ID}/bootstrap.html 
```

## Parametrar

* **** networkNameLivefyre angav nätverksnamn. Till exempel: *labb* i `labs.fyre.co`.
* **** siteIdSamlingens webbplats-ID.
* **b64** articleIdThe Article ID of the Collection using the base64url encoding.

## Exempel

```
https://labs.bootstrap.fyre.co/bs3/labs.fyre.com/4/NTg0/bootstrap.html 
```

## Svar

```
https://gist.github.com/ec5c2457322faf9cf515 
```
