# Telekomünikasyon Müşteri Kaybı (Churn) Tahmini

**📌 Proje Geçmişi ve Sürüm Notu:**
Bu proje, eğitim sürecindeki "Medium Makalesi" görevi için geliştirdiğim temel (baseline) Churn Tahmini projesinin, Final Ödevi yönergelerine uygun olarak genişletilmiş ve optimize edilmiş nihai versiyonudur. Önceki versiyonun üzerine; yeni öznitelikler üretilmesi, Validation setinin ayrılması, 3 farklı makine öğrenmesi algoritmasının karşılaştırılması ve çoklu doğrusallık analizleri eklenmiş ve proje uçtan uca tam kapsamlı bir akışa kavuşturulmuştur.

## Projenin Amacı
Telekomünikasyon müşterilerinin demografik, hizmet ve hesap bilgilerini kullanarak şirketi terk edip etmeyeceklerini (Churn) tahmin etmek. 

## Veri Seti
Projede "Telco Customer Churn" veri seti kullanılmıştır. Veri seti, müşterilerin aldığı hizmetleri, hesap bilgilerini ve demografik verilerini içeren toplam 21 sütundan oluşmaktadır.

## Nasıl Çalıştırılır?
1. Bu repository'yi bilgisayarınıza klonlayın.
2. `pip install -r requirements.txt` komutu ile gerekli kütüphaneleri kurun.
3. Jupyter Notebook veya uygun bir Python IDE'si ile projeyi çalıştırın.

## Kısa Sonuç Yorumu
Lojistik Regresyon, Random Forest ve KNN algoritmaları arasından iş problemi için en iyi açıklanabilirliği ve dengeyi sunan Lojistik Regresyon seçilmiştir. Hiperparametre optimizasyonu (GridSearchCV) ile modelin Recall (Duyarlılık) skoru artırılmış ve riskli müşterileri tespit etme kapasitesi maksimize edilmiştir. Fiber optik kullanıcıları ve manuel ödeme (Electronic Check) yapan müşterilerde kayıp oranının belirgin şekilde yüksek olduğu tespit edilmiştir.
