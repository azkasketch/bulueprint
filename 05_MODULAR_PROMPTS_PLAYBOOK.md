# DOKUMEN 05: PLAYBOOK PROMPTING BERTINGKAT (TAHAP DEMI TAHAP)
## Proyek: FoodWaste Hero

---

> **STRATEGI VIBECODING 3 JAM IT FEST** [cite: 14]
> Kirimkan prompt bertahap berikut ke AI Tools (Cursor / ChatGPT / Claude) untuk membangun aplikasi utuh tanpa error [cite: 14].

### TAHAP 1: HTML Skeleton & Layout Styling (Tailwind CSS)
```text
Buatkan struktur HTML dasar Single Page Application untuk 'FoodWaste Hero' menggunakan Tailwind CSS CDN dan FontAwesome. 
Sediakan Header modern dengan logo hijau, Live Impact Counter (2 stat card: Porsi Diselamatkan & CO2 Dicegah), serta layout grid 2 kolom (Kiri: Peta LeafletJS, Kanan: Grid Card Makanan). Gunakan warna Emerald Green dan Food Orange.
```

### TAHAP 2: Inisialisasi Data & Map LeafletJS
```text
Tambahkan script JavaScript vanilla untuk inisialisasi LeafletJS Map pada div #map dengan koordinat Surabaya (-7.2891, 112.7521). 
Buat seed data JSON 4 merchant resto dan postingan 'Surprise Box' ke localStorage jika belum ada. Render pin resto di peta beserta popup info ringkasnya.
```

### TAHAP 3: Dynamic Product Card Rendering & Filter
```text
Buat fungsi renderPostings() yang mengambil data dari localStorage dan merender kartu produk secara dinamis ke grid. 
Sertakan fitur filter kategori (All, Bakery, Resto) dan fungsi pencarian teks yang secara otomatis memfilter tampilan kartu.
```

### TAHAP 4: Modal Booking & Impact Calculation Real-time
```text
Tambahkan fitur modal booking ketika tombol 'Klaim Porsi' diklik. Saat form diisi dan disubmit, kurangi stok postingan terkait di localStorage, catat booking baru, dan perbarui nilai Live Impact Counter secara real-time tanpa reload halaman.
```
