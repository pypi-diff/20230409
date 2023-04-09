# Comparing `tmp/FinLogic-0.3.4.tar.gz` & `tmp/FinLogic-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FinLogic-0.3.4.tar", last modified: Sun Apr  2 12:46:45 2023, max compression
+gzip compressed data, was "FinLogic-0.3.5.tar", last modified: Sun Apr  9 20:52:53 2023, max compression
```

## Comparing `FinLogic-0.3.4.tar` & `FinLogic-0.3.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1072 2023-03-19 09:29:48.277335 FinLogic-0.3.4/LICENSE
--rw-r--r--   0        0        0    10136 2023-04-01 22:01:36.249290 FinLogic-0.3.4/README.md
--rw-r--r--   0        0        0      423 2023-04-02 12:45:29.754424 FinLogic-0.3.4/finlogic/__init__.py
--rw-r--r--   0        0        0    21430 2023-03-19 09:29:48.278335 FinLogic-0.3.4/finlogic/company.py
--rw-r--r--   0        0        0      745 2023-03-19 09:29:48.278335 FinLogic-0.3.4/finlogic/config.py
--rw-r--r--   0        0        0    15438 2023-04-02 12:44:27.971854 FinLogic-0.3.4/finlogic/database.py
--rw-r--r--   0        0        0      996 2023-04-02 12:44:27.971854 FinLogic-0.3.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-19 09:29:48.278335 FinLogic-0.3.4/tests/__init__.py
--rw-r--r--   0        0        0     2232 2023-04-02 12:44:27.971854 FinLogic-0.3.4/tests/test_company.py
--rw-r--r--   0        0        0      683 2023-04-02 12:44:27.971854 FinLogic-0.3.4/tests/test_database.py
--rw-r--r--   0        0        0    10776 1970-01-01 00:00:00.000000 FinLogic-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-03-19 09:29:48.277335 FinLogic-0.3.5/LICENSE
+-rw-r--r--   0        0        0    10136 2023-04-03 10:41:08.794859 FinLogic-0.3.5/README.md
+-rw-r--r--   0        0        0      423 2023-04-09 20:49:47.249787 FinLogic-0.3.5/finlogic/__init__.py
+-rw-r--r--   0        0        0    22313 2023-04-09 20:35:22.450104 FinLogic-0.3.5/finlogic/company.py
+-rw-r--r--   0        0        0      745 2023-03-19 09:29:48.278335 FinLogic-0.3.5/finlogic/config.py
+-rw-r--r--   0        0        0    16372 2023-04-09 20:35:22.450104 FinLogic-0.3.5/finlogic/database.py
+-rw-r--r--   0        0        0      996 2023-04-02 12:44:27.971854 FinLogic-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-19 09:29:48.278335 FinLogic-0.3.5/tests/__init__.py
+-rw-r--r--   0        0        0     2232 2023-04-02 12:44:27.971854 FinLogic-0.3.5/tests/test_company.py
+-rw-r--r--   0        0        0      683 2023-04-03 10:41:04.879825 FinLogic-0.3.5/tests/test_database.py
+-rw-r--r--   0        0        0    10776 1970-01-01 00:00:00.000000 FinLogic-0.3.5/PKG-INFO
```

### Comparing `FinLogic-0.3.4/LICENSE` & `FinLogic-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `FinLogic-0.3.4/README.md` & `FinLogic-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `FinLogic-0.3.4/finlogic/company.py` & `FinLogic-0.3.5/finlogic/company.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,88 +1,88 @@
-"""
-Module containing the Company Class.
+"""This module contains the Company class, which provides methods for obtaining
+financial reports and calculating financial indicators for a company. Users can
+set the accounting method, unit, tax rate, and language for the company object.
+
+Classes:
+    Company: Represents a company with its financial information and allows
+    users to generate financial reports and indicators.
+
 Abreviations used in code:
     dfi = input dataframe
     dfo = output dataframe
 """
 from typing import Literal
 import numpy as np
 import pandas as pd
 from . import config as c
 
 
 class Company:
-    """
-    Finance Data Class for listed Brazilian Companies.
+    """A class to represent a company financial data.
 
-    Attributes
-    ----------
-    identifier: int or str
-        A unique identifier to filter a company in as fi. Both CVM
-        ID or Fiscal ID can be used. CVM ID (regulator ID) must be an integer.
-        Fiscal ID must be a string in 'XX.XXX.XXX/XXXX-XX' format.
+    This class provides methods to create financial reports and to
+    calculate financial indicators based on a company's accounting data.
+    The class also has an AI generated dictionary to translate from
+    Portuguese to English.
+
+    Attributes:
+        identifier:
+            A unique identifier to filter a company in FinLogic
+            Database. Both CVM ID or Fiscal ID can be used. CVM ID
+            (regulator number) must be an integer. Fiscal ID must be a
+            string in 'XX.XXX.XXX/XXXX-XX' format.
+
+    Methods:
+        report:
+            Generates a financial report based on a specified report
+            type and accounting level.
+        custom_report:
+            Creates a financial report from a custom list of accounting
+            codes.
+        indicators:
+            Returns a DataFrame with common financial indicators for the
+            company.
+
+    Raises:
+        ValueError: If the input arguments are invalid.
     """
 
     def __init__(
         self,
         identifier: int | str,
         acc_method: Literal["consolidated", "separate"] = "consolidated",
         acc_unit: float | str = 1.0,
         tax_rate: float = 0.34,
         language: str = "english",
     ):
