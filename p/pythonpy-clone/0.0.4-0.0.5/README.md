# Comparing `tmp/pythonpy-clone-0.0.4.tar.gz` & `tmp/pythonpy_clone-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pythonpy-clone-0.0.4.tar", last modified: Fri Nov 22 11:43:32 2019, max compression
+gzip compressed data, was "pythonpy_clone-0.0.5.tar", last modified: Mon May 27 03:00:57 2024, max compression
```

## Comparing `pythonpy-clone-0.0.4.tar` & `pythonpy_clone-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2019-11-22 11:43:32.801072 pythonpy-clone-0.0.4/
--rw-r--r--   0 user      (1000) user      (1000)     1764 2019-11-22 11:43:32.801072 pythonpy-clone-0.0.4/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      886 2019-10-21 21:21:03.000000 pythonpy-clone-0.0.4/README.md
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2019-11-22 11:43:32.801072 pythonpy-clone-0.0.4/pythonpy_clone.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     1764 2019-11-22 11:43:32.000000 pythonpy-clone-0.0.4/pythonpy_clone.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      266 2019-11-22 11:43:32.000000 pythonpy-clone-0.0.4/pythonpy_clone.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2019-11-22 11:43:32.000000 pythonpy-clone-0.0.4/pythonpy_clone.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)       98 2019-11-22 11:43:32.000000 pythonpy-clone-0.0.4/pythonpy_clone.egg-info/entry_points.txt
--rw-r--r--   0 user      (1000) user      (1000)       32 2019-11-22 11:43:32.000000 pythonpy-clone-0.0.4/pythonpy_clone.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)       15 2019-11-22 11:43:32.000000 pythonpy-clone-0.0.4/pythonpy_clone.egg-info/top_level.txt
--rwxr-xr-x   0 user      (1000) user      (1000)     2741 2019-11-22 11:34:48.000000 pythonpy-clone-0.0.4/pythonpy_clone.py
--rw-r--r--   0 user      (1000) user      (1000)       38 2019-11-22 11:43:32.801072 pythonpy-clone-0.0.4/setup.cfg
--rwxr-xr-x   0 user      (1000) user      (1000)     1294 2019-11-22 11:32:59.000000 pythonpy-clone-0.0.4/setup.py
+drwxr-x---   0 user      (1000) user      (1000)        0 2024-05-27 03:00:57.857009 pythonpy_clone-0.0.5/
+-rw-r-----   0 user      (1000) user      (1000)     1551 2024-05-26 05:09:07.000000 pythonpy_clone-0.0.5/LICENSE.md
+-rw-r--r--   0 user      (1000) user      (1000)     1607 2024-05-27 03:00:57.857009 pythonpy_clone-0.0.5/PKG-INFO
+-rw-r-----   0 user      (1000) user      (1000)      886 2024-05-26 05:09:07.000000 pythonpy_clone-0.0.5/README.md
+drwxr-x---   0 user      (1000) user      (1000)        0 2024-05-27 03:00:57.857009 pythonpy_clone-0.0.5/pythonpy_clone.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     1607 2024-05-27 03:00:57.000000 pythonpy_clone-0.0.5/pythonpy_clone.egg-info/PKG-INFO
+-rw-r-----   0 user      (1000) user      (1000)      277 2024-05-27 03:00:57.000000 pythonpy_clone-0.0.5/pythonpy_clone.egg-info/SOURCES.txt
+-rw-r-----   0 user      (1000) user      (1000)        1 2024-05-27 03:00:57.000000 pythonpy_clone-0.0.5/pythonpy_clone.egg-info/dependency_links.txt
+-rw-r-----   0 user      (1000) user      (1000)       98 2024-05-27 03:00:57.000000 pythonpy_clone-0.0.5/pythonpy_clone.egg-info/entry_points.txt
+-rw-r-----   0 user      (1000) user      (1000)       32 2024-05-27 03:00:57.000000 pythonpy_clone-0.0.5/pythonpy_clone.egg-info/requires.txt
+-rw-r-----   0 user      (1000) user      (1000)       15 2024-05-27 03:00:57.000000 pythonpy_clone-0.0.5/pythonpy_clone.egg-info/top_level.txt
+-rwxr-x---   0 user      (1000) user      (1000)     2741 2024-05-27 02:58:47.000000 pythonpy_clone-0.0.5/pythonpy_clone.py
+-rw-r-----   0 user      (1000) user      (1000)       38 2024-05-27 03:00:57.857009 pythonpy_clone-0.0.5/setup.cfg
+-rwxr-x---   0 user      (1000) user      (1000)     1296 2024-05-27 02:58:32.000000 pythonpy_clone-0.0.5/setup.py
```

### Comparing `pythonpy-clone-0.0.4/PKG-INFO` & `pythonpy_clone-0.0.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 Metadata-Version: 2.1
 Name: pythonpy-clone
