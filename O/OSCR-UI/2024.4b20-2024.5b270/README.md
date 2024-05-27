# Comparing `tmp/oscr_ui-2024.4b20.tar.gz` & `tmp/oscr_ui-2024.5b270.tar.gz`

## Comparing `oscr_ui-2024.4b20.tar` & `oscr_ui-2024.5b270.tar`

### file list

```diff
@@ -1,68 +1,61 @@
--rw-r--r--   0        0        0     1886 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/.OSCR_settings.ini
--rw-r--r--   0        0        0       58 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/.flake8
--rw-r--r--   0        0        0       98 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/.pre-commit-config.yaml
--rw-r--r--   0        0        0    26538 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/main.py
--rw-r--r--   0        0        0      180 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/shell.nix
--rw-r--r--   0        0        0 105939534 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/~temp_log_files\[24-03-29_06-54-59--24-03-30_15-01-29]combatlog.log
--rw-r--r--   0        0        0 25252302 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/~temp_log_files\[24-03-30_15-08-23--24-03-30_20-19-03]combatlog.log
--rw-r--r--   0        0        0     1306 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/.github/workflows/build.yml
--rw-r--r--   0        0        0      214 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/OSCRUI/__init__.py
--rw-r--r--   0        0        0    58232 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/OSCRUI/app.py
--rw-r--r--   0        0        0     8916 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/OSCRUI/callbacks.py
--rw-r--r--   0        0        0    15450 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/OSCRUI/datafunctions.py
--rw-r--r--   0        0        0    15700 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/OSCRUI/datamodels.py
--rw-r--r--   0        0        0    14983 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/OSCRUI/displayer.py
--rw-r--r--   0        0        0     6127 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/OSCRUI/iofunctions.py
--rw-r--r--   0        0        0     9328 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/OSCRUI/leagueconnector.py
--rw-r--r--   0        0        0     5052 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/OSCRUI/style.py
--rw-r--r--   0        0        0    16622 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/OSCRUI/subwindows.py
--rw-r--r--   0        0        0     4131 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/OSCRUI/textedit.py
--rw-r--r--   0        0        0    14849 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/OSCRUI/widgetbuilder.py
--rw-r--r--   0        0        0    10447 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/OSCRUI/widgets.py
--rw-r--r--   0        0        0   170564 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/Overpass-Bold.ttf
--rw-r--r--   0        0        0   170328 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/Overpass-Medium.ttf
--rw-r--r--   0        0        0   170204 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/Overpass-Regular.ttf
--rw-r--r--   0        0        0    87172 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/RobotoMono-Medium.ttf
--rw-r--r--   0        0        0    87236 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/RobotoMono-Regular.ttf
--rw-r--r--   0        0        0      268 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/arrow-down.svg
--rw-r--r--   0        0        0      269 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/arrow-right.svg
--rw-r--r--   0        0        0      225 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/close.svg
--rw-r--r--   0        0        0      348 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/collapse-bottom.svg
--rw-r--r--   0        0        0      360 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/collapse-left.svg
--rw-r--r--   0        0        0      363 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/collapse-right.svg
--rw-r--r--   0        0        0      339 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/collapse-top.svg
--rw-r--r--   0        0        0      319 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/copy.svg
--rw-r--r--   0        0        0      345 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/expand-bottom.svg
--rw-r--r--   0        0        0      362 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/expand-left.svg
--rw-r--r--   0        0        0      360 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/expand-right.svg
--rw-r--r--   0        0        0      340 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/expand-top.svg
--rw-r--r--   0        0        0      368 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/export-parse.svg
--rw-r--r--   0        0        0      262 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/fat-arrow-down.svg
--rw-r--r--   0        0        0     1006 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/gear.svg
--rw-r--r--   0        0        0      333 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/ladder.svg
--rw-r--r--   0        0        0    12787 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/loading.png
--rw-r--r--   0        0        0      434 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/log-cut-tight.svg
--rw-r--r--   0        0        0      407 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/log-cut-wide.svg
--rw-r--r--   0        0        0      382 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/log-down.svg
--rw-r--r--   0        0        0      391 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/log-up.svg
--rw-r--r--   0        0        0    41619 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/oscr_icon_small.ico
--rw-r--r--   0        0        0    20631 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/oscr_icon_small.png
--rw-r--r--   0        0        0    25546 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/oscrbanner-slim-dark-label.png
--rw-r--r--   0        0        0    10840 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/oscrbanner-slim-dark.png
--rw-r--r--   0        0        0    10750 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/oscrbanner-slim.png
--rw-r--r--   0        0        0      449 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/parser-left.svg
--rw-r--r--   0        0        0      454 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/parser-right.svg
--rw-r--r--   0        0        0      395 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/refresh-cw.svg
--rw-r--r--   0        0        0      389 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/rename.svg
--rw-r--r--   0        0        0      222 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/resize.svg
--rw-r--r--   0        0        0      387 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/save-cw.svg
--rw-r--r--   0        0        0      389 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/save.svg
--rw-r--r--   0        0        0    10497 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/section31badge.png
--rw-r--r--   0        0        0      336 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/star.svg
--rw-r--r--   0        0        0    80078 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/stobuildslogo.png
--rw-r--r--   0        0        0      443 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/truncate-cw.svg
--rw-r--r--   0        0        0       12 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/.gitignore
--rw-r--r--   0        0        0    35149 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/LICENSE
--rw-r--r--   0        0        0      841 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/README.md
--rw-r--r--   0        0        0      986 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/pyproject.toml
--rw-r--r--   0        0        0    42047 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/PKG-INFO
+-rw-r--r--   0        0        0     2003 1980-01-01 00:00:00.000000 oscr_ui-2024.5b270/.OSCR_settings.ini
+-rw-r--r--   0        0        0       58 1980-01-01 00:00:00.000000 oscr_ui-2024.5b270/.flake8
+-rw-r--r--   0        0        0       98 1980-01-01 00:00:00.000000 oscr_ui-2024.5b270/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    27231 1980-01-01 00:00:00.000000 oscr_ui-2024.5b270/main.py
+-rw-r--r--   0        0        0      180 1980-01-01 00:00:00.000000 oscr_ui-2024.5b270/shell.nix
+-rw-r--r--   0        0        0     1306 1980-01-01 00:00:00.000000 oscr_ui-2024.5b270/.github/workflows/build.yml
+-rw-r--r--   0        0        0      214 1980-01-01 00:00:00.000000 oscr_ui-2024.5b270/OSCRUI/__init__.py
+-rw-r--r--   0        0        0    59990 1980-01-01 00:00:00.000000 oscr_ui-2024.5b270/OSCRUI/app.py
+-rw-r--r--   0        0        0     9816 1980-01-01 00:00:00.000000 oscr_ui-2024.5b270/OSCRUI/callbacks.py
+-rw-r--r--   0        0        0    15451 1980-01-01 00:00:00.000000 oscr_ui-2024.5b270/OSCRUI/datafunctions.py
+-rw-r--r--   0        0        0    15700 1980-01-01 00:00:00.000000 oscr_ui-2024.5b270/OSCRUI/datamodels.py
+-rw-r--r--   0        0        0    14843 1980-01-01 00:00:00.000000 oscr_ui-2024.5b270/OSCRUI/displayer.py
+-rw-r--r--   0        0        0     6144 1980-01-01 00:00:00.000000 oscr_ui-2024.5b270/OSCRUI/iofunctions.py
+-rw-r--r--   0        0        0    10150 1980-01-01 00:00:00.000000 oscr_ui-2024.5b270/OSCRUI/leagueconnector.py
+-rw-r--r--   0        0        0     5189 1980-01-01 00:00:00.000000 oscr_ui-2024.5b270/OSCRUI/style.py
+-rw-r--r--   0        0        0    20565 1980-01-01 00:00:00.000000 oscr_ui-2024.5b270/OSCRUI/subwindows.py
+-rw-r--r--   0        0        0     4131 1980-01-01 00:00:00.000000 oscr_ui-2024.5b270/OSCRUI/textedit.py
+-rw-r--r--   0        0        0    15033 1980-01-01 00:00:00.000000 oscr_ui-2024.5b270/OSCRUI/widgetbuilder.py
+-rw-r--r--   0        0        0    13361 1980-01-01 00:00:00.000000 oscr_ui-2024.5b270/OSCRUI/widgets.py
+-rw-r--r--   0        0        0   170564 1980-01-01 00:00:00.000000 oscr_ui-2024.5b270/assets/Overpass-Bold.ttf
+-rw-r--r--   0        0        0   170328 1980-01-01 00:00:00.000000 oscr_ui-2024.5b270/assets/Overpass-Medium.ttf
+-rw-r--r--   0        0        0   170204 1980-01-01 00:00:00.000000 oscr_ui-2024.5b270/assets/Overpass-Regular.ttf
+-rw-r--r--   0        0        0    87172 1980-01-01 00:00:00.000000 oscr_ui-2024.5b270/assets/RobotoMono-Medium.ttf
+-rw-r--r--   0        0        0    87236 1980-01-01 00:00:00.000000 oscr_ui-2024.5b270/assets/RobotoMono-Regular.ttf
+-rw-r--r--   0        0        0      229 1980-01-01 00:00:00.000000 oscr_ui-2024.5b270/assets/check.svg
+-rw-r--r--   0        0        0      227 1980-01-01 00:00:00.000000 oscr_ui-2024.5b270/assets/chevron-down.svg
+-rw-r--r--   0        0        0      227 1980-01-01 00:00:00.000000 oscr_ui-2024.5b270/assets/chevron-right.svg
+-rw-r--r--   0        0        0      225 1980-01-01 00:00:00.000000 oscr_ui-2024.5b270/assets/close.svg
+-rw-r--r--   0        0        0      348 1980-01-01 00:00:00.000000 oscr_ui-2024.5b270/assets/collapse-bottom.svg
+-rw-r--r--   0        0        0      329 1980-01-01 00:00:00.000000 oscr_ui-2024.5b270/assets/collapse-left.svg
+-rw-r--r--   0        0        0      332 1980-01-01 00:00:00.000000 oscr_ui-2024.5b270/assets/collapse-right.svg
+-rw-r--r--   0        0        0      339 1980-01-01 00:00:00.000000 oscr_ui-2024.5b270/assets/collapse-top.svg
+-rw-r--r--   0        0        0      319 1980-01-01 00:00:00.000000 oscr_ui-2024.5b270/assets/copy.svg
+-rw-r--r--   0        0        0      236 1980-01-01 00:00:00.000000 oscr_ui-2024.5b270/assets/dash.svg
+-rw-r--r--   0        0        0      336 1980-01-01 00:00:00.000000 oscr_ui-2024.5b270/assets/database.svg
+-rw-r--r--   0        0        0      283 1980-01-01 00:00:00.000000 oscr_ui-2024.5b270/assets/edit.svg
+-rw-r--r--   0        0        0      345 1980-01-01 00:00:00.000000 oscr_ui-2024.5b270/assets/expand-bottom.svg
+-rw-r--r--   0        0        0      330 1980-01-01 00:00:00.000000 oscr_ui-2024.5b270/assets/expand-left.svg
+-rw-r--r--   0        0        0      329 1980-01-01 00:00:00.000000 oscr_ui-2024.5b270/assets/expand-right.svg
+-rw-r--r--   0        0        0      340 1980-01-01 00:00:00.000000 oscr_ui-2024.5b270/assets/expand-top.svg
+-rw-r--r--   0        0        0      331 1980-01-01 00:00:00.000000 oscr_ui-2024.5b270/assets/export.svg
+-rw-r--r--   0        0        0      333 1980-01-01 00:00:00.000000 oscr_ui-2024.5b270/assets/ladder.svg
+-rw-r--r--   0        0        0    41619 1980-01-01 00:00:00.000000 oscr_ui-2024.5b270/assets/oscr_icon_small.ico
+-rw-r--r--   0        0        0    20631 1980-01-01 00:00:00.000000 oscr_ui-2024.5b270/assets/oscr_icon_small.png
+-rw-r--r--   0        0        0    25546 1980-01-01 00:00:00.000000 oscr_ui-2024.5b270/assets/oscrbanner-slim-dark-label.png
+-rw-r--r--   0        0        0      229 1980-01-01 00:00:00.000000 oscr_ui-2024.5b270/assets/page-down.svg
+-rw-r--r--   0        0        0      230 1980-01-01 00:00:00.000000 oscr_ui-2024.5b270/assets/page-up.svg
+-rw-r--r--   0        0        0      936 1980-01-01 00:00:00.000000 oscr_ui-2024.5b270/assets/parser-left-3.svg
+-rw-r--r--   0        0        0      880 1980-01-01 00:00:00.000000 oscr_ui-2024.5b270/assets/parser-right-3.svg
+-rw-r--r--   0        0        0      389 1980-01-01 00:00:00.000000 oscr_ui-2024.5b270/assets/rename.svg
+-rw-r--r--   0        0        0      222 1980-01-01 00:00:00.000000 oscr_ui-2024.5b270/assets/resize.svg
+-rw-r--r--   0        0        0      360 1980-01-01 00:00:00.000000 oscr_ui-2024.5b270/assets/save.svg
+-rw-r--r--   0        0        0    10497 1980-01-01 00:00:00.000000 oscr_ui-2024.5b270/assets/section31badge.png
+-rw-r--r--   0        0        0      307 1980-01-01 00:00:00.000000 oscr_ui-2024.5b270/assets/star.svg
+-rw-r--r--   0        0        0    80078 1980-01-01 00:00:00.000000 oscr_ui-2024.5b270/assets/stobuildslogo.png
+-rw-r--r--   0        0        0      227 1980-01-01 00:00:00.000000 oscr_ui-2024.5b270/assets/thick-chevron-down.svg
+-rw-r--r--   0        0        0       12 1980-01-01 00:00:00.000000 oscr_ui-2024.5b270/.gitignore
+-rw-r--r--   0        0        0    35149 1980-01-01 00:00:00.000000 oscr_ui-2024.5b270/LICENSE
+-rw-r--r--   0        0        0     1275 1980-01-01 00:00:00.000000 oscr_ui-2024.5b270/README.md
+-rw-r--r--   0        0        0      987 1980-01-01 00:00:00.000000 oscr_ui-2024.5b270/pyproject.toml
+-rw-r--r--   0        0        0    42483 1980-01-01 00:00:00.000000 oscr_ui-2024.5b270/PKG-INFO
```

