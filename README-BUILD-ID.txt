JOS MOBILE - PROYEK ANDROID

Ini adalah proyek sumber Android Studio, BUKAN file APK siap instal.
Alamat backend yang digunakan: https://jasaokuselatan.rf.gd/
Package: id.jos.okuselatan

CARA BUILD DI WINDOWS 10:
1. Instal Android Studio versi stabil dan Android SDK Platform 35.
2. Ekstrak folder JOS-Android.
3. Buka Android Studio > Open > pilih folder JOS-Android.
4. Tunggu Gradle Sync selesai. Jika diminta, instal Android Gradle Plugin/SDK yang disarankan.
5. Pilih Build > Build Bundle(s) / APK(s) > Build APK(s).
6. APK debug hasil build berada di app/build/outputs/apk/debug/app-debug.apk.
7. Untuk distribusi publik, buat APK release yang ditandatangani melalui Build > Generate Signed Bundle / APK > APK.

CATATAN PENTING:
- Pastikan domain HTTPS benar dan website aktif sebelum build.
- Kamera dalam WebView belum diaktifkan otomatis; implementasi izin kamera native perlu diuji sesuai alur unggah/penggunaan kamera website.
- Pengujian wajib dilakukan pada beberapa perangkat Android, termasuk login, upload foto, pesanan, tombol kembali, dan tautan WhatsApp.
- File ini belum ditandatangani dan belum merupakan APK final.
