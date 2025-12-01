# DailyCup — Pratinjau Lokal

Proyek kecil ini berisi `Home.html` (halaman hero) dan folder `assets/` yang berisi placeholder SVG.

Cara melihat pratinjau:
1. Buka PowerShell dan masuk ke folder proyek:

```powershell
cd C:\Users\DELL\Documents\DailyCup
```

2. Buka `Home.html` di browser default Anda:

```powershell
ii .\Home.html
```

Catatan:
- Ganti placeholder SVG di `assets/` dengan gambar Anda sendiri (PNG/JPG/SVG). Perbarui path di `Home.html` jika Anda memindahkannya.
- Untuk menggunakan font TTF/WOFF khusus untuk judul besar, tambahkan file font ke `assets/` dan deklarasikan `@font-face` di bagian `<style>` pada `Home.html`.
 - Untuk menggunakan font TTF/WOFF khusus untuk judul besar, tambahkan file font ke `assets/fonts/` dan deklarasikan `@font-face` di bagian `<style>` pada `Home.html`.

Font yang sekarang ditambahkan:
- `Staatliches` (Google Fonts) — digunakan sebagai font utama untuk judul besar agar lebih mirip desain Anda.

- `Quantico` (Google Fonts) — sekarang ditambahkan dan dipakai untuk heading utama; mendukung regular, bold, dan italic.

Contoh `@font-face` jika Anda ingin menggunakan file lokal (`assets/fonts/MyFont.woff2`):

```css
@font-face {
	font-family: 'MyCustomTitle';
	src: url('assets/fonts/MyFont.woff2') format('woff2');
	font-weight: 700;
	font-style: normal;
	font-display: swap;
}
.big-title { font-family: 'MyCustomTitle', 'Staatliches', 'Russo One', sans-serif; }
```