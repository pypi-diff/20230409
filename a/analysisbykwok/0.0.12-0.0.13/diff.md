# Comparing `tmp/analysisbykwok-0.0.12.tar.gz` & `tmp/analysisbykwok-0.0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "analysisbykwok-0.0.12.tar", last modified: Mon Apr  3 14:41:59 2023, max compression
+gzip compressed data, was "analysisbykwok-0.0.13.tar", last modified: Sun Apr  9 02:54:44 2023, max compression
```

## Comparing `analysisbykwok-0.0.12.tar` & `analysisbykwok-0.0.13.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-03 14:41:59.495183 analysisbykwok-0.0.12/
--rw-rw-rw-   0        0        0       62 2023-04-03 14:41:59.495183 analysisbykwok-0.0.12/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-03 14:41:59.415756 analysisbykwok-0.0.12/analysisbykwok/
--rw-rw-rw-   0        0        0     8867 2023-04-03 14:40:59.000000 analysisbykwok-0.0.12/analysisbykwok/__init__.py
--rw-rw-rw-   0        0        0       23 2023-04-03 14:40:06.000000 analysisbykwok-0.0.12/analysisbykwok/_version.py
-drwxrwxrwx   0        0        0        0 2023-04-03 14:41:59.479558 analysisbykwok-0.0.12/analysisbykwok.egg-info/
--rw-rw-rw-   0        0        0       62 2023-04-03 14:41:59.000000 analysisbykwok-0.0.12/analysisbykwok.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      220 2023-04-03 14:41:59.000000 analysisbykwok-0.0.12/analysisbykwok.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-03 14:41:59.000000 analysisbykwok-0.0.12/analysisbykwok.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-04-03 14:41:59.000000 analysisbykwok-0.0.12/analysisbykwok.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       70 2023-04-03 14:39:58.000000 analysisbykwok-0.0.12/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-03 14:41:59.495183 analysisbykwok-0.0.12/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-09 02:54:44.494120 analysisbykwok-0.0.13/
+-rw-rw-rw-   0        0        0       62 2023-04-09 02:54:44.494120 analysisbykwok-0.0.13/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-09 02:54:44.478527 analysisbykwok-0.0.13/analysisbykwok/
+-rw-rw-rw-   0        0        0     9472 2023-04-09 02:54:24.000000 analysisbykwok-0.0.13/analysisbykwok/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-04-09 02:53:13.000000 analysisbykwok-0.0.13/analysisbykwok/_version.py
+drwxrwxrwx   0        0        0        0 2023-04-09 02:54:44.494120 analysisbykwok-0.0.13/analysisbykwok.egg-info/
+-rw-rw-rw-   0        0        0       62 2023-04-09 02:54:44.000000 analysisbykwok-0.0.13/analysisbykwok.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      220 2023-04-09 02:54:44.000000 analysisbykwok-0.0.13/analysisbykwok.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 02:54:44.000000 analysisbykwok-0.0.13/analysisbykwok.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-04-09 02:54:44.000000 analysisbykwok-0.0.13/analysisbykwok.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       70 2023-04-09 02:53:13.000000 analysisbykwok-0.0.13/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-09 02:54:44.494120 analysisbykwok-0.0.13/setup.cfg
```

### Comparing `analysisbykwok-0.0.12/analysisbykwok/__init__.py` & `analysisbykwok-0.0.13/analysisbykwok/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import pandas as pd
 import requests
 import random
 import execjs
 import json
+import os.path
+from zipfile import ZipFile
+import zipfile
 import os
 if not os.path.exists(
         r'C:\Windows\AgentPool.xlsx'):
     input('注意注意！\n请确保存在\'C:\Windows\AgentPool.xlsx\'的ip代理文件\n否则，ip池功能将无法使用\n继续使用请敲击回车键')
 class info():
     def show():
         print('测试成功，可以使用')
@@ -62,17 +65,18 @@
                     continue
     def GetIpPool():
         IpPool = []
         data = pd.read_excel(r'C:\Windows\AgentPool.xlsx')
         data = data.values.T.tolist()
         ip = data[0]
         port = data[1]
+        type=data[2]
         for i in range(0, len(ip)):
             list = {}
-            list[str(ip[i]).replace(' ', '')] = str(port[i]).replace(' ', '')
+            list[str(type[i])] = str(type[i])+'://'+str(ip[i]).replace(' ', '')+':'+str(port[i]).replace(' ', '')
             IpPool.append(list)
         return IpPool
     def GetCityNumFromBossZhiPing(city):
         ip = function.GetIpPool()
         ip = ip[random.randint(0, len(ip))]
         city=(city.split('省')[1]).split('市')[0]
         print('boss直聘查询说明\n本功能只能通过城市名字查询一个，关键词例如(宁波)，返回结果不是区的字典，只是当前城市代码。\n正在查询Boss的城市代码')
@@ -157,23 +161,33 @@
             else:
                 data = requests.post(url, data=data, headers=header)
             res = data
             res.encoding = 'utf-8'
             res=res.json()
             print(ip,res)
         get_data('070030','070030010','数据',0,ip,'温州')
-class dealDate():
-    def MergeSimilar(dir, names):
-        os.chdir(dir)
-        data = pd.DataFrame()
-        na = []
-        num = 1
-        for name in os.listdir():
-            url = os.path.join(dir, name)
-            data = pd.concat([data, pd.read_excel(url)])
-            print(url, len(pd.read_excel(url)))
-            for i in range(len(pd.read_excel(url))):
-                na.append(name)
-            num = num + 1
-        del (data['Unnamed: 0'])
-        data.insert(1, column='文件名', value=na)
-        data.to_excel(names)
+    def CheckIp(ip):
+        try:
+            if str(ip)[2:7] != 'https':
+                res = requests.get('http://httpbin.org/ip', proxies=ip)
+                result = '可以'
+            else:
+                res = requests.get('https://blog.sina.com.cn/', proxies=ip)
+                result = '可以'
+        except:
+            result = '不行'
+        return result
+    def IntoZip(dir_):
+        with ZipFile(str(dir_) + '.zip', 'w') as z:
+            z.write(dir_, arcname=(dn := os.path.basename(dir_)))
+            for root, dirs, files in os.walk(dir_):
+                for fn in files:
+                    z.write(
+                        fp := os.path.join(root, fn),
+                        arcname=dn + '/' + os.path.relpath(fp, dir_)
+                    )
+        print('压缩成功，已经压缩到了文件夹:' + str(dir_) + '.zip')
+    def ZipOut(dir, out):
+        zf = zipfile.ZipFile(dir)
+        os.chdir(out)
+        ret = zf.extractall(path=out)  # 解压到指定目录
+        print('解压成功')
```

