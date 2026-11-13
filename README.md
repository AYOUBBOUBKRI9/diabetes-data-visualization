# Diabetes Data Visualization & Exploratory Data Analysis

<p align="center">
  <strong>Exploratory Data Analysis | Data Cleaning | Statistical Visualization</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.x-blue?logo=python" />
  <img src="https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas" />
  <img src="https://img.shields.io/badge/NumPy-Scientific%20Computing-013243?logo=numpy" />
  <img src="https://img.shields.io/badge/Matplotlib-Visualization-11557c" />
  <img src="https://img.shields.io/badge/Seaborn-Statistical%20Visualization-4c72b0" />
  <img src="https://img.shields.io/badge/Google%20Colab-Notebook-orange?logo=googlecolab" />
</p>

---

## Project Overview

This project focuses on **Exploratory Data Analysis (EDA), data cleaning, preprocessing, and statistical data visualization** using Python.

The objective is to explore a diabetes-related dataset, identify data quality issues, clean and transform the data, and investigate relationships between different numerical and categorical variables.

The analysis is performed using Pandas, NumPy, Matplotlib, and Seaborn, with a total of 21 visualizations.

## Objectives

- Understand the structure and characteristics of the dataset.
- Identify missing values, duplicate records, and inconsistent data.
- Perform data cleaning and preprocessing.
- Convert variables into appropriate data types.
- Create new categorical features.
- Analyze numerical and categorical variables.
- Explore statistical relationships between variables.
- Build and interpret different types of visualizations.

## Technologies & Tools

| Technology | Purpose |
|---|---|
| Python | Main programming language |
| Pandas | Data manipulation and cleaning |
| NumPy | Numerical operations |
| Matplotlib | Data visualization |
| Seaborn | Statistical visualization |
| Google Colab | Development environment |
| Jupyter Notebook | Interactive analysis |

## Dataset Description

The dataset contains patient-related variables used to perform exploratory analysis.

**Original dataset:**
- 450 rows
- 12 columns

### Variables

| Variable | Description |
|---|---|
| `id` | Patient identifier |
| `age` | Patient age |
| `sexe` | Sex category |
| `imc` | Body Mass Index |
| `pa` | Blood pressure |
| `ct` | Total cholesterol |
| `ldl` | LDL cholesterol |
| `hdl` | HDL cholesterol |
| `ct_hdl` | Total cholesterol / HDL ratio |
| `ltg` | LTG variable |
| `glu` | GLU variable |
| `progression` | Progression indicator |

## Data Cleaning & Preprocessing

The initial dataset contained several intentional data quality issues.

The following operations were performed:

1. **Duplicate detection and removal**
   - Identified 8 duplicate records.
   - Removed duplicate rows.

2. **Data type correction**
   - Converted blood pressure (`pa`) into a numerical variable.
   - Converted `sexe` into a categorical variable.

3. **Missing value treatment**
   - Identified missing values in BMI and glucose.
   - Removed patients with missing age or BMI.
   - Replaced missing blood pressure values using the median (93).
   - Preserved missing values in glucose.

4. **Inconsistent value correction**
   - Identified 3 impossible age values.
   - Replaced inconsistent ages with missing values before filtering.

5. **Feature engineering**
   - Created `classe_age` to group patients into four age categories.
   - Created `categorie_imc` to classify BMI into three categories.

### Cleaning Results

| Indicator | Initial | Final |
|---|---:|---:|
| Number of rows | 450 | 427 |
| Number of columns | 12 | 14 |
| Duplicate records | 8 | 0 |
| Missing BMI values | 12 | 0 |
| Missing blood pressure values | 6 after conversion | 0 |

The final dataset contains **427 observations and 14 columns**.

## Exploratory Data Analysis & Visualization

A total of **21 visualizations** were developed using Matplotlib and Seaborn.

### 1. Matplotlib Visualizations

The first part focuses on fundamental visualization techniques:

- Line plot: Average BMI by age group.
- Bar chart: Number of patients by BMI category.
- Horizontal bar chart: Average HDL by BMI category.
- Stacked bar chart: Patients by age group and sex.
- 100% stacked bar chart: BMI category distribution by sex.
- Histogram: BMI distribution.
- Scatter plot: Total cholesterol versus LDL.
- Pie chart: BMI category proportions.
- Multiple histograms: BMI and blood pressure distributions.
- Box plot: Blood pressure by age group.

### 2. Seaborn Statistical Visualizations

The second part explores more advanced statistical visualizations:

- Line plot with 95% confidence intervals.
- Grouped bar plot.
- Count plot.
- Histogram with KDE.
- KDE density plot.
- Grouped box plots.
- Violin plot.
- Scatter plot with categorical encoding.
- Correlation heatmap.
- Pairplot.

### 3. Final Visualization

A combined figure was created to compare:
- BMI distribution using a histogram.
- BMI distribution by sex using box plots.

All 21 figures are available in the `figures/` directory.

## Key Findings

The exploratory analysis revealed several interesting patterns:

- Average BMI increases progressively across the first age groups.
- The BMI category below 25 is the most represented, with 182 patients.
- Average HDL decreases as BMI category increases.
- Total cholesterol and LDL show a strong positive visual relationship.
- BMI and blood pressure distributions can be compared across age groups and sex.

These observations describe the dataset and should not be interpreted as evidence of causality.

## Project Structure

```text
diabetes-data-visualization/
│
├── README.md
├── requirements.txt
│
├── data/
│   └── diabetes_brut.csv
│
├── notebooks/
│   └── Visualisation_Donnees_Diabetes.ipynb
│
├── reports/
│   └── Rapport_TP_Visualisation_Diabetes.pdf
│
└── figures/
    ├── D1.png
    ├── D2.png
    ├── D3.png
    ├── D4.png
    ├── D5.png
    ├── D6.png
    ├── D7.png
    ├── D8.png
    ├── D9.png
    ├── D10.png
    ├── D11.png
    ├── D12.png
    ├── D13.png
    ├── D14.png
    ├── D15.png
    ├── D16.png
    ├── D17.png
    ├── D18.png
    ├── D19.png
    ├── D20.png
    └── D21.png
```

## How to Run the Project

### 1. Clone the repository

```bash
git clone https://github.com/AYOUBBOUBKRI9/diabetes-data-visualization.git
```

### 2. Navigate to the project directory

```bash
cd diabetes-data-visualization
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Open the notebook

```bash
jupyter notebook
```

You can also open the notebook directly using Google Colab.

## Conclusion

This project provided practical experience in the complete exploratory data analysis workflow, from raw data inspection and preprocessing to statistical visualization and interpretation.

It strengthened my understanding of Python-based data analysis and demonstrated how visualization techniques can help identify patterns, distributions, and relationships within a dataset.

---

## Author

**Mohamed Ayoub Boubkri**

Master's Student in Computer Science  
Digital Governance & Digital Transformation  
Specialization: Digital Governance and Data Engineering

**Institution:** Faculty of Sciences, Rabat – Mohammed V University, Morocco.

**GitHub:** [@AYOUBBOUBKRI9](https://github.com/AYOUBBOUBKRI9)

---

<p align="center">
  <strong>Data Analysis | Python | Data Visualization | Exploratory Data Analysis</strong>
</p>
