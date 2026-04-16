# Tata Motors — Capital Structure EDA

An interactive web dashboard recreating the **Tata Motors Capital Structure EDA** Excel workbook as a fully self-contained HTML website. 

**Live demo →** Deploy via GitHub Pages (instructions below)

---

## 📊 What's Inside

| Section | Description |
|---|---|
| **Dashboard** | Executive KPIs + 4 key charts for FY2024 snapshot |
| **Raw Data** | Annual consolidated financials FY2015–FY2024 |
| **Ratios & Calculations** | 20+ derived metrics — leverage, coverage, profitability, growth |
| **Leverage Analysis** | Debt trajectory, risk flags, narrative timeline |
| **Peer Comparison** | Tata vs Maruti, M&M, Bajaj, Hero — 4 comparison charts |
| **Quarterly Data** | 12-quarter granular view (Q1FY22–Q4FY24) |
| **Data Dictionary** | Definitions, formulas & data sources |

---

## 🚀 Deploy on GitHub Pages

### Option 1 — Quick Deploy (Recommended)

1. **Create a new GitHub repository** (e.g., `tata-motors-eda`)
2. **Upload `index.html`** to the root of the repository
3. Go to **Settings → Pages**
4. Under **Source**, select `Deploy from a branch`
5. Choose `main` branch → `/ (root)` → click **Save**
6. Wait ~60 seconds — your site will be live at:
   ```
   https://<your-username>.github.io/<repo-name>/
   ```

### Option 2 — Using Git CLI

```bash
# 1. Create a new folder and initialize Git
mkdir tata-motors-eda && cd tata-motors-eda
git init

# 2. Copy index.html into this folder, then:
git add index.html
git commit -m "Initial commit: Tata Motors Capital Structure EDA"

# 3. Push to GitHub (create the repo on GitHub first)
git remote add origin https://github.com/<your-username>/tata-motors-eda.git
git branch -M main
git push -u origin main

# 4. Enable GitHub Pages in repo Settings → Pages → main / root
```

---

## 📁 File Structure

```
tata-motors-eda/
└── index.html          ← Single self-contained file (all CSS, JS, data embedded)
```

No build step, no dependencies to install. Everything is embedded in `index.html`.

---

## 🛠 Tech Stack

- **HTML5 / CSS3 / Vanilla JS** — zero framework dependencies
- **Chart.js 4.4.1** — loaded from cdnjs CDN
- **Google Fonts** — Syne, DM Mono, Fraunces
- All data embedded as JavaScript arrays — works fully offline after first load

---

## 📖 Data Sources

- Tata Motors Annual Reports FY2015–FY2024 (IFRS Consolidated)
- BSE India Filings — Scrip: 500570 (TATAMOTORS)
- NSE India / Screener.in (Market Cap data)
- Peer data from individual company Annual Reports FY2024

---

## ⚠️ Disclaimer

This analysis is for educational and research purposes only. Data sourced from public filings. Figures may differ from Bloomberg/Reuters due to rounding conventions.
