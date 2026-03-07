# 🇸🇦 KSA CPI Supply Chain Intelligence

**Strait of Hormuz Vulnerability Assessment | Ministry of Economy & Planning**

A strategic intelligence dashboard analyzing the KSA CPI food basket's exposure to Strait of Hormuz supply chain disruption under an Iran-USA-Israel conflict scenario. Covers 154 CPI items with alternative sourcing routes.

![Dashboard Preview](https://img.shields.io/badge/Items_Analyzed-154-blue) ![Risk](https://img.shields.io/badge/Hormuz_Risk-17.7%25_CPI_Weight-red) ![Alternatives](https://img.shields.io/badge/Alt_Routes_Mapped-38-green)

## Features

- **Supply Chain Flow Map** — Sankey diagram: Source Countries → Shipping Routes → KSA CPI Categories
- **Risk Analytics** — CPI-weighted Hormuz exposure by sector
- **Alternative Sourcing** — 10 Hormuz-dependent flows with 38 safe alternatives
- **Geographic Route Map** — Interactive world map comparing current vs. alternative shipping routes

## Quick Deploy to GitHub Pages

### Prerequisites
- [Git](https://git-scm.com/) installed
- [Node.js](https://nodejs.org/) v18+ installed
- A GitHub account

### Step-by-Step (5 minutes)

**1. Create a new GitHub repository**

Go to https://github.com/new and create a repo named `ksa-cpi-intelligence` (public).

**2. Open terminal and run these commands:**

```bash
# Navigate to the project folder (where you unzipped the files)
cd ksa-cpi-intelligence

# Initialize git
git init
git add .
git commit -m "KSA CPI Supply Chain Intelligence Dashboard"

# Connect to your GitHub repo (replace YOUR_USERNAME)
git remote add origin https://github.com/YOUR_USERNAME/ksa-cpi-intelligence.git
git branch -M main
git push -u origin main

# Deploy to GitHub Pages
npm run deploy
```

**3. Enable GitHub Pages**

- Go to your repo on GitHub → **Settings** → **Pages**
- Under "Source", select **Deploy from a branch**
- Select branch: **gh-pages** → folder: **/ (root)**
- Click **Save**

**4. Access your site**

Your dashboard will be live at:
```
https://YOUR_USERNAME.github.io/ksa-cpi-intelligence/
```

It takes 1-2 minutes for the first deployment to go live.

### Updating the Dashboard

After making changes to the code:

```bash
git add .
git commit -m "Updated analysis"
git push
npm run deploy
```

## Local Development

```bash
npm install
npm run dev
```

Opens at `http://localhost:5173/ksa-cpi-intelligence/`

## Tech Stack

- **React 18** — UI framework
- **D3.js v7** — Data visualization (Sankey flow, geographic map)
- **Vite** — Build tool
- **gh-pages** — GitHub Pages deployment

## Data Source

154 CPI food basket items from KSA GASTAT, with supply chain analysis including:
- Country of origin
- Primary raw material
- Raw material source countries
- Strait of Hormuz routing assessment

---

*Built for strategic intelligence by AI Economic Pulse*
