# Comparing `tmp/boolgen-1.0.0.tar.gz` & `tmp/boolgen-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boolgen-1.0.0.tar", last modified: Sun May 26 19:03:07 2024, max compression
+gzip compressed data, was "boolgen-1.1.0.tar", last modified: Mon May 27 15:15:10 2024, max compression
```

## Comparing `boolgen-1.0.0.tar` & `boolgen-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 sderle     (501) staff       (20)        0 2024-05-26 19:03:07.862265 boolgen-1.0.0/
--rw-r--r--   0 sderle     (501) staff       (20)     1061 2024-05-25 15:43:25.000000 boolgen-1.0.0/LICENSE.md
--rw-r--r--   0 sderle     (501) staff       (20)     2201 2024-05-26 19:03:07.861918 boolgen-1.0.0/PKG-INFO
--rw-r--r--   0 sderle     (501) staff       (20)     1725 2024-05-26 18:46:34.000000 boolgen-1.0.0/README.md
-drwxr-xr-x   0 sderle     (501) staff       (20)        0 2024-05-26 19:03:07.859098 boolgen-1.0.0/boolgen/
--rw-r--r--   0 sderle     (501) staff       (20)     6985 2024-05-26 18:35:00.000000 boolgen-1.0.0/boolgen/__init__.py
-drwxr-xr-x   0 sderle     (501) staff       (20)        0 2024-05-26 19:03:07.861555 boolgen-1.0.0/boolgen.egg-info/
--rw-r--r--   0 sderle     (501) staff       (20)     2201 2024-05-26 19:03:07.000000 boolgen-1.0.0/boolgen.egg-info/PKG-INFO
--rw-r--r--   0 sderle     (501) staff       (20)      229 2024-05-26 19:03:07.000000 boolgen-1.0.0/boolgen.egg-info/SOURCES.txt
--rw-r--r--   0 sderle     (501) staff       (20)        1 2024-05-26 19:03:07.000000 boolgen-1.0.0/boolgen.egg-info/dependency_links.txt
--rw-r--r--   0 sderle     (501) staff       (20)       41 2024-05-26 19:03:07.000000 boolgen-1.0.0/boolgen.egg-info/entry_points.txt
--rw-r--r--   0 sderle     (501) staff       (20)        8 2024-05-26 19:03:07.000000 boolgen-1.0.0/boolgen.egg-info/top_level.txt
--rw-r--r--   0 sderle     (501) staff       (20)       38 2024-05-26 19:03:07.862311 boolgen-1.0.0/setup.cfg
--rw-r--r--   0 sderle     (501) staff       (20)      734 2024-05-26 18:58:38.000000 boolgen-1.0.0/setup.py
-drwxr-xr-x   0 sderle     (501) staff       (20)        0 2024-05-26 19:03:07.861055 boolgen-1.0.0/tests/
--rw-r--r--   0 sderle     (501) staff       (20)     5644 2024-05-26 18:29:19.000000 boolgen-1.0.0/tests/test_boolgen.py
+drwxr-xr-x   0 sderle     (501) staff       (20)        0 2024-05-27 15:15:10.407004 boolgen-1.1.0/
+-rw-r--r--   0 sderle     (501) staff       (20)     1061 2024-05-25 15:43:25.000000 boolgen-1.1.0/LICENSE.md
+-rw-r--r--   0 sderle     (501) staff       (20)     2563 2024-05-27 15:15:10.406577 boolgen-1.1.0/PKG-INFO
+-rw-r--r--   0 sderle     (501) staff       (20)     2087 2024-05-27 14:22:24.000000 boolgen-1.1.0/README.md
+drwxr-xr-x   0 sderle     (501) staff       (20)        0 2024-05-27 15:15:10.403755 boolgen-1.1.0/boolgen/
+-rw-r--r--   0 sderle     (501) staff       (20)     6675 2024-05-27 14:18:55.000000 boolgen-1.1.0/boolgen/__init__.py
+drwxr-xr-x   0 sderle     (501) staff       (20)        0 2024-05-27 15:15:10.406149 boolgen-1.1.0/boolgen.egg-info/
+-rw-r--r--   0 sderle     (501) staff       (20)     2563 2024-05-27 15:15:10.000000 boolgen-1.1.0/boolgen.egg-info/PKG-INFO
+-rw-r--r--   0 sderle     (501) staff       (20)      229 2024-05-27 15:15:10.000000 boolgen-1.1.0/boolgen.egg-info/SOURCES.txt
+-rw-r--r--   0 sderle     (501) staff       (20)        1 2024-05-27 15:15:10.000000 boolgen-1.1.0/boolgen.egg-info/dependency_links.txt
+-rw-r--r--   0 sderle     (501) staff       (20)       41 2024-05-27 15:15:10.000000 boolgen-1.1.0/boolgen.egg-info/entry_points.txt
+-rw-r--r--   0 sderle     (501) staff       (20)        8 2024-05-27 15:15:10.000000 boolgen-1.1.0/boolgen.egg-info/top_level.txt
+-rw-r--r--   0 sderle     (501) staff       (20)       38 2024-05-27 15:15:10.407060 boolgen-1.1.0/setup.cfg
+-rw-r--r--   0 sderle     (501) staff       (20)      734 2024-05-27 15:13:45.000000 boolgen-1.1.0/setup.py
+drwxr-xr-x   0 sderle     (501) staff       (20)        0 2024-05-27 15:15:10.405652 boolgen-1.1.0/tests/
+-rw-r--r--   0 sderle     (501) staff       (20)     6031 2024-05-27 14:20:15.000000 boolgen-1.1.0/tests/test_boolgen.py
```

### Comparing `boolgen-1.0.0/LICENSE.md` & `boolgen-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `boolgen-1.0.0/PKG-INFO` & `boolgen-1.1.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,16 @@
-Metadata-Version: 2.1
-Name: boolgen
-Version: 1.0.0
-Summary: A library for generating and simplifying Boolean expressions from truth tables
-Home-page: https://github.com/schuyler/boolgen
-Author: Schuyler Erle
-Author-email: schuyler@nocat.net
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 # boolgen
 
 `boolgen` is a Python library and command-line tool for generating and
 simplifying Boolean expressions from truth tables. 
 
-The library implenents a version of the [Quine-McCluskey
+The library implements a version of the [Quine-McCluskey
 method](https://en.wikipedia.org/wiki/Quine%E2%80%93McCluskey_algorithm) to
-perform the simplification. 
+perform the simplification. I created it to help with [designing digital logic
+circuits](https://github.com/SebLague/Digital-Logic-Sim) from truth tables.
 
 ## Installation
 
 To install `boolgen`, use pip:
 
 ```bash
 pip install boolgen
