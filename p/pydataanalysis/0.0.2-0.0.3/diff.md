# Comparing `tmp/pydataanalysis-0.0.2.tar.gz` & `tmp/pydataanalysis-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydataanalysis-0.0.2.tar", last modified: Thu Mar 30 10:50:58 2023, max compression
+gzip compressed data, was "pydataanalysis-0.0.3.tar", last modified: Sun Apr  9 09:10:17 2023, max compression
```

## Comparing `pydataanalysis-0.0.2.tar` & `pydataanalysis-0.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-03-30 10:50:58.859572 pydataanalysis-0.0.2/
--rw-rw-rw-   0        0        0     1088 2023-03-22 14:25:57.000000 pydataanalysis-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     2936 2023-03-30 10:50:58.859572 pydataanalysis-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1913 2023-03-30 09:22:45.000000 pydataanalysis-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-03-30 10:50:58.656772 pydataanalysis-0.0.2/descriptive/
--rw-rw-rw-   0        0        0        0 2023-03-22 13:19:42.000000 pydataanalysis-0.0.2/descriptive/__init__.py
--rw-rw-rw-   0        0        0    10953 2023-03-30 08:19:09.000000 pydataanalysis-0.0.2/descriptive/pydataprocessing.py
--rw-rw-rw-   0        0        0    18125 2023-03-30 07:28:53.000000 pydataanalysis-0.0.2/descriptive/pyeda.py
-drwxrwxrwx   0        0        0        0 2023-03-30 10:50:58.687972 pydataanalysis-0.0.2/diagnostic/
--rw-rw-rw-   0        0        0        0 2023-03-22 13:20:23.000000 pydataanalysis-0.0.2/diagnostic/__init__.py
--rw-rw-rw-   0        0        0     6296 2023-03-22 14:15:38.000000 pydataanalysis-0.0.2/diagnostic/pydiagnostic.py
-drwxrwxrwx   0        0        0        0 2023-03-30 10:50:58.734772 pydataanalysis-0.0.2/predictive/
--rw-rw-rw-   0        0        0        0 2023-03-22 13:18:06.000000 pydataanalysis-0.0.2/predictive/__init__.py
--rw-rw-rw-   0        0        0    13967 2023-03-30 08:22:27.000000 pydataanalysis-0.0.2/predictive/pypredictive.py
-drwxrwxrwx   0        0        0        0 2023-03-30 10:50:58.750372 pydataanalysis-0.0.2/prescriptive/
--rw-rw-rw-   0        0        0        0 2023-03-22 13:18:42.000000 pydataanalysis-0.0.2/prescriptive/__init__.py
--rw-rw-rw-   0        0        0     1408 2023-03-22 13:27:15.000000 pydataanalysis-0.0.2/prescriptive/pyprescriptive.py
-drwxrwxrwx   0        0        0        0 2023-03-30 10:50:58.843972 pydataanalysis-0.0.2/pydataanalysis.egg-info/
--rw-rw-rw-   0        0        0     2936 2023-03-30 10:50:56.000000 pydataanalysis-0.0.2/pydataanalysis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      448 2023-03-30 10:50:57.000000 pydataanalysis-0.0.2/pydataanalysis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-30 10:50:56.000000 pydataanalysis-0.0.2/pydataanalysis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-03-30 10:50:56.000000 pydataanalysis-0.0.2/pydataanalysis.egg-info/requires.txt
--rw-rw-rw-   0        0        0       47 2023-03-30 10:50:56.000000 pydataanalysis-0.0.2/pydataanalysis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-30 10:50:58.859572 pydataanalysis-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1118 2023-03-30 09:22:45.000000 pydataanalysis-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 09:10:17.825854 pydataanalysis-0.0.3/
+-rw-rw-rw-   0        0        0     1088 2023-03-22 14:25:57.000000 pydataanalysis-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     2964 2023-04-09 09:10:17.823854 pydataanalysis-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1933 2023-04-09 09:03:16.000000 pydataanalysis-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-09 09:10:17.595840 pydataanalysis-0.0.3/descriptive/
+-rw-rw-rw-   0        0        0        0 2023-03-22 13:19:42.000000 pydataanalysis-0.0.3/descriptive/__init__.py
+-rw-rw-rw-   0        0        0    10312 2023-04-09 08:54:11.000000 pydataanalysis-0.0.3/descriptive/pydataprocessing.py
+-rw-rw-rw-   0        0        0    17822 2023-04-04 09:31:18.000000 pydataanalysis-0.0.3/descriptive/pyeda.py
+drwxrwxrwx   0        0        0        0 2023-04-09 09:10:17.618842 pydataanalysis-0.0.3/diagnostic/
+-rw-rw-rw-   0        0        0        0 2023-03-22 13:20:23.000000 pydataanalysis-0.0.3/diagnostic/__init__.py
+-rw-rw-rw-   0        0        0     5884 2023-04-04 09:31:18.000000 pydataanalysis-0.0.3/diagnostic/pydiagnostic.py
+drwxrwxrwx   0        0        0        0 2023-04-09 09:10:17.666844 pydataanalysis-0.0.3/predictive/
+-rw-rw-rw-   0        0        0        0 2023-03-22 13:18:06.000000 pydataanalysis-0.0.3/predictive/__init__.py
+-rw-rw-rw-   0        0        0    13946 2023-04-04 09:31:19.000000 pydataanalysis-0.0.3/predictive/pypredictive.py
+drwxrwxrwx   0        0        0        0 2023-04-09 09:10:17.697846 pydataanalysis-0.0.3/prescriptive/
+-rw-rw-rw-   0        0        0        0 2023-03-22 13:18:42.000000 pydataanalysis-0.0.3/prescriptive/__init__.py
+-rw-rw-rw-   0        0        0     1351 2023-04-04 09:31:17.000000 pydataanalysis-0.0.3/prescriptive/pyprescriptive.py
+drwxrwxrwx   0        0        0        0 2023-04-09 09:10:17.819853 pydataanalysis-0.0.3/pydataanalysis.egg-info/
+-rw-rw-rw-   0        0        0     2964 2023-04-09 09:10:16.000000 pydataanalysis-0.0.3/pydataanalysis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      448 2023-04-09 09:10:17.000000 pydataanalysis-0.0.3/pydataanalysis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 09:10:16.000000 pydataanalysis-0.0.3/pydataanalysis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-04-09 09:10:16.000000 pydataanalysis-0.0.3/pydataanalysis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       47 2023-04-09 09:10:16.000000 pydataanalysis-0.0.3/pydataanalysis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-09 09:10:17.827854 pydataanalysis-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1118 2023-04-02 13:19:45.000000 pydataanalysis-0.0.3/setup.py
```

### Comparing `pydataanalysis-0.0.2/LICENSE` & `pydataanalysis-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pydataanalysis-0.0.2/PKG-INFO` & `pydataanalysis-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 Metadata-Version: 2.1
 Name: pydataanalysis
-Version: 0.0.2
+Version: 0.0.3
 Summary: Data Analysis and  Visualization Functions
 Home-page: UNKNOWN
 Author: Tamer Samara
 Author-email: tamer.samara@gmail.com
 License: MIT
 Description: <h1>Data Analysis CheatSheet (everything you might need )</h1>
         <p>
         The project include four modules with functions to summarize and analysis dataset in order 
         to understand properties and relationships.
         
