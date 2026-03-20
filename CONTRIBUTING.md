# 🤝 Panduan Kontribusi

Terima kasih tertarik berkontribusi pada **Barcode Absensi Generator**! 

Dokumen ini menjelaskan bagaimana caranya berkontribusi pada project ini.

---

## 📝 Code of Conduct

Kami berkomitmen pada lingkungan yang inklusif dan welcoming. Semua contributors diharapkan:

- ✅ Bersikap sopan dan profesional
- ✅ Hormati ide dan perspektif orang lain
- ✅ Fokus pada konstruktif feedback
- ✅ Laporkan perilaku tidak pantas kepada maintainers

**Pelanggaran Code of Conduct dapat menyebabkan penghapusan dari project.**

---

## 🐛 Melaporkan Bug

### Sebelum Membuat Issue

- ✓ Check existing issues dulu (mungkin sudah ada)
- ✓ Clear browser cache dan coba lagi
- ✓ Test di browser lain
- ✓ Pastikan deskripsi detail dan jelas

### Membuat Bug Report

Gunakan template berikut:

```markdown
## 🐛 Bug Report

### Deskripsi
[Jelaskan bug dengan singkat dan jelas]

### Langkah Reproduksi
1. [Langkah pertama]
2. [Langkah kedua]
3. [Langkah ketiga]

### Expected Behavior
[Apa yang seharusnya terjadi]

### Actual Behavior
[Apa yang terjadi sebenarnya]

### Screenshots/Logs
[Jika ada, sertakan screenshot atau console log]

### Environment
- Browser: [Chrome 120, Firefox 121, dll]
- OS: [Windows 11, macOS 13, Ubuntu 22.04, dll]
- File Size: [Berapa siswa/baris data]

### Additional Context
[Info tambahan yang relevan]
```

---

## 💡 Mengusulkan Fitur Baru

### Sebelum Membuat Feature Request

- ✓ Check existing issues/discussions
- ✓ Pastikan fitur tidak sudah ada
- ✓ Pikirkan use case yang jelas

### Membuat Feature Request

```markdown
## ✨ Feature Request

### Deskripsi
[Jelaskan fitur yang diinginkan]

### Motivasi
[Mengapa fitur ini penting?]

### Implementasi yang Diharapkan
[Bagaimana menurut Anda fitur ini bekerja?]

### Contoh Penggunaan
[Berikan contoh use case]

### Alternatif yang Dipertimbangkan
[Apakah ada cara lain untuk solve ini?]
```

---

## 🚀 Membuat Pull Request

### Development Setup

```bash
# 1. Fork repository di GitHub
# 2. Clone fork Anda
git clone https://github.com/YOUR_USERNAME/barcode-absensi-generator.git
cd barcode-absensi-generator

# 3. Buat branch baru
git checkout -b feature/deskripsi-singkat

# 4. Buat perubahan Anda

# 5. Commit dengan pesan yang jelas
git commit -m "Add: deskripsi fitur baru"

# 6. Push ke fork
git push origin feature/deskripsi-singkat

# 7. Buat Pull Request di GitHub
```

### Commit Message Guidelines

Gunakan format yang jelas:

```
[TYPE]: Deskripsi singkat

Deskripsi lengkap (optional)
- Apa yang diubah
- Mengapa diubah
- Bagaimana cara kerja

Fixes #123 (jika fix bug)
Closes #456 (jika close issue)
```

**Type Prefixes:**
- `feat:` - Fitur baru
- `fix:` - Bug fix
- `docs:` - Dokumentasi
- `style:` - Formatting, missing semicolons, dll
- `refactor:` - Code refactoring
- `perf:` - Performance improvement
- `test:` - Testing
- `chore:` - Build, dependencies, dll

**Contoh:**
```
feat: Add dark mode support

Implement dark/light theme toggle that:
- Persists user preference di localStorage
- Supports OS-level dark mode detection
- Applies ke semua components

Closes #234
```

### Pull Request Checklist

Sebelum submit PR, pastikan:

- [ ] Branch dibuat dari `main` terbaru
- [ ] Commit messages jelas dan deskriptif
- [ ] Kode sudah ditest
- [ ] Tidak ada console errors/warnings
- [ ] Dokumentasi diupdate (jika perlu)
- [ ] No breaking changes (atau jelaskan)
- [ ] README diupdate (jika perlu)

### PR Template

```markdown
## 📝 Deskripsi

[Jelaskan PR Anda]

## 🎯 Tipe Perubahan

- [ ] Bug fix (fix issue tanpa breaking change)
- [ ] Fitur baru (add feature tanpa breaking change)
- [ ] Breaking change (fix atau feature yang breaking)
- [ ] Documentation update

## 🧪 Testing

- [ ] Sudah ditest di browser saya
- [ ] Sudah coba di multiple browsers:
  - [ ] Chrome
  - [ ] Firefox
  - [ ] Safari
  - [ ] Edge

## 📸 Screenshots

[Sertakan screenshot sebelum/sesudah jika ada UI changes]

## ✅ Checklist

- [ ] Kode mengikuti style guide project
- [ ] Self-review sudah dilakukan
- [ ] Comments ditambahkan untuk kode yang sulit
- [ ] Dokumentasi sudah diupdate
- [ ] Tidak ada breaking changes

## 🔗 Related Issue

Closes #[issue number]
```

---

## 🎨 Code Style Guide

### HTML

