# Comparing `tmp/pteropy-0.1.6.tar.gz` & `tmp/pteropy-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pteropy-0.1.6.tar", last modified: Fri Apr  7 15:05:47 2023, max compression
+gzip compressed data, was "pteropy-0.1.7.tar", last modified: Sun Apr  9 13:34:00 2023, max compression
```

## Comparing `pteropy-0.1.6.tar` & `pteropy-0.1.7.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-07 15:05:47.402055 pteropy-0.1.6/
--rw-rw-rw-   0        0        0     2226 2023-04-07 15:05:47.398490 pteropy-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     1774 2023-04-07 15:05:03.000000 pteropy-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-07 15:05:47.365358 pteropy-0.1.6/pteropy/
--rw-rw-rw-   0        0        0     6194 2023-04-07 15:03:19.000000 pteropy-0.1.6/pteropy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-07 15:05:47.387936 pteropy-0.1.6/pteropy.egg-info/
--rw-rw-rw-   0        0        0     2226 2023-04-07 15:05:47.000000 pteropy-0.1.6/pteropy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      162 2023-04-07 15:05:47.000000 pteropy-0.1.6/pteropy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-07 15:05:47.000000 pteropy-0.1.6/pteropy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-07 15:05:47.000000 pteropy-0.1.6/pteropy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-07 15:05:47.402055 pteropy-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      730 2023-04-07 15:03:33.000000 pteropy-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 13:34:00.773383 pteropy-0.1.7/
+-rw-rw-rw-   0        0        0     1083 2023-04-04 14:05:48.000000 pteropy-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0     2778 2023-04-09 13:34:00.769214 pteropy-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2308 2023-04-09 13:33:36.000000 pteropy-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-09 13:34:00.740185 pteropy-0.1.7/pteropy/
+-rw-rw-rw-   0        0        0    10648 2023-04-09 13:27:29.000000 pteropy-0.1.7/pteropy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-09 13:34:00.765214 pteropy-0.1.7/pteropy.egg-info/
+-rw-rw-rw-   0        0        0     2778 2023-04-09 13:34:00.000000 pteropy-0.1.7/pteropy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      170 2023-04-09 13:34:00.000000 pteropy-0.1.7/pteropy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 13:34:00.000000 pteropy-0.1.7/pteropy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-09 13:34:00.000000 pteropy-0.1.7/pteropy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-09 13:34:00.774377 pteropy-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      725 2023-04-09 13:26:15.000000 pteropy-0.1.7/setup.py
```

### Comparing `pteropy-0.1.6/PKG-INFO` & `pteropy-0.1.7/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: pteropy
-Version: 0.1.6
+Version: 0.1.7
 Summary: 簡單存取Pterodactyl api
 Home-page: https://github.com/HansHans135/pteropy
-Author: seanbbear
+Author: Hans
 Author-email: ccoccc14@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # pteropy
 適用於Pterodactyl api的python庫
 
 # 安裝
 ```
 pip install pteropy
@@ -47,20 +48,20 @@
 
 ```py
 from pteropy import Pterodactyl_Application
 base_url = "https://面板網址"
 api_key = "api key"
 ptero = Pterodactyl_Application(base_url, api_key)
 
-#檢查api連線狀態
-ptero.check()
-#創建用戶
-ptero.create_user(username="用戶名",email="用戶email", password="密碼")
-#所有用戶
-ptero.list_users()
+
+ptero.check()  #檢查api連線狀態
+
+ptero.create_user(username="用戶名",email="用戶email", password="密碼")  #創建用戶
+
+ptero.list_users()  #所有用戶
 ```
 
 
 # Pterodactyl_Client範例
 key創建位置:/account/api
 
 ## 基本設置
@@ -85,28 +86,45 @@
 
 ```py
 from pteropy import Pterodactyl_Client
 base_url = "https://面板網址"
 api_key = "api key"
 ptero = Pterodactyl_Client(base_url, api_key)
 
