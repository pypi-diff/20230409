# Comparing `tmp/ga_vqc-0.0.49.tar.gz` & `tmp/ga_vqc-0.0.50.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ga_vqc-0.0.49.tar", last modified: Fri Apr  7 19:37:41 2023, max compression
+gzip compressed data, was "ga_vqc-0.0.50.tar", last modified: Sun Apr  9 06:53:22 2023, max compression
```

## Comparing `ga_vqc-0.0.49.tar` & `ga_vqc-0.0.50.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 tsievert   (502) staff       (20)        0 2023-04-07 19:37:41.732835 ga_vqc-0.0.49/
--rw-r--r--   0 tsievert   (502) staff       (20)     1076 2023-02-08 00:23:26.000000 ga_vqc-0.0.49/LICENSE
--rw-r--r--   0 tsievert   (502) staff       (20)     1260 2023-04-07 19:37:41.732509 ga_vqc-0.0.49/PKG-INFO
--rw-r--r--   0 tsievert   (502) staff       (20)      791 2023-04-01 20:47:43.000000 ga_vqc-0.0.49/README.md
-drwxr-xr-x   0 tsievert   (502) staff       (20)        0 2023-04-07 19:37:41.729937 ga_vqc-0.0.49/ga_vqc/
--rw-r--r--   0 tsievert   (502) staff       (20)     1743 2023-04-07 18:51:17.000000 ga_vqc-0.0.49/ga_vqc/Distance.py
--rw-r--r--   0 tsievert   (502) staff       (20)      495 2023-03-23 02:52:56.000000 ga_vqc-0.0.49/ga_vqc/GA_ABC.py
--rw-r--r--   0 tsievert   (502) staff       (20)      565 2023-04-07 18:02:50.000000 ga_vqc-0.0.49/ga_vqc/GA_Manager.py
--rw-r--r--   0 tsievert   (502) staff       (20)     1019 2023-03-23 02:52:56.000000 ga_vqc-0.0.49/ga_vqc/GA_Support.py
--rw-r--r--   0 tsievert   (502) staff       (20)     2598 2023-04-07 17:34:26.000000 ga_vqc-0.0.49/ga_vqc/Genes.py
--rw-r--r--   0 tsievert   (502) staff       (20)      430 2023-03-23 02:52:56.000000 ga_vqc-0.0.49/ga_vqc/VQC_ABC.py
--rw-r--r--   0 tsievert   (502) staff       (20)       69 2023-04-07 16:50:57.000000 ga_vqc-0.0.49/ga_vqc/__init__.py
--rw-r--r--   0 tsievert   (502) staff       (20)     9420 2023-04-07 17:36:08.000000 ga_vqc-0.0.49/ga_vqc/simple_Individual.py
--rw-r--r--   0 tsievert   (502) staff       (20)    16189 2023-04-07 19:37:03.000000 ga_vqc-0.0.49/ga_vqc/simple_Model.py
-drwxr-xr-x   0 tsievert   (502) staff       (20)        0 2023-04-07 19:37:41.732092 ga_vqc-0.0.49/ga_vqc.egg-info/
--rw-r--r--   0 tsievert   (502) staff       (20)     1260 2023-04-07 19:37:41.000000 ga_vqc-0.0.49/ga_vqc.egg-info/PKG-INFO
--rw-r--r--   0 tsievert   (502) staff       (20)      357 2023-04-07 19:37:41.000000 ga_vqc-0.0.49/ga_vqc.egg-info/SOURCES.txt
--rw-r--r--   0 tsievert   (502) staff       (20)        1 2023-04-07 19:37:41.000000 ga_vqc-0.0.49/ga_vqc.egg-info/dependency_links.txt
--rw-r--r--   0 tsievert   (502) staff       (20)      132 2023-04-07 19:37:41.000000 ga_vqc-0.0.49/ga_vqc.egg-info/requires.txt
--rw-r--r--   0 tsievert   (502) staff       (20)        7 2023-04-07 19:37:41.000000 ga_vqc-0.0.49/ga_vqc.egg-info/top_level.txt
--rw-r--r--   0 tsievert   (502) staff       (20)       38 2023-04-07 19:37:41.732931 ga_vqc-0.0.49/setup.cfg
--rw-r--r--   0 tsievert   (502) staff       (20)     1067 2023-04-06 18:50:32.000000 ga_vqc-0.0.49/setup.py
+drwxr-xr-x   0 tsievert   (502) staff       (20)        0 2023-04-09 06:53:22.863282 ga_vqc-0.0.50/
+-rw-r--r--   0 tsievert   (502) staff       (20)     1076 2023-02-08 00:23:26.000000 ga_vqc-0.0.50/LICENSE
+-rw-r--r--   0 tsievert   (502) staff       (20)     1260 2023-04-09 06:53:22.862946 ga_vqc-0.0.50/PKG-INFO
+-rw-r--r--   0 tsievert   (502) staff       (20)      791 2023-04-01 20:47:43.000000 ga_vqc-0.0.50/README.md
+drwxr-xr-x   0 tsievert   (502) staff       (20)        0 2023-04-09 06:53:22.860237 ga_vqc-0.0.50/ga_vqc/
+-rw-r--r--   0 tsievert   (502) staff       (20)     1916 2023-04-09 06:07:20.000000 ga_vqc-0.0.50/ga_vqc/Distance.py
+-rw-r--r--   0 tsievert   (502) staff       (20)      495 2023-03-23 02:52:56.000000 ga_vqc-0.0.50/ga_vqc/GA_ABC.py
+-rw-r--r--   0 tsievert   (502) staff       (20)      565 2023-04-07 18:02:50.000000 ga_vqc-0.0.50/ga_vqc/GA_Manager.py
+-rw-r--r--   0 tsievert   (502) staff       (20)     1019 2023-03-23 02:52:56.000000 ga_vqc-0.0.50/ga_vqc/GA_Support.py
+-rw-r--r--   0 tsievert   (502) staff       (20)     2598 2023-04-07 17:34:26.000000 ga_vqc-0.0.50/ga_vqc/Genes.py
+-rw-r--r--   0 tsievert   (502) staff       (20)      430 2023-03-23 02:52:56.000000 ga_vqc-0.0.50/ga_vqc/VQC_ABC.py
+-rw-r--r--   0 tsievert   (502) staff       (20)       69 2023-04-07 16:50:57.000000 ga_vqc-0.0.50/ga_vqc/__init__.py
+-rw-r--r--   0 tsievert   (502) staff       (20)    10808 2023-04-09 05:43:08.000000 ga_vqc-0.0.50/ga_vqc/simple_Individual.py
+-rw-r--r--   0 tsievert   (502) staff       (20)    16569 2023-04-09 06:51:39.000000 ga_vqc-0.0.50/ga_vqc/simple_Model.py
+drwxr-xr-x   0 tsievert   (502) staff       (20)        0 2023-04-09 06:53:22.862440 ga_vqc-0.0.50/ga_vqc.egg-info/
+-rw-r--r--   0 tsievert   (502) staff       (20)     1260 2023-04-09 06:53:22.000000 ga_vqc-0.0.50/ga_vqc.egg-info/PKG-INFO
+-rw-r--r--   0 tsievert   (502) staff       (20)      357 2023-04-09 06:53:22.000000 ga_vqc-0.0.50/ga_vqc.egg-info/SOURCES.txt
+-rw-r--r--   0 tsievert   (502) staff       (20)        1 2023-04-09 06:53:22.000000 ga_vqc-0.0.50/ga_vqc.egg-info/dependency_links.txt
+-rw-r--r--   0 tsievert   (502) staff       (20)      132 2023-04-09 06:53:22.000000 ga_vqc-0.0.50/ga_vqc.egg-info/requires.txt
+-rw-r--r--   0 tsievert   (502) staff       (20)        7 2023-04-09 06:53:22.000000 ga_vqc-0.0.50/ga_vqc.egg-info/top_level.txt
+-rw-r--r--   0 tsievert   (502) staff       (20)       38 2023-04-09 06:53:22.863379 ga_vqc-0.0.50/setup.cfg
+-rw-r--r--   0 tsievert   (502) staff       (20)     1067 2023-04-09 06:52:05.000000 ga_vqc-0.0.50/setup.py
```

### Comparing `ga_vqc-0.0.49/LICENSE` & `ga_vqc-0.0.50/LICENSE`

 * *Files identical despite different names*

### Comparing `ga_vqc-0.0.49/PKG-INFO` & `ga_vqc-0.0.50/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ga_vqc
-Version: 0.0.49
+Version: 0.0.50
 Summary: Genetic Algorithm for VQC ansatz search.
 Home-page: https://github.com/tcoulvert/GA_Ansatz_Search
 Author: Thomas Sievert
 Author-email: 63161166+tcoulvert@users.noreply.github.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ga_vqc-0.0.49/README.md` & `ga_vqc-0.0.50/README.md`

 * *Files identical despite different names*

### Comparing `ga_vqc-0.0.49/ga_vqc/GA_Manager.py` & `ga_vqc-0.0.50/ga_vqc/GA_Manager.py`

 * *Files identical despite different names*

### Comparing `ga_vqc-0.0.49/ga_vqc/GA_Support.py` & `ga_vqc-0.0.50/ga_vqc/GA_Support.py`

 * *Files identical despite different names*

### Comparing `ga_vqc-0.0.49/ga_vqc/Genes.py` & `ga_vqc-0.0.50/ga_vqc/Genes.py`

 * *Files identical despite different names*

### Comparing `ga_vqc-0.0.49/ga_vqc/simple_Individual.py` & `ga_vqc-0.0.50/ga_vqc/simple_Individual.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import copy
 
 import numpy as np
 import pennylane as qml
