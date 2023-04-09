# Comparing `tmp/notionai-py-0.1.2.tar.gz` & `tmp/notionai-py-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notionai-py-0.1.2.tar", last modified: Mon Mar 13 08:07:56 2023, max compression
+gzip compressed data, was "notionai-py-0.1.3.tar", last modified: Sun Apr  9 14:16:47 2023, max compression
```

## Comparing `notionai-py-0.1.2.tar` & `notionai-py-0.1.3.tar`

### file list

```diff
@@ -1,92 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 08:07:56.841026 notionai-py-0.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 08:07:56.825026 notionai-py-0.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 08:07:56.829026 notionai-py-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-03-13 08:07:29.000000 notionai-py-0.1.2/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-03-13 08:07:29.000000 notionai-py-0.1.2/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-03-13 08:07:29.000000 notionai-py-0.1.2/.github/workflows/upload-to-chrome-store.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-03-13 08:07:29.000000 notionai-py-0.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-03-13 08:07:29.000000 notionai-py-0.1.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-03-13 08:07:29.000000 notionai-py-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-03-13 08:07:56.841026 notionai-py-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-03-13 08:07:29.000000 notionai-py-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-03-13 08:07:29.000000 notionai-py-0.1.2/changelog.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 08:07:56.829026 notionai-py-0.1.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 08:07:56.833026 notionai-py-0.1.2/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)   336248 2023-03-13 08:07:29.000000 notionai-py-0.1.2/docs/images/example-webui.png
--rw-r--r--   0 runner    (1001) docker     (123)   278813 2023-03-13 08:07:29.000000 notionai-py-0.1.2/docs/images/get_notion_token.png
--rw-r--r--   0 runner    (1001) docker     (123)   217196 2023-03-13 08:07:29.000000 notionai-py-0.1.2/docs/images/notion-space-id.png
--rw-r--r--   0 runner    (1001) docker     (123)    70417 2023-03-13 08:07:29.000000 notionai-py-0.1.2/docs/images/notionai-plus-1.png
--rw-r--r--   0 runner    (1001) docker     (123)   256123 2023-03-13 08:07:29.000000 notionai-py-0.1.2/docs/images/notionai-plus-2.png
--rw-r--r--   0 runner    (1001) docker     (123)   121639 2023-03-13 08:07:29.000000 notionai-py-0.1.2/docs/images/notionai-plus-3.png
--rw-r--r--   0 runner    (1001) docker     (123)    88026 2023-03-13 08:07:29.000000 notionai-py-0.1.2/docs/images/notionai-plus-4.png
--rw-r--r--   0 runner    (1001) docker     (123)   127106 2023-03-13 08:07:29.000000 notionai-py-0.1.2/docs/images/notionai-plus-5.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 08:07:56.829026 notionai-py-0.1.2/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 08:07:56.833026 notionai-py-0.1.2/examples/basic/
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-03-13 08:07:29.000000 notionai-py-0.1.2/examples/basic/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 08:07:56.833026 notionai-py-0.1.2/examples/webui/
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-03-13 08:07:29.000000 notionai-py-0.1.2/examples/webui/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-03-13 08:07:29.000000 notionai-py-0.1.2/examples/webui/app.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-13 08:07:29.000000 notionai-py-0.1.2/examples/webui/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 08:07:56.833026 notionai-py-0.1.2/notionai/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-13 08:07:29.000000 notionai-py-0.1.2/notionai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-03-13 08:07:29.000000 notionai-py-0.1.2/notionai/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    10953 2023-03-13 08:07:29.000000 notionai-py-0.1.2/notionai/notionai.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 08:07:56.833026 notionai-py-0.1.2/notionai-chrome/
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-03-13 08:07:29.000000 notionai-py-0.1.2/notionai-chrome/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-03-13 08:07:29.000000 notionai-py-0.1.2/notionai-chrome/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-03-13 08:07:29.000000 notionai-py-0.1.2/notionai-chrome/background.js
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-03-13 08:07:29.000000 notionai-py-0.1.2/notionai-chrome/content.js
--rw-r--r--   0 runner    (1001) docker     (123)    20835 2023-03-13 08:07:29.000000 notionai-py-0.1.2/notionai-chrome/icon copy.png
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-03-13 08:07:29.000000 notionai-py-0.1.2/notionai-chrome/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-03-13 08:07:29.000000 notionai-py-0.1.2/notionai-chrome/manifest.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 08:07:56.837026 notionai-py-0.1.2/notionai-plus/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 08:07:56.829026 notionai-py-0.1.2/notionai-plus/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 08:07:56.837026 notionai-py-0.1.2/notionai-plus/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-03-13 08:07:29.000000 notionai-py-0.1.2/notionai-plus/.github/workflows/submit.yml
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-03-13 08:07:29.000000 notionai-py-0.1.2/notionai-plus/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-03-13 08:07:29.000000 notionai-py-0.1.2/notionai-plus/.prettierrc.cjs
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-03-13 08:07:29.000000 notionai-py-0.1.2/notionai-plus/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-03-13 08:07:29.000000 notionai-py-0.1.2/notionai-plus/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 08:07:56.837026 notionai-py-0.1.2/notionai-plus/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    79750 2023-03-13 08:07:29.000000 notionai-py-0.1.2/notionai-plus/assets/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-03-13 08:07:29.000000 notionai-py-0.1.2/notionai-plus/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-03-13 08:07:29.000000 notionai-py-0.1.2/notionai-plus/package.json
--rw-r--r--   0 runner    (1001) docker     (123)   188185 2023-03-13 08:07:29.000000 notionai-py-0.1.2/notionai-plus/pnpm-lock.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-03-13 08:07:29.000000 notionai-py-0.1.2/notionai-plus/postcss.config.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 08:07:56.837026 notionai-py-0.1.2/notionai-plus/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 08:07:56.837026 notionai-py-0.1.2/notionai-plus/src/background/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-03-13 08:07:29.000000 notionai-py-0.1.2/notionai-plus/src/background/index.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 08:07:56.837026 notionai-py-0.1.2/notionai-plus/src/background/messages/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-03-13 08:07:29.000000 notionai-py-0.1.2/notionai-plus/src/background/messages/get-notion-spaces.ts
--rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-03-13 08:07:29.000000 notionai-py-0.1.2/notionai-plus/src/background/messages/request.ts
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-03-13 08:07:29.000000 notionai-py-0.1.2/notionai-plus/src/base.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 08:07:56.837026 notionai-py-0.1.2/notionai-plus/src/components/
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-03-13 08:07:29.000000 notionai-py-0.1.2/notionai-plus/src/components/select.tsx
--rw-r--r--   0 runner    (1001) docker     (123)    12827 2023-03-13 08:07:29.000000 notionai-py-0.1.2/notionai-plus/src/content.tsx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 08:07:56.837026 notionai-py-0.1.2/notionai-plus/src/features/
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-03-13 08:07:29.000000 notionai-py-0.1.2/notionai-plus/src/features/count-button.tsx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 08:07:56.837026 notionai-py-0.1.2/notionai-plus/src/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 08:07:56.837026 notionai-py-0.1.2/notionai-plus/src/lib/api/
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-03-13 08:07:29.000000 notionai-py-0.1.2/notionai-plus/src/lib/api/chatgpt.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-03-13 08:07:29.000000 notionai-py-0.1.2/notionai-plus/src/lib/api/chatgptapi.ts
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-03-13 08:07:29.000000 notionai-py-0.1.2/notionai-plus/src/lib/api/notion.ts
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-03-13 08:07:29.000000 notionai-py-0.1.2/notionai-plus/src/lib/api/readability.ts
--rw-r--r--   0 runner    (1001) docker     (123)     6583 2023-03-13 08:07:29.000000 notionai-py-0.1.2/notionai-plus/src/lib/enums.ts
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-03-13 08:07:29.000000 notionai-py-0.1.2/notionai-plus/src/lib/prompt-enums.ts
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-03-13 08:07:29.000000 notionai-py-0.1.2/notionai-plus/src/lib/storage.ts
--rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-03-13 08:07:29.000000 notionai-py-0.1.2/notionai-plus/src/options.tsx
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-03-13 08:07:29.000000 notionai-py-0.1.2/notionai-plus/src/popup.tsx
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-13 08:07:29.000000 notionai-py-0.1.2/notionai-plus/src/style.css
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-03-13 08:07:29.000000 notionai-py-0.1.2/notionai-plus/tailwind.config.js
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-03-13 08:07:29.000000 notionai-py-0.1.2/notionai-plus/tsconfig.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 08:07:56.837026 notionai-py-0.1.2/notionai_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-03-13 08:07:56.000000 notionai-py-0.1.2/notionai_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-03-13 08:07:56.000000 notionai-py-0.1.2/notionai_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 08:07:56.000000 notionai-py-0.1.2/notionai_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-13 08:07:56.000000 notionai-py-0.1.2/notionai_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-13 08:07:56.000000 notionai-py-0.1.2/notionai_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-03-13 08:07:29.000000 notionai-py-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-13 08:07:56.841026 notionai-py-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 08:07:56.841026 notionai-py-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 08:07:29.000000 notionai-py-0.1.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-03-13 08:07:29.000000 notionai-py-0.1.2/tests/notionai_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:16:47.308513 notionai-py-0.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:16:47.304513 notionai-py-0.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:16:47.304513 notionai-py-0.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-09 14:16:25.000000 notionai-py-0.1.3/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 14:16:25.000000 notionai-py-0.1.3/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-04-09 14:16:25.000000 notionai-py-0.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-09 14:16:25.000000 notionai-py-0.1.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-09 14:16:25.000000 notionai-py-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-04-09 14:16:47.308513 notionai-py-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-04-09 14:16:25.000000 notionai-py-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-09 14:16:25.000000 notionai-py-0.1.3/changelog.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:16:47.304513 notionai-py-0.1.3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:16:47.308513 notionai-py-0.1.3/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   336248 2023-04-09 14:16:25.000000 notionai-py-0.1.3/docs/images/example-webui.png
+-rw-r--r--   0 runner    (1001) docker     (123)   278813 2023-04-09 14:16:25.000000 notionai-py-0.1.3/docs/images/get_notion_token.png
+-rw-r--r--   0 runner    (1001) docker     (123)   217196 2023-04-09 14:16:25.000000 notionai-py-0.1.3/docs/images/notion-space-id.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:16:47.304513 notionai-py-0.1.3/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:16:47.308513 notionai-py-0.1.3/examples/basic/
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-09 14:16:25.000000 notionai-py-0.1.3/examples/basic/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:16:47.308513 notionai-py-0.1.3/examples/webui/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-09 14:16:25.000000 notionai-py-0.1.3/examples/webui/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-04-09 14:16:25.000000 notionai-py-0.1.3/examples/webui/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-09 14:16:25.000000 notionai-py-0.1.3/examples/webui/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:16:47.308513 notionai-py-0.1.3/notionai/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-09 14:16:25.000000 notionai-py-0.1.3/notionai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-04-09 14:16:25.000000 notionai-py-0.1.3/notionai/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10988 2023-04-09 14:16:25.000000 notionai-py-0.1.3/notionai/notionai.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:16:47.308513 notionai-py-0.1.3/notionai_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-04-09 14:16:47.000000 notionai-py-0.1.3/notionai_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-09 14:16:47.000000 notionai-py-0.1.3/notionai_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 14:16:47.000000 notionai-py-0.1.3/notionai_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-09 14:16:47.000000 notionai-py-0.1.3/notionai_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-09 14:16:47.000000 notionai-py-0.1.3/notionai_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-04-09 14:16:25.000000 notionai-py-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 14:16:47.308513 notionai-py-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:16:47.308513 notionai-py-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 14:16:25.000000 notionai-py-0.1.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-04-09 14:16:25.000000 notionai-py-0.1.3/tests/notionai_test.py
```

### Comparing `notionai-py-0.1.2/.github/workflows/pypi.yml` & `notionai-py-0.1.3/.github/workflows/pypi.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 name: Publish package
 
 on:
     push:
         tags:
