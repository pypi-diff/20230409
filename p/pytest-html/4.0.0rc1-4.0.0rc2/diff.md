# Comparing `tmp/pytest_html-4.0.0rc1.tar.gz` & `tmp/pytest_html-4.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Mon Apr  3 20:24:16 2023, max compression
+gzip compressed data, last modified: Sat Apr  8 22:35:18 2023, max compression
```

## Comparing `pytest_html-4.0.0rc1.tar` & `pytest_html-4.0.0rc2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0      146 2023-04-03 20:24:16.000000 pytest_html-4.0.0rc1/.coveragerc
--rw-r--r--   0        0        0     1953 2023-04-03 20:24:16.000000 pytest_html-4.0.0rc1/.eslintrc.json
--rw-r--r--   0        0        0       82 2023-04-03 20:24:16.000000 pytest_html-4.0.0rc1/.nycrc
--rw-r--r--   0        0        0     1694 2023-04-03 20:24:16.000000 pytest_html-4.0.0rc1/.pre-commit-config.yaml
--rw-r--r--   0        0        0       63 2023-04-03 20:24:16.000000 pytest_html-4.0.0rc1/.prettierrc
--rw-r--r--   0        0        0      101 2023-04-03 20:24:16.000000 pytest_html-4.0.0rc1/codecov.yml
--rw-r--r--   0        0        0      215 2023-04-03 20:24:16.000000 pytest_html-4.0.0rc1/docker-compose.tmpl.yml
--rw-r--r--   0        0        0   340564 2023-04-03 20:24:16.000000 pytest_html-4.0.0rc1/package-lock.json
--rw-r--r--   0        0        0      661 2023-04-03 20:24:16.000000 pytest_html-4.0.0rc1/package.json
--rw-r--r--   0        0        0    45508 2023-04-03 20:24:16.000000 pytest_html-4.0.0rc1/poetry.lock
--rwxr-xr-x   0        0        0      391 2023-04-03 20:24:16.000000 pytest_html-4.0.0rc1/start
--rw-r--r--   0        0        0     1969 2023-04-03 20:24:16.000000 pytest_html-4.0.0rc1/tox.ini
--rw-r--r--   0        0        0      634 2023-04-03 20:24:16.000000 pytest_html-4.0.0rc1/docs/Makefile
--rw-r--r--   0        0        0      171 2023-04-03 20:24:16.000000 pytest_html-4.0.0rc1/docs/api_reference.rst
--rw-r--r--   0        0        0    13972 2023-04-03 20:24:16.000000 pytest_html-4.0.0rc1/docs/changelog.rst
--rw-r--r--   0        0        0     2208 2023-04-03 20:24:16.000000 pytest_html-4.0.0rc1/docs/conf.py
--rw-r--r--   0        0        0     3386 2023-04-03 20:24:16.000000 pytest_html-4.0.0rc1/docs/development.rst
--rw-r--r--   0        0        0      490 2023-04-03 20:24:16.000000 pytest_html-4.0.0rc1/docs/index.rst
--rw-r--r--   0        0        0      340 2023-04-03 20:24:16.000000 pytest_html-4.0.0rc1/docs/installing.rst
--rw-r--r--   0        0        0      795 2023-04-03 20:24:16.000000 pytest_html-4.0.0rc1/docs/make.bat
--rw-r--r--   0        0        0    10328 2023-04-03 20:24:16.000000 pytest_html-4.0.0rc1/docs/user_guide.rst
--rw-r--r--   0        0        0      111 2023-04-03 20:24:16.000000 pytest_html-4.0.0rc1/src/.gitattributes
--rw-r--r--   0        0        0      125 2023-04-03 20:24:16.000000 pytest_html-4.0.0rc1/src/.gitignore
--rw-r--r--   0        0        0     5212 2023-04-03 20:24:16.000000 pytest_html-4.0.0rc1/src/layout/css/style.scss
--rw-r--r--   0        0        0      224 2023-04-03 20:24:16.000000 pytest_html-4.0.0rc1/src/pytest_html/__init__.py
--rw-r--r--   0        0        0      163 2023-04-03 20:24:16.000000 pytest_html-4.0.0rc1/src/pytest_html/__version.py
--rw-r--r--   0        0        0    12274 2023-04-03 20:24:16.000000 pytest_html-4.0.0rc1/src/pytest_html/basereport.py
--rw-r--r--   0        0        0     1595 2023-04-03 20:24:16.000000 pytest_html-4.0.0rc1/src/pytest_html/extras.py
--rw-r--r--   0        0        0      739 2023-04-03 20:24:16.000000 pytest_html-4.0.0rc1/src/pytest_html/hooks.py
--rw-r--r--   0        0        0     4108 2023-04-03 20:24:16.000000 pytest_html-4.0.0rc1/src/pytest_html/plugin.py
--rw-r--r--   0        0        0     1372 2023-04-03 20:24:16.000000 pytest_html-4.0.0rc1/src/pytest_html/report.py
--rw-r--r--   0        0        0     1178 2023-04-03 20:24:16.000000 pytest_html-4.0.0rc1/src/pytest_html/selfcontained_report.py
--rw-r--r--   0        0        0     1357 2023-04-03 20:24:16.000000 pytest_html-4.0.0rc1/src/pytest_html/table.py
--rw-r--r--   0        0        0      673 2023-04-03 20:24:16.000000 pytest_html-4.0.0rc1/src/pytest_html/util.py
--rw-r--r--   0        0        0    21645 2023-04-03 20:24:16.000000 pytest_html-4.0.0rc1/src/pytest_html/resources/app.js
--rw-r--r--   0        0        0     4931 2023-04-03 20:24:16.000000 pytest_html-4.0.0rc1/src/pytest_html/resources/index.jinja2
--rw-r--r--   0        0        0     4313 2023-04-03 20:24:16.000000 pytest_html-4.0.0rc1/src/pytest_html/resources/style.css
--rw-r--r--   0        0        0     1572 2023-04-03 20:24:16.000000 pytest_html-4.0.0rc1/src/pytest_html/scripts/datamanager.js
--rw-r--r--   0        0        0     5618 2023-04-03 20:24:16.000000 pytest_html-4.0.0rc1/src/pytest_html/scripts/dom.js
--rw-r--r--   0        0        0      855 2023-04-03 20:24:16.000000 pytest_html-4.0.0rc1/src/pytest_html/scripts/filter.js
--rw-r--r--   0        0        0      400 2023-04-03 20:24:16.000000 pytest_html-4.0.0rc1/src/pytest_html/scripts/index.js
--rw-r--r--   0        0        0     4295 2023-04-03 20:24:16.000000 pytest_html-4.0.0rc1/src/pytest_html/scripts/main.js
--rw-r--r--   0        0        0     2269 2023-04-03 20:24:16.000000 pytest_html-4.0.0rc1/src/pytest_html/scripts/mediaviewer.js
--rw-r--r--   0        0        0     1021 2023-04-03 20:24:16.000000 pytest_html-4.0.0rc1/src/pytest_html/scripts/sort.js
--rw-r--r--   0        0        0     3704 2023-04-03 20:24:16.000000 pytest_html-4.0.0rc1/src/pytest_html/scripts/storage.js
--rw-r--r--   0        0        0      743 2023-04-03 20:24:16.000000 pytest_html-4.0.0rc1/src/pytest_html/scripts/utils.js
--rw-r--r--   0        0        0    43300 2023-04-03 20:24:16.000000 pytest_html-4.0.0rc1/testing/legacy_test_pytest_html.py
--rw-r--r--   0        0        0    26312 2023-04-03 20:24:16.000000 pytest_html-4.0.0rc1/testing/test_integration.py
--rw-r--r--   0        0        0     1100 2023-04-03 20:24:16.000000 pytest_html-4.0.0rc1/testing/test_unit.py
--rw-r--r--   0        0        0     9062 2023-04-03 20:24:16.000000 pytest_html-4.0.0rc1/testing/unittest.js
--rw-r--r--   0        0        0      579 2023-04-03 20:24:16.000000 pytest_html-4.0.0rc1/.gitignore
--rw-r--r--   0        0        0      193 2023-04-03 20:24:16.000000 pytest_html-4.0.0rc1/LICENSE
--rw-r--r--   0        0        0     1804 2023-04-03 20:24:16.000000 pytest_html-4.0.0rc1/README.rst
--rw-r--r--   0        0        0     2095 2023-04-03 20:24:16.000000 pytest_html-4.0.0rc1/pyproject.toml
--rw-r--r--   0        0        0     3798 2023-04-03 20:24:16.000000 pytest_html-4.0.0rc1/PKG-INFO
+-rw-r--r--   0        0        0      146 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/.coveragerc
+-rw-r--r--   0        0        0     1953 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/.eslintrc.json
+-rw-r--r--   0        0        0       82 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/.nycrc
+-rw-r--r--   0        0        0     1694 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       63 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/.prettierrc
+-rw-r--r--   0        0        0      101 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/codecov.yml
+-rw-r--r--   0        0        0      215 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/docker-compose.tmpl.yml
+-rw-r--r--   0        0        0   340564 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/package-lock.json
+-rw-r--r--   0        0        0      661 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/package.json
+-rwxr-xr-x   0        0        0      391 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/start
+-rw-r--r--   0        0        0     1970 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/tox.ini
+-rw-r--r--   0        0        0      634 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/docs/Makefile
+-rw-r--r--   0        0        0      171 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/docs/api_reference.rst
+-rw-r--r--   0        0        0    13972 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/docs/changelog.rst
+-rw-r--r--   0        0        0     2208 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/docs/conf.py
+-rw-r--r--   0        0        0     3460 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/docs/deprecations.rst
+-rw-r--r--   0        0        0     3991 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/docs/development.rst
+-rw-r--r--   0        0        0      506 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/docs/index.rst
+-rw-r--r--   0        0        0      340 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/docs/installing.rst
+-rw-r--r--   0        0        0      795 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/docs/make.bat
+-rw-r--r--   0        0        0    10798 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/docs/user_guide.rst
+-rw-r--r--   0        0        0      111 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/src/.gitattributes
+-rw-r--r--   0        0        0      125 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/src/.gitignore
+-rw-r--r--   0        0        0     5212 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/src/layout/css/style.scss
+-rw-r--r--   0        0        0      224 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/src/pytest_html/__init__.py
+-rw-r--r--   0        0        0      163 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/src/pytest_html/__version.py
+-rw-r--r--   0        0        0    12854 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/src/pytest_html/basereport.py
+-rw-r--r--   0        0        0     1595 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/src/pytest_html/extras.py
+-rw-r--r--   0        0        0      739 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/src/pytest_html/hooks.py
+-rw-r--r--   0        0        0     4440 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/src/pytest_html/plugin.py
+-rw-r--r--   0        0        0     1372 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/src/pytest_html/report.py
+-rw-r--r--   0        0        0     1178 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/src/pytest_html/selfcontained_report.py
+-rw-r--r--   0        0        0     2429 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/src/pytest_html/table.py
+-rw-r--r--   0        0        0      673 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/src/pytest_html/util.py
+-rw-r--r--   0        0        0    23906 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/src/pytest_html/resources/app.js
+-rw-r--r--   0        0        0     4931 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/src/pytest_html/resources/index.jinja2
+-rw-r--r--   0        0        0     4313 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/src/pytest_html/resources/style.css
+-rw-r--r--   0        0        0     1572 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/src/pytest_html/scripts/datamanager.js
+-rw-r--r--   0        0        0     6131 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/src/pytest_html/scripts/dom.js
+-rw-r--r--   0        0        0      855 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/src/pytest_html/scripts/filter.js
+-rw-r--r--   0        0        0      400 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/src/pytest_html/scripts/index.js
+-rw-r--r--   0        0        0     5059 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/src/pytest_html/scripts/main.js
+-rw-r--r--   0        0        0     2269 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/src/pytest_html/scripts/mediaviewer.js
+-rw-r--r--   0        0        0     1731 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/src/pytest_html/scripts/sort.js
+-rw-r--r--   0        0        0     3696 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/src/pytest_html/scripts/storage.js
+-rw-r--r--   0        0        0     1025 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/src/pytest_html/scripts/utils.js
+-rw-r--r--   0        0        0    43300 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/testing/legacy_test_pytest_html.py
+-rw-r--r--   0        0        0    30747 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/testing/test_integration.py
+-rw-r--r--   0        0        0      728 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/testing/test_unit.py
+-rw-r--r--   0        0        0    10475 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/testing/unittest.js
+-rw-r--r--   0        0        0      579 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/.gitignore
+-rw-r--r--   0        0        0      193 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/LICENSE
+-rw-r--r--   0        0        0     1804 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/README.rst
+-rw-r--r--   0        0        0     2179 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     3859 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/PKG-INFO
```

### Comparing `pytest_html-4.0.0rc1/.eslintrc.json` & `pytest_html-4.0.0rc2/.eslintrc.json`

 * *Files identical despite different names*

### Comparing `pytest_html-4.0.0rc1/.pre-commit-config.yaml` & `pytest_html-4.0.0rc2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pytest_html-4.0.0rc1/package-lock.json` & `pytest_html-4.0.0rc2/package-lock.json`

 * *Files identical despite different names*

### Comparing `pytest_html-4.0.0rc1/package.json` & `pytest_html-4.0.0rc2/package.json`

 * *Files identical despite different names*

### Comparing `pytest_html-4.0.0rc1/tox.ini` & `pytest_html-4.0.0rc2/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 # See https://docs.readthedocs.io/en/stable/builds.html#understanding-what-s-going-on
 basepython = python
 changedir = docs
 deps = sphinx
 commands = sphinx-build -b html . _build/html
 
 [flake8]
