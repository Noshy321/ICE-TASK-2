
# Medical Aid Cost Prediction - ICE TASK 2

## 📋 Project Overview
This project implements a **Linear Regression model** to predict medical insurance charges based on patient characteristics. Using the Medical Insurance Dataset, I explore relationships between various factors and insurance costs, perform data preprocessing, and evaluate model performance.

**Author:** Kadimetjang Mphahlele  
**Student Number:** ST10496571

## 📊 Dataset Features
The dataset contains information about 1,338 individuals with the following attributes:
- **age**: Age of primary beneficiary
- **sex**: Gender (male/female)
- **bmi**: Body Mass Index
- **children**: Number of children/dependents covered
- **smoker**: Smoking status (yes/no)
- **region**: US residential area (northeast, southeast, southwest, northwest)
- **charges**: Individual medical costs billed by health insurance (target variable)

## 🚀 Key Findings from Exploratory Data Analysis

### Strongest Influencing Factors:
1. **Smoking status** - Smokers have significantly higher charges
2. **Age** - Positive correlation with charges
3. **BMI** - Higher BMI correlates with higher charges, especially above 40
4. **Number of children** - Small positive effect
5. **Region** - Minor variations (southeast slightly higher)
6. **Sex** - Minimal to no significant impact

### Data Distribution:
- Insurance charges are **right-skewed** - most people have lower charges with a long tail of very high charges
- Two distinct clusters appear in age vs. charges, likely separated by smoking status

## 🛠️ Technologies Used
- **Python 3** (ipykernel)
- **Data Manipulation:** Pandas, NumPy
- **Visualization:** Matplotlib, Seaborn
- **Machine Learning:** Scikit-learn
  - Linear Regression
  - Train-test split
  - Metrics: R², MAE, RMSE, MSE

## 📁 Project Structure
```
├── ICE TASK 2.ipynb           # Main Jupyter notebook with complete analysis
├── README.md                   # Project documentation
└── insurance.csv                # Medical insurance dataset
```

## ⚙️ Implementation Steps

### 1. **Data Loading & Exploration**
- Loaded dataset using pandas
- Checked data types and missing values
- Generated summary statistics

### 2. **Exploratory Data Analysis**
- **Univariate analysis:** Distribution of charges
- **Bivariate analysis:** Relationship between features and charges
  - Age vs Charges (scatter plot)
  - BMI vs Charges (scatter plot)
  - Children vs Charges (boxplot)
  - Categorical variables vs Charges (boxplots)

### 3. **Data Preprocessing**
- One-hot encoding for categorical variables (sex, smoker, region)
- Created dummy variables with `drop_first=True` to avoid multicollinearity

### 4. **Model Building**
- Features (X): All columns except 'charges'
- Target (y): 'charges' column
- Train-test split: 80% training, 20% testing
- Model: Linear Regression from scikit-learn

### 5. **Model Evaluation**

```
========================================
MODEL PERFORMANCE
========================================
R-squared (R2): 0.7836
Mean Absolute Error (MAE): $4,181.19
Root Mean Squared Error (RMSE): $5,796.28
Mean Squared Error (MSE): $33,596,915.85
```

## 📊 Visualizations
The notebook includes:
- Distribution plot of insurance charges
- Scatter plots for numerical features vs charges
- Boxplots for categorical features vs charges
- Actual vs Predicted values scatter plot

## 💡 Key Insights
1. **Smoking** is by far the strongest predictor of high insurance costs
2. The model explains **78.36%** of the variance in charges (R² = 0.7836)
3. The model performs well for lower charges but struggles with very high charges (> $40,000)
4. Average prediction error is approximately **$5,796**

## 🔮 Potential Improvements
- Add interaction terms (especially smoker × BMI, smoker × age)
- Use polynomial features for age and BMI
- Try advanced algorithms (Random Forest, Gradient Boosting)
- Collect additional data on medical history or pre-existing conditions
- Investigate high-value outliers as special cases

## 🚦 How to Run
```bash
# Clone the repository
git clone https://github.com/[YOUR-USERNAME]/ICE-TASK-2.git

# Navigate to project directory
cd ICE-TASK-2

# Install required packages
pip install pandas numpy matplotlib seaborn scikit-learn jupyter

# Launch Jupyter Notebook
jupyter notebook "ICE TASK 2.ipynb"
```

## 📝 Reflection Questions Answered

### 1. Which variables most strongly influence medical insurance charges?
**Smoking status, age, and BMI** are the strongest predictors. Smokers have dramatically higher charges, charges increase with age, and very high BMI correlates with elevated costs.

### 2. Why might smoking affect insurance costs?
Smoking leads to numerous health issues (lung cancer, heart disease, respiratory problems) requiring expensive medical treatment. Insurance companies charge higher premiums to smokers to cover these statistically higher expected costs.

### 3. What improvements could be made to the model?
- Adding interaction terms between smoker and other variables
- Polynomial features for non-linear relationships
- Trying ensemble methods like Random Forest
- Collecting more detailed medical history data
- Analyzing high-value outliers separately

## 📄 License
This project is created for educational purposes as part of ICE Task 2.

## 👤 Author
**Kadimetjang Mphahlele**  
- Student Number: ST10496571

## 🙏 Acknowledgments
- Medical Insurance Dataset (source: Kaggle)
- Scikit-learn documentation
- Course instructors for guidance
```