-#檢查api連線狀態
-ptero.check()
-#獲得伺服器資料
-ptero.get_server("3fa3d78d")
-#獲得伺服器列表
-ptero.list_servers()
-#重命名伺服器
-ptero.rename_server("3fa3d78d","名子")
-#發送指令
-ptero.send_command("3fa3d78d","指令")
-
-#啟動伺服器
-ptero.start_server("3fa3d78d")
-#重啟伺服器
-ptero.restart_server("3fa3d78d")
-#關閉伺服器
-ptero.stop_server("3fa3d78d")
-#強制關閉伺服器
-ptero.kill_server("3fa3d78d")
+
+ptero.check()  #檢查api連線狀態
+
+ptero.account_details()  #帳戶資訊
+
+ptero.details_2FA()  #生成TOTP 二維碼圖像以允許設置 2FA
+
+ptero.enable_2FA()  #使用 details_2FA 請求生成的二維碼啟用 TOTP 2FA
+
+ptero.disable_2FA()  #禁用帳戶上的 TOTP 2FA
+
+ptero.update_email()  #更新帳戶的電子郵件位址
+
+ptero.update_password()  #更新帳戶的密碼
+
+ptero.list_API_keys()  #列出 API 金鑰
+
+ptero.create_API_key()  #生成新的 API 金鑰
+
+ptero.delete_API_key()  #刪除指定的 API 金鑰
+
+ptero.get_server("3fa3d78d")  #獲得伺服器資料
+
+ptero.list_servers()  #獲得伺服器列表
+
+ptero.rename_server("3fa3d78d","名子")  #重命名伺服器
+
+ptero.send_command("3fa3d78d","指令")  #發送指令
+
+ptero.start_server("3fa3d78d")  #啟動伺服器
+
+ptero.restart_server("3fa3d78d")  #重啟伺服器
+
+ptero.stop_server("3fa3d78d")  #關閉伺服器
+
+ptero.kill_server("3fa3d78d")  #強制關閉伺服器
 ```
```

### Comparing `pteropy-0.1.6/README.md` & `pteropy-0.1.7/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -32,20 +32,20 @@
 
 ```py
 from pteropy import Pterodactyl_Application
 base_url = "https://面板網址"
 api_key = "api key"
 ptero = Pterodactyl_Application(base_url, api_key)
 
-#檢查api連線狀態
-ptero.check()
-#創建用戶
-ptero.create_user(username="用戶名",email="用戶email", password="密碼")
-#所有用戶
-ptero.list_users()
+
+ptero.check()  #檢查api連線狀態
+
+ptero.create_user(username="用戶名",email="用戶email", password="密碼")  #創建用戶
+
+ptero.list_users()  #所有用戶
 ```
 
 
 # Pterodactyl_Client範例
 key創建位置:/account/api
 
 ## 基本設置
@@ -70,27 +70,44 @@
 
 ```py
 from pteropy import Pterodactyl_Client
 base_url = "https://面板網址"
 api_key = "api key"
 ptero = Pterodactyl_Client(base_url, api_key)
 
-#檢查api連線狀態
-ptero.check()
-#獲得伺服器資料
-ptero.get_server("3fa3d78d")
-#獲得伺服器列表
-ptero.list_servers()
-#重命名伺服器
-ptero.rename_server("3fa3d78d","名子")
-#發送指令
-ptero.send_command("3fa3d78d","指令")
-
-#啟動伺服器
-ptero.start_server("3fa3d78d")
-#重啟伺服器
-ptero.restart_server("3fa3d78d")
-#關閉伺服器
-ptero.stop_server("3fa3d78d")
-#強制關閉伺服器
-ptero.kill_server("3fa3d78d")
+
+ptero.check()  #檢查api連線狀態
+
+ptero.account_details()  #帳戶資訊
+
+ptero.details_2FA()  #生成TOTP 二維碼圖像以允許設置 2FA
+
+ptero.enable_2FA()  #使用 details_2FA 請求生成的二維碼啟用 TOTP 2FA
+
+ptero.disable_2FA()  #禁用帳戶上的 TOTP 2FA
+
+ptero.update_email()  #更新帳戶的電子郵件位址
+
+ptero.update_password()  #更新帳戶的密碼
+
+ptero.list_API_keys()  #列出 API 金鑰
+
+ptero.create_API_key()  #生成新的 API 金鑰
+
+ptero.delete_API_key()  #刪除指定的 API 金鑰
+
+ptero.get_server("3fa3d78d")  #獲得伺服器資料
+
+ptero.list_servers()  #獲得伺服器列表
+
+ptero.rename_server("3fa3d78d","名子")  #重命名伺服器
+
+ptero.send_command("3fa3d78d","指令")  #發送指令
+
+ptero.start_server("3fa3d78d")  #啟動伺服器
+
+ptero.restart_server("3fa3d78d")  #重啟伺服器
+
+ptero.stop_server("3fa3d78d")  #關閉伺服器
+
+ptero.kill_server("3fa3d78d")  #強制關閉伺服器
 ```