+import pennylane.numpy as pnp
 
 from .GA_ABC import GA_Individual
 
 
 class Individual(GA_Individual):
     """
     Data structure for the ansatz.
@@ -21,19 +22,20 @@
 
         TODO: change params to allow for multi-param gates
         """
         self.n_qubits = n_qubits
         self.n_moments = n_moments
         self.genepool = genepool
         self.rng = np.random.default_rng(seed=rng_seed)
+        self.pennylane_rng = pnp.random.default_rng(seed=rng_seed)
 
         self.ansatz_dicts = []
         self.ansatz_qml = []
         self.ansatz_draw = []
-        self.n_params = 0
+        self.params = []
 
         self.generate()  # Should this be done automatically?
         self.convert_to_qml()
         self.draw_ansatz()
 
     def __len__(self):
         return len(self.ansatz_dicts[0])
@@ -69,49 +71,47 @@
             for qubit in qubits:
                 if self.ansatz_dicts[moment][qubit] != 0:
                     continue
                 gate = self.genepool.choice()
 
                 if gate.n_qubits == 1:
                     self.ansatz_dicts[moment][qubit] = gate.name
-                    self.n_params += gate.n_params
                     continue
                 elif gate.n_qubits == 2:
                     qubit_pairs = self.rng.permutation(
                         self.n_qubits
                     )
                     for qubit_pair in qubit_pairs:
                         if self.ansatz_dicts[moment][qubit_pair] != 0 or qubit_pair == qubit:
                             continue
 
                         direction = self.rng.permutation(["_C", "_T"])
                         self.ansatz_dicts[moment][qubit] = gate.name + direction[0] + f"-{qubit_pair}"
                         self.ansatz_dicts[moment][qubit_pair] = gate.name + direction[1] + f"-{qubit}"
