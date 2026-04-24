# 🏥 PraanSetu — AI Patient Triage & ER Queue System

**Developed by Amnex Infotechnologies Pvt. Ltd.**  
A GIGW 3.0 / WCAG 2.1 AA compliant, browser-based AI triage and emergency room queue management system for Indian public health facilities.

---

## 🚀 Live Demo (GitHub Pages)

> Once deployed, your app will be live at:  
> `https://<your-username>.github.io/praansetu/`

---

## 🔐 Application Flow

```
Login Page (MFA)  →  Branded Splash  →  Triage Dashboard
```

| Step | Description |
|---|---|
| 1. Credentials | Login ID + Password + CAPTCHA |
| 2. 2FA Method | OTP / Facial Recognition / Fingerprint / OTP+Bio |
| 3. Verify | Complete selected 2FA factor |
| 4. Access Granted | Smooth transition into main application |

---

## 📋 Features

| Module | Description |
|---|---|
| 🔐 **Secure Login** | Multi-factor auth: Password + CAPTCHA + OTP/Face/Biometric |
| 🩺 **AI Triage** | Symptom-based ESI (1–5) scoring with confidence rating |
| 📋 **ER Queue** | Real-time patient queue with wait time estimation |
| ✅ **Confirm & Assign** | Doctor assignment and handoff note generation |
| 📊 **Admin Dashboard** | ESI distribution, flagged patients, audit log, CSV export |
| ♿ **Accessibility** | Font size toggle, High Contrast mode, Hindi/English toggle |
| 📱 **Responsive** | Mobile-first, works on tablets and desktops |

---

## 🗂️ Project Structure

```
praansetu/
├── index.html              # Complete app — Login + Triage (single file)
├── README.md               # This file
├── .gitignore              # Standard ignore rules
├── .github/
│   └── workflows/
│       └── deploy.yml      # GitHub Pages auto-deploy on push to main
└── docs/
    └── GIGW_Compliance.md  # Accessibility & GIGW 3.0 compliance notes
```

---

## ⚡ Deployment: GitHub Pages

### Option 1 — Automatic via GitHub Actions (Recommended)

```bash
# 1. Clone / init repo
git init
git add .
git commit -m "Initial deploy: PraanSetu v5 — Login + Triage App"
git branch -M main
git remote add origin https://github.com/<your-username>/praansetu.git
git push -u origin main
```

Then go to: **GitHub → Settings → Pages → Source → GitHub Actions → Save**

Your app is live at `https://<your-username>.github.io/praansetu/`

### Option 2 — Manual Static Deploy

1. Go to **Settings → Pages**
2. Source: `Deploy from a branch` → `main` → `/ (root)`
3. Click **Save** — live in ~60 seconds

---

## 🛠️ Local Development

No build tools or dependencies required.

```bash
# Clone
git clone https://github.com/<your-username>/praansetu.git
cd praansetu

# Open directly
open index.html          # Mac
xdg-open index.html      # Linux
start index.html         # Windows

# Or run a local server
python -m http.server 8080
# then visit http://localhost:8080
```

---

## 🔒 Demo Credentials

| Field | Value |
|---|---|
| Login ID | Any value (e.g. `admin` or `N00041`) |
| Password | Any value |
| CAPTCHA | Enter the code shown |
| OTP | Any 6 digits |

> All auth is simulated for demo purposes. No backend or database required.

---

## 🔒 Data & Privacy

- **All data is in-memory only** — no backend, no database, no external API calls
- Patient data is **not persisted** between sessions
- Suitable for demo, training, and prototype use
- For production: integrate secure backend, ABDM-compliant data storage

---

## ♿ GIGW 3.0 / WCAG 2.1 AA Compliance

- Semantic HTML5 landmarks and ARIA roles
- Keyboard navigation on all interactive elements
- High Contrast mode toggle
- Font size adjustment (Small / Default / Large)
- Screen reader compatible structure
- Mobile-first responsive design

---

## 🏷️ ESI Scale Reference

| Level | Label | Target Response |
|---|---|---|
| **ESI 1** | Immediate | Now |
| **ESI 2** | Emergent | ≤ 15 min |
| **ESI 3** | Urgent | ≤ 30 min |
| **ESI 4** | Less Urgent | ≤ 60 min |
| **ESI 5** | Non-Urgent | ≤ 120 min |

---

## 📄 License

© 2025 Amnex Infotechnologies Pvt. Ltd. All rights reserved.  
This software is proprietary. Unauthorized reproduction or distribution is prohibited.

---

## 📞 Contact

**Amnex Infotechnologies Pvt. Ltd.**  
Ahmedabad, Gujarat, India  
🌐 [www.amnex.com](https://www.amnex.com)
