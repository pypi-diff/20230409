# Comparing `tmp/kpLib-1.0.5.tar.gz` & `tmp/kpLib-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kpLib-1.0.5.tar", last modified: Thu Apr 22 23:55:42 2021, max compression
+gzip compressed data, was "kpLib-1.1.0.tar", last modified: Sun Apr  9 03:28:31 2023, max compression
```

## Comparing `kpLib-1.0.5.tar` & `kpLib-1.1.0.tar`

### file list

```diff
@@ -1,36 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-22 23:55:42.000000 kpLib-1.0.5/
--rw-rw-rw-   0 root         (0) root         (0)       16 2021-04-22 23:54:12.000000 kpLib-1.0.5/.clang-format
--rw-rw-rw-   0 root         (0) root         (0)     1470 2021-04-22 23:54:12.000000 kpLib-1.0.5/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      800 2021-04-22 23:54:12.000000 kpLib-1.0.5/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      278 2021-04-22 23:54:12.000000 kpLib-1.0.5/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      982 2021-04-22 23:54:12.000000 kpLib-1.0.5/CMakeLists.txt
--rw-rw-rw-   0 root         (0) root         (0)    10767 2021-04-22 23:54:12.000000 kpLib-1.0.5/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       81 2021-04-22 23:54:12.000000 kpLib-1.0.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    15288 2021-04-22 23:55:42.000000 kpLib-1.0.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    11927 2021-04-22 23:54:12.000000 kpLib-1.0.5/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1304 2021-04-22 23:54:12.000000 kpLib-1.0.5/RELEASE.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-22 23:55:42.000000 kpLib-1.0.5/python/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-22 23:55:42.000000 kpLib-1.0.5/python/kpLib/
--rw-rw-rw-   0 root         (0) root         (0)      235 2021-04-22 23:54:12.000000 kpLib-1.0.5/python/kpLib/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3183 2021-04-22 23:54:12.000000 kpLib-1.0.5/python/kpLib/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1508 2021-04-22 23:54:12.000000 kpLib-1.0.5/python/kpLib/interface.cpp
--rw-rw-rw-   0 root         (0) root         (0)     3578 2021-04-22 23:54:12.000000 kpLib-1.0.5/python/kpLib/interface.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-22 23:55:42.000000 kpLib-1.0.5/python/kpLib.egg-info/
--rw-r--r--   0 root         (0) root         (0)    15288 2021-04-22 23:55:42.000000 kpLib-1.0.5/python/kpLib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      715 2021-04-22 23:55:42.000000 kpLib-1.0.5/python/kpLib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-04-22 23:55:42.000000 kpLib-1.0.5/python/kpLib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       52 2021-04-22 23:55:42.000000 kpLib-1.0.5/python/kpLib.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-04-22 23:55:42.000000 kpLib-1.0.5/python/kpLib.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       42 2021-04-22 23:55:42.000000 kpLib-1.0.5/python/kpLib.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2021-04-22 23:55:42.000000 kpLib-1.0.5/python/kpLib.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       48 2021-04-22 23:54:12.000000 kpLib-1.0.5/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2021-04-22 23:55:42.000000 kpLib-1.0.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2225 2021-04-22 23:54:12.000000 kpLib-1.0.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-22 23:55:42.000000 kpLib-1.0.5/src/
--rw-rw-rw-   0 root         (0) root         (0)     5150 2021-04-22 23:54:12.000000 kpLib-1.0.5/src/kPointLattice.cpp
--rw-rw-rw-   0 root         (0) root         (0)     2984 2021-04-22 23:54:12.000000 kpLib-1.0.5/src/kPointLattice.h
--rw-rw-rw-   0 root         (0) root         (0)    32901 2021-04-22 23:54:12.000000 kpLib-1.0.5/src/kPointLatticeGenerator.cpp
--rw-rw-rw-   0 root         (0) root         (0)    10241 2021-04-22 23:54:12.000000 kpLib-1.0.5/src/kPointLatticeGenerator.h
--rw-rw-rw-   0 root         (0) root         (0)     6788 2021-04-22 23:54:12.000000 kpLib-1.0.5/src/msmath.cpp
--rw-rw-rw-   0 root         (0) root         (0)     2717 2021-04-22 23:54:12.000000 kpLib-1.0.5/src/msmath.h
--rw-rw-rw-   0 root         (0) root         (0)     5993 2021-04-22 23:54:12.000000 kpLib-1.0.5/src/msmath.ipp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 03:28:31.806728 kpLib-1.1.0/
+-rw-rw-rw-   0 root         (0) root         (0)    10767 2023-04-09 03:27:56.000000 kpLib-1.1.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       81 2023-04-09 03:27:56.000000 kpLib-1.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    25972 2023-04-09 03:28:31.805728 kpLib-1.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    24795 2023-04-09 03:27:56.000000 kpLib-1.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 03:28:31.798728 kpLib-1.1.0/python/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 03:28:31.802728 kpLib-1.1.0/python/kpLib/
+-rw-rw-rw-   0 root         (0) root         (0)      233 2023-04-09 03:27:56.000000 kpLib-1.1.0/python/kpLib/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3301 2023-04-09 03:27:56.000000 kpLib-1.1.0/python/kpLib/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     4245 2023-04-09 03:27:56.000000 kpLib-1.1.0/python/kpLib/interface.cpp
+-rw-rw-rw-   0 root         (0) root         (0)     6839 2023-04-09 03:27:56.000000 kpLib-1.1.0/python/kpLib/interface.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 03:28:31.805728 kpLib-1.1.0/python/kpLib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    25972 2023-04-09 03:28:31.000000 kpLib-1.1.0/python/kpLib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      463 2023-04-09 03:28:31.000000 kpLib-1.1.0/python/kpLib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-09 03:28:31.000000 kpLib-1.1.0/python/kpLib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2023-04-09 03:28:31.000000 kpLib-1.1.0/python/kpLib.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-09 03:28:28.000000 kpLib-1.1.0/python/kpLib.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       63 2023-04-09 03:28:31.000000 kpLib-1.1.0/python/kpLib.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-04-09 03:28:31.000000 kpLib-1.1.0/python/kpLib.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-09 03:28:31.806728 kpLib-1.1.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2938 2023-04-09 03:27:56.000000 kpLib-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 03:28:31.801728 kpLib-1.1.0/src/
+-rw-rw-rw-   0 root         (0) root         (0)     5150 2023-04-09 03:27:56.000000 kpLib-1.1.0/src/kPointLattice.cpp
+-rw-rw-rw-   0 root         (0) root         (0)    33024 2023-04-09 03:27:56.000000 kpLib-1.1.0/src/kPointLatticeGenerator.cpp
+-rw-rw-rw-   0 root         (0) root         (0)     6788 2023-04-09 03:27:56.000000 kpLib-1.1.0/src/msmath.cpp
```

### Comparing `kpLib-1.0.5/LICENSE` & `kpLib-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kpLib-1.0.5/python/kpLib/cli.py` & `kpLib-1.1.0/python/kpLib/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import click
 import numpy as np
 from pymatgen.core import Structure
 from pymatgen.io.vasp.inputs import Kpoints, Kpoints_supported_modes
 from kpLib import __version__
