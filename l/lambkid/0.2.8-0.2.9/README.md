# Comparing `tmp/lambkid-0.2.8.tar.gz` & `tmp/lambkid-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lambkid-0.2.8.tar", last modified: Fri May 24 01:11:46 2024, max compression
+gzip compressed data, was "lambkid-0.2.9.tar", last modified: Mon May 27 01:14:42 2024, max compression
```

## Comparing `lambkid-0.2.8.tar` & `lambkid-0.2.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 01:11:46.533216 lambkid-0.2.8/
--rw-rw-rw-   0        0        0     1089 2024-03-27 01:13:02.000000 lambkid-0.2.8/LICENSE
--rw-rw-rw-   0        0        0       27 2024-04-01 08:22:25.000000 lambkid-0.2.8/MANIFEST.in
--rw-rw-rw-   0        0        0     2094 2024-05-24 01:11:46.532219 lambkid-0.2.8/PKG-INFO
--rw-rw-rw-   0        0        0      717 2024-04-24 02:44:24.000000 lambkid-0.2.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-24 01:11:46.482371 lambkid-0.2.8/docs/
--rw-rw-rw-   0        0        0      371 2024-04-08 03:30:43.000000 lambkid-0.2.8/docs/cli.md
--rw-rw-rw-   0        0        0      221 2024-04-24 02:42:57.000000 lambkid-0.2.8/docs/csv.md
--rw-rw-rw-   0        0        0       54 2024-03-31 06:58:42.000000 lambkid-0.2.8/docs/install.md
--rw-rw-rw-   0        0        0      778 2024-04-07 15:20:10.000000 lambkid-0.2.8/docs/log.md
--rw-rw-rw-   0        0        0     1878 2024-04-01 07:39:19.000000 lambkid-0.2.8/docs/sshclient.md
--rw-rw-rw-   0        0        0       36 2024-04-25 02:05:46.000000 lambkid-0.2.8/docs/utils.md
-drwxrwxrwx   0        0        0        0 2024-05-24 01:11:46.484361 lambkid-0.2.8/lambkid/
--rw-rw-rw-   0        0        0      188 2024-05-22 02:46:42.000000 lambkid-0.2.8/lambkid/__init__.py
--rw-rw-rw-   0        0        0      969 2024-04-08 15:55:58.000000 lambkid-0.2.8/lambkid/cli.py
-drwxrwxrwx   0        0        0        0 2024-05-24 01:11:46.527222 lambkid-0.2.8/lambkid/libs/
--rw-rw-rw-   0        0        0        0 2024-03-31 06:59:08.000000 lambkid-0.2.8/lambkid/libs/__init__.py
--rw-rw-rw-   0        0        0     1514 2024-05-22 02:46:35.000000 lambkid-0.2.8/lambkid/libs/log.py
--rw-rw-rw-   0        0        0     1825 2024-05-17 02:16:37.000000 lambkid-0.2.8/lambkid/libs/minio_client.py
--rw-rw-rw-   0        0        0    10029 2024-05-24 01:08:09.000000 lambkid-0.2.8/lambkid/libs/ssh.py
--rw-rw-rw-   0        0        0     2259 2024-04-28 05:47:19.000000 lambkid-0.2.8/lambkid/libs/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-24 01:11:46.531220 lambkid-0.2.8/lambkid.egg-info/
--rw-rw-rw-   0        0        0     2094 2024-05-24 01:11:46.000000 lambkid-0.2.8/lambkid.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      461 2024-05-24 01:11:46.000000 lambkid-0.2.8/lambkid.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 01:11:46.000000 lambkid-0.2.8/lambkid.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-05-24 01:11:46.000000 lambkid-0.2.8/lambkid.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       43 2024-05-24 01:11:46.000000 lambkid-0.2.8/lambkid.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-24 01:11:46.000000 lambkid-0.2.8/lambkid.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-24 01:11:46.533216 lambkid-0.2.8/setup.cfg
--rw-rw-rw-   0        0        0     1834 2024-05-24 01:08:33.000000 lambkid-0.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 01:14:42.045067 lambkid-0.2.9/
+-rw-rw-rw-   0        0        0     1089 2024-03-27 01:13:02.000000 lambkid-0.2.9/LICENSE
+-rw-rw-rw-   0        0        0       27 2024-04-01 08:22:25.000000 lambkid-0.2.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     2094 2024-05-27 01:14:42.043073 lambkid-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0      717 2024-04-24 02:44:24.000000 lambkid-0.2.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 01:14:41.997202 lambkid-0.2.9/docs/
+-rw-rw-rw-   0        0        0      371 2024-04-08 03:30:43.000000 lambkid-0.2.9/docs/cli.md
+-rw-rw-rw-   0        0        0      221 2024-04-24 02:42:57.000000 lambkid-0.2.9/docs/csv.md
+-rw-rw-rw-   0        0        0       54 2024-03-31 06:58:42.000000 lambkid-0.2.9/docs/install.md
+-rw-rw-rw-   0        0        0      778 2024-04-07 15:20:10.000000 lambkid-0.2.9/docs/log.md
+-rw-rw-rw-   0        0        0     1878 2024-04-01 07:39:19.000000 lambkid-0.2.9/docs/sshclient.md
+-rw-rw-rw-   0        0        0       36 2024-04-25 02:05:46.000000 lambkid-0.2.9/docs/utils.md
+drwxrwxrwx   0        0        0        0 2024-05-27 01:14:42.000187 lambkid-0.2.9/lambkid/
+-rw-rw-rw-   0        0        0      188 2024-05-22 02:46:42.000000 lambkid-0.2.9/lambkid/__init__.py
+-rw-rw-rw-   0        0        0      969 2024-04-08 15:55:58.000000 lambkid-0.2.9/lambkid/cli.py
+drwxrwxrwx   0        0        0        0 2024-05-27 01:14:42.038085 lambkid-0.2.9/lambkid/libs/
+-rw-rw-rw-   0        0        0        0 2024-03-31 06:59:08.000000 lambkid-0.2.9/lambkid/libs/__init__.py
+-rw-rw-rw-   0        0        0     1514 2024-05-22 02:46:35.000000 lambkid-0.2.9/lambkid/libs/log.py
+-rw-rw-rw-   0        0        0     1825 2024-05-17 02:16:37.000000 lambkid-0.2.9/lambkid/libs/minio_client.py
+-rw-rw-rw-   0        0        0    10608 2024-05-27 01:13:21.000000 lambkid-0.2.9/lambkid/libs/ssh.py
+-rw-rw-rw-   0        0        0     2259 2024-04-28 05:47:19.000000 lambkid-0.2.9/lambkid/libs/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-27 01:14:42.043073 lambkid-0.2.9/lambkid.egg-info/
+-rw-rw-rw-   0        0        0     2094 2024-05-27 01:14:41.000000 lambkid-0.2.9/lambkid.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      461 2024-05-27 01:14:41.000000 lambkid-0.2.9/lambkid.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 01:14:41.000000 lambkid-0.2.9/lambkid.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-05-27 01:14:41.000000 lambkid-0.2.9/lambkid.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       43 2024-05-27 01:14:41.000000 lambkid-0.2.9/lambkid.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-27 01:14:41.000000 lambkid-0.2.9/lambkid.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 01:14:42.045067 lambkid-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0     1834 2024-05-27 01:13:31.000000 lambkid-0.2.9/setup.py
```

### Comparing `lambkid-0.2.8/LICENSE` & `lambkid-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lambkid-0.2.8/PKG-INFO` & `lambkid-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lambkid
-Version: 0.2.8
+Version: 0.2.9
 Summary: lambkid is an advance abstract from some common pyton lib, it aim to make you write python more easily and more fewer code.
 Home-page: https://github.com/redrose2100/lambkid
 Author: redrose2100
 Author-email: hitredrose@163.com
 Maintainer: redrose2100
 Maintainer-email: hitredrose@163.com
 License: MIT
