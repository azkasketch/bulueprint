# DOKUMEN 04: SPESIFIKASI KOMPONEN FRONTEND & UI WIREFRAME
## Proyek: FoodWaste Hero

---

## 1. DESIGN SYSTEM & COLOR PALETTE
- **Primary Color:** `#10B981` (Emerald Green - melambangkan keberlanjutan & kelestarian)
- **Secondary Color:** `#F97316` (Food Orange - melambangkan selera makan & kehangatan)
- **Background:** `#F8FAFC` (Clean Slate)
- **Typography:** Inter / Plus Jakarta Sans (via Google Fonts / Tailwind Standard)

---

## 2. STRUKTUR KOMPONEN UI
1. **Navbar & Impact Header:**
   - Logo FoodWaste Hero + Badge "SDG 12 & 2 Action" [cite: 4].
   - Banner Live Counter: **"1,240 Porsi Diselamatkan"** & **"310 kg CO2 Dicegah"** [cite: 14].
2. **Filter & Search Bar:**
   - Input pencarian nama merchant/makanan.
   - Button group filter: *Semua*, *Bakery*, *Restoran*, *Minimarket*.
3. **Interactive Leaflet Map Container:**
   - Div tempat render peta interaktif dengan custom icon pin resto [cite: 14].
4. **Product Card Grid:**
   - Gambar produk, badge kategori, diskon % tag, perbandingan harga coret vs harga promo, jam batas ambil, stok sisa, dan button klaim [cite: 14].
5. **Modal Form (Popup Booking & Merchant Add Item):**
   - Modal interaktif cepat dengan Tailwind transition [cite: 14].
