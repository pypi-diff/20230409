# Comparing `tmp/EmailNotice-1.0.0-py3-none-any.whl.zip` & `tmp/EmailNotice-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 45769 bytes, number of entries: 60
+Zip file size: 45777 bytes, number of entries: 60
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Feb-17 10:05 era/__init__.py
 -rw-rw-rw-  2.0 fat    10677 b- defN 23-Apr-07 09:38 era/Assets/refresh-icon.png
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Feb-25 07:10 era/Database/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Feb-20 15:27 era/Database/Dao/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Feb-20 15:26 era/Database/Dao/emailAccountDao.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Feb-23 15:47 era/Database/Dao/emailTemplateDao.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Feb-21 15:14 era/Database/Impl/__init__.py
@@ -23,15 +23,15 @@
 -rw-rw-rw-  2.0 fat     3974 b- defN 23-Apr-08 14:52 era/Utility/ConfigUtility.py
 -rw-rw-rw-  2.0 fat      620 b- defN 23-Mar-25 09:11 era/Utility/FileUtility.py
 -rw-rw-rw-  2.0 fat    11183 b- defN 23-Apr-08 15:34 era/Utility/StringUtilityCTK.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Feb-21 15:05 era/Utility/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Feb-20 15:15 era/View/__init__.py
 -rw-rw-rw-  2.0 fat    10902 b- defN 23-Mar-28 15:32 era/View/edit_email_list_top_level.py
 -rw-rw-rw-  2.0 fat    16075 b- defN 23-Mar-26 15:26 era/View/edit_template_top_level.py
--rw-rw-rw-  2.0 fat    13387 b- defN 23-Apr-08 15:39 era/View/main_view.py
+-rw-rw-rw-  2.0 fat    13393 b- defN 23-Apr-09 08:02 era/View/main_view.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Feb-17 10:05 src/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Feb-25 07:10 src/Database/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Feb-20 15:27 src/Database/Dao/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Feb-20 15:26 src/Database/Dao/emailAccountDao.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Feb-23 15:47 src/Database/Dao/emailTemplateDao.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Feb-21 15:14 src/Database/Impl/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Feb-21 15:14 src/Database/Impl/emailAccountDaoImpl.py
@@ -51,12 +51,12 @@
 -rw-rw-rw-  2.0 fat     1166 b- defN 23-Jan-09 08:16 src/Utility/ConfigUtility.py
 -rw-rw-rw-  2.0 fat     7134 b- defN 23-Mar-19 15:11 src/Utility/StringUtilityCTK.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Feb-21 15:05 src/Utility/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Feb-20 15:15 src/View/__init__.py
 -rw-rw-rw-  2.0 fat    16050 b- defN 23-Mar-19 15:14 src/View/edit_template_top_level.py
 -rw-rw-rw-  2.0 fat     7989 b- defN 23-Mar-19 15:00 src/View/main_view.py
 -rw-rw-rw-  2.0 fat      147 b- defN 23-Feb-19 10:04 src/View/testHtml.py
--rw-rw-rw-  2.0 fat      532 b- defN 23-Apr-09 07:56 EmailNotice-1.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-09 07:56 EmailNotice-1.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        4 b- defN 23-Apr-09 07:56 EmailNotice-1.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     5166 b- defN 23-Apr-09 07:56 EmailNotice-1.0.0.dist-info/RECORD
-60 files, 141452 bytes uncompressed, 37405 bytes compressed:  73.6%
+-rw-rw-rw-  2.0 fat      532 b- defN 23-Apr-09 08:06 EmailNotice-1.0.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-09 08:06 EmailNotice-1.0.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        4 b- defN 23-Apr-09 08:06 EmailNotice-1.0.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     5166 b- defN 23-Apr-09 08:06 EmailNotice-1.0.1.dist-info/RECORD
+60 files, 141458 bytes uncompressed, 37413 bytes compressed:  73.6%
```

## zipnote {}

```diff
@@ -162,20 +162,20 @@
 
 Filename: src/View/main_view.py
 Comment: 
 
 Filename: src/View/testHtml.py
 Comment: 
 
-Filename: EmailNotice-1.0.0.dist-info/METADATA
+Filename: EmailNotice-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: EmailNotice-1.0.0.dist-info/WHEEL
+Filename: EmailNotice-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: EmailNotice-1.0.0.dist-info/top_level.txt
+Filename: EmailNotice-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: EmailNotice-1.0.0.dist-info/RECORD
+Filename: EmailNotice-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## era/View/main_view.py

