# SketchUp Pertemuan 3 - Group dan Component (Agar Model Tidak Berantakan)

Pertemuan ini fokus pada satu kebiasaan kerja yang membuat model rapi: membungkus geometri menjadi **Group** atau **Component**. Setelah itu, Anda menerapkannya pada mini panel sederhana agar paham kapan memakai Group dan kapan memakai Component.

Kalau Anda mengambil satu pelajaran saja dari SketchUp, ambil ini: jangan biarkan geometri menempel tanpa kontrol. Group dan Component adalah alat kontrol tersebut.

---

## Sebelum mulai (wajib)
1) Buat file baru (mm).
2) Terapkan aturan kerja rapi:
   - Bagian yang selesai dibuat, langsung dijadikan Group/Component.
   - Hindari geometri "terbuka" (edges/faces) tanpa wadah.

---

## Hasil akhir yang harus jadi
Mini panel sederhana yang terdiri dari:
1) Backplate (Group)
2) DIN rail (Component)
3) MCB 1P sederhana (Component) sebanyak 3 instance

Ukuran latihan (boleh dipakai):
- Backplate: 300 x 200 x 2 mm
- DIN rail dan MCB: proporsional dan konsisten

---

## Tutorial langkah demi langkah

### Langkah 1 - Backplate (Group)
1) Buat rectangle 300 x 200 mm.
2) **Push/Pull** setebal 2 mm.
3) Seleksi backplate, lalu jadikan **Group**.
4) (Opsional) Ubah nama group menjadi `Backplate`.

Checkpoint: klik backplate, yang terseleksi hanya satu objek utuh.

### Langkah 2 - DIN rail (Component)
1) Buat balok tipis memanjang sebagai DIN rail (ukuran bebas).
2) Seleksi balok DIN rail.
3) Jadikan **Component**, beri nama `DIN_Rail`.
4) Posisikan di atas backplate.

### Langkah 3 - MCB 1P (Component) dan duplikasi
1) Buat balok MCB sederhana (contoh ukuran latihan: 18 x 70 x 80 mm).
2) Seleksi balok tersebut.
3) Jadikan **Component**, beri nama `MCB_1P`.
4) Copy menjadi 3 buah (Move + Copy) dan susun rapi di atas DIN rail.

Checkpoint wajib (uji component):
1) Double click salah satu MCB untuk masuk mode edit component.
2) Ubah sedikit bentuk/ukurannya.
3) Keluar dari mode edit.
4) Pastikan dua MCB lain ikut berubah.

Uji kecil ini penting, karena di proyek nyata Anda sering mengganti satu ukuran kecil dan berharap semua komponen sejenis mengikuti perubahan tersebut.

### Langkah 4 - Rapikan jarak dan posisi
1) Pastikan MCB tidak saling bertabrakan.
2) Beri jarak kecil yang konsisten (misalnya 2-5 mm).
3) Cek tampilan dari Iso dan Front agar terlihat rapi.

### Langkah 5 - Simpan dan screenshot
1) Simpan: `GT_SKP_P3_Nama_NIM.skp`
2) Screenshot Iso: `GT_SKP_P3_Nama_NIM.png`

---

## Jika mengalami masalah (troubleshooting)
- Semua geometri menempel: Anda lupa membungkus bagian awal. Undo, lalu buat Group/Component lebih cepat.
- MCB tidak ikut berubah: pastikan MCB dibuat sebagai Component, dan yang Anda edit adalah component instance.
- Komponen jadi berbeda tanpa sengaja: hindari "Make Unique" kecuali memang ingin variasi.

---

## Latihan tambahan (opsional)
1) Buat component tambahan `Terminal_Block` sederhana, lalu duplikasi beberapa kali.
2) Mulai biasakan menamai objek (akan dipakai serius di pertemuan 4).

Opsional tambahan: import satu komponen dari internet (misalnya terminal block atau konektor) lalu rapikan dengan prosedur yang benar:
1) import,
2) bungkus sebagai Component,
3) cek skala,
4) beri nama yang jelas dan tempatkan rapi.

Panduan lengkap import ada di:
`SketchUp_Lampiran_Import_dan_Sumber_Aset.md`
