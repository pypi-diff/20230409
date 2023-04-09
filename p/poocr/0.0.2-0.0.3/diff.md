# Comparing `tmp/poocr-0.0.2.tar.gz` & `tmp/poocr-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poocr-0.0.2.tar", last modified: Sat Mar 25 21:03:46 2023, max compression
+gzip compressed data, was "poocr-0.0.3.tar", last modified: Sun Apr  9 13:57:08 2023, max compression
```

## Comparing `poocr-0.0.2.tar` & `poocr-0.0.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-03-25 21:03:46.934677 poocr-0.0.2/
--rw-rw-rw-   0        0        0     1093 2022-09-13 01:21:27.000000 poocr-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     4589 2023-03-25 21:03:46.934677 poocr-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     4068 2023-03-06 15:25:33.000000 poocr-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-03-25 21:03:46.770926 poocr-0.0.2/poocr/
--rw-rw-rw-   0        0        0      523 2023-03-25 11:20:01.000000 poocr-0.0.2/poocr/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-25 21:03:46.844387 poocr-0.0.2/poocr/api/
--rw-rw-rw-   0        0        0      265 2023-03-25 11:08:27.000000 poocr-0.0.2/poocr/api/__init__.py
--rw-rw-rw-   0        0        0    20975 2023-01-30 12:39:04.000000 poocr-0.0.2/poocr/api/ocr.py
--rw-rw-rw-   0        0        0     9622 2023-03-25 19:51:41.000000 poocr-0.0.2/poocr/api/ocr2excel.py
-drwxrwxrwx   0        0        0        0 2023-03-25 21:03:46.869004 poocr-0.0.2/poocr/core/
--rw-rw-rw-   0        0        0     4071 2023-01-30 12:39:04.000000 poocr-0.0.2/poocr/core/OCR.py
--rw-rw-rw-   0        0        0      223 2023-01-22 06:56:13.000000 poocr-0.0.2/poocr/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-25 21:03:46.913621 poocr-0.0.2/poocr/lib/
--rw-rw-rw-   0        0        0     1017 2023-01-28 13:49:56.000000 poocr-0.0.2/poocr/lib/CommonUtils.py
--rw-rw-rw-   0        0        0     1132 2023-01-30 12:39:04.000000 poocr-0.0.2/poocr/lib/Config.py
--rw-rw-rw-   0        0        0      852 2023-01-30 12:39:04.000000 poocr-0.0.2/poocr/lib/Const.py
--rw-rw-rw-   0        0        0        0 2023-01-22 10:20:33.000000 poocr-0.0.2/poocr/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-25 21:03:46.807019 poocr-0.0.2/poocr.egg-info/
--rw-rw-rw-   0        0        0     4589 2023-03-25 21:03:46.000000 poocr-0.0.2/poocr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      455 2023-03-25 21:03:46.000000 poocr-0.0.2/poocr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-25 21:03:46.000000 poocr-0.0.2/poocr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-25 19:50:00.000000 poocr-0.0.2/poocr.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       29 2023-03-25 21:03:46.000000 poocr-0.0.2/poocr.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-03-25 21:03:46.000000 poocr-0.0.2/poocr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      719 2023-03-25 21:03:46.937678 poocr-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      389 2022-10-23 08:47:10.000000 poocr-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-25 21:03:46.932675 poocr-0.0.2/tests/
--rw-rw-rw-   0        0        0      181 2023-01-30 12:39:04.000000 poocr-0.0.2/tests/__init__.py
--rw-rw-rw-   0        0        0      380 2023-03-25 10:09:36.000000 poocr-0.0.2/tests/test_tencent.py
+drwxrwxrwx   0        0        0        0 2023-04-09 13:57:08.378192 poocr-0.0.3/
+-rw-rw-rw-   0        0        0     1093 2022-09-13 01:21:27.000000 poocr-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     4588 2023-04-09 13:57:08.378192 poocr-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4067 2023-04-02 05:09:27.000000 poocr-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-09 13:57:08.241899 poocr-0.0.3/poocr/
+-rw-rw-rw-   0        0        0      523 2023-03-25 11:20:01.000000 poocr-0.0.3/poocr/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-09 13:57:08.291442 poocr-0.0.3/poocr/api/
+-rw-rw-rw-   0        0        0      265 2023-03-25 11:08:27.000000 poocr-0.0.3/poocr/api/__init__.py
+-rw-rw-rw-   0        0        0    20975 2023-01-30 12:39:04.000000 poocr-0.0.3/poocr/api/ocr.py
+-rw-rw-rw-   0        0        0     9854 2023-04-09 13:56:17.000000 poocr-0.0.3/poocr/api/ocr2excel.py
+drwxrwxrwx   0        0        0        0 2023-04-09 13:57:08.300441 poocr-0.0.3/poocr/core/
+-rw-rw-rw-   0        0        0     4071 2023-01-30 12:39:04.000000 poocr-0.0.3/poocr/core/OCR.py
+-rw-rw-rw-   0        0        0      223 2023-01-22 06:56:13.000000 poocr-0.0.3/poocr/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-09 13:57:08.354573 poocr-0.0.3/poocr/lib/
+-rw-rw-rw-   0        0        0     1017 2023-01-28 13:49:56.000000 poocr-0.0.3/poocr/lib/CommonUtils.py
+-rw-rw-rw-   0        0        0     1132 2023-01-30 12:39:04.000000 poocr-0.0.3/poocr/lib/Config.py
+-rw-rw-rw-   0        0        0      852 2023-01-30 12:39:04.000000 poocr-0.0.3/poocr/lib/Const.py
+-rw-rw-rw-   0        0        0        0 2023-01-22 10:20:33.000000 poocr-0.0.3/poocr/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-09 13:57:08.282447 poocr-0.0.3/poocr.egg-info/
+-rw-rw-rw-   0        0        0     4588 2023-04-09 13:57:08.000000 poocr-0.0.3/poocr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      455 2023-04-09 13:57:08.000000 poocr-0.0.3/poocr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 13:57:08.000000 poocr-0.0.3/poocr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-09 13:57:08.000000 poocr-0.0.3/poocr.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       40 2023-04-09 13:57:08.000000 poocr-0.0.3/poocr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-09 13:57:08.000000 poocr-0.0.3/poocr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      732 2023-04-09 13:57:08.381190 poocr-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      389 2022-10-23 08:47:10.000000 poocr-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 13:57:08.376191 poocr-0.0.3/tests/
+-rw-rw-rw-   0        0        0      181 2023-01-30 12:39:04.000000 poocr-0.0.3/tests/__init__.py
+-rw-rw-rw-   0        0        0      704 2023-04-09 12:49:12.000000 poocr-0.0.3/tests/test_tencent.py
```

### Comparing `poocr-0.0.2/LICENSE` & `poocr-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `poocr-0.0.2/PKG-INFO` & `poocr-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poocr
-Version: 0.0.2
+Version: 0.0.3
 Summary: pip install poocr
 Home-page: https://www.python-office.com/
 Author: CoderWanFeng
 Author-email: 1957875073@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CoderWanFeng/poocr/issues
 Project-URL: Documentation, https://github.com/CoderWanFeng/poocr/blob/main/README.md
@@ -56,15 +56,15 @@
 -------------------------------------------------------------------------------
 
 ## 📦安装
 
 ### 🍊pip 自动下载&更新
 
 ```
