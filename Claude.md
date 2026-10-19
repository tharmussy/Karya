# CLAUDE.md

Panduan untuk asisten AI (Claude Code, Cursor, Copilot, dsb.) yang membantu mengerjakan proyek ini. Baca seluruh file ini sebelum menulis atau mengubah kode.

## Konteks Proyek

Prototipe web interaktif untuk **[Nama Produk]**, marketplace micro-internship UMKM bagi mahasiswa, dengan fitur konversi pengalaman menjadi portofolio. Ini tugas Vinix Batch 5 - Modul 7 (Kelompok 36): mengubah desain Figma Modul 5 menjadi prototipe web.

Yang dinilai adalah fungsionalitas dan kualitas eksekusi, bukan kerumitan teknologi. Utamakan hasil yang rapi, stabil, dan sesuai desain.

- Desain acuan (sumber kebenaran visual): [ tautan Figma Modul 5 ]
- Detail produk dan fitur: lihat `PRD.md`
- Prototipe memakai **data statis** (tanpa backend dan database)

## Tech Stack

- Framework: [mis. Vite + React]
- Styling: [mis. Tailwind CSS]
- Package manager: [mis. npm]

Jangan menambah library besar tanpa alasan yang jelas. Pilih solusi paling sederhana yang memenuhi kebutuhan.

## Perintah

```bash
npm install        # pasang dependensi
npm run dev        # jalankan server pengembangan
npm run build      # build produksi, harus lolos tanpa error
```

*(sesuaikan dengan framework yang dipakai)*

## Cakupan Pekerjaan

**Dikerjakan:**
- Landing page
- Halaman explore dengan kartu proyek dan filter
- Detail proyek dalam modal
- Drawer navigasi untuk mobile
- Tampilan portofolio (data statis)

**Jangan dikerjakan** kecuali diminta: login/registrasi sungguhan, backend, database, pembayaran, dan fitur di luar daftar di atas. Kalau ada ide tambahan, usulkan dulu dalam respons, jangan langsung diimplementasikan.

## Aturan Wajib

1. **Presisi visual.** Warna, tipografi, jarak, dan tata letak mengikuti Figma Modul 5. Simpan token (warna, font, spacing, radius) di satu tempat, jangan menulis nilai berulang di banyak file.
2. **Responsif.** Mobile-first. Periksa di lebar 360 px, 768 px, dan 1440 px. Tidak boleh ada konten yang terpotong atau scroll horizontal tak disengaja.
3. **Minimal 2 interaksi dinamis yang benar-benar bekerja** dengan state: drawer, modal, dan filter. Interaksi harus bisa dipakai lewat keyboard (Esc menutup modal/drawer, fokus tidak hilang).
4. **Tanpa crash.** Tidak ada error di konsol. Tangani kondisi kosong, misalnya filter yang tidak menghasilkan proyek.
5. **Aksesibilitas dasar.** HTML semantik, teks alternatif pada gambar, kontras warna memadai, dan label pada tombol ikon.

## Struktur Kode

```
src/
  components/   # komponen UI yang dapat dipakai ulang (Navbar, Card, Modal, FilterChips, dll.)
  pages/        # halaman (Landing, Explore, Portfolio)
  data/         # data statis (daftar proyek, UMKM, dsb.)
  styles/       # token desain dan gaya global
```

Konvensi:
- Satu komponen satu file; nama komponen memakai PascalCase.
- Komponen kecil dan fokus. Pecah bila lebih dari sekitar 150 baris.
- Teks antarmuka dalam Bahasa Indonesia.
- Hindari kode mati, komentar yang hanya mengulang isi kode, dan `console.log` yang tertinggal.

## Data Proyek (Statis)

Setiap proyek minimal memuat informasi yang diminta mahasiswa pada riset: posisi, deskripsi tugas, durasi (2-4 minggu), skema kerja (remote/lokasi), kompensasi, requirement wajib dan nilai tambah, alur seleksi, deadline, nama UMKM penyelenggara, serta kategori dan tingkat pengalaman. Gunakan konten contoh yang realistis dan jangan memakai nama merek atau orang sungguhan.

## Git dan GitHub

- Repositori **publik**. Komit kecil dan sering (minimal 5 komit bermakna, idealnya satu per fitur atau perbaikan).
- Format pesan komit: `tipe: deskripsi singkat`, dengan tipe `feat`, `fix`, `style`, `refactor`, `docs`, atau `chore`.
  - Contoh: `feat: tambah filter chips pada halaman explore`
- Jangan komit `node_modules`, file `.env`, atau berkas besar yang tidak perlu.
- Jangan mengubah riwayat komit yang sudah di-push (tanpa `force push`).

## Dokumentasi AI (Pertanggungjawaban)

Penggunaan AI dinilai. Setiap kali menghasilkan atau mengubah bagian penting:

1. Ringkas prompt yang dipakai dan hasilnya untuk dicatat tim di **README.md** (bagian Log Prompt AI).
2. Sebutkan bagian yang perlu diperiksa atau diperbaiki manual.
3. Jangan menyembunyikan keterbatasan hasil. Jika sesuatu belum sesuai Figma atau belum teruji, katakan terus terang.

## Cara Bekerja

- Pahami dulu kode yang ada sebelum mengubahnya, lalu ubah seperlunya saja.
- Untuk perubahan besar, jelaskan rencana singkat lebih dulu.
- Setelah perubahan, jalankan build dan periksa tampilan di ukuran layar yang disebut di atas.
- Bila instruksi ambigu atau bertentangan dengan Figma, tanyakan sebelum menebak.

## Definisi Selesai

- [ ] Tampilan sesuai Figma Modul 5 pada mobile, tablet, dan desktop
- [ ] Minimal 2 aksi interaktif berfungsi tanpa error
- [ ] `npm run build` berhasil
- [ ] Komit rapi dan sudah di-push ke GitHub publik
- [ ] README.md terisi (cara menjalankan, tautan Figma, log prompt, perbaikan manual, kontribusi anggota)
- [ ] PRD memuat tautan repositori GitHub