```

### Comparing `pteropy-0.1.6/pteropy/__init__.py` & `pteropy-0.1.7/pteropy/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,45 +1,48 @@
 import requests
 import os
 import json
+
+
 class Pterodactyl_Application:
     def __init__(self, base_url, api_key):
-        if base_url[-1]=="/":
-            base_url=base_url[:-1]
+        if base_url[-1] == "/":
+            base_url = base_url[:-1]
         self.base_url = base_url
         self.api_key = api_key
 
     def check(self):
         endpoint = f"{self.base_url}/api/application/users"
         headers = {
             "Authorization": f"Bearer {self.api_key}",
             "Content-Type": "application/json",
             "Accept": "Application/vnd.pterodactyl.v1+json"
         }
         try:
             response = requests.get(endpoint, headers=headers)
         except:
-            
+
             return False
         try:
             response.json()["errors"]
             return False
         except:
             return True
+
     def list_uesrs(self):
         url = f'{self.base_url}/api/application/users'
         headers = {
-    "Authorization": f"Bearer {self.api_key}",
-    "Accept": "application/json",
-    "Content-Type": "application/json",
-}
+            "Authorization": f"Bearer {self.api_key}",
+            "Accept": "application/json",
+            "Content-Type": "application/json",
+        }
 
         response = requests.request('GET', url, headers=headers)
         return response.json()
-    
+
     def create_user(self, username, email, password):
         endpoint = f"{self.base_url}/api/application/users"
         headers = {
             "Authorization": f"Bearer {self.api_key}",
             "Content-Type": "application/json",
             "Accept": "Application/vnd.pterodactyl.v1+json"
         }
@@ -48,138 +51,250 @@
             "first_name": username,
             "last_name": username,
             "email": email,
             "password": password
         }
         response = requests.post(endpoint, headers=headers, json=data)
         return response.json()
-    def load_egg(self ,f:str):
+
+    def load_egg(self, f: str):
         all = os.listdir(f)
         for i in all:
             if i[-5:] == ".json":
                 with open(f"{f}/{i}", mode="r", encoding="utf-8") as filt:
                     data = json.load(filt)
                 print(data["name"])
 
 
 class Pterodactyl_Client:
     def __init__(self, base_url, api_key):
-        if base_url[-1]=="/":
-            base_url=base_url[:-1]
+        if base_url[-1] == "/":
+            base_url = base_url[:-1]
         self.base_url = base_url
         self.api_key = api_key
-    
+
     def check(self):
         endpoint = f"{self.base_url}/api/client/account"
         headers = {
             "Authorization": f"Bearer {self.api_key}",
             "Content-Type": "application/json",
             "Accept": "Application/vnd.pterodactyl.v1+json"
         }
         try:
             response = requests.get(endpoint, headers=headers)
         except:
