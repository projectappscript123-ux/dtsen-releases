# 📱 APLIKASI KUESIONER DTSEN

Aplikasi mobile untuk kuesioner data keluarga dan individu dengan integrasi Google Sheets.

**Versi**: 5.2.8 🎉  
**Platform**: React Native (Expo)  
**Android**: ✅ Full Support  
**Status**: Production Ready

---

## 🚀 FITUR

### 📋 **Core Features**
- ✅ Login dengan autentikasi aman
- ✅ **Form Keluarga** (60 pertanyaan dalam 7 bagian)
- ✅ **Form Individu** (43 pertanyaan dalam 7 bagian)
- ✅ Integrasi Google Sheets (online-only)
- ✅ CRUD operations (Create, Read, Update, Delete)
- ✅ Filter & Search by Dusun
- ✅ Session management dengan auto-logout

### 📱 **Mobile Features**
- ✅ **Camera & Gallery** - Upload foto KK/KTP dan rumah
- ✅ **GPS Location** - Auto-detect koordinat rumah
- ✅ **Offline Storage** - AsyncStorage untuk session data
- ✅ **Universal UI** - Optimized untuk semua device Android
- ✅ **Smart Network Status** - Real-time network monitoring dengan icon dinamis (v5.1.3)
- ✅ **Date Picker Calendar** - Kalender native untuk input tanggal lahir (v5.1.4)
- ✅ **WilayahIndonesiaPicker** - Picker cascading Provinsi/Kabupaten/Kecamatan/Desa Indonesia (v5.1.4)
- ✅ **Centralized Settings** - Sistem pengaturan terpusat dengan SettingsService (v5.1.5)
- ✅ **Download Progress Popup** - Progress bar real-time saat download APK (v5.1.6)
- ✅ **In-App Download** - Download APK langsung tanpa buka browser (v5.1.6)
- 🆕 **Improved APK Install** - Multiple fallback methods untuk install APK (v5.1.8)

### 📝 **Form Features**
- ✅ **Smart Validation** - Real-time field validation dengan error highlighting
- ✅ **Auto-scroll** - Scroll otomatis ke field error saat validasi gagal
- ✅ **Conditional Fields** - Field muncul berdasarkan pilihan
- ✅ **Dropdown Options** - 500+ pilihan dropdown sesuai standar BPS
- ✅ **Number Input** - Keyboard numerik untuk field angka
- ✅ **Auto-generate ID** - ID USUL otomatis dengan format terstruktur
- ✅ **Form Reset** - Clear semua field setelah submit berhasil
- ✅ **Confirmation Modal** - Konfirmasi sebelum submit data
- ✅ **Conditional Photo Upload** - Upload foto KK baru jika pindah KK (v5.1.1)
- ✅ **Photo Preview System** - Preview foto baru sebelum update data (v5.1.4)
- ✅ **Photo Reset System** - Reset foto otomatis jika batal/gagal update (v5.1.4)
- ✅ **RT/RW 3-Digit Validation** - Validasi RT dan RW wajib 3 digit termasuk "000" (v5.1.4)

### 🔄 **System Features**
- ✅ **Update Checker** - Menu cek update dengan download & install APK otomatis
- ✅ **Auto-versioning** - Git-based version management
- ✅ **Error Prevention** - Crash detection & recovery
- ✅ **Silent Operation** - No popup notifications
- ✅ **GitHub Releases Support** - Hosting APK di GitHub untuk download yang lebih reliable (v5.1.6)
- ✅ **Session Cleanup** - Auto-cleanup expired sessions
- ✅ **Version Consistency** - Konsistensi versi di semua konfigurasi
- ✅ **Network Monitoring** - Real-time network status dengan ping measurement (v5.1.3)
- ✅ **Photo System Overhaul** - Separated services untuk stabilitas maksimal (v5.1.4)
- ✅ **Direct Upload System** - Simplified photo upload tanpa cache kompleks (v5.1.4)
- ✅ **Global Settings** - Settings GLOBAL untuk semua user, hanya admin yang bisa ubah (v5.1.5)
- ✅ **Force Logout Detection** - Deteksi otomatis saat login di device lain (v5.1.5)
- 🆕 **REQUEST_INSTALL_PACKAGES Permission** - Permission untuk install APK dari dalam aplikasi (v5.1.8)

