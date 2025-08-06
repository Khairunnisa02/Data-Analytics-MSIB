# Data-Analytics-MSIB
Proyek 'data analytics' di PT Zenius Education menggunakan google colab

Judul: "Analisis Klien Gagal Bayar Dengan Membandingkan Beberapa Algoritma yang Berbeda"
Link Google Colab:
1. Data Understanding
   - https://colab.research.google.com/drive/1ZPGt42PEyEy5Gzv5FoS8iD-0RTrbEk6T?usp=sharing
   - https://colab.research.google.com/drive/1L2pGisUQNHy5vDyR02594PDFqajI2O4G?usp=sharing
3. Data Preprocessing
   - https://colab.research.google.com/drive/1Ld5TXTqL0XecjrUWCWuzLWYcykOU0h0y?usp=sharing
5. Modelling & Evaluation
   - https://colab.research.google.com/drive/1XkkAdNSDFI91uk5mDG6J48Hot0rs3yFl?usp=sharing
Tujuan analisis:
- Mengidentifikasi potensi gagalnya membayar pinjaman berdasarkan data historis, menggunakan indikator keuangan dan non-keuangan
- Membuat model yang dapat memprediksi seberapa tinggi kemampuan konsumen dalam membayar angsuran demi memastikan penyaluran pinjaman yang lebih maksimal kepada nasabah yang lebih berkemungkinan dapat membayar angsuran dengan lancar. Model terfokuskan pada konsumen yang diprediksi gagal bayar nyatanya konsumen mampu membayar.
Terdapat 4 Notebook dan penjelasan tiap Notebook:
1. Exploratory Data Analysis (EDA)
   - Membaca dan memvisualisasikan tiap variabel
3. Exploratory Data Analysis (EDA) 2
   - Membaca dan memvisualisasikan tiap variabel
5. Data Preprocessing
   - Mengatasi masalah missing value dengan menghapus kolom yang memiliki persentase missing value diatas 60% dan beberapa dilakukan penanganan dengan mengganti NaN menggunakan nilai median, mean, dan modus. Untuk variable kategorik digunakan penanganan dengan nilai modus dan untuk variable numeric digunakan penanganan dengan nilai median dan mean.
   - Melakukan categorical data enconding.
   - Mengatasi masalah outlier dengan mengganti menggunakan nilai median.
   - Menghapus beberapa variabel yang tidak dibutuhkan.
6. Modelling & Evaluation
   - Logistic Regression
   - K-Nearest Neighbors
   - Decision Tree (menjadi model terbaik yang digunakan untuk pengambilan kesimpulan)
   - Random Forest
   - XGB Classifier

Kesimpulan:

Home Credit untuk memperluas inklusi keuangan bagi populasi yang tidak memiliki rekening bank dengan memberikan pengalaman meminjam yang positif dan aman. Dalam meminjamkan kredit, perusahan menghadapi risiko bernama default risk. Default risk adalah risiko bahwa pemberi pinjaman memberikan pinjaman kepada peminjam yang akan tidak bisa membayar sesuai dengan hutang yang dimiliki. Home Credit Default Risk adalah risiko gagal bayar kredit rumah atau risiko kredit macet pada sektor perumahan. Oleh karena itu, diperlukan suatu cara untuk mengidentifikasi potensi nasabah yang gagal bayar pinjaman (default) berdasarkan data historis, menggunakan indikator keuangan dan non-keuangan. Dengan menggunakan machine learning, dapat dibuat model yang bisa mengidentifikasi hal tersebut.

Setelah melakukan analisis menggunakan 5 algoritma, diputuskan menggunakan model Decision Tree karena model ini memiliki nilai recall tertinggi. Hal ini dikarekan ingin melihat kemampuan model dalam meminimalisir kesalahan saat memprediksi nasabah yang tidak akan gagal bayar (False Negative). Berdasarkan hasil analisis EDA, terdapat beberapa tipe klien yang perlu diutamakan/ dicari, seperti klien yang telah memilih pinjaman Bergulir lebih kecil kemungkinannya untuk gagal bayar. Selain itu, klien dengan status kontrak 'Disetujui' lebih kecil kemungkinannya untuk default terlepas dari variabel lainnya. Ada pun Klien yang merupakan pengusaha atau mahasiswa lebih kecil kemungkinannya untuk wanprestasi. Klien dengan gelar akademik lebih kecil kemungkinannya untuk gagal bayar. Serta klien yang tinggal di apartemen kantor cenderung kecil kemungkinannya untuk gagal bayar. Sedangkan, berdasarkan hasil analisis model Decision Tree, terdapat beberapa variabel yang dapat dipertimbangkan, yaitu indeks tingkat kepercayaan kredit pelanggan, usia nasabah, berapa hari sebelum aplikasi nasabah, lamanya nasabah mengajukan pinjaman, jumlah kredit yang diberikan kepada nasabah, jumlah hari nasabah mengganti nomor, dan total pendapatan pelanggan.
