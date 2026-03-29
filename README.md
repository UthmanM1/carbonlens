# CarbonLens 🌿
### Know your carbon footprint. Shrink it with AI.

CarbonLens is a personal carbon footprint tracker that lets you log your daily activities like travel, food, home energy, flights, and shopping, and instantly see your CO₂ impact visualised. It then uses AI to generate personalised, data-driven tips to help you reduce your emissions.

---

## Live demo

Open `index.html` in any browser. No build step, no server, no dependencies to install.

---

## Features

- **Activity logger** — Log transport, food, energy, flights, and shopping with accurate CO₂ factors sourced from UK government emissions data (DEFRA 2023)
- **Live dashboard** — Donut and bar charts update instantly as you add activities, with a colour-coded impact score
- **AI recommendations** — Powered by (Anthropic API): personalised, specific tips based on your actual logged data, not generic advice
- **Comparison view** — See how your footprint stacks up against the UK average, EU average, and the Paris 1.5°C target
- **Zero backend** — Everything runs in the browser. Your data never leaves your device.

---

## How to run

### Option 1 — Open directly (recommended for demo)
1. Download or clone this repository
2. Open `index.html` in Chrome, Firefox, or Safari
3. Start logging activities on the **Log activity** tab
4. Go to **AI tips**, enter your Anthropic API key, and click **Analyse my footprint**

### Option 2 — Serve locally
```bash
npx serve .
# or
python3 -m http.server 8080
```

---

## Carbon emission factors

All CO₂ calculations use peer-reviewed emission factors:

| Category | Source |
|----------|--------|
| Transport | UK DEFRA GHG Conversion Factors 2023 |
| Food | Our World in Data / Poore & Nemecek (2018) |
| Energy | UK National Grid ESO (2023 grid intensity) |
| Flights | ICAO Carbon Emissions Calculator methodology |
| Shopping | lifecycle assessment averages (WRAP 2023) |

---

## Tech stack

| Layer | Technology |
|-------|-----------|
| Frontend | Vanilla HTML, CSS, JavaScript |
| Charts | Chart.js 4.4 |
| AI | Large language model API (via browser fetch) |
| Fonts | DM Sans + DM Serif Display (Google Fonts) |
| Deployment | Static file — no server needed |

---

## Project structure

```
carbonlens/
├── index.html        # Entire application (single file)
├── README.md         # This file
└── screenshots/
    ├── dashboard.png
    ├── logger.png
    ├── tips.png
    └── compare.png
```

---

## Hackathon track

**Quantum Sprint — Best Climate Impact Project**

CarbonLens addresses the challenge of personal carbon awareness. Most people have no idea what their daily choices cost the planet in CO₂ terms. By making that invisible visible, and pairing it with personalised AI guidance, CarbonLens creates a pathway from awareness to action.

### Judging criteria alignment

| Criterion | How CarbonLens delivers |
|-----------|------------------------|
| Innovation | AI-personalised tips based on *actual user data*, not generic lists |
| Functionality | Fully working: log, calculate, visualise, compare, get AI tips |
| Real-world usability | Zero install, runs in any browser, real emission data |
| Design & UX | Clean, accessible, responsive — judges can use it live in the demo |
| Climate impact | Addresses behaviour change, the hardest problem in climate action |

---

## Potential extensions

- Streak tracking and weekly goals
- Carbon offset marketplace integration
- Team/household mode
- Export to CSV / share card
- Historical trend chart
- Integration with smart meter APIs

---

## Built with

- Chart.js — for data visualisations
- Quantum Sprint Hackathon — for the motivation


