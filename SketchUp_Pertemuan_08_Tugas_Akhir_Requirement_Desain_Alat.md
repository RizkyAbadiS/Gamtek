# SketchUp Pertemuan 8 - Proyek: Desain Alat Berbasis Requirement

Pertemuan ini berisi panduan proyek. Anggap ini sebagai tutorial lengkap: mulai dari memilih tema, menyiapkan komponen dummy, menentukan ukuran, merapikan struktur file, membuat scene, memberi dimensi, sampai mengekspor gambar.

Yang Anda kejar bukan detail bentuk yang rumit, tetapi desain yang rapi, masuk akal, dan mudah direview.

Jika Anda memakai aset import, itu boleh, tetapi Anda tetap harus menjaga kerapian model dan mencatat sumber aset. Lampiran import dan sumber aset terpercaya ada di:
`SketchUp_Lampiran_Import_dan_Sumber_Aset.md`

---

## Langkah 0 - Pilih tema proyek (pilih satu)
Pilih satu tema agar fokus:
1) Alat Monitoring: enclosure berisi PCB dummy, indikator (LED/layar dummy), konektor daya, dan jalur kabel.
2) Mini Panel Kontrol: panel kecil berisi MCB/terminal (dummy), DIN rail, tray/duct (dummy), dan jalur kabel masuk/keluar.

Setelah memilih tema, tulis satu kalimat "alat ini untuk apa" agar Anda punya arah saat menyusun layout.

Kalimat ini akan membantu Anda menentukan prioritas. Contoh: jika alat untuk monitoring, posisi konektor dan jalur kabel akan lebih penting daripada detail estetika.

---

## Checklist spesifikasi yang harus ada (sebagai pegangan saat membuat)
Pastikan desain Anda memiliki:
1) Unit mm dan dimensi utama (panjang, lebar, tinggi)
2) Struktur rapi: semua bagian Group/Component, Outliner jelas
3) Tags minimal: `Enclosure`, `Komponen`, `Jalur`, `Anotasi`
4) Minimal 3 komponen internal dummy + konsep mounting
5) Ada konsep clearance kabel/akses
6) Minimal 4 scene wajib + ekspor PNG dari scene tersebut

Catatan penting: edges/faces tetap Untagged. Tag hanya untuk Group/Component.

Jika Anda mengunduh model dari internet, biasakan menyimpan file aset di folder `Aset_Import` dan mencatat link sumbernya. Ini akan memudahkan Anda saat ditanya "model ini dari mana" atau saat Anda perlu mengganti aset yang terlalu berat.

---

## Tutorial langkah demi langkah

### Langkah 1 - Buat komponen dummy (mulai dari isi)
Buat minimal tiga component dummy sesuai tema Anda. Contoh:
- PCB (misalnya 100 x 70 x 1.6 mm)
- Konektor daya (bentuk sederhana)
- Indikator atau MCB/terminal (bentuk sederhana)

Beri nama component dengan jelas. Hindari nama default.

Saran praktis: gunakan dummy sederhana lebih dulu agar layout cepat jadi. Setelah layout jelas, baru Anda memutuskan apakah perlu mengganti dummy dengan model import yang lebih representatif.

### Langkah 2 - Susun layout internal/top layout
1) Susun komponen di posisi yang masuk akal.
2) Pastikan ada ruang untuk kabel di dekat konektor (clearance).
3) Pastikan akses pemasangan masuk akal (misalnya cover bisa dibuka, komponen tidak menghalangi).

Jika Anda bingung, buat `S04_Top_Layout` lebih awal agar layout mudah dicek.

### Langkah 3 - Tentukan ukuran enclosure/panel berdasarkan layout
1) Ukur kebutuhan ruang komponen.
2) Tambahkan ruang untuk dinding (misalnya 3 mm) dan ruang kabel.
3) Tentukan ukuran luar (tulis angka yang Anda pilih).

Kuncinya: ukuran harus punya alasan, bukan tebak-tebakan.

