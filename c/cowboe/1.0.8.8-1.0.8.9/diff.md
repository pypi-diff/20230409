# Comparing `tmp/cowboe-1.0.8.8.tar.gz` & `tmp/cowboe-1.0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cowboe-1.0.8.8.tar", last modified: Tue Mar 14 23:48:25 2023, max compression
+gzip compressed data, was "cowboe-1.0.8.9.tar", last modified: Sun Apr  9 15:09:52 2023, max compression
```

## Comparing `cowboe-1.0.8.8.tar` & `cowboe-1.0.8.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 naveen    (1000) naveen    (1000)        0 2023-03-14 23:48:25.698166 cowboe-1.0.8.8/
--rw-rw-r--   0 naveen    (1000) naveen    (1000)    35149 2021-04-01 01:51:25.000000 cowboe-1.0.8.8/LICENSE.txt
--rw-rw-r--   0 naveen    (1000) naveen    (1000)     8690 2023-03-14 23:48:25.698166 cowboe-1.0.8.8/PKG-INFO
--rw-rw-r--   0 naveen    (1000) naveen    (1000)     7690 2022-07-22 06:49:06.000000 cowboe-1.0.8.8/README.md
-drwxrwxr-x   0 naveen    (1000) naveen    (1000)        0 2023-03-14 23:48:25.698166 cowboe-1.0.8.8/cowboe/
-drwxrwxr-x   0 naveen    (1000) naveen    (1000)        0 2023-03-14 23:48:25.698166 cowboe-1.0.8.8/cowboe/cowboe.egg-info/
--rw-rw-r--   0 naveen    (1000) naveen    (1000)     8690 2023-03-14 23:48:24.000000 cowboe-1.0.8.8/cowboe/cowboe.egg-info/PKG-INFO
--rw-rw-r--   0 naveen    (1000) naveen    (1000)      241 2023-03-14 23:48:24.000000 cowboe-1.0.8.8/cowboe/cowboe.egg-info/SOURCES.txt
--rw-rw-r--   0 naveen    (1000) naveen    (1000)        1 2023-03-14 23:48:24.000000 cowboe-1.0.8.8/cowboe/cowboe.egg-info/dependency_links.txt
--rw-rw-r--   0 naveen    (1000) naveen    (1000)       54 2023-03-14 23:48:24.000000 cowboe-1.0.8.8/cowboe/cowboe.egg-info/requires.txt
--rw-rw-r--   0 naveen    (1000) naveen    (1000)        7 2023-03-14 23:48:24.000000 cowboe-1.0.8.8/cowboe/cowboe.egg-info/top_level.txt
--rw-rw-r--   0 naveen    (1000) naveen    (1000)   156321 2023-03-14 21:57:28.000000 cowboe-1.0.8.8/cowboe/cowboe.py
--rw-rw-r--   0 naveen    (1000) naveen    (1000)       79 2023-03-14 23:48:25.718155 cowboe-1.0.8.8/setup.cfg
--rw-rw-r--   0 naveen    (1000) naveen    (1000)     2423 2022-07-22 06:48:31.000000 cowboe-1.0.8.8/setup.py
+drwxrwxr-x   0 naveen    (1000) naveen    (1000)        0 2023-04-09 15:09:52.339047 cowboe-1.0.8.9/
+-rw-rw-r--   0 naveen    (1000) naveen    (1000)    35149 2021-04-01 01:51:25.000000 cowboe-1.0.8.9/LICENSE.txt
+-rw-rw-r--   0 naveen    (1000) naveen    (1000)     8690 2023-04-09 15:09:52.339047 cowboe-1.0.8.9/PKG-INFO
+-rw-rw-r--   0 naveen    (1000) naveen    (1000)     7690 2022-07-22 06:49:06.000000 cowboe-1.0.8.9/README.md
+drwxrwxr-x   0 naveen    (1000) naveen    (1000)        0 2023-04-09 15:09:52.339047 cowboe-1.0.8.9/cowboe/
+drwxrwxr-x   0 naveen    (1000) naveen    (1000)        0 2023-04-09 15:09:52.339047 cowboe-1.0.8.9/cowboe/cowboe.egg-info/
+-rw-rw-r--   0 naveen    (1000) naveen    (1000)     8690 2023-04-09 15:09:51.000000 cowboe-1.0.8.9/cowboe/cowboe.egg-info/PKG-INFO
+-rw-rw-r--   0 naveen    (1000) naveen    (1000)      241 2023-04-09 15:09:51.000000 cowboe-1.0.8.9/cowboe/cowboe.egg-info/SOURCES.txt
+-rw-rw-r--   0 naveen    (1000) naveen    (1000)        1 2023-04-09 15:09:51.000000 cowboe-1.0.8.9/cowboe/cowboe.egg-info/dependency_links.txt
+-rw-rw-r--   0 naveen    (1000) naveen    (1000)       54 2023-04-09 15:09:51.000000 cowboe-1.0.8.9/cowboe/cowboe.egg-info/requires.txt
+-rw-rw-r--   0 naveen    (1000) naveen    (1000)        7 2023-04-09 15:09:51.000000 cowboe-1.0.8.9/cowboe/cowboe.egg-info/top_level.txt
+-rw-rw-r--   0 naveen    (1000) naveen    (1000)   158111 2023-04-09 14:02:42.000000 cowboe-1.0.8.9/cowboe/cowboe.py
+-rw-rw-r--   0 naveen    (1000) naveen    (1000)       79 2023-04-09 15:09:52.343047 cowboe-1.0.8.9/setup.cfg
+-rw-rw-r--   0 naveen    (1000) naveen    (1000)     2423 2022-07-22 06:48:31.000000 cowboe-1.0.8.9/setup.py
```

### Comparing `cowboe-1.0.8.8/LICENSE.txt` & `cowboe-1.0.8.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cowboe-1.0.8.8/PKG-INFO` & `cowboe-1.0.8.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cowboe
-Version: 1.0.8.8
+Version: 1.0.8.9
 Summary: Construction Of Windows Based On free Energy
 Home-page: https://github.com/kuroonai/cowboe
 Author: Naveen Vasudevan, Li Xi
 Author-email: naveenovan@gmail.com, xili@mcmaster.ca
 License: GNU General Public License v3.0
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `cowboe-1.0.8.8/README.md` & `cowboe-1.0.8.9/README.md`

 * *Files identical despite different names*

