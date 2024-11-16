# Laporan Proyek Machine Learning Prediksi Penumpang Mana Saja yang Selamat dari Bangkai Kapal Titanic - Robiul Awal

## Domain Proyek

Bencana paling terkenal yang terjadi lebih dari seabad lalu pada tanggal 15 April 1912, yang dikenal sebagai tenggelamnya "Titanic". Tabrakan dengan gunung es tersebut menghancurkan banyak bagian Titanic. Banyak orang dari segala usia dan jenis kelamin hadir pada malam yang menentukan itu, tetapi sialnya hanya ada beberapa sekoci penyelamat yang harus diselamatkan. Korban tewas termasuk sejumlah besar pria yang tempatnya diberikan kepada banyak wanita dan anak-anak di atas kapal. Orang-orang yang bepergian di kelas dua tewas di pohon anggur (Kakde,  Yogesh  & Agrawal, Shefali. 2018).

Pada tanggal 15 April 1912, selama pelayaran perdananya, RMS Titanic yang secara luas dianggap "tidak dapat tenggelam" tenggelam setelah bertabrakan dengan gunung es. Sayangnya, tidak ada cukup sekoci untuk semua orang di dalamnya, yang mengakibatkan kematian 1502 dari 2224 penumpang dan awak kapal (Alexis Cook. 2022).

Meskipun ada sedikit unsur keberuntungan yang terlibat dalam bertahan hidup, tampaknya beberapa kelompok orang lebih mungkin untuk bertahan hidup daripada yang lain.

Kita harus melakukan analisis lengkap tentang jenis atau macam penumpang Titanic yang mungkin selamat dalam bencana Titanic. Jenis penumpang termasuk mereka yang bepergian sendiri dan penumpang dengan keluarga mereka. Jenis penumpang dapat dianalisis berdasarkan ukuran keluarga, ukuran keluarga harus dikategorikan menjadi tiga kategori seperti keluarga tunggal, keluarga kecil dan keluarga besar, dan masih banyak faktor lainnya (Md Arfinul Haque etc. 2020).

Dalam proyek ini, model prediktif akan dibangun yang menjawab pertanyaan: "tipe orang seperti apa yang lebih mungkin untuk bertahan hidup?" menggunakan data penumpang (misalnya nama, usia, jenis kelamin, kelas sosial ekonomi, dll.).

- Penjelasan mengapa dan bagaimana masalah tersebut harus diselesaikan

Kecelakaan merupakan kejadian yang dapat merugikan banyak pihak mulai dari individu sampai instansi. Terlebih lagi jika kecelakaan tersebut memakan banyak korban jiwa. Seperti pada sejarah kecelakaan Tenggelamnya Titanic tahun 1912 mengakibatkan tingginya kekhawatiran orang dalam menaiki kapal laut. Oleh karena itu, perlu adanya solsui untuk menekan dan mengurangi jumlah korban jiwa yang ada jika suatu saat nanti terjadi kecelakaan kembali. Salah satunya menganalisis data, mengetahui, dan memprediksi karakteristik orang seperti apa yang lebih mungkin untuk bertahan hidup. 

Berdasarkan hasil pengolahan data ini, instansi terkait dapat menemukan referensi yang dapat dipercaya karena referensi berdasarkan data untuk mengambil keputusan dengan bijak dalam menangani risiko kecelakaan suatu saat nanti. Contoh pihak instansi terkait dapat memberikan fasilitas keamanan yang lebih bagi orang-orang yang diprediksi kemungkinan untuk hidup jika terjadi kecelakaan. Dengan ini, orang-orang dapat merasakan keamanan yang lebih dalam menaiki kapal laut.

## Business Understanding
Pada proyek klasifikasi penumpang Titanic yang selamat, identifikasi situasinya adalah mengetahui bahwa jumlah penumpang yang selamat dan tidak selamat berbeda, dan beberapa faktor (misalnya, umur, jenis kelamin, dan kelas kabin) mungkin memengaruhi peluang keselamatan. Pada proyek Titanic ini, tantangan yang mungkin dihadapi adalah model klasifikasi yang tidak dapat memprediksi keselamatan penumpang dengan tingkat akurasi yang memadai karena data yang tidak seimbang atau faktor-faktor tertentu yang sulit diprediksi. Tujuan proyek klasifikasi Titanic mungkin adalah untuk meningkatkan kemampuan model dalam memprediksi apakah seorang penumpang akan selamat atau tidak berdasarkan data demografis dan data perjalanan, serta untuk membantu memahami faktor-faktor yang paling memengaruhi keselamatan penumpang. Berdasarkan hal ini dapat dirumuskan beberapa problem statements seperti berikut ini.

### Problem Statements
- Bagaimana karakteristik orang yang memiliki kemungkinan lebih untuk hidup ketika terjadi kecelakaan kapal Titanic?
- Berdasarkan banyak faktor atau variabel, faktor apa yang paling berpengaruh terhadap kemungkinan lebih untuk hidup ketika terjadi kecelakaan kapal Titanic?
- Bagaimana kemungkinan hidup sesorang dengan karakteristik dan faktor tertentu ketika terjadi kecelakaan kapal Titanic?

### Goals
- Mengetahui karakteristik orang yang memiliki kemungkinan lebih untuk hidup ketika terjadi kecelakaan kapal Titanic.
- Mengetahui faktor apa yang paling berpengaruh terhadap kemungkinan lebih untuk hidup ketika terjadi kecelakaan kapal Titanic.
- Membuat model machine learning yang dapat memprediksi kemungkinan hidup seseorang berdasarkan karakteristik dan faktor yang ada.