### Langkah 4 - Buat enclosure/panel (body + cover)
1) Buat body sesuai ukuran luar.
2) Buat tebal dinding (misalnya offset 3 mm) lalu kosongkan interior.
3) Buat cover terpisah (ketebalan 3-5 mm).
4) Bungkus body dan cover sebagai Group/Component terpisah.

### Langkah 5 - Tambahkan mounting (konsep)
Pilih sesuai kebutuhan tema:
- standoff PCB,
- rail/plate untuk komponen panel,
- dudukan sederhana untuk konektor.

Tidak perlu detail ulir. Yang penting masuk akal dan terlihat jelas di section.

### Langkah 6 - Rapikan Outliner dan Tags
1) Pastikan semua objek penting sudah Group/Component.
2) Rapikan nama di Outliner (misalnya `Body`, `Cover`, `PCB`, `Connector`, `MCB`).
3) Buat/assign tags:
   - `Enclosure` untuk body/cover
   - `Komponen` untuk isi
   - `Jalur` untuk tray/conduit/jalur kabel (konseptual)
   - `Anotasi` untuk dimensi dan label

### Langkah 7 - Buat 4 scene wajib (pakai nama ini)
Buat dan beri nama scene berikut:
1) `S01_Iso_Luar`
2) `S02_Iso_Dalam` (cover disembunyikan)
3) `S03_Section`
4) `S04_Top_Layout`

Tips:
- Buat `S02_Iso_Dalam` dengan menyembunyikan cover (hide) atau mematikan tag cover.
- Pastikan `S03_Section` memperlihatkan mounting dan ruang kabel.

### Langkah 8 - Tambahkan dimensi dan label
1) Tambahkan minimal 8 dimensi kunci:
   - dimensi utama enclosure/panel,
   - posisi komponen penting,
   - jarak/clearance yang relevan.
2) Tambahkan minimal 5 label:
   - nama komponen + fungsi singkat.

Pastikan dimensi dan label tidak saling bertumpuk.

### Langkah 9 - Ekspor PNG dari scene
Ekspor minimal 4 PNG (satu untuk tiap scene wajib), dengan nama yang jelas, misalnya:
- `GT_SKP_P8_Nama_NIM_S01_Iso_Luar.png`
- `GT_SKP_P8_Nama_NIM_S02_Iso_Dalam.png`
- `GT_SKP_P8_Nama_NIM_S03_Section.png`
- `GT_SKP_P8_Nama_NIM_S04_Top_Layout.png`

### Langkah 10 - Rapikan paket pengumpulan
Simpan file utama:
- `GT_SKP_P8_Nama_NIM.skp`

Buat folder ekspor:
- `GT_SKP_P8_Nama_NIM_Export` (isi PNG)

Tambahkan satu dokumen ringkas (maksimal 1 halaman), misalnya:
- `GT_SKP_P8_Nama_NIM_Spesifikasi.md`

Isi dokumen ringkas cukup:
1) tema proyek,
2) asumsi ukuran komponen dummy,
3) 3 keputusan desain dan alasannya (misalnya ukuran enclosure, posisi konektor, rute kabel).

Jika Anda memakai aset import, tambahkan satu poin lagi di dokumen:
4) daftar sumber aset (nama situs + link).

---

## Jika mengalami masalah (troubleshooting)
- Model terasa "pecah" saat tag dimatikan: pastikan edges/faces tetap Untagged dan semua geometri dibungkus.
- Scene tidak konsisten: buat scene setelah view benar-benar siap, lalu jangan ubah scene tanpa sengaja.
- Sulit menjelaskan ruang kabel: tampilkan lewat section dan beri satu dimensi atau label "clearance".

---

## Latihan tambahan (opsional)
1) Buat scene `S05_Exploded` untuk memperjelas bagian-bagian.
2) Tambahkan jalur kabel konseptual (garis/tray sederhana) dan taruh di tag `Jalur`.
