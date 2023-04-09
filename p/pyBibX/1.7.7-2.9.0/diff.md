# Comparing `tmp/pyBibX-1.7.7.tar.gz` & `tmp/pyBibX-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyBibX-1.7.7.tar", last modified: Fri Apr  7 15:41:21 2023, max compression
+gzip compressed data, was "dist\pyBibX-2.9.0.tar", last modified: Sun Apr  9 14:52:46 2023, max compression
```

## Comparing `pyBibX-1.7.7.tar` & `pyBibX-2.9.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-04-07 15:41:21.000000 pyBibX-1.7.7/
--rw-rw-rw-   0        0        0      644 2022-03-01 19:24:07.000000 pyBibX-1.7.7/LICENSE
--rw-rw-rw-   0        0        0       40 2022-05-19 14:46:22.000000 pyBibX-1.7.7/MANIFEST.in
--rw-rw-rw-   0        0        0     8357 2023-04-07 15:41:21.000000 pyBibX-1.7.7/PKG-INFO
--rw-rw-rw-   0        0        0     7926 2023-04-07 15:24:42.000000 pyBibX-1.7.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-07 15:41:21.000000 pyBibX-1.7.7/pyBibX/
--rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyBibX-1.7.7/pyBibX/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-07 15:41:21.000000 pyBibX-1.7.7/pyBibX/base/
--rw-rw-rw-   0        0        0       27 2022-03-16 15:26:25.000000 pyBibX-1.7.7/pyBibX/base/__init__.py
--rw-rw-rw-   0        0        0   240753 2023-04-07 15:39:45.000000 pyBibX-1.7.7/pyBibX/base/pbx.py
-drwxrwxrwx   0        0        0        0 2023-04-07 15:41:21.000000 pyBibX-1.7.7/pyBibX/base/stws/
--rw-rw-rw-   0        0        0     1287 2017-07-30 20:46:06.000000 pyBibX-1.7.7/pyBibX/base/stws/Stopwords-Arabic.txt
--rw-rw-rw-   0        0        0     1484 2017-07-30 20:46:06.000000 pyBibX-1.7.7/pyBibX/base/stws/Stopwords-Bengali.txt
--rw-rw-rw-   0        0        0     2408 2017-07-30 20:46:06.000000 pyBibX-1.7.7/pyBibX/base/stws/Stopwords-Bulgarian.txt
--rw-rw-rw-   0        0        0     1518 2017-07-30 20:46:06.000000 pyBibX-1.7.7/pyBibX/base/stws/Stopwords-Czech.txt
--rw-rw-rw-   0        0        0     4212 2017-08-01 12:33:33.000000 pyBibX-1.7.7/pyBibX/base/stws/Stopwords-English.txt
--rw-rw-rw-   0        0        0     6219 2017-07-30 20:46:06.000000 pyBibX-1.7.7/pyBibX/base/stws/Stopwords-Finnish.txt
--rw-rw-rw-   0        0        0     3234 2017-07-30 20:46:06.000000 pyBibX-1.7.7/pyBibX/base/stws/Stopwords-French.txt
--rw-rw-rw-   0        0        0     4350 2017-07-30 20:46:06.000000 pyBibX-1.7.7/pyBibX/base/stws/Stopwords-German.txt
--rw-rw-rw-   0        0        0     2065 2017-07-30 20:46:06.000000 pyBibX-1.7.7/pyBibX/base/stws/Stopwords-Hindi.txt
--rw-rw-rw-   0        0        0     5552 2017-07-30 20:46:06.000000 pyBibX-1.7.7/pyBibX/base/stws/Stopwords-Hungarian.txt
--rw-rw-rw-   0        0        0     2379 2017-07-30 20:46:06.000000 pyBibX-1.7.7/pyBibX/base/stws/Stopwords-Italian.txt
--rw-rw-rw-   0        0        0     1307 2017-07-30 20:46:06.000000 pyBibX-1.7.7/pyBibX/base/stws/Stopwords-Marathi.txt
--rw-rw-rw-   0        0        0     3274 2017-07-30 20:46:06.000000 pyBibX-1.7.7/pyBibX/base/stws/Stopwords-Persian.txt
--rw-rw-rw-   0        0        0      704 2017-07-30 20:46:06.000000 pyBibX-1.7.7/pyBibX/base/stws/Stopwords-Polish.txt
--rw-rw-rw-   0        0        0     3772 2019-05-09 13:59:54.000000 pyBibX-1.7.7/pyBibX/base/stws/Stopwords-Portuguese-br.txt
--rw-rw-rw-   0        0        0     1926 2017-07-30 20:46:06.000000 pyBibX-1.7.7/pyBibX/base/stws/Stopwords-Romanian.txt
--rw-rw-rw-   0        0        0     4963 2017-07-30 20:46:06.000000 pyBibX-1.7.7/pyBibX/base/stws/Stopwords-Russian.txt
--rw-rw-rw-   0        0        0     2420 2017-08-01 12:33:16.000000 pyBibX-1.7.7/pyBibX/base/stws/Stopwords-Spanish.txt
--rw-rw-rw-   0        0        0     2757 2017-07-30 20:46:06.000000 pyBibX-1.7.7/pyBibX/base/stws/Stopwords-Swedish.txt
--rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyBibX-1.7.7/pyBibX/base/stws/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-07 15:41:21.000000 pyBibX-1.7.7/pyBibX.egg-info/
--rw-rw-rw-   0        0        0     8357 2023-04-07 15:41:20.000000 pyBibX-1.7.7/pyBibX.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1047 2023-04-07 15:41:21.000000 pyBibX-1.7.7/pyBibX.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-07 15:41:20.000000 pyBibX-1.7.7/pyBibX.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      205 2023-04-07 15:41:20.000000 pyBibX-1.7.7/pyBibX.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-07 15:41:20.000000 pyBibX-1.7.7/pyBibX.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-04-07 15:41:20.000000 pyBibX-1.7.7/pyBibX.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2023-04-07 15:41:21.000000 pyBibX-1.7.7/setup.cfg
--rw-rw-rw-   0        0        0     1077 2023-04-07 15:41:11.000000 pyBibX-1.7.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 14:52:46.000000 pyBibX-2.9.0/
+-rw-rw-rw-   0        0        0      644 2022-03-01 19:24:07.000000 pyBibX-2.9.0/LICENSE
+-rw-rw-rw-   0        0        0       40 2022-05-19 14:46:22.000000 pyBibX-2.9.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     9092 2023-04-09 14:52:46.000000 pyBibX-2.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0     8655 2023-04-09 13:31:30.000000 pyBibX-2.9.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-09 14:52:45.000000 pyBibX-2.9.0/pyBibX/
+-rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyBibX-2.9.0/pyBibX/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-09 14:52:45.000000 pyBibX-2.9.0/pyBibX/base/
+-rw-rw-rw-   0        0        0       27 2022-03-16 15:26:25.000000 pyBibX-2.9.0/pyBibX/base/__init__.py
+-rw-rw-rw-   0        0        0   261990 2023-04-09 13:26:45.000000 pyBibX-2.9.0/pyBibX/base/pbx.py
+drwxrwxrwx   0        0        0        0 2023-04-09 14:52:46.000000 pyBibX-2.9.0/pyBibX/base/stws/
+-rw-rw-rw-   0        0        0     1287 2017-07-30 20:46:06.000000 pyBibX-2.9.0/pyBibX/base/stws/Stopwords-Arabic.txt
+-rw-rw-rw-   0        0        0     1484 2017-07-30 20:46:06.000000 pyBibX-2.9.0/pyBibX/base/stws/Stopwords-Bengali.txt
+-rw-rw-rw-   0        0        0     2408 2017-07-30 20:46:06.000000 pyBibX-2.9.0/pyBibX/base/stws/Stopwords-Bulgarian.txt
+-rw-rw-rw-   0        0        0     1518 2017-07-30 20:46:06.000000 pyBibX-2.9.0/pyBibX/base/stws/Stopwords-Czech.txt
+-rw-rw-rw-   0        0        0     4212 2017-08-01 12:33:33.000000 pyBibX-2.9.0/pyBibX/base/stws/Stopwords-English.txt
+-rw-rw-rw-   0        0        0     6219 2017-07-30 20:46:06.000000 pyBibX-2.9.0/pyBibX/base/stws/Stopwords-Finnish.txt
+-rw-rw-rw-   0        0        0     3234 2017-07-30 20:46:06.000000 pyBibX-2.9.0/pyBibX/base/stws/Stopwords-French.txt
+-rw-rw-rw-   0        0        0     4350 2017-07-30 20:46:06.000000 pyBibX-2.9.0/pyBibX/base/stws/Stopwords-German.txt
+-rw-rw-rw-   0        0        0     2065 2017-07-30 20:46:06.000000 pyBibX-2.9.0/pyBibX/base/stws/Stopwords-Hindi.txt
+-rw-rw-rw-   0        0        0     5552 2017-07-30 20:46:06.000000 pyBibX-2.9.0/pyBibX/base/stws/Stopwords-Hungarian.txt
+-rw-rw-rw-   0        0        0     2379 2017-07-30 20:46:06.000000 pyBibX-2.9.0/pyBibX/base/stws/Stopwords-Italian.txt
+-rw-rw-rw-   0        0        0     1307 2017-07-30 20:46:06.000000 pyBibX-2.9.0/pyBibX/base/stws/Stopwords-Marathi.txt
+-rw-rw-rw-   0        0        0     3274 2017-07-30 20:46:06.000000 pyBibX-2.9.0/pyBibX/base/stws/Stopwords-Persian.txt
+-rw-rw-rw-   0        0        0      704 2017-07-30 20:46:06.000000 pyBibX-2.9.0/pyBibX/base/stws/Stopwords-Polish.txt
+-rw-rw-rw-   0        0        0     3772 2019-05-09 13:59:54.000000 pyBibX-2.9.0/pyBibX/base/stws/Stopwords-Portuguese-br.txt
+-rw-rw-rw-   0        0        0     1926 2017-07-30 20:46:06.000000 pyBibX-2.9.0/pyBibX/base/stws/Stopwords-Romanian.txt
+-rw-rw-rw-   0        0        0     4963 2017-07-30 20:46:06.000000 pyBibX-2.9.0/pyBibX/base/stws/Stopwords-Russian.txt
+-rw-rw-rw-   0        0        0     2420 2017-08-01 12:33:16.000000 pyBibX-2.9.0/pyBibX/base/stws/Stopwords-Spanish.txt
+-rw-rw-rw-   0        0        0     2757 2017-07-30 20:46:06.000000 pyBibX-2.9.0/pyBibX/base/stws/Stopwords-Swedish.txt
+-rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyBibX-2.9.0/pyBibX/base/stws/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-09 14:52:45.000000 pyBibX-2.9.0/pyBibX.egg-info/
+-rw-rw-rw-   0        0        0     9092 2023-04-09 14:52:42.000000 pyBibX-2.9.0/pyBibX.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1047 2023-04-09 14:52:43.000000 pyBibX-2.9.0/pyBibX.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 14:52:42.000000 pyBibX-2.9.0/pyBibX.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      205 2023-04-09 14:52:42.000000 pyBibX-2.9.0/pyBibX.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-09 14:52:42.000000 pyBibX-2.9.0/pyBibX.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-04-09 14:52:42.000000 pyBibX-2.9.0/pyBibX.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2023-04-09 14:52:46.000000 pyBibX-2.9.0/setup.cfg
+-rw-rw-rw-   0        0        0     1077 2023-04-08 01:55:27.000000 pyBibX-2.9.0/setup.py
```

### Comparing `pyBibX-1.7.7/LICENSE` & `pyBibX-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyBibX-1.7.7/PKG-INFO` & `pyBibX-2.9.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,103 +1,98 @@
-Metadata-Version: 2.1
-Name: pyBibX
-Version: 1.7.7
-Summary: A Bibliometric and Scientometric Library Powered with Artificial Intelligence Tools
-Home-page: https://github.com/Valdecy/pyBibX
-Author: Valdecy Pereira
-Author-email: valdecy.pereira@gmail.com
-License: GNU
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# pyBibX
-
-## Introduction
-
-A Bibliometric and Scientometric python library that uses the raw files generated by **Scopus** (.bib files), **WOS (Web of Science)** (.bib files) and **PubMed** (.txt files) scientific databases. Also Powered with Artificial Intelligence Tools to Analyze Text Data
-
-General Capabilities:
-- a) Works with **Scopus** (.bib files), **WOS** (.bib files) and **PubMed** (.txt files) databases 
-- b) Identification and Removal of duplicates
-- c) Identification of documents per type
-- d) Generates an **EDA (Exploratory Data Analysis)** Report: Publications Timespan, Total Number of Countries, Total Number of Institutions, Total Number of Sources, Total Number of References, Total Number of Languages (and also the number of docs for each language), Total Number of Documents, Average Documents per Author, Average Documents per Institution, Average Documents per Source, Average Documents per Year, Total Number of Authors, Total Number of Authors Keywords, Total Number of Authors Keywords Plus, Total Single-Authored Documents, Total Multi-Authored Documents, Average Collaboration Index, Max H-Index, Total Number of Citations, Average Citations per Author, Average Citations per Institution, Average Citations per Document, Average Citations per Source
-- e) Creates an **ID (Identification)** for each Document, Authors, Sources, Institutions, Countries, Authors' Keywords, Keywords Plus. The IDs can be used in graphs/plots to obtain a cleaner visualization
-- f) Creates a **WordCloud** from the Abstracts, Titles, Authors Keywords or Keywords Plus
-- g) Creates a **N-Gram Bar Plot (interactive plot)** from the Abstracts, Titles, Authors Keywords or Keywords Plus
-- h) Creates a **Projection (interactive plot)** of the documents based on the Abstracts, Titles, Authors Keywords or Keywords Plus
-- i) Creates an **Evolution Plot (interactive plot)** based on Abstracts, Titles, Sources, Authors Keywords or Keywords Plus
-- j) Creates a **Sankey Plot (interactive plot)** with any combination of the following keys: Authors, Countries, Institutions, Journals, Auhors_Keywords, Keywords_Plus, and/or Languages
-- k) Creates a **TreeMap** from the Authors, Countries, Institutions, Journals, Auhors_Keywords, or Keywords_Plus
-- l) Creates an **Authors Productivity Plot (interactive plot)** It informs for each year the documents (IDs) published for each author
-- m) Creates a **Bar Plot**  for the following statistics: Documents per Year, Citations per Year, Past Citations per Year, Lotka's Law, Sources per Documents, Sources per Citations, Authors per Documents, Authors per Citations, Authors per H-Index, Bradford's Law (Core Sources 1, 2 or 3), Institutions per Documents, Institutions per Citations, Countries per Documents, Countries per Citations, Language per Documents, Keywords Plus per Documents and Authors' Keywords per Documents
-
-Network Capabilities:
-- a) **Citation Analysis (interactive plot)** between Documents (Blue Nodes) and Citations (Red Nodes). Documents and Citations can be highlighted for better visualization
-- b) **Collaboration Analysis (interactive plot)** between Authors, Countries, Institutions or **Adjacency Analysis (interactive plot)** between Authors' Keywords or Keywords Plus. Collaboration and Adjacency can be highlighted for better visualization
-- c) **Similarity Analysis (interactive plot)** can be performed using coupling or cocitation methods
-- d) **World MAP Collaboration Analysis (interactive plot)** between Countries in a Map
-
-Artificial Intelligence Capabilities:
-- a) **Topic Modelling** using BERTopic to cluster documents by topic
-- b) Visualize topics distribution
-- c) Visualize topics by the most representative words
-- d) Visualize documents projection and clusterization by topic
-- e) Visualize topics heatmap
-- f) Find the most representative documents from each topic
-- g) Find the most representative topics according to a word
-- h) Creates **Embeddings** from Abstracts, Titles, Authors Keywords or Keywords Plus
-- i) **Abstractive Text Summarization** using **PEGASUS** on a set of selected documents or all documents
-- j) **Abstractive Text Summarization** using **chatGPT** on a set of selected documents or all documents. Requires the user to have an **API key** (https://platform.openai.com/account/api-keys)
-- k) **Extractive Text Summarization** using **BERT** on a set of selected documents or all documents
-
-Correction and Manipulation Capabilities:
-- a) Filter the .bib or .txt file by Year, Sources, Bradford Law Cores, Countries, Languages and/or Abstracts (Documents with Abstracts)
-- b) Merge Authors, Institutions, Countries, Languages and/or Sources that have multiple entries 
-- c) Merge different or same database files one at a time. The preference of information preservation is given to the old database, so the order of merging matters (see Examples 04 and 05)
-
-## Usage
-
-1. Install
-```bash
-pip install pyBibX
-```
-
-2. Try it in **Colab**:
-
-- Example 01: Scopus                ([ Colab Demo ](https://colab.research.google.com/drive/1yHiMMZIKa-RrarXbPB9ca0gLN9YvvtPU?usp=sharing))
-- Example 02: WOS                   ([ Colab Demo ](https://colab.research.google.com/drive/13HLjC4myTvYcjLk2XBTZKbWJ2aqZUST1?usp=sharing))
-- Example 03: PubMed                ([ Colab Demo ](https://colab.research.google.com/drive/13CU-KvZMnazga1BmQf2J8wYM9mhHL2e1?usp=sharing))
-- Example 04: Scopus + WOS          ([ Colab Demo ](https://colab.research.google.com/drive/1DqEk0_IakJPfIZDVcnTWBE_nxyhW9p-W?usp=sharing))
-- Example 05: WOS + Scopus          ([ Colab Demo ](https://colab.research.google.com/drive/12k_IOcSDwumbEtPqqSMbCIE6ZypgKAJn?usp=sharing))
-- Example 06: Scopus + WOS + Pubmed ([ Colab Demo ](https://colab.research.google.com/drive/1Ko6AibkXtB_Kwg3Eu0fhzNMVEIXPkbez?usp=sharing))
-- Example 07: Your Own              ([ Colab Demo ](https://colab.research.google.com/drive/19EYjgal9V1kemmzpHnyp6MSlk9S-kGHT?usp=sharing))
-
-# Acknowledgement 
-This section indicates the libraries that inspired pyBibX
-
-* BERT (https://smrzr.io/)
-- a) Github: https://github.com/dmmiller612/bert-extractive-summarizer
-- b) Paper: DEREK, M. (2019). Leveraging BERT for Extractive Text Summarization on Lectures. arXiv. doi: https://doi.org/10.48550/arXiv.1906.04165
-
-* BERTopic (https://maartengr.github.io/BERTopic/index.html)
-- a) Github: https://github.com/MaartenGr/BERTopic
-- b) Paper: GROOTENDORST, M. (2022). BERTopic: Neural Topic Modeling with a Class-based TF-IDF Procedure. arXiv. doi: https://doi.org/10.48550/arXiv.2203.05794
-
-* Bibliometrix (https://www.bibliometrix.org/home/)
-- a) Github: https://github.com/massimoaria/bibliometrix
-- b) Paper: ARIA, M.; CUCCURULLO, C. (2017). Bibliometrix: An R-tool for Comprehensive Science Mapping Analysis. Journal of informetrics, 11(4), 959-975. doi: https://doi.org/10.1016/j.joi.2017.08.007
-
-* Metaknowledge (http://www.networkslab.org/metaknowledge)
-- a) Github: https://github.com/UWNETLAB/metaknowledge
-- b) Paper: McILROY-YOUNG, R.; McLEVEY, J.; ANDERSON, J. (2015). Metaknowledge: Open Source Software for Social Networks, Bibliometrics, and Sociology of Knowledge Research.
-
-* SentenceTransformers (https://www.sbert.net/)
-- a) Github: https://github.com/UKPLab/sentence-transformers
-- b) Paper: REIMERS, N.; GUREVYCH, I. (2019). Sentence-BERT: Sentence Embeddings using Siamese BERT-Networks. arXiv. doi: https://arxiv.org/abs/1908.10084
-
-* PEGASUS (https://ai.googleblog.com/2020/06/pegasus-state-of-art-model-for.html?m=1)
-- a) Github: https://github.com/huggingface/transformers
-- b) Paper: ZHANG, J.; ZHAO, Y.; SALEH, M.; LIU, P.J. (2019). PEGASUS: Pre-training with Extracted Gap-sentences for Abstractive Summarization. arXiv. doi: https://doi.org/10.48550/arXiv.1912.08777
-
-And to all the people that helped to improve or correct the code. Thank you very much!
-
-* Fabio Ribeiro von Glehn (29.DECEMBER.2022) - UFG - Federal University of Goias (Brazil)
+# pyBibX
+
+## Introduction
+
+A Bibliometric and Scientometric python library that uses the raw files generated by **Scopus** (.bib files), **WOS (Web of Science)** (.bib files), and **PubMed** (.txt files) scientific databases. Also Powered with Artificial Intelligence Tools to Analyze Bibliometric Results and Text Data
+
+General Capabilities:
+- a) Works with **Scopus** (.bib files), **WOS** (.bib files) and **PubMed** (.txt files) databases 
+- b) Identification and Removal of duplicates
+- c) Identification of documents per type
+- d) Generates an **EDA (Exploratory Data Analysis)** Report: Publications Timespan, Total Number of Countries, Total Number of Institutions, Total Number of Sources, Total Number of References, Total Number of Languages (and also the number of docs for each language), Total Number of Documents, Average Documents per Author, Average Documents per Institution, Average Documents per Source, Average Documents per Year, Total Number of Authors, Total Number of Authors Keywords, Total Number of Authors Keywords Plus, Total Single-Authored Documents, Total Multi-Authored Documents, Average Collaboration Index, Max H-Index, Total Number of Citations, Average Citations per Author, Average Citations per Institution, Average Citations per Document, Average Citations per Source
+- e) Creates an **ID (Identification)** for each Document, Authors, Sources, Institutions, Countries, Authors' Keywords, Keywords Plus. The IDs can be used in graphs/plots to obtain a cleaner visualization
+- f) Creates a **WordCloud** from the Abstracts, Titles, Authors Keywords or Keywords Plus
+- g) Creates a **N-Gram Bar Plot (interactive plot)** from the Abstracts, Titles, Authors Keywords or Keywords Plus
+- h) Creates a **Projection (interactive plot)** of the documents based on the Abstracts, Titles, Authors Keywords or Keywords Plus
+- i) Creates an **Evolution Plot (interactive plot)** based on Abstracts, Titles, Sources, Authors Keywords or Keywords Plus
+- j) Creates a **Sankey Diagram (interactive plot)** with any combination of the following keys: Authors, Countries, Institutions, Journals, Auhors_Keywords, Keywords_Plus, and/or Languages
+- k) Creates a **TreeMap** from the Authors, Countries, Institutions, Journals, Auhors_Keywords, or Keywords_Plus
+- l) Creates an **Authors Productivity Plot (interactive plot)** It informs for each year the documents (IDs) published for each author
+- m) Creates a **Bar Plot**  for the following statistics: Documents per Year, Citations per Year, Past Citations per Year, Lotka's Law, Sources per Documents, Sources per Citations, Authors per Documents, Authors per Citations, Authors per H-Index, Bradford's Law (Core Sources 1, 2 or 3), Institutions per Documents, Institutions per Citations, Countries per Documents, Countries per Citations, Language per Documents, Keywords Plus per Documents and Authors' Keywords per Documents
+
+Network Capabilities:
+- a) **Citation Analysis (interactive plot)** between Documents (Blue Nodes) and Citations (Red Nodes). Documents and Citations can be highlighted for better visualization
+- b) **Collaboration Analysis (interactive plot)** between Authors, Countries, Institutions or **Adjacency Analysis (interactive plot)** between Authors' Keywords or Keywords Plus. Collaboration and Adjacency can be highlighted for better visualization
+- c) **Similarity Analysis (interactive plot)** can be performed using coupling or cocitation methods
+- d) **World Map Collaboration Analysis (interactive plot)** between Countries in a Map
+
+Artificial Intelligence Capabilities:
+- a) **Topic Modelling** using BERTopic to cluster documents by topic
+- b) Visualize topics distribution
+- c) Visualize topics by the most representative words
+- d) Visualize documents projection and clusterization by topic
+- e) Visualize topics heatmap
+- f) Find the most representative documents from each topic
+- g) Find the most representative topics according to a word
+- h) Creates **Embeddings** from Abstracts, Titles, Authors Keywords or Keywords Plus
+- i) **Abstractive Text Summarization** using **PEGASUS** on a set of selected documents or all documents
+- j) **Abstractive Text Summarization** using **chatGPT** on a set of selected documents or all documents. Requires the user to have an **API key** (https://platform.openai.com/account/api-keys)
+- k) **Extractive Text Summarization** using **BERT** on a set of selected documents or all documents
+- l) **Ask chatGPT to Analyze Results** available for: EDA Report, WordCloud, N-Grams, Evolution Plot, Sankey Diagram, Authors Productivity Plot, Bar Plots, Citation Analysis, Collaboration Analysis, Similarity Analysis, and World Map Collaboration Analysis (see Example 08). Requires the user to have an **API key** (https://platform.openai.com/account/api-keys)
+
+Correction and Manipulation Capabilities:
+- a) Filter the .bib or .txt file by Year, Sources, Bradford Law Cores, Countries, Languages and/or Abstracts (Documents with Abstracts)
+- b) Merge Authors, Institutions, Countries, Languages and/or Sources that have multiple entries 
+- c) Merge different or the same database files one at a time. The preference for information preservation is given to the old database, so the order of merging matters (see Examples 04 and 05)
+
+## Usage
+
+1. Install
+```bash
+pip install pyBibX
+```
+
+2. Try it in **Colab**:
+
+- Example 01: Scopus                ([ Colab Demo ](https://colab.research.google.com/drive/1yHiMMZIKa-RrarXbPB9ca0gLN9YvvtPU?usp=sharing))
+- Example 02: WOS                   ([ Colab Demo ](https://colab.research.google.com/drive/13HLjC4myTvYcjLk2XBTZKbWJ2aqZUST1?usp=sharing))
+- Example 03: PubMed                ([ Colab Demo ](https://colab.research.google.com/drive/13CU-KvZMnazga1BmQf2J8wYM9mhHL2e1?usp=sharing))
+- Example 04: Scopus + WOS          ([ Colab Demo ](https://colab.research.google.com/drive/1DqEk0_IakJPfIZDVcnTWBE_nxyhW9p-W?usp=sharing))
+- Example 05: WOS + Scopus          ([ Colab Demo ](https://colab.research.google.com/drive/12k_IOcSDwumbEtPqqSMbCIE6ZypgKAJn?usp=sharing))
+- Example 06: Scopus + WOS + Pubmed ([ Colab Demo ](https://colab.research.google.com/drive/1Ko6AibkXtB_Kwg3Eu0fhzNMVEIXPkbez?usp=sharing))
+- Example 07: Your Own              ([ Colab Demo ](https://colab.research.google.com/drive/19EYjgal9V1kemmzpHnyp6MSlk9S-kGHT?usp=sharing))
+- Example 08: Ask chatGPT Analysis  ([ Colab Demo ](https://colab.research.google.com/drive/1LMrR49F54MuX-stlrQbrrjX_dEU3kZ8Y?usp=sharing))
+
+# Acknowledgement 
+This section indicates the libraries that inspired pyBibX
+
+* BERT (https://smrzr.io/)
+- a) Github: https://github.com/dmmiller612/bert-extractive-summarizer
+- b) Paper: DEREK, M. (2019). Leveraging BERT for Extractive Text Summarization on Lectures. arXiv. doi: https://doi.org/10.48550/arXiv.1906.04165
+
+* BERTopic (https://maartengr.github.io/BERTopic/index.html)
+- a) Github: https://github.com/MaartenGr/BERTopic
+- b) Paper: GROOTENDORST, M. (2022). BERTopic: Neural Topic Modeling with a Class-based TF-IDF Procedure. arXiv. doi: https://doi.org/10.48550/arXiv.2203.05794
+
+* Bibliometrix (https://www.bibliometrix.org/home/)
+- a) Github: https://github.com/massimoaria/bibliometrix
+- b) Paper: ARIA, M.; CUCCURULLO, C. (2017). Bibliometrix: An R-tool for Comprehensive Science Mapping Analysis. Journal of informetrics, 11(4), 959-975. doi: https://doi.org/10.1016/j.joi.2017.08.007
+
+* chatGPT (https://chat.openai.com/chat)
+- a) Github: https://github.com/openai
+- b) Paper: ECOFFET, A. (2023). GPT-4 Technical Report. arXiv. doi: https://doi.org/10.48550/arXiv.2303.08774
+
+* Metaknowledge (http://www.networkslab.org/metaknowledge)
+- a) Github: https://github.com/UWNETLAB/metaknowledge
+- b) Paper: McILROY-YOUNG, R.; McLEVEY, J.; ANDERSON, J. (2015). Metaknowledge: Open Source Software for Social Networks, Bibliometrics, and Sociology of Knowledge Research.
+
+* SentenceTransformers (https://www.sbert.net/)
+- a) Github: https://github.com/UKPLab/sentence-transformers
+- b) Paper: REIMERS, N.; GUREVYCH, I. (2019). Sentence-BERT: Sentence Embeddings using Siamese BERT-Networks. arXiv. doi: https://arxiv.org/abs/1908.10084
+
+* PEGASUS (https://ai.googleblog.com/2020/06/pegasus-state-of-art-model-for.html?m=1)
+- a) Github: https://github.com/huggingface/transformers
+- b) Paper: ZHANG, J.; ZHAO, Y.; SALEH, M.; LIU, P.J. (2019). PEGASUS: Pre-training with Extracted Gap-sentences for Abstractive Summarization. arXiv. doi: https://doi.org/10.48550/arXiv.1912.08777
+
+And to all the people that helped to improve or correct the code. Thank you very much!
+
+* Fabio Ribeiro von Glehn (29.DECEMBER.2022) - UFG - Federal University of Goias (Brazil)
```

### Comparing `pyBibX-1.7.7/README.md` & `pyBibX-2.9.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,92 +1,109 @@
-# pyBibX
-
-## Introduction
-
-A Bibliometric and Scientometric python library that uses the raw files generated by **Scopus** (.bib files), **WOS (Web of Science)** (.bib files) and **PubMed** (.txt files) scientific databases. Also Powered with Artificial Intelligence Tools to Analyze Text Data
-
-General Capabilities:
-- a) Works with **Scopus** (.bib files), **WOS** (.bib files) and **PubMed** (.txt files) databases 
-- b) Identification and Removal of duplicates
-- c) Identification of documents per type
-- d) Generates an **EDA (Exploratory Data Analysis)** Report: Publications Timespan, Total Number of Countries, Total Number of Institutions, Total Number of Sources, Total Number of References, Total Number of Languages (and also the number of docs for each language), Total Number of Documents, Average Documents per Author, Average Documents per Institution, Average Documents per Source, Average Documents per Year, Total Number of Authors, Total Number of Authors Keywords, Total Number of Authors Keywords Plus, Total Single-Authored Documents, Total Multi-Authored Documents, Average Collaboration Index, Max H-Index, Total Number of Citations, Average Citations per Author, Average Citations per Institution, Average Citations per Document, Average Citations per Source
-- e) Creates an **ID (Identification)** for each Document, Authors, Sources, Institutions, Countries, Authors' Keywords, Keywords Plus. The IDs can be used in graphs/plots to obtain a cleaner visualization
-- f) Creates a **WordCloud** from the Abstracts, Titles, Authors Keywords or Keywords Plus
-- g) Creates a **N-Gram Bar Plot (interactive plot)** from the Abstracts, Titles, Authors Keywords or Keywords Plus
-- h) Creates a **Projection (interactive plot)** of the documents based on the Abstracts, Titles, Authors Keywords or Keywords Plus
-- i) Creates an **Evolution Plot (interactive plot)** based on Abstracts, Titles, Sources, Authors Keywords or Keywords Plus
-- j) Creates a **Sankey Plot (interactive plot)** with any combination of the following keys: Authors, Countries, Institutions, Journals, Auhors_Keywords, Keywords_Plus, and/or Languages
-- k) Creates a **TreeMap** from the Authors, Countries, Institutions, Journals, Auhors_Keywords, or Keywords_Plus
-- l) Creates an **Authors Productivity Plot (interactive plot)** It informs for each year the documents (IDs) published for each author
-- m) Creates a **Bar Plot**  for the following statistics: Documents per Year, Citations per Year, Past Citations per Year, Lotka's Law, Sources per Documents, Sources per Citations, Authors per Documents, Authors per Citations, Authors per H-Index, Bradford's Law (Core Sources 1, 2 or 3), Institutions per Documents, Institutions per Citations, Countries per Documents, Countries per Citations, Language per Documents, Keywords Plus per Documents and Authors' Keywords per Documents
-
-Network Capabilities:
-- a) **Citation Analysis (interactive plot)** between Documents (Blue Nodes) and Citations (Red Nodes). Documents and Citations can be highlighted for better visualization
-- b) **Collaboration Analysis (interactive plot)** between Authors, Countries, Institutions or **Adjacency Analysis (interactive plot)** between Authors' Keywords or Keywords Plus. Collaboration and Adjacency can be highlighted for better visualization
-- c) **Similarity Analysis (interactive plot)** can be performed using coupling or cocitation methods
-- d) **World MAP Collaboration Analysis (interactive plot)** between Countries in a Map
-
-Artificial Intelligence Capabilities:
-- a) **Topic Modelling** using BERTopic to cluster documents by topic
-- b) Visualize topics distribution
-- c) Visualize topics by the most representative words
-- d) Visualize documents projection and clusterization by topic
-- e) Visualize topics heatmap
-- f) Find the most representative documents from each topic
-- g) Find the most representative topics according to a word
-- h) Creates **Embeddings** from Abstracts, Titles, Authors Keywords or Keywords Plus
-- i) **Abstractive Text Summarization** using **PEGASUS** on a set of selected documents or all documents
-- j) **Abstractive Text Summarization** using **chatGPT** on a set of selected documents or all documents. Requires the user to have an **API key** (https://platform.openai.com/account/api-keys)
-- k) **Extractive Text Summarization** using **BERT** on a set of selected documents or all documents
-
-Correction and Manipulation Capabilities:
-- a) Filter the .bib or .txt file by Year, Sources, Bradford Law Cores, Countries, Languages and/or Abstracts (Documents with Abstracts)
-- b) Merge Authors, Institutions, Countries, Languages and/or Sources that have multiple entries 
-- c) Merge different or same database files one at a time. The preference of information preservation is given to the old database, so the order of merging matters (see Examples 04 and 05)
-
-## Usage
-
-1. Install
-```bash
-pip install pyBibX
-```
-
-2. Try it in **Colab**:
-
-- Example 01: Scopus                ([ Colab Demo ](https://colab.research.google.com/drive/1yHiMMZIKa-RrarXbPB9ca0gLN9YvvtPU?usp=sharing))
-- Example 02: WOS                   ([ Colab Demo ](https://colab.research.google.com/drive/13HLjC4myTvYcjLk2XBTZKbWJ2aqZUST1?usp=sharing))
-- Example 03: PubMed                ([ Colab Demo ](https://colab.research.google.com/drive/13CU-KvZMnazga1BmQf2J8wYM9mhHL2e1?usp=sharing))
-- Example 04: Scopus + WOS          ([ Colab Demo ](https://colab.research.google.com/drive/1DqEk0_IakJPfIZDVcnTWBE_nxyhW9p-W?usp=sharing))
-- Example 05: WOS + Scopus          ([ Colab Demo ](https://colab.research.google.com/drive/12k_IOcSDwumbEtPqqSMbCIE6ZypgKAJn?usp=sharing))
-- Example 06: Scopus + WOS + Pubmed ([ Colab Demo ](https://colab.research.google.com/drive/1Ko6AibkXtB_Kwg3Eu0fhzNMVEIXPkbez?usp=sharing))
-- Example 07: Your Own              ([ Colab Demo ](https://colab.research.google.com/drive/19EYjgal9V1kemmzpHnyp6MSlk9S-kGHT?usp=sharing))
-
-# Acknowledgement 
-This section indicates the libraries that inspired pyBibX
-
-* BERT (https://smrzr.io/)
-- a) Github: https://github.com/dmmiller612/bert-extractive-summarizer
-- b) Paper: DEREK, M. (2019). Leveraging BERT for Extractive Text Summarization on Lectures. arXiv. doi: https://doi.org/10.48550/arXiv.1906.04165
-
-* BERTopic (https://maartengr.github.io/BERTopic/index.html)
-- a) Github: https://github.com/MaartenGr/BERTopic
-- b) Paper: GROOTENDORST, M. (2022). BERTopic: Neural Topic Modeling with a Class-based TF-IDF Procedure. arXiv. doi: https://doi.org/10.48550/arXiv.2203.05794
-
-* Bibliometrix (https://www.bibliometrix.org/home/)
-- a) Github: https://github.com/massimoaria/bibliometrix
-- b) Paper: ARIA, M.; CUCCURULLO, C. (2017). Bibliometrix: An R-tool for Comprehensive Science Mapping Analysis. Journal of informetrics, 11(4), 959-975. doi: https://doi.org/10.1016/j.joi.2017.08.007
-
-* Metaknowledge (http://www.networkslab.org/metaknowledge)
-- a) Github: https://github.com/UWNETLAB/metaknowledge
-- b) Paper: McILROY-YOUNG, R.; McLEVEY, J.; ANDERSON, J. (2015). Metaknowledge: Open Source Software for Social Networks, Bibliometrics, and Sociology of Knowledge Research.
-
-* SentenceTransformers (https://www.sbert.net/)
-- a) Github: https://github.com/UKPLab/sentence-transformers
-- b) Paper: REIMERS, N.; GUREVYCH, I. (2019). Sentence-BERT: Sentence Embeddings using Siamese BERT-Networks. arXiv. doi: https://arxiv.org/abs/1908.10084
-
-* PEGASUS (https://ai.googleblog.com/2020/06/pegasus-state-of-art-model-for.html?m=1)
-- a) Github: https://github.com/huggingface/transformers
-- b) Paper: ZHANG, J.; ZHAO, Y.; SALEH, M.; LIU, P.J. (2019). PEGASUS: Pre-training with Extracted Gap-sentences for Abstractive Summarization. arXiv. doi: https://doi.org/10.48550/arXiv.1912.08777
-
-And to all the people that helped to improve or correct the code. Thank you very much!
-
-* Fabio Ribeiro von Glehn (29.DECEMBER.2022) - UFG - Federal University of Goias (Brazil)
+Metadata-Version: 2.1
+Name: pyBibX
+Version: 2.9.0
+Summary: A Bibliometric and Scientometric Library Powered with Artificial Intelligence Tools
+Home-page: https://github.com/Valdecy/pyBibX
+Author: Valdecy Pereira
+Author-email: valdecy.pereira@gmail.com
+License: GNU
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# pyBibX
+
+## Introduction
+
+A Bibliometric and Scientometric python library that uses the raw files generated by **Scopus** (.bib files), **WOS (Web of Science)** (.bib files), and **PubMed** (.txt files) scientific databases. Also Powered with Artificial Intelligence Tools to Analyze Bibliometric Results and Text Data
+
+General Capabilities:
+- a) Works with **Scopus** (.bib files), **WOS** (.bib files) and **PubMed** (.txt files) databases 
+- b) Identification and Removal of duplicates
+- c) Identification of documents per type
+- d) Generates an **EDA (Exploratory Data Analysis)** Report: Publications Timespan, Total Number of Countries, Total Number of Institutions, Total Number of Sources, Total Number of References, Total Number of Languages (and also the number of docs for each language), Total Number of Documents, Average Documents per Author, Average Documents per Institution, Average Documents per Source, Average Documents per Year, Total Number of Authors, Total Number of Authors Keywords, Total Number of Authors Keywords Plus, Total Single-Authored Documents, Total Multi-Authored Documents, Average Collaboration Index, Max H-Index, Total Number of Citations, Average Citations per Author, Average Citations per Institution, Average Citations per Document, Average Citations per Source
+- e) Creates an **ID (Identification)** for each Document, Authors, Sources, Institutions, Countries, Authors' Keywords, Keywords Plus. The IDs can be used in graphs/plots to obtain a cleaner visualization
+- f) Creates a **WordCloud** from the Abstracts, Titles, Authors Keywords or Keywords Plus
+- g) Creates a **N-Gram Bar Plot (interactive plot)** from the Abstracts, Titles, Authors Keywords or Keywords Plus
+- h) Creates a **Projection (interactive plot)** of the documents based on the Abstracts, Titles, Authors Keywords or Keywords Plus
+- i) Creates an **Evolution Plot (interactive plot)** based on Abstracts, Titles, Sources, Authors Keywords or Keywords Plus
+- j) Creates a **Sankey Diagram (interactive plot)** with any combination of the following keys: Authors, Countries, Institutions, Journals, Auhors_Keywords, Keywords_Plus, and/or Languages
+- k) Creates a **TreeMap** from the Authors, Countries, Institutions, Journals, Auhors_Keywords, or Keywords_Plus
+- l) Creates an **Authors Productivity Plot (interactive plot)** It informs for each year the documents (IDs) published for each author
+- m) Creates a **Bar Plot**  for the following statistics: Documents per Year, Citations per Year, Past Citations per Year, Lotka's Law, Sources per Documents, Sources per Citations, Authors per Documents, Authors per Citations, Authors per H-Index, Bradford's Law (Core Sources 1, 2 or 3), Institutions per Documents, Institutions per Citations, Countries per Documents, Countries per Citations, Language per Documents, Keywords Plus per Documents and Authors' Keywords per Documents
+
+Network Capabilities:
+- a) **Citation Analysis (interactive plot)** between Documents (Blue Nodes) and Citations (Red Nodes). Documents and Citations can be highlighted for better visualization
+- b) **Collaboration Analysis (interactive plot)** between Authors, Countries, Institutions or **Adjacency Analysis (interactive plot)** between Authors' Keywords or Keywords Plus. Collaboration and Adjacency can be highlighted for better visualization
+- c) **Similarity Analysis (interactive plot)** can be performed using coupling or cocitation methods
+- d) **World Map Collaboration Analysis (interactive plot)** between Countries in a Map
+
+Artificial Intelligence Capabilities:
+- a) **Topic Modelling** using BERTopic to cluster documents by topic
+- b) Visualize topics distribution
+- c) Visualize topics by the most representative words
+- d) Visualize documents projection and clusterization by topic
+- e) Visualize topics heatmap
+- f) Find the most representative documents from each topic
+- g) Find the most representative topics according to a word
+- h) Creates **Embeddings** from Abstracts, Titles, Authors Keywords or Keywords Plus
+- i) **Abstractive Text Summarization** using **PEGASUS** on a set of selected documents or all documents
+- j) **Abstractive Text Summarization** using **chatGPT** on a set of selected documents or all documents. Requires the user to have an **API key** (https://platform.openai.com/account/api-keys)
+- k) **Extractive Text Summarization** using **BERT** on a set of selected documents or all documents
+- l) **Ask chatGPT to Analyze Results** available for: EDA Report, WordCloud, N-Grams, Evolution Plot, Sankey Diagram, Authors Productivity Plot, Bar Plots, Citation Analysis, Collaboration Analysis, Similarity Analysis, and World Map Collaboration Analysis (see Example 08). Requires the user to have an **API key** (https://platform.openai.com/account/api-keys)
+
+Correction and Manipulation Capabilities:
+- a) Filter the .bib or .txt file by Year, Sources, Bradford Law Cores, Countries, Languages and/or Abstracts (Documents with Abstracts)
+- b) Merge Authors, Institutions, Countries, Languages and/or Sources that have multiple entries 
+- c) Merge different or the same database files one at a time. The preference for information preservation is given to the old database, so the order of merging matters (see Examples 04 and 05)
+
+## Usage
+
+1. Install
+```bash
+pip install pyBibX
+```
+
+2. Try it in **Colab**:
+
+- Example 01: Scopus                ([ Colab Demo ](https://colab.research.google.com/drive/1yHiMMZIKa-RrarXbPB9ca0gLN9YvvtPU?usp=sharing))
+- Example 02: WOS                   ([ Colab Demo ](https://colab.research.google.com/drive/13HLjC4myTvYcjLk2XBTZKbWJ2aqZUST1?usp=sharing))
+- Example 03: PubMed                ([ Colab Demo ](https://colab.research.google.com/drive/13CU-KvZMnazga1BmQf2J8wYM9mhHL2e1?usp=sharing))
+- Example 04: Scopus + WOS          ([ Colab Demo ](https://colab.research.google.com/drive/1DqEk0_IakJPfIZDVcnTWBE_nxyhW9p-W?usp=sharing))
+- Example 05: WOS + Scopus          ([ Colab Demo ](https://colab.research.google.com/drive/12k_IOcSDwumbEtPqqSMbCIE6ZypgKAJn?usp=sharing))
+- Example 06: Scopus + WOS + Pubmed ([ Colab Demo ](https://colab.research.google.com/drive/1Ko6AibkXtB_Kwg3Eu0fhzNMVEIXPkbez?usp=sharing))
+- Example 07: Your Own              ([ Colab Demo ](https://colab.research.google.com/drive/19EYjgal9V1kemmzpHnyp6MSlk9S-kGHT?usp=sharing))
+- Example 08: Ask chatGPT Analysis  ([ Colab Demo ](https://colab.research.google.com/drive/1LMrR49F54MuX-stlrQbrrjX_dEU3kZ8Y?usp=sharing))
+
+# Acknowledgement 
+This section indicates the libraries that inspired pyBibX
+
+* BERT (https://smrzr.io/)
+- a) Github: https://github.com/dmmiller612/bert-extractive-summarizer
+- b) Paper: DEREK, M. (2019). Leveraging BERT for Extractive Text Summarization on Lectures. arXiv. doi: https://doi.org/10.48550/arXiv.1906.04165
+
+* BERTopic (https://maartengr.github.io/BERTopic/index.html)
+- a) Github: https://github.com/MaartenGr/BERTopic
+- b) Paper: GROOTENDORST, M. (2022). BERTopic: Neural Topic Modeling with a Class-based TF-IDF Procedure. arXiv. doi: https://doi.org/10.48550/arXiv.2203.05794
+
+* Bibliometrix (https://www.bibliometrix.org/home/)
+- a) Github: https://github.com/massimoaria/bibliometrix
+- b) Paper: ARIA, M.; CUCCURULLO, C. (2017). Bibliometrix: An R-tool for Comprehensive Science Mapping Analysis. Journal of informetrics, 11(4), 959-975. doi: https://doi.org/10.1016/j.joi.2017.08.007
+
+* chatGPT (https://chat.openai.com/chat)
+- a) Github: https://github.com/openai
+- b) Paper: ECOFFET, A. (2023). GPT-4 Technical Report. arXiv. doi: https://doi.org/10.48550/arXiv.2303.08774
+
+* Metaknowledge (http://www.networkslab.org/metaknowledge)
+- a) Github: https://github.com/UWNETLAB/metaknowledge
+- b) Paper: McILROY-YOUNG, R.; McLEVEY, J.; ANDERSON, J. (2015). Metaknowledge: Open Source Software for Social Networks, Bibliometrics, and Sociology of Knowledge Research.
+
+* SentenceTransformers (https://www.sbert.net/)
+- a) Github: https://github.com/UKPLab/sentence-transformers
+- b) Paper: REIMERS, N.; GUREVYCH, I. (2019). Sentence-BERT: Sentence Embeddings using Siamese BERT-Networks. arXiv. doi: https://arxiv.org/abs/1908.10084
+
+* PEGASUS (https://ai.googleblog.com/2020/06/pegasus-state-of-art-model-for.html?m=1)
+- a) Github: https://github.com/huggingface/transformers
+- b) Paper: ZHANG, J.; ZHAO, Y.; SALEH, M.; LIU, P.J. (2019). PEGASUS: Pre-training with Extracted Gap-sentences for Abstractive Summarization. arXiv. doi: https://doi.org/10.48550/arXiv.1912.08777
+
+And to all the people that helped to improve or correct the code. Thank you very much!
+
+* Fabio Ribeiro von Glehn (29.DECEMBER.2022) - UFG - Federal University of Goias (Brazil)
```

### Comparing `pyBibX-1.7.7/pyBibX/base/pbx.py` & `pyBibX-2.9.0/pyBibX/base/pbx.py`

 * *Files 4% similar despite different names*

```diff
@@ -374,14 +374,21 @@
                                     '#f4d054', '#fbdd7e', '#ffff7e', '#cd7584', '#f9bc08', '#c7c10c'
                                   ]
         self.data, self.entries = self.__read_bib(file_bib, db, del_duplicated)
         self.__make_bib()
     
     # Function: Prepare .bib File
     def __make_bib(self, verbose = True):
+        self.ask_gpt_ap         = -1
+        self.ask_gpt_bp         = -1
+        self.ask_gpt_ep         = -1
+        self.ask_gpt_ng         = -1
+        self.ask_gpt_rt         = -1
+        self.ask_gpt_sk         = -1
+        self.ask_gpt_wd         = -1
         self.dy                 = pd.to_numeric(self.data['year'], downcast = 'float')
         self.date_str           = int(self.dy.min())
         self.date_end           = int(self.dy.max())
         self.doc_types          = self.data['document_type'].value_counts().sort_index()
         self.av_d_year          = self.dy.value_counts().sort_index()
         self.av_d_year          = round(self.av_d_year.mean(), 2)
         self.citation           = self.__get_citations(self.data['note'])
@@ -771,15 +778,15 @@
             rgba = 'black'
         return rgba
     
     #############################################################################
     
     # Function: EDA .bib docs
     def eda_bib(self):
-        report = []
+        report         = []
         report.append(['Timespan', str(self.date_str)+'-'+str(self.date_end)])
         report.append(['Total Number of Countries', len(self.u_ctr)])
         report.append(['Total Number of Institutions', len(self.u_uni)])
         report.append(['Total Number of Sources', len(self.u_jou)])
         report.append(['Total Number of References', len(self.u_ref)])
         report.append(['Total Number of Languages', len(self.u_lan)])
         for i in range(0, len(self.u_lan)):
@@ -803,15 +810,16 @@
         report.append(['-//-', '-//-'])
         report.append(['Total Number of Citations', sum(self.citation)])
         report.append(['Average Citations per Author', round(sum(self.citation)/len(self.u_aut), 2)])
         report.append(['Average Citations per Institution', round(sum(self.citation)/len(self.u_uni), 2)])
         report.append(['Average Citations per Document', self.av_c_doc])
         report.append(['Average Citations per Source', round(sum(self.jou_cit)/len(self.jou_cit), 2)])
         report.append(['-//-', '-//-'])
-        report_df = pd.DataFrame(report, columns = ['Main Information', 'Results'])
+        self.ask_gpt_rt = pd.DataFrame(report, columns = ['Main Information', 'Results'])
+        report_df       = pd.DataFrame(report, columns = ['Main Information', 'Results'])
         return report_df
 
     ##############################################################################
 
     # Function: Read .bib File
     def __read_bib(self, bib, db = 'scopus', del_duplicated = True):
         self.vb = []
@@ -1438,14 +1446,15 @@
                               contour_width    = 25, 
                               contour_color    = 'steelblue', 
                               collocations     = False, 
                               width            = 1600, 
                               height           = 800
                               )
         wordcloud.generate(corpora)
+        self.ask_gpt_wd = wordcloud.words_
         plt.figure(figsize = (size_x, size_y), facecolor = 'k')
         plt.imshow(wordcloud)
         plt.axis('off')
         plt.tight_layout(pad = 0)
         plt.show()
         return
     
@@ -1537,22 +1546,23 @@
         words_freq   = sorted(words_freq, key = lambda x: x[1], reverse = True)
         common_words = words_freq[:wordsn]
         words        = []
         freqs        = []
         for word, freq in common_words:
             words.append(word)
             freqs.append(freq) 
-        df  = pd.DataFrame({'Word': words, 'Freq': freqs})
-        fig = go.Figure(go.Bar(
-                                x           = df['Freq'],
-                                y           = df['Word'],
-                                orientation = 'h',
-                                marker      = dict(color = 'rgba(246, 78, 139, 0.6)', line = dict(color = 'black', width = 1))
-                               ),
-                        )
+        df              = pd.DataFrame({'Word': words, 'Freq': freqs})
+        self.ask_gpt_ng = pd.DataFrame({'Word': words, 'Freq': freqs})
+        fig             = go.Figure(go.Bar(
+                                            x           = df['Freq'],
+                                            y           = df['Word'],
+                                            orientation = 'h',
+                                            marker      = dict(color = 'rgba(246, 78, 139, 0.6)', line = dict(color = 'black', width = 1))
+                                           ),
+                                    )
         fig.update_yaxes(autorange = 'reversed')
         fig.update_layout(paper_bgcolor = 'rgb(248, 248, 255)', plot_bgcolor = 'rgb(248, 248, 255)')
         fig.show()
         return
     
     # Function: Tree Map
     def tree_map(self, entry = 'kwp', topn = 20, size_x = 10, size_y = 10): 
@@ -1593,15 +1603,15 @@
         plt.title(title, loc = 'center')
         plt.axis('off')
         plt.show()
         return
     
     # Function: Authors' Productivity Plot
     def authors_productivity(self, view = 'browser', topn = 20): 
-        if (view == 'browser' ):
+        if (view == 'browser'):
             pio.renderers.default = 'browser'
         if (topn > len(self.u_aut)):
             topn = len(self.u_aut)
         years        = list(range(self.date_str, self.date_end+1))    
         dicty        = dict(zip(years, list(range(0, len(years)))))
         idx          = sorted(range(0, len(self.doc_aut)), key = self.doc_aut.__getitem__)
         idx.reverse()
@@ -1618,14 +1628,16 @@
             docs = [i for i in range(0, len(self.aut)) if name in self.aut[i]]
             for i in docs:
                 j                       = dicty[int(self.data.loc[i, 'year'])]
                 productivity.iloc[n, j] = productivity.iloc[n, j] + 1
                 n_id[n][j].append( 'id: '+str(i)+' ('+name+', '+self.data.loc[i, 'year']+')')
                 Xv.append(n)
                 Yv.append(j)
+        self.ask_gpt_ap = productivity.copy(deep = True)
+        self.ask_gpt_ap = self.ask_gpt_ap.loc[(self.ask_gpt_ap.sum(axis = 1) != 0), (self.ask_gpt_ap.sum(axis = 0) != 0)]
         node_list_a = [ str(int(productivity.iloc[Xv[i], Yv[i]])) for i in range(0, len(Xv)) ]
         nid_list    = [ n_id[Xv[i]][Yv[i]] for i in range(0, len(Xv)) ]
         nid_list_a  = []
         for item in nid_list:
             if (len(item) == 1):
                 nid_list_a.append(item)
             else:
@@ -1691,35 +1703,32 @@
         fig_aut.update_traces(textfont_size = 10, textfont_color = 'white') 
         fig_aut.update_yaxes(autorange = 'reversed')
         fig_aut.show() 
         return
     
     # Function: Evolution per Year
     def plot_evolution_year(self, view = 'browser', stop_words = ['en'], key = 'kwp', rmv_custom_words = [], topn = 10, start = 2010, end = 2022):
-        if (view == 'browser' ):
+        if (view == 'browser'):
             pio.renderers.default = 'browser'
         if (start < self.date_str or start == -1):
             start = self.date_str
         if (end > self.date_end or end == -1):
             end = self.date_end
         y_idx = [i for i in range(0, self.data.shape[0]) if int(self.data.loc[i, 'year']) >= start and int(self.data.loc[i, 'year']) <= end]
         if (len(rmv_custom_words) == 0):
             rmv_custom_words = ['unknow']
         else:
             rmv_custom_words.append('unknow') 
         if   (key == 'kwp'):
-            #u_ent, ent = self.u_kid, self.kid
             u_ent = [item for item in self.u_kid]
             ent   = [item for item in self.kid]
         elif (key == 'kwa'):
-            #u_ent, ent = self.u_auk, self.auk
             u_ent = [item for item in self.u_auk]
             ent   = [item for item in self.auk]
         elif (key == 'jou'):
-            #u_ent, ent = self.u_jou, self.jou
             u_ent = [item for item in self.u_jou]
             ent   = [item for item in self.jou]
         elif (key == 'abs'):
             abs_  = self.data['abstract'].tolist()
             abs_  = ['the' if i not in y_idx else  abs_[i] for i in range(0, len(abs_))]
             abs_  = self.clear_text(abs_, stop_words = stop_words, lowercase = True, rmv_accents = True, rmv_special_chars = True, rmv_numbers = True, rmv_custom_words = rmv_custom_words)
             u_abs = [item.split() for item in abs_]
@@ -1752,47 +1761,50 @@
             tit_       = [item.split() for item in tit_]
             u_tit      = [u_tit[i] for i in idx]
             u_ent, ent = u_tit, tit_
         traces = []
         years  = list(range(self.date_str, self.date_end+1))
         dict_y = dict(zip(years, list(range(0, len(years)))))
         themes = self.__get_counts_year(u_ent, ent)
-        w_idx  = []
+        #w_idx  = []
         #if (len(target_word) > 0):
             #posit  = -1
             #for word in target_word:
                 #if (word.lower() in u_ent):
                     #posit = u_ent.index(word.lower())
                 #if (posit > 0):
                     #w_idx.append(posit)
             #if (len(w_idx) > 0):
                 #themes = themes.iloc[w_idx, :]
+        self.ask_gpt_ep = ''
         for j in range(dict_y[start], dict_y[end]+1):
             theme_vec = themes.iloc[:, j]
             theme_vec = theme_vec[theme_vec > 0]
             if (len(theme_vec) > 0):
                 theme_vec = theme_vec.sort_values(ascending = False) 
                 theme_vec = theme_vec.iloc[:topn] 
                 idx       = theme_vec.index.tolist()
                 names     = [u_ent[item] for item in idx]
-                if (len(w_idx) > 0):
-                    values = [themes.loc[item, j] for item in idx]
-                else:
-                    values = [themes.iloc[item, j] for item in idx]
-                n_val     = [names[i]+' ('+str(int(values[i]))+')' for i in range(0, len(names))]
-                data      = go.Bar(x                = [years[j]]*len(values), 
-                                   y                = values, 
-                                   text             = names, 
-                                   hoverinfo        = 'text',
-                                   textangle        = 0,
-                                   textfont_size    = 10,
-                                   hovertext        = n_val,
-                                   insidetextanchor = 'middle',
-                                   marker_color     = self.__hex_rgba(hxc = self.color_names[j], alpha = 0.70)
-                                   )
+                values    = [themes.loc[item, j] for item in idx]
+                #if (len(w_idx) > 0):
+                    #values = [themes.loc[item, j] for item in idx]
+                #else:
+                    #values = [themes.iloc[item, j] for item in idx]
+                n_val           = [names[i]+' ('+str(int(values[i]))+')' for i in range(0, len(names))]
+                self.ask_gpt_ep = self.ask_gpt_ep + ' ' + str(years[j]) + ': ' + ', '.join(n_val)
+                data            = go.Bar(x                = [years[j]]*len(values), 
+                                         y                = values, 
+                                         text             = names, 
+                                         hoverinfo        = 'text',
+                                         textangle        = 0,
+                                         textfont_size    = 10,
+                                         hovertext        = n_val,
+                                         insidetextanchor = 'middle',
+                                         marker_color     = self.__hex_rgba(hxc = self.color_names[j], alpha = 0.70)
+                                         )
                 traces.append(data)
         layout = go.Layout(barmode      = 'stack', 
                            showlegend   = False,
                            hovermode    = 'closest',
                            margin       = dict(b = 10, l = 5, r = 5, t = 10),
                            plot_bgcolor = '#f5f5f5',
                            xaxis        = dict(tickangle      =  35,
@@ -2023,17 +2035,20 @@
             key   = [key[i]   for i in idx]
             value = [value[i] for i in idx]
             key   = key[:topn]
             value = value[:topn]
             title = 'Top '+ str(topn)+" - Authors' Keywords per Documents"
             x_lbl = 'Documents'
             y_lbl = "Authors' Keywords"
-        w_1 = 0.135
-        w_2 = 0.045
-        w_s = np.arange(len(value) / 8, step = 0.125)
+        data_tuples       = list(zip(key, value))
+        self.ask_gpt_bp   = pd.DataFrame(data_tuples, columns = [x_lbl, y_lbl])
+        self.ask_gpt_bp_t = title
+        w_1               = 0.135
+        w_2               = 0.045
+        w_s               = np.arange(len(value) / 8, step = 0.125)
         plt.figure(figsize = [size_x, size_y])
         if (statistic.lower() == 'dpy' or statistic.lower() == 'cpy' or statistic.lower() == 'ppy' or statistic.lower() == 'ltk'):
             plt.bar(w_s, value, color = '#dce6f2', width = w_1/2, edgecolor = '#c3d5e8')
             plt.bar(w_s, value, color = '#ffc001', width = w_2/2, edgecolor = '#c3d5e8')
             if (statistic.lower() != 'ltk'):
                 plt.axhline(y = sum(value)/len(value), color = 'r', linestyle = '-', lw = 0.75)
             plt.axhline(y = 0, color = 'gray')
@@ -2057,15 +2072,15 @@
     # Function: Sankey Diagram
     def sankey_diagram(self, view = 'browser', entry = ['aut', 'cout', 'inst'], topn = 20): 
         def sort_count(u_lst, count_lst):
             idx   = sorted(range(0, len(count_lst)), key = count_lst.__getitem__)
             idx.reverse()
             u_lst = [u_lst[i] for i in idx]
             return u_lst   
-        if (view == 'browser' ):
+        if (view == 'browser'):
             pio.renderers.default = 'browser'
         u_keys = ['aut', 'cout', 'inst', 'jou', 'kwa', 'kwp', 'lan']
         u_name = ['Authors', 'Countries', 'Institutions', 'Journals', 'Auhors_Keywords', 'Keywords_Plus', 'Languages']
         u_idx  = [i for i in range(0, len(u_keys)) if u_keys[i] == entry[0]]
         u_cnt  = [self.doc_aut, self.ctr_count, self.uni_count, self.jou_count, self.auk_count, self.kid_count, self.lan_count]
         u_list = [self.aut, self.ctr, self.uni, self.jou, self.auk, self.kid, self.lan]
         u_sort = [self.u_aut, self.u_ctr, self.u_uni, self.u_jou, self.u_auk, self.u_kid, self.u_lan]
@@ -2158,14 +2173,20 @@
                         sk_t.append(dict_s[s_pair[i][1]])
                         sk_v.append(s_vals[i])             
         if (len(sk_s) > len(self.color_names)):
             count = 0
             while (len(self.color_names) < len(sk_s)):
                 self.color_names.append(self.color_names[count])
                 count = count + 1
+        self.ask_gpt_sk = pd.DataFrame(list(zip(sk_s, sk_t, sk_v)), columns = ['Node From', 'Node To', 'Connection Weigth'])
+        for i in range(0, len(sk_s)):
+            source                     = label[self.ask_gpt_sk.iloc[i, 0]]
+            target                     = label[self.ask_gpt_sk.iloc[i, 1]]
+            self.ask_gpt_sk.iloc[i, 0] = source
+            self.ask_gpt_sk.iloc[i, 1] = target
         link = dict(source = sk_s, target = sk_t,   value = sk_v, color = self.color_names)
         node = dict(label  = label,   pad = 10, thickness = 15,   color = 'white')
         data = go.Sankey(
                           link        = link, 
                           node        = node, 
                           arrangement = 'freeform'
                          )
@@ -2657,18 +2678,21 @@
             self.matrix_r         = self.matrix_r.iloc[:, cols]
             self.labels_r         = [self.labels_r[item] for item in cols]
             self.matrix_r.columns = self.labels_r 
         return self
 
     # Function: Network Similarities 
     def network_sim(self, view = 'browser', sim_type = 'coup', node_size = -1, node_labels = False, cut_coup = 0.3, cut_cocit = 5):
+        sim = ''
         if   (sim_type == 'coup'):
             cut = cut_coup
+            sim = 'Bibliographic Coupling'
         elif (sim_type == 'cocit'):
             cut = cut_cocit
+            sim = 'Co-Citation'
         if (view == 'browser' ):
             pio.renderers.default = 'browser'
         if (node_labels == True):
             mode = 'markers+text'
             size = 17
         else:
             mode = 'markers'
@@ -2711,24 +2735,28 @@
             S.add_node(name, color = color, year = year, n_id = n_id )
         for name in u_cols:
             if (name not in u_rows):
                 color = 'blue'
                 year  = int(self.dy[ int(name) ])
                 n_id  = self.data.loc[int(name), 'author']+' ('+self.data.loc[int(name), 'year']+'). '+self.data.loc[int(name), 'title']+'. '+self.data.loc[int(name), 'journal']+'. doi:'+self.data.loc[int(name), 'doi']+'. '
                 S.add_node(name, color = color, year = year, n_id = n_id )
-        self.sim_table = pd.DataFrame(np.zeros((len(edges), 2)), columns = ['Pair Node', 'Sim('+sim_type+')'])
+        self.sim_table   = pd.DataFrame(np.zeros((len(edges), 2)), columns = ['Pair Node', 'Sim('+sim_type+')'])
+        self.ask_gpt_sim = pd.DataFrame(np.zeros((len(edges), 3)), columns = ['Node 1', 'Node 2', 'Simimilarity ('+sim+') Between Nodes'])
         for i in range(0, len(edges)):
             srt, end = edges[i]
             srt_     = str(srt)
             end_     = str(end)
             if ( end_ != '-1' ):
                 wght = round(adjacency_matrix[srt, end], 3)
                 S.add_edge(srt_, end_, weight = wght)
-                self.sim_table.iloc[i, 0] = '('+srt_+','+end_+')'
-                self.sim_table.iloc[i, 1] = wght
+                self.sim_table.iloc[i, 0]   = '('+srt_+','+end_+')'
+                self.sim_table.iloc[i, 1]   = wght
+                self.ask_gpt_sim.iloc[i, 0] = 'Paper ID: '+srt_
+                self.ask_gpt_sim.iloc[i, 1] = 'Paper ID: '+end_
+                self.ask_gpt_sim.iloc[i, 2] = wght
         generator      = nx.algorithms.community.girvan_newman(S)
         community      = next(generator)
         community_list = sorted(map(sorted, community))
         for com in community_list:
             community_list.index(com)
             for node in com:
                 S.nodes[node]['color'] = self.color_names[community_list.index(com)]
@@ -2778,45 +2806,48 @@
         fig_s.update_layout(yaxis = dict(scaleanchor = 'x', scaleratio = 0.5), plot_bgcolor = 'rgb(255, 255, 255)',  hoverlabel = dict(font_size = 12))
         fig_s.update_traces(textfont_size = 10, textfont_color = 'blue', textposition = 'top center') 
         fig_s.show()  
         return
 
     # Function: Map from Country Adjacency Matrix
     def network_adj_map(self, view = 'browser', connections = True, country_lst = []):
-        if (view == 'browser' ):
+        if (view == 'browser'):
             pio.renderers.default = 'browser'
         lat_  = [self.country_lat_long[i][0] for i in range(0, len(self.country_lat_long)) if self.country_names[i] in self.u_ctr]
         lon_  = [self.country_lat_long[i][1] for i in range(0, len(self.country_lat_long)) if self.country_names[i] in self.u_ctr]
         iso_3 = [self.country_alpha_3[i] for i in range(0, len(self.country_lat_long)) if self.country_names[i] in self.u_ctr]
         text  = [item for item in self.country_names if item in self.u_ctr]
         self.__adjacency_matrix_ctr(1)
         adjacency_matrix = self.matrix_a.values
         vals  = [ int(self.dict_ctr_id[text[i]].replace('c_','')) for i in range(0, len(text)) ]
         vals  = [ int(np.sum(adjacency_matrix[i,:])) for i in vals ]
         lat_  = [ lat_[i] for i in range(0, len(vals)) if vals[i] > 0]
         lon_  = [ lon_[i] for i in range(0, len(vals)) if vals[i] > 0]
         iso_3 = [iso_3[i] for i in range(0, len(vals)) if vals[i] > 0]
         text  = [ text[i] for i in range(0, len(vals)) if vals[i] > 0]
         vals  = [ vals[i] for i in range(0, len(vals)) if vals[i] > 0]
-        rows, cols = np.where(adjacency_matrix >= 1)
-        edges      = list(zip(rows.tolist(), cols.tolist()))
+        rows, cols       = np.where(adjacency_matrix >= 1)
+        edges            = list(zip(rows.tolist(), cols.tolist()))
+        self.ask_gpt_map = pd.DataFrame(edges, columns = ['Country 1', 'Country 2']) 
         nids_list  = ['id:                        ' +self.dict_ctr_id[text[i]]+'<br>'+
                       'country:               '     +text[i].upper()+'<br>' +
                       'collaborators:      '        +str(vals[i])  
                       for i in range(0, len(lat_))]
         Xa         = []
         Ya         = []
         Xb         = []
         Yb         = []
         for i in range(0, len(edges)):
             srt, end = edges[i]
             srt      = 'c_'+str(srt)
             end      = 'c_'+str(end)
             srt      = self.dict_id_ctr[srt]
             end      = self.dict_id_ctr[end]
+            self.ask_gpt_map.iloc[i, 0] = srt
+            self.ask_gpt_map.iloc[i, 1] = end
             if (len(country_lst) > 0):
                 country_lst = [item.lower() for item in country_lst]
                 for j in range(0, len(country_lst)):
                     if (srt.lower() in country_lst or end.lower() in country_lst):
                         srt_ = self.country_names.index(srt)
                         end_ = self.country_names.index(end)
                         Xb.append(self.country_lat_long[srt_][0]) 
@@ -2931,25 +2962,26 @@
             G.add_node(name, color = color, year = year, n_id = n_id )
         for i in range(0, len(edges)):
             srt, end = edges[i]
             srt_     = str(srt)
             end_     = self.labels_r[end]
             if ( end_ != '-1' ):
                 G.add_edge(srt_, end_)
-        color          = [G.nodes[n]['color'] if len(G.nodes[n]) > 0 else 'black' for n in G.nodes()]
-        self.pos       = nx.circular_layout(G)
-        self.node_list = list(G.nodes)
-        self.edge_list = list(G.edges)
-        self.nids_list = [G.nodes[n]['n_id'] for n in G.nodes()]
-        self.nids_list = ['<br>'.join(textwrap.wrap(txt, width = 50)) for txt in self.nids_list]
-        self.nids_list = ['id: '+self.node_list[i]+'<br>'+self.nids_list[i] for i in range(0, len(self.nids_list))]
-        self.Xn        = [self.pos[k][0] for k in self.node_list]
-        self.Yn        = [self.pos[k][1] for k in self.node_list]
-        Xa             = []
-        Ya             = []
+        self.ask_gpt_nad = pd.DataFrame(G.edges, columns = ['Paper', 'Cited Reference'])
+        color            = [G.nodes[n]['color'] if len(G.nodes[n]) > 0 else 'black' for n in G.nodes()]
+        self.pos         = nx.circular_layout(G)
+        self.node_list   = list(G.nodes)
+        self.edge_list   = list(G.edges)
+        self.nids_list   = [G.nodes[n]['n_id'] for n in G.nodes()]
+        self.nids_list   = ['<br>'.join(textwrap.wrap(txt, width = 50)) for txt in self.nids_list]
+        self.nids_list   = ['id: '+self.node_list[i]+'<br>'+self.nids_list[i] for i in range(0, len(self.nids_list))]
+        self.Xn          = [self.pos[k][0] for k in self.node_list]
+        self.Yn          = [self.pos[k][1] for k in self.node_list]
+        Xa               = []
+        Ya               = []
         for edge in self.edge_list:
             Xa.append(self.pos[edge[0]][0]*0.97)
             Xa.append(self.pos[edge[1]][0]*0.97)
             Xa.append(None)
             Ya.append(self.pos[edge[0]][1]*0.97)
             Ya.append(self.pos[edge[1]][1]*0.97)
             Ya.append(None)
@@ -2980,15 +3012,17 @@
         self.fig.update_layout(yaxis = dict(scaleanchor = 'x', scaleratio = 0.5), plot_bgcolor = 'rgb(255, 255, 255)',  hoverlabel = dict(font_size = 12))
         self.fig.update_traces(textfont_size = 10, textfont_color = 'yellow') 
         self.fig.show()
         return
 
     # Function: Network from Adjacency Matrix 
     def network_adj(self, view = 'browser', adj_type = 'aut', min_count = 2, node_size = -1, node_labels = False, label_type = 'id', centrality = None): 
-        if (view == 'browser' ):
+        adj_ = ''
+        cen_ = 'Girvan-Newman Community Algorithm'
+        if (view == 'browser'):
             pio.renderers.default = 'browser'
         if (node_labels == True):
             mode = 'markers+text'
             size = 17
         else:
             mode = 'markers'
             size = 10
@@ -2998,30 +3032,35 @@
         elif (node_labels == False and node_size > 0):
             mode = 'markers'
             size = node_size
         if   (adj_type == 'aut'):
             self.__adjacency_matrix_aut(min_count)
             adjacency_matrix = self.matrix_a.values
             dict_            = self.dict_id_aut
+            adj_             = 'Author'
         elif (adj_type == 'cout'):
             self.__adjacency_matrix_ctr(min_count)
             adjacency_matrix = self.matrix_a.values
             dict_            = self.dict_id_ctr
+            adj_             = 'Country'
         elif (adj_type == 'inst'):
             self.__adjacency_matrix_inst(min_count)
             adjacency_matrix = self.matrix_a.values
             dict_            = self.dict_id_uni
+            adj_             = 'Institution'
         elif (adj_type == 'kwa'):
             self.__adjacency_matrix_kwa(min_count)
             adjacency_matrix = self.matrix_a.values
             dict_            = self.dict_id_kwa
+            adj_             = 'Author Keywords'
         elif (adj_type == 'kwp'):
             self.__adjacency_matrix_kwp(min_count)
             adjacency_matrix = self.matrix_a.values
             dict_            = self.dict_id_kwp
+            adj_             = 'Keywords Plus'
         rows, cols = np.where(adjacency_matrix >= 1)
         edges      = list(zip(rows.tolist(), cols.tolist()))
         u_cols     = list(set(cols.tolist()))
         self.H     = nx.Graph()
         if (adj_type == 'aut'):
             for i in range(0, len(u_cols)): 
                 name  = self.labels_a[u_cols[i]]
@@ -3066,82 +3105,115 @@
                 self.H.add_node(name, n_cls = n_cls, color = color, n_coa = n_coa, n_id = n_id )  
         for i in range(0, len(edges)):
             srt, end = edges[i]
             srt_     = self.labels_a[srt]
             end_     = self.labels_a[end]
             if ( end_ != '-1'):
                 self.H.add_edge(srt_, end_)
-        if   (centrality == 'degree'): 
+        dict_cen = []
+        if (centrality == 'degree'): 
             value            = nx.algorithms.centrality.degree_centrality(self.H)
             color            = [value[n] for n in self.H.nodes()]
             self.table_centr = pd.DataFrame(value.items(), columns = ['Node', 'Degree'])
             self.table_centr = self.table_centr.sort_values('Degree', ascending = False)
             self.table_centr.insert(0, 'Name', [dict_[self.table_centr.iloc[i, 0]] for i in range(0, self.table_centr.shape[0])])
+            cen_             = 'Degree Centrality'
+            dict_cen         = dict(zip(self.table_centr.iloc[:,-2], self.table_centr.iloc[:,-1]))
         elif (centrality == 'load'):
             value            = nx.algorithms.centrality.load_centrality(self.H)
             color            = [value[n] for n in self.H.nodes()]
             self.table_centr = pd.DataFrame(value.items(), columns = ['Node', 'Load'])
             self.table_centr = self.table_centr.sort_values('Load', ascending = False)
             self.table_centr.insert(0, 'Name', [dict_[self.table_centr.iloc[i, 0]] for i in range(0, self.table_centr.shape[0])])
+            cen_             = 'Load Centrality'
+            dict_cen         = dict(zip(self.table_centr.iloc[:,-2], self.table_centr.iloc[:,-1]))
         elif (centrality == 'betw'):
             value            = nx.algorithms.centrality.betweenness_centrality(self.H)
             color            = [value[n] for n in self.H.nodes()]
             self.table_centr = pd.DataFrame(value.items(), columns = ['Node', 'Betweenness'])
             self.table_centr = self.table_centr.sort_values('Betweenness', ascending = False)
             self.table_centr.insert(0, 'Name', [dict_[self.table_centr.iloc[i, 0]] for i in range(0, self.table_centr.shape[0])])
+            cen_             = 'Betweenness Centrality'
+            dict_cen         = dict(zip(self.table_centr.iloc[:,-2], self.table_centr.iloc[:,-1]))
         elif (centrality == 'close'):
             value            = nx.algorithms.centrality.closeness_centrality(self.H)
             color            = [value[n] for n in self.H.nodes()]
             self.table_centr = pd.DataFrame(value.items(), columns = ['Node', 'Closeness'])
             self.table_centr = self.table_centr.sort_values('Closeness', ascending = False)
             self.table_centr.insert(0, 'Name', [dict_[self.table_centr.iloc[i, 0]] for i in range(0, self.table_centr.shape[0])])
+            cen_             = 'Closeness Centrality'
+            dict_cen         = dict(zip(self.table_centr.iloc[:,-2], self.table_centr.iloc[:,-1]))
         elif (centrality == 'eigen'):
             value            = nx.algorithms.centrality.eigenvector_centrality(self.H)
             color            = [value[n] for n in self.H.nodes()]
             self.table_centr = pd.DataFrame(value.items(), columns = ['Node', 'Eigenvector'])
             self.table_centr = self.table_centr.sort_values('Eigenvector', ascending = False)
             self.table_centr.insert(0, 'Name', [dict_[self.table_centr.iloc[i, 0]] for i in range(0, self.table_centr.shape[0])])
+            cen_             = 'Eigenvector Centrality'
+            dict_cen         = dict(zip(self.table_centr.iloc[:,-2], self.table_centr.iloc[:,-1]))
         elif (centrality == 'katz'):
             value            = nx.algorithms.centrality.katz_centrality(self.H)
             color            = [value[n] for n in self.H.nodes()]
             self.table_centr = pd.DataFrame(value.items(), columns = ['Node', 'Katz'])
             self.table_centr = self.table_centr.sort_values('Katz', ascending = False)
             self.table_centr.insert(0, 'Name', [dict_[self.table_centr.iloc[i, 0]] for i in range(0, self.table_centr.shape[0])])
+            cen_             = 'Katz Centrality'
+            dict_cen         = dict(zip(self.table_centr.iloc[:,-2], self.table_centr.iloc[:,-1]))
         elif (centrality == 'harmonic'):
             value            = nx.algorithms.centrality.harmonic_centrality(self.H)
             color            = [value[n] for n in self.H.nodes()]
             self.table_centr = pd.DataFrame(value.items(), columns = ['Node', 'Harmonic'])
             self.table_centr = self.table_centr.sort_values('Harmonic', ascending = False)
             self.table_centr.insert(0, 'Name', [dict_[self.table_centr.iloc[i, 0]] for i in range(0, self.table_centr.shape[0])])
+            cen_             = 'Harmonic Centrality'
+            dict_cen         = dict(zip(self.table_centr.iloc[:,-2], self.table_centr.iloc[:,-1]))
         else:
             generator        = nx.algorithms.community.girvan_newman(self.H)
             community        = next(generator)
             community_list   = sorted(map(sorted, community))
             for com in community_list:
                 community_list.index(com)
                 for node in com:
                     self.H.nodes[node]['color'] = self.color_names[community_list.index(com)]
                     self.H.nodes[node]['n_cls'] = community_list.index(com)
             color = [self.H.nodes[n]['color'] for n in self.H.nodes()]
         self.pos_a       = nx.spring_layout(self.H, seed = 42, scale = 1000)
         self.node_list_a = list(self.H.nodes)
         self.edge_list_a = list(self.H.edges)
+        if (cen_ == 'Girvan-Newman Community Algorithm'):
+            self.ask_gpt_adj = pd.DataFrame((np.zeros((len(self.H.edges), 4))), columns = ['Node 1'+' ('+adj_+')', 'Node 2'+' ('+adj_+')', 'Node 1 Cluster', 'Node 2 Cluster'])
+        else:
+            self.ask_gpt_adj = pd.DataFrame((np.zeros((len(self.H.edges), 4))), columns = ['Node 1'+' ('+adj_+')', 'Node 2'+' ('+adj_+')', 'Node 1' + ' ('+cen_+')', 'Node 2' + ' ('+cen_+')'])
+        if (cen_ == 'Girvan-Newman Community Algorithm'):
+            for i in range(0, self.ask_gpt_adj.shape[0]):
+                srt, end                    = list(self.H.edges)[i]
+                self.ask_gpt_adj.iloc[i, 0] = 'ID: ' + srt
+                self.ask_gpt_adj.iloc[i, 1] = 'ID: ' + end
+                self.ask_gpt_adj.iloc[i, 2] = self.H.nodes[srt]['n_cls']
+                self.ask_gpt_adj.iloc[i, 3] = self.H.nodes[end]['n_cls']
+        else:
+            for i in range(0, self.ask_gpt_adj.shape[0]):
+                srt, end                    = list(self.H.edges)[i]
+                self.ask_gpt_adj.iloc[i, 0] = 'ID: ' + srt
+                self.ask_gpt_adj.iloc[i, 1] = 'ID: ' + end
+                self.ask_gpt_adj.iloc[i, 2] = dict_cen[srt]
+                self.ask_gpt_adj.iloc[i, 3] = dict_cen[end]    
         if (adj_type == 'aut'):
             docs_list_a      = [self.H.nodes[n]['n_doc'] for n in self.H.nodes()]
             auts_list_a      = [self.H.nodes[n]['n_coa'] for n in self.H.nodes()]
             lhid_list_a      = [self.H.nodes[n]['n_lhi'] for n in self.H.nodes()]
             clst_list_a      = [self.H.nodes[n]['n_cls'] for n in self.H.nodes()]
             self.nids_list_a = [self.H.nodes[n]['n_id']  for n in self.H.nodes()]
             self.nids_list_a = ['id:                       ' +self.node_list_a[i]+'<br>'+
                                 'cluster:                '   +str(clst_list_a[i])+'<br>'+
                                 'author:                '    +self.nids_list_a[i].upper()+'<br>'+
                                 'documents:         '        +str(docs_list_a[i])+'<br>'+
                                 'collaborators:      '       +str(auts_list_a[i])+'<br>'+
                                 'local h-index:       '      +str(lhid_list_a[i]) 
-                                for i in range(0, len(self.nids_list_a))]
+                                for i in range(0, len(self.nids_list_a))]     
         elif (adj_type == 'cout'):  
             auts_list_a      = [self.H.nodes[n]['n_coa'] for n in self.H.nodes()]
             clst_list_a      = [self.H.nodes[n]['n_cls'] for n in self.H.nodes()]
             self.nids_list_a = [self.H.nodes[n]['n_id']  for n in self.H.nodes()]
             self.nids_list_a = ['id:                        ' +self.node_list_a[i]+'<br>'+
                                 'cluster:                '    +str(clst_list_a[i])+'<br>'+
                                 'country:               '     +self.nids_list_a[i].upper()+'<br>' +
@@ -3524,19 +3596,24 @@
             Yn.append(flag)
         for i in range(0, len(edges)):
             srt, end = edges[i]
             srt_     = str(srt)
             end_     = self.labels_r[end]
             if ( end_ != '-1' ):
                 G.add_edge(srt_, end_)
-        node_list = list(G.nodes)
-        edge_list = list(G.edges)
-        nids_list = [G.nodes[n]['n_id'] for n in G.nodes()]
-        nids_list = ['<br>'.join(textwrap.wrap(txt, width = 50)) for txt in nids_list]
-        nids_list = ['id: '+node_list[i]+'<br>'+nids_list[i] for i in range(0, len(nids_list))]
+        self.ask_gpt_hist = pd.DataFrame(G.edges, columns = ['Paper ID (Year)', 'References (Year)'])
+        for i in range(0, self.ask_gpt_hist.shape[0]):
+            self.ask_gpt_hist.iloc[i, 0] = str(self.ask_gpt_hist.iloc[i, 0]) + ' (' + str(G.nodes[self.ask_gpt_hist.iloc[i,0]]['year']) + ')'
+            self.ask_gpt_hist.iloc[i, 1] = str(self.ask_gpt_hist.iloc[i, 1]) + ' (' + str(G.nodes[self.ask_gpt_hist.iloc[i,1]]['year']) + ')'
+        self.ask_gpt_hist = self.ask_gpt_hist[self.ask_gpt_hist.apply(lambda row: len(row.unique()) > 1, axis = 1)]
+        node_list         = list(G.nodes)
+        edge_list         = list(G.edges)
+        nids_list         = [G.nodes[n]['n_id'] for n in G.nodes()]
+        nids_list         = ['<br>'.join(textwrap.wrap(txt, width = 50)) for txt in nids_list]
+        nids_list         = ['id: '+node_list[i]+'<br>'+nids_list[i] for i in range(0, len(nids_list))]
         for edge in edge_list:
             Xa.append(dict_y[G.nodes[edge[0]]['year']]) 
             Xa.append(dict_y[G.nodes[edge[1]]['year']])
             Xa.append(None)
             Ya.append(G.nodes[edge[0]]['flag'])
             Ya.append(G.nodes[edge[1]]['flag'])
             Ya.append(None)
@@ -3925,23 +4002,25 @@
         for i in range(0, abstracts.shape[0]):
             if (abstracts.iloc[i] != 'UNKNOW' and i in article_ids):
                 corpus.append('Abstract (Document ID' + str(i) + '):\n\n')
                 corpus.append(abstracts.iloc[i])
                 print('Document ID' + str(i) + ' Number of Characters: ' + str(len(abstracts.iloc[i])))
         if (len(corpus) > 0):
             print('')
-            print('Total Number of Valid Abstracts: ', len(corpus)/2)
+            print('Total Number of Valid Abstracts: ', int(len(corpus)/2))
             print('')
             if (join_articles == False):
                 for i, abstract in enumerate(corpus):
                     prompt = query + ':\n\n' + f'{i+1}. {corpus}\n'
             else:    
                 corpus = ' '.join(corpus)
                 prompt = query + ':\n\n' + f'{i+1}. {corpus}\n'
             summary = query_chatgpt(prompt)
+        else:
+            summary    = 'No abstracts were found in the selected set of documents'
         return summary
 
     # Function: Extractive Text Summarization
     def summarize_ext_bert(self, article_ids = []):
         abstracts = self.data['abstract']
         corpus    = []
         if (len(article_ids) == 0):
@@ -3958,8 +4037,267 @@
             corpus     = ' '.join(corpus)
             bert_model = Summarizer()
             summary    = ''.join(bert_model(corpus, min_length = 5))
         else:
             summary    = 'No abstracts were found in the selected set of documents'
         return summary
 
+############################################################################
+
+    # Function: Ask chatGPT about Authors Productivity by Year
+    def ask_chatgpt_ap(self, char_limit = 4097, api_key = 'your_api_key_here', query = 'give me insights about the following information, related to authors productivity by year'):
+        def query_chatgpt(prompt, model = 'text-davinci-003', n = 1):
+            response = openai.Completion.create(
+                                                engine      = model,
+                                                prompt      = prompt,
+                                                max_tokens  = 2000,
+                                                n           = n,
+                                                stop        = None,
+                                                temperature = 0.8
+                                                )
+            return response.choices[0].text.strip()
+        corpus = ''
+        for author, row in self.ask_gpt_ap.iterrows():
+            years        = [(year, row[year]) for year in row.index if row[year] > 0]
+            paper_counts = ', '.join([f'({year}: {count} paper{"s" if count > 1 else ""})' for year, count in years])
+            corpus       = corpus +  f'{author} {paper_counts}\n'
+        openai.api_key = api_key
+        prompt         = query + ':\n\n' + f'{corpus}\n'
+        prompt         = prompt[:char_limit]
+        analyze        = query_chatgpt(prompt)
+        print('Number of Characters: ' + str(len(prompt)))
+        return analyze
+    
+    # Function: Ask chatGPT about Bar Plots 
+    def ask_chatgpt_bp(self, char_limit = 4097, api_key = 'your_api_key_here', query = 'give me insights about the following information'):
+        def query_chatgpt(prompt, model = 'text-davinci-003', n = 1):
+            response = openai.Completion.create(
+                                                engine      = model,
+                                                prompt      = prompt,
+                                                max_tokens  = 2000,
+                                                n           = n,
+                                                stop        = None,
+                                                temperature = 0.8
+                                                )
+            return response.choices[0].text.strip()
+        corpus         = self.ask_gpt_bp.to_string(index = False)    
+        openai.api_key = api_key
+        prompt         = query + ' regarding ' + self.ask_gpt_bp_t + ':\n\n' + f'{corpus}\n'
+        prompt         = prompt[:char_limit]
+        analyze        = query_chatgpt(prompt)
+        print('Number of Characters: ' + str(len(prompt)))
+        return analyze
+    
+    # Function: Ask chatGPT about Citation Analysis 
+    def ask_chatgpt_citation(self, char_limit = 4097, api_key = 'your_api_key_here', query = 'give me insights about the following information'):
+        def query_chatgpt(prompt, model = 'text-davinci-003', n = 1):
+            response = openai.Completion.create(
+                                                engine      = model,
+                                                prompt      = prompt,
+                                                max_tokens  = 2000,
+                                                n           = n,
+                                                stop        = None,
+                                                temperature = 0.8
+                                                )
+            return response.choices[0].text.strip()
+        corpus         = self.ask_gpt_nad.to_string(index = False)    
+        openai.api_key = api_key
+        prompt         = query + ':\n\n' + f'{corpus}\n'
+        prompt         = prompt[:char_limit]
+        analyze        = query_chatgpt(prompt)
+        print('Number of Characters: ' + str(len(prompt)))
+        return analyze
+
+    # Function: Ask chatGPT about Collaboration Analysis
+    def ask_chatgpt_colab(self, char_limit = 4097, api_key = 'your_api_key_here', query = 'give me insights about the following network information, knowing that Node 1 is connected with Node 2'):
+        def query_chatgpt(prompt, model = 'text-davinci-003', n = 1):
+            response = openai.Completion.create(
+                                                engine      = model,
+                                                prompt      = prompt,
+                                                max_tokens  = 2000,
+                                                n           = n,
+                                                stop        = None,
+                                                temperature = 0.8
+                                                )
+            return response.choices[0].text.strip()
+        corpus         = self.ask_gpt_adj.to_string(index = False)
+        openai.api_key = api_key
+        prompt         = query + ':\n\n' + f'{corpus}\n'
+        prompt         = prompt[:char_limit]
+        analyze        = query_chatgpt(prompt)
+        print('Number of Characters: ' + str(len(prompt)))
+        return analyze
+
+    # Function: Ask chatGPT about EDA Report 
+    def ask_chatgpt_eda(self, char_limit = 4097, api_key = 'your_api_key_here', query = 'give me insights about the following information'):
+        def query_chatgpt(prompt, model = 'text-davinci-003', n = 1):
+            response = openai.Completion.create(
+                                                engine      = model,
+                                                prompt      = prompt,
+                                                max_tokens  = 2000,
+                                                n           = n,
+                                                stop        = None,
+                                                temperature = 0.8
+                                                )
+            return response.choices[0].text.strip()
+        corpus         = self.ask_gpt_rt.to_string(index = False)    
+        lines          = corpus.split('\n')
+        corpus         = '\n'.join(' '.join(line.split()) for line in lines)
+        openai.api_key = api_key
+        prompt         = query + ':\n\n' + f'{corpus}\n'
+        prompt         = prompt[:char_limit]
+        analyze        = query_chatgpt(prompt)
+        print('Number of Characters: ' + str(len(prompt)))
+        return analyze
+    
+    # Function: Ask chatGPT about Evolution Plot
+    def ask_chatgpt_ep(self, char_limit = 4097, api_key = 'your_api_key_here', query = 'give me insights about the following information, related to words apperance by year'):
+        def query_chatgpt(prompt, model = 'text-davinci-003', n = 1):
+            response = openai.Completion.create(
+                                                engine      = model,
+                                                prompt      = prompt,
+                                                max_tokens  = 2000,
+                                                n           = n,
+                                                stop        = None,
+                                                temperature = 0.8
+                                                )
+            return response.choices[0].text.strip()
+        corpus         = self.ask_gpt_ep
+        openai.api_key = api_key
+        prompt         = query + ':\n\n' + f'{corpus}\n'
+        prompt         = prompt[:char_limit]
+        analyze        = query_chatgpt(prompt)
+        print('Number of Characters: ' + str(len(prompt)))
+        return analyze
+
+    # Function: Ask chatGPT about Citation Analysis 
+    def ask_chatgpt_hist(self, char_limit = 4097, api_key = 'your_api_key_here', query = 'give me insights about the following information relating the most influential references, also discover if there is relevant network connections'):
+        def query_chatgpt(prompt, model = 'text-davinci-003', n = 1):
+            response = openai.Completion.create(
+                                                engine      = model,
+                                                prompt      = prompt,
+                                                max_tokens  = 2000,
+                                                n           = n,
+                                                stop        = None,
+                                                temperature = 0.8
+                                                )
+            return response.choices[0].text.strip()
+        corpus = []
+        for i in range(0, self.ask_gpt_hist.shape[0]):
+            corpus.append('Paper ' + self.ask_gpt_hist.iloc[i,0] + ' Cites Paper ' + self.ask_gpt_hist.iloc[i,1])
+        corpus         = ', '.join(corpus)    
+        openai.api_key = api_key
+        prompt         = query + ':\n\n' + f'{corpus}\n'
+        prompt         = prompt[:char_limit]
+        analyze        = query_chatgpt(prompt)
+        print('Number of Characters: ' + str(len(prompt)))
+        return analyze
+
+    # Function: Ask chatGPT about Map Analysis 
+    def ask_chatgpt_map(self, char_limit = 4097, api_key = 'your_api_key_here', query = 'give me insights about the following information'):
+        def query_chatgpt(prompt, model = 'text-davinci-003', n = 1):
+            response = openai.Completion.create(
+                                                engine      = model,
+                                                prompt      = prompt,
+                                                max_tokens  = 2000,
+                                                n           = n,
+                                                stop        = None,
+                                                temperature = 0.8
+                                                )
+            return response.choices[0].text.strip()
+        corpus         = self.ask_gpt_map.to_string(index = False)
+        openai.api_key = api_key
+        prompt         = query + ':\n\n' + f'{corpus}\n'
+        prompt         = prompt[:char_limit]
+        analyze        = query_chatgpt(prompt)
+        print('Number of Characters: ' + str(len(prompt)))
+        return analyze
+
+    # Function: Ask chatGPT about N-Grms 
+    def ask_chatgpt_ngrams(self, char_limit = 4097, api_key = 'your_api_key_here', query = 'give me insights about the following information relating the n-grams and their frequency'):
+        def query_chatgpt(prompt, model = 'text-davinci-003', n = 1):
+            response = openai.Completion.create(
+                                                engine      = model,
+                                                prompt      = prompt,
+                                                max_tokens  = 2000,
+                                                n           = n,
+                                                stop        = None,
+                                                temperature = 0.8
+                                                )
+            return response.choices[0].text.strip()
+        corpus         = self.ask_gpt_ng.to_string(index = False)  
+        lines          = corpus.split('\n')
+        corpus         = '\n'.join(' '.join(line.split()) for line in lines)  
+        openai.api_key = api_key
+        prompt         = query + ':\n\n' + f'{corpus}\n'
+        prompt         = prompt[:char_limit]
+        analyze        = query_chatgpt(prompt)
+        print('Number of Characters: ' + str(len(prompt)))
+        return analyze
+
+    # Function: Ask chatGPT about Sankey Diagram
+    def ask_chatgpt_sankey(self, char_limit = 4097, api_key = 'your_api_key_here', query = 'give me insights about the following information from a network called Sankey'):
+        def query_chatgpt(prompt, model = 'text-davinci-003', n = 1):
+            response = openai.Completion.create(
+                                                engine      = model,
+                                                prompt      = prompt,
+                                                max_tokens  = 2000,
+                                                n           = n,
+                                                stop        = None,
+                                                temperature = 0.8
+                                                )
+            return response.choices[0].text.strip()
+        corpus         = self.ask_gpt_sk.to_string(index = False)   
+        lines          = corpus.split('\n')
+        corpus         = '\n'.join(' '.join(line.split()) for line in lines)
+        openai.api_key = api_key
+        prompt         = query + ':\n\n' + f'{corpus}\n'
+        prompt         = prompt[:char_limit]
+        analyze        = query_chatgpt(prompt)
+        print('Number of Characters: ' + str(len(prompt)))
+        return analyze
+
+    # Function: Ask chatGPT about Similarity Analysis 
+    def ask_chatgpt_sim(self, char_limit = 4097, api_key = 'your_api_key_here', query = 'give me insights about the following information'):
+        def query_chatgpt(prompt, model = 'text-davinci-003', n = 1):
+            response = openai.Completion.create(
+                                                engine      = model,
+                                                prompt      = prompt,
+                                                max_tokens  = 2000,
+                                                n           = n,
+                                                stop        = None,
+                                                temperature = 0.8
+                                                )
+            return response.choices[0].text.strip()
+        corpus         = self.ask_gpt_sim.to_string(index = False)
+        openai.api_key = api_key
+        prompt         = query + ':\n\n' + f'{corpus}\n'
+        prompt         = prompt[:char_limit]
+        analyze        = query_chatgpt(prompt)
+        print('Number of Characters: ' + str(len(prompt)))
+        return analyze
+
+    # Function: Ask chatGPT about Wordcloud 
+    def ask_chatgpt_wordcloud(self, char_limit = 4097, api_key = 'your_api_key_here', query = 'give me insights about the following information'):
+        def query_chatgpt(prompt, model = 'text-davinci-003', n = 1):
+            response = openai.Completion.create(
+                                                engine      = model,
+                                                prompt      = prompt,
+                                                max_tokens  = 2000,
+                                                n           = n,
+                                                stop        = None,
+                                                temperature = 0.8
+                                                )
+            return response.choices[0].text.strip()
+        corpus         = pd.DataFrame.from_dict(self.ask_gpt_wd, orient = 'index', columns = ['Frequency'])    
+        corpus         = corpus.reset_index().rename(columns = {'index': 'Word'})
+        corpus         = corpus.to_string(index = False)
+        lines          = corpus.split('\n')
+        corpus         = '\n'.join(' '.join(line.split()) for line in lines)
+        openai.api_key = api_key
+        prompt         = query + ':\n\n' + f'{corpus}\n'
+        prompt         = prompt[:char_limit]
+        analyze        = query_chatgpt(prompt)
+        print('Number of Characters: ' + str(len(prompt)))
+        return analyze
+
 ############################################################################
```

### Comparing `pyBibX-1.7.7/pyBibX/base/stws/Stopwords-Arabic.txt` & `pyBibX-2.9.0/pyBibX/base/stws/Stopwords-Arabic.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-1.7.7/pyBibX/base/stws/Stopwords-Bengali.txt` & `pyBibX-2.9.0/pyBibX/base/stws/Stopwords-Bengali.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-1.7.7/pyBibX/base/stws/Stopwords-Bulgarian.txt` & `pyBibX-2.9.0/pyBibX/base/stws/Stopwords-Bulgarian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-1.7.7/pyBibX/base/stws/Stopwords-Czech.txt` & `pyBibX-2.9.0/pyBibX/base/stws/Stopwords-Czech.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-1.7.7/pyBibX/base/stws/Stopwords-English.txt` & `pyBibX-2.9.0/pyBibX/base/stws/Stopwords-English.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-1.7.7/pyBibX/base/stws/Stopwords-Finnish.txt` & `pyBibX-2.9.0/pyBibX/base/stws/Stopwords-Finnish.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-1.7.7/pyBibX/base/stws/Stopwords-French.txt` & `pyBibX-2.9.0/pyBibX/base/stws/Stopwords-French.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-1.7.7/pyBibX/base/stws/Stopwords-German.txt` & `pyBibX-2.9.0/pyBibX/base/stws/Stopwords-German.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-1.7.7/pyBibX/base/stws/Stopwords-Hindi.txt` & `pyBibX-2.9.0/pyBibX/base/stws/Stopwords-Hindi.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-1.7.7/pyBibX/base/stws/Stopwords-Hungarian.txt` & `pyBibX-2.9.0/pyBibX/base/stws/Stopwords-Hungarian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-1.7.7/pyBibX/base/stws/Stopwords-Italian.txt` & `pyBibX-2.9.0/pyBibX/base/stws/Stopwords-Italian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-1.7.7/pyBibX/base/stws/Stopwords-Marathi.txt` & `pyBibX-2.9.0/pyBibX/base/stws/Stopwords-Marathi.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-1.7.7/pyBibX/base/stws/Stopwords-Persian.txt` & `pyBibX-2.9.0/pyBibX/base/stws/Stopwords-Persian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-1.7.7/pyBibX/base/stws/Stopwords-Polish.txt` & `pyBibX-2.9.0/pyBibX/base/stws/Stopwords-Polish.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-1.7.7/pyBibX/base/stws/Stopwords-Portuguese-br.txt` & `pyBibX-2.9.0/pyBibX/base/stws/Stopwords-Portuguese-br.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-1.7.7/pyBibX/base/stws/Stopwords-Romanian.txt` & `pyBibX-2.9.0/pyBibX/base/stws/Stopwords-Romanian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-1.7.7/pyBibX/base/stws/Stopwords-Russian.txt` & `pyBibX-2.9.0/pyBibX/base/stws/Stopwords-Russian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-1.7.7/pyBibX/base/stws/Stopwords-Spanish.txt` & `pyBibX-2.9.0/pyBibX/base/stws/Stopwords-Spanish.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-1.7.7/pyBibX/base/stws/Stopwords-Swedish.txt` & `pyBibX-2.9.0/pyBibX/base/stws/Stopwords-Swedish.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-1.7.7/pyBibX.egg-info/PKG-INFO` & `pyBibX-2.9.0/pyBibX.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,62 +1,63 @@
 Metadata-Version: 2.1
 Name: pyBibX
-Version: 1.7.7
+Version: 2.9.0
 Summary: A Bibliometric and Scientometric Library Powered with Artificial Intelligence Tools
 Home-page: https://github.com/Valdecy/pyBibX
 Author: Valdecy Pereira
 Author-email: valdecy.pereira@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyBibX
 
 ## Introduction
 
-A Bibliometric and Scientometric python library that uses the raw files generated by **Scopus** (.bib files), **WOS (Web of Science)** (.bib files) and **PubMed** (.txt files) scientific databases. Also Powered with Artificial Intelligence Tools to Analyze Text Data
+A Bibliometric and Scientometric python library that uses the raw files generated by **Scopus** (.bib files), **WOS (Web of Science)** (.bib files), and **PubMed** (.txt files) scientific databases. Also Powered with Artificial Intelligence Tools to Analyze Bibliometric Results and Text Data
 
 General Capabilities:
 - a) Works with **Scopus** (.bib files), **WOS** (.bib files) and **PubMed** (.txt files) databases 
 - b) Identification and Removal of duplicates
 - c) Identification of documents per type
 - d) Generates an **EDA (Exploratory Data Analysis)** Report: Publications Timespan, Total Number of Countries, Total Number of Institutions, Total Number of Sources, Total Number of References, Total Number of Languages (and also the number of docs for each language), Total Number of Documents, Average Documents per Author, Average Documents per Institution, Average Documents per Source, Average Documents per Year, Total Number of Authors, Total Number of Authors Keywords, Total Number of Authors Keywords Plus, Total Single-Authored Documents, Total Multi-Authored Documents, Average Collaboration Index, Max H-Index, Total Number of Citations, Average Citations per Author, Average Citations per Institution, Average Citations per Document, Average Citations per Source
 - e) Creates an **ID (Identification)** for each Document, Authors, Sources, Institutions, Countries, Authors' Keywords, Keywords Plus. The IDs can be used in graphs/plots to obtain a cleaner visualization
 - f) Creates a **WordCloud** from the Abstracts, Titles, Authors Keywords or Keywords Plus
 - g) Creates a **N-Gram Bar Plot (interactive plot)** from the Abstracts, Titles, Authors Keywords or Keywords Plus
 - h) Creates a **Projection (interactive plot)** of the documents based on the Abstracts, Titles, Authors Keywords or Keywords Plus
 - i) Creates an **Evolution Plot (interactive plot)** based on Abstracts, Titles, Sources, Authors Keywords or Keywords Plus
