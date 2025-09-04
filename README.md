# Danone Yogurt LCA - Carbon Footprint Analysis
*Cradle-to-retail emissions assessment with reduction scenarios*

## Project Overview

**What this repo is.** A reproducible cradle-to-retail LCA case study for a Danone yogurt SKU (150 g, France/EU) built with public data (Danone reports, AGRIBALYSE / ecoinvent, DEFRA). The goal: compute a defensible baseline footprint (kgCO₂e per SKU), model 4–6 practical reduction levers, estimate abatement potential and €/tCO₂e, and deliver a small investor-style package (10–12 slide deck + one-page KPI PDF + GitHub repo with runnable notebooks and documented assumptions).

**Quick truth:** this is a public-data case study — not internal Danone procurement data. Expect proxies and documented assumptions; the value is in methodology, reproducibility, sensitivity analysis, and clear communication of uncertainties.

## Project Goal & Success Criteria

### Goal
Produce a reproducible, transparent cradle-to-retail carbon model for a Danone yogurt SKU (150 g, France/EU) that translates public LCA datasets and company disclosures into actionable mitigation insight. Deliverables are aimed at both technical reproducibility (notebooks + data + assumptions) and high-level decision making (abatement curve, top recommendations, cost/impact tradeoffs).

### Core Objectives
- **Reproducible baseline:** single-number headline (kgCO₂e / SKU) with documented inputs and a 90% confidence interval or sensitivity bands.
- **Scenario analysis:** 4–6 realistic levers (energy, farm/supply, packaging, logistics, combination) with tCO₂e avoided and implementation notes.
- **Financial lens:** €/tCO₂e for each lever (range estimates), order-of-magnitude CAPEX/OPEX and payback where possible.
- **Deliverables:** runnable notebooks, `assumptions.md`, `data_sources.md`, 10–12 slide deck, one-page KPI PDF, and a polished `README`.
- **Reproducibility:** notebooks run end-to-end on public proxies; all data sources and transforms logged.

### Success Criteria (what “done” looks like)
- Notebooks execute from raw CSV → final charts without manual edits.
- `assumptions.md` lists every proxy with high/base/low values.
- Baseline footprint reported with uncertainty (± range or MC output).
- Abatement curve completed with €/tCO₂e for each lever and a transparent cost-source for each number.
- A concise deck + one-pager suitable for a hiring manager / sustainability reviewer.
- GitHub repo is tidy, versioned, and contains `README`, `requirements.txt`, and example data.

### Limitations & expected caveats
- Results are illustrative and depend strongly on ingredient origin and farm-level data; do **not** claim corporate-level accuracy.
- Treat estimates as decision-support scenarios, not audit-grade accounting.

**Intended audience:** sustainability analysts, hiring managers, recruiters, and anyone evaluating methodology for food-product LCAs.