-            
+
             return False
         try:
             response.json()["errors"]
             return False
         except:
             return True
 
     def list_servers(self):
         url = f'{self.base_url}/api/client'
         headers = {
-    "Authorization": f"Bearer {self.api_key}",
-    "Accept": "application/json"
-    }
+            "Authorization": f"Bearer {self.api_key}",
+            "Accept": "application/json"
+        }
+
+        response = requests.request('GET', url, headers=headers)
+        return response.json()
+
+    def account_details(self):
+        url = f'{self.base_url}/api/client/account'
+        headers = {
+            "Authorization": f"Bearer {self.api_key}",
+            "Accept": "application/json",
+            "Content-Type": "application/json",
+        }
+
+        response = requests.request('GET', url, headers=headers)
+        return response.json()
+
+    def details_2FA(self):
+        url = f'{self.base_url}/api/client/account/two-factor'
+        headers = {
+            "Authorization": f"Bearer {self.api_key}",
+            "Accept": "application/json",
+            "Content-Type": "application/json",
+        }
+
+        response = requests.request('GET', url, headers=headers)
+        return response.json()
+
+    def enable_2FA(self, code):
+        url = f'{self.base_url}/api/client/account/two-factor'
+        headers = {
+            "Authorization": f"Bearer {self.api_key}",
+            "Accept": "application/json",
+            "Content-Type": "application/json",
+        }
+        payload = '{"code": "awa"}'.replace("awa", code)
+
+        response = requests.request('POST', url, data=payload, headers=headers)
+        return response.json()
+
+    def disable_2FA(self, password):
+        url = f'{self.base_url}/api/client/account/two-factor'
+        headers = {
+            "Authorization": f"Bearer {self.api_key}",
+            "Accept": "application/json",
+            "Content-Type": "application/json",
+        }
+        payload = '{"password": "pd"}'.replace("pd", password)
+
+        response = requests.request(
+            'DELETE', url, data=payload, headers=headers)
+        return response
+
+    def update_email(self, email, password):
+        url = f'{self.base_url}/api/client/account/email'
+        headers = {
+            "Authorization": f"Bearer {self.api_key}",
+            "Accept": "application/json",
+            "Content-Type": "application/json",
+        }
+        payload = '{"email": "ema","password": "pd"}'.replace(
+            "ema", email).replace("pd", password)
+
+        response = requests.request('PUT', url, data=payload, headers=headers)
+        return response
+
+    def update_password(self, current_password, new_password):
+        url = f'{self.base_url}/api/client/account/password'
+        headers = {
+            "Authorization": f"Bearer {self.api_key}",
+            "Accept": "application/json",
+            "Content-Type": "application/json",
+        }
+        payload = '{"current_password": "Pd","password": "pd","password_confirmation": "pd"}'.replace(
+            "Pd", current_password).replace("pd", new_password)
+
+        response = requests.request('PUT', url, data=payload, headers=headers)
+        return response
+
+    def list_API_keys(self):
+        url = f'{self.base_url}/api/client/account/api-keys'
+        headers = {
+            "Authorization": f"Bearer {self.api_key}",
+            "Accept": "application/json",
+            "Content-Type": "application/json",
+        }
 
         response = requests.request('GET', url, headers=headers)
         return response.json()
-    
-    def get_server(self,server:str):
-        self.server=server
+
+    def create_API_key(self, description, allowed_ips: list = None):
+        url = f'{self.base_url}/api/client/account/api-keys'
+        headers = {
+            "Authorization": f"Bearer {self.api_key}",
+            "Accept": "application/json",
+            "Content-Type": "application/json",
+        }
+        if allowed_ips == None:
+            payload = '{"description": "dn"}'.replace("dn", description)
+        else:
+            payload = '{"description": "Restricted IPs","allowed_ips": []}'.replace(
+                "dn", description).replace("[]", allowed_ips)
+
+        response = requests.request('POST', url, data=payload, headers=headers)
+        return response.json()
+
+    def delete_API_key(self, key_identifier):
+        url = f'{self.base_url}/api/client/account/api-keys/{key_identifier}'
+        headers = {
+            "Authorization": f"Bearer {self.api_key}",
+            "Accept": "application/json",
+            "Content-Type": "application/json",
+        }
+
+        response = requests.request('DELETE', url,  headers=headers)
+        return response
+
+    def get_server(self, server: str):
+        self.server = server
         url = f'{self.base_url}/api/client/servers/{self.server}'
         headers = {
-    "Authorization": f"Bearer {self.api_key}",
-    "Accept": "application/json",
-    "Content-Type": "application/json"
-}
+            "Authorization": f"Bearer {self.api_key}",
+            "Accept": "application/json",
+            "Content-Type": "application/json"
+        }
 
         response = requests.request('GET', url, headers=headers)
         try:
             if response.json()["errors"][0]["status"] == "404":
                 return None
             else:
                 return response.json()
         except:
             return response.json()