-max-line-length = 88
+max-line-length = 120
 exclude = .eggs,.tox
 # rationale here:
 # https://github.com/psf/black/blob/master/docs/the_black_code_style.md#slices
 extend-ignore = E203
 
 [pytest]
 testpaths = testing
```

### Comparing `pytest_html-4.0.0rc1/docs/Makefile` & `pytest_html-4.0.0rc2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pytest_html-4.0.0rc1/docs/changelog.rst` & `pytest_html-4.0.0rc2/docs/changelog.rst`

 * *Files identical despite different names*

### Comparing `pytest_html-4.0.0rc1/docs/conf.py` & `pytest_html-4.0.0rc2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pytest_html-4.0.0rc1/docs/development.rst` & `pytest_html-4.0.0rc2/docs/development.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Development
 ===========
 
-To contribute to `pytest-html` you can use `Pipenv`_ to manage a python virtual environment and
+To contribute to `pytest-html` you can use `Hatch`_ to manage a python virtual environment and
 `pre-commit`_ to help you with styling and formatting.
 
 To setup the virtual environment and pre-commit, run:
 
 .. code-block:: bash
 
-  $ pipenv install --dev
-  $ pipenv run pre-commit install
+  $ hatch -e test run pre-commit install
 
-If you're not using `Pipenv`_, run the following to install `pre-commit`_:
+If you're not using `Hatch`_, run the following to install `pre-commit`_:
 
 .. code-block:: bash
 
   $ pip install pre-commit
   $ pre-commit install
 
 
@@ -31,46 +30,63 @@
 
 Running Tests
 -------------
 
 Python
 ~~~~~~
 
-You will need `Tox`_ installed to run the tests against the supported Python versions. If you're using `Pipenv`_
+You will need `Tox`_ and `Docker`_ installed to run the tests against the supported Python versions. If you're using `Hatch`_
 it will be installed for you.
 
-With `Pipenv`_, run:
+The integration tests requires `Docker`_ as we have to render the report.
+This is then done using `Selenium`_ and `BeautifulSoup`_
+
+To start the image needed, run:
+
+.. code-block:: bash
+
+  $ ./start
+
+Sometimes the image becomes unresponsive and needs a restart:
+
+.. code-block:: bash
+
+  $ ./start down && ./start
+
+You can watch the tests in your browser at `localhost:7900`, the password is `secret`.
+
+To run the tests with `Hatch`_, run:
 
 .. code-block:: bash
 
-  $ pipenv run tox
+  $ hatch -e test run tox
 
 Otherwise, to install and run, do:
 
 .. code-block:: bash
 
   $ pip install tox
   $ tox
 
 JavaScript
 ~~~~~~~~~~
 
-You will need `npm`_ installed to run the JavaScript tests. Internally, we use `Grunt`_ and `QUnit`_ to run the tests.
+You will need `npm`_ installed to run the JavaScript tests. Internally, we use `Mocha`_, `Chai`_, `Sinon`_ to run the tests.
 
 Once `npm`_ is installed, you can install all needed dependencies by running:
 
 .. code-block:: bash
 
   $ npm install
 
 Run the following to execute the tests:
 
 .. code-block:: bash
 
-  $ npm test
+  $ npm run unit
 
 Documentation
 -------------
 
 Documentation is hosted on `Read the Docs`_, and is written in `RST`_. Remember to add any new files to the :code:`toctree`
 section in :code:`index.rst`.
 
@@ -106,22 +122,26 @@
 
 #.  Update your local master with the upstream master (``git pull --rebase upstream master``)
 #.  Create a new branch
 #.  Update `the changelog`_ with the new version, today's date, and all changes/new features
 #.  Commit and push the new branch and then create a new pull request
 #.  Wait for tests and reviews and then merge the branch
 #.  Once merged, update your local master again (``git pull --rebase upstream master``)
