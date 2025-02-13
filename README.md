# 🔊 Ses Sınıflandırma: Derin Öğrenme ile Kedi & Köpek Ses Tanıma

Bu proje, **derin öğrenme ve doğal dil işleme (NLP)** teknikleri kullanılarak **kedi ve köpek seslerinin sınıflandırılmasını** amaçlamaktadır.  
**CNN (Evrişimsel Sinir Ağları)** ve **LSTM (Uzun Kısa Süreli Bellek)** modelleri ile ses işleme teknikleri kullanılarak veri analizi ve model eğitimi gerçekleştirilmiştir.

---

## 🚀 Proje Hakkında
- **Veri Seti:** Kaggle **"Audio Cats and Dogs"** veri seti kullanılmıştır.
- **Modelleme:** **CNN ve LSTM** tabanlı sinir ağları uygulanmıştır.
- **Özellik Çıkarımı:** **MFCC (Mel-Frequency Cepstral Coefficients)** kullanılmıştır.
- **Değerlendirme:** **K-katlı Çapraz Doğrulama (K=5)** ile test edilmiştir.

---

## 📂 İçindekiler
- [Kurulum](#kurulum)
- [Veri Seti](#veri-seti)
- [Kullanılan Yöntemler](#kullanılan-yöntemler)
- [Model Eğitimi ve Sonuçlar](#model-eğitimi-ve-sonuçlar)
- [Kaynaklar](#kaynaklar)

---

## 📌 Kurulum

### Gerekli Bağımlılıkları Yükleyin
Proje için gerekli kütüphaneleri yüklemek için aşağıdaki komutu çalıştırabilirsiniz:

```bash
pip install numpy pandas librosa tensorflow keras scikit-learn

# Modeli Eğitmek İçin Çalıştırın
python train.py

# Test Verisi ile Modeli Çalıştırın
python predict.py --audio sample.wav
```

---

## 🎵 VeriSeti

- Veri Seti **Kaggle**'dan alınmıştır: [Audio Cats and Dogs Dataset](https://www.kaggle.com/datasets/mmoreaux/audio-cats-and-dogs/data). 
- Veri setinde 164 kedi sesi ve 113 köpek sesi bulunmaktadır.
- wav formatında değişken uzunlukta ses dosyalarından oluşmaktadır.

## 🧠 Kullanılan Yöntemler

📊 Ses İşleme
- Librosa ve python_speech_features kullanılarak ses verileri işlendi.
- MFCC, STFT ve Log-Mel Filterbank kullanılarak özellik çıkarımı yapıldı.

![image](https://github.com/user-attachments/assets/acf62121-7500-4f0a-bde7-903cd6d3559d)

![image](https://github.com/user-attachments/assets/1cdd7195-55ed-42e7-8dde-dedbb9e03da5)

![image](https://github.com/user-attachments/assets/219e8ea4-1d36-491e-9a49-f16b02c28409)

![image](https://github.com/user-attachments/assets/04ff88a4-4bff-4bf9-ab01-97f23dddda0b)


🔍 Derin Öğrenme Modelleri
- CNN (Evrişimsel Sinir Ağı): Ses verisini spektrograma dönüştürerek analiz eder.
- LSTM (Uzun Kısa Süreli Bellek): Zamansal bağımlılıkları öğrenmek için kullanılır.


📈 Model Değerlendirme
- CNN modeli ve LSTM modeli K=5 ile çapraz doğrulama ile accuracy ve loss metrikleri ile değerlendirilmiştir.
  

## 📊 Model Eğitimi ve Sonuçlar
CNN ve LSTM modelleri test edilerek karşılaştırılmıştır.
LSTM modeli, K-katlı Çapraz Doğrulama yöntemi ile en iyi sonucu vermiştir.

![image](https://github.com/user-attachments/assets/0c9da81e-a8bb-4369-9bbf-7cef60ce62c8)

## 📜 Kaynaklar
[Kaggle - Audio Cats and Dogs Dataset](https://www.kaggle.com/datasets/mmoreaux/audio-cats-and-dogs/data)

[Derin Öğrenme Makalesi](https://dergipark.org.tr/tr/download/article-file/2489965)

[Proje Tanıtım Videosu](https://dergipark.org.tr/tr/download/article-file/2489965)



