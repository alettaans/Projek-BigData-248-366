# 🏨 Hotel Bookings 🌟
![online-hotel-booking-concept-for-web-banner-vector-24954084](https://github.com/user-attachments/assets/bb291f45-1d30-479e-b550-b41f20e30357)

# Table of Content
1. [Introduction](#introduction)
2. [Problem](#Problem)
3. [Problem Solving Plan](#Problem_Solving_Plan)
4. [Analysis Techniques](#Analysis_Techniques)
5. [Workflow](#Workflow)
6. [Dataset](#Dataset)
7. [Dependencies](#Dependencies)
8. [Get Started](#Get_Started)
9. [License](#License)
10. [Team](#Team)

## Introduction
Proyek ini bertujuan untuk menganalisis data pemesanan hotel guna memahami pola dan faktor yang mempengaruhi pembatalan pemesanan. Dengan menggunakan berbagai teknik analisis data, termasuk Exploratory Data Analysis (EDA), pembersihan data (preprocessing), dan pembelajaran mesin (machine learning), proyek ini bertujuan memberikan wawasan yang berguna bagi pengelola hotel dalam membuat keputusan yang lebih baik. Proyek ini dikerjakan dan diselesaikan dengan dua orang dalam satu tim oleh mahasiswa Universitas Muhammadiyah Malang untuk memenuhi tugas mata kuliah Analisis Big Data. Berikut data anggota:
1. Septiannisa Alya Shinta Purwandhani (202110370311248)
2. Aletta Agigia Novta Sajiatmoko (202110370311366)
 
## Problem
Dalam dunia industri perhotelan yang kompetitif, salah satu tantangan utama yang dihadapi oleh para pengelola adalah tingginya angka pembatalan pemesanan kamar oleh pelanggan. Kondisi ini tidak hanya berdampak pada pendapatan hotel, tetapi juga memengaruhi efisiensi dalam mengelola sumber daya yang tersedia, seperti ketersediaan kamar dan alokasi tenaga kerja. Permasalahan ini menjadi semakin kompleks terutama bagi hotel-hotel dengan kapasitas kamar yang terbatas, di mana setiap pembatalan pemesanan dapat menyebabkan kerugian yang signifikan. Oleh karena itu, memahami pola pembatalan pemesanan dan memprediksi kemungkinan pembatalan menjadi langkah yang sangat penting untuk mengoptimalkan strategi pengelolaan dan memastikan kepuasan pelanggan tetap terjaga.  

Dengan melakukan analisis terhadap data pemesanan hotel, pengelola dapat mengevaluasi pola-pola tertentu dalam pemesanan dan pembatalan. Melalui pendekatan ini, dimungkinkan untuk mengidentifikasi faktor-faktor yang memengaruhi pelanggan dalam mengambil keputusan untuk membatalkan reservasi mereka. Wawasan yang diperoleh dari analisis tersebut dapat menjadi landasan bagi pengelola hotel dalam merancang strategi pemesanan yang lebih efektif, yang tidak hanya mampu mengurangi angka pembatalan tetapi juga meningkatkan akurasi perencanaan ketersediaan kamar. Pada akhirnya, langkah ini diharapkan dapat memberikan manfaat yang signifikan, baik dalam hal peningkatan efisiensi operasional hotel maupun pengalaman pelanggan secara keseluruhan.

## Problem Solving Plan
Data yang tersedia meliputi informasi mengenai jenis hotel, status pembatalan, lead time (yaitu jangka waktu antara pemesanan dan kedatangan), jenis layanan makanan yang tersedia, dan banyak lagi. Analisis ini akan dilakukan menggunakan metodologi yang terdiri dari beberapa tahapan, yaitu:

![Multicolor Pastel Modern Corporate Infographic And Chart Presentation](https://github.com/user-attachments/assets/d30eaab1-f19b-4277-a4a2-efd1bd008601)

- Data Preprocessing: Melibatkan penanganan data yang hilang, mengubah variabel kategorikal menjadi format numerik, serta melakukan normalisasi untuk memastikan data siap digunakan.
- Modeling: Menerapkan teknik pembelajaran mesin, yaitu Random Forest untuk memprediksi peluang pembatalan berdasarkan variabel yang tersedia.
- Model Evaluation: Menilai performa model menggunakan metrik evaluasi seperti akurasi, precision, recall, dan F1-score untuk mengukur sejauh mana model dapat memprediksi pembatalan secara akurat.

## Analysis Techniques
Pada tahap awal, dilakukan eksplorasi data (EDA) untuk memahami distribusi dan pola yang ada dalam dataset. Berbagai visualisasi, seperti grafik distribusi, histogram, dan heatmap, digunakan untuk mengidentifikasi variabel-variabel yang memiliki pengaruh signifikan terhadap pembatalan reservasi dan preferensi pelanggan. Selain itu, EDA juga berfungsi untuk mendeteksi keberadaan nilai yang hilang atau outlier dalam data, yang harus diperbaiki agar model yang dihasilkan memiliki akurasi yang lebih baik.

Pendekatan analisis berfokus pada pemodelan klasifikasi untuk memprediksi kemungkinan pembatalan pemesanan. Salah satu algoritma yang digunakan adalah Random Forest, yang membantu dalam mengidentifikasi variabel-variabel paling berpengaruh terhadap pembatalan serta memprediksi peluang pembatalan di masa mendatang. Random Forest memiliki keunggulan dalam mengatasi masalah overfitting, terutama pada dataset dengan banyak fitur, dan dapat memberikan wawasan yang lebih mendalam melalui analisis feature importance yang dihasilkan oleh model.

## Workflow
![Multicolor Pastel Modern Corporate Infographic And Chart Presentation (1)](https://github.com/user-attachments/assets/2f157bcf-45bc-48c3-88c1-23294aea8b2c)

Proses analisis dimulai dengan mengimpor berbagai package yang diperlukan, seperti [Pandas](https://pandas.pydata.org/) untuk manipulasi data, [NumPy](https://numpy.org/) untuk operasi numerik dan array [Matplotlib](https://matplotlib.org/) dan [Seaborn](https://seaborn.pydata.org/) untuk visualisasi, dan [scikit-learn](https://scikit-learn.org/stable/) untuk normalisasi, encoding, pemodelan dan evaluasi. Setelah itu, dataset diimpor untuk memulai analisis.

Setelah dataset dimuat, tahap pertama adalah Exploratory Data Analysis (EDA), di mana data dieksplorasi untuk memahami distribusi variabel, hubungan antar fitur, dan mendeteksi masalah seperti data yang hilang atau pencilan.

Kemudian, proses Preprocessing dilakukan untuk menyiapkan data agar siap digunakan dalam model pembelajaran mesin. Langkah ini meliputi penanganan data yang hilang, konversi variabel kategorikal menjadi format numerik, dan normalisasi data.

Setelah data siap, tahap Modeling dimulai, pada kasus ini model yang digunakan adalah [Random Forest](https://scikit-learn.org/1.5/modules/generated/sklearn.ensemble.RandomForestClassifier.html). Diterapkan untuk memprediksi pemesanan dan pembatalan berdasarkan fitur yang tersedia.

Terakhir, Evaluation dilakukan untuk menilai kinerja model menggunakan [evaluation metrics](https://scikit-learn.org/1.5/api/sklearn.metrics.html) seperti akurasi, precision, recall, dan F1-score, guna memastikan model dapat memprediksi dengan baik dan akurat.

## Dataset
Dataset yang digunakan diambil dari website [github](https://github.com/rfordatascience/tidytuesday/blob/main/data/2020/2020-02-11/readme.md), yang dimana dataset tersebut diambil dari penelitian yg dilakukan oleh [Antonio, Almeida, dan Nunes, 2019](https://www.sciencedirect.com/science/article/pii/S2352340918315191#f0010). Dataset ini berisi informasi mengenai permintaan pemesanan hotel yang didalamnya terdapat banyak variabel seperti negara, jumlah booking yang pernah di cancel sebelumnya, tamu yang memesan secara berulang atau tidak, jumlah orang dewasa, jumlah reservasi berdasarkan bulan kedatangan, status reservasi dan masih banyak variabel lainnya lagi yang tentunya dengan class/tipe data yang berbeda. Tipe data/claass yang tersedia pada dataset ini adalah integer, float, dan object. Dataset dapat di download [disini](https://github.com/rfordatascience/tidytuesday/blob/main/data/2020/2020-02-11/hotels.csv)

## Dependencies
Berikut daftar dependensi yang dibutuhkan agar code yang tertera dapar dijalankan dengan baik

## Get Started
Untuk memulai proyek ini, pastikan Anda telah menginstal semua package yang dibutuhkan. Anda dapat melakukannya dengan mengikuti langkah-langkah berikut:

1. **Clone repository** ini ke mesin lokal Anda:
   ```bash
   git clone https://github.com/username/repository-name.git
   ```

2. **Instal dependencies** menggunakan `pip`:
   ```bash
   pip install -r requirements.txt
   ```

3. **Impor dataset**: Pastikan Anda memiliki [dataset](https://github.com/rfordatascience/tidytuesday/blob/main/data/2020/2020-02-11/hotels.csv) yang sesuai dan letakkan di direktori yang telah ditentukan dalam kode.

4. **Jalankan Kode**: Jalankan kode sesuai dengan urutan yang sudah ada.

## License
Repository ini dibuat dengan akses penuh.

## Team
- Septiannisa Alya Shinta
- Aletta Agigia Novta Sajiatmoko