-#.  Tag the release with the new release version (``git tag v<new tag>``)
+#.  Tag the release with the new release version (``git tag <new tag>``)
 #.  Push the tag (``git push upstream --tags``)
 #. Done. Check `Github Actions`_ for release progress.
 
 .. _GitHub Actions: https://github.com/pytest-dev/pytest-html/actions
-.. _Grunt: https://gruntjs.com
+.. _Mocha: https://mochajs.org/
 .. _npm: https://www.npmjs.com
-.. _Pipenv: https://pipenv.pypa.io/en/latest
+.. _Hatch: https://hatch.pypa.io/latest/
 .. _pre-commit: https://pre-commit.com
-.. _QUnit: https://qunitjs.com
+.. _Chai: https://www.chaijs.com/
+.. _Sinon: https://sinonjs.org/
 .. _Read The Docs: https://readthedocs.com
 .. _RST: https://www.sphinx-doc.org/en/master/usage/restructuredtext/basics.html
 .. _SASS/SCSS: https://sass-lang.com
 .. _the changelog: https://pytest-html.readthedocs.io/en/latest/changelog.html
 .. _Tox: https://tox.readthedocs.io
+.. _Docker: https://www.docker.com/
+.. _Selenium: https://www.selenium.dev/
+.. _BeautifulSoup: https://beautiful-soup-4.readthedocs.io/en/latest/
```

### Comparing `pytest_html-4.0.0rc1/docs/make.bat` & `pytest_html-4.0.0rc2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pytest_html-4.0.0rc1/docs/user_guide.rst` & `pytest_html-4.0.0rc2/docs/user_guide.rst`

 * *Files 4% similar despite different names*

```diff
@@ -98,109 +98,107 @@
 Additional summary information
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 You can edit the *Summary* section by using the :code:`pytest_html_results_summary` hook:
 
 .. code-block:: python
 
-   from py.xml import html
-
-
    def pytest_html_results_summary(prefix, summary, postfix):
        prefix.extend(["<p>foo: bar</p>"])
 
 Extra content
 ~~~~~~~~~~~~~
 
-You can add details to the HTML report by creating an 'extra' list on the
+You can add details to the HTML report by creating an 'extras' list on the
 report object. Here are the types of extra content that can be added:
 
 ==========  ============================================
 Type        Example
 ==========  ============================================
-Raw HTML    ``extra.html('<div>Additional HTML</div>')``
-`JSON`_     ``extra.json({'name': 'pytest'})``
-Plain text  ``extra.text('Add some simple Text')``
-URL         ``extra.url('http://www.example.com/')``
-Image       ``extra.image(image, mime_type='image/gif', extension='gif')``
-Image       ``extra.image('/path/to/file.png')``
-Image       ``extra.image('http://some_image.png')``
+Raw HTML    ``extras.html('<div>Additional HTML</div>')``
+`JSON`_     ``extras.json({'name': 'pytest'})``
+Plain text  ``extras.text('Add some simple Text')``
+URL         ``extras.url('http://www.example.com/')``
+Image       ``extras.image(image, mime_type='image/gif', extension='gif')``
+Image       ``extras.image('/path/to/file.png')``
+Image       ``extras.image('http://some_image.png')``
 ==========  ============================================
 
 **Note**: When adding an image from file, the path can be either absolute
 or relative.
 
 **Note**: When using ``--self-contained-html``, images added as files or links
 may not work as expected, see section `Creating a self-contained report`_ for
 more info.
 
 There are also convenient types for several image formats:
 
 ============  ====================
 Image format  Example
 ============  ====================
-PNG           ``extra.png(image)``
-JPEG          ``extra.jpg(image)``
-SVG           ``extra.svg(image)``
+PNG           ``extras.png(image)``
+JPEG          ``extras.jpg(image)``
+SVG           ``extras.svg(image)``
 ============  ====================
 
 The following example adds the various types of extras using a
 :code:`pytest_runtest_makereport` hook, which can be implemented in a plugin or
 conftest.py file:
 
 .. code-block:: python
 
   import pytest
+  import pytest_html
 
 
   @pytest.hookimpl(hookwrapper=True)
   def pytest_runtest_makereport(item, call):
-      pytest_html = item.config.pluginmanager.getplugin("html")
       outcome = yield
       report = outcome.get_result()
-      extra = getattr(report, "extra", [])
+      extras = getattr(report, "extras", [])
       if report.when == "call":
           # always add url to report
-          extra.append(pytest_html.extras.url("http://www.example.com/"))
+          extras.append(pytest_html.extras.url("http://www.example.com/"))
           xfail = hasattr(report, "wasxfail")
           if (report.skipped and xfail) or (report.failed and not xfail):
               # only add additional html on failure
-              extra.append(pytest_html.extras.html("<div>Additional HTML</div>"))
-          report.extra = extra
+              extras.append(pytest_html.extras.html("<div>Additional HTML</div>"))
+          report.extras = extras
 
 You can also specify the :code:`name` argument for all types other than :code:`html` which will change the title of the
 created hyper link:
 
 .. code-block:: python
 
-    extra.append(pytest_html.extras.text("some string", name="Different title"))
+    extras.append(pytest_html.extras.text("some string", name="Different title"))
 
-It is also possible to use the fixture :code:`extra` to add content directly
+It is also possible to use the fixture :code:`extras` to add content directly
 in a test function without implementing hooks. These will generally end up
 before any extras added by plugins.
 
 .. code-block:: python
 
-   from pytest_html import extras
+   import pytest_html
 
 
-   def test_extra(extra):
-       extra.append(extras.text("some string"))
+   def test_extra(extras):
+       extras.append(pytest_html.extras.text("some string"))
 
 
+.. _modifying-results-table:
+
 Modifying the results table
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 You can modify the columns of the report by implementing custom hooks for the header and rows.
 The following example :code:`conftest.py` adds a description column with the test function docstring,
 adds a sortable time column, and removes the links column:
 
 .. code-block:: python
 
-  from datetime import datetime
   import pytest
 
 
   def pytest_html_results_table_header(cells):
       cells.insert(2, "<th>Description</th>")
       cells.insert(1, '<th class="sortable time" data-column-type="time">Time</th>')
 
@@ -228,63 +226,82 @@
 
 The log output and additional HTML can be modified by implementing the
 :code:`pytest_html_results_html` hook. The following example replaces all
 additional HTML and log output with a notice that the log is empty:
 
 .. code-block:: python
 
-  from py.xml import html
-
-
   def pytest_html_results_table_html(report, data):
       if report.passed:
           del data[:]
           data.append("<div class='empty log'>No log output captured.</div>")
 
 Display options
 ---------------
 
+.. _render-collapsed:
+
 Auto Collapsing Table Rows
 ~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 By default, all rows in the **Results** table will be expanded except those that have :code:`Passed`.
 
 This behavior can be customized with a query parameter: :code:`?collapsed=Passed,XFailed,Skipped`.
 If you want all rows to be collapsed you can pass :code:`?collapsed=All`.
 By setting the query parameter to empty string :code:`?collapsed=""` **none** of the rows will be collapsed.
 
 Note that the query parameter is case insensitive, so passing :code:`PASSED` and :code:`passed` has the same effect.
 
-You can also set the collapsed behaviour by setting the :code:`render_collapsed` in a configuration file (pytest.ini, setup.cfg, etc).
+You can also set the collapsed behaviour by setting :code:`render_collapsed` in a configuration file (pytest.ini, setup.cfg, etc).
 Note that the query parameter takes precedence.
 
 .. code-block:: ini
 
   [pytest]
   render_collapsed = failed,error
 
-Controlling Test Result Visibility Via Query Params
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+Controlling Test Result Visibility
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 By default, all tests are visible, regardless of their results. It is possible to control which tests are visible on
 page load by passing the :code:`visible` query parameter. To use this parameter, please pass a comma separated list
 of test results you wish to be visible. For example, passing :code:`?visible=passed,skipped` will show only those
 tests in the report that have outcome :code:`passed` or :code:`skipped`.
 
 Note that this match is case insensitive, so passing :code:`PASSED` and :code:`passed` has the same effect.
 
-The following query parameters may be passed:
+The following values may be passed:
 
 * :code:`passed`
 * :code:`skipped`
 * :code:`failed`
 * :code:`error`
 * :code:`xfailed`
 * :code:`xpassed`
 * :code:`rerun`
 