### 🔐 **Admin Features**
- ✅ **User Management** - Kelola user (admin only)
- ✅ **Session Management** - Manual & auto cleanup expired sessions
- ✅ **Auto Trigger** - Otomatis setup cleanup trigger saat spreadsheet dibuka
- ✅ **Admin Notes** - Catatan status data dengan 5 pilihan warna di card list (v5.1.0)

---

## 🎉 WHAT'S NEW IN v5.2.8

### 🗑️ **Dashboard Optimization**
- **Menghapus Tabel Status Sinkronisasi**: Tabel yang memiliki masalah penjumlahan tidak akurat telah dihapus
- **Dashboard Lebih Fokus**: Hanya menampilkan 3 tabel utama - Kuesioner per Dusun, Penduduk per Dusun, dan Status Penduduk
- **UI Lebih Bersih**: Interface dashboard lebih sederhana dan mudah dipahami

### 🚀 **Performance Improvements**
- **Loading Lebih Cepat**: Menghapus query `getSyncStatistics()` yang tidak perlu
- **Kode Lebih Maintainable**: Menghapus komponen dan state yang tidak terpakai

---

## 🎉 WHAT'S NEW IN v5.2.6

### ⚡ **Performance Optimization**
- **Optimasi Load Data Offline**: Query database lebih cepat dengan method `getUnsyncedKeluarga()` dan `getUnsyncedIndividu()`
- **Tab Caching**: Cache data per tab selama 30 detik untuk menghindari reload berulang
- **Instant Tab Switching**: Tidak ada lagi blank screen saat switch tab KELUARGA ↔ INDIVIDU

### 👥 **Online Users Fix**
- **Client-side Timeout Check**: User otomatis offline jika tidak aktif >30 detik
- **Optimized Intervals**: Presence update 10s, fetch 15s (dari 5s dan 10s)
- **Accurate Online Status**: Status online lebih akurat dan real-time

### 🐛 **Bug Report Manager (Admin Only)**
- **List Bug Reports**: Lihat semua bug report dengan search & filter
- **Statistics Dashboard**: Total, open, in progress, resolved, closed
- **Detail View**: Stack trace, device info, error message lengkap
- **Update Status**: Ubah status bug (open, in progress, resolved, closed)
- **Delete Bug**: Hapus bug report yang sudah selesai

---

## 🎉 WHAT'S NEW IN v5.2.5

### 🎨 **UI/UX Improvements**
- **Tab Bar Modern**: Efek animasi bounce saat klik menu tab bar seperti aplikasi modern
- **Tab Bar Responsive**: Ukuran teks tab bar responsif agar tidak terpotong di semua ukuran HP
- **Tab Bar Centralized**: Semua konfigurasi tab bar dipindahkan ke file terpusat (TabBarConfig.ts)
- **Splash Screen**: Tampilan logo dan nama aplikasi dengan delay 3 detik sebelum form login
- **Loading Kelola User**: Modal "Memuat data user..." saat membuka halaman Kelola User

### 🐛 **Bug Fixes**
- **Tab Bar Text Truncation**: Memperbaiki teks menu tab bar yang terpotong dengan mengatur width dan padding yang tepat

---

## 🎉 WHAT'S NEW IN v5.2.0

### 🎨 **UI/UX Improvements**
- **Konsistensi Header Bar**: Tinggi header bar hitam disamakan di semua menu utama (Dashboard, Data, Kuesioner, Penduduk, Profile)
- **NotificationBell di Semua Menu**: Icon notifikasi bell sekarang muncul di semua menu untuk admin
- **Komponen Lebih Compact**: NetworkStatusBar dan OnlineUsersIndicator dikecilkan untuk ruang yang lebih baik
- **Total Bar Penduduk**: Menambahkan bar hijau yang menampilkan total data penduduk
- **Update Checker Dirapikan**: Tombol dan modal cek update di menu Profile lebih compact dan rapi
- **Footer Dashboard Dihapus**: Menghilangkan footer yang tidak perlu di dashboard
- **Tab Bar Modern**: Efek animasi bounce saat klik menu tab bar seperti aplikasi modern
- **Tab Bar Responsive**: Ukuran teks tab bar responsif agar tidak terpotong di semua ukuran HP
- **Tab Bar Centralized**: Semua konfigurasi tab bar dipindahkan ke file terpusat (TabBarConfig.ts)
- **Splash Screen**: Tampilan logo dan nama aplikasi dengan delay 3 detik sebelum form login
- **Loading Kelola User**: Modal "Memuat data user..." saat membuka halaman Kelola User

