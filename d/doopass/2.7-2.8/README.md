# Comparing `tmp/doopass-2.7.tar.gz` & `tmp/doopass-2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doopass-2.7.tar", max compression
+gzip compressed data, was "doopass-2.8.tar", max compression
```

## Comparing `doopass-2.7.tar` & `doopass-2.8.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0    35150 2023-02-27 08:33:02.000000 doopass-2.7/LICENSE
--rw-r--r--   0        0        0     3817 2023-02-27 08:33:02.000000 doopass-2.7/README.md
--rw-r--r--   0        0        0     7665 2024-05-25 19:54:47.010823 doopass-2.7/assets/styles.css
--rw-r--r--   0        0        0        0 2023-02-27 08:33:02.000000 doopass-2.7/doopass/__init__.py
--rw-r--r--   0        0        0        0 2024-05-25 11:09:56.842325 doopass-2.7/doopass/core/__init__.py
--rw-r--r--   0        0        0      835 2024-05-27 00:25:57.942044 doopass-2.7/doopass/core/app.py
--rw-r--r--   0        0        0     2557 2024-05-25 17:49:17.589450 doopass-2.7/doopass/core/components/backup_manage_menu.py
--rw-r--r--   0        0        0      854 2024-05-25 17:49:17.598450 doopass-2.7/doopass/core/components/login_page.py
--rw-r--r--   0        0        0     2394 2024-05-25 11:09:56.843325 doopass-2.7/doopass/core/components/login_page_container.py
--rw-r--r--   0        0        0      680 2024-05-25 17:49:17.563451 doopass-2.7/doopass/core/components/message.py
--rw-r--r--   0        0        0     2681 2024-05-25 20:22:08.349197 doopass-2.7/doopass/core/components/pair_handle_page.py
--rw-r--r--   0        0        0     1963 2024-05-25 17:40:20.475409 doopass-2.7/doopass/core/components/select_menu.py
--rw-r--r--   0        0        0     1393 2024-05-25 20:09:25.927919 doopass-2.7/doopass/core/components/settings_handle_page.py
--rw-r--r--   0        0        0     1378 2024-05-26 16:46:58.293219 doopass-2.7/doopass/core/components/settings_pairs_list.py
--rw-r--r--   0        0        0      784 2024-05-25 17:49:17.624450 doopass-2.7/doopass/core/components/signup_page.py
--rw-r--r--   0        0        0     2415 2024-05-26 21:28:43.749946 doopass-2.7/doopass/core/components/store_handle_menu.py
--rw-r--r--   0        0        0     1253 2024-05-27 00:00:42.903759 doopass-2.7/doopass/core/components/store_handle_menu_item.py
--rw-r--r--   0        0        0      303 2024-05-25 17:49:17.577451 doopass-2.7/doopass/core/exceptions.py
--rw-r--r--   0        0        0      331 2024-05-25 17:31:21.256762 doopass-2.7/doopass/core/logo.py
--rw-r--r--   0        0        0     1275 2024-05-25 11:09:56.843325 doopass-2.7/doopass/core/password_validation.py
--rw-r--r--   0        0        0        0 2024-05-25 11:09:56.843325 doopass-2.7/doopass/core/screens/__init__.py
--rw-r--r--   0        0        0     2282 2024-05-25 17:49:17.586450 doopass-2.7/doopass/core/screens/backup_manage_screen.py
--rw-r--r--   0        0        0     5652 2024-05-25 17:49:17.580451 doopass-2.7/doopass/core/screens/help_screen.py
--rw-r--r--   0        0        0      587 2024-05-25 17:49:17.574451 doopass-2.7/doopass/core/screens/login_screen.py
--rw-r--r--   0        0        0     1962 2024-05-25 18:53:11.844134 doopass-2.7/doopass/core/screens/main_menu_screen.py
--rw-r--r--   0        0        0     3068 2024-05-25 17:49:17.616450 doopass-2.7/doopass/core/screens/main_screen.py
--rw-r--r--   0        0        0      861 2024-05-25 17:49:17.608450 doopass-2.7/doopass/core/screens/message_screen.py
--rw-r--r--   0        0        0      873 2024-05-25 17:49:17.611450 doopass-2.7/doopass/core/screens/screen.py
--rw-r--r--   0        0        0     1732 2024-05-26 17:27:08.207030 doopass-2.7/doopass/core/screens/settings_pair_handle_screen.py
--rw-r--r--   0        0        0     2236 2024-05-26 19:44:28.010076 doopass-2.7/doopass/core/screens/settings_screen.py
--rw-r--r--   0        0        0     1527 2024-05-25 17:49:17.614450 doopass-2.7/doopass/core/screens/sign_up_screen.py
--rw-r--r--   0        0        0     5904 2024-05-27 01:04:25.087593 doopass-2.7/doopass/core/screens/store_handle_screen.py
--rw-r--r--   0        0        0     1808 2024-05-26 16:48:37.609060 doopass-2.7/doopass/core/screens/store_pair_handle_screen.py
--rw-r--r--   0        0        0     4081 2024-05-26 20:32:31.008750 doopass-2.7/doopass/core/settings.py
--rw-r--r--   0        0        0     8851 2024-05-26 17:24:24.417995 doopass-2.7/doopass/core/store.py
--rw-r--r--   0        0        0     4265 2024-05-26 17:25:39.999108 doopass-2.7/doopass/core/store_backup.py
--rw-r--r--   0        0        0     1615 2024-05-26 21:27:19.654940 doopass-2.7/doopass/doopass.py
--rw-r--r--   0        0        0        0 2024-05-26 15:44:40.687288 doopass-2.7/doopass/tests/__init__.py
--rw-r--r--   0        0        0     2027 2024-05-26 16:01:07.863590 doopass-2.7/doopass/tests/settings_test.py
--rw-r--r--   0        0        0     1621 2024-05-27 01:09:09.816475 doopass-2.7/pyproject.toml
--rw-r--r--   0        0        0     5989 1970-01-01 00:00:00.000000 doopass-2.7/PKG-INFO
+-rw-r--r--   0        0        0    35150 2023-02-27 08:33:02.000000 doopass-2.8/LICENSE
+-rw-r--r--   0        0        0     3817 2023-02-27 08:33:02.000000 doopass-2.8/README.md
+-rw-r--r--   0        0        0     7665 2024-05-25 19:54:47.010823 doopass-2.8/assets/styles.css
+-rw-r--r--   0        0        0        0 2023-02-27 08:33:02.000000 doopass-2.8/doopass/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-25 11:09:56.842325 doopass-2.8/doopass/core/__init__.py
+-rw-r--r--   0        0        0      835 2024-05-27 00:25:57.942044 doopass-2.8/doopass/core/app.py
+-rw-r--r--   0        0        0     2557 2024-05-25 17:49:17.589450 doopass-2.8/doopass/core/components/backup_manage_menu.py
+-rw-r--r--   0        0        0      854 2024-05-25 17:49:17.598450 doopass-2.8/doopass/core/components/login_page.py
+-rw-r--r--   0        0        0     2394 2024-05-25 11:09:56.843325 doopass-2.8/doopass/core/components/login_page_container.py
+-rw-r--r--   0        0        0      680 2024-05-25 17:49:17.563451 doopass-2.8/doopass/core/components/message.py
+-rw-r--r--   0        0        0     2681 2024-05-25 20:22:08.349197 doopass-2.8/doopass/core/components/pair_handle_page.py
+-rw-r--r--   0        0        0     1963 2024-05-25 17:40:20.475409 doopass-2.8/doopass/core/components/select_menu.py
+-rw-r--r--   0        0        0     1393 2024-05-25 20:09:25.927919 doopass-2.8/doopass/core/components/settings_handle_page.py
+-rw-r--r--   0        0        0     1378 2024-05-26 16:46:58.293219 doopass-2.8/doopass/core/components/settings_pairs_list.py
+-rw-r--r--   0        0        0      784 2024-05-25 17:49:17.624450 doopass-2.8/doopass/core/components/signup_page.py
+-rw-r--r--   0        0        0     2415 2024-05-26 21:28:43.749946 doopass-2.8/doopass/core/components/store_handle_menu.py
+-rw-r--r--   0        0        0     1253 2024-05-27 00:00:42.903759 doopass-2.8/doopass/core/components/store_handle_menu_item.py
+-rw-r--r--   0        0        0      303 2024-05-25 17:49:17.577451 doopass-2.8/doopass/core/exceptions.py
+-rw-r--r--   0        0        0      331 2024-05-25 17:31:21.256762 doopass-2.8/doopass/core/logo.py
+-rw-r--r--   0        0        0     1275 2024-05-25 11:09:56.843325 doopass-2.8/doopass/core/password_validation.py
+-rw-r--r--   0        0        0        0 2024-05-25 11:09:56.843325 doopass-2.8/doopass/core/screens/__init__.py
+-rw-r--r--   0        0        0     2282 2024-05-25 17:49:17.586450 doopass-2.8/doopass/core/screens/backup_manage_screen.py
+-rw-r--r--   0        0        0     5652 2024-05-25 17:49:17.580451 doopass-2.8/doopass/core/screens/help_screen.py
+-rw-r--r--   0        0        0      587 2024-05-25 17:49:17.574451 doopass-2.8/doopass/core/screens/login_screen.py
+-rw-r--r--   0        0        0     1962 2024-05-25 18:53:11.844134 doopass-2.8/doopass/core/screens/main_menu_screen.py
+-rw-r--r--   0        0        0     3068 2024-05-25 17:49:17.616450 doopass-2.8/doopass/core/screens/main_screen.py
+-rw-r--r--   0        0        0      861 2024-05-25 17:49:17.608450 doopass-2.8/doopass/core/screens/message_screen.py
+-rw-r--r--   0        0        0      873 2024-05-25 17:49:17.611450 doopass-2.8/doopass/core/screens/screen.py
+-rw-r--r--   0        0        0     1732 2024-05-26 17:27:08.207030 doopass-2.8/doopass/core/screens/settings_pair_handle_screen.py
+-rw-r--r--   0        0        0     2236 2024-05-26 19:44:28.010076 doopass-2.8/doopass/core/screens/settings_screen.py
+-rw-r--r--   0        0        0     1527 2024-05-25 17:49:17.614450 doopass-2.8/doopass/core/screens/sign_up_screen.py
+-rw-r--r--   0        0        0     5904 2024-05-27 01:04:25.087593 doopass-2.8/doopass/core/screens/store_handle_screen.py
+-rw-r--r--   0        0        0     1808 2024-05-26 16:48:37.609060 doopass-2.8/doopass/core/screens/store_pair_handle_screen.py
+-rw-r--r--   0        0        0     4081 2024-05-26 20:32:31.008750 doopass-2.8/doopass/core/settings.py
+-rw-r--r--   0        0        0     8851 2024-05-26 17:24:24.417995 doopass-2.8/doopass/core/store.py
+-rw-r--r--   0        0        0     4265 2024-05-26 17:25:39.999108 doopass-2.8/doopass/core/store_backup.py
+-rw-r--r--   0        0        0     1615 2024-05-26 21:27:19.654940 doopass-2.8/doopass/doopass.py
+-rw-r--r--   0        0        0        0 2024-05-26 15:44:40.687288 doopass-2.8/doopass/tests/__init__.py
+-rw-r--r--   0        0        0     2027 2024-05-26 16:01:07.863590 doopass-2.8/doopass/tests/settings_test.py
+-rw-r--r--   0        0        0     1739 2024-05-27 01:12:06.177544 doopass-2.8/pyproject.toml
+-rw-r--r--   0        0        0     5989 1970-01-01 00:00:00.000000 doopass-2.8/PKG-INFO
```

### Comparing `doopass-2.7/LICENSE` & `doopass-2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `doopass-2.7/README.md` & `doopass-2.8/README.md`

 * *Files identical despite different names*