### Comparing `cowboe-1.0.8.8/cowboe/cowboe.egg-info/PKG-INFO` & `cowboe-1.0.8.9/cowboe/cowboe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cowboe
-Version: 1.0.8.8
+Version: 1.0.8.9
 Summary: Construction Of Windows Based On free Energy
 Home-page: https://github.com/kuroonai/cowboe
 Author: Naveen Vasudevan, Li Xi
 Author-email: naveenovan@gmail.com, xili@mcmaster.ca
 License: GNU General Public License v3.0
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `cowboe-1.0.8.8/cowboe/cowboe.py` & `cowboe-1.0.8.9/cowboe/cowboe.py`

 * *Files 1% similar despite different names*

```diff
@@ -408,14 +408,17 @@
             sf = '/project/6003277/vasudevn/OPT/equal/BENCHMARK_CONVENTIONAL'
         elif server == 'beluga' : 
             tc = 160
             sf = '/lustre04/scratch/vasudevn/OPT/equal/BENCHMARK_CONVENTIONAL'
         elif server == 'niagara': 
             tc = 160
             sf = '/gpfs/fs0/scratch/x/xili/vasudevn/OPT/equal/BENCHMARK_CONVENTIONAL'
+        elif server == 'narval':
+            tc = 160
+            sf = '/scratch/vasudevn/project/6003277/vasudevn/BENCHMARK_CONVENTIONAL'
         
         A = str(A)
         B = str(B)
         V = str(V)
         
         print("p%s_%s = {\n\
         'A'             :%s,\n\
@@ -833,18 +836,31 @@
     print('\n')
     writeinputdic(pointname,'cedar',A,B,V,windows)
     print('\n')
     writeinputdic(pointname,'beluga',A,B,V,windows)
     print('\n')
     writeinputdic(pointname,'niagara',A,B,V,windows)
     print('\n')
+    writeinputdic(pointname,'narval',A,B,V,windows)
+    print('\n')
 
-    return None
 
 
+    src_folder = f"/media/sf_OD/ACADEMICS/papers/plotfiles/{name}"
+    dst_folder = f"/media/sf_dive/Research_work/afinalpaperrun/analysis/OPT/test/algorithm/bvn/{name}"
+    
+    # Check if the destination folder already exists
+    if os.path.exists(dst_folder):
+        # If the destination folder exists, remove it
+        shutil.rmtree(dst_folder)
+    
+    # Copy the folder and its contents to the destination folder
+    shutil.copytree(src_folder, dst_folder)
+    
+    return None
 
 def cowboe(**kwargs):
     '''
     cowboe algorithm for iteration and window selection
 
     Parameters
     ----------
@@ -1713,38 +1729,47 @@
     ----------
     test : str, mandatory
         name of the pmf curve being tested ( point name used in pmftopoints() ).
     
     bench : str, mandatory
         name of the benchmarck pmf curve
         
+    frommin : bool
+        specify whether to consider error only after the minimum positions i.e. from x where pmf=0
+        
     -------
     Returns
     
     outdict  : dict
         dictionary  with all the calculated deviation information.
 
     '''
-    def clean_files(test_file, bench_file):
+    def clean_files(test_file, bench_file, fromzero):
         # Load data from files
         test_data = np.loadtxt(test_file, dtype=np.float32, delimiter='\t', comments='#')
         bench_data = np.loadtxt(bench_file, dtype=np.float32, delimiter='\t', comments='#')
         
 
         # Make sure the first column values match and are of the same length
         common_indices = np.intersect1d(test_data[:, 0], bench_data[:, 0], assume_unique=True)
         test_data = test_data[np.isin(test_data[:, 0], common_indices)]
         bench_data = bench_data[np.isin(bench_data[:, 0], common_indices)]
         
-        # Splice the files to the same length starting from the row where column 1 value is 0.000000
-        start_index_test = np.argmax(test_data[:, 1] == 0.0)
-        start_index_bench = np.argmax(bench_data[:, 1] == 0.0)
-
-        test_data = test_data[max(start_index_test,start_index_bench):]
-        bench_data = bench_data[max(start_index_test,start_index_bench):]
+        if fromzero:
+            
+            # Splice the files to the same length starting from the row where column 1 value is 0.000000
+            start_index_test = np.argmax(test_data[:, 1] == 0.0)
+            start_index_bench = np.argmax(bench_data[:, 1] == 0.0)
+    
+            test_data = test_data[max(start_index_test,start_index_bench):]
+            bench_data = bench_data[max(start_index_test,start_index_bench):]
+        
+        else : 
+            test_data = test_data[max(0,0):]
+            bench_data = bench_data[max(0,0):]
 
     
         # Remove rows with NaN or Inf values in the second column
         mask = np.isfinite(test_data[:, 1]) & np.isfinite(bench_data[:, 1])
         test_data = test_data[mask]
         bench_data = bench_data[mask]
         
@@ -1817,17 +1842,18 @@
 
         ax.legend()
 
         return max_vertical_distance, absolute_area, min(x), max(x), x[max_pos]
     
     testfile = kwargs['test']
     benchfile = kwargs['bench']
+    frommin = kwargs.get('frommin',True)
 
 
-    cleantestfile, cleanbenchfile = clean_files(testfile, benchfile)
+    cleantestfile, cleanbenchfile = clean_files(testfile, benchfile, frommin)
     
     vdist, varea, xmin, xmax,  maxpos = va(cleantestfile, cleanbenchfile)
     varea_norm = varea/(xmax-xmin)
     
     outdict = {'absolute maximum deviation' : round(vdist,4),
                'maximum position': round(maxpos,4),
                'absolute integral error': round(varea,4),
@@ -3554,50 +3580,60 @@
         
         ########################to make shell script#############################
     
         for i in range (wins):
             filename='%d.sh'%i
             sys.stdout=open(filename,'w')
             print('#!/bin/bash -l')
-            if server =="cedar" or server =="beluga" or server == 'niagara':    
+            
+            if server =="cedar" or server =="beluga" or server == 'niagara' or server == 'narval':    
                 print('#SBATCH --account=def-xili')
             else:
                 print('#SBATCH --account=rrg-xili')
-            print(('#SBATCH -N %d')%node)
-            if server != 'niagara':
-                print(('#SBATCH -n %d')%(node*corepnode))
+                
+            if server != 'narval':print(('#SBATCH -N %d')%node)
+            
+            if server != 'niagara' and server == 'narval':
+                print(('#SBATCH -n %d')%(192))
                 print(('#SBATCH --mem-per-cpu=%d')%mpc)
                 if K[i] > 100.0 :
-                    print(('#SBATCH --time=00:%d:00')%int(TIME_min[i]+60))
+                    print(('#SBATCH --time=00:%d:00')%int(((150/640000)*st_step[-1]+40)))
                 else:
-                    print(('#SBATCH --time=00:%d:00')%int(TIME_min[i]))
-                
+                    print(('#SBATCH --time=00:%d:00')%int(((150/640000)*st_step[-1]+40)))
+            
+            elif server == 'narval':
+                print(('#SBATCH -n %d')%(160))
+                print(('#SBATCH --mem-per-cpu=%s')%('1G'))
             else:
                 print(('#SBATCH --ntasks=%d')%(node*corepnode))
-                if TIME_min[i] <= 24*60 and K[i] > 100.0 : print('#SBATCH --time=00:{}:00'.format(TIME_min[i]+60))
-                elif TIME_min[i] <= 24*60 and K[i] < 100.0 : print('#SBATCH --time=00:{}:00'.format(TIME_min[i]))
+                if TIME_min[i] <= 24*60 and K[i] > 100.0 : print('#SBATCH --time=00:{}:00 #'.format(TIME_min[i]+60+20))
+                elif TIME_min[i] <= 24*60 and K[i] < 100.0 : print('#SBATCH --time=00:{}:00 #'.format(TIME_min[i]+20))
                 else : print(('#SBATCH --time=23:59:59'))
                 
             if mail=='TRUE':
                 print('#SBATCH --mail-type=ALL')
                 print('#SBATCH --mail-user=vasudevnhpcjobs@gmail.com')
             
             
             print(('#SBATCH -J {}-win-{}').format(subloc.split('/')[-1],i))
             
             if server=="beluga":
+                print('\nmodule load intel/2019u4  intelmpi/2019u4\nmodule load lammps/20Nov2019\n')
+                print(('srun -n %d lmp_mpi  < %d.in')%(node*corepnode,i))
+            elif server == "cedar":
                 print('\nmodule load nixpkgs/16.09  intel/2018.3  openmpi/3.1.2\nmodule load lammps-omp/20190807\n')
                 print(('srun -n %d lmp_icc_openmpi  < %d.in')%(node*corepnode,i))
-            elif server == "cedar" or server == "graham":
-                print('\nmodule load nixpkgs/16.09  intel/2018.3  openmpi/3.1.2\nmodule load lammps-omp/20190807\n')
-                print(('srun -n %d lmp_icc_openmpi  < %d.in')%(node*corepnode,i))
-            elif server == 'niagara':
-                #print('\nmodule load intel/2018.2 intelmpi/2018.2 fftw-mpi/3.3.7\n')
-                print('\nmodule load intel/2019u3  intelmpi/2019u3 fftw/3.3.8\n')
-                print(('srun lmp < %d.in')%(i))
+            elif server in ['niagara','graham']:
+                print('\nmodule load StdEnv/2020  intel/2020.1.217  openmpi/4.0.3\nmodule load lammps-omp/20220623\n')
+                print(('srun -n %d lmp < %d.in')%(node*corepnode,i))
+            elif server == "narval":
+                print('\nmodule load StdEnv/2020  intel/2020.1.217  openmpi/4.0.3\nmodule load lammps-omp/20210929\n')
+                print(('srun -n %d lmp < %d.in')%(192,i))
+
+                
             sys.stdout.close();
         sys.stdout=oldstdout;
         
         ########################to make lammps in file#############################
     
 
         if subtype =="100mc": #8086
@@ -3767,14 +3803,21 @@
         
         sys.stdout = open('list.txt','w')
         for i in range(wstart, wstop):
             print('{}{}.colvars.split.traj {} {} {}'.format(subtype, i, middle[i], K[i], 60))
         sys.stdout.close();
         sys.stdout=oldstdout
         
+        ########################## wham command file ##########################
+        
+        sys.stdout = open('wham.txt','w')
+        print(f'wham 2.0 14.5 100 0.0001 300 0 list.txt {f[0]}.txt 10 {random.randint(9999,10000000)}')
+        sys.stdout.close();
+        sys.stdout=oldstdout
+        
         ########################### cp all traj once done #####################
         
         sys.stdout = open('cp.sh','w')
         for i in range(wstart, wstop):
             print('cp {}/{}/dz/{}{}.colvars.split.traj -t {};'.format(subloc, i, subtype, i,subloc))
         sys.stdout.close();
         sys.stdout=oldstdout
```

### Comparing `cowboe-1.0.8.8/setup.py` & `cowboe-1.0.8.9/setup.py`

 * *Files identical despite different names*