-from kpLib.interface import get_kpoints
+from kpLib.interface import get_kpoints, SYMPREC
 
 
 @click.command()
-@click.argument("Structure", default="POSCAR", required=False)
+@click.argument("structure", default="POSCAR", required=False)
+@click.argument("output", default="KPOINTS", required=False)
 @click.option(
-    "-t",
-    "--type",
-    "ktype",
-    default="AUTO",
-    type=click.Choice(["AUTO", "GAMMA", "SHIFTED"], case_sensitive=False),
-    help="Type of Kpoint grid: auto-determined, gamma centered, or shifted"
-    "to not include gamma",
+    "-g",
+    "--gamma",
+    "include_gamma",
+    default="auto",
+    type=click.Choice(["auto", "true", "false"], case_sensitive=False),
+    help="Type of Kpoint grid: auto-determined, gamma centered, or shifted grid"
 )
 @click.option(
-    "--symprec", default=1e-5, help="Precision for symmetry finding in spglib."
+    "--symprec", default=SYMPREC, help="Precision for symmetry finding in spglib."
 )
 @click.option(
     "-s",
     "--use_scale_factor",
     default=False,
     type=bool,
     is_flag=True,
@@ -46,44 +46,43 @@
     "print_version",
     type=bool,
     is_flag=True,
     help="Prints out the version information for kpGen",
 )
 def generate(
     structure,
+    output,
     min_distance,
     min_total_kpoints,
-    ktype,
+    include_gamma,
     symprec,
     use_scale_factor,
     print_version,
 ):
     """
     This script generates a KPOINTs output for a given structure a
     VASP POSCAR, Pymatgen structure JSON, or CIF
     """
 
     if print_version:
         print(f"v{__version__}")
         return
 
-    struc = Structure.from_file(structure)
-    if ktype == "GAMMA":
-        include_gamma = True
-    elif ktype == "SHIFTED":
-        include_gamma = False
-    else:
-        include_gamma = None
+    struct = Structure.from_file(structure)
 
