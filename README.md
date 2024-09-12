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
   * **Statistical Summary:** describe() method provides a statistical summary of numerical columns.

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
  
    
  
  
