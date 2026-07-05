
# Image Classification — Intel Image Classification

## Deskripsi
Proyek ini membangun model CNN untuk mengklasifikasikan gambar pemandangan
ke dalam 6 kategori: buildings, forest, glacier, mountain, sea, dan street.

## Dataset
- Nama: Intel Image Classification
- Sumber: https://www.kaggle.com/datasets/puneet6060/intel-image-classification
- Jumlah gambar: ~25.000
- Jumlah kelas: 6

## Struktur Direktori
submission/
├── tfjs_model/
├── tflite/
│   ├── model.tflite
│   └── label.txt
├── saved_model/
├── notebook.ipynb
├── README.md
└── requirements.txt

## Hasil Model
- Train Accuracy : 90.52%
- Test Accuracy  : 89.40%

## Format Model
- SavedModel : untuk deployment server
- TF-Lite    : untuk perangkat mobile
- TFJS       : untuk aplikasi berbasis browser

## Cara Menjalankan
Buka notebook.ipynb di Google Colab dan jalankan semua cell secara berurutan.
