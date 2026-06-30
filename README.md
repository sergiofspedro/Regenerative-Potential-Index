# Regenerative Potential Index (RPI)

An evaluation framework for assessing regenerative potential — applicable to both **public and private sectors**. This case study applies the RPI methodology to the districts of the **municipality of Amsterdam**, tracking economic, environmental, political and social dimensions across a decade of data (2015–2024) with scenario projections to 2050.

🌐 **[View interactive visualizations →](https://sergiofspedro.github.io/Regenerative-Potential-Index/)**

---

## Framework Overview

The RPI aggregates multiple indicators into four dimensions:

| Dimension | Focus |
|-----------|-------|
| **Economic** | Local economic activity, employment, business dynamics |
| **Environmental** | Air quality, energy use, waste management |
| **Political** | Civic participation, governance, community influence |
| **Social** | Education, social cohesion, discrimination, neighbourhood contact |

Each indicator is normalized to a 0–100 scale (z-score, k=15), aggregated by dimension, and combined into an overall RPI score per district per year.

## Case Study: Amsterdam

- **Geography**: Amsterdam municipality + individual districts
- **Period**: 2015–2024 (observed) + scenarios to 2030 and 2050
- **Scenarios**: Constrained, Business-As-Usual, Optimistic

## Interactive Visualizations

The GitHub Pages site includes six interactive charts built with **Plotly** and **Folium**:

1. **RPI Overall time evolution** (2015–2024) — district trajectories with hover
2. **Dimension time series** — dropdown to switch between Economic / Environmental / Political / Social
3. **District comparison 2024** — bar chart with dimension selector
4. **Scenario projections** — 2030 & 2050 forecasts, toggle by scenario
5. **Interactive district map** — Amsterdam choropleth with tooltips
6. **Indicator correlation heatmap** — Pearson correlations, post-normalization

## Repository Structure

```
├── FINAL_RPI_updated.ipynb   # Full pipeline: data → normalization → viz → export
├── docs/
│   ├── index.html            # GitHub Pages portfolio site
│   ├── assets/style.css      # Styles
│   └── charts/               # Generated HTML charts (committed after running notebook)
└── README.md
```

## Running the Notebook

1. Open `FINAL_RPI_updated.ipynb` in **Google Colab**
2. Mount Google Drive (cell 1) — data files required
3. Run all cells — charts are exported to `docs/charts/`
4. Commit `docs/charts/*.html` to the repo
5. GitHub Pages serves the portfolio automatically

```bash
# After running the notebook and generating docs/charts/*.html:
git add docs/charts/
git commit -m "update interactive charts"
git push
```

## Dependencies

```
pip install plotly folium geopandas pandas numpy openpyxl
```

---

*PhD Research · Urban Regeneration · Management PhD*
