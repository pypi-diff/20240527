# Comparing `tmp/special-octo-robot-0.0.8.tar.gz` & `tmp/special-octo-robot-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "special-octo-robot-0.0.8.tar", last modified: Mon May 27 17:41:50 2024, max compression
+gzip compressed data, was "special-octo-robot-0.0.9.tar", last modified: Mon May 27 18:18:22 2024, max compression
```

## Comparing `special-octo-robot-0.0.8.tar` & `special-octo-robot-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 nginx     (1000) nginx     (1000)        0 2024-05-27 17:41:50.470416 special-octo-robot-0.0.8/
--rw-rw-r--   0 nginx     (1000) nginx     (1000)    35149 2024-03-17 03:53:33.000000 special-octo-robot-0.0.8/LICENSE
--rw-rw-r--   0 nginx     (1000) nginx     (1000)        0 2024-03-17 03:53:33.000000 special-octo-robot-0.0.8/MANIFEST.in
--rw-r--r--   0 nginx     (1000) nginx     (1000)     4751 2024-05-27 17:41:50.470416 special-octo-robot-0.0.8/PKG-INFO
--rw-rw-r--   0 nginx     (1000) nginx     (1000)     4017 2024-05-27 17:06:34.000000 special-octo-robot-0.0.8/README.md
-drwxrwxr-x   0 nginx     (1000) nginx     (1000)        0 2024-05-27 17:41:50.470416 special-octo-robot-0.0.8/app/
--rw-rw-r--   0 nginx     (1000) nginx     (1000)        0 2024-03-17 03:53:33.000000 special-octo-robot-0.0.8/app/__init__.py
--rw-rw-r--   0 nginx     (1000) nginx     (1000)        0 2024-03-17 03:53:33.000000 special-octo-robot-0.0.8/app/__main__.py
--rw-rw-r--   0 nginx     (1000) nginx     (1000)       18 2024-04-14 12:18:34.000000 special-octo-robot-0.0.8/app/__version__.py
--rw-rw-r--   0 nginx     (1000) nginx     (1000)     8915 2024-05-27 17:37:39.000000 special-octo-robot-0.0.8/app/application.py
--rw-rw-r--   0 nginx     (1000) nginx     (1000)      980 2024-04-13 18:24:25.000000 special-octo-robot-0.0.8/app/config.py
--rw-rw-r--   0 nginx     (1000) nginx     (1000)     4823 2024-04-14 12:18:34.000000 special-octo-robot-0.0.8/app/console.py
--rw-rw-r--   0 nginx     (1000) nginx     (1000)      528 2024-04-13 14:03:14.000000 special-octo-robot-0.0.8/app/constants.py
--rw-rw-r--   0 nginx     (1000) nginx     (1000)     2212 2024-04-14 14:33:13.000000 special-octo-robot-0.0.8/app/database.py
--rw-rw-r--   0 nginx     (1000) nginx     (1000)      411 2024-04-14 14:25:05.000000 special-octo-robot-0.0.8/app/migrations.py
--rw-rw-r--   0 nginx     (1000) nginx     (1000)     9170 2024-05-27 17:39:04.000000 special-octo-robot-0.0.8/devcord.py
--rw-rw-r--   0 nginx     (1000) nginx     (1000)       38 2024-05-27 17:41:50.470416 special-octo-robot-0.0.8/setup.cfg
--rw-rw-r--   0 nginx     (1000) nginx     (1000)     1200 2024-04-13 14:19:20.000000 special-octo-robot-0.0.8/setup.py
-drwxrwxr-x   0 nginx     (1000) nginx     (1000)        0 2024-05-27 17:41:50.470416 special-octo-robot-0.0.8/special_octo_robot.egg-info/
--rw-r--r--   0 nginx     (1000) nginx     (1000)     4751 2024-05-27 17:41:50.000000 special-octo-robot-0.0.8/special_octo_robot.egg-info/PKG-INFO
--rw-rw-r--   0 nginx     (1000) nginx     (1000)      453 2024-05-27 17:41:50.000000 special-octo-robot-0.0.8/special_octo_robot.egg-info/SOURCES.txt
--rw-rw-r--   0 nginx     (1000) nginx     (1000)        1 2024-05-27 17:41:50.000000 special-octo-robot-0.0.8/special_octo_robot.egg-info/dependency_links.txt
--rw-rw-r--   0 nginx     (1000) nginx     (1000)       40 2024-05-27 17:41:50.000000 special-octo-robot-0.0.8/special_octo_robot.egg-info/entry_points.txt
--rw-rw-r--   0 nginx     (1000) nginx     (1000)       49 2024-05-27 17:41:50.000000 special-octo-robot-0.0.8/special_octo_robot.egg-info/requires.txt
--rw-rw-r--   0 nginx     (1000) nginx     (1000)       12 2024-05-27 17:41:50.000000 special-octo-robot-0.0.8/special_octo_robot.egg-info/top_level.txt
+drwxrwxr-x   0 nginx     (1000) nginx     (1000)        0 2024-05-27 18:18:22.955299 special-octo-robot-0.0.9/
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)    35149 2024-03-17 03:53:33.000000 special-octo-robot-0.0.9/LICENSE
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)        0 2024-03-17 03:53:33.000000 special-octo-robot-0.0.9/MANIFEST.in
+-rw-r--r--   0 nginx     (1000) nginx     (1000)     4751 2024-05-27 18:18:22.955299 special-octo-robot-0.0.9/PKG-INFO
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)     4017 2024-05-27 17:06:34.000000 special-octo-robot-0.0.9/README.md
+drwxrwxr-x   0 nginx     (1000) nginx     (1000)        0 2024-05-27 18:18:22.955299 special-octo-robot-0.0.9/app/
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)        0 2024-03-17 03:53:33.000000 special-octo-robot-0.0.9/app/__init__.py
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)        0 2024-03-17 03:53:33.000000 special-octo-robot-0.0.9/app/__main__.py
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)       18 2024-05-27 17:58:07.000000 special-octo-robot-0.0.9/app/__version__.py
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)     8962 2024-05-27 17:56:19.000000 special-octo-robot-0.0.9/app/application.py
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)      980 2024-04-13 18:24:25.000000 special-octo-robot-0.0.9/app/config.py
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)     4706 2024-05-27 17:57:44.000000 special-octo-robot-0.0.9/app/console.py
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)      528 2024-04-13 14:03:14.000000 special-octo-robot-0.0.9/app/constants.py
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)     2212 2024-04-14 14:33:13.000000 special-octo-robot-0.0.9/app/database.py
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)      411 2024-04-14 14:25:05.000000 special-octo-robot-0.0.9/app/migrations.py
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)     9170 2024-05-27 17:39:04.000000 special-octo-robot-0.0.9/devcord.py
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)       38 2024-05-27 18:18:22.955299 special-octo-robot-0.0.9/setup.cfg
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)     1200 2024-04-13 14:19:20.000000 special-octo-robot-0.0.9/setup.py
+drwxrwxr-x   0 nginx     (1000) nginx     (1000)        0 2024-05-27 18:18:22.955299 special-octo-robot-0.0.9/special_octo_robot.egg-info/
+-rw-r--r--   0 nginx     (1000) nginx     (1000)     4751 2024-05-27 18:18:22.000000 special-octo-robot-0.0.9/special_octo_robot.egg-info/PKG-INFO
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)      453 2024-05-27 18:18:22.000000 special-octo-robot-0.0.9/special_octo_robot.egg-info/SOURCES.txt
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)        1 2024-05-27 18:18:22.000000 special-octo-robot-0.0.9/special_octo_robot.egg-info/dependency_links.txt
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)       40 2024-05-27 18:18:22.000000 special-octo-robot-0.0.9/special_octo_robot.egg-info/entry_points.txt
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)       49 2024-05-27 18:18:22.000000 special-octo-robot-0.0.9/special_octo_robot.egg-info/requires.txt
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)       12 2024-05-27 18:18:22.000000 special-octo-robot-0.0.9/special_octo_robot.egg-info/top_level.txt
```

### Comparing `special-octo-robot-0.0.8/LICENSE` & `special-octo-robot-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `special-octo-robot-0.0.8/PKG-INFO` & `special-octo-robot-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: special-octo-robot
-Version: 0.0.8
+Version: 0.0.9
 Summary: Creating my own version of what a CLI Task manager and To-do-list would look like
 Home-page: https://github.com/geekNero/special-octo-robot.git
 Author: Jahan Chaware
 Author-email: sg550js@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
 Platform: Windows
 Platform: MacOS X
```

