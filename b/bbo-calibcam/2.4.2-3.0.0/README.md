# Comparing `tmp/bbo-calibcam-2.4.2.tar.gz` & `tmp/bbo-calibcam-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbo-calibcam-2.4.2.tar", last modified: Fri May 17 06:55:01 2024, max compression
+gzip compressed data, was "bbo-calibcam-3.0.0.tar", last modified: Mon May 27 13:58:13 2024, max compression
```

## Comparing `bbo-calibcam-2.4.2.tar` & `bbo-calibcam-3.0.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 voit     (86501) voit     (86501)        0 2024-05-17 06:55:01.443957 bbo-calibcam-2.4.2/
--rw-rw-r--   0 voit     (86501) voit     (86501)    25314 2023-11-13 15:21:57.000000 bbo-calibcam-2.4.2/LICENSE
--rw-rw-r--   0 voit     (86501) voit     (86501)     2969 2024-05-17 06:55:01.443957 bbo-calibcam-2.4.2/PKG-INFO
--rw-rw-r--   0 voit     (86501) voit     (86501)     2486 2024-05-06 12:58:51.000000 bbo-calibcam-2.4.2/README.md
-drwxrwxr-x   0 voit     (86501) voit     (86501)        0 2024-05-17 06:55:01.429957 bbo-calibcam-2.4.2/bbo_calibcam.egg-info/
--rw-rw-r--   0 voit     (86501) voit     (86501)     2969 2024-05-17 06:55:01.000000 bbo-calibcam-2.4.2/bbo_calibcam.egg-info/PKG-INFO
--rw-rw-r--   0 voit     (86501) voit     (86501)      725 2024-05-17 06:55:01.000000 bbo-calibcam-2.4.2/bbo_calibcam.egg-info/SOURCES.txt
--rw-rw-r--   0 voit     (86501) voit     (86501)        1 2024-05-17 06:55:01.000000 bbo-calibcam-2.4.2/bbo_calibcam.egg-info/dependency_links.txt
--rw-rw-r--   0 voit     (86501) voit     (86501)       82 2024-05-17 06:55:01.000000 bbo-calibcam-2.4.2/bbo_calibcam.egg-info/requires.txt
--rw-rw-r--   0 voit     (86501) voit     (86501)        9 2024-05-17 06:55:01.000000 bbo-calibcam-2.4.2/bbo_calibcam.egg-info/top_level.txt
-drwxrwxr-x   0 voit     (86501) voit     (86501)        0 2024-05-17 06:55:01.442957 bbo-calibcam-2.4.2/calibcam/
--rw-rw-r--   0 voit     (86501) voit     (86501)       21 2023-11-13 15:21:57.000000 bbo-calibcam-2.4.2/calibcam/__init__.py
--rwxrwxr-x   0 voit     (86501) voit     (86501)     6939 2024-04-03 11:11:24.000000 bbo-calibcam-2.4.2/calibcam/__main__.py
--rw-rw-r--   0 voit     (86501) voit     (86501)     2177 2024-05-07 16:01:22.000000 bbo-calibcam-2.4.2/calibcam/board.py
--rw-rw-r--   0 voit     (86501) voit     (86501)     6562 2024-04-03 11:11:24.000000 bbo-calibcam-2.4.2/calibcam/calibrator_opts.py
--rw-rw-r--   0 voit     (86501) voit     (86501)    28647 2024-05-08 13:28:24.000000 bbo-calibcam-2.4.2/calibcam/camcalibrator.py
--rw-rw-r--   0 voit     (86501) voit     (86501)     7387 2024-02-21 09:07:16.000000 bbo-calibcam-2.4.2/calibcam/camfunctions.py
--rw-rw-r--   0 voit     (86501) voit     (86501)     3413 2023-11-13 15:21:57.000000 bbo-calibcam-2.4.2/calibcam/camfunctions_ag.py
--rw-rw-r--   0 voit     (86501) voit     (86501)     1500 2023-11-13 15:21:57.000000 bbo-calibcam-2.4.2/calibcam/compatibility.py
--rw-rw-r--   0 voit     (86501) voit     (86501)     7828 2024-03-08 12:23:55.000000 bbo-calibcam-2.4.2/calibcam/detection.py
--rw-rw-r--   0 voit     (86501) voit     (86501)      110 2023-11-13 15:21:57.000000 bbo-calibcam-2.4.2/calibcam/exceptions.py
--rw-rw-r--   0 voit     (86501) voit     (86501)     8574 2024-02-21 09:07:16.000000 bbo-calibcam-2.4.2/calibcam/helper.py
--rw-rw-r--   0 voit     (86501) voit     (86501)     2128 2023-11-13 15:21:57.000000 bbo-calibcam-2.4.2/calibcam/helper_ag.py
-drwxrwxr-x   0 voit     (86501) voit     (86501)        0 2024-05-17 06:55:01.442957 bbo-calibcam-2.4.2/calibcam/opt_jacfwd/
--rw-rw-r--   0 voit     (86501) voit     (86501)        0 2023-11-13 15:21:57.000000 bbo-calibcam-2.4.2/calibcam/opt_jacfwd/__init__.py
--rw-rw-r--   0 voit     (86501) voit     (86501)     4283 2023-12-20 15:01:17.000000 bbo-calibcam-2.4.2/calibcam/opt_jacfwd/optfunctions.py
--rw-rw-r--   0 voit     (86501) voit     (86501)     2067 2023-11-13 15:21:57.000000 bbo-calibcam-2.4.2/calibcam/opt_jacfwd/optfunctions_ag.py
--rw-rw-r--   0 voit     (86501) voit     (86501)     7496 2023-12-20 15:01:17.000000 bbo-calibcam-2.4.2/calibcam/optimization.py
--rw-rw-r--   0 voit     (86501) voit     (86501)     5724 2023-11-13 15:21:57.000000 bbo-calibcam-2.4.2/calibcam/pose_estimation.py
--rw-rw-r--   0 voit     (86501) voit     (86501)     3731 2024-03-11 13:54:23.000000 bbo-calibcam-2.4.2/calibcam/single_camcalibration.py
--rw-rw-r--   0 voit     (86501) voit     (86501)      749 2024-04-03 12:26:54.000000 bbo-calibcam-2.4.2/calibcam/yaml_helper.py
--rw-rw-r--   0 voit     (86501) voit     (86501)       38 2024-05-17 06:55:01.443957 bbo-calibcam-2.4.2/setup.cfg
--rw-rw-r--   0 voit     (86501) voit     (86501)     1024 2024-05-17 06:54:49.000000 bbo-calibcam-2.4.2/setup.py
-drwxrwxr-x   0 voit     (86501) voit     (86501)        0 2024-05-17 06:55:01.443957 bbo-calibcam-2.4.2/test/
--rw-rw-r--   0 voit     (86501) voit     (86501)     3290 2024-02-21 15:41:26.000000 bbo-calibcam-2.4.2/test/test_detection.py
+drwxrwxr-x   0 voit     (86501) voit     (86501)        0 2024-05-27 13:58:13.792453 bbo-calibcam-3.0.0/
+-rw-rw-r--   0 voit     (86501) voit     (86501)    25314 2023-11-13 15:21:57.000000 bbo-calibcam-3.0.0/LICENSE
+-rw-rw-r--   0 voit     (86501) voit     (86501)     2969 2024-05-27 13:58:13.792453 bbo-calibcam-3.0.0/PKG-INFO
+-rw-rw-r--   0 voit     (86501) voit     (86501)     2486 2024-05-06 12:58:51.000000 bbo-calibcam-3.0.0/README.md
+drwxrwxr-x   0 voit     (86501) voit     (86501)        0 2024-05-27 13:58:13.789453 bbo-calibcam-3.0.0/bbo_calibcam.egg-info/
+-rw-rw-r--   0 voit     (86501) voit     (86501)     2969 2024-05-27 13:58:13.000000 bbo-calibcam-3.0.0/bbo_calibcam.egg-info/PKG-INFO
+-rw-rw-r--   0 voit     (86501) voit     (86501)      710 2024-05-27 13:58:13.000000 bbo-calibcam-3.0.0/bbo_calibcam.egg-info/SOURCES.txt
+-rw-rw-r--   0 voit     (86501) voit     (86501)        1 2024-05-27 13:58:13.000000 bbo-calibcam-3.0.0/bbo_calibcam.egg-info/dependency_links.txt
+-rw-rw-r--   0 voit     (86501) voit     (86501)       90 2024-05-27 13:58:13.000000 bbo-calibcam-3.0.0/bbo_calibcam.egg-info/requires.txt
+-rw-rw-r--   0 voit     (86501) voit     (86501)        9 2024-05-27 13:58:13.000000 bbo-calibcam-3.0.0/bbo_calibcam.egg-info/top_level.txt
+drwxrwxr-x   0 voit     (86501) voit     (86501)        0 2024-05-27 13:58:13.791453 bbo-calibcam-3.0.0/calibcam/
+-rw-rw-r--   0 voit     (86501) voit     (86501)       21 2023-11-13 15:21:57.000000 bbo-calibcam-3.0.0/calibcam/__init__.py
+-rwxrwxr-x   0 voit     (86501) voit     (86501)     7595 2024-05-27 13:56:50.000000 bbo-calibcam-3.0.0/calibcam/__main__.py
+-rw-rw-r--   0 voit     (86501) voit     (86501)     2082 2024-05-27 13:56:50.000000 bbo-calibcam-3.0.0/calibcam/board.py
+-rw-rw-r--   0 voit     (86501) voit     (86501)     7124 2024-05-27 13:56:50.000000 bbo-calibcam-3.0.0/calibcam/calibrator_opts.py
+-rw-rw-r--   0 voit     (86501) voit     (86501)    29334 2024-05-27 13:56:50.000000 bbo-calibcam-3.0.0/calibcam/camcalibrator.py
+-rw-rw-r--   0 voit     (86501) voit     (86501)     7325 2024-05-27 13:56:50.000000 bbo-calibcam-3.0.0/calibcam/camfunctions.py
+-rw-rw-r--   0 voit     (86501) voit     (86501)     3413 2023-11-13 15:21:57.000000 bbo-calibcam-3.0.0/calibcam/camfunctions_ag.py
+-rw-rw-r--   0 voit     (86501) voit     (86501)     1500 2023-11-13 15:21:57.000000 bbo-calibcam-3.0.0/calibcam/compatibility.py
+-rw-rw-r--   0 voit     (86501) voit     (86501)     8296 2024-05-27 13:56:50.000000 bbo-calibcam-3.0.0/calibcam/detection.py
+-rw-rw-r--   0 voit     (86501) voit     (86501)      110 2023-11-13 15:21:57.000000 bbo-calibcam-3.0.0/calibcam/exceptions.py
+-rw-rw-r--   0 voit     (86501) voit     (86501)     8574 2024-02-21 09:07:16.000000 bbo-calibcam-3.0.0/calibcam/helper.py
+-rw-rw-r--   0 voit     (86501) voit     (86501)     2128 2023-11-13 15:21:57.000000 bbo-calibcam-3.0.0/calibcam/helper_ag.py
+-rw-rw-r--   0 voit     (86501) voit     (86501)     8066 2024-05-27 13:56:50.000000 bbo-calibcam-3.0.0/calibcam/optimization.py
+-rw-rw-r--   0 voit     (86501) voit     (86501)     6567 2024-05-27 13:56:50.000000 bbo-calibcam-3.0.0/calibcam/pose_estimation.py
+drwxrwxr-x   0 voit     (86501) voit     (86501)        0 2024-05-27 13:58:13.792453 bbo-calibcam-3.0.0/calibcam/repro/
+-rw-rw-r--   0 voit     (86501) voit     (86501)        0 2024-05-27 13:56:50.000000 bbo-calibcam-3.0.0/calibcam/repro/__init__.py
+-rw-rw-r--   0 voit     (86501) voit     (86501)     8639 2024-05-27 13:56:50.000000 bbo-calibcam-3.0.0/calibcam/repro/optfunctions.py
+-rw-rw-r--   0 voit     (86501) voit     (86501)     2067 2024-05-27 13:56:50.000000 bbo-calibcam-3.0.0/calibcam/repro/optfunctions_ag.py
+-rw-rw-r--   0 voit     (86501) voit     (86501)     3731 2024-03-11 13:54:23.000000 bbo-calibcam-3.0.0/calibcam/single_camcalibration.py
+-rw-rw-r--   0 voit     (86501) voit     (86501)      749 2024-04-03 12:26:54.000000 bbo-calibcam-3.0.0/calibcam/yaml_helper.py
+-rw-rw-r--   0 voit     (86501) voit     (86501)       38 2024-05-27 13:58:13.792453 bbo-calibcam-3.0.0/setup.cfg
+-rw-rw-r--   0 voit     (86501) voit     (86501)     1057 2024-05-27 13:56:50.000000 bbo-calibcam-3.0.0/setup.py
+drwxrwxr-x   0 voit     (86501) voit     (86501)        0 2024-05-27 13:58:13.792453 bbo-calibcam-3.0.0/test/
+-rw-rw-r--   0 voit     (86501) voit     (86501)     3290 2024-02-21 15:41:26.000000 bbo-calibcam-3.0.0/test/test_detection.py
```

### Comparing `bbo-calibcam-2.4.2/LICENSE` & `bbo-calibcam-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bbo-calibcam-2.4.2/PKG-INFO` & `bbo-calibcam-3.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbo-calibcam
-Version: 2.4.2
+Version: 3.0.0
 Summary: Calibrate intrinsic and extrinsic parameters of cameras with charuco boards
 Home-page: https://github.com/bbo-lab/calibcam
 Author: BBO-lab @ caesar
 Author-email: kay-michael.voit@mpinb.mpg.de
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bbo-calibcam-2.4.2/README.md` & `bbo-calibcam-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `bbo-calibcam-2.4.2/bbo_calibcam.egg-info/PKG-INFO` & `bbo-calibcam-3.0.0/bbo_calibcam.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbo-calibcam
-Version: 2.4.2
+Version: 3.0.0
 Summary: Calibrate intrinsic and extrinsic parameters of cameras with charuco boards
 Home-page: https://github.com/bbo-lab/calibcam
 Author: BBO-lab @ caesar
 Author-email: kay-michael.voit@mpinb.mpg.de
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bbo-calibcam-2.4.2/bbo_calibcam.egg-info/SOURCES.txt` & `bbo-calibcam-3.0.0/bbo_calibcam.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -18,11 +18,11 @@
 calibcam/exceptions.py
 calibcam/helper.py
 calibcam/helper_ag.py
 calibcam/optimization.py
 calibcam/pose_estimation.py
 calibcam/single_camcalibration.py
 calibcam/yaml_helper.py
-calibcam/opt_jacfwd/__init__.py
-calibcam/opt_jacfwd/optfunctions.py
-calibcam/opt_jacfwd/optfunctions_ag.py
+calibcam/repro/__init__.py
+calibcam/repro/optfunctions.py
+calibcam/repro/optfunctions_ag.py
 test/test_detection.py
```

