
# Türkçe SMS Spam Mesaj Tespit Sistemi

Bu proje, Türkçe SMS mesajlarının spam olup olmadığını otomatik olarak tespit etmeyi amaçlayan bir makine öğrenmesi ve derin öğrenme uygulamasıdır.

## 📌 Proje Amacı

Mobil cihazlar hayatımızın ayrılmaz bir parçası haline gelirken, SMS ile gelen istenmeyen mesajlar (reklamlar, dolandırıcılıklar vb.) da artmıştır. Bu proje, Türkçe dilinin özgün yapısını dikkate alarak spam mesajları tespit eden etkili bir sistem geliştirmeyi hedefler.

## 🧾 Kullanılan Veri Seti

- **Toplam mesaj sayısı:** 4.751  
- **Spam mesajlar:** 2.536  
- **Normal mesajlar:** 2.215  
- **Veri bölünmesi:** %80 eğitim / %20 test  
- **Veri kaynağı:** Türkiye genelinden toplanmıştır

## 🔧 Veri Ön İşleme

- Küçük harfe çevirme  
- Noktalama işaretlerini ve sayıları kaldırma  
- Tokenizasyon (kelimeye ayırma)  
- Türkçe stop-word temizliği  
- TF-IDF ve word embedding dönüşümleri

## 🤖 Kullanılan Yöntemler

### 1. Klasik Makine Öğrenmesi Modelleri
- **Naive Bayes**
- **Lojistik Regresyon**
- **Destek Vektör Makineleri (SVM)**

🧮 En iyi sonuç: Lojistik Regresyon, %100 doğruluk (küçük veri seti nedeniyle iyimser olabilir)

### 2. Derin Öğrenme (LSTM)
- Gömülü katman ve LSTM katmanı ile sıralı model  
- Spam tespiti için sigmoid aktivasyon  
- 5 epoch eğitim  
- Karmaşık yapıları anlamada etkili

## 📊 Değerlendirme Metrikleri

- **Doğruluk (Accuracy)**
- **Kesinlik (Precision)**
- **Duyarlılık (Recall)**
- **F1 Skoru**

## 🔮 Gelecek Çalışmalar

- BERTurk gibi Türkçeye özgü önceden eğitilmiş modellerin kullanımı  
- Gerçek zamanlı filtrelerin mobil cihazlara entegrasyonu  
- Veri setinin güncellenmesi  
- E-posta ve sosyal medya gibi farklı platformlara uyarlanması  
- Kullanıcı geri bildirimiyle sürekli iyileştirme

## 👥 Katkıda Bulunanlar

- Serhat Şimşek – 030721031  
- Ömer Edebalı – 030721030  
- Mervan Şahin – 030720012  

## 🔗 Kaynaklar

1. Çiçekli, İ. & Kılıç, H. (2020). *Machine Learning Methods for Turkish SMS Spam Detection*.  
2. Devlin, J. et al. (2019). *BERT: Pre-training of Deep Bidirectional Transformers for Language Understanding*. NAACL.  
3. [Keras Belgeleri](https://keras.io/)
