# Comparing `tmp/fastsql-1.0.0.tar.gz` & `tmp/fastsql-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fastsql-1.0.0.tar", last modified: Sat Sep  5 17:28:26 2020, max compression
+gzip compressed data, was "fastsql-1.0.1.tar", last modified: Mon May 27 17:02:07 2024, max compression
```

## Comparing `fastsql-1.0.0.tar` & `fastsql-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,20 @@
-drwxrwxr-x   0 jhoward   (1002) jhoward   (1002)        0 2020-09-05 17:28:26.000000 fastsql-1.0.0/
--rw-rw-r--   0 jhoward   (1002) jhoward   (1002)     2392 2020-09-05 17:28:26.000000 fastsql-1.0.0/PKG-INFO
--rw-rw-r--   0 jhoward   (1002) jhoward   (1002)     1217 2019-11-15 20:17:59.000000 fastsql-1.0.0/README.md
-drwxrwxr-x   0 jhoward   (1002) jhoward   (1002)        0 2020-09-05 17:28:26.000000 fastsql-1.0.0/fastsql/
--rw-rw-r--   0 jhoward   (1002) jhoward   (1002)     1823 2020-09-05 17:08:49.000000 fastsql-1.0.0/fastsql/__init__.py
-drwxrwxr-x   0 jhoward   (1002) jhoward   (1002)        0 2020-09-05 17:28:26.000000 fastsql-1.0.0/fastsql.egg-info/
--rw-rw-r--   0 jhoward   (1002) jhoward   (1002)     2392 2020-09-05 17:28:26.000000 fastsql-1.0.0/fastsql.egg-info/PKG-INFO
--rw-rw-r--   0 jhoward   (1002) jhoward   (1002)      256 2020-09-05 17:28:26.000000 fastsql-1.0.0/fastsql.egg-info/SOURCES.txt
--rw-rw-r--   0 jhoward   (1002) jhoward   (1002)        1 2020-09-05 17:28:26.000000 fastsql-1.0.0/fastsql.egg-info/dependency_links.txt
--rw-rw-r--   0 jhoward   (1002) jhoward   (1002)       20 2020-09-05 17:28:26.000000 fastsql-1.0.0/fastsql.egg-info/entry_points.txt
--rw-rw-r--   0 jhoward   (1002) jhoward   (1002)        1 2019-07-21 23:47:55.000000 fastsql-1.0.0/fastsql.egg-info/not-zip-safe
--rw-rw-r--   0 jhoward   (1002) jhoward   (1002)       41 2020-09-05 17:28:26.000000 fastsql-1.0.0/fastsql.egg-info/requires.txt
--rw-rw-r--   0 jhoward   (1002) jhoward   (1002)        8 2020-09-05 17:28:26.000000 fastsql-1.0.0/fastsql.egg-info/top_level.txt
--rw-rw-r--   0 jhoward   (1002) jhoward   (1002)       38 2020-09-05 17:28:26.000000 fastsql-1.0.0/setup.cfg
--rw-rw-r--   0 jhoward   (1002) jhoward   (1002)     2516 2020-09-05 17:08:59.000000 fastsql-1.0.0/setup.py
+drwxr-xr-x   0 jhoward    (501) staff       (20)        0 2024-05-27 17:02:07.027794 fastsql-1.0.1/
+-rw-rw-r--   0 jhoward    (501) staff       (20)    11337 2023-04-27 10:12:58.000000 fastsql-1.0.1/LICENSE
+-rw-rw-r--   0 jhoward    (501) staff       (20)      111 2023-04-27 10:12:58.000000 fastsql-1.0.1/MANIFEST.in
+-rw-r--r--   0 jhoward    (501) staff       (20)     2763 2024-05-27 17:02:07.027614 fastsql-1.0.1/PKG-INFO
+-rw-r--r--   0 jhoward    (501) staff       (20)     1917 2024-05-26 01:36:26.000000 fastsql-1.0.1/README.md
+drwxr-xr-x   0 jhoward    (501) staff       (20)        0 2024-05-27 17:02:07.026444 fastsql-1.0.1/fastsql/
+-rw-r--r--   0 jhoward    (501) staff       (20)       43 2024-05-27 16:58:30.000000 fastsql-1.0.1/fastsql/__init__.py
+-rw-r--r--   0 jhoward    (501) staff       (20)     1355 2024-05-27 16:58:30.000000 fastsql-1.0.1/fastsql/_modidx.py
+-rw-r--r--   0 jhoward    (501) staff       (20)     2293 2024-05-27 16:58:30.000000 fastsql-1.0.1/fastsql/core.py
+drwxr-xr-x   0 jhoward    (501) staff       (20)        0 2024-05-27 17:02:07.027384 fastsql-1.0.1/fastsql.egg-info/
+-rw-r--r--   0 jhoward    (501) staff       (20)     2763 2024-05-27 17:02:06.000000 fastsql-1.0.1/fastsql.egg-info/PKG-INFO
+-rw-r--r--   0 jhoward    (501) staff       (20)      324 2024-05-27 17:02:07.000000 fastsql-1.0.1/fastsql.egg-info/SOURCES.txt
+-rw-r--r--   0 jhoward    (501) staff       (20)        1 2024-05-27 17:02:06.000000 fastsql-1.0.1/fastsql.egg-info/dependency_links.txt
+-rw-r--r--   0 jhoward    (501) staff       (20)       36 2024-05-27 17:02:06.000000 fastsql-1.0.1/fastsql.egg-info/entry_points.txt
+-rw-r--r--   0 jhoward    (501) staff       (20)        1 2024-05-25 23:39:24.000000 fastsql-1.0.1/fastsql.egg-info/not-zip-safe
+-rw-r--r--   0 jhoward    (501) staff       (20)       30 2024-05-27 17:02:06.000000 fastsql-1.0.1/fastsql.egg-info/requires.txt
+-rw-r--r--   0 jhoward    (501) staff       (20)        8 2024-05-27 17:02:06.000000 fastsql-1.0.1/fastsql.egg-info/top_level.txt
+-rw-r--r--   0 jhoward    (501) staff       (20)      862 2024-05-27 16:58:22.000000 fastsql-1.0.1/settings.ini
+-rw-r--r--   0 jhoward    (501) staff       (20)       38 2024-05-27 17:02:07.027842 fastsql-1.0.1/setup.cfg
+-rw-r--r--   0 jhoward    (501) staff       (20)     2606 2024-05-26 01:43:58.000000 fastsql-1.0.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `fastsql-1.0.0/fastsql/__init__.py` & `fastsql-1.0.1/fastsql/core.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,52 +1,76 @@
-from fastcore.all import *
-import sqlalchemy, pandas as pd
-from sqlalchemy import create_engine,MetaData,Table,Column,engine,sql
-from sqlalchemy.sql.base import ImmutableColumnCollection
+# AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/00_core.ipynb.
 
-__all__ = 'pd conn_db patch'.split()
+# %% auto 0
+__all__ = ['old_md_dir', 'old_cc_dir', 'conn_db']
 
-def conn_db(drivername, username=None, password=None, host=None, port=None, database=None):
+# %% ../nbs/00_core.ipynb 2
+import sqlalchemy
+
+from fastcore.utils import *
+from fastcore.net import urlsave
+
+from collections import namedtuple
+from sqlalchemy import create_engine,text,MetaData,Table,Column,engine,sql
+from sqlalchemy.sql.base import ReadOnlyColumnCollection
+from sqlalchemy.engine.base import Connection
+from sqlalchemy.engine.cursor import CursorResult
+
+# %% ../nbs/00_core.ipynb 5
+def conn_db(connstr, **kwargs):
     "Connect to DB using `url.URL()` params and return filled `MetaData`"
-    eng= create_engine(engine.url.URL(drivername, username, password, host, port, database=database))
-    eng.connect()
-    meta = MetaData(bind=eng)
-    meta.reflect()
+    eng = create_engine(connstr, **kwargs)
+    conn = eng.connect()
+    meta = MetaData()
+    meta.reflect(bind=eng)
+    meta.bind = eng
+    meta.conn = conn
     return meta
 
-@patch
-def __getattr__(self:MetaData, n):
-    if n in self.tables: return self.tables[n],self.tables[n].c
-    raise AttributeError
+# %% ../nbs/00_core.ipynb 7
+old_md_dir = MetaData.__dir__
+old_cc_dir = ReadOnlyColumnCollection.__dir__
 
 @patch
-def __dir__(self:ImmutableColumnCollection, old_f): return old_f(self) + self.keys()
+def __dir__(self:MetaData): return old_md_dir(self) + list(self.tables)
+
 @patch
-def __dir__(self:MetaData,                  old_f): return old_f(self) + list(self.tables)
+def __dir__(self:ReadOnlyColumnCollection): return old_cc_dir(self) + self.keys()
 
+def _getattr_(self, n):
+    if n[0]=='_': raise AttributeError
+    if n in self.tables: return self.tables[n]
+    #return super().__getattr__(n)
+    raise AttributeError
+MetaData.__getattr__ = _getattr_
+
+# %% ../nbs/00_core.ipynb 11
 @patch
-def sql(self:engine.Engine, statement, *args, **kwargs):
-    "Execute `statement` string and return `DataFrame` of results (if any)"
-    t = self.execute(statement, *args, **kwargs)
-    if not t.cursor: return
-    return pd.DataFrame(t.fetchall(), columns=t.keys())
+def tuples(self:CursorResult, nm='Row'):
+    "Get all results as named tuples"
+    rs = self.mappings().fetchall()
+    nt = namedtuple(nm, self.keys())
+    return [nt(**o) for o in rs]
+
+@patch
+def sql(self:Connection, statement, nm='Row', *args, **kwargs):
+    "Execute `statement` string and return results (if any)"
+    if isinstance(statement,str): statement=text(statement)
+    t = self.execute(statement)
+    return t.tuples()
 
 @patch
 def sql(self:MetaData, statement, *args, **kwargs):
     "Execute `statement` string and return `DataFrame` of results (if any)"
-    return self.bind.sql(statement, *args, **kwargs)
+    return self.conn.sql(statement, *args, **kwargs)
 
+# %% ../nbs/00_core.ipynb 13
 @patch
-def df(self:engine.Engine, cmd):
-    "Execute SqlAlchemy `cmd` and return `DataFrame` of results"
-    return pd.read_sql(cmd, self)
+def get(self:Table, where=None, limit=None):
+    "Select from table, optionally limited by `where` and `limit` clauses"
+    return self.metadata.conn.sql(self.select().where(where).limit(limit))
 
+# %% ../nbs/00_core.ipynb 17
 @patch
-def df(self:MetaData, cmd):
-    "Execute SqlAlchemy `cmd` and return `DataFrame` of results"
-    return self.bind.df(cmd)
-
-@patch
-def df(self:Table, where=None, limit=None):
-    "`DataFrame` of table, optitionally limited by `where` and `limit` clauses"
-    return self.bind.df(self.select(where).limit(limit))
-
+def close(self:MetaData):
+    "Close the connection"
+    self.conn.close()
```

