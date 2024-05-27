# Comparing `tmp/fh_fablib-1.0.20240517.1.tar.gz` & `tmp/fh_fablib-1.0.20240527.tar.gz`

## Comparing `fh_fablib-1.0.20240517.1.tar` & `fh_fablib-1.0.20240527.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240517.1/.editorconfig
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240517.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0    21621 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240517.1/CHANGELOG.rst
--rwxr-xr-x   0        0        0      364 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240517.1/bumpversion.sh
--rw-r--r--   0        0        0    27027 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240517.1/fh_fablib/__init__.py
--rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240517.1/fh_fablib/extract_js_gettext_strings.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240517.1/fh_fablib/dotfiles/.editorconfig
--rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240517.1/fh_fablib/dotfiles/.pre-commit-config.yaml
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240517.1/fh_fablib/dotfiles/biome.json
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240517.1/fh_fablib/dotfiles/pyproject.toml
--rw-r--r--   0        0        0     6465 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240517.1/fh_fablib/dotfiles/webpack.library.js
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240517.1/.gitignore
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240517.1/LICENSE
--rw-r--r--   0        0        0     7326 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240517.1/README.rst
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240517.1/pyproject.toml
--rw-r--r--   0        0        0     7730 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240517.1/PKG-INFO
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240527/.editorconfig
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240527/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    21743 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240527/CHANGELOG.rst
+-rwxr-xr-x   0        0        0      364 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240527/bumpversion.sh
+-rw-r--r--   0        0        0    27098 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240527/fh_fablib/__init__.py
+-rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240527/fh_fablib/extract_js_gettext_strings.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240527/fh_fablib/dotfiles/.editorconfig
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240527/fh_fablib/dotfiles/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240527/fh_fablib/dotfiles/biome.json
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240527/fh_fablib/dotfiles/pyproject.toml
+-rw-r--r--   0        0        0     6465 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240527/fh_fablib/dotfiles/webpack.library.js
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240527/.gitignore
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240527/LICENSE
+-rw-r--r--   0        0        0     7362 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240527/README.rst
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240527/pyproject.toml
+-rw-r--r--   0        0        0     7764 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240527/PKG-INFO
```

### Comparing `fh_fablib-1.0.20240517.1/.pre-commit-config.yaml` & `fh_fablib-1.0.20240527/.pre-commit-config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
       - id: check-toml
       - id: check-yaml
       - id: detect-private-key
       - id: end-of-file-fixer
       - id: mixed-line-ending
       - id: trailing-whitespace
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: "v0.4.4"
+    rev: "v0.4.5"
     hooks:
       - id: ruff
       - id: ruff-format
   - repo: https://github.com/pre-commit/mirrors-prettier
     rev: v3.1.0
     hooks:
       - id: prettier
```

### Comparing `fh_fablib-1.0.20240517.1/CHANGELOG.rst` & `fh_fablib-1.0.20240527/CHANGELOG.rst`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,21 @@
 Change log
 ==========
 
 Next version
 ~~~~~~~~~~~~
 
 
+1.0.20240527
+~~~~~~~~~~~~
+
+- Switched to ``uv``. Install it using ``pipx install uv`` if you haven't done
+  so already.
+
+
 1.0.20240517.1
 ~~~~~~~~~~~~~~
 
 - Improved the ``*.pyc`` deletion stage by skipping potentially big folders
   which should never contain those files.
 - Skipped freezing more Python packaging libraries.
```

### Comparing `fh_fablib-1.0.20240517.1/fh_fablib/__init__.py` & `fh_fablib-1.0.20240527/fh_fablib/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from fabric import Connection, task
 from invoke import Collection  # noqa: F401
 from speckenv_django import django_database_url
 
 from fh_fablib.extract_js_gettext_strings import generate_strings
 
 
-__version__ = "1.0.20240517.1"
+__version__ = "1.0.20240527"
 
 
 # I don't care, in this context.
 warnings.simplefilter("ignore", category=ResourceWarning)
 
 
 def ansi(code):
