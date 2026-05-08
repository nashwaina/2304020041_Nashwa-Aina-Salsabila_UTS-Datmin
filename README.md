# Dataset Wine Quality


# Pendahuluan

Data mining merupakan proses pengolahan dan analisis data untuk menemukan pola, hubungan, maupun informasi penting yang tersembunyi di dalam suatu kumpulan data. Dalam perkembangan teknologi dan pengolahan data saat ini, data mining banyak digunakan untuk membantu proses pengambilan keputusan pada berbagai bidang, seperti pendidikan, kesehatan, bisnis, industri, dan teknologi pangan. Salah satu teknik yang sering digunakan dalam data mining adalah klasifikasi. Klasifikasi merupakan metode supervised learning yang digunakan untuk memprediksi suatu kategori atau kelas berdasarkan data yang telah memiliki label sebelumnya. Melalui proses klasifikasi, sebuah model dapat mempelajari pola dari data training kemudian digunakan untuk memprediksi data baru yang belum diketahui kelasnya.

Data set Wine Quality dilakukan menganalisis dengan klasifikasi. Dataset tersebut berisi berbagai karakteristik kimiawi anggur, seperti fixed acidity, volatile acidity, citric acid, residual sugar, chlorides, alcohol, sulphates, pH, dan beberapa variabel lainnya yang memengaruhi kualitas anggur. Variabel target yang digunakan adalah quality, yaitu nilai kualitas anggur berdasarkan skala tertentu. Dataset yang digunakan terdiri dari dataset training yang memiliki label kualitas (quality) dan dataset testing yang belum memiliki label kualitas sehingga perlu dilakukan prediksi menggunakan model machine learning.

Dalam proses analisis ini digunakan beberapa metode klasifikasi, yaitu K-Nearest Neighbors (KNN), Decision Tree, dan Random Forest. Ketiga metode tersebut dipilih karena memiliki karakteristik yang berbeda dalam melakukan klasifikasi data. KNN bekerja berdasarkan kedekatan jarak antar data, Decision Tree menggunakan aturan berbentuk pohon keputusan, sedangkan Random Forest merupakan metode ensemble yang menggabungkan banyak pohon keputusan sehingga mampu menghasilkan performa klasifikasi yang lebih baik dan stabil. Seluruh model kemudian dievaluasi menggunakan accuracy score, classification report, dan confusion matrix untuk mengetahui performa masing-masing model dalam memprediksi kualitas anggur.

Melalui analisis ini diharapkan dapat diperoleh model klasifikasi terbaik yang mampu memprediksi kualitas anggur dengan tingkat akurasi yang baik. Selain itu, proses analisis ini juga bertujuan untuk memahami tahapan data mining mulai dari persiapan data, preprocessing, eksplorasi data, pembuatan model, evaluasi model, hingga prediksi data testing menggunakan machine learning

---

# Tujuan
Tujuan dari analisis data mining pada dataset Wine Quality ini adalah untuk membangun model klasifikasi yang mampu memprediksi kualitas anggur berdasarkan karakteristik kimiawi yang dimiliki setiap sampel anggur. Selain itu, analisis ini bertujuan untuk menerapkan tahapan data mining mulai dari persiapan data, pembersihan data, eksplorasi data, preprocessing, pembuatan model machine learning, evaluasi model, hingga prediksi data uji. Dalam penelitian ini digunakan beberapa metode klasifikasi, yaitu K-Nearest Neighbors (KNN), Decision Tree, dan Random Forest untuk dibandingkan performanya dalam memprediksi nilai `quality`. Evaluasi model dilakukan menggunakan accuracy score, classification report, dan confusion matrix untuk mengetahui model dengan performa terbaik. Setelah model terbaik diperoleh, model tersebut digunakan untuk memprediksi kualitas anggur pada dataset testing dan menghasilkan file prediksi dalam format CSV yang sesuai dengan ketentuan tugas UTS Data Mining.

---

# Proses Analisis
Dijelaskan pada bagian _issue_ yang ada di _github_ dan penjelasan proses juga ada di Teks Collab

---

# Hasil
Berdasarkan hasil prediksi menggunakan model Random Forest pada data testing, diperoleh distribusi nilai `quality` yang menunjukkan bahwa sebagian besar data diprediksi berada pada kualitas 5 dan 6. Hal ini terlihat dari hasil `value_counts()` dimana kualitas 5 diprediksi sebanyak 135 data dan kualitas 6 sebanyak 126 data. Selain itu, terdapat 24 data yang diprediksi memiliki kualitas 7 dan hanya 1 data yang diprediksi memiliki kualitas 8.

Hasil tersebut menunjukkan bahwa model Random Forest mengklasifikasikan mayoritas sampel anggur pada dataset testing ke dalam kategori kualitas menengah. Distribusi hasil prediksi ini juga sejalan dengan distribusi data pada dataset training sebelumnya, dimana kualitas 5 dan 6 memiliki jumlah data yang lebih dominan dibandingkan kelas lainnya. Karena model mempelajari pola dari data training, maka model cenderung lebih banyak memprediksi kelas yang memiliki jumlah data lebih besar.

Dengan demikian, hasil prediksi menunjukkan bahwa sebagian besar anggur pada data testing diperkirakan memiliki kualitas cukup baik, namun hanya sedikit sampel yang diprediksi memiliki kualitas sangat tinggi seperti quality 8.

---

# Link Collab
https://colab.research.google.com/drive/1BKo5uw8gEDPzNtID6cIapawqszW6vjCR?usp=sharing
