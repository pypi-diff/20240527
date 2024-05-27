# Comparing `tmp/zimo-web-screenshot-0.2.0.tar.gz` & `tmp/zimo-web-screenshot-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zimo-web-screenshot-0.2.0.tar", last modified: Sun Apr 21 14:51:49 2024, max compression
+gzip compressed data, was "zimo-web-screenshot-0.3.0.tar", last modified: Mon May 27 12:09:40 2024, max compression
```

## Comparing `zimo-web-screenshot-0.2.0.tar` & `zimo-web-screenshot-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 zimoluo    (501) staff       (20)        0 2024-04-21 14:51:49.452212 zimo-web-screenshot-0.2.0/
--rw-r--r--   0 zimoluo    (501) staff       (20)     1057 2024-04-15 05:14:35.000000 zimo-web-screenshot-0.2.0/LICENSE
--rw-r--r--   0 zimoluo    (501) staff       (20)     2162 2024-04-21 14:51:49.452296 zimo-web-screenshot-0.2.0/PKG-INFO
--rw-r--r--   0 zimoluo    (501) staff       (20)     1657 2024-04-15 11:41:59.000000 zimo-web-screenshot-0.2.0/README.md
--rw-r--r--   0 zimoluo    (501) staff       (20)       79 2024-04-21 14:51:49.452510 zimo-web-screenshot-0.2.0/setup.cfg
--rw-r--r--   0 zimoluo    (501) staff       (20)      888 2024-04-21 14:46:41.000000 zimo-web-screenshot-0.2.0/setup.py
-drwxr-xr-x   0 zimoluo    (501) staff       (20)        0 2024-04-21 14:51:49.451124 zimo-web-screenshot-0.2.0/zimo_web_screenshot/
--rw-r--r--   0 zimoluo    (501) staff       (20)        0 2024-04-15 10:38:36.000000 zimo-web-screenshot-0.2.0/zimo_web_screenshot/__init__.py
--rw-r--r--   0 zimoluo    (501) staff       (20)     2753 2024-04-21 14:49:44.000000 zimo-web-screenshot-0.2.0/zimo_web_screenshot/screenshot.py
-drwxr-xr-x   0 zimoluo    (501) staff       (20)        0 2024-04-21 14:51:49.452094 zimo-web-screenshot-0.2.0/zimo_web_screenshot.egg-info/
--rw-r--r--   0 zimoluo    (501) staff       (20)     2162 2024-04-21 14:51:49.000000 zimo-web-screenshot-0.2.0/zimo_web_screenshot.egg-info/PKG-INFO
--rw-r--r--   0 zimoluo    (501) staff       (20)      362 2024-04-21 14:51:49.000000 zimo-web-screenshot-0.2.0/zimo_web_screenshot.egg-info/SOURCES.txt
--rw-r--r--   0 zimoluo    (501) staff       (20)        1 2024-04-21 14:51:49.000000 zimo-web-screenshot-0.2.0/zimo_web_screenshot.egg-info/dependency_links.txt
--rw-r--r--   0 zimoluo    (501) staff       (20)       76 2024-04-21 14:51:49.000000 zimo-web-screenshot-0.2.0/zimo_web_screenshot.egg-info/entry_points.txt
--rw-r--r--   0 zimoluo    (501) staff       (20)        9 2024-04-21 14:51:49.000000 zimo-web-screenshot-0.2.0/zimo_web_screenshot.egg-info/requires.txt
--rw-r--r--   0 zimoluo    (501) staff       (20)       20 2024-04-21 14:51:49.000000 zimo-web-screenshot-0.2.0/zimo_web_screenshot.egg-info/top_level.txt
+drwxr-xr-x   0 zimoluo    (501) staff       (20)        0 2024-05-27 12:09:40.563285 zimo-web-screenshot-0.3.0/
+-rw-r--r--   0 zimoluo    (501) staff       (20)     1057 2024-04-15 05:14:35.000000 zimo-web-screenshot-0.3.0/LICENSE
+-rw-r--r--   0 zimoluo    (501) staff       (20)     2288 2024-05-27 12:09:40.563363 zimo-web-screenshot-0.3.0/PKG-INFO
+-rw-r--r--   0 zimoluo    (501) staff       (20)     1783 2024-05-27 12:04:00.000000 zimo-web-screenshot-0.3.0/README.md
+-rw-r--r--   0 zimoluo    (501) staff       (20)       79 2024-05-27 12:09:40.563553 zimo-web-screenshot-0.3.0/setup.cfg
+-rw-r--r--   0 zimoluo    (501) staff       (20)      888 2024-05-27 12:05:19.000000 zimo-web-screenshot-0.3.0/setup.py
+drwxr-xr-x   0 zimoluo    (501) staff       (20)        0 2024-05-27 12:09:40.562395 zimo-web-screenshot-0.3.0/zimo_web_screenshot/
+-rw-r--r--   0 zimoluo    (501) staff       (20)        0 2024-04-15 10:38:36.000000 zimo-web-screenshot-0.3.0/zimo_web_screenshot/__init__.py
+-rw-r--r--   0 zimoluo    (501) staff       (20)     3529 2024-05-27 12:01:47.000000 zimo-web-screenshot-0.3.0/zimo_web_screenshot/screenshot.py
+drwxr-xr-x   0 zimoluo    (501) staff       (20)        0 2024-05-27 12:09:40.563174 zimo-web-screenshot-0.3.0/zimo_web_screenshot.egg-info/
+-rw-r--r--   0 zimoluo    (501) staff       (20)     2288 2024-05-27 12:09:40.000000 zimo-web-screenshot-0.3.0/zimo_web_screenshot.egg-info/PKG-INFO
+-rw-r--r--   0 zimoluo    (501) staff       (20)      362 2024-05-27 12:09:40.000000 zimo-web-screenshot-0.3.0/zimo_web_screenshot.egg-info/SOURCES.txt
+-rw-r--r--   0 zimoluo    (501) staff       (20)        1 2024-05-27 12:09:40.000000 zimo-web-screenshot-0.3.0/zimo_web_screenshot.egg-info/dependency_links.txt
+-rw-r--r--   0 zimoluo    (501) staff       (20)       76 2024-05-27 12:09:40.000000 zimo-web-screenshot-0.3.0/zimo_web_screenshot.egg-info/entry_points.txt
+-rw-r--r--   0 zimoluo    (501) staff       (20)        9 2024-05-27 12:09:40.000000 zimo-web-screenshot-0.3.0/zimo_web_screenshot.egg-info/requires.txt
+-rw-r--r--   0 zimoluo    (501) staff       (20)       20 2024-05-27 12:09:40.000000 zimo-web-screenshot-0.3.0/zimo_web_screenshot.egg-info/top_level.txt
```

### Comparing `zimo-web-screenshot-0.2.0/LICENSE` & `zimo-web-screenshot-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zimo-web-screenshot-0.2.0/PKG-INFO` & `zimo-web-screenshot-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zimo-web-screenshot
-Version: 0.2.0
+Version: 0.3.0
 Summary: A simple CLI tool to take screenshots of Zimo Web pages with Selenium.
 Home-page: https://github.com/zimoluo/zimo-web-screenshot-tool
 Author: Zimo Luo
 Author-email: abgkings0920@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -44,13 +44,14 @@
 
 ```bash
 zimo-web-screenshot --width 1600 --height 900 --theme plainDark --pathname about --delay 0
 ```
 
 **Command Line Arguments**
 
