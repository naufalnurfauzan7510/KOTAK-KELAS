# AI Logbook: Kotak Kelas

Dokumentasi penggunaan AI selama perancangan, pembuatan, dan perbaikan website **Kotak Kelas**. 

## Informasi Proyek

| Bagian | Keterangan |
|---|---|
| Nama proyek | Kotak Kelas |
| Tujuan | Website marketplace sederhana untuk membantu siswa melihat produk dan menghubungi penjual melalui WhatsApp |
| AI utama | Claude (Anthropic) |
| Teknologi yang tampak pada percakapan | HTML, CSS, JavaScript, `localStorage`, Lucide Icons, Live Server |
| Anggota tim | [Haris suyanto dan Naufal nur fauzan] |
| Sekolah/kelas | [SMKN KABUH] |
| Periode pengerjaan | [21 oktober - 28 oktober] |

---

## Tahap 1 — Eksplorasi Ide dan Perancangan

### Entri 1.1 — Mengubah ide awal menjadi brief website

| Bagian | Catatan |
|---|---|
| AI | Claude |
| Tujuan | Merancang  fondasi awal website dan merancang ui . |
| instruksi | Saya meminta Ai untuk merancang ui dengan warna biru dan kuning dan menggunakan lucide icons sebagai icon di web. |
| Respons AI | Claude mulai merancang struktur file seperti html, css dan javascript. |


### Entri 1.2 — Memperjelas batasan dan fitur

| Bagian | Catatan |
|---|---|
| AI | Claude |
| Tujuan | memastikan fitur berjalan sesuai harapan. |
| Keputusan proyek | kami memutuskan untuk tidak menggunakan database karena ini hanya untuk demo saja ,jadi kami memilih untuk memakai `localStorage` untuk menyimpan data. |
| Respons AI | Claude merevisi brief dengan memasukkan keputusan tersebut, menyarankan pemisahan lapisan penyimpanan agar nantinya dapat diganti dengan layanan database, kompresi gambar, dan pengelolaan akun. |


---

## Tahap 2 — Penyusunan dan Pengembangan Kode

### Entri 2.1 — Membuat versi awal website

| Bagian | Catatan |
|---|---|
| AI | Claude |
| Tujuan | menjadikan brief dan ilustrasi menjadi kode. |
| Prompt dan instruksi | Saya memberikan brief Kotak Kelas beserta gambar referensi. |
| Respons AI | Claude membuat 3 file untuk awalan yaitu index.html,style.css dan script.js ,komponen awal untuk layout. |
|

### Entri 2.2 — Menambahkan layout desktop dan membersihkan scrollbar

| Bagian | Catatan |
|---|---|
| AI | Claude |
| Tujuan | Membuat tampilan untuk mobile. |
| Prompt | “saya ingin menambah sedikit detail, tambahkan layout untuk desktop, promt ini ketika saya jalankan merupakan layout untuk handphone, aku juga minta kasih juga untuk desktop. tidak usah menambahkan dummy untuk contoh websitenya, dan hilangkan scroll yang masih terlihat didalam, agar terlihat lebih clean.” |
| Respons AI | Claude memberikan kode css nya dan juga sudah menghilangkan scroll agar terlihat clean. 
| 

### Entri 2.4 — Memperbaiki hero, bagian “Janji Kami”, dan halaman akun

| Bagian | Catatan |
|---|---|
| AI | Claude |
| Tujuan | Membuat bagian beranda dan halaman login/daftar lebih menarik serta konsisten. |
| Prompt | Saya meminta bagian “Janji Kami” dibuat berbeda dari kartu toko, deskripsi hero dapat berubah-ubah, dan desain login/daftar versi mobile diperbagus atau diberi pilihan model. |
| Respons AI | Claude memberikan alternatif dan memberika desain untuk menu login/daftar. |

---

## Tahap 3 — Debugging dan Perbaikan Masalah

### Entri 3.1 — Kategori tidak memenuhi lebar dan filter tidak bekerja

| Bagian | Catatan |
|---|---|
| AI | Claude |
| Gejala | Kartu kategori tidak memenuhi lebar yang diinginkan. Ketika kategori dipilih, kartu tidak berubah menjadi biru dan produk terkait tidak muncul. |
| Prompt  | “kategori buat sampai keujung dan ketika dipencet tidak berwarna biru dan produk tidak tampil pahdahal ada kategorinya” |
| Analisis AI | Claude menduga terdapat dua handler klik kategori yang saling menimpa, dan bahwa fungsi `refresh()` lama mencoba mengubah elemen `#chips` yang tidak tersedia pada halaman beranda. AI kemudian mengusulkan pemisahan aksi kategori, pemeriksaan elemen sebelum diperbarui, serta penyesuaian fungsi `katCards()`, `chips()`, dan `refresh()`. |
| Perbaikan yang disarankan | Menggunakan aksi terpisah untuk kartu kategori (`katcard`) dan chip filter (`kat`), memperbarui kategori hanya jika elemen terkait tersedia, serta memastikan listener klik tidak terduplikasi. |
| Status  | Masalah sudah selesai dan kartu kategori sudah sampai ke ujung dan begitu dengan masalah lainnya. |


### Catatan debugging tambahan

Dalam percakapan, Claude membedakan pesan Console yang berhubungan dengan masalah kategori dari pesan seperti `favicon.ico 404`, “Tracking Prevention”, dan “Images loaded lazily”, yang dinilai tidak menjadi penyebab utama masalah kategori. Claude meminta pesan error lengkap atau tangkapan layar Console jika masalah masih berlanjut.

---

## Tahap 4 — Penjelasan Kode dan Refleksi

### 4.1 Ringkasan refleksi

Ai membantu dalam pengerjaan projek kami ,banyak pekerjaan yang bisa lumayan kerjakan namun tetap saja kode dari ai tidak bisa di iyakan maka dari itu kami riset dan menyeleksi kode yang ai berikan 

Keputusan mengenai penggunaan `localStorage`, perhitungan margin dari harga jual, rating untuk penjual, dan kebutuhan login penjual merupakan keputusan proyek yang disampaikan dalam percakapan.


---

