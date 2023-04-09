# Comparing `tmp/enum_properties-1.3.3.tar.gz` & `tmp/enum_properties-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enum_properties-1.3.3.tar", max compression
+gzip compressed data, was "enum_properties-1.4.0.tar", max compression
```

## Comparing `enum_properties-1.3.3.tar` & `enum_properties-1.4.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1073 2023-02-16 05:48:06.639467 enum_properties-1.3.3/LICENSE
--rw-r--r--   0        0        0     3645 2022-07-19 05:34:10.648215 enum_properties-1.3.3/README.rst
--rw-r--r--   0        0        0    20084 2023-02-16 05:48:44.591427 enum_properties-1.3.3/enum_properties/__init__.py
--rw-r--r--   0        0        0     1831 2023-02-16 05:48:06.649524 enum_properties-1.3.3/pyproject.toml
--rw-r--r--   0        0        0     4373 1970-01-01 00:00:00.000000 enum_properties-1.3.3/setup.py
--rw-r--r--   0        0        0     5077 1970-01-01 00:00:00.000000 enum_properties-1.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-02-16 05:48:06.639467 enum_properties-1.4.0/LICENSE
+-rw-r--r--   0        0        0     4345 2023-04-08 09:04:38.023115 enum_properties-1.4.0/README.rst
+-rw-r--r--   0        0        0    22470 2023-04-09 03:39:36.450011 enum_properties-1.4.0/enum_properties/__init__.py
+-rw-r--r--   0        0        0     1878 2023-04-09 03:44:31.094954 enum_properties-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     5130 1970-01-01 00:00:00.000000 enum_properties-1.4.0/setup.py
+-rw-r--r--   0        0        0     5804 1970-01-01 00:00:00.000000 enum_properties-1.4.0/PKG-INFO
```

### Comparing `enum_properties-1.3.3/LICENSE` & `enum_properties-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `enum_properties-1.3.3/README.rst` & `enum_properties-1.4.0/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -80,14 +80,44 @@
     Color('00ff00') == Color.GREEN
     Color('00FF00') == Color.GREEN
     Color('0000ff') == Color.BLUE
     Color('0000FF') == Color.BLUE
 
     Color.RED.hex == 'ff0000'
 
+
+Member functions may also be specialized to each enumeration value, using the
+@specialize decorator.
+
+.. code:: python
+
+    from enum_properties import EnumProperties, specialize
+
+    class SpecializedEnum(EnumProperties):
+
+        ONE   = 1
+        TWO   = 2
+        THREE = 3
+
+        @specialize(ONE)
+        def method(self):
+            return 'method_one()'
+
+        @specialize(TWO)
+        def method(self):
+            return 'method_two()'
+
+        @specialize(THREE)
+        def method(self):
+            return 'method_three()'
+
+    SpecializedEnum.ONE.method() == 'method_one()'
+    SpecializedEnum.TWO.method() == 'method_two()'
+    SpecializedEnum.THREE.method() == 'method_three()'
+
 Please report bugs and discuss features on the
 `issues page <https://github.com/bckohan/enum-properties/issues>`_.
 
 `Contributions <https://github.com/bckohan/enum-properties/blob/main/CONTRIBUTING.rst>`_ are
 encouraged!
 
 `Full documentation at read the docs. <https://enum-properties.readthedocs.io/en/latest/>`_
```

### Comparing `enum_properties-1.3.3/enum_properties/__init__.py` & `enum_properties-1.4.0/enum_properties/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,16 @@
    ____                  ___                        __  _
   / __/__  __ ____ _    / _ \_______  ___  ___ ____/ /_(_)__ ___
  / _// _ \/ // /  ' \  / ___/ __/ _ \/ _ \/ -_) __/ __/ / -_|_-<
 /___/_//_/\_,_/_/_/_/ /_/  /_/  \___/ .__/\__/_/  \__/_/\__/___/
                                    /_/
 *******************************************************************************
 
