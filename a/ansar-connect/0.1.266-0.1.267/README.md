# Comparing `tmp/ansar_connect-0.1.266.tar.gz` & `tmp/ansar_connect-0.1.267.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansar_connect-0.1.266.tar", last modified: Sun May 26 07:38:09 2024, max compression
+gzip compressed data, was "ansar_connect-0.1.267.tar", last modified: Sun May 26 20:21:59 2024, max compression
```

## Comparing `ansar_connect-0.1.266.tar` & `ansar_connect-0.1.267.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-26 07:38:09.155658 ansar_connect-0.1.266/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.266/LICENSE
--rw-r--r--   0 scott     (1000) scott     (1000)     1342 2024-05-26 07:38:09.155658 ansar_connect-0.1.266/PKG-INFO
--rwxrwxr-x   0 scott     (1000) scott     (1000)      577 2024-05-23 01:07:25.000000 ansar_connect-0.1.266/README.md
--rwxrwxr-x   0 scott     (1000) scott     (1000)      764 2024-05-26 07:28:48.000000 ansar_connect-0.1.266/pyproject.toml
--rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-05-26 07:38:09.155658 ansar_connect-0.1.266/setup.cfg
--rwxrwxr-x   0 scott     (1000) scott     (1000)     2251 2024-05-26 07:28:40.000000 ansar_connect-0.1.266/setup.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-26 07:38:09.151658 ansar_connect-0.1.266/src/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-26 07:38:09.151658 ansar_connect-0.1.266/src/ansar/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-26 07:38:09.151658 ansar_connect-0.1.266/src/ansar/command/
--rw-rw-r--   0 scott     (1000) scott     (1000)    14549 2024-04-18 02:21:13.000000 ansar_connect-0.1.266/src/ansar/command/ansar_command.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3497 2024-05-18 00:58:30.000000 ansar_connect-0.1.266/src/ansar/command/ansar_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.266/src/ansar/command/ansar_group.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9088 2024-05-18 00:58:30.000000 ansar_connect-0.1.266/src/ansar/command/shared_directory.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-26 07:38:09.151658 ansar_connect-0.1.266/src/ansar/connect/
--rwxrwxr-x   0 scott     (1000) scott     (1000)     3012 2024-05-26 07:38:06.000000 ansar_connect-0.1.266/src/ansar/connect/__init__.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14072 2024-04-18 00:04:05.000000 ansar_connect-0.1.266/src/ansar/connect/connect_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    88764 2024-05-24 02:37:42.000000 ansar_connect-0.1.266/src/ansar/connect/directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    12616 2024-05-18 21:27:31.000000 ansar_connect-0.1.266/src/ansar/connect/directory_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    10503 2024-05-19 15:01:15.000000 ansar_connect-0.1.266/src/ansar/connect/foh_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2192 2024-04-18 00:04:05.000000 ansar_connect-0.1.266/src/ansar/connect/group_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    15853 2024-05-20 01:19:54.000000 ansar_connect-0.1.266/src/ansar/connect/grouping.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.266/src/ansar/connect/moving.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    23051 2024-05-19 00:29:25.000000 ansar_connect-0.1.266/src/ansar/connect/networking.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.266/src/ansar/connect/networking_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9679 2024-05-26 07:36:57.000000 ansar_connect-0.1.266/src/ansar/connect/node.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.266/src/ansar/connect/plumbing.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    34158 2024-05-20 23:55:13.000000 ansar_connect-0.1.266/src/ansar/connect/procedure.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2397 2024-04-17 22:27:55.000000 ansar_connect-0.1.266/src/ansar/connect/product.py
--rwxrwxr-x   0 scott     (1000) scott     (1000)    42336 2024-05-26 07:25:14.000000 ansar_connect-0.1.266/src/ansar/connect/socketry.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.266/src/ansar/connect/standard.py
--rwxrwxr-x   0 scott     (1000) scott     (1000)     2804 2024-05-18 21:19:19.000000 ansar_connect-0.1.266/src/ansar/connect/transporting.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1289 2024-04-17 04:02:16.000000 ansar_connect-0.1.266/src/ansar/connect/transporting_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     6602 2024-05-07 01:18:28.000000 ansar_connect-0.1.266/src/ansar/connect/wan.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-26 07:38:09.155658 ansar_connect-0.1.266/src/ansar_connect.egg-info/
--rw-r--r--   0 scott     (1000) scott     (1000)     1342 2024-05-26 07:38:09.000000 ansar_connect-0.1.266/src/ansar_connect.egg-info/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)     1021 2024-05-26 07:38:09.000000 ansar_connect-0.1.266/src/ansar_connect.egg-info/SOURCES.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-05-26 07:38:09.000000 ansar_connect-0.1.266/src/ansar_connect.egg-info/dependency_links.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-05-26 07:38:09.000000 ansar_connect-0.1.266/src/ansar_connect.egg-info/entry_points.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       48 2024-05-26 07:38:09.000000 ansar_connect-0.1.266/src/ansar_connect.egg-info/requires.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-05-26 07:38:09.000000 ansar_connect-0.1.266/src/ansar_connect.egg-info/top_level.txt
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-26 20:21:59.519556 ansar_connect-0.1.267/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.267/LICENSE
+-rw-r--r--   0 scott     (1000) scott     (1000)     1342 2024-05-26 20:21:59.519556 ansar_connect-0.1.267/PKG-INFO
+-rwxrwxr-x   0 scott     (1000) scott     (1000)      577 2024-05-23 01:07:25.000000 ansar_connect-0.1.267/README.md
+-rwxrwxr-x   0 scott     (1000) scott     (1000)      764 2024-05-26 07:28:48.000000 ansar_connect-0.1.267/pyproject.toml
+-rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-05-26 20:21:59.519556 ansar_connect-0.1.267/setup.cfg
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     2251 2024-05-26 07:28:40.000000 ansar_connect-0.1.267/setup.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-26 20:21:59.519556 ansar_connect-0.1.267/src/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-26 20:21:59.519556 ansar_connect-0.1.267/src/ansar/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-26 20:21:59.519556 ansar_connect-0.1.267/src/ansar/command/
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14549 2024-04-18 02:21:13.000000 ansar_connect-0.1.267/src/ansar/command/ansar_command.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3497 2024-05-18 00:58:30.000000 ansar_connect-0.1.267/src/ansar/command/ansar_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9946 2024-05-26 20:11:05.000000 ansar_connect-0.1.267/src/ansar/command/ansar_group.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9088 2024-05-18 00:58:30.000000 ansar_connect-0.1.267/src/ansar/command/shared_directory.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-26 20:21:59.519556 ansar_connect-0.1.267/src/ansar/connect/
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     3012 2024-05-26 20:21:56.000000 ansar_connect-0.1.267/src/ansar/connect/__init__.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14103 2024-05-26 20:11:05.000000 ansar_connect-0.1.267/src/ansar/connect/connect_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    88764 2024-05-24 02:37:42.000000 ansar_connect-0.1.267/src/ansar/connect/directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    12616 2024-05-18 21:27:31.000000 ansar_connect-0.1.267/src/ansar/connect/directory_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    10503 2024-05-19 15:01:15.000000 ansar_connect-0.1.267/src/ansar/connect/foh_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2192 2024-04-18 00:04:05.000000 ansar_connect-0.1.267/src/ansar/connect/group_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    15870 2024-05-26 20:11:05.000000 ansar_connect-0.1.267/src/ansar/connect/grouping.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.267/src/ansar/connect/moving.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    23196 2024-05-26 20:11:05.000000 ansar_connect-0.1.267/src/ansar/connect/networking.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.267/src/ansar/connect/networking_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9679 2024-05-26 07:36:57.000000 ansar_connect-0.1.267/src/ansar/connect/node.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.267/src/ansar/connect/plumbing.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    34158 2024-05-20 23:55:13.000000 ansar_connect-0.1.267/src/ansar/connect/procedure.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2397 2024-04-17 22:27:55.000000 ansar_connect-0.1.267/src/ansar/connect/product.py
+-rwxrwxr-x   0 scott     (1000) scott     (1000)    42336 2024-05-26 07:25:14.000000 ansar_connect-0.1.267/src/ansar/connect/socketry.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.267/src/ansar/connect/standard.py
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     2804 2024-05-18 21:19:19.000000 ansar_connect-0.1.267/src/ansar/connect/transporting.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1289 2024-04-17 04:02:16.000000 ansar_connect-0.1.267/src/ansar/connect/transporting_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     6602 2024-05-07 01:18:28.000000 ansar_connect-0.1.267/src/ansar/connect/wan.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-26 20:21:59.519556 ansar_connect-0.1.267/src/ansar_connect.egg-info/
+-rw-r--r--   0 scott     (1000) scott     (1000)     1342 2024-05-26 20:21:59.000000 ansar_connect-0.1.267/src/ansar_connect.egg-info/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1021 2024-05-26 20:21:59.000000 ansar_connect-0.1.267/src/ansar_connect.egg-info/SOURCES.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-05-26 20:21:59.000000 ansar_connect-0.1.267/src/ansar_connect.egg-info/dependency_links.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-05-26 20:21:59.000000 ansar_connect-0.1.267/src/ansar_connect.egg-info/entry_points.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       48 2024-05-26 20:21:59.000000 ansar_connect-0.1.267/src/ansar_connect.egg-info/requires.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-05-26 20:21:59.000000 ansar_connect-0.1.267/src/ansar_connect.egg-info/top_level.txt
```

### Comparing `ansar_connect-0.1.266/LICENSE` & `ansar_connect-0.1.267/LICENSE`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.266/PKG-INFO` & `ansar_connect-0.1.267/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.266
+Version: 0.1.267
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_connect-0.1.266/README.md` & `ansar_connect-0.1.267/README.md`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.266/pyproject.toml` & `ansar_connect-0.1.267/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.266/setup.py` & `ansar_connect-0.1.267/setup.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.266/src/ansar/command/ansar_command.py` & `ansar_connect-0.1.267/src/ansar/command/ansar_command.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.266/src/ansar/command/ansar_directory.py` & `ansar_connect-0.1.267/src/ansar/command/ansar_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.266/src/ansar/command/ansar_group.py` & `ansar_connect-0.1.267/src/ansar/command/ansar_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,17 +58,17 @@
 		return None
 	if retry.first_steps or retry.regular_steps:
 		return retry
 	return None
 
 #
 #
