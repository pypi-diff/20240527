# Comparing `tmp/asp_selftest-0.0.6.tar.gz` & `tmp/asp_selftest-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asp_selftest-0.0.6.tar", last modified: Thu May 23 14:26:56 2024, max compression
+gzip compressed data, was "asp_selftest-0.0.7.tar", last modified: Mon May 27 09:47:49 2024, max compression
```

## Comparing `asp_selftest-0.0.6.tar` & `asp_selftest-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 erikgroeneveld   (501) staff       (20)        0 2024-05-23 14:26:56.066046 asp_selftest-0.0.6/
--rw-r--r--   0 erikgroeneveld   (501) staff       (20)    35149 2024-02-19 08:25:44.000000 asp_selftest-0.0.6/LICENSE
--rw-r--r--   0 erikgroeneveld   (501) staff       (20)       20 2024-04-25 13:29:32.000000 asp_selftest-0.0.6/MANIFEST.in
--rw-r--r--   0 erikgroeneveld   (501) staff       (20)     3490 2024-05-23 14:26:56.065861 asp_selftest-0.0.6/PKG-INFO
--rw-r--r--   0 erikgroeneveld   (501) staff       (20)     2878 2024-04-25 15:02:28.000000 asp_selftest-0.0.6/README.md
--rw-r--r--   0 erikgroeneveld   (501) staff       (20)      789 2024-05-23 14:26:48.000000 asp_selftest-0.0.6/pyproject.toml
--rw-r--r--   0 erikgroeneveld   (501) staff       (20)       38 2024-05-23 14:26:56.066092 asp_selftest-0.0.6/setup.cfg
-drwxr-xr-x   0 erikgroeneveld   (501) staff       (20)        0 2024-05-23 14:26:56.063924 asp_selftest-0.0.6/src/
-drwxr-xr-x   0 erikgroeneveld   (501) staff       (20)        0 2024-05-23 14:26:56.064915 asp_selftest-0.0.6/src/asp_selftest/
--rw-r--r--   0 erikgroeneveld   (501) staff       (20)      727 2024-05-08 16:37:36.000000 asp_selftest-0.0.6/src/asp_selftest/__init__.py
--rw-r--r--   0 erikgroeneveld   (501) staff       (20)      526 2024-03-01 15:10:30.000000 asp_selftest-0.0.6/src/asp_selftest/example.lp
--rw-r--r--   0 erikgroeneveld   (501) staff       (20)     1277 2024-02-19 15:49:37.000000 asp_selftest-0.0.6/src/asp_selftest/queens.lp
--rwxr-xr-x   0 erikgroeneveld   (501) staff       (20)     9158 2024-05-23 14:24:43.000000 asp_selftest-0.0.6/src/asp_selftest/runasptests.py
-drwxr-xr-x   0 erikgroeneveld   (501) staff       (20)        0 2024-05-23 14:26:56.065657 asp_selftest-0.0.6/src/asp_selftest.egg-info/
--rw-r--r--   0 erikgroeneveld   (501) staff       (20)     3490 2024-05-23 14:26:56.000000 asp_selftest-0.0.6/src/asp_selftest.egg-info/PKG-INFO
--rw-r--r--   0 erikgroeneveld   (501) staff       (20)      363 2024-05-23 14:26:56.000000 asp_selftest-0.0.6/src/asp_selftest.egg-info/SOURCES.txt
--rw-r--r--   0 erikgroeneveld   (501) staff       (20)        1 2024-05-23 14:26:56.000000 asp_selftest-0.0.6/src/asp_selftest.egg-info/dependency_links.txt
--rw-r--r--   0 erikgroeneveld   (501) staff       (20)       55 2024-05-23 14:26:56.000000 asp_selftest-0.0.6/src/asp_selftest.egg-info/entry_points.txt
--rw-r--r--   0 erikgroeneveld   (501) staff       (20)       13 2024-05-23 14:26:56.000000 asp_selftest-0.0.6/src/asp_selftest.egg-info/top_level.txt
+drwxr-xr-x   0 erikgroeneveld   (501) staff       (20)        0 2024-05-27 09:47:49.079930 asp_selftest-0.0.7/
+-rw-r--r--   0 erikgroeneveld   (501) staff       (20)    35149 2024-02-19 08:25:44.000000 asp_selftest-0.0.7/LICENSE
+-rw-r--r--   0 erikgroeneveld   (501) staff       (20)       20 2024-04-25 13:29:32.000000 asp_selftest-0.0.7/MANIFEST.in
+-rw-r--r--   0 erikgroeneveld   (501) staff       (20)     3490 2024-05-27 09:47:49.079704 asp_selftest-0.0.7/PKG-INFO
+-rw-r--r--   0 erikgroeneveld   (501) staff       (20)     2878 2024-04-25 15:02:28.000000 asp_selftest-0.0.7/README.md
+-rw-r--r--   0 erikgroeneveld   (501) staff       (20)      789 2024-05-27 09:46:52.000000 asp_selftest-0.0.7/pyproject.toml
+-rw-r--r--   0 erikgroeneveld   (501) staff       (20)       38 2024-05-27 09:47:49.079975 asp_selftest-0.0.7/setup.cfg
+drwxr-xr-x   0 erikgroeneveld   (501) staff       (20)        0 2024-05-27 09:47:49.077468 asp_selftest-0.0.7/src/
+drwxr-xr-x   0 erikgroeneveld   (501) staff       (20)        0 2024-05-27 09:47:49.078460 asp_selftest-0.0.7/src/asp_selftest/
+-rw-r--r--   0 erikgroeneveld   (501) staff       (20)      727 2024-05-08 16:37:36.000000 asp_selftest-0.0.7/src/asp_selftest/__init__.py
+-rw-r--r--   0 erikgroeneveld   (501) staff       (20)      629 2024-05-27 09:44:58.000000 asp_selftest-0.0.7/src/asp_selftest/example.lp
+-rw-r--r--   0 erikgroeneveld   (501) staff       (20)     1277 2024-05-27 08:26:50.000000 asp_selftest-0.0.7/src/asp_selftest/queens.lp
+-rwxr-xr-x   0 erikgroeneveld   (501) staff       (20)    10086 2024-05-27 09:37:55.000000 asp_selftest-0.0.7/src/asp_selftest/runasptests.py
+drwxr-xr-x   0 erikgroeneveld   (501) staff       (20)        0 2024-05-27 09:47:49.079464 asp_selftest-0.0.7/src/asp_selftest.egg-info/
+-rw-r--r--   0 erikgroeneveld   (501) staff       (20)     3490 2024-05-27 09:47:49.000000 asp_selftest-0.0.7/src/asp_selftest.egg-info/PKG-INFO
+-rw-r--r--   0 erikgroeneveld   (501) staff       (20)      363 2024-05-27 09:47:49.000000 asp_selftest-0.0.7/src/asp_selftest.egg-info/SOURCES.txt
+-rw-r--r--   0 erikgroeneveld   (501) staff       (20)        1 2024-05-27 09:47:49.000000 asp_selftest-0.0.7/src/asp_selftest.egg-info/dependency_links.txt
+-rw-r--r--   0 erikgroeneveld   (501) staff       (20)       55 2024-05-27 09:47:49.000000 asp_selftest-0.0.7/src/asp_selftest.egg-info/entry_points.txt
+-rw-r--r--   0 erikgroeneveld   (501) staff       (20)       13 2024-05-27 09:47:49.000000 asp_selftest-0.0.7/src/asp_selftest.egg-info/top_level.txt
```

### Comparing `asp_selftest-0.0.6/LICENSE` & `asp_selftest-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `asp_selftest-0.0.6/PKG-INFO` & `asp_selftest-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asp_selftest
-Version: 0.0.6
+Version: 0.0.7
 Summary: A tool for running in-source unittests for Anwer Set Programming (ASP)
 Author-email: Erik Groeneveld <ejgroene@ieee.org>
 Project-URL: Homepage, https://github.com/ejgroene/asp-selftest
 Project-URL: Issues, https://github.com/ejgroene/asp-selftest/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: ASP
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```

