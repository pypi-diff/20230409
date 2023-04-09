# Comparing `tmp/hds_stats-0.0.3-py3-none-any.whl.zip` & `tmp/hds_stats-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,10 @@
-Zip file size: 13574 bytes, number of entries: 9
--rw-r--r--  2.0 unx     6375 b- defN 23-Apr-09 06:00 hds_plot.py
--rw-r--r--  2.0 unx    16071 b- defN 23-Apr-09 06:13 hds_stat.py
--rw-r--r--  2.0 unx     6375 b- defN 23-Apr-09 06:00 plot.py
--rw-r--r--  2.0 unx    16071 b- defN 23-Apr-09 06:13 stat.py
--rw-rw-r--  2.0 unx     1073 b- defN 23-Apr-09 07:04 hds_stats-0.0.3.dist-info/LICENSE
--rw-r--r--  2.0 unx      800 b- defN 23-Apr-09 07:04 hds_stats-0.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-09 07:04 hds_stats-0.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       18 b- defN 23-Apr-09 07:04 hds_stats-0.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      661 b- defN 23-Apr-09 07:04 hds_stats-0.0.3.dist-info/RECORD
-9 files, 47536 bytes uncompressed, 12458 bytes compressed:  73.8%
+Zip file size: 8168 bytes, number of entries: 8
+-rw-r--r--  2.0 unx     6148 b- defN 23-Apr-09 07:05 .DS_Store
+-rw-r--r--  2.0 unx     7055 b- defN 23-Apr-09 07:18 hds_plot.py
+-rw-r--r--  2.0 unx    17245 b- defN 23-Apr-09 07:28 hds_stat.py
+-rw-rw-r--  2.0 unx     1073 b- defN 23-Apr-09 07:29 hds_stats-0.0.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx      800 b- defN 23-Apr-09 07:29 hds_stats-0.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-09 07:29 hds_stats-0.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       18 b- defN 23-Apr-09 07:29 hds_stats-0.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      598 b- defN 23-Apr-09 07:29 hds_stats-0.0.4.dist-info/RECORD
+8 files, 33029 bytes uncompressed, 7138 bytes compressed:  78.4%
```

## zipnote {}

```diff
@@ -1,28 +1,25 @@
-Filename: hds_plot.py
-Comment: 
-
-Filename: hds_stat.py
+Filename: .DS_Store
 Comment: 
 
-Filename: plot.py
+Filename: hds_plot.py
 Comment: 
 
-Filename: stat.py
+Filename: hds_stat.py
 Comment: 
 
-Filename: hds_stats-0.0.3.dist-info/LICENSE
+Filename: hds_stats-0.0.4.dist-info/LICENSE
 Comment: 
 
-Filename: hds_stats-0.0.3.dist-info/METADATA
+Filename: hds_stats-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: hds_stats-0.0.3.dist-info/WHEEL
+Filename: hds_stats-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: hds_stats-0.0.3.dist-info/top_level.txt
+Filename: hds_stats-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: hds_stats-0.0.3.dist-info/RECORD
+Filename: hds_stats-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hds_plot.py