### Comparing `bbo-calibcam-2.4.2/calibcam/__main__.py` & `bbo-calibcam-3.0.0/calibcam/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import argparse
 import yaml
 import numpy as np
 from pathlib import Path
 
 from calibcam import calibrator_opts, helper, yaml_helper
 from calibcam.camcalibrator import CamCalibrator
+from calibcamlib import Camerasystem
 import timeit
 
 
 def main():
     print("Starting")
     tic = timeit.default_timer()
     # PArse command line arguments
@@ -36,14 +37,16 @@
     parser.add_argument('--numerical_jacobian', required=False, default=None, action="store_true", help="")
     # Other
     parser.add_argument('--pipelines', type=str, required=False, nargs='*', default=None,
                         help="Add pipeline readable by bbo-svidreader. "
                              "The final output of the pipeline is used for calibration.")
     parser.add_argument('--write_opts', type=str, required=False, nargs=1, default=[None], help="")
     parser.add_argument('--data_path', type=str, required=False, nargs=1, default=[None], help="")
+    parser.add_argument('--gamma_correction', required=False, default=False, action="store_true", help="")
+    parser.add_argument('--init_extrinsics', type=str, required=False, nargs=1, default=[None], help="")
 
     args = parser.parse_args()
 
     n_cams = len(args.videos)
 
     # Build options from defaults and --opts parameters TODO: Currently not functional for yml, implement helpers!
     opts = calibrator_opts.get_default_opts(n_cams)
