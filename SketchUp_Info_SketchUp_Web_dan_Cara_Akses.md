# SketchUp Web - Ketersediaan dan Cara Akses

File ini menjelaskan opsi SketchUp berbasis web (SketchUp for Web): kapan cocok dipakai, bagaimana cara mengaksesnya, dan hal-hal yang perlu Anda perhatikan saat dipakai untuk praktikum.

---

## 1) Apa itu SketchUp for Web?
SketchUp for Web adalah versi SketchUp yang berjalan di browser. Anda bisa mulai memodel tanpa instalasi aplikasi desktop. Versi web ini memakai teknologi inti yang sama, tetapi tampilannya lebih sederhana dibanding desktop.

SketchUp for Web bisa dipakai tanpa berlangganan, tetapi tetap membutuhkan akun (Trimble ID) untuk masuk.

---

## 2) Kapan SketchUp Web cocok untuk perkuliahan?
SketchUp Web biasanya cocok jika:
1) Mahasiswa tidak bisa install aplikasi (laptop terbatas / lab tidak mengizinkan instalasi).
2) Anda ingin cepat mulai praktik tanpa setup panjang.
3) Fokus materi adalah fundamental (gambar presisi, group/component, tags, scenes, dimensi dasar, export PNG).

SketchUp Web kurang cocok jika:
1) Materi butuh workflow desktop tertentu, plugin/extension khusus, atau fitur lanjutan tertentu.
2) Koneksi internet sering tidak stabil (karena akses dan simpan berbasis web).

---

## 3) Syarat minimal (agar lancar dipakai)
1) Browser modern. Disarankan versi terbaru Chrome, Firefox, atau Microsoft Edge.
2) Mouse dan keyboard (lebih nyaman untuk orbit/zoom dan presisi).
3) Trimble ID untuk login.

Catatan: SketchUp for Web memanfaatkan teknologi browser modern (WebAssembly) dan mesin grafis baru yang memeriksa dukungan WebGPU. Pada perangkat tertentu, performa bisa berbeda.

---

## 4) Cara akses (step-by-step)

### Langkah 1 - Buka SketchUp for Web
Ada dua cara umum:
1) Buka halaman produk SketchUp for Web, lalu pilih tombol untuk mulai memodel.
   - `https://www.sketchup.com/en/products/sketchup-for-web`
2) Jika Anda sudah tahu halaman aplikasi web-nya, Anda bisa langsung masuk lewat halaman SketchUp for Web (Home) dan login dari sana.

### Langkah 2 - Login menggunakan Trimble ID
1) Klik Sign In.
2) Masuk dengan Trimble ID (email/username) atau metode login pihak ketiga (Google/Apple/Microsoft) jika Anda memakainya.
3) Jika belum punya, buat Trimble ID terlebih dulu.

Trimble ID adalah akun yang dipakai untuk layanan SketchUp online (termasuk Trimble Connect).

### Langkah 3 - Buat model baru dan pilih unit (mm)
Saat masuk, Anda akan melihat halaman Home.
1) Klik Create New.
2) Pilih template/unit yang sesuai (untuk kelas ini, pilih mm jika tersedia).

Jika perlu mengganti unit default, Anda bisa mengubahnya melalui App Settings (pengaturan aplikasi).

---

## 5) Menyimpan file (Trimble Connect) dan mengunduh salinan lokal
SketchUp for Web menyimpan model ke Trimble Connect. Setelah penyimpanan pertama, SketchUp for Web juga melakukan auto-save berkala dan membuat revision history.

Jika Anda ingin menyimpan file di laptop (misalnya untuk dikumpulkan):
1) Buka model.
2) Buka Menu.
3) Pilih Download.
4) Pilih format yang dibutuhkan (misalnya .skp atau .png).

Saran praktis untuk kelas:
- Tetap biasakan penamaan file sesuai format tugas (misalnya `GT_SKP_Px_Nama_NIM.skp`).
- Simpan juga hasil export PNG per scene untuk dokumentasi presentasi.

---

## 6) Import file di SketchUp Web (catatan penting)
SketchUp Web tidak memiliki akses bebas ke seluruh file system seperti aplikasi desktop. Karena itu, import/export tertentu punya aturan khusus, terutama untuk model yang membawa tekstur.

Untuk panduan import yang rapi + daftar sumber aset terpercaya, baca:
`SketchUp_Lampiran_Import_dan_Sumber_Aset.md`

---

## 7) Berbagi hasil tanpa mengirim file .skp (opsional)
Jika Anda ingin teman/kelompok lain melihat model tanpa risiko mengedit, Anda bisa memakai Link Sharing dari model yang tersimpan di Trimble Connect. Link yang dibagikan bersifat view-only dan dapat dimatikan kapan saja.

Ini berguna untuk:
1) review antar kelompok,
2) mengumpulkan progress,
3) presentasi berbasis link.

---

## 8) Rekomendasi singkat untuk dosen/asisten
Jika Anda mengizinkan SketchUp Web untuk tugas:
1) Pastikan langkah-langkah tugas tidak bergantung pada fitur yang hanya ada di desktop.
2) Minta mahasiswa selalu cek unit (mm) sejak awal.
3) Anjurkan aset import yang ringan agar browser tidak berat.
4) Tekankan kerapian: group/component, tags, outliner, scene, dan export PNG.

---

## Referensi resmi (untuk dibaca bila perlu)
- Downloading SketchUp (menyebut SketchUp for Web bisa dipakai tanpa download): `https://help.sketchup.com/en/downloading-sketchup`
- SketchUp for Web - What You Need (browser, Trimble ID, catatan grafis): `https://help.sketchup.com/en/sketchup-web/what-you-need`
- Creating and Editing Models (Create New, unit, catatan subscription): `https://help.sketchup.com/en/sketchup-web/creating-and-editing-models`
- Saving Models (Trimble Connect, autosave, download file): `https://help.sketchup.com/en/sketchup-web/saving-models`
- File Management (aturan import/export tertentu di web): `https://help.sketchup.com/en/sketchup-web/file-management`
- Link Sharing (view-only link): `https://help.sketchup.com/en/sketchup-web/link-sharing`

