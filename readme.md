# 📚 Aplikasi Toko Buku Online - Tugas UTS Pemrograman Web 1

Repositori ini berisi proyek Ujian Tengah Semester (UTS) mata kuliah Pemrograman Web 1. Aplikasi web *front-end* toko buku online ini dirancang dengan antarmuka modern bernuansa hijau muda (*emerald/mint*) serta dilengkapi berbagai fitur interaktif berbasis JavaScript.

---

## 🛠️ Fitur Utama Aplikasi
1. **Autentikasi Pengguna & Sapaan Dinamis (`index.html` & `dashboard.html`)**
   - Validasi login akun dengan pencocokan data pengguna.
   - Sapaan otomatis yang berubah sesuai waktu lokal (*Pagi, Siang, Sore, Malam*).
2. **Katalog & Manajemen Stok Buku (`stok.html`)**
   - Menampilkan tabel inventaris buku lengkap dengan informasi cover, edisi, stok, dan harga.
   - **Fitur Pencarian (*Search Bar*):** Mencari judul buku atau kode barang secara *real-time*.
   - **Form Tambah Buku (DOM):** Menambahkan data buku baru langsung ke tabel katalog.
   - **Tombol Hapus:** Menghapus data buku dari daftar katalog.
3. **Keranjang Belanja & Checkout (`stok.html`)**
   - Memilih dan memasukkan buku ke dalam keranjang belanja.
   - Kalkulasi total harga belanja secara otomatis.
   - Simulasi *checkout* yang mengarahkan pengguna ke form pemesanan.
4. **Form Pemesanan & *Generate* Resi (`pemesanan.html`)**
   - Form input data pemesan, alamat pengiriman, dan pilihan ekspedisi.
   - Menghasilkan nomor DO (*Delivery Order*) / Resi pengiriman unik secara instan.
5. **Tracking Resi Pengiriman (`tracking.html`)**
   - Melacak status pengiriman berdasarkan nomor resi yang dimasukkan.
   - Dilengkapi dengan *progress bar* visual dan detail histori perjalanan paket.
6. **Dark / Light Mode Global (`localStorage`)**
   - Saklar mode gelap dan terang (*Dark/Light Mode*) yang tersedia di seluruh halaman dan tersimpan otomatis menggunakan `localStorage`.

---

## 📂 Struktur Proyek
```text
bahan.uts/
│
├── index.html          # Halaman Login Utama
├── dashboard.html      # Halaman Utama / Dashboard Sapaan
├── stok.html           # Informasi Stok, Pencarian, Katalog, & Keranjang
├── pemesanan.html      # Form Pemesanan & Pembuatan Nomor Resi
├── tracking.html       # Pelacakan Resi & Status Pengiriman
│
├── css/
│   └── style.css       # Styling Utama (Tema Hijau Muda & Dark Mode)
│
└── js/
    ├── data.js         # Sumber Data Dummy (Pengguna, Katalog, Tracking)
    └── script.js       # Logika Interaktif JavaScript (DOM, Keranjang, Tema)