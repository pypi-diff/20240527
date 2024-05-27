# Comparing `tmp/import_expression-1.1.5.tar.gz` & `tmp/import_expression-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "import_expression-1.1.5.tar", last modified: Sat May 25 01:19:31 2024, max compression
+gzip compressed data, was "import_expression-2.0.0.tar", last modified: Mon May 27 02:42:32 2024, max compression
```

## Comparing `import_expression-1.1.5.tar` & `import_expression-2.0.0.tar`

### file list

```diff
@@ -1,28 +1,23 @@
-drwxr-x---   0 user      (1000) user      (1000)        0 2024-05-25 01:19:31.776662 import_expression-1.1.5/
--rw-r-----   0 user      (1000) user      (1000)     4280 2024-05-25 01:05:33.000000 import_expression-1.1.5/LICENSE
--rw-r-----   0 user      (1000) user      (1000)     1112 2024-05-25 01:05:33.000000 import_expression-1.1.5/LICENSE-header
--rw-r-----   0 user      (1000) user      (1000)       47 2024-05-25 01:05:33.000000 import_expression-1.1.5/MANIFEST.in
--rw-r--r--   0 user      (1000) user      (1000)     3495 2024-05-25 01:19:31.773328 import_expression-1.1.5/PKG-INFO
--rw-r-----   0 user      (1000) user      (1000)     2946 2024-05-25 01:05:33.000000 import_expression-1.1.5/README.md
-drwxr-x---   0 user      (1000) user      (1000)        0 2024-05-25 01:19:31.773328 import_expression-1.1.5/import_expression/
--rwxr-x---   0 user      (1000) user      (1000)     5513 2024-05-25 01:05:33.000000 import_expression-1.1.5/import_expression/__init__.py
--rw-r-----   0 user      (1000) user      (1000)     9330 2024-05-25 01:05:33.000000 import_expression-1.1.5/import_expression/__main__.py
-drwxr-x---   0 user      (1000) user      (1000)        0 2024-05-25 01:19:31.773328 import_expression-1.1.5/import_expression/_codec/
--rw-r-----   0 user      (1000) user      (1000)     1663 2024-05-25 01:05:33.000000 import_expression-1.1.5/import_expression/_codec/__init__.py
--rw-r-----   0 user      (1000) user      (1000)      836 2024-05-25 01:05:33.000000 import_expression-1.1.5/import_expression/_codec/compat.py
--rw-r-----   0 user      (1000) user      (1000)      965 2024-05-25 01:05:33.000000 import_expression-1.1.5/import_expression/_main2.py
--rw-r-----   0 user      (1000) user      (1000)     7436 2024-05-25 01:05:33.000000 import_expression-1.1.5/import_expression/_parser.py
--rw-r-----   0 user      (1000) user      (1000)     4341 2024-05-25 01:05:33.000000 import_expression-1.1.5/import_expression/_syntax.py
--rw-r-----   0 user      (1000) user      (1000)     1243 2024-05-25 01:05:33.000000 import_expression-1.1.5/import_expression/constants.py
--rw-r-----   0 user      (1000) user      (1000)       22 2024-05-25 01:19:05.000000 import_expression-1.1.5/import_expression/version.py
-drwxr-x---   0 user      (1000) user      (1000)        0 2024-05-25 01:19:31.773328 import_expression-1.1.5/import_expression.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     3495 2024-05-25 01:19:31.000000 import_expression-1.1.5/import_expression.egg-info/PKG-INFO
--rw-r-----   0 user      (1000) user      (1000)      610 2024-05-25 01:19:31.000000 import_expression-1.1.5/import_expression.egg-info/SOURCES.txt
--rw-r-----   0 user      (1000) user      (1000)        1 2024-05-25 01:19:31.000000 import_expression-1.1.5/import_expression.egg-info/dependency_links.txt
--rw-r-----   0 user      (1000) user      (1000)      180 2024-05-25 01:19:31.000000 import_expression-1.1.5/import_expression.egg-info/entry_points.txt
--rw-r-----   0 user      (1000) user      (1000)       51 2024-05-25 01:19:31.000000 import_expression-1.1.5/import_expression.egg-info/requires.txt
--rw-r-----   0 user      (1000) user      (1000)       18 2024-05-25 01:19:31.000000 import_expression-1.1.5/import_expression.egg-info/top_level.txt
--rw-r-----   0 user      (1000) user      (1000)      130 2024-05-25 01:05:33.000000 import_expression-1.1.5/import_expression.pth
--rw-r-----   0 user      (1000) user      (1000)       38 2024-05-25 01:19:31.776662 import_expression-1.1.5/setup.cfg
--rwxr-x---   0 user      (1000) user      (1000)     5035 2024-05-25 01:05:33.000000 import_expression-1.1.5/setup.py
--rw-r-----   0 user      (1000) user      (1000)     8747 2024-05-25 01:05:33.000000 import_expression-1.1.5/tests.py
+drwxr-x---   0 user      (1000) user      (1000)        0 2024-05-27 02:42:32.326960 import_expression-2.0.0/
+-rw-r-----   0 user      (1000) user      (1000)     4280 2024-05-25 01:05:33.000000 import_expression-2.0.0/LICENSE
+-rw-r-----   0 user      (1000) user      (1000)     1100 2024-05-27 02:26:07.000000 import_expression-2.0.0/LICENSE-header
+-rw-r-----   0 user      (1000) user      (1000)       47 2024-05-25 01:05:33.000000 import_expression-2.0.0/MANIFEST.in
+-rw-r--r--   0 user      (1000) user      (1000)     2925 2024-05-27 02:42:32.326960 import_expression-2.0.0/PKG-INFO
+-rw-r-----   0 user      (1000) user      (1000)     2380 2024-05-27 02:29:07.000000 import_expression-2.0.0/README.md
+drwxr-x---   0 user      (1000) user      (1000)        0 2024-05-27 02:42:32.323626 import_expression-2.0.0/import_expression/
+-rwxr-x---   0 user      (1000) user      (1000)     4276 2024-05-27 02:29:07.000000 import_expression-2.0.0/import_expression/__init__.py
+-rw-r-----   0 user      (1000) user      (1000)     9250 2024-05-27 02:27:51.000000 import_expression-2.0.0/import_expression/__main__.py
+-rw-r-----   0 user      (1000) user      (1000)     4081 2024-05-27 02:29:07.000000 import_expression-2.0.0/import_expression/_parser.py
+-rw-r-----   0 user      (1000) user      (1000)     6769 2024-05-27 02:39:47.000000 import_expression-2.0.0/import_expression/_syntax.py
+-rw-r-----   0 user      (1000) user      (1000)     1174 2024-05-27 02:27:51.000000 import_expression-2.0.0/import_expression/constants.py
+-rw-r-----   0 user      (1000) user      (1000)       22 2024-05-27 02:31:54.000000 import_expression-2.0.0/import_expression/version.py
+drwxr-x---   0 user      (1000) user      (1000)        0 2024-05-27 02:42:32.326960 import_expression-2.0.0/import_expression.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     2925 2024-05-27 02:42:32.000000 import_expression-2.0.0/import_expression.egg-info/PKG-INFO
+-rw-r-----   0 user      (1000) user      (1000)      488 2024-05-27 02:42:32.000000 import_expression-2.0.0/import_expression.egg-info/SOURCES.txt
+-rw-r-----   0 user      (1000) user      (1000)        1 2024-05-27 02:42:32.000000 import_expression-2.0.0/import_expression.egg-info/dependency_links.txt
+-rw-r-----   0 user      (1000) user      (1000)      122 2024-05-27 02:42:32.000000 import_expression-2.0.0/import_expression.egg-info/entry_points.txt
+-rw-r-----   0 user      (1000) user      (1000)       52 2024-05-27 02:42:32.000000 import_expression-2.0.0/import_expression.egg-info/requires.txt
+-rw-r-----   0 user      (1000) user      (1000)       18 2024-05-27 02:42:32.000000 import_expression-2.0.0/import_expression.egg-info/top_level.txt
+-rw-r-----   0 user      (1000) user      (1000)       38 2024-05-27 02:42:32.326960 import_expression-2.0.0/setup.cfg
+-rwxr-x---   0 user      (1000) user      (1000)     4042 2024-05-27 02:34:49.000000 import_expression-2.0.0/setup.py
+-rw-r-----   0 user      (1000) user      (1000)     6581 2024-05-27 02:29:07.000000 import_expression-2.0.0/tests.py
```

### Comparing `import_expression-1.1.5/LICENSE` & `import_expression-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `import_expression-1.1.5/LICENSE-header` & `import_expression-2.0.0/LICENSE-header`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright © 2018–2019 Io Mintz <io@mintz.cc>
+# Copyright © io mintz <io@mintz.cc>
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the “Software”),
 # to deal in the Software without restriction, including without limitation the
 # rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
 # sell copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `import_expression-1.1.5/PKG-INFO` & `import_expression-2.0.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,10 @@
