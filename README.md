## The Ultimate EDA Guide
### 1. Import necessary Libraries
The core libraries for EDA:</br>
* **Pandas:** The corner stone for data manipulation in Python.
* **Numpy:** A library for numerical computation.
* **Matplotlib:** A plotting library for creating visualizations.
* **Seaborn:** Built on top of matplotlib, provides a high-level interface for drawing attractive and informative statistical graphics.
* **Scikit-Learn:** Although for machine learning, provides various tools for data preprocessing and model evaluation, which can be useful in EDA.

### 2. Importing Data and Reading Dataset
  **Import Data**
   * **CSV:** data = pd.read_csv("path")
   * **xlsx:** data = pd.read_excel("path")
   * **url:** data = pd.read_csv("url")
   * **Others** data = pd.read_<format>
   
  **Read Data**
   * data.head() # First 5 rows
   * data.tail() # last 5 rows

### 3. Basic Data Inspection
   * **Shape:** df.shape
   * **Data Types and Info:** info() method show data type of each column and identifies any nulls
     
### 4. Data Cleaning/Wrangling
**Data Type Convertion:** </br>
  Convert data types for proper analysis.</br>
**Duplicates**</br>
    i. Identify Duplicates: duplicated()</br>
    ii. Remove Duplicates: drop_duplicates()

**Missing Values**</br>
    i. Identify Missing Values: isnull().sum() method.</br>
    ii. Handle Missing Data</br>
**Inconsistent Data:** </br>
  Correct typos and standardize text.</br>
**Renaming and Reordering Columns:** </br>
  Adjust column names for better readability.

### 5. Data Reduction
The goal is to simplify the dataset by removing unnecessary or redundant features.
i. Drop Irrelevamt Columns
ii. Drop Constant columns as they do not add any information

Consider the domaink knowledge, the objective of your analysis, and statistical measures to determine the relevance of each column.

### 6. Feature Engineering
This is the process of using domain knowledge to create new features from the data, which can significantly improve the performance of ML models. This helps to uncover the most impactful attributes hidden within your data.
**Some Techniques:** </br>
  i. Creating Derived Features: eg age</br>
  ii. Categorizing Continuous variables: eg Binning ages into groups</br>
  iii. Extract Info from Text Data: eg names

### 7. Exploratory Data Analysis
This is an open-ended process where you calculate statistics and make figures to find trends, anomalies, patterns, or relationships within the data. The aim is not only to understand what the data is telling us but also to uncover the underlying structure, detect outliers, and test underlying assumptions.

**NB:** EDA is iterative and exploratory in nature. It guides how you frame your analysis, leading to hypothesis generation and further analysis or modeling.

**Key Components of EDA:** </br>
  i. Descriptive Statistics: Summarize and describe main features of the dataset</br>
  ii. Data Visualization: Use various plots to see the distribution and relationships between variables.</br>
    * Univariate Graphical/ Non-Graphical
    * Bivariate Graphical/ Non-Graphical
    * Multivariate Graphical/ Non-Graphical
  iii. Correlation Analysis: Determine how variables are related to each other.</br>
  iv. Outlier Detection: Identify unusual observations in the dataset.</br>

### 8. Statistics Summary
This step is crucial for understanding the distribution, central tendency, and dispersion of the data.
  * **Descriptive Statistics:** Use describe() method.
  * **Central Tendency:** Measures like mean, median, and mode.
  * **Dispersion Measures:** Standard deviation, variance, range, and IQR.
  * **Skewness and Kurtosis:** Understanding the assymetry and tailedness of the distribution. Helps identify outliers, errors or peculiariries that need attention.

### 9. Data Transformation
This involves modifying the data to a more suitable format or structure for analysis. This step can include normalization, scaling, or applying mathematical transformations.

These transformations hel[ in preparing the data for more accurate and efficcient analysis, especially when building ML models.
  
  
