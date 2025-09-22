# 🏁 Aeros Racing F1 Kiosk - GitHub Pages Version

A professional racing kiosk application that can be deployed on GitHub Pages.

## 🚀 Live Demo

Visit the live demo: [Aeros Racing F1 Kiosk](https://yourusername.github.io/aeros-kiosk-github-pages/)

## 🎮 Features

- **Full-screen kiosk mode** - Professional racing environment
- **RFID card scanning** - Type card ID + Enter to simulate scanning
- **PDF viewing** - Real PDF files with clean display
- **Developer panel** - Press Ctrl+Shift+D to access settings
- **File uploads** - Upload PDFs through the interface
- **Persistent settings** - All settings saved in browser
- **Responsive design** - Works on all devices
- **Offline capable** - Works without internet connection

## 🎯 How to Use

### **RFID Card Scanning:**
1. Type a card ID (e.g., `DEV001`)
2. Press Enter
3. View the associated PDF

### **Developer Panel:**
1. Press `Ctrl+Shift+D` to open developer panel
2. Add card mappings
3. Upload PDF files
4. Switch to production mode

### **Sample Cards:**
- `DEV001` → Developer Manual
- `TEST001` → Test Document
- `USER001` → User Guide

## 📁 File Structure

```
aeros-kiosk-github-pages/
├── index.html              # Main application
├── README.md               # This file
├── pdfs/                   # PDF storage
│   ├── sample1.pdf         # Sample PDF
│   ├── sample2.pdf         # Sample PDF
│   ├── manual.pdf          # Manual PDF
│   └── guide.pdf           # Guide PDF
└── .github/                # (optional) Actions workflows
```

## 🔧 Adding PDFs

There are two ways to use PDFs:

- **Bundled PDFs (no setup):** Place files under `pdfs/` in the repo and push. They will be served by GitHub Pages and selectable in the app.
- **Upload from the app (optional GitHub token):** Configure repo settings in the Developer panel to enable committing uploads directly to the repo.

### Configure GitHub uploads (optional)
1. Open Developer panel → GitHub Repository section
2. Enter:
   - Owner: your GitHub username or org
   - Repo: `aeros-kiosk-github-pages` (or your fork's name)
   - Branch: `main` or `gh-pages` (whichever serves your site)
   - Token: a Personal Access Token with `contents:write` scope
3. Click “Save GitHub Settings”
4. Use “Upload PDF” to add files; they will commit to `pdfs/` on the chosen branch

Notes:
- If token is not set, uploads are session-only (stored as blob URLs in the browser).
- With repo configured, the app lists PDFs dynamically from `pdfs/` using the GitHub API.

## 🚀 Deployment

- Push to the default branch configured for Pages (commonly `main` with Pages set to `/ (root)`), or use `gh-pages` branch if your repo is set that way.
- Ensure the site URL is `https://<owner>.github.io/<repo>/`.
- The app builds absolute URLs correctly for PDFs on GitHub Pages.

## 📱 Browser Support

- ✅ Chrome (recommended)
- ✅ Firefox
- ✅ Safari
- ✅ Edge

## 🎉 License

This project is open source and available under the MIT License.

---

**Built for Aeros Racing F1 Team** 🏁
