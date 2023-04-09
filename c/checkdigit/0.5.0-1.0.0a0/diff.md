# Comparing `tmp/checkdigit-0.5.0.tar.gz` & `tmp/checkdigit-1.0.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "checkdigit-0.5.0.tar", max compression
+gzip compressed data, was "checkdigit-1.0.0a0.tar", last modified: Sat Nov 28 19:40:25 2020, max compression
```

## Comparing `checkdigit-0.5.0.tar` & `checkdigit-1.0.0a0.tar`

### file list

```diff
@@ -1,13 +1,11 @@
--rw-r--r--   0        0        0    35149 2022-04-06 16:07:34.860237 checkdigit-0.5.0/LICENSE
--rw-r--r--   0        0        0     4209 2023-04-09 11:22:58.080936 checkdigit-0.5.0/PYPIREADME.rst
--rw-r--r--   0        0        0     1036 2022-04-06 16:07:34.918039 checkdigit-0.5.0/checkdigit/__init__.py
--rw-r--r--   0        0        0     5390 2023-04-09 10:45:32.974244 checkdigit-0.5.0/checkdigit/_data.py
--rw-r--r--   0        0        0     4258 2023-01-15 16:54:22.458165 checkdigit-0.5.0/checkdigit/crc.py
--rw-r--r--   0        0        0     3508 2022-04-06 16:07:34.918304 checkdigit-0.5.0/checkdigit/gs1.py
--rw-r--r--   0        0        0     3514 2023-04-09 10:45:32.974424 checkdigit-0.5.0/checkdigit/isbn.py
--rw-r--r--   0        0        0     3160 2022-04-06 16:07:34.918447 checkdigit-0.5.0/checkdigit/luhn.py
--rw-r--r--   0        0        0     3119 2022-04-06 16:07:34.918506 checkdigit-0.5.0/checkdigit/parity.py
--rw-r--r--   0        0        0       56 2022-04-06 16:07:34.918556 checkdigit-0.5.0/checkdigit/py.typed
--rw-r--r--   0        0        0     3521 2022-04-06 16:07:34.918633 checkdigit-0.5.0/checkdigit/verhoeff.py
--rw-r--r--   0        0        0     1365 2023-04-09 12:26:24.380991 checkdigit-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     5344 1970-01-01 00:00:00.000000 checkdigit-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2020-11-24 12:09:40.642008 checkdigit-1.0.0a0/LICENSE
+-rw-r--r--   0        0        0     1908 2020-11-28 18:46:25.015274 checkdigit-1.0.0a0/README.md
+-rw-r--r--   0        0        0      683 2020-11-28 11:51:22.296128 checkdigit-1.0.0a0/checkdigit/__init__.py
+-rw-r--r--   0        0        0     1055 2020-11-27 19:55:25.438989 checkdigit-1.0.0a0/checkdigit/data.py
+-rw-r--r--   0        0        0     3566 2020-11-28 19:12:04.616013 checkdigit-1.0.0a0/checkdigit/isbn.py
+-rw-r--r--   0        0        0     2548 2020-11-28 10:41:10.772029 checkdigit-1.0.0a0/checkdigit/luhn.py
+-rw-r--r--   0        0        0     1274 2020-11-28 19:30:25.984037 checkdigit-1.0.0a0/checkdigit/parity.py
+-rw-r--r--   0        0        0     1580 2020-11-27 20:21:21.444436 checkdigit-1.0.0a0/checkdigit/upc.py
+-rw-r--r--   0        0        0      997 2020-11-28 15:24:11.141699 checkdigit-1.0.0a0/pyproject.toml
+-rw-r--r--   0        0        0     2535 2020-11-28 19:40:26.066515 checkdigit-1.0.0a0/setup.py
+-rw-r--r--   0        0        0     2853 2020-11-28 19:40:26.066879 checkdigit-1.0.0a0/PKG-INFO
```

### Comparing `checkdigit-0.5.0/LICENSE` & `checkdigit-1.0.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `checkdigit-0.5.0/checkdigit/__init__.py` & `checkdigit-1.0.0a0/checkdigit/parity.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,16 +9,27 @@
 # checkdigit is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 # You should have received a copy of the GNU General Public License
 # along with checkdigit.  If not, see <http://www.gnu.org/licenses/>.
 
-"""An easy-to-use check digit library for data validation.
+from checkdigit.data import cleanse
 
-This Python library contains various functions relating to Luhn, ISBN, UPC and many other codes.
-It is able to validate blocks of data, as well as calulate missing digits and check digits.
 
-For more information, please look at the wiki page for this library:
-https://checkdigit.rtfd.io/
+# WARNING: Data beginning with 0 must be as a string due to PEP 3127
 
-"""
+
+def calculate(data: str, even: bool = True) -> str:
+    """Adds a parity bit onto the end of a block of data
+
+    Args:
+        data: A string containing binary digits
+        even: Whether to use even parity (otherwise uses odd parity)
+
+    Returns:
+        str: The original data with the parity bit added to the end
+    """
+    data = cleanse(data)
+    if (even and not data.count("1") % 2) or (not even and data.count("1") % 2):
+        return data + "0"
+    return data + "1"
```

### Comparing `checkdigit-0.5.0/checkdigit/isbn.py` & `checkdigit-1.0.0a0/checkdigit/isbn.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,102 +9,107 @@
 # checkdigit is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 # You should have received a copy of the GNU General Public License
 # along with checkdigit.  If not, see <http://www.gnu.org/licenses/>.
 