-Metaprogramming and mixin tools that implement property tuple support for
-python enumeration classes.
+Metaprogramming and mixin tools that implement property tuple and method
+specialization support for python enumeration classes.
 
 .. todo::
     Given how dynamic the typing is in this module, static type checking is
     awkward - revisit in the future if advances warrant it.
 
 """
 import enum
@@ -27,15 +27,15 @@
 try:
     from functools import cached_property
 except ImportError:  # pragma: no cover
     # todo remove when python 3.7 support is dropped
     cached_property = property  # pylint: disable=C0103
 
 
-VERSION = (1, 3, 3)
+VERSION = (1, 4, 0)
 
 __title__ = 'Enum Properties'
 __version__ = '.'.join(str(i) for i in VERSION)
 __author__ = 'Brian Kohan'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2022-2023 Brian Kohan'
 
@@ -44,14 +44,15 @@
     'EnumProperties',
     'IntEnumProperties',
     'FlagProperties',
     'IntFlagProperties',
     'EnumPropertiesMeta',
     'SymmetricMixin',
     'DecomposeMixin',
+    'specialize',
     'p',
     's'
 ]
 
 
 def _do_casenorm(text):
     """Normalize unicode text to be case agnostic."""
@@ -104,14 +105,41 @@
 
     :param prop_name: The name of the property
     :return: a named property class
     """
     return type(prop_name, (_Prop,), {'symmetric': False})
 
 
+class _Specialized:  # pylint: disable=R0903
+    """
+    A member specialization identifier class - private. Used to wrap
+    specialized member functions and tag them with their enum values so the
+    Enum classdict can identify them.
+
+    :param wrapped: The wrapped member function
+    :param value: The value to specialize for
+    """
+    def __init__(self, wrapped, value):
+        self.wrapped = wrapped
+        self.value = value
+
+
+def specialize(value):
+    """
+    A decorator to specialize a method for a given enumeration value.
+
+    :param value: The enumeration value to specialize
+    :return: A decorated specialized member method
+    """
+    def specialize_decorator(method):
+        return _Specialized(method, value)
+
+    return specialize_decorator
+
+
 class SymmetricMixin:  # pylint: disable=R0903
     """
     This mixin enables symmetric Enum_ creation from properties marked
     symmetric. It is included by default in the
     :py:class:`~enum_properties.EnumProperties` base class, but can be
     disabled by overriding ``_missing_`` and explicitly skipping it.
 
@@ -245,22 +273,22 @@
     """
 
     # members expected to be supplied by inheriting classes
     EXPECTED = ['_symmetric_builtins_']
 
     # members reserved for use by EnumProperties
     RESERVED = [
-        'enum_properties',
+        '_properties_',
         '_ep_coerce_types_',
         '_ep_symmetric_map_',
         '_ep_isymmetric_map_'
     ]
 
     @classmethod
