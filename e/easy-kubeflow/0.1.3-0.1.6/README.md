# Comparing `tmp/easy-kubeflow-0.1.3.tar.gz` & `tmp/easy-kubeflow-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/easy-kubeflow-0.1.3.tar", last modified: Wed Dec 13 11:13:49 2023, max compression
+gzip compressed data, was "dist/easy-kubeflow-0.1.6.tar", last modified: Mon May 27 12:51:23 2024, max compression
```

## Comparing `easy-kubeflow-0.1.3.tar` & `easy-kubeflow-0.1.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 lwb        (501) staff       (20)        0 2023-12-13 11:13:49.000000 easy-kubeflow-0.1.3/
--rw-r--r--   0 lwb        (501) staff       (20)      482 2023-12-13 11:13:49.000000 easy-kubeflow-0.1.3/PKG-INFO
-drwxr-xr-x   0 lwb        (501) staff       (20)        0 2023-12-13 11:13:49.000000 easy-kubeflow-0.1.3/easy_kubeflow.egg-info/
--rw-r--r--   0 lwb        (501) staff       (20)      482 2023-12-13 11:13:49.000000 easy-kubeflow-0.1.3/easy_kubeflow.egg-info/PKG-INFO
--rw-r--r--   0 lwb        (501) staff       (20)      551 2023-12-13 11:13:49.000000 easy-kubeflow-0.1.3/easy_kubeflow.egg-info/SOURCES.txt
--rw-r--r--   0 lwb        (501) staff       (20)       71 2023-12-13 11:13:49.000000 easy-kubeflow-0.1.3/easy_kubeflow.egg-info/requires.txt
--rw-r--r--   0 lwb        (501) staff       (20)       14 2023-12-13 11:13:49.000000 easy-kubeflow-0.1.3/easy_kubeflow.egg-info/top_level.txt
--rw-r--r--   0 lwb        (501) staff       (20)        1 2023-12-13 11:13:49.000000 easy-kubeflow-0.1.3/easy_kubeflow.egg-info/dependency_links.txt
-drwxr-xr-x   0 lwb        (501) staff       (20)        0 2023-12-13 11:13:49.000000 easy-kubeflow-0.1.3/easy_kubeflow/
-drwxr-xr-x   0 lwb        (501) staff       (20)        0 2023-12-13 11:13:49.000000 easy-kubeflow-0.1.3/easy_kubeflow/submitjobs/
--rw-r--r--   0 lwb        (501) staff       (20)    13121 2023-10-09 12:07:06.000000 easy-kubeflow-0.1.3/easy_kubeflow/submitjobs/jobs_util.py
--rw-r--r--   0 lwb        (501) staff       (20)       55 2023-09-05 07:42:51.000000 easy-kubeflow-0.1.3/easy_kubeflow/submitjobs/__init__.py
--rw-r--r--   0 lwb        (501) staff       (20)      191 2023-09-05 07:42:51.000000 easy-kubeflow-0.1.3/easy_kubeflow/__init__.py
-drwxr-xr-x   0 lwb        (501) staff       (20)        0 2023-12-13 11:13:49.000000 easy-kubeflow-0.1.3/easy_kubeflow/pipelines/
--rw-r--r--   0 lwb        (501) staff       (20)       69 2021-12-16 02:30:40.000000 easy-kubeflow-0.1.3/easy_kubeflow/pipelines/__init__.py
--rw-r--r--   0 lwb        (501) staff       (20)    22851 2023-09-19 11:56:34.000000 easy-kubeflow-0.1.3/easy_kubeflow/pipelines/pipelines_util.py
-drwxr-xr-x   0 lwb        (501) staff       (20)        0 2023-12-13 11:13:49.000000 easy-kubeflow-0.1.3/easy_kubeflow/utils/
--rw-r--r--   0 lwb        (501) staff       (20)     1140 2021-12-16 02:29:02.000000 easy-kubeflow-0.1.3/easy_kubeflow/utils/log_util.py
--rw-r--r--   0 lwb        (501) staff       (20)       31 2021-12-16 02:30:25.000000 easy-kubeflow-0.1.3/easy_kubeflow/utils/__init__.py
-drwxr-xr-x   0 lwb        (501) staff       (20)        0 2023-12-13 11:13:49.000000 easy-kubeflow-0.1.3/easy_kubeflow/examples/
--rw-r--r--   0 lwb        (501) staff       (20)        0 2021-12-16 08:21:23.000000 easy-kubeflow-0.1.3/easy_kubeflow/examples/__init__.py
-drwxr-xr-x   0 lwb        (501) staff       (20)        0 2023-12-13 11:13:49.000000 easy-kubeflow-0.1.3/easy_kubeflow/_docker/
--rw-r--r--   0 lwb        (501) staff       (20)       36 2021-12-16 02:30:53.000000 easy-kubeflow-0.1.3/easy_kubeflow/_docker/__init__.py
--rw-r--r--   0 lwb        (501) staff       (20)    23012 2023-12-13 11:12:55.000000 easy-kubeflow-0.1.3/easy_kubeflow/_docker/docker_util.py
--rw-r--r--   0 lwb        (501) staff       (20)     7231 2023-02-27 10:44:37.000000 easy-kubeflow-0.1.3/README.md
--rw-r--r--   0 lwb        (501) staff       (20)      856 2023-12-13 11:12:55.000000 easy-kubeflow-0.1.3/setup.py
--rw-r--r--   0 lwb        (501) staff       (20)       38 2023-12-13 11:13:49.000000 easy-kubeflow-0.1.3/setup.cfg
+drwxr-xr-x   0 lwb        (501) staff       (20)        0 2024-05-27 12:51:23.000000 easy-kubeflow-0.1.6/
+-rw-r--r--   0 lwb        (501) staff       (20)      482 2024-05-27 12:51:23.000000 easy-kubeflow-0.1.6/PKG-INFO
+drwxr-xr-x   0 lwb        (501) staff       (20)        0 2024-05-27 12:51:23.000000 easy-kubeflow-0.1.6/easy_kubeflow.egg-info/
+-rw-r--r--   0 lwb        (501) staff       (20)      482 2024-05-27 12:51:23.000000 easy-kubeflow-0.1.6/easy_kubeflow.egg-info/PKG-INFO
+-rw-r--r--   0 lwb        (501) staff       (20)      551 2024-05-27 12:51:23.000000 easy-kubeflow-0.1.6/easy_kubeflow.egg-info/SOURCES.txt
+-rw-r--r--   0 lwb        (501) staff       (20)       71 2024-05-27 12:51:23.000000 easy-kubeflow-0.1.6/easy_kubeflow.egg-info/requires.txt
+-rw-r--r--   0 lwb        (501) staff       (20)       14 2024-05-27 12:51:23.000000 easy-kubeflow-0.1.6/easy_kubeflow.egg-info/top_level.txt
+-rw-r--r--   0 lwb        (501) staff       (20)        1 2024-05-27 12:51:23.000000 easy-kubeflow-0.1.6/easy_kubeflow.egg-info/dependency_links.txt
+drwxr-xr-x   0 lwb        (501) staff       (20)        0 2024-05-27 12:51:23.000000 easy-kubeflow-0.1.6/easy_kubeflow/
+drwxr-xr-x   0 lwb        (501) staff       (20)        0 2024-05-27 12:51:23.000000 easy-kubeflow-0.1.6/easy_kubeflow/submitjobs/
+-rw-r--r--   0 lwb        (501) staff       (20)    13087 2024-05-27 12:49:35.000000 easy-kubeflow-0.1.6/easy_kubeflow/submitjobs/jobs_util.py
+-rw-r--r--   0 lwb        (501) staff       (20)       55 2023-09-05 07:42:51.000000 easy-kubeflow-0.1.6/easy_kubeflow/submitjobs/__init__.py
+-rw-r--r--   0 lwb        (501) staff       (20)      191 2023-09-05 07:42:51.000000 easy-kubeflow-0.1.6/easy_kubeflow/__init__.py
+drwxr-xr-x   0 lwb        (501) staff       (20)        0 2024-05-27 12:51:23.000000 easy-kubeflow-0.1.6/easy_kubeflow/pipelines/
+-rw-r--r--   0 lwb        (501) staff       (20)       69 2021-12-16 02:30:40.000000 easy-kubeflow-0.1.6/easy_kubeflow/pipelines/__init__.py
+-rw-r--r--   0 lwb        (501) staff       (20)    22851 2023-09-19 11:56:34.000000 easy-kubeflow-0.1.6/easy_kubeflow/pipelines/pipelines_util.py
+drwxr-xr-x   0 lwb        (501) staff       (20)        0 2024-05-27 12:51:23.000000 easy-kubeflow-0.1.6/easy_kubeflow/utils/
+-rw-r--r--   0 lwb        (501) staff       (20)     1140 2021-12-16 02:29:02.000000 easy-kubeflow-0.1.6/easy_kubeflow/utils/log_util.py
+-rw-r--r--   0 lwb        (501) staff       (20)       31 2021-12-16 02:30:25.000000 easy-kubeflow-0.1.6/easy_kubeflow/utils/__init__.py
+drwxr-xr-x   0 lwb        (501) staff       (20)        0 2024-05-27 12:51:23.000000 easy-kubeflow-0.1.6/easy_kubeflow/examples/
+-rw-r--r--   0 lwb        (501) staff       (20)        0 2021-12-16 08:21:23.000000 easy-kubeflow-0.1.6/easy_kubeflow/examples/__init__.py
+drwxr-xr-x   0 lwb        (501) staff       (20)        0 2024-05-27 12:51:23.000000 easy-kubeflow-0.1.6/easy_kubeflow/_docker/
+-rw-r--r--   0 lwb        (501) staff       (20)       36 2021-12-16 02:30:53.000000 easy-kubeflow-0.1.6/easy_kubeflow/_docker/__init__.py
+-rw-r--r--   0 lwb        (501) staff       (20)    23012 2023-12-13 11:12:55.000000 easy-kubeflow-0.1.6/easy_kubeflow/_docker/docker_util.py
+-rw-r--r--   0 lwb        (501) staff       (20)     7231 2023-02-27 10:44:37.000000 easy-kubeflow-0.1.6/README.md
+-rw-r--r--   0 lwb        (501) staff       (20)      856 2024-05-27 12:50:46.000000 easy-kubeflow-0.1.6/setup.py
+-rw-r--r--   0 lwb        (501) staff       (20)       38 2024-05-27 12:51:23.000000 easy-kubeflow-0.1.6/setup.cfg
```

### Comparing `easy-kubeflow-0.1.3/easy_kubeflow.egg-info/SOURCES.txt` & `easy-kubeflow-0.1.6/easy_kubeflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `easy-kubeflow-0.1.3/easy_kubeflow/submitjobs/jobs_util.py` & `easy-kubeflow-0.1.6/easy_kubeflow/submitjobs/jobs_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,16 +98,16 @@
 
     def __init__(self, name=None, job_type="standalone"):
         """
         job obj
         :param name: give a job name
         """
         self.cmd = []
-        self.pvc_list = []
-        self.vol_list = []
+        # self.pvc_list = []
+        # self.vol_list = []
         self.type = job_type
         self.name = name if _verify_name(name) else "job-" + str(uuid4())
         self.job_obj = {
             "jobType": self.type,
             "jobName": self.name,
             "gpus": "none",
             "affinityConfig": "none",
@@ -215,46 +215,46 @@
     def datavols(self, name: str = None, mount_path: str = None):
         """
         add pvc
         :param name: pvc name
         :param mount_path: mount path
         :return:
         """
-        self.pvc_list.append(
+        pvc_list = [
             {
                 "name": name,
                 "path": mount_path
             }
-        )
+        ]
         if self.job_obj.get("datavols"):
-            self.job_obj["datavols"].extend(self.pvc_list)
+            self.job_obj["datavols"].extend(pvc_list)
         else:
-            self.job_obj["datavols"] = self.pvc_list
+            self.job_obj["datavols"] = pvc_list
         _logger.info("set job data vol: %s" % name)
         return self
 
     def sharedvols(self, server: str = None, path: str = None, mount_path: str = None):
         """
         add shared volumes
         :param server: nfs ip
         :param path: nfs path
         :param mount_path: mount path
         :return:
         """
-        self.vol_list.append(
+        vol_list = [
             {
                 "server": server,
                 "path": path,
                 "mountPath": mount_path
             }
-        )
+        ]
         if self.job_obj.get("sharedvols"):
-            self.job_obj["sharedvols"].extend(self.vol_list)
+            self.job_obj["sharedvols"].extend(vol_list)
         else:
-            self.job_obj["sharedvols"] = self.vol_list
+            self.job_obj["sharedvols"] = vol_list
         _logger.info("set job shared vol: %s" % path)
         return self
 
     def ttl(self, timeout: int = 3):
         """
         time to terminate completed job
         :param timeout: unit(day)
```

