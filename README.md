# 🎓 Internship Selection - Data Analysis & Preprocessing

## Exploratory data analysis and preprocessing on an internship selection dataset to understand what factors influence whether a student gets selected.

---

# 🔧 Preprocessing Steps
## 1. Exploratory Data Analysis

### • Checked dataset shape, data types, and basic info
### • Verified no missing values (isnull().sum())
### • Confirmed no duplicate records (duplicated().sum())
### • Checked class distribution of target variable (selected)

## 2. Feature Engineering

### • Dropped student_id (non-predictive identifier)
### • Binary encoded extracurricular and placement_training (Yes → 1, No → 0)
### • Applied One-Hot Encoding with drop='first' on college_tier to avoid multicollinearity

## 3. Outlier Analysis

### • Plotted boxplots for CGPA, aptitude_score, interview_score, and github_score
### • No significant outliers found — no treatment required

## 4. Correlation Analysis

### • Generated a correlation heatmap to understand feature relationships
### • Checked correlation of each feature with the target variable selected
### • Checked skewness of all numeric columns

## 5. Train-Test Split & Scaling

### • Split data into 80% train / 20% test with stratify=y to preserve class balance
### • Applied StandardScaler — fitted on training data only, transformed test data separately to prevent data leakage

---

# 🔮 Future Work

### • Build and evaluate classification models (Logistic Regression, Random Forest, etc.)
### • Hyperparameter tuning
### • Feature importance analysis