@@ -75,14 +78,22 @@
     # Fill commandline options
     if args.optimize_only is not None:
         opts['optimize_only'] = args.optimize_only
     if args.numerical_jacobian is not None:
         opts['numerical_jacobian'] = args.numerical_jacobian
     if args.model:
         opts['models'] = args.model
+    if args.gamma_correction:
+        opts['gamma_correction'] = True
+    if args.init_extrinsics[0] is not None:
+        init_extrinsics = Camerasystem.load_dict(args.init_extrinsics[0])
+        opts['init_extrinsics'] = {
+            'rvecs_cam': np.array([c["rvec_cam"] for c in init_extrinsics['calibs']]),
+            'tvecs_cam': np.array([c["tvec_cam"] for c in init_extrinsics['calibs']])
+        }
 
     # It is necessary for the videos to be in sync to perform multi calibration. If some videos lag behind other videos,
     # start_frames_indexes should be provided to adjust for the lag.
     if args.start_frame_indexes is not None:
         assert len(args.start_frame_indexes) == n_cams, "number of start_frame_indexes " \
                                                                   "does not match number of videos!"
         opts['start_frame_indexes'] = np.array(args.start_frame_indexes)
```

### Comparing `bbo-calibcam-2.4.2/calibcam/board.py` & `bbo-calibcam-3.0.0/calibcam/board.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,20 +19,19 @@
     if board_params is not None:
         board_params['marker_size_real'] = board_params['square_size_real'] * board_params['marker_size']  # noqa
 
     return board_params
 
 
 def make_board(board_params):
