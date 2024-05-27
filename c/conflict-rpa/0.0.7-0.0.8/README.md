# Comparing `tmp/conflict_rpa-0.0.7.tar.gz` & `tmp/conflict_rpa-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conflict_rpa-0.0.7.tar", last modified: Mon May 27 04:03:03 2024, max compression
+gzip compressed data, was "conflict_rpa-0.0.8.tar", last modified: Mon May 27 04:27:11 2024, max compression
```

## Comparing `conflict_rpa-0.0.7.tar` & `conflict_rpa-0.0.8.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 04:03:03.388539 conflict_rpa-0.0.7/
--rw-rw-rw-   0        0        0       51 2024-05-26 09:50:21.000000 conflict_rpa-0.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0     6967 2024-05-27 04:03:03.386543 conflict_rpa-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     6701 2024-05-27 04:01:46.000000 conflict_rpa-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-27 04:03:03.354620 conflict_rpa-0.0.7/conflict_rpa/
--rw-rw-rw-   0        0        0        0 2024-05-24 13:02:31.000000 conflict_rpa-0.0.7/conflict_rpa/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-27 04:03:03.381538 conflict_rpa-0.0.7/conflict_rpa/__pycache__/
--rw-rw-rw-   0        0        0      139 2024-05-26 08:54:35.000000 conflict_rpa-0.0.7/conflict_rpa/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     2874 2024-05-26 08:54:35.000000 conflict_rpa-0.0.7/conflict_rpa/__pycache__/content_rpa.cpython-310.pyc
--rw-rw-rw-   0        0        0     8202 2024-05-26 08:54:35.000000 conflict_rpa-0.0.7/conflict_rpa/__pycache__/correcting_framework.cpython-310.pyc
--rw-rw-rw-   0        0        0     2083 2024-05-26 08:54:35.000000 conflict_rpa-0.0.7/conflict_rpa/__pycache__/file_operation.cpython-310.pyc
--rw-rw-rw-   0        0        0     2683 2024-05-26 08:54:35.000000 conflict_rpa-0.0.7/conflict_rpa/__pycache__/get_running_env.cpython-310.pyc
--rw-rw-rw-   0        0        0     1286 2024-05-26 08:54:35.000000 conflict_rpa-0.0.7/conflict_rpa/__pycache__/rpa.cpython-310.pyc
--rw-rw-rw-   0        0        0     3242 2024-05-26 08:54:35.000000 conflict_rpa-0.0.7/conflict_rpa/__pycache__/utils.cpython-310.pyc
--rw-rw-rw-   0        0        0     1852 2024-05-26 11:07:22.000000 conflict_rpa-0.0.7/conflict_rpa/config.py
--rw-rw-rw-   0        0        0     3446 2024-05-27 01:00:53.000000 conflict_rpa-0.0.7/conflict_rpa/content_rpa.py
--rw-rw-rw-   0        0        0    10608 2024-05-27 03:54:41.000000 conflict_rpa-0.0.7/conflict_rpa/correcting_framework.py
--rw-rw-rw-   0        0        0     3596 2024-05-27 02:59:24.000000 conflict_rpa-0.0.7/conflict_rpa/environment_setting.py
--rw-rw-rw-   0        0        0     2436 2024-05-25 10:32:15.000000 conflict_rpa-0.0.7/conflict_rpa/file_operation.py
--rw-rw-rw-   0        0        0     2926 2024-05-25 10:32:16.000000 conflict_rpa-0.0.7/conflict_rpa/get_running_env.py
--rw-rw-rw-   0        0        0     3736 2024-05-27 01:00:54.000000 conflict_rpa-0.0.7/conflict_rpa/link_rpa.py
--rw-rw-rw-   0        0        0     2539 2024-05-27 03:31:27.000000 conflict_rpa-0.0.7/conflict_rpa/rpa.py
--rw-rw-rw-   0        0        0     3309 2024-05-26 23:39:44.000000 conflict_rpa-0.0.7/conflict_rpa/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-27 04:03:03.384543 conflict_rpa-0.0.7/conflict_rpa.egg-info/
--rw-rw-rw-   0        0        0     6967 2024-05-27 04:03:03.000000 conflict_rpa-0.0.7/conflict_rpa.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      912 2024-05-27 04:03:03.000000 conflict_rpa-0.0.7/conflict_rpa.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 04:03:03.000000 conflict_rpa-0.0.7/conflict_rpa.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-05-27 04:03:03.000000 conflict_rpa-0.0.7/conflict_rpa.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       32 2024-05-27 04:03:03.000000 conflict_rpa-0.0.7/conflict_rpa.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-27 04:03:03.000000 conflict_rpa-0.0.7/conflict_rpa.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       95 2024-05-25 13:49:40.000000 conflict_rpa-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-27 04:03:03.388539 conflict_rpa-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      565 2024-05-27 04:02:24.000000 conflict_rpa-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 04:27:11.169345 conflict_rpa-0.0.8/
+-rw-rw-rw-   0        0        0       51 2024-05-26 09:50:21.000000 conflict_rpa-0.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     6967 2024-05-27 04:27:11.168344 conflict_rpa-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     6701 2024-05-27 04:01:46.000000 conflict_rpa-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 04:27:11.146345 conflict_rpa-0.0.8/conflict_rpa/
+-rw-rw-rw-   0        0        0        0 2024-05-24 13:02:31.000000 conflict_rpa-0.0.8/conflict_rpa/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 04:27:11.165346 conflict_rpa-0.0.8/conflict_rpa/__pycache__/
+-rw-rw-rw-   0        0        0      139 2024-05-26 08:54:35.000000 conflict_rpa-0.0.8/conflict_rpa/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2874 2024-05-26 08:54:35.000000 conflict_rpa-0.0.8/conflict_rpa/__pycache__/content_rpa.cpython-310.pyc
+-rw-rw-rw-   0        0        0     8202 2024-05-26 08:54:35.000000 conflict_rpa-0.0.8/conflict_rpa/__pycache__/correcting_framework.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2083 2024-05-26 08:54:35.000000 conflict_rpa-0.0.8/conflict_rpa/__pycache__/file_operation.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2683 2024-05-26 08:54:35.000000 conflict_rpa-0.0.8/conflict_rpa/__pycache__/get_running_env.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1286 2024-05-26 08:54:35.000000 conflict_rpa-0.0.8/conflict_rpa/__pycache__/rpa.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3242 2024-05-26 08:54:35.000000 conflict_rpa-0.0.8/conflict_rpa/__pycache__/utils.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1852 2024-05-26 11:07:22.000000 conflict_rpa-0.0.8/conflict_rpa/config.py
+-rw-rw-rw-   0        0        0     3446 2024-05-27 01:00:53.000000 conflict_rpa-0.0.8/conflict_rpa/content_rpa.py
+-rw-rw-rw-   0        0        0    10864 2024-05-27 04:24:04.000000 conflict_rpa-0.0.8/conflict_rpa/correcting_framework.py
+-rw-rw-rw-   0        0        0     3596 2024-05-27 02:59:24.000000 conflict_rpa-0.0.8/conflict_rpa/environment_setting.py
+-rw-rw-rw-   0        0        0     2436 2024-05-25 10:32:15.000000 conflict_rpa-0.0.8/conflict_rpa/file_operation.py
+-rw-rw-rw-   0        0        0     2926 2024-05-25 10:32:16.000000 conflict_rpa-0.0.8/conflict_rpa/get_running_env.py
+-rw-rw-rw-   0        0        0     3736 2024-05-27 01:00:54.000000 conflict_rpa-0.0.8/conflict_rpa/link_rpa.py
+-rw-rw-rw-   0        0        0     2537 2024-05-27 04:24:13.000000 conflict_rpa-0.0.8/conflict_rpa/rpa.py
+-rw-rw-rw-   0        0        0     3309 2024-05-26 23:39:44.000000 conflict_rpa-0.0.8/conflict_rpa/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-27 04:27:11.167345 conflict_rpa-0.0.8/conflict_rpa.egg-info/
+-rw-rw-rw-   0        0        0     6967 2024-05-27 04:27:10.000000 conflict_rpa-0.0.8/conflict_rpa.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      912 2024-05-27 04:27:11.000000 conflict_rpa-0.0.8/conflict_rpa.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 04:27:10.000000 conflict_rpa-0.0.8/conflict_rpa.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-05-27 04:27:10.000000 conflict_rpa-0.0.8/conflict_rpa.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       32 2024-05-27 04:27:10.000000 conflict_rpa-0.0.8/conflict_rpa.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-27 04:27:10.000000 conflict_rpa-0.0.8/conflict_rpa.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       95 2024-05-25 13:49:40.000000 conflict_rpa-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-27 04:27:11.169345 conflict_rpa-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      565 2024-05-27 04:27:05.000000 conflict_rpa-0.0.8/setup.py
```

### Comparing `conflict_rpa-0.0.7/PKG-INFO` & `conflict_rpa-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conflict_rpa
-Version: 0.0.7
+Version: 0.0.8
 Summary: A tool to rpa in your shell
 Author: FanYangli
 Author-email: yong.feng@centurygame.com
 Description-Content-Type: text/markdown
 Requires-Dist: openai>=1.28.1
 Requires-Dist: requests>=2.22.0