@@ -48,33 +35,34 @@
 `STDIN`.
 
 ### Example Input File
 
 Create a file named `input.txt` with the following content:
 
 ```
-A B C Output1 Output2
+A B C D= E=
 0 0 0 0 1
 0 0 1 1 0
 0 1 0 1 0
 1 0 0 1 0
 1 1 1 0 1
 ```
 
 Input and output variables can be identified with any alphanumeric string
-(including underscores). Output variables are identified by the
-case-insensitive prefix `out`.
+(including underscores). Output variables are identified by a pre- or postfix
+'='. If no output variable is explicitly declared, the last column in the table
+is assumed to be the output.
 
 ### Output
 
 `boolgen` will output the simplified Boolean expressions for each output variable in the truth table.
 
 ```
-Output1 = A | B & ~C
-Output2 = ~A & ~B & ~C | A & B & C
+D = A | B & ~C
+E = ~A & ~B & ~C | A & B & C
 ```
 
 In degenerate cases, an output variable might be set to `0` or `1`.
 
 ## Library
 
 You can also `import boolgen` into your own project. See the function
@@ -84,7 +72,11 @@
 
 Contributions are welcome! Please fork the repository and submit pull requests.
 
 ## License
 
 This project is licensed under the MIT License. See [LICENSE.md](LICENSE.md)
 for details.
+
+TBQH I used ChatGPT liberally when creating this module, so if you find your
+own code in here, please let me know so I can remove it or else attribute you
+properly.
```

### Comparing `boolgen-1.0.0/boolgen/__init__.py` & `boolgen-1.1.0/boolgen/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,24 +10,33 @@
 def parse_input(input_string: str) -> Tuple[List[str], List[str], List[List[int]]]:
     """
     Parse the input data into variables and truth table.
 
     :param input_data: A string containing the input data
     :return: A tuple containing the list of input variables, list of output variables, and the truth table
     """
+
+    def is_output_var(v):
+        return bool(re.search(r'^(?:out|=)|=$', v, re.I))
+
     # Split the input string by non-alphanumeric characters
-    rows = [re.split(r'\W+', row.strip()) for row in input_string.strip().split('\n')]
+    rows = [re.split(r'(?!=)\W+', row.strip()) for row in input_string.strip().split('\n')]
     
     # Extract the header (variables) and the rest of the rows (values)
     variables = rows[0]
     truth_table = [list(map(int, row)) for row in rows[1:]]
     