### Comparing `fastsql-1.0.0/setup.py` & `fastsql-1.0.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,55 +1,57 @@
 from pkg_resources import parse_version
 from configparser import ConfigParser
-import setuptools
-import re
+import setuptools, shlex
 assert parse_version(setuptools.__version__)>=parse_version('36.2')
 
 # note: all settings are in settings.ini; edit there, not here
 config = ConfigParser(delimiters=['='])
-config.read('settings.ini')
+config.read('settings.ini', encoding='utf-8')
 cfg = config['DEFAULT']
 
 cfg_keys = 'version description keywords author author_email'.split()
 expected = cfg_keys + "lib_name user branch license status min_python audience language".split()
 for o in expected: assert o in cfg, "missing expected setting: {}".format(o)
 setup_cfg = {o:cfg[o] for o in cfg_keys}
 
 licenses = {
     'apache2': ('Apache Software License 2.0','OSI Approved :: Apache Software License'),
+    'mit': ('MIT License', 'OSI Approved :: MIT License'),
+    'gpl2': ('GNU General Public License v2', 'OSI Approved :: GNU General Public License v2 (GPLv2)'),
+    'gpl3': ('GNU General Public License v3', 'OSI Approved :: GNU General Public License v3 (GPLv3)'),
+    'bsd3': ('BSD License', 'OSI Approved :: BSD License'),
 }
 statuses = [ '1 - Planning', '2 - Pre-Alpha', '3 - Alpha',
     '4 - Beta', '5 - Production/Stable', '6 - Mature', '7 - Inactive' ]