-pip install -i https://pypi.tuna.tsinghua.edu.cn/simple poocr -U
+pip install -i https://mirrors.aliyun.com/pypi/simple/ poocr -U
 ```
 
 
 -------------------------------------------------------------------------------
 
 ## 📝功能
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: poocr Version: 0.0.2 Summary: pip install poocr
+Metadata-Version: 2.1 Name: poocr Version: 0.0.3 Summary: pip install poocr
 Home-page: https://www.python-office.com/ Author: CoderWanFeng Author-email:
 1957875073@qq.com License: MIT Project-URL: Bug Tracker, https://github.com/
 CoderWanFeng/poocr/issues Project-URL: Documentation, https://github.com/
 CoderWanFeng/poocr/blob/main/README.md Project-URL: Source Code, https://
 github.com/CoderWanFeng/poocr Platform: any Requires-Python: >=3.7 Description-
 Content-Type: text/markdown License-File: LICENSE
 [https://website-python-1300615378.cos.ap-nanjing.myqcloud.com/ads%2F1040x100-
@@ -13,16 +13,16 @@
        badge/%E5%BE%AE%E4%BF%A1-%E4%BA%A4%E6%B5%81%E7%BE%A4-brightgreen]
 ------------------------------------------------------------------------------
 - ## ðç®ä» poocr æ¯å¿«éè°ç¨è¾è®¯äºAIå¹³å°åè½çæ¥å£åéã
 ``poocr``ææåè½çå®ç°ï¼é½ä¾æäºè¾è®¯äºçæå­è¯å«ï¼å¦ææ¯å°ç½ç¨æ·ï¼å¯ä»¥**æ«ç ä¸å¾ï¼åè´¹å¼é**~
 ![](https://article-1300615378.cos.ap-nanjing.myqcloud.com/poocr%2Fapi-
 doc%2Fshare.jpg) --------------------------------------------------------------
 ----------------- ## ð¦å®è£ ### ðpip èªå¨ä¸è½½&æ´æ° ``` pip install
