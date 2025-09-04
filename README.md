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
├── README.md              # This file
├── pdfs/                  # PDF storage
│   ├── sample1.pdf        # Sample PDF
│   ├── sample2.pdf       # Sample PDF
│   ├── manual.pdf         # Manual PDF
│   └── guide.pdf          # Guide PDF
└── .github/               # GitHub configuration
    └── workflows/
        └── deploy.yml     # Auto-deploy workflow
```

## 🔧 Customization

### **Adding Your Own PDFs:**
1. Upload PDFs through the developer panel
2. Add card mappings for your PDFs
3. All settings are automatically saved

### **Changing Colors:**
Edit the CSS variables in `index.html`:
```css
:root {
    --primary-color: #f32411;
    --background-color: #f32411;
}
```

## 🚀 Deployment

This repository is configured for automatic deployment to GitHub Pages.

### **Manual Deployment:**
1. Push to main branch
2. GitHub Actions will automatically deploy
3. Visit your GitHub Pages URL

## 📱 Browser Support

- ✅ Chrome (recommended)
- ✅ Firefox
- ✅ Safari
- ✅ Edge

## 🎉 License

This project is open source and available under the MIT License.

---

**Built for Aeros Racing F1 Team** 🏁