-py_versions = '2.0 2.1 2.2 2.3 2.4 2.5 2.6 2.7 3.0 3.1 3.2 3.3 3.4 3.5 3.6 3.7 3.8'.split()
-min_python = cfg['min_python']
-lic = licenses[cfg['license']]
+py_versions = '3.6 3.7 3.8 3.9 3.10 3.11 3.12'.split()
 
-requirements = ['pip', 'packaging']
-if cfg.get('requirements'): requirements += cfg.get('requirements','').split()
-if cfg.get('pip_requirements'): requirements += cfg.get('pip_requirements','').split()
-
-long_description = open('README.md').read()
-# ![png](docs/images/output_13_0.png)
-for ext in ['png', 'svg']:
-    long_description = re.sub(r'!\['+ext+'\]\((.*)\)', '!['+ext+']('+'https://raw.githubusercontent.com/{}/{}'.format(cfg['user'],cfg['lib_name'])+'/'+cfg['branch']+'/\\1)', long_description)
-    long_description = re.sub(r'src=\"(.*)\.'+ext+'\"', 'src=\"https://raw.githubusercontent.com/{}/{}'.format(cfg['user'],cfg['lib_name'])+'/'+cfg['branch']+'/\\1.'+ext+'\"', long_description)
+requirements = shlex.split(cfg.get('requirements', ''))
+if cfg.get('pip_requirements'): requirements += shlex.split(cfg.get('pip_requirements', ''))
+min_python = cfg['min_python']
+lic = licenses.get(cfg['license'].lower(), (cfg['license'], None))
+dev_requirements = (cfg.get('dev_requirements') or '').split()
 
 setuptools.setup(
     name = cfg['lib_name'],
     license = lic[0],
     classifiers = [
         'Development Status :: ' + statuses[int(cfg['status'])],
         'Intended Audience :: ' + cfg['audience'].title(),
-        'License :: ' + lic[1],
         'Natural Language :: ' + cfg['language'].title(),
-    ] + ['Programming Language :: Python :: '+o for o in py_versions[py_versions.index(min_python):]],
-    url = cfg['git_url'], 
+    ] + ['Programming Language :: Python :: '+o for o in py_versions[py_versions.index(min_python):]] + (['License :: ' + lic[1] ] if lic[1] else []),
+    url = cfg['git_url'],
     packages = setuptools.find_packages(),
     include_package_data = True,
     install_requires = requirements,
+    extras_require={ 'dev': dev_requirements },
+    dependency_links = cfg.get('dep_links','').split(),
     python_requires  = '>=' + cfg['min_python'],
-    long_description = long_description,
+    long_description = open('README.md', encoding='utf-8').read(),
     long_description_content_type = 'text/markdown',
     zip_safe = False,
-    entry_points = { 'console_scripts': cfg.get('console_scripts','').split() },
+    entry_points = {
+        'console_scripts': cfg.get('console_scripts','').split(),
+        'nbdev': [f'{cfg.get("lib_path")}={cfg.get("lib_path")}._modidx:d']
+    },
     **setup_cfg)
 
+
```

