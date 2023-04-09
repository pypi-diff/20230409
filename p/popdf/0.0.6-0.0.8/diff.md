# Comparing `tmp/popdf-0.0.6.tar.gz` & `tmp/popdf-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "popdf-0.0.6.tar", last modified: Mon Apr  3 15:09:17 2023, max compression
+gzip compressed data, was "popdf-0.0.8.tar", last modified: Sun Apr  9 06:17:20 2023, max compression
```

## Comparing `popdf-0.0.6.tar` & `popdf-0.0.8.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-04-03 15:09:17.809339 popdf-0.0.6/
--rw-rw-rw-   0        0        0     1093 2022-09-13 01:21:27.000000 popdf-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     5244 2023-04-03 15:09:17.809339 popdf-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     4719 2023-04-02 05:09:27.000000 popdf-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-03 15:09:17.761692 popdf-0.0.6/popdf/
--rw-rw-rw-   0        0        0       29 2023-04-02 07:16:35.000000 popdf-0.0.6/popdf/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-03 15:09:17.793220 popdf-0.0.6/popdf/api/
--rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 popdf-0.0.6/popdf/api/__init__.py
--rw-rw-rw-   0        0        0     1701 2023-04-03 15:03:37.000000 popdf-0.0.6/popdf/api/pdf.py
-drwxrwxrwx   0        0        0        0 2023-04-03 15:09:17.797325 popdf-0.0.6/popdf/core/
--rw-rw-rw-   0        0        0     8242 2023-04-03 15:09:10.000000 popdf-0.0.6/popdf/core/PDFType.py
--rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 popdf-0.0.6/popdf/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-03 15:09:17.799342 popdf-0.0.6/popdf/lib/
--rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 popdf-0.0.6/popdf/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-03 15:09:17.802341 popdf-0.0.6/popdf/lib/pdf/
--rw-rw-rw-   0        0        0        0 2022-09-01 13:34:44.000000 popdf-0.0.6/popdf/lib/pdf/__init__.py
--rw-rw-rw-   0        0        0     2111 2023-03-24 15:13:04.000000 popdf-0.0.6/popdf/lib/pdf/add_watermark_service.py
-drwxrwxrwx   0        0        0        0 2023-04-03 15:09:17.787232 popdf-0.0.6/popdf.egg-info/
--rw-rw-rw-   0        0        0     5244 2023-04-03 15:09:17.000000 popdf-0.0.6/popdf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      433 2023-04-03 15:09:17.000000 popdf-0.0.6/popdf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-03 15:09:17.000000 popdf-0.0.6/popdf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-08 15:51:16.000000 popdf-0.0.6/popdf.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       70 2023-04-03 15:09:17.000000 popdf-0.0.6/popdf.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-03 15:09:17.000000 popdf-0.0.6/popdf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      776 2023-04-03 15:09:17.811339 popdf-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      389 2022-10-23 08:47:10.000000 popdf-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-03 15:09:17.807341 popdf-0.0.6/tests/
--rw-rw-rw-   0        0        0      181 2022-09-17 08:11:22.000000 popdf-0.0.6/tests/__init__.py
--rw-rw-rw-   0        0        0     2091 2023-04-03 15:03:38.000000 popdf-0.0.6/tests/test_pdf.py
+drwxrwxrwx   0        0        0        0 2023-04-09 06:17:20.462427 popdf-0.0.8/
+-rw-rw-rw-   0        0        0     1093 2022-09-13 01:21:27.000000 popdf-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     5244 2023-04-09 06:17:20.463421 popdf-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     4719 2023-04-02 05:09:27.000000 popdf-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-09 06:17:20.408811 popdf-0.0.8/popdf/
+-rw-rw-rw-   0        0        0       29 2023-04-06 14:38:32.000000 popdf-0.0.8/popdf/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-09 06:17:20.434396 popdf-0.0.8/popdf/api/
+-rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 popdf-0.0.8/popdf/api/__init__.py
+-rw-rw-rw-   0        0        0     1663 2023-04-09 06:14:30.000000 popdf-0.0.8/popdf/api/pdf.py
+drwxrwxrwx   0        0        0        0 2023-04-09 06:17:20.438389 popdf-0.0.8/popdf/core/
+-rw-rw-rw-   0        0        0     8595 2023-04-09 06:14:30.000000 popdf-0.0.8/popdf/core/PDFType.py
+-rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 popdf-0.0.8/popdf/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-09 06:17:20.439392 popdf-0.0.8/popdf/lib/
+-rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 popdf-0.0.8/popdf/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-09 06:17:20.449908 popdf-0.0.8/popdf/lib/pdf/
+-rw-rw-rw-   0        0        0        0 2022-09-01 13:34:44.000000 popdf-0.0.8/popdf/lib/pdf/__init__.py
+-rw-rw-rw-   0        0        0     2111 2023-03-24 15:13:04.000000 popdf-0.0.8/popdf/lib/pdf/add_watermark_service.py
+drwxrwxrwx   0        0        0        0 2023-04-09 06:17:20.431384 popdf-0.0.8/popdf.egg-info/
+-rw-rw-rw-   0        0        0     5244 2023-04-09 06:17:20.000000 popdf-0.0.8/popdf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      433 2023-04-09 06:17:20.000000 popdf-0.0.8/popdf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 06:17:20.000000 popdf-0.0.8/popdf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-09 06:17:20.000000 popdf-0.0.8/popdf.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       70 2023-04-09 06:17:20.000000 popdf-0.0.8/popdf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-09 06:17:20.000000 popdf-0.0.8/popdf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      776 2023-04-09 06:17:20.465949 popdf-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      389 2022-10-23 08:47:10.000000 popdf-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 06:17:20.461420 popdf-0.0.8/tests/
+-rw-rw-rw-   0        0        0      181 2022-09-17 08:11:22.000000 popdf-0.0.8/tests/__init__.py
+-rw-rw-rw-   0        0        0     2089 2023-04-03 15:21:41.000000 popdf-0.0.8/tests/test_pdf.py
```

### Comparing `popdf-0.0.6/LICENSE` & `popdf-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `popdf-0.0.6/PKG-INFO` & `popdf-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: popdf
-Version: 0.0.6
+Version: 0.0.8
 Summary: pip install popdf
 Home-page: https://www.python-office.com/
 Author: CoderWanFeng
 Author-email: 1957875073@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CoderWanFeng/popdf/issues
 Project-URL: Documentation, https://github.com/CoderWanFeng/popdf/blob/master/README.md
```

