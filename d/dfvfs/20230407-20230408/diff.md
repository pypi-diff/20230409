# Comparing `tmp/dfvfs-20230407.tar.gz` & `tmp/dfvfs-20230408.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfvfs-20230407.tar", last modified: Fri Apr  7 07:38:18 2023, max compression
+gzip compressed data, was "dfvfs-20230408.tar", last modified: Sun Apr  9 13:43:04 2023, max compression
```

## Comparing `dfvfs-20230407.tar` & `dfvfs-20230408.tar`

### file list

```diff
@@ -1,686 +1,686 @@
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-07 07:38:18.519766 dfvfs-20230407/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-07 07:38:18.133765 dfvfs-20230407/.github/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-07 07:38:18.216765 dfvfs-20230407/.github/workflows/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3491 2023-01-14 16:01:33.000000 dfvfs-20230407/.github/workflows/test_docker.yml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1857 2023-01-14 16:01:33.000000 dfvfs-20230407/.github/workflows/test_docs.yml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2158 2023-01-14 16:01:33.000000 dfvfs-20230407/.github/workflows/test_tox.yml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22087 2022-12-29 16:06:04.000000 dfvfs-20230407/.pylintrc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      149 2022-12-29 15:59:10.000000 dfvfs-20230407/.yamllint.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1173 2022-11-21 19:14:36.000000 dfvfs-20230407/ACKNOWLEDGEMENTS
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      360 2022-11-21 19:18:17.000000 dfvfs-20230407/AUTHORS
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11358 2022-11-21 19:18:17.000000 dfvfs-20230407/LICENSE
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      632 2022-12-29 15:59:10.000000 dfvfs-20230407/MANIFEST.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      552 2022-12-29 15:59:10.000000 dfvfs-20230407/MANIFEST.test_data.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      900 2023-04-07 07:38:18.520766 dfvfs-20230407/PKG-INFO
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      473 2022-11-21 19:14:36.000000 dfvfs-20230407/README
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1794 2022-12-29 16:06:05.000000 dfvfs-20230407/appveyor.yml
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-07 07:38:18.134765 dfvfs-20230407/config/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-07 07:38:18.217765 dfvfs-20230407/config/appveyor/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1008 2023-01-14 16:01:33.000000 dfvfs-20230407/config/appveyor/install.ps1
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      125 2022-12-29 16:06:05.000000 dfvfs-20230407/config/appveyor/install.sh
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      620 2022-12-29 16:06:05.000000 dfvfs-20230407/config/appveyor/runtests.sh
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-07 07:38:18.218766 dfvfs-20230407/config/dpkg/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      168 2023-04-07 07:26:35.000000 dfvfs-20230407/config/dpkg/changelog
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       32 2022-11-21 19:18:17.000000 dfvfs-20230407/config/dpkg/clean
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        2 2022-12-29 16:06:05.000000 dfvfs-20230407/config/dpkg/compat
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2023-01-14 16:01:33.000000 dfvfs-20230407/config/dpkg/control
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      948 2022-11-21 19:18:17.000000 dfvfs-20230407/config/dpkg/copyright
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      122 2022-12-29 16:06:05.000000 dfvfs-20230407/config/dpkg/rules
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-07 07:38:18.218766 dfvfs-20230407/config/dpkg/source/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       12 2022-11-21 19:18:17.000000 dfvfs-20230407/config/dpkg/source/format
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-07 07:38:18.219766 dfvfs-20230407/config/pylint/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1673 2022-11-21 19:18:17.000000 dfvfs-20230407/config/pylint/spelling-private-dict
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4978 2023-01-14 16:01:33.000000 dfvfs-20230407/dependencies.ini
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-07 07:38:18.219766 dfvfs-20230407/dfvfs/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      278 2023-04-07 07:26:35.000000 dfvfs-20230407/dfvfs/__init__.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-07 07:38:18.260765 dfvfs-20230407/dfvfs/analyzer/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2022-12-29 15:59:10.000000 dfvfs-20230407/dfvfs/analyzer/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13902 2022-12-29 15:59:10.000000 dfvfs-20230407/dfvfs/analyzer/analyzer.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2083 2022-12-29 15:59:10.000000 dfvfs-20230407/dfvfs/analyzer/analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      962 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/analyzer/apfs_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1010 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/analyzer/apfs_container_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1120 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/analyzer/bde_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1087 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/analyzer/bzip2_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1404 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/analyzer/cpio_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      978 2022-12-29 15:59:10.000000 dfvfs-20230407/dfvfs/analyzer/cs_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1182 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/analyzer/ewf_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1182 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/analyzer/ext_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1547 2022-12-29 15:59:10.000000 dfvfs-20230407/dfvfs/analyzer/fat_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1395 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/analyzer/gpt_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      964 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/analyzer/gzip_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1370 2022-12-29 15:59:10.000000 dfvfs-20230407/dfvfs/analyzer/hfs_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      971 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/analyzer/luksde_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1174 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/analyzer/lvm_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1168 2022-12-29 15:59:10.000000 dfvfs-20230407/dfvfs/analyzer/modi_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1186 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/analyzer/ntfs_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1003 2022-12-29 15:59:10.000000 dfvfs-20230407/dfvfs/analyzer/phdi_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1246 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/analyzer/qcow_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4938 2022-12-29 15:59:10.000000 dfvfs-20230407/dfvfs/analyzer/specification.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1057 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/analyzer/tar_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2266 2022-12-29 15:59:10.000000 dfvfs-20230407/dfvfs/analyzer/tsk_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1040 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/analyzer/tsk_partition_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1192 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/analyzer/vhdi_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1194 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/analyzer/vmdk_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1071 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/analyzer/vshadow_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      955 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/analyzer/xfs_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      968 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/analyzer/xz_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      950 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/analyzer/zip_analyzer_helper.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-07 07:38:18.261766 dfvfs-20230407/dfvfs/compression/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      247 2022-11-21 19:17:56.000000 dfvfs-20230407/dfvfs/compression/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1355 2022-12-29 15:59:10.000000 dfvfs-20230407/dfvfs/compression/bzip2_decompressor.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      437 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/compression/decompressor.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2286 2022-12-29 15:59:10.000000 dfvfs-20230407/dfvfs/compression/manager.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2139 2022-12-29 15:59:10.000000 dfvfs-20230407/dfvfs/compression/xz_decompressor.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2118 2022-12-29 15:59:10.000000 dfvfs-20230407/dfvfs/compression/zlib_decompressor.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-07 07:38:18.263765 dfvfs-20230407/dfvfs/credentials/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      313 2022-12-29 15:59:10.000000 dfvfs-20230407/dfvfs/credentials/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      545 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/credentials/apfs_credentials.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      646 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/credentials/bde_credentials.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      562 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/credentials/credentials.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      544 2022-12-29 15:59:10.000000 dfvfs-20230407/dfvfs/credentials/cs_credentials.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      497 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/credentials/encrypted_stream_credentials.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2696 2022-12-29 15:59:10.000000 dfvfs-20230407/dfvfs/credentials/keychain.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      498 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/credentials/luksde_credentials.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1902 2022-12-29 15:59:10.000000 dfvfs-20230407/dfvfs/credentials/manager.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-07 07:38:18.264766 dfvfs-20230407/dfvfs/encoding/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      191 2022-11-21 19:18:12.000000 dfvfs-20230407/dfvfs/encoding/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      967 2022-12-29 15:59:10.000000 dfvfs-20230407/dfvfs/encoding/base16_decoder.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      967 2022-12-29 15:59:10.000000 dfvfs-20230407/dfvfs/encoding/base32_decoder.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1198 2022-12-29 15:59:10.000000 dfvfs-20230407/dfvfs/encoding/base64_decoder.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      392 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/encoding/decoder.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1955 2022-12-29 15:59:10.000000 dfvfs-20230407/dfvfs/encoding/manager.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-07 07:38:18.266765 dfvfs-20230407/dfvfs/encryption/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      245 2022-11-25 17:21:27.000000 dfvfs-20230407/dfvfs/encryption/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1478 2022-12-29 15:59:10.000000 dfvfs-20230407/dfvfs/encryption/aes_decrypter.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1513 2022-12-29 15:59:10.000000 dfvfs-20230407/dfvfs/encryption/blowfish_decrypter.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3897 2022-12-29 15:59:10.000000 dfvfs-20230407/dfvfs/encryption/decrypter.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1502 2022-12-29 15:59:10.000000 dfvfs-20230407/dfvfs/encryption/des3_decrypter.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2274 2022-12-29 15:59:10.000000 dfvfs-20230407/dfvfs/encryption/manager.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1771 2022-12-29 15:59:10.000000 dfvfs-20230407/dfvfs/encryption/rc4_decrypter.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-07 07:38:18.273765 dfvfs-20230407/dfvfs/file_io/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-12-29 15:59:10.000000 dfvfs-20230407/dfvfs/file_io/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3960 2022-12-29 15:59:10.000000 dfvfs-20230407/dfvfs/file_io/apfs_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/file_io/bde_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9503 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/file_io/compressed_stream_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4645 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/file_io/cpio_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4663 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/file_io/cs_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5995 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/file_io/data_range_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9664 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/file_io/encoded_stream_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10632 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/file_io/encrypted_stream_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2710 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/file_io/ewf_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3948 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/file_io/ext_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/file_io/fake_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4398 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/file_io/fat_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4882 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/file_io/file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4157 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/file_io/file_object_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5577 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/file_io/gpt_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2401 2023-01-14 16:01:33.000000 dfvfs-20230407/dfvfs/file_io/gzip_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4501 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/file_io/hfs_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1272 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/file_io/luksde_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3978 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/file_io/lvm_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1856 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/file_io/modi_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4540 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/file_io/ntfs_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6180 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/file_io/os_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4378 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/file_io/phdi_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4074 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/file_io/qcow_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2733 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/file_io/raw_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8349 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/file_io/sqlite_blob_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4775 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/file_io/tar_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7991 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/file_io/tsk_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2370 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/file_io/tsk_partition_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4313 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/file_io/vhdi_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4201 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/file_io/vmdk_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4106 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/file_io/vshadow_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3941 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/file_io/xfs_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9026 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/file_io/zip_file_io.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-07 07:38:18.275766 dfvfs-20230407/dfvfs/helpers/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/helpers/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29824 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/helpers/command_line.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2093 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/helpers/data_slice.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3992 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/helpers/fake_file_system_builder.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22280 2023-04-07 07:26:35.000000 dfvfs-20230407/dfvfs/helpers/file_system_searcher.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30704 2023-04-07 04:40:26.000000 dfvfs-20230407/dfvfs/helpers/source_scanner.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6081 2022-12-23 11:41:15.000000 dfvfs-20230407/dfvfs/helpers/text_file.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28568 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/helpers/volume_scanner.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9518 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/helpers/windows_path_resolver.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-07 07:38:18.279765 dfvfs-20230407/dfvfs/lib/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/lib/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1687 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/lib/apfs_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1710 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/lib/bde_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10516 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/lib/cpio.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4230 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/lib/cpio.yaml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1677 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/lib/cs_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3532 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/lib/data_format.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      710 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/lib/decorators.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4694 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/lib/definitions.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1053 2022-11-21 19:18:10.000000 dfvfs-20230407/dfvfs/lib/errors.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3502 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/lib/ewf_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2345 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/lib/glob2regex.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      723 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/lib/gpt_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19596 2023-01-14 16:01:33.000000 dfvfs-20230407/dfvfs/lib/gzipfile.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1489 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/lib/gzipfile.yaml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1160 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/lib/luksde_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      866 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/lib/lvm_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12570 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/lib/raw_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5970 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/lib/sqlite_database.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1775 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/lib/tsk_image.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4930 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/lib/tsk_partition.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      745 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/lib/vshadow_helper.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-07 07:38:18.280766 dfvfs-20230407/dfvfs/mount/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/mount/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2036 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/mount/manager.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-07 07:38:18.288766 dfvfs-20230407/dfvfs/path/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1413 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/path/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1564 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/path/apfs_container_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1547 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/path/apfs_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1769 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/path/bde_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1387 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/path/compressed_stream_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      965 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/path/cpio_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2397 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/path/cs_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1517 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/path/data_range_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1332 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/path/encoded_stream_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2414 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/path/encrypted_stream_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      777 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/path/ewf_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1475 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/path/ext_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3742 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/path/factory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      940 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/path/fake_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1560 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/path/fat_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1474 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/path/gpt_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      782 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/path/gzip_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1932 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/path/hfs_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      923 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/path/location_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1217 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/path/luksde_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1482 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/path/lvm_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      798 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/path/modi_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1102 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/path/mount_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2364 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/path/ntfs_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/path/os_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4043 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/path/path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      784 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/path/phdi_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      779 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/path/qcow_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      800 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/path/raw_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2964 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/path/sqlite_blob_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      947 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/path/tar_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1777 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/path/tsk_partition_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1943 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/path/tsk_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      810 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/path/vhdi_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      784 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/path/vmdk_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1499 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/path/vshadow_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1475 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/path/xfs_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      978 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/path/zip_path_spec.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-07 07:38:18.288766 dfvfs-20230407/dfvfs/resolver/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:17:56.000000 dfvfs-20230407/dfvfs/resolver/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4365 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/resolver/context.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6142 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/resolver/resolver.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-07 07:38:18.297766 dfvfs-20230407/dfvfs/resolver_helpers/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2723 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/resolver_helpers/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      904 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/resolver_helpers/apfs_container_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1195 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/resolver_helpers/apfs_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1195 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/resolver_helpers/bde_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1329 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/resolver_helpers/compressed_stream_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1246 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/resolver_helpers/cpio_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1198 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/resolver_helpers/cs_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1252 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/resolver_helpers/data_range_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1296 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/resolver_helpers/encoded_stream_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1318 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/resolver_helpers/encrypted_stream_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      824 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/resolver_helpers/ewf_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1184 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/resolver_helpers/ext_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      522 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/resolver_helpers/fake_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1184 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/resolver_helpers/fat_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1207 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/resolver_helpers/gpt_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1205 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/resolver_helpers/gzip_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1184 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/resolver_helpers/hfs_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/resolver_helpers/luksde_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1209 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/resolver_helpers/lvm_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1928 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/resolver_helpers/manager.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      846 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/resolver_helpers/modi_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1195 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/resolver_helpers/ntfs_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1201 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/resolver_helpers/os_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      832 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/resolver_helpers/phdi_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      832 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/resolver_helpers/qcow_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      838 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/resolver_helpers/raw_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/resolver_helpers/resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1300 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/resolver_helpers/sqlite_blob_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1184 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/resolver_helpers/tar_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1312 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/resolver_helpers/tsk_partition_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1208 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/resolver_helpers/tsk_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      830 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/resolver_helpers/vhdi_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      832 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/resolver_helpers/vmdk_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1246 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/resolver_helpers/vshadow_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1184 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/resolver_helpers/xfs_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1184 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/resolver_helpers/zip_resolver_helper.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-07 07:38:18.298766 dfvfs-20230407/dfvfs/serializer/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:18:12.000000 dfvfs-20230407/dfvfs/serializer/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5458 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/serializer/json_serializer.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/serializer/serializer.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-07 07:38:18.311766 dfvfs-20230407/dfvfs/vfs/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:17:59.000000 dfvfs-20230407/dfvfs/vfs/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3622 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/apfs_attribute.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/apfs_container_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4534 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/apfs_container_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4513 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/apfs_container_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/apfs_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8895 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/apfs_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6044 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/apfs_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2064 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/attribute.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2188 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/bde_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2758 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/bde_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1637 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/compressed_stream_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2621 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/vfs/compressed_stream_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/cpio_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7019 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/cpio_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4635 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/cpio_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1112 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/cs_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4353 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/cs_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5012 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/cs_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1335 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/vfs/data_range_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2781 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/vfs/data_range_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      859 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/data_stream.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      961 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/encoded_stream_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2534 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/vfs/encoded_stream_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/encrypted_stream_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2699 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/vfs/encrypted_stream_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3601 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/ext_attribute.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1434 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/ext_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9823 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/ext_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5159 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/vfs/ext_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      844 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/extent.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1212 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/fake_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4684 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/fake_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5004 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/fake_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1437 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/fat_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7675 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/fat_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5634 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/fat_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11742 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7136 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1085 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/gpt_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3578 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/gpt_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4352 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/gpt_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1849 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/vfs/gzip_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1019 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/vfs/gzip_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3601 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/hfs_attribute.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1378 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/hfs_data_stream.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1437 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/hfs_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10348 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/hfs_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5316 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/hfs_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1944 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/luksde_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2856 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/luksde_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/lvm_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3835 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/lvm_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4750 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/lvm_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5041 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/ntfs_attribute.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1411 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/ntfs_data_stream.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1838 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/ntfs_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12181 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/ntfs_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5882 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/vfs/ntfs_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3067 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/os_attribute.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1662 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/os_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9286 2023-01-01 18:32:24.000000 dfvfs-20230407/dfvfs/vfs/os_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6345 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/os_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      665 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/vfs/root_only_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1699 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/root_only_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1853 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/sqlite_blob_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4202 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/sqlite_blob_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3520 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/vfs/sqlite_blob_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2093 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/tar_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6442 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/tar_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5180 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/tar_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4281 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/tsk_attribute.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3018 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/tsk_data_stream.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4156 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/tsk_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27588 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/tsk_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7175 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/tsk_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1865 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/tsk_partition_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4278 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/tsk_partition_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4196 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/tsk_partition_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1128 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/vshadow_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4224 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/vshadow_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4412 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/vshadow_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3601 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/xfs_attribute.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1434 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/xfs_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8567 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/xfs_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5313 2022-12-23 11:39:27.000000 dfvfs-20230407/dfvfs/vfs/xfs_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2261 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/zip_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6332 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/zip_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4975 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/vfs/zip_file_system.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-07 07:38:18.312765 dfvfs-20230407/dfvfs/volume/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      332 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/volume/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2022-12-29 15:59:11.000000 dfvfs-20230407/dfvfs/volume/apfs_volume_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1513 2022-12-29 15:59:12.000000 dfvfs-20230407/dfvfs/volume/cs_volume_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1710 2022-12-29 15:59:12.000000 dfvfs-20230407/dfvfs/volume/factory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1427 2022-12-29 15:59:12.000000 dfvfs-20230407/dfvfs/volume/gpt_volume_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1539 2022-12-29 15:59:12.000000 dfvfs-20230407/dfvfs/volume/lvm_volume_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3054 2022-12-29 15:59:12.000000 dfvfs-20230407/dfvfs/volume/tsk_volume_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7299 2022-12-29 15:59:12.000000 dfvfs-20230407/dfvfs/volume/volume_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2017 2022-12-29 15:59:12.000000 dfvfs-20230407/dfvfs/volume/vshadow_volume_system.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-07 07:38:18.234765 dfvfs-20230407/dfvfs.egg-info/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      900 2023-04-07 07:38:14.000000 dfvfs-20230407/dfvfs.egg-info/PKG-INFO
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    20370 2023-04-07 07:38:17.000000 dfvfs-20230407/dfvfs.egg-info/SOURCES.txt
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        1 2023-04-07 07:38:14.000000 dfvfs-20230407/dfvfs.egg-info/dependency_links.txt
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        1 2022-11-21 19:14:18.000000 dfvfs-20230407/dfvfs.egg-info/not-zip-safe
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      696 2023-04-07 07:38:15.000000 dfvfs-20230407/dfvfs.egg-info/requires.txt
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        6 2023-04-07 07:38:15.000000 dfvfs-20230407/dfvfs.egg-info/top_level.txt
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1017 2022-12-29 15:59:10.000000 dfvfs-20230407/dfvfs.ini
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-07 07:38:18.338765 dfvfs-20230407/docs/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5037 2022-12-29 16:06:05.000000 dfvfs-20230407/docs/conf.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2022-12-29 15:59:12.000000 dfvfs-20230407/docs/index.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      105 2022-12-29 16:06:16.000000 dfvfs-20230407/docs/requirements.txt
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-07 07:38:18.353766 dfvfs-20230407/docs/sources/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3182 2022-12-29 15:59:12.000000 dfvfs-20230407/docs/sources/Code-snippets.md
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14179 2022-12-29 15:59:12.000000 dfvfs-20230407/docs/sources/Path-specifications.md
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3922 2022-12-29 15:59:12.000000 dfvfs-20230407/docs/sources/Supported-formats.md
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-07 07:38:18.409766 dfvfs-20230407/docs/sources/api/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6080 2022-12-29 15:59:12.000000 dfvfs-20230407/docs/sources/api/dfvfs.analyzer.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1125 2022-12-23 11:39:27.000000 dfvfs-20230407/docs/sources/api/dfvfs.compression.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1704 2022-12-29 15:59:12.000000 dfvfs-20230407/docs/sources/api/dfvfs.credentials.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1032 2022-12-23 11:39:27.000000 dfvfs-20230407/docs/sources/api/dfvfs.encoding.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1264 2022-12-23 11:39:27.000000 dfvfs-20230407/docs/sources/api/dfvfs.encryption.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6140 2022-12-29 15:59:12.000000 dfvfs-20230407/docs/sources/api/dfvfs.file_io.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1629 2022-12-23 11:39:27.000000 dfvfs-20230407/docs/sources/api/dfvfs.helpers.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3042 2022-12-29 15:59:12.000000 dfvfs-20230407/docs/sources/api/dfvfs.lib.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      325 2022-12-23 11:39:27.000000 dfvfs-20230407/docs/sources/api/dfvfs.mount.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6547 2022-12-29 15:59:12.000000 dfvfs-20230407/docs/sources/api/dfvfs.path.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      501 2022-12-29 15:59:12.000000 dfvfs-20230407/docs/sources/api/dfvfs.resolver.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8176 2022-12-29 15:59:12.000000 dfvfs-20230407/docs/sources/api/dfvfs.resolver_helpers.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      461 2022-11-21 19:15:00.000000 dfvfs-20230407/docs/sources/api/dfvfs.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      551 2022-12-23 11:39:27.000000 dfvfs-20230407/docs/sources/api/dfvfs.serializer.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15405 2022-12-29 15:59:12.000000 dfvfs-20230407/docs/sources/api/dfvfs.vfs.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2022-12-29 15:59:12.000000 dfvfs-20230407/docs/sources/api/dfvfs.volume.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       52 2022-11-21 19:15:00.000000 dfvfs-20230407/docs/sources/api/modules.rst
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-07 07:38:18.426766 dfvfs-20230407/docs/sources/developer/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6837 2022-12-23 11:39:27.000000 dfvfs-20230407/docs/sources/developer/Adding-new-type.md
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5996 2022-12-23 11:39:27.000000 dfvfs-20230407/docs/sources/developer/Helpers.md
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3991 2022-12-29 15:59:12.000000 dfvfs-20230407/docs/sources/developer/Internals.md
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      447 2022-12-29 15:59:12.000000 dfvfs-20230407/docs/sources/developer/Testing.md
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      398 2022-12-23 11:39:27.000000 dfvfs-20230407/docs/sources/developer/index.rst
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-07 07:38:18.427766 dfvfs-20230407/docs/sources/user/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1597 2022-12-29 15:59:12.000000 dfvfs-20230407/docs/sources/user/Installation-instructions.md
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      282 2022-11-21 19:15:01.000000 dfvfs-20230407/docs/sources/user/index.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      756 2023-01-14 16:01:33.000000 dfvfs-20230407/requirements.txt
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     1018 2022-12-29 15:59:12.000000 dfvfs-20230407/run_tests.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1314 2023-04-07 07:38:18.520766 dfvfs-20230407/setup.cfg
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6873 2022-12-29 16:06:04.000000 dfvfs-20230407/setup.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2022-12-29 15:59:13.000000 dfvfs-20230407/test_dependencies.ini
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2022-12-29 16:06:04.000000 dfvfs-20230407/test_requirements.txt
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-07 07:38:18.440766 dfvfs-20230407/tests/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:14:19.000000 dfvfs-20230407/tests/__init__.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-07 07:38:18.441766 dfvfs-20230407/tests/analyzer/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:14:28.000000 dfvfs-20230407/tests/analyzer/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18459 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/analyzer/analyzer.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      912 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/analyzer/specification.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-07 07:38:18.442766 dfvfs-20230407/tests/compression/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:14:19.000000 dfvfs-20230407/tests/compression/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1231 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/compression/bzip2_decompressor.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2083 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/compression/manager.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      224 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/compression/test_lib.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2425 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/compression/xz_decompressor.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1646 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/compression/zlib_decompressor.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-07 07:38:18.443766 dfvfs-20230407/tests/credentials/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:14:36.000000 dfvfs-20230407/tests/credentials/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      543 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/credentials/apfs_credentials.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      555 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/credentials/bde_credentials.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      475 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/credentials/credentials.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      521 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/credentials/cs_credentials.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      562 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/credentials/encrypted_stream_credentials.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1344 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/credentials/keychain.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      545 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/credentials/luksde_credentials.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2146 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/credentials/manager.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-07 07:38:18.444766 dfvfs-20230407/tests/encoding/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:14:28.000000 dfvfs-20230407/tests/encoding/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      804 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/encoding/base16_decoder.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      804 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/encoding/base32_decoder.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      801 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/encoding/base64_decoder.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/encoding/manager.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      214 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/encoding/test_lib.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-07 07:38:18.457766 dfvfs-20230407/tests/encryption/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:14:32.000000 dfvfs-20230407/tests/encryption/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3435 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/encryption/aes_decrypter.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3643 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/encryption/blowfish_decrypter.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2226 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/encryption/decrypter.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3442 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/encryption/des3_decrypter.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2302 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/encryption/manager.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1136 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/encryption/rc4_decrypter.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      218 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/encryption/test_lib.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-07 07:38:18.462766 dfvfs-20230407/tests/file_io/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:14:34.000000 dfvfs-20230407/tests/file_io/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4656 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/file_io/apfs_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6036 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/file_io/bde_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9395 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/file_io/compressed_stream_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6471 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/file_io/cpio_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9118 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/file_io/cs_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2793 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/file_io/data_range_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6975 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/file_io/encoded_stream_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14381 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/file_io/encrypted_stream_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3128 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/file_io/ewf_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4396 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/file_io/ext_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3463 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/file_io/fake_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3104 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/file_io/fat_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1552 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/file_io/gpt_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4168 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/file_io/gzip_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3512 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/file_io/hfs_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3659 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/file_io/luksde_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6235 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/file_io/lvm_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5726 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/file_io/modi_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3082 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/file_io/ntfs_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5213 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/file_io/os_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3042 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/file_io/phdi_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/file_io/qcow_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2868 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/file_io/raw_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3603 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/file_io/sqlite_blob_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1843 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/file_io/tar_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33122 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/file_io/test_lib.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12616 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/file_io/tsk_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1126 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/file_io/tsk_partition_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16839 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/file_io/vhdi_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1721 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/file_io/vmdk_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5037 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/file_io/vshadow_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4369 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/file_io/xfs_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1895 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/file_io/zip_file_io.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-07 07:38:18.464766 dfvfs-20230407/tests/helpers/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:14:25.000000 dfvfs-20230407/tests/helpers/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39320 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/helpers/command_line.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2714 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/helpers/data_slice.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2644 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/helpers/fake_file_system_builder.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26712 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/helpers/file_system_searcher.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35980 2023-04-07 04:40:26.000000 dfvfs-20230407/tests/helpers/source_scanner.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8964 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/helpers/text_file.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    38545 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/helpers/volume_scanner.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6744 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/helpers/windows_path_resolver.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-07 07:38:18.465766 dfvfs-20230407/tests/lib/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:14:27.000000 dfvfs-20230407/tests/lib/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5054 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/lib/apfs_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9118 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/lib/cpio.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1756 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/lib/cs_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16350 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/lib/ewf_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1923 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/lib/glob2regex.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5410 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/lib/gzipfile.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1806 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/lib/lvm_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20600 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/lib/raw_helper.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-07 07:38:18.465766 dfvfs-20230407/tests/mount/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:14:20.000000 dfvfs-20230407/tests/mount/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3950 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/mount/manager.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-07 07:38:18.470766 dfvfs-20230407/tests/path/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:14:26.000000 dfvfs-20230407/tests/path/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2784 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/path/apfs_container_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2372 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/path/apfs_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1090 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/path/bde_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1601 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/path/compressed_stream_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1335 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/path/cpio_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2429 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/path/cs_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1752 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/path/data_range_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1538 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/path/encoded_stream_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2324 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/path/encryption_stream_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1102 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/path/ewf_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2310 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/path/ext_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1580 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/path/factory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1331 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/path/fake_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2345 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/path/fat_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2457 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/path/gpt_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1113 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/path/gzip_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2843 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/path/hfs_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/path/luksde_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2463 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/path/lvm_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/path/modi_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      945 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/path/mount_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3362 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/path/ntfs_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1990 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/path/os_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2585 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/path/path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1115 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/path/phdi_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1115 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/path/qcow_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1130 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/path/raw_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2920 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/path/sqlite_blob_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1320 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/path/tar_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      778 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/path/test_lib.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3228 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/path/tsk_partition_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/path/tsk_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1141 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/path/vhdi_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1115 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/path/vmdk_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2561 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/path/vshadow_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2310 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/path/xfs_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1320 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/path/zip_path_spec.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-07 07:38:18.470766 dfvfs-20230407/tests/resolver/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5408 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/resolver/context.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-07 07:38:18.480766 dfvfs-20230407/tests/resolver_helpers/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:14:30.000000 dfvfs-20230407/tests/resolver_helpers/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1914 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/resolver_helpers/apfs_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/resolver_helpers/bde_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1682 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/resolver_helpers/compressed_stream_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1587 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/resolver_helpers/cpio_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1846 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/resolver_helpers/cs_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1641 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/resolver_helpers/encoded_stream_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1665 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/resolver_helpers/encrypted_stream_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/resolver_helpers/ewf_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1697 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/resolver_helpers/ext_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1698 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/resolver_helpers/fat_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/resolver_helpers/gpt_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1413 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/resolver_helpers/gzip_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1700 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/resolver_helpers/hfs_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1429 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/resolver_helpers/luksde_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/resolver_helpers/lvm_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1194 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/resolver_helpers/manager.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1463 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/resolver_helpers/modi_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1714 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/resolver_helpers/ntfs_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1378 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/resolver_helpers/os_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1466 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/resolver_helpers/phdi_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1443 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/resolver_helpers/qcow_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/resolver_helpers/raw_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1617 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/resolver_helpers/sqlite_blob_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1413 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/resolver_helpers/tar_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2525 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/resolver_helpers/test_lib.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1882 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/resolver_helpers/tsk_partition_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1721 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/resolver_helpers/tsk_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1467 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/resolver_helpers/vhdi_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1442 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/resolver_helpers/vmdk_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1748 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/resolver_helpers/vshadow_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/resolver_helpers/xfs_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/resolver_helpers/zip_resolver_helper.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-07 07:38:18.480766 dfvfs-20230407/tests/serializer/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:14:28.000000 dfvfs-20230407/tests/serializer/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1978 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/serializer/json_serializer.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1996 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/test_lib.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-07 07:38:18.493766 dfvfs-20230407/tests/vfs/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:14:21.000000 dfvfs-20230407/tests/vfs/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2458 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/vfs/apfs_attribute.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/vfs/apfs_container_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16546 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/vfs/apfs_container_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5723 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/vfs/apfs_container_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2328 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/vfs/apfs_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28404 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/vfs/apfs_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4316 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/vfs/apfs_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      545 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/vfs/attribute.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6755 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/vfs/bde_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2491 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/vfs/bde_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4742 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/vfs/compressed_stream_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2830 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/vfs/compressed_stream_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1790 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/vfs/cpio_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8419 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/vfs/cpio_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3366 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/vfs/cpio_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8349 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/vfs/cs_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6279 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/vfs/cs_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4606 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/vfs/data_range_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2658 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/vfs/data_range_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      883 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/vfs/data_stream.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1379 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/vfs/directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3796 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/vfs/encoded_stream_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2771 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/vfs/encoded_stream_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4144 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/vfs/encrypted_stream_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2979 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/vfs/encrypted_stream_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2226 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/vfs/ext_attribute.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2113 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/vfs/ext_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23810 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/vfs/ext_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3983 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/vfs/ext_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      438 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/vfs/extent.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2323 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/vfs/fake_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10644 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/vfs/fake_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2904 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/vfs/fake_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/vfs/fat_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13064 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/vfs/fat_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4069 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/vfs/fat_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11194 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/vfs/file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2749 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/vfs/file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1880 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/vfs/gpt_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7790 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/vfs/gpt_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6050 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/vfs/gpt_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4674 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/vfs/gzip_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2511 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/vfs/gzip_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2239 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/vfs/hfs_attribute.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4024 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/vfs/hfs_data_stream.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2116 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/vfs/hfs_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17357 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/vfs/hfs_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4062 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/vfs/hfs_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4814 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/vfs/luksde_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2549 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/vfs/luksde_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1880 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/vfs/lvm_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8162 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/vfs/lvm_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6462 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/vfs/lvm_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9765 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/vfs/ntfs_attibute.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4168 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/vfs/ntfs_data_stream.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2139 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/vfs/ntfs_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27468 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/vfs/ntfs_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4115 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/vfs/ntfs_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/vfs/os_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9917 2023-01-01 18:32:24.000000 dfvfs-20230407/tests/vfs/os_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6171 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/vfs/os_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2628 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/vfs/sqlite_blob_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5588 2022-12-29 15:59:14.000000 dfvfs-20230407/tests/vfs/sqlite_blob_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3493 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/vfs/sqlite_blob_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1766 2022-12-29 15:59:15.000000 dfvfs-20230407/tests/vfs/tar_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8767 2022-12-29 15:59:15.000000 dfvfs-20230407/tests/vfs/tar_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5544 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/vfs/tar_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4017 2022-12-29 15:59:15.000000 dfvfs-20230407/tests/vfs/tsk_attribute.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11512 2022-12-29 15:59:15.000000 dfvfs-20230407/tests/vfs/tsk_data_stream.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1893 2022-12-29 15:59:15.000000 dfvfs-20230407/tests/vfs/tsk_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    79436 2022-12-29 15:59:15.000000 dfvfs-20230407/tests/vfs/tsk_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3941 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/vfs/tsk_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1904 2022-12-29 15:59:15.000000 dfvfs-20230407/tests/vfs/tsk_partition_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14462 2022-12-29 15:59:15.000000 dfvfs-20230407/tests/vfs/tsk_partition_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6657 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/vfs/tsk_partition_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1963 2022-12-29 15:59:15.000000 dfvfs-20230407/tests/vfs/vshadow_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8488 2022-12-29 15:59:15.000000 dfvfs-20230407/tests/vfs/vshadow_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6413 2022-12-29 15:59:15.000000 dfvfs-20230407/tests/vfs/vshadow_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2228 2022-12-29 15:59:15.000000 dfvfs-20230407/tests/vfs/xfs_attribute.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2112 2022-12-29 15:59:15.000000 dfvfs-20230407/tests/vfs/xfs_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13190 2022-12-29 15:59:15.000000 dfvfs-20230407/tests/vfs/xfs_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3985 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/vfs/xfs_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1763 2022-12-29 15:59:15.000000 dfvfs-20230407/tests/vfs/zip_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13454 2022-12-29 15:59:15.000000 dfvfs-20230407/tests/vfs/zip_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5641 2022-12-23 11:39:29.000000 dfvfs-20230407/tests/vfs/zip_file_system.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-07 07:38:18.494766 dfvfs-20230407/tests/volume/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:14:18.000000 dfvfs-20230407/tests/volume/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2698 2022-12-29 15:59:15.000000 dfvfs-20230407/tests/volume/apfs_volume_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2088 2022-12-29 15:59:15.000000 dfvfs-20230407/tests/volume/cs_volume_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1474 2022-12-29 15:59:15.000000 dfvfs-20230407/tests/volume/factory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3010 2022-12-29 15:59:15.000000 dfvfs-20230407/tests/volume/gpt_volume_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3695 2022-12-29 15:59:15.000000 dfvfs-20230407/tests/volume/lvm_volume_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8084 2022-12-29 15:59:15.000000 dfvfs-20230407/tests/volume/tsk_volume_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3543 2022-12-29 15:59:15.000000 dfvfs-20230407/tests/volume/vshadow_volume_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1451 2022-12-29 16:06:05.000000 dfvfs-20230407/tox.ini
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-07 07:38:18.505766 dfvfs-20230407/utils/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:17:55.000000 dfvfs-20230407/utils/__init__.py
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      422 2022-12-29 16:06:05.000000 dfvfs-20230407/utils/check_dependencies.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11583 2022-12-29 16:06:05.000000 dfvfs-20230407/utils/dependencies.py
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    14019 2022-12-29 15:59:15.000000 dfvfs-20230407/utils/generate_test_data_linux.sh
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4836 2022-12-29 15:59:15.000000 dfvfs-20230407/utils/generate_test_data_macos.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14212 2022-12-29 15:59:15.000000 dfvfs-20230407/utils/generate_test_data_windows.bat
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      815 2022-11-21 19:17:55.000000 dfvfs-20230407/utils/update_release.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.953698 dfvfs-20230408/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.457697 dfvfs-20230408/.github/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.541697 dfvfs-20230408/.github/workflows/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3491 2023-04-09 13:23:51.000000 dfvfs-20230408/.github/workflows/test_docker.yml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1857 2023-04-08 04:43:15.000000 dfvfs-20230408/.github/workflows/test_docs.yml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2158 2023-04-08 04:43:15.000000 dfvfs-20230408/.github/workflows/test_tox.yml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22087 2023-04-08 04:43:15.000000 dfvfs-20230408/.pylintrc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      149 2022-12-29 15:59:10.000000 dfvfs-20230408/.yamllint.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1173 2022-11-21 19:14:36.000000 dfvfs-20230408/ACKNOWLEDGEMENTS
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      360 2022-11-21 19:18:17.000000 dfvfs-20230408/AUTHORS
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11358 2022-11-21 19:18:17.000000 dfvfs-20230408/LICENSE
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      632 2022-12-29 15:59:10.000000 dfvfs-20230408/MANIFEST.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      552 2022-12-29 15:59:10.000000 dfvfs-20230408/MANIFEST.test_data.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      900 2023-04-09 13:43:04.953698 dfvfs-20230408/PKG-INFO
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      473 2022-11-21 19:14:36.000000 dfvfs-20230408/README
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1794 2023-04-09 13:23:51.000000 dfvfs-20230408/appveyor.yml
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.458697 dfvfs-20230408/config/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.541697 dfvfs-20230408/config/appveyor/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1008 2023-04-08 04:43:15.000000 dfvfs-20230408/config/appveyor/install.ps1
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      125 2023-04-08 04:43:15.000000 dfvfs-20230408/config/appveyor/install.sh
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      620 2023-04-08 04:43:15.000000 dfvfs-20230408/config/appveyor/runtests.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.542697 dfvfs-20230408/config/dpkg/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      168 2023-04-09 13:23:51.000000 dfvfs-20230408/config/dpkg/changelog
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       32 2022-11-21 19:18:17.000000 dfvfs-20230408/config/dpkg/clean
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        2 2023-04-08 04:43:15.000000 dfvfs-20230408/config/dpkg/compat
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2023-04-08 04:43:15.000000 dfvfs-20230408/config/dpkg/control
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      948 2022-11-21 19:18:17.000000 dfvfs-20230408/config/dpkg/copyright
+-rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      122 2023-04-08 04:43:15.000000 dfvfs-20230408/config/dpkg/rules
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.542697 dfvfs-20230408/config/dpkg/source/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       12 2022-11-21 19:18:17.000000 dfvfs-20230408/config/dpkg/source/format
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.543697 dfvfs-20230408/config/pylint/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1673 2022-11-21 19:18:17.000000 dfvfs-20230408/config/pylint/spelling-private-dict
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4978 2023-01-14 16:01:33.000000 dfvfs-20230408/dependencies.ini
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.543697 dfvfs-20230408/dfvfs/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      278 2023-04-09 13:23:51.000000 dfvfs-20230408/dfvfs/__init__.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.566697 dfvfs-20230408/dfvfs/analyzer/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2022-12-29 15:59:10.000000 dfvfs-20230408/dfvfs/analyzer/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13902 2022-12-29 15:59:10.000000 dfvfs-20230408/dfvfs/analyzer/analyzer.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2083 2022-12-29 15:59:10.000000 dfvfs-20230408/dfvfs/analyzer/analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      962 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/analyzer/apfs_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1010 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/analyzer/apfs_container_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1120 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/analyzer/bde_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1087 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/analyzer/bzip2_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1404 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/analyzer/cpio_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      978 2022-12-29 15:59:10.000000 dfvfs-20230408/dfvfs/analyzer/cs_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1182 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/analyzer/ewf_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1182 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/analyzer/ext_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1547 2022-12-29 15:59:10.000000 dfvfs-20230408/dfvfs/analyzer/fat_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1395 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/analyzer/gpt_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      964 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/analyzer/gzip_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1370 2022-12-29 15:59:10.000000 dfvfs-20230408/dfvfs/analyzer/hfs_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      971 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/analyzer/luksde_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1174 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/analyzer/lvm_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1168 2022-12-29 15:59:10.000000 dfvfs-20230408/dfvfs/analyzer/modi_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1186 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/analyzer/ntfs_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1003 2022-12-29 15:59:10.000000 dfvfs-20230408/dfvfs/analyzer/phdi_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1246 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/analyzer/qcow_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4938 2022-12-29 15:59:10.000000 dfvfs-20230408/dfvfs/analyzer/specification.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1057 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/analyzer/tar_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2266 2022-12-29 15:59:10.000000 dfvfs-20230408/dfvfs/analyzer/tsk_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1040 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/analyzer/tsk_partition_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1192 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/analyzer/vhdi_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1194 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/analyzer/vmdk_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1071 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/analyzer/vshadow_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      955 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/analyzer/xfs_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      968 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/analyzer/xz_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      950 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/analyzer/zip_analyzer_helper.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.568697 dfvfs-20230408/dfvfs/compression/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      247 2022-11-21 19:17:56.000000 dfvfs-20230408/dfvfs/compression/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1355 2022-12-29 15:59:10.000000 dfvfs-20230408/dfvfs/compression/bzip2_decompressor.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      437 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/compression/decompressor.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2286 2022-12-29 15:59:10.000000 dfvfs-20230408/dfvfs/compression/manager.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2139 2022-12-29 15:59:10.000000 dfvfs-20230408/dfvfs/compression/xz_decompressor.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2118 2022-12-29 15:59:10.000000 dfvfs-20230408/dfvfs/compression/zlib_decompressor.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.570697 dfvfs-20230408/dfvfs/credentials/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      313 2022-12-29 15:59:10.000000 dfvfs-20230408/dfvfs/credentials/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      545 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/credentials/apfs_credentials.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      646 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/credentials/bde_credentials.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      562 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/credentials/credentials.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      544 2022-12-29 15:59:10.000000 dfvfs-20230408/dfvfs/credentials/cs_credentials.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      497 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/credentials/encrypted_stream_credentials.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2696 2022-12-29 15:59:10.000000 dfvfs-20230408/dfvfs/credentials/keychain.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      498 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/credentials/luksde_credentials.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1902 2022-12-29 15:59:10.000000 dfvfs-20230408/dfvfs/credentials/manager.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.572697 dfvfs-20230408/dfvfs/encoding/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      191 2022-11-21 19:18:12.000000 dfvfs-20230408/dfvfs/encoding/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      967 2022-12-29 15:59:10.000000 dfvfs-20230408/dfvfs/encoding/base16_decoder.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      967 2022-12-29 15:59:10.000000 dfvfs-20230408/dfvfs/encoding/base32_decoder.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1198 2022-12-29 15:59:10.000000 dfvfs-20230408/dfvfs/encoding/base64_decoder.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      392 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/encoding/decoder.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1955 2022-12-29 15:59:10.000000 dfvfs-20230408/dfvfs/encoding/manager.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.574697 dfvfs-20230408/dfvfs/encryption/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      245 2022-11-25 17:21:27.000000 dfvfs-20230408/dfvfs/encryption/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1478 2022-12-29 15:59:10.000000 dfvfs-20230408/dfvfs/encryption/aes_decrypter.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1513 2022-12-29 15:59:10.000000 dfvfs-20230408/dfvfs/encryption/blowfish_decrypter.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3897 2022-12-29 15:59:10.000000 dfvfs-20230408/dfvfs/encryption/decrypter.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1502 2022-12-29 15:59:10.000000 dfvfs-20230408/dfvfs/encryption/des3_decrypter.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2274 2022-12-29 15:59:10.000000 dfvfs-20230408/dfvfs/encryption/manager.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1771 2022-12-29 15:59:10.000000 dfvfs-20230408/dfvfs/encryption/rc4_decrypter.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.585697 dfvfs-20230408/dfvfs/file_io/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-12-29 15:59:10.000000 dfvfs-20230408/dfvfs/file_io/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3960 2022-12-29 15:59:10.000000 dfvfs-20230408/dfvfs/file_io/apfs_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/file_io/bde_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9503 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/file_io/compressed_stream_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4645 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/file_io/cpio_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4663 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/file_io/cs_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5995 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/file_io/data_range_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9664 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/file_io/encoded_stream_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10632 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/file_io/encrypted_stream_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2710 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/file_io/ewf_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3948 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/file_io/ext_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/file_io/fake_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4398 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/file_io/fat_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4882 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/file_io/file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4157 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/file_io/file_object_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5577 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/file_io/gpt_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2401 2023-01-14 16:01:33.000000 dfvfs-20230408/dfvfs/file_io/gzip_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4501 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/file_io/hfs_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1272 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/file_io/luksde_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3978 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/file_io/lvm_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1856 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/file_io/modi_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4540 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/file_io/ntfs_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6180 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/file_io/os_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4378 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/file_io/phdi_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4074 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/file_io/qcow_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2733 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/file_io/raw_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8349 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/file_io/sqlite_blob_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4775 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/file_io/tar_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7991 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/file_io/tsk_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2370 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/file_io/tsk_partition_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4313 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/file_io/vhdi_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4201 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/file_io/vmdk_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4106 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/file_io/vshadow_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3941 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/file_io/xfs_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9026 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/file_io/zip_file_io.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.587697 dfvfs-20230408/dfvfs/helpers/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/helpers/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29824 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/helpers/command_line.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2093 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/helpers/data_slice.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3992 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/helpers/fake_file_system_builder.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22280 2023-04-07 07:26:35.000000 dfvfs-20230408/dfvfs/helpers/file_system_searcher.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30704 2023-04-07 04:40:26.000000 dfvfs-20230408/dfvfs/helpers/source_scanner.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6081 2022-12-23 11:41:15.000000 dfvfs-20230408/dfvfs/helpers/text_file.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28568 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/helpers/volume_scanner.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9518 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/helpers/windows_path_resolver.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.593697 dfvfs-20230408/dfvfs/lib/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/lib/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1687 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/lib/apfs_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1710 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/lib/bde_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10516 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/lib/cpio.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4230 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/lib/cpio.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1677 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/lib/cs_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3532 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/lib/data_format.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      710 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/lib/decorators.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4694 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/lib/definitions.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1053 2022-11-21 19:18:10.000000 dfvfs-20230408/dfvfs/lib/errors.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3502 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/lib/ewf_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2345 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/lib/glob2regex.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      723 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/lib/gpt_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19596 2023-01-14 16:01:33.000000 dfvfs-20230408/dfvfs/lib/gzipfile.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1489 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/lib/gzipfile.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1160 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/lib/luksde_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      866 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/lib/lvm_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12570 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/lib/raw_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5970 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/lib/sqlite_database.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1775 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/lib/tsk_image.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4930 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/lib/tsk_partition.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      745 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/lib/vshadow_helper.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.593697 dfvfs-20230408/dfvfs/mount/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/mount/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2036 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/mount/manager.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.602697 dfvfs-20230408/dfvfs/path/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1413 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/path/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1564 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/path/apfs_container_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1547 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/path/apfs_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1769 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/path/bde_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1387 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/path/compressed_stream_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      965 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/path/cpio_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2397 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/path/cs_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1517 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/path/data_range_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1332 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/path/encoded_stream_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2414 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/path/encrypted_stream_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      777 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/path/ewf_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1475 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/path/ext_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3742 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/path/factory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      940 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/path/fake_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1560 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/path/fat_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1474 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/path/gpt_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      782 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/path/gzip_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1932 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/path/hfs_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      923 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/path/location_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1217 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/path/luksde_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1482 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/path/lvm_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      798 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/path/modi_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1102 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/path/mount_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2364 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/path/ntfs_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/path/os_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4043 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/path/path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      784 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/path/phdi_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      779 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/path/qcow_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      800 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/path/raw_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2964 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/path/sqlite_blob_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      947 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/path/tar_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1777 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/path/tsk_partition_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1943 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/path/tsk_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      810 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/path/vhdi_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      784 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/path/vmdk_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1499 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/path/vshadow_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1475 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/path/xfs_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      978 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/path/zip_path_spec.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.602697 dfvfs-20230408/dfvfs/resolver/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:17:56.000000 dfvfs-20230408/dfvfs/resolver/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4365 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/resolver/context.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6142 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/resolver/resolver.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.609697 dfvfs-20230408/dfvfs/resolver_helpers/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2723 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/resolver_helpers/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      904 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/resolver_helpers/apfs_container_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1195 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/resolver_helpers/apfs_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1195 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/resolver_helpers/bde_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1329 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/resolver_helpers/compressed_stream_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1246 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/resolver_helpers/cpio_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1198 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/resolver_helpers/cs_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1252 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/resolver_helpers/data_range_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1296 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/resolver_helpers/encoded_stream_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1318 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/resolver_helpers/encrypted_stream_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      824 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/resolver_helpers/ewf_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1184 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/resolver_helpers/ext_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      522 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/resolver_helpers/fake_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1184 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/resolver_helpers/fat_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1207 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/resolver_helpers/gpt_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1205 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/resolver_helpers/gzip_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1184 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/resolver_helpers/hfs_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/resolver_helpers/luksde_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1209 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/resolver_helpers/lvm_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1928 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/resolver_helpers/manager.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      846 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/resolver_helpers/modi_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1195 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/resolver_helpers/ntfs_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1201 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/resolver_helpers/os_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      832 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/resolver_helpers/phdi_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      832 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/resolver_helpers/qcow_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      838 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/resolver_helpers/raw_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/resolver_helpers/resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1300 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/resolver_helpers/sqlite_blob_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1184 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/resolver_helpers/tar_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1312 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/resolver_helpers/tsk_partition_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1208 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/resolver_helpers/tsk_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      830 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/resolver_helpers/vhdi_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      832 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/resolver_helpers/vmdk_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1246 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/resolver_helpers/vshadow_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1184 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/resolver_helpers/xfs_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1184 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/resolver_helpers/zip_resolver_helper.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.610697 dfvfs-20230408/dfvfs/serializer/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:18:12.000000 dfvfs-20230408/dfvfs/serializer/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5458 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/serializer/json_serializer.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/serializer/serializer.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.626697 dfvfs-20230408/dfvfs/vfs/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:17:59.000000 dfvfs-20230408/dfvfs/vfs/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3622 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/apfs_attribute.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/apfs_container_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4534 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/apfs_container_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4513 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/apfs_container_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/apfs_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8895 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/apfs_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6044 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/apfs_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2064 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/attribute.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2188 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/bde_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2758 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/bde_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1637 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/compressed_stream_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2621 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/vfs/compressed_stream_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/cpio_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7019 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/cpio_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4635 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/cpio_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1112 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/cs_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4353 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/cs_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5012 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/cs_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1335 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/vfs/data_range_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2781 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/vfs/data_range_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      859 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/data_stream.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      961 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/encoded_stream_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2534 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/vfs/encoded_stream_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/encrypted_stream_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2699 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/vfs/encrypted_stream_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3601 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/ext_attribute.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1434 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/ext_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9823 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/ext_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5159 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/vfs/ext_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      844 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/extent.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1212 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/fake_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4684 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/fake_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5004 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/fake_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1437 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/fat_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7675 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/fat_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5634 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/fat_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11742 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7136 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1085 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/gpt_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3578 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/gpt_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4352 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/gpt_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1849 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/vfs/gzip_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1019 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/vfs/gzip_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3601 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/hfs_attribute.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1378 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/hfs_data_stream.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1437 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/hfs_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10348 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/hfs_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5316 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/hfs_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1944 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/luksde_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2856 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/luksde_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/lvm_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3835 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/lvm_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4750 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/lvm_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5041 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/ntfs_attribute.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1411 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/ntfs_data_stream.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1838 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/ntfs_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12181 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/ntfs_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5882 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/vfs/ntfs_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3067 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/os_attribute.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1662 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/os_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9286 2023-01-01 18:32:24.000000 dfvfs-20230408/dfvfs/vfs/os_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6345 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/os_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      665 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/vfs/root_only_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1699 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/root_only_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1853 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/sqlite_blob_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4202 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/sqlite_blob_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3520 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/vfs/sqlite_blob_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2093 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/tar_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6442 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/tar_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5180 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/tar_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4281 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/tsk_attribute.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3018 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/tsk_data_stream.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4156 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/tsk_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27588 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/tsk_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7175 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/tsk_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1865 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/tsk_partition_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4278 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/tsk_partition_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4196 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/tsk_partition_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1128 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/vshadow_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4224 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/vshadow_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4412 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/vshadow_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3601 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/xfs_attribute.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1434 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/xfs_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8567 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/xfs_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5313 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/vfs/xfs_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2261 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/zip_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6332 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/zip_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4975 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/zip_file_system.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.628697 dfvfs-20230408/dfvfs/volume/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      332 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/volume/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/volume/apfs_volume_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1513 2022-12-29 15:59:12.000000 dfvfs-20230408/dfvfs/volume/cs_volume_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1710 2022-12-29 15:59:12.000000 dfvfs-20230408/dfvfs/volume/factory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1427 2022-12-29 15:59:12.000000 dfvfs-20230408/dfvfs/volume/gpt_volume_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1539 2022-12-29 15:59:12.000000 dfvfs-20230408/dfvfs/volume/lvm_volume_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3054 2022-12-29 15:59:12.000000 dfvfs-20230408/dfvfs/volume/tsk_volume_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7299 2022-12-29 15:59:12.000000 dfvfs-20230408/dfvfs/volume/volume_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2017 2022-12-29 15:59:12.000000 dfvfs-20230408/dfvfs/volume/vshadow_volume_system.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.556697 dfvfs-20230408/dfvfs.egg-info/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      900 2023-04-09 13:43:01.000000 dfvfs-20230408/dfvfs.egg-info/PKG-INFO
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    20370 2023-04-09 13:43:04.000000 dfvfs-20230408/dfvfs.egg-info/SOURCES.txt
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        1 2023-04-09 13:43:01.000000 dfvfs-20230408/dfvfs.egg-info/dependency_links.txt
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        1 2022-11-21 19:14:18.000000 dfvfs-20230408/dfvfs.egg-info/not-zip-safe
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      729 2023-04-09 13:43:02.000000 dfvfs-20230408/dfvfs.egg-info/requires.txt
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        6 2023-04-09 13:43:02.000000 dfvfs-20230408/dfvfs.egg-info/top_level.txt
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1017 2022-12-29 15:59:10.000000 dfvfs-20230408/dfvfs.ini
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.649697 dfvfs-20230408/docs/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5037 2023-04-08 04:43:15.000000 dfvfs-20230408/docs/conf.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2022-12-29 15:59:12.000000 dfvfs-20230408/docs/index.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      105 2023-04-08 04:43:23.000000 dfvfs-20230408/docs/requirements.txt
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.658697 dfvfs-20230408/docs/sources/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3182 2022-12-29 15:59:12.000000 dfvfs-20230408/docs/sources/Code-snippets.md
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14179 2022-12-29 15:59:12.000000 dfvfs-20230408/docs/sources/Path-specifications.md
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3922 2022-12-29 15:59:12.000000 dfvfs-20230408/docs/sources/Supported-formats.md
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.709698 dfvfs-20230408/docs/sources/api/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6080 2022-12-29 15:59:12.000000 dfvfs-20230408/docs/sources/api/dfvfs.analyzer.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1125 2022-12-23 11:39:27.000000 dfvfs-20230408/docs/sources/api/dfvfs.compression.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1704 2022-12-29 15:59:12.000000 dfvfs-20230408/docs/sources/api/dfvfs.credentials.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1032 2022-12-23 11:39:27.000000 dfvfs-20230408/docs/sources/api/dfvfs.encoding.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1264 2022-12-23 11:39:27.000000 dfvfs-20230408/docs/sources/api/dfvfs.encryption.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6140 2022-12-29 15:59:12.000000 dfvfs-20230408/docs/sources/api/dfvfs.file_io.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1629 2022-12-23 11:39:27.000000 dfvfs-20230408/docs/sources/api/dfvfs.helpers.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3042 2022-12-29 15:59:12.000000 dfvfs-20230408/docs/sources/api/dfvfs.lib.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      325 2022-12-23 11:39:27.000000 dfvfs-20230408/docs/sources/api/dfvfs.mount.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6547 2022-12-29 15:59:12.000000 dfvfs-20230408/docs/sources/api/dfvfs.path.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      501 2022-12-29 15:59:12.000000 dfvfs-20230408/docs/sources/api/dfvfs.resolver.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8176 2022-12-29 15:59:12.000000 dfvfs-20230408/docs/sources/api/dfvfs.resolver_helpers.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      461 2022-11-21 19:15:00.000000 dfvfs-20230408/docs/sources/api/dfvfs.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      551 2022-12-23 11:39:27.000000 dfvfs-20230408/docs/sources/api/dfvfs.serializer.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15405 2022-12-29 15:59:12.000000 dfvfs-20230408/docs/sources/api/dfvfs.vfs.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2022-12-29 15:59:12.000000 dfvfs-20230408/docs/sources/api/dfvfs.volume.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       52 2022-11-21 19:15:00.000000 dfvfs-20230408/docs/sources/api/modules.rst
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.727697 dfvfs-20230408/docs/sources/developer/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6837 2022-12-23 11:39:27.000000 dfvfs-20230408/docs/sources/developer/Adding-new-type.md
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5996 2022-12-23 11:39:27.000000 dfvfs-20230408/docs/sources/developer/Helpers.md
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3991 2022-12-29 15:59:12.000000 dfvfs-20230408/docs/sources/developer/Internals.md
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      447 2022-12-29 15:59:12.000000 dfvfs-20230408/docs/sources/developer/Testing.md
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      398 2022-12-23 11:39:27.000000 dfvfs-20230408/docs/sources/developer/index.rst
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.728697 dfvfs-20230408/docs/sources/user/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1597 2022-12-29 15:59:12.000000 dfvfs-20230408/docs/sources/user/Installation-instructions.md
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      282 2022-11-21 19:15:01.000000 dfvfs-20230408/docs/sources/user/index.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      787 2023-04-09 13:23:51.000000 dfvfs-20230408/requirements.txt
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     1018 2022-12-29 15:59:12.000000 dfvfs-20230408/run_tests.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1314 2023-04-09 13:43:04.954698 dfvfs-20230408/setup.cfg
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6873 2023-04-08 04:43:15.000000 dfvfs-20230408/setup.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2022-12-29 15:59:13.000000 dfvfs-20230408/test_dependencies.ini
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-08 04:43:15.000000 dfvfs-20230408/test_requirements.txt
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.729698 dfvfs-20230408/tests/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:14:19.000000 dfvfs-20230408/tests/__init__.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.729698 dfvfs-20230408/tests/analyzer/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:14:28.000000 dfvfs-20230408/tests/analyzer/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18459 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/analyzer/analyzer.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      912 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/analyzer/specification.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.730697 dfvfs-20230408/tests/compression/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:14:19.000000 dfvfs-20230408/tests/compression/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1231 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/compression/bzip2_decompressor.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2083 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/compression/manager.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      224 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/compression/test_lib.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2425 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/compression/xz_decompressor.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1646 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/compression/zlib_decompressor.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.731697 dfvfs-20230408/tests/credentials/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:14:36.000000 dfvfs-20230408/tests/credentials/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      543 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/credentials/apfs_credentials.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      555 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/credentials/bde_credentials.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      475 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/credentials/credentials.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      521 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/credentials/cs_credentials.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      562 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/credentials/encrypted_stream_credentials.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1344 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/credentials/keychain.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      545 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/credentials/luksde_credentials.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2146 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/credentials/manager.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.732698 dfvfs-20230408/tests/encoding/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:14:28.000000 dfvfs-20230408/tests/encoding/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      804 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/encoding/base16_decoder.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      804 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/encoding/base32_decoder.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      801 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/encoding/base64_decoder.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/encoding/manager.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      214 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/encoding/test_lib.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.733698 dfvfs-20230408/tests/encryption/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:14:32.000000 dfvfs-20230408/tests/encryption/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3435 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/encryption/aes_decrypter.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3643 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/encryption/blowfish_decrypter.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2226 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/encryption/decrypter.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3442 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/encryption/des3_decrypter.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2302 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/encryption/manager.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1136 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/encryption/rc4_decrypter.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      218 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/encryption/test_lib.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.738697 dfvfs-20230408/tests/file_io/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:14:34.000000 dfvfs-20230408/tests/file_io/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4656 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/file_io/apfs_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6036 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/file_io/bde_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9395 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/file_io/compressed_stream_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6471 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/file_io/cpio_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9118 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/file_io/cs_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2793 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/file_io/data_range_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6975 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/file_io/encoded_stream_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14381 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/file_io/encrypted_stream_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3128 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/file_io/ewf_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4396 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/file_io/ext_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3463 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/file_io/fake_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3104 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/file_io/fat_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1552 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/file_io/gpt_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4168 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/file_io/gzip_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3512 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/file_io/hfs_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3659 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/file_io/luksde_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6235 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/file_io/lvm_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5726 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/file_io/modi_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3082 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/file_io/ntfs_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5213 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/file_io/os_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3042 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/file_io/phdi_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/file_io/qcow_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2868 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/file_io/raw_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3603 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/file_io/sqlite_blob_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1843 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/file_io/tar_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33122 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/file_io/test_lib.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12616 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/file_io/tsk_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1126 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/file_io/tsk_partition_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16839 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/file_io/vhdi_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1721 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/file_io/vmdk_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5037 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/file_io/vshadow_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4369 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/file_io/xfs_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1895 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/file_io/zip_file_io.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.739698 dfvfs-20230408/tests/helpers/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:14:25.000000 dfvfs-20230408/tests/helpers/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39320 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/helpers/command_line.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2714 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/helpers/data_slice.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2644 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/helpers/fake_file_system_builder.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26712 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/helpers/file_system_searcher.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35980 2023-04-07 04:40:26.000000 dfvfs-20230408/tests/helpers/source_scanner.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8964 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/helpers/text_file.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    38545 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/helpers/volume_scanner.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6744 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/helpers/windows_path_resolver.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.740697 dfvfs-20230408/tests/lib/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:14:27.000000 dfvfs-20230408/tests/lib/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5054 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/lib/apfs_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9118 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/lib/cpio.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1756 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/lib/cs_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16350 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/lib/ewf_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1923 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/lib/glob2regex.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5410 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/lib/gzipfile.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1806 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/lib/lvm_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20600 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/lib/raw_helper.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.741697 dfvfs-20230408/tests/mount/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:14:20.000000 dfvfs-20230408/tests/mount/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3950 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/mount/manager.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.745698 dfvfs-20230408/tests/path/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:14:26.000000 dfvfs-20230408/tests/path/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2784 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/path/apfs_container_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2372 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/path/apfs_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1090 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/path/bde_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1601 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/path/compressed_stream_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1335 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/path/cpio_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2429 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/path/cs_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1752 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/path/data_range_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1538 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/path/encoded_stream_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2324 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/path/encryption_stream_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1102 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/path/ewf_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2310 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/path/ext_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1580 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/path/factory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1331 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/path/fake_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2345 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/path/fat_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2457 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/path/gpt_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1113 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/path/gzip_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2843 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/path/hfs_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/path/luksde_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2463 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/path/lvm_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/path/modi_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      945 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/path/mount_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3362 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/path/ntfs_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1990 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/path/os_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2585 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/path/path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1115 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/path/phdi_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1115 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/path/qcow_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1130 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/path/raw_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2920 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/path/sqlite_blob_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1320 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/path/tar_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      778 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/path/test_lib.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3228 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/path/tsk_partition_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/path/tsk_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1141 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/path/vhdi_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1115 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/path/vmdk_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2561 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/path/vshadow_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2310 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/path/xfs_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1320 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/path/zip_path_spec.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.745698 dfvfs-20230408/tests/resolver/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5408 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/resolver/context.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.750697 dfvfs-20230408/tests/resolver_helpers/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:14:30.000000 dfvfs-20230408/tests/resolver_helpers/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1914 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/resolver_helpers/apfs_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/resolver_helpers/bde_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1682 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/resolver_helpers/compressed_stream_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1587 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/resolver_helpers/cpio_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1846 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/resolver_helpers/cs_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1641 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/resolver_helpers/encoded_stream_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1665 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/resolver_helpers/encrypted_stream_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/resolver_helpers/ewf_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1697 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/resolver_helpers/ext_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1698 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/resolver_helpers/fat_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/resolver_helpers/gpt_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1413 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/resolver_helpers/gzip_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1700 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/resolver_helpers/hfs_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1429 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/resolver_helpers/luksde_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/resolver_helpers/lvm_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1194 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/resolver_helpers/manager.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1463 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/resolver_helpers/modi_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1714 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/resolver_helpers/ntfs_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1378 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/resolver_helpers/os_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1466 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/resolver_helpers/phdi_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1443 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/resolver_helpers/qcow_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/resolver_helpers/raw_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1617 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/resolver_helpers/sqlite_blob_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1413 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/resolver_helpers/tar_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2525 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/resolver_helpers/test_lib.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1882 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/resolver_helpers/tsk_partition_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1721 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/resolver_helpers/tsk_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1467 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/resolver_helpers/vhdi_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1442 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/resolver_helpers/vmdk_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1748 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/resolver_helpers/vshadow_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/resolver_helpers/xfs_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/resolver_helpers/zip_resolver_helper.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.750697 dfvfs-20230408/tests/serializer/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:14:28.000000 dfvfs-20230408/tests/serializer/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1978 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/serializer/json_serializer.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1996 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/test_lib.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.763697 dfvfs-20230408/tests/vfs/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:14:21.000000 dfvfs-20230408/tests/vfs/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2458 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/apfs_attribute.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/apfs_container_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16546 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/apfs_container_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5723 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/vfs/apfs_container_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2328 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/apfs_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28404 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/apfs_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4316 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/vfs/apfs_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      545 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/attribute.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6755 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/bde_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2491 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/bde_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4742 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/compressed_stream_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2830 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/vfs/compressed_stream_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1790 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/cpio_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8419 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/cpio_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3366 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/vfs/cpio_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8349 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/cs_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6279 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/cs_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4606 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/data_range_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2658 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/vfs/data_range_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      883 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/data_stream.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1379 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3796 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/encoded_stream_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2771 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/vfs/encoded_stream_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4144 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/encrypted_stream_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2979 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/vfs/encrypted_stream_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2226 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/ext_attribute.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2113 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/ext_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23810 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/ext_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3983 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/vfs/ext_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      438 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/extent.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2323 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/fake_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10644 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/fake_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2904 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/vfs/fake_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/fat_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13064 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/fat_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4069 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/fat_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11194 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2749 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/vfs/file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1880 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/gpt_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7790 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/gpt_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6050 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/vfs/gpt_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4674 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/gzip_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2511 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/vfs/gzip_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2239 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/hfs_attribute.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4024 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/hfs_data_stream.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2116 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/hfs_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17357 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/hfs_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4062 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/vfs/hfs_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4814 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/luksde_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2549 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/luksde_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1880 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/lvm_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8162 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/lvm_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6462 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/lvm_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9765 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/ntfs_attibute.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4168 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/ntfs_data_stream.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2139 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/ntfs_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27468 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/ntfs_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4115 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/ntfs_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/os_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9917 2023-01-01 18:32:24.000000 dfvfs-20230408/tests/vfs/os_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6171 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/vfs/os_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2628 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/sqlite_blob_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5588 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/sqlite_blob_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3493 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/vfs/sqlite_blob_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1766 2022-12-29 15:59:15.000000 dfvfs-20230408/tests/vfs/tar_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8767 2022-12-29 15:59:15.000000 dfvfs-20230408/tests/vfs/tar_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5544 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/vfs/tar_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4017 2022-12-29 15:59:15.000000 dfvfs-20230408/tests/vfs/tsk_attribute.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11512 2022-12-29 15:59:15.000000 dfvfs-20230408/tests/vfs/tsk_data_stream.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1893 2022-12-29 15:59:15.000000 dfvfs-20230408/tests/vfs/tsk_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    79436 2022-12-29 15:59:15.000000 dfvfs-20230408/tests/vfs/tsk_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3941 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/vfs/tsk_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1904 2022-12-29 15:59:15.000000 dfvfs-20230408/tests/vfs/tsk_partition_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14462 2022-12-29 15:59:15.000000 dfvfs-20230408/tests/vfs/tsk_partition_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6657 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/vfs/tsk_partition_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1963 2022-12-29 15:59:15.000000 dfvfs-20230408/tests/vfs/vshadow_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8488 2022-12-29 15:59:15.000000 dfvfs-20230408/tests/vfs/vshadow_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6413 2022-12-29 15:59:15.000000 dfvfs-20230408/tests/vfs/vshadow_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2228 2022-12-29 15:59:15.000000 dfvfs-20230408/tests/vfs/xfs_attribute.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2112 2022-12-29 15:59:15.000000 dfvfs-20230408/tests/vfs/xfs_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13190 2022-12-29 15:59:15.000000 dfvfs-20230408/tests/vfs/xfs_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3985 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/vfs/xfs_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1763 2022-12-29 15:59:15.000000 dfvfs-20230408/tests/vfs/zip_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13454 2022-12-29 15:59:15.000000 dfvfs-20230408/tests/vfs/zip_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5641 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/vfs/zip_file_system.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.765698 dfvfs-20230408/tests/volume/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:14:18.000000 dfvfs-20230408/tests/volume/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2698 2022-12-29 15:59:15.000000 dfvfs-20230408/tests/volume/apfs_volume_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2088 2022-12-29 15:59:15.000000 dfvfs-20230408/tests/volume/cs_volume_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1474 2022-12-29 15:59:15.000000 dfvfs-20230408/tests/volume/factory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3010 2022-12-29 15:59:15.000000 dfvfs-20230408/tests/volume/gpt_volume_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3695 2022-12-29 15:59:15.000000 dfvfs-20230408/tests/volume/lvm_volume_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8084 2022-12-29 15:59:15.000000 dfvfs-20230408/tests/volume/tsk_volume_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3543 2022-12-29 15:59:15.000000 dfvfs-20230408/tests/volume/vshadow_volume_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1451 2023-04-08 04:43:15.000000 dfvfs-20230408/tox.ini
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.938698 dfvfs-20230408/utils/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:17:55.000000 dfvfs-20230408/utils/__init__.py
+-rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      422 2023-04-08 04:43:15.000000 dfvfs-20230408/utils/check_dependencies.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11583 2023-04-08 04:43:15.000000 dfvfs-20230408/utils/dependencies.py
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    14019 2022-12-29 15:59:15.000000 dfvfs-20230408/utils/generate_test_data_linux.sh
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4836 2022-12-29 15:59:15.000000 dfvfs-20230408/utils/generate_test_data_macos.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14212 2022-12-29 15:59:15.000000 dfvfs-20230408/utils/generate_test_data_windows.bat
+-rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      815 2022-11-21 19:17:55.000000 dfvfs-20230408/utils/update_release.sh
```

### Comparing `dfvfs-20230407/.github/workflows/test_docker.yml` & `dfvfs-20230408/.github/workflows/test_docker.yml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 on: [push]
 permissions: read-all
 jobs:
   test_fedora:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        version: ['36']