-    # Determine the number of input variables and output variables
-    input_vars = [var for var in variables if not var.lower().startswith('out')]
-    output_vars = [var for var in variables if var.lower().startswith('out')]
+    # Determine the input variables and output variables
+    input_vars = [var for var in variables if not is_output_var(var)]
+    output_vars = [var.replace('=', '') for var in variables if is_output_var(var)]
+
+    # If no output variables were explicitly declared using pre/postfix '=',
+    # assume that the last column is meant to be an output.
+    if not output_vars:
+        output_vars.append(input_vars.pop())
     
     return input_vars, output_vars, truth_table
 
 # Helper function to convert minterms to binary format
 def minterm_to_binary(minterm, num_vars):
     return format(minterm, f'0{num_vars}b')
 
@@ -80,56 +89,43 @@
                     prime_implicants.add(term)
 
         if not any(new_groups.values()):
             break
         groups = new_groups
 
     # Essential Prime Implicant Reduction
-    def find_essential_prime_implicants(prime_implicants, minterms):
-        prime_implicant_chart = {term: set(term_to_indices(term)) for term in prime_implicants}
-        minterm_chart = {minterm: [] for minterm in minterms}
-        for term, indices in prime_implicant_chart.items():
-            for index in indices:
-                if index in minterm_chart:
-                    minterm_chart[index].append(term)
-
-        essential_prime_implicants = set()
-        while minterm_chart:
-            for minterm, terms in minterm_chart.items():
-                if len(terms) == 1:
-                    essential_prime_implicant = terms[0]
-                    break
+    prime_implicant_chart = {term: set(term_to_indices(term)) for term in prime_implicants}
+    minterm_chart = {minterm: [] for minterm in minterms}
+    for term, indices in prime_implicant_chart.items():
+        for index in indices:
+            if index in minterm_chart:
+                minterm_chart[index].append(term)
+
+    essential_prime_implicants = set()
+    while minterm_chart:
+        for minterm, terms in minterm_chart.items():
+            if len(terms) == 1:
+                essential_prime_implicant = terms[0]
+                break
+        else:
+            essential_prime_implicant = max(prime_implicant_chart, key=lambda t: len(prime_implicant_chart[t]))
+
+        essential_prime_implicants.add(essential_prime_implicant)
+        covered_minterms = prime_implicant_chart.pop(essential_prime_implicant)
+        minterm_chart = {m: terms for m, terms in minterm_chart.items() if m not in covered_minterms}
+
+        for minterm, terms in minterm_chart.items():
+            terms = [t for t in terms if t != essential_prime_implicant]
+            if terms:
+                minterm_chart[minterm] = terms
             else:
-                essential_prime_implicant = max(prime_implicant_chart, key=lambda t: len(prime_implicant_chart[t]))
+                del minterm_chart[minterm]
+
+    return essential_prime_implicants
 