+Results Table Sorting
+~~~~~~~~~~~~~~~~~~~~~
+
+You can change the sort order of the results table on page load by passing the :code:`sort` query parameter.
+
+The following values may be passed:
+
+* :code:`result`
+* :code:`testId`
+* :code:`duration`
+* :code:`original`
+
+Note that the values are case *sensitive*.
+
+``original`` means that a best effort is made to sort the table in the order of execution.
+If tests are run in parallel (with `pytest-xdist`_ for example), then the order may not be
+in the correct order.
+
+
 .. _@pytest.hookimpl(tryfirst=True): https://docs.pytest.org/en/stable/writing_plugins.html#hook-function-ordering-call-example
 .. _ansi2html: https://pypi.python.org/pypi/ansi2html/
 .. _Content Security Policy (CSP): https://developer.mozilla.org/docs/Web/Security/CSP/
 .. _JSON: https://json.org/
 .. _pytest-metadata: https://pypi.python.org/pypi/pytest-metadata/
+.. _pytest-xdist: https://pypi.python.org/pypi/pytest-xdist/
 .. _time.strftime: https://docs.python.org/3/library/time.html#time.strftime
```

### Comparing `pytest_html-4.0.0rc1/src/layout/css/style.scss` & `pytest_html-4.0.0rc2/src/layout/css/style.scss`

 * *Files identical despite different names*

### Comparing `pytest_html-4.0.0rc1/src/pytest_html/basereport.py` & `pytest_html-4.0.0rc2/src/pytest_html/basereport.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,21 @@
                 "tests": defaultdict(list),
                 "resultsTableHeader": {},
                 "additionalSummary": defaultdict(list),
             }
 
             collapsed = config.getini("render_collapsed")
             if collapsed:
+                if collapsed.lower() == "true":
+                    warnings.warn(
+                        "'render_collapsed = True' is deprecated and support "
+                        "will be removed in the next major release. "
+                        "Please use 'render_collapsed = all' instead.",
+                        DeprecationWarning,
+                    )
                 self.set_data(
                     "collapsed", [outcome.lower() for outcome in collapsed.split(",")]
                 )
 
         @property
         def title(self):
             return self._data["title"]
@@ -67,21 +74,26 @@
         @property
         def data(self):
             return self._data
 
         def set_data(self, key, value):
             self._data[key] = value
 
-        def add_test(self, test_data, report, remove_log=False):
+        def add_test(self, test_data, report, row, remove_log=False):
+            for sortable, value in row.sortables.items():
+                test_data[sortable] = value
+
             # regardless of pass or fail we must add teardown logging to "call"
             if report.when == "teardown" and not remove_log:
                 self.update_test_log(report)
 
             # passed "setup" and "teardown" are not added to the html
-            if report.when == "call" or _is_error(report):
+            if report.when == "call" or (
+                report.when in ["setup", "teardown"] and report.outcome != "passed"
+            ):
                 if not remove_log:
                     processed_logs = _process_logs(report)
                     test_data["log"] = _handle_ansi(processed_logs)
                 self._data["tests"][report.nodeid].append(test_data)
                 return True
 
             return False
@@ -230,16 +242,16 @@
         if hasattr(config, "_metadata") and config._metadata:
             self._report.set_data("environment", self._generate_environment())
 
         session.config.hook.pytest_html_report_title(report=self._report)
 
         header_cells = Header()
         session.config.hook.pytest_html_results_table_header(cells=header_cells)
-
         self._report.set_data("resultsTableHeader", header_cells.html)
+        self._report.set_data("headerPops", header_cells.get_pops())
 
         self._report.set_data("runningState", "Started")
         self._generate_report()
 
     @pytest.hookimpl(trylast=True)
     def pytest_sessionfinish(self, session):
         session.config.hook.pytest_html_results_summary(
@@ -269,36 +281,32 @@
             )
 
         data = {
             "duration": report.duration,
         }
 
         test_id = report.nodeid
-        table_html = Html()
-        if report.when == "call":
-            row_cells = Row()
-            self._config.hook.pytest_html_results_table_row(
-                report=report, cells=row_cells
-            )
-            if row_cells.html is None:
-                return
-            data["resultsTableRow"] = row_cells.html
-
-            self._config.hook.pytest_html_results_table_html(
-                report=report, data=table_html
-            )
-            data["tableHtml"] = table_html.html["html"]
-        else:
+        if report.when != "call":
             test_id += f"::{report.when}"
         data["testId"] = test_id
 
+        row_cells = Row()
+        self._config.hook.pytest_html_results_table_row(report=report, cells=row_cells)
+        if row_cells.html is None:
+            return
+        data["resultsTableRow"] = row_cells.html
+
+        table_html = Html()
+        self._config.hook.pytest_html_results_table_html(report=report, data=table_html)
+        data["tableHtml"] = table_html.html["html"]
+
         data["result"] = _process_outcome(report)
         data["extras"] = self._process_extras(report, test_id)
 
-        if self._report.add_test(data, report, table_html.replace_log):
+        if self._report.add_test(data, report, row_cells, table_html.replace_log):
             self._generate_report()
 
 
 def _process_css(default_css, extra_css):
     with open(default_css, encoding="utf-8") as f:
         css = f.read()
 
@@ -327,15 +335,15 @@
 def _is_error(report):
     return report.when in ["setup", "teardown"] and report.outcome == "failed"
 
 
 def _process_logs(report):
     log = []
     if report.longreprtext:
-        log.append(report.longreprtext + "\n")
+        log.append(report.longreprtext.replace("<", "&lt;").replace(">", "&gt;") + "\n")
     for section in report.sections:
         header, content = section
         log.append(f"{' ' + header + ' ':-^80}")
         log.append(content)
 
         # weird formatting related to logs
         if "log" in header:
```

### Comparing `pytest_html-4.0.0rc1/src/pytest_html/extras.py` & `pytest_html-4.0.0rc2/src/pytest_html/extras.py`

 * *Files identical despite different names*

### Comparing `pytest_html-4.0.0rc1/src/pytest_html/hooks.py` & `pytest_html-4.0.0rc2/src/pytest_html/hooks.py`

 * *Files identical despite different names*

### Comparing `pytest_html-4.0.0rc1/src/pytest_html/plugin.py` & `pytest_html-4.0.0rc2/src/pytest_html/plugin.py`

 * *Files 10% similar despite different names*

```diff
@@ -94,17 +94,24 @@
 
 
 @pytest.hookimpl(tryfirst=True, hookwrapper=True)
 def pytest_runtest_makereport(item, call):
     outcome = yield
     report = outcome.get_result()
     if report.when == "call":
+        deprecated_extra = getattr(report, "extra", [])
+        if deprecated_extra:
+            warnings.warn(
+                "The 'report.extra' attribute is deprecated and will be removed in a future release"
+                ", use 'report.extras' instead.",
+                DeprecationWarning,
+            )
         fixture_extras = getattr(item.config, "extras", [])
         plugin_extras = getattr(report, "extras", [])