### Comparing `easy-kubeflow-0.1.3/easy_kubeflow/pipelines/pipelines_util.py` & `easy-kubeflow-0.1.6/easy_kubeflow/pipelines/pipelines_util.py`

 * *Files identical despite different names*

### Comparing `easy-kubeflow-0.1.3/easy_kubeflow/utils/log_util.py` & `easy-kubeflow-0.1.6/easy_kubeflow/utils/log_util.py`

 * *Files identical despite different names*

### Comparing `easy-kubeflow-0.1.3/easy_kubeflow/_docker/docker_util.py` & `easy-kubeflow-0.1.6/easy_kubeflow/_docker/docker_util.py`

 * *Files identical despite different names*

### Comparing `easy-kubeflow-0.1.3/README.md` & `easy-kubeflow-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `easy-kubeflow-0.1.3/setup.py` & `easy-kubeflow-0.1.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = None
 
 setuptools.setup(
     name="easy-kubeflow",  # Replace with your own name
-    version="0.1.3",
+    version="0.1.6",
     author="CrazyBean",
     author_email="liuweibin@stonewise.cn",
     description="sdk help users for a better use of kubeflow",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.stonewise.cn/mlsys/easy-kubeflow.git",
     install_requires=[
         'docker>=4.2.1',
-        'kfp==1.3.0',
+        'kfp==1.4.0',
         'pandas>=1.1.5',
         'tqdm>=4.56.0',
         'simplejson>=3.17.5'
     ],
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
```

