# Comparing `tmp/dkdc-0.5.0.tar.gz` & `tmp/dkdc-0.6.0.tar.gz`

## Comparing `dkdc-0.5.0.tar` & `dkdc-0.6.0.tar`

### file list

```diff
@@ -1,17 +1,26 @@
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 dkdc-0.5.0/dev-requirements.txt
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 dkdc-0.5.0/justfile
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 dkdc-0.5.0/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dkdc-0.5.0/src/dkdc/__init__.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 dkdc-0.5.0/src/dkdc/ai.py
--rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 dkdc-0.5.0/src/dkdc/cli.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 dkdc-0.5.0/src/dkdc/config.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 dkdc-0.5.0/src/dkdc/defaults.py
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 dkdc-0.5.0/src/dkdc/image.py
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 dkdc-0.5.0/src/dkdc/open.py
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 dkdc-0.5.0/src/dkdc/utils/config.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 dkdc-0.5.0/src/dkdc/utils/envvar.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 dkdc-0.5.0/.gitignore
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 dkdc-0.5.0/LICENSE
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 dkdc-0.5.0/pyproject.toml
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 dkdc-0.5.0/readme.md
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 dkdc-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 dkdc-0.6.0/dev-requirements.txt
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 dkdc-0.6.0/justfile
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dkdc-0.6.0/untitled.ipynb
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 dkdc-0.6.0/src/dkdc/__init__.py
+-rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 dkdc-0.6.0/src/dkdc/defaults.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 dkdc-0.6.0/src/dkdc/ai/__init__.py
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 dkdc-0.6.0/src/dkdc/ai/models.py
+-rw-r--r--   0        0        0     5883 2020-02-02 00:00:00.000000 dkdc-0.6.0/src/dkdc/ai/openai.py
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 dkdc-0.6.0/src/dkdc/ai/systems.py
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 dkdc-0.6.0/src/dkdc/ai/tokenize.py
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 dkdc-0.6.0/src/dkdc/cli/__init__.py
+-rw-r--r--   0        0        0     2794 2020-02-02 00:00:00.000000 dkdc-0.6.0/src/dkdc/cli/ai.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 dkdc-0.6.0/src/dkdc/cli/config.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 dkdc-0.6.0/src/dkdc/cli/console.py
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 dkdc-0.6.0/src/dkdc/cli/image.py
+-rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 dkdc-0.6.0/src/dkdc/cli/open.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 dkdc-0.6.0/src/dkdc/cli/tokenize.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 dkdc-0.6.0/src/dkdc/utils/__init__.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 dkdc-0.6.0/src/dkdc/utils/config.py
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 dkdc-0.6.0/src/dkdc/utils/filesystem.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 dkdc-0.6.0/src/dkdc/utils/vars.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 dkdc-0.6.0/.gitignore
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 dkdc-0.6.0/LICENSE
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 dkdc-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 dkdc-0.6.0/readme.md
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 dkdc-0.6.0/PKG-INFO
```

### Comparing `dkdc-0.5.0/justfile` & `dkdc-0.6.0/justfile`

 * *Files identical despite different names*

### Comparing `dkdc-0.5.0/src/dkdc/cli.py` & `dkdc-0.6.0/src/dkdc/cli/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,94 +1,107 @@
 # imports
 import typer
 
 ## local imports
-from dkdc.ai import tokenize_it
-from dkdc.open import open_it, list_things
-from dkdc.image import resize_image
-from dkdc.config import config_it
+from dkdc.cli.ai import run_ai
+from dkdc.cli.open import open_it, list_things
+from dkdc.cli.image import resize_image, convert_image
+from dkdc.cli.config import config_it
+from dkdc.cli.tokenize import tokenize_it
 
 # typer config
 ## default kwargs
 default_kwargs = {
     "no_args_is_help": True,
     "add_completion": False,
     "context_settings": {"help_option_names": ["-h", "--help"]},
 }
 
 ## main app
 app = typer.Typer(help="dkdc", **default_kwargs)
 
 ## subcommands
