# IBD-Chile

Analysis pipeline for **PhIP-Seq data from the IBD-Chile cohort**, built around development workflows from **`phiper`**.

This repository contains code to:

- reshape peptide-level PhIP-Seq matrices into a long-format dataset,
- export the analysis-ready object to **Parquet**,
- run peptide- and taxon-level exploratory and differential analyses with **phiper**,
- generate static and interactive figures,
- render an automated **Quarto HTML summary report**, and
- launch report generation on an **HPC/Slurm** environment.

---

## Repository layout

```text
IBD-Chile/
├── Data/
│   └── IBD-Chile_MUW.parquet
├── assets/
│   └── logos/
├── scripts/
│   └── get_reports.sh
│   └── run_phiper.sh
│   └── submit_phiper_analysis.sh
├── src/
│   ├── R/
│   │   ├── 01-create_phiper_object.R
│   │   ├── 02-run_phiper_analysis.R
│   │   └── 03-render_phiper_reports.R
│   └── template/
│       └── phiper_summary_report.qmd
└── README.md
