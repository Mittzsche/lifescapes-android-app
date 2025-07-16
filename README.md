# 🧠 Lifescape - Aplikasi Manajemen Gaya Hidup Terpadu

Lifescape adalah aplikasi Android yang dirancang untuk membantu pengguna dalam mengelola tugas, mencatat ide, dan melacak kebiasaan secara efisien dalam satu platform. Aplikasi ini menggabungkan fitur manajemen produktivitas, catatan pribadi, autentikasi pengguna, dan visualisasi statistik tugas berbasis grafik. Dikembangkan menggunakan Java dan C (JNI), Lifescape mengutamakan performa, keamanan, dan pengalaman pengguna yang modern.

---

## 📲 Fitur Utama

### ✅ Manajemen Tugas (Todo List)
- Tambah, ubah, hapus tugas (CRUD)
- Penandaan prioritas (rendah, sedang, tinggi)
- Sorting dan filtering tugas
- Reminder dan tenggat waktu
- Swipe gesture (kanan: selesai, kiri: hapus)
- Searching berbasis Binary Search (C Native)

### 📝 Catatan Pribadi (Notes)
- Tambah dan edit catatan
- Dukungan tag (kategori)
- Sorting berdasarkan waktu/abjad
- Pencarian cepat dengan algoritma C
- Filter berdasarkan tag

### 📊 Statistik Progres
- Visualisasi jumlah tugas selesai vs belum
- Grafik batang, pie chart, dan line chart
- Progress bar mingguan

### 🔐 Autentikasi dan Keamanan
- Login/register/reset password dengan Firebase Authentication
- Sinkronisasi data ke RoomDB untuk offline access
- Validasi dan enkripsi data pengguna

---

## 🏗️ Struktur Proyek
app/
├── activity/              # Halaman utama aplikasi (Auth, Main, Splash)
├── adapter/               # RecyclerView Adapter (Todo, Notes)
├── database/
│   ├── dao/               # NotesDao, TodoDao, UserDao
│   ├── entity/            # Notes, Todo, User
│   └── AppDatabase.java
├── dialog/                # Dialog untuk tambah/edit/hapus
├── fragment/              # Fragment (Todo, Notes, Settings, Home)
├── utils/                 # NativeUtils (C), Auth manager, Notifikasi
├── cpp/                   # Algoritma C: Binary Search & Quick Sort
└── assets/                # File HTML: about.html, privacy.html, terms.html

---

## ⚙️ Teknologi yang Digunakan

* **Java**: Bahasa utama pengembangan Android
* **C (JNI)**: Untuk fungsi algoritma (sorting & searching)
* **RoomDB**: Database lokal untuk Notes & Todo
* **Firebase Auth**: Login, Register, Reset Password
* **MPAndroidChart**: Untuk grafik statistik
* **Glide**: Untuk load gambar (jika diaktifkan)
* **Material Components**: Tampilan modern dan responsif

---

## 🚧 Status Proyek

📘 Tahap: Penyelesaian dan Debugging
✅ Fitur utama telah berjalan dengan baik
🚀 Selanjutnya akan dideploy dan dipush ke GitHub dengan aplikasi Android (.apk)

---

## 🛠️ Rencana Pengembangan Selanjutnya

* Notifikasi berbasis tenggat waktu otomatis
* Ekspor laporan Todo/Notes ke PDF/Excel
* Sinkronisasi cloud penuh via Firebase/Firestore
* Dark Mode & Tema kustom
* Publikasi ke Play Store

---

## 👨‍💻 Kontributor

Kelompok 5 - Universitas Gunadarma

* Ahmad Fadhel Hafizhuddin
* Amanda Sabila
* Rafli Alfian Priyo Utomo
* Rizky Nurliansyah

---

## 📄 Lisensi

MIT License (Opsional — sesuaikan bila ada)

---

## 📌 Catatan

Aplikasi ini merupakan bagian dari tugas mata kuliah *Teknik Pemrograman Terstruktur 1* dan akan diunggah bersama dokumen makalah dan kode sumber secara lengkap setelah selesai tahap pengujian akhir.
