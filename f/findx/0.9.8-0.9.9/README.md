# Comparing `tmp/findx-0.9.8.tar.gz` & `tmp/findx-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findx-0.9.8.tar", last modified: Tue Jun 21 12:43:06 2016, max compression, from Unix
+gzip compressed data, was "dist/findx-0.9.9.tar", last modified: Sat Jun 25 18:09:25 2016, max compression
```

## Comparing `findx-0.9.8.tar` & `findx-0.9.9.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxr-x   0 mike      (2001) mike      (2001)        0 2016-06-21 12:43:06.000000 findx-0.9.8/
--rw-rw-r--   0 mike      (2001) mike      (2001)       60 2016-05-26 10:34:12.000000 findx-0.9.8/MANIFEST.in
-drwxrwxr-x   0 mike      (2001) mike      (2001)        0 2016-06-21 12:43:06.000000 findx-0.9.8/findx.egg-info/
--rw-rw-r--   0 mike      (2001) mike      (2001)      284 2016-06-21 12:43:06.000000 findx-0.9.8/findx.egg-info/SOURCES.txt
--rw-rw-r--   0 mike      (2001) mike      (2001)       70 2016-06-21 12:43:06.000000 findx-0.9.8/findx.egg-info/entry_points.txt
--rw-rw-r--   0 mike      (2001) mike      (2001)       11 2016-06-21 12:43:06.000000 findx-0.9.8/findx.egg-info/top_level.txt
--rw-rw-r--   0 mike      (2001) mike      (2001)        1 2016-05-18 23:38:30.000000 findx-0.9.8/findx.egg-info/zip-safe
--rw-rw-r--   0 mike      (2001) mike      (2001)     4686 2016-06-21 12:43:06.000000 findx-0.9.8/findx.egg-info/PKG-INFO
--rw-rw-r--   0 mike      (2001) mike      (2001)        1 2016-06-21 12:43:06.000000 findx-0.9.8/findx.egg-info/dependency_links.txt
--rw-rw-r--   0 mike      (2001) mike      (2001)      454 2016-05-26 11:17:09.000000 findx-0.9.8/runtests.py
--rw-rw-r--   0 mike      (2001) mike      (2001)       59 2016-06-21 12:43:06.000000 findx-0.9.8/setup.cfg
--rwxrwxr-x   0 mike      (2001) mike      (2001)     1441 2016-05-26 11:25:27.000000 findx-0.9.8/setup.py
--rw-rw-r--   0 mike      (2001) mike      (2001)     1122 2016-05-18 23:43:49.000000 findx-0.9.8/LICENSE.rst
-drwxrwxr-x   0 mike      (2001) mike      (2001)        0 2016-06-21 12:43:06.000000 findx-0.9.8/test/
--rw-rw-r--   0 mike      (2001) mike      (2001)        0 2016-05-18 11:19:45.000000 findx-0.9.8/test/__init__.py
--rwxrwxr-x   0 mike      (2001) mike      (2001)     6233 2016-05-26 10:16:53.000000 findx-0.9.8/test/test_findx.py
--rw-rw-r--   0 mike      (2001) mike      (2001)     1681 2016-06-21 12:38:40.000000 findx-0.9.8/CHANGES.rst
--rwxrwxr-x   0 mike      (2001) mike      (2001)    24554 2016-06-21 12:38:43.000000 findx-0.9.8/findx.py
--rw-rw-r--   0 mike      (2001) mike      (2001)     3051 2016-05-19 01:02:08.000000 findx-0.9.8/README.rst
--rw-rw-r--   0 mike      (2001) mike      (2001)     4686 2016-06-21 12:43:06.000000 findx-0.9.8/PKG-INFO
+drwxrwxr-x   0 mike      (2001) mike      (2001)        0 2016-06-25 18:09:25.000000 findx-0.9.9/
+drwxrwxr-x   0 mike      (2001) mike      (2001)        0 2016-06-25 18:09:25.000000 findx-0.9.9/findx.egg-info/
+-rw-rw-r--   0 mike      (2001) mike      (2001)        1 2016-06-25 14:09:42.000000 findx-0.9.9/findx.egg-info/zip-safe
+-rw-rw-r--   0 mike      (2001) mike      (2001)        1 2016-06-25 18:09:25.000000 findx-0.9.9/findx.egg-info/dependency_links.txt
+-rw-rw-r--   0 mike      (2001) mike      (2001)       70 2016-06-25 18:09:25.000000 findx-0.9.9/findx.egg-info/entry_points.txt
+-rw-rw-r--   0 mike      (2001) mike      (2001)       11 2016-06-25 18:09:25.000000 findx-0.9.9/findx.egg-info/top_level.txt
+-rw-rw-r--   0 mike      (2001) mike      (2001)      308 2016-06-25 18:09:25.000000 findx-0.9.9/findx.egg-info/SOURCES.txt
+-rw-rw-r--   0 mike      (2001) mike      (2001)     4686 2016-06-25 18:09:25.000000 findx-0.9.9/findx.egg-info/PKG-INFO
+-rw-rw-r--   0 mike      (2001) mike      (2001)       46 2016-06-25 18:09:25.000000 findx-0.9.9/findx.egg-info/pbr.json
+-rw-rw-r--   0 mike      (2001) mike      (2001)       59 2016-06-25 18:09:25.000000 findx-0.9.9/setup.cfg
+-rw-rw-r--   0 mike      (2001) mike      (2001)     1864 2016-06-25 18:02:02.000000 findx-0.9.9/CHANGES.rst
+-rw-rw-r--   0 mike      (2001) mike      (2001)     1122 2016-06-23 10:34:15.000000 findx-0.9.9/LICENSE.rst
+-rwxrwxr-x   0 mike      (2001) mike      (2001)     1441 2016-06-23 10:34:15.000000 findx-0.9.9/setup.py
+-rw-rw-r--   0 mike      (2001) mike      (2001)     3051 2016-06-23 10:34:15.000000 findx-0.9.9/README.rst
+-rwxrwxr-x   0 mike      (2001) mike      (2001)    27365 2016-06-25 18:02:02.000000 findx-0.9.9/findx.py
+drwxrwxr-x   0 mike      (2001) mike      (2001)        0 2016-06-25 18:09:25.000000 findx-0.9.9/test/
+-rw-rw-r--   0 mike      (2001) mike      (2001)        0 2016-06-23 10:34:15.000000 findx-0.9.9/test/__init__.py
+-rwxrwxr-x   0 mike      (2001) mike      (2001)     6233 2016-06-23 10:34:15.000000 findx-0.9.9/test/test_findx.py
+-rw-rw-r--   0 mike      (2001) mike      (2001)      454 2016-06-23 10:34:15.000000 findx-0.9.9/runtests.py
+-rw-rw-r--   0 mike      (2001) mike      (2001)     4686 2016-06-25 18:09:25.000000 findx-0.9.9/PKG-INFO
+-rw-rw-r--   0 mike      (2001) mike      (2001)       60 2016-06-23 10:34:15.000000 findx-0.9.9/MANIFEST.in
```

### Comparing `findx-0.9.8/findx.egg-info/PKG-INFO` & `findx-0.9.9/findx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 1.0
+Metadata-Version: 1.1
 Name: findx
