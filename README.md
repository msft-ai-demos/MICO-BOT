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
3. [Language Understanding Service (LUIS)](#3-language-understanding-service-luis)
4. [QnA Maker - Optional](#4-qna-maker)
5. [Bing Maps](#5-bing-maps)
6. [Bing Search](#6-bing-search)


## [Kurulum](#miçoyu-nasıl-kullanabilirim--kurulum)
*Miço kurulum aşamaları.*
1. [Miço'yu Kurun!](#1-miçoyu-kurun)
2. [Miço'yu Publish Edin](#2-miçoyu-publish-edin)
3. [Miço'yu Teams'e Ekleyin](#3-miçoyu-teamse-ekleyin)


## [Yeni Bir Niyet Nasıl Eklenir?](#yeni-bir-niyet-ve-dialog-nasıl-eklenir)

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

## 4. QnA Maker - Optional
Soru-Cevap Oluşturma Servisi, bilgileri kategorilere ayırarak konuşma bağlamında kullanılabilen ve kolayca bulunabilen yanıtlar elde edilmesini sağlar. [Soru-Cevap Oluşturma Servisini](https://docs.microsoft.com/en-us/azure/cognitive-services/QnAMaker/how-to/set-up-qnamaker-service-azure?tabs=v1) kullanmaya başlayın.

## 5. Bing Maps
Bing Haritalar, bir web harita hizmeti arama motorudur. [Bing Haritaları](https://docs.microsoft.com/en-us/bingmaps/getting-started/bing-maps-dev-center-help/creating-a-bing-maps-account) kullanmaya başlayın.

## 6. Bing Search
Bing, Microsoft'un çoklu dilde hizmet veren arama motorudur. Bing'i botunuzda kullanabilmek için Azure Portal üzerinden [Bing Arama Kaynağı](https://docs.microsoft.com/en-us/bing/search-apis/bing-web-search/create-bing-search-service-resource#create-your-bing-resource)'nı oluşturun.




# Miço'yu Nasıl Kullanabilirim : Kurulum

## 1. Miço'yu Kurun!
Bot Composer'ı başarılı bir şekilde indirdikten ve gerekli sevisleri oluşturduktan sonra, artık Miço'yu kurmak ve çalıştırmak için yapmanız gerekenlere başlayabilirsiniz.
İlk olarak bu repository'de yer alan Mico-Bot isimli Bot klasörünü lokalinize indirin veya bu repository'yi klonlayın.

Daha Sonra Miço'yu Bot Composer içerisinden açabilmelisiniz.

<img src="https://user-images.githubusercontent.com/14835957/131674595-f2622de3-92e8-46e5-a790-972f8dcf9d56.png" width=50% height=50%>


## 2. Miço'yu Publish Edin


## 3. Miço'yu Teams'e Ekleyin




# Yeni Bir Niyet ve Dialog Nasıl Eklenir?
## Örnek: Hava Durumu Niyeti ve Dialoğu

Miço'yu kullanırken ona farklı özellikler eklemek isteyebilirsiniz. Bunun için ilk olarak bu özellikle ilişkilendirilecek niyeti belirlemeniz gerekmektedir. Örnek olarak, Miço'ya hava durumunu söyleme yetisi eklemek istediğinizde, burada anlamanız gereken niyet, hava durumudur. Kullanıcıdan gelebilecek hava durumu ile ilgili sorular, Miço'nun doğal dil anlama yeteneği ile ayrıştırılıp, Hava Durumu Niyetini tetiklemelidir. 

Niyeti oluşturup kullanıcıdan gelen talepleri doğru anlarken, bir yandan da dialogu oluşturmaya başlayabilirsiniz. Niyet içerisinden ayıklayabileceğiniz entity'ler, dialoğunuzun akışını da şekillendirecektir.

Miço'ya yeni bir özellik eklerken ilerleyişiniz konusunda rehber olması için, hava durumu niyetini ve dialoğunu baştan nasıl oluşturabileceğinizi aşağıda bulabilirsiniz.

### 1. Niyet : Hava Durumu Niyeti

Niyetleri oluştururken ister Bot Composer içerisinden, ister LUIS'in kendi arayüzünden oluşturabilirsiniz. Bu örnekte Hava Durumu niyeti LUIS'in kendi arayüzü olan luis.ai sitesi üzerinden oluşturulacaktır. [LUIS.AI](https://www.luis.ai)

<img src="https://user-images.githubusercontent.com/14835957/133092774-0df8fd6d-915b-4fdd-a7a5-10f23a56593a.png" width=25% height=25%>

Luis Portalı içerisinde yapmanız gereken ilk şey, +New App diyerek yeni bir proje oluşturmak. MicoIntents isimli bir proje oluşturabilirsiniz. Bu app i oluştururken sizden Azure Portal üzerinden açmış olduğunuz LUIS servisine dair LUIS Prediction Resource'unu seçmeniz istenecek. 

Projeyi oluşturduktan sonra, artık Intent, yani niyet yaratabiliriz. + Intent diyerek 'HavaDurumu' isminde bir niyet ekleyiniz. 

1) Niyeti oluşturduktan sonra, ilk olarak kullanıcılardangelebilecek bir kaç örnek cümleyi ekleyelim.

- Hava nasıl?
- Hava durumu nedir
- Hava nasıl olacak
- hava durumu

<img src="https://user-images.githubusercontent.com/14835957/133099693-1d87d82a-c3d5-48c9-bbe6-22dbb7518d55.png" width=25% height=25%>

Kullanıcıdan gelen cümleler bu şekilde direkt hava durumunu soruyorsa, onlara şehri biz sorabiliriz. Dialoğumuzun akışını da bu şekilde oluşturmamız gerekecek. Bu birinci duruma Dialog kısmında değineceğiz.

2) Eğer kullanıcı, şehri de belirterek hava durumunu soruyorsa, onlara bir daha bu soruyu sormamak için, gelen cümledeki şehir kavramını yakalamalıyız.
Bunun için bir entity oluşturmalıyız.

Soldaki Entities kısmına gelerek, + Create Entity diyebiliriz.
<img src="https://user-images.githubusercontent.com/14835957/133101481-441377b8-f5a1-4fa0-9c83-b20dcaea36c8.png" width=25% height=25%>
Burada karşımıza bir kaç seçenek çıkmakta.
- [Machine Learned Entity](https://docs.microsoft.com/tr-tr/azure/cognitive-services/luis/luis-concept-entity-types#machine-learned-ml-entity):
- [List Entity](https://docs.microsoft.com/tr-tr/azure/cognitive-services/luis/luis-concept-entity-types#list-entity): Sabit ve kapalı bir ilgili sözcük kümesini eş anlamlılarıyla birlikte temsil eder. Birden çok eş anlamlı veya çeşitlemeyi tanımak ve bunlara yönelik normalleştirilmiş bir çıktıyı ayıklamak için liste varlıklarını kullanabilirsiniz. 
- [Regex Entity](https://docs.microsoft.com/tr-tr/azure/cognitive-services/luis/luis-concept-entity-types#regex-entity):
- [Pattern Entity]():

### 2. Dialog : Hava Durumu Dialoğu


