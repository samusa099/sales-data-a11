# 🔐 Security Policy

Thank you for helping keep **Sales Data Analysis — Assessment 11** and its users safe.

This repository contains downloadable Microsoft Excel and Power BI files. Security reports are therefore especially relevant when they involve sensitive data exposure, unsafe external connections, malicious formulas or content, embedded credentials, or tampering with the distributed project files.

## Supported Versions

This project does not currently publish numbered software releases. Security maintenance follows the active repository state shown below.

| Repository state | Security support |
|---|---|
| Latest commit on `main` | ✅ Supported |
| Current files linked from `README.md` | ✅ Supported |
| Older commits, forks, or modified copies | ❌ Not supported |
| Files downloaded from unofficial mirrors | ❌ Not supported |

Security fixes, when required, will be applied to the latest version on the `main` branch.

## Security Scope

### In scope

Please report concerns involving:

- exposed passwords, access tokens, API keys, connection strings, or credentials;
- personal, customer, employee, financial, or other confidential information unintentionally included in the dataset or report;
- unsafe external links, queries, gateways, connectors, or data-source references in `Orders.xlsx` or `eOrderid_powerbi.pbix`;
- malicious or unexpected formulas, scripts, commands, custom visuals, or embedded content;
- spreadsheet formula injection or content that could execute unexpectedly after export or reuse;
- manipulated project files, misleading download links, or repository content tampering;
- a security issue in repository automation, documentation, or future source code;
- instructions that could cause users to disclose credentials or private business data.

### Usually out of scope

The following are normally not security vulnerabilities unless they create a confidentiality, integrity, or execution risk:

- incorrect totals, chart formatting, or analytical interpretation;
- ordinary data-quality issues such as blanks, duplicates, or inconsistent labels;
- feature requests or report-design preferences;
- vulnerabilities that exist only in unsupported third-party software;
- issues affecting a modified fork but not the official `main` branch;
- reports without a reproducible security impact.

## Reporting a Vulnerability

**Do not disclose sensitive vulnerability details in a public GitHub issue.**

Use GitHub's private vulnerability reporting option from the repository's **Security** tab when it is available. Include enough information to reproduce and assess the issue safely.

A useful report should contain:

1. a clear description of the vulnerability;
2. the affected file, report page, query, connection, formula, or repository path;
3. the commit SHA or download date;
4. reproducible steps or a minimal proof of concept;
5. the expected and observed behavior;
6. the potential confidentiality, integrity, or execution impact;
7. screenshots or sanitized evidence, where useful; and
8. suggested remediation, if known.

If private reporting is unavailable, open a public issue containing **only a request for a private contact channel**. Do not include credentials, private records, exploit details, or confidential screenshots in that issue.

## What Not to Include

Please do not send or publish:

- live credentials or authentication tokens;
- real customer, employee, applicant, payroll, banking, or tax information;
- confidential company datasets;
- malware or weaponized payloads beyond what is strictly necessary to demonstrate the issue;
- data belonging to another person or organization without authorization.

Use synthetic, redacted, or minimized evidence wherever possible.

## Response Targets

The following are good-faith response targets, not contractual service-level guarantees:

| Stage | Target |
|---|---|
| Initial acknowledgement | Within 3 business days |
| Preliminary triage | Within 7 business days |
| Status update | At least every 14 days while open |
| Remediation | Based on severity, complexity, and user impact |

A report may be accepted, declined, or returned for more information. Duplicate or non-security reports may be closed with an explanation.

## Severity Guidance

| Severity | Example impact | Typical priority |
|---|---|---|
| Critical | Active credential exposure, arbitrary code execution, or highly sensitive data disclosure | Immediate containment |
| High | Significant confidential data exposure or unsafe executable content | Urgent remediation |
| Medium | Limited data exposure, unsafe connection behavior, or integrity risk requiring user interaction | Planned remediation |
| Low | Minor hardening gap with limited practical impact | Maintenance backlog |

Final severity may differ from the reporter's assessment after reproduction and impact analysis.

## Safe Download and Usage Guidance

Because this repository distributes binary analytics files, users should follow these precautions:

- download files only from the official repository;
- keep Microsoft Excel and Power BI Desktop updated;
- scan downloaded files with trusted security software;
- inspect Excel formulas, named ranges, external links, and data connections before enabling refresh;
- inspect Power Query sources, Power BI data-source settings, custom visuals, and refresh credentials;
- do not enter production credentials into a public or shared copy of the report;
- do not replace the sample dataset with confidential data unless the working environment is properly secured;
- verify file names and repository links before opening downloaded content;
- maintain a backup before modifying the source workbook or Power BI model.

## Data Privacy Expectations

This repository is intended for learning, assessment, and portfolio demonstration. Contributions and examples should use synthetic, anonymized, or properly authorized data.

Do not commit:

- personally identifiable information;
- confidential sales or customer records;
- payroll, banking, tax, health, or identity documents;
- private email addresses or phone numbers;
- passwords, tokens, secrets, or internal connection details.

If sensitive information is committed accidentally, removing it from the latest file is not always sufficient because it may remain in Git history. Treat the incident as a security report and rotate any exposed credentials immediately.

## Coordinated Disclosure

Please allow reasonable time to investigate and remediate a confirmed vulnerability before public disclosure. Public acknowledgement may be provided when appropriate, unless the reporter requests anonymity.

Do not exploit a vulnerability beyond the minimum testing necessary to demonstrate impact, and do not access, modify, retain, or distribute data that you are not authorized to use.

## Security Fixes

A confirmed issue may be addressed through one or more of the following actions:

- replacing or sanitizing an affected workbook or Power BI file;
- removing unsafe external connections or embedded content;
- rotating exposed credentials;
- updating documentation and download guidance;
- removing compromised artifacts from the current branch;
- publishing a corrective commit, advisory, or release note;
- recommending that users delete and re-download affected files.

## No Bug Bounty

This is an educational and portfolio repository. No monetary bug-bounty program is currently offered. Responsible reports are still appreciated and will be reviewed in good faith.

## Attribution

Researchers who submit valid reports may be acknowledged in project documentation, subject to their consent and the sensitivity of the issue.

---

**Repository:** `samusa099/sales-data-a11`  
**Maintainer:** [@samusa099](https://github.com/samusa099)  
**Policy applies to:** the latest official files on the `main` branch
