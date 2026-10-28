# koe-tirta

Kelompok 2
1. yazid indra sangun (23083000094)


# KoeTirta - Sistem Pemesanan Kopi

Sistem pemesanan kopi berbasis web untuk melihat katalog,
memilih varian kopi, melakukan checkout, membayar melalui
transfer bank, dan mengambil pesanan di lokasi KoeTirta.

## Teknologi

- Next.js
- React.js
- TypeScript
- PostgreSQL
- REST API
- Google OAuth 2.0

## Struktur Proyek

koe-tirta/
├── public/
│   ├── images/
│   │   ├── products/
│   │   └── logo.png
│   └── icons/
│
├── src/
│   ├── app/
│   │   ├── (public)/
│   │   │   ├── login/
│   │   │   │   └── page.tsx
│   │   │   ├── katalog/
│   │   │   │   └── page.tsx
│   │   │   ├── produk/
│   │   │   │   └── [slug]/
│   │   │   │       └── page.tsx
│   │   │   └── layout.tsx
│   │   │
│   │   ├── (customer)/
│   │   │   ├── checkout/
│   │   │   │   └── page.tsx
│   │   │   └── pesanan/
│   │   │       ├── page.tsx
│   │   │       └── [orderNumber]/
│   │   │           ├── page.tsx
│   │   │           └── pembayaran/
│   │   │               └── page.tsx
│   │   │
│   │   ├── admin/
│   │   │   ├── page.tsx
│   │   │   ├── kategori/
│   │   │   │   └── page.tsx
│   │   │   ├── produk/
│   │   │   │   ├── page.tsx
│   │   │   │   └── [id]/
│   │   │   │       ├── page.tsx
│   │   │   │       └── varian/
│   │   │   │           └── page.tsx
│   │   │   ├── pembayaran/
│   │   │   │   └── page.tsx
│   │   │   └── pesanan/
│   │   │       └── page.tsx
│   │   │
│   │   ├── superadmin/
│   │   │   ├── users/
│   │   │   │   └── page.tsx
│   │   │   └── riwayat-role/
│   │   │       └── page.tsx
│   │   │
│   │   ├── layout.tsx
│   │   ├── page.tsx
│   │   └── globals.css
│   │
│   ├── components/
│   │   ├── layout/
│   │   ├── ui/
│   │   ├── catalog/
│   │   ├── orders/
│   │   └── forms/
│   │
│   ├── lib/
│   │   ├── api.ts
│   │   ├── auth.ts
│   │   ├── validations.ts
│   │   └── utils.ts
│   │
│   ├── types/
│   │   ├── user.ts
│   │   ├── product.ts
│   │   └── order.ts
│   │
│   └── services/
│       ├── auth.service.ts
│       ├── catalog.service.ts
│       ├── order.service.ts
│       └── payment.service.ts
│
├── database/
│   ├── schema.sql
│   ├── seed.sql
│   └── README.md
│
├── .env.example
├── .gitignore
├── eslint.config.mjs
├── next.config.ts
├── package.json
├── package-lock.json
├── postcss.config.mjs
├── tsconfig.json
└── README.md

## Persyaratan

- Node.js versi LTS yang kompatibel dengan Next.js
- npm
- PostgreSQL
- Git

## Instalasi

1. Clone repository.

   ```bash
   git clone <URL_REPOSITORY>
   cd koe-tirta
   ```

2. Instal dependency.

   ```bash
   npm install
   ```

3. Siapkan database PostgreSQL.

4. Jalankan schema dan seed SQL melalui
   PostgreSQL client atau pgAdmin.

5. Salin `.env.example` menjadi `.env.local`,
   kemudian isi konfigurasi sesuai kebutuhan.

6. Jalankan aplikasi.

   ```bash
   npm run dev
   ```

7. Buka http://localhost:3000

## Modul Sistem

1. Autentikasi Google dan manajemen pengguna
2. Katalog kategori dan produk kopi
3. Varian produk dan manajemen stok
4. Checkout dan transaksi pesanan
5. Verifikasi pembayaran
6. Pengelolaan status pesanan
7. Manajemen role dan riwayat perubahan role

## Database

Database menggunakan PostgreSQL dengan sembilan tabel:

- roles
- users
- role_change_logs
- categories
- products
- product_variants
- orders
- order_items
- payments

File SQL berada di folder `database/`.

## Pembagian Tugas Anggota

| Nama Anggota | Nama Modul | Tabel yang Dikelola | Halaman Antarmuka |
|---|---|---|---|
| Muhammad Arya S | Autentikasi & Manajemen Role | roles, users, role_change_logs | U1, S1, S2 |
| Daeven Natan S M | Manajemen Katalog | categories, products | U2, U3, A2, A3, A4 |
| Yazid Indra Sangun | Varian, Stok & Pesanan | product_variants, orders | A5, A7, U6, U7 |
| Alfredo Budi Dwi S | Checkout & Pembayaran | order_items, payments | U4, U5, A1, A6 |

## Workflow Git

- `main`: development, testing, dan perbaikan fitur.
- `production`: kode yang telah diuji dan siap dirilis.

Alur kerja:

1. Kerjakan fitur pada branch `main`.
2. Commit dan push ke `main`.
3. Lakukan pengujian.
4. Buat Pull Request dari `main` ke `production`.
5. Merge setelah perubahan dinyatakan siap.

## Status Pengembangan

- [ ] Setup Next.js
- [ ] Setup PostgreSQL
- [ ] Autentikasi Google
- [ ] Katalog produk
- [ ] Manajemen varian dan stok
- [ ] Checkout dan transaksi
- [ ] Verifikasi pembayaran
- [ ] Pengelolaan pesanan
- [ ] Manajemen role
- [ ] Pengujian dan integrasi