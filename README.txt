📘 Panduan BojonegoroMart_v1

1) Persiapan
   - Pastikan sudah memiliki akun Firebase dan proyek 'bojonegoromart'
   - Install Firebase CLI: npm install -g firebase-tools
   - Login: firebase login

2) Struktur folder (sudah disiapkan)
   BojonegoroMart_v1/
   ├─ index.html
   ├─ 404.html
   ├─ manifest.json
   ├─ service-worker.js
   ├─ firebase.json
   ├─ README.txt
   └─ assets/
      ├─ logo/logo.png
      └─ icons/
         ├─ icon-512.png
         └─ favicon.ico

3) Deploy
   - Buka terminal di folder BojonegoroMart_v1
   - Inisialisasi hosting (jika belum):
       firebase init hosting
     Pilih project 'bojonegoromart', public directory -> '.', configure as SPA -> y, overwrite index.html -> n
   - Deploy:
       firebase deploy

4) Catatan
   - Upload gambar produk disimpan di Firebase Storage pada folder 'products/{uid}/'
   - Service worker membuat cache ringan hanya untuk index & aset utama
   - Untuk memperbarui logo/gambar, ganti file di assets/ dan redeploy

Dibuat otomatis — selamat deploy! 🚀