-- j) Creates a **Sankey Plot (interactive plot)** with any combination of the following keys: Authors, Countries, Institutions, Journals, Auhors_Keywords, Keywords_Plus, and/or Languages
+- j) Creates a **Sankey Diagram (interactive plot)** with any combination of the following keys: Authors, Countries, Institutions, Journals, Auhors_Keywords, Keywords_Plus, and/or Languages
 - k) Creates a **TreeMap** from the Authors, Countries, Institutions, Journals, Auhors_Keywords, or Keywords_Plus
 - l) Creates an **Authors Productivity Plot (interactive plot)** It informs for each year the documents (IDs) published for each author
 - m) Creates a **Bar Plot**  for the following statistics: Documents per Year, Citations per Year, Past Citations per Year, Lotka's Law, Sources per Documents, Sources per Citations, Authors per Documents, Authors per Citations, Authors per H-Index, Bradford's Law (Core Sources 1, 2 or 3), Institutions per Documents, Institutions per Citations, Countries per Documents, Countries per Citations, Language per Documents, Keywords Plus per Documents and Authors' Keywords per Documents
 
 Network Capabilities:
 - a) **Citation Analysis (interactive plot)** between Documents (Blue Nodes) and Citations (Red Nodes). Documents and Citations can be highlighted for better visualization
 - b) **Collaboration Analysis (interactive plot)** between Authors, Countries, Institutions or **Adjacency Analysis (interactive plot)** between Authors' Keywords or Keywords Plus. Collaboration and Adjacency can be highlighted for better visualization
 - c) **Similarity Analysis (interactive plot)** can be performed using coupling or cocitation methods