-            - "py-v*.*.*"
+            - "v*.*.*"
 
 jobs:
     publish:
         runs-on: ubuntu-latest
         steps:
             - uses: actions/checkout@v3
             - uses: actions/setup-python@v4
```

### Comparing `notionai-py-0.1.2/.gitignore` & `notionai-py-0.1.3/.gitignore`

 * *Files 9% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 .Python
 build/
 develop-eggs/
 dist/
 downloads/
 eggs/
 .eggs/
+lib/
 lib64/
 parts/
 sdist/
 var/
 wheels/
 pip-wheel-metadata/
 share/python-wheels/
@@ -122,10 +123,8 @@
 # mypy
 .mypy_cache/
 .dmypy.json
 dmypy.json
 
 # Pyre type checker
 .pyre/
-
 .envrc
-.DS_Store
```

### Comparing `notionai-py-0.1.2/LICENSE` & `notionai-py-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `notionai-py-0.1.2/README.md` & `notionai-py-0.1.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,21 @@
-# NotionAI
+Metadata-Version: 2.1
+Name: notionai-py
+Version: 0.1.3
+Summary: Unoffical Notion AI API
+Author-email: Vaayne <liu.vaayne@gmail.com>
+License: MIT License
+Project-URL: Homepage, https://github.com/Vaayne/NotionAI
+Project-URL: Bug Tracker, https://github.com/Vaayne/NotionAI/issues
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3
+Description-Content-Type: text/markdown
+License-File: LICENSE
 
