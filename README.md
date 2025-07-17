# Analisis-Pola-Kesehatan-dan-Prediksi-Risiko-Diabetes-Menggunakan-EDA-dan-Machine-Learning
Proyek ini bertujuan untuk menganalisis dan memprediksi risiko diabetes berdasarkan data medis pasien menggunakan metode *data science*. Dengan memanfaatkan teknik *exploratory data analysis (EDA)* dan model prediktif **XGBoost**, proyek ini memberikan pendekatan sistematis dalam mendeteksi dini kemungkinan diabetes, khususnya sebagai alat bantu skrining awal di lingkungan klinis atau rumah sakit.

---

## 🔍 Metodologi: CRISP-DM

Proyek ini menggunakan pendekatan **CRISP-DM** (*Cross Industry Standard Process for Data Mining*), yang terdiri dari:

### 1. Business Understanding
Memahami bahwa deteksi dini diabetes sangat penting untuk mencegah komplikasi lebih lanjut. Sistem prediktif ini bertujuan untuk membantu profesional kesehatan dalam mengevaluasi risiko pasien menggunakan data sederhana dan mudah diperoleh.

### 2. Data Understanding
Dataset yang digunakan adalah **Pima Indians Diabetes Dataset**, yang memuat data kesehatan dari perempuan keturunan Indian Pima. Atribut yang tersedia meliputi:

- Pregnancies
- Glucose
- BloodPressure
- SkinThickness
- Insulin
- BMI
- DiabetesPedigreeFunction
- Age
- Outcome (label: 0 = tidak diabetes, 1 = diabetes)

### 3. Data Preparation
- Mengganti nilai nol pada kolom medis (seperti BMI, Glucose, Insulin) dengan median/mean sebagai bentuk imputasi.
- Standarisasi dan normalisasi fitur jika diperlukan.
- Pembagian data menjadi training dan test set.

### 4. Exploratory Data Analysis (EDA)
Dilakukan analisis eksploratif untuk:
- Memahami distribusi tiap fitur
- Menganalisis korelasi antar fitur dengan label
- Mengidentifikasi fitur yang paling berpengaruh terhadap risiko diabetes
- Visualisasi dengan histogram, heatmap, dan boxplot

### 5. Modeling – XGBoost Classifier
Model utama yang digunakan adalah **XGBoost (Extreme Gradient Boosting)**, karena performanya yang unggul dalam tugas klasifikasi:

- Dilatih pada data training dan diuji pada data test
- Parameter model dituning untuk menghindari overfitting
- Fitur penting (*feature importance*) diekstrak untuk memahami kontribusi masing-masing fitur

### 6. Evaluation
Model dievaluasi menggunakan metrik:
- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix

Hasil evaluasi menunjukkan bahwa XGBoost dapat memprediksi risiko diabetes dengan tingkat akurasi yang cukup tinggi, serta mampu menangani data medis dengan baik.

---

## 📁 Sumber Data

Dataset:
📌 **Pima Indians Diabetes Dataset**  
Sumber:  
- [Kaggle](https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database)

---

## 🛠 Tools & Library

- Python 3.x
- Pandas, NumPy
- Seaborn, Matplotlib
- Scikit-learn
- XGBoost
- Jupyter Notebook