-- d) **World MAP Collaboration Analysis (interactive plot)** between Countries in a Map
+- d) **World Map Collaboration Analysis (interactive plot)** between Countries in a Map
 
 Artificial Intelligence Capabilities:
 - a) **Topic Modelling** using BERTopic to cluster documents by topic
 - b) Visualize topics distribution
 - c) Visualize topics by the most representative words
 - d) Visualize documents projection and clusterization by topic
 - e) Visualize topics heatmap
 - f) Find the most representative documents from each topic
 - g) Find the most representative topics according to a word
 - h) Creates **Embeddings** from Abstracts, Titles, Authors Keywords or Keywords Plus
 - i) **Abstractive Text Summarization** using **PEGASUS** on a set of selected documents or all documents
 - j) **Abstractive Text Summarization** using **chatGPT** on a set of selected documents or all documents. Requires the user to have an **API key** (https://platform.openai.com/account/api-keys)
 - k) **Extractive Text Summarization** using **BERT** on a set of selected documents or all documents
+- l) **Ask chatGPT to Analyze Results** available for: EDA Report, WordCloud, N-Grams, Evolution Plot, Sankey Diagram, Authors Productivity Plot, Bar Plots, Citation Analysis, Collaboration Analysis, Similarity Analysis, and World Map Collaboration Analysis (see Example 08). Requires the user to have an **API key** (https://platform.openai.com/account/api-keys)
 
 Correction and Manipulation Capabilities:
 - a) Filter the .bib or .txt file by Year, Sources, Bradford Law Cores, Countries, Languages and/or Abstracts (Documents with Abstracts)
 - b) Merge Authors, Institutions, Countries, Languages and/or Sources that have multiple entries 