--i https://pypi.tuna.tsinghua.edu.cn/simple poocr -U ``` ----------------------
---------------------------------------------------------- ## ðåè½
+-i https://mirrors.aliyun.com/pypi/simple/ poocr -U ``` -----------------------
+-------------------------------------------------------- ## ðåè½
 [ðå®ç½ï¼https://www.python-office.com/](https://www.python-office.com/
 ) ## ð»ææåè½çåè¡¨ð[ç¹æç´è¾¾](https://mp.weixin.qq.com/s/
 WxICBZZSgkm-OrvXB82hbg) ## ðï¸æ·»ç å ç¦ ### ðPRçå»ºè®® python-
 officeæ¬¢è¿ä»»ä½äººæ¥æ·»ç å ç¦ï¼è´¡ç®ä»£ç ï¼å»ºè®®æäº¤çprï¼pull
 requestï¼ç¬¦åä¸äºè§èï¼è§èå¦ä¸ï¼ åä¸é¡¹ç®å»ºè®¾çæ­¥éª¤ï¼ -
 ä¾å¦ï¼ä½ éè¦ç»python-officeæ·»å ä¸ä¸ªaddæ¹æ³ã 1.
 ä½ çGithubè´¦æ·åä¸ºï¼demo 2. äºæ¯ä½ å¨./
```

### Comparing `poocr-0.0.2/README.md` & `poocr-0.0.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 -------------------------------------------------------------------------------
 
 ## 📦安装
 
 ### 🍊pip 自动下载&更新
 
 ```
-pip install -i https://pypi.tuna.tsinghua.edu.cn/simple poocr -U
+pip install -i https://mirrors.aliyun.com/pypi/simple/ poocr -U
 ```
 
 
 -------------------------------------------------------------------------------
 
 ## 📝功能
```

#### html2text {}

```diff
@@ -6,16 +6,16 @@
        badge/%E5%BE%AE%E4%BF%A1-%E4%BA%A4%E6%B5%81%E7%BE%A4-brightgreen]
 ------------------------------------------------------------------------------
 - ## ðç®ä» poocr æ¯å¿«éè°ç¨è¾è®¯äºAIå¹³å°åè½çæ¥å£åéã
 ``poocr``ææåè½çå®ç°ï¼é½ä¾æäºè¾è®¯äºçæå­è¯å«ï¼å¦ææ¯å°ç½ç¨æ·ï¼å¯ä»¥**æ«ç ä¸å¾ï¼åè´¹å¼é**~
 ![](https://article-1300615378.cos.ap-nanjing.myqcloud.com/poocr%2Fapi-
 doc%2Fshare.jpg) --------------------------------------------------------------
 ----------------- ## ð¦å®è£ ### ðpip èªå¨ä¸è½½&æ´æ° ``` pip install
--i https://pypi.tuna.tsinghua.edu.cn/simple poocr -U ``` ----------------------
---------------------------------------------------------- ## ðåè½
+-i https://mirrors.aliyun.com/pypi/simple/ poocr -U ``` -----------------------
+-------------------------------------------------------- ## ðåè½
 [ðå®ç½ï¼https://www.python-office.com/](https://www.python-office.com/
 ) ## ð»ææåè½çåè¡¨ð[ç¹æç´è¾¾](https://mp.weixin.qq.com/s/
 WxICBZZSgkm-OrvXB82hbg) ## ðï¸æ·»ç å ç¦ ### ðPRçå»ºè®® python-
 officeæ¬¢è¿ä»»ä½äººæ¥æ·»ç å ç¦ï¼è´¡ç®ä»£ç ï¼å»ºè®®æäº¤çprï¼pull
 requestï¼ç¬¦åä¸äºè§èï¼è§èå¦ä¸ï¼ åä¸é¡¹ç®å»ºè®¾çæ­¥éª¤ï¼ -
 ä¾å¦ï¼ä½ éè¦ç»python-officeæ·»å ä¸ä¸ªaddæ¹æ³ã 1.
 ä½ çGithubè´¦æ·åä¸ºï¼demo 2. äºæ¯ä½ å¨./