-        report.extras = fixture_extras + plugin_extras
+        report.extras = fixture_extras + plugin_extras + deprecated_extra
 
 
 @pytest.fixture
 def extra(pytestconfig):
     """Add details to the HTML reports.
 
     .. code-block:: python
```

### Comparing `pytest_html-4.0.0rc1/src/pytest_html/report.py` & `pytest_html-4.0.0rc2/src/pytest_html/report.py`

 * *Files identical despite different names*

### Comparing `pytest_html-4.0.0rc1/src/pytest_html/selfcontained_report.py` & `pytest_html-4.0.0rc2/src/pytest_html/selfcontained_report.py`

 * *Files identical despite different names*

### Comparing `pytest_html-4.0.0rc1/src/pytest_html/util.py` & `pytest_html-4.0.0rc2/src/pytest_html/util.py`

 * *Files identical despite different names*

### Comparing `pytest_html-4.0.0rc1/src/pytest_html/resources/app.js` & `pytest_html-4.0.0rc2/src/pytest_html/resources/app.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -105,15 +105,16 @@
 
     }, {
         "./storage.js": 8
     }],
     2: [function(require, module, exports) {
         const storageModule = require('./storage.js')
         const {
-            formatDuration
+            formatDuration,
+            transformTableObj
         } = require('./utils.js')
         const mediaViewer = require('./mediaviewer.js')
         const templateEnvRow = document.querySelector('#template_environment_row')
         const templateCollGroup = document.querySelector('#template_table-colgroup')
         const templateResult = document.querySelector('#template_results-table__tbody')
         const aTag = document.querySelector('#template_a')
         const listHeader = document.querySelector('#template_results-table__head')
@@ -135,17 +136,17 @@
         const findAll = (selector, elem) => {
             if (!elem) {
                 elem = document
             }
             return [...elem.querySelectorAll(selector)]
         }
 
-        const insertAdditionalHTML = (html, element, selector) => {
+        const insertAdditionalHTML = (html, element, selector, position = 'beforebegin') => {
             Object.keys(html).map((key) => {
-                element.querySelectorAll(selector).item(key).insertAdjacentHTML('beforebegin', html[key])
+                element.querySelectorAll(selector).item(key).insertAdjacentHTML(position, html[key])
             })
         }
 
         const dom = {
             getStaticRow: (key, value) => {
                 const envRow = templateEnvRow.content.cloneNode(true)
                 const isObj = typeof value === 'object' && value !== null
@@ -175,15 +176,17 @@
                         }
                     }
                     return result
                 }, [])
                 const sortables = ['result', 'testId', 'duration', ...cols]
 
                 // Add custom html from the pytest_html_results_table_header hook
-                insertAdditionalHTML(resultsTableHeader, header, 'th')
+                const headers = transformTableObj(resultsTableHeader)
+                insertAdditionalHTML(headers.inserts, header, 'th')
+                insertAdditionalHTML(headers.appends, header, 'tr', 'beforeend')
 
                 sortables.forEach((sortCol) => {
                     if (sortCol === sortAttr) {
                         header.querySelector(`[data-column-type="${sortCol}"]`).classList.add(sortAsc ? 'desc' : 'asc')
                     }
                 })
 
@@ -211,17 +214,18 @@
                 resultBody.querySelector('.col-result').innerText = result
                 resultBody.querySelector('.col-result').classList.add(`${collapsed ? 'expander' : 'collapser'}`)
                 resultBody.querySelector('.col-result').dataset.id = id
                 resultBody.querySelector('.col-name').innerText = testId
 
                 resultBody.querySelector('.col-duration').innerText = duration < 1 ? formatDuration(duration).ms : formatDuration(duration).formatted
 
-
                 if (log) {
-                    resultBody.querySelector('.log').innerHTML = log
+                    // Wrap lines starting with "E" with span.error to color those lines red
+                    const wrappedLog = log.replace(/^E.*$/gm, (match) => `<span class="error">${match}</span>`)
+                    resultBody.querySelector('.log').innerHTML = wrappedLog
                 } else {
                     resultBody.querySelector('.log').remove()
                 }
 
                 if (collapsed) {
                     resultBody.querySelector('.extras-row').classList.add('hidden')
                 }
@@ -253,15 +257,17 @@
                     if (format_type === 'html') {
                         resultBody.querySelector('.extraHTML').insertAdjacentHTML('beforeend', `<div>${content}</div>`)
                     }
                 })
                 mediaViewer.setUp(resultBody, media)
 
                 // Add custom html from the pytest_html_results_table_row hook
-                resultsTableRow && insertAdditionalHTML(resultsTableRow, resultBody, 'td')
+                const rows = transformTableObj(resultsTableRow)
+                resultsTableRow && insertAdditionalHTML(rows.inserts, resultBody, 'td')
+                resultsTableRow && insertAdditionalHTML(rows.appends, resultBody, 'tr', 'beforeend')
 
                 // Add custom html from the pytest_html_results_table_html hook
                 tableHtml?.forEach((item) => {
                     resultBody.querySelector('td[class="extra"]').insertAdjacentHTML('beforeend', item)
                 })
 
                 return resultBody
@@ -410,14 +416,29 @@
             table.appendChild(tableHeader)
 
             rows.forEach((row) => !!row && table.appendChild(row))
 
             table.querySelectorAll('.extra').forEach((item) => {
                 item.colSpan = document.querySelectorAll('th').length
             })
+
+            const {
+                headerPops
+            } = manager.renderData
+            if (headerPops > 0) {
+                // remove 'headerPops' number of header columns
+                findAll('#results-table-head th').splice(-headerPops).forEach(column => column.remove())
+
+                // remove 'headerPops' number of row columns
+                const resultRows = findAll('.results-table-row')
+                resultRows.forEach((elem) => {
+                    findAll('td:not(.extra)', elem).splice(-headerPops).forEach(column => column.remove())
+                })
+            }
+
             findAll('.sortable').forEach((elem) => {
                 elem.addEventListener('click', (evt) => {
                     const {
                         target: element
                     } = evt
                     const {
                         columnType
@@ -440,15 +461,20 @@
             const currentFilter = getVisible()
             possibleResults.forEach(({
                 result,
                 label
             }) => {
                 const count = tests.filter((test) => test.result.toLowerCase() === result).length
                 const input = document.querySelector(`input[data-test-result="${result}"]`)
+                const lastInput = document.querySelector(`input[data-test-result="${result}"]:last-of-type`)
                 document.querySelector(`.${result}`).innerText = `${count} ${label}`
+                // add a comma and whitespace between the results
+                if (input !== lastInput) {
+                    document.querySelector(`.${result}`).innerText += ', '
+                }
 
                 input.disabled = !count
                 input.checked = currentFilter.includes(result)
             })
 
             const numberOfTests = tests.filter(({
                 result
@@ -598,29 +624,48 @@
     }, {}],
     7: [function(require, module, exports) {
         const {
             manager
         } = require('./datamanager.js')
         const storageModule = require('./storage.js')
 
-        const genericSort = (list, key, ascending) => {
-            const sorted = list.sort((a, b) => a[key] === b[key] ? 0 : a[key] > b[key] ? 1 : -1)
+        const genericSort = (list, key, ascending, customOrder) => {
+            let sorted
+            if (customOrder) {
+                sorted = list.sort((a, b) => {
+                    const aValue = a.result.toLowerCase()
+                    const bValue = b.result.toLowerCase()
+
+                    const aIndex = customOrder.findIndex(item => item.toLowerCase() === aValue)
+                    const bIndex = customOrder.findIndex(item => item.toLowerCase() === bValue)
+
+                    // Compare the indices to determine the sort order
+                    return aIndex - bIndex
+                })
+            } else {
+                sorted = list.sort((a, b) => a[key] === b[key] ? 0 : a[key] > b[key] ? 1 : -1)
+            }
 
             if (ascending) {
                 sorted.reverse()
             }
             return sorted
         }
 
         const doInitSort = () => {
             const type = storageModule.getSort()
             const ascending = storageModule.getSortDirection()
             const list = manager.testSubset
-            const sortedList = genericSort(list, type, ascending)
-            manager.setRender(sortedList)
+            const initialOrder = ['Error', 'Failed', 'Rerun', 'XFailed', 'XPassed', 'Skipped', 'Passed']
+            if (type?.toLowerCase() === 'original') {
+                manager.setRender(list)
+            } else {
+                const sortedList = genericSort(list, type, ascending, initialOrder)
+                manager.setRender(sortedList)
+            }
         }
 
         const doSort = (type) => {
             const newSortType = storageModule.getSort() !== type
             const currentAsc = storageModule.getSortDirection()
             const ascending = newSortType ? true : !currentAsc
             storageModule.setSort(type)
@@ -714,25 +759,25 @@
         const getCollapsedCategory = (config) => {
             let categories
             if (typeof window !== 'undefined') {
                 const url = new URL(window.location.href)
                 const collapsedItems = new URLSearchParams(url.search).get('collapsed')
                 switch (true) {
                     case !config && collapsedItems === null:
-                        categories = ['passed'];
-                        break;
+                        categories = ['passed']
+                        break
                     case collapsedItems?.length === 0 || /^["']{2}$/.test(collapsedItems):
-                        categories = [];
-                        break;
+                        categories = []
+                        break
                     case /^all$/.test(collapsedItems) || (collapsedItems === null && /^all$/.test(config)):
-                        categories = [...possibleFilters];
-                        break;
+                        categories = [...possibleFilters]
+                        break
                     default:
-                        categories = collapsedItems?.split(',').map(item => item.toLowerCase()) || config;
-                        break;
+                        categories = collapsedItems?.split(',').map(item => item.toLowerCase()) || config
+                        break
                 }
             } else {
                 categories = []
             }
             return categories
         }
 
@@ -777,13 +822,26 @@
 
             return {
                 seconds: `${Math.round(totalSeconds)} seconds`,
                 formatted: `${formattedNumber(hours)}:${formattedNumber(minutes)}:${formattedNumber(seconds)}`,
             }
         }
 
+        const transformTableObj = (obj) => {
+            const appends = {}
+            const inserts = {}
+            for (const key in obj) {
+                key.startsWith("Z") ? appends[key] = obj[key] : inserts[key] = obj[key]
+            }
+            return {
+                appends,
+                inserts,
+            }
+        }
+
         module.exports = {
-            formatDuration
+            formatDuration,
+            transformTableObj,
         }
 
     }, {}]
 }, {}, [4]);
```

### Comparing `pytest_html-4.0.0rc1/src/pytest_html/resources/index.jinja2` & `pytest_html-4.0.0rc2/src/pytest_html/resources/index.jinja2`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -93,21 +93,21 @@
           <div class="summary__reload__button" onclick="location.reload()">
             <div>There are still tests running. <br />Reload this page to ge the latest results!</div>
           </div>
         </div>
         <div class="summary__spacer"></div>
           <div class="controls">
             <div class="filters">
-              <input checked="true" class="filter" data-test-result="error" name="filter_checkbox" type="checkbox"/><span class="error"></span>
               <input checked="true" class="filter" data-test-result="failed" name="filter_checkbox" type="checkbox"/><span class="failed"></span>
-              <input checked="true" class="filter" data-test-result="rerun" name="filter_checkbox" type="checkbox"/><span class="rerun"></span>
-              <input checked="true" class="filter" data-test-result="xfailed" name="filter_checkbox" type="checkbox"/><span class="xfailed"></span>
-              <input checked="true" class="filter" data-test-result="xpassed" name="filter_checkbox" type="checkbox"/><span class="xpassed"></span>
               <input checked="true" class="filter" data-test-result="passed" name="filter_checkbox" type="checkbox"/><span class="passed"></span>
               <input checked="true" class="filter" data-test-result="skipped" name="filter_checkbox" type="checkbox"/><span class="skipped"></span>
+              <input checked="true" class="filter" data-test-result="xfailed" name="filter_checkbox" type="checkbox"/><span class="xfailed"></span>
+              <input checked="true" class="filter" data-test-result="xpassed" name="filter_checkbox" type="checkbox"/><span class="xpassed"></span>
+              <input checked="true" class="filter" data-test-result="error" name="filter_checkbox" type="checkbox"/><span class="error"></span>
+              <input checked="true" class="filter" data-test-result="rerun" name="filter_checkbox" type="checkbox"/><span class="rerun"></span>
             </div>
             <div class="collapse">
               <button id="show_all_details">Show all details</button>&nbsp;/&nbsp;<button id="hide_all_details">Hide all details</button>
             <div>
           </div>
         </div>
       </div>
```

### Comparing `pytest_html-4.0.0rc1/src/pytest_html/resources/style.css` & `pytest_html-4.0.0rc2/src/pytest_html/resources/style.css`

 * *Files identical despite different names*

### Comparing `pytest_html-4.0.0rc1/src/pytest_html/scripts/datamanager.js` & `pytest_html-4.0.0rc2/src/pytest_html/scripts/datamanager.js`

 * *Files identical despite different names*

### Comparing `pytest_html-4.0.0rc1/src/pytest_html/scripts/dom.js` & `pytest_html-4.0.0rc2/src/pytest_html/scripts/dom.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,11 @@
 const storageModule = require('./storage.js')
 const {
-    formatDuration
+    formatDuration,
+    transformTableObj
 } = require('./utils.js')
 const mediaViewer = require('./mediaviewer.js')
 const templateEnvRow = document.querySelector('#template_environment_row')
 const templateCollGroup = document.querySelector('#template_table-colgroup')
 const templateResult = document.querySelector('#template_results-table__tbody')
 const aTag = document.querySelector('#template_a')
 const listHeader = document.querySelector('#template_results-table__head')
@@ -26,17 +27,17 @@
 const findAll = (selector, elem) => {
     if (!elem) {
         elem = document
     }
     return [...elem.querySelectorAll(selector)]
 }
 
-const insertAdditionalHTML = (html, element, selector) => {
+const insertAdditionalHTML = (html, element, selector, position = 'beforebegin') => {
     Object.keys(html).map((key) => {
-        element.querySelectorAll(selector).item(key).insertAdjacentHTML('beforebegin', html[key])
+        element.querySelectorAll(selector).item(key).insertAdjacentHTML(position, html[key])
     })
 }
 
 const dom = {
     getStaticRow: (key, value) => {
         const envRow = templateEnvRow.content.cloneNode(true)
         const isObj = typeof value === 'object' && value !== null
@@ -66,15 +67,17 @@
                 }
             }
             return result
         }, [])
         const sortables = ['result', 'testId', 'duration', ...cols]
 
         // Add custom html from the pytest_html_results_table_header hook
-        insertAdditionalHTML(resultsTableHeader, header, 'th')
+        const headers = transformTableObj(resultsTableHeader)
+        insertAdditionalHTML(headers.inserts, header, 'th')
+        insertAdditionalHTML(headers.appends, header, 'tr', 'beforeend')
 
         sortables.forEach((sortCol) => {
             if (sortCol === sortAttr) {
                 header.querySelector(`[data-column-type="${sortCol}"]`).classList.add(sortAsc ? 'desc' : 'asc')
             }
         })
 
@@ -102,17 +105,18 @@
         resultBody.querySelector('.col-result').innerText = result
         resultBody.querySelector('.col-result').classList.add(`${collapsed ? 'expander' : 'collapser'}`)
         resultBody.querySelector('.col-result').dataset.id = id
         resultBody.querySelector('.col-name').innerText = testId
 
         resultBody.querySelector('.col-duration').innerText = duration < 1 ? formatDuration(duration).ms : formatDuration(duration).formatted
 
-
         if (log) {
-            resultBody.querySelector('.log').innerHTML = log
+            // Wrap lines starting with "E" with span.error to color those lines red
+            const wrappedLog = log.replace(/^E.*$/gm, (match) => `<span class="error">${match}</span>`)
+            resultBody.querySelector('.log').innerHTML = wrappedLog
         } else {
             resultBody.querySelector('.log').remove()
         }
 
         if (collapsed) {
             resultBody.querySelector('.extras-row').classList.add('hidden')
         }
@@ -144,15 +148,17 @@
             if (format_type === 'html') {
                 resultBody.querySelector('.extraHTML').insertAdjacentHTML('beforeend', `<div>${content}</div>`)
             }
         })
         mediaViewer.setUp(resultBody, media)
 
         // Add custom html from the pytest_html_results_table_row hook
-        resultsTableRow && insertAdditionalHTML(resultsTableRow, resultBody, 'td')
+        const rows = transformTableObj(resultsTableRow)
+        resultsTableRow && insertAdditionalHTML(rows.inserts, resultBody, 'td')
+        resultsTableRow && insertAdditionalHTML(rows.appends, resultBody, 'tr', 'beforeend')
 
         // Add custom html from the pytest_html_results_table_html hook
         tableHtml?.forEach((item) => {
             resultBody.querySelector('td[class="extra"]').insertAdjacentHTML('beforeend', item)
         })
 
         return resultBody
```

### Comparing `pytest_html-4.0.0rc1/src/pytest_html/scripts/filter.js` & `pytest_html-4.0.0rc2/src/pytest_html/scripts/filter.js`

 * *Files identical despite different names*

### Comparing `pytest_html-4.0.0rc1/src/pytest_html/scripts/main.js` & `pytest_html-4.0.0rc2/src/pytest_html/scripts/main.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -54,14 +54,29 @@
     table.appendChild(tableHeader)
 
     rows.forEach((row) => !!row && table.appendChild(row))
 
     table.querySelectorAll('.extra').forEach((item) => {
         item.colSpan = document.querySelectorAll('th').length
     })
+
+    const {
+        headerPops
+    } = manager.renderData
+    if (headerPops > 0) {
+        // remove 'headerPops' number of header columns
+        findAll('#results-table-head th').splice(-headerPops).forEach(column => column.remove())
+
+        // remove 'headerPops' number of row columns
+        const resultRows = findAll('.results-table-row')
+        resultRows.forEach((elem) => {
+            findAll('td:not(.extra)', elem).splice(-headerPops).forEach(column => column.remove())
+        })
+    }
+
     findAll('.sortable').forEach((elem) => {
         elem.addEventListener('click', (evt) => {
             const {
                 target: element
             } = evt
             const {
                 columnType
@@ -84,15 +99,20 @@
     const currentFilter = getVisible()
     possibleResults.forEach(({
         result,
         label
     }) => {
         const count = tests.filter((test) => test.result.toLowerCase() === result).length
         const input = document.querySelector(`input[data-test-result="${result}"]`)
+        const lastInput = document.querySelector(`input[data-test-result="${result}"]:last-of-type`)
         document.querySelector(`.${result}`).innerText = `${count} ${label}`
+        // add a comma and whitespace between the results
+        if (input !== lastInput) {
+            document.querySelector(`.${result}`).innerText += ', '
+        }
 
         input.disabled = !count
         input.checked = currentFilter.includes(result)
     })
 
     const numberOfTests = tests.filter(({
         result
```

### Comparing `pytest_html-4.0.0rc1/src/pytest_html/scripts/mediaviewer.js` & `pytest_html-4.0.0rc2/src/pytest_html/scripts/mediaviewer.js`

 * *Files identical despite different names*

### Comparing `pytest_html-4.0.0rc1/src/pytest_html/scripts/storage.js` & `pytest_html-4.0.0rc2/src/pytest_html/scripts/storage.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -73,25 +73,25 @@
 const getCollapsedCategory = (config) => {
     let categories
     if (typeof window !== 'undefined') {
         const url = new URL(window.location.href)
         const collapsedItems = new URLSearchParams(url.search).get('collapsed')
         switch (true) {
             case !config && collapsedItems === null:
-                categories = ['passed'];
-                break;
+                categories = ['passed']
+                break
             case collapsedItems?.length === 0 || /^["']{2}$/.test(collapsedItems):
-                categories = [];
-                break;
+                categories = []
+                break
             case /^all$/.test(collapsedItems) || (collapsedItems === null && /^all$/.test(config)):
-                categories = [...possibleFilters];
-                break;
+                categories = [...possibleFilters]
+                break
             default:
-                categories = collapsedItems?.split(',').map(item => item.toLowerCase()) || config;
-                break;
+                categories = collapsedItems?.split(',').map(item => item.toLowerCase()) || config
+                break
         }
     } else {
         categories = []
     }
     return categories
 }
```

### Comparing `pytest_html-4.0.0rc1/testing/legacy_test_pytest_html.py` & `pytest_html-4.0.0rc2/testing/legacy_test_pytest_html.py`

 * *Files identical despite different names*

### Comparing `pytest_html-4.0.0rc1/testing/test_integration.py` & `pytest_html-4.0.0rc2/testing/test_integration.py`

 * *Files 7% similar despite different names*

```diff
@@ -77,15 +77,15 @@
     number_of_tests = 0
     for outcome, number in args.items():
         if outcome == "total_tests":
             continue
         if isinstance(number, int):
             number_of_tests += number
             result = get_text(page, f"span[class={outcome}]")
-            assert_that(result).is_equal_to(f"{number} {OUTCOMES[outcome]}")
+            assert_that(result).matches(rf"{number} {OUTCOMES[outcome]}")
 
 
 def get_element(page, selector):
     return page.select_one(selector)
 
 
 def get_text(page, selector):
@@ -188,49 +188,125 @@
 
     def test_skip(self, pytester):
         reason = str(random.random())
         pytester.makepyfile(
             f"""
             import pytest
             def test_skip():
