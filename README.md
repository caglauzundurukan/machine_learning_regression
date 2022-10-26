## Denetimli öğrenme algoritmaları: Regresyon (Basit Doğrusal regresyon ve çoklu regresyon) nedir, çalışma mantığı nedir, kullanım alanları, örnekleri.
![Beige Nude Business Organization Chart](https://user-images.githubusercontent.com/73706248/198099903-bdebf4c3-694a-44d8-b18a-b631f0b36351.png)
**Denetimli öğrenme**; aldığı veriler ve ürettiği sonuçlara dayalı olarak bir model geliştirme işlemidir. Diğer makine öğrenmesi türlerine kıyasla denetimli öğrenmenin en büyük farkı veri etiketi kullanılmasıdır. Etiketlediğimiz veriye, gösterdiğimiz sınıf ve bilgiye göre mevcut gerçekliğe dayanarak model geliştirme algoritmasıdır.

# Regresyon Nedir?
**Regresyon**, bir bağımlı değişken (genellikle Y ile gösterilir) ve diğer bağımsız değişkenler arasındaki ilişkinin gücünü ve karakterini belirlemeye çalışan finans, yatırım, makine öğrenmesi ve diğer disiplinlerde kullanılan istatistiksel bir yöntemdir.

**Bağımlı Değişken:** Anlamaya veya tahmin etmeye çalıştığımız değişkendir.  <br>
**Bağımsız Değişken:** Analizi veya hedef değişkeni etkileyen ve değişkenlerin hedef değişkenle ilişkisi hakkında bize bilgi veren faktörlerdir.

## Makine Öğrenmesinde Regresyon
Makine öğrenmesinde regresyon ise kısaca makinenin veri setini ezberlememesi için oluşturulan algoritmadır. İstenen sonuç makinenin ezberlemesi değil **“öğrenmesi”** yani tutarlı tahmin yeteneğine sahip olmasıdır.
<br> <br>
Yöntem olarak bir eğitim kümesi ve eğitim kümesinden makine öğrenmesi metotları ile bir model elde edilip bu model üzerinden yeni gelen veriler tahmin edilmeye çalışılır.
<br> <br>
Regresyon yönteminde tahmin sonucu kategorik değil nümerik bir değer olmalıdır. Örneğin:
<br>
**Kategorik tahmin sonucu:** Hava çok soğuk, hava soğuk, hava ılık, hava sıcak, hava çok sıcak gibi.
<br>
**Nümerik tahmin sonucu:** Hava -10 derece, 0 derece, 10.01 derece, 30.02 derece gibi sayısal değerlerdir.
![image](https://user-images.githubusercontent.com/73706248/198107595-5a3de238-5f00-4880-94c4-1ddb50fa9bf1.png)

"Uygun olmayan regresyon yöntemlerinin kullanılması hatalı ve yanıltıcı sonuçların elde edilmesine neden olabilmektedir. Regresyon analizinde incelenen değişkenler sürekli ya da kesikli yapıda olabilmektedir ve bu veri yapısına bağlı olarak farklı regresyon modelleri kullanılabilmektedir (Özarıcı, 1996)."
<br> <br>
Denetimli öğrenmenin sınıflandırma ve regresyon olarak iki alt yönteme ayrıldığını yukarıdaki görsellerde ifade etmiştim. Aşağıdaki görselde de bu iki yöntemin grafiksel farklılıklarını görebilirsiniz:
![image](https://user-images.githubusercontent.com/73706248/198109730-7fcedbd7-f703-4afc-963b-73656fcf872d.png)

# Regresyon Çeşitleri Nelerdir? 
Regresyonun tahmin etmek istediğimiz duruma ve elimizdeki verilere göre değişebilen birçok yöntemi ve çeşidi vardır. Uygun olmayan regresyon yöntemlerinin kullanılması hatalı ve yanıltıcı sonuçların elde edilmesine neden olabilmektedir bu yüzden bu yöntemler arasından en doğru olanı seçmek önemli bir detaydır. Bunu şöyle düşünebiliriz: bizden bir probleme yönelik bir kod yazmamız isteniyor bunu 100 satırda da 50 satırda da yazabilir ve aynı sonuca ulaşabiliriz burada bu 50 satırlık farkı sağlayan şey algoritmamızdır. Regresyonda da en doğru tahmin için en doğru yöntemi seçmeye önem göstermeliyiz.
![image](https://user-images.githubusercontent.com/73706248/198112255-0cb572b0-9f9b-4bff-9596-836b5a30f6d0.png)

### Doğrusal Regresyon: 
Doğrusal regresyon, iki değişken arasındaki doğrusal ilişkinin bir doğru denklemi olarak tanımlanıp, değişkenin değerlerinden biri bilindiğinde diğeri hakkında tahmin yapılmasını sağlar.
<br>
Doğrusal regresyon, basit doğrusal regresyon ve çoklu doğrusal regresyon olarak iki başlık altında incelenir:
<br>
**Basit doğrusal regresyon,** yanıt değişkeni ile tek bir açıklayıcı değişken arasındaki doğrusal ilişkiyi açıklar. Eğer tek bir yanıt değişkeni ve birden fazla açıklayıcı değişken arasındaki doğrusal veya eğrisel bir ilişki tanımlanmak istenirse, **ilişki çoklu doğrusal regresyon** ile incelenir (Okur, 2009; Weisberg, 2005).
<br>
### Polinom Regresyon:
Bir bağımlı ve birden fazla bağımsız değişken arasında polinomyal bir artış söz konusu ise bu algoritmayı kullanırız. 
<br>
Polinom Regresyon Formülü: 
**Y = a + bX + cX²**
<br>
### Karar Ağacı Regresyonu:
Karar Ağaçları Algoritmaları hem sınıflandırma da hem de regresyonda kullanılır. Regresyon için kullanılan algoritmayı şöyle açıklayabiliriz; Bağımsız değişkenleri bilgi kazancına göre aralıklara ayırır. Tahmin esnasında bu aralıktan bir değer sorulduğunda cevap olarak bu aralıktaki (eğitim esnasında öğrendiği) ortalamayı verir. Belli aralıklarda istenilen değerler için aynı sonuçları ürettiğinden kesikli bir modeldir. # 
<br>
### Lojistik Regresyon: 
Lojistik regresyon, istatistikte kullanılan bir model oluşturma tekniği olup iki ya da daha fazla sınıfta ifade edilebilen kesikli verilerde yanıt değişkeni (Y) için bir model oluşturma tekniğidir.
<br>
Örneğin, web sitesi ziyaretçinizin alışveriş sepetindeki ödeme düğmesine tıklayıp tıklamayacağını tahmin etmek istediğinizi varsayalım. Lojistik regresyon analizi, web sitesinde harcanan zaman ve sepetteki ürün sayısı gibi geçmiş ziyaretçi davranışlarına bakar. Geçmişte, ziyaretçiler sitede beş dakikadan fazla zaman geçirdiyse ve sepete üçten fazla ürün eklediyse ödeme düğmesine tıkladıklarını belirler. Lojistik regresyon işlevi bu bilgiyi kullanarak daha sonra yeni bir web sitesi ziyaretçisinin davranışını tahmin edebilir.



















