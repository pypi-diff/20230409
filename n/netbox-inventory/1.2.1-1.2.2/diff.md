# Comparing `tmp/netbox-inventory-1.2.1.tar.gz` & `tmp/netbox-inventory-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-inventory-1.2.1.tar", last modified: Thu Mar 30 05:42:54 2023, max compression
+gzip compressed data, was "netbox-inventory-1.2.2.tar", last modified: Sun Apr  9 17:57:54 2023, max compression
```

## Comparing `netbox-inventory-1.2.1.tar` & `netbox-inventory-1.2.2.tar`

### file list

```diff
@@ -1,102 +1,103 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 05:42:54.165546 netbox-inventory-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8079 2023-03-30 05:42:54.165546 netbox-inventory-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7501 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 05:42:54.153545 netbox-inventory-1.2.1/netbox_inventory/
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/analyzers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 05:42:54.157546 netbox-inventory-1.2.1/netbox_inventory/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/api/nested_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/api/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/choices.py
--rw-r--r--   0 runner    (1001) docker     (123)    10860 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/filtersets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 05:42:54.157546 netbox-inventory-1.2.1/netbox_inventory/forms/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6487 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/forms/assign.py
--rw-r--r--   0 runner    (1001) docker     (123)    16144 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/forms/bulk.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/forms/bulk_add.py
--rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/forms/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     8746 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/forms/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/forms/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 05:42:54.157546 netbox-inventory-1.2.1/netbox_inventory/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     6962 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/migrations/0001_initial_prod.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/migrations/0002_alter_asset_serial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/migrations/0003_add_inventoryitemgroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/migrations/0004_inventoryitemgroup_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16765 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/navigation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/signals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11975 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/tables.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/template_content.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 05:42:54.153545 netbox-inventory-1.2.1/netbox_inventory/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 05:42:54.157546 netbox-inventory-1.2.1/netbox_inventory/templates/netbox_inventory/
--rw-r--r--   0 runner    (1001) docker     (123)     7434 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/templates/netbox_inventory/asset.html
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/templates/netbox_inventory/asset_assign.html
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/templates/netbox_inventory/asset_bulk_add.html
--rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/templates/netbox_inventory/asset_bulk_import.html
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/templates/netbox_inventory/asset_create.html
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/templates/netbox_inventory/asset_edit.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 05:42:54.161546 netbox-inventory-1.2.1/netbox_inventory/templates/netbox_inventory/inc/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/templates/netbox_inventory/inc/asset_edit_header.html
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/templates/netbox_inventory/inc/asset_info.html
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/templates/netbox_inventory/inc/asset_warranty.html
--rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/templates/netbox_inventory/inventoryitemgroup.html
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/templates/netbox_inventory/inventoryitemtype.html
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/templates/netbox_inventory/purchase.html
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/templates/netbox_inventory/supplier.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 05:42:54.161546 netbox-inventory-1.2.1/netbox_inventory/templates/netbox_inventory/tabs/
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/templates/netbox_inventory/tabs/located_assets_base.html
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/templates/netbox_inventory/tabs/located_assets_location.html
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/templates/netbox_inventory/tabs/located_assets_rack.html
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/templates/netbox_inventory/tabs/located_assets_site.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 05:42:54.161546 netbox-inventory-1.2.1/netbox_inventory/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 05:42:54.161546 netbox-inventory-1.2.1/netbox_inventory/tests/asset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/tests/asset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/tests/asset/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6358 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/tests/asset/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    11534 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/tests/asset/test_views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/tests/custom.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 05:42:54.161546 netbox-inventory-1.2.1/netbox_inventory/tests/inventoryitem_group/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/tests/inventoryitem_group/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/tests/inventoryitem_group/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/tests/inventoryitem_group/test_views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 05:42:54.161546 netbox-inventory-1.2.1/netbox_inventory/tests/inventoryitem_type/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/tests/inventoryitem_type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/tests/inventoryitem_type/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/tests/inventoryitem_type/test_views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 05:42:54.161546 netbox-inventory-1.2.1/netbox_inventory/tests/purchase/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/tests/purchase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/tests/purchase/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/tests/purchase/test_views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 05:42:54.161546 netbox-inventory-1.2.1/netbox_inventory/tests/supplier/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/tests/supplier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/tests/supplier/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/tests/supplier/test_views.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/tests/test_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 05:42:54.161546 netbox-inventory-1.2.1/netbox_inventory/views/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8810 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/views/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/views/asset_assign.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/views/asset_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/views/inventoryitem_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/views/inventoryitem_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/views/purchase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/views/supplier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/netbox_inventory/views/tabs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 05:42:54.157546 netbox-inventory-1.2.1/netbox_inventory.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8079 2023-03-30 05:42:54.000000 netbox-inventory-1.2.1/netbox_inventory.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-03-30 05:42:54.000000 netbox-inventory-1.2.1/netbox_inventory.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 05:42:54.000000 netbox-inventory-1.2.1/netbox_inventory.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-30 05:42:54.000000 netbox-inventory-1.2.1/netbox_inventory.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-03-30 05:42:45.000000 netbox-inventory-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 05:42:54.165546 netbox-inventory-1.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:57:54.173767 netbox-inventory-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8138 2023-04-09 17:57:54.173767 netbox-inventory-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7560 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:57:54.165767 netbox-inventory-1.2.2/netbox_inventory/
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/analyzers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:57:54.165767 netbox-inventory-1.2.2/netbox_inventory/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/api/nested_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/choices.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10863 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/filtersets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:57:54.165767 netbox-inventory-1.2.2/netbox_inventory/forms/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6487 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/forms/assign.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16144 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/forms/bulk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/forms/bulk_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/forms/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9121 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/forms/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/forms/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:57:54.169767 netbox-inventory-1.2.2/netbox_inventory/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     6962 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/migrations/0001_initial_prod.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/migrations/0002_alter_asset_serial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/migrations/0003_add_inventoryitemgroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/migrations/0004_inventoryitemgroup_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16865 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/navigation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11975 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/template_content.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:57:54.161767 netbox-inventory-1.2.2/netbox_inventory/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:57:54.169767 netbox-inventory-1.2.2/netbox_inventory/templates/netbox_inventory/
+-rw-r--r--   0 runner    (1001) docker     (123)     7446 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/templates/netbox_inventory/asset.html
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/templates/netbox_inventory/asset_assign.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/templates/netbox_inventory/asset_bulk_add.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/templates/netbox_inventory/asset_bulk_import.html
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/templates/netbox_inventory/asset_create.html
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/templates/netbox_inventory/asset_edit.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:57:54.169767 netbox-inventory-1.2.2/netbox_inventory/templates/netbox_inventory/inc/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/templates/netbox_inventory/inc/asset_edit_header.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/templates/netbox_inventory/inc/asset_info.html
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/templates/netbox_inventory/inc/asset_warranty.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/templates/netbox_inventory/inventoryitemgroup.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/templates/netbox_inventory/inventoryitemtype.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/templates/netbox_inventory/purchase.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/templates/netbox_inventory/supplier.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:57:54.169767 netbox-inventory-1.2.2/netbox_inventory/templates/netbox_inventory/tabs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/templates/netbox_inventory/tabs/located_assets_base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/templates/netbox_inventory/tabs/located_assets_location.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/templates/netbox_inventory/tabs/located_assets_rack.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/templates/netbox_inventory/tabs/located_assets_site.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:57:54.169767 netbox-inventory-1.2.2/netbox_inventory/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:57:54.169767 netbox-inventory-1.2.2/netbox_inventory/tests/asset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/tests/asset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/tests/asset/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6099 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/tests/asset/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12618 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/tests/asset/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/tests/custom.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:57:54.169767 netbox-inventory-1.2.2/netbox_inventory/tests/inventoryitem_group/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/tests/inventoryitem_group/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/tests/inventoryitem_group/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/tests/inventoryitem_group/test_views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:57:54.173767 netbox-inventory-1.2.2/netbox_inventory/tests/inventoryitem_type/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/tests/inventoryitem_type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/tests/inventoryitem_type/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/tests/inventoryitem_type/test_views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:57:54.173767 netbox-inventory-1.2.2/netbox_inventory/tests/purchase/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/tests/purchase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/tests/purchase/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/tests/purchase/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/tests/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:57:54.173767 netbox-inventory-1.2.2/netbox_inventory/tests/supplier/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/tests/supplier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/tests/supplier/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/tests/supplier/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/tests/test_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:57:54.173767 netbox-inventory-1.2.2/netbox_inventory/views/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8810 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/views/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/views/asset_assign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/views/asset_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/views/inventoryitem_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/views/inventoryitem_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/views/purchase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/views/supplier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/views/tabs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:57:54.165767 netbox-inventory-1.2.2/netbox_inventory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8138 2023-04-09 17:57:54.000000 netbox-inventory-1.2.2/netbox_inventory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-04-09 17:57:54.000000 netbox-inventory-1.2.2/netbox_inventory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 17:57:54.000000 netbox-inventory-1.2.2/netbox_inventory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-09 17:57:54.000000 netbox-inventory-1.2.2/netbox_inventory.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 17:57:54.173767 netbox-inventory-1.2.2/setup.cfg
```

### Comparing `netbox-inventory-1.2.1/LICENSE` & `netbox-inventory-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.1/PKG-INFO` & `netbox-inventory-1.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-inventory
-Version: 1.2.1
+Version: 1.2.2
 Summary: Inventory asset management in NetBox
 Author-email: Matej Vadnjal <matej.vadnjal@arnes.si>
 Project-URL: Homepage, https://github.com/ArnesSI/netbox-inventory/
 Project-URL: Bug Tracker, https://github.com/ArnesSI/netbox-inventory/issues/
 Keywords: netbox,netbox-plugin,inventory
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -130,24 +130,24 @@
 ```python
 PLUGINS = [
     'netbox_inventory'
 ]
 
 PLUGINS_CONFIG = {
     "netbox_inventory": {
-        # Example settings below
+        # Example settings below, see "Available settings"
+        # in README.md for all possible settings
         "used_status_name": "used",
         "stored_status_name": "stored",
-        "sync_serial_number": True,
-        "sync_asset_tag": True,
+        "sync_hardware_serial_asset_tag": True,
     },
 }
 ```
 
