# SketchUp Pertemuan 6 - Layout Ruangan dan Jalur Instalasi

Pada pertemuan ini Anda tidak hanya memodelkan "benda", tetapi memodelkan **konteks pemasangan**. Untuk teknik elektro, konteks itu biasanya: ruangan, titik beban (lampu/saklar/stopkontak), dan jalur instalasi (tray/conduit). Model yang baik adalah model yang bisa menjelaskan rute instalasi dengan cepat.

Di kelas, Anda tidak dituntut membuat standar industri lengkap. Yang penting dari latihan ini: rute Anda masuk akal dan orang lain bisa memahami rute tersebut hanya dari scene dan tampilan model.

---

## Sebelum mulai (wajib)
1) Buat file baru (mm), atau lanjutkan dari file Anda jika ingin memasukkan panel sebelumnya.
2) Mulai rapi sejak awal: setiap bagian dijadikan Group/Component.

Jika Anda ingin memakai aset import untuk mempercepat (misalnya meja, lampu, atau lemari), boleh. Tetapi pilih aset yang ringan dan rapikan dulu (bungkus sebagai Component, cek skala, beri tag). Panduannya ada di:
`SketchUp_Lampiran_Import_dan_Sumber_Aset.md`

---

## Hasil akhir yang harus jadi
1) Ruangan sederhana ukuran 6000 x 4000 x 3000 mm
2) Minimal 2 lampu, 1 saklar, 2 stopkontak (sebagai component)
3) Jalur tray/conduit konseptual dari panel ke titik beban
4) Tags: `Arsitektur`, `Perangkat`, `Jalur`
5) Minimal 3 scene: Iso, Top, dan Jalur-only

---

## Tutorial langkah demi langkah

### Langkah 1 - Buat ruangan (Group)
1) Buat lantai 6000 x 4000 mm.
2) Buat dinding sampai tinggi 3000 mm.
3) Bungkus lantai + dinding menjadi **Group** bernama `Ruangan` (opsional tapi disarankan).

Checkpoint: ruangan terasa "masuk akal" skalanya (meteran menjadi ribuan mm, bukan puluhan).

### Langkah 2 - Buat component titik beban
Buat tiga component sederhana:
1) `Lampu`
2) `Saklar`
3) `Stopkontak`

Bentuknya tidak perlu detail, tetapi harus konsisten dan mudah dikenali.

Anda boleh membuat bentuk super sederhana (misalnya balok dan silinder). Di tahap ini, yang penting adalah "titik" dan "fungsi", bukan detail produk.

### Langkah 3 - Tempatkan titik beban
1) Duplikasi `Lampu` menjadi 2 buah dan tempatkan di plafon (atau tinggi yang Anda anggap plafon).
2) Tempatkan 1 `Saklar` di salah satu dinding.
3) Duplikasi `Stopkontak` menjadi 2 buah dan tempatkan pada dinding (ketinggian asumsi bebas, tetapi konsisten).

Jika Anda memakai asumsi, catat di label kecil atau cukup Anda ingat untuk dijelaskan saat presentasi.

### Langkah 4 - Tentukan lokasi panel (asumsi)
1) Tentukan satu titik pada dinding sebagai lokasi panel (boleh berupa kotak kecil sederhana).
2) Bungkus panel sebagai Group/Component.

### Langkah 5 - Gambar jalur instalasi (konseptual)
Cara yang paling mudah:
1) Gambar garis rute dari panel ke area titik beban (seperti sketsa jalur).
2) Ubah garis tersebut menjadi bentuk 3D sederhana (misalnya dengan memberi ketebalan/tray).
3) Buat belokan seperlunya.

Tujuannya rute mudah dipahami, bukan detail standar industri.

Jika Anda ingin jalur terlihat lebih jelas saat presentasi, buat jalur sedikit lebih tebal daripada skala aslinya. Di model konseptual, keterbacaan sering lebih penting daripada ketelitian bentuk tray.

### Langkah 6 - Organisasi dengan Tags
1) Buat tag: `Arsitektur`, `Perangkat`, `Jalur`.
2) Assign:
   - Ruangan -> `Arsitektur`
   - Lampu/saklar/stopkontak/panel -> `Perangkat`
   - Tray/conduit -> `Jalur`

Ingat: tag hanya untuk Group/Component.

### Langkah 7 - Buat scene untuk presentasi
Buat minimal tiga scene:
1) `S01_Iso` (overview)
2) `S02_Top` (membaca layout)
3) `S03_Jalur` (matikan tag lain, tampilkan jalur saja)

### Langkah 8 - Simpan dan dokumentasi
1) Simpan: `GT_SKP_P6_Nama_NIM.skp`
2) Ambil 3 screenshot sesuai scene.

---

## Jika mengalami masalah (troubleshooting)
- Skala ruangan terasa aneh: cek lagi unit mm. Ingat 6 m = 6000 mm.
- Jalur sulit dibaca: buat scene jalur-only dan matikan tag lain.
- Objek menempel: pastikan setiap elemen dibungkus group/component.

---

## Latihan tambahan (opsional)
1) Buat satu section yang memperlihatkan elevasi jalur (misalnya jalur di atas).
2) Tambahkan satu label pada belokan jalur (misalnya "belok kiri 90 derajat") agar mudah dibahas.