### 🐛 **Bug Fixes**
- **Modal Dropdown Terhalang**: Memperbaiki modal dropdown yang terhalang tombol navigasi HP dengan menambahkan paddingBottom di semua bottom sheet modal
- **Update Data Penduduk Tidak Tersimpan**: Memperbaiki field yang tidak tersimpan ke spreadsheet dengan normalisasi field names (mixed case dan UPPERCASE)
- **Tab Bar Text Truncation**: Memperbaiki teks menu tab bar yang terpotong dengan mengatur width dan padding yang tepat

### 📝 **Update Konten**
- **Tentang Aplikasi**: Tambah section Menu Utama (Dashboard, Data, Kuesioner, Penduduk, Profile)
- **Pusat Bantuan**: Update panduan dengan menu utama yang lengkap

### 🐛 **Perbaikan Online Users**
- **Timeout Check**: User yang tidak aktif >40 detik tidak ditampilkan meskipun IS_ONLINE = TRUE
- **Force Close Handling**: User yang force close aplikasi akan otomatis hilang dari daftar online setelah 40 detik

### 🧹 **Session Cleanup Enhancement**
- **Auto Delete Logout Sessions**: Session dengan status `logout` atau `force_logout` otomatis dihapus dari spreadsheet
- **Max 20 Sessions**: Membatasi maksimal 20 session di spreadsheet, session paling lama dihapus otomatis jika melebihi

---

## 🎉 WHAT'S NEW IN v5.1.9

### 🔧 **Migrasi Akun Expo Baru & Perbaikan Install APK**
- **Owner Update**: Migrasi ke akun Expo baru `hikmal_zerozeerozeven`
- **Project ID**: Generate projectId baru untuk akun Expo yang baru
- **5 Metode Install**: Menambahkan 2 metode fallback baru (file manager dan file picker)
- **Browser Fallback**: Jika semua metode install gagal, otomatis buka browser untuk download
- **BackHandler Fix**: Memperbaiki tombol "Keluar Aplikasi" yang tidak berfungsi

---

## 🎉 WHAT'S NEW IN v5.1.8

### 🔧 **Fix APK Install & Field Mapping**
- **Multiple Install Methods**: Fungsi installAPK sekarang mencoba 3 metode berbeda untuk install APK
- **REQUEST_INSTALL_PACKAGES Permission**: Menambahkan permission untuk install APK dari sumber tidak dikenal
- **File Manager Fallback**: Jika semua metode install gagal, buka file manager agar user bisa install manual
- **Field NO. Fix**: Memperbaiki mapping field "NO." di data penduduk (sebelumnya tidak terbaca dari spreadsheet)
- **Label Cleanup**: Menghapus keterangan "(Data dari Spreadsheet)" yang tidak perlu di form edit penduduk

---

## 🎉 WHAT'S NEW IN v5.1.7

### 🔧 **Fix In-App Download & GitHub Releases Support**
- **UpdateCheckerStartup In-App Download**: Menambahkan fitur in-app download di komponen UpdateCheckerStartup
- **Download Progress Modal**: Popup progress download dengan progress bar real-time
- **GitHub Releases Support**: Download APK sekarang support URL dari GitHub Releases
- **Expo FileSystem Legacy**: Fix deprecated `downloadAsync` dengan import dari `expo-file-system/legacy`
- **Fallback Browser**: Jika in-app download gagal, otomatis buka browser sebagai fallback

---

## 🎉 WHAT'S NEW IN v5.1.6

### 📥 **Download Progress Popup**
- **Real-time Progress Bar**: Progress bar dengan persentase saat download APK
- **Status Text Dinamis**: Status berubah (Mempersiapkan → Mengunduh → Selesai)
- **Icon Animasi**: Icon cloud-download dengan animasi pulse saat download
- **Download Tips**: Pesan "Jangan tutup aplikasi selama proses download"
- **Tombol Batal**: Bisa batalkan download jika gagal

### 📱 **In-App Download (Android)**
- **Direct Download**: Download APK langsung di dalam aplikasi tanpa buka browser
- **Auto Install**: Setelah download selesai, otomatis buka installer APK
- **Fallback Browser**: Jika in-app download gagal, otomatis buka browser

