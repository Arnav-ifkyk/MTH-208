# 🇮🇳 India Health Dashboard

[![R](https://img.shields.io/badge/R-276DC3?style=for-the-badge&logo=r&logoColor=white)]()
[![Shiny](https://img.shields.io/badge/Shiny-316CE6?style=for-the-badge&logo=rstudio&logoColor=white)]()
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge)]()

Welcome to the **India Health Dashboard**, a sleek, dark-mode R Shiny web application designed to visualize critical health and mortality trends across India. Built with the `slate` theme for a premium, high-contrast look, this dashboard dives deep into state-level mortality causes, historical cancer trends, and self-harm statistics to make complex public health data immediately accessible and visually striking.

---

## ✨ Features

### 🗺️ State Cause Percentages (2021)
* Features a live-search dropdown menu to quickly select any Indian State or Union Territory.
* Displays dynamic, color-coded, and hover-animated tiles showing the percentage of total deaths for individuals aged 15–49 across both sexes.
* Tracks six major causes of death: Cardiovascular diseases, Neoplasms, Respiratory infections and tuberculosis, Nutritional deficiencies, Digestive diseases, and Diabetes and kidney diseases.

### 🎗️ Cancer Trends & Forecasting
* **Historical Trends (2017–2021):** Includes a multi-select checkbox input to compare death counts across various cancer types over time.
* **Mortality Forecast & Analysis:** Calculates and highlights the projected cancer mortality rate for the year 2025.
* Allows users to dynamically calculate the average annual change in mortality rates between custom-selected start and end years.
* Visualizes long-term cancer mortality projections from 1990 through 2050 using smooth `ggplot2` line graphs.

### 🧠 Self-Harm Deaths (2012–2021)
* Provides a year-by-year breakdown of self-harm fatalities.
* Features custom CSS-styled summary cards displaying exact male deaths, female deaths, and the male-to-female mortality ratio.
* Includes a dual-line trend plot comparing male and female self-harm deaths over a decade.

---

## 📊 Data & Architecture

This dashboard is built entirely in **R** and relies heavily on the `tidyverse` ecosystem. The application leverages robust datasets to generate its insights:

* `heat map pf states.csv`: Supplies state-level cause of death percentages for the year 2021.
* `Types of Cancer Deaths.csv`: Contains annual death counts for major cancer types in India from 2017 to 2021.
* `self harm.csv` & `Deaths Self Harm.csv`: Provides yearly self-harm death counts broken down by sex from 2012 to 2021.
* `Cancer Prediction India rate.csv`: Projects age-standardized cancer mortality rates under a "Reference" scenario.

---

## 🚀 Getting Started

### Prerequisites
Make sure you have R and RStudio installed on your machine. The required packages for this app include `shiny`, `ggplot2`, `dplyr`, `shinythemes`, `readr`, and `shinyWidgets`. 

You can install all required dependencies by running the following command in your R console:

```R
install.packages(c("shiny", "ggplot2", "dplyr", "shinythemes", "readr", "shinyWidgets"))
