# Comparing `tmp/smt_portfolio-0.3.3.tar.gz` & `tmp/smt_portfolio-1.0.0.tar.gz`

## Comparing `smt_portfolio-0.3.3.tar` & `smt_portfolio-1.0.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rwxr-xr-x   0        0        0     4886 2020-02-02 00:00:00.000000 smt_portfolio-0.3.3/src/smt_portfolio/__init__.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 smt_portfolio-0.3.3/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 smt_portfolio-0.3.3/LICENSE
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 smt_portfolio-0.3.3/README.md
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 smt_portfolio-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 smt_portfolio-0.3.3/PKG-INFO
+-rwxr-xr-x   0        0        0     4086 2020-02-02 00:00:00.000000 smt_portfolio-1.0.0/src/smt_portfolio/__init__.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 smt_portfolio-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 smt_portfolio-1.0.0/LICENSE
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 smt_portfolio-1.0.0/README.md
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 smt_portfolio-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 smt_portfolio-1.0.0/PKG-INFO
```

### Comparing `smt_portfolio-0.3.3/src/smt_portfolio/__init__.py` & `smt_portfolio-1.0.0/src/smt_portfolio/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import subprocess
 from enum import Enum
 from typing import List
 from pathlib import Path
 from abc import ABC, abstractmethod
 
 
-__version__ = "0.3.3"
+__version__ = "1.0.0"
 
 
 class Result(Enum):
     SAT = 1
     UNSAT = 2
     UNKNOWN = 3
     TIMEOUT = 4
@@ -84,36 +84,14 @@
             return Result.UNSAT
         elif out == "" and "cvc5 interrupted by timeout" in err:
             return Result.TIMEOUT
         else:
             return Result.UNKNOWN
 
 
-class Vampire(Solver):
-    def run(self, input_file: Path) -> subprocess.Popen:
-        assert "smtlib2" in self.args
-        return subprocess.Popen(
-            shlex.split(f"vampire {self.args} {input_file}"),
-            stdin=subprocess.PIPE,
-            stdout=subprocess.PIPE,
-            stderr=subprocess.PIPE,
-            universal_newlines=True,
-            encoding="utf-8",
-            bufsize=1,
-        )
-
-    def parse_result(self, out: str, err: str) -> Result:
-        if out == "sat":
-            return Result.SAT
-        elif out == "unsat":
-            return Result.UNSAT
-        else:
-            return Result.UNKNOWN
-
-
 def clean(procs: List[subprocess.Popen]) -> None:
     for p in procs:
         p.kill()
 
 
 def run_all(solvers: List[Solver], input_file: Path) -> Result:
     procs = [s.run(input_file) for s in solvers]
@@ -149,24 +127,21 @@
         "--file",
         type=Path,
         required=False,
         help="Input SMT-LIB file. If `None`, it reads formula from stdin until `(check-sat)`",
     )
     parser.add_argument("--z3", type=str, help="Z3's command line arguments")
     parser.add_argument("--cvc5", type=str, help="CVC5's command line arguments")
-    parser.add_argument("--vampire", type=str, help="Vampire's command line arguments")
     args = parser.parse_args()
 
     solvers = []
     if args.z3:
         solvers.append(Z3(args.z3))
     if args.cvc5:
         solvers.append(CVC5(args.cvc5))
-    if args.vampire:
-        solvers.append(Vampire(args.vampire))
 
     if args.file:
         result = run_all(solvers, args.file)
     else:
         oup = tempfile.NamedTemporaryFile("wt")
         for line in sys.stdin:
             oup.write(line)
```

### Comparing `smt_portfolio-0.3.3/.gitignore` & `smt_portfolio-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `smt_portfolio-0.3.3/LICENSE` & `smt_portfolio-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `smt_portfolio-0.3.3/pyproject.toml` & `smt_portfolio-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
   "/.github",
   "/examples",
   "/scripts",
 ]
 
 [project]
 name = "smt-portfolio"
-version = "0.3.3"
+version = "1.0.0"
 authors = [
   { name="Kaiyu Yang", email="kaiyuy@caltech.edu" },
 ]
 description = "A simple wrapper to run multiple SMT solvers in parallel."
 keywords = ["SMT"]
 readme = "README.md"
 license = { file = "LICENSE" }
```

### Comparing `smt_portfolio-0.3.3/PKG-INFO` & `smt_portfolio-1.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: smt-portfolio
-Version: 0.3.3
+Version: 1.0.0
 Summary: A simple wrapper to run multiple SMT solvers in parallel.
 Project-URL: Homepage, https://github.com/yangky11/smt-portfolio
 Project-URL: Bug Tracker, https://github.com/yangky11/smt-portfolio/issues
 Author-email: Kaiyu Yang <kaiyuy@caltech.edu>
 License: MIT License
         
         Copyright (c) 2023 Kaiyu Yang
@@ -55,27 +55,26 @@
 [![PyPI](https://img.shields.io/pypi/v/smt-portfolio)](https://pypi.org/project/smt-portfolio/) [![GitHub license](https://img.shields.io/github/license/yangky11/smt-portfolio)](https://github.com/yangky11/smt-portfolio/blob/main/LICENSE) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) 
 
 ______________________________________________________________________
 
 
 ## Requirements
 
-* Z3
-* CVC5
-* Vampire
+* [Z3](https://github.com/Z3Prover/z3)
+* [CVC5](https://cvc5.github.io/)
 
 ## Installation
 
 ```bash
 pip install smt-portfolio
 ```
 
 ## Usage
 
 ```bash
 smt-portfolio --help
 ```
 
 ```bash
-smt-portfolio --file examples/ex1.smt2 --z3 "-smt2 -T:5" --cvc5 "--quiet --lang smt --dag-thresh=0 --enum-inst --tlimit 5000" --vampire "--input_syntax smtlib2 --output_mode smtcomp --time_limit 5"
-cat examples/ex1.smt2 | smt-portfolio --z3 "-smt2 -T:5" --cvc5 "--quiet --lang smt --dag-thresh=0 --enum-inst --tlimit 5000" --vampire "--input_syntax smtlib2 --output_mode smtcomp --time_limit 5"
+smt-portfolio --file examples/ex1.smt2 --z3 "-smt2 -T:5" --cvc5 "--quiet --lang smt --dag-thresh=0 --enum-inst --tlimit 5000"
+cat examples/ex1.smt2 | smt-portfolio --z3 "-smt2 -T:5" --cvc5 "--quiet --lang smt --dag-thresh=0 --enum-inst --tlimit 5000"
 ```
```

