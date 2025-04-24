# Klasifikasi Gambar Hewan

Proyek ini bertujuan untuk membangun model klasifikasi gambar menggunakan **Transfer Learning dengan model MobilenetV2** untuk mengklasifikasikan berbagai jenis gambar hewan. Proyek ini menggunakan **TensorFlow** dan **Keras**.

## Fitur Utama

- Klasifikasi gambar hewan ke dalam kategori yang sudah ditentukan (kucing, anjing, gajah, kuda, singa).
- Implementasi model CNN dengan **transfer learning** menggunakan model **MobileNetV2** yang sudah dilatih sebelumnya.
- Evaluasi model menggunakan metrik **akurasi**

## Persyaratan

Sebelum memulai, pastikan kamu telah menginstal semua dependensi berikut:

```bash
pip install -r requirements.txt
```

## Langkah-Langkah Menjalankan Proyek

### 1. Persiapkan Dataset

dataset dapat diunduh langsung di kaggle, atau menggunakan kagglehub
https://www.kaggle.com/datasets/antobenedetti/animals

### 2. Pelatihan model

model dilatih menggunakan transfer learning dari model pretrained MobilenetV2 

### 3. Evaluasi Model

model di evaluasi dengan matrik accuracy dengan hasil sebagai berikut:
- Train Accuracy : 0.9639381766319275
- Test Accuracy  : 0.9559118151664734
- Val Accuracy   : 0.9558823704719543

### 4. Prediksi Gambar Baru

Untuk inference, kamu perlu menghost model yang di saved ke tf serving terlebih dahulu, kode inference bisa di akses di inference.ipynb


### 5. Menyimpan dan Memuat Model

Model yang telah dilatih disimpan dalam format saved_model di folder `animal_classifier_model/`. Kamu dapat memuat model tersebut kapan saja untuk melakukan prediksi atau melanjutkan pelatihan.


## Penutup
Proyek ini adalah contoh implementasi **Klasifikasi Gambar Hewan** menggunakan **Tranfer Learning dengan Model MobilenetV2**. Kamu bisa meningkatkan akurasi model dengan menggunakan dataset yang lebih besar atau teknik lain seperti **data augmentation**.
