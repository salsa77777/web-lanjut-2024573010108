# Laporan Modul 1: Perkenalan Laravel
**Mata Kuliah:** Workshop Web Lanjut   
**Nama:** [SALSABILA]  
**NIM:** [2024573010108]  
**Kelas:** [TI 1 B]  

---

## Abstrak 
Laporan ini membahas pengenalan framework Laravel, salah satu framework PHP yang populer digunakan untuk membangun aplikasi web modern. Tujuan dari laporan ini adalah memahami dasar Laravel, fitur utamanya, serta bagaimana struktur proyek Laravel bekerja. Selain itu, laporan ini juga menjelaskan konsep MVC yang jadi dasar arsitektur Laravel, kelebihan serta tantangannya, dan contoh penggunaan praktis.

---

## 1. Pendahuluan
Laravel adalah framework PHP open-source yang dirilis oleh Taylor Otwell pada tahun 2011. Framework ini membantu developer membangun aplikasi web dengan lebih cepat, rapi, dan aman. Laravel menggunakan konsep MVC (Model-View-Controller), sehingga memisahkan logika aplikasi, tampilan, dan data dengan jelas.

Laravel disebut opinionated framework, artinya dia punya aturan dan konvensi tertentu yang sebaiknya diikuti. Konvensi ini bikin kode lebih konsisten dan memudahkan kerja tim. Laravel sangat cocok digunakan untuk berbagai jenis aplikasi, mulai dari blog sederhana sampai aplikasi besar seperti sistem perusahaan.

---

## 2. Komponen Utama Laravel 

**Blade (Templating)** Sistem template bawaan Laravel untuk mengelola tampilan dengan sintaks sederhana dan efisien.

**Eloquent (ORM)** Fitur untuk menghubungkan aplikasi dengan database menggunakan model berbasis objek.

**Routing** Menentukan URL dan aksi yang dijalankan, dapat berupa controller maupun closure.

**Controllers** Mengatur logika aplikasi dan menjadi penghubung antara model dan view.

**Migrations & Seeders** Mengelola struktur database (migrations) dan mengisi data awal (seeders).

**Artisan CLI** Command Line bawaan Laravel untuk menjalankan perintah otomatis seperti membuat controller, model, migrasi, dll.

**Testing (PHPUnit)** Mendukung pengujian otomatis untuk memastikan aplikasi berjalan sesuai harapan.

**Middleware** Mengatur lapisan pengolahan request, misalnya autentikasi atau filter akses.

---

## 3. penjelasan untuk setiap folder dan files yang ada didalam struktur sebuah project laravel.
Secara default, proyek Laravel punya struktur folder yang lumayan banyak. Berikut penjelasannya :

**app** Berisi kode utama aplikasi (model, controller, middleware).

**bootstrap** Menyimpan file yang menyiapkan aplikasi saat dijalankan, termasuk konfigurasi awal.

**config** Kumpulan file pengaturan aplikasi, misalnya database, email, session, dan lainnya.

**database** Berisi migration, seeder, dan factory untuk mengelola struktur database, menambahkan data awal, dan membuat data contoh.

**public** Folder yang bisa diakses user lewat browser. Biasanya ada index.php dan file aset (gambar, CSS, JS).

**resources** Tempat menyimpan file view (Blade), file bahasa, dan aset mentah (sebelum di-compile).

**routes** Folder untuk mendefinisikan semua rute URL, seperti web.php untuk web, api.php untuk API, dan console.php untuk perintah Artisan.

**storage** Menyimpan cache, log, dan file yang di-generate aplikasi.

**tests** Folder untuk menyimpan file pengujian otomatis agar aplikasi tetap stabil.

**vendor** Berisi semua library dan paket pihak ketiga yang diinstal melalui Composer.

---

## 4. Diagram MVC 
Laravel menggunakan arsitektur Model-View-Controller (MVC):

Model: Bagian yang mengatur interaksi dengan database.

View: Tampilan yang dilihat oleh user (misalnya HTML).

Controller: Penghubung antara model dan view, berisi logika aplikasi.

## Cara kerjanya:

- Route sebagai pintu masuk: menerima permintaan dari browser, lalu memutuskan controller mana yang akan dijalankan.

- Controller sebagai otak logika: mengatur alur, mengambil/olah data dari Model, dan meneruskan ke View.

- Model sebagai pengelola data: berinteraksi langsung dengan database (mengambil, menyimpan, memperbarui).

- View sebagai tampilan akhir: merender HTML (via Blade) dan menampilkan hasil ke user.

- Berikut diagram arsitektur MVC pada Laravel:

![Diagram MVC](gambar/diagram-mvc.png)

---

## 6. Kelebihan & Kekurangan 

* Kelebihan Laravel
Laravel dikenal memiliki dokumentasi yang sangat lengkap dan komunitas yang aktif. Hal ini membuat proses belajar maupun pengembangan aplikasi menjadi lebih mudah. Struktur kodenya berbasis Model-View-Controller (MVC) sehingga proyek dapat tersusun dengan rapi dan lebih teratur. Selain itu, Laravel sudah menyediakan banyak fitur bawaan seperti routing, autentikasi, Eloquent ORM, dan Blade templating yang dapat mempercepat proses pembuatan aplikasi. Dengan dukungan tersebut, Laravel dapat digunakan baik untuk aplikasi sederhana maupun proyek yang berskala besar.

* Kekurangan / Tantangan untuk Pemula
Untuk memanfaatkan Laravel secara optimal, dibutuhkan pemahaman dasar tentang konsep Object-Oriented Programming (OOP) serta PHP versi modern. Bagi pemula, struktur folder yang cukup kompleks bisa terasa membingungkan di awal. Selain itu, karena memiliki banyak fitur, Laravel umumnya membutuhkan sumber daya perangkat yang lebih besar dibanding framework PHP yang lebih ringan.

---

## 7. Referensi

Modul 1 — intoduction

Dokumentasi Resmi Laravel — https://laravel.com/docs

Petani Kode: Belajar Laravel — https://www.petanikode.com/laravel

W3Schools: PHP Frameworks — https://www.w3schools.com/php/php_frameworks.asp
