# Comparing `tmp/foveatorch-0.1.2.tar.gz` & `tmp/foveatorch-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foveatorch-0.1.2.tar", last modified: Sun Jul  2 23:09:37 2023, max compression
+gzip compressed data, was "foveatorch-0.1.3.tar", last modified: Mon May 27 21:37:28 2024, max compression
```

## Comparing `foveatorch-0.1.2.tar` & `foveatorch-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:09:37.826476 foveatorch-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-02 23:09:23.000000 foveatorch-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-07-02 23:09:37.826476 foveatorch-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-02 23:09:23.000000 foveatorch-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:09:37.826476 foveatorch-0.1.2/foveatorch/
--rwxr-xr-x   0 runner    (1001) docker     (123)      651 2023-07-02 23:09:23.000000 foveatorch-0.1.2/foveatorch/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8494 2023-07-02 23:09:23.000000 foveatorch-0.1.2/foveatorch/modfoveate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9103 2023-07-02 23:09:23.000000 foveatorch-0.1.2/foveatorch/neopyramid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:09:37.826476 foveatorch-0.1.2/foveatorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-07-02 23:09:37.000000 foveatorch-0.1.2/foveatorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-02 23:09:37.000000 foveatorch-0.1.2/foveatorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 23:09:37.000000 foveatorch-0.1.2/foveatorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 23:09:37.000000 foveatorch-0.1.2/foveatorch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-02 23:09:37.000000 foveatorch-0.1.2/foveatorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 23:09:37.826476 foveatorch-0.1.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2207 2023-07-02 23:09:23.000000 foveatorch-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:37:28.489390 foveatorch-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-27 21:37:23.000000 foveatorch-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-27 21:37:28.489390 foveatorch-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-27 21:37:23.000000 foveatorch-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:37:28.489390 foveatorch-0.1.3/foveatorch/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      651 2024-05-27 21:37:23.000000 foveatorch-0.1.3/foveatorch/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8494 2024-05-27 21:37:23.000000 foveatorch-0.1.3/foveatorch/modfoveate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9103 2024-05-27 21:37:23.000000 foveatorch-0.1.3/foveatorch/neopyramid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:37:28.489390 foveatorch-0.1.3/foveatorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-27 21:37:28.000000 foveatorch-0.1.3/foveatorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-27 21:37:28.000000 foveatorch-0.1.3/foveatorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 21:37:28.000000 foveatorch-0.1.3/foveatorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 21:37:28.000000 foveatorch-0.1.3/foveatorch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-27 21:37:28.000000 foveatorch-0.1.3/foveatorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-27 21:37:28.000000 foveatorch-0.1.3/foveatorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 21:37:28.489390 foveatorch-0.1.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1744 2024-05-27 21:37:23.000000 foveatorch-0.1.3/setup.py
```

### Comparing `foveatorch-0.1.2/LICENSE` & `foveatorch-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `foveatorch-0.1.2/PKG-INFO` & `foveatorch-0.1.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: foveatorch
-Version: 0.1.2
+Version: 0.1.3
 Summary: Differentiable foveated vision for Deep Learning methods
 Home-page: https://github.com/emaballarin/foveatorch
 Author: Emanuele Ballarin
 Author-email: emanuele@ballarin.cc
 License: MIT
 Keywords: Deep Learning,Machine Learning,Computer Vision,Computational Neuroscience,Differentiable Programming
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: torch>=2
+Requires-Dist: kornia>=0.6.12
 
 # `FoveaTorch` 👀🔥 <a href="https://bucket.ballarin.cc/serve/img/foveatorch_dalle2.png"><img src="https://bucket.ballarin.cc/serve/img/foveatorch_dalle2.png" align="right" height="139" /></a>
 
 Differentiable foveated vision for Deep Learning methods
 
 ---
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: foveatorch Version: 0.1.2 Summary: Differentiable
+Metadata-Version: 2.1 Name: foveatorch Version: 0.1.3 Summary: Differentiable
 foveated vision for Deep Learning methods Home-page: https://github.com/
 emaballarin/foveatorch Author: Emanuele Ballarin Author-email:
 emanuele@ballarin.cc License: MIT Keywords: Deep Learning,Machine
 Learning,Computer Vision,Computational Neuroscience,Differentiable Programming
 Classifier: Development Status :: 4 - Beta Classifier: Topic :: Scientific/
 Engineering :: Artificial Intelligence Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Requires-Python: >=3.10 Description-Content-Type: text/
-markdown License-File: LICENSE # `FoveaTorch` ðð¥ _[_h_t_t_p_s_:_/_/
-_b_u_c_k_e_t_._b_a_l_l_a_r_i_n_._c_c_/_s_e_r_v_e_/_i_m_g_/_f_o_v_e_a_t_o_r_c_h___d_a_l_l_e_2_._p_n_g_]Differentiable foveated
-vision for Deep Learning methods --- ### References - [J.S. Perry and W.S.
-Geisler, "Gaze-contingent real-time simulation of arbitrary visual fields",
-IS&T/SPIE Electronic Imaging, 2002](https://sci-hub.ru/10.1117/12.469554) - [M.
-Jiang, S. Huang, J. Duan and Q. Zhao, "SALICON: Saliency in Context", IEEE
-Conference on Computer Vision and Pattern Recognition, 2015](https://sci-
-hub.ru/10.1109/CVPR.2015.7298710) - [Zhibo Yang, "Image_Foveation_Python:
-Python implementation of image retina transformation"](https://github.com/
-ouyangzhibo/Image_Foveation_Python)
+markdown License-File: LICENSE Requires-Dist: torch>=2 Requires-Dist:
+kornia>=0.6.12 # `FoveaTorch` ðð¥ _[_h_t_t_p_s_:_/_/_b_u_c_k_e_t_._b_a_l_l_a_r_i_n_._c_c_/_s_e_r_v_e_/_i_m_g_/
+_f_o_v_e_a_t_o_r_c_h___d_a_l_l_e_2_._p_n_g_]Differentiable foveated vision for Deep Learning methods
+--- ### References - [J.S. Perry and W.S. Geisler, "Gaze-contingent real-time
+simulation of arbitrary visual fields", IS&T/SPIE Electronic Imaging, 2002]
+(https://sci-hub.ru/10.1117/12.469554) - [M. Jiang, S. Huang, J. Duan and Q.
+Zhao, "SALICON: Saliency in Context", IEEE Conference on Computer Vision and
+Pattern Recognition, 2015](https://sci-hub.ru/10.1109/CVPR.2015.7298710) -
+[Zhibo Yang, "Image_Foveation_Python: Python implementation of image retina
+transformation"](https://github.com/ouyangzhibo/Image_Foveation_Python)
```

