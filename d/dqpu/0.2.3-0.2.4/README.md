# Comparing `tmp/dqpu-0.2.3.tar.gz` & `tmp/dqpu-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dqpu-0.2.3.tar", last modified: Mon May 27 05:50:24 2024, max compression
+gzip compressed data, was "dqpu-0.2.4.tar", last modified: Mon May 27 05:55:19 2024, max compression
```

## Comparing `dqpu-0.2.3.tar` & `dqpu-0.2.4.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2024-05-27 05:50:24.467845 dqpu-0.2.3/
--rw-r--r--   0 dakk      (1000) dakk      (1000)    10255 2024-04-30 07:00:05.000000 dqpu-0.2.3/LICENSE
--rw-r--r--   0 dakk      (1000) dakk      (1000)     6958 2024-05-27 05:50:24.467845 dqpu-0.2.3/PKG-INFO
--rw-r--r--   0 dakk      (1000) dakk      (1000)     6130 2024-05-25 07:42:18.000000 dqpu-0.2.3/README.md
-drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2024-05-27 05:50:24.461178 dqpu-0.2.3/dqpu/
--rw-r--r--   0 dakk      (1000) dakk      (1000)      593 2024-05-27 05:48:50.000000 dqpu-0.2.3/dqpu/__init__.py
-drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2024-05-27 05:50:24.461178 dqpu-0.2.3/dqpu/backends/
--rw-r--r--   0 dakk      (1000) dakk      (1000)      569 2024-05-17 14:08:15.000000 dqpu-0.2.3/dqpu/backends/__init__.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     1234 2024-05-19 08:07:22.000000 dqpu-0.2.3/dqpu/backends/base.py
-drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2024-05-27 05:50:24.464512 dqpu-0.2.3/dqpu/backends/qiskit/
--rw-r--r--   0 dakk      (1000) dakk      (1000)      717 2024-05-17 11:37:05.000000 dqpu-0.2.3/dqpu/backends/qiskit/__init__.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     4026 2024-05-23 09:22:47.000000 dqpu-0.2.3/dqpu/backends/qiskit/dqpubackend.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     3288 2024-05-20 10:03:30.000000 dqpu-0.2.3/dqpu/backends/qiskit/dqpujob.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     1198 2024-05-19 08:07:22.000000 dqpu-0.2.3/dqpu/backends/qiskit/dqpuprovider.py
-drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2024-05-27 05:50:24.464512 dqpu-0.2.3/dqpu/blockchain/
--rw-r--r--   0 dakk      (1000) dakk      (1000)      726 2024-05-15 08:24:53.000000 dqpu-0.2.3/dqpu/blockchain/__init__.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     1531 2024-05-22 06:01:25.000000 dqpu-0.2.3/dqpu/blockchain/blockchain.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     2495 2024-05-22 14:41:31.000000 dqpu-0.2.3/dqpu/blockchain/ipfs_gateway.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     6404 2024-05-23 09:41:09.000000 dqpu-0.2.3/dqpu/blockchain/near.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     7053 2024-05-25 13:21:17.000000 dqpu-0.2.3/dqpu/cli.py
-drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2024-05-27 05:50:24.464512 dqpu-0.2.3/dqpu/q/
--rw-r--r--   0 dakk      (1000) dakk      (1000)      801 2024-05-07 07:05:38.000000 dqpu-0.2.3/dqpu/q/__init__.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     6613 2024-05-23 09:41:41.000000 dqpu-0.2.3/dqpu/q/circuit.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     1260 2024-05-23 08:49:53.000000 dqpu-0.2.3/dqpu/q/gate.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     2322 2024-05-23 09:22:47.000000 dqpu-0.2.3/dqpu/q/gates.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     2262 2024-05-14 10:21:28.000000 dqpu-0.2.3/dqpu/q/utils.py
-drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2024-05-27 05:50:24.467845 dqpu-0.2.3/dqpu/sampler/
--rw-r--r--   0 dakk      (1000) dakk      (1000)      969 2024-05-23 09:41:33.000000 dqpu-0.2.3/dqpu/sampler/__init__.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     1072 2024-05-23 09:22:47.000000 dqpu-0.2.3/dqpu/sampler/aersimulatorsampler.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     5943 2024-05-15 10:21:58.000000 dqpu-0.2.3/dqpu/sampler/dasksimulatorsampler.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     1185 2024-05-23 09:22:47.000000 dqpu-0.2.3/dqpu/sampler/qracksimulatorsampler.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     1484 2024-05-22 06:06:47.000000 dqpu-0.2.3/dqpu/sampler/sampler.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     6025 2024-05-23 09:22:47.000000 dqpu-0.2.3/dqpu/samplernode.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     1636 2024-05-23 09:22:47.000000 dqpu-0.2.3/dqpu/utils.py
-drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2024-05-27 05:50:24.467845 dqpu-0.2.3/dqpu/verifier/
--rw-r--r--   0 dakk      (1000) dakk      (1000)      691 2024-05-07 08:01:59.000000 dqpu-0.2.3/dqpu/verifier/__init__.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     4158 2024-05-23 09:33:18.000000 dqpu-0.2.3/dqpu/verifier/basictrapper.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     2322 2024-05-19 07:59:25.000000 dqpu-0.2.3/dqpu/verifier/trapper.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)      652 2024-05-07 05:50:44.000000 dqpu-0.2.3/dqpu/verifier/verifier.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     6374 2024-05-23 09:41:33.000000 dqpu-0.2.3/dqpu/verifiernode.py
-drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2024-05-27 05:50:24.461178 dqpu-0.2.3/dqpu.egg-info/
--rw-r--r--   0 dakk      (1000) dakk      (1000)     6958 2024-05-27 05:50:24.000000 dqpu-0.2.3/dqpu.egg-info/PKG-INFO
--rw-r--r--   0 dakk      (1000) dakk      (1000)      987 2024-05-27 05:50:24.000000 dqpu-0.2.3/dqpu.egg-info/SOURCES.txt
--rw-r--r--   0 dakk      (1000) dakk      (1000)        1 2024-05-27 05:50:24.000000 dqpu-0.2.3/dqpu.egg-info/dependency_links.txt
--rw-r--r--   0 dakk      (1000) dakk      (1000)      190 2024-05-27 05:50:24.000000 dqpu-0.2.3/dqpu.egg-info/entry_points.txt
--rw-r--r--   0 dakk      (1000) dakk      (1000)        1 2024-05-27 05:50:23.000000 dqpu-0.2.3/dqpu.egg-info/not-zip-safe
--rw-r--r--   0 dakk      (1000) dakk      (1000)      194 2024-05-27 05:50:24.000000 dqpu-0.2.3/dqpu.egg-info/requires.txt
--rw-r--r--   0 dakk      (1000) dakk      (1000)        5 2024-05-27 05:50:24.000000 dqpu-0.2.3/dqpu.egg-info/top_level.txt
--rw-r--r--   0 dakk      (1000) dakk      (1000)      382 2024-05-27 05:50:24.471179 dqpu-0.2.3/setup.cfg
--rw-r--r--   0 dakk      (1000) dakk      (1000)     3198 2024-05-22 05:34:05.000000 dqpu-0.2.3/setup.py
-drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2024-05-27 05:50:24.467845 dqpu-0.2.3/test/
--rw-r--r--   0 dakk      (1000) dakk      (1000)      741 2024-05-07 08:37:08.000000 dqpu-0.2.3/test/test_empty.py
+drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2024-05-27 05:55:19.007839 dqpu-0.2.4/
+-rw-r--r--   0 dakk      (1000) dakk      (1000)    10255 2024-04-30 07:00:05.000000 dqpu-0.2.4/LICENSE
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     6958 2024-05-27 05:55:19.007839 dqpu-0.2.4/PKG-INFO
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     6130 2024-05-25 07:42:18.000000 dqpu-0.2.4/README.md
+drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2024-05-27 05:55:18.997838 dqpu-0.2.4/dqpu/
+-rw-r--r--   0 dakk      (1000) dakk      (1000)      593 2024-05-27 05:54:56.000000 dqpu-0.2.4/dqpu/__init__.py
+drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2024-05-27 05:55:19.001172 dqpu-0.2.4/dqpu/backends/
+-rw-r--r--   0 dakk      (1000) dakk      (1000)      569 2024-05-17 14:08:15.000000 dqpu-0.2.4/dqpu/backends/__init__.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     1234 2024-05-19 08:07:22.000000 dqpu-0.2.4/dqpu/backends/base.py
+drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2024-05-27 05:55:19.001172 dqpu-0.2.4/dqpu/backends/qiskit/
+-rw-r--r--   0 dakk      (1000) dakk      (1000)      717 2024-05-17 11:37:05.000000 dqpu-0.2.4/dqpu/backends/qiskit/__init__.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     4026 2024-05-23 09:22:47.000000 dqpu-0.2.4/dqpu/backends/qiskit/dqpubackend.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     3288 2024-05-20 10:03:30.000000 dqpu-0.2.4/dqpu/backends/qiskit/dqpujob.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     1198 2024-05-19 08:07:22.000000 dqpu-0.2.4/dqpu/backends/qiskit/dqpuprovider.py
+drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2024-05-27 05:55:19.004505 dqpu-0.2.4/dqpu/blockchain/
+-rw-r--r--   0 dakk      (1000) dakk      (1000)      726 2024-05-15 08:24:53.000000 dqpu-0.2.4/dqpu/blockchain/__init__.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     1531 2024-05-22 06:01:25.000000 dqpu-0.2.4/dqpu/blockchain/blockchain.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     2495 2024-05-22 14:41:31.000000 dqpu-0.2.4/dqpu/blockchain/ipfs_gateway.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     6404 2024-05-23 09:41:09.000000 dqpu-0.2.4/dqpu/blockchain/near.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     7053 2024-05-25 13:21:17.000000 dqpu-0.2.4/dqpu/cli.py
+drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2024-05-27 05:55:19.004505 dqpu-0.2.4/dqpu/q/
+-rw-r--r--   0 dakk      (1000) dakk      (1000)      801 2024-05-07 07:05:38.000000 dqpu-0.2.4/dqpu/q/__init__.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     6613 2024-05-23 09:41:41.000000 dqpu-0.2.4/dqpu/q/circuit.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     1260 2024-05-23 08:49:53.000000 dqpu-0.2.4/dqpu/q/gate.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     2322 2024-05-23 09:22:47.000000 dqpu-0.2.4/dqpu/q/gates.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     2262 2024-05-14 10:21:28.000000 dqpu-0.2.4/dqpu/q/utils.py
+drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2024-05-27 05:55:19.004505 dqpu-0.2.4/dqpu/sampler/
+-rw-r--r--   0 dakk      (1000) dakk      (1000)      969 2024-05-23 09:41:33.000000 dqpu-0.2.4/dqpu/sampler/__init__.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     1072 2024-05-23 09:22:47.000000 dqpu-0.2.4/dqpu/sampler/aersimulatorsampler.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     5943 2024-05-15 10:21:58.000000 dqpu-0.2.4/dqpu/sampler/dasksimulatorsampler.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     1185 2024-05-23 09:22:47.000000 dqpu-0.2.4/dqpu/sampler/qracksimulatorsampler.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     1484 2024-05-22 06:06:47.000000 dqpu-0.2.4/dqpu/sampler/sampler.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     6025 2024-05-23 09:22:47.000000 dqpu-0.2.4/dqpu/samplernode.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     1636 2024-05-23 09:22:47.000000 dqpu-0.2.4/dqpu/utils.py
+drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2024-05-27 05:55:19.007839 dqpu-0.2.4/dqpu/verifier/
+-rw-r--r--   0 dakk      (1000) dakk      (1000)      691 2024-05-07 08:01:59.000000 dqpu-0.2.4/dqpu/verifier/__init__.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     4158 2024-05-23 09:33:18.000000 dqpu-0.2.4/dqpu/verifier/basictrapper.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     2322 2024-05-19 07:59:25.000000 dqpu-0.2.4/dqpu/verifier/trapper.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)      652 2024-05-07 05:50:44.000000 dqpu-0.2.4/dqpu/verifier/verifier.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     6374 2024-05-23 09:41:33.000000 dqpu-0.2.4/dqpu/verifiernode.py
+drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2024-05-27 05:55:19.001172 dqpu-0.2.4/dqpu.egg-info/
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     6958 2024-05-27 05:55:18.000000 dqpu-0.2.4/dqpu.egg-info/PKG-INFO
+-rw-r--r--   0 dakk      (1000) dakk      (1000)      987 2024-05-27 05:55:18.000000 dqpu-0.2.4/dqpu.egg-info/SOURCES.txt
+-rw-r--r--   0 dakk      (1000) dakk      (1000)        1 2024-05-27 05:55:18.000000 dqpu-0.2.4/dqpu.egg-info/dependency_links.txt
+-rw-r--r--   0 dakk      (1000) dakk      (1000)      190 2024-05-27 05:55:18.000000 dqpu-0.2.4/dqpu.egg-info/entry_points.txt
+-rw-r--r--   0 dakk      (1000) dakk      (1000)        1 2024-05-27 05:55:18.000000 dqpu-0.2.4/dqpu.egg-info/not-zip-safe
+-rw-r--r--   0 dakk      (1000) dakk      (1000)      194 2024-05-27 05:55:18.000000 dqpu-0.2.4/dqpu.egg-info/requires.txt
+-rw-r--r--   0 dakk      (1000) dakk      (1000)        5 2024-05-27 05:55:18.000000 dqpu-0.2.4/dqpu.egg-info/top_level.txt
+-rw-r--r--   0 dakk      (1000) dakk      (1000)      382 2024-05-27 05:55:19.007839 dqpu-0.2.4/setup.cfg
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     3516 2024-05-27 05:54:47.000000 dqpu-0.2.4/setup.py
+drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2024-05-27 05:55:19.007839 dqpu-0.2.4/test/
+-rw-r--r--   0 dakk      (1000) dakk      (1000)      741 2024-05-07 08:37:08.000000 dqpu-0.2.4/test/test_empty.py
```

### Comparing `dqpu-0.2.3/LICENSE` & `dqpu-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.3/PKG-INFO` & `dqpu-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dqpu
-Version: 0.2.3
+Version: 0.2.4
 Home-page: https://github.com/dakk/dqpu
 Author: Davide Gessa
 Author-email: gessadavide@gmail.com
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/dakk/dqpu/issues/
 Project-URL: Documentation, https://dakk.github.io/dqpu
 Project-URL: Source, https://github.com/dakk/dqpu