+        version: ['37']
     container:
       image: registry.fedoraproject.org/fedora:${{ matrix.version }}
     steps:
     - uses: actions/checkout@v2
     - name: Set up container
       run: |
         dnf install -y dnf-plugins-core langpacks-en
```

### Comparing `dfvfs-20230407/.github/workflows/test_docs.yml` & `dfvfs-20230408/.github/workflows/test_docs.yml`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/.github/workflows/test_tox.yml` & `dfvfs-20230408/.github/workflows/test_tox.yml`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/.pylintrc` & `dfvfs-20230408/.pylintrc`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/ACKNOWLEDGEMENTS` & `dfvfs-20230408/ACKNOWLEDGEMENTS`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/LICENSE` & `dfvfs-20230408/LICENSE`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/MANIFEST.in` & `dfvfs-20230408/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/MANIFEST.test_data.in` & `dfvfs-20230408/MANIFEST.test_data.in`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/PKG-INFO` & `dfvfs-20230408/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfvfs
-Version: 20230407
+Version: 20230408
 Summary: Digital Forensics Virtual File System (dfVFS).
 Home-page: https://github.com/log2timeline/dfvfs
 Maintainer: Log2Timeline maintainers
 Maintainer-email: log2timeline-maintainers@googlegroups.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `dfvfs-20230407/appveyor.yml` & `dfvfs-20230408/appveyor.yml`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 environment:
   PYPI_TOKEN:
     secure: /FwQrmudDyj+Mu3DaxLEowyvwBaY7x1GRt6gYJrVerEAo4PujrTDfMs9/K6PJSN7KkCL/6LQK2VfTD91bbnUwGMiTjfeItu2+aernJtwLLtoDJ22sHgMiajGMqficrHlOc7uNhFMjQsGa7WiiGGo12c/b7z55dNmU2N0EIc086/Z2G6O+n2+oBeT5SbFu5j5XXkwrd98vnW8hryuZPjLauV1mxc6MMNiv3dOgVL8gtWDjW5xZVJvfOTcYA+7MMLPUbMbqMcXkTSRshqUrX/6mw==
   matrix:
-  - DESCRIPTION: "Windows with 32-bit Python 3.10"
+  - DESCRIPTION: "Windows with 32-bit Python 3.11"
     MACHINE_TYPE: "x86"
-    APPVEYOR_BUILD_WORKER_IMAGE: Visual Studio 2019
-    PYTHON: "C:\\Python310"
-    PYTHON_VERSION: "3.10"
+    APPVEYOR_BUILD_WORKER_IMAGE: Visual Studio 2022
+    PYTHON: "C:\\Python311"
+    PYTHON_VERSION: "3.11"
     L2TBINARIES_TRACK: "dev"
-  - DESCRIPTION: "Windows with 64-bit Python 3.10"
+  - DESCRIPTION: "Windows with 64-bit Python 3.11"
     MACHINE_TYPE: "amd64"
-    APPVEYOR_BUILD_WORKER_IMAGE: Visual Studio 2019
-    PYTHON: "C:\\Python310-x64"
-    PYTHON_VERSION: "3.10"
+    APPVEYOR_BUILD_WORKER_IMAGE: Visual Studio 2022
+    PYTHON: "C:\\Python311-x64"
+    PYTHON_VERSION: "3.11"
     L2TBINARIES_TRACK: "dev"
   - DESCRIPTION: "Mac OS with Python 3.11"
     APPVEYOR_BUILD_WORKER_IMAGE: macos-monterey
     HOMEBREW_NO_INSTALL_CLEANUP: 1
 
 install:
 - cmd: "%PYTHON%\\python.exe -m pip install -U pip setuptools twine wheel"