### Comparing `oscr_ui-2024.4b20/.OSCR_settings.ini` & `oscr_ui-2024.5b270/.OSCR_settings.ini`

 * *Files 11% similar despite different names*

```diff
@@ -14,48 +14,52 @@
 dmg_columns%7C17=false
 dmg_columns%7C18=true
 dmg_columns%7C19=false
 dmg_columns%7C2=true
 dmg_columns%7C20=false
 dmg_columns%7C3=false
 dmg_columns%7C4=true
-dmg_columns%7C5=true
+dmg_columns%7C5=false
 dmg_columns%7C6=true
 dmg_columns%7C7=true
-dmg_columns%7C8=true
-dmg_columns%7C9=true
+dmg_columns%7C8=false
+dmg_columns%7C9=false
 excluded_event_ids=Autodesc.Combatevent.Falling, 
-favorite_ladders=@Invalid()
+favorite_ladders=DPS - Infected: The Conduit (Elite)
 first_overview_tab=0
-geometry=@ByteArray(\x1\xd9\xd0\xcb\0\x3\0\0\0\0\0\0\0\0\0\0\0\0\a\x8f\0\0\x4\x86\0\0\0\0\0\0\0\0\0\0\x5H\0\0\x3\xf9\0\0\0\0\x2\0\0\0\xf\0\0\0\0\0\0\0\0\0\0\0\a\x8f\0\0\x4\x86)
+geometry=@ByteArray(\x1\xd9\xd0\xcb\0\x3\0\0\0\0\0\0\0\0\0\0\0\0\x5Y\0\0\x3\xff\0\0\0\0\0\0\0\0\0\0\x5Y\0\0\x3\xff\0\0\0\0\x2\0\0\0\xf\0\0\0\0\0\0\0\0\0\0\0\x5Y\0\0\x3\xff)
 graph_resolution=0.2
 heal_columns_length=13
-heal_columns%7C0=true
-heal_columns%7C1=true
+heal_columns%7C0=false
+heal_columns%7C1=false
 heal_columns%7C10=true
-heal_columns%7C11=true
-heal_columns%7C12=true
-heal_columns%7C2=true
-heal_columns%7C3=true
-heal_columns%7C4=true
-heal_columns%7C5=true
-heal_columns%7C6=true
+heal_columns%7C11=false
+heal_columns%7C12=false
+heal_columns%7C2=false
+heal_columns%7C3=false
+heal_columns%7C4=false
+heal_columns%7C5=false
+heal_columns%7C6=false
 heal_columns%7C7=true
-heal_columns%7C8=true
-heal_columns%7C9=true
+heal_columns%7C8=false
+heal_columns%7C9=false
 live_columns%7C0=true
-live_columns%7C1=false
-live_columns%7C2=true
+live_columns%7C1=true
+live_columns%7C2=false
 live_columns%7C3=false
 live_columns%7C4=false
 live_columns%7C5=false
 live_columns%7C6=false
-live_geometry=@ByteArray(\x1\xd9\xd0\xcb\0\x3\0\0\0\0\xf\0\0\0\0\0\0\0\x11\x38\0\0\x1\xfd\0\0\xf\0\0\0\0\0\0\0\x16u\0\0\bU\0\0\0\x1\x2\0\0\0\xf\0\0\0\xf\0\0\0\0\0\0\0\x11\x38\0\0\x1\xfd)
-live_graph_active=true
+live_geometry=@ByteArray(\x1\xd9\xd0\xcb\0\x3\0\0\0\0\xf\0\0\0\0\0\0\0\x12\xae\0\0\x1\xf1\0\0\xf\0\0\0\0\0\0\0\x12\xb5\0\0\x4-\0\0\0\x1\x2\0\0\0\xf\0\0\0\xf\0\0\0\0\0\0\0\x12\xae\0\0\x1\xf1)
+live_graph_active=false
 live_graph_field=0
 live_parser_opacity=0.85
+live_scale=1.00
+live_splitter=@Invalid()
 log_path=/opt/SteamLibrary/steamapps/common/Star Trek Online/Star Trek Online/Live/logs/GameClient/combatlog.log
+log_size_warning=true
 overview_sort_column=1
 overview_sort_order=Descending
 seconds_between_combats=60
 split_log_after=480000
 sto_log_path=/opt/SteamLibrary/steamapps/common/Star Trek Online/Star Trek Online/Live/logs/GameClient/combatlog.log
+ui_scale=1.00
```

### Comparing `oscr_ui-2024.4b20/main.py` & `oscr_ui-2024.5b270/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import sys
 
 from OSCRUI import OSCRUI
 
 
 class Launcher():
 
