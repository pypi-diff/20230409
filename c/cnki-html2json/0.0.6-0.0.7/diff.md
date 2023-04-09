# Comparing `tmp/cnki_html2json-0.0.6.tar.gz` & `tmp/cnki_html2json-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnki_html2json-0.0.6.tar", last modified: Thu Apr  6 09:29:25 2023, max compression
+gzip compressed data, was "cnki_html2json-0.0.7.tar", last modified: Sun Apr  9 14:24:59 2023, max compression
```

## Comparing `cnki_html2json-0.0.6.tar` & `cnki_html2json-0.0.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 09:29:25.836012 cnki_html2json-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     5886 2023-04-06 09:29:25.836012 cnki_html2json-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-04-06 09:29:05.000000 cnki_html2json-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 09:29:25.836012 cnki_html2json-0.0.6/cnki_html2json/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 09:29:05.000000 cnki_html2json-0.0.6/cnki_html2json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10606 2023-04-06 09:29:05.000000 cnki_html2json-0.0.6/cnki_html2json/_html2json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-04-06 09:29:05.000000 cnki_html2json-0.0.6/cnki_html2json/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-04-06 09:29:05.000000 cnki_html2json-0.0.6/cnki_html2json/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     9786 2023-04-06 09:29:05.000000 cnki_html2json-0.0.6/cnki_html2json/crawl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-04-06 09:29:05.000000 cnki_html2json-0.0.6/cnki_html2json/parse_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-06 09:29:05.000000 cnki_html2json-0.0.6/cnki_html2json/recognize_slider_coordinate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 09:29:25.836012 cnki_html2json-0.0.6/cnki_html2json.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5886 2023-04-06 09:29:25.000000 cnki_html2json-0.0.6/cnki_html2json.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-06 09:29:25.000000 cnki_html2json-0.0.6/cnki_html2json.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 09:29:25.000000 cnki_html2json-0.0.6/cnki_html2json.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-06 09:29:25.000000 cnki_html2json-0.0.6/cnki_html2json.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-06 09:29:25.000000 cnki_html2json-0.0.6/cnki_html2json.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-06 09:29:25.000000 cnki_html2json-0.0.6/cnki_html2json.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 09:29:25.836012 cnki_html2json-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-04-06 09:29:05.000000 cnki_html2json-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 09:29:25.836012 cnki_html2json-0.0.6/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 09:29:05.000000 cnki_html2json-0.0.6/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-06 09:29:05.000000 cnki_html2json-0.0.6/test/test_html2json.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-06 09:29:05.000000 cnki_html2json-0.0.6/test/test_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:24:59.470739 cnki_html2json-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     5799 2023-04-09 14:24:59.470739 cnki_html2json-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-04-09 14:24:44.000000 cnki_html2json-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:24:59.470739 cnki_html2json-0.0.7/cnki_html2json/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 14:24:44.000000 cnki_html2json-0.0.7/cnki_html2json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10606 2023-04-09 14:24:44.000000 cnki_html2json-0.0.7/cnki_html2json/_html2json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-04-09 14:24:44.000000 cnki_html2json-0.0.7/cnki_html2json/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-04-09 14:24:44.000000 cnki_html2json-0.0.7/cnki_html2json/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9786 2023-04-09 14:24:44.000000 cnki_html2json-0.0.7/cnki_html2json/crawl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-04-09 14:24:44.000000 cnki_html2json-0.0.7/cnki_html2json/parse_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-09 14:24:44.000000 cnki_html2json-0.0.7/cnki_html2json/recognize_slider_coordinate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:24:59.470739 cnki_html2json-0.0.7/cnki_html2json.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5799 2023-04-09 14:24:59.000000 cnki_html2json-0.0.7/cnki_html2json.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-09 14:24:59.000000 cnki_html2json-0.0.7/cnki_html2json.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 14:24:59.000000 cnki_html2json-0.0.7/cnki_html2json.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-09 14:24:59.000000 cnki_html2json-0.0.7/cnki_html2json.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-09 14:24:59.000000 cnki_html2json-0.0.7/cnki_html2json.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-09 14:24:59.000000 cnki_html2json-0.0.7/cnki_html2json.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 14:24:59.470739 cnki_html2json-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-04-09 14:24:44.000000 cnki_html2json-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:24:59.470739 cnki_html2json-0.0.7/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 14:24:44.000000 cnki_html2json-0.0.7/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-09 14:24:44.000000 cnki_html2json-0.0.7/test/test_html2json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-09 14:24:44.000000 cnki_html2json-0.0.7/test/test_metadata.py
```

### Comparing `cnki_html2json-0.0.6/PKG-INFO` & `cnki_html2json-0.0.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnki_html2json
-Version: 0.0.6
+Version: 0.0.7
 Summary: A package to convert cnki html to json
 Home-page: https://github.com/doublessay/cnki-html2json
 Author: WangK2
 Author-email: kw221225@gmail.com
 License: MIT
 Keywords: cnki,text-structure,crawler
 Classifier: Programming Language :: Python :: 3