-class Group(ar.Point, ar.StateMachine):
+class Group(ar.Threaded, ar.StateMachine):
 	def __init__(self, settings):
-		ar.Point.__init__(self)
+		ar.Threaded.__init__(self)
 		ar.StateMachine.__init__(self, INITIAL)
 		self.settings = settings
 		self.group_roles = None			# Names of processes to be maintained.
 		self.main_role = None
 		self.group_start = None			# Moment the first process was started.
 		self.directory_ipp = None
 		self.directory = None
```

### Comparing `ansar_connect-0.1.266/src/ansar/command/shared_directory.py` & `ansar_connect-0.1.267/src/ansar/command/shared_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.266/src/ansar/connect/__init__.py` & `ansar_connect-0.1.267/src/ansar/connect/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Tools and runtime for asynchronous programming.
 
 Repo: git@github.com:mr-ansar/ansar-connect.git
 Branch: main
-Commit: fefa41b6bd9182a9d813f24c0b5168016251bc66
-Version: 0.1.265 (2024-05-26@19:38:06+NZST)
+Commit: bb665d21b8f0dbd57df14a1b012560fbd544a2f4
+Version: 0.1.266 (2024-05-27@08:21:56+NZST)
 """
 
 from ansar.create import *
 
 #bind = bind_any
 #create = create_object
```

### Comparing `ansar_connect-0.1.266/src/ansar/connect/connect_directory.py` & `ansar_connect-0.1.267/src/ansar/connect/connect_directory.py`

 * *Files 0% similar despite different names*

```diff
@@ -495,8 +495,8 @@
 		(Closed, Abandoned, ar.Stop), ()
 	),
 	CLOSING: (
 		(ar.Unknown, Abandoned, Closed), ()
 	),
 }
 
-ar.bind(ConnectToDirectory, CONNECT_TO_DIRECTORY_DISPATCH)
+ar.bind(ConnectToDirectory, CONNECT_TO_DIRECTORY_DISPATCH, thread='connect-to-directory')
```

### Comparing `ansar_connect-0.1.266/src/ansar/connect/directory.py` & `ansar_connect-0.1.267/src/ansar/connect/directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.266/src/ansar/connect/directory_if.py` & `ansar_connect-0.1.267/src/ansar/connect/directory_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.266/src/ansar/connect/foh_if.py` & `ansar_connect-0.1.267/src/ansar/connect/foh_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.266/src/ansar/connect/group_if.py` & `ansar_connect-0.1.267/src/ansar/connect/group_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.266/src/ansar/connect/grouping.py` & `ansar_connect-0.1.267/src/ansar/connect/grouping.py`

 * *Files 0% similar despite different names*

```diff
@@ -465,15 +465,15 @@
 		(ar.Ack, ar.Stop), (ar.Completed, NoAddress, UseAddress)
 	),
 	CLEARING: (
 		(ar.Completed,), ()
 	),
 }
 
-ar.bind(AddressGroup, ADDRESS_GROUP_DISPATCH)
+ar.bind(AddressGroup, ADDRESS_GROUP_DISPATCH, 'address-group')
 
 # Reinstated. Too many existing uses.
 # To be considered deleted.
 
 # A shim object between create_object() and the application object.
 # This is the most concise way to run an object with the support
 # of one or more runtime objects, e.g. a connection to a service.
```

### Comparing `ansar_connect-0.1.266/src/ansar/connect/moving.py` & `ansar_connect-0.1.267/src/ansar/connect/moving.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.266/src/ansar/connect/networking.py` & `ansar_connect-0.1.267/src/ansar/connect/networking.py`

 * *Files 2% similar despite different names*

```diff
@@ -222,15 +222,15 @@
 		(ar.Unknown, GlareTimer, ar.Stop), ()
 	),
 	CLOSING: (
 		(ar.Unknown, Abandoned, Closed), ()
 	),
 }
 
-ar.bind(ConnectToAddress, CONNECT_TO_ADDRESS_DISPATCH)
+ar.bind(ConnectToAddress, CONNECT_TO_ADDRESS_DISPATCH, thread='networking-session')
 
 #
 #
 LISTEN_RETRY = ar.RetryIntervals(first_steps=[], regular_steps=4.0, randomized=0.25)
 
 class ListenAtAddress(ar.Point, ar.StateMachine):
 	"""Maintain a network presence at an IP address and port.
