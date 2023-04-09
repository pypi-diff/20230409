# Comparing `tmp/npm-cockpit-0.2.1.tar.gz` & `tmp/npm-cockpit-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "npm-cockpit-0.2.1.tar", max compression
+gzip compressed data, was "npm-cockpit-0.3.0.tar", max compression
```

## Comparing `npm-cockpit-0.2.1.tar` & `npm-cockpit-0.3.0.tar`

### file list

```diff
@@ -1,91 +1,92 @@
--rw-r--r--   0        0        0     1860 2023-02-27 01:00:34.610513 npm-cockpit-0.2.1/README.md
--rw-r--r--   0        0        0      604 2023-02-27 11:26:37.731911 npm-cockpit-0.2.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-26 14:59:11.224512 npm-cockpit-0.2.1/src/__init__.py
--rw-r--r--   0        0        0     2348 2023-02-26 19:56:00.838209 npm-cockpit-0.2.1/src/app/Router.py
--rw-r--r--   0        0        0      885 2023-02-26 19:56:00.837694 npm-cockpit-0.2.1/src/app/Server.py
--rw-r--r--   0        0        0        0 2023-02-26 13:42:47.729827 npm-cockpit-0.2.1/src/app/__init__.py
--rw-r--r--   0        0        0      916 2023-02-26 19:56:00.829137 npm-cockpit-0.2.1/src/app/app.py
--rw-r--r--   0        0        0      259 2023-01-29 18:17:06.428278 npm-cockpit-0.2.1/src/app/classes/Error.py
--rw-r--r--   0        0        0     1686 2023-02-26 19:56:00.842717 npm-cockpit-0.2.1/src/app/classes/Lib.py
--rw-r--r--   0        0        0      175 2022-11-13 16:04:48.852302 npm-cockpit-0.2.1/src/app/classes/Response.py
--rw-r--r--   0        0        0        0 2022-11-19 18:26:01.953795 npm-cockpit-0.2.1/src/app/classes/Semver.py
--rw-r--r--   0        0        0        0 2022-08-20 11:23:10.007859 npm-cockpit-0.2.1/src/app/classes/__init__.py
--rw-r--r--   0        0        0        0 2022-12-08 23:03:40.836734 npm-cockpit-0.2.1/src/app/data/__init__.py
--rw-r--r--   0        0        0     4185 2023-02-26 19:56:00.842660 npm-cockpit-0.2.1/src/app/data/dependencies.py
--rw-r--r--   0        0        0     1120 2023-02-26 19:56:00.838547 npm-cockpit-0.2.1/src/app/data/deprecated.py
--rw-r--r--   0        0        0      202 2023-02-26 19:56:00.837944 npm-cockpit-0.2.1/src/app/data/package.py
--rw-r--r--   0        0        0      797 2023-02-26 19:56:00.842548 npm-cockpit-0.2.1/src/app/data/updates.py
--rw-r--r--   0        0        0      890 2023-02-26 19:56:00.838271 npm-cockpit-0.2.1/src/app/data/vulnerabilities.py
--rw-r--r--   0        0        0      800 2023-02-12 00:31:18.831583 npm-cockpit-0.2.1/src/app/path.py
--rw-r--r--   0        0        0      831 2023-02-25 17:34:17.689110 npm-cockpit-0.2.1/src/app/utils.py
--rw-r--r--   0        0        0      739 2023-02-26 13:42:47.732704 npm-cockpit-0.2.1/src/client/css/colors.css
--rw-r--r--   0        0        0     3919 2023-02-26 13:42:47.733919 npm-cockpit-0.2.1/src/client/css/styles.classes.css
--rw-r--r--   0        0        0     6144 2023-02-26 13:42:47.734310 npm-cockpit-0.2.1/src/client/css/styles.components.css
--rw-r--r--   0        0        0      670 2023-02-26 13:42:47.734378 npm-cockpit-0.2.1/src/client/css/styles.ids.css
--rw-r--r--   0        0        0     1579 2023-02-26 13:42:47.734722 npm-cockpit-0.2.1/src/client/css/styles.main.css
--rw-r--r--   0        0        0    15406 2023-02-26 13:42:47.734797 npm-cockpit-0.2.1/src/client/favicon.ico
--rw-r--r--   0        0        0   126616 2023-02-26 13:42:47.736223 npm-cockpit-0.2.1/src/client/font/Arimo-Bold.woff2
--rw-r--r--   0        0        0   126592 2023-02-26 13:42:47.736840 npm-cockpit-0.2.1/src/client/font/Arimo-Regular.woff2
--rw-r--r--   0        0        0   135036 2023-02-26 13:42:47.737650 npm-cockpit-0.2.1/src/client/font/Arimo-SemiBold.woff2
--rw-r--r--   0        0        0     1910 2023-02-26 13:42:47.738207 npm-cockpit-0.2.1/src/client/index.html
--rw-r--r--   0        0        0     2966 2023-02-26 13:42:47.739076 npm-cockpit-0.2.1/src/client/js/components/dashboard.js
--rw-r--r--   0        0        0     2673 2023-02-26 13:42:47.739757 npm-cockpit-0.2.1/src/client/js/components/elements/dependency-filter.js
--rw-r--r--   0        0        0      756 2023-02-26 13:42:47.739956 npm-cockpit-0.2.1/src/client/js/components/elements/dependency-info.js
--rw-r--r--   0        0        0     3679 2023-02-26 13:42:47.740033 npm-cockpit-0.2.1/src/client/js/components/elements/dependency-item.js
--rw-r--r--   0        0        0      155 2023-02-26 13:42:47.740087 npm-cockpit-0.2.1/src/client/js/components/elements/dependency-version.js
--rw-r--r--   0        0        0      342 2023-02-26 13:42:47.740144 npm-cockpit-0.2.1/src/client/js/components/elements/icon.js
--rw-r--r--   0        0        0      233 2023-02-26 13:42:47.740198 npm-cockpit-0.2.1/src/client/js/components/elements/index.js
--rw-r--r--   0        0        0     2071 2023-02-26 13:42:47.740254 npm-cockpit-0.2.1/src/client/js/components/elements/select.js
--rw-r--r--   0        0        0     1985 2023-02-26 13:42:47.740310 npm-cockpit-0.2.1/src/client/js/components/elements/table.js
--rw-r--r--   0        0        0     2278 2023-02-26 13:42:47.740366 npm-cockpit-0.2.1/src/client/js/components/index.js
--rw-r--r--   0        0        0     2416 2023-02-26 13:42:47.740842 npm-cockpit-0.2.1/src/client/js/components/items/Item.js
--rw-r--r--   0        0        0     3561 2023-02-26 13:42:47.741050 npm-cockpit-0.2.1/src/client/js/components/items/basic-info.js
--rw-r--r--   0        0        0     3100 2023-02-26 13:42:47.741391 npm-cockpit-0.2.1/src/client/js/components/items/dependencies-list.js
--rw-r--r--   0        0        0     1545 2023-02-26 13:42:47.741870 npm-cockpit-0.2.1/src/client/js/components/items/dependencies-network.js
--rw-r--r--   0        0        0     2446 2023-02-26 13:42:47.742267 npm-cockpit-0.2.1/src/client/js/components/items/dependencies-tree.js
--rw-r--r--   0        0        0     1319 2023-02-26 13:42:47.742462 npm-cockpit-0.2.1/src/client/js/components/items/deprecated-table.js
--rw-r--r--   0        0        0      861 2023-02-26 13:42:47.743010 npm-cockpit-0.2.1/src/client/js/components/items/frequency.js
--rw-r--r--   0        0        0      665 2023-02-26 13:42:47.743093 npm-cockpit-0.2.1/src/client/js/components/items/index.js
--rw-r--r--   0        0        0      877 2023-02-26 13:42:47.743168 npm-cockpit-0.2.1/src/client/js/components/items/issues-table.js
--rw-r--r--   0        0        0     1362 2023-02-26 13:42:47.743234 npm-cockpit-0.2.1/src/client/js/components/items/package-data.js
--rw-r--r--   0        0        0     2871 2023-02-26 13:42:47.743307 npm-cockpit-0.2.1/src/client/js/components/items/updates-table.js
--rw-r--r--   0        0        0     1199 2023-02-26 13:42:47.743625 npm-cockpit-0.2.1/src/client/js/components/items/updates.js
--rw-r--r--   0        0        0     2962 2023-02-26 13:42:47.743722 npm-cockpit-0.2.1/src/client/js/components/items/vulnerabilities-table.js
--rw-r--r--   0        0        0     1031 2023-02-26 13:42:47.744084 npm-cockpit-0.2.1/src/client/js/components/items/vulnerabilities.js
--rw-r--r--   0        0        0      849 2023-02-26 13:42:47.744457 npm-cockpit-0.2.1/src/client/js/components/items/weight.js
--rw-r--r--   0        0        0      420 2023-02-26 13:42:47.744647 npm-cockpit-0.2.1/src/client/js/components/popups/Popup.js
--rw-r--r--   0        0        0      791 2023-02-26 13:42:47.744717 npm-cockpit-0.2.1/src/client/js/components/popups/group-data.js
--rw-r--r--   0        0        0      152 2023-02-26 13:42:47.744782 npm-cockpit-0.2.1/src/client/js/components/popups/index.js
--rw-r--r--   0        0        0     2686 2023-02-26 13:42:47.744850 npm-cockpit-0.2.1/src/client/js/components/popups/module-data.js
--rw-r--r--   0        0        0     3898 2023-02-26 13:42:47.745492 npm-cockpit-0.2.1/src/client/js/components/popups/section-info.js
--rw-r--r--   0        0        0     1682 2023-02-26 13:42:47.744534 npm-cockpit-0.2.1/src/client/js/components/popups.js
--rw-r--r--   0        0        0      369 2023-02-26 13:42:47.745562 npm-cockpit-0.2.1/src/client/js/components/widget.js
--rw-r--r--   0        0        0      336 2023-02-26 13:42:47.745624 npm-cockpit-0.2.1/src/client/js/index.js
--rw-r--r--   0        0        0   273912 2023-02-26 13:42:47.747951 npm-cockpit-0.2.1/src/client/js/lib/d3.min.js
--rw-r--r--   0        0        0     2846 2023-02-26 13:42:47.748466 npm-cockpit-0.2.1/src/client/js/plots/bar.js
--rw-r--r--   0        0        0     6384 2023-02-26 13:42:47.748793 npm-cockpit-0.2.1/src/client/js/plots/dependencies-network.js
--rw-r--r--   0        0        0     3833 2023-02-26 13:42:47.749101 npm-cockpit-0.2.1/src/client/js/plots/dependencies-tree.js
--rw-r--r--   0        0        0     2145 2023-02-26 13:42:47.749326 npm-cockpit-0.2.1/src/client/js/plots/donut.js
--rw-r--r--   0        0        0      171 2023-02-26 13:42:47.749419 npm-cockpit-0.2.1/src/client/js/plots/utils.js
--rw-r--r--   0        0        0      388 2023-02-26 13:42:47.749646 npm-cockpit-0.2.1/src/client/js/utils.js
--rw-r--r--   0        0        0      689 2023-02-26 13:42:47.749732 npm-cockpit-0.2.1/src/client/js/workers/dependenciesList.js
--rw-r--r--   0        0        0     2216 2023-02-26 13:42:47.749824 npm-cockpit-0.2.1/src/client/js/workers/dependenciesNetwork.js
--rw-r--r--   0        0        0     2479 2023-02-26 13:42:47.749948 npm-cockpit-0.2.1/src/client/js/workers/dependenciesTree.js
--rw-r--r--   0        0        0      906 2023-02-26 13:42:47.750010 npm-cockpit-0.2.1/src/client/js/workers/frequency.js
--rw-r--r--   0        0        0      268 2023-02-26 13:42:47.750063 npm-cockpit-0.2.1/src/client/js/workers/issuesTable.js
--rw-r--r--   0        0        0      700 2023-02-26 13:42:47.750115 npm-cockpit-0.2.1/src/client/js/workers/updates.js
--rw-r--r--   0        0        0      829 2023-02-26 13:42:47.750168 npm-cockpit-0.2.1/src/client/js/workers/updatesTable.js
--rw-r--r--   0        0        0      341 2023-02-26 13:42:47.750220 npm-cockpit-0.2.1/src/client/js/workers/vulnerabilitiesTable.js
--rw-r--r--   0        0        0     1066 2023-02-26 13:42:47.750777 npm-cockpit-0.2.1/src/client/js/workers/weight.js
--rw-r--r--   0        0        0     2593 2023-02-26 13:42:47.751363 npm-cockpit-0.2.1/src/client/layout.json
--rw-r--r--   0        0        0     1025 2023-02-26 13:42:47.751606 npm-cockpit-0.2.1/src/client/static/clear-icon.svg
--rw-r--r--   0        0        0      668 2023-02-26 13:42:47.751699 npm-cockpit-0.2.1/src/client/static/dep-icon.svg
--rw-r--r--   0        0        0      325 2023-02-26 13:42:47.751770 npm-cockpit-0.2.1/src/client/static/info-icon.svg
--rw-r--r--   0        0        0     3649 2023-02-26 13:42:47.751832 npm-cockpit-0.2.1/src/client/static/loading.svg
--rw-r--r--   0        0        0     2103 2023-02-26 13:42:47.751906 npm-cockpit-0.2.1/src/client/static/net-icon.svg
--rw-r--r--   0        0        0        0 2023-02-26 13:42:47.751932 npm-cockpit-0.2.1/src/client/static/theme-icon.svg
--rw-r--r--   0        0        0     1643 2023-02-26 13:42:47.751993 npm-cockpit-0.2.1/src/client/static/tree-icon.svg
--rw-r--r--   0        0        0      402 2023-02-26 13:42:47.752045 npm-cockpit-0.2.1/src/client/static/update-icon.svg
--rw-r--r--   0        0        0      733 2023-02-26 13:42:47.752095 npm-cockpit-0.2.1/src/client/static/vuln-icon.svg
--rw-r--r--   0        0        0     3146 1970-01-01 00:00:00.000000 npm-cockpit-0.2.1/setup.py
--rw-r--r--   0        0        0     2578 1970-01-01 00:00:00.000000 npm-cockpit-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1857 2023-04-09 16:22:23.818755 npm-cockpit-0.3.0/README.md
+-rw-r--r--   0        0        0      604 2023-04-09 16:22:23.818755 npm-cockpit-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-13 15:18:57.374789 npm-cockpit-0.3.0/src/__init__.py
+-rw-r--r--   0        0        0     2348 2023-03-13 15:18:57.374789 npm-cockpit-0.3.0/src/app/Router.py
+-rw-r--r--   0        0        0      885 2023-03-13 15:18:57.374789 npm-cockpit-0.3.0/src/app/Server.py
+-rw-r--r--   0        0        0        0 2023-03-13 15:18:57.374789 npm-cockpit-0.3.0/src/app/__init__.py
+-rw-r--r--   0        0        0      916 2023-03-13 15:18:57.374789 npm-cockpit-0.3.0/src/app/app.py
+-rw-r--r--   0        0        0      259 2023-03-13 15:18:57.374789 npm-cockpit-0.3.0/src/app/classes/Error.py
+-rw-r--r--   0        0        0     1686 2023-03-13 15:18:57.374789 npm-cockpit-0.3.0/src/app/classes/Lib.py
+-rw-r--r--   0        0        0      175 2023-03-13 15:18:57.374789 npm-cockpit-0.3.0/src/app/classes/Response.py
+-rw-r--r--   0        0        0        0 2023-03-13 15:18:57.374789 npm-cockpit-0.3.0/src/app/classes/Semver.py
+-rw-r--r--   0        0        0        0 2023-03-13 15:18:57.374789 npm-cockpit-0.3.0/src/app/classes/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-13 15:18:57.374789 npm-cockpit-0.3.0/src/app/data/__init__.py
+-rw-r--r--   0        0        0     4185 2023-03-13 15:18:57.374789 npm-cockpit-0.3.0/src/app/data/dependencies.py
+-rw-r--r--   0        0        0     1120 2023-03-13 15:18:57.374789 npm-cockpit-0.3.0/src/app/data/deprecated.py
+-rw-r--r--   0        0        0      202 2023-03-13 15:18:57.374789 npm-cockpit-0.3.0/src/app/data/package.py
+-rw-r--r--   0        0        0      797 2023-03-13 15:18:57.374789 npm-cockpit-0.3.0/src/app/data/updates.py
+-rw-r--r--   0        0        0      890 2023-03-13 15:18:57.374789 npm-cockpit-0.3.0/src/app/data/vulnerabilities.py
+-rw-r--r--   0        0        0     1068 2023-04-09 16:22:23.818755 npm-cockpit-0.3.0/src/app/path.py
+-rw-r--r--   0        0        0      831 2023-03-13 15:18:57.374789 npm-cockpit-0.3.0/src/app/utils.py
+-rw-r--r--   0        0        0      739 2023-03-13 15:18:57.374789 npm-cockpit-0.3.0/src/client/css/colors.css
+-rw-r--r--   0        0        0     3919 2023-03-13 15:18:57.374789 npm-cockpit-0.3.0/src/client/css/styles.classes.css
+-rw-r--r--   0        0        0     6144 2023-03-13 15:18:57.374789 npm-cockpit-0.3.0/src/client/css/styles.components.css
+-rw-r--r--   0        0        0      738 2023-04-09 16:22:23.818755 npm-cockpit-0.3.0/src/client/css/styles.ids.css
+-rw-r--r--   0        0        0     1579 2023-03-13 15:18:57.374789 npm-cockpit-0.3.0/src/client/css/styles.main.css
+-rw-r--r--   0        0        0    15406 2023-03-13 15:18:57.374789 npm-cockpit-0.3.0/src/client/favicon.ico
+-rw-r--r--   0        0        0   126616 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/font/Arimo-Bold.woff2
+-rw-r--r--   0        0        0   126592 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/font/Arimo-Regular.woff2
+-rw-r--r--   0        0        0   135036 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/font/Arimo-SemiBold.woff2
+-rw-r--r--   0        0        0     1910 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/index.html
+-rw-r--r--   0        0        0     2966 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/components/dashboard.js
+-rw-r--r--   0        0        0     2673 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/components/elements/dependency-filter.js
+-rw-r--r--   0        0        0      756 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/components/elements/dependency-info.js
+-rw-r--r--   0        0        0     3679 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/components/elements/dependency-item.js
+-rw-r--r--   0        0        0      155 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/components/elements/dependency-version.js
+-rw-r--r--   0        0        0      342 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/components/elements/icon.js
+-rw-r--r--   0        0        0      233 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/components/elements/index.js
+-rw-r--r--   0        0        0     2071 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/components/elements/select.js
+-rw-r--r--   0        0        0     1985 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/components/elements/table.js
+-rw-r--r--   0        0        0     2278 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/components/index.js
+-rw-r--r--   0        0        0     2416 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/components/items/Item.js
+-rw-r--r--   0        0        0     3973 2023-04-09 16:22:23.818755 npm-cockpit-0.3.0/src/client/js/components/items/basic-info.js
+-rw-r--r--   0        0        0     3100 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/components/items/dependencies-list.js
+-rw-r--r--   0        0        0     1545 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/components/items/dependencies-network.js
+-rw-r--r--   0        0        0     2446 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/components/items/dependencies-tree.js
+-rw-r--r--   0        0        0     1319 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/components/items/deprecated-table.js
+-rw-r--r--   0        0        0      861 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/components/items/frequency.js
+-rw-r--r--   0        0        0      665 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/components/items/index.js
+-rw-r--r--   0        0        0      877 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/components/items/issues-table.js
+-rw-r--r--   0        0        0     1362 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/components/items/package-data.js
+-rw-r--r--   0        0        0     2871 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/components/items/updates-table.js
+-rw-r--r--   0        0        0     1199 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/components/items/updates.js
+-rw-r--r--   0        0        0     2962 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/components/items/vulnerabilities-table.js
+-rw-r--r--   0        0        0     1031 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/components/items/vulnerabilities.js
+-rw-r--r--   0        0        0      849 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/components/items/weight.js
+-rw-r--r--   0        0        0      420 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/components/popups/Popup.js
+-rw-r--r--   0        0        0      791 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/components/popups/group-data.js
+-rw-r--r--   0        0        0      152 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/components/popups/index.js
+-rw-r--r--   0        0        0     2686 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/components/popups/module-data.js
+-rw-r--r--   0        0        0     3898 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/components/popups/section-info.js
+-rw-r--r--   0        0        0     1682 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/components/popups.js
+-rw-r--r--   0        0        0      369 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/components/widget.js
+-rw-r--r--   0        0        0      336 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/index.js
+-rw-r--r--   0        0        0   273912 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/lib/d3.min.js
+-rw-r--r--   0        0        0     2846 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/plots/bar.js
+-rw-r--r--   0        0        0     6813 2023-04-09 16:22:23.822756 npm-cockpit-0.3.0/src/client/js/plots/dependencies-network.js
+-rw-r--r--   0        0        0     4261 2023-04-09 16:22:23.822756 npm-cockpit-0.3.0/src/client/js/plots/dependencies-tree.js
+-rw-r--r--   0        0        0     2145 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/plots/donut.js
+-rw-r--r--   0        0        0      171 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/plots/utils.js
+-rw-r--r--   0        0        0      388 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/utils.js
+-rw-r--r--   0        0        0      689 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/workers/dependenciesList.js
+-rw-r--r--   0        0        0     2216 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/workers/dependenciesNetwork.js
+-rw-r--r--   0        0        0     2479 2023-03-13 15:18:57.382789 npm-cockpit-0.3.0/src/client/js/workers/dependenciesTree.js
+-rw-r--r--   0        0        0      906 2023-03-13 15:18:57.382789 npm-cockpit-0.3.0/src/client/js/workers/frequency.js
+-rw-r--r--   0        0        0      268 2023-03-13 15:18:57.382789 npm-cockpit-0.3.0/src/client/js/workers/issuesTable.js
+-rw-r--r--   0        0        0      700 2023-03-13 15:18:57.382789 npm-cockpit-0.3.0/src/client/js/workers/updates.js
+-rw-r--r--   0        0        0      829 2023-03-13 15:18:57.382789 npm-cockpit-0.3.0/src/client/js/workers/updatesTable.js
+-rw-r--r--   0        0        0      341 2023-03-13 15:18:57.382789 npm-cockpit-0.3.0/src/client/js/workers/vulnerabilitiesTable.js
+-rw-r--r--   0        0        0     1089 2023-04-09 16:22:23.822756 npm-cockpit-0.3.0/src/client/js/workers/weight.js
+-rw-r--r--   0        0        0     2593 2023-03-13 15:18:57.382789 npm-cockpit-0.3.0/src/client/layout.json
+-rw-r--r--   0        0        0     1207 2023-04-09 16:22:23.822756 npm-cockpit-0.3.0/src/client/static/center-icon.svg
+-rw-r--r--   0        0        0     1025 2023-03-13 15:18:57.382789 npm-cockpit-0.3.0/src/client/static/clear-icon.svg
+-rw-r--r--   0        0        0      668 2023-03-13 15:18:57.382789 npm-cockpit-0.3.0/src/client/static/dep-icon.svg
+-rw-r--r--   0        0        0      325 2023-03-13 15:18:57.382789 npm-cockpit-0.3.0/src/client/static/info-icon.svg
+-rw-r--r--   0        0        0     3649 2023-03-13 15:18:57.382789 npm-cockpit-0.3.0/src/client/static/loading.svg
+-rw-r--r--   0        0        0     2103 2023-03-13 15:18:57.382789 npm-cockpit-0.3.0/src/client/static/net-icon.svg
+-rw-r--r--   0        0        0        0 2023-03-13 15:18:57.382789 npm-cockpit-0.3.0/src/client/static/theme-icon.svg
+-rw-r--r--   0        0        0     1643 2023-03-13 15:18:57.382789 npm-cockpit-0.3.0/src/client/static/tree-icon.svg
+-rw-r--r--   0        0        0      402 2023-03-13 15:18:57.382789 npm-cockpit-0.3.0/src/client/static/update-icon.svg
+-rw-r--r--   0        0        0      733 2023-03-13 15:18:57.382789 npm-cockpit-0.3.0/src/client/static/vuln-icon.svg
+-rw-r--r--   0        0        0     3137 2023-04-09 16:27:16.643936 npm-cockpit-0.3.0/setup.py
+-rw-r--r--   0        0        0     2575 2023-04-09 16:27:16.644183 npm-cockpit-0.3.0/PKG-INFO
```

### Comparing `npm-cockpit-0.2.1/README.md` & `npm-cockpit-0.3.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 ## Requirements
 
 ### General
 - Terminal or command prompt access
 - Target application folder should contain node_modules folder with installed dependencies and package.json
 - Node.js and NPM installed
 
