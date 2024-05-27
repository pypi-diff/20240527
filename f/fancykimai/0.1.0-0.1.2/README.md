# Comparing `tmp/fancykimai-0.1.0.tar.gz` & `tmp/fancykimai-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fancykimai-0.1.0.tar", max compression
+gzip compressed data, was "fancykimai-0.1.2.tar", max compression
```

## Comparing `fancykimai-0.1.0.tar` & `fancykimai-0.1.2.tar`

### file list

```diff
@@ -1,24 +1,15 @@
--rw-r--r--   0        0        0        0 2024-03-18 18:45:36.316907 fancykimai-0.1.0/README.md
--rw-r--r--   0        0        0      182 2024-03-18 16:57:18.845386 fancykimai-0.1.0/fancykimai/app.py
--rw-r--r--   0        0        0      405 2024-03-18 19:11:42.958077 fancykimai-0.1.0/fancykimai/commands/__init__.py
--rw-r--r--   0        0        0      674 2024-03-18 19:12:20.726239 fancykimai-0.1.0/fancykimai/commands/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2318 2024-03-18 19:31:30.527601 fancykimai-0.1.0/fancykimai/commands/__pycache__/activities.cpython-311.pyc
--rw-r--r--   0        0        0     2479 2024-03-18 19:13:51.099396 fancykimai-0.1.0/fancykimai/commands/__pycache__/config.cpython-311.pyc
--rw-r--r--   0        0        0     2367 2024-03-18 19:31:30.544483 fancykimai-0.1.0/fancykimai/commands/__pycache__/customers.cpython-311.pyc
--rw-r--r--   0        0        0     1590 2024-03-18 16:48:27.087518 fancykimai-0.1.0/fancykimai/commands/__pycache__/login.cpython-311.pyc
--rw-r--r--   0        0        0     3925 2024-03-18 19:48:11.974395 fancykimai-0.1.0/fancykimai/commands/__pycache__/projects.cpython-311.pyc
--rw-r--r--   0        0        0     1369 2024-03-18 17:03:14.674210 fancykimai-0.1.0/fancykimai/commands/__pycache__/teams.cpython-311.pyc
--rw-r--r--   0        0        0    12915 2024-03-18 20:29:07.630979 fancykimai-0.1.0/fancykimai/commands/__pycache__/timesheets.cpython-311.pyc
--rw-r--r--   0        0        0     1053 2024-03-18 19:31:17.357052 fancykimai-0.1.0/fancykimai/commands/activities.py
--rw-r--r--   0        0        0      902 2024-03-18 19:13:27.718457 fancykimai-0.1.0/fancykimai/commands/config.py
--rw-r--r--   0        0        0     1120 2024-03-18 19:31:28.839716 fancykimai-0.1.0/fancykimai/commands/customers.py
--rw-r--r--   0        0        0      884 2024-03-18 16:48:20.485136 fancykimai-0.1.0/fancykimai/commands/login.py
--rw-r--r--   0        0        0     2021 2024-03-18 19:48:07.930163 fancykimai-0.1.0/fancykimai/commands/projects.py
--rw-r--r--   0        0        0      497 2024-03-18 17:02:56.472877 fancykimai-0.1.0/fancykimai/commands/teams.py
--rw-r--r--   0        0        0     9543 2024-03-18 20:28:59.637927 fancykimai-0.1.0/fancykimai/commands/timesheets.py
--rw-r--r--   0        0        0     2707 2024-03-18 19:15:14.173652 fancykimai-0.1.0/fancykimai/functions/__pycache__/config.cpython-311.pyc
--rw-r--r--   0        0        0     2278 2024-03-18 19:20:13.856659 fancykimai-0.1.0/fancykimai/functions/__pycache__/kimai.cpython-311.pyc
--rw-r--r--   0        0        0      974 2024-03-18 19:15:12.398993 fancykimai-0.1.0/fancykimai/functions/config.py
--rw-r--r--   0        0        0     1687 2024-03-22 15:14:31.699936 fancykimai-0.1.0/fancykimai/functions/kimai.py
--rw-r--r--   0        0        0      432 2024-03-18 19:36:51.828706 fancykimai-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      511 1970-01-01 00:00:00.000000 fancykimai-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-03-22 15:28:44.147735 fancykimai-0.1.2/LICENSE
+-rw-r--r--   0        0        0      220 2024-03-22 16:06:24.042340 fancykimai-0.1.2/README.md
+-rw-r--r--   0        0        0      877 2024-05-27 15:26:02.991667 fancykimai-0.1.2/fancykimai/app.py
+-rw-r--r--   0        0        0      405 2024-03-18 19:11:42.958077 fancykimai-0.1.2/fancykimai/commands/__init__.py
+-rw-r--r--   0        0        0     1053 2024-03-18 19:31:17.357052 fancykimai-0.1.2/fancykimai/commands/activities.py
+-rw-r--r--   0        0        0      902 2024-03-18 19:13:27.718457 fancykimai-0.1.2/fancykimai/commands/config.py
+-rw-r--r--   0        0        0     1120 2024-03-18 19:31:28.839716 fancykimai-0.1.2/fancykimai/commands/customers.py
+-rw-r--r--   0        0        0      884 2024-03-18 16:48:20.485136 fancykimai-0.1.2/fancykimai/commands/login.py
+-rw-r--r--   0        0        0     2021 2024-05-27 15:25:46.257141 fancykimai-0.1.2/fancykimai/commands/projects.py
+-rw-r--r--   0        0        0      497 2024-03-18 17:02:56.472877 fancykimai-0.1.2/fancykimai/commands/teams.py
+-rw-r--r--   0        0        0    10000 2024-05-27 15:33:58.079750 fancykimai-0.1.2/fancykimai/commands/timesheets.py
+-rw-r--r--   0        0        0      974 2024-03-18 19:15:12.398993 fancykimai-0.1.2/fancykimai/functions/config.py
+-rw-r--r--   0        0        0     1687 2024-03-22 15:14:31.699936 fancykimai-0.1.2/fancykimai/functions/kimai.py
+-rw-r--r--   0        0        0      619 2024-05-27 16:06:44.374165 fancykimai-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      989 1970-01-01 00:00:00.000000 fancykimai-0.1.2/PKG-INFO
```

### Comparing `fancykimai-0.1.0/fancykimai/commands/activities.py` & `fancykimai-0.1.2/fancykimai/commands/activities.py`

 * *Files identical despite different names*

### Comparing `fancykimai-0.1.0/fancykimai/commands/config.py` & `fancykimai-0.1.2/fancykimai/commands/config.py`

 * *Files identical despite different names*

### Comparing `fancykimai-0.1.0/fancykimai/commands/customers.py` & `fancykimai-0.1.2/fancykimai/commands/customers.py`

 * *Files identical despite different names*

### Comparing `fancykimai-0.1.0/fancykimai/commands/login.py` & `fancykimai-0.1.2/fancykimai/commands/login.py`

 * *Files identical despite different names*

### Comparing `fancykimai-0.1.0/fancykimai/commands/projects.py` & `fancykimai-0.1.2/fancykimai/commands/projects.py`

 * *Files identical despite different names*

### Comparing `fancykimai-0.1.0/fancykimai/commands/timesheets.py` & `fancykimai-0.1.2/fancykimai/commands/timesheets.py`

 * *Files 6% similar despite different names*

```diff
@@ -245,28 +245,35 @@
     required=True,
     help="Activity ID",
     default=get_config("activity"),
 )
 @click.option("-d", "--description", type=str, required=True, help="Description")
 @click.option("-b", "--begin", type=str, required=True, help="Begin date", default=datetime.datetime.now().strftime("%Y-%m-%d"))
 @click.option("-e", "--end", type=str, required=False, help="End date")
