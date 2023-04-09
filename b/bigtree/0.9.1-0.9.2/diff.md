# Comparing `tmp/bigtree-0.9.1.tar.gz` & `tmp/bigtree-0.9.2.tar.gz`

## Comparing `bigtree-0.9.1.tar` & `bigtree-0.9.2.tar`

### file list

```diff
@@ -1,105 +1,106 @@
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 bigtree-0.9.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 bigtree-0.9.1/.readthedocs.yaml
--rw-r--r--   0        0        0    11953 2020-02-02 00:00:00.000000 bigtree-0.9.1/CHANGELOG.md
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 bigtree-0.9.1/CONTRIBUTING.md
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 bigtree-0.9.1/.github/workflows/codecov.yml
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 bigtree-0.9.1/.github/workflows/docs.yml
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 bigtree-0.9.1/.github/workflows/pytest.yml
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 bigtree-0.9.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0   757076 2020-02-02 00:00:00.000000 bigtree-0.9.1/assets/DejaVuSans.ttf
--rw-r--r--   0        0        0    20084 2020-02-02 00:00:00.000000 bigtree-0.9.1/assets/binarytree.png
--rw-r--r--   0        0        0    11224 2020-02-02 00:00:00.000000 bigtree-0.9.1/assets/custom_tree.png
--rw-r--r--   0        0        0    14377 2020-02-02 00:00:00.000000 bigtree-0.9.1/assets/dag_construct.png
--rw-r--r--   0        0        0    12108 2020-02-02 00:00:00.000000 bigtree-0.9.1/assets/demo.png
--rw-r--r--   0        0        0    17554 2020-02-02 00:00:00.000000 bigtree-0.9.1/assets/demo_binarytree.png
--rw-r--r--   0        0        0    19320 2020-02-02 00:00:00.000000 bigtree-0.9.1/assets/demo_dag.png
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 bigtree-0.9.1/assets/demo_pillow.png
--rw-r--r--   0        0        0    10235 2020-02-02 00:00:00.000000 bigtree-0.9.1/assets/demo_tree.png
--rw-r--r--   0        0        0   313013 2020-02-02 00:00:00.000000 bigtree-0.9.1/assets/modify_advanced.png
--rw-r--r--   0        0        0   180588 2020-02-02 00:00:00.000000 bigtree-0.9.1/assets/modify_shift_and_copy.png
--rw-r--r--   0        0        0    67777 2020-02-02 00:00:00.000000 bigtree-0.9.1/assets/tree_construct.png
--rw-r--r--   0        0        0    11482 2020-02-02 00:00:00.000000 bigtree-0.9.1/assets/weighted_tree.png
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 bigtree-0.9.1/bigtree/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.1/bigtree/py.typed
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 bigtree-0.9.1/bigtree/binarytree/construct.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.1/bigtree/dag/__init__.py
--rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 bigtree-0.9.1/bigtree/dag/construct.py
--rw-r--r--   0        0        0     9742 2020-02-02 00:00:00.000000 bigtree-0.9.1/bigtree/dag/export.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.1/bigtree/node/__init__.py
--rw-r--r--   0        0        0    21938 2020-02-02 00:00:00.000000 bigtree-0.9.1/bigtree/node/basenode.py
--rw-r--r--   0        0        0    13631 2020-02-02 00:00:00.000000 bigtree-0.9.1/bigtree/node/binarynode.py
--rw-r--r--   0        0        0    18189 2020-02-02 00:00:00.000000 bigtree-0.9.1/bigtree/node/dagnode.py
--rw-r--r--   0        0        0     6343 2020-02-02 00:00:00.000000 bigtree-0.9.1/bigtree/node/node.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.1/bigtree/tree/__init__.py
--rw-r--r--   0        0        0    33732 2020-02-02 00:00:00.000000 bigtree-0.9.1/bigtree/tree/construct.py
--rw-r--r--   0        0        0    30164 2020-02-02 00:00:00.000000 bigtree-0.9.1/bigtree/tree/export.py
--rw-r--r--   0        0        0     6226 2020-02-02 00:00:00.000000 bigtree-0.9.1/bigtree/tree/helper.py
--rw-r--r--   0        0        0    33168 2020-02-02 00:00:00.000000 bigtree-0.9.1/bigtree/tree/modify.py
--rw-r--r--   0        0        0    12597 2020-02-02 00:00:00.000000 bigtree-0.9.1/bigtree/tree/search.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.1/bigtree/utils/__init__.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 bigtree-0.9.1/bigtree/utils/exceptions.py
--rw-r--r--   0        0        0    13884 2020-02-02 00:00:00.000000 bigtree-0.9.1/bigtree/utils/iterators.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.1/bigtree/workflows/__init__.py
--rw-r--r--   0        0        0     8516 2020-02-02 00:00:00.000000 bigtree-0.9.1/bigtree/workflows/app_todo.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 bigtree-0.9.1/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 bigtree-0.9.1/docs/make.bat
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 bigtree-0.9.1/docs/requirements.txt
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 bigtree-0.9.1/docs/source/binarytree.rst
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 bigtree-0.9.1/docs/source/conf.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 bigtree-0.9.1/docs/source/dag.rst
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 bigtree-0.9.1/docs/source/index.rst
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 bigtree-0.9.1/docs/source/node.rst
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 bigtree-0.9.1/docs/source/others.rst
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 bigtree-0.9.1/docs/source/tree.rst
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 bigtree-0.9.1/docs/source/utils.rst
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 bigtree-0.9.1/docs/source/workflows.rst
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 bigtree-0.9.1/docs/source/_static/custom.css
--rw-r--r--   0        0        0    27138 2020-02-02 00:00:00.000000 bigtree-0.9.1/docs/source/_static/favicon.ico
--rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 bigtree-0.9.1/docs/source/_templates/layout.html
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 bigtree-0.9.1/docs/source/bigtree/binarytree/construct.rst
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 bigtree-0.9.1/docs/source/bigtree/dag/construct.rst
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 bigtree-0.9.1/docs/source/bigtree/dag/export.rst
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 bigtree-0.9.1/docs/source/bigtree/node/basenode.rst
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 bigtree-0.9.1/docs/source/bigtree/node/binarynode.rst
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 bigtree-0.9.1/docs/source/bigtree/node/dagnode.rst
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 bigtree-0.9.1/docs/source/bigtree/node/node.rst
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 bigtree-0.9.1/docs/source/bigtree/tree/construct.rst
--rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 bigtree-0.9.1/docs/source/bigtree/tree/export.rst
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 bigtree-0.9.1/docs/source/bigtree/tree/helper.rst
--rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 bigtree-0.9.1/docs/source/bigtree/tree/modify.rst
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 bigtree-0.9.1/docs/source/bigtree/tree/search.rst
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 bigtree-0.9.1/docs/source/bigtree/utils/iterators.rst
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 bigtree-0.9.1/docs/source/bigtree/workflows/app_todo.rst
--rw-r--r--   0        0        0     2897 2020-02-02 00:00:00.000000 bigtree-0.9.1/docs/source/others/contributing.rst
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 bigtree-0.9.1/docs/source/others/list_dir.md
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 bigtree-0.9.1/docs/source/others/merging_trees.md
--rw-r--r--   0        0        0     2389 2020-02-02 00:00:00.000000 bigtree-0.9.1/docs/source/others/nodes.md
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 bigtree-0.9.1/docs/source/others/tips.rst
--rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 bigtree-0.9.1/docs/source/others/weighted_trees.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.1/tests/__init__.py
--rw-r--r--   0        0        0     9434 2020-02-02 00:00:00.000000 bigtree-0.9.1/tests/conftest.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.1/tests/binarytree/__init__.py
--rw-r--r--   0        0        0     6206 2020-02-02 00:00:00.000000 bigtree-0.9.1/tests/binarytree/test_construct.py
--rw-r--r--   0        0        0     2907 2020-02-02 00:00:00.000000 bigtree-0.9.1/tests/binarytree/test_export.py
--rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 bigtree-0.9.1/tests/binarytree/test_helper.py
--rw-r--r--   0        0        0     6806 2020-02-02 00:00:00.000000 bigtree-0.9.1/tests/binarytree/test_search.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.1/tests/dag/__init__.py
--rw-r--r--   0        0        0     5994 2020-02-02 00:00:00.000000 bigtree-0.9.1/tests/dag/test_construct.py
--rw-r--r--   0        0        0    13219 2020-02-02 00:00:00.000000 bigtree-0.9.1/tests/dag/test_export.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.1/tests/node/__init__.py
--rw-r--r--   0        0        0    31896 2020-02-02 00:00:00.000000 bigtree-0.9.1/tests/node/test_basenode.py
--rw-r--r--   0        0        0    36199 2020-02-02 00:00:00.000000 bigtree-0.9.1/tests/node/test_binarynode.py
--rw-r--r--   0        0        0    31052 2020-02-02 00:00:00.000000 bigtree-0.9.1/tests/node/test_dagnode.py
--rw-r--r--   0        0        0    12364 2020-02-02 00:00:00.000000 bigtree-0.9.1/tests/node/test_node.py
--rw-r--r--   0        0        0    57110 2020-02-02 00:00:00.000000 bigtree-0.9.1/tests/tree/test_construct.py
--rw-r--r--   0        0        0    36567 2020-02-02 00:00:00.000000 bigtree-0.9.1/tests/tree/test_export.py
--rw-r--r--   0        0        0     4737 2020-02-02 00:00:00.000000 bigtree-0.9.1/tests/tree/test_helper.py
--rw-r--r--   0        0        0    67770 2020-02-02 00:00:00.000000 bigtree-0.9.1/tests/tree/test_modify.py
--rw-r--r--   0        0        0    17729 2020-02-02 00:00:00.000000 bigtree-0.9.1/tests/tree/test_search.py
--rw-r--r--   0        0        0    13545 2020-02-02 00:00:00.000000 bigtree-0.9.1/tests/utils/test_iterators.py
--rw-r--r--   0        0        0    17809 2020-02-02 00:00:00.000000 bigtree-0.9.1/tests/workflows/test_todo.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 bigtree-0.9.1/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 bigtree-0.9.1/LICENSE
--rw-r--r--   0        0        0    22020 2020-02-02 00:00:00.000000 bigtree-0.9.1/README.md
--rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 bigtree-0.9.1/pyproject.toml
--rw-r--r--   0        0        0    23128 2020-02-02 00:00:00.000000 bigtree-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 bigtree-0.9.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 bigtree-0.9.2/.readthedocs.yaml
+-rw-r--r--   0        0        0    12174 2020-02-02 00:00:00.000000 bigtree-0.9.2/CHANGELOG.md
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 bigtree-0.9.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 bigtree-0.9.2/.github/workflows/codecov.yml
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 bigtree-0.9.2/.github/workflows/docs.yml
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 bigtree-0.9.2/.github/workflows/pytest.yml
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 bigtree-0.9.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0   757076 2020-02-02 00:00:00.000000 bigtree-0.9.2/assets/DejaVuSans.ttf
+-rw-r--r--   0        0        0    20084 2020-02-02 00:00:00.000000 bigtree-0.9.2/assets/binarytree.png
+-rw-r--r--   0        0        0    11224 2020-02-02 00:00:00.000000 bigtree-0.9.2/assets/custom_tree.png
+-rw-r--r--   0        0        0    14377 2020-02-02 00:00:00.000000 bigtree-0.9.2/assets/dag_construct.png
+-rw-r--r--   0        0        0    12108 2020-02-02 00:00:00.000000 bigtree-0.9.2/assets/demo.png
+-rw-r--r--   0        0        0    17554 2020-02-02 00:00:00.000000 bigtree-0.9.2/assets/demo_binarytree.png
+-rw-r--r--   0        0        0    19320 2020-02-02 00:00:00.000000 bigtree-0.9.2/assets/demo_dag.png
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 bigtree-0.9.2/assets/demo_pillow.png
+-rw-r--r--   0        0        0    10235 2020-02-02 00:00:00.000000 bigtree-0.9.2/assets/demo_tree.png
+-rw-r--r--   0        0        0   313013 2020-02-02 00:00:00.000000 bigtree-0.9.2/assets/modify_advanced.png
+-rw-r--r--   0        0        0   180588 2020-02-02 00:00:00.000000 bigtree-0.9.2/assets/modify_shift_and_copy.png
+-rw-r--r--   0        0        0    67777 2020-02-02 00:00:00.000000 bigtree-0.9.2/assets/tree_construct.png
+-rw-r--r--   0        0        0    11482 2020-02-02 00:00:00.000000 bigtree-0.9.2/assets/weighted_tree.png
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 bigtree-0.9.2/bigtree/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.2/bigtree/py.typed
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 bigtree-0.9.2/bigtree/binarytree/construct.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.2/bigtree/dag/__init__.py
+-rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 bigtree-0.9.2/bigtree/dag/construct.py
+-rw-r--r--   0        0        0     9742 2020-02-02 00:00:00.000000 bigtree-0.9.2/bigtree/dag/export.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.2/bigtree/node/__init__.py
+-rw-r--r--   0        0        0    21938 2020-02-02 00:00:00.000000 bigtree-0.9.2/bigtree/node/basenode.py
+-rw-r--r--   0        0        0    13631 2020-02-02 00:00:00.000000 bigtree-0.9.2/bigtree/node/binarynode.py
+-rw-r--r--   0        0        0    18189 2020-02-02 00:00:00.000000 bigtree-0.9.2/bigtree/node/dagnode.py
+-rw-r--r--   0        0        0     6712 2020-02-02 00:00:00.000000 bigtree-0.9.2/bigtree/node/node.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.2/bigtree/tree/__init__.py
+-rw-r--r--   0        0        0    33732 2020-02-02 00:00:00.000000 bigtree-0.9.2/bigtree/tree/construct.py
+-rw-r--r--   0        0        0    30233 2020-02-02 00:00:00.000000 bigtree-0.9.2/bigtree/tree/export.py
+-rw-r--r--   0        0        0     6226 2020-02-02 00:00:00.000000 bigtree-0.9.2/bigtree/tree/helper.py
+-rw-r--r--   0        0        0    33168 2020-02-02 00:00:00.000000 bigtree-0.9.2/bigtree/tree/modify.py
+-rw-r--r--   0        0        0    12597 2020-02-02 00:00:00.000000 bigtree-0.9.2/bigtree/tree/search.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.2/bigtree/utils/__init__.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 bigtree-0.9.2/bigtree/utils/exceptions.py
+-rw-r--r--   0        0        0    13884 2020-02-02 00:00:00.000000 bigtree-0.9.2/bigtree/utils/iterators.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.2/bigtree/workflows/__init__.py
+-rw-r--r--   0        0        0     6533 2020-02-02 00:00:00.000000 bigtree-0.9.2/bigtree/workflows/app_calendar.py
+-rw-r--r--   0        0        0     8516 2020-02-02 00:00:00.000000 bigtree-0.9.2/bigtree/workflows/app_todo.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 bigtree-0.9.2/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 bigtree-0.9.2/docs/make.bat
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 bigtree-0.9.2/docs/requirements.txt
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 bigtree-0.9.2/docs/source/binarytree.rst
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 bigtree-0.9.2/docs/source/conf.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 bigtree-0.9.2/docs/source/dag.rst
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 bigtree-0.9.2/docs/source/index.rst
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 bigtree-0.9.2/docs/source/node.rst
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 bigtree-0.9.2/docs/source/others.rst
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 bigtree-0.9.2/docs/source/tree.rst
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 bigtree-0.9.2/docs/source/utils.rst
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 bigtree-0.9.2/docs/source/workflows.rst
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 bigtree-0.9.2/docs/source/_static/custom.css
+-rw-r--r--   0        0        0    27138 2020-02-02 00:00:00.000000 bigtree-0.9.2/docs/source/_static/favicon.ico
+-rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 bigtree-0.9.2/docs/source/_templates/layout.html
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 bigtree-0.9.2/docs/source/bigtree/binarytree/construct.rst
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 bigtree-0.9.2/docs/source/bigtree/dag/construct.rst
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 bigtree-0.9.2/docs/source/bigtree/dag/export.rst
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 bigtree-0.9.2/docs/source/bigtree/node/basenode.rst
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 bigtree-0.9.2/docs/source/bigtree/node/binarynode.rst
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 bigtree-0.9.2/docs/source/bigtree/node/dagnode.rst
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 bigtree-0.9.2/docs/source/bigtree/node/node.rst
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 bigtree-0.9.2/docs/source/bigtree/tree/construct.rst
+-rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 bigtree-0.9.2/docs/source/bigtree/tree/export.rst
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 bigtree-0.9.2/docs/source/bigtree/tree/helper.rst
+-rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 bigtree-0.9.2/docs/source/bigtree/tree/modify.rst
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 bigtree-0.9.2/docs/source/bigtree/tree/search.rst
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 bigtree-0.9.2/docs/source/bigtree/utils/iterators.rst
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 bigtree-0.9.2/docs/source/bigtree/workflows/app_todo.rst
+-rw-r--r--   0        0        0     2897 2020-02-02 00:00:00.000000 bigtree-0.9.2/docs/source/others/contributing.rst
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 bigtree-0.9.2/docs/source/others/list_dir.md
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 bigtree-0.9.2/docs/source/others/merging_trees.md
+-rw-r--r--   0        0        0     2389 2020-02-02 00:00:00.000000 bigtree-0.9.2/docs/source/others/nodes.md
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 bigtree-0.9.2/docs/source/others/tips.rst
+-rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 bigtree-0.9.2/docs/source/others/weighted_trees.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.2/tests/__init__.py
+-rw-r--r--   0        0        0     9434 2020-02-02 00:00:00.000000 bigtree-0.9.2/tests/conftest.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.2/tests/binarytree/__init__.py
+-rw-r--r--   0        0        0     6206 2020-02-02 00:00:00.000000 bigtree-0.9.2/tests/binarytree/test_construct.py
+-rw-r--r--   0        0        0     2944 2020-02-02 00:00:00.000000 bigtree-0.9.2/tests/binarytree/test_export.py
+-rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 bigtree-0.9.2/tests/binarytree/test_helper.py
+-rw-r--r--   0        0        0     6806 2020-02-02 00:00:00.000000 bigtree-0.9.2/tests/binarytree/test_search.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.2/tests/dag/__init__.py
+-rw-r--r--   0        0        0     5994 2020-02-02 00:00:00.000000 bigtree-0.9.2/tests/dag/test_construct.py
+-rw-r--r--   0        0        0    13410 2020-02-02 00:00:00.000000 bigtree-0.9.2/tests/dag/test_export.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.2/tests/node/__init__.py
+-rw-r--r--   0        0        0    31896 2020-02-02 00:00:00.000000 bigtree-0.9.2/tests/node/test_basenode.py
+-rw-r--r--   0        0        0    36199 2020-02-02 00:00:00.000000 bigtree-0.9.2/tests/node/test_binarynode.py
+-rw-r--r--   0        0        0    31052 2020-02-02 00:00:00.000000 bigtree-0.9.2/tests/node/test_dagnode.py
+-rw-r--r--   0        0        0    12870 2020-02-02 00:00:00.000000 bigtree-0.9.2/tests/node/test_node.py
+-rw-r--r--   0        0        0    57110 2020-02-02 00:00:00.000000 bigtree-0.9.2/tests/tree/test_construct.py
+-rw-r--r--   0        0        0    36938 2020-02-02 00:00:00.000000 bigtree-0.9.2/tests/tree/test_export.py
+-rw-r--r--   0        0        0     4737 2020-02-02 00:00:00.000000 bigtree-0.9.2/tests/tree/test_helper.py
+-rw-r--r--   0        0        0    67770 2020-02-02 00:00:00.000000 bigtree-0.9.2/tests/tree/test_modify.py
+-rw-r--r--   0        0        0    17729 2020-02-02 00:00:00.000000 bigtree-0.9.2/tests/tree/test_search.py
+-rw-r--r--   0        0        0    13545 2020-02-02 00:00:00.000000 bigtree-0.9.2/tests/utils/test_iterators.py
+-rw-r--r--   0        0        0    17809 2020-02-02 00:00:00.000000 bigtree-0.9.2/tests/workflows/test_todo.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 bigtree-0.9.2/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 bigtree-0.9.2/LICENSE
+-rw-r--r--   0        0        0    25288 2020-02-02 00:00:00.000000 bigtree-0.9.2/README.md
+-rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 bigtree-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0    26396 2020-02-02 00:00:00.000000 bigtree-0.9.2/PKG-INFO
```

### Comparing `bigtree-0.9.1/.pre-commit-config.yaml` & `bigtree-0.9.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.1/CHANGELOG.md` & `bigtree-0.9.2/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.9.2] - 2023-04-09
+### Added
+- Node: Added `show` method to print tree to console.
+- Workflow Calendar: Tree use case with calendar implementation.
+
 ## [0.9.1] - 2023-03-30
 ### Changed
 - Node: Added `sep` parameter to constructor instead of using getter and setter methods to set `sep`.
 
 ## [0.9.0] - 2023-03-29
 ### Added
 - Tree Modifier: Ability to copy/shift nodes with full path in `from_paths` for faster search performance, added `with_full_path` parameter.
@@ -247,14 +252,15 @@
 - Tree Exporter: To list, nested dictionary, pandas DataFrame.
 - Tree Helper: Cloning, pruning trees, get difference between two trees.
 - Tree Modifier: Shift and copy nodes within tree and between trees.
 - Tree Search: Find single or multiple nodes based on name, attribute, or custom criteria.
 - Utility Iterator: Tree traversal methods.
 - Workflow To Do App: Tree use case with to-do list implementation.
 
+[0.9.2]: https://github.com/kayjan/bigtree/compare/v0.9.1...v0.9.2
 [0.9.1]: https://github.com/kayjan/bigtree/compare/v0.9.0...v0.9.1
 [0.9.0]: https://github.com/kayjan/bigtree/compare/v0.8.4...v0.9.0
 [0.8.4]: https://github.com/kayjan/bigtree/compare/v0.8.3...v0.8.4
 [0.8.3]: https://github.com/kayjan/bigtree/compare/v0.8.2...v0.8.3
 [0.8.2]: https://github.com/kayjan/bigtree/compare/v0.8.1...v0.8.2
 [0.8.1]: https://github.com/kayjan/bigtree/compare/v0.8.0...v0.8.1
 [0.8.0]: https://github.com/kayjan/bigtree/compare/v0.7.4...v0.8.0
```

### Comparing `bigtree-0.9.1/.github/workflows/codecov.yml` & `bigtree-0.9.2/.github/workflows/codecov.yml`

 * *Files 18% similar despite different names*

```diff
@@ -23,21 +23,21 @@
           python-version: ${{ matrix.python-version }}
       - name: Add conda to system path
         run: |
           # $CONDA is an environment variable pointing to the root of the miniconda directory
           echo $CONDA/bin >> $GITHUB_PATH
       - name: Install dependencies
         run: |