```

### Comparing `dfvfs-20230407/config/appveyor/install.ps1` & `dfvfs-20230408/config/appveyor/install.ps1`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/config/appveyor/runtests.sh` & `dfvfs-20230408/config/appveyor/runtests.sh`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/config/dpkg/control` & `dfvfs-20230408/config/dpkg/control`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/config/dpkg/copyright` & `dfvfs-20230408/config/dpkg/copyright`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/config/pylint/spelling-private-dict` & `dfvfs-20230408/config/pylint/spelling-private-dict`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dependencies.ini` & `dfvfs-20230408/dependencies.ini`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/analyzer/__init__.py` & `dfvfs-20230408/dfvfs/analyzer/__init__.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/analyzer/analyzer.py` & `dfvfs-20230408/dfvfs/analyzer/analyzer.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/analyzer/analyzer_helper.py` & `dfvfs-20230408/dfvfs/analyzer/analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/analyzer/apfs_analyzer_helper.py` & `dfvfs-20230408/dfvfs/analyzer/apfs_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/analyzer/apfs_container_analyzer_helper.py` & `dfvfs-20230408/dfvfs/analyzer/apfs_container_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/analyzer/bde_analyzer_helper.py` & `dfvfs-20230408/dfvfs/analyzer/bde_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/analyzer/bzip2_analyzer_helper.py` & `dfvfs-20230408/dfvfs/analyzer/bzip2_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/analyzer/cpio_analyzer_helper.py` & `dfvfs-20230408/dfvfs/analyzer/cpio_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/analyzer/cs_analyzer_helper.py` & `dfvfs-20230408/dfvfs/analyzer/cs_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/analyzer/ewf_analyzer_helper.py` & `dfvfs-20230408/dfvfs/analyzer/ewf_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/analyzer/ext_analyzer_helper.py` & `dfvfs-20230408/dfvfs/analyzer/ext_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/analyzer/fat_analyzer_helper.py` & `dfvfs-20230408/dfvfs/analyzer/fat_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/analyzer/gpt_analyzer_helper.py` & `dfvfs-20230408/dfvfs/analyzer/gpt_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/analyzer/gzip_analyzer_helper.py` & `dfvfs-20230408/dfvfs/analyzer/gzip_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/analyzer/hfs_analyzer_helper.py` & `dfvfs-20230408/dfvfs/analyzer/hfs_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/analyzer/luksde_analyzer_helper.py` & `dfvfs-20230408/dfvfs/analyzer/luksde_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/analyzer/lvm_analyzer_helper.py` & `dfvfs-20230408/dfvfs/analyzer/lvm_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/analyzer/modi_analyzer_helper.py` & `dfvfs-20230408/dfvfs/analyzer/modi_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/analyzer/ntfs_analyzer_helper.py` & `dfvfs-20230408/dfvfs/analyzer/ntfs_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/analyzer/phdi_analyzer_helper.py` & `dfvfs-20230408/dfvfs/analyzer/phdi_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/analyzer/qcow_analyzer_helper.py` & `dfvfs-20230408/dfvfs/analyzer/qcow_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/analyzer/specification.py` & `dfvfs-20230408/dfvfs/analyzer/specification.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/analyzer/tar_analyzer_helper.py` & `dfvfs-20230408/dfvfs/analyzer/tar_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/analyzer/tsk_analyzer_helper.py` & `dfvfs-20230408/dfvfs/analyzer/tsk_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/analyzer/tsk_partition_analyzer_helper.py` & `dfvfs-20230408/dfvfs/analyzer/tsk_partition_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/analyzer/vhdi_analyzer_helper.py` & `dfvfs-20230408/dfvfs/analyzer/vhdi_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/analyzer/vmdk_analyzer_helper.py` & `dfvfs-20230408/dfvfs/analyzer/vmdk_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/analyzer/vshadow_analyzer_helper.py` & `dfvfs-20230408/dfvfs/analyzer/vshadow_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/analyzer/xfs_analyzer_helper.py` & `dfvfs-20230408/dfvfs/analyzer/xfs_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/analyzer/xz_analyzer_helper.py` & `dfvfs-20230408/dfvfs/analyzer/xz_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/analyzer/zip_analyzer_helper.py` & `dfvfs-20230408/dfvfs/analyzer/zip_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/compression/bzip2_decompressor.py` & `dfvfs-20230408/dfvfs/compression/bzip2_decompressor.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/compression/manager.py` & `dfvfs-20230408/dfvfs/compression/manager.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/compression/xz_decompressor.py` & `dfvfs-20230408/dfvfs/compression/xz_decompressor.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/compression/zlib_decompressor.py` & `dfvfs-20230408/dfvfs/compression/zlib_decompressor.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/credentials/apfs_credentials.py` & `dfvfs-20230408/dfvfs/credentials/apfs_credentials.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/credentials/bde_credentials.py` & `dfvfs-20230408/dfvfs/credentials/bde_credentials.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/credentials/credentials.py` & `dfvfs-20230408/dfvfs/credentials/credentials.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/credentials/cs_credentials.py` & `dfvfs-20230408/dfvfs/credentials/cs_credentials.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/credentials/keychain.py` & `dfvfs-20230408/dfvfs/credentials/keychain.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/credentials/manager.py` & `dfvfs-20230408/dfvfs/credentials/manager.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/encoding/base16_decoder.py` & `dfvfs-20230408/dfvfs/encoding/base16_decoder.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/encoding/base32_decoder.py` & `dfvfs-20230408/dfvfs/encoding/base32_decoder.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/encoding/base64_decoder.py` & `dfvfs-20230408/dfvfs/encoding/base64_decoder.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/encoding/manager.py` & `dfvfs-20230408/dfvfs/encoding/manager.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/encryption/aes_decrypter.py` & `dfvfs-20230408/dfvfs/encryption/aes_decrypter.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/encryption/blowfish_decrypter.py` & `dfvfs-20230408/dfvfs/encryption/blowfish_decrypter.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/encryption/decrypter.py` & `dfvfs-20230408/dfvfs/encryption/decrypter.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/encryption/des3_decrypter.py` & `dfvfs-20230408/dfvfs/encryption/des3_decrypter.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/encryption/manager.py` & `dfvfs-20230408/dfvfs/encryption/manager.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/encryption/rc4_decrypter.py` & `dfvfs-20230408/dfvfs/encryption/rc4_decrypter.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/file_io/apfs_file_io.py` & `dfvfs-20230408/dfvfs/file_io/apfs_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/file_io/bde_file_io.py` & `dfvfs-20230408/dfvfs/file_io/bde_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/file_io/compressed_stream_io.py` & `dfvfs-20230408/dfvfs/file_io/compressed_stream_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/file_io/cpio_file_io.py` & `dfvfs-20230408/dfvfs/file_io/cpio_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/file_io/cs_file_io.py` & `dfvfs-20230408/dfvfs/file_io/cs_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/file_io/data_range_io.py` & `dfvfs-20230408/dfvfs/file_io/data_range_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/file_io/encoded_stream_io.py` & `dfvfs-20230408/dfvfs/file_io/encoded_stream_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/file_io/encrypted_stream_io.py` & `dfvfs-20230408/dfvfs/file_io/encrypted_stream_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/file_io/ewf_file_io.py` & `dfvfs-20230408/dfvfs/file_io/ewf_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/file_io/ext_file_io.py` & `dfvfs-20230408/dfvfs/file_io/ext_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/file_io/fake_file_io.py` & `dfvfs-20230408/dfvfs/file_io/fake_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/file_io/fat_file_io.py` & `dfvfs-20230408/dfvfs/file_io/fat_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/file_io/file_io.py` & `dfvfs-20230408/dfvfs/file_io/file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/file_io/file_object_io.py` & `dfvfs-20230408/dfvfs/file_io/file_object_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/file_io/gpt_file_io.py` & `dfvfs-20230408/dfvfs/file_io/gpt_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/file_io/gzip_file_io.py` & `dfvfs-20230408/dfvfs/file_io/gzip_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/file_io/hfs_file_io.py` & `dfvfs-20230408/dfvfs/file_io/hfs_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/file_io/luksde_file_io.py` & `dfvfs-20230408/dfvfs/file_io/luksde_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/file_io/lvm_file_io.py` & `dfvfs-20230408/dfvfs/file_io/lvm_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/file_io/modi_file_io.py` & `dfvfs-20230408/dfvfs/file_io/modi_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/file_io/ntfs_file_io.py` & `dfvfs-20230408/dfvfs/file_io/ntfs_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/file_io/os_file_io.py` & `dfvfs-20230408/dfvfs/file_io/os_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/file_io/phdi_file_io.py` & `dfvfs-20230408/dfvfs/file_io/phdi_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/file_io/qcow_file_io.py` & `dfvfs-20230408/dfvfs/file_io/qcow_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/file_io/raw_file_io.py` & `dfvfs-20230408/dfvfs/file_io/raw_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/file_io/sqlite_blob_file_io.py` & `dfvfs-20230408/dfvfs/file_io/sqlite_blob_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/file_io/tar_file_io.py` & `dfvfs-20230408/dfvfs/file_io/tar_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/file_io/tsk_file_io.py` & `dfvfs-20230408/dfvfs/file_io/tsk_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/file_io/tsk_partition_file_io.py` & `dfvfs-20230408/dfvfs/file_io/tsk_partition_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/file_io/vhdi_file_io.py` & `dfvfs-20230408/dfvfs/file_io/vhdi_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/file_io/vmdk_file_io.py` & `dfvfs-20230408/dfvfs/file_io/vmdk_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/file_io/vshadow_file_io.py` & `dfvfs-20230408/dfvfs/file_io/vshadow_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/file_io/xfs_file_io.py` & `dfvfs-20230408/dfvfs/file_io/xfs_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/file_io/zip_file_io.py` & `dfvfs-20230408/dfvfs/file_io/zip_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/helpers/command_line.py` & `dfvfs-20230408/dfvfs/helpers/command_line.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/helpers/data_slice.py` & `dfvfs-20230408/dfvfs/helpers/data_slice.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/helpers/fake_file_system_builder.py` & `dfvfs-20230408/dfvfs/helpers/fake_file_system_builder.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/helpers/file_system_searcher.py` & `dfvfs-20230408/dfvfs/helpers/file_system_searcher.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/helpers/source_scanner.py` & `dfvfs-20230408/dfvfs/helpers/source_scanner.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/helpers/text_file.py` & `dfvfs-20230408/dfvfs/helpers/text_file.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/helpers/volume_scanner.py` & `dfvfs-20230408/dfvfs/helpers/volume_scanner.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/helpers/windows_path_resolver.py` & `dfvfs-20230408/dfvfs/helpers/windows_path_resolver.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/lib/apfs_helper.py` & `dfvfs-20230408/dfvfs/lib/apfs_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/lib/bde_helper.py` & `dfvfs-20230408/dfvfs/lib/bde_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/lib/cpio.py` & `dfvfs-20230408/dfvfs/lib/cpio.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/lib/cpio.yaml` & `dfvfs-20230408/dfvfs/lib/cpio.yaml`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/lib/cs_helper.py` & `dfvfs-20230408/dfvfs/lib/cs_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/lib/data_format.py` & `dfvfs-20230408/dfvfs/lib/data_format.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/lib/decorators.py` & `dfvfs-20230408/dfvfs/lib/decorators.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/lib/definitions.py` & `dfvfs-20230408/dfvfs/lib/definitions.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/lib/errors.py` & `dfvfs-20230408/dfvfs/lib/errors.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/lib/ewf_helper.py` & `dfvfs-20230408/dfvfs/lib/ewf_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/lib/glob2regex.py` & `dfvfs-20230408/dfvfs/lib/glob2regex.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/lib/gpt_helper.py` & `dfvfs-20230408/dfvfs/lib/gpt_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/lib/gzipfile.py` & `dfvfs-20230408/dfvfs/lib/gzipfile.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/lib/gzipfile.yaml` & `dfvfs-20230408/dfvfs/lib/gzipfile.yaml`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/lib/luksde_helper.py` & `dfvfs-20230408/dfvfs/lib/luksde_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/lib/lvm_helper.py` & `dfvfs-20230408/dfvfs/lib/lvm_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/lib/raw_helper.py` & `dfvfs-20230408/dfvfs/lib/raw_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/lib/sqlite_database.py` & `dfvfs-20230408/dfvfs/lib/sqlite_database.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/lib/tsk_image.py` & `dfvfs-20230408/dfvfs/lib/tsk_image.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/lib/tsk_partition.py` & `dfvfs-20230408/dfvfs/lib/tsk_partition.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/lib/vshadow_helper.py` & `dfvfs-20230408/dfvfs/lib/vshadow_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/mount/manager.py` & `dfvfs-20230408/dfvfs/mount/manager.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/path/__init__.py` & `dfvfs-20230408/dfvfs/path/__init__.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/path/apfs_container_path_spec.py` & `dfvfs-20230408/dfvfs/path/apfs_container_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/path/apfs_path_spec.py` & `dfvfs-20230408/dfvfs/path/apfs_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/path/bde_path_spec.py` & `dfvfs-20230408/dfvfs/path/bde_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/path/compressed_stream_path_spec.py` & `dfvfs-20230408/dfvfs/path/compressed_stream_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/path/cpio_path_spec.py` & `dfvfs-20230408/dfvfs/path/cpio_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/path/cs_path_spec.py` & `dfvfs-20230408/dfvfs/path/cs_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/path/data_range_path_spec.py` & `dfvfs-20230408/dfvfs/path/data_range_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/path/encoded_stream_path_spec.py` & `dfvfs-20230408/dfvfs/path/encoded_stream_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/path/encrypted_stream_path_spec.py` & `dfvfs-20230408/dfvfs/path/encrypted_stream_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/path/ewf_path_spec.py` & `dfvfs-20230408/dfvfs/path/ewf_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/path/ext_path_spec.py` & `dfvfs-20230408/dfvfs/path/ext_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/path/factory.py` & `dfvfs-20230408/dfvfs/path/factory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/path/fake_path_spec.py` & `dfvfs-20230408/dfvfs/path/fake_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/path/fat_path_spec.py` & `dfvfs-20230408/dfvfs/path/fat_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/path/gpt_path_spec.py` & `dfvfs-20230408/dfvfs/path/gpt_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/path/gzip_path_spec.py` & `dfvfs-20230408/dfvfs/path/gzip_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/path/hfs_path_spec.py` & `dfvfs-20230408/dfvfs/path/hfs_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/path/location_path_spec.py` & `dfvfs-20230408/dfvfs/path/location_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/path/luksde_path_spec.py` & `dfvfs-20230408/dfvfs/path/luksde_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/path/lvm_path_spec.py` & `dfvfs-20230408/dfvfs/path/lvm_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/path/modi_path_spec.py` & `dfvfs-20230408/dfvfs/path/modi_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/path/mount_path_spec.py` & `dfvfs-20230408/dfvfs/path/mount_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/path/ntfs_path_spec.py` & `dfvfs-20230408/dfvfs/path/ntfs_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/path/os_path_spec.py` & `dfvfs-20230408/dfvfs/path/os_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/path/path_spec.py` & `dfvfs-20230408/dfvfs/path/path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/path/phdi_path_spec.py` & `dfvfs-20230408/dfvfs/path/phdi_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/path/qcow_path_spec.py` & `dfvfs-20230408/dfvfs/path/qcow_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/path/raw_path_spec.py` & `dfvfs-20230408/dfvfs/path/raw_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/path/sqlite_blob_path_spec.py` & `dfvfs-20230408/dfvfs/path/sqlite_blob_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/path/tar_path_spec.py` & `dfvfs-20230408/dfvfs/path/tar_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/path/tsk_partition_path_spec.py` & `dfvfs-20230408/dfvfs/path/tsk_partition_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/path/tsk_path_spec.py` & `dfvfs-20230408/dfvfs/path/tsk_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/path/vhdi_path_spec.py` & `dfvfs-20230408/dfvfs/path/vhdi_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/path/vmdk_path_spec.py` & `dfvfs-20230408/dfvfs/path/vmdk_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/path/vshadow_path_spec.py` & `dfvfs-20230408/dfvfs/path/vshadow_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/path/xfs_path_spec.py` & `dfvfs-20230408/dfvfs/path/xfs_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/path/zip_path_spec.py` & `dfvfs-20230408/dfvfs/path/zip_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/resolver/context.py` & `dfvfs-20230408/dfvfs/resolver/context.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/resolver/resolver.py` & `dfvfs-20230408/dfvfs/resolver/resolver.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/resolver_helpers/__init__.py` & `dfvfs-20230408/dfvfs/resolver_helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/resolver_helpers/apfs_container_resolver_helper.py` & `dfvfs-20230408/dfvfs/resolver_helpers/apfs_container_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/resolver_helpers/apfs_resolver_helper.py` & `dfvfs-20230408/dfvfs/resolver_helpers/apfs_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/resolver_helpers/bde_resolver_helper.py` & `dfvfs-20230408/dfvfs/resolver_helpers/bde_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/resolver_helpers/compressed_stream_resolver_helper.py` & `dfvfs-20230408/dfvfs/resolver_helpers/compressed_stream_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/resolver_helpers/cpio_resolver_helper.py` & `dfvfs-20230408/dfvfs/resolver_helpers/cpio_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/resolver_helpers/cs_resolver_helper.py` & `dfvfs-20230408/dfvfs/resolver_helpers/cs_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/resolver_helpers/data_range_resolver_helper.py` & `dfvfs-20230408/dfvfs/resolver_helpers/data_range_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/resolver_helpers/encoded_stream_resolver_helper.py` & `dfvfs-20230408/dfvfs/resolver_helpers/encoded_stream_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/resolver_helpers/encrypted_stream_resolver_helper.py` & `dfvfs-20230408/dfvfs/resolver_helpers/encrypted_stream_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/resolver_helpers/ewf_resolver_helper.py` & `dfvfs-20230408/dfvfs/resolver_helpers/ewf_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/resolver_helpers/ext_resolver_helper.py` & `dfvfs-20230408/dfvfs/resolver_helpers/ext_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/resolver_helpers/fake_resolver_helper.py` & `dfvfs-20230408/dfvfs/resolver_helpers/fake_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/resolver_helpers/fat_resolver_helper.py` & `dfvfs-20230408/dfvfs/resolver_helpers/fat_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/resolver_helpers/gpt_resolver_helper.py` & `dfvfs-20230408/dfvfs/resolver_helpers/gpt_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/resolver_helpers/gzip_resolver_helper.py` & `dfvfs-20230408/dfvfs/resolver_helpers/gzip_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/resolver_helpers/hfs_resolver_helper.py` & `dfvfs-20230408/dfvfs/resolver_helpers/hfs_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/resolver_helpers/luksde_resolver_helper.py` & `dfvfs-20230408/dfvfs/resolver_helpers/luksde_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/resolver_helpers/lvm_resolver_helper.py` & `dfvfs-20230408/dfvfs/resolver_helpers/lvm_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/resolver_helpers/manager.py` & `dfvfs-20230408/dfvfs/resolver_helpers/manager.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/resolver_helpers/modi_resolver_helper.py` & `dfvfs-20230408/dfvfs/resolver_helpers/modi_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/resolver_helpers/ntfs_resolver_helper.py` & `dfvfs-20230408/dfvfs/resolver_helpers/ntfs_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/resolver_helpers/os_resolver_helper.py` & `dfvfs-20230408/dfvfs/resolver_helpers/os_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/resolver_helpers/phdi_resolver_helper.py` & `dfvfs-20230408/dfvfs/resolver_helpers/phdi_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/resolver_helpers/qcow_resolver_helper.py` & `dfvfs-20230408/dfvfs/resolver_helpers/qcow_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/resolver_helpers/raw_resolver_helper.py` & `dfvfs-20230408/dfvfs/resolver_helpers/raw_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/resolver_helpers/resolver_helper.py` & `dfvfs-20230408/dfvfs/resolver_helpers/resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/resolver_helpers/sqlite_blob_resolver_helper.py` & `dfvfs-20230408/dfvfs/resolver_helpers/sqlite_blob_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/resolver_helpers/tar_resolver_helper.py` & `dfvfs-20230408/dfvfs/resolver_helpers/tar_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/resolver_helpers/tsk_partition_resolver_helper.py` & `dfvfs-20230408/dfvfs/resolver_helpers/tsk_partition_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/resolver_helpers/tsk_resolver_helper.py` & `dfvfs-20230408/dfvfs/resolver_helpers/tsk_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/resolver_helpers/vhdi_resolver_helper.py` & `dfvfs-20230408/dfvfs/resolver_helpers/vhdi_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/resolver_helpers/vmdk_resolver_helper.py` & `dfvfs-20230408/dfvfs/resolver_helpers/vmdk_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/resolver_helpers/vshadow_resolver_helper.py` & `dfvfs-20230408/dfvfs/resolver_helpers/vshadow_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/resolver_helpers/xfs_resolver_helper.py` & `dfvfs-20230408/dfvfs/resolver_helpers/xfs_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/resolver_helpers/zip_resolver_helper.py` & `dfvfs-20230408/dfvfs/resolver_helpers/zip_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/serializer/json_serializer.py` & `dfvfs-20230408/dfvfs/serializer/json_serializer.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/serializer/serializer.py` & `dfvfs-20230408/dfvfs/serializer/serializer.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/apfs_attribute.py` & `dfvfs-20230408/dfvfs/vfs/apfs_attribute.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/apfs_container_directory.py` & `dfvfs-20230408/dfvfs/vfs/apfs_container_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/apfs_container_file_entry.py` & `dfvfs-20230408/dfvfs/vfs/apfs_container_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/apfs_container_file_system.py` & `dfvfs-20230408/dfvfs/vfs/apfs_container_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/apfs_directory.py` & `dfvfs-20230408/dfvfs/vfs/apfs_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/apfs_file_entry.py` & `dfvfs-20230408/dfvfs/vfs/apfs_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/apfs_file_system.py` & `dfvfs-20230408/dfvfs/vfs/apfs_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/attribute.py` & `dfvfs-20230408/dfvfs/vfs/attribute.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/bde_file_entry.py` & `dfvfs-20230408/dfvfs/vfs/bde_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/bde_file_system.py` & `dfvfs-20230408/dfvfs/vfs/bde_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/compressed_stream_file_entry.py` & `dfvfs-20230408/dfvfs/vfs/compressed_stream_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/compressed_stream_file_system.py` & `dfvfs-20230408/dfvfs/vfs/compressed_stream_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/cpio_directory.py` & `dfvfs-20230408/dfvfs/vfs/cpio_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/cpio_file_entry.py` & `dfvfs-20230408/dfvfs/vfs/cpio_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/cpio_file_system.py` & `dfvfs-20230408/dfvfs/vfs/cpio_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/cs_directory.py` & `dfvfs-20230408/dfvfs/vfs/cs_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/cs_file_entry.py` & `dfvfs-20230408/dfvfs/vfs/cs_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/cs_file_system.py` & `dfvfs-20230408/dfvfs/vfs/cs_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/data_range_file_entry.py` & `dfvfs-20230408/dfvfs/vfs/data_range_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/data_range_file_system.py` & `dfvfs-20230408/dfvfs/vfs/data_range_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/data_stream.py` & `dfvfs-20230408/dfvfs/vfs/data_stream.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/directory.py` & `dfvfs-20230408/dfvfs/vfs/directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/encoded_stream_file_entry.py` & `dfvfs-20230408/dfvfs/vfs/encoded_stream_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/encoded_stream_file_system.py` & `dfvfs-20230408/dfvfs/vfs/encoded_stream_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/encrypted_stream_file_entry.py` & `dfvfs-20230408/dfvfs/vfs/encrypted_stream_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/encrypted_stream_file_system.py` & `dfvfs-20230408/dfvfs/vfs/encrypted_stream_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/ext_attribute.py` & `dfvfs-20230408/dfvfs/vfs/ext_attribute.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/ext_directory.py` & `dfvfs-20230408/dfvfs/vfs/ext_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/ext_file_entry.py` & `dfvfs-20230408/dfvfs/vfs/ext_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/ext_file_system.py` & `dfvfs-20230408/dfvfs/vfs/ext_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/extent.py` & `dfvfs-20230408/dfvfs/vfs/extent.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/fake_directory.py` & `dfvfs-20230408/dfvfs/vfs/fake_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/fake_file_entry.py` & `dfvfs-20230408/dfvfs/vfs/fake_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/fake_file_system.py` & `dfvfs-20230408/dfvfs/vfs/fake_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/fat_directory.py` & `dfvfs-20230408/dfvfs/vfs/fat_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/fat_file_entry.py` & `dfvfs-20230408/dfvfs/vfs/fat_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/fat_file_system.py` & `dfvfs-20230408/dfvfs/vfs/fat_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/file_entry.py` & `dfvfs-20230408/dfvfs/vfs/file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/file_system.py` & `dfvfs-20230408/dfvfs/vfs/file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/gpt_directory.py` & `dfvfs-20230408/dfvfs/vfs/gpt_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/gpt_file_entry.py` & `dfvfs-20230408/dfvfs/vfs/gpt_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/gpt_file_system.py` & `dfvfs-20230408/dfvfs/vfs/gpt_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/gzip_file_entry.py` & `dfvfs-20230408/dfvfs/vfs/gzip_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/gzip_file_system.py` & `dfvfs-20230408/dfvfs/vfs/gzip_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/hfs_attribute.py` & `dfvfs-20230408/dfvfs/vfs/hfs_attribute.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/hfs_data_stream.py` & `dfvfs-20230408/dfvfs/vfs/hfs_data_stream.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/hfs_directory.py` & `dfvfs-20230408/dfvfs/vfs/hfs_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/hfs_file_entry.py` & `dfvfs-20230408/dfvfs/vfs/hfs_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/hfs_file_system.py` & `dfvfs-20230408/dfvfs/vfs/hfs_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/luksde_file_entry.py` & `dfvfs-20230408/dfvfs/vfs/luksde_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/luksde_file_system.py` & `dfvfs-20230408/dfvfs/vfs/luksde_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/lvm_directory.py` & `dfvfs-20230408/dfvfs/vfs/lvm_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/lvm_file_entry.py` & `dfvfs-20230408/dfvfs/vfs/lvm_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/lvm_file_system.py` & `dfvfs-20230408/dfvfs/vfs/lvm_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/ntfs_attribute.py` & `dfvfs-20230408/dfvfs/vfs/ntfs_attribute.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/ntfs_data_stream.py` & `dfvfs-20230408/dfvfs/vfs/ntfs_data_stream.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/ntfs_directory.py` & `dfvfs-20230408/dfvfs/vfs/ntfs_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/ntfs_file_entry.py` & `dfvfs-20230408/dfvfs/vfs/ntfs_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/ntfs_file_system.py` & `dfvfs-20230408/dfvfs/vfs/ntfs_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/os_attribute.py` & `dfvfs-20230408/dfvfs/vfs/os_attribute.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/os_directory.py` & `dfvfs-20230408/dfvfs/vfs/os_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/os_file_entry.py` & `dfvfs-20230408/dfvfs/vfs/os_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/os_file_system.py` & `dfvfs-20230408/dfvfs/vfs/os_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/root_only_file_entry.py` & `dfvfs-20230408/dfvfs/vfs/root_only_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/root_only_file_system.py` & `dfvfs-20230408/dfvfs/vfs/root_only_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/sqlite_blob_directory.py` & `dfvfs-20230408/dfvfs/vfs/sqlite_blob_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/sqlite_blob_file_entry.py` & `dfvfs-20230408/dfvfs/vfs/sqlite_blob_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/sqlite_blob_file_system.py` & `dfvfs-20230408/dfvfs/vfs/sqlite_blob_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/tar_directory.py` & `dfvfs-20230408/dfvfs/vfs/tar_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/tar_file_entry.py` & `dfvfs-20230408/dfvfs/vfs/tar_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/tar_file_system.py` & `dfvfs-20230408/dfvfs/vfs/tar_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/tsk_attribute.py` & `dfvfs-20230408/dfvfs/vfs/tsk_attribute.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/tsk_data_stream.py` & `dfvfs-20230408/dfvfs/vfs/tsk_data_stream.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/tsk_directory.py` & `dfvfs-20230408/dfvfs/vfs/tsk_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/tsk_file_entry.py` & `dfvfs-20230408/dfvfs/vfs/tsk_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/tsk_file_system.py` & `dfvfs-20230408/dfvfs/vfs/tsk_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/tsk_partition_directory.py` & `dfvfs-20230408/dfvfs/vfs/tsk_partition_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/tsk_partition_file_entry.py` & `dfvfs-20230408/dfvfs/vfs/tsk_partition_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/tsk_partition_file_system.py` & `dfvfs-20230408/dfvfs/vfs/tsk_partition_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/vshadow_directory.py` & `dfvfs-20230408/dfvfs/vfs/vshadow_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/vshadow_file_entry.py` & `dfvfs-20230408/dfvfs/vfs/vshadow_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/vshadow_file_system.py` & `dfvfs-20230408/dfvfs/vfs/vshadow_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/xfs_attribute.py` & `dfvfs-20230408/dfvfs/vfs/xfs_attribute.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/xfs_directory.py` & `dfvfs-20230408/dfvfs/vfs/xfs_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/xfs_file_entry.py` & `dfvfs-20230408/dfvfs/vfs/xfs_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/xfs_file_system.py` & `dfvfs-20230408/dfvfs/vfs/xfs_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/zip_directory.py` & `dfvfs-20230408/dfvfs/vfs/zip_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/zip_file_entry.py` & `dfvfs-20230408/dfvfs/vfs/zip_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/vfs/zip_file_system.py` & `dfvfs-20230408/dfvfs/vfs/zip_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/volume/apfs_volume_system.py` & `dfvfs-20230408/dfvfs/volume/apfs_volume_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/volume/cs_volume_system.py` & `dfvfs-20230408/dfvfs/volume/cs_volume_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/volume/factory.py` & `dfvfs-20230408/dfvfs/volume/factory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/volume/gpt_volume_system.py` & `dfvfs-20230408/dfvfs/volume/gpt_volume_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/volume/lvm_volume_system.py` & `dfvfs-20230408/dfvfs/volume/lvm_volume_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/volume/tsk_volume_system.py` & `dfvfs-20230408/dfvfs/volume/tsk_volume_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/volume/volume_system.py` & `dfvfs-20230408/dfvfs/volume/volume_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs/volume/vshadow_volume_system.py` & `dfvfs-20230408/dfvfs/volume/vshadow_volume_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs.egg-info/PKG-INFO` & `dfvfs-20230408/dfvfs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfvfs
-Version: 20230407
+Version: 20230408
 Summary: Digital Forensics Virtual File System (dfVFS).
 Home-page: https://github.com/log2timeline/dfvfs
 Maintainer: Log2Timeline maintainers
 Maintainer-email: log2timeline-maintainers@googlegroups.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `dfvfs-20230407/dfvfs.egg-info/SOURCES.txt` & `dfvfs-20230408/dfvfs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/dfvfs.egg-info/requires.txt` & `dfvfs-20230408/dfvfs.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -23,8 +23,10 @@
 libsmraw-python>=20140612
 libvhdi-python>=20201014
 libvmdk-python>=20140421
 libvsgpt-python>=20211115
 libvshadow-python>=20160109
 libvslvm-python>=20160109
 pytsk3>=20210419
+
+[:platform_system != "Windows"]
 pyxattr>=0.7.2
```

