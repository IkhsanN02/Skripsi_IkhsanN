# Ekstraksi Fitur Citra Retina Menggunakan ResNet50 dan Klasifikasi dengan Ensemble

Proyek ini bertujuan untuk membangun model yang memanfaatkan arsitektur **ResNet50** untuk ekstraksi fitur citra retina, kemudian mengklasifikasikan penyakit mata dengan teknik **Ensemble Learning**. Dataset yang digunakan mencakup beberapa kategori penyakit mata seperti *Normal*, *Cataract*, *Glaucoma*, dan *Diabetic Retinopathy*.

## Fitur Utama
- **Ekstraksi Fitur** menggunakan arsitektur ResNet50 yang telah dilatih pada dataset ImageNet.
- **Reduksi Dimensi** fitur dengan PCA (Principal Component Analysis).
- **Klasifikasi** menggunakan kombinasi model seperti Random Forest, SVM, dan XGBoost dengan teknik Ensemble Voting.
- **Evaluasi** performa model menggunakan metrik akurasi, laporan klasifikasi, confusion matrix, dan kurva ROC.

## Prasyarat
Proyek ini memerlukan beberapa pustaka Python. Anda dapat menginstalnya dengan perintah berikut:

```bash
pip install numpy pandas matplotlib seaborn tensorflow scikit-learn xgboost tqdm
```

## Dataset
Dataset yang digunakan adalah *Eye Diseases Classification* dari Kaggle. Dataset mencakup citra retina yang dikelompokkan berdasarkan kategori penyakit. Anda dapat mengunduh dataset melalui API Kaggle:

```bash
kaggle datasets download -d gunavenkatdoddi/eye-diseases-classification
```

## Cara Penggunaan
1. **Mengatur Dataset**:
   - Pastikan dataset diunggah ke direktori yang sesuai (`/content/dataset`).
   - Struktur direktori:
     ```
     /content/dataset
     ├── normal
     ├── cataract
     ├── glaucoma
     └── diabetic_retinopathy
     ```

2. **Menjalankan Kode**:
   - Eksekusi kode Python di Google Colab atau IDE lokal Anda.
   - Skrip akan memuat data, memproses citra, dan melatih model.

3. **Evaluasi Model**:
   - Hasil evaluasi termasuk metrik akurasi, confusion matrix, dan kurva ROC yang divisualisasikan.

## Struktur Skrip
1. **Setup dan Preprocessing**
   - Import pustaka.
   - Muat dan preprocess dataset.

2. **Ekstraksi Fitur**
   - Gunakan ResNet50 tanpa lapisan klasifikasi untuk mengekstrak fitur citra.

3. **Reduksi Dimensi**
   - Gunakan PCA untuk mengurangi dimensi fitur.

4. **Klasifikasi dengan Ensemble**
   - Latih model Random Forest, SVM, dan XGBoost.
   - Kombinasikan model dengan teknik *Soft Voting*.

5. **Evaluasi Model**
   - Evaluasi performa model dengan laporan klasifikasi, confusion matrix, dan ROC curve.

## Hasil
- **Akurasi Model Ensemble**: Akurasi model ensemble dicetak di konsol setelah evaluasi.
- **Visualisasi**:
  - Confusion Matrix.
  - ROC Curve untuk performa model.

## Teknologi yang Digunakan
- **ResNet50** untuk ekstraksi fitur citra.
- **PCA** untuk reduksi dimensi.
- **Ensemble Learning** untuk meningkatkan performa klasifikasi.

## Penulis
Ikhsan Nurazis  
Email: [ikhsannurazis22@gmail.com](mailto:ikhsannurazis22@gmail.com)  
LinkedIn: [Ikhsan Nurazis](https://www.linkedin.com/in/ikhsan-nurazis-a34a56219/)

## Lisensi
Proyek ini dilisensikan di bawah MIT License. Anda bebas menggunakan dan memodifikasi proyek ini untuk keperluan Anda.

---
Jika Anda memiliki pertanyaan atau masalah, silakan hubungi saya melalui email atau LinkedIn.