-    click.echo(f"Running kpLib on {struc.composition.reduced_formula}")
+    click.echo(f"Running kpLib on {struct.composition.reduced_formula}")
     kpts = get_kpoints(
-        struc,
-        minDistance=min_distance,
-        minTotalKpoints=min_total_kpoints,
-        include_gamma=include_gamma,
+        struct.lattice.matrix,
+        struct.frac_coords,
+        struct.atomic_numbers,
+        min_distance = min_distance,
+        min_total_kpoints = min_total_kpoints,
+        include_gamma = include_gamma.lower(),
+        symprec = symprec,
+        use_scale_factor = use_scale_factor
     )
 
     # Get distinct points and weights for KPOINTS file
     distinct_coords, distinct_weights = zip(
         *[
             (coord, weight)
             for (coord, weight) in zip(kpts["coords"], kpts["weights"])
@@ -93,16 +92,15 @@
 
     click.echo(f"Generated {len(distinct_coords)} distinct kpoints")
     click.echo(f"Minimum periodic distance is {kpts['min_periodic_distance']}")
 
     comment = (
         f"kpLib version: {__version__}. "
         f"K-Point grid has {kpts['num_total_kpts']} total points. "
-        "Actual minimum periodic distance is"
-        f" {kpts['min_periodic_distance']} Angstroms. "
+        f"Actual minimum periodic distance is {kpts['min_periodic_distance']} Angstroms. "
     )
     if any([np.allclose(d, [0.0, 0.0, 0.0]) for d in distinct_coords]):
         click.echo("Grid includes gamma point.")
         comment += " Grid includes gamma point."
     else:
         click.echo("Grid does not include gamma point.")
         comment += " Grid does not include gamma point."
@@ -111,8 +109,11 @@
         comment=comment,
         style=Kpoints_supported_modes.Reciprocal,
         num_kpts=len(distinct_coords),
         kpts=distinct_coords,
         kpts_weights=distinct_weights,
     )
 
-    kpts_obj.write_file("KPOINTS")
+    kpts_obj.write_file(output)
+
+if __name__ == "__main__":
+    generate()
```

### Comparing `kpLib-1.0.5/src/kPointLattice.cpp` & `kpLib-1.1.0/src/kPointLattice.cpp`

 * *Files identical despite different names*

### Comparing `kpLib-1.0.5/src/kPointLatticeGenerator.cpp` & `kpLib-1.1.0/src/kPointLatticeGenerator.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -10,16 +10,16 @@
  *
  * @param primVectorsArray
  * @param conventionalVectorsArray The third vector should be orthogonal to the first two.
  * @param latticePointOperatorsArray
  * @param numOperators
  * @param isConventionalHexagonal
  */
-KPointLatticeGenerator::KPointLatticeGenerator(const double primVectorsArray[3][3],
-                                               const double conventionalVectorsArray[3][3],
+KPointLatticeGenerator::KPointLatticeGenerator(const double primVectorsArray[][3],
+                                               const double conventionalVectorsArray[][3],
                                                const int latticePointOperatorsArray[][3][3],
                                                const int numOperators,
                                                const bool isConventionalHexagonal) {
 
   const int Ndim = 3;
   Tensor<double> primVectors(Ndim, std::vector<double>(Ndim, 0));
   Tensor<double> conventionalVectors(Ndim, std::vector<double>(Ndim, 0));
@@ -36,29 +36,30 @@
   for (int n = 0; n < numOperators; n++) {
     for (int i = 0; i < Ndim; i++) {
       for (int j = 0; j < Ndim; j++) {
         latticePointOperators[n][i][j] = latticePointOperatorsArray[n][i][j];
       }
     }
   }
-    KPointLatticeGenerator(primVectors,conventionalVectors,latticePointOperators,isConventionalHexagonal);
+
+  initializer(primVectors, conventionalVectors, latticePointOperators, isConventionalHexagonal);
 }
 
 /**
  * Users can get all of the arguments from a SpaceGroup object, but this is more general.
  *
  * @param primVectors
  * @param conventionalVectors The third vector should be orthogonal to the first two.
  * @param latticePointOperators
  * @param isConventionalHexagonal
  */
-KPointLatticeGenerator::KPointLatticeGenerator(Tensor<double> primVectors,
-                                               Tensor<double> conventionalVectors,
-                                               std::vector<Tensor<int>> latticePointOperators,
-                                               const bool isConventionalHexagonal) {
+void KPointLatticeGenerator::initializer(const Tensor<double>& primVectors,
+                                         const Tensor<double>& conventionalVectors,
+                                         const std::vector<Tensor<int>>& latticePointOperators,
+                                         const bool isConventionalHexagonal) {
 
   static const double hexagonal2DShifts[9][2] = {
       {0, 0},
       {1.0 / 3, 1.0 / 3},
       {2.0 / 3, 2.0 / 3},
       {1.0 / 3, 2.0 / 3},
       {2.0 / 3, 1.0 / 3},
@@ -83,14 +84,15 @@
 
   m_Other2DShifts.resize(4, std::vector<double>(2, 0.0));
   for (int i = 0; i < 4; ++i) {
     m_Other2DShifts[i][0] = other2DShifts[i][0];
     m_Other2DShifts[i][1] = other2DShifts[i][1];
   }
 
+  // Copies of the array of operators are made.
   m_PointOperators3D = latticePointOperators;
   // Make it global to save the dynamic allocation;
   m_KPointOperators = std::vector<Tensor<int> >(m_PointOperators3D.size(), Tensor<int>());
 
   m_PrimVectors = primVectors;
   m_CartesianToPrim = MSMath::simpleInverse(primVectors);
   m_PrimCellSize = fabs(MSMath::determinant(primVectors));
@@ -101,28 +103,29 @@
   std::vector<double> directFaceCenter(3, 0);
   MSMath::vectorTimesMatrix(faceCenter, m_CartesianToPrim, directFaceCenter);
   bool isLatticePoint = true;
   for (int dimNum = 0; dimNum < (int) directFaceCenter.size(); dimNum++) {
     int coord = static_cast<int>(MSMath::round(directFaceCenter[dimNum]));
     isLatticePoint &= (coord % 2 == 0);
   }
+
+  m_ConventionalVectors = conventionalVectors;
   if (isLatticePoint) {
-    conventionalVectors[0] = MSMath::arrayDivide(faceCenter, 2);
-    conventionalVectors[1] = MSMath::arraySubtract(conventionalVectors[0], conventionalVectors[1]);
+    m_ConventionalVectors[0] = MSMath::arrayDivide(faceCenter, 2);
+    m_ConventionalVectors[1] = MSMath::arraySubtract(m_ConventionalVectors[0], m_ConventionalVectors[1]);
   }
-  m_ConventionalVectors = conventionalVectors;
 
   if (isConventionalHexagonal) {
     m_Shifts2D = m_Hexagonal2DShifts;
   } else {
     m_Shifts2D = m_Other2DShifts;
   }
 
   Tensor<double> conventionalToPrim =
-      MSMath::matrixMultiply<double, double, double>(conventionalVectors, m_CartesianToPrim);
+      MSMath::matrixMultiply<double, double, double>(m_ConventionalVectors, m_CartesianToPrim);
   Tensor<double> primToConventional = MSMath::simpleInverse(conventionalToPrim);
 
   // Get the two-dimensional point operations.
   std::vector<Tensor<int> > ops2D(m_PointOperators3D.size(), Tensor<int>());
 
   // First we get all of the lattice operations in the coordinates of the conventional
   // lattice vectors.
@@ -171,16 +174,18 @@
     if (match) {
       continue;
     }
     ops2D[keeperIndex++] = op2D;
   }
 
   m_NumConventionalPrimCells = fabs(MSMath::determinant(conventionalToPrim)); // maxLayers;
-  m_MaxZDistance = MSMath::magnitude(conventionalVectors[2]) / m_NumConventionalPrimCells
-      * (isConventionalHexagonal ? 3 : 2);  // 3 is for rhombohedral in primitive hexagonal;
+  // 3 is for primitive rhombohedral unit cell represented in a hexagonal lattice as the
+  // corresponding conventional lattice.
+  m_MaxZDistance = MSMath::magnitude(m_ConventionalVectors[2]) / m_NumConventionalPrimCells
+      * (isConventionalHexagonal ? 3 : 2);
   m_PointOperators2D = ops2D;
   m_PointOperators2D.resize(keeperIndex);
 }
 
 void KPointLatticeGenerator::useScaleFactor(int spaceGroupNum) {
   m_MaxScaleFactor = 3;
   if (spaceGroupNum >0 && spaceGroupNum <= 2) {
@@ -191,16 +196,16 @@
     m_MaxAllowedKPoints = 5832;  // Orthorhombic, Tetragonal, Trigonal, Hexagonal;
   } else if (spaceGroupNum >=195 && spaceGroupNum <= 230){
     m_MaxAllowedKPoints = 46656; // Cubic;
   }
 }
 
 /*
- * Wrapper function of the private getKPointLattice function to disable the scaleFactor for now,
- * but keep the option.
+ * Wrapper function of the private getKPointLattice function to deal with scaleFactor to avoid
+ * deep nested loops.
  */
 KPointLattice KPointLatticeGenerator::getKPointLattice(const double minDistance, const int minSize) {
 
   for (int scaleFactor = 1; scaleFactor <= m_MaxScaleFactor; scaleFactor++) {
     double minScaledDistance = minDistance / scaleFactor;
     int minScaledTotalKPoints = (int) ceil(minSize / pow(scaleFactor, 3));
     KPointLattice lattice = getKPointLattice(minScaledDistance, minScaledTotalKPoints,
```

### Comparing `kpLib-1.0.5/src/msmath.cpp` & `kpLib-1.1.0/src/msmath.cpp`

 * *Files identical despite different names*

