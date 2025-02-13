# Al-Qur'an Web App

Proyek ini adalah aplikasi web sederhana yang menampilkan Al-Qur'an dengan fitur detail surah dan bookmark. Data Al-Qur'an diperoleh dari API [equran.id](https://equran.id/apidev/v2). Source code ini tersedia secara gratis untuk digunakan dan dikembangkan lebih lanjut.

## 📌 Fitur

- Menampilkan daftar surah
- Detail surah
- Bookmark ayat

## 📥 Instalasi dan Penggunaan

### 1. Download atau Clone Repository

Silakan download atau clone repository ini ke dalam komputer Anda.

```sh
# Clone repository
git clone https://github.com/username/alquran-web.git

# Masuk ke folder proyek
cd alquran-web
```

### 2. Struktur File

Pastikan file berikut ada dalam proyek Anda:

```
/
|-- alquran.html          # Halaman utama daftar surah
|-- surah-detail.html     # Halaman detail surah
|-- bookmark.html         # Halaman bookmark
```

### 3. Menjalankan Proyek Secara Lokal

Anda bisa langsung membuka file `alquran.html` dengan browser favorit Anda karena ini adalah proyek berbasis HTML, CSS, dan JavaScript.

## 🚀 Hosting Website

Agar website ini dapat diakses secara online, Anda perlu mengunggahnya ke hosting. Berikut adalah langkah-langkahnya:

### 1. Menyewa Hosting dan Domain

Jika Anda belum memiliki hosting dan domain, Anda bisa menyewanya melalui:

- [IDCloudHost](https://my.idcloudhost.com/aff.php?aff=8496) (Rekomendasi)

### 2. Upload File ke Hosting

1. **Login ke cPanel** hosting Anda.
2. **Buka File Manager** dan masuk ke direktori `public_html`.
3. **Upload semua file** (`alquran.html`, `surah-detail.html`, `bookmark.html`).
4. Jika semua file sudah diunggah, akses website Anda melalui domain yang telah disewa.

## 🔗 Koneksi Antar File

Pastikan setiap file saling terhubung dengan benar menggunakan path yang sesuai:

```html
<!-- Contoh Link dari alquran.html ke surah-detail.html -->
<a href="surah-detail?id=1">Buka Surah Al-Fatihah</a>

<!-- Contoh Link dari surah-detail.html ke bookmark.html -->
<a href="bookmark">Lihat Bookmark</a>
```

⚠ **Catatan:**

- Beberapa server hosting mengizinkan akses ke file HTML tanpa menuliskan ekstensi `.html`. Jika link tanpa `.html` tidak berfungsi, gunakan format lengkap seperti:
  ```html
  <a href="bookmark.html">Lihat Bookmark</a>
  ```
- Jika Anda ingin memastikan file dapat diakses tanpa `.html`, Anda bisa menambahkan aturan `.htaccess` pada hosting berbasis Apache:
  ```apache
  RewriteEngine On
  RewriteCond %{REQUEST_FILENAME}.html -f
  RewriteRule ^([^/]+)/?$ $1.html [L]
  ```

## 📢 Sumber Data

Data Al-Qur'an yang digunakan dalam proyek ini diambil dari API [equran.id](https://equran.id/apidev/v2).

## 📌 Kontribusi

Silakan kontribusi dengan melakukan fork repository ini atau mengajukan pull request.

## 📧 Kontak

Jika ada pertanyaan atau masalah terkait proyek ini, silakan hubungi saya melalui email, repository GitHub, atau Telegram:
- 📬 Telegram: [@kangujang08](https://t.me/kangujang08)

---

🚀 **Jangan lupa untuk memberi ⭐ di repository ini jika bermanfaat!**

