# 📘 How to Use This Sales Analytics Project

This guide explains how to use **Sales Data Analysis — Assessment 11** safely and effectively for Excel review, Power Query practice, Power BI modelling, dashboard validation, portfolio development, and business analysis.

> **Main project files**
>
> - Dataset: [`data/raw/Orders.xlsx`](../data/raw/Orders.xlsx)
> - Power BI report: [`reports/power-bi/eOrderid_powerbi.pbix`](../reports/power-bi/eOrderid_powerbi.pbix)

---

## 📁 Project Structure

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
│   │   └── sales-data-cover.svg
│   └── preview/
│       └── project-preview.svg
├── README.md
├── SECURITY.md
└── LICENSE
```

### Why this structure is used

| Folder | Purpose |
|---|---|
| `data/raw/` | Keeps the original source workbook separate from reports and documentation. |
| `reports/power-bi/` | Contains the editable Power BI project file. |
| `docs/` | Stores detailed usage documentation without crowding the root directory. |
| `assets/cover/` | Stores repository cover visuals. |
| `assets/preview/` | Stores project-preview visuals used in the README. |
| Repository root | Retains only GitHub-standard files: README, security policy, and license. |

---

## 📌 What This Project Is For

| Use case | How the project helps |
|---|---|
| Excel data review | Check headers, formats, blanks, duplicates, invalid dates, and inconsistent values. |
| Data cleaning | Standardise text, dates, numeric fields, and categories before reporting. |
| Power Query practice | Import the workbook and build repeatable transformation steps. |
| Power BI modelling | Review relationships, measures, calculated logic, and filter context. |
| Dashboard development | Improve KPI cards, charts, slicers, navigation, and usability. |
| Sales analysis | Explore order volume, trends, product or customer performance, and other available dimensions. |
| Portfolio presentation | Demonstrate an organised Excel-to-Power BI analytics workflow. |
| Assessment practice | Rebuild, validate, explain, or extend the project. |
| Scenario testing | Replace the source rows with a structurally compatible dataset and test refresh behaviour. |

> The exact analysis available depends on the columns contained in `Orders.xlsx`.

---

## 🧰 Requirements

Prepare the following before starting:

- Microsoft Excel or another trusted application that supports `.xlsx` files;
- Microsoft Power BI Desktop for the `.pbix` report;
- enough local storage for a working copy and backup;
- trusted security software for scanning downloaded files; and
- optional Git, when cloning the repository.

---

## 🚀 Quick Start

### Method 1 — Clone the repository

```bash
git clone https://github.com/samusa099/sales-data-a11.git
cd sales-data-a11
```

### Method 2 — Download the project files directly

- [Download `Orders.xlsx`](https://github.com/samusa099/sales-data-a11/raw/main/data/raw/Orders.xlsx)
- [Download `eOrderid_powerbi.pbix`](https://github.com/samusa099/sales-data-a11/raw/main/reports/power-bi/eOrderid_powerbi.pbix)

### Recommended local working setup

The repository separates files by purpose. For day-to-day work, you may copy the two main files into one private working folder:

```text
sales-analysis-working-copy/
├── Orders.xlsx
└── eOrderid_powerbi.pbix
```

Keeping the workbook and PBIX file together makes local source-path management easier while preserving the clean repository structure.

---

## 🔄 Recommended Workflow

```mermaid
flowchart LR
    A[Download & Backup] --> B[Review & Clean Excel]
    B --> C[Connect & Refresh Power BI]
    C --> D[Validate KPIs & Visuals]
    D --> E[Analyse & Present]
