# ProjectRDM2019

## Text-indexing : Swish-e (Package on Ubuntu)
### a. Requirements :
####Instal swish-e jika belum ada

$ sudo apt-get install swish-e

### b. Proses-proses dalam menjalankan Program :
1. buat folder Teks-indexing(Swish-e)
2. masuk ke dalam folder Teks-indexing(Swish-e)
$ cd Teks-indexing(Swish-e)
3. buat folder data
4. masuk ke dalam folder data
$ cd data
5. masukan file yang sudah di siapkan untuk di index ke dalam folder data
6. buat file Main.conf sebagai program utama yang akan di jalankan
7. di dalam file Main.conf isi dengan
$ IndexDir ./data
$ FuzzyIndexingMode Stemming_en1
$ IndexContents TXT* .txt
![](Screenshots/s4.PNG)
7. jalankan $ swish-e -c Main.conf 
![](Screenshots/s2.PNG)

8.barulah kemudian jalankan, misalnya kata yang akan di cari adalah Java $ swish-e -w [kata yang ingin di cari] 
![](Screenshots/s3.PNG)

## Image-search-engine
### a. Requirements :

$ sudo apt install python3-pip

![](Screenshots/1.PNG)

### b. Cara Menjalankan Program :
1.  $ cd ./image-search-engine
2.  $ pip install -r requirements.txt
![](Screenshots/3.PNG)
3.  $ cd ./app
4.  $ python index.py --dataset static/images --index index.csv 
![](Screenshots/4.PNG)
5. Untuk melihat output dapat dari index.cvs
![](Screenshots/5.PNG)
6. gambar dapat di ganti di folder ./static/images

## Source :
* Text-Indexing: Swish-e (Package on Ubuntu)
* Image-Indexing: https://github.com/kudeh/image-search-engine.