-    board = cv2.aruco.CharucoBoard_create(board_params['boardWidth'],  # noqa
-                                          board_params['boardHeight'],
-                                          board_params['square_size_real'],
-                                          board_params['marker_size'] * board_params['square_size_real'],
-                                          cv2.aruco.getPredefinedDictionary(  # noqa
-                                              board_params['dictionary_type']))
+    board = cv2.aruco.CharucoBoard((board_params['boardWidth'],
+                                    board_params['boardHeight']),
+                                   board_params['square_size_real'],
+                                   board_params['marker_size'] * board_params['square_size_real'],
+                                   cv2.aruco.getPredefinedDictionary(board_params['dictionary_type']))
 
     return board
 
 
 def make_board_points(board_params, exact=False):
     board_width = board_params['boardWidth']
     board_height = board_params['boardHeight']
```

### Comparing `bbo-calibcam-2.4.2/calibcam/calibrator_opts.py` & `bbo-calibcam-3.0.0/calibcam/calibrator_opts.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,14 +48,19 @@
         'optimize_ind_cams': False,
         # Optimize individual board poses then all params again.
         # In a test, optimality was already reached after a first general optimization
         'optimize_board_poses': False,
         # In pixels. replace the pose with higher error and insert 'nearby' pose with lower
         # error while optimizing individual board poses.
         'max_allowed_res': 5.0,
+        # Use these extrinsics for initialization dict('rvecs_cam': nx3, 'tvecs_cam': nx3)
+        'init_extrinsics': {
+            'rvecs_cam': -1,
+            'tvecs_cam': -1,
+        },
 
         'detection_opts': {
             'inter_frame_dist': 1.0,  # In pixels
             'min_corners': 5,  # Minimum number of corners to detect in a frame
             'aruco_detect': {
                 'parameters': get_detector_parameters_opts(),
             },
@@ -82,16 +87,16 @@
         'optimization': {
             'method': 'trf',
             'ftol': 1e-9,
             'xtol': 1e-9,
             'gtol': 1e-9,
             'x_scale': 'jac',
             'loss': 'linear',
-            'tr_solver': 'exact',
-            'max_nfev': 120,
+            'tr_solver': 'lsmr',
+            'max_nfev': 500,
             'verbose': 2,
         }
     }
 
     if do_fill:
         fill(default_opts)
 