### 🐙 **GitHub Releases Support**
- **Reliable Hosting**: APK di-host di GitHub Releases untuk download yang lebih reliable
- **Direct Link**: URL langsung ke file APK tanpa redirect
- **Version Tagging**: Setiap versi di-tag di GitHub untuk tracking

---

## 🎉 WHAT'S NEW IN v5.1.5

### ⚙️ **Centralized Settings System**
- **SettingsService**: Service terpusat untuk mengelola semua pengaturan aplikasi
- **SettingsModal**: Modal pengaturan komprehensif dengan UI user-friendly
- **useSettings Hook**: Custom hook untuk akses settings dengan real-time updates
- **Persistent Storage**: Settings disimpan di AsyncStorage
- **Real-time Sync**: Perubahan settings langsung tersinkronisasi ke seluruh komponen

### 🔐 **Session & Authentication**
- **Global Settings**: Settings sekarang GLOBAL (1 baris untuk semua user), hanya admin yang bisa ubah
- **Force Logout Detection**: Deteksi otomatis saat user login di device lain dengan popup "Sesi Berakhir"
- **Session Cleanup**: Logout sekarang HAPUS baris session dari sheet (bukan hanya set status)
- **Online Users Fix**: Set IS_ONLINE = FALSE otomatis saat user di-force logout
- **Auto-Login Fix**: Memperbaiki bug user bisa login tanpa input setelah logout

### 📊 **Google Apps Script Updates**
- **saveUserSettings()**: Sekarang tanpa userId, simpan ke row 2 (global)
- **getUserSettings()**: Sekarang tanpa userId, baca dari row 2 (global)
- **logoutSession()**: Set status 'logout' → Tunggu 100ms → Hapus baris session
- **setUserOfflineInOnlineUsers()**: Fungsi baru untuk set IS_ONLINE = FALSE

---

## 🎉 WHAT'S NEW IN v5.1.4

### 🗺️ **WilayahIndonesiaPicker**
- **Cascading Picker**: Picker untuk Provinsi → Kabupaten → Kecamatan → Desa Indonesia
- **API Integration**: Data wilayah dari API emsifa.com (gratis dan lengkap)
- **Search Feature**: Fitur pencarian di setiap level wilayah
- **Form Integration**: Terintegrasi di form input-individu dan update-individu
- **Custom Hook**: `useWilayahIndonesia` hook untuk penggunaan yang lebih fleksibel

### 📸 **Major Photo System Overhaul**
- **Separated Photo Services**: Memisahkan semua service foto menjadi 14 file terpisah untuk Keluarga dan Individu
  - `KeluargaPhotoUploadService`, `IndividuPhotoUploadService`
  - `KeluargaPhotoCacheService`, `IndividuPhotoCacheService`
  - `KeluargaBatchPhotoUploadService`, `IndividuBatchPhotoUploadService`
  - `KeluargaPhotoDeleteService`, `IndividuPhotoDeleteService`
  - `KeluargaConsistentPhotoService`, `IndividuConsistentPhotoService`
  - `KeluargaDirectPhotoUploadService`, `IndividuDirectPhotoUploadService`
  - `KeluargaOfflineStorage`, `IndividuOfflineStorage`
- **Simplified Photo Upload**: Mengganti sistem cache kompleks dengan direct upload untuk stabilitas
- **Photo Preview Enhancement**: Foto yang diganti sekarang ditampilkan sebagai preview sebelum update
- **Photo Reset System**: Reset foto otomatis jika user membatalkan update atau jika update gagal
- **Component Separation**: `KeluargaDirectPhotoUpload` dan `IndividuDirectPhotoUpload` terpisah

### 📅 **Date Picker Enhancement**
- **Native Calendar**: Kalender native menggunakan `@react-native-community/datetimepicker`
- **DD-MM-YYYY Format**: Format tanggal konsisten dan user-friendly
- **Auto Validation**: Tidak bisa pilih tanggal masa depan, validasi otomatis
- **Type Safety**: State tanggal diubah dari string ke Date object untuk type safety
- **Cross Platform**: Support Android dan iOS dengan tampilan native masing-masing

