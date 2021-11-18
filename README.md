# MICO-BOT
## Miço Bot Nedir?

Miço, sizin Microsoft Teams'deki sanal asistanınız.


<img src="https://raw.githubusercontent.com/msft-ai-demos/MICO-BOT/main/micologo_small_png.png" width=15% height=15%>

Miço size bir çok konuda yardımcı olabilecek ve sohbet edebilecek bir sanal asistandır. Ona Türkiye'deki hava durumu bilgilerinden, döviz kurlarına ve dönüşümlerine; güncel haberlerden, ansiklopedi tanımını merak ettiğiniz bir konuya, kişiye, eşyaya kadar bir çok şeyi sorabilirsiniz. Onunla Teams'den çıkmadan kısa çeviriler yapabilir, ve ona feedback verebilirsiniz. Üstelik Miço'yu kendi Teams'inizde de kurabilirsiniz. 

<p float="left">
  <img src="https://user-images.githubusercontent.com/14835957/133957964-bb5dc633-1aa5-4924-affc-0d50433030b9.jpeg" width=30% height=25% />
  <img src="https://user-images.githubusercontent.com/14835957/133957977-61e3c06c-6e31-4b71-b36a-adc002e70fe8.jpeg" width=25% height=25% /> 
  <img src="https://user-images.githubusercontent.com/14835957/133957989-b65c0daa-d799-4b90-9acf-147d525bc60e.jpeg" width=25% height=25% /> 
</p>

<p float="left">
  <img src="https://user-images.githubusercontent.com/14835957/133958000-b8bac881-d2cb-4b77-a27c-c8c0075b09c5.jpeg" width=25% height=25% />
  <img src="https://user-images.githubusercontent.com/14835957/133958007-8dff7f60-0c35-4545-acf8-c974dc00e0a0.jpeg" width=25% height=25% /> 
</p>

## [Gereksinimler](#miçoyu-nasıl-kullanabilirim-gereksinimler)
*Miço'yu kullanabilmeniz için gerekli servisler.*