@@ -89,15 +89,18 @@
                 else line
                 for line in old.splitlines(keepends=True)
             )
             if new != old:
                 path.write_text(new)
                 _update_dotfiles()
                 warning(
-                    "The fabfile and dotfiles have been updated automatically.\n\nPlease check the result twice before committing!"
+                    "The fabfile and dotfiles have been updated automatically.\n\n"
+                    "*******************************************\n"
+                    "PLEASE CHECK THE RESULTS BEFORE COMMITTING!\n"
+                    "*******************************************\n"
                 )
 
 
 def run(c, *a, **kw):
     """A Context.run or Connection.run with better defaults"""
     kw.setdefault("pty", False)
     kw.setdefault("replace_env", True)
@@ -227,25 +230,25 @@
 def dev(ctx, host="127.0.0.1", port=8000):
     """Run the development server for the frontend and backend"""
     progress(f"Starting server at http://{host}:{port}/")
     backend = random.randint(50000, 60000)
     _concurrently(
         ctx,
         [
-            f"venv/bin/python manage.py runserver {backend}",
+            f".venv/bin/python manage.py runserver {backend}",
             f"yarn run webpack serve --hot --host {host} --port {port} --env backend={backend}",
         ],
     )
 
 
 def _old_dev(ctx, host="127.0.0.1", port=8000):
     _concurrently(
         ctx,
         [
-            f"venv/bin/python manage.py runserver 0.0.0.0:{port}",
+            f".venv/bin/python manage.py runserver 0.0.0.0:{port}",
             f'HOST="{host}" yarn run webpack-dev-server --host 0.0.0.0 --port 4000 --hot',
         ],
     )
 
 
 @task(auto_shortflags=False)
 def pull_db(ctx, extra_dump_args=""):
@@ -280,15 +283,15 @@
 @task
 def reset_pw(ctx):
     """Set all user passwords to "password" """
     # 'password' encoded with a constant salt. Does not force a login after pull_db
     pw = r"pbkdf2_sha256\$320000\$2Hz1pcncCTWtqEnr3uoBdD\$nVc9Fka1oYQHFgGRGLUC4Nw3w6+ZmdO0IDdZOow+kJ0="
     run_local(
         ctx,
-        f"venv/bin/python manage.py shell -c \"pw='{pw}';"
+        f".venv/bin/python manage.py shell -c \"pw='{pw}';"
         f"from django.contrib.auth import get_user_model as g;"
         f'g()._base_manager.update(password=pw)"',
     )
 
 
 @task
 def reset_sq(ctx):
@@ -352,97 +355,89 @@
     with open("conf/strings.js", "w", encoding="utf-8") as f:
         f.write("/* eslint-disable */\n")
         f.write("".join(f"{string}\n" for string in generate_strings()))
 
     language = f"-l {language}" if language else "-a"
     run_local(
         ctx,
-        f"venv/bin/python manage.py makemessages {language} --add-location file"
-        " -i venv -i htmlcov -i node_modules -i lib -i build -i dist --no-wrap",
+        f".venv/bin/python manage.py makemessages {language} --add-location file"
+        " -i .venv -i htmlcov -i node_modules -i lib -i build -i dist --no-wrap",
         replace_env=False,
     )
     run_local(
         ctx,
-        f"venv/bin/python manage.py makemessages {language} --add-location file"
-        " -i venv -i htmlcov -i node_modules -i lib -i build -i dist --no-wrap"
+        f".venv/bin/python manage.py makemessages {language} --add-location file"
+        " -i .venv -i htmlcov -i node_modules -i lib -i build -i dist --no-wrap"
         " -d djangojs",
         replace_env=False,
     )
 
 
 @task
 def cm(ctx):
     """Compile the translation catalogs"""
     run_local(
         ctx,
-        "venv/bin/python manage.py compilemessages"
-        " -i venv -i htmlcov -i node_modules -i lib -i build -i dist",
+        ".venv/bin/python manage.py compilemessages"
+        " -i .venv -i htmlcov -i node_modules -i lib -i build -i dist",
         replace_env=False,
     )
 
 
 def _python3():
     interpreters = ("python3.12", "python3.11", "python3.10", "python3.9")
     return next(filter(None, (shutil.which(v) for v in interpreters)))
 
 