-    version = '2024.04b020'
-    __version__ = '0.1'
+    version = '2024.05b270'
+    __version__ = '0.2'
 
     # holds the style of the app
     theme = {
         # general style
         'app': {
             'bg': '#1a1a1a',
             'fg': '#eeeeee',
@@ -416,15 +416,15 @@
             'border-bottom-style': 'solid',
             'border-bottom-color': '@bc',
             'outline': '0',  # removes dotted line around clicked item
             'font': ('Overpass', 12, 'Medium'),
             '::section': {
                 'background-color': '@mbg',
                 'color': '@fg',
-                'padding': (0, 0, 0, 0),  # (0, -8, -3, 6), # don't ask
+                'padding': (0, 0, 0, 0),
                 'border': 'none',
                 'margin': 0
             },
             '::section:hover': {
                 'background-color': '@loscr'
             },
         },
@@ -480,19 +480,19 @@
                 'border': 'none'
             },
             '::branch': {
                 'background-color': '@bg'
             },
             # down-pointing arrow
             '::branch:open:has-children': {
-                'image': 'url(assets/arrow-down.svg)'
+                'image': 'url(assets/chevron-down.svg)'
             },
             # right-pointing arrow
             '::branch:closed:has-children': {
-                'image': 'url(assets/arrow-right.svg)'
+                'image': 'url(assets/chevron-right.svg)'
             }
         },
         # header of the analysis table; ::section refers to the individual buttons
         'tree_table_header': {
             'background-color': '@bg',
             'border': 'none',
             'border-bottom-width': '@sep',
@@ -517,15 +517,15 @@
             'border-color': '@bc',
             'border-radius': '@br',
             'background-color': '@bg',
             'padding': (2, 5, 0, 5),
             'color': '@fg',
             'font': '@subhead',
             '::down-arrow': {
-                'image': 'url(assets/fat-arrow-down.svg)',
+                'image': 'url(assets/thick-chevron-down.svg)',
                 'width': '@margin',
             },
             '::drop-down': {
                 'border-style': 'none',
                 'padding': (2, 2, 2, 2)
             },
             '~QAbstractItemView': {
@@ -561,14 +561,18 @@
         },
         # undoes all styling of plot_widget to stop inheritance
         'plot_widget_nullifier': {
             'border': 'none',
             'margin': 0,
             'padding': 0,
         },
+        # smaller tick font for live parser graph
+        'live_plot_widget': {
+            'font': ('Overpass', 9, 'medium')
+        },
         # holds various properties related to graphing
         'plot': {
             'color_cycler': ('#8f54b4', '#B14D54', '#89B177', '#545DB4', '#C8B74E',
                              '#B45492', '#A27534', '#54A9B4', '#E47B1C', '#BCBCBC'),
         },
         'plot_legend': {
             'font': ('Overpass', 11, 'Medium'),
@@ -589,27 +593,27 @@
             'color': '@fg',
             'background-color': '@bg',
             'border-width': '@bw',
             'border-style': 'solid',
             'border-color': '@bc',
             'gridline-color': 'rgba(0,0,0,0)',  # -> s.c: table_gridline
             'outline': '0',  # removes dotted line around clicked item
-            'margin': 10,
+            'margin': (4, 4, 4, 4),
             'font': ('Roboto Mono', 10, 'Medium'),
             '::item': {
-                'padding': (0, 5, 0, 5),
+                'padding': (0, 2, 0, 2),
                 'border-width': '@bw',
                 'border-style': 'solid',
                 'border-color': '@bg',
                 'border-right-width': '@bw',
                 'border-right-style': 'solid',
                 'border-right-color': '@bc',
             },
             '::item:alternate': {
-                'padding': (0, 5, 0, 5),
+                'padding': (0, 2, 0, 2),
                 'background-color': '@mbg',
                 'border-width': '@bw',
                 'border-style': 'solid',
                 'border-color': '@mbg',
                 'border-right-width': '@bw',
                 'border-right-style': 'solid',
                 'border-right-color': '@bc',
@@ -624,15 +628,15 @@
             'border-bottom-style': 'solid',
             'border-bottom-color': '@bc',
             'outline': '0',  # removes dotted line around clicked item
             'font': ('Overpass', 10, 'Medium'),
             '::section': {
                 'background-color': '@mbg',
                 'color': '@fg',
-                'padding': (0, 0, 0, 0),  # (0, -8, -3, 6), # don't ask
+                'padding': (0, 0, 0, 0),
                 'border': 'none',
                 'margin': 0
             },
         },
         # index of the table (vertical header); ::section refers to the individual buttons
         'live_table_index': {
             'color': '@bg',
@@ -641,31 +645,46 @@
             'border-right-width': '@sep',
             'border-right-style': 'solid',
             'border-right-color': '@bc',
             'outline': '0',  # removes dotted line around clicked item
             '::section': {
                 'background-color': '@mbg',
                 'color': '@fg',
-                'padding': (0, 3, 0, 3),
+                'padding': (0, 2, 0, 2),
                 'border': 'none',
                 'margin': 0
             },
         },
         'resize_handle': {
             'border-style': 'none',
             'background-color': 'none',
             'image': 'url(assets/resize.svg)',
         },
+        'splitter': {
+            'border': 'none',
+            'margin': 0,
+            'padding': 0,
+            '::handle': {
+                'background-color': '@oscr'
+            },
+            '::handle:pressed': {
+                'background-color': '@bc'
+            },
+            '::handle:vertical': {
+                'height': '@bw',
+                'margin': (0, 13, 0, 13)
+            }
+        },
         # other style decisions
         's.c': {
             'sidebar_item_width': 0.2,
             'button_icon_size': 24,
             'table_alternate': True,
             'table_gridline': False,
-            'overview_graph_stretch': 11,
+            'overview_graph_stretch': 10,
             'overview_table_stretch': 3
         }
     }
 
     @staticmethod
     def base_path() -> str:
         """initialize the base path"""
@@ -674,29 +693,33 @@
         except Exception:
             base_path = os.path.abspath(os.path.dirname(__file__))
         return base_path
 
     @staticmethod
     def app_config() -> dict:
         config = {
-            'minimum_window_width': 1280,
-            'minimum_window_height': 1016,
+            'minimum_window_width': 1370,
+            'minimum_window_height': 907,
             'settings_path': r'/.OSCR_settings.ini',
             'templog_folder_path': r'/~temp_log_files',
             'link_website': '',
             'link_github': 'https://github.com/STOCD/OSCR-UI',
             'link_downloads': 'https://github.com/STOCD/OSCR-UI/releases',
             'link_stobuilds': 'https://discord.gg/stobuilds',
             'link_stocd': 'https://github.com/STOCD',
             'live_graph_fields': ('DPS', 'Debuff', 'Attacks-in Share', 'HPS'),
+            'ui_scale': 1,
+            'live_scale': 1,
+            'icon_size': 24,
             'default_settings': {
                 'log_path': '',
                 'sto_log_path': '',
                 'geometry': None,
                 'live_geometry': None,
+                'live_splitter': None,
                 'dmg_columns|0': True,
                 'dmg_columns|1': True,
                 'dmg_columns|2': True,
                 'dmg_columns|3': True,
                 'dmg_columns|4': True,
                 'dmg_columns|5': True,
                 'dmg_columns|6': True,
@@ -746,14 +769,16 @@
                 'live_columns|5': False,
                 'live_columns|6': False,
                 'live_parser_opacity': 0.85,
                 'live_graph_active': False,
                 'live_graph_field': 0,
                 'first_overview_tab': 0,
                 'log_size_warning': True,
+                'ui_scale': 1,
+                'live_scale': 1,
             }
         }
         return config
 
     @staticmethod
     def launch():
         args = {}
```

### Comparing `oscr_ui-2024.4b20/.github/workflows/build.yml` & `oscr_ui-2024.5b270/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `oscr_ui-2024.4b20/OSCRUI/app.py` & `oscr_ui-2024.5b270/OSCRUI/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 import os
 
-from PySide6.QtWidgets import QApplication, QWidget, QLineEdit, QFrame, QListWidget
+from PySide6.QtWidgets import QApplication, QWidget, QLineEdit, QFrame, QListWidget, QScrollArea
 from PySide6.QtWidgets import QSpacerItem, QTabWidget, QTableView
 from PySide6.QtWidgets import QVBoxLayout, QHBoxLayout, QGridLayout
 from PySide6.QtCore import QSize, QSettings, QTimer
 from PySide6.QtGui import QFontDatabase, QIntValidator
 
 from OSCR import HEAL_TREE_HEADER, LIVE_TABLE_HEADER, TABLE_HEADER, TREE_HEADER
 
 from .leagueconnector import OSCRClient
 from .iofunctions import get_asset_path, load_icon_series, load_icon, open_link, reset_temp_folder
 from .textedit import format_path
 from .widgets import AnalysisPlot, BannerLabel, FlipButton, WidgetStorage
 from .widgetbuilder import ABOTTOM, ACENTER, AHCENTER, ALEFT, ARIGHT, ATOP, AVCENTER
 from .widgetbuilder import SEXPAND, SMAXMAX, SMAXMIN, SMIN, SMINMAX, SMINMIN, SMIXMAX, SMIXMIN
+from .widgetbuilder import SCROLLOFF, SCROLLON, SMPIXEL
 
 # only for developing; allows to terminate the qt event loop with keyboard interrupt
 from signal import signal, SIGINT, SIG_DFL
 signal(SIGINT, SIG_DFL)
 
 
 class OSCRUI():
 
     from .callbacks import (
             browse_log, browse_sto_logpath, collapse_overview_table, expand_overview_table,
-            favorite_button_callback, navigate_log, save_combat, set_graph_resolution_setting,
-            set_sto_logpath_setting, set_parser_opacity_setting, switch_analysis_tab,
-            switch_main_tab, switch_map_tab, switch_overview_tab)
+            favorite_button_callback, navigate_log, save_combat, set_live_scale_setting,
+            set_parser_opacity_setting, set_graph_resolution_setting, set_sto_logpath_setting,
+            set_ui_scale_setting, switch_analysis_tab, switch_main_tab, switch_map_tab,
+            switch_overview_tab)
     from .datafunctions import analyze_log_callback, copy_analysis_callback
     from .datafunctions import copy_summary_callback, init_parser, update_shown_columns_dmg
     from .datafunctions import update_shown_columns_heal
     from .displayer import create_legend_item
     from .iofunctions import browse_path
     from .style import get_style_class, create_style_sheet, theme_font, get_style
     from .subwindows import live_parser_toggle, split_dialog
@@ -102,31 +104,33 @@
         """
         icons = {
             'oscr': 'oscr_icon_small.png',
             'expand-left': 'expand-left.svg',
             'collapse-left': 'collapse-left.svg',
             'expand-right': 'expand-right.svg',
             'collapse-right': 'collapse-right.svg',
-            'save': 'save.svg',
-            'log-up': 'log-up.svg',
-            'log-down': 'log-down.svg',
-            'log-cut': 'log-cut-tight.svg',
-            'parser-left': 'parser-left.svg',
-            'parser-right': 'parser-right.svg',
-            'export-parse': 'export-parse.svg',
+            'save': 'database.svg',
+            'page-up': 'page-up.svg',
+            'page-down': 'page-down.svg',
+            'edit': 'edit.svg',
+            'parser-left': 'parser-left-3.svg',
+            'parser-right': 'parser-right-3.svg',
+            'export-parse': 'export.svg',
             'copy': 'copy.svg',
             'ladder': 'ladder.svg',
             'star': 'star.svg',
             'stocd': 'section31badge.png',
             'stobuilds': 'stobuildslogo.png',
             'close': 'close.svg',
             'expand-top': 'expand-top.svg',
             'collapse-top': 'collapse-top.svg',
             'expand-bottom': 'expand-bottom.svg',
             'collapse-bottom': 'collapse-bottom.svg',
+            'check': 'check.svg',
+            'dash': 'dash.svg'
         }
         self.icons = load_icon_series(icons, self.app_dir)
 
     def init_settings(self):
         """
         Prepares settings. Loads stored settings. Saves current settings for next startup.
         """
@@ -142,14 +146,18 @@
         """
         Prepares config.
         """
         self.current_combat_id = -1
         self.current_combat_path = ''
         self.config['templog_folder_path'] = os.path.abspath(
                 self.app_dir + self.config['templog_folder_path'])
+        self.config['ui_scale'] = self.settings.value('ui_scale', type=float)
+        self.config['live_scale'] = self.settings.value('live_scale', type=float)
+        self.config['icon_size'] = round(
+                self.config['ui_scale'] * self.theme['s.c']['button_icon_size'])
 
     @property
     def parser_settings(self) -> dict:
         """
         Returns settings relevant to the parser
         """
         relevant_settings = (
@@ -171,15 +179,18 @@
         return {'seconds_between_combats': self.settings.value('seconds_between_combats', type=int)}
 
     @property
     def sidebar_item_width(self) -> int:
         """
         Width of the sidebar.
         """
-        return int(self.theme['s.c']['sidebar_item_width'] * self.window.width())
+        return int(
+                self.theme['s.c']['sidebar_item_width']
+                * self.window.width()
+                * self.config['ui_scale'])
 
     def main_window_close_callback(self, event):
         """
         Executed when application is closed.
         """
         window_geometry = self.window.saveGeometry()
         self.settings.setValue('geometry', window_geometry)
@@ -207,19 +218,19 @@
         font_database.addApplicationFont(get_asset_path('Overpass-Bold.ttf', self.app_dir))
         font_database.addApplicationFont(get_asset_path('Overpass-Medium.ttf', self.app_dir))
         font_database.addApplicationFont(get_asset_path('Overpass-Regular.ttf', self.app_dir))
         font_database.addApplicationFont(get_asset_path('RobotoMono-Regular.ttf', self.app_dir))
         font_database.addApplicationFont(get_asset_path('RobotoMono-Medium.ttf', self.app_dir))
         app.setStyleSheet(self.create_style_sheet(self.theme['app']['style']))
         window = QWidget()
+        window.setMinimumSize(
+                self.config['ui_scale'] * self.config['minimum_window_width'],
+                self.config['ui_scale'] * self.config['minimum_window_height'])
         window.setWindowIcon(load_icon('oscr_icon_small.png', self.app_dir))
         window.setWindowTitle('Open Source Combatlog Reader')
-        window.setMinimumSize(
-                int(self.config['minimum_window_width']),
-                int(self.config['minimum_window_height']))
         if self.settings.value('geometry'):
             window.restoreGeometry(self.settings.value('geometry'))
         window.closeEvent = self.main_window_close_callback
         window.resizeEvent = self.main_window_resize_callback
         return app, window
 
     def setup_main_layout(self):
@@ -247,15 +258,15 @@
         csp = self.theme['defaults']['csp']
         col_1 = QVBoxLayout()
         col_1.setContentsMargins(csp, csp, csp, csp)
         content_layout.addLayout(col_1, 0, 1)
         col_3 = QVBoxLayout()
         col_3.setContentsMargins(csp, csp, csp, csp)
         content_layout.addLayout(col_3, 0, 3)
-        icon_size = self.theme['s.c']['button_icon_size']
+        icon_size = self.config['icon_size']
         left_flip_config = {
             'icon_r': self.icons['collapse-left'], 'func_r': left.hide,
             'icon_l': self.icons['expand-left'], 'func_l': left.show,
             'tooltip_r': 'Collapse Sidebar', 'tooltip_l': 'Expand Sidebar'
         }
         right_flip_config = {
             'icon_r': self.icons['expand-right'], 'func_r': right.show,
@@ -423,15 +434,15 @@
         left_layout.setSpacing(0)
         left_layout.setAlignment(ATOP)
 
         head_layout = QHBoxLayout()
         head = self.create_label('STO Combatlog:', 'label_heading', frame)
         head_layout.addWidget(head, alignment=ALEFT | ABOTTOM)
         cut_log_button = self.create_icon_button(
-                self.icons['log-cut'], 'Manage Logfile', parent=frame)
+                self.icons['edit'], 'Manage Logfile', parent=frame)
         cut_log_button.clicked.connect(self.split_dialog)
         head_layout.addWidget(cut_log_button, alignment=ARIGHT)
         left_layout.addLayout(head_layout)
 
         self.entry = QLineEdit(self.settings.value('log_path', ''), frame)
         self.entry.setStyleSheet(self.get_style_class('QLineEdit', 'entry'))
         self.entry.setFont(self.theme_font('entry'))
@@ -449,15 +460,15 @@
                     path=self.entry.text(), parser_num=1), 'align': ARIGHT}
         }
         entry_buttons = self.create_button_series(frame, entry_button_config, 'button')
         left_layout.addLayout(entry_buttons)
 
         top_button_row = QHBoxLayout()
         top_button_row.setContentsMargins(0, 0, 0, 0)
-        top_button_row.setSpacing(0)
+        top_button_row.setSpacing(m)
 
         combat_button_layout = QHBoxLayout()
         combat_button_layout.setContentsMargins(0, 0, 0, 0)
         combat_button_layout.setSpacing(m)
         combat_button_layout.setAlignment(ALEFT)
         export_button = self.create_icon_button(
                 self.icons['export-parse'], 'Export Combat', parent=frame)
@@ -468,20 +479,20 @@
         top_button_row.addLayout(combat_button_layout)
 
         navigation_button_layout = QHBoxLayout()
         navigation_button_layout.setContentsMargins(0, 0, 0, 0)
         navigation_button_layout.setSpacing(m)
         navigation_button_layout.setAlignment(AHCENTER)
         up_button = self.create_icon_button(
-                self.icons['log-up'], 'Load newer Combats', parent=frame)
+                self.icons['page-up'], 'Load newer Combats', parent=frame)
         up_button.setEnabled(False)
         navigation_button_layout.addWidget(up_button)
         self.widgets.navigate_up_button = up_button
         down_button = self.create_icon_button(
-                self.icons['log-down'], 'Load older Combats', parent=frame)
+                self.icons['page-down'], 'Load older Combats', parent=frame)
         down_button.setEnabled(False)
         navigation_button_layout.addWidget(down_button)
         self.widgets.navigate_down_button = down_button
         top_button_row.addLayout(navigation_button_layout)
 
         parser_button_layout = QHBoxLayout()
         parser_button_layout.setContentsMargins(0, 0, 0, 0)
@@ -562,15 +573,15 @@
         buttons[1].setToolTip(self.config['link_github'])
         buttons[2].setToolTip(self.config['link_downloads'])
         left_layout.addLayout(button_layout)
         left_layout.addSpacerItem(QSpacerItem(1, 1, hData=SMIN, vData=SEXPAND))
         logo_layout = QGridLayout()
         logo_layout.setContentsMargins(0, 0, 0, 0)
         logo_layout.setColumnStretch(1, 1)
-        logo_size = [self.theme['s.c']['button_icon_size'] * 4] * 2
+        logo_size = [self.config['icon_size'] * 4] * 2
         stocd_logo = self.create_icon_button(
                 self.icons['stocd'], self.config['link_stocd'],
                 style_override={'border-style': 'none'}, icon_size=logo_size)
         stocd_logo.clicked.connect(lambda: open_link(self.config['link_stocd']))
         logo_layout.addWidget(stocd_logo, 0, 0)
         left_layout.addLayout(logo_layout)
         stobuilds_logo = self.create_icon_button(
@@ -937,241 +948,262 @@
         Populates the settings frame.
         """
         settings_frame = self.widgets.main_tab_frames[3]
         settings_layout = QHBoxLayout()
         isp = self.theme['defaults']['isp']
         settings_layout.setContentsMargins(2 * isp, isp, isp, isp)
         settings_layout.setSpacing(isp)
+        scroll_layout = QVBoxLayout()
+        scroll_layout.setContentsMargins(0, 0, 0, 0)
+        scroll_layout.setSpacing(isp)
+        scroll_frame = self.create_frame()
+        scroll_area = QScrollArea()
+        scroll_area.setSizePolicy(SMINMIN)
+        scroll_area.setHorizontalScrollBarPolicy(SCROLLOFF)
+        scroll_area.setVerticalScrollBarPolicy(SCROLLON)
+        scroll_area.setAlignment(AHCENTER)
+        settings_layout.addWidget(scroll_area)
+        settings_frame.setLayout(settings_layout)
+        col_1_frame = None  # TODO remove parent parameter from self.create_... functions
+        col_2_frame = None
 
-        col_1_frame = self.create_frame(settings_frame)
-        col_1_frame.setSizePolicy(SMINMAX)
-        settings_layout.addWidget(col_1_frame, alignment=ATOP, stretch=1)
-        col_2_frame = self.create_frame(settings_frame)
-        col_2_frame.setSizePolicy(SMINMAX)
-        settings_layout.addWidget(col_2_frame, alignment=ATOP, stretch=1)
-        col_3_frame = self.create_frame(settings_frame)
-        col_3_frame.setSizePolicy(SMINMAX)
-        settings_layout.addWidget(col_3_frame, alignment=ATOP, stretch=1)
-
-        # first column
-        hider_frame_style_override = {
-            'border-color': '@lbg',
-            'border-width': '@bw', 'border-style': 'solid', 'border-radius': 2
-        }
-        col_1 = QHBoxLayout()
-        col_1.setContentsMargins(0, 0, 0, 0)
-        col_1.setSpacing(self.theme['defaults']['isp'])
-        col_1_1 = QVBoxLayout()
-        col_1_1.setSpacing(0)
-        dmg_hider_label = self.create_label('Damage table columns:', 'label_subhead')
-        col_1_1.addWidget(dmg_hider_label)
-        dmg_hider_layout = QVBoxLayout()
-        dmg_hider_frame = self.create_frame(
-                col_1_frame, size_policy=SMINMAX, style_override=hider_frame_style_override)
-        self.set_buttons = list()
-        for i, head in enumerate(TREE_HEADER[1:]):
-            bt = self.create_button(
-                    head, 'toggle_button', dmg_hider_frame,
-                    toggle=self.settings.value(f'dmg_columns|{i}', type=bool))
-            bt.setSizePolicy(SMINMAX)
-            bt.clicked[bool].connect(
-                    lambda state, i=i: self.settings.setValue(f'dmg_columns|{i}', state))
-            dmg_hider_layout.addWidget(bt, stretch=1)
-        dmg_seperator = self.create_frame(
-                dmg_hider_frame, 'hr', style_override={'background-color': '@lbg'},
-                size_policy=SMINMIN)
-        dmg_seperator.setFixedHeight(self.theme['defaults']['bw'])
-        dmg_hider_layout.addWidget(dmg_seperator)
-        apply_button = self.create_button('Apply', 'button', dmg_hider_frame)
-        apply_button.clicked.connect(self.update_shown_columns_dmg)
-        dmg_hider_layout.addWidget(apply_button, alignment=ARIGHT | ATOP)
-        dmg_hider_frame.setLayout(dmg_hider_layout)
-        col_1_1.addWidget(dmg_hider_frame, alignment=ATOP)
-        col_1.addLayout(col_1_1, stretch=1)
-
-        col_1_2 = QVBoxLayout()
-        col_1_2.setSpacing(0)
-        heal_hider_label = self.create_label('Heal table columns:', 'label_subhead', col_1_frame)
-        col_1_2.addWidget(heal_hider_label)
-        heal_hider_layout = QVBoxLayout()
-        heal_hider_frame = self.create_frame(
-                col_1_frame, size_policy=SMINMAX, style_override=hider_frame_style_override)
-        for i, head in enumerate(HEAL_TREE_HEADER[1:]):
-            bt = self.create_button(
-                    head, 'toggle_button', heal_hider_frame,
-                    toggle=self.settings.value(f'heal_columns|{i}', type=bool))
-            bt.setSizePolicy(SMINMAX)
-            bt.clicked[bool].connect(
-                    lambda state, i=i: self.settings.setValue(f'heal_columns|{i}', state))
-            heal_hider_layout.addWidget(bt, stretch=1)
-        heal_seperator = self.create_frame(
-            heal_hider_frame, 'hr', style_override={'background-color': '@lbg'},
-            size_policy=SMINMIN)
-        heal_seperator.setFixedHeight(self.theme['defaults']['bw'])
-        heal_hider_layout.addWidget(heal_seperator)
-        apply_button_2 = self.create_button('Apply', 'button', heal_hider_frame)
-        apply_button_2.clicked.connect(self.update_shown_columns_heal)
-        heal_hider_layout.addWidget(apply_button_2, alignment=ARIGHT | ATOP)
-        heal_hider_frame.setLayout(heal_hider_layout)
-
-        col_1_2.addWidget(heal_hider_frame, alignment=ATOP)
-        live_hider_label = self.create_label(
-                'Live Parser columns:', 'label_subhead', col_1_frame, {'margin-top': '@isp'})
-        col_1_2.addWidget(live_hider_label)
-        live_hider_layout = QVBoxLayout()
-        live_hider_frame = self.create_frame(
-                col_1_frame, size_policy=SMINMAX, style_override=hider_frame_style_override)
-        for i, head in enumerate(LIVE_TABLE_HEADER):
-            bt = self.create_button(
-                    head, 'toggle_button', live_hider_frame,
-                    toggle=self.settings.value(f'live_columns|{i}', type=bool))
-            bt.setSizePolicy(SMINMAX)
-            bt.clicked[bool].connect(
-                    lambda state, i=i: self.settings.setValue(f'live_columns|{i}', state))
-            live_hider_layout.addWidget(bt, stretch=1)
-        live_hider_frame.setLayout(live_hider_layout)
-        col_1_2.addWidget(live_hider_frame, alignment=ATOP)
-        col_1.addLayout(col_1_2, stretch=1)
-
-        col_1_frame.setLayout(col_1)
-
-        # second column
-        col_2 = QGridLayout()
-        col_2.setContentsMargins(0, 0, 0, 0)
-        col_2.setVerticalSpacing(self.theme['defaults']['isp'])
-        col_2.setHorizontalSpacing(self.theme['defaults']['csp'])
+        # first section
+        sec_1 = QGridLayout()
+        sec_1.setContentsMargins(0, 0, 0, 0)
+        sec_1.setVerticalSpacing(self.theme['defaults']['isp'])
+        sec_1.setHorizontalSpacing(self.theme['defaults']['csp'])
         combat_delta_label = self.create_label('Seconds Between Combats:', 'label_subhead')
-        col_2.addWidget(combat_delta_label, 0, 0, alignment=ARIGHT)
+        sec_1.addWidget(combat_delta_label, 0, 0, alignment=ARIGHT)
         combat_delta_validator = QIntValidator()
         combat_delta_validator.setBottom(1)
         combat_delta_entry = self.create_entry(
                 self.settings.value('seconds_between_combats', type=str),
                 combat_delta_validator, style_override={'margin-top': 0})
         combat_delta_entry.setSizePolicy(SMIXMAX)
         combat_delta_entry.editingFinished.connect(lambda: self.settings.setValue(
                 'seconds_between_combats', combat_delta_entry.text()))
-        col_2.addWidget(combat_delta_entry, 0, 1, alignment=AVCENTER)
+        sec_1.addWidget(combat_delta_entry, 0, 1, alignment=AVCENTER)
         combat_num_label = self.create_label('Number of combats to isolate:', 'label_subhead')
-        col_2.addWidget(combat_num_label, 1, 0, alignment=ARIGHT)
+        sec_1.addWidget(combat_num_label, 1, 0, alignment=ARIGHT)
         combat_num_validator = QIntValidator()
         combat_num_validator.setBottom(1)
         combat_num_entry = self.create_entry(
                 self.settings.value('combats_to_parse', type=str), combat_num_validator,
                 style_override={'margin-top': 0})
         combat_num_entry.setSizePolicy(SMIXMAX)
         combat_num_entry.editingFinished.connect(lambda: self.settings.setValue(
                 'combats_to_parse', combat_num_entry.text()))
-        col_2.addWidget(combat_num_entry, 1, 1, alignment=AVCENTER)
+        sec_1.addWidget(combat_num_entry, 1, 1, alignment=AVCENTER)
         graph_resolution_label = self.create_label(
                 'Graph resolution (interval in seconds):', 'label_subhead')
-        col_2.addWidget(graph_resolution_label, 2, 0, alignment=ARIGHT)
+        sec_1.addWidget(graph_resolution_label, 2, 0, alignment=ARIGHT)
         graph_resolution_layout = self.create_annotated_slider(
                 self.settings.value('graph_resolution', type=float) * 10, 1, 20,
                 callback=self.set_graph_resolution_setting)
-        col_2.addLayout(graph_resolution_layout, 2, 1, alignment=ALEFT)
+        sec_1.addLayout(graph_resolution_layout, 2, 1, alignment=ALEFT)
         split_length_label = self.create_label('Auto Split After Lines:', 'label_subhead')
-        col_2.addWidget(split_length_label, 3, 0, alignment=ARIGHT)
+        sec_1.addWidget(split_length_label, 3, 0, alignment=ARIGHT)
         split_length_validator = QIntValidator()
         split_length_validator.setBottom(1)
         split_length_entry = self.create_entry(
                 self.settings.value('split_log_after', type=str), split_length_validator,
                 style_override={'margin-top': 0})
         split_length_entry.setSizePolicy(SMIXMAX)
         split_length_entry.editingFinished.connect(lambda: self.settings.setValue(
                 'split_log_after', split_length_entry.text()))
-        col_2.addWidget(split_length_entry, 3, 1, alignment=AVCENTER)
+        sec_1.addWidget(split_length_entry, 3, 1, alignment=AVCENTER)
         overview_sort_label = self.create_label('Sort overview table by column:', 'label_subhead')
-        col_2.addWidget(overview_sort_label, 4, 0, alignment=ARIGHT)
+        sec_1.addWidget(overview_sort_label, 4, 0, alignment=ARIGHT)
         overview_sort_combo = self.create_combo_box(
                 col_2_frame, style_override={'font': '@small_text'})
         overview_sort_combo.addItems(TABLE_HEADER)
         overview_sort_combo.setCurrentIndex(self.settings.value('overview_sort_column', type=int))
         overview_sort_combo.currentIndexChanged.connect(
                 lambda new_index: self.settings.setValue('overview_sort_column', new_index))
-        col_2.addWidget(overview_sort_combo, 4, 1, alignment=ALEFT | AVCENTER)
+        sec_1.addWidget(overview_sort_combo, 4, 1, alignment=ALEFT | AVCENTER)
         overview_sort_order_label = self.create_label('Overview table sort order:', 'label_subhead')
-        col_2.addWidget(overview_sort_order_label, 5, 0, alignment=ARIGHT)
+        sec_1.addWidget(overview_sort_order_label, 5, 0, alignment=ARIGHT)
         overview_sort_order_combo = self.create_combo_box(
                 col_2_frame, style_override={'font': '@small_text'})
         overview_sort_order_combo.addItems(('Descending', 'Ascending'))
         overview_sort_order_combo.setCurrentText(self.settings.value('overview_sort_order'))
         overview_sort_order_combo.currentTextChanged.connect(
                 lambda new_text: self.settings.setValue('overview_sort_order', new_text))
-        col_2.addWidget(overview_sort_order_combo, 5, 1, alignment=ALEFT | AVCENTER)
+        sec_1.addWidget(overview_sort_order_combo, 5, 1, alignment=ALEFT | AVCENTER)
         auto_scan_label = self.create_label('Scan log automatically:', 'label_subhead')
-        col_2.addWidget(auto_scan_label, 6, 0, alignment=ARIGHT)
+        sec_1.addWidget(auto_scan_label, 6, 0, alignment=ARIGHT)
         auto_scan_button = FlipButton('Disabled', 'Enabled', col_2_frame, checkable=True)
         auto_scan_button.setStyleSheet(self.get_style_class(
                 'QPushButton', 'toggle_button', override={'margin-top': 0, 'margin-left': 0}))
         auto_scan_button.setFont(self.theme_font('app', '@font'))
         auto_scan_button.r_function = lambda: self.settings.setValue('auto_scan', True)
         auto_scan_button.l_function = lambda: self.settings.setValue('auto_scan', False)
         if self.settings.value('auto_scan', type=bool):
             auto_scan_button.flip()
-        col_2.addWidget(auto_scan_button, 6, 1, alignment=ALEFT | AVCENTER)
+        sec_1.addWidget(auto_scan_button, 6, 1, alignment=ALEFT | AVCENTER)
         sto_log_path_button = self.create_button('STO Logfile:', style_override={
                 'margin': 0, 'font': '@subhead', 'border-color': '@bc', 'border-style': 'solid',
                 'border-width': '@bw'})
-        col_2.addWidget(sto_log_path_button, 7, 0, alignment=ARIGHT | AVCENTER)
+        sec_1.addWidget(sto_log_path_button, 7, 0, alignment=ARIGHT | AVCENTER)
         sto_log_path_entry = self.create_entry(
                 self.settings.value('sto_log_path'), style_override={'margin-top': 0})
         sto_log_path_entry.setSizePolicy(SMIXMAX)
         sto_log_path_entry.editingFinished.connect(
                 lambda: self.set_sto_logpath_setting(sto_log_path_entry))
-        col_2.addWidget(sto_log_path_entry, 7, 1, alignment=AVCENTER)
+        sec_1.addWidget(sto_log_path_entry, 7, 1, alignment=AVCENTER)
         sto_log_path_button.clicked.connect(lambda: self.browse_sto_logpath(sto_log_path_entry))
         opacity_label = self.create_label('Live Parser Opacity:', 'label_subhead')
-        col_2.addWidget(opacity_label, 8, 0, alignment=ARIGHT)
+        sec_1.addWidget(opacity_label, 8, 0, alignment=ARIGHT)
         opacity_slider_layout = self.create_annotated_slider(
                 default_value=round(self.settings.value('live_parser_opacity', type=float) * 20, 0),
                 min=1, max=20,
                 style_override_slider={'::sub-page:horizontal': {'background-color': '@bc'}},
                 callback=self.set_parser_opacity_setting)
-        col_2.addLayout(opacity_slider_layout, 8, 1, alignment=AVCENTER)
+        sec_1.addLayout(opacity_slider_layout, 8, 1, alignment=AVCENTER)
         live_graph_active_label = self.create_label('LiveParser Graph:', 'label_subhead')
-        col_2.addWidget(live_graph_active_label, 9, 0, alignment=ARIGHT)
+        sec_1.addWidget(live_graph_active_label, 9, 0, alignment=ARIGHT)
         live_graph_active_button = FlipButton('Disabled', 'Enabled', col_2_frame, checkable=True)
         live_graph_active_button.setStyleSheet(self.get_style_class(
                 'QPushButton', 'toggle_button', override={'margin-top': 0, 'margin-left': 0}))
         live_graph_active_button.setFont(self.theme_font('app', '@font'))
         live_graph_active_button.r_function = (
                 lambda: self.settings.setValue('live_graph_active', True))
         live_graph_active_button.l_function = (
                 lambda: self.settings.setValue('live_graph_active', False))
         if self.settings.value('live_graph_active', type=bool):
             live_graph_active_button.flip()
-        col_2.addWidget(live_graph_active_button, 9, 1, alignment=ALEFT | AVCENTER)
+        sec_1.addWidget(live_graph_active_button, 9, 1, alignment=ALEFT | AVCENTER)
         live_graph_field_label = self.create_label('LiveParser Graph Field:', 'label_subhead')
-        col_2.addWidget(live_graph_field_label, 10, 0, alignment=ARIGHT)
+        sec_1.addWidget(live_graph_field_label, 10, 0, alignment=ARIGHT)
         live_graph_field_combo = self.create_combo_box(
                 col_2_frame, style_override={'font': '@small_text'})
         live_graph_field_combo.addItems(self.config['live_graph_fields'])
         live_graph_field_combo.setCurrentIndex(self.settings.value('live_graph_field', type=int))
         live_graph_field_combo.currentIndexChanged.connect(
                 lambda new_index: self.settings.setValue('live_graph_field', new_index))
-        col_2.addWidget(live_graph_field_combo, 10, 1, alignment=ALEFT)
+        sec_1.addWidget(live_graph_field_combo, 10, 1, alignment=ALEFT)
         overview_tab_label = self.create_label('Default Overview Tab:', 'label_subhead')
-        col_2.addWidget(overview_tab_label, 11, 0, alignment=ARIGHT)
+        sec_1.addWidget(overview_tab_label, 11, 0, alignment=ARIGHT)
         overview_tab_combo = self.create_combo_box(
                 col_2_frame, style_override={'font': '@small_text'})
         overview_tab_combo.addItems(('DPS Bar', 'DPS Graph', 'Damage Graph'))
         overview_tab_combo.setCurrentIndex(self.settings.value('first_overview_tab', type=int))
         overview_tab_combo.currentIndexChanged.connect(
             lambda new_index: self.settings.setValue('first_overview_tab', new_index))
-        col_2.addWidget(overview_tab_combo, 11, 1, alignment=ALEFT)
+        sec_1.addWidget(overview_tab_combo, 11, 1, alignment=ALEFT)
         size_warning_label = self.create_label('Logfile Size Warning:', 'label_subhead')
-        col_2.addWidget(size_warning_label, 12, 0, alignment=ARIGHT)
+        sec_1.addWidget(size_warning_label, 12, 0, alignment=ARIGHT)
         size_warning_button = FlipButton('Disabled', 'Enabled', col_2_frame, checkable=True)
         size_warning_button.setStyleSheet(self.get_style_class(
                 'QPushButton', 'toggle_button', override={'margin-top': 0, 'margin-left': 0}))
         size_warning_button.setFont(self.theme_font('app', '@font'))
         size_warning_button.r_function = (
                 lambda: self.settings.setValue('log_size_warning', True))
         size_warning_button.l_function = (
                 lambda: self.settings.setValue('log_size_warning', False))
         if self.settings.value('log_size_warning', type=bool):
             size_warning_button.flip()
-        col_2.addWidget(size_warning_button, 12, 1, alignment=ALEFT)
+        sec_1.addWidget(size_warning_button, 12, 1, alignment=ALEFT)
+        ui_scale_label = self.create_label('UI Scale:', 'label_subhead')
+        sec_1.addWidget(ui_scale_label, 13, 0, alignment=ARIGHT)
+        ui_scale_slider_layout = self.create_annotated_slider(
+                default_value=round(self.settings.value('ui_scale', type=float) * 50, 0),
+                min=25, max=75, callback=self.set_ui_scale_setting)
+        sec_1.addLayout(ui_scale_slider_layout, 13, 1, alignment=ALEFT)
+        ui_scale_label = self.create_label('LiveParser Scale:', 'label_subhead')
+        sec_1.addWidget(ui_scale_label, 14, 0, alignment=ARIGHT)
+        live_scale_slider_layout = self.create_annotated_slider(
+                default_value=round(self.settings.value('live_scale', type=float) * 50, 0),
+                min=25, max=75, callback=self.set_live_scale_setting)
+        sec_1.addLayout(live_scale_slider_layout, 14, 1, alignment=ALEFT)
+        sec_1.setAlignment(AHCENTER)
+        scroll_layout.addLayout(sec_1)
+
+        # seperator
+        section_seperator = self.create_frame(
+            scroll_frame, 'hr', style_override={'background-color': '@lbg'},
+            size_policy=SMINMIN)
+        section_seperator.setFixedHeight(self.theme['defaults']['bw'])
+        scroll_layout.addWidget(section_seperator)
 
-        col_2_frame.setLayout(col_2)
+        # second section
+        hider_frame_style_override = {
+            'border-color': '@lbg',
+            'border-width': '@bw', 'border-style': 'solid', 'border-radius': 2
+        }
+        sec_2 = QVBoxLayout()
+        sec_2.setContentsMargins(0, isp, 0, 0)
+        sec_2.setSpacing(isp)
+        sec_2.setAlignment(AHCENTER)
+        dmg_hider_label = self.create_label(
+            'Damage table columns:', 'label_subhead')
+        sec_2.addWidget(dmg_hider_label)
+        dmg_hider_layout = QVBoxLayout()
+        dmg_hider_frame = self.create_frame(
+                col_1_frame, size_policy=SMINMAX, style_override=hider_frame_style_override)
+        dmg_hider_frame.setMinimumWidth(self.sidebar_item_width)
+        self.set_buttons = list()
+        for i, head in enumerate(TREE_HEADER[1:]):
+            bt = self.create_button(
+                    head, 'toggle_button', dmg_hider_frame,
+                    toggle=self.settings.value(f'dmg_columns|{i}', type=bool))
+            bt.setSizePolicy(SMINMAX)
+            bt.clicked[bool].connect(
+                    lambda state, i=i: self.settings.setValue(f'dmg_columns|{i}', state))
+            dmg_hider_layout.addWidget(bt, stretch=1)
+        dmg_seperator = self.create_frame(
+                dmg_hider_frame, 'hr', style_override={'background-color': '@lbg'},
+                size_policy=SMINMIN)
+        dmg_seperator.setFixedHeight(self.theme['defaults']['bw'])
+        dmg_hider_layout.addWidget(dmg_seperator)
+        apply_button = self.create_button('Apply', 'button', dmg_hider_frame)
+        apply_button.clicked.connect(self.update_shown_columns_dmg)
+        dmg_hider_layout.addWidget(apply_button, alignment=ARIGHT | ATOP)
+        dmg_hider_frame.setLayout(dmg_hider_layout)
+        sec_2.addWidget(dmg_hider_frame, alignment=ATOP)
 
-        settings_frame.setLayout(settings_layout)
+        heal_hider_label = self.create_label(
+                'Heal table columns:', 'label_subhead')
+        sec_2.addWidget(heal_hider_label)
+        heal_hider_layout = QVBoxLayout()
+        heal_hider_frame = self.create_frame(
+                col_1_frame, size_policy=SMINMAX, style_override=hider_frame_style_override)
+        for i, head in enumerate(HEAL_TREE_HEADER[1:]):
+            bt = self.create_button(
+                    head, 'toggle_button', heal_hider_frame,
+                    toggle=self.settings.value(f'heal_columns|{i}', type=bool))
+            bt.setSizePolicy(SMINMAX)
+            bt.clicked[bool].connect(
+                    lambda state, i=i: self.settings.setValue(f'heal_columns|{i}', state))
+            heal_hider_layout.addWidget(bt, stretch=1)
+        heal_seperator = self.create_frame(
+            heal_hider_frame, 'hr', style_override={'background-color': '@lbg'},
+            size_policy=SMINMIN)
+        heal_seperator.setFixedHeight(self.theme['defaults']['bw'])
+        heal_hider_layout.addWidget(heal_seperator)
+        apply_button_2 = self.create_button('Apply', 'button', heal_hider_frame)
+        apply_button_2.clicked.connect(self.update_shown_columns_heal)
+        heal_hider_layout.addWidget(apply_button_2, alignment=ARIGHT | ATOP)
+        heal_hider_frame.setLayout(heal_hider_layout)
+
+        sec_2.addWidget(heal_hider_frame, alignment=ATOP)
+        live_hider_label = self.create_label(
+                'Live Parser columns:', 'label_subhead')
+        sec_2.addWidget(live_hider_label)
+        live_hider_layout = QVBoxLayout()
+        live_hider_frame = self.create_frame(
+                col_1_frame, size_policy=SMINMAX, style_override=hider_frame_style_override)
+        for i, head in enumerate(LIVE_TABLE_HEADER):
+            bt = self.create_button(
+                    head, 'toggle_button', live_hider_frame,
+                    toggle=self.settings.value(f'live_columns|{i}', type=bool))
+            bt.setSizePolicy(SMINMAX)
+            bt.clicked[bool].connect(
+                    lambda state, i=i: self.settings.setValue(f'live_columns|{i}', state))
+            live_hider_layout.addWidget(bt, stretch=1)
+        live_hider_frame.setLayout(live_hider_layout)
+        sec_2.addWidget(live_hider_frame, alignment=ATOP)
+
+        scroll_layout.addLayout(sec_2)
+
+        scroll_frame.setLayout(scroll_layout)
+        scroll_area.setWidget(scroll_frame)
```

### Comparing `oscr_ui-2024.4b20/OSCRUI/callbacks.py` & `oscr_ui-2024.5b270/OSCRUI/callbacks.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,17 +27,22 @@
 def save_combat(self, combat_num: int):
     """
     Callback for save button.
 
     Parameters:
     - :param combat_num: number of combat in self.combats
     """
-    if not self.parser1.active_combat:
+    combat = self.parser1.active_combat
+    if not combat:
         return
-    base_dir = os.path.dirname(self.entry.text())
+    filename = combat.map
+    if combat.difficulty is not None and combat.difficulty != '':
+        filename += ' ' + combat.difficulty
+    filename += f' {combat.start_time.strftime("%Y-%m-%d %H.%M")}.log'
+    base_dir = f'{os.path.dirname(self.entry.text())}/{filename}'
     if not base_dir:
         base_dir = self.app_dir
     path = self.browse_path(base_dir, 'Logfile (*.log);;Any File (*.*)', save=True)
     if path:
         self.parser1.export_combat(combat_num, path)
 
 
@@ -168,21 +173,45 @@
 
 
 def set_parser_opacity_setting(self, new_value: int):
     """
     Calculates new_value / 10 and stores it to settings.
 
     Parameters:
-    - :param new_value: data points per second
+    - :param new_value: 20 times the opacity percentage
     """
     setting_value = f'{new_value / 20:.2f}'
     self.settings.setValue('live_parser_opacity', setting_value)
     return setting_value
 
 
+def set_ui_scale_setting(self, new_value: int):
+    """
+    Calculates new_value / 50 and stores it to settings.
+
+    Parameters:
+    - :param new_value: 50 times the ui scale percentage
+    """
+    setting_value = f'{new_value / 50:.2f}'
+    self.settings.setValue('ui_scale', setting_value)
+    return setting_value
+
+
+def set_live_scale_setting(self, new_value: int):
+    """
+    Calculates new_value / 50 and stores it to settings.
+
+    Parameters:
+    - :param new_value: 50 times the live scale percentage
+    """
+    setting_value = f'{new_value / 50:.2f}'
+    self.settings.setValue('live_scale', setting_value)
+    return setting_value
+
+
 def set_sto_logpath_setting(self, entry: QLineEdit):
     """
     Formats and stores new logpath to settings.
 
     Parameters:
     - :param entry: the entry that holds the path
     """
@@ -240,15 +269,15 @@
     index_data = data_model._index
     cell_data = data_model._data
     visible_columns = list()
     for i in range(len(LIVE_TABLE_HEADER)):
         visible_columns.append(self.settings.value(f'live_columns|{i}', type=bool))
     output = list()
     for player_name, row in zip(index_data, cell_data):
-        output.append(f"{player_name}: {row[0]:,.2f} ({row[1]:.1f}s)")
+        output.append(f"`{player_name}`: {row[0]:,.2f} ({row[1]:.1f}s)")
     output = '{ OSCR } DPS (Combat time): ' + ' | '.join(output)
     self.app.clipboard().setText(output)
 
 
 def expand_overview_table(self):
     """
     Shows the overview table
```

### Comparing `oscr_ui-2024.4b20/OSCRUI/datafunctions.py` & `oscr_ui-2024.5b270/OSCRUI/datafunctions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import os
-import sys
 
 from OSCR import OSCR, HEAL_TREE_HEADER, TREE_HEADER
 from PySide6.QtCore import Qt, QThread, Signal
 
 from .callbacks import switch_main_tab, switch_overview_tab, trim_logfile
 from .datamodels import DamageTreeModel, HealTreeModel, TreeSelectionModel
 from .displayer import create_overview
@@ -120,15 +119,15 @@
     players = sorted(
         self.parser1.active_combat.player_dict.values(),
         reverse=True,
         key=lambda player: player.DPS,
     )
     parts = list()
     for player in players:
-        parts.append(f"{player.handle} {player.DPS:,.0f}")
+        parts.append(f"`{player.handle}` {player.DPS:,.0f}")
     summary += " | ".join(parts)
 
     self.app.clipboard().setText(summary)
 
 
 def get_data(self, combat: int | None = None, path: str | None = None):
     """
@@ -298,15 +297,15 @@
                     selection_dict[row_name][column] = cell_data
             output = ['{ OSCR }']
             for row_name, row_data in selection_dict.items():
                 formatted_row = list()
                 for col, value in row_data.items():
                     formatted_row.append(f'[{current_header[col]}] {format_function(value, col)}')
                 formatted_row_name = ''.join(row_name) if isinstance(row_name, tuple) else row_name
-                output.append(f"{formatted_row_name}: {' | '.join(formatted_row)}")
+                output.append(f"`{formatted_row_name}`: {' | '.join(formatted_row)}")
             output_string = '\n'.join(output)
             self.app.clipboard().setText(output_string)
     elif copy_mode == 'Global Max One Hit':
         if current_tab <= 1:
             max_one_hit_col = 4
             prefix = 'Max One Hit'
         else:
@@ -318,15 +317,15 @@
         max_one_hit, max_one_hit_item = max(max_one_hits, key=lambda x: x[0])
         max_one_hit_ability = max(
                 max_one_hit_item._children, key=lambda x: x.get_data(max_one_hit_col))
         max_one_hit_ability = max_one_hit_ability.get_data(0)
         if isinstance(max_one_hit_ability, tuple):
             max_one_hit_ability = ''.join(max_one_hit_ability)
         output_string = (f'{{ OSCR }} {prefix}: {max_one_hit:,.2f} '
-                         f'({"".join(max_one_hit_item.get_data(0))} – '
+                         f'(`{"".join(max_one_hit_item.get_data(0))}` – '
                          f'{max_one_hit_ability})')
         self.app.clipboard().setText(output_string)
     elif copy_mode == 'Max One Hit':
         if current_tab <= 1:
             max_one_hit_col = 4
             prefix = 'Max One Hit'
         else:
@@ -339,15 +338,15 @@
                 max_one_hit_item = max(
                         selected_row._children, key=lambda child: child.get_data(max_one_hit_col))
                 max_one_hit = max_one_hit_item.get_data(max_one_hit_col)
                 max_one_hit_ability = max_one_hit_item.get_data(0)
                 if isinstance(max_one_hit_ability, tuple):
                     max_one_hit_ability = ''.join(max_one_hit_ability)
                 output_string = (f'{{ OSCR }} {prefix}: {max_one_hit:,.2f} '
-                                 f'({"".join(selected_row.get_data(0))} – '
+                                 f'(`{"".join(selected_row.get_data(0))}` – '
                                  f'{max_one_hit_ability})')
                 self.app.clipboard().setText(output_string)
     elif copy_mode == 'Magnitude':
         if current_tab == 0:
             prefix = 'Total Damage Out'
         elif current_tab == 1:
             prefix = 'Total Damage Taken'
@@ -355,15 +354,15 @@
             prefix = 'Total Heal Out'
         else:
             prefix = 'Total Heal In'
         magnitudes = list()
         for player_item in current_table.model()._player._children:
             magnitudes.append((player_item.get_data(2), ''.join(player_item.get_data(0))))
         magnitudes.sort(key=lambda x: x[0], reverse=True)
-        magnitudes = [f"[{''.join(player)}] {magnitude:,.2f}" for magnitude, player in magnitudes]
+        magnitudes = [f"`[{''.join(player)}]` {magnitude:,.2f}" for magnitude, player in magnitudes]
         output_string = (f'{{ OSCR }} {prefix}: {" | ".join(magnitudes)}')
         self.app.clipboard().setText(output_string)
     elif copy_mode == 'Magnitude / s':
         if current_tab == 0:
             prefix = 'Total DPS Out'
         elif current_tab == 1:
             prefix = 'Total DPS Taken'
@@ -371,10 +370,10 @@
             prefix = 'Total HPS Out'
         else:
             prefix = 'Total HPS In'
         magnitudes = list()
         for player_item in current_table.model()._player._children:
             magnitudes.append((player_item.get_data(1), ''.join(player_item.get_data(0))))
         magnitudes.sort(key=lambda x: x[0], reverse=True)
-        magnitudes = [f"[{''.join(player)}] {magnitude:,.2f}" for magnitude, player in magnitudes]
+        magnitudes = [f"`[{''.join(player)}]` {magnitude:,.2f}" for magnitude, player in magnitudes]
         output_string = (f'{{ OSCR }} {prefix}: {" | ".join(magnitudes)}')
         self.app.clipboard().setText(output_string)
```

### Comparing `oscr_ui-2024.4b20/OSCRUI/datamodels.py` & `oscr_ui-2024.5b270/OSCRUI/datamodels.py`

 * *Files identical despite different names*

### Comparing `oscr_ui-2024.4b20/OSCRUI/displayer.py` & `oscr_ui-2024.5b270/OSCRUI/displayer.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,17 +104,14 @@
 
     table_layout = QVBoxLayout()
     table_layout.setContentsMargins(0, 0, 0, 0)
     table = create_overview_table(self, current_table)
     table_layout.addWidget(table)
     self.widgets.overview_table_frame.setLayout(table_layout)
     table.resizeColumnsToContents()
-    horizontal_header = table.horizontalHeader()
-    for col in range(len(TABLE_HEADER)):
-        horizontal_header.resizeSection(col, horizontal_header.sectionSize(col) + 5)
 
 
 @setup_plot
 def create_grouped_bar_plot(
         self, data: dict[str, tuple], time_reference: dict[str, tuple],
         bar_widget: PlotWidget) -> QVBoxLayout:
     """
@@ -129,14 +126,16 @@
     """
     bottom_axis = bar_widget.getAxis('bottom')
     bottom_axis.unit = 's'
     legend_data = list()
 
     group_width = 0.18
     player_num = len(data)
+    if player_num == 0:
+        return
     bar_width = group_width / player_num
     relative_bar_positions = np.linspace(0 + bar_width / 2, group_width - bar_width / 2, player_num)
     bar_position_offsets = relative_bar_positions - np.median(relative_bar_positions)
 
     zipper = zip(data.items(), self.theme['plot']['color_cycler'], bar_position_offsets)
     for (player, graph_data), color, offset in zipper:
         if player in time_reference:
@@ -294,38 +293,38 @@
 def create_live_graph(self) -> tuple[QFrame, list]:
     """
     Creates and styles live graph.
 
     :return: Frame containing the graph and list of curves that will be used to plot the data
     """
     plot_widget = PlotWidget()
-    plot_widget.setAxisItems({'left': CustomPlotAxis('left')})
-    plot_widget.setAxisItems({'bottom': CustomPlotAxis('bottom', unit='s')})
+    plot_widget.setAxisItems({'left': CustomPlotAxis('left', compressed=True)})
+    plot_widget.setAxisItems({'bottom': CustomPlotAxis('bottom', unit='s', no_labels=True)})
     plot_widget.setStyleSheet(get_style(self, 'plot_widget_nullifier'))
     plot_widget.setBackground(None)
     plot_widget.setMouseEnabled(False, False)
     plot_widget.setMenuEnabled(False)
     plot_widget.hideButtons()
     plot_widget.setDefaultPadding(padding=0)
     plot_widget.setXRange(-14, 0, padding=0)
     left_axis = plot_widget.getAxis('left')
-    left_axis.setTickFont(theme_font(self, 'plot_widget'))
+    left_axis.setTickFont(theme_font(self, 'live_plot_widget'))
     left_axis.setTextPen(color=self.theme['defaults']['fg'])
-    left_axis.setTickDensity(3)
+    # left_axis.setTickDensity(0.1)
     bottom_axis = plot_widget.getAxis('bottom')
     bottom_axis.setTickFont(theme_font(self, 'plot_widget'))
     bottom_axis.setTextPen(color=self.theme['defaults']['fg'])
 
     curves = list()
     for color_index in range(5):
         color = self.theme['plot']['color_cycler'][color_index]
         curves.append(plot_widget.plot([0], [0], pen=mkPen(color, width=1)))
 
     frame = create_frame(self, None, 'plot_widget', size_policy=SMIXMAX, style_override={
-            'margin-left': '@margin', 'margin-right': '@margin', 'margin-bottom': 0})
+            'margin': 4, 'padding': 2})
     frame.setMinimumWidth(self.sidebar_item_width * 0.25)
     frame.setMinimumHeight(self.sidebar_item_width * 0.25)
     layout = QHBoxLayout()
     layout.setContentsMargins(0, 0, 0, 0)
     layout.addWidget(plot_widget, stretch=1)
     frame.setLayout(layout)
     return frame, curves