### Comparing `dfvfs-20230407/dfvfs.ini` & `dfvfs-20230408/dfvfs.ini`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/docs/conf.py` & `dfvfs-20230408/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/docs/index.rst` & `dfvfs-20230408/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/docs/sources/Code-snippets.md` & `dfvfs-20230408/docs/sources/Code-snippets.md`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/docs/sources/Path-specifications.md` & `dfvfs-20230408/docs/sources/Path-specifications.md`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/docs/sources/Supported-formats.md` & `dfvfs-20230408/docs/sources/Supported-formats.md`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/docs/sources/api/dfvfs.analyzer.rst` & `dfvfs-20230408/docs/sources/api/dfvfs.analyzer.rst`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/docs/sources/api/dfvfs.compression.rst` & `dfvfs-20230408/docs/sources/api/dfvfs.compression.rst`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/docs/sources/api/dfvfs.credentials.rst` & `dfvfs-20230408/docs/sources/api/dfvfs.credentials.rst`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/docs/sources/api/dfvfs.encoding.rst` & `dfvfs-20230408/docs/sources/api/dfvfs.encoding.rst`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/docs/sources/api/dfvfs.encryption.rst` & `dfvfs-20230408/docs/sources/api/dfvfs.encryption.rst`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/docs/sources/api/dfvfs.file_io.rst` & `dfvfs-20230408/docs/sources/api/dfvfs.file_io.rst`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/docs/sources/api/dfvfs.helpers.rst` & `dfvfs-20230408/docs/sources/api/dfvfs.helpers.rst`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/docs/sources/api/dfvfs.lib.rst` & `dfvfs-20230408/docs/sources/api/dfvfs.lib.rst`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/docs/sources/api/dfvfs.path.rst` & `dfvfs-20230408/docs/sources/api/dfvfs.path.rst`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/docs/sources/api/dfvfs.resolver_helpers.rst` & `dfvfs-20230408/docs/sources/api/dfvfs.resolver_helpers.rst`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/docs/sources/api/dfvfs.serializer.rst` & `dfvfs-20230408/docs/sources/api/dfvfs.serializer.rst`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/docs/sources/api/dfvfs.vfs.rst` & `dfvfs-20230408/docs/sources/api/dfvfs.vfs.rst`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/docs/sources/api/dfvfs.volume.rst` & `dfvfs-20230408/docs/sources/api/dfvfs.volume.rst`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/docs/sources/developer/Adding-new-type.md` & `dfvfs-20230408/docs/sources/developer/Adding-new-type.md`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/docs/sources/developer/Helpers.md` & `dfvfs-20230408/docs/sources/developer/Helpers.md`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/docs/sources/developer/Internals.md` & `dfvfs-20230408/docs/sources/developer/Internals.md`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/docs/sources/user/Installation-instructions.md` & `dfvfs-20230408/docs/sources/user/Installation-instructions.md`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/requirements.txt` & `dfvfs-20230408/requirements.txt`

 * *Files 18% similar despite different names*