-    def __prepare__(mcs, cls, bases):  # pylint: disable=W0221
+    def __prepare__(mcs, cls, bases, **kwargs):  # pylint: disable=W0221,R0915
         """
         Strip properties out of inheritance and record them on our class
         dictionary for per-value based assignment in ``__new__``.
 
         :raises ValueError: If a reserved name is present as either a property
             or a member, or if the number of specified properties does not
             match the number of listed property values in the value tuples.
@@ -278,37 +306,40 @@
                     EnumPropertiesMeta.EXPECTED
                 ):
                     raise ValueError(f'{base.name()} is reserved.')
                 properties[base()] = []
             else:
                 real_bases.append(base)
 
-        class_dict = super().__prepare__(cls, tuple(real_bases))
+        class_dict = super().__prepare__(cls, tuple(real_bases), **kwargs)
 
         class _PropertyEnumDict(class_dict.__class__):
             """
             This wrapper class is used to strip properties off of the
             enumeration values and capture them as they are set into the class
             dictionary. Wrapping the private enumeration code and delegating
             all of the existing functionality to the delegate allows a light
             touch that should be robust to future changes in enum.
             """
 
             _ep_properties_ = properties
             _ep_symmetric_properties = symmetric_properties
+            _specialized_ = {}
 
             def __init__(self):
                 super().__init__()
                 for attr in set(dir(class_dict)).difference(set(dir(self))):
                     setattr(self, attr, getattr(class_dict, attr))
                 for item, value in class_dict.items():
                     self[item] = value
 
             def __setitem__(self, key, value):
-                if key in EnumPropertiesMeta.EXPECTED:
+                if isinstance(value, _Specialized):
+                    self._specialized_.setdefault(value.value, {})[key] = value
+                elif key in EnumPropertiesMeta.EXPECTED:
                     dict.__setitem__(self, key, value)
                 elif key in EnumPropertiesMeta.RESERVED:
                     raise ValueError(f'{key} is reserved.')
                 elif self._ep_properties_:
                     # are we an enum value? - just kick this up to parent class
                     # logic, this code runs once on load - its fine that it's
                     # doing a little redundant work and doing it this way
@@ -346,15 +377,15 @@
                         except TypeError as type_err:
                             raise ValueError(
                                 f'{key} must have {len(self._ep_properties_)} '
                                 f'property values.'
                             ) from type_err
 
                     elif key in class_dict._member_names:
-                        remove = True
+                        remove = True  # pragma: no cover
 
                     super().__setitem__(key, value)
 
                     if remove:
                         # todo remove when minimum python >= 3.13
                         # base class lets nested classes through! see:
                         # https://github.com/bckohan/enum-properties/issues/29
@@ -371,39 +402,53 @@
 
         return _PropertyEnumDict()
 
     def __new__(  # pylint: disable=W0221
             mcs,
             classname,
             bases,
-            classdict
+            classdict,
+            **kwargs
     ):
         """
         Enumeration class construction runs in the following stages:
 
         1) pass up the inheritance tree to build the initial enumeration class.
-        2) Add property value to enumeration value maps for each property and
+        2) Add method specializations to each class
+        3) Add property value to enumeration value maps for each property and
             the property accessors that use them