```

### Comparing `poocr-0.0.2/poocr/__init__.py` & `poocr-0.0.3/poocr/__init__.py`

 * *Files identical despite different names*

### Comparing `poocr-0.0.2/poocr/api/ocr.py` & `poocr-0.0.3/poocr/api/ocr.py`

 * *Files identical despite different names*

### Comparing `poocr-0.0.2/poocr/api/ocr2excel.py` & `poocr-0.0.3/poocr/api/ocr2excel.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,10 +27,17 @@
     # api_res = '{"VatInvoiceInfos": [{"Name": "销售方识别号", "Value": "911201103409033300", "Polygon": {"LeftTop": {"X": 374, "Y": 824}, "RightTop": {"X": 614, "Y": 824}, "RightBottom": {"X": 614, "Y": 847}, "LeftBottom": {"X": 374, "Y": 847}}}, {"Name": "销售方名称", "Value": "深圳腾讯游戏有限公司", "Polygon": {"LeftTop": {"X": 374, "Y": 788}, "RightTop": {"X": 618, "Y": 788}, "RightBottom": {"X": 618, "Y": 813}, "LeftBottom": {"X": 374, "Y": 813}}}, {"Name": "购买方识别号", "Value": "91440300MA55UJ6L44", "Polygon": {"LeftTop": {"X": 378, "Y": 268}, "RightTop": {"X": 653, "Y": 268}, "RightBottom": {"X": 653, "Y": 294}, "LeftBottom": {"X": 378, "Y": 294}}}, {"Name": "购买方名称", "Value": "腾讯优图有限公司", "Polygon": {"LeftTop": {"X": 375, "Y": 230}, "RightTop": {"X": 572, "Y": 230}, "RightBottom": {"X": 572, "Y": 256}, "LeftBottom": {"X": 375, "Y": 256}}}, {"Name": "发票名称", "Value": "天津增值税电子普通发票", "Polygon": {"LeftTop": {"X": 606, "Y": 59}, "RightTop": {"X": 1186, "Y": 59}, "RightBottom": {"X": 1186, "Y": 114}, "LeftBottom": {"X": 606, "Y": 114}}}, {"Name": "发票代码", "Value": "012001100311", "Polygon": {"LeftTop": {"X": 1342, "Y": 62}, "RightTop": {"X": 1502, "Y": 62}, "RightBottom": {"X": 1502, "Y": 85}, "LeftBottom": {"X": 1342, "Y": 85}}}, {"Name": "发票号码", "Value": "No63591128", "Polygon": {"LeftTop": {"X": 1342, "Y": 101}, "RightTop": {"X": 1453, "Y": 101}, "RightBottom": {"X": 1453, "Y": 124}, "LeftBottom": {"X": 1342, "Y": 124}}}, {"Name": "开票日期", "Value": "2019年06月16日", "Polygon": {"LeftTop": {"X": 1341, "Y": 135}, "RightTop": {"X": 1510, "Y": 135}, "RightBottom": {"X": 1510, "Y": 162}, "LeftBottom": {"X": 1341, "Y": 162}}}, {"Name": "机器编号", "Value": "499099606262", "Polygon": {"LeftTop": {"X": 269, "Y": 186}, "RightTop": {"X": 432, "Y": 186}, "RightBottom": {"X": 432, "Y": 210}, "LeftBottom": {"X": 269, "Y": 210}}}, {"Name": "校验码", "Value": "04656054380312409795", "Polygon": {"LeftTop": {"X": 1342, "Y": 177}, "RightTop": {"X": 1631, "Y": 177}, "RightBottom": {"X": 1631, "Y": 198}, "LeftBottom": {"X": 1342, "Y": 198}}}, {"Name": "密码区1", "Value": "033-<<>7>616<-4+*-+4/5230604", "Polygon": {"LeftTop": {"X": 1061, "Y": 233}, "RightTop": {"X": 1641, "Y": 233}, "RightBottom": {"X": 1641, "Y": 260}, "LeftBottom": {"X": 1061, "Y": 260}}}, {"Name": "密码区2", "Value": "*/78+740454724/0<34*9/>61856", "Polygon": {"LeftTop": {"X": 1062, "Y": 270}, "RightTop": {"X": 1641, "Y": 270}, "RightBottom": {"X": 1641, "Y": 297}, "LeftBottom": {"X": 1062, "Y": 297}}}, {"Name": "密码区3", "Value": "29/-0651-2*91440-47386<535<5", "Polygon": {"LeftTop": {"X": 1058, "Y": 307}, "RightTop": {"X": 1640, "Y": 307}, "RightBottom": {"X": 1640, "Y": 334}, "LeftBottom": {"X": 1058, "Y": 334}}}, {"Name": "密码区4", "Value": "92<<9-9+-601452319091>67>--7", "Polygon": {"LeftTop": {"X": 1062, "Y": 345}, "RightTop": {"X": 1642, "Y": 345}, "RightBottom": {"X": 1642, "Y": 372}, "LeftBottom": {"X": 1062, "Y": 372}}}, {"Name": "货物或应税劳务、服务名称", "Value": "客运服务费", "Polygon": {"LeftTop": {"X": 203, "Y": 439}, "RightTop": {"X": 324, "Y": 439}, "RightBottom": {"X": 324, "Y": 466}, "LeftBottom": {"X": 203, "Y": 466}}}, {"Name": "规格型号", "Value": "无", "Polygon": {"LeftTop": {"X": 619, "Y": 428}, "RightTop": {"X": 647, "Y": 428}, "RightBottom": {"X": 647, "Y": 454}, "LeftBottom": {"X": 619, "Y": 454}}}, {"Name": "单位", "Value": "次", "Polygon": {"LeftTop": {"X": 761, "Y": 426}, "RightTop": {"X": 790, "Y": 426}, "RightBottom": {"X": 790, "Y": 454}, "LeftBottom": {"X": 761, "Y": 454}}}, {"Name": "数量", "Value": "1", "Polygon": {"LeftTop": {"X": 886, "Y": 429}, "RightTop": {"X": 905, "Y": 429}, "RightBottom": {"X": 905, "Y": 452}, "LeftBottom": {"X": 886, "Y": 452}}}, {"Name": "单价", "Value": "87.28", "Polygon": {"LeftTop": {"X": 1019, "Y": 428}, "RightTop": {"X": 1082, "Y": 428}, "RightBottom": {"X": 1082, "Y": 452}, "LeftBottom": {"X": 1019, "Y": 452}}}, {"Name": "金额", "Value": "87.28", "Polygon": {"LeftTop": {"X": 1194, "Y": 428}, "RightTop": {"X": 1257, "Y": 428}, "RightBottom": {"X": 1257, "Y": 452}, "LeftBottom": {"X": 1194, "Y": 452}}}, {"Name": "税率", "Value": "3%", "Polygon": {"LeftTop": {"X": 1374, "Y": 427}, "RightTop": {"X": 1410, "Y": 427}, "RightBottom": {"X": 1410, "Y": 451}, "LeftBottom": {"X": 1374, "Y": 451}}}, {"Name": "税额", "Value": "2.62", "Polygon": {"LeftTop": {"X": 1509, "Y": 428}, "RightTop": {"X": 1560, "Y": 428}, "RightBottom": {"X": 1560, "Y": 451}, "LeftBottom": {"X": 1509, "Y": 451}}}, {"Name": "合计金额", "Value": "¥87.28", "Polygon": {"LeftTop": {"X": 1252, "Y": 686}, "RightTop": {"X": 1335, "Y": 686}, "RightBottom": {"X": 1335, "Y": 709}, "LeftBottom": {"X": 1252, "Y": 709}}}, {"Name": "合计税额", "Value": "2.62", "Polygon": {"LeftTop": {"X": 1581, "Y": 685}, "RightTop": {"X": 1650, "Y": 685}, "RightBottom": {"X": 1650, "Y": 709}, "LeftBottom": {"X": 1581, "Y": 709}}}, {"Name": "价税合计(大写)", "Value": "捌拾玖圆玖角整", "Polygon": {"LeftTop": {"X": 573, "Y": 731}, "RightTop": {"X": 744, "Y": 731}, "RightBottom": {"X": 744, "Y": 758}, "LeftBottom": {"X": 573, "Y": 758}}}, {"Name": "小写金额", "Value": "¥89.90", "Polygon": {"LeftTop": {"X": 1414, "Y": 734}, "RightTop": {"X": 1497, "Y": 734}, "RightBottom": {"X": 1497, "Y": 756}, "LeftBottom": {"X": 1414, "Y": 756}}}, {"Name": "销售方地址、电话", "Value": "天津经济技术开发区南港工业区综合服务区办公楼", "Polygon": {"LeftTop": {"X": 372, "Y": 862}, "RightTop": {"X": 722, "Y": 862}, "RightBottom": {"X": 722, "Y": 881}, "LeftBottom": {"X": 372, "Y": 881}}}, {"Name": "销售方开户行及账号", "Value": "招商银行股份有限公司天津自由贸易试验区分行122905939910401", "Polygon": {"LeftTop": {"X": 372, "Y": 894}, "RightTop": {"X": 977, "Y": 894}, "RightBottom": {"X": 977, "Y": 917}, "LeftBottom": {"X": 372, "Y": 917}}}, {"Name": "收款人", "Value": "张强", "Polygon": {"LeftTop": {"X": 299, "Y": 937}, "RightTop": {"X": 350, "Y": 937}, "RightBottom": {"X": 350, "Y": 963}, "LeftBottom": {"X": 299, "Y": 963}}}, {"Name": "复核", "Value": "静静", "Polygon": {"LeftTop": {"X": 699, "Y": 936}, "RightTop": {"X": 751, "Y": 936}, "RightBottom": {"X": 751, "Y": 962}, "LeftBottom": {"X": 699, "Y": 962}}}, {"Name": "开票人", "Value": "丽丽", "Polygon": {"LeftTop": {"X": 1082, "Y": 937}, "RightTop": {"X": 1132, "Y": 937}, "RightBottom": {"X": 1132, "Y": 962}, "LeftBottom": {"X": 1082, "Y": 962}}}, {"Name": "省", "Value": "天津市", "Polygon": null}, {"Name": "是否有公司印章", "Value": "0", "Polygon": null}, {"Name": "发票类型", "Value": "增值税电子普通发票", "Polygon": null}, {"Name": "发票消费类型", "Value": "服务", "Polygon": null}, {"Name": "成品油标志", "Value": "", "Polygon": null}, {"Name": "购买方地址、电话", "Value": "", "Polygon": null}, {"Name": "购买方开户行及账号", "Value": "", "Polygon": null}, {"Name": "打印发票代码", "Value": "", "Polygon": null}, {"Name": "打印发票号码", "Value": "", "Polygon": null}, {"Name": "备注", "Value": "", "Polygon": null}, {"Name": "联次", "Value": "", "Polygon": null}, {"Name": "是否代开", "Value": "", "Polygon": null}, {"Name": "市", "Value": "", "Polygon": null}, {"Name": "服务类型", "Value": "", "Polygon": null}, {"Name": "通行费标志", "Value": "", "Polygon": null}, {"Name": "车船税", "Value": "", "Polygon": null}, {"Name": "车牌号", "Value": "", "Polygon": null}, {"Name": "类型", "Value": "", "Polygon": null}, {"Name": "通行日期起", "Value": "", "Polygon": null}, {"Name": "通行日期止", "Value": "", "Polygon": null}], "Items": [{"LineNo": "1", "Name": "客运服务费", "Spec": "无", "Unit": "次", "Quantity": "1", "UnitPrice": "87.28", "AmountWithoutTax": "87.28", "TaxRate": "3%", "TaxAmount": "2.62", "TaxClassifyCode": null}], "PdfPageSize": 0, "Angle": 0.06033841148018837, "RequestId": "5c647af9-e441-4622-85c9-6cbbaf36e50d"}'
     api_res_json = json.loads(str(api_res))
     VatInvoiceInfos = api_res_json['VatInvoiceInfos']
     dict_pandas = {}
     for VatInvoiceInfo in simple_progress(VatInvoiceInfos):
         dict_pandas[VatInvoiceInfo['Name']] = VatInvoiceInfo['Value']
     Items = api_res_json['Items']
