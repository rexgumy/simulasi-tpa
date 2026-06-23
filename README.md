# Simulasi CBT TPA

Halaman simulasi ujian Tes Potensial Akademik (TPA) berbasis web statis — 100 soal pilihan ganda (numerik, penalaran, spasial, verbal, bahasa Inggris, Ms. Office, Email), dengan timer, navigasi soal, opsi acak urutan, dan rekap hasil per kategori.

## Cara menjalankan secara lokal
Cukup buka `index.html` langsung di browser. Tidak ada dependensi atau proses build.

## Cara deploy ke GitHub Pages
1. Push isi folder ini (terutama `index.html`) ke branch `main` repo GitHub kamu.
2. Buka repo → **Settings → Pages**.
3. Pada bagian **Branch**, pilih `main` dan folder `/ (root)`, lalu klik **Save**.
4. Tunggu 1–2 menit, halaman akan aktif di:
   `https://<username-kamu>.github.io/<nama-repo>/`

## Mengubah soal
Edit array `ORIGINAL_QUESTIONS` di dalam `index.html`. Setiap soal memiliki struktur:
```js
{cat:"Numerik", text:"...", options:["...","...","...","...","..."], correct:0}
```
`correct` adalah index (mulai dari 0) dari opsi yang benar.

## Mengubah durasi default / jumlah soal per layar
Pengaturan durasi dan opsi acak soal bisa diubah langsung oleh pengguna di halaman pengantar sebelum ujian dimulai — tidak perlu edit kode.