### Comparing `doopass-2.7/assets/styles.css` & `doopass-2.8/assets/styles.css`

 * *Files identical despite different names*

### Comparing `doopass-2.7/doopass/core/app.py` & `doopass-2.8/doopass/core/app.py`

 * *Files identical despite different names*

### Comparing `doopass-2.7/doopass/core/components/backup_manage_menu.py` & `doopass-2.8/doopass/core/components/backup_manage_menu.py`

 * *Files identical despite different names*

### Comparing `doopass-2.7/doopass/core/components/login_page.py` & `doopass-2.8/doopass/core/components/login_page.py`

 * *Files identical despite different names*

### Comparing `doopass-2.7/doopass/core/components/login_page_container.py` & `doopass-2.8/doopass/core/components/login_page_container.py`

 * *Files identical despite different names*

### Comparing `doopass-2.7/doopass/core/components/message.py` & `doopass-2.8/doopass/core/components/message.py`

 * *Files identical despite different names*

### Comparing `doopass-2.7/doopass/core/components/pair_handle_page.py` & `doopass-2.8/doopass/core/components/pair_handle_page.py`

 * *Files identical despite different names*

### Comparing `doopass-2.7/doopass/core/components/select_menu.py` & `doopass-2.8/doopass/core/components/select_menu.py`

 * *Files identical despite different names*

