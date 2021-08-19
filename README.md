# MICO-BOT
## MICO BOT Nedir?

Miço, sizin Microsoft Teams'deki sanal asistanınız.

Türkiye’deki hava durumlarını şehre göre bugün, yarın, haftalık şeklinde sorgulayabilirsiniz. Piyasa bilgisini sorgulayabilirsiniz, amerikan doları, euro, ingiliz sterlini, japon yeni ve isveç frangı kurlarının güncel rakamlarını görebilirsiniz. Bu kurlar arasında dönüşümler yapabilirsiniz. Güncel haberleri, özel bir konu veya kurum ile ilgili haberleri okuyabilirsiniz. Merak ettiğiniz çoğu şeyi Miço'ya sorabilirisiniz. Miço sizin için Wikipedia’dan öğrenir ve öğrendiklerini size getirir.

Chitchat dosyasını kullanarak miço ile günlük konuşmalar yapabilirsiniz. Aynı zamanda Miço fıkra da anlatabiliyor!

## Prerequistes 


1. An Azure subscription


Create one for free : https://azure.microsoft.com/free/cognitive-services/


2. Download Composer 


Use the tabs below to select an operating system and download Composer : https://docs.microsoft.com/en-us/composer/install-composer?tabs=windows#download-composer


3. Install Node.js with npm


The Node.js JavaScript runtime with the npm package manager ensures Composer supports Node.js templates.

Install Node.js LTS 14.x with npm : https://nodejs.org/

This is a mandatory requirement for use of Composer.


4. Install .NET Core SDK


For C# template support, Composer requires the .NET Core SDK.

Install .NET Core SDK 3.1 or later : https://dotnet.microsoft.com/download/dotnet-core/3.1

This .NET requirement must be addressed if you plan to build bots with C#.


5. Create LUIS (Language Understanding Service) 


https://docs.microsoft.com/en-us/azure/cognitive-services/luis/sign-in-luis-portal


6. Create QnA Maker Service


https://docs.microsoft.com/en-us/azure/cognitive-services/QnAMaker/how-to/set-up-qnamaker-service-azure?tabs=v1


7. Create Bing Maps 


https://docs.microsoft.com/en-us/bingmaps/getting-started/bing-maps-dev-center-help/getting-a-bing-maps-key#:~:text=If%20you%20have%20a%20Bing%20Maps%20account%2C%20sign,Select%20the%20option%20to%20create%20a%20new%20key.


8. Create Bing News 


Once you have your Azure subscription, create a Bing Search resource in the Azure portal to get your key and endpoint. After it deploys, click Go to resource.
https://portal.azure.com/#create/Microsoft.CognitiveServicesBingSearch-v7


9. Create Bing Search


Go to Azure Portal and sign in with your Microsoft account. If you don't have a Microsoft account, click Create one!.

From the portal, type Bing in the search box.

Under Marketplace in the search results, select the Bing service you're interested in (for example, Bing Search or Bing Custom Search).

If you have a free trial or pay account, skip to Create your Bing resource.

On the Create a free account splash screen, click Start free.

Next, you have the option of continuing with the free trial (click Start free again) or paying for an Azure subscription (click Or buy now). You can always start with the free trial and pay for a subscription later.

https://docs.microsoft.com/en-us/bing/search-apis/bing-web-search/create-bing-search-service-resource#create-your-bing-resource


 

Install .NET Core SDK
For C# template support, Composer requires the .NET Core SDK.

Install .NET Core SDK 3.1 or later.

This .NET requirement must be addressed if you plan to build bots with C#.

## Bot Diyalog
**1. Hava Durumu:**

Hava durumu niyeti, Azure Maps ile Türkiye’deki hava durumlarını şehre, tarihe göre, sorgulamanız için eğitilmiştir.

- Ankara hava durumu
- Ankara'da hava nasıl?
- Ankara hava, Ankara hava durumu

sorularına cevap olarak hava durumu kartını getirir;