-def _pip_up(c):
-    run(c, "venv/bin/python -m pip install -U pip wheel setuptools")
-
-
 @task(
     auto_shortflags=False,
     help={
         "keep": "Keep the existing virtualenv",
         "stable": "Avoid pre-release versions of packages",
     },
 )
 def upgrade(ctx, keep=False, stable=False):
     """Re-create the virtualenv with newest versions of all libraries"""
-    venv = config.base / "venv"
+    venv = config.base / ".venv"
     if not venv.exists() or not keep:
-        run_local(ctx, f"rm -rf venv && {_python3()} -m venv venv")
-    _pip_up(ctx)
+        run_local(ctx, f"rm -rf .venv && uv venv --python {_python3()}")
     extra = "" if stable else "--pre"
-    run_local(
-        ctx, f"venv/bin/python -m pip install -U -r requirements-to-freeze.txt {extra}"
-    )
+    run_local(ctx, f"uv pip install -U -r requirements-to-freeze.txt {extra}")
     freeze(ctx)
     run_local(ctx, "pre-commit install -f")
 
 
 @task
 def freeze(ctx):
     """Freeze the virtualenv's state"""
     run_local(
         ctx,
         '(printf "# AUTOGENERATED, DO NOT EDIT\n\n";'
-        "venv/bin/python -m pip freeze -l"
-        ' | grep -vE "(^packaging==|^pkg.resources==|^setuptools==|^wheel==)"'
+        "uv pip freeze"
+        ' | grep -vE "(^packaging==|^pip==|^pkg.resources==|^setuptools==|^wheel==)"'
         ") > requirements.txt",
     )
 
 
 @task
 def update(ctx):
     """Update virtualenv and node_modules to match the lockfiles"""
-    venv = config.base / "venv"
+    venv = config.base / ".venv"
     if not venv.exists():
-        run_local(ctx, f"{_python3()} -m venv venv")
-    _pip_up(ctx)
+        run_local(ctx, f"uv venv --python {_python3()}")
     _concurrently(
         ctx,
         [
-            "venv/bin/python -m pip install -r requirements.txt",
+            "uv pip install -r requirements.txt",
             "git submodule update --init",
             'find . -name "*.pyc" -delete',
             "yarn",
         ],
     )
-    run_local(ctx, "venv/bin/python manage.py migrate", warn=True)
+    run_local(ctx, ".venv/bin/python manage.py migrate", warn=True)
     run_local(ctx, "pre-commit install -f")
 
 
 def _local_dotenv_if_not_exists():
     dotenv = config.base / ".env"
     if dotenv.exists():
         return
@@ -473,15 +468,15 @@
 @task(
     auto_shortflags=False,
     help={"clobber": "Clobber pre-existing node_modules and venv folders"},
 )
 def local(ctx, clobber=False):
     """Local environment setup"""
     if clobber:
-        run_local(ctx, "rm -rf node_modules venv")
+        run_local(ctx, "rm -rf node_modules .venv")
     dbname = _local_dbname()
     run_local(ctx, f"createdb {dbname}", warn=True)
     update(ctx)
 
 
 @task
 def nine_vhost(ctx):
@@ -713,15 +708,15 @@
     help={"python3": "Python executable"},
 )
 def nine_venv(ctx, python3="python3"):
     """Create a venv and install packages from requirements.txt"""
     with Connection(config.host) as conn, conn.cd(config.domain):
         run(conn, "rm -rf venv")
         run(conn, f"PATH=~/.pyenv/shims:$PATH {python3} -m venv venv")
-        _pip_up(conn)
+        run(conn, "venv/bin/python -m pip install -U pip")
         run(conn, "venv/bin/python -m pip install -r requirements.txt")
 
 
 @task
 def nine_reinit_from(ctx, environment):
     """Reinitialize an environment from a different environment"""
     try:
