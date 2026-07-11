# Dharma Justicia Law Firm

Situs statis (satu file `index.html`, tanpa dependensi build) untuk **Dharma Justicia Law Firm** — firma hukum perdata, korporasi, dan litigasi di Bandung, Jawa Barat.

Konten diekstrak dan dibersihkan dari halaman Wix asli, lalu ditulis ulang sebagai HTML/CSS/JS statis murni agar ringan dan mudah di-host di GitHub Pages.

## Struktur

```
.
├── index.html   # seluruh markup, style, dan script ada di satu file ini
└── README.md
```

## Cara deploy ke GitHub Pages

1. Buat repository baru di GitHub, lalu upload `index.html` (dan `README.md` ini) ke root repo.
2. Buka **Settings → Pages** pada repo tersebut.
3. Pada **Source**, pilih branch `main` dan folder `/ (root)`, lalu **Save**.
4. Tunggu beberapa menit — situs akan tersedia di `https://<username>.github.io/<nama-repo>/`.

## Cara menjalankan secara lokal

Cukup buka `index.html` langsung di browser, atau jalankan server statis sederhana:

```bash
python3 -m http.server 8000
```

lalu buka `http://localhost:8000`.

## Kustomisasi

- **Konten & data tim**: edit langsung di bagian `<section class="team">` pada `index.html`.
- **Warna & tipografi**: seluruh token desain ada di `:root { ... }` pada bagian `<style>`.
- **Kontak**: perbarui nomor telepon, email, dan alamat pada `<section class="contact">`.
