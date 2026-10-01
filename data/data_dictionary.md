# Albotherm Formulation & Testing Dataset Description Report

## Introduction

This document explains the Albotherm dataset. The dataset is made up of four Excel worksheets used during the Albotherm development project. The project focused on creating and testing a special coating system.

The dataset shows:

- the formulations that were created
- the materials used in those formulations
- the checks carried out on starting materials
- how experiments were set up and carried out
- how the finished product performed
- the estimated cost of the formulations

The dataset is currently in a messy state and needs cleaning before it can be used properly.

## Dataset Overview

The dataset contains four main worksheets:

- **AXF-1 data_DS_2026**
- **Durability Data**
- **Starting Material**
- **The Formulation Database**

The data covers the period from **24-07-2024 to 30-10-2025**.

## Main Data Problems

Some common issues were found in the dataset:

- missing values
- blank rows and columns
- duplicate entries
- poor data structure
- inconsistent date formats

These problems need to be fixed before analysis.

## Worksheet Descriptions

### 1. AXF-1 data_DS_2026

This is the experiment diary. It records what was used in each trial, the settings chosen, and how the process was carried out.

It contains three sheets:

- **Raw Data** – this is the main sheet. It contains the full experiment records, including experiment number, date, materials used, quantities used, viscosity results, equipment used, flow settings, curing conditions, UV power, and curing energy.
- **Pivot Table** – this sheet gives a summary of emulsion viscosity results. It helps show patterns without reading every row of the main data.
- **Cure Rig Key** – this sheet explains the different cure rig versions used during the process and how they were operated.

Main issues found in this worksheet include missing values and blank rows.

### 2. Durability Data

This worksheet records how the capsules behaved after production, especially under humidity conditions and over time.

It contains one sheet:

- **Initial Caps Durability** – this sheet includes batch number, formulation used, date of test setup, manufacturing notes, room temperature behaviour, coating compatibility, humidity results, visual observations, and the final quality control result.

Main issues found in this worksheet include missing values, blank rows, and duplicate entries.

### 3. Starting Material

This worksheet records the quality checks carried out on raw materials before they were used in experiments.

It contains three sheets:

- **Core QC** – this sheet records the checks carried out on core materials, including formulation name, batch number, date, quantity, viscosity, temperature, pass or fail result, and comments.
- **UV QC** – this sheet records the checks carried out on UV materials, including formulation name, batch number, date made, quantity, viscosity, curing result, pass or fail result, and comments.
- **Outer QC** – this sheet records the checks carried out on outer materials, including formulation name, batch number, date made, quantity, viscosity, pass or fail result, and comments.

Main issues found in this worksheet include missing values, blank rows, duplicate entries, and inconsistency in the **Old name** column in the Core QC sheet.

### 4. The Formulation Database

This worksheet contains the main formulation recipes, testing results, and cost information.

It contains five sheets:

- **UV Formulations** – this sheet records UV formulation details, including sample name, ingredients used, formulation properties, cure result, and moisture barrier information.
- **Core Formulation** – this sheet records core formulation details, including sample name, date, total amount, viscosity, LCST, refractive index, and other formulation values.
- **UV Testing** – this sheet records test results for UV samples, including viscosity and cure test results.
- **Core Testing** – this sheet records test results for core samples, including viscosity, transition temperature, refractive index, and osmolarity.
- **Formulations COG** – this is the cost sheet. It shows the best-case and worst-case cost estimates for UV and core formulations.

Main issues found in this worksheet include missing values, inconsistent dates, blank rows, duplicate entries, unclear short column names, and poor structure in the cost sheet.

## Cleaning Recommendations

Before analysis, the following steps are recommended:

- remove blank rows and blank columns
- check and resolve duplicate entries
- review and handle missing values
- Restructure the Formulations COG sheet into a standard table format
- replace short column names with full descriptions where needed
- restructure the Formulations COG sheet into a clearer table format
- review the Old name column in Core QC

## Conclusion

The Albotherm dataset is a useful record of the formulation process, starting material checks, experiment setup, product performance, and cost estimation.

However, the dataset needs a lot of cleaning before it can be used reliably. The main problems are missing values, duplicate entries, blank rows, inconsistent dates, and poor structure.

Once cleaned, the dataset will provide a clear record of the Albotherm formulation process.