# Comparing `tmp/factorio_randovania_mod-0.2.1.tar.gz` & `tmp/factorio_randovania_mod-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "factorio_randovania_mod-0.2.1.tar", last modified: Sun May 26 20:36:00 2024, max compression
+gzip compressed data, was "factorio_randovania_mod-0.3.0.tar", last modified: Mon May 27 10:16:25 2024, max compression
```

## Comparing `factorio_randovania_mod-0.2.1.tar` & `factorio_randovania_mod-0.3.0.tar`

### file list

```diff
@@ -1,54 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:36:00.761798 factorio_randovania_mod-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-26 20:35:51.000000 factorio_randovania_mod-0.2.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:36:00.757798 factorio_randovania_mod-0.2.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-26 20:35:51.000000 factorio_randovania_mod-0.2.1/.github/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-26 20:35:51.000000 factorio_randovania_mod-0.2.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:36:00.757798 factorio_randovania_mod-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-26 20:35:51.000000 factorio_randovania_mod-0.2.1/.github/workflows/python.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-26 20:35:51.000000 factorio_randovania_mod-0.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-26 20:35:51.000000 factorio_randovania_mod-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-05-26 20:35:51.000000 factorio_randovania_mod-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-26 20:36:00.761798 factorio_randovania_mod-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-26 20:35:51.000000 factorio_randovania_mod-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-05-26 20:35:51.000000 factorio_randovania_mod-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 20:36:00.761798 factorio_randovania_mod-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:36:00.753798 factorio_randovania_mod-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:36:00.757798 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-26 20:35:51.000000 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-26 20:35:51.000000 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:36:00.761798 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/__pyinstaller/
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-26 20:35:51.000000 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/__pyinstaller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-26 20:35:51.000000 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/__pyinstaller/hook-factorio_randovania_mod.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-05-26 20:35:51.000000 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-26 20:35:51.000000 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/color_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-26 20:35:51.000000 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/configuration.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7133 2024-05-26 20:35:51.000000 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/creator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:36:00.761798 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/files/
--rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-05-26 20:35:51.000000 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/files/schema.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:36:00.761798 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/lua_src/
--rw-r--r--   0 runner    (1001) docker     (127)     5223 2024-05-26 20:35:51.000000 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/lua_src/control.lua
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-26 20:35:51.000000 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/lua_src/data-updates.lua
--rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-05-26 20:35:51.000000 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/lua_src/data.lua
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:36:00.753798 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/lua_src/graphics/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:36:00.761798 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/lua_src/graphics/icons/
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-26 20:35:51.000000 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/lua_src/graphics/icons/nothing.png
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-26 20:35:51.000000 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/lua_src/info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:36:00.753798 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/lua_src/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:36:00.761798 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/lua_src/locale/en/
--rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-05-26 20:35:51.000000 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/lua_src/locale/en/strings.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:36:00.761798 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/lua_src/prototypes/
--rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-05-26 20:35:51.000000 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/lua_src/prototypes/burners.lua
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-26 20:35:51.000000 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/lua_src/prototypes/extra-tiers.lua
--rw-r--r--   0 runner    (1001) docker     (127)     5525 2024-05-26 20:35:51.000000 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/lua_src/prototypes/tech.lua
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-26 20:35:51.000000 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/lua_util.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 20:35:51.000000 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-26 20:36:00.000000 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:36:00.761798 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-26 20:36:00.000000 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-26 20:36:00.000000 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 20:36:00.000000 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-26 20:36:00.000000 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-26 20:36:00.000000 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-26 20:36:00.000000 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:36:00.761798 factorio_randovania_mod-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-26 20:35:51.000000 factorio_randovania_mod-0.2.1/tests/test_color_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:16:25.545808 factorio_randovania_mod-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-27 10:16:20.000000 factorio_randovania_mod-0.3.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:16:25.533808 factorio_randovania_mod-0.3.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-27 10:16:20.000000 factorio_randovania_mod-0.3.0/.github/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-27 10:16:20.000000 factorio_randovania_mod-0.3.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:16:25.537808 factorio_randovania_mod-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-27 10:16:20.000000 factorio_randovania_mod-0.3.0/.github/workflows/python.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-27 10:16:20.000000 factorio_randovania_mod-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-27 10:16:20.000000 factorio_randovania_mod-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-05-27 10:16:20.000000 factorio_randovania_mod-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-27 10:16:25.545808 factorio_randovania_mod-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-27 10:16:20.000000 factorio_randovania_mod-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-05-27 10:16:20.000000 factorio_randovania_mod-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 10:16:25.545808 factorio_randovania_mod-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:16:25.533808 factorio_randovania_mod-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:16:25.537808 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-27 10:16:20.000000 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-27 10:16:20.000000 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:16:25.537808 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/__pyinstaller/
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-27 10:16:20.000000 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/__pyinstaller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-27 10:16:20.000000 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/__pyinstaller/hook-factorio_randovania_mod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-27 10:16:20.000000 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-05-27 10:16:20.000000 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/color_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-27 10:16:20.000000 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/configuration.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7044 2024-05-27 10:16:20.000000 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/creator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:16:25.537808 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/files/
+-rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-05-27 10:16:20.000000 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/files/schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-05-27 10:16:20.000000 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/locale_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:16:25.541808 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/lua_src/
+-rw-r--r--   0 runner    (1001) docker     (127)     5223 2024-05-27 10:16:20.000000 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/lua_src/control.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-27 10:16:20.000000 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/lua_src/data-updates.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-05-27 10:16:20.000000 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/lua_src/data.lua
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:16:25.533808 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/lua_src/graphics/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:16:25.541808 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/lua_src/graphics/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-27 10:16:20.000000 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/lua_src/graphics/icons/nothing.png
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-27 10:16:20.000000 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/lua_src/info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:16:25.533808 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/lua_src/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:16:25.541808 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/lua_src/locale/en/
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-05-27 10:16:20.000000 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/lua_src/locale/en/strings.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:16:25.541808 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/lua_src/prototypes/
+-rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-05-27 10:16:20.000000 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/lua_src/prototypes/burners.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-27 10:16:20.000000 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/lua_src/prototypes/extra-tiers.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     5525 2024-05-27 10:16:20.000000 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/lua_src/prototypes/tech.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-27 10:16:20.000000 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/lua_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-27 10:16:20.000000 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/mod_lua_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 10:16:20.000000 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-27 10:16:20.000000 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-27 10:16:25.000000 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:16:25.541808 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-27 10:16:25.000000 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-05-27 10:16:25.000000 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 10:16:25.000000 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-27 10:16:25.000000 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-27 10:16:25.000000 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-27 10:16:25.000000 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:16:25.541808 factorio_randovania_mod-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-27 10:16:20.000000 factorio_randovania_mod-0.3.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-27 10:16:20.000000 factorio_randovania_mod-0.3.0/tests/test_color_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-27 10:16:20.000000 factorio_randovania_mod-0.3.0/tests/test_creator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:16:25.541808 factorio_randovania_mod-0.3.0/tests/test_files/
+-rw-r--r--   0 runner    (1001) docker     (127)   117666 2024-05-27 10:16:20.000000 factorio_randovania_mod-0.3.0/tests/test_files/patcher_a.json
```

### Comparing `factorio_randovania_mod-0.2.1/.github/dependabot.yml` & `factorio_randovania_mod-0.3.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.2.1/.github/workflows/python.yml` & `factorio_randovania_mod-0.3.0/.github/workflows/python.yml`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.2.1/.gitignore` & `factorio_randovania_mod-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.2.1/.pre-commit-config.yaml` & `factorio_randovania_mod-0.3.0/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -7,12 +7,12 @@
     rev: v0.4.4
     hooks:
       - id: ruff
         args: [ --fix, --exit-non-zero-on-fix ]
       - id: ruff-format
 
 -   repo: https://github.com/henriquegemignani/jsonschema-to-typeddict
-    rev: v1.1
+    rev: v1.1.1
     hooks:
     -   id: jsonschema-to-typeddict
         files: src/factorio_randovania_mod/files/schema.json
         args: [ --output-path, src/factorio_randovania_mod/configuration.pyi, --root-name, Configuration ]
```

