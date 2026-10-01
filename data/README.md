# Data Folder

This folder contains the data that runs through every notebook in this project.
It is organised into three places: raw, processed, and a description of what
everything means. You can start from anywhere, but this page will help you understand
how the pieces fit together.

---

## Contents

[Data Description](<Data Description/data_dictionary.md>) documents every feature and column in the dataset; where it came from, what it measures, and what quality issues were found in it. It is a good place to start if you want to understand the data before looking at any of the files themselves.

[The raw folder](<raw/>) contains the original source files exactly as we received them from Albotherm. Nothing has been changed. They are kept this way intentionally, so there is always a clean record of where everything began.

[The processed folder](<processed/>) contains the cleaned and merged files that the analysis notebooks actually use. If you want to reproduce the results, this is where to look.

---

## Processing of the Data

Albotherm shared four Excel workbooks with us, produced internally between July 2024 and October 2025.

| Workbook | What it contains |
| --- | --- |
| **AXF-1 data_DS_2026** | The experiment file containing every production run, every process setting, every material quantity |
| **Durability Data** | The QC record containing humidity test results, visual observations, pass and fail outcomes |
| **Starting Material** | Starting quality checks on core, UV, and outer phase materials |
| **The Formulation Database** | The recipes, ingredient concentrations, formulation properties |

The data arrived messy with missing values, duplicate rows, inconsistent dates, column names that only made sense to the person who wrote them. We cleaned each source independently, then merged them on shared identifiers such as batch key, formulation code, material batch ID.

That produced a single unified frame `axf_merged.csv` which has **770 rows and 45 columns**, covering **612 unique AXF production runs**.

For the analysis and modelling stages, we trimmed that further. Columns with more than 50% missing values were dropped, they were post run observations recorded alongside the durability test, not formulation inputs, and keeping them would have introduced data leakage. Runs with no durability
result were excluded from the modelling, leaving **619 rows** that form the foundation of everything in notebooks (Analysis and Modelling).

---

## The processed files

| File | Description |
| --- | --- |
| `axf_merged.csv` | Full merged dataset — 770 rows × 45 columns |
| `axf_eda.csv` | Analysis-ready subset — 619 rows × 38 columns |
| `uv_cleaned.csv` | UV formulation ingredient lookup table |
| `core_cleaned.csv` | Core formulation ingredient lookup table |

The full cleaning and merging process is documented step by step
in `notebooks` folder.