```diff
@@ -1,39 +1,28 @@
-# Import libraries for Python Advanced
-import numpy as np
-import pandas as pd
-from scipy import stats
-import seaborn as sns
-import matplotlib.pyplot as plt
-
-
-# Draw a plot
-# plt.plot(0, 0)
-# plt.close()
-
-# Set line width
-plt.rc(group = 'lines', linewidth = 0.5)
-
-
-# EDA functions
 # outlier properties for box plot
 outlier = {
     'marker': 'o', 
     'markersize': 3, 
     'markerfacecolor': 'pink',
     'markeredgecolor': 'red', 
     'markeredgewidth': 0.2
 }
 
-def plot_box_group(
+def box_group(
     data, 
     x, 
     y, 
     pal = None
 ):
+    import numpy as np
+    import pandas as pd
+    from scipy import stats
+    import seaborn as sns
+    import matplotlib.pyplot as plt
+    
     avg = data.groupby(x)[y].mean().reset_index()
     sns.boxplot(
         data = data, 
         x = x, 
         y = y, 
         order = avg[x], 
         palette = pal, 
@@ -51,55 +40,73 @@
     plt.axhline(
         y = data[y].mean(), 
         color = 'red', 
         linestyle = '--'
     )
     plt.title(label = f'{x} 범주별 {y}의 평균 비교');
 
-def plot_scatter(
+def scatter(
     data, 
     x, 
     y, 
     color = '0.3'
 ):
+    import numpy as np
+    import pandas as pd
+    from scipy import stats
+    import seaborn as sns
+    import matplotlib.pyplot as plt
+    
     sns.scatterplot(
         data = data, 
         x = x, 
         y = y, 
         color = color
     )
     plt.title(label = f'{x}와(과) {y}의 관계');
 
-def plot_regression(
+def regression(
     data, 
     x, 
     y, 
     color = '0.3', 
     size = 15
 ):
+    import numpy as np
+    import pandas as pd
+    from scipy import stats
+    import seaborn as sns
+    import matplotlib.pyplot as plt
+    
     x_min = data[x].min()
     x_max = data[x].max()
     sns.regplot(
         data = data, 
         x = x, 
         y = y, 
         ci = None, 
         scatter_kws = {'color': color, 'edgecolor': '1', 
                        's': size, 'linewidth': 0.5},
         line_kws = {'color': 'red', 'linewidth': 1.5}
     )
     plt.title(label = f'{x}와(과) {y}의 관계')
     # plt.xlim(x_min * 0.9, x_max * 1.1);
 
-def plot_bar_freq(
+def bar_freq(
     data, 
     y, 
     color = None, 
     pal = None
 ):
+    import numpy as np
+    import pandas as pd
+    from scipy import stats
+    import seaborn as sns
+    import matplotlib.pyplot as plt
+    
     freq = data[y].value_counts().sort_index().reset_index()
     freq.columns = [y, 'freq']
     sns.barplot(
         data = freq, 
         x = y, 
         y = 'freq', 
         color = color, 
@@ -113,29 +120,36 @@
             ha = 'center', 
             va = 'bottom', 
             c = 'black'
         )
     plt.title(label = '목표변수의 범주별 빈도수 비교')
     plt.ylim(0, freq['freq'].max() * 1.1);
 
-def plot_bar_dodge_freq(
+def bar_dodge_freq(
     data, 
     x, 
     y, 
     pal = None
 ):
+    import numpy as np
+    import pandas as pd
+    from scipy import stats
+    import seaborn as sns
+    import matplotlib.pyplot as plt
+    
     grp = data.groupby(by = [x, y]).count().iloc[:, 0]
     sns.countplot(
         data = data, 
         x = x, 
         hue = y, 
         order = grp.index.levels[0], 
         hue_order = grp.index.levels[1], 
         palette = pal
-    )    
+    )
+    
     for i, v in enumerate(grp):
         if i % 2 == 0:
             i = i/2 - 0.2
         else:
             i = (i-1)/2 + 0.2
         plt.text(
             x = i, 
@@ -143,21 +157,27 @@
             s = v, 
             ha = 'center', 
             va = 'bottom'
         )
     plt.title(label = f'{x}의 범주별 {y}의 빈도수 비교')
     plt.legend(loc = 'best');
 
-def plot_bar_stack_freq(
+def bar_stack_freq(
     data, 
     x, 
     y, 
     kind = 'bar', 
     pal = None
 ):
+    import numpy as np
+    import pandas as pd
+    from scipy import stats
+    import seaborn as sns
+    import matplotlib.pyplot as plt
+    
     p = data[y].unique().size
     pv = pd.pivot_table(
         data = data, 
         index = x, 
         columns = y, 
         aggfunc = 'count'
     )
@@ -203,21 +223,27 @@
                     y = i, 
                     s = v2, 
                     ha = 'center', 
                     va = 'center', 
                     c = 'black'
                 );
 
-def plot_bar_stack_prop(
+def bar_stack_prop(
     data, 
     x, 
     y, 
     kind = 'bar', 
     pal = None
 ):
+    import numpy as np
+    import pandas as pd
+    from scipy import stats
+    import seaborn as sns
+    import matplotlib.pyplot as plt
+    
     p = data[y].unique().size
     pv = pd.pivot_table(
         data = data, 
         index = x, 
         columns = y, 
         aggfunc = 'count'
     )
```

