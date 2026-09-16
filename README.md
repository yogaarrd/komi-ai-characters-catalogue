# Komi AI Characters Catalogue

A community-driven character catalogue for Komi AI. Browse, share, and import AI characters created by the community.

## 🌟 Features

- **Browse Characters** - Discover AI characters created by the community
- **One-Click Import** - Add characters to your Komi AI app instantly
- **Share Your Creations** - Submit your own characters via Pull Request
- **Version Tracking** - Characters are versioned for updates

## 📖 How to Use

### For Users
1. Open Komi AI app
2. Click the "Catalog" button in the sidebar
3. Browse and search for characters
4. Click "Import" to add a character

### For Contributors
1. Fork this repository
2. Add your character in `characters/[your-character]/`
3. Create a Pull Request
4. Wait for review and merge

See [CONTRIBUTING.md](CONTRIBUTING.md) for detailed instructions.

## 📁 Repository Structure

```
komi-ai-characters-catalogue/
├── characters/
│   ├── [character-id]/
│   │   ├── character.json
│   │   └── avatar.png
│   └── _template/
├── index.json
├── CONTRIBUTING.md
└── .github/
    └── workflows/
        └── validate.yml
```

## 📋 Character Schema

```json
{
  "id": "character-id",
  "name": "Character Name",
  "description": "Short description",
  "avatar": "avatar.png",
  "gender": "female",
  "personality": "Santai",
  "customInstructions": "Custom AI instructions",
  "language": "auto",
  "responseLength": "balanced",
  "tags": ["tag1", "tag2"],
  "author": {
    "name": "Your Name",
    "github": "your-username"
  },
  "version": "1.0.0"
}
```

## 🤝 Contributing

We welcome contributions! Please read our [Contributing Guide](CONTRIBUTING.md) before submitting a Pull Request.

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- All contributors who have submitted characters
- The Komi AI community
