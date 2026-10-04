# disease-mapping-direct-travel
Data and R code for BSc (Hons) Research Report: The effect of including direct-travel neighbours in hierarchical Bayesian models for disease mapping
---

## 📁 Repository Contents

* **`DISEASE MAPPING.Rmd`**: R Markdown script containing data processing, spatial graph construction, BYM2 model implementations, and visualization code.
* **`covid_data.xlsx`**: Primary dataset containing state-level COVID-19 hospitalisations, population counts, vaccination rates, and covariates.
* **`LICENSE`**: Repository license.
* **`README.md`**: Project documentation and replication guidelines.

---

## 📊 Data Construction & Source Links

The aggregated dataset **`covid_data.xlsx`** was constructed using three public data sources:

1. **U.S. COVID-19 Hospitalisation Data (2024)**
   * **Description**: State-level count of adult hospitalised confirmed COVID-19 cases.
   * **Source**: U.S. Department of Health and Human Services (HHS)
   * **Link**: [HealthData.gov - COVID-19 Reported Patient Impact and Hospital Capacity](https://healthdata.gov/Hospital/COVID-19-Reported-Patient-Impact-and-Hospital-Capa/9psv-r5iz/about_data)

2. **U.S. Census & Spatial Covariates (2024)**
   * **Description**: State populations and demographic covariates.
   * **Source**: IPUMS National Historical Geographic Information System (NHGIS)
   * **Link**: [IPUMS NHGIS Data Repository](http://doi.org/10.18128/D050.V21.0)

3. **COVID-19 Vaccination Rates (2024)**
   * **Description**: State-level vaccination coverage among adults 18 years and older.
   * **Source**: CDC National Immunization Survey-Fall Respiratory Virus Module (NIS-FRVM)
   * **Link**: [CDC COVID-19 Vaccination Coverage Data](https://data.cdc.gov/Vaccinations/COVID-19-Vaccination-Coverage-Overall-and-by-Selec/ksfb-ug5d)

---
🚀 Reproduction Steps
1. Clone or download this repository to your computer.

2. Ensure covid_data.xlsx and DISEASE MAPPING.Rmd are located in your active R working directory.

3. Open DISEASE MAPPING.Rmd in RStudio.

4. Run all code chunks or click Knit to run the spatial models and generate the report outputs.

---

## 🛠️ Software Requirements & Dependencies

To execute the code, install R along with the required packages below:

```R
# 1. Install required packages from CRAN
install.packages(c("readxl", "dplyr", "tidyr", "ggplot2", "sf", "spdep", "knitr"))

# 2. Install R-INLA from the official repository
install.packages("INLA", repos = c(getOption("repos"), INLA = "[https://inla.r-inla-download.org/R/stable](https://inla.r-inla-download.org/R/stable)"), dep = TRUE)
'''

