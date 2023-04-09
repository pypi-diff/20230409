# Comparing `tmp/yzy-0.0.3.tar.gz` & `tmp/yzy-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yzy-0.0.3.tar", last modified: Sun Apr  9 03:08:48 2023, max compression
+gzip compressed data, was "yzy-0.0.4.tar", last modified: Sun Apr  9 04:25:13 2023, max compression
```

## Comparing `yzy-0.0.3.tar` & `yzy-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 yzy        (501) staff       (20)        0 2023-04-09 03:08:48.506116 yzy-0.0.3/
--rw-r--r--   0 yzy        (501) staff       (20)     1073 2023-04-02 11:39:35.000000 yzy-0.0.3/LICENSE
--rw-r--r--   0 yzy        (501) staff       (20)      767 2023-04-09 03:08:48.505964 yzy-0.0.3/PKG-INFO
--rw-r--r--   0 yzy        (501) staff       (20)      288 2023-04-09 03:08:26.000000 yzy-0.0.3/README.md
--rw-r--r--   0 yzy        (501) staff       (20)      552 2023-04-09 03:07:19.000000 yzy-0.0.3/pyproject.toml
--rw-r--r--   0 yzy        (501) staff       (20)       38 2023-04-09 03:08:48.506177 yzy-0.0.3/setup.cfg
-drwxr-xr-x   0 yzy        (501) staff       (20)        0 2023-04-09 03:08:48.503448 yzy-0.0.3/src/
-drwxr-xr-x   0 yzy        (501) staff       (20)        0 2023-04-09 03:08:48.505056 yzy-0.0.3/src/yzy/
--rw-r--r--   0 yzy        (501) staff       (20)        0 2023-04-02 11:41:50.000000 yzy-0.0.3/src/yzy/__init__.py
--rwx------   0 yzy        (501) staff       (20)     5697 2023-04-09 03:05:07.000000 yzy-0.0.3/src/yzy/arxiv.py
--rwx------   0 yzy        (501) staff       (20)     3793 2023-04-02 12:34:56.000000 yzy-0.0.3/src/yzy/file2md.py
--rwx------   0 yzy        (501) staff       (20)     2933 2023-03-29 09:30:46.000000 yzy-0.0.3/src/yzy/id2md.py
-drwxr-xr-x   0 yzy        (501) staff       (20)        0 2023-04-09 03:08:48.505730 yzy-0.0.3/src/yzy.egg-info/
--rw-r--r--   0 yzy        (501) staff       (20)      767 2023-04-09 03:08:48.000000 yzy-0.0.3/src/yzy.egg-info/PKG-INFO
--rw-r--r--   0 yzy        (501) staff       (20)      229 2023-04-09 03:08:48.000000 yzy-0.0.3/src/yzy.egg-info/SOURCES.txt
--rw-r--r--   0 yzy        (501) staff       (20)        1 2023-04-09 03:08:48.000000 yzy-0.0.3/src/yzy.egg-info/dependency_links.txt
--rw-r--r--   0 yzy        (501) staff       (20)        4 2023-04-09 03:08:48.000000 yzy-0.0.3/src/yzy.egg-info/top_level.txt
+drwxr-xr-x   0 yzy        (501) staff       (20)        0 2023-04-09 04:25:13.170597 yzy-0.0.4/
+-rw-r--r--   0 yzy        (501) staff       (20)     1073 2023-04-02 11:39:35.000000 yzy-0.0.4/LICENSE
+-rw-r--r--   0 yzy        (501) staff       (20)      767 2023-04-09 04:25:13.170457 yzy-0.0.4/PKG-INFO
+-rw-r--r--   0 yzy        (501) staff       (20)      288 2023-04-09 03:08:26.000000 yzy-0.0.4/README.md
+-rw-r--r--   0 yzy        (501) staff       (20)      552 2023-04-09 04:24:53.000000 yzy-0.0.4/pyproject.toml
+-rw-r--r--   0 yzy        (501) staff       (20)       38 2023-04-09 04:25:13.170647 yzy-0.0.4/setup.cfg
+drwxr-xr-x   0 yzy        (501) staff       (20)        0 2023-04-09 04:25:13.168104 yzy-0.0.4/src/
+drwxr-xr-x   0 yzy        (501) staff       (20)        0 2023-04-09 04:25:13.169647 yzy-0.0.4/src/yzy/
+-rw-r--r--   0 yzy        (501) staff       (20)        0 2023-04-02 11:41:50.000000 yzy-0.0.4/src/yzy/__init__.py
+-rwx------   0 yzy        (501) staff       (20)     5820 2023-04-09 04:22:19.000000 yzy-0.0.4/src/yzy/arxiv.py
+-rwx------   0 yzy        (501) staff       (20)     2497 2023-04-09 04:22:05.000000 yzy-0.0.4/src/yzy/file2md.py
+-rwx------   0 yzy        (501) staff       (20)     1767 2023-04-09 04:22:25.000000 yzy-0.0.4/src/yzy/id2md.py
+drwxr-xr-x   0 yzy        (501) staff       (20)        0 2023-04-09 04:25:13.170273 yzy-0.0.4/src/yzy.egg-info/
+-rw-r--r--   0 yzy        (501) staff       (20)      767 2023-04-09 04:25:13.000000 yzy-0.0.4/src/yzy.egg-info/PKG-INFO
+-rw-r--r--   0 yzy        (501) staff       (20)      229 2023-04-09 04:25:13.000000 yzy-0.0.4/src/yzy.egg-info/SOURCES.txt
+-rw-r--r--   0 yzy        (501) staff       (20)        1 2023-04-09 04:25:13.000000 yzy-0.0.4/src/yzy.egg-info/dependency_links.txt
+-rw-r--r--   0 yzy        (501) staff       (20)        4 2023-04-09 04:25:13.000000 yzy-0.0.4/src/yzy.egg-info/top_level.txt
```

### Comparing `yzy-0.0.3/LICENSE` & `yzy-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `yzy-0.0.3/PKG-INFO` & `yzy-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yzy
-Version: 0.0.3
+Version: 0.0.4
 Summary: Utils
 Author-email: Zhiyuan Yang <im.crazyang@gmail.com>
 Project-URL: Homepage, https://github.com/yzy1996/Python-Code
 Project-URL: Bug Tracker, https://github.com/yzy1996/Python-Code/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yzy-0.0.3/pyproject.toml` & `yzy-0.0.4/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "yzy"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Zhiyuan Yang", email="im.crazyang@gmail.com" },
 ]
 description = "Utils"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `yzy-0.0.3/src/yzy/arxiv.py` & `yzy-0.0.4/src/yzy/arxiv.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,47 +1,46 @@
 import re
 from urllib import request
 from pathlib import Path
 import feedparser
 # from urlextract import URLExtract
 
