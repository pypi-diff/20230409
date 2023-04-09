# Comparing `tmp/pref_voting-0.2.3.tar.gz` & `tmp/pref_voting-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pref_voting-0.2.3.tar", max compression
+gzip compressed data, was "pref_voting-0.2.4.tar", max compression
```

## Comparing `pref_voting-0.2.3.tar` & `pref_voting-0.2.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1068 2022-07-08 15:47:57.000000 pref_voting-0.2.3/LICENSE
--rw-r--r--   0        0        0     2502 2023-04-03 00:52:09.950892 pref_voting-0.2.3/README.md
--rw-r--r--   0        0        0       22 2023-04-03 00:51:39.263536 pref_voting-0.2.3/pref_voting/__init__.py
--rw-r--r--   0        0        0     6950 2023-01-11 11:10:50.000000 pref_voting-0.2.3/pref_voting/analysis.py
--rw-r--r--   0        0        0      617 2023-03-19 17:14:54.163308 pref_voting-0.2.3/pref_voting/axioms.py
--rw-r--r--   0        0        0    23041 2023-01-11 11:10:14.000000 pref_voting-0.2.3/pref_voting/c1_methods.py
--rw-r--r--   0        0        0     8564 2023-02-15 17:29:01.299008 pref_voting-0.2.3/pref_voting/combined_methods.py
--rw-r--r--   0        0        0    19427 2022-08-09 10:32:23.000000 pref_voting-0.2.3/pref_voting/generate_profiles.py
--rw-r--r--   0        0        0    10484 2023-01-11 11:10:14.000000 pref_voting-0.2.3/pref_voting/generate_weighted_majority_graphs.py
--rw-r--r--   0        0        0     1806 2022-08-08 19:08:16.000000 pref_voting-0.2.3/pref_voting/helper.py
--rw-r--r--   0        0        0    73235 2023-04-03 00:50:48.493987 pref_voting-0.2.3/pref_voting/iterative_methods.py
--rw-r--r--   0        0        0    20246 2022-07-12 12:12:35.000000 pref_voting-0.2.3/pref_voting/maj_graph_ex1.png
--rw-r--r--   0        0        0    57869 2022-12-27 22:07:30.000000 pref_voting-0.2.3/pref_voting/margin_based_methods.py
--rw-r--r--   0        0        0    22655 2023-01-11 11:10:11.000000 pref_voting-0.2.3/pref_voting/other_methods.py
--rw-r--r--   0        0        0     9527 2022-07-08 18:36:14.000000 pref_voting-0.2.3/pref_voting/pr_voting_methods.py
--rw-r--r--   0        0        0    26712 2023-02-15 16:01:48.269224 pref_voting-0.2.3/pref_voting/profiles.py
--rw-r--r--   0        0        0    34045 2023-03-19 16:14:32.871530 pref_voting-0.2.3/pref_voting/profiles_with_ties.py
--rw-r--r--   0        0        0    11064 2023-03-12 17:38:09.515720 pref_voting-0.2.3/pref_voting/scoring_methods.py
--rw-r--r--   0        0        0     5381 2023-02-15 15:31:23.315651 pref_voting-0.2.3/pref_voting/voting_method.py
--rw-r--r--   0        0        0      253 2022-07-31 21:02:46.000000 pref_voting-0.2.3/pref_voting/voting_methods.py
--rw-r--r--   0        0        0    48830 2023-01-09 01:33:03.000000 pref_voting-0.2.3/pref_voting/weighted_majority_graphs.py
--rw-r--r--   0        0        0      715 2023-04-03 00:51:20.660197 pref_voting-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     3474 1970-01-01 00:00:00.000000 pref_voting-0.2.3/setup.py
--rw-r--r--   0        0        0     3596 1970-01-01 00:00:00.000000 pref_voting-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1068 2022-07-08 15:47:57.000000 pref_voting-0.2.4/LICENSE
+-rw-r--r--   0        0        0     2605 2023-04-09 19:41:59.470121 pref_voting-0.2.4/README.md
+-rw-r--r--   0        0        0       22 2023-04-09 19:41:57.461372 pref_voting-0.2.4/pref_voting/__init__.py
+-rw-r--r--   0        0        0     6950 2023-01-11 11:10:50.000000 pref_voting-0.2.4/pref_voting/analysis.py
+-rw-r--r--   0        0        0      617 2023-03-19 17:14:54.163308 pref_voting-0.2.4/pref_voting/axioms.py
+-rw-r--r--   0        0        0    23041 2023-01-11 11:10:14.000000 pref_voting-0.2.4/pref_voting/c1_methods.py
+-rw-r--r--   0        0        0     8564 2023-02-15 17:29:01.299008 pref_voting-0.2.4/pref_voting/combined_methods.py
+-rw-r--r--   0        0        0    20644 2023-04-09 19:35:14.204698 pref_voting-0.2.4/pref_voting/generate_profiles.py
+-rw-r--r--   0        0        0    10484 2023-01-11 11:10:14.000000 pref_voting-0.2.4/pref_voting/generate_weighted_majority_graphs.py
+-rw-r--r--   0        0        0     1806 2022-08-08 19:08:16.000000 pref_voting-0.2.4/pref_voting/helper.py
+-rw-r--r--   0        0        0    73235 2023-04-03 00:50:48.493987 pref_voting-0.2.4/pref_voting/iterative_methods.py
+-rw-r--r--   0        0        0    20246 2022-07-12 12:12:35.000000 pref_voting-0.2.4/pref_voting/maj_graph_ex1.png
+-rw-r--r--   0        0        0    57869 2022-12-27 22:07:30.000000 pref_voting-0.2.4/pref_voting/margin_based_methods.py
+-rw-r--r--   0        0        0    25682 2023-04-03 23:28:48.128269 pref_voting-0.2.4/pref_voting/other_methods.py
+-rw-r--r--   0        0        0     9527 2022-07-08 18:36:14.000000 pref_voting-0.2.4/pref_voting/pr_voting_methods.py
+-rw-r--r--   0        0        0    26712 2023-02-15 16:01:48.269224 pref_voting-0.2.4/pref_voting/profiles.py
+-rw-r--r--   0        0        0    34045 2023-03-19 16:14:32.871530 pref_voting-0.2.4/pref_voting/profiles_with_ties.py
+-rw-r--r--   0        0        0    11064 2023-03-12 17:38:09.515720 pref_voting-0.2.4/pref_voting/scoring_methods.py
+-rw-r--r--   0        0        0     5381 2023-02-15 15:31:23.315651 pref_voting-0.2.4/pref_voting/voting_method.py
+-rw-r--r--   0        0        0      253 2022-07-31 21:02:46.000000 pref_voting-0.2.4/pref_voting/voting_methods.py
+-rw-r--r--   0        0        0    48830 2023-01-09 01:33:03.000000 pref_voting-0.2.4/pref_voting/weighted_majority_graphs.py
+-rw-r--r--   0        0        0      715 2023-04-09 19:40:36.986854 pref_voting-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     3578 1970-01-01 00:00:00.000000 pref_voting-0.2.4/setup.py
+-rw-r--r--   0        0        0     3699 1970-01-01 00:00:00.000000 pref_voting-0.2.4/PKG-INFO
```

### Comparing `pref_voting-0.2.3/LICENSE` & `pref_voting-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.3/README.md` & `pref_voting-0.2.4/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 - v0.1.14 (2022-12-19): Add plurality_scores to ProfileWithTies; add generate ceots function; bug fixes 
 - v0.1.23 (2022-12-27): Add instant_runoff_for_truncated_linear_orders and functions to truncate overvotes in a ProfileWithTies, add smith_irv_put, document analysis functions
 - v0.1.25 (2023-1-11): Add condorcet_irv, condorcet_irv_put; Update documentation; add axioms.py; add display and equality to Ranking class; fix enumerate ceots functions
 - v0.1.27 (2023-2-07): Add Borda for ProfileWithTies
 - v0.2 (2023-2-15): Add Benham, add anonymize to Profile method, comment out numba to make compatible with Python 3.11, add add_unranked_candidates to ProfileWithTies
 - v0.2.1 (2023-2-15): Bug fixes
 - v0.2.3 (2023-4-2): Add plurality_with_runoff_with_explanation
