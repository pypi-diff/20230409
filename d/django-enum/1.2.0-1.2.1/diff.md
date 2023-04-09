# Comparing `tmp/django_enum-1.2.0.tar.gz` & `tmp/django_enum-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_enum-1.2.0.tar", max compression
+gzip compressed data, was "django_enum-1.2.1.tar", max compression
```

## Comparing `django_enum-1.2.0.tar` & `django_enum-1.2.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1073 2023-02-16 06:02:21.980862 django_enum-1.2.0/LICENSE
--rw-r--r--   0        0        0     7902 2023-04-03 01:58:42.418174 django_enum-1.2.0/README.rst
--rw-r--r--   0        0        0     1476 2023-04-03 02:00:53.705404 django_enum-1.2.0/django_enum/__init__.py
--rw-r--r--   0        0        0     5565 2023-04-02 23:07:31.209203 django_enum-1.2.0/django_enum/choices.py
--rw-r--r--   0        0        0     2886 2023-04-02 23:06:37.543722 django_enum-1.2.0/django_enum/drf.py
--rw-r--r--   0        0        0    14122 2023-04-03 01:16:57.593960 django_enum-1.2.0/django_enum/fields.py
--rw-r--r--   0        0        0     3008 2023-04-02 23:06:37.549687 django_enum-1.2.0/django_enum/filters.py
--rw-r--r--   0        0        0     7949 2023-04-03 01:46:33.467216 django_enum-1.2.0/django_enum/forms.py
--rw-r--r--   0        0        0     2527 2023-04-03 02:00:53.695960 django_enum-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     9123 1970-01-01 00:00:00.000000 django_enum-1.2.0/setup.py
--rw-r--r--   0        0        0     9949 1970-01-01 00:00:00.000000 django_enum-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-02-16 06:02:21.980862 django_enum-1.2.1/LICENSE
+-rw-r--r--   0        0        0     7902 2023-04-03 01:58:42.418174 django_enum-1.2.1/README.rst
+-rw-r--r--   0        0        0     1476 2023-04-09 05:16:33.260336 django_enum-1.2.1/django_enum/__init__.py
+-rw-r--r--   0        0        0     5565 2023-04-02 23:07:31.209203 django_enum-1.2.1/django_enum/choices.py
+-rw-r--r--   0        0        0     2886 2023-04-02 23:06:37.543722 django_enum-1.2.1/django_enum/drf.py
+-rw-r--r--   0        0        0    14122 2023-04-03 01:16:57.593960 django_enum-1.2.1/django_enum/fields.py
+-rw-r--r--   0        0        0     3008 2023-04-02 23:06:37.549687 django_enum-1.2.1/django_enum/filters.py
+-rw-r--r--   0        0        0     7949 2023-04-03 01:46:33.467216 django_enum-1.2.1/django_enum/forms.py
+-rw-r--r--   0        0        0     2561 2023-04-09 05:21:11.101621 django_enum-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     9123 1970-01-01 00:00:00.000000 django_enum-1.2.1/setup.py
+-rw-r--r--   0        0        0     9988 1970-01-01 00:00:00.000000 django_enum-1.2.1/PKG-INFO
```

### Comparing `django_enum-1.2.0/LICENSE` & `django_enum-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_enum-1.2.0/README.rst` & `django_enum-1.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `django_enum-1.2.0/django_enum/__init__.py` & `django_enum-1.2.1/django_enum/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,14 +43,14 @@
     'FloatChoices',
     'DjangoEnumPropertiesMeta',
     'EnumChoiceField',
     'FilterSet',
     'EnumFilter'
 ]
 
-VERSION = (1, 2, 0)
+VERSION = (1, 2, 1)
 
 __title__ = 'Django Enum'
 __version__ = '.'.join(str(i) for i in VERSION)
 __author__ = 'Brian Kohan'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2022-2023 Brian Kohan'
```

