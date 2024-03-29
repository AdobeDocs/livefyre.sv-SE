---
description: Lägg till Livefyre i iOS-appen.
title: Livefyre iOS SDK
exl-id: 961c41dc-fee8-480c-a189-a20a689e705f
source-git-commit: 3091db9d7b9611e26ad65c1432856c9465694e92
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 0%

---

# Livefyre iOS SDK{#livefyre-ios-sdk}

Lägg till Livefyre i iOS-appen.

Använd det här biblioteket med öppen källkod för att integrera Livefyre-tjänster i era iOS-program. Livefyre StreamHub iOS SDK har ett tunt lager runt våra gemensamma API-funktioner, baserat på det utmärkta AFNetworking-biblioteket.

Livefyre innehåller även två exempelappar för iOS baserat på denna SDK: en kommentarström och en exempelapp för recensioner.

## Integrera SDK i ditt projekt som en Cocoa Pod (rekommenderas) {#section_qc5_h3v_zz}

Det enklaste sättet att lägga till StreamHub-iOS SDK i ditt projekt är att använda CocoaPods. Om du inte har CocoaPods kan du köra Gem-installationen av coapods och pod. Här är ett exempel på en podfil:

```
source 'https://github.com/Livefyre/cocoapods.git' 
source 'https://github.com/CocoaPods/Specs.git' 
  
platform :ios, :deployment_target => '6.0' 
  
pod 'StreamHub-iOS-SDK', '~> 0.3.0'
```

Du måste också lägga till en Specs-databas i din CocoaPod-installation (detta klonar den i katalogen `~/.cocoapods/repos`):

```
pod repo add livefyre https://github.com/Livefyre/cocoapods.git
```

När din Podfile har skapats i programprojektroten och databasen ovan har lagts till kör du:

```
pod install
```

Detta hämtar alla beroenden och skapar en fil, MyApp.xcworkspace, som du bör använda från och med nu för att öppna ditt appprojekt i Xcode.

## Som ett Xcode-delprojekt {#section_jcm_g3v_zz}

Du kan också klona databasen:

```
git clone https://github.com/Livefyre/StreamHub-iOS-SDK.git 
```

Sedan lägger du till Xcode-projektet (LFSClient.xcodeproj) i programmet som ett underprojekt (du kan enkelt göra det genom att dra filen LFSClient.xcodeproj till rutan Project Navigator i Xcode).

Du måste också göra samma sak med alla beroenden ([AFNetworking](https://github.com/AFNetworking/AFNetworking), [JSONKit](https://github.com/escherba/JSONKit)).

## Hämta allt på en gång (rekommenderas inte) {#section_rpb_f3v_zz}

```
cd ~/dev 
git clone https://github.com/Livefyre/StreamHub-iOS-SDK.git 
cd StreamHub-iOS-SDK 
git submodule init 
git submodule update 
pod repo add livefyre https://github.com/Livefyre/cocoapods.git 
pod install 
cd examples/CommentStream 
pod install 
open CommentStream.xcworkspace
```

>[!NOTE]
>
>Om du vill köra tester i Xcode 6 måste du lägga till $(PLATFORM_DIR)/Developer/Library/Frameworks i FRAMEWORK_SEARCH_PATHS i Pods-test-XCTest+HTTPStubSuiteCleanUp-pod[https://stackoverflow.com/a/24651704](https://stackoverflow.com/a/24651704).

Du behöver filen LFSTestConfig.plist från Livefyre, som Livefyre tillhandahåller på begäran.

## Xcode-dokumentation {#section_arl_b3v_zz}

Du kan bläddra i [dokumentationen](https://github.com/Livefyre/StreamHub-iOS-SDK) eller så kan du skapa dokumentationsmålet i Xcode (kräver att appledoc är installerat) på datorn.

## Krav {#section_m5l_13v_zz}

StreamHub iOS SDK-versioner sedan v0.2.0 kräver iOS 6.0 eller senare.

## Bilaga (JSON-stöd) {#section_pcd_5hv_zz}

Observera att för dem som tittar på interna StreamHub-iOS SDK-sidor använder vi en modifierad version av [JSONKit](https://github.com/escherba/JSONKit) som JSON-standardtolk (i stället för Apple-tillhandahållen NSJSONSerialization). Vi var tvungna att göra detta eftersom den parser som tillhandahålls av Apple inte stöder avkodning av JSON-filer som innehåller heltal eller flyttal som är större än de som kan representeras av systemet. Vår ändrade version av JSONKit trunkerar mycket stora tal till motsvarande systemmaximum i stället för att generera ett undantag.