### 🎨 **UI/UX Improvements**
- **Photo Border Enhancement**: Border yang jelas pada foto KK baru di form individu
- **Visual Consistency**: Tampilan foto yang konsisten antara form Keluarga dan Individu
- **Loading Messages**: Loading message yang informatif saat delete data dan foto
- **Error Handling**: Error handling yang lebih baik dengan logging detail
- **Logout Button Padding**: Jarak dan padding tombol Keluar di Profil diperbesar

### 🔧 **Critical Bug Fixes**
- **RT/RW Validation**: Validasi RT dan RW wajib 3 digit (termasuk "000")
- **IndividuPhotoDeleteService Import**: Menambahkan import yang hilang di carddetail-individu
- **KeluargaPhotoDeleteService Import**: Menambahkan import yang hilang di carddetail-keluarga
- **Double Login Screen**: Memperbaiki logout yang menyebabkan form login muncul 2 kali
- **Syntax Error**: Fixed missing catch/finally clause di `update-keluarga.tsx`
- **Network Request Failed**: Mengatasi error upload foto dengan sistem direct upload
- **Invalid Image URI Format**: Memperbaiki format URI foto yang tidak valid
- **Date Format**: Memperbaiki format tanggal dari YYYY-MM-DD ke DD-MM-YYYY yang benar

### 🗑️ **Enhanced Delete System**
- **Photo Cleanup**: Foto otomatis terhapus dari Google Drive saat hapus data
- **Smart Detection**: Deteksi otomatis semua foto yang terkait dengan data
- **Progress Tracking**: Loading message yang informatif saat proses delete
- **Error Resilient**: Tetap lanjut delete data meski ada foto yang gagal dihapus
- **Complete Cleanup**: Tidak ada file orphaned yang tertinggal di Google Drive

---

## 🎉 PREVIOUS MAJOR RELEASES

### **v5.1.3** - Smart Network Status & Critical Fixes
- **🌐 Smart Network Status**: Real-time network monitoring dengan ping measurement akurat
- **🐛 Critical Error Fixes**: Fixed undefined property access, hideSaving method, text rendering
- **⚡ Performance**: Optimized endpoints dan realistic ping values berdasarkan jenis koneksi
- **🛡️ Safety Components**: DataErrorBoundary dan SafeText untuk mencegah crash
- **🚨 Critical Bug Fixes**: Resolved infinite loop errors and login stability issues
- **🆕 Admin Notes**: Status tracking dengan 5 pilihan warna di card list
- **📱 Auto Scroll**: Proper implementation dengan multiple attempts
- **🔧 Field Organization**: Logical placement of form fields by category

### **v4.9.0** - Build System Fixes
- **🔧 Critical Build Fix**: Fixed android/app/build.gradle version mismatch
- **🧹 Code Quality**: Fixed TypeScript errors and reduced ESLint warnings
- **📊 Version Consistency**: Unified versioning across entire project

### **v4.8.0** - TypeScript & Consistency
- **🔧 TypeScript Fixes**: Resolved property errors and enhanced type safety
- **📊 Version Consistency**: All files consistently use same version
- **🧹 Project Cleanup**: Removed unnecessary development files

### **v4.0.0** - Major Refactoring
- **🏗️ Complete Refactoring**: New app structure with expo-router
- **🔐 Enhanced Authentication**: Improved session management system
- **🛡️ Robust Error Handling**: Advanced crash prevention and recovery
- **🚀 Performance Boost**: Better memory management and optimizations

---

## 📋 STRUKTUR FORM KUESIONER

### 🏠 **FORM KELUARGA** (60 Pertanyaan)

#### **A. DATA KEPALA KELUARGA** (3 pertanyaan)
- ID USUL (auto-generated)
- NO KK (16 digit)
- NAMA KK

#### **B. BANGUNAN DAN ASET** (16 pertanyaan)
- Status Kepemilikan Bangunan
- Luas Kepemilikan Sawah/Kebun
- Jenis Lantai/Dinding/Atap Terluas
- Kepemilikan Fasilitas BAB & Jenis Kloset
- Tempat Pembuangan Akhir Tinja
- Sumber Air Minum & Jarak ke Tinja
- Sumber Penerangan Utama
- Nomor Pelanggan & Meter Listrik
- Besar Daya & Bahan Bakar Utama

