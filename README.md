# Titanic Survival Analysis 

## Overview
This project analyzes the famous Titanic dataset to discover patterns 
in passenger survival. It includes exploratory data analysis, 
data visualization, a machine learning model, and an interactive 
survival predictor.

---

## Dataset
- **Source:** Seaborn built-in dataset (originally from Kaggle)
- **Link:** https://www.kaggle.com/c/titanic
- **Size:** 891 passengers, 15 features
- **Task:** Binary Classification — Predict survival (0 = Died, 1 = Survived)

### Features Used
| Feature | Description | Type |
|---------|-------------|------|
| pclass | Passenger ticket class (1=First, 2=Second, 3=Third) | Numerical |
| sex | Gender of passenger | Categorical |
| age | Age of passenger in years | Numerical |
| sibsp | Number of siblings/spouses aboard | Numerical |
| parch | Number of parents/children aboard | Numerical |
| fare | Passenger fare paid | Numerical |
| embarked | Port of embarkation (C=Cherbourg, Q=Queenstown, S=Southampton) | Categorical |

---

## Key Findings
- Overall survival rate was **38.4%**
- **Female survival rate: 74.2%** vs Male survival rate: 18.9%
- **1st class survival: 62.9%** vs 3rd class survival: 24.2%
- Children under 10 had a survival rate of **~70%**
- Higher fare strongly correlated with better survival chances

---

## Visualizations
| Chart | Description |
|-------|-------------|
| Missing Values Heatmap | Shows which columns had missing data |
| Survival Count | Overall survived vs died |
| Survival by Gender | Comparison between male and female survival |
| Survival by Class | Comparison across 1st, 2nd, 3rd class |
| Age Distribution | Age spread of passengers vs survival |
| Fare Distribution | Fare paid distribution |
| Correlation Heatmap | Feature correlations |
| Feature Importance | Which features influenced model most |

---

## Machine Learning Model
- **Algorithm:** Random Forest Classifier
- **Library:** scikit-learn
- **Train/Test Split:** 80% / 20%
- **Accuracy:** ~82%

### Model Performance
| Metric | Class 0 (Died) | Class 1 (Survived) |
|--------|---------------|-------------------|
| Precision | 0.84 | 0.80 |
| Recall | 0.88 | 0.74 |
| F1-Score | 0.86 | 0.77 |

### Feature Importance
| Feature | Importance |
|---------|-----------|
| Sex | 28% |
| Fare | 26% |
| Age | 24% |
| Pclass | 15% |
| Sibsp | 4% |
| Parch | 3% |

---

## Interactive Survival Predictor
The notebook includes an interactive predictor.
Run **Cell 16** and enter passenger details to get a survival prediction.

### Example Predictions
| Passenger | Class | Gender | Age | Fare | Prediction | Survival % |
|-----------|-------|--------|-----|------|------------|------------|
| Young woman | 1st | Female | 28 | £71 | ✓ SURVIVE | 91% |
| Young man | 3rd | Male | 22 | £7 | ✗ NOT SURVIVE | 18% |
| Young girl | 2nd | Female | 8 | £26 | ✓ SURVIVE | 78% |
| Middle-aged man | 1st | Male | 45 | £100 | ✗ NOT SURVIVE | 42% |

---

## Tools and Technologies
| Tool | Purpose |
|------|---------|
| Python 3.x | Programming language |
| Pandas | Data manipulation and analysis |
| NumPy | Numerical computations |
| Matplotlib | Data visualization |
| Seaborn | Statistical data visualization |
| Scikit-learn | Machine learning model |
| Jupyter Notebook | Development environment |

---

## Project Structure




