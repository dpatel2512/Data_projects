# 📊 Student Spending Analysis

## 🎯 Project Objective

To explore and analyze the spending behavior of college students, uncover key financial patterns, and provide data-driven recommendations for improved student financial literacy and management.

---

## 🛠️ Tools & Technologies

- **Programming Language:** Python  
- **Environment:** Jupyter Notebook  
- **Visualization:** Matplotlib, Seaborn  
- **Data Source:** [Kaggle](https://www.kaggle.com/datasets/sumanthnimmagadda/student-spending-dataset/data) - `student_spending.xlsx`  
- **Libraries:** `NumPy`, `Pandas`, `Matplotlib`, `Seaborn`

---

## 🧹 Data Preprocessing

### ✅ Initial Steps
- Loaded dataset using `pandas.read_csv()` from Google Drive.
- Dataset contained **1000 rows** and **17 columns**.

### 🔄 Data Cleaning Process
- Removed **duplicate rows** to ensure data uniqueness.
- Identified **numeric** and **categorical** features using data types.
- Imputed missing values:
  - Categorical: Replaced with `'missing'`
  - Numerical: Replaced with `0`
- Handled **outliers** by computing upper/lower bounds (mean ± 3*std) for each numeric feature. No outliers were removed due to all values being within statistical bounds.

---

## 🧮 Exploratory Data Analysis

### 📌 Descriptive Statistics
- Summary statistics (mean, median, std) computed for all numeric columns.
- Grouped analysis performed:
  - **By School Year:** Trends in income and tuition.
  - **By Gender:** Trends in income and average expenditure.

### 🔍 Key Findings
| Category            | Most Frequent Value     |
|---------------------|--------------------------|
| Gender              | Male                     |
| Year in School      | Senior                   |
| Major               | Biology                  |
| Payment Method      | Mobile Payment App       |

---

## 📊 Visualizations

### 🔸 Average Spending by Category
- Bar chart showing highest spending on **housing**, followed by **food** and **technology**.

### 🔸 Spending Trends by Demographics
- **By Gender:** Bar plot of average category-wise spending.
- **By School Year:** Comparative bar chart showing trends across Freshman, Sophomore, Junior, and Senior.

### 🔸 Monthly Income Comparison
- Bar plot segmented by **school year** and **gender**.

### 🔸 Demographic Distributions
- Pie charts visualizing proportions of:
  - **Gender**
  - **Year in School**

---

## 📂 Dataset Columns

| Column Name               | Type     | Description                               |
|---------------------------|----------|-------------------------------------------|
| `age`                     | int      | Student age                               |
| `gender`                  | object   | Gender identity                           |
| `year_in_school`          | object   | Academic standing                         |
| `major`                   | object   | Academic major                            |
| `monthly_income`          | int      | Monthly earnings                          |
| `financial_aid`           | int      | Aid received                              |
| `tuition`                 | int      | Tuition fees                              |
| `housing`                 | int      | Housing costs                             |
| `food`                    | int      | Food-related expenses                     |
| `transportation`          | int      | Transportation spending                   |
| `books_supplies`          | int      | Academic resources                        |
| `entertainment`           | int      | Leisure-related spending                  |
| `personal_care`           | int      | Grooming and hygiene                      |
| `technology`              | int      | Tech-related expenses                     |
| `health_wellness`         | int      | Health and fitness costs                  |
| `miscellaneous`           | int      | Other expenditures                        |
| `preferred_payment_method`| object   | Credit/Debit/Cash/Mobile Payment App      |

---

## 📈 Statistical Breakdown (Examples)

### Monthly Income by School Year
| Year       | Mean   | Median | Std Dev |
|------------|--------|--------|---------|
| Freshman   | 1057.1 | 1104.0 | 305.72  |
| Sophomore  | 998.77 | 972.5  | 289.01  |
| Junior     | 1002.5 | 1011.0 | 290.33  |
| Senior     | 1023.2 | 1025.5 | 287.87  |

### Monthly Income by Gender
| Gender      | Mean   | Median | Std Dev |
|-------------|--------|--------|---------|
| Female      | 1024.3 | 1033.0 | 291.14  |
| Male        | 1008.3 | 1000.5 | 295.19  |
| Non-binary  | 1030.7 | 1038.0 | 295.48  |

