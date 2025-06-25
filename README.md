
# Titanic Dataset - Exploratory Data Analysis (EDA) 🔍🚢

This repository section focuses on performing Exploratory Data Analysis (EDA) on the **Titanic - Machine Learning from Disaster** dataset from Kaggle. The goal is to uncover patterns, spot anomalies, and visualize the dataset to understand the factors influencing passenger survival.

---

## 🎯 Objective

To analyze the Titanic dataset to discover key insights and relationships between features, and how they impact the survival of passengers.

---

## 📂 Repository Structure

```
titanic-eda/
│
├── data/
│   └── train.csv                # Original dataset for EDA
│
├── notebooks/
│   └── Titanic_EDA.ipynb        # Jupyter Notebook with full EDA
│
├── plots/
│   └── *.png                    # Saved visualizations (optional)
│
├── README.md                    # EDA overview and steps
├── requirements.txt             # Python dependencies
└── .gitignore                   # Files to ignore in version control
```

---

## 🧪 Steps Performed in EDA

### 1. Load the Data
- Used pandas to load and inspect the structure of the dataset.

### 2. Basic Data Inspection
- `.info()`, `.describe()`, `.shape`, `.dtypes`

### 3. Handling Missing Values
- Identified missing data using `.isnull().sum()`
- Planned imputation for `Age`, `Embarked`, and noted high nulls in `Cabin`.

### 4. Univariate Analysis
- Count plots for categorical features: `Sex`, `Pclass`, `Embarked`
- Histograms for numerical features: `Age`, `Fare`

### 5. Bivariate Analysis
- Survival distribution by `Sex`, `Pclass`, `Embarked`
- Box plots of `Age` and `Fare` vs. `Survived`

### 6. Correlation Matrix
- Heatmap to show correlation between numerical features

### 7. Group-wise Analysis
- Grouped by `Pclass`, `Sex`, and combined categories to explore survival rates

### 8. Outlier Detection
- Box plots used to visually detect outliers in `Age` and `Fare`

### 9. Feature Engineering Ideas (Optional)
- Created `FamilySize` and `IsAlone`
- Extracted titles from names

---

## 📊 Example Visualizations

- Bar charts comparing survival rates
- Box plots for Fare and Age
- Correlation heatmap

---

## 🛠️ Requirements

Install dependencies with:

```bash
pip install -r requirements.txt
```

Libraries used:
- pandas
- numpy
- seaborn
- matplotlib
- jupyter

---

## 🚀 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/titanic-eda.git
   cd titanic-eda
   ```

2. Launch Jupyter Notebook:
   ```bash
   jupyter notebook notebooks/Titanic_EDA.ipynb
   ```

---

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🙌 Acknowledgments

- [Kaggle Titanic Competition](https://www.kaggle.com/c/titanic)
- Community contributions on data analysis and visualization
