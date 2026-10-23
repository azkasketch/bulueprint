# DOKUMEN 02: SKEMA DATA & SEED DATA LENGKAP
## Proyek: FoodWaste Hero

---

## 1. ARSITEKTUR DATA (localStorage JSON)
Karena kompetisi membatasi waktu hands-on coding 3 jam, seluruh state dan data persistent disimpan di `localStorage` browser [cite: 14].

### Struktur Koleksi:
1. `foodwaste_merchants`: Array object data toko/resto.
2. `foodwaste_postings`: Array object Surprise Box yang ditawarkan.
3. `foodwaste_bookings`: Array object transaksi klaim konsumen.

---

## 2. SKEMA ENTITAS

```json
// Merchants
{
  "id": "m1",
  "name": "Roti O Ngagel",
  "category": "Bakery",
  "address": "Jl. Ngagel Jaya No. 12",
  "lat": -7.2891,
  "lng": 112.7521,
  "rating": 4.8
}

// Postings (Surprise Box)
{
  "id": "p1",
  "merchantId": "m1",
  "title": "Surprise Box Pastry & Roti",
  "originalPrice": 50000,
  "discountPrice": 15000,
  "stock": 5,
  "pickupTime": "20:00 - 21:30",
  "image": "https://images.unsplash.com/photo-1509440159596-0249088772ff?w=500",
  "weightKg": 0.8
}

// Bookings
{
  "id": "b1",
  "postingId": "p1",
  "customerName": "Budi Santoso",
  "customerPhone": "08123456789",
  "qty": 2,
  "totalPrice": 30000,
  "status": "CLAIMED",
  "timestamp": "2026-10-19T18:30:00Z"
}
```