### Comparing `doopass-2.7/doopass/core/components/settings_handle_page.py` & `doopass-2.8/doopass/core/components/settings_handle_page.py`

 * *Files identical despite different names*

### Comparing `doopass-2.7/doopass/core/components/settings_pairs_list.py` & `doopass-2.8/doopass/core/components/settings_pairs_list.py`

 * *Files identical despite different names*

### Comparing `doopass-2.7/doopass/core/components/signup_page.py` & `doopass-2.8/doopass/core/components/signup_page.py`

 * *Files identical despite different names*

### Comparing `doopass-2.7/doopass/core/components/store_handle_menu.py` & `doopass-2.8/doopass/core/components/store_handle_menu.py`

 * *Files identical despite different names*

### Comparing `doopass-2.7/doopass/core/components/store_handle_menu_item.py` & `doopass-2.8/doopass/core/components/store_handle_menu_item.py`

 * *Files identical despite different names*

### Comparing `doopass-2.7/doopass/core/password_validation.py` & `doopass-2.8/doopass/core/password_validation.py`

 * *Files identical despite different names*

### Comparing `doopass-2.7/doopass/core/screens/backup_manage_screen.py` & `doopass-2.8/doopass/core/screens/backup_manage_screen.py`

 * *Files identical despite different names*

