# Comparing `tmp/fortran-magic-0.8.tar.gz` & `tmp/fortran_magic-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fortran-magic-0.8.tar", last modified: Fri Jun 16 11:02:18 2023, max compression
+gzip compressed data, was "fortran_magic-0.9.tar", last modified: Mon May 27 14:22:02 2024, max compression
```

## Comparing `fortran-magic-0.8.tar` & `fortran_magic-0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:02:18.060196 fortran-magic-0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-06-16 11:02:08.000000 fortran-magic-0.8/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-06-16 11:02:08.000000 fortran-magic-0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 11:02:08.000000 fortran-magic-0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-06-16 11:02:18.060196 fortran-magic-0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-06-16 11:02:08.000000 fortran-magic-0.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:02:18.056196 fortran-magic-0.8/fortran_magic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-06-16 11:02:18.000000 fortran-magic-0.8/fortran_magic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-16 11:02:18.000000 fortran-magic-0.8/fortran_magic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 11:02:18.000000 fortran-magic-0.8/fortran_magic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-16 11:02:18.000000 fortran-magic-0.8/fortran_magic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-16 11:02:18.000000 fortran-magic-0.8/fortran_magic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    15908 2023-06-16 11:02:08.000000 fortran-magic-0.8/fortranmagic.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 11:02:18.060196 fortran-magic-0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-06-16 11:02:08.000000 fortran-magic-0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:02:18.060196 fortran-magic-0.8/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-16 11:02:08.000000 fortran-magic-0.8/test/test_010_init_cfg_and_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-06-16 11:02:08.000000 fortran-magic-0.8/test/test_documentation_ipynb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-16 11:02:08.000000 fortran-magic-0.8/test/test_f2py.py
--rw-r--r--   0 runner    (1001) docker     (123)     7639 2023-06-16 11:02:08.000000 fortran-magic-0.8/test/test_fortran_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-16 11:02:08.000000 fortran-magic-0.8/test/test_oserror.py
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-06-16 11:02:08.000000 fortran-magic-0.8/test/test_readme_rst.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-16 11:02:08.000000 fortran-magic-0.8/test/test_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-16 11:02:08.000000 fortran-magic-0.8/test/test_zload_ext.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:22:02.318351 fortran_magic-0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-05-27 14:21:55.000000 fortran_magic-0.9/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-27 14:21:55.000000 fortran_magic-0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 14:21:55.000000 fortran_magic-0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6529 2024-05-27 14:22:02.318351 fortran_magic-0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-05-27 14:21:55.000000 fortran_magic-0.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:22:02.318351 fortran_magic-0.9/fortran_magic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6529 2024-05-27 14:22:02.000000 fortran_magic-0.9/fortran_magic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-27 14:22:02.000000 fortran_magic-0.9/fortran_magic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 14:22:02.000000 fortran_magic-0.9/fortran_magic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-27 14:22:02.000000 fortran_magic-0.9/fortran_magic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-27 14:22:02.000000 fortran_magic-0.9/fortran_magic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18738 2024-05-27 14:21:55.000000 fortran_magic-0.9/fortranmagic.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 14:22:02.318351 fortran_magic-0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-27 14:21:55.000000 fortran_magic-0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:22:02.318351 fortran_magic-0.9/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-27 14:21:55.000000 fortran_magic-0.9/test/test_010_init_cfg_and_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6632 2024-05-27 14:21:55.000000 fortran_magic-0.9/test/test_documentation_ipynb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-05-27 14:21:55.000000 fortran_magic-0.9/test/test_f2py.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7775 2024-05-27 14:21:55.000000 fortran_magic-0.9/test/test_fortran_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-27 14:21:55.000000 fortran_magic-0.9/test/test_oserror.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-05-27 14:21:55.000000 fortran_magic-0.9/test/test_readme_rst.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-27 14:21:55.000000 fortran_magic-0.9/test/test_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-27 14:21:55.000000 fortran_magic-0.9/test/test_zload_ext.py
```

### Comparing `fortran-magic-0.8/CHANGES.rst` & `fortran_magic-0.9/CHANGES.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,26 @@
 
 Changelog
 =========
 