```

### Comparing `oscr_ui-2024.4b20/OSCRUI/iofunctions.py` & `oscr_ui-2024.5b270/OSCRUI/iofunctions.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     allowed.
     Format: "<name of file type> (*.<extension>);;<name of file type> (*.<extension>);; [...]"
     Example: "Logfile (*.log);;Any File (*.*)"
     """
     if default_path is None or default_path == '':
         default_path = self.app_dir
     default_path = os.path.abspath(default_path)
-    if not os.path.exists(default_path):
+    if not os.path.exists(os.path.dirname(default_path)):
         default_path = self.app_dir
     if save:
         f = QFileDialog.getSaveFileName(self.window, 'Save Log', default_path, types)[0]
     else:
         f = QFileDialog.getOpenFileName(self.window, 'Open Log', default_path, types)[0]
         if not os.path.exists(f):
             return ''
```

### Comparing `oscr_ui-2024.4b20/OSCRUI/leagueconnector.py` & `oscr_ui-2024.5b270/OSCRUI/leagueconnector.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """Backend inteface to the OSCR web server"""
 
 import gzip
 import os
 import tempfile
 
 import OSCR_django_client
-from OSCR_django_client.api import CombatlogApi, LadderApi, LadderEntriesApi
 from OSCR.utilities import logline_to_str
+from OSCR_django_client.api import CombatlogApi, LadderApi, LadderEntriesApi
 from PySide6.QtWidgets import QMessageBox
 
-from .datafunctions import analyze_log_callback, CustomThread
+from .datafunctions import CustomThread, analyze_log_callback
 from .datamodels import LeagueTableModel, SortingProxy
-from .subwindows import show_warning
 from .style import theme_font
+from .subwindows import show_warning
 from .textedit import format_datetime_str
 
 LADDER_HEADER = (
     "Name",
     "Handle",
     "DPS",
     "Total Damage",
@@ -46,16 +46,17 @@
     """
     Retrieves maps from API and inserts them into the list.
     """
     ladders = self.league_api.ladders()
     if ladders is not None:
         self.widgets.ladder_selector.clear()
         for ladder in ladders.results:
-            solo = "[Solo] " if ladder.is_solo else ""
-            key = f"{solo}{ladder.metric} - {ladder.name} ({ladder.difficulty})"
+            solo = "[Solo]" if ladder.is_solo else ""
+            variant = f"[{ladder.variant_name}] " if ladder.variant_name != "Default" else ""
+            key = f"{variant}{ladder.name} ({ladder.difficulty}) {solo}"
             self.league_api.ladder_dict[key] = ladder
             self.widgets.ladder_selector.addItem(key)
 
 
 def apply_league_table_filter(self, filter_text: str):
     """
     Sets filter to proxy model of league table