@@ -149,32 +154,40 @@
         flags = cv2.omnidir.CALIB_FIX_SKEW
 
     return flags
 
 
 def get_detector_parameters_opts():
     detector_parameters = {  # SPOT for detector params
-        'adaptiveThreshWinSizeMin': 15,
-        'adaptiveThreshWinSizeMax': 45,
-        'adaptiveThreshWinSizeStep': 5,
-
+        'adaptiveThreshWinSizeMin': 3,
+        'adaptiveThreshWinSizeMax': 23,
+        'adaptiveThreshWinSizeStep': 10,
         'cornerRefinementMethod': cv2.aruco.CORNER_REFINE_SUBPIX,
-        'cornerRefinementWinSize': 3,
-        'cornerRefinementMaxIterations': 60,
-        'cornerRefinementMinAccuracy': 0.05,
-
+        'cornerRefinementWinSize': 5,
+        'cornerRefinementMaxIterations': 30,
+        'cornerRefinementMinAccuracy': 0.01,
+        # 'adaptiveThreshWinSizeMin': 15,
+        # 'adaptiveThreshWinSizeMax': 45,
+        # 'adaptiveThreshWinSizeStep': 5,
+        #
+        # 'cornerRefinementMethod': cv2.aruco.CORNER_REFINE_SUBPIX,
+        # 'cornerRefinementWinSize': 3,
+        # 'cornerRefinementMaxIterations': 60,
+        # 'cornerRefinementMinAccuracy': 0.05,
+        #
         'errorCorrectionRate': 0.3,
         'perspectiveRemovePixelPerCell': 8
     }
     return detector_parameters
 
 
 def finalize_aruco_detector_opts(aruco_detect_opts):
     # Separation is necessary as cv2.aruco.DetectorParameters cannot be pickled
     opts = aruco_detect_opts.copy()
 
-    detector_parameters = cv2.aruco.DetectorParameters_create()
+    detector_parameters = cv2.aruco.DetectorParameters()
     for key, value in aruco_detect_opts['parameters'].items():
         detector_parameters.__setattr__(key, value)
+        # print(f"{key}: {value}")
 
     opts['parameters'] = detector_parameters
     return opts
```

### Comparing `bbo-calibcam-2.4.2/calibcam/camcalibrator.py` & `bbo-calibcam-3.0.0/calibcam/camcalibrator.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,17 +17,19 @@
 
 from calibcam.camfunctions import test_objective_function, make_optim_input
 from calibcam.detection import detect_corners
 from calibcam.exceptions import *
 from calibcam import helper, camfunctions, board, compatibility
 
 from calibcam.calibrator_opts import get_default_opts
-from calibcam.pose_estimation import estimate_cam_poses
+from calibcam.pose_estimation import estimate_cam_poses, build_initialized_calibs
 from calibcam.single_camcalibration import calibrate_single_camera
 
+from glob import glob
+
 from calibcam import yaml_helper
 
 
 class CamCalibrator:
     def __init__(self, recordings, pipelines=None, board_name=None, data_path=None, calibs_init=None, opts=None):
         if opts is None:
             opts = {}
@@ -136,14 +138,17 @@
         n_corners = (self.board_params["boardWidth"] - 1) * (self.board_params["boardHeight"] - 1)
         required_corner_idxs = [0,
                                 self.board_params["boardWidth"] - 2,
                                 (self.board_params["boardWidth"] - 1) * (self.board_params["boardHeight"] - 2),
                                 (self.board_params["boardWidth"] - 1) * (self.board_params["boardHeight"] - 1) - 1,
                                 ]  # Corners that we require to be detected for pose estimation
 
+        if not self.opts["detection"] and (self.opts["calibration_single"] or self.opts["calibration_multi"]):
+            self.opts["detection"] = sorted(glob(self.data_path + "/detection_*.yml"))
+
         # === Detection ===
         if isinstance(self.opts["detection"], list):
             # TODO: Support True in the list instead of strings to only detect individual cams
             assert len(self.opts["detection"]) == self.opts["n_cams"], ("Number of detection files must be equal "
                                                                         "to number of cameras")
 
             corners = []
@@ -187,14 +192,17 @@
                 with open(Path(self.data_path) / f"detection_{i_cam:03d}.yml", "w") as file:
                     yaml.dump(detection, file, default_flow_style=True)
         else:
             print("Cannot proceed without detections. Exiting.")
             return
 
         # === Single cam calibration ===
+        if not self.opts["calibration_single"] and self.opts["calibration_multi"]:
+            self.opts["calibration_single"] = sorted(glob(self.data_path + "/calibration_single_*.yml"))
+
         if isinstance(self.opts["calibration_single"], list):
             # TODO: Support True in the list instead of strings to only detect individual cams
             assert len(self.opts["calibration_single"]) == self.opts["n_cams"], ("Number of calibration_single files "
                                                                                  "must be equal to number of cameras")
             calibs_single = []
             for calibration_single_file in self.opts["calibration_single"]:
                 calibration_single_file = Path(calibration_single_file)
@@ -233,17 +241,22 @@
             save_path = Path(self.data_path) / f"calibration_single_{i_cam:03d}.yml"
             with open(save_path, "w") as file:
                 yaml.dump(yaml_helper.numpy_collection_to_list(calib_single), file, default_flow_style=True)
             # np.save(save_path.with_suffix(".npy"), calib_single, allow_pickle=True)
 
         # === Multi cam calibration ===
         if self.opts["calibration_multi"]:
-            # analytically estimate initial camera poses
-            calibs_multi = estimate_cam_poses(calibs_single, self.opts, corners=corners,
-                                              required_corner_idxs=required_corner_idxs)
+            if (isinstance(self.opts["init_extrinsics"]["rvecs_cam"], np.ndarray) and
+                    isinstance(self.opts["init_extrinsics"]["tvecs_cam"], np.ndarray)):
+                calibs_multi = build_initialized_calibs(calibs_single, self.opts, corners=corners,
+                                   required_corner_idxs=required_corner_idxs)
+            else:
+                # analytically estimate initial camera poses
+                calibs_multi = estimate_cam_poses(calibs_single, self.opts, corners=corners,
+                                                  required_corner_idxs=required_corner_idxs)
 
             if self.opts['debug']:
                 args, vars_free = make_optim_input(self.board_params, calibs_multi, corners, self.opts)
                 test_objective_function(calibs_multi, vars_free, args, corners, self.board_params,
                                         individual_poses=True)
 
             print('OPTIMIZING ALL POSES')
@@ -526,18 +539,14 @@
             result['info']['fun_final'] = min_result.fun
             result['info']['cost_val_final'] = min_result.cost
             result['info']['optimality_final'] = min_result.optimality
 
         return result
 
     def save_multicalibration(self, result, filename="multicam_calibration"):
-        # save
-        return self.save_multicalibration(filename, result)
-
-    def save_multicalibration(self, filename, result):
         data_path = self.data_path
         result_path = Path(data_path + '/' + filename)
         return save_multicalibration(result_path, result)
 
     # Debug function
     def plot(self, calibs, corners, used_frames_ids, board_params, cidx, fidx):
         import matplotlib.pyplot as plt
```

### Comparing `bbo-calibcam-2.4.2/calibcam/camfunctions.py` & `bbo-calibcam-3.0.0/calibcam/camfunctions.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         if verbose > 1 and opts['debug']:
             # This triggers JIT compilation
             jac(vars_free, args)
             # This times
             tic = timeit.default_timer()
             result = jac(vars_free, args)
             print(
-                f"Jacobian took {timeit.default_timer() - tic} s: squaresum {np.sum(result ** 2)} over {result.size} residuals. Shape {result.shape}.")
+                f"Jacobian took {timeit.default_timer() - tic} s. Shape {result.shape}.")
 
     if verbose > 1:
         print('Starting optimization procedure')
 
     min_result: OptimizeResult = least_squares(optimization.obj_fcn_wrapper,
                                                vars_free,
                                                jac=jac,
```

### Comparing `bbo-calibcam-2.4.2/calibcam/camfunctions_ag.py` & `bbo-calibcam-3.0.0/calibcam/camfunctions_ag.py`

 * *Files identical despite different names*

### Comparing `bbo-calibcam-2.4.2/calibcam/compatibility.py` & `bbo-calibcam-3.0.0/calibcam/compatibility.py`

 * *Files identical despite different names*

### Comparing `bbo-calibcam-2.4.2/calibcam/detection.py` & `bbo-calibcam-3.0.0/calibcam/detection.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,15 +33,17 @@
                                     rec_pipeline=rec_pipelines[i_rec])
         for i_rec, rec_file_name in enumerate(rec_file_names))
 
     for i_cam, detection in enumerate(detections):
         corners_all.append(detection[0])
         ids_all.append(detection[1])
         fin_frames_masks[i_cam, :] = detection[2][:fin_frames_masks.shape[1]]
-        print(f'Detected features in {np.sum(fin_frames_masks[i_cam]).astype(int):04d}  frames in camera {i_cam:02d}')
+        n_detections_cam = np.array([len(c) for c in corners_all[i_cam]])
+        print(f'Detected features in {np.sum(fin_frames_masks[i_cam]).astype(int):04d}  frames in camera {i_cam:02d} - '
+              f'({int(np.mean(n_detections_cam)):02d}±{int(np.std(n_detections_cam))})')
 
     if return_matrix:
         return helper.make_corners_array(corners_all, ids_all, (board_params["boardWidth"] - 1) * (
                 board_params["boardHeight"] - 1), fin_frames_masks), np.where(np.any(fin_frames_masks, axis=0))[0]
     else:
         return corners_all, ids_all, fin_frames_masks
 
@@ -86,19 +88,25 @@
         if not init_frames_mask[i_frame]:
             continue
 
         # color management
         if not isinstance(opts['color_convert'], bool) and len(frame.shape) > 2:
             frame = cv2.cvtColor(frame, opts['color_convert'])  # noqa
 
+        parameters = cv2.aruco.DetectorParameters()
+
+        detector = cv2.aruco.ArucoDetector(cv2.aruco.getPredefinedDictionary(board_params['dictionary_type']),
+                                           parameters)
+
         # corner detection