-- `-w`, `--width`: Width of the browser window (default: `1600`)
-- `-H`, `--height`: Height of the browser window (default: `900`)
-- `-t`, `--theme`: Theme name to apply (default: `pixelland`)
-- `-p`, `--pathname`: Pathname of the URL (default: `blog`)
-- `-d`, `--delay`: Delay in seconds before taking the screenshot (default: `0`)
-- `-f`, `--filename`: Output filename without the `.png` suffix (default: `webpage_screenshot`)
+- `-w`, `--width`: Width of the browser window. (default: `1600`)
+- `-H`, `--height`: Height of the browser window. (default: `900`)
+- `-t`, `--theme`: Theme name to apply. (default: `pixelland`)
+- `-p`, `--pathname`: Pathname of the URL. (default: `blog`)
+- `-d`, `--delay`: Delay in seconds before taking the screenshot. (default: `0`)
+- `-f`, `--filename`: Output filename without the `.png` suffix. (default: `webpage_screenshot`)
+- `-c`, `--custom`: Path to custom theme JSON config data file. This argument overrides `-t`. (default: does not exist)
```

### Comparing `zimo-web-screenshot-0.2.0/README.md` & `zimo-web-screenshot-0.3.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -29,13 +29,14 @@
 
 ```bash
 zimo-web-screenshot --width 1600 --height 900 --theme plainDark --pathname about --delay 0
 ```
 
 **Command Line Arguments**
 