@@ -104,37 +105,43 @@
                 row["max_one_hit"],
                 row["debuff"],
                 row.get("build", "Unknown"),
             )
         )
 
     model = LeagueTableModel(
-        table_data, LADDER_HEADER, table_index, theme_font(self, "table_header"),
-        theme_font(self, "table"), combatlog_id_list=logfile_ids)
+        table_data,
+        LADDER_HEADER,
+        table_index,
+        theme_font(self, "table_header"),
+        theme_font(self, "table"),
+        combatlog_id_list=logfile_ids,
+    )
     sorting_proxy = SortingProxy()
     sorting_proxy.setSourceModel(model)
     table = self.widgets.ladder_table
     table.setModel(sorting_proxy)
     table.resizeColumnsToContents()
-    table_header = table.horizontalHeader()
-    for col in range(len(model._header)):
-        table_header.resizeSection(col, table_header.sectionSize(col) + 5)
+    # table_header = table.horizontalHeader()
+    # for col in range(len(model._header)):
+    #     table_header.resizeSection(col, table_header.sectionSize(col) + 5)
 
 
 def extend_ladder(self):
     """
     Extends the ladder table by 50 newly fetched rows.
     """
     if self.league_api.entire_ladder_loaded:
         return
     if self.league_api.current_ladder_id is None:
         return
 
     ladder_data = self.league_api.ladder_entries(
-            self.league_api.current_ladder_id, self.league_api.pages_loaded + 1)
+        self.league_api.current_ladder_id, self.league_api.pages_loaded + 1
+    )
     if ladder_data is not None:
         if len(ladder_data.results) < 50:
             self.league_api.entire_ladder_loaded = True
         self.league_api.pages_loaded += 1
         table_index = list()
         table_data = list()
         logfile_ids = list()
