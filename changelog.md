# Changelog Blackout-X | Republic of Xenoverz

## v1.0.5.0 [Burning 🔥 Whyded]
Tanggal Rilis: [Isi tanggal rilis di sini]

### ✨ Fitur Utama Baru

* **1. Dynamic Mode & Thermal Logic:**
    * Implementasi sistem utama yang otomatis beralih antara X-Mode (Performance) dan Z-Mode (Balance).
    * Penambahan logika Thermal Profile spesifik di `service.sh` untuk PUBG (`PUBG` profile) dan game lainnya (`Game 2` profile).
* **2. RAM Management System:**
    * Optimasi agresif pada Virtual Memory (Swappiness, Dirty Ratios, Min Free Kbytes) untuk memaksimalkan RAM fisik yang tersedia, sangat efektif untuk perangkat RAM 4GB.
* **3. Spoof Device & Chipset:**
    * Fitur spoofing untuk membuka kunci opsi grafis tertinggi (misalnya, HDR-EXTREME di PUBG) dan FPS tertinggi di game lainnya.
* **4. GMS Doze:**
    * Pengoptimalan Google Play Services dan proses latar belakang terkait untuk mengurangi konsumsi daya baterai saat idle.
* **5. Reset Guest (PUBG):**
    * Fungsi *guest reset* khusus yang didesain untuk PUBG Mobile (mendukung versi KR, TW, GL, BETA, dll.). ketik atau jalankan perintah di terminal (`su -c PUBG`) (Fitur untuk game lain segera menyusul).

### 🛠️ Peningkatan & Perbaikan Sistem

* **Peningkatan Stabilitas:** Logika inisialisasi `gamelist.json` dipindahkan dari `customize.sh` ke `service.sh` untuk memastikan *file persistence* dan mencegah *error* saat instalasi.
* **Optimasi Loop:** Penyesuaian waktu *sleep* di *main loop* (`service.sh`) menjadi 2 detik untuk keseimbangan antara responsivitas dan efisiensi daya.
* **P-Kill Fix:** Penggunaan *pkill* disesuaikan untuk menargetkan nama skrip tweak yang baru (`X-Mode` dan `Z-Mode`) agar proses *cleanup* lebih andal.

### 🧪 Fitur Dalam Pengembangan (Testing/Development)

* **Fstrim:** Program ditambahkan ke modul, saat ini dalam tahap pengujian. Dapat dipicu manual via Terminal (`su -c FSTRIM`).
* **Color Saturation:** Fitur untuk penyesuaian saturasi warna ditambahkan, saat ini masih dalam pengembangan.
