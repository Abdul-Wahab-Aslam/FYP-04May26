# SecureV2V-XAI — Bahria University FYP
**Secure V2V Communication using AI** — Abdul Wahab Aslam  
Explainable AI Framework for Vehicular Network Security

---

## 📁 Folder Contents

```
SecureV2V-Vercel/
├── index.html          ← Complete app (HTML + CSS + JS, all-in-one)
├── demo_accident.mp4   ← Demo dashcam video (loops in left pane)
├── favicon.ico         ← Browser tab icon
├── vercel.json         ← Vercel static deployment config
├── .gitignore
└── README.md
```

---

## 🚀 Deploy to Vercel via GitHub (Recommended)

### Step 1 — Push to GitHub
1. Create a new repository on [github.com](https://github.com/new)  
   - Name it e.g. `SecureV2V-XAI`
   - Set to **Public** (required for free Vercel)
   - Do **NOT** initialize with README (you already have one)

2. Open terminal in this folder and run:
```bash
git init
git add .
git commit -m "Initial commit — SecureV2V XAI dashboard"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/SecureV2V-XAI.git
git push -u origin main
```

### Step 2 — Deploy on Vercel
1. Go to [vercel.com](https://vercel.com) and sign in (use GitHub login)
2. Click **"Add New Project"**
3. Click **"Import"** next to your `SecureV2V-XAI` repo
4. On the Configure Project screen:
   - **Framework Preset** → select `Other`
   - **Root Directory** → leave as `/` (default)
   - **Build & Output Settings** → leave all blank (static site, no build needed)
5. Click **"Deploy"**
6. ✅ Done! Your app will be live at `https://secure-v2v-xai.vercel.app` (or similar)

---

## 🌐 Features

| Feature | Description |
|---------|-------------|
| Live V2V Radar | Animated SVG network topology with rotating sweep |
| CARLA Simulation | Real-time canvas vehicle animation with attack links |
| YOLOv8 Dashcam | Upload frame / capture snapshot → HF Space AI inference |
| SHAP Explainability | Live feature contribution chart per threat flag |
| Intel Feed | WebSocket telemetry stream + mock fallback |
| Dataset KPI Bar | Accuracy / Precision / Recall / F1 per dataset |
| Dark / Light Theme | Full CSS variable driven theming |

---

## 🔧 Local Testing

Just open `index.html` in any browser — no server, no npm, no build required.

```bash
# Optional: serve locally with Python
python3 -m http.server 3000
# Then open http://localhost:3000
```

---

## ⚙️ Environment / API Endpoints

The app connects to these external services (gracefully falls back if unavailable):

| Service | URL | Purpose |
|---------|-----|---------|
| Render Backend | `https://secure-v2v-api.onrender.com` | V2V metrics WebSocket |
| HF Space | `https://real-wahab-v2v-crash-detector.hf.space` | YOLOv8 crash detection |

No API keys needed — all endpoints are public.

---

*Bahria University FYP 2026 — Abdul Wahab Aslam — AutoSec AI*
