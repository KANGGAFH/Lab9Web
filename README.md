# PRAKTIKUM 9
- **Nama**    : Kangga Fajarulhakim
- **Kelas**   : TI.23.A.4
- **NIM**     : 312310430
- **Mata Kuliah**: Pemprograman Web 1

**Modularasasi Menggunakan Require**

Modularisasi menggunakan require adalah teknik dalam pemrograman PHP yang digunakan untuk menggabungkan skrip PHP atau teks dari file lain dengan skrip PHP yang memanggilnya.
Jenis modularisasi di dalam php antara lain ; require() digunakan ketika file yang disertakan sangat penting untuk kelangsungan program, include() digunakan jika file tidak kritis untuk kelangsungan program, require_once() digunakan untuk mencegah penyertaan file yang sama lebih dari sekali (menghindari error seperti deklarasi ulang fungsi atau variabel), include_once() digunakan untuk mencegah penyertaan file yang sama lebih dari sekali, seperti require_once, tetapi tidak menghentikan eksekusi jika file tidak ditemukan.
<br>
*Pada praktikum ini adalah hasil pengimplementasian dari modul praktikum 8.* <br>
<br>
![Screenshot_5](https://github.com/user-attachments/assets/e3851af2-8cf8-419e-ab8d-7ec00472e81b)<br>
diatas ini adalah table *data_barang* dari database yang telah dibuat. <br>
![Screenshot_1](https://github.com/user-attachments/assets/961dd9d6-f816-40d5-89db-f4c99d3f7b6e)<br>
dan diatas ini adalah isi data/value dari table *data_barang*<br>
<br>
**Berikut adalah screenshot beserta penjelasan dari kode yang telah dibuat**
<br>

![Screenshot_6](https://github.com/user-attachments/assets/855587ef-92ed-4c44-a505-f99c0de515a5)<br>
terdapat tulisan *Koneksi Berhasil!* yang berarti program berhasil membuat koneksi ke database menggunakan mysqli_connect(). (*kode dapat dilihat pada koneksi.php*) <br>

![Screenshot_2](https://github.com/user-attachments/assets/1e3775c2-40b8-44d0-9801-a307bd06369b)<br>
pada halaman home ini kita menggunakan fungsi require() untuk memanggil *header.php* yang akan menampilkan bagian header halaman, *tambah.php* akan menampilkan form untuk menambah data, *footer.php* untuk menampilkan bagian footer halaman. (*kode bisa dilihat pada home.php, header.php, tambah.php, footer.php*) <br>

![Screenshot_3](https://github.com/user-attachments/assets/ca0c0797-9676-4955-afb6-d3e4c6d36c71)<br>
pada kode PHP ini kita dapat mengubah data barang dalam sebuah database, termasuk gambar, melalui HTML. pada kode *error_reporting(E_ALL)*, digunakan untuk Mengaktifkan pelaporan semua jenis kesalahan PHP, termasuk peringatan dan notifikasi, yang sangat berguna selama pengembangan. *include_once 'koneksi.php';* akan menyertakan file koneksi.php, yang berisi kode untuk koneksi ke database. pada Query SQL dibuat untuk memperbarui data barang berdasarkan id_barang yang diterima dari form. (*kode dapat dilihat pada ubah.php*) <br>

![Screenshot_4](https://github.com/user-attachments/assets/28f12041-83e3-4373-bb06-1a7d1c4b3a48)<br>
pada halaman kontak ini kita menggunakan *require('header.php');* dan *require('footer.php');* untuk menampilkan header dan footer yang telah kita buat, untuk selebihnya kita membuat form kontak dan informasi kontak seperti biasa. (*kode dapat dilihat pada kontak.php*)




