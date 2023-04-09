# Comparing `tmp/accesser-0.8.0rc1.tar.gz` & `tmp/accesser-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accesser-0.8.0rc1.tar", last modified: Sun Jan 29 05:51:49 2023, max compression
+gzip compressed data, was "accesser-0.8.1.tar", last modified: Sun Apr  9 13:04:10 2023, max compression
```

## Comparing `accesser-0.8.0rc1.tar` & `accesser-0.8.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-01-29 05:51:49.089090 accesser-0.8.0rc1/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    35147 2023-01-25 05:10:28.000000 accesser-0.8.0rc1/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3823 2023-01-29 05:51:49.089090 accesser-0.8.0rc1/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3229 2023-01-29 04:13:31.000000 accesser-0.8.0rc1/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-01-29 05:51:49.077090 accesser-0.8.0rc1/accesser/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7728 2023-01-29 01:33:21.000000 accesser-0.8.0rc1/accesser/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      110 2023-01-29 01:22:09.000000 accesser-0.8.0rc1/accesser/__main__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6634 2023-01-25 09:16:13.000000 accesser-0.8.0rc1/accesser/config.toml
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2105 2023-01-25 05:10:28.000000 accesser-0.8.0rc1/accesser/pac
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-01-29 05:51:49.089090 accesser-0.8.0rc1/accesser/utils/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-25 05:10:28.000000 accesser-0.8.0rc1/accesser/utils/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1937 2023-01-25 05:10:28.000000 accesser-0.8.0rc1/accesser/utils/cert_verify.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3619 2023-01-28 13:43:50.000000 accesser-0.8.0rc1/accesser/utils/certmanager.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4363 2023-01-25 05:10:28.000000 accesser-0.8.0rc1/accesser/utils/importca.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      570 2023-01-25 09:11:59.000000 accesser-0.8.0rc1/accesser/utils/log.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      720 2023-01-28 13:43:45.000000 accesser-0.8.0rc1/accesser/utils/setting.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      812 2023-01-25 05:10:28.000000 accesser-0.8.0rc1/accesser/utils/sysproxy.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-01-29 05:51:49.077090 accesser-0.8.0rc1/accesser.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3823 2023-01-29 05:51:49.000000 accesser-0.8.0rc1/accesser.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      491 2023-01-29 05:51:49.000000 accesser-0.8.0rc1/accesser.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-01-29 05:51:49.000000 accesser-0.8.0rc1/accesser.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       42 2023-01-29 05:51:49.000000 accesser-0.8.0rc1/accesser.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       48 2023-01-29 05:51:49.000000 accesser-0.8.0rc1/accesser.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        9 2023-01-29 05:51:49.000000 accesser-0.8.0rc1/accesser.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      872 2023-01-29 04:13:14.000000 accesser-0.8.0rc1/pyproject.toml
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-01-29 05:51:49.089090 accesser-0.8.0rc1/setup.cfg
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-09 13:04:10.321170 accesser-0.8.1/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    35147 2023-01-25 05:10:28.000000 accesser-0.8.1/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3595 2023-04-09 13:04:10.321170 accesser-0.8.1/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3004 2023-04-09 13:00:08.000000 accesser-0.8.1/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-09 13:04:10.317170 accesser-0.8.1/accesser/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8334 2023-04-09 12:52:48.000000 accesser-0.8.1/accesser/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      110 2023-01-29 01:22:09.000000 accesser-0.8.1/accesser/__main__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6985 2023-04-02 08:16:41.000000 accesser-0.8.1/accesser/config.toml
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2207 2023-04-02 08:09:43.000000 accesser-0.8.1/accesser/pac
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-09 13:04:10.321170 accesser-0.8.1/accesser/utils/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-25 05:10:28.000000 accesser-0.8.1/accesser/utils/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1937 2023-01-25 05:10:28.000000 accesser-0.8.1/accesser/utils/cert_verify.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3619 2023-01-28 13:43:50.000000 accesser-0.8.1/accesser/utils/certmanager.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4363 2023-01-25 05:10:28.000000 accesser-0.8.1/accesser/utils/importca.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      570 2023-01-25 09:11:59.000000 accesser-0.8.1/accesser/utils/log.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      785 2023-04-01 14:10:46.000000 accesser-0.8.1/accesser/utils/setting.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1003 2023-01-30 05:39:03.000000 accesser-0.8.1/accesser/utils/sysproxy.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-09 13:04:10.317170 accesser-0.8.1/accesser.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3595 2023-04-09 13:04:10.000000 accesser-0.8.1/accesser.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      491 2023-04-09 13:04:10.000000 accesser-0.8.1/accesser.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-04-09 13:04:10.000000 accesser-0.8.1/accesser.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       42 2023-04-09 13:04:10.000000 accesser-0.8.1/accesser.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       89 2023-04-09 13:04:10.000000 accesser-0.8.1/accesser.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        9 2023-04-09 13:04:10.000000 accesser-0.8.1/accesser.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      916 2023-04-09 12:52:48.000000 accesser-0.8.1/pyproject.toml
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-04-09 13:04:10.321170 accesser-0.8.1/setup.cfg
```

### Comparing `accesser-0.8.0rc1/LICENSE` & `accesser-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `accesser-0.8.0rc1/PKG-INFO` & `accesser-0.8.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,53 +1,51 @@
 Metadata-Version: 2.1
 Name: accesser
-Version: 0.8.0rc1
+Version: 0.8.1
 Summary: 🌏一个解决SNI RST导致维基百科、Pixiv等站点无法访问的工具 | A tool for solving SNI RST
 Author: URenko
 Project-URL: Homepage, https://github.com/URenko/Accesser
 Project-URL: Bug Tracker, https://github.com/URenko/Accesser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: doh
 License-File: LICENSE
 
 # Accesser
 [English version](README.en.md)
 
 一个解决SNI RST导致维基百科、Pixiv等站点无法访问的工具  
 [支持的站点](https://github.com/URenko/Accesser/wiki/目前支持的站点)
 
 [![](https://img.shields.io/github/release/URenko/Accesser.svg)](https://github.com/URenko/Accesser/releases/latest)
+[![](https://img.shields.io/pypi/v/accesser)](https://pypi.org/project/accesser/)
 [![](https://img.shields.io/github/downloads/URenko/Accesser/total.svg)](https://github.com/URenko/Accesser/releases/latest)
 [![](https://img.shields.io/github/license/URenko/Accesser.svg)](https://github.com/URenko/Accesser/blob/master/LICENSE)
 
 ## 使用
 ### 如果不知道什么是Python
-从[这里](https://github.com/URenko/Accesser/releases/download/v0.8.0rc1/accesser.exe)下载Windows一键程序，运行既可，首次使用会要求安装证书，选是即可。
-### 如果已经安装了Python 3.11*或更高版本
+从[这里](https://github.com/URenko/Accesser/releases/download/v0.8.1/accesser.exe)下载Windows一键程序，运行既可，首次使用会要求安装证书，选是即可。
+### 如果已经安装了Python 3.10*或更高版本
 ```
