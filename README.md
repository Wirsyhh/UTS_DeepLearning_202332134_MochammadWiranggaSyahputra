# UTS Deep Learning - Klasifikasi Digit MNIST

## Mahasiswa
- **Nama**: Mochammad Wirangga Syahputra
- **NIM**: 202332134
- **Kelas**: A
- **Mata Kuliah**: Deep Learning

## Deskripsi Proyek
Implementasi dan perbandingan dua pendekatan klasifikasi digit tulisan tangan:
1. **Model A**: Convolutional Neural Network (CNN) dari nol
2. **Model B**: Transfer Learning menggunakan MobileNetV2

## Hasil Akhir

### Model A (CNN dari Nol)
- Test Accuracy (MNIST): **99.31%**
- Accuracy Tulisan Tangan: **96.67%** (29/30 benar)

### Model B (Transfer Learning)
- Test Accuracy (MNIST): **60.00%**
- Accuracy Tulisan Tangan: **60.00%** (18/30 benar)

## Struktur Folder
```
├── README.md
├── UTS_DeepLearning.ipynb          # Notebook utama
├── hasil_evaluasi.txt               # Ringkasan hasil
├── models/
│   ├── model_a_cnn.h5
│   └── model_b_transfer_learning.h5
├── handwritten/                     # 30 gambar tulisan tangan
│   ├── digit01_01.jpg
│   ├── digit02_01.jpg
│   └── digit03_01.jpg
└── results/                         # Hasil visualisasi
    ├── mnist_original_samples.png
    ├── ...
    └── detailed_comparison_bar_chart.png
```

## Requirements
```python
tensorflow>=2.10.0
numpy>=1.21.0
matplotlib>=3.4.0
opencv-python>=4.5.0
scikit-learn>=0.24.0
seaborn>=0.11.0
Pillow>=8.0.0
```


### 1. Clone Repository
```bash
git clone https://github.com/Wirsyhh/UTS-DeepLearning-202332134.git
cd UTS-DeepLearning-202332134
```

### 2. Install Dependencies
```bash
pip install -r requirements.txt
```

### 3. Jalankan Notebook
```bash
jupyter notebook UTS_DeepLearning.ipynb
```

Atau buka di Google Colab: https://colab.research.google.com/drive/1aIwGr14mYxGPAb5LfnLG_NELxX1MRPgR?authuser=0#scrollTo=1DlCr9FQD4fZ

## Kesimpulan
Model CNN sederhana yang dirancang khusus untuk MNIST (Model A) mengungguli 
Transfer Learning (Model B) secara signifikan. Hal ini menunjukkan bahwa 
transfer learning tidak selalu optimal untuk setiap kasus, terutama ketika 
domain gap antara dataset pre-trained dan dataset target terlalu besar.

## Referensi
- [MNIST Database](http://yann.lecun.com/exdb/mnist/)
- [Keras Documentation](https://keras.io/)
- [TensorFlow Transfer Learning Guide](https://www.tensorflow.org/tutorials/images/transfer_learning)
```

```
tensorflow==2.13.0
numpy==1.24.3
matplotlib==3.7.2
opencv-python==4.8.0.76
scikit-learn==1.3.0
seaborn==0.12.2
Pillow==10.0.0
pandas==2.0.3
