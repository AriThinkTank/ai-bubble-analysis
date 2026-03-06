# AI Bubble Burst — Scenario Analysis

A data-driven, interactive scenario analysis of a potential AI investment correction — mapping global cascade effects, stakeholder exposures, and India's position across four possible futures.

## 🔗 Live Demo
Once deployed: `https://[your-username].github.io/ai-bubble-analysis/`

---

## 📊 What's Inside

This single-page analysis covers:

1. **Bubble Anatomy** — Investment intensity vs GDP, P/E comparisons (dotcom vs AI), cashflow coverage ratios, and the investment-revenue gap ($560B invested → $35B revenue = 6¢ per dollar)
2. **Historical Parallels** — Hype cycle positioning, boom-bust comparison (Web3 vs AI), capital efficiency matrix
3. **Four Scenarios** — Probability-weighted: Soft Landing (35%), Hard Crash (25%), Continued Acceleration (15%), Bifurcation (25%)
4. **Stakeholder Risk Matrix** — Foundation labs, hyperscalers, hardware vendors, enterprises, startups, sovereign actors
5. **Global Cascade Map** — Dependency flow from trigger event through to India-specific impacts
6. **India Impact Analysis** — Four scenario pathways for India's IT sector, startup ecosystem, sovereign programs, and application layer
7. **Leverage Points** — Complexity analysis using Meadows' framework
8. **Assumptions & Sources** — All data sources and analytical assumptions made explicit

---

## 📐 Mathematical Framework

Key equations used in the analysis:

```
NPV Sustainability: NPV = Σ(CFt / (1+r)^t) - Capex ≥ 0
  → Requires ~$98B/yr avg cash flows on $560B capex (r=12%, 10yr)

Circular Loop Stability: R(1 - αβγ) = 0
  → System stable only if αβγ < 1; currently estimated 0.7–0.85

OpenAI Required CAGR: (200/13)^(1/5) - 1 = 72%/yr
  → Must grow at 2× market rate to reach break-even by 2030

Infrastructure Utilisation: U(t) = min[1, A(t-τ) / I(t)]
  → Application lag τ = 5–7 years; current U ≈ 0.2–0.4

Expected Value: EV = 0.30×$5T + 0.50×$500B - $300B = +$1.45T
  → Explains rational persistence of investment despite high failure probability
```

---

## 📁 File Structure

```
ai-bubble-analysis/
├── index.html          # Complete self-contained visualization (no dependencies except CDN)
└── README.md           # This file
```

The entire application is **one self-contained HTML file**. No build tools, no npm, no server required.

---

## 🚀 Deploy to GitHub Pages

### Step 1: Create a new GitHub repository

1. Go to [github.com](https://github.com) and log in
2. Click the **"+"** button → **"New repository"**
3. Name it: `ai-bubble-analysis` (or any name you prefer)
4. Set to **Public** (required for free GitHub Pages)
5. Do **NOT** initialize with README (you'll push your own)
6. Click **"Create repository"**

### Step 2: Upload files

**Option A — GitHub Web UI (easiest):**
1. On your new repository page, click **"uploading an existing file"**
2. Drag and drop both `index.html` and `README.md`
3. Scroll down, add commit message: `"Initial commit: AI bubble analysis"`
4. Click **"Commit changes"**

**Option B — Git command line:**
```bash
# Navigate to the folder containing index.html and README.md
cd /path/to/ai-bubble-analysis

# Initialize git
git init
git add .
git commit -m "Initial commit: AI bubble analysis"

# Connect to your GitHub repo (replace YOUR-USERNAME)
git remote add origin https://github.com/YOUR-USERNAME/ai-bubble-analysis.git
git branch -M main
git push -u origin main
```

### Step 3: Enable GitHub Pages

1. In your repository, click **"Settings"** (top menu)
2. Scroll down to **"Pages"** in the left sidebar
3. Under **"Source"**, select **"Deploy from a branch"**
4. Select branch: **"main"**, folder: **"/ (root)"**
5. Click **"Save"**

### Step 4: Access your site

After 1–3 minutes, your analysis will be live at:
```
https://YOUR-USERNAME.github.io/ai-bubble-analysis/
```

You'll see a green checkmark in Settings → Pages when it's ready.

---

## 🔄 Updating the Analysis

To update content, simply edit `index.html` and push again:

```bash
git add index.html
git commit -m "Update: revised scenario probabilities"
git push
```

GitHub Pages auto-redeploys within ~1 minute.

---

## 📚 Data Sources

All data sourced from documents and public research:

| # | Source | Used For |
|---|--------|----------|
| 1 | Provided research documents (AI Bubble papers) | Core framework, scenarios, math models |
| 2 | Bain Global AI Report 2025 | $2T revenue target; 5% transformative returns |
| 3 | Goldman Sachs AI Infrastructure 2025 | 15% circular revenue; capex projections |
| 4 | Company filings (MSFT, Google, Meta, Amazon, Nvidia) | Capex, OCF, AI revenue |
| 5 | PitchBook / CB Insights | VC funding flows; Web3 collapse data |
| 6 | NASSCOM FY2025 | India IT sector data |
| 7 | McKinsey Global Institute | Productivity gains; enterprise adoption |
| 8 | Gartner Hype Cycle 2024/25 | AI positioning |
| 9 | BEA / US GDP | Capex as % of GDP |
| 10 | IndiaAI Mission / MeitY | India sovereign programs |
| 11 | NASDAQ historical data | Dotcom comparison |

---

## ⚠️ Disclaimer

This analysis is for informational and research purposes only. Scenario probabilities are analytical estimates, not actuarial forecasts. This is not investment advice. All figures are based on publicly available data and research documents as of early 2026.

---

*Built as a static single-file HTML application using Chart.js from CDN. No data leaves your browser.*
