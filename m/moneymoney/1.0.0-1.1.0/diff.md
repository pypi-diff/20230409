# Comparing `tmp/moneymoney-1.0.0.tar.gz` & `tmp/moneymoney-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moneymoney-1.0.0.tar", last modified: Fri Mar 24 15:47:54 2023, max compression
+gzip compressed data, was "moneymoney-1.1.0.tar", last modified: Sun Apr  9 16:44:12 2023, max compression
```

## Comparing `moneymoney-1.0.0.tar` & `moneymoney-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 15:47:54.753380 moneymoney-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-24 15:47:44.000000 moneymoney-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-24 15:47:44.000000 moneymoney-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-03-24 15:47:54.753380 moneymoney-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-03-24 15:47:44.000000 moneymoney-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 15:47:54.753380 moneymoney-1.0.0/moneymoney/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 15:47:44.000000 moneymoney-1.0.0/moneymoney/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-03-24 15:47:44.000000 moneymoney-1.0.0/moneymoney/currency_codes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-03-24 15:47:44.000000 moneymoney-1.0.0/moneymoney/money.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 15:47:54.753380 moneymoney-1.0.0/moneymoney.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-03-24 15:47:54.000000 moneymoney-1.0.0/moneymoney.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-03-24 15:47:54.000000 moneymoney-1.0.0/moneymoney.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 15:47:54.000000 moneymoney-1.0.0/moneymoney.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-03-24 15:47:54.000000 moneymoney-1.0.0/moneymoney.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-24 15:47:54.000000 moneymoney-1.0.0/moneymoney.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-03-24 15:47:44.000000 moneymoney-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-24 15:47:54.753380 moneymoney-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:44:12.575771 moneymoney-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-09 16:43:59.000000 moneymoney-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-09 16:43:59.000000 moneymoney-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-04-09 16:44:12.575771 moneymoney-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-09 16:43:59.000000 moneymoney-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:44:12.571771 moneymoney-1.1.0/moneymoney/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 16:43:59.000000 moneymoney-1.1.0/moneymoney/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-09 16:43:59.000000 moneymoney-1.1.0/moneymoney/currency_codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-09 16:43:59.000000 moneymoney-1.1.0/moneymoney/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-04-09 16:43:59.000000 moneymoney-1.1.0/moneymoney/money.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-09 16:43:59.000000 moneymoney-1.1.0/moneymoney/presets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:44:12.575771 moneymoney-1.1.0/moneymoney.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-04-09 16:44:12.000000 moneymoney-1.1.0/moneymoney.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-09 16:44:12.000000 moneymoney-1.1.0/moneymoney.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 16:44:12.000000 moneymoney-1.1.0/moneymoney.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-09 16:44:12.000000 moneymoney-1.1.0/moneymoney.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-09 16:44:12.000000 moneymoney-1.1.0/moneymoney.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-04-09 16:43:59.000000 moneymoney-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-09 16:44:12.575771 moneymoney-1.1.0/setup.cfg
```

### Comparing `moneymoney-1.0.0/LICENSE` & `moneymoney-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `moneymoney-1.0.0/PKG-INFO` & `moneymoney-1.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: moneymoney
-Version: 1.0.0
+Version: 1.1.0
 Summary: Money package for Python
 Author: w0rmr1d3r
 License: GPLv3
 Project-URL: Homepage, https://github.com/w0rmr1d3r/moneymoney
 Project-URL: Repository, https://github.com/w0rmr1d3r/moneymoney
 Project-URL: Bug Tracker, https://github.com/w0rmr1d3r/moneymoney/issues
 Project-URL: Documentation, https://github.com/w0rmr1d3r/moneymoney
 Project-URL: Changelog, https://github.com/w0rmr1d3r/moneymoney/releases
 Project-URL: Funding, https://github.com/sponsors/w0rmr1d3r
-Keywords: currency,python,money
+Keywords: currency,python,money,finance
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -40,21 +40,29 @@
 pip install moneymoney
 ```
 
 ## Usage
 
 ```python
 from moneymoney.currency_codes import CurrencyCodes
+from moneymoney.defaults import ONE_EUR
 from moneymoney.money import Money
+from moneymoney.presets import EUR
 
 # using a string as currency code
 quantity = Money(amount=1000, currency_code="EUR")
 
 # using currency codes from this package
 quantity_two = Money(amount=1000, currency_code=CurrencyCodes.EUR)
+
+# using defaults
+my_price = ONE_EUR
+
+# using presets
+my_euro = EUR(amount=1.0)
 ```
 
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first
 to discuss what you would like to change.
```

### Comparing `moneymoney-1.0.0/README.md` & `moneymoney-1.1.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -13,21 +13,29 @@
 pip install moneymoney
 ```
 
 ## Usage
 
 ```python
 from moneymoney.currency_codes import CurrencyCodes
+from moneymoney.defaults import ONE_EUR
 from moneymoney.money import Money
+from moneymoney.presets import EUR
 
 # using a string as currency code
 quantity = Money(amount=1000, currency_code="EUR")
 
 # using currency codes from this package
 quantity_two = Money(amount=1000, currency_code=CurrencyCodes.EUR)
+
+# using defaults
+my_price = ONE_EUR
+
+# using presets
+my_euro = EUR(amount=1.0)
 ```
 
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first
 to discuss what you would like to change.
```

### Comparing `moneymoney-1.0.0/moneymoney/money.py` & `moneymoney-1.1.0/moneymoney/money.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,14 +9,22 @@
     """Exception thrown when currencies are different."""
 
 
 class OtherIsNotMoneyInstanceException(Exception):
     """Exception thrown when the other compared is not of Money instance."""
 
 
