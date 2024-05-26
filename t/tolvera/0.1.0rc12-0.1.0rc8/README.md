# Comparing `tmp/tolvera-0.1.0rc12.tar.gz` & `tmp/tolvera-0.1.0rc8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tolvera-0.1.0rc12.tar", max compression
+gzip compressed data, was "tolvera-0.1.0rc8.tar", max compression
```

## Comparing `tolvera-0.1.0rc12.tar` & `tolvera-0.1.0rc8.tar`

### file list

```diff
@@ -1,39 +1,46 @@
--rw-r--r--   0        0        0    34523 2023-11-23 15:54:16.427339 tolvera-0.1.0rc12/LICENSE
--rw-r--r--   0        0        0     8913 2024-05-16 16:07:05.231292 tolvera-0.1.0rc12/README.md
--rw-r--r--   0        0        0     1407 2024-05-26 22:22:35.883651 tolvera-0.1.0rc12/pyproject.toml
--rw-r--r--   0        0        0      290 2024-05-26 22:20:08.626815 tolvera-0.1.0rc12/src/tolvera/__init__.py
--rw-r--r--   0        0        0     1400 2024-05-16 16:07:04.226491 tolvera-0.1.0rc12/src/tolvera/__main__.py
--rw-r--r--   0        0        0     8125 2024-05-26 08:23:11.170833 tolvera-0.1.0rc12/src/tolvera/context.py
--rw-r--r--   0        0        0     5792 2024-05-16 16:07:05.231724 tolvera-0.1.0rc12/src/tolvera/cv.py
--rw-r--r--   0        0        0    34367 2024-05-16 16:07:04.227212 tolvera-0.1.0rc12/src/tolvera/iml.py
--rw-r--r--   0        0        0      111 2024-05-16 16:07:04.227370 tolvera-0.1.0rc12/src/tolvera/mp/__init__.py
--rw-r--r--   0        0        0     3543 2024-05-16 16:07:04.227495 tolvera-0.1.0rc12/src/tolvera/mp/face.py
--rw-r--r--   0        0        0     6515 2024-05-16 16:07:04.227616 tolvera-0.1.0rc12/src/tolvera/mp/face_mesh.py
--rw-r--r--   0        0        0    35788 2024-05-16 16:07:04.227840 tolvera-0.1.0rc12/src/tolvera/mp/face_mesh_connections.py
--rw-r--r--   0        0        0     9488 2024-05-16 16:07:04.227969 tolvera-0.1.0rc12/src/tolvera/mp/hands.py
--rw-r--r--   0        0        0     5051 2024-05-16 16:07:04.228100 tolvera-0.1.0rc12/src/tolvera/mp/pose.py
--rw-r--r--   0        0        0    17634 2024-05-16 16:07:04.228329 tolvera-0.1.0rc12/src/tolvera/npndarray_dict.py
--rw-r--r--   0        0        0      109 2024-05-16 16:07:04.228454 tolvera-0.1.0rc12/src/tolvera/osc/__init__.py
--rw-r--r--   0        0        0    18674 2024-05-17 14:13:51.599092 tolvera-0.1.0rc12/src/tolvera/osc/maxmsp.py
--rw-r--r--   0        0        0     2172 2024-05-16 16:07:04.228739 tolvera-0.1.0rc12/src/tolvera/osc/osc.py
--rw-r--r--   0        0        0    18157 2024-05-17 14:13:51.599442 tolvera-0.1.0rc12/src/tolvera/osc/oscmap.py
--rw-r--r--   0        0        0    21320 2024-05-17 14:08:16.180295 tolvera-0.1.0rc12/src/tolvera/osc/pd.py
--rw-r--r--   0        0        0     8050 2024-05-16 16:07:04.229230 tolvera-0.1.0rc12/src/tolvera/osc/update.py
--rw-r--r--   0        0        0    18354 2024-05-21 16:51:00.553777 tolvera-0.1.0rc12/src/tolvera/particles.py
--rw-r--r--   0        0        0     8746 2024-05-16 16:07:04.229651 tolvera-0.1.0rc12/src/tolvera/patches.py
--rw-r--r--   0        0        0    24885 2024-05-26 16:07:55.462098 tolvera-0.1.0rc12/src/tolvera/pixels.py
--rw-r--r--   0        0        0     3434 2024-05-26 22:21:06.607579 tolvera-0.1.0rc12/src/tolvera/rec.py
--rw-r--r--   0        0        0    11293 2024-05-16 16:07:04.230076 tolvera-0.1.0rc12/src/tolvera/sketchbook.py
--rw-r--r--   0        0        0     1603 2024-05-16 16:07:04.230224 tolvera-0.1.0rc12/src/tolvera/species.py
--rw-r--r--   0        0        0    15351 2024-05-16 16:07:04.230392 tolvera-0.1.0rc12/src/tolvera/state.py
--rw-r--r--   0        0        0     2866 2024-05-26 08:23:48.368693 tolvera-0.1.0rc12/src/tolvera/taichi_.py
--rw-r--r--   0        0        0     7364 2024-05-16 16:07:04.230628 tolvera-0.1.0rc12/src/tolvera/tolvera_.py
--rw-r--r--   0        0        0    13382 2024-05-16 16:07:04.230814 tolvera-0.1.0rc12/src/tolvera/utils.py
--rw-r--r--   0        0        0     1351 2024-05-16 16:07:04.230978 tolvera-0.1.0rc12/src/tolvera/vera/__init__.py
--rw-r--r--   0        0        0     5117 2024-05-21 17:08:55.013379 tolvera-0.1.0rc12/src/tolvera/vera/flock.py
--rw-r--r--   0        0        0     9594 2024-05-19 14:13:17.959490 tolvera-0.1.0rc12/src/tolvera/vera/forces.py
--rw-r--r--   0        0        0     2618 2024-05-16 16:07:05.232273 tolvera-0.1.0rc12/src/tolvera/vera/particle_life.py
--rw-r--r--   0        0        0     4145 2024-05-16 16:07:05.232439 tolvera-0.1.0rc12/src/tolvera/vera/reaction_diffusion.py
--rw-r--r--   0        0        0     8254 2024-05-16 16:07:04.231781 tolvera-0.1.0rc12/src/tolvera/vera/slime.py
--rw-r--r--   0        0        0     5944 2024-05-16 16:07:04.231918 tolvera-0.1.0rc12/src/tolvera/vera/swarmalators.py
--rw-r--r--   0        0        0    10054 1970-01-01 00:00:00.000000 tolvera-0.1.0rc12/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-11-23 15:54:16.427339 tolvera-0.1.0rc8/LICENSE
+-rw-r--r--   0        0        0     7283 2024-03-12 14:02:15.429456 tolvera-0.1.0rc8/README.md
+-rw-r--r--   0        0        0     1372 2024-04-24 07:26:46.877033 tolvera-0.1.0rc8/pyproject.toml
+-rw-r--r--   0        0        0      257 2024-04-05 15:10:24.578539 tolvera-0.1.0rc8/src/tolvera/__init__.py
+-rw-r--r--   0        0        0     1415 2024-03-12 14:02:15.430630 tolvera-0.1.0rc8/src/tolvera/__main__.py
+-rw-r--r--   0        0        0     7859 2024-04-06 16:34:13.230063 tolvera-0.1.0rc8/src/tolvera/context.py
+-rw-r--r--   0        0        0     5841 2024-03-12 14:02:15.431092 tolvera-0.1.0rc8/src/tolvera/cv.py
+-rw-r--r--   0        0        0    34367 2024-03-12 14:02:15.431395 tolvera-0.1.0rc8/src/tolvera/iml.py
+-rw-r--r--   0        0        0      111 2024-03-16 12:45:28.778553 tolvera-0.1.0rc8/src/tolvera/mp/__init__.py
+-rw-r--r--   0        0        0     3543 2024-03-16 14:14:12.562796 tolvera-0.1.0rc8/src/tolvera/mp/face.py
+-rw-r--r--   0        0        0     6515 2024-03-16 15:10:11.518026 tolvera-0.1.0rc8/src/tolvera/mp/face_mesh.py
+-rw-r--r--   0        0        0    35788 2024-03-16 14:19:01.531491 tolvera-0.1.0rc8/src/tolvera/mp/face_mesh_connections.py
+-rw-r--r--   0        0        0     9488 2024-03-16 14:03:33.168705 tolvera-0.1.0rc8/src/tolvera/mp/hands.py
+-rw-r--r--   0        0        0     5051 2024-03-16 12:44:02.945408 tolvera-0.1.0rc8/src/tolvera/mp/pose.py
+-rw-r--r--   0        0        0    17634 2024-03-12 14:02:15.432183 tolvera-0.1.0rc8/src/tolvera/npndarray_dict.py
+-rw-r--r--   0        0        0      109 2024-03-12 14:02:15.432380 tolvera-0.1.0rc8/src/tolvera/osc/__init__.py
+-rw-r--r--   0        0        0    16592 2024-03-12 14:02:15.432591 tolvera-0.1.0rc8/src/tolvera/osc/maxmsp.py
+-rw-r--r--   0        0        0     2172 2024-03-12 14:02:15.432747 tolvera-0.1.0rc8/src/tolvera/osc/osc.py
+-rw-r--r--   0        0        0    18115 2024-03-12 14:02:15.432951 tolvera-0.1.0rc8/src/tolvera/osc/oscmap.py
+-rw-r--r--   0        0        0    21320 2024-03-12 14:02:15.433176 tolvera-0.1.0rc8/src/tolvera/osc/pd.py
+-rw-r--r--   0        0        0     8050 2024-03-12 14:02:15.433346 tolvera-0.1.0rc8/src/tolvera/osc/update.py
+-rw-r--r--   0        0        0    18350 2024-04-05 19:33:09.067969 tolvera-0.1.0rc8/src/tolvera/particles.py
+-rw-r--r--   0        0        0     8746 2024-03-12 14:02:15.433864 tolvera-0.1.0rc8/src/tolvera/patches.py
+-rw-r--r--   0        0        0    20397 2024-03-13 09:04:51.448910 tolvera-0.1.0rc8/src/tolvera/pixels.py
+-rw-r--r--   0        0        0     8299 2024-04-14 18:45:30.236884 tolvera-0.1.0rc8/src/tolvera/sf/__init__.py
+-rw-r--r--   0        0        0    11293 2024-03-12 14:02:15.434348 tolvera-0.1.0rc8/src/tolvera/sketchbook.py
+-rw-r--r--   0        0        0     1603 2024-03-12 14:02:15.434519 tolvera-0.1.0rc8/src/tolvera/species.py
+-rw-r--r--   0        0        0    15351 2024-03-12 14:02:15.434756 tolvera-0.1.0rc8/src/tolvera/state.py
+-rw-r--r--   0        0        0     2753 2024-03-12 14:02:15.434914 tolvera-0.1.0rc8/src/tolvera/taichi_.py
+-rw-r--r--   0        0        0     7364 2024-03-16 14:25:42.689663 tolvera-0.1.0rc8/src/tolvera/tolvera_.py
+-rw-r--r--   0        0        0    13382 2024-03-12 14:02:15.435388 tolvera-0.1.0rc8/src/tolvera/utils.py
+-rw-r--r--   0        0        0     1641 2024-04-06 20:24:19.369051 tolvera-0.1.0rc8/src/tolvera/vera/__init__.py
+-rw-r--r--   0        0        0     1410 2024-01-28 15:19:14.309793 tolvera-0.1.0rc8/src/tolvera/vera/attractors.py
+-rw-r--r--   0        0        0     1250 2024-04-06 17:13:45.518822 tolvera-0.1.0rc8/src/tolvera/vera/diffline.py
+-rw-r--r--   0        0        0     5117 2024-04-05 19:16:35.354112 tolvera-0.1.0rc8/src/tolvera/vera/flock.py
+-rw-r--r--   0        0        0     6658 2024-03-20 11:17:12.058891 tolvera-0.1.0rc8/src/tolvera/vera/flock2.py
+-rw-r--r--   0        0        0     4933 2024-03-19 11:20:46.646127 tolvera-0.1.0rc8/src/tolvera/vera/flock_shiffman.py
+-rw-r--r--   0        0        0     9569 2024-04-06 20:21:36.901912 tolvera-0.1.0rc8/src/tolvera/vera/forces.py
+-rw-r--r--   0        0        0     1436 2024-04-06 19:11:18.568109 tolvera-0.1.0rc8/src/tolvera/vera/geom.py
+-rw-r--r--   0        0        0     2558 2024-01-18 21:45:30.996549 tolvera-0.1.0rc8/src/tolvera/vera/nca.py
+-rw-r--r--   0        0        0     2618 2024-04-05 18:26:46.699886 tolvera-0.1.0rc8/src/tolvera/vera/particle_life.py
+-rw-r--r--   0        0        0     4145 2024-04-10 08:39:25.013654 tolvera-0.1.0rc8/src/tolvera/vera/reaction_diffusion.py
+-rw-r--r--   0        0        0     8254 2024-03-12 14:02:15.437046 tolvera-0.1.0rc8/src/tolvera/vera/slime.py
+-rw-r--r--   0        0        0     5944 2024-03-12 14:02:15.437195 tolvera-0.1.0rc8/src/tolvera/vera/swarmalators.py
+-rw-r--r--   0        0        0     2761 2024-03-21 11:59:27.308477 tolvera-0.1.0rc8/src/tolvera/vera/viscek.py
+-rw-r--r--   0        0        0     8428 1970-01-01 00:00:00.000000 tolvera-0.1.0rc8/PKG-INFO
```

### Comparing `tolvera-0.1.0rc12/LICENSE` & `tolvera-0.1.0rc8/LICENSE`

 * *Files identical despite different names*

### Comparing `tolvera-0.1.0rc12/README.md` & `tolvera-0.1.0rc8/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,73 +1,106 @@
-# Tölvera
+Metadata-Version: 2.1
+Name: tolvera
+Version: 0.1.0rc8
+Summary: Tölvera is a library for exploring music interaction with artificial life and self-organising systems.
+Home-page: https://github.com/Intelligent-Instruments-Lab/tolvera
+License: AGPL-3.0
+Author: Jack Armitage
+Author-email: jack.armitage@me.com
+Requires-Python: >=3.10,<3.12
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: anguilla-iml (>=0.1.0b4,<0.2.0)
+Requires-Dist: iipyper (>=0.1.0b1,<0.2.0)
+Requires-Dist: jsons (>=1.6.3,<2.0.0)
+Requires-Dist: mediapipe (==0.10.9)
+Requires-Dist: opencv-python (>=4.8.1.78,<5.0.0.0)
+Requires-Dist: sardine (>=0.0.0b3,<0.0.1)
+Requires-Dist: signalflow (>=0.4.8,<0.5.0)
+Requires-Dist: taichi (>=1.7.0,<2.0.0)
+Requires-Dist: torch (>=2.2.2,<3.0.0)
+Project-URL: Documentation, https://intelligent-instruments-lab.github.io/tolvera/
+Project-URL: Repository, https://github.com/Intelligent-Instruments-Lab/tolvera
+Description-Content-Type: text/markdown
 