```html
<!-- ✓ Indentation 4 spaces -->
<div class="container">
    <p>Paragraph</p>
</div>

<!-- ✓ Semantic HTML -->
<button onclick="handleClick()">Click Me</button>

<!-- ✓ Meaningful class names -->
<div class="card-container">
    <div class="card-header">
        <h2>Title</h2>
    </div>
</div>
```

### CSS

```css
/* ✓ Use CSS variables untuk colors */
:root {
    --primary: #1a1a2e;
    --secondary: #16c784;
    --text: #333;
}

/* ✓ Group related properties */
.button {
    display: inline-block;
    padding: 10px 20px;
    background: var(--primary);
    color: white;
    border: none;
    border-radius: 4px;
    font-size: 14px;
    cursor: pointer;
}

/* ✓ Mobile-first approach */
@media (max-width: 768px) {
    .button {
        padding: 8px 16px;
        font-size: 12px;
    }
}
```

### JavaScript

```javascript
// ✓ Meaningful variable names
const studentCount = 0;
const isGenerating = false;

// ✓ Arrow functions
const generateCards = () => {
    // code
};

// ✓ Template literals
const message = `Total kartu: ${uploadedData.length}`;

// ✓ Comments untuk logika kompleks
// Generate barcode value dari NIS dengan prefix sekolah
const barcodeValue = `${schoolName.substring(0,3).toUpperCase()}${String(student.nis).padStart(5, '0')}`;

// ✓ Error handling
try {
    JsBarcode(`#barcode-${index}`, barcodeValue, { format: "CODE128" });
} catch (e) {
    console.error('Barcode generation error:', e);
    showToast('Error generating barcode');
}
```

---

## 📚 Dokumentasi Contributions

Kontribusi dokumentasi sangat berharga!

### Dokumentasi yang Perlu Diupdate

- README.md - Dokumentasi utama
- CHANGELOG.md - Daftar perubahan setiap release
- docs/SETUP.md - Panduan setup
- docs/TROUBLESHOOTING.md - Solusi common issues
- docs/API.md - API documentation

### Tips Menulis Dokumentasi

- ✓ Gunakan Markdown format
- ✓ Sertakan contoh konkret
- ✓ Gunakan screenshots untuk clarity
- ✓ Update table of contents
- ✓ Cek spelling dan grammar

---

## 🌍 Translasi (i18n)

Ingin menerjemahkan ke bahasa lain? Berikut prosesnya:

1. **Fork repository**
2. **Buat branch baru**: `feat/i18n-[LANGUAGE_CODE]`
3. **Terjemahkan:**
   - README.md
   - Semua dokumentasi di `docs/`
   - Comments di kode (optional)
4. **Submit PR** dengan label `translation`

Supported/planned languages:
- 🇮🇩 Indonesian (native)
- 🇬🇧 English (needed)
- 🇪🇸 Spanish (needed)
- 🇫🇷 French (needed)

---

## 🔄 Review Process

### Untuk Maintainers

```
PR submitted → Review code → Request changes (if any) 
    → Re-review → Merge → Update CHANGELOG
```

### Apa yang Dicek

- ✅ Code quality
- ✅ Dokumentasi lengkap
- ✅ Testing adequate
- ✅ No breaking changes (tanpa alasan)
- ✅ Sesuai dengan code style
- ✅ Performant (tidak menambah load)

### Expected Timeline

- Small fix (docs, typo): 1-3 hari
- Bug fix: 3-7 hari
- Fitur baru: 1-2 minggu
- Major changes: diskusi terlebih dahulu

---

## 📦 Release Process

Releases dilakukan sesuai [Semantic Versioning](https://semver.org/):

- `MAJOR.MINOR.PATCH` (e.g., 1.2.3)
- MAJOR: breaking changes
- MINOR: new features
- PATCH: bug fixes

### Changelog Format

```markdown
## [1.2.0] - 2026-03-21

### Added
- Fitur baru XYZ (#123)

### Changed
- Improvement pada ABC

### Fixed
- Bug pada DEF (#456)

### Breaking Changes
- Removed XYZ (use ABC instead)

### Contributors
@username1 @username2
```

---

## ⚡ Tips untuk Kontributor

### Untuk Pemula

- Mulai dari issue berlabel `good-first-issue`
- Baca dokumentasi dengan teliti
- Tidak perlu khawatir membuat kesalahan
- Tanyakan jika ada yang tidak jelas

### Untuk Kontributor Berpengalaman

- Review PR dari kontributor lain
- Bantu triage issues
- Mentoring kontributor baru
- Propose fitur besar di discussions dulu

### Git Tips

```bash
# Update fork Anda dari upstream
git remote add upstream https://github.com/original/repo.git
git fetch upstream
git rebase upstream/main

# Force push dengan hati-hati
git push -f origin feature-branch

# Buat commit range lebih rapi
git rebase -i HEAD~3
```

---

## 🎯 Prioritas Project

Kami fokus pada:

1. **Stability** - Bug fixes prioritas tinggi
2. **Usability** - Improve UX/DX
3. **Performance** - Optimize speed
4. **Features** - Fitur baru yang useful
5. **Documentation** - Keep docs updated

---

## 📞 Bantuan & Pertanyaan

- **GitHub Discussions**: Untuk Q&A general
- **GitHub Issues**: Untuk bug/feature requests
- **Email**: maintainer@example.com

---

## 🙏 Terima Kasih!

Setiap kontribusi, besar atau kecil, berarti bagi project ini. 

**Terima kasih sudah berkontribusi! 🎉**

---

Last updated: 2026-03-21