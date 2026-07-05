# 🏔️ Image Classification — Intel Image Classification

> **Proyek Klasifikasi Gambar** menggunakan Convolutional Neural Network (CNN) untuk mengklasifikasikan gambar pemandangan alam dan perkotaan ke dalam 6 kategori.

---

## 📌 Deskripsi Proyek

Proyek ini merupakan submission untuk program **Belajar Machine Learning untuk Pemula (BMLP)**. Model dibangun menggunakan TensorFlow/Keras dengan arsitektur CNN untuk mengklasifikasikan gambar ke dalam 6 kelas pemandangan berbeda dari dataset **Intel Image Classification**.

Model yang telah dilatih diekspor dalam tiga format berbeda sehingga dapat di-*deploy* di berbagai platform: server, perangkat mobile, maupun browser.

---

## 🗂️ Dataset

| Properti       | Detail                                                                 |
|----------------|------------------------------------------------------------------------|
| **Nama**       | Intel Image Classification                                             |
| **Sumber**     | [Kaggle — puneet6060](https://www.kaggle.com/datasets/puneet6060/intel-image-classification) |
| **Jumlah Gambar** | ~25.000 gambar                                                      |
| **Jumlah Kelas** | 6 kelas                                                              |

### 🏷️ Kelas / Label

| No | Label       | Deskripsi                  |
|----|-------------|----------------------------|
| 0  | `buildings` | Bangunan / gedung          |
| 1  | `forest`    | Hutan                      |
| 2  | `glacier`   | Gletser / es               |
| 3  | `mountain`  | Pegunungan                 |
| 4  | `sea`       | Laut / pantai              |
| 5  | `street`    | Jalanan / perkotaan        |

---

## 📁 Struktur Direktori

```
ProyekKlasifikasiGambar/
├── 📓 Notebook_Submission_Klasifikasi_Gambar_Gevinta_Aprilia_(3) (1).ipynb
├── 📄 README.md
├── 📋 requirements.txt
│
├── 📂 saved_model/               # Format SavedModel (TensorFlow)
│   ├── saved_model.pb
│   ├── fingerprint.pb
│   ├── assets/
│   └── variables/
│
├── 📂 tfjs_model/                # Format TensorFlow.js (browser)
│   ├── model.json
│   ├── group1-shard1of6.bin
│   ├── group1-shard2of6.bin
│   ├── group1-shard3of6.bin
│   ├── group1-shard4of6.bin
│   ├── group1-shard5of6.bin
│   └── group1-shard6of6.bin
│
└── 📂 tflite/                    # Format TFLite (mobile/edge)
    ├── model.tflite
    └── label.txt
```

---

## 📊 Hasil Model

| Metrik            | Nilai     |
|-------------------|-----------|
| **Train Accuracy** | 90.52%   |
| **Test Accuracy**  | 89.40%   |

---

## 🚀 Format Model & Deployment

Model telah diekspor dalam **3 format** untuk mendukung berbagai skenario deployment:

| Format          | Direktori      | Kegunaan                                      |
|-----------------|----------------|-----------------------------------------------|
| **SavedModel**  | `saved_model/` | Deployment di server (TensorFlow Serving, dll) |
| **TFLite**      | `tflite/`      | Perangkat mobile & edge (Android, iOS, dll)    |
| **TensorFlow.js** | `tfjs_model/` | Aplikasi berbasis browser / web               |

---

## ⚙️ Instalasi & Menjalankan

### 1. Clone Repository

```bash
git clone <url-repository>
cd ProyekKlasifikasiGambar
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

**Daftar dependensi:**

```
tensorflow==2.19.0
numpy
matplotlib
seaborn
Pillow
scikit-learn
tensorflowjs==4.22.0
```

### 3. Jalankan Notebook

Buka notebook di **Google Colab** atau **Jupyter Notebook**, lalu jalankan semua cell secara berurutan:

```
Notebook_Submission_Klasifikasi_Gambar_Gevinta_Aprilia_(3) (1).ipynb
```

> **💡 Rekomendasi:** Gunakan Google Colab dengan GPU runtime untuk mempercepat proses training.

---

## 🧰 Teknologi yang Digunakan

- **Python 3.x**
- **TensorFlow 2.19.0** — framework utama deep learning
- **NumPy** — manipulasi array dan data numerik
- **Matplotlib & Seaborn** — visualisasi data dan kurva training
- **Pillow** — preprocessing dan augmentasi gambar
- **Scikit-learn** — evaluasi model (classification report, confusion matrix)
- **TensorFlow.js 4.22.0** — konversi model ke format web

---

## 👤 Penulis

**Gevinta Aprilia**
Submission — Belajar Machine Learning untuk Pemula (BMLP)

---

## 📜 Lisensi Dataset

Dataset Intel Image Classification tersedia secara publik di Kaggle di bawah lisensi [CC0: Public Domain](https://creativecommons.org/publicdomain/zero/1.0/).
