# 🌿 PilahYuk - Aplikasi Pemilah Sampah Pintar Berbasis AI (Android)

Aplikasi mobile pintar yang memanfaatkan teknologi Kecerdasan Buatan (Artificial Intelligence) untuk membantu masyarakat mengklasifikasikan jenis sampah secara *real-time* dan memberikan edukasi langkah daur ulang yang tepat.

Proyek ini diajukan untuk memenuhi tugas **Ujian Akhir Semester (UAS) Pemrograman Mobile**.

---

## 👥 Identitas Pengembang
*   **Nama Mahasiswa**: Sofyan Agung
*   **NIM**: 231011400159
*   **Mata Kuliah**: Mobile Progamming
*   **Kelas**: 06tplp003

---

## 🚀 Fitur Utama Aplikasi

1.  **Klasifikasi Sampah Berbasis AI (TensorFlow Lite)**
    *   Menggunakan model Deep Learning MobileNet teroptimasi lokal (`.tflite`) yang berjalan **100% Offline** (tanpa kuota internet).
    *   Mendukung pemilahan **6 kategori sampah spesifik**: Plastik, Kertas, Organik, Logam, Kaca, dan sampah B3 (Bahan Berbahaya dan Beracun).
    *   Dilengkapi **Confidence Threshold 55%** untuk meminimalkan salah deteksi (jika di bawah 55%, objek dideteksi sebagai *Tidak Terdeteksi*).
    *   **Auto-Brightness & Exposure override (+4)** agar pratinjau kamera tetap terang di kondisi ruangan redup.
2.  **Dashboard Statistik Dinamis (Room Database)**
    *   Menampilkan ringkasan kontribusi pengguna (Total Scan, Eco Points, Pengurangan Karbon).
    *   Visualisasi **Pie Chart (Diagram Lingkaran) interaktif** yang dihitung secara dinamis dari SQLite lokal menggunakan library **Room Database**.
3.  **Integrasi Peta Bank Sampah Lokal**
    *   Menampilkan titik lokasi Bank Sampah terdekat di wilayah Tangerang Selatan dan Jakarta Selatan.
    *   Menggunakan **Leaflet Map (HTML5 WebView)** yang sangat ringan tanpa ketergantungan Google Maps API Key berbayar.
4.  **Aksesibilitas Lengkap (Accessibility)**
    *   **Text-to-Speech (TTS)**: Aplikasi otomatis membacakan suara hasil klasifikasi dalam Bahasa Indonesia.
    *   **Mode Kontras Tinggi**: Mengubah warna tema aplikasi secara instan menjadi hitam-putih pekat untuk pengguna dengan keterbatasan penglihatan.
    *   **Kontrol Getaran Haptic**: Mematikan atau menghidupkan getaran klik secara total hingga ke tingkat sistem Android.
5.  **Bypass Login Penguji (Tester Account)**
    *   Disediakan akun *bypass* khusus dosen penguji agar tidak perlu registrasi ulang:
        *   **Username**: `agung`
        *   **Password**: `admin123`

---

## 📦 Unduh & Instalasi Aplikasi (APK)

Anda dapat mengunduh file aplikasi mentah siap pasang langsung dari repositori ini:

### 📥 **[Unduh PilahYuk APK Di Sini](./PilahYuk.apk?raw=true)**

#### 📲 Langkah Instalasi di HP Android:
1.  Unduh file **`PilahYuk.apk`** melalui tautan di atas langsung dari HP Anda.
2.  Setelah selesai diunduh, ketuk file tersebut untuk memulai pemasangan.
3.  Jika sistem Android menampilkan peringatan *Install dari Sumber Tidak Dikenal (Unknown Sources)*, silakan masuk ke Setelan HP Anda dan aktifkan izin instalasi untuk Browser/File Manager Anda.
4.  Ketuk **Instal** dan tunggu hingga proses selesai.
5.  Buka aplikasi **PilahYuk** dan gunakan akun bypass `agung` / `admin123` untuk menguji semua fiturnya.

---

## 🛠️ Tech Stack & Library
*   **Language**: Java (Android Native SDK)
*   **UI Architecture**: Material Design 3 (M3 Custom Organic Theme)
*   **Database**: Android Room Persistence Library (SQLite wrapper)
*   **AI Engine**: TensorFlow Lite Android Support Library
*   **Maps Engine**: WebView integration with Leaflet JS & OpenStreetMap
*   **Graphics & Animation**: Custom Canvas, ValueAnimator, & ObjectAnimator

---

Copyright © 2026 Sofyan Agung. All rights reserved.