#### **C. ASET BERGERAK** (14 pertanyaan)
- Tabung Gas 5,5 KG atau Lebih
- Lemari Es/Kulkas
- Air Conditioner (AC)
- Pemanas Air (Water Heater)
- Telepon Rumah (PSTN)
- Televisi Layar Datar (Min 30 Inci)
- Emas/Perhiasan (Min 10 Gram)
- Komputer/Laptop/Tablet
- Sepeda Motor & Sepeda
- Mobil, Perahu, Kapal/Perahu Motor
- Smartphone/HP

#### **D. ASET TIDAK BERGERAK** (2 pertanyaan)
- Lahan Tempat Lain
- Rumah Tempat Lain

#### **E. TERNAK** (5 pertanyaan)
- Jumlah Sapi, Kerbau, Kuda
- Jumlah Kambing/Domba
- Jumlah Babi

#### **F. KOORDINAT DAN LOKASI** (3 pertanyaan)
- Titik Koordinat Rumah (GPS)
- Nama Lokasi/Patokan
- Dusun

#### **G. FOTO** (3 pertanyaan)
- Foto KK/KTP Asli
- Foto Rumah Tampak Depan
- Foto Rumah Tampak Dalam

### 👤 **FORM INDIVIDU** (43 Pertanyaan)

#### **A. DATA INDIVIDU** (25 pertanyaan)
- ID USUL INDIVIDU (auto-generated)
- NO KK & NIK (16 digit)
- Apakah Pindah KK? & NO KK Baru
- 📸 **Foto KK Baru** (muncul jika Pindah KK = YA)
- Nama Lengkap & 📅 **Tanggal Lahir** (dengan date picker kalender)
- Jenis Kelamin & Tempat Lahir
- Status Perkawinan & Hubungan Keluarga
- Pendidikan Terakhir & Pekerjaan
- Status Kedudukan Pekerjaan Utama
- Nama Gadis Ibu Kandung
- Alamat Sesuai KTP (Lengkap)
- Provinsi, Kabupaten, Kecamatan, Desa
- RW, RT, Dusun
- Keberadaan Anggota

#### **B. PENDIDIKAN** (4 pertanyaan)
- Partisipasi Sekolah
- Jenjang Pendidikan
- Kelas Tertinggi
- Ijazah Tertinggi

#### **C. TENAGA KERJA** (6 pertanyaan)
- Apakah Bekerja Seminggu Lalu?
- Berapa Jam Bekerja?
- Lapangan Usaha di Pekerjaan Utama
- Status dalam Pekerjaan Utama
- Pendapatan Sebulan Terakhir
- Keterampilan Khusus/Sertifikat Keahlian

#### **D. KEPEMILIKAN USAHA** (6 pertanyaan)
- Apakah Memiliki Usaha Sendiri/Bersama?
- Berapa Usaha yang Dimiliki?
- Lapangan Usaha dari Usaha Utama
- Jumlah Pekerja yang Dibayar
- Jumlah Pekerja yang Tidak Dibayar
- Omzet Usaha Utama

#### **E. KESEHATAN** (3 pertanyaan)
- Status Hamil (untuk perempuan)
- Penyandang Disabilitas
- Penyakit Menahun Kronis

### 📊 **TOTAL PERTANYAAN**
- **Form Keluarga**: 60 pertanyaan
- **Form Individu**: 44 pertanyaan (termasuk foto KK baru conditional)
- **Total**: 104 pertanyaan komprehensif
- **100% sesuai** dengan header Google Sheets

---

## 📋 REQUIREMENTS

- Node.js (v16 atau lebih baru)
- npm atau yarn
- Expo Go app (untuk testing di mobile)
- Google Sheets dengan Apps Script

---

## 🔧 INSTALASI

### 1. Clone & Install
```bash
git clone [repository-url]
cd dtsen
npm install
```

### 2. Setup Google Apps Script

**File yang digunakan**: `GOOGLE_APPS_SCRIPT_COMPLETE.js`

Script ini sudah lengkap dengan:
- ✅ Session management
- ✅ User authentication
- ✅ Data operations (CRUD)
- ✅ **Update checker**

