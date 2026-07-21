# Catatan keamanan repo ini

Repo ini **PUBLIK** karena dipakai buat hosting landing page + web app lewat GitHub Pages.

## Aturan keras
**JANGAN pernah taruh isi berbayar di sini**, walau nama filenya diacak.
GitHub nampilin **daftar isi folder** ke siapa saja (`api.github.com/repos/.../contents/<folder>`),
jadi "URL rahasia" itu ilusi: orang gak perlu nebak, tinggal baca daftarnya.

## Insiden 21 Jul 2026
- `akses/lengkap-*.html` dan `akses/premium-*.html` (berisi KODE AKSES produk berbayar) sempat ada di sini.
- `bonus/` (e-book + template khusus paket Premium) juga.
- Dampak: gate kode akses web app bisa dilewati siapa saja sebelum iklan pertama tayang.
- Kebetulan Genggam belum punya pembeli saat itu, jadi nol pembeli yang dirugikan.

## Yang dilakukan
1. Folder `akses/` dan `bonus/` dihapus dari repo.
2. Kedua kode akses **dirotasi**, hash SHA-256 di `app/index.html` diganti.
3. Panduan akses + kode sekarang dikirim lewat **teks delivery Scalev per varian** (cuma kelihatan pembeli yang bayar).

## Kalau butuh nambah bonus berbayar lagi
Pakai fitur file/attachment di Scalev, atau storage yang butuh autentikasi. Bukan repo ini.