-- `-w`, `--width`: Width of the browser window (default: `1600`)
-- `-H`, `--height`: Height of the browser window (default: `900`)
-- `-t`, `--theme`: Theme name to apply (default: `pixelland`)
-- `-p`, `--pathname`: Pathname of the URL (default: `blog`)
-- `-d`, `--delay`: Delay in seconds before taking the screenshot (default: `0`)
-- `-f`, `--filename`: Output filename without the `.png` suffix (default: `webpage_screenshot`)
+- `-w`, `--width`: Width of the browser window. (default: `1600`)
+- `-H`, `--height`: Height of the browser window. (default: `900`)
+- `-t`, `--theme`: Theme name to apply. (default: `pixelland`)
+- `-p`, `--pathname`: Pathname of the URL. (default: `blog`)
+- `-d`, `--delay`: Delay in seconds before taking the screenshot. (default: `0`)
+- `-f`, `--filename`: Output filename without the `.png` suffix. (default: `webpage_screenshot`)
+- `-c`, `--custom`: Path to custom theme JSON config data file. This argument overrides `-t`. (default: does not exist)
```

### Comparing `zimo-web-screenshot-0.2.0/setup.py` & `zimo-web-screenshot-0.3.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='zimo-web-screenshot',
-    version='0.2.0',
+    version='0.3.0',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         'selenium',
     ],
     entry_points={
         'console_scripts': [
```

### Comparing `zimo-web-screenshot-0.2.0/zimo_web_screenshot/screenshot.py` & `zimo-web-screenshot-0.3.0/zimo_web_screenshot/screenshot.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,54 @@
 import argparse
+import json
 from selenium import webdriver
 from selenium.webdriver.chrome.options import Options
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.common.by import By
 import time
 
 
-def take_screenshot(width, height, theme_name, pathname, delay, filename):
+def set_local_storage(driver, data):
+    driver.execute_script(
+        f"localStorage.setItem('websiteSettings', '{json.dumps(data)}');")
+
+
+def take_screenshot(width, height, theme_name, pathname, delay, filename, custom_data=None):
     try:
         chrome_options = Options()
         chrome_options.add_argument(f"--window-size={width},{height}")
         chrome_options.add_argument("--headless")
         chrome_options.add_argument("--hide-scrollbars")
 
         driver = webdriver.Chrome(options=chrome_options)
         driver.get(f"https://www.zimoluo.me/{pathname}")
 
         WebDriverWait(driver, 10).until(
-            EC.element_to_be_clickable((By.ID, "menu-button"))).click()
+            EC.presence_of_element_located((By.TAG_NAME, "body")))
 
-        time.sleep(0.4)
+        # Prepare websiteSettings data
+        if custom_data:
+            settings_data = {
+                "pageTheme": {x: "custom" for x in ["home", "blog", "photos", "projects", "about", "design", "management", "themeMaker"]},
+                "customThemeIndex": 0,
+                "customThemeData": [custom_data]
+            }
+        else:
+            settings_data = {
+                "pageTheme": {x: theme_name for x in ["home", "blog", "photos", "projects", "about", "design", "management", "themeMaker"]}
+            }
 
-        button_xpath = f"//button[.//img[@alt='Use {theme_name} theme']]"
-        WebDriverWait(driver, 10).until(
-            EC.element_to_be_clickable((By.XPATH, button_xpath))).click()
-        time.sleep(0.4)
+        set_local_storage(driver, settings_data)
 
-        WebDriverWait(driver, 10).until(
-            EC.element_to_be_clickable((By.ID, "menu-button"))).click()
+        driver.refresh()
 
-        time.sleep(1)
+        time.sleep(2)  # Wait for page to load
 
-        time.sleep(delay)
+        time.sleep(delay)  # Optional delay before taking the screenshot
 
         driver.save_screenshot(f'{filename}.png')
     except KeyboardInterrupt:
         print("Screenshot taking was aborted by the user.")
     except Exception as e:
         print(f"An error occurred: {e}")
     finally:
@@ -54,20 +66,27 @@
                         default="pixelland", help='Theme name to apply')
     parser.add_argument('-p', '--pathname', type=str,
                         default="design", help='Path within Zimo Web')
     parser.add_argument('-d', '--delay', type=float,
                         default=0, help='Delay before taking the screenshot')
     parser.add_argument('-f', '--filename', type=str,
                         default='webpage_screenshot', help='Output filename without suffix')