-### As an NPM package
+### As NPM package
 - `python` command should be available
 
 ## Usage
 
 ### Command params
 
 `path` - a path to project folder with package.json and node_modules inside
```

### Comparing `npm-cockpit-0.2.1/pyproject.toml` & `npm-cockpit-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "npm-cockpit"
-version = "0.2.1"
+version = "0.3.0"
 description = "Installable command-line tool with web interface which helps to track nodejs project dependencies state"
 authors = ["Alex Chirkin <hello@alexchirkin.me>"]
 readme = "README.md"
 packages = [{include = "src"}]
 keywords=[
   "command",
   "dashboard",
```

### Comparing `npm-cockpit-0.2.1/src/app/Router.py` & `npm-cockpit-0.3.0/src/app/Router.py`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.2.1/src/app/Server.py` & `npm-cockpit-0.3.0/src/app/Server.py`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.2.1/src/app/app.py` & `npm-cockpit-0.3.0/src/app/app.py`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.2.1/src/app/classes/Lib.py` & `npm-cockpit-0.3.0/src/app/classes/Lib.py`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.2.1/src/app/data/dependencies.py` & `npm-cockpit-0.3.0/src/app/data/dependencies.py`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.2.1/src/app/data/deprecated.py` & `npm-cockpit-0.3.0/src/app/data/deprecated.py`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.2.1/src/app/data/updates.py` & `npm-cockpit-0.3.0/src/app/data/updates.py`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.2.1/src/app/data/vulnerabilities.py` & `npm-cockpit-0.3.0/src/app/data/vulnerabilities.py`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.2.1/src/app/path.py` & `npm-cockpit-0.3.0/src/app/path.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,26 +5,30 @@
   sys.argv[1]
 except:
   print('ERROR: Please, provide the path to folder with package.json and node_modules', flush=True)
   exit()
 
 path = sys.argv[1]
 package_json_path = path + '/package.json'
+package_lock_path = path + '/package-lock.json'
 node_modules_path = path + '/node_modules'
 
-isfolder = os.path.isdir(node_modules_path)
-isfile = os.path.isfile(package_json_path)
+isNodeModulesFound = os.path.isdir(node_modules_path)
+isPackageJSONFound = os.path.isfile(package_json_path)
+isPackageLockFound = os.path.isfile(package_lock_path)
 
 # provided path validation
-if not(isfile):
+if not(isPackageJSONFound):
   print('ERROR: Target folder should contain package.json file', flush=True)
   exit()
-if not(isfolder):
+if not(isNodeModulesFound):
   print('ERROR: Target folder should contain node_modules folder', flush=True)
   exit()
+if not(isPackageLockFound):
+  print('WARNING: package-lock.json not found, cannot get vulnerabilities info', flush=True)
 
 def get_path():
   global path
   return path
 
 def get_package_json_path():
   global package_json_path
```

### Comparing `npm-cockpit-0.2.1/src/app/utils.py` & `npm-cockpit-0.3.0/src/app/utils.py`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.2.1/src/client/css/colors.css` & `npm-cockpit-0.3.0/src/client/css/colors.css`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.2.1/src/client/css/styles.classes.css` & `npm-cockpit-0.3.0/src/client/css/styles.classes.css`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.2.1/src/client/css/styles.components.css` & `npm-cockpit-0.3.0/src/client/css/styles.components.css`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.2.1/src/client/css/styles.ids.css` & `npm-cockpit-0.3.0/src/client/css/styles.ids.css`

 * *Files 23% similar despite different names*

```diff
@@ -36,8 +36,14 @@
 }
 
 #layout-message {
   position: absolute;
   top: 50%;
   left: 50%;
   transform: translate(-50%, -50%);