### Comparing `special-octo-robot-0.0.8/README.md` & `special-octo-robot-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `special-octo-robot-0.0.8/app/application.py` & `special-octo-robot-0.0.9/app/application.py`

 * *Files 1% similar despite different names*

```diff
@@ -242,15 +242,15 @@
 
     if updated_data["deadline"] == "week":
         today = datetime.date.today()
         weekend = today + datetime.timedelta(days=6 - today.weekday())
         updated_data["deadline"] = str(weekend)
     elif updated_data["deadline"] == "today":
         updated_data["deadline"] = str(datetime.datetime.now().strftime("%Y-%m-%d"))
-    else:
+    elif updated_data["deadline"] not in [None, "None"]:
         updated_data["deadline"] = str(convert_to_db_date(updated_data["deadline"]))
 
     if updated_data["status"] == "Completed":
         updated_data["completed"] = str(datetime.datetime.now().strftime("%Y-%m-%d"))
     else:
         updated_data["completed"] = updated_data["deadline"]
```

### Comparing `special-octo-robot-0.0.8/app/config.py` & `special-octo-robot-0.0.9/app/config.py`

 * *Files identical despite different names*

### Comparing `special-octo-robot-0.0.8/app/console.py` & `special-octo-robot-0.0.9/app/console.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,14 @@
 def get_table(tasks, plain=False):
     table = Table(title="Tasks", highlight=True, leading=True)
     table.add_column("Priority", justify="center", style="white")
     table.add_column("Task", justify="left", style="white")
     table.add_column("Status", justify="center", style="white")
     table.add_column("Deadline", justify="center", style="white")
     table.add_column("Label", justify="center", style="white")
