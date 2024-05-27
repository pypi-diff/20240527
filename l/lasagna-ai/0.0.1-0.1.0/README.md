# Comparing `tmp/lasagna_ai-0.0.1.tar.gz` & `tmp/lasagna_ai-0.1.0.tar.gz`

## Comparing `lasagna_ai-0.0.1.tar` & `lasagna_ai-0.1.0.tar`

### file list

```diff
@@ -1,11 +1,20 @@
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 lasagna_ai-0.0.1/.github/workflows/publish.yml
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 lasagna_ai-0.0.1/.github/workflows/test.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 lasagna_ai-0.0.1/src/lasagna/__about__.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 lasagna_ai-0.0.1/src/lasagna/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lasagna_ai-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 lasagna_ai-0.0.1/tests/test_thing.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 lasagna_ai-0.0.1/.gitignore
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 lasagna_ai-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 lasagna_ai-0.0.1/README.md
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 lasagna_ai-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 lasagna_ai-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 lasagna_ai-0.1.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 lasagna_ai-0.1.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 lasagna_ai-0.1.0/src/lasagna/__init__.py
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 lasagna_ai-0.1.0/src/lasagna/agent_runner.py
+-rw-r--r--   0        0        0    18142 2020-02-02 00:00:00.000000 lasagna_ai-0.1.0/src/lasagna/lasagna_openai.py
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 lasagna_ai-0.1.0/src/lasagna/registrar.py
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 lasagna_ai-0.1.0/src/lasagna/stream.py
+-rw-r--r--   0        0        0     3673 2020-02-02 00:00:00.000000 lasagna_ai-0.1.0/src/lasagna/types.py
+-rw-r--r--   0        0        0     3400 2020-02-02 00:00:00.000000 lasagna_ai-0.1.0/src/lasagna/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lasagna_ai-0.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     3025 2020-02-02 00:00:00.000000 lasagna_ai-0.1.0/tests/test_agent_runner.py
+-rw-r--r--   0        0        0    38083 2020-02-02 00:00:00.000000 lasagna_ai-0.1.0/tests/test_lasagna_openai.py
+-rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 lasagna_ai-0.1.0/tests/test_registrar.py
+-rw-r--r--   0        0        0     3542 2020-02-02 00:00:00.000000 lasagna_ai-0.1.0/tests/test_stream.py
+-rw-r--r--   0        0        0     8540 2020-02-02 00:00:00.000000 lasagna_ai-0.1.0/tests/test_util.py
+-rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 lasagna_ai-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 lasagna_ai-0.1.0/LICENSE.txt
+-rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 lasagna_ai-0.1.0/README.md
+-rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 lasagna_ai-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 lasagna_ai-0.1.0/PKG-INFO
```

### Comparing `lasagna_ai-0.0.1/.github/workflows/publish.yml` & `lasagna_ai-0.1.0/.github/workflows/publish.yml`

 * *Files 21% similar despite different names*

```diff
@@ -13,18 +13,24 @@
     name: Publish to PyPI
     runs-on: ubuntu-latest
 
     steps:
     - uses: actions/checkout@v4
 
     - name: Install Hatch
-      run: pip install --upgrade hatch
+      run: |
+        pip install --upgrade hatch
 
-    - name: Final Test
-      run: hatch test --python 3.8
+    - name: Check type correctness
+      run: |
+        hatch run types:check
+
+    - name: Run tests
+      run: |
+        hatch test --all --cover --randomize
 
     - name: Build
       run: hatch build
 
     - name: Publish
       env:
         HATCH_INDEX_USER: ${{ secrets.HATCH_INDEX_USER }}
```

### Comparing `lasagna_ai-0.0.1/.gitignore` & `lasagna_ai-0.1.0/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -73,14 +73,16 @@
 
 # PyBuilder
 .pybuilder/
 target/
 
 # Jupyter Notebook
 .ipynb_checkpoints
+.virtual_documents
+.Trash-0
 
 # IPython
 profile_default/
 ipython_config.py
 
 # pyenv
 #   For a library or package, you might want to ignore these files since the code is
```

### Comparing `lasagna_ai-0.0.1/LICENSE.txt` & `lasagna_ai-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