**Setup:**
1. Buka Google Sheets Anda
2. Extensions → Apps Script
3. Copy semua kode dari `GOOGLE_APPS_SCRIPT_COMPLETE.js`
4. Paste ke Apps Script Editor (hapus kode lama)
5. Buat sheet baru: `SESSIONS` dengan header sesuai komentar di file
6. Buat sheet baru: `APP_VERSION` dengan header: `VERSION | DOWNLOAD_URL | RELEASE_NOTES | FORCE_UPDATE | UPDATED_AT`
7. **Buat sheet `KELUARGA`** dengan 60 kolom sesuai form keluarga
8. **Buat sheet `INDIVIDU`** dengan 43 kolom sesuai form individu
9. Deploy sebagai Web App (Execute as: Me, Who has access: Anyone)
10. Copy URL deployment

### 3. Update URL

Edit `app.json` dengan URL deployment Anda:
```json
{
  "expo": {
    "extra": {
      "GOOGLE_SHEETS_URL": "https://script.google.com/macros/s/YOUR_SCRIPT_ID/exec"
    }
  }
}
```

### 4. Run Aplikasi

**Development:**
```bash
npm start
# atau
npm run dev
```

**Android Preview:**
```bash
npm run android
```

Scan QR code dengan Expo Go app atau gunakan Android emulator.

---

## ⚠️ TROUBLESHOOTING

### 🚨 **Critical Error Fixes (v5.1.4)**

**Error: "Network request failed" & "Invalid image URI format"**
- **Penyebab**: Sistem cache foto yang kompleks menyebabkan konflik URI dan network errors
- **Solusi**: ✅ **SUDAH DIPERBAIKI** - Mengganti dengan sistem direct upload yang sederhana seperti Individu
- **Prevention**: Menggunakan direct upload tanpa cache kompleks untuk stabilitas maksimal

**Error: "Missing catch or finally clause"**
- **Penyebab**: Syntax error di `update-keluarga.tsx` karena try block yang tidak lengkap
- **Solusi**: ✅ **SUDAH DIPERBAIKI** - Menambahkan catch/finally clause yang proper
- **Prevention**: Code review yang lebih ketat untuk syntax validation

**Error: "Format tanggal YYYY-MM-DD"**
- **Penyebab**: Format tanggal yang tidak konsisten dan tidak user-friendly
- **Solusi**: ✅ **SUDAH DIPERBAIKI** - Menggunakan format DD-MM-YYYY dengan date picker kalender
- **Prevention**: Standardisasi format tanggal di seluruh aplikasi

**Error: "Foto tidak ikut terhapus saat delete data"**
- **Penyebab**: Fungsi delete data tidak menghapus foto dari Google Drive
- **Solusi**: ✅ **SUDAH DIPERBAIKI** - Implementasi delete foto otomatis sebelum delete data
- **Prevention**: Enhanced delete system dengan photo cleanup otomatis

**New Photo System Features:**
- **Separated Services**: 14 service foto terpisah untuk maintainability
- **Direct Upload**: Sistem upload langsung tanpa cache kompleks
- **Photo Preview**: Preview foto baru sebelum update data
- **Photo Reset**: Reset otomatis jika batal atau gagal update
- **Enhanced Delete**: Foto otomatis terhapus dari Google Drive saat delete data

### 🚨 **Previous Critical Error Fixes (v5.1.3 Hotfix)**

**Error: "Cannot set property 'FOTO KTP/KK ASLI' of undefined"**
- **Penyebab**: Objek `updatedData.fields` bernilai undefined saat mengatur properti foto
- **Solusi**: ✅ **SUDAH DIPERBAIKI** - Menambahkan null safety checks dan inisialisasi `updatedData.fields = {}` jika undefined
- **Prevention**: Validasi struktur data sebelum property assignment

**Error: "Property 'hideSaving' doesn't exist"**
- **Penyebab**: Menggunakan method `hideSaving()` yang tidak ada di useLoading hook
- **Solusi**: ✅ **SUDAH DIPERBAIKI** - Mengganti semua `hideSaving()` dengan `hideLoading()` yang benar
- **Prevention**: Konsistensi penggunaan method dari hook yang benar

**Error: "Text strings must be rendered within a <Text> component"**
- **Penyebab**: JSX comment yang tidak tepat atau string yang tidak dibungkus dengan <Text>
- **Solusi**: ✅ **SUDAH DIPERBAIKI** - Menghapus comment bermasalah dan menambahkan SafeText component
- **Prevention**: Gunakan SafeText component untuk semua text rendering

