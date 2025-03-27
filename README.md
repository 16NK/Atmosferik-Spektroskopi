# Atmosferik-Spektroskopi
Doğrudan Görüntüleme Yapılan Ötegezegenlerde Molekül ve Bileşiklerin Geçiş Yoğunlukları Üzerinden Spektroskopik Analiz Yazılımına ait kodların açıklamasıdır.
## 1. Basamak
- Bu kod, seçtiğiniz molekülün/bileşiğin verilerini indirir. 
- Yüksek geçiş yoğunluklarını belirler. 
- Çıktıları tablo ve grafik halinde kullanıcıya sunar. 

Not: Kod içerisinde bulunan yorum satırlarına göre analiz etmek istediğiniz molekülü/bileşiği değiştirebilirsiniz.
### 1. Basamak Kodu çalıştırılır:
[NASA Exoplanet Archive Atmospheric Spectroscopy](https://exoplanetarchive.ipac.caltech.edu/cgi-bin/atmospheres/nph-firefly?atmospheres) bölümünden seçtiğiniz doğrudan görüntüleme ile verisi alınan bir gezegenin dalga boyu (Central Wave. Başlığı'nın altındaki veriler) değerlerini virgül ile ayırarak boşluk bırakmadan girmeniz istenir.

Örnek: 1.88609,1.89468,1.90326,1.91184,1.92043,1.92901,1.93759,1.94618,1.95476,1.96335,1.97193,1.98051,1.9891,1.99768,2.00626,2.01485,2.02343,2.03202,2.0406,2.04918,2.05777,2.06635,2.07494,2.08352,2.0921,2.10069,2.10741,2.10927,2.11544

**1. Kodun çıktısı:**
Seçtiğiniz molekülün/bileşiğin geçiş yoğunluğunun en yüksek olduğu dalga boyu aralığını grafikte gösterir ve bu aralık değerini sayısal olarak ekrana yansıtır.

![1. Kodun Çıktısı](https://github.com/16NK/Atmosferik-Spektroskopi/blob/main/H%C4%B1tran'dan%20Al%C4%B1nan%20H2O%20Ge%C3%A7i%C5%9F%20Yo%C4%9Funlu%C4%9Fu%20Spektrumu.png)
## 2. Basamak 
- Bu kod, gezegene ait verileri kullanıcıdan alır.
- Düşük akı noktalarını belirler.
- Çıktıları tablo ve grafik halinde kullanıcıya sunar.

### 2. Basamak Kodu çalıştırılır:
NASA Exoplanet Archive Atmospheric Spectroscopy bölümünden seçtiğiniz doğrudan görüntüleme ile verisi alınan bir gezegenin dalga boyu (Central Wave. başlığının altındaki veriler) değerlerini ve akı (F_lambda başlığının altındaki veriler) değerlerini virgül ile ayırarak boşluk bırakmadan sizden istediği sırayla giriniz.

Bu iki başlıktan alınan verilerin sayısı aynı olmalıdır.

Örnek dalga boyu değerleri: 1.88609,1.89468,1.90326,1.91184,1.92043,1.92901,1.93759,1.94618,1.95476,1.96335,1.97193,1.98051,1.9891,1.99768,2.00626,2.01485,2.02343,2.03202,2.0406,2.04918,2.05777,2.06635,2.07494,2.08352,2.0921,2.10069,2.10741,2.10927,2.11544

Örnek akı değerleri: 9.78085e-19,2.3454e-17,9.5808e-18,1.08605e-17,5.72937e-18,2.37444e-18,0.0,1.12146e-17,1.48532e-17,1.58714e-17,2.20621e-17,1.84841e-17,1.82458e-17,1.45657e-17,1.55634e-17,1.70932e-17,2.69893e-17,2.72315e-17,2.96508e-17,3.11709e-17,3.68426e-17,3.49629e-17,3.63232e-17,4.01372e-17,4.08904e-17,4.10719e-17,3.56583e-17,3.89937e-17,3.58879e-17

**2. Kodun çıktısı:**
Bilgilerini girdiğiniz gezegenin akı değerinin en düşük olduğu dalga boylarını bir tablo halinde ekrana yansıtacak ve düşük akı değerlerini gezegenin spektrum grafiği üzerinde işaretlenmiş olarak gösterecektir.

![2. Kodun Çıktısı](https://github.com/16NK/Atmosferik-Spektroskopi/blob/main/Gezegen%20Spektrumu%20ve%20Ak%C4%B1%20D%C3%BC%C5%9F%C3%BC%C5%9F%20Noktalar%C4%B1.png)
## 3. Basamak:
- Birinci ve ikinci koddan gelen verileri analiz eder.
- Gezegende belirlenen molekülün/bileşiğin var olup olmadığını kullanıcıya sunar.
- Eğer seçilen molekül/bileşik gezegende tespit edilirse tespit edildiği nokta grafik üzerinde işaretlenir.

### 3. Basamak Kodu çalıştırılır:
- Birinci koddan aldığınız çıktıyı şu formatta giriniz: 1.90 - 1.91 µm
- İkinci koddan aldığınız çıktı içerisindeki akı düşüşlerine denk gelen akı değerlerini virgül ile ayırarak boşluk bırakmadan giriniz.

Örnek: Akı Değerinin En Düşük Olduğu Dalga Boyları:

Dalga Boyu: 1.9033 µm, Akı: 9.5808e-18

Dalga Boyu: 1.9376 µm, Akı: 0.0000e+00

Dalga Boyu: 1.9977 µm, Akı: 1.4566e-17

Dalga Boyu: 2.0663 µm, Akı: 3.4963e-17

Dalga Boyu: 2.1074 µm, Akı: 3.5658e-17

Yukarıda 2. kod için örnek bir çıktı verilmiştir. 3. koda ikinci sırada vereceğiniz veriler şu formatta olmalıdır: 1.9033,1.9376,1.9977,2.0663,2.1074

- Ardından, NASA Exoplanet Archive Atmospheric Spectroscopy bölümünden seçtiğiniz doğrudan görüntüleme ile verisi alınan bir gezegenin dalga boyu (Central Wave. başlığının altındaki veriler) değerlerini giriniz. 

- Aynı gezegene ait akı (F_lambda başlığının altındaki veriler) değerlerini virgül ile ayırarak boşluk bırakmadan giriniz.

Bu iki başlıktan alınan verilerin sayısı aynı olmalıdır.

**3. Kodun Çıktısı:**
Eğer analiz ettiğiniz molekül/bileşik gezegende tespit edilirse alacağınız çıktı " Molekül/Bileşik tespit edildi!" olacak, tespit edildiği dalga boyu değeri ise ekrana yansıtılacaktır. 

Örnek çıktı: "Dalga Boyu: 1.9033 µm, bu aralıkta element tespit edildi!"

![2. Kodun Çıktısı](https://github.com/16NK/Atmosferik-Spektroskopi/blob/main/Gezegen%20Spektrumunda%20%C4%B0lgili%20Elementin%20Tespit%20Edildi%C4%9Fi%20Aral%C4%B1k.png)