### Comparing `popdf-0.0.6/README.md` & `popdf-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `popdf-0.0.6/popdf/api/pdf.py` & `popdf-0.0.8/popdf/api/pdf.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,16 +27,16 @@
 # @except_dec()
 def txt2pdf(path: str, res_pdf='txt2pdf.pdf'):
     mainPDF.file2pdf(path, res_pdf)
 
 
 # PDF加密
 # @except_dec()
-def encrypt4pdf(path, password, output_path=r'./', res_pdf='encrypt.pdf'):
-    mainPDF.encrypt4pdf(path, password, output_path, res_pdf)
+def encrypt4pdf(path, password, output_path):
+    mainPDF.encrypt4pdf(path, password, output_path)
 
 
 # PDF解密
 # @except_dec()
 def decrypt4pdf(path, password, res_pdf='decrypt.pdf'):
     mainPDF.decrypt4pdf(path, password, res_pdf)
```

### Comparing `popdf-0.0.6/popdf/core/PDFType.py` & `popdf-0.0.8/popdf/core/PDFType.py`

 * *Files 3% similar despite different names*

```diff
@@ -92,25 +92,26 @@
                 pdf_writer.add_page(pdf_reader.pages[page])
 
         # 把这个已合并了的PDF文档存储起来
         with open(output, 'wb') as out:
             pdf_writer.write(out)
 
     # PDF加密
-    def encrypt4pdf(self, path, password, output_path, res_pdf='encrypt.pdf', suffix='.pdf'):
+    def encrypt4pdf(self, path, password, output_path, suffix='.pdf'):
         """
         @Author & Date  : CoderWanFeng 2022/5/9 18:27
         @Desc  : path: 存放文件的路径
                 password: 你的密码
                 res_pdf: 结果文件的名称 ，可以为空，默认是：encrypt.pdf
         """
         abs_path = Path(path).absolute()
         pdf_list = get_files(path=str(abs_path), suffix=suffix)
         for index, pdf_file in simple_progress(enumerate(pdf_list)):
             pdf = pikepdf.open(pdf_file)
+            output_path = r'./' if output_path == None else output_path
             pdf.save(str(Path(output_path).absolute()) + '//' + Path(pdf_file).stem + '（加密）' + suffix,
                      encryption=pikepdf.Encryption(owner=password, user=password, R=4))
             pdf.close()
         # print("encrypt4pdf，该功能已过期")
 
     # PDF解密
     def decrypt4pdf(self, path, password, res_pdf='decrypt.pdf'):
@@ -138,29 +139,31 @@
     #         if not os.path.exists(out_dir):  # 判断存放图片的文件夹是否存在
     #             os.makedirs(out_dir)  # 若图片文件夹不存在就创建
 
     #         pix.writePNG(out_dir + '/' + 'images_%s.png' % pg)  # 将图片写入指定的文件夹内
     #     print(f'PDF转换Image完成，图片在你指定的output文件夹{out_dir}，如果没有指定，默认是PDF同一个文件夹')
 
     def pdf2imgs(self, pdf_path: str, out_dir=".") -> None:
+        pdf_file_list = get_files(pdf_path, suffix='.pdf')
         print('PDF开始转换，你可以加入交流群唠唠嗑：http://www.python4office.cn/wechat-group/')