-    
-    def stop_server(self,server:str):
+
+    def stop_server(self, server: str):
         url = f'{self.base_url}/api/client/servers/{server}/power'
         headers = {
-    "Authorization": f"Bearer {self.api_key}",
-    "Accept": "application/json",
-    "Content-Type": "application/json"
-}
+            "Authorization": f"Bearer {self.api_key}",
+            "Accept": "application/json",
+            "Content-Type": "application/json"
+        }
         payload = '{"signal": "stop"}'
 
         response = requests.request('POST', url, data=payload, headers=headers)
         return response
-    
-    def start_server(self,server:str):
+
+    def start_server(self, server: str):
         url = f'{self.base_url}/api/client/servers/{server}/power'
         headers = {
-    "Authorization": f"Bearer {self.api_key}",
-    "Accept": "application/json",
-    "Content-Type": "application/json"
-}
+            "Authorization": f"Bearer {self.api_key}",
+            "Accept": "application/json",
+            "Content-Type": "application/json"
+        }
         payload = '{"signal": "start"}'
 
         response = requests.request('POST', url, data=payload, headers=headers)
         return response
-    
-    def restart_server(self,server:str):
+
+    def restart_server(self, server: str):
         url = f'{self.base_url}/api/client/servers/{server}/power'
         headers = {
-    "Authorization": f"Bearer {self.api_key}",
-    "Accept": "application/json",
-    "Content-Type": "application/json"
-}
+            "Authorization": f"Bearer {self.api_key}",
+            "Accept": "application/json",
+            "Content-Type": "application/json"
+        }
         payload = '{"signal": "restart"}'
 
         response = requests.request('POST', url, data=payload, headers=headers)
         return response
-    
-    def kill_server(self,server:str):
+
+    def kill_server(self, server: str):
         url = f'{self.base_url}/api/client/servers/{server}/power'
         headers = {
-    "Authorization": f"Bearer {self.api_key}",
-    "Accept": "application/json",
-    "Content-Type": "application/json"
-}
+            "Authorization": f"Bearer {self.api_key}",
+            "Accept": "application/json",
+            "Content-Type": "application/json"
+        }
         payload = '{"signal": "kill"}'
 
         response = requests.request('POST', url, data=payload, headers=headers)
         return response
-    
-    def rename_server(self,server:str,name:str):
+
+    def rename_server(self, server: str, name: str):
         url = f'{self.base_url}/api/client/servers/{server}/settings/rename'
         headers = {
-        "Authorization": f"Bearer {self.api_key}",
-        "Accept": "application/json",
-        "Content-Type": "application/json"
+            "Authorization": f"Bearer {self.api_key}",
+            "Accept": "application/json",
+            "Content-Type": "application/json"
         }
-        payload = '{"name": "awa"}'.replace("awa",name)
-        response = requests.request('POST',url,data=payload,headers=headers)
+        payload = '{"name": "awa"}'.replace("awa", name)
+        response = requests.request('POST', url, data=payload, headers=headers)
         return response
-        
-    def send_command(self,server:str,command:str):
+
+    def send_command(self, server: str, command: str):
         url = f'{self.base_url}/api/client/servers/{server}/command'
         headers = {
-        "Authorization": f"Bearer {self.api_key}",
-        "Accept": "application/json",
-        "Content-Type": "application/json"
+            "Authorization": f"Bearer {self.api_key}",
+            "Accept": "application/json",
+            "Content-Type": "application/json"
         }
-        payload = '{"command": "awa"}'.replace("awa",command)
-        response = requests.request('POST',url,data=payload,headers=headers)
+        payload = '{"command": "awa"}'.replace("awa", command)
+        response = requests.request('POST', url, data=payload, headers=headers)
         return response
