# Comparing `tmp/squelch-0.3.0.tar.gz` & `tmp/squelch-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "squelch-0.3.0.tar", max compression
+gzip compressed data, was "squelch-0.3.1.tar", max compression
```

## Comparing `squelch-0.3.0.tar` & `squelch-0.3.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11357 2018-06-22 07:09:46.422789 squelch-0.3.0/LICENSE
--rw-r--r--   0        0        0     5919 2024-05-06 18:59:51.634075 squelch-0.3.0/README.md
--rw-r--r--   0        0        0      721 2024-05-06 18:59:51.634075 squelch-0.3.0/pyproject.toml
--rw-r--r--   0        0        0    29979 2024-05-06 18:59:51.634075 squelch-0.3.0/squelch/__init__.py
--rw-r--r--   0        0        0     6698 2024-05-06 18:59:51.634075 squelch-0.3.0/squelch/__main__.py
--rw-r--r--   0        0        0     6863 1970-01-01 00:00:00.000000 squelch-0.3.0/setup.py
--rw-r--r--   0        0        0     6747 1970-01-01 00:00:00.000000 squelch-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2018-06-22 07:09:46.422789 squelch-0.3.1/LICENSE
+-rw-r--r--   0        0        0     5919 2024-05-06 18:59:51.634075 squelch-0.3.1/README.md
+-rw-r--r--   0        0        0      721 2024-05-27 14:42:47.859256 squelch-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0    30073 2024-05-27 14:42:56.207348 squelch-0.3.1/squelch/__init__.py
+-rw-r--r--   0        0        0     6698 2024-05-06 18:59:51.634075 squelch-0.3.1/squelch/__main__.py
+-rw-r--r--   0        0        0     6863 1970-01-01 00:00:00.000000 squelch-0.3.1/setup.py
+-rw-r--r--   0        0        0     6747 1970-01-01 00:00:00.000000 squelch-0.3.1/PKG-INFO
```

### Comparing `squelch-0.3.0/LICENSE` & `squelch-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `squelch-0.3.0/README.md` & `squelch-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `squelch-0.3.0/pyproject.toml` & `squelch-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "squelch"
-version = "0.3.0"
+version = "0.3.1"
 description = "Simple SQL REPL Command Handler"
 authors = ["Paul Breen <pbree@bas.ac.uk>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/paul-breen/squelch"
 homepage = "https://github.com/paul-breen/squelch"
 documentation = "https://github.com/paul-breen/squelch/blob/main/README.md"
```

### Comparing `squelch-0.3.0/squelch/__init__.py` & `squelch-0.3.1/squelch/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.3.0'
+__version__ = '0.3.1'
 
 import sys
 import logging
 from pathlib import Path
 import atexit
 import traceback
 import re
@@ -271,14 +271,15 @@
 
 Help
   \?                     show help on backslash commands
 
 Informational
   \d                     list tables, views, and sequences
   \d      NAME           describe table or view
+  \di     [NAME]         list indexes
   \ds     [NAME]         list sequences
   \dt     [NAME]         list tables
   \dv     [NAME]         list views
 
 Formatting
   \pset [NAME [VALUE]]   set table output option
                          (pager)
@@ -567,14 +568,16 @@
 
         return self.params
 
     def clean_raw_input(self, raw, terminator=';'):
         """
         Clean the raw input query
 
+        :param raw: The raw query
+        :type raw: str
         :param terminator: A query terminator to be stripped from the query
         :type terminator: str
         :returns: The raw stripped query
         :rtype: str
         """
 
         raw = raw.strip().rstrip(terminator)
@@ -906,15 +909,15 @@
 
         The REPL is initialised, an atexit handler is registered to complete
         the REPL on exit, and the REPL is then entered in an infinite loop.
         The user is prompted to run database queries or REPL commands,
         such as the quit command
         """
 
-        prompt = f"{self.conn.engine.url.database} => "
+        prompt = f"{self.conn.engine.url.database}=> "
         self.init_repl()
         atexit.register(self.complete_repl)
 
         while True:
             raw = self.prompt_for_input(prompt=prompt)
             self.process_input(raw)
```

### Comparing `squelch-0.3.0/squelch/__main__.py` & `squelch-0.3.1/squelch/__main__.py`

 * *Files identical despite different names*

### Comparing `squelch-0.3.0/setup.py` & `squelch-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['sqlalchemy>=2.0.29,<3.0.0', 'tabulate>=0.9.0,<0.10.0']
 
 entry_points = \
 {'console_scripts': ['squelch = squelch.__main__:main']}
 
 setup_kwargs = {
     'name': 'squelch',
-    'version': '0.3.0',
+    'version': '0.3.1',
     'description': 'Simple SQL REPL Command Handler',
     'long_description': '# squelch\n\nSquelch is a package providing a Simple [SQL](https://en.wikipedia.org/wiki/SQL) [REPL](https://en.wikipedia.org/wiki/Read%E2%80%93eval%E2%80%93print_loop) Command Handler.  Squelch uses [SQLAlchemy](https://www.sqlalchemy.org/) for database access and so can support any database engine that SQLAlchemy supports, thereby providing a common database client experience for any of those database engines.  Squelch is modelled on a simplified `psql`, the [PostgreSQL](https://www.postgresql.org/) command line client.  The Squelch [CLI](https://en.wikipedia.org/wiki/Command-line_interface) supports readline history and basic SQL statement tab completions.\n\n## Install\n\nThe package can be installed from [PyPI](https://pypi.org/):\n\n```bash\n$ pip install squelch\n```\n\n## From the command line\n\nThe package comes with a functional CLI called `squelch`, which just calls the package *main*, hence the following two invocations are equivalent:\n\n```bash\n$ python3 -m squelch\n```\n\n```bash\n$ squelch\n```\n\nThe only required argument is a database connection URL.  This can either be passed on the command line, via the `--url` option, or specified in a [JSON](https://en.wikipedia.org/wiki/JSON) configuration file given by the `--conf-file` option.  The form of the JSON configuration file is as follows:\n\n```json\n{\n  "url": "<URL>"\n}\n```\n\nwhere the `<URL>` follows the [SQLAlchemy database connection URL syntax](https://docs.sqlalchemy.org/en/20/core/engines.html#database-urls).  An advantage of using a configuration file is that it avoids providing database login credentials in plain text on the command line.\n\n### Running queries\n\nWhen running the CLI in a terminal, the user is dropped into an interactive REPL.  From here, the user is prompted for input, which can be an SQL statement to be sent to the database engine, or a CLI command (backslash command) such as `\\q` to quit the CLI:\n\n```\n$ python -m squelch -c tests/data/test.json \nsquelch (0.3.0)\nType "help" for help.\n\ntests/data/test.db => select * from data;\n id   | name   | status   | key\n------+--------+----------+-----------\n 1    | pmb    | 0        | 0000-0000\n 2    | abc    | 0        | 0000-0001\n 3    | def    | 0        | 0000-0002\n 4    | ghi    | 1        | 0000-0003\n(4 rows)\n\ntests/data/test.db => \\q\n```\n\nAlternatively, the CLI can be called as a *one-shot* by providing a query on `stdin`, thereby allowing it to be called in scripts.\n\nFor example, using `echo` to pipe a query to the CLI:\n\n```bash\n$ echo "select * from data" | python -m squelch -c tests/data/test.json\n id   | name   | status   | key\n------+--------+----------+-----------\n 1    | pmb    | 0        | 0000-0000\n 2    | abc    | 0        | 0000-0001\n 3    | def    | 0        | 0000-0002\n 4    | ghi    | 1        | 0000-0003\n(4 rows)\n\n```\n\nOr redirecting from a file.  Given the following queries in a file:\n\n```bash\n$ cat tests/data/queries.sql\nselect * from data;\nselect * from data where id = 1;\nselect * from status where status = 1;\n```\n\nthe result would be:\n\n```bash\n$ python -m squelch -c tests/data/test.json < tests/data/queries.sql\n id   | name   | status   | key\n------+--------+----------+-----------\n 1    | pmb    | 0        | 0000-0000\n 2    | abc    | 0        | 0000-0001\n 3    | def    | 0        | 0000-0002\n 4    | ghi    | 1        | 0000-0003\n(4 rows)\n\n id   | name   | status   | key\n------+--------+----------+-----------\n 1    | pmb    | 0        | 0000-0000\n(1 row)\n\n name   | status\n--------+----------\n ghi    | 1\n(1 row)\n\n```\n\n#### Machine-readable data in scripts\n\nIt\'s likely that when calling the CLI from a script, the user is less interested in the data being laid out in a human-readable table, rather, they probably want it as machine-readable data.  The table format can be set (using the `--pset` option) to `csv` so that the table is printed as [CSV](https://en.wikipedia.org/wiki/Comma-separated_values).  Additionally, the table footer can be turned off (again using `--pset`) so that the result is just a simple CSV table.  Taking our example from earlier, the result would be:\n\n```bash\n$ echo "select * from data;" | python -m squelch -c tests/data/test.json --pset format=csv --pset footer=off\nid,name,status,key\n1,pmb,0,0000-0000\n2,abc,0,0000-0001\n3,def,0,0000-0002\n4,ghi,1,0000-0003\n\n```\n\n### Command line usage\n\n```\nusage: squelch [-h] [-c CONF_FILE] [-u URL] [-S [NAME=VALUE [NAME=VALUE ...]]]\n               [-P [NAME=VALUE [NAME=VALUE ...]]] [-v] [-V]\n\nSquelch is a Simple SQL REPL Command Handler.\n\noptional arguments:\n  -h, --help            show this help message and exit\n  -c CONF_FILE, --conf-file CONF_FILE\n                        The full path to a JSON configuration file. It\n                        defaults to ./squelch.json.\n  -u URL, --url URL     The database connection URL, as required by\n                        sqlalchemy.create_engine().\n  -S [NAME=VALUE [NAME=VALUE ...]], --set [NAME=VALUE [NAME=VALUE ...]]\n                        Set state variable NAME to VALUE.\n  -P [NAME=VALUE [NAME=VALUE ...]], --pset [NAME=VALUE [NAME=VALUE ...]]\n                        Set printing state variable NAME to VALUE.\n  -v, --verbose         Turn verbose messaging on. The effects of this option\n                        are incremental.\n  -V, --version         show program\'s version number and exit\n\nDatabase Connection URL\n\nThe database connection URL can either be passed on the command line, via the --url option, or specified in a JSON configuration file given by the --conf-file option.  The form of the JSON configuration file is as follows:\n\n{\n  "url": "<URL>"\n}\n\nFrom the SQLAlchemy documentation:\n\n"The string form of the URL is dialect[+driver]://user:password@host/dbname[?key=value..], where dialect is a database name such as mysql, oracle, postgresql, etc., and driver the name of a DBAPI, such as psycopg2, pyodbc, cx_oracle, etc. Alternatively, the URL can be an instance of URL."\n```\n\n',
     'author': 'Paul Breen',
     'author_email': 'pbree@bas.ac.uk',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/paul-breen/squelch',
```

### Comparing `squelch-0.3.0/PKG-INFO` & `squelch-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: squelch
-Version: 0.3.0
+Version: 0.3.1
 Summary: Simple SQL REPL Command Handler
 Home-page: https://github.com/paul-breen/squelch
 License: Apache-2.0
 Author: Paul Breen
 Author-email: pbree@bas.ac.uk
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

