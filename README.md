# Enterprise-BI-Analytics-Platform-Comparison
Comparative analysis of Oracle FDI, Power BI, Tableau, IBM Cognos, and Workday Prism
# Enterprise BI & Analytics Documentation (MkDocs Ready)

This repository contains an MkDocs Material site with GitHub Pages deployment.

---

## 📁 REQUIRED REPOSITORY STRUCTURE

Create this structure in your repo:
.
├── mkdocs.yml
├── requirements.txt
├── README.md
├── .gitignore
├── docs/
│   ├── index.md
│   ├── overview/
│   │   ├── executive-summary.md
│   │   └── platform-positioning.md
│   ├── architecture/
│   │   ├── analytics-layers.md
│   │   └── integration-patterns.md
│   └── platforms/
│       ├── oracle-fdi.md
│       ├── power-bi.md
│       ├── tableau.md
│       ├── ibm-cognos.md
│       └── workday-prism.md
└── .github/
└── workflows/
└── gh-pages.yml
---

## 📄 mkdocs.yml

```yaml
site_name: Enterprise BI & Analytics Platform Comparison
site_description: Comparative analysis of Oracle FDI, Power BI, Tableau, IBM Cognos, and Workday Prism
site_url: https://<YOUR_GITHUB_USERNAME>.github.io/<REPO_NAME>/

theme:
  name: material
  features:
    - navigation.tabs
    - navigation.sections
    - navigation.expand
    - search.highlight
    - search.suggest

nav:
  - Home: index.md
  - Overview:
      - Executive Summary: overview/executive-summary.md
      - Platform Positioning: overview/platform-positioning.md
  - Architecture:
      - Analytics Layers: architecture/analytics-layers.md
      - Integration Patterns: architecture/integration-patterns.md
  - Platforms:
      - Oracle Fusion Data Intelligence: platforms/oracle-fdi.md
      - Power BI: platforms/power-bi.md
      - Tableau: platforms/tableau.md
      - IBM Cognos: platforms/ibm-cognos.md
      - Workday Prism: platforms/workday-prism.md

markdown_extensions:
  - admonition
  - tables
  - toc:
      permalink: true
