# Comparing `tmp/xyz_exam-0.3.4-py3-none-any.whl.zip` & `tmp/xyz_exam-0.3.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 30410 bytes, number of entries: 31
+Zip file size: 30479 bytes, number of entries: 31
 -rw-r--r--  2.0 unx       43 b- defN 20-Jan-20 09:10 xyz_exam/__init__.py
 -rw-r--r--  2.0 unx     1631 b- defN 22-Dec-07 08:39 xyz_exam/admin.py
 -rw-r--r--  2.0 unx    10615 b- defN 23-Mar-29 09:19 xyz_exam/apis.py
 -rw-r--r--  2.0 unx      326 b- defN 20-Jan-20 09:08 xyz_exam/apps.py
 -rw-r--r--  2.0 unx     1381 b- defN 22-Oct-27 06:40 xyz_exam/choices.py
 -rw-r--r--  2.0 unx    13585 b- defN 23-Mar-14 03:26 xyz_exam/helper.py
 -rw-r--r--  2.0 unx    15318 b- defN 22-Dec-07 08:35 xyz_exam/models.py
 -rw-r--r--  2.0 unx     3688 b- defN 23-Jan-11 04:45 xyz_exam/receivers.py
 -rw-r--r--  2.0 unx     3469 b- defN 22-Dec-07 08:35 xyz_exam/serializers.py
 -rw-r--r--  2.0 unx     3574 b- defN 22-Jun-23 18:16 xyz_exam/stats.py
--rw-r--r--  2.0 unx     2926 b- defN 23-Mar-03 16:46 xyz_exam/stores.py
+-rw-r--r--  2.0 unx     3154 b- defN 23-Apr-09 13:18 xyz_exam/stores.py
 -rw-r--r--  2.0 unx     7732 b- defN 20-Jan-20 09:14 xyz_exam/migrations/0001_initial.py
 -rw-r--r--  2.0 unx     3123 b- defN 20-Jun-15 13:12 xyz_exam/migrations/0002_auto_20200615_2112.py
 -rw-r--r--  2.0 unx     2514 b- defN 20-Jun-25 21:11 xyz_exam/migrations/0003_auto_20200626_0511.py
 -rw-r--r--  2.0 unx     2405 b- defN 20-Aug-01 16:28 xyz_exam/migrations/0004_auto_20200802_0028.py
 -rw-r--r--  2.0 unx      518 b- defN 20-Sep-01 15:06 xyz_exam/migrations/0005_answer_pictures.py
 -rw-r--r--  2.0 unx      543 b- defN 20-Sep-14 19:21 xyz_exam/migrations/0006_answer_grade_detail.py
 -rw-r--r--  2.0 unx      513 b- defN 20-Sep-16 18:32 xyz_exam/migrations/0007_auto_20200917_0232.py
@@ -22,12 +22,12 @@
 -rw-r--r--  2.0 unx     1429 b- defN 21-Mar-31 04:56 xyz_exam/migrations/0010_auto_20210331_1251.py
 -rw-r--r--  2.0 unx     1606 b- defN 22-Sep-08 16:15 xyz_exam/migrations/0011_content.py
 -rw-r--r--  2.0 unx      601 b- defN 22-Sep-17 06:10 xyz_exam/migrations/0012_auto_20220917_1410.py
 -rw-r--r--  2.0 unx      949 b- defN 22-Oct-27 06:41 xyz_exam/migrations/0013_auto_20221027_1441.py
 -rw-r--r--  2.0 unx      498 b- defN 22-Nov-27 11:39 xyz_exam/migrations/0014_paper_parent_id.py
 -rw-r--r--  2.0 unx      484 b- defN 22-Dec-07 08:37 xyz_exam/migrations/0015_paper_is_editable.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Jan-20 09:14 xyz_exam/migrations/__init__.py