-Version: 0.9.8
+Version: 0.9.9
 Summary: ``findx``, an extended ``find`` command.
 Home-page: https://github.com/drmikehenry/findx
 Author: Michael Henry
 Author-email: drmikehenry@drmikehenry.com
 License: MIT
 Description: findx - an extended ``find`` command.
         =====================================
```

### Comparing `findx-0.9.8/setup.py` & `findx-0.9.9/setup.py`

 * *Files identical despite different names*

### Comparing `findx-0.9.8/LICENSE.rst` & `findx-0.9.9/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `findx-0.9.8/test/test_findx.py` & `findx-0.9.9/test/test_findx.py`

 * *Files identical despite different names*

### Comparing `findx-0.9.8/CHANGES.rst` & `findx-0.9.9/CHANGES.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 *******
 History
 *******
 
+Version 0.9.9
+=============
+
+- Return an exit status from ``findx``, reflecting errors from ``find``,
+  ``xargs``, or ``findx`` itself.  See ``findx --help`` for exit status values.
+
 Version 0.9.8
 =============
 
 - Add support for Travis CI (thanks to John Vandenberg).
 
 Version 0.9.7
 =============
```

### Comparing `findx-0.9.8/findx.py` & `findx-0.9.9/findx.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,18 +2,20 @@
 
 from __future__ import print_function
 from __future__ import unicode_literals
 
 import os
 import sys
 import re
