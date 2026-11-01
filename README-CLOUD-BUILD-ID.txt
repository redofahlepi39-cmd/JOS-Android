JOS ANDROID - PAKET SUMBER UNTUK CLOUD BUILD

Isi paket ini adalah proyek sumber Android WebView JOS, BUKAN APK siap instal.
Aplikasi membuka https://jasaokuselatan.rf.gd/ di dalam tampilan aplikasi tanpa kolom alamat browser.
Backend dan database tetap berada di website yang sudah ada.

FILE KONFIGURASI
- codemagic.yaml: workflow Codemagic untuk membangun APK debug.
- app/: kode sumber Android.
- build.gradle / settings.gradle: konfigurasi Gradle proyek.

CARA PAKAI DI CODEMAGIC
1. Ekstrak ZIP ini di komputer.
2. Buat repository GitHub baru bernama JOS-Android.
3. Upload ISI folder JOS-Android (bukan folder luarnya) ke repository. Pastikan codemagic.yaml berada di root repository, sejajar dengan settings.gradle dan build.gradle.
4. Buka https://codemagic.io/ lalu login dengan GitHub.
5. Tambahkan repository JOS-Android dan pilih workflow "JOS Android - APK Debug".
6. Jalankan Start new build.
7. Jika build berhasil, buka tab Artifacts dan unduh app-debug.apk.

CATATAN
- Workflow mengunduh Gradle 8.9 saat build; koneksi internet cloud diperlukan.
- Build debug memakai kunci debug otomatis. Cocok untuk uji coba, bukan distribusi produksi jangka panjang.
- APK harus diuji di HP Android. Uji login, menu, upload gambar/file, kamera, tombol kembali, WhatsApp, dan transaksi.
- Penggunaan kamera tergantung izin Android dan dukungan fitur di website.
- Jika Codemagic menampilkan error, kirim screenshot/log error agar konfigurasi dapat diperbaiki.
- Jangan unggah password, token, atau signing key ke repository publik.