-                        self.n_params += gate.n_params
                         break
 
                     if self.ansatz_dicts[moment][qubit] == 0:
                         gate = self.genepool.choice(n_qubits=1)
                         self.ansatz_dicts[moment][qubit] = gate.name
-                        self.n_params += gate.n_params
                 else:
                     raise Exception("Gates with more than 2 qubits haven't been implemented yet.")
 
     def convert_to_qml(self):
         """
         Converts the ansatz into a general format for the QML.
 
-            moment_dict example: **_C (_T) means current qubit is control (target) qubit of 2-qubit gate**
+            moment_dict example: _C (_T) means current qubit is control (target) qubit of 2-qubit gate
                 {'I': [],
                  'RX': [],
                  'RY': [],
                  'RZ': [],
                  'CNOT': []}
         """
         self.ansatz_qml = []
+        self.params = []
         for moment in range(len(self.ansatz_dicts)):
             moment_dict = {gate.name: list() for gate in self.genepool.gates}
             stored_i = []
             for qubit in range(self.n_qubits):
                 _ix = self.ansatz_dicts[moment][qubit].find("_")
                 if _ix < 0:
                     moment_dict[self.ansatz_dicts[moment][qubit]].append(qubit)
@@ -122,30 +122,46 @@
                     q_p = int(self.ansatz_dicts[moment][qubit][-1])
                     stored_i.append(q_p)
                     if _1ix == "C":
                         moment_dict[self.ansatz_dicts[moment][qubit][:_ix]].append([qubit, int(q_p)])
                     else:
                         moment_dict[self.ansatz_dicts[moment][qubit][:_ix]].append([int(q_p), qubit])
 
