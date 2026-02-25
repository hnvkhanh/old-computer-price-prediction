# Old Computer Price Prediction

Predicting prices for used laptops and desktop computers based on scraped listings and structured features.

## Project Overview

This project explores how to estimate the resale price of old computers using real-world data collected from online listings. The workflow is organized in Jupyter notebooks that cover:

- Crawling raw listing data for desktops and laptops
- Cleaning and preprocessing the data
- Exploratory data analysis (EDA) and visualizations
- Training and evaluating machine learning models for price prediction

## Repository Structure

- [code/](code)
  - [code/crawl_data_desktop.ipynb](code/crawl_data_desktop.ipynb) – Crawl and collect desktop computer listing data.
  - [code/Crawl-Data-Laptop.ipynb](code/Crawl-Data-Laptop.ipynb) – Crawl and collect laptop listing data.
  - [code/Preprocessing.ipynb](code/Preprocessing.ipynb) – Data cleaning, feature engineering, and label encoding.
  - [code/EDA-Sơ-Bộ.ipynb](code/EDA-S%C6%A1-B%E1%BB%99.ipynb) – Initial exploratory data analysis.
  - [code/EDA-Visualization.ipynb](code/EDA-Visualization.ipynb) – Visual EDA: distributions, correlations, and key insights.
  - [code/ModelTraining.ipynb](code/ModelTraining.ipynb) – Model training, evaluation, and comparison for price prediction.

- [data/](data)
  - [data/data_laptop_price.csv](data/data_laptop_price.csv) – Raw laptop listing data.
  - [data/data_may_ban.csv](data/data_may_ban.csv) – Raw desktop/PC listing data.
  - [data/data_preprocessing .csv](data/data_preprocessing%20.csv) – Intermediate dataset after basic preprocessing.
  - [data/data_preprocessing_labelencoder.csv](data/data_preprocessing_labelencoder.csv) – Preprocessed dataset with label-encoded categorical features.
  - [data/final_data.csv](data/final_data.csv) – Final dataset used for model training.
  - [data/link_may_ban.csv](data/link_may_ban.csv) – Source links for desktop listings.
  - [data/links_200.txt](data/links_200.txt) – Sample list of listing URLs used during crawling.

## Notes

- Folder and file names are kept as originally used during experimentation; some are in Vietnamese.
- If you change the crawling logic or add new sources, regenerate the intermediate CSV files before rerunning preprocessing and training.
- For production use, consider exporting your final model (e.g., with `joblib`) and building a small API or UI around it.
