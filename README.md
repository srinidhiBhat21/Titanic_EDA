# 🚢 Titanic Dataset – Exploratory Data Analysis (EDA)

Link;https://roadmap.sh/projects/titanic-eda-python

## 📌 Project Overview

This project focuses on performing Exploratory Data Analysis (EDA) on the Titanic dataset using Python.

The objective is to explore passenger information, understand survival patterns, identify relationships between passenger characteristics and survival, and extract meaningful insights through data analysis and visualization.

## 📂 Dataset Information

The dataset contains **891 passenger records and 12 columns**.

| Column | Description |
|---|---|
| PassengerId | Unique passenger ID |
| Survived | Survival status (0 = No, 1 = Yes) |
| Pclass | Passenger class (1st, 2nd, 3rd) |
| Name | Passenger name |
| Sex | Gender |
| Age | Passenger age |
| SibSp | Number of siblings/spouses aboard |
| Parch | Number of parents/children aboard |
| Ticket | Ticket number |
| Fare | Ticket fare |
| Cabin | Cabin number |
| Embarked | Port of embarkation |

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

## 🧹 Data Cleaning & Preprocessing

The following data-cleaning operations were performed:

- Checked dataset structure using `df.info()`.
- Examined statistical summaries using `df.describe()`.
- Identified missing values using `df.isnull().sum()`.
- Calculated missing-value percentages.
- Filled missing Age values using the median.
- Filled missing Embarked values using the mode.
- Dropped the Cabin column because approximately 77.10% of its values were missing.
- Checked duplicate records.
- Verified that no missing values remained after cleaning.

## 📊 Exploratory Data Analysis

The following analyses were performed:

### 1. Overall Survival Analysis
- Compared the number of survived and non-survived passengers.
- Calculated the overall survival percentage.
- Created a count plot to visualize survival distribution.

### 2. Gender-wise Survival Analysis
- Compared the number of male and female passengers.
- Calculated survival rates for each gender.
- Visualized gender-wise survival rates.

### 3. Passenger Class Analysis
- Analysed passenger distribution across three classes.
- Compared survival rates among first, second, and third-class passengers.

### 4. Age-wise Analysis
- Categorized passengers into:
  - Child
  - Teenager
  - Adult
  - Middle Aged
  - Senior
- Compared survival rates across different age groups.

### 5. Fare Distribution
- Examined the distribution of passenger fares.
- Used a histogram with KDE to understand fare patterns.

### 6. Combined Analysis
- Compared survival rates based on gender and passenger class.
- Used Pandas pivot tables for combined analysis.
- Analysed the relationship between family size and survival.
- Compared solo travellers with passengers travelling with family.

## 💡 Key Findings

| Analysis | Result |
|---|---|
| Overall survival rate | 38.38% |
| Overall non-survival rate | 61.62% |
| Female survival rate | 74.20% |
| Male survival rate | 18.89% |
| First-class survival rate | 62.96% |
| Second-class survival rate | 47.28% |
| Third-class survival rate | 24.24% |
| Child survival rate | 57.97% |
| Solo traveller survival rate | 30.35% |
| Travelling with family survival rate | 50.56% |

### Important Observations

- Female passengers had a significantly higher survival rate than male passengers.
- First-class passengers had the highest survival rate.
- Children had the highest survival rate among the age groups analysed.
- Passengers travelling with family had a higher survival rate than solo travellers.
- Survival patterns varied considerably across passenger classes and genders.

## 📈 Visualizations

The project includes visualizations created using Matplotlib and Seaborn:

- Passenger Survival Count
- Survival Rate by Gender
- Survival Rate by Passenger Class
- Survival Rate by Age Group
- Passenger Fare Distribution
- Survival Rate by Gender and Passenger Class

## 📚 What I Learned

Through this project, I gained practical experience in:

- Data cleaning and handling missing values.
- Performing exploratory data analysis using Pandas.
- Applying `groupby()` for categorical analysis.
- Calculating percentages and proportions.
- Creating age groups using `pd.cut()`.
- Performing combined analysis using pivot tables.
- Creating meaningful visualizations using Matplotlib and Seaborn.
- Interpreting analytical results and communicating insights.

## ▶️ How to Run the Project

1. Clone this repository:

   ```bash
   git clone <your-repository-url>
   ```

2. Navigate to the project folder:

   ```bash
   cd Titanic-EDA
   ```

3. Install the required libraries:

   ```bash
   pip install pandas numpy matplotlib seaborn jupyter
   ```

4. Open Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

5. Open `titanic_EDA.ipynb` and run the cells.

## 📁 Project Structure

```text
Titanic-EDA/
│
├── titanic_EDA.ipynb
├── train.csv
└── README.md
```

## 🎯 Conclusion

This project helped me understand how exploratory data analysis can be used to uncover patterns and relationships within a dataset.

By analysing passenger demographics, ticket classes, family size, and survival rates, I was able to extract meaningful insights and strengthen my practical Python data analysis skills.

#Python #DataAnalysis #EDA #Pandas #Seaborn #Matplotlib