<img width="250" alt="Picture1" src="https://user-images.githubusercontent.com/89071165/129870634-8099f56e-9c0d-4756-9992-749d8534394a.png">

- hava, hava durumu
- bugün hava nasıl?
- yarın hava, yarın hava nasıl?
- hava nasıl?

gibi sorular için ise, ilk olarak hangi şehrin hava durumunu öğrenmek istediğinizi sorar ve cevabınıza göre şehrin hava durumu kartını getirir.

Yarın hava durumunu öğrenmek isterseniz ve örnek olarak yarın Ankara'da hava nasıl? diye sorarsanız yarının hava durumu kartını getirir;

<img width="200" alt="yarın" src="https://user-images.githubusercontent.com/89071165/129952912-77b0278b-7349-44f2-9fc8-7015091e6ae8.png">

Ayrıca hava durumu için haftalık sorgu da yapabilirsiniz.

- haftalık hava durumu
- İzmir'de haftalık hava
- İzmir'de bu hafta hava nasıl?

gibi sorularınız da haftalık hava durumu kartını getirir;

<img width="200" alt="haftalık" src="https://user-images.githubusercontent.com/89071165/129953284-1f9a0dba-b371-4436-bb70-53a6ca1de4e2.png">



**2. Döviz:**

Döviz niyeti, merkez bankası api’leri ile piyasa bilgisini sorgulayabilme, kurlar arası dönüşüm yapabilme için eğitilmiştir.

- bugün döviz
- döviz
- kurlar

istekleriniz için amerikan doları, euro, ingiliz sterlini, japon yeni ve isveç frangı kurlarının piyasa bilgisi kartını getirir;

<img width="250" alt="Capture" src="https://user-images.githubusercontent.com/89071165/129860982-aede8e1c-2246-457b-9a61-7172c145cc8a.PNG">

- dolar
- bugün dolar

gibi tek kur sorularınız için, hem tl karşılığını hemde alış, satış içeren kartı getirir;

<img width="250" alt="döv" src="https://user-images.githubusercontent.com/89071165/129861869-2df83a2e-7488-45eb-9109-afdf03716f1e.PNG">

- dolar kaç euro?
- 5 dolar kaç euro?

sorularınıza ise kurlar arası dönüşüm yapan kartı getirir;

<img width="250" alt="1" src="https://user-images.githubusercontent.com/89071165/129870191-70a67828-6b7f-4945-a10e-941e2baafe44.PNG">


**3. Bing News:**

Bing News ile güncel haberlere veya bir kurum, konu ile ilgili haberlere erişebilirsiniz.

- gündem
- güncel haberler
- haberler

veya 

- Microsoft haberleri
- spor ile ilgili haberler
- ekonomi haberleri

gibi haber sorgularına karşılık olarak haber kartını getirir;

<img width="170" alt="Picture2" src="https://user-images.githubusercontent.com/89071165/129870691-4c1afd95-424a-4620-99ad-ec83d3ac2e7a.png">



**4. Wiki:**

Bing Search ile Wikipedia'ya erişerek merak ettiklerinizi öğrenebilirsiniz.
Örnek olarak, Miço'ya Microsoft nedir? diye sorduğunuzda Microsoft için wikipedia bilgisini size getirir;

<img width="170" alt="wiki" src="https://user-images.githubusercontent.com/89071165/129871814-f3294402-874a-4ea6-88e7-37bef7b622c7.png">



## QnA Maker Chitchat 

Türkçe olarak oluşturduğumuz soru seti havuzunu kullanarak mico ile günlük konuşmalar gerçekleştirebilirsiniz.

- Mutsuz olduğunuzu ya da kötü bir gün geçirdiğinizi söylerseniz size sanal bir kucaklaşma gönderir.
- Seni seviyorum, evlenelim mi? dediğiniz zaman buna şaşırır.
- Yaşın kaç? Yetişkin misin? gibi sorular sorduğunuzda yaşı olmadığını söyler.

Chitcat dosyasını attachment kısmında bulabilirsiniz.

## Publish


