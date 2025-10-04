# Environmental Quality Index (EQI) for U.S. Counties

**Last Updated: October 2025**

---

## 1. Project Objective

The purpose of this project is to develop an **Environmental Quality Index (EQI)** that quantifies the environmental vulnerability of communities within the U.S. through comparing trends between datasets on pollution and green spaces against demographic and public health data from the CDC. 

---

## 2. Data Sources

The following datasets will be used to construct the index. 

* **Health Outcomes:** CDC PLACES - County-level data.
* **Air Quality:** EPA AirData - Annual summary data for PM2.5.
* **Pollution Sites:** EPA Superfund Enterprise Management System (SEMS) - Location data for hazardous waste sites.
* **Green Space:** Satellite-derived Normalized Difference Vegetation Index (NDVI) from Google Earth Engine (using Landsat 8/Sentinel-2 imagery).
* **Demographics:** U.S. Census Bureau - Data on median income and population density.

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