-          [more info read the documentation](docs/_build/html/index.html)
+        [Read Documentation](https://tamer-george.github.io/docs/_build/html/index.html)
         </p>
         <h2>1. DESCRIPTIVE  MODULE</h2>
         <h3>Answer the question (What Happen?)</h3>
         
         Includes two modules:
         
                     
         - <i>pyeda.py</i><br>
         Includes simple EDA functions that might be useful in general cases.<br><br>
-          - <i>pydatapreprocessing.py</i><br> 
-          Useful Functions for data preprocessing.<br>
+        - <i>pydatapreprocessing.py</i><br> 
+        Useful Functions for data preprocessing.<br>
         
-                  For Example:
-                  from descriptive import pyeda
-                  pyeda.distribution_of_numeric_column(data_frame, column_name: str)
+                For Example:
+                from descriptive import pyeda
+                pyeda.visualize_different_plots_of_numeric_col(data_frame, column_name: str)
         
         
-                  For Example:
-                  from descriptive import pydatapreprocessing
-                  pydatapreprocessing.standardization_numerical_columns(data, numerical_column: list)
+                For Example:
+                from descriptive import pydatapreprocessing
+                pydatapreprocessing.standardization_numerical_columns(data, numerical_column: list)
           <h2>2. DIAGNOSTIC MODULE</h2>
           <h3>Answer the question (Why did it happen?)</h3>
           <i>pydiagnostic.py</i><br><br>
           Include functions to apply hypothesis testing 
                   
                   For Example:
                   from diagnostic import pydiagnostic
-                  pydiagnostic.test_p_value(p_value:float)   
+                  pydiagnostic.display_test_p_value(p_value: float)   
         
         
         <h2>3. PREDICTIVE MODULE </h2>
         <h3>Answer the question (What is likely to Happen?)</h3>
         <i>pypredictive.py</i> <br><br>
         The module include functions for:
         *    Regression  
@@ -61,14 +61,15 @@
         <i>pyprescriptive.py</i><br>
         
         Module include functions that might be useful for classification 
         
                 For Example:
                 from prescriptive import pyprescriptive
                 pyprescriptive.visualize_confusion_matrix(actual, predicted)
+        
 Keywords: python,data science,eda,data preprocessing,data analysis,machine learning
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
```

### Comparing `pydataanalysis-0.0.2/README.md` & `pydataanalysis-0.0.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 <h1>Data Analysis CheatSheet (everything you might need )</h1>
 <p>
 The project include four modules with functions to summarize and analysis dataset in order 
 to understand properties and relationships.
 
-  [more info read the documentation](docs/_build/html/index.html)
+[Read Documentation](https://tamer-george.github.io/docs/_build/html/index.html)
 </p>
 <h2>1. DESCRIPTIVE  MODULE</h2>
 <h3>Answer the question (What Happen?)</h3>
 
 Includes two modules:
 
             
 - <i>pyeda.py</i><br>
 Includes simple EDA functions that might be useful in general cases.<br><br>
-  - <i>pydatapreprocessing.py</i><br> 
-  Useful Functions for data preprocessing.<br>
+- <i>pydatapreprocessing.py</i><br> 
+Useful Functions for data preprocessing.<br>
 
-          For Example:
-          from descriptive import pyeda
-          pyeda.distribution_of_numeric_column(data_frame, column_name: str)
+        For Example:
+        from descriptive import pyeda
+        pyeda.visualize_different_plots_of_numeric_col(data_frame, column_name: str)
 
 
-          For Example:
-          from descriptive import pydatapreprocessing
-          pydatapreprocessing.standardization_numerical_columns(data, numerical_column: list)
+        For Example:
+        from descriptive import pydatapreprocessing
+        pydatapreprocessing.standardization_numerical_columns(data, numerical_column: list)
   <h2>2. DIAGNOSTIC MODULE</h2>
   <h3>Answer the question (Why did it happen?)</h3>
   <i>pydiagnostic.py</i><br><br>
   Include functions to apply hypothesis testing 
           
           For Example:
           from diagnostic import pydiagnostic
-          pydiagnostic.test_p_value(p_value:float)   
+          pydiagnostic.display_test_p_value(p_value: float)   
 
 
 <h2>3. PREDICTIVE MODULE </h2>
 <h3>Answer the question (What is likely to Happen?)</h3>
 <i>pypredictive.py</i> <br><br>
 The module include functions for:
 *    Regression  
@@ -52,8 +52,8 @@
 
 <i>pyprescriptive.py</i><br>
 
 Module include functions that might be useful for classification 
 
         For Example:
         from prescriptive import pyprescriptive
-        pyprescriptive.visualize_confusion_matrix(actual, predicted)
+        pyprescriptive.visualize_confusion_matrix(actual, predicted)
```

### Comparing `pydataanalysis-0.0.2/descriptive/pydataprocessing.py` & `pydataanalysis-0.0.3/descriptive/pydataprocessing.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,273 +1,316 @@
 import numpy as np
 import pandas as pd
 from sklearn.preprocessing import LabelEncoder, StandardScaler, Normalizer, KBinsDiscretizer, MinMaxScaler, RobustScaler
 from sklearn.preprocessing import PowerTransformer, QuantileTransformer
 from scipy.stats import boxcox
 from collections import Counter
 
-"""
-
-     Data Preprocessing 
-
-            -  Data Preprocessing - Functions 
-
-
-"""
-
-
 #                 ----------------  DATA PREPROCESSING  ----------------
 
 
 def unique_values(data, categorical_column: str):
     """
-    Print out all the unique values in a categorical column
-    :param data:variable
-    :param categorical_column:string with column name
+    Print out all the unique values in a categorical column.
+
+    :param data: variable
+
+    :param categorical_column:string
+
     :return:unique values in dataset
     """
     cat_col = data[categorical_column].unique()
     cat_col.sort()
     return cat_col
 
 
 def columns_with_missing_values(data) -> list:
     """
-    PRINT COLUMNS WITH MISSING VALUES
+    Missing values.
+
     :param data:variable
+
     :return:a list of columns with missing values
     """
     cols_with_missing = [col for col in data.columns if data[col].isnull().any()]
     return cols_with_missing
 
 
-def fill_missing_value(data, column_name: str, filling_with: str):
+def replace_NaN_value(data, column_name: str, value_by: str):
     """
-    Handle missing values
-    filling_with string replace "NAN" rows, with one of the chosen string name :
-    median
-    mode
-    mean
-    :param data:variable
-    :param column_name:a string with column name
-    :param filling_with:filling with
-    :return: updated filled column
+    Replace value by median, mode or mean.
+
+    :param data:variable
+
+    :param column_name: str
+
+    :param value_by: str
+
+    :return: column
+
     """
-    if filling_with.lower() == "median":
+    if value_by.lower() == "median":
         return data[column_name].fillna(data[column_name].median(), inplace=True)
-    elif filling_with.lower() == "mean":
+    elif value_by.lower() == "mean":
         return data[column_name].fillna(data[column_name].mean(), inplace=True)
-    elif filling_with.lower() == "mode":
+    elif value_by.lower() == "mode":
         return data[column_name].fillna(data[column_name].mode(), inplace=True)
     else:
         print("Enter mean, median or mode to fill in the missing values")
 
 
 def drop_missing_rows(data):
     """
-    Remove all the rows that contain a missing value
+    Drop rows with missing values.
+
     :param data:variable
-    :return:dataframe without missing rows
+
+    :return:dataframe
+
     """
     dataframe_without_missing_rows = data.copy()
     dataframe_without_missing_rows.dropna(inplace=True)
     return dataframe_without_missing_rows
 
 
 def replace_missing_values_with_zero(data):
     """
-    Replace all NaN values with 0
+    Replace all NaN values with 0.
+
     :param data:variable
-    :return:dataframe filled row with 0
+
+    :return:dataframe
+
     """
     data_filled_with_zero = data.copy()
     data_filled_with_zero.fillna(0, inplace=True)
     return data_filled_with_zero
 
 
 def replace_missing_values_with_what_comes_after_it(data):
     """
-    Replace missing values that comes directly after it in the same column,
+    Replace missing values that comes directly after it in the same column.
+
     :param data:variable
+
     :return:filled dataframe
     """
     bfill_data = data.copy()
     bfill_data.fillna(method="bfill", axis=0, inplace=True)
     return bfill_data
 
 
-def replace_missing_values_with_string(data, column: str, my_string: str):
+def replace_missing_values_with_string(data, column_name: str, my_string: str):
     """
-     replace missing values with a string
+     Replace missing value by string.
+
     :param data: variable
-    :param column: categorical column name as a string
-    :param my_string: fill missing values with a string
-    :return: filled dataframe
+
+    :param column_name: string
+
+    :param my_string: string
+
+    :return: dataframe
     """
 
-    data[column].fillna(my_string, axis=0, inplace=True)
+    data[column_name].fillna(my_string, axis=0, inplace=True)
     return data
 
 
 def remove_duplicated_columns(data):
     """
-    Removes duplicated columns(based on column names)
+    Removes duplicated columns(based on column names).
+
     :param data: variable
-    :return: data without duplicate columns
+
+    :return: data
     """
     data_without_duplicates = data.loc[:, ~data.columns.duplicated()]
     return data_without_duplicates
 
 
 def one_hot_encoding(data, categorical_col: list):
     """
-    encode categorical variables using one-hot encoding
+    Encode categorical variables using one-hot encoding.
+
     :param data:variable
-    :param categorical_col:list with categorical columns name
-    :return: one hot encoded  dataframe
+
+    :param categorical_col:list
+
+    :return: dataframe
     """
     try:
         one_hot_encoded_data = pd.get_dummies(data, columns=categorical_col)
 
     except TypeError:
         print("categorical column Input must be a list")
     except KeyError:
         print("None of type ='object' are in the [columns]")
     else:
         return one_hot_encoded_data
 
 
 def label_encoding(data, categorical_col: list):
     """
-    encode categorical variables using label encoder
+    Encode categorical variables using label encoder.
+
     :param data:variable
-    :param categorical_col:list of categorical column names
-    :return: encoded categorical dataframe
+
+    :param categorical_col:list
+
+    :return:  dataframe
     """
     try:
         label_encoder = LabelEncoder()
         data[categorical_col] = data[categorical_col].apply(label_encoder.fit_transform)
     except ValueError:
         print("categorical column Input must be a list")
     except KeyError:
         print("None of type ='object' are in the [columns]")
     else:
         return data
 
 
 def standardization_numerical_columns(data, numerical_column: list):
     """
-    scale the values of a numeric column so that they have zero mean and unit variance
+    Scale values of a numeric column so that they have zero mean and unit variance.
+
     :param data: variable
-    :param numerical_column:String with numerical column name
+
+    :param numerical_column:String
+
     :return: scale dataframe
     """
     std_scaler = StandardScaler()
     df_scaled = std_scaler.fit_transform(data[numerical_column])
     df_scaled = pd.DataFrame(df_scaled, columns=numerical_column)
     return df_scaled
 
 
 def normalize_numerical_column(data, numerical_column: str):
     """
-    scale the values of a numeric column so that they have a minimum value of 0
-    and a maximum value of 1
-    :param data:
-    :param numerical_column:
-    :return:
+    Scale values of a numeric column so that they have a minimum value of 0 and a maximum value of 1.
+
+    :param data: variable
+
+    :param numerical_column: str
+
+    :return: data
     """
     normalizer = Normalizer()
     data[numerical_column] = normalizer.fit_transform(data[[numerical_column]])
     return data
 
 
 def divide_num_col_into_cat_col_using_bins(data, numerical_col: str, number_bins: int):
     """
-    Divide the values of a continuous numeric column into categorical column using bins
+    Divide the values of a continuous numeric column into categorical column using bins.
+
     :param data: variable
-    :param numerical_col: string with numerical column name
-    :param number_bins: integer of numbers of bins
+
+    :param numerical_col: string
+
+    :param number_bins: integer
+
     :return: dataframe
     """
     discretizer = KBinsDiscretizer(n_bins=number_bins, encode="ordinal")
     data[numerical_col] = discretizer.fit_transform(data[[numerical_col]])
     return data
 
 
 def min_max_scaler_to_numerical_column(data, numerical_column: list):
     """
-    scale the values of a numeric column so that they have a minimum value of 0
-    and a maximum value of 1
+    Scale the values of a numeric column so that they have a minimum value of 0 and a maximum value of 1.
+
     :param data: variable
-    :param numerical_column:string with numerical column name
+
+    :param numerical_column:string
+
     :return:dataframe
     """
     scaler = MinMaxScaler()
     df_scaled = scaler.fit_transform(data.to_numpy())
     df_scaled = pd.DataFrame(df_scaled, columns=numerical_column)
     return df_scaled
 
 
 def robust_scaling_to_numerical_column(data, numerical_column: str):
     """
-    scale the values of a numeric column using the median and interquartile range.
-    it's useful when the data contains outliers.
+    Scale values of a numeric column using the median and interquartile range.
+
     :param data:variable
-    :param numerical_column:string with numerical column name
+
+    :param numerical_column:string
+
     :return:dataframe
     """
     scaler = RobustScaler()
     data[numerical_column] = scaler.fit_transform(data[[numerical_column]])
     return data
 
 
 def power_transformation_to_numerical_column(data, numerical_column: str):
     """
-    power transformer are a class of functions that can be used to transform the values of a numeric column in order to
-    stabilize or improve the assumptions of certain statistical models. it can be useful
-    for correcting the skewness of a distribution
+    Transform values of a numeric column in order to stabilize or improve the assumptions of certain statistical models.
+
     :param data:variable
-    :param numerical_column:string with numerical column name
+
+    :param numerical_column:string
+
     :return:dataframe
     """
     transformer = PowerTransformer()
     data[numerical_column] = transformer.fit_transform(data[[numerical_column]])
     return data
 
 
 def quantile_transformation_to_numerical_column(data, numerical_column: str):
     """
-    Transform the values of a numeric columns so that they have a uniform or normal distribution
+    Transform column value so that they have a uniform or normal distribution.
+
     :param data:variable
-    :param numerical_column:string of numerical column name
+
+    :param numerical_column: string
+
     :return:dataframe
+
     """
     transformer = QuantileTransformer()
     data[numerical_column] = transformer.fit_transform(data[[numerical_column]])
     return data
 
 
 def box_cox_transformation_to_numerical_column(data, numerical_column: str):
     """
-    Transform the values of a numeric columns so that they are approximately normally distributed
+    Box cox transformation.
+
     :param data:variable
-    :param numerical_column:string with numerical column name
-    :return:dataframe
+
+    :param numerical_column: string
+
+    :return: dataframe
+
     """
     data[numerical_column], lambda_ = boxcox(data[numerical_column])
     return data
 
 
-def cumulatively_categories(data, variable_column, threshold: float):
+def cumulatively_categories(data, variable_column: str, threshold: float):
     """
-    summing overall column of a random variables less than or equal to a specified threshold percentage
-    :param data: data variable
-    :param variable_column: string with column name
-    :param threshold: float of percentage values to detect
-    :return: dataframe with new cumulative column
+    Cumulatively
+
+    :param data: variable
+
+    :param variable_column: string
+
+    :param threshold: float
+
+    :return: dataframe
+
     """
     threshold_value = int(threshold * len(data[variable_column]))
     categories_list = []
     s = 0
     counts = Counter(data[variable_column])
     for i, j in counts.most_common():
         s += dict(counts)[i]
@@ -277,17 +320,20 @@
     categories_list.append("Other")
     data[variable_column] = data[variable_column].apply(lambda x: x if x in categories_list else "Other")
     return data
 
 
 def detect_outliers(data):
     """
-    Detect outliers in a data frame
+    Detect outliers in a data.
+
     :param data: variable
-    :return: dataframe of columns with outliers percentage
+
+    :return: dataframe
+
     """
     outlier_percents = {}
     for column in data.columns:
         if data[column].dtype != object:
             q1 = np.quantile(data[column], 0.25)
             q3 = np.quantile(data[column], 0.75)
             iqr = q3 - q1
@@ -298,18 +344,49 @@
             outlier_percents[column] = outlier_percentage
     outlier_dataframe = pd.DataFrame(data=outlier_percents.values(), index=list(outlier_percents.keys()),
                                      columns=['Outlier_percentage'])
     return outlier_dataframe.sort_values(by='Outlier_percentage', ascending=False)
 
 
 def handle_outliers(data, column_name: str):
-    tenth = np.percentile(data[column_name], 10)
+    """
+    Handle outliers in a column.
+
+    :param data: variable
+
+    :param column_name: str
+
+    :return: column
+
+    """
     ninetieth = np.percentile(data[column_name], 90)
     data[column_name] = np.where(data[column_name] > ninetieth, ninetieth, data[column_name])
     return data[column_name]
 
 
-def age_range(df, age_col: str):
-    bins = [0, 10, 20, 30, 40, 50, 60, 70, 80, 90, 100]
-    labels = ["0-18", "18-29", "30-41", "42-53", "54-65", "66-77", "77-88", "88-100"]
-    result = pd.cut(df[age_col], bins=bins, labels=labels, right=False)
-    return result
+def age_range(data, age_column: str):
+    """
+    Split age column to bins.
+
+    :param data: dataframe variable
+
+    :param age_column: age column as a string
+
+    :return: age bins column
+    """
+    data[age_column] = pd.cut(x=data[age_column], bins=[0, 18, 30, 40, 50, 60, 70, 80, 90, 100])
+    return data[age_column]
+
+
+def concat_data(data_one, data_two):
+    """
+    Concat data.
+
+    :param data_one: variable
+
+    :param data_two: variable
+
+    :return: concat dataframe
+    """
+    frames = [data_one, data_two]
+    concat_df = pd.concat(frames, axis=1)
+    return concat_df
```

### Comparing `pydataanalysis-0.0.2/descriptive/pyeda.py` & `pydataanalysis-0.0.3/descriptive/pyeda.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,100 +1,107 @@
 import pandas as pd
 import matplotlib.pyplot as plt
 import seaborn as sns
 from pandas.plotting import lag_plot, autocorrelation_plot, scatter_matrix
 import statsmodels.graphics.gofplots as sm
 
-
 pd.set_option("display.max_columns", None)
 
-"""
-
-     Descriptive Analysis - Answer the question (What Happen? )
-
-        It is divided to two parts:
-            -    part_one. EDA - Functions 
-            -    part_two. Analysis Functions 
-
-
-"""
-
-
 #             ----------------  EDA Methods  ---------------
 
 
 def read_dataset(file_name: str):
-    """
-    read cvs data file
-    :param file_name: a string contain the csv file name
+    """    
+    Read cvs data file.
+    
+    :param file_name: string contain the csv file name
+    
     :return: pandas dataframe
+    
     """
     try:
         df = pd.read_csv(file_name, parse_dates=True)
         return df
     except FileNotFoundError:
         print("No such File, upload your dataset CSV file to the project")
 
 
 def display_summary_data(dataframe):
     """
-    The function prints out a summary table of columns
-        - number of unique
-        - Null values
-        - Null Percentage
-        - DataType
+    The function prints out a summary table of columns.
+    
+    - number of unique.
+    
+    - Null values.
+    
+    - Null Percentage.
+    
+    - DataType.
+    
     :param dataframe: variable
+    
     :return: Summarize columns dataframe
+    
     """
     summary_tabel = pd.DataFrame({"Unique": dataframe.nunique(),
                                   "Null": dataframe.isna().sum(),
                                   "NullPercent": dataframe.isna().sum() / len(dataframe),
                                   "Types": dataframe.dtypes.values})
     print(summary_tabel)
 
 
 def display_seperation_list_of_columns(data):
     """
-    Separate numerical features and categorical features
-    and print out a list of variables name
+    Separate numerical features and categorical features.
+    
     :param data: variable
-    :return: list of numerical and categorical features
+    
+    :return: list of numerical and categorical feature names
+    
     """
     numeric_variable_lst = data.select_dtypes(include=["int64", "float64"]).columns.tolist()
     categorical_variable_lst = data.select_dtypes(include=["object"]).columns.tolist()
 
     print(f"Numerical Columns: {numeric_variable_lst}\nCategorical Columns: {categorical_variable_lst}")
 
 
-def select_numeric_variables(data_frame):
+def select_numeric_variables(data_frame) -> list:
     """
-    Selecting numerical variables
+    Selecting numerical variables.
+    
     :param data_frame: variable
+    
     :return: all numeric features in a dataset
     """
     numeric_variable_lst = data_frame.select_dtypes(exclude="object")
-    return numeric_variable_lst
+    return list(numeric_variable_lst)
 
 
-def select_categorical_variables(data):
+def select_categorical_variables(data) -> list:
     """
-    Selecting categorical variables
+    Selecting categorical variables.
+    
     :param data: variable
+    
     :return: all categorical features in a dataset
     """
     categorical_variable_lst = data.select_dtypes(include="object")
-    return categorical_variable_lst
+    return list(categorical_variable_lst)
 
 
 def visualize_different_plots_of_numeric_col(data_frame, column_name: str):
     """
-    Plot numerical variable in different charts
+    Visualize different plots of numeric column.
+    
     :param data_frame: variable
+    
     :param column_name: string with column name
-    :return: collections of charts
+    
+    :return: chart
+    
     """
     if data_frame[column_name].dtype != object:
         fig, ax = plt.subplots(1, 5, figsize=(24, 4))
         sns.histplot(data_frame[column_name], bins=30, kde=True, ax=ax[0])
         sns.kdeplot(data_frame[column_name], ax=ax[1])
         sns.countplot(x=data_frame[column_name], ax=ax[2])
         sns.boxplot(y=data_frame[column_name], ax=ax[3])
@@ -103,437 +110,578 @@
         plt.show()
     else:
         print("Provide a numerical column to visualize")
 
 
 def visualize_categorical_col(data_frame, column_name: str):
     """
-    Plot Categorical Variable
+    Visualize categorical column.
+    
     :param data_frame: variable
-    :param column_name: string with column name
-    :return: bar chart of the categorical column
+    
+    :param column_name: str
+    
+    :return: bar chart 
+    
     """
     data_frame[column_name].value_counts().plot(kind="bar")
     plt.ylabel("Count")
     plt.xlabel(column_name)
     plt.show()
 
 
 def display_statistics_for_individual_col(data, column_name: str) -> None:
     """
-    Print out basic statistics
+    Print out basic statistics.
+    
     :param data: variable
-    :param column_name: string with column name
-    :return: print out basic statistics
+    
+    :param column_name: str
+    
+    :return: basic statistics
+    
     """
     print(data[column_name].describe())
 
 
 def correlation_between_two_numerical_columns(data, column_one: str, column_two: str) -> float:
     """
-    Calculate correlation between two numerical columns
+    Calculate correlation between two numerical columns.
+    
     :param data: variable
-    :param column_one: string with column name
-    :param column_two: string with column name
-    :return: correlation value between two numerical columns
+    
+    :param column_one: str
+    
+    :param column_two: str
+    
+    :return: correlation value 
     """
     return data[column_one].corr(data[column_two])
 
 
 def calculate_statistics_for_cat_by_num_col(data, cat_column: list, num_column: list):
     """
-    Group the data by a categorical column and numerical column and calculate statistics
+    Group the data by a categorical column and numerical column and calculate statistics.
+    
     :param data: variable
+    
     :param cat_column: List with categorical column name
+    
     :param num_column: List with numerical column name
+    
     :return: new index dataframe
     """
     grouped_data = data.groupby(by=cat_column)[num_column].describe(percentiles=[])
     return grouped_data
 
 
 def scatter_plot(data, numeric_column_one: str, numeric_column_two: str):
     """
-    create a scatter plot to visualize the relationship. between two numeric columns
-    :param data:
-    :param numeric_column_one: string with numerical column name
-    :param numeric_column_two: string with numerical column name
+    Visualize the relationship between two numeric column.
+    
+    :param data: variable
+    
+    :param numeric_column_one: str
+    
+    :param numeric_column_two: str
+    
     :return: scatter plot
+    
     """
     plt.scatter(data[numeric_column_one], data[numeric_column_two])
     plt.xlabel(numeric_column_one)
     plt.ylabel(numeric_column_two)
     plt.show()
 
 
 def box_plot_distribution(data, numeric_column: str):
     """
-    Create a box plot to visualize the distribution of a numeric column
+    Create a box plot to visualize the distribution of a numeric column.
+    
     :param data: variable
-    :param numeric_column: string with numerical column name
+    
+    :param numeric_column: str
+    
     :return: boxplot chart
+    
     """
     plt.boxplot(data[numeric_column])
     plt.ylabel(numeric_column)
     plt.show()
 
 
 def visualize_bar_plot_for_each_category_of_categorical_column(data, cat_column: str, num_column: str):
     """
-    Create a bar plot to visualize the mean of a numeric column for each category of
-    a categorical column
+    Visualize the mean of a numeric column for each category of a categorical column.
+    
     :param data: variable
-    :param cat_column:string with categorical column name
-    :param num_column:string with numerical column name
+    
+    :param cat_column:str
+    
+    :param num_column:str
+    
     :return: bar chart
+    
     """
     data.groupby(cat_column)[num_column].mean().plot(kind="bar")
     plt.ylabel(f"Average {num_column}")
     plt.show()
 
 
 def pivot_tabel(data, index_col: list, columns: list, values: list, agg: str):
     """
-    Create a pivot table to summarize the data
+    Create a pivot table to summarize the data.
+
     :param data:variable
-    :param index_col:list of columns names
+
+    :param index_col:list of column name
+
     :param columns:list of columns name
+
     :param values:list of columns name
+
     :param agg:string of aggfunction
+
     :return: pivot table
     """
 
     pivot_table = pd.pivot_table(data, index=index_col, columns=columns, values=values, aggfunc=agg, margins=True)
     return pivot_table
 
 
 def visualize_pivot_table(pivot_table):
     """
-    Create a heatmap to visualize the pivot table
-    :param pivot_table:
+    Visualize pivot table.
+
+    :param pivot_table: variable
+
     :return: heatmap
+    
     """
     try:
         plt.pcolor(pivot_table, cmap="Reds")
         plt.colorbar()
         plt.show()
     except ValueError:
         print("Not enough values to unpack ")
 
 
 def visualize_relationship_between_multiple_numeric_columns(data, numerical_columns: list):
     """
-    Create a pair plot to visualize the relationship between multiple numeric columns
+    Create a pair plot to visualize the relationship between multiple numeric columns.
+    
     :param data:variable
+    
     :param numerical_columns:list of numerical column names
+    
     :return:pair-plot chart
     """
     sns.pairplot(data, vars=numerical_columns)
     plt.title("Relationship Between Columns")
     plt.show()
 
 
 def visualize_the_mean_by_categories_of_categorical_column(data, numerical_col: str, categorical_col: str):
     """
-    create a point plot to visualize the mean of a numerical column
-    by the categories of a categorical column
-    :param data:variable
-    :param numerical_col:string with numerical column name
-    :param categorical_col:string with categorical column name
+    Create a point plot to visualize the mean of a numerical column
+    by the categories of a categorical column.
+    
+    :param data:variable
+    
+    :param numerical_col:str
+    
+    :param categorical_col:str
+    
     :return: point plot chart
     """
     sns.pointplot(data, x=categorical_col, y=numerical_col)
     plt.ylabel(f"Average {numerical_col}")
     plt.show()
 
 
-def visualize_the_count_of_cat_col_by_categories_cat_col(data, cat_col_one: str, by_cat_col_two: str):
+def visualize_count_plot(data, categorical_col: str, categories_col: str):
     """
-    create a count plot to visualize the count of a categorical column
-    by the categories of another categorical column
-    :param data:variable
-    :param cat_col_one:string with categorical column name
-    :param by_cat_col_two:string with categorical column name
-    :return:count plot chart
+    Visualize a categorical column by the categories of another categorical column.
+    
+    :param data: variable
+    
+    :param categorical_col: str
+    
+    :param categories_col: str
+    
+    :return: count plot 
     """
-    sns.countplot(x=cat_col_one, hue=by_cat_col_two, data=data)
+    sns.countplot(x=categorical_col, hue=categories_col, data=data)
     plt.show()
 
 
 def visualize_boxplot_of_numeric_column_by_categorical_col(data, categorical_col: str, numerical_col: str):
     """
     Create a box plot to visualize the distribution of a numeric column
-    by the categories of a categorical column
+    by the categories of a categorical column.
+    
     :param data:variable
+    
     :param categorical_col:string with categorical column name
+    
     :param numerical_col:string with numerical column name
+    
     :return: boxplot chart
     """
     sns.boxplot(data=data, x=categorical_col, y=numerical_col)
     plt.ylabel(f"{numerical_col}")
     plt.show()
 
 
+def visualize_swarm_plot(data, categorical_colum: str, numerical_column: str):
+    """
+    Create a swarm plot to visualize the distribution of numeric
+    column by the categories of a categorical column.
+    
+    :param data: variable 
+    
+    :param categorical_colum: str
+    
+    :param numerical_column: str
+    
+    :return: swarm plot
+    """
+    sns.swarmplot(x=categorical_colum, y=numerical_column, data=data)
+    plt.ylabel(f"{numerical_column}")
+    plt.show()
+    
+
 def visualize_numeric_column_by_the_categories_of_cat_col(data, categorical_colum: str, numerical_column: str):
     """
     Create a faceting grid to visualize the distribution of multiple numeric
-    columns by the categories of a categorical column
+    columns by the categories of a categorical column.
+    
     :param data:variable
-    :param categorical_colum:string with categorical column name
-    :param numerical_column:string with numerical column name
+    
+    :param categorical_colum:str
+    
+    :param numerical_column:str
+    
     :return: visualize chart
     """
     g = sns.FacetGrid(data, col=categorical_colum)
     g.map(plt.hist, numerical_column)
     plt.show()
 
 
-def relationship_matrix_between_multiple_numeric_columns(data, numerical_columns: list):
+def scatter_plot_matrix_between_multiple_numeric_columns(data, numerical_columns: list):
     """
     Create a scatter plot matrix to visualize the relationship between
-    multiple numeric columns
+    multiple numeric columns.
+    
     :param data:variable
+    
     :param numerical_columns:string with numerical column name
+    
     :return: scatter plot matrix
     """
     scatter_matrix(data[numerical_columns], alpha=0.2, figsize=(6, 6))
     plt.show()
 
 
 def visualize_heatmap(data):
     """
-    Create a heatmap to visualize the correlation between multiple numeric columns
+    Visualize the correlation between multiple numeric column.
+    
     :param data:variable
-    :return: Heatmap chart
+    
+    :return: Heatmap 
+    
     """
-    numeric_features = select_numeric_variables(data)
+    numeric_features = data.select_dtypes(exclude="object")
     plt.figure(figsize=(12, 8))
     sns.heatmap(numeric_features.corr(), cmap="RdYlGn", annot=True)
     plt.show()
 
 
 def visualize_check_of_auto_correlation_in_numerical_col(data, numerical_colum: str):
     """
-
-    :param data:
-    :param numerical_colum:
+    Create a lag plot to check for auto correlation in a numeric column.
+     
+    :param data:variable 
+    
+    :param numerical_colum:str
+    
     :return: auto correlation chart
     """
     lag_plot(data[numerical_colum])
     plt.show()
 
 
 def visualize_auto_correlation_in_numerical_column(data, numerical_colum: str):
     """
-
-    :param data:
-    :param numerical_colum:
+    Create an auto correlation plot to visualize the auto correlation in a numeric column.
+    
+    :param data: variable 
+    
+    :param numerical_colum: str
+    
     :return: auto correlation chart
     """
     autocorrelation_plot(data[numerical_colum])
     plt.show()
 
 
-def regression_plot_between_two_numerical_col(data, numerical_col_one: str, numerical_col_two: str):
+def regression_plot_between_two_numerical_col(data, numerical_column: str, numerical_col: str):
     """
-    Create a regression plot to visualize the relationship between two numeric columns
+    Visualize the relationship between two numeric column.
+    
     :param data:variable
-    :param numerical_col_one:string with numerical column name
-    :param numerical_col_two:string with numerical column name
-    :return:regression chart
+    
+    :param numerical_column:str
+    
+    :param numerical_col:str
+    
+    :return: regression plot
     """
-    sns.regplot(x=numerical_col_one, y=numerical_col_two, data=data)
+    sns.regplot(x=numerical_column, y=numerical_col, data=data)
     plt.show()
 
 
 def mean_confidence_interval_of_numeric_by_categories_col(data, categorical_col: str, numerical_col: str):
     """
-    Create a point plot to visualize the mean and confidence interval of a
-    numerical column by the categories of a categorical column
+    Visualize the mean and confidence interval of a numerical column by the categories of a categorical column.
+    
     :param data:variable
-    :param categorical_col:string with categorical column name
-    :param numerical_col:string with numerical column name
-    :return: point plot chart
+    
+    :param categorical_col:str
+    
+    :param numerical_col: str
+    
+    :return: point plot 
     """
     sns.pointplot(x=categorical_col, y=numerical_col, data=data, errorbar=("ci", 95))
     plt.ylabel(f"Average {numerical_col}")
     plt.show()
 
 
-def visualize_relationship_by_two_numeric_and_categories_col(data, num_col_one: str, num_col_two: str, cat_col: str):
+def visualize_relationship_by_two_numeric_and_categories_col(data, numeric_column: str, numeric_col: str, cat_col: str):
     """
-    Create a line plot to visualize the relationship between two numeric columns and the
-    categories of a categorical column
+    Visualize the relationship between two numeric column and the categories of a categorical column.
+    
     :param data:variable
-    :param num_col_one:string with numerical column name
-    :param num_col_two:string with numerical column name
-    :param cat_col:string with categorical column name
-    :return: line plot chart
+    
+    :param numeric_column:str
+    
+    :param numeric_col:str
+    
+    :param cat_col:str
+    
+    :return: line plot 
     """
-    sns.lmplot(data=data, x=num_col_one, y=num_col_two, hue=cat_col)
+    sns.lmplot(data=data, x=numeric_column, y=numeric_col, hue=cat_col)
     plt.show()
 
 
 def boxen_plot_distribution_of_numeric_and_categories_col(data, num_col: str, cat_col: str):
     """
-    Create a boxen plot to visualize the distribution of a numerical column
-    by the categories of a categorical column
+    Visualize the distribution of a numerical column by the categories of a categorical column.
+
     :param data:variable
-    :param num_col:string with numerical column name
-    :param cat_col:string with categorical column name
-    :return: boxen plot chart
+
+    :param num_col:str
+
+    :param cat_col:str
+
+    :return: boxen plot
     """
     sns.boxenplot(data=data, x=cat_col, y=num_col)
     plt.ylabel(f"{num_col}")
     plt.show()
 
 
 def visualize_distribution_of_numerical_column(data, numerical_col: str):
     """
-    Create a distplot to visualize the distribution of numerical column
+    Create a histogram to visualize the distribution of numerical column.
+
     :param data:variable
-    :param numerical_col:string with numerical column name
-    :return:distribution chart
+
+    :param numerical_col:str
+
+    :return: histogram chart
     """
     sns.histplot(data[numerical_col])
     plt.show()
 
 
 def kernel_density_estimate(data, numerical_col: str):
     """
-    Create a kdeplot to visualize the kernel density estimate ofa numerical column
+    Create a kdeplot to visualize the kernel density estimate of a numerical column.
+
     :param data:variable
-    :param numerical_col:string with numerical column name
+
+    :param numerical_col:str
+
     :return:visualize kernel density estimate
     """
     sns.kdeplot(data[numerical_col])
     plt.show()
 
 
 def rugplot(data, numerical_col: str):
     """
-    Create a rugplot to visualize the distribution of numerical column
+    Create a rugplot to visualize the distribution of numerical column.
+
     :param data:variable
-    :param numerical_col:string with numerical column name
-    :return:visualize rugplot distribution
+
+    :param numerical_col:str
+
+    :return: rugplot distribution
     """
     sns.rugplot(data[numerical_col])
     plt.show()
 
 
-def joint_plot(data, numerical_col_one: str, numerical_col_two: str):
+def visualize_joint_plot(data, numerical_column: str, num_column: str):
     """
-    Create a joint plot to visualize the relationship between two numerical columns
-    and their distributions
+    Visualize the relationship between two numerical column and their distribution.
+
     :param data:variable
-    :param numerical_col_one:string with numerical column name
-    :param numerical_col_two:string with numerical column name
-    :return:relationship distribution plot
+
+    :param numerical_column: str
+
+    :param num_column: str
+
+    :return: joint chart
     """
-    sns.jointplot(data=data, x=numerical_col_one, y=numerical_col_two)
+    sns.jointplot(data=data, x=numerical_column, y=num_column)
     plt.show()
 
 
 def pie_chart_by_numerical_col(data, cat_column: str, num_col: str):
     """
-    Pie chart a categorical column by numerical column
+    Pie chart a categorical column by numerical column.
+
     :param data: variable
-    :param cat_column: categorical column as string
-    :param num_col: numerical column as string
+
+    :param cat_column: string
+
+    :param num_col: string
+
     :return: pie chart
     """
     data.groupby([cat_column]).sum().plot(kind="pie", y=num_col, colors=sns.color_palette("dark"),
                                           startangle=90, autopct="%1.0f%%")
     plt.show()
 
 
 def pie_chart_cate_column(data, cat_column: str):
     """
-    Pie chart a categorical column
+    Pie chart a categorical column.
+
     :param data: variable
+
     :param cat_column: column name as string
+
     :return: pie chart
     """
     data[cat_column].value_counts().plot(kind="pie", colors=sns.color_palette("dark"), autopct="%1.0f%%")
     plt.show()
 
 
-def contingency_table(data, cat_column: str, cat_colum_two: str):
+def contingency_table(data, cat_column: str, categorical_column: str):
     """
-    Create contingency table
+    Create contingency table.
+
     :param data: variable
-    :param cat_column: first column name as a string
-    :param cat_colum_two: second column name as a string
+
+    :param cat_column: string
+
+    :param categorical_column: string
+
     :return: dataframe
     """
-    cross_tab_data = pd.crosstab(index=data[cat_column], columns=data[cat_colum_two], margins=True)
+    cross_tab_data = pd.crosstab(index=data[cat_column], columns=data[categorical_column], margins=True)
     return cross_tab_data
 
 #                 ----------------  Analysis Functions  ----------------
 
 
 def calculate_the_skewness(data, numerical_colum: str) -> float:
     """
-    Calculate Kurtosis of a numerical variable
+    Calculate skewness of a numerical column.
+
     :param data:variable
-    :param numerical_colum:string with numerical column name
+
+    :param numerical_colum:string
+
     :return:skewness value
+
     """
     skew = data[numerical_colum].skew()
     if skew == 0:
         print("Symmetric Column")
     elif skew > 0:
         print("Right Skewed ---> most values on the left")
     elif skew < 0:
         print("Left Skewed ---> most values on the right")
     return skew
 
 
 def calculate_the_kurtosis(data, numerical_colum: str) -> float:
     """
-    Calculate Kurtosis of a numerical variable
+    Calculate kurtosis of a numerical column.
+
     :param data:variable
+
     :param numerical_colum:
+
     :return:kurtosis value
+
     """
     kurt = data[numerical_colum].kurtosis()
     if kurt == 0:
         print("Mesokurtic ---> (Normal)")
     elif kurt > 0:
         print("Leptokurtic ---> (Thin)")
     elif kurt < 0:
         print("PlatyKurtic ---> (Flat)")
     return kurt
 
 
 def visualize_normal_probability_plot(data, numerical_column: str):
     """
-    To find the deviation from the normal process
+    Visualize normal probability.
+
     :param data:variable
-    :param numerical_column:string with numerical column name
-    :return: chart
+
+    :param numerical_column:string
+
+    :return: probability chart
+
     """
     fig, ax = plt.subplots(1, 2, figsize=(12, 7))
     sns.histplot(data[numerical_column], kde=True, color="blue", ax=ax[0])
     sm.ProbPlot(data[numerical_column]).qqplot(line="s", ax=ax[1])
     plt.show()
 
 
-def column_summary_statistics(data, column_name: str):
+def display_summary_statistics(data, column_name: str):
     """
-    Statistical report of a variable
+    Display statistical summary.
+
     :param data:variable
-    :param column_name:string with column name
-    :return: print out statistical summary
+
+    :param column_name: string
+
+    :return: statistical summary
     """
     print(data[column_name].describe())
 
 
 def save_data_to_csv_file(data, filename: str):
     """
-    Save the data to a csv file
+    Save data to a csv file.
+
     :param data: variable
-    :param filename: string with file name and csv extension
+
+    :param filename: string
+
     :return: updated csv data file
     """
     new_data = data.to_csv(filename, index=False)
     return new_data
```

### Comparing `pydataanalysis-0.0.2/diagnostic/pydiagnostic.py` & `pydataanalysis-0.0.3/diagnostic/pydiagnostic.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,39 +24,47 @@
            to the test_p_value function. 
      -  compare_the_means_of_two_numerical_columns: perform a t_test to compare the means of two numeric columns 
            and return the p-value, the return value can be passed to the test_p_value function 
 
 """
 
 
-def test_p_value(p_value: float):
+def display_test_p_value(p_value: float):
     """
-    The function test the p-value with significance level of  0.05
-    :param p_value: float p-value
-    :return: print out the test
+    Significance level of  0.05.
+
+    :param p_value:float
+
+    :return: result of test
+
     """
     alpha = 0.05
     p_value = ceil(p_value)
     if p_value < alpha:
         print("Reject the null hypothesis")
     else:
         print("Accept the null hypothesis")
 
 
-def chi2_test(data, categorical_column_one: str, categorical_column_two: str) -> float:
+def chi2_test(data, categorical_column: str, categorical_col: str) -> float:
     """
-    Test about two categorical variables
-    Sample question: Does the proportion of male and female differ across age groups
+    Test two categorical column.
+
+    sample question: does the proportion of male and female differ across age groups?
+
     :param data:variable
-    :param categorical_column_one:string with categorical column name
-    :param categorical_column_two:string with categorical column name
+
+    :param categorical_column:string
+
+    :param categorical_col:string
+
     :return: p-value
     """
 
-    df_cont = pd.crosstab(data[categorical_column_one], data[categorical_column_two])
+    df_cont = pd.crosstab(data[categorical_column], data[categorical_col])
     observed_values = df_cont.values
     val = chi2_contingency(df_cont)
     expected_values = val[3]
     no_of_rows = df_cont.shape[0]
     no_of_columns = df_cont.shape[1]
     degree_of_freedom = (no_of_rows-1) * (no_of_columns - 1)
     chi_square = sum([(o-e)**2/e for o, e in zip(observed_values, expected_values)])
@@ -64,77 +72,98 @@
     # critical_value = stats.chi2.ppf(q=1 -alpha, df=ddof)
     p_value = 1 - stats.chi2.cdf(x=chi_square_statistic, df=degree_of_freedom)
     print("p_value", p_value)
     print("Degree of freedom", degree_of_freedom)
     return p_value
 
 
-def test_one_categorical_and_one_numeric(data, numerical_column: str, categorical_column: str) -> float:
+def test_categorical_by_numeric(data, numerical_column: str, categorical_column: str) -> float:
     """
-    Test about one categorical and one numeric Variable
-    Sample question:  Is there a difference in height between men and women
-    :param data:variable
-    :param numerical_column:string with numerical column name
-    :param categorical_column:string with categorical column name
-    :return: p_value
+    Test categorical column by numeric column.
+
+    sample question: is there difference in height between men and women?
+
+    :param data: variable
+
+    :param numerical_column: str
+
+    :param categorical_column: str
+
+    :return: p-value
     """
     category_group_list = data.groupby(categorical_column)[numerical_column].apply(list)
     fvalue, p_value = stats.ttest_ind(*category_group_list)
     print(f"P-value of: {p_value}")
     return p_value
 
 
-def analysis_of_variance_test(data, numerical_column: str, categorical_group_column: str) -> float:
+def oneway_anova_test(data, numerical_column: str, categories_column: str) -> float:
     """
-    Function takes the  group as input and returns ANOVA f and p value
-    Sample question:  Is there a difference in height between age groups
+    Oneway anova test.
+
+    sample question: is there difference in height between age group?
+
     :param data:variable
-    :param numerical_column:string with numerical column name
-    :param categorical_group_column:string with categorical column name
-    :return: float p_value
+
+    :param numerical_column:string
+
+    :param categories_column:string
+
+    :return: p_value
     """
-    category_group_list = data.groupby(categorical_group_column)[numerical_column].apply(list)
+    category_group_list = data.groupby(categories_column)[numerical_column].apply(list)
     fvalue, p_value = stats.f_oneway(*category_group_list)
     print(f"P-value of: {p_value}")
     return p_value
 
 
 def wilcoxon_rank_test(data, numerical_colum_before: str, numerical_column_after: str) -> float:
     """
-    example hypotheses test:
-            H0: Sample distribution are equal
-            H1: Sample distribution are not equal
+    Wilcoxon test for dependent column.
+
     :param data:variable
-    :param numerical_colum_before:string with numerical column name
-    :param numerical_column_after:string with numerical column name
+
+    :param numerical_colum_before:string
+
+    :param numerical_column_after:string
+
     :return:float p_value
     """
     w, p_value = wilcoxon(data[numerical_colum_before], data[numerical_column_after])
     print(f"P-value of: {p_value}")
     return p_value
 
 
-def test_relationship_between_two_numeric_variables(data, numeric_column_one: str, numeric_column_two: str) -> float:
+def test_relationship_between_numerical_columns(data, numeric_column: str, second_numerical_column: str) -> float:
     """
-    Test about two numeric variables
-    Sample question: Is there a relationship between height and weight
-    :param data:variable
-    :param numeric_column_one:string with numerical column name
-    :param numeric_column_two:string with numerical column name
-    :return:float p_value
+    Perform a test to find the relationship of two numerical columns.
+    
+    sample question: is there relationship between height and weight?
+    
+    :param data:variable
+    
+    :param numeric_column:str
+    
+    :param second_numerical_column: str 
+    
+    :return: float p_value
     """
-    pearson_coef, p_value = stats.pearsonr(data[numeric_column_one], data[numeric_column_two])
+    pearson_coef, p_value = stats.pearsonr(data[numeric_column], data[second_numerical_column])
     print(f"Pearson Correlation Coefficient {pearson_coef}, and a P-value of{p_value}")
     return p_value
 
 
-def compare_the_means_of_two_numerical_columns(data, numerical_col_one: str, numerical_col_two: str) -> float:
+def compare_the_means_of_two_numerical_columns(data, first_numerical_col: str, second_numerical_col: str) -> float:
     """
-    perform a t_test to compare the means of two numeric columns
+    Perform a t_test to compare the means of two numeric column.
+    
     :param data:variable
-    :param numerical_col_one:string with numerical column name
-    :param numerical_col_two:string with numerical column name
+    
+    :param first_numerical_col:string with numerical column name
+    
+    :param second_numerical_col:string with numerical column name
+    
     :return: float p-value
     """
-    t, p_value = ttest_ind(data[numerical_col_one], data[numerical_col_two])
+    t, p_value = ttest_ind(data[first_numerical_col], data[second_numerical_col])
     print(t, p_value)
     return p_value
```

### Comparing `pydataanalysis-0.0.2/predictive/pypredictive.py` & `pydataanalysis-0.0.3/predictive/pypredictive.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 import seaborn as sns
 from sklearn.linear_model import LinearRegression
 from sklearn.preprocessing import PolynomialFeatures
 from sklearn.model_selection import train_test_split
 from scipy.signal import periodogram
 from sklearn.cluster import KMeans
 
-"""
-
-     Predictive Analysis - Answer the question (What is likely to Happen? )
+"""Predictive Analysis - Answer the question (What is likely to Happen?)
 
      The module is divided to three parts:
-     1. Regression  
-     2. Forcasting 
-     3. Classification  
-     4. Clustering 
+     
+             1. Regression  
+             2. Forcasting 
+             3. Classification  
+             4. Clustering 
+             
      Regression vs Classification
      regression algorithms are used to predict the continuous values and classification algorithms are used to
      predict/ classify the discrete values 
      *      Types of Classification Algorithms                           *     Types of Regression Algorithms 
             Logistic Regression                                                Simple Linear Regression              
             K_Nearest Neighbours                                               Multiple Linear Regression   
             Support Vector Machine                                             Polynomial Regression  
@@ -35,18 +35,22 @@
 
 """
 #                   ---------------  REGRESSION     ---------------
 
 
 def calculate_slope(data, independent_column: str, predicted_column: str) -> float:
     """
-    calculate slope
+    Calculate slope.
+
     :param data:variable
+
     :param independent_column:string
+
     :param predicted_column:string
+
     :return: slope value
     """
     if len(data[independent_column]) != len(data[predicted_column]):
         raise ValueError(f"length of {data[independent_column]} is not equal to length of{data[predicted_column]}")
     data[independent_column] = np.array(data[independent_column])
     data[predicted_column] = np.array(data[predicted_column])
     n = len(data[independent_column])
@@ -57,18 +61,22 @@
     slope = (n_sum_x_y - sum_x_sum_y) / (n_sum_x_exp2 - sum_x_exp2)
     # print(f"slope : {np.round(slope, 4)}")
     return np.round(slope, 4)
 
 
 def calculate_intercept_of_y(data, independent_column: str, predicted_column: str) -> float:
     """
-    calculate y - intercept
+    Calculate y - intercept.
+
     :param data:variable
+
     :param independent_column:string
+
     :param predicted_column:string
+
     :return: y_intercept value
     """
     if len(data[independent_column]) != len(data[predicted_column]):
         raise ValueError(f"length of {data[independent_column]} is not equal to length of{data[predicted_column]}")
 
     n, slope = len(data[independent_column]), calculate_slope(data, independent_column, predicted_column)
     sum_y = data[predicted_column].sum()
@@ -76,52 +84,66 @@
     y_intercept = (sum_y - m_sum_x) / n
     # print(f"y intercept: {np.round(y_intercept, 4)}")
     return np.round(y_intercept, 4)
 
 
 def plot_linear_equation(data, independent_column: str, predicted_column: str):
     """
-    Plot a linear equation
+    Visualize a linear equation.
+
     :param data:variable
+
     :param independent_column:string
+
     :param predicted_column:string
+
     :return: scatter plot
+
     """
     slope = calculate_slope(data, independent_column, predicted_column)
     y_intercept = calculate_intercept_of_y(data, independent_column, predicted_column)
     data["predicted"] = data[independent_column].map(lambda x: slope * x + y_intercept)
     sns.scatterplot(x=independent_column, y=predicted_column, data=data)
     sns.lineplot(x=independent_column, y=data["predicted"], color="orange", lw=4, data=data)
     plt.show()
 
 
 def split_data_into_training_and_test(data, independent_colum: list, dependent_column: str):
     """
-    Split data to training and test 80 % train and 20 % test
+    Split data to training and test 80 % train and 20 % test.
+
     :param data:variable
+
     :param independent_colum:list
+
     :param dependent_column:string
-    :return: x_train, x_test, y_train, y_test
+
+    :return: dataframe
+
     """
     x = data[independent_colum]
     y = data[dependent_column]
     x_train, x_test, y_train, y_test = train_test_split(x, y, train_size=0.80, test_size=0.20, random_state=0)
     return x_train, x_test, y_train, y_test
 
 
 def plot_polynomial_regression(data, independent_colum, dependent_column, degree: int):
     """
-    implementing polynomial regression, transforming the inputs to include nonlinear terms such as X2
-    depending on the case choose the right optimal degree by taking in consideration under fitting and over fitting
-    for small data
+    Visualize and display polynomial regression.
+
     :param data:variable
+
     :param independent_colum:string
+
     :param dependent_column:list
+
     :param degree:integer
-    :return: Polynomial Regression Plot & printing out the intercept_, coef_, R2(coefficient of determination)
+
+    :return: model
+
     """
     series = pd.Series(data[independent_colum])
     arr = series.values
     x = arr.reshape((-1, 1))
     y = data[dependent_column]
     x_ = PolynomialFeatures(degree=degree, include_bias=False).fit_transform(x)
     model = LinearRegression().fit(x_, y)
@@ -134,111 +156,152 @@
     plt.ylabel(f"{dependent_column}")
     plt.show()
     return model
 
 
 def multi_linear_regression(data, independent_colum: list, dependent_column: str):
     """
-    implementing MLR, implement independent column as a list
-    :param data:
+    Implementing MLR, implement independent column as a list.
+
+    :param data: variable
+
     :param independent_colum:list
+
     :param dependent_column:string
+
     :return: MLR & printing out the intercept_, coef_, R2(coefficient of determination)
+
     """
     x = data[independent_colum]
     y = data[dependent_column]
     model = LinearRegression().fit(x, y)
     r_sq = model.score(x, y)
     print(f"coefficient of determination: {r_sq}\nintercept: {model.intercept_}\ncoefficients: {model.coef_}")
     return model
 
 
-def print_linear_regression_summary(data, x_input: list, y_output: str):
+def display_ols_summary(data, x_input: list, y_output: str):
     """
+    Display ols summary.
+
+    :param data: variable
 
-    :param data:
     :param x_input: list
-    :param y_output: string
-    :return:
+
+    :param y_output: str
+
+    :return: display ols
+
     """
     x = sm.add_constant(data[x_input])
     model = sm.OLS(data[y_output], x)
     results = model.fit()
     print(results.summary())
     # print(f"coefficient of determination: {results.rsquared}\nadjust coefficient of determination: "
     #       f"{results.rsquared_adj}\nregression coefficients: {results.params}")
 
 
 def make_mi_score(x, y):
     """
-    mutual information
+    Mutual information.
+
     :param x:
+
     :param y:
-    :return:
+
+    :return: mi_score
     """
     for colname in x.select_dtypes(["object", "category"]):
         x[colname], _ = x[colname].factorize()
     discrete_features = [pd.api.types.is_integer_dtype(t) for t in x.dtypes]
     mi_scores = mutual_info_regression(x, y, discrete_features=discrete_features, random_state=0)
     mi_scores = pd.Series(mi_scores, name="MI Scores", index=x.columns)
     mi_scores = mi_scores.sort_values(ascending=False)
     return mi_scores
 
 
-def plot_mi_scores(scores):
+def plot_mi_scores(mi_score):
     """
-    plot out sorted mutual score
-    :param scores: variable
+    Plot sorted score.
+
+    :param mi_score: variable
+
     :return: bar chart
+
     """
-    scores = scores.sort_values(ascending=True)
-    width = pd.Series(scores)
-    ticks = scores.index
-    plt.barh(width, scores)
+    mi_score = mi_score.sort_values(ascending=True)
+    width = pd.Series(mi_score)
+    ticks = mi_score.index
+    plt.barh(width, mi_score)
     plt.yticks((width, ticks))
     plt.title("Mutual Information Scores")
     plt.show()
 
 #                   ---------------  FORCASTING     ---------------
 
 
 def set_index_to_date(data, date_column: str):
+    """
+    Set index to date.
+
+    :param data: variable
+
+    :param date_column: str
+
+    :return: dataframe
+
+    """
     data = data.set_index(date_column)
     set_index_data = pd.to_datetime(data.index, infer_datetime_format=True)
     return set_index_data
 
 
 def create_date_range(start_date: str, end_date: str):
+    """
+    Create date range.
+
+    :param start_date: str
+
+    :param end_date: str
+
+    :return: dataframe
+    """
     data_sequence = pd.date_range(start=start_date, end=end_date)
     return data_sequence
 
 
 def create_date_features(data, date_column: str):
     """
-    create date features
+    Create date features.
+
     :param data: data variable
-    :param date_column: string with date  column name
+
+    :param date_column: string
+
     :return: dataframe with date features
     """
     df = data.set_index[date_column]
     df[date_column] = pd.to_datetime(df[date_column], format="%Y-%m-%d", errors="coerce", infer_datetime_format=True)
     df["dayOfWeek"] = df.index.dayofweek
     df["Quarter"] = df.index.quarter
     df["Month"] = df.index.month
     df["Year"] = df.index.year
     df["dayOfYear"] = df.index.dayofyear
     return df
 
 
 def create_hourly_feature(data, date_column: str):
     """
-    create hourly features
+    Create hourly feature.
+
     :param data: data variable
-    :param date_column: string with date  column name
-    :return: dataframe with hourly features
+
+    :param date_column: string
+
+    :return: dataframe
     """
     df = data.set_index[date_column]
     df[date_column] = pd.to_datetime(df[date_column], format="%Y-%m-%d %H:%M:%S", errors="coerce",
                                      infer_datetime_format=True)
     df["hour"] = df.index.hour
     return df
 
@@ -285,15 +348,15 @@
             va="center",
         )
     return ax
 
 
 def plot_periodogram(ts, detrend='linear', ax=None):
     """
-    plot_periodogram(tunnel.NumVehicles);
+    Plot_periodogram(tunnel.NumVehicles)
     """
     fs = pd.Timedelta("1Y") / pd.Timedelta("1D")
     freqencies, spectrum = periodogram(
         ts,
         fs=fs,
         detrend=detrend,
         window="boxcar",
@@ -322,18 +385,20 @@
     ax.set_title("Periodogram")
     return ax
 
 
 #                   ---------------  Classification     ---------------
 def chi_value_plot(data):
     """
-    plot the variable importance by ch2 for binary classification
-    Higher the chi value , higher the importance
-    :param data:
+    Plot the variable importance by ch2 for binary classification.
+
+    :param data: variable
+
     :return: bar chart
+
     """
     for col in data:
         le = LabelEncoder()
         data[col] = le.fit_transform(data[col])
     x = data.iloc[:, : -1]
     y = data.iloc[:, -1]
     # Higher the chi value , higher the importance
@@ -342,18 +407,20 @@
     chi_values.sort_values(ascending=False, inplace=True)
     chi_values.plot.bar()
     plt.show()
 
 
 def p_value_plot(data):
     """
-    plot the variable importance by ch2 for binary classification
-    if p-value > 0.5, lower the importance
+    Plot the variable importance by p-value for binary classification.
+
     :param data: variable
+
     :return: bar chart
+
     """
     for col in data:
         le = LabelEncoder()
         data[col] = le.fit_transform(data[col])
     x = data.iloc[:, : -1]
     y = data.iloc[:, -1]
     # if p-value > 0.5, lower the importance
@@ -362,30 +429,33 @@
     chi_values.sort_values(ascending=False, inplace=True)
     chi_values.plot.bar()
     plt.show()
 
 
 #                   ---------------  Clustering     ---------------
 
-def number_of_cluster(scaled_features):
+def visualize_cluster_sse(scaled_features):
     """
-    After scaling the features, the function choose the appropriate number of clusters
+    Visualize sse scaled column.
+
     :param scaled_features: variable
-    :return: plot chart
+
+    :return: chart
+
     """
     kmean_kwargs = {
         "init": "random",
         "n_init": 10,
         "max_iter": 300,
         "random_state": 42
     }
     sse = []
     for k in range(1, 11):
         kmeans = KMeans(n_clusters=k, **kmean_kwargs)
         kmeans.fit(scaled_features)
         sse.append(kmeans.inertia_)
     plt.style.use("fivethirtyeight")
-    plt.plot(range(1, 11), sse)
+    plt.plot(range(1, 11), sse, marker="o")
     plt.xticks(range(1, 11))
     plt.xlabel("Number of Clusters")
     plt.ylabel("SSE")
     plt.show()
```

### Comparing `pydataanalysis-0.0.2/prescriptive/pyprescriptive.py` & `pydataanalysis-0.0.3/prescriptive/pyprescriptive.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 import matplotlib.pyplot as plt
 from sklearn.metrics import accuracy_score, confusion_matrix, roc_auc_score, roc_curve, ConfusionMatrixDisplay
 from sklearn.metrics import precision_score, recall_score, f1_score
 
-"""
 
-     Prescriptive - Answer the question (What action should we take?)
-
-     Functions that might be useful for classification 
-     - Confusion Matrix
-     - plot the roc curve
-
-"""
-
-
-def visualize_confusion_matrix(y_test, y_predicted):
-    confusion_matrix_ = confusion_matrix(y_test, y_predicted)
+def visualize_confusion_matrix(y_test, y_predict):
+    """
+    Visualization.
+    
+    :param y_test:variable 
+    
+    :param y_predict:variable 
+    
+    :return:chart 
+    
+    """
+    confusion_matrix_ = confusion_matrix(y_test, y_predict)
     cm_display = ConfusionMatrixDisplay(confusion_matrix=confusion_matrix_, display_labels=[False, True])
     cm_display.plot()
-    print({"Accuracy": accuracy_score(y_test, y_predicted),
-           "Precision": precision_score(y_test, y_predicted),
-           "Sensitivity_recall": recall_score(y_test, y_predicted),
-           "Specificity": recall_score(y_test, y_predicted, pos_label=0),
-           "F1_score": f1_score(y_test, y_predicted)
+    print({"Accuracy": accuracy_score(y_test, y_predict),
+           "Precision": precision_score(y_test, y_predict),
+           "Sensitivity_recall": recall_score(y_test, y_predict),
+           "Specificity": recall_score(y_test, y_predict, pos_label=0),
+           "F1_score": f1_score(y_test, y_predict)
            })
     plt.show()
 
 
 def plot_roc_curve(true_y, y_prob):
     """
-    plots the roc curve based of the probabilities
-    :param true_y:
-    :param y_prob:
-    :return:
+    Plot roc curve.
+
+    :param true_y: variable
+
+    :param y_prob: variable
+
+    :return:AUC score and chart
     """
     fpr, tpr, thresholds = roc_curve(true_y, y_prob)
     plt.plot(fpr, tpr)
     plt.xlabel("False Positive Rate")
     plt.ylabel("True Positive Rate")
     plt.show()
     print(f"AUC score: {roc_auc_score(true_y, y_prob)}")
```

### Comparing `pydataanalysis-0.0.2/pydataanalysis.egg-info/PKG-INFO` & `pydataanalysis-0.0.3/pydataanalysis.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 Metadata-Version: 2.1
 Name: pydataanalysis
-Version: 0.0.2
+Version: 0.0.3
 Summary: Data Analysis and  Visualization Functions
 Home-page: UNKNOWN
 Author: Tamer Samara
 Author-email: tamer.samara@gmail.com
 License: MIT
 Description: <h1>Data Analysis CheatSheet (everything you might need )</h1>
         <p>
         The project include four modules with functions to summarize and analysis dataset in order 
         to understand properties and relationships.
         
-          [more info read the documentation](docs/_build/html/index.html)
+        [Read Documentation](https://tamer-george.github.io/docs/_build/html/index.html)
         </p>
         <h2>1. DESCRIPTIVE  MODULE</h2>
         <h3>Answer the question (What Happen?)</h3>
         
         Includes two modules:
         
                     
         - <i>pyeda.py</i><br>
         Includes simple EDA functions that might be useful in general cases.<br><br>
-          - <i>pydatapreprocessing.py</i><br> 
-          Useful Functions for data preprocessing.<br>
+        - <i>pydatapreprocessing.py</i><br> 
+        Useful Functions for data preprocessing.<br>
         
-                  For Example:
-                  from descriptive import pyeda
-                  pyeda.distribution_of_numeric_column(data_frame, column_name: str)
+                For Example:
+                from descriptive import pyeda
+                pyeda.visualize_different_plots_of_numeric_col(data_frame, column_name: str)
         
         
-                  For Example:
-                  from descriptive import pydatapreprocessing
-                  pydatapreprocessing.standardization_numerical_columns(data, numerical_column: list)
+                For Example:
+                from descriptive import pydatapreprocessing
+                pydatapreprocessing.standardization_numerical_columns(data, numerical_column: list)
           <h2>2. DIAGNOSTIC MODULE</h2>
           <h3>Answer the question (Why did it happen?)</h3>
           <i>pydiagnostic.py</i><br><br>
           Include functions to apply hypothesis testing 
                   
                   For Example:
                   from diagnostic import pydiagnostic
-                  pydiagnostic.test_p_value(p_value:float)   
+                  pydiagnostic.display_test_p_value(p_value: float)   
         
         
         <h2>3. PREDICTIVE MODULE </h2>
         <h3>Answer the question (What is likely to Happen?)</h3>
         <i>pypredictive.py</i> <br><br>
         The module include functions for:
         *    Regression  
@@ -61,14 +61,15 @@
         <i>pyprescriptive.py</i><br>
         
         Module include functions that might be useful for classification 
         
                 For Example:
                 from prescriptive import pyprescriptive
                 pyprescriptive.visualize_confusion_matrix(actual, predicted)
+        
 Keywords: python,data science,eda,data preprocessing,data analysis,machine learning
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
```

### Comparing `pydataanalysis-0.0.2/setup.py` & `pydataanalysis-0.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 from setuptools import setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'Data Analysis and  Visualization Functions'
 LONG_DESCRIPTION = 'The modules include functions that might be useful in general cases for data analysis ' \
                    'and data visualization. '
 
 # Setting up
 setup(
     name="pydataanalysis",
```