-Version: 0.0.4
+Version: 0.0.5
 Summary: rewrite of pythonpy using AST manipulations instead of regex
-Home-page: https://github.com/iomintz/pythonpy-clone
-Author: Io Mintz
+Home-page: https://github.com/ioistired/pythonpy-clone
+Author: io mintz
 License: BlueOak-1.0.0
-Description: # pythonpy clone
-        
-        This is a rewrite of [pythonpy] with (planned) feature parity and which is more robust. Instead of using regex to attempt to automatically
-        import all identifiers, it uses a library which I already wrote called [Import Expression Parser] to add easy inline imports
-        e.g. `urllib.parse!.quote("a b c")`.
-        
-        For more information, see the [pythonpy] README and `py --help`.
-        
-        [pythonpy]: https://github.com/Russell91/pythonpy
-        [Import Expression Parser]: https://github.com/iomintz/import-expression-parser
-        
-        ## Installation
-        
-        `pip install pythonpy-clone` (or via [pipx]: `pipx install pythonpy-clone`)
-        
-        From source:
-        
-        `pip install .`
-        
-        [pipx]: https://github.com/pipxproject/pipx
-        
-        ## License
-        
-        BlueOak Model License v1.0.0, see [LICENSE.md](/LICENSE.md).
-        For rationale, see [kemitchell's blog post on the matter](https://writing.kemitchell.com/2019/03/09/Deprecation-Notice.html).
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: System Administrators
 Classifier: Topic :: Utilities
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown; variant=GFM
+License-File: LICENSE.md
+Requires-Dist: import-expression<3.0.0,>=2.0.0
+
+# pythonpy clone
+
+This is a rewrite of [pythonpy] with (planned) feature parity and which is more robust. Instead of using regex to attempt to automatically
+import all identifiers, it uses a library which I already wrote called [Import Expression Parser] to add easy inline imports
+e.g. `urllib.parse!.quote("a b c")`.
+
+For more information, see the [pythonpy] README and `py --help`.
+
+[pythonpy]: https://github.com/Russell91/pythonpy
+[Import Expression Parser]: https://github.com/iomintz/import-expression-parser
+
+## Installation
+
+`pip install pythonpy-clone` (or via [pipx]: `pipx install pythonpy-clone`)
+
+From source:
+
+`pip install .`
+
+[pipx]: https://github.com/pipxproject/pipx
+
+## License
+
+BlueOak Model License v1.0.0, see [LICENSE.md](/LICENSE.md).
+For rationale, see [kemitchell's blog post on the matter](https://writing.kemitchell.com/2019/03/09/Deprecation-Notice.html).
```

### Comparing `pythonpy-clone-0.0.4/README.md` & `pythonpy_clone-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pythonpy-clone-0.0.4/pythonpy_clone.egg-info/PKG-INFO` & `pythonpy_clone-0.0.5/pythonpy_clone.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 Metadata-Version: 2.1
 Name: pythonpy-clone
-Version: 0.0.4
+Version: 0.0.5
 Summary: rewrite of pythonpy using AST manipulations instead of regex
-Home-page: https://github.com/iomintz/pythonpy-clone
-Author: Io Mintz
+Home-page: https://github.com/ioistired/pythonpy-clone
+Author: io mintz
 License: BlueOak-1.0.0
-Description: # pythonpy clone
-        
-        This is a rewrite of [pythonpy] with (planned) feature parity and which is more robust. Instead of using regex to attempt to automatically
-        import all identifiers, it uses a library which I already wrote called [Import Expression Parser] to add easy inline imports
-        e.g. `urllib.parse!.quote("a b c")`.
-        
-        For more information, see the [pythonpy] README and `py --help`.
-        
-        [pythonpy]: https://github.com/Russell91/pythonpy
-        [Import Expression Parser]: https://github.com/iomintz/import-expression-parser
-        
-        ## Installation
-        
-        `pip install pythonpy-clone` (or via [pipx]: `pipx install pythonpy-clone`)
-        
-        From source:
-        
-        `pip install .`
-        
-        [pipx]: https://github.com/pipxproject/pipx
-        
-        ## License
-        
-        BlueOak Model License v1.0.0, see [LICENSE.md](/LICENSE.md).
-        For rationale, see [kemitchell's blog post on the matter](https://writing.kemitchell.com/2019/03/09/Deprecation-Notice.html).
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: System Administrators
 Classifier: Topic :: Utilities
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown; variant=GFM
+License-File: LICENSE.md
+Requires-Dist: import-expression<3.0.0,>=2.0.0
+
+# pythonpy clone
+
+This is a rewrite of [pythonpy] with (planned) feature parity and which is more robust. Instead of using regex to attempt to automatically
+import all identifiers, it uses a library which I already wrote called [Import Expression Parser] to add easy inline imports
+e.g. `urllib.parse!.quote("a b c")`.
+
+For more information, see the [pythonpy] README and `py --help`.
+
+[pythonpy]: https://github.com/Russell91/pythonpy
+[Import Expression Parser]: https://github.com/iomintz/import-expression-parser
+
+## Installation
+
+`pip install pythonpy-clone` (or via [pipx]: `pipx install pythonpy-clone`)
+
+From source:
+
+`pip install .`
+
+[pipx]: https://github.com/pipxproject/pipx
+
+## License
+
+BlueOak Model License v1.0.0, see [LICENSE.md](/LICENSE.md).
+For rationale, see [kemitchell's blog post on the matter](https://writing.kemitchell.com/2019/03/09/Deprecation-Notice.html).
```

### Comparing `pythonpy-clone-0.0.4/pythonpy_clone.py` & `pythonpy_clone-0.0.5/pythonpy_clone.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-__version__ = '0.0.4'
+__version__ = '0.0.5'
 __license__ = 'BlueOak-1.0.0'
 
 """
 A clone of https://github.com/Russell91/pythonpy with less ugly code and supporting import expressions (e.g. sys!.version)
 """
 
 import argparse
```

### Comparing `pythonpy-clone-0.0.4/setup.py` & `pythonpy_clone-0.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,23 +14,23 @@
 	raise RuntimeError('version is not set')
 
 with open(HERE / 'README.md') as f:
 	README = f.read()
 
 setuptools.setup(
 	name='pythonpy-clone',
-	author='Io Mintz',
-	url='https://github.com/iomintz/pythonpy-clone',
+	author='io mintz',
+	url='https://github.com/ioistired/pythonpy-clone',
 	version=VERSION,
 	py_modules=['pythonpy_clone'],
 	license='BlueOak-1.0.0',
 	description='rewrite of pythonpy using AST manipulations instead of regex',
 	long_description=README,
 	long_description_content_type='text/markdown; variant=GFM',
-	install_requires=['import-expression>=1.0.0,<2.0.0'],
+	install_requires=['import-expression>=2.0.0,<3.0.0'],
 	python_requires='>=3.6.0',
 	classifiers=[
 		'Development Status :: 3 - Alpha',
 		'Environment :: Console',
 		'Intended Audience :: Developers',
 		'Intended Audience :: End Users/Desktop',
 		'Intended Audience :: System Administrators',
```