-0.8 / 2023-06-08
+0.9 / 2024-05-27
+----------------
+
+- Fix for NumPy 1.26 & Python 3.12. Warning: When using the Meson build
+  system (3.12 and later), there are some limitations and differences in
+  the interface.
+
+- Ready to NumPy 2.0
+
+`Serguei E. Leontiev`_
+
+.. _Serguei E. Leontiev: https://github.com/Serge3leo
+
+
+0.8 / 2023-06-16
 ----------------
 
 - Fix use deprecating ``imp`` module (removed from Python 3.12b2)
 
 - Fix exponential duplication any not boolean flags of
   ``%%fortran_config``
```

### Comparing `fortran-magic-0.8/LICENSE` & `fortran_magic-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fortran-magic-0.8/PKG-INFO` & `fortran_magic-0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fortran-magic
-Version: 0.8
+Version: 0.9
 Summary: An extension for IPython that help to use Fortran in your interactive session.
 Home-page: https://github.com/mgaitan/fortran_magic
 Author: Martin Gaitan
 Author-email: gaitan@gmail.com
 License: BSD
 Keywords: ipython notebook fortran f2py science
 Classifier: Development Status :: 4 - Beta
@@ -15,14 +15,16 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Fortran
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: ipython
+Requires-Dist: numpy
 
 =============
 Fortran magic
 =============
 
 .. image:: https://img.shields.io/pypi/v/fortran-magic
    :target: https://pypi.python.org/pypi/fortran-magic
@@ -100,15 +102,29 @@
 See the documentation_ for further details.
 
 
 
 Changelog
 =========
 
-0.8 / 2023-06-08
+0.9 / 2024-05-27
+----------------
+
+- Fix for NumPy 1.26 & Python 3.12. Warning: When using the Meson build
+  system (3.12 and later), there are some limitations and differences in
+  the interface.
+
+- Ready to NumPy 2.0
+
+`Serguei E. Leontiev`_
+
+.. _Serguei E. Leontiev: https://github.com/Serge3leo
+
+
+0.8 / 2023-06-16
 ----------------
 
 - Fix use deprecating ``imp`` module (removed from Python 3.12b2)
 
 - Fix exponential duplication any not boolean flags of
   ``%%fortran_config``
```

### Comparing `fortran-magic-0.8/README.rst` & `fortran_magic-0.9/README.rst`

 * *Files identical despite different names*

### Comparing `fortran-magic-0.8/fortran_magic.egg-info/PKG-INFO` & `fortran_magic-0.9/fortran_magic.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fortran-magic
-Version: 0.8
+Version: 0.9
 Summary: An extension for IPython that help to use Fortran in your interactive session.
 Home-page: https://github.com/mgaitan/fortran_magic
 Author: Martin Gaitan
 Author-email: gaitan@gmail.com
 License: BSD
 Keywords: ipython notebook fortran f2py science
 Classifier: Development Status :: 4 - Beta
@@ -15,14 +15,16 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Fortran
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: ipython
+Requires-Dist: numpy
 
 =============
 Fortran magic
 =============
 
 .. image:: https://img.shields.io/pypi/v/fortran-magic
    :target: https://pypi.python.org/pypi/fortran-magic
@@ -100,15 +102,29 @@
 See the documentation_ for further details.
 
 
 
 Changelog
 =========
 
-0.8 / 2023-06-08
+0.9 / 2024-05-27
+----------------
+
+- Fix for NumPy 1.26 & Python 3.12. Warning: When using the Meson build
+  system (3.12 and later), there are some limitations and differences in
+  the interface.
+
+- Ready to NumPy 2.0
+
+`Serguei E. Leontiev`_
+
+.. _Serguei E. Leontiev: https://github.com/Serge3leo
+
+
+0.8 / 2023-06-16
 ----------------
 
 - Fix use deprecating ``imp`` module (removed from Python 3.12b2)
 
 - Fix exponential duplication any not boolean flags of
   ``%%fortran_config``