-            essential_prime_implicants.add(essential_prime_implicant)
-            covered_minterms = prime_implicant_chart.pop(essential_prime_implicant)
-            minterm_chart = {m: terms for m, terms in minterm_chart.items() if m not in covered_minterms}
-
-            for minterm, terms in minterm_chart.items():
-                terms = [t for t in terms if t != essential_prime_implicant]
-                if terms:
-                    minterm_chart[minterm] = terms
-                else:
-                    del minterm_chart[minterm]
-
-        return essential_prime_implicants
-
-    prime_implicants = find_essential_prime_implicants(prime_implicants, minterms)
-    return prime_implicants
-
-# Function to convert binary terms to Boolean expression
-def binary_to_expression(binary, variables):
-    expression = []
-    for bit, var in zip(binary, variables):
-        if bit == '1':
-            expression.append(var)
-        elif bit == '0':
-            expression.append(f'~{var}')
-    return ' & '.join(expression)
 
 # Function to simplify Boolean expressions
 def simplify_expression(input_vars: List[str], truth_table: List[List[int]], output_index: int) -> str:
     """
     Simplify the boolean expression based on the truth table.
 
     :param input_vars: List of input variable names
@@ -151,15 +147,15 @@
     def term_to_expression(term):
         parts = []
         for var, bit in zip(input_vars, term):
             if bit == '0':
                 parts.append(f"~{var}")
             elif bit == '1':
                 parts.append(var)
-        return ' & '.join(parts)
+        return ' & '.join(sorted(parts))
 
     expressions = [term_to_expression(term) for term in prime_implicants]
     return ' | '.join(sorted(expressions))
 
 
 # Main function
 def evaluate_table(input_string):
```

### Comparing `boolgen-1.0.0/boolgen.egg-info/PKG-INFO` & `boolgen-1.1.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boolgen
-Version: 1.0.0
+Version: 1.1.0
 Summary: A library for generating and simplifying Boolean expressions from truth tables
 Home-page: https://github.com/schuyler/boolgen
 Author: Schuyler Erle
 Author-email: schuyler@nocat.net
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,17 +13,18 @@
 License-File: LICENSE.md
 
 # boolgen
 
 `boolgen` is a Python library and command-line tool for generating and
 simplifying Boolean expressions from truth tables. 
 
-The library implenents a version of the [Quine-McCluskey
+The library implements a version of the [Quine-McCluskey
 method](https://en.wikipedia.org/wiki/Quine%E2%80%93McCluskey_algorithm) to
-perform the simplification. 
+perform the simplification. I created it to help with [designing digital logic
+circuits](https://github.com/SebLague/Digital-Logic-Sim) from truth tables.
 
 ## Installation
 
 To install `boolgen`, use pip:
 
 ```bash
 pip install boolgen
@@ -48,33 +49,34 @@
 `STDIN`.
 
 ### Example Input File
 
 Create a file named `input.txt` with the following content:
 
 ```
-A B C Output1 Output2
+A B C D= E=
 0 0 0 0 1
 0 0 1 1 0
 0 1 0 1 0
 1 0 0 1 0
 1 1 1 0 1
 ```
 
 Input and output variables can be identified with any alphanumeric string
-(including underscores). Output variables are identified by the
-case-insensitive prefix `out`.
+(including underscores). Output variables are identified by a pre- or postfix
+'='. If no output variable is explicitly declared, the last column in the table
+is assumed to be the output.
 
 ### Output
 
 `boolgen` will output the simplified Boolean expressions for each output variable in the truth table.
 
 ```
-Output1 = A | B & ~C
-Output2 = ~A & ~B & ~C | A & B & C
+D = A | B & ~C
+E = ~A & ~B & ~C | A & B & C
 ```
 
 In degenerate cases, an output variable might be set to `0` or `1`.
 
 ## Library
 
 You can also `import boolgen` into your own project. See the function
@@ -84,7 +86,11 @@
 
 Contributions are welcome! Please fork the repository and submit pull requests.
 
 ## License
 
 This project is licensed under the MIT License. See [LICENSE.md](LICENSE.md)
 for details.
+
+TBQH I used ChatGPT liberally when creating this module, so if you find your
+own code in here, please let me know so I can remove it or else attribute you
+properly.
```

### Comparing `boolgen-1.0.0/setup.py` & `boolgen-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='boolgen',
-    version='1.0.0',
+    version='1.1.0',
     packages=find_packages(),
     description='A library for generating and simplifying Boolean expressions from truth tables',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Schuyler Erle',
     author_email='schuyler@nocat.net',
     url='https://github.com/schuyler/boolgen',
```

### Comparing `boolgen-1.0.0/tests/test_boolgen.py` & `boolgen-1.1.0/tests/test_boolgen.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,52 +1,64 @@
 import unittest
 from boolgen import parse_input, simplify_expression
 
 class TestBoolgen(unittest.TestCase):
 
     def test_parse_input_single_output(self):
-        input_data = """A B C Output
+        input_data = """A B C D=
                         0 0 0 0
                         0 0 1 1
                         0 1 0 1
                         0 1 1 0
                         1 0 0 1
                         1 0 1 0
                         1 1 0 0
                         1 1 1 1"""
         input_vars, output_vars, truth_table = parse_input(input_data)
         expected_input_vars = ['A', 'B', 'C']
-        expected_output_vars = ['Output']
+        expected_output_vars = ['D']
         expected_truth_table = [
             [0, 0, 0, 0],
             [0, 0, 1, 1],
             [0, 1, 0, 1],
             [0, 1, 1, 0],
             [1, 0, 0, 1],
             [1, 0, 1, 0],
             [1, 1, 0, 0],
             [1, 1, 1, 1]
         ]
         self.assertEqual(input_vars, expected_input_vars)
         self.assertEqual(output_vars, expected_output_vars)
         self.assertEqual(truth_table, expected_truth_table)
 
+    def test_parse_input_implicit_output(self):
+        input_data = """A B
+                        0 0
+                        0 1
+                        1 0
+                        1 1"""
+        input_vars, output_vars, _ = parse_input(input_data)
+        expected_input_vars = ['A']
+        expected_output_vars = ['B']
+        self.assertEqual(input_vars, expected_input_vars)
+        self.assertEqual(output_vars, expected_output_vars)
+
     def test_parse_input_multiple_outputs(self):