+    res_df = []
     for Item in Items:
         dict_pandas.update(Item)
-    pd.DataFrame(dict_pandas, index=[0]).to_excel(str(abs_output_excel))
+        res_df.append(pd.DataFrame(dict_pandas, index=[0]))
+    res_excel = res_df[0]
+    for index, line_df in enumerate(res_df):
+        if index == 0:
+            continue
+        res_excel = res_excel._append(line_df)
+    pd.DataFrame(res_excel).to_excel(str(abs_output_excel))
```

### Comparing `poocr-0.0.2/poocr/core/OCR.py` & `poocr-0.0.3/poocr/core/OCR.py`

 * *Files identical despite different names*

### Comparing `poocr-0.0.2/poocr/lib/CommonUtils.py` & `poocr-0.0.3/poocr/lib/CommonUtils.py`

 * *Files identical despite different names*

### Comparing `poocr-0.0.2/poocr/lib/Config.py` & `poocr-0.0.3/poocr/lib/Config.py`

 * *Files identical despite different names*

### Comparing `poocr-0.0.2/poocr/lib/Const.py` & `poocr-0.0.3/poocr/lib/Const.py`

 * *Files identical despite different names*

### Comparing `poocr-0.0.2/poocr.egg-info/PKG-INFO` & `poocr-0.0.3/poocr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poocr
-Version: 0.0.2
+Version: 0.0.3
 Summary: pip install poocr
 Home-page: https://www.python-office.com/
 Author: CoderWanFeng
 Author-email: 1957875073@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CoderWanFeng/poocr/issues
 Project-URL: Documentation, https://github.com/CoderWanFeng/poocr/blob/main/README.md
