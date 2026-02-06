# SketchUp Pertemuan 1 - Perkenalan dan Dasar Navigasi

Pertemuan ini dibuat untuk memastikan Anda tidak "berantem" dengan SketchUp. Kita mulai dari hal yang paling dasar dan paling sering dipakai: mengatur unit, mengendalikan kamera, lalu menggambar objek pertama dengan ukuran yang benar.

Di akhir pertemuan, Anda akan punya satu file model sederhana yang rapi, plus satu gambar (screenshot) untuk dokumentasi.

---

## Sebelum mulai (wajib)
1) Buka SketchUp dan buat file baru.
2) Pastikan unit kerja adalah **millimeter (mm)**.
3) Buat folder kerja untuk mata kuliah ini, misalnya `GambarTeknik_SketchUp`, agar semua file tersimpan rapi.

Jika Anda belum yakin unitnya mm, jangan lanjut dulu. Unit yang salah akan membuat semua ukuran terasa "aneh".

Mulai pertemuan ini, biasakan menyimpan versi file secara rapi. Kebiasaan kecil ini berguna saat Anda salah langkah dan perlu kembali ke versi yang lebih aman.

---

## Hasil akhir yang harus jadi
Anda akan membuat **meja kerja sederhana** dengan spesifikasi:
- Ukuran top: 1000 x 600 mm
- Tebal top: 25 mm
- Tinggi meja: 750 mm

Anda tidak perlu membuat detail estetika. Fokusnya akurasi ukuran dan kerapian model.

---

## Tutorial langkah demi langkah

### Langkah 1 - Latihan kamera (2-3 menit)
1) Coba **Orbit** untuk memutar sudut pandang.
2) Coba **Pan** untuk menggeser tampilan.
3) Coba **Zoom** untuk mendekat dan menjauh.
4) Pindah ke Standard Views (misalnya **Top** dan **Front**) agar Anda paham arah sumbu.

Jika Anda "kehilangan objek", gunakan **Zoom Extents** supaya seluruh model terlihat lagi.

Kenapa latihan kamera didahulukan? Karena banyak orang sebenarnya mampu menggambar, tetapi frustrasi karena tidak bisa menemukan objek yang sudah digambar. Kamera yang nyaman membuat proses belajar tool lain terasa jauh lebih ringan.

### Langkah 2 - Buat top meja dengan ukuran presisi
1) Masuk ke tampilan **Top** (disarankan).
2) Pilih tool **Rectangle**.
3) Klik sekali pada area ground untuk titik awal rectangle.
4) Geser sedikit, lalu ketik ukuran `1000,600` dan tekan Enter.

Catatan penting: angka biasanya hanya terbaca setelah Anda benar-benar mulai menggambar (sudah klik titik awal).

Jika Anda membiasakan diri mengetik ukuran, Anda akan jarang perlu mengira-ngira. Ini salah satu kebiasaan penting di gambar teknik: ukuran ditentukan oleh angka, bukan oleh "kira-kira".

### Langkah 3 - Buat ketebalan top (25 mm)
1) Pilih tool **Push/Pull**.
2) Klik permukaan top meja.
3) Tarik ke atas sedikit, lalu ketik `25` dan tekan Enter.
4) Orbit sebentar untuk memastikan top sudah menjadi 3D (bukan hanya garis).

### Langkah 4 - Buat kaki meja sampai tinggi 750 mm
Ada dua cara aman. Pilih salah satu.

Opsi A (disarankan untuk pemula): 4 kaki balok
1) Pada permukaan bawah top, gambar satu kaki (misalnya 40 x 40 mm) di dekat salah satu sudut.
2) Gunakan **Push/Pull** untuk menurunkannya hingga tinggi total meja menjadi 750 mm.
   - Trik: tinggi kaki kira-kira 750 - 25 = 725 mm (karena top sudah 25 mm).
3) Copy kaki tersebut ke tiga sudut lain dengan tool **Move** + Copy.

Opsi B: penyangga sederhana
1) Buat satu balok penyangga di bawah top (ukuran bebas).
2) Dorong (Push/Pull) sampai total tinggi meja menjadi 750 mm.

Tidak masalah bentuknya sederhana, asalkan ukuran utamanya benar.

### Langkah 5 - Rapikan jadi satu objek (Group)
1) Seleksi semua bagian meja (top dan kaki).
2) Buat menjadi **Group**.

Tujuannya agar meja tidak menempel dengan geometri lain saat Anda lanjut latihan di pertemuan berikutnya.

Anggap Group sebagai "wadah". Selama objek ada di dalam wadah, ia tidak akan mengganggu dan tidak akan diganggu geometri lain.

### Langkah 6 - Simpan dan buat screenshot
1) Simpan file dengan nama: `GT_SKP_P1_Nama_NIM.skp`
2) Ubah tampilan ke **Iso**, lalu ambil screenshot dan simpan sebagai:
   - `GT_SKP_P1_Nama_NIM.png`

---

## Cek cepat sebelum selesai
Pastikan tiga hal ini benar:
1) Unit mm.
2) Top 1000 x 600, tebal 25, tinggi meja 750.
3) Meja sudah menjadi satu Group (tidak ada geometri "terbuka" yang menempel liar).

---

## Jika mengalami masalah (troubleshooting)
- Ukuran tidak masuk saat mengetik: pastikan Anda sudah klik titik awal dan sedang dalam proses menggambar.
- Tiba-tiba objek hilang: gunakan Zoom Extents, lalu kembali ke Top/Iso.
- Permukaan tidak bisa di-Push/Pull: biasanya bentuk belum menjadi face (masih garis terbuka). Ulangi rectangle sampai benar-benar membentuk bidang.

---

## Latihan tambahan (opsional)
Jika sudah selesai lebih cepat:
1) Buat dua scene sederhana: `S01_Top` dan `S02_Iso`.
2) Tambahkan satu label teks pada meja (misalnya "Meja Kerja").

Jika Anda penasaran soal aset dari internet, tahan dulu di pertemuan 1. Anda akan lebih siap setelah paham kerapian model (Group/Component dan Tags). Panduan import yang rapi ada di lampiran:
`SketchUp_Lampiran_Import_dan_Sumber_Aset.md`