-            count = 0
             for gate_name in moment_dict.keys():
                 if len(moment_dict[gate_name]) == 0 or gate_name == "I":
                     continue
                 if self.genepool.n_qubits(gate_name) == 1: # Change to check n_params of gate
-                    self.ansatz_qml.append(
-                        f"qml.broadcast(qml.{gate_name}, wires={moment_dict[gate_name]}, pattern='single', " +
-                        f"parameters=params[{count}:{count + (self.genepool.n_params(gate_name) * len(moment_dict[gate_name]))}])"
-                    )
-                    count += self.genepool.n_params(gate_name) * len(moment_dict[gate_name])
-                elif self.genepool.n_qubits(gate_name) == 2:  # Assumes the 2-qubit gates have no parameters, which is not generally true
-                    self.ansatz_qml.append(
-                        f"qml.broadcast(qml.{gate_name}, wires={np.array(moment_dict[gate_name]).flatten(order='C').tolist()}, " +
-                        f"pattern={moment_dict[gate_name]})"
-                    )
-                    # change to allow for two-qubit gates with 1+ params
+                    if self.genepool.n_params(gate_name) > 0:
+                        self.ansatz_qml.append(
+                            f"qml.broadcast(qml.{gate_name}, wires={moment_dict[gate_name]}, pattern='single', " +
+                            f"parameters=params[{len(self.params)}:{len(self.params) + len(moment_dict[gate_name])}])"
+                        )
+                        for _ in range(len(moment_dict[gate_name])):
+                            # self.params.append(np.pi * self.pennylane_rng.random(size=self.genepool.n_params(gate_name), requires_grad=True))
+                            self.params.append(np.pi * self.pennylane_rng.random(size=self.genepool.n_params(gate_name)))
+                    else:
+                        self.ansatz_qml.append(
+                            f"qml.broadcast(qml.{gate_name}, wires={moment_dict[gate_name]}, pattern='single')"
+                        )
+                elif self.genepool.n_qubits(gate_name) == 2:
+                    if self.genepool.n_params(gate_name) > 0:
+                        self.ansatz_qml.append(
+                            f"qml.broadcast(qml.{gate_name}, wires={np.array(moment_dict[gate_name]).flatten(order='C').tolist()}, " +
+                            f"parameters=params[{len(self.params)}:{len(self.params) + len(moment_dict[gate_name])}])" +
+                            f"pattern={moment_dict[gate_name]})"
+                        )
+                        for _ in range(len(moment_dict[gate_name])):
+                            # self.params.append(np.pi * self.pennylane_rng.random(size=self.genepool.n_params(gate_name), requires_grad=True))
+                            self.params.append(np.pi * self.pennylane_rng.random(size=self.genepool.n_params(gate_name)))
+                    else:
+                        self.ansatz_qml.append(
+                            f"qml.broadcast(qml.{gate_name}, wires={np.array(moment_dict[gate_name]).flatten(order='C').tolist()}, " +
+                            f"pattern={moment_dict[gate_name]})"
+                        )
+        self.params = pnp.array(self.params, dtype=object, requires_grad=True)
 
     def ansatz_circuit(self, params, event=None):
         for m in self.ansatz_qml:
             exec(m)
         return qml.expval(qml.PauliZ(wires=[self.n_qubits - 1]))
 
     def draw_ansatz(self):
@@ -154,32 +170,34 @@
             qml.QNode(
                 self.ansatz_circuit,
                 qml.device("default.qubit", wires=self.n_qubits, shots=1),
             ),
             decimals=None,
             expansion_strategy="device",
             show_all_wires=True,
-        )([0.0 for _ in range(self.n_params)], event=[i for i in range(self.n_qubits)])[:-3]
+        )(self.params, event=[i for i in range(self.n_qubits)])[:-3]
         indices = [i for i, c in enumerate(full_ansatz_draw) if c == ":"]
         for _ in range(self.n_qubits):
             self.ansatz_draw.append(full_ansatz_draw[: indices[1] - 2][3:-2])
             full_ansatz_draw = full_ansatz_draw[indices[1] - 1 :]
 
-    def add_moment(self, method='random'):
+    def add_moment(self, method='random', **kwargs):
         """
         TODO: change to randomly generate new moment?
         """
         moment = self.rng.integers(self.n_moments)
 
         if method == 'random':
-            pass
+            raise Exception("Method not yet supported.")
         elif method == 'duplicate':
             self.ansatz_dicts.append(copy.deepcopy(self.ansatz_dicts[moment]))
         elif method == 'pad':