### Comparing `django_enum-1.2.0/django_enum/choices.py` & `django_enum-1.2.1/django_enum/choices.py`

 * *Files identical despite different names*

### Comparing `django_enum-1.2.0/django_enum/drf.py` & `django_enum-1.2.1/django_enum/drf.py`

 * *Files identical despite different names*

### Comparing `django_enum-1.2.0/django_enum/fields.py` & `django_enum-1.2.1/django_enum/fields.py`

 * *Files identical despite different names*

### Comparing `django_enum-1.2.0/django_enum/filters.py` & `django_enum-1.2.1/django_enum/filters.py`

 * *Files identical despite different names*

### Comparing `django_enum-1.2.0/django_enum/forms.py` & `django_enum-1.2.1/django_enum/forms.py`

 * *Files identical despite different names*

### Comparing `django_enum-1.2.0/pyproject.toml` & `django_enum-1.2.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-enum"
-version = "1.2.0"
+version = "1.2.1"
 description = "Full and natural support for enumerations as Django model fields."
 authors = ["Brian Kohan <bckohan@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/bckohan/django-enum"
 homepage = "https://django-enum.readthedocs.io"
 readme = "README.rst"
 keywords = ["enum",  "properties", "defines", "field", "django", "database"]
@@ -12,14 +12,15 @@
     "Environment :: Console",
     "Framework :: Django",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Development Status :: 5 - Production/Stable",
     "Framework :: Django :: 3.2",
     "Framework :: Django :: 4.0",
+    "Framework :: Django :: 4.2",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
@@ -43,15 +44,15 @@
 django-filter = {version = ">=21,<24", optional = true}
 djangorestframework = {version = "^3.9", optional = true}
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.0"
 Sphinx = "^5.0.2"
 sphinx-rtd-theme = "^1.0.0"
-mypy = ">=0.971,<1.2"
+mypy = ">=0.971,<1.3"
 isort = "^5.6.4"
 doc8 = "^0.11.0"
 darglint = "^1.5.7"
 pytest-cov = "^4.0.0"
 pylint = "^2.6.0"
 sphinx-argparse = "^0.3.0"
 deepdiff = ">=5.2.3,<7.0.0"
```

### Comparing `django_enum-1.2.0/setup.py` & `django_enum-1.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
          'djangorestframework>=3.9,<4.0'],
  'djangorestframework': ['djangorestframework>=3.9,<4.0'],
  'filters': ['django-filter>=21,<24'],
  'properties': ['enum-properties>=1.2.0,<2.0.0']}
 
 setup_kwargs = {
     'name': 'django-enum',
-    'version': '1.2.0',
+    'version': '1.2.1',
     'description': 'Full and natural support for enumerations as Django model fields.',
     'long_description': "|MIT license| |PyPI version fury.io| |PyPI pyversions| |PyPI status| |Documentation Status|\n|Code Cov| |Test Status|\n\n.. |MIT license| image:: https://img.shields.io/badge/License-MIT-blue.svg\n   :target: https://lbesson.mit-license.org/\n\n.. |PyPI version fury.io| image:: https://badge.fury.io/py/django-enum.svg\n   :target: https://pypi.python.org/pypi/django-enum/\n\n.. |PyPI pyversions| image:: https://img.shields.io/pypi/pyversions/django-enum.svg\n   :target: https://pypi.python.org/pypi/django-enum/\n\n.. |PyPI status| image:: https://img.shields.io/pypi/status/django-enum.svg\n   :target: https://pypi.python.org/pypi/django-enum\n\n.. |Documentation Status| image:: https://readthedocs.org/projects/django-enum/badge/?version=latest\n   :target: http://django-enum.readthedocs.io/?badge=latest/\n\n.. |Code Cov| image:: https://codecov.io/gh/bckohan/django-enum/branch/main/graph/badge.svg?token=0IZOKN2DYL\n   :target: https://codecov.io/gh/bckohan/django-enum\n\n.. |Test Status| image:: https://github.com/bckohan/django-enum/workflows/test/badge.svg\n   :target: https://github.com/bckohan/django-enum/actions\n\n\n.. _Django: https://www.djangoproject.com/\n.. _GitHub: https://github.com/bckohan/django-enum\n.. _PyPI: https://pypi.python.org/pypi/django-enum\n.. _Enum: https://docs.python.org/3/library/enum.html#enum.Enum\n.. _enumerations: https://docs.python.org/3/library/enum.html#enum.Enum\n.. _ValueError: https://docs.python.org/3/library/exceptions.html#ValueError\n.. _DRY: https://en.wikipedia.org/wiki/Don%27t_repeat_yourself\n\nDjango Enum\n###########\n\nFull and natural support for enumerations_ as Django model fields.\n\nMany packages aim to ease usage of Python enumerations as model fields. Most\nwere made obsolete when Django provided ``TextChoices`` and ``IntegerChoices``\ntypes. The motivation for `django-enum <https://django-enum.readthedocs.io/en/latest/>`_\nwas to:\n\n* Always automatically coerce fields to instances of the Enum type.\n* Allow strict adherence to Enum values to be disabled.\n* Be compatible with Enum classes that do not derive from Django's Choices.\n* Handle migrations appropriately. (See `migrations <https://django-enum.readthedocs.io/en/latest/usage.html#migrations>`_)\n* Integrate as fully as possible with Django_'s existing level of enum support.\n* Integrate with `enum-properties <https://pypi.org/project/enum-properties/>`_ to enable richer enumeration types.\n* Represent enum fields with the smallest possible column type.\n* Be as simple and light-weight an extension to core Django as possible.\n\n`django-enum <https://django-enum.readthedocs.io/en/latest/>`_ works in concert\nwith Django_'s built in ``TextChoices`` and ``IntegerChoices`` to provide a\nnew model field type, ``EnumField``, that resolves the correct native Django_\nfield type for the given enumeration based on its value type and range. For\nexample, ``IntegerChoices`` that contain values between 0 and 32767 become\n`PositiveSmallIntegerField <https://docs.djangoproject.com/en/stable/ref/models/fields/#positivesmallintegerfield>`_.\n\n.. code:: python\n\n    from django.db import models\n    from django_enum import EnumField\n\n    class MyModel(models.Model):\n\n        class TextEnum(models.TextChoices):\n\n            VALUE0 = 'V0', 'Value 0'\n            VALUE1 = 'V1', 'Value 1'\n            VALUE2 = 'V2', 'Value 2'\n\n        class IntEnum(models.IntegerChoices):\n\n            ONE   = 1, 'One'\n            TWO   = 2, 'Two',\n            THREE = 3, 'Three'\n\n        # this is equivalent to:\n        #  CharField(max_length=2, choices=TextEnum.choices, null=True, blank=True)\n        txt_enum = EnumField(TextEnum, null=True, blank=True)\n\n        # this is equivalent to\n        #  PositiveSmallIntegerField(choices=IntEnum.choices)\n        int_enum = EnumField(IntEnum)\n\n\n``EnumField`` **is more than just an alias. The fields are now assignable and\naccessible as their enumeration type rather than by-value:**\n\n.. code:: python\n\n    instance = MyModel.objects.create(\n        txt_enum=MyModel.TextEnum.VALUE1,\n        int_enum=3  # by-value assignment also works\n    )\n\n    assert instance.txt_enum == MyModel.TextEnum('V1')\n    assert instance.txt_enum.label == 'Value 1'\n\n    assert instance.int_enum == MyModel.IntEnum['THREE']\n    assert instance.int_enum.value == 3\n\n\n`django-enum <https://django-enum.readthedocs.io/en/latest/>`_ also provides\n``IntegerChoices`` and ``TextChoices`` types that extend from\n`enum-properties <https://pypi.org/project/enum-properties/>`_ which makes\npossible very rich enumeration fields.\n\n``?> pip install enum-properties``\n\n.. code:: python\n\n    from enum_properties import s\n    from django_enum import TextChoices  # use instead of Django's TextChoices\n    from django.db import models\n\n    class TextChoicesExample(models.Model):\n\n        class Color(TextChoices, s('rgb'), s('hex', case_fold=True)):\n\n            # name   value   label       rgb       hex\n            RED     = 'R',   'Red',   (1, 0, 0), 'ff0000'\n            GREEN   = 'G',   'Green', (0, 1, 0), '00ff00'\n            BLUE    = 'B',   'Blue',  (0, 0, 1), '0000ff'\n\n            # any named s() values in the Enum's inheritance become properties on\n            # each value, and the enumeration value may be instantiated from the\n            # property's value\n\n        color = EnumField(Color)\n\n    instance = TextChoicesExample.objects.create(\n        color=TextChoicesExample.Color('FF0000')\n    )\n    assert instance.color == TextChoicesExample.Color('Red')\n    assert instance.color == TextChoicesExample.Color('R')\n    assert instance.color == TextChoicesExample.Color((1, 0, 0))\n\n    # direct comparison to any symmetric value also works\n    assert instance.color == 'Red'\n    assert instance.color == 'R'\n    assert instance.color == (1, 0, 0)\n\n    # save by any symmetric value\n    instance.color = 'FF0000'\n\n    # access any enum property right from the model field\n    assert instance.color.hex == 'ff0000'\n\n    # this also works!\n    assert instance.color == 'ff0000'\n\n    # and so does this!\n    assert instance.color == 'FF0000'\n\n    instance.save()\n\n    # filtering works by any symmetric value or enum type instance\n    assert TextChoicesExample.objects.filter(\n        color=TextChoicesExample.Color.RED\n    ).first() == instance\n\n    assert TextChoicesExample.objects.filter(color=(1, 0, 0)).first() == instance\n\n    assert TextChoicesExample.objects.filter(color='FF0000').first() == instance\n\n\n.. note::\n\n    Consider using\n    `django-render-static <https://pypi.org/project/django-render-static/>`_\n    to make your enumerations DRY_ across the full stack!\n\nPlease report bugs and discuss features on the\n`issues page <https://github.com/bckohan/django-enum/issues>`_.\n\n`Contributions <https://github.com/bckohan/django-enum/blob/main/CONTRIBUTING.rst>`_\nare encouraged!\n\n`Full documentation at read the docs. <https://django-enum.readthedocs.io/en/latest/>`_\n\nInstallation\n------------\n\n1. Clone django-enum from GitHub_ or install a release off PyPI_ :\n\n.. code:: bash\n\n       pip install django-enum\n\n.. note::\n\n    ``django-enum`` has several optional dependencies that are not pulled in\n    by default. ``EnumFields`` work seamlessly with all Django apps that\n    work with model fields with choices without any additional work. Optional\n    integrations are provided with several popular libraries to extend this\n    basic functionality.\n\nIntegrations are provided that leverage\n`enum-properties <https://pypi.org/project/enum-properties/>`_ to make\nenumerations do more work and to provide extended functionality for\n`django-filter <https://pypi.org/project/django-filter/>`_  and\n`djangorestframework <https://www.django-rest-framework.org>`_.\n\n.. code:: bash\n\n    pip install enum-properties\n    pip install django-filter\n    pip install djangorestframework\n\nIf features are utilized that require a missing optional dependency an\nexception will be thrown.\n",
     'author': 'Brian Kohan',
     'author_email': 'bckohan@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://django-enum.readthedocs.io',
```

### Comparing `django_enum-1.2.0/PKG-INFO` & `django_enum-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: django-enum
-Version: 1.2.0
+Version: 1.2.1
 Summary: Full and natural support for enumerations as Django model fields.
 Home-page: https://django-enum.readthedocs.io
 License: MIT
 Keywords: enum,properties,defines,field,django,database
 Author: Brian Kohan
 Author-email: bckohan@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

