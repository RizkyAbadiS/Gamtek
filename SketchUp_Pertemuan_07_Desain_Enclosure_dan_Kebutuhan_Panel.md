# SketchUp Pertemuan 7 - Desain Enclosure/Panel yang Siap Direview

Pertemuan ini adalah latihan sebelum tugas requirement. Fokusnya: membuat enclosure/panel dengan cara yang benar, yaitu **komponen dulu, baru casing**. Anda akan membuat dummy komponen internal, menyusun layout, menentukan ukuran enclosure berdasarkan layout tersebut, lalu menyiapkan scene untuk review.

Kalau Anda terbiasa memulai dari komponen, desain Anda akan lebih masuk akal dan lebih mudah dijelaskan. Sebaliknya, jika Anda memulai dari casing, sering kali casing jadi "asal muat" dan keputusan desain sulit dipertanggungjawabkan.

---

## Sebelum mulai (wajib)
1) Buat file baru (mm).
2) Tentukan skenario yang akan Anda pakai (pilih satu):
   - Kotak kontrol mini (MCB + terminal dummy)
   - Kotak alat IoT (PCB + indikator + konektor dummy)

Anda boleh menggambar dummy sendiri atau import dari sumber terpercaya. Jika Anda memilih import, lakukan dengan prosedur yang rapi (cek lisensi, cek skala, bungkus menjadi component, sederhanakan). Panduan dan sumber ada di:
`SketchUp_Lampiran_Import_dan_Sumber_Aset.md`

---

## Hasil akhir yang harus jadi
1) Minimal 3 komponen dummy di dalam enclosure
2) Enclosure body + cover terpisah
3) Ada konsep mounting (standoff/rail/plate) dan ruang kabel (clearance)
4) Minimal 3 scene: luar, dalam (cover hidden), section
5) Minimal 2 PNG ekspor (luar dan dalam/section)

---

## Tutorial langkah demi langkah

### Langkah 1 - Buat dummy komponen (mulai dari isi)
Buat minimal tiga component dummy. Contoh yang aman:
1) PCB: 100 x 70 x 1.6 mm
2) Konektor daya: bentuk sederhana
3) Indikator atau MCB/terminal: bentuk sederhana

Tips:
1) Jadikan masing-masing sebagai Component.
2) Beri nama yang jelas (misalnya `PCB`, `DC_Jack`, `MCB_1P_Dummy`).

Kalau Anda memakai import, usahakan satu komponen satu file referensi, lalu masukkan ke model proyek sebagai component. Ini membuat Anda mudah mengganti versi komponen jika di tengah jalan Anda menemukan model yang lebih rapi.

### Langkah 2 - Susun layout internal
1) Letakkan komponen dummy pada posisi yang masuk akal.
2) Sisakan ruang untuk kabel di dekat konektor (misalnya 10-15 mm area bebas).
3) Pastikan tidak ada komponen saling bertabrakan.

Checkpoint: kalau cover nanti ditutup, komponen tetap punya ruang (tidak mentok dinding).

### Langkah 3 - Tentukan ukuran enclosure berdasarkan layout
1) Bayangkan dinding enclosure mengelilingi layout komponen.
2) Tentukan ukuran luar enclosure.
   - Anda boleh mulai dari 220 x 160 x 90 mm lalu sesuaikan.

Catatan: ukuran yang baik adalah ukuran yang punya alasan (komponen + ruang kabel + tebal dinding).

Di titik ini, cobalah menuliskan 2-3 alasan singkat kenapa ukuran Anda seperti itu. Ini akan membantu Anda saat presentasi: Anda tidak sekadar menyebut angka, tetapi menjelaskan logikanya.

### Langkah 4 - Buat body enclosure dengan tebal dinding 3 mm
1) Buat balok luar sesuai ukuran yang Anda pilih.
2) Offset 3 mm ke dalam pada face atas.
3) Push/Pull bagian dalam ke bawah untuk mengosongkan interior.
4) Bungkus body menjadi Group/Component terpisah.

### Langkah 5 - Buat cover terpisah
1) Buat cover di bagian atas (ketebalan 3-5 mm).
2) Bungkus cover menjadi Group/Component terpisah.
3) Pastikan cover bisa disembunyikan tanpa memengaruhi body.

### Langkah 6 - Buat mounting (konsep)
Pilih salah satu atau gabungkan:
1) Standoff PCB: 4 silinder kecil di bawah PCB.
2) Plate/rail sederhana untuk komponen panel.

Tidak perlu detail ulir. Fokusnya menunjukkan cara pemasangan masuk akal.

### Langkah 7 - Buat scene untuk review
Buat minimal tiga scene:
1) `S01_Iso_Luar` (overview)
2) `S02_Iso_Dalam` (cover disembunyikan)
3) `S03_Section` (penampang yang memperlihatkan ruang dan mounting)

### Langkah 8 - Simpan dan ekspor
1) Simpan: `GT_SKP_P7_Nama_NIM.skp`
2) Ekspor minimal dua PNG:
   - `S01_Iso_Luar`
   - `S02_Iso_Dalam` atau `S03_Section`

---

## Jika mengalami masalah (troubleshooting)
- Enclosure dibuat duluan dan komponen tidak muat: ulangi workflow yang benar, komponen dulu baru casing.
- Cover menempel ke body: pastikan cover dibungkus dan dipisah.
- Sulit menilai ruang kabel: buat label "clearance" atau tampilkan lewat section.

---

## Latihan tambahan (opsional)
1) Tambahkan boss dan lubang sekrup cover secara sederhana (tanpa ulir).
2) Buat satu scene tambahan `S04_Exploded` dengan cover dan komponen sedikit digeser agar struktur lebih jelas.