```

### Comparing `conflict_rpa-0.0.7/README.md` & `conflict_rpa-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `conflict_rpa-0.0.7/conflict_rpa/__pycache__/content_rpa.cpython-310.pyc` & `conflict_rpa-0.0.8/conflict_rpa/__pycache__/content_rpa.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `conflict_rpa-0.0.7/conflict_rpa/__pycache__/correcting_framework.cpython-310.pyc` & `conflict_rpa-0.0.8/conflict_rpa/__pycache__/correcting_framework.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `conflict_rpa-0.0.7/conflict_rpa/__pycache__/file_operation.cpython-310.pyc` & `conflict_rpa-0.0.8/conflict_rpa/__pycache__/file_operation.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `conflict_rpa-0.0.7/conflict_rpa/__pycache__/get_running_env.cpython-310.pyc` & `conflict_rpa-0.0.8/conflict_rpa/__pycache__/get_running_env.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `conflict_rpa-0.0.7/conflict_rpa/__pycache__/rpa.cpython-310.pyc` & `conflict_rpa-0.0.8/conflict_rpa/__pycache__/rpa.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `conflict_rpa-0.0.7/conflict_rpa/__pycache__/utils.cpython-310.pyc` & `conflict_rpa-0.0.8/conflict_rpa/__pycache__/utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `conflict_rpa-0.0.7/conflict_rpa/config.py` & `conflict_rpa-0.0.8/conflict_rpa/config.py`

 * *Files identical despite different names*