-        """Initialize main variables.
-
-        Parameters
-        ----------
-        identifier: int or str
-            A unique identifier to filter a company in as fi.
-            Both CVM ID or Fiscal ID can be used.
-            CVM ID (regulator ID) must be an integer.
-            Fiscal ID must be a string in 'XX.XXX.XXX/XXXX-XX' format.
-        acc_method : {'consolidated', 'separate'}, default 'consolidated'
-            Accounting method used for registering investments in subsidiaries.
-        acc_unit : float or str, default 1.0
-            acc_unit is a constant that will divide company account values.
-            The constant can be a number greater than zero or the strings
-            {'thousand', 'million', 'billion'}.
-        tax_rate : float, default 0.34
-            The 'tax_rate' attribute will be used to calculate some of the
-            company indicators.
-            The 'language' attribute will be used to set the language of the
-            account names.
-
-
-        """
+        """Initializes a new instance of the Company class."""
         self.set_id(identifier)
         self.acc_method = acc_method
         self.acc_unit = acc_unit
         self.tax_rate = tax_rate
         self.language = language
 
-    def set_id(self, identifier: int | str):
-        """
-        Set a unique identifier to filter the company in as fi.
+    def set_id(self, identifier) -> None:
+        """Set a unique identifier to select the company in FinLogic Database.
 
-        Parameters
-        ----------
-        value: int or str
-            A unique identifier to filter a company in as fi.
-            Both CVM ID or Fiscal ID can be used.
-            CVM ID (regulator ID) must be an integer.
-            Fiscal ID must be a string in 'XX.XXX.XXX/XXXX-XX' format.
-
-        Returns
-        -------
-        int or str
-
-        Raises
-        ------
-        KeyError
-            * If passed ``identifier`` not found in as fi.
+        This method sets the company's CVM and fiscal ID based on a given
+        identifier. The identifier can be either the CVM ID or the Fiscal ID
+        (CNPJ). If the identifier is not found in the database, a KeyError is
+        raised.
+        Args:
+
+        identifier: A unique identifier for the company, either as a CVM ID or
+            Fiscal ID (CNPJ). CVM ID (regulator ID) must be an integer.
+            Fiscal ID must be a string in the format 'XX.XXX.XXX/XXXX-XX'.
+
+        Returns:
+            None
+
+        Raises:
+            KeyError: If the given identifier isn't found in Finlogic Database.
         """
         # Create custom data frame for ID selection
         df = (
             c.main_df[["cvm_id", "fiscal_id"]]
             .drop_duplicates()
             .astype({"cvm_id": int, "fiscal_id": str})
         )
@@ -94,143 +94,133 @@
             self._cvm_id = df.loc[df["fiscal_id"] == identifier, "cvm_id"].item()
         else:
             raise KeyError("Company 'identifier' not found in database")
         # Only set company data after object identifier validation
         self._set_main_data()
 
     @property
-    def language(self):
-        """
-        Set the language of the account names.
-        """
-        return self._language
-
-    @language.setter
-    def language(self, language: str):
-        """
-        Set the language of the account names.
-
-        Parameters
-        ----------
-        value: str
-            A valid language string.
-
-        Returns
-        -------
-        str
-
-        Raises
-        ------
-        KeyError
-            * If passed ``language`` not supported.
-        """
-
-        # Supported languages
-        list_languages = ["english", "portuguese"]
-        if language.lower() in list_languages:
-            self._language = language.capitalize()
-        else:
-            raise KeyError(
-                f"'{language}' not supported. Supported languages: {', '.join(list_languages)}"
-            )
-
-    @property
-    def acc_method(self):
-        """
-        Get or set accounting method used for registering investments in
+    def acc_method(self) -> Literal["consolidated", "separate"]:
+        """Gets or sets the accounting method for registering investments in
         subsidiaries.
 
-        Parameters
-        ----------
-        value : {'consolidated', 'separate'}, default 'consolidated'
-            Accounting method used for registering investments in subsidiaries.
-
-        Returns
-        -------
-        str
-
-        Raises
-        ------
-        ValueError
-            * If passed ``value`` is invalid.
+        The "acc_method" must be "consolidated" or "separate". Consolidated
+        accounting combines the financial statements of a parent company and its
+        subsidiaries, while separate accounting keeps them separate. Defaults to
+        'consolidated'.
+
+        Raises:
+            ValueError: If the accounting method is invalid.
         """
         return self._acc_unit
 
     @acc_method.setter
     def acc_method(self, value: Literal["consolidated", "separate"]):
         if value in {"consolidated", "separate"}:
             self._acc_method = value
         else:
             raise ValueError("acc_method expects 'consolidated' or 'separate'")
 
     @property
