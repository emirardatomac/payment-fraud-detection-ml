# Online Payment Fraud Detection with ML Models

## Proje Açıklaması

Bu proje, çevrimiçi ödeme dolandırıcılığını tespit etmek amacıyla çeşitli makine öğrenme modellerini kullanarak sınıflandırma işlemi gerçekleştirmektedir. Proje kapsamında hem gözetimli (supervised) hem de gözetimsiz (unsupervised) öğrenme algoritmaları değerlendirilmiştir. Veri seti, bu algoritmaların performanslarını karşılaştırmak ve en uygun olanı belirlemek için kullanılmıştır.

## Veri Seti

Proje, Kaggle'dan sağlanan bir çevrimiçi ödeme dolandırıcılığı veri setini kullanmaktadır. Bu veri seti, işlemlerin dolandırıcılık olup olmadığını belirlemek için kullanılan çeşitli özellikleri içerir.

## Kullanılan Algoritmalar

### Gözetimli Öğrenme Modelleri

1. **Lojistik Regresyon (Logistic Regression)**
   - **Doğruluk Skoru:** %99.33
   - **Performans:** Negatif sınıf (Sınıf 0) için yüksek doğruluk ve mükemmel sonuçlar; pozitif sınıf (Sınıf 1) için düşük performans.
   - **Genel Yorum:** Negatif sınıfın neredeyse mükemmel bir şekilde sınıflandırılması sağlanmıştır. Pozitif sınıfın ise veri setindeki dengesizlik nedeniyle daha düşük performans göstermiştir.

2. **Random Forest**
   - **Doğruluk Skoru:** Projeye dahil edilen sonuçlar üzerinden hesaplanmıştır.
   - **Performans:** Genellikle yüksek doğruluk oranları ve iyi performans göstermiştir. Detaylı sonuçlar projede yer almaktadır.

### Gözetimsiz Öğrenme Modelleri

1. **K-Means Kümeleme**
   - **Karışıklık Matrisi:** Negatif sınıfta yüksek yanlış pozitif oranı ve pozitif sınıfta nispeten iyi performans.
   - **Genel Yorum:** Negatif sınıfta büyük bir hata payı ile karşılaşılmıştır. Pozitif sınıfta ise daha dengeli sonuçlar elde edilmiştir.

2. **DBSCAN**
   - **Performans:** Gözetimsiz öğrenme algoritması olarak kullanılmış, performansı genellikle düşük olmuştur. Detaylı sonuçlar projede yer almaktadır.

## Sonuçların Karşılaştırılması

Gözetimli öğrenme algoritmalarının (Lojistik Regresyon ve Random Forest) performansı, gözetimsiz öğrenme algoritmalarına (K-Means ve DBSCAN) kıyasla genellikle daha iyi sonuçlar vermiştir. Özellikle, veri setindeki sınıf dengesizliği nedeniyle gözetimsiz öğrenme yöntemleri daha düşük performans göstermiştir. Lojistik Regresyon ve Random Forest, dolandırıcılığı tespit etmede daha etkili sonuçlar sağlamıştır.

## Kaggle Not Defteri

Projenin tamamını ve detaylarını içeren Kaggle not defteri için [bu bağlantıya](https://www.kaggle.com/code/emirardatomac/online-payment-fraud-detection-with-ml-models) göz atabilirsiniz.

## Kullanılan Kütüphaneler

- scikit-learn
- pandas
- numpy
- matplotlib
- seaborn

