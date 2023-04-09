# Comparing `tmp/lunchable-0.5.0.tar.gz` & `tmp/lunchable-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lunchable-0.5.0.tar", max compression
+gzip compressed data, was "lunchable-0.5.1.tar", max compression
```

## Comparing `lunchable-0.5.0.tar` & `lunchable-0.5.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     1071 2023-03-08 21:03:51.758115 lunchable-0.5.0/LICENSE
--rw-r--r--   0        0        0     2215 2023-03-08 21:03:51.758115 lunchable-0.5.0/README.md
--rw-r--r--   0        0        0      537 2023-03-08 21:03:51.758115 lunchable-0.5.0/lunchable/__init__.py
--rw-r--r--   0        0        0       98 2023-03-08 21:03:51.758115 lunchable-0.5.0/lunchable/__main__.py
--rw-r--r--   0        0        0    12499 2023-03-08 21:03:51.758115 lunchable-0.5.0/lunchable/_cli.py
--rw-r--r--   0        0        0      160 2023-03-08 21:03:51.758115 lunchable-0.5.0/lunchable/_config/__init__.py
--rw-r--r--   0        0        0     4687 2023-03-08 21:03:51.758115 lunchable-0.5.0/lunchable/_config/api_config.py
--rw-r--r--   0        0        0      379 2023-03-08 21:03:51.758115 lunchable-0.5.0/lunchable/_config/file_config.py
--rw-r--r--   0        0        0     2216 2023-03-08 21:03:51.758115 lunchable-0.5.0/lunchable/_config/logging_config.py
--rw-r--r--   0        0        0      147 2023-03-08 21:03:51.758115 lunchable-0.5.0/lunchable/_version.py
--rw-r--r--   0        0        0      502 2023-03-08 21:03:51.758115 lunchable-0.5.0/lunchable/exceptions.py
--rw-r--r--   0        0        0      917 2023-03-08 21:03:51.758115 lunchable-0.5.0/lunchable/models/__init__.py
--rw-r--r--   0        0        0      322 2023-03-08 21:03:51.758115 lunchable-0.5.0/lunchable/models/_base.py
--rw-r--r--   0        0        0     6250 2023-03-08 21:03:51.758115 lunchable-0.5.0/lunchable/models/_core.py
--rw-r--r--   0        0        0     1895 2023-03-08 21:03:51.758115 lunchable-0.5.0/lunchable/models/_lunchmoney.py
--rw-r--r--   0        0        0     9126 2023-03-08 21:03:51.758115 lunchable-0.5.0/lunchable/models/assets.py
--rw-r--r--   0        0        0     6752 2023-03-08 21:03:51.758115 lunchable-0.5.0/lunchable/models/budgets.py
--rw-r--r--   0        0        0    15170 2023-03-08 21:03:51.758115 lunchable-0.5.0/lunchable/models/categories.py
--rw-r--r--   0        0        0     5188 2023-03-08 21:03:51.758115 lunchable-0.5.0/lunchable/models/crypto.py
--rw-r--r--   0        0        0     4616 2023-03-08 21:03:51.758115 lunchable-0.5.0/lunchable/models/plaid_accounts.py
--rw-r--r--   0        0        0     6857 2023-03-08 21:03:51.758115 lunchable-0.5.0/lunchable/models/recurring_expenses.py
--rw-r--r--   0        0        0     1271 2023-03-08 21:03:51.762115 lunchable-0.5.0/lunchable/models/tags.py
--rw-r--r--   0        0        0    32901 2023-03-08 21:03:51.762115 lunchable-0.5.0/lunchable/models/transactions.py
--rw-r--r--   0        0        0     1535 2023-03-08 21:03:51.762115 lunchable-0.5.0/lunchable/models/user.py
--rw-r--r--   0        0        0      220 2023-03-08 21:03:51.762115 lunchable-0.5.0/lunchable/plugins/__init__.py
--rw-r--r--   0        0        0      205 2023-03-08 21:03:51.762115 lunchable-0.5.0/lunchable/plugins/base/__init__.py
--rw-r--r--   0        0        0    12165 2023-03-08 21:03:51.762115 lunchable-0.5.0/lunchable/plugins/base/base_app.py
--rw-r--r--   0        0        0     1598 2023-03-08 21:03:51.762115 lunchable-0.5.0/lunchable/plugins/base/pandas_app.py
--rw-r--r--   0        0        0     2809 2023-03-08 21:03:51.762115 lunchable-0.5.0/lunchable/plugins/primelunch/README.md
--rw-r--r--   0        0        0       26 2023-03-08 21:03:51.762115 lunchable-0.5.0/lunchable/plugins/primelunch/__init__.py
--rw-r--r--   0        0        0    14911 2023-03-08 21:03:51.762115 lunchable-0.5.0/lunchable/plugins/primelunch/primelunch.py
--rw-r--r--   0        0        0     2104 2023-03-08 21:03:51.762115 lunchable-0.5.0/lunchable/plugins/pushlunch/README.md
--rw-r--r--   0        0        0      100 2023-03-08 21:03:51.762115 lunchable-0.5.0/lunchable/plugins/pushlunch/__init__.py
--rw-r--r--   0        0        0    11661 2023-03-08 21:03:51.762115 lunchable-0.5.0/lunchable/plugins/pushlunch/pushover.py
--rw-r--r--   0        0        0     1707 2023-03-08 21:03:51.762115 lunchable-0.5.0/lunchable/plugins/splitlunch/README.md
--rw-r--r--   0        0        0      230 2023-03-08 21:03:51.762115 lunchable-0.5.0/lunchable/plugins/splitlunch/__init__.py
--rw-r--r--   0        0        0      320 2023-03-08 21:03:51.762115 lunchable-0.5.0/lunchable/plugins/splitlunch/_config.py
--rw-r--r--   0        0        0      150 2023-03-08 21:03:51.762115 lunchable-0.5.0/lunchable/plugins/splitlunch/exceptions.py
--rw-r--r--   0        0        0    49826 2023-03-08 21:03:51.762115 lunchable-0.5.0/lunchable/plugins/splitlunch/lunchmoney_splitwise.py
--rw-r--r--   0        0        0      624 2023-03-08 21:03:51.762115 lunchable-0.5.0/lunchable/plugins/splitlunch/models.py
--rw-r--r--   0        0        0        0 2023-03-08 21:03:51.762115 lunchable-0.5.0/lunchable/py.typed
--rw-r--r--   0        0        0     1800 2023-03-08 21:03:51.762115 lunchable-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     4063 1970-01-01 00:00:00.000000 lunchable-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-09 16:23:36.735018 lunchable-0.5.1/LICENSE
+-rw-r--r--   0        0        0     2215 2023-04-09 16:23:36.735018 lunchable-0.5.1/README.md
+-rw-r--r--   0        0        0      537 2023-04-09 16:23:36.735018 lunchable-0.5.1/lunchable/__init__.py
+-rw-r--r--   0        0        0       98 2023-04-09 16:23:36.735018 lunchable-0.5.1/lunchable/__main__.py
+-rw-r--r--   0        0        0    12499 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/_cli.py
+-rw-r--r--   0        0        0      160 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/_config/__init__.py
+-rw-r--r--   0        0        0     4687 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/_config/api_config.py
+-rw-r--r--   0        0        0      379 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/_config/file_config.py
+-rw-r--r--   0        0        0     2216 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/_config/logging_config.py
+-rw-r--r--   0        0        0      147 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/_version.py
+-rw-r--r--   0        0        0      502 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/exceptions.py
+-rw-r--r--   0        0        0      917 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/models/__init__.py
+-rw-r--r--   0        0        0      322 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/models/_base.py
+-rw-r--r--   0        0        0     6250 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/models/_core.py
+-rw-r--r--   0        0        0     1895 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/models/_lunchmoney.py
+-rw-r--r--   0        0        0     9126 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/models/assets.py
+-rw-r--r--   0        0        0     6752 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/models/budgets.py
+-rw-r--r--   0        0        0    15170 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/models/categories.py
+-rw-r--r--   0        0        0     5188 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/models/crypto.py
+-rw-r--r--   0        0        0     4626 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/models/plaid_accounts.py
+-rw-r--r--   0        0        0     6857 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/models/recurring_expenses.py
+-rw-r--r--   0        0        0     1271 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/models/tags.py
+-rw-r--r--   0        0        0    32901 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/models/transactions.py
+-rw-r--r--   0        0        0     1535 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/models/user.py
+-rw-r--r--   0        0        0      220 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/plugins/__init__.py
+-rw-r--r--   0        0        0      205 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/plugins/base/__init__.py
+-rw-r--r--   0        0        0    12165 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/plugins/base/base_app.py
+-rw-r--r--   0        0        0     1598 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/plugins/base/pandas_app.py
+-rw-r--r--   0        0        0     2809 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/plugins/primelunch/README.md
+-rw-r--r--   0        0        0       26 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/plugins/primelunch/__init__.py
+-rw-r--r--   0        0        0    14911 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/plugins/primelunch/primelunch.py
+-rw-r--r--   0        0        0     2104 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/plugins/pushlunch/README.md
+-rw-r--r--   0        0        0      100 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/plugins/pushlunch/__init__.py
+-rw-r--r--   0        0        0    11661 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/plugins/pushlunch/pushover.py
+-rw-r--r--   0        0        0     1707 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/plugins/splitlunch/README.md
+-rw-r--r--   0        0        0      230 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/plugins/splitlunch/__init__.py
+-rw-r--r--   0        0        0      320 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/plugins/splitlunch/_config.py
+-rw-r--r--   0        0        0      150 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/plugins/splitlunch/exceptions.py
+-rw-r--r--   0        0        0    49826 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/plugins/splitlunch/lunchmoney_splitwise.py
+-rw-r--r--   0        0        0      624 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/plugins/splitlunch/models.py
+-rw-r--r--   0        0        0        0 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/py.typed
+-rw-r--r--   0        0        0     1800 2023-04-09 16:23:36.739018 lunchable-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     4063 1970-01-01 00:00:00.000000 lunchable-0.5.1/PKG-INFO
```

### Comparing `lunchable-0.5.0/LICENSE` & `lunchable-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lunchable-0.5.0/README.md` & `lunchable-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `lunchable-0.5.0/lunchable/__init__.py` & `lunchable-0.5.1/lunchable/__init__.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.5.0/lunchable/_cli.py` & `lunchable-0.5.1/lunchable/_cli.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.5.0/lunchable/_config/api_config.py` & `lunchable-0.5.1/lunchable/_config/api_config.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.5.0/lunchable/_config/logging_config.py` & `lunchable-0.5.1/lunchable/_config/logging_config.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.5.0/lunchable/models/__init__.py` & `lunchable-0.5.1/lunchable/models/__init__.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.5.0/lunchable/models/_core.py` & `lunchable-0.5.1/lunchable/models/_core.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.5.0/lunchable/models/_lunchmoney.py` & `lunchable-0.5.1/lunchable/models/_lunchmoney.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.5.0/lunchable/models/assets.py` & `lunchable-0.5.1/lunchable/models/assets.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.5.0/lunchable/models/budgets.py` & `lunchable-0.5.1/lunchable/models/budgets.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.5.0/lunchable/models/categories.py` & `lunchable-0.5.1/lunchable/models/categories.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.5.0/lunchable/models/crypto.py` & `lunchable-0.5.1/lunchable/models/crypto.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.5.0/lunchable/models/plaid_accounts.py` & `lunchable-0.5.1/lunchable/models/plaid_accounts.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     """
 
     id: int = Field(description="Unique identifier of Plaid account")
     date_linked: datetime.date = Field(description=_date_linked_description)
     name: str = Field(description=_name_description)
     type: str = Field(description=_type_description)
     subtype: str = Field(description=_subtype_description)
-    mask: str = Field(description=_mask_description)
+    mask: Optional[str] = Field(description=_mask_description)
     institution_name: str = Field(description=_institution_name_description)
     status: str = Field(description=_status_description)
     last_import: Optional[datetime.datetime] = Field(
         description=_last_import_description
     )
     balance: Optional[float] = Field(description=_balance_description)
     currency: str = Field(description=_currency_description)
```

