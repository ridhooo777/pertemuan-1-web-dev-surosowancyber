# Bio Link Project (Linktree Clone)

Projek ini adalah halaman tautan bio (bio link) sederhana mirip Linktree yang dibuat menggunakan **HTML5 semantik**, **CSS Modern**, dan **JavaScript dasar** untuk toggle Mode Gelap (Dark Mode). Projek ini didesain agar terlihat premium, responsif, dan siap di-deploy ke GitHub Pages.

## 🚀 Fitur Utama
- **Desain Premium & Glassmorphism**: Tampilan modern transparan dengan blur latar belakang yang memukau.
- **Dark Mode Toggle**: Fitur peralihan mode terang dan gelap dengan transisi halus dan ingatan mode terakhir (menggunakan `localStorage`).
- **Animasi Hover**: Transisi hover yang interaktif pada tombol tautan dan ikon media sosial.
- **Responsif**: Dioptimalkan untuk kenyamanan navigasi baik di desktop maupun perangkat mobile.
- **HTML5 Semantik**: Menggunakan struktur elemen yang baik seperti `<header>`, `<main>`, `<nav>`, `<section>`, dan `<footer>`.

---

## 🛠️ Cara Menjalankan Secara Lokal
Untuk melihat halaman di komputer Anda:
1. Klon repositori ini atau unduh folder projek.
2. Buka berkas `index.html` dengan mengklik dua kali, atau gunakan ekstensi editor seperti **Live Server** di VS Code untuk pengalaman development yang interaktif.

---

## 🌐 Cara Deploy ke GitHub Pages
GitHub Pages adalah layanan gratis dari GitHub untuk meng-hosting halaman statis secara langsung dari repositori Anda.

### Langkah-langkah Deployment:
1. **Buat Repositori Baru di GitHub**:
   - Masuk ke akun GitHub Anda.
   - Buat repositori baru dengan nama yang Anda sukai (misalnya: `bio-link`).
2. **Push Kode Anda ke GitHub**:
   - Inisialisasi git di folder lokal Anda jika belum:
     ```bash
     git init
     git add .
     git commit -m "Initial commit: bio link page"
     ```
   - Hubungkan repositori lokal Anda dengan GitHub lalu kirim (push) kodenya:
     ```bash
     git remote add origin https://github.com/username-anda/nama-repo.git
     git branch -M main
     git push -u origin main
     ```
3. **Aktifkan GitHub Pages**:
   - Di GitHub, buka halaman repositori Anda.
   - Klik tab **Settings** (Pengaturan).
   - Di menu sebelah kiri, cari bagian **Code and automation** lalu klik **Pages**.
   - Di bawah bagian **Build and deployment** -> **Source**, pilih **Deploy from a branch**.
   - Di bawah **Branch**, pilih **main** (atau branch utama Anda) dan pilih folder `/ (root)`.
   - Klik **Save**.
   - Tunggu 1–2 menit. Tautan URL aktif Anda akan muncul di bagian atas halaman pengaturan tersebut!

---

## 🏷️ Menggunakan Custom Domain di GitHub Pages
Jika Anda memiliki nama domain sendiri (seperti `ridho.dev` atau `ridho.my.id`), Anda bisa menghubungkannya ke halaman bio link ini.

### Cara Konfigurasi:
1. **Konfigurasi di GitHub**:
   - Buka kembali halaman **Settings** > **Pages** di repositori Anda.
   - Di bagian **Custom domain**, masukkan nama domain Anda (contoh: `bio.ridho.dev` atau `ridho.my.id`).
   - Klik **Save**. Ini akan otomatis membuat berkas bernama `CNAME` di dalam repositori Anda.
2. **Konfigurasi di Penyedia Domain (DNS Provider)**:
   - Masuk ke dasbor penyedia domain Anda (seperti Niagahoster, Domainesia, Cloudflare, dll.).
   - Masuk ke pengaturan DNS.
   - **Jika Anda menggunakan Subdomain (misal: `bio.domainanda.com`)**:
     - Tambahkan record **CNAME**:
       - **Host/Name**: `bio`
       - **Value/Target**: `username-anda.github.io`
       - **TTL**: Default (misal 3600)
   - **Jika Anda menggunakan Domain Utama (Apex Domain, misal: `domainanda.com`)**:
     - Tambahkan record **A** dengan mengarahkan Host `@` ke IP GitHub Pages berikut:
       - `185.199.108.153`
       - `185.199.109.153`
       - `185.199.110.153`
       - `185.199.111.153`
     - Tambahkan juga record **CNAME** untuk Host `www` yang mengarah ke `username-anda.github.io`.
3. **Aktifkan HTTPS**:
   - Setelah DNS terhubung (proses propagasi biasanya memakan waktu beberapa menit hingga beberapa jam), kembali ke **Settings** > **Pages** di GitHub.
   - Centang opsi **Enforce HTTPS** agar koneksi situs Anda aman.

---
Dibuat untuk tugas belajar HTML & CSS Dasar 🌟. Selamat belajar dan berkarya!
