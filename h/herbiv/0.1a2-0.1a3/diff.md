# Comparing `tmp/herbiv-0.1a2.tar.gz` & `tmp/herbiv-0.1a3.tar.gz`

## Comparing `herbiv-0.1a2.tar` & `herbiv-0.1a3.tar`

### file list

```diff
@@ -1,17 +1,14 @@
--rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 herbiv-0.1a2/setup.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 herbiv-0.1a2/src/herbiv/__init__.py
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 herbiv-0.1a2/src/herbiv/analysis.py
--rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 herbiv-0.1a2/src/herbiv/chemical.py
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 herbiv-0.1a2/src/herbiv/chemical_protein.py
--rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 herbiv-0.1a2/src/herbiv/output.py
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 herbiv-0.1a2/src/herbiv/tcm.py
--rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 herbiv-0.1a2/src/herbiv/tcm_chemical.py
--rw-r--r--   0        0        0 13073523 2020-02-02 00:00:00.000000 herbiv-0.1a2/src/herbiv/data/HerbiV_chemical_protein_links.csv
--rw-r--r--   0        0        0 12622713 2020-02-02 00:00:00.000000 herbiv-0.1a2/src/herbiv/data/HerbiV_chemical_protein_links_pre.csv
--rw-r--r--   0        0        0  1377866 2020-02-02 00:00:00.000000 herbiv-0.1a2/src/herbiv/data/HerbiV_chemicals.csv
--rw-r--r--   0        0        0  1227198 2020-02-02 00:00:00.000000 herbiv-0.1a2/src/herbiv/data/HerbiV_tcm.csv
--rw-r--r--   0        0        0  1029771 2020-02-02 00:00:00.000000 herbiv-0.1a2/src/herbiv/data/HerbiV_tcm_chemical_links.csv
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 herbiv-0.1a2/LICENSE
--rw-r--r--   0        0        0     4890 2020-02-02 00:00:00.000000 herbiv-0.1a2/README.md
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 herbiv-0.1a2/pyproject.toml
--rw-r--r--   0        0        0     5937 2020-02-02 00:00:00.000000 herbiv-0.1a2/PKG-INFO
+-rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 herbiv-0.1a3/setup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 herbiv-0.1a3/src/herbiv/__init__.py
+-rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 herbiv-0.1a3/src/herbiv/analysis.py
+-rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 herbiv-0.1a3/src/herbiv/compute.py
+-rw-r--r--   0        0        0     4725 2020-02-02 00:00:00.000000 herbiv-0.1a3/src/herbiv/get.py
+-rw-r--r--   0        0        0     3263 2020-02-02 00:00:00.000000 herbiv-0.1a3/src/herbiv/output.py
+-rw-r--r--   0        0        0 13073523 2020-02-02 00:00:00.000000 herbiv-0.1a3/src/herbiv/data/HerbiV_chemical_protein_links.csv
+-rw-r--r--   0        0        0  1377866 2020-02-02 00:00:00.000000 herbiv-0.1a3/src/herbiv/data/HerbiV_chemicals.csv
+-rw-r--r--   0        0        0  1227198 2020-02-02 00:00:00.000000 herbiv-0.1a3/src/herbiv/data/HerbiV_tcm.csv
+-rw-r--r--   0        0        0  1029771 2020-02-02 00:00:00.000000 herbiv-0.1a3/src/herbiv/data/HerbiV_tcm_chemical_links.csv
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 herbiv-0.1a3/LICENSE
+-rw-r--r--   0        0        0     6957 2020-02-02 00:00:00.000000 herbiv-0.1a3/README.md
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 herbiv-0.1a3/pyproject.toml
+-rw-r--r--   0        0        0     7980 2020-02-02 00:00:00.000000 herbiv-0.1a3/PKG-INFO
```

