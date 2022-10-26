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









