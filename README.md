# 🪑 Rajdeep Furnitures – Receipt Manager

A **Progressive Web App (PWA)** for managing customer payment receipts at Rajdeep Furnitures, Alwar, Rajasthan.

---

## ✨ Features

- **New Receipt Form** — Name, Address, Mobile, Amount
- **Payment Phase** — Initial (Advance), Work Start, Final
- **Payment Mode** — Cash, Cheque, UPI, Bank Transfer (with notes field for non-cash)
- **Auto Date & Time** — filled automatically, editable
- **PDF Generation** — branded A5 receipt auto-downloads on save
- **WhatsApp Share** — pre-formatted message opens directly to customer's number
- **All Receipts View** — list of saved receipts with re-download & re-share
- **Offline Support** — works without internet after first load (PWA)
- **Local Storage** — receipts persist across sessions

---

## 🚀 Deploy to GitHub Pages

1. **Fork / clone** this repo
2. Go to **Settings → Pages**
3. Set source to `main` branch, root `/`
4. Your app will be live at `https://yourusername.github.io/rajdeep-receipts/`

---

## 📁 File Structure

```
rajdeep-receipts/
├── index.html          # Main app HTML
├── manifest.json       # PWA manifest
├── sw.js               # Service worker (offline support)
├── css/
│   └── style.css       # All styles
├── js/
│   └── app.js          # All logic (form, PDF, WhatsApp, storage)
└── assets/
    └── logo.jpg        # Rajdeep Furnitures logo
```

---

## 🛠 Customisation

| What to change | Where |
|---|---|
| Phone number in PDF | `js/app.js` → search `+91-XXXXXXXXXX` |
| Phone number in PDF header | `js/app.js` → `Mob:` line in `generatePDF()` |
| Company address | `js/app.js` → `Modular Furniture · Alwar` |
| Logo | Replace `assets/logo.jpg` and update `LOGO_DATA_URI` in `js/app.js` |
| Accent colours | `css/style.css` → `:root` CSS variables |

---

## 📱 Install as App (Android / iOS)

1. Open the URL in Chrome (Android) or Safari (iOS)
2. Tap **"Add to Home Screen"**
3. App installs like a native app, works offline

---

## 🔒 Data & Privacy

All data is stored **locally on the device** using `localStorage`. No data is sent to any server.

---

*Built for Rajdeep Furnitures, Alwar, Rajasthan*
