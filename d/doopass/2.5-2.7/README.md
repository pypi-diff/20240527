# Comparing `tmp/doopass-2.5.tar.gz` & `tmp/doopass-2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doopass-2.5.tar", last modified: Sat May 25 10:55:17 2024, max compression
+gzip compressed data, was "doopass-2.7.tar", max compression
```

## Comparing `doopass-2.5.tar` & `doopass-2.7.tar`

### file list

```diff
@@ -1,24 +1,41 @@
-drwxr-xr-x   0 doopath   (1000) doopath   (1000)        0 2024-05-25 10:55:17.847251 doopass-2.5/
--rw-r--r--   0 doopath   (1000) doopath   (1000)      134 2023-02-27 08:33:02.000000 doopass-2.5/.gitignore
--rw-r--r--   0 doopath   (1000) doopath   (1000)    35150 2023-02-27 08:33:02.000000 doopass-2.5/LICENSE
--rw-r--r--   0 doopath   (1000) doopath   (1000)     5467 2024-05-25 10:55:17.846251 doopass-2.5/PKG-INFO
--rw-r--r--   0 doopath   (1000) doopath   (1000)     3817 2023-02-27 08:33:02.000000 doopass-2.5/README.md
-drwxr-xr-x   0 doopath   (1000) doopath   (1000)        0 2024-05-25 10:55:17.843251 doopass-2.5/assets/
--rw-r--r--   0 doopath   (1000) doopath   (1000)    15600 2023-02-27 08:33:02.000000 doopass-2.5/assets/preview.png
--rw-r--r--   0 doopath   (1000) doopath   (1000)     6691 2023-02-27 08:33:02.000000 doopass-2.5/assets/styles.css
--rw-r--r--   0 doopath   (1000) doopath   (1000)      362 2024-05-25 10:44:01.000000 doopass-2.5/dependencies.txt
--rw-r--r--   0 doopath   (1000) doopath   (1000)      330 2024-02-01 20:39:36.000000 doopass-2.5/deversion.py
-drwxr-xr-x   0 doopath   (1000) doopath   (1000)        0 2024-05-25 10:55:17.844251 doopass-2.5/doopass/
--rw-r--r--   0 doopath   (1000) doopath   (1000)        0 2023-02-27 08:33:02.000000 doopass-2.5/doopass/__init__.py
--rw-r--r--   0 doopath   (1000) doopath   (1000)     1012 2024-05-25 10:52:29.000000 doopass-2.5/doopass/app.py
--rw-r--r--   0 doopath   (1000) doopath   (1000)     1380 2024-05-25 10:52:29.000000 doopass-2.5/doopass/doopass.py
-drwxr-xr-x   0 doopath   (1000) doopath   (1000)        0 2024-05-25 10:55:17.845251 doopass-2.5/doopass.egg-info/
--rw-r--r--   0 doopath   (1000) doopath   (1000)     5467 2024-05-25 10:55:17.000000 doopass-2.5/doopass.egg-info/PKG-INFO
--rw-r--r--   0 doopath   (1000) doopath   (1000)      367 2024-05-25 10:55:17.000000 doopass-2.5/doopass.egg-info/SOURCES.txt
--rw-r--r--   0 doopath   (1000) doopath   (1000)        1 2024-05-25 10:55:17.000000 doopass-2.5/doopass.egg-info/dependency_links.txt
--rw-r--r--   0 doopath   (1000) doopath   (1000)       49 2024-05-25 10:55:17.000000 doopass-2.5/doopass.egg-info/entry_points.txt
--rw-r--r--   0 doopath   (1000) doopath   (1000)      628 2024-05-25 10:55:17.000000 doopass-2.5/doopass.egg-info/requires.txt
--rw-r--r--   0 doopath   (1000) doopath   (1000)       15 2024-05-25 10:55:17.000000 doopass-2.5/doopass.egg-info/top_level.txt
--rw-r--r--   0 doopath   (1000) doopath   (1000)      551 2023-02-27 08:33:02.000000 doopass-2.5/installing.txt
--rw-r--r--   0 doopath   (1000) doopath   (1000)     1731 2024-05-25 10:55:02.000000 doopass-2.5/pyproject.toml
--rw-r--r--   0 doopath   (1000) doopath   (1000)       38 2024-05-25 10:55:17.847251 doopass-2.5/setup.cfg
+-rw-r--r--   0        0        0    35150 2023-02-27 08:33:02.000000 doopass-2.7/LICENSE
+-rw-r--r--   0        0        0     3817 2023-02-27 08:33:02.000000 doopass-2.7/README.md
+-rw-r--r--   0        0        0     7665 2024-05-25 19:54:47.010823 doopass-2.7/assets/styles.css
+-rw-r--r--   0        0        0        0 2023-02-27 08:33:02.000000 doopass-2.7/doopass/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-25 11:09:56.842325 doopass-2.7/doopass/core/__init__.py
+-rw-r--r--   0        0        0      835 2024-05-27 00:25:57.942044 doopass-2.7/doopass/core/app.py
+-rw-r--r--   0        0        0     2557 2024-05-25 17:49:17.589450 doopass-2.7/doopass/core/components/backup_manage_menu.py
+-rw-r--r--   0        0        0      854 2024-05-25 17:49:17.598450 doopass-2.7/doopass/core/components/login_page.py
+-rw-r--r--   0        0        0     2394 2024-05-25 11:09:56.843325 doopass-2.7/doopass/core/components/login_page_container.py
+-rw-r--r--   0        0        0      680 2024-05-25 17:49:17.563451 doopass-2.7/doopass/core/components/message.py
+-rw-r--r--   0        0        0     2681 2024-05-25 20:22:08.349197 doopass-2.7/doopass/core/components/pair_handle_page.py
+-rw-r--r--   0        0        0     1963 2024-05-25 17:40:20.475409 doopass-2.7/doopass/core/components/select_menu.py
+-rw-r--r--   0        0        0     1393 2024-05-25 20:09:25.927919 doopass-2.7/doopass/core/components/settings_handle_page.py
+-rw-r--r--   0        0        0     1378 2024-05-26 16:46:58.293219 doopass-2.7/doopass/core/components/settings_pairs_list.py
+-rw-r--r--   0        0        0      784 2024-05-25 17:49:17.624450 doopass-2.7/doopass/core/components/signup_page.py
+-rw-r--r--   0        0        0     2415 2024-05-26 21:28:43.749946 doopass-2.7/doopass/core/components/store_handle_menu.py
+-rw-r--r--   0        0        0     1253 2024-05-27 00:00:42.903759 doopass-2.7/doopass/core/components/store_handle_menu_item.py
+-rw-r--r--   0        0        0      303 2024-05-25 17:49:17.577451 doopass-2.7/doopass/core/exceptions.py
+-rw-r--r--   0        0        0      331 2024-05-25 17:31:21.256762 doopass-2.7/doopass/core/logo.py
+-rw-r--r--   0        0        0     1275 2024-05-25 11:09:56.843325 doopass-2.7/doopass/core/password_validation.py
+-rw-r--r--   0        0        0        0 2024-05-25 11:09:56.843325 doopass-2.7/doopass/core/screens/__init__.py
+-rw-r--r--   0        0        0     2282 2024-05-25 17:49:17.586450 doopass-2.7/doopass/core/screens/backup_manage_screen.py
+-rw-r--r--   0        0        0     5652 2024-05-25 17:49:17.580451 doopass-2.7/doopass/core/screens/help_screen.py
+-rw-r--r--   0        0        0      587 2024-05-25 17:49:17.574451 doopass-2.7/doopass/core/screens/login_screen.py
+-rw-r--r--   0        0        0     1962 2024-05-25 18:53:11.844134 doopass-2.7/doopass/core/screens/main_menu_screen.py
+-rw-r--r--   0        0        0     3068 2024-05-25 17:49:17.616450 doopass-2.7/doopass/core/screens/main_screen.py
+-rw-r--r--   0        0        0      861 2024-05-25 17:49:17.608450 doopass-2.7/doopass/core/screens/message_screen.py
+-rw-r--r--   0        0        0      873 2024-05-25 17:49:17.611450 doopass-2.7/doopass/core/screens/screen.py
+-rw-r--r--   0        0        0     1732 2024-05-26 17:27:08.207030 doopass-2.7/doopass/core/screens/settings_pair_handle_screen.py
+-rw-r--r--   0        0        0     2236 2024-05-26 19:44:28.010076 doopass-2.7/doopass/core/screens/settings_screen.py
+-rw-r--r--   0        0        0     1527 2024-05-25 17:49:17.614450 doopass-2.7/doopass/core/screens/sign_up_screen.py
+-rw-r--r--   0        0        0     5904 2024-05-27 01:04:25.087593 doopass-2.7/doopass/core/screens/store_handle_screen.py
+-rw-r--r--   0        0        0     1808 2024-05-26 16:48:37.609060 doopass-2.7/doopass/core/screens/store_pair_handle_screen.py
+-rw-r--r--   0        0        0     4081 2024-05-26 20:32:31.008750 doopass-2.7/doopass/core/settings.py
+-rw-r--r--   0        0        0     8851 2024-05-26 17:24:24.417995 doopass-2.7/doopass/core/store.py
+-rw-r--r--   0        0        0     4265 2024-05-26 17:25:39.999108 doopass-2.7/doopass/core/store_backup.py
+-rw-r--r--   0        0        0     1615 2024-05-26 21:27:19.654940 doopass-2.7/doopass/doopass.py
+-rw-r--r--   0        0        0        0 2024-05-26 15:44:40.687288 doopass-2.7/doopass/tests/__init__.py
+-rw-r--r--   0        0        0     2027 2024-05-26 16:01:07.863590 doopass-2.7/doopass/tests/settings_test.py
+-rw-r--r--   0        0        0     1621 2024-05-27 01:09:09.816475 doopass-2.7/pyproject.toml
+-rw-r--r--   0        0        0     5989 1970-01-01 00:00:00.000000 doopass-2.7/PKG-INFO
```

### Comparing `doopass-2.5/LICENSE` & `doopass-2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `doopass-2.5/PKG-INFO` & `doopass-2.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,55 +1,67 @@
 Metadata-Version: 2.1
 Name: doopass
-Version: 2.5
+Version: 2.7
 Summary: Crossplatform TUI password manager written in python
-Author-email: Michael Nikishov <doopath@gmail.com>
-Project-URL: Homepage, https://github.com/doopath/PasswordManager
+Home-page: https://github.com/doopath/PasswordManager
+Author: Michael Nikishov
+Author-email: doopath@gmail.com
+Requires-Python: >=3.12.0,<4.0.0
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License (GPL)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: CacheControl (==0.14.0)
+Requires-Dist: Pygments (==2.18.0)
+Requires-Dist: SecretStorage (==3.3.3)
+Requires-Dist: build (==1.2.1)
+Requires-Dist: certifi (==2024.2.2)
+Requires-Dist: cffi (==1.16.0)
+Requires-Dist: charset-normalizer (==3.3.2)
+Requires-Dist: cleo (==2.1.0)
+Requires-Dist: crashtest (==0.4.1)
+Requires-Dist: cryptography (==42.0.7)
+Requires-Dist: distlib (==0.3.8)
+Requires-Dist: dulwich (==0.21.7)
+Requires-Dist: fastjsonschema (==2.19.1)
+Requires-Dist: filelock (==3.14.0)
+Requires-Dist: idna (==3.7)
+Requires-Dist: installer (==0.7.0)
+Requires-Dist: jaraco_classes (==3.4.0)
+Requires-Dist: jeepney (==0.8.0)
+Requires-Dist: keyring (==24.3.1)
+Requires-Dist: linkify-it-py (==2.0.3)
+Requires-Dist: markdown-it-py (==3.0.0)
+Requires-Dist: mdit-py-plugins (==0.4.1)
+Requires-Dist: mdurl (==0.1.2)
+Requires-Dist: more-itertools (==10.2.0)
+Requires-Dist: msgpack (==1.0.8)
+Requires-Dist: packaging (==24.0)
+Requires-Dist: pexpect (==4.9.0)
+Requires-Dist: pkginfo (==1.10.0)
+Requires-Dist: platformdirs (==4.2.2)
+Requires-Dist: poetry (==1.8.3)
+Requires-Dist: poetry-core (==1.9.0)
+Requires-Dist: poetry-plugin-export (==1.8.0)
+Requires-Dist: ptyprocess (==0.7.0)
+Requires-Dist: pycparser (==2.22)
+Requires-Dist: pyperclip (==1.8.2)
+Requires-Dist: pyproject_hooks (==1.1.0)
+Requires-Dist: rapidfuzz (==3.9.1)
+Requires-Dist: requests (==2.32.2)
+Requires-Dist: requests-toolbelt (==1.0.0)
+Requires-Dist: rich (==13.7.1)
+Requires-Dist: shellingham (==1.5.4)
+Requires-Dist: textual (==0.63.4)
+Requires-Dist: tomlkit (==0.12.5)
+Requires-Dist: trove-classifiers (==2024.5.22)
+Requires-Dist: twine (==5.1.0)
+Requires-Dist: typing_extensions (==4.12.0)
+Requires-Dist: uc-micro-py (==1.0.3)
+Requires-Dist: urllib3 (==2.2.1)
+Requires-Dist: virtualenv (==20.26.2)
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: bleach==6.0.0
-Requires-Dist: build==0.10.0
-Requires-Dist: certifi==2022.12.7
-Requires-Dist: cffi==1.15.1
-Requires-Dist: charset-normalizer==3.0.1
-Requires-Dist: click==8.1.3
-Requires-Dist: colorama==0.4.6
-Requires-Dist: cryptography==39.0.1
-Requires-Dist: docutils==0.19
-Requires-Dist: idna==3.4
-Requires-Dist: importlib-metadata==4.13.0
-Requires-Dist: jaraco.classes==3.2.3
-Requires-Dist: keyring==23.13.1
-Requires-Dist: markdown-it-py==2.1.0
-Requires-Dist: mdurl==0.1.2
-Requires-Dist: more-itertools==9.0.0
-Requires-Dist: nanoid==2.0.0
-Requires-Dist: packaging==23.0
-Requires-Dist: pkginfo==1.9.6
-Requires-Dist: pycparser==2.21
-Requires-Dist: Pygments==2.14.0
-Requires-Dist: pyperclip==1.8.2
-Requires-Dist: pyproject_hooks==1.0.0
-Requires-Dist: pywin32-ctypes==0.2.0
-Requires-Dist: readme-renderer==37.3
-Requires-Dist: requests==2.28.2
-Requires-Dist: requests-toolbelt==0.10.1
-Requires-Dist: rfc3986==2.0.0
-Requires-Dist: rich==13.3.1
-Requires-Dist: six==1.16.0
-Requires-Dist: textual==0.10.1
-Requires-Dist: twine==4.0.2
-Requires-Dist: urllib3==1.26.14
-Requires-Dist: webencodings==0.5.1
-Requires-Dist: zipp==3.13.0
-Requires-Dist: doopass-libs==1.0.7
 
 # PasswordManager
 
 ## Preview
 
 ![no image](https://raw.githubusercontent.com/doopath/PasswordManager/master/assets/preview.png)
 
@@ -137,7 +149,8 @@
 ## About
 
 Store format of the current version of **Doopass** is fully compatible with the older one ([_cli_](https://github.com/doopath/PasswordManager/tree/cli)). That means you can move the store.enc file from your cli version of the **Doopass** to the _~/doopass/appdata_ dir and you will able to use it.
 
 **Doopass** uses the _cryptography_ and _base64_ python libs for encrypting your data. It's safe to share your store.enc or backup of the store. You can upload your store.enc somewhere if it's necessary. If you have any ideas about making Doopass more safe please contact me or make a pull request.
 
 If you want to contribute you can make a pull request or create an issue. If you want to contact me you can write me on [Telegram](https://t.me/doopath) or Gmail: *doopath@gmail.com*.
+
```