--rw-r--r--  2.0 unx      987 b- defN 23-Mar-29 09:22 xyz_exam-0.3.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-29 09:22 xyz_exam-0.3.4.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Mar-29 09:22 xyz_exam-0.3.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     2722 b- defN 23-Mar-29 09:22 xyz_exam-0.3.4.dist-info/RECORD
-31 files, 84255 bytes uncompressed, 25978 bytes compressed:  69.2%
+-rw-r--r--  2.0 unx      987 b- defN 23-Apr-09 15:54 xyz_exam-0.3.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-09 15:54 xyz_exam-0.3.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Apr-09 15:54 xyz_exam-0.3.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     2722 b- defN 23-Apr-09 15:54 xyz_exam-0.3.5.dist-info/RECORD
+31 files, 84483 bytes uncompressed, 26047 bytes compressed:  69.2%
```

## zipnote {}

```diff
@@ -75,20 +75,20 @@
 
 Filename: xyz_exam/migrations/0015_paper_is_editable.py
 Comment: 
 
 Filename: xyz_exam/migrations/__init__.py
 Comment: 
 
-Filename: xyz_exam-0.3.4.dist-info/METADATA
+Filename: xyz_exam-0.3.5.dist-info/METADATA
 Comment: 
 
-Filename: xyz_exam-0.3.4.dist-info/WHEEL
+Filename: xyz_exam-0.3.5.dist-info/WHEEL
 Comment: 
 
-Filename: xyz_exam-0.3.4.dist-info/top_level.txt
+Filename: xyz_exam-0.3.5.dist-info/top_level.txt
 Comment: 
 
-Filename: xyz_exam-0.3.4.dist-info/RECORD
+Filename: xyz_exam-0.3.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xyz_exam/stores.py

```diff
@@ -25,14 +25,21 @@
     if 'uid' in q:
         return q['uid']
     gids = g.get('memo', '')
     qids = '%s%s%s' % (gids, q['type'], q['title'])
     return hashlib.md5(qids.encode('utf8')).hexdigest()[:7]
 
 
+def gen_question_subid(q):
+    options = q.get('options')
+    if options:
+        ss = sorted([a['text'] for a in options])
+        return hashlib.md5('\n'.join(ss).encode('utf8')).hexdigest()[:7]
+
+
 def extra_year_month(title):
     import re
     m = re.compile(r'真题(\d{2})(\d{2})$').search(title)
     if m:
         return '20' + m.group(1), m.group(2)
     m = re.compile(r'(\d{4})年').search(title)
     year = m.group(1) if m else None
@@ -53,22 +60,22 @@
 
     for g in p['groups']:
         for q in g['questions']:
             # if g.get('memo'):
             q['group'] = dict([(k, v) for k, v in g.items() if k in ['title', 'memo', 'inputs', 'number']])
             q['ownerType'] = pws
             q['typeName'] = group_name_sumary(g['title'])
-            q['ownerId'] = paper.owner_id
+            owner_id = q['ownerId'] = paper.owner_id
             if year:
                 q['year'] = int(year)
             if month:
                 q['month'] = int(month)
             uid = gen_question_uid(q, g)
             q.pop('papers', [])
-            qs.upsert(dict(uid=uid), q, addToSet=dict(papers=paper.id))
+            qs.upsert(dict(uid=uid, ownerId=owner_id), q, addToSet=dict(papers=paper.id))
 
 
 def group_paper_questions(qset, group='outline'):
     ids = list(qset.values_list('id', flat=True))
     st = QuestionStore()
     return st.count_by(group, {'papers': {'$in': ids}}, output='dict')
```

## Comparing `xyz_exam-0.3.4.dist-info/METADATA` & `xyz_exam-0.3.5.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xyz-exam
-Version: 0.3.4
+Version: 0.3.5
 Summary: exam app
 Home-page: https://github.com/szuprefix/py-xyz-exam
 Author: szuprefix
 Author-email: szuprefix@126.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

## Comparing `xyz_exam-0.3.4.dist-info/RECORD` & `xyz_exam-0.3.5.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 xyz_exam/apps.py,sha256=vQwce8vZ81IpBtAVpe8wvqqZXfV0Ht5AJeMY7rRsP6g,326
 xyz_exam/choices.py,sha256=2lKMyQAWnl_yoow98cpQHwqpk-RXxnxij4xcvxeVUko,1381
 xyz_exam/helper.py,sha256=lKVyMH8fOF4JL1wbdr0Hbhm8nFiJWpY2vh3vc_sdvkQ,13585
 xyz_exam/models.py,sha256=EY97WfuQSSl6bhhUihnipfNkbRowjaP3DNluyAedyBI,15318
 xyz_exam/receivers.py,sha256=oOthYcU_vabvgLLAWrjq3BubC7DQbA-ek6_hQhsqhg4,3688
 xyz_exam/serializers.py,sha256=1hNoFpJJwoKBkpxOhrXH7cfw6G-QZO5Dj5C173EUBHU,3469
 xyz_exam/stats.py,sha256=u6XcKw7wkLOm_JtCLoF6241sAZghHQNh5sQfjmjBkSs,3574
