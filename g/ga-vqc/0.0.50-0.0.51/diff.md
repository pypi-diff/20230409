# Comparing `tmp/ga_vqc-0.0.50.tar.gz` & `tmp/ga_vqc-0.0.51.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ga_vqc-0.0.50.tar", last modified: Sun Apr  9 06:53:22 2023, max compression
+gzip compressed data, was "ga_vqc-0.0.51.tar", last modified: Sun Apr  9 08:41:32 2023, max compression
```

## Comparing `ga_vqc-0.0.50.tar` & `ga_vqc-0.0.51.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 tsievert   (502) staff       (20)        0 2023-04-09 06:53:22.863282 ga_vqc-0.0.50/
--rw-r--r--   0 tsievert   (502) staff       (20)     1076 2023-02-08 00:23:26.000000 ga_vqc-0.0.50/LICENSE
--rw-r--r--   0 tsievert   (502) staff       (20)     1260 2023-04-09 06:53:22.862946 ga_vqc-0.0.50/PKG-INFO
--rw-r--r--   0 tsievert   (502) staff       (20)      791 2023-04-01 20:47:43.000000 ga_vqc-0.0.50/README.md
-drwxr-xr-x   0 tsievert   (502) staff       (20)        0 2023-04-09 06:53:22.860237 ga_vqc-0.0.50/ga_vqc/
--rw-r--r--   0 tsievert   (502) staff       (20)     1916 2023-04-09 06:07:20.000000 ga_vqc-0.0.50/ga_vqc/Distance.py
--rw-r--r--   0 tsievert   (502) staff       (20)      495 2023-03-23 02:52:56.000000 ga_vqc-0.0.50/ga_vqc/GA_ABC.py
--rw-r--r--   0 tsievert   (502) staff       (20)      565 2023-04-07 18:02:50.000000 ga_vqc-0.0.50/ga_vqc/GA_Manager.py
--rw-r--r--   0 tsievert   (502) staff       (20)     1019 2023-03-23 02:52:56.000000 ga_vqc-0.0.50/ga_vqc/GA_Support.py
--rw-r--r--   0 tsievert   (502) staff       (20)     2598 2023-04-07 17:34:26.000000 ga_vqc-0.0.50/ga_vqc/Genes.py
--rw-r--r--   0 tsievert   (502) staff       (20)      430 2023-03-23 02:52:56.000000 ga_vqc-0.0.50/ga_vqc/VQC_ABC.py
--rw-r--r--   0 tsievert   (502) staff       (20)       69 2023-04-07 16:50:57.000000 ga_vqc-0.0.50/ga_vqc/__init__.py
--rw-r--r--   0 tsievert   (502) staff       (20)    10808 2023-04-09 05:43:08.000000 ga_vqc-0.0.50/ga_vqc/simple_Individual.py
--rw-r--r--   0 tsievert   (502) staff       (20)    16569 2023-04-09 06:51:39.000000 ga_vqc-0.0.50/ga_vqc/simple_Model.py
-drwxr-xr-x   0 tsievert   (502) staff       (20)        0 2023-04-09 06:53:22.862440 ga_vqc-0.0.50/ga_vqc.egg-info/
--rw-r--r--   0 tsievert   (502) staff       (20)     1260 2023-04-09 06:53:22.000000 ga_vqc-0.0.50/ga_vqc.egg-info/PKG-INFO
--rw-r--r--   0 tsievert   (502) staff       (20)      357 2023-04-09 06:53:22.000000 ga_vqc-0.0.50/ga_vqc.egg-info/SOURCES.txt
--rw-r--r--   0 tsievert   (502) staff       (20)        1 2023-04-09 06:53:22.000000 ga_vqc-0.0.50/ga_vqc.egg-info/dependency_links.txt
--rw-r--r--   0 tsievert   (502) staff       (20)      132 2023-04-09 06:53:22.000000 ga_vqc-0.0.50/ga_vqc.egg-info/requires.txt
--rw-r--r--   0 tsievert   (502) staff       (20)        7 2023-04-09 06:53:22.000000 ga_vqc-0.0.50/ga_vqc.egg-info/top_level.txt
--rw-r--r--   0 tsievert   (502) staff       (20)       38 2023-04-09 06:53:22.863379 ga_vqc-0.0.50/setup.cfg
--rw-r--r--   0 tsievert   (502) staff       (20)     1067 2023-04-09 06:52:05.000000 ga_vqc-0.0.50/setup.py
+drwxr-xr-x   0 tsievert   (502) staff       (20)        0 2023-04-09 08:41:32.989402 ga_vqc-0.0.51/
+-rw-r--r--   0 tsievert   (502) staff       (20)     1076 2023-02-08 00:23:26.000000 ga_vqc-0.0.51/LICENSE
+-rw-r--r--   0 tsievert   (502) staff       (20)     1260 2023-04-09 08:41:32.989009 ga_vqc-0.0.51/PKG-INFO
+-rw-r--r--   0 tsievert   (502) staff       (20)      791 2023-04-01 20:47:43.000000 ga_vqc-0.0.51/README.md
+drwxr-xr-x   0 tsievert   (502) staff       (20)        0 2023-04-09 08:41:32.986683 ga_vqc-0.0.51/ga_vqc/
+-rw-r--r--   0 tsievert   (502) staff       (20)     1916 2023-04-09 06:07:20.000000 ga_vqc-0.0.51/ga_vqc/Distance.py
+-rw-r--r--   0 tsievert   (502) staff       (20)      495 2023-03-23 02:52:56.000000 ga_vqc-0.0.51/ga_vqc/GA_ABC.py
+-rw-r--r--   0 tsievert   (502) staff       (20)      565 2023-04-07 18:02:50.000000 ga_vqc-0.0.51/ga_vqc/GA_Manager.py
+-rw-r--r--   0 tsievert   (502) staff       (20)     1007 2023-04-09 08:12:19.000000 ga_vqc-0.0.51/ga_vqc/GA_Support.py
+-rw-r--r--   0 tsievert   (502) staff       (20)     2598 2023-04-07 17:34:26.000000 ga_vqc-0.0.51/ga_vqc/Genes.py
+-rw-r--r--   0 tsievert   (502) staff       (20)      430 2023-03-23 02:52:56.000000 ga_vqc-0.0.51/ga_vqc/VQC_ABC.py
+-rw-r--r--   0 tsievert   (502) staff       (20)       69 2023-04-07 16:50:57.000000 ga_vqc-0.0.51/ga_vqc/__init__.py
+-rw-r--r--   0 tsievert   (502) staff       (20)    11015 2023-04-09 08:26:52.000000 ga_vqc-0.0.51/ga_vqc/simple_Individual.py
+-rw-r--r--   0 tsievert   (502) staff       (20)    17922 2023-04-09 08:39:45.000000 ga_vqc-0.0.51/ga_vqc/simple_Model.py
+drwxr-xr-x   0 tsievert   (502) staff       (20)        0 2023-04-09 08:41:32.988536 ga_vqc-0.0.51/ga_vqc.egg-info/
+-rw-r--r--   0 tsievert   (502) staff       (20)     1260 2023-04-09 08:41:32.000000 ga_vqc-0.0.51/ga_vqc.egg-info/PKG-INFO
+-rw-r--r--   0 tsievert   (502) staff       (20)      357 2023-04-09 08:41:32.000000 ga_vqc-0.0.51/ga_vqc.egg-info/SOURCES.txt
+-rw-r--r--   0 tsievert   (502) staff       (20)        1 2023-04-09 08:41:32.000000 ga_vqc-0.0.51/ga_vqc.egg-info/dependency_links.txt
+-rw-r--r--   0 tsievert   (502) staff       (20)      132 2023-04-09 08:41:32.000000 ga_vqc-0.0.51/ga_vqc.egg-info/requires.txt
+-rw-r--r--   0 tsievert   (502) staff       (20)        7 2023-04-09 08:41:32.000000 ga_vqc-0.0.51/ga_vqc.egg-info/top_level.txt
+-rw-r--r--   0 tsievert   (502) staff       (20)       38 2023-04-09 08:41:32.989501 ga_vqc-0.0.51/setup.cfg
+-rw-r--r--   0 tsievert   (502) staff       (20)     1067 2023-04-09 08:05:39.000000 ga_vqc-0.0.51/setup.py
```

### Comparing `ga_vqc-0.0.50/LICENSE` & `ga_vqc-0.0.51/LICENSE`

 * *Files identical despite different names*

### Comparing `ga_vqc-0.0.50/PKG-INFO` & `ga_vqc-0.0.51/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ga_vqc
-Version: 0.0.50
+Version: 0.0.51
 Summary: Genetic Algorithm for VQC ansatz search.
 Home-page: https://github.com/tcoulvert/GA_Ansatz_Search
 Author: Thomas Sievert
 Author-email: 63161166+tcoulvert@users.noreply.github.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ga_vqc-0.0.50/README.md` & `ga_vqc-0.0.51/README.md`

 * *Files identical despite different names*

### Comparing `ga_vqc-0.0.50/ga_vqc/Distance.py` & `ga_vqc-0.0.51/ga_vqc/Distance.py`

 * *Files identical despite different names*

### Comparing `ga_vqc-0.0.50/ga_vqc/GA_Manager.py` & `ga_vqc-0.0.51/ga_vqc/GA_Manager.py`

 * *Files identical despite different names*

### Comparing `ga_vqc-0.0.50/ga_vqc/GA_Support.py` & `ga_vqc-0.0.51/ga_vqc/GA_Support.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import json
 import os
 
 
 def make_results_json(results, start_time, script_path, gen, final_flag=False):
     if final_flag:
-        filename = "final_evolution_results-%s.json" % (start_time)
+        filename = "final_evolution_results.json"
     else:
-        filename = "%03d_evolution_results-%s.json" % (gen, start_time)
-    destdir = os.path.join(script_path, "ga_runs")
+        filename = "%03d_evolution_results.json" % gen
+    destdir = os.path.join(script_path, "ga_runs", "run-%s" % start_time)
     filepath = os.path.join(destdir, filename)
     if not os.path.exists(destdir):
         os.makedirs(destdir)
     json.dump(results, open(filepath, "w"), indent=4)
 
-    return filename
+    return filepath
 
 
 class UnsupportedBackendDecorator(Exception):
     """Exception raised for errors in the backend 'type' decoration.
 
     Attributes:
         bknd_type -- input backend decoration that caused the error
```

### Comparing `ga_vqc-0.0.50/ga_vqc/Genes.py` & `ga_vqc-0.0.51/ga_vqc/Genes.py`

 * *Files identical despite different names*

### Comparing `ga_vqc-0.0.50/ga_vqc/simple_Individual.py` & `ga_vqc-0.0.51/ga_vqc/simple_Individual.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 class Individual(GA_Individual):
     """
     Data structure for the ansatz.
     """
 
-    def __init__(self, n_qubits, n_moments, genepool, rng_seed):
+    def __init__(self, n_qubits, n_moments, genepool, rng_seed, ansatz=None):
         """
         Initializes the inidivual object, all individuals (ansatz) are members of this class.
             - n_qubits: Number of qubits in the ansatz.
             - n_moments: Number of moments in the ansatz.
             - genepool: All the allowed gates for the ansatz, as well as meta-data 
                             about those gates.
 
