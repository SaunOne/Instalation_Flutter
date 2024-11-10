
![Logo](https://storage.googleapis.com/cms-storage-bucket/6a07d8a62f4308d2b854.svg)

# Panduan Instalasi Flutter

Dokumen ini berisi langkah-langkah instalasi Flutter dari awal hingga persiapan Android Studio untuk menjalankan emulator Android.

---

## Langkah-langkah Instalasi

### Langkah 1: Install Flutter SDK

1. **Download Flutter SDK**
   - Buka [flutter.dev](https://docs.flutter.dev/get-started/install).
   - Pilih OS yang sesuai (Windows, macOS, atau Linux).
   - Klik **Download SDK**.

2. **Ekstrak Flutter SDK**
   - Setelah unduhan selesai, ekstrak file `.zip` (untuk Windows) atau `.tar.xz` (untuk macOS/Linux) ke direktori yang diinginkan, misalnya `C:\src\flutter` atau `/usr/local/flutter`.

3. **Tambahkan Flutter ke PATH**
   - Langkah ini memungkinkan Anda untuk menjalankan perintah Flutter di terminal atau command prompt.
   - **Windows**:
     - Buka **Control Panel > System and Security > System > Advanced System Settings > Environment Variables**.
     - Tambahkan path `C:\src\flutter\bin` ke variabel `Path`.
   - **macOS/Linux**:
     - Tambahkan `export PATH="$PATH:/path_to_flutter/flutter/bin"` ke file `~/.bashrc` atau `~/.zshrc` dan jalankan `source ~/.bashrc` atau `source ~/.zshrc` untuk menyegarkan.

4. **Verifikasi Instalasi Flutter**
   - Buka terminal dan jalankan:
     ```bash
     flutter doctor
     ```
   - Perintah ini akan memeriksa apakah Flutter sudah terpasang dengan benar dan menampilkan komponen yang perlu diinstal.

---

### Langkah 2: Install Android Studio

1. **Download dan Instal Android Studio**
   - Buka [Android Studio](https://developer.android.com/studio).
   - Unduh installer sesuai OS, lalu ikuti instruksi instalasi.

2. **Konfigurasi SDK di Android Studio**
   - Buka Android Studio, lalu pergi ke **SDK Manager**:
     - **Windows/macOS**: File > Settings > Appearance & Behavior > System Settings > Android SDK.
     - **Linux**: Android Studio > Preferences > Appearance & Behavior > System Settings > Android SDK.
   - Di tab **SDK Platforms**, pilih versi Android yang kompatibel (misalnya, Android 12).
   - Di tab **SDK Tools**, pastikan **Android SDK Build-Tools** dan **Android Emulator** dicentang.

3. **Install SDK dan Tools Tambahan**
   - Klik **Apply** atau **OK** untuk mengunduh semua tools yang diperlukan.

---

### Langkah 3: Menyiapkan Emulator Android

1. **Buka AVD Manager**
   - Di Android Studio, buka **AVD Manager** melalui **Tools > AVD Manager**.

2. **Buat Virtual Device**
   - Klik **Create Virtual Device**.
   - Pilih perangkat, seperti **Pixel 4**.
   - Pilih versi Android yang diinginkan, misalnya Android 12, lalu klik **Download** (jika belum terpasang), dan **Next**.

3. **Konfigurasi Emulator**
   - Sesuaikan pengaturan emulator jika diperlukan, lalu klik **Finish**.

4. **Jalankan Emulator**
   - Di AVD Manager, klik **Play** (ikon segitiga hijau) di sebelah emulator untuk memulai.

---

### Langkah 4: Integrasi Flutter dengan Android Studio

1. **Install Plugin Flutter dan Dart**
   - Di Android Studio, buka **Settings > Plugins**.
   - Cari **Flutter** dan klik **Install** untuk menambahkan plugin Flutter dan Dart.

2. **Verifikasi dengan Flutter Doctor**
   - Di terminal, jalankan:
     ```bash
     flutter doctor --android-licenses
     ```
   - Tekan `y` untuk menyetujui semua lisensi SDK.

3. **Periksa Koneksi Semua Komponen**
   - Jalankan kembali `flutter doctor` dan pastikan semua komponen terdeteksi, terutama bagian `Android Studio` dan `Connected Device`.

---

### Langkah 5: Membuat dan Menjalankan Proyek Flutter

1. **Buat Proyek Flutter Baru**
   - Di terminal, masuk ke direktori yang diinginkan lalu jalankan:
     ```bash
     flutter create nama_proyek
     ```
   - Ganti `nama_proyek` dengan nama proyek Anda.

2. **Jalankan Proyek**
   - Masuk ke direktori proyek:
     ```bash
     cd nama_proyek
     ```
   - Jalankan aplikasi Flutter di emulator dengan:
     ```bash
     flutter run
     ```

Setelah menjalankan `flutter run`, aplikasi Flutter Anda akan ditampilkan di emulator Android yang sudah dibuat.

---

Dokumen ini membantu dalam melakukan instalasi Flutter dan Android Studio dari awal, termasuk cara menyiapkan emulator untuk pengembangan aplikasi Flutter. 
