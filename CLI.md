## 🧩 Flutter CLI
---

<Details>
  <summary><b> Debug Mode (Default Mode)</b></summary><br>
  
- Mengecek instalasi Flutter, SDK, Android Studio, device, dll:   
  ```
  flutter doctor
  ```   
- Membuat proyek Flutter baru:   
  ```
  flutter create <nama_proyek>
  ```   
- Menjalankan aplikasi dengan memilih perangkat:   
  ```
  flutter run
  ```   
- Menentukan perangkat target (contoh: ``flutter run -d chrome``):   
  ```
  flutter run -d <device>
  ```   
- Membangun file .apk untuk Android:  
  ```
  flutter build apk
  ```   
- Membangun file ``.aab`` untuk Play Store:   
  ```
  flutter build appbundle
  ```   
- Membangun aplikasi untuk web:   
  ```
  flutter build web
  ```   
- Mengambil semua dependency dari pubspec.yaml:   
  ```
  flutter pub get
  ```   
- Memperbarui dependency ke versi terbaru:   
  ```
  flutter pub upgrade
  ```   
- Menghapus cache build dan file sementara:   
  ```
  flutter clean
  ```   
- Menjalankan unit test di proyek:   
  ```
  flutter test
  ```   
...
</Details>

<Details>
  <summary><b> Profile Mode</b></summary><br>
  
- Menjalankan aplikasi di mode profile:   
  ```
  flutter run --profile
  ```   
- Menentukan perangkat target (contoh: Windows):   
  ```
  flutter run --profile -d windows
  ```   
- Membangun file .apk untuk Android (profile build):   
  ```
  flutter build apk --profile
  ```   
- Membangun aplikasi untuk web (profile build):   
  ```
  flutter build web --profile
  ```   
- Membangun aplikasi desktop untuk uji performa:   
  ```
  flutter build windows --profile
  ```   
</Details>   

<Details>
  <summary><b> Release Mode</b></summary><br>    

**`--release` artinya: “jalankan aplikasi dengan performa maksimal untuk produksi.”**
- Menjalankan release mode di windows:   
  ```
  flutter run --release -d windows
  ```    
- Membangun aplikasi untuk windows:  
  ```
  flutter build windows --release
  ```   
...   
</Details>  


| Mode    | Command                           | Target                   | Bisa Inspect | Catatan                                       |
| ------- | --------------------------------- | ------------------------ | ------------ | --------------------------------------------- |
| Debug   | `flutter run -d chrome`           | Browser (JS mode)        | ✅            | Hot reload aktif                              |
| Profile | `flutter run --profile -d chrome` | Browser (profiling mode) | ✅            | Untuk uji performa                            |
| Release | `flutter build chrome --release`     | Build web final          | ❌            | Sudah optimisasi penuh, tidak ada profil data |
