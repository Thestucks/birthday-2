# 📸 Foto — Memory Album

Website menampilkan **semua foto** yang ditaruh di folder ini
(`public/assets/photos/`). Saat ini yang dipakai: `p1.jpg`–`p4.jpg` dan `r1.jpg`–`r2.jpg`.

## Cara menambah / mengganti / menghapus foto

Edit daftar `gallery.items` di **`src/data/content.js`**:

```js
items: [
  { src: 'p1.jpg', category: 'star',   alt: 'Foto Dummy 1' },
  { src: 'r1.jpg', category: 'memori', alt: 'Foto Dummy Kenangan 1' },
  // tambah / kurangi baris sesuai file di folder ini
],
```

- `src` → nama file persis seperti di folder ini.
- `category` → salah satu dari `star`, `heartopia`, `memori` (menentukan label + caption + warna aksen, lihat `gallery.categories`).
- `alt` → deskripsi singkat untuk aksesibilitas.

## Catatan

- Format disarankan `.jpg` / `.jpeg` / `.png` / `.webp`, rasio ± 4:5 (portrait) agar pas di bingkai polaroid.
- Jika sebuah file belum ada, kartu menampilkan ilustrasi placeholder orisinal (tidak error).