#### html2text {}

```diff
@@ -1,32 +1,38 @@
-Metadata-Version: 2.1 Name: doopass Version: 2.5 Summary: Crossplatform TUI
-password manager written in python Author-email: Michael Nikishov
-gmail.com> Project-URL: Homepage, https://github.com/doopath/PasswordManager
-Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
-Approved :: GNU General Public License (GPL) Classifier: Operating System :: OS
-Independent Requires-Python: >=3.11 Description-Content-Type: text/markdown
-License-File: LICENSE Requires-Dist: bleach==6.0.0 Requires-Dist: build==0.10.0
-Requires-Dist: certifi==2022.12.7 Requires-Dist: cffi==1.15.1 Requires-Dist:
-charset-normalizer==3.0.1 Requires-Dist: click==8.1.3 Requires-Dist:
-colorama==0.4.6 Requires-Dist: cryptography==39.0.1 Requires-Dist:
-docutils==0.19 Requires-Dist: idna==3.4 Requires-Dist: importlib-
-metadata==4.13.0 Requires-Dist: jaraco.classes==3.2.3 Requires-Dist:
-keyring==23.13.1 Requires-Dist: markdown-it-py==2.1.0 Requires-Dist:
-mdurl==0.1.2 Requires-Dist: more-itertools==9.0.0 Requires-Dist: nanoid==2.0.0
-Requires-Dist: packaging==23.0 Requires-Dist: pkginfo==1.9.6 Requires-Dist:
-pycparser==2.21 Requires-Dist: Pygments==2.14.0 Requires-Dist: pyperclip==1.8.2
-Requires-Dist: pyproject_hooks==1.0.0 Requires-Dist: pywin32-ctypes==0.2.0
-Requires-Dist: readme-renderer==37.3 Requires-Dist: requests==2.28.2 Requires-
-Dist: requests-toolbelt==0.10.1 Requires-Dist: rfc3986==2.0.0 Requires-Dist:
-rich==13.3.1 Requires-Dist: six==1.16.0 Requires-Dist: textual==0.10.1
-Requires-Dist: twine==4.0.2 Requires-Dist: urllib3==1.26.14 Requires-Dist:
-webencodings==0.5.1 Requires-Dist: zipp==3.13.0 Requires-Dist: doopass-
-libs==1.0.7 # PasswordManager ## Preview ![no image](https://
-raw.githubusercontent.com/doopath/PasswordManager/master/assets/preview.png) ##
-Navigation
+Metadata-Version: 2.1 Name: doopass Version: 2.7 Summary: Crossplatform TUI
+password manager written in python Home-page: https://github.com/doopath/
+PasswordManager Author: Michael Nikishov Author-email: doopath@gmail.com
+Requires-Python: >=3.12.0,<4.0.0 Classifier: Programming Language :: Python ::
+3 Classifier: Programming Language :: Python :: 3.12 Requires-Dist:
+CacheControl (==0.14.0) Requires-Dist: Pygments (==2.18.0) Requires-Dist:
+SecretStorage (==3.3.3) Requires-Dist: build (==1.2.1) Requires-Dist: certifi
+(==2024.2.2) Requires-Dist: cffi (==1.16.0) Requires-Dist: charset-normalizer
+(==3.3.2) Requires-Dist: cleo (==2.1.0) Requires-Dist: crashtest (==0.4.1)
+Requires-Dist: cryptography (==42.0.7) Requires-Dist: distlib (==0.3.8)
+Requires-Dist: dulwich (==0.21.7) Requires-Dist: fastjsonschema (==2.19.1)
+Requires-Dist: filelock (==3.14.0) Requires-Dist: idna (==3.7) Requires-Dist:
+installer (==0.7.0) Requires-Dist: jaraco_classes (==3.4.0) Requires-Dist:
+jeepney (==0.8.0) Requires-Dist: keyring (==24.3.1) Requires-Dist: linkify-it-
+py (==2.0.3) Requires-Dist: markdown-it-py (==3.0.0) Requires-Dist: mdit-py-
+plugins (==0.4.1) Requires-Dist: mdurl (==0.1.2) Requires-Dist: more-itertools
+(==10.2.0) Requires-Dist: msgpack (==1.0.8) Requires-Dist: packaging (==24.0)
+Requires-Dist: pexpect (==4.9.0) Requires-Dist: pkginfo (==1.10.0) Requires-
+Dist: platformdirs (==4.2.2) Requires-Dist: poetry (==1.8.3) Requires-Dist:
+poetry-core (==1.9.0) Requires-Dist: poetry-plugin-export (==1.8.0) Requires-
+Dist: ptyprocess (==0.7.0) Requires-Dist: pycparser (==2.22) Requires-Dist:
+pyperclip (==1.8.2) Requires-Dist: pyproject_hooks (==1.1.0) Requires-Dist:
+rapidfuzz (==3.9.1) Requires-Dist: requests (==2.32.2) Requires-Dist: requests-
+toolbelt (==1.0.0) Requires-Dist: rich (==13.7.1) Requires-Dist: shellingham
+(==1.5.4) Requires-Dist: textual (==0.63.4) Requires-Dist: tomlkit (==0.12.5)
+Requires-Dist: trove-classifiers (==2024.5.22) Requires-Dist: twine (==5.1.0)
+Requires-Dist: typing_extensions (==4.12.0) Requires-Dist: uc-micro-py
+(==1.0.3) Requires-Dist: urllib3 (==2.2.1) Requires-Dist: virtualenv
+(==20.26.2) Description-Content-Type: text/markdown # PasswordManager ##
+Preview ![no image](https://raw.githubusercontent.com/doopath/PasswordManager/
+master/assets/preview.png) ## Navigation
     * _P_r_e_v_i_e_w
     * _N_a_v_i_g_a_t_i_o_n
     * _D_e_s_c_r_i_p_t_i_o_n
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _U_s_a_g_e
     * _A_b_o_u_t
 ## Description **Doopass** is a TUI password manager based on [_textual_]
```

