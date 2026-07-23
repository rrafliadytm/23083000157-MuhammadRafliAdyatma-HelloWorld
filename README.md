# Project Week 1: Hello World - Form Data Mahasiswa

Proyek ini adalah aplikasi Android sederhana yang dibuat menggunakan **Jetpack Compose** untuk memenuhi tugas mata kuliah Pemrograman Mobile. Aplikasi ini berfungsi untuk menginputkan data mahasiswa (Nama dan NIM) dengan validasi input dan tampilan hasil yang interaktif.

## Informasi Mahasiswa
- **Nama:** Muhammad Rafli Adyatma
- **NIM:** 23083000157
- **Kampus:** Universitas Merdeka Malang

---

## Snapshots Aplikasi

Berikut adalah tampilan dari setiap state layar pada aplikasi:

### 1. Tampilan Form Kosong
![Form Kosong](snapshots/1_form_kosong.png)
**Keterangan:**
Ini adalah tampilan awal saat aplikasi pertama kali dijalankan. Terdapat dua field input utama:
- **Nama Lengkap:** Menggunakan `OutlinedTextField` dengan icon person.
- **NIM:** Menggunakan `OutlinedTextField` dengan icon badge yang hanya menerima input angka.
- **Tombol Submit:** Masih dalam keadaan non-aktif (disabled) karena data belum diisi atau belum valid.

### 2. Pengisian Data & Validasi
![Form Terisi](snapshots/2_form_filled.png)
**Keterangan:**
Pada tahap ini, pengguna telah memasukkan data. 
- Sistem melakukan validasi secara real-time. NIM harus berupa angka dengan panjang antara 8 hingga 15 karakter.
- Setelah semua field terisi dengan benar, tombol **Submit Data** akan menjadi aktif (berubah warna).

### 3. Hasil Submit (Success State)
![Hasil Submit](snapshots/3_form_submitted.png)
**Keterangan:**
Setelah tombol submit ditekan, aplikasi akan menampilkan kartu hasil (Result Card) dengan animasi:
- Menampilkan pesan selamat datang khusus untuk mahasiswa tersebut.
- Menampilkan Nama dan NIM yang telah diinputkan.
- Terdapat tombol **Reset Form** untuk menghapus data dan kembali ke tampilan awal jika ingin menginputkan data baru.

---

## Teknologi yang Digunakan
- **Kotlin**: Bahasa pemrograman utama.
- **Jetpack Compose**: Toolkit modern untuk membangun UI Android secara deklaratif.
- **Material Design 3**: Standar desain UI terbaru dari Google untuk tampilan yang bersih dan modern.
- **State Management**: Menggunakan `remember` dan `mutableStateOf` untuk menangani perubahan UI secara reaktif.