@@ -152,16 +159,15 @@
                     row["combat_time"],
                     format_datetime_str(entry.var_date),
                     row["max_one_hit"],
                     row["debuff"],
                     row.get("build", "Unknown"),
                 )
             )
-        self.widgets.ladder_table.model().sourceModel().extend_data(
-                table_index, table_data, logfile_ids)
+        self.widgets.ladder_table.model().sourceModel().extend_data(table_index, table_data, logfile_ids)
 
 
 def download_and_view_combat(self):
     """
     Download a combat log and view its contents in the overview / analysis pages.
     """
     table = self.widgets.ladder_table
@@ -169,35 +175,33 @@
     selection = table.selectedIndexes()
     original_index = table.model().mapToSource(selection[0])
     row = original_index.row()
     log_id = table_model._combatlog_id_list[row]
     result = self.league_api.download(log_id)
     result = gzip.decompress(result)
     with tempfile.NamedTemporaryFile(
-            mode='w', encoding='utf-8', dir=self.config['templog_folder_path'],
-            delete=False) as file:
+        mode="w", encoding="utf-8", dir=self.config["templog_folder_path"], delete=False
+    ) as file:
         file.write(result.decode())
     analyze_log_callback(self, path=file.name, parser_num=1, hidden_path=True)
     self.switch_overview_tab(0)
     self.switch_main_tab(0)
 
 
 def upload_callback(self):
     """
     Helper function to grab the current combat and upload it to the backend.
     """
-    show_warning(self, 'OSCR', 'Uploads are temporarily disabled.')
-    return
     if self.parser1.active_combat is None or self.parser1.active_combat.log_data is None:
-        show_warning(self, 'OSCR - Logfile Upload', 'No data to upload.')
+        show_warning(self, "OSCR - Logfile Upload", "No data to upload.")
         return
 
     establish_league_connection(self)
 
-    with tempfile.NamedTemporaryFile(dir=self.config['templog_folder_path'], delete=False) as file:
+    with tempfile.NamedTemporaryFile(dir=self.config["templog_folder_path"], delete=False) as file:
         data = gzip.compress(
             "".join([logline_to_str(line) for line in self.parser1.active_combat.log_data]).encode()
         )
         file.write(data)
         file.flush()
     self.league_api.upload(file.name)
     os.remove(file.name)
@@ -205,16 +209,15 @@
 
 class OSCRClient:
     def __init__(self, address=None):
         """Initialize an instance of the OSCR backlend client"""
 
         # TODO: This is a test domain and not for production.
         if not address:
-            self.address = "https://oscr-server.vercel.app"
-            # self.address = "http://127.0.0.1:8000"
+            self.address = "https://oscr.stobuilds.com"
 
         self.api_client = OSCR_django_client.api_client.ApiClient()
         self.api_client.configuration.host = self.address
         self.api_combatlog = CombatlogApi(api_client=self.api_client)
         self.api_ladder = LadderApi(api_client=self.api_client)
         self.api_ladder_entries = LadderEntriesApi(api_client=self.api_client)
         self.ladder_dict: dict = dict()
@@ -231,38 +234,50 @@
         try:
             res = self.api_combatlog.combatlog_upload(file=filename)
             lines = []
             for entry in res:
                 lines.append(entry.detail)
             reply.setText("\n".join(lines))
         except OSCR_django_client.exceptions.ServiceException as e:
-            reply.setText(str(e))
+            try:
+                data = json.loads(e.body)
+                reply.setText(data.get("detail", "Failed to parse error from server"))
+            except Exception as e:
+                reply.setText("Failed to parse error from server")
 
         reply.exec()
 
     def download(self, id):
         """Download a combat log"""
         try:
             return self.api_combatlog.combatlog_download(id=id)
         except OSCR_django_client.exceptions.ServiceException as e:
             reply = QMessageBox()
             reply.setWindowTitle("Open Source Combatlog Reader")
-            reply.setText(str(e))
+            try:
+                data = json.loads(e.body)
+                reply.setText(data.get("detail", "Failed to parse error from server"))
+            except Exception as e:
+                reply.setText("Failed to parse error from server")
             reply.exec()
 
         return None
 
     def ladders(self):
         """Fetch the list of ladders"""
         try:
             return self.api_ladder.ladder_list()
         except OSCR_django_client.exceptions.ServiceException as e:
             reply = QMessageBox()
             reply.setWindowTitle("Open Source Combatlog Reader")
-            reply.setText(str(e))
+            try:
+                data = json.loads(e.body)
+                reply.setText(data.get("detail", "Failed to parse error from server"))
+            except Exception as e:
+                reply.setText("Failed to parse error from server")
             reply.exec()
 
         return None
 
     def ladder_entries(self, id, page=1):
         """Fetch the nth page of ladder entries"""
         try:
@@ -271,11 +286,15 @@
                 page=page,
                 ordering="-data__DPS",
                 page_size=50,
             )
         except OSCR_django_client.exceptions.ServiceException as e:
             reply = QMessageBox()
             reply.setWindowTitle("Open Source Combatlog Reader")