+- v0.2.4 (2023-4-9): Update generate_truncated_profile so that it implements and IC probability model.
 
 ## Questions?
 
 Feel free to [send me an email](https://pacuit.org/) if you have questions about the project.
 
 ## License
```

### Comparing `pref_voting-0.2.3/pref_voting/analysis.py` & `pref_voting-0.2.4/pref_voting/analysis.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.3/pref_voting/axioms.py` & `pref_voting-0.2.4/pref_voting/axioms.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.3/pref_voting/c1_methods.py` & `pref_voting-0.2.4/pref_voting/c1_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.3/pref_voting/combined_methods.py` & `pref_voting-0.2.4/pref_voting/combined_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.3/pref_voting/generate_profiles.py` & `pref_voting-0.2.4/pref_voting/generate_profiles.py`

 * *Files 4% similar despite different names*

```diff
@@ -474,22 +474,23 @@
         return
     for k in range(1, len(A) + 1):
         for B in combinations(A, k):  # i.e., all nonempty subsets B
             for order in strict_weak_orders(set(A) - set(B)):
                 yield [B] + order
 
 
-def generate_truncated_profile(num_cands, num_voters, max_num_ranked=3):
+def generate_truncated_profile(num_cands, num_voters, max_num_ranked=3,probmod="IC"):
     """Generate a :class:`ProfileWithTies` with ``num_cands`` candidates and ``num_voters``.  
     `The ballots will be truncated linear orders of the candidates.
 
     Args:
         num_cands (int): The number of candidates to include in the profile. 
         num_voters (int): The number of voters to include in the profile.
-        max_num_ranked (int, default=3): The maximum level to truncate the linear ranking. Each generated ranking will be truncated at a level that is randomly chosen between 1 and max_num_ranked 
+        max_num_ranked (int, default=3): The maximum level to truncate the linear ranking. 
+        probmod (str): optional (default "IC")
 
     Returns: 
         ProfileWithTies 
 
     :Example:
 
         .. exec_code::
@@ -497,24 +498,47 @@
             from pref_voting.generate_profiles import generate_truncated_profile
 
             prof = generate_truncated_profile(6, 7)
             prof.display()
 
             prof = generate_truncated_profile(6, 7, max_num_ranked=6)
             prof.display()
+
+    :Possible Values of probmod:
+    
+    - "IC" (Impartial Culture): each randomly generated linear order of all candidates is truncated at a level from 1 to max_num_ranked, where the probability of truncating at level t is the number of truncated linear orders of length t divided by the number of truncated linear orders of length from 1 to max_num_ranked. Then a voter is equally likely to get any of the truncated linear orders of length from 1 to max_num_ranked.
+    - "RT" (Random Truncation): each randomly generated linear order of all candidates is truncated at a level that is randomly chosen from 1 to max_num_ranked.
         
     """
     
     if max_num_ranked > num_cands:
         max_num_ranked = num_cands
+
+    if probmod == "IC":
+        num_rankings_of_length = dict()
+
+        for n in range(1, max_num_ranked + 1):
+            num_rankings_of_length[n] = 1
+            for i in range(num_cands,num_cands-n, -1):
+                num_rankings_of_length[n] *= i
+
+        num_all_rankings = sum([num_rankings_of_length[n] for n in range(1, max_num_ranked + 1)])
+        probabilities = [num_rankings_of_length[n] / num_all_rankings for n in range(1, max_num_ranked + 1)]
+
     lprof = generate_profile(num_cands, num_voters)
     
     rmaps = list()
     for r in lprof.rankings:
-        truncate_at = random.choice(range(1, max_num_ranked + 1))
+
+        if probmod == "RT":
+            truncate_at = random.choice(range(1, max_num_ranked + 1))
+
+        if probmod == "IC":
+            truncate_at = random.choices(range(1, max_num_ranked + 1), weights=probabilities, k=1)[0]
+
         truncated_r = r[0:truncate_at]
 
         rmap = {c: _r + 1 for _r, c in enumerate(truncated_r)}
 
         rmaps.append(rmap)
 
     return ProfileWithTies(
```

### Comparing `pref_voting-0.2.3/pref_voting/generate_weighted_majority_graphs.py` & `pref_voting-0.2.4/pref_voting/generate_weighted_majority_graphs.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.3/pref_voting/helper.py` & `pref_voting-0.2.4/pref_voting/helper.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.3/pref_voting/iterative_methods.py` & `pref_voting-0.2.4/pref_voting/iterative_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.3/pref_voting/maj_graph_ex1.png` & `pref_voting-0.2.4/pref_voting/maj_graph_ex1.png`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.3/pref_voting/margin_based_methods.py` & `pref_voting-0.2.4/pref_voting/margin_based_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.3/pref_voting/other_methods.py` & `pref_voting-0.2.4/pref_voting/other_methods.py`

 * *Files 5% similar despite different names*

```diff
@@ -626,16 +626,71 @@
                        for c in candidates}
         if any([s >= strict_maj_size for s in cand_scores.values()]):
             break
             
     return sorted([c for c in candidates if cand_scores[c] >= strict_maj_size]), cand_scores
 
 
+@vm(name = "Weighted Bucklin")
+def weighted_bucklin(profile, curr_cands = None, strict_threshold = False, score = lambda num_cands, rank: (num_cands - rank)/ (num_cands - 1) if num_cands > 1 else 1): 
+    """The Weighted Bucklin procedure, studied by D. Marc Kilgour, Jean-Charles Grégoire, and Angèle Foley. The k-th Weighted Bucklin score of a candidate c is the sum for j \leq k of the product of score(num_cands,j) and the number of voters who rank c in j-th place. Compute higher-order Weighted Bucklin scores until reaching a k such that some candidate's k-th Weighted Bucklin score is at least half the number of voters (or the strict majority size if strict_threshold = True). Then return the candidates with maximal k-th Weighted Bucklin score. Bucklin is the special case where strict_threshold = True and score = lambda num_cands, rank: 1.
+    
+    Args:
+        profile (Profile): An anonymous profile of linear orders on a set of candidates
+        curr_cands (List[int], optional): If set, then find the winners for the profile restrcited to the candidates in ``curr_cands``
+        strict_threshold: If True, makes the threshold for the Bucklin procedure the strict majority size; otherwise threshold is half the number of voters, following Kilgour et al.
+        score (function): A function that accepts two parameters ``num_cands`` (the number of candidates) and ``rank`` (a rank of a candidate) used to calculate the score of a candidate. The default ``score`` function is the normalized version of the classic Borda score vector.
+
+    Returns: 
+        A sorted list of candidates
+
+    :Example: 
+
+    .. exec_code:: 
+
+        from pref_voting.profiles import Profile
+        from pref_voting.other_methods import weighted_bucklin
+
+        prof = Profile([[1, 0, 2], [0, 2, 1], [0, 1, 2]], [2, 1, 1])
+
+        prof.display()
+        weighted_bucklin.display(prof)
+
+    """
+    if strict_threshold == True:
+        threshold = profile.strict_maj_size()
+    else:
+        threshold = profile.num_voters / 2
+
+    candidates = profile.candidates if curr_cands is None else curr_cands
+    
+    num_cands = candidates
+    
+    rankings = profile._rankings if curr_cands is None else _find_updated_profile(profile._rankings, np.array([c for c in profile.candidates if c not in curr_cands]), profile.num_cands)
+
+    rcounts = profile._rcounts
+    
+    num_cands = len(candidates)
+    ranks = range(1, num_cands + 1)
+    
+    cand_to_num_voters_rank = dict()
+    for r in ranks:
+        cand_to_num_voters_rank[r] = {c: _num_rank(rankings, rcounts, c, r)
+                                      for c in candidates}
+        cand_scores = {c:sum([score(len(candidates), _r) * cand_to_num_voters_rank[_r][c] for _r in cand_to_num_voters_rank.keys()]) 
+                       for c in candidates}
+        if any([s >= threshold for s in cand_scores.values()]):
+            break
+    max_score = max(cand_scores.values())
+
+    return sorted([c for c in candidates if cand_scores[c] >= max_score])
+
 
 other_vms = [
     banks,
     slater,
     kemmeny_young, 
     majority, 
     bucklin,
-    simplified_bucklin
+    simplified_bucklin,
+    weighted_bucklin
 ]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pref_voting-0.2.3/pref_voting/pr_voting_methods.py` & `pref_voting-0.2.4/pref_voting/pr_voting_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.3/pref_voting/profiles.py` & `pref_voting-0.2.4/pref_voting/profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.3/pref_voting/profiles_with_ties.py` & `pref_voting-0.2.4/pref_voting/profiles_with_ties.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.3/pref_voting/scoring_methods.py` & `pref_voting-0.2.4/pref_voting/scoring_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.3/pref_voting/voting_method.py` & `pref_voting-0.2.4/pref_voting/voting_method.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.3/pref_voting/weighted_majority_graphs.py` & `pref_voting-0.2.4/pref_voting/weighted_majority_graphs.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.3/pyproject.toml` & `pref_voting-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "pref_voting"
-version = "0.2.3"
+version = "0.2.4"
 description = "pref_voting is a Python packaging that contains tools to reason about election profiles and margin graphs, and implementations of a variety of preferential voting methods."
 authors = ["Eric Pacuit <epacuit@umd.edu>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/voting-tools/pref_voting"
 repository = "https://github.com/voting-tools/pref_voting"
```

### Comparing `pref_voting-0.2.3/setup.py` & `pref_voting-0.2.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,17 +12,17 @@
  'networkx>=3.0,<4.0',
  'random2>=1.0.1,<2.0.0',
  'scipy>=1.0.0,<2.0.0',
  'tabulate>=0.9.0,<0.10.0']
 
 setup_kwargs = {
     'name': 'pref-voting',
-    'version': '0.2.3',
+    'version': '0.2.4',
     'description': 'pref_voting is a Python packaging that contains tools to reason about election profiles and margin graphs, and implementations of a variety of preferential voting methods.',
-    'long_description': 'pref_voting\n==========\n\n## Installation\n\nWith pip package manager:\n\n```bash\npip install pref_voting\n```\n## Documentation\n\nOnline documentation is available at [https://pref_voting.readthedocs.io](https://pref_voting.readthedocs.io).\n\n## Profiles and Voting Methods\n\nA profile (of linear orders over the candidates) is created by initializing a Profile class object.  This needs a list of rankings (each ranking is a tuple of numbers), the number of candidates, and a list giving the number of each ranking in the profile:\n\n```python\nfrom pref_voting.profiles import Profile\n\nrankings = [(0, 1, 2, 3), (2, 3, 1, 0), (3, 1, 2, 0), (1, 2, 0, 3), (1, 3, 2, 0)]\nrcounts = [5, 3, 2, 4, 3]\n\nprof = Profile(rankings, rcounts=rcounts)\n```\n\nThe function generate_profile is used to generate a profile for a given number of candidates and voters:  \n```python\nfrom pref_voting.generate_profiles import generate_profile\n\n# generate a profile using the Impartial Culture probability model\nprof = generate_profile(3, 4) # prof is a Profile object\n\n# generate a profile using the Impartial Anonymous Culture probability model\nprof = generate_profile(3, 4, probmod = "IAC") # prof is a Profile object \n```\n\n```python\nfrom pref_voting.profiles import Profile\nfrom pref_voting.voting_methods import *\n\nprof = Profile(rankings, num_cands, rcounts=rcounts)\nprint(f"{split_cycle.name} winners:  {split_cycle(prof)}")\nsplit_cycle.display(prof)\n\n```\n\n## Versions\n\n- v0.1.10 (2022-08-09): **Initial release** \n- v0.1.13 (2022-11-05): Minor updates and bug fixes \n- v0.1.14 (2022-12-19): Add plurality_scores to ProfileWithTies; add generate ceots function; bug fixes \n- v0.1.23 (2022-12-27): Add instant_runoff_for_truncated_linear_orders and functions to truncate overvotes in a ProfileWithTies, add smith_irv_put, document analysis functions\n- v0.1.25 (2023-1-11): Add condorcet_irv, condorcet_irv_put; Update documentation; add axioms.py; add display and equality to Ranking class; fix enumerate ceots functions\n- v0.1.27 (2023-2-07): Add Borda for ProfileWithTies\n- v0.2 (2023-2-15): Add Benham, add anonymize to Profile method, comment out numba to make compatible with Python 3.11, add add_unranked_candidates to ProfileWithTies\n- v0.2.1 (2023-2-15): Bug fixes\n- v0.2.3 (2023-4-2): Add plurality_with_runoff_with_explanation\n\n## Questions?\n\nFeel free to [send me an email](https://pacuit.org/) if you have questions about the project.\n\n## License\n\n[MIT](https://github.com/jontingvold/pyrankvote/blob/master/LICENSE.txt)\n',
+    'long_description': 'pref_voting\n==========\n\n## Installation\n\nWith pip package manager:\n\n```bash\npip install pref_voting\n```\n## Documentation\n\nOnline documentation is available at [https://pref_voting.readthedocs.io](https://pref_voting.readthedocs.io).\n\n## Profiles and Voting Methods\n\nA profile (of linear orders over the candidates) is created by initializing a Profile class object.  This needs a list of rankings (each ranking is a tuple of numbers), the number of candidates, and a list giving the number of each ranking in the profile:\n\n```python\nfrom pref_voting.profiles import Profile\n\nrankings = [(0, 1, 2, 3), (2, 3, 1, 0), (3, 1, 2, 0), (1, 2, 0, 3), (1, 3, 2, 0)]\nrcounts = [5, 3, 2, 4, 3]\n\nprof = Profile(rankings, rcounts=rcounts)\n```\n\nThe function generate_profile is used to generate a profile for a given number of candidates and voters:  \n```python\nfrom pref_voting.generate_profiles import generate_profile\n\n# generate a profile using the Impartial Culture probability model\nprof = generate_profile(3, 4) # prof is a Profile object\n\n# generate a profile using the Impartial Anonymous Culture probability model\nprof = generate_profile(3, 4, probmod = "IAC") # prof is a Profile object \n```\n\n```python\nfrom pref_voting.profiles import Profile\nfrom pref_voting.voting_methods import *\n\nprof = Profile(rankings, num_cands, rcounts=rcounts)\nprint(f"{split_cycle.name} winners:  {split_cycle(prof)}")\nsplit_cycle.display(prof)\n\n```\n\n## Versions\n\n- v0.1.10 (2022-08-09): **Initial release** \n- v0.1.13 (2022-11-05): Minor updates and bug fixes \n- v0.1.14 (2022-12-19): Add plurality_scores to ProfileWithTies; add generate ceots function; bug fixes \n- v0.1.23 (2022-12-27): Add instant_runoff_for_truncated_linear_orders and functions to truncate overvotes in a ProfileWithTies, add smith_irv_put, document analysis functions\n- v0.1.25 (2023-1-11): Add condorcet_irv, condorcet_irv_put; Update documentation; add axioms.py; add display and equality to Ranking class; fix enumerate ceots functions\n- v0.1.27 (2023-2-07): Add Borda for ProfileWithTies\n- v0.2 (2023-2-15): Add Benham, add anonymize to Profile method, comment out numba to make compatible with Python 3.11, add add_unranked_candidates to ProfileWithTies\n- v0.2.1 (2023-2-15): Bug fixes\n- v0.2.3 (2023-4-2): Add plurality_with_runoff_with_explanation\n- v0.2.4 (2023-4-9): Update generate_truncated_profile so that it implements and IC probability model.\n\n## Questions?\n\nFeel free to [send me an email](https://pacuit.org/) if you have questions about the project.\n\n## License\n\n[MIT](https://github.com/jontingvold/pyrankvote/blob/master/LICENSE.txt)\n',
     'author': 'Eric Pacuit',
     'author_email': 'epacuit@umd.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/voting-tools/pref_voting',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `pref_voting-0.2.3/PKG-INFO` & `pref_voting-0.2.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pref-voting
-Version: 0.2.3
+Version: 0.2.4
 Summary: pref_voting is a Python packaging that contains tools to reason about election profiles and margin graphs, and implementations of a variety of preferential voting methods.
 Home-page: https://github.com/voting-tools/pref_voting
 License: MIT
 Author: Eric Pacuit
 Author-email: epacuit@umd.edu
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -78,14 +78,15 @@
 - v0.1.14 (2022-12-19): Add plurality_scores to ProfileWithTies; add generate ceots function; bug fixes 
 - v0.1.23 (2022-12-27): Add instant_runoff_for_truncated_linear_orders and functions to truncate overvotes in a ProfileWithTies, add smith_irv_put, document analysis functions
 - v0.1.25 (2023-1-11): Add condorcet_irv, condorcet_irv_put; Update documentation; add axioms.py; add display and equality to Ranking class; fix enumerate ceots functions
 - v0.1.27 (2023-2-07): Add Borda for ProfileWithTies
 - v0.2 (2023-2-15): Add Benham, add anonymize to Profile method, comment out numba to make compatible with Python 3.11, add add_unranked_candidates to ProfileWithTies
 - v0.2.1 (2023-2-15): Bug fixes
 - v0.2.3 (2023-4-2): Add plurality_with_runoff_with_explanation
+- v0.2.4 (2023-4-9): Update generate_truncated_profile so that it implements and IC probability model.
 
 ## Questions?
 
 Feel free to [send me an email](https://pacuit.org/) if you have questions about the project.
 
 ## License
```