-[Tölvera](https://tolvera.is) is a Python library designed for [composing together](https://arxiv.org/abs/2303.06777) and interacting with [basal](https://royalsocietypublishing.org/doi/full/10.1098/rstb.2019.0750) [agencies](https://link.springer.com/article/10.1007/s00018-023-04790-z), inspired by fields such as artificial life (ALife) and self-organising systems. 
-It provides creative coding-style APIs that allow users to combine and compose various built-in behaviours, such as flocking, slime mold growth, and swarming, and also author their own. 
-With built-in support for Open Sound Control (OSC) via [iipyper](https://github.com/Intelligent-Instruments-Lab/iipyper) and interactive machine learning (IML) via [anguilla](https://github.com/Intelligent-Instruments-Lab/anguilla), Tölvera interfaces with and rapidly maps onto existing creative computing software and hardware, striving to be both an accessible and powerful tool for exploring [diverse intelligence](https://www.frontiersin.org/articles/10.3389/fnsys.2022.768201/full) in artistic contexts.
+# Tölvera
 
-Inspired by our lab's location in Iceland, the word Tölvera is an Icelandic [kenning](https://en.wikipedia.org/wiki/Kenning) based on _tölva_ meaning computer, from _tala_ (number) and _völva_ (prophetess), and _vera_ (being), composed together as _number being_.
+[Tölvera](https://tolvera.is) is a library for exploring musical performance with artificial life (ALife) and self-organising systems. The word is an Icelandic [kenning](https://en.wikipedia.org/wiki/Kenning):
 
-We have employed Tölvera in various collaborative artistic works, including musical performances, compositions, and multimedia installations (see [`references.bib`](https://github.com/Intelligent-Instruments-Lab/tolvera/blob/main/references.bib) for peer-reviewed publications).
-Tölvera's role in these pieces has mainly been "mappable behaviour engine", where interface inputs can control Tölvera programs, and Tölvera runtime data can control interface outputs, in practically any combination.
-In this way, and to controllable degrees, Tölvera can contribute to the underlying dynamics of a given interactive scenario.
-It can also add a [visual component](https://www.youtube.com/watch?v=W2c8vFmdANY), and equally has been used without projection in [other works](https://marcodonnarumma.com/works/ex-silens/).
+- Tölva = computer, from tala (number) + völva (prophetess)
+- Vera = being
+- Tölvera = number being
 
-Tölvera makes use of [Taichi](https://www.taichi-lang.org/), a domain-specific language embedded in Python that enables parallelisation, and is experimental software subject to change.
+Tölvera is written in [Taichi](https://www.taichi-lang.org/), a domain-specific language embedded in Python.
 
-We would be happy to have you join us on our [Discord](https://discord.gg/ER7tWds9vM) server!
+This is experimental software and everything is currently subject to change.
 
-## Showcase & Examples
+Join us on the Tölvera [Discord](https://discord.gg/ER7tWds9vM).
 
-Examples can be found at [iil-examples/tolvera](https://github.com/Intelligent-Instruments-Lab/iil-examples/tree/main/tolvera).
-See also the [guide](https://intelligent-instruments-lab.github.io/tolvera/guide), [reference](https://intelligent-instruments-lab.github.io/tolvera/reference) and [experiments](https://intelligent-instruments-lab.github.io/tolvera/experiments) pages.
+## Showcase
 
 [Visit the YouTube Playlist](https://www.youtube.com/embed/ahSXjnYHZLU?&list=PL8bdQleKUA1vNez5gw-pfQB21Q1-vHn3x) (if you'd like to add a video, please get in touch).
 
 ![type:video](https://www.youtube.com/embed/ahSXjnYHZLU?&list=PL8bdQleKUA1vNez5gw-pfQB21Q1-vHn3x)
 
 <!-- [![](assets/images/tolvera.jpg)](https://www.youtube.com/watch?v=ahSXjnYHZLU&list=PL8bdQleKUA1vNez5gw-pfQB21Q1-vHn3x&pp=gAQBiAQB) -->
 
+## Features
+
+- `tv.v`: a collection of "vera" (beings) including Move, Flock, Slime and Swarm, with more being continuously added. Vera can be combined and composed in various ways.
+- `tv.p`: extensible particle system. Particles are divided into multiple species, where each species has a unique relationship with every other species, including itself
+- `tv.s`: n-dimensional state structures that can be used by "vera", including built-in OSC and IML creation (see below).
+- `tv.px`: drawing library including various shapes and blend modes, styled similarly to p5.js etc.
+- `tv.osc`: Open Sound Control (OSC) via [iipyper](https://github.com/Intelligent-Instruments-Lab/iipyper), including automated export of OSC schemas to JSON, XML, Pure Data (Pd), Max/MSP (SuperCollider TBC).
+- `tv.iml`: Interactive Machine Learning via [anguilla](https://github.com/Intelligent-Instruments-Lab/anguilla).
+- `tv.ti`: Taichi-based simulation and rendering engine. Can be run "headless" (without graphics).
+- `tv.cv`: computer vision integration based on OpenCV and Mediapipe.
+
+## Examples
+
+Examples can be found at [iil-examples/tolvera](https://github.com/Intelligent-Instruments-Lab/iil-examples/tree/main/tolvera).
+When run as a script, Tölvera program looks like this:
+
+```py
+from tolvera import Tolvera, run
+
+def main(**kwargs):
+    tv = Tolvera(**kwargs)
+
+    @tv.render
+    def _():
+        return tv.px
+
+if __name__ == '__main__':
+    run(main)
+```
+
 ## Install
 
 Taichi [supports numerous operating systems and backends](https://docs.taichi-lang.org/docs/hello_world#supported-systems-and-backends).
 If you plan on using Vulkan for graphics (recommended for macOS), you may need to [install the Vulkan SDK](https://docs.taichi-lang.org/docs/hello_world#supported-systems-and-backends) first and restart your machine.
 
 Tölvera is [registered on PyPI](https://pypi.org/project/tolvera) and can be installed via a Python package manager such as `pip`:
 
 ```sh
 pip install tolvera
 ```
 
 ## Develop
 
-For development, we use [`poetry`](https://python-poetry.org/).
-Fork/clone this repository and install the package with `poetry:
+Fork/clone this repository and install the package with `poetry`:
 
 ```sh
 git clone https://github.com/Intelligent-Instruments-Lab/tolvera # (or clone your own fork)
 cd tolvera
 poetry install
 ```
 
-## Known Issues & Limitations
-
-- Tölvera currently [does not support Python 3.12 and above](https://github.com/taichi-dev/taichi/issues/8365) - a Python 3.11 installation is recommended.
-This can be created in the following way using [miniconda](https://docs.anaconda.com/free/miniconda/index.html):
-```sh
-conda create -n tolvera python=3.11
-conda activate tolvera
-```
-- Tölvera does not support Intel-based Apple devices (due to [`anguilla`](https://github.com/Intelligent-Instruments-Lab/anguilla)'s FAISS dependency, and Mediapipe not supporting Intel Macs).
-- On macOS, [an OpenMP issue](https://github.com/pytorch/pytorch/issues/78490) may prevent Tölvera programs from running, which can be addressed by adding the following environment variable:
-```sh
-export KMP_DUPLICATE_LIB_OK=TRUE
-```
-- Sonification via [SignalFlow](https://signalflow.dev) does not work on Windows.
-- Mediapipe versions [may need to be downgraded](https://github.com/google/mediapipe/issues/5168) in order to work on macOS and Windows.
-
 ## Contribute
 
 We welcome [Pull Requests](https://github.com/Intelligent-Instruments-Lab/tolvera/pulls) across all areas of the project:
 
 - Addressing [Issues](https://github.com/Intelligent-Instruments-Lab/tolvera/issues)
 - Adding features (see [Issues](https://github.com/Intelligent-Instruments-Lab/tolvera/issues) and [Discussion](https://github.com/Intelligent-Instruments-Lab/tolvera/discussion))
 - [Examples](https://github.com/Intelligent-Instruments-Lab/iil-examples/tolvera)
@@ -85,51 +118,62 @@
 Across the project, we follow the [Berlin Code of Conduct](https://berlincodeofconduct.org/). 
 Please get in touch if you experience or witness any conduct issues.
 
 ## Roadmap
 
 See [Discussion](https://github.com/Intelligent-Instruments-Lab/tolvera/discussion).
 
-## Citation
+## Citing
 
-Tölvera is being written about and used in a number of contexts (see [references.bib](https://github.com/Intelligent-Instruments-Lab/tolvera/blob/main/references.bib)).
-The current canonical citation is our [NIME 2024](https://www.nime2024.org/) paper:
+Tölvera is being written about and used in a number of contexts (see [references.bib](https://github.com/Intelligent-Instruments-Lab/tolvera/blob/main/references.bib)), here are a few recent examples:
 
 ```bibtex
-@inproceedings{armitageTolveraComposingBasal2024,
-  title = {T{\"o}lvera: {{Composing With Basal Agencies}}},
-  booktitle = {Proc. {{New Interfaces}} for {{Musical Expression}}},
-  author = {Armitage, Jack and Shepardson, Victor and Magnusson, Thor},
-  year = {2024},
-  address = {Utrecht, NL},
+@inproceedings{armitageAgentialScoresExploring2023,
+  Address = {Boston, Massachusetts, USA},
+  Author = { Jack Armitage and Thor Magnusson },
+  Title = {Agential Scores: Artificial Life for Emergent, Self-Organising and Entangled Music Notation},
+  Booktitle = {Proceedings of the International Conference on Technologies for Music Notation and Representation -- TENOR'2023},
+  Pages = {51 - 61},
+  Year = {2023},
+  Editor = {Anthony Paul De Ritis and Victor Zappi and Jeremy Van Buskirk and John Mallia},
+  Publisher = {Northeastern University},
+  ISBN = {978-0-6481592-7-8}
+}
+
+@inproceedings{armitageStrengjavera2023,
+  title = {Strengjavera},
+  booktitle = {{{AI Music Creativity}} 2023},
+  author = {Armitage, Jack},
+  year = {2023},
+  address = {{University of Sussex, Brighton, UK}},
+  doi = {10.5281/zenodo.8329855},
+  ISBN = {978-0-9957862-9-5},
+  url = {https://zenodo.org/records/8329855}
 }
 ```
 
 ## Inspiration
 
-- [Michael Levin](https://en.wikipedia.org/wiki/Michael_Levin_(biologist))
 - [SwissGL](https://swiss.gl)
 - [Lenia](https://chakazul.github.io/lenia.html)
 - Particle Life (attributed to various, see for example [Clusters](https://www.ventrella.com/Clusters/))
 - [Journey to the Microcosmos](https://www.youtube.com/@journeytomicro)
 - [Complexity Explorables](https://www.complexity-explorables.org/)
 
 ## Contact
 
-Tölvera is developed primarily by [Jack Armitage](https://jackarmitage.com) and [collaborators](https://iil.is/people) at the [Intelligent Instruments Lab](https://iil.is/about). 
-Get in touch to [collaborate](https://iil.is/collaborate):
+`tolvera` is developed by the [Intelligent Instruments Lab](https://iil.is/about). Get in touch to [collaborate](https://iil.is/collaborate):
 
  ◦ <a href="https://iil.is" target="_blank" title="Intelligent Instrumets Lab">iil.is</a> ◦ 
 <a href="https://facebook.com/intelligentinstrumentslab" target="_blank" title="facebook.com">Facebook</a> ◦ 
 <a href="https://instagram.com/intelligentinstruments" target="_blank" title="instagram.com">Instagram</a> ◦ 
 <a href="https://x.com/_iil_is" target="_blank" title="x.com">X (Twitter)</a> ◦ 
 <a href="https://youtube.com/@IntelligentInstruments" target="_blank" title="youtube.com">YouTube</a> ◦ 
 <a href="https://discord.gg/fY9GYMebtJ" target="_blank" title="discord.gg">Discord</a> ◦ 
 <a href="https://github.com/intelligent-instruments-lab" target="_blank" title="github.com">GitHub</a> ◦ 
 <a href="https://www.linkedin.com/company/intelligent-instruments-lab" target="_blank" title="www.linkedin.com">LinkedIn</a> ◦ 
-<a href="mailto:jack@hi.is" target="_blank" title="">Email</a> ◦ 
+<a href="mailto:iil@lhi.is" target="_blank" title="">Email</a> ◦ 
 
-## Acknowledgements
+## Funding
 
-We thank the Taichi community for their wonderful project, that makes Tölvera possible.
+The Intelligent Instruments project (INTENT) is funded by the European Research Council (ERC) under the European Union’s Horizon 2020 research and innovation programme (Grant agreement No. 101001848).
 
-The [Intelligent Instruments](https://iil.is) project (INTENT) is funded by the European Research Council (ERC) under the European Union’s Horizon 2020 research and innovation programme (Grant agreement No. 101001848).
```

### Comparing `tolvera-0.1.0rc12/pyproject.toml` & `tolvera-0.1.0rc8/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "tolvera"
 packages = [{ include = "tolvera", from = "src"}]
-version = "0.1.0-rc12"
+version = "0.1.0-rc8"
 description = "Tölvera is a library for exploring music interaction with artificial life and self-organising systems."
 authors = ["Jack Armitage <jack.armitage@me.com>"]
 readme = "README.md"
 license = "AGPL-3.0"
 repository = "https://github.com/Intelligent-Instruments-Lab/tolvera"
 documentation = "https://intelligent-instruments-lab.github.io/tolvera/"
 
@@ -14,27 +14,26 @@
 taichi = "^1.7.0"
 jsons = "^1.6.3"
 opencv-python = "^4.8.1.78"
 iipyper = "^0.1.0b1"
 anguilla-iml = "^0.1.0b4"
 sardine = "^0.0.0b3"
 mediapipe = "0.10.9"
+signalflow = "^0.4.8"
 torch = "^2.2.2"
-tqdm = "^4.66.4"
 
 [tool.poetry.group.dev.dependencies]
 mkdocs = "^1.5.3"
 mkdocs-video = "^1.5.0"
 mkdocstrings = {extras = ["python"], version = "^0.23.0"}
 mkdocs-gen-files = "^0.5.0"
 mkdocs-include-markdown-plugin = "^6.0.4"
 mkdocs-material = "^9.4.8"
 mkdocs-material-extensions = "^1.3"
 mkdocs-autorefs = "^0.5.0"
-mkdocs-awesome-pages-plugin = "^2.9.2"
 pytest = "^7.4.3"
 black = "^23.11.0"
 isort = "^5.12.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `tolvera-0.1.0rc12/src/tolvera/__main__.py` & `tolvera-0.1.0rc8/src/tolvera/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     print("Running demo...")
     tv = Tolvera(**kwargs)
 
     @tv.render
     def _():
         """Render function that draws flocking particles."""
         tv.px.diffuse(0.99)
+        tv.p()
         tv.v.flock(tv.p)
         tv.px.particles(tv.p, tv.s.species, "circle")
         return tv.px
 
 
 def main(**kwargs):
     """Run Tölvera with kwargs.
```

### Comparing `tolvera-0.1.0rc12/src/tolvera/context.py` & `tolvera-0.1.0rc8/src/tolvera/context.py`

 * *Files 8% similar despite different names*

```diff
@@ -144,21 +144,14 @@
             **kwargs: Keyword arguments for function.
         """
         if f is not None:
             print(f"[{self.name}] Running with render function {f.__name__}...")
         else:
             print(f"[{self.name}] Running with no render function...")
         while self.ti.window.running:
-            # print(kwargs)
-            # exit()
-            # gui = kwargs.get('gui', None)
-            # if gui is not None:
-            #     gui()
-            # with self.ti.gui.sub_window("Sub Window", 0.1, 0.1, 0.2, 0.2) as w:
-            #     w.text("text")
             with _lock:
                 self.step(f, **kwargs)
     
     def step(self, f, **kwargs):
         [t.p() for t in self.tolveras.values()]
         if f is not None:
             self.canvas = f(**kwargs)
```

### Comparing `tolvera-0.1.0rc12/src/tolvera/cv.py` & `tolvera-0.1.0rc8/src/tolvera/cv.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     def __init__(self, context, **kwargs) -> None:
         self.ctx = context
         self.x, self.y = self.ctx.x, self.ctx.y
         self.px = Pixels(self.ctx, **kwargs)
         self.frame_rgb = np.zeros((self.y, self.x, 3), np.uint8)
         self.ggui_fps_limit = kwargs.get("ggui_fps_limit", 120)
         self.substeps = kwargs.get("substeps", 2)
+        self.invert = kwargs.get("invert", True)
         self.colormode = kwargs.get("colormode", "rgba")
         self.device = kwargs.get("device", 0)
         self._camera = kwargs.get("camera", False)
         self.cc_frame = np.zeros((self.y, self.x, 3), np.uint8)
         self.cc_frame_f32 = np.zeros((self.y, self.x, 3), np.float32)
         self.diff = np.zeros((self.y, self.x, 3), np.uint8)
         self.diff_p = 0.0
```

### Comparing `tolvera-0.1.0rc12/src/tolvera/iml.py` & `tolvera-0.1.0rc8/src/tolvera/iml.py`

 * *Files identical despite different names*

### Comparing `tolvera-0.1.0rc12/src/tolvera/mp/face.py` & `tolvera-0.1.0rc8/src/tolvera/mp/face.py`

 * *Files identical despite different names*

### Comparing `tolvera-0.1.0rc12/src/tolvera/mp/face_mesh.py` & `tolvera-0.1.0rc8/src/tolvera/mp/face_mesh.py`

 * *Files identical despite different names*

### Comparing `tolvera-0.1.0rc12/src/tolvera/mp/face_mesh_connections.py` & `tolvera-0.1.0rc8/src/tolvera/mp/face_mesh_connections.py`

 * *Files identical despite different names*

### Comparing `tolvera-0.1.0rc12/src/tolvera/mp/hands.py` & `tolvera-0.1.0rc8/src/tolvera/mp/hands.py`

 * *Files identical despite different names*

### Comparing `tolvera-0.1.0rc12/src/tolvera/mp/pose.py` & `tolvera-0.1.0rc8/src/tolvera/mp/pose.py`

 * *Files identical despite different names*

### Comparing `tolvera-0.1.0rc12/src/tolvera/npndarray_dict.py` & `tolvera-0.1.0rc8/src/tolvera/npndarray_dict.py`

 * *Files identical despite different names*

### Comparing `tolvera-0.1.0rc12/src/tolvera/osc/maxmsp.py` & `tolvera-0.1.0rc8/src/tolvera/osc/maxmsp.py`

 * *Files 8% similar despite different names*

```diff
@@ -86,37 +86,33 @@
 
     def init(self):
         self.w = 5.5  # default width (scaling factor)
         self.h = 22.0  # default height (pixels)
         self.s_x, self.s_y = 30, 125  # insertion point
         self.r_x, self.r_y = 30, 575  # insertion point
         self.patcher_ids = {}
-        self.patcher_ids["send_id"] = self.osc_send(
+        self.patcher_ids["send_id"] = self.add_osc_send(
             self.osc.host, self.osc.port, self.s_x, 30, print_label="sent"
         )
-        self.patcher_ids["receive_id"] = self.osc_receive(
+        self.patcher_ids["receive_id"] = self.add_osc_receive(
             self.client_port, self.s_x + 150, 30, print_label="received"
         )
-        self.comment("Max → Python", self.s_x, self.s_y, 24)
-        self.comment("Python → Max", self.r_x, self.r_y, 24)
+        self.add_comment("Max → Python", self.s_x, self.s_y, 24)
+        self.add_comment("Python → Max", self.r_x, self.r_y, 24)
         self.s_y += 50
         self.r_y += 50
         self.save(self.filepath)
 
-    """
-    basic objects
-    """
-
-    def box(self, box_type, inlets, outlets, x, y, w, h=None):
+    def add_box(self, box_type, inlets, outlets, x, y, w, h=None):
         if h is None:
             h = self.h
         box_id, box = self.create_box(box_type, inlets, outlets, x, y, w, h)
-        return self._box(box)
+        return self._add_box(box)
 
-    def _box(self, box):
+    def _add_box(self, box):
         self.patch["patcher"]["boxes"].append(box)
         return self.id_from_str(box["box"]["id"])
 
     def create_box(self, box_type, inlets, outlets, x, y, w, h=None):
         if h is None:
             h = self.h
         box_id = len(self.patch["patcher"]["boxes"]) + 1
@@ -133,173 +129,169 @@
             if outlets == 1:
                 box["box"]["outlettype"] = [""]
             match box_type:
                 case "int" | "float" | "bang":
                     box["box"]["outlettype"] = ["", "bang"]
         return box_id, box
 
-    def object(self, text: str, inlets: int, outlets: int, x: float, y: float):
+    def add_object(self, text, inlets, outlets, x, y):
         box_id, box = self.create_box(
             "object", inlets, outlets, x, y, len(text) * self.w
         )
         box["box"]["text"] = text
-        self._box(box)
+        self._add_box(box)
         return box_id
 
-    def message(self, text, x, y):
+    def add_message(self, text, x, y):
         box_id, box = self.create_box("message", 2, 1, x, y, len(text) * self.w)
         box["box"]["text"] = text
-        self._box(box)
+        self._add_box(box)
         return box_id
 
-    def comment(self, text, x, y, fontsize=12):
+    def add_comment(self, text, x, y, fontsize=12):
         box_id, box = self.create_box("comment", 0, 0, x, y, len(text) * self.w)
         box["box"]["text"] = text
         box["box"]["fontsize"] = fontsize
-        self._box(box)
+        self._add_box(box)
         return box_id
 
-    def bang(self, x, y):
+    def add_bang(self, x, y):
         box_id, box = self.create_box("bang", 1, 1, x, y, 20.0)
-        self._box(box)
+        self._add_box(box)
         return box_id
 
-    def slider(self, x, y, min_val, size, float=False):
+    def add_slider(self, x, y, min_val, size, float=False):
         box_id, box = self.create_box("slider", 1, 1, x, y, 20.0, 140.0)
         if float:
             box["box"]["floatoutput"] = 1
         box["box"]["min"] = min_val
         box["box"]["size"] = size
-        self._box(box)
+        self._add_box(box)
         return box_id
 
-    """
-    connections
-    """
-
     def connect(self, src, src_outlet, dst, dst_inlet):
         patchline = {
             "patchline": {
                 "destination": ["obj-" + str(dst), dst_inlet],
                 "source": ["obj-" + str(src), src_outlet],
             }
         }
         self.patch["patcher"]["lines"].append(patchline)
         return patchline
 
-    """
-    osc send/receive
-    """
-
-    def osc_send(self, ip, port, x, y, print=True, print_label=None):
-        box_id_0 = self.object("r send", 0, 1, x, y)
-        box_id = self.object("udpsend " + ip + " " + str(port), 1, 0, x, y + 25)
+    def save(self, name):
+        with open(name + ".maxpat", "w") as f:
+            f.write(json.dumps(self.patch, indent=2))
+
+    def load(self, name):
+        with open(name + ".maxpat", "r") as f:
+            self.patch = json.loads(f.read())
+
+    def get_box_by_id(self, id):
+        for box in self.patch["patcher"]["boxes"]:
+            if self.id_from_str(box["box"]["id"]) == id:
+                return box
+        return None
+
+    def str_from_id(self, id):
+        return "obj-" + str(id)
+
+    def id_from_str(self, obj_str):
+        return int(obj_str[4:])
+
+    def add_osc_send(self, ip, port, x, y, print=True, print_label=None):
+        box_id_0 = self.add_object("r send", 0, 1, x, y)
+        box_id = self.add_object("udpsend " + ip + " " + str(port), 1, 0, x, y + 25)
         if print:
             text = "print" if print_label is None else "print " + print_label
-            print_id = self.object(text, 1, 0, x + 50, y)
+            print_id = self.add_object(text, 1, 0, x + 50, y)
             self.connect(box_id_0, 0, box_id, 0)
             self.connect(box_id_0, 0, print_id, 0)
             return box_id_0
         return box_id
 
-    def osc_receive(self, port, x, y, print=True, print_label=None):
-        box_id_0 = self.object("s receive", 0, 1, x, y + 25)
-        box_id = self.object("udpreceive " + str(port), 1, 1, x, y)
+    def add_osc_receive(self, port, x, y, print=True, print_label=None):
+        box_id_0 = self.add_object("s receive", 0, 1, x, y + 25)
+        box_id = self.add_object("udpreceive " + str(port), 1, 1, x, y)
         if print:
             text = "print" if print_label is None else "print " + print_label
-            print_id = self.object(text, 1, 0, x + 60, y + 25)
+            print_id = self.add_object(text, 1, 0, x + 60, y + 25)
             self.connect(box_id, 0, print_id, 0)
             self.connect(box_id, 0, box_id_0, 0)
             return box_id_0
         return box_id
 
-    def osc_route(self, port, x, y, print=True, print_label=None):
+    def add_osc_route(self, port, x, y, print=True, print_label=None):
         """
         [route path]
         [s name] [print]
         [unpack] ?
         [r name]
         """
         pass
 
-    """
-    osc send/receive args/list
-    """
-
-    def send_args_func(self, f):
-        hints = typing.get_type_hints(f["f"])["return"].__args__
-        f_p = f["params"]
-        params = []
-        if len(f_p) == 0:
-            self.osc_receive_msg(self.r_x, self.r_y, f["address"])
-        else:
-            for i, p in enumerate(f_p):
-                p_def, p_min, p_max = f_p[p][0], f_p[p][1], f_p[p][2]
-                params.append(
-                    {
-                        "label": p,
-                        "data": hints[i].__name__,
-                        "min_val": p_min,
-                        "size": p_max - p_min,
-                    }
-                )
-            self.osc_receive_with_controls(self.r_x, self.r_y, f["address"], params)
-        self.r_x += max(len(params) * 52.0 + 100.0, len(f["address"]) * 6.0 + 25.0)
-        self.save(self.filepath)
-
-    def send_list_func(self, f):
-        raise NotImplementedError("send_list_func not implemented yet")
+    def add_sliders(self, x, y, sliders):
+        """
+        sliders = [
+          { 'label': 'x', data: 'float', min_val: 0.0, size: 0.0 },
+        ]
 
-    def receive_args_func(self, f):
-        hints = typing.get_type_hints(f["f"])
-        f_p = f["params"]
-        params = []
-        if len(f_p) == 0:
-            self.osc_send_msg(self.s_x, self.s_y, f["address"])
-        else:
-            for p in f_p:
-                p_def, p_min, p_max = f_p[p][0], f_p[p][1], f_p[p][2]
-                params.append(
-                    {
-                        "label": p,
-                        "data": hints[p].__name__,
-                        "min_val": p_min,
-                        "size": p_max - p_min,
-                    }
-                )
-            self.osc_send_with_controls(self.s_x, self.s_y, f["address"], params)
-        self.s_x += max(len(params) * 52.0 + 100.0, len(f["address"]) * 6.0 + 25.0)
-        self.save(self.filepath)
+        [slider] ...
+        |
+        [number] ...
+        """
+        slider_ids = []
+        float_ids = []
+        y_off = 0
+        for i, s in enumerate(sliders):
+            y_off = 0
+            x_i = x + (i * 52.0)
+            y_off += self.h
+            slider_id = self.add_slider(
+                x_i, y + y_off, s["min_val"], s["size"], float=s["data"] == "float"
+            )
+            y_off += 150
+            float_id = self.add_box("float", 1, 2, x_i, y + y_off, 50)
+            slider_ids.append(slider_id)
+            float_ids.append(float_id)
+        return slider_ids, float_ids, y_off
 
-    def receive_list_func(self, f):
-        self.osc_send_list(self.s_x, self.s_y, f["address"], f["params"])
-        self.s_x += len(f["address"]) * 6.0 + 50.0
-        self.save(self.filepath)
+    def add_param_comments(self, x, y, params):
+        comment_ids = []
+        y_off = 0
+        for i, p in enumerate(params):
+            y_off = 0
+            x_i = x + (i * 52.0)
+            p_max = (
+                p["min_val"] + p["size"]
+                if p["data"] == "float"
+                else p["min_val"] + p["size"] - 1
+            )
+            comment_id1 = self.add_comment(f'{p["label"]}', x_i, y)
+            y_off += 15
+            comment_id2 = self.add_comment(
+                f'{p["data"][0]} {p["min_val"]}-{p_max}', x_i, y + y_off
+            )
+            comment_ids.append(comment_id1)
+            comment_ids.append(comment_id2)
+        return comment_ids, y_off
 
-    """
-    osc send/receive no args/list (msg)
-    """
-
-    def osc_send_msg(self, x, y, path):
-        msg_id = self.message(path, x, y + 225 + self.h)
-        send_id = self.object("s send", 1, 0, x, y + 250 + self.h)
+    def add_osc_send_msg(self, x, y, path):
+        msg_id = self.add_message(path, x, y + 225 + self.h)
+        send_id = self.add_object("s send", 1, 0, x, y + 250 + self.h)
         self.connect(msg_id, 0, send_id, 0)
         return msg_id
 
-    def osc_receive_msg(self, x, y, path):
-        receive_id = self.object("r receive", 0, 1, x, y + 225 + self.h)
-        msg_id = self.message(path, x, y + 250 + self.h)
+    def add_osc_receive_msg(self, x, y, path):
+        receive_id = self.add_object("r receive", 0, 1, x, y + 225 + self.h)
+        msg_id = self.add_message(path, x, y + 250 + self.h)
         self.connect(receive_id, 0, msg_id, 0)
         return msg_id
 
-    """
-    osc send/receive args with line, slider, rate-limiting, and change detection
-    """
-
-    def osc_send_with_controls(self, x, y, path, parameters):
+    def add_osc_send_with_controls(self, x, y, path, parameters):
         # TODO: add default param value and a loadbang
         """
         [comment path]
         [comment args]
         [r path_arg_name]
         sliders
         |                   |
@@ -307,48 +299,48 @@
         |
         [msg /path $1 $2 $3 ...]
         |
         [s send]
         """
         y_off = 0
         # [comment path]
-        path_comment_id = self.comment(path, x, y + y_off)
+        path_comment_id = self.add_comment(path, x, y + y_off)
         y_off += 15
-        param_comment_ids, _y_off = self.param_comments(x, y + y_off, parameters)
+        param_comment_ids, _y_off = self.add_param_comments(x, y + y_off, parameters)
 
         # [r path_arg_name]
         y_off += 35
         receive_ids = [
-            self.object(
+            self.add_object(
                 "r " + path.replace("/", "_")[1:] + "_" + p["label"][0:3],
                 1,
                 0,
                 x + i * 52.0,
                 y + y_off + (0 if i % 2 == 0 else 25),
             )
             for i, p in enumerate(parameters)
         ]
         y_off += 30
 
         # sliders
-        slider_ids, slider_float_ids, _y_off = self.sliders(
+        slider_ids, slider_float_ids, _y_off = self.add_sliders(
             x, y + y_off, parameters
         )
         y_off += _y_off + 25
         # [pak $1 $2 $3 ...]
-        pack_id = self.object(
+        pack_id = self.add_object(
             "pak " + self._pack_args(parameters), len(parameters) + 1, 1, x, y + y_off
         )
         pack_width = self.get_box_by_id(pack_id)["box"]["patching_rect"][2]
         # [msg /path $1 $2 $3 ...]
         y_off += 25
-        msg_id = self.message(path + " " + self._msg_args(parameters), x, y + y_off)
+        msg_id = self.add_message(path + " " + self._msg_args(parameters), x, y + y_off)
         # [s send]
         y_off += 25
-        send_id = self.object("s send", 1, 0, x, y + y_off)
+        send_id = self.add_object("s send", 1, 0, x, y + y_off)
         # connections
         [
             self.connect(receive_ids[i], 0, slider_ids[i], 0)
             for i in range(len(parameters))
         ]
         [
             self.connect(slider_ids[i], 0, slider_float_ids[i], 0)
@@ -358,15 +350,15 @@
             self.connect(slider_float_ids[i], 0, pack_id, i)
             for i in range(len(parameters))
         ]
         self.connect(pack_id, 0, msg_id, 0)
         self.connect(msg_id, 0, send_id, 0)
         return slider_ids, pack_id, msg_id
 
-    def osc_receive_with_controls(self, x, y, path, parameters):
+    def add_osc_receive_with_controls(self, x, y, path, parameters):
         # TODO: add default param value and a loadbang
         """
         [comment path]
         [r receive]
         |
         [route /path]
         |                  |
@@ -378,193 +370,119 @@
         |
         [s arg_name]
         [comment path_arg_name]
         [comment type min-max]
         """
         # [comment path]
         y_off = 0
-        path_comment_id = self.comment(path, x, y + y_off)
+        path_comment_id = self.add_comment(path, x, y + y_off)
 
         # [r receive]
         y_off += 25
-        receive_id = self.object("r receive", 0, 1, x, y + y_off)
+        receive_id = self.add_object("r receive", 0, 1, x, y + y_off)
 
         # [route /path]
         y_off += 25
-        route_id = self.object("route " + path, 1, 1, x, y + y_off)
+        route_id = self.add_object("route " + path, 1, 1, x, y + y_off)
 
         # [unpack f f f ...] [print /path]
         y_off += 25
-        unpack_id = self.object(
+        unpack_id = self.add_object(
             "unpack " + self._pack_args(parameters),
             len(parameters) + 1,
             1,
             x,
             y + y_off,
         )
         unpack_width = self.get_box_by_id(unpack_id)["box"]["patching_rect"][2]
-        print_id = self.object(
+        print_id = self.add_object(
             "print " + path, 1, 0, x + unpack_width + 10, y + y_off
         )
 
         # sliders
         y_off += 10
-        slider_ids, float_ids, _y_off = self.sliders(x, y + y_off, parameters)
+        slider_ids, float_ids, _y_off = self.add_sliders(x, y + y_off, parameters)
 
         # [s arg_name]
         y_off += _y_off + 25
         send_ids = [
-            self.object(
+            self.add_object(
                 "s " + path.replace("/", "_")[1:] + "_" + p["label"][0:3],
                 1,
                 0,
                 x + i * 52.0,
                 y + y_off + (0 if i % 2 == 0 else 25),
             )
             for i, p in enumerate(parameters)
         ]
 
         # [comment params]
         y_off += 50
-        param_comment_ids, _y_off = self.param_comments(x, y + y_off, parameters)
+        param_comment_ids, _y_off = self.add_param_comments(x, y + y_off, parameters)
 
         # connections
         self.connect(receive_id, 0, route_id, 0)
         self.connect(route_id, 0, unpack_id, 0)
         self.connect(route_id, 0, print_id, 0)
         [self.connect(unpack_id, i, slider_ids[i], 0) for i in range(len(parameters))]
         [
             self.connect(slider_ids[i], 0, float_ids[i], 0)
             for i in range(len(parameters))
         ]
         [self.connect(float_ids[i], 0, send_ids[i], 0) for i in range(len(parameters))]
 
         return slider_ids, unpack_id
 
-    """
-    sliders
-    """
-
-    def sliders(self, x, y, sliders):
-        """
-        sliders = [
-          { 'label': 'x', data: 'float', min_val: 0.0, size: 0.0 },
-        ]
-
-        [slider] ...
-        |
-        [number] ...
-        """
-        slider_ids = []
-        float_ids = []
-        y_off = 0
-        for i, s in enumerate(sliders):
-            y_off = 0
-            x_i = x + (i * 52.0)
-            y_off += self.h
-            slider_id = self.slider(
-                x_i, y + y_off, s["min_val"], s["size"], float=s["data"] == "float"
-            )
-            y_off += 150
-            float_id = self.box("float", 1, 2, x_i, y + y_off, 50)
-            slider_ids.append(slider_id)
-            float_ids.append(float_id)
-        return slider_ids, float_ids, y_off
-
-    """
-    comments
-    """
-
-    def param_comments(self, x, y, params):
-        comment_ids = []
-        y_off = 0
-        for i, p in enumerate(params):
-            y_off = 0
-            x_i = x + (i * 52.0)
-            p_max = (
-                p["min_val"] + p["size"]
-                if p["data"] == "float"
-                else p["min_val"] + p["size"] - 1
-            )
-            comment_id1 = self.comment(f'{p["label"]}', x_i, y)
-            y_off += 15
-            comment_id2 = self.comment(
-                f'{p["data"][0]} {p["min_val"]}-{p_max}', x_i, y + y_off
-            )
-            comment_ids.append(comment_id1)
-            comment_ids.append(comment_id2)
-        return comment_ids, y_off
-
-    """
-    lists
-    """
-
-    def osc_send_list(self, x, y, path, params):
-        """
-        [comment] path, list name, params
-        [r] path
-        [prepend path]
-        [s send]
-        """
-        y_off = 0
-        self.comment(path, x, y)
-        y_off += 15
-        l = list(params.items())[0]
-        self.comment(f"{l[0]}", x, y + y_off)
-        y_off += 15
-        self.comment(f"l {l[1][1]} {l[1][2]}", x, y + y_off)
-        y_off += self.h
-        receive_id = self.object(f"r {self.path_to_snakecase(path)}", 0, 1, x, y + y_off)
-        y_off += self.h + 3
-        prepend_id = self.object(f"prepend {path}", 1, 1, x, y + y_off)
-        y_off += self.h + 3
-        send_id = self.object(f"s send", 0, 1, x, y + y_off)
-        self.connect(receive_id, 0, prepend_id, 0)
-        self.connect(prepend_id, 0, send_id, 0)
-
-    def osc_receive_list(self, x, y, path, params):
-        """
-        [comment] path
-        [r receive.from.iipyper]
-        [routeOSC path]
-        [s path]
-        [comment] params
-        """
-        # y_off = 0
-        # self.comment(path, x, y)
-        # y_off += self.h
-        # receive_id = self.object(f"r receive.from.iipyper", x, y + y_off)
-        # y_off += self.h
-        # route_id = self.object(f"routeOSC {path}", x, y + y_off)
-        # y_off += self.h
-        # send_id = self.object(f"s {self.path_to_snakecase(path)}", x, y + y_off)
-        # y_off += self.h
-        # l = list(params.items())[0]
-        # self.comment(f"{l[0]}", x, y + y_off)
-        # y_off += 15
-        # self.comment(f"l {l[1][1]} {l[1][2]}", x, y + y_off)
-        # self.connect(receive_id, 0, route_id, 0)
-        # self.connect(route_id, 0, send_id, 0)
-        pass
-
-    """
-    utils
-    """
+    def add_send_args_func(self, f):
+        hints = typing.get_type_hints(f["f"])["return"].__args__
+        f_p = f["params"]
+        params = []
+        if len(f_p) == 0:
+            self.add_osc_receive_msg(self.r_x, self.r_y, f["address"])
+        else:
+            for i, p in enumerate(f_p):
+                p_def, p_min, p_max = f_p[p][0], f_p[p][1], f_p[p][2]
+                params.append(
+                    {
+                        "label": p,
+                        "data": hints[i].__name__,
+                        "min_val": p_min,
+                        "size": p_max - p_min,
+                    }
+                )
+            self.add_osc_receive_with_controls(self.r_x, self.r_y, f["address"], params)
+        self.r_x += max(len(params) * 52.0 + 100.0, len(f["address"]) * 6.0 + 25.0)
+        self.save(self.filepath)
 
-    def get_box_by_id(self, id):
-        for box in self.patch["patcher"]["boxes"]:
-            if self.id_from_str(box["box"]["id"]) == id:
-                return box
-        return None
+    def add_send_list_func(self, f):
+        raise NotImplementedError("add_send_list_func not implemented yet")
 
-    def str_from_id(self, id):
-        return "obj-" + str(id)
+    def add_receive_args_func(self, f):
+        hints = typing.get_type_hints(f["f"])
+        f_p = f["params"]
+        params = []
+        if len(f_p) == 0:
+            self.add_osc_send_msg(self.s_x, self.s_y, f["address"])
+        else:
+            for p in f_p:
+                p_def, p_min, p_max = f_p[p][0], f_p[p][1], f_p[p][2]
+                params.append(
+                    {
+                        "label": p,
+                        "data": hints[p].__name__,
+                        "min_val": p_min,
+                        "size": p_max - p_min,
+                    }
+                )
+            self.add_osc_send_with_controls(self.s_x, self.s_y, f["address"], params)
+        self.s_x += max(len(params) * 52.0 + 100.0, len(f["address"]) * 6.0 + 25.0)
+        self.save(self.filepath)
 
-    def id_from_str(self, obj_str):
-        return int(obj_str[4:])
+    def add_receive_list_func(self, f):
+        raise NotImplementedError("add_receive_list_func not implemented yet")
 
     def _msg_args(self, args):
         return " ".join(["$" + str(i + 1) for i in range(len(args))])
 
     def _pack_args(self, args):
         arg_types = []
         for a in args:
@@ -572,22 +490,7 @@
                 case "int":
                     arg_types.append("i")
                 case "float":
                     arg_types.append("f")
                 case "string":
                     arg_types.append("s")
         return " ".join(arg_types)
-
-    def path_to_snakecase(self, path):
-        return path.replace("/", "_")[1:]  # +'_'+label[0:3]
-
-    """
-    save/load
-    """
-
-    def save(self, name):
-        with open(name + ".maxpat", "w") as f:
-            f.write(json.dumps(self.patch, indent=2))
-
-    def load(self, name):
-        with open(name + ".maxpat", "r") as f:
-            self.patch = json.loads(f.read())
```

### Comparing `tolvera-0.1.0rc12/src/tolvera/osc/osc.py` & `tolvera-0.1.0rc8/src/tolvera/osc/osc.py`

 * *Files identical despite different names*

### Comparing `tolvera-0.1.0rc12/src/tolvera/osc/oscmap.py` & `tolvera-0.1.0rc8/src/tolvera/osc/oscmap.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,17 +176,17 @@
             ]
             wrapper(default_arg)
             return wrapper
 
         return decorator
 
     def add_send_list(self, func, kwargs):
-        f = self.add_send_list_to_osc_map(func, kwargs)
+        self.add_send_list_to_osc_map(func, kwargs)
         if self.create_patch is True:
-            self.add_send_list_to_patcher(f)
+            self.add_send_list_to_patcher(func)
 
     def add_send_list_to_osc_map(self, func, kwargs):
         f = self.map_func_to_dict(func, kwargs)
         # TODO: Hack for send_list_inline which doesn't have a return type hint
         if "return" in f["hints"]:
             hint = f["hints"]["return"]
         else:
@@ -211,22 +211,21 @@
                 client=self.client_name,
             )
         f["type"] = "list"
         f["length"] = kwargs["length"]
         self.dict["send"][f["name"]] = f
         if self.export is not None:
             self.export_dict()
-        return f
 
     def add_send_list_to_patcher(self, func):
-        f = self.dict["send"][func["name"]]
+        f = self.dict["send"][func.__name__]
         self.patcher.send_list_func(f)
 
     def send_list_inline(self, name: str, sender_func, length: int, send_mode="broadcast", count=1, **kwargs):
-        kwargs = {**kwargs, **{"name": name, "vector": (0.0,0.0,1.0), "length": length, "send_mode": send_mode, "count": count}}
+        kwargs = {**kwargs, **{"name": name, "length": length, "send_mode": send_mode, "count": count}}
         self.send_list(**kwargs)(sender_func)
 
     """
     send kwargs
     """
 
     def send_kwargs(self, **kwargs):
```

### Comparing `tolvera-0.1.0rc12/src/tolvera/osc/pd.py` & `tolvera-0.1.0rc8/src/tolvera/osc/pd.py`

 * *Files identical despite different names*

### Comparing `tolvera-0.1.0rc12/src/tolvera/osc/update.py` & `tolvera-0.1.0rc8/src/tolvera/osc/update.py`

 * *Files identical despite different names*

### Comparing `tolvera-0.1.0rc12/src/tolvera/particles.py` & `tolvera-0.1.0rc8/src/tolvera/particles.py`

 * *Files 0% similar despite different names*

```diff
@@ -237,16 +237,16 @@
     def update(self):
         """Update the particle system."""
         j = 0
         for i in range(self.n):
             if self.field[i] == 0.0: continue
             self.toroidal_wrap(i)
             self.limit_speed(i)
-            # self.detect_collisions(i, self.C.COLL_RAD)
-            # self.update_prev(i)
+            self.detect_collisions(i, self.C.COLL_RAD)
+            self.update_prev(i)
             self.active_indexes[j] = i
             j += 1
         self.active_count[None] = j
 
     @ti.func
     def toroidal_wrap(self, i: ti.i32):
         """Toroidal wrap a particle.
```

### Comparing `tolvera-0.1.0rc12/src/tolvera/patches.py` & `tolvera-0.1.0rc8/src/tolvera/patches.py`

 * *Files identical despite different names*

### Comparing `tolvera-0.1.0rc12/src/tolvera/pixels.py` & `tolvera-0.1.0rc8/src/tolvera/pixels.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,15 +25,14 @@
     ```
 """
 
 import taichi as ti
 from typing import Any
 from taichi.lang.matrix import MatrixField
 from taichi.lang.struct import StructField
-from taichi.lang.field import ScalarField
 
 from .utils import CONSTS
 
 vec1 = ti.types.vector(1, ti.f32)
 vec2 = ti.math.vec2
 vec3 = ti.math.vec3
 vec4 = ti.math.vec4
@@ -63,16 +62,16 @@
             **kwargs: Keyword arguments.
                 polygon_mode (str): Polygon mode. Defaults to "crossing".
                 brightness (float): Brightness. Defaults to 1.0. 
         """
         self.tv = tolvera
         self.kwargs = kwargs
         self.polygon_mode = kwargs.get("polygon_mode", "crossing")
-        self.x = kwargs.get("x", self.tv.x)
-        self.y = kwargs.get("y", self.tv.y)
+        self.x = self.tv.x
+        self.y = self.tv.y
         self.px = Pixel.field(shape=(self.x, self.y))
         brightness = kwargs.get("brightness", 1.0)
         self.CONSTS = CONSTS(
             {
                 "BRIGHTNESS": (ti.f32, brightness),
             }
         )
@@ -100,45 +99,14 @@
             self.px.rgba[x, y] = px.px.rgba[x, y]
 
     @ti.kernel
     def f_set(self, px: ti.template()):
         for x, y in ti.ndrange(self.x, self.y):
             self.px.rgba[x, y] = px.px.rgba[x, y]
 
-    @ti.func
-    def stamp(self, x: ti.i32, y: ti.i32, px: ti.template()):
-        """Stamp pixels.
-
-        Args:
-            x (ti.i32): X position.
-            y (ti.i32): Y position.
-            px (ti.template): Pixels to stamp.
-        """
-        for i, j in ti.ndrange(px.px.shape[0], px.px.shape[1]):
-            p = px.px.rgba[i, j]
-            if p[0]+p[1]+p[2] > 0: # transparency
-                self.px.rgba[x + i, y + j] = p
-
-    @ti.kernel
-    def from_numpy(self, img: ti.template()):
-        for x, y in ti.ndrange(self.x, self.y):
-            if img[x, y, 0]+img[x, y, 1]+img[x, y, 2] > 0.:
-                self.px.rgba[x, y] = ti.Vector([
-                    img[x, y, 0]/255.,
-                    img[x, y, 1]/255.,
-                    img[x, y, 2]/255.,
-                    img[x, y, 3]/255.])
-
-    def from_img(self, path: str):
-        img = ti.tools.imread(path)
-        img_fld = ti.field(dtype=ti.f32, shape=img.shape)
-        img_fld.from_numpy(img)
-        self.from_numpy(img_fld)
-        return img_fld
-
     def get(self):
         """Get pixels."""
         return self.px
 
     @ti.kernel
     def clear(self):
         """Clear pixels."""
@@ -209,151 +177,52 @@
         """
         # TODO: fill arg
         # TODO: gradients, lerp with ti.math.mix(x, y, a)
         for i, j in ti.ndrange(w, h):
             self.px.rgba[x + i, y + j] = rgba
 
     @ti.func
-    def stamp(self, x: ti.i32, y: ti.i32, px: ti.template()):
-        """Stamp pixels.
+    def line(self, x0: ti.i32, y0: ti.i32, x1: ti.i32, y1: ti.i32, rgba: vec4):
+        """Draw a line using Bresenham's algorithm.
 
         Args:
-            x (ti.i32): X position.
-            y (ti.i32): Y position.
-            px (ti.template): Pixels to stamp.
-        """
-        for i, j in ti.ndrange(px.px.shape[0], px.px.shape[1]):
-            p = px.px.rgba[i, j]
-            if p[0]+p[1]+p[2] > 0: # transparency
-                self.px.rgba[x + i, y + j] = p
-
-    @ti.func
-    def plot(self, x, y, c, rgba):
-        """Set the pixel color with blending."""
-        self.px.rgba[x, y] = self.px.rgba[x, y] * (1 - c) + rgba * c
-
-    @ti.func
-    def ipart(self, x):
-        return ti.math.floor(x)
-
-    @ti.func
-    def round(self, x):
-        return self.ipart(x + 0.5)
-
-    @ti.func
-    def fpart(self, x):
-        return x - ti.math.floor(x)
-
-    @ti.func
-    def rfpart(self, x):
-        return 1 - self.fpart(x)
-
-    @ti.func
-    def line(self, x0: ti.f32, y0: ti.f32, x1: ti.f32, y1: ti.f32, rgba: vec4):
-        """Draw an anti-aliased line using Xiaolin Wu's algorithm."""
-        steep = ti.abs(y1 - y0) > ti.abs(x1 - x0)
-        if steep:
-            x0, y0 = y0, x0
-            x1, y1 = y1, x1
-
-        if x0 > x1:
-            x0, x1 = x1, x0
-            y0, y1 = y1, y0
-
-        dx = x1 - x0
-        dy = y1 - y0
-        gradient = dy / dx if dx != 0 else 1.0
-
-        xend = ti.math.round(x0)
-        yend = y0 + gradient * (xend - x0)
-        xgap = self.rfpart(x0 + 0.5)
-        xpxl1 = int(xend)
-        ypxl1 = int(self.ipart(yend))
-        if steep:
-            self.plot(ypxl1, xpxl1, self.rfpart(yend) * xgap, rgba)
-            self.plot(ypxl1 + 1, xpxl1, self.fpart(yend) * xgap, rgba)
-        else:
-            self.plot(xpxl1, ypxl1, self.rfpart(yend) * xgap, rgba)
-            self.plot(xpxl1, ypxl1 + 1, self.fpart(yend) * xgap, rgba)
-
-        intery = yend + gradient
-
-        xend = ti.math.round(x1)
-        yend = y1 + gradient * (xend - x1)
-        xgap = self.fpart(x1 + 0.5)
-        xpxl2 = int(xend)
-        ypxl2 = int(self.ipart(yend))
-        if steep:
-            self.plot(ypxl2, xpxl2, self.rfpart(yend) * xgap, rgba)
-            self.plot(ypxl2 + 1, xpxl2, self.fpart(yend) * xgap, rgba)
-        else:
-            self.plot(xpxl2, ypxl2, self.rfpart(yend) * xgap, rgba)
-            self.plot(xpxl2, ypxl2 + 1, self.fpart(yend) * xgap, rgba)
+            x0 (ti.i32): X start position.
+            y0 (ti.i32): Y start position.
+            x1 (ti.i32): X end position.
+            y1 (ti.i32): Y end position.
+            rgba (vec4): Colour.
 
-        if steep:
-            for x in range(xpxl1 + 1, xpxl2):
-                self.plot(int(self.ipart(intery)), x, self.rfpart(intery), rgba)
-                self.plot(int(self.ipart(intery)) + 1, x, self.fpart(intery), rgba)
-                intery += gradient
+        TODO: thickness
+        TODO: anti-aliasing
+        TODO: should lines wrap around (as two lines)?
+        """
+        dx = ti.abs(x1 - x0)
+        dy = ti.abs(y1 - y0)
+        x, y = x0, y0
+        sx = -1 if x0 > x1 else 1
+        sy = -1 if y0 > y1 else 1
+        if dx > dy:
+            err = dx / 2.0
+            while x != x1:
+                self.px.rgba[x, y] = rgba
+                err -= dy
+                if err < 0:
+                    y += sy
+                    err += dx
+                x += sx
         else:
-            for x in range(xpxl1 + 1, xpxl2):
-                self.plot(x, int(self.ipart(intery)), self.rfpart(intery), rgba)
-                self.plot(x, int(self.ipart(intery)) + 1, self.fpart(intery), rgba)
-                intery += gradient
-
-    # @ti.func
-    # def line(self, x0: ti.i32, y0: ti.i32, x1: ti.i32, y1: ti.i32, rgba: vec4):
-    #     """Draw a line using Bresenham's algorithm.
-
-    #     Args:
-    #         x0 (ti.i32): X start position.
-    #         y0 (ti.i32): Y start position.
-    #         x1 (ti.i32): X end position.
-    #         y1 (ti.i32): Y end position.
-    #         rgba (vec4): Colour.
-
-    #     TODO: thickness
-    #     TODO: anti-aliasing
-    #     TODO: should lines wrap around (as two lines)?
-    #     """
-    #     dx = ti.abs(x1 - x0)
-    #     dy = ti.abs(y1 - y0)
-    #     x, y = x0, y0
-    #     sx = -1 if x0 > x1 else 1
-    #     sy = -1 if y0 > y1 else 1
-    #     if dx > dy:
-    #         err = dx / 2.0
-    #         while x != x1:
-    #             self.px.rgba[x, y] = rgba
-    #             err -= dy
-    #             if err < 0:
-    #                 y += sy
-    #                 err += dx
-    #             x += sx
-    #     else:
-    #         err = dy / 2.0
-    #         while y != y1:
-    #             self.px.rgba[x, y] = rgba
-    #             err -= dx
-    #             if err < 0:
-    #                 x += sx
-    #                 err += dy
-    #             y += sy
-    #     self.px.rgba[x, y] = rgba
-
-    @ti.func
-    def lines(self, points: ti.template(), rgba: vec4):
-        """Draw lines with the same colour.
-
-        Args:
-            points (ti.template): Points.
-            rgba (vec4): Colour.
-        """
-        for i in range(points.shape[0] - 1):
-            self.line(points[i][0], points[i][1], points[i + 1][0], points[i + 1][1], rgba)
+            err = dy / 2.0
+            while y != y1:
+                self.px.rgba[x, y] = rgba
+                err -= dx
+                if err < 0:
+                    x += sx
+                    err += dy
+                y += sy
+        self.px.rgba[x, y] = rgba
 
     @ti.func
     def circle(self, x: ti.i32, y: ti.i32, r: ti.i32, rgba: vec4):
         """Draw a filled circle.
 
         Args:
             x (ti.i32): X position.
@@ -783,16 +652,14 @@
         """
         if isinstance(px, Pixels):
             return px.px.rgba
         elif isinstance(px, StructField):
             return px.rgba
         elif isinstance(px, MatrixField):
             return px
-        elif isinstance(px, ScalarField):
-            return px
         else:
             try:
                 return px.px.px.rgba
             except:
                 raise TypeError(f"Cannot find pixel field in {type(px)}")
 
     def __call__(self):
```

### Comparing `tolvera-0.1.0rc12/src/tolvera/sketchbook.py` & `tolvera-0.1.0rc8/src/tolvera/sketchbook.py`

 * *Files identical despite different names*

### Comparing `tolvera-0.1.0rc12/src/tolvera/species.py` & `tolvera-0.1.0rc8/src/tolvera/species.py`

 * *Files identical despite different names*

### Comparing `tolvera-0.1.0rc12/src/tolvera/state.py` & `tolvera-0.1.0rc8/src/tolvera/state.py`

 * *Files identical despite different names*

### Comparing `tolvera-0.1.0rc12/src/tolvera/taichi_.py` & `tolvera-0.1.0rc8/src/tolvera/taichi_.py`

 * *Files 11% similar despite different names*

```diff
@@ -59,17 +59,14 @@
         self.window = ti.ui.Window(
             self.name,
             (self.ctx.x, self.ctx.y),
             fps_limit=self.fps,
             show_window=not self.headless,
         )
         self.canvas = self.window.get_canvas()
-        self.gui = self.window.get_gui()
-        # if self.3D:
-        #   self.scene = self.window.scene() # 3D
 
     def show(self, px):
         """Show Taichi canvas and show window."""
         self.canvas.set_image(px.px.rgba)
         if not self.headless:
             self.window.show()
```

### Comparing `tolvera-0.1.0rc12/src/tolvera/tolvera_.py` & `tolvera-0.1.0rc8/src/tolvera/tolvera_.py`

 * *Files identical despite different names*

### Comparing `tolvera-0.1.0rc12/src/tolvera/utils.py` & `tolvera-0.1.0rc8/src/tolvera/utils.py`

 * *Files identical despite different names*

### Comparing `tolvera-0.1.0rc12/src/tolvera/vera/__init__.py` & `tolvera-0.1.0rc8/src/tolvera/vera/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """The Vera module provides a wrapper for all available forces and behaviours."""
 
 from . import forces
+from . import geom
 from .flock import Flock
+from .flock2 import Flock2
 from .reaction_diffusion import ReactionDiffusion
 from .slime import Slime
 from .particle_life import ParticleLife
 from .swarmalators import Swarmalators
 
 class Vera:
     """The Vera class provides a wrapper for all available forces and behaviours,
@@ -15,23 +17,30 @@
         
         Args:
             tolvera (Tolvera): A Tolvera instance.
             **kwargs: Keyword arguments passed to the Vera.
         """
         self.tv = tolvera
         self.add_forces_to_self()
+        # self.add_geom_to_self()
         self.flock = Flock(tolvera, **kwargs)
+        self.flock2 = Flock2(tolvera, **kwargs)
         self.slime = Slime(tolvera, **kwargs)
         self.rd = ReactionDiffusion(tolvera, **kwargs)
         self.plife = ParticleLife(tolvera, **kwargs)
         self.swarm = Swarmalators(tolvera, **kwargs)
 
     def add_forces_to_self(self):
         """Add all forces to the Vera instance."""
-        for force in forces.__all__:
-            setattr(self, force, getattr(forces, force))
+        for f in forces.__all__:
+            setattr(self, f, getattr(forces, f))
+    
+    def add_geom_to_self(self):
+        """Add all geom functions to the Vera instance."""
+        for g in geom.__all__:
+            setattr(self, g, getattr(geom, g))
 
     def randomise(self):
         """Randomise all forces and behaviours."""
         self.flock.randomise()
         self.slime.randomise()
         self.rd.randomise()
```

### Comparing `tolvera-0.1.0rc12/src/tolvera/vera/flock.py` & `tolvera-0.1.0rc8/src/tolvera/vera/flock.py`

 * *Files identical despite different names*

### Comparing `tolvera-0.1.0rc12/src/tolvera/vera/forces.py` & `tolvera-0.1.0rc8/src/tolvera/vera/forces.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,25 +23,25 @@
     "noise",
     "centripetal",
     "centripetal_particle",
 ]
 
 
 @ti.kernel
-def move(particles: ti.template(), weight: ti.f32):
+def move(particles: ti.template()):
     """Move the particles.
 
     Args:
         particles (ti.template): Particles.
     """
     for i in range(particles.field.shape[0]):
         if particles.field[i].active == 0:
             continue
         p1 = particles.field[i]
-        particles.field[i].pos += p1.vel * p1.speed * p1.active * weight
+        particles.field[i].pos += p1.vel * p1.speed * p1.active
 
 
 @ti.kernel
 def attract(particles: ti.template(), pos: ti.math.vec2, mass: ti.f32, radius: ti.f32):
     """Attract the particles to a position.
 
     Args:
```

### Comparing `tolvera-0.1.0rc12/src/tolvera/vera/particle_life.py` & `tolvera-0.1.0rc8/src/tolvera/vera/particle_life.py`

 * *Files identical despite different names*

### Comparing `tolvera-0.1.0rc12/src/tolvera/vera/reaction_diffusion.py` & `tolvera-0.1.0rc8/src/tolvera/vera/reaction_diffusion.py`

 * *Files identical despite different names*

### Comparing `tolvera-0.1.0rc12/src/tolvera/vera/slime.py` & `tolvera-0.1.0rc8/src/tolvera/vera/slime.py`

 * *Files identical despite different names*

### Comparing `tolvera-0.1.0rc12/src/tolvera/vera/swarmalators.py` & `tolvera-0.1.0rc8/src/tolvera/vera/swarmalators.py`

 * *Files identical despite different names*

### Comparing `tolvera-0.1.0rc12/PKG-INFO` & `tolvera-0.1.0rc8/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,99 +1,80 @@
-Metadata-Version: 2.1
-Name: tolvera
-Version: 0.1.0rc12
-Summary: Tölvera is a library for exploring music interaction with artificial life and self-organising systems.
-Home-page: https://github.com/Intelligent-Instruments-Lab/tolvera
-License: AGPL-3.0
-Author: Jack Armitage
-Author-email: jack.armitage@me.com
-Requires-Python: >=3.10,<3.12
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: anguilla-iml (>=0.1.0b4,<0.2.0)
-Requires-Dist: iipyper (>=0.1.0b1,<0.2.0)
-Requires-Dist: jsons (>=1.6.3,<2.0.0)
-Requires-Dist: mediapipe (==0.10.9)
-Requires-Dist: opencv-python (>=4.8.1.78,<5.0.0.0)
-Requires-Dist: sardine (>=0.0.0b3,<0.0.1)
-Requires-Dist: taichi (>=1.7.0,<2.0.0)
-Requires-Dist: torch (>=2.2.2,<3.0.0)
-Requires-Dist: tqdm (>=4.66.4,<5.0.0)
-Project-URL: Documentation, https://intelligent-instruments-lab.github.io/tolvera/
-Project-URL: Repository, https://github.com/Intelligent-Instruments-Lab/tolvera
-Description-Content-Type: text/markdown
-
 # Tölvera
 
-[Tölvera](https://tolvera.is) is a Python library designed for [composing together](https://arxiv.org/abs/2303.06777) and interacting with [basal](https://royalsocietypublishing.org/doi/full/10.1098/rstb.2019.0750) [agencies](https://link.springer.com/article/10.1007/s00018-023-04790-z), inspired by fields such as artificial life (ALife) and self-organising systems. 
-It provides creative coding-style APIs that allow users to combine and compose various built-in behaviours, such as flocking, slime mold growth, and swarming, and also author their own. 
-With built-in support for Open Sound Control (OSC) via [iipyper](https://github.com/Intelligent-Instruments-Lab/iipyper) and interactive machine learning (IML) via [anguilla](https://github.com/Intelligent-Instruments-Lab/anguilla), Tölvera interfaces with and rapidly maps onto existing creative computing software and hardware, striving to be both an accessible and powerful tool for exploring [diverse intelligence](https://www.frontiersin.org/articles/10.3389/fnsys.2022.768201/full) in artistic contexts.
-
-Inspired by our lab's location in Iceland, the word Tölvera is an Icelandic [kenning](https://en.wikipedia.org/wiki/Kenning) based on _tölva_ meaning computer, from _tala_ (number) and _völva_ (prophetess), and _vera_ (being), composed together as _number being_.
+[Tölvera](https://tolvera.is) is a library for exploring musical performance with artificial life (ALife) and self-organising systems. The word is an Icelandic [kenning](https://en.wikipedia.org/wiki/Kenning):
 
-We have employed Tölvera in various collaborative artistic works, including musical performances, compositions, and multimedia installations (see [`references.bib`](https://github.com/Intelligent-Instruments-Lab/tolvera/blob/main/references.bib) for peer-reviewed publications).
-Tölvera's role in these pieces has mainly been "mappable behaviour engine", where interface inputs can control Tölvera programs, and Tölvera runtime data can control interface outputs, in practically any combination.
-In this way, and to controllable degrees, Tölvera can contribute to the underlying dynamics of a given interactive scenario.
-It can also add a [visual component](https://www.youtube.com/watch?v=W2c8vFmdANY), and equally has been used without projection in [other works](https://marcodonnarumma.com/works/ex-silens/).
+- Tölva = computer, from tala (number) + völva (prophetess)
+- Vera = being
+- Tölvera = number being
 
-Tölvera makes use of [Taichi](https://www.taichi-lang.org/), a domain-specific language embedded in Python that enables parallelisation, and is experimental software subject to change.
+Tölvera is written in [Taichi](https://www.taichi-lang.org/), a domain-specific language embedded in Python.
 
-We would be happy to have you join us on our [Discord](https://discord.gg/ER7tWds9vM) server!
+This is experimental software and everything is currently subject to change.
 
-## Showcase & Examples
+Join us on the Tölvera [Discord](https://discord.gg/ER7tWds9vM).
 
-Examples can be found at [iil-examples/tolvera](https://github.com/Intelligent-Instruments-Lab/iil-examples/tree/main/tolvera).
-See also the [guide](https://intelligent-instruments-lab.github.io/tolvera/guide), [reference](https://intelligent-instruments-lab.github.io/tolvera/reference) and [experiments](https://intelligent-instruments-lab.github.io/tolvera/experiments) pages.
+## Showcase
 
 [Visit the YouTube Playlist](https://www.youtube.com/embed/ahSXjnYHZLU?&list=PL8bdQleKUA1vNez5gw-pfQB21Q1-vHn3x) (if you'd like to add a video, please get in touch).
 
 ![type:video](https://www.youtube.com/embed/ahSXjnYHZLU?&list=PL8bdQleKUA1vNez5gw-pfQB21Q1-vHn3x)
 
 <!-- [![](assets/images/tolvera.jpg)](https://www.youtube.com/watch?v=ahSXjnYHZLU&list=PL8bdQleKUA1vNez5gw-pfQB21Q1-vHn3x&pp=gAQBiAQB) -->
 
+## Features
+
+- `tv.v`: a collection of "vera" (beings) including Move, Flock, Slime and Swarm, with more being continuously added. Vera can be combined and composed in various ways.
+- `tv.p`: extensible particle system. Particles are divided into multiple species, where each species has a unique relationship with every other species, including itself
+- `tv.s`: n-dimensional state structures that can be used by "vera", including built-in OSC and IML creation (see below).
+- `tv.px`: drawing library including various shapes and blend modes, styled similarly to p5.js etc.
+- `tv.osc`: Open Sound Control (OSC) via [iipyper](https://github.com/Intelligent-Instruments-Lab/iipyper), including automated export of OSC schemas to JSON, XML, Pure Data (Pd), Max/MSP (SuperCollider TBC).
+- `tv.iml`: Interactive Machine Learning via [anguilla](https://github.com/Intelligent-Instruments-Lab/anguilla).
+- `tv.ti`: Taichi-based simulation and rendering engine. Can be run "headless" (without graphics).
+- `tv.cv`: computer vision integration based on OpenCV and Mediapipe.
+
+## Examples
+
+Examples can be found at [iil-examples/tolvera](https://github.com/Intelligent-Instruments-Lab/iil-examples/tree/main/tolvera).
+When run as a script, Tölvera program looks like this:
+
+```py
+from tolvera import Tolvera, run
+
+def main(**kwargs):
+    tv = Tolvera(**kwargs)
+
+    @tv.render
+    def _():
+        return tv.px
+
+if __name__ == '__main__':
+    run(main)
+```
+
 ## Install
 
 Taichi [supports numerous operating systems and backends](https://docs.taichi-lang.org/docs/hello_world#supported-systems-and-backends).
 If you plan on using Vulkan for graphics (recommended for macOS), you may need to [install the Vulkan SDK](https://docs.taichi-lang.org/docs/hello_world#supported-systems-and-backends) first and restart your machine.
 
 Tölvera is [registered on PyPI](https://pypi.org/project/tolvera) and can be installed via a Python package manager such as `pip`:
 
 ```sh
 pip install tolvera
 ```
 
 ## Develop
 
-For development, we use [`poetry`](https://python-poetry.org/).
-Fork/clone this repository and install the package with `poetry:
+Fork/clone this repository and install the package with `poetry`:
 
 ```sh
 git clone https://github.com/Intelligent-Instruments-Lab/tolvera # (or clone your own fork)
 cd tolvera
 poetry install
 ```
 
-## Known Issues & Limitations
-
-- Tölvera currently [does not support Python 3.12 and above](https://github.com/taichi-dev/taichi/issues/8365) - a Python 3.11 installation is recommended.
-This can be created in the following way using [miniconda](https://docs.anaconda.com/free/miniconda/index.html):
-```sh
-conda create -n tolvera python=3.11
-conda activate tolvera
-```
-- Tölvera does not support Intel-based Apple devices (due to [`anguilla`](https://github.com/Intelligent-Instruments-Lab/anguilla)'s FAISS dependency, and Mediapipe not supporting Intel Macs).
-- On macOS, [an OpenMP issue](https://github.com/pytorch/pytorch/issues/78490) may prevent Tölvera programs from running, which can be addressed by adding the following environment variable:
-```sh
-export KMP_DUPLICATE_LIB_OK=TRUE
-```
-- Sonification via [SignalFlow](https://signalflow.dev) does not work on Windows.
-- Mediapipe versions [may need to be downgraded](https://github.com/google/mediapipe/issues/5168) in order to work on macOS and Windows.
-
 ## Contribute
 
 We welcome [Pull Requests](https://github.com/Intelligent-Instruments-Lab/tolvera/pulls) across all areas of the project:
 
 - Addressing [Issues](https://github.com/Intelligent-Instruments-Lab/tolvera/issues)
 - Adding features (see [Issues](https://github.com/Intelligent-Instruments-Lab/tolvera/issues) and [Discussion](https://github.com/Intelligent-Instruments-Lab/tolvera/discussion))
 - [Examples](https://github.com/Intelligent-Instruments-Lab/iil-examples/tolvera)
@@ -111,52 +92,61 @@
 Across the project, we follow the [Berlin Code of Conduct](https://berlincodeofconduct.org/). 
 Please get in touch if you experience or witness any conduct issues.
 
 ## Roadmap
 
 See [Discussion](https://github.com/Intelligent-Instruments-Lab/tolvera/discussion).
 
-## Citation
+## Citing
 
-Tölvera is being written about and used in a number of contexts (see [references.bib](https://github.com/Intelligent-Instruments-Lab/tolvera/blob/main/references.bib)).
-The current canonical citation is our [NIME 2024](https://www.nime2024.org/) paper:
+Tölvera is being written about and used in a number of contexts (see [references.bib](https://github.com/Intelligent-Instruments-Lab/tolvera/blob/main/references.bib)), here are a few recent examples:
 
 ```bibtex
-@inproceedings{armitageTolveraComposingBasal2024,
-  title = {T{\"o}lvera: {{Composing With Basal Agencies}}},
-  booktitle = {Proc. {{New Interfaces}} for {{Musical Expression}}},
-  author = {Armitage, Jack and Shepardson, Victor and Magnusson, Thor},
-  year = {2024},
-  address = {Utrecht, NL},
+@inproceedings{armitageAgentialScoresExploring2023,
+  Address = {Boston, Massachusetts, USA},
+  Author = { Jack Armitage and Thor Magnusson },
+  Title = {Agential Scores: Artificial Life for Emergent, Self-Organising and Entangled Music Notation},
+  Booktitle = {Proceedings of the International Conference on Technologies for Music Notation and Representation -- TENOR'2023},
+  Pages = {51 - 61},
+  Year = {2023},
+  Editor = {Anthony Paul De Ritis and Victor Zappi and Jeremy Van Buskirk and John Mallia},
+  Publisher = {Northeastern University},
+  ISBN = {978-0-6481592-7-8}
+}
+
+@inproceedings{armitageStrengjavera2023,
+  title = {Strengjavera},
+  booktitle = {{{AI Music Creativity}} 2023},
+  author = {Armitage, Jack},
+  year = {2023},
+  address = {{University of Sussex, Brighton, UK}},
+  doi = {10.5281/zenodo.8329855},
+  ISBN = {978-0-9957862-9-5},
+  url = {https://zenodo.org/records/8329855}
 }
 ```
 
 ## Inspiration
 
-- [Michael Levin](https://en.wikipedia.org/wiki/Michael_Levin_(biologist))
 - [SwissGL](https://swiss.gl)
 - [Lenia](https://chakazul.github.io/lenia.html)
 - Particle Life (attributed to various, see for example [Clusters](https://www.ventrella.com/Clusters/))
 - [Journey to the Microcosmos](https://www.youtube.com/@journeytomicro)
 - [Complexity Explorables](https://www.complexity-explorables.org/)
 
 ## Contact
 
-Tölvera is developed primarily by [Jack Armitage](https://jackarmitage.com) and [collaborators](https://iil.is/people) at the [Intelligent Instruments Lab](https://iil.is/about). 
-Get in touch to [collaborate](https://iil.is/collaborate):
+`tolvera` is developed by the [Intelligent Instruments Lab](https://iil.is/about). Get in touch to [collaborate](https://iil.is/collaborate):
 
  ◦ <a href="https://iil.is" target="_blank" title="Intelligent Instrumets Lab">iil.is</a> ◦ 
 <a href="https://facebook.com/intelligentinstrumentslab" target="_blank" title="facebook.com">Facebook</a> ◦ 
 <a href="https://instagram.com/intelligentinstruments" target="_blank" title="instagram.com">Instagram</a> ◦ 
 <a href="https://x.com/_iil_is" target="_blank" title="x.com">X (Twitter)</a> ◦ 
 <a href="https://youtube.com/@IntelligentInstruments" target="_blank" title="youtube.com">YouTube</a> ◦ 
 <a href="https://discord.gg/fY9GYMebtJ" target="_blank" title="discord.gg">Discord</a> ◦ 
 <a href="https://github.com/intelligent-instruments-lab" target="_blank" title="github.com">GitHub</a> ◦ 
 <a href="https://www.linkedin.com/company/intelligent-instruments-lab" target="_blank" title="www.linkedin.com">LinkedIn</a> ◦ 
-<a href="mailto:jack@hi.is" target="_blank" title="">Email</a> ◦ 
-
-## Acknowledgements
-
-We thank the Taichi community for their wonderful project, that makes Tölvera possible.
+<a href="mailto:iil@lhi.is" target="_blank" title="">Email</a> ◦ 
 
-The [Intelligent Instruments](https://iil.is) project (INTENT) is funded by the European Research Council (ERC) under the European Union’s Horizon 2020 research and innovation programme (Grant agreement No. 101001848).
+## Funding
 
+The Intelligent Instruments project (INTENT) is funded by the European Research Council (ERC) under the European Union’s Horizon 2020 research and innovation programme (Grant agreement No. 101001848).
```