### Comparing `doopass-2.5/README.md` & `doopass-2.7/README.md`

 * *Files identical despite different names*

### Comparing `doopass-2.5/assets/styles.css` & `doopass-2.7/assets/styles.css`

 * *Files 9% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     scrollbar-color-active: #ffffff;
 }
 
 .button {
     background: #e9ecef;
     color: #1b1b1b;
     border: none;
+    height: 5;
 }
 
 .button:focus {
     text-style: bold !important;
     color: #ffffff !important;
     background: #000000 !important;
     border: tall #e9ecef !important;
@@ -135,16 +136,16 @@
 .select_menu_logo_label {
     color: #e9ecef;
     text-align: left;
 }
 
 .select_menu_buttons_supercontainer {
     width: 100%;
-    height: 16;
-    grid-size: 3 1;
+    height: 20;
+    grid-size: 4 1;
     grid-columns: 1fr 3fr 1fr;
     align: center middle;
 }
 
 .select_menu_buttons_container {
     width: 100%;
     height: 100%;
@@ -180,14 +181,15 @@
 .store_handle_search_input_field {
     width: 100%;
 }
 
 .store_handle_search_clean_button {
     width: 100%;
     margin: 0 1 0 0;
+    height: 5;
 }
 
 .store_handle_item {
     width: 100%;
     height: 5;
     margin: 0 1 1 0;
     background: black;
@@ -206,26 +208,27 @@
 
 .store_handle_item_label {
     color: #e9ecef;
 }
 
 .store_handle_item_buttons_container {
     align: right middle;
-    height: 3;
+    height: 5;
     grid-size: 3 1;
     grid-columns: 1fr 1fr 1fr;
     margin: 0 1 0 1;
 }
 
 .store_handle_item_button,
 .store_handle_button {
     margin: 0 1 0 0;
     width: 100%;
     min-width: 10;
     align: right middle;
+    height: 5;
 }
 
 .store_handle_buttons_container {
     width: 100%;
     height: 3;
     margin: 0 1 0 1;
     grid-size: 3 1;
@@ -274,15 +277,15 @@
     color: #e9ecef;
     margin: 0 0 0 2;
 }
 
 .backup_manage_screen_container {
     width: 100%;
     height: 100%;
-    margin: 3;
+    margin: 1 3 0 3;
     align: center top;
     content-align: center middle;
 }
 
 .backup_manage_screen_no_backups_label {
     color: #e9ecef;
     width: 100%;
@@ -406,7 +409,61 @@
 }
 
 .help_screen_separator {
     width: 100%;
     height: 1;
     margin: 1 0 1 0;
 }
+
+
+.settings_handle_page_container {
+    width: 100%;
+    height: 100%;
+    margin: 1 4;
+}
+
+.settings_handle_page_buttons_container {
+    width: 100%;
+    height: 3;
+    grid-size: 3 1;
+    grid-columns: 1fr 1fr 1fr;
+}
+
+.settings_manage_screen_button {
+    width: 100%;
+    margin: 0 1 0 0;
+}
+
+.settings_manage_page_pairs_container {
+    width: 100%;
+    height: auto;
+    margin: 0 0 5 0;
+}
+
+.settings_manage_page_pairs_label {
+    width: 100%;
+    text-style: bold;
+    text-align: center;
+    margin: 4 0 2 0;
+}
+
+.settings_manage_page_pair_label_first,
+.settings_manage_page_pair_label_second {
+    text-align: justify;
+    height: auto;
+    margin: 1 0 0 0;
+    width: 100%;
+}
+
+.settings_manage_page_pair_container {
+    width: 100%;
+    height: 3;
+    grid-size: 3 1;
+    grid-columns: 1fr 1fr 1fr;
+    grid-rows: 1fr;
+    margin: 0 0 1 0;
+}
+
+.settings_manage_page_pair_button {
+    width: 100%;
+    margin: 0 5 0 10;
+}
```

### Comparing `doopass-2.5/doopass/doopass.py` & `doopass-2.7/doopass/doopass.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,51 @@
 """ A python module that helps you to manage your secret data. """
 import logging
 import sys
 from typing import override
+from uuid import uuid4
 
-from doopass_libs.core.screens.main_screen import MainScreen
 from rich.console import RenderableType
-from textual.app import ReturnType
-from textual.screen import Screen as textaulScreen
+from textual.app import ReturnType, ScreenError
+from textual.screen import Screen as textaulScreen, Screen
 
-from doopass.app import App
+from doopass.core.app import App
+from doopass.core.screens.main_screen import MainScreen
 
 
 class Doopass(App):
     def on_mount(self) -> None:
         main_screen = MainScreen(self)
         self.install_screen(main_screen, name="MainScreen")
         self.push_screen(main_screen)
         self.screen.styles.background = "black"
         logging.debug("The app has been launched")
 
-    @override
     def apply_screen(
             self, screen: textaulScreen, pop: bool = True, name: str | None = None
     ) -> None:
         screen.styles.background = "black"
 
         if name:
             self.app.install_screen(screen, name=name)
         else:
-            self.app.install_screen(screen)
+            self.app.install_screen(screen, name=uuid4().hex)
 
         if pop:
             self.app.pop_screen()
 
         self.app.push_screen(screen)
 
+    @override
+    def install_screen(self, screen: Screen, name: str) -> None:
+        try:
+            super().install_screen(screen, name)
+        except ScreenError:
+            pass
+
     def exit(self, result: ReturnType | None = None, return_code: int = 0, message: RenderableType | None = None,
              **kwargs) -> None:
         logging.debug("App exited\n")
         super().exit(result, return_code, message)
 
 
 def main() -> int:
```

