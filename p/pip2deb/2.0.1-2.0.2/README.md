# Comparing `tmp/pip2deb-2.0.1.tar.gz` & `tmp/pip2deb-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pip2deb-2.0.1.tar", last modified: Mon May 27 15:28:19 2024, max compression
+gzip compressed data, was "pip2deb-2.0.2.tar", last modified: Mon May 27 15:56:18 2024, max compression
```

## Comparing `pip2deb-2.0.1.tar` & `pip2deb-2.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 whoami    (1002) whoami    (1002)        0 2024-05-27 15:28:19.752925 pip2deb-2.0.1/
--rw-r--r--   0 whoami    (1002) whoami    (1002)     3397 2024-05-26 20:11:06.000000 pip2deb-2.0.1/LICENSE
--rw-r--r--   0 whoami    (1002) whoami    (1002)     1417 2024-05-27 15:28:19.752925 pip2deb-2.0.1/PKG-INFO
--rw-r--r--   0 whoami    (1002) whoami    (1002)      976 2024-05-26 20:09:37.000000 pip2deb-2.0.1/README.rst
--rwxr-xr-x   0 whoami    (1002) whoami    (1002)     3448 2024-05-27 15:27:24.000000 pip2deb-2.0.1/pip2deb
-drwxr-xr-x   0 whoami    (1002) whoami    (1002)        0 2024-05-27 15:28:19.752925 pip2deb-2.0.1/pip2deb.egg-info/
--rw-r--r--   0 whoami    (1002) whoami    (1002)     1417 2024-05-27 15:28:19.000000 pip2deb-2.0.1/pip2deb.egg-info/PKG-INFO
--rw-r--r--   0 whoami    (1002) whoami    (1002)      159 2024-05-27 15:28:19.000000 pip2deb-2.0.1/pip2deb.egg-info/SOURCES.txt
--rw-r--r--   0 whoami    (1002) whoami    (1002)        1 2024-05-27 15:28:19.000000 pip2deb-2.0.1/pip2deb.egg-info/dependency_links.txt
--rw-r--r--   0 whoami    (1002) whoami    (1002)        1 2024-05-27 15:28:19.000000 pip2deb-2.0.1/pip2deb.egg-info/top_level.txt
--rw-r--r--   0 whoami    (1002) whoami    (1002)       38 2024-05-27 15:28:19.752925 pip2deb-2.0.1/setup.cfg
--rw-r--r--   0 whoami    (1002) whoami    (1002)      791 2024-05-27 15:27:36.000000 pip2deb-2.0.1/setup.py
+drwxr-xr-x   0 whoami    (1002) whoami    (1002)        0 2024-05-27 15:56:18.058532 pip2deb-2.0.2/
+-rw-r--r--   0 whoami    (1002) whoami    (1002)     3397 2024-05-26 20:11:06.000000 pip2deb-2.0.2/LICENSE
+-rw-r--r--   0 whoami    (1002) whoami    (1002)     1417 2024-05-27 15:56:18.058532 pip2deb-2.0.2/PKG-INFO
+-rw-r--r--   0 whoami    (1002) whoami    (1002)      976 2024-05-26 20:09:37.000000 pip2deb-2.0.2/README.rst
+-rwxr-xr-x   0 whoami    (1002) whoami    (1002)     4807 2024-05-27 15:56:02.000000 pip2deb-2.0.2/pip2deb
+drwxr-xr-x   0 whoami    (1002) whoami    (1002)        0 2024-05-27 15:56:18.058532 pip2deb-2.0.2/pip2deb.egg-info/
+-rw-r--r--   0 whoami    (1002) whoami    (1002)     1417 2024-05-27 15:56:18.000000 pip2deb-2.0.2/pip2deb.egg-info/PKG-INFO
+-rw-r--r--   0 whoami    (1002) whoami    (1002)      159 2024-05-27 15:56:18.000000 pip2deb-2.0.2/pip2deb.egg-info/SOURCES.txt
+-rw-r--r--   0 whoami    (1002) whoami    (1002)        1 2024-05-27 15:56:18.000000 pip2deb-2.0.2/pip2deb.egg-info/dependency_links.txt
+-rw-r--r--   0 whoami    (1002) whoami    (1002)        1 2024-05-27 15:56:18.000000 pip2deb-2.0.2/pip2deb.egg-info/top_level.txt
+-rw-r--r--   0 whoami    (1002) whoami    (1002)       38 2024-05-27 15:56:18.058532 pip2deb-2.0.2/setup.cfg
+-rw-r--r--   0 whoami    (1002) whoami    (1002)      791 2024-05-27 15:56:07.000000 pip2deb-2.0.2/setup.py
```

### Comparing `pip2deb-2.0.1/LICENSE` & `pip2deb-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pip2deb-2.0.1/PKG-INFO` & `pip2deb-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip2deb
-Version: 2.0.1
+Version: 2.0.2
 Home-page: https://github.com/pacspedd/pip2deb
 Author: PacSpedd
 Author-email: pacspedd@outlook.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pip2deb-2.0.1/README.rst` & `pip2deb-2.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `pip2deb-2.0.1/pip2deb` & `pip2deb-2.0.2/pip2deb`

 * *Files 25% similar despite different names*