@@ -389,15 +389,15 @@
 		(ar.Unknown, GlareTimer, ar.Stop), ()
 	),
 	CLOSING: (
 		(Abandoned, Closed), ()
 	),
 }
 
-ar.bind(ListenAtAddress, LISTEN_AT_ADDRESS_DISPATCH)
+ar.bind(ListenAtAddress, LISTEN_AT_ADDRESS_DISPATCH, thread='networking-session')
 
 #
 # Subscribe/Publish
 class SubscribeToListing(ar.Point, ar.StateMachine):
 	"""Maintain a connection to a published name.
 
 	:param listing: the name of interest (not a regular expression)
@@ -559,15 +559,15 @@
 		(ar.Unknown, Dropped, Cleared, ar.Stop), ()
 	),
 	CLOSING: (
 		(ar.Unknown, Abandoned, Closed), ()
 	),
 }
 
-ar.bind(SubscribeToListing, SUBSCRIBE_TO_LISTING_DISPATCH)
+ar.bind(SubscribeToListing, SUBSCRIBE_TO_LISTING_DISPATCH, thread='networking-session')
 
 #
 #
 class PublishAListing(ar.Point, ar.StateMachine):
 	"""Maintain a network presence at a name.
 
 	:param listing: the name this object will be known by
@@ -703,15 +703,15 @@
 		(Delivered, ar.Unknown, Dropped, Cleared, ar.Stop), ()
 	),
 	CLOSING: (
 		(Dropped, Cleared), ()
 	),
 }
 
