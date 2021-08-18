# MICO-BOT
## MICO BOT Nedir?

Miço, sizin Microsoft Teams'deki sanal asistanınız.

Türkiye’deki hava durumlarını şehre ve tarihe göre sorgulayabilirsiniz. Piyasa bilgisini sorgulayabilir, kurlar arası dönüşüm yapabilirsiniz. Güncel haberleri veya bir konu ile ilgili haberleri, okuyabilirsiniz. Merak ettiğiniz çoğu şeyi, Miço Wikipedia’dan öğrenir ve size getirir.

Chitchat dosyasını kullanarak miço ile günlük konuşmalar yapabilirsiniz. Aynı zamanda Miço fıkra da anlatabiliyor!

## Prerequistes (bot composer download, Azure subscripiton, luis, bing apilar oluşturma)


## Bot Diyalog
**1. Hava Durumu:**

Hava durumu niyeti, Azure Maps ile Türkiye’deki hava durumlarını şehre, tarihe göre, sorgulamanız için eğitilmiştir.

- Ankara hava durumu
- Ankara'da hava nasıl?
- Ankara'da yarın hava nasıl?
- Ankara hava, Ankara hava durumu

sorularına cevap olarak hava durumu kartını getirir;

<img width="250" alt="Picture1" src="https://user-images.githubusercontent.com/89071165/129870634-8099f56e-9c0d-4756-9992-749d8534394a.png">

- hava, hava durumu
- bugün hava nasıl?
- yarın hava, yarın hava nasıl?
- hava nasıl?

gibi sorular için ise, ilk olarak hangi şehrin hava durumunu öğrenmek istediğinizi sorar ve cevabınıza göre şehrin hava durumu kartını getirir.


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
- 3 dolar kaç euro?

sorularınıza ise kurlar arası dönüşüm yapan kartı getirir;

<img width="250" alt="1" src="https://user-images.githubusercontent.com/89071165/129870191-70a67828-6b7f-4945-a10e-941e2baafe44.PNG">


**3. Bing News:**

Bing News ile güncel haberlere veya bir konu ile ilgili haberlere erişebilirsiniz.

- gündem
- güncel haberler
- haberler

veya 

- Microsoft haberleri
- Microsoft ile ilgili haberler

gibi haber sorgularına karşılık olarak haber kartını getirir;

<img width="170" alt="Picture2" src="https://user-images.githubusercontent.com/89071165/129870691-4c1afd95-424a-4620-99ad-ec83d3ac2e7a.png">



**4. Wiki:**

Bing Search ile Wikipedia'ya erişerek merak ettiklerinizi öğrenebilirsiniz.
Örnek olarak, Miço'ya Microsoft nedir? diye sorduğunuzda Microsoft için wikipedia bilgisini size getirir;

<img width="170" alt="wiki" src="https://user-images.githubusercontent.com/89071165/129871814-f3294402-874a-4ea6-88e7-37bef7b622c7.png">



## QnA Maker Chitchat 

Türkçe olarak oluşturduğumuz soru seti havuzunu kullanarak mico ile günlük konuşmalar gerçekleştirebilirsiniz. Dosyayı attachment kısmında bulabilirsiniz.

## Publish


