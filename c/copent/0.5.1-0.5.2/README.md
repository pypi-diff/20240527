# Comparing `tmp/copent-0.5.1.tar.gz` & `tmp/copent-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copent-0.5.1.tar", last modified: Mon Feb 12 23:42:43 2024, max compression
+gzip compressed data, was "copent-0.5.2.tar", last modified: Mon May 27 20:38:24 2024, max compression
```

## Comparing `copent-0.5.1.tar` & `copent-0.5.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxr-x   0 majian    (1000) majian    (1000)        0 2024-02-12 23:42:43.689805 copent-0.5.1/
--rw-rw-r--   0 majian    (1000) majian    (1000)     7275 2024-02-12 23:42:43.689805 copent-0.5.1/PKG-INFO
--rw-rw-r--   0 majian    (1000) majian    (1000)     5915 2024-02-12 07:14:14.000000 copent-0.5.1/README.md
-drwxrwxr-x   0 majian    (1000) majian    (1000)        0 2024-02-12 23:42:43.689805 copent-0.5.1/copent/
--rw-rw-r--   0 majian    (1000) majian    (1000)       97 2024-02-12 06:43:57.000000 copent-0.5.1/copent/__init__.py
--rw-rw-r--   0 majian    (1000) majian    (1000)     5089 2024-02-12 23:42:19.000000 copent-0.5.1/copent/copent.py
-drwxrwxr-x   0 majian    (1000) majian    (1000)        0 2024-02-12 23:42:43.689805 copent-0.5.1/copent.egg-info/
--rw-rw-r--   0 majian    (1000) majian    (1000)     7275 2024-02-12 23:42:43.000000 copent-0.5.1/copent.egg-info/PKG-INFO
--rw-rw-r--   0 majian    (1000) majian    (1000)      203 2024-02-12 23:42:43.000000 copent-0.5.1/copent.egg-info/SOURCES.txt
--rw-rw-r--   0 majian    (1000) majian    (1000)        1 2024-02-12 23:42:43.000000 copent-0.5.1/copent.egg-info/dependency_links.txt
--rw-rw-r--   0 majian    (1000) majian    (1000)       12 2024-02-12 23:42:43.000000 copent-0.5.1/copent.egg-info/requires.txt
--rw-rw-r--   0 majian    (1000) majian    (1000)        7 2024-02-12 23:42:43.000000 copent-0.5.1/copent.egg-info/top_level.txt
--rw-rw-r--   0 majian    (1000) majian    (1000)       38 2024-02-12 23:42:43.689805 copent-0.5.1/setup.cfg
--rw-rw-r--   0 majian    (1000) majian    (1000)      555 2024-02-12 23:41:57.000000 copent-0.5.1/setup.py
+drwxrwxr-x   0 majian    (1000) majian    (1000)        0 2024-05-27 20:38:24.161776 copent-0.5.2/
+-rw-rw-r--   0 majian    (1000) majian    (1000)    35149 2022-09-11 06:39:52.000000 copent-0.5.2/LICENSE
+-rw-rw-r--   0 majian    (1000) majian    (1000)     6220 2024-05-27 20:38:24.161776 copent-0.5.2/PKG-INFO
+-rw-rw-r--   0 majian    (1000) majian    (1000)     5889 2024-03-14 23:57:08.000000 copent-0.5.2/README.md
+drwxrwxr-x   0 majian    (1000) majian    (1000)        0 2024-05-27 20:38:24.161776 copent-0.5.2/copent/
+-rw-rw-r--   0 majian    (1000) majian    (1000)       97 2024-02-12 06:43:57.000000 copent-0.5.2/copent/__init__.py
+-rw-rw-r--   0 majian    (1000) majian    (1000)     6323 2024-05-27 20:23:02.000000 copent-0.5.2/copent/copent.py
+drwxrwxr-x   0 majian    (1000) majian    (1000)        0 2024-05-27 20:38:24.161776 copent-0.5.2/copent.egg-info/
+-rw-rw-r--   0 majian    (1000) majian    (1000)     6220 2024-05-27 20:38:24.000000 copent-0.5.2/copent.egg-info/PKG-INFO
+-rw-rw-r--   0 majian    (1000) majian    (1000)      211 2024-05-27 20:38:24.000000 copent-0.5.2/copent.egg-info/SOURCES.txt
+-rw-rw-r--   0 majian    (1000) majian    (1000)        1 2024-05-27 20:38:24.000000 copent-0.5.2/copent.egg-info/dependency_links.txt
+-rw-rw-r--   0 majian    (1000) majian    (1000)       12 2024-05-27 20:38:24.000000 copent-0.5.2/copent.egg-info/requires.txt
+-rw-rw-r--   0 majian    (1000) majian    (1000)        7 2024-05-27 20:38:24.000000 copent-0.5.2/copent.egg-info/top_level.txt
+-rw-rw-r--   0 majian    (1000) majian    (1000)       38 2024-05-27 20:38:24.161776 copent-0.5.2/setup.cfg
+-rw-rw-r--   0 majian    (1000) majian    (1000)      555 2024-05-27 20:34:06.000000 copent-0.5.2/setup.py
```

### Comparing `copent-0.5.1/PKG-INFO` & `copent-0.5.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,142 +1,145 @@
 Metadata-Version: 2.1
 Name: copent