-        pdfDoc = fitz.open(pdf_path)
-        if pdfDoc.page_count > 50:
-            print('少年，你的PDF页数有点多哟，请耐心等待~')
-        for pg in simple_progress(range(pdfDoc.page_count)):
-            page = pdfDoc[pg]
-            rotate = int(0)
-            # 每个尺寸的缩放系数为1.3，这将为我们生成分辨率提高2.6的图像。
-            # 此处若是不做设置，默认图片大小为：792X612, dpi=96
-            zoom_x = 1.33333333  # (1.33333333-->1056x816)   (2-->1584x1224)
-            zoom_y = 1.33333333
-            mat = fitz.Matrix(zoom_x, zoom_y).prerotate(rotate)
-            pix = page.get_pixmap(matrix=mat, alpha=False)
-
-            if not os.path.exists(out_dir):  # 判断存放图片的文件夹是否存在
-                os.makedirs(out_dir)  # 若图片文件夹不存在就创建
-
-            pix.save(out_dir + '/' + 'images_%s.png' % pg)  # 将图片写入指定的文件夹内
-        print(f'PDF转换Image完成，图片在你指定的output文件夹{out_dir}，如果没有指定，默认是PDF同一个文件夹')
+        for pdf_file in simple_progress(pdf_file_list):
+            pdfDoc = fitz.open(pdf_file)
+            if pdfDoc.page_count > 50:
+                print('少年，你的PDF页数有点多哟，请耐心等待~')
+            for pg in simple_progress(range(pdfDoc.page_count)):
+                page = pdfDoc[pg]
+                rotate = int(0)
+                # 每个尺寸的缩放系数为1.3，这将为我们生成分辨率提高2.6的图像。
+                # 此处若是不做设置，默认图片大小为：792X612, dpi=96
+                zoom_x = 1.33333333  # (1.33333333-->1056x816)   (2-->1584x1224)
+                zoom_y = 1.33333333
+                mat = fitz.Matrix(zoom_x, zoom_y).prerotate(rotate)
+                pix = page.get_pixmap(matrix=mat, alpha=False)
+                abs_output = str(Path(out_dir).absolute())
+                if not os.path.exists(abs_output):  # 判断存放图片的文件夹是否存在
+                    os.makedirs(abs_output)  # 若图片文件夹不存在就创建
+                pdf_file_name = Path(pdf_file).stem
+                pix.save(abs_output + f'/ [{pdf_file_name}]-{pg}.jpg')  # 将图片写入指定的文件夹内
+        print(f'PDF转换Image完成，图片在你指定的output文件夹{abs_output}，如果没有指定，默认是PDF同一个文件夹')
 
     def add_img_watermark(self, pdf_file_in, pdf_file_mark, pdf_file_out):
         add_watermark_service.pdf_add_watermark(pdf_file_in, pdf_file_mark, pdf_file_out)
```

### Comparing `popdf-0.0.6/popdf/lib/pdf/add_watermark_service.py` & `popdf-0.0.8/popdf/lib/pdf/add_watermark_service.py`

 * *Files identical despite different names*

### Comparing `popdf-0.0.6/popdf.egg-info/PKG-INFO` & `popdf-0.0.8/popdf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: popdf
-Version: 0.0.6
+Version: 0.0.8
 Summary: pip install popdf
 Home-page: https://www.python-office.com/
 Author: CoderWanFeng
 Author-email: 1957875073@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CoderWanFeng/popdf/issues
 Project-URL: Documentation, https://github.com/CoderWanFeng/popdf/blob/master/README.md
```

### Comparing `popdf-0.0.6/setup.cfg` & `popdf-0.0.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 6f70 6466 0d0a 7665 7273 696f   = popdf..versio
-00000020: 6e20 3d20 302e 302e 360d 0a64 6573 6372  n = 0.0.6..descr
+00000020: 6e20 3d20 302e 302e 380d 0a64 6573 6372  n = 0.0.8..descr
 00000030: 6970 7469 6f6e 203d 2070 6970 2069 6e73  iption = pip ins
 00000040: 7461 6c6c 2070 6f70 6466 0d0a 6c6f 6e67  tall popdf..long
 00000050: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
 00000060: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
 00000070: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 00000080: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type = 
 00000090: 7465 7874 2f6d 6172 6b64 6f77 6e0d 0a75  text/markdown..u
```

### Comparing `popdf-0.0.6/tests/test_pdf.py` & `popdf-0.0.8/tests/test_pdf.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,14 @@
         )
 
     def test_encrypt4pdf(self):
         encrypt4pdf(
             path=r'D:\workplace\code\github\popdf\tests\test_files\pdf',
             password='123456',
             output_path=r'./test_output'
-
         )
 
     def test_decrypt4pdf(self):
         decrypt4pdf(
             path=r'./test_files/pdf/encrypt.pdf',
             password='123456'
         )
```

