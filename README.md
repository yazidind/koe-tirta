# koe-tirta

Kelompok 2
1. yazid indra sangun (23083000094)


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