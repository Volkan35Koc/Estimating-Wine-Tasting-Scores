# Estimating-Wine-Tasting-Scores

Bu proje, şarapların çeşitli özelliklerine dayanarak tadım puanlarını ('points') tahmin etmeyi amaçlayan bir makine öğrenmesi uygulamasıdır.
Projede farklı algoritmalar karşılaştırılarak en iyi tahmin performansını sağlayan model belirlenmiştir.


##  Proje Amacı

Şarap tadım puanları, şarap kalitesinin belirlenmesinde önemli bir rol oynamaktadır.
Bu projede amaç; şarabın fiyatı, menşei, üzüm türü gibi bilgileri kullanarak tadım puanlarını doğru bir şekilde tahmin etmektir.

## Veri Seti

- Kaynak: 150.000 şarap incelemesinden oluşan veri seti.
- Bu çalışmada ilk 1.000 kayıt kullanılmıştır.
- Eksik veriler temizlenmiştir.
- Kategorik değişkenler one-hot encoding yöntemi ile dönüştürülmüştür.


## Problem Tanımı

- **Hedef Değişken:** `points` (şarap tadım puanı)
- **Bağımsız Değişkenler:** fiyat, bölge, üzüm türü gibi kategorik ve sayısal değişkenler.
- **Problem Türü:** Regresyon


## Kullanılan Algoritmalar

1. **Random Forest Regressor**  
2. **Linear Regression**  
3. **Decision Tree Regressor**  
4. **K-Nearest Neighbors Regressor**


## Performans Metrikleri

| Model                   | MAE   | MSE   | RMSE  | R²    |
|------------------------|-------|-------|-------|-------|
| Random Forest           | 1.223 | 2.664 | 1.632 | 0.523 |
| Linear Regression       | 1.593 | 3.603 | 1.898 | 0.355 |
| Decision Tree           | 1.045 | 3.075 | 1.753 | 0.450 |
| K-Nearest Neighbors     | 1.854 | 4.605 | 2.146 | 0.176 |

 **En iyi performansı Random Forest göstermiştir.**


## Görselleştirmeler

- **Parity Plot:** Gerçek ve tahmin edilen puanlar karşılaştırılmıştır.
- **Residual Plot:** Hataların tahmin değerlerine göre dağılımı incelenmiştir.
- **Density Plot:** Hata dağılımı analiz edilmiştir.


## Çapraz Doğrulama Sonuçları

| Metrik    | Ortalama Skor | Standart Sapma |
|-----------|----------------|----------------|
| MAE       | 1.031          | 0.121          |
| MSE       | 1.977          | 0.508          |
| R²        | 0.642          | 0.028          |


## Kullanılan Teknolojiler

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn


## İbrahim Volkan KOÇ

**Veri Bilimci**  
linkedin.com/in/ibrahimvolkankoc35
