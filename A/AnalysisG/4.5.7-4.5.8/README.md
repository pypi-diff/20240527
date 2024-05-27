# Comparing `tmp/analysisg-4.5.7.tar.gz` & `tmp/analysisg-4.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "analysisg-4.5.7.tar", last modified: Mon May 27 20:19:31 2024, max compression
+gzip compressed data, was "analysisg-4.5.8.tar", last modified: Mon May 27 20:32:25 2024, max compression
```

## Comparing `analysisg-4.5.7.tar` & `analysisg-4.5.8.tar`

### file list

```diff
@@ -1,223 +1,223 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:19:31.939695 analysisg-4.5.7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:19:31.939695 analysisg-4.5.7/AnalysisG.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-05-27 20:19:31.000000 analysisg-4.5.7/AnalysisG.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5865 2024-05-27 20:19:31.000000 analysisg-4.5.7/AnalysisG.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 20:19:31.000000 analysisg-4.5.7/AnalysisG.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-27 20:19:31.000000 analysisg-4.5.7/AnalysisG.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-27 20:19:31.000000 analysisg-4.5.7/AnalysisG.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-27 20:19:31.000000 analysisg-4.5.7/AnalysisG.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-27 20:18:04.000000 analysisg-4.5.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-05-27 20:19:31.939695 analysisg-4.5.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-05-27 20:18:04.000000 analysisg-4.5.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-05-27 20:18:04.000000 analysisg-4.5.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 20:19:31.939695 analysisg-4.5.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-27 20:18:04.000000 analysisg-4.5.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:19:31.887694 analysisg-4.5.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:19:31.887694 analysisg-4.5.7/src/Events/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:19:31.887694 analysisg-4.5.7/src/Events/Deprecated/
--rw-r--r--   0 runner    (1001) docker     (127)     4657 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Events/Deprecated/Event.py
--rw-r--r--   0 runner    (1001) docker     (127)     4831 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Events/Deprecated/EventIndex.py
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Events/Deprecated/EventIndexParticle.py
--rw-r--r--   0 runner    (1001) docker     (127)     4263 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Events/Deprecated/EventParticles.py
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Events/Deprecated/ExperimentalEvent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Events/Deprecated/ExperimentalParticles.py
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Events/Deprecated/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:19:31.887694 analysisg-4.5.7/src/Events/Events/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Events/Events/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:19:31.887694 analysisg-4.5.7/src/Events/Events/bsm_4tops/
--rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Events/Events/bsm_4tops/Event.py
--rw-r--r--   0 runner    (1001) docker     (127)     4172 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Events/Events/bsm_4tops/Particles.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Events/Events/bsm_4tops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:19:31.891694 analysisg-4.5.7/src/Events/Events/mc20_ssml/
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Events/Events/mc20_ssml/Event.py
--rw-r--r--   0 runner    (1001) docker     (127)     3975 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Events/Events/mc20_ssml/Particles.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Events/Events/mc20_ssml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:19:31.891694 analysisg-4.5.7/src/Events/Events/ssml/
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Events/Events/ssml/Event.py
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Events/Events/ssml/Particles.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Events/Events/ssml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:19:31.891694 analysisg-4.5.7/src/Events/Graphs/
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Events/Graphs/EventGraphs.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Events/Graphs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Events/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:19:31.891694 analysisg-4.5.7/src/Generators/
--rw-r--r--   0 runner    (1001) docker     (127)    11135 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Generators/Analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     3920 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Generators/EventGenerator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Generators/GraphGenerator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Generators/Interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     7952 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Generators/Optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Generators/SampleGenerator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Generators/SelectionGenerator.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Generators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:19:31.891694 analysisg-4.5.7/src/IO/
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/IO/Pickle.py
--rw-r--r--   0 runner    (1001) docker     (127)     6551 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/IO/UpROOT.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/IO/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8529 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/IO/nTupler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:19:31.891694 analysisg-4.5.7/src/Model/
--rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Model/LossFunctions.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Model/Model.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:19:31.895694 analysisg-4.5.7/src/Notification/
--rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Notification/Analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Notification/Condor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Notification/EventGenerator.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Notification/FeatureAnalysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Notification/GraphGenerator.py
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Notification/IO.py
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Notification/Model.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Notification/MultiThreading.py
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Notification/Notification.py
--rw-r--r--   0 runner    (1001) docker     (127)     6149 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Notification/Optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Notification/RandomSamplers.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Notification/SelectionGenerator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Notification/UpROOT.py
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Notification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Notification/nTupler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:19:31.895694 analysisg-4.5.7/src/Plotting/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Plotting/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:19:31.895694 analysisg-4.5.7/src/SampleTracer/
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/SampleTracer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:19:31.895694 analysisg-4.5.7/src/Settings/
--rw-r--r--   0 runner    (1001) docker     (127)     5567 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Settings/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:19:31.895694 analysisg-4.5.7/src/Submission/
--rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Submission/Condor.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Submission/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4412 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Submission/script_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:19:31.895694 analysisg-4.5.7/src/Templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:19:31.895694 analysisg-4.5.7/src/Templates/Features/
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Templates/Features/FeatureAnalysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Templates/Features/FeatureTemplate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:19:31.895694 analysisg-4.5.7/src/Templates/Features/Jet/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Templates/Features/Jet/Edge.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Templates/Features/Jet/Graph.py
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Templates/Features/Jet/Node.py
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Templates/Features/Jet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:19:31.899694 analysisg-4.5.7/src/Templates/Features/TruthJet/
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Templates/Features/TruthJet/Edge.py
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Templates/Features/TruthJet/Graph.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Templates/Features/TruthJet/Node.py
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Templates/Features/TruthJet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:19:31.899694 analysisg-4.5.7/src/Templates/Features/TruthTop/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Templates/Features/TruthTop/Edge.py
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Templates/Features/TruthTop/Graph.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Templates/Features/TruthTop/Node.py
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Templates/Features/TruthTop/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:19:31.899694 analysisg-4.5.7/src/Templates/Features/TruthTopChildren/
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Templates/Features/TruthTopChildren/Edge.py
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Templates/Features/TruthTopChildren/Graph.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Templates/Features/TruthTopChildren/Node.py
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Templates/Features/TruthTopChildren/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Templates/Features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:19:31.899694 analysisg-4.5.7/src/Tools/
--rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Tools/General.py
--rw-r--r--   0 runner    (1001) docker     (127)     5787 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Tools/MultiThreading.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/Tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:19:31.899694 analysisg-4.5.7/src/cmodules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/cmodules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:19:31.899694 analysisg-4.5.7/src/cmodules/abstractions/
--rw-r--r--   0 runner    (1001) docker     (127)     6585 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/cmodules/abstractions/abstractions.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/cmodules/abstractions/abstractions.h
--rw-r--r--   0 runner    (1001) docker     (127)    12412 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/cmodules/abstractions/cytypes.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:19:31.899694 analysisg-4.5.7/src/cmodules/code/
--rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/cmodules/code/code.cxx
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/cmodules/code/code.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:19:31.931694 analysisg-4.5.7/src/cmodules/cyincludes/
--rw-r--r--   0 runner    (1001) docker     (127)  1030789 2024-05-27 20:19:29.000000 analysisg-4.5.7/src/cmodules/cyincludes/cycode.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/cmodules/cyincludes/cycode.pxd
--rw-r--r--   0 runner    (1001) docker     (127)    11818 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/cmodules/cyincludes/cycode.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/cmodules/cyincludes/cyepoch.pxd
--rw-r--r--   0 runner    (1001) docker     (127)  1227010 2024-05-27 20:19:29.000000 analysisg-4.5.7/src/cmodules/cyincludes/cyevent.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/cmodules/cyincludes/cyevent.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     8029 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/cmodules/cyincludes/cyevent.pyx
--rw-r--r--   0 runner    (1001) docker     (127)  1710540 2024-05-27 20:19:29.000000 analysisg-4.5.7/src/cmodules/cyincludes/cygraph.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/cmodules/cyincludes/cygraph.pxd
--rw-r--r--   0 runner    (1001) docker     (127)    14256 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/cmodules/cyincludes/cygraph.pyx
--rw-r--r--   0 runner    (1001) docker     (127)  2216395 2024-05-27 20:19:30.000000 analysisg-4.5.7/src/cmodules/cyincludes/cymetadata.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/cmodules/cyincludes/cymetadata.pxd
--rw-r--r--   0 runner    (1001) docker     (127)    24686 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/cmodules/cyincludes/cymetadata.pyx
--rw-r--r--   0 runner    (1001) docker     (127)  2407332 2024-05-27 20:19:30.000000 analysisg-4.5.7/src/cmodules/cyincludes/cyoptimizer.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6312 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/cmodules/cyincludes/cyoptimizer.pxd
--rw-r--r--   0 runner    (1001) docker     (127)    32123 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/cmodules/cyincludes/cyoptimizer.pyx
--rw-r--r--   0 runner    (1001) docker     (127)   842737 2024-05-27 20:19:28.000000 analysisg-4.5.7/src/cmodules/cyincludes/cyparticle.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/cmodules/cyincludes/cyparticle.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     8770 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/cmodules/cyincludes/cyparticle.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/cmodules/cyincludes/cyplotstruct.pxd
--rw-r--r--   0 runner    (1001) docker     (127)  2023505 2024-05-27 20:19:30.000000 analysisg-4.5.7/src/cmodules/cyincludes/cyplotting.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/cmodules/cyincludes/cyplotting.pxd
--rw-r--r--   0 runner    (1001) docker     (127)    29907 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/cmodules/cyincludes/cyplotting.pyx
--rw-r--r--   0 runner    (1001) docker     (127)  1524074 2024-05-27 20:19:30.000000 analysisg-4.5.7/src/cmodules/cyincludes/cyrunner.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/cmodules/cyincludes/cyrunner.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/cmodules/cyincludes/cyrunner.pyx
--rw-r--r--   0 runner    (1001) docker     (127)  4138415 2024-05-27 20:19:31.000000 analysisg-4.5.7/src/cmodules/cyincludes/cysampletracer.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/cmodules/cyincludes/cysampletracer.pxd
--rw-r--r--   0 runner    (1001) docker     (127)    55067 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/cmodules/cyincludes/cysampletracer.pyx
--rw-r--r--   0 runner    (1001) docker     (127)  1251042 2024-05-27 20:19:29.000000 analysisg-4.5.7/src/cmodules/cyincludes/cyselection.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/cmodules/cyincludes/cyselection.pxd
--rw-r--r--   0 runner    (1001) docker     (127)    12439 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/cmodules/cyincludes/cyselection.pyx
--rw-r--r--   0 runner    (1001) docker     (127)   856671 2024-05-27 20:19:29.000000 analysisg-4.5.7/src/cmodules/cyincludes/cytooling.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/cmodules/cyincludes/cytooling.pyx
--rw-r--r--   0 runner    (1001) docker     (127)    10796 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/cmodules/cyincludes/cytools.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     8743 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/cmodules/cyincludes/cytypes.pxd
--rw-r--r--   0 runner    (1001) docker     (127)  1273497 2024-05-27 20:19:29.000000 analysisg-4.5.7/src/cmodules/cyincludes/cywrapping.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/cmodules/cyincludes/cywrapping.pxd
--rw-r--r--   0 runner    (1001) docker     (127)    18693 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/cmodules/cyincludes/cywrapping.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:19:31.931694 analysisg-4.5.7/src/cmodules/epoch/
--rw-r--r--   0 runner    (1001) docker     (127)     5528 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/cmodules/epoch/epoch.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/cmodules/epoch/epoch.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:19:31.931694 analysisg-4.5.7/src/cmodules/event/
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/cmodules/event/event.cxx
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/cmodules/event/event.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:19:31.931694 analysisg-4.5.7/src/cmodules/graph/
--rw-r--r--   0 runner    (1001) docker     (127)     4031 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/cmodules/graph/graph.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/cmodules/graph/graph.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:19:31.931694 analysisg-4.5.7/src/cmodules/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)     9801 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/cmodules/metadata/metadata.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/cmodules/metadata/metadata.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:19:31.931694 analysisg-4.5.7/src/cmodules/optimizer/
--rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/cmodules/optimizer/optimizer.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/cmodules/optimizer/optimizer.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:19:31.931694 analysisg-4.5.7/src/cmodules/particle/
--rw-r--r--   0 runner    (1001) docker     (127)     9313 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/cmodules/particle/particle.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/cmodules/particle/particle.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:19:31.931694 analysisg-4.5.7/src/cmodules/plotting/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/cmodules/plotting/plotting.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/cmodules/plotting/plotting.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:19:31.931694 analysisg-4.5.7/src/cmodules/root/
--rw-r--r--   0 runner    (1001) docker     (127)    15660 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/cmodules/root/root.cxx
--rw-r--r--   0 runner    (1001) docker     (127)    11195 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/cmodules/root/root.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:19:31.935694 analysisg-4.5.7/src/cmodules/sampletracer/
--rw-r--r--   0 runner    (1001) docker     (127)    16542 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/cmodules/sampletracer/sampletracer.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     6806 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/cmodules/sampletracer/sampletracer.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:19:31.935694 analysisg-4.5.7/src/cmodules/selection/
--rw-r--r--   0 runner    (1001) docker     (127)     6694 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/cmodules/selection/selection.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-27 20:18:04.000000 analysisg-4.5.7/src/cmodules/selection/selection.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:19:31.939695 analysisg-4.5.7/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-27 20:18:04.000000 analysisg-4.5.7/test/test_ami.py
--rw-r--r--   0 runner    (1001) docker     (127)    12562 2024-05-27 20:18:04.000000 analysisg-4.5.7/test/test_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-05-27 20:18:04.000000 analysisg-4.5.7/test/test_cache_flush.py
--rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-05-27 20:18:04.000000 analysisg-4.5.7/test/test_event_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5159 2024-05-27 20:18:04.000000 analysisg-4.5.7/test/test_event_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     6466 2024-05-27 20:18:04.000000 analysisg-4.5.7/test/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     5128 2024-05-27 20:18:04.000000 analysisg-4.5.7/test/test_graph_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-05-27 20:18:04.000000 analysisg-4.5.7/test/test_graph_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-05-27 20:18:04.000000 analysisg-4.5.7/test/test_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-27 20:18:04.000000 analysisg-4.5.7/test/test_io.py
--rw-r--r--   0 runner    (1001) docker     (127)    10461 2024-05-27 20:18:04.000000 analysisg-4.5.7/test/test_machine_learning.py
--rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-05-27 20:18:04.000000 analysisg-4.5.7/test/test_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-27 20:18:04.000000 analysisg-4.5.7/test/test_notification.py
--rw-r--r--   0 runner    (1001) docker     (127)    20233 2024-05-27 20:18:04.000000 analysisg-4.5.7/test/test_nusol.py
--rw-r--r--   0 runner    (1001) docker     (127)    11275 2024-05-27 20:18:04.000000 analysisg-4.5.7/test/test_nusol_versions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4862 2024-05-27 20:18:04.000000 analysisg-4.5.7/test/test_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     5189 2024-05-27 20:18:04.000000 analysisg-4.5.7/test/test_particle_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     4545 2024-05-27 20:18:04.000000 analysisg-4.5.7/test/test_physics.py
--rw-r--r--   0 runner    (1001) docker     (127)     6130 2024-05-27 20:18:04.000000 analysisg-4.5.7/test/test_selection_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-27 20:18:04.000000 analysisg-4.5.7/test/test_selection_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     7296 2024-05-27 20:18:04.000000 analysisg-4.5.7/test/test_submission.py
--rw-r--r--   0 runner    (1001) docker     (127)     6688 2024-05-27 20:18:04.000000 analysisg-4.5.7/test/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     8639 2024-05-27 20:18:04.000000 analysisg-4.5.7/test/test_tracer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5631 2024-05-27 20:18:04.000000 analysisg-4.5.7/test/test_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:32:25.281463 analysisg-4.5.8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:32:25.281463 analysisg-4.5.8/AnalysisG.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-05-27 20:32:25.000000 analysisg-4.5.8/AnalysisG.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5865 2024-05-27 20:32:25.000000 analysisg-4.5.8/AnalysisG.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 20:32:25.000000 analysisg-4.5.8/AnalysisG.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-27 20:32:25.000000 analysisg-4.5.8/AnalysisG.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-27 20:32:25.000000 analysisg-4.5.8/AnalysisG.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-27 20:32:25.000000 analysisg-4.5.8/AnalysisG.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-27 20:31:07.000000 analysisg-4.5.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-05-27 20:32:25.281463 analysisg-4.5.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-05-27 20:31:07.000000 analysisg-4.5.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-05-27 20:31:07.000000 analysisg-4.5.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 20:32:25.281463 analysisg-4.5.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-27 20:31:07.000000 analysisg-4.5.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:32:25.229463 analysisg-4.5.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:32:25.229463 analysisg-4.5.8/src/Events/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:32:25.229463 analysisg-4.5.8/src/Events/Deprecated/
+-rw-r--r--   0 runner    (1001) docker     (127)     4657 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Events/Deprecated/Event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4831 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Events/Deprecated/EventIndex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Events/Deprecated/EventIndexParticle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4263 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Events/Deprecated/EventParticles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Events/Deprecated/ExperimentalEvent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Events/Deprecated/ExperimentalParticles.py
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Events/Deprecated/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:32:25.229463 analysisg-4.5.8/src/Events/Events/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Events/Events/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:32:25.229463 analysisg-4.5.8/src/Events/Events/bsm_4tops/
+-rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Events/Events/bsm_4tops/Event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4172 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Events/Events/bsm_4tops/Particles.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Events/Events/bsm_4tops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:32:25.229463 analysisg-4.5.8/src/Events/Events/mc20_ssml/
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Events/Events/mc20_ssml/Event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3975 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Events/Events/mc20_ssml/Particles.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Events/Events/mc20_ssml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:32:25.233463 analysisg-4.5.8/src/Events/Events/ssml/
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Events/Events/ssml/Event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Events/Events/ssml/Particles.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Events/Events/ssml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:32:25.233463 analysisg-4.5.8/src/Events/Graphs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Events/Graphs/EventGraphs.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Events/Graphs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Events/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:32:25.233463 analysisg-4.5.8/src/Generators/
+-rw-r--r--   0 runner    (1001) docker     (127)    11135 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Generators/Analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3920 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Generators/EventGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Generators/GraphGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Generators/Interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7952 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Generators/Optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Generators/SampleGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Generators/SelectionGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Generators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:32:25.233463 analysisg-4.5.8/src/IO/
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/IO/Pickle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6551 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/IO/UpROOT.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/IO/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8529 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/IO/nTupler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:32:25.233463 analysisg-4.5.8/src/Model/
+-rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Model/LossFunctions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Model/Model.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:32:25.237464 analysisg-4.5.8/src/Notification/
+-rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Notification/Analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Notification/Condor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Notification/EventGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Notification/FeatureAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Notification/GraphGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Notification/IO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Notification/Model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Notification/MultiThreading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Notification/Notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6149 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Notification/Optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Notification/RandomSamplers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Notification/SelectionGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Notification/UpROOT.py
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Notification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Notification/nTupler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:32:25.237464 analysisg-4.5.8/src/Plotting/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Plotting/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:32:25.237464 analysisg-4.5.8/src/SampleTracer/
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/SampleTracer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:32:25.237464 analysisg-4.5.8/src/Settings/
+-rw-r--r--   0 runner    (1001) docker     (127)     5567 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Settings/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:32:25.237464 analysisg-4.5.8/src/Submission/
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Submission/Condor.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Submission/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4412 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Submission/script_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:32:25.237464 analysisg-4.5.8/src/Templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:32:25.237464 analysisg-4.5.8/src/Templates/Features/
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Templates/Features/FeatureAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Templates/Features/FeatureTemplate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:32:25.237464 analysisg-4.5.8/src/Templates/Features/Jet/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Templates/Features/Jet/Edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Templates/Features/Jet/Graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Templates/Features/Jet/Node.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Templates/Features/Jet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:32:25.241464 analysisg-4.5.8/src/Templates/Features/TruthJet/
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Templates/Features/TruthJet/Edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Templates/Features/TruthJet/Graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Templates/Features/TruthJet/Node.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Templates/Features/TruthJet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:32:25.241464 analysisg-4.5.8/src/Templates/Features/TruthTop/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Templates/Features/TruthTop/Edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Templates/Features/TruthTop/Graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Templates/Features/TruthTop/Node.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Templates/Features/TruthTop/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:32:25.241464 analysisg-4.5.8/src/Templates/Features/TruthTopChildren/
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Templates/Features/TruthTopChildren/Edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Templates/Features/TruthTopChildren/Graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Templates/Features/TruthTopChildren/Node.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Templates/Features/TruthTopChildren/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Templates/Features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:32:25.241464 analysisg-4.5.8/src/Tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Tools/General.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5787 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Tools/MultiThreading.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/Tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:32:25.241464 analysisg-4.5.8/src/cmodules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/cmodules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:32:25.241464 analysisg-4.5.8/src/cmodules/abstractions/
+-rw-r--r--   0 runner    (1001) docker     (127)     6585 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/cmodules/abstractions/abstractions.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/cmodules/abstractions/abstractions.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12412 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/cmodules/abstractions/cytypes.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:32:25.241464 analysisg-4.5.8/src/cmodules/code/
+-rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/cmodules/code/code.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/cmodules/code/code.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:32:25.273464 analysisg-4.5.8/src/cmodules/cyincludes/
+-rw-r--r--   0 runner    (1001) docker     (127)  1030789 2024-05-27 20:32:22.000000 analysisg-4.5.8/src/cmodules/cyincludes/cycode.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/cmodules/cyincludes/cycode.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)    11818 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/cmodules/cyincludes/cycode.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/cmodules/cyincludes/cyepoch.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)  1227010 2024-05-27 20:32:22.000000 analysisg-4.5.8/src/cmodules/cyincludes/cyevent.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/cmodules/cyincludes/cyevent.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     8029 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/cmodules/cyincludes/cyevent.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)  1710540 2024-05-27 20:32:22.000000 analysisg-4.5.8/src/cmodules/cyincludes/cygraph.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/cmodules/cyincludes/cygraph.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)    14256 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/cmodules/cyincludes/cygraph.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)  2216395 2024-05-27 20:32:23.000000 analysisg-4.5.8/src/cmodules/cyincludes/cymetadata.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/cmodules/cyincludes/cymetadata.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)    24686 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/cmodules/cyincludes/cymetadata.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)  2407780 2024-05-27 20:32:23.000000 analysisg-4.5.8/src/cmodules/cyincludes/cyoptimizer.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6312 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/cmodules/cyincludes/cyoptimizer.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)    32208 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/cmodules/cyincludes/cyoptimizer.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)   842737 2024-05-27 20:32:22.000000 analysisg-4.5.8/src/cmodules/cyincludes/cyparticle.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/cmodules/cyincludes/cyparticle.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     8770 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/cmodules/cyincludes/cyparticle.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/cmodules/cyincludes/cyplotstruct.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)  2023505 2024-05-27 20:32:23.000000 analysisg-4.5.8/src/cmodules/cyincludes/cyplotting.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/cmodules/cyincludes/cyplotting.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)    29907 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/cmodules/cyincludes/cyplotting.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)  1524074 2024-05-27 20:32:23.000000 analysisg-4.5.8/src/cmodules/cyincludes/cyrunner.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/cmodules/cyincludes/cyrunner.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/cmodules/cyincludes/cyrunner.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)  4138415 2024-05-27 20:32:24.000000 analysisg-4.5.8/src/cmodules/cyincludes/cysampletracer.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/cmodules/cyincludes/cysampletracer.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)    55067 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/cmodules/cyincludes/cysampletracer.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)  1251042 2024-05-27 20:32:22.000000 analysisg-4.5.8/src/cmodules/cyincludes/cyselection.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/cmodules/cyincludes/cyselection.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)    12439 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/cmodules/cyincludes/cyselection.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)   856671 2024-05-27 20:32:22.000000 analysisg-4.5.8/src/cmodules/cyincludes/cytooling.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/cmodules/cyincludes/cytooling.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    10796 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/cmodules/cyincludes/cytools.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     8743 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/cmodules/cyincludes/cytypes.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)  1273497 2024-05-27 20:32:22.000000 analysisg-4.5.8/src/cmodules/cyincludes/cywrapping.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/cmodules/cyincludes/cywrapping.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)    18693 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/cmodules/cyincludes/cywrapping.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:32:25.273464 analysisg-4.5.8/src/cmodules/epoch/
+-rw-r--r--   0 runner    (1001) docker     (127)     5528 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/cmodules/epoch/epoch.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/cmodules/epoch/epoch.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:32:25.273464 analysisg-4.5.8/src/cmodules/event/
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/cmodules/event/event.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/cmodules/event/event.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:32:25.273464 analysisg-4.5.8/src/cmodules/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)     4031 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/cmodules/graph/graph.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/cmodules/graph/graph.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:32:25.273464 analysisg-4.5.8/src/cmodules/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)     9801 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/cmodules/metadata/metadata.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/cmodules/metadata/metadata.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:32:25.277464 analysisg-4.5.8/src/cmodules/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/cmodules/optimizer/optimizer.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/cmodules/optimizer/optimizer.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:32:25.277464 analysisg-4.5.8/src/cmodules/particle/
+-rw-r--r--   0 runner    (1001) docker     (127)     9313 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/cmodules/particle/particle.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/cmodules/particle/particle.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:32:25.277464 analysisg-4.5.8/src/cmodules/plotting/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/cmodules/plotting/plotting.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/cmodules/plotting/plotting.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:32:25.277464 analysisg-4.5.8/src/cmodules/root/
+-rw-r--r--   0 runner    (1001) docker     (127)    15660 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/cmodules/root/root.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)    11195 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/cmodules/root/root.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:32:25.277464 analysisg-4.5.8/src/cmodules/sampletracer/
+-rw-r--r--   0 runner    (1001) docker     (127)    16542 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/cmodules/sampletracer/sampletracer.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     6806 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/cmodules/sampletracer/sampletracer.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:32:25.277464 analysisg-4.5.8/src/cmodules/selection/
+-rw-r--r--   0 runner    (1001) docker     (127)     6694 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/cmodules/selection/selection.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-27 20:31:07.000000 analysisg-4.5.8/src/cmodules/selection/selection.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:32:25.281463 analysisg-4.5.8/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-27 20:31:08.000000 analysisg-4.5.8/test/test_ami.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12562 2024-05-27 20:31:08.000000 analysisg-4.5.8/test/test_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-05-27 20:31:08.000000 analysisg-4.5.8/test/test_cache_flush.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-05-27 20:31:08.000000 analysisg-4.5.8/test/test_event_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5159 2024-05-27 20:31:08.000000 analysisg-4.5.8/test/test_event_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6466 2024-05-27 20:31:08.000000 analysisg-4.5.8/test/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5128 2024-05-27 20:31:08.000000 analysisg-4.5.8/test/test_graph_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-05-27 20:31:08.000000 analysisg-4.5.8/test/test_graph_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-05-27 20:31:08.000000 analysisg-4.5.8/test/test_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-27 20:31:08.000000 analysisg-4.5.8/test/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10461 2024-05-27 20:31:08.000000 analysisg-4.5.8/test/test_machine_learning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-05-27 20:31:08.000000 analysisg-4.5.8/test/test_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-27 20:31:08.000000 analysisg-4.5.8/test/test_notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20233 2024-05-27 20:31:08.000000 analysisg-4.5.8/test/test_nusol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11275 2024-05-27 20:31:08.000000 analysisg-4.5.8/test/test_nusol_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4862 2024-05-27 20:31:08.000000 analysisg-4.5.8/test/test_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5189 2024-05-27 20:31:08.000000 analysisg-4.5.8/test/test_particle_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4545 2024-05-27 20:31:08.000000 analysisg-4.5.8/test/test_physics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6130 2024-05-27 20:31:08.000000 analysisg-4.5.8/test/test_selection_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-27 20:31:08.000000 analysisg-4.5.8/test/test_selection_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7296 2024-05-27 20:31:08.000000 analysisg-4.5.8/test/test_submission.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6688 2024-05-27 20:31:08.000000 analysisg-4.5.8/test/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8639 2024-05-27 20:31:08.000000 analysisg-4.5.8/test/test_tracer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5631 2024-05-27 20:31:08.000000 analysisg-4.5.8/test/test_transform.py
```

### Comparing `analysisg-4.5.7/AnalysisG.egg-info/PKG-INFO` & `analysisg-4.5.8/AnalysisG.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AnalysisG
-Version: 4.5.7
+Version: 4.5.8
 Author: woywoy123
 Project-URL: Homepage, https://github.com/woywoy123/AnalysisG
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `analysisg-4.5.7/AnalysisG.egg-info/SOURCES.txt` & `analysisg-4.5.8/AnalysisG.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/LICENSE` & `analysisg-4.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/PKG-INFO` & `analysisg-4.5.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AnalysisG
-Version: 4.5.7
+Version: 4.5.8
 Author: woywoy123
 Project-URL: Homepage, https://github.com/woywoy123/AnalysisG
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `analysisg-4.5.7/README.md` & `analysisg-4.5.8/README.md`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/pyproject.toml` & `analysisg-4.5.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "cython", "setuptools",
     "wheel", "torch"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "AnalysisG"
-version = "4.5.7"
+version = "4.5.8"
 authors = [{name = "woywoy123"}]
 readme.content-type = "text/markdown"
 readme.file = "README.md"
 requires-python = ">=3.7"
 dependencies = [
     "mplhep==0.3.28",
     "matplotlib==3.5.3",
```

### Comparing `analysisg-4.5.7/setup.py` & `analysisg-4.5.8/setup.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/Events/Deprecated/Event.py` & `analysisg-4.5.8/src/Events/Deprecated/Event.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/Events/Deprecated/EventIndex.py` & `analysisg-4.5.8/src/Events/Deprecated/EventIndex.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/Events/Deprecated/EventIndexParticle.py` & `analysisg-4.5.8/src/Events/Deprecated/EventIndexParticle.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/Events/Deprecated/EventParticles.py` & `analysisg-4.5.8/src/Events/Deprecated/EventParticles.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/Events/Deprecated/ExperimentalEvent.py` & `analysisg-4.5.8/src/Events/Deprecated/ExperimentalEvent.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/Events/Deprecated/ExperimentalParticles.py` & `analysisg-4.5.8/src/Events/Deprecated/ExperimentalParticles.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/Events/Events/bsm_4tops/Event.py` & `analysisg-4.5.8/src/Events/Events/bsm_4tops/Event.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/Events/Events/bsm_4tops/Particles.py` & `analysisg-4.5.8/src/Events/Events/bsm_4tops/Particles.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/Events/Events/mc20_ssml/Event.py` & `analysisg-4.5.8/src/Events/Events/mc20_ssml/Event.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/Events/Events/mc20_ssml/Particles.py` & `analysisg-4.5.8/src/Events/Events/mc20_ssml/Particles.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/Events/Events/ssml/Event.py` & `analysisg-4.5.8/src/Events/Events/ssml/Event.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/Events/Events/ssml/Particles.py` & `analysisg-4.5.8/src/Events/Events/ssml/Particles.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/Events/Graphs/EventGraphs.py` & `analysisg-4.5.8/src/Events/Graphs/EventGraphs.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/Generators/Analysis.py` & `analysisg-4.5.8/src/Generators/Analysis.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/Generators/EventGenerator.py` & `analysisg-4.5.8/src/Generators/EventGenerator.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/Generators/GraphGenerator.py` & `analysisg-4.5.8/src/Generators/GraphGenerator.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/Generators/Interfaces.py` & `analysisg-4.5.8/src/Generators/Interfaces.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/Generators/Optimizer.py` & `analysisg-4.5.8/src/Generators/Optimizer.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/Generators/SampleGenerator.py` & `analysisg-4.5.8/src/Generators/SampleGenerator.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/Generators/SelectionGenerator.py` & `analysisg-4.5.8/src/Generators/SelectionGenerator.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/IO/Pickle.py` & `analysisg-4.5.8/src/IO/Pickle.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/IO/UpROOT.py` & `analysisg-4.5.8/src/IO/UpROOT.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/IO/nTupler.py` & `analysisg-4.5.8/src/IO/nTupler.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/Model/LossFunctions.py` & `analysisg-4.5.8/src/Model/LossFunctions.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/Model/Model.py` & `analysisg-4.5.8/src/Model/Model.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/Notification/Analysis.py` & `analysisg-4.5.8/src/Notification/Analysis.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/Notification/Condor.py` & `analysisg-4.5.8/src/Notification/Condor.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/Notification/EventGenerator.py` & `analysisg-4.5.8/src/Notification/EventGenerator.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/Notification/FeatureAnalysis.py` & `analysisg-4.5.8/src/Notification/FeatureAnalysis.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/Notification/GraphGenerator.py` & `analysisg-4.5.8/src/Notification/GraphGenerator.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/Notification/IO.py` & `analysisg-4.5.8/src/Notification/IO.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/Notification/Model.py` & `analysisg-4.5.8/src/Notification/Model.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/Notification/Notification.py` & `analysisg-4.5.8/src/Notification/Notification.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/Notification/Optimization.py` & `analysisg-4.5.8/src/Notification/Optimization.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/Notification/RandomSamplers.py` & `analysisg-4.5.8/src/Notification/RandomSamplers.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/Notification/SelectionGenerator.py` & `analysisg-4.5.8/src/Notification/SelectionGenerator.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/Notification/UpROOT.py` & `analysisg-4.5.8/src/Notification/UpROOT.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/Notification/nTupler.py` & `analysisg-4.5.8/src/Notification/nTupler.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/Settings/__init__.py` & `analysisg-4.5.8/src/Settings/__init__.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/Submission/Condor.py` & `analysisg-4.5.8/src/Submission/Condor.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/Submission/script_builder.py` & `analysisg-4.5.8/src/Submission/script_builder.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/Templates/Features/FeatureAnalysis.py` & `analysisg-4.5.8/src/Templates/Features/FeatureAnalysis.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/Templates/Features/FeatureTemplate.py` & `analysisg-4.5.8/src/Templates/Features/FeatureTemplate.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/Templates/Features/Jet/Edge.py` & `analysisg-4.5.8/src/Templates/Features/Jet/Edge.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/Templates/Features/Jet/Node.py` & `analysisg-4.5.8/src/Templates/Features/Jet/Node.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/Templates/Features/TruthJet/Edge.py` & `analysisg-4.5.8/src/Templates/Features/TruthJet/Edge.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/Templates/Features/TruthJet/Node.py` & `analysisg-4.5.8/src/Templates/Features/TruthJet/Node.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/Templates/Features/TruthTopChildren/Graph.py` & `analysisg-4.5.8/src/Templates/Features/TruthTopChildren/Graph.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/Templates/__init__.py` & `analysisg-4.5.8/src/Templates/__init__.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/Tools/General.py` & `analysisg-4.5.8/src/Tools/General.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/Tools/MultiThreading.py` & `analysisg-4.5.8/src/Tools/MultiThreading.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/cmodules/abstractions/abstractions.cxx` & `analysisg-4.5.8/src/cmodules/abstractions/abstractions.cxx`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/cmodules/abstractions/abstractions.h` & `analysisg-4.5.8/src/cmodules/abstractions/abstractions.h`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/cmodules/abstractions/cytypes.h` & `analysisg-4.5.8/src/cmodules/abstractions/cytypes.h`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/cmodules/code/code.cxx` & `analysisg-4.5.8/src/cmodules/code/code.cxx`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/cmodules/code/code.h` & `analysisg-4.5.8/src/cmodules/code/code.h`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/cmodules/cyincludes/cycode.cpp` & `analysisg-4.5.8/src/cmodules/cyincludes/cycode.cpp`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/cmodules/cyincludes/cycode.pxd` & `analysisg-4.5.8/src/cmodules/cyincludes/cycode.pxd`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/cmodules/cyincludes/cycode.pyx` & `analysisg-4.5.8/src/cmodules/cyincludes/cycode.pyx`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/cmodules/cyincludes/cyepoch.pxd` & `analysisg-4.5.8/src/cmodules/cyincludes/cyepoch.pxd`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/cmodules/cyincludes/cyevent.cpp` & `analysisg-4.5.8/src/cmodules/cyincludes/cyevent.cpp`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/cmodules/cyincludes/cyevent.pxd` & `analysisg-4.5.8/src/cmodules/cyincludes/cyevent.pxd`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/cmodules/cyincludes/cyevent.pyx` & `analysisg-4.5.8/src/cmodules/cyincludes/cyevent.pyx`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/cmodules/cyincludes/cygraph.cpp` & `analysisg-4.5.8/src/cmodules/cyincludes/cygraph.cpp`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/cmodules/cyincludes/cygraph.pxd` & `analysisg-4.5.8/src/cmodules/cyincludes/cygraph.pxd`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/cmodules/cyincludes/cygraph.pyx` & `analysisg-4.5.8/src/cmodules/cyincludes/cygraph.pyx`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/cmodules/cyincludes/cymetadata.cpp` & `analysisg-4.5.8/src/cmodules/cyincludes/cymetadata.cpp`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/cmodules/cyincludes/cymetadata.pxd` & `analysisg-4.5.8/src/cmodules/cyincludes/cymetadata.pxd`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/cmodules/cyincludes/cymetadata.pyx` & `analysisg-4.5.8/src/cmodules/cyincludes/cymetadata.pyx`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/cmodules/cyincludes/cyoptimizer.cpp` & `analysisg-4.5.8/src/cmodules/cyincludes/cyoptimizer.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1657,15 +1657,15 @@
  *     int node_size
  */
 struct __pyx_t_9AnalysisG_9_cmodules_10cOptimizer_k_graphed {
   std::string pkl;
   int node_size;
 };
 
-/* "src/cmodules/cyincludes/cyoptimizer.pyx":471
+/* "src/cmodules/cyincludes/cyoptimizer.pyx":474
  * 
  * 
  * cdef class DataLoader:             # <<<<<<<<<<<<<<
  * 
  *     cdef CyOptimizer* ptr
  */
 struct __pyx_obj_9AnalysisG_9_cmodules_10cOptimizer_DataLoader {
@@ -1683,15 +1683,15 @@
   PyObject *online;
   bool purge;
   PyObject *sampletracer;
   int threads;
 };
 
 
-/* "src/cmodules/cyincludes/cyoptimizer.pyx":601
+/* "src/cmodules/cyincludes/cyoptimizer.pyx":604
  * 
  * 
  * cdef class cOptimizer:             # <<<<<<<<<<<<<<
  *     cdef CyOptimizer* ptr
  *     cdef DataLoader data
  */
 struct __pyx_obj_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer {
@@ -1706,29 +1706,29 @@
   bool metric_plots;
   int threads;
   PyObject *sampletracer;
 };
 
 
 
-/* "src/cmodules/cyincludes/cyoptimizer.pyx":471
+/* "src/cmodules/cyincludes/cyoptimizer.pyx":474
  * 
  * 
  * cdef class DataLoader:             # <<<<<<<<<<<<<<
  * 
  *     cdef CyOptimizer* ptr
  */
 
 struct __pyx_vtabstruct_9AnalysisG_9_cmodules_10cOptimizer_DataLoader {
   struct __pyx_obj_9AnalysisG_9_cmodules_10cOptimizer_DataLoader *(*set_batch)(struct __pyx_obj_9AnalysisG_9_cmodules_10cOptimizer_DataLoader *, int, int, std::string);
 };
 static struct __pyx_vtabstruct_9AnalysisG_9_cmodules_10cOptimizer_DataLoader *__pyx_vtabptr_9AnalysisG_9_cmodules_10cOptimizer_DataLoader;
 
 
-/* "src/cmodules/cyincludes/cyoptimizer.pyx":601
+/* "src/cmodules/cyincludes/cyoptimizer.pyx":604
  * 
  * 
  * cdef class cOptimizer:             # <<<<<<<<<<<<<<
  *     cdef CyOptimizer* ptr
  *     cdef DataLoader data
  */
 
@@ -2440,23 +2440,14 @@
 
 /* PyObjectCallMethod1.proto */
 static PyObject* __Pyx_PyObject_CallMethod1(PyObject* obj, PyObject* method_name, PyObject* arg);
 
 /* append.proto */
 static CYTHON_INLINE int __Pyx_PyObject_Append(PyObject* L, PyObject* x);
 
-/* PyObjectSetAttrStr.proto */
-#if CYTHON_USE_TYPE_SLOTS
-#define __Pyx_PyObject_DelAttrStr(o,n) __Pyx_PyObject_SetAttrStr(o, n, NULL)
-static CYTHON_INLINE int __Pyx_PyObject_SetAttrStr(PyObject* obj, PyObject* attr_name, PyObject* value);
-#else
-#define __Pyx_PyObject_DelAttrStr(o,n)   PyObject_DelAttr(o,n)
-#define __Pyx_PyObject_SetAttrStr(o,n,v) PyObject_SetAttr(o,n,v)
-#endif
-
 /* KeywordStringCheck.proto */
 static int __Pyx_CheckKeywordStrings(PyObject *kw, const char* function_name, int kw_allowed);
 
 /* py_dict_clear.proto */
 #define __Pyx_PyDict_Clear(d) (PyDict_Clear(d), 0)
 
 /* unicode_tailmatch.proto */
@@ -2476,14 +2467,23 @@
 #define __Pyx_TypeCheck2(obj, type1, type2) (PyObject_TypeCheck(obj, (PyTypeObject *)type1) || PyObject_TypeCheck(obj, (PyTypeObject *)type2))
 #define __Pyx_PyErr_GivenExceptionMatches(err, type) PyErr_GivenExceptionMatches(err, type)
 #define __Pyx_PyErr_GivenExceptionMatches2(err, type1, type2) (PyErr_GivenExceptionMatches(err, type1) || PyErr_GivenExceptionMatches(err, type2))
 #endif
 #define __Pyx_PyErr_ExceptionMatches2(err1, err2)  __Pyx_PyErr_GivenExceptionMatches2(__Pyx_PyErr_CurrentExceptionType(), err1, err2)
 #define __Pyx_PyException_Check(obj) __Pyx_TypeCheck(obj, PyExc_Exception)
 
+/* PyObjectSetAttrStr.proto */
+#if CYTHON_USE_TYPE_SLOTS
+#define __Pyx_PyObject_DelAttrStr(o,n) __Pyx_PyObject_SetAttrStr(o, n, NULL)
+static CYTHON_INLINE int __Pyx_PyObject_SetAttrStr(PyObject* obj, PyObject* attr_name, PyObject* value);
+#else
+#define __Pyx_PyObject_DelAttrStr(o,n)   PyObject_DelAttr(o,n)
+#define __Pyx_PyObject_SetAttrStr(o,n,v) PyObject_SetAttr(o,n,v)
+#endif
+
 /* IncludeStructmemberH.proto */
 #include <structmember.h>
 
 /* FixUpExtensionType.proto */
 #if CYTHON_USE_TYPE_SPECS
 static int __Pyx_fix_up_extension_type_from_spec(PyType_Spec *spec, PyTypeObject *type);
 #endif
@@ -3161,14 +3161,15 @@
 static const char __pyx_k_getstate[] = "__getstate__";
 static const char __pyx_k_makedirs[] = "makedirs";
 static const char __pyx_k_makelist[] = "makelist";
 static const char __pyx_k_pickle_2[] = "_pickle";
 static const char __pyx_k_recreate[] = "recreate";
 static const char __pyx_k_setstate[] = "__setstate__";
 static const char __pyx_k_training[] = "training";
+static const char __pyx_k_Histogram[] = "Histogram";
 static const char __pyx_k_ROC_Curve[] = "ROC Curve: ";
 static const char __pyx_k_ROC_Epoch[] = "/ROC/Epoch-";
 static const char __pyx_k_TypeError[] = "TypeError";
 static const char __pyx_k_acc_train[] = "acc_train";
 static const char __pyx_k_acc_valid[] = "acc_valid";
 static const char __pyx_k_auc_train[] = "auc_train";
 static const char __pyx_k_auc_valid[] = "auc_valid";
@@ -3528,14 +3529,15 @@
   PyObject *__pyx_n_s_FileExistsError;
   PyObject *__pyx_n_s_FileNotFoundError;
   PyObject *__pyx_n_u_Filename;
   PyObject *__pyx_n_s_FlushGraphs;
   PyObject *__pyx_n_s_GetHDF5Hashes;
   PyObject *__pyx_n_u_Graph;
   PyObject *__pyx_kp_u_GraphCache;
+  PyObject *__pyx_n_u_Histogram;
   PyObject *__pyx_n_u_Histograms;
   PyObject *__pyx_n_s_IndexError;
   PyObject *__pyx_n_s_KeyError;
   PyObject *__pyx_n_u_L;
   PyObject *__pyx_n_u_Lines;
   PyObject *__pyx_kp_u_Loss_Curve_for;
   PyObject *__pyx_kp_u_Loss_arb;
@@ -3928,15 +3930,15 @@
   PyObject *__pyx_n_u_xMin;
   PyObject *__pyx_n_u_xStep;
   PyObject *__pyx_n_u_xTitle;
   PyObject *__pyx_n_u_yData;
   PyObject *__pyx_n_u_yDataDown;
   PyObject *__pyx_n_u_yDataUp;
   PyObject *__pyx_n_u_yLogarithmic;
-  PyObject *__pyx_n_s_yMax;
+  PyObject *__pyx_n_u_yMax;
   PyObject *__pyx_n_u_yMin;
   PyObject *__pyx_n_u_yTitle;
   PyObject *__pyx_int_0;
   PyObject *__pyx_int_1;
   PyObject *__pyx_int_5;
   PyObject *__pyx_int_100;
   PyObject *__pyx_int_300;
@@ -4115,14 +4117,15 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_FileExistsError);
   Py_CLEAR(clear_module_state->__pyx_n_s_FileNotFoundError);
   Py_CLEAR(clear_module_state->__pyx_n_u_Filename);
   Py_CLEAR(clear_module_state->__pyx_n_s_FlushGraphs);
   Py_CLEAR(clear_module_state->__pyx_n_s_GetHDF5Hashes);
   Py_CLEAR(clear_module_state->__pyx_n_u_Graph);
   Py_CLEAR(clear_module_state->__pyx_kp_u_GraphCache);
+  Py_CLEAR(clear_module_state->__pyx_n_u_Histogram);
   Py_CLEAR(clear_module_state->__pyx_n_u_Histograms);
   Py_CLEAR(clear_module_state->__pyx_n_s_IndexError);
   Py_CLEAR(clear_module_state->__pyx_n_s_KeyError);
   Py_CLEAR(clear_module_state->__pyx_n_u_L);
   Py_CLEAR(clear_module_state->__pyx_n_u_Lines);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Loss_Curve_for);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Loss_arb);
@@ -4515,15 +4518,15 @@
   Py_CLEAR(clear_module_state->__pyx_n_u_xMin);
   Py_CLEAR(clear_module_state->__pyx_n_u_xStep);
   Py_CLEAR(clear_module_state->__pyx_n_u_xTitle);
   Py_CLEAR(clear_module_state->__pyx_n_u_yData);
   Py_CLEAR(clear_module_state->__pyx_n_u_yDataDown);
   Py_CLEAR(clear_module_state->__pyx_n_u_yDataUp);
   Py_CLEAR(clear_module_state->__pyx_n_u_yLogarithmic);
-  Py_CLEAR(clear_module_state->__pyx_n_s_yMax);
+  Py_CLEAR(clear_module_state->__pyx_n_u_yMax);
   Py_CLEAR(clear_module_state->__pyx_n_u_yMin);
   Py_CLEAR(clear_module_state->__pyx_n_u_yTitle);
   Py_CLEAR(clear_module_state->__pyx_int_0);
   Py_CLEAR(clear_module_state->__pyx_int_1);
   Py_CLEAR(clear_module_state->__pyx_int_5);
   Py_CLEAR(clear_module_state->__pyx_int_100);
   Py_CLEAR(clear_module_state->__pyx_int_300);
@@ -4680,14 +4683,15 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_FileExistsError);
   Py_VISIT(traverse_module_state->__pyx_n_s_FileNotFoundError);
   Py_VISIT(traverse_module_state->__pyx_n_u_Filename);
   Py_VISIT(traverse_module_state->__pyx_n_s_FlushGraphs);
   Py_VISIT(traverse_module_state->__pyx_n_s_GetHDF5Hashes);
   Py_VISIT(traverse_module_state->__pyx_n_u_Graph);
   Py_VISIT(traverse_module_state->__pyx_kp_u_GraphCache);
+  Py_VISIT(traverse_module_state->__pyx_n_u_Histogram);
   Py_VISIT(traverse_module_state->__pyx_n_u_Histograms);
   Py_VISIT(traverse_module_state->__pyx_n_s_IndexError);
   Py_VISIT(traverse_module_state->__pyx_n_s_KeyError);
   Py_VISIT(traverse_module_state->__pyx_n_u_L);
   Py_VISIT(traverse_module_state->__pyx_n_u_Lines);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Loss_Curve_for);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Loss_arb);
@@ -5080,15 +5084,15 @@
   Py_VISIT(traverse_module_state->__pyx_n_u_xMin);
   Py_VISIT(traverse_module_state->__pyx_n_u_xStep);
   Py_VISIT(traverse_module_state->__pyx_n_u_xTitle);
   Py_VISIT(traverse_module_state->__pyx_n_u_yData);
   Py_VISIT(traverse_module_state->__pyx_n_u_yDataDown);
   Py_VISIT(traverse_module_state->__pyx_n_u_yDataUp);
   Py_VISIT(traverse_module_state->__pyx_n_u_yLogarithmic);
-  Py_VISIT(traverse_module_state->__pyx_n_s_yMax);
+  Py_VISIT(traverse_module_state->__pyx_n_u_yMax);
   Py_VISIT(traverse_module_state->__pyx_n_u_yMin);
   Py_VISIT(traverse_module_state->__pyx_n_u_yTitle);
   Py_VISIT(traverse_module_state->__pyx_int_0);
   Py_VISIT(traverse_module_state->__pyx_int_1);
   Py_VISIT(traverse_module_state->__pyx_int_5);
   Py_VISIT(traverse_module_state->__pyx_int_100);
   Py_VISIT(traverse_module_state->__pyx_int_300);
@@ -5283,14 +5287,15 @@
 #define __pyx_n_s_FileExistsError __pyx_mstate_global->__pyx_n_s_FileExistsError
 #define __pyx_n_s_FileNotFoundError __pyx_mstate_global->__pyx_n_s_FileNotFoundError
 #define __pyx_n_u_Filename __pyx_mstate_global->__pyx_n_u_Filename
 #define __pyx_n_s_FlushGraphs __pyx_mstate_global->__pyx_n_s_FlushGraphs
 #define __pyx_n_s_GetHDF5Hashes __pyx_mstate_global->__pyx_n_s_GetHDF5Hashes
 #define __pyx_n_u_Graph __pyx_mstate_global->__pyx_n_u_Graph
 #define __pyx_kp_u_GraphCache __pyx_mstate_global->__pyx_kp_u_GraphCache
+#define __pyx_n_u_Histogram __pyx_mstate_global->__pyx_n_u_Histogram
 #define __pyx_n_u_Histograms __pyx_mstate_global->__pyx_n_u_Histograms
 #define __pyx_n_s_IndexError __pyx_mstate_global->__pyx_n_s_IndexError
 #define __pyx_n_s_KeyError __pyx_mstate_global->__pyx_n_s_KeyError
 #define __pyx_n_u_L __pyx_mstate_global->__pyx_n_u_L
 #define __pyx_n_u_Lines __pyx_mstate_global->__pyx_n_u_Lines
 #define __pyx_kp_u_Loss_Curve_for __pyx_mstate_global->__pyx_kp_u_Loss_Curve_for
 #define __pyx_kp_u_Loss_arb __pyx_mstate_global->__pyx_kp_u_Loss_arb
@@ -5683,15 +5688,15 @@
 #define __pyx_n_u_xMin __pyx_mstate_global->__pyx_n_u_xMin
 #define __pyx_n_u_xStep __pyx_mstate_global->__pyx_n_u_xStep
 #define __pyx_n_u_xTitle __pyx_mstate_global->__pyx_n_u_xTitle
 #define __pyx_n_u_yData __pyx_mstate_global->__pyx_n_u_yData
 #define __pyx_n_u_yDataDown __pyx_mstate_global->__pyx_n_u_yDataDown
 #define __pyx_n_u_yDataUp __pyx_mstate_global->__pyx_n_u_yDataUp
 #define __pyx_n_u_yLogarithmic __pyx_mstate_global->__pyx_n_u_yLogarithmic
-#define __pyx_n_s_yMax __pyx_mstate_global->__pyx_n_s_yMax
+#define __pyx_n_u_yMax __pyx_mstate_global->__pyx_n_u_yMax
 #define __pyx_n_u_yMin __pyx_mstate_global->__pyx_n_u_yMin
 #define __pyx_n_u_yTitle __pyx_mstate_global->__pyx_n_u_yTitle
 #define __pyx_int_0 __pyx_mstate_global->__pyx_int_0
 #define __pyx_int_1 __pyx_mstate_global->__pyx_int_1
 #define __pyx_int_5 __pyx_mstate_global->__pyx_int_5
 #define __pyx_int_100 __pyx_mstate_global->__pyx_int_100
 #define __pyx_int_300 __pyx_mstate_global->__pyx_int_300
@@ -28254,15 +28259,15 @@
       }
 
       /* "src/cmodules/cyincludes/cyoptimizer.pyx":141
  *             try: xData += ev_t[file_n][x]["xData"]
  *             except KeyError: pass
  *             try: xData += tr_t[file_n][x]["xData"]             # <<<<<<<<<<<<<<
  *             except KeyError: pass
- *             tmpl["Histograms"] += [TH1F(**{"Title" : "truth", "xData" : xData})]
+ * 
  */
       {
         __Pyx_PyThreadState_declare
         __Pyx_PyThreadState_assign
         __Pyx_ExceptionSave(&__pyx_t_10, &__pyx_t_11, &__pyx_t_12);
         __Pyx_XGOTREF(__pyx_t_10);
         __Pyx_XGOTREF(__pyx_t_11);
@@ -28300,30 +28305,30 @@
         __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
 
         /* "src/cmodules/cyincludes/cyoptimizer.pyx":142
  *             except KeyError: pass
  *             try: xData += tr_t[file_n][x]["xData"]
  *             except KeyError: pass             # <<<<<<<<<<<<<<
- *             tmpl["Histograms"] += [TH1F(**{"Title" : "truth", "xData" : xData})]
- *             tmpl["yLogarithmic"] = True
+ * 
+ *             tmpl["Histogram"] = TH1F(**{"Title" : "truth", "xData" : xData})
  */
         __pyx_t_15 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_KeyError);
         if (__pyx_t_15) {
           __Pyx_ErrRestore(0,0,0);
           goto __pyx_L72_exception_handled;
         }
         goto __pyx_L73_except_error;
 
         /* "src/cmodules/cyincludes/cyoptimizer.pyx":141
  *             try: xData += ev_t[file_n][x]["xData"]
  *             except KeyError: pass
  *             try: xData += tr_t[file_n][x]["xData"]             # <<<<<<<<<<<<<<
  *             except KeyError: pass
- *             tmpl["Histograms"] += [TH1F(**{"Title" : "truth", "xData" : xData})]
+ * 
  */
         __pyx_L73_except_error:;
         __Pyx_XGIVEREF(__pyx_t_10);
         __Pyx_XGIVEREF(__pyx_t_11);
         __Pyx_XGIVEREF(__pyx_t_12);
         __Pyx_ExceptionReset(__pyx_t_10, __pyx_t_11, __pyx_t_12);
         goto __pyx_L1_error;
@@ -28331,132 +28336,120 @@
         __Pyx_XGIVEREF(__pyx_t_10);
         __Pyx_XGIVEREF(__pyx_t_11);
         __Pyx_XGIVEREF(__pyx_t_12);
         __Pyx_ExceptionReset(__pyx_t_10, __pyx_t_11, __pyx_t_12);
         __pyx_L78_try_end:;
       }
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":143
- *             try: xData += tr_t[file_n][x]["xData"]
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":144
  *             except KeyError: pass
- *             tmpl["Histograms"] += [TH1F(**{"Title" : "truth", "xData" : xData})]             # <<<<<<<<<<<<<<
+ * 
+ *             tmpl["Histogram"] = TH1F(**{"Title" : "truth", "xData" : xData})             # <<<<<<<<<<<<<<
  *             tmpl["yLogarithmic"] = True
- *             th = TH1F(**tmpl)
+ *             tmpl["Stack"] = True
  */
-      if (unlikely(__pyx_v_tmpl == Py_None)) {
-        PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-        __PYX_ERR(0, 143, __pyx_L1_error)
-      }
-      __Pyx_INCREF(__pyx_v_tmpl);
-      __pyx_t_16 = __pyx_v_tmpl;
-      __Pyx_INCREF(__pyx_n_u_Histograms);
-      __pyx_t_17 = __pyx_n_u_Histograms;
-      if (unlikely(__pyx_t_16 == Py_None)) {
-        PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-        __PYX_ERR(0, 143, __pyx_L1_error)
-      }
-      __pyx_t_19 = __Pyx_PyDict_GetItem(__pyx_t_16, __pyx_t_17); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 143, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_19, __pyx_n_s_TH1F); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 144, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_19);
-      __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_TH1F); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 143, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 144, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_18 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 143, __pyx_L1_error)
+      if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_Title, __pyx_n_u_truth) < 0) __PYX_ERR(0, 144, __pyx_L1_error)
+      if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_xData, __pyx_v_xData) < 0) __PYX_ERR(0, 144, __pyx_L1_error)
+      __pyx_t_18 = __Pyx_PyObject_Call(__pyx_t_19, __pyx_empty_tuple, __pyx_t_2); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 144, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_18);
-      if (PyDict_SetItem(__pyx_t_18, __pyx_n_u_Title, __pyx_n_u_truth) < 0) __PYX_ERR(0, 143, __pyx_L1_error)
-      if (PyDict_SetItem(__pyx_t_18, __pyx_n_u_xData, __pyx_v_xData) < 0) __PYX_ERR(0, 143, __pyx_L1_error)
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_empty_tuple, __pyx_t_18); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 143, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_8);
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
-      __pyx_t_18 = PyList_New(1); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 143, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_18);
-      __Pyx_GIVEREF(__pyx_t_8);
-      if (__Pyx_PyList_SET_ITEM(__pyx_t_18, 0, __pyx_t_8)) __PYX_ERR(0, 143, __pyx_L1_error);
-      __pyx_t_8 = 0;
-      __pyx_t_8 = PyNumber_InPlaceAdd(__pyx_t_19, __pyx_t_18); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 143, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_8);
       __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
-      __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
-      if (unlikely(__pyx_t_16 == Py_None)) {
+      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+      if (unlikely(__pyx_v_tmpl == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-        __PYX_ERR(0, 143, __pyx_L1_error)
+        __PYX_ERR(0, 144, __pyx_L1_error)
       }
-      if (unlikely((PyDict_SetItem(__pyx_t_16, __pyx_t_17, __pyx_t_8) < 0))) __PYX_ERR(0, 143, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
-      __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
+      if (unlikely((PyDict_SetItem(__pyx_v_tmpl, __pyx_n_u_Histogram, __pyx_t_18) < 0))) __PYX_ERR(0, 144, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":144
- *             except KeyError: pass
- *             tmpl["Histograms"] += [TH1F(**{"Title" : "truth", "xData" : xData})]
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":145
+ * 
+ *             tmpl["Histogram"] = TH1F(**{"Title" : "truth", "xData" : xData})
  *             tmpl["yLogarithmic"] = True             # <<<<<<<<<<<<<<
+ *             tmpl["Stack"] = True
+ *             th = TH1F(**tmpl)
+ */
+      if (unlikely(__pyx_v_tmpl == Py_None)) {
+        PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
+        __PYX_ERR(0, 145, __pyx_L1_error)
+      }
+      if (unlikely((PyDict_SetItem(__pyx_v_tmpl, __pyx_n_u_yLogarithmic, Py_True) < 0))) __PYX_ERR(0, 145, __pyx_L1_error)
+
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":146
+ *             tmpl["Histogram"] = TH1F(**{"Title" : "truth", "xData" : xData})
+ *             tmpl["yLogarithmic"] = True
+ *             tmpl["Stack"] = True             # <<<<<<<<<<<<<<
  *             th = TH1F(**tmpl)
  *             th.SaveFigure()
  */
       if (unlikely(__pyx_v_tmpl == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-        __PYX_ERR(0, 144, __pyx_L1_error)
+        __PYX_ERR(0, 146, __pyx_L1_error)
       }
-      if (unlikely((PyDict_SetItem(__pyx_v_tmpl, __pyx_n_u_yLogarithmic, Py_True) < 0))) __PYX_ERR(0, 144, __pyx_L1_error)
+      if (unlikely((PyDict_SetItem(__pyx_v_tmpl, __pyx_n_u_Stack, Py_True) < 0))) __PYX_ERR(0, 146, __pyx_L1_error)
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":145
- *             tmpl["Histograms"] += [TH1F(**{"Title" : "truth", "xData" : xData})]
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":147
  *             tmpl["yLogarithmic"] = True
+ *             tmpl["Stack"] = True
  *             th = TH1F(**tmpl)             # <<<<<<<<<<<<<<
  *             th.SaveFigure()
  *             del th
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_TH1F); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 145, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_8);
+      __Pyx_GetModuleGlobalName(__pyx_t_18, __pyx_n_s_TH1F); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 147, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_18);
       if (unlikely(__pyx_v_tmpl == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "argument after ** must be a mapping, not NoneType");
-        __PYX_ERR(0, 145, __pyx_L1_error)
+        __PYX_ERR(0, 147, __pyx_L1_error)
       }
-      __pyx_t_18 = PyDict_Copy(__pyx_v_tmpl); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 145, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_18);
-      __pyx_t_19 = __Pyx_PyObject_Call(__pyx_t_8, __pyx_empty_tuple, __pyx_t_18); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 145, __pyx_L1_error)
+      __pyx_t_2 = PyDict_Copy(__pyx_v_tmpl); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 147, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_2);
+      __pyx_t_19 = __Pyx_PyObject_Call(__pyx_t_18, __pyx_empty_tuple, __pyx_t_2); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 147, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_19);
-      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
+      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __pyx_v_th = __pyx_t_19;
       __pyx_t_19 = 0;
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":146
- *             tmpl["yLogarithmic"] = True
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":148
+ *             tmpl["Stack"] = True
  *             th = TH1F(**tmpl)
  *             th.SaveFigure()             # <<<<<<<<<<<<<<
  *             del th
  * 
  */
-      __pyx_t_18 = __Pyx_PyObject_GetAttrStr(__pyx_v_th, __pyx_n_s_SaveFigure); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 146, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_18);
-      __pyx_t_8 = NULL;
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_th, __pyx_n_s_SaveFigure); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 148, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_2);
+      __pyx_t_18 = NULL;
       __pyx_t_15 = 0;
       #if CYTHON_UNPACK_METHODS
-      if (likely(PyMethod_Check(__pyx_t_18))) {
-        __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_18);
-        if (likely(__pyx_t_8)) {
-          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_18);
-          __Pyx_INCREF(__pyx_t_8);
+      if (likely(PyMethod_Check(__pyx_t_2))) {
+        __pyx_t_18 = PyMethod_GET_SELF(__pyx_t_2);
+        if (likely(__pyx_t_18)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+          __Pyx_INCREF(__pyx_t_18);
           __Pyx_INCREF(function);
-          __Pyx_DECREF_SET(__pyx_t_18, function);
+          __Pyx_DECREF_SET(__pyx_t_2, function);
           __pyx_t_15 = 1;
         }
       }
       #endif
       {
-        PyObject *__pyx_callargs[2] = {__pyx_t_8, NULL};
-        __pyx_t_19 = __Pyx_PyObject_FastCall(__pyx_t_18, __pyx_callargs+1-__pyx_t_15, 0+__pyx_t_15);
-        __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-        if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 146, __pyx_L1_error)
+        PyObject *__pyx_callargs[2] = {__pyx_t_18, NULL};
+        __pyx_t_19 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_15, 0+__pyx_t_15);
+        __Pyx_XDECREF(__pyx_t_18); __pyx_t_18 = 0;
+        if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 148, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_19);
-        __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
+        __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       }
       __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":147
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":149
  *             th = TH1F(**tmpl)
  *             th.SaveFigure()
  *             del th             # <<<<<<<<<<<<<<
  * 
  * cdef dict collapse_points(map[string, vector[point_t]]* tmp, int epoch, dict lines, str mode, report_t* state, str metric):
  */
       __Pyx_DECREF(__pyx_v_th); __pyx_v_th = 0;
@@ -28500,15 +28493,15 @@
   __Pyx_XDECREF(__pyx_v_kf);
   __Pyx_XDECREF(__pyx_v_x);
   __Pyx_XDECREF(__pyx_v_file_n);
   __Pyx_XDECREF(__pyx_v_th);
   __Pyx_RefNannyFinishContext();
 }
 
-/* "src/cmodules/cyincludes/cyoptimizer.pyx":149
+/* "src/cmodules/cyincludes/cyoptimizer.pyx":151
  *             del th
  * 
  * cdef dict collapse_points(map[string, vector[point_t]]* tmp, int epoch, dict lines, str mode, report_t* state, str metric):             # <<<<<<<<<<<<<<
  *     cdef pair[string, vector[point_t]]itv
  *     cdef point_t pnt
  */
 
@@ -28529,682 +28522,682 @@
   int __pyx_t_9;
   float __pyx_t_10;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("collapse_points", 1);
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":154
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":156
  *     cdef str var_name
  * 
  *     for itv in dereference(tmp):             # <<<<<<<<<<<<<<
  *         pnt = point_t()
  *         stats(&itv.second, &pnt)
  */
   __pyx_t_2 = &(*__pyx_v_tmp);
   __pyx_t_1 = __pyx_t_2->begin();
   for (;;) {
     if (!(__pyx_t_1 != __pyx_t_2->end())) break;
     __pyx_t_3 = *__pyx_t_1;
     ++__pyx_t_1;
     __pyx_v_itv = __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_3);
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":155
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":157
  * 
  *     for itv in dereference(tmp):
  *         pnt = point_t()             # <<<<<<<<<<<<<<
  *         stats(&itv.second, &pnt)
  *         var_name = env(itv.first)
  */
     __pyx_v_pnt = __pyx_t_4;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":156
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":158
  *     for itv in dereference(tmp):
  *         pnt = point_t()
  *         stats(&itv.second, &pnt)             # <<<<<<<<<<<<<<
  *         var_name = env(itv.first)
  *         if var_name not in lines: lines[var_name] = {}
  */
-    __pyx_t_5 = __pyx_f_7cyepoch_stats((&__pyx_v_itv.second), (&__pyx_v_pnt)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 156, __pyx_L1_error)
+    __pyx_t_5 = __pyx_f_7cyepoch_stats((&__pyx_v_itv.second), (&__pyx_v_pnt)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 158, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":157
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":159
  *         pnt = point_t()
  *         stats(&itv.second, &pnt)
  *         var_name = env(itv.first)             # <<<<<<<<<<<<<<
  *         if var_name not in lines: lines[var_name] = {}
  *         if mode not in lines[var_name]:
  */
-    __pyx_t_5 = __pyx_f_7cytools_env(__pyx_v_itv.first); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 157, __pyx_L1_error)
+    __pyx_t_5 = __pyx_f_7cytools_env(__pyx_v_itv.first); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 159, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_XDECREF_SET(__pyx_v_var_name, ((PyObject*)__pyx_t_5));
     __pyx_t_5 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":158
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":160
  *         stats(&itv.second, &pnt)
  *         var_name = env(itv.first)
  *         if var_name not in lines: lines[var_name] = {}             # <<<<<<<<<<<<<<
  *         if mode not in lines[var_name]:
  *             lines[var_name][mode] = {"yDataDown" : [], "yDataUp" : [], "xData" : [], "yData" : [], "Title" : mode}
  */
     if (unlikely(__pyx_v_lines == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-      __PYX_ERR(0, 158, __pyx_L1_error)
+      __PYX_ERR(0, 160, __pyx_L1_error)
     }
-    __pyx_t_6 = (__Pyx_PyDict_ContainsTF(__pyx_v_var_name, __pyx_v_lines, Py_NE)); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 158, __pyx_L1_error)
+    __pyx_t_6 = (__Pyx_PyDict_ContainsTF(__pyx_v_var_name, __pyx_v_lines, Py_NE)); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 160, __pyx_L1_error)
     if (__pyx_t_6) {
-      __pyx_t_5 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 158, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 160, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       if (unlikely(__pyx_v_lines == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-        __PYX_ERR(0, 158, __pyx_L1_error)
+        __PYX_ERR(0, 160, __pyx_L1_error)
       }
-      if (unlikely((PyDict_SetItem(__pyx_v_lines, __pyx_v_var_name, __pyx_t_5) < 0))) __PYX_ERR(0, 158, __pyx_L1_error)
+      if (unlikely((PyDict_SetItem(__pyx_v_lines, __pyx_v_var_name, __pyx_t_5) < 0))) __PYX_ERR(0, 160, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     }
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":159
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":161
  *         var_name = env(itv.first)
  *         if var_name not in lines: lines[var_name] = {}
  *         if mode not in lines[var_name]:             # <<<<<<<<<<<<<<
  *             lines[var_name][mode] = {"yDataDown" : [], "yDataUp" : [], "xData" : [], "yData" : [], "Title" : mode}
  *         lines[var_name][mode]["yDataDown"].append(pnt.stdev)
  */
     if (unlikely(__pyx_v_lines == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 159, __pyx_L1_error)
+      __PYX_ERR(0, 161, __pyx_L1_error)
     }
-    __pyx_t_5 = __Pyx_PyDict_GetItem(__pyx_v_lines, __pyx_v_var_name); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 159, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyDict_GetItem(__pyx_v_lines, __pyx_v_var_name); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 161, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_6 = (__Pyx_PySequence_ContainsTF(__pyx_v_mode, __pyx_t_5, Py_NE)); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 159, __pyx_L1_error)
+    __pyx_t_6 = (__Pyx_PySequence_ContainsTF(__pyx_v_mode, __pyx_t_5, Py_NE)); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 161, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     if (__pyx_t_6) {
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":160
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":162
  *         if var_name not in lines: lines[var_name] = {}
  *         if mode not in lines[var_name]:
  *             lines[var_name][mode] = {"yDataDown" : [], "yDataUp" : [], "xData" : [], "yData" : [], "Title" : mode}             # <<<<<<<<<<<<<<
  *         lines[var_name][mode]["yDataDown"].append(pnt.stdev)
  *         lines[var_name][mode]["yDataUp"].append(pnt.stdev)
  */
-      __pyx_t_5 = __Pyx_PyDict_NewPresized(5); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 160, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyDict_NewPresized(5); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 162, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_7 = PyList_New(0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 160, __pyx_L1_error)
+      __pyx_t_7 = PyList_New(0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 162, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
-      if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_yDataDown, __pyx_t_7) < 0) __PYX_ERR(0, 160, __pyx_L1_error)
+      if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_yDataDown, __pyx_t_7) < 0) __PYX_ERR(0, 162, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      __pyx_t_7 = PyList_New(0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 160, __pyx_L1_error)
+      __pyx_t_7 = PyList_New(0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 162, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
-      if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_yDataUp, __pyx_t_7) < 0) __PYX_ERR(0, 160, __pyx_L1_error)
+      if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_yDataUp, __pyx_t_7) < 0) __PYX_ERR(0, 162, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      __pyx_t_7 = PyList_New(0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 160, __pyx_L1_error)
+      __pyx_t_7 = PyList_New(0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 162, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
-      if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_xData, __pyx_t_7) < 0) __PYX_ERR(0, 160, __pyx_L1_error)
+      if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_xData, __pyx_t_7) < 0) __PYX_ERR(0, 162, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      __pyx_t_7 = PyList_New(0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 160, __pyx_L1_error)
+      __pyx_t_7 = PyList_New(0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 162, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
-      if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_yData, __pyx_t_7) < 0) __PYX_ERR(0, 160, __pyx_L1_error)
+      if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_yData, __pyx_t_7) < 0) __PYX_ERR(0, 162, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_Title, __pyx_v_mode) < 0) __PYX_ERR(0, 160, __pyx_L1_error)
+      if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_Title, __pyx_v_mode) < 0) __PYX_ERR(0, 162, __pyx_L1_error)
       if (unlikely(__pyx_v_lines == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-        __PYX_ERR(0, 160, __pyx_L1_error)
+        __PYX_ERR(0, 162, __pyx_L1_error)
       }
-      __pyx_t_7 = __Pyx_PyDict_GetItem(__pyx_v_lines, __pyx_v_var_name); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 160, __pyx_L1_error)
+      __pyx_t_7 = __Pyx_PyDict_GetItem(__pyx_v_lines, __pyx_v_var_name); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 162, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
-      if (unlikely((PyObject_SetItem(__pyx_t_7, __pyx_v_mode, __pyx_t_5) < 0))) __PYX_ERR(0, 160, __pyx_L1_error)
+      if (unlikely((PyObject_SetItem(__pyx_t_7, __pyx_v_mode, __pyx_t_5) < 0))) __PYX_ERR(0, 162, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":159
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":161
  *         var_name = env(itv.first)
  *         if var_name not in lines: lines[var_name] = {}
  *         if mode not in lines[var_name]:             # <<<<<<<<<<<<<<
  *             lines[var_name][mode] = {"yDataDown" : [], "yDataUp" : [], "xData" : [], "yData" : [], "Title" : mode}
  *         lines[var_name][mode]["yDataDown"].append(pnt.stdev)
  */
     }
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":161
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":163
  *         if mode not in lines[var_name]:
  *             lines[var_name][mode] = {"yDataDown" : [], "yDataUp" : [], "xData" : [], "yData" : [], "Title" : mode}
  *         lines[var_name][mode]["yDataDown"].append(pnt.stdev)             # <<<<<<<<<<<<<<
  *         lines[var_name][mode]["yDataUp"].append(pnt.stdev)
  *         lines[var_name][mode]["yData"].append(pnt.average)
  */
     if (unlikely(__pyx_v_lines == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 161, __pyx_L1_error)
+      __PYX_ERR(0, 163, __pyx_L1_error)
     }
-    __pyx_t_5 = __Pyx_PyDict_GetItem(__pyx_v_lines, __pyx_v_var_name); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 161, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyDict_GetItem(__pyx_v_lines, __pyx_v_var_name); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 163, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_7 = __Pyx_PyObject_Dict_GetItem(__pyx_t_5, __pyx_v_mode); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 161, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_Dict_GetItem(__pyx_t_5, __pyx_v_mode); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 163, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_5 = __Pyx_PyObject_Dict_GetItem(__pyx_t_7, __pyx_n_u_yDataDown); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 161, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_Dict_GetItem(__pyx_t_7, __pyx_n_u_yDataDown); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 163, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_t_7 = PyFloat_FromDouble(__pyx_v_pnt.stdev); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 161, __pyx_L1_error)
+    __pyx_t_7 = PyFloat_FromDouble(__pyx_v_pnt.stdev); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 163, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_8 = __Pyx_PyObject_Append(__pyx_t_5, __pyx_t_7); if (unlikely(__pyx_t_8 == ((int)-1))) __PYX_ERR(0, 161, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_Append(__pyx_t_5, __pyx_t_7); if (unlikely(__pyx_t_8 == ((int)-1))) __PYX_ERR(0, 163, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":162
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":164
  *             lines[var_name][mode] = {"yDataDown" : [], "yDataUp" : [], "xData" : [], "yData" : [], "Title" : mode}
  *         lines[var_name][mode]["yDataDown"].append(pnt.stdev)
  *         lines[var_name][mode]["yDataUp"].append(pnt.stdev)             # <<<<<<<<<<<<<<
  *         lines[var_name][mode]["yData"].append(pnt.average)
  *         lines[var_name][mode]["xData"].append(epoch)
  */
     if (unlikely(__pyx_v_lines == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 162, __pyx_L1_error)
+      __PYX_ERR(0, 164, __pyx_L1_error)
     }
-    __pyx_t_7 = __Pyx_PyDict_GetItem(__pyx_v_lines, __pyx_v_var_name); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 162, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyDict_GetItem(__pyx_v_lines, __pyx_v_var_name); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 164, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_5 = __Pyx_PyObject_Dict_GetItem(__pyx_t_7, __pyx_v_mode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 162, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_Dict_GetItem(__pyx_t_7, __pyx_v_mode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 164, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_t_7 = __Pyx_PyObject_Dict_GetItem(__pyx_t_5, __pyx_n_u_yDataUp); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 162, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_Dict_GetItem(__pyx_t_5, __pyx_n_u_yDataUp); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 164, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_5 = PyFloat_FromDouble(__pyx_v_pnt.stdev); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 162, __pyx_L1_error)
+    __pyx_t_5 = PyFloat_FromDouble(__pyx_v_pnt.stdev); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 164, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_8 = __Pyx_PyObject_Append(__pyx_t_7, __pyx_t_5); if (unlikely(__pyx_t_8 == ((int)-1))) __PYX_ERR(0, 162, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_Append(__pyx_t_7, __pyx_t_5); if (unlikely(__pyx_t_8 == ((int)-1))) __PYX_ERR(0, 164, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":163
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":165
  *         lines[var_name][mode]["yDataDown"].append(pnt.stdev)
  *         lines[var_name][mode]["yDataUp"].append(pnt.stdev)
  *         lines[var_name][mode]["yData"].append(pnt.average)             # <<<<<<<<<<<<<<
  *         lines[var_name][mode]["xData"].append(epoch)
  *         if   metric == "auc" and mode == "training"  : state.auc_train[itv.first] = pnt.average
  */
     if (unlikely(__pyx_v_lines == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 163, __pyx_L1_error)
+      __PYX_ERR(0, 165, __pyx_L1_error)
     }
-    __pyx_t_5 = __Pyx_PyDict_GetItem(__pyx_v_lines, __pyx_v_var_name); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 163, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyDict_GetItem(__pyx_v_lines, __pyx_v_var_name); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 165, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_7 = __Pyx_PyObject_Dict_GetItem(__pyx_t_5, __pyx_v_mode); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 163, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_Dict_GetItem(__pyx_t_5, __pyx_v_mode); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 165, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_5 = __Pyx_PyObject_Dict_GetItem(__pyx_t_7, __pyx_n_u_yData); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 163, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_Dict_GetItem(__pyx_t_7, __pyx_n_u_yData); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 165, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_t_7 = PyFloat_FromDouble(__pyx_v_pnt.average); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 163, __pyx_L1_error)
+    __pyx_t_7 = PyFloat_FromDouble(__pyx_v_pnt.average); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 165, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_8 = __Pyx_PyObject_Append(__pyx_t_5, __pyx_t_7); if (unlikely(__pyx_t_8 == ((int)-1))) __PYX_ERR(0, 163, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_Append(__pyx_t_5, __pyx_t_7); if (unlikely(__pyx_t_8 == ((int)-1))) __PYX_ERR(0, 165, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":164
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":166
  *         lines[var_name][mode]["yDataUp"].append(pnt.stdev)
  *         lines[var_name][mode]["yData"].append(pnt.average)
  *         lines[var_name][mode]["xData"].append(epoch)             # <<<<<<<<<<<<<<
  *         if   metric == "auc" and mode == "training"  : state.auc_train[itv.first] = pnt.average
  *         elif metric == "auc" and mode == "validation": state.auc_valid[itv.first] = pnt.average
  */
     if (unlikely(__pyx_v_lines == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 164, __pyx_L1_error)
+      __PYX_ERR(0, 166, __pyx_L1_error)
     }
-    __pyx_t_7 = __Pyx_PyDict_GetItem(__pyx_v_lines, __pyx_v_var_name); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 164, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyDict_GetItem(__pyx_v_lines, __pyx_v_var_name); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 166, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_5 = __Pyx_PyObject_Dict_GetItem(__pyx_t_7, __pyx_v_mode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 164, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_Dict_GetItem(__pyx_t_7, __pyx_v_mode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 166, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_t_7 = __Pyx_PyObject_Dict_GetItem(__pyx_t_5, __pyx_n_u_xData); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 164, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_Dict_GetItem(__pyx_t_5, __pyx_n_u_xData); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 166, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_epoch); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 164, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_epoch); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 166, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_8 = __Pyx_PyObject_Append(__pyx_t_7, __pyx_t_5); if (unlikely(__pyx_t_8 == ((int)-1))) __PYX_ERR(0, 164, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_Append(__pyx_t_7, __pyx_t_5); if (unlikely(__pyx_t_8 == ((int)-1))) __PYX_ERR(0, 166, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":165
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":167
  *         lines[var_name][mode]["yData"].append(pnt.average)
  *         lines[var_name][mode]["xData"].append(epoch)
  *         if   metric == "auc" and mode == "training"  : state.auc_train[itv.first] = pnt.average             # <<<<<<<<<<<<<<
  *         elif metric == "auc" and mode == "validation": state.auc_valid[itv.first] = pnt.average
  *         elif metric == "auc" and mode == "evaluation": state.auc_eval[itv.first] = pnt.average
  */
-    __pyx_t_9 = (__Pyx_PyUnicode_Equals(__pyx_v_metric, __pyx_n_u_auc, Py_EQ)); if (unlikely((__pyx_t_9 < 0))) __PYX_ERR(0, 165, __pyx_L1_error)
+    __pyx_t_9 = (__Pyx_PyUnicode_Equals(__pyx_v_metric, __pyx_n_u_auc, Py_EQ)); if (unlikely((__pyx_t_9 < 0))) __PYX_ERR(0, 167, __pyx_L1_error)
     if (__pyx_t_9) {
     } else {
       __pyx_t_6 = __pyx_t_9;
       goto __pyx_L8_bool_binop_done;
     }
-    __pyx_t_9 = (__Pyx_PyUnicode_Equals(__pyx_v_mode, __pyx_n_u_training, Py_EQ)); if (unlikely((__pyx_t_9 < 0))) __PYX_ERR(0, 165, __pyx_L1_error)
+    __pyx_t_9 = (__Pyx_PyUnicode_Equals(__pyx_v_mode, __pyx_n_u_training, Py_EQ)); if (unlikely((__pyx_t_9 < 0))) __PYX_ERR(0, 167, __pyx_L1_error)
     __pyx_t_6 = __pyx_t_9;
     __pyx_L8_bool_binop_done:;
     if (__pyx_t_6) {
       __pyx_t_10 = __pyx_v_pnt.average;
       (__pyx_v_state->auc_train[__pyx_v_itv.first]) = __pyx_t_10;
       goto __pyx_L7;
     }
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":166
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":168
  *         lines[var_name][mode]["xData"].append(epoch)
  *         if   metric == "auc" and mode == "training"  : state.auc_train[itv.first] = pnt.average
  *         elif metric == "auc" and mode == "validation": state.auc_valid[itv.first] = pnt.average             # <<<<<<<<<<<<<<
  *         elif metric == "auc" and mode == "evaluation": state.auc_eval[itv.first] = pnt.average
  * 
  */
-    __pyx_t_9 = (__Pyx_PyUnicode_Equals(__pyx_v_metric, __pyx_n_u_auc, Py_EQ)); if (unlikely((__pyx_t_9 < 0))) __PYX_ERR(0, 166, __pyx_L1_error)
+    __pyx_t_9 = (__Pyx_PyUnicode_Equals(__pyx_v_metric, __pyx_n_u_auc, Py_EQ)); if (unlikely((__pyx_t_9 < 0))) __PYX_ERR(0, 168, __pyx_L1_error)
     if (__pyx_t_9) {
     } else {
       __pyx_t_6 = __pyx_t_9;
       goto __pyx_L10_bool_binop_done;
     }
-    __pyx_t_9 = (__Pyx_PyUnicode_Equals(__pyx_v_mode, __pyx_n_u_validation, Py_EQ)); if (unlikely((__pyx_t_9 < 0))) __PYX_ERR(0, 166, __pyx_L1_error)
+    __pyx_t_9 = (__Pyx_PyUnicode_Equals(__pyx_v_mode, __pyx_n_u_validation, Py_EQ)); if (unlikely((__pyx_t_9 < 0))) __PYX_ERR(0, 168, __pyx_L1_error)
     __pyx_t_6 = __pyx_t_9;
     __pyx_L10_bool_binop_done:;
     if (__pyx_t_6) {
       __pyx_t_10 = __pyx_v_pnt.average;
       (__pyx_v_state->auc_valid[__pyx_v_itv.first]) = __pyx_t_10;
       goto __pyx_L7;
     }
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":167
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":169
  *         if   metric == "auc" and mode == "training"  : state.auc_train[itv.first] = pnt.average
  *         elif metric == "auc" and mode == "validation": state.auc_valid[itv.first] = pnt.average
  *         elif metric == "auc" and mode == "evaluation": state.auc_eval[itv.first] = pnt.average             # <<<<<<<<<<<<<<
  * 
  *         elif metric == "acc" and mode == "training"  :
  */
-    __pyx_t_9 = (__Pyx_PyUnicode_Equals(__pyx_v_metric, __pyx_n_u_auc, Py_EQ)); if (unlikely((__pyx_t_9 < 0))) __PYX_ERR(0, 167, __pyx_L1_error)
+    __pyx_t_9 = (__Pyx_PyUnicode_Equals(__pyx_v_metric, __pyx_n_u_auc, Py_EQ)); if (unlikely((__pyx_t_9 < 0))) __PYX_ERR(0, 169, __pyx_L1_error)
     if (__pyx_t_9) {
     } else {
       __pyx_t_6 = __pyx_t_9;
       goto __pyx_L12_bool_binop_done;
     }
-    __pyx_t_9 = (__Pyx_PyUnicode_Equals(__pyx_v_mode, __pyx_n_u_evaluation, Py_EQ)); if (unlikely((__pyx_t_9 < 0))) __PYX_ERR(0, 167, __pyx_L1_error)
+    __pyx_t_9 = (__Pyx_PyUnicode_Equals(__pyx_v_mode, __pyx_n_u_evaluation, Py_EQ)); if (unlikely((__pyx_t_9 < 0))) __PYX_ERR(0, 169, __pyx_L1_error)
     __pyx_t_6 = __pyx_t_9;
     __pyx_L12_bool_binop_done:;
     if (__pyx_t_6) {
       __pyx_t_10 = __pyx_v_pnt.average;
       (__pyx_v_state->auc_eval[__pyx_v_itv.first]) = __pyx_t_10;
       goto __pyx_L7;
     }
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":169
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":171
  *         elif metric == "auc" and mode == "evaluation": state.auc_eval[itv.first] = pnt.average
  * 
  *         elif metric == "acc" and mode == "training"  :             # <<<<<<<<<<<<<<
  *             state.acc_train[itv.first]      = pnt.average
  *             state.acc_train_up[itv.first]   = pnt.maximum
  */
-    __pyx_t_9 = (__Pyx_PyUnicode_Equals(__pyx_v_metric, __pyx_n_u_acc, Py_EQ)); if (unlikely((__pyx_t_9 < 0))) __PYX_ERR(0, 169, __pyx_L1_error)
+    __pyx_t_9 = (__Pyx_PyUnicode_Equals(__pyx_v_metric, __pyx_n_u_acc, Py_EQ)); if (unlikely((__pyx_t_9 < 0))) __PYX_ERR(0, 171, __pyx_L1_error)
     if (__pyx_t_9) {
     } else {
       __pyx_t_6 = __pyx_t_9;
       goto __pyx_L14_bool_binop_done;
     }
-    __pyx_t_9 = (__Pyx_PyUnicode_Equals(__pyx_v_mode, __pyx_n_u_training, Py_EQ)); if (unlikely((__pyx_t_9 < 0))) __PYX_ERR(0, 169, __pyx_L1_error)
+    __pyx_t_9 = (__Pyx_PyUnicode_Equals(__pyx_v_mode, __pyx_n_u_training, Py_EQ)); if (unlikely((__pyx_t_9 < 0))) __PYX_ERR(0, 171, __pyx_L1_error)
     __pyx_t_6 = __pyx_t_9;
     __pyx_L14_bool_binop_done:;
     if (__pyx_t_6) {
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":170
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":172
  * 
  *         elif metric == "acc" and mode == "training"  :
  *             state.acc_train[itv.first]      = pnt.average             # <<<<<<<<<<<<<<
  *             state.acc_train_up[itv.first]   = pnt.maximum
  *             state.acc_train_down[itv.first] = pnt.minimum
  */
       __pyx_t_10 = __pyx_v_pnt.average;
       (__pyx_v_state->acc_train[__pyx_v_itv.first]) = __pyx_t_10;
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":171
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":173
  *         elif metric == "acc" and mode == "training"  :
  *             state.acc_train[itv.first]      = pnt.average
  *             state.acc_train_up[itv.first]   = pnt.maximum             # <<<<<<<<<<<<<<
  *             state.acc_train_down[itv.first] = pnt.minimum
  * 
  */
       __pyx_t_10 = __pyx_v_pnt.maximum;
       (__pyx_v_state->acc_train_up[__pyx_v_itv.first]) = __pyx_t_10;
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":172
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":174
  *             state.acc_train[itv.first]      = pnt.average
  *             state.acc_train_up[itv.first]   = pnt.maximum
  *             state.acc_train_down[itv.first] = pnt.minimum             # <<<<<<<<<<<<<<
  * 
  *         elif metric == "acc" and mode == "validation":
  */
       __pyx_t_10 = __pyx_v_pnt.minimum;
       (__pyx_v_state->acc_train_down[__pyx_v_itv.first]) = __pyx_t_10;
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":169
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":171
  *         elif metric == "auc" and mode == "evaluation": state.auc_eval[itv.first] = pnt.average
  * 
  *         elif metric == "acc" and mode == "training"  :             # <<<<<<<<<<<<<<
  *             state.acc_train[itv.first]      = pnt.average
  *             state.acc_train_up[itv.first]   = pnt.maximum
  */
       goto __pyx_L7;
     }
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":174
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":176
  *             state.acc_train_down[itv.first] = pnt.minimum
  * 
  *         elif metric == "acc" and mode == "validation":             # <<<<<<<<<<<<<<
  *             state.acc_valid[itv.first]      = pnt.average
  *             state.acc_valid_up[itv.first]   = pnt.maximum
  */
-    __pyx_t_9 = (__Pyx_PyUnicode_Equals(__pyx_v_metric, __pyx_n_u_acc, Py_EQ)); if (unlikely((__pyx_t_9 < 0))) __PYX_ERR(0, 174, __pyx_L1_error)
+    __pyx_t_9 = (__Pyx_PyUnicode_Equals(__pyx_v_metric, __pyx_n_u_acc, Py_EQ)); if (unlikely((__pyx_t_9 < 0))) __PYX_ERR(0, 176, __pyx_L1_error)
     if (__pyx_t_9) {
     } else {
       __pyx_t_6 = __pyx_t_9;
       goto __pyx_L16_bool_binop_done;
     }
-    __pyx_t_9 = (__Pyx_PyUnicode_Equals(__pyx_v_mode, __pyx_n_u_validation, Py_EQ)); if (unlikely((__pyx_t_9 < 0))) __PYX_ERR(0, 174, __pyx_L1_error)
+    __pyx_t_9 = (__Pyx_PyUnicode_Equals(__pyx_v_mode, __pyx_n_u_validation, Py_EQ)); if (unlikely((__pyx_t_9 < 0))) __PYX_ERR(0, 176, __pyx_L1_error)
     __pyx_t_6 = __pyx_t_9;
     __pyx_L16_bool_binop_done:;
     if (__pyx_t_6) {
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":175
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":177
  * 
  *         elif metric == "acc" and mode == "validation":
  *             state.acc_valid[itv.first]      = pnt.average             # <<<<<<<<<<<<<<
  *             state.acc_valid_up[itv.first]   = pnt.maximum
  *             state.acc_valid_down[itv.first] = pnt.minimum
  */
       __pyx_t_10 = __pyx_v_pnt.average;
       (__pyx_v_state->acc_valid[__pyx_v_itv.first]) = __pyx_t_10;
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":176
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":178
  *         elif metric == "acc" and mode == "validation":
  *             state.acc_valid[itv.first]      = pnt.average
  *             state.acc_valid_up[itv.first]   = pnt.maximum             # <<<<<<<<<<<<<<
  *             state.acc_valid_down[itv.first] = pnt.minimum
  * 
  */
       __pyx_t_10 = __pyx_v_pnt.maximum;
       (__pyx_v_state->acc_valid_up[__pyx_v_itv.first]) = __pyx_t_10;
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":177
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":179
  *             state.acc_valid[itv.first]      = pnt.average
  *             state.acc_valid_up[itv.first]   = pnt.maximum
  *             state.acc_valid_down[itv.first] = pnt.minimum             # <<<<<<<<<<<<<<
  * 
  *         elif metric == "acc" and mode == "evaluation":
  */
       __pyx_t_10 = __pyx_v_pnt.minimum;
       (__pyx_v_state->acc_valid_down[__pyx_v_itv.first]) = __pyx_t_10;
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":174
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":176
  *             state.acc_train_down[itv.first] = pnt.minimum
  * 
  *         elif metric == "acc" and mode == "validation":             # <<<<<<<<<<<<<<
  *             state.acc_valid[itv.first]      = pnt.average
  *             state.acc_valid_up[itv.first]   = pnt.maximum
  */
       goto __pyx_L7;
     }
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":179
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":181
  *             state.acc_valid_down[itv.first] = pnt.minimum
  * 
  *         elif metric == "acc" and mode == "evaluation":             # <<<<<<<<<<<<<<
  *             state.acc_eval[itv.first]      = pnt.average
  *             state.acc_eval_up[itv.first]   = pnt.maximum
  */
-    __pyx_t_9 = (__Pyx_PyUnicode_Equals(__pyx_v_metric, __pyx_n_u_acc, Py_EQ)); if (unlikely((__pyx_t_9 < 0))) __PYX_ERR(0, 179, __pyx_L1_error)
+    __pyx_t_9 = (__Pyx_PyUnicode_Equals(__pyx_v_metric, __pyx_n_u_acc, Py_EQ)); if (unlikely((__pyx_t_9 < 0))) __PYX_ERR(0, 181, __pyx_L1_error)
     if (__pyx_t_9) {
     } else {
       __pyx_t_6 = __pyx_t_9;
       goto __pyx_L18_bool_binop_done;
     }
-    __pyx_t_9 = (__Pyx_PyUnicode_Equals(__pyx_v_mode, __pyx_n_u_evaluation, Py_EQ)); if (unlikely((__pyx_t_9 < 0))) __PYX_ERR(0, 179, __pyx_L1_error)
+    __pyx_t_9 = (__Pyx_PyUnicode_Equals(__pyx_v_mode, __pyx_n_u_evaluation, Py_EQ)); if (unlikely((__pyx_t_9 < 0))) __PYX_ERR(0, 181, __pyx_L1_error)
     __pyx_t_6 = __pyx_t_9;
     __pyx_L18_bool_binop_done:;
     if (__pyx_t_6) {
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":180
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":182
  * 
  *         elif metric == "acc" and mode == "evaluation":
  *             state.acc_eval[itv.first]      = pnt.average             # <<<<<<<<<<<<<<
  *             state.acc_eval_up[itv.first]   = pnt.maximum
  *             state.acc_eval_down[itv.first] = pnt.minimum
  */
       __pyx_t_10 = __pyx_v_pnt.average;
       (__pyx_v_state->acc_eval[__pyx_v_itv.first]) = __pyx_t_10;
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":181
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":183
  *         elif metric == "acc" and mode == "evaluation":
  *             state.acc_eval[itv.first]      = pnt.average
  *             state.acc_eval_up[itv.first]   = pnt.maximum             # <<<<<<<<<<<<<<
  *             state.acc_eval_down[itv.first] = pnt.minimum
  * 
  */
       __pyx_t_10 = __pyx_v_pnt.maximum;
       (__pyx_v_state->acc_eval_up[__pyx_v_itv.first]) = __pyx_t_10;
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":182
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":184
  *             state.acc_eval[itv.first]      = pnt.average
  *             state.acc_eval_up[itv.first]   = pnt.maximum
  *             state.acc_eval_down[itv.first] = pnt.minimum             # <<<<<<<<<<<<<<
  * 
  *         elif metric == "lss" and mode == "training":
  */
       __pyx_t_10 = __pyx_v_pnt.minimum;
       (__pyx_v_state->acc_eval_down[__pyx_v_itv.first]) = __pyx_t_10;
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":179
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":181
  *             state.acc_valid_down[itv.first] = pnt.minimum
  * 
  *         elif metric == "acc" and mode == "evaluation":             # <<<<<<<<<<<<<<
  *             state.acc_eval[itv.first]      = pnt.average
  *             state.acc_eval_up[itv.first]   = pnt.maximum
  */
       goto __pyx_L7;
     }
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":184
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":186
  *             state.acc_eval_down[itv.first] = pnt.minimum
  * 
  *         elif metric == "lss" and mode == "training":             # <<<<<<<<<<<<<<
  *             state.loss_train[itv.first]      = pnt.average
  *             state.loss_train_up[itv.first]   = pnt.maximum
  */
-    __pyx_t_9 = (__Pyx_PyUnicode_Equals(__pyx_v_metric, __pyx_n_u_lss, Py_EQ)); if (unlikely((__pyx_t_9 < 0))) __PYX_ERR(0, 184, __pyx_L1_error)
+    __pyx_t_9 = (__Pyx_PyUnicode_Equals(__pyx_v_metric, __pyx_n_u_lss, Py_EQ)); if (unlikely((__pyx_t_9 < 0))) __PYX_ERR(0, 186, __pyx_L1_error)
     if (__pyx_t_9) {
     } else {
       __pyx_t_6 = __pyx_t_9;
       goto __pyx_L20_bool_binop_done;
     }
-    __pyx_t_9 = (__Pyx_PyUnicode_Equals(__pyx_v_mode, __pyx_n_u_training, Py_EQ)); if (unlikely((__pyx_t_9 < 0))) __PYX_ERR(0, 184, __pyx_L1_error)
+    __pyx_t_9 = (__Pyx_PyUnicode_Equals(__pyx_v_mode, __pyx_n_u_training, Py_EQ)); if (unlikely((__pyx_t_9 < 0))) __PYX_ERR(0, 186, __pyx_L1_error)
     __pyx_t_6 = __pyx_t_9;
     __pyx_L20_bool_binop_done:;
     if (__pyx_t_6) {
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":185
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":187
  * 
  *         elif metric == "lss" and mode == "training":
  *             state.loss_train[itv.first]      = pnt.average             # <<<<<<<<<<<<<<
  *             state.loss_train_up[itv.first]   = pnt.maximum
  *             state.loss_train_down[itv.first] = pnt.minimum
  */
       __pyx_t_10 = __pyx_v_pnt.average;
       (__pyx_v_state->loss_train[__pyx_v_itv.first]) = __pyx_t_10;
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":186
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":188
  *         elif metric == "lss" and mode == "training":
  *             state.loss_train[itv.first]      = pnt.average
  *             state.loss_train_up[itv.first]   = pnt.maximum             # <<<<<<<<<<<<<<
  *             state.loss_train_down[itv.first] = pnt.minimum
  * 
  */
       __pyx_t_10 = __pyx_v_pnt.maximum;
       (__pyx_v_state->loss_train_up[__pyx_v_itv.first]) = __pyx_t_10;
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":187
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":189
  *             state.loss_train[itv.first]      = pnt.average
  *             state.loss_train_up[itv.first]   = pnt.maximum
  *             state.loss_train_down[itv.first] = pnt.minimum             # <<<<<<<<<<<<<<
  * 
  *         elif metric == "lss" and mode == "validation":
  */
       __pyx_t_10 = __pyx_v_pnt.minimum;
       (__pyx_v_state->loss_train_down[__pyx_v_itv.first]) = __pyx_t_10;
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":184
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":186
  *             state.acc_eval_down[itv.first] = pnt.minimum
  * 
  *         elif metric == "lss" and mode == "training":             # <<<<<<<<<<<<<<
  *             state.loss_train[itv.first]      = pnt.average
  *             state.loss_train_up[itv.first]   = pnt.maximum
  */
       goto __pyx_L7;
     }
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":189
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":191
  *             state.loss_train_down[itv.first] = pnt.minimum
  * 
  *         elif metric == "lss" and mode == "validation":             # <<<<<<<<<<<<<<
  *             state.loss_valid[itv.first]      = pnt.average
  *             state.loss_valid_up[itv.first]   = pnt.maximum
  */
-    __pyx_t_9 = (__Pyx_PyUnicode_Equals(__pyx_v_metric, __pyx_n_u_lss, Py_EQ)); if (unlikely((__pyx_t_9 < 0))) __PYX_ERR(0, 189, __pyx_L1_error)
+    __pyx_t_9 = (__Pyx_PyUnicode_Equals(__pyx_v_metric, __pyx_n_u_lss, Py_EQ)); if (unlikely((__pyx_t_9 < 0))) __PYX_ERR(0, 191, __pyx_L1_error)
     if (__pyx_t_9) {
     } else {
       __pyx_t_6 = __pyx_t_9;
       goto __pyx_L22_bool_binop_done;
     }
-    __pyx_t_9 = (__Pyx_PyUnicode_Equals(__pyx_v_mode, __pyx_n_u_validation, Py_EQ)); if (unlikely((__pyx_t_9 < 0))) __PYX_ERR(0, 189, __pyx_L1_error)
+    __pyx_t_9 = (__Pyx_PyUnicode_Equals(__pyx_v_mode, __pyx_n_u_validation, Py_EQ)); if (unlikely((__pyx_t_9 < 0))) __PYX_ERR(0, 191, __pyx_L1_error)
     __pyx_t_6 = __pyx_t_9;
     __pyx_L22_bool_binop_done:;
     if (__pyx_t_6) {
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":190
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":192
  * 
  *         elif metric == "lss" and mode == "validation":
  *             state.loss_valid[itv.first]      = pnt.average             # <<<<<<<<<<<<<<
  *             state.loss_valid_up[itv.first]   = pnt.maximum
  *             state.loss_valid_down[itv.first] = pnt.minimum
  */
       __pyx_t_10 = __pyx_v_pnt.average;
       (__pyx_v_state->loss_valid[__pyx_v_itv.first]) = __pyx_t_10;
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":191
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":193
  *         elif metric == "lss" and mode == "validation":
  *             state.loss_valid[itv.first]      = pnt.average
  *             state.loss_valid_up[itv.first]   = pnt.maximum             # <<<<<<<<<<<<<<
  *             state.loss_valid_down[itv.first] = pnt.minimum
  * 
  */
       __pyx_t_10 = __pyx_v_pnt.maximum;
       (__pyx_v_state->loss_valid_up[__pyx_v_itv.first]) = __pyx_t_10;
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":192
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":194
  *             state.loss_valid[itv.first]      = pnt.average
  *             state.loss_valid_up[itv.first]   = pnt.maximum
  *             state.loss_valid_down[itv.first] = pnt.minimum             # <<<<<<<<<<<<<<
  * 
  *         elif metric == "lss" and mode == "evaluation":
  */
       __pyx_t_10 = __pyx_v_pnt.minimum;
       (__pyx_v_state->loss_valid_down[__pyx_v_itv.first]) = __pyx_t_10;
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":189
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":191
  *             state.loss_train_down[itv.first] = pnt.minimum
  * 
  *         elif metric == "lss" and mode == "validation":             # <<<<<<<<<<<<<<
  *             state.loss_valid[itv.first]      = pnt.average
  *             state.loss_valid_up[itv.first]   = pnt.maximum
  */
       goto __pyx_L7;
     }
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":194
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":196
  *             state.loss_valid_down[itv.first] = pnt.minimum
  * 
  *         elif metric == "lss" and mode == "evaluation":             # <<<<<<<<<<<<<<
  *             state.loss_eval[itv.first]      = pnt.average
  *             state.loss_eval_up[itv.first]   = pnt.maximum
  */
-    __pyx_t_9 = (__Pyx_PyUnicode_Equals(__pyx_v_metric, __pyx_n_u_lss, Py_EQ)); if (unlikely((__pyx_t_9 < 0))) __PYX_ERR(0, 194, __pyx_L1_error)
+    __pyx_t_9 = (__Pyx_PyUnicode_Equals(__pyx_v_metric, __pyx_n_u_lss, Py_EQ)); if (unlikely((__pyx_t_9 < 0))) __PYX_ERR(0, 196, __pyx_L1_error)
     if (__pyx_t_9) {
     } else {
       __pyx_t_6 = __pyx_t_9;
       goto __pyx_L24_bool_binop_done;
     }
-    __pyx_t_9 = (__Pyx_PyUnicode_Equals(__pyx_v_mode, __pyx_n_u_evaluation, Py_EQ)); if (unlikely((__pyx_t_9 < 0))) __PYX_ERR(0, 194, __pyx_L1_error)
+    __pyx_t_9 = (__Pyx_PyUnicode_Equals(__pyx_v_mode, __pyx_n_u_evaluation, Py_EQ)); if (unlikely((__pyx_t_9 < 0))) __PYX_ERR(0, 196, __pyx_L1_error)
     __pyx_t_6 = __pyx_t_9;
     __pyx_L24_bool_binop_done:;
     if (__pyx_t_6) {
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":195
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":197
  * 
  *         elif metric == "lss" and mode == "evaluation":
  *             state.loss_eval[itv.first]      = pnt.average             # <<<<<<<<<<<<<<
  *             state.loss_eval_up[itv.first]   = pnt.maximum
  *             state.loss_eval_down[itv.first] = pnt.minimum
  */
       __pyx_t_10 = __pyx_v_pnt.average;
       (__pyx_v_state->loss_eval[__pyx_v_itv.first]) = __pyx_t_10;
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":196
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":198
  *         elif metric == "lss" and mode == "evaluation":
  *             state.loss_eval[itv.first]      = pnt.average
  *             state.loss_eval_up[itv.first]   = pnt.maximum             # <<<<<<<<<<<<<<
  *             state.loss_eval_down[itv.first] = pnt.minimum
  *     return lines
  */
       __pyx_t_10 = __pyx_v_pnt.maximum;
       (__pyx_v_state->loss_eval_up[__pyx_v_itv.first]) = __pyx_t_10;
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":197
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":199
  *             state.loss_eval[itv.first]      = pnt.average
  *             state.loss_eval_up[itv.first]   = pnt.maximum
  *             state.loss_eval_down[itv.first] = pnt.minimum             # <<<<<<<<<<<<<<
  *     return lines
  * 
  */
       __pyx_t_10 = __pyx_v_pnt.minimum;
       (__pyx_v_state->loss_eval_down[__pyx_v_itv.first]) = __pyx_t_10;
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":194
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":196
  *             state.loss_valid_down[itv.first] = pnt.minimum
  * 
  *         elif metric == "lss" and mode == "evaluation":             # <<<<<<<<<<<<<<
  *             state.loss_eval[itv.first]      = pnt.average
  *             state.loss_eval_up[itv.first]   = pnt.maximum
  */
     }
     __pyx_L7:;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":154
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":156
  *     cdef str var_name
  * 
  *     for itv in dereference(tmp):             # <<<<<<<<<<<<<<
  *         pnt = point_t()
  *         stats(&itv.second, &pnt)
  */
   }
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":198
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":200
  *             state.loss_eval_up[itv.first]   = pnt.maximum
  *             state.loss_eval_down[itv.first] = pnt.minimum
  *     return lines             # <<<<<<<<<<<<<<
  * 
  * cdef void make_accuracy_plots(map[int, CyEpoch*] train, map[int, CyEpoch*] valid, map[int, CyEpoch*] test, str path, report_t* state):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_lines);
   __pyx_r = __pyx_v_lines;
   goto __pyx_L0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":149
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":151
  *             del th
  * 
  * cdef dict collapse_points(map[string, vector[point_t]]* tmp, int epoch, dict lines, str mode, report_t* state, str metric):             # <<<<<<<<<<<<<<
  *     cdef pair[string, vector[point_t]]itv
  *     cdef point_t pnt
  */
 
@@ -29217,15 +29210,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_var_name);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/cmodules/cyincludes/cyoptimizer.pyx":200
+/* "src/cmodules/cyincludes/cyoptimizer.pyx":202
  *     return lines
  * 
  * cdef void make_accuracy_plots(map[int, CyEpoch*] train, map[int, CyEpoch*] valid, map[int, CyEpoch*] test, str path, report_t* state):             # <<<<<<<<<<<<<<
  *     cdef pair[int, CyEpoch*] itr
  *     cdef pair[string, point_t] its
  */
 
@@ -29266,306 +29259,306 @@
   PyObject *__pyx_t_19 = NULL;
   PyObject *__pyx_t_20 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("make_accuracy_plots", 1);
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":209
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":211
  *     cdef map[string, vector[point_t]] tmp_te
  * 
  *     cdef list folds = []             # <<<<<<<<<<<<<<
  *     cdef list epochs = []
  *     cdef int epoch, kf
  */
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 209, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 211, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_folds = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":210
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":212
  * 
  *     cdef list folds = []
  *     cdef list epochs = []             # <<<<<<<<<<<<<<
  *     cdef int epoch, kf
  * 
  */
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 210, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 212, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_epochs = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":213
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":215
  *     cdef int epoch, kf
  * 
  *     for itr in train:             # <<<<<<<<<<<<<<
  *         folds += list(train[itr.first].accuracy)
  *         epochs += [itr.first]
  */
   __pyx_t_2 = __pyx_v_train.begin();
   for (;;) {
     if (!(__pyx_t_2 != __pyx_v_train.end())) break;
     __pyx_t_3 = *__pyx_t_2;
     ++__pyx_t_2;
     __pyx_v_itr = __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_3);
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":214
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":216
  * 
  *     for itr in train:
  *         folds += list(train[itr.first].accuracy)             # <<<<<<<<<<<<<<
  *         epochs += [itr.first]
  * 
  */
-    __pyx_t_1 = __pyx_convert_map_to_py_int____std_3a__3a_map_3c_std_3a__3a_string_2c_struct__point_t_3e___((__pyx_v_train[__pyx_v_itr.first])->accuracy); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 214, __pyx_L1_error)
+    __pyx_t_1 = __pyx_convert_map_to_py_int____std_3a__3a_map_3c_std_3a__3a_string_2c_struct__point_t_3e___((__pyx_v_train[__pyx_v_itr.first])->accuracy); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 216, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_4 = __Pyx_PySequence_ListKeepNew(__pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 214, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PySequence_ListKeepNew(__pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 216, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = PyNumber_InPlaceAdd(__pyx_v_folds, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 214, __pyx_L1_error)
+    __pyx_t_1 = PyNumber_InPlaceAdd(__pyx_v_folds, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 216, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF_SET(__pyx_v_folds, ((PyObject*)__pyx_t_1));
     __pyx_t_1 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":215
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":217
  *     for itr in train:
  *         folds += list(train[itr.first].accuracy)
  *         epochs += [itr.first]             # <<<<<<<<<<<<<<
  * 
  *     for itr in valid:
  */
-    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_itr.first); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 215, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_itr.first); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 217, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_4 = PyList_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 215, __pyx_L1_error)
+    __pyx_t_4 = PyList_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 217, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_1);
-    if (__Pyx_PyList_SET_ITEM(__pyx_t_4, 0, __pyx_t_1)) __PYX_ERR(0, 215, __pyx_L1_error);
+    if (__Pyx_PyList_SET_ITEM(__pyx_t_4, 0, __pyx_t_1)) __PYX_ERR(0, 217, __pyx_L1_error);
     __pyx_t_1 = 0;
-    __pyx_t_1 = PyNumber_InPlaceAdd(__pyx_v_epochs, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 215, __pyx_L1_error)
+    __pyx_t_1 = PyNumber_InPlaceAdd(__pyx_v_epochs, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 217, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF_SET(__pyx_v_epochs, ((PyObject*)__pyx_t_1));
     __pyx_t_1 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":213
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":215
  *     cdef int epoch, kf
  * 
  *     for itr in train:             # <<<<<<<<<<<<<<
  *         folds += list(train[itr.first].accuracy)
  *         epochs += [itr.first]
  */
   }
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":217
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":219
  *         epochs += [itr.first]
  * 
  *     for itr in valid:             # <<<<<<<<<<<<<<
  *         folds += list(valid[itr.first].accuracy)
  *         epochs += [itr.first]
  */
   __pyx_t_2 = __pyx_v_valid.begin();
   for (;;) {
     if (!(__pyx_t_2 != __pyx_v_valid.end())) break;
     __pyx_t_3 = *__pyx_t_2;
     ++__pyx_t_2;
     __pyx_v_itr = __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_3);
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":218
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":220
  * 
  *     for itr in valid:
  *         folds += list(valid[itr.first].accuracy)             # <<<<<<<<<<<<<<
  *         epochs += [itr.first]
  * 
  */
-    __pyx_t_1 = __pyx_convert_map_to_py_int____std_3a__3a_map_3c_std_3a__3a_string_2c_struct__point_t_3e___((__pyx_v_valid[__pyx_v_itr.first])->accuracy); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 218, __pyx_L1_error)
+    __pyx_t_1 = __pyx_convert_map_to_py_int____std_3a__3a_map_3c_std_3a__3a_string_2c_struct__point_t_3e___((__pyx_v_valid[__pyx_v_itr.first])->accuracy); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 220, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_4 = __Pyx_PySequence_ListKeepNew(__pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 218, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PySequence_ListKeepNew(__pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 220, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = PyNumber_InPlaceAdd(__pyx_v_folds, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 218, __pyx_L1_error)
+    __pyx_t_1 = PyNumber_InPlaceAdd(__pyx_v_folds, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 220, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF_SET(__pyx_v_folds, ((PyObject*)__pyx_t_1));
     __pyx_t_1 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":219
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":221
  *     for itr in valid:
  *         folds += list(valid[itr.first].accuracy)
  *         epochs += [itr.first]             # <<<<<<<<<<<<<<
  * 
  *     for itr in test:
  */
-    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_itr.first); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 219, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_itr.first); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 221, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_4 = PyList_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 219, __pyx_L1_error)
+    __pyx_t_4 = PyList_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 221, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_1);
-    if (__Pyx_PyList_SET_ITEM(__pyx_t_4, 0, __pyx_t_1)) __PYX_ERR(0, 219, __pyx_L1_error);
+    if (__Pyx_PyList_SET_ITEM(__pyx_t_4, 0, __pyx_t_1)) __PYX_ERR(0, 221, __pyx_L1_error);
     __pyx_t_1 = 0;
-    __pyx_t_1 = PyNumber_InPlaceAdd(__pyx_v_epochs, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 219, __pyx_L1_error)
+    __pyx_t_1 = PyNumber_InPlaceAdd(__pyx_v_epochs, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 221, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF_SET(__pyx_v_epochs, ((PyObject*)__pyx_t_1));
     __pyx_t_1 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":217
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":219
  *         epochs += [itr.first]
  * 
  *     for itr in valid:             # <<<<<<<<<<<<<<
  *         folds += list(valid[itr.first].accuracy)
  *         epochs += [itr.first]
  */
   }
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":221
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":223
  *         epochs += [itr.first]
  * 
  *     for itr in test:             # <<<<<<<<<<<<<<
  *         folds += list(test[itr.first].accuracy)
  *         epochs += [itr.first]
  */
   __pyx_t_2 = __pyx_v_test.begin();
   for (;;) {
     if (!(__pyx_t_2 != __pyx_v_test.end())) break;
     __pyx_t_3 = *__pyx_t_2;
     ++__pyx_t_2;
     __pyx_v_itr = __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_3);
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":222
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":224
  * 
  *     for itr in test:
  *         folds += list(test[itr.first].accuracy)             # <<<<<<<<<<<<<<
  *         epochs += [itr.first]
  * 
  */
-    __pyx_t_1 = __pyx_convert_map_to_py_int____std_3a__3a_map_3c_std_3a__3a_string_2c_struct__point_t_3e___((__pyx_v_test[__pyx_v_itr.first])->accuracy); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 222, __pyx_L1_error)
+    __pyx_t_1 = __pyx_convert_map_to_py_int____std_3a__3a_map_3c_std_3a__3a_string_2c_struct__point_t_3e___((__pyx_v_test[__pyx_v_itr.first])->accuracy); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 224, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_4 = __Pyx_PySequence_ListKeepNew(__pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 222, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PySequence_ListKeepNew(__pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 224, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = PyNumber_InPlaceAdd(__pyx_v_folds, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 222, __pyx_L1_error)
+    __pyx_t_1 = PyNumber_InPlaceAdd(__pyx_v_folds, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 224, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF_SET(__pyx_v_folds, ((PyObject*)__pyx_t_1));
     __pyx_t_1 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":223
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":225
  *     for itr in test:
  *         folds += list(test[itr.first].accuracy)
  *         epochs += [itr.first]             # <<<<<<<<<<<<<<
  * 
  *     cdef point_t pnt
  */
-    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_itr.first); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 223, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_itr.first); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 225, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_4 = PyList_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 223, __pyx_L1_error)
+    __pyx_t_4 = PyList_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 225, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_1);
-    if (__Pyx_PyList_SET_ITEM(__pyx_t_4, 0, __pyx_t_1)) __PYX_ERR(0, 223, __pyx_L1_error);
+    if (__Pyx_PyList_SET_ITEM(__pyx_t_4, 0, __pyx_t_1)) __PYX_ERR(0, 225, __pyx_L1_error);
     __pyx_t_1 = 0;
-    __pyx_t_1 = PyNumber_InPlaceAdd(__pyx_v_epochs, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 223, __pyx_L1_error)
+    __pyx_t_1 = PyNumber_InPlaceAdd(__pyx_v_epochs, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 225, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF_SET(__pyx_v_epochs, ((PyObject*)__pyx_t_1));
     __pyx_t_1 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":221
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":223
  *         epochs += [itr.first]
  * 
  *     for itr in test:             # <<<<<<<<<<<<<<
  *         folds += list(test[itr.first].accuracy)
  *         epochs += [itr.first]
  */
   }
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":226
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":228
  * 
  *     cdef point_t pnt
  *     cdef dict lines = {}             # <<<<<<<<<<<<<<
  *     for epoch in sorted(set(epochs)):
  *         for kf in sorted(set(folds)):
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 226, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 228, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_lines = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":227
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":229
  *     cdef point_t pnt
  *     cdef dict lines = {}
  *     for epoch in sorted(set(epochs)):             # <<<<<<<<<<<<<<
  *         for kf in sorted(set(folds)):
  *             if train.count(epoch) and train[epoch].accuracy.count(kf):
  */
-  __pyx_t_4 = PySet_New(__pyx_v_epochs); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 227, __pyx_L1_error)
+  __pyx_t_4 = PySet_New(__pyx_v_epochs); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 229, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = PySequence_List(__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 227, __pyx_L1_error)
+  __pyx_t_5 = PySequence_List(__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 229, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_1 = ((PyObject*)__pyx_t_5);
   __pyx_t_5 = 0;
-  __pyx_t_6 = PyList_Sort(__pyx_t_1); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 227, __pyx_L1_error)
+  __pyx_t_6 = PyList_Sort(__pyx_t_1); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 229, __pyx_L1_error)
   __pyx_t_5 = __pyx_t_1; __Pyx_INCREF(__pyx_t_5);
   __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   for (;;) {
     {
       Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_5);
       #if !CYTHON_ASSUME_SAFE_MACROS
-      if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 227, __pyx_L1_error)
+      if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 229, __pyx_L1_error)
       #endif
       if (__pyx_t_7 >= __pyx_temp) break;
     }
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-    __pyx_t_1 = PyList_GET_ITEM(__pyx_t_5, __pyx_t_7); __Pyx_INCREF(__pyx_t_1); __pyx_t_7++; if (unlikely((0 < 0))) __PYX_ERR(0, 227, __pyx_L1_error)
+    __pyx_t_1 = PyList_GET_ITEM(__pyx_t_5, __pyx_t_7); __Pyx_INCREF(__pyx_t_1); __pyx_t_7++; if (unlikely((0 < 0))) __PYX_ERR(0, 229, __pyx_L1_error)
     #else
-    __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_5, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 227, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_5, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 229, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     #endif
-    __pyx_t_8 = __Pyx_PyInt_As_int(__pyx_t_1); if (unlikely((__pyx_t_8 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 227, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyInt_As_int(__pyx_t_1); if (unlikely((__pyx_t_8 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 229, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_v_epoch = __pyx_t_8;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":228
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":230
  *     cdef dict lines = {}
  *     for epoch in sorted(set(epochs)):
  *         for kf in sorted(set(folds)):             # <<<<<<<<<<<<<<
  *             if train.count(epoch) and train[epoch].accuracy.count(kf):
  *                 for its in train[epoch].accuracy[kf]: tmp_tr[its.first].push_back(its.second)
  */
-    __pyx_t_4 = PySet_New(__pyx_v_folds); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 228, __pyx_L1_error)
+    __pyx_t_4 = PySet_New(__pyx_v_folds); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 230, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_9 = PySequence_List(__pyx_t_4); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 228, __pyx_L1_error)
+    __pyx_t_9 = PySequence_List(__pyx_t_4); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 230, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_1 = ((PyObject*)__pyx_t_9);
     __pyx_t_9 = 0;
-    __pyx_t_6 = PyList_Sort(__pyx_t_1); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 228, __pyx_L1_error)
+    __pyx_t_6 = PyList_Sort(__pyx_t_1); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 230, __pyx_L1_error)
     __pyx_t_9 = __pyx_t_1; __Pyx_INCREF(__pyx_t_9);
     __pyx_t_10 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     for (;;) {
       {
         Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_9);
         #if !CYTHON_ASSUME_SAFE_MACROS
-        if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 228, __pyx_L1_error)
+        if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 230, __pyx_L1_error)
         #endif
         if (__pyx_t_10 >= __pyx_temp) break;
       }
       #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-      __pyx_t_1 = PyList_GET_ITEM(__pyx_t_9, __pyx_t_10); __Pyx_INCREF(__pyx_t_1); __pyx_t_10++; if (unlikely((0 < 0))) __PYX_ERR(0, 228, __pyx_L1_error)
+      __pyx_t_1 = PyList_GET_ITEM(__pyx_t_9, __pyx_t_10); __Pyx_INCREF(__pyx_t_1); __pyx_t_10++; if (unlikely((0 < 0))) __PYX_ERR(0, 230, __pyx_L1_error)
       #else
-      __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_9, __pyx_t_10); __pyx_t_10++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 228, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_9, __pyx_t_10); __pyx_t_10++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 230, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       #endif
-      __pyx_t_8 = __Pyx_PyInt_As_int(__pyx_t_1); if (unlikely((__pyx_t_8 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 228, __pyx_L1_error)
+      __pyx_t_8 = __Pyx_PyInt_As_int(__pyx_t_1); if (unlikely((__pyx_t_8 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 230, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_v_kf = __pyx_t_8;
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":229
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":231
  *     for epoch in sorted(set(epochs)):
  *         for kf in sorted(set(folds)):
  *             if train.count(epoch) and train[epoch].accuracy.count(kf):             # <<<<<<<<<<<<<<
  *                 for its in train[epoch].accuracy[kf]: tmp_tr[its.first].push_back(its.second)
  *             if valid.count(epoch) and valid[epoch].accuracy.count(kf):
  */
       __pyx_t_12 = (__pyx_v_train.count(__pyx_v_epoch) != 0);
@@ -29575,15 +29568,15 @@
         goto __pyx_L17_bool_binop_done;
       }
       __pyx_t_12 = ((__pyx_v_train[__pyx_v_epoch])->accuracy.count(__pyx_v_kf) != 0);
       __pyx_t_11 = __pyx_t_12;
       __pyx_L17_bool_binop_done:;
       if (__pyx_t_11) {
 
-        /* "src/cmodules/cyincludes/cyoptimizer.pyx":230
+        /* "src/cmodules/cyincludes/cyoptimizer.pyx":232
  *         for kf in sorted(set(folds)):
  *             if train.count(epoch) and train[epoch].accuracy.count(kf):
  *                 for its in train[epoch].accuracy[kf]: tmp_tr[its.first].push_back(its.second)             # <<<<<<<<<<<<<<
  *             if valid.count(epoch) and valid[epoch].accuracy.count(kf):
  *                 for its in valid[epoch].accuracy[kf]: tmp_va[its.first].push_back(its.second)
  */
         __pyx_t_14 = &((__pyx_v_train[__pyx_v_epoch])->accuracy[__pyx_v_kf]);
@@ -29593,28 +29586,28 @@
           __pyx_t_15 = *__pyx_t_13;
           ++__pyx_t_13;
           __pyx_v_its = __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_15);
           try {
             (__pyx_v_tmp_tr[__pyx_v_its.first]).push_back(__pyx_v_its.second);
           } catch(...) {
             __Pyx_CppExn2PyErr();
-            __PYX_ERR(0, 230, __pyx_L1_error)
+            __PYX_ERR(0, 232, __pyx_L1_error)
           }
         }
 
-        /* "src/cmodules/cyincludes/cyoptimizer.pyx":229
+        /* "src/cmodules/cyincludes/cyoptimizer.pyx":231
  *     for epoch in sorted(set(epochs)):
  *         for kf in sorted(set(folds)):
  *             if train.count(epoch) and train[epoch].accuracy.count(kf):             # <<<<<<<<<<<<<<
  *                 for its in train[epoch].accuracy[kf]: tmp_tr[its.first].push_back(its.second)
  *             if valid.count(epoch) and valid[epoch].accuracy.count(kf):
  */
       }
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":231
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":233
  *             if train.count(epoch) and train[epoch].accuracy.count(kf):
  *                 for its in train[epoch].accuracy[kf]: tmp_tr[its.first].push_back(its.second)
  *             if valid.count(epoch) and valid[epoch].accuracy.count(kf):             # <<<<<<<<<<<<<<
  *                 for its in valid[epoch].accuracy[kf]: tmp_va[its.first].push_back(its.second)
  *             if test.count(epoch) and test[epoch].accuracy.count(kf):
  */
       __pyx_t_12 = (__pyx_v_valid.count(__pyx_v_epoch) != 0);
@@ -29624,15 +29617,15 @@
         goto __pyx_L23_bool_binop_done;
       }
       __pyx_t_12 = ((__pyx_v_valid[__pyx_v_epoch])->accuracy.count(__pyx_v_kf) != 0);
       __pyx_t_11 = __pyx_t_12;
       __pyx_L23_bool_binop_done:;
       if (__pyx_t_11) {
 
-        /* "src/cmodules/cyincludes/cyoptimizer.pyx":232
+        /* "src/cmodules/cyincludes/cyoptimizer.pyx":234
  *                 for its in train[epoch].accuracy[kf]: tmp_tr[its.first].push_back(its.second)
  *             if valid.count(epoch) and valid[epoch].accuracy.count(kf):
  *                 for its in valid[epoch].accuracy[kf]: tmp_va[its.first].push_back(its.second)             # <<<<<<<<<<<<<<
  *             if test.count(epoch) and test[epoch].accuracy.count(kf):
  *                 for its in test[epoch].accuracy[kf]: tmp_te[its.first].push_back(its.second)
  */
         __pyx_t_14 = &((__pyx_v_valid[__pyx_v_epoch])->accuracy[__pyx_v_kf]);
@@ -29642,28 +29635,28 @@
           __pyx_t_15 = *__pyx_t_13;
           ++__pyx_t_13;
           __pyx_v_its = __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_15);
           try {
             (__pyx_v_tmp_va[__pyx_v_its.first]).push_back(__pyx_v_its.second);
           } catch(...) {
             __Pyx_CppExn2PyErr();
-            __PYX_ERR(0, 232, __pyx_L1_error)
+            __PYX_ERR(0, 234, __pyx_L1_error)
           }
         }
 
-        /* "src/cmodules/cyincludes/cyoptimizer.pyx":231
+        /* "src/cmodules/cyincludes/cyoptimizer.pyx":233
  *             if train.count(epoch) and train[epoch].accuracy.count(kf):
  *                 for its in train[epoch].accuracy[kf]: tmp_tr[its.first].push_back(its.second)
  *             if valid.count(epoch) and valid[epoch].accuracy.count(kf):             # <<<<<<<<<<<<<<
  *                 for its in valid[epoch].accuracy[kf]: tmp_va[its.first].push_back(its.second)
  *             if test.count(epoch) and test[epoch].accuracy.count(kf):
  */
       }
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":233
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":235
  *             if valid.count(epoch) and valid[epoch].accuracy.count(kf):
  *                 for its in valid[epoch].accuracy[kf]: tmp_va[its.first].push_back(its.second)
  *             if test.count(epoch) and test[epoch].accuracy.count(kf):             # <<<<<<<<<<<<<<
  *                 for its in test[epoch].accuracy[kf]: tmp_te[its.first].push_back(its.second)
  * 
  */
       __pyx_t_12 = (__pyx_v_test.count(__pyx_v_epoch) != 0);
@@ -29673,15 +29666,15 @@
         goto __pyx_L29_bool_binop_done;
       }
       __pyx_t_12 = ((__pyx_v_test[__pyx_v_epoch])->accuracy.count(__pyx_v_kf) != 0);
       __pyx_t_11 = __pyx_t_12;
       __pyx_L29_bool_binop_done:;
       if (__pyx_t_11) {
 
-        /* "src/cmodules/cyincludes/cyoptimizer.pyx":234
+        /* "src/cmodules/cyincludes/cyoptimizer.pyx":236
  *                 for its in valid[epoch].accuracy[kf]: tmp_va[its.first].push_back(its.second)
  *             if test.count(epoch) and test[epoch].accuracy.count(kf):
  *                 for its in test[epoch].accuracy[kf]: tmp_te[its.first].push_back(its.second)             # <<<<<<<<<<<<<<
  * 
  *         lines = collapse_points(&tmp_tr, epoch, lines, "training", state, "acc")
  */
         __pyx_t_14 = &((__pyx_v_test[__pyx_v_epoch])->accuracy[__pyx_v_kf]);
@@ -29691,262 +29684,262 @@
           __pyx_t_15 = *__pyx_t_13;
           ++__pyx_t_13;
           __pyx_v_its = __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_15);
           try {
             (__pyx_v_tmp_te[__pyx_v_its.first]).push_back(__pyx_v_its.second);
           } catch(...) {
             __Pyx_CppExn2PyErr();
-            __PYX_ERR(0, 234, __pyx_L1_error)
+            __PYX_ERR(0, 236, __pyx_L1_error)
           }
         }
 
-        /* "src/cmodules/cyincludes/cyoptimizer.pyx":233
+        /* "src/cmodules/cyincludes/cyoptimizer.pyx":235
  *             if valid.count(epoch) and valid[epoch].accuracy.count(kf):
  *                 for its in valid[epoch].accuracy[kf]: tmp_va[its.first].push_back(its.second)
  *             if test.count(epoch) and test[epoch].accuracy.count(kf):             # <<<<<<<<<<<<<<
  *                 for its in test[epoch].accuracy[kf]: tmp_te[its.first].push_back(its.second)
  * 
  */
       }
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":228
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":230
  *     cdef dict lines = {}
  *     for epoch in sorted(set(epochs)):
  *         for kf in sorted(set(folds)):             # <<<<<<<<<<<<<<
  *             if train.count(epoch) and train[epoch].accuracy.count(kf):
  *                 for its in train[epoch].accuracy[kf]: tmp_tr[its.first].push_back(its.second)
  */
     }
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":236
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":238
  *                 for its in test[epoch].accuracy[kf]: tmp_te[its.first].push_back(its.second)
  * 
  *         lines = collapse_points(&tmp_tr, epoch, lines, "training", state, "acc")             # <<<<<<<<<<<<<<
  *         lines = collapse_points(&tmp_va, epoch, lines, "validation", state, "acc")
  *         lines = collapse_points(&tmp_te, epoch, lines, "evaluation", state, "acc")
  */
-    __pyx_t_9 = __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_collapse_points((&__pyx_v_tmp_tr), __pyx_v_epoch, __pyx_v_lines, __pyx_n_u_training, __pyx_v_state, __pyx_n_u_acc); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 236, __pyx_L1_error)
+    __pyx_t_9 = __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_collapse_points((&__pyx_v_tmp_tr), __pyx_v_epoch, __pyx_v_lines, __pyx_n_u_training, __pyx_v_state, __pyx_n_u_acc); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 238, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     __Pyx_DECREF_SET(__pyx_v_lines, ((PyObject*)__pyx_t_9));
     __pyx_t_9 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":237
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":239
  * 
  *         lines = collapse_points(&tmp_tr, epoch, lines, "training", state, "acc")
  *         lines = collapse_points(&tmp_va, epoch, lines, "validation", state, "acc")             # <<<<<<<<<<<<<<
  *         lines = collapse_points(&tmp_te, epoch, lines, "evaluation", state, "acc")
  * 
  */
-    __pyx_t_9 = __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_collapse_points((&__pyx_v_tmp_va), __pyx_v_epoch, __pyx_v_lines, __pyx_n_u_validation, __pyx_v_state, __pyx_n_u_acc); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 237, __pyx_L1_error)
+    __pyx_t_9 = __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_collapse_points((&__pyx_v_tmp_va), __pyx_v_epoch, __pyx_v_lines, __pyx_n_u_validation, __pyx_v_state, __pyx_n_u_acc); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 239, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     __Pyx_DECREF_SET(__pyx_v_lines, ((PyObject*)__pyx_t_9));
     __pyx_t_9 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":238
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":240
  *         lines = collapse_points(&tmp_tr, epoch, lines, "training", state, "acc")
  *         lines = collapse_points(&tmp_va, epoch, lines, "validation", state, "acc")
  *         lines = collapse_points(&tmp_te, epoch, lines, "evaluation", state, "acc")             # <<<<<<<<<<<<<<
  * 
  *     for var_name in lines:
  */
-    __pyx_t_9 = __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_collapse_points((&__pyx_v_tmp_te), __pyx_v_epoch, __pyx_v_lines, __pyx_n_u_evaluation, __pyx_v_state, __pyx_n_u_acc); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 238, __pyx_L1_error)
+    __pyx_t_9 = __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_collapse_points((&__pyx_v_tmp_te), __pyx_v_epoch, __pyx_v_lines, __pyx_n_u_evaluation, __pyx_v_state, __pyx_n_u_acc); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 240, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     __Pyx_DECREF_SET(__pyx_v_lines, ((PyObject*)__pyx_t_9));
     __pyx_t_9 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":227
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":229
  *     cdef point_t pnt
  *     cdef dict lines = {}
  *     for epoch in sorted(set(epochs)):             # <<<<<<<<<<<<<<
  *         for kf in sorted(set(folds)):
  *             if train.count(epoch) and train[epoch].accuracy.count(kf):
  */
   }
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":240
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":242
  *         lines = collapse_points(&tmp_te, epoch, lines, "evaluation", state, "acc")
  * 
  *     for var_name in lines:             # <<<<<<<<<<<<<<
  *         for mode in lines[var_name]: lines[var_name][mode] = TLine(**lines[var_name][mode])
  *         tmpl = template_tline(path, "Epoch", "Accuracy", "Achieved Accuracy of " + var_name)
  */
   __pyx_t_7 = 0;
   if (unlikely(__pyx_v_lines == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-    __PYX_ERR(0, 240, __pyx_L1_error)
+    __PYX_ERR(0, 242, __pyx_L1_error)
   }
-  __pyx_t_9 = __Pyx_dict_iterator(__pyx_v_lines, 1, ((PyObject *)NULL), (&__pyx_t_10), (&__pyx_t_8)); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 240, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_dict_iterator(__pyx_v_lines, 1, ((PyObject *)NULL), (&__pyx_t_10), (&__pyx_t_8)); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 242, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __Pyx_XDECREF(__pyx_t_5);
   __pyx_t_5 = __pyx_t_9;
   __pyx_t_9 = 0;
   while (1) {
     __pyx_t_16 = __Pyx_dict_iter_next(__pyx_t_5, __pyx_t_10, &__pyx_t_7, &__pyx_t_9, NULL, NULL, __pyx_t_8);
     if (unlikely(__pyx_t_16 == 0)) break;
-    if (unlikely(__pyx_t_16 == -1)) __PYX_ERR(0, 240, __pyx_L1_error)
+    if (unlikely(__pyx_t_16 == -1)) __PYX_ERR(0, 242, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     __Pyx_XDECREF_SET(__pyx_v_var_name, __pyx_t_9);
     __pyx_t_9 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":241
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":243
  * 
  *     for var_name in lines:
  *         for mode in lines[var_name]: lines[var_name][mode] = TLine(**lines[var_name][mode])             # <<<<<<<<<<<<<<
  *         tmpl = template_tline(path, "Epoch", "Accuracy", "Achieved Accuracy of " + var_name)
  *         tmpl["Filename"] = var_name + "_accuracy"
  */
     if (unlikely(__pyx_v_lines == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 241, __pyx_L1_error)
+      __PYX_ERR(0, 243, __pyx_L1_error)
     }
-    __pyx_t_9 = __Pyx_PyDict_GetItem(__pyx_v_lines, __pyx_v_var_name); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 241, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyDict_GetItem(__pyx_v_lines, __pyx_v_var_name); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 243, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     if (likely(PyList_CheckExact(__pyx_t_9)) || PyTuple_CheckExact(__pyx_t_9)) {
       __pyx_t_1 = __pyx_t_9; __Pyx_INCREF(__pyx_t_1);
       __pyx_t_17 = 0;
       __pyx_t_18 = NULL;
     } else {
-      __pyx_t_17 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_t_9); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 241, __pyx_L1_error)
+      __pyx_t_17 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_t_9); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 243, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_18 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_1); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 241, __pyx_L1_error)
+      __pyx_t_18 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_1); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 243, __pyx_L1_error)
     }
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     for (;;) {
       if (likely(!__pyx_t_18)) {
         if (likely(PyList_CheckExact(__pyx_t_1))) {
           {
             Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_1);
             #if !CYTHON_ASSUME_SAFE_MACROS
-            if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 241, __pyx_L1_error)
+            if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 243, __pyx_L1_error)
             #endif
             if (__pyx_t_17 >= __pyx_temp) break;
           }
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_9 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_17); __Pyx_INCREF(__pyx_t_9); __pyx_t_17++; if (unlikely((0 < 0))) __PYX_ERR(0, 241, __pyx_L1_error)
+          __pyx_t_9 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_17); __Pyx_INCREF(__pyx_t_9); __pyx_t_17++; if (unlikely((0 < 0))) __PYX_ERR(0, 243, __pyx_L1_error)
           #else
-          __pyx_t_9 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_17); __pyx_t_17++; if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 241, __pyx_L1_error)
+          __pyx_t_9 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_17); __pyx_t_17++; if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 243, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_9);
           #endif
         } else {
           {
             Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_1);
             #if !CYTHON_ASSUME_SAFE_MACROS
-            if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 241, __pyx_L1_error)
+            if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 243, __pyx_L1_error)
             #endif
             if (__pyx_t_17 >= __pyx_temp) break;
           }
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_9 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_17); __Pyx_INCREF(__pyx_t_9); __pyx_t_17++; if (unlikely((0 < 0))) __PYX_ERR(0, 241, __pyx_L1_error)
+          __pyx_t_9 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_17); __Pyx_INCREF(__pyx_t_9); __pyx_t_17++; if (unlikely((0 < 0))) __PYX_ERR(0, 243, __pyx_L1_error)
           #else
-          __pyx_t_9 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_17); __pyx_t_17++; if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 241, __pyx_L1_error)
+          __pyx_t_9 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_17); __pyx_t_17++; if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 243, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_9);
           #endif
         }
       } else {
         __pyx_t_9 = __pyx_t_18(__pyx_t_1);
         if (unlikely(!__pyx_t_9)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 241, __pyx_L1_error)
+            else __PYX_ERR(0, 243, __pyx_L1_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_9);
       }
       __Pyx_XDECREF_SET(__pyx_v_mode, __pyx_t_9);
       __pyx_t_9 = 0;
-      __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_TLine); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 241, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_TLine); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 243, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
       if (unlikely(__pyx_v_lines == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-        __PYX_ERR(0, 241, __pyx_L1_error)
+        __PYX_ERR(0, 243, __pyx_L1_error)
       }
-      __pyx_t_19 = __Pyx_PyDict_GetItem(__pyx_v_lines, __pyx_v_var_name); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 241, __pyx_L1_error)
+      __pyx_t_19 = __Pyx_PyDict_GetItem(__pyx_v_lines, __pyx_v_var_name); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 243, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_19);
-      __pyx_t_20 = __Pyx_PyObject_GetItem(__pyx_t_19, __pyx_v_mode); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 241, __pyx_L1_error)
+      __pyx_t_20 = __Pyx_PyObject_GetItem(__pyx_t_19, __pyx_v_mode); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 243, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_20);
       __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
       if (unlikely(__pyx_t_20 == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "argument after ** must be a mapping, not NoneType");
-        __PYX_ERR(0, 241, __pyx_L1_error)
+        __PYX_ERR(0, 243, __pyx_L1_error)
       }
       if (likely(PyDict_CheckExact(__pyx_t_20))) {
-        __pyx_t_4 = PyDict_Copy(__pyx_t_20); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 241, __pyx_L1_error)
+        __pyx_t_4 = PyDict_Copy(__pyx_t_20); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 243, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
       } else {
-        __pyx_t_4 = __Pyx_PyObject_CallOneArg((PyObject*)&PyDict_Type, __pyx_t_20); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 241, __pyx_L1_error)
+        __pyx_t_4 = __Pyx_PyObject_CallOneArg((PyObject*)&PyDict_Type, __pyx_t_20); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 243, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
       }
-      __pyx_t_20 = __Pyx_PyObject_Call(__pyx_t_9, __pyx_empty_tuple, __pyx_t_4); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 241, __pyx_L1_error)
+      __pyx_t_20 = __Pyx_PyObject_Call(__pyx_t_9, __pyx_empty_tuple, __pyx_t_4); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 243, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_20);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       if (unlikely(__pyx_v_lines == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-        __PYX_ERR(0, 241, __pyx_L1_error)
+        __PYX_ERR(0, 243, __pyx_L1_error)
       }
-      __pyx_t_4 = __Pyx_PyDict_GetItem(__pyx_v_lines, __pyx_v_var_name); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 241, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyDict_GetItem(__pyx_v_lines, __pyx_v_var_name); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 243, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      if (unlikely((PyObject_SetItem(__pyx_t_4, __pyx_v_mode, __pyx_t_20) < 0))) __PYX_ERR(0, 241, __pyx_L1_error)
+      if (unlikely((PyObject_SetItem(__pyx_t_4, __pyx_v_mode, __pyx_t_20) < 0))) __PYX_ERR(0, 243, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
     }
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":242
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":244
  *     for var_name in lines:
  *         for mode in lines[var_name]: lines[var_name][mode] = TLine(**lines[var_name][mode])
  *         tmpl = template_tline(path, "Epoch", "Accuracy", "Achieved Accuracy of " + var_name)             # <<<<<<<<<<<<<<
  *         tmpl["Filename"] = var_name + "_accuracy"
  *         tmpl["Lines"] = list(lines[var_name].values())
  */
-    __pyx_t_1 = PyNumber_Add(__pyx_kp_u_Achieved_Accuracy_of, __pyx_v_var_name); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 242, __pyx_L1_error)
+    __pyx_t_1 = PyNumber_Add(__pyx_kp_u_Achieved_Accuracy_of, __pyx_v_var_name); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 244, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_t_1))) __PYX_ERR(0, 242, __pyx_L1_error)
-    __pyx_t_20 = __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_template_tline(__pyx_v_path, __pyx_n_u_Epoch_2, __pyx_n_u_Accuracy, ((PyObject*)__pyx_t_1)); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 242, __pyx_L1_error)
+    if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_t_1))) __PYX_ERR(0, 244, __pyx_L1_error)
+    __pyx_t_20 = __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_template_tline(__pyx_v_path, __pyx_n_u_Epoch_2, __pyx_n_u_Accuracy, ((PyObject*)__pyx_t_1)); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 244, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_20);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_v_tmpl = ((PyObject*)__pyx_t_20);
     __pyx_t_20 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":243
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":245
  *         for mode in lines[var_name]: lines[var_name][mode] = TLine(**lines[var_name][mode])
  *         tmpl = template_tline(path, "Epoch", "Accuracy", "Achieved Accuracy of " + var_name)
  *         tmpl["Filename"] = var_name + "_accuracy"             # <<<<<<<<<<<<<<
  *         tmpl["Lines"] = list(lines[var_name].values())
- *         tl = TLine(**tmpl)
+ *         tmpl["yMax"] = 100
  */
-    __pyx_t_20 = PyNumber_Add(__pyx_v_var_name, __pyx_n_u_accuracy_3); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 243, __pyx_L1_error)
+    __pyx_t_20 = PyNumber_Add(__pyx_v_var_name, __pyx_n_u_accuracy_3); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 245, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_20);
     if (unlikely(__pyx_v_tmpl == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 243, __pyx_L1_error)
+      __PYX_ERR(0, 245, __pyx_L1_error)
     }
-    if (unlikely((PyDict_SetItem(__pyx_v_tmpl, __pyx_n_u_Filename, __pyx_t_20) < 0))) __PYX_ERR(0, 243, __pyx_L1_error)
+    if (unlikely((PyDict_SetItem(__pyx_v_tmpl, __pyx_n_u_Filename, __pyx_t_20) < 0))) __PYX_ERR(0, 245, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":244
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":246
  *         tmpl = template_tline(path, "Epoch", "Accuracy", "Achieved Accuracy of " + var_name)
  *         tmpl["Filename"] = var_name + "_accuracy"
  *         tmpl["Lines"] = list(lines[var_name].values())             # <<<<<<<<<<<<<<
+ *         tmpl["yMax"] = 100
  *         tl = TLine(**tmpl)
- *         tl.yMax = 100
  */
     if (unlikely(__pyx_v_lines == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 244, __pyx_L1_error)
+      __PYX_ERR(0, 246, __pyx_L1_error)
     }
-    __pyx_t_1 = __Pyx_PyDict_GetItem(__pyx_v_lines, __pyx_v_var_name); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 244, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyDict_GetItem(__pyx_v_lines, __pyx_v_var_name); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 246, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_values); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 244, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_values); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 246, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_1 = NULL;
     __pyx_t_16 = 0;
     #if CYTHON_UNPACK_METHODS
     if (likely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_4);
@@ -29959,67 +29952,71 @@
       }
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_1, NULL};
       __pyx_t_20 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_16, 0+__pyx_t_16);
       __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-      if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 244, __pyx_L1_error)
+      if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 246, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_20);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     }
-    __pyx_t_4 = __Pyx_PySequence_ListKeepNew(__pyx_t_20); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 244, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PySequence_ListKeepNew(__pyx_t_20); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 246, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
     if (unlikely(__pyx_v_tmpl == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 244, __pyx_L1_error)
+      __PYX_ERR(0, 246, __pyx_L1_error)
     }
-    if (unlikely((PyDict_SetItem(__pyx_v_tmpl, __pyx_n_u_Lines, __pyx_t_4) < 0))) __PYX_ERR(0, 244, __pyx_L1_error)
+    if (unlikely((PyDict_SetItem(__pyx_v_tmpl, __pyx_n_u_Lines, __pyx_t_4) < 0))) __PYX_ERR(0, 246, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":245
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":247
  *         tmpl["Filename"] = var_name + "_accuracy"
  *         tmpl["Lines"] = list(lines[var_name].values())
+ *         tmpl["yMax"] = 100             # <<<<<<<<<<<<<<
+ *         tl = TLine(**tmpl)
+ *         tl.SaveFigure()
+ */
+    if (unlikely(__pyx_v_tmpl == Py_None)) {
+      PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
+      __PYX_ERR(0, 247, __pyx_L1_error)
+    }
+    if (unlikely((PyDict_SetItem(__pyx_v_tmpl, __pyx_n_u_yMax, __pyx_int_100) < 0))) __PYX_ERR(0, 247, __pyx_L1_error)
+
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":248
+ *         tmpl["Lines"] = list(lines[var_name].values())
+ *         tmpl["yMax"] = 100
  *         tl = TLine(**tmpl)             # <<<<<<<<<<<<<<
- *         tl.yMax = 100
  *         tl.SaveFigure()
+ *         del tl
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_TLine); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 245, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_TLine); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 248, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     if (unlikely(__pyx_v_tmpl == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "argument after ** must be a mapping, not NoneType");
-      __PYX_ERR(0, 245, __pyx_L1_error)
+      __PYX_ERR(0, 248, __pyx_L1_error)
     }
-    __pyx_t_20 = PyDict_Copy(__pyx_v_tmpl); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 245, __pyx_L1_error)
+    __pyx_t_20 = PyDict_Copy(__pyx_v_tmpl); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 248, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_20);
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_empty_tuple, __pyx_t_20); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 245, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_empty_tuple, __pyx_t_20); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 248, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
     __pyx_v_tl = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":246
- *         tmpl["Lines"] = list(lines[var_name].values())
- *         tl = TLine(**tmpl)
- *         tl.yMax = 100             # <<<<<<<<<<<<<<
- *         tl.SaveFigure()
- *         del tl
- */
-    if (__Pyx_PyObject_SetAttrStr(__pyx_v_tl, __pyx_n_s_yMax, __pyx_int_100) < 0) __PYX_ERR(0, 246, __pyx_L1_error)
-
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":247
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":249
+ *         tmpl["yMax"] = 100
  *         tl = TLine(**tmpl)
- *         tl.yMax = 100
  *         tl.SaveFigure()             # <<<<<<<<<<<<<<
  *         del tl
  *         del tmpl
  */
-    __pyx_t_20 = __Pyx_PyObject_GetAttrStr(__pyx_v_tl, __pyx_n_s_SaveFigure); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 247, __pyx_L1_error)
+    __pyx_t_20 = __Pyx_PyObject_GetAttrStr(__pyx_v_tl, __pyx_n_s_SaveFigure); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 249, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_20);
     __pyx_t_4 = NULL;
     __pyx_t_16 = 0;
     #if CYTHON_UNPACK_METHODS
     if (likely(PyMethod_Check(__pyx_t_20))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_20);
       if (likely(__pyx_t_4)) {
@@ -30031,86 +30028,86 @@
       }
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_4, NULL};
       __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_20, __pyx_callargs+1-__pyx_t_16, 0+__pyx_t_16);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 247, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 249, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
     }
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":248
- *         tl.yMax = 100
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":250
+ *         tl = TLine(**tmpl)
  *         tl.SaveFigure()
  *         del tl             # <<<<<<<<<<<<<<
  *         del tmpl
  *     del lines
  */
     __Pyx_DECREF(__pyx_v_tl); __pyx_v_tl = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":249
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":251
  *         tl.SaveFigure()
  *         del tl
  *         del tmpl             # <<<<<<<<<<<<<<
  *     del lines
  *     del folds
  */
     __Pyx_DECREF(__pyx_v_tmpl); __pyx_v_tmpl = 0;
   }
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":250
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":252
  *         del tl
  *         del tmpl
  *     del lines             # <<<<<<<<<<<<<<
  *     del folds
  *     tmp_tr.clear()
  */
   __Pyx_DECREF(__pyx_v_lines); __pyx_v_lines = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":251
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":253
  *         del tmpl
  *     del lines
  *     del folds             # <<<<<<<<<<<<<<
  *     tmp_tr.clear()
  *     tmp_va.clear()
  */
   __Pyx_DECREF(__pyx_v_folds); __pyx_v_folds = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":252
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":254
  *     del lines
  *     del folds
  *     tmp_tr.clear()             # <<<<<<<<<<<<<<
  *     tmp_va.clear()
  *     tmp_te.clear()
  */
   __pyx_v_tmp_tr.clear();
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":253
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":255
  *     del folds
  *     tmp_tr.clear()
  *     tmp_va.clear()             # <<<<<<<<<<<<<<
  *     tmp_te.clear()
  * 
  */
   __pyx_v_tmp_va.clear();
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":254
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":256
  *     tmp_tr.clear()
  *     tmp_va.clear()
  *     tmp_te.clear()             # <<<<<<<<<<<<<<
  * 
  * cdef void make_loss_plots(map[int, CyEpoch*] train, map[int, CyEpoch*] valid, map[int, CyEpoch*] test, str path, report_t* state):
  */
   __pyx_v_tmp_te.clear();
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":200
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":202
  *     return lines
  * 
  * cdef void make_accuracy_plots(map[int, CyEpoch*] train, map[int, CyEpoch*] valid, map[int, CyEpoch*] test, str path, report_t* state):             # <<<<<<<<<<<<<<
  *     cdef pair[int, CyEpoch*] itr
  *     cdef pair[string, point_t] its
  */
 
@@ -30131,15 +30128,15 @@
   __Pyx_XDECREF(__pyx_v_var_name);
   __Pyx_XDECREF(__pyx_v_mode);
   __Pyx_XDECREF(__pyx_v_tmpl);
   __Pyx_XDECREF(__pyx_v_tl);
   __Pyx_RefNannyFinishContext();
 }
 
-/* "src/cmodules/cyincludes/cyoptimizer.pyx":256
+/* "src/cmodules/cyincludes/cyoptimizer.pyx":258
  *     tmp_te.clear()
  * 
  * cdef void make_loss_plots(map[int, CyEpoch*] train, map[int, CyEpoch*] valid, map[int, CyEpoch*] test, str path, report_t* state):             # <<<<<<<<<<<<<<
  *     cdef pair[int, CyEpoch*] itr
  *     cdef pair[string, point_t] its
  */
 
@@ -30180,306 +30177,306 @@
   PyObject *__pyx_t_19 = NULL;
   PyObject *__pyx_t_20 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("make_loss_plots", 1);
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":265
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":267
  *     cdef map[string, vector[point_t]] tmp_te
  * 
  *     cdef list folds = []             # <<<<<<<<<<<<<<
  *     cdef list epochs = []
  *     cdef int epoch, kf
  */
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 265, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 267, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_folds = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":266
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":268
  * 
  *     cdef list folds = []
  *     cdef list epochs = []             # <<<<<<<<<<<<<<
  *     cdef int epoch, kf
  * 
  */
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 266, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 268, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_epochs = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":269
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":271
  *     cdef int epoch, kf
  * 
  *     for itr in train:             # <<<<<<<<<<<<<<
  *         folds += list(train[itr.first].loss)
  *         epochs += [itr.first]
  */
   __pyx_t_2 = __pyx_v_train.begin();
   for (;;) {
     if (!(__pyx_t_2 != __pyx_v_train.end())) break;
     __pyx_t_3 = *__pyx_t_2;
     ++__pyx_t_2;
     __pyx_v_itr = __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_3);
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":270
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":272
  * 
  *     for itr in train:
  *         folds += list(train[itr.first].loss)             # <<<<<<<<<<<<<<
  *         epochs += [itr.first]
  * 
  */
-    __pyx_t_1 = __pyx_convert_map_to_py_int____std_3a__3a_map_3c_std_3a__3a_string_2c_struct__point_t_3e___((__pyx_v_train[__pyx_v_itr.first])->loss); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 270, __pyx_L1_error)
+    __pyx_t_1 = __pyx_convert_map_to_py_int____std_3a__3a_map_3c_std_3a__3a_string_2c_struct__point_t_3e___((__pyx_v_train[__pyx_v_itr.first])->loss); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 272, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_4 = __Pyx_PySequence_ListKeepNew(__pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 270, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PySequence_ListKeepNew(__pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 272, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = PyNumber_InPlaceAdd(__pyx_v_folds, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 270, __pyx_L1_error)
+    __pyx_t_1 = PyNumber_InPlaceAdd(__pyx_v_folds, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 272, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF_SET(__pyx_v_folds, ((PyObject*)__pyx_t_1));
     __pyx_t_1 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":271
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":273
  *     for itr in train:
  *         folds += list(train[itr.first].loss)
  *         epochs += [itr.first]             # <<<<<<<<<<<<<<
  * 
  *     for itr in valid:
  */
-    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_itr.first); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 271, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_itr.first); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 273, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_4 = PyList_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 271, __pyx_L1_error)
+    __pyx_t_4 = PyList_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 273, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_1);
-    if (__Pyx_PyList_SET_ITEM(__pyx_t_4, 0, __pyx_t_1)) __PYX_ERR(0, 271, __pyx_L1_error);
+    if (__Pyx_PyList_SET_ITEM(__pyx_t_4, 0, __pyx_t_1)) __PYX_ERR(0, 273, __pyx_L1_error);
     __pyx_t_1 = 0;
-    __pyx_t_1 = PyNumber_InPlaceAdd(__pyx_v_epochs, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 271, __pyx_L1_error)
+    __pyx_t_1 = PyNumber_InPlaceAdd(__pyx_v_epochs, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 273, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF_SET(__pyx_v_epochs, ((PyObject*)__pyx_t_1));
     __pyx_t_1 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":269
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":271
  *     cdef int epoch, kf
  * 
  *     for itr in train:             # <<<<<<<<<<<<<<
  *         folds += list(train[itr.first].loss)
  *         epochs += [itr.first]
  */
   }
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":273
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":275
  *         epochs += [itr.first]
  * 
  *     for itr in valid:             # <<<<<<<<<<<<<<
  *         folds += list(valid[itr.first].loss)
  *         epochs += [itr.first]
  */
   __pyx_t_2 = __pyx_v_valid.begin();
   for (;;) {
     if (!(__pyx_t_2 != __pyx_v_valid.end())) break;
     __pyx_t_3 = *__pyx_t_2;
     ++__pyx_t_2;
     __pyx_v_itr = __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_3);
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":274
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":276
  * 
  *     for itr in valid:
  *         folds += list(valid[itr.first].loss)             # <<<<<<<<<<<<<<
  *         epochs += [itr.first]
  * 
  */
-    __pyx_t_1 = __pyx_convert_map_to_py_int____std_3a__3a_map_3c_std_3a__3a_string_2c_struct__point_t_3e___((__pyx_v_valid[__pyx_v_itr.first])->loss); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 274, __pyx_L1_error)
+    __pyx_t_1 = __pyx_convert_map_to_py_int____std_3a__3a_map_3c_std_3a__3a_string_2c_struct__point_t_3e___((__pyx_v_valid[__pyx_v_itr.first])->loss); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 276, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_4 = __Pyx_PySequence_ListKeepNew(__pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 274, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PySequence_ListKeepNew(__pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 276, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = PyNumber_InPlaceAdd(__pyx_v_folds, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 274, __pyx_L1_error)
+    __pyx_t_1 = PyNumber_InPlaceAdd(__pyx_v_folds, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 276, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF_SET(__pyx_v_folds, ((PyObject*)__pyx_t_1));
     __pyx_t_1 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":275
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":277
  *     for itr in valid:
  *         folds += list(valid[itr.first].loss)
  *         epochs += [itr.first]             # <<<<<<<<<<<<<<
  * 
  *     for itr in test:
  */
-    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_itr.first); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 275, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_itr.first); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 277, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_4 = PyList_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 275, __pyx_L1_error)
+    __pyx_t_4 = PyList_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 277, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_1);
-    if (__Pyx_PyList_SET_ITEM(__pyx_t_4, 0, __pyx_t_1)) __PYX_ERR(0, 275, __pyx_L1_error);
+    if (__Pyx_PyList_SET_ITEM(__pyx_t_4, 0, __pyx_t_1)) __PYX_ERR(0, 277, __pyx_L1_error);
     __pyx_t_1 = 0;
-    __pyx_t_1 = PyNumber_InPlaceAdd(__pyx_v_epochs, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 275, __pyx_L1_error)
+    __pyx_t_1 = PyNumber_InPlaceAdd(__pyx_v_epochs, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 277, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF_SET(__pyx_v_epochs, ((PyObject*)__pyx_t_1));
     __pyx_t_1 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":273
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":275
  *         epochs += [itr.first]
  * 
  *     for itr in valid:             # <<<<<<<<<<<<<<
  *         folds += list(valid[itr.first].loss)
  *         epochs += [itr.first]
  */
   }
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":277
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":279
  *         epochs += [itr.first]
  * 
  *     for itr in test:             # <<<<<<<<<<<<<<
  *         folds += list(test[itr.first].loss)
  *         epochs += [itr.first]
  */
   __pyx_t_2 = __pyx_v_test.begin();
   for (;;) {
     if (!(__pyx_t_2 != __pyx_v_test.end())) break;
     __pyx_t_3 = *__pyx_t_2;
     ++__pyx_t_2;
     __pyx_v_itr = __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_3);
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":278
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":280
  * 
  *     for itr in test:
  *         folds += list(test[itr.first].loss)             # <<<<<<<<<<<<<<
  *         epochs += [itr.first]
  * 
  */
-    __pyx_t_1 = __pyx_convert_map_to_py_int____std_3a__3a_map_3c_std_3a__3a_string_2c_struct__point_t_3e___((__pyx_v_test[__pyx_v_itr.first])->loss); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 278, __pyx_L1_error)
+    __pyx_t_1 = __pyx_convert_map_to_py_int____std_3a__3a_map_3c_std_3a__3a_string_2c_struct__point_t_3e___((__pyx_v_test[__pyx_v_itr.first])->loss); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 280, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_4 = __Pyx_PySequence_ListKeepNew(__pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 278, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PySequence_ListKeepNew(__pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 280, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = PyNumber_InPlaceAdd(__pyx_v_folds, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 278, __pyx_L1_error)
+    __pyx_t_1 = PyNumber_InPlaceAdd(__pyx_v_folds, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 280, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF_SET(__pyx_v_folds, ((PyObject*)__pyx_t_1));
     __pyx_t_1 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":279
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":281
  *     for itr in test:
  *         folds += list(test[itr.first].loss)
  *         epochs += [itr.first]             # <<<<<<<<<<<<<<
  * 
  *     cdef point_t pnt
  */
-    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_itr.first); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 279, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_itr.first); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 281, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_4 = PyList_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 279, __pyx_L1_error)
+    __pyx_t_4 = PyList_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 281, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_1);
-    if (__Pyx_PyList_SET_ITEM(__pyx_t_4, 0, __pyx_t_1)) __PYX_ERR(0, 279, __pyx_L1_error);
+    if (__Pyx_PyList_SET_ITEM(__pyx_t_4, 0, __pyx_t_1)) __PYX_ERR(0, 281, __pyx_L1_error);
     __pyx_t_1 = 0;
-    __pyx_t_1 = PyNumber_InPlaceAdd(__pyx_v_epochs, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 279, __pyx_L1_error)
+    __pyx_t_1 = PyNumber_InPlaceAdd(__pyx_v_epochs, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 281, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF_SET(__pyx_v_epochs, ((PyObject*)__pyx_t_1));
     __pyx_t_1 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":277
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":279
  *         epochs += [itr.first]
  * 
  *     for itr in test:             # <<<<<<<<<<<<<<
  *         folds += list(test[itr.first].loss)
  *         epochs += [itr.first]
  */
   }
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":282
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":284
  * 
  *     cdef point_t pnt
  *     cdef dict lines = {}             # <<<<<<<<<<<<<<
  *     for epoch in sorted(set(epochs)):
  *         for kf in sorted(set(folds)):
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 282, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 284, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_lines = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":283
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":285
  *     cdef point_t pnt
  *     cdef dict lines = {}
  *     for epoch in sorted(set(epochs)):             # <<<<<<<<<<<<<<
  *         for kf in sorted(set(folds)):
  *             if train.count(epoch) and train[epoch].loss.count(kf):
  */
-  __pyx_t_4 = PySet_New(__pyx_v_epochs); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 283, __pyx_L1_error)
+  __pyx_t_4 = PySet_New(__pyx_v_epochs); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 285, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = PySequence_List(__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 283, __pyx_L1_error)
+  __pyx_t_5 = PySequence_List(__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 285, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_1 = ((PyObject*)__pyx_t_5);
   __pyx_t_5 = 0;
-  __pyx_t_6 = PyList_Sort(__pyx_t_1); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 283, __pyx_L1_error)
+  __pyx_t_6 = PyList_Sort(__pyx_t_1); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 285, __pyx_L1_error)
   __pyx_t_5 = __pyx_t_1; __Pyx_INCREF(__pyx_t_5);
   __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   for (;;) {
     {
       Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_5);
       #if !CYTHON_ASSUME_SAFE_MACROS
-      if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 283, __pyx_L1_error)
+      if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 285, __pyx_L1_error)
       #endif
       if (__pyx_t_7 >= __pyx_temp) break;
     }
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-    __pyx_t_1 = PyList_GET_ITEM(__pyx_t_5, __pyx_t_7); __Pyx_INCREF(__pyx_t_1); __pyx_t_7++; if (unlikely((0 < 0))) __PYX_ERR(0, 283, __pyx_L1_error)
+    __pyx_t_1 = PyList_GET_ITEM(__pyx_t_5, __pyx_t_7); __Pyx_INCREF(__pyx_t_1); __pyx_t_7++; if (unlikely((0 < 0))) __PYX_ERR(0, 285, __pyx_L1_error)
     #else
-    __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_5, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 283, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_5, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 285, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     #endif
-    __pyx_t_8 = __Pyx_PyInt_As_int(__pyx_t_1); if (unlikely((__pyx_t_8 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 283, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyInt_As_int(__pyx_t_1); if (unlikely((__pyx_t_8 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 285, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_v_epoch = __pyx_t_8;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":284
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":286
  *     cdef dict lines = {}
  *     for epoch in sorted(set(epochs)):
  *         for kf in sorted(set(folds)):             # <<<<<<<<<<<<<<
  *             if train.count(epoch) and train[epoch].loss.count(kf):
  *                 for its in train[epoch].loss[kf]: tmp_tr[its.first].push_back(its.second)
  */
-    __pyx_t_4 = PySet_New(__pyx_v_folds); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 284, __pyx_L1_error)
+    __pyx_t_4 = PySet_New(__pyx_v_folds); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 286, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_9 = PySequence_List(__pyx_t_4); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 284, __pyx_L1_error)
+    __pyx_t_9 = PySequence_List(__pyx_t_4); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 286, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_1 = ((PyObject*)__pyx_t_9);
     __pyx_t_9 = 0;
-    __pyx_t_6 = PyList_Sort(__pyx_t_1); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 284, __pyx_L1_error)
+    __pyx_t_6 = PyList_Sort(__pyx_t_1); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 286, __pyx_L1_error)
     __pyx_t_9 = __pyx_t_1; __Pyx_INCREF(__pyx_t_9);
     __pyx_t_10 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     for (;;) {
       {
         Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_9);
         #if !CYTHON_ASSUME_SAFE_MACROS
-        if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 284, __pyx_L1_error)
+        if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 286, __pyx_L1_error)
         #endif
         if (__pyx_t_10 >= __pyx_temp) break;
       }
       #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-      __pyx_t_1 = PyList_GET_ITEM(__pyx_t_9, __pyx_t_10); __Pyx_INCREF(__pyx_t_1); __pyx_t_10++; if (unlikely((0 < 0))) __PYX_ERR(0, 284, __pyx_L1_error)
+      __pyx_t_1 = PyList_GET_ITEM(__pyx_t_9, __pyx_t_10); __Pyx_INCREF(__pyx_t_1); __pyx_t_10++; if (unlikely((0 < 0))) __PYX_ERR(0, 286, __pyx_L1_error)
       #else
-      __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_9, __pyx_t_10); __pyx_t_10++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 284, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_9, __pyx_t_10); __pyx_t_10++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 286, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       #endif
-      __pyx_t_8 = __Pyx_PyInt_As_int(__pyx_t_1); if (unlikely((__pyx_t_8 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 284, __pyx_L1_error)
+      __pyx_t_8 = __Pyx_PyInt_As_int(__pyx_t_1); if (unlikely((__pyx_t_8 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 286, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_v_kf = __pyx_t_8;
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":285
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":287
  *     for epoch in sorted(set(epochs)):
  *         for kf in sorted(set(folds)):
  *             if train.count(epoch) and train[epoch].loss.count(kf):             # <<<<<<<<<<<<<<
  *                 for its in train[epoch].loss[kf]: tmp_tr[its.first].push_back(its.second)
  *             if valid.count(epoch) and valid[epoch].loss.count(kf):
  */
       __pyx_t_12 = (__pyx_v_train.count(__pyx_v_epoch) != 0);
@@ -30489,15 +30486,15 @@
         goto __pyx_L17_bool_binop_done;
       }
       __pyx_t_12 = ((__pyx_v_train[__pyx_v_epoch])->loss.count(__pyx_v_kf) != 0);
       __pyx_t_11 = __pyx_t_12;
       __pyx_L17_bool_binop_done:;
       if (__pyx_t_11) {
 
-        /* "src/cmodules/cyincludes/cyoptimizer.pyx":286
+        /* "src/cmodules/cyincludes/cyoptimizer.pyx":288
  *         for kf in sorted(set(folds)):
  *             if train.count(epoch) and train[epoch].loss.count(kf):
  *                 for its in train[epoch].loss[kf]: tmp_tr[its.first].push_back(its.second)             # <<<<<<<<<<<<<<
  *             if valid.count(epoch) and valid[epoch].loss.count(kf):
  *                 for its in valid[epoch].loss[kf]: tmp_va[its.first].push_back(its.second)
  */
         __pyx_t_14 = &((__pyx_v_train[__pyx_v_epoch])->loss[__pyx_v_kf]);
@@ -30507,28 +30504,28 @@
           __pyx_t_15 = *__pyx_t_13;
           ++__pyx_t_13;
           __pyx_v_its = __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_15);
           try {
             (__pyx_v_tmp_tr[__pyx_v_its.first]).push_back(__pyx_v_its.second);
           } catch(...) {
             __Pyx_CppExn2PyErr();
-            __PYX_ERR(0, 286, __pyx_L1_error)
+            __PYX_ERR(0, 288, __pyx_L1_error)
           }
         }
 
-        /* "src/cmodules/cyincludes/cyoptimizer.pyx":285
+        /* "src/cmodules/cyincludes/cyoptimizer.pyx":287
  *     for epoch in sorted(set(epochs)):
  *         for kf in sorted(set(folds)):
  *             if train.count(epoch) and train[epoch].loss.count(kf):             # <<<<<<<<<<<<<<
  *                 for its in train[epoch].loss[kf]: tmp_tr[its.first].push_back(its.second)
  *             if valid.count(epoch) and valid[epoch].loss.count(kf):
  */
       }
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":287
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":289
  *             if train.count(epoch) and train[epoch].loss.count(kf):
  *                 for its in train[epoch].loss[kf]: tmp_tr[its.first].push_back(its.second)
  *             if valid.count(epoch) and valid[epoch].loss.count(kf):             # <<<<<<<<<<<<<<
  *                 for its in valid[epoch].loss[kf]: tmp_va[its.first].push_back(its.second)
  *             if test.count(epoch) and test[epoch].loss.count(kf):
  */
       __pyx_t_12 = (__pyx_v_valid.count(__pyx_v_epoch) != 0);
@@ -30538,15 +30535,15 @@
         goto __pyx_L23_bool_binop_done;
       }
       __pyx_t_12 = ((__pyx_v_valid[__pyx_v_epoch])->loss.count(__pyx_v_kf) != 0);
       __pyx_t_11 = __pyx_t_12;
       __pyx_L23_bool_binop_done:;
       if (__pyx_t_11) {
 
-        /* "src/cmodules/cyincludes/cyoptimizer.pyx":288
+        /* "src/cmodules/cyincludes/cyoptimizer.pyx":290
  *                 for its in train[epoch].loss[kf]: tmp_tr[its.first].push_back(its.second)
  *             if valid.count(epoch) and valid[epoch].loss.count(kf):
  *                 for its in valid[epoch].loss[kf]: tmp_va[its.first].push_back(its.second)             # <<<<<<<<<<<<<<
  *             if test.count(epoch) and test[epoch].loss.count(kf):
  *                 for its in test[epoch].loss[kf]: tmp_te[its.first].push_back(its.second)
  */
         __pyx_t_14 = &((__pyx_v_valid[__pyx_v_epoch])->loss[__pyx_v_kf]);
@@ -30556,28 +30553,28 @@
           __pyx_t_15 = *__pyx_t_13;
           ++__pyx_t_13;
           __pyx_v_its = __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_15);
           try {
             (__pyx_v_tmp_va[__pyx_v_its.first]).push_back(__pyx_v_its.second);
           } catch(...) {
             __Pyx_CppExn2PyErr();
-            __PYX_ERR(0, 288, __pyx_L1_error)
+            __PYX_ERR(0, 290, __pyx_L1_error)
           }
         }
 
-        /* "src/cmodules/cyincludes/cyoptimizer.pyx":287
+        /* "src/cmodules/cyincludes/cyoptimizer.pyx":289
  *             if train.count(epoch) and train[epoch].loss.count(kf):
  *                 for its in train[epoch].loss[kf]: tmp_tr[its.first].push_back(its.second)
  *             if valid.count(epoch) and valid[epoch].loss.count(kf):             # <<<<<<<<<<<<<<
  *                 for its in valid[epoch].loss[kf]: tmp_va[its.first].push_back(its.second)
  *             if test.count(epoch) and test[epoch].loss.count(kf):
  */
       }
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":289
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":291
  *             if valid.count(epoch) and valid[epoch].loss.count(kf):
  *                 for its in valid[epoch].loss[kf]: tmp_va[its.first].push_back(its.second)
  *             if test.count(epoch) and test[epoch].loss.count(kf):             # <<<<<<<<<<<<<<
  *                 for its in test[epoch].loss[kf]: tmp_te[its.first].push_back(its.second)
  * 
  */
       __pyx_t_12 = (__pyx_v_test.count(__pyx_v_epoch) != 0);
@@ -30587,15 +30584,15 @@
         goto __pyx_L29_bool_binop_done;
       }
       __pyx_t_12 = ((__pyx_v_test[__pyx_v_epoch])->loss.count(__pyx_v_kf) != 0);
       __pyx_t_11 = __pyx_t_12;
       __pyx_L29_bool_binop_done:;
       if (__pyx_t_11) {
 
-        /* "src/cmodules/cyincludes/cyoptimizer.pyx":290
+        /* "src/cmodules/cyincludes/cyoptimizer.pyx":292
  *                 for its in valid[epoch].loss[kf]: tmp_va[its.first].push_back(its.second)
  *             if test.count(epoch) and test[epoch].loss.count(kf):
  *                 for its in test[epoch].loss[kf]: tmp_te[its.first].push_back(its.second)             # <<<<<<<<<<<<<<
  * 
  *         lines = collapse_points(&tmp_tr, epoch, lines, "training", state, "lss")
  */
         __pyx_t_14 = &((__pyx_v_test[__pyx_v_epoch])->loss[__pyx_v_kf]);
@@ -30605,262 +30602,262 @@
           __pyx_t_15 = *__pyx_t_13;
           ++__pyx_t_13;
           __pyx_v_its = __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_15);
           try {
             (__pyx_v_tmp_te[__pyx_v_its.first]).push_back(__pyx_v_its.second);
           } catch(...) {
             __Pyx_CppExn2PyErr();
-            __PYX_ERR(0, 290, __pyx_L1_error)
+            __PYX_ERR(0, 292, __pyx_L1_error)
           }
         }
 
-        /* "src/cmodules/cyincludes/cyoptimizer.pyx":289
+        /* "src/cmodules/cyincludes/cyoptimizer.pyx":291
  *             if valid.count(epoch) and valid[epoch].loss.count(kf):
  *                 for its in valid[epoch].loss[kf]: tmp_va[its.first].push_back(its.second)
  *             if test.count(epoch) and test[epoch].loss.count(kf):             # <<<<<<<<<<<<<<
  *                 for its in test[epoch].loss[kf]: tmp_te[its.first].push_back(its.second)
  * 
  */
       }
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":284
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":286
  *     cdef dict lines = {}
  *     for epoch in sorted(set(epochs)):
  *         for kf in sorted(set(folds)):             # <<<<<<<<<<<<<<
  *             if train.count(epoch) and train[epoch].loss.count(kf):
  *                 for its in train[epoch].loss[kf]: tmp_tr[its.first].push_back(its.second)
  */
     }
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":292
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":294
  *                 for its in test[epoch].loss[kf]: tmp_te[its.first].push_back(its.second)
  * 
  *         lines = collapse_points(&tmp_tr, epoch, lines, "training", state, "lss")             # <<<<<<<<<<<<<<
  *         lines = collapse_points(&tmp_va, epoch, lines, "validation", state, "lss")
  *         lines = collapse_points(&tmp_te, epoch, lines, "evaluation", state, "lss")
  */
-    __pyx_t_9 = __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_collapse_points((&__pyx_v_tmp_tr), __pyx_v_epoch, __pyx_v_lines, __pyx_n_u_training, __pyx_v_state, __pyx_n_u_lss); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 292, __pyx_L1_error)
+    __pyx_t_9 = __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_collapse_points((&__pyx_v_tmp_tr), __pyx_v_epoch, __pyx_v_lines, __pyx_n_u_training, __pyx_v_state, __pyx_n_u_lss); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 294, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     __Pyx_DECREF_SET(__pyx_v_lines, ((PyObject*)__pyx_t_9));
     __pyx_t_9 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":293
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":295
  * 
  *         lines = collapse_points(&tmp_tr, epoch, lines, "training", state, "lss")
  *         lines = collapse_points(&tmp_va, epoch, lines, "validation", state, "lss")             # <<<<<<<<<<<<<<
  *         lines = collapse_points(&tmp_te, epoch, lines, "evaluation", state, "lss")
  * 
  */
-    __pyx_t_9 = __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_collapse_points((&__pyx_v_tmp_va), __pyx_v_epoch, __pyx_v_lines, __pyx_n_u_validation, __pyx_v_state, __pyx_n_u_lss); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 293, __pyx_L1_error)
+    __pyx_t_9 = __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_collapse_points((&__pyx_v_tmp_va), __pyx_v_epoch, __pyx_v_lines, __pyx_n_u_validation, __pyx_v_state, __pyx_n_u_lss); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 295, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     __Pyx_DECREF_SET(__pyx_v_lines, ((PyObject*)__pyx_t_9));
     __pyx_t_9 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":294
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":296
  *         lines = collapse_points(&tmp_tr, epoch, lines, "training", state, "lss")
  *         lines = collapse_points(&tmp_va, epoch, lines, "validation", state, "lss")
  *         lines = collapse_points(&tmp_te, epoch, lines, "evaluation", state, "lss")             # <<<<<<<<<<<<<<
  * 
  *     for var_name in lines:
  */
-    __pyx_t_9 = __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_collapse_points((&__pyx_v_tmp_te), __pyx_v_epoch, __pyx_v_lines, __pyx_n_u_evaluation, __pyx_v_state, __pyx_n_u_lss); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 294, __pyx_L1_error)
+    __pyx_t_9 = __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_collapse_points((&__pyx_v_tmp_te), __pyx_v_epoch, __pyx_v_lines, __pyx_n_u_evaluation, __pyx_v_state, __pyx_n_u_lss); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 296, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     __Pyx_DECREF_SET(__pyx_v_lines, ((PyObject*)__pyx_t_9));
     __pyx_t_9 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":283
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":285
  *     cdef point_t pnt
  *     cdef dict lines = {}
  *     for epoch in sorted(set(epochs)):             # <<<<<<<<<<<<<<
  *         for kf in sorted(set(folds)):
  *             if train.count(epoch) and train[epoch].loss.count(kf):
  */
   }
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":296
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":298
  *         lines = collapse_points(&tmp_te, epoch, lines, "evaluation", state, "lss")
  * 
  *     for var_name in lines:             # <<<<<<<<<<<<<<
  *         for mode in lines[var_name]: lines[var_name][mode] = TLine(**lines[var_name][mode])
  *         tmpl = template_tline(path, "Epoch", "Loss (arb.)", "Loss Curve for " + var_name)
  */
   __pyx_t_7 = 0;
   if (unlikely(__pyx_v_lines == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-    __PYX_ERR(0, 296, __pyx_L1_error)
+    __PYX_ERR(0, 298, __pyx_L1_error)
   }
-  __pyx_t_9 = __Pyx_dict_iterator(__pyx_v_lines, 1, ((PyObject *)NULL), (&__pyx_t_10), (&__pyx_t_8)); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 296, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_dict_iterator(__pyx_v_lines, 1, ((PyObject *)NULL), (&__pyx_t_10), (&__pyx_t_8)); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 298, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __Pyx_XDECREF(__pyx_t_5);
   __pyx_t_5 = __pyx_t_9;
   __pyx_t_9 = 0;
   while (1) {
     __pyx_t_16 = __Pyx_dict_iter_next(__pyx_t_5, __pyx_t_10, &__pyx_t_7, &__pyx_t_9, NULL, NULL, __pyx_t_8);
     if (unlikely(__pyx_t_16 == 0)) break;
-    if (unlikely(__pyx_t_16 == -1)) __PYX_ERR(0, 296, __pyx_L1_error)
+    if (unlikely(__pyx_t_16 == -1)) __PYX_ERR(0, 298, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     __Pyx_XDECREF_SET(__pyx_v_var_name, __pyx_t_9);
     __pyx_t_9 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":297
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":299
  * 
  *     for var_name in lines:
  *         for mode in lines[var_name]: lines[var_name][mode] = TLine(**lines[var_name][mode])             # <<<<<<<<<<<<<<
  *         tmpl = template_tline(path, "Epoch", "Loss (arb.)", "Loss Curve for " + var_name)
  *         tmpl["Filename"] = var_name + "_loss"
  */
     if (unlikely(__pyx_v_lines == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 297, __pyx_L1_error)
+      __PYX_ERR(0, 299, __pyx_L1_error)
     }
-    __pyx_t_9 = __Pyx_PyDict_GetItem(__pyx_v_lines, __pyx_v_var_name); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 297, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyDict_GetItem(__pyx_v_lines, __pyx_v_var_name); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 299, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     if (likely(PyList_CheckExact(__pyx_t_9)) || PyTuple_CheckExact(__pyx_t_9)) {
       __pyx_t_1 = __pyx_t_9; __Pyx_INCREF(__pyx_t_1);
       __pyx_t_17 = 0;
       __pyx_t_18 = NULL;
     } else {
-      __pyx_t_17 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_t_9); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 297, __pyx_L1_error)
+      __pyx_t_17 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_t_9); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 299, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_18 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_1); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 297, __pyx_L1_error)
+      __pyx_t_18 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_1); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 299, __pyx_L1_error)
     }
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     for (;;) {
       if (likely(!__pyx_t_18)) {
         if (likely(PyList_CheckExact(__pyx_t_1))) {
           {
             Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_1);
             #if !CYTHON_ASSUME_SAFE_MACROS
-            if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 297, __pyx_L1_error)
+            if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 299, __pyx_L1_error)
             #endif
             if (__pyx_t_17 >= __pyx_temp) break;
           }
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_9 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_17); __Pyx_INCREF(__pyx_t_9); __pyx_t_17++; if (unlikely((0 < 0))) __PYX_ERR(0, 297, __pyx_L1_error)
+          __pyx_t_9 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_17); __Pyx_INCREF(__pyx_t_9); __pyx_t_17++; if (unlikely((0 < 0))) __PYX_ERR(0, 299, __pyx_L1_error)
           #else
-          __pyx_t_9 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_17); __pyx_t_17++; if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 297, __pyx_L1_error)
+          __pyx_t_9 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_17); __pyx_t_17++; if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 299, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_9);
           #endif
         } else {
           {
             Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_1);
             #if !CYTHON_ASSUME_SAFE_MACROS
-            if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 297, __pyx_L1_error)
+            if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 299, __pyx_L1_error)
             #endif
             if (__pyx_t_17 >= __pyx_temp) break;
           }
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_9 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_17); __Pyx_INCREF(__pyx_t_9); __pyx_t_17++; if (unlikely((0 < 0))) __PYX_ERR(0, 297, __pyx_L1_error)
+          __pyx_t_9 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_17); __Pyx_INCREF(__pyx_t_9); __pyx_t_17++; if (unlikely((0 < 0))) __PYX_ERR(0, 299, __pyx_L1_error)
           #else
-          __pyx_t_9 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_17); __pyx_t_17++; if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 297, __pyx_L1_error)
+          __pyx_t_9 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_17); __pyx_t_17++; if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 299, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_9);
           #endif
         }
       } else {
         __pyx_t_9 = __pyx_t_18(__pyx_t_1);
         if (unlikely(!__pyx_t_9)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 297, __pyx_L1_error)
+            else __PYX_ERR(0, 299, __pyx_L1_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_9);
       }
       __Pyx_XDECREF_SET(__pyx_v_mode, __pyx_t_9);
       __pyx_t_9 = 0;
-      __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_TLine); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 297, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_TLine); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 299, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
       if (unlikely(__pyx_v_lines == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-        __PYX_ERR(0, 297, __pyx_L1_error)
+        __PYX_ERR(0, 299, __pyx_L1_error)
       }
-      __pyx_t_19 = __Pyx_PyDict_GetItem(__pyx_v_lines, __pyx_v_var_name); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 297, __pyx_L1_error)
+      __pyx_t_19 = __Pyx_PyDict_GetItem(__pyx_v_lines, __pyx_v_var_name); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 299, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_19);
-      __pyx_t_20 = __Pyx_PyObject_GetItem(__pyx_t_19, __pyx_v_mode); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 297, __pyx_L1_error)
+      __pyx_t_20 = __Pyx_PyObject_GetItem(__pyx_t_19, __pyx_v_mode); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 299, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_20);
       __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
       if (unlikely(__pyx_t_20 == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "argument after ** must be a mapping, not NoneType");
-        __PYX_ERR(0, 297, __pyx_L1_error)
+        __PYX_ERR(0, 299, __pyx_L1_error)
       }
       if (likely(PyDict_CheckExact(__pyx_t_20))) {
-        __pyx_t_4 = PyDict_Copy(__pyx_t_20); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 297, __pyx_L1_error)
+        __pyx_t_4 = PyDict_Copy(__pyx_t_20); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 299, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
       } else {
-        __pyx_t_4 = __Pyx_PyObject_CallOneArg((PyObject*)&PyDict_Type, __pyx_t_20); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 297, __pyx_L1_error)
+        __pyx_t_4 = __Pyx_PyObject_CallOneArg((PyObject*)&PyDict_Type, __pyx_t_20); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 299, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
       }
-      __pyx_t_20 = __Pyx_PyObject_Call(__pyx_t_9, __pyx_empty_tuple, __pyx_t_4); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 297, __pyx_L1_error)
+      __pyx_t_20 = __Pyx_PyObject_Call(__pyx_t_9, __pyx_empty_tuple, __pyx_t_4); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 299, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_20);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       if (unlikely(__pyx_v_lines == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-        __PYX_ERR(0, 297, __pyx_L1_error)
+        __PYX_ERR(0, 299, __pyx_L1_error)
       }
-      __pyx_t_4 = __Pyx_PyDict_GetItem(__pyx_v_lines, __pyx_v_var_name); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 297, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyDict_GetItem(__pyx_v_lines, __pyx_v_var_name); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 299, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      if (unlikely((PyObject_SetItem(__pyx_t_4, __pyx_v_mode, __pyx_t_20) < 0))) __PYX_ERR(0, 297, __pyx_L1_error)
+      if (unlikely((PyObject_SetItem(__pyx_t_4, __pyx_v_mode, __pyx_t_20) < 0))) __PYX_ERR(0, 299, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
     }
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":298
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":300
  *     for var_name in lines:
  *         for mode in lines[var_name]: lines[var_name][mode] = TLine(**lines[var_name][mode])
  *         tmpl = template_tline(path, "Epoch", "Loss (arb.)", "Loss Curve for " + var_name)             # <<<<<<<<<<<<<<
  *         tmpl["Filename"] = var_name + "_loss"
  *         tmpl["Lines"] = list(lines[var_name].values())
  */
-    __pyx_t_1 = PyNumber_Add(__pyx_kp_u_Loss_Curve_for, __pyx_v_var_name); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 298, __pyx_L1_error)
+    __pyx_t_1 = PyNumber_Add(__pyx_kp_u_Loss_Curve_for, __pyx_v_var_name); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 300, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_t_1))) __PYX_ERR(0, 298, __pyx_L1_error)
-    __pyx_t_20 = __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_template_tline(__pyx_v_path, __pyx_n_u_Epoch_2, __pyx_kp_u_Loss_arb, ((PyObject*)__pyx_t_1)); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 298, __pyx_L1_error)
+    if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_t_1))) __PYX_ERR(0, 300, __pyx_L1_error)
+    __pyx_t_20 = __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_template_tline(__pyx_v_path, __pyx_n_u_Epoch_2, __pyx_kp_u_Loss_arb, ((PyObject*)__pyx_t_1)); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 300, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_20);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_v_tmpl = ((PyObject*)__pyx_t_20);
     __pyx_t_20 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":299
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":301
  *         for mode in lines[var_name]: lines[var_name][mode] = TLine(**lines[var_name][mode])
  *         tmpl = template_tline(path, "Epoch", "Loss (arb.)", "Loss Curve for " + var_name)
  *         tmpl["Filename"] = var_name + "_loss"             # <<<<<<<<<<<<<<
  *         tmpl["Lines"] = list(lines[var_name].values())
  *         tl = TLine(**tmpl)
  */
-    __pyx_t_20 = PyNumber_Add(__pyx_v_var_name, __pyx_n_u_loss_3); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 299, __pyx_L1_error)
+    __pyx_t_20 = PyNumber_Add(__pyx_v_var_name, __pyx_n_u_loss_3); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 301, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_20);
     if (unlikely(__pyx_v_tmpl == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 299, __pyx_L1_error)
+      __PYX_ERR(0, 301, __pyx_L1_error)
     }
-    if (unlikely((PyDict_SetItem(__pyx_v_tmpl, __pyx_n_u_Filename, __pyx_t_20) < 0))) __PYX_ERR(0, 299, __pyx_L1_error)
+    if (unlikely((PyDict_SetItem(__pyx_v_tmpl, __pyx_n_u_Filename, __pyx_t_20) < 0))) __PYX_ERR(0, 301, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":300
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":302
  *         tmpl = template_tline(path, "Epoch", "Loss (arb.)", "Loss Curve for " + var_name)
  *         tmpl["Filename"] = var_name + "_loss"
  *         tmpl["Lines"] = list(lines[var_name].values())             # <<<<<<<<<<<<<<
  *         tl = TLine(**tmpl)
  *         tl.SaveFigure()
  */
     if (unlikely(__pyx_v_lines == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 300, __pyx_L1_error)
+      __PYX_ERR(0, 302, __pyx_L1_error)
     }
-    __pyx_t_1 = __Pyx_PyDict_GetItem(__pyx_v_lines, __pyx_v_var_name); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 300, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyDict_GetItem(__pyx_v_lines, __pyx_v_var_name); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 302, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_values); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 300, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_values); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 302, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_1 = NULL;
     __pyx_t_16 = 0;
     #if CYTHON_UNPACK_METHODS
     if (likely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_4);
@@ -30873,58 +30870,58 @@
       }
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_1, NULL};
       __pyx_t_20 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_16, 0+__pyx_t_16);
       __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-      if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 300, __pyx_L1_error)
+      if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 302, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_20);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     }
-    __pyx_t_4 = __Pyx_PySequence_ListKeepNew(__pyx_t_20); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 300, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PySequence_ListKeepNew(__pyx_t_20); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 302, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
     if (unlikely(__pyx_v_tmpl == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 300, __pyx_L1_error)
+      __PYX_ERR(0, 302, __pyx_L1_error)
     }
-    if (unlikely((PyDict_SetItem(__pyx_v_tmpl, __pyx_n_u_Lines, __pyx_t_4) < 0))) __PYX_ERR(0, 300, __pyx_L1_error)
+    if (unlikely((PyDict_SetItem(__pyx_v_tmpl, __pyx_n_u_Lines, __pyx_t_4) < 0))) __PYX_ERR(0, 302, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":301
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":303
  *         tmpl["Filename"] = var_name + "_loss"
  *         tmpl["Lines"] = list(lines[var_name].values())
  *         tl = TLine(**tmpl)             # <<<<<<<<<<<<<<
  *         tl.SaveFigure()
  *         del tl
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_TLine); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 301, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_TLine); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 303, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     if (unlikely(__pyx_v_tmpl == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "argument after ** must be a mapping, not NoneType");
-      __PYX_ERR(0, 301, __pyx_L1_error)
+      __PYX_ERR(0, 303, __pyx_L1_error)
     }
-    __pyx_t_20 = PyDict_Copy(__pyx_v_tmpl); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 301, __pyx_L1_error)
+    __pyx_t_20 = PyDict_Copy(__pyx_v_tmpl); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 303, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_20);
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_empty_tuple, __pyx_t_20); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 301, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_empty_tuple, __pyx_t_20); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 303, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
     __pyx_v_tl = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":302
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":304
  *         tmpl["Lines"] = list(lines[var_name].values())
  *         tl = TLine(**tmpl)
  *         tl.SaveFigure()             # <<<<<<<<<<<<<<
  *         del tl
  *         del tmpl
  */
-    __pyx_t_20 = __Pyx_PyObject_GetAttrStr(__pyx_v_tl, __pyx_n_s_SaveFigure); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 302, __pyx_L1_error)
+    __pyx_t_20 = __Pyx_PyObject_GetAttrStr(__pyx_v_tl, __pyx_n_s_SaveFigure); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 304, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_20);
     __pyx_t_4 = NULL;
     __pyx_t_16 = 0;
     #if CYTHON_UNPACK_METHODS
     if (likely(PyMethod_Check(__pyx_t_20))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_20);
       if (likely(__pyx_t_4)) {
@@ -30936,95 +30933,95 @@
       }
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_4, NULL};
       __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_20, __pyx_callargs+1-__pyx_t_16, 0+__pyx_t_16);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 302, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 304, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
     }
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":303
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":305
  *         tl = TLine(**tmpl)
  *         tl.SaveFigure()
  *         del tl             # <<<<<<<<<<<<<<
  *         del tmpl
  * 
  */
     __Pyx_DECREF(__pyx_v_tl); __pyx_v_tl = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":304
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":306
  *         tl.SaveFigure()
  *         del tl
  *         del tmpl             # <<<<<<<<<<<<<<
  * 
  *     del lines
  */
     __Pyx_DECREF(__pyx_v_tmpl); __pyx_v_tmpl = 0;
   }
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":306
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":308
  *         del tmpl
  * 
  *     del lines             # <<<<<<<<<<<<<<
  *     del folds
  *     del epochs
  */
   __Pyx_DECREF(__pyx_v_lines); __pyx_v_lines = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":307
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":309
  * 
  *     del lines
  *     del folds             # <<<<<<<<<<<<<<
  *     del epochs
  *     tmp_tr.clear()
  */
   __Pyx_DECREF(__pyx_v_folds); __pyx_v_folds = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":308
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":310
  *     del lines
  *     del folds
  *     del epochs             # <<<<<<<<<<<<<<
  *     tmp_tr.clear()
  *     tmp_va.clear()
  */
   __Pyx_DECREF(__pyx_v_epochs); __pyx_v_epochs = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":309
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":311
  *     del folds
  *     del epochs
  *     tmp_tr.clear()             # <<<<<<<<<<<<<<
  *     tmp_va.clear()
  *     tmp_te.clear()
  */
   __pyx_v_tmp_tr.clear();
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":310
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":312
  *     del epochs
  *     tmp_tr.clear()
  *     tmp_va.clear()             # <<<<<<<<<<<<<<
  *     tmp_te.clear()
  * 
  */
   __pyx_v_tmp_va.clear();
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":311
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":313
  *     tmp_tr.clear()
  *     tmp_va.clear()
  *     tmp_te.clear()             # <<<<<<<<<<<<<<
  * 
  * cdef dict make_roc_curve(map[string, roc_t]* roc_, dict lines, str mode):
  */
   __pyx_v_tmp_te.clear();
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":256
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":258
  *     tmp_te.clear()
  * 
  * cdef void make_loss_plots(map[int, CyEpoch*] train, map[int, CyEpoch*] valid, map[int, CyEpoch*] test, str path, report_t* state):             # <<<<<<<<<<<<<<
  *     cdef pair[int, CyEpoch*] itr
  *     cdef pair[string, point_t] its
  */
 
@@ -31045,15 +31042,15 @@
   __Pyx_XDECREF(__pyx_v_var_name);
   __Pyx_XDECREF(__pyx_v_mode);
   __Pyx_XDECREF(__pyx_v_tmpl);
   __Pyx_XDECREF(__pyx_v_tl);
   __Pyx_RefNannyFinishContext();
 }
 
-/* "src/cmodules/cyincludes/cyoptimizer.pyx":313
+/* "src/cmodules/cyincludes/cyoptimizer.pyx":315
  *     tmp_te.clear()
  * 
  * cdef dict make_roc_curve(map[string, roc_t]* roc_, dict lines, str mode):             # <<<<<<<<<<<<<<
  *     cdef pair[string, roc_t] its
  * 
  */
 
@@ -31070,808 +31067,829 @@
   PyObject *__pyx_v_cls = NULL;
   PyObject *__pyx_v_name = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   std::map<std::string,struct roc_t> ::iterator __pyx_t_1;
   std::map<std::string,struct roc_t>  *__pyx_t_2;
   std::pair<std::string,struct roc_t>  __pyx_t_3;
-  PyObject *__pyx_t_4 = NULL;
+  int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
-  int __pyx_t_8;
-  PyObject *__pyx_t_9 = NULL;
+  PyObject *__pyx_t_8 = NULL;
+  int __pyx_t_9;
   PyObject *__pyx_t_10 = NULL;
-  PyObject *(*__pyx_t_11)(PyObject *);
-  Py_ssize_t __pyx_t_12;
-  PyObject *(*__pyx_t_13)(PyObject *);
-  PyObject *__pyx_t_14 = NULL;
+  PyObject *__pyx_t_11 = NULL;
+  PyObject *(*__pyx_t_12)(PyObject *);
+  Py_ssize_t __pyx_t_13;
+  PyObject *(*__pyx_t_14)(PyObject *);
   PyObject *__pyx_t_15 = NULL;
   PyObject *__pyx_t_16 = NULL;
-  float __pyx_t_17;
-  int __pyx_t_18;
+  PyObject *__pyx_t_17 = NULL;
+  float __pyx_t_18;
   PyObject *__pyx_t_19 = NULL;
   PyObject *__pyx_t_20 = NULL;
   PyObject *__pyx_t_21 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("make_roc_curve", 1);
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":316
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":318
  *     cdef pair[string, roc_t] its
  * 
  *     for its in dereference(roc_):             # <<<<<<<<<<<<<<
+ *         if not its.second.pred.size(): continue
  *         pred = torch.tensor(its.second.pred)
- *         dereference(roc_)[its.first].pred.clear()
  */
   __pyx_t_2 = &(*__pyx_v_roc_);
   __pyx_t_1 = __pyx_t_2->begin();
   for (;;) {
     if (!(__pyx_t_1 != __pyx_t_2->end())) break;
     __pyx_t_3 = *__pyx_t_1;
     ++__pyx_t_1;
     __pyx_v_its = __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_3);
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":317
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":319
  * 
  *     for its in dereference(roc_):
+ *         if not its.second.pred.size(): continue             # <<<<<<<<<<<<<<
+ *         pred = torch.tensor(its.second.pred)
+ *         dereference(roc_)[its.first].pred.clear()
+ */
+    __pyx_t_4 = (!(__pyx_v_its.second.pred.size() != 0));
+    if (__pyx_t_4) {
+      goto __pyx_L3_continue;
+    }
+
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":320
+ *     for its in dereference(roc_):
+ *         if not its.second.pred.size(): continue
  *         pred = torch.tensor(its.second.pred)             # <<<<<<<<<<<<<<
  *         dereference(roc_)[its.first].pred.clear()
  * 
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_torch); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 317, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_tensor); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 317, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_torch); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 320, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_5 = __pyx_convert_vector_to_py_std_3a__3a_vector_3c_float_3e___(__pyx_v_its.second.pred); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 317, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_7 = NULL;
-    __pyx_t_8 = 0;
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_tensor); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 320, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __pyx_t_6 = __pyx_convert_vector_to_py_std_3a__3a_vector_3c_float_3e___(__pyx_v_its.second.pred); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 320, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __pyx_t_8 = NULL;
+    __pyx_t_9 = 0;
     #if CYTHON_UNPACK_METHODS
-    if (unlikely(PyMethod_Check(__pyx_t_6))) {
-      __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
-      if (likely(__pyx_t_7)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
-        __Pyx_INCREF(__pyx_t_7);
+    if (unlikely(PyMethod_Check(__pyx_t_7))) {
+      __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_7);
+      if (likely(__pyx_t_8)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
+        __Pyx_INCREF(__pyx_t_8);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_6, function);
-        __pyx_t_8 = 1;
+        __Pyx_DECREF_SET(__pyx_t_7, function);
+        __pyx_t_9 = 1;
       }
     }
     #endif
     {
-      PyObject *__pyx_callargs[2] = {__pyx_t_7, __pyx_t_5};
-      __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
-      __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 317, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
+      PyObject *__pyx_callargs[2] = {__pyx_t_8, __pyx_t_6};
+      __pyx_t_5 = __Pyx_PyObject_FastCall(__pyx_t_7, __pyx_callargs+1-__pyx_t_9, 1+__pyx_t_9);
+      __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 320, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     }
-    __pyx_v_pred = __pyx_t_4;
-    __pyx_t_4 = 0;
+    __pyx_v_pred = __pyx_t_5;
+    __pyx_t_5 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":318
- *     for its in dereference(roc_):
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":321
+ *         if not its.second.pred.size(): continue
  *         pred = torch.tensor(its.second.pred)
  *         dereference(roc_)[its.first].pred.clear()             # <<<<<<<<<<<<<<
  * 
  *         tru = torch.tensor(its.second.truth, dtype = torch.long).view(-1)
  */
     ((*__pyx_v_roc_)[__pyx_v_its.first]).pred.clear();
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":320
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":323
  *         dereference(roc_)[its.first].pred.clear()
  * 
  *         tru = torch.tensor(its.second.truth, dtype = torch.long).view(-1)             # <<<<<<<<<<<<<<
  *         dereference(roc_)[its.first].truth.clear()
  * 
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_torch); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 320, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_tensor); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 320, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_6 = __pyx_convert_vector_to_py_std_3a__3a_vector_3c_float_3e___(__pyx_v_its.second.truth); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 320, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_7 = PyTuple_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 320, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_torch); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 323, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __Pyx_GIVEREF(__pyx_t_6);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_6)) __PYX_ERR(0, 320, __pyx_L1_error);
-    __pyx_t_6 = 0;
-    __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 320, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_tensor); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 323, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_torch); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 320, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_9);
-    __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_long); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 320, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __pyx_t_7 = __pyx_convert_vector_to_py_std_3a__3a_vector_3c_float_3e___(__pyx_v_its.second.truth); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 323, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __pyx_t_8 = PyTuple_New(1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 323, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_8);
+    __Pyx_GIVEREF(__pyx_t_7);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_7)) __PYX_ERR(0, 323, __pyx_L1_error);
+    __pyx_t_7 = 0;
+    __pyx_t_7 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 323, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_torch); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 323, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
-    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-    if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_t_10) < 0) __PYX_ERR(0, 320, __pyx_L1_error)
+    __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_long); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 323, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_11);
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-    __pyx_t_10 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_7, __pyx_t_6); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 320, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_10);
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_dtype, __pyx_t_11) < 0) __PYX_ERR(0, 323, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+    __pyx_t_11 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_8, __pyx_t_7); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 323, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_11);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_view); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 320, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-    __pyx_t_10 = NULL;
-    __pyx_t_8 = 0;
+    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_view); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 323, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+    __pyx_t_11 = NULL;
+    __pyx_t_9 = 0;
     #if CYTHON_UNPACK_METHODS
-    if (likely(PyMethod_Check(__pyx_t_6))) {
-      __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_6);
-      if (likely(__pyx_t_10)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
-        __Pyx_INCREF(__pyx_t_10);
+    if (likely(PyMethod_Check(__pyx_t_7))) {
+      __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_7);
+      if (likely(__pyx_t_11)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
+        __Pyx_INCREF(__pyx_t_11);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_6, function);
-        __pyx_t_8 = 1;
+        __Pyx_DECREF_SET(__pyx_t_7, function);
+        __pyx_t_9 = 1;
       }
     }
     #endif
     {
-      PyObject *__pyx_callargs[2] = {__pyx_t_10, __pyx_int_neg_1};
-      __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
-      __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
-      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 320, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      PyObject *__pyx_callargs[2] = {__pyx_t_11, __pyx_int_neg_1};
+      __pyx_t_5 = __Pyx_PyObject_FastCall(__pyx_t_7, __pyx_callargs+1-__pyx_t_9, 1+__pyx_t_9);
+      __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
+      if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 323, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     }
-    __pyx_v_tru = __pyx_t_4;
-    __pyx_t_4 = 0;
+    __pyx_v_tru = __pyx_t_5;
+    __pyx_t_5 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":321
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":324
  * 
  *         tru = torch.tensor(its.second.truth, dtype = torch.long).view(-1)
  *         dereference(roc_)[its.first].truth.clear()             # <<<<<<<<<<<<<<
  * 
  *         roc = MulticlassROC(**{"num_classes": pred.size()[1], "thresholds" : None})
  */
     ((*__pyx_v_roc_)[__pyx_v_its.first]).truth.clear();
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":323
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":326
  *         dereference(roc_)[its.first].truth.clear()
  * 
  *         roc = MulticlassROC(**{"num_classes": pred.size()[1], "thresholds" : None})             # <<<<<<<<<<<<<<
  *         fpr, tpr, thres = roc(pred, tru)
  * 
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_MulticlassROC); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 323, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_6 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 323, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_pred, __pyx_n_s_size); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 323, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_MulticlassROC); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 326, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_t_7 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 326, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_5 = NULL;
-    __pyx_t_8 = 0;
+    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_pred, __pyx_n_s_size); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 326, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_8);
+    __pyx_t_6 = NULL;
+    __pyx_t_9 = 0;
     #if CYTHON_UNPACK_METHODS
-    if (likely(PyMethod_Check(__pyx_t_7))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_7);
-      if (likely(__pyx_t_5)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
-        __Pyx_INCREF(__pyx_t_5);
+    if (likely(PyMethod_Check(__pyx_t_8))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_8);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
+        __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_7, function);
-        __pyx_t_8 = 1;
+        __Pyx_DECREF_SET(__pyx_t_8, function);
+        __pyx_t_9 = 1;
       }
     }
     #endif
     {
-      PyObject *__pyx_callargs[2] = {__pyx_t_5, NULL};
-      __pyx_t_10 = __Pyx_PyObject_FastCall(__pyx_t_7, __pyx_callargs+1-__pyx_t_8, 0+__pyx_t_8);
-      __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-      if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 323, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_10);
-      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+      PyObject *__pyx_callargs[2] = {__pyx_t_6, NULL};
+      __pyx_t_11 = __Pyx_PyObject_FastCall(__pyx_t_8, __pyx_callargs+1-__pyx_t_9, 0+__pyx_t_9);
+      __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+      if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 326, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_11);
+      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     }
-    __pyx_t_7 = __Pyx_GetItemInt(__pyx_t_10, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 323, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-    if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_num_classes, __pyx_t_7) < 0) __PYX_ERR(0, 323, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_GetItemInt(__pyx_t_11, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 326, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_8);
+    __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+    if (PyDict_SetItem(__pyx_t_7, __pyx_n_u_num_classes, __pyx_t_8) < 0) __PYX_ERR(0, 326, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+    if (PyDict_SetItem(__pyx_t_7, __pyx_n_u_thresholds, Py_None) < 0) __PYX_ERR(0, 326, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_empty_tuple, __pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 326, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_8);
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_thresholds, Py_None) < 0) __PYX_ERR(0, 323, __pyx_L1_error)
-    __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_empty_tuple, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 323, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __Pyx_XDECREF_SET(__pyx_v_roc, __pyx_t_7);
-    __pyx_t_7 = 0;
+    __Pyx_XDECREF_SET(__pyx_v_roc, __pyx_t_8);
+    __pyx_t_8 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":324
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":327
  * 
  *         roc = MulticlassROC(**{"num_classes": pred.size()[1], "thresholds" : None})
  *         fpr, tpr, thres = roc(pred, tru)             # <<<<<<<<<<<<<<
  * 
  *         auc = MulticlassAUROC(**{"num_classes": pred.size()[1], "thresholds" : None, "average" : None})
  */
     __Pyx_INCREF(__pyx_v_roc);
-    __pyx_t_6 = __pyx_v_roc; __pyx_t_4 = NULL;
-    __pyx_t_8 = 0;
+    __pyx_t_7 = __pyx_v_roc; __pyx_t_5 = NULL;
+    __pyx_t_9 = 0;
     #if CYTHON_UNPACK_METHODS
-    if (unlikely(PyMethod_Check(__pyx_t_6))) {
-      __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_6);
-      if (likely(__pyx_t_4)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
-        __Pyx_INCREF(__pyx_t_4);
+    if (unlikely(PyMethod_Check(__pyx_t_7))) {
+      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_7);
+      if (likely(__pyx_t_5)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
+        __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_6, function);
-        __pyx_t_8 = 1;
+        __Pyx_DECREF_SET(__pyx_t_7, function);
+        __pyx_t_9 = 1;
       }
     }
     #endif
     {
-      PyObject *__pyx_callargs[3] = {__pyx_t_4, __pyx_v_pred, __pyx_v_tru};
-      __pyx_t_7 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_8, 2+__pyx_t_8);
-      __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 324, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_7);
-      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      PyObject *__pyx_callargs[3] = {__pyx_t_5, __pyx_v_pred, __pyx_v_tru};
+      __pyx_t_8 = __Pyx_PyObject_FastCall(__pyx_t_7, __pyx_callargs+1-__pyx_t_9, 2+__pyx_t_9);
+      __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+      if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 327, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_8);
+      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     }
-    if ((likely(PyTuple_CheckExact(__pyx_t_7))) || (PyList_CheckExact(__pyx_t_7))) {
-      PyObject* sequence = __pyx_t_7;
+    if ((likely(PyTuple_CheckExact(__pyx_t_8))) || (PyList_CheckExact(__pyx_t_8))) {
+      PyObject* sequence = __pyx_t_8;
       Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
       if (unlikely(size != 3)) {
         if (size > 3) __Pyx_RaiseTooManyValuesError(3);
         else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-        __PYX_ERR(0, 324, __pyx_L1_error)
+        __PYX_ERR(0, 327, __pyx_L1_error)
       }
       #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
       if (likely(PyTuple_CheckExact(sequence))) {
-        __pyx_t_6 = PyTuple_GET_ITEM(sequence, 0); 
-        __pyx_t_4 = PyTuple_GET_ITEM(sequence, 1); 
-        __pyx_t_10 = PyTuple_GET_ITEM(sequence, 2); 
+        __pyx_t_7 = PyTuple_GET_ITEM(sequence, 0); 
+        __pyx_t_5 = PyTuple_GET_ITEM(sequence, 1); 
+        __pyx_t_11 = PyTuple_GET_ITEM(sequence, 2); 
       } else {
-        __pyx_t_6 = PyList_GET_ITEM(sequence, 0); 
-        __pyx_t_4 = PyList_GET_ITEM(sequence, 1); 
-        __pyx_t_10 = PyList_GET_ITEM(sequence, 2); 
+        __pyx_t_7 = PyList_GET_ITEM(sequence, 0); 
+        __pyx_t_5 = PyList_GET_ITEM(sequence, 1); 
+        __pyx_t_11 = PyList_GET_ITEM(sequence, 2); 
       }
-      __Pyx_INCREF(__pyx_t_6);
-      __Pyx_INCREF(__pyx_t_4);
-      __Pyx_INCREF(__pyx_t_10);
+      __Pyx_INCREF(__pyx_t_7);
+      __Pyx_INCREF(__pyx_t_5);
+      __Pyx_INCREF(__pyx_t_11);
       #else
-      __pyx_t_6 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 324, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_4 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 324, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_10 = PySequence_ITEM(sequence, 2); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 324, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_10);
+      __pyx_t_7 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 327, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_7);
+      __pyx_t_5 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 327, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __pyx_t_11 = PySequence_ITEM(sequence, 2); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 327, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_11);
       #endif
-      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     } else {
       Py_ssize_t index = -1;
-      __pyx_t_5 = PyObject_GetIter(__pyx_t_7); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 324, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_5);
-      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      __pyx_t_11 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_5);
-      index = 0; __pyx_t_6 = __pyx_t_11(__pyx_t_5); if (unlikely(!__pyx_t_6)) goto __pyx_L5_unpacking_failed;
+      __pyx_t_6 = PyObject_GetIter(__pyx_t_8); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 327, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      index = 1; __pyx_t_4 = __pyx_t_11(__pyx_t_5); if (unlikely(!__pyx_t_4)) goto __pyx_L5_unpacking_failed;
-      __Pyx_GOTREF(__pyx_t_4);
-      index = 2; __pyx_t_10 = __pyx_t_11(__pyx_t_5); if (unlikely(!__pyx_t_10)) goto __pyx_L5_unpacking_failed;
-      __Pyx_GOTREF(__pyx_t_10);
-      if (__Pyx_IternextUnpackEndCheck(__pyx_t_11(__pyx_t_5), 3) < 0) __PYX_ERR(0, 324, __pyx_L1_error)
-      __pyx_t_11 = NULL;
-      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      goto __pyx_L6_unpacking_done;
-      __pyx_L5_unpacking_failed:;
-      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __pyx_t_11 = NULL;
+      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+      __pyx_t_12 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_6);
+      index = 0; __pyx_t_7 = __pyx_t_12(__pyx_t_6); if (unlikely(!__pyx_t_7)) goto __pyx_L6_unpacking_failed;
+      __Pyx_GOTREF(__pyx_t_7);
+      index = 1; __pyx_t_5 = __pyx_t_12(__pyx_t_6); if (unlikely(!__pyx_t_5)) goto __pyx_L6_unpacking_failed;
+      __Pyx_GOTREF(__pyx_t_5);
+      index = 2; __pyx_t_11 = __pyx_t_12(__pyx_t_6); if (unlikely(!__pyx_t_11)) goto __pyx_L6_unpacking_failed;
+      __Pyx_GOTREF(__pyx_t_11);
+      if (__Pyx_IternextUnpackEndCheck(__pyx_t_12(__pyx_t_6), 3) < 0) __PYX_ERR(0, 327, __pyx_L1_error)
+      __pyx_t_12 = NULL;
+      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      goto __pyx_L7_unpacking_done;
+      __pyx_L6_unpacking_failed:;
+      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      __pyx_t_12 = NULL;
       if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-      __PYX_ERR(0, 324, __pyx_L1_error)
-      __pyx_L6_unpacking_done:;
+      __PYX_ERR(0, 327, __pyx_L1_error)
+      __pyx_L7_unpacking_done:;
     }
-    __Pyx_XDECREF_SET(__pyx_v_fpr, __pyx_t_6);
-    __pyx_t_6 = 0;
-    __Pyx_XDECREF_SET(__pyx_v_tpr, __pyx_t_4);
-    __pyx_t_4 = 0;
-    __pyx_v_thres = __pyx_t_10;
-    __pyx_t_10 = 0;
+    __Pyx_XDECREF_SET(__pyx_v_fpr, __pyx_t_7);
+    __pyx_t_7 = 0;
+    __Pyx_XDECREF_SET(__pyx_v_tpr, __pyx_t_5);
+    __pyx_t_5 = 0;
+    __pyx_v_thres = __pyx_t_11;
+    __pyx_t_11 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":326
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":329
  *         fpr, tpr, thres = roc(pred, tru)
  * 
  *         auc = MulticlassAUROC(**{"num_classes": pred.size()[1], "thresholds" : None, "average" : None})             # <<<<<<<<<<<<<<
  *         auc_ = auc(pred, tru).view(-1)
  * 
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_MulticlassAUROC); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 326, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_MulticlassAUROC); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 329, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_8);
+    __pyx_t_11 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 329, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_11);
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_pred, __pyx_n_s_size); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 329, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_10 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 326, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_10);
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_pred, __pyx_n_s_size); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 326, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_5 = NULL;
-    __pyx_t_8 = 0;
+    __pyx_t_6 = NULL;
+    __pyx_t_9 = 0;
     #if CYTHON_UNPACK_METHODS
-    if (likely(PyMethod_Check(__pyx_t_6))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_6);
-      if (likely(__pyx_t_5)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
-        __Pyx_INCREF(__pyx_t_5);
+    if (likely(PyMethod_Check(__pyx_t_7))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_7);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
+        __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_6, function);
-        __pyx_t_8 = 1;
+        __Pyx_DECREF_SET(__pyx_t_7, function);
+        __pyx_t_9 = 1;
       }
     }
     #endif
     {
-      PyObject *__pyx_callargs[2] = {__pyx_t_5, NULL};
-      __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_8, 0+__pyx_t_8);
-      __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 326, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      PyObject *__pyx_callargs[2] = {__pyx_t_6, NULL};
+      __pyx_t_5 = __Pyx_PyObject_FastCall(__pyx_t_7, __pyx_callargs+1-__pyx_t_9, 0+__pyx_t_9);
+      __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+      if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 329, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     }
-    __pyx_t_6 = __Pyx_GetItemInt(__pyx_t_4, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 326, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_num_classes, __pyx_t_6) < 0) __PYX_ERR(0, 326, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_thresholds, Py_None) < 0) __PYX_ERR(0, 326, __pyx_L1_error)
-    if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_average, Py_None) < 0) __PYX_ERR(0, 326, __pyx_L1_error)
-    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_empty_tuple, __pyx_t_10); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 326, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
+    __pyx_t_7 = __Pyx_GetItemInt(__pyx_t_5, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 329, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (PyDict_SetItem(__pyx_t_11, __pyx_n_u_num_classes, __pyx_t_7) < 0) __PYX_ERR(0, 329, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-    __Pyx_XDECREF_SET(__pyx_v_auc, __pyx_t_6);
-    __pyx_t_6 = 0;
+    if (PyDict_SetItem(__pyx_t_11, __pyx_n_u_thresholds, Py_None) < 0) __PYX_ERR(0, 329, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_11, __pyx_n_u_average, Py_None) < 0) __PYX_ERR(0, 329, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_8, __pyx_empty_tuple, __pyx_t_11); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 329, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+    __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+    __Pyx_XDECREF_SET(__pyx_v_auc, __pyx_t_7);
+    __pyx_t_7 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":327
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":330
  * 
  *         auc = MulticlassAUROC(**{"num_classes": pred.size()[1], "thresholds" : None, "average" : None})
  *         auc_ = auc(pred, tru).view(-1)             # <<<<<<<<<<<<<<
  * 
  *         del tru
  */
     __Pyx_INCREF(__pyx_v_auc);
-    __pyx_t_7 = __pyx_v_auc; __pyx_t_4 = NULL;
-    __pyx_t_8 = 0;
+    __pyx_t_8 = __pyx_v_auc; __pyx_t_5 = NULL;
+    __pyx_t_9 = 0;
     #if CYTHON_UNPACK_METHODS
-    if (unlikely(PyMethod_Check(__pyx_t_7))) {
-      __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_7);
-      if (likely(__pyx_t_4)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
-        __Pyx_INCREF(__pyx_t_4);
+    if (unlikely(PyMethod_Check(__pyx_t_8))) {
+      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_8);
+      if (likely(__pyx_t_5)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
+        __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_7, function);
-        __pyx_t_8 = 1;
+        __Pyx_DECREF_SET(__pyx_t_8, function);
+        __pyx_t_9 = 1;
       }
     }
     #endif
     {
-      PyObject *__pyx_callargs[3] = {__pyx_t_4, __pyx_v_pred, __pyx_v_tru};
-      __pyx_t_10 = __Pyx_PyObject_FastCall(__pyx_t_7, __pyx_callargs+1-__pyx_t_8, 2+__pyx_t_8);
-      __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 327, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_10);
-      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+      PyObject *__pyx_callargs[3] = {__pyx_t_5, __pyx_v_pred, __pyx_v_tru};
+      __pyx_t_11 = __Pyx_PyObject_FastCall(__pyx_t_8, __pyx_callargs+1-__pyx_t_9, 2+__pyx_t_9);
+      __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+      if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 330, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_11);
+      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     }
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_view); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 327, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-    __pyx_t_10 = NULL;
-    __pyx_t_8 = 0;
+    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_view); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 330, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_8);
+    __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+    __pyx_t_11 = NULL;
+    __pyx_t_9 = 0;
     #if CYTHON_UNPACK_METHODS
-    if (likely(PyMethod_Check(__pyx_t_7))) {
-      __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_7);
-      if (likely(__pyx_t_10)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
-        __Pyx_INCREF(__pyx_t_10);
+    if (likely(PyMethod_Check(__pyx_t_8))) {
+      __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_8);
+      if (likely(__pyx_t_11)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
+        __Pyx_INCREF(__pyx_t_11);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_7, function);
-        __pyx_t_8 = 1;
+        __Pyx_DECREF_SET(__pyx_t_8, function);
+        __pyx_t_9 = 1;
       }
     }
     #endif
     {
-      PyObject *__pyx_callargs[2] = {__pyx_t_10, __pyx_int_neg_1};
-      __pyx_t_6 = __Pyx_PyObject_FastCall(__pyx_t_7, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
-      __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
-      if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 327, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_6);
-      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+      PyObject *__pyx_callargs[2] = {__pyx_t_11, __pyx_int_neg_1};
+      __pyx_t_7 = __Pyx_PyObject_FastCall(__pyx_t_8, __pyx_callargs+1-__pyx_t_9, 1+__pyx_t_9);
+      __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
+      if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 330, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_7);
+      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     }
-    __Pyx_XDECREF_SET(__pyx_v_auc_, __pyx_t_6);
-    __pyx_t_6 = 0;
+    __Pyx_XDECREF_SET(__pyx_v_auc_, __pyx_t_7);
+    __pyx_t_7 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":329
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":332
  *         auc_ = auc(pred, tru).view(-1)
  * 
  *         del tru             # <<<<<<<<<<<<<<
  *         del pred
  *         del thres
  */
     __Pyx_DECREF(__pyx_v_tru); __pyx_v_tru = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":330
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":333
  * 
  *         del tru
  *         del pred             # <<<<<<<<<<<<<<
  *         del thres
  *         for cls in range(len(fpr)):
  */
     __Pyx_DECREF(__pyx_v_pred); __pyx_v_pred = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":331
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":334
  *         del tru
  *         del pred
  *         del thres             # <<<<<<<<<<<<<<
  *         for cls in range(len(fpr)):
- *             try: dereference(roc_)[its.first].auc[cls+1] = auc_[cls].item()
+ *             try: dereference(roc_)[its.first].auc[cls] = auc_[cls].item()
  */
     __Pyx_DECREF(__pyx_v_thres); __pyx_v_thres = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":332
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":335
  *         del pred
  *         del thres
  *         for cls in range(len(fpr)):             # <<<<<<<<<<<<<<
- *             try: dereference(roc_)[its.first].auc[cls+1] = auc_[cls].item()
- *             except IndexError: pass
+ *             try: dereference(roc_)[its.first].auc[cls] = auc_[cls].item()
+ *             except IndexError: continue
  */
-    __pyx_t_12 = PyObject_Length(__pyx_v_fpr); if (unlikely(__pyx_t_12 == ((Py_ssize_t)-1))) __PYX_ERR(0, 332, __pyx_L1_error)
-    __pyx_t_6 = PyInt_FromSsize_t(__pyx_t_12); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 332, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_7 = __Pyx_PyObject_CallOneArg(__pyx_builtin_range, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 332, __pyx_L1_error)
+    __pyx_t_13 = PyObject_Length(__pyx_v_fpr); if (unlikely(__pyx_t_13 == ((Py_ssize_t)-1))) __PYX_ERR(0, 335, __pyx_L1_error)
+    __pyx_t_7 = PyInt_FromSsize_t(__pyx_t_13); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 335, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (likely(PyList_CheckExact(__pyx_t_7)) || PyTuple_CheckExact(__pyx_t_7)) {
-      __pyx_t_6 = __pyx_t_7; __Pyx_INCREF(__pyx_t_6);
-      __pyx_t_12 = 0;
-      __pyx_t_13 = NULL;
+    __pyx_t_8 = __Pyx_PyObject_CallOneArg(__pyx_builtin_range, __pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 335, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_8);
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    if (likely(PyList_CheckExact(__pyx_t_8)) || PyTuple_CheckExact(__pyx_t_8)) {
+      __pyx_t_7 = __pyx_t_8; __Pyx_INCREF(__pyx_t_7);
+      __pyx_t_13 = 0;
+      __pyx_t_14 = NULL;
     } else {
-      __pyx_t_12 = -1; __pyx_t_6 = PyObject_GetIter(__pyx_t_7); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 332, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_13 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_6); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 332, __pyx_L1_error)
+      __pyx_t_13 = -1; __pyx_t_7 = PyObject_GetIter(__pyx_t_8); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 335, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_7);
+      __pyx_t_14 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_7); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 335, __pyx_L1_error)
     }
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     for (;;) {
-      if (likely(!__pyx_t_13)) {
-        if (likely(PyList_CheckExact(__pyx_t_6))) {
+      if (likely(!__pyx_t_14)) {
+        if (likely(PyList_CheckExact(__pyx_t_7))) {
           {
-            Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_6);
+            Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_7);
             #if !CYTHON_ASSUME_SAFE_MACROS
-            if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 332, __pyx_L1_error)
+            if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 335, __pyx_L1_error)
             #endif
-            if (__pyx_t_12 >= __pyx_temp) break;
+            if (__pyx_t_13 >= __pyx_temp) break;
           }
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_7 = PyList_GET_ITEM(__pyx_t_6, __pyx_t_12); __Pyx_INCREF(__pyx_t_7); __pyx_t_12++; if (unlikely((0 < 0))) __PYX_ERR(0, 332, __pyx_L1_error)
+          __pyx_t_8 = PyList_GET_ITEM(__pyx_t_7, __pyx_t_13); __Pyx_INCREF(__pyx_t_8); __pyx_t_13++; if (unlikely((0 < 0))) __PYX_ERR(0, 335, __pyx_L1_error)
           #else
-          __pyx_t_7 = __Pyx_PySequence_ITEM(__pyx_t_6, __pyx_t_12); __pyx_t_12++; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 332, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_7);
+          __pyx_t_8 = __Pyx_PySequence_ITEM(__pyx_t_7, __pyx_t_13); __pyx_t_13++; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 335, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_8);
           #endif
         } else {
           {
-            Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_6);
+            Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_7);
             #if !CYTHON_ASSUME_SAFE_MACROS
-            if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 332, __pyx_L1_error)
+            if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 335, __pyx_L1_error)
             #endif
-            if (__pyx_t_12 >= __pyx_temp) break;
+            if (__pyx_t_13 >= __pyx_temp) break;
           }
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_7 = PyTuple_GET_ITEM(__pyx_t_6, __pyx_t_12); __Pyx_INCREF(__pyx_t_7); __pyx_t_12++; if (unlikely((0 < 0))) __PYX_ERR(0, 332, __pyx_L1_error)
+          __pyx_t_8 = PyTuple_GET_ITEM(__pyx_t_7, __pyx_t_13); __Pyx_INCREF(__pyx_t_8); __pyx_t_13++; if (unlikely((0 < 0))) __PYX_ERR(0, 335, __pyx_L1_error)
           #else
-          __pyx_t_7 = __Pyx_PySequence_ITEM(__pyx_t_6, __pyx_t_12); __pyx_t_12++; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 332, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_7);
+          __pyx_t_8 = __Pyx_PySequence_ITEM(__pyx_t_7, __pyx_t_13); __pyx_t_13++; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 335, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_8);
           #endif
         }
       } else {
-        __pyx_t_7 = __pyx_t_13(__pyx_t_6);
-        if (unlikely(!__pyx_t_7)) {
+        __pyx_t_8 = __pyx_t_14(__pyx_t_7);
+        if (unlikely(!__pyx_t_8)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 332, __pyx_L1_error)
+            else __PYX_ERR(0, 335, __pyx_L1_error)
           }
           break;
         }
-        __Pyx_GOTREF(__pyx_t_7);
+        __Pyx_GOTREF(__pyx_t_8);
       }
-      __Pyx_XDECREF_SET(__pyx_v_cls, __pyx_t_7);
-      __pyx_t_7 = 0;
+      __Pyx_XDECREF_SET(__pyx_v_cls, __pyx_t_8);
+      __pyx_t_8 = 0;
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":333
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":336
  *         del thres
  *         for cls in range(len(fpr)):
- *             try: dereference(roc_)[its.first].auc[cls+1] = auc_[cls].item()             # <<<<<<<<<<<<<<
- *             except IndexError: pass
+ *             try: dereference(roc_)[its.first].auc[cls] = auc_[cls].item()             # <<<<<<<<<<<<<<
+ *             except IndexError: continue
  *             name = "ROC Curve: "+ env(its.first) + " classification - " + str(cls)
  */
       {
         __Pyx_PyThreadState_declare
         __Pyx_PyThreadState_assign
-        __Pyx_ExceptionSave(&__pyx_t_14, &__pyx_t_15, &__pyx_t_16);
-        __Pyx_XGOTREF(__pyx_t_14);
+        __Pyx_ExceptionSave(&__pyx_t_15, &__pyx_t_16, &__pyx_t_17);
         __Pyx_XGOTREF(__pyx_t_15);
         __Pyx_XGOTREF(__pyx_t_16);
+        __Pyx_XGOTREF(__pyx_t_17);
         /*try:*/ {
-          __pyx_t_10 = __Pyx_PyObject_GetItem(__pyx_v_auc_, __pyx_v_cls); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 333, __pyx_L9_error)
-          __Pyx_GOTREF(__pyx_t_10);
-          __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_item); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 333, __pyx_L9_error)
-          __Pyx_GOTREF(__pyx_t_4);
-          __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-          __pyx_t_10 = NULL;
-          __pyx_t_8 = 0;
+          __pyx_t_11 = __Pyx_PyObject_GetItem(__pyx_v_auc_, __pyx_v_cls); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 336, __pyx_L10_error)
+          __Pyx_GOTREF(__pyx_t_11);
+          __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_item); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 336, __pyx_L10_error)
+          __Pyx_GOTREF(__pyx_t_5);
+          __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+          __pyx_t_11 = NULL;
+          __pyx_t_9 = 0;
           #if CYTHON_UNPACK_METHODS
-          if (likely(PyMethod_Check(__pyx_t_4))) {
-            __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_4);
-            if (likely(__pyx_t_10)) {
-              PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
-              __Pyx_INCREF(__pyx_t_10);
+          if (likely(PyMethod_Check(__pyx_t_5))) {
+            __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_5);
+            if (likely(__pyx_t_11)) {
+              PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
+              __Pyx_INCREF(__pyx_t_11);
               __Pyx_INCREF(function);
-              __Pyx_DECREF_SET(__pyx_t_4, function);
-              __pyx_t_8 = 1;
+              __Pyx_DECREF_SET(__pyx_t_5, function);
+              __pyx_t_9 = 1;
             }
           }
           #endif
           {
-            PyObject *__pyx_callargs[2] = {__pyx_t_10, NULL};
-            __pyx_t_7 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_8, 0+__pyx_t_8);
-            __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
-            if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 333, __pyx_L9_error)
-            __Pyx_GOTREF(__pyx_t_7);
-            __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+            PyObject *__pyx_callargs[2] = {__pyx_t_11, NULL};
+            __pyx_t_8 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_9, 0+__pyx_t_9);
+            __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
+            if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 336, __pyx_L10_error)
+            __Pyx_GOTREF(__pyx_t_8);
+            __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
           }
-          __pyx_t_17 = __pyx_PyFloat_AsFloat(__pyx_t_7); if (unlikely((__pyx_t_17 == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 333, __pyx_L9_error)
-          __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-          __pyx_t_7 = __Pyx_PyInt_AddObjC(__pyx_v_cls, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 333, __pyx_L9_error)
-          __Pyx_GOTREF(__pyx_t_7);
-          __pyx_t_8 = __Pyx_PyInt_As_int(__pyx_t_7); if (unlikely((__pyx_t_8 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 333, __pyx_L9_error)
-          __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-          (((*__pyx_v_roc_)[__pyx_v_its.first]).auc[__pyx_t_8]) = __pyx_t_17;
+          __pyx_t_18 = __pyx_PyFloat_AsFloat(__pyx_t_8); if (unlikely((__pyx_t_18 == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 336, __pyx_L10_error)
+          __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+          __pyx_t_9 = __Pyx_PyInt_As_int(__pyx_v_cls); if (unlikely((__pyx_t_9 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 336, __pyx_L10_error)
+          (((*__pyx_v_roc_)[__pyx_v_its.first]).auc[__pyx_t_9]) = __pyx_t_18;
         }
-        __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
         __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
         __Pyx_XDECREF(__pyx_t_16); __pyx_t_16 = 0;
-        goto __pyx_L16_try_end;
-        __pyx_L9_error:;
+        __Pyx_XDECREF(__pyx_t_17); __pyx_t_17 = 0;
+        goto __pyx_L17_try_end;
+        __pyx_L10_error:;
         __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
-        __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+        __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
         __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-        __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-        __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
+        __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+        __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-        /* "src/cmodules/cyincludes/cyoptimizer.pyx":334
+        /* "src/cmodules/cyincludes/cyoptimizer.pyx":337
  *         for cls in range(len(fpr)):
- *             try: dereference(roc_)[its.first].auc[cls+1] = auc_[cls].item()
- *             except IndexError: pass             # <<<<<<<<<<<<<<
+ *             try: dereference(roc_)[its.first].auc[cls] = auc_[cls].item()
+ *             except IndexError: continue             # <<<<<<<<<<<<<<
  *             name = "ROC Curve: "+ env(its.first) + " classification - " + str(cls)
  *             if name not in lines: lines[name] = []
  */
-        __pyx_t_8 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_IndexError);
-        if (__pyx_t_8) {
-          __Pyx_ErrRestore(0,0,0);
-          goto __pyx_L10_exception_handled;
+        __pyx_t_9 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_IndexError);
+        if (__pyx_t_9) {
+          __Pyx_AddTraceback("AnalysisG._cmodules.cOptimizer.make_roc_curve", __pyx_clineno, __pyx_lineno, __pyx_filename);
+          if (__Pyx_GetException(&__pyx_t_8, &__pyx_t_5, &__pyx_t_11) < 0) __PYX_ERR(0, 337, __pyx_L12_except_error)
+          __Pyx_XGOTREF(__pyx_t_8);
+          __Pyx_XGOTREF(__pyx_t_5);
+          __Pyx_XGOTREF(__pyx_t_11);
+          goto __pyx_L18_except_continue;
+          __pyx_L18_except_continue:;
+          __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+          __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+          __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
+          goto __pyx_L16_try_continue;
         }
-        goto __pyx_L11_except_error;
+        goto __pyx_L12_except_error;
 
-        /* "src/cmodules/cyincludes/cyoptimizer.pyx":333
+        /* "src/cmodules/cyincludes/cyoptimizer.pyx":336
  *         del thres
  *         for cls in range(len(fpr)):
- *             try: dereference(roc_)[its.first].auc[cls+1] = auc_[cls].item()             # <<<<<<<<<<<<<<
- *             except IndexError: pass
+ *             try: dereference(roc_)[its.first].auc[cls] = auc_[cls].item()             # <<<<<<<<<<<<<<
+ *             except IndexError: continue
  *             name = "ROC Curve: "+ env(its.first) + " classification - " + str(cls)
  */
-        __pyx_L11_except_error:;
-        __Pyx_XGIVEREF(__pyx_t_14);
+        __pyx_L12_except_error:;
         __Pyx_XGIVEREF(__pyx_t_15);
         __Pyx_XGIVEREF(__pyx_t_16);
-        __Pyx_ExceptionReset(__pyx_t_14, __pyx_t_15, __pyx_t_16);
+        __Pyx_XGIVEREF(__pyx_t_17);
+        __Pyx_ExceptionReset(__pyx_t_15, __pyx_t_16, __pyx_t_17);
         goto __pyx_L1_error;
-        __pyx_L10_exception_handled:;
-        __Pyx_XGIVEREF(__pyx_t_14);
+        __pyx_L16_try_continue:;
         __Pyx_XGIVEREF(__pyx_t_15);
         __Pyx_XGIVEREF(__pyx_t_16);
-        __Pyx_ExceptionReset(__pyx_t_14, __pyx_t_15, __pyx_t_16);
-        __pyx_L16_try_end:;
+        __Pyx_XGIVEREF(__pyx_t_17);
+        __Pyx_ExceptionReset(__pyx_t_15, __pyx_t_16, __pyx_t_17);
+        goto __pyx_L8_continue;
+        __pyx_L17_try_end:;
       }
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":335
- *             try: dereference(roc_)[its.first].auc[cls+1] = auc_[cls].item()
- *             except IndexError: pass
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":338
+ *             try: dereference(roc_)[its.first].auc[cls] = auc_[cls].item()
+ *             except IndexError: continue
  *             name = "ROC Curve: "+ env(its.first) + " classification - " + str(cls)             # <<<<<<<<<<<<<<
  *             if name not in lines: lines[name] = []
  *             lines[name] += [TLine(**{"xData" : fpr[cls].tolist(), "yData" : tpr[cls].tolist(), "Title" : mode})]
  */
-      __pyx_t_7 = __pyx_f_7cytools_env(__pyx_v_its.first); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 335, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_7);
-      __pyx_t_4 = __Pyx_PyUnicode_ConcatSafe(__pyx_kp_u_ROC_Curve, __pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 335, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      __pyx_t_7 = __Pyx_PyUnicode_ConcatInPlace(__pyx_t_4, __pyx_kp_u_classification_2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 335, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_7);
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_4 = __Pyx_PyObject_Str(__pyx_v_cls); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 335, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_10 = PyNumber_Add(__pyx_t_7, __pyx_t_4); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 335, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_10);
-      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __Pyx_XDECREF_SET(__pyx_v_name, __pyx_t_10);
-      __pyx_t_10 = 0;
+      __pyx_t_11 = __pyx_f_7cytools_env(__pyx_v_its.first); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 338, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_11);
+      __pyx_t_5 = __Pyx_PyUnicode_ConcatSafe(__pyx_kp_u_ROC_Curve, __pyx_t_11); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 338, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+      __pyx_t_11 = __Pyx_PyUnicode_ConcatInPlace(__pyx_t_5, __pyx_kp_u_classification_2); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 338, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_11);
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      __pyx_t_5 = __Pyx_PyObject_Str(__pyx_v_cls); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 338, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __pyx_t_8 = PyNumber_Add(__pyx_t_11, __pyx_t_5); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 338, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_8);
+      __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      __Pyx_XDECREF_SET(__pyx_v_name, __pyx_t_8);
+      __pyx_t_8 = 0;
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":336
- *             except IndexError: pass
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":339
+ *             except IndexError: continue
  *             name = "ROC Curve: "+ env(its.first) + " classification - " + str(cls)
  *             if name not in lines: lines[name] = []             # <<<<<<<<<<<<<<
  *             lines[name] += [TLine(**{"xData" : fpr[cls].tolist(), "yData" : tpr[cls].tolist(), "Title" : mode})]
  *     return lines
  */
       if (unlikely(__pyx_v_lines == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-        __PYX_ERR(0, 336, __pyx_L1_error)
+        __PYX_ERR(0, 339, __pyx_L1_error)
       }
-      __pyx_t_18 = (__Pyx_PyDict_ContainsTF(__pyx_v_name, __pyx_v_lines, Py_NE)); if (unlikely((__pyx_t_18 < 0))) __PYX_ERR(0, 336, __pyx_L1_error)
-      if (__pyx_t_18) {
-        __pyx_t_10 = PyList_New(0); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 336, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_10);
+      __pyx_t_4 = (__Pyx_PyDict_ContainsTF(__pyx_v_name, __pyx_v_lines, Py_NE)); if (unlikely((__pyx_t_4 < 0))) __PYX_ERR(0, 339, __pyx_L1_error)
+      if (__pyx_t_4) {
+        __pyx_t_8 = PyList_New(0); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 339, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_8);
         if (unlikely(__pyx_v_lines == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-          __PYX_ERR(0, 336, __pyx_L1_error)
+          __PYX_ERR(0, 339, __pyx_L1_error)
         }
-        if (unlikely((PyDict_SetItem(__pyx_v_lines, __pyx_v_name, __pyx_t_10) < 0))) __PYX_ERR(0, 336, __pyx_L1_error)
-        __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+        if (unlikely((PyDict_SetItem(__pyx_v_lines, __pyx_v_name, __pyx_t_8) < 0))) __PYX_ERR(0, 339, __pyx_L1_error)
+        __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       }
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":337
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":340
  *             name = "ROC Curve: "+ env(its.first) + " classification - " + str(cls)
  *             if name not in lines: lines[name] = []
  *             lines[name] += [TLine(**{"xData" : fpr[cls].tolist(), "yData" : tpr[cls].tolist(), "Title" : mode})]             # <<<<<<<<<<<<<<
  *     return lines
  * 
  */
       if (unlikely(__pyx_v_lines == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-        __PYX_ERR(0, 337, __pyx_L1_error)
+        __PYX_ERR(0, 340, __pyx_L1_error)
       }
       __Pyx_INCREF(__pyx_v_lines);
       __pyx_t_19 = __pyx_v_lines;
       __Pyx_INCREF(__pyx_v_name);
-      __pyx_t_10 = __pyx_v_name;
+      __pyx_t_8 = __pyx_v_name;
       if (unlikely(__pyx_t_19 == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-        __PYX_ERR(0, 337, __pyx_L1_error)
+        __PYX_ERR(0, 340, __pyx_L1_error)
       }
-      __pyx_t_4 = __Pyx_PyDict_GetItem(__pyx_t_19, __pyx_t_10); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 337, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_TLine); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 337, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_7);
-      __pyx_t_5 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 337, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyDict_GetItem(__pyx_t_19, __pyx_t_8); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 340, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_20 = __Pyx_PyObject_GetItem(__pyx_v_fpr, __pyx_v_cls); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 337, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_TLine); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 340, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_11);
+      __pyx_t_6 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 340, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_6);
+      __pyx_t_20 = __Pyx_PyObject_GetItem(__pyx_v_fpr, __pyx_v_cls); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 340, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_20);
-      __pyx_t_21 = __Pyx_PyObject_GetAttrStr(__pyx_t_20, __pyx_n_s_tolist); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 337, __pyx_L1_error)
+      __pyx_t_21 = __Pyx_PyObject_GetAttrStr(__pyx_t_20, __pyx_n_s_tolist); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 340, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_21);
       __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
       __pyx_t_20 = NULL;
-      __pyx_t_8 = 0;
+      __pyx_t_9 = 0;
       #if CYTHON_UNPACK_METHODS
       if (likely(PyMethod_Check(__pyx_t_21))) {
         __pyx_t_20 = PyMethod_GET_SELF(__pyx_t_21);
         if (likely(__pyx_t_20)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_21);
           __Pyx_INCREF(__pyx_t_20);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_21, function);
-          __pyx_t_8 = 1;
+          __pyx_t_9 = 1;
         }
       }
       #endif
       {
         PyObject *__pyx_callargs[2] = {__pyx_t_20, NULL};
-        __pyx_t_9 = __Pyx_PyObject_FastCall(__pyx_t_21, __pyx_callargs+1-__pyx_t_8, 0+__pyx_t_8);
+        __pyx_t_10 = __Pyx_PyObject_FastCall(__pyx_t_21, __pyx_callargs+1-__pyx_t_9, 0+__pyx_t_9);
         __Pyx_XDECREF(__pyx_t_20); __pyx_t_20 = 0;
-        if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 337, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_9);
+        if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 340, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_10);
         __Pyx_DECREF(__pyx_t_21); __pyx_t_21 = 0;
       }
-      if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_xData, __pyx_t_9) < 0) __PYX_ERR(0, 337, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-      __pyx_t_21 = __Pyx_PyObject_GetItem(__pyx_v_tpr, __pyx_v_cls); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 337, __pyx_L1_error)
+      if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_xData, __pyx_t_10) < 0) __PYX_ERR(0, 340, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+      __pyx_t_21 = __Pyx_PyObject_GetItem(__pyx_v_tpr, __pyx_v_cls); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 340, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_21);
-      __pyx_t_20 = __Pyx_PyObject_GetAttrStr(__pyx_t_21, __pyx_n_s_tolist); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 337, __pyx_L1_error)
+      __pyx_t_20 = __Pyx_PyObject_GetAttrStr(__pyx_t_21, __pyx_n_s_tolist); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 340, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_20);
       __Pyx_DECREF(__pyx_t_21); __pyx_t_21 = 0;
       __pyx_t_21 = NULL;
-      __pyx_t_8 = 0;
+      __pyx_t_9 = 0;
       #if CYTHON_UNPACK_METHODS
       if (likely(PyMethod_Check(__pyx_t_20))) {
         __pyx_t_21 = PyMethod_GET_SELF(__pyx_t_20);
         if (likely(__pyx_t_21)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_20);
           __Pyx_INCREF(__pyx_t_21);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_20, function);
-          __pyx_t_8 = 1;
+          __pyx_t_9 = 1;
         }
       }
       #endif
       {
         PyObject *__pyx_callargs[2] = {__pyx_t_21, NULL};
-        __pyx_t_9 = __Pyx_PyObject_FastCall(__pyx_t_20, __pyx_callargs+1-__pyx_t_8, 0+__pyx_t_8);
+        __pyx_t_10 = __Pyx_PyObject_FastCall(__pyx_t_20, __pyx_callargs+1-__pyx_t_9, 0+__pyx_t_9);
         __Pyx_XDECREF(__pyx_t_21); __pyx_t_21 = 0;
-        if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 337, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_9);
+        if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 340, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_10);
         __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
       }
-      if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_yData, __pyx_t_9) < 0) __PYX_ERR(0, 337, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-      if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_Title, __pyx_v_mode) < 0) __PYX_ERR(0, 337, __pyx_L1_error)
-      __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_empty_tuple, __pyx_t_5); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 337, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_9);
-      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __pyx_t_5 = PyList_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 337, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_5);
-      __Pyx_GIVEREF(__pyx_t_9);
-      if (__Pyx_PyList_SET_ITEM(__pyx_t_5, 0, __pyx_t_9)) __PYX_ERR(0, 337, __pyx_L1_error);
-      __pyx_t_9 = 0;
-      __pyx_t_9 = PyNumber_InPlaceAdd(__pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 337, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_9);
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+      if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_yData, __pyx_t_10) < 0) __PYX_ERR(0, 340, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+      if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_Title, __pyx_v_mode) < 0) __PYX_ERR(0, 340, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyObject_Call(__pyx_t_11, __pyx_empty_tuple, __pyx_t_6); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 340, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_10);
+      __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      __pyx_t_6 = PyList_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 340, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_6);
+      __Pyx_GIVEREF(__pyx_t_10);
+      if (__Pyx_PyList_SET_ITEM(__pyx_t_6, 0, __pyx_t_10)) __PYX_ERR(0, 340, __pyx_L1_error);
+      __pyx_t_10 = 0;
+      __pyx_t_10 = PyNumber_InPlaceAdd(__pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 340, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_10);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       if (unlikely(__pyx_t_19 == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-        __PYX_ERR(0, 337, __pyx_L1_error)
+        __PYX_ERR(0, 340, __pyx_L1_error)
       }
-      if (unlikely((PyDict_SetItem(__pyx_t_19, __pyx_t_10, __pyx_t_9) < 0))) __PYX_ERR(0, 337, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+      if (unlikely((PyDict_SetItem(__pyx_t_19, __pyx_t_8, __pyx_t_10) < 0))) __PYX_ERR(0, 340, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":332
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":335
  *         del pred
  *         del thres
  *         for cls in range(len(fpr)):             # <<<<<<<<<<<<<<
- *             try: dereference(roc_)[its.first].auc[cls+1] = auc_[cls].item()
- *             except IndexError: pass
+ *             try: dereference(roc_)[its.first].auc[cls] = auc_[cls].item()
+ *             except IndexError: continue
  */
+      __pyx_L8_continue:;
     }
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":316
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":318
  *     cdef pair[string, roc_t] its
  * 
  *     for its in dereference(roc_):             # <<<<<<<<<<<<<<
+ *         if not its.second.pred.size(): continue
  *         pred = torch.tensor(its.second.pred)
- *         dereference(roc_)[its.first].pred.clear()
  */
+    __pyx_L3_continue:;
   }
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":338
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":341
  *             if name not in lines: lines[name] = []
  *             lines[name] += [TLine(**{"xData" : fpr[cls].tolist(), "yData" : tpr[cls].tolist(), "Title" : mode})]
  *     return lines             # <<<<<<<<<<<<<<
  * 
  * cdef void make_auc_curve(map[string, roc_t]* roc_, map[string, vector[point_t]]* auc_):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_lines);
   __pyx_r = __pyx_v_lines;
   goto __pyx_L0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":313
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":315
  *     tmp_te.clear()
  * 
  * cdef dict make_roc_curve(map[string, roc_t]* roc_, dict lines, str mode):             # <<<<<<<<<<<<<<
  *     cdef pair[string, roc_t] its
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_XDECREF(__pyx_t_9);
+  __Pyx_XDECREF(__pyx_t_8);
   __Pyx_XDECREF(__pyx_t_10);
+  __Pyx_XDECREF(__pyx_t_11);
   __Pyx_XDECREF(__pyx_t_19);
   __Pyx_XDECREF(__pyx_t_20);
   __Pyx_XDECREF(__pyx_t_21);
   __Pyx_AddTraceback("AnalysisG._cmodules.cOptimizer.make_roc_curve", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_pred);
@@ -31885,15 +31903,15 @@
   __Pyx_XDECREF(__pyx_v_cls);
   __Pyx_XDECREF(__pyx_v_name);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/cmodules/cyincludes/cyoptimizer.pyx":340
+/* "src/cmodules/cyincludes/cyoptimizer.pyx":343
  *     return lines
  * 
  * cdef void make_auc_curve(map[string, roc_t]* roc_, map[string, vector[point_t]]* auc_):             # <<<<<<<<<<<<<<
  *     cdef pair[string, roc_t] its
  *     cdef pair[int, float] iti
  */
 
@@ -31914,111 +31932,111 @@
   PyObject *__pyx_t_10 = NULL;
   std::string __pyx_t_11;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("make_auc_curve", 1);
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":344
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":347
  *     cdef pair[int, float] iti
  *     cdef point_t data
  *     for its in dereference(roc_):             # <<<<<<<<<<<<<<
  *         for iti in its.second.auc:
  *             data = point_t()
  */
   __pyx_t_2 = &(*__pyx_v_roc_);
   __pyx_t_1 = __pyx_t_2->begin();
   for (;;) {
     if (!(__pyx_t_1 != __pyx_t_2->end())) break;
     __pyx_t_3 = *__pyx_t_1;
     ++__pyx_t_1;
     __pyx_v_its = __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_3);
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":345
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":348
  *     cdef point_t data
  *     for its in dereference(roc_):
  *         for iti in its.second.auc:             # <<<<<<<<<<<<<<
  *             data = point_t()
  *             data.average = iti.second
  */
     __pyx_t_4 = __pyx_v_its.second.auc.begin();
     for (;;) {
       if (!(__pyx_t_4 != __pyx_v_its.second.auc.end())) break;
       __pyx_t_5 = *__pyx_t_4;
       ++__pyx_t_4;
       __pyx_v_iti = __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_5);
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":346
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":349
  *     for its in dereference(roc_):
  *         for iti in its.second.auc:
  *             data = point_t()             # <<<<<<<<<<<<<<
  *             data.average = iti.second
  *             dereference(auc_)[enc(env(its.first) + " classification - " + str(iti.first))].push_back(data)
  */
       __pyx_v_data = __pyx_t_6;
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":347
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":350
  *         for iti in its.second.auc:
  *             data = point_t()
  *             data.average = iti.second             # <<<<<<<<<<<<<<
  *             dereference(auc_)[enc(env(its.first) + " classification - " + str(iti.first))].push_back(data)
  * 
  */
       __pyx_t_7 = __pyx_v_iti.second;
       __pyx_v_data.average = __pyx_t_7;
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":348
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":351
  *             data = point_t()
  *             data.average = iti.second
  *             dereference(auc_)[enc(env(its.first) + " classification - " + str(iti.first))].push_back(data)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-      __pyx_t_8 = __pyx_f_7cytools_env(__pyx_v_its.first); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 348, __pyx_L1_error)
+      __pyx_t_8 = __pyx_f_7cytools_env(__pyx_v_its.first); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 351, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
-      __pyx_t_9 = __Pyx_PyUnicode_ConcatInPlaceSafe(__pyx_t_8, __pyx_kp_u_classification_2); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 348, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyUnicode_ConcatInPlaceSafe(__pyx_t_8, __pyx_kp_u_classification_2); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 351, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __pyx_t_8 = __Pyx_PyInt_From_int(__pyx_v_iti.first); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 348, __pyx_L1_error)
+      __pyx_t_8 = __Pyx_PyInt_From_int(__pyx_v_iti.first); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 351, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
-      __pyx_t_10 = __Pyx_PyObject_Str(__pyx_t_8); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 348, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyObject_Str(__pyx_t_8); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 351, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __pyx_t_8 = PyNumber_Add(__pyx_t_9, __pyx_t_10); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 348, __pyx_L1_error)
+      __pyx_t_8 = PyNumber_Add(__pyx_t_9, __pyx_t_10); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 351, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-      __pyx_t_11 = __pyx_f_7cytools_enc(((PyObject*)__pyx_t_8)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 348, __pyx_L1_error)
+      __pyx_t_11 = __pyx_f_7cytools_enc(((PyObject*)__pyx_t_8)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 351, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       try {
         ((*__pyx_v_auc_)[__pyx_t_11]).push_back(__pyx_v_data);
       } catch(...) {
         __Pyx_CppExn2PyErr();
-        __PYX_ERR(0, 348, __pyx_L1_error)
+        __PYX_ERR(0, 351, __pyx_L1_error)
       }
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":345
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":348
  *     cdef point_t data
  *     for its in dereference(roc_):
  *         for iti in its.second.auc:             # <<<<<<<<<<<<<<
  *             data = point_t()
  *             data.average = iti.second
  */
     }
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":344
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":347
  *     cdef pair[int, float] iti
  *     cdef point_t data
  *     for its in dereference(roc_):             # <<<<<<<<<<<<<<
  *         for iti in its.second.auc:
  *             data = point_t()
  */
   }
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":340
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":343
  *     return lines
  * 
  * cdef void make_auc_curve(map[string, roc_t]* roc_, map[string, vector[point_t]]* auc_):             # <<<<<<<<<<<<<<
  *     cdef pair[string, roc_t] its
  *     cdef pair[int, float] iti
  */
 
@@ -32029,15 +32047,15 @@
   __Pyx_XDECREF(__pyx_t_9);
   __Pyx_XDECREF(__pyx_t_10);
   __Pyx_AddTraceback("AnalysisG._cmodules.cOptimizer.make_auc_curve", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "src/cmodules/cyincludes/cyoptimizer.pyx":351
+/* "src/cmodules/cyincludes/cyoptimizer.pyx":354
  * 
  * 
  * cdef void make_roc_plots(map[int, CyEpoch*] train, map[int, CyEpoch*] valid, map[int, CyEpoch*] test, str path, report_t* state):             # <<<<<<<<<<<<<<
  *     cdef pair[int, CyEpoch*] itr
  * 
  */
 
@@ -32089,387 +32107,387 @@
   PyObject *__pyx_t_20 = NULL;
   PyObject *(*__pyx_t_21)(PyObject *);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("make_roc_plots", 1);
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":354
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":357
  *     cdef pair[int, CyEpoch*] itr
  * 
  *     cdef dict tmp_tr = {}             # <<<<<<<<<<<<<<
  *     cdef dict tmp_va = {}
  *     cdef dict tmp_te = {}
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 354, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 357, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_tmp_tr = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":355
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":358
  * 
  *     cdef dict tmp_tr = {}
  *     cdef dict tmp_va = {}             # <<<<<<<<<<<<<<
  *     cdef dict tmp_te = {}
  * 
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 355, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 358, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_tmp_va = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":356
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":359
  *     cdef dict tmp_tr = {}
  *     cdef dict tmp_va = {}
  *     cdef dict tmp_te = {}             # <<<<<<<<<<<<<<
  * 
  *     cdef list folds = []
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 356, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 359, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_tmp_te = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":358
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":361
  *     cdef dict tmp_te = {}
  * 
  *     cdef list folds = []             # <<<<<<<<<<<<<<
  *     cdef list epochs = []
  *     cdef int epoch, kf
  */
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 358, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 361, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_folds = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":359
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":362
  * 
  *     cdef list folds = []
  *     cdef list epochs = []             # <<<<<<<<<<<<<<
  *     cdef int epoch, kf
  *     cdef pair[int, map[string, roc_t]] itx
  */
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 359, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 362, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_epochs = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":363
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":366
  *     cdef pair[int, map[string, roc_t]] itx
  * 
  *     for itr in train:             # <<<<<<<<<<<<<<
  *         folds += [itx.first for itx in train[itr.first].auc]
  *         epochs += [itr.first]
  */
   __pyx_t_2 = __pyx_v_train.begin();
   for (;;) {
     if (!(__pyx_t_2 != __pyx_v_train.end())) break;
     __pyx_t_3 = *__pyx_t_2;
     ++__pyx_t_2;
     __pyx_v_itr = __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_3);
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":364
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":367
  * 
  *     for itr in train:
  *         folds += [itx.first for itx in train[itr.first].auc]             # <<<<<<<<<<<<<<
  *         epochs += [itr.first]
  * 
  */
     { /* enter inner scope */
-      __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 364, __pyx_L1_error)
+      __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 367, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __pyx_t_5 = (__pyx_v_train[__pyx_v_itr.first])->auc;
       __pyx_t_4 = __pyx_t_5.begin();
       for (;;) {
         if (!(__pyx_t_4 != __pyx_t_5.end())) break;
         __pyx_t_6 = *__pyx_t_4;
         ++__pyx_t_4;
         __pyx_7genexpr__pyx_v_itx = __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_6);
-        __pyx_t_7 = __Pyx_PyInt_From_int(__pyx_7genexpr__pyx_v_itx.first); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 364, __pyx_L1_error)
+        __pyx_t_7 = __Pyx_PyInt_From_int(__pyx_7genexpr__pyx_v_itx.first); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 367, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_7);
-        if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_7))) __PYX_ERR(0, 364, __pyx_L1_error)
+        if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_7))) __PYX_ERR(0, 367, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       }
     } /* exit inner scope */
-    __pyx_t_7 = PyNumber_InPlaceAdd(__pyx_v_folds, __pyx_t_1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 364, __pyx_L1_error)
+    __pyx_t_7 = PyNumber_InPlaceAdd(__pyx_v_folds, __pyx_t_1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 367, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF_SET(__pyx_v_folds, ((PyObject*)__pyx_t_7));
     __pyx_t_7 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":365
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":368
  *     for itr in train:
  *         folds += [itx.first for itx in train[itr.first].auc]
  *         epochs += [itr.first]             # <<<<<<<<<<<<<<
  * 
  *     for itr in valid:
  */
-    __pyx_t_7 = __Pyx_PyInt_From_int(__pyx_v_itr.first); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 365, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyInt_From_int(__pyx_v_itr.first); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 368, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 365, __pyx_L1_error)
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 368, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_GIVEREF(__pyx_t_7);
-    if (__Pyx_PyList_SET_ITEM(__pyx_t_1, 0, __pyx_t_7)) __PYX_ERR(0, 365, __pyx_L1_error);
+    if (__Pyx_PyList_SET_ITEM(__pyx_t_1, 0, __pyx_t_7)) __PYX_ERR(0, 368, __pyx_L1_error);
     __pyx_t_7 = 0;
-    __pyx_t_7 = PyNumber_InPlaceAdd(__pyx_v_epochs, __pyx_t_1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 365, __pyx_L1_error)
+    __pyx_t_7 = PyNumber_InPlaceAdd(__pyx_v_epochs, __pyx_t_1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 368, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF_SET(__pyx_v_epochs, ((PyObject*)__pyx_t_7));
     __pyx_t_7 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":363
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":366
  *     cdef pair[int, map[string, roc_t]] itx
  * 
  *     for itr in train:             # <<<<<<<<<<<<<<
  *         folds += [itx.first for itx in train[itr.first].auc]
  *         epochs += [itr.first]
  */
   }
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":367
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":370
  *         epochs += [itr.first]
  * 
  *     for itr in valid:             # <<<<<<<<<<<<<<
  *         folds += [itx.first for itx in valid[itr.first].auc]
  *         epochs += [itr.first]
  */
   __pyx_t_2 = __pyx_v_valid.begin();
   for (;;) {
     if (!(__pyx_t_2 != __pyx_v_valid.end())) break;
     __pyx_t_3 = *__pyx_t_2;
     ++__pyx_t_2;
     __pyx_v_itr = __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_3);
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":368
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":371
  * 
  *     for itr in valid:
  *         folds += [itx.first for itx in valid[itr.first].auc]             # <<<<<<<<<<<<<<
  *         epochs += [itr.first]
  * 
  */
     { /* enter inner scope */
-      __pyx_t_7 = PyList_New(0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 368, __pyx_L1_error)
+      __pyx_t_7 = PyList_New(0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 371, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __pyx_t_5 = (__pyx_v_valid[__pyx_v_itr.first])->auc;
       __pyx_t_4 = __pyx_t_5.begin();
       for (;;) {
         if (!(__pyx_t_4 != __pyx_t_5.end())) break;
         __pyx_t_6 = *__pyx_t_4;
         ++__pyx_t_4;
         __pyx_8genexpr1__pyx_v_itx = __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_6);
-        __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_8genexpr1__pyx_v_itx.first); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 368, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_8genexpr1__pyx_v_itx.first); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 371, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
-        if (unlikely(__Pyx_ListComp_Append(__pyx_t_7, (PyObject*)__pyx_t_1))) __PYX_ERR(0, 368, __pyx_L1_error)
+        if (unlikely(__Pyx_ListComp_Append(__pyx_t_7, (PyObject*)__pyx_t_1))) __PYX_ERR(0, 371, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       }
     } /* exit inner scope */
-    __pyx_t_1 = PyNumber_InPlaceAdd(__pyx_v_folds, __pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 368, __pyx_L1_error)
+    __pyx_t_1 = PyNumber_InPlaceAdd(__pyx_v_folds, __pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 371, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF_SET(__pyx_v_folds, ((PyObject*)__pyx_t_1));
     __pyx_t_1 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":369
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":372
  *     for itr in valid:
  *         folds += [itx.first for itx in valid[itr.first].auc]
  *         epochs += [itr.first]             # <<<<<<<<<<<<<<
  * 
  *     for itr in test:
  */
-    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_itr.first); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 369, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_itr.first); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 372, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_7 = PyList_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 369, __pyx_L1_error)
+    __pyx_t_7 = PyList_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 372, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_GIVEREF(__pyx_t_1);
-    if (__Pyx_PyList_SET_ITEM(__pyx_t_7, 0, __pyx_t_1)) __PYX_ERR(0, 369, __pyx_L1_error);
+    if (__Pyx_PyList_SET_ITEM(__pyx_t_7, 0, __pyx_t_1)) __PYX_ERR(0, 372, __pyx_L1_error);
     __pyx_t_1 = 0;
-    __pyx_t_1 = PyNumber_InPlaceAdd(__pyx_v_epochs, __pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 369, __pyx_L1_error)
+    __pyx_t_1 = PyNumber_InPlaceAdd(__pyx_v_epochs, __pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 372, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF_SET(__pyx_v_epochs, ((PyObject*)__pyx_t_1));
     __pyx_t_1 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":367
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":370
  *         epochs += [itr.first]
  * 
  *     for itr in valid:             # <<<<<<<<<<<<<<
  *         folds += [itx.first for itx in valid[itr.first].auc]
  *         epochs += [itr.first]
  */
   }
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":371
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":374
  *         epochs += [itr.first]
  * 
  *     for itr in test:             # <<<<<<<<<<<<<<
  *         folds += [itx.first for itx in test[itr.first].auc]
  *         epochs += [itr.first]
  */
   __pyx_t_2 = __pyx_v_test.begin();
   for (;;) {
     if (!(__pyx_t_2 != __pyx_v_test.end())) break;
     __pyx_t_3 = *__pyx_t_2;
     ++__pyx_t_2;
     __pyx_v_itr = __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_3);
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":372
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":375
  * 
  *     for itr in test:
  *         folds += [itx.first for itx in test[itr.first].auc]             # <<<<<<<<<<<<<<
  *         epochs += [itr.first]
  * 
  */
     { /* enter inner scope */
-      __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 372, __pyx_L1_error)
+      __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 375, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __pyx_t_5 = (__pyx_v_test[__pyx_v_itr.first])->auc;
       __pyx_t_4 = __pyx_t_5.begin();
       for (;;) {
         if (!(__pyx_t_4 != __pyx_t_5.end())) break;
         __pyx_t_6 = *__pyx_t_4;
         ++__pyx_t_4;
         __pyx_8genexpr2__pyx_v_itx = __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_6);
-        __pyx_t_7 = __Pyx_PyInt_From_int(__pyx_8genexpr2__pyx_v_itx.first); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 372, __pyx_L1_error)
+        __pyx_t_7 = __Pyx_PyInt_From_int(__pyx_8genexpr2__pyx_v_itx.first); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 375, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_7);
-        if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_7))) __PYX_ERR(0, 372, __pyx_L1_error)
+        if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_7))) __PYX_ERR(0, 375, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       }
     } /* exit inner scope */
-    __pyx_t_7 = PyNumber_InPlaceAdd(__pyx_v_folds, __pyx_t_1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 372, __pyx_L1_error)
+    __pyx_t_7 = PyNumber_InPlaceAdd(__pyx_v_folds, __pyx_t_1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 375, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF_SET(__pyx_v_folds, ((PyObject*)__pyx_t_7));
     __pyx_t_7 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":373
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":376
  *     for itr in test:
  *         folds += [itx.first for itx in test[itr.first].auc]
  *         epochs += [itr.first]             # <<<<<<<<<<<<<<
  * 
  *     cdef dict lines
  */
-    __pyx_t_7 = __Pyx_PyInt_From_int(__pyx_v_itr.first); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 373, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyInt_From_int(__pyx_v_itr.first); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 376, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 373, __pyx_L1_error)
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 376, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_GIVEREF(__pyx_t_7);
-    if (__Pyx_PyList_SET_ITEM(__pyx_t_1, 0, __pyx_t_7)) __PYX_ERR(0, 373, __pyx_L1_error);
+    if (__Pyx_PyList_SET_ITEM(__pyx_t_1, 0, __pyx_t_7)) __PYX_ERR(0, 376, __pyx_L1_error);
     __pyx_t_7 = 0;
-    __pyx_t_7 = PyNumber_InPlaceAdd(__pyx_v_epochs, __pyx_t_1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 373, __pyx_L1_error)
+    __pyx_t_7 = PyNumber_InPlaceAdd(__pyx_v_epochs, __pyx_t_1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 376, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF_SET(__pyx_v_epochs, ((PyObject*)__pyx_t_7));
     __pyx_t_7 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":371
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":374
  *         epochs += [itr.first]
  * 
  *     for itr in test:             # <<<<<<<<<<<<<<
  *         folds += [itx.first for itx in test[itr.first].auc]
  *         epochs += [itr.first]
  */
   }
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":376
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":379
  * 
  *     cdef dict lines
  *     cdef dict line_auc = {}             # <<<<<<<<<<<<<<
  *     cdef map[string, vector[point_t]] auc_tr
  *     cdef map[string, vector[point_t]] auc_va
  */
-  __pyx_t_7 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 376, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 379, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __pyx_v_line_auc = ((PyObject*)__pyx_t_7);
   __pyx_t_7 = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":381
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":384
  *     cdef map[string, vector[point_t]] auc_ev
  * 
  *     for epoch in sorted(set(epochs)):             # <<<<<<<<<<<<<<
  *         for kf in sorted(set(folds)):
  *             lines = {}
  */
-  __pyx_t_1 = PySet_New(__pyx_v_epochs); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 381, __pyx_L1_error)
+  __pyx_t_1 = PySet_New(__pyx_v_epochs); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 384, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_8 = PySequence_List(__pyx_t_1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 381, __pyx_L1_error)
+  __pyx_t_8 = PySequence_List(__pyx_t_1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 384, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_7 = ((PyObject*)__pyx_t_8);
   __pyx_t_8 = 0;
-  __pyx_t_9 = PyList_Sort(__pyx_t_7); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(0, 381, __pyx_L1_error)
+  __pyx_t_9 = PyList_Sort(__pyx_t_7); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(0, 384, __pyx_L1_error)
   __pyx_t_8 = __pyx_t_7; __Pyx_INCREF(__pyx_t_8);
   __pyx_t_10 = 0;
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   for (;;) {
     {
       Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_8);
       #if !CYTHON_ASSUME_SAFE_MACROS
-      if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 381, __pyx_L1_error)
+      if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 384, __pyx_L1_error)
       #endif
       if (__pyx_t_10 >= __pyx_temp) break;
     }
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-    __pyx_t_7 = PyList_GET_ITEM(__pyx_t_8, __pyx_t_10); __Pyx_INCREF(__pyx_t_7); __pyx_t_10++; if (unlikely((0 < 0))) __PYX_ERR(0, 381, __pyx_L1_error)
+    __pyx_t_7 = PyList_GET_ITEM(__pyx_t_8, __pyx_t_10); __Pyx_INCREF(__pyx_t_7); __pyx_t_10++; if (unlikely((0 < 0))) __PYX_ERR(0, 384, __pyx_L1_error)
     #else
-    __pyx_t_7 = __Pyx_PySequence_ITEM(__pyx_t_8, __pyx_t_10); __pyx_t_10++; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 381, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PySequence_ITEM(__pyx_t_8, __pyx_t_10); __pyx_t_10++; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 384, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     #endif
-    __pyx_t_11 = __Pyx_PyInt_As_int(__pyx_t_7); if (unlikely((__pyx_t_11 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 381, __pyx_L1_error)
+    __pyx_t_11 = __Pyx_PyInt_As_int(__pyx_t_7); if (unlikely((__pyx_t_11 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 384, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __pyx_v_epoch = __pyx_t_11;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":382
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":385
  * 
  *     for epoch in sorted(set(epochs)):
  *         for kf in sorted(set(folds)):             # <<<<<<<<<<<<<<
  *             lines = {}
  *             if train.count(epoch) and train[epoch].auc.count(kf):
  */
-    __pyx_t_1 = PySet_New(__pyx_v_folds); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 382, __pyx_L1_error)
+    __pyx_t_1 = PySet_New(__pyx_v_folds); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 385, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_12 = PySequence_List(__pyx_t_1); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 382, __pyx_L1_error)
+    __pyx_t_12 = PySequence_List(__pyx_t_1); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 385, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_12);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_7 = ((PyObject*)__pyx_t_12);
     __pyx_t_12 = 0;
-    __pyx_t_9 = PyList_Sort(__pyx_t_7); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(0, 382, __pyx_L1_error)
+    __pyx_t_9 = PyList_Sort(__pyx_t_7); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(0, 385, __pyx_L1_error)
     __pyx_t_12 = __pyx_t_7; __Pyx_INCREF(__pyx_t_12);
     __pyx_t_13 = 0;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     for (;;) {
       {
         Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_12);
         #if !CYTHON_ASSUME_SAFE_MACROS
-        if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 382, __pyx_L1_error)
+        if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 385, __pyx_L1_error)
         #endif
         if (__pyx_t_13 >= __pyx_temp) break;
       }
       #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-      __pyx_t_7 = PyList_GET_ITEM(__pyx_t_12, __pyx_t_13); __Pyx_INCREF(__pyx_t_7); __pyx_t_13++; if (unlikely((0 < 0))) __PYX_ERR(0, 382, __pyx_L1_error)
+      __pyx_t_7 = PyList_GET_ITEM(__pyx_t_12, __pyx_t_13); __Pyx_INCREF(__pyx_t_7); __pyx_t_13++; if (unlikely((0 < 0))) __PYX_ERR(0, 385, __pyx_L1_error)
       #else
-      __pyx_t_7 = __Pyx_PySequence_ITEM(__pyx_t_12, __pyx_t_13); __pyx_t_13++; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 382, __pyx_L1_error)
+      __pyx_t_7 = __Pyx_PySequence_ITEM(__pyx_t_12, __pyx_t_13); __pyx_t_13++; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 385, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       #endif
-      __pyx_t_11 = __Pyx_PyInt_As_int(__pyx_t_7); if (unlikely((__pyx_t_11 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 382, __pyx_L1_error)
+      __pyx_t_11 = __Pyx_PyInt_As_int(__pyx_t_7); if (unlikely((__pyx_t_11 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 385, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       __pyx_v_kf = __pyx_t_11;
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":383
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":386
  *     for epoch in sorted(set(epochs)):
  *         for kf in sorted(set(folds)):
  *             lines = {}             # <<<<<<<<<<<<<<
  *             if train.count(epoch) and train[epoch].auc.count(kf):
  *                 lines = make_roc_curve(&train[epoch].auc[kf], lines, "training")
  */
-      __pyx_t_7 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 383, __pyx_L1_error)
+      __pyx_t_7 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 386, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_XDECREF_SET(__pyx_v_lines, ((PyObject*)__pyx_t_7));
       __pyx_t_7 = 0;
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":384
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":387
  *         for kf in sorted(set(folds)):
  *             lines = {}
  *             if train.count(epoch) and train[epoch].auc.count(kf):             # <<<<<<<<<<<<<<
  *                 lines = make_roc_curve(&train[epoch].auc[kf], lines, "training")
  *                 make_auc_curve(&train[epoch].auc[kf], &auc_tr)
  */
       __pyx_t_15 = (__pyx_v_train.count(__pyx_v_epoch) != 0);
@@ -32479,45 +32497,45 @@
         goto __pyx_L26_bool_binop_done;
       }
       __pyx_t_15 = ((__pyx_v_train[__pyx_v_epoch])->auc.count(__pyx_v_kf) != 0);
       __pyx_t_14 = __pyx_t_15;
       __pyx_L26_bool_binop_done:;
       if (__pyx_t_14) {
 
-        /* "src/cmodules/cyincludes/cyoptimizer.pyx":385
+        /* "src/cmodules/cyincludes/cyoptimizer.pyx":388
  *             lines = {}
  *             if train.count(epoch) and train[epoch].auc.count(kf):
  *                 lines = make_roc_curve(&train[epoch].auc[kf], lines, "training")             # <<<<<<<<<<<<<<
  *                 make_auc_curve(&train[epoch].auc[kf], &auc_tr)
  * 
  */
-        __pyx_t_7 = __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_make_roc_curve((&((__pyx_v_train[__pyx_v_epoch])->auc[__pyx_v_kf])), __pyx_v_lines, __pyx_n_u_training); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 385, __pyx_L1_error)
+        __pyx_t_7 = __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_make_roc_curve((&((__pyx_v_train[__pyx_v_epoch])->auc[__pyx_v_kf])), __pyx_v_lines, __pyx_n_u_training); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 388, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_7);
         __Pyx_DECREF_SET(__pyx_v_lines, ((PyObject*)__pyx_t_7));
         __pyx_t_7 = 0;
 
-        /* "src/cmodules/cyincludes/cyoptimizer.pyx":386
+        /* "src/cmodules/cyincludes/cyoptimizer.pyx":389
  *             if train.count(epoch) and train[epoch].auc.count(kf):
  *                 lines = make_roc_curve(&train[epoch].auc[kf], lines, "training")
  *                 make_auc_curve(&train[epoch].auc[kf], &auc_tr)             # <<<<<<<<<<<<<<
  * 
  *             if valid.count(epoch) and valid[epoch].auc.count(kf):
  */
-        __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_make_auc_curve((&((__pyx_v_train[__pyx_v_epoch])->auc[__pyx_v_kf])), (&__pyx_v_auc_tr)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 386, __pyx_L1_error)
+        __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_make_auc_curve((&((__pyx_v_train[__pyx_v_epoch])->auc[__pyx_v_kf])), (&__pyx_v_auc_tr)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 389, __pyx_L1_error)
 
-        /* "src/cmodules/cyincludes/cyoptimizer.pyx":384
+        /* "src/cmodules/cyincludes/cyoptimizer.pyx":387
  *         for kf in sorted(set(folds)):
  *             lines = {}
  *             if train.count(epoch) and train[epoch].auc.count(kf):             # <<<<<<<<<<<<<<
  *                 lines = make_roc_curve(&train[epoch].auc[kf], lines, "training")
  *                 make_auc_curve(&train[epoch].auc[kf], &auc_tr)
  */
       }
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":388
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":391
  *                 make_auc_curve(&train[epoch].auc[kf], &auc_tr)
  * 
  *             if valid.count(epoch) and valid[epoch].auc.count(kf):             # <<<<<<<<<<<<<<
  *                 lines = make_roc_curve(&valid[epoch].auc[kf], lines, "validation")
  *                 make_auc_curve(&valid[epoch].auc[kf], &auc_va)
  */
       __pyx_t_15 = (__pyx_v_valid.count(__pyx_v_epoch) != 0);
@@ -32527,45 +32545,45 @@
         goto __pyx_L29_bool_binop_done;
       }
       __pyx_t_15 = ((__pyx_v_valid[__pyx_v_epoch])->auc.count(__pyx_v_kf) != 0);
       __pyx_t_14 = __pyx_t_15;
       __pyx_L29_bool_binop_done:;
       if (__pyx_t_14) {
 
-        /* "src/cmodules/cyincludes/cyoptimizer.pyx":389
+        /* "src/cmodules/cyincludes/cyoptimizer.pyx":392
  * 
  *             if valid.count(epoch) and valid[epoch].auc.count(kf):
  *                 lines = make_roc_curve(&valid[epoch].auc[kf], lines, "validation")             # <<<<<<<<<<<<<<
  *                 make_auc_curve(&valid[epoch].auc[kf], &auc_va)
  * 
  */
-        __pyx_t_7 = __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_make_roc_curve((&((__pyx_v_valid[__pyx_v_epoch])->auc[__pyx_v_kf])), __pyx_v_lines, __pyx_n_u_validation); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 389, __pyx_L1_error)
+        __pyx_t_7 = __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_make_roc_curve((&((__pyx_v_valid[__pyx_v_epoch])->auc[__pyx_v_kf])), __pyx_v_lines, __pyx_n_u_validation); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 392, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_7);
         __Pyx_DECREF_SET(__pyx_v_lines, ((PyObject*)__pyx_t_7));
         __pyx_t_7 = 0;
 
-        /* "src/cmodules/cyincludes/cyoptimizer.pyx":390
+        /* "src/cmodules/cyincludes/cyoptimizer.pyx":393
  *             if valid.count(epoch) and valid[epoch].auc.count(kf):
  *                 lines = make_roc_curve(&valid[epoch].auc[kf], lines, "validation")
  *                 make_auc_curve(&valid[epoch].auc[kf], &auc_va)             # <<<<<<<<<<<<<<
  * 
  *             if test.count(epoch) and test[epoch].auc.count(kf):
  */
-        __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_make_auc_curve((&((__pyx_v_valid[__pyx_v_epoch])->auc[__pyx_v_kf])), (&__pyx_v_auc_va)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 390, __pyx_L1_error)
+        __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_make_auc_curve((&((__pyx_v_valid[__pyx_v_epoch])->auc[__pyx_v_kf])), (&__pyx_v_auc_va)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 393, __pyx_L1_error)
 
-        /* "src/cmodules/cyincludes/cyoptimizer.pyx":388
+        /* "src/cmodules/cyincludes/cyoptimizer.pyx":391
  *                 make_auc_curve(&train[epoch].auc[kf], &auc_tr)
  * 
  *             if valid.count(epoch) and valid[epoch].auc.count(kf):             # <<<<<<<<<<<<<<
  *                 lines = make_roc_curve(&valid[epoch].auc[kf], lines, "validation")
  *                 make_auc_curve(&valid[epoch].auc[kf], &auc_va)
  */
       }
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":392
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":395
  *                 make_auc_curve(&valid[epoch].auc[kf], &auc_va)
  * 
  *             if test.count(epoch) and test[epoch].auc.count(kf):             # <<<<<<<<<<<<<<
  *                 lines = make_roc_curve(&test[epoch].auc[kf], lines, "evaluation")
  *                 make_auc_curve(&test[epoch].auc[kf], &auc_ev)
  */
       __pyx_t_15 = (__pyx_v_test.count(__pyx_v_epoch) != 0);
@@ -32575,77 +32593,77 @@
         goto __pyx_L32_bool_binop_done;
       }
       __pyx_t_15 = ((__pyx_v_test[__pyx_v_epoch])->auc.count(__pyx_v_kf) != 0);
       __pyx_t_14 = __pyx_t_15;
       __pyx_L32_bool_binop_done:;
       if (__pyx_t_14) {
 
-        /* "src/cmodules/cyincludes/cyoptimizer.pyx":393
+        /* "src/cmodules/cyincludes/cyoptimizer.pyx":396
  * 
  *             if test.count(epoch) and test[epoch].auc.count(kf):
  *                 lines = make_roc_curve(&test[epoch].auc[kf], lines, "evaluation")             # <<<<<<<<<<<<<<
  *                 make_auc_curve(&test[epoch].auc[kf], &auc_ev)
  * 
  */
-        __pyx_t_7 = __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_make_roc_curve((&((__pyx_v_test[__pyx_v_epoch])->auc[__pyx_v_kf])), __pyx_v_lines, __pyx_n_u_evaluation); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 393, __pyx_L1_error)
+        __pyx_t_7 = __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_make_roc_curve((&((__pyx_v_test[__pyx_v_epoch])->auc[__pyx_v_kf])), __pyx_v_lines, __pyx_n_u_evaluation); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 396, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_7);
         __Pyx_DECREF_SET(__pyx_v_lines, ((PyObject*)__pyx_t_7));
         __pyx_t_7 = 0;
 
-        /* "src/cmodules/cyincludes/cyoptimizer.pyx":394
+        /* "src/cmodules/cyincludes/cyoptimizer.pyx":397
  *             if test.count(epoch) and test[epoch].auc.count(kf):
  *                 lines = make_roc_curve(&test[epoch].auc[kf], lines, "evaluation")
  *                 make_auc_curve(&test[epoch].auc[kf], &auc_ev)             # <<<<<<<<<<<<<<
  * 
  *             for name in lines:
  */
-        __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_make_auc_curve((&((__pyx_v_test[__pyx_v_epoch])->auc[__pyx_v_kf])), (&__pyx_v_auc_ev)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 394, __pyx_L1_error)
+        __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_make_auc_curve((&((__pyx_v_test[__pyx_v_epoch])->auc[__pyx_v_kf])), (&__pyx_v_auc_ev)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 397, __pyx_L1_error)
 
-        /* "src/cmodules/cyincludes/cyoptimizer.pyx":392
+        /* "src/cmodules/cyincludes/cyoptimizer.pyx":395
  *                 make_auc_curve(&valid[epoch].auc[kf], &auc_va)
  * 
  *             if test.count(epoch) and test[epoch].auc.count(kf):             # <<<<<<<<<<<<<<
  *                 lines = make_roc_curve(&test[epoch].auc[kf], lines, "evaluation")
  *                 make_auc_curve(&test[epoch].auc[kf], &auc_ev)
  */
       }
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":396
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":399
  *                 make_auc_curve(&test[epoch].auc[kf], &auc_ev)
  * 
  *             for name in lines:             # <<<<<<<<<<<<<<
  *                 fname = name.split(" ")[2].replace(" ", "")
  *                 cls = name.split("-")[1].replace(" ", "")
  */
       __pyx_t_16 = 0;
       if (unlikely(__pyx_v_lines == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-        __PYX_ERR(0, 396, __pyx_L1_error)
+        __PYX_ERR(0, 399, __pyx_L1_error)
       }
-      __pyx_t_1 = __Pyx_dict_iterator(__pyx_v_lines, 1, ((PyObject *)NULL), (&__pyx_t_17), (&__pyx_t_11)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 396, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_dict_iterator(__pyx_v_lines, 1, ((PyObject *)NULL), (&__pyx_t_17), (&__pyx_t_11)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 399, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_XDECREF(__pyx_t_7);
       __pyx_t_7 = __pyx_t_1;
       __pyx_t_1 = 0;
       while (1) {
         __pyx_t_18 = __Pyx_dict_iter_next(__pyx_t_7, __pyx_t_17, &__pyx_t_16, &__pyx_t_1, NULL, NULL, __pyx_t_11);
         if (unlikely(__pyx_t_18 == 0)) break;
-        if (unlikely(__pyx_t_18 == -1)) __PYX_ERR(0, 396, __pyx_L1_error)
+        if (unlikely(__pyx_t_18 == -1)) __PYX_ERR(0, 399, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_XDECREF_SET(__pyx_v_name, __pyx_t_1);
         __pyx_t_1 = 0;
 
-        /* "src/cmodules/cyincludes/cyoptimizer.pyx":397
+        /* "src/cmodules/cyincludes/cyoptimizer.pyx":400
  * 
  *             for name in lines:
  *                 fname = name.split(" ")[2].replace(" ", "")             # <<<<<<<<<<<<<<
  *                 cls = name.split("-")[1].replace(" ", "")
  * 
  */
-        __pyx_t_19 = __Pyx_PyObject_GetAttrStr(__pyx_v_name, __pyx_n_s_split); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 397, __pyx_L1_error)
+        __pyx_t_19 = __Pyx_PyObject_GetAttrStr(__pyx_v_name, __pyx_n_s_split); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_19);
         __pyx_t_20 = NULL;
         __pyx_t_18 = 0;
         #if CYTHON_UNPACK_METHODS
         if (likely(PyMethod_Check(__pyx_t_19))) {
           __pyx_t_20 = PyMethod_GET_SELF(__pyx_t_19);
           if (likely(__pyx_t_20)) {
@@ -32657,38 +32675,38 @@
           }
         }
         #endif
         {
           PyObject *__pyx_callargs[2] = {__pyx_t_20, __pyx_kp_u__63};
           __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_19, __pyx_callargs+1-__pyx_t_18, 1+__pyx_t_18);
           __Pyx_XDECREF(__pyx_t_20); __pyx_t_20 = 0;
-          if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 397, __pyx_L1_error)
+          if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 400, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_1);
           __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
         }
-        __pyx_t_19 = __Pyx_GetItemInt(__pyx_t_1, 2, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 397, __pyx_L1_error)
+        __pyx_t_19 = __Pyx_GetItemInt(__pyx_t_1, 2, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_19);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_19, __pyx_n_s_replace); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 397, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_19, __pyx_n_s_replace); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
-        __pyx_t_19 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_tuple__64, NULL); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 397, __pyx_L1_error)
+        __pyx_t_19 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_tuple__64, NULL); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_19);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_XDECREF_SET(__pyx_v_fname, __pyx_t_19);
         __pyx_t_19 = 0;
 
-        /* "src/cmodules/cyincludes/cyoptimizer.pyx":398
+        /* "src/cmodules/cyincludes/cyoptimizer.pyx":401
  *             for name in lines:
  *                 fname = name.split(" ")[2].replace(" ", "")
  *                 cls = name.split("-")[1].replace(" ", "")             # <<<<<<<<<<<<<<
  * 
  *                 pth = path + "/ROC/Epoch-" + str(epoch) + "/classification-" + cls + "/kfold-" + str(kf)
  */
-        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_name, __pyx_n_s_split); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 398, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_name, __pyx_n_s_split); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 401, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         __pyx_t_20 = NULL;
         __pyx_t_18 = 0;
         #if CYTHON_UNPACK_METHODS
         if (likely(PyMethod_Check(__pyx_t_1))) {
           __pyx_t_20 = PyMethod_GET_SELF(__pyx_t_1);
           if (likely(__pyx_t_20)) {
@@ -32700,170 +32718,170 @@
           }
         }
         #endif
         {
           PyObject *__pyx_callargs[2] = {__pyx_t_20, __pyx_kp_u__65};
           __pyx_t_19 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_18, 1+__pyx_t_18);
           __Pyx_XDECREF(__pyx_t_20); __pyx_t_20 = 0;
-          if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 398, __pyx_L1_error)
+          if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 401, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_19);
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         }
-        __pyx_t_1 = __Pyx_GetItemInt(__pyx_t_19, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 398, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_GetItemInt(__pyx_t_19, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 401, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
-        __pyx_t_19 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_replace); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 398, __pyx_L1_error)
+        __pyx_t_19 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_replace); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 401, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_19);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-        __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_19, __pyx_tuple__64, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 398, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_19, __pyx_tuple__64, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 401, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
         __Pyx_XDECREF_SET(__pyx_v_cls, __pyx_t_1);
         __pyx_t_1 = 0;
 
-        /* "src/cmodules/cyincludes/cyoptimizer.pyx":400
+        /* "src/cmodules/cyincludes/cyoptimizer.pyx":403
  *                 cls = name.split("-")[1].replace(" ", "")
  * 
  *                 pth = path + "/ROC/Epoch-" + str(epoch) + "/classification-" + cls + "/kfold-" + str(kf)             # <<<<<<<<<<<<<<
  *                 tmpl = template_tline(pth, "False Positive Rate", "True Positive Rate", name + " @ Epoch: " + str(epoch))
  *                 tmpl["Filename"] = fname + "_epoch_" + str(epoch)
  */
-        __pyx_t_1 = __Pyx_PyUnicode_ConcatSafe(__pyx_v_path, __pyx_kp_u_ROC_Epoch); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 400, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyUnicode_ConcatSafe(__pyx_v_path, __pyx_kp_u_ROC_Epoch); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 403, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
-        __pyx_t_19 = __Pyx_PyInt_From_int(__pyx_v_epoch); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 400, __pyx_L1_error)
+        __pyx_t_19 = __Pyx_PyInt_From_int(__pyx_v_epoch); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 403, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_19);
-        __pyx_t_20 = __Pyx_PyObject_Str(__pyx_t_19); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 400, __pyx_L1_error)
+        __pyx_t_20 = __Pyx_PyObject_Str(__pyx_t_19); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 403, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_20);
         __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
-        __pyx_t_19 = PyNumber_Add(__pyx_t_1, __pyx_t_20); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 400, __pyx_L1_error)
+        __pyx_t_19 = PyNumber_Add(__pyx_t_1, __pyx_t_20); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 403, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_19);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
-        __pyx_t_20 = __Pyx_PyUnicode_ConcatInPlace(__pyx_t_19, __pyx_kp_u_classification_3); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 400, __pyx_L1_error)
+        __pyx_t_20 = __Pyx_PyUnicode_ConcatInPlace(__pyx_t_19, __pyx_kp_u_classification_3); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 403, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_20);
         __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
-        __pyx_t_19 = PyNumber_Add(__pyx_t_20, __pyx_v_cls); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 400, __pyx_L1_error)
+        __pyx_t_19 = PyNumber_Add(__pyx_t_20, __pyx_v_cls); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 403, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_19);
         __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
-        __pyx_t_20 = PyNumber_Add(__pyx_t_19, __pyx_kp_u_kfold); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 400, __pyx_L1_error)
+        __pyx_t_20 = PyNumber_Add(__pyx_t_19, __pyx_kp_u_kfold); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 403, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_20);
         __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
-        __pyx_t_19 = __Pyx_PyInt_From_int(__pyx_v_kf); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 400, __pyx_L1_error)
+        __pyx_t_19 = __Pyx_PyInt_From_int(__pyx_v_kf); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 403, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_19);
-        __pyx_t_1 = __Pyx_PyObject_Str(__pyx_t_19); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 400, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyObject_Str(__pyx_t_19); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 403, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
-        __pyx_t_19 = PyNumber_Add(__pyx_t_20, __pyx_t_1); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 400, __pyx_L1_error)
+        __pyx_t_19 = PyNumber_Add(__pyx_t_20, __pyx_t_1); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 403, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_19);
         __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_XDECREF_SET(__pyx_v_pth, __pyx_t_19);
         __pyx_t_19 = 0;
 
-        /* "src/cmodules/cyincludes/cyoptimizer.pyx":401
+        /* "src/cmodules/cyincludes/cyoptimizer.pyx":404
  * 
  *                 pth = path + "/ROC/Epoch-" + str(epoch) + "/classification-" + cls + "/kfold-" + str(kf)
  *                 tmpl = template_tline(pth, "False Positive Rate", "True Positive Rate", name + " @ Epoch: " + str(epoch))             # <<<<<<<<<<<<<<
  *                 tmpl["Filename"] = fname + "_epoch_" + str(epoch)
  *                 tmpl["Lines"] = lines[name]
  */
-        if (!(likely(PyUnicode_CheckExact(__pyx_v_pth))||((__pyx_v_pth) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_v_pth))) __PYX_ERR(0, 401, __pyx_L1_error)
-        __pyx_t_19 = PyNumber_Add(__pyx_v_name, __pyx_kp_u_Epoch_3); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 401, __pyx_L1_error)
+        if (!(likely(PyUnicode_CheckExact(__pyx_v_pth))||((__pyx_v_pth) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_v_pth))) __PYX_ERR(0, 404, __pyx_L1_error)
+        __pyx_t_19 = PyNumber_Add(__pyx_v_name, __pyx_kp_u_Epoch_3); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 404, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_19);
-        __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_epoch); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 401, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_epoch); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 404, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
-        __pyx_t_20 = __Pyx_PyObject_Str(__pyx_t_1); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 401, __pyx_L1_error)
+        __pyx_t_20 = __Pyx_PyObject_Str(__pyx_t_1); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 404, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_20);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-        __pyx_t_1 = PyNumber_Add(__pyx_t_19, __pyx_t_20); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 401, __pyx_L1_error)
+        __pyx_t_1 = PyNumber_Add(__pyx_t_19, __pyx_t_20); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 404, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
         __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
-        if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_t_1))) __PYX_ERR(0, 401, __pyx_L1_error)
-        __pyx_t_20 = __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_template_tline(((PyObject*)__pyx_v_pth), __pyx_kp_u_False_Positive_Rate, __pyx_kp_u_True_Positive_Rate, ((PyObject*)__pyx_t_1)); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 401, __pyx_L1_error)
+        if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_t_1))) __PYX_ERR(0, 404, __pyx_L1_error)
+        __pyx_t_20 = __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_template_tline(((PyObject*)__pyx_v_pth), __pyx_kp_u_False_Positive_Rate, __pyx_kp_u_True_Positive_Rate, ((PyObject*)__pyx_t_1)); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 404, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_20);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_XDECREF_SET(__pyx_v_tmpl, ((PyObject*)__pyx_t_20));
         __pyx_t_20 = 0;
 
-        /* "src/cmodules/cyincludes/cyoptimizer.pyx":402
+        /* "src/cmodules/cyincludes/cyoptimizer.pyx":405
  *                 pth = path + "/ROC/Epoch-" + str(epoch) + "/classification-" + cls + "/kfold-" + str(kf)
  *                 tmpl = template_tline(pth, "False Positive Rate", "True Positive Rate", name + " @ Epoch: " + str(epoch))
  *                 tmpl["Filename"] = fname + "_epoch_" + str(epoch)             # <<<<<<<<<<<<<<
  *                 tmpl["Lines"] = lines[name]
  *                 tl = TLine(**tmpl)
  */
-        __pyx_t_20 = PyNumber_Add(__pyx_v_fname, __pyx_n_u_epoch); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 402, __pyx_L1_error)
+        __pyx_t_20 = PyNumber_Add(__pyx_v_fname, __pyx_n_u_epoch); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 405, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_20);
-        __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_epoch); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 402, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_epoch); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 405, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
-        __pyx_t_19 = __Pyx_PyObject_Str(__pyx_t_1); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 402, __pyx_L1_error)
+        __pyx_t_19 = __Pyx_PyObject_Str(__pyx_t_1); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 405, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_19);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-        __pyx_t_1 = PyNumber_Add(__pyx_t_20, __pyx_t_19); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 402, __pyx_L1_error)
+        __pyx_t_1 = PyNumber_Add(__pyx_t_20, __pyx_t_19); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 405, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
         __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
         if (unlikely(__pyx_v_tmpl == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-          __PYX_ERR(0, 402, __pyx_L1_error)
+          __PYX_ERR(0, 405, __pyx_L1_error)
         }
-        if (unlikely((PyDict_SetItem(__pyx_v_tmpl, __pyx_n_u_Filename, __pyx_t_1) < 0))) __PYX_ERR(0, 402, __pyx_L1_error)
+        if (unlikely((PyDict_SetItem(__pyx_v_tmpl, __pyx_n_u_Filename, __pyx_t_1) < 0))) __PYX_ERR(0, 405, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-        /* "src/cmodules/cyincludes/cyoptimizer.pyx":403
+        /* "src/cmodules/cyincludes/cyoptimizer.pyx":406
  *                 tmpl = template_tline(pth, "False Positive Rate", "True Positive Rate", name + " @ Epoch: " + str(epoch))
  *                 tmpl["Filename"] = fname + "_epoch_" + str(epoch)
  *                 tmpl["Lines"] = lines[name]             # <<<<<<<<<<<<<<
  *                 tl = TLine(**tmpl)
  *                 tl.SaveFigure()
  */
         if (unlikely(__pyx_v_lines == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-          __PYX_ERR(0, 403, __pyx_L1_error)
+          __PYX_ERR(0, 406, __pyx_L1_error)
         }
-        __pyx_t_1 = __Pyx_PyDict_GetItem(__pyx_v_lines, __pyx_v_name); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 403, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyDict_GetItem(__pyx_v_lines, __pyx_v_name); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 406, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         if (unlikely(__pyx_v_tmpl == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-          __PYX_ERR(0, 403, __pyx_L1_error)
+          __PYX_ERR(0, 406, __pyx_L1_error)
         }
-        if (unlikely((PyDict_SetItem(__pyx_v_tmpl, __pyx_n_u_Lines, __pyx_t_1) < 0))) __PYX_ERR(0, 403, __pyx_L1_error)
+        if (unlikely((PyDict_SetItem(__pyx_v_tmpl, __pyx_n_u_Lines, __pyx_t_1) < 0))) __PYX_ERR(0, 406, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-        /* "src/cmodules/cyincludes/cyoptimizer.pyx":404
+        /* "src/cmodules/cyincludes/cyoptimizer.pyx":407
  *                 tmpl["Filename"] = fname + "_epoch_" + str(epoch)
  *                 tmpl["Lines"] = lines[name]
  *                 tl = TLine(**tmpl)             # <<<<<<<<<<<<<<
  *                 tl.SaveFigure()
  *                 del tl
  */
-        __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_TLine); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 404, __pyx_L1_error)
+        __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_TLine); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 407, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         if (unlikely(__pyx_v_tmpl == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "argument after ** must be a mapping, not NoneType");
-          __PYX_ERR(0, 404, __pyx_L1_error)
+          __PYX_ERR(0, 407, __pyx_L1_error)
         }
-        __pyx_t_19 = PyDict_Copy(__pyx_v_tmpl); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 404, __pyx_L1_error)
+        __pyx_t_19 = PyDict_Copy(__pyx_v_tmpl); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 407, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_19);
-        __pyx_t_20 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_19); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 404, __pyx_L1_error)
+        __pyx_t_20 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_19); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 407, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_20);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
         __pyx_v_tl = __pyx_t_20;
         __pyx_t_20 = 0;
 
-        /* "src/cmodules/cyincludes/cyoptimizer.pyx":405
+        /* "src/cmodules/cyincludes/cyoptimizer.pyx":408
  *                 tmpl["Lines"] = lines[name]
  *                 tl = TLine(**tmpl)
  *                 tl.SaveFigure()             # <<<<<<<<<<<<<<
  *                 del tl
  * 
  */
-        __pyx_t_19 = __Pyx_PyObject_GetAttrStr(__pyx_v_tl, __pyx_n_s_SaveFigure); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 405, __pyx_L1_error)
+        __pyx_t_19 = __Pyx_PyObject_GetAttrStr(__pyx_v_tl, __pyx_n_s_SaveFigure); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 408, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_19);
         __pyx_t_1 = NULL;
         __pyx_t_18 = 0;
         #if CYTHON_UNPACK_METHODS
         if (likely(PyMethod_Check(__pyx_t_19))) {
           __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_19);
           if (likely(__pyx_t_1)) {
@@ -32875,230 +32893,230 @@
           }
         }
         #endif
         {
           PyObject *__pyx_callargs[2] = {__pyx_t_1, NULL};
           __pyx_t_20 = __Pyx_PyObject_FastCall(__pyx_t_19, __pyx_callargs+1-__pyx_t_18, 0+__pyx_t_18);
           __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-          if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 405, __pyx_L1_error)
+          if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 408, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_20);
           __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
         }
         __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
 
-        /* "src/cmodules/cyincludes/cyoptimizer.pyx":406
+        /* "src/cmodules/cyincludes/cyoptimizer.pyx":409
  *                 tl = TLine(**tmpl)
  *                 tl.SaveFigure()
  *                 del tl             # <<<<<<<<<<<<<<
  * 
  *         line_auc = collapse_points(&auc_tr, epoch, line_auc, "training", state, "auc")
  */
         __Pyx_DECREF(__pyx_v_tl); __pyx_v_tl = 0;
       }
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":382
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":385
  * 
  *     for epoch in sorted(set(epochs)):
  *         for kf in sorted(set(folds)):             # <<<<<<<<<<<<<<
  *             lines = {}
  *             if train.count(epoch) and train[epoch].auc.count(kf):
  */
     }
     __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":408
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":411
  *                 del tl
  * 
  *         line_auc = collapse_points(&auc_tr, epoch, line_auc, "training", state, "auc")             # <<<<<<<<<<<<<<
  *         line_auc = collapse_points(&auc_va, epoch, line_auc, "validation", state, "auc")
  *         line_auc = collapse_points(&auc_ev, epoch, line_auc, "evaluation", state, "auc")
  */
-    __pyx_t_12 = __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_collapse_points((&__pyx_v_auc_tr), __pyx_v_epoch, __pyx_v_line_auc, __pyx_n_u_training, __pyx_v_state, __pyx_n_u_auc); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 408, __pyx_L1_error)
+    __pyx_t_12 = __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_collapse_points((&__pyx_v_auc_tr), __pyx_v_epoch, __pyx_v_line_auc, __pyx_n_u_training, __pyx_v_state, __pyx_n_u_auc); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 411, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_12);
     __Pyx_DECREF_SET(__pyx_v_line_auc, ((PyObject*)__pyx_t_12));
     __pyx_t_12 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":409
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":412
  * 
  *         line_auc = collapse_points(&auc_tr, epoch, line_auc, "training", state, "auc")
  *         line_auc = collapse_points(&auc_va, epoch, line_auc, "validation", state, "auc")             # <<<<<<<<<<<<<<
  *         line_auc = collapse_points(&auc_ev, epoch, line_auc, "evaluation", state, "auc")
  * 
  */
-    __pyx_t_12 = __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_collapse_points((&__pyx_v_auc_va), __pyx_v_epoch, __pyx_v_line_auc, __pyx_n_u_validation, __pyx_v_state, __pyx_n_u_auc); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 409, __pyx_L1_error)
+    __pyx_t_12 = __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_collapse_points((&__pyx_v_auc_va), __pyx_v_epoch, __pyx_v_line_auc, __pyx_n_u_validation, __pyx_v_state, __pyx_n_u_auc); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 412, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_12);
     __Pyx_DECREF_SET(__pyx_v_line_auc, ((PyObject*)__pyx_t_12));
     __pyx_t_12 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":410
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":413
  *         line_auc = collapse_points(&auc_tr, epoch, line_auc, "training", state, "auc")
  *         line_auc = collapse_points(&auc_va, epoch, line_auc, "validation", state, "auc")
  *         line_auc = collapse_points(&auc_ev, epoch, line_auc, "evaluation", state, "auc")             # <<<<<<<<<<<<<<
  * 
  *     for var_name in line_auc:
  */
-    __pyx_t_12 = __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_collapse_points((&__pyx_v_auc_ev), __pyx_v_epoch, __pyx_v_line_auc, __pyx_n_u_evaluation, __pyx_v_state, __pyx_n_u_auc); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 410, __pyx_L1_error)
+    __pyx_t_12 = __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_collapse_points((&__pyx_v_auc_ev), __pyx_v_epoch, __pyx_v_line_auc, __pyx_n_u_evaluation, __pyx_v_state, __pyx_n_u_auc); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 413, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_12);
     __Pyx_DECREF_SET(__pyx_v_line_auc, ((PyObject*)__pyx_t_12));
     __pyx_t_12 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":381
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":384
  *     cdef map[string, vector[point_t]] auc_ev
  * 
  *     for epoch in sorted(set(epochs)):             # <<<<<<<<<<<<<<
  *         for kf in sorted(set(folds)):
  *             lines = {}
  */
   }
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":412
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":415
  *         line_auc = collapse_points(&auc_ev, epoch, line_auc, "evaluation", state, "auc")
  * 
  *     for var_name in line_auc:             # <<<<<<<<<<<<<<
  *         for mode in line_auc[var_name]: line_auc[var_name][mode] = TLine(**line_auc[var_name][mode])
  *         pth = path + "/AUC/classification-" + var_name.split("-")[-1].replace(" ", "")
  */
   __pyx_t_10 = 0;
   if (unlikely(__pyx_v_line_auc == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-    __PYX_ERR(0, 412, __pyx_L1_error)
+    __PYX_ERR(0, 415, __pyx_L1_error)
   }
-  __pyx_t_12 = __Pyx_dict_iterator(__pyx_v_line_auc, 1, ((PyObject *)NULL), (&__pyx_t_13), (&__pyx_t_11)); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 412, __pyx_L1_error)
+  __pyx_t_12 = __Pyx_dict_iterator(__pyx_v_line_auc, 1, ((PyObject *)NULL), (&__pyx_t_13), (&__pyx_t_11)); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 415, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_12);
   __Pyx_XDECREF(__pyx_t_8);
   __pyx_t_8 = __pyx_t_12;
   __pyx_t_12 = 0;
   while (1) {
     __pyx_t_18 = __Pyx_dict_iter_next(__pyx_t_8, __pyx_t_13, &__pyx_t_10, &__pyx_t_12, NULL, NULL, __pyx_t_11);
     if (unlikely(__pyx_t_18 == 0)) break;
-    if (unlikely(__pyx_t_18 == -1)) __PYX_ERR(0, 412, __pyx_L1_error)
+    if (unlikely(__pyx_t_18 == -1)) __PYX_ERR(0, 415, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_12);
     __Pyx_XDECREF_SET(__pyx_v_var_name, __pyx_t_12);
     __pyx_t_12 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":413
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":416
  * 
  *     for var_name in line_auc:
  *         for mode in line_auc[var_name]: line_auc[var_name][mode] = TLine(**line_auc[var_name][mode])             # <<<<<<<<<<<<<<
  *         pth = path + "/AUC/classification-" + var_name.split("-")[-1].replace(" ", "")
  *         tmpl = template_tline(pth, "Epoch", "Area Under Curve", "Area Under Curve of MVA: " + var_name)
  */
     if (unlikely(__pyx_v_line_auc == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 413, __pyx_L1_error)
+      __PYX_ERR(0, 416, __pyx_L1_error)
     }
-    __pyx_t_12 = __Pyx_PyDict_GetItem(__pyx_v_line_auc, __pyx_v_var_name); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 413, __pyx_L1_error)
+    __pyx_t_12 = __Pyx_PyDict_GetItem(__pyx_v_line_auc, __pyx_v_var_name); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 416, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_12);
     if (likely(PyList_CheckExact(__pyx_t_12)) || PyTuple_CheckExact(__pyx_t_12)) {
       __pyx_t_7 = __pyx_t_12; __Pyx_INCREF(__pyx_t_7);
       __pyx_t_17 = 0;
       __pyx_t_21 = NULL;
     } else {
-      __pyx_t_17 = -1; __pyx_t_7 = PyObject_GetIter(__pyx_t_12); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 413, __pyx_L1_error)
+      __pyx_t_17 = -1; __pyx_t_7 = PyObject_GetIter(__pyx_t_12); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 416, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
-      __pyx_t_21 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_7); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 413, __pyx_L1_error)
+      __pyx_t_21 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_7); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 416, __pyx_L1_error)
     }
     __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
     for (;;) {
       if (likely(!__pyx_t_21)) {
         if (likely(PyList_CheckExact(__pyx_t_7))) {
           {
             Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_7);
             #if !CYTHON_ASSUME_SAFE_MACROS
-            if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 413, __pyx_L1_error)
+            if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 416, __pyx_L1_error)
             #endif
             if (__pyx_t_17 >= __pyx_temp) break;
           }
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_12 = PyList_GET_ITEM(__pyx_t_7, __pyx_t_17); __Pyx_INCREF(__pyx_t_12); __pyx_t_17++; if (unlikely((0 < 0))) __PYX_ERR(0, 413, __pyx_L1_error)
+          __pyx_t_12 = PyList_GET_ITEM(__pyx_t_7, __pyx_t_17); __Pyx_INCREF(__pyx_t_12); __pyx_t_17++; if (unlikely((0 < 0))) __PYX_ERR(0, 416, __pyx_L1_error)
           #else
-          __pyx_t_12 = __Pyx_PySequence_ITEM(__pyx_t_7, __pyx_t_17); __pyx_t_17++; if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 413, __pyx_L1_error)
+          __pyx_t_12 = __Pyx_PySequence_ITEM(__pyx_t_7, __pyx_t_17); __pyx_t_17++; if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 416, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_12);
           #endif
         } else {
           {
             Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_7);
             #if !CYTHON_ASSUME_SAFE_MACROS
-            if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 413, __pyx_L1_error)
+            if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 416, __pyx_L1_error)
             #endif
             if (__pyx_t_17 >= __pyx_temp) break;
           }
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_12 = PyTuple_GET_ITEM(__pyx_t_7, __pyx_t_17); __Pyx_INCREF(__pyx_t_12); __pyx_t_17++; if (unlikely((0 < 0))) __PYX_ERR(0, 413, __pyx_L1_error)
+          __pyx_t_12 = PyTuple_GET_ITEM(__pyx_t_7, __pyx_t_17); __Pyx_INCREF(__pyx_t_12); __pyx_t_17++; if (unlikely((0 < 0))) __PYX_ERR(0, 416, __pyx_L1_error)
           #else
-          __pyx_t_12 = __Pyx_PySequence_ITEM(__pyx_t_7, __pyx_t_17); __pyx_t_17++; if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 413, __pyx_L1_error)
+          __pyx_t_12 = __Pyx_PySequence_ITEM(__pyx_t_7, __pyx_t_17); __pyx_t_17++; if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 416, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_12);
           #endif
         }
       } else {
         __pyx_t_12 = __pyx_t_21(__pyx_t_7);
         if (unlikely(!__pyx_t_12)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 413, __pyx_L1_error)
+            else __PYX_ERR(0, 416, __pyx_L1_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_12);
       }
       __Pyx_XDECREF_SET(__pyx_v_mode, __pyx_t_12);
       __pyx_t_12 = 0;
-      __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_TLine); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 413, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_TLine); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 416, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_12);
       if (unlikely(__pyx_v_line_auc == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-        __PYX_ERR(0, 413, __pyx_L1_error)
+        __PYX_ERR(0, 416, __pyx_L1_error)
       }
-      __pyx_t_19 = __Pyx_PyDict_GetItem(__pyx_v_line_auc, __pyx_v_var_name); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 413, __pyx_L1_error)
+      __pyx_t_19 = __Pyx_PyDict_GetItem(__pyx_v_line_auc, __pyx_v_var_name); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 416, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_19);
-      __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_t_19, __pyx_v_mode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 413, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_t_19, __pyx_v_mode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 416, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
       if (unlikely(__pyx_t_1 == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "argument after ** must be a mapping, not NoneType");
-        __PYX_ERR(0, 413, __pyx_L1_error)
+        __PYX_ERR(0, 416, __pyx_L1_error)
       }
       if (likely(PyDict_CheckExact(__pyx_t_1))) {
-        __pyx_t_20 = PyDict_Copy(__pyx_t_1); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 413, __pyx_L1_error)
+        __pyx_t_20 = PyDict_Copy(__pyx_t_1); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 416, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_20);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       } else {
-        __pyx_t_20 = __Pyx_PyObject_CallOneArg((PyObject*)&PyDict_Type, __pyx_t_1); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 413, __pyx_L1_error)
+        __pyx_t_20 = __Pyx_PyObject_CallOneArg((PyObject*)&PyDict_Type, __pyx_t_1); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 416, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_20);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       }
-      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_12, __pyx_empty_tuple, __pyx_t_20); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 413, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_12, __pyx_empty_tuple, __pyx_t_20); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 416, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
       __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
       if (unlikely(__pyx_v_line_auc == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-        __PYX_ERR(0, 413, __pyx_L1_error)
+        __PYX_ERR(0, 416, __pyx_L1_error)
       }
-      __pyx_t_20 = __Pyx_PyDict_GetItem(__pyx_v_line_auc, __pyx_v_var_name); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 413, __pyx_L1_error)
+      __pyx_t_20 = __Pyx_PyDict_GetItem(__pyx_v_line_auc, __pyx_v_var_name); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 416, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_20);
-      if (unlikely((PyObject_SetItem(__pyx_t_20, __pyx_v_mode, __pyx_t_1) < 0))) __PYX_ERR(0, 413, __pyx_L1_error)
+      if (unlikely((PyObject_SetItem(__pyx_t_20, __pyx_v_mode, __pyx_t_1) < 0))) __PYX_ERR(0, 416, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     }
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":414
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":417
  *     for var_name in line_auc:
  *         for mode in line_auc[var_name]: line_auc[var_name][mode] = TLine(**line_auc[var_name][mode])
  *         pth = path + "/AUC/classification-" + var_name.split("-")[-1].replace(" ", "")             # <<<<<<<<<<<<<<
  *         tmpl = template_tline(pth, "Epoch", "Area Under Curve", "Area Under Curve of MVA: " + var_name)
  *         tmpl["Filename"] = var_name.split(" ")[0]
  */
-    __pyx_t_7 = __Pyx_PyUnicode_ConcatSafe(__pyx_v_path, __pyx_kp_u_AUC_classification); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 414, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyUnicode_ConcatSafe(__pyx_v_path, __pyx_kp_u_AUC_classification); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 417, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_20 = __Pyx_PyObject_GetAttrStr(__pyx_v_var_name, __pyx_n_s_split); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 414, __pyx_L1_error)
+    __pyx_t_20 = __Pyx_PyObject_GetAttrStr(__pyx_v_var_name, __pyx_n_s_split); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 417, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_20);
     __pyx_t_12 = NULL;
     __pyx_t_18 = 0;
     #if CYTHON_UNPACK_METHODS
     if (likely(PyMethod_Check(__pyx_t_20))) {
       __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_20);
       if (likely(__pyx_t_12)) {
@@ -33110,59 +33128,59 @@
       }
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_12, __pyx_kp_u__65};
       __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_20, __pyx_callargs+1-__pyx_t_18, 1+__pyx_t_18);
       __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 414, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 417, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
     }
-    __pyx_t_20 = __Pyx_GetItemInt(__pyx_t_1, -1L, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 414, __pyx_L1_error)
+    __pyx_t_20 = __Pyx_GetItemInt(__pyx_t_1, -1L, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 417, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_20);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_20, __pyx_n_s_replace); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 414, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_20, __pyx_n_s_replace); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 417, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
-    __pyx_t_20 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_tuple__64, NULL); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 414, __pyx_L1_error)
+    __pyx_t_20 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_tuple__64, NULL); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 417, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_20);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = PyNumber_Add(__pyx_t_7, __pyx_t_20); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 414, __pyx_L1_error)
+    __pyx_t_1 = PyNumber_Add(__pyx_t_7, __pyx_t_20); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 417, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
     __Pyx_XDECREF_SET(__pyx_v_pth, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":415
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":418
  *         for mode in line_auc[var_name]: line_auc[var_name][mode] = TLine(**line_auc[var_name][mode])
  *         pth = path + "/AUC/classification-" + var_name.split("-")[-1].replace(" ", "")
  *         tmpl = template_tline(pth, "Epoch", "Area Under Curve", "Area Under Curve of MVA: " + var_name)             # <<<<<<<<<<<<<<
  *         tmpl["Filename"] = var_name.split(" ")[0]
  *         tmpl["Lines"] = list(line_auc[var_name].values())
  */
-    if (!(likely(PyUnicode_CheckExact(__pyx_v_pth))||((__pyx_v_pth) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_v_pth))) __PYX_ERR(0, 415, __pyx_L1_error)
-    __pyx_t_1 = PyNumber_Add(__pyx_kp_u_Area_Under_Curve_of_MVA, __pyx_v_var_name); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 415, __pyx_L1_error)
+    if (!(likely(PyUnicode_CheckExact(__pyx_v_pth))||((__pyx_v_pth) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_v_pth))) __PYX_ERR(0, 418, __pyx_L1_error)
+    __pyx_t_1 = PyNumber_Add(__pyx_kp_u_Area_Under_Curve_of_MVA, __pyx_v_var_name); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 418, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_t_1))) __PYX_ERR(0, 415, __pyx_L1_error)
-    __pyx_t_20 = __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_template_tline(((PyObject*)__pyx_v_pth), __pyx_n_u_Epoch_2, __pyx_kp_u_Area_Under_Curve, ((PyObject*)__pyx_t_1)); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 415, __pyx_L1_error)
+    if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_t_1))) __PYX_ERR(0, 418, __pyx_L1_error)
+    __pyx_t_20 = __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_template_tline(((PyObject*)__pyx_v_pth), __pyx_n_u_Epoch_2, __pyx_kp_u_Area_Under_Curve, ((PyObject*)__pyx_t_1)); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 418, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_20);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF_SET(__pyx_v_tmpl, ((PyObject*)__pyx_t_20));
     __pyx_t_20 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":416
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":419
  *         pth = path + "/AUC/classification-" + var_name.split("-")[-1].replace(" ", "")
  *         tmpl = template_tline(pth, "Epoch", "Area Under Curve", "Area Under Curve of MVA: " + var_name)
  *         tmpl["Filename"] = var_name.split(" ")[0]             # <<<<<<<<<<<<<<
  *         tmpl["Lines"] = list(line_auc[var_name].values())
  * 
  */
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_var_name, __pyx_n_s_split); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 416, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_var_name, __pyx_n_s_split); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 419, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_7 = NULL;
     __pyx_t_18 = 0;
     #if CYTHON_UNPACK_METHODS
     if (likely(PyMethod_Check(__pyx_t_1))) {
       __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_1);
       if (likely(__pyx_t_7)) {
@@ -33174,42 +33192,42 @@
       }
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_7, __pyx_kp_u__63};
       __pyx_t_20 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_18, 1+__pyx_t_18);
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-      if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 416, __pyx_L1_error)
+      if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 419, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_20);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     }
-    __pyx_t_1 = __Pyx_GetItemInt(__pyx_t_20, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 416, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_GetItemInt(__pyx_t_20, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 419, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
     if (unlikely(__pyx_v_tmpl == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 416, __pyx_L1_error)
+      __PYX_ERR(0, 419, __pyx_L1_error)
     }
-    if (unlikely((PyDict_SetItem(__pyx_v_tmpl, __pyx_n_u_Filename, __pyx_t_1) < 0))) __PYX_ERR(0, 416, __pyx_L1_error)
+    if (unlikely((PyDict_SetItem(__pyx_v_tmpl, __pyx_n_u_Filename, __pyx_t_1) < 0))) __PYX_ERR(0, 419, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":417
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":420
  *         tmpl = template_tline(pth, "Epoch", "Area Under Curve", "Area Under Curve of MVA: " + var_name)
  *         tmpl["Filename"] = var_name.split(" ")[0]
  *         tmpl["Lines"] = list(line_auc[var_name].values())             # <<<<<<<<<<<<<<
  * 
  *         tl = TLine(**tmpl)
  */
     if (unlikely(__pyx_v_line_auc == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 417, __pyx_L1_error)
+      __PYX_ERR(0, 420, __pyx_L1_error)
     }
-    __pyx_t_20 = __Pyx_PyDict_GetItem(__pyx_v_line_auc, __pyx_v_var_name); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 417, __pyx_L1_error)
+    __pyx_t_20 = __Pyx_PyDict_GetItem(__pyx_v_line_auc, __pyx_v_var_name); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 420, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_20);
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_20, __pyx_n_s_values); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 417, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_20, __pyx_n_s_values); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 420, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
     __pyx_t_20 = NULL;
     __pyx_t_18 = 0;
     #if CYTHON_UNPACK_METHODS
     if (likely(PyMethod_Check(__pyx_t_7))) {
       __pyx_t_20 = PyMethod_GET_SELF(__pyx_t_7);
@@ -33222,58 +33240,58 @@
       }
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_20, NULL};
       __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_7, __pyx_callargs+1-__pyx_t_18, 0+__pyx_t_18);
       __Pyx_XDECREF(__pyx_t_20); __pyx_t_20 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 417, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 420, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     }
-    __pyx_t_7 = __Pyx_PySequence_ListKeepNew(__pyx_t_1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 417, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PySequence_ListKeepNew(__pyx_t_1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 420, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     if (unlikely(__pyx_v_tmpl == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 417, __pyx_L1_error)
+      __PYX_ERR(0, 420, __pyx_L1_error)
     }
-    if (unlikely((PyDict_SetItem(__pyx_v_tmpl, __pyx_n_u_Lines, __pyx_t_7) < 0))) __PYX_ERR(0, 417, __pyx_L1_error)
+    if (unlikely((PyDict_SetItem(__pyx_v_tmpl, __pyx_n_u_Lines, __pyx_t_7) < 0))) __PYX_ERR(0, 420, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":419
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":422
  *         tmpl["Lines"] = list(line_auc[var_name].values())
  * 
  *         tl = TLine(**tmpl)             # <<<<<<<<<<<<<<
  *         tl.SaveFigure()
  *         del tl
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_TLine); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 419, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_TLine); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 422, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     if (unlikely(__pyx_v_tmpl == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "argument after ** must be a mapping, not NoneType");
-      __PYX_ERR(0, 419, __pyx_L1_error)
+      __PYX_ERR(0, 422, __pyx_L1_error)
     }
-    __pyx_t_1 = PyDict_Copy(__pyx_v_tmpl); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 419, __pyx_L1_error)
+    __pyx_t_1 = PyDict_Copy(__pyx_v_tmpl); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 422, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_20 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_empty_tuple, __pyx_t_1); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 419, __pyx_L1_error)
+    __pyx_t_20 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_empty_tuple, __pyx_t_1); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 422, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_20);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_v_tl = __pyx_t_20;
     __pyx_t_20 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":420
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":423
  * 
  *         tl = TLine(**tmpl)
  *         tl.SaveFigure()             # <<<<<<<<<<<<<<
  *         del tl
  *     del line_auc
  */
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_tl, __pyx_n_s_SaveFigure); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 420, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_tl, __pyx_n_s_SaveFigure); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 423, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_7 = NULL;
     __pyx_t_18 = 0;
     #if CYTHON_UNPACK_METHODS
     if (likely(PyMethod_Check(__pyx_t_1))) {
       __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_1);
       if (likely(__pyx_t_7)) {
@@ -33285,41 +33303,41 @@
       }
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_7, NULL};
       __pyx_t_20 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_18, 0+__pyx_t_18);
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-      if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 420, __pyx_L1_error)
+      if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 423, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_20);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     }
     __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":421
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":424
  *         tl = TLine(**tmpl)
  *         tl.SaveFigure()
  *         del tl             # <<<<<<<<<<<<<<
  *     del line_auc
  * 
  */
     __Pyx_DECREF(__pyx_v_tl); __pyx_v_tl = 0;
   }
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":422
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":425
  *         tl.SaveFigure()
  *         del tl
  *     del line_auc             # <<<<<<<<<<<<<<
  * 
  * cdef void make_nodes(map[int, CyEpoch*] train, map[int, CyEpoch*] valid, map[int, CyEpoch*] test, str path):
  */
   __Pyx_DECREF(__pyx_v_line_auc); __pyx_v_line_auc = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":351
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":354
  * 
  * 
  * cdef void make_roc_plots(map[int, CyEpoch*] train, map[int, CyEpoch*] valid, map[int, CyEpoch*] test, str path, report_t* state):             # <<<<<<<<<<<<<<
  *     cdef pair[int, CyEpoch*] itr
  * 
  */
 
@@ -33348,15 +33366,15 @@
   __Pyx_XDECREF(__pyx_v_tmpl);
   __Pyx_XDECREF(__pyx_v_tl);
   __Pyx_XDECREF(__pyx_v_var_name);
   __Pyx_XDECREF(__pyx_v_mode);
   __Pyx_RefNannyFinishContext();
 }
 
-/* "src/cmodules/cyincludes/cyoptimizer.pyx":424
+/* "src/cmodules/cyincludes/cyoptimizer.pyx":427
  *     del line_auc
  * 
  * cdef void make_nodes(map[int, CyEpoch*] train, map[int, CyEpoch*] valid, map[int, CyEpoch*] test, str path):             # <<<<<<<<<<<<<<
  *     cdef pair[int, CyEpoch*] its
  *     cdef pair[int, node_t] nd
  */
 
@@ -33394,877 +33412,877 @@
   int __pyx_t_16;
   PyObject *__pyx_t_17 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("make_nodes", 1);
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":428
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":431
  *     cdef pair[int, node_t] nd
  *     cdef dict hist = {
  *             "training"  : {"xData" : [], "Title" : "training"},             # <<<<<<<<<<<<<<
  *             "validation": {"xData" : [], "Title" : "validation"},
  *             "evaluation": {"xData" : [], "Title" : "evaluation"}
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 428, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 431, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 428, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 431, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 428, __pyx_L1_error)
+  __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 431, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_xData, __pyx_t_3) < 0) __PYX_ERR(0, 428, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_xData, __pyx_t_3) < 0) __PYX_ERR(0, 431, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_Title, __pyx_n_u_training) < 0) __PYX_ERR(0, 428, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_training, __pyx_t_2) < 0) __PYX_ERR(0, 428, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_Title, __pyx_n_u_training) < 0) __PYX_ERR(0, 431, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_training, __pyx_t_2) < 0) __PYX_ERR(0, 431, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":429
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":432
  *     cdef dict hist = {
  *             "training"  : {"xData" : [], "Title" : "training"},
  *             "validation": {"xData" : [], "Title" : "validation"},             # <<<<<<<<<<<<<<
  *             "evaluation": {"xData" : [], "Title" : "evaluation"}
  *     }
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 429, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 432, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 429, __pyx_L1_error)
+  __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 432, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_xData, __pyx_t_3) < 0) __PYX_ERR(0, 429, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_xData, __pyx_t_3) < 0) __PYX_ERR(0, 432, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_Title, __pyx_n_u_validation) < 0) __PYX_ERR(0, 429, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_validation, __pyx_t_2) < 0) __PYX_ERR(0, 428, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_Title, __pyx_n_u_validation) < 0) __PYX_ERR(0, 432, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_validation, __pyx_t_2) < 0) __PYX_ERR(0, 431, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":430
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":433
  *             "training"  : {"xData" : [], "Title" : "training"},
  *             "validation": {"xData" : [], "Title" : "validation"},
  *             "evaluation": {"xData" : [], "Title" : "evaluation"}             # <<<<<<<<<<<<<<
  *     }
  * 
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 430, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 433, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 430, __pyx_L1_error)
+  __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 433, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_xData, __pyx_t_3) < 0) __PYX_ERR(0, 430, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_xData, __pyx_t_3) < 0) __PYX_ERR(0, 433, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_Title, __pyx_n_u_evaluation) < 0) __PYX_ERR(0, 430, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_evaluation, __pyx_t_2) < 0) __PYX_ERR(0, 428, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_Title, __pyx_n_u_evaluation) < 0) __PYX_ERR(0, 433, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_evaluation, __pyx_t_2) < 0) __PYX_ERR(0, 431, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_hist = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":433
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":436
  *     }
  * 
  *     cdef int mx_ = 0             # <<<<<<<<<<<<<<
  *     for its in train:
  *         for nd in its.second.nodes:
  */
   __pyx_v_mx_ = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":434
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":437
  * 
  *     cdef int mx_ = 0
  *     for its in train:             # <<<<<<<<<<<<<<
  *         for nd in its.second.nodes:
  *             hist["training"]["xData"] += sum([[i]*j for i, j in dict(nd.second.num_nodes).items()], [])
  */
   __pyx_t_4 = __pyx_v_train.begin();
   for (;;) {
     if (!(__pyx_t_4 != __pyx_v_train.end())) break;
     __pyx_t_5 = *__pyx_t_4;
     ++__pyx_t_4;
     __pyx_v_its = __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_5);
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":435
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":438
  *     cdef int mx_ = 0
  *     for its in train:
  *         for nd in its.second.nodes:             # <<<<<<<<<<<<<<
  *             hist["training"]["xData"] += sum([[i]*j for i, j in dict(nd.second.num_nodes).items()], [])
  *             m = max(hist["training"]["xData"])
  */
     __pyx_t_6 = __pyx_v_its.second->nodes.begin();
     for (;;) {
       if (!(__pyx_t_6 != __pyx_v_its.second->nodes.end())) break;
       __pyx_t_7 = *__pyx_t_6;
       ++__pyx_t_6;
       __pyx_v_nd = __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_7);
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":436
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":439
  *     for its in train:
  *         for nd in its.second.nodes:
  *             hist["training"]["xData"] += sum([[i]*j for i, j in dict(nd.second.num_nodes).items()], [])             # <<<<<<<<<<<<<<
  *             m = max(hist["training"]["xData"])
  *             if m > mx_: mx_ = m
  */
-      __pyx_t_1 = __Pyx_PyDict_GetItem(__pyx_v_hist, __pyx_n_u_training); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 436, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyDict_GetItem(__pyx_v_hist, __pyx_n_u_training); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 439, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_INCREF(__pyx_n_u_xData);
       __pyx_t_8 = __pyx_n_u_xData;
-      __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_t_1, __pyx_t_8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 436, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_t_1, __pyx_t_8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 439, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       { /* enter inner scope */
-        __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 436, __pyx_L9_error)
+        __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 439, __pyx_L9_error)
         __Pyx_GOTREF(__pyx_t_3);
         __pyx_t_10 = 0;
-        __pyx_t_13 = __pyx_convert_map_to_py_int____int(__pyx_v_nd.second.num_nodes); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 436, __pyx_L9_error)
+        __pyx_t_13 = __pyx_convert_map_to_py_int____int(__pyx_v_nd.second.num_nodes); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 439, __pyx_L9_error)
         __Pyx_GOTREF(__pyx_t_13);
-        __pyx_t_14 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyDict_Type)), __pyx_t_13); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 436, __pyx_L9_error)
+        __pyx_t_14 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyDict_Type)), __pyx_t_13); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 439, __pyx_L9_error)
         __Pyx_GOTREF(__pyx_t_14);
         __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
-        __pyx_t_13 = __Pyx_dict_iterator(__pyx_t_14, 1, __pyx_n_s_items, (&__pyx_t_11), (&__pyx_t_12)); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 436, __pyx_L9_error)
+        __pyx_t_13 = __Pyx_dict_iterator(__pyx_t_14, 1, __pyx_n_s_items, (&__pyx_t_11), (&__pyx_t_12)); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 439, __pyx_L9_error)
         __Pyx_GOTREF(__pyx_t_13);
         __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
         __Pyx_XDECREF(__pyx_t_9);
         __pyx_t_9 = __pyx_t_13;
         __pyx_t_13 = 0;
         while (1) {
           __pyx_t_15 = __Pyx_dict_iter_next(__pyx_t_9, __pyx_t_11, &__pyx_t_10, &__pyx_t_13, &__pyx_t_14, NULL, __pyx_t_12);
           if (unlikely(__pyx_t_15 == 0)) break;
-          if (unlikely(__pyx_t_15 == -1)) __PYX_ERR(0, 436, __pyx_L9_error)
+          if (unlikely(__pyx_t_15 == -1)) __PYX_ERR(0, 439, __pyx_L9_error)
           __Pyx_GOTREF(__pyx_t_13);
           __Pyx_GOTREF(__pyx_t_14);
           __Pyx_XDECREF_SET(__pyx_8genexpr3__pyx_v_i, __pyx_t_13);
           __pyx_t_13 = 0;
           __Pyx_XDECREF_SET(__pyx_8genexpr3__pyx_v_j, __pyx_t_14);
           __pyx_t_14 = 0;
-          __pyx_t_14 = PyList_New(1); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 436, __pyx_L9_error)
+          __pyx_t_14 = PyList_New(1); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 439, __pyx_L9_error)
           __Pyx_GOTREF(__pyx_t_14);
           __Pyx_INCREF(__pyx_8genexpr3__pyx_v_i);
           __Pyx_GIVEREF(__pyx_8genexpr3__pyx_v_i);
-          if (__Pyx_PyList_SET_ITEM(__pyx_t_14, 0, __pyx_8genexpr3__pyx_v_i)) __PYX_ERR(0, 436, __pyx_L9_error);
-          { PyObject* __pyx_temp = PyNumber_InPlaceMultiply(__pyx_t_14, __pyx_8genexpr3__pyx_v_j); if (unlikely(!__pyx_temp)) __PYX_ERR(0, 436, __pyx_L9_error)
+          if (__Pyx_PyList_SET_ITEM(__pyx_t_14, 0, __pyx_8genexpr3__pyx_v_i)) __PYX_ERR(0, 439, __pyx_L9_error);
+          { PyObject* __pyx_temp = PyNumber_InPlaceMultiply(__pyx_t_14, __pyx_8genexpr3__pyx_v_j); if (unlikely(!__pyx_temp)) __PYX_ERR(0, 439, __pyx_L9_error)
             __Pyx_GOTREF(__pyx_temp);
             __Pyx_DECREF(__pyx_t_14);
             __pyx_t_14 = __pyx_temp;
           }
-          if (unlikely(__Pyx_ListComp_Append(__pyx_t_3, (PyObject*)__pyx_t_14))) __PYX_ERR(0, 436, __pyx_L9_error)
+          if (unlikely(__Pyx_ListComp_Append(__pyx_t_3, (PyObject*)__pyx_t_14))) __PYX_ERR(0, 439, __pyx_L9_error)
           __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
         }
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
         __Pyx_XDECREF(__pyx_8genexpr3__pyx_v_i); __pyx_8genexpr3__pyx_v_i = 0;
         __Pyx_XDECREF(__pyx_8genexpr3__pyx_v_j); __pyx_8genexpr3__pyx_v_j = 0;
         goto __pyx_L12_exit_scope;
         __pyx_L9_error:;
         __Pyx_XDECREF(__pyx_8genexpr3__pyx_v_i); __pyx_8genexpr3__pyx_v_i = 0;
         __Pyx_XDECREF(__pyx_8genexpr3__pyx_v_j); __pyx_8genexpr3__pyx_v_j = 0;
         goto __pyx_L1_error;
         __pyx_L12_exit_scope:;
       } /* exit inner scope */
-      __pyx_t_9 = PyList_New(0); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 436, __pyx_L1_error)
+      __pyx_t_9 = PyList_New(0); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 439, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
-      __pyx_t_14 = PyTuple_New(2); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 436, __pyx_L1_error)
+      __pyx_t_14 = PyTuple_New(2); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 439, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_14);
       __Pyx_GIVEREF(__pyx_t_3);
-      if (__Pyx_PyTuple_SET_ITEM(__pyx_t_14, 0, __pyx_t_3)) __PYX_ERR(0, 436, __pyx_L1_error);
+      if (__Pyx_PyTuple_SET_ITEM(__pyx_t_14, 0, __pyx_t_3)) __PYX_ERR(0, 439, __pyx_L1_error);
       __Pyx_GIVEREF(__pyx_t_9);
-      if (__Pyx_PyTuple_SET_ITEM(__pyx_t_14, 1, __pyx_t_9)) __PYX_ERR(0, 436, __pyx_L1_error);
+      if (__Pyx_PyTuple_SET_ITEM(__pyx_t_14, 1, __pyx_t_9)) __PYX_ERR(0, 439, __pyx_L1_error);
       __pyx_t_3 = 0;
       __pyx_t_9 = 0;
-      __pyx_t_9 = __Pyx_PyObject_Call(__pyx_builtin_sum, __pyx_t_14, NULL); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 436, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyObject_Call(__pyx_builtin_sum, __pyx_t_14, NULL); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 439, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
       __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
-      __pyx_t_14 = PyNumber_InPlaceAdd(__pyx_t_2, __pyx_t_9); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 436, __pyx_L1_error)
+      __pyx_t_14 = PyNumber_InPlaceAdd(__pyx_t_2, __pyx_t_9); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 439, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_14);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-      if (unlikely((PyObject_SetItem(__pyx_t_1, __pyx_t_8, __pyx_t_14) < 0))) __PYX_ERR(0, 436, __pyx_L1_error)
+      if (unlikely((PyObject_SetItem(__pyx_t_1, __pyx_t_8, __pyx_t_14) < 0))) __PYX_ERR(0, 439, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":437
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":440
  *         for nd in its.second.nodes:
  *             hist["training"]["xData"] += sum([[i]*j for i, j in dict(nd.second.num_nodes).items()], [])
  *             m = max(hist["training"]["xData"])             # <<<<<<<<<<<<<<
  *             if m > mx_: mx_ = m
  *         break
  */
-      __pyx_t_1 = __Pyx_PyDict_GetItem(__pyx_v_hist, __pyx_n_u_training); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 437, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyDict_GetItem(__pyx_v_hist, __pyx_n_u_training); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 440, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_14 = __Pyx_PyObject_Dict_GetItem(__pyx_t_1, __pyx_n_u_xData); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 437, __pyx_L1_error)
+      __pyx_t_14 = __Pyx_PyObject_Dict_GetItem(__pyx_t_1, __pyx_n_u_xData); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 440, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_14);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_max, __pyx_t_14); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 437, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_max, __pyx_t_14); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 440, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
       __Pyx_XDECREF_SET(__pyx_v_m, __pyx_t_1);
       __pyx_t_1 = 0;
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":438
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":441
  *             hist["training"]["xData"] += sum([[i]*j for i, j in dict(nd.second.num_nodes).items()], [])
  *             m = max(hist["training"]["xData"])
  *             if m > mx_: mx_ = m             # <<<<<<<<<<<<<<
  *         break
  * 
  */
-      __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_mx_); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 438, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_mx_); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 441, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_14 = PyObject_RichCompare(__pyx_v_m, __pyx_t_1, Py_GT); __Pyx_XGOTREF(__pyx_t_14); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 438, __pyx_L1_error)
+      __pyx_t_14 = PyObject_RichCompare(__pyx_v_m, __pyx_t_1, Py_GT); __Pyx_XGOTREF(__pyx_t_14); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 441, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_t_16 = __Pyx_PyObject_IsTrue(__pyx_t_14); if (unlikely((__pyx_t_16 < 0))) __PYX_ERR(0, 438, __pyx_L1_error)
+      __pyx_t_16 = __Pyx_PyObject_IsTrue(__pyx_t_14); if (unlikely((__pyx_t_16 < 0))) __PYX_ERR(0, 441, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
       if (__pyx_t_16) {
-        __pyx_t_12 = __Pyx_PyInt_As_int(__pyx_v_m); if (unlikely((__pyx_t_12 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 438, __pyx_L1_error)
+        __pyx_t_12 = __Pyx_PyInt_As_int(__pyx_v_m); if (unlikely((__pyx_t_12 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 441, __pyx_L1_error)
         __pyx_v_mx_ = __pyx_t_12;
       }
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":435
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":438
  *     cdef int mx_ = 0
  *     for its in train:
  *         for nd in its.second.nodes:             # <<<<<<<<<<<<<<
  *             hist["training"]["xData"] += sum([[i]*j for i, j in dict(nd.second.num_nodes).items()], [])
  *             m = max(hist["training"]["xData"])
  */
     }
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":439
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":442
  *             m = max(hist["training"]["xData"])
  *             if m > mx_: mx_ = m
  *         break             # <<<<<<<<<<<<<<
  * 
  *     for its in valid:
  */
     goto __pyx_L4_break;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":434
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":437
  * 
  *     cdef int mx_ = 0
  *     for its in train:             # <<<<<<<<<<<<<<
  *         for nd in its.second.nodes:
  *             hist["training"]["xData"] += sum([[i]*j for i, j in dict(nd.second.num_nodes).items()], [])
  */
   }
   goto __pyx_L15_for_end;
   __pyx_L4_break:;
   goto __pyx_L15_for_end;
   __pyx_L15_for_end:;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":441
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":444
  *         break
  * 
  *     for its in valid:             # <<<<<<<<<<<<<<
  *         for nd in its.second.nodes:
  *             hist["validation"]["xData"] += sum([[i]*j for i, j in dict(nd.second.num_nodes).items()], [])
  */
   __pyx_t_4 = __pyx_v_valid.begin();
   for (;;) {
     if (!(__pyx_t_4 != __pyx_v_valid.end())) break;
     __pyx_t_5 = *__pyx_t_4;
     ++__pyx_t_4;
     __pyx_v_its = __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_5);
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":442
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":445
  * 
  *     for its in valid:
  *         for nd in its.second.nodes:             # <<<<<<<<<<<<<<
  *             hist["validation"]["xData"] += sum([[i]*j for i, j in dict(nd.second.num_nodes).items()], [])
  *             m = max(hist["validation"]["xData"])
  */
     __pyx_t_6 = __pyx_v_its.second->nodes.begin();
     for (;;) {
       if (!(__pyx_t_6 != __pyx_v_its.second->nodes.end())) break;
       __pyx_t_7 = *__pyx_t_6;
       ++__pyx_t_6;
       __pyx_v_nd = __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_7);
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":443
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":446
  *     for its in valid:
  *         for nd in its.second.nodes:
  *             hist["validation"]["xData"] += sum([[i]*j for i, j in dict(nd.second.num_nodes).items()], [])             # <<<<<<<<<<<<<<
  *             m = max(hist["validation"]["xData"])
  *             if m > mx_: mx_ = m
  */
-      __pyx_t_14 = __Pyx_PyDict_GetItem(__pyx_v_hist, __pyx_n_u_validation); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 443, __pyx_L1_error)
+      __pyx_t_14 = __Pyx_PyDict_GetItem(__pyx_v_hist, __pyx_n_u_validation); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 446, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_14);
       __Pyx_INCREF(__pyx_n_u_xData);
       __pyx_t_8 = __pyx_n_u_xData;
-      __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_t_14, __pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 443, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_t_14, __pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 446, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       { /* enter inner scope */
-        __pyx_t_9 = PyList_New(0); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 443, __pyx_L22_error)
+        __pyx_t_9 = PyList_New(0); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 446, __pyx_L22_error)
         __Pyx_GOTREF(__pyx_t_9);
         __pyx_t_11 = 0;
-        __pyx_t_3 = __pyx_convert_map_to_py_int____int(__pyx_v_nd.second.num_nodes); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 443, __pyx_L22_error)
+        __pyx_t_3 = __pyx_convert_map_to_py_int____int(__pyx_v_nd.second.num_nodes); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 446, __pyx_L22_error)
         __Pyx_GOTREF(__pyx_t_3);
-        __pyx_t_13 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyDict_Type)), __pyx_t_3); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 443, __pyx_L22_error)
+        __pyx_t_13 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyDict_Type)), __pyx_t_3); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 446, __pyx_L22_error)
         __Pyx_GOTREF(__pyx_t_13);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        __pyx_t_3 = __Pyx_dict_iterator(__pyx_t_13, 1, __pyx_n_s_items, (&__pyx_t_10), (&__pyx_t_12)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 443, __pyx_L22_error)
+        __pyx_t_3 = __Pyx_dict_iterator(__pyx_t_13, 1, __pyx_n_s_items, (&__pyx_t_10), (&__pyx_t_12)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 446, __pyx_L22_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
         __Pyx_XDECREF(__pyx_t_2);
         __pyx_t_2 = __pyx_t_3;
         __pyx_t_3 = 0;
         while (1) {
           __pyx_t_15 = __Pyx_dict_iter_next(__pyx_t_2, __pyx_t_10, &__pyx_t_11, &__pyx_t_3, &__pyx_t_13, NULL, __pyx_t_12);
           if (unlikely(__pyx_t_15 == 0)) break;
-          if (unlikely(__pyx_t_15 == -1)) __PYX_ERR(0, 443, __pyx_L22_error)
+          if (unlikely(__pyx_t_15 == -1)) __PYX_ERR(0, 446, __pyx_L22_error)
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_GOTREF(__pyx_t_13);
           __Pyx_XDECREF_SET(__pyx_8genexpr4__pyx_v_i, __pyx_t_3);
           __pyx_t_3 = 0;
           __Pyx_XDECREF_SET(__pyx_8genexpr4__pyx_v_j, __pyx_t_13);
           __pyx_t_13 = 0;
-          __pyx_t_13 = PyList_New(1); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 443, __pyx_L22_error)
+          __pyx_t_13 = PyList_New(1); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 446, __pyx_L22_error)
           __Pyx_GOTREF(__pyx_t_13);
           __Pyx_INCREF(__pyx_8genexpr4__pyx_v_i);
           __Pyx_GIVEREF(__pyx_8genexpr4__pyx_v_i);
-          if (__Pyx_PyList_SET_ITEM(__pyx_t_13, 0, __pyx_8genexpr4__pyx_v_i)) __PYX_ERR(0, 443, __pyx_L22_error);
-          { PyObject* __pyx_temp = PyNumber_InPlaceMultiply(__pyx_t_13, __pyx_8genexpr4__pyx_v_j); if (unlikely(!__pyx_temp)) __PYX_ERR(0, 443, __pyx_L22_error)
+          if (__Pyx_PyList_SET_ITEM(__pyx_t_13, 0, __pyx_8genexpr4__pyx_v_i)) __PYX_ERR(0, 446, __pyx_L22_error);
+          { PyObject* __pyx_temp = PyNumber_InPlaceMultiply(__pyx_t_13, __pyx_8genexpr4__pyx_v_j); if (unlikely(!__pyx_temp)) __PYX_ERR(0, 446, __pyx_L22_error)
             __Pyx_GOTREF(__pyx_temp);
             __Pyx_DECREF(__pyx_t_13);
             __pyx_t_13 = __pyx_temp;
           }
-          if (unlikely(__Pyx_ListComp_Append(__pyx_t_9, (PyObject*)__pyx_t_13))) __PYX_ERR(0, 443, __pyx_L22_error)
+          if (unlikely(__Pyx_ListComp_Append(__pyx_t_9, (PyObject*)__pyx_t_13))) __PYX_ERR(0, 446, __pyx_L22_error)
           __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
         }
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_XDECREF(__pyx_8genexpr4__pyx_v_i); __pyx_8genexpr4__pyx_v_i = 0;
         __Pyx_XDECREF(__pyx_8genexpr4__pyx_v_j); __pyx_8genexpr4__pyx_v_j = 0;
         goto __pyx_L25_exit_scope;
         __pyx_L22_error:;
         __Pyx_XDECREF(__pyx_8genexpr4__pyx_v_i); __pyx_8genexpr4__pyx_v_i = 0;
         __Pyx_XDECREF(__pyx_8genexpr4__pyx_v_j); __pyx_8genexpr4__pyx_v_j = 0;
         goto __pyx_L1_error;
         __pyx_L25_exit_scope:;
       } /* exit inner scope */
-      __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 443, __pyx_L1_error)
+      __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 446, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_13 = PyTuple_New(2); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 443, __pyx_L1_error)
+      __pyx_t_13 = PyTuple_New(2); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 446, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_13);
       __Pyx_GIVEREF(__pyx_t_9);
-      if (__Pyx_PyTuple_SET_ITEM(__pyx_t_13, 0, __pyx_t_9)) __PYX_ERR(0, 443, __pyx_L1_error);
+      if (__Pyx_PyTuple_SET_ITEM(__pyx_t_13, 0, __pyx_t_9)) __PYX_ERR(0, 446, __pyx_L1_error);
       __Pyx_GIVEREF(__pyx_t_2);
-      if (__Pyx_PyTuple_SET_ITEM(__pyx_t_13, 1, __pyx_t_2)) __PYX_ERR(0, 443, __pyx_L1_error);
+      if (__Pyx_PyTuple_SET_ITEM(__pyx_t_13, 1, __pyx_t_2)) __PYX_ERR(0, 446, __pyx_L1_error);
       __pyx_t_9 = 0;
       __pyx_t_2 = 0;
-      __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_sum, __pyx_t_13, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 443, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_sum, __pyx_t_13, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 446, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
-      __pyx_t_13 = PyNumber_InPlaceAdd(__pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 443, __pyx_L1_error)
+      __pyx_t_13 = PyNumber_InPlaceAdd(__pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 446, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_13);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      if (unlikely((PyObject_SetItem(__pyx_t_14, __pyx_t_8, __pyx_t_13) < 0))) __PYX_ERR(0, 443, __pyx_L1_error)
+      if (unlikely((PyObject_SetItem(__pyx_t_14, __pyx_t_8, __pyx_t_13) < 0))) __PYX_ERR(0, 446, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":444
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":447
  *         for nd in its.second.nodes:
  *             hist["validation"]["xData"] += sum([[i]*j for i, j in dict(nd.second.num_nodes).items()], [])
  *             m = max(hist["validation"]["xData"])             # <<<<<<<<<<<<<<
  *             if m > mx_: mx_ = m
  *         break
  */
-      __pyx_t_14 = __Pyx_PyDict_GetItem(__pyx_v_hist, __pyx_n_u_validation); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 444, __pyx_L1_error)
+      __pyx_t_14 = __Pyx_PyDict_GetItem(__pyx_v_hist, __pyx_n_u_validation); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 447, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_14);
-      __pyx_t_13 = __Pyx_PyObject_Dict_GetItem(__pyx_t_14, __pyx_n_u_xData); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 444, __pyx_L1_error)
+      __pyx_t_13 = __Pyx_PyObject_Dict_GetItem(__pyx_t_14, __pyx_n_u_xData); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 447, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_13);
       __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
-      __pyx_t_14 = __Pyx_PyObject_CallOneArg(__pyx_builtin_max, __pyx_t_13); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 444, __pyx_L1_error)
+      __pyx_t_14 = __Pyx_PyObject_CallOneArg(__pyx_builtin_max, __pyx_t_13); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 447, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_14);
       __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
       __Pyx_XDECREF_SET(__pyx_v_m, __pyx_t_14);
       __pyx_t_14 = 0;
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":445
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":448
  *             hist["validation"]["xData"] += sum([[i]*j for i, j in dict(nd.second.num_nodes).items()], [])
  *             m = max(hist["validation"]["xData"])
  *             if m > mx_: mx_ = m             # <<<<<<<<<<<<<<
  *         break
  * 
  */
-      __pyx_t_14 = __Pyx_PyInt_From_int(__pyx_v_mx_); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 445, __pyx_L1_error)
+      __pyx_t_14 = __Pyx_PyInt_From_int(__pyx_v_mx_); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 448, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_14);
-      __pyx_t_13 = PyObject_RichCompare(__pyx_v_m, __pyx_t_14, Py_GT); __Pyx_XGOTREF(__pyx_t_13); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 445, __pyx_L1_error)
+      __pyx_t_13 = PyObject_RichCompare(__pyx_v_m, __pyx_t_14, Py_GT); __Pyx_XGOTREF(__pyx_t_13); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 448, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
-      __pyx_t_16 = __Pyx_PyObject_IsTrue(__pyx_t_13); if (unlikely((__pyx_t_16 < 0))) __PYX_ERR(0, 445, __pyx_L1_error)
+      __pyx_t_16 = __Pyx_PyObject_IsTrue(__pyx_t_13); if (unlikely((__pyx_t_16 < 0))) __PYX_ERR(0, 448, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
       if (__pyx_t_16) {
-        __pyx_t_12 = __Pyx_PyInt_As_int(__pyx_v_m); if (unlikely((__pyx_t_12 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 445, __pyx_L1_error)
+        __pyx_t_12 = __Pyx_PyInt_As_int(__pyx_v_m); if (unlikely((__pyx_t_12 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 448, __pyx_L1_error)
         __pyx_v_mx_ = __pyx_t_12;
       }
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":442
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":445
  * 
  *     for its in valid:
  *         for nd in its.second.nodes:             # <<<<<<<<<<<<<<
  *             hist["validation"]["xData"] += sum([[i]*j for i, j in dict(nd.second.num_nodes).items()], [])
  *             m = max(hist["validation"]["xData"])
  */
     }
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":446
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":449
  *             m = max(hist["validation"]["xData"])
  *             if m > mx_: mx_ = m
  *         break             # <<<<<<<<<<<<<<
  * 
  *     for its in test:
  */
     goto __pyx_L17_break;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":441
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":444
  *         break
  * 
  *     for its in valid:             # <<<<<<<<<<<<<<
  *         for nd in its.second.nodes:
  *             hist["validation"]["xData"] += sum([[i]*j for i, j in dict(nd.second.num_nodes).items()], [])
  */
   }
   goto __pyx_L28_for_end;
   __pyx_L17_break:;
   goto __pyx_L28_for_end;
   __pyx_L28_for_end:;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":448
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":451
  *         break
  * 
  *     for its in test:             # <<<<<<<<<<<<<<
  *         for nd in its.second.nodes:
  *             hist["evaluation"]["xData"] += sum([[i]*j for i, j in dict(nd.second.num_nodes).items()], [])
  */
   __pyx_t_4 = __pyx_v_test.begin();
   for (;;) {
     if (!(__pyx_t_4 != __pyx_v_test.end())) break;
     __pyx_t_5 = *__pyx_t_4;
     ++__pyx_t_4;
     __pyx_v_its = __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_5);
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":449
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":452
  * 
  *     for its in test:
  *         for nd in its.second.nodes:             # <<<<<<<<<<<<<<
  *             hist["evaluation"]["xData"] += sum([[i]*j for i, j in dict(nd.second.num_nodes).items()], [])
  *             m = max(hist["evaluation"]["xData"])
  */
     __pyx_t_6 = __pyx_v_its.second->nodes.begin();
     for (;;) {
       if (!(__pyx_t_6 != __pyx_v_its.second->nodes.end())) break;
       __pyx_t_7 = *__pyx_t_6;
       ++__pyx_t_6;
       __pyx_v_nd = __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_7);
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":450
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":453
  *     for its in test:
  *         for nd in its.second.nodes:
  *             hist["evaluation"]["xData"] += sum([[i]*j for i, j in dict(nd.second.num_nodes).items()], [])             # <<<<<<<<<<<<<<
  *             m = max(hist["evaluation"]["xData"])
  *             if m > mx_: mx_ = m
  */
-      __pyx_t_13 = __Pyx_PyDict_GetItem(__pyx_v_hist, __pyx_n_u_evaluation); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 450, __pyx_L1_error)
+      __pyx_t_13 = __Pyx_PyDict_GetItem(__pyx_v_hist, __pyx_n_u_evaluation); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 453, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_13);
       __Pyx_INCREF(__pyx_n_u_xData);
       __pyx_t_8 = __pyx_n_u_xData;
-      __pyx_t_14 = __Pyx_PyObject_Dict_GetItem(__pyx_t_13, __pyx_t_8); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 450, __pyx_L1_error)
+      __pyx_t_14 = __Pyx_PyObject_Dict_GetItem(__pyx_t_13, __pyx_t_8); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 453, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_14);
       { /* enter inner scope */
-        __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 450, __pyx_L35_error)
+        __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 453, __pyx_L35_error)
         __Pyx_GOTREF(__pyx_t_2);
         __pyx_t_10 = 0;
-        __pyx_t_9 = __pyx_convert_map_to_py_int____int(__pyx_v_nd.second.num_nodes); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 450, __pyx_L35_error)
+        __pyx_t_9 = __pyx_convert_map_to_py_int____int(__pyx_v_nd.second.num_nodes); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 453, __pyx_L35_error)
         __Pyx_GOTREF(__pyx_t_9);
-        __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyDict_Type)), __pyx_t_9); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 450, __pyx_L35_error)
+        __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyDict_Type)), __pyx_t_9); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 453, __pyx_L35_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-        __pyx_t_9 = __Pyx_dict_iterator(__pyx_t_3, 1, __pyx_n_s_items, (&__pyx_t_11), (&__pyx_t_12)); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 450, __pyx_L35_error)
+        __pyx_t_9 = __Pyx_dict_iterator(__pyx_t_3, 1, __pyx_n_s_items, (&__pyx_t_11), (&__pyx_t_12)); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 453, __pyx_L35_error)
         __Pyx_GOTREF(__pyx_t_9);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_XDECREF(__pyx_t_1);
         __pyx_t_1 = __pyx_t_9;
         __pyx_t_9 = 0;
         while (1) {
           __pyx_t_15 = __Pyx_dict_iter_next(__pyx_t_1, __pyx_t_11, &__pyx_t_10, &__pyx_t_9, &__pyx_t_3, NULL, __pyx_t_12);
           if (unlikely(__pyx_t_15 == 0)) break;
-          if (unlikely(__pyx_t_15 == -1)) __PYX_ERR(0, 450, __pyx_L35_error)
+          if (unlikely(__pyx_t_15 == -1)) __PYX_ERR(0, 453, __pyx_L35_error)
           __Pyx_GOTREF(__pyx_t_9);
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_XDECREF_SET(__pyx_8genexpr5__pyx_v_i, __pyx_t_9);
           __pyx_t_9 = 0;
           __Pyx_XDECREF_SET(__pyx_8genexpr5__pyx_v_j, __pyx_t_3);
           __pyx_t_3 = 0;
-          __pyx_t_3 = PyList_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 450, __pyx_L35_error)
+          __pyx_t_3 = PyList_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 453, __pyx_L35_error)
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_INCREF(__pyx_8genexpr5__pyx_v_i);
           __Pyx_GIVEREF(__pyx_8genexpr5__pyx_v_i);
-          if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 0, __pyx_8genexpr5__pyx_v_i)) __PYX_ERR(0, 450, __pyx_L35_error);
-          { PyObject* __pyx_temp = PyNumber_InPlaceMultiply(__pyx_t_3, __pyx_8genexpr5__pyx_v_j); if (unlikely(!__pyx_temp)) __PYX_ERR(0, 450, __pyx_L35_error)
+          if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 0, __pyx_8genexpr5__pyx_v_i)) __PYX_ERR(0, 453, __pyx_L35_error);
+          { PyObject* __pyx_temp = PyNumber_InPlaceMultiply(__pyx_t_3, __pyx_8genexpr5__pyx_v_j); if (unlikely(!__pyx_temp)) __PYX_ERR(0, 453, __pyx_L35_error)
             __Pyx_GOTREF(__pyx_temp);
             __Pyx_DECREF(__pyx_t_3);
             __pyx_t_3 = __pyx_temp;
           }
-          if (unlikely(__Pyx_ListComp_Append(__pyx_t_2, (PyObject*)__pyx_t_3))) __PYX_ERR(0, 450, __pyx_L35_error)
+          if (unlikely(__Pyx_ListComp_Append(__pyx_t_2, (PyObject*)__pyx_t_3))) __PYX_ERR(0, 453, __pyx_L35_error)
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         }
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_XDECREF(__pyx_8genexpr5__pyx_v_i); __pyx_8genexpr5__pyx_v_i = 0;
         __Pyx_XDECREF(__pyx_8genexpr5__pyx_v_j); __pyx_8genexpr5__pyx_v_j = 0;
         goto __pyx_L38_exit_scope;
         __pyx_L35_error:;
         __Pyx_XDECREF(__pyx_8genexpr5__pyx_v_i); __pyx_8genexpr5__pyx_v_i = 0;
         __Pyx_XDECREF(__pyx_8genexpr5__pyx_v_j); __pyx_8genexpr5__pyx_v_j = 0;
         goto __pyx_L1_error;
         __pyx_L38_exit_scope:;
       } /* exit inner scope */
-      __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 450, __pyx_L1_error)
+      __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 453, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 450, __pyx_L1_error)
+      __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 453, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_GIVEREF(__pyx_t_2);
-      if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_2)) __PYX_ERR(0, 450, __pyx_L1_error);
+      if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_2)) __PYX_ERR(0, 453, __pyx_L1_error);
       __Pyx_GIVEREF(__pyx_t_1);
-      if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_1)) __PYX_ERR(0, 450, __pyx_L1_error);
+      if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_1)) __PYX_ERR(0, 453, __pyx_L1_error);
       __pyx_t_2 = 0;
       __pyx_t_1 = 0;
-      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_sum, __pyx_t_3, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 450, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_sum, __pyx_t_3, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 453, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_3 = PyNumber_InPlaceAdd(__pyx_t_14, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 450, __pyx_L1_error)
+      __pyx_t_3 = PyNumber_InPlaceAdd(__pyx_t_14, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 453, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      if (unlikely((PyObject_SetItem(__pyx_t_13, __pyx_t_8, __pyx_t_3) < 0))) __PYX_ERR(0, 450, __pyx_L1_error)
+      if (unlikely((PyObject_SetItem(__pyx_t_13, __pyx_t_8, __pyx_t_3) < 0))) __PYX_ERR(0, 453, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":451
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":454
  *         for nd in its.second.nodes:
  *             hist["evaluation"]["xData"] += sum([[i]*j for i, j in dict(nd.second.num_nodes).items()], [])
  *             m = max(hist["evaluation"]["xData"])             # <<<<<<<<<<<<<<
  *             if m > mx_: mx_ = m
  *         break
  */
-      __pyx_t_13 = __Pyx_PyDict_GetItem(__pyx_v_hist, __pyx_n_u_evaluation); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 451, __pyx_L1_error)
+      __pyx_t_13 = __Pyx_PyDict_GetItem(__pyx_v_hist, __pyx_n_u_evaluation); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 454, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_13);
-      __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_t_13, __pyx_n_u_xData); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 451, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_t_13, __pyx_n_u_xData); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 454, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
-      __pyx_t_13 = __Pyx_PyObject_CallOneArg(__pyx_builtin_max, __pyx_t_3); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 451, __pyx_L1_error)
+      __pyx_t_13 = __Pyx_PyObject_CallOneArg(__pyx_builtin_max, __pyx_t_3); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 454, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_13);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_XDECREF_SET(__pyx_v_m, __pyx_t_13);
       __pyx_t_13 = 0;
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":452
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":455
  *             hist["evaluation"]["xData"] += sum([[i]*j for i, j in dict(nd.second.num_nodes).items()], [])
  *             m = max(hist["evaluation"]["xData"])
  *             if m > mx_: mx_ = m             # <<<<<<<<<<<<<<
  *         break
  *     if sum(hist["training"]["xData"] + hist["validation"]["xData"] + hist["evaluation"]["xData"]): pass
  */
-      __pyx_t_13 = __Pyx_PyInt_From_int(__pyx_v_mx_); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 452, __pyx_L1_error)
+      __pyx_t_13 = __Pyx_PyInt_From_int(__pyx_v_mx_); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 455, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_13);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_m, __pyx_t_13, Py_GT); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 452, __pyx_L1_error)
+      __pyx_t_3 = PyObject_RichCompare(__pyx_v_m, __pyx_t_13, Py_GT); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 455, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
-      __pyx_t_16 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely((__pyx_t_16 < 0))) __PYX_ERR(0, 452, __pyx_L1_error)
+      __pyx_t_16 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely((__pyx_t_16 < 0))) __PYX_ERR(0, 455, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       if (__pyx_t_16) {
-        __pyx_t_12 = __Pyx_PyInt_As_int(__pyx_v_m); if (unlikely((__pyx_t_12 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 452, __pyx_L1_error)
+        __pyx_t_12 = __Pyx_PyInt_As_int(__pyx_v_m); if (unlikely((__pyx_t_12 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 455, __pyx_L1_error)
         __pyx_v_mx_ = __pyx_t_12;
       }
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":449
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":452
  * 
  *     for its in test:
  *         for nd in its.second.nodes:             # <<<<<<<<<<<<<<
  *             hist["evaluation"]["xData"] += sum([[i]*j for i, j in dict(nd.second.num_nodes).items()], [])
  *             m = max(hist["evaluation"]["xData"])
  */
     }
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":453
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":456
  *             m = max(hist["evaluation"]["xData"])
  *             if m > mx_: mx_ = m
  *         break             # <<<<<<<<<<<<<<
  *     if sum(hist["training"]["xData"] + hist["validation"]["xData"] + hist["evaluation"]["xData"]): pass
  *     else: return
  */
     goto __pyx_L30_break;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":448
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":451
  *         break
  * 
  *     for its in test:             # <<<<<<<<<<<<<<
  *         for nd in its.second.nodes:
  *             hist["evaluation"]["xData"] += sum([[i]*j for i, j in dict(nd.second.num_nodes).items()], [])
  */
   }
   goto __pyx_L41_for_end;
   __pyx_L30_break:;
   goto __pyx_L41_for_end;
   __pyx_L41_for_end:;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":454
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":457
  *             if m > mx_: mx_ = m
  *         break
  *     if sum(hist["training"]["xData"] + hist["validation"]["xData"] + hist["evaluation"]["xData"]): pass             # <<<<<<<<<<<<<<
  *     else: return
  * 
  */
-  __pyx_t_3 = __Pyx_PyDict_GetItem(__pyx_v_hist, __pyx_n_u_training); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 454, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_GetItem(__pyx_v_hist, __pyx_n_u_training); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 457, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_13 = __Pyx_PyObject_Dict_GetItem(__pyx_t_3, __pyx_n_u_xData); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 454, __pyx_L1_error)
+  __pyx_t_13 = __Pyx_PyObject_Dict_GetItem(__pyx_t_3, __pyx_n_u_xData); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 457, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_13);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyDict_GetItem(__pyx_v_hist, __pyx_n_u_validation); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 454, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_GetItem(__pyx_v_hist, __pyx_n_u_validation); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 457, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_t_3, __pyx_n_u_xData); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 454, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_t_3, __pyx_n_u_xData); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 457, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyNumber_Add(__pyx_t_13, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 454, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Add(__pyx_t_13, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 457, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyDict_GetItem(__pyx_v_hist, __pyx_n_u_evaluation); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 454, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_GetItem(__pyx_v_hist, __pyx_n_u_evaluation); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 457, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_13 = __Pyx_PyObject_Dict_GetItem(__pyx_t_1, __pyx_n_u_xData); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 454, __pyx_L1_error)
+  __pyx_t_13 = __Pyx_PyObject_Dict_GetItem(__pyx_t_1, __pyx_n_u_xData); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 457, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_13);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyNumber_Add(__pyx_t_3, __pyx_t_13); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 454, __pyx_L1_error)
+  __pyx_t_1 = PyNumber_Add(__pyx_t_3, __pyx_t_13); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 457, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
-  __pyx_t_13 = __Pyx_PyObject_CallOneArg(__pyx_builtin_sum, __pyx_t_1); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 454, __pyx_L1_error)
+  __pyx_t_13 = __Pyx_PyObject_CallOneArg(__pyx_builtin_sum, __pyx_t_1); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 457, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_13);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_16 = __Pyx_PyObject_IsTrue(__pyx_t_13); if (unlikely((__pyx_t_16 < 0))) __PYX_ERR(0, 454, __pyx_L1_error)
+  __pyx_t_16 = __Pyx_PyObject_IsTrue(__pyx_t_13); if (unlikely((__pyx_t_16 < 0))) __PYX_ERR(0, 457, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
   if (__pyx_t_16) {
     goto __pyx_L42;
   }
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":455
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":458
  *         break
  *     if sum(hist["training"]["xData"] + hist["validation"]["xData"] + hist["evaluation"]["xData"]): pass
  *     else: return             # <<<<<<<<<<<<<<
  * 
  *     tmpl = template_th1f(path, "Number of Nodes", "Entries (arb.)", "Node Distribution for Sample Type", 1)
  */
   /*else*/ {
     goto __pyx_L0;
   }
   __pyx_L42:;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":457
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":460
  *     else: return
  * 
  *     tmpl = template_th1f(path, "Number of Nodes", "Entries (arb.)", "Node Distribution for Sample Type", 1)             # <<<<<<<<<<<<<<
  *     tmpl["Filename"] = "NodeStatistics"
  *     tmpl["xBins"] = mx_ + 1
  */
-  __pyx_t_13 = __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_template_th1f(__pyx_v_path, __pyx_kp_u_Number_of_Nodes, __pyx_kp_u_Entries_arb, __pyx_kp_u_Node_Distribution_for_Sample_Typ, 1.0); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 457, __pyx_L1_error)
+  __pyx_t_13 = __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_template_th1f(__pyx_v_path, __pyx_kp_u_Number_of_Nodes, __pyx_kp_u_Entries_arb, __pyx_kp_u_Node_Distribution_for_Sample_Typ, 1.0); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 460, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_13);
   __pyx_v_tmpl = ((PyObject*)__pyx_t_13);
   __pyx_t_13 = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":458
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":461
  * 
  *     tmpl = template_th1f(path, "Number of Nodes", "Entries (arb.)", "Node Distribution for Sample Type", 1)
  *     tmpl["Filename"] = "NodeStatistics"             # <<<<<<<<<<<<<<
  *     tmpl["xBins"] = mx_ + 1
  *     tmpl["xStep"] = 5
  */
   if (unlikely(__pyx_v_tmpl == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-    __PYX_ERR(0, 458, __pyx_L1_error)
+    __PYX_ERR(0, 461, __pyx_L1_error)
   }
-  if (unlikely((PyDict_SetItem(__pyx_v_tmpl, __pyx_n_u_Filename, __pyx_n_u_NodeStatistics) < 0))) __PYX_ERR(0, 458, __pyx_L1_error)
+  if (unlikely((PyDict_SetItem(__pyx_v_tmpl, __pyx_n_u_Filename, __pyx_n_u_NodeStatistics) < 0))) __PYX_ERR(0, 461, __pyx_L1_error)
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":459
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":462
  *     tmpl = template_th1f(path, "Number of Nodes", "Entries (arb.)", "Node Distribution for Sample Type", 1)
  *     tmpl["Filename"] = "NodeStatistics"
  *     tmpl["xBins"] = mx_ + 1             # <<<<<<<<<<<<<<
  *     tmpl["xStep"] = 5
  *     tmpl["xMax"] = mx_ + 1
  */
-  __pyx_t_13 = __Pyx_PyInt_From_long((__pyx_v_mx_ + 1)); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 459, __pyx_L1_error)
+  __pyx_t_13 = __Pyx_PyInt_From_long((__pyx_v_mx_ + 1)); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 462, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_13);
   if (unlikely(__pyx_v_tmpl == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-    __PYX_ERR(0, 459, __pyx_L1_error)
+    __PYX_ERR(0, 462, __pyx_L1_error)
   }
-  if (unlikely((PyDict_SetItem(__pyx_v_tmpl, __pyx_n_u_xBins, __pyx_t_13) < 0))) __PYX_ERR(0, 459, __pyx_L1_error)
+  if (unlikely((PyDict_SetItem(__pyx_v_tmpl, __pyx_n_u_xBins, __pyx_t_13) < 0))) __PYX_ERR(0, 462, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":460
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":463
  *     tmpl["Filename"] = "NodeStatistics"
  *     tmpl["xBins"] = mx_ + 1
  *     tmpl["xStep"] = 5             # <<<<<<<<<<<<<<
  *     tmpl["xMax"] = mx_ + 1
  *     tmpl["Stack"] = True
  */
   if (unlikely(__pyx_v_tmpl == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-    __PYX_ERR(0, 460, __pyx_L1_error)
+    __PYX_ERR(0, 463, __pyx_L1_error)
   }
-  if (unlikely((PyDict_SetItem(__pyx_v_tmpl, __pyx_n_u_xStep, __pyx_int_5) < 0))) __PYX_ERR(0, 460, __pyx_L1_error)
+  if (unlikely((PyDict_SetItem(__pyx_v_tmpl, __pyx_n_u_xStep, __pyx_int_5) < 0))) __PYX_ERR(0, 463, __pyx_L1_error)
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":461
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":464
  *     tmpl["xBins"] = mx_ + 1
  *     tmpl["xStep"] = 5
  *     tmpl["xMax"] = mx_ + 1             # <<<<<<<<<<<<<<
  *     tmpl["Stack"] = True
  *     tmpl["OverlayHists"] = False
  */
-  __pyx_t_13 = __Pyx_PyInt_From_long((__pyx_v_mx_ + 1)); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 461, __pyx_L1_error)
+  __pyx_t_13 = __Pyx_PyInt_From_long((__pyx_v_mx_ + 1)); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 464, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_13);
   if (unlikely(__pyx_v_tmpl == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-    __PYX_ERR(0, 461, __pyx_L1_error)
+    __PYX_ERR(0, 464, __pyx_L1_error)
   }
-  if (unlikely((PyDict_SetItem(__pyx_v_tmpl, __pyx_n_u_xMax, __pyx_t_13) < 0))) __PYX_ERR(0, 461, __pyx_L1_error)
+  if (unlikely((PyDict_SetItem(__pyx_v_tmpl, __pyx_n_u_xMax, __pyx_t_13) < 0))) __PYX_ERR(0, 464, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":462
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":465
  *     tmpl["xStep"] = 5
  *     tmpl["xMax"] = mx_ + 1
  *     tmpl["Stack"] = True             # <<<<<<<<<<<<<<
  *     tmpl["OverlayHists"] = False
  *     tmpl["xBinCentering"] = True
  */
   if (unlikely(__pyx_v_tmpl == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-    __PYX_ERR(0, 462, __pyx_L1_error)
+    __PYX_ERR(0, 465, __pyx_L1_error)
   }
-  if (unlikely((PyDict_SetItem(__pyx_v_tmpl, __pyx_n_u_Stack, Py_True) < 0))) __PYX_ERR(0, 462, __pyx_L1_error)
+  if (unlikely((PyDict_SetItem(__pyx_v_tmpl, __pyx_n_u_Stack, Py_True) < 0))) __PYX_ERR(0, 465, __pyx_L1_error)
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":463
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":466
  *     tmpl["xMax"] = mx_ + 1
  *     tmpl["Stack"] = True
  *     tmpl["OverlayHists"] = False             # <<<<<<<<<<<<<<
  *     tmpl["xBinCentering"] = True
  *     for node in hist: tmpl["Histograms"] += [TH1F(**hist[node])]
  */
   if (unlikely(__pyx_v_tmpl == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-    __PYX_ERR(0, 463, __pyx_L1_error)
+    __PYX_ERR(0, 466, __pyx_L1_error)
   }
-  if (unlikely((PyDict_SetItem(__pyx_v_tmpl, __pyx_n_u_OverlayHists, Py_False) < 0))) __PYX_ERR(0, 463, __pyx_L1_error)
+  if (unlikely((PyDict_SetItem(__pyx_v_tmpl, __pyx_n_u_OverlayHists, Py_False) < 0))) __PYX_ERR(0, 466, __pyx_L1_error)
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":464
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":467
  *     tmpl["Stack"] = True
  *     tmpl["OverlayHists"] = False
  *     tmpl["xBinCentering"] = True             # <<<<<<<<<<<<<<
  *     for node in hist: tmpl["Histograms"] += [TH1F(**hist[node])]
  *     th = TH1F(**tmpl)
  */
   if (unlikely(__pyx_v_tmpl == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-    __PYX_ERR(0, 464, __pyx_L1_error)
+    __PYX_ERR(0, 467, __pyx_L1_error)
   }
-  if (unlikely((PyDict_SetItem(__pyx_v_tmpl, __pyx_n_u_xBinCentering, Py_True) < 0))) __PYX_ERR(0, 464, __pyx_L1_error)
+  if (unlikely((PyDict_SetItem(__pyx_v_tmpl, __pyx_n_u_xBinCentering, Py_True) < 0))) __PYX_ERR(0, 467, __pyx_L1_error)
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":465
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":468
  *     tmpl["OverlayHists"] = False
  *     tmpl["xBinCentering"] = True
  *     for node in hist: tmpl["Histograms"] += [TH1F(**hist[node])]             # <<<<<<<<<<<<<<
  *     th = TH1F(**tmpl)
  *     th.SaveFigure()
  */
   __pyx_t_11 = 0;
-  __pyx_t_1 = __Pyx_dict_iterator(__pyx_v_hist, 1, ((PyObject *)NULL), (&__pyx_t_10), (&__pyx_t_12)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 465, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_dict_iterator(__pyx_v_hist, 1, ((PyObject *)NULL), (&__pyx_t_10), (&__pyx_t_12)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 468, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_13);
   __pyx_t_13 = __pyx_t_1;
   __pyx_t_1 = 0;
   while (1) {
     __pyx_t_15 = __Pyx_dict_iter_next(__pyx_t_13, __pyx_t_10, &__pyx_t_11, &__pyx_t_1, NULL, NULL, __pyx_t_12);
     if (unlikely(__pyx_t_15 == 0)) break;
-    if (unlikely(__pyx_t_15 == -1)) __PYX_ERR(0, 465, __pyx_L1_error)
+    if (unlikely(__pyx_t_15 == -1)) __PYX_ERR(0, 468, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_XDECREF_SET(__pyx_v_node, __pyx_t_1);
     __pyx_t_1 = 0;
     if (unlikely(__pyx_v_tmpl == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 465, __pyx_L1_error)
+      __PYX_ERR(0, 468, __pyx_L1_error)
     }
     __Pyx_INCREF(__pyx_v_tmpl);
     __pyx_t_17 = __pyx_v_tmpl;
     __Pyx_INCREF(__pyx_n_u_Histograms);
     __pyx_t_8 = __pyx_n_u_Histograms;
     if (unlikely(__pyx_t_17 == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 465, __pyx_L1_error)
+      __PYX_ERR(0, 468, __pyx_L1_error)
     }
-    __pyx_t_1 = __Pyx_PyDict_GetItem(__pyx_t_17, __pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 465, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyDict_GetItem(__pyx_t_17, __pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 468, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_TH1F); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 465, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_TH1F); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 468, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_2 = __Pyx_PyDict_GetItem(__pyx_v_hist, __pyx_v_node); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 465, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyDict_GetItem(__pyx_v_hist, __pyx_v_node); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 468, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     if (unlikely(__pyx_t_2 == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "argument after ** must be a mapping, not NoneType");
-      __PYX_ERR(0, 465, __pyx_L1_error)
+      __PYX_ERR(0, 468, __pyx_L1_error)
     }
     if (likely(PyDict_CheckExact(__pyx_t_2))) {
-      __pyx_t_14 = PyDict_Copy(__pyx_t_2); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 465, __pyx_L1_error)
+      __pyx_t_14 = PyDict_Copy(__pyx_t_2); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 468, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_14);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     } else {
-      __pyx_t_14 = __Pyx_PyObject_CallOneArg((PyObject*)&PyDict_Type, __pyx_t_2); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 465, __pyx_L1_error)
+      __pyx_t_14 = __Pyx_PyObject_CallOneArg((PyObject*)&PyDict_Type, __pyx_t_2); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 468, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_14);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     }
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_empty_tuple, __pyx_t_14); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 465, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_empty_tuple, __pyx_t_14); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 468, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
-    __pyx_t_14 = PyList_New(1); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 465, __pyx_L1_error)
+    __pyx_t_14 = PyList_New(1); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 468, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_14);
     __Pyx_GIVEREF(__pyx_t_2);
-    if (__Pyx_PyList_SET_ITEM(__pyx_t_14, 0, __pyx_t_2)) __PYX_ERR(0, 465, __pyx_L1_error);
+    if (__Pyx_PyList_SET_ITEM(__pyx_t_14, 0, __pyx_t_2)) __PYX_ERR(0, 468, __pyx_L1_error);
     __pyx_t_2 = 0;
-    __pyx_t_2 = PyNumber_InPlaceAdd(__pyx_t_1, __pyx_t_14); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 465, __pyx_L1_error)
+    __pyx_t_2 = PyNumber_InPlaceAdd(__pyx_t_1, __pyx_t_14); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 468, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
     if (unlikely(__pyx_t_17 == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 465, __pyx_L1_error)
+      __PYX_ERR(0, 468, __pyx_L1_error)
     }
-    if (unlikely((PyDict_SetItem(__pyx_t_17, __pyx_t_8, __pyx_t_2) < 0))) __PYX_ERR(0, 465, __pyx_L1_error)
+    if (unlikely((PyDict_SetItem(__pyx_t_17, __pyx_t_8, __pyx_t_2) < 0))) __PYX_ERR(0, 468, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
   }
   __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":466
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":469
  *     tmpl["xBinCentering"] = True
  *     for node in hist: tmpl["Histograms"] += [TH1F(**hist[node])]
  *     th = TH1F(**tmpl)             # <<<<<<<<<<<<<<
  *     th.SaveFigure()
  *     del th
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_13, __pyx_n_s_TH1F); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 466, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_13, __pyx_n_s_TH1F); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 469, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_13);
   if (unlikely(__pyx_v_tmpl == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "argument after ** must be a mapping, not NoneType");
-    __PYX_ERR(0, 466, __pyx_L1_error)
+    __PYX_ERR(0, 469, __pyx_L1_error)
   }
-  __pyx_t_2 = PyDict_Copy(__pyx_v_tmpl); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 466, __pyx_L1_error)
+  __pyx_t_2 = PyDict_Copy(__pyx_v_tmpl); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 469, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_14 = __Pyx_PyObject_Call(__pyx_t_13, __pyx_empty_tuple, __pyx_t_2); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 466, __pyx_L1_error)
+  __pyx_t_14 = __Pyx_PyObject_Call(__pyx_t_13, __pyx_empty_tuple, __pyx_t_2); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 469, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_14);
   __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_th = __pyx_t_14;
   __pyx_t_14 = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":467
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":470
  *     for node in hist: tmpl["Histograms"] += [TH1F(**hist[node])]
  *     th = TH1F(**tmpl)
  *     th.SaveFigure()             # <<<<<<<<<<<<<<
  *     del th
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_th, __pyx_n_s_SaveFigure); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 467, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_th, __pyx_n_s_SaveFigure); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 470, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_13 = NULL;
   __pyx_t_12 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_13 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_13)) {
@@ -34276,30 +34294,30 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_13, NULL};
     __pyx_t_14 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_12, 0+__pyx_t_12);
     __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
-    if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 467, __pyx_L1_error)
+    if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 470, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_14);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":468
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":471
  *     th = TH1F(**tmpl)
  *     th.SaveFigure()
  *     del th             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_DECREF(__pyx_v_th); __pyx_v_th = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":424
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":427
  *     del line_auc
  * 
  * cdef void make_nodes(map[int, CyEpoch*] train, map[int, CyEpoch*] valid, map[int, CyEpoch*] test, str path):             # <<<<<<<<<<<<<<
  *     cdef pair[int, CyEpoch*] its
  *     cdef pair[int, node_t] nd
  */
 
@@ -34326,15 +34344,15 @@
   __Pyx_XDECREF(__pyx_8genexpr4__pyx_v_i);
   __Pyx_XDECREF(__pyx_8genexpr4__pyx_v_j);
   __Pyx_XDECREF(__pyx_8genexpr5__pyx_v_i);
   __Pyx_XDECREF(__pyx_8genexpr5__pyx_v_j);
   __Pyx_RefNannyFinishContext();
 }
 
-/* "src/cmodules/cyincludes/cyoptimizer.pyx":489
+/* "src/cmodules/cyincludes/cyoptimizer.pyx":492
  *     cdef public int threads
  * 
  *     def __cinit__(self):             # <<<<<<<<<<<<<<
  *         self.sampletracer = None
  *         self.purge = False
  */
 
@@ -34367,52 +34385,52 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__cinit__", 1);
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":490
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":493
  * 
  *     def __cinit__(self):
  *         self.sampletracer = None             # <<<<<<<<<<<<<<
  *         self.purge = False
  *         self.online = {}
  */
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
   __Pyx_GOTREF(__pyx_v_self->sampletracer);
   __Pyx_DECREF(__pyx_v_self->sampletracer);
   __pyx_v_self->sampletracer = Py_None;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":491
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":494
  *     def __cinit__(self):
  *         self.sampletracer = None
  *         self.purge = False             # <<<<<<<<<<<<<<
  *         self.online = {}
  * 
  */
   __pyx_v_self->purge = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":492
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":495
  *         self.sampletracer = None
  *         self.purge = False
  *         self.online = {}             # <<<<<<<<<<<<<<
  * 
  *     def __init__(self): pass
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 492, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 495, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->online);
   __Pyx_DECREF(__pyx_v_self->online);
   __pyx_v_self->online = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":489
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":492
  *     cdef public int threads
  * 
  *     def __cinit__(self):             # <<<<<<<<<<<<<<
  *         self.sampletracer = None
  *         self.purge = False
  */
 
@@ -34424,15 +34442,15 @@
   __Pyx_AddTraceback("AnalysisG._cmodules.cOptimizer.DataLoader.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/cmodules/cyincludes/cyoptimizer.pyx":494
+/* "src/cmodules/cyincludes/cyoptimizer.pyx":497
  *         self.online = {}
  * 
  *     def __init__(self): pass             # <<<<<<<<<<<<<<
  *     def __dealloc__(self): pass
  *     def __len__(self): return self.batch_hash.size()
  */
 
@@ -34464,15 +34482,15 @@
   int __pyx_r;
 
   /* function exit code */
   __pyx_r = 0;
   return __pyx_r;
 }
 
-/* "src/cmodules/cyincludes/cyoptimizer.pyx":495
+/* "src/cmodules/cyincludes/cyoptimizer.pyx":498
  * 
  *     def __init__(self): pass
  *     def __dealloc__(self): pass             # <<<<<<<<<<<<<<
  *     def __len__(self): return self.batch_hash.size()
  * 
  */
 
@@ -34490,15 +34508,15 @@
 }
 
 static void __pyx_pf_9AnalysisG_9_cmodules_10cOptimizer_10DataLoader_4__dealloc__(CYTHON_UNUSED struct __pyx_obj_9AnalysisG_9_cmodules_10cOptimizer_DataLoader *__pyx_v_self) {
 
   /* function exit code */
 }
 
-/* "src/cmodules/cyincludes/cyoptimizer.pyx":496
+/* "src/cmodules/cyincludes/cyoptimizer.pyx":499
  *     def __init__(self): pass
  *     def __dealloc__(self): pass
  *     def __len__(self): return self.batch_hash.size()             # <<<<<<<<<<<<<<
  * 
  *     cdef DataLoader set_batch(self, int kfold, int batch_size, string mode):
  */
 
@@ -34523,15 +34541,15 @@
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "src/cmodules/cyincludes/cyoptimizer.pyx":498
+/* "src/cmodules/cyincludes/cyoptimizer.pyx":501
  *     def __len__(self): return self.batch_hash.size()
  * 
  *     cdef DataLoader set_batch(self, int kfold, int batch_size, string mode):             # <<<<<<<<<<<<<<
  *         cdef vector[vector[string]] batches
  *         if   mode == b"train": batches = self.ptr.fetch_train(kfold, batch_size)
  */
 
@@ -34568,161 +34586,161 @@
   size_t __pyx_t_18;
   size_t __pyx_t_19;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_batch", 1);
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":500
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":503
  *     cdef DataLoader set_batch(self, int kfold, int batch_size, string mode):
  *         cdef vector[vector[string]] batches
  *         if   mode == b"train": batches = self.ptr.fetch_train(kfold, batch_size)             # <<<<<<<<<<<<<<
  *         elif mode == b"valid": batches = self.ptr.fetch_validation(kfold, batch_size)
  *         elif mode == b"eval":  batches = self.ptr.fetch_evaluation(batch_size)
  */
   __pyx_t_1 = (__pyx_v_mode == ((char const *)"train"));
   if (__pyx_t_1) {
     try {
       __pyx_t_2 = __pyx_v_self->ptr->fetch_train(__pyx_v_kfold, __pyx_v_batch_size);
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 500, __pyx_L1_error)
+      __PYX_ERR(0, 503, __pyx_L1_error)
     }
     __pyx_v_batches = __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_2);
     goto __pyx_L3;
   }
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":501
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":504
  *         cdef vector[vector[string]] batches
  *         if   mode == b"train": batches = self.ptr.fetch_train(kfold, batch_size)
  *         elif mode == b"valid": batches = self.ptr.fetch_validation(kfold, batch_size)             # <<<<<<<<<<<<<<
  *         elif mode == b"eval":  batches = self.ptr.fetch_evaluation(batch_size)
  *         else: return self
  */
   __pyx_t_1 = (__pyx_v_mode == ((char const *)"valid"));
   if (__pyx_t_1) {
     try {
       __pyx_t_2 = __pyx_v_self->ptr->fetch_validation(__pyx_v_kfold, __pyx_v_batch_size);
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 501, __pyx_L1_error)
+      __PYX_ERR(0, 504, __pyx_L1_error)
     }
     __pyx_v_batches = __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_2);
     goto __pyx_L3;
   }
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":502
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":505
  *         if   mode == b"train": batches = self.ptr.fetch_train(kfold, batch_size)
  *         elif mode == b"valid": batches = self.ptr.fetch_validation(kfold, batch_size)
  *         elif mode == b"eval":  batches = self.ptr.fetch_evaluation(batch_size)             # <<<<<<<<<<<<<<
  *         else: return self
  * 
  */
   __pyx_t_1 = (__pyx_v_mode == ((char const *)"eval"));
   if (__pyx_t_1) {
     try {
       __pyx_t_2 = __pyx_v_self->ptr->fetch_evaluation(__pyx_v_batch_size);
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 502, __pyx_L1_error)
+      __PYX_ERR(0, 505, __pyx_L1_error)
     }
     __pyx_v_batches = __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_2);
     goto __pyx_L3;
   }
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":503
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":506
  *         elif mode == b"valid": batches = self.ptr.fetch_validation(kfold, batch_size)
  *         elif mode == b"eval":  batches = self.ptr.fetch_evaluation(batch_size)
  *         else: return self             # <<<<<<<<<<<<<<
  * 
  *         self.device = self.sampletracer.Device
  */
   /*else*/ {
     __Pyx_XDECREF((PyObject *)__pyx_r);
     __Pyx_INCREF((PyObject *)__pyx_v_self);
     __pyx_r = __pyx_v_self;
     goto __pyx_L0;
   }
   __pyx_L3:;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":505
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":508
  *         else: return self
  * 
  *         self.device = self.sampletracer.Device             # <<<<<<<<<<<<<<
  *         self.threads = self.sampletracer.Threads
  *         self.this_batch.clear()
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->sampletracer, __pyx_n_s_Device); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 505, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->sampletracer, __pyx_n_s_Device); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 508, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (!(likely(PyUnicode_CheckExact(__pyx_t_3))||((__pyx_t_3) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_t_3))) __PYX_ERR(0, 505, __pyx_L1_error)
+  if (!(likely(PyUnicode_CheckExact(__pyx_t_3))||((__pyx_t_3) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_t_3))) __PYX_ERR(0, 508, __pyx_L1_error)
   __Pyx_GIVEREF(__pyx_t_3);
   __Pyx_GOTREF(__pyx_v_self->device);
   __Pyx_DECREF(__pyx_v_self->device);
   __pyx_v_self->device = ((PyObject*)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":506
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":509
  * 
  *         self.device = self.sampletracer.Device
  *         self.threads = self.sampletracer.Threads             # <<<<<<<<<<<<<<
  *         self.this_batch.clear()
  *         self.batch_hash.clear()
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->sampletracer, __pyx_n_s_Threads); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 506, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->sampletracer, __pyx_n_s_Threads); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 509, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_4 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 506, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_4 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 509, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_self->threads = __pyx_t_4;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":507
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":510
  *         self.device = self.sampletracer.Device
  *         self.threads = self.sampletracer.Threads
  *         self.this_batch.clear()             # <<<<<<<<<<<<<<
  *         self.batch_hash.clear()
  *         self.kfold = kfold
  */
   __pyx_v_self->this_batch.clear();
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":508
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":511
  *         self.threads = self.sampletracer.Threads
  *         self.this_batch.clear()
  *         self.batch_hash.clear()             # <<<<<<<<<<<<<<
  *         self.kfold = kfold
  *         self.mode = mode
  */
   __pyx_v_self->batch_hash.clear();
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":509
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":512
  *         self.this_batch.clear()
  *         self.batch_hash.clear()
  *         self.kfold = kfold             # <<<<<<<<<<<<<<
  *         self.mode = mode
  * 
  */
   __pyx_v_self->kfold = __pyx_v_kfold;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":510
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":513
  *         self.batch_hash.clear()
  *         self.kfold = kfold
  *         self.mode = mode             # <<<<<<<<<<<<<<
  * 
  *         cdef int idx
  */
   __pyx_v_self->mode = __pyx_v_mode;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":514
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":517
  *         cdef int idx
  *         cdef string hash_
  *         cdef int size = batches.size()             # <<<<<<<<<<<<<<
  *         cdef map[string, k_graphed*] to_fetch
  *         for idx in prange(size, nogil = True, num_threads = self.threads):
  */
   __pyx_v_size = __pyx_v_batches.size();
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":516
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":519
  *         cdef int size = batches.size()
  *         cdef map[string, k_graphed*] to_fetch
  *         for idx in prange(size, nogil = True, num_threads = self.threads):             # <<<<<<<<<<<<<<
  *             if   mode == b"train": self.batch_hash[idx] = self.ptr.check_train(&batches[idx], kfold)
  *             elif mode == b"valid": self.batch_hash[idx] = self.ptr.check_validation(&batches[idx], kfold)
  */
   {
@@ -34764,15 +34782,15 @@
                     #pragma omp for lastprivate(__pyx_v_hash_) firstprivate(__pyx_v_idx) lastprivate(__pyx_v_idx)
                     #endif /* _OPENMP */
                     for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_6; __pyx_t_5++){
                         if (__pyx_parallel_why < 2)
                         {
                             __pyx_v_idx = (int)(0 + 1 * __pyx_t_5);
 
-                            /* "src/cmodules/cyincludes/cyoptimizer.pyx":517
+                            /* "src/cmodules/cyincludes/cyoptimizer.pyx":520
  *         cdef map[string, k_graphed*] to_fetch
  *         for idx in prange(size, nogil = True, num_threads = self.threads):
  *             if   mode == b"train": self.batch_hash[idx] = self.ptr.check_train(&batches[idx], kfold)             # <<<<<<<<<<<<<<
  *             elif mode == b"valid": self.batch_hash[idx] = self.ptr.check_validation(&batches[idx], kfold)
  *             elif mode == b"eval":  self.batch_hash[idx] = self.ptr.check_evaluation(&batches[idx])
  */
                             __pyx_t_1 = (__pyx_v_mode == ((char const *)"train"));
@@ -34783,21 +34801,21 @@
                                 #ifdef WITH_THREAD
                                 PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
                                 #endif
                                 __Pyx_CppExn2PyErr();
                                 #ifdef WITH_THREAD
                                 __Pyx_PyGILState_Release(__pyx_gilstate_save);
                                 #endif
-                                __PYX_ERR(0, 517, __pyx_L9_error)
+                                __PYX_ERR(0, 520, __pyx_L9_error)
                               }
                               (__pyx_v_self->batch_hash[__pyx_v_idx]) = __pyx_t_7;
                               goto __pyx_L11;
                             }
 
-                            /* "src/cmodules/cyincludes/cyoptimizer.pyx":518
+                            /* "src/cmodules/cyincludes/cyoptimizer.pyx":521
  *         for idx in prange(size, nogil = True, num_threads = self.threads):
  *             if   mode == b"train": self.batch_hash[idx] = self.ptr.check_train(&batches[idx], kfold)
  *             elif mode == b"valid": self.batch_hash[idx] = self.ptr.check_validation(&batches[idx], kfold)             # <<<<<<<<<<<<<<
  *             elif mode == b"eval":  self.batch_hash[idx] = self.ptr.check_evaluation(&batches[idx])
  *             for hash_ in batches[idx]: self.this_batch[hash_] = &self.data[hash_]
  */
                             __pyx_t_1 = (__pyx_v_mode == ((char const *)"valid"));
@@ -34808,21 +34826,21 @@
                                 #ifdef WITH_THREAD
                                 PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
                                 #endif
                                 __Pyx_CppExn2PyErr();
                                 #ifdef WITH_THREAD
                                 __Pyx_PyGILState_Release(__pyx_gilstate_save);
                                 #endif
-                                __PYX_ERR(0, 518, __pyx_L9_error)
+                                __PYX_ERR(0, 521, __pyx_L9_error)
                               }
                               (__pyx_v_self->batch_hash[__pyx_v_idx]) = __pyx_t_7;
                               goto __pyx_L11;
                             }
 
-                            /* "src/cmodules/cyincludes/cyoptimizer.pyx":519
+                            /* "src/cmodules/cyincludes/cyoptimizer.pyx":522
  *             if   mode == b"train": self.batch_hash[idx] = self.ptr.check_train(&batches[idx], kfold)
  *             elif mode == b"valid": self.batch_hash[idx] = self.ptr.check_validation(&batches[idx], kfold)
  *             elif mode == b"eval":  self.batch_hash[idx] = self.ptr.check_evaluation(&batches[idx])             # <<<<<<<<<<<<<<
  *             for hash_ in batches[idx]: self.this_batch[hash_] = &self.data[hash_]
  *             for hash_ in self.batch_hash[idx]: to_fetch[hash_] = &self.data[hash_]
  */
                             __pyx_t_1 = (__pyx_v_mode == ((char const *)"eval"));
@@ -34833,21 +34851,21 @@
                                 #ifdef WITH_THREAD
                                 PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
                                 #endif
                                 __Pyx_CppExn2PyErr();
                                 #ifdef WITH_THREAD
                                 __Pyx_PyGILState_Release(__pyx_gilstate_save);
                                 #endif
-                                __PYX_ERR(0, 519, __pyx_L9_error)
+                                __PYX_ERR(0, 522, __pyx_L9_error)
                               }
                               (__pyx_v_self->batch_hash[__pyx_v_idx]) = __pyx_t_7;
                             }
                             __pyx_L11:;
 
-                            /* "src/cmodules/cyincludes/cyoptimizer.pyx":520
+                            /* "src/cmodules/cyincludes/cyoptimizer.pyx":523
  *             elif mode == b"valid": self.batch_hash[idx] = self.ptr.check_validation(&batches[idx], kfold)
  *             elif mode == b"eval":  self.batch_hash[idx] = self.ptr.check_evaluation(&batches[idx])
  *             for hash_ in batches[idx]: self.this_batch[hash_] = &self.data[hash_]             # <<<<<<<<<<<<<<
  *             for hash_ in self.batch_hash[idx]: to_fetch[hash_] = &self.data[hash_]
  *             if self.batch_hash[idx].size(): pass
  */
                             __pyx_t_9 = &(__pyx_v_batches[__pyx_v_idx]);
@@ -34856,15 +34874,15 @@
                               if (!(__pyx_t_8 != __pyx_t_9->end())) break;
                               __pyx_t_10 = *__pyx_t_8;
                               ++__pyx_t_8;
                               __pyx_v_hash_ = __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_10);
                               (__pyx_v_self->this_batch[__pyx_v_hash_]) = (&(__pyx_v_self->data[__pyx_v_hash_]));
                             }
 
-                            /* "src/cmodules/cyincludes/cyoptimizer.pyx":521
+                            /* "src/cmodules/cyincludes/cyoptimizer.pyx":524
  *             elif mode == b"eval":  self.batch_hash[idx] = self.ptr.check_evaluation(&batches[idx])
  *             for hash_ in batches[idx]: self.this_batch[hash_] = &self.data[hash_]
  *             for hash_ in self.batch_hash[idx]: to_fetch[hash_] = &self.data[hash_]             # <<<<<<<<<<<<<<
  *             if self.batch_hash[idx].size(): pass
  *             else: self.batch_hash[idx] = batches[idx]
  */
                             __pyx_t_9 = &(__pyx_v_self->batch_hash[__pyx_v_idx]);
@@ -34873,27 +34891,27 @@
                               if (!(__pyx_t_8 != __pyx_t_9->end())) break;
                               __pyx_t_10 = *__pyx_t_8;
                               ++__pyx_t_8;
                               __pyx_v_hash_ = __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_10);
                               (__pyx_v_to_fetch[__pyx_v_hash_]) = (&(__pyx_v_self->data[__pyx_v_hash_]));
                             }
 
-                            /* "src/cmodules/cyincludes/cyoptimizer.pyx":522
+                            /* "src/cmodules/cyincludes/cyoptimizer.pyx":525
  *             for hash_ in batches[idx]: self.this_batch[hash_] = &self.data[hash_]
  *             for hash_ in self.batch_hash[idx]: to_fetch[hash_] = &self.data[hash_]
  *             if self.batch_hash[idx].size(): pass             # <<<<<<<<<<<<<<
  *             else: self.batch_hash[idx] = batches[idx]
  *         self.indx_e = size
  */
                             __pyx_t_1 = ((__pyx_v_self->batch_hash[__pyx_v_idx]).size() != 0);
                             if (__pyx_t_1) {
                               goto __pyx_L18;
                             }
 
-                            /* "src/cmodules/cyincludes/cyoptimizer.pyx":523
+                            /* "src/cmodules/cyincludes/cyoptimizer.pyx":526
  *             for hash_ in self.batch_hash[idx]: to_fetch[hash_] = &self.data[hash_]
  *             if self.batch_hash[idx].size(): pass
  *             else: self.batch_hash[idx] = batches[idx]             # <<<<<<<<<<<<<<
  *         self.indx_e = size
  * 
  */
                             /*else*/ {
@@ -34979,15 +34997,15 @@
             #undef likely
             #undef unlikely
             #define likely(x)   __builtin_expect(!!(x), 1)
             #define unlikely(x) __builtin_expect(!!(x), 0)
         #endif
       }
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":516
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":519
  *         cdef int size = batches.size()
  *         cdef map[string, k_graphed*] to_fetch
  *         for idx in prange(size, nogil = True, num_threads = self.threads):             # <<<<<<<<<<<<<<
  *             if   mode == b"train": self.batch_hash[idx] = self.ptr.check_train(&batches[idx], kfold)
  *             elif mode == b"valid": self.batch_hash[idx] = self.ptr.check_validation(&batches[idx], kfold)
  */
       /*finally:*/ {
@@ -35005,84 +35023,84 @@
           #endif
           goto __pyx_L1_error;
         }
         __pyx_L6:;
       }
   }
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":524
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":527
  *             if self.batch_hash[idx].size(): pass
  *             else: self.batch_hash[idx] = batches[idx]
  *         self.indx_e = size             # <<<<<<<<<<<<<<
  * 
  *         if not to_fetch.size(): return self
  */
   __pyx_v_self->indx_e = __pyx_v_size;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":526
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":529
  *         self.indx_e = size
  * 
  *         if not to_fetch.size(): return self             # <<<<<<<<<<<<<<
  *         cdef pair[string, k_graphed*] itr
  *         cdef vector[string] cfetch = [itr.first for itr in to_fetch]
  */
   __pyx_t_1 = (!(__pyx_v_to_fetch.size() != 0));
   if (__pyx_t_1) {
     __Pyx_XDECREF((PyObject *)__pyx_r);
     __Pyx_INCREF((PyObject *)__pyx_v_self);
     __pyx_r = __pyx_v_self;
     goto __pyx_L0;
   }
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":528
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":531
  *         if not to_fetch.size(): return self
  *         cdef pair[string, k_graphed*] itr
  *         cdef vector[string] cfetch = [itr.first for itr in to_fetch]             # <<<<<<<<<<<<<<
  *         cdef list fetch = pdec(&cfetch)
  *         self.sampletracer.RestoreGraphs(fetch)
  */
   { /* enter inner scope */
-    __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 528, __pyx_L1_error)
+    __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 531, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_11 = __pyx_v_to_fetch.begin();
     for (;;) {
       if (!(__pyx_t_11 != __pyx_v_to_fetch.end())) break;
       __pyx_t_12 = *__pyx_t_11;
       ++__pyx_t_11;
       __pyx_8genexpr6__pyx_v_itr = __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_12);
-      __pyx_t_13 = __pyx_convert_PyBytes_string_to_py_6libcpp_6string_std__in_string(__pyx_8genexpr6__pyx_v_itr.first); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 528, __pyx_L1_error)
+      __pyx_t_13 = __pyx_convert_PyBytes_string_to_py_6libcpp_6string_std__in_string(__pyx_8genexpr6__pyx_v_itr.first); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 531, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_13);
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_3, (PyObject*)__pyx_t_13))) __PYX_ERR(0, 528, __pyx_L1_error)
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_3, (PyObject*)__pyx_t_13))) __PYX_ERR(0, 531, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
     }
   } /* exit inner scope */
-  __pyx_t_7 = __pyx_convert_vector_from_py_std_3a__3a_string(__pyx_t_3); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 528, __pyx_L1_error)
+  __pyx_t_7 = __pyx_convert_vector_from_py_std_3a__3a_string(__pyx_t_3); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 531, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_cfetch = __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_7);
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":529
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":532
  *         cdef pair[string, k_graphed*] itr
  *         cdef vector[string] cfetch = [itr.first for itr in to_fetch]
  *         cdef list fetch = pdec(&cfetch)             # <<<<<<<<<<<<<<
  *         self.sampletracer.RestoreGraphs(fetch)
  * 
  */
-  __pyx_t_3 = __pyx_f_7cytools_pdec((&__pyx_v_cfetch)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 529, __pyx_L1_error)
+  __pyx_t_3 = __pyx_f_7cytools_pdec((&__pyx_v_cfetch)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 532, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_v_fetch = ((PyObject*)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":530
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":533
  *         cdef vector[string] cfetch = [itr.first for itr in to_fetch]
  *         cdef list fetch = pdec(&cfetch)
  *         self.sampletracer.RestoreGraphs(fetch)             # <<<<<<<<<<<<<<
  * 
  *         cdef map[string, graph_t] graphs = self.sampletracer.makelist(fetch, True)[1]
  */
-  __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->sampletracer, __pyx_n_s_RestoreGraphs); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 530, __pyx_L1_error)
+  __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->sampletracer, __pyx_n_s_RestoreGraphs); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 533, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_13);
   __pyx_t_14 = NULL;
   __pyx_t_6 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_13))) {
     __pyx_t_14 = PyMethod_GET_SELF(__pyx_t_13);
     if (likely(__pyx_t_14)) {
@@ -35094,28 +35112,28 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_14, __pyx_v_fetch};
     __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_13, __pyx_callargs+1-__pyx_t_6, 1+__pyx_t_6);
     __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 530, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 533, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":532
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":535
  *         self.sampletracer.RestoreGraphs(fetch)
  * 
  *         cdef map[string, graph_t] graphs = self.sampletracer.makelist(fetch, True)[1]             # <<<<<<<<<<<<<<
  *         if not graphs.size(): self.ptr.flush_train(&cfetch, self.kfold)
  *         else: self.sampletracer.FlushGraphs(fetch)
  */
-  __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->sampletracer, __pyx_n_s_makelist); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 532, __pyx_L1_error)
+  __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->sampletracer, __pyx_n_s_makelist); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 535, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_13);
   __pyx_t_14 = NULL;
   __pyx_t_6 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_13))) {
     __pyx_t_14 = PyMethod_GET_SELF(__pyx_t_13);
     if (likely(__pyx_t_14)) {
@@ -35127,52 +35145,52 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[3] = {__pyx_t_14, __pyx_v_fetch, Py_True};
     __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_13, __pyx_callargs+1-__pyx_t_6, 2+__pyx_t_6);
     __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 532, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 535, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
   }
-  __pyx_t_13 = __Pyx_GetItemInt(__pyx_t_3, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 532, __pyx_L1_error)
+  __pyx_t_13 = __Pyx_GetItemInt(__pyx_t_3, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 535, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_13);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_15 = __pyx_convert_map_from_py_std_3a__3a_string__and_struct__graph_t(__pyx_t_13); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 532, __pyx_L1_error)
+  __pyx_t_15 = __pyx_convert_map_from_py_std_3a__3a_string__and_struct__graph_t(__pyx_t_13); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 535, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
   __pyx_v_graphs = __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_15);
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":533
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":536
  * 
  *         cdef map[string, graph_t] graphs = self.sampletracer.makelist(fetch, True)[1]
  *         if not graphs.size(): self.ptr.flush_train(&cfetch, self.kfold)             # <<<<<<<<<<<<<<
  *         else: self.sampletracer.FlushGraphs(fetch)
  * 
  */
   __pyx_t_1 = (!(__pyx_v_graphs.size() != 0));
   if (__pyx_t_1) {
     try {
       __pyx_v_self->ptr->flush_train((&__pyx_v_cfetch), __pyx_v_self->kfold);
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 533, __pyx_L1_error)
+      __PYX_ERR(0, 536, __pyx_L1_error)
     }
     goto __pyx_L25;
   }
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":534
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":537
  *         cdef map[string, graph_t] graphs = self.sampletracer.makelist(fetch, True)[1]
  *         if not graphs.size(): self.ptr.flush_train(&cfetch, self.kfold)
  *         else: self.sampletracer.FlushGraphs(fetch)             # <<<<<<<<<<<<<<
  * 
  *         cdef graph_t* gr
  */
   /*else*/ {
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->sampletracer, __pyx_n_s_FlushGraphs); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 534, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->sampletracer, __pyx_n_s_FlushGraphs); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 537, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_14 = NULL;
     __pyx_t_6 = 0;
     #if CYTHON_UNPACK_METHODS
     if (likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_14 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_14)) {
@@ -35184,23 +35202,23 @@
       }
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_14, __pyx_v_fetch};
       __pyx_t_13 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_6, 1+__pyx_t_6);
       __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
-      if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 534, __pyx_L1_error)
+      if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 537, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_13);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     }
     __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
   }
   __pyx_L25:;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":537
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":540
  * 
  *         cdef graph_t* gr
  *         for idx in prange(graphs.size(), nogil = True, num_threads = graphs.size()):             # <<<<<<<<<<<<<<
  *             gr = &graphs[cfetch[idx]]
  *             to_fetch[gr.event_hash].pkl = gr.pickled_data
  */
   {
@@ -35232,34 +35250,34 @@
                     #endif /* _OPENMP */
                     for (__pyx_t_17 = 0; __pyx_t_17 < __pyx_t_18; __pyx_t_17++){
                         {
                             __pyx_v_idx = (int)(0 + 1 * __pyx_t_17);
                             /* Initialize private variables to invalid values */
                             __pyx_v_gr = ((struct graph_t *)1);
 
-                            /* "src/cmodules/cyincludes/cyoptimizer.pyx":538
+                            /* "src/cmodules/cyincludes/cyoptimizer.pyx":541
  *         cdef graph_t* gr
  *         for idx in prange(graphs.size(), nogil = True, num_threads = graphs.size()):
  *             gr = &graphs[cfetch[idx]]             # <<<<<<<<<<<<<<
  *             to_fetch[gr.event_hash].pkl = gr.pickled_data
  *             to_fetch[gr.event_hash].node_size = gr.hash_particle.size()
  */
                             __pyx_v_gr = (&(__pyx_v_graphs[(__pyx_v_cfetch[__pyx_v_idx])]));
 
-                            /* "src/cmodules/cyincludes/cyoptimizer.pyx":539
+                            /* "src/cmodules/cyincludes/cyoptimizer.pyx":542
  *         for idx in prange(graphs.size(), nogil = True, num_threads = graphs.size()):
  *             gr = &graphs[cfetch[idx]]
  *             to_fetch[gr.event_hash].pkl = gr.pickled_data             # <<<<<<<<<<<<<<
  *             to_fetch[gr.event_hash].node_size = gr.hash_particle.size()
  *         graphs.clear()
  */
                             __pyx_t_10 = __pyx_v_gr->pickled_data;
                             (__pyx_v_to_fetch[__pyx_v_gr->event_hash])->pkl = __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_10);
 
-                            /* "src/cmodules/cyincludes/cyoptimizer.pyx":540
+                            /* "src/cmodules/cyincludes/cyoptimizer.pyx":543
  *             gr = &graphs[cfetch[idx]]
  *             to_fetch[gr.event_hash].pkl = gr.pickled_data
  *             to_fetch[gr.event_hash].node_size = gr.hash_particle.size()             # <<<<<<<<<<<<<<
  *         graphs.clear()
  *         return self
  */
                             (__pyx_v_to_fetch[__pyx_v_gr->event_hash])->node_size = __pyx_v_gr->hash_particle.size();
@@ -35272,15 +35290,15 @@
             #undef likely
             #undef unlikely
             #define likely(x)   __builtin_expect(!!(x), 1)
             #define unlikely(x) __builtin_expect(!!(x), 0)
         #endif
       }
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":537
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":540
  * 
  *         cdef graph_t* gr
  *         for idx in prange(graphs.size(), nogil = True, num_threads = graphs.size()):             # <<<<<<<<<<<<<<
  *             gr = &graphs[cfetch[idx]]
  *             to_fetch[gr.event_hash].pkl = gr.pickled_data
  */
       /*finally:*/ {
@@ -35291,36 +35309,36 @@
           #endif
           goto __pyx_L28;
         }
         __pyx_L28:;
       }
   }
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":541
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":544
  *             to_fetch[gr.event_hash].pkl = gr.pickled_data
  *             to_fetch[gr.event_hash].node_size = gr.hash_particle.size()
  *         graphs.clear()             # <<<<<<<<<<<<<<
  *         return self
  * 
  */
   __pyx_v_graphs.clear();
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":542
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":545
  *             to_fetch[gr.event_hash].node_size = gr.hash_particle.size()
  *         graphs.clear()
  *         return self             # <<<<<<<<<<<<<<
  * 
  *     def __iter__(self):
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __Pyx_INCREF((PyObject *)__pyx_v_self);
   __pyx_r = __pyx_v_self;
   goto __pyx_L0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":498
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":501
  *     def __len__(self): return self.batch_hash.size()
  * 
  *     cdef DataLoader set_batch(self, int kfold, int batch_size, string mode):             # <<<<<<<<<<<<<<
  *         cdef vector[vector[string]] batches
  *         if   mode == b"train": batches = self.ptr.fetch_train(kfold, batch_size)
  */
 
@@ -35334,15 +35352,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_fetch);
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/cmodules/cyincludes/cyoptimizer.pyx":544
+/* "src/cmodules/cyincludes/cyoptimizer.pyx":547
  *         return self
  * 
  *     def __iter__(self):             # <<<<<<<<<<<<<<
  *         self.indx_s = 0
  *         return self
  */
 
@@ -35362,51 +35380,51 @@
 }
 
 static PyObject *__pyx_pf_9AnalysisG_9_cmodules_10cOptimizer_10DataLoader_8__iter__(struct __pyx_obj_9AnalysisG_9_cmodules_10cOptimizer_DataLoader *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__iter__", 1);
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":545
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":548
  * 
  *     def __iter__(self):
  *         self.indx_s = 0             # <<<<<<<<<<<<<<
  *         return self
  * 
  */
   __pyx_v_self->indx_s = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":546
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":549
  *     def __iter__(self):
  *         self.indx_s = 0
  *         return self             # <<<<<<<<<<<<<<
  * 
  *     def __next__(self):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF((PyObject *)__pyx_v_self);
   __pyx_r = ((PyObject *)__pyx_v_self);
   goto __pyx_L0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":544
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":547
  *         return self
  * 
  *     def __iter__(self):             # <<<<<<<<<<<<<<
  *         self.indx_s = 0
  *         return self
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/cmodules/cyincludes/cyoptimizer.pyx":548
+/* "src/cmodules/cyincludes/cyoptimizer.pyx":551
  *         return self
  * 
  *     def __next__(self):             # <<<<<<<<<<<<<<
  *         if self.indx_s == self.indx_e: raise StopIteration
  *         cdef vector[string]* hash_ = &self.batch_hash[self.indx_s]
  */
 
@@ -35459,44 +35477,44 @@
   PyObject *__pyx_t_18 = NULL;
   PyObject *__pyx_t_19 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__next__", 1);
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":549
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":552
  * 
  *     def __next__(self):
  *         if self.indx_s == self.indx_e: raise StopIteration             # <<<<<<<<<<<<<<
  *         cdef vector[string]* hash_ = &self.batch_hash[self.indx_s]
  *         cdef bool trig = len(self.sampletracer.MonitorMemory("Graph"))
  */
   __pyx_t_1 = (__pyx_v_self->indx_s == __pyx_v_self->indx_e);
   if (unlikely(__pyx_t_1)) {
     __pyx_error_without_exception = 1;
     goto __pyx_L1_error;;
   }
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":550
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":553
  *     def __next__(self):
  *         if self.indx_s == self.indx_e: raise StopIteration
  *         cdef vector[string]* hash_ = &self.batch_hash[self.indx_s]             # <<<<<<<<<<<<<<
  *         cdef bool trig = len(self.sampletracer.MonitorMemory("Graph"))
  *         if trig:
  */
   __pyx_v_hash_ = (&(__pyx_v_self->batch_hash[__pyx_v_self->indx_s]));
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":551
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":554
  *         if self.indx_s == self.indx_e: raise StopIteration
  *         cdef vector[string]* hash_ = &self.batch_hash[self.indx_s]
  *         cdef bool trig = len(self.sampletracer.MonitorMemory("Graph"))             # <<<<<<<<<<<<<<
  *         if trig:
  *             for k in self.online.values(): del k
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->sampletracer, __pyx_n_s_MonitorMemory); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 551, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->sampletracer, __pyx_n_s_MonitorMemory); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 554, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   __pyx_t_5 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
@@ -35508,217 +35526,217 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_n_u_Graph};
     __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 551, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 554, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
-  __pyx_t_6 = PyObject_Length(__pyx_t_2); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 551, __pyx_L1_error)
+  __pyx_t_6 = PyObject_Length(__pyx_t_2); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 554, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_trig = __pyx_t_6;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":552
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":555
  *         cdef vector[string]* hash_ = &self.batch_hash[self.indx_s]
  *         cdef bool trig = len(self.sampletracer.MonitorMemory("Graph"))
  *         if trig:             # <<<<<<<<<<<<<<
  *             for k in self.online.values(): del k
  *             self.online.clear()
  */
   __pyx_t_1 = (__pyx_v_trig != 0);
   if (__pyx_t_1) {
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":553
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":556
  *         cdef bool trig = len(self.sampletracer.MonitorMemory("Graph"))
  *         if trig:
  *             for k in self.online.values(): del k             # <<<<<<<<<<<<<<
  *             self.online.clear()
  *             if self.mode.compare(b"train"): self.ptr.flush_train(hash_, self.kfold)
  */
     __pyx_t_6 = 0;
     if (unlikely(__pyx_v_self->online == Py_None)) {
       PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "values");
-      __PYX_ERR(0, 553, __pyx_L1_error)
+      __PYX_ERR(0, 556, __pyx_L1_error)
     }
-    __pyx_t_3 = __Pyx_dict_iterator(__pyx_v_self->online, 1, __pyx_n_s_values, (&__pyx_t_7), (&__pyx_t_5)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 553, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_dict_iterator(__pyx_v_self->online, 1, __pyx_n_s_values, (&__pyx_t_7), (&__pyx_t_5)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 556, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_XDECREF(__pyx_t_2);
     __pyx_t_2 = __pyx_t_3;
     __pyx_t_3 = 0;
     while (1) {
       __pyx_t_8 = __Pyx_dict_iter_next(__pyx_t_2, __pyx_t_7, &__pyx_t_6, NULL, &__pyx_t_3, NULL, __pyx_t_5);
       if (unlikely(__pyx_t_8 == 0)) break;
-      if (unlikely(__pyx_t_8 == -1)) __PYX_ERR(0, 553, __pyx_L1_error)
+      if (unlikely(__pyx_t_8 == -1)) __PYX_ERR(0, 556, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __pyx_v_k = __pyx_t_3;
       __pyx_t_3 = 0;
       __Pyx_DECREF(__pyx_v_k); __pyx_v_k = 0;
     }
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":554
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":557
  *         if trig:
  *             for k in self.online.values(): del k
  *             self.online.clear()             # <<<<<<<<<<<<<<
  *             if self.mode.compare(b"train"): self.ptr.flush_train(hash_, self.kfold)
  *             elif self.mode.compare(b"valid"): self.ptr.flush_validation(hash_, self.kfold)
  */
     if (unlikely(__pyx_v_self->online == Py_None)) {
       PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "clear");
-      __PYX_ERR(0, 554, __pyx_L1_error)
+      __PYX_ERR(0, 557, __pyx_L1_error)
     }
-    __pyx_t_9 = __Pyx_PyDict_Clear(__pyx_v_self->online); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(0, 554, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyDict_Clear(__pyx_v_self->online); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(0, 557, __pyx_L1_error)
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":555
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":558
  *             for k in self.online.values(): del k
  *             self.online.clear()
  *             if self.mode.compare(b"train"): self.ptr.flush_train(hash_, self.kfold)             # <<<<<<<<<<<<<<
  *             elif self.mode.compare(b"valid"): self.ptr.flush_validation(hash_, self.kfold)
  *             elif self.mode.compare(b"eval"):  self.ptr.flush_evaluation(hash_)
  */
     try {
       __pyx_t_5 = __pyx_v_self->mode.compare(((char const *)"train"));
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 555, __pyx_L1_error)
+      __PYX_ERR(0, 558, __pyx_L1_error)
     }
     __pyx_t_1 = (__pyx_t_5 != 0);
     if (__pyx_t_1) {
       try {
         __pyx_v_self->ptr->flush_train(__pyx_v_hash_, __pyx_v_self->kfold);
       } catch(...) {
         __Pyx_CppExn2PyErr();
-        __PYX_ERR(0, 555, __pyx_L1_error)
+        __PYX_ERR(0, 558, __pyx_L1_error)
       }
       goto __pyx_L7;
     }
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":556
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":559
  *             self.online.clear()
  *             if self.mode.compare(b"train"): self.ptr.flush_train(hash_, self.kfold)
  *             elif self.mode.compare(b"valid"): self.ptr.flush_validation(hash_, self.kfold)             # <<<<<<<<<<<<<<
  *             elif self.mode.compare(b"eval"):  self.ptr.flush_evaluation(hash_)
  * 
  */
     try {
       __pyx_t_5 = __pyx_v_self->mode.compare(((char const *)"valid"));
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 556, __pyx_L1_error)
+      __PYX_ERR(0, 559, __pyx_L1_error)
     }
     __pyx_t_1 = (__pyx_t_5 != 0);
     if (__pyx_t_1) {
       try {
         __pyx_v_self->ptr->flush_validation(__pyx_v_hash_, __pyx_v_self->kfold);
       } catch(...) {
         __Pyx_CppExn2PyErr();
-        __PYX_ERR(0, 556, __pyx_L1_error)
+        __PYX_ERR(0, 559, __pyx_L1_error)
       }
       goto __pyx_L7;
     }
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":557
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":560
  *             if self.mode.compare(b"train"): self.ptr.flush_train(hash_, self.kfold)
  *             elif self.mode.compare(b"valid"): self.ptr.flush_validation(hash_, self.kfold)
  *             elif self.mode.compare(b"eval"):  self.ptr.flush_evaluation(hash_)             # <<<<<<<<<<<<<<
  * 
  *         self.indx_s += 1
  */
     try {
       __pyx_t_5 = __pyx_v_self->mode.compare(((char const *)"eval"));
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 557, __pyx_L1_error)
+      __PYX_ERR(0, 560, __pyx_L1_error)
     }
     __pyx_t_1 = (__pyx_t_5 != 0);
     if (__pyx_t_1) {
       try {
         __pyx_v_self->ptr->flush_evaluation(__pyx_v_hash_);
       } catch(...) {
         __Pyx_CppExn2PyErr();
-        __PYX_ERR(0, 557, __pyx_L1_error)
+        __PYX_ERR(0, 560, __pyx_L1_error)
       }
     }
     __pyx_L7:;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":552
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":555
  *         cdef vector[string]* hash_ = &self.batch_hash[self.indx_s]
  *         cdef bool trig = len(self.sampletracer.MonitorMemory("Graph"))
  *         if trig:             # <<<<<<<<<<<<<<
  *             for k in self.online.values(): del k
  *             self.online.clear()
  */
   }
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":559
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":562
  *             elif self.mode.compare(b"eval"):  self.ptr.flush_evaluation(hash_)
  * 
  *         self.indx_s += 1             # <<<<<<<<<<<<<<
  * 
  *         cdef int idx = self.sampletracer.MaxGPU
  */
   __pyx_v_self->indx_s = (__pyx_v_self->indx_s + 1);
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":561
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":564
  *         self.indx_s += 1
  * 
  *         cdef int idx = self.sampletracer.MaxGPU             # <<<<<<<<<<<<<<
  *         cdef tuple cuda = (None, None)
  *         if idx != -1:
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->sampletracer, __pyx_n_s_MaxGPU); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 561, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->sampletracer, __pyx_n_s_MaxGPU); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 564, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_2); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 561, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_2); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 564, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_idx = __pyx_t_5;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":562
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":565
  * 
  *         cdef int idx = self.sampletracer.MaxGPU
  *         cdef tuple cuda = (None, None)             # <<<<<<<<<<<<<<
  *         if idx != -1:
  *             try: cuda = torch.cuda.mem_get_info()
  */
   __Pyx_INCREF(__pyx_tuple__66);
   __pyx_v_cuda = __pyx_tuple__66;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":563
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":566
  *         cdef int idx = self.sampletracer.MaxGPU
  *         cdef tuple cuda = (None, None)
  *         if idx != -1:             # <<<<<<<<<<<<<<
  *             try: cuda = torch.cuda.mem_get_info()
  *             except RuntimeError: pass
  */
   __pyx_t_1 = (__pyx_v_idx != -1L);
   if (__pyx_t_1) {
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":564
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":567
  *         cdef tuple cuda = (None, None)
  *         if idx != -1:
  *             try: cuda = torch.cuda.mem_get_info()             # <<<<<<<<<<<<<<
  *             except RuntimeError: pass
  * 
  */
     {
       __Pyx_PyThreadState_declare
       __Pyx_PyThreadState_assign
       __Pyx_ExceptionSave(&__pyx_t_10, &__pyx_t_11, &__pyx_t_12);
       __Pyx_XGOTREF(__pyx_t_10);
       __Pyx_XGOTREF(__pyx_t_11);
       __Pyx_XGOTREF(__pyx_t_12);
       /*try:*/ {
-        __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_torch); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 564, __pyx_L9_error)
+        __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_torch); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 567, __pyx_L9_error)
         __Pyx_GOTREF(__pyx_t_3);
-        __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_cuda); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 564, __pyx_L9_error)
+        __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_cuda); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 567, __pyx_L9_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_mem_get_info); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 564, __pyx_L9_error)
+        __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_mem_get_info); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 567, __pyx_L9_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         __pyx_t_4 = NULL;
         __pyx_t_5 = 0;
         #if CYTHON_UNPACK_METHODS
         if (likely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
@@ -35731,46 +35749,46 @@
           }
         }
         #endif
         {
           PyObject *__pyx_callargs[2] = {__pyx_t_4, NULL};
           __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 0+__pyx_t_5);
           __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-          if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 564, __pyx_L9_error)
+          if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 567, __pyx_L9_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         }
-        if (!(likely(PyTuple_CheckExact(__pyx_t_2))||((__pyx_t_2) == Py_None) || __Pyx_RaiseUnexpectedTypeError("tuple", __pyx_t_2))) __PYX_ERR(0, 564, __pyx_L9_error)
+        if (!(likely(PyTuple_CheckExact(__pyx_t_2))||((__pyx_t_2) == Py_None) || __Pyx_RaiseUnexpectedTypeError("tuple", __pyx_t_2))) __PYX_ERR(0, 567, __pyx_L9_error)
         __Pyx_DECREF_SET(__pyx_v_cuda, ((PyObject*)__pyx_t_2));
         __pyx_t_2 = 0;
       }
       __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
       __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
       __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
       goto __pyx_L14_try_end;
       __pyx_L9_error:;
       __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":565
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":568
  *         if idx != -1:
  *             try: cuda = torch.cuda.mem_get_info()
  *             except RuntimeError: pass             # <<<<<<<<<<<<<<
  * 
  *         cdef list out = []
  */
       __pyx_t_5 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_RuntimeError);
       if (__pyx_t_5) {
         __Pyx_ErrRestore(0,0,0);
         goto __pyx_L10_exception_handled;
       }
       goto __pyx_L11_except_error;
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":564
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":567
  *         cdef tuple cuda = (None, None)
  *         if idx != -1:
  *             try: cuda = torch.cuda.mem_get_info()             # <<<<<<<<<<<<<<
  *             except RuntimeError: pass
  * 
  */
       __pyx_L11_except_error:;
@@ -35783,63 +35801,63 @@
       __Pyx_XGIVEREF(__pyx_t_10);
       __Pyx_XGIVEREF(__pyx_t_11);
       __Pyx_XGIVEREF(__pyx_t_12);
       __Pyx_ExceptionReset(__pyx_t_10, __pyx_t_11, __pyx_t_12);
       __pyx_L14_try_end:;
     }
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":563
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":566
  *         cdef int idx = self.sampletracer.MaxGPU
  *         cdef tuple cuda = (None, None)
  *         if idx != -1:             # <<<<<<<<<<<<<<
  *             try: cuda = torch.cuda.mem_get_info()
  *             except RuntimeError: pass
  */
   }
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":567
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":570
  *             except RuntimeError: pass
  * 
  *         cdef list out = []             # <<<<<<<<<<<<<<
  *         cdef list hashes = []
  *         cdef string t_hash
  */
-  __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 567, __pyx_L1_error)
+  __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 570, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_v_out = ((PyObject*)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":568
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":571
  * 
  *         cdef list out = []
  *         cdef list hashes = []             # <<<<<<<<<<<<<<
  *         cdef string t_hash
  *         cdef k_graphed* gr
  */
-  __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 568, __pyx_L1_error)
+  __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 571, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_v_hashes = ((PyObject*)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":571
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":574
  *         cdef string t_hash
  *         cdef k_graphed* gr
  *         for t_hash in dereference(hash_):             # <<<<<<<<<<<<<<
  *             try: data = self.online[env(t_hash)]
  *             except KeyError:
  */
   __pyx_t_14 = &(*__pyx_v_hash_);
   __pyx_t_13 = __pyx_t_14->begin();
   for (;;) {
     if (!(__pyx_t_13 != __pyx_t_14->end())) break;
     __pyx_t_15 = *__pyx_t_13;
     ++__pyx_t_13;
     __pyx_v_t_hash = __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_15);
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":572
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":575
  *         cdef k_graphed* gr
  *         for t_hash in dereference(hash_):
  *             try: data = self.online[env(t_hash)]             # <<<<<<<<<<<<<<
  *             except KeyError:
  *                 gr = self.this_batch[t_hash]
  */
     {
@@ -35848,70 +35866,70 @@
       __Pyx_ExceptionSave(&__pyx_t_12, &__pyx_t_11, &__pyx_t_10);
       __Pyx_XGOTREF(__pyx_t_12);
       __Pyx_XGOTREF(__pyx_t_11);
       __Pyx_XGOTREF(__pyx_t_10);
       /*try:*/ {
         if (unlikely(__pyx_v_self->online == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-          __PYX_ERR(0, 572, __pyx_L17_error)
+          __PYX_ERR(0, 575, __pyx_L17_error)
         }
-        __pyx_t_2 = __pyx_f_7cytools_env(__pyx_v_t_hash); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 572, __pyx_L17_error)
+        __pyx_t_2 = __pyx_f_7cytools_env(__pyx_v_t_hash); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 575, __pyx_L17_error)
         __Pyx_GOTREF(__pyx_t_2);
-        __pyx_t_3 = __Pyx_PyDict_GetItem(__pyx_v_self->online, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 572, __pyx_L17_error)
+        __pyx_t_3 = __Pyx_PyDict_GetItem(__pyx_v_self->online, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 575, __pyx_L17_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_XDECREF_SET(__pyx_v_data, __pyx_t_3);
         __pyx_t_3 = 0;
       }
       __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
       __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
       __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
       goto __pyx_L24_try_end;
       __pyx_L17_error:;
       __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":573
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":576
  *         for t_hash in dereference(hash_):
  *             try: data = self.online[env(t_hash)]
  *             except KeyError:             # <<<<<<<<<<<<<<
  *                 gr = self.this_batch[t_hash]
  *                 if gr.pkl.size(): pass
  */
       __pyx_t_5 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_KeyError);
       if (__pyx_t_5) {
         __Pyx_AddTraceback("AnalysisG._cmodules.cOptimizer.DataLoader.__next__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-        if (__Pyx_GetException(&__pyx_t_3, &__pyx_t_2, &__pyx_t_4) < 0) __PYX_ERR(0, 573, __pyx_L19_except_error)
+        if (__Pyx_GetException(&__pyx_t_3, &__pyx_t_2, &__pyx_t_4) < 0) __PYX_ERR(0, 576, __pyx_L19_except_error)
         __Pyx_XGOTREF(__pyx_t_3);
         __Pyx_XGOTREF(__pyx_t_2);
         __Pyx_XGOTREF(__pyx_t_4);
 
-        /* "src/cmodules/cyincludes/cyoptimizer.pyx":574
+        /* "src/cmodules/cyincludes/cyoptimizer.pyx":577
  *             try: data = self.online[env(t_hash)]
  *             except KeyError:
  *                 gr = self.this_batch[t_hash]             # <<<<<<<<<<<<<<
  *                 if gr.pkl.size(): pass
  *                 else: return None
  */
         __pyx_v_gr = (__pyx_v_self->this_batch[__pyx_v_t_hash]);
 
-        /* "src/cmodules/cyincludes/cyoptimizer.pyx":575
+        /* "src/cmodules/cyincludes/cyoptimizer.pyx":578
  *             except KeyError:
  *                 gr = self.this_batch[t_hash]
  *                 if gr.pkl.size(): pass             # <<<<<<<<<<<<<<
  *                 else: return None
  *                 gc.disable()
  */
         __pyx_t_1 = (__pyx_v_gr->pkl.size() != 0);
         if (__pyx_t_1) {
           goto __pyx_L27;
         }
 
-        /* "src/cmodules/cyincludes/cyoptimizer.pyx":576
+        /* "src/cmodules/cyincludes/cyoptimizer.pyx":579
  *                 gr = self.this_batch[t_hash]
  *                 if gr.pkl.size(): pass
  *                 else: return None             # <<<<<<<<<<<<<<
  *                 gc.disable()
  *                 data = pickle.loads(gr.pkl)
  */
         /*else*/ {
@@ -35920,24 +35938,24 @@
           __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
           goto __pyx_L20_except_return;
         }
         __pyx_L27:;
 
-        /* "src/cmodules/cyincludes/cyoptimizer.pyx":577
+        /* "src/cmodules/cyincludes/cyoptimizer.pyx":580
  *                 if gr.pkl.size(): pass
  *                 else: return None
  *                 gc.disable()             # <<<<<<<<<<<<<<
  *                 data = pickle.loads(gr.pkl)
  *                 gc.enable()
  */
-        __Pyx_GetModuleGlobalName(__pyx_t_17, __pyx_n_s_gc); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 577, __pyx_L19_except_error)
+        __Pyx_GetModuleGlobalName(__pyx_t_17, __pyx_n_s_gc); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 580, __pyx_L19_except_error)
         __Pyx_GOTREF(__pyx_t_17);
-        __pyx_t_18 = __Pyx_PyObject_GetAttrStr(__pyx_t_17, __pyx_n_s_disable); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 577, __pyx_L19_except_error)
+        __pyx_t_18 = __Pyx_PyObject_GetAttrStr(__pyx_t_17, __pyx_n_s_disable); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 580, __pyx_L19_except_error)
         __Pyx_GOTREF(__pyx_t_18);
         __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
         __pyx_t_17 = NULL;
         __pyx_t_5 = 0;
         #if CYTHON_UNPACK_METHODS
         if (unlikely(PyMethod_Check(__pyx_t_18))) {
           __pyx_t_17 = PyMethod_GET_SELF(__pyx_t_18);
@@ -35950,33 +35968,33 @@
           }
         }
         #endif
         {
           PyObject *__pyx_callargs[2] = {__pyx_t_17, NULL};
           __pyx_t_16 = __Pyx_PyObject_FastCall(__pyx_t_18, __pyx_callargs+1-__pyx_t_5, 0+__pyx_t_5);
           __Pyx_XDECREF(__pyx_t_17); __pyx_t_17 = 0;
-          if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 577, __pyx_L19_except_error)
+          if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 580, __pyx_L19_except_error)
           __Pyx_GOTREF(__pyx_t_16);
           __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
         }
         __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
 
-        /* "src/cmodules/cyincludes/cyoptimizer.pyx":578
+        /* "src/cmodules/cyincludes/cyoptimizer.pyx":581
  *                 else: return None
  *                 gc.disable()
  *                 data = pickle.loads(gr.pkl)             # <<<<<<<<<<<<<<
  *                 gc.enable()
  *                 data = data.contiguous()
  */
-        __Pyx_GetModuleGlobalName(__pyx_t_18, __pyx_n_s_pickle); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 578, __pyx_L19_except_error)
+        __Pyx_GetModuleGlobalName(__pyx_t_18, __pyx_n_s_pickle); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 581, __pyx_L19_except_error)
         __Pyx_GOTREF(__pyx_t_18);
-        __pyx_t_17 = __Pyx_PyObject_GetAttrStr(__pyx_t_18, __pyx_n_s_loads); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 578, __pyx_L19_except_error)
+        __pyx_t_17 = __Pyx_PyObject_GetAttrStr(__pyx_t_18, __pyx_n_s_loads); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 581, __pyx_L19_except_error)
         __Pyx_GOTREF(__pyx_t_17);
         __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
-        __pyx_t_18 = __pyx_convert_PyBytes_string_to_py_6libcpp_6string_std__in_string(__pyx_v_gr->pkl); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 578, __pyx_L19_except_error)
+        __pyx_t_18 = __pyx_convert_PyBytes_string_to_py_6libcpp_6string_std__in_string(__pyx_v_gr->pkl); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 581, __pyx_L19_except_error)
         __Pyx_GOTREF(__pyx_t_18);
         __pyx_t_19 = NULL;
         __pyx_t_5 = 0;
         #if CYTHON_UNPACK_METHODS
         if (unlikely(PyMethod_Check(__pyx_t_17))) {
           __pyx_t_19 = PyMethod_GET_SELF(__pyx_t_17);
           if (likely(__pyx_t_19)) {
@@ -35989,31 +36007,31 @@
         }
         #endif
         {
           PyObject *__pyx_callargs[2] = {__pyx_t_19, __pyx_t_18};
           __pyx_t_16 = __Pyx_PyObject_FastCall(__pyx_t_17, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
           __Pyx_XDECREF(__pyx_t_19); __pyx_t_19 = 0;
           __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
-          if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 578, __pyx_L19_except_error)
+          if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 581, __pyx_L19_except_error)
           __Pyx_GOTREF(__pyx_t_16);
           __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
         }
         __Pyx_XDECREF_SET(__pyx_v_data, __pyx_t_16);
         __pyx_t_16 = 0;
 
-        /* "src/cmodules/cyincludes/cyoptimizer.pyx":579
+        /* "src/cmodules/cyincludes/cyoptimizer.pyx":582
  *                 gc.disable()
  *                 data = pickle.loads(gr.pkl)
  *                 gc.enable()             # <<<<<<<<<<<<<<
  *                 data = data.contiguous()
  *                 if cuda[0] is None: data = data.cpu()
  */
-        __Pyx_GetModuleGlobalName(__pyx_t_17, __pyx_n_s_gc); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 579, __pyx_L19_except_error)
+        __Pyx_GetModuleGlobalName(__pyx_t_17, __pyx_n_s_gc); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 582, __pyx_L19_except_error)
         __Pyx_GOTREF(__pyx_t_17);
-        __pyx_t_18 = __Pyx_PyObject_GetAttrStr(__pyx_t_17, __pyx_n_s_enable); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 579, __pyx_L19_except_error)
+        __pyx_t_18 = __Pyx_PyObject_GetAttrStr(__pyx_t_17, __pyx_n_s_enable); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 582, __pyx_L19_except_error)
         __Pyx_GOTREF(__pyx_t_18);
         __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
         __pyx_t_17 = NULL;
         __pyx_t_5 = 0;
         #if CYTHON_UNPACK_METHODS
         if (unlikely(PyMethod_Check(__pyx_t_18))) {
           __pyx_t_17 = PyMethod_GET_SELF(__pyx_t_18);
@@ -36026,28 +36044,28 @@
           }
         }
         #endif
         {
           PyObject *__pyx_callargs[2] = {__pyx_t_17, NULL};
           __pyx_t_16 = __Pyx_PyObject_FastCall(__pyx_t_18, __pyx_callargs+1-__pyx_t_5, 0+__pyx_t_5);
           __Pyx_XDECREF(__pyx_t_17); __pyx_t_17 = 0;
-          if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 579, __pyx_L19_except_error)
+          if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 582, __pyx_L19_except_error)
           __Pyx_GOTREF(__pyx_t_16);
           __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
         }
         __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
 
-        /* "src/cmodules/cyincludes/cyoptimizer.pyx":580
+        /* "src/cmodules/cyincludes/cyoptimizer.pyx":583
  *                 data = pickle.loads(gr.pkl)
  *                 gc.enable()
  *                 data = data.contiguous()             # <<<<<<<<<<<<<<
  *                 if cuda[0] is None: data = data.cpu()
  *                 else: data = data.cuda(device = self.device)
  */
-        __pyx_t_18 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_contiguous); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 580, __pyx_L19_except_error)
+        __pyx_t_18 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_contiguous); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 583, __pyx_L19_except_error)
         __Pyx_GOTREF(__pyx_t_18);
         __pyx_t_17 = NULL;
         __pyx_t_5 = 0;
         #if CYTHON_UNPACK_METHODS
         if (likely(PyMethod_Check(__pyx_t_18))) {
           __pyx_t_17 = PyMethod_GET_SELF(__pyx_t_18);
           if (likely(__pyx_t_17)) {
@@ -36059,38 +36077,38 @@
           }
         }
         #endif
         {
           PyObject *__pyx_callargs[2] = {__pyx_t_17, NULL};
           __pyx_t_16 = __Pyx_PyObject_FastCall(__pyx_t_18, __pyx_callargs+1-__pyx_t_5, 0+__pyx_t_5);
           __Pyx_XDECREF(__pyx_t_17); __pyx_t_17 = 0;
-          if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 580, __pyx_L19_except_error)
+          if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 583, __pyx_L19_except_error)
           __Pyx_GOTREF(__pyx_t_16);
           __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
         }
         __Pyx_DECREF_SET(__pyx_v_data, __pyx_t_16);
         __pyx_t_16 = 0;
 
-        /* "src/cmodules/cyincludes/cyoptimizer.pyx":581
+        /* "src/cmodules/cyincludes/cyoptimizer.pyx":584
  *                 gc.enable()
  *                 data = data.contiguous()
  *                 if cuda[0] is None: data = data.cpu()             # <<<<<<<<<<<<<<
  *                 else: data = data.cuda(device = self.device)
  *                 self.online[env(t_hash)] = data
  */
         if (unlikely(__pyx_v_cuda == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-          __PYX_ERR(0, 581, __pyx_L19_except_error)
+          __PYX_ERR(0, 584, __pyx_L19_except_error)
         }
-        __pyx_t_16 = __Pyx_GetItemInt_Tuple(__pyx_v_cuda, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 581, __pyx_L19_except_error)
+        __pyx_t_16 = __Pyx_GetItemInt_Tuple(__pyx_v_cuda, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 584, __pyx_L19_except_error)
         __Pyx_GOTREF(__pyx_t_16);
         __pyx_t_1 = (__pyx_t_16 == Py_None);
         __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
         if (__pyx_t_1) {
-          __pyx_t_18 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_cpu); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 581, __pyx_L19_except_error)
+          __pyx_t_18 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_cpu); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 584, __pyx_L19_except_error)
           __Pyx_GOTREF(__pyx_t_18);
           __pyx_t_17 = NULL;
           __pyx_t_5 = 0;
           #if CYTHON_UNPACK_METHODS
           if (likely(PyMethod_Check(__pyx_t_18))) {
             __pyx_t_17 = PyMethod_GET_SELF(__pyx_t_18);
             if (likely(__pyx_t_17)) {
@@ -36102,68 +36120,68 @@
             }
           }
           #endif
           {
             PyObject *__pyx_callargs[2] = {__pyx_t_17, NULL};
             __pyx_t_16 = __Pyx_PyObject_FastCall(__pyx_t_18, __pyx_callargs+1-__pyx_t_5, 0+__pyx_t_5);
             __Pyx_XDECREF(__pyx_t_17); __pyx_t_17 = 0;
-            if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 581, __pyx_L19_except_error)
+            if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 584, __pyx_L19_except_error)
             __Pyx_GOTREF(__pyx_t_16);
             __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
           }
           __Pyx_DECREF_SET(__pyx_v_data, __pyx_t_16);
           __pyx_t_16 = 0;
           goto __pyx_L28;
         }
 
-        /* "src/cmodules/cyincludes/cyoptimizer.pyx":582
+        /* "src/cmodules/cyincludes/cyoptimizer.pyx":585
  *                 data = data.contiguous()
  *                 if cuda[0] is None: data = data.cpu()
  *                 else: data = data.cuda(device = self.device)             # <<<<<<<<<<<<<<
  *                 self.online[env(t_hash)] = data
  * 
  */
         /*else*/ {
-          __pyx_t_16 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_cuda); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 582, __pyx_L19_except_error)
+          __pyx_t_16 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_cuda); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 585, __pyx_L19_except_error)
           __Pyx_GOTREF(__pyx_t_16);
-          __pyx_t_18 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 582, __pyx_L19_except_error)
+          __pyx_t_18 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 585, __pyx_L19_except_error)
           __Pyx_GOTREF(__pyx_t_18);
-          if (PyDict_SetItem(__pyx_t_18, __pyx_n_s_device, __pyx_v_self->device) < 0) __PYX_ERR(0, 582, __pyx_L19_except_error)
-          __pyx_t_17 = __Pyx_PyObject_Call(__pyx_t_16, __pyx_empty_tuple, __pyx_t_18); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 582, __pyx_L19_except_error)
+          if (PyDict_SetItem(__pyx_t_18, __pyx_n_s_device, __pyx_v_self->device) < 0) __PYX_ERR(0, 585, __pyx_L19_except_error)
+          __pyx_t_17 = __Pyx_PyObject_Call(__pyx_t_16, __pyx_empty_tuple, __pyx_t_18); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 585, __pyx_L19_except_error)
           __Pyx_GOTREF(__pyx_t_17);
           __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
           __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
           __Pyx_DECREF_SET(__pyx_v_data, __pyx_t_17);
           __pyx_t_17 = 0;
         }
         __pyx_L28:;
 
-        /* "src/cmodules/cyincludes/cyoptimizer.pyx":583
+        /* "src/cmodules/cyincludes/cyoptimizer.pyx":586
  *                 if cuda[0] is None: data = data.cpu()
  *                 else: data = data.cuda(device = self.device)
  *                 self.online[env(t_hash)] = data             # <<<<<<<<<<<<<<
  * 
  *             out.append(data)
  */
         if (unlikely(__pyx_v_self->online == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-          __PYX_ERR(0, 583, __pyx_L19_except_error)
+          __PYX_ERR(0, 586, __pyx_L19_except_error)
         }
-        __pyx_t_17 = __pyx_f_7cytools_env(__pyx_v_t_hash); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 583, __pyx_L19_except_error)
+        __pyx_t_17 = __pyx_f_7cytools_env(__pyx_v_t_hash); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 586, __pyx_L19_except_error)
         __Pyx_GOTREF(__pyx_t_17);
-        if (unlikely((PyDict_SetItem(__pyx_v_self->online, __pyx_t_17, __pyx_v_data) < 0))) __PYX_ERR(0, 583, __pyx_L19_except_error)
+        if (unlikely((PyDict_SetItem(__pyx_v_self->online, __pyx_t_17, __pyx_v_data) < 0))) __PYX_ERR(0, 586, __pyx_L19_except_error)
         __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
         __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
         goto __pyx_L18_exception_handled;
       }
       goto __pyx_L19_except_error;
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":572
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":575
  *         cdef k_graphed* gr
  *         for t_hash in dereference(hash_):
  *             try: data = self.online[env(t_hash)]             # <<<<<<<<<<<<<<
  *             except KeyError:
  *                 gr = self.this_batch[t_hash]
  */
       __pyx_L19_except_error:;
@@ -36182,52 +36200,52 @@
       __Pyx_XGIVEREF(__pyx_t_12);
       __Pyx_XGIVEREF(__pyx_t_11);
       __Pyx_XGIVEREF(__pyx_t_10);
       __Pyx_ExceptionReset(__pyx_t_12, __pyx_t_11, __pyx_t_10);
       __pyx_L24_try_end:;
     }
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":585
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":588
  *                 self.online[env(t_hash)] = data
  * 
  *             out.append(data)             # <<<<<<<<<<<<<<
  *             hashes.append(t_hash)
  *         data = Batch().from_data_list(out)
  */
-    __pyx_t_9 = __Pyx_PyList_Append(__pyx_v_out, __pyx_v_data); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(0, 585, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyList_Append(__pyx_v_out, __pyx_v_data); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(0, 588, __pyx_L1_error)
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":586
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":589
  * 
  *             out.append(data)
  *             hashes.append(t_hash)             # <<<<<<<<<<<<<<
  *         data = Batch().from_data_list(out)
  *         out = []
  */
-    __pyx_t_4 = __pyx_convert_PyBytes_string_to_py_6libcpp_6string_std__in_string(__pyx_v_t_hash); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 586, __pyx_L1_error)
+    __pyx_t_4 = __pyx_convert_PyBytes_string_to_py_6libcpp_6string_std__in_string(__pyx_v_t_hash); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 589, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_9 = __Pyx_PyList_Append(__pyx_v_hashes, __pyx_t_4); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(0, 586, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyList_Append(__pyx_v_hashes, __pyx_t_4); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(0, 589, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":571
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":574
  *         cdef string t_hash
  *         cdef k_graphed* gr
  *         for t_hash in dereference(hash_):             # <<<<<<<<<<<<<<
  *             try: data = self.online[env(t_hash)]
  *             except KeyError:
  */
   }
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":587
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":590
  *             out.append(data)
  *             hashes.append(t_hash)
  *         data = Batch().from_data_list(out)             # <<<<<<<<<<<<<<
  *         out = []
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Batch); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 587, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Batch); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 590, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_17 = NULL;
   __pyx_t_5 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_17 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_17)) {
@@ -36239,19 +36257,19 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_17, NULL};
     __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 0+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_17); __pyx_t_17 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 587, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 590, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_from_data_list); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 587, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_from_data_list); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 590, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   __pyx_t_5 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
@@ -36264,153 +36282,153 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_2, __pyx_v_out};
     __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 587, __pyx_L1_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 590, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __Pyx_XDECREF_SET(__pyx_v_data, __pyx_t_4);
   __pyx_t_4 = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":588
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":591
  *             hashes.append(t_hash)
  *         data = Batch().from_data_list(out)
  *         out = []             # <<<<<<<<<<<<<<
  * 
  *         self.purge = False
  */
-  __pyx_t_4 = PyList_New(0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 588, __pyx_L1_error)
+  __pyx_t_4 = PyList_New(0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 591, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF_SET(__pyx_v_out, ((PyObject*)__pyx_t_4));
   __pyx_t_4 = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":590
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":593
  *         out = []
  * 
  *         self.purge = False             # <<<<<<<<<<<<<<
  *         if (cuda[1] - cuda[0])/(1024**3) < idx: return data, hashes
  * 
  */
   __pyx_v_self->purge = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":591
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":594
  * 
  *         self.purge = False
  *         if (cuda[1] - cuda[0])/(1024**3) < idx: return data, hashes             # <<<<<<<<<<<<<<
  * 
  *         self.purge = True
  */
   if (unlikely(__pyx_v_cuda == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-    __PYX_ERR(0, 591, __pyx_L1_error)
+    __PYX_ERR(0, 594, __pyx_L1_error)
   }
-  __pyx_t_4 = __Pyx_GetItemInt_Tuple(__pyx_v_cuda, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 591, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_GetItemInt_Tuple(__pyx_v_cuda, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 594, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   if (unlikely(__pyx_v_cuda == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-    __PYX_ERR(0, 591, __pyx_L1_error)
+    __PYX_ERR(0, 594, __pyx_L1_error)
   }
-  __pyx_t_3 = __Pyx_GetItemInt_Tuple(__pyx_v_cuda, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 591, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_GetItemInt_Tuple(__pyx_v_cuda, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 594, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = PyNumber_Subtract(__pyx_t_4, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 591, __pyx_L1_error)
+  __pyx_t_2 = PyNumber_Subtract(__pyx_t_4, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 594, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyInt_TrueDivideObjC(__pyx_t_2, __pyx_int_1073741824, 0x40000000, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 591, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_TrueDivideObjC(__pyx_t_2, __pyx_int_1073741824, 0x40000000, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 594, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_idx); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 591, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_idx); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 594, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = PyObject_RichCompare(__pyx_t_3, __pyx_t_2, Py_LT); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 591, __pyx_L1_error)
+  __pyx_t_4 = PyObject_RichCompare(__pyx_t_3, __pyx_t_2, Py_LT); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 594, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 591, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 594, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (__pyx_t_1) {
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 591, __pyx_L1_error)
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 594, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_INCREF(__pyx_v_data);
     __Pyx_GIVEREF(__pyx_v_data);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_v_data)) __PYX_ERR(0, 591, __pyx_L1_error);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_v_data)) __PYX_ERR(0, 594, __pyx_L1_error);
     __Pyx_INCREF(__pyx_v_hashes);
     __Pyx_GIVEREF(__pyx_v_hashes);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_v_hashes)) __PYX_ERR(0, 591, __pyx_L1_error);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_v_hashes)) __PYX_ERR(0, 594, __pyx_L1_error);
     __pyx_r = __pyx_t_4;
     __pyx_t_4 = 0;
     goto __pyx_L0;
   }
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":593
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":596
  *         if (cuda[1] - cuda[0])/(1024**3) < idx: return data, hashes
  * 
  *         self.purge = True             # <<<<<<<<<<<<<<
  *         for k in self.online.values(): del k
  *         self.online.clear()
  */
   __pyx_v_self->purge = 1;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":594
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":597
  * 
  *         self.purge = True
  *         for k in self.online.values(): del k             # <<<<<<<<<<<<<<
  *         self.online.clear()
  *         torch.cuda.empty_cache()
  */
   __pyx_t_7 = 0;
   if (unlikely(__pyx_v_self->online == Py_None)) {
     PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "values");
-    __PYX_ERR(0, 594, __pyx_L1_error)
+    __PYX_ERR(0, 597, __pyx_L1_error)
   }
-  __pyx_t_2 = __Pyx_dict_iterator(__pyx_v_self->online, 1, __pyx_n_s_values, (&__pyx_t_6), (&__pyx_t_5)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 594, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_dict_iterator(__pyx_v_self->online, 1, __pyx_n_s_values, (&__pyx_t_6), (&__pyx_t_5)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 597, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_4);
   __pyx_t_4 = __pyx_t_2;
   __pyx_t_2 = 0;
   while (1) {
     __pyx_t_8 = __Pyx_dict_iter_next(__pyx_t_4, __pyx_t_6, &__pyx_t_7, NULL, &__pyx_t_2, NULL, __pyx_t_5);
     if (unlikely(__pyx_t_8 == 0)) break;
-    if (unlikely(__pyx_t_8 == -1)) __PYX_ERR(0, 594, __pyx_L1_error)
+    if (unlikely(__pyx_t_8 == -1)) __PYX_ERR(0, 597, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_v_k = __pyx_t_2;
     __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_v_k); __pyx_v_k = 0;
   }
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":595
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":598
  *         self.purge = True
  *         for k in self.online.values(): del k
  *         self.online.clear()             # <<<<<<<<<<<<<<
  *         torch.cuda.empty_cache()
  *         return data, hashes
  */
   if (unlikely(__pyx_v_self->online == Py_None)) {
     PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "clear");
-    __PYX_ERR(0, 595, __pyx_L1_error)
+    __PYX_ERR(0, 598, __pyx_L1_error)
   }
-  __pyx_t_9 = __Pyx_PyDict_Clear(__pyx_v_self->online); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(0, 595, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyDict_Clear(__pyx_v_self->online); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(0, 598, __pyx_L1_error)
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":596
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":599
  *         for k in self.online.values(): del k
  *         self.online.clear()
  *         torch.cuda.empty_cache()             # <<<<<<<<<<<<<<
  *         return data, hashes
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_torch); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 596, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_torch); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 599, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_cuda); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 596, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_cuda); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 599, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_empty_cache); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 596, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_empty_cache); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 599, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = NULL;
   __pyx_t_5 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
@@ -36423,41 +36441,41 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_3, NULL};
     __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_5, 0+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 596, __pyx_L1_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 599, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":597
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":600
  *         self.online.clear()
  *         torch.cuda.empty_cache()
  *         return data, hashes             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 597, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 600, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_INCREF(__pyx_v_data);
   __Pyx_GIVEREF(__pyx_v_data);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_v_data)) __PYX_ERR(0, 597, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_v_data)) __PYX_ERR(0, 600, __pyx_L1_error);
   __Pyx_INCREF(__pyx_v_hashes);
   __Pyx_GIVEREF(__pyx_v_hashes);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_v_hashes)) __PYX_ERR(0, 597, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_v_hashes)) __PYX_ERR(0, 600, __pyx_L1_error);
   __pyx_r = __pyx_t_4;
   __pyx_t_4 = 0;
   goto __pyx_L0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":548
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":551
  *         return self
  * 
  *     def __next__(self):             # <<<<<<<<<<<<<<
  *         if self.indx_s == self.indx_e: raise StopIteration
  *         cdef vector[string]* hash_ = &self.batch_hash[self.indx_s]
  */
 
@@ -36481,15 +36499,15 @@
   __Pyx_XDECREF(__pyx_v_hashes);
   __Pyx_XDECREF(__pyx_v_data);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/cmodules/cyincludes/cyoptimizer.pyx":485
+/* "src/cmodules/cyincludes/cyoptimizer.pyx":488
  *     cdef str device
  *     cdef dict online
  *     cdef public bool purge             # <<<<<<<<<<<<<<
  *     cdef public sampletracer
  *     cdef public int threads
  */
 
@@ -36513,15 +36531,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 1);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_v_self->purge); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 485, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_v_self->purge); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 488, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -36551,28 +36569,28 @@
 
 static int __pyx_pf_9AnalysisG_9_cmodules_10cOptimizer_10DataLoader_5purge_2__set__(struct __pyx_obj_9AnalysisG_9_cmodules_10cOptimizer_DataLoader *__pyx_v_self, PyObject *__pyx_v_value) {
   int __pyx_r;
   bool __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_value); if (unlikely((__pyx_t_1 == ((bool)-1)) && PyErr_Occurred())) __PYX_ERR(0, 485, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_value); if (unlikely((__pyx_t_1 == ((bool)-1)) && PyErr_Occurred())) __PYX_ERR(0, 488, __pyx_L1_error)
   __pyx_v_self->purge = __pyx_t_1;
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("AnalysisG._cmodules.cOptimizer.DataLoader.purge.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "src/cmodules/cyincludes/cyoptimizer.pyx":486
+/* "src/cmodules/cyincludes/cyoptimizer.pyx":489
  *     cdef dict online
  *     cdef public bool purge
  *     cdef public sampletracer             # <<<<<<<<<<<<<<
  *     cdef public int threads
  * 
  */
 
@@ -36665,15 +36683,15 @@
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/cmodules/cyincludes/cyoptimizer.pyx":487
+/* "src/cmodules/cyincludes/cyoptimizer.pyx":490
  *     cdef public bool purge
  *     cdef public sampletracer
  *     cdef public int threads             # <<<<<<<<<<<<<<
  * 
  *     def __cinit__(self):
  */
 
@@ -36697,15 +36715,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 1);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->threads); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 487, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->threads); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 490, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -36735,15 +36753,15 @@
 
 static int __pyx_pf_9AnalysisG_9_cmodules_10cOptimizer_10DataLoader_7threads_2__set__(struct __pyx_obj_9AnalysisG_9_cmodules_10cOptimizer_DataLoader *__pyx_v_self, PyObject *__pyx_v_value) {
   int __pyx_r;
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_value); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 487, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_value); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 490, __pyx_L1_error)
   __pyx_v_self->threads = __pyx_t_1;
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("AnalysisG._cmodules.cOptimizer.DataLoader.threads.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
@@ -36962,15 +36980,15 @@
   __Pyx_AddTraceback("AnalysisG._cmodules.cOptimizer.DataLoader.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/cmodules/cyincludes/cyoptimizer.pyx":614
+/* "src/cmodules/cyincludes/cyoptimizer.pyx":617
  *     cdef public sampletracer
  * 
  *     def __cinit__(self):             # <<<<<<<<<<<<<<
  *         self.ptr = new CyOptimizer()
  *         self.data = DataLoader()
  */
 
@@ -37005,104 +37023,104 @@
   PyObject *__pyx_t_2 = NULL;
   struct __pyx_t_11cyoptimizer_report_t __pyx_t_3;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__cinit__", 1);
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":615
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":618
  * 
  *     def __cinit__(self):
  *         self.ptr = new CyOptimizer()             # <<<<<<<<<<<<<<
  *         self.data = DataLoader()
  *         self.data.ptr = self.ptr
  */
   try {
     __pyx_t_1 = new Optimizer::CyOptimizer();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 615, __pyx_L1_error)
+    __PYX_ERR(0, 618, __pyx_L1_error)
   }
   __pyx_v_self->ptr = __pyx_t_1;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":616
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":619
  *     def __cinit__(self):
  *         self.ptr = new CyOptimizer()
  *         self.data = DataLoader()             # <<<<<<<<<<<<<<
  *         self.data.ptr = self.ptr
  *         self.sampletracer = None
  */
-  __pyx_t_2 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_DataLoader)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 616, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_DataLoader)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 619, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_2);
   __Pyx_GOTREF((PyObject *)__pyx_v_self->data);
   __Pyx_DECREF((PyObject *)__pyx_v_self->data);
   __pyx_v_self->data = ((struct __pyx_obj_9AnalysisG_9_cmodules_10cOptimizer_DataLoader *)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":617
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":620
  *         self.ptr = new CyOptimizer()
  *         self.data = DataLoader()
  *         self.data.ptr = self.ptr             # <<<<<<<<<<<<<<
  *         self.sampletracer = None
  *         self._train = False
  */
   __pyx_t_1 = __pyx_v_self->ptr;
   __pyx_v_self->data->ptr = __pyx_t_1;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":618
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":621
  *         self.data = DataLoader()
  *         self.data.ptr = self.ptr
  *         self.sampletracer = None             # <<<<<<<<<<<<<<
  *         self._train = False
  *         self._test = False
  */
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
   __Pyx_GOTREF(__pyx_v_self->sampletracer);
   __Pyx_DECREF(__pyx_v_self->sampletracer);
   __pyx_v_self->sampletracer = Py_None;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":619
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":622
  *         self.data.ptr = self.ptr
  *         self.sampletracer = None
  *         self._train = False             # <<<<<<<<<<<<<<
  *         self._test = False
  *         self._val = False
  */
   __pyx_v_self->_train = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":620
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":623
  *         self.sampletracer = None
  *         self._train = False
  *         self._test = False             # <<<<<<<<<<<<<<
  *         self._val = False
  *         self.state = report_t()
  */
   __pyx_v_self->_test = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":621
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":624
  *         self._train = False
  *         self._test = False
  *         self._val = False             # <<<<<<<<<<<<<<
  *         self.state = report_t()
  * 
  */
   __pyx_v_self->_val = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":622
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":625
  *         self._test = False
  *         self._val = False
  *         self.state = report_t()             # <<<<<<<<<<<<<<
  * 
  *     def __init__(self): pass
  */
   __pyx_v_self->state = __pyx_t_3;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":614
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":617
  *     cdef public sampletracer
  * 
  *     def __cinit__(self):             # <<<<<<<<<<<<<<
  *         self.ptr = new CyOptimizer()
  *         self.data = DataLoader()
  */
 
@@ -37114,15 +37132,15 @@
   __Pyx_AddTraceback("AnalysisG._cmodules.cOptimizer.cOptimizer.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/cmodules/cyincludes/cyoptimizer.pyx":624
+/* "src/cmodules/cyincludes/cyoptimizer.pyx":627
  *         self.state = report_t()
  * 
  *     def __init__(self): pass             # <<<<<<<<<<<<<<
  *     def __dealloc__(self): del self.ptr
  * 
  */
 
@@ -37154,15 +37172,15 @@
   int __pyx_r;
 
   /* function exit code */
   __pyx_r = 0;
   return __pyx_r;
 }
 
-/* "src/cmodules/cyincludes/cyoptimizer.pyx":625
+/* "src/cmodules/cyincludes/cyoptimizer.pyx":628
  * 
  *     def __init__(self): pass
  *     def __dealloc__(self): del self.ptr             # <<<<<<<<<<<<<<
  * 
  *     def length(self):
  */
 
@@ -37181,15 +37199,15 @@
 
 static void __pyx_pf_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_4__dealloc__(struct __pyx_obj_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer *__pyx_v_self) {
   delete __pyx_v_self->ptr;
 
   /* function exit code */
 }
 
-/* "src/cmodules/cyincludes/cyoptimizer.pyx":627
+/* "src/cmodules/cyincludes/cyoptimizer.pyx":630
  *     def __dealloc__(self): del self.ptr
  * 
  *     def length(self):             # <<<<<<<<<<<<<<
  *         return map_to_dict(<map[string, int]>self.ptr.fold_map())
  * 
  */
 
@@ -37240,35 +37258,35 @@
   std::map<std::string,int>  __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("length", 1);
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":628
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":631
  * 
  *     def length(self):
  *         return map_to_dict(<map[string, int]>self.ptr.fold_map())             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
   try {
     __pyx_t_1 = __pyx_v_self->ptr->fold_map();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 628, __pyx_L1_error)
+    __PYX_ERR(0, 631, __pyx_L1_error)
   }
-  __pyx_t_2 = __pyx_fuse_0__pyx_f_7cytools_map_to_dict(((std::map<std::string,int> )__pyx_t_1)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 628, __pyx_L1_error)
+  __pyx_t_2 = __pyx_fuse_0__pyx_f_7cytools_map_to_dict(((std::map<std::string,int> )__pyx_t_1)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 631, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":627
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":630
  *     def __dealloc__(self): del self.ptr
  * 
  *     def length(self):             # <<<<<<<<<<<<<<
  *         return map_to_dict(<map[string, int]>self.ptr.fold_map())
  * 
  */
 
@@ -37279,15 +37297,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/cmodules/cyincludes/cyoptimizer.pyx":630
+/* "src/cmodules/cyincludes/cyoptimizer.pyx":633
  *         return map_to_dict(<map[string, int]>self.ptr.fold_map())
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def kFolds(self): return self.ptr.use_folds
  * 
  */
 
@@ -37311,29 +37329,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 1);
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":631
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":634
  * 
  *     @property
  *     def kFolds(self): return self.ptr.use_folds             # <<<<<<<<<<<<<<
  * 
  *     cpdef report_t reportable(self): return self.state
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_convert_vector_to_py_int(__pyx_v_self->ptr->use_folds); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 631, __pyx_L1_error)
+  __pyx_t_1 = __pyx_convert_vector_to_py_int(__pyx_v_self->ptr->use_folds); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 634, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":630
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":633
  *         return map_to_dict(<map[string, int]>self.ptr.fold_map())
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def kFolds(self): return self.ptr.use_folds
  * 
  */
 
@@ -37344,15 +37362,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/cmodules/cyincludes/cyoptimizer.pyx":633
+/* "src/cmodules/cyincludes/cyoptimizer.pyx":636
  *     def kFolds(self): return self.ptr.use_folds
  * 
  *     cpdef report_t reportable(self): return self.state             # <<<<<<<<<<<<<<
  * 
  *     cpdef bool GetHDF5Hashes(self, str path):
  */
 
@@ -37381,15 +37399,15 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || __Pyx_PyType_HasFeature(Py_TYPE(((PyObject *)__pyx_v_self)), (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_typedict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_reportable); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 633, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_reportable); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 636, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!__Pyx_IsSameCFunction(__pyx_t_1, (void*) __pyx_pw_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_9reportable)) {
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         __pyx_t_5 = 0;
         #if CYTHON_UNPACK_METHODS
         if (unlikely(PyMethod_Check(__pyx_t_3))) {
@@ -37403,19 +37421,19 @@
           }
         }
         #endif
         {
           PyObject *__pyx_callargs[2] = {__pyx_t_4, NULL};
           __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 0+__pyx_t_5);
           __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-          if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 633, __pyx_L1_error)
+          if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 636, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         }
-        __pyx_t_6 = __pyx_convert__from_py_struct____pyx_t_11cyoptimizer_report_t(__pyx_t_2); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 633, __pyx_L1_error)
+        __pyx_t_6 = __pyx_convert__from_py_struct____pyx_t_11cyoptimizer_report_t(__pyx_t_2); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 636, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __pyx_r = __pyx_t_6;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
       __pyx_tp_dict_version = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
@@ -37492,16 +37510,16 @@
   struct __pyx_t_11cyoptimizer_report_t __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("reportable", 1);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_reportable(__pyx_v_self, 1); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 633, __pyx_L1_error)
-  __pyx_t_2 = __pyx_convert__to_py_struct____pyx_t_11cyoptimizer_report_t(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 633, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_reportable(__pyx_v_self, 1); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 636, __pyx_L1_error)
+  __pyx_t_2 = __pyx_convert__to_py_struct____pyx_t_11cyoptimizer_report_t(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 636, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -37510,15 +37528,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/cmodules/cyincludes/cyoptimizer.pyx":635
+/* "src/cmodules/cyincludes/cyoptimizer.pyx":638
  *     cpdef report_t reportable(self): return self.state
  * 
  *     cpdef bool GetHDF5Hashes(self, str path):             # <<<<<<<<<<<<<<
  *         if path.endswith(".hdf5"): pass
  *         else: path += ".hdf5"
  */
 
@@ -37576,15 +37594,15 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || __Pyx_PyType_HasFeature(Py_TYPE(((PyObject *)__pyx_v_self)), (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_typedict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_GetHDF5Hashes); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 635, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_GetHDF5Hashes); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 638, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!__Pyx_IsSameCFunction(__pyx_t_1, (void*) __pyx_pw_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_11GetHDF5Hashes)) {
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         __pyx_t_5 = 0;
         #if CYTHON_UNPACK_METHODS
         if (unlikely(PyMethod_Check(__pyx_t_3))) {
@@ -37598,19 +37616,19 @@
           }
         }
         #endif
         {
           PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_v_path};
           __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
           __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-          if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 635, __pyx_L1_error)
+          if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 638, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         }
-        __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely((__pyx_t_6 == ((bool)-1)) && PyErr_Occurred())) __PYX_ERR(0, 635, __pyx_L1_error)
+        __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely((__pyx_t_6 == ((bool)-1)) && PyErr_Occurred())) __PYX_ERR(0, 638, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __pyx_r = __pyx_t_6;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
       __pyx_tp_dict_version = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
@@ -37621,63 +37639,63 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":636
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":639
  * 
  *     cpdef bool GetHDF5Hashes(self, str path):
  *         if path.endswith(".hdf5"): pass             # <<<<<<<<<<<<<<
  *         else: path += ".hdf5"
  * 
  */
   if (unlikely(__pyx_v_path == Py_None)) {
     PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "endswith");
-    __PYX_ERR(0, 636, __pyx_L1_error)
+    __PYX_ERR(0, 639, __pyx_L1_error)
   }
-  __pyx_t_7 = __Pyx_PyUnicode_Tailmatch(__pyx_v_path, __pyx_kp_u_hdf5, 0, PY_SSIZE_T_MAX, 1); if (unlikely(__pyx_t_7 == ((int)-1))) __PYX_ERR(0, 636, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyUnicode_Tailmatch(__pyx_v_path, __pyx_kp_u_hdf5, 0, PY_SSIZE_T_MAX, 1); if (unlikely(__pyx_t_7 == ((int)-1))) __PYX_ERR(0, 639, __pyx_L1_error)
   if (__pyx_t_7) {
     goto __pyx_L3;
   }
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":637
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":640
  *     cpdef bool GetHDF5Hashes(self, str path):
  *         if path.endswith(".hdf5"): pass
  *         else: path += ".hdf5"             # <<<<<<<<<<<<<<
  * 
  *         try: f = h5py.File(path, "r")
  */
   /*else*/ {
-    __pyx_t_1 = __Pyx_PyUnicode_ConcatInPlaceSafe(__pyx_v_path, __pyx_kp_u_hdf5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 637, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyUnicode_ConcatInPlaceSafe(__pyx_v_path, __pyx_kp_u_hdf5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 640, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF_SET(__pyx_v_path, ((PyObject*)__pyx_t_1));
     __pyx_t_1 = 0;
   }
   __pyx_L3:;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":639
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":642
  *         else: path += ".hdf5"
  * 
  *         try: f = h5py.File(path, "r")             # <<<<<<<<<<<<<<
  *         except FileNotFoundError: return False
  * 
  */
   {
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_8, &__pyx_t_9, &__pyx_t_10);
     __Pyx_XGOTREF(__pyx_t_8);
     __Pyx_XGOTREF(__pyx_t_9);
     __Pyx_XGOTREF(__pyx_t_10);
     /*try:*/ {
-      __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_h5py); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 639, __pyx_L4_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_h5py); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 642, __pyx_L4_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_File); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 639, __pyx_L4_error)
+      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_File); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 642, __pyx_L4_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __pyx_t_2 = NULL;
       __pyx_t_5 = 0;
       #if CYTHON_UNPACK_METHODS
       if (unlikely(PyMethod_Check(__pyx_t_3))) {
         __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
@@ -37690,15 +37708,15 @@
         }
       }
       #endif
       {
         PyObject *__pyx_callargs[3] = {__pyx_t_2, __pyx_v_path, __pyx_n_u_r};
         __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 2+__pyx_t_5);
         __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-        if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 639, __pyx_L4_error)
+        if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 642, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       }
       __pyx_v_f = __pyx_t_1;
       __pyx_t_1 = 0;
     }
     __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
@@ -37707,43 +37725,43 @@
     goto __pyx_L9_try_end;
     __pyx_L4_error:;
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":640
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":643
  * 
  *         try: f = h5py.File(path, "r")
  *         except FileNotFoundError: return False             # <<<<<<<<<<<<<<
  * 
  *         cdef bool k
  */
     __Pyx_ErrFetch(&__pyx_t_1, &__pyx_t_3, &__pyx_t_2);
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_FileNotFoundError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 640, __pyx_L6_except_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_FileNotFoundError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 643, __pyx_L6_except_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = __Pyx_PyErr_GivenExceptionMatches(__pyx_t_1, __pyx_t_4);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_ErrRestore(__pyx_t_1, __pyx_t_3, __pyx_t_2);
     __pyx_t_1 = 0; __pyx_t_3 = 0; __pyx_t_2 = 0;
     if (__pyx_t_5) {
       __Pyx_AddTraceback("AnalysisG._cmodules.cOptimizer.cOptimizer.GetHDF5Hashes", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_2, &__pyx_t_3, &__pyx_t_1) < 0) __PYX_ERR(0, 640, __pyx_L6_except_error)
+      if (__Pyx_GetException(&__pyx_t_2, &__pyx_t_3, &__pyx_t_1) < 0) __PYX_ERR(0, 643, __pyx_L6_except_error)
       __Pyx_XGOTREF(__pyx_t_2);
       __Pyx_XGOTREF(__pyx_t_3);
       __Pyx_XGOTREF(__pyx_t_1);
       __pyx_r = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       goto __pyx_L7_except_return;
     }
     goto __pyx_L6_except_error;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":639
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":642
  *         else: path += ".hdf5"
  * 
  *         try: f = h5py.File(path, "r")             # <<<<<<<<<<<<<<
  *         except FileNotFoundError: return False
  * 
  */
     __pyx_L6_except_error:;
@@ -37757,155 +37775,155 @@
     __Pyx_XGIVEREF(__pyx_t_9);
     __Pyx_XGIVEREF(__pyx_t_10);
     __Pyx_ExceptionReset(__pyx_t_8, __pyx_t_9, __pyx_t_10);
     goto __pyx_L0;
     __pyx_L9_try_end:;
   }
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":645
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":648
  *         cdef str h_, h__
  *         cdef map[string, vector[tuple[string, bool]]] res
  *         for h_ in f: res[enc(h_)] = [(enc(h__), k) for h__, k in f[h_].attrs.items()]             # <<<<<<<<<<<<<<
  *         cdef vector[string] idx = <vector[string]>(list(res))
  * 
  */
   if (likely(PyList_CheckExact(__pyx_v_f)) || PyTuple_CheckExact(__pyx_v_f)) {
     __pyx_t_1 = __pyx_v_f; __Pyx_INCREF(__pyx_t_1);
     __pyx_t_11 = 0;
     __pyx_t_12 = NULL;
   } else {
-    __pyx_t_11 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_f); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 645, __pyx_L1_error)
+    __pyx_t_11 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_f); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 648, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_12 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_1); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 645, __pyx_L1_error)
+    __pyx_t_12 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_1); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 648, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_12)) {
       if (likely(PyList_CheckExact(__pyx_t_1))) {
         {
           Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_1);
           #if !CYTHON_ASSUME_SAFE_MACROS
-          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 645, __pyx_L1_error)
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 648, __pyx_L1_error)
           #endif
           if (__pyx_t_11 >= __pyx_temp) break;
         }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_3 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_11); __Pyx_INCREF(__pyx_t_3); __pyx_t_11++; if (unlikely((0 < 0))) __PYX_ERR(0, 645, __pyx_L1_error)
+        __pyx_t_3 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_11); __Pyx_INCREF(__pyx_t_3); __pyx_t_11++; if (unlikely((0 < 0))) __PYX_ERR(0, 648, __pyx_L1_error)
         #else
-        __pyx_t_3 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_11); __pyx_t_11++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 645, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_11); __pyx_t_11++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 648, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         #endif
       } else {
         {
           Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_1);
           #if !CYTHON_ASSUME_SAFE_MACROS
-          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 645, __pyx_L1_error)
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 648, __pyx_L1_error)
           #endif
           if (__pyx_t_11 >= __pyx_temp) break;
         }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_11); __Pyx_INCREF(__pyx_t_3); __pyx_t_11++; if (unlikely((0 < 0))) __PYX_ERR(0, 645, __pyx_L1_error)
+        __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_11); __Pyx_INCREF(__pyx_t_3); __pyx_t_11++; if (unlikely((0 < 0))) __PYX_ERR(0, 648, __pyx_L1_error)
         #else
-        __pyx_t_3 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_11); __pyx_t_11++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 645, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_11); __pyx_t_11++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 648, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         #endif
       }
     } else {
       __pyx_t_3 = __pyx_t_12(__pyx_t_1);
       if (unlikely(!__pyx_t_3)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 645, __pyx_L1_error)
+          else __PYX_ERR(0, 648, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_3);
     }
-    if (!(likely(PyUnicode_CheckExact(__pyx_t_3))||((__pyx_t_3) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_t_3))) __PYX_ERR(0, 645, __pyx_L1_error)
+    if (!(likely(PyUnicode_CheckExact(__pyx_t_3))||((__pyx_t_3) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_t_3))) __PYX_ERR(0, 648, __pyx_L1_error)
     __Pyx_XDECREF_SET(__pyx_v_h_, ((PyObject*)__pyx_t_3));
     __pyx_t_3 = 0;
     { /* enter inner scope */
-      __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 645, __pyx_L16_error)
+      __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 648, __pyx_L16_error)
       __Pyx_GOTREF(__pyx_t_3);
       __pyx_t_13 = 0;
-      __pyx_t_4 = __Pyx_PyObject_Dict_GetItem(__pyx_v_f, __pyx_v_h_); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 645, __pyx_L16_error)
+      __pyx_t_4 = __Pyx_PyObject_Dict_GetItem(__pyx_v_f, __pyx_v_h_); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 648, __pyx_L16_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_attrs); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 645, __pyx_L16_error)
+      __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_attrs); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 648, __pyx_L16_error)
       __Pyx_GOTREF(__pyx_t_15);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       if (unlikely(__pyx_t_15 == Py_None)) {
         PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "items");
-        __PYX_ERR(0, 645, __pyx_L16_error)
+        __PYX_ERR(0, 648, __pyx_L16_error)
       }
-      __pyx_t_4 = __Pyx_dict_iterator(__pyx_t_15, 0, __pyx_n_s_items, (&__pyx_t_14), (&__pyx_t_5)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 645, __pyx_L16_error)
+      __pyx_t_4 = __Pyx_dict_iterator(__pyx_t_15, 0, __pyx_n_s_items, (&__pyx_t_14), (&__pyx_t_5)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 648, __pyx_L16_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
       __Pyx_XDECREF(__pyx_t_2);
       __pyx_t_2 = __pyx_t_4;
       __pyx_t_4 = 0;
       while (1) {
         __pyx_t_16 = __Pyx_dict_iter_next(__pyx_t_2, __pyx_t_14, &__pyx_t_13, &__pyx_t_4, &__pyx_t_15, NULL, __pyx_t_5);
         if (unlikely(__pyx_t_16 == 0)) break;
-        if (unlikely(__pyx_t_16 == -1)) __PYX_ERR(0, 645, __pyx_L16_error)
+        if (unlikely(__pyx_t_16 == -1)) __PYX_ERR(0, 648, __pyx_L16_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_GOTREF(__pyx_t_15);
-        if (!(likely(PyUnicode_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_t_4))) __PYX_ERR(0, 645, __pyx_L16_error)
-        __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_15); if (unlikely((__pyx_t_6 == ((bool)-1)) && PyErr_Occurred())) __PYX_ERR(0, 645, __pyx_L16_error)
+        if (!(likely(PyUnicode_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_t_4))) __PYX_ERR(0, 648, __pyx_L16_error)
+        __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_15); if (unlikely((__pyx_t_6 == ((bool)-1)) && PyErr_Occurred())) __PYX_ERR(0, 648, __pyx_L16_error)
         __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
         __Pyx_XDECREF_SET(__pyx_8genexpr7__pyx_v_h__, ((PyObject*)__pyx_t_4));
         __pyx_t_4 = 0;
         __pyx_8genexpr7__pyx_v_k = __pyx_t_6;
-        __pyx_t_17 = __pyx_f_7cytools_enc(__pyx_8genexpr7__pyx_v_h__); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 645, __pyx_L16_error)
-        __pyx_t_15 = __pyx_convert_PyBytes_string_to_py_6libcpp_6string_std__in_string(__pyx_t_17); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 645, __pyx_L16_error)
+        __pyx_t_17 = __pyx_f_7cytools_enc(__pyx_8genexpr7__pyx_v_h__); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 648, __pyx_L16_error)
+        __pyx_t_15 = __pyx_convert_PyBytes_string_to_py_6libcpp_6string_std__in_string(__pyx_t_17); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 648, __pyx_L16_error)
         __Pyx_GOTREF(__pyx_t_15);
-        __pyx_t_4 = __Pyx_PyBool_FromLong(__pyx_8genexpr7__pyx_v_k); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 645, __pyx_L16_error)
+        __pyx_t_4 = __Pyx_PyBool_FromLong(__pyx_8genexpr7__pyx_v_k); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 648, __pyx_L16_error)
         __Pyx_GOTREF(__pyx_t_4);
-        __pyx_t_18 = PyTuple_New(2); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 645, __pyx_L16_error)
+        __pyx_t_18 = PyTuple_New(2); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 648, __pyx_L16_error)
         __Pyx_GOTREF(__pyx_t_18);
         __Pyx_GIVEREF(__pyx_t_15);
-        if (__Pyx_PyTuple_SET_ITEM(__pyx_t_18, 0, __pyx_t_15)) __PYX_ERR(0, 645, __pyx_L16_error);
+        if (__Pyx_PyTuple_SET_ITEM(__pyx_t_18, 0, __pyx_t_15)) __PYX_ERR(0, 648, __pyx_L16_error);
         __Pyx_GIVEREF(__pyx_t_4);
-        if (__Pyx_PyTuple_SET_ITEM(__pyx_t_18, 1, __pyx_t_4)) __PYX_ERR(0, 645, __pyx_L16_error);
+        if (__Pyx_PyTuple_SET_ITEM(__pyx_t_18, 1, __pyx_t_4)) __PYX_ERR(0, 648, __pyx_L16_error);
         __pyx_t_15 = 0;
         __pyx_t_4 = 0;
-        if (unlikely(__Pyx_ListComp_Append(__pyx_t_3, (PyObject*)__pyx_t_18))) __PYX_ERR(0, 645, __pyx_L16_error)
+        if (unlikely(__Pyx_ListComp_Append(__pyx_t_3, (PyObject*)__pyx_t_18))) __PYX_ERR(0, 648, __pyx_L16_error)
         __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
       }
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_XDECREF(__pyx_8genexpr7__pyx_v_h__); __pyx_8genexpr7__pyx_v_h__ = 0;
       goto __pyx_L19_exit_scope;
       __pyx_L16_error:;
       __Pyx_XDECREF(__pyx_8genexpr7__pyx_v_h__); __pyx_8genexpr7__pyx_v_h__ = 0;
       goto __pyx_L1_error;
       __pyx_L19_exit_scope:;
     } /* exit inner scope */
-    __pyx_t_19 = __pyx_convert_vector_from_py___pyx_ctuple_6libcpp_6string_std__in_string__and_6libcpp_bool(__pyx_t_3); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 645, __pyx_L1_error)
+    __pyx_t_19 = __pyx_convert_vector_from_py___pyx_ctuple_6libcpp_6string_std__in_string__and_6libcpp_bool(__pyx_t_3); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 648, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_17 = __pyx_f_7cytools_enc(__pyx_v_h_); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 645, __pyx_L1_error)
+    __pyx_t_17 = __pyx_f_7cytools_enc(__pyx_v_h_); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 648, __pyx_L1_error)
     (__pyx_v_res[__pyx_t_17]) = __pyx_t_19;
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":646
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":649
  *         cdef map[string, vector[tuple[string, bool]]] res
  *         for h_ in f: res[enc(h_)] = [(enc(h__), k) for h__, k in f[h_].attrs.items()]
  *         cdef vector[string] idx = <vector[string]>(list(res))             # <<<<<<<<<<<<<<
  * 
  *         cdef int i, j
  */
-  __pyx_t_1 = __pyx_convert_map_to_py_std_3a__3a_string____std_3a__3a_vector_3c___pyx_ctuple_6libcpp_6string_std__in_string__and_6libcpp_bool_3e___(__pyx_v_res); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 646, __pyx_L1_error)
+  __pyx_t_1 = __pyx_convert_map_to_py_std_3a__3a_string____std_3a__3a_vector_3c___pyx_ctuple_6libcpp_6string_std__in_string__and_6libcpp_bool_3e___(__pyx_v_res); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 649, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PySequence_ListKeepNew(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 646, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PySequence_ListKeepNew(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 649, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_20 = __pyx_convert_vector_from_py_std_3a__3a_string(__pyx_t_3); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 646, __pyx_L1_error)
+  __pyx_t_20 = __pyx_convert_vector_from_py_std_3a__3a_string(__pyx_t_3); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 649, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_idx = ((std::vector<std::string> )__pyx_t_20);
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":650
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":653
  *         cdef int i, j
  *         cdef map[string, vector[folds_t]] output
  *         for i in prange(idx.size(), nogil = True, num_threads = self.threads):             # <<<<<<<<<<<<<<
  *             output[idx[i]] = kfold_build(&idx[i], &res[idx[i]])
  *             for j in range(output[idx[i]].size()): self.ptr.register_fold(&output[idx[i]][j])
  */
   {
@@ -37949,24 +37967,24 @@
                     for (__pyx_t_22 = 0; __pyx_t_22 < __pyx_t_23; __pyx_t_22++){
                         if (__pyx_parallel_why < 2)
                         {
                             __pyx_v_i = (int)(0 + 1 * __pyx_t_22);
                             /* Initialize private variables to invalid values */
                             __pyx_v_j = ((int)0xbad0bad0);
 
-                            /* "src/cmodules/cyincludes/cyoptimizer.pyx":651
+                            /* "src/cmodules/cyincludes/cyoptimizer.pyx":654
  *         cdef map[string, vector[folds_t]] output
  *         for i in prange(idx.size(), nogil = True, num_threads = self.threads):
  *             output[idx[i]] = kfold_build(&idx[i], &res[idx[i]])             # <<<<<<<<<<<<<<
  *             for j in range(output[idx[i]].size()): self.ptr.register_fold(&output[idx[i]][j])
  *         output.clear()
  */
                             (__pyx_v_output[(__pyx_v_idx[__pyx_v_i])]) = __pyx_f_11cyoptimizer_kfold_build((&(__pyx_v_idx[__pyx_v_i])), (&(__pyx_v_res[(__pyx_v_idx[__pyx_v_i])])));
 
-                            /* "src/cmodules/cyincludes/cyoptimizer.pyx":652
+                            /* "src/cmodules/cyincludes/cyoptimizer.pyx":655
  *         for i in prange(idx.size(), nogil = True, num_threads = self.threads):
  *             output[idx[i]] = kfold_build(&idx[i], &res[idx[i]])
  *             for j in range(output[idx[i]].size()): self.ptr.register_fold(&output[idx[i]][j])             # <<<<<<<<<<<<<<
  *         output.clear()
  *         return True
  */
                             __pyx_t_24 = (__pyx_v_output[(__pyx_v_idx[__pyx_v_i])]).size();
@@ -37979,15 +37997,15 @@
                                 #ifdef WITH_THREAD
                                 PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
                                 #endif
                                 __Pyx_CppExn2PyErr();
                                 #ifdef WITH_THREAD
                                 __Pyx_PyGILState_Release(__pyx_gilstate_save);
                                 #endif
-                                __PYX_ERR(0, 652, __pyx_L26_error)
+                                __PYX_ERR(0, 655, __pyx_L26_error)
                               }
                             }
                             goto __pyx_L31;
                             __pyx_L26_error:;
                             {
                                 #ifdef WITH_THREAD
                                 PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
@@ -38065,15 +38083,15 @@
             #undef likely
             #undef unlikely
             #define likely(x)   __builtin_expect(!!(x), 1)
             #define unlikely(x) __builtin_expect(!!(x), 0)
         #endif
       }
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":650
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":653
  *         cdef int i, j
  *         cdef map[string, vector[folds_t]] output
  *         for i in prange(idx.size(), nogil = True, num_threads = self.threads):             # <<<<<<<<<<<<<<
  *             output[idx[i]] = kfold_build(&idx[i], &res[idx[i]])
  *             for j in range(output[idx[i]].size()): self.ptr.register_fold(&output[idx[i]][j])
  */
       /*finally:*/ {
@@ -38091,34 +38109,34 @@
           #endif
           goto __pyx_L1_error;
         }
         __pyx_L23:;
       }
   }
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":653
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":656
  *             output[idx[i]] = kfold_build(&idx[i], &res[idx[i]])
  *             for j in range(output[idx[i]].size()): self.ptr.register_fold(&output[idx[i]][j])
  *         output.clear()             # <<<<<<<<<<<<<<
  *         return True
  * 
  */
   __pyx_v_output.clear();
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":654
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":657
  *             for j in range(output[idx[i]].size()): self.ptr.register_fold(&output[idx[i]][j])
  *         output.clear()
  *         return True             # <<<<<<<<<<<<<<
  * 
  *     cpdef UseAllHashes(self, list inpt):
  */
   __pyx_r = 1;
   goto __pyx_L0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":635
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":638
  *     cpdef report_t reportable(self): return self.state
  * 
  *     cpdef bool GetHDF5Hashes(self, str path):             # <<<<<<<<<<<<<<
  *         if path.endswith(".hdf5"): pass
  *         else: path += ".hdf5"
  */
 
@@ -38190,45 +38208,45 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_path)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 635, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 638, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "GetHDF5Hashes") < 0)) __PYX_ERR(0, 635, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "GetHDF5Hashes") < 0)) __PYX_ERR(0, 638, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_path = ((PyObject*)values[0]);
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("GetHDF5Hashes", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 635, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("GetHDF5Hashes", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 638, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("AnalysisG._cmodules.cOptimizer.cOptimizer.GetHDF5Hashes", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_path), (&PyUnicode_Type), 1, "path", 1))) __PYX_ERR(0, 635, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_path), (&PyUnicode_Type), 1, "path", 1))) __PYX_ERR(0, 638, __pyx_L1_error)
   __pyx_r = __pyx_pf_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_10GetHDF5Hashes(((struct __pyx_obj_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer *)__pyx_v_self), __pyx_v_path);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -38248,16 +38266,16 @@
   bool __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("GetHDF5Hashes", 1);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_GetHDF5Hashes(__pyx_v_self, __pyx_v_path, 1); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 635, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 635, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_GetHDF5Hashes(__pyx_v_self, __pyx_v_path, 1); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 638, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 638, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -38266,15 +38284,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/cmodules/cyincludes/cyoptimizer.pyx":656
+/* "src/cmodules/cyincludes/cyoptimizer.pyx":659
  *         return True
  * 
  *     cpdef UseAllHashes(self, list inpt):             # <<<<<<<<<<<<<<
  *         cdef int idx
  *         cdef folds_t fold_hash
  */
 
@@ -38310,15 +38328,15 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || __Pyx_PyType_HasFeature(Py_TYPE(((PyObject *)__pyx_v_self)), (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_typedict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_UseAllHashes); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 656, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_UseAllHashes); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 659, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!__Pyx_IsSameCFunction(__pyx_t_1, (void*) __pyx_pw_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_13UseAllHashes)) {
         __Pyx_XDECREF(__pyx_r);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         __pyx_t_5 = 0;
         #if CYTHON_UNPACK_METHODS
@@ -38333,15 +38351,15 @@
           }
         }
         #endif
         {
           PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_v_inpt};
           __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
           __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-          if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 656, __pyx_L1_error)
+          if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 659, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         }
         __pyx_r = __pyx_t_2;
         __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
@@ -38355,25 +38373,25 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":659
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":662
  *         cdef int idx
  *         cdef folds_t fold_hash
  *         cdef vector[string] data = penc(inpt)             # <<<<<<<<<<<<<<
  *         for idx in prange(data.size(), nogil = True, num_threads = self.threads):
  *             fold_hash = folds_t()
  */
-  __pyx_t_6 = __pyx_f_7cytools_penc(__pyx_v_inpt); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 659, __pyx_L1_error)
+  __pyx_t_6 = __pyx_f_7cytools_penc(__pyx_v_inpt); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 662, __pyx_L1_error)
   __pyx_v_data = __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_6);
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":660
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":663
  *         cdef folds_t fold_hash
  *         cdef vector[string] data = penc(inpt)
  *         for idx in prange(data.size(), nogil = True, num_threads = self.threads):             # <<<<<<<<<<<<<<
  *             fold_hash = folds_t()
  *             fold_hash.kfold = 1
  */
   {
@@ -38415,51 +38433,51 @@
                     #pragma omp for lastprivate(__pyx_v_fold_hash) firstprivate(__pyx_v_idx) lastprivate(__pyx_v_idx)
                     #endif /* _OPENMP */
                     for (__pyx_t_8 = 0; __pyx_t_8 < __pyx_t_9; __pyx_t_8++){
                         if (__pyx_parallel_why < 2)
                         {
                             __pyx_v_idx = (int)(0 + 1 * __pyx_t_8);
 
-                            /* "src/cmodules/cyincludes/cyoptimizer.pyx":661
+                            /* "src/cmodules/cyincludes/cyoptimizer.pyx":664
  *         cdef vector[string] data = penc(inpt)
  *         for idx in prange(data.size(), nogil = True, num_threads = self.threads):
  *             fold_hash = folds_t()             # <<<<<<<<<<<<<<
  *             fold_hash.kfold = 1
  *             fold_hash.train = True
  */
                             __pyx_v_fold_hash = __pyx_t_10;
 
-                            /* "src/cmodules/cyincludes/cyoptimizer.pyx":662
+                            /* "src/cmodules/cyincludes/cyoptimizer.pyx":665
  *         for idx in prange(data.size(), nogil = True, num_threads = self.threads):
  *             fold_hash = folds_t()
  *             fold_hash.kfold = 1             # <<<<<<<<<<<<<<
  *             fold_hash.train = True
  *             fold_hash.event_hash = data[idx]
  */
                             __pyx_v_fold_hash.kfold = 1;
 
-                            /* "src/cmodules/cyincludes/cyoptimizer.pyx":663
+                            /* "src/cmodules/cyincludes/cyoptimizer.pyx":666
  *             fold_hash = folds_t()
  *             fold_hash.kfold = 1
  *             fold_hash.train = True             # <<<<<<<<<<<<<<
  *             fold_hash.event_hash = data[idx]
  *             self.ptr.register_fold(&fold_hash)
  */
                             __pyx_v_fold_hash.train = 1;
 
-                            /* "src/cmodules/cyincludes/cyoptimizer.pyx":664
+                            /* "src/cmodules/cyincludes/cyoptimizer.pyx":667
  *             fold_hash.kfold = 1
  *             fold_hash.train = True
  *             fold_hash.event_hash = data[idx]             # <<<<<<<<<<<<<<
  *             self.ptr.register_fold(&fold_hash)
  *         data.clear()
  */
                             __pyx_v_fold_hash.event_hash = (__pyx_v_data[__pyx_v_idx]);
 
-                            /* "src/cmodules/cyincludes/cyoptimizer.pyx":665
+                            /* "src/cmodules/cyincludes/cyoptimizer.pyx":668
  *             fold_hash.train = True
  *             fold_hash.event_hash = data[idx]
  *             self.ptr.register_fold(&fold_hash)             # <<<<<<<<<<<<<<
  *         data.clear()
  * 
  */
                             try {
@@ -38468,15 +38486,15 @@
                               #ifdef WITH_THREAD
                               PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
                               #endif
                               __Pyx_CppExn2PyErr();
                               #ifdef WITH_THREAD
                               __Pyx_PyGILState_Release(__pyx_gilstate_save);
                               #endif
-                              __PYX_ERR(0, 665, __pyx_L8_error)
+                              __PYX_ERR(0, 668, __pyx_L8_error)
                             }
                             goto __pyx_L11;
                             __pyx_L8_error:;
                             {
                                 #ifdef WITH_THREAD
                                 PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
                                 #endif
@@ -38553,15 +38571,15 @@
             #undef likely
             #undef unlikely
             #define likely(x)   __builtin_expect(!!(x), 1)
             #define unlikely(x) __builtin_expect(!!(x), 0)
         #endif
       }
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":660
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":663
  *         cdef folds_t fold_hash
  *         cdef vector[string] data = penc(inpt)
  *         for idx in prange(data.size(), nogil = True, num_threads = self.threads):             # <<<<<<<<<<<<<<
  *             fold_hash = folds_t()
  *             fold_hash.kfold = 1
  */
       /*finally:*/ {
@@ -38579,24 +38597,24 @@
           #endif
           goto __pyx_L1_error;
         }
         __pyx_L5:;
       }
   }
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":666
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":669
  *             fold_hash.event_hash = data[idx]
  *             self.ptr.register_fold(&fold_hash)
  *         data.clear()             # <<<<<<<<<<<<<<
  * 
  *     cpdef FetchTraining(self, int kfold, int batch_size):
  */
   __pyx_v_data.clear();
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":656
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":659
  *         return True
  * 
  *     cpdef UseAllHashes(self, list inpt):             # <<<<<<<<<<<<<<
  *         cdef int idx
  *         cdef folds_t fold_hash
  */
 
@@ -38665,45 +38683,45 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_inpt)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 656, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 659, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "UseAllHashes") < 0)) __PYX_ERR(0, 656, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "UseAllHashes") < 0)) __PYX_ERR(0, 659, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_inpt = ((PyObject*)values[0]);
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("UseAllHashes", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 656, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("UseAllHashes", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 659, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("AnalysisG._cmodules.cOptimizer.cOptimizer.UseAllHashes", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_inpt), (&PyList_Type), 1, "inpt", 1))) __PYX_ERR(0, 656, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_inpt), (&PyList_Type), 1, "inpt", 1))) __PYX_ERR(0, 659, __pyx_L1_error)
   __pyx_r = __pyx_pf_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_12UseAllHashes(((struct __pyx_obj_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer *)__pyx_v_self), __pyx_v_inpt);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -38722,15 +38740,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("UseAllHashes", 1);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_UseAllHashes(__pyx_v_self, __pyx_v_inpt, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 656, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_UseAllHashes(__pyx_v_self, __pyx_v_inpt, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 659, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -38739,15 +38757,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/cmodules/cyincludes/cyoptimizer.pyx":668
+/* "src/cmodules/cyincludes/cyoptimizer.pyx":671
  *         data.clear()
  * 
  *     cpdef FetchTraining(self, int kfold, int batch_size):             # <<<<<<<<<<<<<<
  *         if self.data.sampletracer is not None: pass
  *         else: self.data.sampletracer = self.sampletracer
  */
 
@@ -38779,21 +38797,21 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || __Pyx_PyType_HasFeature(Py_TYPE(((PyObject *)__pyx_v_self)), (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_typedict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_FetchTraining); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 668, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_FetchTraining); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 671, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!__Pyx_IsSameCFunction(__pyx_t_1, (void*) __pyx_pw_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_15FetchTraining)) {
         __Pyx_XDECREF(__pyx_r);
-        __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_kfold); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 668, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_kfold); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 671, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
-        __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_batch_size); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 668, __pyx_L1_error)
+        __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_batch_size); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 671, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_5 = __pyx_t_1; __pyx_t_6 = NULL;
         __pyx_t_7 = 0;
         #if CYTHON_UNPACK_METHODS
         if (unlikely(PyMethod_Check(__pyx_t_5))) {
           __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
@@ -38808,15 +38826,15 @@
         #endif
         {
           PyObject *__pyx_callargs[3] = {__pyx_t_6, __pyx_t_3, __pyx_t_4};
           __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_7, 2+__pyx_t_7);
           __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-          if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 668, __pyx_L1_error)
+          if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 671, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
         }
         __pyx_r = __pyx_t_2;
         __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
@@ -38830,27 +38848,27 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":669
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":672
  * 
  *     cpdef FetchTraining(self, int kfold, int batch_size):
  *         if self.data.sampletracer is not None: pass             # <<<<<<<<<<<<<<
  *         else: self.data.sampletracer = self.sampletracer
  *         self._train = True
  */
   __pyx_t_8 = (__pyx_v_self->data->sampletracer != Py_None);
   if (__pyx_t_8) {
     goto __pyx_L3;
   }
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":670
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":673
  *     cpdef FetchTraining(self, int kfold, int batch_size):
  *         if self.data.sampletracer is not None: pass
  *         else: self.data.sampletracer = self.sampletracer             # <<<<<<<<<<<<<<
  *         self._train = True
  *         self._val = False
  */
   /*else*/ {
@@ -38860,57 +38878,57 @@
     __Pyx_GOTREF(__pyx_v_self->data->sampletracer);
     __Pyx_DECREF(__pyx_v_self->data->sampletracer);
     __pyx_v_self->data->sampletracer = __pyx_t_1;
     __pyx_t_1 = 0;
   }
   __pyx_L3:;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":671
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":674
  *         if self.data.sampletracer is not None: pass
  *         else: self.data.sampletracer = self.sampletracer
  *         self._train = True             # <<<<<<<<<<<<<<
  *         self._val = False
  *         self._test = False
  */
   __pyx_v_self->_train = 1;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":672
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":675
  *         else: self.data.sampletracer = self.sampletracer
  *         self._train = True
  *         self._val = False             # <<<<<<<<<<<<<<
  *         self._test = False
  *         return self.data.set_batch(kfold, batch_size, b"train")
  */
   __pyx_v_self->_val = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":673
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":676
  *         self._train = True
  *         self._val = False
  *         self._test = False             # <<<<<<<<<<<<<<
  *         return self.data.set_batch(kfold, batch_size, b"train")
  * 
  */
   __pyx_v_self->_test = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":674
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":677
  *         self._val = False
  *         self._test = False
  *         return self.data.set_batch(kfold, batch_size, b"train")             # <<<<<<<<<<<<<<
  * 
  *     cpdef FetchValidation(self, int kfold, int batch_size):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_9 = __pyx_convert_string_from_py_6libcpp_6string_std__in_string(__pyx_n_b_train); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 674, __pyx_L1_error)
-  __pyx_t_1 = ((PyObject *)((struct __pyx_vtabstruct_9AnalysisG_9_cmodules_10cOptimizer_DataLoader *)__pyx_v_self->data->__pyx_vtab)->set_batch(__pyx_v_self->data, __pyx_v_kfold, __pyx_v_batch_size, __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_9))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 674, __pyx_L1_error)
+  __pyx_t_9 = __pyx_convert_string_from_py_6libcpp_6string_std__in_string(__pyx_n_b_train); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 677, __pyx_L1_error)
+  __pyx_t_1 = ((PyObject *)((struct __pyx_vtabstruct_9AnalysisG_9_cmodules_10cOptimizer_DataLoader *)__pyx_v_self->data->__pyx_vtab)->set_batch(__pyx_v_self->data, __pyx_v_kfold, __pyx_v_batch_size, __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_9))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 677, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":668
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":671
  *         data.clear()
  * 
  *     cpdef FetchTraining(self, int kfold, int batch_size):             # <<<<<<<<<<<<<<
  *         if self.data.sampletracer is not None: pass
  *         else: self.data.sampletracer = self.sampletracer
  */
 
@@ -38982,43 +39000,43 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_kfold_2)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 668, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 671, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_batch_size)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 668, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 671, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("FetchTraining", 1, 2, 2, 1); __PYX_ERR(0, 668, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("FetchTraining", 1, 2, 2, 1); __PYX_ERR(0, 671, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "FetchTraining") < 0)) __PYX_ERR(0, 668, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "FetchTraining") < 0)) __PYX_ERR(0, 671, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 2)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
-    __pyx_v_kfold = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_kfold == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 668, __pyx_L3_error)
-    __pyx_v_batch_size = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_batch_size == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 668, __pyx_L3_error)
+    __pyx_v_kfold = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_kfold == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 671, __pyx_L3_error)
+    __pyx_v_batch_size = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_batch_size == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 671, __pyx_L3_error)
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("FetchTraining", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 668, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("FetchTraining", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 671, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -39046,15 +39064,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("FetchTraining", 1);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_FetchTraining(__pyx_v_self, __pyx_v_kfold, __pyx_v_batch_size, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 668, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_FetchTraining(__pyx_v_self, __pyx_v_kfold, __pyx_v_batch_size, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 671, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -39063,15 +39081,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/cmodules/cyincludes/cyoptimizer.pyx":676
+/* "src/cmodules/cyincludes/cyoptimizer.pyx":679
  *         return self.data.set_batch(kfold, batch_size, b"train")
  * 
  *     cpdef FetchValidation(self, int kfold, int batch_size):             # <<<<<<<<<<<<<<
  *         if self.data.sampletracer is not None: pass
  *         else: self.data.sampletracer = self.sampletracer
  */
 
@@ -39103,21 +39121,21 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || __Pyx_PyType_HasFeature(Py_TYPE(((PyObject *)__pyx_v_self)), (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_typedict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_FetchValidation); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 676, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_FetchValidation); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 679, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!__Pyx_IsSameCFunction(__pyx_t_1, (void*) __pyx_pw_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_17FetchValidation)) {
         __Pyx_XDECREF(__pyx_r);
-        __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_kfold); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 676, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_kfold); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 679, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
-        __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_batch_size); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 676, __pyx_L1_error)
+        __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_batch_size); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 679, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_5 = __pyx_t_1; __pyx_t_6 = NULL;
         __pyx_t_7 = 0;
         #if CYTHON_UNPACK_METHODS
         if (unlikely(PyMethod_Check(__pyx_t_5))) {
           __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
@@ -39132,15 +39150,15 @@
         #endif
         {
           PyObject *__pyx_callargs[3] = {__pyx_t_6, __pyx_t_3, __pyx_t_4};
           __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_7, 2+__pyx_t_7);
           __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-          if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 676, __pyx_L1_error)
+          if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 679, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
         }
         __pyx_r = __pyx_t_2;
         __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
@@ -39154,27 +39172,27 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":677
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":680
  * 
  *     cpdef FetchValidation(self, int kfold, int batch_size):
  *         if self.data.sampletracer is not None: pass             # <<<<<<<<<<<<<<
  *         else: self.data.sampletracer = self.sampletracer
  *         self._train = False
  */
   __pyx_t_8 = (__pyx_v_self->data->sampletracer != Py_None);
   if (__pyx_t_8) {
     goto __pyx_L3;
   }
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":678
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":681
  *     cpdef FetchValidation(self, int kfold, int batch_size):
  *         if self.data.sampletracer is not None: pass
  *         else: self.data.sampletracer = self.sampletracer             # <<<<<<<<<<<<<<
  *         self._train = False
  *         self._val = True
  */
   /*else*/ {
@@ -39184,57 +39202,57 @@
     __Pyx_GOTREF(__pyx_v_self->data->sampletracer);
     __Pyx_DECREF(__pyx_v_self->data->sampletracer);
     __pyx_v_self->data->sampletracer = __pyx_t_1;
     __pyx_t_1 = 0;
   }
   __pyx_L3:;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":679
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":682
  *         if self.data.sampletracer is not None: pass
  *         else: self.data.sampletracer = self.sampletracer
  *         self._train = False             # <<<<<<<<<<<<<<
  *         self._val = True
  *         self._test = False
  */
   __pyx_v_self->_train = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":680
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":683
  *         else: self.data.sampletracer = self.sampletracer
  *         self._train = False
  *         self._val = True             # <<<<<<<<<<<<<<
  *         self._test = False
  *         return self.data.set_batch(kfold, batch_size, b"valid")
  */
   __pyx_v_self->_val = 1;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":681
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":684
  *         self._train = False
  *         self._val = True
  *         self._test = False             # <<<<<<<<<<<<<<
  *         return self.data.set_batch(kfold, batch_size, b"valid")
  * 
  */
   __pyx_v_self->_test = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":682
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":685
  *         self._val = True
  *         self._test = False
  *         return self.data.set_batch(kfold, batch_size, b"valid")             # <<<<<<<<<<<<<<
  * 
  *     cpdef FetchEvaluation(self, int batch_size):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_9 = __pyx_convert_string_from_py_6libcpp_6string_std__in_string(__pyx_n_b_valid); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 682, __pyx_L1_error)
-  __pyx_t_1 = ((PyObject *)((struct __pyx_vtabstruct_9AnalysisG_9_cmodules_10cOptimizer_DataLoader *)__pyx_v_self->data->__pyx_vtab)->set_batch(__pyx_v_self->data, __pyx_v_kfold, __pyx_v_batch_size, __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_9))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 682, __pyx_L1_error)
+  __pyx_t_9 = __pyx_convert_string_from_py_6libcpp_6string_std__in_string(__pyx_n_b_valid); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 685, __pyx_L1_error)
+  __pyx_t_1 = ((PyObject *)((struct __pyx_vtabstruct_9AnalysisG_9_cmodules_10cOptimizer_DataLoader *)__pyx_v_self->data->__pyx_vtab)->set_batch(__pyx_v_self->data, __pyx_v_kfold, __pyx_v_batch_size, __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_9))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 685, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":676
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":679
  *         return self.data.set_batch(kfold, batch_size, b"train")
  * 
  *     cpdef FetchValidation(self, int kfold, int batch_size):             # <<<<<<<<<<<<<<
  *         if self.data.sampletracer is not None: pass
  *         else: self.data.sampletracer = self.sampletracer
  */
 
@@ -39306,43 +39324,43 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_kfold_2)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 676, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 679, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_batch_size)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 676, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 679, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("FetchValidation", 1, 2, 2, 1); __PYX_ERR(0, 676, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("FetchValidation", 1, 2, 2, 1); __PYX_ERR(0, 679, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "FetchValidation") < 0)) __PYX_ERR(0, 676, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "FetchValidation") < 0)) __PYX_ERR(0, 679, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 2)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
-    __pyx_v_kfold = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_kfold == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 676, __pyx_L3_error)
-    __pyx_v_batch_size = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_batch_size == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 676, __pyx_L3_error)
+    __pyx_v_kfold = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_kfold == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 679, __pyx_L3_error)
+    __pyx_v_batch_size = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_batch_size == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 679, __pyx_L3_error)
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("FetchValidation", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 676, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("FetchValidation", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 679, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -39370,15 +39388,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("FetchValidation", 1);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_FetchValidation(__pyx_v_self, __pyx_v_kfold, __pyx_v_batch_size, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 676, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_FetchValidation(__pyx_v_self, __pyx_v_kfold, __pyx_v_batch_size, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 679, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -39387,15 +39405,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/cmodules/cyincludes/cyoptimizer.pyx":684
+/* "src/cmodules/cyincludes/cyoptimizer.pyx":687
  *         return self.data.set_batch(kfold, batch_size, b"valid")
  * 
  *     cpdef FetchEvaluation(self, int batch_size):             # <<<<<<<<<<<<<<
  *         if self.data.sampletracer is not None: pass
  *         else: self.data.sampletracer = self.sampletracer
  */
 
@@ -39426,19 +39444,19 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || __Pyx_PyType_HasFeature(Py_TYPE(((PyObject *)__pyx_v_self)), (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_typedict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_FetchEvaluation); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 684, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_FetchEvaluation); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 687, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!__Pyx_IsSameCFunction(__pyx_t_1, (void*) __pyx_pw_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_19FetchEvaluation)) {
         __Pyx_XDECREF(__pyx_r);
-        __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_batch_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 684, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_batch_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 687, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_4 = __pyx_t_1; __pyx_t_5 = NULL;
         __pyx_t_6 = 0;
         #if CYTHON_UNPACK_METHODS
         if (unlikely(PyMethod_Check(__pyx_t_4))) {
           __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
@@ -39452,15 +39470,15 @@
         }
         #endif
         {
           PyObject *__pyx_callargs[2] = {__pyx_t_5, __pyx_t_3};
           __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_6, 1+__pyx_t_6);
           __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-          if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 684, __pyx_L1_error)
+          if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 687, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         }
         __pyx_r = __pyx_t_2;
         __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
@@ -39474,27 +39492,27 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":685
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":688
  * 
  *     cpdef FetchEvaluation(self, int batch_size):
  *         if self.data.sampletracer is not None: pass             # <<<<<<<<<<<<<<
  *         else: self.data.sampletracer = self.sampletracer
  *         self._train = False
  */
   __pyx_t_7 = (__pyx_v_self->data->sampletracer != Py_None);
   if (__pyx_t_7) {
     goto __pyx_L3;
   }
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":686
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":689
  *     cpdef FetchEvaluation(self, int batch_size):
  *         if self.data.sampletracer is not None: pass
  *         else: self.data.sampletracer = self.sampletracer             # <<<<<<<<<<<<<<
  *         self._train = False
  *         self._val = False
  */
   /*else*/ {
@@ -39504,57 +39522,57 @@
     __Pyx_GOTREF(__pyx_v_self->data->sampletracer);
     __Pyx_DECREF(__pyx_v_self->data->sampletracer);
     __pyx_v_self->data->sampletracer = __pyx_t_1;
     __pyx_t_1 = 0;
   }
   __pyx_L3:;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":687
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":690
  *         if self.data.sampletracer is not None: pass
  *         else: self.data.sampletracer = self.sampletracer
  *         self._train = False             # <<<<<<<<<<<<<<
  *         self._val = False
  *         self._test = True
  */
   __pyx_v_self->_train = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":688
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":691
  *         else: self.data.sampletracer = self.sampletracer
  *         self._train = False
  *         self._val = False             # <<<<<<<<<<<<<<
  *         self._test = True
  *         return self.data.set_batch(-1, batch_size, b"eval")
  */
   __pyx_v_self->_val = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":689
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":692
  *         self._train = False
  *         self._val = False
  *         self._test = True             # <<<<<<<<<<<<<<
  *         return self.data.set_batch(-1, batch_size, b"eval")
  * 
  */
   __pyx_v_self->_test = 1;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":690
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":693
  *         self._val = False
  *         self._test = True
  *         return self.data.set_batch(-1, batch_size, b"eval")             # <<<<<<<<<<<<<<
  * 
  *     cpdef UseTheseFolds(self, list inpt): self.ptr.use_folds = <vector[int]>inpt
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_8 = __pyx_convert_string_from_py_6libcpp_6string_std__in_string(__pyx_n_b_eval); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 690, __pyx_L1_error)
-  __pyx_t_1 = ((PyObject *)((struct __pyx_vtabstruct_9AnalysisG_9_cmodules_10cOptimizer_DataLoader *)__pyx_v_self->data->__pyx_vtab)->set_batch(__pyx_v_self->data, -1, __pyx_v_batch_size, __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_8))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 690, __pyx_L1_error)
+  __pyx_t_8 = __pyx_convert_string_from_py_6libcpp_6string_std__in_string(__pyx_n_b_eval); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 693, __pyx_L1_error)
+  __pyx_t_1 = ((PyObject *)((struct __pyx_vtabstruct_9AnalysisG_9_cmodules_10cOptimizer_DataLoader *)__pyx_v_self->data->__pyx_vtab)->set_batch(__pyx_v_self->data, -1, __pyx_v_batch_size, __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_8))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 693, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":684
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":687
  *         return self.data.set_batch(kfold, batch_size, b"valid")
  * 
  *     cpdef FetchEvaluation(self, int batch_size):             # <<<<<<<<<<<<<<
  *         if self.data.sampletracer is not None: pass
  *         else: self.data.sampletracer = self.sampletracer
  */
 
@@ -39622,31 +39640,31 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_batch_size)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 684, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 687, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "FetchEvaluation") < 0)) __PYX_ERR(0, 684, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "FetchEvaluation") < 0)) __PYX_ERR(0, 687, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
-    __pyx_v_batch_size = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_batch_size == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 684, __pyx_L3_error)
+    __pyx_v_batch_size = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_batch_size == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 687, __pyx_L3_error)
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("FetchEvaluation", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 684, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("FetchEvaluation", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 687, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -39674,15 +39692,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("FetchEvaluation", 1);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_FetchEvaluation(__pyx_v_self, __pyx_v_batch_size, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 684, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_FetchEvaluation(__pyx_v_self, __pyx_v_batch_size, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 687, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -39691,15 +39709,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/cmodules/cyincludes/cyoptimizer.pyx":692
+/* "src/cmodules/cyincludes/cyoptimizer.pyx":695
  *         return self.data.set_batch(-1, batch_size, b"eval")
  * 
  *     cpdef UseTheseFolds(self, list inpt): self.ptr.use_folds = <vector[int]>inpt             # <<<<<<<<<<<<<<
  * 
  *     cpdef AddkFold(self, int epoch, int kfold, dict inpt, dict out_map):
  */
 
@@ -39728,15 +39746,15 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || __Pyx_PyType_HasFeature(Py_TYPE(((PyObject *)__pyx_v_self)), (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_typedict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_UseTheseFolds); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 692, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_UseTheseFolds); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 695, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!__Pyx_IsSameCFunction(__pyx_t_1, (void*) __pyx_pw_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_21UseTheseFolds)) {
         __Pyx_XDECREF(__pyx_r);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         __pyx_t_5 = 0;
         #if CYTHON_UNPACK_METHODS
@@ -39751,15 +39769,15 @@
           }
         }
         #endif
         {
           PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_v_inpt};
           __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
           __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-          if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 692, __pyx_L1_error)
+          if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 695, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         }
         __pyx_r = __pyx_t_2;
         __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
@@ -39772,15 +39790,15 @@
       }
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
-  __pyx_t_6 = __pyx_convert_vector_from_py_int(__pyx_v_inpt); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 692, __pyx_L1_error)
+  __pyx_t_6 = __pyx_convert_vector_from_py_int(__pyx_v_inpt); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 695, __pyx_L1_error)
   __pyx_v_self->ptr->use_folds = ((std::vector<int> )__pyx_t_6);
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
@@ -39844,45 +39862,45 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_inpt)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 692, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 695, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "UseTheseFolds") < 0)) __PYX_ERR(0, 692, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "UseTheseFolds") < 0)) __PYX_ERR(0, 695, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_inpt = ((PyObject*)values[0]);
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("UseTheseFolds", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 692, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("UseTheseFolds", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 695, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("AnalysisG._cmodules.cOptimizer.cOptimizer.UseTheseFolds", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_inpt), (&PyList_Type), 1, "inpt", 1))) __PYX_ERR(0, 692, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_inpt), (&PyList_Type), 1, "inpt", 1))) __PYX_ERR(0, 695, __pyx_L1_error)
   __pyx_r = __pyx_pf_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_20UseTheseFolds(((struct __pyx_obj_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer *)__pyx_v_self), __pyx_v_inpt);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -39901,15 +39919,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("UseTheseFolds", 1);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_UseTheseFolds(__pyx_v_self, __pyx_v_inpt, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 692, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_UseTheseFolds(__pyx_v_self, __pyx_v_inpt, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 695, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -39918,15 +39936,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/cmodules/cyincludes/cyoptimizer.pyx":694
+/* "src/cmodules/cyincludes/cyoptimizer.pyx":697
  *     cpdef UseTheseFolds(self, list inpt): self.ptr.use_folds = <vector[int]>inpt
  * 
  *     cpdef AddkFold(self, int epoch, int kfold, dict inpt, dict out_map):             # <<<<<<<<<<<<<<
  *         cdef map[string, data_t] map_data = recast(inpt, out_map)
  *         if  self._train: self.ptr.train_epoch_kfold(epoch, kfold, &map_data)
  */
 
@@ -39959,21 +39977,21 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || __Pyx_PyType_HasFeature(Py_TYPE(((PyObject *)__pyx_v_self)), (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_typedict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_AddkFold); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 694, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_AddkFold); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 697, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!__Pyx_IsSameCFunction(__pyx_t_1, (void*) __pyx_pw_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_23AddkFold)) {
         __Pyx_XDECREF(__pyx_r);
-        __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_epoch); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 694, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_epoch); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 697, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
-        __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_kfold); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 694, __pyx_L1_error)
+        __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_kfold); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 697, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_5 = __pyx_t_1; __pyx_t_6 = NULL;
         __pyx_t_7 = 0;
         #if CYTHON_UNPACK_METHODS
         if (unlikely(PyMethod_Check(__pyx_t_5))) {
           __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
@@ -39988,15 +40006,15 @@
         #endif
         {
           PyObject *__pyx_callargs[5] = {__pyx_t_6, __pyx_t_3, __pyx_t_4, __pyx_v_inpt, __pyx_v_out_map};
           __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_7, 4+__pyx_t_7);
           __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-          if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 694, __pyx_L1_error)
+          if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 697, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
         }
         __pyx_r = __pyx_t_2;
         __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
@@ -40010,91 +40028,91 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":695
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":698
  * 
  *     cpdef AddkFold(self, int epoch, int kfold, dict inpt, dict out_map):
  *         cdef map[string, data_t] map_data = recast(inpt, out_map)             # <<<<<<<<<<<<<<
  *         if  self._train: self.ptr.train_epoch_kfold(epoch, kfold, &map_data)
  *         elif  self._val: self.ptr.validation_epoch_kfold(epoch, kfold, &map_data)
  */
-  __pyx_t_1 = __pyx_f_7cytools_recast(__pyx_v_inpt, __pyx_v_out_map, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 695, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_7cytools_recast(__pyx_v_inpt, __pyx_v_out_map, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 698, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_8 = __pyx_convert_map_from_py_std_3a__3a_string__and_struct__data_t(__pyx_t_1); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 695, __pyx_L1_error)
+  __pyx_t_8 = __pyx_convert_map_from_py_std_3a__3a_string__and_struct__data_t(__pyx_t_1); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 698, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_map_data = __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_8);
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":696
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":699
  *     cpdef AddkFold(self, int epoch, int kfold, dict inpt, dict out_map):
  *         cdef map[string, data_t] map_data = recast(inpt, out_map)
  *         if  self._train: self.ptr.train_epoch_kfold(epoch, kfold, &map_data)             # <<<<<<<<<<<<<<
  *         elif  self._val: self.ptr.validation_epoch_kfold(epoch, kfold, &map_data)
  *         elif self._test: self.ptr.evaluation_epoch_kfold(epoch, kfold, &map_data)
  */
   __pyx_t_9 = (__pyx_v_self->_train != 0);
   if (__pyx_t_9) {
     try {
       __pyx_v_self->ptr->train_epoch_kfold(__pyx_v_epoch, __pyx_v_kfold, (&__pyx_v_map_data));
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 696, __pyx_L1_error)
+      __PYX_ERR(0, 699, __pyx_L1_error)
     }
     goto __pyx_L3;
   }
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":697
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":700
  *         cdef map[string, data_t] map_data = recast(inpt, out_map)
  *         if  self._train: self.ptr.train_epoch_kfold(epoch, kfold, &map_data)
  *         elif  self._val: self.ptr.validation_epoch_kfold(epoch, kfold, &map_data)             # <<<<<<<<<<<<<<
  *         elif self._test: self.ptr.evaluation_epoch_kfold(epoch, kfold, &map_data)
  *         map_data.clear()
  */
   __pyx_t_9 = (__pyx_v_self->_val != 0);
   if (__pyx_t_9) {
     try {
       __pyx_v_self->ptr->validation_epoch_kfold(__pyx_v_epoch, __pyx_v_kfold, (&__pyx_v_map_data));
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 697, __pyx_L1_error)
+      __PYX_ERR(0, 700, __pyx_L1_error)
     }
     goto __pyx_L3;
   }
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":698
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":701
  *         if  self._train: self.ptr.train_epoch_kfold(epoch, kfold, &map_data)
  *         elif  self._val: self.ptr.validation_epoch_kfold(epoch, kfold, &map_data)
  *         elif self._test: self.ptr.evaluation_epoch_kfold(epoch, kfold, &map_data)             # <<<<<<<<<<<<<<
  *         map_data.clear()
  * 
  */
   __pyx_t_9 = (__pyx_v_self->_test != 0);
   if (__pyx_t_9) {
     try {
       __pyx_v_self->ptr->evaluation_epoch_kfold(__pyx_v_epoch, __pyx_v_kfold, (&__pyx_v_map_data));
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 698, __pyx_L1_error)
+      __PYX_ERR(0, 701, __pyx_L1_error)
     }
   }
   __pyx_L3:;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":699
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":702
  *         elif  self._val: self.ptr.validation_epoch_kfold(epoch, kfold, &map_data)
  *         elif self._test: self.ptr.evaluation_epoch_kfold(epoch, kfold, &map_data)
  *         map_data.clear()             # <<<<<<<<<<<<<<
  * 
  *     cpdef FastGraphRecast(self, int epoch, int kfold, list inpt, dict out_map):
  */
   __pyx_v_map_data.clear();
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":694
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":697
  *     cpdef UseTheseFolds(self, list inpt): self.ptr.use_folds = <vector[int]>inpt
  * 
  *     cpdef AddkFold(self, int epoch, int kfold, dict inpt, dict out_map):             # <<<<<<<<<<<<<<
  *         cdef map[string, data_t] map_data = recast(inpt, out_map)
  *         if  self._train: self.ptr.train_epoch_kfold(epoch, kfold, &map_data)
  */
 
@@ -40174,82 +40192,82 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_epoch_2)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 694, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 697, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_kfold_2)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 694, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 697, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("AddkFold", 1, 4, 4, 1); __PYX_ERR(0, 694, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("AddkFold", 1, 4, 4, 1); __PYX_ERR(0, 697, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_inpt)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[2]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 694, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 697, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("AddkFold", 1, 4, 4, 2); __PYX_ERR(0, 694, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("AddkFold", 1, 4, 4, 2); __PYX_ERR(0, 697, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_out_map)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[3]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 694, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 697, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("AddkFold", 1, 4, 4, 3); __PYX_ERR(0, 694, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("AddkFold", 1, 4, 4, 3); __PYX_ERR(0, 697, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "AddkFold") < 0)) __PYX_ERR(0, 694, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "AddkFold") < 0)) __PYX_ERR(0, 697, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 4)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
       values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
       values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
     }
-    __pyx_v_epoch = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_epoch == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 694, __pyx_L3_error)
-    __pyx_v_kfold = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_kfold == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 694, __pyx_L3_error)
+    __pyx_v_epoch = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_epoch == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 697, __pyx_L3_error)
+    __pyx_v_kfold = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_kfold == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 697, __pyx_L3_error)
     __pyx_v_inpt = ((PyObject*)values[2]);
     __pyx_v_out_map = ((PyObject*)values[3]);
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("AddkFold", 1, 4, 4, __pyx_nargs); __PYX_ERR(0, 694, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("AddkFold", 1, 4, 4, __pyx_nargs); __PYX_ERR(0, 697, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("AnalysisG._cmodules.cOptimizer.cOptimizer.AddkFold", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_inpt), (&PyDict_Type), 1, "inpt", 1))) __PYX_ERR(0, 694, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_out_map), (&PyDict_Type), 1, "out_map", 1))) __PYX_ERR(0, 694, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_inpt), (&PyDict_Type), 1, "inpt", 1))) __PYX_ERR(0, 697, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_out_map), (&PyDict_Type), 1, "out_map", 1))) __PYX_ERR(0, 697, __pyx_L1_error)
   __pyx_r = __pyx_pf_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_22AddkFold(((struct __pyx_obj_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer *)__pyx_v_self), __pyx_v_epoch, __pyx_v_kfold, __pyx_v_inpt, __pyx_v_out_map);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -40268,15 +40286,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("AddkFold", 1);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_AddkFold(__pyx_v_self, __pyx_v_epoch, __pyx_v_kfold, __pyx_v_inpt, __pyx_v_out_map, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 694, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_AddkFold(__pyx_v_self, __pyx_v_epoch, __pyx_v_kfold, __pyx_v_inpt, __pyx_v_out_map, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 697, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -40285,15 +40303,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/cmodules/cyincludes/cyoptimizer.pyx":701
+/* "src/cmodules/cyincludes/cyoptimizer.pyx":704
  *         map_data.clear()
  * 
  *     cpdef FastGraphRecast(self, int epoch, int kfold, list inpt, dict out_map):             # <<<<<<<<<<<<<<
  *         cdef str key
  *         cdef int i, l
  */
 
@@ -40344,21 +40362,21 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || __Pyx_PyType_HasFeature(Py_TYPE(((PyObject *)__pyx_v_self)), (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_typedict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_FastGraphRecast); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 701, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_FastGraphRecast); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 704, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!__Pyx_IsSameCFunction(__pyx_t_1, (void*) __pyx_pw_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_25FastGraphRecast)) {
         __Pyx_XDECREF(__pyx_r);
-        __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_epoch); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 701, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_epoch); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 704, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
-        __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_kfold); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 701, __pyx_L1_error)
+        __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_kfold); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 704, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_5 = __pyx_t_1; __pyx_t_6 = NULL;
         __pyx_t_7 = 0;
         #if CYTHON_UNPACK_METHODS
         if (unlikely(PyMethod_Check(__pyx_t_5))) {
           __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
@@ -40373,15 +40391,15 @@
         #endif
         {
           PyObject *__pyx_callargs[5] = {__pyx_t_6, __pyx_t_3, __pyx_t_4, __pyx_v_inpt, __pyx_v_out_map};
           __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_7, 4+__pyx_t_7);
           __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-          if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 701, __pyx_L1_error)
+          if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 704, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
         }
         __pyx_r = __pyx_t_2;
         __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
@@ -40395,29 +40413,29 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":706
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":709
  *         cdef list graphs
  *         cdef map[string, data_t] map_data
  *         for i in trange(len(inpt)):             # <<<<<<<<<<<<<<
  *             graphs = inpt[i].pop("graphs")
  *             graphs = [Batch().from_data_list(graphs)]
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_trange); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 706, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_trange); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 709, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (unlikely(__pyx_v_inpt == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-    __PYX_ERR(0, 706, __pyx_L1_error)
+    __PYX_ERR(0, 709, __pyx_L1_error)
   }
-  __pyx_t_8 = __Pyx_PyList_GET_SIZE(__pyx_v_inpt); if (unlikely(__pyx_t_8 == ((Py_ssize_t)-1))) __PYX_ERR(0, 706, __pyx_L1_error)
-  __pyx_t_5 = PyInt_FromSsize_t(__pyx_t_8); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 706, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyList_GET_SIZE(__pyx_v_inpt); if (unlikely(__pyx_t_8 == ((Py_ssize_t)-1))) __PYX_ERR(0, 709, __pyx_L1_error)
+  __pyx_t_5 = PyInt_FromSsize_t(__pyx_t_8); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 709, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_4 = NULL;
   __pyx_t_7 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_4)) {
@@ -40430,89 +40448,89 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_t_5};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_7, 1+__pyx_t_7);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 706, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 709, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   if (likely(PyList_CheckExact(__pyx_t_1)) || PyTuple_CheckExact(__pyx_t_1)) {
     __pyx_t_2 = __pyx_t_1; __Pyx_INCREF(__pyx_t_2);
     __pyx_t_8 = 0;
     __pyx_t_9 = NULL;
   } else {
-    __pyx_t_8 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 706, __pyx_L1_error)
+    __pyx_t_8 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 709, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_9 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_2); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 706, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_2); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 709, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   for (;;) {
     if (likely(!__pyx_t_9)) {
       if (likely(PyList_CheckExact(__pyx_t_2))) {
         {
           Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_2);
           #if !CYTHON_ASSUME_SAFE_MACROS
-          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 706, __pyx_L1_error)
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 709, __pyx_L1_error)
           #endif
           if (__pyx_t_8 >= __pyx_temp) break;
         }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_1 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_8); __Pyx_INCREF(__pyx_t_1); __pyx_t_8++; if (unlikely((0 < 0))) __PYX_ERR(0, 706, __pyx_L1_error)
+        __pyx_t_1 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_8); __Pyx_INCREF(__pyx_t_1); __pyx_t_8++; if (unlikely((0 < 0))) __PYX_ERR(0, 709, __pyx_L1_error)
         #else
-        __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_8); __pyx_t_8++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 706, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_8); __pyx_t_8++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 709, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         #endif
       } else {
         {
           Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_2);
           #if !CYTHON_ASSUME_SAFE_MACROS
-          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 706, __pyx_L1_error)
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 709, __pyx_L1_error)
           #endif
           if (__pyx_t_8 >= __pyx_temp) break;
         }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_8); __Pyx_INCREF(__pyx_t_1); __pyx_t_8++; if (unlikely((0 < 0))) __PYX_ERR(0, 706, __pyx_L1_error)
+        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_8); __Pyx_INCREF(__pyx_t_1); __pyx_t_8++; if (unlikely((0 < 0))) __PYX_ERR(0, 709, __pyx_L1_error)
         #else
-        __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_8); __pyx_t_8++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 706, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_8); __pyx_t_8++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 709, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         #endif
       }
     } else {
       __pyx_t_1 = __pyx_t_9(__pyx_t_2);
       if (unlikely(!__pyx_t_1)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 706, __pyx_L1_error)
+          else __PYX_ERR(0, 709, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_1);
     }
-    __pyx_t_7 = __Pyx_PyInt_As_int(__pyx_t_1); if (unlikely((__pyx_t_7 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 706, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyInt_As_int(__pyx_t_1); if (unlikely((__pyx_t_7 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 709, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_v_i = __pyx_t_7;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":707
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":710
  *         cdef map[string, data_t] map_data
  *         for i in trange(len(inpt)):
  *             graphs = inpt[i].pop("graphs")             # <<<<<<<<<<<<<<
  *             graphs = [Batch().from_data_list(graphs)]
  *             graphs = [{k : j.numpy(force = True) for k, j in k.to_dict().items()} for k in graphs[0].to_data_list()]
  */
     if (unlikely(__pyx_v_inpt == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 707, __pyx_L1_error)
+      __PYX_ERR(0, 710, __pyx_L1_error)
     }
-    __pyx_t_5 = __Pyx_GetItemInt_List(__pyx_v_inpt, __pyx_v_i, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 707, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_GetItemInt_List(__pyx_v_inpt, __pyx_v_i, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 710, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_pop); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 707, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_pop); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 710, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_t_5 = NULL;
     __pyx_t_7 = 0;
     #if CYTHON_UNPACK_METHODS
     if (likely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
@@ -40525,30 +40543,30 @@
       }
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_5, __pyx_n_u_graphs};
       __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_7, 1+__pyx_t_7);
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 707, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 710, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     }
-    if (!(likely(PyList_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None) || __Pyx_RaiseUnexpectedTypeError("list", __pyx_t_1))) __PYX_ERR(0, 707, __pyx_L1_error)
+    if (!(likely(PyList_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None) || __Pyx_RaiseUnexpectedTypeError("list", __pyx_t_1))) __PYX_ERR(0, 710, __pyx_L1_error)
     __Pyx_XDECREF_SET(__pyx_v_graphs, ((PyObject*)__pyx_t_1));
     __pyx_t_1 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":708
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":711
  *         for i in trange(len(inpt)):
  *             graphs = inpt[i].pop("graphs")
  *             graphs = [Batch().from_data_list(graphs)]             # <<<<<<<<<<<<<<
  *             graphs = [{k : j.numpy(force = True) for k, j in k.to_dict().items()} for k in graphs[0].to_data_list()]
  *             for k in inpt[i]:
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_Batch); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 708, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_Batch); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 711, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_3 = NULL;
     __pyx_t_7 = 0;
     #if CYTHON_UNPACK_METHODS
     if (unlikely(PyMethod_Check(__pyx_t_5))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_5);
       if (likely(__pyx_t_3)) {
@@ -40560,19 +40578,19 @@
       }
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_3, NULL};
       __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_7, 0+__pyx_t_7);
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 708, __pyx_L1_error)
+      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 711, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     }
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_from_data_list); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 708, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_from_data_list); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 711, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_4 = NULL;
     __pyx_t_7 = 0;
     #if CYTHON_UNPACK_METHODS
     if (likely(PyMethod_Check(__pyx_t_5))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_5);
@@ -40585,39 +40603,39 @@
       }
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_v_graphs};
       __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_7, 1+__pyx_t_7);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 708, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 711, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     }
-    __pyx_t_5 = PyList_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 708, __pyx_L1_error)
+    __pyx_t_5 = PyList_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 711, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_GIVEREF(__pyx_t_1);
-    if (__Pyx_PyList_SET_ITEM(__pyx_t_5, 0, __pyx_t_1)) __PYX_ERR(0, 708, __pyx_L1_error);
+    if (__Pyx_PyList_SET_ITEM(__pyx_t_5, 0, __pyx_t_1)) __PYX_ERR(0, 711, __pyx_L1_error);
     __pyx_t_1 = 0;
     __Pyx_DECREF_SET(__pyx_v_graphs, ((PyObject*)__pyx_t_5));
     __pyx_t_5 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":709
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":712
  *             graphs = inpt[i].pop("graphs")
  *             graphs = [Batch().from_data_list(graphs)]
  *             graphs = [{k : j.numpy(force = True) for k, j in k.to_dict().items()} for k in graphs[0].to_data_list()]             # <<<<<<<<<<<<<<
  *             for k in inpt[i]:
  *                 if not isinstance(inpt[i][k], dict): inpt[i][k] = inpt[i][k].numpy(force = True)
  */
     { /* enter inner scope */
-      __pyx_t_5 = PyList_New(0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 709, __pyx_L7_error)
+      __pyx_t_5 = PyList_New(0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 712, __pyx_L7_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_4 = __Pyx_GetItemInt_List(__pyx_v_graphs, 0, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 709, __pyx_L7_error)
+      __pyx_t_4 = __Pyx_GetItemInt_List(__pyx_v_graphs, 0, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 712, __pyx_L7_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_to_data_list); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 709, __pyx_L7_error)
+      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_to_data_list); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 712, __pyx_L7_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_t_4 = NULL;
       __pyx_t_7 = 0;
       #if CYTHON_UNPACK_METHODS
       if (likely(PyMethod_Check(__pyx_t_3))) {
         __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
@@ -40630,78 +40648,78 @@
         }
       }
       #endif
       {
         PyObject *__pyx_callargs[2] = {__pyx_t_4, NULL};
         __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_7, 0+__pyx_t_7);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 709, __pyx_L7_error)
+        if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 712, __pyx_L7_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       }
       if (likely(PyList_CheckExact(__pyx_t_1)) || PyTuple_CheckExact(__pyx_t_1)) {
         __pyx_t_3 = __pyx_t_1; __Pyx_INCREF(__pyx_t_3);
         __pyx_t_10 = 0;
         __pyx_t_11 = NULL;
       } else {
-        __pyx_t_10 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 709, __pyx_L7_error)
+        __pyx_t_10 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 712, __pyx_L7_error)
         __Pyx_GOTREF(__pyx_t_3);
-        __pyx_t_11 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_3); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 709, __pyx_L7_error)
+        __pyx_t_11 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_3); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 712, __pyx_L7_error)
       }
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       for (;;) {
         if (likely(!__pyx_t_11)) {
           if (likely(PyList_CheckExact(__pyx_t_3))) {
             {
               Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_3);
               #if !CYTHON_ASSUME_SAFE_MACROS
-              if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 709, __pyx_L7_error)
+              if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 712, __pyx_L7_error)
               #endif
               if (__pyx_t_10 >= __pyx_temp) break;
             }
             #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-            __pyx_t_1 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_10); __Pyx_INCREF(__pyx_t_1); __pyx_t_10++; if (unlikely((0 < 0))) __PYX_ERR(0, 709, __pyx_L7_error)
+            __pyx_t_1 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_10); __Pyx_INCREF(__pyx_t_1); __pyx_t_10++; if (unlikely((0 < 0))) __PYX_ERR(0, 712, __pyx_L7_error)
             #else
-            __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_3, __pyx_t_10); __pyx_t_10++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 709, __pyx_L7_error)
+            __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_3, __pyx_t_10); __pyx_t_10++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 712, __pyx_L7_error)
             __Pyx_GOTREF(__pyx_t_1);
             #endif
           } else {
             {
               Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_3);
               #if !CYTHON_ASSUME_SAFE_MACROS
-              if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 709, __pyx_L7_error)
+              if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 712, __pyx_L7_error)
               #endif
               if (__pyx_t_10 >= __pyx_temp) break;
             }
             #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-            __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_10); __Pyx_INCREF(__pyx_t_1); __pyx_t_10++; if (unlikely((0 < 0))) __PYX_ERR(0, 709, __pyx_L7_error)
+            __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_10); __Pyx_INCREF(__pyx_t_1); __pyx_t_10++; if (unlikely((0 < 0))) __PYX_ERR(0, 712, __pyx_L7_error)
             #else
-            __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_3, __pyx_t_10); __pyx_t_10++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 709, __pyx_L7_error)
+            __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_3, __pyx_t_10); __pyx_t_10++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 712, __pyx_L7_error)
             __Pyx_GOTREF(__pyx_t_1);
             #endif
           }
         } else {
           __pyx_t_1 = __pyx_t_11(__pyx_t_3);
           if (unlikely(!__pyx_t_1)) {
             PyObject* exc_type = PyErr_Occurred();
             if (exc_type) {
               if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-              else __PYX_ERR(0, 709, __pyx_L7_error)
+              else __PYX_ERR(0, 712, __pyx_L7_error)
             }
             break;
           }
           __Pyx_GOTREF(__pyx_t_1);
         }
         __Pyx_XDECREF_SET(__pyx_8genexpr8__pyx_v_k, __pyx_t_1);
         __pyx_t_1 = 0;
         { /* enter inner scope */
-          __pyx_t_1 = PyDict_New(); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 709, __pyx_L12_error)
+          __pyx_t_1 = PyDict_New(); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 712, __pyx_L12_error)
           __Pyx_GOTREF(__pyx_t_1);
           __pyx_t_12 = 0;
-          __pyx_t_14 = __Pyx_PyObject_GetAttrStr(__pyx_8genexpr8__pyx_v_k, __pyx_n_s_to_dict); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 709, __pyx_L12_error)
+          __pyx_t_14 = __Pyx_PyObject_GetAttrStr(__pyx_8genexpr8__pyx_v_k, __pyx_n_s_to_dict); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 712, __pyx_L12_error)
           __Pyx_GOTREF(__pyx_t_14);
           __pyx_t_15 = NULL;
           __pyx_t_16 = 0;
           #if CYTHON_UNPACK_METHODS
           if (likely(PyMethod_Check(__pyx_t_14))) {
             __pyx_t_15 = PyMethod_GET_SELF(__pyx_t_14);
             if (likely(__pyx_t_15)) {
@@ -40713,433 +40731,433 @@
             }
           }
           #endif
           {
             PyObject *__pyx_callargs[2] = {__pyx_t_15, NULL};
             __pyx_t_6 = __Pyx_PyObject_FastCall(__pyx_t_14, __pyx_callargs+1-__pyx_t_16, 0+__pyx_t_16);
             __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
-            if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 709, __pyx_L12_error)
+            if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 712, __pyx_L12_error)
             __Pyx_GOTREF(__pyx_t_6);
             __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
           }
           if (unlikely(__pyx_t_6 == Py_None)) {
             PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "items");
-            __PYX_ERR(0, 709, __pyx_L12_error)
+            __PYX_ERR(0, 712, __pyx_L12_error)
           }
-          __pyx_t_14 = __Pyx_dict_iterator(__pyx_t_6, 0, __pyx_n_s_items, (&__pyx_t_13), (&__pyx_t_7)); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 709, __pyx_L12_error)
+          __pyx_t_14 = __Pyx_dict_iterator(__pyx_t_6, 0, __pyx_n_s_items, (&__pyx_t_13), (&__pyx_t_7)); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 712, __pyx_L12_error)
           __Pyx_GOTREF(__pyx_t_14);
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
           __Pyx_XDECREF(__pyx_t_4);
           __pyx_t_4 = __pyx_t_14;
           __pyx_t_14 = 0;
           while (1) {
             __pyx_t_16 = __Pyx_dict_iter_next(__pyx_t_4, __pyx_t_13, &__pyx_t_12, &__pyx_t_14, &__pyx_t_6, NULL, __pyx_t_7);
             if (unlikely(__pyx_t_16 == 0)) break;
-            if (unlikely(__pyx_t_16 == -1)) __PYX_ERR(0, 709, __pyx_L12_error)
+            if (unlikely(__pyx_t_16 == -1)) __PYX_ERR(0, 712, __pyx_L12_error)
             __Pyx_GOTREF(__pyx_t_14);
             __Pyx_GOTREF(__pyx_t_6);
             __Pyx_XDECREF_SET(__pyx_8genexpr9__pyx_v_k, __pyx_t_14);
             __pyx_t_14 = 0;
             __Pyx_XDECREF_SET(__pyx_8genexpr9__pyx_v_j, __pyx_t_6);
             __pyx_t_6 = 0;
-            __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_8genexpr9__pyx_v_j, __pyx_n_s_numpy); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 709, __pyx_L12_error)
+            __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_8genexpr9__pyx_v_j, __pyx_n_s_numpy); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 712, __pyx_L12_error)
             __Pyx_GOTREF(__pyx_t_6);
-            __pyx_t_14 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 709, __pyx_L12_error)
+            __pyx_t_14 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 712, __pyx_L12_error)
             __Pyx_GOTREF(__pyx_t_14);
-            if (PyDict_SetItem(__pyx_t_14, __pyx_n_s_force, Py_True) < 0) __PYX_ERR(0, 709, __pyx_L12_error)
-            __pyx_t_15 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_empty_tuple, __pyx_t_14); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 709, __pyx_L12_error)
+            if (PyDict_SetItem(__pyx_t_14, __pyx_n_s_force, Py_True) < 0) __PYX_ERR(0, 712, __pyx_L12_error)
+            __pyx_t_15 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_empty_tuple, __pyx_t_14); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 712, __pyx_L12_error)
             __Pyx_GOTREF(__pyx_t_15);
             __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
             __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
-            if (unlikely(PyDict_SetItem(__pyx_t_1, (PyObject*)__pyx_8genexpr9__pyx_v_k, (PyObject*)__pyx_t_15))) __PYX_ERR(0, 709, __pyx_L12_error)
+            if (unlikely(PyDict_SetItem(__pyx_t_1, (PyObject*)__pyx_8genexpr9__pyx_v_k, (PyObject*)__pyx_t_15))) __PYX_ERR(0, 712, __pyx_L12_error)
             __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
           }
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
           __Pyx_XDECREF(__pyx_8genexpr9__pyx_v_j); __pyx_8genexpr9__pyx_v_j = 0;
           __Pyx_XDECREF(__pyx_8genexpr9__pyx_v_k); __pyx_8genexpr9__pyx_v_k = 0;
           goto __pyx_L15_exit_scope;
           __pyx_L12_error:;
           __Pyx_XDECREF(__pyx_8genexpr9__pyx_v_j); __pyx_8genexpr9__pyx_v_j = 0;
           __Pyx_XDECREF(__pyx_8genexpr9__pyx_v_k); __pyx_8genexpr9__pyx_v_k = 0;
           goto __pyx_L7_error;
           __pyx_L15_exit_scope:;
         } /* exit inner scope */
-        if (unlikely(__Pyx_ListComp_Append(__pyx_t_5, (PyObject*)__pyx_t_1))) __PYX_ERR(0, 709, __pyx_L7_error)
+        if (unlikely(__Pyx_ListComp_Append(__pyx_t_5, (PyObject*)__pyx_t_1))) __PYX_ERR(0, 712, __pyx_L7_error)
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       }
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_XDECREF(__pyx_8genexpr8__pyx_v_k); __pyx_8genexpr8__pyx_v_k = 0;
       goto __pyx_L17_exit_scope;
       __pyx_L7_error:;
       __Pyx_XDECREF(__pyx_8genexpr8__pyx_v_k); __pyx_8genexpr8__pyx_v_k = 0;
       goto __pyx_L1_error;
       __pyx_L17_exit_scope:;
     } /* exit inner scope */
     __Pyx_DECREF_SET(__pyx_v_graphs, ((PyObject*)__pyx_t_5));
     __pyx_t_5 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":710
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":713
  *             graphs = [Batch().from_data_list(graphs)]
  *             graphs = [{k : j.numpy(force = True) for k, j in k.to_dict().items()} for k in graphs[0].to_data_list()]
  *             for k in inpt[i]:             # <<<<<<<<<<<<<<
  *                 if not isinstance(inpt[i][k], dict): inpt[i][k] = inpt[i][k].numpy(force = True)
  *                 else: inpt[i][k] = {l : inpt[i][k][l].numpy(force = True) for l in inpt[i][k]}
  */
     if (unlikely(__pyx_v_inpt == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 710, __pyx_L1_error)
+      __PYX_ERR(0, 713, __pyx_L1_error)
     }
-    __pyx_t_5 = __Pyx_GetItemInt_List(__pyx_v_inpt, __pyx_v_i, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 710, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_GetItemInt_List(__pyx_v_inpt, __pyx_v_i, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 713, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     if (likely(PyList_CheckExact(__pyx_t_5)) || PyTuple_CheckExact(__pyx_t_5)) {
       __pyx_t_3 = __pyx_t_5; __Pyx_INCREF(__pyx_t_3);
       __pyx_t_10 = 0;
       __pyx_t_11 = NULL;
     } else {
-      __pyx_t_10 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 710, __pyx_L1_error)
+      __pyx_t_10 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 713, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_11 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_3); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 710, __pyx_L1_error)
+      __pyx_t_11 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_3); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 713, __pyx_L1_error)
     }
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     for (;;) {
       if (likely(!__pyx_t_11)) {
         if (likely(PyList_CheckExact(__pyx_t_3))) {
           {
             Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_3);
             #if !CYTHON_ASSUME_SAFE_MACROS
-            if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 710, __pyx_L1_error)
+            if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 713, __pyx_L1_error)
             #endif
             if (__pyx_t_10 >= __pyx_temp) break;
           }
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_5 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_10); __Pyx_INCREF(__pyx_t_5); __pyx_t_10++; if (unlikely((0 < 0))) __PYX_ERR(0, 710, __pyx_L1_error)
+          __pyx_t_5 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_10); __Pyx_INCREF(__pyx_t_5); __pyx_t_10++; if (unlikely((0 < 0))) __PYX_ERR(0, 713, __pyx_L1_error)
           #else
-          __pyx_t_5 = __Pyx_PySequence_ITEM(__pyx_t_3, __pyx_t_10); __pyx_t_10++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 710, __pyx_L1_error)
+          __pyx_t_5 = __Pyx_PySequence_ITEM(__pyx_t_3, __pyx_t_10); __pyx_t_10++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 713, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_5);
           #endif
         } else {
           {
             Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_3);
             #if !CYTHON_ASSUME_SAFE_MACROS
-            if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 710, __pyx_L1_error)
+            if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 713, __pyx_L1_error)
             #endif
             if (__pyx_t_10 >= __pyx_temp) break;
           }
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_10); __Pyx_INCREF(__pyx_t_5); __pyx_t_10++; if (unlikely((0 < 0))) __PYX_ERR(0, 710, __pyx_L1_error)
+          __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_10); __Pyx_INCREF(__pyx_t_5); __pyx_t_10++; if (unlikely((0 < 0))) __PYX_ERR(0, 713, __pyx_L1_error)
           #else
-          __pyx_t_5 = __Pyx_PySequence_ITEM(__pyx_t_3, __pyx_t_10); __pyx_t_10++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 710, __pyx_L1_error)
+          __pyx_t_5 = __Pyx_PySequence_ITEM(__pyx_t_3, __pyx_t_10); __pyx_t_10++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 713, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_5);
           #endif
         }
       } else {
         __pyx_t_5 = __pyx_t_11(__pyx_t_3);
         if (unlikely(!__pyx_t_5)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 710, __pyx_L1_error)
+            else __PYX_ERR(0, 713, __pyx_L1_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_5);
       }
       __Pyx_XDECREF_SET(__pyx_v_k, __pyx_t_5);
       __pyx_t_5 = 0;
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":711
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":714
  *             graphs = [{k : j.numpy(force = True) for k, j in k.to_dict().items()} for k in graphs[0].to_data_list()]
  *             for k in inpt[i]:
  *                 if not isinstance(inpt[i][k], dict): inpt[i][k] = inpt[i][k].numpy(force = True)             # <<<<<<<<<<<<<<
  *                 else: inpt[i][k] = {l : inpt[i][k][l].numpy(force = True) for l in inpt[i][k]}
  *             inpt[i]["graphs"] = graphs
  */
       if (unlikely(__pyx_v_inpt == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-        __PYX_ERR(0, 711, __pyx_L1_error)
+        __PYX_ERR(0, 714, __pyx_L1_error)
       }
-      __pyx_t_5 = __Pyx_GetItemInt_List(__pyx_v_inpt, __pyx_v_i, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 711, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_GetItemInt_List(__pyx_v_inpt, __pyx_v_i, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 714, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_t_5, __pyx_v_k); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 711, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_t_5, __pyx_v_k); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 714, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __pyx_t_17 = PyDict_Check(__pyx_t_1); 
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_t_18 = (!__pyx_t_17);
       if (__pyx_t_18) {
         if (unlikely(__pyx_v_inpt == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-          __PYX_ERR(0, 711, __pyx_L1_error)
+          __PYX_ERR(0, 714, __pyx_L1_error)
         }
-        __pyx_t_1 = __Pyx_GetItemInt_List(__pyx_v_inpt, __pyx_v_i, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 711, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_GetItemInt_List(__pyx_v_inpt, __pyx_v_i, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 714, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
-        __pyx_t_5 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_v_k); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 711, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_v_k); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 714, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_numpy); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 711, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_numpy); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 714, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-        __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 711, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 714, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
-        if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_force, Py_True) < 0) __PYX_ERR(0, 711, __pyx_L1_error)
-        __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 711, __pyx_L1_error)
+        if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_force, Py_True) < 0) __PYX_ERR(0, 714, __pyx_L1_error)
+        __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 714, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
         if (unlikely(__pyx_v_inpt == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-          __PYX_ERR(0, 711, __pyx_L1_error)
+          __PYX_ERR(0, 714, __pyx_L1_error)
         }
-        __pyx_t_5 = __Pyx_GetItemInt_List(__pyx_v_inpt, __pyx_v_i, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 711, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_GetItemInt_List(__pyx_v_inpt, __pyx_v_i, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 714, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
-        if (unlikely((PyObject_SetItem(__pyx_t_5, __pyx_v_k, __pyx_t_4) < 0))) __PYX_ERR(0, 711, __pyx_L1_error)
+        if (unlikely((PyObject_SetItem(__pyx_t_5, __pyx_v_k, __pyx_t_4) < 0))) __PYX_ERR(0, 714, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         goto __pyx_L20;
       }
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":712
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":715
  *             for k in inpt[i]:
  *                 if not isinstance(inpt[i][k], dict): inpt[i][k] = inpt[i][k].numpy(force = True)
  *                 else: inpt[i][k] = {l : inpt[i][k][l].numpy(force = True) for l in inpt[i][k]}             # <<<<<<<<<<<<<<
  *             inpt[i]["graphs"] = graphs
  *             map_data = recast(inpt[i], out_map)
  */
       /*else*/ {
         { /* enter inner scope */
-          __pyx_t_4 = PyDict_New(); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 712, __pyx_L1_error)
+          __pyx_t_4 = PyDict_New(); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 715, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_4);
           if (unlikely(__pyx_v_inpt == Py_None)) {
             PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-            __PYX_ERR(0, 712, __pyx_L1_error)
+            __PYX_ERR(0, 715, __pyx_L1_error)
           }
-          __pyx_t_5 = __Pyx_GetItemInt_List(__pyx_v_inpt, __pyx_v_i, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 712, __pyx_L1_error)
+          __pyx_t_5 = __Pyx_GetItemInt_List(__pyx_v_inpt, __pyx_v_i, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 715, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_5);
-          __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_t_5, __pyx_v_k); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 712, __pyx_L1_error)
+          __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_t_5, __pyx_v_k); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 715, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_1);
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
           if (likely(PyList_CheckExact(__pyx_t_1)) || PyTuple_CheckExact(__pyx_t_1)) {
             __pyx_t_5 = __pyx_t_1; __Pyx_INCREF(__pyx_t_5);
             __pyx_t_13 = 0;
             __pyx_t_19 = NULL;
           } else {
-            __pyx_t_13 = -1; __pyx_t_5 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 712, __pyx_L1_error)
+            __pyx_t_13 = -1; __pyx_t_5 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 715, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_5);
-            __pyx_t_19 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_5); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 712, __pyx_L1_error)
+            __pyx_t_19 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_5); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 715, __pyx_L1_error)
           }
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
           for (;;) {
             if (likely(!__pyx_t_19)) {
               if (likely(PyList_CheckExact(__pyx_t_5))) {
                 {
                   Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_5);
                   #if !CYTHON_ASSUME_SAFE_MACROS
-                  if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 712, __pyx_L1_error)
+                  if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 715, __pyx_L1_error)
                   #endif
                   if (__pyx_t_13 >= __pyx_temp) break;
                 }
                 #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-                __pyx_t_1 = PyList_GET_ITEM(__pyx_t_5, __pyx_t_13); __Pyx_INCREF(__pyx_t_1); __pyx_t_13++; if (unlikely((0 < 0))) __PYX_ERR(0, 712, __pyx_L1_error)
+                __pyx_t_1 = PyList_GET_ITEM(__pyx_t_5, __pyx_t_13); __Pyx_INCREF(__pyx_t_1); __pyx_t_13++; if (unlikely((0 < 0))) __PYX_ERR(0, 715, __pyx_L1_error)
                 #else
-                __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_5, __pyx_t_13); __pyx_t_13++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 712, __pyx_L1_error)
+                __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_5, __pyx_t_13); __pyx_t_13++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 715, __pyx_L1_error)
                 __Pyx_GOTREF(__pyx_t_1);
                 #endif
               } else {
                 {
                   Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_5);
                   #if !CYTHON_ASSUME_SAFE_MACROS
-                  if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 712, __pyx_L1_error)
+                  if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 715, __pyx_L1_error)
                   #endif
                   if (__pyx_t_13 >= __pyx_temp) break;
                 }
                 #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-                __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_5, __pyx_t_13); __Pyx_INCREF(__pyx_t_1); __pyx_t_13++; if (unlikely((0 < 0))) __PYX_ERR(0, 712, __pyx_L1_error)
+                __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_5, __pyx_t_13); __Pyx_INCREF(__pyx_t_1); __pyx_t_13++; if (unlikely((0 < 0))) __PYX_ERR(0, 715, __pyx_L1_error)
                 #else
-                __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_5, __pyx_t_13); __pyx_t_13++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 712, __pyx_L1_error)
+                __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_5, __pyx_t_13); __pyx_t_13++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 715, __pyx_L1_error)
                 __Pyx_GOTREF(__pyx_t_1);
                 #endif
               }
             } else {
               __pyx_t_1 = __pyx_t_19(__pyx_t_5);
               if (unlikely(!__pyx_t_1)) {
                 PyObject* exc_type = PyErr_Occurred();
                 if (exc_type) {
                   if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-                  else __PYX_ERR(0, 712, __pyx_L1_error)
+                  else __PYX_ERR(0, 715, __pyx_L1_error)
                 }
                 break;
               }
               __Pyx_GOTREF(__pyx_t_1);
             }
-            __pyx_t_7 = __Pyx_PyInt_As_int(__pyx_t_1); if (unlikely((__pyx_t_7 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 712, __pyx_L1_error)
+            __pyx_t_7 = __Pyx_PyInt_As_int(__pyx_t_1); if (unlikely((__pyx_t_7 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 715, __pyx_L1_error)
             __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
             __pyx_9genexpr10__pyx_v_l = __pyx_t_7;
-            __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_9genexpr10__pyx_v_l); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 712, __pyx_L1_error)
+            __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_9genexpr10__pyx_v_l); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 715, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_1);
             if (unlikely(__pyx_v_inpt == Py_None)) {
               PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-              __PYX_ERR(0, 712, __pyx_L1_error)
+              __PYX_ERR(0, 715, __pyx_L1_error)
             }
-            __pyx_t_15 = __Pyx_GetItemInt_List(__pyx_v_inpt, __pyx_v_i, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 712, __pyx_L1_error)
+            __pyx_t_15 = __Pyx_GetItemInt_List(__pyx_v_inpt, __pyx_v_i, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 715, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_15);
-            __pyx_t_14 = __Pyx_PyObject_GetItem(__pyx_t_15, __pyx_v_k); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 712, __pyx_L1_error)
+            __pyx_t_14 = __Pyx_PyObject_GetItem(__pyx_t_15, __pyx_v_k); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 715, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_14);
             __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
-            __pyx_t_15 = __Pyx_GetItemInt(__pyx_t_14, __pyx_9genexpr10__pyx_v_l, int, 1, __Pyx_PyInt_From_int, 0, 1, 1); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 712, __pyx_L1_error)
+            __pyx_t_15 = __Pyx_GetItemInt(__pyx_t_14, __pyx_9genexpr10__pyx_v_l, int, 1, __Pyx_PyInt_From_int, 0, 1, 1); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 715, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_15);
             __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
-            __pyx_t_14 = __Pyx_PyObject_GetAttrStr(__pyx_t_15, __pyx_n_s_numpy); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 712, __pyx_L1_error)
+            __pyx_t_14 = __Pyx_PyObject_GetAttrStr(__pyx_t_15, __pyx_n_s_numpy); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 715, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_14);
             __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
-            __pyx_t_15 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 712, __pyx_L1_error)
+            __pyx_t_15 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 715, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_15);
-            if (PyDict_SetItem(__pyx_t_15, __pyx_n_s_force, Py_True) < 0) __PYX_ERR(0, 712, __pyx_L1_error)
-            __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_14, __pyx_empty_tuple, __pyx_t_15); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 712, __pyx_L1_error)
+            if (PyDict_SetItem(__pyx_t_15, __pyx_n_s_force, Py_True) < 0) __PYX_ERR(0, 715, __pyx_L1_error)
+            __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_14, __pyx_empty_tuple, __pyx_t_15); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 715, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_6);
             __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
             __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
-            if (unlikely(PyDict_SetItem(__pyx_t_4, (PyObject*)__pyx_t_1, (PyObject*)__pyx_t_6))) __PYX_ERR(0, 712, __pyx_L1_error)
+            if (unlikely(PyDict_SetItem(__pyx_t_4, (PyObject*)__pyx_t_1, (PyObject*)__pyx_t_6))) __PYX_ERR(0, 715, __pyx_L1_error)
             __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
             __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
           }
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
         } /* exit inner scope */
         if (unlikely(__pyx_v_inpt == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-          __PYX_ERR(0, 712, __pyx_L1_error)
+          __PYX_ERR(0, 715, __pyx_L1_error)
         }
-        __pyx_t_5 = __Pyx_GetItemInt_List(__pyx_v_inpt, __pyx_v_i, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 712, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_GetItemInt_List(__pyx_v_inpt, __pyx_v_i, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 715, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
-        if (unlikely((PyObject_SetItem(__pyx_t_5, __pyx_v_k, __pyx_t_4) < 0))) __PYX_ERR(0, 712, __pyx_L1_error)
+        if (unlikely((PyObject_SetItem(__pyx_t_5, __pyx_v_k, __pyx_t_4) < 0))) __PYX_ERR(0, 715, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       }
       __pyx_L20:;
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":710
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":713
  *             graphs = [Batch().from_data_list(graphs)]
  *             graphs = [{k : j.numpy(force = True) for k, j in k.to_dict().items()} for k in graphs[0].to_data_list()]
  *             for k in inpt[i]:             # <<<<<<<<<<<<<<
  *                 if not isinstance(inpt[i][k], dict): inpt[i][k] = inpt[i][k].numpy(force = True)
  *                 else: inpt[i][k] = {l : inpt[i][k][l].numpy(force = True) for l in inpt[i][k]}
  */
     }
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":713
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":716
  *                 if not isinstance(inpt[i][k], dict): inpt[i][k] = inpt[i][k].numpy(force = True)
  *                 else: inpt[i][k] = {l : inpt[i][k][l].numpy(force = True) for l in inpt[i][k]}
  *             inpt[i]["graphs"] = graphs             # <<<<<<<<<<<<<<
  *             map_data = recast(inpt[i], out_map)
  *             if  self._train: self.ptr.train_epoch_kfold(epoch, kfold, &map_data)
  */
     if (unlikely(__pyx_v_inpt == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 713, __pyx_L1_error)
+      __PYX_ERR(0, 716, __pyx_L1_error)
     }
-    __pyx_t_3 = __Pyx_GetItemInt_List(__pyx_v_inpt, __pyx_v_i, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 713, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_GetItemInt_List(__pyx_v_inpt, __pyx_v_i, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 716, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    if (unlikely((PyObject_SetItem(__pyx_t_3, __pyx_n_u_graphs, __pyx_v_graphs) < 0))) __PYX_ERR(0, 713, __pyx_L1_error)
+    if (unlikely((PyObject_SetItem(__pyx_t_3, __pyx_n_u_graphs, __pyx_v_graphs) < 0))) __PYX_ERR(0, 716, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":714
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":717
  *                 else: inpt[i][k] = {l : inpt[i][k][l].numpy(force = True) for l in inpt[i][k]}
  *             inpt[i]["graphs"] = graphs
  *             map_data = recast(inpt[i], out_map)             # <<<<<<<<<<<<<<
  *             if  self._train: self.ptr.train_epoch_kfold(epoch, kfold, &map_data)
  *             elif  self._val: self.ptr.validation_epoch_kfold(epoch, kfold, &map_data)
  */
     if (unlikely(__pyx_v_inpt == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 714, __pyx_L1_error)
+      __PYX_ERR(0, 717, __pyx_L1_error)
     }
-    __pyx_t_3 = __Pyx_GetItemInt_List(__pyx_v_inpt, __pyx_v_i, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 714, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_GetItemInt_List(__pyx_v_inpt, __pyx_v_i, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 717, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    if (!(likely(PyDict_CheckExact(__pyx_t_3))||((__pyx_t_3) == Py_None) || __Pyx_RaiseUnexpectedTypeError("dict", __pyx_t_3))) __PYX_ERR(0, 714, __pyx_L1_error)
-    __pyx_t_4 = __pyx_f_7cytools_recast(((PyObject*)__pyx_t_3), __pyx_v_out_map, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 714, __pyx_L1_error)
+    if (!(likely(PyDict_CheckExact(__pyx_t_3))||((__pyx_t_3) == Py_None) || __Pyx_RaiseUnexpectedTypeError("dict", __pyx_t_3))) __PYX_ERR(0, 717, __pyx_L1_error)
+    __pyx_t_4 = __pyx_f_7cytools_recast(((PyObject*)__pyx_t_3), __pyx_v_out_map, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 717, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_20 = __pyx_convert_map_from_py_std_3a__3a_string__and_struct__data_t(__pyx_t_4); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 714, __pyx_L1_error)
+    __pyx_t_20 = __pyx_convert_map_from_py_std_3a__3a_string__and_struct__data_t(__pyx_t_4); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 717, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_v_map_data = __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_20);
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":715
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":718
  *             inpt[i]["graphs"] = graphs
  *             map_data = recast(inpt[i], out_map)
  *             if  self._train: self.ptr.train_epoch_kfold(epoch, kfold, &map_data)             # <<<<<<<<<<<<<<
  *             elif  self._val: self.ptr.validation_epoch_kfold(epoch, kfold, &map_data)
  *             elif self._test: self.ptr.evaluation_epoch_kfold(epoch, kfold, &map_data)
  */
     __pyx_t_18 = (__pyx_v_self->_train != 0);
     if (__pyx_t_18) {
       try {
         __pyx_v_self->ptr->train_epoch_kfold(__pyx_v_epoch, __pyx_v_kfold, (&__pyx_v_map_data));
       } catch(...) {
         __Pyx_CppExn2PyErr();
-        __PYX_ERR(0, 715, __pyx_L1_error)
+        __PYX_ERR(0, 718, __pyx_L1_error)
       }
       goto __pyx_L25;
     }
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":716
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":719
  *             map_data = recast(inpt[i], out_map)
  *             if  self._train: self.ptr.train_epoch_kfold(epoch, kfold, &map_data)
  *             elif  self._val: self.ptr.validation_epoch_kfold(epoch, kfold, &map_data)             # <<<<<<<<<<<<<<
  *             elif self._test: self.ptr.evaluation_epoch_kfold(epoch, kfold, &map_data)
  *             map_data.clear()
  */
     __pyx_t_18 = (__pyx_v_self->_val != 0);
     if (__pyx_t_18) {
       try {
         __pyx_v_self->ptr->validation_epoch_kfold(__pyx_v_epoch, __pyx_v_kfold, (&__pyx_v_map_data));
       } catch(...) {
         __Pyx_CppExn2PyErr();
-        __PYX_ERR(0, 716, __pyx_L1_error)
+        __PYX_ERR(0, 719, __pyx_L1_error)
       }
       goto __pyx_L25;
     }
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":717
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":720
  *             if  self._train: self.ptr.train_epoch_kfold(epoch, kfold, &map_data)
  *             elif  self._val: self.ptr.validation_epoch_kfold(epoch, kfold, &map_data)
  *             elif self._test: self.ptr.evaluation_epoch_kfold(epoch, kfold, &map_data)             # <<<<<<<<<<<<<<
  *             map_data.clear()
  * 
  */
     __pyx_t_18 = (__pyx_v_self->_test != 0);
     if (__pyx_t_18) {
       try {
         __pyx_v_self->ptr->evaluation_epoch_kfold(__pyx_v_epoch, __pyx_v_kfold, (&__pyx_v_map_data));
       } catch(...) {
         __Pyx_CppExn2PyErr();
-        __PYX_ERR(0, 717, __pyx_L1_error)
+        __PYX_ERR(0, 720, __pyx_L1_error)
       }
     }
     __pyx_L25:;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":718
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":721
  *             elif  self._val: self.ptr.validation_epoch_kfold(epoch, kfold, &map_data)
  *             elif self._test: self.ptr.evaluation_epoch_kfold(epoch, kfold, &map_data)
  *             map_data.clear()             # <<<<<<<<<<<<<<
  * 
  *     cpdef DumpEpochHDF5(self, int epoch, str path, int kfold):
  */
     __pyx_v_map_data.clear();
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":706
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":709
  *         cdef list graphs
  *         cdef map[string, data_t] map_data
  *         for i in trange(len(inpt)):             # <<<<<<<<<<<<<<
  *             graphs = inpt[i].pop("graphs")
  *             graphs = [Batch().from_data_list(graphs)]
  */
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":701
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":704
  *         map_data.clear()
  * 
  *     cpdef FastGraphRecast(self, int epoch, int kfold, list inpt, dict out_map):             # <<<<<<<<<<<<<<
  *         cdef str key
  *         cdef int i, l
  */
 
@@ -41226,82 +41244,82 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_epoch_2)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 701, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 704, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_kfold_2)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 701, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 704, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("FastGraphRecast", 1, 4, 4, 1); __PYX_ERR(0, 701, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("FastGraphRecast", 1, 4, 4, 1); __PYX_ERR(0, 704, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_inpt)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[2]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 701, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 704, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("FastGraphRecast", 1, 4, 4, 2); __PYX_ERR(0, 701, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("FastGraphRecast", 1, 4, 4, 2); __PYX_ERR(0, 704, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_out_map)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[3]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 701, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 704, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("FastGraphRecast", 1, 4, 4, 3); __PYX_ERR(0, 701, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("FastGraphRecast", 1, 4, 4, 3); __PYX_ERR(0, 704, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "FastGraphRecast") < 0)) __PYX_ERR(0, 701, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "FastGraphRecast") < 0)) __PYX_ERR(0, 704, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 4)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
       values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
       values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
     }
-    __pyx_v_epoch = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_epoch == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 701, __pyx_L3_error)
-    __pyx_v_kfold = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_kfold == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 701, __pyx_L3_error)
+    __pyx_v_epoch = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_epoch == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 704, __pyx_L3_error)
+    __pyx_v_kfold = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_kfold == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 704, __pyx_L3_error)
     __pyx_v_inpt = ((PyObject*)values[2]);
     __pyx_v_out_map = ((PyObject*)values[3]);
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("FastGraphRecast", 1, 4, 4, __pyx_nargs); __PYX_ERR(0, 701, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("FastGraphRecast", 1, 4, 4, __pyx_nargs); __PYX_ERR(0, 704, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("AnalysisG._cmodules.cOptimizer.cOptimizer.FastGraphRecast", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_inpt), (&PyList_Type), 1, "inpt", 1))) __PYX_ERR(0, 701, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_out_map), (&PyDict_Type), 1, "out_map", 1))) __PYX_ERR(0, 701, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_inpt), (&PyList_Type), 1, "inpt", 1))) __PYX_ERR(0, 704, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_out_map), (&PyDict_Type), 1, "out_map", 1))) __PYX_ERR(0, 704, __pyx_L1_error)
   __pyx_r = __pyx_pf_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_24FastGraphRecast(((struct __pyx_obj_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer *)__pyx_v_self), __pyx_v_epoch, __pyx_v_kfold, __pyx_v_inpt, __pyx_v_out_map);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -41320,15 +41338,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("FastGraphRecast", 1);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_FastGraphRecast(__pyx_v_self, __pyx_v_epoch, __pyx_v_kfold, __pyx_v_inpt, __pyx_v_out_map, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 701, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_FastGraphRecast(__pyx_v_self, __pyx_v_epoch, __pyx_v_kfold, __pyx_v_inpt, __pyx_v_out_map, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 704, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -41337,15 +41355,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/cmodules/cyincludes/cyoptimizer.pyx":720
+/* "src/cmodules/cyincludes/cyoptimizer.pyx":723
  *             map_data.clear()
  * 
  *     cpdef DumpEpochHDF5(self, int epoch, str path, int kfold):             # <<<<<<<<<<<<<<
  * 
  *         cdef CyEpoch* ep
  */
 
@@ -41383,21 +41401,21 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || __Pyx_PyType_HasFeature(Py_TYPE(((PyObject *)__pyx_v_self)), (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_typedict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_DumpEpochHDF5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 720, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_DumpEpochHDF5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 723, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!__Pyx_IsSameCFunction(__pyx_t_1, (void*) __pyx_pw_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_27DumpEpochHDF5)) {
         __Pyx_XDECREF(__pyx_r);
-        __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_epoch); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 720, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_epoch); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 723, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
-        __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_kfold); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 720, __pyx_L1_error)
+        __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_kfold); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 723, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_5 = __pyx_t_1; __pyx_t_6 = NULL;
         __pyx_t_7 = 0;
         #if CYTHON_UNPACK_METHODS
         if (unlikely(PyMethod_Check(__pyx_t_5))) {
           __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
@@ -41412,15 +41430,15 @@
         #endif
         {
           PyObject *__pyx_callargs[4] = {__pyx_t_6, __pyx_t_3, __pyx_v_path, __pyx_t_4};
           __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_7, 3+__pyx_t_7);
           __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-          if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 720, __pyx_L1_error)
+          if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 723, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
         }
         __pyx_r = __pyx_t_2;
         __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
@@ -41434,35 +41452,35 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":724
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":727
  *         cdef CyEpoch* ep
  *         cdef pair[string, data_t] dt
  *         f = h5py.File(path + str(kfold) + "/epoch_data.hdf5", "w")             # <<<<<<<<<<<<<<
  *         if self.ptr.epoch_train.count(epoch):
  *             grp = _check_sub(f, "training")
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_h5py); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 724, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_h5py); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 727, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_File); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 724, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_File); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 727, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_kfold); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 724, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_kfold); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 727, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = __Pyx_PyObject_Str(__pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 724, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Str(__pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 727, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyNumber_Add(__pyx_v_path, __pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 724, __pyx_L1_error)
+  __pyx_t_2 = PyNumber_Add(__pyx_v_path, __pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 727, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyUnicode_ConcatInPlace(__pyx_t_2, __pyx_kp_u_epoch_data_hdf5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 724, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyUnicode_ConcatInPlace(__pyx_t_2, __pyx_kp_u_epoch_data_hdf5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 727, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   __pyx_t_7 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_5);
@@ -41476,251 +41494,251 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[3] = {__pyx_t_2, __pyx_t_4, __pyx_n_u_w};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_7, 2+__pyx_t_7);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 724, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 727, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
   __pyx_v_f = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":725
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":728
  *         cdef pair[string, data_t] dt
  *         f = h5py.File(path + str(kfold) + "/epoch_data.hdf5", "w")
  *         if self.ptr.epoch_train.count(epoch):             # <<<<<<<<<<<<<<
  *             grp = _check_sub(f, "training")
  *             ep = self.ptr.epoch_train[epoch]
  */
   __pyx_t_8 = (__pyx_v_self->ptr->epoch_train.count(__pyx_v_epoch) != 0);
   if (__pyx_t_8) {
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":726
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":729
  *         f = h5py.File(path + str(kfold) + "/epoch_data.hdf5", "w")
  *         if self.ptr.epoch_train.count(epoch):
  *             grp = _check_sub(f, "training")             # <<<<<<<<<<<<<<
  *             ep = self.ptr.epoch_train[epoch]
  *             for dt in ep.container[kfold]: _check_h5(grp, env(dt.first), &dt.second)
  */
-    __pyx_t_1 = __pyx_f_9AnalysisG_9_cmodules_10cOptimizer__check_sub(__pyx_v_f, __pyx_n_u_training); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 726, __pyx_L1_error)
+    __pyx_t_1 = __pyx_f_9AnalysisG_9_cmodules_10cOptimizer__check_sub(__pyx_v_f, __pyx_n_u_training); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 729, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_v_grp = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":727
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":730
  *         if self.ptr.epoch_train.count(epoch):
  *             grp = _check_sub(f, "training")
  *             ep = self.ptr.epoch_train[epoch]             # <<<<<<<<<<<<<<
  *             for dt in ep.container[kfold]: _check_h5(grp, env(dt.first), &dt.second)
  *             ep.process_data()
  */
     __pyx_v_ep = (__pyx_v_self->ptr->epoch_train[__pyx_v_epoch]);
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":728
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":731
  *             grp = _check_sub(f, "training")
  *             ep = self.ptr.epoch_train[epoch]
  *             for dt in ep.container[kfold]: _check_h5(grp, env(dt.first), &dt.second)             # <<<<<<<<<<<<<<
  *             ep.process_data()
  * 
  */
     __pyx_t_10 = &(__pyx_v_ep->container[__pyx_v_kfold]);
     __pyx_t_9 = __pyx_t_10->begin();
     for (;;) {
       if (!(__pyx_t_9 != __pyx_t_10->end())) break;
       __pyx_t_11 = *__pyx_t_9;
       ++__pyx_t_9;
       __pyx_v_dt = __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_11);
-      __pyx_t_1 = __pyx_f_7cytools_env(__pyx_v_dt.first); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 728, __pyx_L1_error)
+      __pyx_t_1 = __pyx_f_7cytools_env(__pyx_v_dt.first); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 731, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_f_11cyoptimizer__check_h5(__pyx_v_grp, ((PyObject*)__pyx_t_1), (&__pyx_v_dt.second)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 728, __pyx_L1_error)
+      __pyx_f_11cyoptimizer__check_h5(__pyx_v_grp, ((PyObject*)__pyx_t_1), (&__pyx_v_dt.second)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 731, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     }
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":729
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":732
  *             ep = self.ptr.epoch_train[epoch]
  *             for dt in ep.container[kfold]: _check_h5(grp, env(dt.first), &dt.second)
  *             ep.process_data()             # <<<<<<<<<<<<<<
  * 
  *         if self.ptr.epoch_valid.count(epoch):
  */
     try {
       __pyx_v_ep->process_data();
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 729, __pyx_L1_error)
+      __PYX_ERR(0, 732, __pyx_L1_error)
     }
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":725
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":728
  *         cdef pair[string, data_t] dt
  *         f = h5py.File(path + str(kfold) + "/epoch_data.hdf5", "w")
  *         if self.ptr.epoch_train.count(epoch):             # <<<<<<<<<<<<<<
  *             grp = _check_sub(f, "training")
  *             ep = self.ptr.epoch_train[epoch]
  */
   }
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":731
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":734
  *             ep.process_data()
  * 
  *         if self.ptr.epoch_valid.count(epoch):             # <<<<<<<<<<<<<<
  *             grp = _check_sub(f, "validation")
  *             ep = self.ptr.epoch_valid[epoch]
  */
   __pyx_t_8 = (__pyx_v_self->ptr->epoch_valid.count(__pyx_v_epoch) != 0);
   if (__pyx_t_8) {
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":732
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":735
  * 
  *         if self.ptr.epoch_valid.count(epoch):
  *             grp = _check_sub(f, "validation")             # <<<<<<<<<<<<<<
  *             ep = self.ptr.epoch_valid[epoch]
  *             for dt in ep.container[kfold]: _check_h5(grp, env(dt.first), &dt.second)
  */
-    __pyx_t_1 = __pyx_f_9AnalysisG_9_cmodules_10cOptimizer__check_sub(__pyx_v_f, __pyx_n_u_validation); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 732, __pyx_L1_error)
+    __pyx_t_1 = __pyx_f_9AnalysisG_9_cmodules_10cOptimizer__check_sub(__pyx_v_f, __pyx_n_u_validation); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 735, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_XDECREF_SET(__pyx_v_grp, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":733
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":736
  *         if self.ptr.epoch_valid.count(epoch):
  *             grp = _check_sub(f, "validation")
  *             ep = self.ptr.epoch_valid[epoch]             # <<<<<<<<<<<<<<
  *             for dt in ep.container[kfold]: _check_h5(grp, env(dt.first), &dt.second)
  *             ep.process_data()
  */
     __pyx_v_ep = (__pyx_v_self->ptr->epoch_valid[__pyx_v_epoch]);
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":734
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":737
  *             grp = _check_sub(f, "validation")
  *             ep = self.ptr.epoch_valid[epoch]
  *             for dt in ep.container[kfold]: _check_h5(grp, env(dt.first), &dt.second)             # <<<<<<<<<<<<<<
  *             ep.process_data()
  * 
  */
     __pyx_t_10 = &(__pyx_v_ep->container[__pyx_v_kfold]);
     __pyx_t_9 = __pyx_t_10->begin();
     for (;;) {
       if (!(__pyx_t_9 != __pyx_t_10->end())) break;
       __pyx_t_11 = *__pyx_t_9;
       ++__pyx_t_9;
       __pyx_v_dt = __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_11);
-      __pyx_t_1 = __pyx_f_7cytools_env(__pyx_v_dt.first); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 734, __pyx_L1_error)
+      __pyx_t_1 = __pyx_f_7cytools_env(__pyx_v_dt.first); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 737, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_f_11cyoptimizer__check_h5(__pyx_v_grp, ((PyObject*)__pyx_t_1), (&__pyx_v_dt.second)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 734, __pyx_L1_error)
+      __pyx_f_11cyoptimizer__check_h5(__pyx_v_grp, ((PyObject*)__pyx_t_1), (&__pyx_v_dt.second)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 737, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     }
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":735
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":738
  *             ep = self.ptr.epoch_valid[epoch]
  *             for dt in ep.container[kfold]: _check_h5(grp, env(dt.first), &dt.second)
  *             ep.process_data()             # <<<<<<<<<<<<<<
  * 
  *         if self.ptr.epoch_test.count(epoch):
  */
     try {
       __pyx_v_ep->process_data();
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 735, __pyx_L1_error)
+      __PYX_ERR(0, 738, __pyx_L1_error)
     }
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":731
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":734
  *             ep.process_data()
  * 
  *         if self.ptr.epoch_valid.count(epoch):             # <<<<<<<<<<<<<<
  *             grp = _check_sub(f, "validation")
  *             ep = self.ptr.epoch_valid[epoch]
  */
   }
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":737
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":740
  *             ep.process_data()
  * 
  *         if self.ptr.epoch_test.count(epoch):             # <<<<<<<<<<<<<<
  *             grp = _check_sub(f, "evaluation")
  *             ep = self.ptr.epoch_test[epoch]
  */
   __pyx_t_8 = (__pyx_v_self->ptr->epoch_test.count(__pyx_v_epoch) != 0);
   if (__pyx_t_8) {
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":738
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":741
  * 
  *         if self.ptr.epoch_test.count(epoch):
  *             grp = _check_sub(f, "evaluation")             # <<<<<<<<<<<<<<
  *             ep = self.ptr.epoch_test[epoch]
  *             for dt in ep.container[kfold]: _check_h5(grp, env(dt.first), &dt.second)
  */
-    __pyx_t_1 = __pyx_f_9AnalysisG_9_cmodules_10cOptimizer__check_sub(__pyx_v_f, __pyx_n_u_evaluation); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 738, __pyx_L1_error)
+    __pyx_t_1 = __pyx_f_9AnalysisG_9_cmodules_10cOptimizer__check_sub(__pyx_v_f, __pyx_n_u_evaluation); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 741, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_XDECREF_SET(__pyx_v_grp, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":739
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":742
  *         if self.ptr.epoch_test.count(epoch):
  *             grp = _check_sub(f, "evaluation")
  *             ep = self.ptr.epoch_test[epoch]             # <<<<<<<<<<<<<<
  *             for dt in ep.container[kfold]: _check_h5(grp, env(dt.first), &dt.second)
  *             ep.process_data()
  */
     __pyx_v_ep = (__pyx_v_self->ptr->epoch_test[__pyx_v_epoch]);
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":740
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":743
  *             grp = _check_sub(f, "evaluation")
  *             ep = self.ptr.epoch_test[epoch]
  *             for dt in ep.container[kfold]: _check_h5(grp, env(dt.first), &dt.second)             # <<<<<<<<<<<<<<
  *             ep.process_data()
  *         f.close()
  */
     __pyx_t_10 = &(__pyx_v_ep->container[__pyx_v_kfold]);
     __pyx_t_9 = __pyx_t_10->begin();
     for (;;) {
       if (!(__pyx_t_9 != __pyx_t_10->end())) break;
       __pyx_t_11 = *__pyx_t_9;
       ++__pyx_t_9;
       __pyx_v_dt = __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_11);
-      __pyx_t_1 = __pyx_f_7cytools_env(__pyx_v_dt.first); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 740, __pyx_L1_error)
+      __pyx_t_1 = __pyx_f_7cytools_env(__pyx_v_dt.first); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 743, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_f_11cyoptimizer__check_h5(__pyx_v_grp, ((PyObject*)__pyx_t_1), (&__pyx_v_dt.second)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 740, __pyx_L1_error)
+      __pyx_f_11cyoptimizer__check_h5(__pyx_v_grp, ((PyObject*)__pyx_t_1), (&__pyx_v_dt.second)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 743, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     }
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":741
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":744
  *             ep = self.ptr.epoch_test[epoch]
  *             for dt in ep.container[kfold]: _check_h5(grp, env(dt.first), &dt.second)
  *             ep.process_data()             # <<<<<<<<<<<<<<
  *         f.close()
  *         gc.collect()
  */
     try {
       __pyx_v_ep->process_data();
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 741, __pyx_L1_error)
+      __PYX_ERR(0, 744, __pyx_L1_error)
     }
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":737
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":740
  *             ep.process_data()
  * 
  *         if self.ptr.epoch_test.count(epoch):             # <<<<<<<<<<<<<<
  *             grp = _check_sub(f, "evaluation")
  *             ep = self.ptr.epoch_test[epoch]
  */
   }
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":742
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":745
  *             for dt in ep.container[kfold]: _check_h5(grp, env(dt.first), &dt.second)
  *             ep.process_data()
  *         f.close()             # <<<<<<<<<<<<<<
  *         gc.collect()
  * 
  */
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_f, __pyx_n_s_close); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 742, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_f, __pyx_n_s_close); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 745, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_4 = NULL;
   __pyx_t_7 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_4)) {
@@ -41732,30 +41750,30 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_4, NULL};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_7, 0+__pyx_t_7);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 742, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 745, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":743
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":746
  *             ep.process_data()
  *         f.close()
  *         gc.collect()             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_gc); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 743, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_gc); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 746, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_collect); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 743, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_collect); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 746, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_5 = NULL;
   __pyx_t_7 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
@@ -41768,21 +41786,21 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_5, NULL};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_7, 0+__pyx_t_7);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 743, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 746, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":720
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":723
  *             map_data.clear()
  * 
  *     cpdef DumpEpochHDF5(self, int epoch, str path, int kfold):             # <<<<<<<<<<<<<<
  * 
  *         cdef CyEpoch* ep
  */
 
@@ -41861,69 +41879,69 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_epoch_2)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 720, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 723, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_path)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 720, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 723, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("DumpEpochHDF5", 1, 3, 3, 1); __PYX_ERR(0, 720, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("DumpEpochHDF5", 1, 3, 3, 1); __PYX_ERR(0, 723, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_kfold_2)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[2]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 720, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 723, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("DumpEpochHDF5", 1, 3, 3, 2); __PYX_ERR(0, 720, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("DumpEpochHDF5", 1, 3, 3, 2); __PYX_ERR(0, 723, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "DumpEpochHDF5") < 0)) __PYX_ERR(0, 720, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "DumpEpochHDF5") < 0)) __PYX_ERR(0, 723, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 3)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
       values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
     }
-    __pyx_v_epoch = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_epoch == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 720, __pyx_L3_error)
+    __pyx_v_epoch = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_epoch == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 723, __pyx_L3_error)
     __pyx_v_path = ((PyObject*)values[1]);
-    __pyx_v_kfold = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_kfold == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 720, __pyx_L3_error)
+    __pyx_v_kfold = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_kfold == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 723, __pyx_L3_error)
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("DumpEpochHDF5", 1, 3, 3, __pyx_nargs); __PYX_ERR(0, 720, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("DumpEpochHDF5", 1, 3, 3, __pyx_nargs); __PYX_ERR(0, 723, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("AnalysisG._cmodules.cOptimizer.cOptimizer.DumpEpochHDF5", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_path), (&PyUnicode_Type), 1, "path", 1))) __PYX_ERR(0, 720, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_path), (&PyUnicode_Type), 1, "path", 1))) __PYX_ERR(0, 723, __pyx_L1_error)
   __pyx_r = __pyx_pf_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_26DumpEpochHDF5(((struct __pyx_obj_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer *)__pyx_v_self), __pyx_v_epoch, __pyx_v_path, __pyx_v_kfold);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -41942,15 +41960,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("DumpEpochHDF5", 1);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_DumpEpochHDF5(__pyx_v_self, __pyx_v_epoch, __pyx_v_path, __pyx_v_kfold, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 720, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_DumpEpochHDF5(__pyx_v_self, __pyx_v_epoch, __pyx_v_path, __pyx_v_kfold, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 723, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -41959,15 +41977,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/cmodules/cyincludes/cyoptimizer.pyx":746
+/* "src/cmodules/cyincludes/cyoptimizer.pyx":749
  * 
  * 
  *     cpdef RebuildEpochHDF5(self, int epoch, str path, int kfold):             # <<<<<<<<<<<<<<
  *         f = h5py.File(path + str(kfold) + "/epoch_data.hdf5", "r")
  * 
  */
 
@@ -42005,21 +42023,21 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || __Pyx_PyType_HasFeature(Py_TYPE(((PyObject *)__pyx_v_self)), (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_typedict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_RebuildEpochHDF5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 746, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_RebuildEpochHDF5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 749, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!__Pyx_IsSameCFunction(__pyx_t_1, (void*) __pyx_pw_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_29RebuildEpochHDF5)) {
         __Pyx_XDECREF(__pyx_r);
-        __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_epoch); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 746, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_epoch); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 749, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
-        __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_kfold); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 746, __pyx_L1_error)
+        __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_kfold); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 749, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_5 = __pyx_t_1; __pyx_t_6 = NULL;
         __pyx_t_7 = 0;
         #if CYTHON_UNPACK_METHODS
         if (unlikely(PyMethod_Check(__pyx_t_5))) {
           __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
@@ -42034,15 +42052,15 @@
         #endif
         {
           PyObject *__pyx_callargs[4] = {__pyx_t_6, __pyx_t_3, __pyx_v_path, __pyx_t_4};
           __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_7, 3+__pyx_t_7);
           __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-          if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 746, __pyx_L1_error)
+          if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 749, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
         }
         __pyx_r = __pyx_t_2;
         __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
@@ -42056,35 +42074,35 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":747
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":750
  * 
  *     cpdef RebuildEpochHDF5(self, int epoch, str path, int kfold):
  *         f = h5py.File(path + str(kfold) + "/epoch_data.hdf5", "r")             # <<<<<<<<<<<<<<
  * 
  *         cdef str key
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_h5py); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 747, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_h5py); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 750, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_File); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 747, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_File); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 750, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_kfold); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 747, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_kfold); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 750, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = __Pyx_PyObject_Str(__pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 747, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Str(__pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 750, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyNumber_Add(__pyx_v_path, __pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 747, __pyx_L1_error)
+  __pyx_t_2 = PyNumber_Add(__pyx_v_path, __pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 750, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyUnicode_ConcatInPlace(__pyx_t_2, __pyx_kp_u_epoch_data_hdf5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 747, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyUnicode_ConcatInPlace(__pyx_t_2, __pyx_kp_u_epoch_data_hdf5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 750, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   __pyx_t_7 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_5);
@@ -42098,155 +42116,155 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[3] = {__pyx_t_2, __pyx_t_4, __pyx_n_u_r};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_7, 2+__pyx_t_7);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 747, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 750, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
   __pyx_v_f = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":750
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":753
  * 
  *         cdef str key
  *         cdef dict unique = {}             # <<<<<<<<<<<<<<
  *         for key in f["training"].keys():
  *             key = key.split("-")[0]
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 750, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 753, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_unique = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":751
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":754
  *         cdef str key
  *         cdef dict unique = {}
  *         for key in f["training"].keys():             # <<<<<<<<<<<<<<
  *             key = key.split("-")[0]
  *             if key in unique: pass
  */
   __pyx_t_8 = 0;
-  __pyx_t_5 = __Pyx_PyObject_Dict_GetItem(__pyx_v_f, __pyx_n_u_training); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 751, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Dict_GetItem(__pyx_v_f, __pyx_n_u_training); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 754, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (unlikely(__pyx_t_5 == Py_None)) {
     PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "keys");
-    __PYX_ERR(0, 751, __pyx_L1_error)
+    __PYX_ERR(0, 754, __pyx_L1_error)
   }
-  __pyx_t_4 = __Pyx_dict_iterator(__pyx_t_5, 0, __pyx_n_s_keys, (&__pyx_t_9), (&__pyx_t_7)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 751, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_dict_iterator(__pyx_t_5, 0, __pyx_n_s_keys, (&__pyx_t_9), (&__pyx_t_7)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 754, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_XDECREF(__pyx_t_1);
   __pyx_t_1 = __pyx_t_4;
   __pyx_t_4 = 0;
   while (1) {
     __pyx_t_10 = __Pyx_dict_iter_next(__pyx_t_1, __pyx_t_9, &__pyx_t_8, &__pyx_t_4, NULL, NULL, __pyx_t_7);
     if (unlikely(__pyx_t_10 == 0)) break;
-    if (unlikely(__pyx_t_10 == -1)) __PYX_ERR(0, 751, __pyx_L1_error)
+    if (unlikely(__pyx_t_10 == -1)) __PYX_ERR(0, 754, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    if (!(likely(PyUnicode_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_t_4))) __PYX_ERR(0, 751, __pyx_L1_error)
+    if (!(likely(PyUnicode_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_t_4))) __PYX_ERR(0, 754, __pyx_L1_error)
     __Pyx_XDECREF_SET(__pyx_v_key, ((PyObject*)__pyx_t_4));
     __pyx_t_4 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":752
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":755
  *         cdef dict unique = {}
  *         for key in f["training"].keys():
  *             key = key.split("-")[0]             # <<<<<<<<<<<<<<
  *             if key in unique: pass
  *             else: unique[key] = None
  */
     if (unlikely(__pyx_v_key == Py_None)) {
       PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "split");
-      __PYX_ERR(0, 752, __pyx_L1_error)
+      __PYX_ERR(0, 755, __pyx_L1_error)
     }
-    __pyx_t_4 = PyUnicode_Split(__pyx_v_key, __Pyx_NoneAsNull(__pyx_kp_u__65), -1L); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 752, __pyx_L1_error)
+    __pyx_t_4 = PyUnicode_Split(__pyx_v_key, __Pyx_NoneAsNull(__pyx_kp_u__65), -1L); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 755, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = __Pyx_GetItemInt_List(__pyx_t_4, 0, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 752, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_GetItemInt_List(__pyx_t_4, 0, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 755, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (!(likely(PyUnicode_CheckExact(__pyx_t_5))||((__pyx_t_5) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_t_5))) __PYX_ERR(0, 752, __pyx_L1_error)
+    if (!(likely(PyUnicode_CheckExact(__pyx_t_5))||((__pyx_t_5) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_t_5))) __PYX_ERR(0, 755, __pyx_L1_error)
     __Pyx_DECREF_SET(__pyx_v_key, ((PyObject*)__pyx_t_5));
     __pyx_t_5 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":753
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":756
  *         for key in f["training"].keys():
  *             key = key.split("-")[0]
  *             if key in unique: pass             # <<<<<<<<<<<<<<
  *             else: unique[key] = None
  *         _rebuild_h5(f, list(unique), self.ptr, b"training"  , epoch, kfold)
  */
-    __pyx_t_11 = (__Pyx_PyDict_ContainsTF(__pyx_v_key, __pyx_v_unique, Py_EQ)); if (unlikely((__pyx_t_11 < 0))) __PYX_ERR(0, 753, __pyx_L1_error)
+    __pyx_t_11 = (__Pyx_PyDict_ContainsTF(__pyx_v_key, __pyx_v_unique, Py_EQ)); if (unlikely((__pyx_t_11 < 0))) __PYX_ERR(0, 756, __pyx_L1_error)
     if (__pyx_t_11) {
       goto __pyx_L5;
     }
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":754
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":757
  *             key = key.split("-")[0]
  *             if key in unique: pass
  *             else: unique[key] = None             # <<<<<<<<<<<<<<
  *         _rebuild_h5(f, list(unique), self.ptr, b"training"  , epoch, kfold)
  *         _rebuild_h5(f, list(unique), self.ptr, b"validation", epoch, kfold)
  */
     /*else*/ {
-      if (unlikely((PyDict_SetItem(__pyx_v_unique, __pyx_v_key, Py_None) < 0))) __PYX_ERR(0, 754, __pyx_L1_error)
+      if (unlikely((PyDict_SetItem(__pyx_v_unique, __pyx_v_key, Py_None) < 0))) __PYX_ERR(0, 757, __pyx_L1_error)
     }
     __pyx_L5:;
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":755
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":758
  *             if key in unique: pass
  *             else: unique[key] = None
  *         _rebuild_h5(f, list(unique), self.ptr, b"training"  , epoch, kfold)             # <<<<<<<<<<<<<<
  *         _rebuild_h5(f, list(unique), self.ptr, b"validation", epoch, kfold)
  *         _rebuild_h5(f, list(unique), self.ptr, b"evaluation", epoch, kfold)
  */
-  __pyx_t_1 = PySequence_List(__pyx_v_unique); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 755, __pyx_L1_error)
+  __pyx_t_1 = PySequence_List(__pyx_v_unique); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 758, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_12 = __pyx_convert_string_from_py_6libcpp_6string_std__in_string(__pyx_n_b_training); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 755, __pyx_L1_error)
-  __pyx_f_11cyoptimizer__rebuild_h5(__pyx_v_f, ((PyObject*)__pyx_t_1), __pyx_v_self->ptr, __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_12), __pyx_v_epoch, __pyx_v_kfold); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 755, __pyx_L1_error)
+  __pyx_t_12 = __pyx_convert_string_from_py_6libcpp_6string_std__in_string(__pyx_n_b_training); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 758, __pyx_L1_error)
+  __pyx_f_11cyoptimizer__rebuild_h5(__pyx_v_f, ((PyObject*)__pyx_t_1), __pyx_v_self->ptr, __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_12), __pyx_v_epoch, __pyx_v_kfold); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 758, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":756
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":759
  *             else: unique[key] = None
  *         _rebuild_h5(f, list(unique), self.ptr, b"training"  , epoch, kfold)
  *         _rebuild_h5(f, list(unique), self.ptr, b"validation", epoch, kfold)             # <<<<<<<<<<<<<<
  *         _rebuild_h5(f, list(unique), self.ptr, b"evaluation", epoch, kfold)
  *         f.close()
  */
-  __pyx_t_1 = PySequence_List(__pyx_v_unique); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 756, __pyx_L1_error)
+  __pyx_t_1 = PySequence_List(__pyx_v_unique); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 759, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_12 = __pyx_convert_string_from_py_6libcpp_6string_std__in_string(__pyx_n_b_validation); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 756, __pyx_L1_error)
-  __pyx_f_11cyoptimizer__rebuild_h5(__pyx_v_f, ((PyObject*)__pyx_t_1), __pyx_v_self->ptr, __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_12), __pyx_v_epoch, __pyx_v_kfold); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 756, __pyx_L1_error)
+  __pyx_t_12 = __pyx_convert_string_from_py_6libcpp_6string_std__in_string(__pyx_n_b_validation); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 759, __pyx_L1_error)
+  __pyx_f_11cyoptimizer__rebuild_h5(__pyx_v_f, ((PyObject*)__pyx_t_1), __pyx_v_self->ptr, __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_12), __pyx_v_epoch, __pyx_v_kfold); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 759, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":757
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":760
  *         _rebuild_h5(f, list(unique), self.ptr, b"training"  , epoch, kfold)
  *         _rebuild_h5(f, list(unique), self.ptr, b"validation", epoch, kfold)
  *         _rebuild_h5(f, list(unique), self.ptr, b"evaluation", epoch, kfold)             # <<<<<<<<<<<<<<
  *         f.close()
  * 
  */
-  __pyx_t_1 = PySequence_List(__pyx_v_unique); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 757, __pyx_L1_error)
+  __pyx_t_1 = PySequence_List(__pyx_v_unique); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 760, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_12 = __pyx_convert_string_from_py_6libcpp_6string_std__in_string(__pyx_n_b_evaluation); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 757, __pyx_L1_error)
-  __pyx_f_11cyoptimizer__rebuild_h5(__pyx_v_f, ((PyObject*)__pyx_t_1), __pyx_v_self->ptr, __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_12), __pyx_v_epoch, __pyx_v_kfold); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 757, __pyx_L1_error)
+  __pyx_t_12 = __pyx_convert_string_from_py_6libcpp_6string_std__in_string(__pyx_n_b_evaluation); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 760, __pyx_L1_error)
+  __pyx_f_11cyoptimizer__rebuild_h5(__pyx_v_f, ((PyObject*)__pyx_t_1), __pyx_v_self->ptr, __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_12), __pyx_v_epoch, __pyx_v_kfold); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 760, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":758
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":761
  *         _rebuild_h5(f, list(unique), self.ptr, b"validation", epoch, kfold)
  *         _rebuild_h5(f, list(unique), self.ptr, b"evaluation", epoch, kfold)
  *         f.close()             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_f, __pyx_n_s_close); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 758, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_f, __pyx_n_s_close); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 761, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_4 = NULL;
   __pyx_t_7 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_4)) {
@@ -42258,21 +42276,21 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_4, NULL};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_7, 0+__pyx_t_7);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 758, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 761, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":746
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":749
  * 
  * 
  *     cpdef RebuildEpochHDF5(self, int epoch, str path, int kfold):             # <<<<<<<<<<<<<<
  *         f = h5py.File(path + str(kfold) + "/epoch_data.hdf5", "r")
  * 
  */
 
@@ -42352,69 +42370,69 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_epoch_2)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 746, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 749, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_path)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 746, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 749, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("RebuildEpochHDF5", 1, 3, 3, 1); __PYX_ERR(0, 746, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("RebuildEpochHDF5", 1, 3, 3, 1); __PYX_ERR(0, 749, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_kfold_2)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[2]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 746, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 749, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("RebuildEpochHDF5", 1, 3, 3, 2); __PYX_ERR(0, 746, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("RebuildEpochHDF5", 1, 3, 3, 2); __PYX_ERR(0, 749, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "RebuildEpochHDF5") < 0)) __PYX_ERR(0, 746, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "RebuildEpochHDF5") < 0)) __PYX_ERR(0, 749, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 3)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
       values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
     }
-    __pyx_v_epoch = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_epoch == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 746, __pyx_L3_error)
+    __pyx_v_epoch = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_epoch == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 749, __pyx_L3_error)
     __pyx_v_path = ((PyObject*)values[1]);
-    __pyx_v_kfold = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_kfold == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 746, __pyx_L3_error)
+    __pyx_v_kfold = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_kfold == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 749, __pyx_L3_error)
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("RebuildEpochHDF5", 1, 3, 3, __pyx_nargs); __PYX_ERR(0, 746, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("RebuildEpochHDF5", 1, 3, 3, __pyx_nargs); __PYX_ERR(0, 749, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("AnalysisG._cmodules.cOptimizer.cOptimizer.RebuildEpochHDF5", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_path), (&PyUnicode_Type), 1, "path", 1))) __PYX_ERR(0, 746, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_path), (&PyUnicode_Type), 1, "path", 1))) __PYX_ERR(0, 749, __pyx_L1_error)
   __pyx_r = __pyx_pf_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_28RebuildEpochHDF5(((struct __pyx_obj_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer *)__pyx_v_self), __pyx_v_epoch, __pyx_v_path, __pyx_v_kfold);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -42433,15 +42451,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("RebuildEpochHDF5", 1);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_RebuildEpochHDF5(__pyx_v_self, __pyx_v_epoch, __pyx_v_path, __pyx_v_kfold, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 746, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_RebuildEpochHDF5(__pyx_v_self, __pyx_v_epoch, __pyx_v_path, __pyx_v_kfold, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 749, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -42450,15 +42468,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/cmodules/cyincludes/cyoptimizer.pyx":761
+/* "src/cmodules/cyincludes/cyoptimizer.pyx":764
  * 
  * 
  *     cpdef BuildPlots(self, int epoch, str path):             # <<<<<<<<<<<<<<
  *         make_mass_plots(self.ptr.epoch_train, self.ptr.epoch_valid, self.ptr.epoch_test, path)
  *         make_accuracy_plots(self.ptr.epoch_train, self.ptr.epoch_valid, self.ptr.epoch_test, path, &self.state)
  */
 
@@ -42487,19 +42505,19 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || __Pyx_PyType_HasFeature(Py_TYPE(((PyObject *)__pyx_v_self)), (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_typedict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_BuildPlots); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 761, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_BuildPlots); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 764, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!__Pyx_IsSameCFunction(__pyx_t_1, (void*) __pyx_pw_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_31BuildPlots)) {
         __Pyx_XDECREF(__pyx_r);
-        __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_epoch); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 761, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_epoch); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 764, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_4 = __pyx_t_1; __pyx_t_5 = NULL;
         __pyx_t_6 = 0;
         #if CYTHON_UNPACK_METHODS
         if (unlikely(PyMethod_Check(__pyx_t_4))) {
           __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
@@ -42513,15 +42531,15 @@
         }
         #endif
         {
           PyObject *__pyx_callargs[3] = {__pyx_t_5, __pyx_t_3, __pyx_v_path};
           __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_6, 2+__pyx_t_6);
           __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-          if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 761, __pyx_L1_error)
+          if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 764, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         }
         __pyx_r = __pyx_t_2;
         __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
@@ -42535,60 +42553,60 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":762
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":765
  * 
  *     cpdef BuildPlots(self, int epoch, str path):
  *         make_mass_plots(self.ptr.epoch_train, self.ptr.epoch_valid, self.ptr.epoch_test, path)             # <<<<<<<<<<<<<<
  *         make_accuracy_plots(self.ptr.epoch_train, self.ptr.epoch_valid, self.ptr.epoch_test, path, &self.state)
  *         make_loss_plots(self.ptr.epoch_train, self.ptr.epoch_valid, self.ptr.epoch_test, path, &self.state)
  */
-  __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_make_mass_plots(__pyx_v_self->ptr->epoch_train, __pyx_v_self->ptr->epoch_valid, __pyx_v_self->ptr->epoch_test, __pyx_v_path); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 762, __pyx_L1_error)
+  __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_make_mass_plots(__pyx_v_self->ptr->epoch_train, __pyx_v_self->ptr->epoch_valid, __pyx_v_self->ptr->epoch_test, __pyx_v_path); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 765, __pyx_L1_error)
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":763
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":766
  *     cpdef BuildPlots(self, int epoch, str path):
  *         make_mass_plots(self.ptr.epoch_train, self.ptr.epoch_valid, self.ptr.epoch_test, path)
  *         make_accuracy_plots(self.ptr.epoch_train, self.ptr.epoch_valid, self.ptr.epoch_test, path, &self.state)             # <<<<<<<<<<<<<<
  *         make_loss_plots(self.ptr.epoch_train, self.ptr.epoch_valid, self.ptr.epoch_test, path, &self.state)
  *         make_roc_plots(self.ptr.epoch_train, self.ptr.epoch_valid, self.ptr.epoch_test, path, &self.state)
  */
-  __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_make_accuracy_plots(__pyx_v_self->ptr->epoch_train, __pyx_v_self->ptr->epoch_valid, __pyx_v_self->ptr->epoch_test, __pyx_v_path, (&__pyx_v_self->state)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 763, __pyx_L1_error)
+  __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_make_accuracy_plots(__pyx_v_self->ptr->epoch_train, __pyx_v_self->ptr->epoch_valid, __pyx_v_self->ptr->epoch_test, __pyx_v_path, (&__pyx_v_self->state)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 766, __pyx_L1_error)
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":764
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":767
  *         make_mass_plots(self.ptr.epoch_train, self.ptr.epoch_valid, self.ptr.epoch_test, path)
  *         make_accuracy_plots(self.ptr.epoch_train, self.ptr.epoch_valid, self.ptr.epoch_test, path, &self.state)
  *         make_loss_plots(self.ptr.epoch_train, self.ptr.epoch_valid, self.ptr.epoch_test, path, &self.state)             # <<<<<<<<<<<<<<
  *         make_roc_plots(self.ptr.epoch_train, self.ptr.epoch_valid, self.ptr.epoch_test, path, &self.state)
  *         make_nodes(self.ptr.epoch_train, self.ptr.epoch_valid, self.ptr.epoch_test, path)
  */
-  __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_make_loss_plots(__pyx_v_self->ptr->epoch_train, __pyx_v_self->ptr->epoch_valid, __pyx_v_self->ptr->epoch_test, __pyx_v_path, (&__pyx_v_self->state)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 764, __pyx_L1_error)
+  __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_make_loss_plots(__pyx_v_self->ptr->epoch_train, __pyx_v_self->ptr->epoch_valid, __pyx_v_self->ptr->epoch_test, __pyx_v_path, (&__pyx_v_self->state)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 767, __pyx_L1_error)
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":765
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":768
  *         make_accuracy_plots(self.ptr.epoch_train, self.ptr.epoch_valid, self.ptr.epoch_test, path, &self.state)
  *         make_loss_plots(self.ptr.epoch_train, self.ptr.epoch_valid, self.ptr.epoch_test, path, &self.state)
  *         make_roc_plots(self.ptr.epoch_train, self.ptr.epoch_valid, self.ptr.epoch_test, path, &self.state)             # <<<<<<<<<<<<<<
  *         make_nodes(self.ptr.epoch_train, self.ptr.epoch_valid, self.ptr.epoch_test, path)
  * 
  */
-  __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_make_roc_plots(__pyx_v_self->ptr->epoch_train, __pyx_v_self->ptr->epoch_valid, __pyx_v_self->ptr->epoch_test, __pyx_v_path, (&__pyx_v_self->state)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 765, __pyx_L1_error)
+  __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_make_roc_plots(__pyx_v_self->ptr->epoch_train, __pyx_v_self->ptr->epoch_valid, __pyx_v_self->ptr->epoch_test, __pyx_v_path, (&__pyx_v_self->state)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 768, __pyx_L1_error)
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":766
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":769
  *         make_loss_plots(self.ptr.epoch_train, self.ptr.epoch_valid, self.ptr.epoch_test, path, &self.state)
  *         make_roc_plots(self.ptr.epoch_train, self.ptr.epoch_valid, self.ptr.epoch_test, path, &self.state)
  *         make_nodes(self.ptr.epoch_train, self.ptr.epoch_valid, self.ptr.epoch_test, path)             # <<<<<<<<<<<<<<
  * 
  *     cpdef Purge(self):
  */
-  __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_make_nodes(__pyx_v_self->ptr->epoch_train, __pyx_v_self->ptr->epoch_valid, __pyx_v_self->ptr->epoch_test, __pyx_v_path); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 766, __pyx_L1_error)
+  __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_make_nodes(__pyx_v_self->ptr->epoch_train, __pyx_v_self->ptr->epoch_valid, __pyx_v_self->ptr->epoch_test, __pyx_v_path); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 769, __pyx_L1_error)
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":761
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":764
  * 
  * 
  *     cpdef BuildPlots(self, int epoch, str path):             # <<<<<<<<<<<<<<
  *         make_mass_plots(self.ptr.epoch_train, self.ptr.epoch_valid, self.ptr.epoch_test, path)
  *         make_accuracy_plots(self.ptr.epoch_train, self.ptr.epoch_valid, self.ptr.epoch_test, path, &self.state)
  */
 
@@ -42661,57 +42679,57 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_epoch_2)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 761, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 764, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_path)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 761, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 764, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("BuildPlots", 1, 2, 2, 1); __PYX_ERR(0, 761, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("BuildPlots", 1, 2, 2, 1); __PYX_ERR(0, 764, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "BuildPlots") < 0)) __PYX_ERR(0, 761, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "BuildPlots") < 0)) __PYX_ERR(0, 764, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 2)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
-    __pyx_v_epoch = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_epoch == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 761, __pyx_L3_error)
+    __pyx_v_epoch = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_epoch == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 764, __pyx_L3_error)
     __pyx_v_path = ((PyObject*)values[1]);
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("BuildPlots", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 761, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("BuildPlots", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 764, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("AnalysisG._cmodules.cOptimizer.cOptimizer.BuildPlots", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_path), (&PyUnicode_Type), 1, "path", 1))) __PYX_ERR(0, 761, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_path), (&PyUnicode_Type), 1, "path", 1))) __PYX_ERR(0, 764, __pyx_L1_error)
   __pyx_r = __pyx_pf_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_30BuildPlots(((struct __pyx_obj_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer *)__pyx_v_self), __pyx_v_epoch, __pyx_v_path);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -42730,15 +42748,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("BuildPlots", 1);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_BuildPlots(__pyx_v_self, __pyx_v_epoch, __pyx_v_path, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 761, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_BuildPlots(__pyx_v_self, __pyx_v_epoch, __pyx_v_path, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 764, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -42747,15 +42765,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/cmodules/cyincludes/cyoptimizer.pyx":768
+/* "src/cmodules/cyincludes/cyoptimizer.pyx":771
  *         make_nodes(self.ptr.epoch_train, self.ptr.epoch_valid, self.ptr.epoch_test, path)
  * 
  *     cpdef Purge(self):             # <<<<<<<<<<<<<<
  *         cdef pair[int, CyEpoch*] itr
  *         for itr in self.ptr.epoch_train: itr.second.purge()
  */
 
@@ -42786,15 +42804,15 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || __Pyx_PyType_HasFeature(Py_TYPE(((PyObject *)__pyx_v_self)), (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_typedict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_Purge); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 768, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_Purge); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 771, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!__Pyx_IsSameCFunction(__pyx_t_1, (void*) __pyx_pw_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_33Purge)) {
         __Pyx_XDECREF(__pyx_r);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         __pyx_t_5 = 0;
         #if CYTHON_UNPACK_METHODS
@@ -42809,15 +42827,15 @@
           }
         }
         #endif
         {
           PyObject *__pyx_callargs[2] = {__pyx_t_4, NULL};
           __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 0+__pyx_t_5);
           __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-          if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 768, __pyx_L1_error)
+          if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 771, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         }
         __pyx_r = __pyx_t_2;
         __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
@@ -42831,15 +42849,15 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":770
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":773
  *     cpdef Purge(self):
  *         cdef pair[int, CyEpoch*] itr
  *         for itr in self.ptr.epoch_train: itr.second.purge()             # <<<<<<<<<<<<<<
  *         for itr in self.ptr.epoch_valid: itr.second.purge()
  *         for itr in self.ptr.epoch_test:  itr.second.purge()
  */
   __pyx_t_6 = __pyx_v_self->ptr->epoch_train.begin();
@@ -42847,15 +42865,15 @@
     if (!(__pyx_t_6 != __pyx_v_self->ptr->epoch_train.end())) break;
     __pyx_t_7 = *__pyx_t_6;
     ++__pyx_t_6;
     __pyx_v_itr = __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_7);
     __pyx_v_itr.second->purge();
   }
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":771
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":774
  *         cdef pair[int, CyEpoch*] itr
  *         for itr in self.ptr.epoch_train: itr.second.purge()
  *         for itr in self.ptr.epoch_valid: itr.second.purge()             # <<<<<<<<<<<<<<
  *         for itr in self.ptr.epoch_test:  itr.second.purge()
  * 
  */
   __pyx_t_6 = __pyx_v_self->ptr->epoch_valid.begin();
@@ -42863,15 +42881,15 @@
     if (!(__pyx_t_6 != __pyx_v_self->ptr->epoch_valid.end())) break;
     __pyx_t_7 = *__pyx_t_6;
     ++__pyx_t_6;
     __pyx_v_itr = __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_7);
     __pyx_v_itr.second->purge();
   }
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":772
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":775
  *         for itr in self.ptr.epoch_train: itr.second.purge()
  *         for itr in self.ptr.epoch_valid: itr.second.purge()
  *         for itr in self.ptr.epoch_test:  itr.second.purge()             # <<<<<<<<<<<<<<
  * 
  *     cpdef SinkInjector(self, model, bar):
  */
   __pyx_t_6 = __pyx_v_self->ptr->epoch_test.begin();
@@ -42879,15 +42897,15 @@
     if (!(__pyx_t_6 != __pyx_v_self->ptr->epoch_test.end())) break;
     __pyx_t_7 = *__pyx_t_6;
     ++__pyx_t_6;
     __pyx_v_itr = __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_7);
     __pyx_v_itr.second->purge();
   }
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":768
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":771
  *         make_nodes(self.ptr.epoch_train, self.ptr.epoch_valid, self.ptr.epoch_test, path)
  * 
  *     cpdef Purge(self):             # <<<<<<<<<<<<<<
  *         cdef pair[int, CyEpoch*] itr
  *         for itr in self.ptr.epoch_train: itr.second.purge()
  */
 
@@ -42953,15 +42971,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("Purge", 1);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_Purge(__pyx_v_self, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 768, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_Purge(__pyx_v_self, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 771, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -42970,15 +42988,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/cmodules/cyincludes/cyoptimizer.pyx":774
+/* "src/cmodules/cyincludes/cyoptimizer.pyx":777
  *         for itr in self.ptr.epoch_test:  itr.second.purge()
  * 
  *     cpdef SinkInjector(self, model, bar):             # <<<<<<<<<<<<<<
  *         cdef str v
  *         cdef list g
  */
 
@@ -43062,15 +43080,15 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || __Pyx_PyType_HasFeature(Py_TYPE(((PyObject *)__pyx_v_self)), (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_typedict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_SinkInjector); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 774, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_SinkInjector); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 777, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!__Pyx_IsSameCFunction(__pyx_t_1, (void*) __pyx_pw_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_35SinkInjector)) {
         __Pyx_XDECREF(__pyx_r);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         __pyx_t_5 = 0;
         #if CYTHON_UNPACK_METHODS
@@ -43085,15 +43103,15 @@
           }
         }
         #endif
         {
           PyObject *__pyx_callargs[3] = {__pyx_t_4, __pyx_v_model, __pyx_v_bar};
           __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 2+__pyx_t_5);
           __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-          if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 774, __pyx_L1_error)
+          if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 777, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         }
         __pyx_r = __pyx_t_2;
         __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
@@ -43107,108 +43125,108 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":777
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":780
  *         cdef str v
  *         cdef list g
  *         cdef int idx = 0             # <<<<<<<<<<<<<<
  *         cdef int idy = 0
  *         cdef dict gh2
  */
   __pyx_v_idx = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":778
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":781
  *         cdef list g
  *         cdef int idx = 0
  *         cdef int idy = 0             # <<<<<<<<<<<<<<
  *         cdef dict gh2
  *         cdef dict data_e
  */
   __pyx_v_idy = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":782
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":785
  *         cdef dict data_e
  * 
  *         h5_file = None             # <<<<<<<<<<<<<<
  *         up_root = None
  *         cdef str rp = self.sampletracer.WorkingPath
  */
   __Pyx_INCREF(Py_None);
   __pyx_v_h5_file = Py_None;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":783
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":786
  * 
  *         h5_file = None
  *         up_root = None             # <<<<<<<<<<<<<<
  *         cdef str rp = self.sampletracer.WorkingPath
  *         cdef str tp = rp + "Training/" + model.RunName + "/"
  */
   __Pyx_INCREF(Py_None);
   __pyx_v_up_root = Py_None;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":784
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":787
  *         h5_file = None
  *         up_root = None
  *         cdef str rp = self.sampletracer.WorkingPath             # <<<<<<<<<<<<<<
  *         cdef str tp = rp + "Training/" + model.RunName + "/"
  *         cdef str tree = self.sampletracer.Tree
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->sampletracer, __pyx_n_s_WorkingPath); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 784, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->sampletracer, __pyx_n_s_WorkingPath); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 787, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_t_1))) __PYX_ERR(0, 784, __pyx_L1_error)
+  if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_t_1))) __PYX_ERR(0, 787, __pyx_L1_error)
   __pyx_v_rp = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":785
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":788
  *         up_root = None
  *         cdef str rp = self.sampletracer.WorkingPath
  *         cdef str tp = rp + "Training/" + model.RunName + "/"             # <<<<<<<<<<<<<<
  *         cdef str tree = self.sampletracer.Tree
  *         cdef dict gh = self.sampletracer.makehashes()["graph"]
  */
-  __pyx_t_1 = __Pyx_PyUnicode_ConcatSafe(__pyx_v_rp, __pyx_kp_u_Training); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 785, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyUnicode_ConcatSafe(__pyx_v_rp, __pyx_kp_u_Training); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 788, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_model, __pyx_n_s_RunName); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 785, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_model, __pyx_n_s_RunName); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 788, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyNumber_Add(__pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 785, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Add(__pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 788, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyNumber_Add(__pyx_t_3, __pyx_kp_u__62); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 785, __pyx_L1_error)
+  __pyx_t_2 = PyNumber_Add(__pyx_t_3, __pyx_kp_u__62); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 788, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (!(likely(PyUnicode_CheckExact(__pyx_t_2))||((__pyx_t_2) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_t_2))) __PYX_ERR(0, 785, __pyx_L1_error)
+  if (!(likely(PyUnicode_CheckExact(__pyx_t_2))||((__pyx_t_2) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_t_2))) __PYX_ERR(0, 788, __pyx_L1_error)
   __pyx_v_tp = ((PyObject*)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":786
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":789
  *         cdef str rp = self.sampletracer.WorkingPath
  *         cdef str tp = rp + "Training/" + model.RunName + "/"
  *         cdef str tree = self.sampletracer.Tree             # <<<<<<<<<<<<<<
  *         cdef dict gh = self.sampletracer.makehashes()["graph"]
  *         cdef list roots = [tp + v.replace(rp + "GraphCache/", "") for v in gh]
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->sampletracer, __pyx_n_s_Tree); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 786, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->sampletracer, __pyx_n_s_Tree); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 789, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (!(likely(PyUnicode_CheckExact(__pyx_t_2))||((__pyx_t_2) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_t_2))) __PYX_ERR(0, 786, __pyx_L1_error)
+  if (!(likely(PyUnicode_CheckExact(__pyx_t_2))||((__pyx_t_2) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_t_2))) __PYX_ERR(0, 789, __pyx_L1_error)
   __pyx_v_tree = ((PyObject*)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":787
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":790
  *         cdef str tp = rp + "Training/" + model.RunName + "/"
  *         cdef str tree = self.sampletracer.Tree
  *         cdef dict gh = self.sampletracer.makehashes()["graph"]             # <<<<<<<<<<<<<<
  *         cdef list roots = [tp + v.replace(rp + "GraphCache/", "") for v in gh]
  *         cdef vector[int] indx = [0] + [len(g) for g in gh.values()]
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->sampletracer, __pyx_n_s_makehashes); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 787, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->sampletracer, __pyx_n_s_makehashes); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 790, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_1 = NULL;
   __pyx_t_5 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_1)) {
@@ -43220,231 +43238,231 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_1, NULL};
     __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 0+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 787, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 790, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
-  __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_t_2, __pyx_n_u_graph); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 787, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_t_2, __pyx_n_u_graph); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 790, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (!(likely(PyDict_CheckExact(__pyx_t_3))||((__pyx_t_3) == Py_None) || __Pyx_RaiseUnexpectedTypeError("dict", __pyx_t_3))) __PYX_ERR(0, 787, __pyx_L1_error)
+  if (!(likely(PyDict_CheckExact(__pyx_t_3))||((__pyx_t_3) == Py_None) || __Pyx_RaiseUnexpectedTypeError("dict", __pyx_t_3))) __PYX_ERR(0, 790, __pyx_L1_error)
   __pyx_v_gh = ((PyObject*)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":788
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":791
  *         cdef str tree = self.sampletracer.Tree
  *         cdef dict gh = self.sampletracer.makehashes()["graph"]
  *         cdef list roots = [tp + v.replace(rp + "GraphCache/", "") for v in gh]             # <<<<<<<<<<<<<<
  *         cdef vector[int] indx = [0] + [len(g) for g in gh.values()]
  *         self.UseAllHashes(sum(gh.values(), []))
  */
   { /* enter inner scope */
-    __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 788, __pyx_L5_error)
+    __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 791, __pyx_L5_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_6 = 0;
     if (unlikely(__pyx_v_gh == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-      __PYX_ERR(0, 788, __pyx_L5_error)
+      __PYX_ERR(0, 791, __pyx_L5_error)
     }
-    __pyx_t_1 = __Pyx_dict_iterator(__pyx_v_gh, 1, ((PyObject *)NULL), (&__pyx_t_7), (&__pyx_t_5)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 788, __pyx_L5_error)
+    __pyx_t_1 = __Pyx_dict_iterator(__pyx_v_gh, 1, ((PyObject *)NULL), (&__pyx_t_7), (&__pyx_t_5)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 791, __pyx_L5_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_XDECREF(__pyx_t_2);
     __pyx_t_2 = __pyx_t_1;
     __pyx_t_1 = 0;
     while (1) {
       __pyx_t_8 = __Pyx_dict_iter_next(__pyx_t_2, __pyx_t_7, &__pyx_t_6, &__pyx_t_1, NULL, NULL, __pyx_t_5);
       if (unlikely(__pyx_t_8 == 0)) break;
-      if (unlikely(__pyx_t_8 == -1)) __PYX_ERR(0, 788, __pyx_L5_error)
+      if (unlikely(__pyx_t_8 == -1)) __PYX_ERR(0, 791, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_1);
-      if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_t_1))) __PYX_ERR(0, 788, __pyx_L5_error)
+      if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_t_1))) __PYX_ERR(0, 791, __pyx_L5_error)
       __Pyx_XDECREF_SET(__pyx_9genexpr11__pyx_v_v, ((PyObject*)__pyx_t_1));
       __pyx_t_1 = 0;
       if (unlikely(__pyx_9genexpr11__pyx_v_v == Py_None)) {
         PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "replace");
-        __PYX_ERR(0, 788, __pyx_L5_error)
+        __PYX_ERR(0, 791, __pyx_L5_error)
       }
-      __pyx_t_1 = __Pyx_PyUnicode_ConcatSafe(__pyx_v_rp, __pyx_kp_u_GraphCache); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 788, __pyx_L5_error)
+      __pyx_t_1 = __Pyx_PyUnicode_ConcatSafe(__pyx_v_rp, __pyx_kp_u_GraphCache); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 791, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_4 = PyUnicode_Replace(__pyx_9genexpr11__pyx_v_v, __pyx_t_1, __pyx_kp_u__61, -1L); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 788, __pyx_L5_error)
+      __pyx_t_4 = PyUnicode_Replace(__pyx_9genexpr11__pyx_v_v, __pyx_t_1, __pyx_kp_u__61, -1L); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 791, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_t_1 = __Pyx_PyUnicode_ConcatSafe(__pyx_v_tp, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 788, __pyx_L5_error)
+      __pyx_t_1 = __Pyx_PyUnicode_ConcatSafe(__pyx_v_tp, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 791, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_3, (PyObject*)__pyx_t_1))) __PYX_ERR(0, 788, __pyx_L5_error)
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_3, (PyObject*)__pyx_t_1))) __PYX_ERR(0, 791, __pyx_L5_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     }
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_9genexpr11__pyx_v_v); __pyx_9genexpr11__pyx_v_v = 0;
     goto __pyx_L8_exit_scope;
     __pyx_L5_error:;
     __Pyx_XDECREF(__pyx_9genexpr11__pyx_v_v); __pyx_9genexpr11__pyx_v_v = 0;
     goto __pyx_L1_error;
     __pyx_L8_exit_scope:;
   } /* exit inner scope */
   __pyx_v_roots = ((PyObject*)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":789
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":792
  *         cdef dict gh = self.sampletracer.makehashes()["graph"]
  *         cdef list roots = [tp + v.replace(rp + "GraphCache/", "") for v in gh]
  *         cdef vector[int] indx = [0] + [len(g) for g in gh.values()]             # <<<<<<<<<<<<<<
  *         self.UseAllHashes(sum(gh.values(), []))
  * 
  */
-  __pyx_t_3 = PyList_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 789, __pyx_L1_error)
+  __pyx_t_3 = PyList_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 792, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_int_0);
   __Pyx_GIVEREF(__pyx_int_0);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 0, __pyx_int_0)) __PYX_ERR(0, 789, __pyx_L1_error);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 0, __pyx_int_0)) __PYX_ERR(0, 792, __pyx_L1_error);
   { /* enter inner scope */
-    __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 789, __pyx_L11_error)
+    __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 792, __pyx_L11_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_7 = 0;
     if (unlikely(__pyx_v_gh == Py_None)) {
       PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "values");
-      __PYX_ERR(0, 789, __pyx_L11_error)
+      __PYX_ERR(0, 792, __pyx_L11_error)
     }
-    __pyx_t_4 = __Pyx_dict_iterator(__pyx_v_gh, 1, __pyx_n_s_values, (&__pyx_t_6), (&__pyx_t_5)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 789, __pyx_L11_error)
+    __pyx_t_4 = __Pyx_dict_iterator(__pyx_v_gh, 1, __pyx_n_s_values, (&__pyx_t_6), (&__pyx_t_5)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 792, __pyx_L11_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_1);
     __pyx_t_1 = __pyx_t_4;
     __pyx_t_4 = 0;
     while (1) {
       __pyx_t_8 = __Pyx_dict_iter_next(__pyx_t_1, __pyx_t_6, &__pyx_t_7, NULL, &__pyx_t_4, NULL, __pyx_t_5);
       if (unlikely(__pyx_t_8 == 0)) break;
-      if (unlikely(__pyx_t_8 == -1)) __PYX_ERR(0, 789, __pyx_L11_error)
+      if (unlikely(__pyx_t_8 == -1)) __PYX_ERR(0, 792, __pyx_L11_error)
       __Pyx_GOTREF(__pyx_t_4);
-      if (!(likely(PyList_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None) || __Pyx_RaiseUnexpectedTypeError("list", __pyx_t_4))) __PYX_ERR(0, 789, __pyx_L11_error)
+      if (!(likely(PyList_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None) || __Pyx_RaiseUnexpectedTypeError("list", __pyx_t_4))) __PYX_ERR(0, 792, __pyx_L11_error)
       __Pyx_XDECREF_SET(__pyx_9genexpr12__pyx_v_g, ((PyObject*)__pyx_t_4));
       __pyx_t_4 = 0;
       if (unlikely(__pyx_9genexpr12__pyx_v_g == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-        __PYX_ERR(0, 789, __pyx_L11_error)
+        __PYX_ERR(0, 792, __pyx_L11_error)
       }
-      __pyx_t_9 = __Pyx_PyList_GET_SIZE(__pyx_9genexpr12__pyx_v_g); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 789, __pyx_L11_error)
-      __pyx_t_4 = PyInt_FromSsize_t(__pyx_t_9); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 789, __pyx_L11_error)
+      __pyx_t_9 = __Pyx_PyList_GET_SIZE(__pyx_9genexpr12__pyx_v_g); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 792, __pyx_L11_error)
+      __pyx_t_4 = PyInt_FromSsize_t(__pyx_t_9); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 792, __pyx_L11_error)
       __Pyx_GOTREF(__pyx_t_4);
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_2, (PyObject*)__pyx_t_4))) __PYX_ERR(0, 789, __pyx_L11_error)
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_2, (PyObject*)__pyx_t_4))) __PYX_ERR(0, 792, __pyx_L11_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     }
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_9genexpr12__pyx_v_g); __pyx_9genexpr12__pyx_v_g = 0;
     goto __pyx_L14_exit_scope;
     __pyx_L11_error:;
     __Pyx_XDECREF(__pyx_9genexpr12__pyx_v_g); __pyx_9genexpr12__pyx_v_g = 0;
     goto __pyx_L1_error;
     __pyx_L14_exit_scope:;
   } /* exit inner scope */
-  __pyx_t_1 = PyNumber_Add(__pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 789, __pyx_L1_error)
+  __pyx_t_1 = PyNumber_Add(__pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 792, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_10 = __pyx_convert_vector_from_py_int(__pyx_t_1); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 789, __pyx_L1_error)
+  __pyx_t_10 = __pyx_convert_vector_from_py_int(__pyx_t_1); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 792, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_indx = __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_10);
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":790
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":793
  *         cdef list roots = [tp + v.replace(rp + "GraphCache/", "") for v in gh]
  *         cdef vector[int] indx = [0] + [len(g) for g in gh.values()]
  *         self.UseAllHashes(sum(gh.values(), []))             # <<<<<<<<<<<<<<
  * 
  *         self._train = True
  */
   if (unlikely(__pyx_v_gh == Py_None)) {
     PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "values");
-    __PYX_ERR(0, 790, __pyx_L1_error)
+    __PYX_ERR(0, 793, __pyx_L1_error)
   }
-  __pyx_t_1 = __Pyx_PyDict_Values(__pyx_v_gh); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 790, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_Values(__pyx_v_gh); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 793, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 790, __pyx_L1_error)
+  __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 793, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 790, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 793, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_1);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1)) __PYX_ERR(0, 790, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1)) __PYX_ERR(0, 793, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_2);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_2)) __PYX_ERR(0, 790, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_2)) __PYX_ERR(0, 793, __pyx_L1_error);
   __pyx_t_1 = 0;
   __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_sum, __pyx_t_3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 790, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_sum, __pyx_t_3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 793, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (!(likely(PyList_CheckExact(__pyx_t_2))||((__pyx_t_2) == Py_None) || __Pyx_RaiseUnexpectedTypeError("list", __pyx_t_2))) __PYX_ERR(0, 790, __pyx_L1_error)
-  __pyx_t_3 = ((struct __pyx_vtabstruct_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer *)__pyx_v_self->__pyx_vtab)->UseAllHashes(__pyx_v_self, ((PyObject*)__pyx_t_2), 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 790, __pyx_L1_error)
+  if (!(likely(PyList_CheckExact(__pyx_t_2))||((__pyx_t_2) == Py_None) || __Pyx_RaiseUnexpectedTypeError("list", __pyx_t_2))) __PYX_ERR(0, 793, __pyx_L1_error)
+  __pyx_t_3 = ((struct __pyx_vtabstruct_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer *)__pyx_v_self->__pyx_vtab)->UseAllHashes(__pyx_v_self, ((PyObject*)__pyx_t_2), 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 793, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":792
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":795
  *         self.UseAllHashes(sum(gh.values(), []))
  * 
  *         self._train = True             # <<<<<<<<<<<<<<
  *         self._val   = False
  *         self._test  = False
  */
   __pyx_v_self->_train = 1;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":793
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":796
  * 
  *         self._train = True
  *         self._val   = False             # <<<<<<<<<<<<<<
  *         self._test  = False
  * 
  */
   __pyx_v_self->_val = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":794
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":797
  *         self._train = True
  *         self._val   = False
  *         self._test  = False             # <<<<<<<<<<<<<<
  * 
  *         cdef vector[string] hashes
  */
   __pyx_v_self->_test = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":797
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":800
  * 
  *         cdef vector[string] hashes
  *         cdef DataLoader loader = self.data.set_batch(1, 1, b"train")             # <<<<<<<<<<<<<<
  *         bar.total = len(loader)
  *         bar.refresh()
  */
-  __pyx_t_11 = __pyx_convert_string_from_py_6libcpp_6string_std__in_string(__pyx_n_b_train); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 797, __pyx_L1_error)
-  __pyx_t_3 = ((PyObject *)((struct __pyx_vtabstruct_9AnalysisG_9_cmodules_10cOptimizer_DataLoader *)__pyx_v_self->data->__pyx_vtab)->set_batch(__pyx_v_self->data, 1, 1, __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_11))); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 797, __pyx_L1_error)
+  __pyx_t_11 = __pyx_convert_string_from_py_6libcpp_6string_std__in_string(__pyx_n_b_train); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 800, __pyx_L1_error)
+  __pyx_t_3 = ((PyObject *)((struct __pyx_vtabstruct_9AnalysisG_9_cmodules_10cOptimizer_DataLoader *)__pyx_v_self->data->__pyx_vtab)->set_batch(__pyx_v_self->data, 1, 1, __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_11))); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 800, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_v_loader = ((struct __pyx_obj_9AnalysisG_9_cmodules_10cOptimizer_DataLoader *)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":798
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":801
  *         cdef vector[string] hashes
  *         cdef DataLoader loader = self.data.set_batch(1, 1, b"train")
  *         bar.total = len(loader)             # <<<<<<<<<<<<<<
  *         bar.refresh()
  * 
  */
-  __pyx_t_6 = PyObject_Length(((PyObject *)__pyx_v_loader)); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 798, __pyx_L1_error)
-  __pyx_t_3 = PyInt_FromSsize_t(__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 798, __pyx_L1_error)
+  __pyx_t_6 = PyObject_Length(((PyObject *)__pyx_v_loader)); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 801, __pyx_L1_error)
+  __pyx_t_3 = PyInt_FromSsize_t(__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 801, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_bar, __pyx_n_s_total, __pyx_t_3) < 0) __PYX_ERR(0, 798, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_bar, __pyx_n_s_total, __pyx_t_3) < 0) __PYX_ERR(0, 801, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":799
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":802
  *         cdef DataLoader loader = self.data.set_batch(1, 1, b"train")
  *         bar.total = len(loader)
  *         bar.refresh()             # <<<<<<<<<<<<<<
  * 
  *         cdef int ix = 0
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_bar, __pyx_n_s_refresh); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 799, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_bar, __pyx_n_s_refresh); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 802, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_1 = NULL;
   __pyx_t_5 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_1)) {
@@ -43456,141 +43474,141 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_1, NULL};
     __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_5, 0+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 799, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 802, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":801
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":804
  *         bar.refresh()
  * 
  *         cdef int ix = 0             # <<<<<<<<<<<<<<
  *         cdef map[int, int] index_map
  *         cdef pair[int, int] index_itr
  */
   __pyx_v_ix = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":808
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":811
  *         cdef pair[string, map[int, vector[float]]] data_i
  * 
  *         for data, hashes in loader:             # <<<<<<<<<<<<<<
  *             gh = model(data)
  *             gh2 = gh.pop("graphs")[0].to_dict()
  */
   if (likely(PyList_CheckExact(((PyObject *)__pyx_v_loader))) || PyTuple_CheckExact(((PyObject *)__pyx_v_loader))) {
     __pyx_t_3 = ((PyObject *)__pyx_v_loader); __Pyx_INCREF(__pyx_t_3);
     __pyx_t_6 = 0;
     __pyx_t_12 = NULL;
   } else {
-    __pyx_t_6 = -1; __pyx_t_3 = PyObject_GetIter(((PyObject *)__pyx_v_loader)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 808, __pyx_L1_error)
+    __pyx_t_6 = -1; __pyx_t_3 = PyObject_GetIter(((PyObject *)__pyx_v_loader)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 811, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_12 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_3); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 808, __pyx_L1_error)
+    __pyx_t_12 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_3); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 811, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_12)) {
       if (likely(PyList_CheckExact(__pyx_t_3))) {
         {
           Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_3);
           #if !CYTHON_ASSUME_SAFE_MACROS
-          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 808, __pyx_L1_error)
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 811, __pyx_L1_error)
           #endif
           if (__pyx_t_6 >= __pyx_temp) break;
         }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_2 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_6); __Pyx_INCREF(__pyx_t_2); __pyx_t_6++; if (unlikely((0 < 0))) __PYX_ERR(0, 808, __pyx_L1_error)
+        __pyx_t_2 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_6); __Pyx_INCREF(__pyx_t_2); __pyx_t_6++; if (unlikely((0 < 0))) __PYX_ERR(0, 811, __pyx_L1_error)
         #else
-        __pyx_t_2 = __Pyx_PySequence_ITEM(__pyx_t_3, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 808, __pyx_L1_error)
+        __pyx_t_2 = __Pyx_PySequence_ITEM(__pyx_t_3, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 811, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         #endif
       } else {
         {
           Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_3);
           #if !CYTHON_ASSUME_SAFE_MACROS
-          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 808, __pyx_L1_error)
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 811, __pyx_L1_error)
           #endif
           if (__pyx_t_6 >= __pyx_temp) break;
         }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_6); __Pyx_INCREF(__pyx_t_2); __pyx_t_6++; if (unlikely((0 < 0))) __PYX_ERR(0, 808, __pyx_L1_error)
+        __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_6); __Pyx_INCREF(__pyx_t_2); __pyx_t_6++; if (unlikely((0 < 0))) __PYX_ERR(0, 811, __pyx_L1_error)
         #else
-        __pyx_t_2 = __Pyx_PySequence_ITEM(__pyx_t_3, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 808, __pyx_L1_error)
+        __pyx_t_2 = __Pyx_PySequence_ITEM(__pyx_t_3, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 811, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         #endif
       }
     } else {
       __pyx_t_2 = __pyx_t_12(__pyx_t_3);
       if (unlikely(!__pyx_t_2)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 808, __pyx_L1_error)
+          else __PYX_ERR(0, 811, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_2);
     }
     if ((likely(PyTuple_CheckExact(__pyx_t_2))) || (PyList_CheckExact(__pyx_t_2))) {
       PyObject* sequence = __pyx_t_2;
       Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
       if (unlikely(size != 2)) {
         if (size > 2) __Pyx_RaiseTooManyValuesError(2);
         else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-        __PYX_ERR(0, 808, __pyx_L1_error)
+        __PYX_ERR(0, 811, __pyx_L1_error)
       }
       #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
       if (likely(PyTuple_CheckExact(sequence))) {
         __pyx_t_1 = PyTuple_GET_ITEM(sequence, 0); 
         __pyx_t_4 = PyTuple_GET_ITEM(sequence, 1); 
       } else {
         __pyx_t_1 = PyList_GET_ITEM(sequence, 0); 
         __pyx_t_4 = PyList_GET_ITEM(sequence, 1); 
       }
       __Pyx_INCREF(__pyx_t_1);
       __Pyx_INCREF(__pyx_t_4);
       #else
-      __pyx_t_1 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 808, __pyx_L1_error)
+      __pyx_t_1 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 811, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_4 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 808, __pyx_L1_error)
+      __pyx_t_4 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 811, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       #endif
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     } else {
       Py_ssize_t index = -1;
-      __pyx_t_13 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 808, __pyx_L1_error)
+      __pyx_t_13 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 811, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_13);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __pyx_t_14 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_13);
       index = 0; __pyx_t_1 = __pyx_t_14(__pyx_t_13); if (unlikely(!__pyx_t_1)) goto __pyx_L17_unpacking_failed;
       __Pyx_GOTREF(__pyx_t_1);
       index = 1; __pyx_t_4 = __pyx_t_14(__pyx_t_13); if (unlikely(!__pyx_t_4)) goto __pyx_L17_unpacking_failed;
       __Pyx_GOTREF(__pyx_t_4);
-      if (__Pyx_IternextUnpackEndCheck(__pyx_t_14(__pyx_t_13), 2) < 0) __PYX_ERR(0, 808, __pyx_L1_error)
+      if (__Pyx_IternextUnpackEndCheck(__pyx_t_14(__pyx_t_13), 2) < 0) __PYX_ERR(0, 811, __pyx_L1_error)
       __pyx_t_14 = NULL;
       __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
       goto __pyx_L18_unpacking_done;
       __pyx_L17_unpacking_failed:;
       __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
       __pyx_t_14 = NULL;
       if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-      __PYX_ERR(0, 808, __pyx_L1_error)
+      __PYX_ERR(0, 811, __pyx_L1_error)
       __pyx_L18_unpacking_done:;
     }
-    __pyx_t_15 = __pyx_convert_vector_from_py_std_3a__3a_string(__pyx_t_4); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 808, __pyx_L1_error)
+    __pyx_t_15 = __pyx_convert_vector_from_py_std_3a__3a_string(__pyx_t_4); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 811, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_XDECREF_SET(__pyx_v_data, __pyx_t_1);
     __pyx_t_1 = 0;
     __pyx_v_hashes = __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_15);
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":809
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":812
  * 
  *         for data, hashes in loader:
  *             gh = model(data)             # <<<<<<<<<<<<<<
  *             gh2 = gh.pop("graphs")[0].to_dict()
  *             gh.update(gh2)
  */
     __Pyx_INCREF(__pyx_v_model);
@@ -43608,39 +43626,39 @@
       }
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_1, __pyx_v_data};
       __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
       __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 809, __pyx_L1_error)
+      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 812, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     }
-    if (!(likely(PyDict_CheckExact(__pyx_t_2))||((__pyx_t_2) == Py_None) || __Pyx_RaiseUnexpectedTypeError("dict", __pyx_t_2))) __PYX_ERR(0, 809, __pyx_L1_error)
+    if (!(likely(PyDict_CheckExact(__pyx_t_2))||((__pyx_t_2) == Py_None) || __Pyx_RaiseUnexpectedTypeError("dict", __pyx_t_2))) __PYX_ERR(0, 812, __pyx_L1_error)
     __Pyx_DECREF_SET(__pyx_v_gh, ((PyObject*)__pyx_t_2));
     __pyx_t_2 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":810
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":813
  *         for data, hashes in loader:
  *             gh = model(data)
  *             gh2 = gh.pop("graphs")[0].to_dict()             # <<<<<<<<<<<<<<
  *             gh.update(gh2)
  *             if indx[idx] == idy:
  */
     if (unlikely(__pyx_v_gh == Py_None)) {
       PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "pop");
-      __PYX_ERR(0, 810, __pyx_L1_error)
+      __PYX_ERR(0, 813, __pyx_L1_error)
     }
-    __pyx_t_4 = __Pyx_PyDict_Pop(__pyx_v_gh, __pyx_n_u_graphs, ((PyObject *)NULL)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 810, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyDict_Pop(__pyx_v_gh, __pyx_n_u_graphs, ((PyObject *)NULL)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 813, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_1 = __Pyx_GetItemInt(__pyx_t_4, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 810, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_GetItemInt(__pyx_t_4, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 813, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_to_dict); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 810, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_to_dict); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 813, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_1 = NULL;
     __pyx_t_5 = 0;
     #if CYTHON_UNPACK_METHODS
     if (likely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_4);
@@ -43653,59 +43671,59 @@
       }
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_1, NULL};
       __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_5, 0+__pyx_t_5);
       __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 810, __pyx_L1_error)
+      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 813, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     }
-    if (!(likely(PyDict_CheckExact(__pyx_t_2))||((__pyx_t_2) == Py_None) || __Pyx_RaiseUnexpectedTypeError("dict", __pyx_t_2))) __PYX_ERR(0, 810, __pyx_L1_error)
+    if (!(likely(PyDict_CheckExact(__pyx_t_2))||((__pyx_t_2) == Py_None) || __Pyx_RaiseUnexpectedTypeError("dict", __pyx_t_2))) __PYX_ERR(0, 813, __pyx_L1_error)
     __Pyx_XDECREF_SET(__pyx_v_gh2, ((PyObject*)__pyx_t_2));
     __pyx_t_2 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":811
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":814
  *             gh = model(data)
  *             gh2 = gh.pop("graphs")[0].to_dict()
  *             gh.update(gh2)             # <<<<<<<<<<<<<<
  *             if indx[idx] == idy:
  *                 v = os.path.abspath(roots[idx])
  */
-    __pyx_t_2 = __Pyx_CallUnboundCMethod1(&__pyx_umethod_PyDict_Type_update, __pyx_v_gh, __pyx_v_gh2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 811, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_CallUnboundCMethod1(&__pyx_umethod_PyDict_Type_update, __pyx_v_gh, __pyx_v_gh2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 814, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":812
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":815
  *             gh2 = gh.pop("graphs")[0].to_dict()
  *             gh.update(gh2)
  *             if indx[idx] == idy:             # <<<<<<<<<<<<<<
  *                 v = os.path.abspath(roots[idx])
  *                 try: os.makedirs("/".join(v.split("/")[:-1]))
  */
     __pyx_t_16 = ((__pyx_v_indx[__pyx_v_idx]) == __pyx_v_idy);
     if (__pyx_t_16) {
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":813
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":816
  *             gh.update(gh2)
  *             if indx[idx] == idy:
  *                 v = os.path.abspath(roots[idx])             # <<<<<<<<<<<<<<
  *                 try: os.makedirs("/".join(v.split("/")[:-1]))
  *                 except FileExistsError: pass
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_os); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 813, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_os); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 816, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_path); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 813, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_path); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 816, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_abspath); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 813, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_abspath); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 816, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_t_1 = __Pyx_GetItemInt_List(__pyx_v_roots, __pyx_v_idx, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 813, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_GetItemInt_List(__pyx_v_roots, __pyx_v_idx, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 816, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __pyx_t_13 = NULL;
       __pyx_t_5 = 0;
       #if CYTHON_UNPACK_METHODS
       if (likely(PyMethod_Check(__pyx_t_4))) {
         __pyx_t_13 = PyMethod_GET_SELF(__pyx_t_4);
         if (likely(__pyx_t_13)) {
@@ -43718,52 +43736,52 @@
       }
       #endif
       {
         PyObject *__pyx_callargs[2] = {__pyx_t_13, __pyx_t_1};
         __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
         __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 813, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 816, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       }
-      if (!(likely(PyUnicode_CheckExact(__pyx_t_2))||((__pyx_t_2) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_t_2))) __PYX_ERR(0, 813, __pyx_L1_error)
+      if (!(likely(PyUnicode_CheckExact(__pyx_t_2))||((__pyx_t_2) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_t_2))) __PYX_ERR(0, 816, __pyx_L1_error)
       __Pyx_XDECREF_SET(__pyx_v_v, ((PyObject*)__pyx_t_2));
       __pyx_t_2 = 0;
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":814
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":817
  *             if indx[idx] == idy:
  *                 v = os.path.abspath(roots[idx])
  *                 try: os.makedirs("/".join(v.split("/")[:-1]))             # <<<<<<<<<<<<<<
  *                 except FileExistsError: pass
  *                 if h5_file is not None: h5_file.close()
  */
       {
         __Pyx_PyThreadState_declare
         __Pyx_PyThreadState_assign
         __Pyx_ExceptionSave(&__pyx_t_17, &__pyx_t_18, &__pyx_t_19);
         __Pyx_XGOTREF(__pyx_t_17);
         __Pyx_XGOTREF(__pyx_t_18);
         __Pyx_XGOTREF(__pyx_t_19);
         /*try:*/ {
-          __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_os); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 814, __pyx_L20_error)
+          __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_os); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 817, __pyx_L20_error)
           __Pyx_GOTREF(__pyx_t_4);
-          __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_makedirs); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 814, __pyx_L20_error)
+          __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_makedirs); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 817, __pyx_L20_error)
           __Pyx_GOTREF(__pyx_t_1);
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
           if (unlikely(__pyx_v_v == Py_None)) {
             PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "split");
-            __PYX_ERR(0, 814, __pyx_L20_error)
+            __PYX_ERR(0, 817, __pyx_L20_error)
           }
-          __pyx_t_4 = PyUnicode_Split(__pyx_v_v, __Pyx_NoneAsNull(__pyx_kp_u__62), -1L); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 814, __pyx_L20_error)
+          __pyx_t_4 = PyUnicode_Split(__pyx_v_v, __Pyx_NoneAsNull(__pyx_kp_u__62), -1L); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 817, __pyx_L20_error)
           __Pyx_GOTREF(__pyx_t_4);
-          __pyx_t_13 = __Pyx_PyObject_GetSlice(__pyx_t_4, 0, -1L, NULL, NULL, &__pyx_slice__67, 0, 1, 1); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 814, __pyx_L20_error)
+          __pyx_t_13 = __Pyx_PyObject_GetSlice(__pyx_t_4, 0, -1L, NULL, NULL, &__pyx_slice__67, 0, 1, 1); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 817, __pyx_L20_error)
           __Pyx_GOTREF(__pyx_t_13);
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-          __pyx_t_4 = PyUnicode_Join(__pyx_kp_u__62, __pyx_t_13); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 814, __pyx_L20_error)
+          __pyx_t_4 = PyUnicode_Join(__pyx_kp_u__62, __pyx_t_13); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 817, __pyx_L20_error)
           __Pyx_GOTREF(__pyx_t_4);
           __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
           __pyx_t_13 = NULL;
           __pyx_t_5 = 0;
           #if CYTHON_UNPACK_METHODS
           if (unlikely(PyMethod_Check(__pyx_t_1))) {
             __pyx_t_13 = PyMethod_GET_SELF(__pyx_t_1);
@@ -43777,15 +43795,15 @@
           }
           #endif
           {
             PyObject *__pyx_callargs[2] = {__pyx_t_13, __pyx_t_4};
             __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
             __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
             __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-            if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 814, __pyx_L20_error)
+            if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 817, __pyx_L20_error)
             __Pyx_GOTREF(__pyx_t_2);
             __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
           }
           __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         }
         __Pyx_XDECREF(__pyx_t_17); __pyx_t_17 = 0;
         __Pyx_XDECREF(__pyx_t_18); __pyx_t_18 = 0;
@@ -43793,35 +43811,35 @@
         goto __pyx_L27_try_end;
         __pyx_L20_error:;
         __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
         __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-        /* "src/cmodules/cyincludes/cyoptimizer.pyx":815
+        /* "src/cmodules/cyincludes/cyoptimizer.pyx":818
  *                 v = os.path.abspath(roots[idx])
  *                 try: os.makedirs("/".join(v.split("/")[:-1]))
  *                 except FileExistsError: pass             # <<<<<<<<<<<<<<
  *                 if h5_file is not None: h5_file.close()
  *                 h5_file = h5py.File(v, "w")
  */
         __Pyx_ErrFetch(&__pyx_t_2, &__pyx_t_1, &__pyx_t_4);
-        __Pyx_GetModuleGlobalName(__pyx_t_13, __pyx_n_s_FileExistsError); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 815, __pyx_L22_except_error)
+        __Pyx_GetModuleGlobalName(__pyx_t_13, __pyx_n_s_FileExistsError); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 818, __pyx_L22_except_error)
         __Pyx_GOTREF(__pyx_t_13);
         __pyx_t_5 = __Pyx_PyErr_GivenExceptionMatches(__pyx_t_2, __pyx_t_13);
         __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
         __Pyx_ErrRestore(__pyx_t_2, __pyx_t_1, __pyx_t_4);
         __pyx_t_2 = 0; __pyx_t_1 = 0; __pyx_t_4 = 0;
         if (__pyx_t_5) {
           __Pyx_ErrRestore(0,0,0);
           goto __pyx_L21_exception_handled;
         }
         goto __pyx_L22_except_error;
 
-        /* "src/cmodules/cyincludes/cyoptimizer.pyx":814
+        /* "src/cmodules/cyincludes/cyoptimizer.pyx":817
  *             if indx[idx] == idy:
  *                 v = os.path.abspath(roots[idx])
  *                 try: os.makedirs("/".join(v.split("/")[:-1]))             # <<<<<<<<<<<<<<
  *                 except FileExistsError: pass
  *                 if h5_file is not None: h5_file.close()
  */
         __pyx_L22_except_error:;
@@ -43834,24 +43852,24 @@
         __Pyx_XGIVEREF(__pyx_t_17);
         __Pyx_XGIVEREF(__pyx_t_18);
         __Pyx_XGIVEREF(__pyx_t_19);
         __Pyx_ExceptionReset(__pyx_t_17, __pyx_t_18, __pyx_t_19);
         __pyx_L27_try_end:;
       }
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":816
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":819
  *                 try: os.makedirs("/".join(v.split("/")[:-1]))
  *                 except FileExistsError: pass
  *                 if h5_file is not None: h5_file.close()             # <<<<<<<<<<<<<<
  *                 h5_file = h5py.File(v, "w")
  *                 if up_root is not None:
  */
       __pyx_t_16 = (__pyx_v_h5_file != Py_None);
       if (__pyx_t_16) {
-        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_h5_file, __pyx_n_s_close); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 816, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_h5_file, __pyx_n_s_close); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 819, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         __pyx_t_2 = NULL;
         __pyx_t_5 = 0;
         #if CYTHON_UNPACK_METHODS
         if (likely(PyMethod_Check(__pyx_t_1))) {
           __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_1);
           if (likely(__pyx_t_2)) {
@@ -43863,31 +43881,31 @@
           }
         }
         #endif
         {
           PyObject *__pyx_callargs[2] = {__pyx_t_2, NULL};
           __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_5, 0+__pyx_t_5);
           __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-          if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 816, __pyx_L1_error)
+          if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 819, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_4);
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         }
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       }
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":817
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":820
  *                 except FileExistsError: pass
  *                 if h5_file is not None: h5_file.close()
  *                 h5_file = h5py.File(v, "w")             # <<<<<<<<<<<<<<
  *                 if up_root is not None:
  *                     put  = {env(data_i.first) : awkward.Array([data_i.second[index_itr.first] for index_itr in index_map]) for data_i in data_map}
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_h5py); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 817, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_h5py); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 820, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_File); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 817, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_File); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 820, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_t_1 = NULL;
       __pyx_t_5 = 0;
       #if CYTHON_UNPACK_METHODS
       if (unlikely(PyMethod_Check(__pyx_t_2))) {
         __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_2);
@@ -43900,66 +43918,66 @@
         }
       }
       #endif
       {
         PyObject *__pyx_callargs[3] = {__pyx_t_1, __pyx_v_v, __pyx_n_u_w};
         __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_5, 2+__pyx_t_5);
         __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 817, __pyx_L1_error)
+        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 820, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       }
       __Pyx_DECREF_SET(__pyx_v_h5_file, __pyx_t_4);
       __pyx_t_4 = 0;
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":818
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":821
  *                 if h5_file is not None: h5_file.close()
  *                 h5_file = h5py.File(v, "w")
  *                 if up_root is not None:             # <<<<<<<<<<<<<<
  *                     put  = {env(data_i.first) : awkward.Array([data_i.second[index_itr.first] for index_itr in index_map]) for data_i in data_map}
  *                     put |= {"event_index" : awkward.Array([index_itr.first for index_itr in index_map])}
  */
       __pyx_t_16 = (__pyx_v_up_root != Py_None);
       if (__pyx_t_16) {
 
-        /* "src/cmodules/cyincludes/cyoptimizer.pyx":819
+        /* "src/cmodules/cyincludes/cyoptimizer.pyx":822
  *                 h5_file = h5py.File(v, "w")
  *                 if up_root is not None:
  *                     put  = {env(data_i.first) : awkward.Array([data_i.second[index_itr.first] for index_itr in index_map]) for data_i in data_map}             # <<<<<<<<<<<<<<
  *                     put |= {"event_index" : awkward.Array([index_itr.first for index_itr in index_map])}
  *                     up_root[tree] = put
  */
         { /* enter inner scope */
-          __pyx_t_4 = PyDict_New(); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 819, __pyx_L1_error)
+          __pyx_t_4 = PyDict_New(); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 822, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_4);
           __pyx_t_20 = __pyx_v_data_map.begin();
           for (;;) {
             if (!(__pyx_t_20 != __pyx_v_data_map.end())) break;
             __pyx_t_21 = *__pyx_t_20;
             ++__pyx_t_20;
             __pyx_9genexpr13__pyx_v_data_i = __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_21);
-            __pyx_t_2 = __pyx_f_7cytools_env(__pyx_9genexpr13__pyx_v_data_i.first); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 819, __pyx_L1_error)
+            __pyx_t_2 = __pyx_f_7cytools_env(__pyx_9genexpr13__pyx_v_data_i.first); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 822, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_2);
-            __Pyx_GetModuleGlobalName(__pyx_t_13, __pyx_n_s_awkward); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 819, __pyx_L1_error)
+            __Pyx_GetModuleGlobalName(__pyx_t_13, __pyx_n_s_awkward); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 822, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_13);
-            __pyx_t_22 = __Pyx_PyObject_GetAttrStr(__pyx_t_13, __pyx_n_s_Array); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 819, __pyx_L1_error)
+            __pyx_t_22 = __Pyx_PyObject_GetAttrStr(__pyx_t_13, __pyx_n_s_Array); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 822, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_22);
             __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
             { /* enter inner scope */
-              __pyx_t_13 = PyList_New(0); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 819, __pyx_L1_error)
+              __pyx_t_13 = PyList_New(0); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 822, __pyx_L1_error)
               __Pyx_GOTREF(__pyx_t_13);
               __pyx_t_23 = __pyx_v_index_map.begin();
               for (;;) {
                 if (!(__pyx_t_23 != __pyx_v_index_map.end())) break;
                 __pyx_t_24 = *__pyx_t_23;
                 ++__pyx_t_23;
                 __pyx_9genexpr14__pyx_v_index_itr = __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_24);
-                __pyx_t_25 = __pyx_convert_vector_to_py_float((__pyx_9genexpr13__pyx_v_data_i.second[__pyx_9genexpr14__pyx_v_index_itr.first])); if (unlikely(!__pyx_t_25)) __PYX_ERR(0, 819, __pyx_L1_error)
+                __pyx_t_25 = __pyx_convert_vector_to_py_float((__pyx_9genexpr13__pyx_v_data_i.second[__pyx_9genexpr14__pyx_v_index_itr.first])); if (unlikely(!__pyx_t_25)) __PYX_ERR(0, 822, __pyx_L1_error)
                 __Pyx_GOTREF(__pyx_t_25);
-                if (unlikely(__Pyx_ListComp_Append(__pyx_t_13, (PyObject*)__pyx_t_25))) __PYX_ERR(0, 819, __pyx_L1_error)
+                if (unlikely(__Pyx_ListComp_Append(__pyx_t_13, (PyObject*)__pyx_t_25))) __PYX_ERR(0, 822, __pyx_L1_error)
                 __Pyx_DECREF(__pyx_t_25); __pyx_t_25 = 0;
               }
             } /* exit inner scope */
             __pyx_t_25 = NULL;
             __pyx_t_5 = 0;
             #if CYTHON_UNPACK_METHODS
             if (unlikely(PyMethod_Check(__pyx_t_22))) {
@@ -43974,52 +43992,52 @@
             }
             #endif
             {
               PyObject *__pyx_callargs[2] = {__pyx_t_25, __pyx_t_13};
               __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_22, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
               __Pyx_XDECREF(__pyx_t_25); __pyx_t_25 = 0;
               __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
-              if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 819, __pyx_L1_error)
+              if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 822, __pyx_L1_error)
               __Pyx_GOTREF(__pyx_t_1);
               __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
             }
-            if (unlikely(PyDict_SetItem(__pyx_t_4, (PyObject*)__pyx_t_2, (PyObject*)__pyx_t_1))) __PYX_ERR(0, 819, __pyx_L1_error)
+            if (unlikely(PyDict_SetItem(__pyx_t_4, (PyObject*)__pyx_t_2, (PyObject*)__pyx_t_1))) __PYX_ERR(0, 822, __pyx_L1_error)
             __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
             __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
           }
         } /* exit inner scope */
         __Pyx_XDECREF_SET(__pyx_v_put, ((PyObject*)__pyx_t_4));
         __pyx_t_4 = 0;
 
-        /* "src/cmodules/cyincludes/cyoptimizer.pyx":820
+        /* "src/cmodules/cyincludes/cyoptimizer.pyx":823
  *                 if up_root is not None:
  *                     put  = {env(data_i.first) : awkward.Array([data_i.second[index_itr.first] for index_itr in index_map]) for data_i in data_map}
  *                     put |= {"event_index" : awkward.Array([index_itr.first for index_itr in index_map])}             # <<<<<<<<<<<<<<
  *                     up_root[tree] = put
  *                     up_root.close()
  */
-        __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 820, __pyx_L1_error)
+        __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 823, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
-        __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_awkward); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 820, __pyx_L1_error)
+        __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_awkward); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 823, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
-        __pyx_t_22 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_Array); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 820, __pyx_L1_error)
+        __pyx_t_22 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_Array); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 823, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_22);
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         { /* enter inner scope */
-          __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 820, __pyx_L1_error)
+          __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 823, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __pyx_t_23 = __pyx_v_index_map.begin();
           for (;;) {
             if (!(__pyx_t_23 != __pyx_v_index_map.end())) break;
             __pyx_t_24 = *__pyx_t_23;
             ++__pyx_t_23;
             __pyx_9genexpr15__pyx_v_index_itr = __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_24);
-            __pyx_t_13 = __Pyx_PyInt_From_int(__pyx_9genexpr15__pyx_v_index_itr.first); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 820, __pyx_L1_error)
+            __pyx_t_13 = __Pyx_PyInt_From_int(__pyx_9genexpr15__pyx_v_index_itr.first); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 823, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_13);
-            if (unlikely(__Pyx_ListComp_Append(__pyx_t_2, (PyObject*)__pyx_t_13))) __PYX_ERR(0, 820, __pyx_L1_error)
+            if (unlikely(__Pyx_ListComp_Append(__pyx_t_2, (PyObject*)__pyx_t_13))) __PYX_ERR(0, 823, __pyx_L1_error)
             __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
           }
         } /* exit inner scope */
         __pyx_t_13 = NULL;
         __pyx_t_5 = 0;
         #if CYTHON_UNPACK_METHODS
         if (unlikely(PyMethod_Check(__pyx_t_22))) {
@@ -44034,43 +44052,43 @@
         }
         #endif
         {
           PyObject *__pyx_callargs[2] = {__pyx_t_13, __pyx_t_2};
           __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_22, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
           __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
           __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-          if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 820, __pyx_L1_error)
+          if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 823, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_1);
           __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
         }
-        if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_event_index, __pyx_t_1) < 0) __PYX_ERR(0, 820, __pyx_L1_error)
+        if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_event_index, __pyx_t_1) < 0) __PYX_ERR(0, 823, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-        __pyx_t_1 = PyNumber_InPlaceOr(__pyx_v_put, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 820, __pyx_L1_error)
+        __pyx_t_1 = PyNumber_InPlaceOr(__pyx_v_put, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 823, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         __Pyx_DECREF_SET(__pyx_v_put, ((PyObject*)__pyx_t_1));
         __pyx_t_1 = 0;
 
-        /* "src/cmodules/cyincludes/cyoptimizer.pyx":821
+        /* "src/cmodules/cyincludes/cyoptimizer.pyx":824
  *                     put  = {env(data_i.first) : awkward.Array([data_i.second[index_itr.first] for index_itr in index_map]) for data_i in data_map}
  *                     put |= {"event_index" : awkward.Array([index_itr.first for index_itr in index_map])}
  *                     up_root[tree] = put             # <<<<<<<<<<<<<<
  *                     up_root.close()
  *                 up_root = uproot.recreate(v.replace(".hdf5", ".root"))
  */
-        if (unlikely((PyObject_SetItem(__pyx_v_up_root, __pyx_v_tree, __pyx_v_put) < 0))) __PYX_ERR(0, 821, __pyx_L1_error)
+        if (unlikely((PyObject_SetItem(__pyx_v_up_root, __pyx_v_tree, __pyx_v_put) < 0))) __PYX_ERR(0, 824, __pyx_L1_error)
 
-        /* "src/cmodules/cyincludes/cyoptimizer.pyx":822
+        /* "src/cmodules/cyincludes/cyoptimizer.pyx":825
  *                     put |= {"event_index" : awkward.Array([index_itr.first for index_itr in index_map])}
  *                     up_root[tree] = put
  *                     up_root.close()             # <<<<<<<<<<<<<<
  *                 up_root = uproot.recreate(v.replace(".hdf5", ".root"))
  * 
  */
-        __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_up_root, __pyx_n_s_close); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 822, __pyx_L1_error)
+        __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_up_root, __pyx_n_s_close); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 825, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __pyx_t_22 = NULL;
         __pyx_t_5 = 0;
         #if CYTHON_UNPACK_METHODS
         if (likely(PyMethod_Check(__pyx_t_4))) {
           __pyx_t_22 = PyMethod_GET_SELF(__pyx_t_4);
           if (likely(__pyx_t_22)) {
@@ -44082,46 +44100,46 @@
           }
         }
         #endif
         {
           PyObject *__pyx_callargs[2] = {__pyx_t_22, NULL};
           __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_5, 0+__pyx_t_5);
           __Pyx_XDECREF(__pyx_t_22); __pyx_t_22 = 0;
-          if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 822, __pyx_L1_error)
+          if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 825, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_1);
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         }
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-        /* "src/cmodules/cyincludes/cyoptimizer.pyx":818
+        /* "src/cmodules/cyincludes/cyoptimizer.pyx":821
  *                 if h5_file is not None: h5_file.close()
  *                 h5_file = h5py.File(v, "w")
  *                 if up_root is not None:             # <<<<<<<<<<<<<<
  *                     put  = {env(data_i.first) : awkward.Array([data_i.second[index_itr.first] for index_itr in index_map]) for data_i in data_map}
  *                     put |= {"event_index" : awkward.Array([index_itr.first for index_itr in index_map])}
  */
       }
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":823
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":826
  *                     up_root[tree] = put
  *                     up_root.close()
  *                 up_root = uproot.recreate(v.replace(".hdf5", ".root"))             # <<<<<<<<<<<<<<
  * 
  *                 data_map.clear()
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_uproot); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 823, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_uproot); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 826, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_22 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_recreate); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 823, __pyx_L1_error)
+      __pyx_t_22 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_recreate); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 826, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_22);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       if (unlikely(__pyx_v_v == Py_None)) {
         PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "replace");
-        __PYX_ERR(0, 823, __pyx_L1_error)
+        __PYX_ERR(0, 826, __pyx_L1_error)
       }
-      __pyx_t_4 = PyUnicode_Replace(__pyx_v_v, __pyx_kp_u_hdf5, __pyx_kp_u_root, -1L); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 823, __pyx_L1_error)
+      __pyx_t_4 = PyUnicode_Replace(__pyx_v_v, __pyx_kp_u_hdf5, __pyx_kp_u_root, -1L); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 826, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __pyx_t_2 = NULL;
       __pyx_t_5 = 0;
       #if CYTHON_UNPACK_METHODS
       if (unlikely(PyMethod_Check(__pyx_t_22))) {
         __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_22);
         if (likely(__pyx_t_2)) {
@@ -44134,80 +44152,80 @@
       }
       #endif
       {
         PyObject *__pyx_callargs[2] = {__pyx_t_2, __pyx_t_4};
         __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_22, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
         __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 823, __pyx_L1_error)
+        if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 826, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
       }
       __Pyx_DECREF_SET(__pyx_v_up_root, __pyx_t_1);
       __pyx_t_1 = 0;
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":825
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":828
  *                 up_root = uproot.recreate(v.replace(".hdf5", ".root"))
  * 
  *                 data_map.clear()             # <<<<<<<<<<<<<<
  *                 index_map.clear()
  * 
  */
       __pyx_v_data_map.clear();
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":826
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":829
  * 
  *                 data_map.clear()
  *                 index_map.clear()             # <<<<<<<<<<<<<<
  * 
  *                 idx += 1
  */
       __pyx_v_index_map.clear();
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":828
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":831
  *                 index_map.clear()
  * 
  *                 idx += 1             # <<<<<<<<<<<<<<
  *                 idy = 0
  * 
  */
       __pyx_v_idx = (__pyx_v_idx + 1);
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":829
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":832
  * 
  *                 idx += 1
  *                 idy = 0             # <<<<<<<<<<<<<<
  * 
  *             ix = gh["i"].tolist()[0]
  */
       __pyx_v_idy = 0;
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":812
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":815
  *             gh2 = gh.pop("graphs")[0].to_dict()
  *             gh.update(gh2)
  *             if indx[idx] == idy:             # <<<<<<<<<<<<<<
  *                 v = os.path.abspath(roots[idx])
  *                 try: os.makedirs("/".join(v.split("/")[:-1]))
  */
     }
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":831
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":834
  *                 idy = 0
  * 
  *             ix = gh["i"].tolist()[0]             # <<<<<<<<<<<<<<
  *             f = _check_sub(h5_file, env(hashes[0]))
  *             f.attrs.update({"event_index" : ix})
  */
     if (unlikely(__pyx_v_gh == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 831, __pyx_L1_error)
+      __PYX_ERR(0, 834, __pyx_L1_error)
     }
-    __pyx_t_22 = __Pyx_PyDict_GetItem(__pyx_v_gh, __pyx_n_u_i); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 831, __pyx_L1_error)
+    __pyx_t_22 = __Pyx_PyDict_GetItem(__pyx_v_gh, __pyx_n_u_i); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 834, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_22);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_22, __pyx_n_s_tolist); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 831, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_22, __pyx_n_s_tolist); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 834, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
     __pyx_t_22 = NULL;
     __pyx_t_5 = 0;
     #if CYTHON_UNPACK_METHODS
     if (likely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_22 = PyMethod_GET_SELF(__pyx_t_4);
@@ -44220,57 +44238,57 @@
       }
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_22, NULL};
       __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_5, 0+__pyx_t_5);
       __Pyx_XDECREF(__pyx_t_22); __pyx_t_22 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 831, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 834, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     }
-    __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_1, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 831, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_1, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 834, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_4); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 831, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_4); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 834, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_v_ix = __pyx_t_5;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":832
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":835
  * 
  *             ix = gh["i"].tolist()[0]
  *             f = _check_sub(h5_file, env(hashes[0]))             # <<<<<<<<<<<<<<
  *             f.attrs.update({"event_index" : ix})
  *             index_map[ix] = 0
  */
-    __pyx_t_4 = __pyx_f_7cytools_env((__pyx_v_hashes[0])); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 832, __pyx_L1_error)
+    __pyx_t_4 = __pyx_f_7cytools_env((__pyx_v_hashes[0])); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 835, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_1 = __pyx_f_9AnalysisG_9_cmodules_10cOptimizer__check_sub(__pyx_v_h5_file, ((PyObject*)__pyx_t_4)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 832, __pyx_L1_error)
+    __pyx_t_1 = __pyx_f_9AnalysisG_9_cmodules_10cOptimizer__check_sub(__pyx_v_h5_file, ((PyObject*)__pyx_t_4)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 835, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_XDECREF_SET(__pyx_v_f, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":833
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":836
  *             ix = gh["i"].tolist()[0]
  *             f = _check_sub(h5_file, env(hashes[0]))
  *             f.attrs.update({"event_index" : ix})             # <<<<<<<<<<<<<<
  *             index_map[ix] = 0
  *             for v, tn in gh.items():
  */
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_f, __pyx_n_s_attrs); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 833, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_f, __pyx_n_s_attrs); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 836, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_22 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_update); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 833, __pyx_L1_error)
+    __pyx_t_22 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_update); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 836, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_22);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 833, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 836, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_ix); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 833, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_ix); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 836, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_event_index, __pyx_t_2) < 0) __PYX_ERR(0, 833, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_event_index, __pyx_t_2) < 0) __PYX_ERR(0, 836, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_t_2 = NULL;
     __pyx_t_5 = 0;
     #if CYTHON_UNPACK_METHODS
     if (likely(PyMethod_Check(__pyx_t_22))) {
       __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_22);
       if (likely(__pyx_t_2)) {
@@ -44283,83 +44301,83 @@
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_2, __pyx_t_4};
       __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_22, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
       __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 833, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 836, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
     }
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":834
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":837
  *             f = _check_sub(h5_file, env(hashes[0]))
  *             f.attrs.update({"event_index" : ix})
  *             index_map[ix] = 0             # <<<<<<<<<<<<<<
  *             for v, tn in gh.items():
  *                 if not v.startswith("O_"): continue
  */
     (__pyx_v_index_map[__pyx_v_ix]) = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":835
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":838
  *             f.attrs.update({"event_index" : ix})
  *             index_map[ix] = 0
  *             for v, tn in gh.items():             # <<<<<<<<<<<<<<
  *                 if not v.startswith("O_"): continue
  *                 tn = tn.softmax(-1)
  */
     __pyx_t_7 = 0;
     if (unlikely(__pyx_v_gh == Py_None)) {
       PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "items");
-      __PYX_ERR(0, 835, __pyx_L1_error)
+      __PYX_ERR(0, 838, __pyx_L1_error)
     }
-    __pyx_t_22 = __Pyx_dict_iterator(__pyx_v_gh, 1, __pyx_n_s_items, (&__pyx_t_9), (&__pyx_t_5)); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 835, __pyx_L1_error)
+    __pyx_t_22 = __Pyx_dict_iterator(__pyx_v_gh, 1, __pyx_n_s_items, (&__pyx_t_9), (&__pyx_t_5)); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 838, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_22);
     __Pyx_XDECREF(__pyx_t_1);
     __pyx_t_1 = __pyx_t_22;
     __pyx_t_22 = 0;
     while (1) {
       __pyx_t_8 = __Pyx_dict_iter_next(__pyx_t_1, __pyx_t_9, &__pyx_t_7, &__pyx_t_22, &__pyx_t_4, NULL, __pyx_t_5);
       if (unlikely(__pyx_t_8 == 0)) break;
-      if (unlikely(__pyx_t_8 == -1)) __PYX_ERR(0, 835, __pyx_L1_error)
+      if (unlikely(__pyx_t_8 == -1)) __PYX_ERR(0, 838, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_22);
       __Pyx_GOTREF(__pyx_t_4);
-      if (!(likely(PyUnicode_CheckExact(__pyx_t_22))||((__pyx_t_22) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_t_22))) __PYX_ERR(0, 835, __pyx_L1_error)
+      if (!(likely(PyUnicode_CheckExact(__pyx_t_22))||((__pyx_t_22) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_t_22))) __PYX_ERR(0, 838, __pyx_L1_error)
       __Pyx_XDECREF_SET(__pyx_v_v, ((PyObject*)__pyx_t_22));
       __pyx_t_22 = 0;
       __Pyx_XDECREF_SET(__pyx_v_tn, __pyx_t_4);
       __pyx_t_4 = 0;
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":836
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":839
  *             index_map[ix] = 0
  *             for v, tn in gh.items():
  *                 if not v.startswith("O_"): continue             # <<<<<<<<<<<<<<
  *                 tn = tn.softmax(-1)
  *                 ten = tn.view(-1, tn.size()[-1])
  */
       if (unlikely(__pyx_v_v == Py_None)) {
         PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "startswith");
-        __PYX_ERR(0, 836, __pyx_L1_error)
+        __PYX_ERR(0, 839, __pyx_L1_error)
       }
-      __pyx_t_16 = __Pyx_PyUnicode_Tailmatch(__pyx_v_v, __pyx_n_u_O, 0, PY_SSIZE_T_MAX, -1); if (unlikely(__pyx_t_16 == ((int)-1))) __PYX_ERR(0, 836, __pyx_L1_error)
+      __pyx_t_16 = __Pyx_PyUnicode_Tailmatch(__pyx_v_v, __pyx_n_u_O, 0, PY_SSIZE_T_MAX, -1); if (unlikely(__pyx_t_16 == ((int)-1))) __PYX_ERR(0, 839, __pyx_L1_error)
       __pyx_t_26 = (!__pyx_t_16);
       if (__pyx_t_26) {
         goto __pyx_L39_continue;
       }
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":837
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":840
  *             for v, tn in gh.items():
  *                 if not v.startswith("O_"): continue
  *                 tn = tn.softmax(-1)             # <<<<<<<<<<<<<<
  *                 ten = tn.view(-1, tn.size()[-1])
  *                 f.attrs.update({v : ten.tolist()})
  */
-      __pyx_t_22 = __Pyx_PyObject_GetAttrStr(__pyx_v_tn, __pyx_n_s_softmax); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 837, __pyx_L1_error)
+      __pyx_t_22 = __Pyx_PyObject_GetAttrStr(__pyx_v_tn, __pyx_n_s_softmax); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 840, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_22);
       __pyx_t_2 = NULL;
       __pyx_t_8 = 0;
       #if CYTHON_UNPACK_METHODS
       if (likely(PyMethod_Check(__pyx_t_22))) {
         __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_22);
         if (likely(__pyx_t_2)) {
@@ -44371,31 +44389,31 @@
         }
       }
       #endif
       {
         PyObject *__pyx_callargs[2] = {__pyx_t_2, __pyx_int_neg_1};
         __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_22, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
         __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 837, __pyx_L1_error)
+        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 840, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
       }
       __Pyx_DECREF_SET(__pyx_v_tn, __pyx_t_4);
       __pyx_t_4 = 0;
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":838
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":841
  *                 if not v.startswith("O_"): continue
  *                 tn = tn.softmax(-1)
  *                 ten = tn.view(-1, tn.size()[-1])             # <<<<<<<<<<<<<<
  *                 f.attrs.update({v : ten.tolist()})
  *                 for k in range(tn.size()[-1]):
  */
-      __pyx_t_22 = __Pyx_PyObject_GetAttrStr(__pyx_v_tn, __pyx_n_s_view); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 838, __pyx_L1_error)
+      __pyx_t_22 = __Pyx_PyObject_GetAttrStr(__pyx_v_tn, __pyx_n_s_view); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 841, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_22);
-      __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_v_tn, __pyx_n_s_size); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 838, __pyx_L1_error)
+      __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_v_tn, __pyx_n_s_size); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 841, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_13);
       __pyx_t_25 = NULL;
       __pyx_t_8 = 0;
       #if CYTHON_UNPACK_METHODS
       if (likely(PyMethod_Check(__pyx_t_13))) {
         __pyx_t_25 = PyMethod_GET_SELF(__pyx_t_13);
         if (likely(__pyx_t_25)) {
@@ -44407,19 +44425,19 @@
         }
       }
       #endif
       {
         PyObject *__pyx_callargs[2] = {__pyx_t_25, NULL};
         __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_13, __pyx_callargs+1-__pyx_t_8, 0+__pyx_t_8);
         __Pyx_XDECREF(__pyx_t_25); __pyx_t_25 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 838, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 841, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
       }
-      __pyx_t_13 = __Pyx_GetItemInt(__pyx_t_2, -1L, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 838, __pyx_L1_error)
+      __pyx_t_13 = __Pyx_GetItemInt(__pyx_t_2, -1L, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 841, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_13);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __pyx_t_2 = NULL;
       __pyx_t_8 = 0;
       #if CYTHON_UNPACK_METHODS
       if (likely(PyMethod_Check(__pyx_t_22))) {
         __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_22);
@@ -44433,36 +44451,36 @@
       }
       #endif
       {
         PyObject *__pyx_callargs[3] = {__pyx_t_2, __pyx_int_neg_1, __pyx_t_13};
         __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_22, __pyx_callargs+1-__pyx_t_8, 2+__pyx_t_8);
         __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
-        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 838, __pyx_L1_error)
+        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 841, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
       }
       __Pyx_XDECREF_SET(__pyx_v_ten, __pyx_t_4);
       __pyx_t_4 = 0;
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":839
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":842
  *                 tn = tn.softmax(-1)
  *                 ten = tn.view(-1, tn.size()[-1])
  *                 f.attrs.update({v : ten.tolist()})             # <<<<<<<<<<<<<<
  *                 for k in range(tn.size()[-1]):
  *                     data_map[enc(v[2:] + "_cls_" + str(k))][ix] = tn[:, k].tolist()
  */
-      __pyx_t_22 = __Pyx_PyObject_GetAttrStr(__pyx_v_f, __pyx_n_s_attrs); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 839, __pyx_L1_error)
+      __pyx_t_22 = __Pyx_PyObject_GetAttrStr(__pyx_v_f, __pyx_n_s_attrs); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 842, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_22);
-      __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_t_22, __pyx_n_s_update); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 839, __pyx_L1_error)
+      __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_t_22, __pyx_n_s_update); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 842, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_13);
       __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
-      __pyx_t_22 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 839, __pyx_L1_error)
+      __pyx_t_22 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 842, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_22);
-      __pyx_t_25 = __Pyx_PyObject_GetAttrStr(__pyx_v_ten, __pyx_n_s_tolist); if (unlikely(!__pyx_t_25)) __PYX_ERR(0, 839, __pyx_L1_error)
+      __pyx_t_25 = __Pyx_PyObject_GetAttrStr(__pyx_v_ten, __pyx_n_s_tolist); if (unlikely(!__pyx_t_25)) __PYX_ERR(0, 842, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_25);
       __pyx_t_27 = NULL;
       __pyx_t_8 = 0;
       #if CYTHON_UNPACK_METHODS
       if (likely(PyMethod_Check(__pyx_t_25))) {
         __pyx_t_27 = PyMethod_GET_SELF(__pyx_t_25);
         if (likely(__pyx_t_27)) {
@@ -44474,19 +44492,19 @@
         }
       }
       #endif
       {
         PyObject *__pyx_callargs[2] = {__pyx_t_27, NULL};
         __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_25, __pyx_callargs+1-__pyx_t_8, 0+__pyx_t_8);
         __Pyx_XDECREF(__pyx_t_27); __pyx_t_27 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 839, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 842, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_25); __pyx_t_25 = 0;
       }
-      if (PyDict_SetItem(__pyx_t_22, __pyx_v_v, __pyx_t_2) < 0) __PYX_ERR(0, 839, __pyx_L1_error)
+      if (PyDict_SetItem(__pyx_t_22, __pyx_v_v, __pyx_t_2) < 0) __PYX_ERR(0, 842, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __pyx_t_2 = NULL;
       __pyx_t_8 = 0;
       #if CYTHON_UNPACK_METHODS
       if (likely(PyMethod_Check(__pyx_t_13))) {
         __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_13);
         if (likely(__pyx_t_2)) {
@@ -44499,28 +44517,28 @@
       }
       #endif
       {
         PyObject *__pyx_callargs[2] = {__pyx_t_2, __pyx_t_22};
         __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_13, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
         __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
-        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 839, __pyx_L1_error)
+        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 842, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
       }
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-      /* "src/cmodules/cyincludes/cyoptimizer.pyx":840
+      /* "src/cmodules/cyincludes/cyoptimizer.pyx":843
  *                 ten = tn.view(-1, tn.size()[-1])
  *                 f.attrs.update({v : ten.tolist()})
  *                 for k in range(tn.size()[-1]):             # <<<<<<<<<<<<<<
  *                     data_map[enc(v[2:] + "_cls_" + str(k))][ix] = tn[:, k].tolist()
  *             bar.update(1)
  */
-      __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_v_tn, __pyx_n_s_size); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 840, __pyx_L1_error)
+      __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_v_tn, __pyx_n_s_size); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 843, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_13);
       __pyx_t_22 = NULL;
       __pyx_t_8 = 0;
       #if CYTHON_UNPACK_METHODS
       if (likely(PyMethod_Check(__pyx_t_13))) {
         __pyx_t_22 = PyMethod_GET_SELF(__pyx_t_13);
         if (likely(__pyx_t_22)) {
@@ -44532,99 +44550,99 @@
         }
       }
       #endif
       {
         PyObject *__pyx_callargs[2] = {__pyx_t_22, NULL};
         __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_13, __pyx_callargs+1-__pyx_t_8, 0+__pyx_t_8);
         __Pyx_XDECREF(__pyx_t_22); __pyx_t_22 = 0;
-        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 840, __pyx_L1_error)
+        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 843, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
       }
-      __pyx_t_13 = __Pyx_GetItemInt(__pyx_t_4, -1L, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 840, __pyx_L1_error)
+      __pyx_t_13 = __Pyx_GetItemInt(__pyx_t_4, -1L, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 843, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_13);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_range, __pyx_t_13); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 840, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_range, __pyx_t_13); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 843, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
       if (likely(PyList_CheckExact(__pyx_t_4)) || PyTuple_CheckExact(__pyx_t_4)) {
         __pyx_t_13 = __pyx_t_4; __Pyx_INCREF(__pyx_t_13);
         __pyx_t_28 = 0;
         __pyx_t_29 = NULL;
       } else {
-        __pyx_t_28 = -1; __pyx_t_13 = PyObject_GetIter(__pyx_t_4); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 840, __pyx_L1_error)
+        __pyx_t_28 = -1; __pyx_t_13 = PyObject_GetIter(__pyx_t_4); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 843, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_13);
-        __pyx_t_29 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_13); if (unlikely(!__pyx_t_29)) __PYX_ERR(0, 840, __pyx_L1_error)
+        __pyx_t_29 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_13); if (unlikely(!__pyx_t_29)) __PYX_ERR(0, 843, __pyx_L1_error)
       }
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       for (;;) {
         if (likely(!__pyx_t_29)) {
           if (likely(PyList_CheckExact(__pyx_t_13))) {
             {
               Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_13);
               #if !CYTHON_ASSUME_SAFE_MACROS
-              if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 840, __pyx_L1_error)
+              if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 843, __pyx_L1_error)
               #endif
               if (__pyx_t_28 >= __pyx_temp) break;
             }
             #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-            __pyx_t_4 = PyList_GET_ITEM(__pyx_t_13, __pyx_t_28); __Pyx_INCREF(__pyx_t_4); __pyx_t_28++; if (unlikely((0 < 0))) __PYX_ERR(0, 840, __pyx_L1_error)
+            __pyx_t_4 = PyList_GET_ITEM(__pyx_t_13, __pyx_t_28); __Pyx_INCREF(__pyx_t_4); __pyx_t_28++; if (unlikely((0 < 0))) __PYX_ERR(0, 843, __pyx_L1_error)
             #else
-            __pyx_t_4 = __Pyx_PySequence_ITEM(__pyx_t_13, __pyx_t_28); __pyx_t_28++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 840, __pyx_L1_error)
+            __pyx_t_4 = __Pyx_PySequence_ITEM(__pyx_t_13, __pyx_t_28); __pyx_t_28++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 843, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_4);
             #endif
           } else {
             {
               Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_13);
               #if !CYTHON_ASSUME_SAFE_MACROS
-              if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 840, __pyx_L1_error)
+              if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 843, __pyx_L1_error)
               #endif
               if (__pyx_t_28 >= __pyx_temp) break;
             }
             #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-            __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_13, __pyx_t_28); __Pyx_INCREF(__pyx_t_4); __pyx_t_28++; if (unlikely((0 < 0))) __PYX_ERR(0, 840, __pyx_L1_error)
+            __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_13, __pyx_t_28); __Pyx_INCREF(__pyx_t_4); __pyx_t_28++; if (unlikely((0 < 0))) __PYX_ERR(0, 843, __pyx_L1_error)
             #else
-            __pyx_t_4 = __Pyx_PySequence_ITEM(__pyx_t_13, __pyx_t_28); __pyx_t_28++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 840, __pyx_L1_error)
+            __pyx_t_4 = __Pyx_PySequence_ITEM(__pyx_t_13, __pyx_t_28); __pyx_t_28++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 843, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_4);
             #endif
           }
         } else {
           __pyx_t_4 = __pyx_t_29(__pyx_t_13);
           if (unlikely(!__pyx_t_4)) {
             PyObject* exc_type = PyErr_Occurred();
             if (exc_type) {
               if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-              else __PYX_ERR(0, 840, __pyx_L1_error)
+              else __PYX_ERR(0, 843, __pyx_L1_error)
             }
             break;
           }
           __Pyx_GOTREF(__pyx_t_4);
         }
         __Pyx_XDECREF_SET(__pyx_v_k, __pyx_t_4);
         __pyx_t_4 = 0;
 
-        /* "src/cmodules/cyincludes/cyoptimizer.pyx":841
+        /* "src/cmodules/cyincludes/cyoptimizer.pyx":844
  *                 f.attrs.update({v : ten.tolist()})
  *                 for k in range(tn.size()[-1]):
  *                     data_map[enc(v[2:] + "_cls_" + str(k))][ix] = tn[:, k].tolist()             # <<<<<<<<<<<<<<
  *             bar.update(1)
  *             idy+=1
  */
-        __pyx_t_22 = PyTuple_New(2); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 841, __pyx_L1_error)
+        __pyx_t_22 = PyTuple_New(2); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 844, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_22);
         __Pyx_INCREF(__pyx_slice__68);
         __Pyx_GIVEREF(__pyx_slice__68);
-        if (__Pyx_PyTuple_SET_ITEM(__pyx_t_22, 0, __pyx_slice__68)) __PYX_ERR(0, 841, __pyx_L1_error);
+        if (__Pyx_PyTuple_SET_ITEM(__pyx_t_22, 0, __pyx_slice__68)) __PYX_ERR(0, 844, __pyx_L1_error);
         __Pyx_INCREF(__pyx_v_k);
         __Pyx_GIVEREF(__pyx_v_k);
-        if (__Pyx_PyTuple_SET_ITEM(__pyx_t_22, 1, __pyx_v_k)) __PYX_ERR(0, 841, __pyx_L1_error);
-        __pyx_t_2 = __Pyx_PyObject_GetItem(__pyx_v_tn, __pyx_t_22); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 841, __pyx_L1_error)
+        if (__Pyx_PyTuple_SET_ITEM(__pyx_t_22, 1, __pyx_v_k)) __PYX_ERR(0, 844, __pyx_L1_error);
+        __pyx_t_2 = __Pyx_PyObject_GetItem(__pyx_v_tn, __pyx_t_22); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 844, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
-        __pyx_t_22 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_tolist); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 841, __pyx_L1_error)
+        __pyx_t_22 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_tolist); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 844, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_22);
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __pyx_t_2 = NULL;
         __pyx_t_8 = 0;
         #if CYTHON_UNPACK_METHODS
         if (likely(PyMethod_Check(__pyx_t_22))) {
           __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_22);
@@ -44637,60 +44655,60 @@
           }
         }
         #endif
         {
           PyObject *__pyx_callargs[2] = {__pyx_t_2, NULL};
           __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_22, __pyx_callargs+1-__pyx_t_8, 0+__pyx_t_8);
           __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-          if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 841, __pyx_L1_error)
+          if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 844, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_4);
           __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
         }
-        __pyx_t_30 = __pyx_convert_vector_from_py_float(__pyx_t_4); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 841, __pyx_L1_error)
+        __pyx_t_30 = __pyx_convert_vector_from_py_float(__pyx_t_4); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 844, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         if (unlikely(__pyx_v_v == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-          __PYX_ERR(0, 841, __pyx_L1_error)
+          __PYX_ERR(0, 844, __pyx_L1_error)
         }
-        __pyx_t_4 = __Pyx_PyUnicode_Substring(__pyx_v_v, 2, PY_SSIZE_T_MAX); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 841, __pyx_L1_error)
+        __pyx_t_4 = __Pyx_PyUnicode_Substring(__pyx_v_v, 2, PY_SSIZE_T_MAX); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 844, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
-        __pyx_t_22 = __Pyx_PyUnicode_ConcatInPlace(__pyx_t_4, __pyx_n_u_cls); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 841, __pyx_L1_error)
+        __pyx_t_22 = __Pyx_PyUnicode_ConcatInPlace(__pyx_t_4, __pyx_n_u_cls); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 844, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_22);
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        __pyx_t_4 = __Pyx_PyObject_Str(__pyx_v_k); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 841, __pyx_L1_error)
+        __pyx_t_4 = __Pyx_PyObject_Str(__pyx_v_k); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 844, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
-        __pyx_t_2 = PyNumber_Add(__pyx_t_22, __pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 841, __pyx_L1_error)
+        __pyx_t_2 = PyNumber_Add(__pyx_t_22, __pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 844, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        __pyx_t_11 = __pyx_f_7cytools_enc(((PyObject*)__pyx_t_2)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 841, __pyx_L1_error)
+        __pyx_t_11 = __pyx_f_7cytools_enc(((PyObject*)__pyx_t_2)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 844, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         ((__pyx_v_data_map[__pyx_t_11])[__pyx_v_ix]) = __pyx_t_30;
 
-        /* "src/cmodules/cyincludes/cyoptimizer.pyx":840
+        /* "src/cmodules/cyincludes/cyoptimizer.pyx":843
  *                 ten = tn.view(-1, tn.size()[-1])
  *                 f.attrs.update({v : ten.tolist()})
  *                 for k in range(tn.size()[-1]):             # <<<<<<<<<<<<<<
  *                     data_map[enc(v[2:] + "_cls_" + str(k))][ix] = tn[:, k].tolist()
  *             bar.update(1)
  */
       }
       __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
       __pyx_L39_continue:;
     }
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":842
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":845
  *                 for k in range(tn.size()[-1]):
  *                     data_map[enc(v[2:] + "_cls_" + str(k))][ix] = tn[:, k].tolist()
  *             bar.update(1)             # <<<<<<<<<<<<<<
  *             idy+=1
  *         h5_file.close()
  */
-    __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_v_bar, __pyx_n_s_update); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 842, __pyx_L1_error)
+    __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_v_bar, __pyx_n_s_update); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 845, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_13);
     __pyx_t_2 = NULL;
     __pyx_t_5 = 0;
     #if CYTHON_UNPACK_METHODS
     if (likely(PyMethod_Check(__pyx_t_13))) {
       __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_13);
       if (likely(__pyx_t_2)) {
@@ -44702,47 +44720,47 @@
       }
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_2, __pyx_int_1};
       __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_13, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
       __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 842, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 845, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
     }
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":843
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":846
  *                     data_map[enc(v[2:] + "_cls_" + str(k))][ix] = tn[:, k].tolist()
  *             bar.update(1)
  *             idy+=1             # <<<<<<<<<<<<<<
  *         h5_file.close()
  *         put  = {env(data_i.first) : awkward.Array([data_i.second[index_itr.first] for index_itr in index_map]) for data_i in data_map}
  */
     __pyx_v_idy = (__pyx_v_idy + 1);
 
-    /* "src/cmodules/cyincludes/cyoptimizer.pyx":808
+    /* "src/cmodules/cyincludes/cyoptimizer.pyx":811
  *         cdef pair[string, map[int, vector[float]]] data_i
  * 
  *         for data, hashes in loader:             # <<<<<<<<<<<<<<
  *             gh = model(data)
  *             gh2 = gh.pop("graphs")[0].to_dict()
  */
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":844
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":847
  *             bar.update(1)
  *             idy+=1
  *         h5_file.close()             # <<<<<<<<<<<<<<
  *         put  = {env(data_i.first) : awkward.Array([data_i.second[index_itr.first] for index_itr in index_map]) for data_i in data_map}
  *         put |= {"event_index" : awkward.Array([index_itr.first for index_itr in index_map])}
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_h5_file, __pyx_n_s_close); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 844, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_h5_file, __pyx_n_s_close); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 847, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_13 = NULL;
   __pyx_t_5 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_1))) {
     __pyx_t_13 = PyMethod_GET_SELF(__pyx_t_1);
     if (likely(__pyx_t_13)) {
@@ -44754,55 +44772,55 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_13, NULL};
     __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_5, 0+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 844, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 847, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":845
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":848
  *             idy+=1
  *         h5_file.close()
  *         put  = {env(data_i.first) : awkward.Array([data_i.second[index_itr.first] for index_itr in index_map]) for data_i in data_map}             # <<<<<<<<<<<<<<
  *         put |= {"event_index" : awkward.Array([index_itr.first for index_itr in index_map])}
  *         up_root[tree] = put
  */
   { /* enter inner scope */
-    __pyx_t_3 = PyDict_New(); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 845, __pyx_L1_error)
+    __pyx_t_3 = PyDict_New(); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 848, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_20 = __pyx_v_data_map.begin();
     for (;;) {
       if (!(__pyx_t_20 != __pyx_v_data_map.end())) break;
       __pyx_t_21 = *__pyx_t_20;
       ++__pyx_t_20;
       __pyx_9genexpr16__pyx_v_data_i = __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_21);
-      __pyx_t_1 = __pyx_f_7cytools_env(__pyx_9genexpr16__pyx_v_data_i.first); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 845, __pyx_L1_error)
+      __pyx_t_1 = __pyx_f_7cytools_env(__pyx_9genexpr16__pyx_v_data_i.first); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 848, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_awkward); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 845, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_awkward); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 848, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_Array); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 845, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_Array); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 848, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       { /* enter inner scope */
-        __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 845, __pyx_L1_error)
+        __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 848, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __pyx_t_23 = __pyx_v_index_map.begin();
         for (;;) {
           if (!(__pyx_t_23 != __pyx_v_index_map.end())) break;
           __pyx_t_24 = *__pyx_t_23;
           ++__pyx_t_23;
           __pyx_9genexpr17__pyx_v_index_itr = __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_24);
-          __pyx_t_22 = __pyx_convert_vector_to_py_float((__pyx_9genexpr16__pyx_v_data_i.second[__pyx_9genexpr17__pyx_v_index_itr.first])); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 845, __pyx_L1_error)
+          __pyx_t_22 = __pyx_convert_vector_to_py_float((__pyx_9genexpr16__pyx_v_data_i.second[__pyx_9genexpr17__pyx_v_index_itr.first])); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 848, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_22);
-          if (unlikely(__Pyx_ListComp_Append(__pyx_t_2, (PyObject*)__pyx_t_22))) __PYX_ERR(0, 845, __pyx_L1_error)
+          if (unlikely(__Pyx_ListComp_Append(__pyx_t_2, (PyObject*)__pyx_t_22))) __PYX_ERR(0, 848, __pyx_L1_error)
           __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
         }
       } /* exit inner scope */
       __pyx_t_22 = NULL;
       __pyx_t_5 = 0;
       #if CYTHON_UNPACK_METHODS
       if (unlikely(PyMethod_Check(__pyx_t_4))) {
@@ -44817,52 +44835,52 @@
       }
       #endif
       {
         PyObject *__pyx_callargs[2] = {__pyx_t_22, __pyx_t_2};
         __pyx_t_13 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
         __Pyx_XDECREF(__pyx_t_22); __pyx_t_22 = 0;
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-        if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 845, __pyx_L1_error)
+        if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 848, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_13);
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       }
-      if (unlikely(PyDict_SetItem(__pyx_t_3, (PyObject*)__pyx_t_1, (PyObject*)__pyx_t_13))) __PYX_ERR(0, 845, __pyx_L1_error)
+      if (unlikely(PyDict_SetItem(__pyx_t_3, (PyObject*)__pyx_t_1, (PyObject*)__pyx_t_13))) __PYX_ERR(0, 848, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
     }
   } /* exit inner scope */
   __Pyx_XDECREF_SET(__pyx_v_put, ((PyObject*)__pyx_t_3));
   __pyx_t_3 = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":846
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":849
  *         h5_file.close()
  *         put  = {env(data_i.first) : awkward.Array([data_i.second[index_itr.first] for index_itr in index_map]) for data_i in data_map}
  *         put |= {"event_index" : awkward.Array([index_itr.first for index_itr in index_map])}             # <<<<<<<<<<<<<<
  *         up_root[tree] = put
  *         up_root.close()
  */
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 846, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 849, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_awkward); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 846, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_awkward); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 849, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_Array); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 846, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_Array); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 849, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   { /* enter inner scope */
-    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 846, __pyx_L1_error)
+    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 849, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_23 = __pyx_v_index_map.begin();
     for (;;) {
       if (!(__pyx_t_23 != __pyx_v_index_map.end())) break;
       __pyx_t_24 = *__pyx_t_23;
       ++__pyx_t_23;
       __pyx_9genexpr18__pyx_v_index_itr = __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_24);
-      __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_9genexpr18__pyx_v_index_itr.first); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 846, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_9genexpr18__pyx_v_index_itr.first); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 849, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_2))) __PYX_ERR(0, 846, __pyx_L1_error)
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_2))) __PYX_ERR(0, 849, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     }
   } /* exit inner scope */
   __pyx_t_2 = NULL;
   __pyx_t_5 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_4))) {
@@ -44877,43 +44895,43 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_2, __pyx_t_1};
     __pyx_t_13 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 846, __pyx_L1_error)
+    if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 849, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_13);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   }
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_event_index, __pyx_t_13) < 0) __PYX_ERR(0, 846, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_event_index, __pyx_t_13) < 0) __PYX_ERR(0, 849, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
-  __pyx_t_13 = PyNumber_InPlaceOr(__pyx_v_put, __pyx_t_3); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 846, __pyx_L1_error)
+  __pyx_t_13 = PyNumber_InPlaceOr(__pyx_v_put, __pyx_t_3); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 849, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_13);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF_SET(__pyx_v_put, ((PyObject*)__pyx_t_13));
   __pyx_t_13 = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":847
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":850
  *         put  = {env(data_i.first) : awkward.Array([data_i.second[index_itr.first] for index_itr in index_map]) for data_i in data_map}
  *         put |= {"event_index" : awkward.Array([index_itr.first for index_itr in index_map])}
  *         up_root[tree] = put             # <<<<<<<<<<<<<<
  *         up_root.close()
  * 
  */
-  if (unlikely((PyObject_SetItem(__pyx_v_up_root, __pyx_v_tree, __pyx_v_put) < 0))) __PYX_ERR(0, 847, __pyx_L1_error)
+  if (unlikely((PyObject_SetItem(__pyx_v_up_root, __pyx_v_tree, __pyx_v_put) < 0))) __PYX_ERR(0, 850, __pyx_L1_error)
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":848
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":851
  *         put |= {"event_index" : awkward.Array([index_itr.first for index_itr in index_map])}
  *         up_root[tree] = put
  *         up_root.close()             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_up_root, __pyx_n_s_close); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 848, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_up_root, __pyx_n_s_close); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 851, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   __pyx_t_5 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
@@ -44925,21 +44943,21 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_4, NULL};
     __pyx_t_13 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 0+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 848, __pyx_L1_error)
+    if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 851, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_13);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":774
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":777
  *         for itr in self.ptr.epoch_test:  itr.second.purge()
  * 
  *     cpdef SinkInjector(self, model, bar):             # <<<<<<<<<<<<<<
  *         cdef str v
  *         cdef list g
  */
 
@@ -45033,43 +45051,43 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_model)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 774, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 777, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_bar)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 774, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 777, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("SinkInjector", 1, 2, 2, 1); __PYX_ERR(0, 774, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("SinkInjector", 1, 2, 2, 1); __PYX_ERR(0, 777, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "SinkInjector") < 0)) __PYX_ERR(0, 774, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "SinkInjector") < 0)) __PYX_ERR(0, 777, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 2)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
     __pyx_v_model = values[0];
     __pyx_v_bar = values[1];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("SinkInjector", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 774, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("SinkInjector", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 777, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -45097,15 +45115,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("SinkInjector", 1);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_SinkInjector(__pyx_v_self, __pyx_v_model, __pyx_v_bar, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 774, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_SinkInjector(__pyx_v_self, __pyx_v_model, __pyx_v_bar, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -45114,15 +45132,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/cmodules/cyincludes/cyoptimizer.pyx":610
+/* "src/cmodules/cyincludes/cyoptimizer.pyx":613
  * 
  *     cdef report_t state
  *     cdef public bool metric_plots             # <<<<<<<<<<<<<<
  *     cdef public int threads
  *     cdef public sampletracer
  */
 
@@ -45146,15 +45164,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 1);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_v_self->metric_plots); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 610, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_v_self->metric_plots); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 613, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -45184,28 +45202,28 @@
 
 static int __pyx_pf_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_12metric_plots_2__set__(struct __pyx_obj_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer *__pyx_v_self, PyObject *__pyx_v_value) {
   int __pyx_r;
   bool __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_value); if (unlikely((__pyx_t_1 == ((bool)-1)) && PyErr_Occurred())) __PYX_ERR(0, 610, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_value); if (unlikely((__pyx_t_1 == ((bool)-1)) && PyErr_Occurred())) __PYX_ERR(0, 613, __pyx_L1_error)
   __pyx_v_self->metric_plots = __pyx_t_1;
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("AnalysisG._cmodules.cOptimizer.cOptimizer.metric_plots.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "src/cmodules/cyincludes/cyoptimizer.pyx":611
+/* "src/cmodules/cyincludes/cyoptimizer.pyx":614
  *     cdef report_t state
  *     cdef public bool metric_plots
  *     cdef public int threads             # <<<<<<<<<<<<<<
  *     cdef public sampletracer
  * 
  */
 
@@ -45229,15 +45247,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 1);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->threads); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 611, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->threads); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 614, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -45267,28 +45285,28 @@
 
 static int __pyx_pf_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_7threads_2__set__(struct __pyx_obj_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer *__pyx_v_self, PyObject *__pyx_v_value) {
   int __pyx_r;
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_value); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 611, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_value); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 614, __pyx_L1_error)
   __pyx_v_self->threads = __pyx_t_1;
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("AnalysisG._cmodules.cOptimizer.cOptimizer.threads.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "src/cmodules/cyincludes/cyoptimizer.pyx":612
+/* "src/cmodules/cyincludes/cyoptimizer.pyx":615
  *     cdef public bool metric_plots
  *     cdef public int threads
  *     cdef public sampletracer             # <<<<<<<<<<<<<<
  * 
  *     def __cinit__(self):
  */
 
@@ -46165,14 +46183,15 @@
     {&__pyx_n_s_FileExistsError, __pyx_k_FileExistsError, sizeof(__pyx_k_FileExistsError), 0, 0, 1, 1},
     {&__pyx_n_s_FileNotFoundError, __pyx_k_FileNotFoundError, sizeof(__pyx_k_FileNotFoundError), 0, 0, 1, 1},
     {&__pyx_n_u_Filename, __pyx_k_Filename, sizeof(__pyx_k_Filename), 0, 1, 0, 1},
     {&__pyx_n_s_FlushGraphs, __pyx_k_FlushGraphs, sizeof(__pyx_k_FlushGraphs), 0, 0, 1, 1},
     {&__pyx_n_s_GetHDF5Hashes, __pyx_k_GetHDF5Hashes, sizeof(__pyx_k_GetHDF5Hashes), 0, 0, 1, 1},
     {&__pyx_n_u_Graph, __pyx_k_Graph, sizeof(__pyx_k_Graph), 0, 1, 0, 1},
     {&__pyx_kp_u_GraphCache, __pyx_k_GraphCache, sizeof(__pyx_k_GraphCache), 0, 1, 0, 0},
+    {&__pyx_n_u_Histogram, __pyx_k_Histogram, sizeof(__pyx_k_Histogram), 0, 1, 0, 1},
     {&__pyx_n_u_Histograms, __pyx_k_Histograms, sizeof(__pyx_k_Histograms), 0, 1, 0, 1},
     {&__pyx_n_s_IndexError, __pyx_k_IndexError, sizeof(__pyx_k_IndexError), 0, 0, 1, 1},
     {&__pyx_n_s_KeyError, __pyx_k_KeyError, sizeof(__pyx_k_KeyError), 0, 0, 1, 1},
     {&__pyx_n_u_L, __pyx_k_L, sizeof(__pyx_k_L), 0, 1, 0, 1},
     {&__pyx_n_u_Lines, __pyx_k_Lines, sizeof(__pyx_k_Lines), 0, 1, 0, 1},
     {&__pyx_kp_u_Loss_Curve_for, __pyx_k_Loss_Curve_for, sizeof(__pyx_k_Loss_Curve_for), 0, 1, 0, 0},
     {&__pyx_kp_u_Loss_arb, __pyx_k_Loss_arb, sizeof(__pyx_k_Loss_arb), 0, 1, 0, 0},
@@ -46565,31 +46584,31 @@
     {&__pyx_n_u_xMin, __pyx_k_xMin, sizeof(__pyx_k_xMin), 0, 1, 0, 1},
     {&__pyx_n_u_xStep, __pyx_k_xStep, sizeof(__pyx_k_xStep), 0, 1, 0, 1},
     {&__pyx_n_u_xTitle, __pyx_k_xTitle, sizeof(__pyx_k_xTitle), 0, 1, 0, 1},
     {&__pyx_n_u_yData, __pyx_k_yData, sizeof(__pyx_k_yData), 0, 1, 0, 1},
     {&__pyx_n_u_yDataDown, __pyx_k_yDataDown, sizeof(__pyx_k_yDataDown), 0, 1, 0, 1},
     {&__pyx_n_u_yDataUp, __pyx_k_yDataUp, sizeof(__pyx_k_yDataUp), 0, 1, 0, 1},
     {&__pyx_n_u_yLogarithmic, __pyx_k_yLogarithmic, sizeof(__pyx_k_yLogarithmic), 0, 1, 0, 1},
-    {&__pyx_n_s_yMax, __pyx_k_yMax, sizeof(__pyx_k_yMax), 0, 0, 1, 1},
+    {&__pyx_n_u_yMax, __pyx_k_yMax, sizeof(__pyx_k_yMax), 0, 1, 0, 1},
     {&__pyx_n_u_yMin, __pyx_k_yMin, sizeof(__pyx_k_yMin), 0, 1, 0, 1},
     {&__pyx_n_u_yTitle, __pyx_k_yTitle, sizeof(__pyx_k_yTitle), 0, 1, 0, 1},
     {0, 0, 0, 0, 0, 0, 0}
   };
   return __Pyx_InitStrings(__pyx_string_tab);
 }
 /* #### Code section: cached_builtins ### */
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 35, __pyx_L1_error)
   __pyx_builtin_sum = __Pyx_GetBuiltinName(__pyx_n_s_sum); if (!__pyx_builtin_sum) __PYX_ERR(0, 110, __pyx_L1_error)
   __pyx_builtin_KeyError = __Pyx_GetBuiltinName(__pyx_n_s_KeyError); if (!__pyx_builtin_KeyError) __PYX_ERR(0, 116, __pyx_L1_error)
-  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 332, __pyx_L1_error)
-  __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(0, 334, __pyx_L1_error)
-  __pyx_builtin_max = __Pyx_GetBuiltinName(__pyx_n_s_max); if (!__pyx_builtin_max) __PYX_ERR(0, 437, __pyx_L1_error)
-  __pyx_builtin_StopIteration = __Pyx_GetBuiltinName(__pyx_n_s_StopIteration); if (!__pyx_builtin_StopIteration) __PYX_ERR(0, 549, __pyx_L1_error)
-  __pyx_builtin_RuntimeError = __Pyx_GetBuiltinName(__pyx_n_s_RuntimeError); if (!__pyx_builtin_RuntimeError) __PYX_ERR(0, 565, __pyx_L1_error)
+  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 335, __pyx_L1_error)
+  __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(0, 337, __pyx_L1_error)
+  __pyx_builtin_max = __Pyx_GetBuiltinName(__pyx_n_s_max); if (!__pyx_builtin_max) __PYX_ERR(0, 440, __pyx_L1_error)
+  __pyx_builtin_StopIteration = __Pyx_GetBuiltinName(__pyx_n_s_StopIteration); if (!__pyx_builtin_StopIteration) __PYX_ERR(0, 552, __pyx_L1_error)
+  __pyx_builtin_RuntimeError = __Pyx_GetBuiltinName(__pyx_n_s_RuntimeError); if (!__pyx_builtin_RuntimeError) __PYX_ERR(0, 568, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(1, 2, __pyx_L1_error)
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(1, 68, __pyx_L1_error)
   __pyx_builtin_AttributeError = __Pyx_GetBuiltinName(__pyx_n_s_AttributeError); if (!__pyx_builtin_AttributeError) __PYX_ERR(2, 297, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
@@ -47233,55 +47252,55 @@
  *     result.mass_pred = value
  *     return result
  */
   __pyx_tuple__58 = PyTuple_Pack(1, __pyx_kp_s_No_value_specified_for_struct_at_58); if (unlikely(!__pyx_tuple__58)) __PYX_ERR(1, 55, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__58);
   __Pyx_GIVEREF(__pyx_tuple__58);
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":397
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":400
  * 
  *             for name in lines:
  *                 fname = name.split(" ")[2].replace(" ", "")             # <<<<<<<<<<<<<<
  *                 cls = name.split("-")[1].replace(" ", "")
  * 
  */
-  __pyx_tuple__64 = PyTuple_Pack(2, __pyx_kp_u__63, __pyx_kp_u__61); if (unlikely(!__pyx_tuple__64)) __PYX_ERR(0, 397, __pyx_L1_error)
+  __pyx_tuple__64 = PyTuple_Pack(2, __pyx_kp_u__63, __pyx_kp_u__61); if (unlikely(!__pyx_tuple__64)) __PYX_ERR(0, 400, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__64);
   __Pyx_GIVEREF(__pyx_tuple__64);
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":562
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":565
  * 
  *         cdef int idx = self.sampletracer.MaxGPU
  *         cdef tuple cuda = (None, None)             # <<<<<<<<<<<<<<
  *         if idx != -1:
  *             try: cuda = torch.cuda.mem_get_info()
  */
-  __pyx_tuple__66 = PyTuple_Pack(2, Py_None, Py_None); if (unlikely(!__pyx_tuple__66)) __PYX_ERR(0, 562, __pyx_L1_error)
+  __pyx_tuple__66 = PyTuple_Pack(2, Py_None, Py_None); if (unlikely(!__pyx_tuple__66)) __PYX_ERR(0, 565, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__66);
   __Pyx_GIVEREF(__pyx_tuple__66);
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":814
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":817
  *             if indx[idx] == idy:
  *                 v = os.path.abspath(roots[idx])
  *                 try: os.makedirs("/".join(v.split("/")[:-1]))             # <<<<<<<<<<<<<<
  *                 except FileExistsError: pass
  *                 if h5_file is not None: h5_file.close()
  */
-  __pyx_slice__67 = PySlice_New(Py_None, __pyx_int_neg_1, Py_None); if (unlikely(!__pyx_slice__67)) __PYX_ERR(0, 814, __pyx_L1_error)
+  __pyx_slice__67 = PySlice_New(Py_None, __pyx_int_neg_1, Py_None); if (unlikely(!__pyx_slice__67)) __PYX_ERR(0, 817, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_slice__67);
   __Pyx_GIVEREF(__pyx_slice__67);
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":841
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":844
  *                 f.attrs.update({v : ten.tolist()})
  *                 for k in range(tn.size()[-1]):
  *                     data_map[enc(v[2:] + "_cls_" + str(k))][ix] = tn[:, k].tolist()             # <<<<<<<<<<<<<<
  *             bar.update(1)
  *             idy+=1
  */
-  __pyx_slice__68 = PySlice_New(Py_None, Py_None, Py_None); if (unlikely(!__pyx_slice__68)) __PYX_ERR(0, 841, __pyx_L1_error)
+  __pyx_slice__68 = PySlice_New(Py_None, Py_None, Py_None); if (unlikely(!__pyx_slice__68)) __PYX_ERR(0, 844, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_slice__68);
   __Pyx_GIVEREF(__pyx_slice__68);
 
   /* "cytools.pxd":270
  *         else: convert(ten, &(dereference(app)[enc(val[2:])].nodes))
  * 
  * cpdef inline recast(dict inpt, dict out_map):             # <<<<<<<<<<<<<<
@@ -47310,172 +47329,172 @@
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
   __pyx_tuple__74 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_pyx_state); if (unlikely(!__pyx_tuple__74)) __PYX_ERR(1, 3, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__74);
   __Pyx_GIVEREF(__pyx_tuple__74);
   __pyx_codeobj__75 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__74, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__75)) __PYX_ERR(1, 3, __pyx_L1_error)
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":627
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":630
  *     def __dealloc__(self): del self.ptr
  * 
  *     def length(self):             # <<<<<<<<<<<<<<
  *         return map_to_dict(<map[string, int]>self.ptr.fold_map())
  * 
  */
-  __pyx_codeobj__76 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__72, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_cmodules_cyincludes_cyoptimi, __pyx_n_s_length, 627, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__76)) __PYX_ERR(0, 627, __pyx_L1_error)
+  __pyx_codeobj__76 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__72, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_cmodules_cyincludes_cyoptimi, __pyx_n_s_length, 630, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__76)) __PYX_ERR(0, 630, __pyx_L1_error)
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":633
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":636
  *     def kFolds(self): return self.ptr.use_folds
  * 
  *     cpdef report_t reportable(self): return self.state             # <<<<<<<<<<<<<<
  * 
  *     cpdef bool GetHDF5Hashes(self, str path):
  */
-  __pyx_codeobj__77 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__72, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_cmodules_cyincludes_cyoptimi, __pyx_n_s_reportable, 633, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__77)) __PYX_ERR(0, 633, __pyx_L1_error)
+  __pyx_codeobj__77 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__72, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_cmodules_cyincludes_cyoptimi, __pyx_n_s_reportable, 636, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__77)) __PYX_ERR(0, 636, __pyx_L1_error)
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":635
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":638
  *     cpdef report_t reportable(self): return self.state
  * 
  *     cpdef bool GetHDF5Hashes(self, str path):             # <<<<<<<<<<<<<<
  *         if path.endswith(".hdf5"): pass
  *         else: path += ".hdf5"
  */
-  __pyx_tuple__78 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_path); if (unlikely(!__pyx_tuple__78)) __PYX_ERR(0, 635, __pyx_L1_error)
+  __pyx_tuple__78 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_path); if (unlikely(!__pyx_tuple__78)) __PYX_ERR(0, 638, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__78);
   __Pyx_GIVEREF(__pyx_tuple__78);
-  __pyx_codeobj__79 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__78, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_cmodules_cyincludes_cyoptimi, __pyx_n_s_GetHDF5Hashes, 635, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__79)) __PYX_ERR(0, 635, __pyx_L1_error)
+  __pyx_codeobj__79 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__78, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_cmodules_cyincludes_cyoptimi, __pyx_n_s_GetHDF5Hashes, 638, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__79)) __PYX_ERR(0, 638, __pyx_L1_error)
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":656
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":659
  *         return True
  * 
  *     cpdef UseAllHashes(self, list inpt):             # <<<<<<<<<<<<<<
  *         cdef int idx
  *         cdef folds_t fold_hash
  */
-  __pyx_tuple__80 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_inpt); if (unlikely(!__pyx_tuple__80)) __PYX_ERR(0, 656, __pyx_L1_error)
+  __pyx_tuple__80 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_inpt); if (unlikely(!__pyx_tuple__80)) __PYX_ERR(0, 659, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__80);
   __Pyx_GIVEREF(__pyx_tuple__80);
-  __pyx_codeobj__81 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__80, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_cmodules_cyincludes_cyoptimi, __pyx_n_s_UseAllHashes, 656, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__81)) __PYX_ERR(0, 656, __pyx_L1_error)
+  __pyx_codeobj__81 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__80, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_cmodules_cyincludes_cyoptimi, __pyx_n_s_UseAllHashes, 659, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__81)) __PYX_ERR(0, 659, __pyx_L1_error)
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":668
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":671
  *         data.clear()
  * 
  *     cpdef FetchTraining(self, int kfold, int batch_size):             # <<<<<<<<<<<<<<
  *         if self.data.sampletracer is not None: pass
  *         else: self.data.sampletracer = self.sampletracer
  */
-  __pyx_tuple__82 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_kfold_2, __pyx_n_s_batch_size); if (unlikely(!__pyx_tuple__82)) __PYX_ERR(0, 668, __pyx_L1_error)
+  __pyx_tuple__82 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_kfold_2, __pyx_n_s_batch_size); if (unlikely(!__pyx_tuple__82)) __PYX_ERR(0, 671, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__82);
   __Pyx_GIVEREF(__pyx_tuple__82);
-  __pyx_codeobj__83 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__82, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_cmodules_cyincludes_cyoptimi, __pyx_n_s_FetchTraining, 668, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__83)) __PYX_ERR(0, 668, __pyx_L1_error)
+  __pyx_codeobj__83 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__82, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_cmodules_cyincludes_cyoptimi, __pyx_n_s_FetchTraining, 671, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__83)) __PYX_ERR(0, 671, __pyx_L1_error)
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":676
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":679
  *         return self.data.set_batch(kfold, batch_size, b"train")
  * 
  *     cpdef FetchValidation(self, int kfold, int batch_size):             # <<<<<<<<<<<<<<
  *         if self.data.sampletracer is not None: pass
  *         else: self.data.sampletracer = self.sampletracer
  */
-  __pyx_codeobj__84 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__82, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_cmodules_cyincludes_cyoptimi, __pyx_n_s_FetchValidation, 676, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__84)) __PYX_ERR(0, 676, __pyx_L1_error)
+  __pyx_codeobj__84 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__82, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_cmodules_cyincludes_cyoptimi, __pyx_n_s_FetchValidation, 679, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__84)) __PYX_ERR(0, 679, __pyx_L1_error)
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":684
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":687
  *         return self.data.set_batch(kfold, batch_size, b"valid")
  * 
  *     cpdef FetchEvaluation(self, int batch_size):             # <<<<<<<<<<<<<<
  *         if self.data.sampletracer is not None: pass
  *         else: self.data.sampletracer = self.sampletracer
  */
-  __pyx_tuple__85 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_batch_size); if (unlikely(!__pyx_tuple__85)) __PYX_ERR(0, 684, __pyx_L1_error)
+  __pyx_tuple__85 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_batch_size); if (unlikely(!__pyx_tuple__85)) __PYX_ERR(0, 687, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__85);
   __Pyx_GIVEREF(__pyx_tuple__85);
-  __pyx_codeobj__86 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__85, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_cmodules_cyincludes_cyoptimi, __pyx_n_s_FetchEvaluation, 684, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__86)) __PYX_ERR(0, 684, __pyx_L1_error)
+  __pyx_codeobj__86 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__85, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_cmodules_cyincludes_cyoptimi, __pyx_n_s_FetchEvaluation, 687, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__86)) __PYX_ERR(0, 687, __pyx_L1_error)
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":692
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":695
  *         return self.data.set_batch(-1, batch_size, b"eval")
  * 
  *     cpdef UseTheseFolds(self, list inpt): self.ptr.use_folds = <vector[int]>inpt             # <<<<<<<<<<<<<<
  * 
  *     cpdef AddkFold(self, int epoch, int kfold, dict inpt, dict out_map):
  */
-  __pyx_codeobj__87 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__80, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_cmodules_cyincludes_cyoptimi, __pyx_n_s_UseTheseFolds, 692, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__87)) __PYX_ERR(0, 692, __pyx_L1_error)
+  __pyx_codeobj__87 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__80, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_cmodules_cyincludes_cyoptimi, __pyx_n_s_UseTheseFolds, 695, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__87)) __PYX_ERR(0, 695, __pyx_L1_error)
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":694
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":697
  *     cpdef UseTheseFolds(self, list inpt): self.ptr.use_folds = <vector[int]>inpt
  * 
  *     cpdef AddkFold(self, int epoch, int kfold, dict inpt, dict out_map):             # <<<<<<<<<<<<<<
  *         cdef map[string, data_t] map_data = recast(inpt, out_map)
  *         if  self._train: self.ptr.train_epoch_kfold(epoch, kfold, &map_data)
  */
-  __pyx_tuple__88 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_epoch_2, __pyx_n_s_kfold_2, __pyx_n_s_inpt, __pyx_n_s_out_map); if (unlikely(!__pyx_tuple__88)) __PYX_ERR(0, 694, __pyx_L1_error)
+  __pyx_tuple__88 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_epoch_2, __pyx_n_s_kfold_2, __pyx_n_s_inpt, __pyx_n_s_out_map); if (unlikely(!__pyx_tuple__88)) __PYX_ERR(0, 697, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__88);
   __Pyx_GIVEREF(__pyx_tuple__88);
-  __pyx_codeobj__89 = (PyObject*)__Pyx_PyCode_New(5, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__88, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_cmodules_cyincludes_cyoptimi, __pyx_n_s_AddkFold, 694, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__89)) __PYX_ERR(0, 694, __pyx_L1_error)
+  __pyx_codeobj__89 = (PyObject*)__Pyx_PyCode_New(5, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__88, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_cmodules_cyincludes_cyoptimi, __pyx_n_s_AddkFold, 697, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__89)) __PYX_ERR(0, 697, __pyx_L1_error)
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":701
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":704
  *         map_data.clear()
  * 
  *     cpdef FastGraphRecast(self, int epoch, int kfold, list inpt, dict out_map):             # <<<<<<<<<<<<<<
  *         cdef str key
  *         cdef int i, l
  */
-  __pyx_codeobj__90 = (PyObject*)__Pyx_PyCode_New(5, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__88, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_cmodules_cyincludes_cyoptimi, __pyx_n_s_FastGraphRecast, 701, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__90)) __PYX_ERR(0, 701, __pyx_L1_error)
+  __pyx_codeobj__90 = (PyObject*)__Pyx_PyCode_New(5, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__88, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_cmodules_cyincludes_cyoptimi, __pyx_n_s_FastGraphRecast, 704, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__90)) __PYX_ERR(0, 704, __pyx_L1_error)
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":720
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":723
  *             map_data.clear()
  * 
  *     cpdef DumpEpochHDF5(self, int epoch, str path, int kfold):             # <<<<<<<<<<<<<<
  * 
  *         cdef CyEpoch* ep
  */
-  __pyx_tuple__91 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_epoch_2, __pyx_n_s_path, __pyx_n_s_kfold_2); if (unlikely(!__pyx_tuple__91)) __PYX_ERR(0, 720, __pyx_L1_error)
+  __pyx_tuple__91 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_epoch_2, __pyx_n_s_path, __pyx_n_s_kfold_2); if (unlikely(!__pyx_tuple__91)) __PYX_ERR(0, 723, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__91);
   __Pyx_GIVEREF(__pyx_tuple__91);
-  __pyx_codeobj__92 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__91, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_cmodules_cyincludes_cyoptimi, __pyx_n_s_DumpEpochHDF5, 720, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__92)) __PYX_ERR(0, 720, __pyx_L1_error)
+  __pyx_codeobj__92 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__91, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_cmodules_cyincludes_cyoptimi, __pyx_n_s_DumpEpochHDF5, 723, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__92)) __PYX_ERR(0, 723, __pyx_L1_error)
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":746
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":749
  * 
  * 
  *     cpdef RebuildEpochHDF5(self, int epoch, str path, int kfold):             # <<<<<<<<<<<<<<
  *         f = h5py.File(path + str(kfold) + "/epoch_data.hdf5", "r")
  * 
  */
-  __pyx_codeobj__93 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__91, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_cmodules_cyincludes_cyoptimi, __pyx_n_s_RebuildEpochHDF5, 746, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__93)) __PYX_ERR(0, 746, __pyx_L1_error)
+  __pyx_codeobj__93 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__91, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_cmodules_cyincludes_cyoptimi, __pyx_n_s_RebuildEpochHDF5, 749, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__93)) __PYX_ERR(0, 749, __pyx_L1_error)
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":761
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":764
  * 
  * 
  *     cpdef BuildPlots(self, int epoch, str path):             # <<<<<<<<<<<<<<
  *         make_mass_plots(self.ptr.epoch_train, self.ptr.epoch_valid, self.ptr.epoch_test, path)
  *         make_accuracy_plots(self.ptr.epoch_train, self.ptr.epoch_valid, self.ptr.epoch_test, path, &self.state)
  */
-  __pyx_tuple__94 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_epoch_2, __pyx_n_s_path); if (unlikely(!__pyx_tuple__94)) __PYX_ERR(0, 761, __pyx_L1_error)
+  __pyx_tuple__94 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_epoch_2, __pyx_n_s_path); if (unlikely(!__pyx_tuple__94)) __PYX_ERR(0, 764, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__94);
   __Pyx_GIVEREF(__pyx_tuple__94);
-  __pyx_codeobj__95 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__94, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_cmodules_cyincludes_cyoptimi, __pyx_n_s_BuildPlots, 761, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__95)) __PYX_ERR(0, 761, __pyx_L1_error)
+  __pyx_codeobj__95 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__94, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_cmodules_cyincludes_cyoptimi, __pyx_n_s_BuildPlots, 764, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__95)) __PYX_ERR(0, 764, __pyx_L1_error)
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":768
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":771
  *         make_nodes(self.ptr.epoch_train, self.ptr.epoch_valid, self.ptr.epoch_test, path)
  * 
  *     cpdef Purge(self):             # <<<<<<<<<<<<<<
  *         cdef pair[int, CyEpoch*] itr
  *         for itr in self.ptr.epoch_train: itr.second.purge()
  */
-  __pyx_codeobj__96 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__72, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_cmodules_cyincludes_cyoptimi, __pyx_n_s_Purge, 768, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__96)) __PYX_ERR(0, 768, __pyx_L1_error)
+  __pyx_codeobj__96 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__72, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_cmodules_cyincludes_cyoptimi, __pyx_n_s_Purge, 771, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__96)) __PYX_ERR(0, 771, __pyx_L1_error)
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":774
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":777
  *         for itr in self.ptr.epoch_test:  itr.second.purge()
  * 
  *     cpdef SinkInjector(self, model, bar):             # <<<<<<<<<<<<<<
  *         cdef str v
  *         cdef list g
  */
-  __pyx_tuple__97 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_model, __pyx_n_s_bar); if (unlikely(!__pyx_tuple__97)) __PYX_ERR(0, 774, __pyx_L1_error)
+  __pyx_tuple__97 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_model, __pyx_n_s_bar); if (unlikely(!__pyx_tuple__97)) __PYX_ERR(0, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__97);
   __Pyx_GIVEREF(__pyx_tuple__97);
-  __pyx_codeobj__98 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__97, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_cmodules_cyincludes_cyoptimi, __pyx_n_s_SinkInjector, 774, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__98)) __PYX_ERR(0, 774, __pyx_L1_error)
+  __pyx_codeobj__98 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__97, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_cmodules_cyincludes_cyoptimi, __pyx_n_s_SinkInjector, 777, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__98)) __PYX_ERR(0, 777, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
  */
   __pyx_codeobj__99 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__72, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__99)) __PYX_ERR(1, 1, __pyx_L1_error)
@@ -47570,39 +47589,39 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
   __pyx_vtabptr_9AnalysisG_9_cmodules_10cOptimizer_DataLoader = &__pyx_vtable_9AnalysisG_9_cmodules_10cOptimizer_DataLoader;
   __pyx_vtable_9AnalysisG_9_cmodules_10cOptimizer_DataLoader.set_batch = (struct __pyx_obj_9AnalysisG_9_cmodules_10cOptimizer_DataLoader *(*)(struct __pyx_obj_9AnalysisG_9_cmodules_10cOptimizer_DataLoader *, int, int, std::string))__pyx_f_9AnalysisG_9_cmodules_10cOptimizer_10DataLoader_set_batch;
   #if CYTHON_USE_TYPE_SPECS
-  __pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_DataLoader = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_9AnalysisG_9_cmodules_10cOptimizer_DataLoader_spec, NULL); if (unlikely(!__pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_DataLoader)) __PYX_ERR(0, 471, __pyx_L1_error)
-  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_9AnalysisG_9_cmodules_10cOptimizer_DataLoader_spec, __pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_DataLoader) < 0) __PYX_ERR(0, 471, __pyx_L1_error)
+  __pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_DataLoader = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_9AnalysisG_9_cmodules_10cOptimizer_DataLoader_spec, NULL); if (unlikely(!__pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_DataLoader)) __PYX_ERR(0, 474, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_9AnalysisG_9_cmodules_10cOptimizer_DataLoader_spec, __pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_DataLoader) < 0) __PYX_ERR(0, 474, __pyx_L1_error)
   #else
   __pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_DataLoader = &__pyx_type_9AnalysisG_9_cmodules_10cOptimizer_DataLoader;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   #endif
   #if !CYTHON_USE_TYPE_SPECS
-  if (__Pyx_PyType_Ready(__pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_DataLoader) < 0) __PYX_ERR(0, 471, __pyx_L1_error)
+  if (__Pyx_PyType_Ready(__pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_DataLoader) < 0) __PYX_ERR(0, 474, __pyx_L1_error)
   #endif
   #if PY_MAJOR_VERSION < 3
   __pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_DataLoader->tp_print = 0;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_DataLoader->tp_dictoffset && __pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_DataLoader->tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_DataLoader->tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
   #endif
-  if (__Pyx_SetVtable(__pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_DataLoader, __pyx_vtabptr_9AnalysisG_9_cmodules_10cOptimizer_DataLoader) < 0) __PYX_ERR(0, 471, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_DataLoader, __pyx_vtabptr_9AnalysisG_9_cmodules_10cOptimizer_DataLoader) < 0) __PYX_ERR(0, 474, __pyx_L1_error)
   #if !CYTHON_COMPILING_IN_LIMITED_API
-  if (__Pyx_MergeVtables(__pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_DataLoader) < 0) __PYX_ERR(0, 471, __pyx_L1_error)
+  if (__Pyx_MergeVtables(__pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_DataLoader) < 0) __PYX_ERR(0, 474, __pyx_L1_error)
   #endif
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_DataLoader, (PyObject *) __pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_DataLoader) < 0) __PYX_ERR(0, 471, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_DataLoader, (PyObject *) __pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_DataLoader) < 0) __PYX_ERR(0, 474, __pyx_L1_error)
   #if !CYTHON_COMPILING_IN_LIMITED_API
-  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_DataLoader) < 0) __PYX_ERR(0, 471, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_DataLoader) < 0) __PYX_ERR(0, 474, __pyx_L1_error)
   #endif
   __pyx_vtabptr_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer = &__pyx_vtable_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer;
   __pyx_vtable_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer.reportable = (struct __pyx_t_11cyoptimizer_report_t (*)(struct __pyx_obj_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer *, int __pyx_skip_dispatch))__pyx_f_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_reportable;
   __pyx_vtable_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer.GetHDF5Hashes = (bool (*)(struct __pyx_obj_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer *, PyObject *, int __pyx_skip_dispatch))__pyx_f_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_GetHDF5Hashes;
   __pyx_vtable_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer.UseAllHashes = (PyObject *(*)(struct __pyx_obj_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer *, PyObject *, int __pyx_skip_dispatch))__pyx_f_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_UseAllHashes;
   __pyx_vtable_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer.FetchTraining = (PyObject *(*)(struct __pyx_obj_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer *, int, int, int __pyx_skip_dispatch))__pyx_f_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_FetchTraining;
   __pyx_vtable_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer.FetchValidation = (PyObject *(*)(struct __pyx_obj_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer *, int, int, int __pyx_skip_dispatch))__pyx_f_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_FetchValidation;
@@ -47612,39 +47631,39 @@
   __pyx_vtable_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer.FastGraphRecast = (PyObject *(*)(struct __pyx_obj_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer *, int, int, PyObject *, PyObject *, int __pyx_skip_dispatch))__pyx_f_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_FastGraphRecast;
   __pyx_vtable_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer.DumpEpochHDF5 = (PyObject *(*)(struct __pyx_obj_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer *, int, PyObject *, int, int __pyx_skip_dispatch))__pyx_f_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_DumpEpochHDF5;
   __pyx_vtable_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer.RebuildEpochHDF5 = (PyObject *(*)(struct __pyx_obj_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer *, int, PyObject *, int, int __pyx_skip_dispatch))__pyx_f_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_RebuildEpochHDF5;
   __pyx_vtable_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer.BuildPlots = (PyObject *(*)(struct __pyx_obj_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer *, int, PyObject *, int __pyx_skip_dispatch))__pyx_f_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_BuildPlots;
   __pyx_vtable_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer.Purge = (PyObject *(*)(struct __pyx_obj_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer *, int __pyx_skip_dispatch))__pyx_f_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_Purge;
   __pyx_vtable_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer.SinkInjector = (PyObject *(*)(struct __pyx_obj_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer *, PyObject *, PyObject *, int __pyx_skip_dispatch))__pyx_f_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_SinkInjector;
   #if CYTHON_USE_TYPE_SPECS
-  __pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer_spec, NULL); if (unlikely(!__pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer)) __PYX_ERR(0, 601, __pyx_L1_error)
-  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer_spec, __pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer) < 0) __PYX_ERR(0, 601, __pyx_L1_error)
+  __pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer_spec, NULL); if (unlikely(!__pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer)) __PYX_ERR(0, 604, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer_spec, __pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer) < 0) __PYX_ERR(0, 604, __pyx_L1_error)
   #else
   __pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer = &__pyx_type_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   #endif
   #if !CYTHON_USE_TYPE_SPECS
-  if (__Pyx_PyType_Ready(__pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer) < 0) __PYX_ERR(0, 601, __pyx_L1_error)
+  if (__Pyx_PyType_Ready(__pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer) < 0) __PYX_ERR(0, 604, __pyx_L1_error)
   #endif
   #if PY_MAJOR_VERSION < 3
   __pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer->tp_print = 0;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer->tp_dictoffset && __pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer->tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer->tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
   #endif
-  if (__Pyx_SetVtable(__pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer, __pyx_vtabptr_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer) < 0) __PYX_ERR(0, 601, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer, __pyx_vtabptr_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer) < 0) __PYX_ERR(0, 604, __pyx_L1_error)
   #if !CYTHON_COMPILING_IN_LIMITED_API
-  if (__Pyx_MergeVtables(__pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer) < 0) __PYX_ERR(0, 601, __pyx_L1_error)
+  if (__Pyx_MergeVtables(__pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer) < 0) __PYX_ERR(0, 604, __pyx_L1_error)
   #endif
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_cOptimizer, (PyObject *) __pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer) < 0) __PYX_ERR(0, 601, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_cOptimizer, (PyObject *) __pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer) < 0) __PYX_ERR(0, 604, __pyx_L1_error)
   #if !CYTHON_COMPILING_IN_LIMITED_API
-  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer) < 0) __PYX_ERR(0, 601, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer) < 0) __PYX_ERR(0, 604, __pyx_L1_error)
   #endif
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
@@ -48175,206 +48194,206 @@
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
   __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9AnalysisG_9_cmodules_10cOptimizer_10DataLoader_15__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_DataLoader___setstate_cython, NULL, __pyx_n_s_AnalysisG__cmodules_cOptimizer, __pyx_d, ((PyObject *)__pyx_codeobj__75)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 3, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_setstate_cython, __pyx_t_2) < 0) __PYX_ERR(1, 3, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":627
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":630
  *     def __dealloc__(self): del self.ptr
  * 
  *     def length(self):             # <<<<<<<<<<<<<<
  *         return map_to_dict(<map[string, int]>self.ptr.fold_map())
  * 
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_7length, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_cOptimizer_length, NULL, __pyx_n_s_AnalysisG__cmodules_cOptimizer, __pyx_d, ((PyObject *)__pyx_codeobj__76)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 627, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_7length, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_cOptimizer_length, NULL, __pyx_n_s_AnalysisG__cmodules_cOptimizer, __pyx_d, ((PyObject *)__pyx_codeobj__76)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 630, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer, __pyx_n_s_length, __pyx_t_2) < 0) __PYX_ERR(0, 627, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer, __pyx_n_s_length, __pyx_t_2) < 0) __PYX_ERR(0, 630, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer);
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":633
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":636
  *     def kFolds(self): return self.ptr.use_folds
  * 
  *     cpdef report_t reportable(self): return self.state             # <<<<<<<<<<<<<<
  * 
  *     cpdef bool GetHDF5Hashes(self, str path):
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_9reportable, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_cOptimizer_reportable, NULL, __pyx_n_s_AnalysisG__cmodules_cOptimizer, __pyx_d, ((PyObject *)__pyx_codeobj__77)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 633, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_9reportable, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_cOptimizer_reportable, NULL, __pyx_n_s_AnalysisG__cmodules_cOptimizer, __pyx_d, ((PyObject *)__pyx_codeobj__77)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 636, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer, __pyx_n_s_reportable, __pyx_t_2) < 0) __PYX_ERR(0, 633, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer, __pyx_n_s_reportable, __pyx_t_2) < 0) __PYX_ERR(0, 636, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer);
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":635
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":638
  *     cpdef report_t reportable(self): return self.state
  * 
  *     cpdef bool GetHDF5Hashes(self, str path):             # <<<<<<<<<<<<<<
  *         if path.endswith(".hdf5"): pass
  *         else: path += ".hdf5"
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_11GetHDF5Hashes, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_cOptimizer_GetHDF5Hashes, NULL, __pyx_n_s_AnalysisG__cmodules_cOptimizer, __pyx_d, ((PyObject *)__pyx_codeobj__79)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 635, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_11GetHDF5Hashes, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_cOptimizer_GetHDF5Hashes, NULL, __pyx_n_s_AnalysisG__cmodules_cOptimizer, __pyx_d, ((PyObject *)__pyx_codeobj__79)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 638, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer, __pyx_n_s_GetHDF5Hashes, __pyx_t_2) < 0) __PYX_ERR(0, 635, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer, __pyx_n_s_GetHDF5Hashes, __pyx_t_2) < 0) __PYX_ERR(0, 638, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer);
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":656
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":659
  *         return True
  * 
  *     cpdef UseAllHashes(self, list inpt):             # <<<<<<<<<<<<<<
  *         cdef int idx
  *         cdef folds_t fold_hash
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_13UseAllHashes, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_cOptimizer_UseAllHashes, NULL, __pyx_n_s_AnalysisG__cmodules_cOptimizer, __pyx_d, ((PyObject *)__pyx_codeobj__81)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 656, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_13UseAllHashes, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_cOptimizer_UseAllHashes, NULL, __pyx_n_s_AnalysisG__cmodules_cOptimizer, __pyx_d, ((PyObject *)__pyx_codeobj__81)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 659, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer, __pyx_n_s_UseAllHashes, __pyx_t_2) < 0) __PYX_ERR(0, 656, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer, __pyx_n_s_UseAllHashes, __pyx_t_2) < 0) __PYX_ERR(0, 659, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer);
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":668
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":671
  *         data.clear()
  * 
  *     cpdef FetchTraining(self, int kfold, int batch_size):             # <<<<<<<<<<<<<<
  *         if self.data.sampletracer is not None: pass
  *         else: self.data.sampletracer = self.sampletracer
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_15FetchTraining, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_cOptimizer_FetchTraining, NULL, __pyx_n_s_AnalysisG__cmodules_cOptimizer, __pyx_d, ((PyObject *)__pyx_codeobj__83)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 668, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_15FetchTraining, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_cOptimizer_FetchTraining, NULL, __pyx_n_s_AnalysisG__cmodules_cOptimizer, __pyx_d, ((PyObject *)__pyx_codeobj__83)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 671, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer, __pyx_n_s_FetchTraining, __pyx_t_2) < 0) __PYX_ERR(0, 668, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer, __pyx_n_s_FetchTraining, __pyx_t_2) < 0) __PYX_ERR(0, 671, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer);
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":676
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":679
  *         return self.data.set_batch(kfold, batch_size, b"train")
  * 
  *     cpdef FetchValidation(self, int kfold, int batch_size):             # <<<<<<<<<<<<<<
  *         if self.data.sampletracer is not None: pass
  *         else: self.data.sampletracer = self.sampletracer
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_17FetchValidation, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_cOptimizer_FetchValidation, NULL, __pyx_n_s_AnalysisG__cmodules_cOptimizer, __pyx_d, ((PyObject *)__pyx_codeobj__84)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 676, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_17FetchValidation, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_cOptimizer_FetchValidation, NULL, __pyx_n_s_AnalysisG__cmodules_cOptimizer, __pyx_d, ((PyObject *)__pyx_codeobj__84)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 679, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer, __pyx_n_s_FetchValidation, __pyx_t_2) < 0) __PYX_ERR(0, 676, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer, __pyx_n_s_FetchValidation, __pyx_t_2) < 0) __PYX_ERR(0, 679, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer);
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":684
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":687
  *         return self.data.set_batch(kfold, batch_size, b"valid")
  * 
  *     cpdef FetchEvaluation(self, int batch_size):             # <<<<<<<<<<<<<<
  *         if self.data.sampletracer is not None: pass
  *         else: self.data.sampletracer = self.sampletracer
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_19FetchEvaluation, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_cOptimizer_FetchEvaluation, NULL, __pyx_n_s_AnalysisG__cmodules_cOptimizer, __pyx_d, ((PyObject *)__pyx_codeobj__86)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 684, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_19FetchEvaluation, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_cOptimizer_FetchEvaluation, NULL, __pyx_n_s_AnalysisG__cmodules_cOptimizer, __pyx_d, ((PyObject *)__pyx_codeobj__86)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 687, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer, __pyx_n_s_FetchEvaluation, __pyx_t_2) < 0) __PYX_ERR(0, 684, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer, __pyx_n_s_FetchEvaluation, __pyx_t_2) < 0) __PYX_ERR(0, 687, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer);
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":692
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":695
  *         return self.data.set_batch(-1, batch_size, b"eval")
  * 
  *     cpdef UseTheseFolds(self, list inpt): self.ptr.use_folds = <vector[int]>inpt             # <<<<<<<<<<<<<<
  * 
  *     cpdef AddkFold(self, int epoch, int kfold, dict inpt, dict out_map):
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_21UseTheseFolds, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_cOptimizer_UseTheseFolds, NULL, __pyx_n_s_AnalysisG__cmodules_cOptimizer, __pyx_d, ((PyObject *)__pyx_codeobj__87)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 692, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_21UseTheseFolds, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_cOptimizer_UseTheseFolds, NULL, __pyx_n_s_AnalysisG__cmodules_cOptimizer, __pyx_d, ((PyObject *)__pyx_codeobj__87)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 695, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer, __pyx_n_s_UseTheseFolds, __pyx_t_2) < 0) __PYX_ERR(0, 692, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer, __pyx_n_s_UseTheseFolds, __pyx_t_2) < 0) __PYX_ERR(0, 695, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer);
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":694
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":697
  *     cpdef UseTheseFolds(self, list inpt): self.ptr.use_folds = <vector[int]>inpt
  * 
  *     cpdef AddkFold(self, int epoch, int kfold, dict inpt, dict out_map):             # <<<<<<<<<<<<<<
  *         cdef map[string, data_t] map_data = recast(inpt, out_map)
  *         if  self._train: self.ptr.train_epoch_kfold(epoch, kfold, &map_data)
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_23AddkFold, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_cOptimizer_AddkFold, NULL, __pyx_n_s_AnalysisG__cmodules_cOptimizer, __pyx_d, ((PyObject *)__pyx_codeobj__89)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 694, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_23AddkFold, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_cOptimizer_AddkFold, NULL, __pyx_n_s_AnalysisG__cmodules_cOptimizer, __pyx_d, ((PyObject *)__pyx_codeobj__89)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 697, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer, __pyx_n_s_AddkFold, __pyx_t_2) < 0) __PYX_ERR(0, 694, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer, __pyx_n_s_AddkFold, __pyx_t_2) < 0) __PYX_ERR(0, 697, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer);
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":701
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":704
  *         map_data.clear()
  * 
  *     cpdef FastGraphRecast(self, int epoch, int kfold, list inpt, dict out_map):             # <<<<<<<<<<<<<<
  *         cdef str key
  *         cdef int i, l
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_25FastGraphRecast, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_cOptimizer_FastGraphRecast, NULL, __pyx_n_s_AnalysisG__cmodules_cOptimizer, __pyx_d, ((PyObject *)__pyx_codeobj__90)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 701, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_25FastGraphRecast, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_cOptimizer_FastGraphRecast, NULL, __pyx_n_s_AnalysisG__cmodules_cOptimizer, __pyx_d, ((PyObject *)__pyx_codeobj__90)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 704, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer, __pyx_n_s_FastGraphRecast, __pyx_t_2) < 0) __PYX_ERR(0, 701, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer, __pyx_n_s_FastGraphRecast, __pyx_t_2) < 0) __PYX_ERR(0, 704, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer);
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":720
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":723
  *             map_data.clear()
  * 
  *     cpdef DumpEpochHDF5(self, int epoch, str path, int kfold):             # <<<<<<<<<<<<<<
  * 
  *         cdef CyEpoch* ep
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_27DumpEpochHDF5, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_cOptimizer_DumpEpochHDF5, NULL, __pyx_n_s_AnalysisG__cmodules_cOptimizer, __pyx_d, ((PyObject *)__pyx_codeobj__92)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 720, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_27DumpEpochHDF5, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_cOptimizer_DumpEpochHDF5, NULL, __pyx_n_s_AnalysisG__cmodules_cOptimizer, __pyx_d, ((PyObject *)__pyx_codeobj__92)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 723, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer, __pyx_n_s_DumpEpochHDF5, __pyx_t_2) < 0) __PYX_ERR(0, 720, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer, __pyx_n_s_DumpEpochHDF5, __pyx_t_2) < 0) __PYX_ERR(0, 723, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer);
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":746
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":749
  * 
  * 
  *     cpdef RebuildEpochHDF5(self, int epoch, str path, int kfold):             # <<<<<<<<<<<<<<
  *         f = h5py.File(path + str(kfold) + "/epoch_data.hdf5", "r")
  * 
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_29RebuildEpochHDF5, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_cOptimizer_RebuildEpochHDF5, NULL, __pyx_n_s_AnalysisG__cmodules_cOptimizer, __pyx_d, ((PyObject *)__pyx_codeobj__93)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 746, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_29RebuildEpochHDF5, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_cOptimizer_RebuildEpochHDF5, NULL, __pyx_n_s_AnalysisG__cmodules_cOptimizer, __pyx_d, ((PyObject *)__pyx_codeobj__93)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 749, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer, __pyx_n_s_RebuildEpochHDF5, __pyx_t_2) < 0) __PYX_ERR(0, 746, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer, __pyx_n_s_RebuildEpochHDF5, __pyx_t_2) < 0) __PYX_ERR(0, 749, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer);
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":761
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":764
  * 
  * 
  *     cpdef BuildPlots(self, int epoch, str path):             # <<<<<<<<<<<<<<
  *         make_mass_plots(self.ptr.epoch_train, self.ptr.epoch_valid, self.ptr.epoch_test, path)
  *         make_accuracy_plots(self.ptr.epoch_train, self.ptr.epoch_valid, self.ptr.epoch_test, path, &self.state)
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_31BuildPlots, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_cOptimizer_BuildPlots, NULL, __pyx_n_s_AnalysisG__cmodules_cOptimizer, __pyx_d, ((PyObject *)__pyx_codeobj__95)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 761, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_31BuildPlots, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_cOptimizer_BuildPlots, NULL, __pyx_n_s_AnalysisG__cmodules_cOptimizer, __pyx_d, ((PyObject *)__pyx_codeobj__95)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 764, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer, __pyx_n_s_BuildPlots, __pyx_t_2) < 0) __PYX_ERR(0, 761, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer, __pyx_n_s_BuildPlots, __pyx_t_2) < 0) __PYX_ERR(0, 764, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer);
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":768
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":771
  *         make_nodes(self.ptr.epoch_train, self.ptr.epoch_valid, self.ptr.epoch_test, path)
  * 
  *     cpdef Purge(self):             # <<<<<<<<<<<<<<
  *         cdef pair[int, CyEpoch*] itr
  *         for itr in self.ptr.epoch_train: itr.second.purge()
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_33Purge, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_cOptimizer_Purge, NULL, __pyx_n_s_AnalysisG__cmodules_cOptimizer, __pyx_d, ((PyObject *)__pyx_codeobj__96)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 768, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_33Purge, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_cOptimizer_Purge, NULL, __pyx_n_s_AnalysisG__cmodules_cOptimizer, __pyx_d, ((PyObject *)__pyx_codeobj__96)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 771, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer, __pyx_n_s_Purge, __pyx_t_2) < 0) __PYX_ERR(0, 768, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer, __pyx_n_s_Purge, __pyx_t_2) < 0) __PYX_ERR(0, 771, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer);
 
-  /* "src/cmodules/cyincludes/cyoptimizer.pyx":774
+  /* "src/cmodules/cyincludes/cyoptimizer.pyx":777
  *         for itr in self.ptr.epoch_test:  itr.second.purge()
  * 
  *     cpdef SinkInjector(self, model, bar):             # <<<<<<<<<<<<<<
  *         cdef str v
  *         cdef list g
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_35SinkInjector, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_cOptimizer_SinkInjector, NULL, __pyx_n_s_AnalysisG__cmodules_cOptimizer, __pyx_d, ((PyObject *)__pyx_codeobj__98)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 774, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9AnalysisG_9_cmodules_10cOptimizer_10cOptimizer_35SinkInjector, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_cOptimizer_SinkInjector, NULL, __pyx_n_s_AnalysisG__cmodules_cOptimizer, __pyx_d, ((PyObject *)__pyx_codeobj__98)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer, __pyx_n_s_SinkInjector, __pyx_t_2) < 0) __PYX_ERR(0, 774, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer, __pyx_n_s_SinkInjector, __pyx_t_2) < 0) __PYX_ERR(0, 777, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_9AnalysisG_9_cmodules_10cOptimizer_cOptimizer);
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
@@ -51326,28 +51345,14 @@
         if (unlikely(!retval))
             return -1;
         Py_DECREF(retval);
     }
     return 0;
 }
 
-/* PyObjectSetAttrStr */
-#if CYTHON_USE_TYPE_SLOTS
-static CYTHON_INLINE int __Pyx_PyObject_SetAttrStr(PyObject* obj, PyObject* attr_name, PyObject* value) {
-    PyTypeObject* tp = Py_TYPE(obj);
-    if (likely(tp->tp_setattro))
-        return tp->tp_setattro(obj, attr_name, value);
-#if PY_MAJOR_VERSION < 3
-    if (likely(tp->tp_setattr))
-        return tp->tp_setattr(obj, PyString_AS_STRING(attr_name), value);
-#endif
-    return PyObject_SetAttr(obj, attr_name, value);
-}
-#endif
-
 /* KeywordStringCheck */
 static int __Pyx_CheckKeywordStrings(
     PyObject *kw,
     const char* function_name,
     int kw_allowed)
 {
     PyObject* key = 0;
@@ -51559,14 +51564,28 @@
     if (likely(PyExceptionClass_Check(err))) {
         return __Pyx_inner_PyErr_GivenExceptionMatches2(err, exc_type1, exc_type2);
     }
     return (PyErr_GivenExceptionMatches(err, exc_type1) || PyErr_GivenExceptionMatches(err, exc_type2));
 }
 #endif
 
+/* PyObjectSetAttrStr */
+#if CYTHON_USE_TYPE_SLOTS
+static CYTHON_INLINE int __Pyx_PyObject_SetAttrStr(PyObject* obj, PyObject* attr_name, PyObject* value) {
+    PyTypeObject* tp = Py_TYPE(obj);
+    if (likely(tp->tp_setattro))
+        return tp->tp_setattro(obj, attr_name, value);
+#if PY_MAJOR_VERSION < 3
+    if (likely(tp->tp_setattr))
+        return tp->tp_setattr(obj, PyString_AS_STRING(attr_name), value);
+#endif
+    return PyObject_SetAttr(obj, attr_name, value);
+}
+#endif
+
 /* FixUpExtensionType */
 #if CYTHON_USE_TYPE_SPECS
 static int __Pyx_fix_up_extension_type_from_spec(PyType_Spec *spec, PyTypeObject *type) {
 #if PY_VERSION_HEX > 0x030900B1 || CYTHON_COMPILING_IN_LIMITED_API
     CYTHON_UNUSED_VAR(spec);
     CYTHON_UNUSED_VAR(type);
 #else
```

### Comparing `analysisg-4.5.7/src/cmodules/cyincludes/cyoptimizer.pxd` & `analysisg-4.5.8/src/cmodules/cyincludes/cyoptimizer.pxd`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/cmodules/cyincludes/cyoptimizer.pyx` & `analysisg-4.5.8/src/cmodules/cyincludes/cyoptimizer.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -136,16 +136,18 @@
 
             try: xData += va_t[file_n][x]["xData"]
             except KeyError: pass
             try: xData += ev_t[file_n][x]["xData"]
             except KeyError: pass
             try: xData += tr_t[file_n][x]["xData"]
             except KeyError: pass
-            tmpl["Histograms"] += [TH1F(**{"Title" : "truth", "xData" : xData})]
+
+            tmpl["Histogram"] = TH1F(**{"Title" : "truth", "xData" : xData})
             tmpl["yLogarithmic"] = True
+            tmpl["Stack"] = True
             th = TH1F(**tmpl)
             th.SaveFigure()
             del th
 
 cdef dict collapse_points(map[string, vector[point_t]]* tmp, int epoch, dict lines, str mode, report_t* state, str metric):
     cdef pair[string, vector[point_t]]itv
     cdef point_t pnt
@@ -238,16 +240,16 @@
         lines = collapse_points(&tmp_te, epoch, lines, "evaluation", state, "acc")
 
     for var_name in lines:
         for mode in lines[var_name]: lines[var_name][mode] = TLine(**lines[var_name][mode])
         tmpl = template_tline(path, "Epoch", "Accuracy", "Achieved Accuracy of " + var_name)
         tmpl["Filename"] = var_name + "_accuracy"
         tmpl["Lines"] = list(lines[var_name].values())
+        tmpl["yMax"] = 100
         tl = TLine(**tmpl)
-        tl.yMax = 100
         tl.SaveFigure()
         del tl
         del tmpl
     del lines
     del folds
     tmp_tr.clear()
     tmp_va.clear()
@@ -310,14 +312,15 @@
     tmp_va.clear()
     tmp_te.clear()
 
 cdef dict make_roc_curve(map[string, roc_t]* roc_, dict lines, str mode):
     cdef pair[string, roc_t] its
 
     for its in dereference(roc_):
+        if not its.second.pred.size(): continue
         pred = torch.tensor(its.second.pred)
         dereference(roc_)[its.first].pred.clear()
 
         tru = torch.tensor(its.second.truth, dtype = torch.long).view(-1)
         dereference(roc_)[its.first].truth.clear()
 
         roc = MulticlassROC(**{"num_classes": pred.size()[1], "thresholds" : None})
@@ -326,16 +329,16 @@
         auc = MulticlassAUROC(**{"num_classes": pred.size()[1], "thresholds" : None, "average" : None})
         auc_ = auc(pred, tru).view(-1)
 
         del tru
         del pred
         del thres
         for cls in range(len(fpr)):
-            try: dereference(roc_)[its.first].auc[cls+1] = auc_[cls].item()
-            except IndexError: pass
+            try: dereference(roc_)[its.first].auc[cls] = auc_[cls].item()
+            except IndexError: continue
             name = "ROC Curve: "+ env(its.first) + " classification - " + str(cls)
             if name not in lines: lines[name] = []
             lines[name] += [TLine(**{"xData" : fpr[cls].tolist(), "yData" : tpr[cls].tolist(), "Title" : mode})]
     return lines
 
 cdef void make_auc_curve(map[string, roc_t]* roc_, map[string, vector[point_t]]* auc_):
     cdef pair[string, roc_t] its
```

### Comparing `analysisg-4.5.7/src/cmodules/cyincludes/cyparticle.cpp` & `analysisg-4.5.8/src/cmodules/cyincludes/cyparticle.cpp`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/cmodules/cyincludes/cyparticle.pxd` & `analysisg-4.5.8/src/cmodules/cyincludes/cyparticle.pxd`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/cmodules/cyincludes/cyparticle.pyx` & `analysisg-4.5.8/src/cmodules/cyincludes/cyparticle.pyx`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/cmodules/cyincludes/cyplotstruct.pxd` & `analysisg-4.5.8/src/cmodules/cyincludes/cyplotstruct.pxd`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/cmodules/cyincludes/cyplotting.cpp` & `analysisg-4.5.8/src/cmodules/cyincludes/cyplotting.cpp`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/cmodules/cyincludes/cyplotting.pyx` & `analysisg-4.5.8/src/cmodules/cyincludes/cyplotting.pyx`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/cmodules/cyincludes/cyrunner.cpp` & `analysisg-4.5.8/src/cmodules/cyincludes/cyrunner.cpp`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/cmodules/cyincludes/cyrunner.pxd` & `analysisg-4.5.8/src/cmodules/cyincludes/cyrunner.pxd`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/cmodules/cyincludes/cyrunner.pyx` & `analysisg-4.5.8/src/cmodules/cyincludes/cyrunner.pyx`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/cmodules/cyincludes/cysampletracer.cpp` & `analysisg-4.5.8/src/cmodules/cyincludes/cysampletracer.cpp`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/cmodules/cyincludes/cysampletracer.pxd` & `analysisg-4.5.8/src/cmodules/cyincludes/cysampletracer.pxd`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/cmodules/cyincludes/cysampletracer.pyx` & `analysisg-4.5.8/src/cmodules/cyincludes/cysampletracer.pyx`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/cmodules/cyincludes/cyselection.cpp` & `analysisg-4.5.8/src/cmodules/cyincludes/cyselection.cpp`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/cmodules/cyincludes/cyselection.pxd` & `analysisg-4.5.8/src/cmodules/cyincludes/cyselection.pxd`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/cmodules/cyincludes/cyselection.pyx` & `analysisg-4.5.8/src/cmodules/cyincludes/cyselection.pyx`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/cmodules/cyincludes/cytooling.cpp` & `analysisg-4.5.8/src/cmodules/cyincludes/cytooling.cpp`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/cmodules/cyincludes/cytooling.pyx` & `analysisg-4.5.8/src/cmodules/cyincludes/cytooling.pyx`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/cmodules/cyincludes/cytools.pxd` & `analysisg-4.5.8/src/cmodules/cyincludes/cytools.pxd`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/cmodules/cyincludes/cytypes.pxd` & `analysisg-4.5.8/src/cmodules/cyincludes/cytypes.pxd`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/cmodules/cyincludes/cywrapping.cpp` & `analysisg-4.5.8/src/cmodules/cyincludes/cywrapping.cpp`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/cmodules/cyincludes/cywrapping.pxd` & `analysisg-4.5.8/src/cmodules/cyincludes/cywrapping.pxd`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/cmodules/cyincludes/cywrapping.pyx` & `analysisg-4.5.8/src/cmodules/cyincludes/cywrapping.pyx`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/cmodules/epoch/epoch.cxx` & `analysisg-4.5.8/src/cmodules/epoch/epoch.cxx`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/cmodules/epoch/epoch.h` & `analysisg-4.5.8/src/cmodules/epoch/epoch.h`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/cmodules/event/event.cxx` & `analysisg-4.5.8/src/cmodules/event/event.cxx`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/cmodules/event/event.h` & `analysisg-4.5.8/src/cmodules/event/event.h`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/cmodules/graph/graph.cxx` & `analysisg-4.5.8/src/cmodules/graph/graph.cxx`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/cmodules/graph/graph.h` & `analysisg-4.5.8/src/cmodules/graph/graph.h`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/cmodules/metadata/metadata.cxx` & `analysisg-4.5.8/src/cmodules/metadata/metadata.cxx`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/cmodules/metadata/metadata.h` & `analysisg-4.5.8/src/cmodules/metadata/metadata.h`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/cmodules/optimizer/optimizer.cxx` & `analysisg-4.5.8/src/cmodules/optimizer/optimizer.cxx`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/cmodules/optimizer/optimizer.h` & `analysisg-4.5.8/src/cmodules/optimizer/optimizer.h`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/cmodules/particle/particle.cxx` & `analysisg-4.5.8/src/cmodules/particle/particle.cxx`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/cmodules/particle/particle.h` & `analysisg-4.5.8/src/cmodules/particle/particle.h`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/cmodules/plotting/plotting.h` & `analysisg-4.5.8/src/cmodules/plotting/plotting.h`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/cmodules/root/root.cxx` & `analysisg-4.5.8/src/cmodules/root/root.cxx`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/cmodules/root/root.h` & `analysisg-4.5.8/src/cmodules/root/root.h`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/cmodules/sampletracer/sampletracer.cxx` & `analysisg-4.5.8/src/cmodules/sampletracer/sampletracer.cxx`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/cmodules/sampletracer/sampletracer.h` & `analysisg-4.5.8/src/cmodules/sampletracer/sampletracer.h`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/cmodules/selection/selection.cxx` & `analysisg-4.5.8/src/cmodules/selection/selection.cxx`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/src/cmodules/selection/selection.h` & `analysisg-4.5.8/src/cmodules/selection/selection.h`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/test/test_ami.py` & `analysisg-4.5.8/test/test_ami.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/test/test_analysis.py` & `analysisg-4.5.8/test/test_analysis.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/test/test_cache_flush.py` & `analysisg-4.5.8/test/test_cache_flush.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/test/test_event_generator.py` & `analysisg-4.5.8/test/test_event_generator.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/test/test_event_templates.py` & `analysisg-4.5.8/test/test_event_templates.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/test/test_graph.py` & `analysisg-4.5.8/test/test_graph.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/test/test_graph_generator.py` & `analysisg-4.5.8/test/test_graph_generator.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/test/test_graph_templates.py` & `analysisg-4.5.8/test/test_graph_templates.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/test/test_imports.py` & `analysisg-4.5.8/test/test_imports.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/test/test_io.py` & `analysisg-4.5.8/test/test_io.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/test/test_machine_learning.py` & `analysisg-4.5.8/test/test_machine_learning.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/test/test_memory.py` & `analysisg-4.5.8/test/test_memory.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/test/test_notification.py` & `analysisg-4.5.8/test/test_notification.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/test/test_nusol.py` & `analysisg-4.5.8/test/test_nusol.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/test/test_nusol_versions.py` & `analysisg-4.5.8/test/test_nusol_versions.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/test/test_operators.py` & `analysisg-4.5.8/test/test_operators.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/test/test_particle_template.py` & `analysisg-4.5.8/test/test_particle_template.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/test/test_physics.py` & `analysisg-4.5.8/test/test_physics.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/test/test_selection_generator.py` & `analysisg-4.5.8/test/test_selection_generator.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/test/test_selection_template.py` & `analysisg-4.5.8/test/test_selection_template.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/test/test_submission.py` & `analysisg-4.5.8/test/test_submission.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/test/test_tools.py` & `analysisg-4.5.8/test/test_tools.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/test/test_tracer.py` & `analysisg-4.5.8/test/test_tracer.py`

 * *Files identical despite different names*

### Comparing `analysisg-4.5.7/test/test_transform.py` & `analysisg-4.5.8/test/test_transform.py`

 * *Files identical despite different names*

