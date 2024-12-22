# Hayvan Sınıflandırma Projesi

Bu proje, belirli hayvan türlerini görüntü verileri kullanarak sınıflandırmayı amaçlamaktadır. 
Makine öğrenimi ve derin öğrenme yöntemlerini kullanarak hayvan resimlerini sınıflandıran bir Convolutional Neural Network (CNN) modeli oluşturulmuştur.

## Proje Özeti
- **Veri Seti**: 
  - Veri seti, `JPEGImages` adlı bir klasör içerisinde bulunan farklı hayvan türlerine ait görüntülerden oluşmaktadır.
  - Toplam 10 hayvan sınıfı seçildi: `collie`, `dolphin`, `elephant`, `fox`, `moose`, `rabbit`, `sheep`, `squirrel`, `giant panda`, `polar bear`.
  - Görüntüler 128x128 piksel boyutuna normalize edilmiştir.

- **Kullanılan Kütüphaneler**:
  - `TensorFlow`, `Keras`, `Scikit-learn`, `OpenCV`, `Matplotlib`, `Seaborn`, `Numpy`, `Pandas`, `Skimage`.

- **Model**:
  - CNN tabanlı model, 3 adet evrişim (Convolutional) ve havuzlama (Pooling) katmanına sahiptir.
  - Son katmanlarda 256 nöronlu bir Dense katman ve ardından Softmax aktivasyon fonksiyonu kullanılmıştır.

- **Başarı Oranı**:
  - Orijinal test verileri üzerinde doğruluk: **%75.59**.
  - Manipüle edilmiş test verileri üzerinde doğruluk: **%10.05**.
  - Renk dengesi uygulanmış veriler üzerinde doğruluk: **%11.79**.
