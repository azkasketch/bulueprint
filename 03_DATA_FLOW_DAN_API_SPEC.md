# DOKUMEN 03: DATA FLOW, STATE MANAGEMENT & KONTRAK FUNGSI
## Proyek: FoodWaste Hero

---

## 1. ALUR TRANSAKSI & PENGELOLAAN STOK
1. **Pengambilan Data:** Komponen UI membaca data dari `localStorage`. Jika kosong, sistem melakukan inisialisasi menggunakan *seed data*.
2. **Klaim Produk:**
   - Konsumen menekan tombol **"Klaim Porsi"** [cite: 14].
   - Sistem memeriksa ketersediaan `stock`.
   - Jika `stock >= qty`, `stock` berkurang, item `booking` baru disimpan ke `foodwaste_bookings`.
   - *Impact Counter* (Total Makanan & CO2) otomatis diperbarui secara sistemik [cite: 14].
3. **Penambahan Postingan Baru (Merchant View):**
   - Resto menginput judul, harga, stok, dan jam ambil via form [cite: 14].
   - Data tersimpan ke `foodwaste_postings` dan merender ulang grid produk tanpa reload halaman [cite: 14].

---

## 2. KONTRAK FUNGSI HELPER (JAVASCRIPT)
- `initStorage()`: Menyiapkan seed data awal.
- `getPostings(categoryFilter)`: Mengambil daftar makanan aktif berdasarkan kategori.
- `claimProduct(postingId, customerData)`: Mengurangi stok dan menambah data klaim.
- `calculateImpact()`: Mengkalkulasi total kg makanan yang diselamatkan ($\sum \text{qty} \times \text{weightKg}$) dan CO2 ($
\text{totalKg} \times 2.5$).
