### Proje README.md Metni

```markdown
# Akbank Derin Öğrenme Bootcamp: Görüntü Sınıflandırma Projesi

Bu proje, Akbank Derin Öğrenme Bootcamp kapsamında, CNN (Convolutional Neural Network) mimarisi kullanılarak bir görüntü sınıflandırma modeli geliştirmeyi amaçlamaktadır. Proje, veri ön işlemeden model optimizasyonuna ve yorumlanmasına kadar tüm aşamaları kapsamlı bir şekilde ele almaktadır.

---

###  Projenin Amacı
Amacımız, **Intel Görüntü Sınıflandırma** veri setindeki görüntülerden yola çıkarak, binalar, orman, deniz gibi 6 farklı sınıfı yüksek doğrulukla ayırt edebilen sağlam bir derin öğrenme modeli oluşturmaktır.

---

###  Veri Seti Hakkında
Proje, Kaggle üzerinden erişilen `Intel Image Classification` veri setini kullanmaktadır. Bu veri seti; `buildings`, `forest`, `glacier`, `mountain`, `sea` ve `street` olmak üzere 6 farklı sınıfa ait yaklaşık 25.000 görüntü içermektedir. Veri, modelin doğru bir şekilde değerlendirilmesi için eğitim, validasyon ve test kümelerine ayrılmıştır.

---

###  Kullanılan Yöntemler
Projenin her aşamasında en güncel ve etkili derin öğrenme teknikleri kullanılmıştır.

* **Veri Çoğaltma (Data Augmentation):** Modelin aşırı uyumunu (overfitting) engellemek ve genelleme yeteneğini artırmak amacıyla, mevcut veri seti döndürme, yatay çevirme ve yakınlaştırma gibi dönüşümlerle zenginleştirilmiştir.
* **Özel CNN Mimarisi:** Görüntüden özellik çıkarmak için **Evrişimsel (Convolutional)** ve **Havuzlama (Pooling)** katmanları içeren özel bir model mimarisi tasarlanmıştır. Modelin performansını artırmak için **Dropout** gibi düzenlileştirme (regularization) teknikleri de uygulanmıştır.
* **Hiperparametre Optimizasyonu (Keras Tuner):** En iyi model mimarisini ve en uygun hiperparametreleri (filtre sayısı, öğrenme oranı, dropout oranı vb.) bulmak için **Keras Tuner** kütüphanesi ile otomatik arama yapılmıştır. Bu yaklaşım, manuel denemelerin ötesine geçerek en yüksek performanslı modelin elde edilmesini sağlamıştır.
* **Model Yorumlama (Grad-CAM):** Modelin tahminlerini yaparken görüntülerin hangi bölgelerine odaklandığını anlamak için **Grad-CAM (Gradient-weighted Class Activation Mapping)** tekniği kullanılmıştır. Bu görselleştirmeler, modelin kararlarının mantıklı ve ilgili görsel özelliklere dayandığını kanıtlamaktadır.

---

###  Elde Edilen Sonuçlar
Optimizasyon ve model eğitimi sonucunda, modelimiz test verisi üzerinde **%82** gibi yüksek bir genel doğruluk oranına ulaşmıştır. Model, özellikle `forest` ve `buildings` gibi sınıflarda çok yüksek başarı gösterirken, `glacier` ve `mountain` gibi birbirine benzer sınıfları ayırt etmekte biraz daha zorlanmıştır. Sınıflandırma Raporu ve Karışıklık Matrisi, bu sonuçları detaylı olarak doğrulamaktadır.

---

###  Kaggle Notebook Linki
Projenin tüm kodlarına, detaylı teknik anlatımlarına, adımlarına ve sonuçlarına aşağıdaki Kaggle Notebook linkinden erişebilirsiniz.

[**Akbank Bootcamp CNN Projesi (Kaggle Notebook)**](https://www.kaggle.com/code/elifnalkac/akbank-bootcamp-cnn-projesi)
```