-xyz_exam/stores.py,sha256=kI-Brx6hwVL_Ca6yWk1F34S8WMf5OOsnSAbbij7YwHg,2926
+xyz_exam/stores.py,sha256=2T5aMjrMQ4w-qxgkrkx2ZmNcbZq_8lojUZf8dWjGh90,3154
 xyz_exam/migrations/0001_initial.py,sha256=Poa0-alDt7Ylgm6YeJ2cUwNPvHJz55qsuuPTT0IPBR0,7732
 xyz_exam/migrations/0002_auto_20200615_2112.py,sha256=JofSLAwEIoJ1pjZu6MLRiPyWn1nAhxQUuTketVO81Yc,3123
 xyz_exam/migrations/0003_auto_20200626_0511.py,sha256=sAkmKE3fYO9gi9aDOPbZALKZ8T0ZRCvSHiiJjMbRzmM,2514
 xyz_exam/migrations/0004_auto_20200802_0028.py,sha256=oJxvhMj_uh5qYoqTe68wNNrtFLTaIYUbjIfLX14u7pc,2405
 xyz_exam/migrations/0005_answer_pictures.py,sha256=TMr2dBWmxvq0rHsqH20rkO-0uz9k0vMgHgiZqJf8TII,518
 xyz_exam/migrations/0006_answer_grade_detail.py,sha256=LhvXN8qNpjIQT_QKCftSLdm02-lcg75sWA4_CxudVYs,543
 xyz_exam/migrations/0007_auto_20200917_0232.py,sha256=yWIPcc_R4imuhDvhYOyYS62eqN4eTYfuKTJFsSfIv4U,513
@@ -21,11 +21,11 @@
 xyz_exam/migrations/0010_auto_20210331_1251.py,sha256=terrpUXEcDr0jX_cMWRuM4mLkUUYsSCuragsTs77H4Q,1429
 xyz_exam/migrations/0011_content.py,sha256=FqT4q-o8xJywQ2382G6js1Av7ZEgROr7NmLGSxBp6NU,1606
 xyz_exam/migrations/0012_auto_20220917_1410.py,sha256=RHYolr37Gk2lqZifxypAcylcADeTNZBRRvDGJWAoDmE,601
 xyz_exam/migrations/0013_auto_20221027_1441.py,sha256=_iFsdTKrADPb_EGTTw-3gMD8FMakD8nTbBJOsXRLhY4,949
 xyz_exam/migrations/0014_paper_parent_id.py,sha256=WpMmFmzN2c_4UiSJl2x2QiNv7MZccIbA8kq6M8WWZd8,498
 xyz_exam/migrations/0015_paper_is_editable.py,sha256=8Fbh6vDwxJnKcXar8s6LfGfvAsPdp0vAjxb0XrtjNU0,484
 xyz_exam/migrations/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-xyz_exam-0.3.4.dist-info/METADATA,sha256=WxASwmqjOYWGQjrpOygmqT9C9xhqt3zkr_Xwjl434FU,987
-xyz_exam-0.3.4.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-xyz_exam-0.3.4.dist-info/top_level.txt,sha256=AdR0uTxGwndkM__gIaBc3_DMomtP0FQ-PKg_WJP2KTE,9
-xyz_exam-0.3.4.dist-info/RECORD,,
+xyz_exam-0.3.5.dist-info/METADATA,sha256=j7z-fGcg9lNyMZ64K7a18LvtcZQLYUx_vLHWMAHgc8U,987
+xyz_exam-0.3.5.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+xyz_exam-0.3.5.dist-info/top_level.txt,sha256=AdR0uTxGwndkM__gIaBc3_DMomtP0FQ-PKg_WJP2KTE,9
+xyz_exam-0.3.5.dist-info/RECORD,,
```

