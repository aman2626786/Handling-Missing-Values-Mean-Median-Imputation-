# Handling-Missing-Values-Mean-Median-Imputation-

### Mean-Median Imputation : 
This Involves mean/median values to fill missing data.

 **Advantages :**
 Simple

 **Disadvantages :**
 1.Distribution Shape
 2.Outliers
 3.Covariance/Correlation Change

 I'll analyze the notebook and summarize its contents for you. Let me take a look at the file first.

### Summary of the Notebook

The notebook is focused on **Mean and Median Imputation** using **Python and Scikit-Learn**, specifically applied to handling missing values in a dataset.

#### **Key Steps in the Notebook**
1. **Imports Libraries**  
   - Uses `pandas`, `numpy`, `matplotlib`, and `sklearn`.

2. **Loads Titanic Dataset**  
   - Reads a CSV file (`titanic_toy.csv`) into a DataFrame.
   - Performs basic exploratory analysis (`df.head()`, `df.info()`, `df.isnull().mean()`).

3. **Splits Data into Train and Test Sets**  
   - Drops the target column (`Survived`).
   - Uses `train_test_split()` to split the dataset.

4. **Computes Mean and Median for Imputation**  
   - Calculates the **mean** and **median** of `Age` and `Fare`.

5. **Performs Mean and Median Imputation Manually**  
   - Fills missing values in `Age` and `Fare` using both the **mean** and **median**.

6. **Analyzes Variance Changes**  
   - Compares variance before and after imputation.

7. **Visualizes Distributions**  
   - Uses **KDE plots** to compare original and imputed values.
   - Uses **boxplots** to show data distribution changes.

8. **Computes Covariance & Correlation**  
   - Checks how imputation affects variable relationships.

9. **Implements Mean & Median Imputation Using Scikit-Learn**  
   - Uses `SimpleImputer` and `ColumnTransformer` for automated imputation.

10. **Transforms Train & Test Data**  
   - Applies the imputation pipeline.