-CONF = 'ICML|NIPS|NeurIPS|ICLR|CVPR|ICCV|ECCV|AAAI|IJCAI|3DV|UAI|WACV|ICASSP|ICIP|ICME|ICPR|ICRA|ICST|ICWSM|IJCNN|IJC'
+CONF = 'ICML|NIPS|NeurIPS|ICLR|CVPR|ICCV|ECCV|AAAI|IJCAI|3DV|UAI|WACV|ICASSP|ICRA'
 
 
 class Information():
     '''
     extract information from arxiv api
     '''
+
     def __init__(self, query_id=None, query_title=None) -> None:
 
         if query_id:
-            self.query_url = f'http://export.arxiv.org/api/query?id_list={query_id}'
+            query_url = f'http://export.arxiv.org/api/query?id_list={query_id}'
         elif query_title:
-            query_title1 = str(query_title)[:-4].replace(' ', '+').replace(
-                '-', '+')
-            self.query_url = f'https://export.arxiv.org/api/query?search_query=ti:{query_title1}&max_results=1'
-
-        self.export_arxiv = request.urlopen(
-            self.query_url).read().decode('utf-8')
-        feed = feedparser.parse(self.export_arxiv)
+            query_title1 = str(query_title)[:-4].replace(' ', '+').replace('-', '+')
+            query_url = f'https://export.arxiv.org/api/query?search_query=ti:{query_title1}&max_results=1'
+
+        export_arxiv = request.urlopen(query_url).read().decode('utf-8')
+        feed = feedparser.parse(export_arxiv)
 
         self.title = re.sub(r'[^\w\s-]', '', feed.entries[0].title)
         self.authors = [author.name for author in feed.entries[0].authors]
         self.abs_url = feed.entries[0].id
         self.pdf_url = self.abs_url.replace('abs', 'pdf')
         self.id_version = self.abs_url[-12:]
         self.year = feed.entries[0].published[:4]
