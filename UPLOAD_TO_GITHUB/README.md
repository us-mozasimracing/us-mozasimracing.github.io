# MOZA Racing E-Commerce Storefront & Showcase

A pixel-faithful, responsive replica of the official [MOZA Racing US](https://us.mozaracing.com/) online storefront and high-performance sim-racing product pages.

---

## 🚀 Live Demo & GitHub Pages Deployment

This project is 100% static (HTML, Vanilla JS, Tailwind CSS via CDN, and official MOZA SVG/WebP assets). It requires **zero build steps** and runs instantly anywhere.

### Deploying to GitHub Pages (2 Minutes)

1. **Create a new GitHub repository** (e.g. `moza-racing-store`) at [github.com/new](https://github.com/new).
2. **Push this folder to GitHub**:
   ```bash
   git remote add origin https://github.com/<YOUR-USERNAME>/<YOUR-REPO-NAME>.git
   git branch -M main
   git push -u origin main
   ```
   *(Or simply drag and drop all files from this folder directly into GitHub's web interface).*
3. **Turn on GitHub Pages**:
   - Go to your repository on GitHub.
   - Click **Settings** &rarr; **Pages** (under "Code and automation" in the left sidebar).
   - Under **Build and deployment > Source**, select **Deploy from a branch**.
   - Under **Branch**, choose `main` and folder `/ (root)`, then click **Save**.
4. In about 30 seconds, your website will be live at:
   ```text
   https://<YOUR-USERNAME>.github.io/<YOUR-REPO-NAME>/
   ```

---

## 💻 Running Locally

### Option 1: One-Click Local Server (Recommended)
From this folder, run:
```bash
python3 -m http.server 8000
```
Then visit [http://localhost:8000](http://localhost:8000) in your browser.

### Option 2: Direct File Open
You can also directly double-click [`index.html`](index.html) in your Finder / File Explorer to open it in any browser without needing a server.

---

## 🏎️ Pages & Key Features

| Page | File | Key Highlights |
| :--- | :--- | :--- |
| **Storefront Landing Page** | [`index.html`](index.html) | Mega-menu navigation, hero slider, Mustang GTD showcase, category carousel, interactive live search, dynamic cart drawer |
| **CS Pro Wheel** | [`cs-pro-wheel.html`](cs-pro-wheel.html) | **$199.99 USD** (30% off strikethrough), 360° product gallery, bundle selector, quick release specs, sticky mobile buy bar |
| **R21 Ultra Wheel Base** | [`r21-ultra.html`](r21-ultra.html) | **$489.99 USD** (30% off strikethrough), 21Nm direct drive specs, official social headers, customer reviews with media |
| **R16 Ultra Wheel Base** | [`r16-ultra.html`](r16-ultra.html) | 16Nm direct drive ecosystem specs and bundle configurations |
| **R12 Wheel Base** | [`r12-wheelbase.html`](r12-wheelbase.html) | Mid-range direct drive base details and compatibility matrix |
| **CRP2 Pedals** | [`crp2-pedals.html`](crp2-pedals.html) | Load cell 200kg pedal set showcase with throttle/brake curves |
| **SRP2 Pedals** | [`srp2-pedals.html`](srp2-pedals.html) | Entry-level load cell pedal set showcase |
| **mBooster Active Pedals** | [`mbooster-active-pedal.html`](mbooster-active-pedal.html) | Active force-feedback telemetry-driven pedals |
| **Mustang GTD Sim Wheel** | [`ford-gtd-wheel.html`](ford-gtd-wheel.html) | Ford Performance licensed GTD wheel showcase |
| **404 Smart Redirect** | [`404.html`](404.html) | Custom dark 404 handler with smart path recovery for pretty product routes |

---

## 📂 Repository File Structure

```text
UPLOAD_TO_GITHUB/
├── .gitignore                   # Ignores OS & IDE temporary files
├── README.md                    # Project documentation & deployment guide
├── index.html                   # Main store landing page
├── cs-pro-wheel.html            # MOZA CS Pro Wheel ($199.99)
├── r21-ultra.html               # MOZA R21 Ultra Wheelbase ($489.99)
├── r16-ultra.html               # MOZA R16 Ultra
├── r12-wheelbase.html           # MOZA R12 Base
├── crp2-pedals.html             # MOZA CRP2 Pedals
├── srp2-pedals.html             # MOZA SRP Pedals
├── mbooster-active-pedal.html   # MOZA mBooster Active Pedals
├── ford-gtd-wheel.html          # Ford Mustang GTD Wheel
├── 404.html                     # Custom 404 page & path router
├── home/                        # Supports /home/ pretty URLs
│   └── index.html
└── products/                    # Supports /products/<item>/ pretty URLs
    ├── index.html
    ├── cs-pro-wheel/index.html
    └── r21-ultra/index.html
```

---

## 🛠️ Tech Stack

- **HTML5**: Semantic, accessible markup.
- **Tailwind CSS (CDN)**: Modern utility-first styling with responsive breakpoints for desktop, tablet, and mobile.
- **Vanilla JavaScript**: Zero build configuration, instant load times, interactive cart and tab components.
- **Assets**: Official vector SVGs and CDN-hosted imagery for maximum fidelity and lightning-fast speeds.
