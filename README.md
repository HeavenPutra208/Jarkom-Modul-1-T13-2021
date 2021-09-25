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
