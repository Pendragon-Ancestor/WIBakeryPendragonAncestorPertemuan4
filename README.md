# 🥖 WIB Bakery - Aplikasi Flutter Pemesanan Roti & Kue

**Proyek Akhir Pemrograman Mobile - Kelompok 1**

Aplikasi mobile untuk pesan roti dan kue online dengan fitur customer dan admin dashboard.

---

## 🚀 QUICK START (5 Menit Jalan)

### 1️⃣ Install & Run
```bash
# Clone project
git clone https://github.com/Pendragon-Ancestor/WIBakeryPendragonAncestorPertemuan4.git
cd wib_bakery

# Install dependencies
flutter pub get

# Run di emulator / device
flutter run
```

**Selesai! Aplikasi akan terbuka dalam 1-2 menit** ✅

---

## 📱 Akun Demo (Copy-Paste Langsung)

### 👨‍💼 **Login sebagai Admin**
```
Email:    admin@wibbakery.com
Password: admin123
```

### 👤 **Login sebagai Customer**
```
Email:    fanduy@gmail.com
Password: customer123
```

---

## ✨ Fitur yang Bisa Dicek

### 🛍️ **Customer Features (Login pakai customer account)**

1. **Browse Produk**
   - Home tab → Scroll lihat roti/kue
   - Tap produk untuk detail

2. **Belanja**
   - Pilih jumlah → "Tambah ke Keranjang"
   - Tap ikon keranjang → lihat item

3. **Checkout**
   - "Proceed to Checkout"
   - Isi alamat → "Confirm Order"

4. **Lihat Pesanan**
   - Tab "Orders" → Status pesanan

### 🛠️ **Admin Features (Login pakai admin account)**

1. **Dashboard**
   - Lihat total penjualan & order

2. **Tambah Produk**
   - Tab "Products" → "Add Product"
   - Isi nama, harga, deskripsi → Save

3. **Manage Orders**
   - Tab "Orders" → Update status pesanan

4. **Manage Promo**
   - Tab "Promo" → "Add Promo"
   - Isi kode & diskon → Save

---

## 🔧 Troubleshooting

### ❌ Error: "flutter: command not found"
```bash
# Tambah flutter ke PATH
export PATH="$PATH:~/flutter/bin"
```

### ❌ Error: "Android SDK not found"
- Buka Android Studio → SDK Manager → Install Android SDK

### ❌ Emulator lambat?
- Pakai device Android fisik (lebih cepat)

### ❌ Build error?
```bash
flutter clean
flutter pub get
flutter run
```

---

## 📋 Step-by-Step Testing

### ✅ Test 1: Login Customer
1. Klik "Login"
2. Email: `fanduy@gmail.com`
3. Password: `customer123`
4. Klik "Login" → Masuk ke Home ✓

### ✅ Test 2: Browse & Add Cart
1. (Sudah login)
2. Home → Scroll lihat produk
3. Tap "Roti Sisir"
4. Quantity = 2
5. Klik "Tambah ke Keranjang" ✓
6. Tap ikon keranjang → Lihat 2 item ✓

### ✅ Test 3: Checkout
1. Tap ikon keranjang
2. Klik "Proceed to Checkout"
3. Isi alamat pengiriman
4. Klik "Confirm Order" ✓
5. Tab "Orders" → Lihat pesanan ✓

### ✅ Test 4: Admin Login
1. Logout (swipe menu kiri)
2. Klik "Login"
3. Email: `admin@wibbakery.com`
4. Password: `admin123`
5. Masuk Admin Dashboard ✓

### ✅ Test 5: Admin Add Product
1. (Login sebagai admin)
2. Tab "Products"
3. Klik "+" atau "Add Product"
4. Isi:
   - Name: "Donat Coklat"
   - Category: "Kue"
   - Price: "15000"
   - Description: "Donat enak"
   - Stock: "20"
5. Klik "Save" ✓
6. Produk baru muncul di list ✓

### ✅ Test 6: Admin Add Promo
1. Tab "Promo"
2. Klik "Add Promo"
3. Isi:
   - Code: "DISKON10"
   - Discount: "10"
4. Klik "Save" ✓

---

## 📁 Project Structure

```
lib/
├── main.dart              ← Main app
├── features/
│   ├── auth/              ← Login/Register
│   ├── products/          ← Browse produk
│   ├── cart/              ← Keranjang belanja
│   ├── orders/            ← Lihat pesanan
│   ├── admin/             ← Admin dashboard
│   └── promo/             ← Promo system
├── core/
│   ├── models/            ← Data structures
│   ├── database/          ← SQLite
│   └── theme/             ← Colors & UI
└── assets/                ← Images
```

---

## 🛠️ Tech Stack

- **Frontend:** Flutter 3.0+, Dart 3.0+
- **State Management:** Provider
- **Database:** SQLite (local)
- **Design:** Material Design 3

---

## 📊 File Penting

| File | Fungsi |
|------|--------|
| `lib/main.dart` | Entry point |
| `lib/features/auth/` | Login/Register |
| `lib/features/products/` | Katalog produk |
| `lib/features/admin/` | Admin dashboard |
| `lib/core/database/` | Database SQLite |
| `pubspec.yaml` | Dependencies |

---

## 🗄️ Database (Local SQLite)

Data disimpan **lokal** di device. Database auto-created saat app pertama dibuka.

**Tables:**
- `users` - Login data
- `products` - Katalog
- `orders` - Pesanan
- `cart_items` - Keranjang
- `promos` - Kode promo

---

## 📝 Catatan

- **Database:** Lokal, tidak ada server
- **Pembayaran:** Simulasi
- **Notifikasi:** Basic
- **Auth:** Email + Password

---

## ✅ Checklist untuk Dosen

- [x] Login/Register (2 role)
- [x] Product Catalog
- [x] Shopping Cart
- [x] Order Management
- [x] Admin Dashboard
- [x] Promo System
- [x] SQLite Database
- [x] Responsive UI
- [x] State Management
- [x] Clean Code

---

## 🎯 Yang Perlu Diperhatikan Saat Presentasi

1. **Show Login** → Demo 2 role (Admin vs Customer)
2. **Customer Flow** → Browse → Cart → Checkout → Order
3. **Admin Flow** → Dashboard → Add Product → Manage Orders
4. **Highlight** → Promo, Order Tracking, real-time status

---

**Ready to test? Follow QUICK START di atas! 🔥**

*Last Updated: October 2026*
