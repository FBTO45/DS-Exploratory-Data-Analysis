# World Population Insights: Exploratory Data Analysis (EDA)

This repository contains my **Exploratory Data Analysis (EDA) Portfolio** presented at **Digital Skill Fair 39.0**. The analysis focuses on uncovering insights from global population data, identifying outliers, and setting the foundation for advanced modeling techniques.

---

## 📌 Project Overview

### **Objectives**
- Extract meaningful insights from world population data.
- Detect outliers and patterns in the dataset.
- Lay the groundwork for further analysis (clustering, predictive modeling, etc.).

### **Presentation File**
- **EDA Portfolio**: [`EDA_Portfolio.pptx`](./EDA_Portfolio.pptx)
- **Dataset**: `world_population2024.csv`

---

## 📊 Dataset Information

- **File:** `world_population2024.csv`
- **Size:** 216 rows × 12 columns
- **Key Features:**
  - `Rank`
  - `Country (or dependency)`
  - `Population (2024)`
  - `Yearly Change`
  - `Net Change`
  - `Density (P/km^2)`
  - `Land Area (Km^2)`
  - `Migrants (net)`
  - `Fert. Rate`
  - `Med. Age`
  - `Urban Pop %`
  - `World Share`

---

## 🔍 Data Exploration & Analysis

### **Libraries Used**
- `pandas`, `numpy`
- `matplotlib`, `seaborn`
- `sklearn` (PCA, StandardScaler)

### **Data Cleaning**
- No missing values.
- No duplicate entries.
- Dataset ready for analysis.

### **Outlier Detection**
- Outliers identified in:
  - `Yearly Change` (2.31% of total data)
  - `Fert. Rate` (2.31% of total data)
  - `World Share` (10.65% of total data)

### **Correlation Analysis**
- Strong negative correlation (-0.87) between `Fert. Rate` and `Med. Age`.

### **Principal Component Analysis (PCA)**
- First two components explain **71.26% of total variance**.
- Key variables influencing PCA: `Rank`, `Fert. Rate`, `Med. Age`, `Urban Pop %`, `World Share`.

---

## 📌 Recommendations & Next Steps

- Investigate outlier causes (data errors vs. real trends).
- Perform clustering (e.g., K-Means) to find population patterns.
- Build predictive models using insights from EDA.
- Apply dimensionality reduction (PCA) for data visualization.

---

## 🚀 Getting Started

### **Prerequisites**
Ensure you have:
- Python 3.x installed
- Required libraries:
  ```bash
  pip install pandas numpy matplotlib seaborn scikit-learn