### Comparing `lunchable-0.5.0/lunchable/models/recurring_expenses.py` & `lunchable-0.5.1/lunchable/models/recurring_expenses.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.5.0/lunchable/models/tags.py` & `lunchable-0.5.1/lunchable/models/tags.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.5.0/lunchable/models/transactions.py` & `lunchable-0.5.1/lunchable/models/transactions.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.5.0/lunchable/models/user.py` & `lunchable-0.5.1/lunchable/models/user.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.5.0/lunchable/plugins/base/base_app.py` & `lunchable-0.5.1/lunchable/plugins/base/base_app.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.5.0/lunchable/plugins/base/pandas_app.py` & `lunchable-0.5.1/lunchable/plugins/base/pandas_app.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.5.0/lunchable/plugins/primelunch/README.md` & `lunchable-0.5.1/lunchable/plugins/primelunch/README.md`

 * *Files identical despite different names*

### Comparing `lunchable-0.5.0/lunchable/plugins/primelunch/primelunch.py` & `lunchable-0.5.1/lunchable/plugins/primelunch/primelunch.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.5.0/lunchable/plugins/pushlunch/README.md` & `lunchable-0.5.1/lunchable/plugins/pushlunch/README.md`

 * *Files identical despite different names*

### Comparing `lunchable-0.5.0/lunchable/plugins/pushlunch/pushover.py` & `lunchable-0.5.1/lunchable/plugins/pushlunch/pushover.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.5.0/lunchable/plugins/splitlunch/README.md` & `lunchable-0.5.1/lunchable/plugins/splitlunch/README.md`

 * *Files identical despite different names*