-pip3 install git+https://github.com/URenko/Accesser.git
+pip3 install -U accesser[doh]
 ```
-如果要使用DNS-over-HTTPS，需要使用`pip install httpx[http2]`安装`httpx`。
+如果你不需要DNS-over-HTTPS，则可以不用带`[doh]`。
 
 然后通过如下命令启动：
 ```
 accesser
 ```
 对于Windows系统，默认情况下（没有指定`--notsetproxy`）会设置PAC代理为`http://localhost:7654/pac/?t=<随机数>`，如果没有可以手动设置。
 
 此外，对于Windows系统，默认情况下（没有指定`--notimportca`）会自动导入证书至系统，如果没有可以手动导入，请看[这里](https://github.com/URenko/Accesser/wiki/FAQ#q-windows%E8%AE%BF%E9%97%AE%E7%9B%B8%E5%85%B3%E7%BD%91%E7%AB%99%E5%87%BA%E7%8E%B0%E8%AF%81%E4%B9%A6%E9%94%99%E8%AF%AF%E6%82%A8%E7%9A%84%E8%BF%9E%E6%8E%A5%E4%B8%8D%E6%98%AF%E7%A7%81%E5%AF%86%E8%BF%9E%E6%8E%A5neterr_cert_invalid%E4%B9%8B%E7%B1%BB%E7%9A%84%E6%80%8E%E4%B9%88%E5%8A%9E%E8%AF%81%E4%B9%A6%E5%AF%BC%E5%85%A5%E9%94%99%E8%AF%AF%E6%80%8E%E4%B9%88%E5%8A%9E%E5%A6%82%E4%BD%95%E5%8D%B8%E8%BD%BD%E8%AF%81%E4%B9%A6)。
 
-#### *为什么所需的python最低版本是3.11?
-为了能优雅地用协程将socket连接升级为TLS连接，需要[asyncio.StreamWriter.start_tls()](https://docs.python.org/zh-cn/3/library/asyncio-stream.html#asyncio.StreamWriter.start_tls)，这一功能到python 3.11才提供。
-
-可以使用例如[pyenv](https://github.com/pyenv/pyenv)来安装python 3.11。
+*可以使用例如[pyenv](https://github.com/pyenv/pyenv)来安装所需的Python版本（推荐Python 3.11）。
 
 ## 设置
 编辑工作目录下的`config.toml`，具体含义见其中注释，保存后重新打开程序。
 
 ## 进阶1: 与v2ray等其他代理软件一起使用
 Accesser是一个本地HTTP代理，默认代理地址为`http://localhost:7654`，只要网络流量能从其他代理软件以HTTP代理导出就能联合使用。
```

### Comparing `accesser-0.8.0rc1/README.md` & `accesser-0.8.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 # Accesser
 [English version](README.en.md)
 
 一个解决SNI RST导致维基百科、Pixiv等站点无法访问的工具  
 [支持的站点](https://github.com/URenko/Accesser/wiki/目前支持的站点)
 
 [![](https://img.shields.io/github/release/URenko/Accesser.svg)](https://github.com/URenko/Accesser/releases/latest)
+[![](https://img.shields.io/pypi/v/accesser)](https://pypi.org/project/accesser/)
 [![](https://img.shields.io/github/downloads/URenko/Accesser/total.svg)](https://github.com/URenko/Accesser/releases/latest)
 [![](https://img.shields.io/github/license/URenko/Accesser.svg)](https://github.com/URenko/Accesser/blob/master/LICENSE)
 
 ## 使用
 ### 如果不知道什么是Python
-从[这里](https://github.com/URenko/Accesser/releases/download/v0.8.0rc1/accesser.exe)下载Windows一键程序，运行既可，首次使用会要求安装证书，选是即可。
-### 如果已经安装了Python 3.11*或更高版本
+从[这里](https://github.com/URenko/Accesser/releases/download/v0.8.1/accesser.exe)下载Windows一键程序，运行既可，首次使用会要求安装证书，选是即可。
+### 如果已经安装了Python 3.10*或更高版本
 ```
-pip3 install git+https://github.com/URenko/Accesser.git
+pip3 install -U accesser[doh]
 ```
-如果要使用DNS-over-HTTPS，需要使用`pip install httpx[http2]`安装`httpx`。
+如果你不需要DNS-over-HTTPS，则可以不用带`[doh]`。
 
 然后通过如下命令启动：
 ```
 accesser
 ```
 对于Windows系统，默认情况下（没有指定`--notsetproxy`）会设置PAC代理为`http://localhost:7654/pac/?t=<随机数>`，如果没有可以手动设置。
 
 此外，对于Windows系统，默认情况下（没有指定`--notimportca`）会自动导入证书至系统，如果没有可以手动导入，请看[这里](https://github.com/URenko/Accesser/wiki/FAQ#q-windows%E8%AE%BF%E9%97%AE%E7%9B%B8%E5%85%B3%E7%BD%91%E7%AB%99%E5%87%BA%E7%8E%B0%E8%AF%81%E4%B9%A6%E9%94%99%E8%AF%AF%E6%82%A8%E7%9A%84%E8%BF%9E%E6%8E%A5%E4%B8%8D%E6%98%AF%E7%A7%81%E5%AF%86%E8%BF%9E%E6%8E%A5neterr_cert_invalid%E4%B9%8B%E7%B1%BB%E7%9A%84%E6%80%8E%E4%B9%88%E5%8A%9E%E8%AF%81%E4%B9%A6%E5%AF%BC%E5%85%A5%E9%94%99%E8%AF%AF%E6%80%8E%E4%B9%88%E5%8A%9E%E5%A6%82%E4%BD%95%E5%8D%B8%E8%BD%BD%E8%AF%81%E4%B9%A6)。
 
-#### *为什么所需的python最低版本是3.11?
-为了能优雅地用协程将socket连接升级为TLS连接，需要[asyncio.StreamWriter.start_tls()](https://docs.python.org/zh-cn/3/library/asyncio-stream.html#asyncio.StreamWriter.start_tls)，这一功能到python 3.11才提供。
-
-可以使用例如[pyenv](https://github.com/pyenv/pyenv)来安装python 3.11。
+*可以使用例如[pyenv](https://github.com/pyenv/pyenv)来安装所需的Python版本（推荐Python 3.11）。
 
 ## 设置
 编辑工作目录下的`config.toml`，具体含义见其中注释，保存后重新打开程序。
 
 ## 进阶1: 与v2ray等其他代理软件一起使用
 Accesser是一个本地HTTP代理，默认代理地址为`http://localhost:7654`，只要网络流量能从其他代理软件以HTTP代理导出就能联合使用。
```

### Comparing `accesser-0.8.0rc1/accesser/__init__.py` & `accesser-0.8.1/accesser/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,17 +12,18 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-__version__ = '0.8.0rc1'
+__version__ = '0.8.1'
 
 import os, sys
+import json
 import random
 import ssl
 import asyncio
 import traceback
 from contextlib import closing
 from urllib import request
 from pkg_resources import parse_version
@@ -31,14 +32,15 @@
 
 from .utils import certmanager as cm
 from .utils import importca
 from .utils import setting
 from .utils.setting import basepath
 from .utils.log import logger
 from .utils.cert_verify import match_hostname
+from .utils import sysproxy
 
 
 async def update_cert(server_name):
     global context, cert_store, cert_lock
     res = get_tld(server_name, as_object=True, fix_protocol=True)
     if res.subdomain:
         server_name = res.subdomain.split('.', 1)[-1] + '.' + res.domain + '.' + res.tld
@@ -48,38 +50,41 @@
         if not server_name in cert_store:
             cm.create_certificate(server_name)
         context.load_cert_chain(os.path.join(cm.certpath, "{}.crt".format(server_name)))
         cert_store.add(server_name)
 
 async def send_pac(writer: asyncio.StreamWriter):
     with open('pac' if os.path.exists('pac') else os.path.join(basepath, 'pac'), 'rb') as f:
-        pac = f.read().replace(b'{{port}}', str(setting.config['server']['port']).encode('iso-8859-1'))
+        pac = f.read().replace(b'{{port}}', str(setting.config['server']['port']).encode('iso-8859-1')).replace(b'{{host}}', setting.config['server'].get('pac_host', '127.0.0.1').encode('iso-8859-1'))
     writer.write(f'HTTP/1.1 200 OK\r\nContent-Type: application/x-ns-proxy-autoconfig\r\nContent-Length: {len(pac)}\r\n\r\n'.encode('iso-8859-1'))
     writer.write(pac)
     await writer.drain()
     writer.close()
+    await writer.wait_closed()
 
 async def send_crt(writer: asyncio.StreamWriter, path: str):
     with open(os.path.join(basepath, path.lstrip('/')), 'rb') as f:
         crt = f.read()
     writer.write(f'HTTP/1.1 200 OK\r\nContent-Type: application/x-x509-ca-cert\r\nContent-Length: {len(crt)}\r\n\r\n'.encode('iso-8859-1'))
     writer.write(crt)
     await writer.drain()
     writer.close()
+    await writer.wait_closed()
     
 async def http_redirect(writer: asyncio.StreamWriter, path: str):
     path = path.removeprefix('http://')
     for key in setting.config['http_redirect']:
         if path.startswith(key):
             path = setting.config['http_redirect'][key] + path[len(key):]
             break
     logger.debug('Redirect to '+path)
     writer.write(f'HTTP/1.1 301 Moved Permanently\r\nLocation: https://{path}\r\n\r\n'.encode('iso-8859-1'))
     await writer.drain()
     writer.close()
+    await writer.wait_closed()
 
 async def forward_stream(reader: asyncio.StreamReader, writer: asyncio.StreamWriter):
     while True:
         data = await reader.read(32768)
         if data == b'':
             return
         writer.write(data)
@@ -109,15 +114,18 @@
                 else:
                     return await http_redirect(writer, path)
             case _:
                 return await http_redirect(writer, path)
         writer.write(b'HTTP/1.1 200 Connection Established\r\n\r\n')
 
         await update_cert(host)
-        await writer.start_tls(context)
+        if sys.version_info[1] >= 11:
+            await writer.start_tls(context)
+        else:
+            writer._transport = await writer._loop.start_tls(writer.transport, writer._protocol, context, server_side=True)
         server_hostname = setting.config['alter_hostname'].get(host, '')
         logger.debug(f'[{i_port:5}] {server_hostname=}')
         remote_context = ssl.create_default_context()
         remote_context.check_hostname = False
         remote_reader, remote_writer = await asyncio.open_connection(remote_ip, port, ssl=remote_context, server_hostname=server_hostname)
         cert = remote_writer.get_extra_info('peercert')
         logger.debug(f"[{i_port:5}] {cert.get('subjectAltName', ())=}")
@@ -128,25 +136,30 @@
                 logger.warning(f'[{i_port:5}] {err}')
                 return
         
         await asyncio.gather(
             forward_stream(reader, remote_writer),
             forward_stream(remote_reader, writer)
         )
+    writer.close()
+    remote_writer.close()
+    await remote_writer.wait_closed()
+    await writer.wait_closed()
 
 async def proxy():
     server = await asyncio.start_server(handle, setting.config['server']['address'], setting.config['server']['port'])
 
     print(f"Serving on {', '.join(str(sock.getsockname()) for sock in server.sockets)}")
-    if setting.config['setproxy'] and sys.platform.startswith('win'):
-        from .utils import sysproxy
-        sysproxy.set_pac('http://localhost:'+str(setting.config['server']['port'])+'/pac/?t='+str(random.randrange(2**16)))
+    sysproxy.set_pac('http://localhost:'+str(setting.config['server']['port'])+'/pac/?t='+str(random.randrange(2**16)))
 
-    async with server:
-        await server.serve_forever()
+    try:
+        async with server:
+            await server.serve_forever()
+    finally:
+        sysproxy.set_pac(None)
 
 async def DNSquery(domain):
     global DNSresolver
     try:
         return next(v for k,v in setting.config['hosts'].items() if k==domain or (k.startswith('.') and domain.endswith(k)))
     except StopIteration: pass
     if setting.config['ipv6']:
@@ -155,40 +168,44 @@
         except dns.asyncresolver.NoAnswer:
             ret = await DNSresolver.resolve(domain, 'A')
     else:
         ret = await DNSresolver.resolve(domain, 'A')
     return ret[0].to_text()
 
 def update_checker():
-    try:
+    for pypi_url in ['https://pypi.org/pypi/accesser/json', 'https://mirrors.cloud.tencent.com/pypi/json/accesser']:
+        try:
+            with request.urlopen(pypi_url) as f:
+                v2 = parse_version(json.load(f)["info"]["version"])
+                break
+        except Exception:
+            logger.warning(traceback.format_exc())
+    else:
         with request.urlopen('https://github.com/URenko/Accesser/releases/latest') as f:
             v2 = parse_version(f.geturl().rsplit('/', maxsplit=1)[-1])
-            v1 = parse_version(__version__)
-            if v2 > v1:
-                logger.warning('There is a new version, check {} for update.'.format(f.geturl()))
-    except Exception:
-        logger.warning('Check for update failure, please check manually.')
-        logger.warning(traceback.format_exc())
+    v1 = parse_version(__version__)
+    if v2 > v1:
+        logger.warning("There is a new version, you can update with 'python3 -m pip install -U accesser' or download from GitHub")
 
 async def main():
     global context, cert_store, cert_lock, DNSresolver
     print(f"Accesser v{__version__}  Copyright (C) 2018-2023  URenko")
     setting.parse_args()
-    
-    async with asyncio.TaskGroup() as tg:
-        tg.create_task(asyncio.to_thread(update_checker))
-        
-        DNSresolver = dns.asyncresolver.Resolver(configure=False)
-        DNSresolver.cache = dns.resolver.LRUCache()
-        DNSresolver.nameservers = setting.config['DNS']['nameserver']
-        DNSresolver.port = int(setting.config['DNS']['port'])
         
-        importca.import_ca()
+    DNSresolver = dns.asyncresolver.Resolver(configure=False)
+    DNSresolver.cache = dns.resolver.LRUCache()
+    DNSresolver.nameservers = setting.config['DNS']['nameserver']
+    DNSresolver.port = int(setting.config['DNS']['port'])
+    
+    importca.import_ca()
 
-        context = ssl.SSLContext(ssl.PROTOCOL_TLS_SERVER)
-        cert_store = set()
-        cert_lock = asyncio.Lock()
-        
-        tg.create_task(proxy())
+    context = ssl.SSLContext(ssl.PROTOCOL_TLS_SERVER)
+    cert_store = set()
+    cert_lock = asyncio.Lock()
+    
+    await asyncio.gather(
+        asyncio.to_thread(update_checker),
+        proxy()
+    )
 
 def run():
     asyncio.run(main())
```

### Comparing `accesser-0.8.0rc1/accesser/config.toml` & `accesser-0.8.1/accesser/config.toml`

 * *Files 3% similar despite different names*

```diff
@@ -35,14 +35,18 @@
 # The address to which the server is bound. Set to "0.0.0.0" to allow devices on the same LAN to connect to the program, such as using your phone to connect to your computer's WiFi, after setting the PAC to allow both your phone to use it. There may be a firewall prompt to allow access.
 address = "127.0.0.1"
 
 # 服务器的端口号，如果与其他程序发生端口冲突时可以更改，其值应为1-65535，建议>1024。
 # The port number of the server, which can be changed in case of port conflicts with other programs, should have a value of 1-65535, with >1024 recommended.
 port = 7654
 
+# PAC文件中的代理主机。如供局域网使用，应设为安装了Accesser的设备在局域网中的IP。
+# The proxy host in the PAC file. If for LAN usage, it should be set to the IP of the device on the LAN where Accesser is installed.
+pac_host = "127.0.0.1"
+
 
 [DNS]
 
 # DNS服务器地址。如果以 https:// 开头，则使用DNS-over-HTTPS (DoH)，否则是传统的UDP DNS。
 # DNS server address. If it starts with https://, then DNS-over-HTTPS (DoH) is used, otherwise it is a traditional UDP DNS.
 nameserver = [
   "https://firefox.cloudflare-dns.com/dns-query",
@@ -78,14 +82,15 @@
 "sketch.pixiv.net" = "pixivsketch.net"
 "cdn1-smallimg.phncdn.com" = "pabbp.com"
 "nyaa.si" = "ddos-guard.net"
 "site.nicovideo.jp" = "d4fsvsnk8os9s.cloudfront.net"
 "blog.nicovideo.jp" = "d11c2xcc0ucqv1.cloudfront.net"
 "info.nicovideo.jp" = "d2c1o7y4lmdvf6.cloudfront.net"
 "www.ftchinese.com" = "dsiij4vzr462k.cloudfront.net"
+"pipelines.actions.githubusercontent.com" = "origin.mediaservices.windows.net"
 
 
 [hosts]
 
 # 连接键所对应的域名时使用值所对应的IP。此设置优先于上面的DNS服务器设置。
 # When connecting the domain name corresponding to the key, use the IP corresponding to the value. This setting takes precedence over the DNS server setting above.
```

### Comparing `accesser-0.8.0rc1/accesser/pac` & `accesser-0.8.1/accesser/pac`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,17 @@
   "dropbox-dns.com": 1,
   "dw.com": 1,
   "e-hentai.org": 1,
   "epochtimes.com": 1,
   "euronews.com": 1,
   "exhentai.org": 1,
   "ftchinese.com": 1,
+  "github.com": 1,
+  "githubassets.com": 1,
+  "githubusercontent.com": 1,
   "imgur.com": 1,
   "instagram.com": 1,
   "i.pximg.net": 1,
   "kobo.com": 1,
   "medium.com": 1,
   "mega.nz": 1,
   "nicovideo.jp": 1,
@@ -42,26 +45,27 @@
   "uptodown.com": 1,
   "vimeo.com": 1,
   "wenxuecity.com": 1,
   "wikipedia.org": 1
 };
 
 var shexps = {
+  "*://api.openai.com/*": 1,
   "*://steamcommunity-a.akamaihd.net/*": 1,
   "*://steamuserimages-a.akamaihd.net/*": 1,
   "*://*.amazon.co.jp/*": 1,
   "*://*onedrive.live.com/*": 1,
   "*://*.bbc.co.uk/*": 1,
   "*://*.bbci.co.uk/*": 1,
   "*://*.japantimes.co.jp/*": 1,
   "*://*.yahoo.co.jp/*": 1,
   "*://*.cna.com.tw/*": 1
 };
 
-var proxy = "PROXY 127.0.0.1:{{port}};";
+var proxy = "PROXY {{host}}:{{port}};";
 
 var direct = 'DIRECT;';
 
 var hasOwnProperty = Object.hasOwnProperty;
 
 function shExpMatchs(str, shexps) {
     for (shexp in shexps) {
```

### Comparing `accesser-0.8.0rc1/accesser/utils/cert_verify.py` & `accesser-0.8.1/accesser/utils/cert_verify.py`

 * *Files identical despite different names*

### Comparing `accesser-0.8.0rc1/accesser/utils/certmanager.py` & `accesser-0.8.1/accesser/utils/certmanager.py`

 * *Files identical despite different names*

### Comparing `accesser-0.8.0rc1/accesser/utils/importca.py` & `accesser-0.8.1/accesser/utils/importca.py`

 * *Files identical despite different names*

### Comparing `accesser-0.8.0rc1/accesser/utils/log.py` & `accesser-0.8.1/accesser/utils/log.py`

 * *Files identical despite different names*

### Comparing `accesser-0.8.0rc1/accesser/utils/setting.py` & `accesser-0.8.1/accesser/utils/setting.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 from pathlib import Path
 import shutil
-import tomllib
+try:
+    import tomllib
+except ModuleNotFoundError:
+    import tomli as tomllib
 import argparse
 
 basepath = Path(__file__).parent.parent
 
 if not Path('config.toml').exists():
     shutil.copyfile(basepath / 'config.toml', 'config.toml')
 with open('config.toml', 'rb') as f:
```

### Comparing `accesser-0.8.0rc1/accesser/utils/sysproxy.py` & `accesser-0.8.1/accesser/utils/sysproxy.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,23 @@
-from ctypes import windll
-import winreg
+import sys
+from . import setting
+
+if sys.platform.startswith('win'):
+    from ctypes import windll
+    import winreg
 
 #TODO: use Windows API instead of winreg, see https://github.com/Noisyfox/sysproxy for example.
 
 def set_pac(pac):
-    with winreg.OpenKey(winreg.HKEY_CURRENT_USER,
-                                    r'Software\Microsoft\Windows\CurrentVersion\Internet Settings',
-                                    0, winreg.KEY_ALL_ACCESS) as INTERNET_SETTINGS:
-        if pac is None:
-            winreg.DeleteValue(INTERNET_SETTINGS, 'AutoConfigURL')
-        else:
-            winreg.SetValueEx(INTERNET_SETTINGS, 'AutoConfigURL', 0, winreg.REG_SZ, pac)
+    if setting.config['setproxy'] and sys.platform.startswith('win'):
+        with winreg.OpenKey(winreg.HKEY_CURRENT_USER,
+                                        r'Software\Microsoft\Windows\CurrentVersion\Internet Settings',
+                                        0, winreg.KEY_ALL_ACCESS) as INTERNET_SETTINGS:
+            if pac is None:
+                winreg.DeleteValue(INTERNET_SETTINGS, 'AutoConfigURL')
+            else:
+                winreg.SetValueEx(INTERNET_SETTINGS, 'AutoConfigURL', 0, winreg.REG_SZ, pac)
 
-    INTERNET_OPTION_REFRESH = 37
-    INTERNET_OPTION_SETTINGS_CHANGED = 39
-    windll.Wininet.InternetSetOptionW(0, INTERNET_OPTION_REFRESH, 0, 0)
-    windll.Wininet.InternetSetOptionW(0, INTERNET_OPTION_SETTINGS_CHANGED, 0, 0)
+        INTERNET_OPTION_REFRESH = 37
+        INTERNET_OPTION_SETTINGS_CHANGED = 39
+        windll.Wininet.InternetSetOptionW(0, INTERNET_OPTION_REFRESH, 0, 0)
+        windll.Wininet.InternetSetOptionW(0, INTERNET_OPTION_SETTINGS_CHANGED, 0, 0)
```

### Comparing `accesser-0.8.0rc1/accesser.egg-info/PKG-INFO` & `accesser-0.8.1/accesser.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,53 +1,51 @@
 Metadata-Version: 2.1
 Name: accesser
-Version: 0.8.0rc1
+Version: 0.8.1
 Summary: 🌏一个解决SNI RST导致维基百科、Pixiv等站点无法访问的工具 | A tool for solving SNI RST
 Author: URenko
 Project-URL: Homepage, https://github.com/URenko/Accesser
 Project-URL: Bug Tracker, https://github.com/URenko/Accesser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: doh
 License-File: LICENSE
 
 # Accesser
 [English version](README.en.md)
 
 一个解决SNI RST导致维基百科、Pixiv等站点无法访问的工具  
 [支持的站点](https://github.com/URenko/Accesser/wiki/目前支持的站点)
 
 [![](https://img.shields.io/github/release/URenko/Accesser.svg)](https://github.com/URenko/Accesser/releases/latest)
+[![](https://img.shields.io/pypi/v/accesser)](https://pypi.org/project/accesser/)
 [![](https://img.shields.io/github/downloads/URenko/Accesser/total.svg)](https://github.com/URenko/Accesser/releases/latest)
 [![](https://img.shields.io/github/license/URenko/Accesser.svg)](https://github.com/URenko/Accesser/blob/master/LICENSE)
 
 ## 使用
 ### 如果不知道什么是Python
-从[这里](https://github.com/URenko/Accesser/releases/download/v0.8.0rc1/accesser.exe)下载Windows一键程序，运行既可，首次使用会要求安装证书，选是即可。
-### 如果已经安装了Python 3.11*或更高版本
+从[这里](https://github.com/URenko/Accesser/releases/download/v0.8.1/accesser.exe)下载Windows一键程序，运行既可，首次使用会要求安装证书，选是即可。
+### 如果已经安装了Python 3.10*或更高版本
 ```
-pip3 install git+https://github.com/URenko/Accesser.git
+pip3 install -U accesser[doh]
 ```
-如果要使用DNS-over-HTTPS，需要使用`pip install httpx[http2]`安装`httpx`。
+如果你不需要DNS-over-HTTPS，则可以不用带`[doh]`。
 
 然后通过如下命令启动：
 ```
 accesser
 ```
 对于Windows系统，默认情况下（没有指定`--notsetproxy`）会设置PAC代理为`http://localhost:7654/pac/?t=<随机数>`，如果没有可以手动设置。
 
 此外，对于Windows系统，默认情况下（没有指定`--notimportca`）会自动导入证书至系统，如果没有可以手动导入，请看[这里](https://github.com/URenko/Accesser/wiki/FAQ#q-windows%E8%AE%BF%E9%97%AE%E7%9B%B8%E5%85%B3%E7%BD%91%E7%AB%99%E5%87%BA%E7%8E%B0%E8%AF%81%E4%B9%A6%E9%94%99%E8%AF%AF%E6%82%A8%E7%9A%84%E8%BF%9E%E6%8E%A5%E4%B8%8D%E6%98%AF%E7%A7%81%E5%AF%86%E8%BF%9E%E6%8E%A5neterr_cert_invalid%E4%B9%8B%E7%B1%BB%E7%9A%84%E6%80%8E%E4%B9%88%E5%8A%9E%E8%AF%81%E4%B9%A6%E5%AF%BC%E5%85%A5%E9%94%99%E8%AF%AF%E6%80%8E%E4%B9%88%E5%8A%9E%E5%A6%82%E4%BD%95%E5%8D%B8%E8%BD%BD%E8%AF%81%E4%B9%A6)。
 
-#### *为什么所需的python最低版本是3.11?
-为了能优雅地用协程将socket连接升级为TLS连接，需要[asyncio.StreamWriter.start_tls()](https://docs.python.org/zh-cn/3/library/asyncio-stream.html#asyncio.StreamWriter.start_tls)，这一功能到python 3.11才提供。
-
-可以使用例如[pyenv](https://github.com/pyenv/pyenv)来安装python 3.11。
+*可以使用例如[pyenv](https://github.com/pyenv/pyenv)来安装所需的Python版本（推荐Python 3.11）。
 
 ## 设置
 编辑工作目录下的`config.toml`，具体含义见其中注释，保存后重新打开程序。
 
 ## 进阶1: 与v2ray等其他代理软件一起使用
 Accesser是一个本地HTTP代理，默认代理地址为`http://localhost:7654`，只要网络流量能从其他代理软件以HTTP代理导出就能联合使用。
```

### Comparing `accesser-0.8.0rc1/pyproject.toml` & `accesser-0.8.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "accesser"
-version = "0.8.0rc1"
+version = "0.8.1"
 authors = [
   { name="URenko" },
 ]
 description = "🌏一个解决SNI RST导致维基百科、Pixiv等站点无法访问的工具 | A tool for solving SNI RST"
 readme = "README.md"
-requires-python = ">=3.11"
+requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "pyopenssl",
     'tld',
     'dnspython < 2.4',
+    'tomli >= 1.1.0 ; python_version < "3.11"'
 ]
 
 [project.optional-dependencies]
 doh = ["httpx[http2]"]
 
 [project.scripts]
 accesser = "accesser:run"
```

