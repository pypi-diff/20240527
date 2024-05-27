# Comparing `tmp/ondivi-0.1.0.tar.gz` & `tmp/ondivi-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ondivi-0.1.0.tar", max compression
+gzip compressed data, was "ondivi-0.2.1.tar", max compression
```

## Comparing `ondivi-0.1.0.tar` & `ondivi-0.2.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1109 2024-05-16 12:50:20.031251 ondivi-0.1.0/LICENSE
--rw-r--r--   0        0        0      793 2024-05-16 12:50:20.031251 ondivi-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-05-16 12:50:20.031251 ondivi-0.1.0/ondivi/__init__.py
--rw-r--r--   0        0        0     3202 2024-05-16 12:50:20.031251 ondivi-0.1.0/ondivi/__main__.py
--rw-r--r--   0        0        0     2367 2024-05-16 12:50:20.759257 ondivi-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1277 1970-01-01 00:00:00.000000 ondivi-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1109 2024-05-27 12:11:26.056879 ondivi-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1624 2024-05-27 12:11:26.056879 ondivi-0.2.1/README.md
+-rw-r--r--   0        0        0      151 2024-05-27 12:11:26.056879 ondivi-0.2.1/ondivi/__init__.py
+-rw-r--r--   0        0        0     4448 2024-05-27 12:11:26.056879 ondivi-0.2.1/ondivi/__main__.py
+-rw-r--r--   0        0        0     3770 2024-05-27 12:11:26.368882 ondivi-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2108 1970-01-01 00:00:00.000000 ondivi-0.2.1/PKG-INFO
```

### Comparing `ondivi-0.1.0/LICENSE` & `ondivi-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ondivi-0.1.0/ondivi/__main__.py` & `ondivi-0.2.1/ondivi/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,24 +16,32 @@
 # EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
 # MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
 # IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
 # DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
 # OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE
 # OR OTHER DEALINGS IN THE SOFTWARE.
 
+"""Ondivi (Only diff violations).
+
+Python script filtering coding violations, identified by static analysis,
+only for changed lines in a Git repo.
+"""
+
+import argparse
+import sys
 from contextlib import suppress
 
 from git import Repo
 
 Diff = str
 FileName = str
 
 
-def define_changed_lines(diff: Diff) -> dict[FileName, list[int]]:
-    """Поиск измененных строк в файлах.
+def define_changed_lines(diff: Diff) -> dict[FileName, list[int]]:  # noqa: WPS210. TODO: too many local variables
+    """Define changed lines in file.
 
     :param diff: Diff
     :return: dict[FileName, list[int]]
     """
     res: dict[FileName, list[int]] = {}
     current_file = ''
     for line in diff.splitlines():
@@ -42,52 +50,87 @@
             res[current_file] = []
         elif line.startswith('@@'):
             splitted_line = line.split('@@')[1].strip()
             added_lines = splitted_line.split('+')[1]
             start_line = int(
                 added_lines.split(',')[0],
             )
-            num_lines = 0 if ',' not in added_lines else int(added_lines.split(',')[1]) - 1
+            if ',' not in added_lines:  # noqa: SIM108. Too complexity line
+                num_lines = 0
+            else:
+                num_lines = int(added_lines.split(',')[1]) - 1
             res[current_file].extend(list(range(
                 start_line, start_line + num_lines + 1,
             )))
     return res
 
 
-def filter_out_violations(changed_lines: dict[FileName, list[int]], violations: list[str]) -> list[str]:
+def filter_out_violations(
+    changed_lines: dict[FileName, list[int]],
+    violations: list[str],
+) -> list[str]:
+    """Collect target violations.
+
+    :param changed_lines: dict[FileName, list[int]], violations: list[str]
+    :param violations: list[str]
+    :return: list[str]
+    """
     res = []
     for violation in violations:
         with suppress(ValueError, IndexError):
             filename = violation.split(':')[0]
             line = int(violation.split(':')[1])
             if filename not in changed_lines:
                 continue
             if line not in changed_lines[filename]:
                 continue
         res.append(violation)
     return res
 
 
 def controller(diff: Diff, violations: list[str]) -> list[str]:
+    """Entrypoint.
+
+    :param diff: Diff
+    :param violations: list[str]
+    :return: list[str]
+    """
     changed_lines = define_changed_lines(diff)
     return filter_out_violations(changed_lines, violations)
 
 
 def main() -> None:
-    a = 'not empty'
-    violations = []
-    while a:
-        try:
-            a = input()
-            violations.append(a)
-        except EOFError:  # noqa: PERF203
-            break
-    print('\n'.join(  # noqa: T201
+    """Entrypoint."""
+    parser = argparse.ArgumentParser(
+        description='\n'.join([
+            'Ondivi (Only diff violations).\n',
+            'Python script filtering coding violations, identified by static analysis,',
+            'only for changed lines in a Git repo.\n',
+            'Usage example:\n',
+            'flake8 script.py | ondivi',
+        ]),
+        formatter_class=argparse.RawTextHelpFormatter,
+    )
+    parser.add_argument(
+        '--baseline',
+        dest='baseline',
+        type=str,
+        default='master',
+        help=' '.join([
+            'Commit or branch which will contain legacy code.',
+            'Program filter out violations on baseline',
+            '(default: "master")',
+        ]),
+    )
+    args = parser.parse_args()
+    violations = sys.stdin.read().strip().splitlines()
+    sys.stdout.write('\n'.join(
         controller(
-            Repo('.').git.diff('--unified=0', 'origin/master..HEAD'),
+            Repo('.').git.diff('--unified=0', args.baseline),
             violations,
         ),
     ))
+    sys.stdout.write('\n')
 
 
 if __name__ == '__main__':
     main()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