@@ -56,15 +56,15 @@
 -------------------------------------------------------------------------------
 
 ## 📦安装
 
 ### 🍊pip 自动下载&更新
 
 ```
-pip install -i https://pypi.tuna.tsinghua.edu.cn/simple poocr -U
+pip install -i https://mirrors.aliyun.com/pypi/simple/ poocr -U
 ```
 
 
 -------------------------------------------------------------------------------
 
 ## 📝功能
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: poocr Version: 0.0.2 Summary: pip install poocr
+Metadata-Version: 2.1 Name: poocr Version: 0.0.3 Summary: pip install poocr
 Home-page: https://www.python-office.com/ Author: CoderWanFeng Author-email:
 1957875073@qq.com License: MIT Project-URL: Bug Tracker, https://github.com/
 CoderWanFeng/poocr/issues Project-URL: Documentation, https://github.com/
 CoderWanFeng/poocr/blob/main/README.md Project-URL: Source Code, https://
 github.com/CoderWanFeng/poocr Platform: any Requires-Python: >=3.7 Description-
 Content-Type: text/markdown License-File: LICENSE
 [https://website-python-1300615378.cos.ap-nanjing.myqcloud.com/ads%2F1040x100-
@@ -13,16 +13,16 @@
        badge/%E5%BE%AE%E4%BF%A1-%E4%BA%A4%E6%B5%81%E7%BE%A4-brightgreen]
 ------------------------------------------------------------------------------
 - ## ðç®ä» poocr æ¯å¿«éè°ç¨è¾è®¯äºAIå¹³å°åè½çæ¥å£åéã
 ``poocr``ææåè½çå®ç°ï¼é½ä¾æäºè¾è®¯äºçæå­è¯å«ï¼å¦ææ¯å°ç½ç¨æ·ï¼å¯ä»¥**æ«ç ä¸å¾ï¼åè´¹å¼é**~
 ![](https://article-1300615378.cos.ap-nanjing.myqcloud.com/poocr%2Fapi-
 doc%2Fshare.jpg) --------------------------------------------------------------
 ----------------- ## ð¦å®è£ ### ðpip èªå¨ä¸è½½&æ´æ° ``` pip install