### Comparing `lunchable-0.5.0/lunchable/plugins/splitlunch/lunchmoney_splitwise.py` & `lunchable-0.5.1/lunchable/plugins/splitlunch/lunchmoney_splitwise.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.5.0/lunchable/plugins/splitlunch/models.py` & `lunchable-0.5.1/lunchable/plugins/splitlunch/models.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.5.0/pyproject.toml` & `lunchable-0.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 documentation = "https://juftin.github.io/lunchable"
 homepage = "https://github.com/juftin/lunchable"
 include = ["lunchable/py.typed"]
 license = "MIT"
 name = "lunchable"
 readme = "README.md"
 repository = "https://github.com/juftin/lunchable"
-version = "0.5.0"
+version = "0.5.1"
 
 [tool.poetry.dependencies]
 click = ">=8.0.1"
 pandas = {version = "^1.3", optional = true}
 pydantic = ">=1.2.0,<2.0.0"
 python = ">=3.7.1,<4.0"
 python-dateutil = {version = "^2.8.2", optional = true}
```

### Comparing `lunchable-0.5.0/PKG-INFO` & `lunchable-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lunchable
-Version: 0.5.0
+Version: 0.5.1
 Summary: A simple Python SDK around the Lunch Money Developer API
 Home-page: https://github.com/juftin/lunchable
 License: MIT
 Author: Justin Flannery
 Author-email: juftin@juftin.com
 Requires-Python: >=3.7.1,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lunchable Version: 0.5.0 Summary: A simple Python
+Metadata-Version: 2.1 Name: lunchable Version: 0.5.1 Summary: A simple Python
 SDK around the Lunch Money Developer API Home-page: https://github.com/juftin/
 lunchable License: MIT Author: Justin Flannery Author-email: juftin@juftin.com
 Requires-Python: >=3.7.1,<4.0 Classifier: Development Status :: 5 - Production/
 Stable Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```