-    def acc_unit(self):
-        """
-        Get or set a constant to divide company account values.
+    def acc_unit(self) -> float:
+        """Gets or sets the accounting unit for the financial statements.
 
-        Parameters
-        ----------
-        value : float or str, default 1.0
-            acc_unit is a constant that will divide company account values.
-            The constant can be a number greater than zero or the strings
-            {'thousand', 'million', 'billion'}.
-
-        Returns
-        -------
-        float
-
-        Raises
-        ------
-        ValueError
-            * If passed ``value`` is invalid.
+        The "acc_unit" is a constant that will divide all company
+        accounting values. The constant must be a number greater than
+        zero or one of the following strings:
+            - "thousand" to represent thousands       (1,000)
+            - "million" to represent millions     (1,000,000)
+            - "billion" to represent billions (1,000,000,000)
+
+        Returns:
+            The current accounting unit.
+
+        Raises:
+            ValueError: If the accounting unit is invalid.
+
+        Examples:
+            To set the accounting unit to millions:
+                company.acc_unit = "million"
+
+            To set the accounting unit to a custom factor, e.g., 10,000:
+                company.acc_unit = 10_000
         """
         return self._acc_unit
 
     @acc_unit.setter
     def acc_unit(self, value: float | str):
         if value == "thousand":
             self._acc_unit = 1_000
         elif value == "million":
             self._acc_unit = 1_000_000
         elif value == "billion":
             self._acc_unit = 1_000_000_000
-        elif value >= 0:
+        elif value > 0:
             self._acc_unit = value
         else:
             raise ValueError("Accounting Unit is invalid")
 
     @property
-    def tax_rate(self):
-        """
-        Get or set company 'tax_rate' attribute.
+    def tax_rate(self) -> float:
+        """Gets or sets company 'tax_rate' property.
+
+        The "tax_rate" is used to calculate some of the company
+        indicators, such as EBIT and net income. The default value
+        is 0.34, which is the standard corporate tax rate in Brazil.
+
+        Returns:
+            The tax rate value.
+
+        Raises:
+            ValueError: If the tax rate is not a float between 0 and 1.
 
-        Parameters
-        ----------
-        value : float, default 0.34
-            'value' will be passed to 'tax_rate' object attribute if
-             0 <= value <= 1.
-
-        Returns
-        -------
-        float
-
-        Raises
-        ------
-        ValueError
-            * If passed ``value`` is invalid.
+        Examples:
+            To set the tax rate to 21%:
+                company.tax_rate = 0.21
+
+            To set the tax rate to 0% (tax exempt):
+                company.tax_rate = 0.0
         """
         return self._tax_rate
 
     @tax_rate.setter
     def tax_rate(self, value: float):
         if 0 <= value <= 1:
             self._tax_rate = value
         else:
             raise ValueError("Company 'tax_rate' value is invalid")
 