--i https://pypi.tuna.tsinghua.edu.cn/simple poocr -U ``` ----------------------
---------------------------------------------------------- ## ðåè½
+-i https://mirrors.aliyun.com/pypi/simple/ poocr -U ``` -----------------------
+-------------------------------------------------------- ## ðåè½
 [ðå®ç½ï¼https://www.python-office.com/](https://www.python-office.com/
 ) ## ð»ææåè½çåè¡¨ð[ç¹æç´è¾¾](https://mp.weixin.qq.com/s/
 WxICBZZSgkm-OrvXB82hbg) ## ðï¸æ·»ç å ç¦ ### ðPRçå»ºè®® python-
 officeæ¬¢è¿ä»»ä½äººæ¥æ·»ç å ç¦ï¼è´¡ç®ä»£ç ï¼å»ºè®®æäº¤çprï¼pull
 requestï¼ç¬¦åä¸äºè§èï¼è§èå¦ä¸ï¼ åä¸é¡¹ç®å»ºè®¾çæ­¥éª¤ï¼ -
 ä¾å¦ï¼ä½ éè¦ç»python-officeæ·»å ä¸ä¸ªaddæ¹æ³ã 1.
 ä½ çGithubè´¦æ·åä¸ºï¼demo 2. äºæ¯ä½ å¨./
