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
**NB:** Correct the data types if need be.

### 4. Duplication and Missing Values Management
**Duplicates**
i. Identify Duplicates: duplicated()
ii. Remove Duplicates: drop_duplicates()

**Missing Values**
i. Identify Missing Values: isnull().sum() method.
ii. Handle Missing Data
  
    
  
  