-          conda install pandas
-          conda install pydot
-          conda install Pillow
+          python -m pip install pandas
+          python -m pip install pydot
+          python -m pip install Pillow
       - name: Generate coverage report
         run: |
-          conda install pytest
-          conda install pytest-cov
+          python -m pip install pytest
+          python -m pip install pytest-cov
           pytest --cov=./ --cov-report=xml
       - name: Upload coverage to Codecov
         if: ${{ github.event_name == 'push' }}
         uses: codecov/codecov-action@v3
         with:
           fail_ci_if_error: true # optional (default = false)
           name: codecov-umbrella
```

### Comparing `bigtree-0.9.1/.github/workflows/docs.yml` & `bigtree-0.9.2/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.1/.github/workflows/pytest.yml` & `bigtree-0.9.2/.github/workflows/pytest.yml`

 * *Files 12% similar despite different names*

```diff
@@ -23,29 +23,29 @@
           python-version: ${{ matrix.python-version }}
       - name: Add conda to system path
         run: |
           # $CONDA is an environment variable pointing to the root of the miniconda directory
           echo $CONDA/bin >> $GITHUB_PATH
       - name: Install dependencies
         run: |
-          conda install pandas
-          conda install pydot
-          conda install Pillow
+          python -m pip install pandas
+          python -m pip install pydot
+          python -m pip install Pillow
       - name: Lint with flake8
         run: |
-          conda install flake8
+          python -m pip install flake8
           # stop the build if there are Python syntax errors or undefined names
           flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics
           # exit-zero treats all errors as warnings. The GitHub editor is 127 chars wide
           flake8 . --count --exit-zero --max-complexity=10 --max-line-length=127 --statistics
       - name: Lint with black
         run: |
-          conda install black
+          python -m pip install black
           black . --check
       - name: Lint with isort
         run: |
-          conda install isort
+          python -m pip install isort
           isort --profile black . --check
       - name: Test with pytest
         run: |
-          conda install pytest
+          python -m pip install pytest
           pytest
```

### Comparing `bigtree-0.9.1/.github/workflows/python-publish.yml` & `bigtree-0.9.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.1/assets/DejaVuSans.ttf` & `bigtree-0.9.2/assets/DejaVuSans.ttf`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.1/assets/binarytree.png` & `bigtree-0.9.2/assets/binarytree.png`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.1/assets/custom_tree.png` & `bigtree-0.9.2/assets/custom_tree.png`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.1/assets/dag_construct.png` & `bigtree-0.9.2/assets/dag_construct.png`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.1/assets/demo.png` & `bigtree-0.9.2/assets/demo.png`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.1/assets/demo_binarytree.png` & `bigtree-0.9.2/assets/demo_binarytree.png`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.1/assets/demo_dag.png` & `bigtree-0.9.2/assets/demo_dag.png`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.1/assets/demo_pillow.png` & `bigtree-0.9.2/assets/demo_pillow.png`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.1/assets/demo_tree.png` & `bigtree-0.9.2/assets/demo_tree.png`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.1/assets/modify_advanced.png` & `bigtree-0.9.2/assets/modify_advanced.png`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.1/assets/modify_shift_and_copy.png` & `bigtree-0.9.2/assets/modify_shift_and_copy.png`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.1/assets/tree_construct.png` & `bigtree-0.9.2/assets/tree_construct.png`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.1/assets/weighted_tree.png` & `bigtree-0.9.2/assets/weighted_tree.png`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.1/bigtree/__init__.py` & `bigtree-0.9.2/bigtree/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.9.1"
+__version__ = "0.9.2"
 
 from bigtree.binarytree.construct import list_to_binarytree
 from bigtree.dag.construct import dataframe_to_dag, dict_to_dag, list_to_dag
 from bigtree.dag.export import dag_to_dataframe, dag_to_dict, dag_to_dot, dag_to_list
 from bigtree.node.basenode import BaseNode
 from bigtree.node.binarynode import BinaryNode
 from bigtree.node.dagnode import DAGNode
@@ -63,8 +63,9 @@
     dag_iterator,
     inorder_iter,
     levelorder_iter,
     levelordergroup_iter,
     postorder_iter,
     preorder_iter,
 )
+from bigtree.workflows.app_calendar import Calendar
 from bigtree.workflows.app_todo import AppToDo
```

### Comparing `bigtree-0.9.1/bigtree/binarytree/construct.py` & `bigtree-0.9.2/bigtree/binarytree/construct.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.1/bigtree/dag/construct.py` & `bigtree-0.9.2/bigtree/dag/construct.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.1/bigtree/dag/export.py` & `bigtree-0.9.2/bigtree/dag/export.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.1/bigtree/node/basenode.py` & `bigtree-0.9.2/bigtree/node/basenode.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.1/bigtree/node/binarynode.py` & `bigtree-0.9.2/bigtree/node/binarynode.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.1/bigtree/node/dagnode.py` & `bigtree-0.9.2/bigtree/node/dagnode.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.1/bigtree/node/node.py` & `bigtree-0.9.2/bigtree/node/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,22 @@
     1. ``sep``: Get/set separator for path name
 
     Get `Node` configuration
 
     1. ``node_name``: Get node name, without accessing `name` directly
     2. ``path_name``: Get path name from root, separated by `sep`
 
+    **Node Methods**
+
+    These are methods available to be performed on `Node`.
+
+    `Node` methods
+
+    1. ``show()``: Print tree to console
+
     ----
 
     """
 
     def __init__(self, name: str = "", sep: str = "/", **kwargs: Any):
         self.name = name
         self._sep = sep
@@ -195,14 +203,20 @@
         """No rules
 
         Args:
             new_children (List[Self]): new children to be added
         """
         self.__post_assign_children(new_children)
 
+    def show(self, **kwargs: Any) -> None:
+        """Print tree to console, takes in same keyword arguments as `print_tree` function"""
+        from bigtree.tree.export import print_tree
+
+        print_tree(self, **kwargs)
+
     def __repr__(self) -> str:
         """Print format of Node
 
         Returns:
             (str)
         """
         class_name = self.__class__.__name__
```

### Comparing `bigtree-0.9.1/bigtree/tree/construct.py` & `bigtree-0.9.2/bigtree/tree/construct.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.1/bigtree/tree/export.py` & `bigtree-0.9.2/bigtree/tree/export.py`

 * *Files 1% similar despite different names*

```diff
@@ -389,15 +389,15 @@
 
     Args:
         tree (Node): tree to be exported
         name_key (str): dictionary key for `node.node_name`, defaults to 'name'
         parent_key (str): dictionary key for `node.parent.node_name`, optional
         attr_dict (Dict[str, str]): dictionary mapping node attributes to dictionary key,
             key: node attributes, value: corresponding dictionary key, optional
-        all_attrs (bool): indicator whether to retrieve all `Node` attributes, defaults to False
+        all_attrs (bool): indicator whether to retrieve all `Node` attributes, overrides `attr_dict`, defaults to False
         max_depth (int): maximum depth to export tree, optional
         skip_depth (int): number of initial depth to skip, optional
         leaf_only (bool): indicator to retrieve only information from leaf nodes
 
     Returns:
         (Dict[str, Any])
     """
@@ -463,15 +463,15 @@
 
     Args:
         tree (Node): tree to be exported
         name_key (str): dictionary key for `node.node_name`, defaults to 'name'
         child_key (str): dictionary key for list of children, optional
         attr_dict (Dict[str, str]): dictionary mapping node attributes to dictionary key,
             key: node attributes, value: corresponding dictionary key, optional
-        all_attrs (bool): indicator whether to retrieve all `Node` attributes, defaults to False
+        all_attrs (bool): indicator whether to retrieve all `Node` attributes, overrides `attr_dict`, defaults to False
         max_depth (int): maximum depth to export tree, optional
 
     Returns:
         (Dict[str, Any])
     """
     tree = tree.copy()
     data_dict: Dict[str, List[Dict[str, Any]]] = {}
@@ -544,15 +544,15 @@
     Args:
         tree (Node): tree to be exported
         path_col (str): column name for `node.path_name`, optional
         name_col (str): column name for `node.node_name`, defaults to 'name'
         parent_col (str): column name for `node.parent.node_name`, optional
         attr_dict (Dict[str, str]): dictionary mapping node attributes to column name,
             key: node attributes, value: corresponding column in dataframe, optional
-        all_attrs (bool): indicator whether to retrieve all `Node` attributes, defaults to False
+        all_attrs (bool): indicator whether to retrieve all `Node` attributes, overrides `attr_dict`, defaults to False
         max_depth (int): maximum depth to export tree, optional
         skip_depth (int): number of initial depth to skip, optional
         leaf_only (bool): indicator to retrieve only information from leaf nodes
 
     Returns:
         (pd.DataFrame)
     """
```

### Comparing `bigtree-0.9.1/bigtree/tree/helper.py` & `bigtree-0.9.2/bigtree/tree/helper.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.1/bigtree/tree/modify.py` & `bigtree-0.9.2/bigtree/tree/modify.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.1/bigtree/tree/search.py` & `bigtree-0.9.2/bigtree/tree/search.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.1/bigtree/utils/iterators.py` & `bigtree-0.9.2/bigtree/utils/iterators.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.1/bigtree/workflows/app_todo.py` & `bigtree-0.9.2/bigtree/workflows/app_todo.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.1/docs/Makefile` & `bigtree-0.9.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.1/docs/make.bat` & `bigtree-0.9.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.1/docs/source/conf.py` & `bigtree-0.9.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.1/docs/source/index.rst` & `bigtree-0.9.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.1/docs/source/_static/custom.css` & `bigtree-0.9.2/docs/source/_static/custom.css`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.1/docs/source/_static/favicon.ico` & `bigtree-0.9.2/docs/source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.1/docs/source/_templates/layout.html` & `bigtree-0.9.2/docs/source/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.1/docs/source/bigtree/dag/construct.rst` & `bigtree-0.9.2/docs/source/bigtree/dag/construct.rst`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.1/docs/source/bigtree/dag/export.rst` & `bigtree-0.9.2/docs/source/bigtree/dag/export.rst`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.1/docs/source/bigtree/tree/construct.rst` & `bigtree-0.9.2/docs/source/bigtree/tree/construct.rst`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.1/docs/source/bigtree/tree/export.rst` & `bigtree-0.9.2/docs/source/bigtree/tree/export.rst`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.1/docs/source/bigtree/tree/modify.rst` & `bigtree-0.9.2/docs/source/bigtree/tree/modify.rst`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.1/docs/source/bigtree/tree/search.rst` & `bigtree-0.9.2/docs/source/bigtree/tree/search.rst`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.1/docs/source/bigtree/utils/iterators.rst` & `bigtree-0.9.2/docs/source/bigtree/utils/iterators.rst`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.1/docs/source/others/contributing.rst` & `bigtree-0.9.2/docs/source/others/contributing.rst`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.1/docs/source/others/merging_trees.md` & `bigtree-0.9.2/docs/source/others/merging_trees.md`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.1/docs/source/others/nodes.md` & `bigtree-0.9.2/docs/source/others/nodes.md`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.1/docs/source/others/weighted_trees.md` & `bigtree-0.9.2/docs/source/others/weighted_trees.md`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.1/tests/conftest.py` & `bigtree-0.9.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.1/tests/binarytree/test_construct.py` & `bigtree-0.9.2/tests/binarytree/test_construct.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.1/tests/binarytree/test_export.py` & `bigtree-0.9.2/tests/binarytree/test_export.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,16 @@
     tree_to_dataframe,
     tree_to_dict,
     tree_to_dot,
     tree_to_nested_dict,
 )
 from tests.conftest import assert_print_statement
 
+LOCAL = False
+
 
 class TestPrintTree:
     @staticmethod
     def test_print_tree(binarytree_node):
         expected_str = """1\n├── 2\n│   ├── 4\n│   │   └── 8\n│   └── 5\n└── 3\n    ├── 6\n    └── 7\n"""
         assert_print_statement(print_tree, expected_str, tree=binarytree_node)
 
@@ -76,12 +78,13 @@
 
 class TestTreeToDot:
     @staticmethod
     def test_tree_to_dot(binarytree_node):
         graph = tree_to_dot(binarytree_node)
         expected = """strict digraph G {\nrankdir=TB;\n10 [label=1];\n20 [label=2];\n10 -> 20;\n40 [label=4];\n20 -> 40;\n80 [label=8];\n40 -> 80;\n50 [label=5];\n20 -> 50;\n30 [label=3];\n10 -> 30;\n60 [label=6];\n30 -> 60;\n70 [label=7];\n30 -> 70;\n}\n"""
         actual = graph.to_string()
-        graph.write_png("tests/binarytree.png")
+        if LOCAL:
+            graph.write_png("tests/binarytree.png")
         for expected_str in expected.split():
             assert (
                 expected_str in actual
             ), f"Expected {expected_str} not in actual string"
```

### Comparing `bigtree-0.9.1/tests/binarytree/test_helper.py` & `bigtree-0.9.2/tests/binarytree/test_helper.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.1/tests/binarytree/test_search.py` & `bigtree-0.9.2/tests/binarytree/test_search.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.1/tests/dag/test_construct.py` & `bigtree-0.9.2/tests/dag/test_construct.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.1/tests/dag/test_export.py` & `bigtree-0.9.2/tests/dag/test_export.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,16 @@
     list_to_dag,
 )
 from tests.node.test_dagnode import (
     assert_dag_structure_attr_root,
     assert_dag_structure_root,
 )
 
+LOCAL = False
+
 
 class TestDAGToList:
     @staticmethod
     def test_dag_to_list(dag_node):
         expected = [
             ("a", "c"),
             ("a", "d"),
@@ -125,37 +127,40 @@
 
 class TestDAGToDot:
     @staticmethod
     def test_dag_to_dot(dag_node):
         graph = dag_to_dot(dag_node)
         expected = """strict digraph G {\na [label=a];\nc [label=c];\na -> c;\nd [label=d];\na -> d;\nc [label=c];\na [label=a];\na -> c;\nb [label=b];\nb -> c;\nd [label=d];\nc -> d;\nf [label=f];\nc -> f;\ng [label=g];\nc -> g;\nd [label=d];\na [label=a];\na -> d;\nc [label=c];\nc -> d;\ne [label=e];\nd -> e;\nf [label=f];\nd -> f;\ne [label=e];\nd [label=d];\nd -> e;\nf [label=f];\nc [label=c];\nc -> f;\nd [label=d];\nd -> f;\ng [label=g];\nc [label=c];\nc -> g;\nh [label=h];\ng -> h;\nh [label=h];\ng [label=g];\ng -> h;\nb [label=b];\nc [label=c];\nb -> c;\n}\n"""
         actual = graph.to_string()
-        graph.write_png("tests/dag.png")
+        if LOCAL:
+            graph.write_png("tests/dag.png")
         for expected_str in expected.split():
             assert (
                 expected_str in actual
             ), f"Expected {expected_str} not in actual string"
 
     @staticmethod
     def test_dag_to_dot_multiple(dag_node, dag_node_plot):
         graph = dag_to_dot([dag_node, dag_node_plot])
         expected = """strict digraph G {\nrankdir=TB;\nc [label=c];\na [label=a];\na -> c;\nd [label=d];\na [label=a];\na -> d;\nc [label=c];\nb [label=b];\nb -> c;\nd [label=d];\nc [label=c];\nc -> d;\nf [label=f];\nc [label=c];\nc -> f;\ng [label=g];\nc [label=c];\nc -> g;\ne [label=e];\nd [label=d];\nd -> e;\nf [label=f];\nd [label=d];\nd -> f;\nh [label=h];\ng [label=g];\ng -> h;\ny [label=y];\nz [label=z];\nz -> y;\n}\n"""
         actual = graph.to_string()
-        graph.write_png("tests/dag_multiple.png")
+        if LOCAL:
+            graph.write_png("tests/dag_multiple.png")
         for expected_str in expected.split():
             assert (
                 expected_str in actual
             ), f"Expected {expected_str} not in actual string"
 
     @staticmethod
     def test_dag_to_dot_from_child(dag_node_child):
         graph = dag_to_dot(dag_node_child)
         expected = """strict digraph G {\nf [label=f];\nc [label=c];\nc -> f;\nd [label=d];\nd -> f;\nc [label=c];\na [label=a];\na -> c;\nb [label=b];\nb -> c;\nd [label=d];\nc -> d;\nf [label=f];\nc -> f;\ng [label=g];\nc -> g;\nd [label=d];\na [label=a];\na -> d;\nc [label=c];\nc -> d;\ne [label=e];\nd -> e;\nf [label=f];\nd -> f;\ne [label=e];\nd [label=d];\nd -> e;\na [label=a];\nc [label=c];\na -> c;\nd [label=d];\na -> d;\ng [label=g];\nc [label=c];\nc -> g;\nh [label=h];\ng -> h;\nh [label=h];\ng [label=g];\ng -> h;\nb [label=b];\nc [label=c];\nb -> c;\n}\n"""
         actual = graph.to_string()
-        graph.write_png("tests/dag_child.png")
+        if LOCAL:
+            graph.write_png("tests/dag_child.png")
         for expected_str in expected.split():
             assert (
                 expected_str in actual
             ), f"Expected {expected_str} not in actual string"
 
     @staticmethod
     def test_dag_to_dot_type_error(tree_node):
@@ -164,56 +169,61 @@
         assert str(exc_info.value).startswith("Tree should be of type `DAGNode`")
 
     @staticmethod
     def test_dag_to_dot_bg_color(dag_node):
         graph = dag_to_dot(dag_node, bg_colour="blue")
         expected = """strict digraph G {\nbgcolor=blue;\na [label=a];\nc [label=c];\na -> c;\nd [label=d];\na -> d;\nc [label=c];\na [label=a];\na -> c;\nb [label=b];\nb -> c;\nd [label=d];\nc -> d;\nf [label=f];\nc -> f;\ng [label=g];\nc -> g;\nd [label=d];\na [label=a];\na -> d;\nc [label=c];\nc -> d;\ne [label=e];\nd -> e;\nf [label=f];\nd -> f;\ne [label=e];\nd [label=d];\nd -> e;\nf [label=f];\nc [label=c];\nc -> f;\nd [label=d];\nd -> f;\ng [label=g];\nc [label=c];\nc -> g;\nh [label=h];\ng -> h;\nh [label=h];\ng [label=g];\ng -> h;\nb [label=b];\nc [label=c];\nb -> c;\n}\n"""
         actual = graph.to_string()
-        graph.write_png("tests/dag_bg.png")
+        if LOCAL:
+            graph.write_png("tests/dag_bg.png")
         for expected_str in expected.split():
             assert (
                 expected_str in actual
             ), f"Expected {expected_str} not in actual string"
 
     @staticmethod
     def test_dag_to_dot_fill_color(dag_node):
         graph = dag_to_dot(dag_node, node_colour="gold")
         expected = """strict digraph G {\na [fillcolor=gold, label=a, style=filled];\nc [fillcolor=gold, label=c, style=filled];\na -> c;\nd [fillcolor=gold, label=d, style=filled];\na -> d;\nc [fillcolor=gold, label=c, style=filled];\na [fillcolor=gold, label=a, style=filled];\na -> c;\nb [fillcolor=gold, label=b, style=filled];\nb -> c;\nd [fillcolor=gold, label=d, style=filled];\nc -> d;\nf [fillcolor=gold, label=f, style=filled];\nc -> f;\ng [fillcolor=gold, label=g, style=filled];\nc -> g;\nd [fillcolor=gold, label=d, style=filled];\na [fillcolor=gold, label=a, style=filled];\na -> d;\nc [fillcolor=gold, label=c, style=filled];\nc -> d;\ne [fillcolor=gold, label=e, style=filled];\nd -> e;\nf [fillcolor=gold, label=f, style=filled];\nd -> f;\ne [fillcolor=gold, label=e, style=filled];\nd [fillcolor=gold, label=d, style=filled];\nd -> e;\nf [fillcolor=gold, label=f, style=filled];\nc [fillcolor=gold, label=c, style=filled];\nc -> f;\nd [fillcolor=gold, label=d, style=filled];\nd -> f;\ng [fillcolor=gold, label=g, style=filled];\nc [fillcolor=gold, label=c, style=filled];\nc -> g;\nh [fillcolor=gold, label=h, style=filled];\ng -> h;\nh [fillcolor=gold, label=h, style=filled];\ng [fillcolor=gold, label=g, style=filled];\ng -> h;\nb [fillcolor=gold, label=b, style=filled];\nc [fillcolor=gold, label=c, style=filled];\nb -> c;\n}\n"""
         actual = graph.to_string()
-        graph.write_png("tests/dag_fill.png")
+        if LOCAL:
+            graph.write_png("tests/dag_fill.png")
         for expected_str in expected.split():
             assert (
                 expected_str in actual
             ), f"Expected {expected_str} not in actual string"
 
     @staticmethod
     def test_dag_to_dot_edge_colour(dag_node):
         graph = dag_to_dot(dag_node, edge_colour="red")
         expected = """strict digraph G {\na [label=a];\nc [label=c];\na -> c  [color=red];\nd [label=d];\na -> d  [color=red];\nc [label=c];\na [label=a];\na -> c  [color=red];\nb [label=b];\nb -> c  [color=red];\nd [label=d];\nc -> d  [color=red];\nf [label=f];\nc -> f  [color=red];\ng [label=g];\nc -> g  [color=red];\nd [label=d];\na [label=a];\na -> d  [color=red];\nc [label=c];\nc -> d  [color=red];\ne [label=e];\nd -> e  [color=red];\nf [label=f];\nd -> f  [color=red];\ne [label=e];\nd [label=d];\nd -> e  [color=red];\nf [label=f];\nc [label=c];\nc -> f  [color=red];\nd [label=d];\nd -> f  [color=red];\ng [label=g];\nc [label=c];\nc -> g  [color=red];\nh [label=h];\ng -> h  [color=red];\nh [label=h];\ng [label=g];\ng -> h  [color=red];\nb [label=b];\nc [label=c];\nb -> c  [color=red];\n}\n"""
         actual = graph.to_string()
-        graph.write_png("tests/dag_edge.png")
+        if LOCAL:
+            graph.write_png("tests/dag_edge.png")
         for expected_str in expected.split():
             assert (
                 expected_str in actual
             ), f"Expected {expected_str} not in actual string"
 
     @staticmethod
     def test_dag_to_dot_node_attr(dag_node_style):
         graph = dag_to_dot(dag_node_style, node_attr="node_style")
         expected = """strict digraph G {\na [fillcolor=gold, label=a, style=filled];\nc [fillcolor=gold, label=c, style=filled];\na -> c;\nd [fillcolor=gold, label=d, style=filled];\na -> d;\nc [fillcolor=blue, label=c, style=filled];\na [fillcolor=blue, label=a, style=filled];\na -> c;\nb [fillcolor=blue, label=b, style=filled];\nb -> c;\nd [fillcolor=blue, label=d, style=filled];\nc -> d;\nf [fillcolor=blue, label=f, style=filled];\nc -> f;\ng [fillcolor=blue, label=g, style=filled];\nc -> g;\nd [fillcolor=green, label=d, style=filled];\na [fillcolor=green, label=a, style=filled];\na -> d;\nc [fillcolor=green, label=c, style=filled];\nc -> d;\ne [fillcolor=green, label=e, style=filled];\nd -> e;\nf [fillcolor=green, label=f, style=filled];\nd -> f;\ne [fillcolor=green, label=e, style=filled];\nd [fillcolor=green, label=d, style=filled];\nd -> e;\nf [fillcolor=green, label=f, style=filled];\nc [fillcolor=green, label=c, style=filled];\nc -> f;\nd [fillcolor=green, label=d, style=filled];\nd -> f;\ng [fillcolor=red, label=g, style=filled];\nc [fillcolor=red, label=c, style=filled];\nc -> g;\nh [fillcolor=red, label=h, style=filled];\ng -> h;\nh [fillcolor=red, label=h, style=filled];\ng [fillcolor=red, label=g, style=filled];\ng -> h;\nb [fillcolor=blue, label=b, style=filled];\nc [fillcolor=blue, label=c, style=filled];\nb -> c;\n}\n"""
         actual = graph.to_string()
-        graph.write_png("tests/dag_node_style.png")
+        if LOCAL:
+            graph.write_png("tests/dag_node_style.png")
         for expected_str in expected.split():
             assert (
                 expected_str in actual
             ), f"Expected {expected_str} not in actual string"
 
     @staticmethod
     def test_tree_to_dot_edge_attr(dag_node_style):
         graph = dag_to_dot(dag_node_style, edge_attr="edge_style")
         expected = """strict digraph G {\nrankdir=TB;\nc [label=c];\na [label=a];\na -> c  [label=c, style=bold];\nd [label=d];\na [label=a];\na -> d  [label=1, style=bold];\nc [label=c];\nb [label=b];\nb -> c  [label=c, style=bold];\nd [label=d];\nc [label=c];\nc -> d  [label=1, style=bold];\nf [label=f];\nc [label=c];\nc -> f  [label=3, style=bold];\ng [label=g];\nc [label=c];\nc -> g  [label=4, style=bold];\ne [label=e];\nd [label=d];\nd -> e  [label=2, style=bold];\nf [label=f];\nd [label=d];\nd -> f  [label=3, style=bold];\nh [label=h];\ng [label=g];\ng -> h  [label=5, style=bold];\n}\n"""
         actual = graph.to_string()
-        graph.write_png("tests/dag_edge_style.png")
+        if LOCAL:
+            graph.write_png("tests/dag_edge_style.png")
         for expected_str in expected.split():
             assert (
                 expected_str in actual
             ), f"Expected {expected_str} not in actual string"
```

### Comparing `bigtree-0.9.1/tests/node/test_basenode.py` & `bigtree-0.9.2/tests/node/test_basenode.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.1/tests/node/test_binarynode.py` & `bigtree-0.9.2/tests/node/test_binarynode.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.1/tests/node/test_dagnode.py` & `bigtree-0.9.2/tests/node/test_dagnode.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.1/tests/node/test_node.py` & `bigtree-0.9.2/tests/node/test_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from itertools import combinations
 
 import pytest
 
 from bigtree.node.node import Node
 from bigtree.utils.exceptions import LoopError, TreeError
 from bigtree.utils.iterators import preorder_iter
+from tests.conftest import assert_print_statement
 from tests.node.test_basenode import (
     assert_tree_structure_basenode_root_attr,
     assert_tree_structure_basenode_root_generic,
     assert_tree_structure_basenode_self,
 )
 
 
@@ -346,14 +347,28 @@
     ]
     for node, expected in zip(nodes, expected_ans):
         actual = node.path_name
         assert (
             actual == expected
         ), f"Node should have path {expected}, but path is {actual}"
 