@@ -855,15 +850,15 @@
     run(conn, f"git reset --hard origin/{config.branch}")
     run(conn, "git submodule update --init")
     skip = "".join(
         f"-path {path} -prune -o "
         for path in ["./venv", "./static", "./media", "./.git", "./node_modules"]
     )
     run(conn, f'find . {skip} -name "*.pyc" -print | xargs rm -f')
-    _pip_up(conn)
+    run(conn, "venv/bin/python -m pip install -U pip")
     run(conn, "venv/bin/python -m pip install -r requirements.txt")
     run(conn, "venv/bin/python manage.py migrate")
     run(conn, "venv/bin/python manage.py check --deploy", warn=True)
 
 
 def _deploy_staticfiles(conn):
     run(conn, "venv/bin/python manage.py collectstatic --noinput")
```

### Comparing `fh_fablib-1.0.20240517.1/fh_fablib/extract_js_gettext_strings.py` & `fh_fablib-1.0.20240527/fh_fablib/extract_js_gettext_strings.py`

 * *Files identical despite different names*

### Comparing `fh_fablib-1.0.20240517.1/fh_fablib/dotfiles/.pre-commit-config.yaml` & `fh_fablib-1.0.20240527/fh_fablib/dotfiles/.pre-commit-config.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -16,41 +16,41 @@
       - id: file-contents-sorter
         args: [--ignore-case, --unique]
         files: requirements-to-freeze.txt
   - repo: local
     hooks:
       - id: django-check
         name: django check
-        entry: venv/bin/python manage.py check
+        entry: .venv/bin/python manage.py check
         pass_filenames: false
         language: system
         always_run: true
   - repo: https://github.com/adamchainz/django-upgrade
     rev: 1.17.0
     hooks:
       - id: django-upgrade
         args: [--target-version, "4.0"]
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: "v0.4.4"
+    rev: "v0.4.5"
     hooks:
       - id: ruff
       - id: ruff-format
   - repo: https://github.com/pre-commit/mirrors-prettier
     rev: v3.1.0
     hooks:
       - id: prettier
         args: [--list-different, --no-semi]
         types_or: [css, scss]
         exclude: "^conf/|.*\\.html$|.*\\.json$"
   - repo: https://github.com/tox-dev/pyproject-fmt
-    rev: 2.1.1
+    rev: 2.1.3
     hooks:
       - id: pyproject-fmt
   - repo: https://github.com/abravalheri/validate-pyproject
-    rev: v0.17
+    rev: v0.18
     hooks:
       - id: validate-pyproject
   - repo: https://github.com/biomejs/pre-commit
     rev: "v0.1.0"
     hooks:
       - id: biome-check
         additional_dependencies: ["@biomejs/biome@1.7.3"]
```

### Comparing `fh_fablib-1.0.20240517.1/fh_fablib/dotfiles/pyproject.toml` & `fh_fablib-1.0.20240527/fh_fablib/dotfiles/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fh_fablib-1.0.20240517.1/fh_fablib/dotfiles/webpack.library.js` & `fh_fablib-1.0.20240527/fh_fablib/dotfiles/webpack.library.js`

 * *Files identical despite different names*

### Comparing `fh_fablib-1.0.20240517.1/LICENSE` & `fh_fablib-1.0.20240527/LICENSE`

 * *Files identical despite different names*

### Comparing `fh_fablib-1.0.20240517.1/README.rst` & `fh_fablib-1.0.20240527/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -2,27 +2,28 @@
 fh-fablib
 =========
 
 Usage
 =====
 
 1. Install `pipx <https://pipxproject.github.io/pipx/>`__
-2. Install fh-fablib
+2. Install uv using ``pipx install uv``
+3. Install fh-fablib
 
    a. ``pipx install fh_fablib`` if you're happy with the packaged version
    b. ``pipx install ~/Projects/fh-fablib`` if you have a local git checkout
       you want to install from
 
-3. Add a ``fabfile.py`` to your project. A minimal example follows:
+4. Add a ``fabfile.py`` to your project. A minimal example follows:
 
    .. code-block:: python
 
        import fh_fablib as fl
 