-                pytest.skip('{reason}')
+                pytest.skip("{reason}")
+        """
+        )
+        page = run(pytester)
+        assert_results(page, skipped=1, total_tests=0)
+
+        log = get_text(page, ".summary div[class='log']")
+        assert_that(log).contains(reason)
+
+    def test_skip_function_marker(self, pytester):
+        reason = str(random.random())
+        pytester.makepyfile(
+            f"""
+            import pytest
+            @pytest.mark.skip(reason="{reason}")
+            def test_skip():
+                assert True
+        """
+        )
+        page = run(pytester)
+        assert_results(page, skipped=1, total_tests=0)
+
+        log = get_text(page, ".summary div[class='log']")
+        assert_that(log).contains(reason)
+
+    def test_skip_class_marker(self, pytester):
+        reason = str(random.random())
+        pytester.makepyfile(
+            f"""
+            import pytest
+            @pytest.mark.skip(reason="{reason}")
+            class TestSkip:
+                def test_skip():
+                    assert True
         """
         )
         page = run(pytester)
         assert_results(page, skipped=1, total_tests=0)
 
         log = get_text(page, ".summary div[class='log']")
         assert_that(log).contains(reason)
 
     def test_fail(self, pytester):
         pytester.makepyfile("def test_fail(): assert False")
         page = run(pytester)
         assert_results(page, failed=1)
         assert_that(get_log(page)).contains("AssertionError")
+        assert_that(get_text(page, ".summary div[class='log'] span.error")).matches(
+            r"^E\s+assert False$"
+        )
 
     def test_xfail(self, pytester):
         reason = str(random.random())
         pytester.makepyfile(
             f"""
             import pytest
             def test_xfail():
