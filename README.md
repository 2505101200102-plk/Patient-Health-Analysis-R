# Patient Health Analysis Using R

## Student Details

**Student Name:** Palak Chavda  
**Enrollment Number:** 2505101200102

---

## Project Overview

This Tiny Project analyzes patient health records using **R** and follows the Practical 8–10 workflow.

The project demonstrates a complete data analysis process, including importing data, inspecting and cleaning the dataset, calculating statistical measures, creating visualizations, and analyzing correlations.

---

## Objectives

The main objectives of this project are:

- Import CSV data
- Inspect and clean the data
- Calculate statistical measures
- Create graphs and visualizations
- Analyze correlations between variables
- Analyze patient risk levels

---

## Dataset

The project uses the following dataset:

**`Palak_Chavda_Patient_Health.csv`**

The dataset contains the following fields:

| Column | Description |
|---|---|
| `Patient_ID` | Unique identification number of the patient |
| `Age` | Age of the patient |
| `Gender` | Gender of the patient |
| `BMI` | Body Mass Index |
| `Blood_Pressure` | Blood pressure value |
| `Cholesterol` | Cholesterol level |
| `Risk_Level` | Patient risk classification |

---

## Technologies Used

- **R Programming**
- **R Markdown**
- **HTML**
- **CSV Dataset**

---

## Analysis Performed

The following analysis is performed using R:

### 1. Data Import

The patient health dataset is imported from a CSV file using:

```r
health_data <- read.csv("Palak_Chavda_Patient_Health.csv")
```

### 2. Data Inspection

The structure and summary of the dataset are examined using:

```r
summary(health_data)
str(health_data)
```

### 3. Data Cleaning

Missing values and duplicate records are checked using:

```r
colSums(is.na(health_data))
sum(duplicated(health_data))
```

### 4. Statistical Analysis

The following statistical measures are calculated for BMI:

```r
mean(health_data$BMI)
median(health_data$BMI)
var(health_data$BMI)
sd(health_data$BMI)
```

### 5. Risk Level Analysis

Patient risk levels are analyzed using:

```r
risk_count <- table(health_data$Risk_Level)
```

### 6. Gender-wise BMI Analysis

Average BMI by gender is calculated using:

```r
aggregate(BMI ~ Gender, data=health_data, FUN=mean)
```

### 7. Correlation Analysis

The relationship between BMI and Blood Pressure is analyzed using:

```r
cor(health_data$BMI, health_data$Blood_Pressure)
```

---

## Key Findings

The analysis produced the following results:

- **Mean BMI:** 28.24
- **Median BMI:** 28.30
- **Standard Deviation:** 3.89
- **BMI/Blood Pressure Correlation:** 0.952

These values are obtained from the analysis performed in the project.

---

## Visualizations

The project includes graphical analysis such as:

- Risk Level Distribution
- BMI vs Blood Pressure

These visualizations help in understanding the distribution of patient risk levels and the relationship between BMI and Blood Pressure.

---

## Project Files

The repository contains the following files:

```text
Patient-Health-Analysis-R/
│
├── Palak_Chavda_Tiny_Project(1).Rmd
├── Palak_Chavda_Tiny_Project.html
├── Palak_Chavda_Patient_Health.csv
├── README.md
│
└── screenshots/
    ├── risk-level-distribution.png
    ├── bmi-vs-blood-pressure.png
    └── project-output.png
```

---

## How to Run the Project

### Step 1: Install R

Install R on your computer.

### Step 2: Open the R Markdown File

Open:

```text
Palak_Chavda_Tiny_Project(1).Rmd
```

using RStudio.

### Step 3: Keep the Dataset in the Same Folder

Make sure:

```text
Palak_Chavda_Patient_Health.csv
```

is located in the same project directory as the R Markdown file.

### Step 4: Run the R Markdown File

Open the `.Rmd` file in RStudio and run/knit the document to generate the HTML output.

The generated analysis can also be viewed directly using:

```text
Palak_Chavda_Tiny_Project.html
```

---

## Project Output

The HTML file contains:

- Project introduction
- Objectives
- R code
- Statistical analysis
- Graphical visualizations
- Findings
- Conclusion
- Complete dataset

---

## Conclusion

This project demonstrates a complete **R data-analysis workflow using healthcare data**. It covers data importing, inspection, cleaning, statistical analysis, visualization, and correlation analysis.

The project provides practical experience in using R for analyzing and interpreting patient health data.

---

## Author

**Palak Chavda**  
**Enrollment Number:** 2505101200102