### Comparing `herbiv-0.1a2/setup.py` & `herbiv-0.1a3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 here = pathlib.Path(__file__).parent.resolve()
 
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="herbiv",
-    version="0.1a2",
+    version="0.1a3",
     description="HerbiV是一个具有多种功能的中药网络药理学分析工具，可进行经典的网络药理学及反向网络药理学分析。HerbiV is a multi-functional traditional chinese medicine network pharmacology analysis tool for classical network pharmacology and reverse network pharmacology.",
     # Optional
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/MLi-lab-Bioinformatics-NJUCM/HerbiV",
     author="王皓阳",
     author_email="Wesady@qq.com",
@@ -27,15 +27,16 @@
         "Topic :: Scientific/Engineering :: Bio-Informatics",
         "Topic :: Scientific/Engineering :: Information Analysis"
     ],
     keywords="network pharmacology",
     package_dir={"": "src"},
     packages=find_packages(where="src"),
     python_requires=">=3.8",
-    install_requires=["numpy",
+    install_requires=[
+                      "numpy",
                       "pandas",
                       ],
     project_urls={
-        "Bug Reports": "https://github.com/MLi-lab-Bioinformatics-NJUCM/HerbiV/issues",
-        "Source": "https://github.com/MLi-lab-Bioinformatics-NJUCM/HerbiV",
+        "Bug Reports": "https://github.com/MLi-lab-Bioinformatics-NJUCM/pharmastar/issues",
+        "Source": "https://github.com/MLi-lab-Bioinformatics-NJUCM/pharmastar",
     },
 )
```

### Comparing `herbiv-0.1a2/src/herbiv/chemical_protein.py` & `herbiv-0.1a3/src/herbiv/analysis.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,53 @@
-import os
-import pandas as pd
+from . import get
+from . import compute
+from . import output
 
 
-def get_chem_protein_links(genes,
-                           score=900,
-                           save=True):
+def from_tcm(tcm,
+             score=900,
+             re=True):
     r"""
-    读取HerbiV_chemical_protein_links数据集，返回包含目标基因且combined_score大于等于score的记录
+    进行逆向网络药理学分析
+    :param tcm: 列表类型，拟分析的中药的中文名称
+    :param score: int类型，仅combined_score大于等于score的记录会被筛选出
+    :param re: 布尔类型，是否返回原始分析结果
+    :return: tcm: pd.DataFrame类型，中药信息
+    :return: tcm_chem_links: pd.DataFrame类型，中药-成分信息
+    :return: chem_protein_links: pd.DataFrame类型，化合物-蛋白质（靶点）信息
+    """
+
+    tcm = get.get_tcm('cn_name', tcm)
+    tcm_chem_links = get.get_tcm_chem_links('HVMID', tcm['HVMID'])
+    chem = get.get_chemicals('HVCID', tcm_chem_links['HVCID'])
+    chem_protein_links = get.get_chem_protein_links('HVCID', chem['HVCID'], score)
+
+    if re:
+        return tcm, tcm_chem_links, chem_protein_links
+
+
+def from_genes(genes,
+               score=900,
+               out_for_cytoscape=True,
+               re=True,
+               path='result/'):
+    r"""
+    进行逆向网络药理学分析
     :param genes: 字典类型，存储拟分析蛋白（基因）在STITCH中的ID与其名称的对应关系
     :param score: int类型，仅combined_score大于等于score的记录会被筛选出
-    :param save: 布尔类型，是否保存原始分析结果
-    :return: chem_protein_links: pd.DataFrame类型，HerbiV_chemical_protein_links数据集数据集中包含目标基因且Combined_score大于等于score的记录
+    :param out_for_cytoscape: 布尔类型，是否输出用于Cytoscape绘图的文件
+    :param re: 布尔类型，是否返回原始分析结果
+    :param path: 字符串类型，存放结果的目录
+    :return: tcm: pd.DataFrame类型，中药信息
+    :return: tcm_chem_links: pd.DataFrame类型，中药-成分信息
     """
+    chem_protein_links = get.get_chem_protein_links('Ensembl_ID', genes, score)
+    chem = get.get_chemicals('HVCID', chem_protein_links['HVCID'])
+    tcm_chem_links = get.get_tcm_chem_links('HVCID', chem['HVCID'])
+    tcm = get.get_tcm('HVMID', tcm_chem_links['HVMID'])
+    chem, tcm = compute.score(chem_protein_links, chem, tcm_chem_links, tcm)
 
