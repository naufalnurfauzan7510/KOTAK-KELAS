# KOTAK KELAS

## a. Judul dan Deskripsi
**Kotak Kelas** adalah Marketplace mini untuk siswa SMK yang ingin berjualan produk hasil praktek dan usaha kelas langsung dari laptop dan HP!

### latar belakang masalah
Disekolah kejuruan saya, banyak siswa kejuruan selain saya praktik membuat barang yang bisa dijual (Makanan, Minuman, DLL) dan dijual. Tapi mereka mempromoasikan jualannya ke Story Whatsapp.

### Solusi
**Kotak Kelas** adalah website yang mengumpulkan semua produk dari berbagai penjual yang disini adalah siswa di dalam satu tempat ini. Pembeli bebas memilih semua produk yang dijual, lalu memesannya dengan mengisi format pembeli lalu dikirim ke Whatsapp. penjual juga dibantu dengan kalkulator untuk menentukan dengan margin harga agar siswa tidak memperkira-kirakan harga produknya.

### Target Pengguna
1. **Pembeli** siswa, guru, dan warga sekolah yang ingin membeli dari website tersebut.
2. **Penjual** siswa SMK Negeri Kabuh yang ingin berjualan.

### Fitur Utama
**Pembeli**
- Melihat daftar produk, mencari nama produk atau penjual.
- Detail produk dengan status **READY** atau **PRE-ORDER**.
- Format pesan yang sederhana (nama, kelas, jumlah, catatan) kemudian dikirimkan ke Whatsapp.
- Beri rating dan ulasan untuk **penjual**.

**Penjual**
- Daftar dan login dengan nomor WhatsApp dan password.
- Dashboard penjual kamu bisa mengelola produk dan lihat pesanan masuk.
- Upload foto produk dan foto profile untuk toko atau penjual.
- **Kalkulator estimasi harga** hitung harga jual dari modal dan margin, dan markup dan hasil estimasi untung.

## b. Teknologi yang digunakan

**Katergori dan Teknologi**
Bahasa | HTML, CSS, dan JavaScript (tanpa framework)
Ikon | Lucide Icons (https://github.com/lucide-icons/lucide)
Font | Google Fonts (Plus Jakarta Sans)
Database | localStorage 
Keamanan password | Web Crypto API (SHA-256)
Integrasi pesan | WhatsApp wa.me link
Platform publikasi | Github Pages
Editor kode | Visual Studio Code

**Desain:** dengan gaya Liquid (glassmorphism). Palet warna menggunakan Warna `#f9e208` dan `#0234ad`. 

## c. Pemanfaatan AI (AI Usage Disclosure)

### Alat AI yang Digunakan
- **Claude (Anthropic)**: Merancang alur dari website dan desain kasar dari website tersebut.

### Contoh Prompt Utama
**1. Eksplorasi ide dan flowchart (Tahap 1)**
> Posisikan kamu sebagai profesional prompt untuk AI membuat flowchart untuk website, dengan logika seperti website developer. Nama websitenya "Kotak Kelas". Dashboardnya seperti gambar referensi dengan UI/UX Liquid, warna dari gambar palet, ikon dari Lucide, dan diakses lewat handphone. *(Alur kasar dari saya poduk, detail penjual, checkout pre-order, redirect WhatsApp, data pembeli, daftar penjual, rating, dan kalkulator harga.)*

**2. Penyusunan kerangka kode (Tahap 2)**
> Tolong saya untuk membuat kerangka code dari flowchart yang sudah dibuat diatas.

**3. Debugging (Tahap 3)**
> Kenapa navbar saya masih terpendam dan tombol kembali tidak bisa dipencet jika tertutup navbar buat agar dia mengukuti navbar dan tidak tertutup.

### Penyusaian dan perbaikan sendiri
**Bagian | Saran AI | Perbaikan sendiri**
Rencana awal | saran dari claude penjual tidak harus daftar atau login tanpa password | kita putuskan untuk menggunakan login dan daftar dengan login.
Beberapa tampilan | dari AI kami mendapatkan style yang kurang cocok | kita putuskan untuk menggunakan style yang seusai dari keinginan.

## d. Panduan Penggunaan

### Membuka Website
Buka tautan berikut lewat browser HP atau laptop

### Sebagai Pembeli
1. Buka beranda, lalu cari produk atau pilih dari kategori.
2. Klik produk untuk melihat detail dan status produk (READY atau PRE-ORDER).
3. Klik **Beli Sekarang** atau **Pre-Order**, lalu isi nama, kelas, jumlah, dan catatan.
4. Klik kirim, dan kamu akan dialihkan ke WhatsApp penjual dengan pesan otomatis ke penjual.
5. Setelah memesan, buka menu **Pesanan** untuk memberi rating kepada penjual.

### Sebagai Penjual
1. Buka menu **Jual**, lalu pilih **Daftar** dan isi data serta password.
2. Masuk Login dengan nomor WhatsApp dan password.
3. Di dashboard, klik **Tambah Produk**, unggah foto produk, isi nama produk, kategori produk, deskripsi produk, dan status produk masih PRE-ORDER atau READY.
4. Isi modal dan margin pada **kalkulator harga**, lalu pilih harga rekomendasi atau isi manual.
5. Simpan produk. Pesanan yang masuk muncul di dashboard dan juga di Whatsapp.

### Keterbatasan
- Data tersimpan di `localStorage`, jadi banyak keterbatasan, dan juga website ini untuk demo.
- Proteksi password hanya untuk demo, belum untuk penggunaan sungguhan.
- Pembayaran dan pengambilan barang diatur langsung antara pembeli dan penjual lewat WhatsApp.

### Struktur Repositori

├── index.html
├── style.css
├── script.js
├── README.md
└── AI_LOGBOOK.md

---

## e. Identitas Developer atau Pengembang
| | Pengembang 1 | Pengembang 2 |
| --- | --- | --- |
| **Nama lengkap** | Naufal Nur Fauzan | Haris Suyanto |
| **Kelas** | XI | XI |
| **Jurusan** | SIJA | SIJA |
| **Asal sekolah** | SMKN KABUH | SMKN KABUH |

*Karya ini dibuat dalam Pelatihan TIK bagi Murid SMA/SMK Tahun 2026, UPT. TIKP Dinas Pendidikan Provinsi Jawa Timur, dengan tema "Solusi Digital untuk Kehidupan Sehari-hari Berbantuan Kecerdasan Artifisial".*