# Comparing `tmp/flusso-0.0.1.tar.gz` & `tmp/flusso-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flusso-0.0.1.tar", last modified: Wed Apr  5 13:13:42 2023, max compression
+gzip compressed data, was "flusso-0.1.0.tar", last modified: Sun Apr  9 06:51:18 2023, max compression
```

## Comparing `flusso-0.0.1.tar` & `flusso-0.1.0.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxr-xr-x   0 tomiwaadey   (501) staff       (20)        0 2023-04-05 13:13:42.634552 flusso-0.0.1/
--rw-r--r--   0 tomiwaadey   (501) staff       (20)     1075 2023-03-29 21:20:14.000000 flusso-0.0.1/LICENSE
--rw-r--r--   0 tomiwaadey   (501) staff       (20)    22421 2023-04-05 13:13:42.633913 flusso-0.0.1/PKG-INFO
--rw-r--r--   0 tomiwaadey   (501) staff       (20)    21868 2023-04-05 09:31:08.000000 flusso-0.0.1/README.md
-drwxr-xr-x   0 tomiwaadey   (501) staff       (20)        0 2023-04-05 13:13:42.626736 flusso-0.0.1/flusso/
--rw-r--r--   0 tomiwaadey   (501) staff       (20)       97 2023-04-05 09:34:47.000000 flusso-0.0.1/flusso/__init__.py
--rw-r--r--   0 tomiwaadey   (501) staff       (20)      952 2023-04-05 09:48:00.000000 flusso-0.0.1/flusso/functions.py
--rw-r--r--   0 tomiwaadey   (501) staff       (20)     6433 2023-04-05 13:06:32.000000 flusso-0.0.1/flusso/option.py
-drwxr-xr-x   0 tomiwaadey   (501) staff       (20)        0 2023-04-05 13:13:42.630159 flusso-0.0.1/flusso/primitives/
--rw-r--r--   0 tomiwaadey   (501) staff       (20)        0 2023-04-01 04:29:14.000000 flusso-0.0.1/flusso/primitives/__init__.py
--rw-r--r--   0 tomiwaadey   (501) staff       (20)     4677 2023-04-05 10:08:03.000000 flusso-0.0.1/flusso/primitives/base.py
--rw-r--r--   0 tomiwaadey   (501) staff       (20)      652 2023-04-05 09:47:36.000000 flusso-0.0.1/flusso/primitives/exceptions.py
--rw-r--r--   0 tomiwaadey   (501) staff       (20)     6608 2023-04-05 13:08:17.000000 flusso-0.0.1/flusso/result.py
--rw-r--r--   0 tomiwaadey   (501) staff       (20)       78 2023-04-01 03:30:18.000000 flusso-0.0.1/flusso/types.py
-drwxr-xr-x   0 tomiwaadey   (501) staff       (20)        0 2023-04-05 13:13:42.628690 flusso-0.0.1/flusso.egg-info/
--rw-r--r--   0 tomiwaadey   (501) staff       (20)    22421 2023-04-05 13:13:42.000000 flusso-0.0.1/flusso.egg-info/PKG-INFO
--rw-r--r--   0 tomiwaadey   (501) staff       (20)      432 2023-04-05 13:13:42.000000 flusso-0.0.1/flusso.egg-info/SOURCES.txt
--rw-r--r--   0 tomiwaadey   (501) staff       (20)        1 2023-04-05 13:13:42.000000 flusso-0.0.1/flusso.egg-info/dependency_links.txt
--rw-r--r--   0 tomiwaadey   (501) staff       (20)       32 2023-04-05 13:13:42.000000 flusso-0.0.1/flusso.egg-info/requires.txt
--rw-r--r--   0 tomiwaadey   (501) staff       (20)       12 2023-04-05 13:13:42.000000 flusso-0.0.1/flusso.egg-info/top_level.txt
--rw-r--r--   0 tomiwaadey   (501) staff       (20)       38 2023-04-05 13:13:42.634761 flusso-0.0.1/setup.cfg
--rw-r--r--   0 tomiwaadey   (501) staff       (20)      908 2023-04-01 04:05:36.000000 flusso-0.0.1/setup.py
-drwxr-xr-x   0 tomiwaadey   (501) staff       (20)        0 2023-04-05 13:13:42.632836 flusso-0.0.1/test/
--rw-r--r--   0 tomiwaadey   (501) staff       (20)        0 2023-03-29 21:20:14.000000 flusso-0.0.1/test/__init__.py
--rw-r--r--   0 tomiwaadey   (501) staff       (20)      794 2023-04-05 09:43:08.000000 flusso-0.0.1/test/test_functions.py
--rw-r--r--   0 tomiwaadey   (501) staff       (20)     3303 2023-04-05 09:43:16.000000 flusso-0.0.1/test/test_option.py
--rw-r--r--   0 tomiwaadey   (501) staff       (20)     4303 2023-04-05 09:43:28.000000 flusso-0.0.1/test/test_result.py
+drwxr-xr-x   0 tomiwaadey   (501) staff       (20)        0 2023-04-09 06:51:18.291174 flusso-0.1.0/
+-rw-r--r--   0 tomiwaadey   (501) staff       (20)     1075 2023-03-29 21:20:14.000000 flusso-0.1.0/LICENSE
+-rw-r--r--   0 tomiwaadey   (501) staff       (20)    30441 2023-04-09 06:51:18.290738 flusso-0.1.0/PKG-INFO
+-rw-r--r--   0 tomiwaadey   (501) staff       (20)    29888 2023-04-09 06:41:35.000000 flusso-0.1.0/README.md
+drwxr-xr-x   0 tomiwaadey   (501) staff       (20)        0 2023-04-09 06:51:18.283492 flusso-0.1.0/flusso/
+-rw-r--r--   0 tomiwaadey   (501) staff       (20)       97 2023-04-05 09:34:47.000000 flusso-0.1.0/flusso/__init__.py
+-rw-r--r--   0 tomiwaadey   (501) staff       (20)     7128 2023-04-09 06:21:28.000000 flusso-0.1.0/flusso/async_result.py
+-rw-r--r--   0 tomiwaadey   (501) staff       (20)      952 2023-04-05 09:48:00.000000 flusso-0.1.0/flusso/functions.py
+-rw-r--r--   0 tomiwaadey   (501) staff       (20)     6433 2023-04-05 13:06:32.000000 flusso-0.1.0/flusso/option.py
+drwxr-xr-x   0 tomiwaadey   (501) staff       (20)        0 2023-04-09 06:51:18.286752 flusso-0.1.0/flusso/primitives/
+-rw-r--r--   0 tomiwaadey   (501) staff       (20)        0 2023-04-01 04:29:14.000000 flusso-0.1.0/flusso/primitives/__init__.py
+-rw-r--r--   0 tomiwaadey   (501) staff       (20)     4677 2023-04-06 19:29:12.000000 flusso-0.1.0/flusso/primitives/base.py
+-rw-r--r--   0 tomiwaadey   (501) staff       (20)      652 2023-04-05 09:47:36.000000 flusso-0.1.0/flusso/primitives/exceptions.py
+-rw-r--r--   0 tomiwaadey   (501) staff       (20)     6608 2023-04-05 13:08:17.000000 flusso-0.1.0/flusso/result.py
+-rw-r--r--   0 tomiwaadey   (501) staff       (20)       78 2023-04-01 03:30:18.000000 flusso-0.1.0/flusso/types.py
+drwxr-xr-x   0 tomiwaadey   (501) staff       (20)        0 2023-04-09 06:51:18.285526 flusso-0.1.0/flusso.egg-info/
+-rw-r--r--   0 tomiwaadey   (501) staff       (20)    30441 2023-04-09 06:51:18.000000 flusso-0.1.0/flusso.egg-info/PKG-INFO
+-rw-r--r--   0 tomiwaadey   (501) staff       (20)      481 2023-04-09 06:51:18.000000 flusso-0.1.0/flusso.egg-info/SOURCES.txt
+-rw-r--r--   0 tomiwaadey   (501) staff       (20)        1 2023-04-09 06:51:18.000000 flusso-0.1.0/flusso.egg-info/dependency_links.txt
+-rw-r--r--   0 tomiwaadey   (501) staff       (20)       47 2023-04-09 06:51:18.000000 flusso-0.1.0/flusso.egg-info/requires.txt
+-rw-r--r--   0 tomiwaadey   (501) staff       (20)       12 2023-04-09 06:51:18.000000 flusso-0.1.0/flusso.egg-info/top_level.txt
+-rw-r--r--   0 tomiwaadey   (501) staff       (20)       38 2023-04-09 06:51:18.291337 flusso-0.1.0/setup.cfg
+-rw-r--r--   0 tomiwaadey   (501) staff       (20)      949 2023-04-09 06:44:29.000000 flusso-0.1.0/setup.py
+drwxr-xr-x   0 tomiwaadey   (501) staff       (20)        0 2023-04-09 06:51:18.289807 flusso-0.1.0/test/
+-rw-r--r--   0 tomiwaadey   (501) staff       (20)        0 2023-03-29 21:20:14.000000 flusso-0.1.0/test/__init__.py
+-rw-r--r--   0 tomiwaadey   (501) staff       (20)     5095 2023-04-09 05:29:43.000000 flusso-0.1.0/test/test_async_result.py
+-rw-r--r--   0 tomiwaadey   (501) staff       (20)      794 2023-04-05 09:43:08.000000 flusso-0.1.0/test/test_functions.py
+-rw-r--r--   0 tomiwaadey   (501) staff       (20)     3303 2023-04-05 09:43:16.000000 flusso-0.1.0/test/test_option.py
+-rw-r--r--   0 tomiwaadey   (501) staff       (20)     4303 2023-04-05 09:43:28.000000 flusso-0.1.0/test/test_result.py
```

### Comparing `flusso-0.0.1/LICENSE` & `flusso-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flusso-0.0.1/PKG-INFO` & `flusso-0.1.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flusso
-Version: 0.0.1
+Version: 0.1.0
 Summary: Rust Inspired Type-Safe Errors and Missing Values for Python.
 Home-page: https://github.com/gum-tech/flusso
 Author: Tomiwa Adey
 Author-email: tomiwa@tomiwaadey.com
 License: MIT
 Keywords: python,monad,rust,functional-programming,option,result
 Classifier: Programming Language :: Python :: 3
