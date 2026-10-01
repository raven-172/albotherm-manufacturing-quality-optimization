# Albotherm Quality Intelligence System

Predictive quality control system for Albotherm's Advanced sustainable cooling solution. Developed to optimize Albotherm's manufacturing Process.


## Table of Contents

- [About Albotherm](#about-albotherm)
- [Project Summary](#project-summary)
- [The Problem](#the-problem)
- [Team Members](#team-members)
- [Contribution Matrix](#contribution-matrix)
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Documentation](#documentation)
  - [Team Charter](#team-charter)
  - [Data Governance](#data-governance)

---

## About Albotherm

Albotherm is a chemical manufacturing company focused on developing innovative, sustainable temperature regulation technologies. Their work centres on advanced coating solutions that enable efficient temperature control across a range of applications — from greenhouses to commercial buildings — without requiring additional energy input. With a strong emphasis on tackling climate challenges, they aim to support more sustainable and energy-efficient industries.

## Project Summary

This project looks at data from a chemical manufacturing process to better understand what’s really going on behind the scenes. The goal is to explore how different inputs, process conditions, and material batches are connected, and to identify any patterns or trends that might not be obvious at first glance. By digging into the data, we hope to uncover insights that can help improve decision-making, optimise production, and ultimately support a more efficient and consistent manufacturing process for Albotherm.

### The Problem

Albotherms production run is inconsistent, with 83% of their experiments being fails. The aim is to have % dry of the product to be below 20% after 24 hours as well as 48 hours. Some experiments succeed in the 24 hour test, however, inconsistent changes occur in the 48 hour results. This means there is a drift problem that we have to solve as well.

#### Pipeline

##### How we went about solving this

- Data Cleaning
- Data Merging
- In Depth Analysis of Data
- Hypothesis Testing
- Creating a Machine Learning Model

#### Key Findings

UV chemical formulation is the primary driver of a good 24 hour result. Drifting is caused by process settings, so we worked on optimising the best process settings for experiment runs.

---

### Team Members

- Amir Hossein Mashhadi Zadeh
- Daud Sulaimon
- Hoang Viet Huy Le
- Lin Htet Moe Myint
- Ogbuchi Obinna Stanley

### Contribution Matrix

| Task | Daud | Leo | Lin | Obinna | Amir |
| ----- | ----- | ----- | ----- | ----- | ----- |
| Research & Report | 20 | 15 | 20 | 15 | 30 |
| Data Cleaning | 20 | 10 | 30 | 25 | 15 |
| Data Merging | 35 | 05 | 10 | 45 | 05 |
| Data Analysis | 35 | 05 | 15 | 15 | 30 |
| Hypothesis Testing | 05 | 45 | 15 | 05 | 30 |
| ML Model | 05 | 45 | 15 | 05 | 30 |
| Team Meetings | 20 | 15 | 35 | 20 | 10 |
| Total | 20 | 20 | 20 | 20 | 20 |

---

## Project Structure

```text
portfolio/
├── data/           # Raw and processed datasets used in the project
├── individual/     # Individual Reports
├── literature/     # Literature Review
├── notebooks/      # Jupyter notebooks for data cleaning, analysis and modeling
├── outputs/        # Output figures
├── project management/        # Meeting notes and documents showing the process of the project
├── report/         # Project report
├── .gitignore
├── README.md
└── requirements.txt
```

---

## Installation

```git bash
git clone https://gitlab.uwe.ac.uk/igp_sep25_team08/portfolio.git
cd portfolio
pip install -r requirements.txt
```

## Documentation

The [docs](<project management/docs/>) folder contains all supporting project documentation.

### Team Charter

[This link](./docs/Team_8_Charter.pdf) is to access the current team charter.

### Data Governance

In line with [Data Security Agreement](./docs/Data_Security_Agreement_Signed.pdf), all original Excel data files used in this project have been intentionally excluded from the repository. These datasets contain confidential information and are not permitted for public distribution.
