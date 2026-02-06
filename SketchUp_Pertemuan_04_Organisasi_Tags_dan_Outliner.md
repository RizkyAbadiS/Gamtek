# SketchUp Pertemuan 4 - Tags dan Outliner (Agar Mudah Dipresentasikan)

Pertemuan ini adalah "beres-beres proyek". Anda akan menamai objek dengan rapi lewat Outliner, lalu memakai Tags untuk menampilkan/menyembunyikan bagian tertentu saat menjelaskan model. Setelah selesai, Anda bisa presentasi dengan cara yang lebih terstruktur: on/off tag untuk fokus, bukan orbit tanpa arah.

Pada tahap ini, model Anda mulai seperti "proyek". Proyek yang bagus bukan hanya yang selesai, tetapi yang bisa dibaca dan dipahami orang lain.

---

## Aturan paling penting (wajib)
**Edges dan Faces harus tetap Untagged.**

Tags hanya diberikan ke **Group/Component** (wadahnya). Jika edges/faces ikut ditag, model sering terlihat "sobek" saat tag dimatikan.

---

## Hasil akhir yang harus jadi
1) Outliner rapi (nama jelas, bukan `Group#123`)
2) Tags minimal: `Struktur`, `Komponen`, `Anotasi`
3) Anda bisa on/off tag tanpa merusak tampilan model

---

## Tutorial langkah demi langkah

### Langkah 1 - Buka file pertemuan 3
1) Buka `GT_SKP_P3_Nama_NIM.skp`.
2) Simpan sebagai file baru (supaya aman): `GT_SKP_P4_Nama_NIM.skp`

### Langkah 2 - Rapikan penamaan lewat Outliner
1) Buka panel **Outliner**.
2) Ubah nama objek penting, misalnya:
   - `Backplate`
   - `DIN_Rail`
   - `MCB_1P`
   - `Terminal_Block` (jika ada)

Checkpoint: Anda bisa membaca struktur model dari Outliner tanpa bingung.

### Langkah 3 - Buat Tags
1) Buka panel **Tags**.
2) Buat tag:
   - `Struktur`
   - `Komponen`
   - `Anotasi`

### Langkah 4 - Assign tag ke Group/Component
1) Klik backplate (group), set tag menjadi `Struktur`.
2) Klik DIN rail (component instance), set tag menjadi `Struktur` atau `Komponen` (pilih satu, konsisten).
3) Klik semua MCB (instances), set tag menjadi `Komponen`.

Checkpoint: saat Anda double click masuk ke dalam component, edges/faces di dalamnya tetap Untagged.

Jika Anda memakai aset import, prinsipnya sama: aset import harus dibungkus menjadi Component terlebih dahulu, lalu tag diberikan pada wadahnya. Jangan men-tag geometri di dalam aset.

### Langkah 5 - Uji show/hide untuk presentasi
1) Matikan `Komponen`. Yang terlihat harus tinggal struktur.
2) Nyalakan lagi `Komponen`.
3) Matikan `Struktur`. Yang terlihat harus komponen tetap utuh.

Jika ada bagian "hilang aneh", biasanya ada geometri yang tidak dibungkus atau edges/faces terlanjur ditag.

### Langkah 6 - Buat dua screenshot dokumentasi
1) Ambil screenshot kondisi semua tag menyala.
2) Ambil screenshot kondisi salah satu tag dimatikan (pilih yang paling menjelaskan).

---

## Jika mengalami masalah (troubleshooting)
- Model sobek saat tag dimatikan: periksa apakah ada edges/faces yang ditag, atau ada geometri tanpa Group/Component.
- Outliner terlalu ramai: rapikan dari objek yang paling penting dulu, lalu lanjutkan jika sempat.

---

## Latihan tambahan (opsional)
1) Tambahkan tag baru `WiringTray` untuk persiapan pertemuan berikutnya.
2) Buat satu scene yang hanya menampilkan `Komponen` (akan membantu presentasi).

Jika Anda ingin mulai memakai aset import dengan aman, baca lampiran ini terlebih dulu:
`SketchUp_Lampiran_Import_dan_Sumber_Aset.md`