### Comparing `conflict_rpa-0.0.7/conflict_rpa/content_rpa.py` & `conflict_rpa-0.0.8/conflict_rpa/content_rpa.py`

 * *Files identical despite different names*

### Comparing `conflict_rpa-0.0.7/conflict_rpa/correcting_framework.py` & `conflict_rpa-0.0.8/conflict_rpa/correcting_framework.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,18 +37,24 @@
 def DEBUG(*args, **kwargs):
     if debug:
         print(*args)
 
 
 def operate_script(script):
     env = dict(os.environ)
-    env["LANG"] = "zh_CN.UTF-8"
     # 使用 subprocess.Popen 执行 Bash 命令并捕获输出
-    process = subprocess.Popen(script, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True, env=env,
-                               encoding='utf-8')
+    try:
+        process = subprocess.Popen(script, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True,
+                                   env=env,
+                                   encoding='utf-8')
+
+    except UnicodeDecodeError as e:
+        print('尝试使用unicode编码')
+    process = subprocess.Popen(script, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True,
+                               env=env)
     outputs = ''
     # 实时地将输出同步到标准输出中
     while True:
         output = process.stdout.readline()
         if output == '' and process.poll() is not None:
             break
         if output:
```

### Comparing `conflict_rpa-0.0.7/conflict_rpa/environment_setting.py` & `conflict_rpa-0.0.8/conflict_rpa/environment_setting.py`

 * *Files identical despite different names*

### Comparing `conflict_rpa-0.0.7/conflict_rpa/file_operation.py` & `conflict_rpa-0.0.8/conflict_rpa/file_operation.py`

 * *Files identical despite different names*

### Comparing `conflict_rpa-0.0.7/conflict_rpa/get_running_env.py` & `conflict_rpa-0.0.8/conflict_rpa/get_running_env.py`

 * *Files identical despite different names*

### Comparing `conflict_rpa-0.0.7/conflict_rpa/link_rpa.py` & `conflict_rpa-0.0.8/conflict_rpa/link_rpa.py`

 * *Files identical despite different names*

### Comparing `conflict_rpa-0.0.7/conflict_rpa/rpa.py` & `conflict_rpa-0.0.8/conflict_rpa/rpa.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,19 +13,18 @@
         print('需要初始化OPENAI配置')
         init_config()
         print('配置完成，`source ~/.bashrc`或重启后可执行`crpa`操作')
         return
     parser = argparse.ArgumentParser()
     parser.add_argument('-l', '--link', type=str, help="提供链接进行自动化操作", default=None)
     parser.add_argument('-t', '--tutorial', type=str, help="希望自动化操作的流程文本，不需要整理地很好", default=None)
+    parser.add_argument('-i', '--instruct', type=str, help="想要RPA的指令或者自然语言", default=None)
     parser.add_argument('command',
                         nargs='*',
                         help='上一条执行的指令，用户莫动')
-    parser.add_argument('-i', '--instruct', type=str, help="想要RPA的指令或者自然语言", default=None)
-
     args = parser.parse_args()
     openai_config = read_all_config()
     if openai_config is None:
         print('需要初始化OPENAI配置')
         init_config()
         return
     else:
```

### Comparing `conflict_rpa-0.0.7/conflict_rpa/utils.py` & `conflict_rpa-0.0.8/conflict_rpa/utils.py`

 * *Files identical despite different names*

### Comparing `conflict_rpa-0.0.7/conflict_rpa.egg-info/PKG-INFO` & `conflict_rpa-0.0.8/conflict_rpa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conflict_rpa
-Version: 0.0.7
+Version: 0.0.8
 Summary: A tool to rpa in your shell
 Author: FanYangli
 Author-email: yong.feng@centurygame.com
 Description-Content-Type: text/markdown
 Requires-Dist: openai>=1.28.1
 Requires-Dist: requests>=2.22.0
```

### Comparing `conflict_rpa-0.0.7/conflict_rpa.egg-info/SOURCES.txt` & `conflict_rpa-0.0.8/conflict_rpa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `conflict_rpa-0.0.7/setup.py` & `conflict_rpa-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='conflict_rpa',
-    version='0.0.7',
+    version='0.0.8',
     packages=find_packages(),
     install_requires=[
         'openai>=1.28.1',
         'requests>=2.22.0',
     ],
     author='FanYangli',
     author_email='yong.feng@centurygame.com',
```

