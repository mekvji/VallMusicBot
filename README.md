# 🎵 Telegram Enterprise Music & Video Bot

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?style=for-the-badge&logo=python)
![Telethon](https://img.shields.io/badge/Telethon-Async-red?style=for-the-badge&logo=telegram)
![PyTgCalls](https://img.shields.io/badge/PyTgCalls-v3.0%2B-success?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)

Bot pemutar Musik dan Video Telegram berkinerja tinggi yang dibangun menggunakan **Telethon** dan **PyTgCalls v3**. Dirancang khusus untuk skalabilitas kelas *Enterprise*, bot ini dilengkapi dengan sistem manajemen server cerdas, antrean berbasis database, dan pembagian hak akses (Kasta/VIP) untuk memastikan server Anda tidak pernah *overload*.

---

## ✨ Fitur Unggulan

* **🎧 Seamless Streaming:** Putar lagu dan video dari YouTube, TikTok, atau File Telegram lokal tanpa lag.
* **📑 Smart Database Queue:** Sistem antrean lagu yang aman dan persisten (menyimpan data di SQLite), tidak hilang saat bot di-*restart*.
* **👑 Sistem Kasta (VIP & User):** User biasa dibatasi maksimal 5 antrean, sementara pengguna VIP menikmati akses tanpa batas.
* **🛡️ Global Server Limit & Auto-Kick:** Server dibatasi maksimal 10 grup bersamaan. VIP dapat memotong antrean dan menghentikan pemutaran User Biasa jika server penuh.
* **🎛️ Interactive Admin Dashboard:** Pantau grup yang aktif (`/listplay`) dan hentikan paksa atau *banned* grup nakal (`/listban`) langsung dari panel interaktif.
* **🎬 Integrasi LK21 (Bioskop VIP):** Fitur nonton bareng (Nobar) eksklusif untuk VIP menggunakan API LK21.
* **📥 Smart Downloader:** Unduh media dengan batasan kuota (10x untuk User Biasa, *Unlimited* untuk VIP).

---

## 🚀 Rekomendasi Hosting Terbaik

Streaming musik dan video ke Voice Chat Telegram membutuhkan koneksi internet berkecepatan tinggi dan CPU yang stabil. 

Untuk performa **tanpa jeda (Zero Lag)** dan **Uptime 99.9%**, kami sangat merekomendasikan Anda untuk menghosting bot ini di **[CloudNext](https://cloudnext.my.id)**.

💎 **Kenapa CloudNext?**
* **Harga Terjangkau:** Spesifikasi mewah dengan harga yang bersahabat untuk *developer*.
* **Koneksi Super Cepat:** Jaringan optimal yang mencegah suara patah-patah (stuttering) pada PyTgCalls.
* **Dukungan Penuh:** Lingkungan server yang sangat ramah untuk instalasi Node.js, Python, dan FFmpeg.

👉 **[Kunjungi CloudNext.my.id Sekarang](https://cloudnext.my.id)**

---

## 🛠️ Persyaratan Sistem

Sebelum melakukan instalasi, pastikan server Anda memiliki komponen berikut:
- Python 3.8 atau lebih baru
- Node.js (untuk API pencarian film LK21)
- `ffmpeg` terinstall di sistem environment

---

## ⚙️ Cara Instalasi (Auto Setup)

Kami telah menyediakan skrip *Auto-Installer* berdesain modern untuk memudahkan proses *deployment*. Skrip ini akan otomatis mengecek dependensi, membuat environment, dan menjalankan bot Anda.

1. **Clone Repositori ini:**
   ```bash
   git clone [https://github.com/UsernameAnda/NamaRepoAnda.git](https://github.com/UsernameAnda/NamaRepoAnda.git)
   cd NamaRepoAnda
   
