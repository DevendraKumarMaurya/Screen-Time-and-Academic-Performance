# Screen Time and Academic Performance Analysis

A Probability & Statistics investigation analyzing the relationship between smartphone screen time, daily study habits, and final exam performance among college students.

---

## 📌 Dataset

- **Source:** [Kaggle: Digital Distraction vs Academic Performance](https://www.kaggle.com/datasets/neurocipher/digital-distraction-vs-academic-performance/data)
- **Local File:** `student_digital_life.csv`
- **Sample Size:** 15,000 student records
- **Primary Metrics:**
  - `smartphone_usage_hours`: Daily smartphone screen time (hours)
  - `study_hours_per_day`: Daily study time (hours)
  - `final_exam_score`: Final academic performance score
  - Auxiliary usage features: social media, streaming, gaming hours

---

## 🔬 Research Objectives & Hypotheses

1. **Distributions:** Understand the distributions and summary statistics for screen time, study time, and exam scores.
2. **Correlation Analysis:** Test for linear correlation between smartphone usage and final exam scores ($H_0: \rho = 0$ vs. $H_1: \rho \neq 0$ at $\alpha = 0.05$).
3. **Multiple Regression:** Determine whether smartphone usage remains a significant predictor of exam performance after controlling for study hours.
4. **Group Comparisons:** Assess whether mean exam scores differ significantly between low and high smartphone usage cohorts.

---

## 🚀 Setup & Execution Guide

### 1. Prerequisites
Ensure you have Python 3.10+ installed.

### 2. Clone / Navigate to Project Directory
```bash
cd "Screen-Time-and-Academic-Performance"
```

### 3. Create and Activate a Virtual Environment
```bash
# Create virtual environment
python3 -m venv venv

# Activate on Linux/macOS:
source venv/bin/activate

# Activate on Windows:
# .\venv\Scripts\activate
```

### 4. Install Dependencies
```bash
pip install -r requirements.txt
```
*(Or install manually: `pip install pandas numpy matplotlib seaborn scipy statsmodels scikit-learn jupyter ipykernel`)*

### 5. Run the Analysis

#### In VS Code / IDE:
Open `Screen_Time_Academic_Performance_Analysis.ipynb`, select the virtual environment as your Jupyter kernel, and click **Run All**.

#### In Jupyter Notebook / Lab:
```bash
jupyter notebook Screen_Time_Academic_Performance_Analysis.ipynb
```

#### In Google Colab:
1. Upload `Screen_Time_Academic_Performance_Analysis.ipynb` to Colab.
2. Upload `student_digital_life.csv` into the Colab file explorer.
3. Select **Runtime** > **Run all**.

---

## 📂 Project Structure

```text
├── README.md                                    # Project documentation & setup instructions
├── requirements.txt                             # Python dependencies
├── Screen_Time_Academic_Performance_Analysis.ipynb # Jupyter notebook with EDA, hypothesis tests & regression
└── student_digital_life.csv                     # Dataset (15,000 records)
```

---

## 📊 Summary of Analysis Flow
1. **Data Ingestion & Integrity Checks:** Verify missing values, types, and summary statistics.
2. **Exploratory Data Analysis (EDA):** Histograms, box plots, and scatter plots.
3. **Hypothesis Testing:** Pearson correlation test, two-sample t-test / Welch's t-test.
4. **Ordinary Least Squares (OLS) Regression:** Simple and multiple linear regression models with multicollinearity (VIF) checks and residual diagnostics.
5. **Conclusions & Practical Takeaways:** Interpreting findings within the context of student digital habits.
