# 💍 Undangan Pernikahan Digital (Habib & Sofia)

Website undangan pernikahan digital modern, elegan, responsif, dan sangat ringan yang dibuat menggunakan **HTML5, Tailwind CSS, dan JavaScript murni**. Siap untuk di-*deploy* langsung secara gratis ke **GitHub Pages**.

---

## ✨ Fitur-Fitur Utama

1. **Cover "Buka Undangan" (Welcome Screen)**
   - Menampilkan nama mempelai: **Habib & Sofia**.
   - Animasi buka cover halus ke atas.
   - Mengunci scroll halaman sampai tamu menekan tombol *Buka Undangan*.
   - Otomatis memutar audio instrumen romantis saat cover dibuka.
2. **Nama Tamu Undangan Dinamis**
   - Mendukung pembacaan parameter URL: `?to=Nama%20Tamu`.
   - Contoh: `https://username.github.io/undangan/?to=Bapak%20Budi%20Santoso`.
   - Nama otomatis terisi juga di input formulir ucapan.
3. **Kontrol Musik Melayang (Floating Audio Controller)**
   - Tombol piringan hitam (*vinyl rotating*) melayang di kanan atas.
   - Bisa *play/pause* audio kapan saja.
4. **Bottom Dock Navigation**
   - Navigasi cepat ala aplikasi mobile (*Home, Mempelai, Acara, Galeri, Hadiah, Ucapan*).
5. **Countdown Timer Interaktif**
   - Menghitung mundur (Hari, Jam, Menit, Detik) menuju hari H secara *real-time*.
6. **Rangkaian Acara & Integrasi Kalender/Peta**
   - Akad Nikah & Resepsi Pernikahan.
   - Tombol langsung ke **Google Maps**.
   - Tombol **Simpan ke Google Calendar**.
7. **Galeri Foto Prewedding & Lightbox**
   - Grid galeri foto estetik.
   - Klik foto untuk memperbesar (*pop-up lightbox fullscreen*).
8. **Amplop Digital / Hadiah (Wedding Gift)**
   - Rekening BCA (a.n Muhammad Habib) & Rekening Mandiri (a.n Sofia Azzahra).
   - Alamat pengiriman kado fisik.
   - Tombol **Salin Nomor Rekening / Alamat** dengan notifikasi *toast* "Berhasil Disalin!".
9. **Buku Tamu & RSVP (Ucapan & Konfirmasi Kehadiran)**
   - **Tanpa database server**: Menggunakan `localStorage` browser sehingga tamu bisa langsung kirim doa/ucapan dan langsung muncul di daftar secara interaktif.
   - Disertai badge kehadiran (*Hadir, Masih Ragu, Tidak Hadir*).
10. **Animasi Halus (AOS - Animate On Scroll)**
    - Teks, foto, dan kartu acara muncul bertahap saat di-scroll ke bawah.

---

## 🚀 Cara Menjalankan di Komputer Lokal

1. Cukup buka file [index.html](file:///d:/Penyimpanan%20Utama/Documents/html/undangan/index.html) langsung di browser (Chrome, Edge, Firefox, dll).
2. Untuk menguji nama tamu tertentu, tambahkan query di akhir alamat file browser:
   ```text
   file:///D:/Penyimpanan%20Utama/Documents/html/undangan/index.html?to=Bapak%20Joko%20Susilo
   ```

---

## 🌐 Cara Deploy ke GitHub Pages (Gratis & 1 Menit)

1. Buat repositori baru di akun GitHub Anda (misal: `undangan-habib-sofia`).
2. Masukkan dan upload file `index.html` dan `README.md` ke repositori tersebut:
   ```bash
   git init
   git add .
   git commit -m "feat: initial wedding invitation website"
   git branch -M main
   git remote add origin https://github.com/USERNAME/undangan-habib-sofia.git
   git push -u origin main
   ```
3. Buka tab **Settings** di repositori GitHub Anda.
4. Pilih menu **Pages** di sebelah kiri (di bawah *Code and automation*).
5. Pada bagian **Build and deployment**:
   - **Source**: `Deploy from a branch`
   - **Branch**: Pilih `main` dan folder `/ (root)`
   - Klik **Save**.
6. Tunggu 1–2 menit, website undangan Anda sudah online di:
   ```text
   https://USERNAME.github.io/undangan-habib-sofia/?to=Nama%20Tamu
   ```

---

## 🎨 Cara Kustomisasi Data Sendiri

Buka [index.html](file:///d:/Penyimpanan%20Utama/Documents/html/undangan/index.html) di teks editor (VS Code, Notepad, dll):

| Bagian | Lokasi di `index.html` |
| :--- | :--- |
| **Nama Pengantin** | Cari kata `Habib & Sofia` dan sesuaikan. |
| **Tanggal Acara** | Cari `27 NOVEMBER 2026` & ubah variabel `targetDate` di script JS. |
| **Nomor Rekening** | Cari tag id `rek-bca` dan `rek-mandiri` di bagian `#hadiah`. |
| **Foto-foto** | Ganti URL gambar Unsplash dengan link foto Anda sendiri atau foto lokal di folder project. |
| **Lagu Latar** | Ganti atribut `src` pada tag `<audio id="bg-audio">` dengan link MP3 pilihan Anda. |
