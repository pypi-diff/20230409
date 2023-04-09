# Comparing `tmp/analysisbykwok-0.0.14.tar.gz` & `tmp/analysisbykwok-0.0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "analysisbykwok-0.0.14.tar", last modified: Sun Apr  9 05:15:18 2023, max compression
+gzip compressed data, was "analysisbykwok-0.0.15.tar", last modified: Sun Apr  9 12:08:58 2023, max compression
```

## Comparing `analysisbykwok-0.0.14.tar` & `analysisbykwok-0.0.15.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 05:15:18.722718 analysisbykwok-0.0.14/
--rw-rw-rw-   0        0        0       62 2023-04-09 05:15:18.722718 analysisbykwok-0.0.14/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-09 05:15:18.717763 analysisbykwok-0.0.14/analysisbykwok/
--rw-rw-rw-   0        0        0    11439 2023-04-09 05:14:56.000000 analysisbykwok-0.0.14/analysisbykwok/__init__.py
--rw-rw-rw-   0        0        0       23 2023-04-09 05:13:19.000000 analysisbykwok-0.0.14/analysisbykwok/_version.py
-drwxrwxrwx   0        0        0        0 2023-04-09 05:15:18.721654 analysisbykwok-0.0.14/analysisbykwok.egg-info/
--rw-rw-rw-   0        0        0       62 2023-04-09 05:15:18.000000 analysisbykwok-0.0.14/analysisbykwok.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      220 2023-04-09 05:15:18.000000 analysisbykwok-0.0.14/analysisbykwok.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 05:15:18.000000 analysisbykwok-0.0.14/analysisbykwok.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-04-09 05:15:18.000000 analysisbykwok-0.0.14/analysisbykwok.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       70 2023-04-09 05:13:19.000000 analysisbykwok-0.0.14/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-09 05:15:18.722718 analysisbykwok-0.0.14/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-09 12:08:58.646615 analysisbykwok-0.0.15/
+-rw-rw-rw-   0        0        0       62 2023-04-09 12:08:58.646615 analysisbykwok-0.0.15/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-09 12:08:58.271590 analysisbykwok-0.0.15/analysisbykwok/
+-rw-rw-rw-   0        0        0    13917 2023-04-09 12:07:37.000000 analysisbykwok-0.0.15/analysisbykwok/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-04-09 12:05:52.000000 analysisbykwok-0.0.15/analysisbykwok/_version.py
+drwxrwxrwx   0        0        0        0 2023-04-09 12:08:58.631106 analysisbykwok-0.0.15/analysisbykwok.egg-info/
+-rw-rw-rw-   0        0        0       62 2023-04-09 12:08:58.000000 analysisbykwok-0.0.15/analysisbykwok.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      220 2023-04-09 12:08:58.000000 analysisbykwok-0.0.15/analysisbykwok.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 12:08:58.000000 analysisbykwok-0.0.15/analysisbykwok.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-04-09 12:08:58.000000 analysisbykwok-0.0.15/analysisbykwok.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       70 2023-04-09 12:05:40.000000 analysisbykwok-0.0.15/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-09 12:08:58.646615 analysisbykwok-0.0.15/setup.cfg
```

### Comparing `analysisbykwok-0.0.14/analysisbykwok/__init__.py` & `analysisbykwok-0.0.15/analysisbykwok/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 import pandas as pd
 import requests
 import random
+import email
+import imaplib
+import os
+from email.header import decode_header
+import datetime
 import execjs
 import json
 import mimetypes
 import smtplib   # 发送邮件模块
 from email import encoders
 from email.mime.multipart import MIMEMultipart    # 使用MIMEMultipart来标示这个邮件是多个部分组成的
 from email.mime.base import MIMEBase
@@ -224,8 +229,62 @@
             encoders.encode_base64(file_msg)  # 把附件编码
             file_msg.add_header('Content-Disposition', 'attachment',
                                 filename=str(filepath.split('\\')[-1].split('.')[0]))  # 修改邮件头
             msg.attach(file_msg)
         server = smtplib.SMTP(smtp_server)
         server.login(username, password)
         server.sendmail(sender, receivers, msg.as_string())
-        server.quit()
+        server.quit()
+    def GetEmail(mail, password, dir):
+        def decode_str(s):  # 字符编码转换
+            value, charset = decode_header(s)[0]
+            if charset:
+                value = value.decode(charset)
+                return value
+
+        def get_email_title(msg):
+            subject = email.header.decode_header(msg.get('subject'))
+            if type(subject[-1][0]) == bytes:
+                title = subject[-1][0].decode(str(subject[-1][1]))
+            elif type(subject[-1][0]) == str:
+                title = subject[-1][0]
+            print("title:", title)
+            return title
+
+        def get_att(msg, dir):
+            for part in msg.walk():
+                # file_name = part.get_param("name")
+                file_name = part.get_filename()
+                if file_name:
+                    h = email.header.Header(file_name)
+                    dh = email.header.decode_header(h)
+                    filename = dh[0][0]
+                    if dh[0][1]:
+                        filename = decode_str(str(filename, dh[0][1]))
+                        data = part.get_payload(decode=True)
+                        att_file = open(dir + file_name + '.zip', 'wb')
+                        print('附件下载成功',file_name)
+                        att_file.write(data)
+                        att_file.close()
+
+        """入口函数，登录imap服务"""
+        server = imaplib.IMAP4_SSL('smtp.qq.com', 993)
+        server.login(mail, password)
+        server.select('INBOX')
+        status, data = server.search(None, "ALL")
+        if status != 'OK':
+            raise Exception('read email error')
+        emailids = data[0].split()
+        mail_counts = len(emailids)
+        # print("count:", mail_counts)
+        # 邮件的遍历是按时间从后往前，这里我们选择最新的一封邮件
+        for i in range(mail_counts - 1, mail_counts - 2, -2):
+            status, edata = server.fetch(emailids[i], '(RFC822)')
+            msg = email.message_from_bytes(edata[0][1])
+            # 获取邮件主题title
+            subject = email.header.decode_header(msg.get('subject'))
+            if type(subject[-1][0]) == bytes:
+                title = subject[-1][0].decode(str(subject[-1][1]))
+            elif type(subject[-1][0]) == str:
+                title = subject[-1][0]
+            # print("title:", title)
+            get_att(msg, dir)
```

