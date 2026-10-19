# One-Pager PRD

**Produk:** [Nama Produk] - website marketplace micro-internship UMKM dengan konversi portofolio untuk mahasiswa
**Kelompok 36 (Web Dev & UI/UX):** M Khoirohman, Nabila Ammara Saleemah, Nathalia Gunalan, Adhya Triwardhana Ikhsan Prasetya, Paulia Nur Jayanti

---

## Section 1: Purpose

Apa yang dibuat, untuk siapa, dan mengapa penting.

### Intro: Elevator Pitch

- **For:** *mahasiswa semester awal hingga akhir di Indonesia yang minim pengalaman dan ingin membangun portofolio sebelum lulus*
- **Who:** *sulit menemukan kegiatan yang relevan dan ramah pemula, karena informasi tersebar, syarat pengalaman terlalu tinggi, dan takut ditolak atau di-ghosting*
- **The:** *[Nama Produk] adalah website persiapan karier berbentuk marketplace micro-internship UMKM*
- **That:** *memberi pengalaman kerja nyata (proyek 2-4 minggu) dari UMKM tanpa syarat pengalaman, lalu mengubah hasilnya menjadi portofolio terverifikasi, ulasan mitra, dan poin CV*
- **Unlike:** *LinkedIn, JobStreet, Glints, dan Kalibrr yang berfokus pada lowongan atau networking bagi yang sudah berpengalaman*
- **Our Product:** *menyediakan proyek ramah pemula dengan informasi transparan sejak awal, plus skor kesiapan kerja dan portofolio yang siap dilirik rekruter*

### Who is it for?

- **Persona Lulu** (22 tahun, mahasiswi semester 7): ingin menambah pengalaman, keterampilan, relasi, dan portofolio, tetapi ragu mendaftar karena syarat pengalaman tinggi, info tugas tidak lengkap, dan takut tidak mendapat kabar.
- **Pengguna sekunder:** UMKM mitra yang membutuhkan bantuan tugas praktis.

### Why build it?

- **Background:** 48% dari 68 mahasiswa sulit mencari magang yang relevan dan 20,6% tidak punya koneksi (Wahjuningsih dkk., 2025). Magang terbukti meningkatkan employability skills (Sitorus & Hidayatulloh, 2025).
- **Assumptions:** UMKM bersedia memberi tugas riil singkat; mahasiswa mau mengerjakan proyek 2-4 minggu di sela kuliah.
- **Market opportunities:**
  1. **Ada kebutuhan nyata.** Mahasiswa butuh pengalaman kerja untuk portofolio, tetapi aksesnya sempit: 48% sulit menemukan magang relevan, 20,6% tidak punya koneksi, 16,2% kurang info dari kampus (Wahjuningsih dkk., 2025). Di Reddit, pencari kerja tanpa pengalaman mengirim 100+ lamaran dan hanya mendapat 3 respons.
  2. **Ada celah di solusi yang ada.** LinkedIn, JobStreet, Glints, dan Kalibrr berfokus pada lowongan dan syarat pengalaman, sehingga pemula tetap harus mencari pengalaman pertamanya sendiri.
  3. **Peluangnya:** platform tahap awal sebelum dunia kerja. Mahasiswa mengerjakan proyek singkat UMKM tanpa syarat pengalaman, dan hasilnya langsung menjadi portofolio terverifikasi. UMKM mendapat bantuan tugas praktis.
  4. **Validasi:** baru tahap riset. Lima wawancara mahasiswa menunjukkan kebutuhan yang sama, yaitu peluang ramah pemula dengan info transparan. Uji usability prototipe (target >80% berhasil) dan minat UMKM belum diuji.
- **Company goals:** mewujudkan desain Figma Modul 5 menjadi prototipe web interaktif dengan AI-assisted prototyping dan Git yang disiplin.

---

## Section 2: Features and Functionality

Elemen praktis dari build, dari sudut pandang pengguna.

### What is it?

Alur utama: Landing Page, Sign Up/Log In, Onboarding (jurusan, minat/skill, tujuan, tingkat pengalaman), Dashboard (Explore, Search, Filter), Detail Project, Apply, Application Status, Project Workspace, Review & Feedback, Verified Experience, lalu Portfolio Builder dan Share Portfolio.

- **How will users interact?** Mencari dan menyaring proyek (bidang, skill, durasi, tingkat pengalaman), membuka detail proyek dalam modal, melihat Match %, lalu apply dan memantau status. Di mobile, navigasi lewat menu hamburger/drawer.
- **Terms to know?** *Micro-internship* (proyek singkat 2-4 minggu), *Readiness Score* (skor kesiapan kerja), *Verified Experience* (bukti kerja dengan ulasan mitra).
- **Problems solved:** info kegiatan tersebar, syarat tidak realistis bagi pemula, takut ditolak/ghosting, dan bingung mengubah pengalaman menjadi portofolio.
- **Info wajib di tiap proyek** (dari wawancara): posisi, tugas, durasi, skema kerja, kompensasi, requirement wajib vs nilai tambah, alur seleksi, deadline, dan penyelenggara.
- **Cakupan prototipe Modul 7:** landing page, explore + filter, detail proyek (modal), drawer navigasi, dan tampilan portofolio dengan data statis; fitur lain sebagai tahap lanjutan.

### What does it look like / How does it feel?

Mengikuti desain Figma Modul 5 dengan komponen Navbar/Sidebar, Card, Badge, Filter Chips, Modal, Progress Bar, dan Verification Badge. Terasa ramah dan aman bagi pemula.

Figma: [ tempel tautan Figma Modul 5 ]

---

## Section 3: Release Criteria

Persyaratan minimum untuk rilis.

| Kategori | Kriteria |
|---|---|
| **Functionality** | Minimal 2 aksi interaktif berfungsi (drawer, modal, filter) |
| **Usability** | >80% pengguna menemukan kegiatan dan memahami requirement; menemukan kegiatan <3 menit |
| **Reliability** | Bebas crash/runtime error dan broken layout di mobile hingga desktop |
| **Performance** | Halaman cepat dimuat, interaksi tanpa lag |
| **Supportability** | README lengkap; repo GitHub publik dengan minimal 5 komit deskriptif |

---

## Section 4: Timeline and Constraints

Rencana waktu dan kendala yang mungkin berpengaruh.

- **Ideal launch date:** [tanggal pengumpulan Modul 7]
- **Timeline:** Setup & PRD, Ekstraksi Desain, Generasi AI, Pasang Logika, lalu Poles & Audit

**Known constraints:**

- **Budget:** tanpa anggaran, hanya layanan gratis
- **Timeline:** mengikuti tenggat Modul 7
- **Resources:** 5 anggota kelompok
- **Dependencies:** desain Figma Modul 5, tool AI, akses GitHub; data proyek dan UMKM masih simulasi

---

## Additional Resources

Tautan desain, riset, dan papan proyek.

> **Aplikasi terpublikasi di Github Repository dan dicantumkan dalam PRD ini.**

| Item | Tautan |
|---|---|
| GitHub Repository | [ https://github.com/... ] |
| Desain Figma Modul 5 | [ https://figma.com/... ] |
| User Journey (Canva) |[ https://canva.link/....] |
| Design Thinking Map | [ https://canva.link/....] |