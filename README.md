# 🧩 Admin Dashboard Template (HTML/CSS)

This is a simple and clean **HTML/CSS admin dashboard template**, designed as a starting point for coding tests or quick integration with frameworks like Laravel, Node.js, or others.

## 📦 What's Included

- Plain HTML pages (no build tools needed)
- Responsive layout (basic)
- Sidebar navigation
- Top navbar
- Dashboard homepage with sample card layout
- Basic table & form styles
- CSS (pure CSS or Bootstrap 5 depending on version)

---

## 📘 Use Case (For Coding Test)

This template is intended for use during coding tests, where candidates are expected to:

1. Integrate this front-end with a backend (e.g., Laravel, Express).
2. Build functional CRUD operations while reusing the existing HTML/CSS layout.
3. Focus on functionality rather than UI design.

---

## 🧪 Soal Coding Laravel – CRUD Transaksi dengan Autentikasi & Produk

1. Buat aplikasi Laravel untuk mengelola **transaksi penjualan** dan **produk**, lengkap dengan fitur login.
2. Fitur autentikasi (bebas menggunakan Breeze, Jetstream, dll):
   - Tampilkan halaman login dan register.
   - Hanya pengguna yang sudah login bisa mengakses data produk dan transaksi.
3. Buat modul **produk** dengan fitur CRUD dan kolom:
   - `id` (otomatis)
   - `nama_produk`
   - `deskripsi`
   - `foto` (upload file gambar, simpan ke storage)
   - `harga`
4. Buat modul **transaksi** dengan fitur CRUD dan kolom:
   - `id` (otomatis)
   - `nama_pelanggan`
   - `produk_id` (relasi ke produk, dipilih dari dropdown)
   - `jumlah`
   - `total_harga` (otomatis dihitung: jumlah x harga produk)
   - `tanggal_transaksi` (default: tanggal hari ini)
5. Total harga **tidak diinput manual**, tetapi dihitung otomatis di backend berdasarkan produk yang dipilih. Bisa memilih lebih dari 1 produk.
6. Buat tampilan menggunakan **Blade template**, dengan:
   - Dashboard setelah login
   - Daftar produk dan transaksi (dalam tabel)
   - Form tambah/edit produk dan transaksi
   - Tampilkan pesan sukses atau error setelah aksi simpan/hapus
7. Untuk upload foto produk:
   - Simpan file ke folder `/storage/app/public`
   - Tampilkan foto dengan URL `asset('storage/…')`
8. Lakukan **validasi semua input** (gunakan FormRequest jika bisa):
   - Nama produk dan harga wajib
   - Jumlah transaksi minimal 1
   - Foto hanya menerima file gambar (jpg/png)
9. Tambahkan `middleware auth` agar halaman hanya bisa diakses setelah login.
10. Waktu pengerjaan: **maksimal 4 jam**
11. Opsional (Bonus):
    - Tambahkan fitur pencarian produk berdasarkan nama
    - Tambahkan filter transaksi berdasarkan tanggal
    - Jika mampu, pisahkan peran admin (kelola produk) dan user (input transaksi)
12. Upload hasilnya ke GitHub masing-masing, lalu kirimkan link repository ke HRD.

---

## 🚫 Aturan Tes (DILARANG)

- Tidak diperbolehkan menggunakan AI seperti:
- ChatGPT, GitHub Copilot, Bing AI, Google Gemini, dll
- Tidak boleh membuka situs seperti GitHub, YouTube, dan sejenisnya.
- Hanya boleh menggunakan dokumentasi Laravel atau PHP.
- Tes dikerjakan secara **mandiri** dan akan diawasi.
- Kode harus bisa dijelaskan saat sesi review/interview.