```

### Comparing `fortran-magic-0.8/fortranmagic.py` & `fortran_magic-0.9/fortranmagic.py`

 * *Files 16% similar despite different names*

```diff
@@ -29,20 +29,25 @@
 
 import numpy as np
 from IPython.core import display, magic_arguments
 from IPython.core.magic import Magics, cell_magic, line_magic, magics_class
 from IPython.paths import get_ipython_cache_dir
 from IPython.utils import py3compat
 from IPython.utils.io import capture_output
-from numpy.distutils import fcompiler
 from numpy.f2py import f2py2e
 
-__version__ = '0.8'
-fcompiler.load_all_fcompiler_classes()
+__version__ = '0.9'
 
+try:
+    from numpy.distutils import fcompiler
+
+    _use_meson = False
+    fcompiler.load_all_fcompiler_classes()
+except ImportError:
+    _use_meson = True
 
 try:
     import importlib.machinery
     import importlib.util
 
     def _imp_load_dynamic(name, path):
         loader = importlib.machinery.ExtensionFileLoader(name, path)
@@ -83,57 +88,72 @@
         return v[1:-1]
     return v
 
 
 @magics_class
 class FortranMagics(Magics):
 
-    allowed_fcompilers = sorted(fcompiler.fcompiler_class.keys())
+    if _use_meson:
+        allowed_fcompilers = None
+    else:
+        allowed_fcompilers = sorted(fcompiler.fcompiler_class.keys())
     allowed_compilers = sorted(compiler_class.keys())
 
     my_magic_arguments = compose(
         magic_arguments.magic_arguments(),
         magic_arguments.argument(
             "-v", "--verbosity", action="count", default=0,
             help="increase output verbosity"
         ),
         magic_arguments.argument(
+            '--backend',
+            choices=['distutils', 'meson'],
+            help="""Specify the build backend for the compilation
+                 process. On Python 3.12 or higher, the default is
+                 'meson', see numpy.f2py documentation for details.
+                 [TODO, unimplemented]"""  # TODO:XXX
+        ),
+        magic_arguments.argument(
             '--fcompiler',
             choices=allowed_fcompilers,
             help="""Specify Fortran compiler type by vendor.
-                 See %%f2py_help --fcompiler""",
+                 See %%f2py_help --fcompiler. [NO_MESON]""",
         ),
         magic_arguments.argument(
             '--compiler',
             choices=allowed_compilers,
             help="""Specify C compiler type (as defined by distutils).
-                    See %%f2py_help --compiler"""
+                    See %%f2py_help --compiler.  [NO_MESON]"""
         ),
         magic_arguments.argument(
             '--f90flags', help="Specify F90 compiler flags"
         ),
         magic_arguments.argument(
             '--f77flags', help="Specify F77 compiler flags"
         ),
         magic_arguments.argument(
-            '--opt', help="Specify optimization flags"
+            '--opt', help="Specify optimization flags. [NO_MESON]"
         ),
         magic_arguments.argument(
-            '--arch', help="Specify architecture specific optimization flags"
+            '--arch',
+            help="""Specify architecture specific optimization flags.
+                 [NO_MESON]"""
         ),
         magic_arguments.argument(
-            '--noopt', action="store_true", help="Compile without optimization"
+            '--noopt', action="store_true",
+            help="Compile without optimization. [NO_MESON]"
         ),
         magic_arguments.argument(
-            '--noarch', action="store_true", help="Compile without "
-            "arch-dependent optimization"
+            '--noarch', action="store_true",
+            help="""Compile without arch-dependent optimization.
+                 [NO_MESON]"""
         ),
         magic_arguments.argument(
-            '--debug', action="store_true", help="Compile with debugging "
-            "information"
+            '--debug', action="store_true",
+            help="Compile with debugging information"
         ),
         magic_arguments.argument(
             '--link', action='append', default=[],
             help="""Link extension module with LINK resource, as defined
                     by numpy.distutils/system_info.py. E.g. to link
                     with optimized LAPACK libraries (vecLib on MacOSX,
                     ATLAS elsewhere), use --link lapack_opt.
@@ -213,18 +233,29 @@
                 v.__source__ = code
                 self.shell.push({k: v})
                 imported.append(k)
         if verbosity > 0 and imported:
             print("\nOk. The following fortran objects "
                   "are ready to use: %s" % ", ".join(imported))
 
-    def _run_f2py(self, argv, show_captured=False, verbosity=0):
+    def _run_f2py(self,
+                  argv,
+                  show_captured=False,
+                  verbosity=0,
+                  fflags=None):
         """
         Here we directly call the numpy.f2py module or the f2py executable.
         """
+        environ = None if fflags is None else os.environ.copy()
+        if fflags is not None:
+            environ = os.environ.copy()
+            environ['FFLAGS'] = environ.get('FFLAGS', '') + ' ' + fflags
+        else:
+            environ = None
+
         if np.__version__ < LooseVersion('1.10.0'):
             if sys.version_info[0] >= 3:
                 command = ['f2py3']
             else:
                 command = ['f2py']
         else:
             command = [sys.executable, '-m', 'numpy.f2py']
@@ -236,14 +267,15 @@
         p, out, err = None, None, None
         try:
             with capture_output() as captured:
                 # subprocess.call(command)
                 # Refactor subprocess call to work with jupyterhub
                 try:
                     p = Popen(command, stdout=PIPE, stderr=PIPE, stdin=PIPE,
+                              env=environ,
                               cwd=self._lib_dir)
                 except OSError as e:
                     if e.errno == errno.ENOENT:
                         print("Couldn't find program: %r" % command[0])
                         return -1
                     raise
                 out, err = p.communicate(input=None)
@@ -401,15 +433,22 @@
         kw = ['--%s=%s' % (k, v) for k, v in vars(args).items()
               if isinstance(v, base_str_class)]
 
         f2py_args.extend(kw)
 
         # link resource
         if args.link:
-            resources = ['--link-%s' % r for r in args.link]
+            # TODO: Now `f2py --backend meson` unimplemented
+            if not _use_meson:
+                resources = ['--link-%s' % r for r in args.link]
+            else:
+                resources = []
+                for r in args.link:
+                    resources.append('--dep')
+                    resources.append(r)
             f2py_args.extend(resources)
 
         if args.extra:
             extras = ' '.join(map(unquote, args.extra))
             extras = extras.split()
             f2py_args.extend(extras)
 
@@ -426,22 +465,57 @@
             module = sys.modules[module_name]
             print("The extension", module_name,
                   "is already loaded. To reload it, use:")
             print("  %fortran_config --clean-cache")
         else:
             module_path = os.path.join(self._lib_dir, module_name + self.so_ext)
 
-            f90_file = os.path.join(self._lib_dir, module_name + '.f90')
-            f90_file = py3compat.cast_bytes_py2(f90_file,
-                                                encoding=sys.getfilesystemencoding())
-            with io.open(f90_file, 'w', encoding='utf-8') as f:
+            fsuffix = ".f90"
+
+            # TODO: Now `f2py --backend meson` unimplemented
+            if not _use_meson:
+                fflags = None
+            else:
+                # `--f77flags` & `--f90flags`. Use `FFLAGS` workaround, see
+                # https://github.com/numpy/numpy/issues/24874#issuecomment-1762981664
+                # https://github.com/numpy/numpy/issues/24874
+
+                if args.f77flags is not None:
+                    fflags = args.f77flags
+                else:
+                    fflags = args.f90flags
+                if args.f77flags is not None and args.f90flags is not None:
+                    # TODO: f2py used requiresf90wrapper()
+                    print("Warning: ambiguity, both f77flags and f90flags "
+                          "are set, assume the %s module" % (
+                              "f77" if fflags == args.f77flags else "f90"),
+                          file=sys.stderr)
+                lfflags = unquote(fflags).split() if fflags is not None else []
+                fflags = ""
+                for flag in lfflags:
+                    if flag == "-ffixed-form":
+                        fsuffix = ".f"
+                    elif flag == "-ffree-form":
+                        fsuffix = ".f90"
+                    else:
+                        fflags += flag + " "
+                if fflags and ' ' == fflags[-1]:
+                    fflags = fflags[:-1]
+
+            f_f90_file = os.path.join(self._lib_dir, module_name + fsuffix)
+            f_f90_file = py3compat.cast_bytes_py2(
+                            f_f90_file,
+                            encoding=sys.getfilesystemencoding())
+            with io.open(f_f90_file, 'w', encoding='utf-8') as f:
                 f.write(code)
 
-            res = self._run_f2py(f2py_args + ['-m', module_name, '-c', f90_file],
-                                 verbosity=args.verbosity)
+            res = self._run_f2py(f2py_args + ['-m', module_name, '-c',
+                                              f_f90_file],
+                                 verbosity=args.verbosity,
+                                 fflags=fflags)
             if res != 0:
                 raise RuntimeError("f2py failed, see output")
 
             self._code_cache[key] = module_name
             module = _imp_load_dynamic(module_name, module_path)
         self._import_all(module, verbosity=args.verbosity, code=code)
```

### Comparing `fortran-magic-0.8/setup.py` & `fortran_magic-0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 long_description = (open('README.rst').read() + '\n\n' +
                     open('CHANGES.rst').read())
 
 setup(
     name='fortran-magic',
-    version='0.8',
+    version='0.9',
     description='An extension for IPython that help to use Fortran in '
                 'your interactive session.',
     long_description=long_description,
     long_description_content_type="text/x-rst",
     author='Martin Gaitan',
     author_email='gaitan@gmail.com',
     url='https://github.com/mgaitan/fortran_magic',
```

### Comparing `fortran-magic-0.8/test/test_010_init_cfg_and_cache.py` & `fortran_magic-0.9/test/test_010_init_cfg_and_cache.py`

 * *Files identical despite different names*

### Comparing `fortran-magic-0.8/test/test_documentation_ipynb.py` & `fortran_magic-0.9/test/test_documentation_ipynb.py`

 * *Files identical despite different names*

### Comparing `fortran-magic-0.8/test/test_f2py.py` & `fortran_magic-0.9/test/test_f2py.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 import numpy.f2py
 import pytest
 
 
 @pytest.mark.skipif(sys.platform.startswith("win"),
                     reason="Probably gnu95/mingw32 can't load module "
                            "with print")
+@pytest.mark.skipif(np.__version__ >= "2",
+                    reason="NumPy 2.0 remove numpy.f2py.compile")
 @pytest.mark.slow
 def test_f2py_compile_fsource(capfd, numpy_correct_compilers):
     """
     Check `numpy.f2py.compile`.
 
     See: https://numpy.org/doc/stable/f2py/usage.html#numpy.f2py.compile
     """
```

### Comparing `fortran-magic-0.8/test/test_fortran_config.py` & `fortran_magic-0.9/test/test_fortran_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 import sys
 import warnings
 
 import IPython.core.interactiveshell as ici
 import IPython.paths
 import pytest
 
+_USE_MESON = (sys.version_info >= (3, 12))
+
 # For slightly faster compilations.
 FORTRAN = "%%fortran --noopt  --f90flags '-O0' "
 
 GOOD_PRG = """
 subroutine hj(x)
     x = 1.
 end subroutine hj
@@ -241,10 +243,12 @@
 
     ctxish.f_config(f_config_arg)
     ctxish.f_config("--clean-cache")
     ctxish.check_pattern([
         {'a': "-vv " + fortran_arg,
          'ps': [
             {'p': "-DNPY_NO_DEPRECATED_API=0", 'o': [2, 2], 'e': [0, 0]},
-            {'p': "--link-lapack", 'o': [1, 1], 'e': [0, 0]},
-            {'p': "--link-blas", 'o': [1, 1], 'e': [0, 0]},
+            {'p': "--dep lapack" if _USE_MESON else "--link-lapack",
+             'o': [1, 1], 'e': [0, 0]},
+            {'p': "--dep blas" if _USE_MESON else "--link-blas",
+             'o': [1, 1], 'e': [0, 0]},
             ]}])
```

### Comparing `fortran-magic-0.8/test/test_oserror.py` & `fortran_magic-0.9/test/test_oserror.py`

 * *Files identical despite different names*

### Comparing `fortran-magic-0.8/test/test_readme_rst.py` & `fortran_magic-0.9/test/test_readme_rst.py`

 * *Files identical despite different names*

### Comparing `fortran-magic-0.8/test/test_zload_ext.py` & `fortran_magic-0.9/test/test_zload_ext.py`

 * *Files identical despite different names*