-ai_app = typer.Typer(help="ai subcommands", **default_kwargs)
 image_app = typer.Typer(help="image subcommands", **default_kwargs)
 
 ## add subcommands
-app.add_typer(ai_app, name="ai")
 app.add_typer(image_app, name="image")
 
 ## add subcommand aliases
-app.add_typer(ai_app, name="ml", hidden=True)
 app.add_typer(image_app, name="i", hidden=True)
 
 
 # commands
 @app.command()
+@app.command("ml", hidden=True)
+def ai():
+    """
+    chat with ai
+    """
+    run_ai()
+
+
+@app.command()
 @app.command("c", hidden=True)
 def config(
-    vim: bool = typer.Option(False, "--vim", "-v", help="Open with (n)vim."),
-    env: bool = typer.Option(False, "--env", "-e", help="Open .env file."),
+    vim: bool = typer.Option(False, "--vim", "-v", help="open with (n)vim"),
+    env: bool = typer.Option(False, "--env", "-e", help="open .env file"),
 ):
     """
     open config file(s)
     """
     config_it(vim, env)
 
 
 @app.command()
 @app.command("o", hidden=True)
 def open(
-    thing: str = typer.Argument(None, help="Thing to open."),
+    thing: str = typer.Argument(None, help="thing to open"),
 ):
     """
     open thing
     """
     if thing is None:
         list_things()
     else:
         open_it(thing)
 
 
-## image commands
-@ai_app.command()
-@ai_app.command("t", hidden=True)
-def tokenize(text: str = typer.Argument(..., help="Text to tokenize.")):
+@app.command()
+@app.command("t", hidden=True)
+def tokenize(text: str = typer.Argument(..., help="text to tokenize")):
     """
     tokenize text
     """
-    tokens = tokenize_it(text)
-    print(text, end=" -> ")
-    print(tokens)
+    tokenize_it(text)
 
 
+## image commands
 @image_app.command()
+@image_app.command("r", hidden=True)
 def resize(
     input_path: str = typer.Argument("thumbnail.png"),
     output_path: str = typer.Argument("resized.png"),
-    height: int = typer.Option(256, "--height", "-H", help="Height of the image."),
-    width: int = typer.Option(256, "--width", "-W", help="Width of the image."),
+    height: int = typer.Option(256, "--height", "-H", help="height of the image"),
+    width: int = typer.Option(256, "--width", "-W", help="width of the image"),
 ):
     """
     resize an image
     """
     resize_image(input_path, output_path, height, width)
 
 
-# main
-@app.callback()
-def cli():
-    return
+@image_app.command()
+@image_app.command("c", hidden=True)
+def convert(
+    input_path: str = typer.Argument(..., help="input path"),
+    output_path: str = typer.Option(None, "--output", "-o", help="output path"),
+    output_format: str = typer.Option("png", "--format", "-f", help="output format"),
+):
+    """
+    convert an image
+    """
+    convert_image(input_path, output_path=output_path, output_format=output_format)
 
 
 # main
 if __name__ == "__main__":
-    typer.run(cli)
+    typer.run(app)
```

### Comparing `dkdc-0.5.0/LICENSE` & `dkdc-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dkdc-0.5.0/pyproject.toml` & `dkdc-0.6.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "dkdc"
-version = "0.5.0"
+version = "0.6.0"
 authors = [{ name = "Cody", email = "cody@dkdc.dev" }]
 description = "dkdc"
 readme = "readme.md"
 requires-python = ">=3.11"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
 ]
 dependencies = [
+  'cairosvg',
   'html2text',
   'httpx',
   'ibis-framework[duckdb]',
   'openai',
   'Pillow',
   'python-dotenv',
+  'rich',
   'tiktoken',
   'typer[all]',
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/lostmygithubaccount/dkdc"
 "Bug Tracker" = "https://github.com/lostmygithubaccount/dkdc/issues"
```