-        input_data = """A B C Output1 Output2
+        input_data = """A B C D= E=
                         0 0 0 0 1
                         0 0 1 1 0
                         0 1 0 1 0
                         0 1 1 0 1
                         1 0 0 1 0
                         1 0 1 0 1
                         1 1 0 0 1
                         1 1 1 1 0"""
         input_vars, output_vars, truth_table = parse_input(input_data)
         expected_input_vars = ['A', 'B', 'C']
-        expected_output_vars = ['Output1', 'Output2']
+        expected_output_vars = ['D', 'E']
         expected_truth_table = [
             [0, 0, 0, 0, 1],
             [0, 0, 1, 1, 0],
             [0, 1, 0, 1, 0],
             [0, 1, 1, 0, 1],
             [1, 0, 0, 1, 0],
             [1, 0, 1, 0, 1],
@@ -54,54 +66,54 @@
             [1, 1, 1, 1, 0]
         ]
         self.assertEqual(input_vars, expected_input_vars)
         self.assertEqual(output_vars, expected_output_vars)
         self.assertEqual(truth_table, expected_truth_table)
 
     def test_simplify_expression_single_output(self):
-        input_data = """A B C Output
+        input_data = """A B C D=
                         0 0 0 0
                         0 0 1 1
                         0 1 0 1
                         0 1 1 0
                         1 0 0 1
                         1 0 1 0
                         1 1 0 0
                         1 1 1 1"""
         input_vars, output_vars, truth_table = parse_input(input_data)
         expression = simplify_expression(input_vars, truth_table, 0)
-        expected_expression = "~A & B & ~C | A & ~B & ~C | ~A & ~B & C | A & B & C"
+        expected_expression = "A & B & C | A & ~B & ~C | B & ~A & ~C | C & ~A & ~B"
         sorted_expected_expression = ' | '.join(sorted(expected_expression.split(' | ')))
 
         self.assertEqual(expression, sorted_expected_expression)
 
     def test_simplify_expression_multiple_outputs(self):
-        input_data = """A B C Output1 Output2
+        input_data = """A B C D= E=
                         0 0 0 0 1
                         0 0 1 1 0
                         0 1 0 1 0
                         0 1 1 0 1
                         1 0 0 1 0
                         1 0 1 0 1
                         1 1 0 0 1
                         1 1 1 1 0"""
         input_vars, output_vars, truth_table = parse_input(input_data)
         expression1 = simplify_expression(input_vars, truth_table, 0)
         expression2 = simplify_expression(input_vars, truth_table, 1)
 
-        expected_expression1 = "A & B & C | A & ~B & ~C | ~A & B & ~C | ~A & ~B & C"
-        expected_expression2 = "~A & ~B & ~C | A & B & ~C | ~A & B & C | A & ~B & C"
+        expected_expression1 = "A & B & C | A & ~B & ~C | B & ~A & ~C | C & ~A & ~B"
+        expected_expression2 = "A & B & ~C | A & C & ~B | B & C & ~A | ~A & ~B & ~C"
         sorted_expected_expression1 = ' | '.join(sorted(expected_expression1.split(' | ')))
         sorted_expected_expression2 = ' | '.join(sorted(expected_expression2.split(' | ')))
 
         self.assertEqual(expression1, sorted_expected_expression1)
         self.assertEqual(expression2, sorted_expected_expression2)
 
     def test_simplify_expression_all_zeros(self):
-        input_data = """A B C Output
+        input_data = """A B C D=
                         0 0 0 0
                         0 0 1 0
                         0 1 0 0
                         0 1 1 0
                         1 0 0 0
                         1 0 1 0
                         1 1 0 0
@@ -109,15 +121,15 @@
         input_vars, output_vars, truth_table = parse_input(input_data)
         expression = simplify_expression(input_vars, truth_table, 0)
         expected_expression = "0"
 
         self.assertEqual(expression, expected_expression)
 
     def test_simplify_expression_all_ones(self):
-        input_data = """A B C Output
+        input_data = """A B C D=
                         0 0 0 1
                         0 0 1 1
                         0 1 0 1
                         0 1 1 1
                         1 0 0 1
                         1 0 1 1
                         1 1 0 1
@@ -125,15 +137,15 @@
         input_vars, output_vars, truth_table = parse_input(input_data)
         expression = simplify_expression(input_vars, truth_table, 0)
         expected_expression = "1"
 
         self.assertEqual(expression, expected_expression)
 
     def test_simplify_expression_some_simplification(self):
-        input_data = """A B C Output
+        input_data = """A B C D=
                         0 0 0 0
                         0 0 1 1
                         0 1 0 1
                         0 1 1 1
                         1 0 0 0
                         1 0 1 1
                         1 1 0 1
```

