# Comparing `tmp/gpx-0.2.0.tar.gz` & `tmp/gpx-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpx-0.2.0.tar", last modified: Thu Apr  6 12:09:16 2023, max compression
+gzip compressed data, was "gpx-0.2.1.tar", last modified: Sun Apr  9 20:15:06 2023, max compression
```

## Comparing `gpx-0.2.0.tar` & `gpx-0.2.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0      376 2023-04-06 12:09:03.581236 gpx-0.2.0/.editorconfig
--rw-r--r--   0        0        0       66 2023-04-06 12:09:03.581236 gpx-0.2.0/.gitattributes
--rw-r--r--   0        0        0      731 2023-04-06 12:09:03.581236 gpx-0.2.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0     3078 2023-04-06 12:09:03.581236 gpx-0.2.0/.gitignore
--rw-r--r--   0        0        0     1655 2023-04-06 12:09:03.581236 gpx-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      198 2023-04-06 12:09:03.581236 gpx-0.2.0/.readthedocs.yaml
--rw-r--r--   0        0        0       57 2023-04-06 12:09:03.581236 gpx-0.2.0/.vscode/extensions.json
--rw-r--r--   0        0        0    35884 2023-04-06 12:09:03.581236 gpx-0.2.0/LICENSE
--rw-r--r--   0        0        0     2117 2023-04-06 12:09:03.581236 gpx-0.2.0/README.md
--rw-r--r--   0        0        0      715 2023-04-06 12:09:03.581236 gpx-0.2.0/docs/Makefile
--rw-r--r--   0        0        0     1574 2023-04-06 12:09:03.581236 gpx-0.2.0/docs/api.md
--rw-r--r--   0        0        0     2573 2023-04-06 12:09:03.581236 gpx-0.2.0/docs/changelog.md
--rw-r--r--   0        0        0     1528 2023-04-06 12:09:03.585236 gpx-0.2.0/docs/conf.py
--rw-r--r--   0        0        0      322 2023-04-06 12:09:03.585236 gpx-0.2.0/docs/index.md
--rw-r--r--   0        0        0      153 2023-04-06 12:09:03.585236 gpx-0.2.0/docs/installation.md
--rw-r--r--   0        0        0      765 2023-04-06 12:09:03.585236 gpx-0.2.0/docs/make.bat
--rw-r--r--   0        0        0      132 2023-04-06 12:09:03.585236 gpx-0.2.0/docs/usage.md
--rw-r--r--   0        0        0     1561 2023-04-06 12:09:03.585236 gpx-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      673 2023-04-06 12:09:03.585236 gpx-0.2.0/src/gpx/__init__.py
--rw-r--r--   0        0        0     1773 2023-04-06 12:09:03.585236 gpx-0.2.0/src/gpx/bounds.py
--rw-r--r--   0        0        0     1839 2023-04-06 12:09:03.585236 gpx-0.2.0/src/gpx/copyright.py
--rw-r--r--   0        0        0     1571 2023-04-06 12:09:03.585236 gpx-0.2.0/src/gpx/element.py
--rw-r--r--   0        0        0     1059 2023-04-06 12:09:03.585236 gpx-0.2.0/src/gpx/email.py
--rw-r--r--   0        0        0      172 2023-04-06 12:09:03.585236 gpx-0.2.0/src/gpx/errors.py
--rw-r--r--   0        0        0     8997 2023-04-06 12:09:03.585236 gpx-0.2.0/src/gpx/gpx.py
--rw-r--r--   0        0        0    25872 2023-04-06 12:09:03.585236 gpx-0.2.0/src/gpx/gpx.xsd
--rw-r--r--   0        0        0     1577 2023-04-06 12:09:03.585236 gpx-0.2.0/src/gpx/link.py
--rw-r--r--   0        0        0     4140 2023-04-06 12:09:03.585236 gpx-0.2.0/src/gpx/metadata.py
--rw-r--r--   0        0        0     2909 2023-04-06 12:09:03.585236 gpx-0.2.0/src/gpx/mixins.py
--rw-r--r--   0        0        0     1716 2023-04-06 12:09:03.585236 gpx-0.2.0/src/gpx/person.py
--rw-r--r--   0        0        0        0 2023-04-06 12:09:03.585236 gpx-0.2.0/src/gpx/py.typed
--rw-r--r--   0        0        0     4098 2023-04-06 12:09:03.585236 gpx-0.2.0/src/gpx/route.py
--rw-r--r--   0        0        0     5061 2023-04-06 12:09:03.585236 gpx-0.2.0/src/gpx/track.py
--rw-r--r--   0        0        0     2471 2023-04-06 12:09:03.585236 gpx-0.2.0/src/gpx/track_segment.py
--rw-r--r--   0        0        0     3419 2023-04-06 12:09:03.585236 gpx-0.2.0/src/gpx/types.py
--rw-r--r--   0        0        0      379 2023-04-06 12:09:03.585236 gpx-0.2.0/src/gpx/utils.py
--rw-r--r--   0        0        0    10652 2023-04-06 12:09:03.585236 gpx-0.2.0/src/gpx/waypoint.py
--rw-r--r--   0        0        0     3733 1970-01-01 00:00:00.000000 gpx-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      376 2023-04-09 20:14:57.353153 gpx-0.2.1/.editorconfig
+-rw-r--r--   0        0        0       66 2023-04-09 20:14:57.353153 gpx-0.2.1/.gitattributes
+-rw-r--r--   0        0        0      731 2023-04-09 20:14:57.353153 gpx-0.2.1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     3078 2023-04-09 20:14:57.353153 gpx-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1655 2023-04-09 20:14:57.353153 gpx-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      198 2023-04-09 20:14:57.353153 gpx-0.2.1/.readthedocs.yaml
+-rw-r--r--   0        0        0       57 2023-04-09 20:14:57.353153 gpx-0.2.1/.vscode/extensions.json
+-rw-r--r--   0        0        0    35884 2023-04-09 20:14:57.353153 gpx-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2117 2023-04-09 20:14:57.353153 gpx-0.2.1/README.md
+-rw-r--r--   0        0        0      715 2023-04-09 20:14:57.353153 gpx-0.2.1/docs/Makefile
+-rw-r--r--   0        0        0     1574 2023-04-09 20:14:57.353153 gpx-0.2.1/docs/api.md
+-rw-r--r--   0        0        0     2690 2023-04-09 20:14:57.353153 gpx-0.2.1/docs/changelog.md
+-rw-r--r--   0        0        0     1528 2023-04-09 20:14:57.353153 gpx-0.2.1/docs/conf.py
+-rw-r--r--   0        0        0      322 2023-04-09 20:14:57.353153 gpx-0.2.1/docs/index.md
+-rw-r--r--   0        0        0      153 2023-04-09 20:14:57.353153 gpx-0.2.1/docs/installation.md
+-rw-r--r--   0        0        0      765 2023-04-09 20:14:57.353153 gpx-0.2.1/docs/make.bat
+-rw-r--r--   0        0        0      132 2023-04-09 20:14:57.353153 gpx-0.2.1/docs/usage.md
+-rw-r--r--   0        0        0     1561 2023-04-09 20:14:57.353153 gpx-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      673 2023-04-09 20:14:57.353153 gpx-0.2.1/src/gpx/__init__.py
+-rw-r--r--   0        0        0     1996 2023-04-09 20:14:57.353153 gpx-0.2.1/src/gpx/bounds.py
+-rw-r--r--   0        0        0     2049 2023-04-09 20:14:57.353153 gpx-0.2.1/src/gpx/copyright.py
+-rw-r--r--   0        0        0     1506 2023-04-09 20:14:57.357153 gpx-0.2.1/src/gpx/element.py
+-rw-r--r--   0        0        0     1256 2023-04-09 20:14:57.357153 gpx-0.2.1/src/gpx/email.py
+-rw-r--r--   0        0        0      172 2023-04-09 20:14:57.357153 gpx-0.2.1/src/gpx/errors.py
+-rw-r--r--   0        0        0     9237 2023-04-09 20:14:57.357153 gpx-0.2.1/src/gpx/gpx.py
+-rw-r--r--   0        0        0    25872 2023-04-09 20:14:57.357153 gpx-0.2.1/src/gpx/gpx.xsd
+-rw-r--r--   0        0        0     1787 2023-04-09 20:14:57.357153 gpx-0.2.1/src/gpx/link.py
+-rw-r--r--   0        0        0     4423 2023-04-09 20:14:57.357153 gpx-0.2.1/src/gpx/metadata.py
+-rw-r--r--   0        0        0     2909 2023-04-09 20:14:57.357153 gpx-0.2.1/src/gpx/mixins.py
+-rw-r--r--   0        0        0     1926 2023-04-09 20:14:57.357153 gpx-0.2.1/src/gpx/person.py
+-rw-r--r--   0        0        0        0 2023-04-09 20:14:57.357153 gpx-0.2.1/src/gpx/py.typed
+-rw-r--r--   0        0        0     4396 2023-04-09 20:14:57.357153 gpx-0.2.1/src/gpx/route.py
+-rw-r--r--   0        0        0     5371 2023-04-09 20:14:57.357153 gpx-0.2.1/src/gpx/track.py
+-rw-r--r--   0        0        0     2673 2023-04-09 20:14:57.357153 gpx-0.2.1/src/gpx/track_segment.py
+-rw-r--r--   0        0        0     3419 2023-04-09 20:14:57.357153 gpx-0.2.1/src/gpx/types.py
+-rw-r--r--   0        0        0      379 2023-04-09 20:14:57.357153 gpx-0.2.1/src/gpx/utils.py
+-rw-r--r--   0        0        0    11127 2023-04-09 20:14:57.357153 gpx-0.2.1/src/gpx/waypoint.py
+-rw-r--r--   0        0        0     3733 1970-01-01 00:00:00.000000 gpx-0.2.1/PKG-INFO
```

### Comparing `gpx-0.2.0/.github/workflows/publish.yml` & `gpx-0.2.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `gpx-0.2.0/.gitignore` & `gpx-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `gpx-0.2.0/.pre-commit-config.yaml` & `gpx-0.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `gpx-0.2.0/LICENSE` & `gpx-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gpx-0.2.0/README.md` & `gpx-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `gpx-0.2.0/docs/Makefile` & `gpx-0.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gpx-0.2.0/docs/api.md` & `gpx-0.2.1/docs/api.md`

 * *Files identical despite different names*

### Comparing `gpx-0.2.0/docs/changelog.md` & `gpx-0.2.1/docs/changelog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # Changelog
 
