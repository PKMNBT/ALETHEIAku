[README-PANDUAN.md](https://github.com/user-attachments/files/34221376/README-PANDUAN.md)
# ALETHEIAku PWA

Paket siap deploy berisi aplikasi, manifest PWA, ikon Android, service worker, dan konfigurasi Firebase Hosting.

## GitHub Pages
Buat repository `alethia-ku`, upload seluruh isi folder paket ke root, lalu aktifkan Settings > Pages > Deploy from a branch > main > /(root).

## Firebase Hosting
1. Buat project di Firebase Console.
2. Instal CLI: `npm install -g firebase-tools`
3. Login: `firebase login`
4. Di folder ini jalankan `firebase init hosting`, pilih project, public directory `.`
5. Jalankan `firebase deploy`.

## Catatan
- Riwayat saat ini tersimpan di localStorage perangkat/browser. Hapus riwayat akan menghapus semua skor dan statistik dashboard pada perangkat tersebut.
- Firebase Hosting hanya menerbitkan situs. Sinkronisasi nilai antarperangkat memerlukan konfigurasi Firebase Authentication + Cloud Firestore dan aturan keamanan. Belum diaktifkan karena memerlukan project Firebase milik pemilik aplikasi.
- Pemasangan PWA Android memerlukan situs HTTPS. Buka situs di Chrome Android > menu ⋮ > Tambahkan ke layar utama / Install app.


## Preview interaktif iPhone 17
Panel Preview di bagian atas memuat aplikasi yang sama melalui iframe dengan query `?preview=1`. Seluruh tombol dan menu di dalam preview aktif dan menggunakan penyimpanan browser/origin yang sama. Bingkai iPhone 17 hanya mockup perangkat; aplikasi tetap berjalan sebagai web app.


## V9 — Ukuran preview disesuaikan
Bingkai preview iPhone 17 di layar laptop diperkecil menjadi sekitar 290 × 610 px. Pada layar sempit, bingkai tetap responsif agar muat di layar.


## V10 — Label preview netral
Label pada aplikasi menggunakan 'Preview Tampilan HP'. Bingkai perangkat tetap sebagai ilustrasi visual; aplikasi tetap responsif dan kompatibel lintas perangkat.


## V11 — Narasi preview diringkas
Keterangan penjelas di bawah judul dan bingkai preview dihapus sesuai permintaan. Fungsi preview tetap interaktif.
