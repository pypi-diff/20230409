# Comparing `tmp/analysisbykwok-0.0.13.tar.gz` & `tmp/analysisbykwok-0.0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "analysisbykwok-0.0.13.tar", last modified: Sun Apr  9 02:54:44 2023, max compression
+gzip compressed data, was "analysisbykwok-0.0.14.tar", last modified: Sun Apr  9 05:15:18 2023, max compression
```

## Comparing `analysisbykwok-0.0.13.tar` & `analysisbykwok-0.0.14.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 02:54:44.494120 analysisbykwok-0.0.13/
--rw-rw-rw-   0        0        0       62 2023-04-09 02:54:44.494120 analysisbykwok-0.0.13/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-09 02:54:44.478527 analysisbykwok-0.0.13/analysisbykwok/
--rw-rw-rw-   0        0        0     9472 2023-04-09 02:54:24.000000 analysisbykwok-0.0.13/analysisbykwok/__init__.py
--rw-rw-rw-   0        0        0       23 2023-04-09 02:53:13.000000 analysisbykwok-0.0.13/analysisbykwok/_version.py
-drwxrwxrwx   0        0        0        0 2023-04-09 02:54:44.494120 analysisbykwok-0.0.13/analysisbykwok.egg-info/
--rw-rw-rw-   0        0        0       62 2023-04-09 02:54:44.000000 analysisbykwok-0.0.13/analysisbykwok.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      220 2023-04-09 02:54:44.000000 analysisbykwok-0.0.13/analysisbykwok.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 02:54:44.000000 analysisbykwok-0.0.13/analysisbykwok.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-04-09 02:54:44.000000 analysisbykwok-0.0.13/analysisbykwok.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       70 2023-04-09 02:53:13.000000 analysisbykwok-0.0.13/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-09 02:54:44.494120 analysisbykwok-0.0.13/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-09 05:15:18.722718 analysisbykwok-0.0.14/
+-rw-rw-rw-   0        0        0       62 2023-04-09 05:15:18.722718 analysisbykwok-0.0.14/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-09 05:15:18.717763 analysisbykwok-0.0.14/analysisbykwok/
+-rw-rw-rw-   0        0        0    11439 2023-04-09 05:14:56.000000 analysisbykwok-0.0.14/analysisbykwok/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-04-09 05:13:19.000000 analysisbykwok-0.0.14/analysisbykwok/_version.py
+drwxrwxrwx   0        0        0        0 2023-04-09 05:15:18.721654 analysisbykwok-0.0.14/analysisbykwok.egg-info/
+-rw-rw-rw-   0        0        0       62 2023-04-09 05:15:18.000000 analysisbykwok-0.0.14/analysisbykwok.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      220 2023-04-09 05:15:18.000000 analysisbykwok-0.0.14/analysisbykwok.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 05:15:18.000000 analysisbykwok-0.0.14/analysisbykwok.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-04-09 05:15:18.000000 analysisbykwok-0.0.14/analysisbykwok.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       70 2023-04-09 05:13:19.000000 analysisbykwok-0.0.14/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-09 05:15:18.722718 analysisbykwok-0.0.14/setup.cfg
```

### Comparing `analysisbykwok-0.0.13/analysisbykwok/__init__.py` & `analysisbykwok-0.0.14/analysisbykwok/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,20 @@
 import pandas as pd
 import requests
 import random
 import execjs
 import json
+import mimetypes
+import smtplib   # 发送邮件模块
+from email import encoders
+from email.mime.multipart import MIMEMultipart    # 使用MIMEMultipart来标示这个邮件是多个部分组成的
+from email.mime.base import MIMEBase
+from email.mime.text import MIMEText   # 定义邮件内容
+import  datetime
+from email.utils import formataddr
 import os.path
 from zipfile import ZipFile
 import zipfile
 import os
 if not os.path.exists(
         r'C:\Windows\AgentPool.xlsx'):
     input('注意注意！\n请确保存在\'C:\Windows\AgentPool.xlsx\'的ip代理文件\n否则，ip池功能将无法使用\n继续使用请敲击回车键')
@@ -186,8 +194,38 @@
                         arcname=dn + '/' + os.path.relpath(fp, dir_)
                     )
         print('压缩成功，已经压缩到了文件夹:' + str(dir_) + '.zip')
     def ZipOut(dir, out):
         zf = zipfile.ZipFile(dir)
         os.chdir(out)
         ret = zf.extractall(path=out)  # 解压到指定目录
-        print('解压成功')
+        print('解压成功')
+    def SendEmail(password, receivers, text, sub, filepath):
+        smtp_server = "smtp.qq.com"  # 发送邮箱服务器
+        username = "yongxingkwok@foxmail.com"  # 用于发送邮箱的用户账号
+        sender = 'yongxingkwok@foxmail.com'  # 发送者的邮箱
+        EMAIL_FROM_NAME = '郭永兴'  # 自定义发件人名称
+        time = datetime.datetime.today().strftime("%m-%d %H：%M")
+        msg = MIMEMultipart()
+        # 邮件正文
+        msg.attach(MIMEText(str(text), 'plain', 'utf-8'))  # 文本内容换行\r\n
+        msg['From'] = formataddr(pair=(EMAIL_FROM_NAME, sender))  # 自定义发件人的名称
+        msg['To'] = ";".join(receivers)  # 发送给多个好友
+        subject = str(sub).format(time)
+        msg['Subject'] = subject
+        if filepath != '':
+            data = open(filepath, 'rb')
+            ctype, encoding = mimetypes.guess_type(filepath)
+            if ctype is None or encoding is not None:
+                ctype = 'application/octet-stream'
+            maintype, subtype = ctype.split('/', 1)
+            file_msg = MIMEBase(maintype, subtype)
+            file_msg.set_payload(data.read())
+            data.close()
+            encoders.encode_base64(file_msg)  # 把附件编码
+            file_msg.add_header('Content-Disposition', 'attachment',
+                                filename=str(filepath.split('\\')[-1].split('.')[0]))  # 修改邮件头
+            msg.attach(file_msg)
+        server = smtplib.SMTP(smtp_server)
+        server.login(username, password)
+        server.sendmail(sender, receivers, msg.as_string())
+        server.quit()
```