```diff
@@ -270,32 +270,23 @@
 
             messagebox.showerror(self.stringValue.retry.get(), errorMessage)
             pass
 
         pass
 
 
+    
+# customtkinter.set_appearance_mode("Light")  # Modes: "System" (standard), "Dark", "Light"
+# customtkinter.set_default_color_theme("dark-blue")  # Themes: "blue" (standard), "green", "dark-blue"
 
+# app = customtkinter.CTk()
+# app.geometry("1000x1000")
 
+# # set grid layout 1x2
+# app.grid_rowconfigure(0, weight=1)
+# app.grid_columnconfigure(1, weight=1)
 
+# email = MainView(app)
+# email.grid(row=0, column=1, sticky="nsew")
 
-
-
-
-
-
-
-customtkinter.set_appearance_mode("Light")  # Modes: "System" (standard), "Dark", "Light"
-customtkinter.set_default_color_theme("dark-blue")  # Themes: "blue" (standard), "green", "dark-blue"
-
-app = customtkinter.CTk()
-app.geometry("1000x1000")
-
-# set grid layout 1x2
-app.grid_rowconfigure(0, weight=1)
-app.grid_columnconfigure(1, weight=1)
-
-email = MainView(app)
-email.grid(row=0, column=1, sticky="nsew")
-
-app.mainloop()
+# app.mainloop()
```

## Comparing `EmailNotice-1.0.0.dist-info/METADATA` & `EmailNotice-1.0.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EmailNotice
-Version: 1.0.0
+Version: 1.0.1
 Summary: GUI Application
 Home-page: 
 Author: HexBee
 Author-email: mat230821@hotmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `EmailNotice-1.0.0.dist-info/RECORD` & `EmailNotice-1.0.1.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 era/Utility/ConfigUtility.py,sha256=HO5r1PFdveE1TdsExnhRTf5zDsHfsZRW3M1LmR3EBiM,3974
 era/Utility/FileUtility.py,sha256=5kCFOD6C3dBu0mXZ3KsMW6eWyNhlcmoeBh1T1KBJEew,620
 era/Utility/StringUtilityCTK.py,sha256=WTT8IY92SGTN1-zeIaVKqFuFXEXZJSkX03byRc8Aojk,11183
 era/Utility/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 era/View/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 era/View/edit_email_list_top_level.py,sha256=0_WyPrh45jpj1tLkLXl1uVrd3cQUSSQH8E_YK08-Vu4,10902
 era/View/edit_template_top_level.py,sha256=3QA4Nif8jUZAAa7cM2JOZftDxq0vT9KbEO40xLwX76s,16075
-era/View/main_view.py,sha256=PSumMXBhLqFiu_Aw-qk1kb0XjJYMgp1JxTImYtIqTTE,13387
+era/View/main_view.py,sha256=4gMkuuUGpaq1dylrPOx10ZIKwzTQUGYQshuXW-2_wkI,13393
 src/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 src/Database/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 src/Database/Dao/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 src/Database/Dao/emailAccountDao.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 src/Database/Dao/emailTemplateDao.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 src/Database/Impl/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 src/Database/Impl/emailAccountDaoImpl.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
@@ -50,11 +50,11 @@
 src/Utility/ConfigUtility.py,sha256=ryrC2uVxU0slRZAp9294-vam6T1tBMHiZeYqbZ9Z1pc,1166
 src/Utility/StringUtilityCTK.py,sha256=JahZ119BJVHCxJ2SOwQC_pw-1oQCPGssJpqF_MGfybo,7134
 src/Utility/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 src/View/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 src/View/edit_template_top_level.py,sha256=j7vjeUyT4NME7GLlMP5mlTtngmlooa9k9RTWkzhvg-M,16050
 src/View/main_view.py,sha256=NU8UEFs8QbGxQgUz8w27t8ACiQCjaTN1bTBcRjG0EyQ,7989
 src/View/testHtml.py,sha256=T6tMYcnII859MpDblnFcwaSEMZLaNmybQXoIJcHaSm8,147
-EmailNotice-1.0.0.dist-info/METADATA,sha256=XmSprUKZTU5Xaru_OWZgkZVsUgyBsj-5uPXjGwvvgGk,532
-EmailNotice-1.0.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-EmailNotice-1.0.0.dist-info/top_level.txt,sha256=mwOEYCo2fCv-4-kWSscMR7P3BTepFDFooHL4qGH9pyg,4
-EmailNotice-1.0.0.dist-info/RECORD,,
+EmailNotice-1.0.1.dist-info/METADATA,sha256=gfgertHb0WWHfER8xWNK6zZ0p42eFjJUC1ynxEdmcEU,532
+EmailNotice-1.0.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+EmailNotice-1.0.1.dist-info/top_level.txt,sha256=mwOEYCo2fCv-4-kWSscMR7P3BTepFDFooHL4qGH9pyg,4
+EmailNotice-1.0.1.dist-info/RECORD,,
```