### Comparing `doopass-2.7/doopass/core/screens/help_screen.py` & `doopass-2.8/doopass/core/screens/help_screen.py`

 * *Files identical despite different names*

### Comparing `doopass-2.7/doopass/core/screens/login_screen.py` & `doopass-2.8/doopass/core/screens/login_screen.py`

 * *Files identical despite different names*

### Comparing `doopass-2.7/doopass/core/screens/main_menu_screen.py` & `doopass-2.8/doopass/core/screens/main_menu_screen.py`

 * *Files identical despite different names*

### Comparing `doopass-2.7/doopass/core/screens/main_screen.py` & `doopass-2.8/doopass/core/screens/main_screen.py`

 * *Files identical despite different names*

### Comparing `doopass-2.7/doopass/core/screens/message_screen.py` & `doopass-2.8/doopass/core/screens/message_screen.py`

 * *Files identical despite different names*

### Comparing `doopass-2.7/doopass/core/screens/screen.py` & `doopass-2.8/doopass/core/screens/screen.py`

 * *Files identical despite different names*

### Comparing `doopass-2.7/doopass/core/screens/settings_pair_handle_screen.py` & `doopass-2.8/doopass/core/screens/settings_pair_handle_screen.py`

 * *Files identical despite different names*

### Comparing `doopass-2.7/doopass/core/screens/settings_screen.py` & `doopass-2.8/doopass/core/screens/settings_screen.py`

 * *Files identical despite different names*

