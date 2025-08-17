# 🚗 Multiple Linear Regression – CO2 Emissions Prediction

## 📌 Problem Statement  
The goal of this project is to model the relationship between vehicle specifications and CO2 emissions using **Multiple Linear Regression**.  
We aim to predict `CO2EMISSIONS` from features like `ENGINESIZE`, `CYLINDERS`, and `FUELCONSUMPTION_COMB`.

> هدف پروژه مدل‌سازی رابطه‌ی بین ویژگی‌های فنی خودرو و میزان انتشار گاز CO2 با استفاده از رگرسیون خطی چندمتغیره است.

---

## 🧠 Solution Approach

This notebook demonstrates the full pipeline of implementing multiple linear regression using scikit-learn:

1. **Data Loading**  
   Load the `FuelConsumption.csv` dataset using pandas.

2. **Feature Selection**  
   Selected columns:  
   `ENGINESIZE`, `CYLINDERS`, `FUELCONSUMPTION_COMB`, and `CO2EMISSIONS`.

3. **Data Visualization**  
   Scatter plots to explore correlation between features and target.

4. **Train-Test Split**  
   Dataset split randomly into training (80%) and test (20%) subsets.

5. **Model Training**  
   A linear regression model is trained using:
   ```python
   regr = LinearRegression()
   regr.fit(train_x, train_y)
``

6. **Evaluation**

   * Coefficients and intercept are printed.
   * R² score is computed on test data using `r2_score`.

---

## 🛠️ Technologies & Libraries

* **Python 3**
* **Pandas** – data manipulation
* **NumPy** – numerical operations
* **Matplotlib & Pylab** – plotting
* **scikit-learn** – `LinearRegression` and `r2_score`

---

## 🚀 Installation & Execution Guide

### 1. Install Dependencies

```bash
pip install pandas numpy matplotlib scikit-learn
```

### 2. Dataset

Place `FuelConsumption.csv` in the appropriate directory or update the path in the notebook accordingly.

### 3. Run Notebook

Use Jupyter to open and run the notebook:

```bash
jupyter notebook 02_Multiple-Linear-Regression.ipynb
```

---

## 📊 Key Results & Model Performance

* **Coefficients**:

  ```
  [[10.52277345, 7.57289264, 9.46033011]]
  ```
* **R² Score**: \~0.84 (reported from other version)

> مدل موفق شد با دقت حدود ۸۴٪ واریانس CO2 را با استفاده از ویژگی‌ها پیش‌بینی کند.

---

## 🖼️ Sample Outputs

### 1. Raw Dataset Preview:

```
ENGINESIZE | CYLINDERS | FUELCONSUMPTION_COMB | CO2EMISSIONS
    2.0    |     4     |          8.5         |     196
```

### 2. Selected Features:

```
ENGINESIZE | CYLINDERS | FUELCONSUMPTION_COMB | CO2EMISSIONS
    2.4    |     4     |          9.6         |     221
```

### 3. Visualizations:

* `ENGINESIZE` vs `CO2EMISSIONS`
* Train/Test scatter plot
* Regression line on training data

> نمودارها برای درک بهتر رابطه ویژگی‌ها و متغیر هدف استفاده شده‌اند.

---

## 💡 What This Project Demonstrates

* Practical understanding of multiple linear regression
* Feature selection and preprocessing
* Model training with scikit-learn
* Use of R² score for evaluation
* Professional plotting for data interpretation
* Documentation and clarity in model-building steps

---

## 👤 Author

**Mehran Asgari**
📧 [imehranasgari@gmail.com](mailto:imehranasgari@gmail.com)
🔗 [github.com/imehranasgari](https://github.com/imehranasgari)

---

## 📄 License

This project is licensed under the Apache 2.0 License.

```
