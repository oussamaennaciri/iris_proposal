# International Risk Intelligence System
### MSDS692 — Data Science Practicum I
**Regis University | Anderson College of Business and Computing**
**Author: Oussama Ennaciri**

---

## Project Overview

A near-real-time geopolitical intelligence platform that ingests, integrates,
and models data from nine open international data sources to produce
country-level risk scores, anomaly alerts, and relationship graphs for
multilateral decision support.

Built as an open, neutral alternative to proprietary systems such as Palantir
Gotham — purpose-designed for the United Nations, ICRC, World Bank, and
international agencies that require politically neutral, globally comprehensive
intelligence infrastructure.

---

## Repository Structure

```
iris_proposal/
├── main.tex          # Full IEEE-format practicum proposal
├── references.bib    # BibTeX references (11 sources)
├── IEEEtran.cls      # IEEE LaTeX formatting class
├── figures/          # Figures directory (architecture diagram to be added)
└── README.md         # This file
```

---

## Data Sources

| Source | Content | Update Frequency |
|---|---|---|
| GDELT Project | 250M+ global events, 300 categories | Every 15 minutes |
| ACLED | Armed conflict and political violence | Weekly |
| World Bank API | 16,000+ economic indicators | Quarterly |
| UN Comtrade | Bilateral trade flows | Monthly |
| UNHCR Statistics | Displacement and refugee data | Regular |
| OpenSanctions | 332 global sanctions lists | Real-time |
| UN GA Voting | Member state votes, 1946-2023 | Per session |
| V-Dem | Democracy and institutional indicators | Annual |
| GPR Index | News-based geopolitical risk scores | Monthly |

---

## System Architecture

Four layers:
1. **Ingestion Pipeline** — Apache Airflow orchestrating all 9 sources
2. **Graph Engine** — NetworkX + Neo4j for relationship mapping
3. **ML Layer** — XGBoost risk scorer + Isolation Forest anomaly detector
4. **Dashboard** — Streamlit + Pyvis live interface

---

## Compiling the Proposal

**Overleaf (recommended):**
Import this repository directly via New Project > Import from GitHub.

**Local:**
```bash
pdflatex main.tex
bibtex main
pdflatex main.tex
pdflatex main.tex
```

---

## Course Information

- Course: MSDS692 S40 Data Science Practicum I
- Professor: Dr. Ghulam Mujtaba
- Institution: Regis University, Denver CO