-    # 读取数据集
-    current_directory = os.path.dirname(os.path.abspath(__file__))
-    chem_protein_links_all = pd.read_csv(current_directory + r'/data/HerbiV_chemical_protein_links.csv')
-
-    # 选取HerbiV_chemical_protein_links数据集中Ensembl_ID为拟分析蛋白（基因）的ID、combined_score大于等于score的记录
-    chem_protein_links = chem_protein_links_all.loc[
-        (chem_protein_links_all['Ensembl_ID'].isin(genes)) &
-        (chem_protein_links_all['Combined_score'] >= score)].copy()
-
-    # 将Combined_score变换为0-1的浮点数
-    chem_protein_links.loc[:, 'Combined_score'] = chem_protein_links.loc[:, 'Combined_score'].apply(
-        lambda x: x / 1000)
-
-    # 重新设置索引
-    chem_protein_links.index = range(chem_protein_links.shape[0])
-
-    # 保存结果
-    if save:
-        chem_protein_links.to_csv('result/chemical_protein_links.csv', index=False)
+    if out_for_cytoscape:
+        output.out_for_cyto(chem_protein_links, chem, genes, tcm_chem_links, tcm, path)
 
-    return chem_protein_links
+    if re:
+        return tcm, tcm_chem_links, chem_protein_links
```

### Comparing `herbiv-0.1a2/src/herbiv/data/HerbiV_chemical_protein_links.csv` & `herbiv-0.1a3/src/herbiv/data/HerbiV_chemical_protein_links.csv`

 * *Files identical despite different names*

### Comparing `herbiv-0.1a2/src/herbiv/data/HerbiV_chemicals.csv` & `herbiv-0.1a3/src/herbiv/data/HerbiV_chemicals.csv`

 * *Files identical despite different names*

### Comparing `herbiv-0.1a2/src/herbiv/data/HerbiV_tcm.csv` & `herbiv-0.1a3/src/herbiv/data/HerbiV_tcm.csv`

 * *Files identical despite different names*

### Comparing `herbiv-0.1a2/src/herbiv/data/HerbiV_tcm_chemical_links.csv` & `herbiv-0.1a3/src/herbiv/data/HerbiV_tcm_chemical_links.csv`

 * *Files identical despite different names*

### Comparing `herbiv-0.1a2/LICENSE` & `herbiv-0.1a3/LICENSE`

 * *Files identical despite different names*

### Comparing `herbiv-0.1a2/pyproject.toml` & `herbiv-0.1a3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 [build-system]
 requires = [
     "hatchling",
+    "numpy",
+    "pandas",
     "typing-extensions",
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "herbiv"
-version = "0.1a2"
+version = "0.1a3"
 authors = [
   { name="王皓阳", email="Wesady@qq.com" },
 ]
-description = "HerbiV是一个具有多种功能的中药网络药理学分析工具，可进行经典的网络药理学及反向网络药理学分析。HerbiV is a multi-functional traditional chinese medicine network pharmacology analysis tool for classical network pharmacology and reverse network pharmacology."
+description = "药理大师是一个具有多种功能的中药网络药理学分析工具，可进行经典的网络药理学及反向网络药理学分析。Pharmastar is a multi-functional traditional chinese medicine network pharmacology analysis tool for classical network pharmacology and reverse network pharmacology."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Development Status :: 3 - Alpha",
@@ -24,9 +26,9 @@
     "Natural Language :: Chinese (Simplified)",
     "Natural Language :: English",
     "Topic :: Scientific/Engineering :: Bio-Informatics",
     "Topic :: Scientific/Engineering :: Information Analysis"
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/MLi-lab-Bioinformatics-NJUCM/HerbiV"
-"Bug Tracker" = "https://github.com/MLi-lab-Bioinformatics-NJUCM/HerbiV/issues"
+"Homepage" = "https://github.com/MLi-lab-Bioinformatics-NJUCM/pharmastar"
+"Bug Tracker" = "https://github.com/MLi-lab-Bioinformatics-NJUCM/pharmastar/issues"
```