+    @property
+    def language(self) -> str:
+        """Gets or sets the language of the account names.
+
+        It is the language used in the account names of the financial
+        statements. This property accepts a string representing the
+        desired language. Supported languages are "english" and
+        "portuguese". The default is 'english'.
+
+        Returns:
+            The language used in the account names.
+
+        Raises:
+            KeyError: If the provided language is not supported.
+        """
+
+        return self._language
+
+    @language.setter
+    def language(self, language: str):
+        # Supported languages
+        list_languages = ["english", "portuguese"]
+        if language.lower() in list_languages:
+            self._language = language.capitalize()
+        else:
+            raise KeyError(
+                f"'{language}' not supported. Supported languages: {', '.join(list_languages)}"
+            )
+
     def _set_main_data(self) -> pd.DataFrame:
         self._COMP_DF = (
             c.main_df.query("cvm_id == @self._cvm_id")
             .astype(
                 {
                     "co_name": str,
                     "cvm_id": np.uint32,
@@ -282,53 +272,49 @@
 
     def report(
         self,
         report_type: str,
         acc_level: int | None = None,
         num_years: int = 0,
     ) -> pd.DataFrame:
-        """
-        Return a DataFrame with company selected report type.
+        """Generate an accounting report for the company.
 
         This function generates a report representing one of the financial
-        statements for the company adjusted by the attributes passed and
-        returns a pandas.DataFrame with this report.
+        statements for the company adjusted by the attributes passed.
+
+        Args:
+            report_type: Type of financial report to be generated. Options
+                include: "assets", "cash", "current_assets",
+                "non_current_assets", "liabilities", "debt",
+                "current_liabilities", "non_current_liabilities",
+                "liabilities_and_equity", "equity", "income",
+                "earnings_per_share", "comprehensive_income",
+                "changes_in_equity", "cash_flow" and "added_value".
+            acc_level: Detail level to show for account codes. Options are 2,
+                3, 4 or None. Defaults to None.
+                    None -> X...       (default: show all accounts)
+                    2    -> X.YY       (show 2 levels)
+                    3    -> X.YY.ZZ    (show 3 levels)
+                    4    -> X.YY.ZZ.WW (show 4 levels)
+            num_years: Number of years to include in the report. Defaults to 0
+                (all years).
 
-        Parameters
-        ----------
-        report_type : {'assets', 'liabilities_and_equity', 'liabilities',
-            'equity', 'income', 'cash_flow'}
-            Report type to be generated.
-        acc_level : {None, 2, 3, 4}, default None
-            Detail level to show for account codes.
-            acc_level = None -> X...       (default: show all accounts)
-            acc_level = 2    -> X.YY       (show 2 levels)
-            acc_level = 3    -> X.YY.ZZ    (show 3 levels)
-            acc_level = 4    -> X.YY.ZZ.WW (show 4 levels)
-        num_years : int, default 0
-            Select how many last years to show where 0 -> show all years
-
-        Returns
-        ------
-        pandas.DataFrame
-
-        Raises
-        ------
-        ValueError
-            * If ``report_type`` attribute is invalid
-            * If ``acc_level`` attribute is invalid
+        Returns:
+            pd.DataFrame: Generated financial report as a pandas DataFrame.
+
+        Raises:
+            ValueError: If some argument is invalid.
         """
         # Check input arguments.
         if acc_level not in {None, 2, 3, 4}:
             raise ValueError("acc_level expects None, 2, 3 or 4")
 
         df = self._COMP_DF.query("acc_method == @self._acc_method").copy()
 
         # Set language
-
         class MyDict(dict):
             """Custom dictionary class to return key if key is not found."""
 
             def __missing__(self, key):
                 return "(pt) " + key
 
         if self._language == "English":
@@ -369,15 +355,14 @@
             "liabilities": ["2.01", "2.02"],
             "debt": ["2.01.04", "2.02.01"],
             "current_liabilities": ["2.01"],
             "non_current_liabilities": ["2.02"],
             "liabilities_and_equity": ["2"],
             "equity": ["2.03"],
             "income": ["3"],
-            # "earnings_per_share": ["3.99.01.01", "3.99.02.01"],
             "earnings_per_share": ["3.99"],
             "comprehensive_income": ["4"],
             "changes_in_equity": ["5"],
             "cash_flow": ["6"],
             "added_value": ["7"],
         }
         acc_codes = report_types[report_type]
@@ -435,30 +420,27 @@
         return pd.concat([df_annual, df_ttm], ignore_index=True)
 
     def custom_report(
         self,
         acc_list: list[str],
         num_years: int = 0,
     ) -> pd.DataFrame:
-        """
-        Return a financial report from custom list of accounting codes
+        """Generate a financial report from custom list of accounting codes
+
+        Args:
+            acc_list: A list of strings containg accounting codes to be used
+                in the report
+            num_years: Select how many years to show in the report.
+                Defaults to 0 (show all years)
 
-        Creates DataFrame object with a custom list of accounting codes
-        adjusted by function attributes
+        Returns:
+            pd.DataFrame: Generated financial report as a pandas DataFrame.
 
-        Parameters
-        ----------
-        acc_list : list[str]
-            A list of strings containg accounting codes to be used in report
-        num_years : int, default 0
-            Select how many last years to show where 0 -> show all years
-
-        Returns
-        -------
-        pandas.DataFrame
+        Raises:
+            ValueError: If some argument is invalid.
         """
         df_as = self.report("assets")
         df_le = self.report("liabilities_and_equity")
         df_is = self.report("income")
         df_cf = self.report("cash_flow")
         dfo = pd.concat([df_as, df_le, df_is, df_cf]).query("acc_code == @acc_list")
         # Show only selected years
@@ -474,34 +456,27 @@
         if is_prior:
             arr = s.iloc[:-1].values
             return np.append(np.nan, arr)
         else:
             return s
 
     def indicators(self, num_years: int = 0, is_prior: bool = True) -> pd.DataFrame:
-        """
-        Return company main operating indicators.
+        """Calculate the company main operating indicators.
+
+        Args:
+            num_years: Number of years to consider for calculation. If 0, use
+                all available years. Defaults to 0.
+            is_prior: Divide return measurements by book values from the end of
+                the prior year (see Damodaran reference). Defaults to True.
 
-        Creates DataFrame object with company operating indicators as
-        described in reference [1]
+        Returns:
+            pd.DataFrame: Dataframe containing calculated financial indicators.
 
-        Parameters
-        ----------
-        num_years : int, default 0
-            Select how many last years to show where 0 -> show all years
-        is_prior : bool, default True
-            Divide return measurements by book values from the end of the prior
-            year (see Damodaran reference).
-        Returns
-        -------
-        pandas.Dataframe
-
-        References
-        ----------
-        .. [1]  Aswath Damodaran, "Return on Capital (ROC), Return on Invested
+        References:
+            [1] Aswath Damodaran, "Return on Capital (ROC), Return on Invested
                 Capital (ROIC) and Return on Equity (ROE): Measurement and
                 Implications.", 2007,
                 https://people.stern.nyu.edu/adamodar/pdfoles/papers/returnmeasures.pdf
                 https://people.stern.nyu.edu/adamodar/New_Home_Page/datafile/variable.htm
         """
         df_as = self.report("assets")
         df_le = self.report("liabilities_and_equity")
```

### Comparing `FinLogic-0.3.4/finlogic/config.py` & `FinLogic-0.3.5/finlogic/config.py`

 * *Files identical despite different names*

### Comparing `FinLogic-0.3.4/finlogic/database.py` & `FinLogic-0.3.5/finlogic/database.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,15 @@
-"""Module containing local database functions."""
+"""Finlogic Database module.
+
+This module provides functions to handle financial data from the CVM Portal. It
+allows updating, processing and consolidating financial statements, as well as
+searching for company names in the FinLogic Database and retrieving information
+about the database itself.
+"""
+
 import os
 from pathlib import Path
 import shutil
 import math
 import zipfile
 from datetime import datetime
 from typing import List
@@ -19,15 +26,14 @@
 PROCESSED_DIR = c.DATA_PATH / "processed"
 INTERIM_DIR = c.DATA_PATH / "interim"
 CHECKMARK = "\033[32m\u2714\033[0m"
 
 
 def list_urls() -> List[str]:
     """Update the CVM Portal file base.
-
     Urls with CVM raw files:
     http://dados.cvm.gov.br/dados/CIA_ABERTA/DOC/DFP/DADOS/
     http://dados.cvm.gov.br/dados/CIA_ABERTA/DOC/ITR/DADOS/
     Links example:
     http://dados.cvm.gov.br/dados/CIA_ABERTA/DOC/DFP/DADOS/dfp_cia_aberta_2020.zip
     http://dados.cvm.gov.br/dados/CIA_ABERTA/DOC/ITR/DADOS/itr_cia_aberta_2020.zip
     Throughout 2021, there are already DFs for the year 2022 because the
@@ -91,16 +97,15 @@
         results = executor.map(update_raw_file, urls)
     c.cvm_df.to_pickle(c.CVM_DF_PATH)
     updated_raw_paths = [r for r in results if r is not None]
     return updated_raw_paths
 
 
 def process_raw_file(raw_path: Path) -> Path:
-    """
-    Read yearly raw file, process it, save the result and return a file path
+    """Read yearly raw file, process it, save the result and return a file path
     object.
     """
     df = pd.DataFrame()
     raw_zipfile = zipfile.ZipFile(raw_path)
     child_filenames = raw_zipfile.namelist()
 
     for child_filename in child_filenames[1:]:
@@ -150,86 +155,86 @@
         return
 
     for filename in processed_filenames:
         updated_df = pd.read_pickle(PROCESSED_DIR / filename)
         c.main_df = pd.concat([c.main_df, updated_df], ignore_index=True)
     c.main_df = c.main_df.astype("category")
     # Keep only the newest 'report_version' in df if values are repeated
-    # print(len(main_df.index))
     cols = [
         "cvm_id",
         "report_type",
         "period_reference",
         "report_version",
         "period_order",
         "acc_method",
         "acc_code",
     ]
     c.main_df.sort_values(by=cols, ignore_index=True, inplace=True)
     cols = list(c.main_df.columns)
     cols_remove = ["report_version", "acc_value", "acc_fixed"]
     [cols.remove(col) for col in cols_remove]
-    # tmp = main_df[main_df.duplicated(cols, keep=False)]
     # Ascending order --> last is the newest report_version
     c.main_df.drop_duplicates(cols, keep="last", inplace=True)
-    # print(len(main_df.index))
     c.main_df.to_pickle(c.MAIN_DF_PATH)
 
 
 def search_company(expression: str) -> pd.DataFrame:
-    """
-    Search companies names in database that contains the ```expression```
+    """Search for company names in the FinLogic Database containing a given expression.
 
-    Parameters
-    ----------
-    expression : str
-        A expression to search in as fi column 'co_name'.
-
-    Returns
-    -------
-    pd.DataFrame with search results
+    This function searches the 'co_name' column in the FinLogic Database for company names
+    that contain the provided expression. It returns a DataFrame containing the search
+    results, with each row representing a unique company that matches the search criteria.
+
+    Args:
+        expression (str): A string to search for in the FinLogic Database 'co_name' column.
+
+    Returns:
+        pd.DataFrame: A DataFrame containing the search results, with columns 'co_name',
+            'cvm_id', and 'fiscal_id' for each unique company that matches the search
+            criteria.
     """
     expression = expression.upper()
     df = (
         c.main_df.query("co_name.str.contains(@expression)")
         .sort_values(by="co_name")
         .drop_duplicates(subset="cvm_id", ignore_index=True)[
             ["co_name", "cvm_id", "fiscal_id"]
         ]
     )
     return df
 
 
 def database_info() -> pd.DataFrame:
-    """
-    Return information about FinLogic database
+    """Returns general information about FinLogic Database.
 
-    Returns
-    -------
-    pd.DataFrame
+    This function generates a pandas DataFrame containing various information
+    about the FinLogic database, such as the database path, file size, last
+    update call, last modified dates, size in memory, number of accounting rows,
+    unique accounting codes, companies, unique financial statements, first
+    financial statement date, and last financial statement date.
+
+    Returns:
+        pd.DataFrame: A DataFrame containing the FinLogic Database information.
     """
     if c.main_df.empty:
         print("There is no data in database")
         return
     info_df = pd.DataFrame()
     info_df.index.name = "FinLogic Database Info"
     info_df["Value"] = ""
     info_df.loc["Database Path"] = c.DATA_PATH
     info_df.loc["File Size (MB)"] = round(
         c.MAIN_DF_PATH.lstat().st_size / (1024 * 1024), 1
     )
     info_df.loc["Last Update Call"] = c.cvm_df.index.max().round("1s").tz_localize(None)
-
     # Convert python datetime to Pandas Timestamp
     last_modified_python = datetime.fromtimestamp(c.MAIN_DF_PATH.lstat().st_mtime)
     last_modified_pandas = pd.to_datetime(last_modified_python).round("1s")
     info_df.loc["Finlogic Last Modified"] = last_modified_pandas
-
     info_df.loc["CVM Last Update"] = c.cvm_df["last_modified"].max().tz_localize(None)
-
     info_df.loc["Size in Memory (MB)"] = round(
         c.main_df.memory_usage(index=True, deep=True).sum() / (1024 * 1024), 1
     )
     info_df.loc["Accounting Rows"] = len(c.main_df.index)
     info_df.loc["Unique Accounting Codes"] = c.main_df["acc_code"].nunique()
     info_df.loc["Companies"] = c.main_df["cvm_id"].nunique()
     columns_duplicates = ["cvm_id", "report_version", "report_type", "period_reference"]
@@ -244,69 +249,58 @@
     )
     return info_df
 
 
 def update_database(
     reset_data: bool = False, asynchronous: bool = False, cpu_usage: float = 0.75
 ):
-    """
-    Create/Update all remote files (raw files) and process them for local data
+    """Create/Update all remote files (raw files) and process them for local data
     access.
 
-    Parameters
-    ----------
-    reset_data: bool, default True
-        Delete all raw files and force a full database recompilation
-    asynchronous: bool, default False
-        Generate database by processing raw files asynchronously. Works only on Linux
-        and Mac
-    cpu_usage: float, default 0.75
-        A number between 0 and 1, where 1 represents 100% CPU usage. This
-        argument will define the number of cpu cores used for data processing when
-        function asynchronous mode is set to 'True'.
-
-    Returns
-    -------
-    None
+    Args:
+        reset_data: Delete all raw files and force a full database recompilation. Default
+            is False.
+        asynchronous: Generate the database by processing raw files asynchronously.
+            Works only on Linux and Mac. Default is False.
+        cpu_usage: A number between 0 and 1, where 1 represents 100% CPU usage. This
+            argument will define the number of cpu cores used for data processing when
+            function asynchronous mode is set to 'True'. Default is 0.75.
+
+    Returns:
+        None
     """
     # Parameter 'reset_data'-> delete, if they exist, data folders
     if reset_data:
         if Path.exists(c.DATA_PATH):
             shutil.rmtree(c.DATA_PATH)
         c.main_df = pd.DataFrame()
-
     # create data folders if they do not exist
     Path.mkdir(RAW_DIR, parents=True, exist_ok=True)
     Path.mkdir(PROCESSED_DIR, parents=True, exist_ok=True)
-
     # Define the number of cpu cores for parallel data processing
     workers = math.trunc(os.cpu_count() * cpu_usage)
     if workers < 1:
         workers = 1
-
     print("Updating financial statements...")
     urls = list_urls()
     raw_paths = update_raw_files(urls)
     print(f"Number of financial statements updated = {len(raw_paths)}")
     print("\nProcessing financial statements...")
     processed_filenames = process_raw_files(
         workers, raw_paths, asynchronous=asynchronous
     )
     print("\nConsolidating processed files...")
     consolidate_main_df(processed_filenames)
-
     print('Updating "language" database...')
     process_language_df()
-
     print(f"{CHECKMARK} FinLogic database updated!")
 
 
 def process_raw_df(df: pd.DataFrame) -> pd.DataFrame:
     """Process a raw dataframe"""
-
     columns_translation = {
         "CD_CVM": "cvm_id",
         "CNPJ_CIA": "fiscal_id",
         "DENOM_CIA": "co_name",
         "VERSAO": "report_version",
         "DT_INI_EXERC": "period_begin",
         "DT_FIM_EXERC": "period_end",
@@ -317,45 +311,38 @@
         "ST_CONTA_FIXA": "acc_fixed",
         "VL_CONTA": "acc_value",
         "COLUNA_DF": "equity_statement_column",
         "MOEDA": "currency",
         "ESCALA_MOEDA": "currency_unit",
     }
     df.rename(columns=columns_translation, inplace=True)
-
     # df['report_version'].unique() -> ['3', '2', '4', '1', '7', '5', '6', '9', '8']
     df["report_version"] = df["report_version"].astype(np.int8)
     df["cvm_id"] = df["cvm_id"].astype(np.int32)  # max < 600_000
     df["acc_value"] = df["acc_value"].astype(float)
-
     # df['currency'].value_counts() -> REAL    43391302
     df.drop(columns=["currency"], inplace=True)
-
     # df['currency_unit'].value_counts()
     #   MIL        40483230
     #   UNIDADE     2908072
     df["currency_unit"] = df["currency_unit"].map({"MIL": 1000, "UNIDADE": 1})
-
     # Unit base currency.
     df["acc_codes_level"] = df["acc_code"].str[0:4]
     # Do not adjust earnings per share rows (account codes 3.99...)
     df["acc_value"] = np.where(
         df.acc_codes_level == "3.99",
         df["acc_value"],
         df["acc_value"] * df["currency_unit"],
     )
     df.drop(columns=["currency_unit", "acc_codes_level"], inplace=True)
-
     # df['acc_fixed'].unique() -> ['S', 'N']
     df["acc_fixed"] = df["acc_fixed"].map({"S": True, "N": False})
-
     # df['period_order'].unique() -> ['PENÚLTIMO', 'ÚLTIMO']
     df["period_order"] = df["period_order"].map({"ÚLTIMO": 0, "PENÚLTIMO": -1})
     df["period_order"] = df["period_order"].astype(np.int8)
-
     df["period_reference"] = pd.to_datetime(df["period_reference"])
     df["period_end"] = pd.to_datetime(df["period_end"])
     # BPA, BPP and DFC files have no period_begin column.
     if "period_begin" in df.columns:
         df["period_begin"] = pd.to_datetime(df["period_begin"])
     else:
         # column_order.remove('period_begin')
@@ -386,23 +373,20 @@
     if == 'Ind' -> separate statement
     """
     df["acc_method"] = (
         df["GRUPO_DFP"].str[3:6].map({"Con": "consolidated", "Ind": "separate"})
     )
     # 'GRUPO_DFP' data can be inferred from 'acc_method' and report_type
     df.drop(columns=["GRUPO_DFP"], inplace=True)
-
     # Correct/harmonize some account texts.
     df.replace(to_replace=["\xa0ON\xa0", "On"], value="ON", inplace=True)
-
     # Remove duplicated accounts
     cols = list(df.columns)
     cols.remove("acc_value")
     df.drop_duplicates(cols, keep="last", inplace=True)
-
     columns_order = [
         "co_name",
         "cvm_id",
         "fiscal_id",
         "report_type",
         "report_version",
         "period_reference",
@@ -413,15 +397,14 @@
         "acc_name",
         "acc_method",
         "acc_fixed",
         "acc_value",
         "equity_statement_column",
     ]
     df = df[columns_order]
-
     return df
 
 
 def process_language_df():
     """Process language dataframe."""
     language_df = pd.read_csv(URL_LANGUAGE)
     Path.mkdir(INTERIM_DIR, parents=True, exist_ok=True)
```

### Comparing `FinLogic-0.3.4/pyproject.toml` & `FinLogic-0.3.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
     "pandas>=1.4.0",
     "requests>=2.27.0",
     "zstandard>=0.17.0",
 ]
-version = "0.3.4"
+version = "0.3.5"
 
 [project.license]
 file = "LICENSE"
 
 [project.optional-dependencies]
 test = [
     "pytest>=7.0.0",
```

### Comparing `FinLogic-0.3.4/tests/test_company.py` & `FinLogic-0.3.5/tests/test_company.py`

 * *Files identical despite different names*

### Comparing `FinLogic-0.3.4/tests/test_database.py` & `FinLogic-0.3.5/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `FinLogic-0.3.4/PKG-INFO` & `FinLogic-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FinLogic
-Version: 0.3.4
+Version: 0.3.5
 Summary: Finance toolkit for listed Brazilian companies
 Keywords: pandas, cvm, finance, investment, accounting
 Author-email: Carlos Carvalho <cr.cj@outlook.com>
 Requires-Python: >=3.10
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: FinLogic Version: 0.3.4 Summary: Finance toolkit
+Metadata-Version: 2.1 Name: FinLogic Version: 0.3.5 Summary: Finance toolkit
 for listed Brazilian companies Keywords: pandas, cvm, finance, investment,
 accounting Author-email: Carlos Carvalho
 cj@outlook.com> Requires-Python: >=3.10 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Classifier: Topic :: Office/Business ::
 Financial :: Accounting Classifier: Topic :: Office/Business :: Financial ::
 Investment Provides-Extra: test Project-URL: repository, https://github.com/
```