```

---

## 1️⃣ Review the Excel Dataset

Open `data/raw/Orders.xlsx` before refreshing the Power BI report.

### Check the workbook structure

Confirm that:

- the intended data sheet is present;
- column headers are unique and meaningful;
- each row represents the expected level of detail;
- no merged cells interrupt the main data table;
- dates are stored as valid dates;
- quantities and monetary fields are numeric;
- categories use consistent spelling; and
- formulas, external links, hidden content, and named ranges are understood.

### Data-quality checks

| Check | What to look for | Recommended action |
|---|---|---|
| Blank records | Empty rows or required fields | Remove or investigate them. |
| Duplicate records | Repeated IDs or identical rows | Confirm whether they are genuine. |
| Invalid dates | Text dates, impossible dates, mixed formats | Convert to one consistent date type. |
| Numeric errors | Numbers stored as text or mixed with symbols | Clean and convert the field. |
| Category inconsistency | Different spellings, casing, or extra spaces | Standardise the values. |
| Missing identifiers | Records without expected keys | Correct, exclude, or document them. |
| Outliers | Unusually high, low, or negative values | Validate before keeping or removing them. |

### Preserve the source schema

The PBIX report may depend on the current sheet, table, and column names. Before structural changes:

1. create a backup;
2. record the existing schema;
3. inspect Power Query dependencies;
4. change one element at a time; and
5. refresh and validate after every change.

---

## 2️⃣ Open and Connect the Power BI Report

Open `reports/power-bi/eOrderid_powerbi.pbix` in Power BI Desktop.

### When the Excel source is found automatically

1. Select **Home → Refresh**.
2. Wait for Power Query and the data model to finish loading.
3. Review every report page for errors or blank visuals.
4. Compare important totals with the Excel source.

### When Power BI cannot find `Orders.xlsx`

1. Open **File → Options and settings → Data source settings**.
2. Select the Excel source used by the report.
3. Choose **Change Source**.
4. Browse to your local working copy of `Orders.xlsx`.
5. Confirm the path.
6. Select **Home → Refresh**.

If the source still fails, open **Transform data** and inspect the first Power Query step, normally named `Source`.

---

## 3️⃣ Review Power Query

Open **Home → Transform data** and inspect:

- source file path;
- selected sheet or table;
- promoted headers;
- assigned data types;
- removed or renamed columns;
- replaced values;
- filtered rows;
- merged or appended queries;
- custom columns; and
- error-handling steps.

Use descriptive step names such as:

```text
Source
Selected Orders Table
Promoted Headers
Assigned Data Types
Removed Blank Orders
Standardised Categories
Validated Numeric Fields
```

---

## 4️⃣ Validate the Data Model

In **Model view**, check:

- all expected tables are loaded;
- relationships are active and correctly directed;
- key fields do not contain unintended duplicates or blanks;
- date analysis uses a valid date field or date table;
- numeric fields use appropriate summarisation;
- technical fields are hidden where appropriate; and
- measures have clear names and definitions.

Avoid unnecessary calculated columns when a measure or Power Query transformation is more suitable.

---

## 5️⃣ Validate the Dashboard

### Visual validation

- KPI cards match the source data.
- Chart totals agree with validated Excel summaries.
- Slicers filter the expected visuals.
- Cross-filtering behaves logically.
- Titles describe the metric and context clearly.
- Units and number formats are consistent.
- Blank and error states are handled cleanly.
- Visuals remain readable at normal screen size.

### Business validation

For every KPI, document:

- business definition;
- source fields;
- aggregation method;
- included and excluded records;
- date logic;
- treatment of blanks, returns, or cancellations; and
- assumptions or limitations.

---

## 📊 Analysis Ideas

Depending on the available fields, review:

- sales performance over time;
- strongest and weakest periods;
- order count and average order value;
- high-value or unusual orders;
- product or category performance;
- customer concentration and repeat ordering;
- regional, branch, or channel performance; and
- data-quality and operational-control gaps.

Do not make claims that the validated source fields cannot support.

---

## ♻️ Replacing the Sample Data

Use a structurally compatible dataset only.

1. Copy the repository or create a private working folder.
2. Keep the expected workbook, sheet, table, and column names initially.
3. Replace only the source rows.
4. Confirm that data types remain compatible.
5. Refresh the PBIX report.
6. Inspect Power Query errors.
7. Validate relationships, measures, filters, and totals.
8. Save the reused version under a new project name.

When columns differ, update Power Query steps, relationships, DAX, visuals, slicers, and documentation carefully.

---

## 🔐 Safe Usage

Before opening or refreshing the files:

- download only from the official repository;
- scan downloaded files with trusted security software;
- review Excel formulas, links, and connections;
- review Power BI sources, custom visuals, and credentials;
- never store production passwords or tokens in the project;
- do not commit private customer or company data; and
- read the full [`SECURITY.md`](../SECURITY.md) policy.

---

## 🛠️ Troubleshooting

| Problem | Likely cause | Recommended fix |
|---|---|---|
| Power BI cannot find the workbook | Local source path changed | Update the source through Data source settings. |
| Refresh returns column errors | Columns were renamed, removed, or changed | Restore the schema or update Power Query. |
| Numbers do not match Excel | Filters, data types, or aggregation logic differ | Compare rows, measures, filters, and exclusions. |
| Dates do not group correctly | Invalid date type or missing date structure | Convert the field to Date and review date modelling. |
| A visual is blank | Filter context, relationship, or missing-data issue | Clear filters and inspect fields and relationships. |
| Power Query shows errors | Invalid values or incompatible transformations | Inspect the first failing step. |
| GitHub cannot preview the PBIX file | `.pbix` is a binary Power BI file | Download it and open it in Power BI Desktop. |

---

## ✅ Final Review Checklist

- [ ] Source workbook is backed up.
- [ ] Required fields have been checked for blanks and duplicates.
- [ ] Data types are correct.
- [ ] Power BI connects to the intended workbook.
- [ ] All queries refresh without errors.
- [ ] Relationships are valid.
- [ ] KPI definitions are documented.
- [ ] Dashboard totals match validated source calculations.
- [ ] Filters and interactions work correctly.
- [ ] No credentials or confidential records are included.
- [ ] File paths and documentation are current.

---

## 👤 Author

**MUSA**  
*HR Professional • Data Analytics Practitioner*  
Building practical, business-focused insights with Excel and Power BI.