-            reply.setText(str(e))
+            try:
+                data = json.loads(e.body)
+                reply.setText(data.get("detail", "Failed to parse error from server"))
+            except Exception as e:
+                reply.setText("Failed to parse error from server")
             reply.exec()
 
         return None
```

### Comparing `oscr_ui-2024.4b20/OSCRUI/style.py` & `oscr_ui-2024.5b270/OSCRUI/style.py`

 * *Files 7% similar despite different names*

```diff
@@ -87,25 +87,26 @@
 
 def get_css(self, style: dict) -> str:
     """
     Converts style dictionary into css style sheet. Escapes '@' - shortcuts with their respective
     values.
     """
     css = str()
+    ui_scale = self.config['ui_scale']
     for key, val in style.items():
-        if isinstance(val, str) and val[0] == '@':
+        if isinstance(val, str) and val.startswith('@'):
             v = self.theme['defaults'][val[1:]]
         else:
             v = val
         if key.startswith(':') or key.startswith('~') or key == 'font':
             continue
         elif isinstance(v, int):
-            css += f'{key}:{v}px;'
+            css += f'{key}:{v * ui_scale}px;'
         elif isinstance(v, tuple):
-            css += f'''{key}:{'px '.join(map(str, v))}px;'''
+            css += f'''{key}:{'px '.join(map(lambda s: str(s * ui_scale), v))}px;'''
         else:
             css += f'{key}:{v};'
     return css
 
 
 def theme_font(self, key, font_spec=()) -> QFont:
     """
@@ -124,19 +125,20 @@
         if isinstance(font_spec, str) and font_spec.startswith('@'):
             font = self.theme['defaults'][font_spec[1:]]
         else:
             font = font_spec
     except KeyError:
         font = self.theme['app']['font']
     font_family = (font[0], *self.theme['app']['font-fallback'])
+    font_size = int(font[1] * self.config['ui_scale'])
     try:
         font_weight = WEIGHT_CONVERSION[font[2]]
     except KeyError:
         font_weight = QFont.Weight.Normal
-    return QFont(font_family, font[1], font_weight)
+    return QFont(font_family, font_size, font_weight)
 
 
 def create_style_sheet(self, d: dict) -> str:
     """
     Creates Stylesheet from dictionary. Dictionary keys represent css selector.
 
     Parameters:
```

### Comparing `oscr_ui-2024.4b20/OSCRUI/subwindows.py` & `oscr_ui-2024.5b270/OSCRUI/subwindows.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import os
 
-from PySide6.QtCore import QPoint, Qt
+from PySide6.QtCore import QPoint, QSize, Qt
 from PySide6.QtGui import QIntValidator, QMouseEvent
 from PySide6.QtWidgets import QAbstractItemView, QDialog
 from PySide6.QtWidgets import QGridLayout, QHBoxLayout, QLineEdit
-from PySide6.QtWidgets import QMessageBox, QSpacerItem, QTableView
+from PySide6.QtWidgets import QMessageBox, QSpacerItem, QSplitter, QTableView
 from PySide6.QtWidgets import QVBoxLayout
 
 from OSCR import LiveParser, LIVE_TABLE_HEADER
 from .callbacks import (
         auto_split_callback, combat_split_callback, copy_live_data_callback, trim_logfile)
 from .displayer import create_live_graph, update_live_display, update_live_graph, update_live_table
 from .datamodels import LiveParserTableModel
 from .style import get_style, get_style_class, theme_font
 from .textedit import format_path
 from .widgetbuilder import create_button, create_frame, create_icon_button, create_label
-from .widgetbuilder import ABOTTOM, ALEFT, ARIGHT, AVCENTER, RFIXED
-from .widgetbuilder import SEXPAND, SMAX, SMAXMAX, SMINMIN
+from .widgetbuilder import ABOTTOM, AHCENTER, ALEFT, ARIGHT, AVCENTER, RFIXED
+from .widgetbuilder import SEXPAND, SMAX, SMAXMAX, SMINMAX, SMINMIN
 from .widgets import FlipButton, LiveParserWindow, SizeGrip
 
 
 def show_warning(self, title: str, message: str):
     """
     Displays a warning in form of a message box
 
@@ -188,14 +188,73 @@
     dialog.setLayout(main_layout)
     dialog.setWindowTitle('OSCR - Split Logfile')
     dialog.setStyleSheet(get_style(self, 'dialog_window'))
     dialog.setSizePolicy(SMAXMAX)
     dialog.exec()
 
 
+def uploadresult_dialog(self, result):
+    """
+    Shows a dialog that informs about the result of the triggered upload.
+
+    Paramters:
+    - :param result: dict containing result
+    """
+    dialog = QDialog(self.window)
+    main_layout = QVBoxLayout()
+    thick = self.theme['app']['frame_thickness']
+    main_layout.setContentsMargins(thick, thick, thick, thick)
+    content_frame = create_frame(self)
+    main_layout.addWidget(content_frame)
+    content_layout = QGridLayout()
+    content_layout.setContentsMargins(thick, thick, thick, thick)
+    content_layout.setSpacing(0)
+    margin = {'margin-bottom': self.theme['defaults']['isp']}
+    title_label = create_label(self, 'Upload Results:', 'label_heading', style_override=margin)
+    content_layout.addWidget(title_label, 0, 0, 1, 4, alignment=ALEFT)
+    icon_size = QSize(self.config['icon_size'] / 1.5, self.config['icon_size'] / 1.5)
+    for row, line in enumerate(result, 1):
+        if row % 2 == 1:
+            table_style = {'background-color': '@mbg', 'padding': (5, 3, 3, 3), 'margin': 0}
+            icon_table_style = {'background-color': '@mbg', 'padding': (3, 3, 3, 3), 'margin': 0}
+        else:
+            table_style = {'background-color': '@bg', 'padding': (5, 3, 3, 3), 'margin': 0}
+            icon_table_style = {'background-color': '@bg', 'padding': (3, 3, 3, 3), 'margin': 0}
+        if line['updated']:
+            icon = self.icons['check'].pixmap(icon_size)
+        else:
+            icon = self.icons['dash'].pixmap(icon_size)
+        status_label = create_label(self, '', style_override=icon_table_style)
+        status_label.setPixmap(icon)
+        status_label.setSizePolicy(SMINMIN)
+        content_layout.addWidget(status_label, row, 0)
+        name_label = create_label(self, line['name'], style_override=table_style)
+        name_label.setSizePolicy(SMINMAX)
+        content_layout.addWidget(name_label, row, 1)
+        value_label = create_label(self, str(line['value']), style_override=table_style)
+        value_label.setSizePolicy(SMINMAX)
+        value_label.setAlignment(ARIGHT)
+        content_layout.addWidget(value_label, row, 2)
+        detail_label = create_label(self, line['detail'], style_override=table_style)
+        detail_label.setSizePolicy(SMINMAX)
+        content_layout.addWidget(detail_label, row, 3)
+    top_margin = {'margin-top': self.theme['defaults']['isp']}
+    close_button = create_button(self, 'Close', style_override=top_margin)
+    close_button.clicked.connect(dialog.close)
+    content_layout.addWidget(close_button, row + 1, 0, 1, 4, alignment=AHCENTER)
+    content_frame.setLayout(content_layout)
+
+    dialog.setLayout(main_layout)
+    dialog.setWindowTitle('OSCR - Upload Results')
+    dialog.setStyleSheet(get_style(self, 'dialog_window'))
+    dialog.setSizePolicy(SMAXMAX)
+    dialog.setFixedSize(dialog.sizeHint())
+    dialog.exec()
+
+
 def live_parser_toggle(self, activate):
     """
     Activates / Deactivates LiveParser.
 
     Parameters:
     - :param activate: True when parser should be shown; False when open parser should be closed.
     """
@@ -226,18 +285,25 @@
             pass
         self.live_parser_window.update_table.disconnect()
         self.live_parser_window.update_graph.disconnect()
         self.live_parser_window.deleteLater()
         self.live_parser_window = None
         self.live_parser = None
         self.widgets.live_parser_table = None
+        self.widgets.live_parser_splitter = None
         self.widgets.live_parser_button.setChecked(False)
 
 
 def create_live_parser_window(self):
+    """
+    Creates the LiveParser window.
+    """
+    ui_scale = self.config['ui_scale']
+    self.config['ui_scale'] = self.config['live_scale']
+
     live_window = LiveParserWindow()
     live_window.setStyleSheet(get_style(self, 'live_parser'))
     live_window.setWindowFlags(
             live_window.windowFlags()
             | Qt.WindowType.WindowStaysOnTopHint
             | Qt.WindowType.WindowDoesNotAcceptFocus
             | Qt.WindowType.SubWindow
@@ -252,93 +318,113 @@
     live_window.setSizePolicy(SMAXMAX)
     layout = QVBoxLayout()
     layout.setContentsMargins(0, 0, 0, 0)
     layout.setSpacing(0)
 
     graph_colors = None
     graph_column = None
-    if self.settings.value('live_graph_active', type=bool):
+    graph_active = self.settings.value('live_graph_active', type=bool)
+    if graph_active:
+        splitter = QSplitter(Qt.Orientation.Vertical)
+        splitter.setStyleSheet(get_style_class(self, 'QSplitter', 'splitter'))
+        splitter.setChildrenCollapsible(False)
+        self.widgets.live_parser_splitter = splitter
         graph_frame, curves = create_live_graph(self)
-        layout.addWidget(graph_frame, stretch=1)
+        graph_frame.setMinimumHeight(self.sidebar_item_width * 0.1)
+        splitter.addWidget(graph_frame)
         self.widgets.live_parser_curves = curves
         FIELD_INDEX_CONVERSION = {0: 0, 1: 2, 2: 3, 3: 4}
         graph_column = FIELD_INDEX_CONVERSION[self.settings.value('live_graph_field', type=int)]
         graph_colors = self.theme['plot']['color_cycler'][:5]
+        table_layout = splitter
+        layout.addWidget(splitter, stretch=1)
+    else:
+        table_layout = layout
 
     table = QTableView()
     table.setAlternatingRowColors(self.theme['s.c']['table_alternate'])
     table.setShowGrid(self.theme['s.c']['table_gridline'])
     table.setStyleSheet(get_style_class(self, 'QTableView', 'live_table'))
     table.setVerticalScrollBarPolicy(Qt.ScrollBarPolicy.ScrollBarAlwaysOff)
     table.setHorizontalScrollBarPolicy(Qt.ScrollBarPolicy.ScrollBarAlwaysOff)
     table.horizontalHeader().setStyleSheet(
             get_style_class(self, 'QHeaderView', 'live_table_header'))
     table.verticalHeader().setStyleSheet(get_style_class(self, 'QHeaderView', 'live_table_index'))
+    table.verticalHeader().setMinimumHeight(1)
+    table.verticalHeader().setDefaultSectionSize(1)
+    table.horizontalHeader().setMinimumWidth(1)
+    table.horizontalHeader().setDefaultSectionSize(1)
     table.horizontalHeader().setSectionResizeMode(RFIXED)
     table.verticalHeader().setSectionResizeMode(RFIXED)
     table.setSizePolicy(SMINMIN)
     table.setSelectionMode(QAbstractItemView.SelectionMode.NoSelection)
-    table.setMinimumWidth(self.sidebar_item_width * 0.25)
-    table.setMinimumHeight(self.sidebar_item_width * 0.25)
+    table.setMinimumWidth(self.sidebar_item_width * 0.1)
+    table.setMinimumHeight(self.sidebar_item_width * 0.1)
     model = LiveParserTableModel(
             [[0] * len(LIVE_TABLE_HEADER)], LIVE_TABLE_HEADER, [''],
             theme_font(self, 'live_table_header'), theme_font(self, 'live_table'),
             legend_col=graph_column, colors=graph_colors)
     table.setModel(model)
     table.resizeColumnsToContents()
     table.resizeRowsToContents()
     for index in range(len(LIVE_TABLE_HEADER)):
         if not self.settings.value(f'live_columns|{index}', type=bool):
             table.hideColumn(index)
     self.widgets.live_parser_table = table
-    layout.addWidget(table, stretch=1)
+    table_layout.addWidget(table)
+
+    if graph_active and self.settings.value('live_splitter'):
+        table_layout.restoreState(self.settings.value('live_splitter'))
 
     bottom_layout = QGridLayout()
     bottom_layout.setContentsMargins(self.theme['defaults']['isp'], 0, 0, 0)
     bottom_layout.setSpacing(0)
     bottom_layout.setColumnStretch(0, 1)
     bottom_layout.setColumnStretch(2, 1)
 
+    icon_size = [self.theme['s.c']['button_icon_size'] * self.config['live_scale'] * 0.8] * 2
     copy_button = copy_button = create_icon_button(
-            self, self.icons['copy'], 'Copy Result', style_override={'margin-bottom': '@margin'},
-            icon_size=[self.theme['s.c']['button_icon_size'] * 0.8] * 2)
+            self, self.icons['copy'], 'Copy Result', icon_size=icon_size)
     copy_button.clicked.connect(lambda: copy_live_data_callback(self))
     bottom_layout.addWidget(copy_button, 0, 0, alignment=ARIGHT | AVCENTER)
     activate_button = FlipButton('Activate', 'Deactivate', live_window, checkable=True)
     activate_button.setStyleSheet(self.get_style_class(
-            'QPushButton', 'toggle_button', {'margin': (1, 8, 10, 8)}))
+            'QPushButton', 'toggle_button', {'margin': (0, 8, 0, 8)}))
     activate_button.setFont(self.theme_font('app', '@subhead'))
     activate_button.r_function = lambda: self.live_parser.start()
     activate_button.l_function = lambda: self.live_parser.stop()
     bottom_layout.addWidget(activate_button, 0, 1, alignment=AVCENTER)
     close_button = create_icon_button(
-            self, self.icons['close'], 'Close Live Parser',
-            style_override={'margin-bottom': '@margin'},
-            icon_size=[self.theme['s.c']['button_icon_size'] * 0.8] * 2)
+            self, self.icons['close'], 'Close Live Parser', icon_size=icon_size)
     close_button.clicked.connect(lambda: live_parser_toggle(self, False))
     bottom_layout.addWidget(close_button, 0, 2, alignment=ALEFT | AVCENTER)
 
     grip = SizeGrip(live_window)
     grip.setStyleSheet(get_style(self, 'resize_handle'))
     bottom_layout.addWidget(grip, 0, 3, alignment=ARIGHT | ABOTTOM)
 
     layout.addLayout(bottom_layout)
     live_window.setLayout(layout)
     live_window.update_table.connect(lambda data: update_live_table(self, data))
     live_window.update_graph.connect(update_live_graph)
     self.live_parser_window = live_window
+    self.config['ui_scale'] = ui_scale
     live_window.show()
 
 
 def live_parser_close_callback(self, event):
     """
     Executed when application is closed.
     """
     window_geometry = self.live_parser_window.saveGeometry()
     self.settings.setValue('live_geometry', window_geometry)
+    try:
+        self.settings.setValue('live_splitter', self.widgets.live_parser_splitter.saveState())
+    except AttributeError:
+        pass
     event.accept()
 
 
 def live_parser_press_event(self, event: QMouseEvent):
     self.live_parser_window.start_pos = event.globalPosition().toPoint()
     event.accept()
```

### Comparing `oscr_ui-2024.4b20/OSCRUI/textedit.py` & `oscr_ui-2024.5b270/OSCRUI/textedit.py`

 * *Files identical despite different names*

### Comparing `oscr_ui-2024.4b20/OSCRUI/widgetbuilder.py` & `oscr_ui-2024.5b270/OSCRUI/widgetbuilder.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,17 +28,19 @@
 ALEFT = Qt.AlignmentFlag.AlignLeft
 ACENTER = Qt.AlignmentFlag.AlignCenter
 AVCENTER = Qt.AlignmentFlag.AlignVCenter
 AHCENTER = Qt.AlignmentFlag.AlignHCenter
 
 RFIXED = QHeaderView.ResizeMode.Fixed
 
-
 SMPIXEL = QAbstractItemView.ScrollMode.ScrollPerPixel
 
+SCROLLOFF = Qt.ScrollBarPolicy.ScrollBarAlwaysOff
+SCROLLON = Qt.ScrollBarPolicy.ScrollBarAlwaysOn
+
 
 def create_button(self, text, style: str = 'button', parent=None, style_override={}, toggle=None):
     """
     Creates a button according to style with parent.
 
     Parameters:
     - :param text: text to be shown on the button
