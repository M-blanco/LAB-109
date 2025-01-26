# Microglial Marker Analysis with Jupyter Notebook

This project provides a **Python-based Jupyter Notebook** designed to simplify and streamline the analysis of microglial marker data obtained from 3D microscopy using **IMARIS** software. 

IMARIS generates multiple CSV files for each marker in every image, creating an overwhelming number of files for comprehensive studies. This notebook automates the process of organizing, aggregating, and analyzing these datasets, saving time and reducing errors in data handling.

---

## Problem Overview

In typical experiments:
- **IMARIS generates** 2–4 CSV files for each image, depending on the number of amyloid plaques finded analyzed.
- **10 images per sample** result in 20–40 CSVs per sample.
- For a study with 10 samples, up to **400 CSV files** may be generated.
  
Manually combining these files for statistical analysis would be a **tedious and time-consuming process.**

---

## Key Features

This notebook addresses the problem by automating the following steps:

1. **File Aggregation**:
   - Scans the specified directory to identify and extract CSV files containing the selected marker (e.g., `IBA1`, `IB4`, `Evans Blue (EB)`).
   - Combines relevant data into a unified dataset.

2. **Data Summarization**:
   - Aggregates the surface values of different markers for each specific sample.

3. **Statistical Analysis**:
   - Performs correlation analysis between markers.
   - Tests for statistical differences between markers across different samples.

---

## Requirements

### Dependencies
- Libraries:
  - `pandas`: For data manipulation and aggregation.
  - `numpy`: For numerical operations.
  - `scipy`: For statistical tests.
  - `matplotlib`/`seaborn`: For visualizations (optional, if required for plotting).