-        
         self.summary = feed.entries[0].summary
 
         try:
             self.comment = feed.entries[0].arxiv_comment
             publish = re.findall(rf'[\s\S]*(({CONF}).*?\d{{4}})[\s\S]*', self.comment)
-            self.publish = publish[0][0] if publish else f'arXiv {self.year}'
+            self.publish = re.sub(r'(\w)(\d{4})', r'\1 \2', publish[0][0]) if publish else f'arXiv {self.year}'
         except:
+            self.publish = f'arXiv {self.year}'
             pass
 
         # self.project_urls = URLExtract().find_urls(self.summary) if self.comment else None
 
     # deprecated
     def _get_arxiv_info_regex(self):
 
@@ -113,16 +112,17 @@
         authors = f'*{authors_str}*  '
 
         print('-', title_url)
         print(' ', publish, authors, '\n')
 
 def read_pdf(filename, update=False):
     '''
-    read pdf and return id, version, text
+    read pdf and return id, text
     '''
+
     from PyPDF2 import PdfReader
     with open(filename, 'rb') as f:
 
         pdf = PdfReader(f)
 
         first_page = pdf.pages[0]
         text_split = first_page.extract_text().split()
@@ -156,27 +156,33 @@
 
 def file2md():
     root_dir = Path('./')
     pdf_list = sorted(root_dir.glob('*.pdf'))
 
     for file in list(pdf_list):
         try:
-            Information(query_title=file)
+            information = Information(query_title=file)
+            information.write_notes()
 
-        except:
-            print('Error: ', file)
+        except Exception as ex:
+            print('Error: ', ex)
             pass
 
 
 def id2md():
     while True:
         id = input("type id: ")
 
-        ## 先判断 id 是否有效，形如：2011.13126
+        # 2011.13126
         if re.findall(r'\d{4}\.\d{5}', id):
 
-            information = Information(id)
-            information.write_notes()
+            try:
+                information = Information(id)
+                information.write_notes()
+
+            except Exception as ex:
+                print('Error: ', ex)
+                pass
 
 
 if __name__ == '__main__':
     check_version()
```

### Comparing `yzy-0.0.3/src/yzy/file2md.py` & `yzy-0.0.4/src/yzy/file2md.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,129 +1,82 @@
 from urllib import request
 import re
 from pathlib import Path
 from PyPDF2 import PdfReader
+import feedparser
 
-CONF = 'ICML|NIPS|NeurIPS|ICLR|CVPR|ICCV|ECCV|AAAI|IJCAI|3DV|UAI'
+CONF = 'ICML|NIPS|NeurIPS|ICLR|CVPR|ICCV|ECCV|AAAI|IJCAI|3DV|UAI|WACV|ICASSP|ICRA'
 
 
 class Information():
     def __init__(self, query_title) -> None:
 
-        query_id, _, _ = self.read_pdf(query_title)
+        query_id = read_pdf(query_title)
 
         if re.findall(r'\d{4}.\d{5}', query_id):
-            self.query_url = f'http://export.arxiv.org/api/query?id_list={query_id}'
-            self.id = query_id
+            query_url = f'http://export.arxiv.org/api/query?id_list={query_id}'
 
         else:
-            # 预处理title去掉 - 等转义符号
-            query_title1 = str(str(query_title)[:-4]).replace(' ', '+').replace('-', '+')
+            query_title1 = str(query_title)[:-4].replace(' ', '+').replace('-', '+')
             self.query_url = f'https://export.arxiv.org/api/query?search_query=ti:{query_title1}&max_results=1'
 
-        self.strInf = request.urlopen(self.query_url).read().decode('utf-8')
+        export_arxiv = request.urlopen(query_url).read().decode('utf-8')
+        feed = feedparser.parse(export_arxiv)
 
