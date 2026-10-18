# WordCraft 2.1

Editor dokumen lokal dengan ribbon berbahasa Indonesia. Ekstrak ZIP lalu buka `index.html` di browser desktop modern. Untuk pengembangan, jalankan `python3 -m http.server 8000` dari folder ini lalu buka http://localhost:8000. Tidak memerlukan build atau layanan backend.

## Tambahan berdasarkan referensi

- Sisipkan: halaman sampul berisi judul, subjudul, penulis, instansi dan tahun; bookmark paragraf; referensi silang ke judul, keterangan atau bookmark; bagan batang dengan tabel data.
- Referensi: kelola sumber, sisipkan ulang kutipan tersimpan, daftar gambar/tabel/persamaan dengan tautan ke keterangannya.
- Tampilan: garis kisi dan zoom satu halaman.
- File → Informasi: properti penulis, tag, keterangan, statistik isi, akses versi dan unduh cadangan. Properti tersimpan lokal dan ikut cadangan WordCraft.
- Perbaikan: Escape mengakhiri mode baca; pencarian perintah menghormati mode baca untuk alat penyuntingan.

Fitur sebelumnya tetap tersedia: pemformatan teks dan paragraf, tabel, gambar, bentuk, margin, orientasi, ukuran kertas, kolom, header/footer, nomor halaman, daftar isi, kutipan sederhana, komentar, pelacakan teks dasar, gabung surat CSV, snapshot versi, impor/ekspor DOCX dasar dan cetak/PDF melalui browser.

## Cara menggunakan tambahan

1. Untuk bookmark, letakkan kursor dalam paragraf lalu pilih Sisipkan → Bookmark. Gunakan nama seperti `Bab_III`.
2. Gunakan gaya Judul 1–3 atau buat keterangan terlebih dahulu, kemudian pilih Referensi silang.
3. Untuk daftar gambar atau tabel, sisipkan keterangan melalui tab Referensi lalu pilih Daftar gambar / tabel. Sisipkan ulang daftar jika keterangannya berubah.
4. Bagan menerima 1–15 baris `Label; angka`, dengan nilai nol atau positif. Gambar bagan bersifat statis; sisipkan kembali untuk mengubah datanya.
5. File → Informasi → Simpan properti menyimpan metadata dokumen. Ekspor cadangan `.wordcraft` untuk memindahkannya ke perangkat lain.

## Batas dukungan

Aplikasi ini tidak mereplikasi seluruh fungsi Microsoft Word. Referensi silang dan daftar gambar tidak memiliki field atau nomor halaman otomatis. Sumber menggunakan format sederhana (Penulis, Tahun), bukan implementasi APA/MLA lengkap. Catatan dikumpulkan di akhir dokumen. Properti tambahan dijaga dalam cadangan WordCraft; tidak diekspor sebagai metadata DOCX. DOCX kompleks dapat mengalami perubahan format. Penyimpanan lokal bergantung pada data browser.

## Verifikasi versi ini

Pemeriksaan sintaks JavaScript lolos. Uji DOM lolos untuk startup, bookmark, referensi silang, bagan dan penolakan data tidak valid, sampul, kutipan/sumber, properti, pemuatan ulang, serta Escape dari mode baca. Uji DOM menggunakan pengganti API kanvas dan pengukuran halaman sehingga tidak memverifikasi gambar bagan atau tata letak visual. Uji browser visual belum dapat diselesaikan karena unduhan browser pengujian gagal. Periksa hasil pagination dan cetak dalam browser tujuan sebelum penggunaan dokumen final.
