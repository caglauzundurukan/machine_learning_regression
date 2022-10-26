## Denetimli öğrenme algoritmaları: Regresyon (Basit Doğrusal regresyon ve çoklu regresyon) nedir, çalışma mantığı nedir, kullanım alanları, örnekleri.
![Beige Nude Business Organization Chart](https://user-images.githubusercontent.com/73706248/198099903-bdebf4c3-694a-44d8-b18a-b631f0b36351.png)
**Denetimli öğrenme**; aldığı veriler ve ürettiği sonuçlara dayalı olarak bir model geliştirme işlemidir. Diğer makine öğrenmesi türlerine kıyasla denetimli öğrenmenin en büyük farkı veri etiketi kullanılmasıdır. Etiketlediğimiz veriye, gösterdiğimiz sınıf ve bilgiye göre mevcut gerçekliğe dayanarak model geliştirme algoritmasıdır.

# Regresyon Nedir?
**Regresyon**, bir bağımlı değişken (genellikle Y ile gösterilir) ve diğer bağımsız değişkenler arasındaki ilişkinin gücünü ve karakterini belirlemeye çalışan finans, yatırım, makine öğrenmesi ve diğer disiplinlerde kullanılan istatistiksel bir yöntemdir.

**Bağımlı Değişken:** Anlamaya veya tahmin etmeye çalıştığımız değişkendir.  <br>
**Bağımsız Değişken:** Analizi veya hedef değişkeni etkileyen ve değişkenlerin hedef değişkenle ilişkisi hakkında bize bilgi veren faktörlerdir.

# Makine Öğrenmesinde Regresyon
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
### Basit Doğrusal Regresyon:
Basit doğrusal regresyon; bağımsız değişken (X)ile bağımlı değişken (Y)deki değişimi açıklamayı, bağımsız değişkendeki bir birimlik değişimin bağımlı değişken üzerindeki etkisini ölçmeyi amaçlar.
<br>
Temel amaç, bağımlı ve bağımsız değişken arasındaki ilişkiyi ifade eden doğrusal fonksiyonu bulmaktır.
<br>
![image](https://user-images.githubusercontent.com/73706248/198124537-f69d719d-1455-45d3-af04-4dcdab8219d5.png)
<br> <br>
**Basit doğrusal regresyon kullanımına birkaç örnek:**
<br>
Tarım bilimcileri, gübre ve suyun mahsul verimi üzerindeki etkisini ölçmek için genellikle doğrusal regresyon kullanırlar. bilim adamları farklı alanlarda farklı miktarlarda gübre ve su kullanabilir ve bunun mahsul verimini nasıl etkilediğini görebilirler. 
 <br> <br>
Araştırmacılar hastalara belirli bir ilacın çeşitli dozajlarını uygulayabilir ve kan basıncının nasıl tepki verdiğini gözlemleyebilir. Yordayıcı değişken olarak dozajı ve yanıt değişkeni olarak kan basıncını kullanan basit bir doğrusal regresyon modeline uyabilirler.
 

### Çoklu Doğrusal Regresyon: 
Doğrusal basit regresyonun bağımsız değişken sayısı birden fazla olan versiyonudur. Yani çoklu regreson denkleminde yanıt değişkenimiz olan bağımlı değişkeni etkileyen birden fazla bağımsız değişken vardır.
Kullanımı ve mantığı basit doğrusal regresyon ile benzerdir. Sadece birden fazla değişken vardır.
<br>
Çoklu doğrusal regresyon denklemi aşağıdaki gibidir:
<br> 
![image](https://user-images.githubusercontent.com/73706248/198126326-b82fabb8-7d31-4e6f-9e8c-e0d7a83932f2.png)
<br>
**Çoklu doğrusal regresyon kullanımına birkaç örnek:**
<br> 
Bulaşıcı bir hastalığın yayılmasını inceleyen bir epidemiyologsunuz. Mevcut bilinen enfeksiyonlara dayanarak bu hastalığın gelecekteki yayılmasını tahmin etmek istiyorsunuz. Çok sayıda bağımsız değişken, popülasyon büyüklüğü, popülasyon yoğunluğu, hava sıcaklığı, asemptomatik taşıyıcılar ve popülasyonun sürü bağışıklığına ulaşıp ulaşmadığı dahil olmak üzere gelecekteki enfeksiyonların sayısını etkileyebilir. Yordayıcı değişkenlerin katsayı değerlerindeki olası değişiklikleri hesaba katan bir sonucu tahmin etmek için ampirik veriler üzerinde istatistiksel modelleme ve çoklu doğrusal regresyon analizi yapabilirsiniz.br
<br> <br>
Ev satmak için en iyi zamanı tahmin etmeye yardımcı olacak bir model oluşturmak isteyen bir emlak uzmanısınız. Evleri maksimum satış fiyatından satmak istersiniz, ancak satış fiyatını birden fazla faktör etkileyebilir. Bu değişkenler, diğer faktörlerin yanı sıra evin yaşını, mahalledeki diğer evlerin değerini, devlet okulu sisteminin öğrenci performansına ilişkin nicel ölçümlerini ve yakındaki parkların sayısını içerir.Evlerin maksimum satış fiyatını tahmin etmek için bu dört bağımsız değişkenden bir tahmin modeli oluşturabilirsiniz. Bu faktörlerden herhangi biri katsayı değerleri açısından değişirse değişkenleri ayarlayabilirsiniz.



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
<br>
Ridge Regresyon, Lasso Regresyon, Sıralı Regresyon gibi daha birçok regresyon türü de bulunmaktadır.
# Regresyon Modeli Kurulumunda Beş Metod
Lineer modelde iki farklı değişkenimiz vardı: ilki bağımlı değişken (hedef değişken – y) diğeri ise bağımsız değişken(ler)(predictors – x). Gerçek hayatta bir hedef değişkene etki eden birçok belirleyici değişken vardır. Örnek olarak şirket karı hedef değişken olsun. Karı etkileyen birçok faktör vardır. Peki biz kardaki değişkenliği açıklamak için bu faktörlerden hangilerini modelimize dahil edeceğiz? Hepsini mi? Kabaca seçtiğimiz 3-5 tanesini mi? En iyi sonucu vereni mi? En iyi sonucu hangisi verir? Bunu nasıl ölçeriz?
<br> <br>
Her bağımsız değişkeni modele dahil edersek model arap saçına dönebilir ve modelin anlaşılırlığı azalabilir. Peki bu karmaşaya nasıl bir çözüm bulunabilir? Yaygın olarak kullanılan beş yöntem ile bağımsız değişkenleri eleyerek sağlıklı modeller oluşturabiliyoruz:
![image](https://user-images.githubusercontent.com/73706248/198132912-62ae2361-f0bd-47c5-9933-e0bcd966bc92.png)
### Bağımsız değişkenlerin hepsini birden modele dahil etmek (All-in):
lk yöntem olan hepsini birden modele dahil et yöntemini kuramlara dayalı geliştirilen modellerde kullanırız. Daha önce benzer alanda bir çok ampirik çalışma yapılmıştır ve bazı kavramlar arasındaki ilişkiler defalarca farklı örneklem üzerinde kanıtlanmıştır. Yani modele dahil edilen bağımsız değişkenlerin bağımlı değişkene etki ettiğine dair yeterince kanıt vardır. 
### Geriye doğru eleme (Backward Elimination):
-Anlamlılık düzeyi belirlenir. Mesela; p < 0.05.

-Bir önceki yöntemde olduğu gibi tüm değişkenler modele dahil edilir.

-Her bir bağımsız değişkenin anlamlılık düzeyi incelenir. Eğer anlamlılık düzeyi model için belirlenenden daha büyük ise bu bağımsız değişken modelden çıkarılır. Eğer birden fazla var ise bu işlem en büyük p değerine sahip olana uygulanır. Şayet bütün p değerleri sınır değerden küçük ise model tamam demektir.

-Çıkarılan her bir değişkenden sonra model tekrar kurulur (eğitilir) ve üçüncü adım tekrar edilir.

-Tüm bağımsız değişkenlerin p değeri eşik altında kalana kadar, başka bir deyişle bağımsız değişken ile ilişkisi istatistiksel anlamlı olana kadar üç ve dört tekrar edilir.
### İleriye doğru seçme (Forward Selection):
-Anlamlılık düzeyi belirlenir.

-Bağımlı değişken (y) ile tüm bağımsız değişkenler (X) tek tek basit regresyona sokulur. Aralarından en düşük p değerine sahip olan seçilir.

-Bu en düşük değerli bağımsız değişken ile diğer bağımsız değişkenlerden oluşturulan modeller ayrı ayrı ikili olarak çoklu regresyona sokulur. En düşük p değerine sahip olan ikili seçilir.

-En düşük p değerli ikili ile kalan bağımsız değişkenlerden üçlü kombinasyonlar oluşturulur ve modeller tek tek regresyona sokulur. p değeri anlamsız çıkana kadar üçüncü ve dördüncü adımlar tekrarlanır.
### İki yönlü eleyerek seçme (Bidirectional Elimination):
-Anlamlılık düzeyi belirlenir.

-İleri doğru seçme yönteminde olduğu gibi anlamlılık düzeyi altında kaldığı sürece modele yeni değişkenler ilave edilir.

-Geriye doğru eleme yönteminin tüm adımları uygulanır.

-Yeni bir değişken ekleyemeyene ve eski değişkenlerden birini çıkaramayana kadar adım 2 ve 3 tekrarlanır.
### Sonuçları karşılaştırma (Score comparision)
-Uyum indeksi için kriter belirlenir.

-Olası tüm modeller denenir.

-En iyi uyum indeksine sahip olan seçilir.

NOT: Bu yöntemler arasında en çok tercih edilen iki yöntem **Geriye Doğru Eleme** ve **İleriye Doğru Seçme**'dir.









## KAYNAKÇA
https://dergipark.org.tr/en/download/article-file/187511 <br>
https://aws.amazon.com/tr/what-is/logistic-regression/  <br>
https://www.ibm.com/tr-tr/analytics/learn/linear-regression   <br>
https://www.scribbr.com/statistics/simple-linear-regression/#:~:text=What%20is%20simple%20linear%20regressio%20n,Both%20variables%20should%20be%20quantitative.




