```

### Comparing `dqpu-0.2.3/README.md` & `dqpu-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.3/dqpu/__init__.py` & `dqpu-0.2.4/dqpu/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = "0.2.3"
+__version__ = "0.2.4"
```

### Comparing `dqpu-0.2.3/dqpu/backends/__init__.py` & `dqpu-0.2.4/dqpu/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.3/dqpu/backends/base.py` & `dqpu-0.2.4/dqpu/backends/base.py`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.3/dqpu/backends/qiskit/__init__.py` & `dqpu-0.2.4/dqpu/backends/qiskit/__init__.py`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.3/dqpu/backends/qiskit/dqpubackend.py` & `dqpu-0.2.4/dqpu/backends/qiskit/dqpubackend.py`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.3/dqpu/backends/qiskit/dqpujob.py` & `dqpu-0.2.4/dqpu/backends/qiskit/dqpujob.py`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.3/dqpu/backends/qiskit/dqpuprovider.py` & `dqpu-0.2.4/dqpu/backends/qiskit/dqpuprovider.py`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.3/dqpu/blockchain/__init__.py` & `dqpu-0.2.4/dqpu/blockchain/__init__.py`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.3/dqpu/blockchain/blockchain.py` & `dqpu-0.2.4/dqpu/blockchain/blockchain.py`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.3/dqpu/blockchain/ipfs_gateway.py` & `dqpu-0.2.4/dqpu/blockchain/ipfs_gateway.py`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.3/dqpu/blockchain/near.py` & `dqpu-0.2.4/dqpu/blockchain/near.py`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.3/dqpu/cli.py` & `dqpu-0.2.4/dqpu/cli.py`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.3/dqpu/q/__init__.py` & `dqpu-0.2.4/dqpu/q/__init__.py`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.3/dqpu/q/circuit.py` & `dqpu-0.2.4/dqpu/q/circuit.py`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.3/dqpu/q/gate.py` & `dqpu-0.2.4/dqpu/q/gate.py`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.3/dqpu/q/gates.py` & `dqpu-0.2.4/dqpu/q/gates.py`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.3/dqpu/q/utils.py` & `dqpu-0.2.4/dqpu/q/utils.py`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.3/dqpu/sampler/__init__.py` & `dqpu-0.2.4/dqpu/sampler/__init__.py`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.3/dqpu/sampler/aersimulatorsampler.py` & `dqpu-0.2.4/dqpu/sampler/aersimulatorsampler.py`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.3/dqpu/sampler/dasksimulatorsampler.py` & `dqpu-0.2.4/dqpu/sampler/dasksimulatorsampler.py`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.3/dqpu/sampler/qracksimulatorsampler.py` & `dqpu-0.2.4/dqpu/sampler/qracksimulatorsampler.py`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.3/dqpu/sampler/sampler.py` & `dqpu-0.2.4/dqpu/sampler/sampler.py`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.3/dqpu/samplernode.py` & `dqpu-0.2.4/dqpu/samplernode.py`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.3/dqpu/utils.py` & `dqpu-0.2.4/dqpu/utils.py`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.3/dqpu/verifier/__init__.py` & `dqpu-0.2.4/dqpu/verifier/__init__.py`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.3/dqpu/verifier/basictrapper.py` & `dqpu-0.2.4/dqpu/verifier/basictrapper.py`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.3/dqpu/verifier/trapper.py` & `dqpu-0.2.4/dqpu/verifier/trapper.py`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.3/dqpu/verifier/verifier.py` & `dqpu-0.2.4/dqpu/verifier/verifier.py`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.3/dqpu/verifiernode.py` & `dqpu-0.2.4/dqpu/verifiernode.py`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.3/dqpu.egg-info/PKG-INFO` & `dqpu-0.2.4/dqpu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dqpu
-Version: 0.2.3
+Version: 0.2.4
 Home-page: https://github.com/dakk/dqpu
 Author: Davide Gessa
 Author-email: gessadavide@gmail.com
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/dakk/dqpu/issues/
 Project-URL: Documentation, https://dakk.github.io/dqpu
 Project-URL: Source, https://github.com/dakk/dqpu
```