-                pytest.xfail('{reason}')
+                pytest.xfail("{reason}")
         """
         )
         page = run(pytester)
         assert_results(page, xfailed=1)
         assert_that(get_log(page)).contains(reason)
 
+    def test_xfail_function_marker(self, pytester):
+        reason = str(random.random())
+        pytester.makepyfile(
+            f"""
+            import pytest
+            @pytest.mark.xfail(reason="{reason}")
+            def test_xfail():
+                assert False
+        """
+        )
+        page = run(pytester)
+        assert_results(page, xfailed=1)
+        assert_that(get_log(page)).contains(reason)
+
+    def test_xfail_class_marker(self, pytester):
+        pytester.makepyfile(
+            """
+            import pytest
+            @pytest.mark.xfail(reason="broken")
+            class TestXFail:
+                def test_xfail(self):
+                    assert False
+        """
+        )
+        page = run(pytester)
+        assert_results(page, xfailed=1)
+
     def test_xpass(self, pytester):
         pytester.makepyfile(
             """
             import pytest
             @pytest.mark.xfail()
             def test_xpass():
-                pass
+                assert True
+        """
+        )
+        page = run(pytester)
+        assert_results(page, xpassed=1)
+
+    def test_xpass_class_marker(self, pytester):
+        pytester.makepyfile(
+            """
+            import pytest
+            @pytest.mark.xfail()
+            class TestXPass:
+                def test_xpass(self):
+                    assert True
         """
         )
         page = run(pytester)
         assert_results(page, xpassed=1)
 
     def test_rerun(self, pytester):
         pytester.makepyfile(
@@ -512,14 +588,52 @@
         )
 
     def test_xdist(self, pytester):
         pytester.makepyfile("def test_xdist(): pass")
         page = run(pytester, cmd_flags=["-n1"])
         assert_results(page, passed=1)
 
+    def test_results_table_hook_append(self, pytester):
+        header_selector = (
+            ".summary #results-table-head tr:nth-child(1) th:nth-child({})"
+        )
+        row_selector = ".summary #results-table tr:nth-child(1) td:nth-child({})"
+
+        pytester.makeconftest(
+            """
+            def pytest_html_results_table_header(cells):
+                cells.append("<th>Description</th>")
+                cells.append(
+                    '<th class="sortable time" data-column-type="time">Time</th>'
+                )
+
+            def pytest_html_results_table_row(report, cells):
+                cells.append("<td>A description</td>")
+                cells.append('<td class="col-time">A time</td>')
+        """
+        )
+        pytester.makepyfile("def test_pass(): pass")
+        page = run(pytester)
+
+        description_index = 5
+        time_index = 6
+        assert_that(get_text(page, header_selector.format(time_index))).is_equal_to(
+            "Time"
+        )
+        assert_that(
+            get_text(page, header_selector.format(description_index))
+        ).is_equal_to("Description")
+
+        assert_that(get_text(page, row_selector.format(time_index))).is_equal_to(
+            "A time"
+        )
+        assert_that(get_text(page, row_selector.format(description_index))).is_equal_to(
+            "A description"
+        )
+
     def test_results_table_hook_insert(self, pytester):
         header_selector = (
             ".summary #results-table-head tr:nth-child(1) th:nth-child({})"
         )
         row_selector = ".summary #results-table tr:nth-child(1) td:nth-child({})"
 
         pytester.makeconftest(
@@ -535,21 +649,29 @@
                 cells.insert(2, "<td>A description</td>")
                 cells.insert(1, '<td class="col-time">A time</td>')
         """
         )
         pytester.makepyfile("def test_pass(): pass")
         page = run(pytester)
 
-        assert_that(get_text(page, header_selector.format(2))).is_equal_to("Time")
-        assert_that(get_text(page, header_selector.format(3))).is_equal_to(
-            "Description"
-        )
+        description_index = 3
+        time_index = 2
+        assert_that(get_text(page, header_selector.format(time_index))).is_equal_to(
+            "Time"
+        )
+        assert_that(
+            get_text(page, header_selector.format(description_index))
+        ).is_equal_to("Description")
 
-        assert_that(get_text(page, row_selector.format(2))).is_equal_to("A time")
-        assert_that(get_text(page, row_selector.format(3))).is_equal_to("A description")
+        assert_that(get_text(page, row_selector.format(time_index))).is_equal_to(
+            "A time"
+        )
+        assert_that(get_text(page, row_selector.format(description_index))).is_equal_to(
+            "A description"
+        )
 
     def test_results_table_hook_delete(self, pytester):
         pytester.makeconftest(
             """
             def pytest_html_results_table_row(report, cells):
                 if report.skipped:
                     del cells[:]
@@ -564,14 +686,35 @@
             def test_pass(): pass
 
         """
         )
         page = run(pytester)
         assert_results(page, passed=1)
 