-        corners, ids, rejected_img_points = \
-            cv2.aruco.detectMarkers(frame,  # noqa
-                                    cv2.aruco.getPredefinedDictionary(board_params['dictionary_type']),  # noqa
-                                    **finalize_aruco_detector_opts(opts['detection_opts']['aruco_detect']))
+        corners, ids, rejected_img_points = detector.detectMarkers(frame)
+        # corners, ids, rejected_img_points = \
+        #     cv2.aruco.detectMarkers(frame,  # noqa
+        #                             cv2.aruco.getPredefinedDictionary(board_params['dictionary_type']),  # noqa
+        #                             **finalize_aruco_detector_opts(opts['detection_opts']['aruco_detect']))
 
         if len(corners) == 0:
             continue
 
         # corner refinement
         corners_ref, ids_ref = \
             cv2.aruco.refineDetectedMarkers(frame,  # noqa
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `bbo-calibcam-2.4.2/calibcam/helper.py` & `bbo-calibcam-3.0.0/calibcam/helper.py`

 * *Files identical despite different names*

### Comparing `bbo-calibcam-2.4.2/calibcam/helper_ag.py` & `bbo-calibcam-3.0.0/calibcam/helper_ag.py`

 * *Files identical despite different names*

### Comparing `bbo-calibcam-2.4.2/calibcam/opt_jacfwd/optfunctions_ag.py` & `bbo-calibcam-3.0.0/calibcam/repro/optfunctions_ag.py`

 * *Files identical despite different names*

### Comparing `bbo-calibcam-2.4.2/calibcam/optimization.py` & `bbo-calibcam-3.0.0/calibcam/optimization.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,60 +7,80 @@
 import sys
 
 # This could also be done dynamically, based on opts ...
 # from calibcam.opt_vmapgrad.optfunctions import obj_fcn_wrapper, obj_fcn_jacobian_wrapper, get_precalc  # noqa
 # Calculating Jacobians would be much more straightforward, but seems to be prohibitively slow ...
 import calibcamlib
 from calibcam import board, helper
-from calibcam.opt_jacfwd.optfunctions import obj_fcn_wrapper, obj_fcn_jacobian_wrapper, obj_fcn_jacobian_wrapper_sparse, \
+from calibcam.repro.optfunctions import obj_fcn_wrapper, obj_fcn_jacobian_wrapper, obj_fcn_jacobian_wrapper_sparse, \
     get_precalc  # noqa
 from scipy.spatial.transform import Rotation as R  # noqa
 
 
 def make_vars_full(vars_opt, args, verbose=False):
     n_cams = args['corners'].shape[0]
+    n_boards = args['corners'].shape[1]
 
     # Update full set of vars with free vars
     vars_full = args['vars_full']
     if verbose:
         print(vars_full[0:7])
     mask_opt = args['mask_opt']
     vars_full[mask_opt] = vars_opt
 
     if verbose:
         print(mask_opt[0:7])
         print(vars_full[0:7])
 
-    return vars_full, n_cams
+    return vars_full, n_cams, n_boards
 
 
-def unravel_vars_full(vars_full, n_cams):
-    n_cam_param_list = np.array([3, 3, 9, 1, 5])  # r, t, A, xi, k
-    n_cam_params = n_cam_param_list.sum(dtype=int)
-
-    start_idx = 0
-    cam_pose_vars = vars_full[start_idx:start_idx + n_cams * 6]
-    rvecs_cams = cam_pose_vars[0:int(cam_pose_vars.size / 2)].reshape(-1, 3)
-    tvecs_cams = cam_pose_vars[int(cam_pose_vars.size / 2):].reshape(-1, 3)
-
-    start_idx = start_idx + n_cams * 6
-    cam_mats_vars = vars_full[start_idx:start_idx + n_cams * 9]
-    cam_matrices = cam_mats_vars.reshape(-1, 3, 3)
-
-    start_idx = start_idx + n_cams * 9
-    xis_vars = vars_full[start_idx:start_idx + n_cams * 1]
-    xis = xis_vars.reshape(-1, 1)
-
-    start_idx = start_idx + n_cams * 1
-    ks_vars = vars_full[start_idx:start_idx + n_cams * 5]
-    ks = ks_vars.reshape(-1, 5)
-
-    board_pose_vars = vars_full[n_cams * n_cam_params:]
-    rvecs_boards = board_pose_vars[0:int(board_pose_vars.size / 2)].reshape(-1, 3)
-    tvecs_boards = board_pose_vars[int(board_pose_vars.size / 2):].reshape(-1, 3)
+def get_cam_field_sizes(m):
+    field_sizes = np.array([m * 3,  # cam extrinsic rotations
+                            m * 3,  # cam extrinsic positions
+                            m * 9,  # cam intrinsics A
+                            m,  # cam intrinsics xi
+                            m * 5,  # cam intrinsics k
+                            ])
+    return field_sizes
+
+
+def get_board_field_sizes(k):
+    field_sizes = np.array([k * 3,  # boards rotations
+                            k * 3,  # boards extrinsic positions
+                            ])
+    return field_sizes
+
+
+def get_var_edges(m, k):
+    field_sizes = np.concatenate(([0], get_cam_field_sizes(m), get_board_field_sizes(k)))
+    edges = np.cumsum(field_sizes)
+    return edges
+
+
+def unravel_vars_full(vars_full, n_cams, n_boards):
+    edges = get_var_edges(n_cams, n_boards)
+    edge_idx = 0
+
+    rvecs_cams = vars_full[edges[edge_idx]:edges[edge_idx + 1]].reshape(-1, 3)
+    edge_idx += 1
+    tvecs_cams = vars_full[edges[edge_idx]:edges[edge_idx + 1]].reshape(-1, 3)
+    edge_idx += 1
+
+    cam_matrices = vars_full[edges[edge_idx]:edges[edge_idx + 1]].reshape(-1, 3, 3)
+    edge_idx += 1
+    xis = vars_full[edges[edge_idx]:edges[edge_idx + 1]].reshape(-1, 1)
+    edge_idx += 1
+    ks = vars_full[edges[edge_idx]:edges[edge_idx + 1]].reshape(-1, 5)
+    edge_idx += 1
+
+    rvecs_boards = vars_full[edges[edge_idx]:edges[edge_idx + 1]].reshape(-1, 3)
+    edge_idx += 1
+    tvecs_boards = vars_full[edges[edge_idx]:edges[edge_idx + 1]].reshape(-1, 3)
+    edge_idx += 1
 
     return rvecs_cams, tvecs_cams, cam_matrices, xis, ks, rvecs_boards, tvecs_boards
 
 
 def make_initialization(calibs, corners, board_params, opts):
     opts_free_vars = opts['free_vars']
 
@@ -174,18 +194,19 @@
         ks_mask.ravel(),
         pose_mask.ravel()),
         axis=0)
 
 
 def unravel_to_calibs(vars_opt, args):
     # Fill vars_full from initialization with vars_opts
