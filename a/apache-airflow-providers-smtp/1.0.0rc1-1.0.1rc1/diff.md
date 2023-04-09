# Comparing `tmp/apache-airflow-providers-smtp-1.0.0rc1.tar.gz` & `tmp/apache-airflow-providers-smtp-1.0.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-smtp-1.0.0rc1.tar", last modified: Sun Apr  2 05:49:16 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-smtp-1.0.1rc1.tar", last modified: Sun Apr  9 13:49:56 2023, max compression
```

## Comparing `apache-airflow-providers-smtp-1.0.0rc1.tar` & `apache-airflow-providers-smtp-1.0.1rc1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:49:16.000000 apache-airflow-providers-smtp-1.0.0rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-smtp-1.0.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1122 2023-04-02 05:49:14.000000 apache-airflow-providers-smtp-1.0.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-smtp-1.0.0rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     4509 2023-04-02 05:49:16.000000 apache-airflow-providers-smtp-1.0.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2988 2023-04-02 05:49:14.000000 apache-airflow-providers-smtp-1.0.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:49:15.000000 apache-airflow-providers-smtp-1.0.0rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:49:15.000000 apache-airflow-providers-smtp-1.0.0rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:49:15.000000 apache-airflow-providers-smtp-1.0.0rc1/airflow/providers/smtp/
--rw-r--r--   0 root         (0) root         (0)      787 2023-03-15 08:58:48.000000 apache-airflow-providers-smtp-1.0.0rc1/airflow/providers/smtp/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2251 2023-04-02 05:49:14.000000 apache-airflow-providers-smtp-1.0.0rc1/airflow/providers/smtp/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:49:15.000000 apache-airflow-providers-smtp-1.0.0rc1/airflow/providers/smtp/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-03-15 08:58:48.000000 apache-airflow-providers-smtp-1.0.0rc1/airflow/providers/smtp/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13813 2023-03-15 08:58:48.000000 apache-airflow-providers-smtp-1.0.0rc1/airflow/providers/smtp/hooks/smtp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:49:15.000000 apache-airflow-providers-smtp-1.0.0rc1/airflow/providers/smtp/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-03-15 08:58:48.000000 apache-airflow-providers-smtp-1.0.0rc1/airflow/providers/smtp/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3385 2023-03-15 08:58:48.000000 apache-airflow-providers-smtp-1.0.0rc1/airflow/providers/smtp/operators/smtp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:49:16.000000 apache-airflow-providers-smtp-1.0.0rc1/apache_airflow_providers_smtp.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4509 2023-04-02 05:49:15.000000 apache-airflow-providers-smtp-1.0.0rc1/apache_airflow_providers_smtp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      686 2023-04-02 05:49:15.000000 apache-airflow-providers-smtp-1.0.0rc1/apache_airflow_providers_smtp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-02 05:49:15.000000 apache-airflow-providers-smtp-1.0.0rc1/apache_airflow_providers_smtp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      101 2023-04-02 05:49:15.000000 apache-airflow-providers-smtp-1.0.0rc1/apache_airflow_providers_smtp.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-02 05:49:15.000000 apache-airflow-providers-smtp-1.0.0rc1/apache_airflow_providers_smtp.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       27 2023-04-02 05:49:15.000000 apache-airflow-providers-smtp-1.0.0rc1/apache_airflow_providers_smtp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-02 05:49:15.000000 apache-airflow-providers-smtp-1.0.0rc1/apache_airflow_providers_smtp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5393 2023-04-01 16:40:04.000000 apache-airflow-providers-smtp-1.0.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1816 2023-04-02 05:49:16.000000 apache-airflow-providers-smtp-1.0.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1456 2023-04-02 05:49:14.000000 apache-airflow-providers-smtp-1.0.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:49:56.000000 apache-airflow-providers-smtp-1.0.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-smtp-1.0.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-04-09 13:49:54.000000 apache-airflow-providers-smtp-1.0.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-smtp-1.0.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     4888 2023-04-09 13:49:56.000000 apache-airflow-providers-smtp-1.0.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3367 2023-04-09 13:49:54.000000 apache-airflow-providers-smtp-1.0.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:49:56.000000 apache-airflow-providers-smtp-1.0.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:49:56.000000 apache-airflow-providers-smtp-1.0.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:49:56.000000 apache-airflow-providers-smtp-1.0.1rc1/airflow/providers/smtp/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-03-15 08:58:48.000000 apache-airflow-providers-smtp-1.0.1rc1/airflow/providers/smtp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2288 2023-04-09 13:49:54.000000 apache-airflow-providers-smtp-1.0.1rc1/airflow/providers/smtp/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:49:56.000000 apache-airflow-providers-smtp-1.0.1rc1/airflow/providers/smtp/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-03-15 08:58:48.000000 apache-airflow-providers-smtp-1.0.1rc1/airflow/providers/smtp/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13824 2023-04-07 21:10:19.000000 apache-airflow-providers-smtp-1.0.1rc1/airflow/providers/smtp/hooks/smtp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:49:56.000000 apache-airflow-providers-smtp-1.0.1rc1/airflow/providers/smtp/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-03-15 08:58:48.000000 apache-airflow-providers-smtp-1.0.1rc1/airflow/providers/smtp/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3434 2023-04-09 06:57:27.000000 apache-airflow-providers-smtp-1.0.1rc1/airflow/providers/smtp/operators/smtp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:49:56.000000 apache-airflow-providers-smtp-1.0.1rc1/apache_airflow_providers_smtp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4888 2023-04-09 13:49:56.000000 apache-airflow-providers-smtp-1.0.1rc1/apache_airflow_providers_smtp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      686 2023-04-09 13:49:56.000000 apache-airflow-providers-smtp-1.0.1rc1/apache_airflow_providers_smtp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-09 13:49:56.000000 apache-airflow-providers-smtp-1.0.1rc1/apache_airflow_providers_smtp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      101 2023-04-09 13:49:56.000000 apache-airflow-providers-smtp-1.0.1rc1/apache_airflow_providers_smtp.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-09 13:49:56.000000 apache-airflow-providers-smtp-1.0.1rc1/apache_airflow_providers_smtp.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       27 2023-04-09 13:49:56.000000 apache-airflow-providers-smtp-1.0.1rc1/apache_airflow_providers_smtp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-09 13:49:56.000000 apache-airflow-providers-smtp-1.0.1rc1/apache_airflow_providers_smtp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5246 2023-04-07 12:28:58.000000 apache-airflow-providers-smtp-1.0.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1816 2023-04-09 13:49:56.000000 apache-airflow-providers-smtp-1.0.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1626 2023-04-09 13:49:54.000000 apache-airflow-providers-smtp-1.0.1rc1/setup.py
```

### Comparing `apache-airflow-providers-smtp-1.0.0rc1/LICENSE` & `apache-airflow-providers-smtp-1.0.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-smtp-1.0.0rc1/MANIFEST.in` & `apache-airflow-providers-smtp-1.0.1rc1/MANIFEST.in`

 * *Files 6% similar despite different names*

```diff
@@ -23,10 +23,9 @@
 # `MANIFEST_TEMPLATE.py.jinja2` IN the `provider_packages` DIRECTORY
 
 
 
 
 include NOTICE
 include LICENSE