```

### Comparing `pteropy-0.1.6/pteropy.egg-info/PKG-INFO` & `pteropy-0.1.7/pteropy.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: pteropy
-Version: 0.1.6
+Version: 0.1.7
 Summary: 簡單存取Pterodactyl api
 Home-page: https://github.com/HansHans135/pteropy
-Author: seanbbear
+Author: Hans
 Author-email: ccoccc14@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # pteropy
 適用於Pterodactyl api的python庫
 
 # 安裝
 ```
 pip install pteropy
@@ -47,20 +48,20 @@
 
 ```py
 from pteropy import Pterodactyl_Application
 base_url = "https://面板網址"
 api_key = "api key"
 ptero = Pterodactyl_Application(base_url, api_key)
 
-#檢查api連線狀態
-ptero.check()
-#創建用戶
-ptero.create_user(username="用戶名",email="用戶email", password="密碼")
-#所有用戶
-ptero.list_users()
+
+ptero.check()  #檢查api連線狀態
+
+ptero.create_user(username="用戶名",email="用戶email", password="密碼")  #創建用戶
+
+ptero.list_users()  #所有用戶
 ```
 
 
 # Pterodactyl_Client範例
 key創建位置:/account/api
 
 ## 基本設置
@@ -85,28 +86,45 @@
 
 ```py
 from pteropy import Pterodactyl_Client
 base_url = "https://面板網址"
 api_key = "api key"
 ptero = Pterodactyl_Client(base_url, api_key)
 
-#檢查api連線狀態
-ptero.check()
-#獲得伺服器資料
-ptero.get_server("3fa3d78d")
-#獲得伺服器列表
-ptero.list_servers()
-#重命名伺服器
-ptero.rename_server("3fa3d78d","名子")
-#發送指令
-ptero.send_command("3fa3d78d","指令")
-
-#啟動伺服器
-ptero.start_server("3fa3d78d")
-#重啟伺服器
-ptero.restart_server("3fa3d78d")
-#關閉伺服器
-ptero.stop_server("3fa3d78d")
-#強制關閉伺服器
-ptero.kill_server("3fa3d78d")
+
+ptero.check()  #檢查api連線狀態
+
+ptero.account_details()  #帳戶資訊
+
+ptero.details_2FA()  #生成TOTP 二維碼圖像以允許設置 2FA
+
+ptero.enable_2FA()  #使用 details_2FA 請求生成的二維碼啟用 TOTP 2FA
+
+ptero.disable_2FA()  #禁用帳戶上的 TOTP 2FA
+
+ptero.update_email()  #更新帳戶的電子郵件位址
+
+ptero.update_password()  #更新帳戶的密碼
+
+ptero.list_API_keys()  #列出 API 金鑰
+
+ptero.create_API_key()  #生成新的 API 金鑰
+
+ptero.delete_API_key()  #刪除指定的 API 金鑰
+
+ptero.get_server("3fa3d78d")  #獲得伺服器資料
+
+ptero.list_servers()  #獲得伺服器列表
+
+ptero.rename_server("3fa3d78d","名子")  #重命名伺服器
+
+ptero.send_command("3fa3d78d","指令")  #發送指令
+
+ptero.start_server("3fa3d78d")  #啟動伺服器
+
+ptero.restart_server("3fa3d78d")  #重啟伺服器
+
+ptero.stop_server("3fa3d78d")  #關閉伺服器
+
+ptero.kill_server("3fa3d78d")  #強制關閉伺服器
 ```
```

### Comparing `pteropy-0.1.6/setup.py` & `pteropy-0.1.7/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 with open("README.md", "r",encoding="utf-8") as f:
     long_description = f.read()
     
 setuptools.setup(
     name = "pteropy",
-    version = "0.1.6",
-    author = "seanbbear",
+    version = "0.1.7",
+    author = "Hans",
     author_email="ccoccc14@gmail.com",
     description="簡單存取Pterodactyl api",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/HansHans135/pteropy",                                         
     packages=setuptools.find_packages(),     
     classifiers=[
```

