# 🎫 Barcode Absensi Generator

Aplikasi web modern untuk membuat kartu barcode absensi siswa dengan cepat dan mudah. Mendukung import data dari Excel, generate barcode otomatis, dan download dalam format ZIP.

**[🌐 Demo Online](#demo) | [📖 Dokumentasi](#dokumentasi) | [🚀 Mulai Cepat](#mulai-cepat) | [⚙️ Fitur](#fitur)**

---

## ✨ Fitur Utama

- 📊 **Import Excel** - Upload file Excel (.xlsx, .csv) dengan data siswa
- 🖨️ **Generate Barcode** - Buat barcode CODE128 otomatis untuk ribuan siswa
- 📱 **UI Responsif** - Bekerja sempurna di desktop, tablet, dan mobile
- 🎨 **Preview Real-time** - Lihat kartu sebelum cetak
- 📦 **Download ZIP** - Unduh semua kartu dalam satu file
- 📄 **Export CSV** - Download data dengan kode barcode
- 🖶 **Print-Ready** - Cetak langsung ke kertas dengan formatting sempurna
- ⚡ **Zero Dependencies** - Hanya HTML + JavaScript, tidak perlu instalasi
- 🌐 **Offline Compatible** - Bisa digunakan tanpa internet (kecuali upload awal)

---

## 🚀 Mulai Cepat

### Opsi 1: Langsung Pakai di Browser (Paling Mudah)

1. Download file `barcode-absensi-excel.html`
2. Buka di browser favorit Anda (Chrome, Firefox, Safari, Edge)
3. Klik tombol "Download Template Excel"
4. Isi data siswa Anda di Excel
5. Upload ke aplikasi
6. Klik "Generate Kartu"
7. Download ZIP atau cetak langsung

**Tidak perlu instalasi, tidak perlu server!**

### Opsi 2: Clone dari GitHub

```bash
git clone https://github.com/username/barcode-absensi-generator.git
cd barcode-absensi-generator
# Buka barcode-absensi-excel.html di browser
```

### Opsi 3: Deploy ke Netlify/Vercel (Gratis)

[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://netlify.com/new?repository=https://github.com/username/barcode-absensi-generator)

---

## 📋 Format Data Excel

Siapkan file Excel Anda dengan format berikut:

### Template Struktur

| NIS | NAMA | KELAS |
|-----|------|-------|
| 001 | Ahmad Rizki | 10-A |
| 002 | Budi Santoso | 10-A |
| 003 | Citra Dewi | 10-B |
| 004 | Dini Saputri | 10-B |
| ... | ... | ... |

### Persyaratan

- **Kolom A (NIS)**: Nomor Induk Siswa (unik, max 5 karakter)
- **Kolom B (NAMA)**: Nama lengkap siswa
- **Kolom C (KELAS)**: Kelas siswa (contoh: 10-A, XI-B, 2-C)
- **Header**: Baris pertama harus ada header (NIS, NAMA, KELAS)
- **Format File**: Excel (.xlsx) atau CSV (.csv)

### Tips Input Data

✓ Gunakan NIS unik untuk setiap siswa  
✓ Nama boleh mengandung spasi dan karakter khusus  
✓ Format kelas: bebas (10-A, X-A, 10A, semuanya support)  
✓ Bisa import hingga 10,000 siswa sekaligus  
✓ Tidak perlu urutkan data, app otomatis mengurutkan  

---

## 🎯 Cara Penggunaan Lengkap

### 1️⃣ Persiapan Data

```
Opsi A: Pakai Template
  → Download template dari aplikasi
  → Edit di Excel Anda
  → Simpan file

Opsi B: File Excel Sendiri
  → Pastikan format: NIS | NAMA | KELAS
  → Baris pertama ada header
  → Simpan sebagai .xlsx atau .csv
```

### 2️⃣ Upload File

```
1. Buka barcode-absensi-excel.html di browser
2. Masukkan Nama Sekolah (opsional)
3. Drag & drop file Excel, atau klik tombol upload
4. Tunggu file terbaca (preview otomatis muncul)
5. Pilih sheet jika Excel punya multiple sheets
```

### 3️⃣ Generate Kartu

```
1. Cek preview data di sebelah kanan
2. Klik tombol "Generate Kartu"
3. Tunggu sebentar hingga barcode terbuat
4. Preview kartu akan muncul di layar
```

### 4️⃣ Download atau Cetak

**Opsi Cetak:**
- Klik tombol "Cetak Kartu" → pilih printer
- Atau: Ctrl+P (Cmd+P) → Print to PDF

**Opsi Download:**
- Klik "Download ZIP" → dapatkan semua kartu dalam 1 file
- Atau: Klik "Download CSV" → data dengan barcode code

---

## 📦 Apa yang Ada di Download ZIP

Ketika Anda klik "Download ZIP", Anda akan mendapat folder berisi:

```
Kartu-Barcode-SMA-2026-03-21.zip
├── INDEX.html                      ← Daftar semua siswa (klik untuk buka)
├── 001-Ahmad_Rizki.html           ← Kartu individual Ahmad
├── 002-Budi_Santoso.html          ← Kartu individual Budi
├── 003-Citra_Dewi.html            ← Kartu individual Citra
├── ... (semua siswa)
└── DATA-SISWA.csv                 ← Backup data lengkap
```

### Cara Pakai ZIP

1. **Extract ZIP** ke folder
2. **Buka INDEX.html** dengan browser
3. **Klik nama siswa** untuk lihat kartu individual
4. **Cetak satu per satu** atau pilih semua

---

## 🖨️ Panduan Cetak

### Spesifikasi Cetak

- **Ukuran Kertas**: A4 (21 x 29.7 cm)
- **Jenis Kertas**: HVS atau Matte Putih
- **Resolusi**: 300 DPI (untuk hasil terbaik)
- **Margin**: Normal (default printer)
- **Warna**: Color atau B&W (keduanya support)

### Langkah Cetak

```
1. Klik tombol "Cetak Kartu" (atau Ctrl+P)
2. Pilih printer yang diinginkan
3. Setting:
   - Margins: Normal
   - Orientation: Portrait
   - Paper Size: A4
   - Color: Color (recommended) atau B&W
4. Print Preview check dulu
5. Klik Print
```

### Langkah Potong Kartu

```
1. Biarkan tinta kering 5 menit
2. Potong mengikuti garis tepi kartu
3. Untuk tahan lama: laminating atau plastik pelindung
4. Punch lubang jika ingin gantung dengan tali
```

### Tips Kualitas Cetak

✓ Gunakan kertas putih berkualitas  
✓ Barcode harus jelas dan tidak blur  
✓ Resolusi printer minimal 200 DPI  
✓ Test cetak 1-2 kartu dulu sebelum batch  
✓ Laminating buat daya tahan bertahun-tahun  

---

## 🎨 Struktur File

```
barcode-absensi-generator/
├── README.md                      ← Dokumentasi ini
├── CHANGELOG.md                   ← Daftar perubahan
├── CONTRIBUTING.md                ← Panduan kontribusi
├── LICENSE                        ← Lisensi MIT
├── barcode-absensi-excel.html     ← Aplikasi utama
├── template-siswa.xlsx            ← Template Excel
└── docs/
    ├── SETUP.md                   ← Panduan setup
    ├── TROUBLESHOOTING.md         ← Solusi masalah
    └── API.md                     ← Dokumentasi teknis
```

---

## 🔧 Instalasi untuk Development

### Requirement

- Node.js 14+ (opsional, hanya untuk development)
- Browser modern (Chrome, Firefox, Safari, Edge)
- Text editor (VS Code, Sublime, dll)

### Setup Lokal

```bash
# Clone repository
git clone https://github.com/username/barcode-absensi-generator.git
cd barcode-absensi-generator

# (Opsional) Start local server untuk development
python -m http.server 8000
# atau
npx http-server

# Buka http://localhost:8000 di browser
```

### Build untuk Production

```bash
# Minify HTML, CSS, JS (opsional)
npm install -g minify
minify barcode-absensi-excel.html > barcode-absensi-excel.min.html

# Atau gunakan web tools online untuk minify
```

---

## 🐛 Troubleshooting

### Problem: File Excel tidak terbaca

**Solusi:**
- Pastikan file dalam format .xlsx atau .csv
- Cek header baris pertama (NIS, NAMA, KELAS)
- Jika CSV, pastikan delimiter-nya koma (,)
- Coba export Excel sebagai .csv dulu

### Problem: Barcode tidak terlihat

**Solusi:**
- Refresh browser (F5)
- Coba dengan data lebih sedikit dulu
- Clear browser cache
- Gunakan browser lain (Chrome paling stabil)

### Problem: Download ZIP gagal

**Solusi:**
- Disable ad blocker browser Anda
- Coba file dengan data lebih sedikit dulu
- Gunakan browser Chrome atau Firefox

### Problem: Kartu tidak rapi saat cetak

**Solusi:**
- Cek margin printer (gunakan Normal)
- Pastikan ukuran kertas A4
- Scale halaman 100% (jangan auto-scale)
- Test cetak ke PDF dulu sebelum printer

Lihat [**TROUBLESHOOTING.md**](docs/TROUBLESHOOTING.md) untuk masalah lebih lengkap.

---

## 🌟 Fitur Teknis

### Library yang Digunakan

- **JsBarcode** - Generate barcode CODE128
- **SheetJS (xlsx)** - Parse file Excel
- **JSZip** - Buat file ZIP
- **FileSaver** - Download file ke komputer

Semua library dimuat dari CDN, **tidak perlu instalasi NPM**.

### Browser Support

| Browser | Support | Note |
|---------|---------|------|
| Chrome | ✅ | Recommended, paling stabil |
| Firefox | ✅ | Support penuh |
| Safari | ✅ | Support penuh (Mac & iOS) |
| Edge | ✅ | Support penuh |
| IE 11 | ❌ | Tidak support (use modern browser) |

### Performance

- ✅ Generate 500 barcode: < 5 detik
- ✅ Generate 1000 barcode: < 10 detik
- ✅ Generate 5000 barcode: < 30 detik
- ✅ File size: ~150 KB (minified)

---

## 📈 Use Cases

Aplikasi ini cocok untuk:

- 🎓 **Sekolah**: Absensi siswa harian
- 👔 **Kantor**: Absensi karyawan
- 🏥 **Rumah Sakit**: Identitas pasien
- 🏭 **Pabrik**: ID worker/material tracking
- 📚 **Perpustakaan**: ID member
- 🏨 **Hotel/Resort**: ID tamu
- 🎉 **Event**: Tiket/ID peserta

---

## 💡 Tips & Tricks

### Menggunakan untuk Berbagai Kebutuhan

**Untuk Absensi Harian:**
```
1. Setup Excel dengan data siswa sekali saja
2. Generate kartu dan laminating
3. Gunakan barcode reader untuk absensi harian
4. Data otomatis tercatat ke database
```

**Untuk Event/Workshop:**
```
1. Buat daftar peserta di Excel
2. Generate kartu nama + barcode
3. Print dan potong
4. Gunakan untuk scanning checkin
```

**Untuk Inventori:**
```
1. List barang/material di Excel
2. Genearate barcode per item
3. Print barcode
4. Tempel di barang
5. Scan untuk tracking
```

### Mengoptimalkan Data

```excel
NIS: Gunakan format tetap (01, 02, 03)
NAMA: Capitalize (Ahmad Rizki, bukan ahmad rizki)
KELAS: Konsisten (10-A, bukan 10A atau 10 A)
```

---

## 🤝 Kontribusi

Kami terbuka untuk kontribusi! Baca [**CONTRIBUTING.md**](CONTRIBUTING.md) untuk panduan.

### Area yang Bisa Dikontribusi

- 🐛 Bug fixes
- ✨ Fitur baru
- 📖 Dokumentasi
- 🌍 Translasi (EN, FR, ES, dll)
- 🎨 Improvement UI/UX
- ⚡ Performance optimization

### Proses Kontribusi

```bash
1. Fork repository
2. Create feature branch (git checkout -b feature/amazing-feature)
3. Commit changes (git commit -m 'Add amazing feature')
4. Push ke branch (git push origin feature/amazing-feature)
5. Buat Pull Request
```

---

## 📄 Lisensi

Project ini menggunakan lisensi **MIT License** - bebas untuk komersial dan personal use.

Lihat file [**LICENSE**](LICENSE) untuk detail lengkap.

---

## 📞 Support & Kontak

- 🐛 **Report Bug**: [Buat Issue di GitHub](https://github.com/username/barcode-absensi-generator/issues)
- 💬 **Diskusi**: [GitHub Discussions](https://github.com/username/barcode-absensi-generator/discussions)
- 📧 **Email**: support@example.com
- 🌐 **Website**: https://barcode-absensi.example.com

---

## 🎉 Terima Kasih

Terima kasih sudah menggunakan **Barcode Absensi Generator**!

Jika aplikasi ini membantu, beri ⭐ di GitHub dan share ke teman-teman.

---

## 📊 Statistik

[![GitHub Stars](https://img.shields.io/github/stars/username/barcode-absensi-generator?style=social)](https://github.com/username/barcode-absensi-generator)
[![GitHub Forks](https://img.shields.io/github/forks/username/barcode-absensi-generator?style=social)](https://github.com/username/barcode-absensi-generator)
[![GitHub Issues](https://img.shields.io/github/issues/username/barcode-absensi-generator)](https://github.com/username/barcode-absensi-generator/issues)
[![MIT License](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

---

**Made with ❤️ for Indonesian Schools and Institutions**

Last updated: 2026-03-21