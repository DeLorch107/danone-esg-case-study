# Danone Yogurt LCA - Carbon Footprint Analysis

A reproducible cradle-to-retail life cycle assessment (LCA) case study for Danone yogurt, built with publicly available data to model emissions and evaluate reduction scenarios.

## Overview

This repository contains a transparent carbon footprint model for a 150g Danone yogurt SKU (France/EU market), using public data sources including Danone sustainability reports, AGRIBALYSE/ecoinvent databases, and DEFRA emission factors. The analysis computes baseline emissions (kgCO₂e per SKU), models 4-6 practical reduction levers, and estimates their abatement potential with associated costs.

**Note:** This is a methodological case study using public data proxies, not internal Danone procurement data. Results are illustrative and intended to demonstrate LCA methodology and scenario analysis capabilities.

## Project Objectives

- **Baseline Assessment:** Calculate single-SKU carbon footprint with documented confidence intervals
- **Scenario Modeling:** Analyze 4-6 realistic reduction levers across energy, supply chain, packaging, and logistics
- **Financial Analysis:** Estimate €/tCO₂e abatement costs with CAPEX/OPEX considerations
- **Reproducibility:** Provide fully executable notebooks with transparent assumptions and data sources

## Quick Start

```bash
git clone https://github.com/DeLorch107/danone-esg-case-study
cd danone-esg-case-study
pip install -r requirements.txt
jupyter lab notebooks/
```

### Key Analysis Notebooks

1. `01_data_cleaning.ipynb` - Data preparation and validation
2. `02_baseline_emissions.ipynb` - LCA calculations and baseline model
3. `03_scenarios.ipynb` - Reduction scenario development
4. `04_financial_analysis.ipynb` - Abatement cost analysis

## Methodology

The analysis follows GHG Protocol standards for Scope 3 accounting and uses a cradle-to-retail system boundary. For detailed methodology, see [METHODOLOGY.md](METHODOLOGY.md).

### Scope Definition

- **Product:** Danone set yogurt, 150g pot (France/EU)
- **System Boundary:** Cradle-to-retail (excludes consumer use and disposal)
- **Baseline Year:** 2020
- **Impact Category:** Climate change (kgCO₂e)
- **Allocation Method:** Mass-based for multi-output processes

## Project Structure

```
danone-esg-case-study/
├── METHODOLOGY.md              # Complete technical approach
├── notebooks/                  # Jupyter notebooks for analysis
│   ├── 01_data_cleaning.ipynb
│   ├── 02_baseline_emissions.ipynb
│   ├── 03_scenarios.ipynb
│   └── 04_financial_analysis.ipynb
├── data/                       
│   ├── raw/                   # Original data files
│   ├── processed/             # Cleaned datasets
│   └── emission_factors/      # LCA databases
├── src/                        # Python modules
│   ├── lca_calculator.py
│   ├── scenario_builder.py
│   └── visualization.py
├── docs/
│   ├── assumptions.md         # Modeling assumptions
│   ├── data-sources.md        # Data references
│   └── phase-guides/          # Step-by-step documentation
└── outputs/                    # Final deliverables
    ├── presentation/
    └── kpi_summary.pdf
```

## Key Results

### Baseline Emissions
[Results pending - will include emissions breakdown by life cycle stage]

### Reduction Scenarios

| Scenario | Abatement Potential | Cost (€/tCO₂e) | Implementation Complexity |
|----------|-------------------|----------------|-------------------------|
| Renewable Energy | TBD | TBD | Medium |
| Regenerative Agriculture | TBD | TBD | High |
| Packaging Optimization | TBD | TBD | Low |
| Transport Efficiency | TBD | TBD | Medium |

### Top Recommendations
1. [To be completed based on analysis results]
2. [To be completed based on analysis results]
3. [To be completed based on analysis results]

## Data Sources

- **AGRIBALYSE v3.1** - French environmental database for agricultural products
- **ecoinvent v3.8** - Global life cycle inventory database
- **DEFRA 2023** - UK Government emission factors
- **Danone Reports** - Public sustainability disclosures (2020-2023)
- **GLEC Framework** - Logistics emissions methodology

Full data source documentation: [data-sources.md](docs/data-sources.md)

## Technical Requirements

- Python 3.8+
- pandas, numpy for data processing
- matplotlib, plotly for visualization
- jupyter for interactive notebooks

See `requirements.txt` for complete dependencies.

## Documentation

### Core Documents
- [METHODOLOGY.md](METHODOLOGY.md) - Complete LCA methodology
- [assumptions.md](docs/assumptions.md) - All modeling assumptions with sensitivity ranges
- [data-sources.md](docs/data-sources.md) - Data provenance and quality assessment

### Phase Guides
Detailed implementation guides for each project phase:
- [Phase 0: Project Scope](docs/phase-guides/00-project-scope.md)
- [Phase 1: Data Collection](docs/phase-guides/01-data-collection.md)
- [Phase 2: Baseline Model](docs/phase-guides/02-baseline-model.md)
- [Phase 3: Scenario Development](docs/phase-guides/03-scenario-development.md)
- [Phase 4: Financial Analysis](docs/phase-guides/04-financial-analysis.md)
- [Phase 5: Uncertainty & Validation](docs/phase-guides/05-uncertainty-validation.md)
- [Phase 6: Deliverables](docs/phase-guides/06-deliverables.md)

## Deliverables

- **Executive Presentation:** 10-12 slide deck with key findings and recommendations
- **KPI Summary:** One-page dashboard with baseline and scenario results
- **Technical Repository:** This GitHub repo with reproducible analysis
- **Interactive Notebooks:** Step-by-step calculations with visualizations

## Limitations

- Results based on public data proxies, not actual supplier data
- Uncertainty inherent in agricultural emission factors (±30-50%)
- Cost estimates are order-of-magnitude approximations
- Excludes consumer use phase and end-of-life emissions

## Contact

**Ibrahim ELORCH**  
Email: ibrahim.elorch@emines.um6p.ma  
LinkedIn: [Ibrahim Elorch](https://www.linkedin.com/in/ibrahim-elorch-6879782ba/)

## License

MIT License - see [LICENSE](LICENSE) file for details

---

*This project demonstrates LCA methodology for food products using public data. Results should not be interpreted as official Danone product footprints.*
