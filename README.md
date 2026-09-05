# NYC Airbnb Safety & Crime Heatmap Analytics 🗺️

> **Interactive Visual Analytics Dashboard for NYC Accommodation Safety & Neighborhood Risk Assessment**

An interactive visual analytics platform developed for Georgia Tech's **CSE6242: Data and Visual Analytics**. The application combines Airbnb listing data across New York City with historical NYPD crime incident reports to help prospective travelers assess safety and price trade-offs across boroughs.

---

## 📋 Overview

### The Problem
When booking short-term accommodations on platforms like Airbnb, travelers can compare price, ratings, and amenities, but have little visibility into local neighborhood safety metrics or historical crime distributions.

### The Solution
This project correlates NYC Airbnb listing coordinates and pricing data with NYPD historical crime incident datasets (categorized by offense severity: Felony, Misdemeanor, and Violation). Using D3.js and Google Maps visual layers, users can explore interactive safety heatmaps, toggle crime severity filters, and view localized risk metrics before making lodging decisions.

---

## ✨ Key Features

- **🗺️ Multi-Layer Crime Heatmap**: Visualizes geospatial crime density across New York City boroughs (Manhattan, Brooklyn, Queens, Bronx, Staten Island).
- **⚖️ Severity-Based Filtering**: Dynamic toggling between major crime categories:
  - *Felony* (high-severity offenses)
  - *Misdemeanor* (moderate-severity offenses)
  - *Violation* (minor infractions)
- **📍 Airbnb Accommodation Overlay**: Pinpoints lodging options alongside weighted risk scores.
- **📊 Data Analysis & Preprocessing Pipeline**: Jupyter notebooks executing spatial data cleaning, classification, and aggregation.

---

## 💻 Tech Stack

- **Frontend & Visualization**: D3.js, Google Maps JavaScript API, jQuery, Bootstrap, Materialize CSS
- **Data Engineering**: Python, Pandas, Jupyter Notebook
- **Datasets**: NYPD Historic Crime Incident Data & Inside Airbnb NYC dataset

---

## ⚡ Quick Start

### 1. Installation

Clone the repository:
```bash
git clone https://github.com/imanandvardhan/CSE6242_Project.git
cd CSE6242_Project
```

### 2. Local Execution

1. Open `html/index.html` in any modern web browser.
2. *(Optional)* If the Google Maps tile layer fails to load, supply your own [Google Maps JavaScript API key](https://developers.google.com/maps/documentation/javascript/get-api-key) in the script tag within `html/index.html`.

---

## 📂 Project Structure

```
CSE6242_Project/
├── airbnb_data/               # Preprocessed NYC Airbnb accommodation CSV datasets
├── crime_data/                # Filtered NYPD crime incident records (Felony, Misdemeanor, Violation)
├── crime_heatmap_bylevel/     # Geospatial HTML heatmaps and toggle implementations
├── data_analysis/             # Python Jupyter notebooks for clustering & data preparation
├── html/                      # Web dashboard entry point (index.html)
└── README.md
```

---

## 📜 Attribution & Academic Context

This project was developed as part of **CSE6242 / CX4242 Data and Visual Analytics** coursework. Historical data sources courtesy of NYC Open Data (NYPD) and Inside Airbnb.