### Solution statements
Tujuan pada proyek ini adalah memprediksi keselamatan sesorang terhadap kecelakaan kapal Titanic berdasarkan karakteristik dan faktor tertentu. Pada kasus ini, hasil prediksi hanya berupa dua nilai yaitu hidup (1) atau mati (0). Berdasarkan hal tersebut, artinya kasus ini merupakan masalah klasifikasi. Oleh karena itu, metodologi dalam proyek ini adalah membangun model klasifikasi keselamatan penumpang kapal berdasarkan karakteristik dan faktor yang dimiliki orang tersebut pada kecelakaan kapal Titanic. Sementara itu, algoritma yang digunakan ada tiga yaitu, Support Vector Machine (SVM), Random Forest Classifier, dan K-Neighbors Classifier. Setiap model dilakukan hyperparameter tuning untuk mendapatkan hasil akurasi skor yang tinggi. Dari hasil evaluasi terebut, maka akan dipilih satu model yang memiliki tingkat akurasi training dan test tertinggi untuk memprediksi dataset baru.

Evaluasi model pada model klasifikasi sangat penting untuk menentukan seberapa baik model dapat memprediksi kelas dari data baru. Evaluasi ini menggunakan berbagai metrik untuk menilai performa model, yang mencakup kemampuan model dalam membedakan kelas positif dan negatif secara benar. Metrik evaluasi digunakan untuk mengevaluasi tingkat keakuratan model dalam memprediksi keselamatan penumpang. Dalam proyek ini, metrik yang digunakan adalah accuracy score, precission score, recall score, f1 score, dan confussion matrix. Matrik seperti accuracy score akan memberikan presentase keberhasilan model dalam memprediksi output dengan benar. Precision mengukur ketepatan dari prediksi positif, atau seberapa banyak prediksi positif yang benar dari semua yang diprediksi sebagai positif. F1 Score adalah rata-rata harmonis dari precision dan recall. Ini memberikan keseimbangan antara keduanya dan cocok digunakan jika terdapat ketidakseimbangan antara precision dan recall. Recall mengukur seberapa baik model dalam menemukan semua contoh positif yang benar dari total kelas positif yang sebenarnya. Confusion matrix adalah tabel yang menunjukkan jumlah prediksi benar dan salah yang dibuat oleh model, dibagi berdasarkan kelas aktual dan kelas yang diprediksi. 

## Data Understanding
Kumpulan dataset ini mencakup informasi penumpang seperti id penumpang, nama, usia, jenis kelamin, kelas sosial ekonomi, jumlah saudara dan orang tua yang bersama sebagai penumpang, tarif penumpang, nomor tiket, nomor kabin penumpang, dan pelabuhan keberangkatan. Sebagian informasi-informasi tersebut merupakan variabel dan faktor yang dapat mempengaruhi keselamatan penumpang pada kecelakaan kapal Titanic. Variabel yang digunakan dalam pembuatan model prediktif kali ini yaitu usia, jenis kelamin, kelas sosial ekonomi, jumlah saudara yang bersama sebagai penumpang, jumlah orang tua yang bersama sebagai penumpang, tarif penumpang, dan pelabuhan keberangkatan. Sementara variabel Id penumpang, nama, nomor tiket, dan nomor kabin tidak digunakan karena merupakan data unik yang tidak akan berpengaruh dalam hasil prediksi. Terdapat dua dataset yaitu satu kumpulan data berjudul train.csv dan yang lainnya berjudul test.csv.

Train.csv akan berisi detail sebagian penumpang di dalam pesawat (tepatnya 891 rekaman) dan yang terpenting, akan mengungkapkan apakah mereka selamat atau tidak, yang juga dikenal sebagai "ground truth" (Will Cukierski. 2012).

Kumpulan data test.csv berisi informasi serupa tetapi tidak mengungkapkan "ground truth" untuk setiap penumpang. Ini akan menjadi tugas yang harus diselesaikan yaitu memprediksi hasil ini. Dengan menggunakan pola yang ditemukan dalam data train.csv, akan diprediksi apakah 418 penumpang lainnya di dalam pesawat (ditemukan di test.csv) selamat (Will Cukierski. 2012). 