-       fl.require("1.0.20240517.1")
+       fl.require("1.0.20240527")
        fl.config.update(host="www-data@feinheit06.nine.ch")
 
        environments = [
            fl.environment(
                "production",
                {
                    "domain": "example.com",
@@ -31,19 +32,19 @@
                },
                aliases=["p"],
            ),
        ]
 
        ns = fl.Collection(*fl.GENERAL, *fl.NINE, *environments)
 
-4. Run ``fl hook`` to provide a default `pre-commit
+5. Run ``fl hook`` to provide a default `pre-commit
    <https://pre-commit.com/>`__ configuration (or ``fl hook --force`` to
    override the dotfiles).
 
-5. Run ``fl --list`` to get a list of commands.
+6. Run ``fl --list`` to get a list of commands.
 
 
 Configuration values
 ====================
 
 - ``app = "app"``: Name of primary Django app containing settings, assets etc.
 - ``base``: ``pathlib.Path`` object pointing to the base dir of the project.
@@ -90,15 +91,15 @@
 
 If you need multiple environments, add environment tasks as follows:
 
 .. code-block:: python
 
     import fh_fablib as fl
 
-    fl.require("1.0.20240517.1")
+    fl.require("1.0.20240527")
     fl.config.update(host="www-data@feinheit06.nine.ch")
 
     environments = [
         fl.environment(
             "production",
             {
                 "domain": "example.com",
```

### Comparing `fh_fablib-1.0.20240517.1/pyproject.toml` & `fh_fablib-1.0.20240527/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fh_fablib-1.0.20240517.1/PKG-INFO` & `fh_fablib-1.0.20240527/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: fh-fablib
-Version: 1.0.20240517.1
+Version: 1.0.20240527
 Summary: fh-fablib
 Project-URL: Homepage, https://github.com/feinheit/fh-fablib/
 Author-email: Matthias Kestenholz <mk@feinheit.ch>
 License: BSD-3-Clause
 License-File: LICENSE
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >=3.9
@@ -16,27 +16,28 @@
 fh-fablib
 =========
 
 Usage
 =====
 
 1. Install `pipx <https://pipxproject.github.io/pipx/>`__
-2. Install fh-fablib
+2. Install uv using ``pipx install uv``
+3. Install fh-fablib
 
    a. ``pipx install fh_fablib`` if you're happy with the packaged version
    b. ``pipx install ~/Projects/fh-fablib`` if you have a local git checkout
       you want to install from
 
-3. Add a ``fabfile.py`` to your project. A minimal example follows:
+4. Add a ``fabfile.py`` to your project. A minimal example follows:
 
    .. code-block:: python
 
        import fh_fablib as fl
 
-       fl.require("1.0.20240517.1")
+       fl.require("1.0.20240527")
        fl.config.update(host="www-data@feinheit06.nine.ch")
 
        environments = [
            fl.environment(
                "production",
                {
                    "domain": "example.com",
@@ -45,19 +46,19 @@
                },
                aliases=["p"],
            ),
        ]
 
        ns = fl.Collection(*fl.GENERAL, *fl.NINE, *environments)
 
-4. Run ``fl hook`` to provide a default `pre-commit
+5. Run ``fl hook`` to provide a default `pre-commit
    <https://pre-commit.com/>`__ configuration (or ``fl hook --force`` to
    override the dotfiles).
 
-5. Run ``fl --list`` to get a list of commands.
+6. Run ``fl --list`` to get a list of commands.
 
 
 Configuration values
 ====================
 
 - ``app = "app"``: Name of primary Django app containing settings, assets etc.
 - ``base``: ``pathlib.Path`` object pointing to the base dir of the project.
@@ -104,15 +105,15 @@
 
 If you need multiple environments, add environment tasks as follows:
 
 .. code-block:: python
 
     import fh_fablib as fl
 
-    fl.require("1.0.20240517.1")
+    fl.require("1.0.20240527")
     fl.config.update(host="www-data@feinheit06.nine.ch")
 
     environments = [
         fl.environment(
             "production",
             {
                 "domain": "example.com",
```