+    # Test show
+    expected_str = """a\n├── b\n│   ├── d\n│   └── e\n│       ├── g\n│       └── h\n└── c\n    └── f\n"""
+    assert_print_statement(
+        self.a.show,
+        expected_str,
+    )
+
+    expected_str = """a\n|-- b\n|   |-- d\n|   `-- e\n|       |-- g\n|       `-- h\n`-- c\n    `-- f\n"""
+    assert_print_statement(
+        self.a.show,
+        expected_str,
+        style="ansi",
+    )
+
 
 def assert_tree_structure_node_root_sep(root):
     # Test path_name
     expected = "\\a"
     actual = root.path_name
     assert actual == expected, f"Node should have path {expected}, but path is {actual}"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `bigtree-0.9.1/tests/tree/test_construct.py` & `bigtree-0.9.2/tests/tree/test_construct.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.1/tests/tree/test_export.py` & `bigtree-0.9.2/tests/tree/test_export.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,17 @@
 from tests.node.test_node import assert_tree_structure_node_root_generic
 
 tree_node_str = """a [age=90]\n├── b [age=65]\n│   ├── d [age=40]\n│   └── e [age=35]\n│       ├── g [age=10]
 │       └── h [age=6]\n└── c [age=60]\n    └── f [age=38]\n"""
 tree_node_no_attr_str = """a\n├── b\n│   ├── d\n│   └── e\n│       ├── g\n│       └── h\n└── c\n    └── f\n"""
 
 
+LOCAL = False
+
+
 class TestPrintTree:
     @staticmethod
     def test_print_tree_child_node_name(tree_node):
         expected_str = """b\n├── d\n└── e\n    ├── g\n    └── h\n"""
         assert_print_statement(
             print_tree,
             expected_str,
@@ -290,15 +293,15 @@
         pd.testing.assert_frame_equal(expected, actual)
 
     @staticmethod
     def test_tree_to_dataframe_name_path_col_missing(tree_node):
         expected = pd.DataFrame()
         expected.index = range(8)
         actual = tree_to_dataframe(tree_node, name_col="", path_col="")
-        pd.testing.assert_frame_equal(expected, actual)
+        pd.testing.assert_frame_equal(expected, actual, check_column_type=False)
 
     @staticmethod
     def test_tree_to_dataframe_parent_col(tree_node):
         expected = pd.DataFrame(
             [
                 ["/a", "a", None],
                 ["/a/b", "b", "a"],
@@ -790,37 +793,40 @@
 
 class TestTreeToDot:
     @staticmethod
     def test_tree_to_dot(tree_node):
         graph = tree_to_dot(tree_node)
         expected = """strict digraph G {\nrankdir=TB;\na0 [label=a];\nb0 [label=b];\na0 -> b0;\nd0 [label=d];\nb0 -> d0;\ne0 [label=e];\nb0 -> e0;\ng0 [label=g];\ne0 -> g0;\nh0 [label=h];\ne0 -> h0;\nc0 [label=c];\na0 -> c0;\nf0 [label=f];\nc0 -> f0;\n}\n"""
         actual = graph.to_string()
-        graph.write_png("tests/tree.png")
+        if LOCAL:
+            graph.write_png("tests/tree.png")
         for expected_str in expected.split():
             assert (
                 expected_str in actual
             ), f"Expected {expected_str} not in actual string"
 
     @staticmethod
     def test_tree_to_dot_multiple(tree_node, tree_node_plot):
         graph = tree_to_dot([tree_node, tree_node_plot])
         expected = """strict digraph G {\nrankdir=TB;\na0 [label=a];\nb0 [label=b];\na0 -> b0;\nd0 [label=d];\nb0 -> d0;\ne0 [label=e];\nb0 -> e0;\ng0 [label=g];\ne0 -> g0;\nh0 [label=h];\ne0 -> h0;\nc0 [label=c];\na0 -> c0;\nf0 [label=f];\nc0 -> f0;\nz0 [label=z];\ny0 [label=y];\nz0 -> y0;\n}\n"""
         actual = graph.to_string()
-        graph.write_png("tests/tree_multiple.png")
+        if LOCAL:
+            graph.write_png("tests/tree_multiple.png")
         for expected_str in expected.split():
             assert (
                 expected_str in actual
             ), f"Expected {expected_str} not in actual string"
 
     @staticmethod
     def test_tree_to_dot_duplicate_names(tree_node_duplicate_names):
         graph = tree_to_dot(tree_node_duplicate_names)
         expected = """strict digraph G {\nrankdir=TB;\na0 [label=a];\na1 [label=a];\na0 -> a1;\na2 [label=a];\na1 -> a2;\nb0 [label=b];\na1 -> b0;\na3 [label=a];\nb0 -> a3;\nb1 [label=b];\nb0 -> b1;\nb2 [label=b];\na0 -> b2;\na4 [label=a];\nb2 -> a4;\n}\n"""
         actual = graph.to_string()
-        graph.write_png("tests/tree_duplicate.png")
+        if LOCAL:
+            graph.write_png("tests/tree_duplicate.png")
         for expected_str in expected.split():
             assert (
                 expected_str in actual
             ), f"Expected {expected_str} not in actual string"
 
     @staticmethod
     def test_tree_to_dot_type_error(dag_node):
@@ -829,107 +835,119 @@
         assert str(exc_info.value).startswith("Tree should be of type `Node`")
 
     @staticmethod
     def test_tree_to_dot_directed(tree_node):
         graph = tree_to_dot(tree_node, directed=False)
         expected = """strict graph G {\nrankdir=TB;\na0 [label=a];\nb0 [label=b];\na0 -- b0;\nd0 [label=d];\nb0 -- d0;\ne0 [label=e];\nb0 -- e0;\ng0 [label=g];\ne0 -- g0;\nh0 [label=h];\ne0 -- h0;\nc0 [label=c];\na0 -- c0;\nf0 [label=f];\nc0 -- f0;\n}\n"""
         actual = graph.to_string()
-        graph.write_png("tests/tree_undirected.png")
+        if LOCAL:
+            graph.write_png("tests/tree_undirected.png")
         for expected_str in expected.split():
             assert (
                 expected_str in actual
             ), f"Expected {expected_str} not in actual string"
 
     @staticmethod
     def test_tree_to_dot_bg_color(tree_node):
         graph = tree_to_dot(tree_node, bg_colour="blue")
         expected = """strict digraph G {\nbgcolor=blue;\nrankdir=TB;\na0 [label=a];\nb0 [label=b];\na0 -> b0;\nd0 [label=d];\nb0 -> d0;\ne0 [label=e];\nb0 -> e0;\ng0 [label=g];\ne0 -> g0;\nh0 [label=h];\ne0 -> h0;\nc0 [label=c];\na0 -> c0;\nf0 [label=f];\nc0 -> f0;\n}\n"""
         actual = graph.to_string()
-        graph.write_png("tests/tree_bg.png")
+        if LOCAL:
+            graph.write_png("tests/tree_bg.png")
         for expected_str in expected.split():
             assert (
                 expected_str in actual
             ), f"Expected {expected_str} not in actual string"
 
     @staticmethod
     def test_tree_to_dot_node_colour(tree_node):
         graph = tree_to_dot(tree_node, node_colour="gold")
         expected = """strict digraph G {\nrankdir=TB;\na0 [fillcolor=gold, label=a, style=filled];\nb0 [fillcolor=gold, label=b, style=filled];\na0 -> b0;\nd0 [fillcolor=gold, label=d, style=filled];\nb0 -> d0;\ne0 [fillcolor=gold, label=e, style=filled];\nb0 -> e0;\ng0 [fillcolor=gold, label=g, style=filled];\ne0 -> g0;\nh0 [fillcolor=gold, label=h, style=filled];\ne0 -> h0;\nc0 [fillcolor=gold, label=c, style=filled];\na0 -> c0;\nf0 [fillcolor=gold, label=f, style=filled];\nc0 -> f0;\n}\n"""
         actual = graph.to_string()
-        graph.write_png("tests/tree_fill.png")
+        if LOCAL:
+            graph.write_png("tests/tree_fill.png")
         for expected_str in expected.split():
             assert (
                 expected_str in actual
             ), f"Expected {expected_str} not in actual string"
 
     @staticmethod
     def test_tree_to_dot_node_shape(tree_node):
         graph = tree_to_dot(tree_node, node_shape="triangle")
         expected = """strict digraph G {\nrankdir=TB;\na0 [label=a, shape=triangle];\nb0 [label=b, shape=triangle];\na0 -> b0;\nd0 [label=d, shape=triangle];\nb0 -> d0;\ne0 [label=e, shape=triangle];\nb0 -> e0;\ng0 [label=g, shape=triangle];\ne0 -> g0;\nh0 [label=h, shape=triangle];\ne0 -> h0;\nc0 [label=c, shape=triangle];\na0 -> c0;\nf0 [label=f, shape=triangle];\nc0 -> f0;\n}\n"""
         actual = graph.to_string()
-        graph.write_png("tests/tree_triangle.png")
+        if LOCAL:
+            graph.write_png("tests/tree_triangle.png")
         for expected_str in expected.split():
             assert (
                 expected_str in actual
             ), f"Expected {expected_str} not in actual string"
 
     @staticmethod
     def test_tree_to_dot_edge_colour(tree_node):
         graph = tree_to_dot(tree_node, edge_colour="red")
         expected = """strict digraph G {\nrankdir=TB;\na0 [label=a];\nb0 [label=b];\na0 -> b0  [color=red];\nd0 [label=d];\nb0 -> d0  [color=red];\ne0 [label=e];\nb0 -> e0  [color=red];\ng0 [label=g];\ne0 -> g0  [color=red];\nh0 [label=h];\ne0 -> h0  [color=red];\nc0 [label=c];\na0 -> c0  [color=red];\nf0 [label=f];\nc0 -> f0  [color=red];\n}\n"""
         actual = graph.to_string()
-        graph.write_png("tests/tree_edge.png")
+        if LOCAL:
+            graph.write_png("tests/tree_edge.png")
         for expected_str in expected.split():
             assert (
                 expected_str in actual
             ), f"Expected {expected_str} not in actual string"
 
     @staticmethod
     def test_tree_to_dot_node_attr(tree_node_style):
         graph = tree_to_dot(tree_node_style, node_attr="node_style")
         expected = """strict digraph G {\nrankdir=TB;\na0 [fillcolor=gold, label=a, style=filled];\nb0 [fillcolor=blue, label=b, style=filled];\na0 -> b0;\nd0 [fillcolor=green, label=d, style=filled];\nb0 -> d0;\ng0 [fillcolor=red, label=g, style=filled];\nd0 -> g0;\ne0 [fillcolor=green, label=e, style=filled];\nb0 -> e0;\nh0 [fillcolor=red, label=h, style=filled];\ne0 -> h0;\nc0 [fillcolor=blue, label=c, style=filled];\na0 -> c0;\nf0 [fillcolor=green, label=f, style=filled];\nc0 -> f0;\n}\n"""
         actual = graph.to_string()
-        graph.write_png("tests/tree_node_style.png")
+        if LOCAL:
+            graph.write_png("tests/tree_node_style.png")
         for expected_str in expected.split():
             assert (
                 expected_str in actual
             ), f"Expected {expected_str} not in actual string"
 
     @staticmethod
     def test_tree_to_dot_edge_attr(tree_node_style):
         graph = tree_to_dot(tree_node_style, edge_attr="edge_style")
         expected = """strict digraph G {\nrankdir=TB;\na0 [label=a];\nb0 [label=b];\na0 -> b0  [label=b, style=bold];\nd0 [label=d];\nb0 -> d0  [label=1, style=bold];\ng0 [label=g];\nd0 -> g0  [label=4, style=bold];\ne0 [label=e];\nb0 -> e0  [label=2, style=bold];\nh0 [label=h];\ne0 -> h0  [label=5, style=bold];\nc0 [label=c];\na0 -> c0  [label=c, style=bold];\nf0 [label=f];\nc0 -> f0  [label=3, style=bold];\n}\n"""
         actual = graph.to_string()
-        graph.write_png("tests/tree_edge_style.png")
+        if LOCAL:
+            graph.write_png("tests/tree_edge_style.png")
         for expected_str in expected.split():
             assert (
                 expected_str in actual
             ), f"Expected {expected_str} not in actual string"
 
 
 class TestTreeToPillow:
     @staticmethod
     def test_tree_to_pillow(tree_node):
         pillow_image = tree_to_pillow(tree_node)
-        pillow_image.save("tests/tree_pillow.png")
+        if LOCAL:
+            pillow_image.save("tests/tree_pillow.png")
 
     @staticmethod
     def test_tree_to_pillow_start_pos(tree_node):
         pillow_image = tree_to_pillow(tree_node, start_pos=(100, 50))
-        pillow_image.save("tests/tree_pillow_start_pos.png")
+        if LOCAL:
+            pillow_image.save("tests/tree_pillow_start_pos.png")
 
     @staticmethod
     def test_tree_to_pillow_start_pos_small(tree_node):
         pillow_image = tree_to_pillow(tree_node, start_pos=(0, 0))
-        pillow_image.save("tests/tree_pillow_start_pos_small.png")
+        if LOCAL:
+            pillow_image.save("tests/tree_pillow_start_pos_small.png")
 
     @staticmethod
     def test_tree_to_pillow_font(tree_node):
         pillow_image = tree_to_pillow(
             tree_node, font_size=20, font_colour="red", bg_colour="lightblue"
         )
-        pillow_image.save("tests/tree_pillow_font.png")
+        if LOCAL:
+            pillow_image.save("tests/tree_pillow_font.png")
 
     @staticmethod
     def test_tree_to_pillow_kwargs(tree_node):
         pillow_image = tree_to_pillow(tree_node, max_depth=2, style="const_bold")
-        pillow_image.save("tests/tree_pillow_style.png")
+        if LOCAL:
+            pillow_image.save("tests/tree_pillow_style.png")
```