### Comparing `doopass-2.7/doopass/core/screens/sign_up_screen.py` & `doopass-2.8/doopass/core/screens/sign_up_screen.py`

 * *Files identical despite different names*

### Comparing `doopass-2.7/doopass/core/screens/store_handle_screen.py` & `doopass-2.8/doopass/core/screens/store_handle_screen.py`

 * *Files identical despite different names*

### Comparing `doopass-2.7/doopass/core/screens/store_pair_handle_screen.py` & `doopass-2.8/doopass/core/screens/store_pair_handle_screen.py`

 * *Files identical despite different names*

### Comparing `doopass-2.7/doopass/core/settings.py` & `doopass-2.8/doopass/core/settings.py`

 * *Files identical despite different names*

### Comparing `doopass-2.7/doopass/core/store.py` & `doopass-2.8/doopass/core/store.py`

 * *Files identical despite different names*

### Comparing `doopass-2.7/doopass/core/store_backup.py` & `doopass-2.8/doopass/core/store_backup.py`

 * *Files identical despite different names*

### Comparing `doopass-2.7/doopass/doopass.py` & `doopass-2.8/doopass/doopass.py`

 * *Files identical despite different names*

### Comparing `doopass-2.7/doopass/tests/settings_test.py` & `doopass-2.8/doopass/tests/settings_test.py`

 * *Files identical despite different names*

### Comparing `doopass-2.7/pyproject.toml` & `doopass-2.8/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 [tool.poetry]
 name = "doopass"
-version = "2.7"
+version = "2.8"
 description = 'Crossplatform TUI password manager written in python'
 authors = ["Michael Nikishov <doopath@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/doopath/PasswordManager"
 packages = [
     {include = "doopass"},
+    {include = "doopass/core"},
+    {include = "doopass/core/components"},
+    {include = "doopass/core/screens"},
     {include = "assets/styles.css"}
 ]
 
 [tool.poetry.scripts]
 doopass = 'doopass.doopass:main'
 
 [tool.poetry.dependencies]
```

### Comparing `doopass-2.7/PKG-INFO` & `doopass-2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doopass
-Version: 2.7
+Version: 2.8
 Summary: Crossplatform TUI password manager written in python
 Home-page: https://github.com/doopath/PasswordManager
 Author: Michael Nikishov
 Author-email: doopath@gmail.com
 Requires-Python: >=3.12.0,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: doopass Version: 2.7 Summary: Crossplatform TUI
+Metadata-Version: 2.1 Name: doopass Version: 2.8 Summary: Crossplatform TUI
 password manager written in python Home-page: https://github.com/doopath/
 PasswordManager Author: Michael Nikishov Author-email: doopath@gmail.com
 Requires-Python: >=3.12.0,<4.0.0 Classifier: Programming Language :: Python ::
 3 Classifier: Programming Language :: Python :: 3.12 Requires-Dist:
 CacheControl (==0.14.0) Requires-Dist: Pygments (==2.18.0) Requires-Dist:
 SecretStorage (==3.3.3) Requires-Dist: build (==1.2.1) Requires-Dist: certifi
 (==2024.2.2) Requires-Dist: cffi (==1.16.0) Requires-Dist: charset-normalizer
```