Pengumpulan data dilakukan dengan mengunduh dataset dari sumber referensi resmi dari Kaggle yaitu pada link berikut [kaggle download -c titanic](https://www.kaggle.com/competitions/titanic/data)

### Variabel-variabel pada -c Titanic dataset adalah sebagai berikut:
- PassengerId : merupakan Id yang dimiliki penumpang.
- Survived : merupakan status keselamatan penumpang Titanic. (0 = No, 1 = Yes)
- Pclass : merupakan kelas tiket yang dimiliki penumpang. (1 = 1st (upper), 2 = 2nd (middle), 3 = 3rd (lower))
- Name : merupakan nama dari penumpang.
- Sex : merupakan jenis kelamin penumpang.
- Age : merupakan usia penumpang dalam tahun.
- SibSp : merupakan jumlah saudara kandung / pasangan yang berada di atas Titanic
- Parch : merupakan jumlah orang tua/anak di atas Titanic.
- Ticket : merupakan nomor tiket yang dimiliki penumpang.
- Fare : merupakan tarif yang dibayar oleh penumpang
- Cabin : merupakan nomor kabin yang dimiliki penumpang
- Embarked : merupakan pelabuhan keberangkatan dari penumpang. (C = Cherbourg, Q = Queenstown, S = Southampton)

### Exploratory Data Analysis

Pada proyek ini dilakukan juga proses exploratory data analysis (EDA). EDA merupakan proses investigasi awal pada data untuk menganalisis karakteristik, menemukan pola, anomali, dan memeriksa asumsi pada data. Teknik ini biasanya menggunakan bantuan statistik dan representasi grafis atau visualisasi.  Proses ini untuk mengetahui beberapa hal seperti berikut ini:
- Apa saja jenis variabel pada dataset?
Untuk menetahui jenis variabel pada dataset sudah dilakukan sebelumnya yaitu memahami definsi dari setiap variabel. Kemudian menggunakan perintah `dataset.info()` untuk mengetahui tipe dari setiap variabel. Berdasarkan output di atas ini, dapat diketahui bahwa terdapat 5 variabel yang bertipe data numerik int64, terdapat 2 variabel yang bertipe data numerik float64, terdapat 5 variabel yang bertipe karakter atau object.
- Apakah ada missing value?
Untuk mengetahui nilai kosong dapat menggunakan perintah `dataNull = data_train.isnull().sum()`. Berdasarkan output, dapat diketahui bahwa terdapat data kosong pada variabel Age sebanyak 177 data, pada variabel Cabin sebanyak 697 data, dan pada variabel Embarked sebanyak 2 data. Setelah dilakukan analisis variabel, perlu dilakukan pembersihan dataset ini agar dapat diolah dengan baik. Pada proyek ini akan dilakukan pembersihan pada beberapa varibel. Yang pertama akan dilakukan penghapusan baris yang memiliki data kosong pada varibael Age dan Embarked. 
- Apakah ada fitur yang tidak berguna (redundant)?
Kemudian diputuskan beberapa variabel untuk dihapus karena merupakan noise atau redundant yang tidak memiliki pengaruh pada model prediksi dalam proyek ini. Data-data tersebut data unik yang bukan merupakan faktor hidup atau matinya penumpang pada kecelakaan kapal Titanic karena sama sekali tidak menyebabkan hal itu terjadi. Variabel yang akan dihapus diantaranya, Id penumpang, nama, nomor tiket, dan nomor kabin,
- Bagaimana distribusi variabel dalam dataset?
Untuk mengetahui distribusi variabel dalam dataset, dilakukan analisis unvariat. ![image](https://github.com/user-attachments/assets/9101400a-9414-4616-a847-32b3895e0fb0) Berdasarkan analisis unvariat diperoleh hasil sebagai berikut. Penumpang kapal titanic dengan jenis kelamin laki-laki lebih banyak daripada perempuan. ![image](https://github.com/user-attachments/assets/b407cb94-612a-4bdc-b5ca-6f6ddac93070) Sebagian besar penumpang berangkat dari pelabuhan S (Shouthampton). ![image](https://github.com/user-attachments/assets/b704d53f-7675-4bca-bc42-45470d1cea7d) Berdasarkan grafik juga dapat disimpulkan bahwa lebih banyak penumpang yang mengalami kematian daripada penumpang yang selamat.
- Bagaimana korelasi antara fitur dan target?
Untuk mengetahui hal ini, dilakukan analisis multivariat. Proses dilakukan dengan cara mencari korelasi antar variabel. ![image](https://github.com/user-attachments/assets/3c1b5c9b-3130-47c6-87a7-3fbacd72e9d5) Berdasarkan grafik korelasi diperoleh bahwa setiap variabel memiliki korelasi yang rendah dengan variabel yang lain. Sementara itu, variabel yang paling berpengaruh diantara yang lain terhadap keselamatan penumpang pada kecelakaan kapal Titanic adalah fare atau tarif penumpang.

## Data Preparation
Teknik yang digunakan dalam data preparation data adalah sebagai berikut:
1. Penanganan Missing Value dan Noise
2. Encoding data menggunakan OneHotEncoder
3. Pemisahan data menjadi data faktor (x) dan data target (y)
4. Over sampling data menggunakan RandomOverSampler()
5. Normalisasi data numerik dengan StandardScaler()
6. Feature Selection

- Penjelasan proses data preparation yang dilakukan

1. Penanganan Missing Value
Setelah menganalisis variabel, perlu dilakukan pembersihan dataset agar dapat diproses dengan baik. Dalam proyek ini, pembersihan akan dilakukan pada beberapa variabel. Yang pertama adalah penghapusan baris yang memiliki data kosong pada variabel Age dan Embarked. Perintah untuk menangani missing value adalah sebagai berikut.
```
# Create a new DataFrame (clean_df) by removing rows that have missing values ​​(NaN) from data_train
clean_df = data_train.dropna(subset=['Age'])
clean_df = clean_df.dropna(subset=['Embarked'])
```
- Kemudian diputuskan bahwa beberapa variabel akan dihilangkan karena bersifat noise atau redundan yang tidak berpengaruh terhadap model prediksi dalam proyek ini. Data tersebut merupakan data unik yang bukan merupakan faktor dalam hidup atau matinya penumpang dalam kecelakaan Titanic karena sama sekali tidak menyebabkan terjadinya kecelakaan tersebut. Variabel yang akan dihilangkan antara lain, ID Penumpang, nama, nomor tiket, dan nomor kabin. Berikut ini perintah untuk menghilangkan noise.
```
# Removing noise from a dataset
clean_df.drop(['PassengerId', 'Name', 'Ticket', 'Cabin'], inplace=True, axis=1)
```
2. Encoding data menggunakan OneHotEncoder
Untuk melakukan proses encoding fitur kategori, salah satu teknik yang umum dilakukan adalah teknik one-hot-encoding. Library scikit-learn menyediakan fungsi ini untuk mendapatkan fitur baru yang sesuai sehingga dapat mewakili variabel kategori. Pada proyek ini terdapat dua variabel kategori yaitu 'sex' dan 'embarked'. Proses encoding ini dilakukan agar variabel yang nilainya objek dapat menjadi nilai numerik sehingga dapat diolah. Proses encoding ini dilakukan dengan fitur get_dummies. Proses encoding menggunakan perintah seperti berikut ini.
```
one_hot_encoder = OneHotEncoder(sparse_output=False)
data_final = pd.concat([clean_df, pd.get_dummies(clean_df['Sex'], prefix='Sex').astype(int)],axis=1)
data_final = pd.concat([data_final, pd.get_dummies(data_final['Embarked'], prefix='Embarked').astype(int)],axis=1)
data_final.drop(['Sex','Embarked'], axis=1, inplace=True)
```
3. Over sampling data menggunakan RandomOverSampler()
Over-sampling adalah teknik untuk menyeimbangkan jumlah data antara kelas mayoritas dan minoritas dalam dataset yang tidak seimbang. Metode yang digunakan untuk over-sampling pada proyek ini adalah RandomOverSampler dari pustaka imbalanced-learn. Teknik ini menambahkan salinan acak dari sampel di kelas minoritas hingga jumlahnya seimbang dengan kelas mayoritas. Dalam kasus ini, proses oversampling dilakukan untuk menyeimbangkan rekaman yang memiliki nilai survived 0 dan 1. Proses over sampling dilakukan dengan perintah sebagai berikut.
```
# Oversampling menggunakan RandomOverSampler
ros = RandomOverSampler(random_state=42)
X_resampled, y_resampled = ros.fit_resample(X, y)
```
4. Splitting Data dengan fungsi train_test_split dari library sklearn
`train_test_split()` adalah fungsi dari pustaka scikit-learn yang digunakan untuk membagi dataset menjadi dua atau lebih bagian, seperti data pelatihan (training set) dan data pengujian (testing set). Pemisahan ini penting dalam pembelajaran mesin untuk mengevaluasi performa model dengan menggunakan data yang tidak pernah dilihat oleh model selama pelatihan, sehingga memberikan gambaran yang lebih realistis tentang kinerja model pada data yang tidak terlihat. Perintah yang digunakan untuk splitting data adalah
```
X_train, X_test, y_train, y_test = train_test_split(X_resampled, y_resampled, test_size = 0.1, random_state = 42)
```
5. Normalisasi data numerik dengan StandardScaler()
Normalisasi atau standarisasi data adalah proses mengubah skala fitur numerik sehingga memiliki sifat statistik tertentu, biasanya dengan tujuan membuat model pembelajaran mesin lebih stabil dan akurat. Metode yang digunakan untuk normalisasi pada proyek ini adalah menggunakan StandardScaler() dari pustaka scikit-learn. Berikut ini perintah yang digunakan untuk melakukan proses normalisasi.
```
numerical_features = ['Pclass', 'Age', 'SibSp', 'Parch', 'Fare']
scaler = StandardScaler()
scaler.fit(X_train[numerical_features])
X_train[numerical_features] = scaler.transform(X_train.loc[:, numerical_features])
```
6. Feature Selection
Data preparation tidak menggunakan teknik reduksi dimensi seperti Principal Component Analysis (PCA) karena setelah dilakukan analisis korelasi, setiap variabel tidak memiliki korelasi yang tinggi sehingga tidak perlu melakukan reduksi dimensi. 

Menjelaskan alasan mengapa diperlukan tahapan data preparation tersebut.

- Tujuan Penanganan Missing Value dan Noise
Meningkatkan Kualitas Data: Menangani nilai yang hilang dapat meningkatkan kualitas data, sehingga analisis atau model yang dibangun dapat menghasilkan output yang lebih akurat dan relevan.; Mengurangi Bias: Jika nilai yang hilang tidak ditangani dengan baik, analisis atau model dapat menghasilkan hasil yang bias karena hanya menggunakan data yang tersisa.; Mengoptimalkan Kinerja Model: Model machine learning sering kali tidak bisa menangani missing value secara langsung. Dengan menangani missing value terlebih dahulu, performa model dapat lebih optimal.
- Tujuan Utama Encoding Fitur
Membuat Data Kategorikal Dapat Digunakan dalam Model: Algoritma pembelajaran mesin seperti pohon keputusan, SVM, atau jaringan saraf tiruan memerlukan input numerik. Data kategorikal, seperti "laki-laki" dan "perempuan" atau "Embarked_S", "Embarked_Q", dan "Embarked_C" tidak dapat langsung digunakan oleh algoritma tersebut.; Meningkatkan Kinerja Model: Encoding fitur membantu meningkatkan akurasi dan efisiensi model dengan merepresentasikan informasi secara numerik. Tanpa encoding yang tepat, model dapat menghasilkan performa yang buruk atau tidak dapat belajar sama sekali.; Mengurangi Bias dalam Model: Teknik encoding tertentu dapat membantu mengurangi bias yang mungkin terjadi akibat penggunaan data kategorikal yang tidak diproses. Misalnya, jika satu kategori memiliki frekuensi lebih tinggi daripada yang lain, itu dapat mempengaruhi cara model membuat prediksi.; Memastikan Konsistensi dan Reproduksibilitas: Encoding fitur mengubah data menjadi format standar sehingga model dapat menghasilkan hasil yang konsisten setiap kali dijalankan.
- Tujuan Utama Over-Sampling
Menyeimbangkan Jumlah Sampel pada Setiap Kelas: Dengan menambah jumlah sampel pada kelas minoritas, over-sampling membantu menyeimbangkan distribusi kelas. Hal ini memungkinkan model untuk belajar dari kedua kelas secara lebih adil.; Meningkatkan Akurasi untuk Kelas Minoritas: Ketika dataset sangat tidak seimbang, model cenderung mengabaikan kelas minoritas dan lebih sering memprediksi kelas mayoritas. Dengan over-sampling, model dapat mempelajari karakteristik kelas minoritas dengan lebih baik, sehingga meningkatkan akurasi untuk kelas tersebut.; Mengurangi Bias dalam Model: Ketika dataset tidak seimbang, model pembelajaran mesin dapat cenderung memberikan prediksi yang bias terhadap kelas yang memiliki lebih banyak sampel. Over-sampling membantu mengurangi bias tersebut dengan menyediakan lebih banyak sampel dari kelas minoritas untuk dilatih oleh model.
- Tujuan dilakukan pemisahan data adalah 
Validasi Model: Untuk menilai seberapa baik model akan bekerja pada data baru yang tidak terlihat selama pelatihan.; Menghindari Overfitting: Dengan memisahkan data pelatihan dan pengujian, kita dapat memastikan bahwa model tidak hanya menghafal data pelatihan.; Evaluasi Model: Data pengujian digunakan untuk mengevaluasi metrik performa seperti akurasi, presisi, recall, atau F1-score.
- Tujuan Normalisasi Data dengan StandardScaler()
Menyamakan Skala Fitur: Dalam dataset, fitur bisa memiliki rentang nilai yang sangat berbeda. Misalnya, satu fitur bisa memiliki nilai dari 0 hingga 1000, sementara yang lain hanya dari 0 hingga 1. Model pembelajaran mesin yang sensitif terhadap skala (seperti regresi linier atau SVM) dapat terpengaruh oleh perbedaan ini.; Meningkatkan Kinerja Model: Model seperti gradient descent bekerja lebih efektif jika fitur memiliki rentang nilai yang serupa, karena langkah-langkah perhitungan gradien menjadi lebih konsisten.; Mempercepat Proses Pelatihan: Dengan skala yang seragam, model dapat mencapai konvergensi lebih cepat selama proses pelatihan.; Mengurangi Bias pada Fitur Tertentu: Fitur dengan skala yang lebih besar tidak akan mendominasi model dibandingkan fitur lainnya.

## Modeling
Pada kasus klasifikasi penumpang Titanic, tujuannya adalah memprediksi apakah penumpang akan selamat atau tidak berdasarkan beberapa fitur (misalnya usia, jenis kelamin, kelas tiket, dll.). Berikut adalah tahapan dan parameter utama dari tiga algoritma yang digunakan dalam pemodelan: Support Vector Machine (SVM), Random Forest, dan K-Nearest Neighbors (K-NN).

### 1. Support Vector Machine (SVM)
**Tahapan dan Penjelasan:**
- **a. Preprocessing Data:** Data perlu dinormalisasi atau di-standardisasi karena SVM sensitif terhadap skala fitur. Pada proyek ini menggunakan `StandardScaler()` agar semua fitur memiliki mean 0 dan standar deviasi 1.
- **b. Hyperparameter Tuning:** Ada beberapa parameter penting pada SVM:
  - `C` (regularization parameter): Mengontrol trade-off antara memperkecil kesalahan klasifikasi pada data pelatihan dan meningkatkan margin dari hyperplane yang memisahkan data. Nilai yang lebih kecil dari `C` akan menghasilkan margin yang lebih lebar, meskipun beberapa titik data bisa salah klasifikasi.
  - `kernel`: Menentukan jenis kernel yang digunakan untuk memetakan data ke ruang fitur yang lebih tinggi. Pilihan kernel yang umum adalah `'linear'`, `'poly'`, `'rbf'`, dan `'sigmoid'`. Misalnya, `'rbf'` sering digunakan untuk data yang tidak dapat dipisahkan secara linier.
  - `gamma`: Parameter kernel untuk kernel `'rbf'`, `'poly'`, dan `'sigmoid'`, yang mengontrol jarak pengaruh satu titik data. Nilai gamma yang besar menghasilkan model yang lebih kompleks, sedangkan nilai yang kecil membuat model lebih sederhana.
- **c. Pelatihan Model:** Setelah memilih parameter, model dilatih menggunakan data pelatihan.
- **d. Evaluasi Model:** Metrik seperti akurasi, precision, recall, dan F1-score digunakan untuk mengevaluasi kinerja model.

### 2. Random Forest
**Tahapan dan Penjelasan:**
- **a. Preprocessing Data:** Random Forest dapat bekerja dengan baik pada data yang tidak dinormalisasi, tetapi tetap perlu dilakukan preprocessing seperti menangani nilai yang hilang dan encoding fitur kategorikal.
- **b. Hyperparameter Tuning:** Parameter penting dalam Random Forest adalah:
  - `n_estimators`: Jumlah pohon dalam hutan. Semakin banyak pohon, semakin baik performa model, namun juga meningkatkan waktu komputasi.
  - `max_depth`: Kedalaman maksimum dari setiap pohon. Mengontrol kompleksitas pohon, dan membantu mencegah overfitting jika diatur ke nilai yang wajar.
  - `min_samples_split`: Jumlah minimum sampel yang diperlukan untuk membagi simpul internal. Nilai yang lebih besar membantu mencegah overfitting.
  - `criterion`: Ukuran untuk membagi node pohon, biasanya `'gini'` atau `'entropy'`.
- **c. Pelatihan Model:** Dilakukan dengan membangun beberapa pohon keputusan dan menggunakan hasil voting mayoritas untuk membuat prediksi.
- **d. Evaluasi Model:** Kinerja dievaluasi dengan cara yang sama seperti SVM, menggunakan metrik akurasi dan lainnya.

### 3. K-Nearest Neighbors (K-NN)
**Tahapan dan Penjelasan:**
- **a. Preprocessing Data:** Sangat penting untuk menormalisasi atau standarisasi data karena K-NN menggunakan jarak Euclidean untuk mengukur kedekatan antar titik. Data dengan skala yang berbeda akan mempengaruhi hasil perhitungan jarak.
- **b. Hyperparameter Tuning:** Parameter utama dalam K-NN adalah:
  - `n_neighbors`: Menentukan jumlah tetangga terdekat yang digunakan untuk melakukan klasifikasi. Memilih nilai yang terlalu kecil dapat menyebabkan overfitting, sedangkan nilai yang terlalu besar dapat membuat model kurang sensitif terhadap perbedaan data.
  - `weights`: Menentukan apakah semua tetangga memiliki kontribusi yang sama (`'uniform'`) atau kontribusi yang berbobot berdasarkan jarak (`'distance'`).
  - `metric`: Fungsi untuk mengukur jarak antara sampel. Default adalah jarak Euclidean, tetapi juga bisa menggunakan jarak Manhattan atau lainnya.
- **c. Pelatihan Model:** Model dilatih dengan menyimpan data pelatihan dan menggunakan algoritma pencarian tetangga terdekat untuk melakukan prediksi pada data baru.
- **d. Evaluasi Model:** Menggunakan metrik akurasi, precision, recall, dan F1-score untuk mengukur performa.

### Langkah-Langkah Umum dalam Pemodelan
1. **Membagi Dataset:** Data dibagi menjadi data pelatihan dan pengujian (misalnya, 80% pelatihan, 20% pengujian) menggunakan `train_test_split` untuk mengevaluasi performa model secara obyektif.
2. **Melakukan Preprocessing Data:** Meliputi penanganan nilai yang hilang, encoding fitur kategorikal, dan normalisasi jika diperlukan.
3. **Pelatihan Model:** Membangun model menggunakan data pelatihan dan menyimpan model untuk melakukan prediksi pada data pengujian.
4. **Evaluasi Kinerja Model:** Membandingkan hasil dari beberapa model untuk menentukan model terbaik berdasarkan berbagai metrik evaluasi.

Ketiga algoritma yang digunakan memiliki kekuatan yang berbeda-beda dan dapat memberikan hasil yang bervariasi tergantung pada karakteristik dataset Titanic yang digunakan. Evaluasi dan pemilihan model yang paling sesuai bergantung pada hasil analisis performa di atas berbagai metrik.

### Kelebihan dan Kekurangan Setiap Algoritma
Berikut adalah penjelasan kelebihan dan kekurangan dari masing-masing algoritma (Support Vector Machine, Random Forest, dan K-Nearest Neighbors), serta penjelasan tentang pemilihan model terbaik dan proses peningkatan performa model.
#### 1. Support Vector Machine (SVM)
**Kelebihan:**
- **Efektif untuk data dengan dimensi tinggi:** SVM dapat bekerja dengan baik pada dataset dengan banyak fitur, bahkan ketika jumlah sampel lebih sedikit daripada jumlah fitur.
- **Memiliki berbagai kernel yang fleksibel:** Kernel seperti `'linear'`, `'polynomial'`, dan `'rbf'` memungkinkan SVM untuk memetakan data ke ruang dimensi yang lebih tinggi untuk memisahkan kelas yang tidak dapat dipisahkan secara linier.
- **Mampu menghasilkan margin yang optimal:** Dengan memaksimalkan margin antara dua kelas, SVM membantu menghasilkan model yang lebih generalisasi.

**Kekurangan:**
- **Sensitif terhadap data dengan skala yang berbeda:** Data perlu distandardisasi atau dinormalisasi untuk hasil yang baik.
- **Kurang efisien pada dataset yang sangat besar:** SVM bisa menjadi lambat ketika jumlah sampel sangat besar karena membutuhkan komputasi yang intensif.
- **Pemilihan parameter yang tepat cukup rumit:** Memilih parameter seperti `C` dan `gamma` sangat penting untuk performa model dan memerlukan hyperparameter tuning.

#### 2. Random Forest
**Kelebihan:**
- **Mampu menangani data dengan missing values dan fitur kategorikal:** Algoritma ini dapat bekerja dengan baik meskipun ada nilai yang hilang dalam dataset.
- **Cegah overfitting secara alami:** Dengan menggabungkan prediksi dari banyak pohon, Random Forest menghasilkan model yang lebih stabil dan generalisasi lebih baik dibandingkan pohon keputusan tunggal.
- **Menyediakan estimasi pentingnya fitur:** Sangat berguna untuk memahami fitur mana yang paling mempengaruhi prediksi.

**Kekurangan:**
- **Cenderung lebih lambat pada prediksi real-time:** Karena banyaknya pohon yang perlu diproses, Random Forest dapat menjadi lebih lambat untuk digunakan dalam aplikasi dengan waktu respon cepat.
- **Kurang interpretatif dibandingkan model sederhana:** Meskipun estimasi pentingnya fitur tersedia, model Random Forest lebih sulit untuk diinterpretasi daripada pohon keputusan tunggal.

#### 3. K-Nearest Neighbors (K-NN)
**Kelebihan:**
- **Mudah diimplementasikan dan dipahami:** Algoritma K-NN sederhana karena tidak memerlukan model eksplisit yang dilatih.
- **Dapat menangani masalah klasifikasi non-linear:** Karena memprediksi berdasarkan tetangga terdekat, K-NN dapat memetakan keputusan yang kompleks.
- **Tidak ada asumsi khusus mengenai distribusi data:** Membuatnya cocok untuk data dengan distribusi yang tidak normal.

**Kekurangan:**
- **Membutuhkan normalisasi data:** Jarak antar titik data akan dipengaruhi oleh skala fitur jika tidak dinormalisasi.
- **Kurang efisien pada dataset yang sangat besar:** Karena membutuhkan pencarian tetangga untuk setiap prediksi, K-NN bisa lambat pada dataset besar.
- **Sensitif terhadap data yang tidak seimbang:** Jika jumlah sampel kelas tidak seimbang, hasil klasifikasi dapat terpengaruh.

### Pemilihan Model Terbaik dan Proses Improvement

Setelah menggunakan ketiga algoritma, langkah selanjutnya adalah memilih model terbaik berdasarkan kinerja pada metrik evaluasi (misalnya akurasi, precision, recall, F1-score) serta kompleksitas model. Berikut adalah langkah-langkah proses improvement dan pemilihan model terbaik:

#### Proses Improvement dengan Hyperparameter Tuning
Setelah memilih Random Forest sebagai model terbaik, langkah selanjutnya adalah melakukan peningkatan performa dengan **hyperparameter tuning**. Berikut adalah parameter yang bisa diatur dan langkah-langkah yang dilakukan:

1. **Support Vector Machine**
Diperoleh parameter terbaik seperti berikut ini.
```
svm = SVC(kernel='rbf', C=128, gamma=2048)
```

2. **Random forest**
Diperoleh parameter terbaik seperti pada kode berikut ini.
```
RF = RandomForestClassifier(class_weight='balanced', random_state=42)
```
3. **K-Nearest Neighbors**
Diperoleh parameter terbaik seperti pada kode berikut ini.
```
knn = KNeighborsClassifier(n_neighbors=3,          # Menggunakan 3 tetangga terdekat
    weights='distance',     # Memberikan bobot berdasarkan jarak (tetangga lebih dekat memiliki bobot lebih besar)
    algorithm='auto',       # Memilih algoritma secara otomatis berdasarkan data
    leaf_size=30,           # Ukuran daun untuk Ball Tree atau KD Tree
    p=1,                    # Menggunakan jarak Euclidean (p=2)
    metric='manhattan',     # Metrik jarak Minkowski
    n_jobs=-1     )
```

Dengan melakukan hyperparameter tuning, diharapkan kinerja model dapat lebih baik dalam memprediksi penumpang Titanic yang selamat atau tidak. Pemilihan algoritma yang tepat serta penyetelan parameter yang optimal adalah langkah penting dalam meningkatkan performa model klasifikasi.

#### Pemilihan Model Terbaik
Setelah melakukan evaluasi, hasil menunjukkan bahwa **Random Forest memberikan performa terbaik** di antara ketiga model. Alasan pemilihan Random Forest sebagai model terbaik karena:
- **Stabilitas dan generalisasi lebih baik:** Random Forest menggabungkan hasil dari banyak pohon, sehingga lebih tahan terhadap overfitting dibandingkan SVM dan K-NN.
- **Kemampuan menangani data yang tidak seimbang dengan lebih baik:** Random Forest memberikan prediksi berdasarkan agregasi hasil dari beberapa pohon, yang mengurangi bias terhadap kelas mayoritas.
- **Kinerja pada berbagai metrik yang lebih baik:** Random Forest dapat memberikan keseimbangan yang baik dengan akurasi skor train sebesar 0,98 dan akurasi skor test sebesar 0,90.

## Evaluation
Evaluasi model pada model klasifikasi sangat penting untuk menentukan seberapa baik model dapat memprediksi kelas dari data baru. Evaluasi ini menggunakan berbagai metrik untuk menilai performa model, yang mencakup kemampuan model dalam membedakan kelas positif dan negatif secara benar. Berikut adalah beberapa metrik yang digunakan pada proyek ini yaitu accuraacy score, precision score, recall score, dan f1-score. Berikut adalah penjelasan mengenai beberapa metrik evaluasi yang digunakan dalam proyek klasifikasi ini, serta bagaimana menginterpretasi hasilnya.

### Metrik Evaluasi yang Digunakan

#### 1. Akurasi
- **Definisi:** Akurasi adalah rasio jumlah prediksi yang benar terhadap total prediksi yang dilakukan. Akurasi menghitung persentase sampel yang diklasifikasikan dengan benar dari keseluruhan data. Akurasi sangat tepat untuk dataset yang seimbang, di mana jumlah sampel di setiap kelas hampir sama. Jika data tidak seimbang (misalnya, satu kelas jauh lebih banyak dari yang lain), akurasi bisa memberikan hasil yang menyesatkan.

#### 2. Precision
- **Definisi:** Precision adalah rasio jumlah prediksi positif yang benar terhadap total jumlah prediksi positif yang dilakukan. Precision menilai akurasi klasifikasi terhadap kelas positif. Precision penting ketika biaya kesalahan prediksi positif sangat tinggi, seperti dalam deteksi penipuan atau penyakit serius, di mana mengurangi *false positives* (prediksi positif yang salah) sangat penting.

#### 3. Recall
- **Definisi:** Recall adalah rasio jumlah prediksi positif yang benar terhadap total jumlah sampel positif yang sebenarnya. Recall mengukur seberapa baik model menangkap sampel positif yang sebenarnya ada. Recall penting ketika mengidentifikasi semua sampel positif sangat diutamakan. Misalnya, dalam sistem deteksi penyakit, semua kasus penyakit perlu dideteksi meskipun menghasilkan beberapa prediksi positif yang salah.

#### 4. F1 Score
- **Definisi:** F1 score adalah rata-rata harmonis dari precision dan recall. Ini memberikan keseimbangan antara precision dan recall, terutama jika keduanya perlu dioptimalkan sekaligus. F1 score berguna ketika dataset tidak seimbang dan kita ingin mengukur keseimbangan antara menghindari false positives dan false negatives. F1 score lebih informatif daripada akurasi dalam kasus seperti ini.

### Hasil Proyek Berdasarkan Metrik Evaluasi yang Digunakan

Setelah melakukan evaluasi terhadap model terbaik yaitu random forest klasifikasi penumpang Titanic, didapatkan hasil sebagai berikut:
![Classification Report](https://github.com/user-attachments/assets/72856f15-40d2-4f71-86c9-a8b01cd4fce0)
Diperoleh 
- **Akurasi:** 91%
- **Precision untuk Kelas "Selamat":** 85%
- **Recall untuk Kelas "Selamat":** 97%
- **F1 Score untuk Kelas "Selamat":** 91%

Penjelasan hasil berdasarkan metrik tersebut:
- **Akurasi 91%** menunjukkan bahwa model mengklasifikasikan 91% sampel dengan benar. Namun, mengingat akurasi bisa dipengaruhi oleh ketidakseimbangan kelas, kita juga perlu melihat precision dan recall.
- **Precision 85%** mengindikasikan bahwa 85% dari penumpang yang diprediksi "selamat" benar-benar selamat. Ini menunjukkan bahwa model cukup baik dalam menghindari false positives (penumpang yang tidak selamat tetapi diprediksi selamat).
- **Recall 97%** menunjukkan bahwa model berhasil mengidentifikasi 97% dari semua penumpang yang sebenarnya selamat. Model cukup baik, karena hanya ada peluang bahwa 3% penumpang yang seharusnya selamat tidak teridentifikasi oleh model (false negatives).
- **F1 Score 91%** memberikan gambaran menyeluruh tentang keseimbangan antara precision dan recall. Ini menunjukkan bahwa model memiliki kinerja yang seimbang dalam menangkap penumpang yang selamat sekaligus meminimalkan kesalahan prediksi.

Hasil tersebut mengindikasikan bahwa model memiliki performa yang baik dalam memprediksi penumpang yang selamat, dengan keseimbangan yang wajar antara ketepatan prediksi (precision) dan kemampuan mendeteksi sampel positif (recall). Jika perlu ditingkatkan, langkah selanjutnya dapat mencakup tuning hyperparameter atau mencoba algoritma lain untuk melihat apakah ada peningkatan performa.

### Penjelasan formula metrik dan bagaimana metrik tersebut bekerja 
Berikut adalah penjelasan formula untuk beberapa metrik evaluasi yang umum digunakan dalam klasifikasi, serta bagaimana masing-masing metrik bekerja dalam mengevaluasi model.

#### 1. Akurasi
- **Formula:**

$$\text{Akurasi} = \frac{\text{Jumlah Prediksi Benar}}{\text{Total Sampel}}$$

  atau dapat ditulis sebagai:

  $$\text{Akurasi} = \frac{\text{True Positives (TP)} + \text{True Negatives (TN)}}{\text{TP} + \text{TN} + \text{False Positives (FP)} + \text{False Negatives (FN)}}$$

- **Bagaimana Akurasi Bekerja:**
  Akurasi mengukur persentase sampel yang diklasifikasikan dengan benar dari total sampel. Ini memberikan gambaran keseluruhan tentang kinerja model, tetapi bisa menyesatkan jika kelas tidak seimbang (misalnya, ketika satu kelas lebih dominan daripada yang lain). Dalam kasus seperti itu, akurasi tinggi dapat dicapai dengan selalu memprediksi kelas mayoritas, meskipun model tidak benar-benar memahami pola dari kelas yang lebih sedikit.

#### 2. Precision
- **Formula:**

  $$\text{Precision} = \frac{\text{True Positives (TP)}}{\text{TP} + \text{False Positives (FP)}}$$

- **Bagaimana Precision Bekerja:**
  Precision mengukur ketepatan prediksi model dalam mengklasifikasikan sampel sebagai positif. Ini menunjukkan berapa persen prediksi positif yang benar-benar positif. Precision penting dalam situasi di mana kesalahan positif palsu (false positives) memiliki biaya yang tinggi. Misalnya, dalam deteksi penipuan, precision yang tinggi berarti kebanyakan transaksi yang terdeteksi sebagai penipuan benar-benar merupakan penipuan.

#### 3. Recall
- **Formula:**

  $$\text{Recall} = \frac{\text{True Positives (TP)}}{\text{TP} + \text{False Negatives (FN)}}$$

- **Bagaimana Recall Bekerja:**
  Recall mengukur sejauh mana model dapat menangkap semua sampel positif yang ada di data. Ini menunjukkan persentase sampel positif yang sebenarnya (true positives) yang berhasil ditemukan oleh model. Recall penting dalam kasus di mana kita ingin meminimalkan kesalahan negatif palsu (false negatives), seperti pada sistem deteksi penyakit di mana penting untuk mendeteksi semua kasus penyakit.

#### 4. F1 Score
- **Formula:**

  $$\text{F1 Score} = 2 \times \frac{\text{Precision} \times \text{Recall}}{\text{Precision} + \text{Recall}}$$

- **Bagaimana F1 Score Bekerja:**
  F1 score adalah rata-rata harmonis dari precision dan recall, sehingga memberikan keseimbangan antara keduanya. Ini lebih informatif dibandingkan akurasi ketika kita ingin mengoptimalkan precision dan recall secara bersamaan, terutama dalam kasus ketidakseimbangan kelas. F1 score rendah menunjukkan bahwa model tidak baik dalam menjaga keseimbangan antara menghindari false positives dan menangkap semua true positives.

### Kesimpulan
Berdasarkan analisis dan pengolahan yang dilakukan diperoleh kesimpulan sebagai berikut.
1. Berdasarkan variabel kategori dapat disimpulkan bahwa karakteristik orang yang memiliki kemungkinan lebih untuk hidup ketika terjadi kecelakaan kapal Titanic adalah perempuan dan yang berangkat dari pelabuhan Cherbourg. Sedangkan berdasarkan variabel numerik menunjukkan bahwa hubungan setiap variabel terhadap variabel survived menunjukkan hubungan yang tidak beraturan atau acak.
2. Berdasarkan heatmap yang menunjukkan nilai korelasi antar variabel menunjukkan bahwa setiap variabel memiliki korelasi yang rendah terhadap variabel survived. Namun, berdasarkan nilai korelasi tertinggi, dapat disimpulkan bahwa faktor yang paling berpengaruh terhadap kemungkinan lebih untuk hidup ketika terjadi kecelakaan kapal Titanic adalah tarif yang dikeluarkan oleh penumpang dengan korelasi terhadap variabel survived sebesar 0,27.
3. Model machine learning terbaik yang dapat memprediksi kemungkinan hidup seseorang berdasarkan karakteristik dan faktor yang ada menggunakan model random forest dengan melakukan hyperparameter tuning dengan tingkat akurasi sebesar 91%, precision untuk Kelas "Selamat" sebesar 85%, Recall untuk Kelas "Selamat" sebesar 97%, dan F1 Score untuk Kelas "Selamat" sebesar 91%.

Berdasarkan kesimpulan di atas, menunjukkan bahwa problem statement dapat diselesaikan dan semua goals atau tujuan dari proyek ini tercapai. Kemudian pengolahan dan analisis data sesuai dengan rencana pada solusi statement yaitu penggunaan algoritma machine learning lebih dari satu dapat memberikan opsi lebih banyak untuk mendapatkan model machine learning terbaik dengan tingkat akurasi yang tinggi. Selain itu, hyperparameter tuning juga dapat menghasilkan peningkatan tingkat akurasi atau nilai evaluasi lainnya yang lebih tinggi. Oleh karena itu, berdasarkan kesimpulan poin 3 menunjukkan bahwa akurasi yang dihasilkan dari model terbaik cukup memuaskan karena memiliki akurasi di atas 90%. Hal ini membuktikan bahwa solusi statement yang sudah direncanakan berjalan dengan baik.

## Referensi/Daftar Pustaka
[Will Cukierski. (2012). Titanic - Machine Learning from Disaster. Kaggle.](https://kaggle.com/competitions/titanic)
[Alexis Cook. (2022). Titanic Tutorial. Kaggle.](https://www.kaggle.com/code/alexisbcook/titanic-tutorial)
[Kakde,  Yogesh  & Agrawal, Shefali. (2018). Predicting Survival on Titanic by Applying Exploratory Data Analytics and Machine Learning Techniques. International Journal of Computer Applications (0975 – 8887) Volume 179 – No.44.
](https://www.researchgate.net/profile/Yogesh-Kakde/publication/325228831_Predicting_Survival_on_Titanic_by_Applying_Exploratory_Data_Analytics_and_Machine_Learning_Techniques/links/5c068f63a6fdcc315f9c0bb9/Predicting-Survival-on-Titanic-by-Applying-Exploratory-Data-Analytics-and-Machine-Learning-Techniques.pdf)
[Md Arfinul Haque etc. (2020). Passenger data analysis of Titanic using machine learning approach in the context of chances of surviving the disaster. IOP Conf. Series: Materials Science and Engineering 1065 (2021) 012042 IOP Publishing doi:10.1088/1757-899X/1065/1/012042.](https://iopscience.iop.org/article/10.1088/1757-899X/1065/1/012042/meta)