-Metadata-Version: 2.1
-Name: import_expression
-Version: 1.1.5
-Summary: Parses a superset of Python allowing for inline module import expressions
-Home-page: https://github.com/iomintz/import-expression-parser
-Author: io mintz
-Author-email: io@mintz.cc
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: LICENSE-header
-Requires-Dist: astunparse<2.0.0,>=1.6.3
-Provides-Extra: test
-Requires-Dist: pytest; extra == "test"
-Requires-Dist: pytest-cov; extra == "test"
-
 # Import Expression Parser (for lack of a better name)
 
-[![Build Status](https://img.shields.io/travis/iomintz/import-expression-parser/main.svg?label=tests)](https://travis-ci.org/iomintz/import-expression-parser)
-[![Coverage Status](https://coveralls.io/repos/github/iomintz/import-expression-parser/badge.svg?branch=main)](https://coveralls.io/github/iomintz/import-expression-parser?branch=main)
+[![Coverage Status](https://coveralls.io/repos/github/iomintz/import-expression-parser/badge.svg?branch=main)](https://coveralls.io/github/ioistired/import-expression-parser?branch=main)
 
 Import Expression Parser converts code like this:
 
 ```py
 urllib.parse!.quote('hello there')
 ```
 
@@ -35,15 +17,15 @@
 
 ```py
 >>> import import_expression
 >>> import_expression.eval('collections!.Counter("bccdddeeee")')
 Counter({'e': 4, 'd': 3, 'c': 2, 'b': 1})
 ```
 
-The other public functions are `exec`, `compile`, `parse`, `find_imports`, and `update_globals`.
+The other public functions are `exec`, `compile`, and `parse`.
 See their docstrings for details.
 
 By default, the filename for `SyntaxError`s is `<string>`.
 To change this, pass in a filename via the `filename` kwarg.
 
 ### Reusing compiled code objects
 
@@ -61,44 +43,30 @@
 
 ```py
 code = import_expression.compile('foo!.bar(l)', mode='eval')
 for line in sys.stdin:
 	print(import_expression.eval(code, dict(l=line)))
 ```
 
-### Custom encoding
-
-```py
-# encoding: import_expression
-print(typing!.TYPE_CHECKING)
-```
-
-This file, when run, will print True/False. For maximum laziness you can also do `#coding:ie`.
-
 ### REPL usage
 
 Run `import-expression` for an import expression enabled REPL. \
 Run `import-expression -a` for a REPL that supports both import expressions and top level `await` (3.8+).
 
 See `import-expression --help` for more details.
 
 ### Running a file
 
 Run `import-expression <filename.py>`.
 
-### File rewriter
-
-Run `import-expression-rewrite <file.py>` to rewrite a file containing import expressions to standard Python. \
-Add the `-i` flag to rewrite in-place.
-
 ## Limitations / Known Issues
 
 * Due to the hell that is f-string parsing, and because `!` is already an operator inside f-strings,
   import expressions inside f-strings will likely never be supported.
 * Due to python limitations, results of `import_expression.exec` will have no effect on the caller's globals or locals
   without an explicit `globals` argument.
 * Unlike real operators, spaces before and after the import expression operator (such as `x ! .y`) are not supported.
 
-## [License](https://github.com/iomintz/import-expression-parser/blob/main/LICENSE)
+## [License](https://github.com/ioistired/import-expression/blob/main/LICENSE)
 
-Copyright © 2018–2019 Io Mintz <<io@mintz.cc>>. All Rights Reserved. \
+Copyright © io mintz <<io@mintz.cc>>. All Rights Reserved. \
 Licensed under the MIT License. See the LICENSE file for details.
```

### Comparing `import_expression-1.1.5/README.md` & `import_expression-2.0.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,27 @@
+Metadata-Version: 2.1
+Name: import_expression
+Version: 2.0.0
+Summary: Parses a superset of Python allowing for inline module import expressions
+Home-page: https://github.com/ioistired/import-expression
+Author: io mintz
+Author-email: io@mintz.cc
+License: MIT
+Classifier: License :: OSI Approved :: MIT License
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: LICENSE-header
+Requires-Dist: typing-extensions<5,>=4.3
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
+
 # Import Expression Parser (for lack of a better name)
 
-[![Build Status](https://img.shields.io/travis/iomintz/import-expression-parser/main.svg?label=tests)](https://travis-ci.org/iomintz/import-expression-parser)
-[![Coverage Status](https://coveralls.io/repos/github/iomintz/import-expression-parser/badge.svg?branch=main)](https://coveralls.io/github/iomintz/import-expression-parser?branch=main)
+[![Coverage Status](https://coveralls.io/repos/github/iomintz/import-expression-parser/badge.svg?branch=main)](https://coveralls.io/github/ioistired/import-expression-parser?branch=main)
 
 Import Expression Parser converts code like this:
 
 ```py
 urllib.parse!.quote('hello there')
 ```
 
@@ -18,15 +34,15 @@
 
 ```py
 >>> import import_expression
 >>> import_expression.eval('collections!.Counter("bccdddeeee")')
 Counter({'e': 4, 'd': 3, 'c': 2, 'b': 1})
 ```
 
-The other public functions are `exec`, `compile`, `parse`, `find_imports`, and `update_globals`.
+The other public functions are `exec`, `compile`, and `parse`.
 See their docstrings for details.
 
 By default, the filename for `SyntaxError`s is `<string>`.
 To change this, pass in a filename via the `filename` kwarg.
 
 ### Reusing compiled code objects
 
@@ -44,44 +60,30 @@
 
 ```py
 code = import_expression.compile('foo!.bar(l)', mode='eval')
 for line in sys.stdin:
 	print(import_expression.eval(code, dict(l=line)))
 ```
 
-### Custom encoding
-
-```py
-# encoding: import_expression
-print(typing!.TYPE_CHECKING)
-```
-
-This file, when run, will print True/False. For maximum laziness you can also do `#coding:ie`.
-
 ### REPL usage
 
 Run `import-expression` for an import expression enabled REPL. \
 Run `import-expression -a` for a REPL that supports both import expressions and top level `await` (3.8+).
 
 See `import-expression --help` for more details.
 
 ### Running a file
 
 Run `import-expression <filename.py>`.
 
-### File rewriter
-
-Run `import-expression-rewrite <file.py>` to rewrite a file containing import expressions to standard Python. \
-Add the `-i` flag to rewrite in-place.
-
 ## Limitations / Known Issues
 
 * Due to the hell that is f-string parsing, and because `!` is already an operator inside f-strings,
   import expressions inside f-strings will likely never be supported.
 * Due to python limitations, results of `import_expression.exec` will have no effect on the caller's globals or locals
   without an explicit `globals` argument.
 * Unlike real operators, spaces before and after the import expression operator (such as `x ! .y`) are not supported.
 
-## [License](https://github.com/iomintz/import-expression-parser/blob/main/LICENSE)
+## [License](https://github.com/ioistired/import-expression/blob/main/LICENSE)
 
-Copyright © 2018–2019 Io Mintz <<io@mintz.cc>>. All Rights Reserved. \
+Copyright © io mintz <<io@mintz.cc>>. All Rights Reserved. \
 Licensed under the MIT License. See the LICENSE file for details.
```

### Comparing `import_expression-1.1.5/import_expression/__init__.py` & `import_expression-2.0.0/import_expression/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright © 2018–2019 Io Mintz <io@mintz.cc>
+# Copyright © io mintz <io@mintz.cc>
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the “Software”),
 # to deal in the Software without restriction, including without limitation the
 # rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
 # sell copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -25,22 +25,21 @@
 import inspect as _inspect
 import typing as _typing
 import types as _types
 from codeop import PyCF_DONT_IMPLY_DEDENT
 
 from . import constants
 from ._syntax import fix_syntax as _fix_syntax
-from ._parser import parse_ast as _parse_ast
-from ._parser import find_imports as _find_imports
+from ._parser import transform_ast as _transform_ast
 from .version import __version__
 
 with _contextlib.suppress(NameError):
 	del version
 
-__all__ = ('compile', 'parse', 'eval', 'exec', 'constants', 'find_imports', 'update_globals')
+__all__ = ('compile', 'parse', 'eval', 'exec', 'constants')
 
 _source = _typing.Union[_ast.AST, _typing.AnyStr]
 
 def parse(source: _source, filename=constants.DEFAULT_FILENAME, mode='exec', *, flags=0, **kwargs) -> _ast.AST:
 	"""
 	convert Import Expression Python™ to an AST
 
@@ -53,22 +52,22 @@
 
 	Filename is used in tracebacks, in case of invalid syntax or runtime exceptions.
 
 	The remaining keyword arguments are passed to ast.parse as is.
 	"""
 	# for some API compatibility with ast, allow parse(parse('foo')) to work
 	if isinstance(source, _ast.AST):
-		return _parse_ast(source, filename=filename)
+		return _transform_ast(source, filename=filename)
 
 	fixed = _fix_syntax(source, filename=filename)
 	if flags & PyCF_DONT_IMPLY_DEDENT:
 		# just run it for the syntax errors, which codeop picks up on
 		_builtins.compile(fixed, filename, mode, flags)
 	tree = _ast.parse(fixed, filename, mode, **kwargs)
-	return _parse_ast(tree, source=source, filename=filename)
+	return _transform_ast(tree, source=source, filename=filename)
 
 def compile(
 	source: _source,
 	filename=constants.DEFAULT_FILENAME,
 	mode='exec',
 	flags=0,
 	dont_inherit=False,
@@ -97,37 +96,15 @@
 	Therefore, if no globals are provided, the results will be discarded!
 	"""
 	globals, locals = _parse_eval_exec_args(globals, locals)
 	if _inspect.iscode(source):
 		return _builtins.eval(source, globals, locals)
 	_builtins.eval(compile(source, constants.DEFAULT_FILENAME, 'exec'), globals, locals)
 
-def find_imports(source: str, filename=constants.DEFAULT_FILENAME, mode='exec'):
-	"""return a list of all module names required by the given source code."""
-	# passing an AST is not supported because it doesn't make sense to.
-	# either the AST is one that we made, in which case the imports have already been made and calling parse_ast again
-	# would find no imports, or it's an AST made by parsing the output of fix_syntax, which is internal.
-	fixed = _fix_syntax(source, filename=filename)
-	tree = _ast.parse(fixed, filename, mode)
-	return _find_imports(tree, filename=filename)
-
-def update_globals(globals: dict) -> dict:
-	"""Ensure that the variables required for eval/exec are present in the given dict.
-	Note that import_expression.eval and import_expression.exec do this for you automatically.
-	Calling this function yourself is only necessary if you want to call builtins.eval or builtins.exec
-	with the return value of import_expression.compile.
-
-	This function always returns the passed dictionary to make expression chaining easier.
-	"""
-	globals.update({constants.IMPORTER: _importlib.import_module})
-	return globals
-
 def _parse_eval_exec_args(globals, locals):
 	if globals is None:
 		globals = {}
 
-	update_globals(globals)
-
 	if locals is None:
 		locals = globals
 
 	return globals, locals
```

### Comparing `import_expression-1.1.5/import_expression/__main__.py` & `import_expression-2.0.0/import_expression/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright © 2018–2019 Io Mintz <io@mintz.cc>
+# Copyright © io mintz <io@mintz.cc>
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the “Software”),
 # to deal in the Software without restriction, including without limitation the
 # rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
 # sell copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -86,15 +86,14 @@
 				self.flags |= feature.compiler_flag
 		return codeob
 
 
 class ImportExpressionInteractiveConsole(code.InteractiveConsole):
 	def __init__(self, locals=None, filename='<console>'):
 		super().__init__(locals, filename)
-		self.locals.update({constants.IMPORTER: importlib.import_module})
 		self.compile = ImportExpressionCommandCompiler()
 
 # we must vendor this class because it creates global variables that the main code depends on
 class ImportExpressionAsyncIOInteractiveConsole(ImportExpressionInteractiveConsole):
 	def __init__(self, locals, loop):
 		super().__init__(locals)
 		self.loop = loop
```

### Comparing `import_expression-1.1.5/import_expression/constants.py` & `import_expression-2.0.0/import_expression/constants.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright © 2018–2019 Io Mintz <io@mintz.cc>
+# Copyright © io mintz <io@mintz.cc>
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the “Software”),
 # to deal in the Software without restriction, including without limitation the
 # rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
 # sell copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -15,11 +15,10 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
 # THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 
 IMPORT_OP = '!'
-IMPORTER = '_IMPORT_MODULE'
-MARKER = '_IMPORT_EXPR_END'  # TODO replace with UUIDs
+MARKER = '_IMPORT_MARKER'
 
 DEFAULT_FILENAME = '<string>'
```

### Comparing `import_expression-1.1.5/import_expression.egg-info/PKG-INFO` & `import_expression-2.0.0/import_expression.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: import_expression
-Version: 1.1.5
+Version: 2.0.0
 Summary: Parses a superset of Python allowing for inline module import expressions
-Home-page: https://github.com/iomintz/import-expression-parser
+Home-page: https://github.com/ioistired/import-expression
 Author: io mintz
 Author-email: io@mintz.cc
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSE-header
-Requires-Dist: astunparse<2.0.0,>=1.6.3
+Requires-Dist: typing-extensions<5,>=4.3
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 
 # Import Expression Parser (for lack of a better name)
 
-[![Build Status](https://img.shields.io/travis/iomintz/import-expression-parser/main.svg?label=tests)](https://travis-ci.org/iomintz/import-expression-parser)
-[![Coverage Status](https://coveralls.io/repos/github/iomintz/import-expression-parser/badge.svg?branch=main)](https://coveralls.io/github/iomintz/import-expression-parser?branch=main)
+[![Coverage Status](https://coveralls.io/repos/github/iomintz/import-expression-parser/badge.svg?branch=main)](https://coveralls.io/github/ioistired/import-expression-parser?branch=main)
 
 Import Expression Parser converts code like this:
 
 ```py
 urllib.parse!.quote('hello there')
 ```
 
@@ -35,15 +34,15 @@
 
 ```py
 >>> import import_expression
 >>> import_expression.eval('collections!.Counter("bccdddeeee")')
 Counter({'e': 4, 'd': 3, 'c': 2, 'b': 1})
 ```
 
-The other public functions are `exec`, `compile`, `parse`, `find_imports`, and `update_globals`.
+The other public functions are `exec`, `compile`, and `parse`.
 See their docstrings for details.
 
 By default, the filename for `SyntaxError`s is `<string>`.
 To change this, pass in a filename via the `filename` kwarg.
 
 ### Reusing compiled code objects
 
@@ -61,44 +60,30 @@
 
 ```py
 code = import_expression.compile('foo!.bar(l)', mode='eval')
 for line in sys.stdin:
 	print(import_expression.eval(code, dict(l=line)))
 ```
 
-### Custom encoding
-
-```py
-# encoding: import_expression
-print(typing!.TYPE_CHECKING)
-```
-
-This file, when run, will print True/False. For maximum laziness you can also do `#coding:ie`.
-
 ### REPL usage
 
 Run `import-expression` for an import expression enabled REPL. \
 Run `import-expression -a` for a REPL that supports both import expressions and top level `await` (3.8+).
 
 See `import-expression --help` for more details.
 
 ### Running a file
 
 Run `import-expression <filename.py>`.
 
-### File rewriter
-
-Run `import-expression-rewrite <file.py>` to rewrite a file containing import expressions to standard Python. \
-Add the `-i` flag to rewrite in-place.
-
 ## Limitations / Known Issues
 
 * Due to the hell that is f-string parsing, and because `!` is already an operator inside f-strings,
   import expressions inside f-strings will likely never be supported.
 * Due to python limitations, results of `import_expression.exec` will have no effect on the caller's globals or locals
   without an explicit `globals` argument.
 * Unlike real operators, spaces before and after the import expression operator (such as `x ! .y`) are not supported.
 
-## [License](https://github.com/iomintz/import-expression-parser/blob/main/LICENSE)
+## [License](https://github.com/ioistired/import-expression/blob/main/LICENSE)
 
-Copyright © 2018–2019 Io Mintz <<io@mintz.cc>>. All Rights Reserved. \
+Copyright © io mintz <<io@mintz.cc>>. All Rights Reserved. \
 Licensed under the MIT License. See the LICENSE file for details.
```

### Comparing `import_expression-1.1.5/setup.py` & `import_expression-2.0.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-# Copyright © 2018–2019 Io Mintz <io@mintz.cc>
+# Copyright © io mintz <io@mintz.cc>
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the “Software”),
 # to deal in the Software without restriction, including without limitation the
 # rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
 # sell copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -104,77 +104,45 @@
 	commands=(
 		(sys.executable, __file__, 'sdist', 'bdist_wheel'),
 		('twine', 'upload', 'dist/*'),
 	)
 ):
 	pass
 
-# `class install` is modified from future_fstrings/setup.py at 596deb0
-
-class install(_install):
-	def initialize_options(self):
-		super().initialize_options()
-
-		with open('import_expression.pth') as f:
-			self.extra_path = (self.distribution.metadata.name, f.read())
-
-	def finalize_options(self):
-		super().finalize_options()
-
-		install_suffix = os.path.relpath(
-			self.install_lib, self.install_libbase,
-		)
-		if install_suffix == '.':
-			distutils.log.info('skipping install of .pth during easy-install')
-		elif install_suffix == self.extra_path[1]:
-			self.install_lib = self.install_libbase
-			distutils.log.info(
-				"will install .pth to '%s.pth'",
-				os.path.join(self.install_lib, self.extra_path[0]),
-			)
-		else:
-			raise AssertionError(
-				'unexpected install_suffix',
-				self.install_lib, self.install_libbase, install_suffix,
-			)
-
-command_classes['install'] = install
-
 setuptools.setup(
 	name='import_expression',
 	version=version,
 
 	description='Parses a superset of Python allowing for inline module import expressions',
 	long_description=long_description,
 	long_description_content_type='text/markdown',
 
 	license='MIT',
 
 	author='io mintz',
 	author_email='io@mintz.cc',
-	url='https://github.com/iomintz/import-expression-parser',
+	url='https://github.com/ioistired/import-expression',
 
-	packages=['import_expression', 'import_expression._codec'],
+	packages=['import_expression'],
 
 	install_requires=[
-		'astunparse>=1.6.3,<2.0.0',
+		'typing-extensions >= 4.3, < 5'
 	],
 
 	extras_require={
 		'test': [
 			'pytest',
 			'pytest-cov',
 		],
 	},
 
 	entry_points={
 		'console_scripts': [
 			'import_expression = import_expression.__main__:main',
 			'import-expression = import_expression.__main__:main',
-			'import-expression-rewrite = import_expression._main2:main',
 		],
 	},
 
 	cmdclass=command_classes,
 
 	classifiers=[
 		'License :: OSI Approved :: MIT License',
```

### Comparing `import_expression-1.1.5/tests.py` & `import_expression-2.0.0/tests.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright © 2018–2019 Io Mintz <io@mintz.cc>
+# Copyright © io mintz <io@mintz.cc>
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the “Software”),
 # to deal in the Software without restriction, including without limitation the
 # rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
 # sell copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -22,22 +22,14 @@
 import os
 import textwrap
 
 import pytest
 
 import import_expression as ie
 
-try:
-	import astunparse
-except ImportError:
-	HAVE_ASTUNPARSE = False
-else:
-	HAVE_ASTUNPARSE = True
-
-
 invalid_attribute_cases = (
 	# arrange this as if ! is binary 1, empty str is 0
 	'!a',
 
 	'a.!b',
 	'!a.b',
 	'a!.b!',
@@ -212,19 +204,14 @@
 			
 
 			return bar()
 	"""), g)
 
 	assert g['foo'](1) == 'can we make it into jishaku?'
 
-def test_importer_name_not_mangled():
-	# if import_expression.constants.IMPORTER.startswith('__'),
-	# this will fail
-	ie.exec('class Foo: x = io!')
-
 def test_flags():
 	import ast
 	assert isinstance(ie.compile('foo', flags=ast.PyCF_ONLY_AST), ast.AST)
 
 def test_eval_code_object():
 	import collections
 	code = ie.compile('collections!.Counter', '', 'eval')
@@ -244,89 +231,23 @@
 		ie.compile(invalid)
 
 def test_dont_imply_dedent():
 	from codeop import PyCF_DONT_IMPLY_DEDENT
 	with pytest.raises(SyntaxError):
 		ie.compile('def foo():\n\tpass', mode='single', flags=PyCF_DONT_IMPLY_DEDENT)
 
-def test_parse_ast():
+def test_transform_ast():
 	from typing import Any
 	node = ie.parse(ie.parse('typing!.Any', mode='eval'))
 	assert ie.eval(node) is Any
 
 def test_locals_arg():
 	ie.exec('assert locals() is globals()', {})
 	ie.exec('assert locals() is not globals()', {}, {})
 
-def test_update_globals():
-	import collections
-	code = ie.compile('collections!.Counter', mode='eval')
-	g = ie.update_globals({})
-	assert eval(code, g) is collections.Counter
-
-def test_find_imports():
-	with pytest.raises(SyntaxError):
-		ie.find_imports('x; y', mode='eval')
-
-	assert set(ie.find_imports(textwrap.dedent("""
-		x = a!
-		y = a.b!.c
-		z = d.e.f
-	"""))) == {'a', 'a.b'}
-
-	assert ie.find_imports('urllib.parse!.quote', mode='eval') == ['urllib.parse']
-
-class remove(contextlib.AbstractContextManager):
-	def __init__(self, name):
-		self.name = name
-	def __enter__(self):
-		return self
-	def __exit__(self, *excinfo):
-		os.remove(self.name)
-
 def test_bytes():
 	import typing
 	assert ie.eval(b'typing!.TYPE_CHECKING') == typing.TYPE_CHECKING
 
-@pytest.mark.skipif(not HAVE_ASTUNPARSE, reason='requires the [codec] setup.py extra')
-@pytest.mark.parametrize('encoding', ['import_expression', 'ie'])
-def test_encoding(encoding):
-	import import_expression._codec
-	import_expression._codec.register()
-
-	import tempfile
-	import typing
-	fn = tempfile.mktemp()
-	with remove(fn), open(fn, mode='w+', encoding=encoding) as f:
-		f.write('x = typing!.TYPE_CHECKING')
-		f.seek(0)
-		g = {}
-		exec(f.read(), g)
-		assert g['x'] == typing.TYPE_CHECKING
-		assert not f.read()
-
-		f.seek(0)
-		while f.readline():  # we must reach EOF eventually
-			pass
-
-@pytest.mark.skipif(not HAVE_ASTUNPARSE, reason='requires the [codec] setup.py extra')
-@pytest.mark.parametrize('encoding', ['import_expression', 'ie'])
-def test_encoding_2(encoding):
-	import codecs
-	import typing
-	g = {}
-	exec(codecs.decode(b'x = typing!.TYPE_CHECKING', encoding=encoding), g)
-	assert g['x'] == typing.TYPE_CHECKING
-
-@pytest.mark.skipif(not HAVE_ASTUNPARSE, reason='no need to test built in encoding without the [codec] setup.py extra')
-def test_utf8_unaffected():
-	import tempfile
-	fn = tempfile.mktemp()
-	with remove(fn), open(fn, mode='w+', encoding='shift-jis') as f:
-		f.write('foo')
-		f.seek(0)
-		assert f.read() == 'foo'
-		assert not f.read()
-
 def test_beat_is_gay():
 	with pytest.raises(SyntaxError):
 		ie.compile('"beat".succ!')
```

