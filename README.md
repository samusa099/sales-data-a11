<div align="center">

# 📊 Sales Data Analysis — Assessment 11

**An Excel-to-Power BI sales analytics project for exploring order data and presenting business insights through an interactive report.**

[![Microsoft Excel](https://img.shields.io/badge/Data-Microsoft%20Excel-217346?style=for-the-badge&logo=microsoftexcel&logoColor=white)](https://github.com/samusa099/sales-data-a11/raw/main/Orders.xlsx)
[![Power BI](https://img.shields.io/badge/Dashboard-Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=000000)](https://github.com/samusa099/sales-data-a11/raw/main/eOrderid_powerbi.pbix)
[![Assessment Project](https://img.shields.io/badge/Project-Assessment%2011-6f42c1?style=for-the-badge&logo=github)](https://github.com/samusa099/sales-data-a11)

[![License](https://img.shields.io/github/license/samusa099/sales-data-a11?style=flat-square)](LICENSE)
[![Last Commit](https://img.shields.io/github/last-commit/samusa099/sales-data-a11?style=flat-square)](https://github.com/samusa099/sales-data-a11/commits/main)
[![Repository Size](https://img.shields.io/github/repo-size/samusa099/sales-data-a11?style=flat-square)](https://github.com/samusa099/sales-data-a11)
[![Security Policy](https://img.shields.io/badge/security-policy%20available-2ea44f?style=flat-square&logo=github)](SECURITY.md)

[Overview](#-project-overview) • [Files](#-repository-contents) • [Workflow](#-analytics-workflow) • [Usage](#-how-to-use) • [Security](#-security--file-safety) • [License](#-license)

</div>

---

## 🎯 Project Overview

This repository contains a compact sales analytics assessment that connects a source dataset in **Microsoft Excel** with a report developed in **Microsoft Power BI**.

The project demonstrates a practical analytics workflow:

- reviewing and organizing order-level sales data;
- preparing the dataset for reporting;
- building a Power BI data model and report;
- presenting sales information through clear, interactive visuals; and
- maintaining the supporting dataset, report file, documentation, security policy, and license in one repository.

> **Project type:** Data analytics assessment and portfolio project.

## 📁 Repository Contents

| File | Type | Purpose |
|---|---|---|
| [`Orders.xlsx`](Orders.xlsx) | Excel workbook | Source sales and order dataset used by the project. |
| [`eOrderid_powerbi.pbix`](eOrderid_powerbi.pbix) | Power BI report | Interactive report and analytics model built from the Excel dataset. |
| [`README.md`](README.md) | Documentation | Project overview, file guide, workflow, and usage instructions. |
| [`SECURITY.md`](SECURITY.md) | Security policy | Responsible disclosure, data privacy, and binary-file safety guidance. |
| [`LICENSE`](LICENSE) | MPL 2.0 | Terms governing use and distribution of the repository content. |

## 🔄 Analytics Workflow

```mermaid
flowchart LR
    A[Orders.xlsx<br/>Source Data] --> B[Data Review<br/>& Preparation]
    B --> C[Power BI<br/>Data Model]
    C --> D[Interactive<br/>Visual Analysis]
    D --> E[Business<br/>Interpretation]
```

## 🧰 Tools and Capabilities

| Area | Technology / Capability |
|---|---|
| Data source | Microsoft Excel (`.xlsx`) |
| Reporting | Microsoft Power BI Desktop (`.pbix`) |
| Data preparation | Data review, transformation, and model preparation |
| Analysis | Sales and order-level exploratory analysis |
| Visualization | Interactive charts, filters, and report views |
| Documentation | Markdown and GitHub repository documentation |

## 🚀 How to Use

### Option 1 — Download the complete repository

```bash
git clone https://github.com/samusa099/sales-data-a11.git
cd sales-data-a11
```

### Option 2 — Download the project files directly

- [⬇️ Download the Excel dataset](https://github.com/samusa099/sales-data-a11/raw/main/Orders.xlsx)
- [⬇️ Download the Power BI report](https://github.com/samusa099/sales-data-a11/raw/main/eOrderid_powerbi.pbix)

### Open and review the project

1. Open `Orders.xlsx` in Microsoft Excel to inspect the source data.
2. Open `eOrderid_powerbi.pbix` in Microsoft Power BI Desktop.
3. If Power BI cannot locate the workbook, update the data-source path to the downloaded `Orders.xlsx` file.
4. Refresh the report and use its visuals, filters, and report pages to explore the available sales information.

> Power BI files cannot be previewed directly on GitHub. Download the `.pbix` file and open it with **Power BI Desktop**.

## ✅ Recommended Review Checklist

- Confirm that column names and data types are consistent in `Orders.xlsx`.
- Check for blank, duplicate, or invalid order records before refreshing the report.
- Verify that the Power BI data-source path points to the correct local workbook.
- Refresh the model and confirm that all report visuals load correctly.
- Review filter interactions and totals before using the report for presentation or decision support.

## 🔐 Security & File Safety

This repository distributes binary Microsoft Excel and Power BI files. Download them only from the official repository and review their connections and embedded content before using them with confidential or production data.

### Security controls and expectations

| Area | Recommended action |
|---|---|
| Download source | Use only the official `samusa099/sales-data-a11` repository. |
| Excel workbook | Review formulas, named ranges, external links, and data connections before enabling refresh. |
| Power BI report | Review Power Query sources, data-source settings, refresh credentials, and custom visuals. |
| Credentials | Never commit or share passwords, tokens, gateway credentials, or connection strings. |
| Data privacy | Use synthetic, anonymized, or properly authorized data only. |
| Local protection | Keep Excel and Power BI Desktop updated and scan downloaded files with trusted security software. |
| Reporting | Do not publish sensitive vulnerability details in a public issue. |

### Before opening or refreshing

- verify that the file was downloaded from this repository;
- keep a backup before modifying the workbook or report;
- inspect external links and queries before approving access;
- avoid entering production credentials into a public or shared copy;
- do not replace sample data with confidential records unless the environment is properly secured.

### Reporting a security concern

Read the complete [`SECURITY.md`](SECURITY.md) policy for:

- supported repository versions;
- vulnerabilities that are in or out of scope;
- private and responsible reporting guidance;
- expected acknowledgement and triage targets;
- severity classification;
- coordinated disclosure and remediation practices.

**Do not publish credentials, personal records, private customer information, confidential company data, or exploit details in a public GitHub issue.** Use GitHub's private vulnerability reporting option from the repository **Security** tab when available.

## 📄 License

This project is distributed under the **Mozilla Public License 2.0**. See the [`LICENSE`](LICENSE) file for the complete terms.

## 👤 Author

**Siam Ahmad Musa**  
GitHub: [@samusa099](https://github.com/samusa099)

---

<div align="center">

**Built for practical sales analytics learning with Excel and Power BI.**

⭐ Star the repository if the project is useful to you.

</div>