### Comparing `factorio_randovania_mod-0.2.1/LICENSE` & `factorio_randovania_mod-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.2.1/PKG-INFO` & `factorio_randovania_mod-0.3.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 Metadata-Version: 2.1
 Name: factorio-randovania-mod
-Version: 0.2.1
+Version: 0.3.0
 Summary: Generator of Factorio Randomizer mods for Randovania
 Author: Henrique Gemignani Passos Lima
 Project-URL: Homepage, https://github.com/randovania/factorio-randovania-mod
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pillow
 Requires-Dist: numpy
+Requires-Dist: jsonschema
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pytest-mock; extra == "test"
 Requires-Dist: pre-commit; extra == "test"
 Provides-Extra: typing
 Requires-Dist: mypy; extra == "typing"
 Requires-Dist: types-Pillow; extra == "typing"
+Requires-Dist: types-pyinstaller; extra == "typing"
+Requires-Dist: types-jsonschema; extra == "typing"
 
 # Factorio Randomizer
 
 This python package creates Factorio mod files that randomizes the game, based on a JSON file.
 Intended to be used by used by [Randovania](https://randovania.org/).
```

### Comparing `factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/cli.py` & `factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,20 +18,16 @@
     )
     parser.add_argument(
         "--output-path",
         required=True,
         type=Path,
         help="Path to where the mod files will be written to.",
     )
