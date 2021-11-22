# MICO-BOT
# What is Miço Bot?

Miço is your virtual assistant in Microsoft Teams.

<img src="https://github.com/eda-ayan/MICO-BOT/blob/main/media/micologo_small.png?raw=true" width=15% height=15%>

Miço is a virtual assistant that can help you in many ways and chat. You can ask a lot of things; From weather information in Turkey, to exchange rates and conversions, from current news on a subject, to a person or thing you are curious about the definition in encyclopedia. You can do short translations and give feedback to him without leaving Teams. Moreover, you can install Miço in your own Teams.

<img src="https://user-images.githubusercontent.com/14835957/133957964-bb5dc633-1aa5-4924-affc-0d50433030b9.jpeg" width=25% height=25%>
<img src="https://user-images.githubusercontent.com/14835957/133957977-61e3c06c-6e31-4b71-b36a-adc002e70fe8.jpeg" width=25% height=25%>
<img src="https://user-images.githubusercontent.com/14835957/133957989-b65c0daa-d799-4b90-9acf-147d525bc60e.jpeg" width=25% height=25%>
<img src="https://user-images.githubusercontent.com/14835957/133958000-b8bac881-d2cb-4b77-a27c-c8c0075b09c5.jpeg" width=25% height=25%>
<img src="https://user-images.githubusercontent.com/14835957/133958007-8dff7f60-0c35-4545-acf8-c974dc00e0a0.jpeg" width=25% height=25%>

## [Requirements](#miçoyu-nasıl-kullanabilirim-gereksinimler)
*Services required to use Miço.*