-            pass
+            for _ in range(kwargs['num_pad']):
+                self.ansatz_dicts.append(dict.fromkeys(range(self.n_qubits), 'I'))
+                self.n_moments += 1
         else:
             raise Exception("Method not supported.")
         
         self.n_moments += 1
 
     def mutate(self, moment, qubit):
         """
```

### Comparing `ga_vqc-0.0.49/ga_vqc/simple_Model.py` & `ga_vqc-0.0.50/ga_vqc/simple_Model.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 import time
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pennylane as qml
 
-from .Distance import euclidian_distances, tsne
+from .Distance import euclidean_distances, tsne
 from .GA_ABC import GA_Model
 from .GA_Support import make_results_json
 from .simple_Individual import Individual
 
 
 class Model(GA_Model):
     """
@@ -111,42 +111,42 @@
         exec_time = end_time - start_time
         print(f"Initial generation/selection in {exec_time:.2f} seconds")
 
     def evolve(self):
         """
         Evolves the GA.
         """
-        step = 0
+        gen = 0
         while True:
-            print(f"GA iteration {step}")
+            print(f"GA iteration {gen}")
             self.fitness_arr = [0 for i in self.population]
-            self.evaluate_fitness(step)
+            self.evaluate_fitness(gen)
 
-            results = self.make_results()
+            results = self.make_results(gen)
 
             parents = self.select()
             self.mate(parents)
             self.immigrate()
-            self.check_max_moments()
+            # self.check_max_moments()
 
             print(
                 f"Best fitness: {self.best_perf['fitness']}, " + 
                 f"Best metrics: {self.best_perf['eval_metrics']}, " +
                 f"Best ansatz: {self.best_perf['ansatz_dicts']}"
             )
 
-            if step > 20:
-                if (step - self.best_perf["generation"]) > self.n_steps_patience:
+            if gen > 20:
+                if (gen - self.best_perf["generation"]) > self.n_steps_patience:
                     break
