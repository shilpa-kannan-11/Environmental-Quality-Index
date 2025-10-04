# Environmental Quality Index (EQI) for California Counties

**Last Updated: October 2025**

---

## 1. Project Objective

The purpose of this project is to develop an **Environmental Quality Index (EQI)** that quantifies the environmental vulnerability of communities within California through comparing trends between datasets on pollution and green spaces against demographic and public health data from the CDC. 

---

## 2. Data Sources

The following datasets were downloaded on **October 3, 2025**.

* **Health Outcomes:** [CDC PLACES - County-level Data, 2024 Release](https://data.cdc.gov/500-Cities-Places/PLACES-Local-Data-for-Better-Health-County-Data-20/swc5-untb/about_data)
    * *File:* `cdc_places_county_california_2024.csv`
* **Air Quality:** [EPA Annual AQI by County, 2024](https://aqs.epa.gov/aqsweb/airdata/download_files.html)
    * *File:* `epa_aqi_county_usa_2024.csv`
* **Demographics:** [U.S. Census Bureau - ACS 1-Year Estimates, Table DP03, 2024](https://data.census.gov/table?q=DP03)
    * *Files:* `census_economic_county_california_2024.csv` and `census_economic_county_california_2024_column_metadata.csv`

---

## 3. Methodology

The analysis will be conducted using Python and the following key steps:

1.  **Data Acquisition & Cleaning:** Sourcing and preprocessing datasets to handle missing values and ensure consistent formatting.
2.  **Feature Engineering:** Calculating new, meaningful variables from the raw data.
3.  **Data Standardization:** Scaling all variables to have a mean of 0 and a standard deviation of 1, a prerequisite for PCA.
4.  **Principal Component Analysis (PCA):** Applying PCA to the environmental variables to identify the primary factors contributing to environmental vulnerability.
5.  **Index Calculation & Validation:** Using the PCA results to calculate a final EQI score for each county and analyzing the relationship between the EQI and health outcomes.

---

## 4. Planned Visualizations

* A **choropleth map** of the United States displaying the final EQI score for each county.
* A **scree plot** to justify the number of principal components selected.
* A **scatter plot** with a regression line showing the correlation between the EQI and a selected health outcome. 

---

## 5. Technologies Used

* **Language:** Python
* **Libraries:**
    * `pandas` for data manipulation
    * `geopandas` for geographic data processing
    * `scikit-learn` for PCA and data scaling
    * `matplotlib` / `seaborn` / `plotly` for visualizations
    * `Jupyter Notebook` for exploratory analysis

---

## 6. How to Run This Project

*(Instructions will be added upon project completion.)*