-ar.bind(PublishAListing, PUBLISH_A_LISTING_DISPATCH)
+ar.bind(PublishAListing, PUBLISH_A_LISTING_DISPATCH, thread='networking-session')
 
 #
 #
 class SubscribeToSearch(ar.Point, ar.StateMachine):
 	"""Maintain connections with multiple published names.
 
 	:param listing: the names to search for (regular expression)
@@ -849,8 +849,8 @@
 		(Available, ar.Unknown, Dropped, Cleared, ar.Stop), ()
 	),
 	CLOSING: (
 		(Dropped, Cleared), ()
 	),
 }
 
-ar.bind(SubscribeToSearch, SUBSCRIBE_TO_SEARCH_DISPATCH)
+ar.bind(SubscribeToSearch, SUBSCRIBE_TO_SEARCH_DISPATCH, thread='networking-session')
```

### Comparing `ansar_connect-0.1.266/src/ansar/connect/networking_if.py` & `ansar_connect-0.1.267/src/ansar/connect/networking_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.266/src/ansar/connect/node.py` & `ansar_connect-0.1.267/src/ansar/connect/node.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.266/src/ansar/connect/plumbing.py` & `ansar_connect-0.1.267/src/ansar/connect/plumbing.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.266/src/ansar/connect/procedure.py` & `ansar_connect-0.1.267/src/ansar/connect/procedure.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.266/src/ansar/connect/product.py` & `ansar_connect-0.1.267/src/ansar/connect/product.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.266/src/ansar/connect/socketry.py` & `ansar_connect-0.1.267/src/ansar/connect/socketry.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.266/src/ansar/connect/standard.py` & `ansar_connect-0.1.267/src/ansar/connect/standard.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.266/src/ansar/connect/transporting.py` & `ansar_connect-0.1.267/src/ansar/connect/transporting.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.266/src/ansar/connect/transporting_if.py` & `ansar_connect-0.1.267/src/ansar/connect/transporting_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.266/src/ansar/connect/wan.py` & `ansar_connect-0.1.267/src/ansar/connect/wan.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.266/src/ansar_connect.egg-info/PKG-INFO` & `ansar_connect-0.1.267/src/ansar_connect.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.266
+Version: 0.1.267
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_connect-0.1.266/src/ansar_connect.egg-info/SOURCES.txt` & `ansar_connect-0.1.267/src/ansar_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