+import traceback
+import signal
 import distutils.spawn
 from subprocess import Popen, STDOUT, PIPE
 
-__version__ = '0.9.8'
+__version__ = '0.9.9'
 
 HELP_TEXT = """\
 Usage: findx [OPTION | FINDOPTION | DIR | METAGLOB]*
   or:  findx [OPTION | FINDOPTION | DIR | METAGLOB]* : [XARG]+
 
 Additional shortcut commands:
 
@@ -118,14 +120,36 @@
   (Use '-show' to see the list.)
 
 STANDARD ACTION
   If EXPRESSION contains no 'find' action (e.g., '-print', '-print0',
   '-delete', ...), a standard action will be appended to EXPRESSION.  The
   standard action is '-print0' when XARGS are present, and '-print' otherwise.
 
+EXIT STATUS
+  0         full success
+  1         ``findx`` syntax error (e.g., invalid command-line option)
+  2         ``findx`` runtime error (e.g., missing ``xargs`` command)
+  3         ``findx`` uncaught exception (if seen, please submit a bug report)
+  4..99     reserved
+  100       multiple pipeline failures (``find`` and ``xargs`` both non-zero)
+
+  101..119  ``find`` returned 1..19
+  120       ``find`` returned 20..127
+
+  121       ``xargs`` returned 1
+  122       ``xargs`` returned 2..122
+  123..127  ``xargs`` returned 123..127
+
+  128+n     ``findx`` or other program terminated on signal n
+
+  Returning 128+n takes precedence over returning 100.  If any of ``findx``,
+  ``find``, or ``xargs`` are terminated by a signal, the overall exit status
+  will reflect one of their individual exit statuses rather than a combined
+  code of 100.
+
 EXAMPLES
 
 # Grep for 'main' in .c and .cpp files.
   findx *.{c,cpp} : grep main
 
 # Grep for 'main' in .c and .cpp files, excluding .svn and CVS directories.
   findx *.{c,cpp} -x -name .svn,CVS : grep main
@@ -173,45 +197,85 @@
         try:
             msg = self.msg
         except AttributeError:
             msg = self.__class__.__name__
         return msg + ' ' + ', '.join(map(repr, self.args))
 
 
-class MissingArgumentError(FindxError):
+class FindxSyntaxError(FindxError):
+    pass
+
+
+class FindxRuntimeError(FindxError):
+    pass
+
+
+class MissingArgumentError(FindxSyntaxError):
     msg = 'Error: Missing argument'
 
 
-class MissingXargError(FindxError):
+class MissingXargError(FindxSyntaxError):
     msg = 'Error: Missing required xarg'
 
 
-class InvalidOptionError(FindxError):
+class InvalidOptionError(FindxSyntaxError):
     msg = 'Error: Invalid option'
 
 
-class InvalidDirectoryError(FindxError):
-    msg = 'Error: Invalid directory'
+class PrintWithXargsError(FindxSyntaxError):
+    msg = """Error: Cannot mix '-print' with XARGS"""
 
 
-class PrintWithXargsError(FindxError):
-    msg = """Error: Cannot mix '-print' with XARGS"""
+class InvalidDirectoryError(FindxRuntimeError):
+    msg = 'Error: Invalid directory'
 
 
-class ExecutableNotFoundError(FindxError):
+class ExecutableNotFoundError(FindxRuntimeError):
     msg = 'Error: Executable not found'
 
 
 def must_find_executable(name):
     executable_abs_path = distutils.spawn.find_executable(name)
     if executable_abs_path is None:
         raise ExecutableNotFoundError(name)
     return executable_abs_path
 
 
+def map_find_status(find_status):
+    if 1 <= find_status <= 19:
+        return 100 + find_status
+    elif 20 <= find_status <= 127:
+        return 120
+    else:
+        return find_status
+
+
+def map_xargs_status(xargs_status):
+    if xargs_status == 1:
+        return 121
+    elif 2 <= xargs_status <= 122:
+        return 122
+    else:
+        return xargs_status
+
+
+def merge_find_xargs_status(find_status, xargs_status):
+    if find_status >= 128:
+        exit_status = find_status
+    elif xargs_status >= 128:
+        exit_status = xargs_status
+    elif find_status != 0 and xargs_status != 0:
+        exit_status = 100
+    elif find_status != 0:
+        exit_status = map_find_status(find_status)
+    else:
+        exit_status = map_xargs_status(xargs_status)
+    return exit_status
+
+
 class Findx(object):
     OPTIONS_0 = []
     OPTIONS_1 = []
     OPTIONS_2 = []
     OPTIONS_VAR = []
 
     # PRE_PATH_OPTIONS must come before any paths.
@@ -367,14 +431,15 @@
         self.need_xarg = False
         self.xargs = []
         self.find_pipe_args = []
         self.xargs_pipe_args = []
         self.show = False
         self.show_help = False
         self.show_version = False
+        self.pipe_status = None
 
         self.check_xargs()
 
     def check_xargs(self):
         try:
             p = Popen(['xargs', '--version'], stdout=PIPE, stderr=STDOUT)
             output = p.communicate()[0]
@@ -722,14 +787,16 @@
             if self.is_gnu_xargs:
                 self.xargs_pipe_args.append('--no-run-if-empty')
             self.xargs_pipe_args.extend(self.xargs)
         else:
             self.xargs_pipe_args = []
 
     def run(self):
+        self.pipe_status = None
+        exit_status = 0
         if self.show_help:
             self.help()
         elif self.show_version:
             print('findx version %s' % __version__)
         elif self.show:
             s = ' '.join(self.find_pipe_args)
             if self.xargs_pipe_args:
@@ -745,38 +812,57 @@
                 find_proc = Popen(self.find_pipe_args, stdout=PIPE,
                                   executable=find_abs_path)
                 xargs_proc = Popen(self.xargs_pipe_args,
                                    stdin=find_proc.stdout,
                                    executable=xargs_abs_path)
                 find_proc.wait()
                 xargs_proc.wait()
+                find_status = find_proc.returncode
+                xargs_status = xargs_proc.returncode
+                self.pipe_status = (find_status, xargs_status)
+                exit_status = merge_find_xargs_status(find_status,
+                                                      xargs_status)
             else:
                 find_proc = Popen(self.find_pipe_args,
                                   executable=find_abs_path)
                 find_proc.wait()
+                find_status = find_proc.returncode
+                self.pipe_status = (find_status,)
+                exit_status = merge_find_xargs_status(find_status, 0)
+        return exit_status
 
     def help(self):
         print(HELP_TEXT)
 
 
 def main():
-    f = Findx()
     try:
-        f.parse_command_line(sys.argv[1:])
-        f.run()
-    except FindxError as e:
-        print(e)
-    except KeyboardInterrupt as e:
-        print('<break>')
+        f = Findx()
+        try:
+            f.parse_command_line(sys.argv[1:])
+            exit_status = f.run()
+        except FindxSyntaxError as e:
+            print('findx:', e, file=sys.stderr)
+            exit_status = 1
+        except FindxRuntimeError as e:
+            print('findx:', e, file=sys.stderr)
+            exit_status = 2
+        except KeyboardInterrupt:
+            exit_status = 128 + signal.SIGINT
+    except:
+        print('findx: Uncaught exception:', file=sys.stderr)
+        traceback.print_exc()
+        exit_status = 3
+    return exit_status
 
 
 def ffx():
     sys.argv.insert(1, '-ffx')
-    main()
+    return main()
 
 
 def ffg():
     sys.argv.insert(1, '-ffg')
-    main()
+    return main()
 
 if __name__ == '__main__':
-    main()
+    sys.exit(main())
```

### Comparing `findx-0.9.8/README.rst` & `findx-0.9.9/README.rst`

 * *Files identical despite different names*

### Comparing `findx-0.9.8/PKG-INFO` & `findx-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 1.0
+Metadata-Version: 1.1
 Name: findx
-Version: 0.9.8
+Version: 0.9.9
 Summary: ``findx``, an extended ``find`` command.
 Home-page: https://github.com/drmikehenry/findx
 Author: Michael Henry
 Author-email: drmikehenry@drmikehenry.com
 License: MIT
 Description: findx - an extended ``find`` command.
         =====================================
```