-    parser.add_argument(
-        "--input-json", required=True, type=Path, help="Path to the configuration json."
-    )
-    parser.add_argument(
-        "-q", "--quiet", action="store_true", help="Disables all info and debug logs."
-    )
+    parser.add_argument("--input-json", required=True, type=Path, help="Path to the configuration json.")
+    parser.add_argument("-q", "--quiet", action="store_true", help="Disables all info and debug logs.")
     return parser
 
 
 def setup_logging() -> None:
     handlers = {
         "default": {
             "level": "DEBUG",
```

### Comparing `factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/color_util.py` & `factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/color_util.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,16 @@
-import PIL.Image
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
+
 import numpy as np
+import PIL.Image
 
+if TYPE_CHECKING:
+    from pathlib import Path
 
 # Code copied from https://stackoverflow.com/a/7274986
 # It's licensed under CC BY-SA 3.0
 
 
 def rgb_to_hsv(rgb: np.ndarray) -> np.ndarray:
     # Translated from source of colorsys.rgb_to_hsv
@@ -22,17 +28,15 @@
     hsv[mask, 1] = (maxc - minc)[mask] / maxc[mask]
     rc = np.zeros_like(r)
     gc = np.zeros_like(g)
     bc = np.zeros_like(b)
     rc[mask] = (maxc - r)[mask] / (maxc - minc)[mask]
     gc[mask] = (maxc - g)[mask] / (maxc - minc)[mask]
     bc[mask] = (maxc - b)[mask] / (maxc - minc)[mask]
-    hsv[..., 0] = np.select(
-        [r == maxc, g == maxc], [bc - gc, 2.0 + rc - bc], default=4.0 + gc - rc
-    )
+    hsv[..., 0] = np.select([r == maxc, g == maxc], [bc - gc, 2.0 + rc - bc], default=4.0 + gc - rc)
     hsv[..., 0] = (hsv[..., 0] / 6.0) % 1.0
     return hsv
 
 
 def hsv_to_rgb(hsv: np.ndarray) -> np.ndarray:
     # Translated from source of colorsys.hsv_to_rgb
     # h,s should be a numpy arrays with values between 0.0 and 1.0
@@ -58,7 +62,15 @@
     arr = np.array(img.convert("RGBA"))
 
     hsv = rgb_to_hsv(arr)
     hsv[..., 0] = hue
     rgb = hsv_to_rgb(hsv)
 
     return PIL.Image.fromarray(rgb, "RGBA")
+
+
+def hue_shift(input_path: Path, output_path: Path, rotation: float) -> None:
+    """Creates a new image, by shifting the hue of the input image."""
+    img = PIL.Image.open(input_path)
+    new_img = shift_hue(img, rotation / 360.0)
+    output_path.parent.mkdir(parents=True, exist_ok=True)
+    new_img.save(output_path)
```

### Comparing `factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/configuration.pyi` & `factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/configuration.pyi`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/creator.py` & `factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/creator.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,86 +1,27 @@
 from __future__ import annotations
 
 import collections
 import configparser
-import os
 import shutil
 import typing
 from pathlib import Path
 
-import PIL.Image
-
-from factorio_randovania_mod import color_util
-from factorio_randovania_mod.lua_util import wrap_array_pretty, wrap
+from factorio_randovania_mod import schema
+from factorio_randovania_mod.color_util import hue_shift
+from factorio_randovania_mod.locale_lib import ensure_locale_read, get_from_locale
+from factorio_randovania_mod.lua_util import wrap, wrap_array_pretty
 
 if typing.TYPE_CHECKING:
-    from factorio_randovania_mod.configuration import Configuration
-
-
-def get_from_locale(locale: configparser.ConfigParser, group: str, n: str) -> str:
-    if n in locale[group]:
-        return locale[group][n]
-    if f"{n}-1" in locale[group]:
-        return locale[group][f"{n}-1"]
-
-    i = n.rfind("-")
-    if i != -1:
-        front, number = n[:i], n[i + 1 :]
-        if number.isdigit():
-            return get_from_locale(locale, group, front)
-
-    raise KeyError(n)
-
-
-def get_localized_name(locale: configparser.ConfigParser, n: str) -> str:
-    for k in [
-        "item-name",
-        "entity-name",
-        "fluid-name",
-        "equipment-name",
-        "recipe-name",
-        "technology-name",
-    ]:
-        if n in locale[k]:
-            return locale[k][n]
-        if f"{n}-1" in locale[k]:
-            return locale[k][f"{n}-1"]
-
-    if n.startswith("fill-"):
-        return f"Fill {locale['fluid-name'][n[5:-7]]} barrel"
-
-    if n.endswith("-barrel"):
-        return f"{locale['fluid-name'][n[:-7]]} barrel"
-
-    hardcoded_names = {
-        "solid-fuel-from-heavy-oil": "Solid Fuel (Heavy Oil)",
-        "solid-fuel-from-light-oil": "Solid Fuel (Light Oil)",
-        "solid-fuel-from-petroleum-gas": "Solid Fuel (Petroleum Gas)",
-    }
+    from factorio_randovania_mod.configuration import (
+        ConfigurationTechnologiesItem,
+    )
+    from factorio_randovania_mod.mod_lua_api import CustomTechTreeItem, GeneratedFiles
 
-    try:
-        return hardcoded_names[n]
-    except KeyError:
-        i = n.rfind("-")
-        if i != -1:
-            front, number = n[:i], n[i + 1 :]
-            if number.isdigit():
-                return f"{get_localized_name(locale, front)} {number}"
-        raise
-
-
-template_path = Path(__file__).parent.joinpath("lua_src")
-
-
-def hue_shift(input_path: Path, output_path: Path, rotation: float) -> None:
-    """Creates a new image, by shifting the hue of the input image."""
-    img = PIL.Image.open(input_path)
-    new_img = color_util.shift_hue(img, rotation / 360.0)
-    output_path.parent.mkdir(parents=True, exist_ok=True)
-    new_img.save(output_path)
+_TEMPLATE_PATH = Path(__file__).parent.joinpath("lua_src")
 
 
 def create_hue_shifted_images(factorio_path: Path, output_path: Path) -> None:
     lab_angle = 120.0
     assembler_angle = 310.0
 
     base_graphics_path = factorio_path.joinpath("data/base/graphics")
@@ -122,101 +63,148 @@
         hue_shift(
             base_graphics_path.joinpath(source_path),
             output_path.joinpath("graphics", target_path),
             rotation,
         )
 
 
-def ensure_locale_read(locale: configparser.ConfigParser, files: list[Path]) -> None:
-    filenames = [os.fspath(filename) for filename in files]
-    did_read = locale.read(filenames)
-    if did_read != filenames:
-        missing = set(filenames) - set(did_read)
-        raise FileNotFoundError(str(missing))
+def process_technology(
+    output_locale: configparser.ConfigParser,
+    local_unlocks: dict[str, list[str]],
+    progressive_sources: dict[tuple[str, ...], list[str]],
+    tech: ConfigurationTechnologiesItem,
+    source_locale: configparser.ConfigParser | None,
+) -> CustomTechTreeItem:
+    """
+    Process an entry of patch_data["technologies"]
+    :param output_locale:
+    :param local_unlocks:
+    :param progressive_sources:
+    :param tech:
+    :param source_locale:
+    :return: A new entry for tech-tree.lua
+    """
+    tech_name = tech["tech_name"]
+    output_locale["technology-name"][tech_name] = tech["locale_name"]
+    output_locale["technology-description"][tech_name] = tech["description"]
+
+    new_tech: CustomTechTreeItem = {
+        "name": tech_name,
+        "icon": tech["icon"],
+        "costs": {
+            "count": tech["cost"]["count"],
+            "time": tech["cost"]["time"],
+            "ingredients": [(it, 1) for it in tech["cost"]["ingredients"]],
+        },
+        "prerequisites": tech["prerequisites"] if tech["prerequisites"] else None,
+        # "fake_effects": tech["fake_effects"],
+    }
+    if "icon_size" in tech:
+        new_tech["icon_size"] = tech["icon_size"]
 
+    if len(tech["unlocks"]) == 1:
+        new_tech["take_effects_from"] = tech["unlocks"][0]
+        if source_locale is not None:
+            output_locale["technology-description"][tech_name] = get_from_locale(
+                source_locale, "technology-description", tech["unlocks"][0]
+            )
+    elif tech["unlocks"]:
+        local_unlocks[tech_name] = tech["unlocks"]
+        progressive_sources[tuple(tech["unlocks"])].append(tech_name)
+
+    return new_tech
+
+
+def generate_output(
+    output_path: Path,
+    generated_files: GeneratedFiles,
+    locale: configparser.ConfigParser,
+    factorio_path: Path | None,
+) -> None:
+    """
+    Generates all files for the mod.
+    :param output_path: Where to place the output
+    :param generated_files: Data for generating all lua files
+    :param locale: Used as template
+    :param factorio_path: Source for hue shifting the images
+    :return:
+    """
+    shutil.copytree(_TEMPLATE_PATH, output_path)
+    output_path.joinpath("generated").mkdir()
 
-def create(factorio_path: Path, patch_data: Configuration, output_folder: Path) -> None:
+    def generate_file(name: str, content: str) -> None:
+        output_path.joinpath("generated", name).write_text("return " + content)
+
+    generate_file("tech-tree.lua", wrap_array_pretty(generated_files["tech_tree"]))
+    generate_file("local-unlocks.lua", wrap(generated_files["local_unlocks"]))
+    generate_file("existing-tree-repurpose.lua", wrap(generated_files["existing_tree_repurpose"]))
+
+    generate_file("starting-tech.lua", wrap_array_pretty(generated_files["starting_tech"]))
+    generate_file("custom-recipes.lua", wrap_array_pretty(generated_files["custom_recipes"]))
+
+    with output_path.joinpath("locale/en/strings.cfg").open("w") as f:
+        locale.write(f, space_around_delimiters=False)
+
+    if factorio_path is not None:
+        create_hue_shifted_images(factorio_path, output_path)
+
+
+def create(factorio_path: Path | None, patch_data: dict, output_folder: Path) -> None:
     output_path = output_folder.joinpath("randovania-layout")
     shutil.rmtree(output_path, ignore_errors=True)
 
-    original_locale = configparser.ConfigParser()
-    ensure_locale_read(
-        original_locale,
-        [
-            factorio_path.joinpath("data/base/locale/en/base.cfg"),
-            template_path.joinpath("locale/en/strings.cfg"),
-        ],
-    )
+    configuration = schema.validate(patch_data)
+
+    original_locale: configparser.ConfigParser | None = None
+    if factorio_path is not None:
+        original_locale = configparser.ConfigParser()
+        ensure_locale_read(
+            original_locale,
+            [
+                factorio_path.joinpath("data/base/locale/en/base.cfg"),
+                _TEMPLATE_PATH.joinpath("locale/en/strings.cfg"),
+            ],
+        )
 
     locale = configparser.ConfigParser()
     ensure_locale_read(
         locale,
         [
-            template_path.joinpath("locale/en/strings.cfg"),
+            _TEMPLATE_PATH.joinpath("locale/en/strings.cfg"),
         ],
     )
 
-    tech_tree_lua = []
-    progressive_sources = collections.defaultdict(list)
-    local_unlocks = {}
-
-    for tech in patch_data["technologies"]:
-        tech_name = tech["tech_name"]
-        locale["technology-name"][tech_name] = tech["locale_name"]
-        locale["technology-description"][tech_name] = tech["description"]
-
-        new_tech: dict = {
-            "name": tech_name,
-            "icon": tech["icon"],
-            "costs": {
-                "count": tech["cost"]["count"],
-                "time": tech["cost"]["time"],
-                "ingredients": [[it, 1] for it in tech["cost"]["ingredients"]],
-            },
-            "prerequisites": tech["prerequisites"] if tech["prerequisites"] else None,
-            # "fake_effects": tech["fake_effects"],
-        }
-        if "icon_size" in tech:
-            new_tech["icon_size"] = tech["icon_size"]
-        tech_tree_lua.append(new_tech)
-
-        if len(tech["unlocks"]) == 1:
-            new_tech["take_effects_from"] = tech["unlocks"][0]
-            locale["technology-description"][tech_name] = get_from_locale(
-                original_locale, "technology-description", tech["unlocks"][0]
-            )
-        elif tech["unlocks"]:
-            local_unlocks[tech_name] = tech["unlocks"]
-            progressive_sources[tuple(tech["unlocks"])].append(tech_name)
+    progressive_sources: dict[tuple[str, ...], list[str]] = collections.defaultdict(list)
+    generated_files: GeneratedFiles = {
+        "tech_tree": [],
+        "local_unlocks": {},
+        "existing_tree_repurpose": {},
+        "starting_tech": configuration["starting_tech"],
+        "custom_recipes": configuration["recipes"],
+    }
 
-    existing_tree_repurpose = {}
+    for tech in configuration["technologies"]:
+        generated_files["tech_tree"].append(
+            process_technology(
+                locale,
+                generated_files["local_unlocks"],
+                progressive_sources,
+                tech,
+                original_locale,
+            )
+        )
 
     # TODO: add the offworld research to `existing_tree_repurpose`
 
     for progressive_sequence, sources in progressive_sources.items():
         for i, tech_name in enumerate(progressive_sequence):
             if i == 0:
                 prerequisites = sources
             else:
                 prerequisites = [progressive_sequence[i - 1]]
 
-            existing_tree_repurpose[tech_name] = {
+            generated_files["existing_tree_repurpose"][tech_name] = {
                 "science_pack": "impossible-science-pack",
                 "prerequisites": prerequisites,
             }
 
-    shutil.copytree(template_path, output_path)
-    output_path.joinpath("generated").mkdir()
-
-    def generate_file(name: str, content: str) -> None:
-        output_path.joinpath("generated", name).write_text("return " + content)
-
-    generate_file("tech-tree.lua", wrap_array_pretty(tech_tree_lua))
-    generate_file("local-unlocks.lua", wrap(local_unlocks))
-    generate_file("starting-tech.lua", wrap_array_pretty(patch_data["starting_tech"]))
-    generate_file("existing-tree-repurpose.lua", wrap(existing_tree_repurpose))
-    generate_file("custom-recipes.lua", wrap_array_pretty(patch_data["recipes"]))
-
-    create_hue_shifted_images(factorio_path, output_path)
-
-    with output_path.joinpath("locale/en/strings.cfg").open("w") as f:
-        locale.write(f, space_around_delimiters=False)
+    generate_output(output_path, generated_files, locale, factorio_path)
```

### Comparing `factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/files/schema.json` & `factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/files/schema.json`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/lua_src/control.lua` & `factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/lua_src/control.lua`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/lua_src/data-updates.lua` & `factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/lua_src/data-updates.lua`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/lua_src/data.lua` & `factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/lua_src/data.lua`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/lua_src/graphics/icons/nothing.png` & `factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/lua_src/graphics/icons/nothing.png`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/lua_src/locale/en/strings.cfg` & `factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/lua_src/locale/en/strings.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 regular-inserter-capacity-bonus=Allows non-stack inserters to move more items at once.
 stack-inserter-capacity-bonus=Allows stack inserters to move more items at once.
 steam-power=Source of electric energy by boiling water.
 oil-cracking=Refine the different oil products.
 big-electric-pole=Distribute electricity over long distances.
 gate=Wall sections that open up when needed. Can be controlled by the circuit network.
 long-handed-inserter=An electric inserter that picks up and places items two tiles from its location instead of the usual one.
+longer-handed-inserter=An electric inserter that picks up and places items three tiles from its location instead of the usual one.
 solid-fuel=A burnable fuel produced from the oil products.
 research-productivity=Improves the yield of your science packs, providing more research at no cost.
 
 [entity-name]
 burner-lab=Burner lab
 lab=Electric lab
 burner-assembling-machine=Burner assembling machine
@@ -32,8 +33,8 @@
 burner-lab=Burner lab
 lab=Electric lab
 burner-assembling-machine=Burner assembling machine
 impossible-science-pack=Unresearchable
 longer-handed-inserter=Longer-handed inserter
 
 [item-description]
-impossible-science-pack=This research is unlocked by researching something else.
+impossible-science-pack=This research is unlocked by researching something else.
```

### Comparing `factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/lua_src/prototypes/burners.lua` & `factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/lua_src/prototypes/burners.lua`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/lua_src/prototypes/extra-tiers.lua` & `factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/lua_src/prototypes/extra-tiers.lua`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/lua_src/prototypes/tech.lua` & `factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/lua_src/prototypes/tech.lua`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/lua_util.py` & `factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/lua_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,16 +19,15 @@
     if isinstance(data, list):
         return "{" + ", ".join(wrap(item, indent) for item in data) + "}"
 
     if isinstance(data, dict):
         return (
             "{\n"
             + "\n".join(
-                f"{indent}    {_dict_key(key)} = {wrap(value, f'{indent}    ')},"
-                for key, value in data.items()
+                f"{indent}    {_dict_key(key)} = {wrap(value, f'{indent}    ')}," for key, value in data.items()
             )
             + f"\n{indent}}}"
         )
 
     if isinstance(data, bool):
         return "true" if data else "false"
```

### Comparing `factorio_randovania_mod-0.2.1/src/factorio_randovania_mod.egg-info/PKG-INFO` & `factorio_randovania_mod-0.3.0/src/factorio_randovania_mod.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 Metadata-Version: 2.1
 Name: factorio-randovania-mod
-Version: 0.2.1
+Version: 0.3.0
 Summary: Generator of Factorio Randomizer mods for Randovania
 Author: Henrique Gemignani Passos Lima
 Project-URL: Homepage, https://github.com/randovania/factorio-randovania-mod
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pillow
 Requires-Dist: numpy
+Requires-Dist: jsonschema
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pytest-mock; extra == "test"
 Requires-Dist: pre-commit; extra == "test"
 Provides-Extra: typing
 Requires-Dist: mypy; extra == "typing"
 Requires-Dist: types-Pillow; extra == "typing"
+Requires-Dist: types-pyinstaller; extra == "typing"
+Requires-Dist: types-jsonschema; extra == "typing"
 
 # Factorio Randomizer
 
 This python package creates Factorio mod files that randomizes the game, based on a JSON file.
 Intended to be used by used by [Randovania](https://randovania.org/).
```

### Comparing `factorio_randovania_mod-0.2.1/src/factorio_randovania_mod.egg-info/SOURCES.txt` & `factorio_randovania_mod-0.3.0/src/factorio_randovania_mod.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -9,16 +9,19 @@
 .github/workflows/python.yml
 src/factorio_randovania_mod/__init__.py
 src/factorio_randovania_mod/__main__.py
 src/factorio_randovania_mod/cli.py
 src/factorio_randovania_mod/color_util.py
 src/factorio_randovania_mod/configuration.pyi
 src/factorio_randovania_mod/creator.py
+src/factorio_randovania_mod/locale_lib.py
 src/factorio_randovania_mod/lua_util.py
+src/factorio_randovania_mod/mod_lua_api.py
 src/factorio_randovania_mod/py.typed
+src/factorio_randovania_mod/schema.py
 src/factorio_randovania_mod/version.py
 src/factorio_randovania_mod.egg-info/PKG-INFO
 src/factorio_randovania_mod.egg-info/SOURCES.txt
 src/factorio_randovania_mod.egg-info/dependency_links.txt
 src/factorio_randovania_mod.egg-info/entry_points.txt
 src/factorio_randovania_mod.egg-info/requires.txt
 src/factorio_randovania_mod.egg-info/top_level.txt
@@ -30,8 +33,11 @@
 src/factorio_randovania_mod/lua_src/data.lua
 src/factorio_randovania_mod/lua_src/info.json
 src/factorio_randovania_mod/lua_src/graphics/icons/nothing.png
 src/factorio_randovania_mod/lua_src/locale/en/strings.cfg
 src/factorio_randovania_mod/lua_src/prototypes/burners.lua
 src/factorio_randovania_mod/lua_src/prototypes/extra-tiers.lua
 src/factorio_randovania_mod/lua_src/prototypes/tech.lua
-tests/test_color_util.py
+tests/conftest.py
+tests/test_color_util.py
+tests/test_creator.py
+tests/test_files/patcher_a.json
```

