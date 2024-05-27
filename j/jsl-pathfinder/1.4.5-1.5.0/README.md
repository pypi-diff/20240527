# Comparing `tmp/jsl-pathfinder-1.4.5.tar.gz` & `tmp/jsl-pathfinder-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsl-pathfinder-1.4.5.tar", last modified: Tue Nov 28 23:41:15 2023, max compression
+gzip compressed data, was "jsl-pathfinder-1.5.0.tar", last modified: Mon May 27 18:29:48 2024, max compression
```

## Comparing `jsl-pathfinder-1.4.5.tar` & `jsl-pathfinder-1.5.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 matthewcooke   (501) staff       (20)        0 2023-11-28 23:41:15.540861 jsl-pathfinder-1.4.5/
--rwxr-xr-x   0 matthewcooke   (501) staff       (20)    35149 2022-07-18 21:00:09.000000 jsl-pathfinder-1.4.5/LICENSE
--rw-r--r--   0 matthewcooke   (501) staff       (20)     9377 2023-11-28 23:41:15.540687 jsl-pathfinder-1.4.5/PKG-INFO
--rwxr-xr-x   0 matthewcooke   (501) staff       (20)     8647 2023-01-05 20:39:43.000000 jsl-pathfinder-1.4.5/README.md
-drwxr-xr-x   0 matthewcooke   (501) staff       (20)        0 2023-11-28 23:41:15.539549 jsl-pathfinder-1.4.5/SearchStrategyAnalysis/
--rwxr-xr-x   0 matthewcooke   (501) staff       (20)   123947 2023-11-28 23:33:47.000000 jsl-pathfinder-1.4.5/SearchStrategyAnalysis/Pathfinder.py
--rwxr-xr-x   0 matthewcooke   (501) staff       (20)      170 2022-07-18 21:00:09.000000 jsl-pathfinder-1.4.5/SearchStrategyAnalysis/__init__.py
--rwxr-xr-x   0 matthewcooke   (501) staff       (20)    21416 2023-01-05 20:27:29.000000 jsl-pathfinder-1.4.5/SearchStrategyAnalysis/appTrial.py
--rwxr-xr-x   0 matthewcooke   (501) staff       (20)     3933 2023-01-05 20:09:48.000000 jsl-pathfinder-1.4.5/SearchStrategyAnalysis/heatmap.py
-drwxr-xr-x   0 matthewcooke   (501) staff       (20)        0 2023-11-28 23:41:15.540459 jsl-pathfinder-1.4.5/jsl_pathfinder.egg-info/
--rwxr-xr-x   0 matthewcooke   (501) staff       (20)     9377 2023-11-28 23:41:15.000000 jsl-pathfinder-1.4.5/jsl_pathfinder.egg-info/PKG-INFO
--rwxr-xr-x   0 matthewcooke   (501) staff       (20)      397 2023-11-28 23:41:15.000000 jsl-pathfinder-1.4.5/jsl_pathfinder.egg-info/SOURCES.txt
--rwxr-xr-x   0 matthewcooke   (501) staff       (20)        1 2023-11-28 23:41:15.000000 jsl-pathfinder-1.4.5/jsl_pathfinder.egg-info/dependency_links.txt
--rwxr-xr-x   0 matthewcooke   (501) staff       (20)       66 2023-11-28 23:41:15.000000 jsl-pathfinder-1.4.5/jsl_pathfinder.egg-info/entry_points.txt
--rwxr-xr-x   0 matthewcooke   (501) staff       (20)       50 2023-11-28 23:41:15.000000 jsl-pathfinder-1.4.5/jsl_pathfinder.egg-info/requires.txt
--rwxr-xr-x   0 matthewcooke   (501) staff       (20)       23 2023-11-28 23:41:15.000000 jsl-pathfinder-1.4.5/jsl_pathfinder.egg-info/top_level.txt
--rw-r--r--   0 matthewcooke   (501) staff       (20)       38 2023-11-28 23:41:15.540912 jsl-pathfinder-1.4.5/setup.cfg
--rwxr-xr-x   0 matthewcooke   (501) staff       (20)     1266 2023-11-28 23:33:47.000000 jsl-pathfinder-1.4.5/setup.py
+drwxr-xr-x   0 matthewcooke   (501) staff       (20)        0 2024-05-27 18:29:48.549171 jsl-pathfinder-1.5.0/
+-rwxr-xr-x   0 matthewcooke   (501) staff       (20)    35149 2022-07-18 21:00:09.000000 jsl-pathfinder-1.5.0/LICENSE
+-rw-r--r--   0 matthewcooke   (501) staff       (20)     9481 2024-05-27 18:29:48.548820 jsl-pathfinder-1.5.0/PKG-INFO
+-rwxr-xr-x   0 matthewcooke   (501) staff       (20)     8633 2024-05-27 18:21:02.000000 jsl-pathfinder-1.5.0/README.md
+drwxr-xr-x   0 matthewcooke   (501) staff       (20)        0 2024-05-27 18:29:48.547263 jsl-pathfinder-1.5.0/SearchStrategyAnalysis/
+-rwxr-xr-x   0 matthewcooke   (501) staff       (20)   123970 2024-05-27 18:21:02.000000 jsl-pathfinder-1.5.0/SearchStrategyAnalysis/Pathfinder.py
+-rwxr-xr-x   0 matthewcooke   (501) staff       (20)      170 2022-07-18 21:00:09.000000 jsl-pathfinder-1.5.0/SearchStrategyAnalysis/__init__.py
+-rwxr-xr-x   0 matthewcooke   (501) staff       (20)    20821 2024-05-27 18:21:02.000000 jsl-pathfinder-1.5.0/SearchStrategyAnalysis/appTrial.py
+-rwxr-xr-x   0 matthewcooke   (501) staff       (20)     3861 2024-05-27 18:21:02.000000 jsl-pathfinder-1.5.0/SearchStrategyAnalysis/heatmap.py
+drwxr-xr-x   0 matthewcooke   (501) staff       (20)        0 2024-05-27 18:29:48.548346 jsl-pathfinder-1.5.0/jsl_pathfinder.egg-info/
+-rw-r--r--   0 matthewcooke   (501) staff       (20)     9481 2024-05-27 18:29:48.000000 jsl-pathfinder-1.5.0/jsl_pathfinder.egg-info/PKG-INFO
+-rwxr-xr-x   0 matthewcooke   (501) staff       (20)      397 2024-05-27 18:29:48.000000 jsl-pathfinder-1.5.0/jsl_pathfinder.egg-info/SOURCES.txt
+-rwxr-xr-x   0 matthewcooke   (501) staff       (20)        1 2024-05-27 18:29:48.000000 jsl-pathfinder-1.5.0/jsl_pathfinder.egg-info/dependency_links.txt
+-rwxr-xr-x   0 matthewcooke   (501) staff       (20)       66 2024-05-27 18:29:48.000000 jsl-pathfinder-1.5.0/jsl_pathfinder.egg-info/entry_points.txt
+-rwxr-xr-x   0 matthewcooke   (501) staff       (20)       43 2024-05-27 18:29:48.000000 jsl-pathfinder-1.5.0/jsl_pathfinder.egg-info/requires.txt
+-rwxr-xr-x   0 matthewcooke   (501) staff       (20)       23 2024-05-27 18:29:48.000000 jsl-pathfinder-1.5.0/jsl_pathfinder.egg-info/top_level.txt
+-rw-r--r--   0 matthewcooke   (501) staff       (20)       38 2024-05-27 18:29:48.549250 jsl-pathfinder-1.5.0/setup.cfg
+-rwxr-xr-x   0 matthewcooke   (501) staff       (20)     1247 2024-05-27 18:29:41.000000 jsl-pathfinder-1.5.0/setup.py
```

### Comparing `jsl-pathfinder-1.4.5/LICENSE` & `jsl-pathfinder-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jsl-pathfinder-1.4.5/PKG-INFO` & `jsl-pathfinder-1.5.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: jsl-pathfinder
-Version: 1.4.5
-Summary: Morris Water Maze Search Strategy Analysis
-Home-page: https://github.com/MatthewBCooke/Pathfinder
-Author: Matthew Cooke
-Author-email: matthew.cooke@ubc.ca
-License: GNU
-Keywords: morris water maze jason snyder lab search strategy strategies analysis
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Science/Research
-Classifier: Natural Language :: English
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Classifier: Programming Language :: Python :: 3.5
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Pathfinder    [![DOI](https://zenodo.org/badge/188258387.svg)](https://zenodo.org/badge/latestdoi/188258387)
 
 Morris Water Maze search strategy and entropy analysis.
 
 Created by **Matthew Cooke** at **The University of British Columbia**, **Jason Snyder Lab**
 
 **For more information about the features and usage of Pathfinder please visit our [wiki](https://github.com/MatthewBCooke/Pathfinder/wiki)**
@@ -122,22 +104,22 @@
 
 For the most recent stable version, cloning the GitHub repository or installing via PyPi is possible. For the most recent beta version of the software, the develop branch of the GitHub repository will host the version currently being worked on.
 
 Installation Instructions:
 
 Windows:
 
-1. Installing from the Python Package Index:
+Installing from the Python Package Index:
 Launch a CMD window by launching `run` from the start menu, and typing `CMD` in Run.
 
 Once the CMD shell has opened, type `pip install jsl-pathfinder`
 
 Press enter
 
-2. Installing from GitHub:
+Installing from GitHub
 
 Download and install Git here: https://git-scm.com
 
 Open Git Bash.
 
 Change the current working directory to the location where you want the cloned directory to be made.
 
@@ -145,23 +127,23 @@
 
 Press enter
 
 ***
 
 Mac:
 
-1. Installing from the Python Package Index:
+Installing from the Python Package Index:
 
 Open a terminal window (located in your utilities folder under the Applications directory.
 
 Type `pip install jsl-pathfinder`
 
 Press return
 
-2. Installing from GitHub:
+Installing from GitHub
 
 Open a terminal window Navigate to the folder you wish to install Pathfinder into
 
 Type `git clone https://github.com/MatthewBCooke/Pathfinder/`
 
 press return
```

### Comparing `jsl-pathfinder-1.4.5/README.md` & `jsl-pathfinder-1.5.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,30 @@
+Metadata-Version: 2.1
+Name: jsl-pathfinder
+Version: 1.5.0
+Summary: Morris Water Maze Search Strategy Analysis
+Home-page: https://github.com/MatthewBCooke/Pathfinder
+Author: Matthew Cooke
+Author-email: matthew.cooke@ubc.ca
+License: GNU
+Keywords: morris water maze jason snyder lab search strategy strategies analysis
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Science/Research
+Classifier: Natural Language :: English
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Programming Language :: Python :: 3.5
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: xlrd==1.2.0
+Requires-Dist: plotly
+Requires-Dist: pillow
+Requires-Dist: matplotlib
+Requires-Dist: scipy
+
 # Pathfinder    [![DOI](https://zenodo.org/badge/188258387.svg)](https://zenodo.org/badge/latestdoi/188258387)
 
 Morris Water Maze search strategy and entropy analysis.
 
 Created by **Matthew Cooke** at **The University of British Columbia**, **Jason Snyder Lab**
 
 **For more information about the features and usage of Pathfinder please visit our [wiki](https://github.com/MatthewBCooke/Pathfinder/wiki)**
@@ -104,22 +127,22 @@
 
 For the most recent stable version, cloning the GitHub repository or installing via PyPi is possible. For the most recent beta version of the software, the develop branch of the GitHub repository will host the version currently being worked on.
 
 Installation Instructions:
 
 Windows:
 
-1. Installing from the Python Package Index:
+Installing from the Python Package Index:
 Launch a CMD window by launching `run` from the start menu, and typing `CMD` in Run.
 
 Once the CMD shell has opened, type `pip install jsl-pathfinder`
 
 Press enter
 
-2. Installing from GitHub:
+Installing from GitHub
 
 Download and install Git here: https://git-scm.com
 
 Open Git Bash.
 
 Change the current working directory to the location where you want the cloned directory to be made.
 
@@ -127,23 +150,23 @@
 
 Press enter
 
 ***
 
 Mac:
 
-1. Installing from the Python Package Index:
+Installing from the Python Package Index:
 
 Open a terminal window (located in your utilities folder under the Applications directory.
 
 Type `pip install jsl-pathfinder`
 
 Press return
 
-2. Installing from GitHub:
+Installing from GitHub
 
 Open a terminal window Navigate to the folder you wish to install Pathfinder into
 
 Type `git clone https://github.com/MatthewBCooke/Pathfinder/`
 
 press return
```

### Comparing `jsl-pathfinder-1.4.5/SearchStrategyAnalysis/Pathfinder.py` & `jsl-pathfinder-1.5.0/SearchStrategyAnalysis/Pathfinder.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,30 +11,28 @@
 import webbrowser
 import statistics
 from collections import defaultdict
 from sys import platform as _platform
 from time import localtime, strftime
 import PIL.Image
 from PIL import ImageTk
-#from xlrd import open_workbook
+import pandas as pd
 from functools import partial
 import numpy as np
 import pickle
 import datetime
 import scipy.ndimage as sp
-import pandas as pd
 
 
-try:  # Tries to import local dependencies (pypi install)
-    from SearchStrategyAnalysis.appTrial import Trial, Experiment, Parameters, saveFileAsExperiment, Datapoint, defineOwnSoftware
-    import SearchStrategyAnalysis.heatmap
-    
-except: #For local path
-    from appTrial import Trial, Experiment, Parameters, saveFileAsExperiment, Datapoint, \
+try:  # Tries to import local dependencies
+    from SearchStrategyAnalysis.appTrial import Trial, Experiment, Parameters, saveFileAsExperiment, Datapoint, \
         defineOwnSoftware
+    import SearchStrategyAnalysis.heatmap
+except:
+    from appTrial import Trial, Experiment, Parameters, saveFileAsExperiment, Datapoint, defineOwnSoftware
     import heatmap
 from scipy.stats import norm
 import re
 import traceback
 
 try:  # Imports MATLAB engine if available
     import matlab.engine
@@ -657,16 +655,21 @@
                 if (set(['x', 'y', 't']).issubset(twoRows[1])):
                     softwareStringVar.set("watermaze")
                 if (set(eztrack).issubset(twoRows[0])):
                     softwareStringVar.set("eztrack")
                 else:
                     softwareStringVar.set("custom")
         elif (file_extension == '.xlsx'):
-            softwareStringVar.set("ethovision")
-
+            workbook = open_workbook(theFile)
+            sheet = workbook.sheet_by_index(0)
+            rowNames = sheet.col_values(0)
+            if (set(ethovision).issubset(rowNames)):
+                softwareStringVar.set("ethovision")
+            else:
+                softwareStringVar.set("custom")
 
     def openFile(self):  # opens a dialog to get a single file
         logging.debug("Open File...")
         global theFile
         global fileDirectory
         global fileFlag
         fileFlag = 1
@@ -1968,15 +1971,15 @@
 
             # Swim Path centroid
             i += 1.0
             xSummed += float(aDatapoint.getx())
             ySummed += float(aDatapoint.gety())
             aX = float(aDatapoint.getx())
             aY = float(aDatapoint.gety())
-            print(aX)
+
             arrayX.append(aX)
             arrayY.append(aY)
 
             # Average Distance
             currentDistanceFromGoal = math.sqrt((goalX - aX) ** 2 + (goalY - aY) ** 2)
 
             # in zones
@@ -2161,16 +2164,15 @@
             params = Parameters(name="Custom", ipeMaxVal=float(ipeMaxVal), headingMaxVal=float(headingMaxVal),
                                 distanceToSwimMaxVal=float(distanceToSwimMaxVal),
                                 distanceToPlatMaxVal=float(distanceToPlatMaxVal),
                                 distanceToSwimMaxVal2=float(distanceToSwimMaxVal2),
                                 distanceToPlatMaxVal2=float(distanceToPlatMaxVal2),
                                 corridorAverageMinVal=float(corridorAverageMinVal),
                                 directedSearchMaxDistance=float(directedSearchMaxDistance),
-                                focalMinDistance=float(focalMinDistance), 
-                                focalMaxDistance=float(focalMaxDistance),
+                                focalMinDistance=float(focalMinDistance), focalMaxDistance=float(focalMaxDistance),
                                 semiFocalMinDistance=float(semiFocalMinDistance),
                                 semiFocalMaxDistance=float(semiFocalMaxDistance),
                                 corridoripeMaxVal=float(corridoripeMaxVal),
                                 annulusCounterMaxVal=float(annulusCounterMaxVal),
                                 quadrantTotalMaxVal=int(quadrantTotalMaxVal),
                                 chainingMaxCoverage=float(chainingMaxCoverage),
                                 percentTraversedMaxVal=float(percentTraversedMaxVal),
@@ -2270,15 +2272,15 @@
             if aExperiment.hasTrialNames:
                 headersToWrite.append("Name")
             if aExperiment.hasAnimalNames:
                 headersToWrite.append("Animal")
         except:
             pass
         headersToWrite.extend(
-            ["Trial name", "Trial Code", "Strategy", "IPE", "Velocity", "Distance covered", "Average distance to goal",
+            ["Trial Code", "Strategy", "IPE", "Velocity", "Distance covered", "Average distance to goal",
              "Average heading error", "Percent of maze traversed", "Latency", "Score", "Initial heading error",
              "Entropy", "Distance to swim path centroid", "Average distance to centre of maze",
              "Percent in angular corridor", "Percent in annulus zone", "Percent in smaller thigmotaxis zone",
              "Percent in full thigmotaxis zone", "Strategy (manual)"])
         writer.writerow(headersToWrite)  # write to the csv
 
         dayNum = 0
@@ -2440,22 +2442,20 @@
                                 ("Animal: " + str(animal) + "  Day/Trial: " + str(dayNum) + "/" + str(
                                     trialNum[animal])), float(goalDiamVar))  # ask user for answer
                 root.wait_window(self.top2)  # we wait until the user responds
                 strategyManual = searchStrategyV  # update the strategyType to that of the user
 
             dataToWrite = []
 
+
             dataToWrite.append(trialNum[animal])
-            #if aExperiment.hasTrialNames:
-            if hasattr(aTrial, 'name'):
+            if aExperiment.hasTrialNames:
                 dataToWrite.append(aTrial.name)
-            elif aExperiment.hasAnimalNames:
+            if aExperiment.hasAnimalNames:
                 dataToWrite.append(aTrial.animal)
-            else:
-                dataToWrite.append('')
 
             dataToWrite.extend(
                 [(str(animal) + " " + str(dayNum) + " " + str(trialNum[animal])), strategyType, round(ipe, 2),
                  round(velocity, 2), round(totalDistance, 2), round(distanceAverage, 2),
                  round(averageHeadingError, 2), round(percentTraversed, 2), round(latency, 2), score,
                  initialHeadingError, round(entropyResult, 2), round(averageDistanceToSwimPathCentroid, 2),
                  round(averageDistanceToCentre, 2), round(corridorAverage, 2), round(annulusCounter / i, 2),
```

### Comparing `jsl-pathfinder-1.4.5/SearchStrategyAnalysis/appTrial.py` & `jsl-pathfinder-1.5.0/SearchStrategyAnalysis/appTrial.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 # Module: appTrial.py
 # Holds data structures
-#__requires__= 'xlrd==1.2.0'
+
 
 import sys
 from sys import platform as _platform
 import csv
 import math
 import logging
 import os
 import fnmatch
 import datetime
 import tkinter
 from operator import add
 from collections import defaultdict
 import pkg_resources
-#pkg_resources.require("xlrd==1.2.0")
 import pandas as pd
 
-#from xlrd import open_workbook
 if sys.version_info<(3,0,0):  # tkinter names for python 2
     print("Update to Python3 for best results... You may encounter errors")
     from Tkinter import *
     import tkMessageBox as messagebox
     import ttk
     import tkFileDialog as filedialog
 else:  # tkinter for python 3
@@ -375,38 +373,28 @@
                 for (i, v) in enumerate(row):
                     columns[i].append(v)
 
             aTrial = Trial()
             aTrial.setname(filename.split("/")[-1])
 
             for time, x, y in zip(columns[0][1:], columns[1][1:], columns[2][1:]):
-                print("TIME: ",time)
-                if (sum(map(lambda x : 1 if ':' in x else 0, time))>0):
-                    try:
-                        if (sum(map(lambda x : 1 if ':' in x else 0, time)) == 2):
-                            hours = float(time.split(':')[0])
-                            minutes = float(time.split(':')[1])
-                            seconds = float(time.split(':')[2])
-                        else:
-                            minutes = float(time.split(':')[0])
-                            seconds = float(time.split(':')[1])
-                            hours = 0
-                        time = seconds + minutes*60 + hours*3600
-                    except:
-                        aTrial.markDataAsCorrupted()
-                else:
-                    time = float(time)
- 
-                x = float(x)
-                y = float(y)
-                aTrial.append(Datapoint(time, x, y))
-                
+                try:
+                    hours = float(time.split(':')[0])
+                    minutes = float(time.split(':')[1])
+                    seconds = float(time.split(':')[2])
+                    time = seconds + minutes*60 + hours*3600
+                    x = float(x)
+                    y = float(y)
+                    aTrial.append(Datapoint(time, x, y))
+                except:
+                    aTrial.markDataAsCorrupted()
+
             trialList.append(aTrial)
 
-        elif software == "watermaze":  
+        elif software == "watermaze":
             logging.info("Reading watermaze")
             experiment.setHasAnimalNames(True)
             experiment.setHasDateInfo(True)
             experiment.setHasTrialNames(False)
 
             columns = defaultdict(list)  # each value in each column is appended to a list
```

### Comparing `jsl-pathfinder-1.4.5/SearchStrategyAnalysis/heatmap.py` & `jsl-pathfinder-1.5.0/SearchStrategyAnalysis/heatmap.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 import math
 import os
 import sys
-try:
-    from SearchStrategyAnalysis.appTrial import Trial, Experiment, Parameters
-except:
-    from appTrial import Trial, Experiment, Parameters
+from SearchStrategyAnalysis.appTrial import Trial, Experiment, Parameters
 from time import localtime, strftime
 
 if sys.version_info<(3,0,0):  # tkinter names for python 2
     print("Update to Python3 for best results... You may encounter errors")
     from Tkinter import *
     import tkMessageBox as messagebox
     import ttk
```

### Comparing `jsl-pathfinder-1.4.5/jsl_pathfinder.egg-info/PKG-INFO` & `jsl-pathfinder-1.5.0/jsl_pathfinder.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 Metadata-Version: 2.1
 Name: jsl-pathfinder
-Version: 1.4.5
+Version: 1.5.0
 Summary: Morris Water Maze Search Strategy Analysis
 Home-page: https://github.com/MatthewBCooke/Pathfinder
 Author: Matthew Cooke
 Author-email: matthew.cooke@ubc.ca
 License: GNU
 Keywords: morris water maze jason snyder lab search strategy strategies analysis
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Programming Language :: Python :: 3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: xlrd==1.2.0
+Requires-Dist: plotly
+Requires-Dist: pillow
+Requires-Dist: matplotlib
+Requires-Dist: scipy
 
 # Pathfinder    [![DOI](https://zenodo.org/badge/188258387.svg)](https://zenodo.org/badge/latestdoi/188258387)
 
 Morris Water Maze search strategy and entropy analysis.
 
 Created by **Matthew Cooke** at **The University of British Columbia**, **Jason Snyder Lab**
 
@@ -122,22 +127,22 @@
 
 For the most recent stable version, cloning the GitHub repository or installing via PyPi is possible. For the most recent beta version of the software, the develop branch of the GitHub repository will host the version currently being worked on.
 
 Installation Instructions:
 
 Windows:
 
-1. Installing from the Python Package Index:
+Installing from the Python Package Index:
 Launch a CMD window by launching `run` from the start menu, and typing `CMD` in Run.
 
 Once the CMD shell has opened, type `pip install jsl-pathfinder`
 
 Press enter
 
-2. Installing from GitHub:
+Installing from GitHub
 
 Download and install Git here: https://git-scm.com
 
 Open Git Bash.
 
 Change the current working directory to the location where you want the cloned directory to be made.
 
@@ -145,23 +150,23 @@
 
 Press enter
 
 ***
 
 Mac:
 
-1. Installing from the Python Package Index:
+Installing from the Python Package Index:
 
 Open a terminal window (located in your utilities folder under the Applications directory.
 
 Type `pip install jsl-pathfinder`
 
 Press return
 
-2. Installing from GitHub:
+Installing from GitHub
 
 Open a terminal window Navigate to the folder you wish to install Pathfinder into
 
 Type `git clone https://github.com/MatthewBCooke/Pathfinder/`
 
 press return
```

### Comparing `jsl-pathfinder-1.4.5/setup.py` & `jsl-pathfinder-1.5.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import *
 
 with open('README.md', encoding="utf8") as f:
     long_description = f.read()
 
 setup(
     name='jsl-pathfinder',
-    version='1.4.5',
+    version='1.5.0',
     description='Morris Water Maze Search Strategy Analysis',
     url='https://github.com/MatthewBCooke/Pathfinder',
     author='Matthew Cooke',
     author_email='matthew.cooke@ubc.ca',
     license='GNU',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
@@ -28,15 +28,14 @@
     packages=find_packages(),
     install_requires=[
         'xlrd == 1.2.0',
         'plotly',
         'pillow',
         'matplotlib',
         'scipy',
-        'pandas',
     ],
     long_description=long_description,
     long_description_content_type='text/markdown',
     entry_points={
        'gui_scripts': [
            'pathfinder = SearchStrategyAnalysis.Pathfinder:main',
        ],
```