```diff
@@ -1,37 +1,74 @@
 #!/bin/bash
 
 name="$1"
 distro="$2"
+flags="${@:3}"
 
 # Define Colors
-# But without Tput
 green="\033[01;32m"
 red="\033[01;31m"
 blue="\033[01;34m"
 cyan="\033[01;36m"
 reset="\033[0m"
-cursive="\033[01;33m"
-bold="\033[01m"
 
+# Funktionen definieren
 msg() {
     echo -e "${green}[${red}*${green}]${cyan} ${@:1} ${reset}" 2>&1
 }
 
 abort() {
     msg "${red}Unsuccessful, Canceling..."
     rm -rf .tmp-venv
     exit 1
 }
 
-if [ "$#" -ne 2 ]; then
-    msg "Usage: $0 <name> <distro>"
+handle_flags() {
+    if [ -n "${flags}" ]; then
+        msg "${green}Flags Found"
+        for flag in ${flags}; do
+            case "${flag}" in
+                --debug|-d)
+                    msg "${green}${flag} is valid"
+                    exec &> ${name}-output.log
+                    ;;
+                --install|-i)
+                    handle_installation
+                    ;;
+                *)
+                    msg "${red}${flag} is invalid"
+                    ;;
+            esac
+        done
+    fi
+}
+
+handle_installation() {
+    msg "${green}${flag} is Valid"
+    if [[ ${distro} == "debian" || ${distro} == "ubuntu" ]]; then
+        if ! command -v sudo &>/dev/null; then
+            dpkg -i --force-overwrite ${package_name} &>/dev/null || abort
+            msg "${green}${blue}${package_name}${green} Successfully Installed"
+        else
+            sudo dpkg -i --force-overwrite ${package_name} &>/dev/null || abort
+            msg "${green}${blue}${package_name}${green} Successfully Installed"
+        fi
+    else
+        dpkg -i --force-overwrite ${package_name} &>/dev/null || abort
+        msg "${green}${blue}${package_name}${green} Successfully Installed"
+    fi
+}
+
+# Überprüfung der Eingabeparameter
+if [ "$#" -ne 3 ]; then
+    msg "Usage: $0 <name> <distro> <flags>"
     exit 1
 fi
 
+# Unterstützte Distributionen
 case "${distro}" in
     debian|ubuntu)
         prefix="/usr"
         pythonpath="/usr/lib/python3/dist-packages"
         depends="python3, python3-venv, python-is-python3"
         ;;
     termux)
@@ -41,81 +78,85 @@
         ;;
     *)
         msg "Unsupported distribution: ${distro}"
         exit 1
         ;;
 esac
 
-# Creating Virtual Environment and install Module there
+# Virtuelle Umgebung erstellen und Modul installieren
 msg "Setting up Venv ..."
 python -m venv .tmp-venv &>/dev/null || abort
 source .tmp-venv/bin/activate || abort
 pip install ${name} &>/dev/null || abort
 
-# Grep Meta Data from Module
+# Metadaten aus dem Modul extrahieren
 msg "Grep Meta Data from Module"
 package=$(pip show ${name} | grep -E '^Name: ' | cut -d' ' -f2) || abort
 version=$(pip show ${name} | grep -E '^Version: ' | cut -d' ' -f2) || abort
 summary=$(pip show ${name} | grep -E '^Summary: ' | cut -d' ' -f2) || abort
 author=$(pip show ${name} | grep -E '^Author: ' | cut -d' ' -f2) || abort
 email=$(pip show ${name} | grep -E '^Author-email: ' | cut -d' ' -f2) || abort
 pip_depends=$(pip show ${name} | grep -E '^Requires: ' | cut -d' ' -f2) || abort
 arch=$(dpkg --print-architecture) || abort
 
-#Struct Package
+# Paketstruktur aufbauen
 msg "Struct Package"
 build_dir="${name}${pythonpath}"
 build_prefix="${name}${prefix}"
 debian_dir="${name}/DEBIAN"
 control_file="${debian_dir}/control"
 
-# Create Folder and Build distribution
+# Verzeichnisse erstellen und Distribution aufbauen
 mkdir -p ${build_dir} ${debian_dir} || abort
 touch ${control_file} || abort
 
-# Install PIP Module to build_dir
+# PIP-Modul in build_dir installieren
 msg "Install PIP Module to build_dir"
 pip install ${name} --target ${build_dir} &>/dev/null || abort
 
-# Check for Bin in build_dir
+# Überprüfung auf Bin-Verzeichnis in build_dir
 msg "Check for Bin in build_dir"
 if [ -d "${build_dir}/bin" ]; then
     msg "${green}Bin Folder Found"
     mkdir -p ${build_prefix}/bin || abort
     cp -rf ${build_dir}/bin/* ${build_prefix}/bin || abort
     rm -rf ${build_dir}/bin || abort
-    # Fix Shebang, and add Shebang to bin, if the hebang ending with python or python3
+    # Shebang korrigieren
     msg "Fix Shebang and Correct to the Right Shebang"
     for file in $(find ${build_prefix}/bin -type f); do
         shebang=$(head -n 1 ${file})
         if [[ ${shebang} =~ ^#!.*/python[0-9.]+$ ]]; then
             sed -i "1s|#!.*/python[0-9.]+|#!${prefix}/bin/python3|" ${file} || abort
         fi
+        if [[ ${distro} == "termux" ]]; then
+            termux-fix-shebang ${file} || abort
+        fi
     done
 else
     msg "${red}Bin Folder Not Found"
 fi
 
-
-# Create Control File and Give him Correct Rights
+# Control-Datei erstellen und Rechte setzen
 msg "Create Control File and Give Rights"
 cat <<EOF > ${control_file} || abort
 Package: ${name}
 Version: ${version}
 Architecture: ${arch}
 Maintainer: ${author} <${email}>
 Depends: ${depends}
 Description: ${summary}
 EOF
 
-# Create Debian Package
+# Debian-Paket erstellen
 msg "Create Debian Package"
 chmod -R 755 ${name} || abort
 dpkg-deb --build ${name} &>/dev/null || abort
 package_name="${name}_${version}_${arch}_${distro}.deb"
 mv ${name}.deb ${package_name} || abort
 
 msg "Package Created: ${package_name}, for distro: ${distro}:${arch}"
 msg "Cleaning Up"
 rm -rf ${name} .tmp-venv || abort
 
+handle_flags
+
 msg "${green}Done"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pip2deb-2.0.1/pip2deb.egg-info/PKG-INFO` & `pip2deb-2.0.2/pip2deb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip2deb
-Version: 2.0.1
+Version: 2.0.2
 Home-page: https://github.com/pacspedd/pip2deb
 Author: PacSpedd
 Author-email: pacspedd@outlook.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pip2deb-2.0.1/setup.py` & `pip2deb-2.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 def readme():
     with open('README.rst', 'r') as f:
         content = f.read()
     return content
 
 setup(
     name="pip2deb",
-    version="2.0.1",
+    version="2.0.2",
     decription="A Simple Tool to Pack Python Project into a Debian Package, For Debian/Ubuntu and Termux",
     long_description=readme(),
     url='https://github.com/pacspedd/pip2deb',
     author="PacSpedd",
     author_email="pacspedd@outlook.com",
     license='MIT',
     classifiers=[
```

