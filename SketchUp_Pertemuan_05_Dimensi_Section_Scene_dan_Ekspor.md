# SketchUp Pertemuan 5 - Dimensi, Section, Scene, dan Ekspor

Mulai pertemuan ini, model Anda tidak hanya "ada", tetapi harus **mudah dibaca**. Ukuran harus jelas, isi di dalam harus bisa ditunjukkan, dan Anda harus bisa menjelaskan model hanya dengan berpindah scene (bukan orbit tanpa arah). Output akhirnya adalah gambar yang siap dimasukkan ke laporan.

---

## Sebelum mulai (wajib)
1) Buka `GT_SKP_P4_Nama_NIM.skp` (atau file terbaru Anda).
2) Simpan sebagai: `GT_SKP_P5_Nama_NIM.skp` (supaya aman).

Jika Anda memakai aset import, rapikan dulu sebelum mulai memberi dimensi: bungkus sebagai Component, cek skala, dan pastikan tag-nya benar. Panduan import ada di:
`SketchUp_Lampiran_Import_dan_Sumber_Aset.md`

---

## Hasil akhir yang harus jadi
1) Minimal 3 scene: `S01_Iso`, `S02_Front` (atau `S02_Top`), `S03_Section`
2) Minimal 5 dimensi kunci
3) Minimal 3 label komponen
4) Minimal 2 file PNG hasil ekspor (Iso dan Section)

---

## Tutorial langkah demi langkah

### Langkah 1 - Siapkan style tampilan yang enak dibaca
1) Gunakan tampilan sederhana (misalnya garis tegas, warna tidak terlalu ramai).
2) Tujuannya: dimensi dan label mudah terlihat.

Anda tidak perlu membuat render. Fokus pada keterbacaan.

Bayangkan Anda sedang membuat "halaman gambar teknik" dari model 3D. Kalau tampilannya ramai, dimensi dan label akan sulit terbaca, dan presentasi Anda akan terasa berputar-putar.

### Langkah 2 - Buat scene `S01_Iso`
1) Atur tampilan ke Iso.
2) Pastikan model terlihat utuh dan rapi.
3) Tambahkan scene dan beri nama `S01_Iso`.

### Langkah 3 - Buat scene `S02_Front` (atau `S02_Top`)
1) Pindah ke tampilan Front (atau Top jika lebih informatif untuk layout).
2) Tambahkan scene dan beri nama `S02_Front` atau `S02_Top` (pilih salah satu).

### Langkah 4 - Buat section dan simpan sebagai `S03_Section`
1) Tambahkan **Section Plane**.
2) Posisikan section sehingga bagian penting di dalam terlihat (misalnya posisi komponen di atas backplate).
3) Aktifkan section.
4) Atur tampilan agar penampang jelas.
5) Tambahkan scene bernama `S03_Section`.

Checkpoint: di `S03_Section`, Anda bisa melihat bagian dalam tanpa harus menyembunyikan objek satu per satu.

Section adalah cara paling cepat untuk menjelaskan bagian dalam tanpa "membongkar" model. Karena itu, simpan section menjadi scene supaya Anda tidak mengatur ulang setiap kali presentasi.

### Langkah 5 - Tambahkan dimensi kunci (minimal 5)
Tambahkan dimensi yang memang membantu orang memahami ukuran. Contoh yang aman:
1) ukuran backplate,
2) jarak antar MCB,
3) panjang DIN rail,
4) jarak komponen ke tepi backplate,
5) tinggi/posisi komponen (jika relevan).

Tips agar rapi:
1) tempatkan dimensi sedikit menjauh dari objek,
2) jangan menumpuk dimensi di satu area,
3) kalau terlalu penuh, pilih dimensi yang paling penting.

Jika Anda ragu harus menaruh dimensi di mana, prinsipnya sederhana: dimensi harus membantu orang lain memahami ukuran tanpa menutupi objek. Dimensi yang rapi itu lebih bernilai daripada dimensi yang banyak tetapi tidak terbaca.

### Langkah 6 - Tambahkan label komponen (minimal 3)
Untuk tiap label, gunakan format sederhana:
`Nama komponen - fungsi singkat`

Contoh:
`MCB_1P - proteksi beban`

### Langkah 7 - Ekspor gambar dari scene
Ekspor minimal dua gambar:
1) dari `S01_Iso` (overview),
2) dari `S03_Section` (menjelaskan bagian dalam).

Simpan sebagai PNG dengan nama yang jelas, misalnya:
- `GT_SKP_P5_Nama_NIM_S01_Iso.png`
- `GT_SKP_P5_Nama_NIM_S03_Section.png`

---

## Cek cepat sebelum selesai
1) Scene berpindah rapi dan konsisten.
2) Dimensi tidak menutupi objek penting.
3) Label mudah dibaca.
4) PNG ekspor sesuai scene.

---

## Jika mengalami masalah (troubleshooting)
- Dimensi bertumpuk: pindahkan dimensi menjauh, atau kurangi dimensi yang tidak penting.
- Section tidak terlihat: pastikan section plane aktif, dan Anda berada pada scene yang menyimpan kondisi itu.
- Scene berubah-ubah: pastikan saat membuat scene Anda sudah berada pada view yang tepat.

---

## Latihan tambahan (opsional)
Buat satu scene "Exploded" sederhana:
1) Copy komponen, geser sedikit menjauh agar struktur terlihat.
2) Simpan sebagai `S04_Exploded`.
