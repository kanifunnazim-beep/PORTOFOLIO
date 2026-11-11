# Portofolio Moch. Zaim Zidan KN

Website statis interaktif berdasarkan isi dan dokumentasi PPT yang diberikan. Dibuat dengan HTML, CSS, dan JavaScript murni. Tidak memerlukan npm, proses build, database, atau API key.

## Membuka di komputer

Ekstrak ZIP, lalu buka index.html di Chrome, Edge, atau Firefox terbaru. Untuk preview melalui localhost, buka folder ini di VS Code dan gunakan Live Server. Fitur salin email paling andal pada HTTPS atau localhost.

## Hosting melalui GitHub Pages

1. Masuk ke GitHub dan buat repository baru, misalnya `zaim-portfolio`. Pilih Public jika menggunakan GitHub Free.
2. Buka repository, pilih **Add file > Upload files**.
3. Unggah **isi folder hasil ekstraksi**, bukan ZIP. `index.html`, `style.css`, `script.js`, dan folder `assets` harus ada langsung di root repository. Jangan menaruh index.html di dalam folder tambahan.
4. Commit file ke branch `main`. File `.nojekyll` disertakan; jika tidak ikut saat drag-and-drop, buat file kosong bernama `.nojekyll` di root melalui Git atau editor GitHub.
5. Buka **Settings > Pages**.
6. Pada **Build and deployment**, pilih **Source: Deploy from a branch**.
7. Pilih **Branch: main** dan **Folder: / (root)**, kemudian **Save**.
8. Tunggu deployment selesai. GitHub menampilkan alamat website pada halaman Pages. Pola alamat project site: `https://USERNAME.github.io/zaim-portfolio/` (ganti USERNAME dan nama repository).
9. Jika belum muncul, periksa tab Actions dan pastikan index.html berada di root branch yang dipilih.

Panduan resmi: https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site

## Isi folder

- `index.html`: profil, pengalaman, karya, pendidikan, sertifikasi, kontak.
- `style.css`: desain responsif, mode gelap/terang, dan tampilan dialog.
- `script.js`: filter karya, detail proyek, galeri foto, tema, menu mobile, dan salin email.
- `assets/`: foto dan dokumen asli dari PPT, favicon, serta PPT untuk tombol unduh.
- `.nojekyll`: menghindari pemrosesan Jekyll.

## Mengedit konten

- Ubah profil, pendidikan, kontak, dan ringkasan kartu pada index.html.
- Ubah detail proyek pada objek `projects` di script.js; sesuaikan ringkasan di index.html agar konsisten.
- Ubah warna melalui variabel di awal style.css.
- Ganti foto di assets dengan nama yang sama atau ubah path pada HTML/JavaScript. Gunakan path relatif agar berfungsi pada subfolder repository GitHub Pages.
- Email dan WhatsApp sudah diisi sesuai PPT. Jika mengganti email, perbarui juga handler `copy-email` di script.js.
- Tombol unduh mengambil PPT asli yang disertakan, bukan CV PDF.

## Fitur

Navigasi bagian, filter dua kategori karya, dialog detail proyek, pembesaran foto dan sertifikat, mode terang/gelap tersimpan pada browser, menu mobile, email/WhatsApp/telepon, salin email, dan unduh portofolio. Dialog bisa ditutup dengan tombol silang atau Escape. Dukungan reduced motion dan fokus keyboard tersedia.

Dokumentasi dashboard adalah gambar dari PPT, bukan data langsung atau simulasi monitoring. Website belum dipublikasikan ke akun GitHub. Tidak ada formulir server; tombol kontak membuka aplikasi email atau WhatsApp.

## Pemeriksaan

Sintaks JavaScript dan seluruh tautan aset lokal diperiksa. Filter, kedua dialog proyek, galeri bertingkat, dan pergantian tema diuji pada browser desktop. CSS memiliki breakpoint 1000px dan 700px; pengujian pada perangkat ponsel fisik belum dilakukan.
