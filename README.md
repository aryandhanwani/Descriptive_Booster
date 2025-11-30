## 📁 Dataset Structure  
A synthetic dataset of **150+ households** was generated with the following columns:

| Column Name               | Type         | Description |
|--------------------------|--------------|-------------|
| Household_ID             | Categorical  | Unique household identifier |
| Age_of_Household_Head    | Numerical    | Age of the family head |
| Household_Income         | Numerical    | Monthly income |
| Education_Level          | Categorical  | Primary / Secondary / Graduate / Post-Grad |
| Family_Size              | Numerical    | Total members |
| Owns_House               | Categorical  | Yes / No |
| Urban_Rural              | Categorical  | Urban or Rural |

---

# 📝 Part A — Theory  

## 1. Types of Data  
**Numerical Data** — Values expressed in numbers  
Examples: `Age`, `Household_Income`, `Family_Size`

**Categorical Data** — Labels or categories  
Examples: `Education_Level`, `Urban_Rural`, `Owns_House`  
(Aligned with handwritten notes on page 1 of the PDF :contentReference[oaicite:1]{index=1})

---

## 2. Types of Statistics  
### Descriptive Statistics  
Used to summarize and describe data (mean, median, mode, variance, SD, graphs).  
(Referenced from page 4 of your notes :contentReference[oaicite:2]{index=2})

### Inferential Statistics  
Used to draw conclusions about a population using hypothesis testing and sample data.

---

## 3. Measures of Central Tendency  
- **Mean:** Average value  
- **Median:** Middle value  
- **Mode:** Most frequently occurring value  
(Same as described on page 5 of your notes :contentReference[oaicite:3]{index=3})

---

## 4. Measures of Dispersion  
- **Range:** Difference between max and min  
- **Variance:** Average of squared deviations  
- **Standard Deviation:** Typical deviation from mean in original units  
(Referenced from page 3–5 of your notes :contentReference[oaicite:4]{index=4})

---

## 5. Important Statistical Concepts  

### • Gaussian (Normal) Distribution  
A symmetric bell-shaped curve where mean = median = mode.  
(Your handwritten explanation on page 3 :contentReference[oaicite:5]{index=5})

### • Log-Normal Distribution  
Right-skewed distribution where log(data) becomes normal.

### • Percentiles  
Shows the position of data relative to the entire dataset.

### • Quartiles  
Q1, Q2, Q3 divide data into four equal parts.

### • Five Number Summary  
Min, Q1, Median, Q3, Max

### • Skewness  
Indicates asymmetry in distribution.  
(Described on page 2 of PDF as “asymmetry of data” :contentReference[oaicite:6]{index=6})

### • Kurtosis  
Shows heaviness of tails and peakedness.  
(From handwritten notes on page 2–3 :contentReference[oaicite:7]{index=7})

---

# 🧪 Part B — Practical Analysis (Python)

## 1. Data Types Identification  
- **Numerical:** Age, Income, Family Size  
- **Categorical:** Education Level, Urban/Rural, Owns House, Household ID  

---

## 2. Central Tendency (Income & Age)
Calculated using Python:  
- Mean  
- Median  
- Mode  

### **Interpretation (Income)**  
The mean is higher than the median → **right-skewed distribution**, which is expected for income.

---

## 3. Measures of Dispersion  
Computed values include:  
- Range  
- Variance  
- Standard Deviation  
- **Interquartile Range (IQR)**  

### **Interpretation**  
A higher IQR shows that incomes vary widely.  
The presence of outliers confirms right skewness.

---

## 4. Distribution Analysis  
- Histogram of income  
- Gaussian curve fitting  
- Skewness & Kurtosis calculated  

### Interpretation  
- Skewness > 0 indicates right skew  
- Kurtosis describes tail heaviness  
- Histogram confirms non-normal income distribution  

---

## 5. Data Categorization — Visual Comparisons  

### **Boxplots Created:**  
✔ Income vs Education Level  
✔ Income vs Urban/Rural  

These clearly show variations in income across groups and fulfill the assignment requirement.

### **Additional Visuals (if included):**  
- KDE plot  
- Boxplot: Family Size vs Education Level  
- Age vs Income scatter/distribution curve  

---

# 📊 Key Insights  
- Urban households generally earn more than rural households.  
- Higher education levels correlate with higher incomes.  
- Income distribution is right-skewed and not normally distributed.  
- Family size does not strongly predict income.  
- Age shows moderate variation but no extreme skew.

---

# ✔ Conclusion  
This project applies real statistical concepts—mean, median, standard deviation, Gaussian distribution, skewness, kurtosis—combined with Python visualizations to understand household socio-economic patterns.  
The analysis shows meaningful relationships between education, region, and income, demonstrating how statistics helps interpret real-world datasets.

---

# 📎 Files Included  
- `Exam1.ipynb` — Python notebook  
- Generated dataset (CSV)  
- Theory notes (referenced from handwritten PDF)  