```

### Comparing `lambkid-0.2.8/README.md` & `lambkid-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `lambkid-0.2.8/docs/log.md` & `lambkid-0.2.9/docs/log.md`

 * *Files identical despite different names*

### Comparing `lambkid-0.2.8/docs/sshclient.md` & `lambkid-0.2.9/docs/sshclient.md`

 * *Files identical despite different names*

### Comparing `lambkid-0.2.8/lambkid/cli.py` & `lambkid-0.2.9/lambkid/cli.py`

 * *Files identical despite different names*

### Comparing `lambkid-0.2.8/lambkid/libs/log.py` & `lambkid-0.2.9/lambkid/libs/log.py`

 * *Files identical despite different names*

### Comparing `lambkid-0.2.8/lambkid/libs/minio_client.py` & `lambkid-0.2.9/lambkid/libs/minio_client.py`

 * *Files identical despite different names*

### Comparing `lambkid-0.2.8/lambkid/libs/ssh.py` & `lambkid-0.2.9/lambkid/libs/ssh.py`

 * *Files 4% similar despite different names*

```diff
@@ -203,18 +203,47 @@
             self.__transport.set_keepalive(self.__keep_alive_interval)
             log.info(f" {self.__ip}:{self.__port} | successful to create ssh connect: OK.")
             return True
         except Exception as e:
             log.warning(f" {self.__ip}:{self.__port} | fail create ssh connect: Error.err msg is {str(e)}")
             return False
 
+    def __del__(self):
+        try:
+            self.__sftp.close()
+        except:
+            pass
+        try:
+            self.__scp.close()
+        except:
+            pass
+        try:
+            self.__transport.close()
+        except:
+            pass
+        try:
+            self.__ssh.close()
+        except:
+            pass
+
     def __reconnect(self):
         try:
-            if self.__ssh:
-                del self.__ssh
+            self.__sftp.close()
+        except:
+            pass
+        try:
+            self.__scp.close()
+        except:
+            pass
+        try:
+            self.__transport.close()
+        except:
+            pass
+        try:
+            self.__ssh.close()
         except:
             pass
         return self.__connect()
 
     def __is_active(self):
         try:
             if not self.__transport:
```

### Comparing `lambkid-0.2.8/lambkid/libs/utils.py` & `lambkid-0.2.9/lambkid/libs/utils.py`

 * *Files identical despite different names*

### Comparing `lambkid-0.2.8/lambkid.egg-info/PKG-INFO` & `lambkid-0.2.9/lambkid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lambkid
-Version: 0.2.8
+Version: 0.2.9
 Summary: lambkid is an advance abstract from some common pyton lib, it aim to make you write python more easily and more fewer code.
 Home-page: https://github.com/redrose2100/lambkid
 Author: redrose2100
 Author-email: hitredrose@163.com
 Maintainer: redrose2100
 Maintainer-email: hitredrose@163.com
 License: MIT
```

### Comparing `lambkid-0.2.8/setup.py` & `lambkid-0.2.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
         long_desc=f.read()
 except:
     long_desc=""
 
 
 setup(
     name="lambkid",
-    version="0.2.8",
+    version="0.2.9",
     description="lambkid is an advance abstract from some common pyton lib, it aim to make you write python more easily and more fewer code.",
     long_description=long_desc,
     long_description_content_type="text/markdown",
     author="redrose2100",
     author_email="hitredrose@163.com",
     maintainer="redrose2100",
     maintainer_email="hitredrose@163.com",
```