### Comparing `dqpu-0.2.3/dqpu.egg-info/SOURCES.txt` & `dqpu-0.2.4/dqpu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.3/setup.py` & `dqpu-0.2.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -47,14 +47,33 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from setuptools import setup
 
 import dqpu
 
+REQUIREMENTS = [
+    #"dask[distributed]==2024.4.2",
+    "scipy==1.13.0",
+    "matplotlib",
+    "qiskit==1.0.2",
+    "qiskit_aer==0.14.1",
+    "py-near",
+    "requests",
+    "numpy==1.26.4",
+    "openqasm3[parser]",
+    "scikit-build",
+    "base58",
+    "loguru",
+    "pydantic",
+    "nest_asyncio",
+    "pyqrack",
+    "qiskit-qrack-provider>=0.11.0"
+]
+
 setup(
     name="dqpu",
     version=dqpu.__version__,
     python_requires=">= 3.9.2",
     description="",
     long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
@@ -68,15 +87,15 @@
         "dqpu.sampler",
         "dqpu.verifier",
         "dqpu.blockchain",
         "dqpu.backends",
         "dqpu.backends.qiskit",
     ],
     zip_safe=False,
-    install_requires=open("requirements.txt", "r").read().split("\n"),
+    install_requires=REQUIREMENTS,
     extras_require={},
     entry_points={
         "console_scripts": [
             "dqpu-sim_trap_test_main = dqpu.sim_trap_test_main:main",
             "dqpu-verifier = dqpu.verifiernode:verifier_node",
             "dqpu-sampler = dqpu.samplernode:sampler_node",
             "dqpu-cli = dqpu.cli:cli",
```

### Comparing `dqpu-0.2.3/test/test_empty.py` & `dqpu-0.2.4/test/test_empty.py`

 * *Files identical despite different names*