+}
+
+#center-icon {
+  width: 25px;
+  height: 25px;
+  cursor: pointer;
 }
```

### Comparing `npm-cockpit-0.2.1/src/client/css/styles.main.css` & `npm-cockpit-0.3.0/src/client/css/styles.main.css`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.2.1/src/client/favicon.ico` & `npm-cockpit-0.3.0/src/client/favicon.ico`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.2.1/src/client/font/Arimo-Bold.woff2` & `npm-cockpit-0.3.0/src/client/font/Arimo-Bold.woff2`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.2.1/src/client/font/Arimo-Regular.woff2` & `npm-cockpit-0.3.0/src/client/font/Arimo-Regular.woff2`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.2.1/src/client/font/Arimo-SemiBold.woff2` & `npm-cockpit-0.3.0/src/client/font/Arimo-SemiBold.woff2`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.2.1/src/client/index.html` & `npm-cockpit-0.3.0/src/client/index.html`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.2.1/src/client/js/components/dashboard.js` & `npm-cockpit-0.3.0/src/client/js/components/dashboard.js`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.2.1/src/client/js/components/elements/dependency-filter.js` & `npm-cockpit-0.3.0/src/client/js/components/elements/dependency-filter.js`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.2.1/src/client/js/components/elements/dependency-info.js` & `npm-cockpit-0.3.0/src/client/js/components/elements/dependency-info.js`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.2.1/src/client/js/components/elements/dependency-item.js` & `npm-cockpit-0.3.0/src/client/js/components/elements/dependency-item.js`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.2.1/src/client/js/components/elements/select.js` & `npm-cockpit-0.3.0/src/client/js/components/elements/select.js`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.2.1/src/client/js/components/elements/table.js` & `npm-cockpit-0.3.0/src/client/js/components/elements/table.js`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.2.1/src/client/js/components/index.js` & `npm-cockpit-0.3.0/src/client/js/components/index.js`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.2.1/src/client/js/components/items/Item.js` & `npm-cockpit-0.3.0/src/client/js/components/items/Item.js`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.2.1/src/client/js/components/items/basic-info.js` & `npm-cockpit-0.3.0/src/client/js/components/items/basic-info.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,54 +1,70 @@
 import Item from './Item.js'
 import {
     makeRequest
 } from '../../utils.js'
 
 export class BasicInfo extends Item {
-    updates = 0
-    vulnerabilities = 0
-    nodes = 0
-    deprecated = 0
+    updates = null
+    vulnerabilities = null
+    nodes = null
+    deprecated = null
     directDependencies = 0
     directUpdates = 0
     directVulns = 0
     directDeprecated = 0
 
     constructor() {
         super('/api/dependencies')
     }
 
     async processData() {
         this.loading = true
 
-        const vulnerabilitiesData = await makeRequest('/api/vulnerabilities')
-        const updates = await makeRequest('/api/updates')
-        const deprecated = await makeRequest('/api/deprecated')
-
-        if (vulnerabilitiesData.error || updates.error || deprecated.error) {
-            this.error = true
-            this.loading = false
-            this.render()
-            return
+        let vulnLibs = []
+        let updatesLibs = []
+        let deprecatedLibs = []
+
+        const [vulnerabilities, updates, deprecated] = await Promise.allSettled(
+            [
+                makeRequest('/api/vulnerabilities'),
+                makeRequest('/api/updates'),
+                makeRequest('/api/deprecated')
+            ]
+        ).then((values) => values.map(item => item.value))
+
+        // if(vulnerabilities.error || updates.error || deprecated.error) {
+        //   this.error = true
+        //   this.loading = false
+        //   this.render()
+        //   return
+        // }
+
+        if (!vulnerabilities.error) {
+            const {
+                vulnerabilities: vulnerabilitiesItems
+            } = vulnerabilities
+            vulnLibs = Object.keys(vulnerabilitiesItems)
+            this.vulnerabilities = vulnLibs.length
         }
 
-        const {
-            vulnerabilities
-        } = vulnerabilitiesData
-        const vulnLibs = Object.keys(vulnerabilities)
-        const updatesLibs = Object.keys(updates)
-        const deprecatedLibs = Object.keys(deprecated)
+        if (!updates.error) {
+            updatesLibs = Object.keys(updates)
+            this.updates = updatesLibs.length
+        }
 
-        this.nodes = Object.keys(this.data.dependencies).length
-        this.updates = updatesLibs.length
-        this.vulnerabilities = vulnLibs.length
-        this.deprecated = deprecatedLibs.length
+        if (!deprecated.error) {
+            deprecatedLibs = Object.keys(deprecated)
+            this.deprecated = deprecatedLibs.length
+        }
 
+        this.nodes = Object.keys(this.data.dependencies).length
         const root = this.data.dependencies[this.data.root][0]
         this.directDependencies = root.connections.length
+
         root.connections.forEach(item => {
             if (updatesLibs.includes(item.name)) {
                 this.directUpdates += 1
             }
             if (vulnLibs.includes(item.name)) {
                 this.directVulns += 1
             }
@@ -58,14 +74,19 @@
         })
 
         this.loading = false
         this.render()
     }
 
     createSection(title, total, direct, indicator, target) {
+        // if data was not loaded hide the section
+        if (total === null) {
+            return ''
+        }
+
         const container = document.createElement('div')
         container.className = 'basic-info_section'
 
         const dataContainer = document.createElement('div')
 
         const titleContainer = document.createElement('div')
         titleContainer.className = 'basic-info_section_title'
```

### Comparing `npm-cockpit-0.2.1/src/client/js/components/items/dependencies-list.js` & `npm-cockpit-0.3.0/src/client/js/components/items/dependencies-list.js`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.2.1/src/client/js/components/items/dependencies-network.js` & `npm-cockpit-0.3.0/src/client/js/components/items/dependencies-network.js`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.2.1/src/client/js/components/items/dependencies-tree.js` & `npm-cockpit-0.3.0/src/client/js/components/items/dependencies-tree.js`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.2.1/src/client/js/components/items/deprecated-table.js` & `npm-cockpit-0.3.0/src/client/js/components/items/deprecated-table.js`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.2.1/src/client/js/components/items/frequency.js` & `npm-cockpit-0.3.0/src/client/js/components/items/frequency.js`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.2.1/src/client/js/components/items/index.js` & `npm-cockpit-0.3.0/src/client/js/components/items/index.js`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.2.1/src/client/js/components/items/issues-table.js` & `npm-cockpit-0.3.0/src/client/js/components/items/issues-table.js`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.2.1/src/client/js/components/items/package-data.js` & `npm-cockpit-0.3.0/src/client/js/components/items/package-data.js`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.2.1/src/client/js/components/items/updates-table.js` & `npm-cockpit-0.3.0/src/client/js/components/items/updates-table.js`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.2.1/src/client/js/components/items/updates.js` & `npm-cockpit-0.3.0/src/client/js/components/items/updates.js`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.2.1/src/client/js/components/items/vulnerabilities-table.js` & `npm-cockpit-0.3.0/src/client/js/components/items/vulnerabilities-table.js`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.2.1/src/client/js/components/items/vulnerabilities.js` & `npm-cockpit-0.3.0/src/client/js/components/items/vulnerabilities.js`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.2.1/src/client/js/components/items/weight.js` & `npm-cockpit-0.3.0/src/client/js/components/items/weight.js`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.2.1/src/client/js/components/popups/group-data.js` & `npm-cockpit-0.3.0/src/client/js/components/popups/group-data.js`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.2.1/src/client/js/components/popups/module-data.js` & `npm-cockpit-0.3.0/src/client/js/components/popups/module-data.js`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.2.1/src/client/js/components/popups/section-info.js` & `npm-cockpit-0.3.0/src/client/js/components/popups/section-info.js`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.2.1/src/client/js/components/popups.js` & `npm-cockpit-0.3.0/src/client/js/components/popups.js`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.2.1/src/client/js/lib/d3.min.js` & `npm-cockpit-0.3.0/src/client/js/lib/d3.min.js`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.2.1/src/client/js/plots/bar.js` & `npm-cockpit-0.3.0/src/client/js/plots/bar.js`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.2.1/src/client/js/plots/dependencies-network.js` & `npm-cockpit-0.3.0/src/client/js/plots/dependencies-network.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -8,27 +8,36 @@
         .attr('height', '100%')
 
     const height = parseInt(plot.style('height'))
     const width = parseInt(plot.style('width'))
 
     const g = plot.append('g')
         .attr('id', 'plot-content')
+    const buttons = plot.append('g')
 
     const zoom = d3.zoom()
         .extent([
             [0, 0],
             [width, height]
         ])
         .on('zoom', zoomed)
 
-    // applying zoom
-    plot
-        // setting default zoom values
-        .call(zoom.transform, d3.zoomIdentity.translate(40, height / 4).scale(0.5))
-        .call(zoom)
+    defaultZoom()
+
+    // applying center plot button
+    buttons.append('image')
+        .attr('xlink:href', '/static/center-icon.svg')
+        .attr('id', 'center-icon')
+        .on('click', function() {
+            defaultZoom()
+        })
+        // numbers are slight moving for better positioning
+        .attr('transform', `translate(${width - 40}, 16)`)
+        .append('title')
+        .text('Center plot')
 
     plot.append('defs')
         .append('marker')
         .attr('id', 'arrow')
         .attr('viewBox', '0 0 10 10')
         .attr('refX', '5')
         .attr('refY', '5')
@@ -149,14 +158,21 @@
                     return 1
                 }
 
                 return 0.2
             })
     }
 
+    function defaultZoom() {
+        plot
+            // setting default zoom values
+            .call(zoom.transform, d3.zoomIdentity.translate(40, height / 4).scale(0.5))
+            .call(zoom)
+    }
+
     function findParents(nodes, selected, root) {
         const parents = nodes.filter(node => node.connections.find(connection => connection.name === selected.name && connection.version === selected.version))
         return [...parents, ...parents.map(item => findParents(nodes, item, root))].flat()
     }
 
     function findChilds(nodes, selected, target) {
         const childs = selected.connections.map(connection => {
```

### Comparing `npm-cockpit-0.2.1/src/client/js/plots/dependencies-tree.js` & `npm-cockpit-0.3.0/src/client/js/plots/dependencies-tree.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -23,31 +23,48 @@
         .attr('r', nodeRadius)
         .style('stroke', '#63a3ee')
         .style('stroke-width', '1')
         .style('rx', '10')
         .style('ry', '10')
         .style('box-shadow', '5px 10px')
 
+    const buttons = plot.append('g')
     const content = plot.append('g')
         .attr('id', 'plot-content')
     content.append('g')
         .attr('id', 'paths')
     content.append('g')
         .attr('id', 'nodes')
 
-    // applying zoom
-    plot
-        // setting default zoom values
-        .call(zoom.transform, d3.zoomIdentity.translate(width / 2, height / 2).scale(0.5))
-        .call(zoom)
+    defaultZoom()
+
+    // applying center plot button
+    buttons.append('image')
+        .attr('xlink:href', '/static/center-icon.svg')
+        .attr('id', 'center-icon')
+        .on('click', function() {
+            defaultZoom()
+        })
+        // numbers are slight moving for better positioning
+        .attr('transform', `translate(${width - 40}, 16)`)
+        .append('title')
+        .text('Center plot')
+
 
     render(data)
 
     return render
 
+    function defaultZoom() {
+        plot
+            // setting default zoom values
+            .call(zoom.transform, d3.zoomIdentity.translate(width / 2, height / 2).scale(0.5))
+            .call(zoom)
+    }
+
     function render(data) {
         const nodes = d3.hierarchy(data, d => d.deps)
         const pathsContainer = plot.select('#paths')
         const nodesContainer = plot.select('#nodes')
 
         d3.tree().nodeSize([nodeHeight + nodeSeparation, nodeWidth + nodeSeparation * 5])(nodes)
```

### Comparing `npm-cockpit-0.2.1/src/client/js/plots/donut.js` & `npm-cockpit-0.3.0/src/client/js/plots/donut.js`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.2.1/src/client/js/workers/dependenciesList.js` & `npm-cockpit-0.3.0/src/client/js/workers/dependenciesList.js`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.2.1/src/client/js/workers/dependenciesNetwork.js` & `npm-cockpit-0.3.0/src/client/js/workers/dependenciesNetwork.js`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.2.1/src/client/js/workers/dependenciesTree.js` & `npm-cockpit-0.3.0/src/client/js/workers/dependenciesTree.js`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.2.1/src/client/js/workers/frequency.js` & `npm-cockpit-0.3.0/src/client/js/workers/frequency.js`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.2.1/src/client/js/workers/updates.js` & `npm-cockpit-0.3.0/src/client/js/workers/updates.js`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.2.1/src/client/js/workers/updatesTable.js` & `npm-cockpit-0.3.0/src/client/js/workers/updatesTable.js`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.2.1/src/client/js/workers/weight.js` & `npm-cockpit-0.3.0/src/client/js/workers/weight.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -18,14 +18,16 @@
         const found = []
 
         // -1 because the package itself will be also added, but it shouldn't
         let count = -1
 
         while (stack.length && stack.length) {
             const dep = stack.shift()
+            if (!dep) return
+
             const namever = dep.name + '@' + dep.version
             if (found.includes(namever)) continue
 
             const packages = dep.connections.map(item => {
                 const {
                     name,
                     version
```

### Comparing `npm-cockpit-0.2.1/src/client/layout.json` & `npm-cockpit-0.3.0/src/client/layout.json`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.2.1/src/client/static/clear-icon.svg` & `npm-cockpit-0.3.0/src/client/static/clear-icon.svg`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.2.1/src/client/static/dep-icon.svg` & `npm-cockpit-0.3.0/src/client/static/dep-icon.svg`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.2.1/src/client/static/loading.svg` & `npm-cockpit-0.3.0/src/client/static/loading.svg`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.2.1/src/client/static/net-icon.svg` & `npm-cockpit-0.3.0/src/client/static/net-icon.svg`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.2.1/src/client/static/tree-icon.svg` & `npm-cockpit-0.3.0/src/client/static/tree-icon.svg`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.2.1/src/client/static/vuln-icon.svg` & `npm-cockpit-0.3.0/src/client/static/vuln-icon.svg`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.2.1/setup.py` & `npm-cockpit-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,22 +23,22 @@
 ['requests>=2.28.2,<3.0.0']
 
 entry_points = \
 {'console_scripts': ['npm-cockpit = src.app.app:init']}
 
 setup_kwargs = {
     'name': 'npm-cockpit',
-    'version': '0.2.1',
+    'version': '0.3.0',
     'description': 'Installable command-line tool with web interface which helps to track nodejs project dependencies state',
-    'long_description': '# NPM-COCKPIT\n\nA user-friendly application for JavaScript developers to visualize the dependency tree of NPM packages and NodeJS applications. \n\nAllows to get statistical info about application dependencies tree state. Provides an interface for filtering and viewing information through convenient tables and diagrams.\n\n## Features\n\nVisual representation of the entire dependency tree of a project. With ability to look all the paths for a specific package. Dependency tree can be visualized as a tree or directed network chart\n\n![tree chart](https://chartexample.com/images/npm-cockpit/network.jpg)\n\nDetailed information about each package, including version, description, and related links.\n\n![packages list](https://chartexample.com/images/npm-cockpit/list.jpg)\n\nIdentify potential issues such as outdated, deprecated or vulnerable packages.\n\n![packages list](https://chartexample.com/images/npm-cockpit/deprecated.jpg)\n\n**AND MUCH MORE!**\n\n\n## Requirements\n\n### General\n- Terminal or command prompt access\n- Target application folder should contain node_modules folder with installed dependencies and package.json\n- Node.js and NPM installed\n\n### As an NPM package\n- `python` command should be available\n\n## Usage\n\n### Command params\n\n`path` - a path to project folder with package.json and node_modules inside\n\n`port` - available local port to serve the app (default `8080`)\n\n### PIP\n`pip install npm-cockpit`\n\n`npm-cockpit [path] [port]`\n\n### NPM globally installed\n`npm install --global npm-cockpit`\n\n`npm-cockpit [path] [port]`\n\n### NPX\n`npx npm-cockpit [path] [port]`\n\n### NPM dependency in package\n`npm install npm-cockpit` and add the run script in the package json with proper params\n\n## Development\n- `git clone https://github.com/b0000ring/npm-cockpit.git`\n- `cd npm-cockpit`\n- `node index.js [path] [port]` or `python __main__.py [path] [port]`\n',
+    'long_description': '# NPM-COCKPIT\n\nA user-friendly application for JavaScript developers to visualize the dependency tree of NPM packages and NodeJS applications. \n\nAllows to get statistical info about application dependencies tree state. Provides an interface for filtering and viewing information through convenient tables and diagrams.\n\n## Features\n\nVisual representation of the entire dependency tree of a project. With ability to look all the paths for a specific package. Dependency tree can be visualized as a tree or directed network chart\n\n![tree chart](https://chartexample.com/images/npm-cockpit/network.jpg)\n\nDetailed information about each package, including version, description, and related links.\n\n![packages list](https://chartexample.com/images/npm-cockpit/list.jpg)\n\nIdentify potential issues such as outdated, deprecated or vulnerable packages.\n\n![packages list](https://chartexample.com/images/npm-cockpit/deprecated.jpg)\n\n**AND MUCH MORE!**\n\n\n## Requirements\n\n### General\n- Terminal or command prompt access\n- Target application folder should contain node_modules folder with installed dependencies and package.json\n- Node.js and NPM installed\n\n### As NPM package\n- `python` command should be available\n\n## Usage\n\n### Command params\n\n`path` - a path to project folder with package.json and node_modules inside\n\n`port` - available local port to serve the app (default `8080`)\n\n### PIP\n`pip install npm-cockpit`\n\n`npm-cockpit [path] [port]`\n\n### NPM globally installed\n`npm install --global npm-cockpit`\n\n`npm-cockpit [path] [port]`\n\n### NPX\n`npx npm-cockpit [path] [port]`\n\n### NPM dependency in package\n`npm install npm-cockpit` and add the run script in the package json with proper params\n\n## Development\n- `git clone https://github.com/b0000ring/npm-cockpit.git`\n- `cd npm-cockpit`\n- `node index.js [path] [port]` or `python __main__.py [path] [port]`\n',
     'author': 'Alex Chirkin',
     'author_email': 'hello@alexchirkin.me',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
+    'maintainer': None,
+    'maintainer_email': None,
+    'url': None,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
     'python_requires': '>=3.7,<4.0',
 }
```

### Comparing `npm-cockpit-0.2.1/PKG-INFO` & `npm-cockpit-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: npm-cockpit
-Version: 0.2.1
+Version: 0.3.0
 Summary: Installable command-line tool with web interface which helps to track nodejs project dependencies state
 License: MIT
 Keywords: command,dashboard,npm,statistic,dependencies,packages,info
 Author: Alex Chirkin
 Author-email: hello@alexchirkin.me
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Description-Content-Type: text/markdown
 
 # NPM-COCKPIT
 
 A user-friendly application for JavaScript developers to visualize the dependency tree of NPM packages and NodeJS applications. 
 
@@ -42,15 +42,15 @@
 ## Requirements
 
 ### General
 - Terminal or command prompt access
 - Target application folder should contain node_modules folder with installed dependencies and package.json
 - Node.js and NPM installed
 
-### As an NPM package
+### As NPM package
 - `python` command should be available
 
 ## Usage
 
 ### Command params
 
 `path` - a path to project folder with package.json and node_modules inside
```