## hds_stat.py

```diff
@@ -1,32 +1,13 @@
-# Import libraries for Python Advanced
-import numpy as np
-import pandas as pd
-from scipy import stats
-import seaborn as sns
-import matplotlib.pyplot as plt
-
-import statsmodels.api as sm
-import statsmodels.formula.api as smf
-import statsmodels.stats.outliers_influence as oi
-from statsmodels.stats.outliers_influence import OLSInfluence
-
-from sklearn.metrics import mean_squared_error
-from sklearn.metrics import mean_squared_log_error
-from sklearn.metrics import mean_absolute_error
-from sklearn.metrics import mean_absolute_percentage_error
-from sklearn.metrics import roc_curve, auc
-from sklearn.metrics import PrecisionRecallDisplay
-from sklearn.metrics import confusion_matrix
-from sklearn.metrics import classification_report
-from sklearn.metrics import matthews_corrcoef
-
-
 # Linear Regression Variable Selection
 def forward_selection(y, X):
+    import numpy as np
+    import pandas as pd
+    import statsmodels.formula.api as smf
+    
     if 'const' in X.columns:
         X = X.drop(labels = ['const'], axis = 1)
     Xvars = set(X.columns)
     dat = pd.concat(objs = [X, y], axis = 1)
     
     formula = f'{y.name} ~ 1'
     curr_aic = smf.ols(formula = formula, data = dat).fit().aic
@@ -51,14 +32,18 @@
             break
     
     formula = f'{y.name} ~ {" + ".join(selected)} + 1'
     model = smf.ols(formula = formula, data = dat).fit()
     return model
 
 def backward_selection(y, X):
+    import numpy as np
+    import pandas as pd
+    import statsmodels.formula.api as smf
+    
     if 'const' in X.columns:
         X = X.drop(labels = ['const'], axis = 1)
     Xvars = set(X.columns)
     dat = pd.concat(objs = [X, y], axis = 1)
     
     formula = f'{y.name} ~ {" + ".join(list(Xvars))}'
     curr_aic = smf.ols(formula = formula, data = dat).fit().aic
@@ -88,14 +73,18 @@
     dat_Xvars = set(dat.columns) - set([y.name])
     
     formula = f'{y.name} ~ {" + ".join(list(dat_Xvars))} + 1'
     model = smf.ols(formula = formula, data = dat).fit()
     return model
 
 def stepwise_selection(y, X):
+    import numpy as np
+    import pandas as pd
+    import statsmodels.formula.api as smf
+    
     if 'const' in X.columns:
         X = X.drop(labels = ['const'], axis = 1)
     Xvars = set(X.columns)
     dat = pd.concat(objs = [X, y], axis = 1)
     
     formula = f'{y.name} ~ 1'
     curr_aic = smf.ols(formula = formula, data = dat).fit().aic
@@ -147,14 +136,20 @@
     else:
         model = None
     return model
 
 
 # Linear Regression Diagnosis
 def regressionDiagnosis(model):
+    import numpy as np
+    import pandas as pd
+    import seaborn as sns
+    import matplotlib.pyplot as plt
+    from scipy import stats
+    
     plt.figure(figsize = (10, 10), dpi = 100)
     
     # Linearity
     # lowess: locally weighted linear regression
     ax1 = plt.subplot(2, 2, 1)
     sns.regplot(
         x = model.fittedvalues, 
@@ -257,46 +252,59 @@
     
     plt.tight_layout()
     plt.show()
 
 
 # Influence Points
 def influencePoints(model):
+    from statsmodels.stats.outliers_influence import OLSInfluence
+    
     cd, _ = OLSInfluence(results = model).cooks_distance
     cd = cd.sort_values(ascending = False)
     return cd
 
 # Hat Matrix
 def hat_matrix(X):
+    import numpy as np
+    import pandas as pd
+    
     X = np.array(object = X)
     XtX = np.matmul(X.transpose(), X)
     XtX_inv = np.linalg.inv(XtX)
     result = np.matmul(
         np.matmul(X, XtX_inv), 
         X.transpose()
     )
     return result
 
 # Leverage: Hat Value
 def leverage(X):
+    import numpy as np
+    import pandas as pd
+    
     n = X.shape[0]
     hatMat = hat_matrix(X = X)
     X['Leverage'] = np.array([hatMat[i][i] for i in range(n)])
     X = X.iloc[:, -1].sort_values(ascending = False)
     return X
 
 # Standardized residuals
 def std_Resid(model):
+    from scipy import stats
+    
     stdres = stats.zscore(a = model.resid)
     locs = stdres.abs().sort_values(ascending = False)
     return stdres[locs.index]
 
 
 # Effect Points for Linear Regression
 def augment(model):
+    import numpy as np
+    import pandas as pd
+    
     infl = model.get_influence()
     df1 = pd.DataFrame(
         data = {model.model.endog_names: infl.endog},
         index = model.fittedvalues.index
     )
     df2 = pd.DataFrame(
         data = {
@@ -309,27 +317,38 @@
         }
     )
     result = pd.concat(objs = [df1, df2], axis = 1)
     return result
 
 # Residual Homoscedasticity Test: Breusch-Pagan Lagrange Multiplier Test
 def breushpagan(model):
+    import numpy as np
+    import pandas as pd
+    import statsmodels.api as sm
+    
     test = sm.stats.het_breuschpagan(
         resid = model.resid, 
         exog_het = model.model.exog
     )
     result = pd.DataFrame(
         data = test, 
         index = ['Statistic', 'P-Value', 'F-Value', 'F P-Value']
     ).T
     return result
 
 
 # Metrics for Regression: MSE, RMSE, MSE, MAPE
 def regmetrics(y_true, y_pred):
+    import numpy as np
+    import pandas as pd
+    from sklearn.metrics import mean_squared_error
+    from sklearn.metrics import mean_squared_log_error
+    from sklearn.metrics import mean_absolute_error
+    from sklearn.metrics import mean_absolute_percentage_error
+    
     MSE = mean_squared_error(
         y_true = y_true, 
         y_pred = y_pred
     )
     
     RMSE = MSE**(1/2)
     
@@ -366,14 +385,20 @@
 # Metrics for Classification: ROC, AUC
 def plot_roc(
     y_true, 
     y_prob, 
     pos = None, 
     color = None
 ):
+    import numpy as np
+    import pandas as pd
+    import seaborn as sns
+    import matplotlib.pyplot as plt
+    from sklearn.metrics import roc_curve, auc
+    
     y_class = y_true.value_counts().sort_index()
     
     if pos == None:
         pos = y_class.loc[y_class == y_class.min()].index[0]
     
     idx = np.where(y_class.index == pos)[0][0]
     
@@ -413,14 +438,20 @@
 def plot_pr(
     y_true, 
     y_prob, 
     pos = None, 
     name = None, 
     color = None
 ):
+    import numpy as np
+    import pandas as pd
+    import seaborn as sns
+    import matplotlib.pyplot as plt
+    from sklearn.metrics import PrecisionRecallDisplay
+    
     y_class = y_true.value_counts().sort_index()
     
     if pos == None:
         pos = y_class.loc[y_class == y_class.min()].index[0]
     
     idx = np.where(y_class.index == pos)[0][0]
     
@@ -439,26 +470,33 @@
     plt.xlabel(xlabel = 'Recall')
     plt.ylabel(ylabel = 'Precision')
     plt.legend(loc = 'best');
 
 
 # Variance Inflation factor
 def vif(X):
+    import numpy as np
+    import pandas as pd
+    import statsmodels.stats.outliers_influence as oi
+    
     X2 = X.copy()
     if 'const' not in X2.columns:
         X2.insert(loc = 0, column = 'const', value = 1)
     
     func = oi.variance_inflation_factor
     ncol = X2.shape[1]
     vifs = [func(exog = X2.values, exog_idx = i) for i in range(1, ncol)]
     result = pd.DataFrame(data = vifs, index = X2.columns[1:]).T
     return result
 
 # Coefficients for Regression
 def coefs(model):
+    import numpy as np
+    import pandas as pd
+    
     if model.coef_.ndim == 1:
         coefs = pd.Series(
             data = model.coef_, 
             index = model.feature_names_in_
         )
     elif model.coef_.ndim == 2:
         coefs = pd.Series(
@@ -467,14 +505,17 @@
         )
     else:
         coefs = pd.Series()
     return coefs
 
 # Standardized Coefficients
 def std_coefs(model):
+    import numpy as np
+    import pandas as pd
+    
     model_type = str(type(model.model))
     X = pd.DataFrame(
         data = model.model.exog, 
         columns = model.model.exog_names
     )
     if 'OLS' in model_type:
         y = model.model.endog
@@ -483,14 +524,17 @@
         y = 1
         result = model.params * (X.std() / 1)
     return result
 
 
 # Metrics for Classification: Confusion Matrix, F1 Score
 def clfmetrics(y_true, y_pred):
+    from sklearn.metrics import confusion_matrix
+    from sklearn.metrics import classification_report
+    
     print('▶ Confusion Matrix')
     print(
         confusion_matrix(
             y_true = y_true, 
             y_pred = y_pred
         )
     )
@@ -506,14 +550,20 @@
         )
     )
 
 
 # Classification metrics with Cutoff for Logistic Regression
 # Plus, Matthew's Correlation coefficient
 def clfCutoffs(y_true, y_prob):
+    import numpy as np
+    import pandas as pd
+    from sklearn.metrics import confusion_matrix
+    from sklearn.metrics import classification_report
+    from sklearn.metrics import matthews_corrcoef
+    
     cutoffs = np.linspace(0, 1, 101)
     sens = []
     spec = []
     prec = []
     mccs = []
     
     for cutoff in cutoffs:
@@ -555,15 +605,17 @@
     cols = ['Cutoff', 'Sensitivity', 'Specificity', 'Optimal', \
             'Precision', 'TPR', 'FPR', 'MCC']
     result = result[cols]
     return result
 
 # Draw ROC Curve with Optimal Cutoff
 def EpiROC(obj):
-    
+    import seaborn as sns
+    import matplotlib.pyplot as plt
+
     # Draw ROC curve
     sns.lineplot(
         data = obj, 
         x = 'FPR', 
         y = 'TPR', 
         color = 'black'
     )
```

## Comparing `hds_stats-0.0.3.dist-info/LICENSE` & `hds_stats-0.0.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `hds_stats-0.0.3.dist-info/METADATA` & `hds_stats-0.0.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hds-stats
-Version: 0.0.3
+Version: 0.0.4
 Summary: Useful functions for Statistics and Machine Learning
 Home-page: https://github.com/HelloDataScience/hds-stats
 Author: HelloDataScience
 Author-email: hellodatasciencekorea@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/HelloDataScience/hds-stats/issues
 Classifier: Programming Language :: Python :: 3
```

