# YobaseHub

### Personal Profile & Linktree Website

Website profil modern milik **Yoganugroho** yang menggabungkan profil pribadi, media sosial, dan berbagai channel resmi dalam satu halaman.

**Live Website:**
https://yobasehub.net

[![Website](https://img.shields.io/badge/Website-yobasehub.net-2563eb?style=for-the-badge)](https://yobasehub.net)
[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge\&logo=html5\&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge\&logo=css3\&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge\&logo=javascript\&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Vercel](https://img.shields.io/badge/Vercel-000000?style=for-the-badge\&logo=vercel\&logoColor=white)](https://vercel.com)

---

## Tentang

YobaseHub adalah halaman profil dan linktree yang dibuat untuk menampilkan identitas digital Yoganugroho sekaligus menyediakan akses cepat menuju berbagai channel dan layanan.

Website menggunakan desain biru dan putih modern, responsive, dan dapat digunakan pada perangkat desktop maupun mobile.

---

## Fitur

| Fitur              | Keterangan                                         |
| ------------------ | -------------------------------------------------- |
| Profil             | Menampilkan nama, username, bio, avatar, dan cover |
| Linktree           | Kumpulan link penting dalam satu halaman           |
| WhatsApp Channel   | Akses channel resmi Yobasepay, Yobase, dan Yohost  |
| Instagram          | Link langsung menuju Instagram                     |
| Dark Mode          | Mode terang dan gelap                              |
| Background Music   | Musik latar menggunakan `music.mp3`                |
| Share              | Membagikan halaman menggunakan Web Share API       |
| Copy Link          | Fallback untuk menyalin URL halaman                |
| Toast Notification | Notifikasi interaktif                              |
| Responsive         | Mendukung mobile, tablet, dan desktop              |
| Static Website     | Tidak membutuhkan database atau PHP                |

---

## Struktur Folder

```text
yobasehub/
│
├── index.html
├── vercel.json
└── music.mp3
```

### Penjelasan File

**index.html**

File utama website. Seluruh HTML, CSS, dan JavaScript berada di dalam file ini.

**vercel.json**

Konfigurasi deployment untuk Vercel.

**music.mp3**

File musik yang digunakan sebagai background music website.

Jika tidak ingin menggunakan musik, file `music.mp3` dapat dihapus dan bagian audio pada `index.html` dapat dihilangkan.

---

## Cara Memasang

### 1. Download File

Siapkan file berikut:

```text
index.html
vercel.json
music.mp3
```

Kemudian masukkan semuanya ke dalam satu folder.

```text
yobasehub/
├── index.html
├── vercel.json
└── music.mp3
```

---

## Menjalankan di Localhost

Website ini merupakan static HTML sehingga tidak membutuhkan PHP atau database.

### Windows

Buka folder project kemudian buka:

```text
index.html
```

File akan langsung terbuka melalui browser.

### Menggunakan Visual Studio Code

Jika menggunakan Visual Studio Code, Anda dapat menggunakan extension Live Server.

Klik kanan `index.html`, kemudian pilih:

```text
Open with Live Server
```

---

# Deploy ke Vercel

## Cara 1 — Menggunakan GitHub

### Step 1 — Buat Repository

Buat repository baru di GitHub.

Contoh nama repository:

```text
yobasehub
```

Upload file:

```text
index.html
vercel.json
music.mp3
```

---

### Step 2 — Import ke Vercel

Buka:

https://vercel.com

Login menggunakan akun GitHub.

Kemudian pilih:

```text
Add New Project
```

Pilih repository:

```text
yobasehub
```

---

### Step 3 — Konfigurasi Project

Gunakan konfigurasi berikut:

```text
Framework Preset : Other
Build Command    : kosong
Output Directory : .
Install Command  : kosong
```

Kemudian klik:

```text
Deploy
```

Setelah proses selesai, website sudah dapat diakses melalui domain Vercel.

---

# Menggunakan Domain yobasehub.net

Setelah project berhasil di-deploy:

1. Masuk ke project di Vercel.
2. Buka `Settings`.
3. Pilih `Domains`.
4. Tambahkan domain:

```text
yobasehub.net
```

5. Ikuti konfigurasi DNS yang diberikan Vercel.
6. Tunggu proses propagasi DNS.
7. Setelah selesai, website dapat diakses melalui:

https://yobasehub.net

---

# Konfigurasi DNS

Jika domain menggunakan Cloudflare atau DNS provider lainnya, masukkan record yang diberikan oleh Vercel.

Contoh:

```text
Type : CNAME
Name : www
Target : cname.vercel-dns.com
```

Untuk domain utama, gunakan record yang ditampilkan pada dashboard Vercel.

Jangan menggunakan IP atau target lama apabila Vercel memberikan konfigurasi yang berbeda.

---

# Mengubah Profil

Data profil dapat diubah langsung melalui `index.html`.

Contoh nama:

```html
<h1 class="profile-name">
    Yoganugroho
</h1>
```

Username:

```html
<a href="https://www.instagram.com/yogakarsadipa">
    @yogakarsadipa
</a>
```

Bio:

```html
<p class="profile-bio">
    Digital Tech Enthusiast & Founder Yobase, Yobasepay & Yohost
</p>
```

---

# Mengubah Foto Profil

Cari bagian gambar profil pada `index.html`:

```html
<img
    src="https://domainanda.com/avatar.jpg"
    alt="Yoganugroho"
    class="avatar-img"
>
```

Kemudian ganti URL gambar sesuai kebutuhan.

---

# Mengubah Cover

Cari bagian:

```html
<img
    src="https://domainanda.com/cover.jpg"
    class="cover-img-full"
>
```

Kemudian ganti URL dengan gambar cover yang diinginkan.

---

# Menambahkan Link

Tambahkan kartu baru di dalam:

```html
<div class="links-container">
```

Contoh:

```html
<a
    href="https://example.com"
    target="_blank"
    rel="noopener noreferrer"
    class="link-card blue-standard"
>
    <div class="link-left">

        <div class="icon-box">
            <i class="fa-solid fa-globe"></i>
        </div>

        <div class="link-info">

            <div class="link-title">
                Website Saya
                <span class="link-badge">
                    Website
                </span>
            </div>

            <div class="link-desc">
                Kunjungi website resmi saya
            </div>

        </div>

    </div>

    <div class="link-arrow">
        <i class="fa-solid fa-chevron-right"></i>
    </div>
</a>
```

---

# Mengganti Musik

Letakkan file musik dengan nama:

```text
music.mp3
```

di folder yang sama dengan `index.html`.

```text
yobasehub/
├── index.html
├── vercel.json
└── music.mp3
```

Kemudian HTML akan menggunakan:

```html
<audio
    id="bgMusic"
    src="music.mp3"
    loop
    preload="auto">
</audio>
```

Browser modern dapat memblokir autoplay audio sebelum pengguna melakukan interaksi pada halaman.

Website sudah menyediakan mekanisme untuk mencoba menjalankan musik setelah pengguna melakukan interaksi.

---

# Dark Mode

Dark Mode menggunakan `localStorage` sehingga pilihan tema pengguna dapat disimpan pada browser.

Contoh:

```javascript
localStorage.setItem(
    'yoganugroho_theme',
    newTheme
);
```

Ketika website dibuka kembali, tema sebelumnya akan digunakan.

---

# Share Website

Website menggunakan Web Share API:

```javascript
navigator.share()
```

pada perangkat atau browser yang mendukungnya.

Jika fitur tersebut tidak tersedia, website akan menggunakan metode copy link sebagai alternatif.

---

# Teknologi

Project ini menggunakan:

* HTML5
* CSS3
* JavaScript
* Font Awesome
* Google Fonts
* Vercel

---

# Mengapa Menggunakan Vercel?

Versi awal website menggunakan PHP untuk menyimpan konfigurasi profil dan melakukan looping data link.

Versi YobaseHub telah dikonversi menjadi static website menggunakan:

```text
HTML
CSS
JavaScript
```

Sehingga tidak membutuhkan:

```text
PHP
MySQL
Apache
Nginx
Backend Server
```

Website dapat langsung di-deploy ke Vercel sebagai static website.

---

# Database

YobaseHub tidak menggunakan database.

Konten utama website berada pada:

```text
index.html
```

Gambar profil dan cover dapat menggunakan URL eksternal atau CDN.

---

# Responsive

Website dirancang agar dapat digunakan pada:

```text
Desktop
Laptop
Tablet
Android
iPhone
```

---

# Live Website

**YobaseHub**

https://yobasehub.net

Personal Profile, Social Links & Official Channels.

---

# Lisensi

Project ini merupakan website personal YobaseHub milik Yoganugroho.

© 2026 Yoganugroho. All Rights Reserved.
