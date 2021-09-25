# Jarkom-Modul-1-T13-2021

## Anggota Kelompok

| No. | Nama | NRP |
| ------ | ------ | ------ |
| 1. | Heaven Happyna Putra F. | (05311940000026) |
| 2. | Gavin Bagus Kenzie Narain | (05311940000028) |
| 3. | Tera Nurwahyu Pratama | (05311940000039) |

## Pembagian Tugas
Per anak membuat lapres 5 soal (Gavin 1-5, Tera 6-10, 11-15), namun pada pengerjaan soalnya bersamaan

## Daftar Isi
* [Soal 1](#soal-1)
* [Soal 2](#soal-2)
* [Soal 3](#soal-3)
* [Soal 4](#soal-4)
* [Soal 5](#soal-5)
* [Soal 6](#soal-6)
* [Soal 7](#soal-7)
* [Soal 8](#soal-8)
* [Soal 9](#soal-9)
* [Soal 10](#soal-10)
* [Soal 11](#soal-11)
* [Soal 12](#soal-12)
* [Soal 13](#soal-13)
* [Soal 14](#soal-14)
* [Soal 15](#soal-15)

## Soal 1
Sebutkan webserver yang digunakan pada "ichimarumaru.tech"! 
### Penyelesaian
Mengisi display filter: http.host contains "ichimarumaru.tech" lalu cek HTTP headernya
<br>
webservernya nginx/1.18.0 (Ubuntu)
<br>
![image](https://user-images.githubusercontent.com/73151823/134769759-63591806-260e-4996-8922-c14b0afc4c1e.png)
<br>

## Soal 2
Temukan paket dari web-web yang menggunakan basic authentication method!
### Penyelesaian
Mengisi display filter: http.authbasic
<br>
![image](https://user-images.githubusercontent.com/73151823/134769838-da2aa4e0-8a66-454c-b474-d3cd322fafe9.png)
<br>

## Soal 3
Ikuti perintah di basic.ichimarumaru.tech! Username dan password bisa didapatkan dari file .pcapng!
### Penyelesaian
Mengisi display filter http.host contains “ichimarumaru.tech”
<br>
![image](https://user-images.githubusercontent.com/73151823/134770004-d04fd1bf-90de-43c2-bd33-ba61b333b761.png)
<br>
Kemudian buka paket no 2066. Atau bisa cari menggunakan search string "credentials"
<br>
![image](https://user-images.githubusercontent.com/73151823/134770060-783b88f4-a2bf-4ced-b4d8-6b3b054c342a.png)
<br>
kuncimenujulautan: tQKEJFbgNGC1NCZlWAOjhyCOm6o3xEbPkJhTciZN gunakan kredensial tersebut untuk login di basic.ichimarumaru.tech dan isi konfigurasi kabel T568A
<br>
```hijau-putih, hijau, putih-orange, biru, putih-biru, orange, putih-coklat, coklat```
![image](https://user-images.githubusercontent.com/73151823/134770115-3012c00a-acb4-4103-9173-a6bc9474d0dd.png)
<br>

## Soal 6
Cari username dan password ketika melakukan login ke FTP Server menggunakan display filter ftp kemudian cari request USER dan PASS
### Penyelesaian
Mengisi Display Filter dengan **ftp**, sehingga USER dan PASS dapat ditemukan
<br>
<img width="600" src="https://github.com/HeavenPutra208/Jarkom-Modul-1-T13-2021/blob/main/img/6.1.png" />
<br>

## Soal 7
Ada 500 file zip yang disimpan ke FTP Server dengan nama 0.zip, 1.zip, 2.zip, ..., 499.zip. Simpan dan Buka file pdf tersebut. (Hint = nama pdf-nya "Real.pdf")
### Penyelesaian
Mengisi Display Filter dengan **frame contains "Real.pdf"**. Kemudian dioperoleh 2 zip sebagai berikut 
<br>
<img width="700" src="https://github.com/HeavenPutra208/Jarkom-Modul-1-T13-2021/blob/main/img/7.1.png" />
<br>

Setelah itu, klik kanan pada salah satu file dan pilih Follow -> TCP Stream. Ubah data dari ASCII ke Raw lalu save menjadi "Real.zip"
<br>
<img width="500" src="https://github.com/HeavenPutra208/Jarkom-Modul-1-T13-2021/blob/main/img/7.3.png" />
<br>

Setelah file "Real.zip" dibuka akan ada file "Real.pdf" yang berisi 
<br>
<img width="500" src="https://github.com/HeavenPutra208/Jarkom-Modul-1-T13-2021/blob/main/img/7.4.png" />
<br>

## Soal 8
Cari paket yang menunjukan pengambilan file dari FTP tersebut!
### Penyelesaian
Mengisi Display Filter dengan : **ftp.request.command==STOR**
<br>
<img width="500" src="https://github.com/HeavenPutra208/Jarkom-Modul-1-T13-2021/blob/main/img/8.png" />
<br>

## Soal 9 
Dari paket-paket yang menuju FTP terdapat indikasi penyimpanan beberapa file. Salah satunya adalah sebuah file berisi data rahasia dengan nama "secret.zip". Simpan dan buka file tersebut!
### Penyelesaian 
Dengan menggunakan Display Filter **ftp-data** maka akan ditemukan file bernama "secret.zip"
<br>
<img width="500" src="https://github.com/HeavenPutra208/Jarkom-Modul-1-T13-2021/blob/main/img/9.1.png" />
<br>

Setelah itu, klik kanan pada salah satu file dan pilih Follow -> TCP Stream. Ubah data dari ASCII menjadi Raw dan simpan menjadi "secret.zip"
<br>
<img width="500" src="https://github.com/HeavenPutra208/Jarkom-Modul-1-T13-2021/blob/main/img/9.png" />
<br>

Setelah file "secret.zip" dibuka, akan ada file "Wanted.pdf" yang tidak dapat dibuka karna memiliki password
<br>
<img width="500" src="https://github.com/HeavenPutra208/Jarkom-Modul-1-T13-2021/blob/main/img/9.2.png" />
<br>

## Soal 10
Selain itu terdapat "history.txt" yang kemungkinan berisi history bash server tersebut! Gunakan isi dari "history.txt" untuk menemukan password untuk membuka file rahasia yang ada di "secret.zip"!
### Penyelesaian
Mengisi Display Filter dengan **ftp-data** dan menemukan file "history.txt" yang berisi history bash
<br>
<img width="500" src="https://github.com/HeavenPutra208/Jarkom-Modul-1-T13-2021/blob/main/img/10.1.png" />
<br>

Setelah melihat isi history bash, terlihat bahwa password dari file "secret.zip" merupakan hasil dari tail -1 "bukanapaapa.txt". Sehingga, selanjutnya kami mencari file "bukanapaapa.txt" dengan menggunakan **ftp-data**
<br>
<img width="700" src="https://github.com/HeavenPutra208/Jarkom-Modul-1-T13-2021/blob/main/img/10.2.png" />
<br>

Setelah itu, klik kanan pada salah satu file dan pilih Follow -> TCP Stream. Lalu akan tampil data berbentuk ASCII
<br>
<img width="500" src="https://github.com/HeavenPutra208/Jarkom-Modul-1-T13-2021/blob/main/img/10.4.png" />
<br>

Terlihat dalam file "buknapaapa.txt" berisikan tulisan <em>d1b1langbukanapaapajugagapercaya</em>. Kemudian kami menggunakan tulisan tersebut untuk mengisi password "Wanted.pdf". Berikut adalah isi dari "Wanted.pdf"
<br>
<img width="500" src="https://github.com/HeavenPutra208/Jarkom-Modul-1-T13-2021/blob/main/img/9.3.png" />
<br>

## Soal 11
Filter sehingga wireshark hanya mengambil paket yang berasal dari port 80!
### Penyelesaian
Mengisi Capture Filter dengan : **src port 80**
<br>
<img width="500" src="https://github.com/HeavenPutra208/Jarkom-Modul-1-T13-2021/blob/main/img/11-1.jpg" />
<br>

Berikut hasil dari wireshark
<br>
<img width="500" src="https://github.com/HeavenPutra208/Jarkom-Modul-1-T13-2021/blob/main/img/11-2.jpg" />
<br>

## Soal 12
Filter sehingga wireshark hanya mengambil paket yang mengandung port 21!
### Penyelesaian
Pertama, nyalakan wireshark dengan capture filter port 21, pilih adapter for loopback traffic
<br>
<img width="500" src="https://github.com/HeavenPutra208/Jarkom-Modul-1-T13-2021/blob/main/img/12-1.jpg" />
<br>

Kemudian nyalakan aplikasi Xampp sekaligus aplikasi Filezilla
<br>
<img width="500" src="https://github.com/HeavenPutra208/Jarkom-Modul-1-T13-2021/blob/main/img/12-2.jpg" />
<br>

Kemudian dengan Filezilla client, lakukan ftp dengan kredensial yang sudah dibuat
<br>
<img width="500" src="https://github.com/HeavenPutra208/Jarkom-Modul-1-T13-2021/blob/main/img/12-3.jpg" />
<br>

Drag file dari remote site ke local site. jika berhasil, nanti muncul di wireshark
<br>
<img wdith="500" src="https://github.com/HeavenPutra208/Jarkom-Modul-1-T13-2021/blob/main/img/12-4.jpg" />
<br>

Berikut merupakan tampilan di wireshark dengan capture filter port 21
<br>
<img width="500" src="https://github.com/HeavenPutra208/Jarkom-Modul-1-T13-2021/blob/main/img/12-5.jpg" />
<br>

## Soal 13
Filter sehingga wireshark hanya menampilkan paket yang menuju port 443!
### Penyelesaian
Mengisi Capture Filter dengan `dst port 443`
<br>
<img width="500" src="https://github.com/HeavenPutra208/Jarkom-Modul-1-T13-2021/blob/main/img/13-1.jpg" />
<br>

Setelah itu, akan menampilkan paket yang menuju port 443.
<br>
<img width="500" src="https://github.com/HeavenPutra208/Jarkom-Modul-1-T13-2021/blob/main/img/13-2.jpg" />
<br>

## Soal 14
Filter sehingga wireshark hanya mengambil paket yang tujuannya ke kemenag.go.id!
### Penyelesaian
Mengisi Capture Filter dengan `host kemenag.go.id` menggunakan loopback traffic
<br>
<img width="500" src="https://github.com/HeavenPutra208/Jarkom-Modul-1-T13-2021/blob/main/img/14-1.jpg" />
<br>

Setelah itu wireshark akan menampilkan pengambilan hasil pake yang menuju ke kemenag.go.id
<br>
<img width="500" src="https://github.com/HeavenPutra208/Jarkom-Modul-1-T13-2021/blob/main/img/14-2.jpg" />
<br>

## Soal 15
Filter sehingga wireshark hanya mengambil paket yang berasal dari ip kalian!
### Penyelesaian
Mengisi capture filter dengan `src host 192.168.0.29`
<br>
<img width="500" src="https://github.com/HeavenPutra208/Jarkom-Modul-1-T13-2021/blob/main/img/15-1.jpg" />
<br>

Setelah itu, wireshark akan memunculkan paket yang berasal dari ip tersebut
<br>
<img width="500" src="https://github.com/HeavenPutra208/Jarkom-Modul-1-T13-2021/blob/main/img/15-2.jpg" />
<br>

## Kendala yang Dialami
Tidak ada
