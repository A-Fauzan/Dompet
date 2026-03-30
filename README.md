# 🏡 Dompet Keluarga — Fauzan & Venska

> Aplikasi pencatatan keuangan keluarga berbasis web. Ringan, gratis, tanpa server, tanpa langganan.

![preview](https://img.shields.io/badge/status-ready-4CAF82?style=flat-square) ![license](https://img.shields.io/badge/license-MIT-C8865C?style=flat-square) ![platform](https://img.shields.io/badge/platform-web%20%7C%20mobile-blue?style=flat-square)

---

## ✨ Fitur

| Fitur | Keterangan |
|-------|-----------|
| 💰 Catat pemasukan & pengeluaran | Manual dengan form atau import teks dari WhatsApp |
| 📊 Grafik per kategori | Pie chart pengeluaran & pemasukan per bulan |
| 📈 Tren 6 bulan | Bar chart perbandingan masuk vs keluar |
| 📋 Riwayat lengkap | Filter, search, hapus transaksi |
| 📱 Responsif | Bisa diakses dari HP maupun laptop |
| 💾 Penyimpanan lokal | Data tersimpan di `localStorage` browser, tanpa server |
| 📲 Input cepat WA | Paste teks dari WhatsApp → auto-detect kategori |

---

## 🗂️ Kategori

**Pengeluaran:** Makan & Minum · Transportasi · Belanja · Tagihan · Kesehatan · Pendidikan · Si Kecil 🍼 · Hiburan · Perawatan · Lainnya

**Pemasukan:** Gaji · Freelance · Hadiah/THR · Investasi · Lainnya

---

## 🚀 Deploy Gratis

File ini adalah **satu file HTML mandiri** — tidak perlu backend, database, atau NPM sama sekali.

### Opsi 1 — GitHub Pages *(rekomendasi)*

> Cocok kalau sudah punya akun GitHub. URL tetap & bisa diperbarui kapan saja.

1. **Buat repositori baru** di [github.com/new](https://github.com/new)
   - Nama repo: `dompet-keluarga` (atau bebas)
   - Visibility: **Public** (diperlukan untuk GitHub Pages gratis)
   - Klik **Create repository**

2. **Upload file**
   - Klik **Add file → Upload files**
   - Upload `dompet-keluarga.html` dan `README.md`
   - **Penting:** rename `dompet-keluarga.html` menjadi `index.html` sebelum upload agar URL langsung terbuka tanpa nama file

3. **Aktifkan GitHub Pages**
   - Buka tab **Settings** di repo
   - Scroll ke **Pages** (sidebar kiri)
   - Source: pilih **Deploy from a branch**
   - Branch: `main` → folder `/root (/)` → klik **Save**

4. **Tunggu 1–2 menit**, lalu URL kamu aktif:
   ```
   https://<username>.github.io/dompet-keluarga/
   ```

✅ Selesai. Bagikan URL ke Venska — bisa langsung dibuka dari HP.

---

### Opsi 2 — Netlify Drop *(paling cepat, <1 menit)*

> Tanpa daftar, tanpa GitHub. Cocok untuk deploy instan.

1. Buka [app.netlify.com/drop](https://app.netlify.com/drop)
2. **Drag & drop** file `index.html` ke area yang tersedia
3. URL langsung aktif dalam hitungan detik, contoh:
   ```
   https://shiny-alpaca-abc123.netlify.app
   ```
4. *(Opsional)* Daftar akun Netlify gratis untuk ganti URL jadi lebih rapi

---

### Opsi 3 — Vercel *(jika mau domain custom nanti)*

1. Buka [vercel.com](https://vercel.com) → daftar dengan GitHub
2. **New Project → Import** repo GitHub yang sudah dibuat di Opsi 1
3. Klik Deploy — URL langsung aktif:
   ```
   https://dompet-keluarga.vercel.app
   ```

---

## 📲 Input Cepat dari WhatsApp

Di halaman **Tambah**, tersedia fitur *Input Cepat dari WhatsApp*:

1. Copy beberapa baris teks dari chat WA (pengeluaran/pemasukan hari ini)
2. Paste di kolom yang tersedia
3. Klik **Analisa Teks**
4. App otomatis mendeteksi kategori dari kata kunci:

| Kata kunci | Kategori |
|-----------|---------|
| bensin, ojek, grab, parkir | Transportasi |
| makan, warung, bakso, kopi | Makan & Minum |
| listrik, wifi, tagihan, token | Tagihan |
| susu, pampers, shafiyyah, athiyyah | Si Kecil 🍼 |
| gaji, salary | Gaji |
| freelance, proyek, klien | Freelance |

5. Klik **Simpan Semua** — semua transaksi langsung tersimpan

---

## 💡 Tips Penggunaan

- **Navigasi bulan** — gunakan tombol `‹` dan `›` di header untuk pindah bulan
- **Hapus transaksi** — buka tab Riwayat → klik **hapus** di transaksi yang ingin dihapus
- **Data tidak hilang** — tersimpan di browser lokal (`localStorage`). Jangan hapus data browser / gunakan mode Incognito
- **Backup data** — buka DevTools (F12) → Console → ketik `localStorage.getItem('fv_dompet_v2')` → copy hasilnya sebagai backup JSON

---

## 🔮 Pengembangan Selanjutnya

- [ ] Integrasi Telegram Bot untuk input otomatis tanpa buka browser
- [ ] Export data ke Excel/CSV
- [ ] Notifikasi jika pengeluaran melewati budget
- [ ] Sinkronisasi data antar perangkat (Fauzan & Venska)
- [ ] Mode multi-bulan untuk laporan tahunan

---

## 🛠️ Teknologi

- **React 18** — UI framework (via CDN, tanpa build step)
- **Recharts** — grafik pie & bar
- **localStorage** — penyimpanan data lokal di browser
- **Google Fonts** — Playfair Display + Plus Jakarta Sans

---

## 📄 Lisensi

MIT — bebas dipakai dan dimodifikasi.

---

*Dibuat dengan ❤️ untuk keluarga kecil Fauzan & Venska — dan dua malaikat kecil Shafiyyah & Athiyyah 🍼*