### Comparing `asp_selftest-0.0.6/README.md` & `asp_selftest-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `asp_selftest-0.0.6/pyproject.toml` & `asp_selftest-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "asp_selftest"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Erik Groeneveld", email="ejgroene@ieee.org" },
 ]
 description = "A tool for running in-source unittests for Anwer Set Programming (ASP)"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `asp_selftest-0.0.6/src/asp_selftest/__init__.py` & `asp_selftest-0.0.7/src/asp_selftest/__init__.py`

 * *Files identical despite different names*

### Comparing `asp_selftest-0.0.6/src/asp_selftest/example.lp` & `asp_selftest-0.0.7/src/asp_selftest/example.lp`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #program step(n).
 { fix(A) : A=1..n } = 1.
 
 #program teststep(step(10)).
-assert(@all(select_one)) :- { fix(X) : X=1..10 } = 1.
+assert(@all(select_one(Y))) :- Y=1..10,  { fix(X) : X=1..10 } = 1.  % not sure if this is a good test; don't think so; something got lost during refactoring
 assert(@models(10)).
 
 
 #program define_inputs().
 input(input_a, 1, position(4), "Input A").       % full definition
 input(input_b, 2, position(3), "Input B").       % full definition
 input(Id)  :-  input(Id, _, _, _).               % shortcut for easier testing
```

### Comparing `asp_selftest-0.0.6/src/asp_selftest/queens.lp` & `asp_selftest-0.0.7/src/asp_selftest/queens.lp`

 * *Files identical despite different names*

### Comparing `asp_selftest-0.0.6/src/asp_selftest/runasptests.py` & `asp_selftest-0.0.7/src/asp_selftest/runasptests.py`

 * *Files 4% similar despite different names*

```diff
@@ -164,15 +164,15 @@
     """ read all the #program parts and register their dependencies """
     lines = asp_code.splitlines()
     programs = {'base': []}
     for i, line in enumerate(lines):
         if line.strip().startswith('#program'):
             name, dependencies = parse_signature(line.split('#program')[1].strip()[:-1])
             if name in programs:
-                raise Exception(f"Duplicate test name: {name!r}")
+                raise Exception(f"Duplicate program name: {name!r}")
             programs[name] = dependencies
             # rewrite into valid ASP (turn functions into plain terms)
             lines[i] = f"#program {name}({','.join(dep[0] for dep in dependencies)})."
     return lines, programs
 
 
 @test
@@ -200,38 +200,41 @@
 def read_function_args():
     lines, programs = read_programs(""" fact. \n#program a(x). \n #program b(a(42)). """)
     test.eq([" fact. ", "#program a(x).", "#program b(a)."], lines)  # 42 removed
     test.eq({'base': [], 'a': [('x', [])], 'b': [('a', [42])]}, programs)
 
 
 @test
-def check_for_duplicate_test(raises:(Exception, "Duplicate test name: 'test_a'")):
+def check_for_duplicate_test(raises:(Exception, "Duplicate program name: 'test_a'")):
     read_programs(""" #program test_a. \n #program test_a. """)
 
 
 
 def run_tests(lines, programs):
-    for name in programs:
-        if name.startswith('test'):
+    for prog_name, dependencies in programs.items():
+        if prog_name.startswith('test'):
             global current_tester
             tester = current_tester = Tester()
             control = clingo.Control(['0'])
             control.add('\n'.join(lines))
 
-            def prog_with_args(name):
-                dependencies = programs[name]
-                yield name, [clingo.Number(1) for _ in dependencies]
-                for dep_name, actual_args in dependencies:
-                    yield from prog_with_args(dep_name)
+            def prog_with_dependencies(name, dependencies):
+                yield name, [clingo.Number(42) for _ in dependencies]
+                for dep, args in dependencies:
+                    formal_args = programs.get(dep, [])
+                    formal_names = list(a[0] for a in formal_args)
+                    if len(args) != len(formal_names):
+                        raise Exception(f"Argument mismatch in {prog_name!r} for dependency {dep!r}. Required: {formal_names}, given: {args}.")
+                    yield dep, [clingo.Number(a) for a in args]
 
-            to_ground = list(prog_with_args(name))
+            to_ground = list(prog_with_dependencies(prog_name, dependencies))
             control.register_observer(tester)
             control.ground(to_ground, context = tester)
             control.solve(on_model = tester.on_model)
-            yield name, tester.report()
+            yield prog_name, tester.report()
 
 
 
 def parse_and_run_tests(asp_code):
     lines, programs = read_programs(asp_code)
     return run_tests(lines, programs)
 
@@ -264,30 +267,48 @@
 
 
 @test
 def dependencies():
     t = parse_and_run_tests("""
         base_fact.
 
-        #program one(base).
+        #program one(b).
         one_fact.
 
         #program test_base(base).
         assert(@all("base_facts")) :- base_fact.
         assert(@models(1)).
 
-        #program test_one(one).
+        #program test_one(base, one(1)).
         assert(@all("one includes base")) :- base_fact, one_fact.
         assert(@models(1)).
      """)
     test.eq(('test_base', {'asserts': {'assert("base_facts")'       , 'assert(models(1))'}, 'models': 1}), next(t))
     test.eq(('test_one' , {'asserts': {'assert("one includes base")', 'assert(models(1))'}, 'models': 1}), next(t))
 
 
 @test
+def pass_constant_values():
+    t = parse_and_run_tests("""
+        #program fact_maker(n).
+        fact(n).
+
+        #program test_fact_2(fact_maker(2)).
+        assert(@all(two)) :- fact(2).
+        assert(@models(1)).
+
+        #program test_fact_4(fact_maker(4)).
+        assert(@all(four)) :- fact(4).
+        assert(@models(1)).
+     """)
+    test.eq(('test_fact_2', {'asserts': {'assert(two)', 'assert(models(1))'}, 'models': 1}), next(t))
+    test.eq(('test_fact_4', {'asserts': {'assert(four)', 'assert(models(1))'}, 'models': 1}), next(t))
+
+
+@test
 def warn_for_disjunctions():
     t = parse_and_run_tests("""
         time(0; 1).
         #program test_base(base).
         assert(@all(time_exists)) :- time(T).
         assert(@models(1)).
      """)
```

### Comparing `asp_selftest-0.0.6/src/asp_selftest.egg-info/PKG-INFO` & `asp_selftest-0.0.7/src/asp_selftest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asp_selftest
-Version: 0.0.6
+Version: 0.0.7
 Summary: A tool for running in-source unittests for Anwer Set Programming (ASP)
 Author-email: Erik Groeneveld <ejgroene@ieee.org>
 Project-URL: Homepage, https://github.com/ejgroene/asp-selftest
 Project-URL: Issues, https://github.com/ejgroene/asp-selftest/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: ASP
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```

