# Lampiran - Import File dan Sumber Aset yang Terpercaya (SketchUp)

Lampiran ini membantu Anda saat ingin memakai model siap pakai (asset), misalnya komponen elektrikal, konektor, furniture, atau part mekanik sederhana. Gunakan asset untuk mempercepat, tetapi tetap jaga model Anda rapi dan mudah dibaca.

---

## 1) Prinsip aman sebelum import
Sebelum klik "Download", biasakan cek 4 hal ini:
1) Lisensi/penggunaan: pastikan model boleh dipakai untuk tugas kuliah. Kalau sumbernya komunitas, jangan anggap semua bebas.
2) Format file: semakin "native" semakin aman. SKP biasanya paling nyaman untuk SketchUp.
3) Unit dan skala: banyak aset beredar tanpa informasi unit. Anda harus siap mengecek ulang.
4) Kompleksitas: pilih model yang sederhana. Model yang terlalu detail sering bikin file berat dan sulit dipresentasikan.

Prinsipnya: untuk tugas teknik, Anda butuh model yang informatif, bukan model yang paling realistis.

---

## 2) Sumber aset yang umumnya bisa dipercaya
Di bawah ini adalah sumber yang sering dipakai dan relatif aman dari sisi reputasi. Tetap cek lisensi tiap model.

### A) Sumber resmi SketchUp
1) 3D Warehouse (Trimble/SketchUp)  
   Cocok untuk aset umum (furniture, komponen generik, contoh panel sederhana). Banyak pilihan, tetapi kualitas beragam, jadi pilih yang ringan dan rapi.
   - `https://3dwarehouse.sketchup.com/`

2) SketchUp Help Center (panduan import dan workflow resmi)  
   Referensi paling aman kalau Anda bingung opsi import.
   - `https://help.sketchup.com/`

### B) Library CAD/part engineering yang populer
1) TraceParts  
   Banyak part mekanik dan industri. Sering menyediakan beberapa format (termasuk CAD). Cocok untuk konektor, bracket, dan part standar (tergantung ketersediaan).
   - `https://www.traceparts.com/`

2) 3D ContentCentral (Dassault Systemes)  
   Library komunitas + vendor, fokus part engineering.
   - `https://www.3dcontentcentral.com/`

3) McMaster-Carr (CAD)  
   Bagus untuk part mekanik umum (baut, bracket, dll) dan banyak format CAD.
   - `https://www.mcmaster.com/`

4) GrabCAD Library  
   Banyak model komunitas. Kualitas bervariasi; pakai dengan selektif, dan selalu cek lisensi.
   - `https://grabcad.com/library`

### C) Sumber pabrikan (paling aman untuk komponen tertentu)
Banyak pabrikan menyediakan portal CAD/BIM untuk produk mereka. Jika Anda butuh bentuk yang mendekati nyata (misalnya konektor, enclosure, MCB), sumber pabrikan biasanya paling aman.

Strateginya: cari kata kunci `CAD model` atau `BIM` + nama produk/pabrikan.

---

## 3) Cara import yang rapi (step-by-step)
Bagian ini sengaja ditulis sebagai prosedur yang bisa Anda ulang kapan pun.

### Langkah 1 - Siapkan folder aset
1) Buat folder `Aset_Import` di folder kerja Anda.
2) Simpan semua file yang diunduh di sana (jangan campur dengan tugas).
3) Ubah nama file aset agar jelas, misalnya `DC_Jack_SourceName.ext`.

Tujuannya sederhana: kalau ada masalah, Anda mudah melacak dari mana aset itu berasal.

### Langkah 2 - Import ke SketchUp
1) Buka SketchUp.
2) Pilih menu File > Import.
3) Pilih jenis file yang sesuai (misalnya `.skp`, `.dae`, `.dwg`, `.dxf`, dll).
4) Jika ada tombol Options, buka dan pastikan:
   - unit masuk akal (mm/inch),
   - pengaturan yang membantu (misalnya merge coplanar faces) sesuai kebutuhan.
5) Klik Import.

Catatan: kemampuan import bisa berbeda tergantung versi SketchUp (web vs desktop) dan paket lisensi.

### Langkah 3 - Setelah import, langsung "bungkus"
Begitu aset masuk ke model, jangan biarkan geometri import "telanjang".
1) Seleksi seluruh aset import.
2) Jadikan Component (disarankan) dan beri nama jelas.
3) (Opsional) Set axis component agar mudah diposisikan.

Dengan cara ini, aset tidak menempel ke geometri lain saat Anda edit.

### Langkah 4 - Cek skala dan unit (wajib)
1) Ukur satu dimensi yang Anda kenal (misalnya diameter lubang, lebar komponen).
2) Kalau ukuran tidak masuk akal, perbaiki skala sebelum lanjut:
   - bisa dengan Tape Measure + Scale,
   - atau import ulang dengan opsi unit yang benar.

Jangan menunda cek skala. Kalau skala salah, seluruh desain bisa ikut salah.

### Langkah 5 - Sederhanakan dan rapikan
Jika aset terlalu berat:
1) Hapus detail yang tidak penting untuk tugas (misalnya chamfer kecil, baut kecil).
2) Pastikan tidak ada tag aneh yang terbawa.
3) Rapikan Outliner (nama jelas).

Target Anda: file tetap ringan dan mudah dipresentasikan.

---

## 4) Cara memakai aset tanpa merusak kerapian tugas
Rekomendasi kebiasaan:
1) Buat tag khusus `Aset_Import` (opsional) atau masukkan ke tag sistem (`Komponen`, `Perangkat`).
2) Jangan men-tag edges/faces.
3) Batasi jumlah aset import (lebih sedikit tapi jelas lebih baik).
4) Saat presentasi, jelaskan aset import Anda hanya sebagai konteks. Fokus tetap pada desain dan keputusan Anda.

---

## 5) Catatan etika akademik (singkat)
Jika Anda memakai aset dari internet:
1) catat sumbernya (link),
2) sebutkan di dokumen spesifikasi,
3) jangan mengklaim aset itu buatan Anda.