-    vars_full, n_cams = make_vars_full(vars_opt, args, verbose=False)
+    vars_full, n_cams, n_boards = make_vars_full(vars_opt, args, verbose=False)
 
     # Unravel inputs.
-    rvecs_cams, tvecs_cams, cam_matrices, xis, ks, rvecs_boards, tvecs_boards = unravel_vars_full(vars_full, n_cams)
+    (rvecs_cams, tvecs_cams, cam_matrices, xis, ks,
+     rvecs_boards, tvecs_boards) = unravel_vars_full(vars_full, n_cams, n_boards)
 
     calibs = [
         {
             'rvec_cam': rvecs_cams[i_cam],
             'tvec_cam': tvecs_cams[i_cam],
             'A': cam_matrices[i_cam],
             'xi': xis[i_cam],
```

### Comparing `bbo-calibcam-2.4.2/calibcam/pose_estimation.py` & `bbo-calibcam-3.0.0/calibcam/pose_estimation.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,28 @@
 import numpy as np
 from copy import deepcopy
 from scipy.spatial.transform import Rotation as R  # noqa
+from bbo.geometry import RigidTransform
+
+def build_initialized_calibs(calibs_single, opts, corners=None, required_corner_idxs=None):
+    calibs = deepcopy(calibs_single)
+
+    for i_calib, calib in enumerate(calibs):
+        calib["rvec_cam"] = opts["init_extrinsics"]["rvecs_cam"][i_calib]
+        calib["tvec_cam"] = opts["init_extrinsics"]["tvecs_cam"][i_calib]
+
+        cam2camsystem = RigidTransform(rotation=calib["rvec_cam"], translation=calib["tvec_cam"],
+                                       rotation_type="rotvec").inv()
+        board2cam = RigidTransform(rotation=calib["rvecs"], translation=calib["tvecs"], rotation_type="rotvec")
+        board2camsystem = cam2camsystem * board2cam
+
+        calib["rvecs"] = board2camsystem.get_rotation().as_rotvec()
+        calib["tvecs"] = board2camsystem.get_translation()
+
+    return calibs
 
 
 def estimate_cam_poses(calibs_single, opts, corners=None, required_corner_idxs=None):
     calibs = deepcopy(calibs_single)
 
     cams_oriented = np.zeros(len(calibs), dtype=bool)
     cams_oriented[opts['coord_cam']] = True
```

### Comparing `bbo-calibcam-2.4.2/calibcam/single_camcalibration.py` & `bbo-calibcam-3.0.0/calibcam/single_camcalibration.py`

 * *Files identical despite different names*

### Comparing `bbo-calibcam-2.4.2/calibcam/yaml_helper.py` & `bbo-calibcam-3.0.0/calibcam/yaml_helper.py`

 * *Files identical despite different names*

### Comparing `bbo-calibcam-2.4.2/setup.py` & `bbo-calibcam-3.0.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,24 +7,25 @@
 README = (HERE / "README.md").read_text()
 
 packages=find_packages()
 print(packages)
 # This call to setup() does all the work
 setup(
     name="bbo-calibcam",
-    version="2.4.2",
+    version="3.0.0",
     description="Calibrate intrinsic and extrinsic parameters of cameras with charuco boards",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/bbo-lab/calibcam",
     author="BBO-lab @ caesar",
     author_email="kay-michael.voit@mpinb.mpg.de",
     license="BSD",
     classifiers=[
         "License :: OSI Approved :: BSD License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.10",
     ],
     packages=packages,
     include_package_data=True,
-    install_requires=["numpy", "pyyaml", "scipy", "bbo-calibcamlib", "jax", "jaxlib", "imageio", "bbo-ccvtools", "bbo-svidreader"],
+    install_requires=["numpy", "pyyaml", "scipy", "bbo-calibcamlib", "jax", "jaxlib", "imageio", "bbo-ccvtools",
+                      "bbo-svidreader", "bbo_bbo"],
 )
```

### Comparing `bbo-calibcam-2.4.2/test/test_detection.py` & `bbo-calibcam-3.0.0/test/test_detection.py`

 * *Files identical despite different names*