![Python](https://img.shields.io/badge/Python-3.8+-blue) ![LCA](https://img.shields.io/badge/LCA-GHG%20Protocol-green) ![Status](https://img.shields.io/badge/Status-In%20Progress-yellow)

**Key Result:** [Results will be added upon completion]

## 🔍 **[READ THE METHODOLOGY](METHODOLOGY.md)** 📋
*Complete LCA approach following GHG Protocol standards*

---

## 🗺️ Quick Navigation
| Section | Description | Time to Read |
|---------|-------------|--------------|
| [**📊 Key Results**](#-key-results) | Main findings & visuals | 2 min |
| [**🛠️ Run Analysis**](#-run-analysis) | Clone & reproduce | 5 min |
| [**📚 Methodology**](METHODOLOGY.md) | Technical approach | 10 min |
| [**📁 Project Structure**](#-project-structure) | Repo organization | 1 min |

---

## 📊 Key Results

![Emissions Breakdown](images/results/sankey_baseline.png)
*[Baseline emissions chart will be added here]*

### Reduction Scenarios
![Abatement Curve](images/results/abatement_curve.png)

**Top 3 Recommendations:**
1. [Recommendation 1 - impact and cost data pending]
2. [Recommendation 2 - impact and cost data pending]
3. [Recommendation 3 - impact and cost data pending]

> 📖 **Details:** Full analysis methodology in [METHODOLOGY.md](METHODOLOGY.md)

---

## 🛠️ Run Analysis

### Quick Start
```bash
git clone https://github.com/DeLorch107/danone-esg-case-study
cd danone-esg-case-study
pip install -r requirements.txt
jupyter lab notebooks/
```

### Key Notebooks
- `01_data_cleaning.ipynb` - Data preparation
- `02_baseline_emissions.ipynb` - LCA calculations  
- `03_scenarios.ipynb` - Reduction scenarios
- `04_financial_analysis.ipynb` - Abatement costs

---

## 🎯 Project Scope

**Product:** Danone set yogurt, 150g pot (France/EU)  
**Boundary:** Cradle-to-retail  
**Baseline Year:** 2020  
**Methodology:** GHG Protocol + AGRIBALYSE

> 📋 **Complete scope definition:** [Phase 0 - Project Scope](docs/phase-guides/00-project-scope.md)

---

## 📁 Project Structure

```
danone-esg-case-study/
├── 📖 METHODOLOGY.md           # Technical approach
├── 📊 notebooks/               # Interactive analysis
├── 📁 data/                   # Datasets & emission factors
├── 🖼️ images/                  # Charts & diagrams
├── 📋 docs/phase-guides/       # Step-by-step guides
├── 💻 src/                     # Reusable Python functions
└── 📈 outputs/                 # Final deliverables
```

---

## 🛠️ Technical Stack

**LCA Data Sources:**
- AGRIBALYSE (French food LCA database)
- ecoinvent (Global LCI datasets)
- DEFRA emission factors

**Analysis Tools:**
- Python: pandas, numpy, matplotlib, plotly
- Jupyter notebooks
- GitHub

**Standards:**
- GHG Protocol Scope 3 guidance
- GLEC framework for logistics emissions

---

## 📈 Key Findings Summary

| Metric | Baseline | Best Case | Reduction |
|--------|----------|-----------|-----------|
| **Total Emissions** | [TBD] | [TBD] | [TBD] |
| **Ingredient Impact** | [TBD] | [TBD] | [TBD] |
| **Packaging Impact** | [TBD] | [TBD] | [TBD] |
| **Energy Impact** | [TBD] | [TBD] | [TBD] |

**Implementation Cost:** [Results pending]  
**Timeline:** [Results pending]

---

## 📚 Documentation

### Core Documentation
- **[METHODOLOGY.md](METHODOLOGY.md)** - Complete LCA methodology & calculations
- **[assumptions.md](docs/assumptions.md)** - All modeling assumptions
- **[data-sources.md](docs/data-sources.md)** - Data source references

### Phase-by-Phase Guides
- [Phase 0: Project Scope](docs/phase-guides/00-project-scope.md)
- [Phase 1: Data Collection](docs/phase-guides/01-data-collection.md)  
- [Phase 2: Baseline Model](docs/phase-guides/02-baseline-model.md)
- [Phase 3: Scenario Development](docs/phase-guides/03-scenario-development.md)
- [Phase 4: Financial Analysis](docs/phase-guides/04-financial-analysis.md)
- [Phase 5: Uncertainty & Validation](docs/phase-guides/05-uncertainty-validation.md)
- [Phase 6: Deliverables](docs/phase-guides/06-deliverables.md)

---

## 🎯 Final Deliverables

- 📊 [Presentation](outputs/presentation/) - [To be completed]
- 📋 [KPI summary](outputs/kpi_summary.pdf) - [To be completed]
- 💻 Reproducible Python analysis
- 📈 Interactive Jupyter notebooks

---

## 👤 Contact

**Ibrahim ELORCH**  
📧 ibrahim.elorch@emines.um6p.ma  
🔗 [LinkedIn](https://www.linkedin.com/in/ibrahim-elorch-6879782ba/)

---

## 📄 License
MIT License - see [LICENSE](LICENSE) file for details