```

### Comparing `poocr-0.0.2/setup.cfg` & `poocr-0.0.3/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 6f6f 6372 0d0a 7665 7273 696f   = poocr..versio
-00000020: 6e20 3d20 302e 302e 320d 0a64 6573 6372  n = 0.0.2..descr
+00000020: 6e20 3d20 302e 302e 330d 0a64 6573 6372  n = 0.0.3..descr
 00000030: 6970 7469 6f6e 203d 2070 6970 2069 6e73  iption = pip ins
 00000040: 7461 6c6c 2070 6f6f 6372 0d0a 6c6f 6e67  tall poocr..long
 00000050: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
 00000060: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
 00000070: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 00000080: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type = 
 00000090: 7465 7874 2f6d 6172 6b64 6f77 6e0d 0a75  text/markdown..u
@@ -31,15 +31,16 @@
 000001e0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
 000001f0: 6d2f 436f 6465 7257 616e 4665 6e67 2f70  m/CoderWanFeng/p
 00000200: 6f6f 6372 0d0a 0d0a 5b6f 7074 696f 6e73  oocr....[options
 00000210: 5d0d 0a70 6163 6b61 6765 7320 3d20 6669  ]..packages = fi
 00000220: 6e64 3a0d 0a69 6e73 7461 6c6c 5f72 6571  nd:..install_req
 00000230: 7569 7265 7320 3d20 0d0a 0974 6f6d 6c0d  uires = ...toml.
 00000240: 0a09 7465 6e63 656e 7463 6c6f 7564 2d73  ..tencentcloud-s
-00000250: 646b 2d70 7974 686f 6e0d 0a70 7974 686f  dk-python..pytho
-00000260: 6e5f 7265 7175 6972 6573 203d 203e 3d33  n_requires = >=3
-00000270: 2e37 0d0a 696e 636c 7564 655f 7061 636b  .7..include_pack
-00000280: 6167 655f 6461 7461 203d 2054 7275 650d  age_data = True.
-00000290: 0a7a 6970 5f73 6166 6520 3d20 4661 6c73  .zip_safe = Fals
-000002a0: 650d 0a0d 0a5b 6567 675f 696e 666f 5d0d  e....[egg_info].
-000002b0: 0a74 6167 5f62 7569 6c64 203d 200d 0a74  .tag_build = ..t
-000002c0: 6167 5f64 6174 6520 3d20 300d 0a0d 0a    ag_date = 0....
+00000250: 646b 2d70 7974 686f 6e0d 0a09 706f 7072  dk-python...popr
+00000260: 6f67 7265 7373 0d0a 7079 7468 6f6e 5f72  ogress..python_r
+00000270: 6571 7569 7265 7320 3d20 3e3d 332e 370d  equires = >=3.7.
+00000280: 0a69 6e63 6c75 6465 5f70 6163 6b61 6765  .include_package
+00000290: 5f64 6174 6120 3d20 5472 7565 0d0a 7a69  _data = True..zi
+000002a0: 705f 7361 6665 203d 2046 616c 7365 0d0a  p_safe = False..
+000002b0: 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a 7461  ..[egg_info]..ta
+000002c0: 675f 6275 696c 6420 3d20 0d0a 7461 675f  g_build = ..tag_
+000002d0: 6461 7465 203d 2030 0d0a 0d0a            date = 0....
```

