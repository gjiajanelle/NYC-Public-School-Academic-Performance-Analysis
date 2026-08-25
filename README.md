# 🏫 NYC Public School Academic Performance Analysis

An exploratory data analysis (EDA) project investigating standardized test performance across New York City public schools using Python and pandas 📊.

---

## 📌 Overview

This project analyzes NYC public school SAT results alongside geographic and demographic data to identify key performance trends, top-performing institutions, and borough-level variations 🏙️.

### 🎯 Key Objectives
* 📐 Identify schools with the highest math performance (SAT math score $\ge 640$ / 800).
* 🏆 Rank the top 10 public schools based on combined average SAT scores (Math, Reading, and Writing).
* 📍 Analyze borough-level academic performance to identify the borough with the highest variability (standard deviation) in SAT scores.

---

## 📁 Project Structure

```text
├── project-exploring-nyc-public-school-test-results_.ipynb      # Main Jupyter Notebook containing analysis and code
├── schools.csv         # Dataset containing NYC public school SAT scores
├── schoolbus.jpg       # Asset / cover image
└── README.md           # Project documentation
```

---

## 🗃️ Dataset Description

The analysis uses `schools.csv`, which contains school-level SAT examination results across New York City:

| Column Name | Type | Description |
| :--- | :--- | :--- |
| `school_name` | string | Name of the NYC public high school |
| `borough` | string | NYC borough where the school is located |
| `building_code` | string | Unique NYC Department of Education building identifier |
| `average_math` | integer | Average SAT Math section score |
| `average_reading` | integer | Average SAT Critical Reading section score |
| `average_writing` | integer | Average SAT Writing section score |
| `percent_tested` | float | Percentage of eligible students tested (where available) |

---

## 🔍 Key Findings

* 📈 **Top Math Performance:** Filtered schools where the average SAT math score was $\ge 640$ (at least 80% of the maximum 800-point section score), sorted descending by math score.
* 🏅 **Top 10 Overall Schools:** Calculated `total_SAT` by summing average math, reading, and writing scores, highlighting the top 10 institutions city-wide.
* 🗺️ **Borough-Level Variability:** Aggregated SAT metrics by borough to determine the count of schools (`num_schools`), mean composite score (`average_SAT`), and score dispersion (`std_SAT`), pinpointing the borough with the largest score variance.

---

## 🚀 How to Run

### 1. ⚙️ Prerequisites
Ensure you have Python 3.8+ installed along with the required libraries:
* `pandas`
* `numpy`
* `jupyter`

### 2. 💻 Installation & Setup
Clone the repository and install the dependencies:
```bash
git clone https://github.com/gjiajanelle/NYC-Public-School-Academic-Performance-Analysis.git
cd NYC-Public-School-Academic-Performance-Analysis
pip install pandas numpy jupyter
```

### 3. ▶️ Running the Analysis
Launch the Jupyter Notebook environment to inspect the analysis and execute the cells:
```bash
jupyter notebook notebook.ipynb
```