+class OtherIsMoneyInstanceException(Exception):
+    """Exception thrown when the other is of Money instance."""
+
+
+class OtherIsZeroException(Exception):
+    """Exception thrown when the other is equal to zero."""
+
+
 class Money:
     """Class representing an amount with a currency.
 
     Money of different currency cannot operate between them, they need
     to be of the same currency.
     """
 
@@ -37,30 +45,60 @@
         return self._currency_code
 
     @staticmethod
     def __assert_other_is_instance_money(other):
         if not isinstance(other, Money):
             raise OtherIsNotMoneyInstanceException()
 
+    @staticmethod
+    def __assert_other_is_not_instance_of_money(other):
+        if isinstance(other, Money):
+            raise OtherIsMoneyInstanceException()
+
     def __assert_currencies_are_the_same(self, other):
         if other.currency_code.lower() != self.currency_code.lower():
             raise CurrencyIsNotTheSameException()
 
+    @staticmethod
+    def __assert_other_is_not_zero(other):
+        if other == 0:
+            raise OtherIsZeroException()
+
     def __add__(self, other):
         self.__assert_other_is_instance_money(other)
         self.__assert_currencies_are_the_same(other)
         amount = self.amount + other.amount
         return self.__class__(amount=amount, currency_code=self.currency_code)
 
+    def __radd__(self, other):
+        return self.__add__(other)
+
     def __sub__(self, other):
         self.__assert_other_is_instance_money(other)
         self.__assert_currencies_are_the_same(other)
         amount = self.amount - other.amount
         return self.__class__(amount=amount, currency_code=self.currency_code)
 
+    def __mul__(self, other):
+        self.__assert_other_is_not_instance_of_money(other)
+        amount = self._amount * other
+        return self.__class__(amount=amount, currency_code=self.currency_code)
+
+    def __rmul__(self, other):
+        return self.__mul__(other)
+
+    def __truediv__(self, other):
+        self.__assert_other_is_not_instance_of_money(other)
+        self.__assert_other_is_not_zero(other)
+        amount = self._amount / other
+        return self.__class__(amount=amount, currency_code=self._currency_code)
+
+    def __hash__(self):
+        return hash((self._amount, self._currency_code))
+
     def __eq__(self, other):
         if isinstance(other, Money):
             return (self._amount == other.amount) and (self._currency_code.lower() == other.currency_code.lower())
         return False
 
     def __lt__(self, other):
         self.__assert_other_is_instance_money(other)
@@ -78,13 +116,23 @@
         return self._amount > other.amount
 
     def __ge__(self, other):
         self.__assert_other_is_instance_money(other)
         self.__assert_currencies_are_the_same(other)
         return self._amount >= other.amount
 
+    def __neg__(self):
+        return self.__class__(amount=-self._amount, currency_code=self._currency_code)
+
+    def __pos__(self):
+        return self.__class__(amount=+self._amount, currency_code=self._currency_code)
+
+    def __abs__(self):
+        return self.__class__(amount=abs(self._amount), currency_code=self._currency_code)
+
     def __str__(self):
         rounded_amount = round(self.amount, 2)
         return f"{rounded_amount}{self.currency_code}"
 
 
+# To be deprecated in next major version
 DEFAULT_MONEY = Money(currency_code=CurrencyCodes.EUR)
```

### Comparing `moneymoney-1.0.0/moneymoney.egg-info/PKG-INFO` & `moneymoney-1.1.0/moneymoney.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: moneymoney
-Version: 1.0.0
+Version: 1.1.0
 Summary: Money package for Python
 Author: w0rmr1d3r
 License: GPLv3
 Project-URL: Homepage, https://github.com/w0rmr1d3r/moneymoney
 Project-URL: Repository, https://github.com/w0rmr1d3r/moneymoney
 Project-URL: Bug Tracker, https://github.com/w0rmr1d3r/moneymoney/issues
 Project-URL: Documentation, https://github.com/w0rmr1d3r/moneymoney
 Project-URL: Changelog, https://github.com/w0rmr1d3r/moneymoney/releases
 Project-URL: Funding, https://github.com/sponsors/w0rmr1d3r
-Keywords: currency,python,money
+Keywords: currency,python,money,finance
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -40,21 +40,29 @@
 pip install moneymoney
 ```
 
 ## Usage
 
 ```python
 from moneymoney.currency_codes import CurrencyCodes
+from moneymoney.defaults import ONE_EUR
 from moneymoney.money import Money
+from moneymoney.presets import EUR
 
 # using a string as currency code
 quantity = Money(amount=1000, currency_code="EUR")
 
 # using currency codes from this package
 quantity_two = Money(amount=1000, currency_code=CurrencyCodes.EUR)
+
+# using defaults
+my_price = ONE_EUR
+
+# using presets
+my_euro = EUR(amount=1.0)
 ```
 
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first
 to discuss what you would like to change.
```

### Comparing `moneymoney-1.0.0/pyproject.toml` & `moneymoney-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -17,16 +17,16 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Software Development :: Libraries",
 ]
 # Make sure this matches the keywords in GitHub
-keywords = ["currency", "python", "money"]
-version = "1.0.0"
+keywords = ["currency", "python", "money", "finance"]
+version = "1.1.0"
 # Minumum supported version
 # If supporting newer versions, update ->  CI and classifiers
 # If minimum supported version changes, update -> CI, coverage, lint, release and classifiers.
 requires-python = ">=3.9.0"
 
 # Always try to be compatible with these versions and above
 dependencies = []
```