+    parser.add_argument('-c', '--custom', type=str,
+                        help='Path to custom theme JSON config data')
 
     args = parser.parse_args()
 
     try:
+        custom_data = None
+        if args.custom:
+            with open(args.custom, 'r') as file:
+                custom_data = json.load(file)
+
         take_screenshot(args.width, args.height, args.theme,
-                        args.pathname, args.delay, args.filename)
+                        args.pathname, args.delay, args.filename, custom_data)
     except Exception as e:
         print(f"Failed to take screenshot: {e}")
 
 
 if __name__ == "__main__":
     try:
         main()
```

### Comparing `zimo-web-screenshot-0.2.0/zimo_web_screenshot.egg-info/PKG-INFO` & `zimo-web-screenshot-0.3.0/zimo_web_screenshot.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zimo-web-screenshot
-Version: 0.2.0
+Version: 0.3.0
 Summary: A simple CLI tool to take screenshots of Zimo Web pages with Selenium.
 Home-page: https://github.com/zimoluo/zimo-web-screenshot-tool
 Author: Zimo Luo
 Author-email: abgkings0920@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -44,13 +44,14 @@
 
 ```bash
 zimo-web-screenshot --width 1600 --height 900 --theme plainDark --pathname about --delay 0
 ```
 
 **Command Line Arguments**
 
-- `-w`, `--width`: Width of the browser window (default: `1600`)
-- `-H`, `--height`: Height of the browser window (default: `900`)
-- `-t`, `--theme`: Theme name to apply (default: `pixelland`)
-- `-p`, `--pathname`: Pathname of the URL (default: `blog`)
-- `-d`, `--delay`: Delay in seconds before taking the screenshot (default: `0`)
-- `-f`, `--filename`: Output filename without the `.png` suffix (default: `webpage_screenshot`)
+- `-w`, `--width`: Width of the browser window. (default: `1600`)
+- `-H`, `--height`: Height of the browser window. (default: `900`)
+- `-t`, `--theme`: Theme name to apply. (default: `pixelland`)
+- `-p`, `--pathname`: Pathname of the URL. (default: `blog`)
+- `-d`, `--delay`: Delay in seconds before taking the screenshot. (default: `0`)
+- `-f`, `--filename`: Output filename without the `.png` suffix. (default: `webpage_screenshot`)
+- `-c`, `--custom`: Path to custom theme JSON config data file. This argument overrides `-t`. (default: does not exist)
```