@@ -82,15 +84,15 @@
     """
     button = QPushButton('', parent)
     button.setIcon(icon)
     if tooltip:
         button.setToolTip(tooltip)
     button.setStyleSheet(get_style_class(self, 'QPushButton', style, style_override))
     if len(icon_size) != 2:
-        icon_size = [self.theme['s.c']['button_icon_size']] * 2
+        icon_size = [self.config['icon_size']] * 2
     button.setIconSize(QSize(*icon_size))
     button.setCursor(Qt.CursorShape.PointingHandCursor)
     button.setSizePolicy(SMAXMAX)
     return button
 
 
 def create_frame(self, parent=None, style='frame', style_override={}, size_policy=None) -> QFrame:
@@ -357,14 +359,16 @@
     table.setShowGrid(self.theme['s.c']['table_gridline'])
     table.setSortingEnabled(True)
     table.setStyleSheet(get_style_class(self, 'QTableView', 'table', style_override))
     table.setHorizontalScrollMode(SMPIXEL)
     table.setVerticalScrollMode(SMPIXEL)
     table.horizontalHeader().setStyleSheet(get_style_class(self, 'QHeaderView', 'table_header'))
     table.verticalHeader().setStyleSheet(get_style_class(self, 'QHeaderView', 'table_index'))
+    table.verticalHeader().setMinimumHeight(1)
+    table.verticalHeader().setDefaultSectionSize(1)
     table.resizeColumnsToContents()
     table.resizeRowsToContents()
     table.horizontalHeader().setSortIndicatorShown(False)
     table.horizontalHeader().setSectionResizeMode(RFIXED)
     table.verticalHeader().setSectionResizeMode(RFIXED)
     table.setSizePolicy(SMINMIN)
     if single_row_selection:
```

### Comparing `oscr_ui-2024.4b20/OSCRUI/widgets.py` & `oscr_ui-2024.5b270/OSCRUI/widgets.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+from math import sqrt, floor, frexp
+
 import numpy as np
 from pyqtgraph import AxisItem, BarGraphItem, PlotWidget
 from PySide6.QtCore import QRect, Qt, Signal, Slot
 from PySide6.QtGui import QIcon, QMouseEvent, QPixmap, QPainter, QFont
-from PySide6.QtWidgets import QComboBox, QFrame, QListWidget, QPushButton, QSizeGrip, QTableView
-from PySide6.QtWidgets import QTabWidget, QTreeView, QWidget
+from PySide6.QtWidgets import QComboBox, QFrame, QListWidget, QPushButton, QSizeGrip, QSplitter
+from PySide6.QtWidgets import QTableView, QTabWidget, QTreeView, QWidget
 
 from .widgetbuilder import SMINMIN
 
 
 class WidgetStorage():
     """
     Class to store widgets.
@@ -48,14 +50,15 @@
         self.favorite_ladder_selector: QListWidget
         self.season_ladder_selector: QListWidget
         self.ladder_table: QTableView
 
         self.live_parser_table: QTableView
         self.live_parser_button: QPushButton
         self.live_parser_curves: list
+        self.live_parser_splitter: QSplitter
 
     @property
     def analysis_table(self):
         return (self.analysis_table_dout, self.analysis_table_dtaken, self.analysis_table_hout,
                 self.analysis_table_hin)
 
 
@@ -171,40 +174,120 @@
             self.setMinimumHeight(h)
 
 
 class CustomPlotAxis(AxisItem):
     """
     Extending AxisItem for custom tick formatting
     """
-    def __init__(self, *args, unit: str = '', **kwargs):
+    def __init__(self, *args, unit: str = '', no_labels=False, compressed=False, **kwargs):
         super().__init__(*args, **kwargs)
         self._unit = ' ' + unit
+        self._no_labels = no_labels
+        self._compressed = compressed
 
     @property
     def unit(self):
         return self._unit
 
     @unit.setter
     def unit(self, value):
         self._unit = ' ' + value
 
     def tickStrings(self, values, scale, spacing):
+        if self._no_labels:
+            return []
+
         if self.logMode:
             return self.logTickStrings(values, scale, spacing)
 
         strings = list()
         for tick in values:
             if tick >= 1000000:
                 strings.append(f'{tick / 1000000:.2f} M{self._unit}')
             elif tick >= 1000:
                 strings.append(f'{tick / 1000:.0f} k{self._unit}')
             else:
                 strings.append(f'{tick:.0f}{self._unit}')
         return strings
 
+    def tickSpacing(self, minVal, maxVal, size):
+        """Return values describing the desired spacing and offset of ticks.
+
+        This method is called whenever the axis needs to be redrawn and is a
+        good method to override in subclasses that require control over tick locations.
+
+        The return value must be a list of tuples, one for each set of ticks::
+
+            [
+                (major tick spacing, offset),
+                (minor tick spacing, offset),
+                (sub-minor tick spacing, offset),
+                ...
+            ]
+        """
+        # almost the original implementation of tickSpacing
+        if self._tickSpacing is not None:
+            return self._tickSpacing
+
+        dif = abs(maxVal - minVal)
+        if dif == 0:
+            return []
+
+        ref_size = 300.
+        minNumberOfIntervals = max(2.25, 2.25 * self._tickDensity * sqrt(size / ref_size))
+
+        majorMaxSpacing = dif / minNumberOfIntervals
+
+        mantissa, exp2 = frexp(majorMaxSpacing)
+        p10unit = 10. ** (floor((exp2 - 1) / 3.32192809488736) - 1)
+        if 100. * p10unit <= majorMaxSpacing:
+            majorScaleFactor = 10
+            p10unit *= 10.
+        else:
+            if self._compressed:
+                scale_factors = (50, 30, 20, 10)
+            else:
+                scale_factors = (50, 20, 10)
+            for majorScaleFactor in scale_factors:
+                if majorScaleFactor * p10unit <= majorMaxSpacing:
+                    break
+        majorInterval = majorScaleFactor * p10unit
+
+        minorMinSpacing = 2 * dif / size
+        if majorScaleFactor == 10:
+            trials = (5, 10)
+        else:
+            trials = (10, 20, 50)
+        for minorScaleFactor in trials:
+            minorInterval = minorScaleFactor * p10unit
+            if minorInterval >= minorMinSpacing:
+                break
+        levels = [
+            (majorInterval, 0),
+            (minorInterval, 0)
+        ]
+
+        if self.style['maxTickLevel'] >= 2:
+            if majorScaleFactor == 10:
+                trials = (1, 2, 5, 10)
+            elif majorScaleFactor == 20:
+                trials = (2, 5, 10, 20)
+            elif majorScaleFactor == 50:
+                trials = (5, 10, 50)
+            else:
+                trials = ()
+                extraInterval = minorInterval
+            for extraScaleFactor in trials:
+                extraInterval = extraScaleFactor * p10unit
+                if extraInterval >= minorMinSpacing or extraInterval == minorInterval:
+                    break
+            if extraInterval < minorInterval:
+                levels.append((extraInterval, 0))
+        return levels
+
 
 class AnalysisPlot(PlotWidget):
     """
     PlotWidget for plotting the analysis plot.
     """
     def __init__(self, colors: tuple, tick_color: str, tick_font: QFont, legend_layout):
         """
```

### Comparing `oscr_ui-2024.4b20/assets/Overpass-Bold.ttf` & `oscr_ui-2024.5b270/assets/Overpass-Bold.ttf`

 * *Files identical despite different names*

### Comparing `oscr_ui-2024.4b20/assets/Overpass-Medium.ttf` & `oscr_ui-2024.5b270/assets/Overpass-Medium.ttf`

 * *Files identical despite different names*

### Comparing `oscr_ui-2024.4b20/assets/Overpass-Regular.ttf` & `oscr_ui-2024.5b270/assets/Overpass-Regular.ttf`

 * *Files identical despite different names*

### Comparing `oscr_ui-2024.4b20/assets/RobotoMono-Medium.ttf` & `oscr_ui-2024.5b270/assets/RobotoMono-Medium.ttf`

 * *Files identical despite different names*

### Comparing `oscr_ui-2024.4b20/assets/RobotoMono-Regular.ttf` & `oscr_ui-2024.5b270/assets/RobotoMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `oscr_ui-2024.4b20/assets/oscr_icon_small.ico` & `oscr_ui-2024.5b270/assets/oscr_icon_small.ico`

 * *Files identical despite different names*

### Comparing `oscr_ui-2024.4b20/assets/oscr_icon_small.png` & `oscr_ui-2024.5b270/assets/oscr_icon_small.png`

 * *Files identical despite different names*

### Comparing `oscr_ui-2024.4b20/assets/oscrbanner-slim-dark-label.png` & `oscr_ui-2024.5b270/assets/oscrbanner-slim-dark-label.png`

 * *Files identical despite different names*

### Comparing `oscr_ui-2024.4b20/assets/section31badge.png` & `oscr_ui-2024.5b270/assets/section31badge.png`

 * *Files identical despite different names*

### Comparing `oscr_ui-2024.4b20/assets/stobuildslogo.png` & `oscr_ui-2024.5b270/assets/stobuildslogo.png`

 * *Files identical despite different names*

### Comparing `oscr_ui-2024.4b20/LICENSE` & `oscr_ui-2024.5b270/LICENSE`

 * *Files identical despite different names*

### Comparing `oscr_ui-2024.4b20/pyproject.toml` & `oscr_ui-2024.5b270/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "OSCR-UI"
 dependencies = [
   "PySide6>=6.6.0",
   "pyqtgraph>=0.13.4",
   "numpy>=1.26.1",
-  "STO-OSCR>=2024.4b20",
+  "STO-OSCR>=2024.5b270",
   "OSCR-django-client>=2024.3b40",
 ]
 requires-python = ">=3.10"
 authors = []
 maintainers = []
 description = " Frontend for the OSCR parser."
 readme = "README.md"
```

### Comparing `oscr_ui-2024.4b20/PKG-INFO` & `oscr_ui-2024.5b270/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: OSCR-UI
-Version: 2024.4b20
+Version: 2024.5b270
 Summary:  Frontend for the OSCR parser.
 Project-URL: Homepage, https://github.com/STOCD/OSCR-UI
 Project-URL: Repository, https://github.com/STOCD/OSCR-UI.git
 Project-URL: Bug Tracker, https://github.com/STOCD/OSCR-UI/issues
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
@@ -683,28 +683,29 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.10
 Requires-Dist: numpy>=1.26.1
 Requires-Dist: oscr-django-client>=2024.3b40
 Requires-Dist: pyqtgraph>=0.13.4
 Requires-Dist: pyside6>=6.6.0
-Requires-Dist: sto-oscr>=2024.4b20
+Requires-Dist: sto-oscr>=2024.5b270
 Provides-Extra: cli
 Provides-Extra: gui
 Description-Content-Type: text/markdown
 
 # OSCR-UI
 
 [![PyPI version](https://badge.fury.io/py/OSCR-UI.svg)](https://badge.fury.io/py/OSCR-UI)
 
 User Interface for the OSCR parser. 
 
 # Windows Users
 
 For Windows users we have pre-compiled standalone binaries available on the [Releases](https://github.com/STOCD/OSCR-UI/releases) page.
+
 # Installation
 
 ## PyPI
 
 ```bash
 python3 -m pip install OSCR-UI
 ```
@@ -738,7 +739,14 @@
 
 # Linux
 source ./venv/bin/activate
 
 # Install OSCR + Requirements.
 python3 -m pip install .
 ```
+
+# Companion Web Application
+
+The STOCD team provides a companion web application for OSCR located at [oscr.stobuilds.com](https://oscr.stobuilds.com).
+This allows users to view and download combat log data without OSCR installed, however uploads
+and more detailed analysis of combat logs requires OSCR or a parser that supports
+interracting with OSCR's backend such as [CLA](https://github.com/AnotherNathan/STO_CombatLogAnalyzer).
```

