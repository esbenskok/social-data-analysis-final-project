# Testing Running Myths — Lyngby Half Marathon 2026

**Social Data Analysis · DTU 2026 · Marta Arana · Esben · Sergi**

> *"We stopped arguing about running advice and decided to test it with data."*

On April 26, 2026, 25 runners lined up at the Lyngby Half Marathon. They had different training backgrounds, different experience levels, and very different race days. We collected their GPS tracks, heart rate data, and training logs — and put four classic running myths to the test.

---

## The Myths

| # | Myth | Verdict |
|---|---|---|
| 1 | Experienced runners pace themselves better | Supported |
| 2 | Hill training helps on a hilly course | Supported |
| 3 | More training always means faster times | Partially supported |
| 4 | Interval training leads to smarter race strategy | Partially supported |

---

## Repository Structure

```
├── docs/
│   └── index.html              ← Interactive website (GitHub Pages — live site)
├── notebook/
│   └── explainer_notebook.ipynb
├── data/
│   ├── processed/
│   │   ├── lyngby_runners_2026.csv   ← Master dataset (25 runners, 22 columns)
│   │   └── 🏃 Lyngby Halvmarathon 2026 — Datos del corredor (respuestas).xlsx
│   └── race_day/               ← Raw GPX files (25 runner folders)
├── requirements.txt
└── README.md
```

> The website is fully self-contained — photos and map data are embedded. Also available at the live URL below.

---

## Setup

```bash
pip install -r requirements.txt
jupyter notebook notebook/explainer_notebook.ipynb
```

---

## The Website

**Live:** https://esbenskok.github.io/social-data-analysis-final-project/

Or open `docs/index.html` directly in any browser — no server needed.

**Features:** interactive runner profiles · GPS route heatmap per runner · 6,759-point elevation chart with synchronized map cursor · four myth sections · Copenhagen HM comparison.

---

## The Dataset

`data/processed/lyngby_runners_2026.csv` — 25 runners × 22 columns including `finish_min`, `target_min`, `km_per_week`, `training_weeks`, `archetype`, `trained_hills`, `trains_intervals`, `split_ratio`, `has_gps`.

---

## Team

| | |
|---|---|
| **Marta Arana** | Data collection, GPX pipeline, hill training analysis, website design |
| **Esben** | EDA, prediction model, Myth 3, Segal & Heer analysis |
| **Sergi** | Course visualisations, Myth 1 & 4, interactive charts |