-Available settings:
+#### Available settings
 
 | Setting | Default value | Description |
 |---------|---------------|-------------|
 | `top_level_menu` | `True`| Add netbox-inventory to the top level of netbox navigation menu under Inventory heading. If set to False the plugin will add a menu item under the Plugins menu item. This setting is only valid under netbox v3.4 and newer.
 | `used_status_name` | `'used'`| Status that indicates asset is in use. See "Automatic management of asset status" below for more info on this setting.
 | `stored_status_name` | `'stored'`| Status that indicates asset is in storage. See "Automatic management of asset status" below for more info on this setting.
 | `sync_hardware_serial_asset_tag` | `False` | When an asset is assigned or unassigned to a device, module or inventory item, update its serial number and asset tag to be in sync with the asset? |
```

### Comparing `netbox-inventory-1.2.1/README.md` & `netbox-inventory-1.2.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -115,24 +115,24 @@
 ```python
 PLUGINS = [
     'netbox_inventory'
 ]
 
 PLUGINS_CONFIG = {
     "netbox_inventory": {
-        # Example settings below
+        # Example settings below, see "Available settings"
+        # in README.md for all possible settings
         "used_status_name": "used",
         "stored_status_name": "stored",
-        "sync_serial_number": True,
-        "sync_asset_tag": True,
+        "sync_hardware_serial_asset_tag": True,
     },
 }
 ```
 
