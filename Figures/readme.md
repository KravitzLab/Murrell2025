# Murrell2026 — Figures

This folder contains the **figure-generation notebooks** and **schematic art assets** used to produce figures for the Murrell (2026) project.

At a high level:
- `Murrell_2026_Fig*.ipynb` notebooks generate analysis panels and plots for specific manuscript figures.
- `Murrell_2026jpgs/` contains **schematic image files** used in the figure assemblies.

---

## Contents

---

## Notebooks

### `Murrell_2026_Fig1.ipynb`
Notebook for **Figure 1**. The header indicates authorship and last update metadata. :contentReference[oaicite:1]{index=1}

Key traits:
- Designed to run in a notebook environment (imports include `google.colab`). :contentReference[oaicite:2]{index=2}
- Installs/uses the FED3 analysis stack (e.g., `fed3`, `fed3bandit`) and common stats/plotting libs (e.g., `pingouin`, `statsmodels`, `matplotlib`, `seaborn`). :contentReference[oaicite:3]{index=3}
- Pulls behavioral data from GitHub-hosted zip exports (e.g., Bandit100) and joins against the subject key (`Murrell2026_Key.csv`). :contentReference[oaicite:4]{index=4}

### `Murrell_2026_Fig2.ipynb`
Notebook for **Figure 2** (same author/update header style as Fig 1). :contentReference[oaicite:5]{index=5}

Key traits:
- Uses the same install/import scaffold as Fig 1 (FED3 + stats/plotting stack). :contentReference[oaicite:6]{index=6}
- Loads **FR1** data from a GitHub-hosted zip and joins to `Murrell2026_Key.csv` for metadata. :contentReference[oaicite:7]{index=7}

### `Murrell_2026_Fig3.ipynb`
Notebook for **Figure 3**. The header notes this figure is focused on **Bandit 80/20** and “metrics of performance in trained mice (last 24 hours)”. :contentReference[oaicite:8]{index=8}

Key traits:
- Same general analysis environment as Fig 1/2. :contentReference[oaicite:9]{index=9}
- Loads **Bandit80** data from GitHub-hosted zip exports and joins to `Murrell2026_Key.csv`. :contentReference[oaicite:10]{index=10}

---

## Schematic assets (`Murrell_2026jpgs/`)

This subfolder contains schematic PNGs for **Figures 1–5**, named consistently as:

- `Murrell_2026_Figure{N}_schematic.png` :contentReference[oaicite:11]{index=11}

These are intended to be dropped into the final figure layouts (Illustrator/PowerPoint/Inkscape/etc.) or imported into notebooks/scripts that assemble composite figure panels.

---

## How to use

1. Open the appropriate notebook for the figure you want (`Murrell_2026_Fig1.ipynb`, etc.). :contentReference[oaicite:12]{index=12}
2. Run the install/import cells (the notebooks are set up to install missing dependencies).
3. Run the data import cell(s) — the notebooks download the needed task zip(s) and the key file from GitHub. :contentReference[oaicite:13]{index=13}
4. Export plots/panels as needed and combine with the schematic PNGs from `Murrell_2026jpgs/`. :contentReference[oaicite:14]{index=14}

---

## Notes

- These notebooks are written in a “Colab-friendly” style (e.g., they import `google.colab` and include download helpers). :contentReference[oaicite:15]{index=15}
- If you add new figure notebooks, please follow the naming convention `Murrell_2026_Fig{N}.ipynb` and add any new static assets to `Murrell_2026jpgs/` (or a clearly named subfolder).