@@ -74,14 +74,19 @@
     - [Option decorator](#option-decorator)
     - [Benefits](#benefits)
 - `Result<T,E>`
     - [Introduction](#introduction-1)
     - [Basic usage](#basic-usage-1)
     - [Result decorator](#result-decorator)
     - [Benefits](#benefits-1)
+- `AsyncResult<T,E>`
+    - [Introduction](#introduction-2)
+    - [Basic usage](#basic-usage-2)
+    - [AsyncResult decorator](#async_result-decorator)
+    - [Benefits](#benefits-2)
 - Utils
     - [Flatten](#flatten)
     - [Pattern matching](#pattern-matching)
     - [Do Notation](#do)
 
 
 ## `Option<T>`
@@ -151,28 +156,28 @@
   The code also uses None to define missing values. Even with a simple example like this, it’s not immediately clear where the None is coming from when we check if the username is None. In large codebases, this can be a nightmare to diagnose and fix.
 
   However, since this code style is more familiar and follows a more traditional control flow, it can be easier to understand for most programmers.
 
   Let's rewrite this with a declarative style using flusso
 
   ```python
-    from flusso import Option, Some, Nothing
+    from flusso.option import Option, Some, Nothing
 
     class User:
         def __init__(self, id: int, fullname: str, username: str):
             self.id = id
             self.fullname = fullname
             self.username = username
 
     users = [
         User(1, "Leonardo Da Vinci", "leo"),
         User(2, "Galileo Galilei", "gaga")
     ]
 
-    def get_user(id: int) -> 'Option[User]':
+    def get_user(id: int) -> Option[User]:
         user = next((user for user in users if user.id == id), Nothing)
         return Some(user)
 
     def get_username(id: int) -> Option[str]:
         return get_user(id).fmap(lambda user: user.username)
 
 
@@ -200,24 +205,24 @@
    **Example II**
 
   Let’s look at another example of using option to handle optional values.
 
   if the value of an object can be empty or optional like the `middle_name`of `User` in the following example, we can set its data type as an `Option`type.
 
   ```python
-   from flusso import Option, Some, Nothing
+   from flusso.option import Option, Some, Nothing
 
     def get_full_name(first_name: str, middle_name: Option[str], last_name: str) -> str:
-    match(middle_name):
-        case Some(mname):
-            print(f"{first_name} {mname} {last_name}")
-
-        # Matches `Nothing` instance
-        case Nothing:
-            print(f"{first_name} {last_name}")
+        match(middle_name):
+            case Some(mname):
+                print(f"{first_name} {mname} {last_name}")
+
+            # Matches `Nothing` instance
+            case Nothing:
+                print(f"{first_name} {last_name}")
 
     get_full_name("Galileo", None, "Galilei"); # Galileo Galilei
     get_full_name("Leonardo", Some("Da"), "Vinci"); # Leonardo Da Vinci
   ```
    Let’s look at another example by chaining calculations
 
   ```python
@@ -276,15 +281,15 @@
 
 ## Option decorator
 When working with functions that return Optional values, it's common to encounter numerous if x is not None: checks in your code. Flusso comes to the rescue with the @option decorator, which simplifies this process by converting functions that return Optional values to return Option instances instead.
 
 Here's how to use the @option decorator in Flusso:
   ```python
     from typing import Optional
-    from flusso import Option, Some, option
+    from flusso.option import Option, Some, option
 
     @option
     def find_even_number(numbers: list[int]) -> Optional[int]:
         for number in numbers:
             if number % 2 == 0:
                 return number
         return None
@@ -417,31 +422,167 @@
 1. Improved error handling: Result provides a structured way to handle errors and exceptions, allowing for more predictable and easy-to-reason-about code.
 2. Improved code readability: By using Result, it is clear to anyone reading the code that a computation may or may not be successful, and what to do in each case. This can make the code easier to understand and maintain.
 3. Improved code reliability: By using the Result, it is easier to ensure that errors and exceptions are properly handled and do not result in unexpected behavior or crashes.
 4. Improved code composability: Result allows for the chaining of operations. This can make it easier to build up complex computations from simpler ones.
 
 [⬆️  Back to top](#toc)
 
-## Utils
+## AsyncResult[T, E]
+
+### **Introduction**
+
+  `AsyncResult` is a utility class for working with asynchronous operations that may result in a success or an error. It is built on top of the Result class, which represents a synchronous operation's result. The AsyncResult class is useful for chaining, transforming, and handling results from asynchronous operations.
+
+  [⬆️  Back to top](#toc)
+
+### **Basic usage**
+
+  Let’s start with an example of how you might use exceptions in Python.
+
+  ```python
+    from flusso.async_result import async_result, Ok, Err
+
+    @async_result
+    async def async_fetch_data(url: str) -> Dict[str, Any]:
+        async with aiohttp.ClientSession() as session:
+            async with session.get(url) as response:
+                if response.status != 200:
+                    raise ValueError("Failed to fetch data")
+                return await response.json()
+
+    async def fetch():
+        url = "https://jsonplaceholder.typicode.com/todos/1"
+        async_result = await async_fetch_data(url)
+
+        match async_result._result:
+            case Ok(value):
+                print("Fetched data:", value)
+            case Err(error):
+                print("Error fetching data:", error)
+
+        # Alternatively
+        # if async_result.is_ok():
+        #     print("Fetched data:", await async_result.unwrap())
+        # else:
+        #     print("Error fetching data:", await async_result.unwrap_err())
+
+    asyncio.run(fetch())
+
+  ```
+AsyncResult provides several methods for working with and transforming the result:
+
+- fmap(fn): Transform the successful value using an asynchronous or synchronous function.
+- fmap_err(fn): Transform the error value using an asynchronous or synchronous function.
+- and_then(fn): Chain an asynchronous operation that returns a new AsyncResult if the current result is a success.
+- or_else(fn): Chain an asynchronous operation that returns a new AsyncResult if the current result is an error.
+
+#### fmap
+Transform the successful value using an asynchronous or synchronous function. If the AsyncResult is an error, the function won't be called, and the original error will be propagated.
+```python
+    async def async_multiply(value, factor):
+        return value * factor
+
+    async_result = AsyncResult(Ok(5))
+    mapped_result = await async_result.fmap(async_multiply, 2)  # Ok(10)
+```
+#### fmap_err
+Transform the error value using an asynchronous or synchronous function. If the AsyncResult is a success, the function won't be called, and the original success value will be propagated.
+```python
+    async def async_error_message(code):
+        return f"Error {code}"
+
+    async_result = AsyncResult(Err(404))
+    mapped_error_result = await async_result.fmap_err(async_error_message)  # Err("Error 404")
+```
+#### and_then
+Chain an asynchronous operation that returns a new AsyncResult if the current result is a success. If the AsyncResult is an error, the function won't be called, and the original error will be propagated.
+```python
+    async def async_double(value):
+        return AsyncResult(Ok(value * 2))
+
+    async_result = AsyncResult(Ok(5))
+    chained_result = await async_result.and_then(async_double)  # Ok(10)
+```
+
+#### or_else
+Chain an asynchronous operation that returns a new AsyncResult if the current result is an error. If the AsyncResult is a success, the function won't be called, and the original success value will be propagated.
+
+```python
+    async def async_handle_error(error):
+        return AsyncResult(Ok(f"Recovered from {error}"))
+
+    async_result = AsyncResult(Err("an error"))
+    handled_result = await async_result.or_else(async_handle_error)  # Ok("Recovered from an error")
+```
+
+[⬆️  Back to top](#toc)
+
+## AsyncResult decorator
+When working with asynchronous functions that might raise exceptions, it's common to see many try-except blocks combined with async-await syntax, which can complicate your code. Flusso comes to the rescue with the @async_result decorator, which simplifies this process by converting asynchronous functions that raise exceptions into functions that return AsyncResult instances instead.
+
+Here's how to use the @async_result_decorator in Flusso:
+  ```python
+    @async_result
+    # Apply the @async_result decorator to your asynchronous functions that might raise exceptions:
+    async def async_fetch_data(url: str) -> Result[str, Exception]:
+        async with aiohttp.ClientSession() as session:
+            async with session.get(url) as response:
+                if response.status != 200:
+                    raise ValueError("Failed to fetch data")
+                return await response.text()
+
+    # When calling the decorated function, it will return an AsyncResult object instead of raising an exception:
+    async def main():
+        url = "https://example.com/data"
+        async_result = await async_fetch_data(url)
+
+        if async_result.is_ok():
+            print("Fetched data:", await async_result.unwrap())
+        else:
+            print("Error fetching data:", await async_result.unwrap_err())
+  ```
+
+
+### **Benefits**
+
+There are several reasons why you might choose to use the flusso.async_result in your code:
+
+1. Cleaner code: By using AsyncResult, you can minimize the need for nested try-except blocks and async-await syntax, leading to more readable and maintainable code.
 
+2. Composable error handling: The AsyncResult class allows you to chain error handling and transformation functions, making it easy to compose complex error handling logic in a declarative manner.
+
+3. Separation of concerns: AsyncResult helps you separate the success and error cases, ensuring that your functions are focused on their primary responsibilities and not cluttered with error handling logic.
+
+4. Type safety: AsyncResult is a generic type that allows you to specify the success and error types, providing better type-checking and making it easier to catch potential issues during development.
+
+5. Flexible error transformation: The AsyncResult class provides methods like fmap, fmap_err, and_then, and or_else, which allow you to transform, chain, and handle errors in a flexible way.
+
+6. Easier testing: Since functions that return AsyncResult objects no longer raise exceptions directly, testing various scenarios and edge cases becomes simpler and more intuitive.
+
+7. Consistent error handling: By using AsyncResult throughout your code, you can establish a consistent approach to error handling, making your codebase more robust and easier to understand.
+
+8. Integration with Result: AsyncResult is designed to work seamlessly with Flusso's Result class, allowing you to handle both synchronous and asynchronous operations with a consistent API.
+
+
+## Utils
 
 ### Flatten
 To remove many levels of nesting:
 
 ```python
-import { Some, None, Ok, Err, flatten } from 'flow-ts'
-// with Option
-flatten(Some(Some(None))) // None
-flatten(Some('some1')) // Some('some1')
-flatten(None) // None
-// with Result
-flatten(Ok(Ok(Ok(Ok(Ok(Ok(Ok(10)))))))) // Ok(10)
-flatten(Ok(Ok(Err('error1')))) // Err('error2')
-flatten(Ok('ok1')) // Ok('ok1')
-flatten(Err('error1')) // Err('error1')
+# With Option
+print(flatten(Some(Some(Nothing))))  # Nothing
+print(flatten(Some("some1")))        # Some("some1")
+print(flatten(Nothing))              # Nothing
+
+# With Result
+print(flatten(Ok(Ok(Ok(Ok(Ok(Ok(Ok(10)))))))) # Ok(10)
+print(flatten(Ok(Ok(Err("error1")))))         # Err("error1")
+print(flatten(Ok("ok1")))                     # Ok("ok1")
+print(flatten(Err("error1")))                 # Err("error1")
 ```
 
 ### Pattern matching
 When using pattern matching with Flusso, you can match on Some, Nothing, Ok, and Err cases and extract the inner values accordingly. This approach allows you to focus on the logic of your application, making your code more maintainable and easier to understand.
 
   ```python
 
@@ -468,16 +609,18 @@
                     print(f"Error: {err_msg}")
         case Nothing:
             print("Value not found in the data")
 
   ```
 
 ### Do Notation
-Flusso provides a simple way to handle chained computations using the Do notation. The Do notation is a feature that simplifies complex operations with Option and Result instances. With Flusso's implementation of Do notation, you can easily manage multiple steps in a computation while maintaining clean, readable code.
-Here's how to use the Do notation for both Option and Result types in Flusso.
+Flusso provides a simple way to handle chained computations using the Do notation.
+The do notation offers a more intuitive and readable Imperative-style syntax for working with monadic types like Result, Option, and AsyncResult, allowing you to write sequential-like code while retaining the powerful error handling and encapsulation features of monads.
+With Flusso's implementation of Do notation, you can easily manage multiple steps in a computation while maintaining clean, readable code.
+Here's how to use the Do notation for Option, Result, and AsyncResult types in Flusso.
 
 Option example:
 ```python
     def add_numbers(a: int, b: int) -> Option[int]:
         return Some(a + b)
 
     def multiply_numbers(a: int, b: int) -> Option[int]:
@@ -513,18 +656,45 @@
     ):
         result = Ok(c)
 
     assert result == Ok(((x + y) * x) + y)
 ```
 Similarly, the Do notation can also be used with Result instances. It provides a clean, functional way to handle chained computations and potential errors.
 
-By using the Do notation in Flusso, you can write more expressive and maintainable code when working with Option and Result instances.
+AsyncResult example:
+```python
+    @async_result
+    async def async_fetch_data(url: str) -> Dict[str, Any]:
+        async with aiohttp.ClientSession() as session:
+            async with session.get(url) as response:
+                if response.status != 200:
+                    raise ValueError("Failed to fetch data")
+                return await response.json()
+
+    async def fetch_do():
+        url = "https://jsonplaceholder.typicode.com/todos/1"
+
+        async with (
+            AsyncResult.do(fetch_data=async_fetch_data(url)) as fetch_result
+        ):
+
+            match fetch_result._result:
+                case Ok(data):
+                    print("Fetched data:", data)
+                case Err(error):
+                    print("Error fetching data:", error)
+
+    asyncio.run(fetch_do())
+```
+
+By using the Do notation in Flusso, you can write more expressive and maintainable code when working with Option, Result, and AsyncResult instances.
 
 ### Coming soon
-- Asynchronous support: Integrate seamless handling of asynchronous operations with Option and Result instances, making it even more convenient to work with coroutines.
-- Comprehensive documentation and examples: Expand the library's documentation and provide more practical examples to help users get the most out of Flusso.
-- Enhancing the Do notation to allow more fine-grained error handling or recovery, such as customizing the behavior for specific error cases or providing default values when certain errors occur.
-- Improving the error messages produced by the Do notation to provide more context and clarity when something goes wrong.
-- Custom data types: Provide an easy-to-use interface for creating custom data types that adhere to Flusso's functional programming principles and type safety requirements.
+- [x] Asynchronous support: Integrate seamless handling of asynchronous operations with Result instances, making it even more convenient to work with coroutines.
+- [ ] Comprehensive documentation and examples: Expand the library's documentation and provide more practical examples to help users get the most out of Flusso.
+- [ ] Enhancing the Do notation to allow more fine-grained error handling or recovery, such as customizing the behavior for specific error cases or providing default values when certain errors occur.
+- [ ] Improving the error messages produced by the Do notation to provide more context and clarity when something goes wrong.
+- [ ] Custom data types: Provide an easy-to-use interface for creating custom data types that adhere to Flusso's functional programming principles and type safety requirements.
+
 [⬆️  Back to top](#toc)
 
 If you find this package useful, please click the star button ✨!
```

### Comparing `flusso-0.0.1/README.md` & `flusso-0.1.0/flusso.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: flusso
+Version: 0.1.0
+Summary: Rust Inspired Type-Safe Errors and Missing Values for Python.
+Home-page: https://github.com/gum-tech/flusso
+Author: Tomiwa Adey
+Author-email: tomiwa@tomiwaadey.com
+License: MIT
+Keywords: python,monad,rust,functional-programming,option,result
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
 ## What is flusso?
 
 `flusso` is a library for Python that aims to safely handle exceptions and missing values, similar to how Rust handles them with its `Option` and `Result` types.
 
 In short, Flusso empowers you to craft Python code that is:
 - Free from None values
 - Devoid of exceptions
@@ -57,14 +74,19 @@
     - [Option decorator](#option-decorator)
     - [Benefits](#benefits)
 - `Result<T,E>`
     - [Introduction](#introduction-1)
     - [Basic usage](#basic-usage-1)
     - [Result decorator](#result-decorator)
     - [Benefits](#benefits-1)
+- `AsyncResult<T,E>`
+    - [Introduction](#introduction-2)
+    - [Basic usage](#basic-usage-2)
+    - [AsyncResult decorator](#async_result-decorator)
+    - [Benefits](#benefits-2)
 - Utils
     - [Flatten](#flatten)
     - [Pattern matching](#pattern-matching)
     - [Do Notation](#do)
 
 
 ## `Option<T>`
@@ -134,28 +156,28 @@
   The code also uses None to define missing values. Even with a simple example like this, it’s not immediately clear where the None is coming from when we check if the username is None. In large codebases, this can be a nightmare to diagnose and fix.
 
   However, since this code style is more familiar and follows a more traditional control flow, it can be easier to understand for most programmers.
 
   Let's rewrite this with a declarative style using flusso
 
   ```python
-    from flusso import Option, Some, Nothing
+    from flusso.option import Option, Some, Nothing
 
     class User:
         def __init__(self, id: int, fullname: str, username: str):
             self.id = id
             self.fullname = fullname
             self.username = username
 
     users = [
         User(1, "Leonardo Da Vinci", "leo"),
         User(2, "Galileo Galilei", "gaga")
     ]
 
-    def get_user(id: int) -> 'Option[User]':
+    def get_user(id: int) -> Option[User]:
         user = next((user for user in users if user.id == id), Nothing)
         return Some(user)
 
     def get_username(id: int) -> Option[str]:
         return get_user(id).fmap(lambda user: user.username)
 
 
@@ -183,24 +205,24 @@
    **Example II**
 
   Let’s look at another example of using option to handle optional values.
 
   if the value of an object can be empty or optional like the `middle_name`of `User` in the following example, we can set its data type as an `Option`type.
 
   ```python
-   from flusso import Option, Some, Nothing
+   from flusso.option import Option, Some, Nothing
 
     def get_full_name(first_name: str, middle_name: Option[str], last_name: str) -> str:
-    match(middle_name):
-        case Some(mname):
-            print(f"{first_name} {mname} {last_name}")
-
-        # Matches `Nothing` instance
-        case Nothing:
-            print(f"{first_name} {last_name}")
+        match(middle_name):
+            case Some(mname):
+                print(f"{first_name} {mname} {last_name}")
+
+            # Matches `Nothing` instance
+            case Nothing:
+                print(f"{first_name} {last_name}")
 
     get_full_name("Galileo", None, "Galilei"); # Galileo Galilei
     get_full_name("Leonardo", Some("Da"), "Vinci"); # Leonardo Da Vinci
   ```
    Let’s look at another example by chaining calculations
 
   ```python
@@ -259,15 +281,15 @@
 
 ## Option decorator
 When working with functions that return Optional values, it's common to encounter numerous if x is not None: checks in your code. Flusso comes to the rescue with the @option decorator, which simplifies this process by converting functions that return Optional values to return Option instances instead.
 
 Here's how to use the @option decorator in Flusso:
   ```python
     from typing import Optional
-    from flusso import Option, Some, option
+    from flusso.option import Option, Some, option
 
     @option
     def find_even_number(numbers: list[int]) -> Optional[int]:
         for number in numbers:
             if number % 2 == 0:
                 return number
         return None
@@ -400,31 +422,167 @@
 1. Improved error handling: Result provides a structured way to handle errors and exceptions, allowing for more predictable and easy-to-reason-about code.
 2. Improved code readability: By using Result, it is clear to anyone reading the code that a computation may or may not be successful, and what to do in each case. This can make the code easier to understand and maintain.
 3. Improved code reliability: By using the Result, it is easier to ensure that errors and exceptions are properly handled and do not result in unexpected behavior or crashes.
 4. Improved code composability: Result allows for the chaining of operations. This can make it easier to build up complex computations from simpler ones.
 
 [⬆️  Back to top](#toc)
 
-## Utils
+## AsyncResult[T, E]
+
+### **Introduction**
+
+  `AsyncResult` is a utility class for working with asynchronous operations that may result in a success or an error. It is built on top of the Result class, which represents a synchronous operation's result. The AsyncResult class is useful for chaining, transforming, and handling results from asynchronous operations.
 
+  [⬆️  Back to top](#toc)
+
+### **Basic usage**
+
+  Let’s start with an example of how you might use exceptions in Python.
+
+  ```python
+    from flusso.async_result import async_result, Ok, Err
+
+    @async_result
+    async def async_fetch_data(url: str) -> Dict[str, Any]:
+        async with aiohttp.ClientSession() as session:
+            async with session.get(url) as response:
+                if response.status != 200:
+                    raise ValueError("Failed to fetch data")
+                return await response.json()
+
+    async def fetch():
+        url = "https://jsonplaceholder.typicode.com/todos/1"
+        async_result = await async_fetch_data(url)
+
+        match async_result._result:
+            case Ok(value):
+                print("Fetched data:", value)
+            case Err(error):
+                print("Error fetching data:", error)
+
+        # Alternatively
+        # if async_result.is_ok():
+        #     print("Fetched data:", await async_result.unwrap())
+        # else:
+        #     print("Error fetching data:", await async_result.unwrap_err())
+
+    asyncio.run(fetch())
+
+  ```
+AsyncResult provides several methods for working with and transforming the result:
+
+- fmap(fn): Transform the successful value using an asynchronous or synchronous function.
+- fmap_err(fn): Transform the error value using an asynchronous or synchronous function.
+- and_then(fn): Chain an asynchronous operation that returns a new AsyncResult if the current result is a success.
+- or_else(fn): Chain an asynchronous operation that returns a new AsyncResult if the current result is an error.
+
+#### fmap
+Transform the successful value using an asynchronous or synchronous function. If the AsyncResult is an error, the function won't be called, and the original error will be propagated.
+```python
+    async def async_multiply(value, factor):
+        return value * factor
+
+    async_result = AsyncResult(Ok(5))
+    mapped_result = await async_result.fmap(async_multiply, 2)  # Ok(10)
+```
+#### fmap_err
+Transform the error value using an asynchronous or synchronous function. If the AsyncResult is a success, the function won't be called, and the original success value will be propagated.
+```python
+    async def async_error_message(code):
+        return f"Error {code}"
+
+    async_result = AsyncResult(Err(404))
+    mapped_error_result = await async_result.fmap_err(async_error_message)  # Err("Error 404")
+```
+#### and_then
+Chain an asynchronous operation that returns a new AsyncResult if the current result is a success. If the AsyncResult is an error, the function won't be called, and the original error will be propagated.
+```python
+    async def async_double(value):
+        return AsyncResult(Ok(value * 2))
+
+    async_result = AsyncResult(Ok(5))
+    chained_result = await async_result.and_then(async_double)  # Ok(10)
+```
+
+#### or_else
+Chain an asynchronous operation that returns a new AsyncResult if the current result is an error. If the AsyncResult is a success, the function won't be called, and the original success value will be propagated.
+
+```python
+    async def async_handle_error(error):
+        return AsyncResult(Ok(f"Recovered from {error}"))
+
+    async_result = AsyncResult(Err("an error"))
+    handled_result = await async_result.or_else(async_handle_error)  # Ok("Recovered from an error")
+```
+
+[⬆️  Back to top](#toc)
+
+## AsyncResult decorator
+When working with asynchronous functions that might raise exceptions, it's common to see many try-except blocks combined with async-await syntax, which can complicate your code. Flusso comes to the rescue with the @async_result decorator, which simplifies this process by converting asynchronous functions that raise exceptions into functions that return AsyncResult instances instead.
+
+Here's how to use the @async_result_decorator in Flusso:
+  ```python
+    @async_result
+    # Apply the @async_result decorator to your asynchronous functions that might raise exceptions:
+    async def async_fetch_data(url: str) -> Result[str, Exception]:
+        async with aiohttp.ClientSession() as session:
+            async with session.get(url) as response:
+                if response.status != 200:
+                    raise ValueError("Failed to fetch data")
+                return await response.text()
+
+    # When calling the decorated function, it will return an AsyncResult object instead of raising an exception:
+    async def main():
+        url = "https://example.com/data"
+        async_result = await async_fetch_data(url)
+
+        if async_result.is_ok():
+            print("Fetched data:", await async_result.unwrap())
+        else:
+            print("Error fetching data:", await async_result.unwrap_err())
+  ```
+
+
+### **Benefits**
+
+There are several reasons why you might choose to use the flusso.async_result in your code:
+
+1. Cleaner code: By using AsyncResult, you can minimize the need for nested try-except blocks and async-await syntax, leading to more readable and maintainable code.
+
+2. Composable error handling: The AsyncResult class allows you to chain error handling and transformation functions, making it easy to compose complex error handling logic in a declarative manner.
+
+3. Separation of concerns: AsyncResult helps you separate the success and error cases, ensuring that your functions are focused on their primary responsibilities and not cluttered with error handling logic.
+
+4. Type safety: AsyncResult is a generic type that allows you to specify the success and error types, providing better type-checking and making it easier to catch potential issues during development.
+
+5. Flexible error transformation: The AsyncResult class provides methods like fmap, fmap_err, and_then, and or_else, which allow you to transform, chain, and handle errors in a flexible way.
+
+6. Easier testing: Since functions that return AsyncResult objects no longer raise exceptions directly, testing various scenarios and edge cases becomes simpler and more intuitive.
+
+7. Consistent error handling: By using AsyncResult throughout your code, you can establish a consistent approach to error handling, making your codebase more robust and easier to understand.
+
+8. Integration with Result: AsyncResult is designed to work seamlessly with Flusso's Result class, allowing you to handle both synchronous and asynchronous operations with a consistent API.
+
+
+## Utils
 
 ### Flatten
 To remove many levels of nesting:
 
 ```python
-import { Some, None, Ok, Err, flatten } from 'flow-ts'
-// with Option
-flatten(Some(Some(None))) // None
-flatten(Some('some1')) // Some('some1')
-flatten(None) // None
-// with Result
-flatten(Ok(Ok(Ok(Ok(Ok(Ok(Ok(10)))))))) // Ok(10)
-flatten(Ok(Ok(Err('error1')))) // Err('error2')
-flatten(Ok('ok1')) // Ok('ok1')
-flatten(Err('error1')) // Err('error1')
+# With Option
+print(flatten(Some(Some(Nothing))))  # Nothing
+print(flatten(Some("some1")))        # Some("some1")
+print(flatten(Nothing))              # Nothing
+
+# With Result
+print(flatten(Ok(Ok(Ok(Ok(Ok(Ok(Ok(10)))))))) # Ok(10)
+print(flatten(Ok(Ok(Err("error1")))))         # Err("error1")
+print(flatten(Ok("ok1")))                     # Ok("ok1")
+print(flatten(Err("error1")))                 # Err("error1")
 ```
 
 ### Pattern matching
 When using pattern matching with Flusso, you can match on Some, Nothing, Ok, and Err cases and extract the inner values accordingly. This approach allows you to focus on the logic of your application, making your code more maintainable and easier to understand.
 
   ```python
 
@@ -451,16 +609,18 @@
                     print(f"Error: {err_msg}")
         case Nothing:
             print("Value not found in the data")
 
   ```
 
 ### Do Notation
-Flusso provides a simple way to handle chained computations using the Do notation. The Do notation is a feature that simplifies complex operations with Option and Result instances. With Flusso's implementation of Do notation, you can easily manage multiple steps in a computation while maintaining clean, readable code.
-Here's how to use the Do notation for both Option and Result types in Flusso.
+Flusso provides a simple way to handle chained computations using the Do notation.
+The do notation offers a more intuitive and readable Imperative-style syntax for working with monadic types like Result, Option, and AsyncResult, allowing you to write sequential-like code while retaining the powerful error handling and encapsulation features of monads.
+With Flusso's implementation of Do notation, you can easily manage multiple steps in a computation while maintaining clean, readable code.
+Here's how to use the Do notation for Option, Result, and AsyncResult types in Flusso.
 
 Option example:
 ```python
     def add_numbers(a: int, b: int) -> Option[int]:
         return Some(a + b)
 
     def multiply_numbers(a: int, b: int) -> Option[int]:
@@ -496,18 +656,45 @@
     ):
         result = Ok(c)
 
     assert result == Ok(((x + y) * x) + y)
 ```
 Similarly, the Do notation can also be used with Result instances. It provides a clean, functional way to handle chained computations and potential errors.
 
-By using the Do notation in Flusso, you can write more expressive and maintainable code when working with Option and Result instances.
+AsyncResult example:
+```python
+    @async_result
+    async def async_fetch_data(url: str) -> Dict[str, Any]:
+        async with aiohttp.ClientSession() as session:
+            async with session.get(url) as response:
+                if response.status != 200:
+                    raise ValueError("Failed to fetch data")
+                return await response.json()
+
+    async def fetch_do():
+        url = "https://jsonplaceholder.typicode.com/todos/1"
+
+        async with (
+            AsyncResult.do(fetch_data=async_fetch_data(url)) as fetch_result
+        ):
+
+            match fetch_result._result:
+                case Ok(data):
+                    print("Fetched data:", data)
+                case Err(error):
+                    print("Error fetching data:", error)
+
+    asyncio.run(fetch_do())
+```
+
+By using the Do notation in Flusso, you can write more expressive and maintainable code when working with Option, Result, and AsyncResult instances.
 
 ### Coming soon
-- Asynchronous support: Integrate seamless handling of asynchronous operations with Option and Result instances, making it even more convenient to work with coroutines.
-- Comprehensive documentation and examples: Expand the library's documentation and provide more practical examples to help users get the most out of Flusso.
-- Enhancing the Do notation to allow more fine-grained error handling or recovery, such as customizing the behavior for specific error cases or providing default values when certain errors occur.
-- Improving the error messages produced by the Do notation to provide more context and clarity when something goes wrong.
-- Custom data types: Provide an easy-to-use interface for creating custom data types that adhere to Flusso's functional programming principles and type safety requirements.
+- [x] Asynchronous support: Integrate seamless handling of asynchronous operations with Result instances, making it even more convenient to work with coroutines.
+- [ ] Comprehensive documentation and examples: Expand the library's documentation and provide more practical examples to help users get the most out of Flusso.
+- [ ] Enhancing the Do notation to allow more fine-grained error handling or recovery, such as customizing the behavior for specific error cases or providing default values when certain errors occur.
+- [ ] Improving the error messages produced by the Do notation to provide more context and clarity when something goes wrong.
+- [ ] Custom data types: Provide an easy-to-use interface for creating custom data types that adhere to Flusso's functional programming principles and type safety requirements.
+
 [⬆️  Back to top](#toc)
 
 If you find this package useful, please click the star button ✨!
```

### Comparing `flusso-0.0.1/flusso/functions.py` & `flusso-0.1.0/flusso/functions.py`

 * *Files identical despite different names*

### Comparing `flusso-0.0.1/flusso/option.py` & `flusso-0.1.0/flusso/option.py`

 * *Files identical despite different names*

### Comparing `flusso-0.0.1/flusso/primitives/base.py` & `flusso-0.1.0/flusso/primitives/base.py`

 * *Files identical despite different names*

### Comparing `flusso-0.0.1/flusso/primitives/exceptions.py` & `flusso-0.1.0/flusso/primitives/exceptions.py`

 * *Files identical despite different names*

### Comparing `flusso-0.0.1/flusso/result.py` & `flusso-0.1.0/flusso/result.py`

 * *Files identical despite different names*

### Comparing `flusso-0.0.1/flusso.egg-info/PKG-INFO` & `flusso-0.1.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: flusso
-Version: 0.0.1
-Summary: Rust Inspired Type-Safe Errors and Missing Values for Python.
-Home-page: https://github.com/gum-tech/flusso
-Author: Tomiwa Adey
-Author-email: tomiwa@tomiwaadey.com
-License: MIT
-Keywords: python,monad,rust,functional-programming,option,result
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 ## What is flusso?
 
 `flusso` is a library for Python that aims to safely handle exceptions and missing values, similar to how Rust handles them with its `Option` and `Result` types.
 
 In short, Flusso empowers you to craft Python code that is:
 - Free from None values
 - Devoid of exceptions
@@ -74,14 +57,19 @@
     - [Option decorator](#option-decorator)
     - [Benefits](#benefits)
 - `Result<T,E>`
     - [Introduction](#introduction-1)
     - [Basic usage](#basic-usage-1)
     - [Result decorator](#result-decorator)
     - [Benefits](#benefits-1)
+- `AsyncResult<T,E>`
+    - [Introduction](#introduction-2)
+    - [Basic usage](#basic-usage-2)
+    - [AsyncResult decorator](#async_result-decorator)
+    - [Benefits](#benefits-2)
 - Utils
     - [Flatten](#flatten)
     - [Pattern matching](#pattern-matching)
     - [Do Notation](#do)
 
 
 ## `Option<T>`
@@ -151,28 +139,28 @@
   The code also uses None to define missing values. Even with a simple example like this, it’s not immediately clear where the None is coming from when we check if the username is None. In large codebases, this can be a nightmare to diagnose and fix.
 
   However, since this code style is more familiar and follows a more traditional control flow, it can be easier to understand for most programmers.
 
   Let's rewrite this with a declarative style using flusso
 
   ```python
-    from flusso import Option, Some, Nothing
+    from flusso.option import Option, Some, Nothing
 
     class User:
         def __init__(self, id: int, fullname: str, username: str):
             self.id = id
             self.fullname = fullname
             self.username = username
 
     users = [
         User(1, "Leonardo Da Vinci", "leo"),
         User(2, "Galileo Galilei", "gaga")
     ]
 
-    def get_user(id: int) -> 'Option[User]':
+    def get_user(id: int) -> Option[User]:
         user = next((user for user in users if user.id == id), Nothing)
         return Some(user)
 
     def get_username(id: int) -> Option[str]:
         return get_user(id).fmap(lambda user: user.username)
 
 
@@ -200,24 +188,24 @@
    **Example II**
 
   Let’s look at another example of using option to handle optional values.
 
   if the value of an object can be empty or optional like the `middle_name`of `User` in the following example, we can set its data type as an `Option`type.
 
   ```python
-   from flusso import Option, Some, Nothing
+   from flusso.option import Option, Some, Nothing
 
     def get_full_name(first_name: str, middle_name: Option[str], last_name: str) -> str:
-    match(middle_name):
-        case Some(mname):
-            print(f"{first_name} {mname} {last_name}")
-
-        # Matches `Nothing` instance
-        case Nothing:
-            print(f"{first_name} {last_name}")
+        match(middle_name):
+            case Some(mname):
+                print(f"{first_name} {mname} {last_name}")
+
+            # Matches `Nothing` instance
+            case Nothing:
+                print(f"{first_name} {last_name}")
 
     get_full_name("Galileo", None, "Galilei"); # Galileo Galilei
     get_full_name("Leonardo", Some("Da"), "Vinci"); # Leonardo Da Vinci
   ```
    Let’s look at another example by chaining calculations
 
   ```python
@@ -276,15 +264,15 @@
 
 ## Option decorator
 When working with functions that return Optional values, it's common to encounter numerous if x is not None: checks in your code. Flusso comes to the rescue with the @option decorator, which simplifies this process by converting functions that return Optional values to return Option instances instead.
 
 Here's how to use the @option decorator in Flusso:
   ```python
     from typing import Optional
-    from flusso import Option, Some, option
+    from flusso.option import Option, Some, option
 
     @option
     def find_even_number(numbers: list[int]) -> Optional[int]:
         for number in numbers:
             if number % 2 == 0:
                 return number
         return None
@@ -417,31 +405,167 @@
 1. Improved error handling: Result provides a structured way to handle errors and exceptions, allowing for more predictable and easy-to-reason-about code.
 2. Improved code readability: By using Result, it is clear to anyone reading the code that a computation may or may not be successful, and what to do in each case. This can make the code easier to understand and maintain.
 3. Improved code reliability: By using the Result, it is easier to ensure that errors and exceptions are properly handled and do not result in unexpected behavior or crashes.
 4. Improved code composability: Result allows for the chaining of operations. This can make it easier to build up complex computations from simpler ones.
 
 [⬆️  Back to top](#toc)
 
-## Utils
+## AsyncResult[T, E]
+
+### **Introduction**
+
+  `AsyncResult` is a utility class for working with asynchronous operations that may result in a success or an error. It is built on top of the Result class, which represents a synchronous operation's result. The AsyncResult class is useful for chaining, transforming, and handling results from asynchronous operations.
 
+  [⬆️  Back to top](#toc)
+
+### **Basic usage**
+
+  Let’s start with an example of how you might use exceptions in Python.
+
+  ```python
+    from flusso.async_result import async_result, Ok, Err
+
+    @async_result
+    async def async_fetch_data(url: str) -> Dict[str, Any]:
+        async with aiohttp.ClientSession() as session:
+            async with session.get(url) as response:
+                if response.status != 200:
+                    raise ValueError("Failed to fetch data")
+                return await response.json()
+
+    async def fetch():
+        url = "https://jsonplaceholder.typicode.com/todos/1"
+        async_result = await async_fetch_data(url)
+
+        match async_result._result:
+            case Ok(value):
+                print("Fetched data:", value)
+            case Err(error):
+                print("Error fetching data:", error)
+
+        # Alternatively
+        # if async_result.is_ok():
+        #     print("Fetched data:", await async_result.unwrap())
+        # else:
+        #     print("Error fetching data:", await async_result.unwrap_err())
+
+    asyncio.run(fetch())
+
+  ```
+AsyncResult provides several methods for working with and transforming the result:
+
+- fmap(fn): Transform the successful value using an asynchronous or synchronous function.
+- fmap_err(fn): Transform the error value using an asynchronous or synchronous function.
+- and_then(fn): Chain an asynchronous operation that returns a new AsyncResult if the current result is a success.
+- or_else(fn): Chain an asynchronous operation that returns a new AsyncResult if the current result is an error.
+
+#### fmap
+Transform the successful value using an asynchronous or synchronous function. If the AsyncResult is an error, the function won't be called, and the original error will be propagated.
+```python
+    async def async_multiply(value, factor):
+        return value * factor
+
+    async_result = AsyncResult(Ok(5))
+    mapped_result = await async_result.fmap(async_multiply, 2)  # Ok(10)
+```
+#### fmap_err
+Transform the error value using an asynchronous or synchronous function. If the AsyncResult is a success, the function won't be called, and the original success value will be propagated.
+```python
+    async def async_error_message(code):
+        return f"Error {code}"
+
+    async_result = AsyncResult(Err(404))
+    mapped_error_result = await async_result.fmap_err(async_error_message)  # Err("Error 404")
+```
+#### and_then
+Chain an asynchronous operation that returns a new AsyncResult if the current result is a success. If the AsyncResult is an error, the function won't be called, and the original error will be propagated.
+```python
+    async def async_double(value):
+        return AsyncResult(Ok(value * 2))
+
+    async_result = AsyncResult(Ok(5))
+    chained_result = await async_result.and_then(async_double)  # Ok(10)
+```
+
+#### or_else
+Chain an asynchronous operation that returns a new AsyncResult if the current result is an error. If the AsyncResult is a success, the function won't be called, and the original success value will be propagated.
+
+```python
+    async def async_handle_error(error):
+        return AsyncResult(Ok(f"Recovered from {error}"))
+
+    async_result = AsyncResult(Err("an error"))
+    handled_result = await async_result.or_else(async_handle_error)  # Ok("Recovered from an error")
+```
+
+[⬆️  Back to top](#toc)
+
+## AsyncResult decorator
+When working with asynchronous functions that might raise exceptions, it's common to see many try-except blocks combined with async-await syntax, which can complicate your code. Flusso comes to the rescue with the @async_result decorator, which simplifies this process by converting asynchronous functions that raise exceptions into functions that return AsyncResult instances instead.
+
+Here's how to use the @async_result_decorator in Flusso:
+  ```python
+    @async_result
+    # Apply the @async_result decorator to your asynchronous functions that might raise exceptions:
+    async def async_fetch_data(url: str) -> Result[str, Exception]:
+        async with aiohttp.ClientSession() as session:
+            async with session.get(url) as response:
+                if response.status != 200:
+                    raise ValueError("Failed to fetch data")
+                return await response.text()
+
+    # When calling the decorated function, it will return an AsyncResult object instead of raising an exception:
+    async def main():
+        url = "https://example.com/data"
+        async_result = await async_fetch_data(url)
+
+        if async_result.is_ok():
+            print("Fetched data:", await async_result.unwrap())
+        else:
+            print("Error fetching data:", await async_result.unwrap_err())
+  ```
+
+
+### **Benefits**
+
+There are several reasons why you might choose to use the flusso.async_result in your code:
+
+1. Cleaner code: By using AsyncResult, you can minimize the need for nested try-except blocks and async-await syntax, leading to more readable and maintainable code.
+
+2. Composable error handling: The AsyncResult class allows you to chain error handling and transformation functions, making it easy to compose complex error handling logic in a declarative manner.
+
+3. Separation of concerns: AsyncResult helps you separate the success and error cases, ensuring that your functions are focused on their primary responsibilities and not cluttered with error handling logic.
+
+4. Type safety: AsyncResult is a generic type that allows you to specify the success and error types, providing better type-checking and making it easier to catch potential issues during development.
+
+5. Flexible error transformation: The AsyncResult class provides methods like fmap, fmap_err, and_then, and or_else, which allow you to transform, chain, and handle errors in a flexible way.
+
+6. Easier testing: Since functions that return AsyncResult objects no longer raise exceptions directly, testing various scenarios and edge cases becomes simpler and more intuitive.
+
+7. Consistent error handling: By using AsyncResult throughout your code, you can establish a consistent approach to error handling, making your codebase more robust and easier to understand.
+
+8. Integration with Result: AsyncResult is designed to work seamlessly with Flusso's Result class, allowing you to handle both synchronous and asynchronous operations with a consistent API.
+
+
+## Utils
 
 ### Flatten
 To remove many levels of nesting:
 
 ```python
-import { Some, None, Ok, Err, flatten } from 'flow-ts'
-// with Option
-flatten(Some(Some(None))) // None
-flatten(Some('some1')) // Some('some1')
-flatten(None) // None
-// with Result
-flatten(Ok(Ok(Ok(Ok(Ok(Ok(Ok(10)))))))) // Ok(10)
-flatten(Ok(Ok(Err('error1')))) // Err('error2')
-flatten(Ok('ok1')) // Ok('ok1')
-flatten(Err('error1')) // Err('error1')
+# With Option
+print(flatten(Some(Some(Nothing))))  # Nothing
+print(flatten(Some("some1")))        # Some("some1")
+print(flatten(Nothing))              # Nothing
+
+# With Result
+print(flatten(Ok(Ok(Ok(Ok(Ok(Ok(Ok(10)))))))) # Ok(10)
+print(flatten(Ok(Ok(Err("error1")))))         # Err("error1")
+print(flatten(Ok("ok1")))                     # Ok("ok1")
+print(flatten(Err("error1")))                 # Err("error1")
 ```
 
 ### Pattern matching
 When using pattern matching with Flusso, you can match on Some, Nothing, Ok, and Err cases and extract the inner values accordingly. This approach allows you to focus on the logic of your application, making your code more maintainable and easier to understand.
 
   ```python
 
@@ -468,16 +592,18 @@
                     print(f"Error: {err_msg}")
         case Nothing:
             print("Value not found in the data")
 
   ```
 
 ### Do Notation
-Flusso provides a simple way to handle chained computations using the Do notation. The Do notation is a feature that simplifies complex operations with Option and Result instances. With Flusso's implementation of Do notation, you can easily manage multiple steps in a computation while maintaining clean, readable code.
-Here's how to use the Do notation for both Option and Result types in Flusso.
+Flusso provides a simple way to handle chained computations using the Do notation.
+The do notation offers a more intuitive and readable Imperative-style syntax for working with monadic types like Result, Option, and AsyncResult, allowing you to write sequential-like code while retaining the powerful error handling and encapsulation features of monads.
+With Flusso's implementation of Do notation, you can easily manage multiple steps in a computation while maintaining clean, readable code.
+Here's how to use the Do notation for Option, Result, and AsyncResult types in Flusso.
 
 Option example:
 ```python
     def add_numbers(a: int, b: int) -> Option[int]:
         return Some(a + b)
 
     def multiply_numbers(a: int, b: int) -> Option[int]:
@@ -513,18 +639,45 @@
     ):
         result = Ok(c)
 
     assert result == Ok(((x + y) * x) + y)
 ```
 Similarly, the Do notation can also be used with Result instances. It provides a clean, functional way to handle chained computations and potential errors.
 
-By using the Do notation in Flusso, you can write more expressive and maintainable code when working with Option and Result instances.
+AsyncResult example:
+```python
+    @async_result
+    async def async_fetch_data(url: str) -> Dict[str, Any]:
+        async with aiohttp.ClientSession() as session:
+            async with session.get(url) as response:
+                if response.status != 200:
+                    raise ValueError("Failed to fetch data")
+                return await response.json()
+
+    async def fetch_do():
+        url = "https://jsonplaceholder.typicode.com/todos/1"
+
+        async with (
+            AsyncResult.do(fetch_data=async_fetch_data(url)) as fetch_result
+        ):
+
+            match fetch_result._result:
+                case Ok(data):
+                    print("Fetched data:", data)
+                case Err(error):
+                    print("Error fetching data:", error)
+
+    asyncio.run(fetch_do())
+```
+
+By using the Do notation in Flusso, you can write more expressive and maintainable code when working with Option, Result, and AsyncResult instances.
 
 ### Coming soon
-- Asynchronous support: Integrate seamless handling of asynchronous operations with Option and Result instances, making it even more convenient to work with coroutines.
-- Comprehensive documentation and examples: Expand the library's documentation and provide more practical examples to help users get the most out of Flusso.
-- Enhancing the Do notation to allow more fine-grained error handling or recovery, such as customizing the behavior for specific error cases or providing default values when certain errors occur.
-- Improving the error messages produced by the Do notation to provide more context and clarity when something goes wrong.
-- Custom data types: Provide an easy-to-use interface for creating custom data types that adhere to Flusso's functional programming principles and type safety requirements.
+- [x] Asynchronous support: Integrate seamless handling of asynchronous operations with Result instances, making it even more convenient to work with coroutines.
+- [ ] Comprehensive documentation and examples: Expand the library's documentation and provide more practical examples to help users get the most out of Flusso.
+- [ ] Enhancing the Do notation to allow more fine-grained error handling or recovery, such as customizing the behavior for specific error cases or providing default values when certain errors occur.
+- [ ] Improving the error messages produced by the Do notation to provide more context and clarity when something goes wrong.
+- [ ] Custom data types: Provide an easy-to-use interface for creating custom data types that adhere to Flusso's functional programming principles and type safety requirements.
+
 [⬆️  Back to top](#toc)
 
 If you find this package useful, please click the star button ✨!
```

### Comparing `flusso-0.0.1/setup.py` & `flusso-0.1.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="flusso",
-    version="0.0.1",
+    version="0.1.0",
     author="Tomiwa Adey",
     author_email="tomiwa@tomiwaadey.com",
     description="Rust Inspired Type-Safe Errors and Missing Values for Python.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/gum-tech/flusso",
     packages= find_packages(),
     license="MIT",
     keywords=['python', 'monad', 'rust', 'functional-programming', 'option', 'result'],
     extras_require={
-        "dev": ["pytest>=7.0", "twine>=4.0.2"],
+        "dev": ["pytest>=7.0", "pytest-asyncio", "twine>=4.0.2"], #pip install -e .[dev]
     },
     python_requires=">=3.7",
     include_package_data=True,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

### Comparing `flusso-0.0.1/test/test_functions.py` & `flusso-0.1.0/test/test_functions.py`

 * *Files identical despite different names*

### Comparing `flusso-0.0.1/test/test_option.py` & `flusso-0.1.0/test/test_option.py`

 * *Files identical despite different names*

### Comparing `flusso-0.0.1/test/test_result.py` & `flusso-0.1.0/test/test_result.py`

 * *Files identical despite different names*