-"""International Standard Book Number.
+from checkdigit.data import cleanse, convert
 
-ISBN codes are product identifiers used predominantly for books.
-Support is provided for both ISBN-10 and ISBN-13.
 
-"""
+# WARNING: Data beginning with 0 must be as a string due to PEP 3127
 
-from checkdigit._data import cleanse, convert, missing_template
 
-
-def calculate(data: str) -> str:
-    """Calculates ISBN Check Digits.
+def calculate10(data: str) -> str:
+    """Calculates ISBN-10 Check Digit
 
     Args:
-        data: A string of characters representing an ISBN code without the check digit
+        data: A string of 9 characters
 
     Returns:
         str: The check digit that was missing
+    """
+    data = cleanse(data)
+    total_sum = 0
+    multiply_counter = 10
+    for item in data:
+        total_sum += int(item) * multiply_counter
+        multiply_counter -= 1  # Multiplies first digit by 10, second by 9...
+    check_digit = 11 - (total_sum % 11)
+    return convert(check_digit)
+
+
+def validate10(data: str) -> bool:
+    """Validates ISBN-10
+
+    Args:
+        data: A string of characters representing a full ISBN-10 code
+
+    Returns:
+        bool: A boolean representing whether the check digit validates the data or not
 
-    Examples:
-        >>> from checkdigit import isbn
-        >>> # ISBN-10
-        >>> isbn.calculate("043942089")
-        'X'
-        >>> # ISBN-13
-        >>> isbn.calculate("978-1-86197-876")
-        '9'
     """
     data = cleanse(data)
+    return (
+        calculate10(data[:9]) == data[-1]
+    )  # Determines if calculated Check Digit of the data is the last digit given
 
-    if len(data) == 9:
-        # ISBN 10 (without the check digit)
-        # Multiply first digit by 10, second by 9, ... and take the sum
-        total_sum = sum(
-            int(digit) * weight for digit, weight in zip(data, range(10, 0, -1))
-        )
-        return convert(11 - (total_sum % 11))
-    # elif not required since return above (and makes pylint happy)
-    if len(data) == 12:
-        # ISBN weights is 1 for odd positions and 3 for even
-        # Since there are 12 digits, multiply weights by 6
-        weights = (1, 3) * 6
-        # Multiply each digit by its weight
-        total_sum = sum(int(digit) * weight for digit, weight in zip(data, weights))
-        # Return final check digit and type of barcode
-        return convert(10 - (total_sum % 10), False)
-    return "Invalid"
 
+def calculate13(data: str, barcode: str = "isbn") -> str:
+    """Calculates ISBN-13 Check Digit
 
-def validate(data: str) -> bool:
-    """Validates ISBN check digits.
+    Args:
+        data: A string of 12 characters
+        barcode: The type of code (either isbn or upc)
+
+    Returns:
+        str: The check digit that was missing
+    """
+    data = cleanse(data)
+    mod_number = 0 if barcode == "isbn" else 1
+    total_sum = 0
+    position_counter = 1  # 1 based indexing for data
+    for item in data:
+        digit = int(item)
+        if position_counter % 2 == mod_number:
+            total_sum += digit * 3  # Multiplies by 3 if position is even
+        else:
+            total_sum += digit
+        position_counter += 1
+    final_value = 10 - (total_sum % 10)
+    return convert(final_value, barcode)
+
+
+def validate13(data: str) -> bool:
+    """Validates ISBN-13
 
     Args:
-        data: A string of characters representing a fall ISBN code
+        data: A string of characters representing a full ISBN-13 code
 
     Returns:
-        bool: A boolean representing whether the
-            check digit validates the data or non
+        bool: A boolean representing whether the check digit validates the data
 
-    Examples:
-        >>> from checkdigit import isbn
-        >>> # ISBN-10
-        >>> isbn.validate("0198526636")
-        True
-        >>> # ISBN-13
-        >>> isbn.validate("978-1-56619-909-4")
-        True
     """
-    # The calculate method already cleanses the data.
-    # If the return result is 'Invalid', it won't match the check digit (hence false).
-    return calculate(data[:-1]) == data[-1]
+    data = cleanse(data)
+    return calculate13(data[:12]) == data[-1]
 
 
 def missing(data: str) -> str:
-    """Calculates a missing digit in an ISBN Code represented by a question mark.
+    """Calculates a missing digit in an ISBN Code
 
     Args:
-        data: A string of characters representing a full ISBN code
-            with a question mark representing a missing character
+        data: A string of characters representing a full ISBN code with a question mark representing a missing character
 
     Returns:
         str: The missing value that should've been where the question mark was
 
-    Examples:
-        >>> from checkdigit import isbn
-        >>> # ISBN-10
-        >>> isbn.missing("15688?111X")
-        '1'
-        >>> # ISBN-13
-        >>> isbn.missing("978186197876?")
-        '9'
-        >>> isbn.missing("023456789128")
-        'Invalid'
     """
-    return missing_template(data, "isbn")
+    data = cleanse(data)
+    for poss_digit in range(11):  # Brute Force the 11 options
+        option = convert(poss_digit)
+        # Depending on the size of the data, the relevant validating function tests it with the generated number
+        # If this fails, the next number is tried
+        if (len(data) == 10 and validate10(data.replace("?", option))) or (
+            len(data) == 13 and validate13(data.replace("?", option))
+        ):
+            return option
+    return "Invalid"
```

