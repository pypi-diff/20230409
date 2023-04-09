# Comparing `tmp/paper-qa-0.1.0.tar.gz` & `tmp/paper-qa-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paper-qa-0.1.0.tar", last modified: Sun Mar 26 00:53:45 2023, max compression
+gzip compressed data, was "paper-qa-1.0.0.tar", last modified: Sun Apr  9 19:59:35 2023, max compression
```

## Comparing `paper-qa-0.1.0.tar` & `paper-qa-1.0.0.tar`

### file list

```diff
@@ -1,21 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 00:53:45.708383 paper-qa-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-03-26 00:53:22.000000 paper-qa-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7948 2023-03-26 00:53:45.708383 paper-qa-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7513 2023-03-26 00:53:22.000000 paper-qa-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 00:53:45.708383 paper-qa-0.1.0/paper_qa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7948 2023-03-26 00:53:45.000000 paper-qa-0.1.0/paper_qa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-03-26 00:53:45.000000 paper-qa-0.1.0/paper_qa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-26 00:53:45.000000 paper-qa-0.1.0/paper_qa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-26 00:53:45.000000 paper-qa-0.1.0/paper_qa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-26 00:53:45.000000 paper-qa-0.1.0/paper_qa.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 00:53:45.708383 paper-qa-0.1.0/paperqa/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-26 00:53:22.000000 paper-qa-0.1.0/paperqa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13743 2023-03-26 00:53:22.000000 paper-qa-0.1.0/paperqa/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-03-26 00:53:22.000000 paper-qa-0.1.0/paperqa/qaprompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-03-26 00:53:22.000000 paper-qa-0.1.0/paperqa/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-03-26 00:53:22.000000 paper-qa-0.1.0/paperqa/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-26 00:53:22.000000 paper-qa-0.1.0/paperqa/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-26 00:53:45.708383 paper-qa-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-03-26 00:53:22.000000 paper-qa-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 00:53:45.708383 paper-qa-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7670 2023-03-26 00:53:22.000000 paper-qa-0.1.0/tests/test_paperqa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:59:35.497224 paper-qa-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-09 19:59:04.000000 paper-qa-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9954 2023-04-09 19:59:35.493224 paper-qa-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9519 2023-04-09 19:59:04.000000 paper-qa-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:59:35.493224 paper-qa-1.0.0/paper_qa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9954 2023-04-09 19:59:35.000000 paper-qa-1.0.0/paper_qa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-09 19:59:35.000000 paper-qa-1.0.0/paper_qa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 19:59:35.000000 paper-qa-1.0.0/paper_qa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-09 19:59:35.000000 paper-qa-1.0.0/paper_qa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-09 19:59:35.000000 paper-qa-1.0.0/paper_qa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:59:35.493224 paper-qa-1.0.0/paperqa/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-09 19:59:04.000000 paper-qa-1.0.0/paperqa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-04-09 19:59:04.000000 paper-qa-1.0.0/paperqa/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:59:35.493224 paper-qa-1.0.0/paperqa/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-09 19:59:04.000000 paper-qa-1.0.0/paperqa/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9682 2023-04-09 19:59:04.000000 paper-qa-1.0.0/paperqa/contrib/zotero.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17412 2023-04-09 19:59:04.000000 paper-qa-1.0.0/paperqa/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-09 19:59:04.000000 paper-qa-1.0.0/paperqa/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-04-09 19:59:04.000000 paper-qa-1.0.0/paperqa/qaprompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7004 2023-04-09 19:59:04.000000 paper-qa-1.0.0/paperqa/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-04-09 19:59:04.000000 paper-qa-1.0.0/paperqa/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-09 19:59:04.000000 paper-qa-1.0.0/paperqa/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 19:59:35.497224 paper-qa-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-09 19:59:04.000000 paper-qa-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:59:35.493224 paper-qa-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9477 2023-04-09 19:59:04.000000 paper-qa-1.0.0/tests/test_paperqa.py
```

### Comparing `paper-qa-0.1.0/LICENSE` & `paper-qa-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `paper-qa-0.1.0/PKG-INFO` & `paper-qa-1.0.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-qa
-Version: 0.1.0
+Version: 1.0.0
 Summary: LLM Chain for answering questions from docs 
 Home-page: https://github.com/whitead/paper-qa
 Author: Andrew White
 Author-email: white.d.andrew@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -31,17 +31,14 @@
 create summary of each passage relevant to query -> put summaries into prompt -> generate answer
 ```
 
 ## Hugging Face Demo
 
 [Hugging Face Demo](https://huggingface.co/spaces/whitead/paper-qa)
 
-
-![image](https://user-images.githubusercontent.com/908389/218957863-4aa2fa2c-14cf-4b0d-82fd-bf837f5f550b.png)
-
 ## Example
 
 Question: How can carbon nanotubes be manufactured at a large scale?
 
 Carbon nanotubes can be manufactured at a large scale using the electric-arc technique (Journet6644). This technique involves creating an arc between two electrodes in a reactor under a helium atmosphere and using a mixture of a metallic catalyst and graphite powder in the anode. Yields of 80% of entangled carbon filaments can be achieved, which consist of smaller aligned SWNTs self-organized into bundle-like crystallites (Journet6644). Additionally, carbon nanotubes can be synthesized and self-assembled using various methods such as DNA-mediated self-assembly, nanoparticle-assisted alignment, chemical self-assembly, and electro-addressed functionalization (Tulevski2007). These methods have been used to fabricate large-area nanostructured arrays, high-density integration, and freestanding networks (Tulevski2007). 98% semiconducting CNT network solution can also be used and is separated from metallic nanotubes using a density gradient ultracentrifugation approach (Chen2014). The substrate is incubated in the solution and then rinsed with deionized water and dried with N2 air gun, leaving a uniform carbon network (Chen2014).
 
 ### References
@@ -92,15 +89,68 @@
 docs.query("What manufacturing challenges are unique to bispecific antibodies?", k = 5, max_sources = 2)
 ```
 
 ## Where do I get papers?
 
 Well that's a really good question! It's probably best to just download PDFs of papers you think will help answer your question and start from there.
 
-If you want to do it automatically, I've found an unrelated project called [paper-scraper](https://github.com/blackadad/paper-scraper) that looks
+### Zotero
+
+If you use [Zotero](https://www.zotero.org/) to organize your personal bibliography,
+you can use the `paperqa.contrib.ZoteroDB` to query papers from your library,
+which relies on [pyzotero](https://github.com/urschrei/pyzotero).
+
+First, note that `paperqa` parses the PDFs of papers to store in the database,
+so all relevant papers should have PDFs stored inside your database.
+You can get Zotero to automatically do this by highlighting the references
+you wish to retrieve, right clicking, and selecting *"Find Available PDFs"*.
+You can also manually drag-and-drop PDFs onto each reference.
+
+To download papers, you need to get an API key for your account.
+
+1. Get your library ID, and set it as the environment variable `ZOTERO_USER_ID`.
+    - For personal libraries, this ID is given [here](https://www.zotero.org/settings/keys) at the part "*Your userID for use in API calls is XXXXXX*".
+    - For group libraries, go to your group page `https://www.zotero.org/groups/groupname`, and hover over the settings link. The ID is the integer after /groups/. (*h/t pyzotero!*)
+2. Create a new API key [here](https://www.zotero.org/settings/keys/new) and set it as the environment variable `ZOTERO_API_KEY`.
+    - The key will need read access to the library.
+
+With this, we can download papers from our library and add them to `paperqa`:
+
+```py
+from paperqa.contrib import ZoteroDB
+
+docs = paperqa.Docs()
+zotero = ZoteroDB(library_type="user")  # "group" if group library
+
+for item in zotero.iterate(limit=20):
+    docs.add(item.pdf, key=item.key)
+```
+
+which will download the first 20 papers in your Zotero database and add
+them to the `Docs` object.
+
+We can also do specific queries of our Zotero library and iterate over the results:
+
+```py
+for item in zotero.iterate(
+        q="large language models",
+        qmode="everything", 
+        sort="date",
+        direction="desc",
+        limit=100,
+):
+    print("Adding", item.title)
+    docs.add(item.pdf, key=item.key)
+```
+
+You can read more about the search syntax by typing `zotero.iterate?` in IPython.
+
+### Paper Scraper
+
+If you want to search for papers outside of your own collection, I've found an unrelated project called [paper-scraper](https://github.com/blackadad/paper-scraper) that looks
 like it might help. But beware, this project looks like it uses some scraping tools that may violate publisher's rights or be in a gray area of legality.
 
 ```py
 keyword_search = 'bispecific antibody manufacture'
 papers = paperscraper.search_papers(keyword_search)
 docs = paperqa.Docs()
 for path,data in papers.items():
@@ -113,15 +163,15 @@
 print(answer.formatted_answer)
 ```
 
 ## FAQ
 
 ### How is this different from LlamaIndex?
 
-It's not that different! This is similar to the tree response method in LlamaIndex. I just have included some prompts I find useful, readers that give page numbers/line numbers, and am focused on one tasks - answering technical questions with cited sources.
+It's not that different! This is similar to the tree response method in LlamaIndex. I just have included some prompts I find useful, readers that give page numbers/line numbers, and am focused on one task - answering technical questions with cited sources.
 
 ### How is this different from LangChain?
 
 It's not! We use langchain to abstract the LLMS, and the process is very similar to the `map_reduce` chain in LangChain.
 
 ### Caching
```

### Comparing `paper-qa-0.1.0/README.md` & `paper-qa-1.0.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -17,17 +17,14 @@
 create summary of each passage relevant to query -> put summaries into prompt -> generate answer
 ```
 
 ## Hugging Face Demo
 
 [Hugging Face Demo](https://huggingface.co/spaces/whitead/paper-qa)
 
-
-![image](https://user-images.githubusercontent.com/908389/218957863-4aa2fa2c-14cf-4b0d-82fd-bf837f5f550b.png)
-
 ## Example
 
 Question: How can carbon nanotubes be manufactured at a large scale?
 
 Carbon nanotubes can be manufactured at a large scale using the electric-arc technique (Journet6644). This technique involves creating an arc between two electrodes in a reactor under a helium atmosphere and using a mixture of a metallic catalyst and graphite powder in the anode. Yields of 80% of entangled carbon filaments can be achieved, which consist of smaller aligned SWNTs self-organized into bundle-like crystallites (Journet6644). Additionally, carbon nanotubes can be synthesized and self-assembled using various methods such as DNA-mediated self-assembly, nanoparticle-assisted alignment, chemical self-assembly, and electro-addressed functionalization (Tulevski2007). These methods have been used to fabricate large-area nanostructured arrays, high-density integration, and freestanding networks (Tulevski2007). 98% semiconducting CNT network solution can also be used and is separated from metallic nanotubes using a density gradient ultracentrifugation approach (Chen2014). The substrate is incubated in the solution and then rinsed with deionized water and dried with N2 air gun, leaving a uniform carbon network (Chen2014).
 
 ### References
@@ -78,15 +75,68 @@
 docs.query("What manufacturing challenges are unique to bispecific antibodies?", k = 5, max_sources = 2)
 ```
 
 ## Where do I get papers?
 
 Well that's a really good question! It's probably best to just download PDFs of papers you think will help answer your question and start from there.
 
-If you want to do it automatically, I've found an unrelated project called [paper-scraper](https://github.com/blackadad/paper-scraper) that looks
+### Zotero
+
+If you use [Zotero](https://www.zotero.org/) to organize your personal bibliography,
+you can use the `paperqa.contrib.ZoteroDB` to query papers from your library,
+which relies on [pyzotero](https://github.com/urschrei/pyzotero).
+
+First, note that `paperqa` parses the PDFs of papers to store in the database,
+so all relevant papers should have PDFs stored inside your database.
+You can get Zotero to automatically do this by highlighting the references
+you wish to retrieve, right clicking, and selecting *"Find Available PDFs"*.
+You can also manually drag-and-drop PDFs onto each reference.
+
+To download papers, you need to get an API key for your account.
+
+1. Get your library ID, and set it as the environment variable `ZOTERO_USER_ID`.
+    - For personal libraries, this ID is given [here](https://www.zotero.org/settings/keys) at the part "*Your userID for use in API calls is XXXXXX*".
+    - For group libraries, go to your group page `https://www.zotero.org/groups/groupname`, and hover over the settings link. The ID is the integer after /groups/. (*h/t pyzotero!*)
+2. Create a new API key [here](https://www.zotero.org/settings/keys/new) and set it as the environment variable `ZOTERO_API_KEY`.
+    - The key will need read access to the library.
+
+With this, we can download papers from our library and add them to `paperqa`:
+
+```py
+from paperqa.contrib import ZoteroDB
+
+docs = paperqa.Docs()
+zotero = ZoteroDB(library_type="user")  # "group" if group library
+
+for item in zotero.iterate(limit=20):
+    docs.add(item.pdf, key=item.key)
+```
+
+which will download the first 20 papers in your Zotero database and add
+them to the `Docs` object.
+
+We can also do specific queries of our Zotero library and iterate over the results:
+
+```py
+for item in zotero.iterate(
+        q="large language models",
+        qmode="everything", 
+        sort="date",
+        direction="desc",
+        limit=100,
+):
+    print("Adding", item.title)
+    docs.add(item.pdf, key=item.key)
+```
+
+You can read more about the search syntax by typing `zotero.iterate?` in IPython.
+
+### Paper Scraper
+
+If you want to search for papers outside of your own collection, I've found an unrelated project called [paper-scraper](https://github.com/blackadad/paper-scraper) that looks
 like it might help. But beware, this project looks like it uses some scraping tools that may violate publisher's rights or be in a gray area of legality.
 
 ```py
 keyword_search = 'bispecific antibody manufacture'
 papers = paperscraper.search_papers(keyword_search)
 docs = paperqa.Docs()
 for path,data in papers.items():
@@ -99,15 +149,15 @@
 print(answer.formatted_answer)
 ```
 
 ## FAQ
 
 ### How is this different from LlamaIndex?
 
-It's not that different! This is similar to the tree response method in LlamaIndex. I just have included some prompts I find useful, readers that give page numbers/line numbers, and am focused on one tasks - answering technical questions with cited sources.
+It's not that different! This is similar to the tree response method in LlamaIndex. I just have included some prompts I find useful, readers that give page numbers/line numbers, and am focused on one task - answering technical questions with cited sources.
 
 ### How is this different from LangChain?
 
 It's not! We use langchain to abstract the LLMS, and the process is very similar to the `map_reduce` chain in LangChain.
 
 ### Caching
```

### Comparing `paper-qa-0.1.0/paper_qa.egg-info/PKG-INFO` & `paper-qa-1.0.0/paper_qa.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-qa
-Version: 0.1.0
+Version: 1.0.0
 Summary: LLM Chain for answering questions from docs 
 Home-page: https://github.com/whitead/paper-qa
 Author: Andrew White
 Author-email: white.d.andrew@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -31,17 +31,14 @@
 create summary of each passage relevant to query -> put summaries into prompt -> generate answer
 ```
 
 ## Hugging Face Demo
 
 [Hugging Face Demo](https://huggingface.co/spaces/whitead/paper-qa)
 
-
-![image](https://user-images.githubusercontent.com/908389/218957863-4aa2fa2c-14cf-4b0d-82fd-bf837f5f550b.png)
-
 ## Example
 
 Question: How can carbon nanotubes be manufactured at a large scale?
 
 Carbon nanotubes can be manufactured at a large scale using the electric-arc technique (Journet6644). This technique involves creating an arc between two electrodes in a reactor under a helium atmosphere and using a mixture of a metallic catalyst and graphite powder in the anode. Yields of 80% of entangled carbon filaments can be achieved, which consist of smaller aligned SWNTs self-organized into bundle-like crystallites (Journet6644). Additionally, carbon nanotubes can be synthesized and self-assembled using various methods such as DNA-mediated self-assembly, nanoparticle-assisted alignment, chemical self-assembly, and electro-addressed functionalization (Tulevski2007). These methods have been used to fabricate large-area nanostructured arrays, high-density integration, and freestanding networks (Tulevski2007). 98% semiconducting CNT network solution can also be used and is separated from metallic nanotubes using a density gradient ultracentrifugation approach (Chen2014). The substrate is incubated in the solution and then rinsed with deionized water and dried with N2 air gun, leaving a uniform carbon network (Chen2014).
 
 ### References
@@ -92,15 +89,68 @@
 docs.query("What manufacturing challenges are unique to bispecific antibodies?", k = 5, max_sources = 2)
 ```
 
 ## Where do I get papers?
 
 Well that's a really good question! It's probably best to just download PDFs of papers you think will help answer your question and start from there.
 
-If you want to do it automatically, I've found an unrelated project called [paper-scraper](https://github.com/blackadad/paper-scraper) that looks
+### Zotero
+
+If you use [Zotero](https://www.zotero.org/) to organize your personal bibliography,
+you can use the `paperqa.contrib.ZoteroDB` to query papers from your library,
+which relies on [pyzotero](https://github.com/urschrei/pyzotero).
+
+First, note that `paperqa` parses the PDFs of papers to store in the database,
+so all relevant papers should have PDFs stored inside your database.
+You can get Zotero to automatically do this by highlighting the references
+you wish to retrieve, right clicking, and selecting *"Find Available PDFs"*.
+You can also manually drag-and-drop PDFs onto each reference.
+
+To download papers, you need to get an API key for your account.
+
+1. Get your library ID, and set it as the environment variable `ZOTERO_USER_ID`.
+    - For personal libraries, this ID is given [here](https://www.zotero.org/settings/keys) at the part "*Your userID for use in API calls is XXXXXX*".
+    - For group libraries, go to your group page `https://www.zotero.org/groups/groupname`, and hover over the settings link. The ID is the integer after /groups/. (*h/t pyzotero!*)
+2. Create a new API key [here](https://www.zotero.org/settings/keys/new) and set it as the environment variable `ZOTERO_API_KEY`.
+    - The key will need read access to the library.
+
+With this, we can download papers from our library and add them to `paperqa`:
+
+```py
+from paperqa.contrib import ZoteroDB
+
+docs = paperqa.Docs()
+zotero = ZoteroDB(library_type="user")  # "group" if group library
+
+for item in zotero.iterate(limit=20):
+    docs.add(item.pdf, key=item.key)
+```
+
+which will download the first 20 papers in your Zotero database and add
+them to the `Docs` object.
+
+We can also do specific queries of our Zotero library and iterate over the results:
+
+```py
+for item in zotero.iterate(
+        q="large language models",
+        qmode="everything", 
+        sort="date",
+        direction="desc",
+        limit=100,
+):
+    print("Adding", item.title)
+    docs.add(item.pdf, key=item.key)
+```
+
+You can read more about the search syntax by typing `zotero.iterate?` in IPython.
+
+### Paper Scraper
+
+If you want to search for papers outside of your own collection, I've found an unrelated project called [paper-scraper](https://github.com/blackadad/paper-scraper) that looks
 like it might help. But beware, this project looks like it uses some scraping tools that may violate publisher's rights or be in a gray area of legality.
 
 ```py
 keyword_search = 'bispecific antibody manufacture'
 papers = paperscraper.search_papers(keyword_search)
 docs = paperqa.Docs()
 for path,data in papers.items():
@@ -113,15 +163,15 @@
 print(answer.formatted_answer)
 ```
 
 ## FAQ
 
 ### How is this different from LlamaIndex?
 
-It's not that different! This is similar to the tree response method in LlamaIndex. I just have included some prompts I find useful, readers that give page numbers/line numbers, and am focused on one tasks - answering technical questions with cited sources.
+It's not that different! This is similar to the tree response method in LlamaIndex. I just have included some prompts I find useful, readers that give page numbers/line numbers, and am focused on one task - answering technical questions with cited sources.
 
 ### How is this different from LangChain?
 
 It's not! We use langchain to abstract the LLMS, and the process is very similar to the `map_reduce` chain in LangChain.
 
 ### Caching
```

### Comparing `paper-qa-0.1.0/paperqa/docs.py` & `paper-qa-1.0.0/paperqa/docs.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 from typing import List, Optional, Tuple, Dict, Callable, Any, Union
 from functools import reduce
 import os
-import os
+import sys
+import asyncio
 from pathlib import Path
 import re
+from .paths import CACHE_PATH
 from .utils import maybe_is_text, maybe_is_truncated
 from .qaprompts import (
     summary_prompt,
     qa_prompt,
     search_prompt,
     citation_prompt,
+    select_paper_prompt,
     make_chain,
 )
 from dataclasses import dataclass
 from .readers import read_doc
 from langchain.vectorstores import FAISS
 from langchain.embeddings.openai import OpenAIEmbeddings
+from langchain.embeddings.base import Embeddings
 from langchain.chat_models import ChatOpenAI
 from langchain.llms.base import LLM
 from langchain.chains import LLMChain
 from langchain.callbacks import get_openai_callback
 from langchain.cache import SQLiteCache
 import langchain
 from datetime import datetime
 
-CACHE_PATH = Path.home() / ".paperqa" / "llm_cache.db"
 os.makedirs(os.path.dirname(CACHE_PATH), exist_ok=True)
 langchain.llm_cache = SQLiteCache(CACHE_PATH)
 
 
 @dataclass
 class Answer:
     """A class to hold the answer to a question."""
@@ -37,14 +40,15 @@
     answer: str = ""
     context: str = ""
     contexts: List[Any] = None
     references: str = ""
     formatted_answer: str = ""
     passages: Dict[str, str] = None
     tokens: int = 0
+    cost: float = 0
 
     def __post_init__(self):
         """Initialize the answer."""
         if self.contexts is None:
             self.contexts = []
         if self.passages is None:
             self.passages = {}
@@ -56,41 +60,44 @@
 
 class Docs:
     """A collection of documents to be used for answering questions."""
 
     def __init__(
         self,
         chunk_size_limit: int = 3000,
-        llm: Optional[LLM] = None,
-        summary_llm: Optional[LLM] = None,
+        llm: Optional[Union[LLM, str]] = None,
+        summary_llm: Optional[Union[LLM, str]] = None,
         name: str = "default",
         index_path: Optional[Path] = None,
-        model_name: str = "gpt-3.5-turbo",
+        embeddings: Optional[Embeddings] = None,
     ) -> None:
         """Initialize the collection of documents.
 
 
 
         Args:
             chunk_size_limit: The maximum number of characters to use for a single chunk of text.
             llm: The language model to use for answering questions. Default - OpenAI chat-gpt-turbo
             summary_llm: The language model to use for summarizing documents. If None, llm is used.
             name: The name of the collection.
             index_path: The path to the index file IF pickled. If None, defaults to using name in $HOME/.paperqa/name
-            model_name: The name of the model to use assuming OpenAI. Default - gpt-3.5-turbo
         """
         self.docs = dict()
         self.chunk_size_limit = chunk_size_limit
         self.keys = set()
         self._faiss_index = None
+        self._doc_index = None
         self.update_llm(llm, summary_llm)
         if index_path is None:
             index_path = Path.home() / ".paperqa" / name
         self.index_path = index_path
         self.name = name
+        if embeddings is None:
+            embeddings = OpenAIEmbeddings()
+        self.embeddings = embeddings
 
     def update_llm(
         self,
         llm: Optional[Union[LLM, str]] = None,
         summary_llm: Optional[Union[LLM, str]] = None,
     ) -> None:
         """Update the LLM for answering questions."""
@@ -165,119 +172,193 @@
             raise ValueError(
                 f"This does not look like a text document: {path}. Path disable_check to ignore this error."
             )
 
         self.docs[path] = dict(texts=texts, metadata=metadata, key=key)
         if self._faiss_index is not None:
             self._faiss_index.add_texts(texts, metadatas=metadata)
+        if self._doc_index is not None:
+            self._doc_index.add_texts([citation], metadatas=[{"key": key}])
 
     def clear(self) -> None:
         """Clear the collection of documents."""
         self.docs = dict()
         self.keys = set()
         self._faiss_index = None
+        self._doc_index = None
         # delete index file
         pkl = self.index_path / "index.pkl"
         if pkl.exists():
             pkl.unlink()
         fs = self.index_path / "index.faiss"
         if fs.exists():
             fs.unlink()
 
-    @property
     def doc_previews(self) -> List[Tuple[int, str, str]]:
         """Return a list of tuples of (key, citation) for each document."""
         return [
             (
                 len(doc["texts"]),
                 doc["metadata"][0]["dockey"],
                 doc["metadata"][0]["citation"],
             )
             for doc in self.docs.values()
         ]
 
+    def doc_match(self, query: str, k: int = 25) -> List[str]:
+        """Return a list of documents that match the query."""
+        if len(self.docs) == 0:
+            return ''
+        if self._doc_index is None:
+            texts = [doc["metadata"][0]["citation"] for doc in self.docs.values()]
+            metadatas = [
+                {"key": doc["metadata"][0]["dockey"]} for doc in self.docs.values()
+            ]
+            self._doc_index = FAISS.from_texts(
+                texts, metadatas=metadatas, embedding=self.embeddings
+            )
+        docs = self._doc_index.max_marginal_relevance_search(query, k=k)
+        chain = make_chain(select_paper_prompt, self.summary_llm)
+        papers = [f"{d.metadata['key']}: {d.page_content}" for d in docs]
+        result = chain.run(instructions=query, papers="\n".join(papers))
+        return result
+
     # to pickle, we have to save the index as a file
+
     def __getstate__(self):
         if self._faiss_index is None and len(self.docs) > 0:
             self._build_faiss_index()
         state = self.__dict__.copy()
         if self._faiss_index is not None:
             state["_faiss_index"].save_local(self.index_path)
         del state["_faiss_index"]
+        del state["_doc_index"]
         # remove LLMs (they can have callbacks, which can't be pickled)
         del state["summary_chain"]
         del state["qa_chain"]
         del state["cite_chain"]
         del state["search_chain"]
         return state
 
     def __setstate__(self, state):
         self.__dict__.update(state)
         try:
-            self._faiss_index = FAISS.load_local(self.index_path, OpenAIEmbeddings())
+            self._faiss_index = FAISS.load_local(self.index_path, self.embeddings)
         except:
             # they use some special exception type, but I don't want to import it
             self._faiss_index = None
-        self.update_llm("gpt-3.5-turbo")
+        self.update_llm(None, None)
 
     def _build_faiss_index(self):
         if self._faiss_index is None:
             texts = reduce(
                 lambda x, y: x + y, [doc["texts"] for doc in self.docs.values()], []
             )
             metadatas = reduce(
                 lambda x, y: x + y, [doc["metadata"] for doc in self.docs.values()], []
             )
             self._faiss_index = FAISS.from_texts(
-                texts, OpenAIEmbeddings(), metadatas=metadatas
+                texts, self.embeddings, metadatas=metadatas
             )
 
     def get_evidence(
         self,
         answer: Answer,
         k: int = 3,
         max_sources: int = 5,
         marginal_relevance: bool = True,
+        key_filter: Optional[List[str]] = None,
+    ) -> str:
+        # special case for jupyter notebooks
+        if "get_ipython" in globals() or "google.colab" in sys.modules:
+            import nest_asyncio
+            nest_asyncio.apply()
+        try:
+            loop = asyncio.get_event_loop()
+        except RuntimeError:
+            loop = asyncio.new_event_loop()
+            asyncio.set_event_loop(loop)
+        return loop.run_until_complete(
+            self.aget_evidence(
+                answer,
+                k=k,
+                max_sources=max_sources,
+                marginal_relevance=marginal_relevance,
+                key_filter=key_filter,
+            )
+        )
+
+    async def aget_evidence(
+        self,
+        answer: Answer,
+        k: int = 3,
+        max_sources: int = 5,
+        marginal_relevance: bool = True,
+        key_filter: Optional[List[str]] = None,
     ) -> str:
+        if len(self.docs) == 0:
+            return answer
         if self._faiss_index is None:
             self._build_faiss_index()
-
+        _k = k
+        if key_filter is not None:
+            _k = k * 10  # heuristic
         # want to work through indices but less k
         if marginal_relevance:
             docs = self._faiss_index.max_marginal_relevance_search(
-                answer.question, k=k, fetch_k=5 * k
+                answer.question, k=_k, fetch_k=5 * _k
             )
         else:
             docs = self._faiss_index.similarity_search(
-                answer.question, k=k, fetch_k=5 * k
+                answer.question, k=_k, fetch_k=5 * _k
             )
-        for doc in docs:
+
+        async def process(doc):
+            if key_filter is not None and doc.metadata["dockey"] not in key_filter:
+                return None
+            # check if it is already in answer (possible in agent setting)
+            if doc.metadata["key"] in [c[0] for c in answer.contexts]:
+                return None
             c = (
                 doc.metadata["key"],
                 doc.metadata["citation"],
-                self.summary_chain.run(
+                await self.summary_chain.arun(
                     question=answer.question,
                     context_str=doc.page_content,
                     citation=doc.metadata["citation"],
                 ),
                 doc.page_content,
             )
             if "Not applicable" not in c[2]:
+                return c
+            return None
+
+        with get_openai_callback() as cb:
+            contexts = await asyncio.gather(*[process(doc) for doc in docs])
+        answer.tokens += cb.total_tokens
+        answer.cost += cb.total_cost
+        contexts = [c for c in contexts if c is not None]
+        if len(contexts) == 0:
+            return answer
+        contexts = sorted(contexts, key=lambda x: x[2], reverse=True)
+        contexts = contexts[:max_sources]
+        # add to answer (if not already there)
+        keys = [c[0] for c in answer.contexts]
+        for c in contexts:
+            if c[0] not in keys:
                 answer.contexts.append(c)
-                yield answer
-            if len(answer.contexts) == max_sources:
-                break
+
         context_str = "\n\n".join(
             [f"{k}: {s}" for k, c, s, t in answer.contexts if "Not applicable" not in s]
         )
         valid_keys = [k for k, c, s, t in answer.contexts if "Not applicable" not in s]
         if len(valid_keys) > 0:
             context_str += "\n\nValid keys: " + ", ".join(valid_keys)
         answer.context = context_str
-        yield answer
+        return answer
 
     def generate_search_query(self, query: str) -> List[str]:
         """Generate a list of search strings that can be used to find
         relevant papers.
 
         Args:
             query (str): The query to generate search strings for.
@@ -285,82 +366,87 @@
 
         search_query = self.search_chain.run(question=query)
         queries = [s for s in search_query.split("\n") if len(s) > 3]
         # remove 2., 3. from queries
         queries = [re.sub(r"^\d+\.\s*", "", q) for q in queries]
         return queries
 
-    def query_gen(
+    def query(
         self,
         query: str,
         k: int = 10,
         max_sources: int = 5,
         length_prompt: str = "about 100 words",
         marginal_relevance: bool = True,
+        answer: Optional[Answer] = None,
+        key_filter: Optional[bool] = None,
     ):
-        yield from self._query(
-            query,
-            k=k,
-            max_sources=max_sources,
-            length_prompt=length_prompt,
-            marginal_relevance=marginal_relevance,
+        # special case for jupyter notebooks
+        if "get_ipython" in globals() or "google.colab" in sys.modules:
+            import nest_asyncio
+
+            nest_asyncio.apply()
+        try:
+            loop = asyncio.get_event_loop()
+        except RuntimeError:
+            loop = asyncio.new_event_loop()
+            asyncio.set_event_loop(loop)
+        return loop.run_until_complete(
+            self.aquery(
+                query,
+                k=k,
+                max_sources=max_sources,
+                length_prompt=length_prompt,
+                marginal_relevance=marginal_relevance,
+                answer=answer,
+                key_filter=key_filter
+            )
         )
 
-    def query(
+    async def aquery(
         self,
         query: str,
         k: int = 10,
         max_sources: int = 5,
         length_prompt: str = "about 100 words",
         marginal_relevance: bool = True,
-    ):
-        for answer in self._query(
-            query,
-            k=k,
-            max_sources=max_sources,
-            length_prompt=length_prompt,
-            marginal_relevance=marginal_relevance,
-        ):
-            pass
-        return answer
-
-    def _query(
-        self,
-        query: str,
-        k: int,
-        max_sources: int,
-        length_prompt: str,
-        marginal_relevance: bool,
+        answer: Optional[Answer] = None,
+        key_filter: Optional[bool] = None
     ):
         if k < max_sources:
             raise ValueError("k should be greater than max_sources")
-        tokens = 0
-        answer = Answer(query)
-        with get_openai_callback() as cb:
-            for answer in self.get_evidence(
+        if answer is None:
+            answer = Answer(query)
+        if key_filter or (key_filter is None and len(self.docs) > 5)    :
+            with get_openai_callback() as cb:
+                keys = self.doc_match(answer.question)
+            answer.tokens += cb.total_tokens
+            answer.cost += cb.total_cost
+        if len(answer.contexts) == 0:
+            answer = await self.aget_evidence(
                 answer,
                 k=k,
                 max_sources=max_sources,
                 marginal_relevance=marginal_relevance,
-            ):
-                yield answer
-            tokens += cb.total_tokens
+                key_filter=keys if key_filter else None
+            )
         context_str, citations = answer.context, answer.contexts
         bib = dict()
         passages = dict()
         if len(context_str) < 10:
             answer_text = (
                 "I cannot answer this question due to insufficient information."
             )
         else:
             with get_openai_callback() as cb:
-                answer_text = self.qa_chain.run(
+                answer_text = await self.qa_chain.arun(
                     question=query, context_str=context_str, length=length_prompt
                 )
-                tokens += cb.total_tokens
+            answer.tokens += cb.total_tokens
+            answer.cost += cb.total_cost
         # it still happens lol
         if "(Foo2012)" in answer_text:
             answer_text = answer_text.replace("(Foo2012)", "")
         for key, citation, summary, text in citations:
             # do check for whole key (so we don't catch Callahan2019a with Callahan2019)
             skey = key.split(" ")[0]
             if skey + " " in answer_text or skey + ")" or skey + "," in answer_text:
@@ -368,14 +454,13 @@
                 passages[key] = text
         bib_str = "\n\n".join(
             [f"{i+1}. ({k}): {c}" for i, (k, c) in enumerate(bib.items())]
         )
         formatted_answer = f"Question: {query}\n\n{answer_text}\n"
         if len(bib) > 0:
             formatted_answer += f"\nReferences\n\n{bib_str}\n"
-        formatted_answer += f"\nTokens Used: {tokens} Cost: ${tokens/1000 * 0.002:.2f}"
+        formatted_answer += f"\nTokens Used: {answer.tokens} Cost: ${answer.cost:.2f}"
         answer.answer = answer_text
         answer.formatted_answer = formatted_answer
         answer.references = bib_str
         answer.passages = passages
-        answer.tokens = tokens
-        yield answer
+        return answer
```

### Comparing `paper-qa-0.1.0/paperqa/qaprompts.py` & `paper-qa-1.0.0/paperqa/qaprompts.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,32 +9,32 @@
 summary_prompt = prompts.PromptTemplate(
     input_variables=["question", "context_str", "citation"],
     template="Summarize and provide direct quotes from the text below to help answer a question. "
     "Do not directly answer the question, instead summarize and "
     "quote to give evidence to help answer the question. "
     "Do not use outside sources. "
     'Reply with "Not applicable" if the text is unrelated to the question. '
-    "Use 75 or less words."
+    "Use 150 or less words."
     "\n\n"
     "{context_str}\n"
     "Extracted from {citation}\n"
     "Question: {question}\n"
     "Relevant Information Summary:",
 )
 
 
 qa_prompt = prompts.PromptTemplate(
     input_variables=["question", "context_str", "length"],
     template="Write an answer ({length}) "
-    "for the question below solely based on the provided context. "
+    "for the question below based on the provided context. "
     "If the context provides insufficient information, "
     'reply "I cannot answer". '
     "For each sentence in your answer, indicate which sources most support it "
     "via valid citation markers at the end of sentences, like (Example2012). "
-    "Answer in an unbiased and scholarly tone. Make clear what is your opinion. "
+    "Answer in an unbiased, comprehensive, and scholarly tone. "
     "Use Markdown for formatting code or text, and try to use direct quotes to support arguments.\n\n"
     "{context_str}\n"
     "Question: {question}\n"
     "Answer: ",
 )
 
 
@@ -44,14 +44,26 @@
     "Provide three keyword searches (one search per line) "
     "that will find papers to help answer the question. Do not use boolean operators. "
     "Recent years are 2021, 2022, 2023.\n\n"
     "1.",
 )
 
 
+select_paper_prompt = prompts.PromptTemplate(
+    input_variables=["instructions", "papers"],
+    template="Select papers according to instructions below. "
+    "Papers are listed as $KEY: $PAPER_INFO. "
+    "Return a list of keys, separated by commas. "
+    'Return "None", if no papers are applicable. \n\n'
+    "Instructions: {instructions}\n\n"
+    "{papers}\n\n"
+    "Selected keys:",
+)
+
+
 def _get_datetime():
     now = datetime.now()
     return now.strftime("%m/%d/%Y")
 
 
 citation_prompt = prompts.PromptTemplate(
     input_variables=["text"],
```

### Comparing `paper-qa-0.1.0/paperqa/utils.py` & `paper-qa-1.0.0/paperqa/utils.py`

 * *Files identical despite different names*

### Comparing `paper-qa-0.1.0/setup.py` & `paper-qa-1.0.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,23 +9,24 @@
     name="paper-qa",
     version=__version__,
     description="LLM Chain for answering questions from docs ",
     author="Andrew White",
     author_email="white.d.andrew@gmail.com",
     url="https://github.com/whitead/paper-qa",
     license="MIT",
-    packages=["paperqa"],
+    packages=["paperqa", "paperqa.contrib"],
     install_requires=[
         "pypdf",
-        "langchain>=0.0.98",
+        "langchain>=0.0.129",
         "openai>=0.27.0",
         "faiss-cpu",
         "PyCryptodome",
         "html2text",
         "tiktoken",
+        "pyzotero",
     ],
     test_suite="tests",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

### Comparing `paper-qa-0.1.0/tests/test_paperqa.py` & `paper-qa-1.0.0/tests/test_paperqa.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import paperqa
 import requests
 import os
 import pickle
 from paperqa.utils import strings_similarity
 from langchain.llms import OpenAI
+from unittest import IsolatedAsyncioTestCase
 
 
 def test_maybe_is_text():
     assert paperqa.maybe_is_text(
         "This is a test. The sample conc. was 1.0 mM (at 245 ^F)"
     )
     assert not paperqa.maybe_is_text("\\C0\\C0\\B1\x00")
@@ -37,18 +38,17 @@
     doc_path = "example.txt"
     with open(doc_path, "w", encoding="utf-8") as f:
         # get wiki page about politician
         r = requests.get("https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
         f.write(r.text)
     docs = paperqa.Docs()
     docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now")
-    for evidence in docs.get_evidence(
+    evidence = docs.get_evidence(
         paperqa.Answer("For which state was he a governor"), k=1, max_sources=1
-    ):
-        pass
+    )
     assert "Missouri" in evidence.context
     os.remove(doc_path)
 
 
 def test_query():
     doc_path = "example.txt"
     with open(doc_path, "w", encoding="utf-8") as f:
@@ -57,26 +57,40 @@
         f.write(r.text)
     docs = paperqa.Docs()
     docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now")
     answer = docs.query("What is Frederick Bates's greatest accomplishment?")
     os.remove(doc_path)
 
 
-def test_query_gen():
+class Test(IsolatedAsyncioTestCase):
+    async def test_aquery(self):
+        doc_path = "example.txt"
+        with open(doc_path, "w", encoding="utf-8") as f:
+            # get wiki page about politician
+            r = requests.get(
+                "https://en.wikipedia.org/wiki/Frederick_Bates_(politician)"
+            )
+            f.write(r.text)
+        docs = paperqa.Docs()
+        docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now")
+        i = 0
+        answer = await docs.aquery("What is Frederick Bates's greatest accomplishment?")
+        os.remove(doc_path)
+
+
+def test_doc_match():
     doc_path = "example.txt"
     with open(doc_path, "w", encoding="utf-8") as f:
         # get wiki page about politician
         r = requests.get("https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
         f.write(r.text)
     docs = paperqa.Docs()
     docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now")
     i = 0
-    for answer in docs.query_gen("What is Frederick Bates's greatest accomplishment?"):
-        i += 1
-    assert i >= 2
+    result = docs.doc_match("What is Frederick Bates's greatest accomplishment?")
     os.remove(doc_path)
 
 
 def test_docs_pickle():
     doc_path = "example.txt"
     with open(doc_path, "w", encoding="utf-8") as f:
         # get front page of wikipedia
@@ -87,28 +101,24 @@
     docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now", chunk_chars=1000)
     docs_pickle = pickle.dumps(docs)
     docs2 = pickle.loads(docs_pickle)
     docs2.update_llm(llm)
     assert len(docs.docs) == len(docs2.docs)
     assert (
         strings_similarity(
-            list(
-                docs.get_evidence(
-                    paperqa.Answer("What date is flag day in Canada?"),
-                    k=3,
-                    max_sources=1,
-                )
-            )[-1].context,
-            list(
-                docs2.get_evidence(
-                    paperqa.Answer("What date is flag day in Canada?"),
-                    k=3,
-                    max_sources=1,
-                )
-            )[-1].context,
+            docs.get_evidence(
+                paperqa.Answer("What date is flag day in Canada?"),
+                k=3,
+                max_sources=1,
+            ).context,
+            docs2.get_evidence(
+                paperqa.Answer("What date is flag day in Canada?"),
+                k=3,
+                max_sources=1,
+            ).context,
         )
         > 0.75
     )
     os.remove(doc_path)
 
 
 def test_bad_context():
@@ -119,15 +129,14 @@
         f.write(r.text)
     docs = paperqa.Docs()
     docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now")
     answer = docs.query(
         "What year was Barack Obama born?",
         length_prompt="about 20 words",
     )
-    print(answer.context)
     assert "cannot answer" in answer.answer
     os.remove(doc_path)
 
 
 def test_repeat_keys():
     doc_path = "example.txt"
     with open(doc_path, "w", encoding="utf-8") as f:
@@ -182,15 +191,15 @@
     doc_path = "example.txt"
     with open(doc_path, "w", encoding="utf-8") as f:
         # get wiki page about politician
         r = requests.get("https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
         f.write(r.text)
     docs = paperqa.Docs(llm=OpenAI(temperature=0.0, model_name="text-ada-001"))
     docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now")
-    assert len(docs.doc_previews) == 1
+    assert len(docs.doc_previews()) == 1
 
 
 def test_code():
     # load this script
     doc_path = os.path.abspath(__file__)
     docs = paperqa.Docs(llm=OpenAI(temperature=0.0, model_name="text-ada-001"))
     docs.add(doc_path, "test_paperqa.py", key="test", disable_check=True)
@@ -206,7 +215,38 @@
         f.write(r.text)
     docs = paperqa.Docs()
     docs.add(doc_path)
     assert (
         list(docs.docs.values())[0]["metadata"][0]["key"] == "Wikipedia2023"
         or list(docs.docs.values())[0]["metadata"][0]["key"] == "Frederick2023"
     )
+
+
+def test_dockey_filter():
+    """Test that we can filter evidence with dockeys"""
+    doc_path = "example2.txt"
+    with open(doc_path, "w", encoding="utf-8") as f:
+        # get wiki page about politician
+        r = requests.get("https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
+        f.write(r.text)
+    docs = paperqa.Docs()
+    docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now")
+    # add with new dockey
+    docs.add("example.txt", "WikiMedia Foundation, 2023, Accessed now", key="test")
+    answer = paperqa.Answer("What country is Bates from?")
+    docs.get_evidence(answer, key_filter=["test"])
+
+
+def test_query_filter():
+    """Test that we can filter evidence with in query"""
+    doc_path = "example2.txt"
+    with open(doc_path, "w", encoding="utf-8") as f:
+        # get wiki page about politician
+        r = requests.get("https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
+        f.write(r.text)
+    docs = paperqa.Docs()
+    docs.add(doc_path, "Information about Fredrick Bates, WikiMedia Foundation, 2023, Accessed now")
+    # add with new dockey
+    docs.add("example.txt", "WikiMedia Foundation, 2023, Accessed now", key="test")
+    answer = docs.query("What country is Bates from?", key_filter=True)
+    print(answer.context)
+    assert "United States" in answer.answer
```

