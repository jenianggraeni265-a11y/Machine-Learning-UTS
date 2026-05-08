## Machine-Learning-UTS
# Prediksi Kualitas Wine Menggunakan Machine Learning

Project ini merupakan tugas UTS mata kuliah Machine Learning yang bertujuan untuk memprediksi kualitas wine berdasarkan karakteristik fisikokimia menggunakan beberapa algoritma klasifikasi machine learning.

Dataset yang digunakan berisi informasi seperti:

fixed acidity

volatile acidity

citric acid

residual sugar

chlorides

alcohol

pH

sulphates

dan variabel kimia lainnya

Target yang diprediksi adalah:

quality (kualitas wine)


## Tujuan Analisis

Tujuan dari project ini adalah:
1. Melakukan eksplorasi data (EDA)
2. Melakukan preprocessing data
3. Membangun model machine learning klasifikasi
4. Membandingkan performa beberapa algoritma
5. Menentukan model terbaik
6. Membuat prediksi pada data testing
7. Menghasilkan file submission CSV


## Struktur Project

├── UTS_MACHINE_LEARNING.ipynb

├── data_training.csv

├── data_testing.csv

├── hasilprediksi_021.csv

└── README.md


## Exploratory Data Analysis (EDA)

Tahapan EDA yang dilakukan:
1. Informasi dataset
2. Statistik deskriptif
3. Pengecekan missing values
4. Pengecekan duplicate data
5. Distribusi target
6. Heatmap korelasi

### Hasil EDA

Beberapa insight yang diperoleh:
1. Dataset tidak memiliki missing values
2. Tidak terdapat data duplikat
3. Kualitas wine didominasi kelas 5 dan 6
4. Variabel alcohol memiliki korelasi positif terhadap kualitas wine
5. Variabel volatile acidity memiliki korelasi negatif terhadap kualitas wine

## Data Preprocessing

Tahapan preprocessing yang dilakukan:

1. Memisahkan fitur dan target
2. Menghapus kolom Id
3. Train-test split
4. Feature scaling menggunakan StandardScaler

Train-Test Split

Dataset dibagi menjadi: 80% training dan 20% validation

Feature Scaling

Scaling hanya dilakukan pada data training untuk menghindari data leakage.

## Algoritma Machine Learning

Model yang digunakan:

Logistic Regression

Decision Tree

Random Forest

Support Vector Machine (SVM)

K-Nearest Neighbor (KNN)

## Evaluasi Model

Evaluasi dilakukan menggunakan:

Accuracy

Classification Report

Confusion Matrix

Hasil Accuracy

### Model	Accuracy
Random Forest	0.616

Logistic Regression	0.610

Decision Tree	0.599

SVM	0.593

KNN	0.483

## Model Terbaik

Model terbaik pada analisis ini adalah: Random Forest Classifier

Alasan:
a. Memiliki accuracy tertinggi
b. Lebih stabil dibanding decision tree tunggal
c. Mampu menangani hubungan non-linear antar fitur
d. Mengurangi risiko overfitting

## Confusion Matrix

Confusion matrix digunakan untuk melihat detail hasil prediksi model.

Hasil menunjukkan bahwa:
1. Sebagian besar prediksi berada pada kelas yang benar
2. Kesalahan prediksi banyak terjadi pada kelas kualitas yang berdekatan seperti 5 dan 6

## Output Project

Output akhir project berupa file: hasilprediksi_021.csv

Format file:
Id, quality

## Tools dan Library
Python, Google Colab, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn

## Konsep Machine Learning yang Digunakan
a. Supervised Learning
b. Classification
c. Train-Test Split
d. Feature Scaling
e. Model Evaluation
f. Confusion Matrix
g. Accuracy Score

## Kesimpulan

Berdasarkan hasil analisis machine learning pada dataset Wine Quality:

1. Dataset berhasil diproses dengan baik tanpa missing values
2. Random Forest memberikan performa terbaik dibanding model lainnya
3. Feature scaling dan train-test split membantu meningkatkan validitas model
4. Model mampu memprediksi kualitas wine dengan cukup baik berdasarkan karakteristik kimianya

## Author
Nama: Jeni Anggraeni

Mata Kuliah: Machine Learning

Program Studi: D3 Statistika Terapan dan Komputasi
