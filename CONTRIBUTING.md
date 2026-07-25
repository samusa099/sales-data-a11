# 🛠️ Contributing Guide

Thank you for considering a contribution to **Sales Data Analysis — Assessment 11**.

This repository is an educational and portfolio-oriented Excel-to-Power BI project. Contributions should improve accuracy, usability, documentation, data quality, security, or the clarity of the analytical workflow.

## Ways to Contribute

Useful contributions include:

- correcting documentation, spelling, links, or formatting;
- improving Excel data-quality checks or source organisation;
- refining Power Query transformation steps;
- improving Power BI measures, relationships, filters, or report usability;
- adding validated KPI definitions or a data dictionary;
- strengthening security, privacy, or troubleshooting guidance;
- improving accessible visual assets and repository documentation; and
- reporting reproducible bugs or broken file paths.

## Repository Structure

Please preserve the current structure:

```text
sales-data-a11/
├── data/
│   └── raw/
│       └── Orders.xlsx
├── reports/
│   └── power-bi/
│       └── eOrderid_powerbi.pbix
├── docs/
│   └── HOW_TO_USE.md
├── assets/
│   ├── cover/
│   └── preview/
├── README.md
├── CODE_OF_CONDUCT.md
├── CONTRIBUTING.md
├── SECURITY.md
└── LICENSE
```

Do not move files or introduce new top-level folders without explaining why the change improves navigation or maintainability.

## Before You Start

1. Review [`README.md`](README.md), [`docs/HOW_TO_USE.md`](docs/HOW_TO_USE.md), [`SECURITY.md`](SECURITY.md), and [`CODE_OF_CONDUCT.md`](CODE_OF_CONDUCT.md).
2. Search existing issues and pull requests to avoid duplicate work.
3. Create a focused branch from the latest `main` branch.
4. Keep each contribution limited to one clear purpose.
5. Never use confidential, personal, customer, employee, payroll, banking, tax, or credential data.

## Suggested Branch Names

Use short, descriptive branch names:

```text
docs/improve-usage-guide
fix/power-bi-source-path
feature/add-kpi-dictionary
assets/update-project-preview
```

## Working with the Excel Dataset

When changing `data/raw/Orders.xlsx`:

- preserve a backup of the original file;
- document changed sheets, columns, formulas, or named ranges;
- avoid merged cells inside the main data table;
- keep dates, quantities, and monetary fields in valid data types;
- check blanks, duplicates, invalid identifiers, and outliers;
- disclose external links and data connections; and
- do not add macros or executable content without prior discussion.

## Working with the Power BI Report

When changing `reports/power-bi/eOrderid_powerbi.pbix`:

- confirm that the report points to the intended Excel source;
- review every Power Query step for errors;
- document material changes to measures, relationships, filters, or visuals;
- validate key report totals against the Excel source;
- remove credentials and environment-specific secrets;
- disclose added custom visuals or external connectors; and
- include a concise change summary because GitHub cannot display a normal text diff for `.pbix` files.

A screenshot or written validation note is strongly recommended for material dashboard changes.

## Documentation and Visual Assets

For Markdown changes:

- use clear headings and concise professional language;
- keep relative links valid after any file move;
- avoid unsupported claims or fabricated analytical findings;
- distinguish designed mockups from actual report screenshots; and
- maintain consistent terminology across README, guide, and security documentation.

For SVG or image changes:

- use descriptive file names and alt text;
- keep text readable at normal GitHub display sizes;
- avoid unnecessary large files;
- do not include copyrighted or confidential visual material without permission; and
- verify that the asset renders correctly in GitHub light and dark interfaces where practical.

## Commit Messages

Use concise, action-oriented commit messages:

```text
Improve Power BI refresh instructions
Fix broken dataset download links
Add KPI validation checklist
Update project preview alignment
```

Avoid vague messages such as `update`, `changes`, or `fix stuff`.

## Pull Request Checklist

Before opening a pull request, confirm:

- [ ] The contribution has one clear purpose.
- [ ] The latest `main` branch was used as the base.
- [ ] File paths and documentation links work.
- [ ] Excel data types and source structure were checked.
- [ ] Power Query refreshes without unexpected errors, when applicable.
- [ ] KPI and dashboard totals were validated, when applicable.
- [ ] No credentials, personal records, or confidential data are included.
- [ ] Binary-file changes are explained clearly.
- [ ] Screenshots or validation notes are included when useful.
- [ ] The contribution follows the Code of Conduct.

## Pull Request Description

A strong pull request description should include:

1. **Purpose** — what problem is being solved;
2. **Changes** — which files and behaviours changed;
3. **Validation** — how the result was checked;
4. **Screenshots** — when the report or visual layout changed; and
5. **Limitations** — anything reviewers should know.

## Security Reports

Do not use a public issue or pull request to disclose credentials, sensitive data, or exploitable security details. Follow [`SECURITY.md`](SECURITY.md) for responsible reporting.

## Review and Acceptance

A contribution may be revised or declined when it:

- breaks the documented folder structure without justification;
- introduces unsupported or misleading analysis;
- includes unsafe connections, secrets, or private data;
- cannot be reproduced or validated;
- creates unnecessary complexity; or
- falls outside the purpose of this repository.

Acceptance is based on project relevance, correctness, clarity, maintainability, and safety.

---

**Maintainer:** MUSA  
**Repository:** `samusa099/sales-data-a11`
