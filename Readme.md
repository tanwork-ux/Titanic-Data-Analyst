# 🚢 Proyek Analisis Data Kasus Studi Titanic
*(Menggunakan dataset dari Kaggle untuk latihan Data Analyst.)*

## 📄 Deskripsi Proyek
Proyek ini adalah studi kasus untuk latihan Data Analyst menggunakan dataset Titanic. Saya menggunakan **Virtual Environment (Venv)** dan **Jupyter Notebook** di **Visual Studio Code** untuk melakukan seluruh proses analisis.

## 🛠️ Metodologi Analisis
Berikut adalah langkah-langkah utama yang saya lakukan dalam proyek ini:

### 1. Persiapan Data
* Menginstal *dependencies* penting: Pandas, NumPy, Seaborn, dan Matplotlib.
* Mengimpor dataset mentah berbentuk CSV.

### 2. Penanganan Missing Values (Data Cleaning)
* Melakukan pengecekan data dengan `df.info()` dan menemukan 3 kolom yang memiliki *missing value* (data null): **Age**, **Cabin**, dan **Embarked**.
* **Kolom 'Age':** Karena data *null* hanya 20%, saya mengisi nilai *null* dengan **median** (metode imputasi yang aman).
* **Kolom 'Cabin':** Karena data *null* mencapai 77%, kolom ini saya **hapus** karena tingkat kehilangan data yang terlalu tinggi.
* **Kolom 'Embarked':** Karena data *null* hanya 2 baris, saya memutuskan untuk **mengisi** dengan metode pengisian yang terbaik.

### 3. Visualisasi dan Eksplorasi Data (EDA)
Setelah proses seleksi dan pembersihan data, saya melakukan visualisasi untuk memahami distribusi data:
* **Histogram** untuk menampilkan distribusi usia penumpang.
* **Pie Chart** untuk proporsi penumpang berdasarkan jenis kelamin.
* **Box Plot** untuk membandingkan peluang kelangsungan hidup berdasarkan usia.
* **Bar Plot** untuk persentase kelangsungan hidup berdasarkan kelas penumpang.
* **Bar Plot** untuk Persentase Kelangsungan Hidup berdasarkan jenis kelamin.
* Menyajikan *bar plot* data hasil agregasi untuk jumlah penumpang Pria dan Wanita.

## 💾 Hasil Akhir
* Setelah selesai, saya mengekstrak data hasil agregasi ke file **CSV** baru.