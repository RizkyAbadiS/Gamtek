# SketchUp Pertemuan 2 - Dari 2D Presisi ke 3D (Push/Pull)

Pada pertemuan ini Anda melatih workflow yang paling sering dipakai di SketchUp: menggambar bentuk 2D dengan ukuran presisi, lalu mengubahnya menjadi objek 3D yang bisa dipahami sebagai benda nyata. Objek latihannya adalah **enclosure** (kotak perangkat) sederhana: ada body, ada ketebalan dinding, ada cover terpisah.

Bayangkan enclosure sebagai "kulit" yang melindungi perangkat. Karena itu, latihan ini sengaja menekankan ketebalan dinding yang konsisten dan pemisahan body-cover, supaya nanti Anda terbiasa memperlihatkan isi di dalamnya saat presentasi.

---

## Sebelum mulai (wajib)
1) Buat file baru dan pastikan unit **mm**.
2) Siapkan kebiasaan kerja rapi: selesai satu bagian penting, segera jadikan Group/Component.

---

## Hasil akhir yang harus jadi
Enclosure sederhana dengan spesifikasi:
- Ukuran luar body: 200 x 150 x 80 mm
- Tebal dinding: 3 mm
- Cover (tutup) terpisah dari body
- Minimal ada 2 lubang kabel sederhana (konsep)

---

## Tutorial langkah demi langkah

### Langkah 1 - Buat body luar (balok utama)
1) Masuk tampilan **Top** (disarankan).
2) Buat rectangle 200 x 150 mm pada ground.
3) Gunakan **Push/Pull** setinggi 80 mm sehingga menjadi balok.

Checkpoint: Anda punya balok ukuran 200 x 150 x 80 mm.

### Langkah 2 - Buat ketebalan dinding 3 mm dan kosongkan bagian dalam
1) Klik face atas body.
2) Gunakan **Offset**, masukkan `3`, arahkan ke dalam.
3) Klik area dalam (hasil offset), lalu **Push/Pull** ke bawah untuk mengosongkan interior.
   - Berhenti sebelum menembus bawah jika Anda ingin enclosure tertutup.

Checkpoint: interior kosong terlihat dari atas, dan dinding terasa berketebalan.

Di tahap ini, jangan buru-buru menambah detail. Pastikan dulu Anda benar-benar bisa membuat ketebalan dinding yang konsisten. Ketebalan yang konsisten adalah informasi yang paling mudah dibaca dan paling mudah dicek.

### Langkah 3 - Bungkus body menjadi Group
1) Seleksi seluruh body.
2) Jadikan **Group**.
3) (Opsional) Beri nama: `Body_Enclosure`.

### Langkah 4 - Buat cover (tutup) terpisah
Fungsi cover: cover bisa disembunyikan saat presentasi supaya bagian dalam terlihat.

Cara sederhana yang aman:
1) Pada bagian atas body, buat rectangle mengikuti ukuran luar (200 x 150 mm).
2) **Push/Pull** setebal 3 mm atau 5 mm (pilih salah satu dan konsisten).
3) Seleksi cover lalu jadikan **Group** terpisah.
4) (Opsional) Beri nama: `Cover_Enclosure`.
5) Pastikan cover berada pada posisi menutup body (gunakan **Move** bila perlu).

Checkpoint: saat Anda klik cover, yang terseleksi hanya cover (body tidak ikut).

Uji cepat: coba hide cover. Body harus tetap utuh, dan interior harus tetap bisa dilihat tanpa Anda membongkar-bongkar model.

### Langkah 5 - Buat 2 lubang kabel sederhana
1) Orbit sampai Anda melihat salah satu sisi dinding.
2) Gambar rectangle 20 x 10 mm pada dinding.
3) **Push/Pull** menembus dinding sampai menjadi lubang.
4) Buat satu lubang lagi di sisi lain atau posisi lain.

### Langkah 6 - Simpan dan screenshot
1) Simpan file: `GT_SKP_P2_Nama_NIM.skp`
2) Screenshot tampilan Iso: `GT_SKP_P2_Nama_NIM.png`

---

## Cek cepat sebelum selesai
1) Body dan cover adalah dua Group berbeda.
2) Ukuran luar body benar (200 x 150 x 80 mm).
3) Tebal dinding konsisten 3 mm (cek 1-2 titik bila perlu).
4) Dua lubang kabel benar-benar menembus dinding.

---

## Jika mengalami masalah (troubleshooting)
- Offset mengarah ke luar: undo, lalu ulangi offset ke arah dalam.
- Bagian dalam masih solid: pastikan area dalam (hasil offset) yang Anda Push/Pull ke bawah.
- Cover menempel: jadikan cover Group terpisah setelah selesai dibuat.

---

## Latihan tambahan (opsional)
Jika masih ada waktu:
1) Tambahkan 4 kaki kecil di bawah enclosure.
2) Coba buat satu sudut cover sedikit membulat menggunakan Arc (cukup konsep).

Opsional tambahan (untuk konteks): import satu model konektor sederhana (misalnya DC jack atau konektor) lalu letakkan di dekat lubang kabel. Ikuti prosedur import yang rapi di:
`SketchUp_Lampiran_Import_dan_Sumber_Aset.md`