-Version: 0.5.1
+Version: 0.5.2
 Summary: Estimating Copula Entropy and Transfer Entropy
 Home-page: https://github.com/majianthu/pycopent
 Author: MA Jian
 Author-email: majian03@gmail.com
 License: GPL License
-Description: [![PyPI version](https://badge.fury.io/py/copent.svg)](https://pypi.org/project/copent)
-        # copent
-        Estimating Copula Entropy and Transfer Entropy
-        
-        #### Introduction
-        The nonparametric methods for estimating copula entropy, transfer entropy, and the statistics for multivariate normality test and two-sample test are implemented. The change point detection method based on this two-sample test is also implemented.
-        
-        The method for estimating copula entropy composes of two simple steps: estimating empirical copula by rank statistic and estimating copula entropy with the KSG method. Copula Entropy is a mathematical concept for multivariate statistical independence measuring and testing, and proved to be equivalent to mutual information. Different from Pearson Correlation Coefficient, Copula Entropy is defined for non-linear, high-order and multivariate cases, which makes it universally applicable. Estimating copula entropy can be applied to many cases, including but not limited to variable selection and causal discovery (by estimating transfer entropy). Please refer to Ma and Sun (2011) <[doi:10.1016/S1007-0214(11)70008-6](http://www.doi.org/10.1016/S1007-0214(11)70008-6)> for more information.
-        
-        The nonparametric method for estimating transfer entropy composes of two steps: estimating three copula entropy and calculating transfer entropy from the estimated copula entropies. A function for conditional independence testing is also provided. Please refer to Ma (2019) <[arXiv:1910.04375](https://arxiv.org/abs/1910.04375)> for more information.
-        
-        The copula entropy based statistics for multivariate normality test and two-sample test are implemented. The change point detection method based on this two-sample test is also implemented. Please refer to Ma (2022) <[arXiv:2206.05956](https://arxiv.org/abs/2206.05956)>, Ma (2023) <[arXiv:2307.07247](https://arxiv.org/abs/2307.07247)>, and Ma (2024) <[doi:10.13140/RG.2.2.16378.26562](https://doi.org/10.13140/RG.2.2.16378.26562)> for more details. 
-        
-        #### Functions
-        * copent -- estimating copula entropy;
-        * construct_empirical_copula -- the first step of the copent function, which estimates empirical copula for data by rank statistics;
-        * entknn -- the second step of the copent function, which estimates copula entropy from empirical copula with kNN method;
-        * ci -- conditional independence testing based on copula entropy 
-        * transent -- estimating transfer entropy via copula entropy
-        * mvnt -- estimating the copula entropy-based statistic for multivariate normality test
-        * tst -- estimating the copula entropy-based statistic for two-sample test
-        * cpd -- single change point detection
-        * mcpd -- multiple change point detection
-        
-        #### Parameters
-        * x: N * d data, N samples, d dimensions
-        * k: kth nearest neighbour, parameter for kNN entropy estimation. default = 3
-        * dtype: distance type, can be 'euclidean' or 'chebychev' (for Maximum Distance)
-        * lag: time lag. default = 1
-        * s0,s1: two samples with same dimension
-        * n: repeat time of estimation
-        * thd	: threshold for the statistic of two-sample test
-        * maxp	: maximal number of change points
-        * minseglen : minimal length of binary segmentation
-        
-        #### Installation
-        The package can be installed from PyPI directly:
-        ```
-        pip install copent
-        ```
-        The package can be installed from Github:
-        ```
-        pip install git+https://github.com/majianthu/pycopent.git
-        ```
-        #### Usage Examples
-        ##### estimating copula entropy 
-        ```python
-        from numpy.random import multivariate_normal as mnorm
-        import copent
-        rho = 0.6
-        mean1 = [0,0]
-        cov1 = [ [1,rho],[rho,1] ]
-        x = mnorm(mean1,cov1,200) # bivariate gaussian 
-        ce1 = copent.copent(x) # estimated copula entropy
-        ```
-        
-        ##### estimating transfer entropy 
-        ```python
-        from copent import transent
-        from pandas import read_csv
-        import numpy as np
-        url = "https://archive.ics.uci.edu/ml/machine-learning-databases/00381/PRSA_data_2010.1.1-2014.12.31.csv"
-        prsa2010 = read_csv(url)
-        # index: 5(PM2.5),6(Dew Point),7(Temperature),8(Pressure),10(Cumulative Wind Speed)
-        data = prsa2010.iloc[2200:2700,[5,8]].values
-        te = np.zeros(24)
-        for lag in range(1,25):
-        	te[lag-1] = transent(data[:,0],data[:,1],lag)
-        	str = "TE from pressure to PM2.5 at %d hours lag : %f" %(lag,te[lag-1])
-        	print(str)
-        ```
-        
-        ##### multivariate normality test
-        ```python
-        from numpy.random import multivariate_normal as mnorm
-        from copent import mvnt
-        mean1 = [0,0]
-        cov1 = [[1,0.65],[0.65,1]]
-        data = mnorm(mean1, cov1, 500)
-        stat1 = mvnt(data)
-        ```
-        
-        ##### two-sample test
-        ```python
-        from copent import tst
-        from numpy import zeros
-        from numpy.random import multivariate_normal as mnorm
-        m0 = [0,0]
-        rho1 = 0.5
-        v0 = [[1,rho1],[rho1,1]]
-        s0 = mnorm(m0, v0, 400) # bivariate gaussian 
-        stat1 = zeros(9)
-        for i in range(0,9):
-        	m1 = [i,i]
-        	s1 = mnorm(m1,v0,500)
-        	stat1[i] = tst(s0,s1)
-        	print(stat1[i])
-        ```
-        
-        ##### change point detection
-        ```python
-        from copent import mcpd
-        import numpy as np
-        from numpy.random import multivariate_normal as mnorm
-        
-        n1 = 50
-        x1 = np.random.normal(0,1,n1)
-        x2 = np.random.normal(5,1,n1)
-        x3 = np.random.normal(10,1,n1)
-        x4 = np.random.normal(1,1,n1)
-        x = np.concatenate((x1,x2,x3,x4))
-        pos,maxstat = mcpd(x,thd =0.2)
-        print(pos)
-        
-        x1 = mnorm([0,0],[[1,0],[0,1]],n1)
-        x2 = mnorm([10,10],[[1,0],[0,1]],n1)
-        x3 = mnorm([5,5],[[1,0],[0,1]],n1)
-        x4 = mnorm([1,1],[[1,0],[0,1]],n1)
-        x = np.concatenate((x1,x2,x3,x4))
-        pos,maxstat = mcpd(x,thd =0.2)
-        print(pos)
-        ```
-        
-        #### References
-        1. Jian Ma and Zengqi Sun. Mutual information is copula entropy. Tsinghua Science & Technology, 2011, 16(1): 51-54. See also arXiv preprint arXiv:0808.0845, 2008.
-        2. Jian Ma. Estimating Transfer Entropy via Copula Entropy. arXiv preprint arXiv:1910.04375, 2019.
-        3. Jian Ma. Multivariate Normality Test with Copula Entropy. arXiv preprint arXiv:2206.05956, 2022.
-        4. Jian Ma. Two-Sample Test with Copula Entropy. arXiv preprint arXiv:2307.07247, 2023.
-        5. Jian Ma. Change Point Detection with Copula Entropy based Two-Sample Test. DOI:10.13140/RG.2.2.16378.26562, 2024.
-        
-        
 Platform: UNKNOWN
 Requires-Python: >=2.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![PyPI version](https://badge.fury.io/py/copent.svg)](https://pypi.org/project/copent)
+# copent
+Estimating Copula Entropy and Transfer Entropy
+
+#### Introduction
+The nonparametric methods for estimating copula entropy, transfer entropy, and the statistics for multivariate normality test and two-sample test are implemented. The change point detection method based on this two-sample test is also implemented.
+
+The method for estimating copula entropy composes of two simple steps: estimating empirical copula by rank statistic and estimating copula entropy with the KSG method. Copula Entropy is a mathematical concept for multivariate statistical independence measuring and testing, and proved to be equivalent to mutual information. Different from Pearson Correlation Coefficient, Copula Entropy is defined for non-linear, high-order and multivariate cases, which makes it universally applicable. Estimating copula entropy can be applied to many cases, including but not limited to variable selection and causal discovery (by estimating transfer entropy). Please refer to Ma and Sun (2011) <[doi:10.1016/S1007-0214(11)70008-6](http://www.doi.org/10.1016/S1007-0214(11)70008-6)> for more information.
+
+The nonparametric method for estimating transfer entropy composes of two steps: estimating three copula entropy and calculating transfer entropy from the estimated copula entropies. A function for conditional independence testing is also provided. Please refer to Ma (2019) <[arXiv:1910.04375](https://arxiv.org/abs/1910.04375)> for more information.
+
+The copula entropy based statistics for multivariate normality test and two-sample test are implemented. The change point detection method based on this two-sample test is also implemented. Please refer to Ma (2022) <[arXiv:2206.05956](https://arxiv.org/abs/2206.05956)>, Ma (2023) <[arXiv:2307.07247](https://arxiv.org/abs/2307.07247)>, and Ma (2024) <[arXiv:2403.07892](https://arxiv.org/abs/2403.07892)> for more details. 
+
+#### Functions
+* copent -- estimating copula entropy;
+* construct_empirical_copula -- the first step of the copent function, which estimates empirical copula for data by rank statistics;
+* entknn -- the second step of the copent function, which estimates copula entropy from empirical copula with kNN method;
+* ci -- conditional independence testing based on copula entropy 
+* transent -- estimating transfer entropy via copula entropy
+* mvnt -- estimating the copula entropy-based statistic for multivariate normality test
+* tst -- estimating the copula entropy-based statistic for two-sample test
+* cpd -- single change point detection
+* mcpd -- multiple change point detection
+
+#### Parameters
+* x: N * d data, N samples, d dimensions
+* k: kth nearest neighbour, parameter for kNN entropy estimation. default = 3
+* dtype: distance type, can be 'euclidean' or 'chebychev' (for Maximum Distance)
+* lag: time lag. default = 1
+* s0,s1: two samples with same dimension
+* n: repeat time of estimation
+* thd	: threshold for the statistic of two-sample test
+* maxp	: maximal number of change points
+* minseglen : minimal length of binary segmentation
+
+#### Installation
+The package can be installed from PyPI directly:
+```
+pip install copent
+```
+The package can be installed from Github:
+```
+pip install git+https://github.com/majianthu/pycopent.git
+```
+#### Usage Examples
+##### estimating copula entropy 
+```python
+from numpy.random import multivariate_normal as mnorm
+import copent
+rho = 0.6
+mean1 = [0,0]
+cov1 = [ [1,rho],[rho,1] ]
+x = mnorm(mean1,cov1,200) # bivariate gaussian 
+ce1 = copent.copent(x) # estimated copula entropy
+```
+
+##### estimating transfer entropy 
+```python
+from copent import transent
+from pandas import read_csv
+import numpy as np
+url = "https://archive.ics.uci.edu/ml/machine-learning-databases/00381/PRSA_data_2010.1.1-2014.12.31.csv"
+prsa2010 = read_csv(url)
+# index: 5(PM2.5),6(Dew Point),7(Temperature),8(Pressure),10(Cumulative Wind Speed)
+data = prsa2010.iloc[2200:2700,[5,8]].values
+te = np.zeros(24)
+for lag in range(1,25):
+	te[lag-1] = transent(data[:,0],data[:,1],lag)
+	str = "TE from pressure to PM2.5 at %d hours lag : %f" %(lag,te[lag-1])
+	print(str)
+```
+
+##### multivariate normality test
+```python
+from numpy.random import multivariate_normal as mnorm
+from copent import mvnt
+mean1 = [0,0]
+cov1 = [[1,0.65],[0.65,1]]
+data = mnorm(mean1, cov1, 500)
+stat1 = mvnt(data)
+```
+
+##### two-sample test
+```python
+from copent import tst
+from numpy import zeros
+from numpy.random import multivariate_normal as mnorm
+m0 = [0,0]
+rho1 = 0.5
+v0 = [[1,rho1],[rho1,1]]
+s0 = mnorm(m0, v0, 400) # bivariate gaussian 
+stat1 = zeros(9)
+for i in range(0,9):
+	m1 = [i,i]
+	s1 = mnorm(m1,v0,500)
+	stat1[i] = tst(s0,s1)
+	print(stat1[i])
+```
+
+##### change point detection
+```python
+from copent import mcpd
+import numpy as np
+from numpy.random import multivariate_normal as mnorm
+
+n1 = 50
+x1 = np.random.normal(0,1,n1)
+x2 = np.random.normal(5,1,n1)
+x3 = np.random.normal(10,1,n1)
+x4 = np.random.normal(1,1,n1)
+x = np.concatenate((x1,x2,x3,x4))
+pos,maxstat = mcpd(x,thd =0.2)
+print(pos)
+
+x1 = mnorm([0,0],[[1,0],[0,1]],n1)
+x2 = mnorm([10,10],[[1,0],[0,1]],n1)
+x3 = mnorm([5,5],[[1,0],[0,1]],n1)
+x4 = mnorm([1,1],[[1,0],[0,1]],n1)
+x = np.concatenate((x1,x2,x3,x4))
+pos,maxstat = mcpd(x,thd =0.2)
+print(pos)
+```
+
+#### References
+1. Jian Ma and Zengqi Sun. Mutual information is copula entropy. Tsinghua Science & Technology, 2011, 16(1): 51-54. See also arXiv preprint arXiv:0808.0845, 2008.
+2. Jian Ma. Estimating Transfer Entropy via Copula Entropy. arXiv preprint arXiv:1910.04375, 2019.
+3. Jian Ma. Multivariate Normality Test with Copula Entropy. arXiv preprint arXiv:2206.05956, 2022.
+4. Jian Ma. Two-Sample Test with Copula Entropy. arXiv preprint arXiv:2307.07247, 2023.
+5. Jian Ma. Change Point Detection with Copula Entropy based Two-Sample Test. arXiv preprint arXiv:2403.07892, 2024.
+
+
+
```

### Comparing `copent-0.5.1/README.md` & `copent-0.5.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 #### Introduction
 The nonparametric methods for estimating copula entropy, transfer entropy, and the statistics for multivariate normality test and two-sample test are implemented. The change point detection method based on this two-sample test is also implemented.
 
 The method for estimating copula entropy composes of two simple steps: estimating empirical copula by rank statistic and estimating copula entropy with the KSG method. Copula Entropy is a mathematical concept for multivariate statistical independence measuring and testing, and proved to be equivalent to mutual information. Different from Pearson Correlation Coefficient, Copula Entropy is defined for non-linear, high-order and multivariate cases, which makes it universally applicable. Estimating copula entropy can be applied to many cases, including but not limited to variable selection and causal discovery (by estimating transfer entropy). Please refer to Ma and Sun (2011) <[doi:10.1016/S1007-0214(11)70008-6](http://www.doi.org/10.1016/S1007-0214(11)70008-6)> for more information.
 
 The nonparametric method for estimating transfer entropy composes of two steps: estimating three copula entropy and calculating transfer entropy from the estimated copula entropies. A function for conditional independence testing is also provided. Please refer to Ma (2019) <[arXiv:1910.04375](https://arxiv.org/abs/1910.04375)> for more information.
 
-The copula entropy based statistics for multivariate normality test and two-sample test are implemented. The change point detection method based on this two-sample test is also implemented. Please refer to Ma (2022) <[arXiv:2206.05956](https://arxiv.org/abs/2206.05956)>, Ma (2023) <[arXiv:2307.07247](https://arxiv.org/abs/2307.07247)>, and Ma (2024) <[doi:10.13140/RG.2.2.16378.26562](https://doi.org/10.13140/RG.2.2.16378.26562)> for more details. 
+The copula entropy based statistics for multivariate normality test and two-sample test are implemented. The change point detection method based on this two-sample test is also implemented. Please refer to Ma (2022) <[arXiv:2206.05956](https://arxiv.org/abs/2206.05956)>, Ma (2023) <[arXiv:2307.07247](https://arxiv.org/abs/2307.07247)>, and Ma (2024) <[arXiv:2403.07892](https://arxiv.org/abs/2403.07892)> for more details. 
 
 #### Functions
 * copent -- estimating copula entropy;
 * construct_empirical_copula -- the first step of the copent function, which estimates empirical copula for data by rank statistics;
 * entknn -- the second step of the copent function, which estimates copula entropy from empirical copula with kNN method;
 * ci -- conditional independence testing based on copula entropy 
 * transent -- estimating transfer entropy via copula entropy
@@ -122,9 +122,9 @@
 ```
 
 #### References
 1. Jian Ma and Zengqi Sun. Mutual information is copula entropy. Tsinghua Science & Technology, 2011, 16(1): 51-54. See also arXiv preprint arXiv:0808.0845, 2008.
 2. Jian Ma. Estimating Transfer Entropy via Copula Entropy. arXiv preprint arXiv:1910.04375, 2019.
 3. Jian Ma. Multivariate Normality Test with Copula Entropy. arXiv preprint arXiv:2206.05956, 2022.
 4. Jian Ma. Two-Sample Test with Copula Entropy. arXiv preprint arXiv:2307.07247, 2023.
-5. Jian Ma. Change Point Detection with Copula Entropy based Two-Sample Test. DOI:10.13140/RG.2.2.16378.26562, 2024.
+5. Jian Ma. Change Point Detection with Copula Entropy based Two-Sample Test. arXiv preprint arXiv:2403.07892, 2024.
```

### Comparing `copent-0.5.1/copent/copent.py` & `copent-0.5.2/copent/copent.py`

 * *Files 17% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 from scipy.special import digamma
 from scipy.stats import rankdata as rank 
 from scipy.spatial.distance import cdist
 from math import gamma, log, pi
 from numpy import array, abs, max, hstack, vstack, ones, zeros, cov, mat, where
 from numpy.random import uniform, normal as rnorm
 from numpy.linalg import det
+from multiprocessing import Pool
 
 ##### constructing empirical copula density [1]
 def construct_empirical_copula(x):
 	(N,d) = x.shape	
 	xc = zeros([N,d]) 
 	for i in range(0,d):
 		xc[:,i] = rank(x[:,i]) / N
@@ -122,27 +123,59 @@
 	for i in range(0,n):
 		y1 = vstack((ones([N0,1]),ones([N1,1])*2)) + uniform(0, 0.0000001,[N0+N1,1])
 		y0 = ones([N0+N1,1]) + uniform(0,0.0000001,[N0+N1,1])
 		stat1 = stat1 + copent(hstack((x,y1)),k,dtype) - copent(hstack((x,y0)),k,dtype)
 	return stat1/n
 
 ##### single change point detection [6]
+def init_x_n(X,N):
+	global x,n
+	x = X
+	n = N
+
+def tsti(i):
+	s0 = x[0:(i+1),:]
+	s1 = x[(i+2):,:]
+	return tst(s0,s1,n)
+	
 def cpd(x, thd = 0.13, n = 30):
 	x = mat(x)
 	len1 = x.shape[0]
 	if len1 == 1:
 		len1 = x.shape[1]
 		x = x.T
 	pos = -1
 	maxstat = 0
+	pool = Pool(initializer = init_x_n, initargs=(x,n))
+	stat1 = [0] + pool.map(tsti,range(len1-1))
+	if(max(stat1) > thd):
+		maxstat = max(stat1)
+		pos = where(stat1 == maxstat)[0][0]+1
+	return pos, maxstat, stat1
+
+def cpd2(x, thd = 0.13, n = 30):
+	x = mat(x)
+	len1 = x.shape[0]
+	if len1 == 1:
+		len1 = x.shape[1]
+		x = x.T
+	pos = -1
+	maxstat = 0
 	stat1 = zeros(len1)
-	for i in range(1,len1-1):
+	
+	def fun(i):
 		s0 = x[0:i,:]
 		s1 = x[(i+1):,:]
-		stat1[i] = tst(s0,s1,n)
+		return tst(s0,s1,n)
+	pool = Pool()
+	stat1 = pool.map(fun,range(len1-1))
+	#for i in range(1,len1-1):
+	#	s0 = x[0:i,:]
+	#	s1 = x[(i+1):,:]
+	#	stat1[i] = tst(s0,s1,n)
 	if(max(stat1) > thd):
 		maxstat = max(stat1)
 		pos = where(stat1 == maxstat)[0][0]+1
 	return pos, maxstat, stat1
 
 ##### multiple change point detection [6]
 def mcpd(x, maxp = 5, thd = 0.13, minseglen = 10, n = 30):
@@ -161,10 +194,33 @@
 		if rpos > -1 :
 			rpos = rpos + bisegs[i,0]
 			maxstat.append(rmaxstat)
 			pos.append(rpos)
 			if (rpos - bisegs[i,0]) > minseglen :
 				bisegs = vstack((bisegs,[bisegs[i,0],rpos-1]))
 			if (bisegs[i,1] - rpos +1) > minseglen :
+				bisegs = vstack((bisegs,[rpos,bisegs[i,1]]))
+	return pos,maxstat
+
+def mcpd2(x, maxp = 5, thd = 0.13, minseglen = 10, n = 30):
+	x = mat(x)
+	len1 = x.shape[0]
+	if len1 == 1:
+		len1 = x.shape[1]
+		x = x.T
+	maxstat = []
+	pos = []
+	bisegs = mat([0,len1-1])
+	for i in range(0,maxp):
+		if i >= bisegs.shape[0]:
+			break
+		rpos, rmaxstat, _ = cpd2(x[bisegs[i,0]:bisegs[i,1],:],thd,n)
+		if rpos > -1 :
+			rpos = rpos + bisegs[i,0]
+			maxstat.append(rmaxstat)
+			pos.append(rpos)
+			if (rpos - bisegs[i,0]) > minseglen :
+				bisegs = vstack((bisegs,[bisegs[i,0],rpos-1]))
+			if (bisegs[i,1] - rpos +1) > minseglen :
 				bisegs = vstack((bisegs,[rpos,bisegs[i,1]]))
 	return pos,maxstat
```

### Comparing `copent-0.5.1/copent.egg-info/PKG-INFO` & `copent-0.5.2/copent.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,142 +1,145 @@
 Metadata-Version: 2.1
 Name: copent
-Version: 0.5.1
+Version: 0.5.2
 Summary: Estimating Copula Entropy and Transfer Entropy
 Home-page: https://github.com/majianthu/pycopent
 Author: MA Jian
 Author-email: majian03@gmail.com
 License: GPL License
-Description: [![PyPI version](https://badge.fury.io/py/copent.svg)](https://pypi.org/project/copent)
-        # copent
-        Estimating Copula Entropy and Transfer Entropy
-        
-        #### Introduction
-        The nonparametric methods for estimating copula entropy, transfer entropy, and the statistics for multivariate normality test and two-sample test are implemented. The change point detection method based on this two-sample test is also implemented.
-        
-        The method for estimating copula entropy composes of two simple steps: estimating empirical copula by rank statistic and estimating copula entropy with the KSG method. Copula Entropy is a mathematical concept for multivariate statistical independence measuring and testing, and proved to be equivalent to mutual information. Different from Pearson Correlation Coefficient, Copula Entropy is defined for non-linear, high-order and multivariate cases, which makes it universally applicable. Estimating copula entropy can be applied to many cases, including but not limited to variable selection and causal discovery (by estimating transfer entropy). Please refer to Ma and Sun (2011) <[doi:10.1016/S1007-0214(11)70008-6](http://www.doi.org/10.1016/S1007-0214(11)70008-6)> for more information.
-        
-        The nonparametric method for estimating transfer entropy composes of two steps: estimating three copula entropy and calculating transfer entropy from the estimated copula entropies. A function for conditional independence testing is also provided. Please refer to Ma (2019) <[arXiv:1910.04375](https://arxiv.org/abs/1910.04375)> for more information.
-        
-        The copula entropy based statistics for multivariate normality test and two-sample test are implemented. The change point detection method based on this two-sample test is also implemented. Please refer to Ma (2022) <[arXiv:2206.05956](https://arxiv.org/abs/2206.05956)>, Ma (2023) <[arXiv:2307.07247](https://arxiv.org/abs/2307.07247)>, and Ma (2024) <[doi:10.13140/RG.2.2.16378.26562](https://doi.org/10.13140/RG.2.2.16378.26562)> for more details. 
-        
-        #### Functions
-        * copent -- estimating copula entropy;
-        * construct_empirical_copula -- the first step of the copent function, which estimates empirical copula for data by rank statistics;
-        * entknn -- the second step of the copent function, which estimates copula entropy from empirical copula with kNN method;
-        * ci -- conditional independence testing based on copula entropy 
-        * transent -- estimating transfer entropy via copula entropy
-        * mvnt -- estimating the copula entropy-based statistic for multivariate normality test
-        * tst -- estimating the copula entropy-based statistic for two-sample test
-        * cpd -- single change point detection
-        * mcpd -- multiple change point detection
-        
-        #### Parameters
-        * x: N * d data, N samples, d dimensions
-        * k: kth nearest neighbour, parameter for kNN entropy estimation. default = 3
-        * dtype: distance type, can be 'euclidean' or 'chebychev' (for Maximum Distance)
-        * lag: time lag. default = 1
-        * s0,s1: two samples with same dimension
-        * n: repeat time of estimation
-        * thd	: threshold for the statistic of two-sample test
-        * maxp	: maximal number of change points
-        * minseglen : minimal length of binary segmentation
-        
-        #### Installation
-        The package can be installed from PyPI directly:
-        ```
-        pip install copent
-        ```
-        The package can be installed from Github:
-        ```
-        pip install git+https://github.com/majianthu/pycopent.git
-        ```
-        #### Usage Examples
-        ##### estimating copula entropy 
-        ```python
-        from numpy.random import multivariate_normal as mnorm
-        import copent
-        rho = 0.6
-        mean1 = [0,0]
-        cov1 = [ [1,rho],[rho,1] ]
-        x = mnorm(mean1,cov1,200) # bivariate gaussian 
-        ce1 = copent.copent(x) # estimated copula entropy
-        ```
-        
-        ##### estimating transfer entropy 
-        ```python
-        from copent import transent
-        from pandas import read_csv
-        import numpy as np
-        url = "https://archive.ics.uci.edu/ml/machine-learning-databases/00381/PRSA_data_2010.1.1-2014.12.31.csv"
-        prsa2010 = read_csv(url)
-        # index: 5(PM2.5),6(Dew Point),7(Temperature),8(Pressure),10(Cumulative Wind Speed)
-        data = prsa2010.iloc[2200:2700,[5,8]].values
-        te = np.zeros(24)
-        for lag in range(1,25):
-        	te[lag-1] = transent(data[:,0],data[:,1],lag)
-        	str = "TE from pressure to PM2.5 at %d hours lag : %f" %(lag,te[lag-1])
-        	print(str)
-        ```
-        
-        ##### multivariate normality test
-        ```python
-        from numpy.random import multivariate_normal as mnorm
-        from copent import mvnt
-        mean1 = [0,0]
-        cov1 = [[1,0.65],[0.65,1]]
-        data = mnorm(mean1, cov1, 500)
-        stat1 = mvnt(data)
-        ```
-        
-        ##### two-sample test
-        ```python
-        from copent import tst
-        from numpy import zeros
-        from numpy.random import multivariate_normal as mnorm
-        m0 = [0,0]
-        rho1 = 0.5
-        v0 = [[1,rho1],[rho1,1]]
-        s0 = mnorm(m0, v0, 400) # bivariate gaussian 
-        stat1 = zeros(9)
-        for i in range(0,9):
-        	m1 = [i,i]
-        	s1 = mnorm(m1,v0,500)
-        	stat1[i] = tst(s0,s1)
-        	print(stat1[i])
-        ```
-        
-        ##### change point detection
-        ```python
-        from copent import mcpd
-        import numpy as np
-        from numpy.random import multivariate_normal as mnorm
-        
-        n1 = 50
-        x1 = np.random.normal(0,1,n1)
-        x2 = np.random.normal(5,1,n1)
-        x3 = np.random.normal(10,1,n1)
-        x4 = np.random.normal(1,1,n1)
-        x = np.concatenate((x1,x2,x3,x4))
-        pos,maxstat = mcpd(x,thd =0.2)
-        print(pos)
-        
-        x1 = mnorm([0,0],[[1,0],[0,1]],n1)
-        x2 = mnorm([10,10],[[1,0],[0,1]],n1)
-        x3 = mnorm([5,5],[[1,0],[0,1]],n1)
-        x4 = mnorm([1,1],[[1,0],[0,1]],n1)
-        x = np.concatenate((x1,x2,x3,x4))
-        pos,maxstat = mcpd(x,thd =0.2)
-        print(pos)
-        ```
-        
-        #### References
-        1. Jian Ma and Zengqi Sun. Mutual information is copula entropy. Tsinghua Science & Technology, 2011, 16(1): 51-54. See also arXiv preprint arXiv:0808.0845, 2008.
-        2. Jian Ma. Estimating Transfer Entropy via Copula Entropy. arXiv preprint arXiv:1910.04375, 2019.
-        3. Jian Ma. Multivariate Normality Test with Copula Entropy. arXiv preprint arXiv:2206.05956, 2022.
-        4. Jian Ma. Two-Sample Test with Copula Entropy. arXiv preprint arXiv:2307.07247, 2023.
-        5. Jian Ma. Change Point Detection with Copula Entropy based Two-Sample Test. DOI:10.13140/RG.2.2.16378.26562, 2024.
-        
-        
 Platform: UNKNOWN
 Requires-Python: >=2.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![PyPI version](https://badge.fury.io/py/copent.svg)](https://pypi.org/project/copent)
+# copent
+Estimating Copula Entropy and Transfer Entropy
+
+#### Introduction
+The nonparametric methods for estimating copula entropy, transfer entropy, and the statistics for multivariate normality test and two-sample test are implemented. The change point detection method based on this two-sample test is also implemented.
+
+The method for estimating copula entropy composes of two simple steps: estimating empirical copula by rank statistic and estimating copula entropy with the KSG method. Copula Entropy is a mathematical concept for multivariate statistical independence measuring and testing, and proved to be equivalent to mutual information. Different from Pearson Correlation Coefficient, Copula Entropy is defined for non-linear, high-order and multivariate cases, which makes it universally applicable. Estimating copula entropy can be applied to many cases, including but not limited to variable selection and causal discovery (by estimating transfer entropy). Please refer to Ma and Sun (2011) <[doi:10.1016/S1007-0214(11)70008-6](http://www.doi.org/10.1016/S1007-0214(11)70008-6)> for more information.
+
+The nonparametric method for estimating transfer entropy composes of two steps: estimating three copula entropy and calculating transfer entropy from the estimated copula entropies. A function for conditional independence testing is also provided. Please refer to Ma (2019) <[arXiv:1910.04375](https://arxiv.org/abs/1910.04375)> for more information.
+
+The copula entropy based statistics for multivariate normality test and two-sample test are implemented. The change point detection method based on this two-sample test is also implemented. Please refer to Ma (2022) <[arXiv:2206.05956](https://arxiv.org/abs/2206.05956)>, Ma (2023) <[arXiv:2307.07247](https://arxiv.org/abs/2307.07247)>, and Ma (2024) <[arXiv:2403.07892](https://arxiv.org/abs/2403.07892)> for more details. 
+
+#### Functions
+* copent -- estimating copula entropy;
+* construct_empirical_copula -- the first step of the copent function, which estimates empirical copula for data by rank statistics;
+* entknn -- the second step of the copent function, which estimates copula entropy from empirical copula with kNN method;
+* ci -- conditional independence testing based on copula entropy 
+* transent -- estimating transfer entropy via copula entropy
+* mvnt -- estimating the copula entropy-based statistic for multivariate normality test
+* tst -- estimating the copula entropy-based statistic for two-sample test
+* cpd -- single change point detection
+* mcpd -- multiple change point detection
+
+#### Parameters
+* x: N * d data, N samples, d dimensions
+* k: kth nearest neighbour, parameter for kNN entropy estimation. default = 3
+* dtype: distance type, can be 'euclidean' or 'chebychev' (for Maximum Distance)
+* lag: time lag. default = 1
+* s0,s1: two samples with same dimension
+* n: repeat time of estimation
+* thd	: threshold for the statistic of two-sample test
+* maxp	: maximal number of change points
+* minseglen : minimal length of binary segmentation
+
+#### Installation
+The package can be installed from PyPI directly:
+```
+pip install copent
+```
+The package can be installed from Github:
+```
+pip install git+https://github.com/majianthu/pycopent.git
+```
+#### Usage Examples
+##### estimating copula entropy 
+```python
+from numpy.random import multivariate_normal as mnorm
+import copent
+rho = 0.6
+mean1 = [0,0]
+cov1 = [ [1,rho],[rho,1] ]
+x = mnorm(mean1,cov1,200) # bivariate gaussian 
+ce1 = copent.copent(x) # estimated copula entropy
+```
+
+##### estimating transfer entropy 
+```python
+from copent import transent
+from pandas import read_csv
+import numpy as np
+url = "https://archive.ics.uci.edu/ml/machine-learning-databases/00381/PRSA_data_2010.1.1-2014.12.31.csv"
+prsa2010 = read_csv(url)
+# index: 5(PM2.5),6(Dew Point),7(Temperature),8(Pressure),10(Cumulative Wind Speed)
+data = prsa2010.iloc[2200:2700,[5,8]].values
+te = np.zeros(24)
+for lag in range(1,25):
+	te[lag-1] = transent(data[:,0],data[:,1],lag)
+	str = "TE from pressure to PM2.5 at %d hours lag : %f" %(lag,te[lag-1])
+	print(str)
+```
+
+##### multivariate normality test
+```python
+from numpy.random import multivariate_normal as mnorm
+from copent import mvnt
+mean1 = [0,0]
+cov1 = [[1,0.65],[0.65,1]]
+data = mnorm(mean1, cov1, 500)
+stat1 = mvnt(data)
+```
+
+##### two-sample test
+```python
+from copent import tst
+from numpy import zeros
+from numpy.random import multivariate_normal as mnorm
+m0 = [0,0]
+rho1 = 0.5
+v0 = [[1,rho1],[rho1,1]]
+s0 = mnorm(m0, v0, 400) # bivariate gaussian 
+stat1 = zeros(9)
+for i in range(0,9):
+	m1 = [i,i]
+	s1 = mnorm(m1,v0,500)
+	stat1[i] = tst(s0,s1)
+	print(stat1[i])
+```
+
+##### change point detection
+```python
+from copent import mcpd
+import numpy as np
+from numpy.random import multivariate_normal as mnorm
+
+n1 = 50
+x1 = np.random.normal(0,1,n1)
+x2 = np.random.normal(5,1,n1)
+x3 = np.random.normal(10,1,n1)
+x4 = np.random.normal(1,1,n1)
+x = np.concatenate((x1,x2,x3,x4))
+pos,maxstat = mcpd(x,thd =0.2)
+print(pos)
+
+x1 = mnorm([0,0],[[1,0],[0,1]],n1)
+x2 = mnorm([10,10],[[1,0],[0,1]],n1)
+x3 = mnorm([5,5],[[1,0],[0,1]],n1)
+x4 = mnorm([1,1],[[1,0],[0,1]],n1)
+x = np.concatenate((x1,x2,x3,x4))
+pos,maxstat = mcpd(x,thd =0.2)
+print(pos)
+```
+
+#### References
+1. Jian Ma and Zengqi Sun. Mutual information is copula entropy. Tsinghua Science & Technology, 2011, 16(1): 51-54. See also arXiv preprint arXiv:0808.0845, 2008.
+2. Jian Ma. Estimating Transfer Entropy via Copula Entropy. arXiv preprint arXiv:1910.04375, 2019.
+3. Jian Ma. Multivariate Normality Test with Copula Entropy. arXiv preprint arXiv:2206.05956, 2022.
+4. Jian Ma. Two-Sample Test with Copula Entropy. arXiv preprint arXiv:2307.07247, 2023.
+5. Jian Ma. Change Point Detection with Copula Entropy based Two-Sample Test. arXiv preprint arXiv:2403.07892, 2024.
+
+
+
```

### Comparing `copent-0.5.1/setup.py` & `copent-0.5.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="copent",
-    version="0.5.1",
+    version="0.5.2",
     author="MA Jian",
     author_email="majian03@gmail.com",
     description="Estimating Copula Entropy and Transfer Entropy",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license = 'GPL License',
     url="https://github.com/majianthu/pycopent",
```

