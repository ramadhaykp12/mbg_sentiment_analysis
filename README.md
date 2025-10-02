# Analisis Sentimen Program MBG (Makan Bergizi Gratis)

## Background & Objective
Program Makanan Bergizi Gratis atau biasa disebut MBG, merupakan program utama dari pemerintahan Presiden
Prabowo Subianto yang sudah berjalan sejak Januari 2025. Program ini untuk menyediakan makan siang gratis 
yang ditargetkan khusus untuk siswa-siswi PAUD hingga SMA serta Ibu hamil dan menyusui. 
Seiring berjalannya program MBG, tentu memunculkan berbagai opini dari masyarakat terhadap 
program ini. X (Twitter) menjadi salah satu wadah bagi publik dalam menyampaikan pendapat dan 
aspirasinya secara langsung termasuk tentang program MBG yang dijalankan oleh pemerintah.
Dengan memanfaatkan NLP dan teknik analisis sentimen, kita dapat mengetahui bagaimana persepsi 
publik apakah dominan sentimen positif, negatif atau bahkan netral. Dan apakah ada pola tertentu 
dalam reaksi masyarakat.

## Data Collection
Data merupakan tweet dari platform sosial media X (Twitter) yang diambil menggunakan metode data crawling.
Data yang diambil merupakan tweet dari rentang tanggal 27 September 2025 - 30 September 2025.

## Data Labeling
Pelabelan data dilakukan menggunakan model open source dari HuggingFace. Adapun model yang digunakan
adalah w11wo/indonesian-roberta-base-sentiment-classifier yang merupakan model Indonesian RoBERTa Base 
yang telah fine-tuned dengan dataset SMSA indonlu. Model ini merupakan model open-sourse dari HuggingFace.

## Exploratory Data Analysis
### Sentiment Label Percentage
![image](https://github.com/ramadhaykp12/mbg_sentiment_analysis/blob/main/charts/percentage_mbg.png)

Berdasarkan pie chart diatas, label sentimen negatif adalah yang paling banyak mencapai 59%, lalu sentimen
netral sebesar 28.8% dan yang terendah adalah label positif yaitu 12.2%.

### Wordcloud: Negative Sentiment
![image](https://github.com/ramadhaykp12/mbg_sentiment_analysis/blob/main/charts/wordcloud_negatif_mbg.png)

Pada gambar diatas merupakan wordcloud dari data berlabel sentimen negatif. Ukuran pada teks merupakan
volume atau frekuensi banyaknya kata tersebut digunakan pada tweet berlabel negatif.

### Wordcloud: Positive Sentiment
![image](https://github.com/ramadhaykp12/mbg_sentiment_analysis/blob/main/charts/wordcloud_positif_mbg.png)

Pada gambar diatas merupakan wordcloud dari data berlabel sentimen positif. Ukuran pada teks merupakan
volume atau frekuensi banyaknya kata tersebut digunakan pada tweet berlabel positif.

### Negative Label Word Frequency
![image](https://github.com/ramadhaykp12/mbg_sentiment_analysis/blob/main/charts/word_neg_freq.png)

Berdasarkan barplot diatas, kata mbg merupakan kata dengan frekuensi tertinggi disusul dengan kata keracunan

### Positive Label Word Frequency
![image](https://github.com/ramadhaykp12/mbg_sentiment_analysis/blob/main/charts/word_pos_freq.png)

Berdasarkan barplot disamping, kata mbg merupakan kata dengan frekuensi tertinggi disusul dengan kata makan









