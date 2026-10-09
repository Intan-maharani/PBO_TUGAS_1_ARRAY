# 🏦 Simple Banking System - Java

## 📌 Deskripsi Proyek

**Simple Banking System** adalah program simulasi perbankan sederhana yang dibuat menggunakan bahasa pemrograman Java. Program ini menerapkan konsep *Object-Oriented Programming* (OOP) untuk mengelola data nasabah, rekening, serta transaksi perbankan seperti penyetoran dan penarikan saldo.

Program ini juga memiliki validasi transaksi untuk mencegah setoran atau penarikan dengan nominal nol maupun negatif, serta memastikan saldo rekening tidak kurang dari saldo minimum yang telah ditentukan.

## ✨ Fitur Utama

* **Manajemen Nasabah:** Menyimpan nama depan dan nama belakang nasabah.
* **Manajemen Rekening:** Membuat rekening dan menyimpan saldo nasabah.
* **Deposit:** Menambahkan saldo dengan nominal positif.
* **Withdraw:** Melakukan penarikan saldo dengan nominal positif.
* **Validasi Transaksi:** Menolak transaksi dengan nominal nol atau negatif.
* **Saldo Minimum:** Mempertahankan saldo minimum sebesar Rp100.000 setelah penarikan.
* **Multiple Accounts:** Mendukung penyimpanan beberapa rekening dalam satu objek nasabah menggunakan `ArrayList`.
* **Simulasi Transaksi:** Menguji transaksi yang berhasil maupun yang ditolak.

## 🛠️ Teknologi yang Digunakan

* **Bahasa Pemrograman:** Java
* **Konsep:** Object-Oriented Programming (OOP)
* **Struktur Data:** `ArrayList`
* **Input/Output:** `System.out.println()` dan `System.out.print()`

## 📂 Struktur File

```text
Simple-Banking-System/
├── Account.java
├── Customer.java
├── BankDemo.java
└── README.md
```

### Penjelasan File

| File            | Deskripsi                                                                          |
| --------------- | ---------------------------------------------------------------------------------- |
| `Account.java`  | Mengelola saldo rekening, setoran, penarikan, dan validasi saldo minimum.          |
| `Customer.java` | Menyimpan informasi nasabah dan mengelola daftar rekening menggunakan `ArrayList`. |
| `BankDemo.java` | Berisi metode `main()` untuk menjalankan program dan menguji simulasi transaksi.   |

## ⚙️ Aturan Program

1. Saldo awal rekening minimal **Rp100.000**.
2. Setoran harus memiliki nominal lebih dari nol.
3. Penarikan harus memiliki nominal lebih dari nol.
4. Penarikan hanya berhasil jika saldo setelah transaksi tetap minimal Rp100.000.
5. Jika transaksi tidak memenuhi ketentuan, program menampilkan pesan kegagalan dan saldo tidak berubah.

## 🚀 Cara Menjalankan Program

### 1. Pastikan Java Terinstal

Periksa instalasi Java melalui terminal atau Command Prompt:

```bash
java -version
javac -version
```

### 2. Clone Repository

Ganti `USERNAME` dan `NAMA-REPOSITORY` sesuai informasi repository GitHub milikmu.

```bash
git clone https://github.com/USERNAME/NAMA-REPOSITORY.git
```

### 3. Masuk ke Folder Proyek

```bash
cd NAMA-REPOSITORY
```

### 4. Compile Program

Kompilasi seluruh file Java:

```bash
javac Account.java Customer.java BankDemo.java
```

### 5. Jalankan Program

```bash
java BankDemo
```

## 🧪 Skenario Pengujian

Program menguji beberapa skenario transaksi berikut:

| No. | Skenario                                     |     Nominal | Hasil yang Diharapkan                                  |
| --- | -------------------------------------------- | ----------: | ------------------------------------------------------ |
| 1   | Membuat rekening pertama                     |   Rp500.000 | Rekening berhasil dibuat                               |
| 2   | Deposit dengan nominal negatif               |   -Rp50.000 | Transaksi ditolak                                      |
| 3   | Withdraw dengan nominal negatif              |  -Rp100.000 | Transaksi ditolak                                      |
| 4   | Deposit dengan nominal valid                 |   Rp200.000 | Transaksi berhasil                                     |
| 5   | Withdraw melebihi batas saldo yang diizinkan |   Rp650.000 | Transaksi ditolak karena saldo minimum tidak terpenuhi |
| 6   | Membuat rekening nasabah kedua               | Rp1.200.000 | Rekening kedua dibuat dengan saldo awal sesuai nominal |

### Contoh Perubahan Saldo Nasabah Pertama

Dengan saldo awal Rp500.000:

* Deposit -Rp50.000 → ditolak, saldo tetap Rp500.000.
* Withdraw -Rp100.000 → ditolak, saldo tetap Rp500.000.
* Deposit Rp200.000 → berhasil, saldo menjadi Rp700.000.
* Withdraw Rp650.000 → ditolak karena sisa saldo Rp50.000, di bawah batas minimum Rp100.000.

**Saldo akhir yang diharapkan: Rp700.000.**

## 📚 Konsep Pemrograman yang Dipelajari

Melalui proyek ini, beberapa konsep dasar Java dipraktikkan:

* **Class dan Object:** Membuat objek `Account` dan `Customer`.
* **Encapsulation:** Menggunakan atribut `private` dan metode untuk mengakses atau memodifikasi data.
* **Constructor:** Menginisialisasi objek nasabah dan rekening.
* **Method:** Memisahkan fungsi pengelolaan rekening dan transaksi.
* **ArrayList:** Menyimpan daftar rekening milik nasabah.
* **Conditional Statements:** Menggunakan `if-else` untuk memvalidasi transaksi.
* **Boolean Return Value:** Menggunakan nilai `true` atau `false` untuk menunjukkan keberhasilan transaksi.

## 🎯 Tujuan Proyek

Proyek ini bertujuan untuk memahami penerapan konsep OOP dalam Java melalui simulasi sistem perbankan sederhana, sekaligus mempelajari pengelolaan objek, validasi data, struktur data, dan penanganan transaksi.

## 👨‍💻 Author

**Nama:** [ANAK AGUNG AYU INTAN PUTRI MAHARANI]
**Kelas:** [B]
**NIM:** [F1D02510037]

---