+    def test_results_table_hook_pop(self, pytester):
+        pytester.makeconftest(
+            """
+            def pytest_html_results_table_header(cells):
+                cells.pop()
+
+            def pytest_html_results_table_row(report, cells):
+                cells.pop()
+        """
+        )
+        pytester.makepyfile("def test_pass(): pass")
+        page = run(pytester)
+
+        header_columns = page.select(".summary #results-table-head th")
+        assert_that(header_columns).is_length(3)
+
+        row_columns = page.select_one(".summary .results-table-row").select(
+            "td:not(.extra)"
+        )
+        assert_that(row_columns).is_length(3)
+
     @pytest.mark.parametrize("no_capture", ["", "-s"])
     def test_standard_streams(self, pytester, no_capture):
         pytester.makepyfile(
             """
             import pytest
             import sys
             @pytest.fixture
```

### Comparing `pytest_html-4.0.0rc1/testing/test_unit.py` & `pytest_html-4.0.0rc2/testing/test_unit.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,23 +20,7 @@
     pytester.makepyfile("def test_pass(): pass")
     result = run(pytester)
     result.stdout.fnmatch_lines(
         [
             "*DeprecationWarning: 'duration_formatter'*",
         ],
     )
-
-
-def test_cells_pop_deprecation_warning(pytester):
-    pytester.makeconftest(
-        """
-        def pytest_html_results_table_row(cells):
-            cells.pop()
-    """
-    )
-    pytester.makepyfile("def test_pass(): pass")
-    result = run(pytester)
-    result.stdout.fnmatch_lines(
-        [
-            "*DeprecationWarning: 'pop' is deprecated*",
-        ],
-    )
```

### Comparing `pytest_html-4.0.0rc1/testing/unittest.js` & `pytest_html-4.0.0rc2/testing/unittest.js`

 * *Files 13% similar despite different names*

#### js-beautify {}

```diff
@@ -7,15 +7,16 @@
     doFilter
 } = require('../src/pytest_html/scripts/filter.js')
 const {
     doInitSort,
     doSort
 } = require('../src/pytest_html/scripts/sort.js')
 const {
-    formatDuration
+    formatDuration,
+    transformTableObj
 } = require('../src/pytest_html/scripts/utils.js')
 const dataModule = require('../src/pytest_html/scripts/datamanager.js')
 const storageModule = require('../src/pytest_html/scripts/storage.js')
 
 
 const setTestData = () => {
     const jsonDatan = {
@@ -112,15 +113,15 @@
             managerSpy = sinon.spy(dataModule.manager, 'setRender')
 
             doInitSort()
             expect(managerSpy.callCount).to.eql(1)
             expect(dataModule.manager.testSubset.map(({
                 result
             }) => result)).to.eql([
-                'passed', 'failed', 'passed', 'passed', 'passed', 'passed',
+                'failed', 'passed', 'passed', 'passed', 'passed', 'passed',
             ])
         })
         it('has stored sort preference', () => {
             sortMock = sinon.stub(storageModule, 'getSort').returns('result')
             sortDirectionMock = sinon.stub(storageModule, 'getSortDirection').returns(false)
             managerSpy = sinon.spy(dataModule.manager, 'setRender')
 
@@ -128,14 +129,27 @@
             expect(managerSpy.callCount).to.eql(1)
             expect(dataModule.manager.testSubset.map(({
                 result
             }) => result)).to.eql([
                 'failed', 'passed', 'passed', 'passed', 'passed', 'passed',
             ])
         })
+        it('keeps original test execution order', () => {
+            sortMock = sinon.stub(storageModule, 'getSort').returns('original')
+            sortDirectionMock = sinon.stub(storageModule, 'getSortDirection').returns(false)
+            managerSpy = sinon.spy(dataModule.manager, 'setRender')
+
+            doInitSort()
+            expect(managerSpy.callCount).to.eql(1)
+            expect(dataModule.manager.testSubset.map(({
+                result
+            }) => result)).to.eql([
+                'passed', 'failed', 'passed', 'passed', 'passed', 'passed',
+            ])
+        })
     })
     describe('doSort', () => {
         let getSortMock
         let setSortMock
         let getSortDirectionMock
         let setSortDirection
         let managerSpy
@@ -169,14 +183,58 @@
             expect(formatDuration(0.999).ms).to.eql('999 ms')
         })
         it('handles larger durations', () => {
             expect(formatDuration(1.234).formatted).to.eql('00:00:01')
             expect(formatDuration(12345.678).formatted).to.eql('03:25:46')
         })
     })
+    describe('transformTableObj', () => {
+        it('handles empty object', () => {
+            expect(transformTableObj({})).to.eql({
+                appends: {},
+                inserts: {}
+            })
+        })
+        it('handles no appends', () => {
+            const expected = {
+                1: "hello",
+                2: "goodbye"
+            }
+            expect(transformTableObj(expected)).to.eql({
+                appends: {},
+                inserts: expected
+            })
+        })
+        it('handles no inserts', () => {
+            const expected = {
+                "Z1": "hello",
+                "Z2": "goodbye"
+            }
+            expect(transformTableObj(expected)).to.eql({
+                appends: expected,
+                inserts: {}
+            })
+        })
+        it('handles both', () => {
+            const expected = {
+                appends: {
+                    "Z1": "hello",
+                    "Z2": "goodbye"
+                },
+                inserts: {
+                    1: "mee",
+                    2: "moo"
+                }
+            }
+            expect(transformTableObj({
+                ...expected.appends,
+                ...expected.inserts
+            })).to.eql(expected)
+        })
+    })
 })
 
 describe('Storage tests', () => {
     describe('getCollapsedCategory', () => {
         let originalWindow
         const mockWindow = (queryParam) => {
             const mock = {
```

### Comparing `pytest_html-4.0.0rc1/.gitignore` & `pytest_html-4.0.0rc2/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest_html-4.0.0rc1/README.rst` & `pytest_html-4.0.0rc2/README.rst`

 * *Files identical despite different names*

### Comparing `pytest_html-4.0.0rc1/pyproject.toml` & `pytest_html-4.0.0rc2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -54,25 +54,31 @@
   "assertpy>=1.1",
   "beautifulsoup4>=4.11.1",
   "black>=22.1.0",
   "flake8>=4.0.1",
   "pre-commit>=2.17.0",
   "pytest-xdist>=2.4.0",
   "pytest-mock>=3.7.0",
+  "pytest-rerunfailures>=11.1.2",
   "selenium>=4.3.0",
   "tox>=3.24.5",
 ]
 
 [project.urls]
 Homepage = "https://github.com/pytest-dev/pytest-html"
 Tracker = "https://github.com/pytest-dev/pytest-html/issues"
 Source = "https://github.com/pytest-dev/pytest-html"
 
 [project.entry-points.pytest11]
-env = "pytest_html.plugin"
+html = "pytest_html.plugin"
+
+[tool.hatch.envs.test]
+features = [
+  "test",
+]
 
 [tool.hatch.version]
 source = "vcs"
 
 [tool.hatch.build.targets.wheel]
 exclude = [
   "src/pytest_html/scripts/*",
```

### Comparing `pytest_html-4.0.0rc1/PKG-INFO` & `pytest_html-4.0.0rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-html
-Version: 4.0.0rc1
+Version: 4.0.0rc2
 Summary: pytest plugin for generating HTML reports
 Project-URL: Homepage, https://github.com/pytest-dev/pytest-html
 Project-URL: Tracker, https://github.com/pytest-dev/pytest-html/issues
 Project-URL: Source, https://github.com/pytest-dev/pytest-html
 Author-email: Dave Hunt <dhunt@mozilla.com>, Jim Brannlund <jimbrannlund@fastmail.com>
 License-Expression: MPL-2.0
 License-File: LICENSE
@@ -34,14 +34,15 @@
 Provides-Extra: test
 Requires-Dist: assertpy>=1.1; extra == 'test'
 Requires-Dist: beautifulsoup4>=4.11.1; extra == 'test'
 Requires-Dist: black>=22.1.0; extra == 'test'
 Requires-Dist: flake8>=4.0.1; extra == 'test'
 Requires-Dist: pre-commit>=2.17.0; extra == 'test'
 Requires-Dist: pytest-mock>=3.7.0; extra == 'test'
+Requires-Dist: pytest-rerunfailures>=11.1.2; extra == 'test'
 Requires-Dist: pytest-xdist>=2.4.0; extra == 'test'
 Requires-Dist: selenium>=4.3.0; extra == 'test'
 Requires-Dist: tox>=3.24.5; extra == 'test'
 Description-Content-Type: text/x-rst
 
 pytest-html
 ===========
```