-include CHANGELOG.txt
-include README.md
+include CHANGELOG.rst
 global-exclude __pycache__  *.pyc
```

### Comparing `apache-airflow-providers-smtp-1.0.0rc1/PKG-INFO` & `apache-airflow-providers-smtp-1.0.1rc1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-smtp
-Version: 1.0.0rc1
+Version: 1.0.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-smtp package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-smtp/1.0.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-smtp/1.0.1/
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -48,28 +48,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-smtp``
 
-Release: ``1.0.0rc1``
+Release: ``1.0.1rc1``
 
 
 `Simple Mail Transfer Protocol (SMTP) <https://tools.ietf.org/html/rfc5321>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``smtp`` provider. All classes for this provider package
 are in ``airflow.providers.smtp`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-smtp/1.0.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-smtp/1.0.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -108,11 +108,24 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+1.0.1
+.....
+
+Bug Fixes
+~~~~~~~~~
+
+* ``'EmailOperator': fix wrong assignment of 'from_email' (#30524)``
+* ``Accept None for 'EmailOperator.from_email' to load it from smtp connection (#30533)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add mechanism to suspend providers (#30422)``
+
 1.0.0
 .....
 
 Initial version of the provider.
```

### Comparing `apache-airflow-providers-smtp-1.0.0rc1/README.rst` & `apache-airflow-providers-smtp-1.0.1rc1/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -15,28 +15,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-smtp``
 
-Release: ``1.0.0rc1``
+Release: ``1.0.1rc1``
 
 
 `Simple Mail Transfer Protocol (SMTP) <https://tools.ietf.org/html/rfc5321>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``smtp`` provider. All classes for this provider package
 are in ``airflow.providers.smtp`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-smtp/1.0.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-smtp/1.0.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -75,11 +75,24 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+1.0.1
+.....
+
+Bug Fixes
+~~~~~~~~~
+
+* ``'EmailOperator': fix wrong assignment of 'from_email' (#30524)``
+* ``Accept None for 'EmailOperator.from_email' to load it from smtp connection (#30533)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add mechanism to suspend providers (#30422)``
+
 1.0.0
 .....
 
 Initial version of the provider.
```

### Comparing `apache-airflow-providers-smtp-1.0.0rc1/airflow/providers/smtp/__init__.py` & `apache-airflow-providers-smtp-1.0.1rc1/airflow/providers/smtp/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-smtp-1.0.0rc1/airflow/providers/smtp/get_provider_info.py` & `apache-airflow-providers-smtp-1.0.1rc1/airflow/providers/smtp/get_provider_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,16 @@
 
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-smtp",
         "name": "Simple Mail Transfer Protocol (SMTP)",
         "description": "`Simple Mail Transfer Protocol (SMTP) <https://tools.ietf.org/html/rfc5321>`__\n",
-        "versions": ["1.0.0"],
+        "suspended": False,
+        "versions": ["1.0.1", "1.0.0"],
         "dependencies": ["apache-airflow>=2.3.0"],
         "integrations": [
             {
                 "integration-name": "Simple Mail Transfer Protocol (SMTP)",
                 "external-doc-url": "https://tools.ietf.org/html/rfc5321",
                 "logo": "/integration-logos/smtp/SMTP.png",
                 "tags": ["protocol"],
```

### Comparing `apache-airflow-providers-smtp-1.0.0rc1/airflow/providers/smtp/hooks/__init__.py` & `apache-airflow-providers-smtp-1.0.1rc1/airflow/providers/smtp/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-smtp-1.0.0rc1/airflow/providers/smtp/hooks/smtp.py` & `apache-airflow-providers-smtp-1.0.1rc1/airflow/providers/smtp/hooks/smtp.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,14 +147,15 @@
                     return True, "Connection successfully tested"
         except Exception as e:
             return False, str(e)
         return False, "Failed to establish connection"
 
     def send_email_smtp(
         self,
+        *,
         to: str | Iterable[str],
         subject: str,
         html_content: str,
         from_email: str | None = None,
         files: list[str] | None = None,
         dryrun: bool = False,
         cc: str | Iterable[str] | None = None,
```

### Comparing `apache-airflow-providers-smtp-1.0.0rc1/airflow/providers/smtp/operators/__init__.py` & `apache-airflow-providers-smtp-1.0.1rc1/airflow/providers/smtp/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-smtp-1.0.0rc1/airflow/providers/smtp/operators/smtp.py` & `apache-airflow-providers-smtp-1.0.1rc1/airflow/providers/smtp/operators/smtp.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,46 +47,46 @@
     template_ext: Sequence[str] = (".html",)
     ui_color = "#e6faf9"
 
     def __init__(
         self,
         *,
         to: list[str] | str,
-        from_email: str,
         subject: str,
         html_content: str,
+        from_email: str | None = None,
         files: list | None = None,
         cc: list[str] | str | None = None,
         bcc: list[str] | str | None = None,
         mime_subtype: str = "mixed",
         mime_charset: str = "utf-8",
         conn_id: str = "smtp_default",
         custom_headers: dict[str, Any] | None = None,
         **kwargs,
     ) -> None:
         super().__init__(**kwargs)
         self.to = to
-        self.from_email = from_email
         self.subject = subject
         self.html_content = html_content
+        self.from_email = from_email
         self.files = files or []
         self.cc = cc
         self.bcc = bcc
         self.mime_subtype = mime_subtype
         self.mime_charset = mime_charset
         self.conn_id = conn_id
         self.custom_headers = custom_headers
 
     def execute(self, context: Context):
         with SmtpHook(smtp_conn_id=self.conn_id) as smtp_hook:
             return smtp_hook.send_email_smtp(
-                self.to,
-                self.from_email,
-                self.subject,
-                self.html_content,
+                to=self.to,
+                subject=self.subject,
+                html_content=self.html_content,
+                from_email=self.from_email,
                 files=self.files,
                 cc=self.cc,
                 bcc=self.bcc,
                 mime_subtype=self.mime_subtype,
                 mime_charset=self.mime_charset,
                 conn_id=self.conn_id,
                 custom_headers=self.custom_headers,
```

### Comparing `apache-airflow-providers-smtp-1.0.0rc1/apache_airflow_providers_smtp.egg-info/PKG-INFO` & `apache-airflow-providers-smtp-1.0.1rc1/apache_airflow_providers_smtp.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-smtp
-Version: 1.0.0rc1
+Version: 1.0.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-smtp package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-smtp/1.0.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-smtp/1.0.1/
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -48,28 +48,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-smtp``
 
-Release: ``1.0.0rc1``
+Release: ``1.0.1rc1``
 
 
 `Simple Mail Transfer Protocol (SMTP) <https://tools.ietf.org/html/rfc5321>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``smtp`` provider. All classes for this provider package
 are in ``airflow.providers.smtp`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-smtp/1.0.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-smtp/1.0.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -108,11 +108,24 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+1.0.1
+.....
+
+Bug Fixes
+~~~~~~~~~
+
+* ``'EmailOperator': fix wrong assignment of 'from_email' (#30524)``
+* ``Accept None for 'EmailOperator.from_email' to load it from smtp connection (#30533)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add mechanism to suspend providers (#30422)``
+
 1.0.0
 .....
 
 Initial version of the provider.
```

### Comparing `apache-airflow-providers-smtp-1.0.0rc1/apache_airflow_providers_smtp.egg-info/SOURCES.txt` & `apache-airflow-providers-smtp-1.0.1rc1/apache_airflow_providers_smtp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-smtp-1.0.0rc1/pyproject.toml` & `apache-airflow-providers-smtp-1.0.1rc1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -135,18 +135,15 @@
 
 # The test_python.py is needed because adding __future__.annotations breaks runtime checks that are
 # needed for the test to work
 "tests/decorators/test_python.py" = ["I002"]
 
 # The Pydantic representations of SqlAlchemy Models are not parsed well with Pydantic
 # when __future__.annotations is used so we need to skip them from upgrading
-"airflow/models/pydantic/taskinstance.py" = ["I002"]
-"airflow/models/pydantic/dag_run.py" = ["I002"]
-"airflow/models/pydantic/dataset.py" = ["I002"]
-"airflow/jobs/pydantic/base_job.py" = ["I002"]
+"airflow/serialization/pydantic/*.py" = ["I002"]
 
 # Ignore pydoc style from these
 "*.pyi" = ["D"]
 "tests/*" = ["D"]
 "scripts/*" = ["D"]
 "dev/*" = ["D"]
 "docs/*" = ["D"]
```

### Comparing `apache-airflow-providers-smtp-1.0.0rc1/setup.cfg` & `apache-airflow-providers-smtp-1.0.1rc1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-smtp/1.0.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-smtp/1.0.1/
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
```

### Comparing `apache-airflow-providers-smtp-1.0.0rc1/setup.py` & `apache-airflow-providers-smtp-1.0.1rc1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,21 +22,28 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-smtp package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "1.0.0"
+version = "1.0.1"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-smtp setup."""
     setup(
         version=version,
         extras_require={},
-        packages=find_namespace_packages(include=["airflow.providers.smtp", "airflow.providers.smtp.*"]),
+        packages=find_namespace_packages(
+            include=[
+                "airflow.providers.smtp",
+                "airflow.providers.smtp.*",
+                "airflow.providers.smtp_vendor",
+                "airflow.providers.smtp_vendor.*",
+            ],
+        ),
     )
 
 
 if __name__ == "__main__":
     do_setup()
```