### Comparing `bigtree-0.9.1/tests/tree/test_helper.py` & `bigtree-0.9.2/tests/tree/test_helper.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.1/tests/tree/test_modify.py` & `bigtree-0.9.2/tests/tree/test_modify.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.1/tests/tree/test_search.py` & `bigtree-0.9.2/tests/tree/test_search.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.1/tests/utils/test_iterators.py` & `bigtree-0.9.2/tests/utils/test_iterators.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.1/tests/workflows/test_todo.py` & `bigtree-0.9.2/tests/workflows/test_todo.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.1/LICENSE` & `bigtree-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.1/README.md` & `bigtree-0.9.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -116,139 +116,123 @@
 
 1. **From `Node`**
 
 Nodes can be linked to each other with `parent` and `children` setter methods,
 or using bitshift operator with the convention `parent_node >> child_node` or `child_node << parent_node`.
 
 ```python
-from bigtree import Node, print_tree, tree_to_dot
+from bigtree import Node, tree_to_dot
 
-root = Node("a", age=90)
-b = Node("b", age=65)
-c = Node("c", age=60)
-d = Node("d", age=40)
+root = Node("a")
+b = Node("b")
+c = Node("c")
+d = Node("d")
 
 root.children = [b, c]
 d.parent = b
 
-print_tree(root, attr_list=["age"])
-# a [age=90]
-# ├── b [age=65]
-# │   └── d [age=40]
-# └── c [age=60]
+root.show()
+# a
+# ├── b
+# │   └── d
+# └── c
 
 graph = tree_to_dot(root, node_colour="gold")
 graph.write_png("assets/demo_tree.png")
 ```
 
 ![Sample Tree Output](https://github.com/kayjan/bigtree/raw/master/assets/demo_tree.png)
 
 ```python
-from bigtree import Node, print_tree
+from bigtree import Node
 
-root = Node("a", age=90)
-b = Node("b", age=65)
-c = Node("c", age=60)
-d = Node("d", age=40)
+root = Node("a")
+b = Node("b")
+c = Node("c")
+d = Node("d")
 
 root >> b
 root >> c
 d << b
 
-print_tree(root, attr_list=["age"])
-# a [age=90]
-# ├── b [age=65]
-# │   └── d [age=40]
-# └── c [age=60]
+root.show()
+# a
+# ├── b
+# │   └── d
+# └── c
 ```
 
 Alternatively, we can directly pass `parent` or `children` argument.
 
 ```python
-from bigtree import Node, print_tree
+from bigtree import Node
 
-root = Node("a")
-b = Node("b", parent=root)
-c = Node("c", parent=root)
-d = Node("d", parent=b)
-
-print_tree(root, style="ascii")
-# a
-# |-- b
-# |   +-- d
-# +-- c
-```
-
-```python
-from bigtree import Node, print_tree
-
-d = Node("d")
+b = Node("b")
 c = Node("c")
-b = Node("b", children=[d])
+d = Node("d", parent=b)
 root = Node("a", children=[b, c])
 
-print_tree(root, style="ascii")
+root.show(style="ascii")
 # a
 # |-- b
 # |   +-- d
 # +-- c
 ```
 
 2. **From *list***
 
 Construct nodes only, list can contain either full paths or tuples of parent-child names.
 
 ```python
-from bigtree import list_to_tree, list_to_tree_by_relation, print_tree
+from bigtree import list_to_tree, list_to_tree_by_relation
 
 root = list_to_tree(["a/b/d", "a/c"])
-
-print_tree(root)
+root.show()
 # a
 # ├── b
 # │   └── d
 # └── c
 
 root = list_to_tree_by_relation([("a", "b"), ("a", "c"), ("b", "d")])
-print_tree(root)
+root.show()
 # a
 # ├── b
 # │   └── d
 # └── c
 ```
 
 3. **From *nested dictionary***
 
 Construct nodes with attributes, `key`: path, `value`: dict of node attribute names and attribute values.
 
 ```python
-from bigtree import dict_to_tree, print_tree
+from bigtree import dict_to_tree
 
 path_dict = {
    "a": {"age": 90},
    "a/b": {"age": 65},
    "a/c": {"age": 60},
    "a/b/d": {"age": 40},
 }
-root = dict_to_tree(path_dict)
 
-print_tree(root, attr_list=["age"])
+root = dict_to_tree(path_dict)
+root.show(attr_list=["age"])
 # a [age=90]
 # ├── b [age=65]
 # │   └── d [age=40]
 # └── c [age=60]
 ```
 
 4. **From *nested recursive dictionary***
 
 Construct nodes with attributes, `key`: node attribute names, `value`: node attribute values, and list of
 children (recursive).
 
 ```python
-from bigtree import nested_dict_to_tree, print_tree
+from bigtree import nested_dict_to_tree
 
 path_dict = {
    "name": "a",
    "age": 90,
    "children": [
       {
          "name": "b",
@@ -256,82 +240,83 @@
          "children": [
             {"name": "d", "age": 40},
          ],
       },
       {"name": "c", "age": 60},
    ],
 }
-root = nested_dict_to_tree(path_dict)
 
-print_tree(root, attr_list=["age"])
+root = nested_dict_to_tree(path_dict)
+root.show(attr_list=["age"])
 # a [age=90]
 # ├── b [age=65]
 # │   └── d [age=40]
 # └── c [age=60]
 ```
 
 5. **From *pandas DataFrame***
 
 Construct nodes with attributes, *pandas DataFrame* can contain either path column or parent-child columns,
 and attribute columns.
 
 ```python
 import pandas as pd
 
-from bigtree import dataframe_to_tree, dataframe_to_tree_by_relation, print_tree
+from bigtree import dataframe_to_tree, dataframe_to_tree_by_relation
 
 data = pd.DataFrame(
    [
       ["a", 90],
       ["a/b", 65],
       ["a/c", 60],
       ["a/b/d", 40],
    ],
    columns=["path", "age"],
 )
-root = dataframe_to_tree(data)
 
-print_tree(root, attr_list=["age"])
+root = dataframe_to_tree(data)
+root.show(attr_list=["age"])
 # a [age=90]
 # ├── b [age=65]
 # │   └── d [age=40]
 # └── c [age=60]
 
 data = pd.DataFrame(
    [
       ["a", None, 90],
       ["b", "a", 65],
       ["c", "a", 60],
       ["d", "b", 40],
    ],
    columns=["child", "parent", "age"],
 )
-root = dataframe_to_tree_by_relation(data)
 
-print_tree(root, attr_list=["age"])
+root = dataframe_to_tree_by_relation(data)
+root.show(attr_list=["age"])
 # a [age=90]
 # ├── b [age=65]
 # │   └── d [age=40]
 # └── c [age=60]
 ```
 
 > If tree is already created, attributes can still be added using dictionary or pandas DataFrame!
 
 ### Print Tree
 
-After tree is constructed, it can be viewed by printing to console using `print_tree` method.
+After tree is constructed, it can be viewed by printing to console using `show` method directly.
+Alternatively, the `print_tree` method can be used.
 
 ```python
 from bigtree import Node, print_tree
 
-root = Node("a", age=90)
-b = Node("b", age=65, parent=root)
-c = Node("c", age=60, parent=root)
-d = Node("d", age=40, parent=b)
-e = Node("e", age=35, parent=b)
+root = Node("a", age=90, gender="F")
+b = Node("b", age=65, gender="M", parent=root)
+c = Node("c", age=60, gender="M", parent=root)
+d = Node("d", age=40, gender="F", parent=b)
+e = Node("e", age=35, gender="M", parent=b)
 print_tree(root)
 # a
 # ├── b
 # │   ├── d
 # │   └── e
 # └── c
 
@@ -357,14 +342,21 @@
 print_tree(root, attr_list=["age"], attr_bracket=["*(", ")"])
 # a *(age=90)
 # ├── b *(age=65)
 # │   ├── d *(age=40)
 # │   └── e *(age=35)
 # └── c *(age=60)
 
+print_tree(root, all_attrs=True)
+# a [age=90, gender=F]
+# ├── b [age=65, gender=M]
+# │   ├── d [age=40, gender=F]
+# │   └── e [age=35, gender=M]
+# └── c [age=60, gender=M]
+
 # Available styles
 print_tree(root, style="ansi")
 # a
 # |-- b
 # |   |-- d
 # |   `-- e
 # `-- c
@@ -412,113 +404,145 @@
 # a
 # |-- b
 # |   |-- d
 # |   +-- e
 # +-- c
 ```
 
+### Traverse Tree
+
+Tree can be traversed using pre-order, post-order, level-order, or level-order-group traversal methods.
+
+```python
+from bigtree import Node, preorder_iter, postorder_iter, levelorder_iter, levelordergroup_iter
+
+root = Node("a")
+b = Node("b", parent=root)
+c = Node("c", parent=root)
+d = Node("d", parent=b)
+e = Node("e", parent=b)
+root.show()
+# a
+# ├── b
+# │   ├── d
+# │   └── e
+# └── c
+
+[node.name for node in preorder_iter(root)]
+# ['a', 'b', 'd', 'e', 'c']
+
+[node.name for node in postorder_iter(root)]
+# ['d', 'e', 'b', 'c', 'a']
+
+[node.name for node in levelorder_iter(root)]
+# ['a', 'b', 'c', 'd', 'e']
+
+[[node.name for node in node_group] for node_group in levelordergroup_iter(root)]
+# [['a'], ['b', 'c'], ['d', 'e']]
+```
+
 ### Modify Tree
 
 Nodes can be shifted or copied from one path to another.
 
 ```python
-from bigtree import Node, shift_nodes, print_tree
+from bigtree import Node, shift_nodes
 
 root = Node("a")
 b = Node("b", parent=root)
 c = Node("c", parent=root)
 d = Node("d", parent=root)
-print_tree(root)
+root.show()
 # a
 # ├── b
 # ├── c
 # └── d
 
 shift_nodes(
    tree=root,
    from_paths=["a/c", "a/d"],
    to_paths=["a/b/c", "a/dummy/d"],
 )
-print_tree(root)
+root.show()
 # a
 # ├── b
 # │   └── c
 # └── dummy
 #     └── d
 ```
 
 ```python
-from bigtree import Node, copy_nodes, print_tree
+from bigtree import Node, copy_nodes
 
 root = Node("a")
 b = Node("b", parent=root)
 c = Node("c", parent=root)
 d = Node("d", parent=root)
-print_tree(root)
+root.show()
 # a
 # ├── b
 # ├── c
 # └── d
 
 copy_nodes(
    tree=root,
    from_paths=["a/c", "a/d"],
    to_paths=["a/b/c", "a/dummy/d"],
 )
-print_tree(root)
+root.show()
 # a
 # ├── b
 # │   └── c
 # ├── c
 # ├── d
 # └── dummy
 #     └── d
 ```
 
 Nodes can also be copied between two different trees.
 
 ```python
-from bigtree import Node, copy_nodes_from_tree_to_tree, print_tree
+from bigtree import Node, copy_nodes_from_tree_to_tree
 root = Node("a")
 b = Node("b", parent=root)
 c = Node("c", parent=root)
 d = Node("d", parent=root)
-print_tree(root)
+root.show()
 # a
 # ├── b
 # ├── c
 # └── d
 
 root_other = Node("aa")
 copy_nodes_from_tree_to_tree(
    from_tree=root,
    to_tree=root_other,
    from_paths=["a/b", "a/c", "a/d"],
    to_paths=["aa/b", "aa/b/c", "aa/dummy/d"],
 )
-print_tree(root_other)
+root_other.show()
 # aa
 # ├── b
 # │   └── c
 # └── dummy
 #     └── d
 ```
 
 ### Tree Search
 
 One or multiple nodes can be search based on name, path, attribute value, or user-defined condition.
 
 To find a single node,
 ```python
-from bigtree import Node, print_tree, find, find_name, find_path, find_full_path, find_attr
+from bigtree import Node, find, find_name, find_path, find_full_path, find_attr
 root = Node("a", age=90)
 b = Node("b", age=65, parent=root)
 c = Node("c", age=60, parent=root)
 d = Node("d", age=40, parent=c)
-print_tree(root, attr_list=["age"])
+root.show(attr_list=["age"])
 # a [age=90]
 # ├── b [age=65]
 # └── c [age=60]
 #     └── d [age=40]
 
 find(root, lambda node: node.age == 60)
 # Node(/a/c, age=60)
@@ -534,23 +558,23 @@
 
 find_attr(root, "age", 40)
 # Node(/a/c/d, age=40)
 ```
 
 To find multiple nodes,
 ```python
-from bigtree import Node, print_tree, findall, find_names, find_paths, find_attrs
+from bigtree import Node, findall, find_names, find_paths, find_attrs
 root = Node("a", age=90)
 b = Node("b", age=65, parent=root)
 c = Node("c", age=60, parent=root)
 d = Node("c", age=40, parent=c)
-print_tree(root, attr_list=["age"])
+root.show(attr_list=["age"])
 # a [age=90]
 # ├── b [age=65]
-# └── c [age=65]
+# └── c [age=60]
 #     └── c [age=40]
 
 findall(root, lambda node: node.age >= 65)
 # (Node(/a, age=90), Node(/a/b, age=65))
 
 find_names(root, "c")
 # (Node(/a/c, age=60), Node(/a/c/c, age=40))
@@ -558,64 +582,92 @@
 find_paths(root, "/c")  # partial path
 # (Node(/a/c, age=60), Node(/a/c/c, age=40))
 
 find_attrs(root, "age", 40)
 # (Node(/a/c/c, age=40),)
 ```
 
+It is also possible to search for one or more child node(s) based on attributes, and the search will be faster as
+this does not require traversing the whole tree to find the node(s).
+
+```python
+from bigtree import Node, find_children, find_child, find_child_by_name
+root = Node("a", age=90)
+b = Node("b", age=65, parent=root)
+c = Node("c", age=60, parent=root)
+d = Node("c", age=40, parent=c)
+root.show(attr_list=["age"])
+# a [age=90]
+# ├── b [age=65]
+# └── c [age=60]
+#     └── c [age=40]
+
+find_children(root, lambda node: node.age >= 60)
+# (Node(/a/b, age=65), Node(/a/c, age=60))
+
+find_child(root, lambda node: node.name == "c")
+# Node(/a/c, age=60)
+
+find_child_by_name(root, "c")
+# Node(/a/c, age=60)
+
+find_child_by_name(c, "c")
+# Node(/a/c/c, age=40)
+```
+
 ### Helper Utility
 
 There following are helper functions for cloning tree to another `Node` type, pruning tree, and getting difference
 between two trees.
 
 ```python
-from bigtree import BaseNode, Node, print_tree, clone_tree, prune_tree, get_tree_diff
+from bigtree import BaseNode, Node, clone_tree, prune_tree, get_tree_diff
 
 # Cloning tree from `BaseNode` to `Node` type
 root = BaseNode(name="a")
 b = BaseNode(name="b", parent=root)
 clone_tree(root, Node)
 # Node(/a, )
 
 # Prune tree to only path a/b
 root = Node("a")
 b = Node("b", parent=root)
 c = Node("c", parent=root)
-print_tree(root)
+root.show()
 # a
 # ├── b
 # └── c
 
 root_pruned = prune_tree(root, "a/b")
-print_tree(root_pruned)
+root_pruned.show()
 # a
 # └── b
 
 # Get difference between two trees
 root = Node("a")
 b = Node("b", parent=root)
 c = Node("c", parent=root)
-print_tree(root)
+root.show()
 # a
 # ├── b
 # └── c
 
 root_other = Node("a")
 b_other = Node("b", parent=root_other)
-print_tree(root_other)
+root_other.show()
 # a
 # └── b
 
 tree_diff = get_tree_diff(root, root_other)
-print_tree(tree_diff)
+tree_diff.show()
 # a
 # └── c (-)
 
 tree_diff = get_tree_diff(root, root_other, only_diff=False)
-print_tree(tree_diff)
+tree_diff.show()
 # a
 # ├── b
 # └── c (-)
 ```
 
 ### Export Tree
 
@@ -624,22 +676,22 @@
 1. *Export to **nested dictionary***
 2. *Export to **nested recursive dictionary***
 3. *Export to **pandas DataFrame***
 4. *Export to **dot** (and png)*
 5. *Export to **Pillow** (and png)*
 
 ```python
-from bigtree import Node, print_tree, tree_to_dict, tree_to_nested_dict, tree_to_dataframe, tree_to_dot, tree_to_pillow
+from bigtree import Node, tree_to_dict, tree_to_nested_dict, tree_to_dataframe, tree_to_dot, tree_to_pillow
 
 root = Node("a", age=90)
 b = Node("b", age=65, parent=root)
 c = Node("c", age=60, parent=root)
 d = Node("d", age=40, parent=b)
 e = Node("e", age=35, parent=b)
-print_tree(root)
+root.show()
 # a
 # ├── b
 # │   ├── d
 # │   └── e
 # └── c
 
 tree_to_dict(
@@ -745,29 +797,63 @@
 ![Sample DAG Output](https://github.com/kayjan/bigtree/raw/master/assets/demo_binarytree.png)
 
 2. **From *list***
 
 Construct nodes only, list has similar format as `heapq` list.
 
 ```python
-from bigtree import list_to_binarytree, print_tree
+from bigtree import list_to_binarytree
 
 nums_list = [1, 2, 3, 4, 5, 6, 7, 8]
 root = list_to_binarytree(nums_list)
-print_tree(root)
+root.show()
 # 1
 # ├── 2
 # │   ├── 4
 # │   │   └── 8
 # │   └── 5
 # └── 3
 #     ├── 6
 #     └── 7
 ```
 
+### Traverse Binary Tree
+
+In addition to the traversal methods in the usual tree, binary tree includes in-order traversal method.
+
+```python
+from bigtree import list_to_binarytree, inorder_iter, preorder_iter, postorder_iter, levelorder_iter, levelordergroup_iter
+
+nums_list = [1, 2, 3, 4, 5, 6, 7, 8]
+root = list_to_binarytree(nums_list)
+root.show()
+# 1
+# ├── 2
+# │   ├── 4
+# │   │   └── 8
+# │   └── 5
+# └── 3
+#     ├── 6
+#     └── 7
+
+[node.name for node in inorder_iter(root)]
+# ['8', '4', '2', '5', '1', '6', '3', '7']
+
+[node.name for node in preorder_iter(root)]
+# ['1', '2', '4', '8', '5', '3', '6', '7']
+
+[node.name for node in postorder_iter(root)]
+# ['8', '4', '5', '2', '6', '7', '3', '1']
+
+[node.name for node in levelorder_iter(root)]
+# ['1', '2', '3', '4', '5', '6', '7', '8']
+
+[[node.name for node in node_group] for node_group in levelordergroup_iter(root)]
+# [['1'], ['2', '3'], ['4', '5', '6', '7'], ['8']]
+```
 
 ----
 
 ## DAG Demonstration
 
 Compared to nodes in tree, nodes in DAG are able to have multiple parents.
 
@@ -858,17 +944,18 @@
 # [('a', 'd'), ('c', 'd'), ('d', 'e'), ('a', 'c'), ('b', 'c')]
 ```
 
 ----
 
 ## Demo Usage
 
-### To Do Application
+There are existing implementations of workflows to showcase how `bigtree` can be used!
 
-There is existing implementation of a To-Do app to showcase how `bigtree` can be used. There are functions to:
+### To Do Application
+There are functions to:
 - Add or remove list to To-Do application
 - Add or remove item to list, default list is the 'General' list
 - Prioritize a list/item by reordering them as first list/item
 - Save and import To-Do application to and from an external JSON file
 - Show To-Do application, which prints tree to console
 
 ```python
@@ -886,7 +973,45 @@
 # │   └── Bread [description=Urgent]
 # └── General
 #   └── Cook
 
 app.save("list.json")
 app2 = AppToDo.load("list.json")
 ```
+
+### Calendar Application
+
+There are functions to:
+- Add or remove event from Calendar
+- Find event by name, or name and date
+- Display calendar, which prints events to console
+- Export calendar to pandas DataFrame
+
+```python
+import datetime as dt
+from bigtree import Calendar
+calendar = Calendar("My Calendar")
+calendar.add_event("Gym", "2023-01-01 18:00")
+calendar.add_event("Dinner", "2023-01-01", date_format="%Y-%m-%d", budget=20)
+calendar.add_event("Gym", "2023-01-02 18:00")
+calendar.show()
+# My Calendar
+# 2023-01-01 00:00:00 - Dinner (budget: 20)
+# 2023-01-01 18:00:00 - Gym
+# 2023-01-02 18:00:00 - Gym
+
+calendar.find_event("Gym")
+# 2023-01-01 18:00:00 - Gym
+# 2023-01-02 18:00:00 - Gym
+
+calendar.delete_event("Gym", dt.date(2023, 1, 1))
+calendar.show()
+# My Calendar
+# 2023-01-01 00:00:00 - Dinner (budget: 20)
+# 2023-01-02 18:00:00 - Gym
+
+data_calendar = calendar.to_dataframe()
+data_calendar
+#                              path    name        date      time  budget
+# 0  /My Calendar/2023/01/01/Dinner  Dinner  2023-01-01  00:00:00    20.0
+# 1     /My Calendar/2023/01/02/Gym     Gym  2023-01-02  18:00:00     NaN
+```
```

#### html2text {}

```diff
@@ -63,214 +63,254 @@
 prompt: ```shell $ pip install 'bigtree[image]' $ brew install gprof2dot # for
 MacOS $ conda install graphviz # for Windows ``` ---- ## Tree Demonstration
 Here are some codes to get started. ### Construct Tree Nodes can have
 attributes if they are initialized from `Node`, *dictionary*, or *pandas
 DataFrame*. 1. **From `Node`** Nodes can be linked to each other with `parent`
 and `children` setter methods, or using bitshift operator with the convention
 `parent_node >> child_node` or `child_node << parent_node`. ```python from
-bigtree import Node, print_tree, tree_to_dot root = Node("a", age=90) b = Node
-("b", age=65) c = Node("c", age=60) d = Node("d", age=40) root.children = [b,
-c] d.parent = b print_tree(root, attr_list=["age"]) # a [age=90] # âââ b
-[age=65] # â âââ d [age=40] # âââ c [age=60] graph = tree_to_dot
-(root, node_colour="gold") graph.write_png("assets/demo_tree.png") ``` ![Sample
-Tree Output](https://github.com/kayjan/bigtree/raw/master/assets/demo_tree.png)
-```python from bigtree import Node, print_tree root = Node("a", age=90) b =
-Node("b", age=65) c = Node("c", age=60) d = Node("d", age=40) root >> b root >>
-c d << b print_tree(root, attr_list=["age"]) # a [age=90] # âââ b
-[age=65] # â âââ d [age=40] # âââ c [age=60] ``` Alternatively,
-we can directly pass `parent` or `children` argument. ```python from bigtree
-import Node, print_tree root = Node("a") b = Node("b", parent=root) c = Node
-("c", parent=root) d = Node("d", parent=b) print_tree(root, style="ascii") # a
-# |-- b # | +-- d # +-- c ``` ```python from bigtree import Node, print_tree d
-= Node("d") c = Node("c") b = Node("b", children=[d]) root = Node("a",
-children=[b, c]) print_tree(root, style="ascii") # a # |-- b # | +-- d # +-- c
-``` 2. **From *list*** Construct nodes only, list can contain either full paths
-or tuples of parent-child names. ```python from bigtree import list_to_tree,
-list_to_tree_by_relation, print_tree root = list_to_tree(["a/b/d", "a/c"])
-print_tree(root) # a # âââ b # â âââ d # âââ c root =
-list_to_tree_by_relation([("a", "b"), ("a", "c"), ("b", "d")]) print_tree(root)
-# a # âââ b # â âââ d # âââ c ``` 3. **From *nested
+bigtree import Node, tree_to_dot root = Node("a") b = Node("b") c = Node("c") d
+= Node("d") root.children = [b, c] d.parent = b root.show() # a # âââ b #
+â âââ d # âââ c graph = tree_to_dot(root, node_colour="gold")
+graph.write_png("assets/demo_tree.png") ``` ![Sample Tree Output](https://
+github.com/kayjan/bigtree/raw/master/assets/demo_tree.png) ```python from
+bigtree import Node root = Node("a") b = Node("b") c = Node("c") d = Node("d")
+root >> b root >> c d << b root.show() # a # âââ b # â âââ d #
+âââ c ``` Alternatively, we can directly pass `parent` or `children`
+argument. ```python from bigtree import Node b = Node("b") c = Node("c") d =
+Node("d", parent=b) root = Node("a", children=[b, c]) root.show(style="ascii")
+# a # |-- b # | +-- d # +-- c ``` 2. **From *list*** Construct nodes only, list
+can contain either full paths or tuples of parent-child names. ```python from
+bigtree import list_to_tree, list_to_tree_by_relation root = list_to_tree(["a/
+b/d", "a/c"]) root.show() # a # âââ b # â âââ d # âââ c
+root = list_to_tree_by_relation([("a", "b"), ("a", "c"), ("b", "d")]) root.show
+() # a # âââ b # â âââ d # âââ c ``` 3. **From *nested
 dictionary*** Construct nodes with attributes, `key`: path, `value`: dict of
 node attribute names and attribute values. ```python from bigtree import
-dict_to_tree, print_tree path_dict = { "a": {"age": 90}, "a/b": {"age": 65},
-"a/c": {"age": 60}, "a/b/d": {"age": 40}, } root = dict_to_tree(path_dict)
-print_tree(root, attr_list=["age"]) # a [age=90] # âââ b [age=65] # â
-âââ d [age=40] # âââ c [age=60] ``` 4. **From *nested recursive
-dictionary*** Construct nodes with attributes, `key`: node attribute names,
-`value`: node attribute values, and list of children (recursive). ```python
-from bigtree import nested_dict_to_tree, print_tree path_dict = { "name": "a",
-"age": 90, "children": [ { "name": "b", "age": 65, "children": [ {"name": "d",
-"age": 40}, ], }, {"name": "c", "age": 60}, ], } root = nested_dict_to_tree
-(path_dict) print_tree(root, attr_list=["age"]) # a [age=90] # âââ b
-[age=65] # â âââ d [age=40] # âââ c [age=60] ``` 5. **From
-*pandas DataFrame*** Construct nodes with attributes, *pandas DataFrame* can
-contain either path column or parent-child columns, and attribute columns.
-```python import pandas as pd from bigtree import dataframe_to_tree,
-dataframe_to_tree_by_relation, print_tree data = pd.DataFrame( [ ["a", 90],
-["a/b", 65], ["a/c", 60], ["a/b/d", 40], ], columns=["path", "age"], ) root =
-dataframe_to_tree(data) print_tree(root, attr_list=["age"]) # a [age=90] #
-âââ b [age=65] # â âââ d [age=40] # âââ c [age=60] data =
-pd.DataFrame( [ ["a", None, 90], ["b", "a", 65], ["c", "a", 60], ["d", "b",
-40], ], columns=["child", "parent", "age"], ) root =
-dataframe_to_tree_by_relation(data) print_tree(root, attr_list=["age"]) # a
-[age=90] # âââ b [age=65] # â âââ d [age=40] # âââ c
-[age=60] ``` > If tree is already created, attributes can still be added using
-dictionary or pandas DataFrame! ### Print Tree After tree is constructed, it
-can be viewed by printing to console using `print_tree` method. ```python from
-bigtree import Node, print_tree root = Node("a", age=90) b = Node("b", age=65,
-parent=root) c = Node("c", age=60, parent=root) d = Node("d", age=40, parent=b)
-e = Node("e", age=35, parent=b) print_tree(root) # a # âââ b # â
-âââ d # â âââ e # âââ c # Print subtree print_tree(root,
-node_name_or_path="b") # b # âââ d # âââ e print_tree(root,
-max_depth=2) # a # âââ b # âââ c # Print attributes print_tree
-(root, attr_list=["age"]) # a [age=90] # âââ b [age=65] # â âââ d
-[age=40] # â âââ e [age=35] # âââ c [age=60] print_tree(root,
-attr_list=["age"], attr_bracket=["*(", ")"]) # a *(age=90) # âââ b *
-(age=65) # â âââ d *(age=40) # â âââ e *(age=35) # âââ c
-*(age=60) # Available styles print_tree(root, style="ansi") # a # |-- b # | |-
+dict_to_tree path_dict = { "a": {"age": 90}, "a/b": {"age": 65}, "a/c": {"age":
+60}, "a/b/d": {"age": 40}, } root = dict_to_tree(path_dict) root.show
+(attr_list=["age"]) # a [age=90] # âââ b [age=65] # â âââ d
+[age=40] # âââ c [age=60] ``` 4. **From *nested recursive dictionary***
+Construct nodes with attributes, `key`: node attribute names, `value`: node
+attribute values, and list of children (recursive). ```python from bigtree
+import nested_dict_to_tree path_dict = { "name": "a", "age": 90, "children": [
+{ "name": "b", "age": 65, "children": [ {"name": "d", "age": 40}, ], },
+{"name": "c", "age": 60}, ], } root = nested_dict_to_tree(path_dict) root.show
+(attr_list=["age"]) # a [age=90] # âââ b [age=65] # â âââ d
+[age=40] # âââ c [age=60] ``` 5. **From *pandas DataFrame*** Construct
+nodes with attributes, *pandas DataFrame* can contain either path column or
+parent-child columns, and attribute columns. ```python import pandas as pd from
+bigtree import dataframe_to_tree, dataframe_to_tree_by_relation data =
+pd.DataFrame( [ ["a", 90], ["a/b", 65], ["a/c", 60], ["a/b/d", 40], ], columns=
+["path", "age"], ) root = dataframe_to_tree(data) root.show(attr_list=["age"])
+# a [age=90] # âââ b [age=65] # â âââ d [age=40] # âââ c
+[age=60] data = pd.DataFrame( [ ["a", None, 90], ["b", "a", 65], ["c", "a",
+60], ["d", "b", 40], ], columns=["child", "parent", "age"], ) root =
+dataframe_to_tree_by_relation(data) root.show(attr_list=["age"]) # a [age=90] #
+âââ b [age=65] # â âââ d [age=40] # âââ c [age=60] ``` > If
+tree is already created, attributes can still be added using dictionary or
+pandas DataFrame! ### Print Tree After tree is constructed, it can be viewed by
+printing to console using `show` method directly. Alternatively, the
+`print_tree` method can be used. ```python from bigtree import Node, print_tree
+root = Node("a", age=90, gender="F") b = Node("b", age=65, gender="M",
+parent=root) c = Node("c", age=60, gender="M", parent=root) d = Node("d",
+age=40, gender="F", parent=b) e = Node("e", age=35, gender="M", parent=b)
+print_tree(root) # a # âââ b # â âââ d # â âââ e #
+âââ c # Print subtree print_tree(root, node_name_or_path="b") # b #
+âââ d # âââ e print_tree(root, max_depth=2) # a # âââ b #
+âââ c # Print attributes print_tree(root, attr_list=["age"]) # a [age=90]
+# âââ b [age=65] # â âââ d [age=40] # â âââ e [age=35] #
+âââ c [age=60] print_tree(root, attr_list=["age"], attr_bracket=["*(",
+")"]) # a *(age=90) # âââ b *(age=65) # â âââ d *(age=40) # â
+âââ e *(age=35) # âââ c *(age=60) print_tree(root, all_attrs=True)
+# a [age=90, gender=F] # âââ b [age=65, gender=M] # â âââ d
+[age=40, gender=F] # â âââ e [age=35, gender=M] # âââ c [age=60,
+gender=M] # Available styles print_tree(root, style="ansi") # a # |-- b # | |-
 - d # | `-- e # `-- c print_tree(root, style="ascii") # a # |-- b # | |-- d # |
 +-- e # +-- c print_tree(root, style="const") # a # âââ b # â âââ
 d # â âââ e # âââ c print_tree(root, style="const_bold") # a #
 â£ââ b # â â£ââ d # â âââ e # âââ c print_tree(root,
 style="rounded") # a # âââ b # â âââ d # â â°ââ e #
 â°ââ c print_tree(root, style="double") # a # â ââ b # â â ââ
 d # â âââ e # âââ c print_tree( root, style="custom",
 custom_style=("| ", "|-- ", "+-- "), ) # a # |-- b # | |-- d # | +-- e # +-- c
-``` ### Modify Tree Nodes can be shifted or copied from one path to another.
-```python from bigtree import Node, shift_nodes, print_tree root = Node("a") b
-= Node("b", parent=root) c = Node("c", parent=root) d = Node("d", parent=root)
-print_tree(root) # a # âââ b # âââ c # âââ d shift_nodes
-( tree=root, from_paths=["a/c", "a/d"], to_paths=["a/b/c", "a/dummy/d"], )
-print_tree(root) # a # âââ b # â âââ c # âââ dummy #
-âââ d ``` ```python from bigtree import Node, copy_nodes, print_tree root
+``` ### Traverse Tree Tree can be traversed using pre-order, post-order, level-
+order, or level-order-group traversal methods. ```python from bigtree import
+Node, preorder_iter, postorder_iter, levelorder_iter, levelordergroup_iter root
 = Node("a") b = Node("b", parent=root) c = Node("c", parent=root) d = Node("d",
-parent=root) print_tree(root) # a # âââ b # âââ c # âââ d
-copy_nodes( tree=root, from_paths=["a/c", "a/d"], to_paths=["a/b/c", "a/dummy/
-d"], ) print_tree(root) # a # âââ b # â âââ c # âââ c #
-âââ d # âââ dummy # âââ d ``` Nodes can also be copied
-between two different trees. ```python from bigtree import Node,
-copy_nodes_from_tree_to_tree, print_tree root = Node("a") b = Node("b",
-parent=root) c = Node("c", parent=root) d = Node("d", parent=root) print_tree
-(root) # a # âââ b # âââ c # âââ d root_other = Node("aa")
+parent=b) e = Node("e", parent=b) root.show() # a # âââ b # â âââ
+d # â âââ e # âââ c [node.name for node in preorder_iter(root)] #
+['a', 'b', 'd', 'e', 'c'] [node.name for node in postorder_iter(root)] # ['d',
+'e', 'b', 'c', 'a'] [node.name for node in levelorder_iter(root)] # ['a', 'b',
+'c', 'd', 'e'] [[node.name for node in node_group] for node_group in
+levelordergroup_iter(root)] # [['a'], ['b', 'c'], ['d', 'e']] ``` ### Modify
+Tree Nodes can be shifted or copied from one path to another. ```python from
+bigtree import Node, shift_nodes root = Node("a") b = Node("b", parent=root) c
+= Node("c", parent=root) d = Node("d", parent=root) root.show() # a # âââ
+b # âââ c # âââ d shift_nodes( tree=root, from_paths=["a/c", "a/
+d"], to_paths=["a/b/c", "a/dummy/d"], ) root.show() # a # âââ b # â
+âââ c # âââ dummy # âââ d ``` ```python from bigtree import
+Node, copy_nodes root = Node("a") b = Node("b", parent=root) c = Node("c",
+parent=root) d = Node("d", parent=root) root.show() # a # âââ b #
+âââ c # âââ d copy_nodes( tree=root, from_paths=["a/c", "a/d"],
+to_paths=["a/b/c", "a/dummy/d"], ) root.show() # a # âââ b # â
+âââ c # âââ c # âââ d # âââ dummy # âââ d ```
+Nodes can also be copied between two different trees. ```python from bigtree
+import Node, copy_nodes_from_tree_to_tree root = Node("a") b = Node("b",
+parent=root) c = Node("c", parent=root) d = Node("d", parent=root) root.show()
+# a # âââ b # âââ c # âââ d root_other = Node("aa")
 copy_nodes_from_tree_to_tree( from_tree=root, to_tree=root_other, from_paths=
-["a/b", "a/c", "a/d"], to_paths=["aa/b", "aa/b/c", "aa/dummy/d"], ) print_tree
-(root_other) # aa # âââ b # â âââ c # âââ dummy # âââ
-d ``` ### Tree Search One or multiple nodes can be search based on name, path,
-attribute value, or user-defined condition. To find a single node, ```python
-from bigtree import Node, print_tree, find, find_name, find_path,
-find_full_path, find_attr root = Node("a", age=90) b = Node("b", age=65,
-parent=root) c = Node("c", age=60, parent=root) d = Node("d", age=40, parent=c)
-print_tree(root, attr_list=["age"]) # a [age=90] # âââ b [age=65] #
-âââ c [age=60] # âââ d [age=40] find(root, lambda node: node.age ==
-60) # Node(/a/c, age=60) find_name(root, "d") # Node(/a/c/d, age=40) find_path
-(root, "/c/d") # partial path # Node(/a/c/d, age=40) find_full_path(root, "a/c/
-d") # full path # Node(/a/c/d, age=40) find_attr(root, "age", 40) # Node(/a/c/
-d, age=40) ``` To find multiple nodes, ```python from bigtree import Node,
-print_tree, findall, find_names, find_paths, find_attrs root = Node("a",
-age=90) b = Node("b", age=65, parent=root) c = Node("c", age=60, parent=root) d
-= Node("c", age=40, parent=c) print_tree(root, attr_list=["age"]) # a [age=90]
-# âââ b [age=65] # âââ c [age=65] # âââ c [age=40] findall
-(root, lambda node: node.age >= 65) # (Node(/a, age=90), Node(/a/b, age=65))
-find_names(root, "c") # (Node(/a/c, age=60), Node(/a/c/c, age=40)) find_paths
-(root, "/c") # partial path # (Node(/a/c, age=60), Node(/a/c/c, age=40))
-find_attrs(root, "age", 40) # (Node(/a/c/c, age=40),) ``` ### Helper Utility
-There following are helper functions for cloning tree to another `Node` type,
-pruning tree, and getting difference between two trees. ```python from bigtree
-import BaseNode, Node, print_tree, clone_tree, prune_tree, get_tree_diff #
-Cloning tree from `BaseNode` to `Node` type root = BaseNode(name="a") b =
-BaseNode(name="b", parent=root) clone_tree(root, Node) # Node(/a, ) # Prune
-tree to only path a/b root = Node("a") b = Node("b", parent=root) c = Node("c",
-parent=root) print_tree(root) # a # âââ b # âââ c root_pruned =
-prune_tree(root, "a/b") print_tree(root_pruned) # a # âââ b # Get
-difference between two trees root = Node("a") b = Node("b", parent=root) c =
-Node("c", parent=root) print_tree(root) # a # âââ b # âââ c
-root_other = Node("a") b_other = Node("b", parent=root_other) print_tree
-(root_other) # a # âââ b tree_diff = get_tree_diff(root, root_other)
-print_tree(tree_diff) # a # âââ c (-) tree_diff = get_tree_diff(root,
-root_other, only_diff=False) print_tree(tree_diff) # a # âââ b #
-âââ c (-) ``` ### Export Tree Tree can be exported to another data type.
-1. *Export to **nested dictionary*** 2. *Export to **nested recursive
-dictionary*** 3. *Export to **pandas DataFrame*** 4. *Export to **dot** (and
-png)* 5. *Export to **Pillow** (and png)* ```python from bigtree import Node,
-print_tree, tree_to_dict, tree_to_nested_dict, tree_to_dataframe, tree_to_dot,
-tree_to_pillow root = Node("a", age=90) b = Node("b", age=65, parent=root) c =
-Node("c", age=60, parent=root) d = Node("d", age=40, parent=b) e = Node("e",
-age=35, parent=b) print_tree(root) # a # âââ b # â âââ d # â
-âââ e # âââ c tree_to_dict( root, name_key="name",
-parent_key="parent", attr_dict={"age": "person age"} ) # { # '/a': {'name':
-'a', 'parent': None, 'person age': 90}, # '/a/b': {'name': 'b', 'parent': 'a',
-'person age': 65}, # '/a/b/d': {'name': 'd', 'parent': 'b', 'person age': 40},
-# '/a/b/e': {'name': 'e', 'parent': 'b', 'person age': 35}, # '/a/c': {'name':
-'c', 'parent': 'a', 'person age': 60} # } tree_to_nested_dict(root,
-all_attrs=True) # { # 'name': 'a', # 'age': 90, # 'children': [ # { # 'name':
-'b', # 'age': 65, # 'children': [ # { # 'name': 'd', # 'age': 40 # }, # { #
-'name': 'e', # 'age': 35 # } # ] # }, # { # 'name': 'c', # 'age': 60 # } # ] #
-} tree_to_dataframe( root, name_col="name", parent_col="parent",
-path_col="path", attr_dict={"age": "person age"} ) # path name parent person
-age # 0 /a a None 90 # 1 /a/b b a 65 # 2 /a/b/d d b 40 # 3 /a/b/e e b 35 # 4 /
-a/c c a 60 graph = tree_to_dot(root, node_colour="gold") graph.write_png
-("assets/demo.png") pillow_image = tree_to_pillow(root) pillow_image.save
-("assets/demo_pillow.png") ``` - demo.png ![Sample Dot Image Output](https://
-github.com/kayjan/bigtree/raw/master/assets/demo.png) - demo_pillow.png !
-[Sample Pillow Image Output](https://github.com/kayjan/bigtree/raw/master/
-assets/demo_pillow.png) ---- ## Binary Tree Demonstration Compared to nodes in
-tree, nodes in Binary Tree are only allowed maximum of 2 children. Since
-BinaryNode extends from Node, construct, traverse, search, export methods from
-Node are applicable to Binary Tree as well. ### Construct Binary Tree 1. **From
-`BinaryNode`** BinaryNode can be linked to each other with `parent`,
-`children`, `left`, and `right` setter methods, or using bitshift operator with
-the convention `parent_node >> child_node` or `child_node << parent_node`.
-```python from bigtree import BinaryNode, tree_to_dot e = BinaryNode(5) d =
-BinaryNode(4) c = BinaryNode(3) b = BinaryNode(2, left=d, right=e) a =
-BinaryNode(1, children=[b, c]) f = BinaryNode(6, parent=c) g = BinaryNode(7,
-parent=c) h = BinaryNode(8, parent=d) graph = tree_to_dot(a,
-node_colour="gold") graph.write_png("assets/demo_binarytree.png") ``` ![Sample
-DAG Output](https://github.com/kayjan/bigtree/raw/master/assets/
-demo_binarytree.png) 2. **From *list*** Construct nodes only, list has similar
-format as `heapq` list. ```python from bigtree import list_to_binarytree,
-print_tree nums_list = [1, 2, 3, 4, 5, 6, 7, 8] root = list_to_binarytree
-(nums_list) print_tree(root) # 1 # âââ 2 # â âââ 4 # â â
-âââ 8 # â âââ 5 # âââ 3 # âââ 6 # âââ 7 ``` ---
-- ## DAG Demonstration Compared to nodes in tree, nodes in DAG are able to have
-multiple parents. ### Construct DAG 1. **From `DAGNode`** DAGNode can be linked
-to each other with `parents` and `children` setter methods, or using bitshift
-operator with the convention `parent_node >> child_node` or `child_node <<
-parent_node`. ```python from bigtree import DAGNode, dag_to_dot a = DAGNode
-("a") b = DAGNode("b") c = DAGNode("c", parents=[a, b]) d = DAGNode("d",
-parents=[a, c]) e = DAGNode("e", parents=[d]) f = DAGNode("f", parents=[c, d])
-h = DAGNode("h") g = DAGNode("g", parents=[c], children=[h]) graph = dag_to_dot
-(a, node_colour="gold") graph.write_png("assets/demo_dag.png") ``` ![Sample DAG
-Output](https://github.com/kayjan/bigtree/raw/master/assets/demo_dag.png) 2.
-**From *list*** Construct nodes only, list contains parent-child tuples.
-```python from bigtree import list_to_dag, dag_iterator relations_list = [
-("a", "c"), ("a", "d"), ("b", "c"), ("c", "d"), ("d", "e") ] dag = list_to_dag
-(relations_list) print([(parent.node_name, child.node_name) for parent, child
-in dag_iterator(dag)]) # [('a', 'd'), ('c', 'd'), ('d', 'e'), ('a', 'c'), ('b',
-'c')] ``` 3. **From *nested dictionary*** Construct nodes with attributes,
-`key`: child name, `value`: dict of parent name, child node attributes.
-```python from bigtree import dict_to_dag, dag_iterator relation_dict = { "a":
-{"step": 1}, "b": {"step": 1}, "c": {"parents": ["a", "b"], "step": 2}, "d":
-{"parents": ["a", "c"], "step": 2}, "e": {"parents": ["d"], "step": 3}, } dag =
-dict_to_dag(relation_dict, parent_key="parents") print([(parent.node_name,
+["a/b", "a/c", "a/d"], to_paths=["aa/b", "aa/b/c", "aa/dummy/d"], )
+root_other.show() # aa # âââ b # â âââ c # âââ dummy #
+âââ d ``` ### Tree Search One or multiple nodes can be search based on
+name, path, attribute value, or user-defined condition. To find a single node,
+```python from bigtree import Node, find, find_name, find_path, find_full_path,
+find_attr root = Node("a", age=90) b = Node("b", age=65, parent=root) c = Node
+("c", age=60, parent=root) d = Node("d", age=40, parent=c) root.show(attr_list=
+["age"]) # a [age=90] # âââ b [age=65] # âââ c [age=60] # âââ
+d [age=40] find(root, lambda node: node.age == 60) # Node(/a/c, age=60)
+find_name(root, "d") # Node(/a/c/d, age=40) find_path(root, "/c/d") # partial
+path # Node(/a/c/d, age=40) find_full_path(root, "a/c/d") # full path # Node(/
+a/c/d, age=40) find_attr(root, "age", 40) # Node(/a/c/d, age=40) ``` To find
+multiple nodes, ```python from bigtree import Node, findall, find_names,
+find_paths, find_attrs root = Node("a", age=90) b = Node("b", age=65,
+parent=root) c = Node("c", age=60, parent=root) d = Node("c", age=40, parent=c)
+root.show(attr_list=["age"]) # a [age=90] # âââ b [age=65] # âââ c
+[age=60] # âââ c [age=40] findall(root, lambda node: node.age >= 65) #
+(Node(/a, age=90), Node(/a/b, age=65)) find_names(root, "c") # (Node(/a/c,
+age=60), Node(/a/c/c, age=40)) find_paths(root, "/c") # partial path # (Node(/
+a/c, age=60), Node(/a/c/c, age=40)) find_attrs(root, "age", 40) # (Node(/a/c/c,
+age=40),) ``` It is also possible to search for one or more child node(s) based
+on attributes, and the search will be faster as this does not require
+traversing the whole tree to find the node(s). ```python from bigtree import
+Node, find_children, find_child, find_child_by_name root = Node("a", age=90) b
+= Node("b", age=65, parent=root) c = Node("c", age=60, parent=root) d = Node
+("c", age=40, parent=c) root.show(attr_list=["age"]) # a [age=90] # âââ b
+[age=65] # âââ c [age=60] # âââ c [age=40] find_children(root,
+lambda node: node.age >= 60) # (Node(/a/b, age=65), Node(/a/c, age=60))
+find_child(root, lambda node: node.name == "c") # Node(/a/c, age=60)
+find_child_by_name(root, "c") # Node(/a/c, age=60) find_child_by_name(c, "c") #
+Node(/a/c/c, age=40) ``` ### Helper Utility There following are helper
+functions for cloning tree to another `Node` type, pruning tree, and getting
+difference between two trees. ```python from bigtree import BaseNode, Node,
+clone_tree, prune_tree, get_tree_diff # Cloning tree from `BaseNode` to `Node`
+type root = BaseNode(name="a") b = BaseNode(name="b", parent=root) clone_tree
+(root, Node) # Node(/a, ) # Prune tree to only path a/b root = Node("a") b =
+Node("b", parent=root) c = Node("c", parent=root) root.show() # a # âââ b
+# âââ c root_pruned = prune_tree(root, "a/b") root_pruned.show() # a #
+âââ b # Get difference between two trees root = Node("a") b = Node("b",
+parent=root) c = Node("c", parent=root) root.show() # a # âââ b #
+âââ c root_other = Node("a") b_other = Node("b", parent=root_other)
+root_other.show() # a # âââ b tree_diff = get_tree_diff(root, root_other)
+tree_diff.show() # a # âââ c (-) tree_diff = get_tree_diff(root,
+root_other, only_diff=False) tree_diff.show() # a # âââ b # âââ c
+(-) ``` ### Export Tree Tree can be exported to another data type. 1. *Export
+to **nested dictionary*** 2. *Export to **nested recursive dictionary*** 3.
+*Export to **pandas DataFrame*** 4. *Export to **dot** (and png)* 5. *Export to
+**Pillow** (and png)* ```python from bigtree import Node, tree_to_dict,
+tree_to_nested_dict, tree_to_dataframe, tree_to_dot, tree_to_pillow root = Node
+("a", age=90) b = Node("b", age=65, parent=root) c = Node("c", age=60,
+parent=root) d = Node("d", age=40, parent=b) e = Node("e", age=35, parent=b)
+root.show() # a # âââ b # â âââ d # â âââ e # âââ c
+tree_to_dict( root, name_key="name", parent_key="parent", attr_dict={"age":
+"person age"} ) # { # '/a': {'name': 'a', 'parent': None, 'person age': 90}, #
+'/a/b': {'name': 'b', 'parent': 'a', 'person age': 65}, # '/a/b/d': {'name':
+'d', 'parent': 'b', 'person age': 40}, # '/a/b/e': {'name': 'e', 'parent': 'b',
+'person age': 35}, # '/a/c': {'name': 'c', 'parent': 'a', 'person age': 60} # }
+tree_to_nested_dict(root, all_attrs=True) # { # 'name': 'a', # 'age': 90, #
+'children': [ # { # 'name': 'b', # 'age': 65, # 'children': [ # { # 'name':
+'d', # 'age': 40 # }, # { # 'name': 'e', # 'age': 35 # } # ] # }, # { # 'name':
+'c', # 'age': 60 # } # ] # } tree_to_dataframe( root, name_col="name",
+parent_col="parent", path_col="path", attr_dict={"age": "person age"} ) # path
+name parent person age # 0 /a a None 90 # 1 /a/b b a 65 # 2 /a/b/d d b 40 # 3 /
+a/b/e e b 35 # 4 /a/c c a 60 graph = tree_to_dot(root, node_colour="gold")
+graph.write_png("assets/demo.png") pillow_image = tree_to_pillow(root)
+pillow_image.save("assets/demo_pillow.png") ``` - demo.png ![Sample Dot Image
+Output](https://github.com/kayjan/bigtree/raw/master/assets/demo.png) -
+demo_pillow.png ![Sample Pillow Image Output](https://github.com/kayjan/
+bigtree/raw/master/assets/demo_pillow.png) ---- ## Binary Tree Demonstration
+Compared to nodes in tree, nodes in Binary Tree are only allowed maximum of 2
+children. Since BinaryNode extends from Node, construct, traverse, search,
+export methods from Node are applicable to Binary Tree as well. ### Construct
+Binary Tree 1. **From `BinaryNode`** BinaryNode can be linked to each other
+with `parent`, `children`, `left`, and `right` setter methods, or using
+bitshift operator with the convention `parent_node >> child_node` or
+`child_node << parent_node`. ```python from bigtree import BinaryNode,
+tree_to_dot e = BinaryNode(5) d = BinaryNode(4) c = BinaryNode(3) b =
+BinaryNode(2, left=d, right=e) a = BinaryNode(1, children=[b, c]) f =
+BinaryNode(6, parent=c) g = BinaryNode(7, parent=c) h = BinaryNode(8, parent=d)
+graph = tree_to_dot(a, node_colour="gold") graph.write_png("assets/
+demo_binarytree.png") ``` ![Sample DAG Output](https://github.com/kayjan/
+bigtree/raw/master/assets/demo_binarytree.png) 2. **From *list*** Construct
+nodes only, list has similar format as `heapq` list. ```python from bigtree
+import list_to_binarytree nums_list = [1, 2, 3, 4, 5, 6, 7, 8] root =
+list_to_binarytree(nums_list) root.show() # 1 # âââ 2 # â âââ 4 #
+â â âââ 8 # â âââ 5 # âââ 3 # âââ 6 # âââ 7
+``` ### Traverse Binary Tree In addition to the traversal methods in the usual
+tree, binary tree includes in-order traversal method. ```python from bigtree
+import list_to_binarytree, inorder_iter, preorder_iter, postorder_iter,
+levelorder_iter, levelordergroup_iter nums_list = [1, 2, 3, 4, 5, 6, 7, 8] root
+= list_to_binarytree(nums_list) root.show() # 1 # âââ 2 # â âââ 4
+# â â âââ 8 # â âââ 5 # âââ 3 # âââ 6 # âââ
+7 [node.name for node in inorder_iter(root)] # ['8', '4', '2', '5', '1', '6',
+'3', '7'] [node.name for node in preorder_iter(root)] # ['1', '2', '4', '8',
+'5', '3', '6', '7'] [node.name for node in postorder_iter(root)] # ['8', '4',
+'5', '2', '6', '7', '3', '1'] [node.name for node in levelorder_iter(root)] #
+['1', '2', '3', '4', '5', '6', '7', '8'] [[node.name for node in node_group]
+for node_group in levelordergroup_iter(root)] # [['1'], ['2', '3'], ['4', '5',
+'6', '7'], ['8']] ``` ---- ## DAG Demonstration Compared to nodes in tree,
+nodes in DAG are able to have multiple parents. ### Construct DAG 1. **From
+`DAGNode`** DAGNode can be linked to each other with `parents` and `children`
+setter methods, or using bitshift operator with the convention `parent_node >>
+child_node` or `child_node << parent_node`. ```python from bigtree import
+DAGNode, dag_to_dot a = DAGNode("a") b = DAGNode("b") c = DAGNode("c", parents=
+[a, b]) d = DAGNode("d", parents=[a, c]) e = DAGNode("e", parents=[d]) f =
+DAGNode("f", parents=[c, d]) h = DAGNode("h") g = DAGNode("g", parents=[c],
+children=[h]) graph = dag_to_dot(a, node_colour="gold") graph.write_png
+("assets/demo_dag.png") ``` ![Sample DAG Output](https://github.com/kayjan/
+bigtree/raw/master/assets/demo_dag.png) 2. **From *list*** Construct nodes
+only, list contains parent-child tuples. ```python from bigtree import
+list_to_dag, dag_iterator relations_list = [ ("a", "c"), ("a", "d"), ("b",
+"c"), ("c", "d"), ("d", "e") ] dag = list_to_dag(relations_list) print([
+(parent.node_name, child.node_name) for parent, child in dag_iterator(dag)]) #
+[('a', 'd'), ('c', 'd'), ('d', 'e'), ('a', 'c'), ('b', 'c')] ``` 3. **From
+*nested dictionary*** Construct nodes with attributes, `key`: child name,
+`value`: dict of parent name, child node attributes. ```python from bigtree
+import dict_to_dag, dag_iterator relation_dict = { "a": {"step": 1}, "b":
+{"step": 1}, "c": {"parents": ["a", "b"], "step": 2}, "d": {"parents": ["a",
+"c"], "step": 2}, "e": {"parents": ["d"], "step": 3}, } dag = dict_to_dag
+(relation_dict, parent_key="parents") print([(parent.node_name,
 child.node_name) for parent, child in dag_iterator(dag)]) # [('a', 'd'), ('c',
 'd'), ('d', 'e'), ('a', 'c'), ('b', 'c')] ``` 4. **From *pandas DataFrame***
 Construct nodes with attributes, *pandas DataFrame* contains child column,
 parent column, and attribute columns. ```python import pandas as pd from
 bigtree import dataframe_to_dag, dag_iterator path_data = pd.DataFrame([ ["a",
 None, 1], ["b", None, 1], ["c", "a", 2], ["c", "b", 2], ["d", "a", 2], ["d",
 "c", 2], ["e", "d", 3], ], columns=["child", "parent", "step"] ) dag =
 dataframe_to_dag(path_data) print([(parent.node_name, child.node_name) for
 parent, child in dag_iterator(dag)]) # [('a', 'd'), ('c', 'd'), ('d', 'e'),
-('a', 'c'), ('b', 'c')] ``` ---- ## Demo Usage ### To Do Application There is
-existing implementation of a To-Do app to showcase how `bigtree` can be used.
-There are functions to: - Add or remove list to To-Do application - Add or
-remove item to list, default list is the 'General' list - Prioritize a list/
-item by reordering them as first list/item - Save and import To-Do application
-to and from an external JSON file - Show To-Do application, which prints tree
-to console ```python from bigtree import AppToDo app = AppToDo("To Do App")
-app.add_item(item_name="Homework 1", list_name="School") app.add_item
+('a', 'c'), ('b', 'c')] ``` ---- ## Demo Usage There are existing
+implementations of workflows to showcase how `bigtree` can be used! ### To Do
+Application There are functions to: - Add or remove list to To-Do application -
+Add or remove item to list, default list is the 'General' list - Prioritize a
+list/item by reordering them as first list/item - Save and import To-Do
+application to and from an external JSON file - Show To-Do application, which
+prints tree to console ```python from bigtree import AppToDo app = AppToDo("To
+Do App") app.add_item(item_name="Homework 1", list_name="School") app.add_item
 (item_name=["Milk", "Bread"], list_name="Groceries", description="Urgent")
 app.add_item(item_name="Cook") app.show() # To Do App # âââ School # â
 âââ Homework 1 # âââ Groceries # â âââ Milk
 [description=Urgent] # â âââ Bread [description=Urgent] # âââ
 General # âââ Cook app.save("list.json") app2 = AppToDo.load("list.json")
-```
+``` ### Calendar Application There are functions to: - Add or remove event from
+Calendar - Find event by name, or name and date - Display calendar, which
+prints events to console - Export calendar to pandas DataFrame ```python import
+datetime as dt from bigtree import Calendar calendar = Calendar("My Calendar")
+calendar.add_event("Gym", "2023-01-01 18:00") calendar.add_event("Dinner",
+"2023-01-01", date_format="%Y-%m-%d", budget=20) calendar.add_event("Gym",
+"2023-01-02 18:00") calendar.show() # My Calendar # 2023-01-01 00:00:00 -
+Dinner (budget: 20) # 2023-01-01 18:00:00 - Gym # 2023-01-02 18:00:00 - Gym
+calendar.find_event("Gym") # 2023-01-01 18:00:00 - Gym # 2023-01-02 18:00:00 -
+Gym calendar.delete_event("Gym", dt.date(2023, 1, 1)) calendar.show() # My
+Calendar # 2023-01-01 00:00:00 - Dinner (budget: 20) # 2023-01-02 18:00:00 -
+Gym data_calendar = calendar.to_dataframe() data_calendar # path name date time
+budget # 0 /My Calendar/2023/01/01/Dinner Dinner 2023-01-01 00:00:00 20.0 # 1 /
+My Calendar/2023/01/02/Gym Gym 2023-01-02 18:00:00 NaN ```
```

### Comparing `bigtree-0.9.1/pyproject.toml` & `bigtree-0.9.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.1/PKG-INFO` & `bigtree-0.9.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigtree
-Version: 0.9.1
+Version: 0.9.2
 Summary: Tree Implementation for Python, integrated with Python list, dictionary, and pandas DataFrame.
 Project-URL: Documentation, https://bigtree.readthedocs.io
 Project-URL: Issues, https://github.com/kayjan/bigtree/issues
 Project-URL: Source, https://github.com/kayjan/bigtree
 Author-email: Kay Jan <kayjanw@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -143,139 +143,123 @@
 
 1. **From `Node`**
 
 Nodes can be linked to each other with `parent` and `children` setter methods,
 or using bitshift operator with the convention `parent_node >> child_node` or `child_node << parent_node`.
 
 ```python
-from bigtree import Node, print_tree, tree_to_dot
+from bigtree import Node, tree_to_dot
 
-root = Node("a", age=90)
-b = Node("b", age=65)
-c = Node("c", age=60)
-d = Node("d", age=40)
+root = Node("a")
+b = Node("b")
+c = Node("c")
+d = Node("d")
 
 root.children = [b, c]
 d.parent = b
 
-print_tree(root, attr_list=["age"])
-# a [age=90]
-# ├── b [age=65]
-# │   └── d [age=40]
-# └── c [age=60]
+root.show()
+# a
+# ├── b
+# │   └── d
+# └── c
 
 graph = tree_to_dot(root, node_colour="gold")
 graph.write_png("assets/demo_tree.png")
 ```
 
 ![Sample Tree Output](https://github.com/kayjan/bigtree/raw/master/assets/demo_tree.png)
 
 ```python
-from bigtree import Node, print_tree
+from bigtree import Node
 
-root = Node("a", age=90)
-b = Node("b", age=65)
-c = Node("c", age=60)
-d = Node("d", age=40)
+root = Node("a")
+b = Node("b")
+c = Node("c")
+d = Node("d")
 
 root >> b
 root >> c
 d << b
 
-print_tree(root, attr_list=["age"])
-# a [age=90]
-# ├── b [age=65]
-# │   └── d [age=40]
-# └── c [age=60]
+root.show()
+# a
+# ├── b
+# │   └── d
+# └── c
 ```
 
 Alternatively, we can directly pass `parent` or `children` argument.
 
 ```python
-from bigtree import Node, print_tree
+from bigtree import Node
 
-root = Node("a")
-b = Node("b", parent=root)
-c = Node("c", parent=root)
-d = Node("d", parent=b)
-
-print_tree(root, style="ascii")
-# a
-# |-- b
-# |   +-- d
-# +-- c
-```
-
-```python
-from bigtree import Node, print_tree
-
-d = Node("d")
+b = Node("b")
 c = Node("c")
-b = Node("b", children=[d])
+d = Node("d", parent=b)
 root = Node("a", children=[b, c])
 
-print_tree(root, style="ascii")
+root.show(style="ascii")
 # a
 # |-- b
 # |   +-- d
 # +-- c
 ```
 
 2. **From *list***
 
 Construct nodes only, list can contain either full paths or tuples of parent-child names.
 
 ```python
-from bigtree import list_to_tree, list_to_tree_by_relation, print_tree
+from bigtree import list_to_tree, list_to_tree_by_relation
 
 root = list_to_tree(["a/b/d", "a/c"])
-
-print_tree(root)
+root.show()
 # a
 # ├── b
 # │   └── d
 # └── c
 
 root = list_to_tree_by_relation([("a", "b"), ("a", "c"), ("b", "d")])
-print_tree(root)
+root.show()
 # a
 # ├── b
 # │   └── d
 # └── c
 ```
 
 3. **From *nested dictionary***
 
 Construct nodes with attributes, `key`: path, `value`: dict of node attribute names and attribute values.
 
 ```python
-from bigtree import dict_to_tree, print_tree
+from bigtree import dict_to_tree
 
 path_dict = {
    "a": {"age": 90},
    "a/b": {"age": 65},
    "a/c": {"age": 60},
    "a/b/d": {"age": 40},
 }
-root = dict_to_tree(path_dict)
 
-print_tree(root, attr_list=["age"])
+root = dict_to_tree(path_dict)
+root.show(attr_list=["age"])
 # a [age=90]
 # ├── b [age=65]
 # │   └── d [age=40]
 # └── c [age=60]
 ```
 
 4. **From *nested recursive dictionary***
 
 Construct nodes with attributes, `key`: node attribute names, `value`: node attribute values, and list of
 children (recursive).
 
 ```python
-from bigtree import nested_dict_to_tree, print_tree
+from bigtree import nested_dict_to_tree
 
 path_dict = {
    "name": "a",
    "age": 90,
    "children": [
       {
          "name": "b",
@@ -283,82 +267,83 @@
          "children": [
             {"name": "d", "age": 40},
          ],
       },
       {"name": "c", "age": 60},
    ],
 }
-root = nested_dict_to_tree(path_dict)
 
-print_tree(root, attr_list=["age"])
+root = nested_dict_to_tree(path_dict)
+root.show(attr_list=["age"])
 # a [age=90]
 # ├── b [age=65]
 # │   └── d [age=40]
 # └── c [age=60]
 ```
 
 5. **From *pandas DataFrame***
 
 Construct nodes with attributes, *pandas DataFrame* can contain either path column or parent-child columns,
 and attribute columns.
 
 ```python
 import pandas as pd
 
-from bigtree import dataframe_to_tree, dataframe_to_tree_by_relation, print_tree
+from bigtree import dataframe_to_tree, dataframe_to_tree_by_relation
 
 data = pd.DataFrame(
    [
       ["a", 90],
       ["a/b", 65],
       ["a/c", 60],
       ["a/b/d", 40],
    ],
    columns=["path", "age"],
 )
-root = dataframe_to_tree(data)
 
-print_tree(root, attr_list=["age"])
+root = dataframe_to_tree(data)
+root.show(attr_list=["age"])
 # a [age=90]
 # ├── b [age=65]
 # │   └── d [age=40]
 # └── c [age=60]
 
 data = pd.DataFrame(
    [
       ["a", None, 90],
       ["b", "a", 65],
       ["c", "a", 60],
       ["d", "b", 40],
    ],
    columns=["child", "parent", "age"],
 )
-root = dataframe_to_tree_by_relation(data)
 
-print_tree(root, attr_list=["age"])
+root = dataframe_to_tree_by_relation(data)
+root.show(attr_list=["age"])
 # a [age=90]
 # ├── b [age=65]
 # │   └── d [age=40]
 # └── c [age=60]
 ```
 
 > If tree is already created, attributes can still be added using dictionary or pandas DataFrame!
 
 ### Print Tree
 
-After tree is constructed, it can be viewed by printing to console using `print_tree` method.
+After tree is constructed, it can be viewed by printing to console using `show` method directly.
+Alternatively, the `print_tree` method can be used.
 
 ```python
 from bigtree import Node, print_tree
 
-root = Node("a", age=90)
-b = Node("b", age=65, parent=root)
-c = Node("c", age=60, parent=root)
-d = Node("d", age=40, parent=b)
-e = Node("e", age=35, parent=b)
+root = Node("a", age=90, gender="F")
+b = Node("b", age=65, gender="M", parent=root)
+c = Node("c", age=60, gender="M", parent=root)
+d = Node("d", age=40, gender="F", parent=b)
+e = Node("e", age=35, gender="M", parent=b)
 print_tree(root)
 # a
 # ├── b
 # │   ├── d
 # │   └── e
 # └── c
 
@@ -384,14 +369,21 @@
 print_tree(root, attr_list=["age"], attr_bracket=["*(", ")"])
 # a *(age=90)
 # ├── b *(age=65)
 # │   ├── d *(age=40)
 # │   └── e *(age=35)
 # └── c *(age=60)
 
+print_tree(root, all_attrs=True)
+# a [age=90, gender=F]
+# ├── b [age=65, gender=M]
+# │   ├── d [age=40, gender=F]
+# │   └── e [age=35, gender=M]
+# └── c [age=60, gender=M]
+
 # Available styles
 print_tree(root, style="ansi")
 # a
 # |-- b
 # |   |-- d
 # |   `-- e
 # `-- c
@@ -439,113 +431,145 @@
 # a
 # |-- b
 # |   |-- d
 # |   +-- e
 # +-- c
 ```
 
+### Traverse Tree
+
+Tree can be traversed using pre-order, post-order, level-order, or level-order-group traversal methods.
+
+```python
+from bigtree import Node, preorder_iter, postorder_iter, levelorder_iter, levelordergroup_iter
+
+root = Node("a")
+b = Node("b", parent=root)
+c = Node("c", parent=root)
+d = Node("d", parent=b)
+e = Node("e", parent=b)
+root.show()
+# a
+# ├── b
+# │   ├── d
+# │   └── e
+# └── c
+
+[node.name for node in preorder_iter(root)]
+# ['a', 'b', 'd', 'e', 'c']
+
+[node.name for node in postorder_iter(root)]
+# ['d', 'e', 'b', 'c', 'a']
+
+[node.name for node in levelorder_iter(root)]
+# ['a', 'b', 'c', 'd', 'e']
+
+[[node.name for node in node_group] for node_group in levelordergroup_iter(root)]
+# [['a'], ['b', 'c'], ['d', 'e']]
+```
+
 ### Modify Tree
 
 Nodes can be shifted or copied from one path to another.
 
 ```python
-from bigtree import Node, shift_nodes, print_tree
+from bigtree import Node, shift_nodes
 
 root = Node("a")
 b = Node("b", parent=root)
 c = Node("c", parent=root)
 d = Node("d", parent=root)
-print_tree(root)
+root.show()
 # a
 # ├── b
 # ├── c
 # └── d
 
 shift_nodes(
    tree=root,
    from_paths=["a/c", "a/d"],
    to_paths=["a/b/c", "a/dummy/d"],
 )
-print_tree(root)
+root.show()
 # a
 # ├── b
 # │   └── c
 # └── dummy
 #     └── d
 ```
 
 ```python
-from bigtree import Node, copy_nodes, print_tree
+from bigtree import Node, copy_nodes
 
 root = Node("a")
 b = Node("b", parent=root)
 c = Node("c", parent=root)
 d = Node("d", parent=root)
-print_tree(root)
+root.show()
 # a
 # ├── b
 # ├── c
 # └── d
 
 copy_nodes(
    tree=root,
    from_paths=["a/c", "a/d"],
    to_paths=["a/b/c", "a/dummy/d"],
 )
-print_tree(root)
+root.show()
 # a
 # ├── b
 # │   └── c
 # ├── c
 # ├── d
 # └── dummy
 #     └── d
 ```
 
 Nodes can also be copied between two different trees.
 
 ```python
-from bigtree import Node, copy_nodes_from_tree_to_tree, print_tree
+from bigtree import Node, copy_nodes_from_tree_to_tree
 root = Node("a")
 b = Node("b", parent=root)
 c = Node("c", parent=root)
 d = Node("d", parent=root)
-print_tree(root)
+root.show()
 # a
 # ├── b
 # ├── c
 # └── d
 
 root_other = Node("aa")
 copy_nodes_from_tree_to_tree(
    from_tree=root,
    to_tree=root_other,
    from_paths=["a/b", "a/c", "a/d"],
    to_paths=["aa/b", "aa/b/c", "aa/dummy/d"],
 )
-print_tree(root_other)
+root_other.show()
 # aa
 # ├── b
 # │   └── c
 # └── dummy
 #     └── d
 ```
 
 ### Tree Search
 
 One or multiple nodes can be search based on name, path, attribute value, or user-defined condition.
 
 To find a single node,
 ```python
-from bigtree import Node, print_tree, find, find_name, find_path, find_full_path, find_attr
+from bigtree import Node, find, find_name, find_path, find_full_path, find_attr
 root = Node("a", age=90)
 b = Node("b", age=65, parent=root)
 c = Node("c", age=60, parent=root)
 d = Node("d", age=40, parent=c)
-print_tree(root, attr_list=["age"])
+root.show(attr_list=["age"])
 # a [age=90]
 # ├── b [age=65]
 # └── c [age=60]
 #     └── d [age=40]
 
 find(root, lambda node: node.age == 60)
 # Node(/a/c, age=60)
@@ -561,23 +585,23 @@
 
 find_attr(root, "age", 40)
 # Node(/a/c/d, age=40)
 ```
 
 To find multiple nodes,
 ```python
-from bigtree import Node, print_tree, findall, find_names, find_paths, find_attrs
+from bigtree import Node, findall, find_names, find_paths, find_attrs
 root = Node("a", age=90)
 b = Node("b", age=65, parent=root)
 c = Node("c", age=60, parent=root)
 d = Node("c", age=40, parent=c)
-print_tree(root, attr_list=["age"])
+root.show(attr_list=["age"])
 # a [age=90]
 # ├── b [age=65]
-# └── c [age=65]
+# └── c [age=60]
 #     └── c [age=40]
 
 findall(root, lambda node: node.age >= 65)
 # (Node(/a, age=90), Node(/a/b, age=65))
 
 find_names(root, "c")
 # (Node(/a/c, age=60), Node(/a/c/c, age=40))
@@ -585,64 +609,92 @@
 find_paths(root, "/c")  # partial path
 # (Node(/a/c, age=60), Node(/a/c/c, age=40))
 
 find_attrs(root, "age", 40)
 # (Node(/a/c/c, age=40),)
 ```
 
+It is also possible to search for one or more child node(s) based on attributes, and the search will be faster as
+this does not require traversing the whole tree to find the node(s).
+
+```python
+from bigtree import Node, find_children, find_child, find_child_by_name
+root = Node("a", age=90)
+b = Node("b", age=65, parent=root)
+c = Node("c", age=60, parent=root)
+d = Node("c", age=40, parent=c)
+root.show(attr_list=["age"])
+# a [age=90]
+# ├── b [age=65]
+# └── c [age=60]
+#     └── c [age=40]
+
+find_children(root, lambda node: node.age >= 60)
+# (Node(/a/b, age=65), Node(/a/c, age=60))
+
+find_child(root, lambda node: node.name == "c")
+# Node(/a/c, age=60)
+
+find_child_by_name(root, "c")
+# Node(/a/c, age=60)
+
+find_child_by_name(c, "c")
+# Node(/a/c/c, age=40)
+```
+
 ### Helper Utility
 
 There following are helper functions for cloning tree to another `Node` type, pruning tree, and getting difference
 between two trees.
 
 ```python
-from bigtree import BaseNode, Node, print_tree, clone_tree, prune_tree, get_tree_diff
+from bigtree import BaseNode, Node, clone_tree, prune_tree, get_tree_diff
 
 # Cloning tree from `BaseNode` to `Node` type
 root = BaseNode(name="a")
 b = BaseNode(name="b", parent=root)
 clone_tree(root, Node)
 # Node(/a, )
 
 # Prune tree to only path a/b
 root = Node("a")
 b = Node("b", parent=root)
 c = Node("c", parent=root)
-print_tree(root)
+root.show()
 # a
 # ├── b
 # └── c
 
 root_pruned = prune_tree(root, "a/b")
-print_tree(root_pruned)
+root_pruned.show()
 # a
 # └── b
 
 # Get difference between two trees
 root = Node("a")
 b = Node("b", parent=root)
 c = Node("c", parent=root)
-print_tree(root)
+root.show()
 # a
 # ├── b
 # └── c
 
 root_other = Node("a")
 b_other = Node("b", parent=root_other)
-print_tree(root_other)
+root_other.show()
 # a
 # └── b
 
 tree_diff = get_tree_diff(root, root_other)
-print_tree(tree_diff)
+tree_diff.show()
 # a
 # └── c (-)
 
 tree_diff = get_tree_diff(root, root_other, only_diff=False)
-print_tree(tree_diff)
+tree_diff.show()
 # a
 # ├── b
 # └── c (-)
 ```
 
 ### Export Tree
 
@@ -651,22 +703,22 @@
 1. *Export to **nested dictionary***
 2. *Export to **nested recursive dictionary***
 3. *Export to **pandas DataFrame***
 4. *Export to **dot** (and png)*
 5. *Export to **Pillow** (and png)*
 
 ```python
-from bigtree import Node, print_tree, tree_to_dict, tree_to_nested_dict, tree_to_dataframe, tree_to_dot, tree_to_pillow
+from bigtree import Node, tree_to_dict, tree_to_nested_dict, tree_to_dataframe, tree_to_dot, tree_to_pillow
 
 root = Node("a", age=90)
 b = Node("b", age=65, parent=root)
 c = Node("c", age=60, parent=root)
 d = Node("d", age=40, parent=b)
 e = Node("e", age=35, parent=b)
-print_tree(root)
+root.show()
 # a
 # ├── b
 # │   ├── d
 # │   └── e
 # └── c
 
 tree_to_dict(
@@ -772,29 +824,63 @@
 ![Sample DAG Output](https://github.com/kayjan/bigtree/raw/master/assets/demo_binarytree.png)
 
 2. **From *list***
 
 Construct nodes only, list has similar format as `heapq` list.
 
 ```python
-from bigtree import list_to_binarytree, print_tree
+from bigtree import list_to_binarytree
 
 nums_list = [1, 2, 3, 4, 5, 6, 7, 8]
 root = list_to_binarytree(nums_list)
-print_tree(root)
+root.show()
 # 1
 # ├── 2
 # │   ├── 4
 # │   │   └── 8
 # │   └── 5
 # └── 3
 #     ├── 6
 #     └── 7
 ```
 
+### Traverse Binary Tree
+
+In addition to the traversal methods in the usual tree, binary tree includes in-order traversal method.
+
+```python
+from bigtree import list_to_binarytree, inorder_iter, preorder_iter, postorder_iter, levelorder_iter, levelordergroup_iter
+
+nums_list = [1, 2, 3, 4, 5, 6, 7, 8]
+root = list_to_binarytree(nums_list)
+root.show()
+# 1
+# ├── 2
+# │   ├── 4
+# │   │   └── 8
+# │   └── 5
+# └── 3
+#     ├── 6
+#     └── 7
+
+[node.name for node in inorder_iter(root)]
+# ['8', '4', '2', '5', '1', '6', '3', '7']
+
+[node.name for node in preorder_iter(root)]
+# ['1', '2', '4', '8', '5', '3', '6', '7']
+
+[node.name for node in postorder_iter(root)]
+# ['8', '4', '5', '2', '6', '7', '3', '1']
+
+[node.name for node in levelorder_iter(root)]
+# ['1', '2', '3', '4', '5', '6', '7', '8']
+
+[[node.name for node in node_group] for node_group in levelordergroup_iter(root)]
+# [['1'], ['2', '3'], ['4', '5', '6', '7'], ['8']]
+```
 
 ----
 
 ## DAG Demonstration
 
 Compared to nodes in tree, nodes in DAG are able to have multiple parents.
 
@@ -885,17 +971,18 @@
 # [('a', 'd'), ('c', 'd'), ('d', 'e'), ('a', 'c'), ('b', 'c')]
 ```
 
 ----
 
 ## Demo Usage
 
-### To Do Application
+There are existing implementations of workflows to showcase how `bigtree` can be used!
 
-There is existing implementation of a To-Do app to showcase how `bigtree` can be used. There are functions to:
+### To Do Application
+There are functions to:
 - Add or remove list to To-Do application
 - Add or remove item to list, default list is the 'General' list
 - Prioritize a list/item by reordering them as first list/item
 - Save and import To-Do application to and from an external JSON file
 - Show To-Do application, which prints tree to console
 
 ```python
@@ -913,7 +1000,45 @@
 # │   └── Bread [description=Urgent]
 # └── General
 #   └── Cook
 
 app.save("list.json")
 app2 = AppToDo.load("list.json")
 ```
+
+### Calendar Application
+
+There are functions to:
+- Add or remove event from Calendar
+- Find event by name, or name and date
+- Display calendar, which prints events to console
+- Export calendar to pandas DataFrame
+
+```python
+import datetime as dt
+from bigtree import Calendar
+calendar = Calendar("My Calendar")
+calendar.add_event("Gym", "2023-01-01 18:00")
+calendar.add_event("Dinner", "2023-01-01", date_format="%Y-%m-%d", budget=20)
+calendar.add_event("Gym", "2023-01-02 18:00")
+calendar.show()
+# My Calendar
+# 2023-01-01 00:00:00 - Dinner (budget: 20)
+# 2023-01-01 18:00:00 - Gym
+# 2023-01-02 18:00:00 - Gym
+
+calendar.find_event("Gym")
+# 2023-01-01 18:00:00 - Gym
+# 2023-01-02 18:00:00 - Gym
+
+calendar.delete_event("Gym", dt.date(2023, 1, 1))
+calendar.show()
+# My Calendar
+# 2023-01-01 00:00:00 - Dinner (budget: 20)
+# 2023-01-02 18:00:00 - Gym
+
+data_calendar = calendar.to_dataframe()
+data_calendar
+#                              path    name        date      time  budget
+# 0  /My Calendar/2023/01/01/Dinner  Dinner  2023-01-01  00:00:00    20.0
+# 1     /My Calendar/2023/01/02/Gym     Gym  2023-01-02  18:00:00     NaN
+```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bigtree Version: 0.9.1 Summary: Tree Implementation
+Metadata-Version: 2.1 Name: bigtree Version: 0.9.2 Summary: Tree Implementation
 for Python, integrated with Python list, dictionary, and pandas DataFrame.
 Project-URL: Documentation, https://bigtree.readthedocs.io Project-URL: Issues,
 https://github.com/kayjan/bigtree/issues Project-URL: Source, https://
 github.com/kayjan/bigtree Author-email: Kay Jan
 gmail.com> License-Expression: MIT License-File: LICENSE Keywords: bigtree,tree
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3.7 Classifier:
@@ -78,214 +78,254 @@
 prompt: ```shell $ pip install 'bigtree[image]' $ brew install gprof2dot # for
 MacOS $ conda install graphviz # for Windows ``` ---- ## Tree Demonstration
 Here are some codes to get started. ### Construct Tree Nodes can have
 attributes if they are initialized from `Node`, *dictionary*, or *pandas
 DataFrame*. 1. **From `Node`** Nodes can be linked to each other with `parent`
 and `children` setter methods, or using bitshift operator with the convention
 `parent_node >> child_node` or `child_node << parent_node`. ```python from
-bigtree import Node, print_tree, tree_to_dot root = Node("a", age=90) b = Node
-("b", age=65) c = Node("c", age=60) d = Node("d", age=40) root.children = [b,
-c] d.parent = b print_tree(root, attr_list=["age"]) # a [age=90] # âââ b
-[age=65] # â âââ d [age=40] # âââ c [age=60] graph = tree_to_dot
-(root, node_colour="gold") graph.write_png("assets/demo_tree.png") ``` ![Sample
-Tree Output](https://github.com/kayjan/bigtree/raw/master/assets/demo_tree.png)
-```python from bigtree import Node, print_tree root = Node("a", age=90) b =
-Node("b", age=65) c = Node("c", age=60) d = Node("d", age=40) root >> b root >>
-c d << b print_tree(root, attr_list=["age"]) # a [age=90] # âââ b
-[age=65] # â âââ d [age=40] # âââ c [age=60] ``` Alternatively,
-we can directly pass `parent` or `children` argument. ```python from bigtree
-import Node, print_tree root = Node("a") b = Node("b", parent=root) c = Node
-("c", parent=root) d = Node("d", parent=b) print_tree(root, style="ascii") # a
-# |-- b # | +-- d # +-- c ``` ```python from bigtree import Node, print_tree d
-= Node("d") c = Node("c") b = Node("b", children=[d]) root = Node("a",
-children=[b, c]) print_tree(root, style="ascii") # a # |-- b # | +-- d # +-- c
-``` 2. **From *list*** Construct nodes only, list can contain either full paths
-or tuples of parent-child names. ```python from bigtree import list_to_tree,
-list_to_tree_by_relation, print_tree root = list_to_tree(["a/b/d", "a/c"])
-print_tree(root) # a # âââ b # â âââ d # âââ c root =
-list_to_tree_by_relation([("a", "b"), ("a", "c"), ("b", "d")]) print_tree(root)
-# a # âââ b # â âââ d # âââ c ``` 3. **From *nested
+bigtree import Node, tree_to_dot root = Node("a") b = Node("b") c = Node("c") d
+= Node("d") root.children = [b, c] d.parent = b root.show() # a # âââ b #
+â âââ d # âââ c graph = tree_to_dot(root, node_colour="gold")
+graph.write_png("assets/demo_tree.png") ``` ![Sample Tree Output](https://
+github.com/kayjan/bigtree/raw/master/assets/demo_tree.png) ```python from
+bigtree import Node root = Node("a") b = Node("b") c = Node("c") d = Node("d")
+root >> b root >> c d << b root.show() # a # âââ b # â âââ d #
+âââ c ``` Alternatively, we can directly pass `parent` or `children`
+argument. ```python from bigtree import Node b = Node("b") c = Node("c") d =
+Node("d", parent=b) root = Node("a", children=[b, c]) root.show(style="ascii")
+# a # |-- b # | +-- d # +-- c ``` 2. **From *list*** Construct nodes only, list
+can contain either full paths or tuples of parent-child names. ```python from
+bigtree import list_to_tree, list_to_tree_by_relation root = list_to_tree(["a/
+b/d", "a/c"]) root.show() # a # âââ b # â âââ d # âââ c
+root = list_to_tree_by_relation([("a", "b"), ("a", "c"), ("b", "d")]) root.show
+() # a # âââ b # â âââ d # âââ c ``` 3. **From *nested
 dictionary*** Construct nodes with attributes, `key`: path, `value`: dict of
 node attribute names and attribute values. ```python from bigtree import
-dict_to_tree, print_tree path_dict = { "a": {"age": 90}, "a/b": {"age": 65},
-"a/c": {"age": 60}, "a/b/d": {"age": 40}, } root = dict_to_tree(path_dict)
-print_tree(root, attr_list=["age"]) # a [age=90] # âââ b [age=65] # â
-âââ d [age=40] # âââ c [age=60] ``` 4. **From *nested recursive
-dictionary*** Construct nodes with attributes, `key`: node attribute names,
-`value`: node attribute values, and list of children (recursive). ```python
-from bigtree import nested_dict_to_tree, print_tree path_dict = { "name": "a",
-"age": 90, "children": [ { "name": "b", "age": 65, "children": [ {"name": "d",
-"age": 40}, ], }, {"name": "c", "age": 60}, ], } root = nested_dict_to_tree
-(path_dict) print_tree(root, attr_list=["age"]) # a [age=90] # âââ b
-[age=65] # â âââ d [age=40] # âââ c [age=60] ``` 5. **From
-*pandas DataFrame*** Construct nodes with attributes, *pandas DataFrame* can
-contain either path column or parent-child columns, and attribute columns.
-```python import pandas as pd from bigtree import dataframe_to_tree,
-dataframe_to_tree_by_relation, print_tree data = pd.DataFrame( [ ["a", 90],
-["a/b", 65], ["a/c", 60], ["a/b/d", 40], ], columns=["path", "age"], ) root =
-dataframe_to_tree(data) print_tree(root, attr_list=["age"]) # a [age=90] #
-âââ b [age=65] # â âââ d [age=40] # âââ c [age=60] data =
-pd.DataFrame( [ ["a", None, 90], ["b", "a", 65], ["c", "a", 60], ["d", "b",
-40], ], columns=["child", "parent", "age"], ) root =
-dataframe_to_tree_by_relation(data) print_tree(root, attr_list=["age"]) # a
-[age=90] # âââ b [age=65] # â âââ d [age=40] # âââ c
-[age=60] ``` > If tree is already created, attributes can still be added using
-dictionary or pandas DataFrame! ### Print Tree After tree is constructed, it
-can be viewed by printing to console using `print_tree` method. ```python from
-bigtree import Node, print_tree root = Node("a", age=90) b = Node("b", age=65,
-parent=root) c = Node("c", age=60, parent=root) d = Node("d", age=40, parent=b)
-e = Node("e", age=35, parent=b) print_tree(root) # a # âââ b # â
-âââ d # â âââ e # âââ c # Print subtree print_tree(root,
-node_name_or_path="b") # b # âââ d # âââ e print_tree(root,
-max_depth=2) # a # âââ b # âââ c # Print attributes print_tree
-(root, attr_list=["age"]) # a [age=90] # âââ b [age=65] # â âââ d
-[age=40] # â âââ e [age=35] # âââ c [age=60] print_tree(root,
-attr_list=["age"], attr_bracket=["*(", ")"]) # a *(age=90) # âââ b *
-(age=65) # â âââ d *(age=40) # â âââ e *(age=35) # âââ c
-*(age=60) # Available styles print_tree(root, style="ansi") # a # |-- b # | |-
+dict_to_tree path_dict = { "a": {"age": 90}, "a/b": {"age": 65}, "a/c": {"age":
+60}, "a/b/d": {"age": 40}, } root = dict_to_tree(path_dict) root.show
+(attr_list=["age"]) # a [age=90] # âââ b [age=65] # â âââ d
+[age=40] # âââ c [age=60] ``` 4. **From *nested recursive dictionary***
+Construct nodes with attributes, `key`: node attribute names, `value`: node
+attribute values, and list of children (recursive). ```python from bigtree
+import nested_dict_to_tree path_dict = { "name": "a", "age": 90, "children": [
+{ "name": "b", "age": 65, "children": [ {"name": "d", "age": 40}, ], },
+{"name": "c", "age": 60}, ], } root = nested_dict_to_tree(path_dict) root.show
+(attr_list=["age"]) # a [age=90] # âââ b [age=65] # â âââ d
+[age=40] # âââ c [age=60] ``` 5. **From *pandas DataFrame*** Construct
+nodes with attributes, *pandas DataFrame* can contain either path column or
+parent-child columns, and attribute columns. ```python import pandas as pd from
+bigtree import dataframe_to_tree, dataframe_to_tree_by_relation data =
+pd.DataFrame( [ ["a", 90], ["a/b", 65], ["a/c", 60], ["a/b/d", 40], ], columns=
+["path", "age"], ) root = dataframe_to_tree(data) root.show(attr_list=["age"])
+# a [age=90] # âââ b [age=65] # â âââ d [age=40] # âââ c
+[age=60] data = pd.DataFrame( [ ["a", None, 90], ["b", "a", 65], ["c", "a",
+60], ["d", "b", 40], ], columns=["child", "parent", "age"], ) root =
+dataframe_to_tree_by_relation(data) root.show(attr_list=["age"]) # a [age=90] #
+âââ b [age=65] # â âââ d [age=40] # âââ c [age=60] ``` > If
+tree is already created, attributes can still be added using dictionary or
+pandas DataFrame! ### Print Tree After tree is constructed, it can be viewed by
+printing to console using `show` method directly. Alternatively, the
+`print_tree` method can be used. ```python from bigtree import Node, print_tree
+root = Node("a", age=90, gender="F") b = Node("b", age=65, gender="M",
+parent=root) c = Node("c", age=60, gender="M", parent=root) d = Node("d",
+age=40, gender="F", parent=b) e = Node("e", age=35, gender="M", parent=b)
+print_tree(root) # a # âââ b # â âââ d # â âââ e #
+âââ c # Print subtree print_tree(root, node_name_or_path="b") # b #
+âââ d # âââ e print_tree(root, max_depth=2) # a # âââ b #
+âââ c # Print attributes print_tree(root, attr_list=["age"]) # a [age=90]
+# âââ b [age=65] # â âââ d [age=40] # â âââ e [age=35] #
+âââ c [age=60] print_tree(root, attr_list=["age"], attr_bracket=["*(",
+")"]) # a *(age=90) # âââ b *(age=65) # â âââ d *(age=40) # â
+âââ e *(age=35) # âââ c *(age=60) print_tree(root, all_attrs=True)
+# a [age=90, gender=F] # âââ b [age=65, gender=M] # â âââ d
+[age=40, gender=F] # â âââ e [age=35, gender=M] # âââ c [age=60,
+gender=M] # Available styles print_tree(root, style="ansi") # a # |-- b # | |-
 - d # | `-- e # `-- c print_tree(root, style="ascii") # a # |-- b # | |-- d # |
 +-- e # +-- c print_tree(root, style="const") # a # âââ b # â âââ
 d # â âââ e # âââ c print_tree(root, style="const_bold") # a #
 â£ââ b # â â£ââ d # â âââ e # âââ c print_tree(root,
 style="rounded") # a # âââ b # â âââ d # â â°ââ e #
 â°ââ c print_tree(root, style="double") # a # â ââ b # â â ââ
 d # â âââ e # âââ c print_tree( root, style="custom",
 custom_style=("| ", "|-- ", "+-- "), ) # a # |-- b # | |-- d # | +-- e # +-- c
-``` ### Modify Tree Nodes can be shifted or copied from one path to another.
-```python from bigtree import Node, shift_nodes, print_tree root = Node("a") b
-= Node("b", parent=root) c = Node("c", parent=root) d = Node("d", parent=root)
-print_tree(root) # a # âââ b # âââ c # âââ d shift_nodes
-( tree=root, from_paths=["a/c", "a/d"], to_paths=["a/b/c", "a/dummy/d"], )
-print_tree(root) # a # âââ b # â âââ c # âââ dummy #
-âââ d ``` ```python from bigtree import Node, copy_nodes, print_tree root
+``` ### Traverse Tree Tree can be traversed using pre-order, post-order, level-
+order, or level-order-group traversal methods. ```python from bigtree import
+Node, preorder_iter, postorder_iter, levelorder_iter, levelordergroup_iter root
 = Node("a") b = Node("b", parent=root) c = Node("c", parent=root) d = Node("d",
-parent=root) print_tree(root) # a # âââ b # âââ c # âââ d
-copy_nodes( tree=root, from_paths=["a/c", "a/d"], to_paths=["a/b/c", "a/dummy/
-d"], ) print_tree(root) # a # âââ b # â âââ c # âââ c #
-âââ d # âââ dummy # âââ d ``` Nodes can also be copied
-between two different trees. ```python from bigtree import Node,
-copy_nodes_from_tree_to_tree, print_tree root = Node("a") b = Node("b",
-parent=root) c = Node("c", parent=root) d = Node("d", parent=root) print_tree
-(root) # a # âââ b # âââ c # âââ d root_other = Node("aa")
+parent=b) e = Node("e", parent=b) root.show() # a # âââ b # â âââ
+d # â âââ e # âââ c [node.name for node in preorder_iter(root)] #
+['a', 'b', 'd', 'e', 'c'] [node.name for node in postorder_iter(root)] # ['d',
+'e', 'b', 'c', 'a'] [node.name for node in levelorder_iter(root)] # ['a', 'b',
+'c', 'd', 'e'] [[node.name for node in node_group] for node_group in
+levelordergroup_iter(root)] # [['a'], ['b', 'c'], ['d', 'e']] ``` ### Modify
+Tree Nodes can be shifted or copied from one path to another. ```python from
+bigtree import Node, shift_nodes root = Node("a") b = Node("b", parent=root) c
+= Node("c", parent=root) d = Node("d", parent=root) root.show() # a # âââ
+b # âââ c # âââ d shift_nodes( tree=root, from_paths=["a/c", "a/
+d"], to_paths=["a/b/c", "a/dummy/d"], ) root.show() # a # âââ b # â
+âââ c # âââ dummy # âââ d ``` ```python from bigtree import
+Node, copy_nodes root = Node("a") b = Node("b", parent=root) c = Node("c",
+parent=root) d = Node("d", parent=root) root.show() # a # âââ b #
+âââ c # âââ d copy_nodes( tree=root, from_paths=["a/c", "a/d"],
+to_paths=["a/b/c", "a/dummy/d"], ) root.show() # a # âââ b # â
+âââ c # âââ c # âââ d # âââ dummy # âââ d ```
+Nodes can also be copied between two different trees. ```python from bigtree
+import Node, copy_nodes_from_tree_to_tree root = Node("a") b = Node("b",
+parent=root) c = Node("c", parent=root) d = Node("d", parent=root) root.show()
+# a # âââ b # âââ c # âââ d root_other = Node("aa")
 copy_nodes_from_tree_to_tree( from_tree=root, to_tree=root_other, from_paths=
-["a/b", "a/c", "a/d"], to_paths=["aa/b", "aa/b/c", "aa/dummy/d"], ) print_tree
-(root_other) # aa # âââ b # â âââ c # âââ dummy # âââ
-d ``` ### Tree Search One or multiple nodes can be search based on name, path,
-attribute value, or user-defined condition. To find a single node, ```python
-from bigtree import Node, print_tree, find, find_name, find_path,
-find_full_path, find_attr root = Node("a", age=90) b = Node("b", age=65,
-parent=root) c = Node("c", age=60, parent=root) d = Node("d", age=40, parent=c)
-print_tree(root, attr_list=["age"]) # a [age=90] # âââ b [age=65] #
-âââ c [age=60] # âââ d [age=40] find(root, lambda node: node.age ==
-60) # Node(/a/c, age=60) find_name(root, "d") # Node(/a/c/d, age=40) find_path
-(root, "/c/d") # partial path # Node(/a/c/d, age=40) find_full_path(root, "a/c/
-d") # full path # Node(/a/c/d, age=40) find_attr(root, "age", 40) # Node(/a/c/
-d, age=40) ``` To find multiple nodes, ```python from bigtree import Node,
-print_tree, findall, find_names, find_paths, find_attrs root = Node("a",
-age=90) b = Node("b", age=65, parent=root) c = Node("c", age=60, parent=root) d
-= Node("c", age=40, parent=c) print_tree(root, attr_list=["age"]) # a [age=90]
-# âââ b [age=65] # âââ c [age=65] # âââ c [age=40] findall
-(root, lambda node: node.age >= 65) # (Node(/a, age=90), Node(/a/b, age=65))
-find_names(root, "c") # (Node(/a/c, age=60), Node(/a/c/c, age=40)) find_paths
-(root, "/c") # partial path # (Node(/a/c, age=60), Node(/a/c/c, age=40))
-find_attrs(root, "age", 40) # (Node(/a/c/c, age=40),) ``` ### Helper Utility
-There following are helper functions for cloning tree to another `Node` type,
-pruning tree, and getting difference between two trees. ```python from bigtree
-import BaseNode, Node, print_tree, clone_tree, prune_tree, get_tree_diff #
-Cloning tree from `BaseNode` to `Node` type root = BaseNode(name="a") b =
-BaseNode(name="b", parent=root) clone_tree(root, Node) # Node(/a, ) # Prune
-tree to only path a/b root = Node("a") b = Node("b", parent=root) c = Node("c",
-parent=root) print_tree(root) # a # âââ b # âââ c root_pruned =
-prune_tree(root, "a/b") print_tree(root_pruned) # a # âââ b # Get
-difference between two trees root = Node("a") b = Node("b", parent=root) c =
-Node("c", parent=root) print_tree(root) # a # âââ b # âââ c
-root_other = Node("a") b_other = Node("b", parent=root_other) print_tree
-(root_other) # a # âââ b tree_diff = get_tree_diff(root, root_other)
-print_tree(tree_diff) # a # âââ c (-) tree_diff = get_tree_diff(root,
-root_other, only_diff=False) print_tree(tree_diff) # a # âââ b #
-âââ c (-) ``` ### Export Tree Tree can be exported to another data type.
-1. *Export to **nested dictionary*** 2. *Export to **nested recursive
-dictionary*** 3. *Export to **pandas DataFrame*** 4. *Export to **dot** (and
-png)* 5. *Export to **Pillow** (and png)* ```python from bigtree import Node,
-print_tree, tree_to_dict, tree_to_nested_dict, tree_to_dataframe, tree_to_dot,
-tree_to_pillow root = Node("a", age=90) b = Node("b", age=65, parent=root) c =
-Node("c", age=60, parent=root) d = Node("d", age=40, parent=b) e = Node("e",
-age=35, parent=b) print_tree(root) # a # âââ b # â âââ d # â
-âââ e # âââ c tree_to_dict( root, name_key="name",
-parent_key="parent", attr_dict={"age": "person age"} ) # { # '/a': {'name':
-'a', 'parent': None, 'person age': 90}, # '/a/b': {'name': 'b', 'parent': 'a',
-'person age': 65}, # '/a/b/d': {'name': 'd', 'parent': 'b', 'person age': 40},
-# '/a/b/e': {'name': 'e', 'parent': 'b', 'person age': 35}, # '/a/c': {'name':
-'c', 'parent': 'a', 'person age': 60} # } tree_to_nested_dict(root,
-all_attrs=True) # { # 'name': 'a', # 'age': 90, # 'children': [ # { # 'name':
-'b', # 'age': 65, # 'children': [ # { # 'name': 'd', # 'age': 40 # }, # { #
-'name': 'e', # 'age': 35 # } # ] # }, # { # 'name': 'c', # 'age': 60 # } # ] #
-} tree_to_dataframe( root, name_col="name", parent_col="parent",
-path_col="path", attr_dict={"age": "person age"} ) # path name parent person
-age # 0 /a a None 90 # 1 /a/b b a 65 # 2 /a/b/d d b 40 # 3 /a/b/e e b 35 # 4 /
-a/c c a 60 graph = tree_to_dot(root, node_colour="gold") graph.write_png
-("assets/demo.png") pillow_image = tree_to_pillow(root) pillow_image.save
-("assets/demo_pillow.png") ``` - demo.png ![Sample Dot Image Output](https://
-github.com/kayjan/bigtree/raw/master/assets/demo.png) - demo_pillow.png !
-[Sample Pillow Image Output](https://github.com/kayjan/bigtree/raw/master/
-assets/demo_pillow.png) ---- ## Binary Tree Demonstration Compared to nodes in
-tree, nodes in Binary Tree are only allowed maximum of 2 children. Since
-BinaryNode extends from Node, construct, traverse, search, export methods from
-Node are applicable to Binary Tree as well. ### Construct Binary Tree 1. **From
-`BinaryNode`** BinaryNode can be linked to each other with `parent`,
-`children`, `left`, and `right` setter methods, or using bitshift operator with
-the convention `parent_node >> child_node` or `child_node << parent_node`.
-```python from bigtree import BinaryNode, tree_to_dot e = BinaryNode(5) d =
-BinaryNode(4) c = BinaryNode(3) b = BinaryNode(2, left=d, right=e) a =
-BinaryNode(1, children=[b, c]) f = BinaryNode(6, parent=c) g = BinaryNode(7,
-parent=c) h = BinaryNode(8, parent=d) graph = tree_to_dot(a,
-node_colour="gold") graph.write_png("assets/demo_binarytree.png") ``` ![Sample
-DAG Output](https://github.com/kayjan/bigtree/raw/master/assets/
-demo_binarytree.png) 2. **From *list*** Construct nodes only, list has similar
-format as `heapq` list. ```python from bigtree import list_to_binarytree,
-print_tree nums_list = [1, 2, 3, 4, 5, 6, 7, 8] root = list_to_binarytree
-(nums_list) print_tree(root) # 1 # âââ 2 # â âââ 4 # â â
-âââ 8 # â âââ 5 # âââ 3 # âââ 6 # âââ 7 ``` ---
-- ## DAG Demonstration Compared to nodes in tree, nodes in DAG are able to have
-multiple parents. ### Construct DAG 1. **From `DAGNode`** DAGNode can be linked
-to each other with `parents` and `children` setter methods, or using bitshift
-operator with the convention `parent_node >> child_node` or `child_node <<
-parent_node`. ```python from bigtree import DAGNode, dag_to_dot a = DAGNode
-("a") b = DAGNode("b") c = DAGNode("c", parents=[a, b]) d = DAGNode("d",
-parents=[a, c]) e = DAGNode("e", parents=[d]) f = DAGNode("f", parents=[c, d])
-h = DAGNode("h") g = DAGNode("g", parents=[c], children=[h]) graph = dag_to_dot
-(a, node_colour="gold") graph.write_png("assets/demo_dag.png") ``` ![Sample DAG
-Output](https://github.com/kayjan/bigtree/raw/master/assets/demo_dag.png) 2.
-**From *list*** Construct nodes only, list contains parent-child tuples.
-```python from bigtree import list_to_dag, dag_iterator relations_list = [
-("a", "c"), ("a", "d"), ("b", "c"), ("c", "d"), ("d", "e") ] dag = list_to_dag
-(relations_list) print([(parent.node_name, child.node_name) for parent, child
-in dag_iterator(dag)]) # [('a', 'd'), ('c', 'd'), ('d', 'e'), ('a', 'c'), ('b',
-'c')] ``` 3. **From *nested dictionary*** Construct nodes with attributes,
-`key`: child name, `value`: dict of parent name, child node attributes.
-```python from bigtree import dict_to_dag, dag_iterator relation_dict = { "a":
-{"step": 1}, "b": {"step": 1}, "c": {"parents": ["a", "b"], "step": 2}, "d":
-{"parents": ["a", "c"], "step": 2}, "e": {"parents": ["d"], "step": 3}, } dag =
-dict_to_dag(relation_dict, parent_key="parents") print([(parent.node_name,
+["a/b", "a/c", "a/d"], to_paths=["aa/b", "aa/b/c", "aa/dummy/d"], )
+root_other.show() # aa # âââ b # â âââ c # âââ dummy #
+âââ d ``` ### Tree Search One or multiple nodes can be search based on
+name, path, attribute value, or user-defined condition. To find a single node,
+```python from bigtree import Node, find, find_name, find_path, find_full_path,
+find_attr root = Node("a", age=90) b = Node("b", age=65, parent=root) c = Node
+("c", age=60, parent=root) d = Node("d", age=40, parent=c) root.show(attr_list=
+["age"]) # a [age=90] # âââ b [age=65] # âââ c [age=60] # âââ
+d [age=40] find(root, lambda node: node.age == 60) # Node(/a/c, age=60)
+find_name(root, "d") # Node(/a/c/d, age=40) find_path(root, "/c/d") # partial
+path # Node(/a/c/d, age=40) find_full_path(root, "a/c/d") # full path # Node(/
+a/c/d, age=40) find_attr(root, "age", 40) # Node(/a/c/d, age=40) ``` To find
+multiple nodes, ```python from bigtree import Node, findall, find_names,
+find_paths, find_attrs root = Node("a", age=90) b = Node("b", age=65,
+parent=root) c = Node("c", age=60, parent=root) d = Node("c", age=40, parent=c)
+root.show(attr_list=["age"]) # a [age=90] # âââ b [age=65] # âââ c
+[age=60] # âââ c [age=40] findall(root, lambda node: node.age >= 65) #
+(Node(/a, age=90), Node(/a/b, age=65)) find_names(root, "c") # (Node(/a/c,
+age=60), Node(/a/c/c, age=40)) find_paths(root, "/c") # partial path # (Node(/
+a/c, age=60), Node(/a/c/c, age=40)) find_attrs(root, "age", 40) # (Node(/a/c/c,
+age=40),) ``` It is also possible to search for one or more child node(s) based
+on attributes, and the search will be faster as this does not require
+traversing the whole tree to find the node(s). ```python from bigtree import
+Node, find_children, find_child, find_child_by_name root = Node("a", age=90) b
+= Node("b", age=65, parent=root) c = Node("c", age=60, parent=root) d = Node
+("c", age=40, parent=c) root.show(attr_list=["age"]) # a [age=90] # âââ b
+[age=65] # âââ c [age=60] # âââ c [age=40] find_children(root,
+lambda node: node.age >= 60) # (Node(/a/b, age=65), Node(/a/c, age=60))
+find_child(root, lambda node: node.name == "c") # Node(/a/c, age=60)
+find_child_by_name(root, "c") # Node(/a/c, age=60) find_child_by_name(c, "c") #
+Node(/a/c/c, age=40) ``` ### Helper Utility There following are helper
+functions for cloning tree to another `Node` type, pruning tree, and getting
+difference between two trees. ```python from bigtree import BaseNode, Node,
+clone_tree, prune_tree, get_tree_diff # Cloning tree from `BaseNode` to `Node`
+type root = BaseNode(name="a") b = BaseNode(name="b", parent=root) clone_tree
+(root, Node) # Node(/a, ) # Prune tree to only path a/b root = Node("a") b =
+Node("b", parent=root) c = Node("c", parent=root) root.show() # a # âââ b
+# âââ c root_pruned = prune_tree(root, "a/b") root_pruned.show() # a #
+âââ b # Get difference between two trees root = Node("a") b = Node("b",
+parent=root) c = Node("c", parent=root) root.show() # a # âââ b #
+âââ c root_other = Node("a") b_other = Node("b", parent=root_other)
+root_other.show() # a # âââ b tree_diff = get_tree_diff(root, root_other)
+tree_diff.show() # a # âââ c (-) tree_diff = get_tree_diff(root,
+root_other, only_diff=False) tree_diff.show() # a # âââ b # âââ c
+(-) ``` ### Export Tree Tree can be exported to another data type. 1. *Export
+to **nested dictionary*** 2. *Export to **nested recursive dictionary*** 3.
+*Export to **pandas DataFrame*** 4. *Export to **dot** (and png)* 5. *Export to
+**Pillow** (and png)* ```python from bigtree import Node, tree_to_dict,
+tree_to_nested_dict, tree_to_dataframe, tree_to_dot, tree_to_pillow root = Node
+("a", age=90) b = Node("b", age=65, parent=root) c = Node("c", age=60,
+parent=root) d = Node("d", age=40, parent=b) e = Node("e", age=35, parent=b)
+root.show() # a # âââ b # â âââ d # â âââ e # âââ c
+tree_to_dict( root, name_key="name", parent_key="parent", attr_dict={"age":
+"person age"} ) # { # '/a': {'name': 'a', 'parent': None, 'person age': 90}, #
+'/a/b': {'name': 'b', 'parent': 'a', 'person age': 65}, # '/a/b/d': {'name':
+'d', 'parent': 'b', 'person age': 40}, # '/a/b/e': {'name': 'e', 'parent': 'b',
+'person age': 35}, # '/a/c': {'name': 'c', 'parent': 'a', 'person age': 60} # }
+tree_to_nested_dict(root, all_attrs=True) # { # 'name': 'a', # 'age': 90, #
+'children': [ # { # 'name': 'b', # 'age': 65, # 'children': [ # { # 'name':
+'d', # 'age': 40 # }, # { # 'name': 'e', # 'age': 35 # } # ] # }, # { # 'name':
+'c', # 'age': 60 # } # ] # } tree_to_dataframe( root, name_col="name",
+parent_col="parent", path_col="path", attr_dict={"age": "person age"} ) # path
+name parent person age # 0 /a a None 90 # 1 /a/b b a 65 # 2 /a/b/d d b 40 # 3 /
+a/b/e e b 35 # 4 /a/c c a 60 graph = tree_to_dot(root, node_colour="gold")
+graph.write_png("assets/demo.png") pillow_image = tree_to_pillow(root)
+pillow_image.save("assets/demo_pillow.png") ``` - demo.png ![Sample Dot Image
+Output](https://github.com/kayjan/bigtree/raw/master/assets/demo.png) -
+demo_pillow.png ![Sample Pillow Image Output](https://github.com/kayjan/
+bigtree/raw/master/assets/demo_pillow.png) ---- ## Binary Tree Demonstration
+Compared to nodes in tree, nodes in Binary Tree are only allowed maximum of 2
+children. Since BinaryNode extends from Node, construct, traverse, search,
+export methods from Node are applicable to Binary Tree as well. ### Construct
+Binary Tree 1. **From `BinaryNode`** BinaryNode can be linked to each other
+with `parent`, `children`, `left`, and `right` setter methods, or using
+bitshift operator with the convention `parent_node >> child_node` or
+`child_node << parent_node`. ```python from bigtree import BinaryNode,
+tree_to_dot e = BinaryNode(5) d = BinaryNode(4) c = BinaryNode(3) b =
+BinaryNode(2, left=d, right=e) a = BinaryNode(1, children=[b, c]) f =
+BinaryNode(6, parent=c) g = BinaryNode(7, parent=c) h = BinaryNode(8, parent=d)
+graph = tree_to_dot(a, node_colour="gold") graph.write_png("assets/
+demo_binarytree.png") ``` ![Sample DAG Output](https://github.com/kayjan/
+bigtree/raw/master/assets/demo_binarytree.png) 2. **From *list*** Construct
+nodes only, list has similar format as `heapq` list. ```python from bigtree
+import list_to_binarytree nums_list = [1, 2, 3, 4, 5, 6, 7, 8] root =
+list_to_binarytree(nums_list) root.show() # 1 # âââ 2 # â âââ 4 #
+â â âââ 8 # â âââ 5 # âââ 3 # âââ 6 # âââ 7
+``` ### Traverse Binary Tree In addition to the traversal methods in the usual
+tree, binary tree includes in-order traversal method. ```python from bigtree
+import list_to_binarytree, inorder_iter, preorder_iter, postorder_iter,
+levelorder_iter, levelordergroup_iter nums_list = [1, 2, 3, 4, 5, 6, 7, 8] root
+= list_to_binarytree(nums_list) root.show() # 1 # âââ 2 # â âââ 4
+# â â âââ 8 # â âââ 5 # âââ 3 # âââ 6 # âââ
+7 [node.name for node in inorder_iter(root)] # ['8', '4', '2', '5', '1', '6',
+'3', '7'] [node.name for node in preorder_iter(root)] # ['1', '2', '4', '8',
+'5', '3', '6', '7'] [node.name for node in postorder_iter(root)] # ['8', '4',
+'5', '2', '6', '7', '3', '1'] [node.name for node in levelorder_iter(root)] #
+['1', '2', '3', '4', '5', '6', '7', '8'] [[node.name for node in node_group]
+for node_group in levelordergroup_iter(root)] # [['1'], ['2', '3'], ['4', '5',
+'6', '7'], ['8']] ``` ---- ## DAG Demonstration Compared to nodes in tree,
+nodes in DAG are able to have multiple parents. ### Construct DAG 1. **From
+`DAGNode`** DAGNode can be linked to each other with `parents` and `children`
+setter methods, or using bitshift operator with the convention `parent_node >>
+child_node` or `child_node << parent_node`. ```python from bigtree import
+DAGNode, dag_to_dot a = DAGNode("a") b = DAGNode("b") c = DAGNode("c", parents=
+[a, b]) d = DAGNode("d", parents=[a, c]) e = DAGNode("e", parents=[d]) f =
+DAGNode("f", parents=[c, d]) h = DAGNode("h") g = DAGNode("g", parents=[c],
+children=[h]) graph = dag_to_dot(a, node_colour="gold") graph.write_png
+("assets/demo_dag.png") ``` ![Sample DAG Output](https://github.com/kayjan/
+bigtree/raw/master/assets/demo_dag.png) 2. **From *list*** Construct nodes
+only, list contains parent-child tuples. ```python from bigtree import
+list_to_dag, dag_iterator relations_list = [ ("a", "c"), ("a", "d"), ("b",
+"c"), ("c", "d"), ("d", "e") ] dag = list_to_dag(relations_list) print([
+(parent.node_name, child.node_name) for parent, child in dag_iterator(dag)]) #
+[('a', 'd'), ('c', 'd'), ('d', 'e'), ('a', 'c'), ('b', 'c')] ``` 3. **From
+*nested dictionary*** Construct nodes with attributes, `key`: child name,
+`value`: dict of parent name, child node attributes. ```python from bigtree
+import dict_to_dag, dag_iterator relation_dict = { "a": {"step": 1}, "b":
+{"step": 1}, "c": {"parents": ["a", "b"], "step": 2}, "d": {"parents": ["a",
+"c"], "step": 2}, "e": {"parents": ["d"], "step": 3}, } dag = dict_to_dag
+(relation_dict, parent_key="parents") print([(parent.node_name,
 child.node_name) for parent, child in dag_iterator(dag)]) # [('a', 'd'), ('c',
 'd'), ('d', 'e'), ('a', 'c'), ('b', 'c')] ``` 4. **From *pandas DataFrame***
 Construct nodes with attributes, *pandas DataFrame* contains child column,
 parent column, and attribute columns. ```python import pandas as pd from
 bigtree import dataframe_to_dag, dag_iterator path_data = pd.DataFrame([ ["a",
 None, 1], ["b", None, 1], ["c", "a", 2], ["c", "b", 2], ["d", "a", 2], ["d",
 "c", 2], ["e", "d", 3], ], columns=["child", "parent", "step"] ) dag =
 dataframe_to_dag(path_data) print([(parent.node_name, child.node_name) for
 parent, child in dag_iterator(dag)]) # [('a', 'd'), ('c', 'd'), ('d', 'e'),
-('a', 'c'), ('b', 'c')] ``` ---- ## Demo Usage ### To Do Application There is
-existing implementation of a To-Do app to showcase how `bigtree` can be used.
-There are functions to: - Add or remove list to To-Do application - Add or
-remove item to list, default list is the 'General' list - Prioritize a list/
-item by reordering them as first list/item - Save and import To-Do application
-to and from an external JSON file - Show To-Do application, which prints tree
-to console ```python from bigtree import AppToDo app = AppToDo("To Do App")
-app.add_item(item_name="Homework 1", list_name="School") app.add_item
+('a', 'c'), ('b', 'c')] ``` ---- ## Demo Usage There are existing
+implementations of workflows to showcase how `bigtree` can be used! ### To Do
+Application There are functions to: - Add or remove list to To-Do application -
+Add or remove item to list, default list is the 'General' list - Prioritize a
+list/item by reordering them as first list/item - Save and import To-Do
+application to and from an external JSON file - Show To-Do application, which
+prints tree to console ```python from bigtree import AppToDo app = AppToDo("To
+Do App") app.add_item(item_name="Homework 1", list_name="School") app.add_item
 (item_name=["Milk", "Bread"], list_name="Groceries", description="Urgent")
 app.add_item(item_name="Cook") app.show() # To Do App # âââ School # â
 âââ Homework 1 # âââ Groceries # â âââ Milk
 [description=Urgent] # â âââ Bread [description=Urgent] # âââ
 General # âââ Cook app.save("list.json") app2 = AppToDo.load("list.json")
-```
+``` ### Calendar Application There are functions to: - Add or remove event from
+Calendar - Find event by name, or name and date - Display calendar, which
+prints events to console - Export calendar to pandas DataFrame ```python import
+datetime as dt from bigtree import Calendar calendar = Calendar("My Calendar")
+calendar.add_event("Gym", "2023-01-01 18:00") calendar.add_event("Dinner",
+"2023-01-01", date_format="%Y-%m-%d", budget=20) calendar.add_event("Gym",
+"2023-01-02 18:00") calendar.show() # My Calendar # 2023-01-01 00:00:00 -
+Dinner (budget: 20) # 2023-01-01 18:00:00 - Gym # 2023-01-02 18:00:00 - Gym
+calendar.find_event("Gym") # 2023-01-01 18:00:00 - Gym # 2023-01-02 18:00:00 -
+Gym calendar.delete_event("Gym", dt.date(2023, 1, 1)) calendar.show() # My
+Calendar # 2023-01-01 00:00:00 - Dinner (budget: 20) # 2023-01-02 18:00:00 -
+Gym data_calendar = calendar.to_dataframe() data_calendar # path name date time
+budget # 0 /My Calendar/2023/01/01/Dinner Dinner 2023-01-01 00:00:00 20.0 # 1 /
+My Calendar/2023/01/02/Gym Gym 2023-01-02 18:00:00 NaN ```
```