-NotionAI is an unofficial NotionAI API that provides a Python SDK and a Chrome extension.
-
-## NotionAI Plus Extension
-
-NotionAI Plus is a browser extension that adds NotionAI's powerful features to any website you visit. With NotionAI Plus, you can easily analyze text, generate summaries, and perform sentiment analysis on any webpage.
-
-- [Chrome Web Store](https://chrome.google.com/webstore/detail/notionai-plus/ilgkcoockdhdpkikaakkjacblhpmdmeo)
-- [Firefox Addon](https://addons.mozilla.org/en-US/firefox/addon/notionai-plus/)
-
-
-### NotionAI Chrome Extension Demo
-
-
-
-https://user-images.githubusercontent.com/10231735/221889423-17fe70e3-2be6-40b3-84b6-57a3333510f0.mp4
-
-
-
-#### Screen Capture
-
-|            Screen Capture 1            |            Screen Capture 2            |            Screen Capture 3            |            Screen Capture 4            |            Screen Capture 5            |
-| :------------------------------------: | :------------------------------------: | :------------------------------------: | :------------------------------------: | :------------------------------------: |
-| ![](./docs/images/notionai-plus-1.png) | ![](./docs/images/notionai-plus-2.png) | ![](./docs/images/notionai-plus-3.png) | ![](./docs/images/notionai-plus-4.png) | ![](./docs/images/notionai-plus-5.png) |
-
-
-## NotionAI Python SDK
+# NotionAI Python SDK
 
 The NotionAI Python SDK is a wrapper for the NotionAI APIs with Python bindings, simplifying integration of NotionAI solutions into your projects.
 
 ### Features
 
 - Full APIs from Notion AI
 - Support stream response
```

### Comparing `notionai-py-0.1.2/docs/images/example-webui.png` & `notionai-py-0.1.3/docs/images/example-webui.png`

 * *Files identical despite different names*

### Comparing `notionai-py-0.1.2/docs/images/get_notion_token.png` & `notionai-py-0.1.3/docs/images/get_notion_token.png`

 * *Files identical despite different names*

### Comparing `notionai-py-0.1.2/docs/images/notion-space-id.png` & `notionai-py-0.1.3/docs/images/notion-space-id.png`

 * *Files identical despite different names*

### Comparing `notionai-py-0.1.2/examples/basic/main.py` & `notionai-py-0.1.3/examples/basic/main.py`

 * *Files identical despite different names*

### Comparing `notionai-py-0.1.2/examples/webui/app.py` & `notionai-py-0.1.3/examples/webui/app.py`

 * *Files identical despite different names*

### Comparing `notionai-py-0.1.2/notionai/enums.py` & `notionai-py-0.1.3/notionai/enums.py`

 * *Files identical despite different names*

### Comparing `notionai-py-0.1.2/notionai/notionai.py` & `notionai-py-0.1.3/notionai/notionai.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 import json
 import uuid
 
 import requests
 
 from notionai.enums import PromptTypeEnum, ToneEnum, TopicEnum, TranslateLanguageEnum
```

### Comparing `notionai-py-0.1.2/pyproject.toml` & `notionai-py-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "notionai-py"
 description = "Unoffical Notion AI API"
-version="0.1.2"
+version="0.1.3"
 authors = [
   { name="Vaayne", email="liu.vaayne@gmail.com" },
 ]
 readme = "README.md"
 requires-python = ">=3"
 license = {text = "MIT License"}
 classifiers = [
```

### Comparing `notionai-py-0.1.2/tests/notionai_test.py` & `notionai-py-0.1.3/tests/notionai_test.py`

 * *Files identical despite different names*