### Comparing `foveatorch-0.1.2/README.md` & `foveatorch-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `foveatorch-0.1.2/foveatorch/__init__.py` & `foveatorch-0.1.3/foveatorch/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # ------------------------------------------------------------------------------
 #
-#  Copyright (c) 2023 Emanuele Ballarin <emanuele@ballarin.cc>
+#  Copyright (c) 2024 Emanuele Ballarin <emanuele@ballarin.cc>
 #  Released under the terms of the MIT License
 #  (see: https://url.ballarin.cc/mitlicense)
 #
 # ------------------------------------------------------------------------------
 # Imports
 from .modfoveate import foveate
 from .modfoveate import Foveate2D
```

### Comparing `foveatorch-0.1.2/foveatorch/modfoveate.py` & `foveatorch-0.1.3/foveatorch/modfoveate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # ------------------------------------------------------------------------------
 #
 #  Copyright (c) 2018-2023 Zhibo Yang (CV2/NumPy original,
 #                see: https://github.com/ouyangzhibo/Image_Foveation_Python/blob/master/retina_transform.py)
-#            (c) 2023 Emanuele Ballarin <emanuele@ballarin.cc>
+#            (c) 2024 Emanuele Ballarin <emanuele@ballarin.cc>
 #
 #  Originally released under the terms of the MIT License
 #  (see: https://github.com/ouyangzhibo/Image_Foveation_Python/blob/master/LICENSE)
 #
 #  Released under the terms of the MIT License
 #  (see: https://url.ballarin.cc/mitlicense)
 #
```

### Comparing `foveatorch-0.1.2/foveatorch/neopyramid.py` & `foveatorch-0.1.3/foveatorch/neopyramid.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # ------------------------------------------------------------------------------
 #
 #  Copyright (c) 2018-2023 The Kornia Developers (original implementation,
 #                see: https://github.com/kornia/kornia/blob/master/kornia/geometry/transform/pyramid.py)
