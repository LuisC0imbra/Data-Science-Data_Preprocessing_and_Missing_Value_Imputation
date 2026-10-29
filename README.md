# Data Preprocessing and Missing Value Imputation

### Academic Data Science Project | Python | Data Cleaning | Statistical Analysis

**Final Grade: 16/20**

## Project Overview

This project was developed as part of my **Master's Degree in Data Analysis and Decision Support Systems** at **ISCAC - Coimbra Business School, Polytechnic Institute of Coimbra**.

The objective was to explore and compare different techniques for handling missing values in a real-world housing dataset, assessing how each method affects data completeness and the statistical characteristics of the dataset.

The project combines exploratory data analysis, statistical techniques, and machine learning-based imputation using Python.

## Dataset

The dataset contains residential property information from **King County, Washington (USA)**, covering transactions between May 2014 and May 2015.

| Characteristic | Description |
|---|---|
| Dataset size | 1,639 records |
| Number of variables | 12 |
| Domain | Real Estate |
| Main challenge | Missing values |
| Missing-value variables | `grade`, `sqft_basement`, `zipcode` |

**Dataset Availability:** The dataset (`dataset.csv`) was provided during our university classes for academic purposes and has not been publicly released. Therefore, it is not included in this repository.

## Project Objectives

- Identify and visualize missing values across the dataset.
- Analyze the distribution and characteristics of incomplete records.
- Apply different data deletion and imputation techniques.
- Compare the resulting datasets using descriptive statistics.
- Explore the use of regression and machine learning for missing-value estimation.
- Understand the advantages and limitations of each approach.

## Methodology

### 1. Exploratory Data Analysis

The initial analysis focused on understanding the dataset's structure, identifying missing values, and examining relationships between numerical variables.

Techniques included descriptive statistics, missing-value visualization, and correlation analysis.

### 2. Missing Data Removal

Two approaches were explored:

**Column Removal:** Removing variables containing missing values to obtain a simplified dataset.

**Listwise Deletion:** Removing observations with missing values in the relevant variables, producing a dataset containing 512 records.

An additional filtering approach was explored to retain observations with at least one available value among the selected variables, resulting in 1,617 records.

### 3. Statistical Imputation

**Median Imputation**

Missing numerical values were replaced using the median of the corresponding variable.

**Mode Imputation**

Missing values in the categorical `zipcode` variable were replaced using the most frequent category.

### 4. Regression-Based Imputation

Linear regression models were applied to estimate missing values using relationships between housing characteristics.

This approach explores whether information from other variables can provide reasonable estimates for incomplete observations.

### 5. K-Nearest Neighbors Imputation

KNN-based imputation was implemented using **5 nearest neighbors**, estimating missing numerical values from similar observations.

This approach was compared with the statistical and regression-based methods.

## Results and Key Findings

The comparison highlighted several important observations:

- Listwise deletion significantly reduced the available dataset, demonstrating the potential loss of information when incomplete records are removed.
- Median imputation offered a straightforward approach to preserving the dataset's size.
- KNN imputation produced descriptive statistical results relatively similar to median imputation.
- Regression-based imputation produced more noticeable differences in the resulting values.
- Different preprocessing strategies can influence the distribution and statistical properties of a dataset.

These comparisons were based primarily on descriptive statistics. They do not establish which imputation method is most accurate without additional validation against known values.

## Technologies Used

| Technology | Purpose |
|---|---|
| Python | Data processing and analysis |
| Pandas | Data manipulation and cleaning |
| NumPy | Numerical operations |
| Matplotlib | Data visualization |
| Seaborn | Statistical visualization |
| Scikit-learn | Linear regression and KNN imputation |
| Jupyter Notebook | Analysis and documentation |

## Repository Structure

```text
Data-Preprocessing-and-Missing-Value-Imputation/
│
├── notebook/
│   └── CECD_Data_Preprocessing_English_Portfolio.ipynb
│
├── documentation/
│   └── Data-Science-Data_Preprocessing_and_Missing_Value_Imputation.pdf
│
└── README.md
```

## How to Explore the Project

1. Open the notebook in the `notebooks/` directory.
2. Follow the exploratory analysis and missing-value identification.
3. Review the different deletion and imputation approaches.
4. Compare the statistical results produced by each method.
5. Consult the academic report in `docs/` for additional context.

**Note:** The original dataset is not publicly available. The notebook requires `dataset.csv` to reproduce the analysis.

## Academic Information

| Field | Details |
|---|---|
| Institution | ISCAC - Coimbra Business School |
| University | Polytechnic Institute of Coimbra |
| Degree | Master's in Data Analysis and Decision Support Systems |
| Project Type | Academic Group Project |
| Final Grade | **16/20** |
| Contributors | Luís Coimbra, Mário Simão, Ricardo Neto |

## Skills Demonstrated

- Data Cleaning and Preprocessing
- Exploratory Data Analysis (EDA)
- Missing Data Analysis
- Statistical Imputation
- Regression-Based Imputation
- K-Nearest Neighbors (KNN)
- Python Data Analysis
- Statistical Interpretation

## Final Considerations

This project provided practical experience with an essential stage of the Data Science workflow: **preparing incomplete datasets for reliable analysis**.

By implementing and comparing several missing-value handling techniques, the project reinforced the importance of selecting preprocessing strategies according to the characteristics of the data and the objectives of the analysis.

The work contributed to my foundations in Data Science, statistical analysis, and machine learning, which I continue to develop through professional and personal projects.