1. [Azure Hesabı](#1-azure-hesabı-oluşturma)
2. [Bot Composer](#2-bot-composer-kurulum)
3. [Language Understanding Service (LUIS)](#3-language-understanding-service-luis)
4. [QnA Maker - Optional](#4-qna-maker---optional)
5. [Bing Maps](#5-bing-maps)
6. [Bing Search](#6-bing-search)


## [Installation](#how-can-i-use-mico--requirements)
*Miço installation steps.*
1. [Miço'yu Kurun!](#1-miçoyu-kurun)
2. [Miço'yu Publish Edin](#2-miçoyu-publish-edin)
3. [Miço'yu Teams'e Ekleyin](#3-miçoyu-teamse-ekleyin)


## [How to Add a New Intent?](#yeni-bir-niyet-ve-dialog-nasıl-eklenir)
1. [Hava Durumu Niyeti](#1-niyet--hava-durumu-niyeti)
2. [Hava Durumu Dialoğu](#2-dialog--hava-durumu-dialoğu)


# How can I use Miço: Requirements

## 1. Creating an Azure Account
Create a free [Azure account](https://azure.microsoft.com/en-us/free/cognitive-services/).

## 2. Bot Composer Installation

To download [Bot Composer](https://docs.microsoft.com/en-us/composer/install-composer?tabs=windows) by choosing the operating system that suits you, you must first download [Node.js LTS 14.x](https://nodejs.org/) with npm and [.NET Core SDK](https://dotnet.microsoft.com/download/dotnet-core/3.1).

You can then download and install Bot Composer.

<img src="https://raw.githubusercontent.com/msft-ai-demos/MICO-BOT/main/Additional/ss1.png" width=25% height=25%>

### 2.1. Node.js ve npm
Installing the Node.js JavaScript platform and the npm package enables Composer to run Node.js models. Download [Node.js LTS 14.x](https://nodejs.org/) with npm. This is a mandatory service to be able to use Composer.

### 2.2. .NET Core SDK
Download [.NET Core SDK](https://dotnet.microsoft.com/download/dotnet-core/3.1). This service is required in order to create your bot using C# language.

Run Bot Composer.

<img src="https://raw.githubusercontent.com/msft-ai-demos/MICO-BOT/main/Additional/ss2.png" width=50% height=50%>

## 3. Language Understanding Service (LUIS)
Language Understanding (LUIS) is a natural language understanding (NLU) cognitive service that enables users to interact with your applications, bots, and IoT devices using natural language. Get started with the [LUIS](https://docs.microsoft.com/en-us/azure/cognitive-services/luis/sign-in-luis-portal) service.

## 4. QnA Maker - Optional
The Q&A Maker Service categorizes information, resulting in easy-to-find answers that can be used in a conversational context. Get started with the [Question and Answer Creation Service](https://docs.microsoft.com/en-us/azure/cognitive-services/QnAMaker/how-to/set-up-qnamaker-service-azure?tabs=v1).

## 5. Bing Maps - Optional
Bing Maps is a web map service search engine. Get started with [Bing Maps](https://docs.microsoft.com/en-us/bingmaps/getting-started/bing-maps-dev-center-help/creating-a-bing-maps-account).

## 6. Bing Search - Optional
Bing is Microsoft's multilingual search engine. To use Bing on your bot, you can create [Bing Search Resource](https://docs.microsoft.com/en-us/bing/search-apis/bing-web-search/create-bing-search-service-resource) via Azure Portal.

## 7. Merkez Bankası API -Optional
You can create a key by following [Central Bank EVDS Web Service Documentation](https://evds2.tcmb.gov.tr/help/videos/EVDS_Web_Servis_Usim_Kilavuzu.pdf) so that the bot can access up-to-date currency information.


# How can I use Miço: Installation

## 1. Install Miço!

After you have successfully downloaded Bot Composer and created the necessary services, you can now begin what you need to do to install and run Miço.
First, download the Bot folder named Mico-Bot in this repository to your local or clone this repository.

Open composer and find the bot file you have extracted by selecting it from within composer.

You should then be able to open Miço from within Bot Composer.

<img src="https://user-images.githubusercontent.com/14835957/131674595-f2622de3-92e8-46e5-a790-972f8dcf9d56.png" width=50% height=50%>


## 2. Publish Miço

Miço'yu publish edebilmek için yapmanız gereken ilk şey, bir Publishing Profile oluşturmak. Bu adımı tamamen composer içerisinden tamamlayabilirsiniz. Eğer LUIS, QnA maker gibi kaynakları Azure Portal'da çoktan oluşturduysanız, import existing resources seçeneğinden kaynaklarınızın endpointlerini ve keylerini doldurarak bir Publishing Profile oluşturabilirsiniz. Eğer daha önce hiç kaynak açmadıysanız Create new resources seçeneğiyle bu kaynakları Bot Composer üzerinden oluşturabilir ve Publishing Profile'ınıza ekleyebilirsiniz.
![image](https://user-images.githubusercontent.com/14835957/133958169-b4069ba8-4acd-4053-887f-b2daf5faeac3.png)

Daha sonra Publishing Profile'ınızı seçerek Publish selected bots seçeneğine tıklamanız yeterli olacaktır. 

## 3. Add Miço to Teams

There are a few steps left to complete before you can add the bot you have published to Teams. We will complete these steps from within the Azure Portal. When you open your published bot from the Azure Portal, you can see the channels in the Channels tab where you can integrate your bot. You can position your bot on Teams by choosing Teams from these channels.

![image](https://user-images.githubusercontent.com/25666677/142224934-07e6cc97-d9e0-4304-927d-08ca9c905fad.png)


# How to Add a New Intent and Dialog?
## Example: Weather Intent and Dialogue

While using Miço, you may want to add different features to it. For this, you first need to determine the intent to be associated with this feature. For example, when you want to add Miço the ability to tell the weather, the intent you need to understand here is the weather. Weather related questions from the user should be parsed with Miço's natural language understanding and trigger the Weather Intent.

While you create the intent and understand the requests from the user correctly, you can also start creating the dialog. Entities that you can extract from the intent will also shape the flow of your dialog.

Here's how you can recreate the weather intent and dialogue to guide your progress as you add a new feature to Miço.

### 1. Intent : Weather Intent

While creating the intents, you can create them from Bot Composer or from LUIS's own interface. In this example, the Weather intent will be created via LUIS' own interface, luis.ai. [LUIS.AI](https://www.luis.ai)

<img src="https://user-images.githubusercontent.com/14835957/133092774-0df8fd6d-915b-4fdd-a7a5-10f23a56593a.png" width=50% height=50%>

The first thing you need to do in the Luis Portal is to create a new project by clicking +New App. You can create a project called MicoIntents. While creating this app, you will be asked to select the LUIS Prediction Resource for the LUIS service you have opened through the Azure Portal.

After creating the project, we can now create the Intent. Add an intention called 'Weather' by clicking + Intent.

1) After creating the intent, let's first add a few sample sentences that may come from users.

- How's the weather?
- What is the weather
- What will the weather be like?
- weather forecast

<img src="https://user-images.githubusercontent.com/14835957/133099693-1d87d82a-c3d5-48c9-bbe6-22dbb7518d55.png" width=50% height=50%>

If the user directly asks about the weather, we can ask them about the city. This is how we will need to create the flow of our dialogue. We will address this first case in the Dialogue section.

2) If the user asks about the weather by specifying the city, we should catch the concept of the city in the incoming sentence in order not to ask them this question again.
For this we need to create an entity.

In the Entities section on the left, we can click + Create Entity.

<img src="https://user-images.githubusercontent.com/14835957/133101481-441377b8-f5a1-4fa0-9c83-b20dcaea36c8.png" width=50% height=50%>

Here we have a few options.

- [List Entity](https://docs.microsoft.com/en-us/azure/cognitive-services/luis/luis-concept-entity-types#list-entity): A fixed and closed set of related words with synonyms represent together. You can use list entities to recognize multiple synonyms or variations and extract a normalized output for them. Example: Days of the Week.
- [Regex Entity](https://docs.microsoft.com/en-us/azure/cognitive-services/luis/luis-concept-entity-types#regex-entity): Ideal for regular expression, structured text, or predefined set of alphanumeric values in a specific format. Example: Flight Numbers, Identification Numbers...
- [Machine Learned Entity](https://docs.microsoft.com/en-us/azure/cognitive-services/luis/luis-concept-entity-types#machine-learned-ml-entity): Machine-learned entity uses its context to extract assets based on tagged instances. It uses machine learning algorithms and requires tagging to be successfully adapted to your application. Example: Contact names.
- [More](https://docs.microsoft.com/en-us/azure/cognitive-services/luis/luis-concept-entity-types)
- 
3. The first Entity we will add to the Micho will be the time interval that can come from the user. If the user does not provide a time range in the sentence, we can give him the weather for today and for the next days. But if the user wants to know about tomorrow, or if he wants to see detailed weekly results, we should understand that too. We will create a List type entity for the time range entity. The List will have three elements: Today, Tomorrow, Weekly.

<img src="https://user-images.githubusercontent.com/14835957/133231586-f520fdf8-154d-45f4-af52-614dfce67475.png" width=50% height=50%>

4.  Bu entity'yi Machine Learned entity tipinde oluşturacağız, bu sayede, kullanıcının girebileceği tüm şehir örneklerini LUIS'e vermeden, onun öğrenme yeteneğinden faydalanarak, sadece bir kaç örnekle ona şehir kısmını yakalamayı öğretebiliriz.

4. Our next enity will be the City entity that we will generate, in case the user may also specify the city when asking for the weather. We will create this entity as a Machine Learned entity, so that we can take advantage of its learning ability to teach it to capture the city part with just a few examples without giving all the city examples that the user can enter to LUIS.

Let's go back to the Weather Intent and start entering sample phrases. This time, include the city. Then, let's select these cities and match them with the Machine Learned City entity we created.

<img src="https://user-images.githubusercontent.com/14835957/133232461-f139ef04-81da-4ba9-a3f8-16ba2b79909b.png" width=50% height=50%>

After diversifying it with a few more examples, you can click on Train from the upper right corner and then test it with sample sentences.

After completing our intents and entities, we can now add this format to Bot Composer. For this, you have to go to the LUIS portal homepage, select your app and say export as .lu file.

<img src="https://user-images.githubusercontent.com/14835957/133232861-0e8190e6-b14f-4cf9-9dd7-788cb3f5a19b.png" width=50% height=50%>

We should use the content of the .lu file we exported in the weather trigger in the bot.

<img src="https://user-images.githubusercontent.com/14835957/133771647-380d4f4d-0365-47c9-a6ff-77b0b5764f0b.png" width=50% height=50%>

The example structure is as follows:

  - {@city=basement} how is the weather
  - {@city=basement} weather tomorrow
  - {@city=basement} weather tomorrow
  - {@city=kayseri} weekly weather
  - {@city=aksaray} how is the weather today?
  - How is the weather next week in {@city=erzurum}?
  - How is the weather in {@city=elazig}?
  - How is the weather tomorrow in {@city=aksaray}
  - {@city=seali} weather
  - What is the weather for {@city=denizli}
  - {@city=edirne} is it foggy today
  - weather next week
  - what will the weather be like next week {@city=istanbul}
  - next week {@city=istanbul} is it sunny?
  - will it be cold next week?
  - weather
  - weather forecast
  - weather this week
  - weather weekly
  - weather {@city=istanbul}
  - How is the weather
  - how is the weather {@city=samsun}
  - weather tomorrow
  - weather {@city=istanbul}
  - how's the weather
  - how is the weather {@city=izmir}
  - What will the weather be like tomorrow?
  - This week the weather will be like?
  - What will the weather be like in {@city=istanbul} this week?

  @ ml city

@ list time =
    - today :
      - today
      - today
      - today
      - today
      - today's
      - now
      - now
      - now
      - now
    - tomorrow :
      - tomorrow
      - tomorrow
    - weekly :
      - this week
      - next week
      - weekly
      - weekly
      - weekend
      - weekend
      - mid-week
      - mid-week
      - of the week
      - mid-week

### Dialog 2 : Weather Dialogue

After we understand the intents, we can start to create our dialogue by using the entities we have extracted from the incoming sentences.

<img src="https://user-images.githubusercontent.com/14835957/133772337-04526d3f-f172-417a-99c4-9d23ee409acf.png" width=80% height=80%>

There will be 2 issues that we need to focus on while creating the dialog, the first is to create a flow according to the incoming time and city information. The second is to throw the API Request from within the bot.

### 2.1. Segregation According to City and Time Information: If-Else

We get the entities that come from the user in the sentence, the city and time information, if any, in the recognized entities heading. Once we understand that the user wants to check the weather, this will be the first thing we should check. We can pull this with a function from bot composer.

### 'turn.recognized.entities'

<img src="https://user-images.githubusercontent.com/14835957/133773097-467e6abe-f854-4239-86ba-bb85a5dc1f2d.png" width=60% height=60%>

### Has User Specified City Information?

After assigning the 'turn.recognized.entities' concept to a property named dialog.entity, we can control it this way. What we need to do now is create an If-Else condition.

![image](https://user-images.githubusercontent.com/14835957/133773313-8073613b-ee49-412e-9202-9192996d6942.png)

If this block returns True, our recognized entities contain City information, if it returns False, it does not contain City information. We can edit our flow below accordingly.

If the user did not provide city information, that is, if we entered False, we should ask him which city he would like to see the weather forecast for, maybe with a few suggestions!

![image](https://user-images.githubusercontent.com/14835957/133773753-084b5d4d-ca52-4b13-a29e-8f653c26ccaf.png)

![image](https://user-images.githubusercontent.com/14835957/133773790-517af25a-e7c3-47ba-b513-98087a00931e.png)

### Has User Specified Time Range?

The second entity we need to check is whether the user has specified a time. Since we are looking at the City status first, we have to do the Time check in both places, whether it returns True or False from the City control.

![image](https://user-images.githubusercontent.com/14835957/133773569-bd04dc82-d6e5-4bc9-b7c7-8063e1184eab.png)

![image](https://user-images.githubusercontent.com/14835957/133773610-efb69123-f368-4ea1-b122-e18787f9cd2f.png)

If the user didn't specify a time range, we don't need to ask him again. We can return to it the weather conditions of today and the following days.

### 2.2. Retrieve Weather Information: API Request

Once we have our dialog flow in place, we can now retrieve weather information from Azure Maps for each situation.

Reference is made on [Azure Maps API Documentation](https://docs.microsoft.com/en-us/azure/azure-maps/) for this section.

First, the coordinates of this city are drawn from the incoming city information.

![image](https://user-images.githubusercontent.com/14835957/133774679-72c8852f-2c84-4a47-b7de-f27f3b4ea9ed.png)

After the coordinates are obtained, we can query the weather with this coordinate information.

![image](https://user-images.githubusercontent.com/14835957/133774824-e4d57c5c-ba64-4d4c-91a7-7f7ac95b5fc5.png)

## Note

The current application runs in Bot Composer v2.0.0. You can follow [link](https://staticsint.teams.cdn.office.net/evergreen-assets/safelinks/1/atp-safelinks.html) for updates.

## Licence

Copyright (c) Microsoft Corporation. All rights reserved.

Licensed under [MIT License](https://github.com/msft-ai-demos/MICO-BOT/blob/main/LICENSE.md).

## Resources

Project page with suggestions and demos for cognitive services: https://azure.microsoft.com/en-us/services/cognitive-services/

Access link for free trial: https://azure.microsoft.com/free/cognitive-services/

Support channels: Stack Overflow and Azure Support