-    table.add_column("ID", justify="center", style="white", no_wrap=True)
     table.add_column("Properties", justify="center", style="white")
     text_style = Style(color="#FFFFFF")
     bold_text_style = Style(color="#FFFFFF", bold=True)
     none_style = Style(color="magenta")
     for task in tasks:
         properties = []
         if task["description"] and task["description"] not in [
@@ -66,15 +65,14 @@
                 if not plain
                 else f"[{text_style}]{task['priority']}"
             ),
             f'[{text_style}]{task["title"]}',
             f'[{get_status_color(task["status"])}][italic]{task["status"]}',
             task["deadline"],
             f'[{bold_text_style if task["label"] != "None" else none_style}]{task["label"]}',
-            f"[{text_style}]{task['id']}",
             f"[{text_style}]{','.join(properties)}",
         )
     return table
 
 
 def sanitize_path(path):
     if path[-1] == "/":
```

### Comparing `special-octo-robot-0.0.8/app/constants.py` & `special-octo-robot-0.0.9/app/constants.py`

 * *Files identical despite different names*

### Comparing `special-octo-robot-0.0.8/app/database.py` & `special-octo-robot-0.0.9/app/database.py`

 * *Files identical despite different names*

### Comparing `special-octo-robot-0.0.8/devcord.py` & `special-octo-robot-0.0.9/devcord.py`

 * *Files identical despite different names*

### Comparing `special-octo-robot-0.0.8/setup.py` & `special-octo-robot-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `special-octo-robot-0.0.8/special_octo_robot.egg-info/PKG-INFO` & `special-octo-robot-0.0.9/special_octo_robot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: special-octo-robot
-Version: 0.0.8
+Version: 0.0.9
 Summary: Creating my own version of what a CLI Task manager and To-do-list would look like
 Home-page: https://github.com/geekNero/special-octo-robot.git
 Author: Jahan Chaware
 Author-email: sg550js@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
 Platform: Windows
 Platform: MacOS X
```