```diff
@@ -23,8 +23,8 @@
 libsmraw-python >= 20140612
 libvhdi-python >= 20201014
 libvmdk-python >= 20140421
 libvsgpt-python >= 20211115
 libvshadow-python >= 20160109
 libvslvm-python >= 20160109
 pytsk3 >= 20210419
-pyxattr >= 0.7.2
+pyxattr >= 0.7.2 ; platform_system != "Windows"
```

### Comparing `dfvfs-20230407/run_tests.py` & `dfvfs-20230408/run_tests.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/setup.cfg` & `dfvfs-20230408/setup.cfg`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/setup.py` & `dfvfs-20230408/setup.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/analyzer/analyzer.py` & `dfvfs-20230408/tests/analyzer/analyzer.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/analyzer/specification.py` & `dfvfs-20230408/tests/analyzer/specification.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/compression/bzip2_decompressor.py` & `dfvfs-20230408/tests/compression/bzip2_decompressor.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/compression/manager.py` & `dfvfs-20230408/tests/compression/manager.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/compression/xz_decompressor.py` & `dfvfs-20230408/tests/compression/xz_decompressor.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/compression/zlib_decompressor.py` & `dfvfs-20230408/tests/compression/zlib_decompressor.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/credentials/apfs_credentials.py` & `dfvfs-20230408/tests/credentials/apfs_credentials.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/credentials/bde_credentials.py` & `dfvfs-20230408/tests/credentials/bde_credentials.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/credentials/cs_credentials.py` & `dfvfs-20230408/tests/credentials/cs_credentials.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/credentials/encrypted_stream_credentials.py` & `dfvfs-20230408/tests/credentials/encrypted_stream_credentials.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/credentials/keychain.py` & `dfvfs-20230408/tests/credentials/keychain.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/credentials/luksde_credentials.py` & `dfvfs-20230408/tests/credentials/luksde_credentials.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/credentials/manager.py` & `dfvfs-20230408/tests/credentials/manager.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/encoding/base16_decoder.py` & `dfvfs-20230408/tests/encoding/base16_decoder.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/encoding/base32_decoder.py` & `dfvfs-20230408/tests/encoding/base32_decoder.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/encoding/base64_decoder.py` & `dfvfs-20230408/tests/encoding/base64_decoder.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/encoding/manager.py` & `dfvfs-20230408/tests/encoding/manager.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/encryption/aes_decrypter.py` & `dfvfs-20230408/tests/encryption/aes_decrypter.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/encryption/blowfish_decrypter.py` & `dfvfs-20230408/tests/encryption/blowfish_decrypter.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/encryption/decrypter.py` & `dfvfs-20230408/tests/encryption/decrypter.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/encryption/des3_decrypter.py` & `dfvfs-20230408/tests/encryption/des3_decrypter.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/encryption/manager.py` & `dfvfs-20230408/tests/encryption/manager.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/encryption/rc4_decrypter.py` & `dfvfs-20230408/tests/encryption/rc4_decrypter.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/file_io/apfs_file_io.py` & `dfvfs-20230408/tests/file_io/apfs_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/file_io/bde_file_io.py` & `dfvfs-20230408/tests/file_io/bde_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/file_io/compressed_stream_io.py` & `dfvfs-20230408/tests/file_io/compressed_stream_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/file_io/cpio_file_io.py` & `dfvfs-20230408/tests/file_io/cpio_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/file_io/cs_file_io.py` & `dfvfs-20230408/tests/file_io/cs_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/file_io/data_range_io.py` & `dfvfs-20230408/tests/file_io/data_range_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/file_io/encoded_stream_io.py` & `dfvfs-20230408/tests/file_io/encoded_stream_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/file_io/encrypted_stream_io.py` & `dfvfs-20230408/tests/file_io/encrypted_stream_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/file_io/ewf_file_io.py` & `dfvfs-20230408/tests/file_io/ewf_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/file_io/ext_file_io.py` & `dfvfs-20230408/tests/file_io/ext_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/file_io/fake_file_io.py` & `dfvfs-20230408/tests/file_io/fake_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/file_io/fat_file_io.py` & `dfvfs-20230408/tests/file_io/fat_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/file_io/gpt_file_io.py` & `dfvfs-20230408/tests/file_io/gpt_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/file_io/gzip_file_io.py` & `dfvfs-20230408/tests/file_io/gzip_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/file_io/hfs_file_io.py` & `dfvfs-20230408/tests/file_io/hfs_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/file_io/luksde_file_io.py` & `dfvfs-20230408/tests/file_io/luksde_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/file_io/lvm_file_io.py` & `dfvfs-20230408/tests/file_io/lvm_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/file_io/modi_file_io.py` & `dfvfs-20230408/tests/file_io/modi_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/file_io/ntfs_file_io.py` & `dfvfs-20230408/tests/file_io/ntfs_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/file_io/os_file_io.py` & `dfvfs-20230408/tests/file_io/os_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/file_io/phdi_file_io.py` & `dfvfs-20230408/tests/file_io/phdi_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/file_io/qcow_file_io.py` & `dfvfs-20230408/tests/file_io/qcow_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/file_io/raw_file_io.py` & `dfvfs-20230408/tests/file_io/raw_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/file_io/sqlite_blob_file_io.py` & `dfvfs-20230408/tests/file_io/sqlite_blob_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/file_io/tar_file_io.py` & `dfvfs-20230408/tests/file_io/tar_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/file_io/test_lib.py` & `dfvfs-20230408/tests/file_io/test_lib.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/file_io/tsk_file_io.py` & `dfvfs-20230408/tests/file_io/tsk_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/file_io/tsk_partition_file_io.py` & `dfvfs-20230408/tests/file_io/tsk_partition_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/file_io/vhdi_file_io.py` & `dfvfs-20230408/tests/file_io/vhdi_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/file_io/vmdk_file_io.py` & `dfvfs-20230408/tests/file_io/vmdk_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/file_io/vshadow_file_io.py` & `dfvfs-20230408/tests/file_io/vshadow_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/file_io/xfs_file_io.py` & `dfvfs-20230408/tests/file_io/xfs_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/file_io/zip_file_io.py` & `dfvfs-20230408/tests/file_io/zip_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/helpers/command_line.py` & `dfvfs-20230408/tests/helpers/command_line.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/helpers/data_slice.py` & `dfvfs-20230408/tests/helpers/data_slice.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/helpers/fake_file_system_builder.py` & `dfvfs-20230408/tests/helpers/fake_file_system_builder.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/helpers/file_system_searcher.py` & `dfvfs-20230408/tests/helpers/file_system_searcher.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/helpers/source_scanner.py` & `dfvfs-20230408/tests/helpers/source_scanner.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/helpers/text_file.py` & `dfvfs-20230408/tests/helpers/text_file.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/helpers/volume_scanner.py` & `dfvfs-20230408/tests/helpers/volume_scanner.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/helpers/windows_path_resolver.py` & `dfvfs-20230408/tests/helpers/windows_path_resolver.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/lib/apfs_helper.py` & `dfvfs-20230408/tests/lib/apfs_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/lib/cpio.py` & `dfvfs-20230408/tests/lib/cpio.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/lib/cs_helper.py` & `dfvfs-20230408/tests/lib/cs_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/lib/ewf_helper.py` & `dfvfs-20230408/tests/lib/ewf_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/lib/glob2regex.py` & `dfvfs-20230408/tests/lib/glob2regex.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/lib/gzipfile.py` & `dfvfs-20230408/tests/lib/gzipfile.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/lib/lvm_helper.py` & `dfvfs-20230408/tests/lib/lvm_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/lib/raw_helper.py` & `dfvfs-20230408/tests/lib/raw_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/mount/manager.py` & `dfvfs-20230408/tests/mount/manager.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/path/apfs_container_path_spec.py` & `dfvfs-20230408/tests/path/apfs_container_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/path/apfs_path_spec.py` & `dfvfs-20230408/tests/path/apfs_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/path/bde_path_spec.py` & `dfvfs-20230408/tests/path/bde_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/path/compressed_stream_path_spec.py` & `dfvfs-20230408/tests/path/compressed_stream_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/path/cpio_path_spec.py` & `dfvfs-20230408/tests/path/cpio_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/path/cs_path_spec.py` & `dfvfs-20230408/tests/path/cs_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/path/data_range_path_spec.py` & `dfvfs-20230408/tests/path/data_range_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/path/encoded_stream_path_spec.py` & `dfvfs-20230408/tests/path/encoded_stream_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/path/encryption_stream_path_spec.py` & `dfvfs-20230408/tests/path/encryption_stream_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/path/ewf_path_spec.py` & `dfvfs-20230408/tests/path/ewf_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/path/ext_path_spec.py` & `dfvfs-20230408/tests/path/ext_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/path/factory.py` & `dfvfs-20230408/tests/path/factory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/path/fake_path_spec.py` & `dfvfs-20230408/tests/path/fake_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/path/fat_path_spec.py` & `dfvfs-20230408/tests/path/fat_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/path/gpt_path_spec.py` & `dfvfs-20230408/tests/path/gpt_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/path/gzip_path_spec.py` & `dfvfs-20230408/tests/path/gzip_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/path/hfs_path_spec.py` & `dfvfs-20230408/tests/path/hfs_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/path/luksde_path_spec.py` & `dfvfs-20230408/tests/path/luksde_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/path/lvm_path_spec.py` & `dfvfs-20230408/tests/path/lvm_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/path/modi_path_spec.py` & `dfvfs-20230408/tests/path/modi_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/path/mount_path_spec.py` & `dfvfs-20230408/tests/path/mount_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/path/ntfs_path_spec.py` & `dfvfs-20230408/tests/path/ntfs_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/path/os_path_spec.py` & `dfvfs-20230408/tests/path/os_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/path/path_spec.py` & `dfvfs-20230408/tests/path/path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/path/phdi_path_spec.py` & `dfvfs-20230408/tests/path/phdi_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/path/qcow_path_spec.py` & `dfvfs-20230408/tests/path/qcow_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/path/raw_path_spec.py` & `dfvfs-20230408/tests/path/raw_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/path/sqlite_blob_path_spec.py` & `dfvfs-20230408/tests/path/sqlite_blob_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/path/tar_path_spec.py` & `dfvfs-20230408/tests/path/tar_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/path/test_lib.py` & `dfvfs-20230408/tests/path/test_lib.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/path/tsk_partition_path_spec.py` & `dfvfs-20230408/tests/path/tsk_partition_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/path/tsk_path_spec.py` & `dfvfs-20230408/tests/path/tsk_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/path/vhdi_path_spec.py` & `dfvfs-20230408/tests/path/vhdi_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/path/vmdk_path_spec.py` & `dfvfs-20230408/tests/path/vmdk_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/path/vshadow_path_spec.py` & `dfvfs-20230408/tests/path/vshadow_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/path/xfs_path_spec.py` & `dfvfs-20230408/tests/path/xfs_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/path/zip_path_spec.py` & `dfvfs-20230408/tests/path/zip_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/resolver/context.py` & `dfvfs-20230408/tests/resolver/context.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/resolver_helpers/apfs_resolver_helper.py` & `dfvfs-20230408/tests/resolver_helpers/apfs_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/resolver_helpers/bde_resolver_helper.py` & `dfvfs-20230408/tests/resolver_helpers/bde_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/resolver_helpers/compressed_stream_resolver_helper.py` & `dfvfs-20230408/tests/resolver_helpers/compressed_stream_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/resolver_helpers/cpio_resolver_helper.py` & `dfvfs-20230408/tests/resolver_helpers/cpio_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/resolver_helpers/cs_resolver_helper.py` & `dfvfs-20230408/tests/resolver_helpers/cs_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/resolver_helpers/encoded_stream_resolver_helper.py` & `dfvfs-20230408/tests/resolver_helpers/encoded_stream_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/resolver_helpers/encrypted_stream_resolver_helper.py` & `dfvfs-20230408/tests/resolver_helpers/encrypted_stream_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/resolver_helpers/ewf_resolver_helper.py` & `dfvfs-20230408/tests/resolver_helpers/ewf_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/resolver_helpers/ext_resolver_helper.py` & `dfvfs-20230408/tests/resolver_helpers/ext_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/resolver_helpers/fat_resolver_helper.py` & `dfvfs-20230408/tests/resolver_helpers/fat_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/resolver_helpers/gpt_resolver_helper.py` & `dfvfs-20230408/tests/resolver_helpers/gpt_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/resolver_helpers/gzip_resolver_helper.py` & `dfvfs-20230408/tests/resolver_helpers/gzip_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/resolver_helpers/hfs_resolver_helper.py` & `dfvfs-20230408/tests/resolver_helpers/hfs_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/resolver_helpers/luksde_resolver_helper.py` & `dfvfs-20230408/tests/resolver_helpers/luksde_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/resolver_helpers/lvm_resolver_helper.py` & `dfvfs-20230408/tests/resolver_helpers/lvm_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/resolver_helpers/manager.py` & `dfvfs-20230408/tests/resolver_helpers/manager.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/resolver_helpers/modi_resolver_helper.py` & `dfvfs-20230408/tests/resolver_helpers/modi_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/resolver_helpers/ntfs_resolver_helper.py` & `dfvfs-20230408/tests/resolver_helpers/ntfs_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/resolver_helpers/os_resolver_helper.py` & `dfvfs-20230408/tests/resolver_helpers/os_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/resolver_helpers/phdi_resolver_helper.py` & `dfvfs-20230408/tests/resolver_helpers/phdi_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/resolver_helpers/qcow_resolver_helper.py` & `dfvfs-20230408/tests/resolver_helpers/qcow_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/resolver_helpers/raw_resolver_helper.py` & `dfvfs-20230408/tests/resolver_helpers/raw_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/resolver_helpers/sqlite_blob_resolver_helper.py` & `dfvfs-20230408/tests/resolver_helpers/sqlite_blob_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/resolver_helpers/tar_resolver_helper.py` & `dfvfs-20230408/tests/resolver_helpers/tar_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/resolver_helpers/test_lib.py` & `dfvfs-20230408/tests/resolver_helpers/test_lib.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/resolver_helpers/tsk_partition_resolver_helper.py` & `dfvfs-20230408/tests/resolver_helpers/tsk_partition_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/resolver_helpers/tsk_resolver_helper.py` & `dfvfs-20230408/tests/resolver_helpers/tsk_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/resolver_helpers/vhdi_resolver_helper.py` & `dfvfs-20230408/tests/resolver_helpers/vhdi_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/resolver_helpers/vmdk_resolver_helper.py` & `dfvfs-20230408/tests/resolver_helpers/vmdk_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/resolver_helpers/vshadow_resolver_helper.py` & `dfvfs-20230408/tests/resolver_helpers/vshadow_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/resolver_helpers/xfs_resolver_helper.py` & `dfvfs-20230408/tests/resolver_helpers/xfs_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/resolver_helpers/zip_resolver_helper.py` & `dfvfs-20230408/tests/resolver_helpers/zip_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/serializer/json_serializer.py` & `dfvfs-20230408/tests/serializer/json_serializer.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/test_lib.py` & `dfvfs-20230408/tests/test_lib.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/apfs_attribute.py` & `dfvfs-20230408/tests/vfs/apfs_attribute.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/apfs_container_directory.py` & `dfvfs-20230408/tests/vfs/apfs_container_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/apfs_container_file_entry.py` & `dfvfs-20230408/tests/vfs/apfs_container_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/apfs_container_file_system.py` & `dfvfs-20230408/tests/vfs/apfs_container_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/apfs_directory.py` & `dfvfs-20230408/tests/vfs/apfs_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/apfs_file_entry.py` & `dfvfs-20230408/tests/vfs/apfs_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/apfs_file_system.py` & `dfvfs-20230408/tests/vfs/apfs_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/attribute.py` & `dfvfs-20230408/tests/vfs/attribute.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/bde_file_entry.py` & `dfvfs-20230408/tests/vfs/bde_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/bde_file_system.py` & `dfvfs-20230408/tests/vfs/bde_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/compressed_stream_file_entry.py` & `dfvfs-20230408/tests/vfs/compressed_stream_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/compressed_stream_file_system.py` & `dfvfs-20230408/tests/vfs/compressed_stream_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/cpio_directory.py` & `dfvfs-20230408/tests/vfs/cpio_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/cpio_file_entry.py` & `dfvfs-20230408/tests/vfs/cpio_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/cpio_file_system.py` & `dfvfs-20230408/tests/vfs/cpio_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/cs_file_entry.py` & `dfvfs-20230408/tests/vfs/cs_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/cs_file_system.py` & `dfvfs-20230408/tests/vfs/cs_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/data_range_file_entry.py` & `dfvfs-20230408/tests/vfs/data_range_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/data_range_file_system.py` & `dfvfs-20230408/tests/vfs/data_range_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/data_stream.py` & `dfvfs-20230408/tests/vfs/data_stream.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/directory.py` & `dfvfs-20230408/tests/vfs/directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/encoded_stream_file_entry.py` & `dfvfs-20230408/tests/vfs/encoded_stream_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/encoded_stream_file_system.py` & `dfvfs-20230408/tests/vfs/encoded_stream_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/encrypted_stream_file_entry.py` & `dfvfs-20230408/tests/vfs/encrypted_stream_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/encrypted_stream_file_system.py` & `dfvfs-20230408/tests/vfs/encrypted_stream_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/ext_attribute.py` & `dfvfs-20230408/tests/vfs/ext_attribute.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/ext_directory.py` & `dfvfs-20230408/tests/vfs/ext_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/ext_file_entry.py` & `dfvfs-20230408/tests/vfs/ext_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/ext_file_system.py` & `dfvfs-20230408/tests/vfs/ext_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/fake_directory.py` & `dfvfs-20230408/tests/vfs/fake_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/fake_file_entry.py` & `dfvfs-20230408/tests/vfs/fake_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/fake_file_system.py` & `dfvfs-20230408/tests/vfs/fake_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/fat_directory.py` & `dfvfs-20230408/tests/vfs/fat_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/fat_file_entry.py` & `dfvfs-20230408/tests/vfs/fat_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/fat_file_system.py` & `dfvfs-20230408/tests/vfs/fat_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/file_entry.py` & `dfvfs-20230408/tests/vfs/file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/file_system.py` & `dfvfs-20230408/tests/vfs/file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/gpt_directory.py` & `dfvfs-20230408/tests/vfs/gpt_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/gpt_file_entry.py` & `dfvfs-20230408/tests/vfs/gpt_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/gpt_file_system.py` & `dfvfs-20230408/tests/vfs/gpt_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/gzip_file_entry.py` & `dfvfs-20230408/tests/vfs/gzip_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/gzip_file_system.py` & `dfvfs-20230408/tests/vfs/gzip_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/hfs_attribute.py` & `dfvfs-20230408/tests/vfs/hfs_attribute.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/hfs_data_stream.py` & `dfvfs-20230408/tests/vfs/hfs_data_stream.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/hfs_directory.py` & `dfvfs-20230408/tests/vfs/hfs_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/hfs_file_entry.py` & `dfvfs-20230408/tests/vfs/hfs_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/hfs_file_system.py` & `dfvfs-20230408/tests/vfs/hfs_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/luksde_file_entry.py` & `dfvfs-20230408/tests/vfs/luksde_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/luksde_file_system.py` & `dfvfs-20230408/tests/vfs/luksde_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/lvm_directory.py` & `dfvfs-20230408/tests/vfs/lvm_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/lvm_file_entry.py` & `dfvfs-20230408/tests/vfs/lvm_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/lvm_file_system.py` & `dfvfs-20230408/tests/vfs/lvm_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/ntfs_attibute.py` & `dfvfs-20230408/tests/vfs/ntfs_attibute.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/ntfs_data_stream.py` & `dfvfs-20230408/tests/vfs/ntfs_data_stream.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/ntfs_directory.py` & `dfvfs-20230408/tests/vfs/ntfs_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/ntfs_file_entry.py` & `dfvfs-20230408/tests/vfs/ntfs_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/ntfs_file_system.py` & `dfvfs-20230408/tests/vfs/ntfs_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/os_directory.py` & `dfvfs-20230408/tests/vfs/os_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/os_file_entry.py` & `dfvfs-20230408/tests/vfs/os_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/os_file_system.py` & `dfvfs-20230408/tests/vfs/os_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/sqlite_blob_directory.py` & `dfvfs-20230408/tests/vfs/sqlite_blob_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/sqlite_blob_file_entry.py` & `dfvfs-20230408/tests/vfs/sqlite_blob_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/sqlite_blob_file_system.py` & `dfvfs-20230408/tests/vfs/sqlite_blob_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/tar_directory.py` & `dfvfs-20230408/tests/vfs/tar_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/tar_file_entry.py` & `dfvfs-20230408/tests/vfs/tar_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/tar_file_system.py` & `dfvfs-20230408/tests/vfs/tar_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/tsk_attribute.py` & `dfvfs-20230408/tests/vfs/tsk_attribute.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/tsk_data_stream.py` & `dfvfs-20230408/tests/vfs/tsk_data_stream.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/tsk_directory.py` & `dfvfs-20230408/tests/vfs/tsk_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/tsk_file_entry.py` & `dfvfs-20230408/tests/vfs/tsk_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/tsk_file_system.py` & `dfvfs-20230408/tests/vfs/tsk_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/tsk_partition_directory.py` & `dfvfs-20230408/tests/vfs/tsk_partition_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/tsk_partition_file_entry.py` & `dfvfs-20230408/tests/vfs/tsk_partition_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/tsk_partition_file_system.py` & `dfvfs-20230408/tests/vfs/tsk_partition_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/vshadow_directory.py` & `dfvfs-20230408/tests/vfs/vshadow_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/vshadow_file_entry.py` & `dfvfs-20230408/tests/vfs/vshadow_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/vshadow_file_system.py` & `dfvfs-20230408/tests/vfs/vshadow_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/xfs_attribute.py` & `dfvfs-20230408/tests/vfs/xfs_attribute.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/xfs_directory.py` & `dfvfs-20230408/tests/vfs/xfs_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/xfs_file_entry.py` & `dfvfs-20230408/tests/vfs/xfs_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/xfs_file_system.py` & `dfvfs-20230408/tests/vfs/xfs_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/zip_directory.py` & `dfvfs-20230408/tests/vfs/zip_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/zip_file_entry.py` & `dfvfs-20230408/tests/vfs/zip_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/vfs/zip_file_system.py` & `dfvfs-20230408/tests/vfs/zip_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/volume/apfs_volume_system.py` & `dfvfs-20230408/tests/volume/apfs_volume_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/volume/cs_volume_system.py` & `dfvfs-20230408/tests/volume/cs_volume_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/volume/factory.py` & `dfvfs-20230408/tests/volume/factory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/volume/gpt_volume_system.py` & `dfvfs-20230408/tests/volume/gpt_volume_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/volume/lvm_volume_system.py` & `dfvfs-20230408/tests/volume/lvm_volume_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/volume/tsk_volume_system.py` & `dfvfs-20230408/tests/volume/tsk_volume_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tests/volume/vshadow_volume_system.py` & `dfvfs-20230408/tests/volume/vshadow_volume_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/tox.ini` & `dfvfs-20230408/tox.ini`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/utils/dependencies.py` & `dfvfs-20230408/utils/dependencies.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/utils/generate_test_data_linux.sh` & `dfvfs-20230408/utils/generate_test_data_linux.sh`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/utils/generate_test_data_macos.sh` & `dfvfs-20230408/utils/generate_test_data_macos.sh`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/utils/generate_test_data_windows.bat` & `dfvfs-20230408/utils/generate_test_data_windows.bat`

 * *Files identical despite different names*

### Comparing `dfvfs-20230407/utils/update_release.sh` & `dfvfs-20230408/utils/update_release.sh`

 * *Files identical despite different names*

