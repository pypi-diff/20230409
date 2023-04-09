# Comparing `tmp/webtypy-0.1.2.tar.gz` & `tmp/webtypy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webtypy-0.1.2.tar", last modified: Sun Apr  9 08:00:12 2023, max compression
+gzip compressed data, was "webtypy-0.1.3.tar", last modified: Sun Apr  9 10:02:37 2023, max compression
```

## Comparing `webtypy-0.1.2.tar` & `webtypy-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-09 08:00:12.756496 webtypy-0.1.2/
--rw-rw-r--   0 simone    (1000) simone    (1000)     1891 2023-04-09 08:00:12.756496 webtypy-0.1.2/PKG-INFO
--rw-rw-r--   0 simone    (1000) simone    (1000)     1445 2023-04-09 06:17:24.000000 webtypy-0.1.2/README.md
--rw-rw-r--   0 simone    (1000) simone    (1000)       90 2023-04-07 08:23:05.000000 webtypy-0.1.2/pyproject.toml
--rw-rw-r--   0 simone    (1000) simone    (1000)      780 2023-04-09 08:00:12.756496 webtypy-0.1.2/setup.cfg
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-09 08:00:12.752496 webtypy-0.1.2/src/
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-09 08:00:12.752496 webtypy-0.1.2/src/js/
--rw-rw-r--   0 simone    (1000) simone    (1000)        0 2023-04-09 07:53:45.000000 webtypy-0.1.2/src/js/__init__.py
--rw-rw-r--   0 simone    (1000) simone    (1000)   526414 2023-04-09 07:56:45.000000 webtypy-0.1.2/src/js/__init__.pyi
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-09 08:00:12.756496 webtypy-0.1.2/src/webtypy.egg-info/
--rw-rw-r--   0 simone    (1000) simone    (1000)     1891 2023-04-09 08:00:12.000000 webtypy-0.1.2/src/webtypy.egg-info/PKG-INFO
--rw-rw-r--   0 simone    (1000) simone    (1000)      281 2023-04-09 08:00:12.000000 webtypy-0.1.2/src/webtypy.egg-info/SOURCES.txt
--rw-rw-r--   0 simone    (1000) simone    (1000)        1 2023-04-09 08:00:12.000000 webtypy-0.1.2/src/webtypy.egg-info/dependency_links.txt
--rw-rw-r--   0 simone    (1000) simone    (1000)        1 2023-04-07 08:59:42.000000 webtypy-0.1.2/src/webtypy.egg-info/not-zip-safe
--rw-rw-r--   0 simone    (1000) simone    (1000)       53 2023-04-09 08:00:12.000000 webtypy-0.1.2/src/webtypy.egg-info/requires.txt
--rw-rw-r--   0 simone    (1000) simone    (1000)        3 2023-04-09 08:00:12.000000 webtypy-0.1.2/src/webtypy.egg-info/top_level.txt
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-09 10:02:37.804861 webtypy-0.1.3/
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1891 2023-04-09 10:02:37.804861 webtypy-0.1.3/PKG-INFO
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1445 2023-04-09 06:17:24.000000 webtypy-0.1.3/README.md
+-rw-rw-r--   0 simone    (1000) simone    (1000)       90 2023-04-07 08:23:05.000000 webtypy-0.1.3/pyproject.toml
+-rw-rw-r--   0 simone    (1000) simone    (1000)      780 2023-04-09 10:02:37.804861 webtypy-0.1.3/setup.cfg
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-09 10:02:37.800861 webtypy-0.1.3/src/
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-09 10:02:37.804861 webtypy-0.1.3/src/js/
+-rw-rw-r--   0 simone    (1000) simone    (1000)        0 2023-04-09 07:53:45.000000 webtypy-0.1.3/src/js/__init__.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)   537733 2023-04-09 10:01:43.000000 webtypy-0.1.3/src/js/__init__.pyi
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-09 10:02:37.804861 webtypy-0.1.3/src/webtypy.egg-info/
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1891 2023-04-09 10:02:37.000000 webtypy-0.1.3/src/webtypy.egg-info/PKG-INFO
+-rw-rw-r--   0 simone    (1000) simone    (1000)      281 2023-04-09 10:02:37.000000 webtypy-0.1.3/src/webtypy.egg-info/SOURCES.txt
+-rw-rw-r--   0 simone    (1000) simone    (1000)        1 2023-04-09 10:02:37.000000 webtypy-0.1.3/src/webtypy.egg-info/dependency_links.txt
+-rw-rw-r--   0 simone    (1000) simone    (1000)        1 2023-04-07 08:59:42.000000 webtypy-0.1.3/src/webtypy.egg-info/not-zip-safe
+-rw-rw-r--   0 simone    (1000) simone    (1000)       53 2023-04-09 10:02:37.000000 webtypy-0.1.3/src/webtypy.egg-info/requires.txt
+-rw-rw-r--   0 simone    (1000) simone    (1000)        3 2023-04-09 10:02:37.000000 webtypy-0.1.3/src/webtypy.egg-info/top_level.txt
```

### Comparing `webtypy-0.1.2/PKG-INFO` & `webtypy-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webtypy
-Version: 0.1.2
+Version: 0.1.3
 Summary: This module contains the DOM types for the majority of the web APIs used in a web browser. These can be used by an IDE to give type hinting and completion during the development using DOM apis.
 Home-page: https://github.com/pyodide/webtypy
 Author: Simone Giacomelli
 Author-email: simone.giacomelli@gmail.com
 License: MPL 2.0
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `webtypy-0.1.2/README.md` & `webtypy-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `webtypy-0.1.2/setup.cfg` & `webtypy-0.1.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = webtypy
 url = https://github.com/pyodide/webtypy