-        3) Add casefolded symmetric maps for any symmetric properties
-        4) Add any symmetric builtin properties to our symmetric maps
+        4) Add casefolded symmetric maps for any symmetric properties
+        5) Add any symmetric builtin properties to our symmetric maps
 
         :raises ValueError: if ``_symmetric_builtins_`` is specified
             incorrectly, or if non-hashable values are provided for a
             symmetric property.
         """
         cls = super().__new__(
             mcs,
             classname,
             tuple(base for base in bases if not issubclass(base, _Prop)),
-            classdict
+            classdict,
+            **kwargs
         )
         cls._ep_coerce_types_ = []
         cls._ep_symmetric_map_ = cls._member_map_
         cls._ep_isymmetric_map_ = {}
-        cls.enum_properties = list(classdict._ep_properties_.keys())
+        cls._properties_ = list(classdict._ep_properties_.keys())
+
+        for val in cls:
+            for member_name, specialization in classdict._specialized_.get(
+                    val.value, {}
+            ).items():
+                # use descriptor binding
+                setattr(
+                    val,
+                    member_name,
+                    specialization.wrapped.__get__(val)
+                )
 
         def add_sym_lookup(prop, p_val, enum_inst):
             if not isinstance(p_val, Hashable):
                 raise ValueError(
                     f'{cls}.{prop}:{p_val} is not hashable. Symmetrical '
                     f'enumeration properties must be hashable or a list of '
                     f'hashable values.'
@@ -418,33 +463,26 @@
                 isinstance(typ, Hashable) and not issubclass(typ, cls)
             ):
                 cls._ep_coerce_types_.append(typ)
 
         for val in cls:
             add_coerce_type(type(val.value))
 
-        for prop in cls.enum_properties:
-            values = classdict._ep_properties_[prop]
-            setattr(
-                cls,
-                f'_value2{prop}_map_',
-                dict(zip(cls._value2member_map_, values))
-            )
-            setattr(
-                cls,
-                prop,
-                property(
-                    lambda self, prop=prop:
-                    getattr(cls, f'_value2{prop}_map_').get(self.value)
+        # set properties onto the members
+        for idx, member in enumerate(cls.__members__.values()):
+            for prop, values in classdict._ep_properties_.items():
+                setattr(
+                    member,
+                    prop,
+                    values[idx]
                 )
-            )
 
         # we reverse to maintain precedence order for symmetric lookups
         for prop in reversed([
-            prop for prop in cls.enum_properties if prop.symmetric
+            prop for prop in cls._properties_ if prop.symmetric
         ]):
             for idx, val in enumerate(
                 reversed(classdict._ep_properties_[prop])
             ):
                 enum_cls = list(cls._value2member_map_.values())[
                     len(cls._value2member_map_)-1-idx
                 ]
@@ -576,17 +614,53 @@
     enum.Flag,
     metaclass=EnumPropertiesMeta
 ):
     """
     A Flag that supports properties
     """
 
+    def _generate_next_value_(
+            name,
+            start,
+            count,
+            last_values
+    ):  # pylint: disable=E0213
+        """
+        Intermixed property tuples can corrupt the last_values list with
+        tuples. This method ensures only ints are present in last_values and
+        delegates to the super class.
+        """
+        return enum.Flag._generate_next_value_(
+            name,
+            start,
+            count,
+            [val[0] if isinstance(val, tuple) else val for val in last_values]
+        )
+
 
 class IntFlagProperties(
     DecomposeMixin,
     SymmetricMixin,
     enum.IntFlag,
     metaclass=EnumPropertiesMeta
 ):
     """
     An IntFlag that supports properties.
     """
+
+    def _generate_next_value_(
+            name,
+            start,
+            count,
+            last_values
+    ):  # pylint: disable=E0213
+        """
+        Intermixed property tuples can corrupt the last_values list with
+        tuples. This method ensures only ints are present in last_values and
+        delegates to the super class.
+        """
+        return enum.IntFlag._generate_next_value_(
+            name,
+            start,
+            count,
+            [val[0] if isinstance(val, tuple) else val for val in last_values]
+        )
```

### Comparing `enum_properties-1.3.3/pyproject.toml` & `enum_properties-1.4.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "enum-properties"
-version = "1.3.3"
-description = "Add properties to Python enumeration values with a simple declarative syntax."
+version = "1.4.0"
+description = "Add properties and method specializations to Python enumeration values with a simple declarative syntax."
 authors = ["Brian Kohan <bckohan@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/bckohan/enum-properties"
 homepage = "https://enum-properties.readthedocs.io"
 readme = "README.rst"
 keywords = ["enum",  "properties", "defines", "field"]
 classifiers = [
@@ -33,26 +33,26 @@
 [tool.poetry.dependencies]
 python = ">=3.7,<4.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.0"
 Sphinx = "^5.0.2"
 sphinx-rtd-theme = "^1.0.0"
-mypy = "^0.982"
+mypy = ">=0.982,<1.3"
 isort = "^5.6.4"
 doc8 = "^0.11.0"
 darglint = "^1.5.7"
 pytest-cov = "^4.0.0"
 pylint = "^2.12.0"
 sphinx-argparse = "^0.3.0"
-deepdiff = "^5.2.3"
+deepdiff = ">=5.2.3,<7.0.0"
 safety = "^2.0.0"
 readme-renderer = "^37.1"
 pygount = "^1.2.4"
-coverage = "^6.2"
+coverage = ">=6.2,<8.0"
 importlib-metadata = [
     { version = "<5.0", markers = "python_version <= '3.7'" },
     { version = ">=5.0", markers = "python_version > '3.7'" },
 ]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `enum_properties-1.3.3/setup.py` & `enum_properties-1.4.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 ['enum_properties']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'enum-properties',
-    'version': '1.3.3',
-    'description': 'Add properties to Python enumeration values with a simple declarative syntax.',
-    'long_description': "|MIT license| |PyPI version fury.io| |PyPI pyversions| |PyPI status| |Documentation Status|\n|Code Cov| |Test Status|\n\n.. |MIT license| image:: https://img.shields.io/badge/License-MIT-blue.svg\n   :target: https://lbesson.mit-license.org/\n\n.. |PyPI version fury.io| image:: https://badge.fury.io/py/enum-properties.svg\n   :target: https://pypi.python.org/pypi/enum-properties/\n\n.. |PyPI pyversions| image:: https://img.shields.io/pypi/pyversions/enum-properties.svg\n   :target: https://pypi.python.org/pypi/enum-properties/\n\n.. |PyPI status| image:: https://img.shields.io/pypi/status/enum-properties.svg\n   :target: https://pypi.python.org/pypi/enum-properties\n\n.. |Documentation Status| image:: https://readthedocs.org/projects/enum-properties/badge/?version=latest\n   :target: http://enum-properties.readthedocs.io/?badge=latest/\n\n.. |Code Cov| image:: https://codecov.io/gh/bckohan/enum-properties/branch/main/graph/badge.svg?token=0IZOKN2DYL\n   :target: https://codecov.io/gh/bckohan/enum-properties\n\n.. |Test Status| image:: https://github.com/bckohan/enum-properties/workflows/test/badge.svg\n   :target: https://github.com/bckohan/enum-properties/actions\n\nEnum Properties\n#######################\n\nAdd properties to Python enumeration values with a simple declarative syntax.\n`Enum Properties <https://enum-properties.readthedocs.io/en/latest/>`_ is a\nlightweight extension to\n`Python's Enum class <https://docs.python.org/3/library/enum.html>`_. Example:\n\n.. code:: python\n\n    from enum_properties import EnumProperties, p\n    from enum import auto\n\n    class Color(EnumProperties, p('rgb'), p('hex')):\n\n        # name   value      rgb       hex\n        RED    = auto(), (1, 0, 0), 'ff0000'\n        GREEN  = auto(), (0, 1, 0), '00ff00'\n        BLUE   = auto(), (0, 0, 1), '0000ff'\n\n    # the named p() values in the Enum's inheritance become properties on\n    # each value, matching the order in which they are specified\n\n    Color.RED.rgb   == (1, 0, 0)\n    Color.GREEN.rgb == (0, 1, 0)\n    Color.BLUE.rgb  == (0, 0, 1)\n\n    Color.RED.hex   == 'ff0000'\n    Color.GREEN.hex == '00ff00'\n    Color.BLUE.hex  == '0000ff'\n\nProperties may also be symmetrically mapped to enumeration values, using\ns() values:\n\n.. code:: python\n\n    from enum_properties import EnumProperties, s\n    from enum import auto\n\n    class Color(EnumProperties, s('rgb'), s('hex', case_fold=True)):\n\n        RED    = auto(), (1, 0, 0), 'ff0000'\n        GREEN  = auto(), (0, 1, 0), '00ff00'\n        BLUE   = auto(), (0, 0, 1), '0000ff'\n\n    # any named s() values in the Enum's inheritance become properties on\n    # each value, and the enumeration value may be instantiated from the\n    # property's value\n\n    Color((1, 0, 0)) == Color.RED\n    Color((0, 1, 0)) == Color.GREEN\n    Color((0, 0, 1)) == Color.BLUE\n\n    Color('ff0000') == Color.RED\n    Color('FF0000') == Color.RED  # case_fold makes mapping case insensitive\n    Color('00ff00') == Color.GREEN\n    Color('00FF00') == Color.GREEN\n    Color('0000ff') == Color.BLUE\n    Color('0000FF') == Color.BLUE\n\n    Color.RED.hex == 'ff0000'\n\nPlease report bugs and discuss features on the\n`issues page <https://github.com/bckohan/enum-properties/issues>`_.\n\n`Contributions <https://github.com/bckohan/enum-properties/blob/main/CONTRIBUTING.rst>`_ are\nencouraged!\n\n`Full documentation at read the docs. <https://enum-properties.readthedocs.io/en/latest/>`_\n\nInstallation\n------------\n\n1. Clone enum-properties from GitHub_ or install a release off PyPI_ :\n\n.. code:: bash\n\n       pip install enum-properties\n\n\n.. _GitHub: http://github.com/bckohan/enum-properties\n.. _PyPI: http://pypi.python.org/pypi/enum-properties\n",
+    'version': '1.4.0',
+    'description': 'Add properties and method specializations to Python enumeration values with a simple declarative syntax.',
+    'long_description': "|MIT license| |PyPI version fury.io| |PyPI pyversions| |PyPI status| |Documentation Status|\n|Code Cov| |Test Status|\n\n.. |MIT license| image:: https://img.shields.io/badge/License-MIT-blue.svg\n   :target: https://lbesson.mit-license.org/\n\n.. |PyPI version fury.io| image:: https://badge.fury.io/py/enum-properties.svg\n   :target: https://pypi.python.org/pypi/enum-properties/\n\n.. |PyPI pyversions| image:: https://img.shields.io/pypi/pyversions/enum-properties.svg\n   :target: https://pypi.python.org/pypi/enum-properties/\n\n.. |PyPI status| image:: https://img.shields.io/pypi/status/enum-properties.svg\n   :target: https://pypi.python.org/pypi/enum-properties\n\n.. |Documentation Status| image:: https://readthedocs.org/projects/enum-properties/badge/?version=latest\n   :target: http://enum-properties.readthedocs.io/?badge=latest/\n\n.. |Code Cov| image:: https://codecov.io/gh/bckohan/enum-properties/branch/main/graph/badge.svg?token=0IZOKN2DYL\n   :target: https://codecov.io/gh/bckohan/enum-properties\n\n.. |Test Status| image:: https://github.com/bckohan/enum-properties/workflows/test/badge.svg\n   :target: https://github.com/bckohan/enum-properties/actions\n\nEnum Properties\n#######################\n\nAdd properties to Python enumeration values with a simple declarative syntax.\n`Enum Properties <https://enum-properties.readthedocs.io/en/latest/>`_ is a\nlightweight extension to\n`Python's Enum class <https://docs.python.org/3/library/enum.html>`_. Example:\n\n.. code:: python\n\n    from enum_properties import EnumProperties, p\n    from enum import auto\n\n    class Color(EnumProperties, p('rgb'), p('hex')):\n\n        # name   value      rgb       hex\n        RED    = auto(), (1, 0, 0), 'ff0000'\n        GREEN  = auto(), (0, 1, 0), '00ff00'\n        BLUE   = auto(), (0, 0, 1), '0000ff'\n\n    # the named p() values in the Enum's inheritance become properties on\n    # each value, matching the order in which they are specified\n\n    Color.RED.rgb   == (1, 0, 0)\n    Color.GREEN.rgb == (0, 1, 0)\n    Color.BLUE.rgb  == (0, 0, 1)\n\n    Color.RED.hex   == 'ff0000'\n    Color.GREEN.hex == '00ff00'\n    Color.BLUE.hex  == '0000ff'\n\nProperties may also be symmetrically mapped to enumeration values, using\ns() values:\n\n.. code:: python\n\n    from enum_properties import EnumProperties, s\n    from enum import auto\n\n    class Color(EnumProperties, s('rgb'), s('hex', case_fold=True)):\n\n        RED    = auto(), (1, 0, 0), 'ff0000'\n        GREEN  = auto(), (0, 1, 0), '00ff00'\n        BLUE   = auto(), (0, 0, 1), '0000ff'\n\n    # any named s() values in the Enum's inheritance become properties on\n    # each value, and the enumeration value may be instantiated from the\n    # property's value\n\n    Color((1, 0, 0)) == Color.RED\n    Color((0, 1, 0)) == Color.GREEN\n    Color((0, 0, 1)) == Color.BLUE\n\n    Color('ff0000') == Color.RED\n    Color('FF0000') == Color.RED  # case_fold makes mapping case insensitive\n    Color('00ff00') == Color.GREEN\n    Color('00FF00') == Color.GREEN\n    Color('0000ff') == Color.BLUE\n    Color('0000FF') == Color.BLUE\n\n    Color.RED.hex == 'ff0000'\n\n\nMember functions may also be specialized to each enumeration value, using the\n@specialize decorator.\n\n.. code:: python\n\n    from enum_properties import EnumProperties, specialize\n\n    class SpecializedEnum(EnumProperties):\n\n        ONE   = 1\n        TWO   = 2\n        THREE = 3\n\n        @specialize(ONE)\n        def method(self):\n            return 'method_one()'\n\n        @specialize(TWO)\n        def method(self):\n            return 'method_two()'\n\n        @specialize(THREE)\n        def method(self):\n            return 'method_three()'\n\n    SpecializedEnum.ONE.method() == 'method_one()'\n    SpecializedEnum.TWO.method() == 'method_two()'\n    SpecializedEnum.THREE.method() == 'method_three()'\n\nPlease report bugs and discuss features on the\n`issues page <https://github.com/bckohan/enum-properties/issues>`_.\n\n`Contributions <https://github.com/bckohan/enum-properties/blob/main/CONTRIBUTING.rst>`_ are\nencouraged!\n\n`Full documentation at read the docs. <https://enum-properties.readthedocs.io/en/latest/>`_\n\nInstallation\n------------\n\n1. Clone enum-properties from GitHub_ or install a release off PyPI_ :\n\n.. code:: bash\n\n       pip install enum-properties\n\n\n.. _GitHub: http://github.com/bckohan/enum-properties\n.. _PyPI: http://pypi.python.org/pypi/enum-properties\n",
     'author': 'Brian Kohan',
     'author_email': 'bckohan@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://enum-properties.readthedocs.io',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `enum_properties-1.3.3/PKG-INFO` & `enum_properties-1.4.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: enum-properties
-Version: 1.3.3
-Summary: Add properties to Python enumeration values with a simple declarative syntax.
+Version: 1.4.0
+Summary: Add properties and method specializations to Python enumeration values with a simple declarative syntax.
 Home-page: https://enum-properties.readthedocs.io
 License: MIT
 Keywords: enum,properties,defines,field
 Author: Brian Kohan
 Author-email: bckohan@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -113,14 +113,44 @@
     Color('00ff00') == Color.GREEN
     Color('00FF00') == Color.GREEN
     Color('0000ff') == Color.BLUE
     Color('0000FF') == Color.BLUE
 
     Color.RED.hex == 'ff0000'
 
+
+Member functions may also be specialized to each enumeration value, using the
+@specialize decorator.
+
+.. code:: python
+
+    from enum_properties import EnumProperties, specialize
+
+    class SpecializedEnum(EnumProperties):
+
+        ONE   = 1
+        TWO   = 2
+        THREE = 3
+
+        @specialize(ONE)
+        def method(self):
+            return 'method_one()'
+
+        @specialize(TWO)
+        def method(self):
+            return 'method_two()'
+
+        @specialize(THREE)
+        def method(self):
+            return 'method_three()'
+
+    SpecializedEnum.ONE.method() == 'method_one()'
+    SpecializedEnum.TWO.method() == 'method_two()'
+    SpecializedEnum.THREE.method() == 'method_three()'
+
 Please report bugs and discuss features on the
 `issues page <https://github.com/bckohan/enum-properties/issues>`_.
 
 `Contributions <https://github.com/bckohan/enum-properties/blob/main/CONTRIBUTING.rst>`_ are
 encouraged!
 
 `Full documentation at read the docs. <https://enum-properties.readthedocs.io/en/latest/>`_
```

