<div align="center">

# JATI<span>e</span>

**Furniture Jati, Langsung dari Pengrajin**

Website demo katalog furniture kayu jati bergaya sinematik, responsif, dan siap memesan lewat WhatsApp.

[Lihat Demo](https://jatie.vercel.app) · [Instagram](https://instagram.com/misbah_smply)

![Next.js](https://img.shields.io/badge/Next.js-App_Router-black?logo=nextdotjs)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?logo=typescript&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-06B6D4?logo=tailwindcss&logoColor=white)
![Vercel](https://img.shields.io/badge/Deploy-Vercel-black?logo=vercel)

</div>

---

## Tentang Proyek

**JATIe** adalah website demo toko furniture kayu jati dengan data fiktif. Proyek ini dibuat sebagai **portofolio jasa pembuatan website untuk UMKM**, untuk menunjukkan seperti apa website katalog produk yang modern, cepat, dan mengarahkan pengunjung langsung memesan lewat WhatsApp.

> ⚠️ **Website Demo.** Semua nama produk, harga, alamat, dan testimoni adalah data fiktif untuk keperluan portofolio.

## Fitur

- 🎬 **Tampilan sinematik**: hero layar penuh, film grain, animasi masuk bertahap, parallax halus, dan smooth scroll
- 📱 **Responsif penuh**: mobile-first, diuji dari 360px sampai 1536px+
- 🛋️ **Katalog produk**: filter kategori, pencarian, dan pengurutan harga
- 📄 **Halaman detail produk** statis dengan galeri foto, spesifikasi, dan produk serupa
- 💬 **Pesan via WhatsApp**: pesan otomatis terisi nama produk, harga, dan tautan halaman
- 📝 **Custom order**: form permintaan furniture sesuai ukuran, dikirim sebagai pesan WhatsApp terformat
- 🔍 **SEO siap pakai**: metadata per halaman, Open Graph, sitemap, dan robots
- ♿ **Aksesibel**: kontras memenuhi WCAG AA, navigasi keyboard, dan menghormati `prefers-reduced-motion`

## Halaman

| Rute | Isi |
|---|---|
| `/` | Beranda: hero, keunggulan, statistik, kategori, produk terlaris, proses pembuatan, testimoni |
| `/katalog` | Daftar produk dengan filter, pencarian, dan urutan |
| `/produk/[slug]` | Detail produk |
| `/custom-order` | Form pesanan custom |
| `/tentang` | Cerita pengrajin dan nilai brand |
| `/kontak` | WhatsApp, alamat workshop, jam buka, peta |
| `404` | Halaman tidak ditemukan bermerek |

## Tech Stack

- [Next.js](https://nextjs.org/) (App Router)
- [TypeScript](https://www.typescriptlang.org/)
- [Tailwind CSS](https://tailwindcss.com/)
- [Motion](https://motion.dev/) untuk animasi
- [Lenis](https://lenis.darkroom.engineering/) untuk smooth scroll
- [Lucide React](https://lucide.dev/) untuk ikon
- Deploy di [Vercel](https://vercel.com/)

## Menjalankan di Komputer

**Prasyarat:** Node.js versi LTS.

```bash
# 1. Clone repo
git clone https://github.com/USERNAME/jatie.git
cd jatie

# 2. Install dependensi
npm install

# 3. Salin file environment
cp .env.example .env.local

# 4. Jalankan mode pengembangan
npm run dev
```

Buka [http://localhost:3000](http://localhost:3000) di browser.

### Perintah lain

```bash
npm run build   # build untuk produksi
npm run start   # jalankan hasil build
npm run lint    # cek kode
```

## Konfigurasi

### Nomor WhatsApp

Ubah di file `.env.local`:

```env
NEXT_PUBLIC_WA_NUMBER=6281234567890
```

Gunakan format internasional tanpa tanda `+` dan tanpa angka `0` di depan (contoh: `6281234567890`).

### Mengganti produk

Edit file `data/products.ts`. Setiap produk memiliki `nama`, `kategori`, `harga`, `deskripsi`, `gambar`, `spesifikasi`, dan penanda `terlaris`. Halaman katalog dan detail produk terbuat otomatis dari data ini.

### Mengganti info toko

Edit file `data/site.ts` untuk nama brand, tagline, alamat, jam buka, dan username Instagram.

### Mengganti foto

Foto contoh memakai Unsplash. Ganti URL pada `data/products.ts`, atau letakkan foto sendiri di folder `public/` lalu arahkan path-nya. Untuk hasil terbaik, pakai foto beresolusi tinggi dengan rasio lebar.

## Deploy ke Vercel

1. Push proyek ini ke GitHub.
2. Buka [vercel.com](https://vercel.com), lalu pilih **Add New → Project** dan import repo `jatie`.
3. Pada **Environment Variables**, tambahkan `NEXT_PUBLIC_WA_NUMBER` dengan nomor WhatsApp kamu.
4. Klik **Deploy**.

Setiap kali kamu push ke GitHub, Vercel akan otomatis memperbarui website.

## Struktur Folder

```
jatie/
├── app/            # Halaman dan layout (App Router)
├── components/     # Komponen reusable
├── data/           # Data produk dan info situs
├── lib/            # Helper (format Rupiah, link WhatsApp)
├── public/         # Aset statis
├── AGENTS.md       # Petunjuk untuk agent AI
└── .env.example    # Contoh environment variable
```

## Ingin Website Seperti Ini untuk Usahamu?

Saya menerima jasa pembuatan website untuk UMKM: toko online, company profile, dan landing page.

📩 Hubungi lewat Instagram [@misbah_smply](https://instagram.com/misbah_smply)

## Lisensi dan Hak Cipta

© 2026 misbah_smply. All rights reserved.

Proyek ini adalah karya portofolio. Foto produk bersumber dari Unsplash dan hak ciptanya milik masing-masing fotografer.
