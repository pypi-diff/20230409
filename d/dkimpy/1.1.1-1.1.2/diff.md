# Comparing `tmp/dkimpy-1.1.1.tar.gz` & `tmp/dkimpy-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkimpy-1.1.1.tar", last modified: Fri Mar 10 16:17:46 2023, max compression
+gzip compressed data, was "dkimpy-1.1.2.tar", last modified: Sun Apr  9 13:34:23 2023, max compression
```

## Comparing `dkimpy-1.1.1.tar` & `dkimpy-1.1.2.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 kitterma  (1001) kitterma  (1001)        0 2023-03-10 16:17:46.791211 dkimpy-1.1.1/
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)    13322 2023-03-10 16:17:15.000000 dkimpy-1.1.1/ChangeLog
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      979 2020-04-06 04:06:13.000000 dkimpy-1.1.1/LICENSE
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      200 2020-04-06 04:27:45.000000 dkimpy-1.1.1/MANIFEST.in
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)    10824 2023-03-10 16:17:46.791211 dkimpy-1.1.1/PKG-INFO
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     7905 2023-02-28 04:48:54.000000 dkimpy-1.1.1/README.md
-drwxr-xr-x   0 kitterma  (1001) kitterma  (1001)        0 2023-03-10 16:17:46.783211 dkimpy-1.1.1/dkim/
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)    57797 2023-02-25 22:13:05.000000 dkimpy-1.1.1/dkim/__init__.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      139 2020-04-06 04:06:13.000000 dkimpy-1.1.1/dkim/__main__.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     2570 2020-04-06 04:06:13.000000 dkimpy-1.1.1/dkim/arcsign.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     1774 2020-04-06 04:06:13.000000 dkimpy-1.1.1/dkim/arcverify.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4300 2022-12-02 02:29:32.000000 dkimpy-1.1.1/dkim/asn1.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4829 2023-02-28 04:59:06.000000 dkimpy-1.1.1/dkim/asyncsupport.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4610 2020-04-06 04:06:13.000000 dkimpy-1.1.1/dkim/canonicalization.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     8173 2022-12-02 02:29:32.000000 dkimpy-1.1.1/dkim/crypto.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     3628 2020-04-06 04:06:13.000000 dkimpy-1.1.1/dkim/dkimsign.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     1951 2022-12-02 02:29:32.000000 dkimpy-1.1.1/dkim/dkimverify.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4688 2022-12-02 02:29:32.000000 dkimpy-1.1.1/dkim/dknewkey.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     2982 2020-08-08 20:55:43.000000 dkimpy-1.1.1/dkim/dnsplug.py
-drwxr-xr-x   0 kitterma  (1001) kitterma  (1001)        0 2023-03-10 16:17:46.783211 dkimpy-1.1.1/dkim/tests/
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     1769 2022-12-02 02:29:32.000000 dkimpy-1.1.1/dkim/tests/__init__.py
-drwxr-xr-x   0 kitterma  (1001) kitterma  (1001)        0 2023-03-10 16:17:46.787211 dkimpy-1.1.1/dkim/tests/data/
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      887 2020-04-06 04:27:45.000000 dkimpy-1.1.1/dkim/tests/data/1024_testkey.key
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      212 2020-04-06 04:27:45.000000 dkimpy-1.1.1/dkim/tests/data/1024_testkey_wo_markers.pub.rsa.txt
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      240 2020-04-06 04:27:45.000000 dkimpy-1.1.1/dkim/tests/data/1024_testkey_wo_markers.pub.txt
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     1679 2020-04-06 04:27:45.000000 dkimpy-1.1.1/dkim/tests/data/2048_testkey.key
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     1704 2022-12-02 02:29:32.000000 dkimpy-1.1.1/dkim/tests/data/2048_testkey_PKCS8.key
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      416 2022-12-02 02:29:32.000000 dkimpy-1.1.1/dkim/tests/data/2048_testkey_PKCS8.key.pub.txt
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      384 2020-04-06 04:27:45.000000 dkimpy-1.1.1/dkim/tests/data/2048_testkey_wo_markers.pub.rsa.txt
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      416 2020-04-06 04:27:45.000000 dkimpy-1.1.1/dkim/tests/data/2048_testkey_wo_markers.pub.txt
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      251 2020-04-06 04:06:13.000000 dkimpy-1.1.1/dkim/tests/data/badk.txt
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      240 2020-04-06 04:06:13.000000 dkimpy-1.1.1/dkim/tests/data/badversion.txt
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)       58 2020-04-06 04:06:13.000000 dkimpy-1.1.1/dkim/tests/data/ed25519test.dns
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)       45 2020-04-06 04:06:13.000000 dkimpy-1.1.1/dkim/tests/data/ed25519test.key
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      346 2020-04-06 04:06:13.000000 dkimpy-1.1.1/dkim/tests/data/ed25519test.msg
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      588 2020-04-06 04:06:13.000000 dkimpy-1.1.1/dkim/tests/data/ed25519test2.msg
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)       67 2020-04-06 04:06:13.000000 dkimpy-1.1.1/dkim/tests/data/eximtest.dns
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4444 2020-04-06 04:06:13.000000 dkimpy-1.1.1/dkim/tests/data/message.mbox
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      269 2020-04-06 04:06:13.000000 dkimpy-1.1.1/dkim/tests/data/rfc6376.msg
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     1069 2020-04-06 04:06:13.000000 dkimpy-1.1.1/dkim/tests/data/rfc6376.signed.msg
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      708 2020-04-06 04:06:13.000000 dkimpy-1.1.1/dkim/tests/data/rfc6376.signed.rsa.msg
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      275 2022-12-05 20:53:17.000000 dkimpy-1.1.1/dkim/tests/data/rfc6376.w1258.msg
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)       45 2020-04-06 04:06:13.000000 dkimpy-1.1.1/dkim/tests/data/rfc8032_7_1.key
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      346 2020-04-06 04:06:13.000000 dkimpy-1.1.1/dkim/tests/data/test.message
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      778 2022-12-02 02:29:32.000000 dkimpy-1.1.1/dkim/tests/data/test.message.baddomain
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      887 2020-04-06 04:06:13.000000 dkimpy-1.1.1/dkim/tests/data/test.private
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      240 2020-04-06 04:06:13.000000 dkimpy-1.1.1/dkim/tests/data/test.txt
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     1104 2020-04-06 04:06:13.000000 dkimpy-1.1.1/dkim/tests/data/test2.message
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      887 2020-04-06 04:06:13.000000 dkimpy-1.1.1/dkim/tests/data/test2.private
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      233 2020-04-06 04:06:13.000000 dkimpy-1.1.1/dkim/tests/data/test2.txt
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      240 2020-04-06 04:06:13.000000 dkimpy-1.1.1/dkim/tests/data/test_bad.txt
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      219 2020-04-06 04:06:13.000000 dkimpy-1.1.1/dkim/tests/data/test_extra.message
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      164 2020-04-06 04:06:13.000000 dkimpy-1.1.1/dkim/tests/data/test_nofrom.message
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      250 2020-04-06 04:27:45.000000 dkimpy-1.1.1/dkim/tests/data/test_tlsrpt.txt
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     5300 2020-04-06 04:27:45.000000 dkimpy-1.1.1/dkim/tests/test_arc.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     6045 2020-04-06 04:06:13.000000 dkimpy-1.1.1/dkim/tests/test_canonicalization.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     6786 2020-04-06 04:06:13.000000 dkimpy-1.1.1/dkim/tests/test_crypto.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)    23644 2023-02-25 20:35:32.000000 dkimpy-1.1.1/dkim/tests/test_dkim.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)    12866 2020-04-06 04:27:45.000000 dkimpy-1.1.1/dkim/tests/test_dkim_ed25519.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4426 2022-12-05 21:05:46.000000 dkimpy-1.1.1/dkim/tests/test_dkim_generate.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4923 2022-12-02 02:29:32.000000 dkimpy-1.1.1/dkim/tests/test_dkim_rsavariants.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)    11980 2020-04-06 04:27:45.000000 dkimpy-1.1.1/dkim/tests/test_dkim_tlsrpt.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     1557 2020-04-06 04:27:45.000000 dkimpy-1.1.1/dkim/tests/test_dnsplug.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     3432 2020-04-06 04:06:13.000000 dkimpy-1.1.1/dkim/tests/test_util.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     2501 2020-04-06 04:06:13.000000 dkimpy-1.1.1/dkim/util.py
-drwxr-xr-x   0 kitterma  (1001) kitterma  (1001)        0 2023-03-10 16:17:46.791211 dkimpy-1.1.1/dkimpy.egg-info/
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)    10824 2023-03-10 16:17:46.000000 dkimpy-1.1.1/dkimpy.egg-info/PKG-INFO
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     1986 2023-03-10 16:17:46.000000 dkimpy-1.1.1/dkimpy.egg-info/SOURCES.txt
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)        1 2023-03-10 16:17:46.000000 dkimpy-1.1.1/dkimpy.egg-info/dependency_links.txt
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      173 2023-03-10 16:17:46.000000 dkimpy-1.1.1/dkimpy.egg-info/entry_points.txt
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)        1 2020-04-06 12:14:30.000000 dkimpy-1.1.1/dkimpy.egg-info/not-zip-safe
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)       84 2023-03-10 16:17:46.000000 dkimpy-1.1.1/dkimpy.egg-info/requires.txt
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)        5 2023-03-10 16:17:46.000000 dkimpy-1.1.1/dkimpy.egg-info/top_level.txt
-drwxr-xr-x   0 kitterma  (1001) kitterma  (1001)        0 2023-03-10 16:17:46.791211 dkimpy-1.1.1/man/
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4392 2020-04-06 04:06:13.000000 dkimpy-1.1.1/man/arcsign.1
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4152 2020-04-06 04:06:13.000000 dkimpy-1.1.1/man/arcverify.1
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4957 2020-04-06 04:06:13.000000 dkimpy-1.1.1/man/dkimsign.1
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4273 2022-12-02 02:29:32.000000 dkimpy-1.1.1/man/dkimverify.1
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4923 2020-04-06 04:06:13.000000 dkimpy-1.1.1/man/dknewkey.1
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)       38 2023-03-10 16:17:46.791211 dkimpy-1.1.1/setup.cfg
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     3387 2023-02-28 04:41:07.000000 dkimpy-1.1.1/setup.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      268 2020-04-06 04:06:13.000000 dkimpy-1.1.1/test.py
+drwxr-xr-x   0 kitterma  (1001) kitterma  (1001)        0 2023-04-09 13:34:23.106676 dkimpy-1.1.2/
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)    13427 2023-04-09 13:33:30.000000 dkimpy-1.1.2/ChangeLog
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      979 2020-04-06 04:06:13.000000 dkimpy-1.1.2/LICENSE
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      200 2020-04-06 04:27:45.000000 dkimpy-1.1.2/MANIFEST.in
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)    10824 2023-04-09 13:34:23.106676 dkimpy-1.1.2/PKG-INFO
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     7905 2023-03-31 17:07:31.000000 dkimpy-1.1.2/README.md
+drwxr-xr-x   0 kitterma  (1001) kitterma  (1001)        0 2023-04-09 13:34:23.094675 dkimpy-1.1.2/dkim/
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)    57849 2023-03-31 17:04:51.000000 dkimpy-1.1.2/dkim/__init__.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      139 2020-04-06 04:06:13.000000 dkimpy-1.1.2/dkim/__main__.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     2570 2020-04-06 04:06:13.000000 dkimpy-1.1.2/dkim/arcsign.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     1774 2020-04-06 04:06:13.000000 dkimpy-1.1.2/dkim/arcverify.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4300 2022-12-02 02:29:32.000000 dkimpy-1.1.2/dkim/asn1.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4829 2023-02-28 04:59:06.000000 dkimpy-1.1.2/dkim/asyncsupport.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4610 2020-04-06 04:06:13.000000 dkimpy-1.1.2/dkim/canonicalization.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     8173 2022-12-02 02:29:32.000000 dkimpy-1.1.2/dkim/crypto.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     3628 2020-04-06 04:06:13.000000 dkimpy-1.1.2/dkim/dkimsign.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     1951 2022-12-02 02:29:32.000000 dkimpy-1.1.2/dkim/dkimverify.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4688 2022-12-02 02:29:32.000000 dkimpy-1.1.2/dkim/dknewkey.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     2982 2020-08-08 20:55:43.000000 dkimpy-1.1.2/dkim/dnsplug.py
+drwxr-xr-x   0 kitterma  (1001) kitterma  (1001)        0 2023-04-09 13:34:23.094675 dkimpy-1.1.2/dkim/tests/
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     1769 2022-12-02 02:29:32.000000 dkimpy-1.1.2/dkim/tests/__init__.py
+drwxr-xr-x   0 kitterma  (1001) kitterma  (1001)        0 2023-04-09 13:34:23.102676 dkimpy-1.1.2/dkim/tests/data/
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      887 2020-04-06 04:27:45.000000 dkimpy-1.1.2/dkim/tests/data/1024_testkey.key
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      212 2020-04-06 04:27:45.000000 dkimpy-1.1.2/dkim/tests/data/1024_testkey_wo_markers.pub.rsa.txt
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      240 2020-04-06 04:27:45.000000 dkimpy-1.1.2/dkim/tests/data/1024_testkey_wo_markers.pub.txt
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     1679 2020-04-06 04:27:45.000000 dkimpy-1.1.2/dkim/tests/data/2048_testkey.key
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     1704 2022-12-02 02:29:32.000000 dkimpy-1.1.2/dkim/tests/data/2048_testkey_PKCS8.key
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      416 2022-12-02 02:29:32.000000 dkimpy-1.1.2/dkim/tests/data/2048_testkey_PKCS8.key.pub.txt
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      384 2020-04-06 04:27:45.000000 dkimpy-1.1.2/dkim/tests/data/2048_testkey_wo_markers.pub.rsa.txt
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      416 2020-04-06 04:27:45.000000 dkimpy-1.1.2/dkim/tests/data/2048_testkey_wo_markers.pub.txt
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      251 2020-04-06 04:06:13.000000 dkimpy-1.1.2/dkim/tests/data/badk.txt
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      240 2020-04-06 04:06:13.000000 dkimpy-1.1.2/dkim/tests/data/badversion.txt
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)       58 2020-04-06 04:06:13.000000 dkimpy-1.1.2/dkim/tests/data/ed25519test.dns
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)       45 2020-04-06 04:06:13.000000 dkimpy-1.1.2/dkim/tests/data/ed25519test.key
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      346 2020-04-06 04:06:13.000000 dkimpy-1.1.2/dkim/tests/data/ed25519test.msg
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      588 2020-04-06 04:06:13.000000 dkimpy-1.1.2/dkim/tests/data/ed25519test2.msg
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)       67 2020-04-06 04:06:13.000000 dkimpy-1.1.2/dkim/tests/data/eximtest.dns
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4444 2020-04-06 04:06:13.000000 dkimpy-1.1.2/dkim/tests/data/message.mbox
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      269 2020-04-06 04:06:13.000000 dkimpy-1.1.2/dkim/tests/data/rfc6376.msg
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     1069 2020-04-06 04:06:13.000000 dkimpy-1.1.2/dkim/tests/data/rfc6376.signed.msg
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      708 2020-04-06 04:06:13.000000 dkimpy-1.1.2/dkim/tests/data/rfc6376.signed.rsa.msg
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      275 2022-12-05 20:53:17.000000 dkimpy-1.1.2/dkim/tests/data/rfc6376.w1258.msg
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)       45 2020-04-06 04:06:13.000000 dkimpy-1.1.2/dkim/tests/data/rfc8032_7_1.key
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      346 2020-04-06 04:06:13.000000 dkimpy-1.1.2/dkim/tests/data/test.message
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      778 2022-12-02 02:29:32.000000 dkimpy-1.1.2/dkim/tests/data/test.message.baddomain
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      887 2020-04-06 04:06:13.000000 dkimpy-1.1.2/dkim/tests/data/test.private
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      240 2020-04-06 04:06:13.000000 dkimpy-1.1.2/dkim/tests/data/test.txt
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     1104 2020-04-06 04:06:13.000000 dkimpy-1.1.2/dkim/tests/data/test2.message
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      887 2020-04-06 04:06:13.000000 dkimpy-1.1.2/dkim/tests/data/test2.private
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      233 2020-04-06 04:06:13.000000 dkimpy-1.1.2/dkim/tests/data/test2.txt
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      240 2020-04-06 04:06:13.000000 dkimpy-1.1.2/dkim/tests/data/test_bad.txt
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      219 2020-04-06 04:06:13.000000 dkimpy-1.1.2/dkim/tests/data/test_extra.message
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      164 2020-04-06 04:06:13.000000 dkimpy-1.1.2/dkim/tests/data/test_nofrom.message
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      250 2020-04-06 04:27:45.000000 dkimpy-1.1.2/dkim/tests/data/test_tlsrpt.txt
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     5300 2020-04-06 04:27:45.000000 dkimpy-1.1.2/dkim/tests/test_arc.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     6045 2020-04-06 04:06:13.000000 dkimpy-1.1.2/dkim/tests/test_canonicalization.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     6786 2020-04-06 04:06:13.000000 dkimpy-1.1.2/dkim/tests/test_crypto.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)    23644 2023-02-25 20:35:32.000000 dkimpy-1.1.2/dkim/tests/test_dkim.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)    12866 2020-04-06 04:27:45.000000 dkimpy-1.1.2/dkim/tests/test_dkim_ed25519.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4426 2022-12-05 21:05:46.000000 dkimpy-1.1.2/dkim/tests/test_dkim_generate.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4923 2022-12-02 02:29:32.000000 dkimpy-1.1.2/dkim/tests/test_dkim_rsavariants.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)    11980 2020-04-06 04:27:45.000000 dkimpy-1.1.2/dkim/tests/test_dkim_tlsrpt.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     1557 2020-04-06 04:27:45.000000 dkimpy-1.1.2/dkim/tests/test_dnsplug.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     3432 2020-04-06 04:06:13.000000 dkimpy-1.1.2/dkim/tests/test_util.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     2501 2020-04-06 04:06:13.000000 dkimpy-1.1.2/dkim/util.py
+drwxr-xr-x   0 kitterma  (1001) kitterma  (1001)        0 2023-04-09 13:34:23.102676 dkimpy-1.1.2/dkimpy.egg-info/
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)    10824 2023-04-09 13:34:22.000000 dkimpy-1.1.2/dkimpy.egg-info/PKG-INFO
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     1986 2023-04-09 13:34:23.000000 dkimpy-1.1.2/dkimpy.egg-info/SOURCES.txt
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)        1 2023-04-09 13:34:22.000000 dkimpy-1.1.2/dkimpy.egg-info/dependency_links.txt
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      173 2023-04-09 13:34:22.000000 dkimpy-1.1.2/dkimpy.egg-info/entry_points.txt
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)        1 2020-04-06 12:14:30.000000 dkimpy-1.1.2/dkimpy.egg-info/not-zip-safe
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)       84 2023-04-09 13:34:22.000000 dkimpy-1.1.2/dkimpy.egg-info/requires.txt
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)        5 2023-04-09 13:34:22.000000 dkimpy-1.1.2/dkimpy.egg-info/top_level.txt
+drwxr-xr-x   0 kitterma  (1001) kitterma  (1001)        0 2023-04-09 13:34:23.106676 dkimpy-1.1.2/man/
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4392 2020-04-06 04:06:13.000000 dkimpy-1.1.2/man/arcsign.1
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4152 2020-04-06 04:06:13.000000 dkimpy-1.1.2/man/arcverify.1
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4957 2020-04-06 04:06:13.000000 dkimpy-1.1.2/man/dkimsign.1
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4273 2022-12-02 02:29:32.000000 dkimpy-1.1.2/man/dkimverify.1
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4923 2020-04-06 04:06:13.000000 dkimpy-1.1.2/man/dknewkey.1
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)       38 2023-04-09 13:34:23.106676 dkimpy-1.1.2/setup.cfg
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     3387 2023-03-31 17:07:05.000000 dkimpy-1.1.2/setup.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      268 2020-04-06 04:06:13.000000 dkimpy-1.1.2/test.py
```

### Comparing `dkimpy-1.1.1/ChangeLog` & `dkimpy-1.1.2/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-04-09 Version 1.1.2
+   - Verify correct AMS header is used for ARC seal verification (André Cruz)
+
 2023-03-09 Version 1.1.1
     - Document dropping of Python 2 support (dropped as of 1.1.0) (LP:
       #20086738)
     - Fix traceback when attempting to verify an unsigned message using
       async verify (Thanks to Nikita Sychev for the report and a suggested
       fix) (LP: #2008723)
```

### Comparing `dkimpy-1.1.1/LICENSE` & `dkimpy-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.1/PKG-INFO` & `dkimpy-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkimpy
-Version: 1.1.1
+Version: 1.1.2
 Summary: DKIM (DomainKeys Identified Mail), ARC (Authenticated Receive Chain), and TLSRPT (TLS Report) email signing and verification
 Home-page: https://launchpad.net/dkimpy
 Author: Scott Kitterman
 Author-email: scott@kitterman.com
 License: BSD-like
 Description: dkimpy - DKIM (DomainKeys Identified Mail)
         https://launchpad.net/dkimpy/
@@ -17,15 +17,15 @@
         dkimpy is a library that implements DKIM (DomainKeys Identified Mail) email
         signing and verification.  Basic DKIM requirements are defined in RFC 6376:
         
         https://tools.ietf.org/html/rfc6376
         
         # VERSION
         
-        This is dkimpy 1.1.1.
+        This is dkimpy 1.1.2.
         
         # REQUIREMENTS
         
         Dependencies will be automatically included for normal DKIM usage.  The
         extras_requires feature 'ed25519' will add the dependencies needed for signing
         and verifying using the new DCRUP ed25519-sha256 algorithm.  The
         extras_requires feature 'ARC' will add the extra dependencies needed for ARC.
```

### Comparing `dkimpy-1.1.1/README.md` & `dkimpy-1.1.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 dkimpy is a library that implements DKIM (DomainKeys Identified Mail) email
 signing and verification.  Basic DKIM requirements are defined in RFC 6376:
 
 https://tools.ietf.org/html/rfc6376
 
 # VERSION
 
-This is dkimpy 1.1.1.
+This is dkimpy 1.1.2.
 
 # REQUIREMENTS
 
 Dependencies will be automatically included for normal DKIM usage.  The
 extras_requires feature 'ed25519' will add the dependencies needed for signing
 and verifying using the new DCRUP ed25519-sha256 algorithm.  The
 extras_requires feature 'ARC' will add the extra dependencies needed for ARC.
```

### Comparing `dkimpy-1.1.1/dkim/__init__.py` & `dkimpy-1.1.2/dkim/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1289,15 +1289,17 @@
 
     ams_header = (b'ARC-Message-Signature', b' ' + ams_value)
 
 
     # we can't use the AMS provided above, as it's already been canonicalized relaxed
     # for use in validating the AS.  However the AMS is included in the AMS itself,
     # and this can use simple canonicalization
-    raw_ams_header = [(x, y) for (x, y) in self.headers if x.lower() == b'arc-message-signature'][0]
+    raw_ams_header = [
+       (x, y) for (x, y) in self.headers if x.lower() == b'arc-message-signature' and b" i="+sig[b'i']+b";" in y.lower()
+    ][0]
 
     # Only relaxed canonicalization used by ARC
     if b'c' not in sig:
         sig[b'c'] = b'relaxed/relaxed'
     try:
       ams_valid = self.verify_sig(sig, include_headers, raw_ams_header, dnsfunc)
     except DKIMException as e:
```

### Comparing `dkimpy-1.1.1/dkim/arcsign.py` & `dkimpy-1.1.2/dkim/arcsign.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.1/dkim/arcverify.py` & `dkimpy-1.1.2/dkim/arcverify.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.1/dkim/asn1.py` & `dkimpy-1.1.2/dkim/asn1.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.1/dkim/asyncsupport.py` & `dkimpy-1.1.2/dkim/asyncsupport.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.1/dkim/canonicalization.py` & `dkimpy-1.1.2/dkim/canonicalization.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.1/dkim/crypto.py` & `dkimpy-1.1.2/dkim/crypto.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.1/dkim/dkimsign.py` & `dkimpy-1.1.2/dkim/dkimsign.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.1/dkim/dkimverify.py` & `dkimpy-1.1.2/dkim/dkimverify.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.1/dkim/dknewkey.py` & `dkimpy-1.1.2/dkim/dknewkey.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.1/dkim/dnsplug.py` & `dkimpy-1.1.2/dkim/dnsplug.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.1/dkim/tests/__init__.py` & `dkimpy-1.1.2/dkim/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.1/dkim/tests/data/1024_testkey.key` & `dkimpy-1.1.2/dkim/tests/data/1024_testkey.key`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.1/dkim/tests/data/2048_testkey.key` & `dkimpy-1.1.2/dkim/tests/data/2048_testkey.key`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.1/dkim/tests/data/2048_testkey_PKCS8.key` & `dkimpy-1.1.2/dkim/tests/data/2048_testkey_PKCS8.key`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.1/dkim/tests/data/ed25519test2.msg` & `dkimpy-1.1.2/dkim/tests/data/ed25519test2.msg`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.1/dkim/tests/data/message.mbox` & `dkimpy-1.1.2/dkim/tests/data/message.mbox`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.1/dkim/tests/data/rfc6376.signed.msg` & `dkimpy-1.1.2/dkim/tests/data/rfc6376.signed.msg`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.1/dkim/tests/data/rfc6376.signed.rsa.msg` & `dkimpy-1.1.2/dkim/tests/data/rfc6376.signed.rsa.msg`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.1/dkim/tests/data/test.message.baddomain` & `dkimpy-1.1.2/dkim/tests/data/test.message.baddomain`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.1/dkim/tests/data/test.private` & `dkimpy-1.1.2/dkim/tests/data/test.private`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.1/dkim/tests/data/test2.message` & `dkimpy-1.1.2/dkim/tests/data/test2.message`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.1/dkim/tests/data/test2.private` & `dkimpy-1.1.2/dkim/tests/data/test2.private`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.1/dkim/tests/test_arc.py` & `dkimpy-1.1.2/dkim/tests/test_arc.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.1/dkim/tests/test_canonicalization.py` & `dkimpy-1.1.2/dkim/tests/test_canonicalization.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.1/dkim/tests/test_crypto.py` & `dkimpy-1.1.2/dkim/tests/test_crypto.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.1/dkim/tests/test_dkim.py` & `dkimpy-1.1.2/dkim/tests/test_dkim.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.1/dkim/tests/test_dkim_ed25519.py` & `dkimpy-1.1.2/dkim/tests/test_dkim_ed25519.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.1/dkim/tests/test_dkim_generate.py` & `dkimpy-1.1.2/dkim/tests/test_dkim_generate.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.1/dkim/tests/test_dkim_rsavariants.py` & `dkimpy-1.1.2/dkim/tests/test_dkim_rsavariants.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.1/dkim/tests/test_dkim_tlsrpt.py` & `dkimpy-1.1.2/dkim/tests/test_dkim_tlsrpt.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.1/dkim/tests/test_dnsplug.py` & `dkimpy-1.1.2/dkim/tests/test_dnsplug.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.1/dkim/tests/test_util.py` & `dkimpy-1.1.2/dkim/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.1/dkim/util.py` & `dkimpy-1.1.2/dkim/util.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.1/dkimpy.egg-info/PKG-INFO` & `dkimpy-1.1.2/dkimpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkimpy
-Version: 1.1.1
+Version: 1.1.2
 Summary: DKIM (DomainKeys Identified Mail), ARC (Authenticated Receive Chain), and TLSRPT (TLS Report) email signing and verification
 Home-page: https://launchpad.net/dkimpy
 Author: Scott Kitterman
 Author-email: scott@kitterman.com
 License: BSD-like
 Description: dkimpy - DKIM (DomainKeys Identified Mail)
         https://launchpad.net/dkimpy/
@@ -17,15 +17,15 @@
         dkimpy is a library that implements DKIM (DomainKeys Identified Mail) email
         signing and verification.  Basic DKIM requirements are defined in RFC 6376:
         
         https://tools.ietf.org/html/rfc6376
         
         # VERSION
         
-        This is dkimpy 1.1.1.
+        This is dkimpy 1.1.2.
         
         # REQUIREMENTS
         
         Dependencies will be automatically included for normal DKIM usage.  The
         extras_requires feature 'ed25519' will add the dependencies needed for signing
         and verifying using the new DCRUP ed25519-sha256 algorithm.  The
         extras_requires feature 'ARC' will add the extra dependencies needed for ARC.
```

### Comparing `dkimpy-1.1.1/dkimpy.egg-info/SOURCES.txt` & `dkimpy-1.1.2/dkimpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.1/man/arcsign.1` & `dkimpy-1.1.2/man/arcsign.1`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.1/man/arcverify.1` & `dkimpy-1.1.2/man/arcverify.1`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.1/man/dkimsign.1` & `dkimpy-1.1.2/man/dkimsign.1`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.1/man/dkimverify.1` & `dkimpy-1.1.2/man/dkimverify.1`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.1/man/dknewkey.1` & `dkimpy-1.1.2/man/dknewkey.1`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.1/setup.py` & `dkimpy-1.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 # This has been modified from the original software.
 # Copyright (c) 2011,2012,2018 Scott Kitterman <scott@kitterman.com>
 
 from setuptools import setup
 import os
 import sys
 
-version = "1.1.1"
+version = "1.1.2"
 
 kw = {}  # Work-around for lack of 'or' requires in setuptools.
 try:
     import DNS
     kw['install_requires'] = ['Py3DNS']
 except ImportError:  # If PyDNS is not installed, prefer dnspython
     kw['install_requires'] = ['dnspython>=1.16.0']
```