-version = 0.1.2
+version = 0.1.3
 license = MPL 2.0
 license_files = LICENCE
 description = This module contains the DOM types for the majority of the web APIs used in a web browser. These can be used by an IDE to give type hinting and completion during the development using DOM apis.
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Simone Giacomelli
 author_email = simone.giacomelli@gmail.com
```

### Comparing `webtypy-0.1.2/src/js/__init__.pyi` & `webtypy-0.1.3/src/js/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4222,14 +4222,450 @@
     length: int
     def getPropertyValue(self, property: CSSOMString) -> CSSOMString: ...
     def getPropertyPriority(self, property: CSSOMString) -> CSSOMString: ...
     def setProperty(self, property: CSSOMString, value: CSSOMString, priority: CSSOMString | None = ""): ...
     def removeProperty(self, property: CSSOMString) -> CSSOMString: ...
     parentRule: CSSRule | None
     cssFloat: CSSOMString
+    accentColor: String
+    additiveSymbols: String
+    alignContent: String
+    alignItems: String
+    alignSelf: String
+    alignmentBaseline: String
+    all: String
+    animation: String
+    animationComposition: String
+    animationDelay: String
+    animationDirection: String
+    animationDuration: String
+    animationFillMode: String
+    animationIterationCount: String
+    animationName: String
+    animationPlayState: String
+    animationTimingFunction: String
+    appRegion: String
+    appearance: String
+    ascentOverride: String
+    aspectRatio: String
+    backdropFilter: String
+    backfaceVisibility: String
+    background: String
+    backgroundAttachment: String
+    backgroundBlendMode: String
+    backgroundClip: String
+    backgroundColor: String
+    backgroundImage: String
+    backgroundOrigin: String
+    backgroundPosition: String
+    backgroundPositionX: String
+    backgroundPositionY: String
+    backgroundRepeat: String
+    backgroundRepeatX: String
+    backgroundRepeatY: String
+    backgroundSize: String
+    basePalette: String
+    baselineShift: String
+    baselineSource: String
+    blockSize: String
+    border: String
+    borderBlock: String
+    borderBlockColor: String
+    borderBlockEnd: String
+    borderBlockEndColor: String
+    borderBlockEndStyle: String
+    borderBlockEndWidth: String
+    borderBlockStart: String
+    borderBlockStartColor: String
+    borderBlockStartStyle: String
+    borderBlockStartWidth: String
+    borderBlockStyle: String
+    borderBlockWidth: String
+    borderBottom: String
+    borderBottomColor: String
+    borderBottomLeftRadius: String
+    borderBottomRightRadius: String
+    borderBottomStyle: String
+    borderBottomWidth: String
+    borderCollapse: String
+    borderColor: String
+    borderEndEndRadius: String
+    borderEndStartRadius: String
+    borderImage: String
+    borderImageOutset: String
+    borderImageRepeat: String
+    borderImageSlice: String
+    borderImageSource: String
+    borderImageWidth: String
+    borderInline: String
+    borderInlineColor: String
+    borderInlineEnd: String
+    borderInlineEndColor: String
+    borderInlineEndStyle: String
+    borderInlineEndWidth: String
+    borderInlineStart: String
+    borderInlineStartColor: String
+    borderInlineStartStyle: String
+    borderInlineStartWidth: String
+    borderInlineStyle: String
+    borderInlineWidth: String
+    borderLeft: String
+    borderLeftColor: String
+    borderLeftStyle: String
+    borderLeftWidth: String
+    borderRadius: String
+    borderRight: String
+    borderRightColor: String
+    borderRightStyle: String
+    borderRightWidth: String
+    borderSpacing: String
+    borderStartEndRadius: String
+    borderStartStartRadius: String
+    borderStyle: String
+    borderTop: String
+    borderTopColor: String
+    borderTopLeftRadius: String
+    borderTopRightRadius: String
+    borderTopStyle: String
+    borderTopWidth: String
+    borderWidth: String
+    bottom: String
+    boxShadow: String
+    boxSizing: String
+    breakAfter: String
+    breakBefore: String
+    breakInside: String
+    bufferedRendering: String
+    captionSide: String
+    caretColor: String
+    clear: String
+    clip: String
+    clipPath: String
+    clipRule: String
+    color: String
+    colorInterpolation: String
+    colorInterpolationFilters: String
+    colorRendering: String
+    colorScheme: String
+    columnCount: String
+    columnFill: String
+    columnGap: String
+    columnRule: String
+    columnRuleColor: String
+    columnRuleStyle: String
+    columnRuleWidth: String
+    columnSpan: String
+    columnWidth: String
+    columns: String
+    contain: String
+    containIntrinsicBlockSize: String
+    containIntrinsicHeight: String
+    containIntrinsicInlineSize: String
+    containIntrinsicSize: String
+    containIntrinsicWidth: String
+    container: String
+    containerName: String
+    containerType: String
+    content: String
+    contentVisibility: String
+    counterIncrement: String
+    counterReset: String
+    counterSet: String
+    cursor: String
+    cx: String
+    cy: String
+    descentOverride: String
+    direction: String
+    display: String
+    dominantBaseline: String
+    emptyCells: String
+    fallback: String
+    fill: String
+    fillOpacity: String
+    fillRule: String
+    filter: String
+    flex: String
+    flexBasis: String
+    flexDirection: String
+    flexFlow: String
+    flexGrow: String
+    flexShrink: String
+    flexWrap: String
+    floodColor: String
+    floodOpacity: String
+    font: String
+    fontDisplay: String
+    fontFamily: String
+    fontFeatureSettings: String
+    fontKerning: String
+    fontOpticalSizing: String
+    fontPalette: String
+    fontSize: String
+    fontStretch: String
+    fontStyle: String
+    fontSynthesis: String
+    fontSynthesisSmallCaps: String
+    fontSynthesisStyle: String
+    fontSynthesisWeight: String
+    fontVariant: String
+    fontVariantAlternates: String
+    fontVariantCaps: String
+    fontVariantEastAsian: String
+    fontVariantLigatures: String
+    fontVariantNumeric: String
+    fontVariationSettings: String
+    fontWeight: String
+    forcedColorAdjust: String
+    gap: String
+    grid: String
+    gridArea: String
+    gridAutoColumns: String
+    gridAutoFlow: String
+    gridAutoRows: String
+    gridColumn: String
+    gridColumnEnd: String
+    gridColumnGap: String
+    gridColumnStart: String
+    gridGap: String
+    gridRow: String
+    gridRowEnd: String
+    gridRowGap: String
+    gridRowStart: String
+    gridTemplate: String
+    gridTemplateAreas: String
+    gridTemplateColumns: String
+    gridTemplateRows: String
+    height: String
+    hyphenateCharacter: String
+    hyphenateLimitChars: String
+    hyphens: String
+    imageOrientation: String
+    imageRendering: String
+    inherits: String
+    initialLetter: String
+    initialValue: String
+    inlineSize: String
+    inset: String
+    insetBlock: String
+    insetBlockEnd: String
+    insetBlockStart: String
+    insetInline: String
+    insetInlineEnd: String
+    insetInlineStart: String
+    isolation: String
+    justifyContent: String
+    justifyItems: String
+    justifySelf: String
+    left: String
+    letterSpacing: String
+    lightingColor: String
+    lineBreak: String
+    lineGapOverride: String
+    lineHeight: String
+    listStyle: String
+    listStyleImage: String
+    listStylePosition: String
+    listStyleType: String
+    margin: String
+    marginBlock: String
+    marginBlockEnd: String
+    marginBlockStart: String
+    marginBottom: String
+    marginInline: String
+    marginInlineEnd: String
+    marginInlineStart: String
+    marginLeft: String
+    marginRight: String
+    marginTop: String
+    marker: String
+    markerEnd: String
+    markerMid: String
+    markerStart: String
+    mask: String
+    maskType: String
+    mathDepth: String
+    mathShift: String
+    mathStyle: String
+    maxBlockSize: String
+    maxHeight: String
+    maxInlineSize: String
+    maxWidth: String
+    minBlockSize: String
+    minHeight: String
+    minInlineSize: String
+    minWidth: String
+    mixBlendMode: String
+    negative: String
+    objectFit: String
+    objectPosition: String
+    objectViewBox: String
+    offset: String
+    offsetDistance: String
+    offsetPath: String
+    offsetRotate: String
+    opacity: String
+    order: String
+    orphans: String
+    outline: String
+    outlineColor: String
+    outlineOffset: String
+    outlineStyle: String
+    outlineWidth: String
+    overflow: String
+    overflowAnchor: String
+    overflowClipMargin: String
+    overflowWrap: String
+    overflowX: String
+    overflowY: String
+    overrideColors: String
+    overscrollBehavior: String
+    overscrollBehaviorBlock: String
+    overscrollBehaviorInline: String
+    overscrollBehaviorX: String
+    overscrollBehaviorY: String
+    pad: String
+    padding: String
+    paddingBlock: String
+    paddingBlockEnd: String
+    paddingBlockStart: String
+    paddingBottom: String
+    paddingInline: String
+    paddingInlineEnd: String
+    paddingInlineStart: String
+    paddingLeft: String
+    paddingRight: String
+    paddingTop: String
+    page: String
+    pageBreakAfter: String
+    pageBreakBefore: String
+    pageBreakInside: String
+    pageOrientation: String
+    paintOrder: String
+    perspective: String
+    perspectiveOrigin: String
+    placeContent: String
+    placeItems: String
+    placeSelf: String
+    pointerEvents: String
+    position: String
+    prefix: String
+    quotes: String
+    range: String
+    resize: String
+    right: String
+    rotate: String
+    rowGap: String
+    rubyPosition: String
+    rx: String
+    ry: String
+    scale: String
+    scrollBehavior: String
+    scrollMargin: String
+    scrollMarginBlock: String
+    scrollMarginBlockEnd: String
+    scrollMarginBlockStart: String
+    scrollMarginBottom: String
+    scrollMarginInline: String
+    scrollMarginInlineEnd: String
+    scrollMarginInlineStart: String
+    scrollMarginLeft: String
+    scrollMarginRight: String
+    scrollMarginTop: String
+    scrollPadding: String
+    scrollPaddingBlock: String
+    scrollPaddingBlockEnd: String
+    scrollPaddingBlockStart: String
+    scrollPaddingBottom: String
+    scrollPaddingInline: String
+    scrollPaddingInlineEnd: String
+    scrollPaddingInlineStart: String
+    scrollPaddingLeft: String
+    scrollPaddingRight: String
+    scrollPaddingTop: String
+    scrollSnapAlign: String
+    scrollSnapStop: String
+    scrollSnapType: String
+    scrollbarGutter: String
+    shapeImageThreshold: String
+    shapeMargin: String
+    shapeOutside: String
+    shapeRendering: String
+    size: String
+    sizeAdjust: String
+    speak: String
+    speakAs: String
+    src: String
+    stopColor: String
+    stopOpacity: String
+    stroke: String
+    strokeDasharray: String
+    strokeDashoffset: String
+    strokeLinecap: String
+    strokeLinejoin: String
+    strokeMiterlimit: String
+    strokeOpacity: String
+    strokeWidth: String
+    suffix: String
+    symbols: String
+    syntax: String
+    system: String
+    tabSize: String
+    tableLayout: String
+    textAlign: String
+    textAlignLast: String
+    textAnchor: String
+    textCombineUpright: String
+    textDecoration: String
+    textDecorationColor: String
+    textDecorationLine: String
+    textDecorationSkipInk: String
+    textDecorationStyle: String
+    textDecorationThickness: String
+    textEmphasis: String
+    textEmphasisColor: String
+    textEmphasisPosition: String
+    textEmphasisStyle: String
+    textIndent: String
+    textOrientation: String
+    textOverflow: String
+    textRendering: String
+    textShadow: String
+    textSizeAdjust: String
+    textTransform: String
+    textUnderlineOffset: String
+    textUnderlinePosition: String
+    top: String
+    touchAction: String
+    transform: String
+    transformBox: String
+    transformOrigin: String
+    transformStyle: String
+    transition: String
+    transitionDelay: String
+    transitionDuration: String
+    transitionProperty: String
+    transitionTimingFunction: String
+    translate: String
+    unicodeBidi: String
+    unicodeRange: String
+    userSelect: String
+    vectorEffect: String
+    verticalAlign: String
+    viewTransitionName: String
+    visibility: String
+    whiteSpace: String
+    widows: String
+    width: String
+    willChange: String
+    wordBreak: String
+    wordSpacing: String
+    wordWrap: String
+    writingMode: String
+    zIndex: String
+    zoom: String
 
 class MathMLElement(Element, ElementCSSInlineStyle, GlobalEventHandlers, HTMLOrSVGElement): ...
 
 class ElementInternals(ARIAMixin):
     states: CustomStateSet
     shadowRoot: ShadowRoot | None
     def setFormValue(self, value: File | USVString | FormData | None, state: File | USVString | FormData | None = None): ...
```

### Comparing `webtypy-0.1.2/src/webtypy.egg-info/PKG-INFO` & `webtypy-0.1.3/src/webtypy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webtypy
-Version: 0.1.2
+Version: 0.1.3
 Summary: This module contains the DOM types for the majority of the web APIs used in a web browser. These can be used by an IDE to give type hinting and completion during the development using DOM apis.
 Home-page: https://github.com/pyodide/webtypy
 Author: Simone Giacomelli
 Author-email: simone.giacomelli@gmail.com
 License: MPL 2.0
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

