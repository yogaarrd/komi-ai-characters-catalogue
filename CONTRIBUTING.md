# Contributing to Komi AI Characters Catalogue

Terima kasih telah berkontribusi! 🎉

## Cara Submit Karakter

### 1. Fork Repository
Klik tombol "Fork" di pojok kanan atas repository ini.

### 2. Clone Fork kamu
```bash
git clone https://github.com/[username]/komi-ai-characters-catalogue.git
cd komi-ai-characters-catalogue
```

### 3. Buat Branch Baru
```bash
git checkout -b karakter/[nama-karakter]
```

### 4. Buat Folder Karakter
```bash
mkdir characters/[nama-karakter]
```

Gunakan nama karakter dalam format **kebab-case** (huruf kecil, gunakan `-` sebagai pengganti spasi).
Contoh: `komi`, `naruto-uzumaki`, `shin-chan`

### 5. Buat `character.json`
Buat file `character.json` di dalam folder karakter dengan format berikut:

```json
{
  "id": "karakter-id",
  "name": "Nama Karakter",
  "description": "Deskripsi singkat tentang karakter",
  "avatar": "avatar.png",
  "gender": "female",
  "personality": "Santai",
  "customInstructions": "Instruksi kustom untuk karakter",
  "language": "auto",
  "responseLength": "sedang",
  "tags": ["tag1", "tag2"],
  "author": {
    "name": "Nama Kamu",
    "github": "username-github"
  },
  "version": "1.0.0",
  "createdAt": "2024-01-15"
}
```

### 6. Tambah Avatar
Simpan file gambar sebagai `avatar.png` di folder yang sama.

**Ketentuan Avatar:**
- Format: PNG atau JPG
- Ukuran: 200x200px atau lebih (square ratio)
- Maksimal: 500KB
- Nama file: `avatar.png`

### 7. Commit & Push
```bash
git add .
git commit -m "feat: tambah karakter [nama-karakter]"
git push origin karakter/[nama-karakter]
```

### 8. Buat Pull Request
Buka GitHub dan buat Pull Request dari branch kamu ke branch `main` di repository utama.

---

## Field Requirements

### Required Fields
| Field | Tipe | Deskripsi |
|-------|------|-----------|
| `id` | string | ID unik (kebab-case) |
| `name` | string | Nama karakter |
| `description` | string | Deskripsi singkat |
| `avatar` | string | Nama file avatar |
| `author.name` | string | Nama lengkap |
| `author.github` | string | Username GitHub |

### Optional Fields
| Field | Tipe | Default | Deskripsi |
|-------|------|---------|-----------|
| `gender` | string | `"not_specified"` | `"male"`, `"female"`, `"other"`, `"not_specified"` |
| `personality` | string | `"default"` | `"default"`, `"casual"`, `"professional"`, `"creative"`, `"teacher"`, `"coder"` |
| `customInstructions` | string | `""` | Instruksi kustom untuk AI |
| `language` | string | `"auto"` | `"id"`, `"en"`, `"auto"` |
| `responseLength` | string | `"balanced"` | `"short"`, `"balanced"`, `"detailed"` |
| `tags` | array | `[]` | Array tags untuk kategorisasi |
| `version` | string | `"1.0.0"` | Semantic versioning |
| `createdAt` | string | - | ISO 8601 date |

---

## Contoh Karakter

### Contoh Sederhana
```json
{
  "id": "komi",
  "name": "Komi",
  "description": "AI assistant friendly dan komunikatif",
  "avatar": "avatar.png",
  "gender": "female",
  "personality": "casual",
  "customInstructions": "Kamu adalah Komi, AI assistant yang ramah dan suka membantu.",
  "language": "auto",
  "responseLength": "balanced",
  "tags": ["assistant", "friendly", "indonesia"],
  "author": {
    "name": "Yoga Ardiana",
    "github": "yogaardiana"
  },
  "version": "1.0.0",
  "createdAt": "2024-01-15"
}
```

---

## Guidelines

### Do's ✅
- Gunakan nama yang deskriptif untuk karakter
- Berikan deskripsi yang jelas
- Gunakan avatar yang berkualitas
- Berikan custom instructions yang membantu AI memahami karakter
- Gunakan tags yang relevan

### Don'ts ❌
- Jangan submit karakter yang menyinggung SARA
- Jangan submit karakter yang mengandung konten dewasa
- Jangan gunakan ID yang sudah ada
- Jangan upload file yang terlalu besar (>500KB)
- Jangan ubah structure folder yang sudah ada

---

## Questions?

Jika ada pertanyaan, buka Issue di repository ini atau hubungi maintainers.