-Available settings:
+#### Available settings
 
 | Setting | Default value | Description |
 |---------|---------------|-------------|
 | `top_level_menu` | `True`| Add netbox-inventory to the top level of netbox navigation menu under Inventory heading. If set to False the plugin will add a menu item under the Plugins menu item. This setting is only valid under netbox v3.4 and newer.
 | `used_status_name` | `'used'`| Status that indicates asset is in use. See "Automatic management of asset status" below for more info on this setting.
 | `stored_status_name` | `'stored'`| Status that indicates asset is in storage. See "Automatic management of asset status" below for more info on this setting.
 | `sync_hardware_serial_asset_tag` | `False` | When an asset is assigned or unassigned to a device, module or inventory item, update its serial number and asset tag to be in sync with the asset? |
```

### Comparing `netbox-inventory-1.2.1/netbox_inventory/__init__.py` & `netbox-inventory-1.2.2/netbox_inventory/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     name = 'netbox_inventory'
     verbose_name = 'NetBox Inventory'
     version = __version__
     description = 'Inventory asset management in NetBox'
     author = 'Matej Vadnjal'
     author_email = 'matej.vadnjal@arnes.si'
     base_url = 'inventory'
-    min_version = '3.3.0'
+    min_version = '3.4.0'
     default_settings = {
         'top_level_menu': True,
         'used_status_name': 'used',
         'stored_status_name': 'stored',
         'sync_hardware_serial_asset_tag': False,
         'asset_import_create_purchase': False,
         'asset_import_create_device_type': False,
```

### Comparing `netbox-inventory-1.2.1/netbox_inventory/analyzers.py` & `netbox-inventory-1.2.2/netbox_inventory/analyzers.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.1/netbox_inventory/api/nested_serializers.py` & `netbox-inventory-1.2.2/netbox_inventory/api/nested_serializers.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.1/netbox_inventory/api/serializers.py` & `netbox-inventory-1.2.2/netbox_inventory/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.1/netbox_inventory/api/urls.py` & `netbox-inventory-1.2.2/netbox_inventory/api/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.1/netbox_inventory/api/views.py` & `netbox-inventory-1.2.2/netbox_inventory/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.1/netbox_inventory/filtersets.py` & `netbox-inventory-1.2.2/netbox_inventory/filtersets.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,15 +155,15 @@
         model = Asset
         fields = ('id', 'name', 'serial', 'asset_tag')
 
     def search(self, queryset, name, value):
         query = Q(
             Q(serial__icontains=value)|
             Q(name__icontains=value)|
-            Q(asset_tag__iexact=value)|
+            Q(asset_tag__icontains=value)|
             Q(device_type__model__icontains=value)|
             Q(module_type__model__icontains=value)|
             Q(inventoryitem_type__model__icontains=value)
         )
         return queryset.filter(query)
 
     def filter_kind(self, queryset, name, value):
```

### Comparing `netbox-inventory-1.2.1/netbox_inventory/forms/assign.py` & `netbox-inventory-1.2.2/netbox_inventory/forms/assign.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.1/netbox_inventory/forms/bulk.py` & `netbox-inventory-1.2.2/netbox_inventory/forms/bulk.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.1/netbox_inventory/forms/create.py` & `netbox-inventory-1.2.2/netbox_inventory/forms/create.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.1/netbox_inventory/forms/filters.py` & `netbox-inventory-1.2.2/netbox_inventory/forms/filters.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     'InventoryItemGroupFilterForm',
 )
 
 
 class AssetFilterForm(NetBoxModelFilterSetForm):
     model = Asset
     fieldsets = (
-        (None, ('q', 'tag', 'status')),
+        (None, ('q', 'filter_id', 'tag', 'status')),
         ('Hardware', (
             'kind', 'manufacturer_id', 'device_type_id', 'module_type_id',
             'inventoryitem_type_id', 'inventoryitem_group_id', 'is_assigned'
         )),
         ('Usage', ('tenant_id', 'contact_id')),
         ('Purchase', (
             'owner_id', 'purchase_id', 'supplier_id', 'purchase_date_after',
@@ -233,14 +233,18 @@
     )
 
     tag = TagFilterField(model)
 
 
 class PurchaseFilterForm(NetBoxModelFilterSetForm):
     model = Purchase
+    fieldsets = (
+        (None, ('q', 'filter_id', 'tag')),
+        ('Purchase', ('supplier_id', 'date_after', 'date_before')),
+    )
 
     supplier_id = DynamicModelMultipleChoiceField(
         queryset=Supplier.objects.all(),
         required=False,
         label='Supplier',
     )
     date_after = forms.DateField(
@@ -254,14 +258,18 @@
         widget=DatePicker,
     )
     tag = TagFilterField(model)
 
 
 class InventoryItemTypeFilterForm(NetBoxModelFilterSetForm):
     model = InventoryItemType
+    fieldsets = (
+        (None, ('q', 'filter_id', 'tag')),
+        ('Inventory Item Type', ('manufacturer_id', 'inventoryitem_group_id')),
+    )
     manufacturer_id = DynamicModelMultipleChoiceField(
         queryset=Manufacturer.objects.all(),
         required=False,
         label='Manufacturer',
     )
     inventoryitem_group_id = DynamicModelMultipleChoiceField(
         queryset=InventoryItemGroup.objects.all(),
@@ -269,13 +277,16 @@
         label='Inventory Item Group',
     )
     tag = TagFilterField(model)
 
 
 class InventoryItemGroupFilterForm(NetBoxModelFilterSetForm):
     model = InventoryItemGroup
+    fieldsets = (
+        (None, ('q', 'filter_id', 'tag', 'parent_id')),
+    )
     parent_id = DynamicModelMultipleChoiceField(
         queryset=InventoryItemGroup.objects.all(),
         required=False,
         label='Parent group'
     )
     tag = TagFilterField(model)
```

### Comparing `netbox-inventory-1.2.1/netbox_inventory/forms/models.py` & `netbox-inventory-1.2.2/netbox_inventory/forms/models.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.1/netbox_inventory/migrations/0001_initial_prod.py` & `netbox-inventory-1.2.2/netbox_inventory/migrations/0001_initial_prod.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.1/netbox_inventory/migrations/0003_add_inventoryitemgroup.py` & `netbox-inventory-1.2.2/netbox_inventory/migrations/0003_add_inventoryitemgroup.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.1/netbox_inventory/migrations/0004_inventoryitemgroup_tree.py` & `netbox-inventory-1.2.2/netbox_inventory/migrations/0004_inventoryitemgroup_tree.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.1/netbox_inventory/models.py` & `netbox-inventory-1.2.2/netbox_inventory/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -356,15 +356,18 @@
     def get_absolute_url(self):
         return reverse('plugins:netbox_inventory:asset', args=[self.pk])
 
     def get_status_color(self):
         return AssetStatusChoices.colors.get(self.status)
 
     def __str__(self):
-        return f'{self.hardware_type} {self.serial}'
+        if self.serial:
+            return f'{self.hardware_type} {self.serial}'
+        else:
+            return f'{self.hardware_type} (id:{self.id})'
 
     class Meta:
         ordering = ('device_type', 'module_type', 'inventoryitem_type', 'serial',)
         unique_together = (
             ('device_type', 'serial'),
             ('module_type', 'serial'),
             ('inventoryitem_type', 'serial'),
```

### Comparing `netbox-inventory-1.2.1/netbox_inventory/navigation.py` & `netbox-inventory-1.2.2/netbox_inventory/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.1/netbox_inventory/search.py` & `netbox-inventory-1.2.2/netbox_inventory/search.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.1/netbox_inventory/signals.py` & `netbox-inventory-1.2.2/netbox_inventory/signals.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from django.dispatch import receiver
 from django.db.models.signals import pre_save, pre_delete
 
 from dcim.models import Device, Module, InventoryItem
 from utilities.exceptions import AbortRequest
 from .models import Asset
-from .utils import get_plugin_setting, get_status_for
+from .utils import get_plugin_setting, get_status_for, is_equal_none
 
 
 logger = logging.getLogger('netbox.netbox_inventory.signals')
 
 
 @receiver(pre_save, sender=Device)
 @receiver(pre_save, sender=Module)
@@ -27,16 +27,21 @@
         # will raise RelatedObjectDoesNotExist if not set
         asset = instance.assigned_asset
     except Asset.DoesNotExist:
         return
     if not get_plugin_setting('sync_hardware_serial_asset_tag'):
         # don't enforce if sync not enabled
         return
-    if asset.serial != instance.serial or asset.asset_tag != instance.asset_tag:
-        raise AbortRequest(f'Cannot change {asset.kind} serial and asset tag if asset is assigned. Please update via inventory > asset instead.')
+    if instance.pk and (
+        not is_equal_none(asset.serial, instance.serial)
+        or not is_equal_none(asset.asset_tag, instance.asset_tag)
+    ):
+        raise AbortRequest(
+            f'Cannot change {asset.kind} serial and asset tag if asset is assigned. Please update via inventory > asset instead.'
+        )
 
 
 @receiver(pre_delete, sender=Device)
 @receiver(pre_delete, sender=Module)
 @receiver(pre_delete, sender=InventoryItem)
 def free_assigned_asset(instance, **kwargs):
     """
```

### Comparing `netbox-inventory-1.2.1/netbox_inventory/tables.py` & `netbox-inventory-1.2.2/netbox_inventory/tables.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.1/netbox_inventory/template_content.py` & `netbox-inventory-1.2.2/netbox_inventory/template_content.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.1/netbox_inventory/templates/netbox_inventory/asset.html` & `netbox-inventory-1.2.2/netbox_inventory/templates/netbox_inventory/asset.html`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
             </tr>
             <tr>
               <th scope="row">Asset Tag</th>
               <td class="font-monospace">{{ object.asset_tag|placeholder }}</td>
             </tr>
             <tr>
               <th scope="row">Serial Number</th>
-              <td class="font-monospace">{{ object.serial }}</td>
+              <td class="font-monospace">{{ object.serial|placeholder }}</td>
             </tr>
             <tr>
               <th scope="row">Status</th>
               <td>{% badge object.get_status_display bg_color=object.get_status_color %}</td>
             </tr>
             <tr>
               <th scope="row">{{ object.get_kind_display }} Type</th>
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 block title %}{{ object.hardware_type.manufacturer }} {{ object }}{% endblock
 %} {% block breadcrumbs %} {{ block.super }}
 {{_object.hardware_type.manufacturer_}}_{{_object.hardware_type_}}
 {% endblock %} {% block content %}
 ** Asset **
 Name                    {{ object.name|placeholder }}
 Asset Tag               {{ object.asset_tag|placeholder }}
-Serial Number           {{ object.serial }}
+Serial Number           {{ object.serial|placeholder }}
 Status                  {% badge object.get_status_display
                         bg_color=object.get_status_color %}
 {
 {                       {{_object.hardware_type.manufacturer_}}_{
 object.get_kind_display {_object.hardware_type_}}
 }} Type
                         {% if object.inventoryitem_type.inventoryitem_group %} {%
```

### Comparing `netbox-inventory-1.2.1/netbox_inventory/templates/netbox_inventory/asset_bulk_add.html` & `netbox-inventory-1.2.2/netbox_inventory/templates/netbox_inventory/asset_bulk_add.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.1/netbox_inventory/templates/netbox_inventory/asset_bulk_import.html` & `netbox-inventory-1.2.2/netbox_inventory/templates/netbox_inventory/asset_bulk_import.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.1/netbox_inventory/templates/netbox_inventory/inc/asset_edit_header.html` & `netbox-inventory-1.2.2/netbox_inventory/templates/netbox_inventory/inc/asset_edit_header.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.1/netbox_inventory/templates/netbox_inventory/inc/asset_info.html` & `netbox-inventory-1.2.2/netbox_inventory/templates/netbox_inventory/inc/asset_info.html`

 * *Files 19% similar despite different names*

```diff
@@ -3,29 +3,33 @@
 <div class="card">
   <h5 class="card-header">Asset</h5>
   <div class="card-body">
   {% if asset %}
     <table class="table table-hover attr-table">
       <tr>
         <th scope="row"><span title="Asset name">Name</span></th>
-        <td><a href="{% url "plugins:netbox_inventory:asset" asset.pk %}">{{ asset.name|default:'(None)' }}</a></td>
+        <td><a href="{% url "plugins:netbox_inventory:asset" asset.pk %}">{{ asset.hardware_type.manufacturer }} {{ asset }}{% if asset.name %} ({{ asset.name }}){% endif %}</a></td>
       </tr>
       <tr>
         <th scope="row"><span title="Asset status">Status</span></a></th>
         <td>{% badge asset.get_status_display bg_color=asset.get_status_color %}</a></td>
       </tr>
       <tr>
         <th scope="row">Owner</th>
         <td>{{ asset.owner|linkify|placeholder }}</td>
       </tr>
       <tr>
+        <th scope="row">Purchase</th>
+        <td>{{ asset.purchase|linkify|placeholder }}</td>
+      </tr>
+      <tr>
         <th>Warranty remaining</th>
         <td>
           {% include "netbox_inventory/inc/asset_warranty.html" with asset=asset %}
         </td>
       </tr>
     </table>
   {% else %}
-    <div class="text-muted">None</div>
+    <div class="text-muted">None assigned</div>
   {% endif %}
   </div>
 </div>
```

#### html2text {}

```diff
@@ -1,12 +1,14 @@
 {% load helpers %}
 ** Asset **
 {% if asset %}
-Name                asset.pk %}">{{ asset.name|default:'(None)' }}
+Name                asset.pk %}">{{ asset.hardware_type.manufacturer }} {
+                   { asset }}{% if asset.name %} ({{ asset.name }}){% endif %}
 Status             {% badge asset.get_status_display
                    bg_color=asset.get_status_color %}
 Owner              {{ asset.owner|linkify|placeholder }}
+Purchase           {{ asset.purchase|linkify|placeholder }}
 Warranty remaining {% include "netbox_inventory/inc/asset_warranty.html" with
                    asset=asset %}
 {% else %}
-None
+None assigned
 {% endif %}
```

### Comparing `netbox-inventory-1.2.1/netbox_inventory/templates/netbox_inventory/inc/asset_warranty.html` & `netbox-inventory-1.2.2/netbox_inventory/templates/netbox_inventory/inc/asset_warranty.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.1/netbox_inventory/templates/netbox_inventory/inventoryitemgroup.html` & `netbox-inventory-1.2.2/netbox_inventory/templates/netbox_inventory/inventoryitemgroup.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.1/netbox_inventory/templates/netbox_inventory/inventoryitemtype.html` & `netbox-inventory-1.2.2/netbox_inventory/templates/netbox_inventory/inventoryitemtype.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.1/netbox_inventory/templates/netbox_inventory/purchase.html` & `netbox-inventory-1.2.2/netbox_inventory/templates/netbox_inventory/purchase.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.1/netbox_inventory/templates/netbox_inventory/supplier.html` & `netbox-inventory-1.2.2/netbox_inventory/templates/netbox_inventory/supplier.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.1/netbox_inventory/templates/netbox_inventory/tabs/located_assets_base.html` & `netbox-inventory-1.2.2/netbox_inventory/templates/netbox_inventory/tabs/located_assets_base.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.1/netbox_inventory/templates/netbox_inventory/tabs/located_assets_location.html` & `netbox-inventory-1.2.2/netbox_inventory/templates/netbox_inventory/tabs/located_assets_location.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.1/netbox_inventory/templates/netbox_inventory/tabs/located_assets_rack.html` & `netbox-inventory-1.2.2/netbox_inventory/templates/netbox_inventory/tabs/located_assets_rack.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.1/netbox_inventory/templates/netbox_inventory/tabs/located_assets_site.html` & `netbox-inventory-1.2.2/netbox_inventory/templates/netbox_inventory/tabs/located_assets_site.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.1/netbox_inventory/tests/asset/test_api.py` & `netbox-inventory-1.2.2/netbox_inventory/tests/asset/test_api.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.1/netbox_inventory/tests/asset/test_models.py` & `netbox-inventory-1.2.2/netbox_inventory/tests/asset/test_models.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,13 @@
-from copy import deepcopy
-from django.conf import settings
 from django.test import override_settings, TestCase
 
 from dcim.models import Device, DeviceType, DeviceRole, Manufacturer, Site
 from utilities.exceptions import AbortRequest
 from netbox_inventory.models import Asset
-
-
-CONFIG_SYNC_ON = deepcopy(settings.PLUGINS_CONFIG)
-CONFIG_SYNC_ON['netbox_inventory']['sync_hardware_serial_asset_tag']=True
-CONFIG_SYNC_OFF = deepcopy(settings.PLUGINS_CONFIG)
-CONFIG_SYNC_OFF['netbox_inventory']['sync_hardware_serial_asset_tag']=False
+from ..settings import CONFIG_SYNC_OFF, CONFIG_SYNC_ON
 
 
 class TestAssetModel(TestCase):
     def setUp(self):
         self.site1 = Site.objects.create(
             name='site1',
             slug='site1',
```

### Comparing `netbox-inventory-1.2.1/netbox_inventory/tests/asset/test_views.py` & `netbox-inventory-1.2.2/netbox_inventory/tests/asset/test_views.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,17 @@
-from copy import deepcopy
-from django.conf import settings
 from django.contrib.contenttypes.models import ContentType
 from django.test import override_settings
 
 from dcim.models import Manufacturer, DeviceType, DeviceRole, Device, InventoryItem, Module, ModuleBay, ModuleType, Site
 from users.models import ObjectPermission
 from utilities.testing import post_data, ViewTestCases
 
 from netbox_inventory.tests.custom import ModelViewTestCase
 from netbox_inventory.models import Asset, InventoryItemType
-
-
-CONFIG_ALLOW_CREATE_DEVICE_TYPE = deepcopy(settings.PLUGINS_CONFIG)
-CONFIG_ALLOW_CREATE_DEVICE_TYPE['netbox_inventory']['asset_import_create_device_type']=True
+from ..settings import CONFIG_SYNC_ON, CONFIG_ALLOW_CREATE_DEVICE_TYPE
 
 
 class AssetTestCase(
     ModelViewTestCase,
     ViewTestCases.PrimaryObjectViewTestCase,
 ):
 
@@ -78,53 +73,15 @@
             f'{asset3.pk},333,stored',
         )
         cls.bulk_edit_data = {
             'status': 'retired',
         }
 
     @override_settings(EXEMPT_VIEW_PERMISSIONS=['*'])
-    def test_create_devcie_from_asset(self):
-
-        # Assign unconstrained permission
-        obj_perm = ObjectPermission(
-            name='test-device-create permission',
-            actions=['add', 'change']
-        )
-        obj_perm.save()
-        obj_perm.users.add(self.user)
-        obj_perm.object_types.add(ContentType.objects.get_for_model(self.model))
-        obj_perm.object_types.add(ContentType.objects.get_for_model(Device))
-
-        asset = Asset.objects.create(
-            status='stored',
-            serial='123create',
-            device_type=DeviceType.objects.first(),
-        )
-
-        form_data = {
-            'name': 'test-device-create',
-            'device_role': DeviceRole.objects.first(),
-            'device_type': asset.device_type.pk,
-            'serial': asset.serial,
-            'site': Site.objects.first(),
-            'status': 'active',
-        }
-
-        request = {
-            'path': self._get_url('device_create')+f'?asset_id={asset.pk}',
-            'data': post_data(form_data),
-        }
-        self.assertHttpStatus(self.client.post(**request), 302)
-
-        devices = Device.objects.filter(name=form_data['name'])
-        self.assertEqual(len(devices), 1)
-        self.assertEqual(devices.first().assigned_asset, asset)
-
-    @override_settings(EXEMPT_VIEW_PERMISSIONS=['*'])
-    def test_assign_devcie_from_asset(self):
+    def test_assign_device_from_asset(self):
 
         # Assign unconstrained permission
         obj_perm = ObjectPermission(
             name='test-device-assign permission',
             actions=['add', 'change']
         )
         obj_perm.save()
@@ -200,17 +157,17 @@
 
     def _get_url(self, action, instance=None):
         # fix - CreateMultipleObjectsViewTestCase assumes view names contains only 'add' but we need 'bulk_add'
         if action == 'add':
             action = 'bulk_add'
         return super()._get_url(action, instance)
 
-class AssetAssignBase():
+class AssetCreateHwBase():
     """
-    Base class for tests that assign Asset to specific hardware
+    Base class for tests that create hardware and assign Asset to it
     """
 
     def setUp(self):
         super().setUp()
 
         self.site1 = Site.objects.create(
             name='site1',
@@ -246,101 +203,171 @@
             device_role=self.device_role1,
             name='device1',
         )
         self.module_bay1 = ModuleBay.objects.create(
             device=self.device1,
             name='1',
         )
-        self.asset_device = Asset.objects.create(
+        self.asset_device_sn = Asset.objects.create(
             asset_tag='asset_device',
             serial='asset_device',
             status='stored',
             device_type=self.device_type1,
         )
-        self.asset_module = Asset.objects.create(
+        self.asset_module_sn = Asset.objects.create(
             asset_tag='asset_module',
             serial='asset_module',
             status='stored',
             module_type=self.module_type1,
         )
-        self.asset_inventoryitem = Asset.objects.create(
+        self.asset_inventoryitem_sn = Asset.objects.create(
             asset_tag='asset_inventoryitem',
             serial='asset_inventoryitem',
             status='stored',
             inventoryitem_type=self.inventoryitem_type1,
         )
+        self.asset_device_no = Asset.objects.create(
+            status='stored',
+            device_type=self.device_type1,
+        )
+        self.asset_module_no = Asset.objects.create(
+            status='stored',
+            module_type=self.module_type1,
+        )
+        self.asset_inventoryitem_no = Asset.objects.create(
+            status='stored',
+            inventoryitem_type=self.inventoryitem_type1,
+        )
 
     def _get_url(self, _):
         hardware_kind = self.tested_asset.kind
         if hardware_kind == 'inventoryitem':
             hardware_kind = 'inventory-item'
         return f'/plugins/inventory/assets/{hardware_kind}/create/?asset_id={self.tested_asset.pk}'
 
     @override_settings(EXEMPT_VIEW_PERMISSIONS=['*'])
+    @override_settings(PLUGINS_CONFIG=CONFIG_SYNC_ON)
     def test_create_object_with_permission(self):
         super().test_create_object_with_permission()
         # in addition to a new inventoryitem instance in db,
         # it must have matching serial and asset2 must have it assigned
+        # blank value for Asset.serial is None, but for Device/Module/IItem.serial it's ''
+        checked_serial = self.tested_asset.serial or '' 
         instance = self._get_queryset().order_by('pk').last()
-        self.assertEqual(instance.serial, self.tested_asset.serial)
+        self.assertEqual(instance.asset_tag, self.tested_asset.asset_tag)
+        self.assertEqual(instance.serial, checked_serial)
         self.tested_asset.refresh_from_db()
         self.assertEqual(instance, self.tested_asset.hardware)
 
     @override_settings(EXEMPT_VIEW_PERMISSIONS=['*'])
+    @override_settings(PLUGINS_CONFIG=CONFIG_SYNC_ON)
     def test_create_object_with_constrained_permission(self):
         super().test_create_object_with_constrained_permission()
         # in addition to a new inventoryitem instance in db,
         # it must have matching serial and asset2 must have it assigned
+        # blank value for Asset.serial is None, but for Device/Module/IItem.serial it's ''
+        checked_serial = self.tested_asset.serial or '' 
         instance = self._get_queryset().order_by('pk').last()
-        self.assertEqual(instance.serial, self.tested_asset.serial)
+        self.assertEqual(instance.asset_tag, self.tested_asset.asset_tag)
+        self.assertEqual(instance.serial, checked_serial)
         self.tested_asset.refresh_from_db()
         self.assertEqual(instance, self.tested_asset.hardware)
 
 
-class DeviceAssetAssignTestCase(AssetAssignBase, ModelViewTestCase, ViewTestCases.CreateObjectViewTestCase):
+class SerialDeviceAssetCreateHwTestCase(AssetCreateHwBase, ModelViewTestCase, ViewTestCases.CreateObjectViewTestCase):
+    """
+    Test creating new Device from Asset with serial
+    """
+    model = Device
+
+    def setUp(self):
+        super().setUp()
+        self.form_data = {
+            'site': self.site1.pk,
+            'device_type': self.device_type1.pk,
+            'device_role': self.device_role1.pk,
+            'status': 'active',
+            'name': 'tested_device',
+        }
+        self.tested_asset = self.asset_device_sn
+
+
+class SerialModuleAssetCreateHwTestCase(AssetCreateHwBase, ModelViewTestCase, ViewTestCases.CreateObjectViewTestCase):
+    """
+    Test creating new Module from Asset with serial
+    """
+    model = Module
+
+    def setUp(self):
+        super().setUp()
+        self.form_data = {
+            'device': self.device1.pk,
+            'module_bay': self.module_bay1.pk,
+            'module_type': self.module_type1.pk,
+            'status': 'active',
+        }
+        self.tested_asset = self.asset_module_sn
+
+
+class SerialInventoryItemAssetCreateHwTestCase(AssetCreateHwBase, ModelViewTestCase, ViewTestCases.CreateObjectViewTestCase):
+    """
+    Test creating new InventoryItem from Asset with serial
+    """
+    model = InventoryItem
+
+    def setUp(self):
+        super().setUp()
+        self.form_data = {
+            'device': self.device1.pk,
+            'name': 'inventoryitem1',
+        }
+        self.tested_asset = self.asset_inventoryitem_sn
+
+
+class NoSerialDeviceAssetCreateHwTestCase(AssetCreateHwBase, ModelViewTestCase, ViewTestCases.CreateObjectViewTestCase):
     """
-    Test creating new Device from Asset
+    Test creating new Device from Asset with blank serial
     """
     model = Device
 
     def setUp(self):
         super().setUp()
         self.form_data = {
             'site': self.site1.pk,
             'device_type': self.device_type1.pk,
             'device_role': self.device_role1.pk,
             'status': 'active',
             'name': 'tested_device',
         }
-        self.tested_asset = self.asset_device
+        self.tested_asset = self.asset_device_no
 
 
-class ModuleAssetAssignTestCase(AssetAssignBase, ModelViewTestCase, ViewTestCases.CreateObjectViewTestCase):
+class NoSerialModuleAssetCreateHwTestCase(AssetCreateHwBase, ModelViewTestCase, ViewTestCases.CreateObjectViewTestCase):
     """
-    Test creating new Module from Asset
+    Test creating new Module from Asset with blank serial
     """
     model = Module
 
     def setUp(self):
         super().setUp()
         self.form_data = {
             'device': self.device1.pk,
             'module_bay': self.module_bay1.pk,
             'module_type': self.module_type1.pk,
             'status': 'active',
         }
-        self.tested_asset = self.asset_module
+        self.tested_asset = self.asset_module_no
 
 
-class InventoryItemAssetAssignTestCase(AssetAssignBase, ModelViewTestCase, ViewTestCases.CreateObjectViewTestCase):
+class NoSerialInventoryItemAssetCreateHwTestCase(AssetCreateHwBase, ModelViewTestCase, ViewTestCases.CreateObjectViewTestCase):
     """
-    Test creating new InventoryItem from Asset
+    Test creating new InventoryItem from Asset with blank serial
     """
     model = InventoryItem
 
     def setUp(self):
         super().setUp()
         self.form_data = {
             'device': self.device1.pk,
             'name': 'inventoryitem1',
         }
-        self.tested_asset = self.asset_inventoryitem
+        self.tested_asset = self.asset_inventoryitem_no
```

### Comparing `netbox-inventory-1.2.1/netbox_inventory/tests/custom.py` & `netbox-inventory-1.2.2/netbox_inventory/tests/custom.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.1/netbox_inventory/tests/inventoryitem_group/test_api.py` & `netbox-inventory-1.2.2/netbox_inventory/tests/inventoryitem_group/test_api.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.1/netbox_inventory/tests/inventoryitem_group/test_views.py` & `netbox-inventory-1.2.2/netbox_inventory/tests/inventoryitem_group/test_views.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.1/netbox_inventory/tests/inventoryitem_type/test_api.py` & `netbox-inventory-1.2.2/netbox_inventory/tests/inventoryitem_type/test_api.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.1/netbox_inventory/tests/inventoryitem_type/test_views.py` & `netbox-inventory-1.2.2/netbox_inventory/tests/inventoryitem_type/test_views.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.1/netbox_inventory/tests/purchase/test_api.py` & `netbox-inventory-1.2.2/netbox_inventory/tests/purchase/test_api.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.1/netbox_inventory/tests/purchase/test_views.py` & `netbox-inventory-1.2.2/netbox_inventory/tests/purchase/test_views.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.1/netbox_inventory/tests/supplier/test_api.py` & `netbox-inventory-1.2.2/netbox_inventory/tests/supplier/test_api.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.1/netbox_inventory/tests/supplier/test_views.py` & `netbox-inventory-1.2.2/netbox_inventory/tests/supplier/test_views.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.1/netbox_inventory/tests/test_load.py` & `netbox-inventory-1.2.2/netbox_inventory/tests/test_load.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 class NetboxDnsVersionTestCase(SimpleTestCase):
     """
     Test for netbox_inventory package
     """
 
     def test_version(self):
-        assert __version__ == "1.2.1"
+        assert __version__ == "1.2.2"
 
 
 class AppTest(APITestCase):
     """
     Test the availability of the plugin API root
     """
```

### Comparing `netbox-inventory-1.2.1/netbox_inventory/urls.py` & `netbox-inventory-1.2.2/netbox_inventory/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.1/netbox_inventory/utils.py` & `netbox-inventory-1.2.2/netbox_inventory/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -99,14 +99,21 @@
     old_hw.asset_tag = None
     old_hw.save()
     pre_save.connect(prevent_update_serial_asset_tag, sender=Device)
     pre_save.connect(prevent_update_serial_asset_tag, sender=Module)
     pre_save.connect(prevent_update_serial_asset_tag, sender=InventoryItem)
 
 
+def is_equal_none(a, b):
+    """ Compare a and b as string. None is considered the same as empty string. """
+    if a is None or b is None:
+        return a == b or a == '' or b == ''
+    return a == b
+
+
 def query_located(queryset, field_name, values, assets_shown='all'):
     """
     Filters queryset on located values. Can filter for installed
     location/site and/or stored location/site for assets makred as stored.
     Args:
         * queryset - queryset of Asset model
         * field_name - 'site' or 'location' or 'rack'
```

### Comparing `netbox-inventory-1.2.1/netbox_inventory/views/asset.py` & `netbox-inventory-1.2.2/netbox_inventory/views/asset.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.1/netbox_inventory/views/asset_assign.py` & `netbox-inventory-1.2.2/netbox_inventory/views/asset_assign.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.1/netbox_inventory/views/asset_create.py` & `netbox-inventory-1.2.2/netbox_inventory/views/asset_create.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.1/netbox_inventory/views/inventoryitem_group.py` & `netbox-inventory-1.2.2/netbox_inventory/views/inventoryitem_group.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.1/netbox_inventory/views/inventoryitem_type.py` & `netbox-inventory-1.2.2/netbox_inventory/views/inventoryitem_type.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.1/netbox_inventory/views/purchase.py` & `netbox-inventory-1.2.2/netbox_inventory/views/purchase.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.1/netbox_inventory/views/supplier.py` & `netbox-inventory-1.2.2/netbox_inventory/views/supplier.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.1/netbox_inventory/views/tabs.py` & `netbox-inventory-1.2.2/netbox_inventory/views/tabs.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.1/netbox_inventory.egg-info/PKG-INFO` & `netbox-inventory-1.2.2/netbox_inventory.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-inventory
-Version: 1.2.1
+Version: 1.2.2
 Summary: Inventory asset management in NetBox
 Author-email: Matej Vadnjal <matej.vadnjal@arnes.si>
 Project-URL: Homepage, https://github.com/ArnesSI/netbox-inventory/
 Project-URL: Bug Tracker, https://github.com/ArnesSI/netbox-inventory/issues/
 Keywords: netbox,netbox-plugin,inventory
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -130,24 +130,24 @@
 ```python
 PLUGINS = [
     'netbox_inventory'
 ]
 
 PLUGINS_CONFIG = {
     "netbox_inventory": {
-        # Example settings below
+        # Example settings below, see "Available settings"
+        # in README.md for all possible settings
         "used_status_name": "used",
         "stored_status_name": "stored",
-        "sync_serial_number": True,
-        "sync_asset_tag": True,
+        "sync_hardware_serial_asset_tag": True,
     },
 }
 ```
 
-Available settings:
+#### Available settings
 
 | Setting | Default value | Description |
 |---------|---------------|-------------|
 | `top_level_menu` | `True`| Add netbox-inventory to the top level of netbox navigation menu under Inventory heading. If set to False the plugin will add a menu item under the Plugins menu item. This setting is only valid under netbox v3.4 and newer.
 | `used_status_name` | `'used'`| Status that indicates asset is in use. See "Automatic management of asset status" below for more info on this setting.
 | `stored_status_name` | `'stored'`| Status that indicates asset is in storage. See "Automatic management of asset status" below for more info on this setting.
 | `sync_hardware_serial_asset_tag` | `False` | When an asset is assigned or unassigned to a device, module or inventory item, update its serial number and asset tag to be in sync with the asset? |
```

### Comparing `netbox-inventory-1.2.1/netbox_inventory.egg-info/SOURCES.txt` & `netbox-inventory-1.2.2/netbox_inventory.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 netbox_inventory/templates/netbox_inventory/inc/asset_warranty.html
 netbox_inventory/templates/netbox_inventory/tabs/located_assets_base.html
 netbox_inventory/templates/netbox_inventory/tabs/located_assets_location.html
 netbox_inventory/templates/netbox_inventory/tabs/located_assets_rack.html
 netbox_inventory/templates/netbox_inventory/tabs/located_assets_site.html
 netbox_inventory/tests/__init__.py
 netbox_inventory/tests/custom.py
+netbox_inventory/tests/settings.py
 netbox_inventory/tests/test_load.py
 netbox_inventory/tests/asset/__init__.py
 netbox_inventory/tests/asset/test_api.py
 netbox_inventory/tests/asset/test_models.py
 netbox_inventory/tests/asset/test_views.py
 netbox_inventory/tests/inventoryitem_group/__init__.py
 netbox_inventory/tests/inventoryitem_group/test_api.py
```

### Comparing `netbox-inventory-1.2.1/pyproject.toml` & `netbox-inventory-1.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "netbox-inventory"
-version = "1.2.1"
+version = "1.2.2"
 authors = [
   { name="Matej Vadnjal", email="matej.vadnjal@arnes.si" },
 ]
 description = "Inventory asset management in NetBox"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

