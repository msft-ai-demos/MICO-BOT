# MICO-BOT
## Miço Bot Nedir?

Miço, sizin Microsoft Teams'deki sanal asistanınız.

<img src="https://raw.githubusercontent.com/msft-ai-demos/MICO-BOT/main/micologo_small_png.png" width=15% height=15%>

Miço sana bir çok konuda yardımcı olabilecek ve seninle sohbet edebilecek bir sanal asistandır. Ona Türkiye'deki hava durumu bilgilerinden, döviz kurlarına ve dönüşümlerine; güncel haberlerden, ansiklopedi tanımını merak ettiğin bir konuya, kişiye, eşyaya kadar bir çok şeyi sorabilirsin. Onunla Teams'den çıkmadan kısa çeviriler yapabilir, ve ona feedback verebilirsin. Üstelik Miço'yu kendi Teams'ine de kurabilirsin. 

<img src="https://raw.githubusercontent.com/msft-ai-demos/MICO-BOT/main/Mico%20Teams%20Screenshots/mico_teamsmobile1.jpeg" width=25% height=25%>

## [Gereksinimler](#miçoyu-nasıl-kullanabilirim-gereksinimler)
*Miço'yu kullanabilmeniz için gerekli servisler.*

1. [Azure Hesabı](#1-azure-hesabı-oluşturma)
2. [Bot Composer](#2-bot-composer)
* [Node.js ve npm]
* [.NET Core SDK]

3. [Language Understanding Service (LUIS)](#3-language-understanding-service-luis)
4. [QnA Maker](#4-qna-maker)
5. [Bing Maps](#5-bing-maps)
6. [Bing Search](#6-bing-search)
7. [Translate](#7-translate)


## [Kurulum](#miçoyu-nasıl-kullanabilirim-kurulum)
*Miço kurulum aşamaları.*
1. [Miço'yu Kurun!](#1-miçoyu-kurun)
2. [Miço'yu Publish Edin](#2-miçoyu-publish-edin)
3. [Miço'yu Teams'e Ekleyin](#3-miçoyu-teamse-ekleyin)


# Miço'yu Nasıl Kullanabilirim: Gereksinimler

## 1. Azure Hesabı Oluşturma
Ücretsiz [Azure hesabı](https://azure.microsoft.com/en-us/free/cognitive-services/) oluşturun.

## 2. Bot Composer Kurulum
Size uygun işletim sistemini seçerek [Bot Composer](https://docs.microsoft.com/en-us/composer/install-composer?tabs=windows)'ı indirmek için önce [Node.js LTS 14.x](https://nodejs.org/)'i npm ile birlikte ve [.NET Core SDK](https://dotnet.microsoft.com/download/dotnet-core/3.1)'ı indirmelisiniz.

Daha sonra Bot Composer'ı indirip kurabilirsiniz.

<img src="https://raw.githubusercontent.com/msft-ai-demos/MICO-BOT/main/Additional/ss1.png" width=25% height=25%>

### 2.1. Node.js ve npm
Node.js JavaScript platformunu ve npm paketini yüklemeniz Composer'ın Node.js modellerini çalıştırabilmesine imkan tanır. [Node.js LTS 14.x](https://nodejs.org/)'i npm ile birlikte indirin. Bu Composer'ı kullanabilmek için zorunlu bir servistir.

### 2.2. .NET Core SDK
[.NET Core SDK](https://dotnet.microsoft.com/download/dotnet-core/3.1)'ı indirin. C# dilini kullanarak botunuzu oluşturabilmeniz için bu servis gereklidir.

Bot Composer'ı çalıştırın.

<img src="https://raw.githubusercontent.com/msft-ai-demos/MICO-BOT/main/Additional/ss2.png" width=50% height=50%>

## 3. Language Understanding Service (LUIS)
Language Understanding (LUIS), kullanıcıların doğal dil kullanarak uygulamalarınız, botlarınız ve IoT cihazlarınızla etkileşim kurmasına olanak sağlayan bir doğal dil anlama (NLU) yapay zeka hizmetidir. [LUIS](https://docs.microsoft.com/en-us/azure/cognitive-services/luis/sign-in-luis-portal) hizmetini kullanmaya başlayın.

## 4. QnA Maker
Soru-Cevap Oluşturma Servisi, bilgileri kategorilere ayırarak konuşma bağlamında kullanılabilen ve kolayca bulunabilen yanıtlar elde edilmesini sağlar. [Soru-Cevap Oluşturma Servisini](https://docs.microsoft.com/en-us/azure/cognitive-services/QnAMaker/how-to/set-up-qnamaker-service-azure?tabs=v1) kullanmaya başlayın.

## 5. Bing Maps
Bing Haritalar, bir web harita hizmeti arama motorudur. [Bing Haritaları](https://docs.microsoft.com/en-us/bingmaps/getting-started/bing-maps-dev-center-help/creating-a-bing-maps-account) kullanmaya başlayın.

## 6. Bing Search
Bing, Microsoft'un çoklu dilde hizmet veren arama motorudur. Bing'i botunuzda kullanabilmek için Azure Portal üzerinden [Bing Arama Kaynağı](https://docs.microsoft.com/en-us/bing/search-apis/bing-web-search/create-bing-search-service-resource#create-your-bing-resource)'nı oluşturun.

## 7. Translate


# Miço'yu Nasıl Kullanabilirim : Kurulum

## 1. Miço'yu Kurun!
Bot Composer'ı başarılı bir şekilde indirdikten ve gerekli sevisleri oluşturduktan sonra, artık Miço'yu kurmak ve çalıştırmak için yapmanız gerekenlere başlayabilirsiniz.
İlk olarak bu repository'de yer alan Mico-Bot isimli Bot klasörünü lokalinize indirin veya bu repository'yi klonlayın.

Daha Sonra Miço'yu Bot Composer içerisinden açabilmelisiniz.

<img src="https://user-images.githubusercontent.com/14835957/131674595-f2622de3-92e8-46e5-a790-972f8dcf9d56.png" width=50% height=50%>


## 2. Miço'yu Publish Edin


## 3. Miço'yu Teams'e Ekleyin





