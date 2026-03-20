# 📋 Changelog

Semua perubahan penting pada project ini didokumentasikan di file ini.

Format mengikuti [Keep a Changelog](https://keepachangelog.com/) dan [Semantic Versioning](https://semver.org/).

---

## [1.0.0] - 2026-03-21

### 🎉 Release Pertama!

Version 1.0.0 adalah release resmi pertama dengan fitur lengkap dan dokumentasi profesional.

### ✨ Added

- ✅ **Import Excel** - Support .xlsx dan .csv format
- ✅ **Auto Barcode Generation** - Generate CODE128 barcode otomatis
- ✅ **Preview Real-time** - Lihat kartu sebelum cetak
- ✅ **Print Support** - Cetak langsung dari browser
- ✅ **Download ZIP** - Unduh semua kartu dalam satu file ZIP
  - Includes: Individual HTML files per siswa
  - Includes: INDEX.html untuk navigasi
  - Includes: CSV backup data
- ✅ **Export CSV** - Download data dengan barcode code
- ✅ **Responsive UI** - Support desktop, tablet, mobile
- ✅ **Multi-sheet Support** - Auto-detect dan pilih sheet dari Excel
- ✅ **Drag & Drop** - Upload file dengan drag & drop
- ✅ **Form Validation** - Validasi data otomatis
- ✅ **Toast Notifications** - Feedback untuk user actions
- ✅ **Professional UI** - Modern design dengan gradient dan shadows

### 🔧 Technical

- Menggunakan JsBarcode untuk generate barcode
- SheetJS (xlsx.js) untuk parse Excel
- JSZip untuk buat ZIP file
- FileSaver untuk download
- Pure HTML/CSS/JavaScript (no build step)
- CDN libraries untuk zero installation

### 📚 Documentation

- README.md - Dokumentasi lengkap
- CONTRIBUTING.md - Panduan kontribusi
- CHANGELOG.md - File ini
- Template Excel siap pakai

### 🌍 Supported Languages

- 🇮🇩 Indonesian (native)

---

## [0.9.0] - 2026-03-20

### Beta Testing

Development version untuk internal testing.

### ✨ Added (Beta)

- Excel import functionality
- Barcode generation
- Basic UI
- Print support

### 🐛 Fixed (Beta)

- Multiple bug fixes dari testing
- UI improvements

---

## Rencana Fitur Mendatang

### v1.1.0 (Mei 2026)

- [ ] Dark mode support
- [ ] Multiple barcode formats (QR, DataMatrix, dll)
- [ ] Batch operations (bulk generate, delete)
- [ ] Database integration (save to cloud)
- [ ] API endpoint untuk automation

### v1.2.0 (Juni 2026)

- [ ] Translation support (EN, ES, FR)
- [ ] Custom card design template
- [ ] Email integration (send cards)
- [ ] Real-time collaboration
- [ ] Mobile app (React Native)

### v2.0.0 (Q3 2026)

- [ ] Full database backend
- [ ] User authentication
- [ ] Advanced analytics & reporting
- [ ] Barcode scanner integration
- [ ] Real-time absensi tracking

---

## Versioning Policy

Kami mengikuti [Semantic Versioning](https://semver.org/):

```
MAJOR.MINOR.PATCH[-PRERELEASE]

- MAJOR: Breaking changes / major rewrite
- MINOR: New features (backward compatible)
- PATCH: Bug fixes (backward compatible)
- PRERELEASE: alpha, beta, rc
```

**Contoh:**
- `1.0.0` - Release stabil
- `1.1.0` - Release dengan fitur baru
- `1.1.1` - Release dengan bug fix
- `2.0.0-alpha.1` - Pre-release major version

---

## Support Timeline

| Version | Release | Support Until | Status |
|---------|---------|---------------|--------|
| 1.0.x   | 2026-03-21 | 2027-03-21 | ✅ Active |
| 0.9.x   | 2026-03-20 | 2026-03-21 | ❌ Deprecated |

---

## Upgrade Guide

### Dari 0.9.x ke 1.0.0

**Breaking Changes:** Tidak ada. Fully backward compatible.

**Upgrade Steps:**
1. Download file HTML baru
2. Gunakan template Excel baru (atau pakai file lama)
3. Tidak perlu clear data/settings

---

## Migration Notes

### Data Compatibility

- ✅ File Excel dari v0.9 compatible dengan v1.0
- ✅ Downloaded ZIP dari v0.9 bisa dibuka di v1.0
- ✅ CSV export format sama

---

## Credits & Contributors

### Version 1.0.0

**Core Development:**
- [@maindev](https://github.com/maindev) - Project Lead
- [@contributor1](https://github.com/contributor1) - Features
- [@contributor2](https://github.com/contributor2) - Bug Fixes

**Documentation:**
- [@docwriter](https://github.com/docwriter) - README & Docs

**Testing:**
- Beta testers dari berbagai sekolah di Indonesia

**Special Thanks:**
- Terimakasih kepada semua yang memberikan feedback dan suggestion!

---

## Deprecation Policy

Fitur/API yang deprecated akan:

1. **Di-announce** di changelog sebelum 1 versi
2. **Di-dokumentasikan** bagaimana migrasi/alternatif
3. **Tetap berfungsi** untuk 2-3 versi
4. **Dihapus** sepenuhnya pada major version berikutnya

**Contoh:**
- v1.2: Announce deprecation
- v1.3: Fitur masih berfungsi, warning di console
- v2.0: Fitur dihapus total

---

## Release Notes Format

Setiap release mengikuti format:

```markdown
## [Version] - YYYY-MM-DD

### Added
- New features

### Changed
- Improvements & changes

### Deprecated
- Features yang akan dihapus

### Removed
- Features yang sudah dihapus

### Fixed
- Bug fixes

### Security
- Security fixes

### Contributors
- @username1, @username2
```

---

## How to Report Issues

Jika menemukan issue:

1. Check existing issues (kemungkinan sudah ada)
2. Create new issue dengan template yang tersedia
3. Include: deskripsi, steps, screenshot
4. Label issue yang sesuai (bug, feature, docs, dll)

---

## How to Suggest Features

Untuk suggest fitur baru:

1. Open GitHub Discussion atau Issue
2. Jelaskan use case dengan detail
3. Sertakan contoh implementasi (jika ada ide)
4. Diskusikan dengan maintainers sebelum coding

---

## Community & Support

- **GitHub Issues**: Bug reports & feature requests
- **GitHub Discussions**: Q&A dan general discussion
- **Email**: support@example.com
- **Website**: https://barcode-absensi.example.com

---

## License

Semua changes dan contributions di-cover oleh [MIT License](LICENSE).

---

## Keeping Track

### Subscribe to Updates

- ⭐ Star repository untuk notifikasi release
- 👁️ Watch repository untuk semua activities
- 📧 Subscribe ke release notifications

### Stay Informed

- Blog: https://blog.example.com
- Twitter: [@handle](https://twitter.com/handle)
- Newsletter: https://example.com/newsletter

---

Last updated: 2026-03-21

**Made with ❤️ for Indonesian Schools**