-- c) Merge different or same database files one at a time. The preference of information preservation is given to the old database, so the order of merging matters (see Examples 04 and 05)
+- c) Merge different or the same database files one at a time. The preference for information preservation is given to the old database, so the order of merging matters (see Examples 04 and 05)
 
 ## Usage
 
 1. Install
 ```bash
 pip install pyBibX
 ```
@@ -66,14 +67,15 @@
 - Example 01: Scopus                ([ Colab Demo ](https://colab.research.google.com/drive/1yHiMMZIKa-RrarXbPB9ca0gLN9YvvtPU?usp=sharing))
 - Example 02: WOS                   ([ Colab Demo ](https://colab.research.google.com/drive/13HLjC4myTvYcjLk2XBTZKbWJ2aqZUST1?usp=sharing))
 - Example 03: PubMed                ([ Colab Demo ](https://colab.research.google.com/drive/13CU-KvZMnazga1BmQf2J8wYM9mhHL2e1?usp=sharing))
 - Example 04: Scopus + WOS          ([ Colab Demo ](https://colab.research.google.com/drive/1DqEk0_IakJPfIZDVcnTWBE_nxyhW9p-W?usp=sharing))
 - Example 05: WOS + Scopus          ([ Colab Demo ](https://colab.research.google.com/drive/12k_IOcSDwumbEtPqqSMbCIE6ZypgKAJn?usp=sharing))
 - Example 06: Scopus + WOS + Pubmed ([ Colab Demo ](https://colab.research.google.com/drive/1Ko6AibkXtB_Kwg3Eu0fhzNMVEIXPkbez?usp=sharing))
 - Example 07: Your Own              ([ Colab Demo ](https://colab.research.google.com/drive/19EYjgal9V1kemmzpHnyp6MSlk9S-kGHT?usp=sharing))
+- Example 08: Ask chatGPT Analysis  ([ Colab Demo ](https://colab.research.google.com/drive/1LMrR49F54MuX-stlrQbrrjX_dEU3kZ8Y?usp=sharing))
 
 # Acknowledgement 
 This section indicates the libraries that inspired pyBibX
 
 * BERT (https://smrzr.io/)
 - a) Github: https://github.com/dmmiller612/bert-extractive-summarizer
 - b) Paper: DEREK, M. (2019). Leveraging BERT for Extractive Text Summarization on Lectures. arXiv. doi: https://doi.org/10.48550/arXiv.1906.04165
@@ -82,14 +84,18 @@
 - a) Github: https://github.com/MaartenGr/BERTopic
 - b) Paper: GROOTENDORST, M. (2022). BERTopic: Neural Topic Modeling with a Class-based TF-IDF Procedure. arXiv. doi: https://doi.org/10.48550/arXiv.2203.05794
 
 * Bibliometrix (https://www.bibliometrix.org/home/)
 - a) Github: https://github.com/massimoaria/bibliometrix
 - b) Paper: ARIA, M.; CUCCURULLO, C. (2017). Bibliometrix: An R-tool for Comprehensive Science Mapping Analysis. Journal of informetrics, 11(4), 959-975. doi: https://doi.org/10.1016/j.joi.2017.08.007
 
+* chatGPT (https://chat.openai.com/chat)
+- a) Github: https://github.com/openai
+- b) Paper: ECOFFET, A. (2023). GPT-4 Technical Report. arXiv. doi: https://doi.org/10.48550/arXiv.2303.08774
+
 * Metaknowledge (http://www.networkslab.org/metaknowledge)
 - a) Github: https://github.com/UWNETLAB/metaknowledge
 - b) Paper: McILROY-YOUNG, R.; McLEVEY, J.; ANDERSON, J. (2015). Metaknowledge: Open Source Software for Social Networks, Bibliometrics, and Sociology of Knowledge Research.
 
 * SentenceTransformers (https://www.sbert.net/)
 - a) Github: https://github.com/UKPLab/sentence-transformers
 - b) Paper: REIMERS, N.; GUREVYCH, I. (2019). Sentence-BERT: Sentence Embeddings using Siamese BERT-Networks. arXiv. doi: https://arxiv.org/abs/1908.10084
```

### Comparing `pyBibX-1.7.7/pyBibX.egg-info/SOURCES.txt` & `pyBibX-2.9.0/pyBibX.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-1.7.7/setup.py` & `pyBibX-2.9.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name='pyBibX',
-    version='1.7.7',
+    version='2.9.0',
     license='GNU',
     author='Valdecy Pereira',
     author_email='valdecy.pereira@gmail.com',
     url='https://github.com/Valdecy/pyBibX',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
```