+## 0.2.1 (2023-04-09)
+
+### Fixed
+
+-   Serialization of route and track numbers. #10
+-   Mutable default values. #11
+
 ## 0.2.0 (2023-04-06)
 
 With this release, PyGPX is now fully [^spec-compat] compatible with the [GPX 1.1 specification](https://www.topografix.com/GPX/1/1/gpx.xsd).
 
 ### Changes
 
 -   Added the following new modules and classes:
```

### Comparing `gpx-0.2.0/docs/conf.py` & `gpx-0.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `gpx-0.2.0/docs/make.bat` & `gpx-0.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `gpx-0.2.0/pyproject.toml` & `gpx-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gpx-0.2.0/src/gpx/__init__.py` & `gpx-0.2.1/src/gpx/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,8 +19,8 @@
 from .person import Person
 from .route import Route
 from .track import Track
 from .track_segment import TrackSegment
 from .types import Degrees, DGPSStation, Fix, Latitude, Longitude
 from .waypoint import Waypoint
 
-__version__ = "0.2.0"
+__version__ = "0.2.1"
```

### Comparing `gpx-0.2.0/src/gpx/bounds.py` & `gpx-0.2.1/src/gpx/bounds.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,25 +15,31 @@
 
     Two lat/lon pairs defining the extent of an element.
 
     Args:
         element: The bounds XML element. Defaults to `None`.
     """
 
-    #: The minimum latitude.
-    minlat: Latitude
+    def __init__(self, element: etree._Element | None = None) -> None:
+        super().__init__(element)
 
-    #: The minimum longitude.
-    minlon: Longitude
+        #: The minimum latitude.
+        self.minlat: Latitude
 
-    #: The maximum latitude.
-    maxlat: Latitude
+        #: The minimum longitude.
+        self.minlon: Longitude
 
-    #: The maximum longitude.
-    maxlon: Longitude
+        #: The maximum latitude.
+        self.maxlat: Latitude
+
+        #: The maximum longitude.
+        self.maxlon: Longitude
+
+        if self._element is not None:
+            self._parse()
 
     def as_tuple(self) -> tuple[Latitude, Longitude, Latitude, Longitude]:
         """Return the bounds as a tuple."""
         return (self.minlat, self.minlon, self.maxlat, self.maxlon)
 
     def __getitem__(self, index: int) -> Latitude | Longitude:
         return self.as_tuple()[index]
```

### Comparing `gpx-0.2.0/src/gpx/copyright.py` & `gpx-0.2.1/src/gpx/copyright.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,22 +17,28 @@
     file. By linking to an appropriate license, you may place your data into the
     public domain or grant additional usage rights.
 
     Args:
         element: The copyright XML element. Defaults to `None`.
     """
 
-    #: Copyright holder (e.g. TopoSoft, Inc.).
-    author: str
+    def __init__(self, element: etree._Element | None = None) -> None:
+        super().__init__(element)
 
-    #: Year of copyright.
-    year: int | None = None
+        #: Copyright holder (e.g. TopoSoft, Inc.).
+        self.author: str
 
-    #: Link to external file containing license text.
-    license: str | None = None
+        #: Year of copyright.
+        self.year: int | None = None
+
+        #: Link to external file containing license text.
+        self.license: str | None = None
+
+        if self._element is not None:
+            self._parse()
 
     def _parse(self) -> None:
         super()._parse()
 
         # assertion to satisfy mypy
         assert self._element is not None
```

### Comparing `gpx-0.2.0/src/gpx/element.py` & `gpx-0.2.1/src/gpx/element.py`

 * *Files 17% similar despite different names*

```diff
@@ -19,17 +19,14 @@
     def __init__(self, element: etree._Element | None = None) -> None:
         #: The XML element.
         self._element: etree._Element | None = element
 
         #: The XML namespace mapping from prefix -> URI.
         self._nsmap: dict[str, str] | None = None
 
-        if self._element is not None:
-            self._parse()
-
     def _parse(self) -> None:
         """Parses the XML element.
 
         Raises:
             ParseError: If the XML element is `None`.
         """
         # check if element exists before attempting to parse
```

### Comparing `gpx-0.2.0/src/gpx/email.py` & `gpx-0.2.1/src/gpx/email.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,19 +12,25 @@
     An email address. Broken into two parts (id and domain) to help prevent
     email harvesting.
 
     Args:
         element: The email XML element. Defaults to `None`.
     """
 
-    #: id half of email address (e.g. billgates2004)
-    id: str
+    def __init__(self, element: etree._Element | None = None) -> None:
+        super().__init__(element)
 
-    #: domain half of email address (e.g. hotmail.com)
-    domain: str
+        #: id half of email address (e.g. billgates2004)
+        self.id: str
+
+        #: domain half of email address (e.g. hotmail.com)
+        self.domain: str
+
+        if self._element is not None:
+            self._parse()
 
     def _parse(self) -> None:
         super()._parse()
 
         # assertion to satisfy mypy
         assert self._element is not None
```

### Comparing `gpx-0.2.0/src/gpx/gpx.py` & `gpx-0.2.1/src/gpx/gpx.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,29 +30,35 @@
     tracks. You can add your own elements to the extensions section of the GPX
     document.
 
     Args:
         element: The GPX XML element. Defaults to `None`.
     """
 
-    #: The name or URL of the software that created your GPX document. Defaults
-    #: to "PyGPX".
-    creator: str = "PyGPX"
+    def __init__(self, element: etree._Element | None = None) -> None:
+        super().__init__(element)
 
-    #: Metadata about the file.
-    metadata: Metadata | None = None
+        #: The name or URL of the software that created your GPX document.
+        #: Defaults to "PyGPX".
+        self.creator: str = "PyGPX"
 
-    #: A list of waypoints.
-    waypoints: list[Waypoint] = []
+        #: Metadata about the file.
+        self.metadata: Metadata | None = None
 
-    #: A list of routes.
-    routes: list[Route] = []
+        #: A list of waypoints.
+        self.waypoints: list[Waypoint] = []
 
-    #: A list of tracks.
-    tracks: list[Track] = []
+        #: A list of routes.
+        self.routes: list[Route] = []
+
+        #: A list of tracks.
+        self.tracks: list[Track] = []
+
+        if self._element is not None:
+            self._parse()
 
     @property
     def name(self) -> str | None:
         """The name of the GPX file.
 
         Alias of :attr:`gpx.metadata.Metadata.name`.
         """
```

### Comparing `gpx-0.2.0/src/gpx/gpx.xsd` & `gpx-0.2.1/src/gpx/gpx.xsd`

 * *Files identical despite different names*

### Comparing `gpx-0.2.0/src/gpx/link.py` & `gpx-0.2.1/src/gpx/link.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,22 +15,28 @@
     A link to an external resource (Web page, digital photo, video clip, etc)
     with additional information.
 
     Args:
         element: The link XML element. Defaults to `None`.
     """
 
-    #: URL of hyperlink.
-    href: str
+    def __init__(self, element: etree._Element | None = None) -> None:
+        super().__init__(element)
 
-    #: Text of hyperlink.
-    text: str | None = None
+        #: URL of hyperlink.
+        self.href: str
 
-    #: Mime type of content (e.g. image/jpeg)
-    type: str | None = None
+        #: Text of hyperlink.
+        self.text: str | None = None
+
+        #: Mime type of content (e.g. image/jpeg)
+        self.type: str | None = None
+
+        if self._element is not None:
+            self._parse()
 
     def _parse(self) -> None:
         super()._parse()
 
         # assertion to satisfy mypy
         assert self._element is not None
```

### Comparing `gpx-0.2.0/src/gpx/metadata.py` & `gpx-0.2.1/src/gpx/metadata.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,39 +23,45 @@
     the metadata section. Providing rich, meaningful information about your GPX
     files allows others to search for and use your GPS data.
 
     Args:
         element: The metadata XML element. Defaults to `None`.
     """
 
-    #: The name of the GPX file.
-    name: str | None = None
+    def __init__(self, element: etree._Element | None = None) -> None:
+        super().__init__(element)
 
-    #: A description of the contents of the GPX file.
-    desc: str | None = None
+        #: The name of the GPX file.
+        self.name: str | None = None
 
-    #: The person or organization who created the GPX file.
-    author: Person | None = None
+        #: A description of the contents of the GPX file.
+        self.desc: str | None = None
 
-    #: Copyright and license information governing use of the file.
-    copyright: Copyright | None = None
+        #: The person or organization who created the GPX file.
+        self.author: Person | None = None
 
-    #: URLs associated with the location described in the file.
-    links: list[Link] = []
+        #: Copyright and license information governing use of the file.
+        self.copyright: Copyright | None = None
 
-    #: The creation date of the file.
-    time: datetime.datetime | None = None
+        #: URLs associated with the location described in the file.
+        self.links: list[Link] = []
 
-    #: Keywords associated with the file. Search engines or databases can use
-    #: this information to classify the data.
-    keywords: str | None = None
+        #: The creation date of the file.
+        self.time: datetime.datetime | None = None
 
-    #: Minimum and maximum coordinates which describe the extent of the
-    #: coordinates in the file.
-    bounds: Bounds | None = None
+        #: Keywords associated with the file. Search engines or databases can
+        #: use this information to classify the data.
+        self.keywords: str | None = None
+
+        #: Minimum and maximum coordinates which describe the extent of the
+        #: coordinates in the file.
+        self.bounds: Bounds | None = None
+
+        if self._element is not None:
+            self._parse()
 
     def _parse(self) -> None:
         super()._parse()
 
         # assertion to satisfy mypy
         assert self._element is not None
```

### Comparing `gpx-0.2.0/src/gpx/mixins.py` & `gpx-0.2.1/src/gpx/mixins.py`

 * *Files identical despite different names*

### Comparing `gpx-0.2.0/src/gpx/person.py` & `gpx-0.2.1/src/gpx/person.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,24 +14,30 @@
 
     A person or organization.
 
     Args:
         element: The person XML element. Defaults to `None`.
     """
 
-    #: Name of person or organization.
-    name: str | None = None
+    __keys__ = ("name", "email", "link")
 
-    #: Email address.
-    email: Email | None = None
+    def __init__(self, element: etree._Element | None = None) -> None:
+        super().__init__(element)
 
-    #: Link to Web site or other external information about person.
-    link: Link | None = None
+        #: Name of person or organization.
+        self.name: str | None = None
 
-    __keys__ = ("name", "email", "link")
+        #: Email address.
+        self.email: Email | None = None
+
+        #: Link to Web site or other external information about person.
+        self.link: Link | None = None
+
+        if self._element is not None:
+            self._parse()
 
     def _parse(self) -> None:
         super()._parse()
 
         # assertion to satisfy mypy
         assert self._element is not None
```

### Comparing `gpx-0.2.0/src/gpx/route.py` & `gpx-0.2.1/src/gpx/route.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,39 +19,45 @@
     A route represents an ordered list of waypoints representing a series of
     turn points leading to a destination.
 
     Args:
         element: The route XML element. Defaults to `None`.
     """
 
-    #: GPS name of route.
-    name: str | None = None
+    def __init__(self, element: etree._Element | None = None) -> None:
+        super().__init__(element)
 
-    #: GPS comment for route.
-    cmt: str | None = None
+        #: GPS name of route.
+        self.name: str | None = None
 
-    #: Text description of route for user. Not sent to GPS.
-    desc: str | None = None
+        #: GPS comment for route.
+        self.cmt: str | None = None
 
-    #: Source of data. Included to give user some idea of reliability and
-    #: accuracy of data.
-    src: str | None = None
+        #: Text description of route for user. Not sent to GPS.
+        self.desc: str | None = None
 
-    #: Links to external information about the route.
-    links: list[Link] = []
+        #: Source of data. Included to give user some idea of reliability and
+        #: accuracy of data.
+        self.src: str | None = None
 
-    #: GPS route number.
-    number: int | None = None
+        #: Links to external information about the route.
+        self.links: list[Link] = []
 
-    #: Type (classification) of route.
-    type: str | None = None
+        #: GPS route number.
+        self.number: int | None = None
 
-    #: A list of route points.
-    rtepts: list[Waypoint] = []
-    points = rtepts  #: Alias of :attr:`rtepts`.
+        #: Type (classification) of route.
+        self.type: str | None = None
+
+        #: A list of route points.
+        self.rtepts: list[Waypoint] = []
+        self.points = self.rtepts  #: Alias of :attr:`rtepts`.
+
+        if self._element is not None:
+            self._parse()
 
     def _parse(self) -> None:
         super()._parse()
 
         # assertion to satisfy mypy
         assert self._element is not None
 
@@ -101,15 +107,15 @@
             src.text = self.src
 
         for link in self.links:
             route.append(link._build())
 
         if self.number is not None:
             number = etree.SubElement(route, "number", nsmap=self._nsmap)
-            number.text = self.number
+            number.text = str(self.number)
 
         if self.type is not None:
             _type = etree.SubElement(route, "type", nsmap=self._nsmap)
             _type.text = self.type
 
         for _rtept in self.rtepts:
             route.append(_rtept._build(tag="rtept"))
```

### Comparing `gpx-0.2.0/src/gpx/track.py` & `gpx-0.2.1/src/gpx/track.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,42 +20,48 @@
 
     A track represents an ordered list of points describing a path.
 
     Args:
         element: The track XML element. Defaults to `None`.
     """
 
-    #: GPS name of track.
-    name: str | None = None
+    def __init__(self, element: etree._Element | None = None) -> None:
+        super().__init__(element)
 
-    #: GPS comment for track.
-    cmt: str | None = None
+        #: GPS name of track.
+        self.name: str | None = None
 
-    #: User description of track.
-    desc: str | None = None
+        #: GPS comment for track.
+        self.cmt: str | None = None
 
-    #: Source of data. Included to give user some idea of reliability and
-    #: accuracy of data.
-    src: str | None = None
-
-    #: Links to external information about track.
-    links: list[Link] = []
-
-    #: GPS track number.
-    number: int | None = None
-
-    #: Type (classification) of track.
-    type: str | None = None
-
-    #: A Track Segment holds a list of Track Points which are logically
-    #: connected in order. To represent a single GPS track where GPS
-    #: reception was lost, or the GPS receiver was turned off, start a new
-    #: Track Segment for each continuous span of track data.
-    trksegs: list[TrackSegment] = []
-    segments = trksegs  #: Alias of :attr:`trksegs`.
+        #: User description of track.
+        self.desc: str | None = None
+
+        #: Source of data. Included to give user some idea of reliability and
+        #: accuracy of data.
+        self.src: str | None = None
+
+        #: Links to external information about track.
+        self.links: list[Link] = []
+
+        #: GPS track number.
+        self.number: int | None = None
+
+        #: Type (classification) of track.
+        self.type: str | None = None
+
+        #: A Track Segment holds a list of Track Points which are logically
+        #: connected in order. To represent a single GPS track where GPS
+        #: reception was lost, or the GPS receiver was turned off, start a new
+        #: Track Segment for each continuous span of track data.
+        self.trksegs: list[TrackSegment] = []
+        self.segments = self.trksegs  #: Alias of :attr:`trksegs`.
+
+        if self._element is not None:
+            self._parse()
 
     def __getitem__(self, index: int) -> TrackSegment:
         """Returns the track segment at the given index."""
         return self.trksegs[index]
 
     def __len__(self) -> int:
         """Returns the number of track segments."""
@@ -117,15 +123,15 @@
             src.text = self.src
 
         for link in self.links:
             track.append(link._build())
 
         if self.number is not None:
             number = etree.SubElement(track, "number", nsmap=self._nsmap)
-            number.text = self.number
+            number.text = str(self.number)
 
         if self.type is not None:
             _type = etree.SubElement(track, "type", nsmap=self._nsmap)
             _type.text = self.type
 
         for segment in self.trksegs:
             track.append(segment._build())
```

### Comparing `gpx-0.2.0/src/gpx/track_segment.py` & `gpx-0.2.1/src/gpx/track_segment.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,18 +22,24 @@
     the GPS receiver was turned off, start a new Track Segment for each
     continuous span of track data.
 
     Args:
         element: The track segment XML element. Defaults to `None`.
     """
 
-    #: A Track Point holds the coordinates, elevation, timestamp, and
-    #: metadata for a single point in a track.
-    trkpts: list[Waypoint] = []
-    points = trkpts  #: Alias of :attr:`trkpts`.
+    def __init__(self, element: etree._Element | None = None) -> None:
+        super().__init__(element)
+
+        #: A Track Point holds the coordinates, elevation, timestamp, and
+        #: metadata for a single point in a track.
+        self.trkpts: list[Waypoint] = []
+        self.points = self.trkpts  #: Alias of :attr:`trkpts`.
+
+        if self._element is not None:
+            self._parse()
 
     def _parse(self) -> None:
         super()._parse()
 
         # assertion to satisfy mypy
         assert self._element is not None
```

### Comparing `gpx-0.2.0/src/gpx/types.py` & `gpx-0.2.1/src/gpx/types.py`

 * *Files identical despite different names*

### Comparing `gpx-0.2.0/src/gpx/waypoint.py` & `gpx-0.2.1/src/gpx/waypoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,84 +19,90 @@
     A waypoint represents a waypoint, point of interest, or named feature on a
     map.
 
     Args:
         element: The waypoint XML element. Defaults to `None`.
     """
 
-    #: The latitude of the point. Decimal degrees, WGS84 datum.
-    lat: Latitude
+    def __init__(self, element: etree._Element | None = None) -> None:
+        super().__init__(element)
 
-    #: The longitude of the point. Decimal degrees, WGS84 datum.
-    lon: Longitude
+        #: The latitude of the point. Decimal degrees, WGS84 datum.
+        self.lat: Latitude
 
-    #: Elevation (in meters) of the point.
-    ele: Decimal | None = None
+        #: The longitude of the point. Decimal degrees, WGS84 datum.
+        self.lon: Longitude
 
-    #: Creation/modification timestamp for element. Date and time in are in
-    #: Universal Coordinated Time (UTC), not local time! Conforms to ISO 8601
-    #: specification for date/time representation. Fractional seconds are
-    #: allowed for millisecond timing in tracklogs.
-    time: datetime | None = None
+        #: Elevation (in meters) of the point.
+        self.ele: Decimal | None = None
 
-    #: Magnetic variation (in degrees) at the point
-    magvar: Degrees | None = None
+        #: Creation/modification timestamp for element. Date and time in are in
+        #: Universal Coordinated Time (UTC), not local time! Conforms to ISO
+        #: 8601 specification for date/time representation. Fractional seconds
+        #: are allowed for millisecond timing in tracklogs.
+        self.time: datetime | None = None
 
-    #: Height (in meters) of geoid (mean sea level) above WGS84 earth
-    #: ellipsoid. As defined in NMEA GGA message.
-    geoidheight: Decimal | None = None
+        #: Magnetic variation (in degrees) at the point
+        self.magvar: Degrees | None = None
 
-    #: The GPS name of the waypoint. This field will be transferred to and
-    #: from the GPS. GPX does not place restrictions on the length of this
-    #: field or the characters contained in it. It is up to the receiving
-    #: application to validate the field before sending it to the GPS.
-    name: str | None = None
+        #: Height (in meters) of geoid (mean sea level) above WGS84 earth
+        #: ellipsoid. As defined in NMEA GGA message.
+        self.geoidheight: Decimal | None = None
 
-    #: GPS waypoint comment. Sent to GPS as comment.
-    cmt: str | None = None
+        #: The GPS name of the waypoint. This field will be transferred to and
+        #: from the GPS. GPX does not place restrictions on the length of this
+        #: field or the characters contained in it. It is up to the receiving
+        #: application to validate the field before sending it to the GPS.
+        self.name: str | None = None
 
-    #: A text description of the element. Holds additional information about
-    #: the element intended for the user, not the GPS.
-    desc: str | None = None
+        #: GPS waypoint comment. Sent to GPS as comment.
+        self.cmt: str | None = None
 
-    #: Source of data. Included to give user some idea of reliability and
-    #: accuracy of data. "Garmin eTrex", "USGS quad Boston North", e.g.
-    src: str | None = None
+        #: A text description of the element. Holds additional information about
+        #: the element intended for the user, not the GPS.
+        self.desc: str | None = None
 
-    #: Link to additional information about the waypoint.
-    links: list[Link] = []
+        #: Source of data. Included to give user some idea of reliability and
+        #: accuracy of data. "Garmin eTrex", "USGS quad Boston North", e.g.
+        self.src: str | None = None
 
-    #: Text of GPS symbol name. For interchange with other programs, use the
-    #: exact spelling of the symbol as displayed on the GPS. If the GPS
-    #: abbreviates words, spell them out.
-    sym: str | None = None
+        #: Link to additional information about the waypoint.
+        self.links: list[Link] = []
 
-    #: Type (classification) of the waypoint.
-    type: str | None = None
+        #: Text of GPS symbol name. For interchange with other programs, use the
+        #: exact spelling of the symbol as displayed on the GPS. If the GPS
+        #: abbreviates words, spell them out.
+        self.sym: str | None = None
 
-    #: Type of GPX fix.
-    fix: Fix | None = None
+        #: Type (classification) of the waypoint.
+        self.type: str | None = None
 
-    #: Number of satellites used to calculate the GPX fix.
-    sat: int | None = None
+        #: Type of GPX fix.
+        self.fix: Fix | None = None
 
-    #: Horizontal dilution of precision.
-    hdop: Decimal | None = None
+        #: Number of satellites used to calculate the GPX fix.
+        self.sat: int | None = None
 
-    #: Vertical dilution of precision.
-    vdop: Decimal | None = None
+        #: Horizontal dilution of precision.
+        self.hdop: Decimal | None = None
 
-    #: Position dilution of precision.
-    pdop: Decimal | None = None
+        #: Vertical dilution of precision.
+        self.vdop: Decimal | None = None
 
-    #: Number of seconds since last DGPS update.
-    ageofdgpsdata: Decimal | None = None
+        #: Position dilution of precision.
+        self.pdop: Decimal | None = None
 
-    #: ID of DGPS station used in differential correction.
-    dgpsid: DGPSStation | None = None
+        #: Number of seconds since last DGPS update.
+        self.ageofdgpsdata: Decimal | None = None
+
+        #: ID of DGPS station used in differential correction.
+        self.dgpsid: DGPSStation | None = None
+
+        if self._element is not None:
+            self._parse()
 
     def _parse(self) -> None:  # noqa: C901
         super()._parse()
 
         # assertion to satisfy mypy
         assert self._element is not None
```

### Comparing `gpx-0.2.0/PKG-INFO` & `gpx-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpx
-Version: 0.2.0
+Version: 0.2.1
 Summary: PyGPX is a Python package that brings support for reading, writing and
 Keywords: gpx,gps,xml
 Author-email: Steven van de Graaf <steven@vandegraaf.xyz>
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