-#            (c) 2023 Emanuele Ballarin <emanuele@ballarin.cc>
+#            (c) 2024 Emanuele Ballarin <emanuele@ballarin.cc>
 #
 #  Originally released under the terms of the Apache License, Version 2.0
 #  (see: https://github.com/kornia/kornia/blob/master/LICENSE)
 #
 #  Released under the terms of the MIT License
 #  (see: https://url.ballarin.cc/mitlicense)
 #
```

### Comparing `foveatorch-0.1.2/foveatorch.egg-info/PKG-INFO` & `foveatorch-0.1.3/foveatorch.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: foveatorch
-Version: 0.1.2
+Version: 0.1.3
 Summary: Differentiable foveated vision for Deep Learning methods
 Home-page: https://github.com/emaballarin/foveatorch
 Author: Emanuele Ballarin
 Author-email: emanuele@ballarin.cc
 License: MIT
 Keywords: Deep Learning,Machine Learning,Computer Vision,Computational Neuroscience,Differentiable Programming
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: torch>=2
+Requires-Dist: kornia>=0.6.12
 
 # `FoveaTorch` 👀🔥 <a href="https://bucket.ballarin.cc/serve/img/foveatorch_dalle2.png"><img src="https://bucket.ballarin.cc/serve/img/foveatorch_dalle2.png" align="right" height="139" /></a>
 
 Differentiable foveated vision for Deep Learning methods
 
 ---
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: foveatorch Version: 0.1.2 Summary: Differentiable
+Metadata-Version: 2.1 Name: foveatorch Version: 0.1.3 Summary: Differentiable
 foveated vision for Deep Learning methods Home-page: https://github.com/
 emaballarin/foveatorch Author: Emanuele Ballarin Author-email:
 emanuele@ballarin.cc License: MIT Keywords: Deep Learning,Machine
 Learning,Computer Vision,Computational Neuroscience,Differentiable Programming
 Classifier: Development Status :: 4 - Beta Classifier: Topic :: Scientific/
 Engineering :: Artificial Intelligence Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Requires-Python: >=3.10 Description-Content-Type: text/
-markdown License-File: LICENSE # `FoveaTorch` ðð¥ _[_h_t_t_p_s_:_/_/
-_b_u_c_k_e_t_._b_a_l_l_a_r_i_n_._c_c_/_s_e_r_v_e_/_i_m_g_/_f_o_v_e_a_t_o_r_c_h___d_a_l_l_e_2_._p_n_g_]Differentiable foveated
-vision for Deep Learning methods --- ### References - [J.S. Perry and W.S.
-Geisler, "Gaze-contingent real-time simulation of arbitrary visual fields",
-IS&T/SPIE Electronic Imaging, 2002](https://sci-hub.ru/10.1117/12.469554) - [M.
-Jiang, S. Huang, J. Duan and Q. Zhao, "SALICON: Saliency in Context", IEEE
-Conference on Computer Vision and Pattern Recognition, 2015](https://sci-
-hub.ru/10.1109/CVPR.2015.7298710) - [Zhibo Yang, "Image_Foveation_Python:
-Python implementation of image retina transformation"](https://github.com/
-ouyangzhibo/Image_Foveation_Python)
+markdown License-File: LICENSE Requires-Dist: torch>=2 Requires-Dist:
+kornia>=0.6.12 # `FoveaTorch` ðð¥ _[_h_t_t_p_s_:_/_/_b_u_c_k_e_t_._b_a_l_l_a_r_i_n_._c_c_/_s_e_r_v_e_/_i_m_g_/
+_f_o_v_e_a_t_o_r_c_h___d_a_l_l_e_2_._p_n_g_]Differentiable foveated vision for Deep Learning methods
+--- ### References - [J.S. Perry and W.S. Geisler, "Gaze-contingent real-time
+simulation of arbitrary visual fields", IS&T/SPIE Electronic Imaging, 2002]
+(https://sci-hub.ru/10.1117/12.469554) - [M. Jiang, S. Huang, J. Duan and Q.
+Zhao, "SALICON: Saliency in Context", IEEE Conference on Computer Vision and
+Pattern Recognition, 2015](https://sci-hub.ru/10.1109/CVPR.2015.7298710) -
+[Zhibo Yang, "Image_Foveation_Python: Python implementation of image retina
+transformation"](https://github.com/ouyangzhibo/Image_Foveation_Python)
```