**Error: showError function parameter validation**
- **Penyebab**: Fungsi `showError` memerlukan 2 parameter (title, message) tetapi hanya diberikan 1
- **Solusi**: ✅ **SUDAH DIPERBAIKI** - Memisahkan parameter menjadi title dan message yang terpisah
- **Prevention**: Selalu gunakan format `showError('Title', 'Message')` yang benar

**New Safety Components Added:**
- **DataErrorBoundary**: Menangkap text rendering errors secara otomatis
- **SafeText**: Wrapper aman untuk semua text rendering, mencegah undefined/null values

### 🔐 **Authentication Issues**

**Login Error: "JSON Parse error"**
- **Solusi**: Deploy ulang `GOOGLE_APPS_SCRIPT_COMPLETE.js` sebagai Web App
- **Check**: URL di `app.json` harus benar dan accessible

**Session Expired**
- **Solusi**: Login ulang, session berlaku 1 jam
- **Check**: Pastikan device time/date benar
- **Auto-cleanup**: Trigger berjalan setiap 1 jam untuk cleanup otomatis

### 📊 **Data Issues**

**Data Tidak Muncul**
- **Solusi**: Test URL Google Apps Script di browser
- **Expected**: Return JSON dengan `success: true`
- **Check**: Permission Google Apps Script (Execute as: Me, Anyone can access)

**Form Tidak Bisa Submit**
- **Solusi**: Check network connection dan Google Apps Script status
- **Check**: Console log untuk error details
- **Validasi**: Pastikan field wajib sudah diisi (NO KK, NAMA KK/NAMA LENGKAP, DUSUN)

---

## 📈 VERSION HISTORY

| Version | Date | Description |
|---------|------|-------------|
| **5.2.8** | Mar 2026 | 🗑️ Dashboard Optimization: menghapus tabel Status Sinkronisasi, dashboard lebih fokus |
| **5.2.6** | Mar 2026 | ⚡ Performance: optimasi loading, tab caching, online users fix, bug report manager |
| **5.2.5** | Mar 2026 | 🎨 UI/UX Improvements: konsistensi header, tab bar modern |
| **5.2.0** | Jan 2026 | 🎨 UI/UX Improvements: konsistensi header, NotificationBell di semua menu |
| **5.1.9** | Jan 2026 | 🔧 Migrasi akun Expo baru: owner hikmal_zerozeerozeven |
| **5.1.8** | Jan 2026 | � Fix APK Install & Field Mapping: multiple install methods |
| **5.1.7** | Jan 2026 | 📥 Fix In-App Download & GitHub Releases Support |
| **5.1.6** | Jan 2026 | 📥 Popup Download Progress & GitHub Releases Support |
| **5.1.5** | Jan 2026 | ⚙️ Centralized Settings System & Session Management |
| **5.1.4** | Jan 2026 | 📸 Major Photo System Overhaul: separated services, direct upload, date picker calendar |
| **5.1.3** | Jan 2026 | 🌐 Smart Network Status Bar dengan real-time detection & ping measurement |
| **5.1.2** | Jan 2026 | � Notifikasi koordinasi SIKS-NG & Cek Update Otomatis |
| **5.1.1** | Jan 2026 | � Upload foto KK baru di form individu jika pindah KK |
| **5.1.0** | Dec 2025 | � Admin Notes feature in card list, family-individual sync |
| **5.0.0** | Dec 2025 | 🐛 Critical bug fixes, auto scroll implementation, field organization |
| **4.9.0** | Dec 2025 | 🔧 Build system fixes, automated version sync |
| **4.8.0** | Dec 2025 | 🔧 TypeScript fixes, enhanced type safety |
| **4.0.0** | Dec 2025 | 🎉 Complete app refactoring, enhanced stability |

---

## 🔑 DEFAULT LOGIN

Setelah setup, gunakan kredensial default:
- **Username**: admin
- **Password**: admin123

⚠️ **Penting**: Ganti password setelah login pertama!

---

## 📞 SUPPORT

Jika ada masalah:
1. Lihat section **TROUBLESHOOTING** di atas
2. Cek console log di aplikasi (tekan `j` di Expo terminal)
3. Test URL Google Apps Script di browser
4. Verifikasi permission di Google Apps Script (Execute as: Me, Who has access: Anyone)

---

## 📝 LICENSE

Private project - All rights reserved

---

**Dibuat dengan ❤️ untuk DTSEN**