-        self._update()
-
-    def _update(self):
-
-        if re.findall(r'<entry>[\s\S]*</entry>', self.strInf):  # 匹配到了内容
-
-            Id = r'<id>http://arxiv.org/abs/(.*)</id>'
-            Title = r'<title>([\s\S]*)</title>'  # 有时候名字太长了，会换行
-            Authors = r'<author>\s*<name>(.*)</name>\s*</author>'
-            Year = r'<published>(\d{4}).*</published>'
-
-            id_version = re.findall(Id, self.strInf)[0]
-            id = id_version[0:-2]
-
-            title = re.findall(Title, self.strInf)[0]
-            title = re.sub(r'\n\s', '', title)  # 去掉换行
-            title_sub = re.sub(r'[^\w\s-]', '', title)  # 去掉标点
-
-            authors = re.findall(Authors, self.strInf)
-            year = re.findall(Year, self.strInf)[0]
-
-            self.id_version = id_version
-            self.id = id
-            self.title = title
-            self.title_sub = title_sub
-            self.authors = authors
-            self.year = year
-            self.publish = ''
-
-            self.abs_url = f'https://arxiv.org/abs/{self.id}'
-            self.pdf_url = f'https://arxiv.org/pdf/{self.id}'
-
-            self.write_notes()
-
-        else:
+        self.title = re.sub(r'[^\w\s-]', '', feed.entries[0].title)
+        self.authors = [author.name for author in feed.entries[0].authors]
+        self.abs_url = feed.entries[0].id
+        self.pdf_url = self.abs_url.replace('abs', 'pdf')
+        self.id_version = self.abs_url[-12:]
+        self.year = feed.entries[0].published[:4]
+        self.summary = feed.entries[0].summary
+
+        try:
+            self.comment = feed.entries[0].arxiv_comment
+            publish = re.findall(rf'[\s\S]*(({CONF}).*?\d{{4}})[\s\S]*', self.comment)
+            self.publish = re.sub(r'(\w)(\d{4})', r'\1 \2', publish[0][0]) if publish else f'arXiv {self.year}'
+        except:
+            self.publish = f'arXiv {self.year}'
             pass
 
-    def _get_publish(self):
-
-        # 读取 txt 预定义会议名称
-
-        # with open(r'conf_list.txt') as f:
-        #     lines = [line.strip() for line in f]
-        # reg = '|'.join(lines)
-
-        # obtain form arxiv comments
-        Publish = f'<arxiv:comment xmlns:arxiv="http://arxiv.org/schemas/atom">[\s\S]*(({CONF}).*?\d{{4}})[\s\S]*</arxiv:comment>'
-        publish = re.findall(Publish, self.strInf)
-
-        if publish != []:
-            self.publish = publish[0][0]
-
-            # 处理例如 CVPR2020 -> CVPR 2020
-            self.publish = re.sub(r'(\w)(\d{4})', r'\1 \2', self.publish)
-
-        else:
-            # 未来对接整个互联网搜索
-            self.publish = 'arXiv ' + self.year
-
     def write_notes(self):
 
-        self._get_publish()
-
-        # 组合处理
         title_url = f'[{self.title}]({self.abs_url})  '
-
         publish = f'**[`{self.publish}`]**'
-
         authors = ', '.join(self.authors)
         authors = f'*{authors}*'
 
         print('-', title_url)
         print(' ', publish, authors, '\n')
 
-    def read_pdf(self, filename):
-        '''
-        读取pdf文件，返回id, version, text
-        '''
-
-        with open(filename, 'rb') as f:
-
-            pdf = PdfReader(f)
-
-            first_page = pdf.pages[0]
-            text = first_page.extract_text()
-            text_split = text.split()
-            id_version_local = text_split[-5]
-            id_version = id_version_local.split(':')[-1]
 
-            id = id_version[0:-2] if id_version else []
-            version = id_version[-1] if id_version else []
+def read_pdf(filename, update=False):
+    '''
+    read pdf and return id
+    '''
+
+    with open(filename, 'rb') as f:
+
+        pdf = PdfReader(f)
+
+        first_page = pdf.pages[0]
+        text_split = first_page.extract_text().split()
+        str_id = text_split[-5]
+        id_version_local = re.findall(r'\d{4}\.\d{5}v\d{1}', str_id)[0]
+        id = id_version_local[:-2]
 
-        return id, version, text
+    return id
 
 
 if __name__ == "__main__":
 
     root_dir = Path('./')
     pdf_list = sorted(root_dir.glob('*.pdf'))
 
     for file in list(pdf_list):
+        try:
+            information = Information(query_title=file)
+            information.write_notes()
 
-            Information(query_title=file)
-
-
+        except Exception as ex:
+            print('Error: ', ex)
+            pass
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `yzy-0.0.3/src/yzy.egg-info/PKG-INFO` & `yzy-0.0.4/src/yzy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yzy
-Version: 0.0.3
+Version: 0.0.4
 Summary: Utils
 Author-email: Zhiyuan Yang <im.crazyang@gmail.com>
 Project-URL: Homepage, https://github.com/yzy1996/Python-Code
 Project-URL: Bug Tracker, https://github.com/yzy1996/Python-Code/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