@@ -29,15 +29,18 @@
         self.pennylane_rng = pnp.random.default_rng(seed=rng_seed)
 
         self.ansatz_dicts = []
         self.ansatz_qml = []
         self.ansatz_draw = []
         self.params = []
 
-        self.generate()  # Should this be done automatically?
+        if ansatz is None:
+            self.generate()
+        else:
+            self.generate_from(ansatz)
         self.convert_to_qml()
         self.draw_ansatz()
 
     def __len__(self):
         return len(self.ansatz_dicts[0])
 
     def __getitem__(self, key):
@@ -91,14 +94,19 @@
 
                     if self.ansatz_dicts[moment][qubit] == 0:
                         gate = self.genepool.choice(n_qubits=1)
                         self.ansatz_dicts[moment][qubit] = gate.name
                 else:
                     raise Exception("Gates with more than 2 qubits haven't been implemented yet.")
 
+    def generate_from(self, ansatz):
+        self.ansatz_dicts = copy.deepcopy(ansatz)
+        self.convert_to_qml()
+        self.ansatz_draw()
+
     def convert_to_qml(self):
         """
         Converts the ansatz into a general format for the QML.
 
             moment_dict example: _C (_T) means current qubit is control (target) qubit of 2-qubit gate
                 {'I': [],
                  'RX': [],
@@ -224,24 +232,23 @@
             qubit_pairs = self.rng.permutation(self.n_qubits)
             for qubit_pair in qubit_pairs:
                 if qubit_pair == qubit:
                     continue
                 if self.ansatz_dicts[moment][qubit_pair].find("_") > 0:
                     double_swap_flag += 1
                     gate_pair = self.genepool.choice()
-                    if double_swap_flag == 2 and gate_pair.n_qubits == 1:
+                    if double_swap_flag == 2 and gate_pair.n_qubits == 2:
                         direction = self.rng.permutation(["_C", "_T"])
                         self.ansatz_dicts[moment][int(self.ansatz_dicts[moment][qubit][-1])] = (
-                            gate.name + direction[0] + f"-{int(self.ansatz_dicts[moment][qubit_pair][-1])}"
+                            gate_pair.name + direction[0] + f"-{int(self.ansatz_dicts[moment][qubit_pair][-1])}"
                         )
                         self.ansatz_dicts[moment][int(self.ansatz_dicts[moment][qubit_pair][-1])] = (
-                            gate.name + direction[1] + f"-{int(self.ansatz_dicts[moment][qubit][-1])}"
+                            gate_pair.name + direction[1] + f"-{int(self.ansatz_dicts[moment][qubit][-1])}"
                         )
                     else:
-                        self.ansatz_dicts[moment][int(self.ansatz_dicts[moment][qubit_pair][-1])] = self.rng.choice(
-                            self.gates_arr[:-1]
-                        )
+                        gate_pair = self.genepool.choice(n_qubits=1)
+                        self.ansatz_dicts[moment][int(self.ansatz_dicts[moment][qubit_pair][-1])] = gate_pair.name
 
                 direction = self.rng.permutation(["_C", "_T"])
                 self.ansatz_dicts[moment][qubit] = gate.name + direction[0] + f"-{qubit_pair}"
                 self.ansatz_dicts[moment][qubit_pair] = gate.name + direction[1] + f"-{qubit}"
                 break
```

### Comparing `ga_vqc-0.0.50/ga_vqc/simple_Model.py` & `ga_vqc-0.0.51/ga_vqc/simple_Model.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,14 +41,15 @@
         self.n_winners = config["n_winners"]
         self.n_mutations = config["n_mutations"]
         self.n_mate_swaps = config["n_mate_swaps"]
         self.n_steps_patience = config["n_steps_patience"]
         self.best_perf = {
             "fitness": 0,
             "eval_metrics": [],
+            "ansatz": None,
             "ansatz_dicts": [],
             "ansatz_draw": str(),
             "generation": 0,
             "index": 0,
         }
 
         self.start_time = datetime.datetime.now().strftime("%Y-%m-%d_%H-%M-%S")
@@ -133,23 +134,47 @@
                 f"Best metrics: {self.best_perf['eval_metrics']}, " +
                 f"Best ansatz: {self.best_perf['ansatz_dicts']}"
             )
 
             if gen > 20:
                 if (gen - self.best_perf["generation"]) > self.n_steps_patience:
                     break
-            make_results_json(results, self.start_time, self.ga_output_path, gen)
+            print(
+                "filepath is: ",
+                make_results_json(results, self.start_time, self.ga_output_path, gen)
+            )
             gen += 1
         print(
-            "filename is: ",
+            "filepath is: ",
             make_results_json(
                 results, self.start_time, self.ga_output_path, gen, final_flag=True
             ),
         )
 
+        ### Final re-training for std. dev. estimate ###
+        ansatz = self.best_perf["ansatz"]
+        ansatz.convert_to_qml()
+        ansatz.draw_ansatz()
+        vqc_config_ansatz = {key: value for key, value in self.vqc_config.items()}
+        vqc_config_ansatz["ansatz_dicts"] = ansatz.ansatz_dicts
+        vqc_config_ansatz["ansatz_qml"] = ansatz.ansatz_qml
+        vqc_config_ansatz["params"] = ansatz.params
+        vqc_config_ansatz["gen"] = gen
+        fitness_arr = []
+        auroc_arr = []
+        for i in range(20):
+            vqc_config_ansatz["ix"] = i
+            output_dict = self.vqc(vqc_config_ansatz)
+            fitness_arr.append(output_dict["fitness_metric"])
+            auroc_arr.append(output_dict["eval_metrics"]["auroc"])
+        print(f"Final fitness distribution: {fitness_arr}")
+        print(f"Avg fitness: {np.mean(fitness_arr)},  Std Dev: {np.std(fitness_arr)}, Std Dev of Mean: {np.std(fitness_arr) / (20**0.5)}")
+        print(f"Final AUROC distribution: {auroc_arr}")
+        print(f"Avg AUROC: {np.mean(auroc_arr)},  Std Dev: {np.std(auroc_arr)}, Std Dev of Mean: {np.std(auroc_arr) / (20**0.5)}")
+
     def evaluate_fitness(self, gen):
         """
         Evaluates the fitness level of all ansatz. Runs the QML optimization task.
 
         TODO: change to do per given ansatz (so we don't have to train every ansatz).
             -> make so fitness_arr can be shorter than population
         """
@@ -190,51 +215,54 @@
 
         if self.best_perf["fitness"] < np.amax(self.fitness_arr):
             print("!! IMPROVED PERFORMANCE !!")
             self.best_perf["fitness"] = np.amax(self.fitness_arr).item()
             self.best_perf["eval_metrics"] = copy.deepcopy(
                 self.metrics_arr[np.argmax(self.fitness_arr)]
             )
+            self.best_perf["ansatz"] = copy.deepcopy(
+                self.population[np.argmax(self.fitness_arr)]
+            )
             self.best_perf["ansatz_dicts"] = copy.deepcopy(
                 self.population[np.argmax(self.fitness_arr)].ansatz_dicts
             )
             self.best_perf["ansatz_draw"] = copy.deepcopy(
                 self.population[np.argmax(self.fitness_arr)].ansatz_draw
             )
             self.best_perf["generation"] = gen
             self.best_perf["index"] = np.argmax(self.fitness_arr).item()
 
     def make_results(self, gen):
         ### Euclidean distances ###
         distances_from_best = euclidean_distances(self.population[np.argmax(self.fitness_arr)], self.population)
-        destdir_curves = os.path.join(self.ga_output_path, "ga_curves")
+        destdir_curves = os.path.join(self.ga_output_path, "ga_curves", "run-%s" % self.start_time)
         if not os.path.exists(destdir_curves):
             os.makedirs(destdir_curves)
         filepath_euclid = os.path.join(
             destdir_curves,
-            "%03deuclid_distance-%s_data.png"
-            % (gen, self.start_time),
+            "%03deuclid_distance_data.png"
+            % gen
         )
         plt.figure(0)
         plt.style.use("seaborn")
         plt.scatter(distances_from_best, [i["auroc"] for i in self.metrics_arr], marker=".", color="g")
         plt.ylabel("AUROC")
         plt.xlabel("Euclidian distance from best ansatz")
         plt.title("Euclidean Distances from Best Performing Ansatz")
         plt.savefig(filepath_euclid, format="png")
         plt.close(0)
         ### tSNE clustering ###
         data_tsne = tsne(self.population, rng_seed=self.rng_seed, perplexity=2)
         x, y = data_tsne[0], data_tsne[1]
         filepath_tsne = os.path.join(
             destdir_curves,
-            "%03dtsne_distance-%s_data.png"
-            % (gen, self.start_time),
+            "%03dtsne_distance_data.png"
+            % gen
         )
-        plt.figure(0)
+        plt.figure(1)
         plt.style.use("seaborn")
         plt.scatter(x, y, marker=".", c=[i["auroc"] for i in self.metrics_arr], cmap=plt.set_cmap('plasma'))
         plt.ylabel("a.u.")
         plt.xlabel("a.u.")
         cbar = plt.colorbar()
         cbar.set_label("AUROC")
         plt.title("tSNE of Current Population")
@@ -265,15 +293,15 @@
         return results
 
     def select(self):
         """
         Picks the top performing ansatz from a generation to mate and mutate for the next generation.
         """
         winner_arr = []
-        for i in range(self.n_winners):
+        for _ in range(self.n_winners):
             winner_ix = np.argmax(self.fitness_arr)
             winner = self.population[winner_ix]
             winner_arr.append(winner)
             self.fitness_arr.pop(winner_ix)
 
         self.population = []
         return winner_arr
```

### Comparing `ga_vqc-0.0.50/ga_vqc.egg-info/PKG-INFO` & `ga_vqc-0.0.51/ga_vqc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ga-vqc
-Version: 0.0.50
+Version: 0.0.51
 Summary: Genetic Algorithm for VQC ansatz search.
 Home-page: https://github.com/tcoulvert/GA_Ansatz_Search
 Author: Thomas Sievert
 Author-email: 63161166+tcoulvert@users.noreply.github.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ga_vqc-0.0.50/setup.py` & `ga_vqc-0.0.51/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="ga_vqc",
-    version="0.0.50",
+    version="0.0.51",
     description="Genetic Algorithm for VQC ansatz search.",
     packages=find_packages(include=["ga_vqc"]),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
```