-def set_timesheet(project: int, activity: int, description: str, begin: str, end: str):
+@click.option("-h", "--hours", type=float, required=False, help="Hours to be set. When set, ignores the end date and if no begin time is set, sets it to 09:00")
+def set_timesheet(project: int, activity: int, description: str, begin: str, end: str, hours: float):
     # Check if the hours are set on the dates
     begin_datetime = datetime.datetime.strptime(begin, "%Y-%m-%d")
     if end:
         end_datetime = datetime.datetime.strptime(end, "%Y-%m-%d")
     else:
         end_datetime = begin_datetime
         end = begin
     if begin_datetime > end_datetime:
         click.echo("Begin date cannot be after end date.")
         raise click.Abort("Begin date cannot be after end date.")
-    # ask for the time to be set
-    begin_time = click.prompt("Begin time", type=str, default="00:00")
-    end_time = click.prompt("End time", type=str, default="23:59")
+    if not hours:
+        # ask for the time to be set
+        begin_time = click.prompt("Begin time", type=str, default="00:00")
+        end_time = click.prompt("End time", type=str, default="23:59")
+    else:
+        begin_time = "09:00"
+        # add `hours` to 9 AM to get the end time
+        am9 = datetime.datetime.strptime(begin, "%Y-%m-%d").replace(hour=9, minute=0)
+        end_time = (am9 + datetime.timedelta(hours=hours)).strftime("%H:%M")
     begin = f"{begin}T{begin_time}:00"
     end = f"{end}T{end_time}:00"
     # Check if the begin and end dates are valid
     begin_datetime = datetime.datetime.strptime(begin, "%Y-%m-%dT%H:%M:%S")
     end_datetime = datetime.datetime.strptime(end, "%Y-%m-%dT%H:%M:%S")
     if begin_datetime > end_datetime:
         click.echo("Begin date cannot be after end date.")
```

### Comparing `fancykimai-0.1.0/fancykimai/functions/config.py` & `fancykimai-0.1.2/fancykimai/functions/config.py`

 * *Files identical despite different names*

### Comparing `fancykimai-0.1.0/fancykimai/functions/kimai.py` & `fancykimai-0.1.2/fancykimai/functions/kimai.py`

 * *Files identical despite different names*

