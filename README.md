<h1 align="center">AutoEDA-Tool</h1>

<p align="center">
  <strong>R Shiny application for automated exploratory data analysis.</strong><br>
  Upload a CSV, inspect summaries, visualize distributions, detect outliers, review correlations, and explore data quality quickly.
</p>



<p align="center">
  <img alt="GitHub Repo stars" src="https://img.shields.io/github/stars/AjaySoni-Dev/AutoEDA-Tool?style=social">
  <img alt="GitHub forks" src="https://img.shields.io/github/forks/AjaySoni-Dev/AutoEDA-Tool?style=social">
</p>

<p align="center">
  <img alt="status: working prototype" src="https://img.shields.io/badge/status-working%20prototype-blue">
  <img alt="stack: R / Shiny" src="https://img.shields.io/badge/stack-R%20/%20Shiny-informational">
  <img alt="license: MIT" src="https://img.shields.io/badge/license-MIT-green">

</p>

<p align="center">
  <a href="#overview">Overview</a> ·
  <a href="#features">Features</a> ·
  <a href="#repository-structure">Repository Structure</a> ·
  <a href="#run-locally">Run Locally</a> ·
  <a href="#limitations">Limitations</a>
</p>

---

## Overview

**AutoEDA-Tool** is an interactive exploratory data analysis app built with **R Shiny**. It helps users upload a dataset and quickly inspect numerical summaries, missing values, outliers, distributions, and correlations.

The repository includes a working `script.R`, a sample `data.csv`, and one generated distribution image. The included sample dataset has **4,000 rows** and weather-related columns: `Temperature`, `Humidity`, `Air_Pressure`, `Wind_Speed`, and `Weather_Condition`.

## Features

- CSV upload through Shiny UI.
- Dataset preview and summary tables.
- Missing value inspection.
- Outlier detection helper logic.
- Distribution plots.
- Correlation analysis for numeric columns.
- Variable selection inputs.
- Example dataset included for quick testing.

## Repository Structure

| File | Purpose |
|---|---|
| `script.R` | Main R Shiny application containing UI, server logic, EDA helpers, plots, tables, and correlation workflow. |
| `data.csv` | Sample weather dataset for testing the application. |
| `distribution.jpg` | Example output/visual asset. |
| `README.md` | Original documentation. |
| `LICENSE` | MIT license. |

## Tech Stack

| Area | Tools |
|---|---|
| App framework | R Shiny |
| Visualization | ggplot2, base plotting |
| Data analysis | R data frames, summary functions, correlation logic |
| Input format | CSV |

## Run Locally

Install the required R packages:

```r
install.packages("shiny")
install.packages("ggplot2")
```

Run the app:

```r
shiny::runApp("script.R")
```

Or open `script.R` in RStudio and click **Run App**.

## Limitations

- The project is currently a single-file Shiny app.
- There is no packaged `renv.lock` or dependency lock file.
- File type support is focused on CSV.
- Advanced profiling, automated report export, and feature recommendation are not implemented yet.
- The UI is functional, but it can be polished for a more professional portfolio presentation.

## Recommended Improvements

- Add `renv` for reproducible R dependencies.
- Add screenshots to the README.
- Add downloadable EDA report export.
- Add categorical feature plots.
- Add cleaner modular structure with separate UI/server/helper files.
- Add better error handling for invalid or empty datasets.

## License

This project is licensed under the MIT License.