@@ -134,9 +134,8 @@
 
 | 工具  | 描述 |
 | --- | --- |
 | [vermin](https://github.com/netromdk/vermin) | 从语法层面检测一个项目最低支持的 `python` 版本 |
 
 ## 责任声明
 
-- 请确保本工具用于研究、个人学习等目的，不得用于商业用途
-- 使用者使用本工具所造成的一切后果，由使用者自行承担
+- 使用者使用本工具造成的一切后果，由使用者自行承担
```

### Comparing `cnki_html2json-0.0.6/README.md` & `cnki_html2json-0.0.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -112,9 +112,8 @@
 
 | 工具  | 描述 |
 | --- | --- |
 | [vermin](https://github.com/netromdk/vermin) | 从语法层面检测一个项目最低支持的 `python` 版本 |
 
 ## 责任声明
 
-- 请确保本工具用于研究、个人学习等目的，不得用于商业用途
-- 使用者使用本工具所造成的一切后果，由使用者自行承担
+- 使用者使用本工具造成的一切后果，由使用者自行承担
```

### Comparing `cnki_html2json-0.0.6/cnki_html2json/_html2json.py` & `cnki_html2json-0.0.7/cnki_html2json/_html2json.py`

 * *Files identical despite different names*

### Comparing `cnki_html2json-0.0.6/cnki_html2json/cli.py` & `cnki_html2json-0.0.7/cnki_html2json/cli.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 from cnki_html2json.core import start_crawl
 
 def main():
     parser = argparse.ArgumentParser(description='CNKI crawler. Convert the html format of papers to json format.')
     parser.add_argument('-s','--start_paper_index',type=int,default=1,help='开始下载索引, 默认为1')
     parser.add_argument('-e','--end_paper_index',type=int,default=None,help='结束下载索引, 默认为None, 即下载到最后')
     parser.add_argument('-m','--mode',type=str,default='structure',help='模式: structure|plain|raw, 默认为structure')
+    parser.add_argument('-b','--browser_type',type=str,default='Chrome',help='浏览器类型: Chrome(default)|Firefox|Edge')
     parser.add_argument('-save','--save_path',type=str,default='data',help='文件保存路径, 默认为当前目录的data文件夹')
     parser.add_argument('-wait','--wait_time',type=int,default=120,help='为检索预留的等待时间, 默认为120秒')
-    parser.add_argument('-b','--browser_type',type=str,default='Chrome',help='浏览器类型: Chrome(default)|Firefox|Edge')
     parser.add_argument('--debug',action='store_false')
     args = parser.parse_args()
     start_crawl(start_paper_index = args.start_paper_index,
                 end_paper_index = args.end_paper_index,
                 mode = args.mode,
                 save_path = args.save_path,
                 log = args.debug,
```

### Comparing `cnki_html2json-0.0.6/cnki_html2json/core.py` & `cnki_html2json-0.0.7/cnki_html2json/core.py`

 * *Files identical despite different names*

### Comparing `cnki_html2json-0.0.6/cnki_html2json/crawl.py` & `cnki_html2json-0.0.7/cnki_html2json/crawl.py`

 * *Files identical despite different names*

### Comparing `cnki_html2json-0.0.6/cnki_html2json/parse_metadata.py` & `cnki_html2json-0.0.7/cnki_html2json/parse_metadata.py`

 * *Files identical despite different names*

### Comparing `cnki_html2json-0.0.6/cnki_html2json/recognize_slider_coordinate.py` & `cnki_html2json-0.0.7/cnki_html2json/recognize_slider_coordinate.py`

 * *Files identical despite different names*

### Comparing `cnki_html2json-0.0.6/cnki_html2json.egg-info/PKG-INFO` & `cnki_html2json-0.0.7/cnki_html2json.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnki-html2json
-Version: 0.0.6
+Version: 0.0.7
 Summary: A package to convert cnki html to json
 Home-page: https://github.com/doublessay/cnki-html2json
 Author: WangK2
 Author-email: kw221225@gmail.com
 License: MIT
 Keywords: cnki,text-structure,crawler
 Classifier: Programming Language :: Python :: 3
@@ -134,9 +134,8 @@
 
 | 工具  | 描述 |
 | --- | --- |
 | [vermin](https://github.com/netromdk/vermin) | 从语法层面检测一个项目最低支持的 `python` 版本 |
 
 ## 责任声明
 
-- 请确保本工具用于研究、个人学习等目的，不得用于商业用途
-- 使用者使用本工具所造成的一切后果，由使用者自行承担
+- 使用者使用本工具造成的一切后果，由使用者自行承担
```

### Comparing `cnki_html2json-0.0.6/cnki_html2json.egg-info/SOURCES.txt` & `cnki_html2json-0.0.7/cnki_html2json.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cnki_html2json-0.0.6/setup.py` & `cnki_html2json-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup,find_packages
 
 setup(
     name="cnki_html2json",
     author = "WangK2",
     author_email = "kw221225@gmail.com",
-    version="0.0.6",
+    version="0.0.7",
     description="A package to convert cnki html to json",
     long_description = open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords = ["cnki","text-structure","crawler"],
     license="MIT",
     url="https://github.com/doublessay/cnki-html2json",
     packages=find_packages(),
```

### Comparing `cnki_html2json-0.0.6/test/test_html2json.py` & `cnki_html2json-0.0.7/test/test_html2json.py`

 * *Files identical despite different names*