-            make_results_json(results, self.start_time, self.ga_output_path, step)
-            step += 1
+            make_results_json(results, self.start_time, self.ga_output_path, gen)
+            gen += 1
         print(
             "filename is: ",
             make_results_json(
-                results, self.start_time, self.ga_output_path, step, final_flag=True
+                results, self.start_time, self.ga_output_path, gen, final_flag=True
             ),
         )
 
     def evaluate_fitness(self, gen):
         """
         Evaluates the fitness level of all ansatz. Runs the QML optimization task.
 
@@ -157,15 +157,15 @@
         args_arr = []
         for ansatz in self.population:
             ansatz.convert_to_qml()
             ansatz.draw_ansatz()
             vqc_config_ansatz = {key: value for key, value in self.vqc_config.items()}
             vqc_config_ansatz["ansatz_dicts"] = ansatz.ansatz_dicts
             vqc_config_ansatz["ansatz_qml"] = ansatz.ansatz_qml
-            vqc_config_ansatz["n_params"] = ansatz.n_params
+            vqc_config_ansatz["params"] = ansatz.params
             vqc_config_ansatz["ix"] = ix
             vqc_config_ansatz["gen"] = gen
             args_arr.append(copy.deepcopy(vqc_config_ansatz))
             ix += 1
 
         start_time = time.time()
         output_arr = []
@@ -199,43 +199,51 @@
             )
             self.best_perf["ansatz_draw"] = copy.deepcopy(
                 self.population[np.argmax(self.fitness_arr)].ansatz_draw
             )
             self.best_perf["generation"] = gen
             self.best_perf["index"] = np.argmax(self.fitness_arr).item()
 
-    def make_results(self):
-
-        distances_from_best = euclidian_distances(self.best_perf["ansatz_dicts"], self.population)
+    def make_results(self, gen):
+        ### Euclidean distances ###
+        distances_from_best = euclidean_distances(self.population[np.argmax(self.fitness_arr)], self.population)
         destdir_curves = os.path.join(self.ga_output_path, "ga_curves")
         if not os.path.exists(destdir_curves):
             os.makedirs(destdir_curves)
         filepath_euclid = os.path.join(
             destdir_curves,
-            "%03deuclid_distance-%d_data.png"
-            % (self.best_perf["generation"], self.start_time),
+            "%03deuclid_distance-%s_data.png"
+            % (gen, self.start_time),
         )
         plt.figure(0)
         plt.style.use("seaborn")
-        plt.scatter(distances_from_best, self.fitness_arr, marker=".", color="g")
-        plt.ylabel("Fitness")
+        plt.scatter(distances_from_best, [i["auroc"] for i in self.metrics_arr], marker=".", color="g")
+        plt.ylabel("AUROC")
         plt.xlabel("Euclidian distance from best ansatz")
+        plt.title("Euclidean Distances from Best Performing Ansatz")
         plt.savefig(filepath_euclid, format="png")
-        # data_tsne = tsne(self.population)
-        # filepath_tsne = os.path.join(
-        #     destdir_curves,
-        #     "%03dtsne_distance-%d_data.png"
-        #     % (self.best_perf["generation"], self.start_time),
-        # )
-        # plt.figure(0)
-        # plt.style.use("seaborn")
-        # plt.scatter([i[0] for i in data_tsne.T], [i[1] for i in data_tsne.T], marker=".", cmap=)
-        # plt.ylabel("a.u.")
-        # plt.xlabel("a.u.")
-        # plt.savefig(filepath_tsne, format="png")
+        plt.close(0)
+        ### tSNE clustering ###
+        data_tsne = tsne(self.population, rng_seed=self.rng_seed, perplexity=2)
+        x, y = data_tsne[0], data_tsne[1]
+        filepath_tsne = os.path.join(
+            destdir_curves,
+            "%03dtsne_distance-%s_data.png"
+            % (gen, self.start_time),
+        )
+        plt.figure(0)
+        plt.style.use("seaborn")
+        plt.scatter(x, y, marker=".", c=[i["auroc"] for i in self.metrics_arr], cmap=plt.set_cmap('plasma'))
+        plt.ylabel("a.u.")
+        plt.xlabel("a.u.")
+        cbar = plt.colorbar()
+        cbar.set_label("AUROC")
+        plt.title("tSNE of Current Population")
+        plt.savefig(filepath_tsne, format="png")
+        plt.close(1)
 
         results = {
             "full_population": [i.ansatz_dicts for i in self.population],
             "full_drawn_population": [i.ansatz_draw for i in self.population],
             "full_fitness": self.fitness_arr,
             "fitness_stats": f"Avg fitness: {np.mean(self.fitness_arr)}, Std. Dev: {np.std(self.fitness_arr)}",
             "full_eval_metrics": self.metrics_arr,
@@ -288,15 +296,15 @@
                 if i % 2 != 0:
                     continue
                 swap_ixs.append(
                     [(j * self.n_winners) + i, (j * self.n_winners) + i + 1]
                 )
 
         # Perform the swap with neighboring parents
-        swap_set = set()
+        # swap_set = set()
         for swap_ix in swap_ixs:  # set up for odd number of parents
             children = [copy.deepcopy(parents[swap_ix[0]]), copy.deepcopy(parents[swap_ix[1]])]
             moment_A = self.rng.integers(children[0].n_moments) 
             moment_B = self.rng.integers(children[1].n_moments)
             # children = {
             #     "child_A": copy.deepcopy(parents[swap_ix[0]]), 
             #     "child_B": copy.deepcopy(parents[swap_ix[1]])
@@ -398,15 +406,16 @@
         """
         Adds in new individuals with every generation, in order to keep up the overall population diversity.
         """
         for _ in range(self.n_new_individuals):
             self.population.append(
                 Individual(
                     self.n_qubits,
-                    self.rng.integers(1, self.max_moments + 1),
+                    # self.rng.integers(1, self.max_moments + 1),
+                    self.max_moments,
                     self.genepool,
                     self.rng_seed,
                 )
             )
 
     def check_max_moments(self):
         """
```

### Comparing `ga_vqc-0.0.49/ga_vqc.egg-info/PKG-INFO` & `ga_vqc-0.0.50/ga_vqc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ga-vqc
-Version: 0.0.49
+Version: 0.0.50
 Summary: Genetic Algorithm for VQC ansatz search.
 Home-page: https://github.com/tcoulvert/GA_Ansatz_Search
 Author: Thomas Sievert
 Author-email: 63161166+tcoulvert@users.noreply.github.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ga_vqc-0.0.49/setup.py` & `ga_vqc-0.0.50/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="ga_vqc",
-    version="0.0.49",
+    version="0.0.50",
     description="Genetic Algorithm for VQC ansatz search.",
     packages=find_packages(include=["ga_vqc"]),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
```

