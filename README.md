# MICO-BOT
## MICO BOT Nedir?

Miço, sizin Microsoft Teams'deki sanal asistanınız.

Türkiye’deki hava durumlarını şehre göre bugün, yarın, haftalık şeklinde sorgulayabilirsiniz. Piyasa bilgisini sorgulayabilirsiniz, amerikan doları, euro, ingiliz sterlini, japon yeni ve isveç frangı kurlarının güncel rakamlarını görebilirsiniz. Bu kurlar arasında dönüşümler yapabilirsiniz. Güncel haberleri, özel bir konu veya kurum ile ilgili haberleri okuyabilirsiniz. Merak ettiğiniz çoğu şeyi Miço'ya sorabilirisiniz. Miço sizin için Wikipedia’dan öğrenir ve size getirir.

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

Yarın hava durumunu öğrenmek isterseniz 
Bugün hava durumu
Haftalık hava durumu


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
- Ona, Miço bana bir soru sor dediğiniz zaman soru sormayabilir çünkü soruları cevaplamakta daha iyidir.

Chitcat dosyasını attachment kısmında bulabilirsiniz.

## Publish