1. [Azure Hesabı](#1-azure-hesabı-oluşturma)
2. [Bot Composer](#2-bot-composer-kurulum)
3. [Language Understanding Service (LUIS)](#3-language-understanding-service-luis)
4. [QnA Maker - Optional](#4-qna-maker---optional)
5. [Bing Maps](#5-bing-maps)
6. [Bing Search](#6-bing-search)


## [Kurulum](#miçoyu-nasıl-kullanabilirim--kurulum)
*Miço kurulum aşamaları.*
1. [Miço'yu Kurun!](#1-miçoyu-kurun)
2. [Miço'yu Publish Edin](#2-miçoyu-publish-edin)
3. [Miço'yu Teams'e Ekleyin](#3-miçoyu-teamse-ekleyin)


## [Yeni Bir Niyet Nasıl Eklenir?](#yeni-bir-niyet-ve-dialog-nasıl-eklenir)
1. [Hava Durumu Niyeti](#1-niyet--hava-durumu-niyeti)
2. [Hava Durumu Dialoğu](#2-dialog--hava-durumu-dialoğu)



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

## 7. Merkez Bankası API -Optional
Botun güncel döviz bilgilerine ulaşabilmesi için [Merkez Bankası EVDS Web Servis Dokumantasyonu](https://evds2.tcmb.gov.tr/help/videos/EVDS_Web_Servis_Kullanim_Kilavuzu.pdf)'nu takip ederek key oluşturabilirsiniz. 


# Miço'yu Nasıl Kullanabilirim : Kurulum

## 1. Miço'yu Kurun!
Bot Composer'ı başarılı bir şekilde indirdikten ve gerekli sevisleri oluşturduktan sonra, artık Miço'yu kurmak ve çalıştırmak için yapmanız gerekenlere başlayabilirsiniz.
İlk olarak bu repository'de yer alan Mico-Bot isimli Bot klasörünü lokalinize indirin veya bu repository'yi klonlayın.

Extract ettiğiniz bot dosyasını composerı açarak, composer içerisinden seçip bulun.

Daha Sonra Miço'yu Bot Composer içerisinden açabilmelisiniz.

<img src="https://user-images.githubusercontent.com/14835957/131674595-f2622de3-92e8-46e5-a790-972f8dcf9d56.png" width=50% height=50%>


## 2. Miço'yu Publish Edin

Miço'yu publish edebilmek için yapmanız gereken ilk şey, bir Publishing Profile oluşturmak. Bu adımı tamamen composer içerisinden tamamlayabilirsiniz. 

![image](https://user-images.githubusercontent.com/14835957/133958169-b4069ba8-4acd-4053-887f-b2daf5faeac3.png)

Eğer LUIS, QnA maker gibi kaynakları Azure Portal'da çoktan oluşturduysanız, import existing resources seçeneğinden kaynaklarınızın endpointlerini ve keylerini doldurarak bir Publishing Profile oluşturabilirsiniz. Publishing profile oluştururken, luis bağlantısını kurmak için, görseldeki gibi "luisResource" bölümüne luis prediction resource ismini eklemelisiniz.

![image](https://user-images.githubusercontent.com/25666677/142438454-9f56e3e1-f03f-4428-ada9-f3ae321347e4.png)

Eğer daha önce hiç kaynak açmadıysanız Create new resources seçeneğiyle bu kaynakları Bot Composer üzerinden oluşturabilir ve Publishing Profile'ınıza ekleyebilirsiniz.
Daha sonra Publishing Profile'ınızı seçerek Publish selected bots seçeneğine tıklamanız yeterli olacaktır. 

## 3. Miço'yu Teams'e Ekleyin

Publish etmiş olduğunuz botu Teams'e ekleyebilmeniz için tamamlamanız gereken bir kaç adım kaldı. Bu adımları Azure Portal içerisinden tamamlayacağız. Publish edilmiş botunuzu Azure Portal'dan açtığınızda Channels tabında botunuzu entegre edebileceğiniz kanalları görebilirsiniz. Bu kanallardan Teams'i seçerek botunuzu Teams üzerinde konumlandırabilirsiniz. 

![image](https://user-images.githubusercontent.com/25666677/142224934-07e6cc97-d9e0-4304-927d-08ca9c905fad.png)


# Yeni Bir Niyet ve Dialog Nasıl Eklenir?
## Örnek: Hava Durumu Niyeti ve Dialoğu

Miço'yu kullanırken ona farklı özellikler eklemek isteyebilirsiniz. Bunun için ilk olarak bu özellikle ilişkilendirilecek niyeti belirlemeniz gerekmektedir. Örnek olarak, Miço'ya hava durumunu söyleme yetisi eklemek istediğinizde, burada anlamanız gereken niyet, hava durumudur. Kullanıcıdan gelebilecek hava durumu ile ilgili sorular, Miço'nun doğal dil anlama yeteneği ile ayrıştırılıp, Hava Durumu Niyetini tetiklemelidir. 

Niyeti oluşturup kullanıcıdan gelen talepleri doğru anlarken, bir yandan da dialogu oluşturmaya başlayabilirsiniz. Niyet içerisinden ayıklayabileceğiniz entity'ler, dialoğunuzun akışını da şekillendirecektir.

Miço'ya yeni bir özellik eklerken ilerleyişiniz konusunda rehber olması için, hava durumu niyetini ve dialoğunu baştan nasıl oluşturabileceğinizi aşağıda bulabilirsiniz.

### 1. Niyet : Hava Durumu Niyeti

Niyetleri oluştururken ister Bot Composer içerisinden, ister LUIS'in kendi arayüzünden oluşturabilirsiniz. Bu örnekte Hava Durumu niyeti LUIS'in kendi arayüzü olan luis.ai sitesi üzerinden oluşturulacaktır. [LUIS.AI](https://www.luis.ai)

<img src="https://user-images.githubusercontent.com/14835957/133092774-0df8fd6d-915b-4fdd-a7a5-10f23a56593a.png" width=50% height=50%>

Luis Portalı içerisinde yapmanız gereken ilk şey, +New App diyerek yeni bir proje oluşturmak. MicoIntents isimli bir proje oluşturabilirsiniz. Bu app i oluştururken sizden Azure Portal üzerinden açmış olduğunuz LUIS servisine dair LUIS Prediction Resource'unu seçmeniz istenecek. 

Projeyi oluşturduktan sonra, artık Intent, yani niyet yaratabiliriz. + Intent diyerek 'HavaDurumu' isminde bir niyet ekleyiniz. 

1) Niyeti oluşturduktan sonra, ilk olarak kullanıcılardangelebilecek bir kaç örnek cümleyi ekleyelim.

- Hava nasıl?
- Hava durumu nedir
- Hava nasıl olacak
- hava durumu

<img src="https://user-images.githubusercontent.com/14835957/133099693-1d87d82a-c3d5-48c9-bbe6-22dbb7518d55.png" width=50% height=50%>

Kullanıcıdan gelen cümleler bu şekilde direkt hava durumunu soruyorsa, onlara şehri biz sorabiliriz. Dialoğumuzun akışını da bu şekilde oluşturmamız gerekecek. Bu birinci duruma Dialog kısmında değineceğiz.

2) Eğer kullanıcı, şehri de belirterek hava durumunu soruyorsa, onlara bir daha bu soruyu sormamak için, gelen cümledeki şehir kavramını yakalamalıyız.
Bunun için bir entity oluşturmalıyız.

Soldaki Entities kısmına gelerek, + Create Entity diyebiliriz.

<img src="https://user-images.githubusercontent.com/14835957/133101481-441377b8-f5a1-4fa0-9c83-b20dcaea36c8.png" width=50% height=50%>

Burada karşımıza bir kaç seçenek çıkmakta.

- [List Entity](https://docs.microsoft.com/tr-tr/azure/cognitive-services/luis/luis-concept-entity-types#list-entity): Sabit ve kapalı bir ilgili sözcük kümesini eş anlamlılarıyla birlikte temsil eder. Birden çok eş anlamlı veya çeşitlemeyi tanımak ve bunlara yönelik normalleştirilmiş bir çıktıyı ayıklamak için liste varlıklarını kullanabilirsiniz. Örnek: Haftanın Günleri.
- [Regex Entity](https://docs.microsoft.com/tr-tr/azure/cognitive-services/luis/luis-concept-entity-types#regex-entity): Normal ifade, yapılandırılmış metin veya belirli bir biçimde beklenen, önceden tanımlanmış alfasayısal değerler dizisi için idealdir. Örnek: Uçuş Numaraları, Kimlik Numaraları ...
- [Machine Learned Entity](https://docs.microsoft.com/tr-tr/azure/cognitive-services/luis/luis-concept-entity-types#machine-learned-ml-entity): Makine tarafından öğrenilen varlık, etiketlenmiş örneklere göre varlıkları ayıklamak için bağlamını kullanır. Makine öğrenimi algoritmalarını kullanır ve etiketlemeye, uygulamanıza başarıyla uyarlanmasını gerektirir. Örnek: Kişi isimleri.
- [Daha Fazlası](https://docs.microsoft.com/tr-tr/azure/cognitive-services/luis/luis-concept-entity-types)

3. Miçoya ekleyeceğimiz ilk Entity, kullanıcıdan gelebilecek zaman aralığı olacak. Kullanıcı cümle içinde bir zaman aralığı vermezse, ona bugünün ve sonraki günlerin hava durumunu verebiliriz. Ama kullanıcı yarını öğrenmek istiyorsa, ya da haftalık detaylı sonuçları görmek istiyorsa, bunu da anlamalıyız. Zaman aralığı entitysi için Liste tipinde entity oluşturacağız. Liste'nin üç elemanı olacak: Bugün, Yarın, Haftalık.

<img src="https://user-images.githubusercontent.com/14835957/133231586-f520fdf8-154d-45f4-af52-614dfce67475.png" width=50% height=50%>

4. Bir sonraki enity'miz ise, kullanıcının hava durumunu sorarken şehri de belirtme ihtimaline karşın üreteceğimiz Şehir entity'si olacak. Bu entity'yi Machine Learned entity tipinde oluşturacağız, bu sayede, kullanıcının girebileceği tüm şehir örneklerini LUIS'e vermeden, onun öğrenme yeteneğinden faydalanarak, sadece bir kaç örnekle ona şehir kısmını yakalamayı öğretebiliriz.

Tekrar HavaDurumu Intent'ine gidip örnek phraseler girmeye başlayalım. Bu sefer içlerinde şehir de olsun. Daha sonra bu şehirleri seçip, oluşturduğumuz Machine Learned Şehir entity'si ile eşleştirelim.

<img src="https://user-images.githubusercontent.com/14835957/133232461-f139ef04-81da-4ba9-a3f8-16ba2b79909b.png" width=50% height=50%>

Bir kaç örnekle daha çeşitlendirdikten sonra, sağ üst köşeden Train diyip, sonrasında örnek cümlelerle test edebilirsiniz.

Intent ve entity'lerimizi tamamladıktan sonra, artık bu formatı Bot Composer içerisine de ekleyebiliriz. Bunun için LUIS portal anasayfasına gidip, app'inizi seçip, export as .lu file demelisiniz. 

<img src="https://user-images.githubusercontent.com/14835957/133232861-0e8190e6-b14f-4cf9-9dd7-788cb3f5a19b.png" width=50% height=50%>

Export ettiğimiz .lu dosyasının içeriğini, bot içerisindeki havadurumu triggerında kullanmalıyız. 

<img src="https://user-images.githubusercontent.com/14835957/133771647-380d4f4d-0365-47c9-a6ff-77b0b5764f0b.png" width=50% height=50%>

Bu dosyanın içeriğini ilgili dosyadan bulabilirsiniz. Örnek yapı aşağıdaki gibidir:

  - {@city=bodrum} hava nasıl
  - {@city=bodrum} yarın hava
  - {@city=bodrum} yarın hava
  - {@city=kayseri} haftalık hava
  - {@city=aksaray} bugün hava nasıl?
  - {@city=erzurum}'da haftaya hava nasıl?
  - {@city=elazig}'da hava nasıl?
  - {@city=aksaray}'da yarın hava nasıl
  - {@city=denizli} hava
  - {@city=denizli} hava durumu nedir
  - {@city=edirne} sisli mi bugun
  - haftaya hava
  - haftaya hava nasıl olacak {@city=istanbulda}
  - haftaya {@city=istanbul} güneşli mi?
  - haftaya soguk mu olacak?
  - hava
  - hava durumu
  - hava durumu bu hafta
  - hava durumu haftalık
  - hava durumu {@city=istanbul}
  - hava durumu nasıl
  - hava durumu nasıl {@city=samsun}
  - hava durumu yarın
  - hava {@city=istanbul}
  - hava nasıl
  - hava nasıl {@city=izmir}
  - hava nasıl olacak yarın
  - bu hafta hava nasıl olacak?
  - bu hafta hava {@city=istanbul}'da nasıl olacak?

  @ ml city

  @ list zaman = 
    - bugun :
      - bugun
      - bugün
      - bugünkü
      - bugunun
      - bugünün
      - suan
      - şuan
      - simdi
      - şimdi
    - yarin :
      - yarın
      - yarin
    - haftalik :
      - bu hafta
      - haftaya
      - haftalık
      - haftalik
      - haftasonu
      - hafta sonu
      - hafta içi
      - haftaiçi
      - haftanın
      - haftaici



### 2. Dialog : Hava Durumu Dialoğu

Niyetleri anladıktan sonra artık gelen cümlelerden ayıkladığımız entity'leri de kullanarak dialoğumuzu oluşturmaya başlayabiliriz.

<img src="https://user-images.githubusercontent.com/14835957/133772337-04526d3f-f172-417a-99c4-9d23ee409acf.png" width=80% height=80%>

Dialog oluştururken üzerinde durmamız gereken 2 konu olacak, ilki, gelen zaman ve şehir bilgisine göre bir akış oluşturmak. İkincisi ise, API Request'i bot içerisinden atmak.

### 2.1. Şehir ve Zaman Bilgisine göre Ayrışmalar: If-Else

Kullanıcıdan cümle içerisinde gelen entityleri, bizim durumumuzda varsa şehir ve zaman bilgisini, recognized entities başlığında almaktayız. Kullanıcının hava durumuna bakmak istediğini anladıktan sonra, ilk kontrol etmemiz gereken şey bu olacak. Bu, bot composer içerisinden bir fonksiyon ile çekebilmekteyiz. 

### 'turn.recognized.entities'

<img src="https://user-images.githubusercontent.com/14835957/133773097-467e6abe-f854-4239-86ba-bb85a5dc1f2d.png" width=60% height=60%>

### Kullanıcı Şehir Bilgisi Girmiş mi?

'turn.recognized.entities' kavramını, dialog.entity isimli bir property'ye atadıktan sonra, bu şekilde de kontrol edebiliriz. Şimdi yapmamız gereken, bir If-Else koşulu oluşturmak.

![image](https://user-images.githubusercontent.com/14835957/133773313-8073613b-ee49-412e-9202-9192996d6942.png)

Bu blok, True dönüyorsa, tanınan entitylerimiz Şehir bilgisi içeriyor, False dönüyorsa, Şehir bilgisi içermiyor demektir. Aşağıdaki akışımızı buna göre düzenleyebiliriz.

Kullanıcı şehir bilgisi vermediyse, yani False'a girdiysek, hangi şehrin hava durumuna bakmak isteediğini biz ona sormalıyız, belki bir kaç öneri ile!

![image](https://user-images.githubusercontent.com/14835957/133773753-084b5d4d-ca52-4b13-a29e-8f653c26ccaf.png)

![image](https://user-images.githubusercontent.com/14835957/133773790-517af25a-e7c3-47ba-b513-98087a00931e.png)

### Kullanıcı Zamar Aralığı Belirtmiş mi?

Kontrol etmemiz gereken ikinci varlık, kullanıcının zaman belirtip belirtmediği. İlk olarak Şehir durumuna baktığımız için, Zaman kontrolünü iki yerde de yapmalıyız, Şehir kontrolünden True dönüyorsa da, False dönüyorsa da.

![image](https://user-images.githubusercontent.com/14835957/133773569-bd04dc82-d6e5-4bc9-b7c7-8063e1184eab.png)

![image](https://user-images.githubusercontent.com/14835957/133773610-efb69123-f368-4ea1-b122-e18787f9cd2f.png)

Kullanıcı zaman aralığı belirtmediyse, ona bir daha sormamıza gerek yok. Bugünün ve ilerleyen günlerin hava durumunu ona dönebiliriz.


### 2.2. Hava Durumu Bilgisini Çekmek: API Request

Dialog akışımızı oturttuktan sonra, artık her durum için Azure Maps'ten hava durumu bilgisini çekebiliriz.

Bu kısım için [Azure Maps API Dökümantasyonu](https://docs.microsoft.com/en-us/azure/azure-maps/) referans alınmıştır. 

İlk olarak gelen şehir bilgisinden, bu şehrin koordinatları çekilmekte.

![image](https://user-images.githubusercontent.com/14835957/133774679-72c8852f-2c84-4a47-b7de-f27f3b4ea9ed.png)

Koordinatlar elde edildikten sonra, bu koordinat bilgisi ile hava durumuna sorgu atabiliriz.

![image](https://user-images.githubusercontent.com/14835957/133774824-e4d57c5c-ba64-4d4c-91a7-7f7ac95b5fc5.png)

## Not

Mevcut uygulama Bot Composer v2.0.0 içerisinde çalışmaktadır. Güncellemeler için [linkini](https://staticsint.teams.cdn.office.net/evergreen-assets/safelinks/1/atp-safelinks.html) takip edebilirsiniz.

## Lisans

Telif Hakkı (c) Microsoft Corporation. Tüm hakları saklıdır.

[MIT Lisansı](https://github.com/msft-ai-demos/MICO-BOT/blob/main/LICENSE.md) altında lisanslıdır. 

## Kaynaklar
Bilişsel hizmetlere ait önerileri ve demoları içeren proje sayfası: https://azure.microsoft.com/en-us/services/cognitive-services/

Ücretsiz deneme için erişim linki: https://azure.microsoft.com/free/cognitive-services/

Destek kanalları: Stack Overflow ve Azure Destek

