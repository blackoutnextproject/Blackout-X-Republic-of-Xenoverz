# 🚀 Blackout-X | Republic of Xenoverz

![Blackout-X Banner](https://raw.githubusercontent.com/blackoutnextproject/Blackout-Project-Banner/main/Blackout-banner.jpg)

| Version | Codename | Download |
| :--- | :--- | :--- |
| **v1.0.5.0** | Burning 🔥 Whyded | [Link Download Terbaru] |

Modul Magisk Dinamis yang dirancang untuk memberikan pengalaman gaming maksimal dan efisiensi baterai optimal. Blackout-X secara otomatis mendeteksi ketika sebuah game berjalan dan menyesuaikan pengaturan sistem (CPU, RAM, Thermal, dan Spoofing) sesuai kebutuhan, kemudian mengembalikannya ke mode seimbang saat game ditutup.

---

## ✨ Fitur Utama

| Fitur | Deskripsi | Status |
| :--- | :--- | :--- |
| **1. Dynamic Mode & Thermal Logic** | Sistem utama yang secara otomatis beralih antara **X-Mode (Performance)** dan **Z-Mode (Balance)** berdasarkan deteksi game dari `gamelist.json`. Termasuk logika *Thermal Profile* spesifik per game (misalnya, PUBG menggunakan profil khusus). | ✅ Aktif |
| **2. RAM Management System** | Tweak agresif pada ZRAM, Swappiness, Dirty Ratios, dan Min Free Kbytes untuk memaksimalkan ketersediaan RAM fisik (4GB Friendly) saat gaming, dan kembali ke mode aman saat idle. | ✅ Aktif |
| **3. Spoof Device & Chipset** | Mengubah *device fingerprint* secara virtual untuk membuka kunci opsi grafis dan FPS tertinggi (misalnya, HDR-EXTREME di PUBG Mobile dan FPS tertinggi di game lain). | ✅ Aktif |
| **4. GMS Doze** | Mengoptimalkan Google Play Services dan proses latar belakang terkait untuk mengurangi konsumsi daya tanpa mengorbankan stabilitas sistem inti. | ✅ Aktif |
| **5. Reset Guest (PUBG)** | Fungsi *guest reset* khusus yang didesain untuk PUBG Mobile (mendukung versi KR, TW, GL, BETA, & dll.). Memungkinkan pengguna mereset akun tamu dengan mudah. | ✅ Aktif |
| **6. Fstrim** | Program untuk menjaga kecepatan I/O *disk* tetap optimal. | 🛠️ Testing Phase |
| **7. Color Saturation** | Penyesuaian saturasi warna untuk pengalaman visual yang lebih baik. | 🛠️ Under Development |

---

## ⚙️ Petunjuk Penggunaan dan Konfigurasi

### A. Konfigurasi Daftar Game (`gamelist.json`)

Untuk memastikan Mode Gaming aktif, Anda wajib memasukkan *package name* game Anda ke dalam file `gamelist.json`.

**Lokasi File:** `/data/adb/modules/Blackout-X-Republic-of-Xenoverz/gamelist.json`

**Format:**
```json
[
  "com.tencent.ig",        // Contoh PUBG Mobile
  "com.mobile.legends",    // Contoh Mobile Legends
  "com.example.yourgame"   // Tambahkan package game Anda di sini
]
