# Comparing `tmp/pip2deb-1.7.tar.gz` & `tmp/pip2deb-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pip2deb-1.7.tar", last modified: Sun May 26 21:30:49 2024, max compression
+gzip compressed data, was "pip2deb-1.8.tar", last modified: Mon May 27 14:48:43 2024, max compression
```

## Comparing `pip2deb-1.7.tar` & `pip2deb-1.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 whoami    (1002) whoami    (1002)        0 2024-05-26 21:30:49.551975 pip2deb-1.7/
--rw-r--r--   0 whoami    (1002) whoami    (1002)     3397 2024-05-26 20:11:06.000000 pip2deb-1.7/LICENSE
--rw-r--r--   0 whoami    (1002) whoami    (1002)     1415 2024-05-26 21:30:49.551975 pip2deb-1.7/PKG-INFO
--rw-r--r--   0 whoami    (1002) whoami    (1002)      976 2024-05-26 20:09:37.000000 pip2deb-1.7/README.rst
--rwxr-xr-x   0 whoami    (1002) whoami    (1002)     2737 2024-05-26 21:30:24.000000 pip2deb-1.7/pip2deb
--rwxr-xr-x   0 whoami    (1002) whoami    (1002)     2759 2024-05-26 21:15:49.000000 pip2deb-1.7/pip2deb-sub
-drwxr-xr-x   0 whoami    (1002) whoami    (1002)        0 2024-05-26 21:30:49.551975 pip2deb-1.7/pip2deb.egg-info/
--rw-r--r--   0 whoami    (1002) whoami    (1002)     1415 2024-05-26 21:30:49.000000 pip2deb-1.7/pip2deb.egg-info/PKG-INFO
--rw-r--r--   0 whoami    (1002) whoami    (1002)      171 2024-05-26 21:30:49.000000 pip2deb-1.7/pip2deb.egg-info/SOURCES.txt
--rw-r--r--   0 whoami    (1002) whoami    (1002)        1 2024-05-26 21:30:49.000000 pip2deb-1.7/pip2deb.egg-info/dependency_links.txt
--rw-r--r--   0 whoami    (1002) whoami    (1002)        1 2024-05-26 21:30:49.000000 pip2deb-1.7/pip2deb.egg-info/top_level.txt
--rw-r--r--   0 whoami    (1002) whoami    (1002)       38 2024-05-26 21:30:49.551975 pip2deb-1.7/setup.cfg
--rw-r--r--   0 whoami    (1002) whoami    (1002)      788 2024-05-26 21:30:33.000000 pip2deb-1.7/setup.py
+drwxr-xr-x   0 whoami    (1002) whoami    (1002)        0 2024-05-27 14:48:43.771734 pip2deb-1.8/
+-rw-r--r--   0 whoami    (1002) whoami    (1002)     3397 2024-05-26 20:11:06.000000 pip2deb-1.8/LICENSE
+-rw-r--r--   0 whoami    (1002) whoami    (1002)     1415 2024-05-27 14:48:43.771734 pip2deb-1.8/PKG-INFO
+-rw-r--r--   0 whoami    (1002) whoami    (1002)      976 2024-05-26 20:09:37.000000 pip2deb-1.8/README.rst
+-rwxr-xr-x   0 whoami    (1002) whoami    (1002)     2769 2024-05-27 14:48:06.000000 pip2deb-1.8/pip2deb
+-rwxr-xr-x   0 whoami    (1002) whoami    (1002)     2759 2024-05-26 21:15:49.000000 pip2deb-1.8/pip2deb-sub
+drwxr-xr-x   0 whoami    (1002) whoami    (1002)        0 2024-05-27 14:48:43.771734 pip2deb-1.8/pip2deb.egg-info/
+-rw-r--r--   0 whoami    (1002) whoami    (1002)     1415 2024-05-27 14:48:43.000000 pip2deb-1.8/pip2deb.egg-info/PKG-INFO
+-rw-r--r--   0 whoami    (1002) whoami    (1002)      171 2024-05-27 14:48:43.000000 pip2deb-1.8/pip2deb.egg-info/SOURCES.txt
+-rw-r--r--   0 whoami    (1002) whoami    (1002)        1 2024-05-27 14:48:43.000000 pip2deb-1.8/pip2deb.egg-info/dependency_links.txt
+-rw-r--r--   0 whoami    (1002) whoami    (1002)        1 2024-05-27 14:48:43.000000 pip2deb-1.8/pip2deb.egg-info/top_level.txt
+-rw-r--r--   0 whoami    (1002) whoami    (1002)       38 2024-05-27 14:48:43.771734 pip2deb-1.8/setup.cfg
+-rw-r--r--   0 whoami    (1002) whoami    (1002)      788 2024-05-27 14:42:29.000000 pip2deb-1.8/setup.py
```

### Comparing `pip2deb-1.7/LICENSE` & `pip2deb-1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pip2deb-1.7/PKG-INFO` & `pip2deb-1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip2deb
-Version: 1.7
+Version: 1.8
 Home-page: https://github.com/pacspedd/pip2deb
 Author: PacSpedd
 Author-email: pacspedd@outlook.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pip2deb-1.7/README.rst` & `pip2deb-1.8/README.rst`

 * *Files identical despite different names*

### Comparing `pip2deb-1.7/pip2deb` & `pip2deb-1.8/pip2deb-sub`

 * *Files 4% similar despite different names*

```diff
@@ -25,22 +25,22 @@
         ;;
     *)
         msg "Unsupported distribution: ${distro}"
         exit 1
         ;;
 esac
 
-# Creating Virtual Environment and install Module there
+# Creating Virtual Environment and install Modul there
 msg "[*] Setting up Venv ..."
 python -m venv .tmp-venv &>/dev/null
 source .tmp-venv/bin/activate
 pip install ${name} &>/dev/null
 
-# Grep Meta Data from Module
-msg "[*] Grep Meta Data from Module"
+# Grep Meta Data from Modul
+msg "[*] Grep Meta Data from Modul"
 package=$(pip show ${name} | grep -E '^Name: ' | cut -d' ' -f2)
 version=$(pip show ${name} | grep -E '^Version: ' | cut -d' ' -f2)
 summary=$(pip show ${name} | grep -E '^Summary: ' | cut -d' ' -f2)
 author=$(pip show ${name} | grep -E '^Author: ' | cut -d' ' -f2)
 email=$(pip show ${name} | grep -E '^Author-email: ' | cut -d' ' -f2)
 pip_depends=$(pip show ${name} | grep -E '^Requires: ' | cut -d' ' -f2)
 arch=$(dpkg --print-architecture)
@@ -64,21 +64,22 @@
 msg "[*] Check for Bin in build_dir"
 if [ -d "${build_dir}/bin" ]; then
     msg "[*] Bin Folder Found"
     mkdir -p ${build_prefix}/bin
     cp -rf ${build_dir}/bin/* ${build_prefix}/bin
     rm -rf ${build_dir}/bin
 else
-    msg "[*] Bin Folder Not Found"
+    msg "[*] Bin Folder Not Foun"
 fi
 
-# Install Requires Separate
-msg "[*] Install Requirements Separate"
+# Install Requires Seperate
+msg "[*] Install Requirements Seperate"
 for dep in ${pip_depends}; do
-    pip2deb ${dep} ${distro}
+    pip2deb-sub ${dep} ${distro}
+    rm -rf ${build_dir}/${dep}*
 done
 
 # Create Control File and Give him Correct Rights
 msg "[*] Create Control File and Give Rights"
 cat <<EOF > ${control_file}
 Package: ${name}
 Version: ${version}
@@ -88,15 +89,15 @@
 Description: ${summary}
 EOF
 
 # Create Debian Package
 msg "[*] Create Debian Package"
 chmod -R 755 ${name}
 dpkg-deb --build ${name} &>/dev/null
-package_name="${name}_${version}_${arch}_${distro}.deb"
+package_name="${name}_${version}_${arch}.deb"
 mv ${name}.deb ${package_name}
 
 msg "[*] Package Created: ${package_name}, for distro: ${distro}:${arch}"
 msg "[*] Cleaning Up"
 rm -rf ${name} .tmp-venv
 
 msg "[*] Done"
```

### Comparing `pip2deb-1.7/pip2deb-sub` & `pip2deb-1.8/pip2deb`

 * *Files 26% similar despite different names*

```diff
@@ -1,103 +1,106 @@
 #!/bin/bash
 
 name="$1"
 distro="$2"
 
+# Define Colors
+# But without Tput
+green="\033[01;32m"
+red="\033[01;31m"
+blue="\033[01;34m"
+cyan="\033[01;36m"
+reset="\033[0m"
+cursive="\033[01;33m"
+bold="\033[01m"
+
 msg() {
-    echo "${@:1}" 2>&1
+    echo "${green}[${red}*${green}]${cyan} ${@:1} ${reset}" 2>&1
 }
 
 if [ "$#" -ne 2 ]; then
     msg "Usage: $0 <name> <distro>"
     exit 1
 fi
 
 case "${distro}" in
     debian|ubuntu)
         prefix="/usr"
         pythonpath="/usr/lib/python3/dist-packages"
-        depends="python3, python3-pip, python3-venv, python-is-python3"
+        depends="python3, python3-venv, python-is-python3"
         ;;
     termux)
         prefix="/data/data/com.termux/files/usr"
         pythonpath="/data/data/com.termux/files/usr/lib/python3.11/site-packages"
-        depends="python, python-pip"
+        depends="python, python"
         ;;
     *)
         msg "Unsupported distribution: ${distro}"
         exit 1
         ;;
 esac
 
-# Creating Virtual Environment and install Modul there
-msg "[*] Setting up Venv ..."
+# Creating Virtual Environment and install Module there
+msg "Setting up Venv ..."
 python -m venv .tmp-venv &>/dev/null
 source .tmp-venv/bin/activate
 pip install ${name} &>/dev/null
 
-# Grep Meta Data from Modul
-msg "[*] Grep Meta Data from Modul"
+# Grep Meta Data from Module
+msg "Grep Meta Data from Module"
 package=$(pip show ${name} | grep -E '^Name: ' | cut -d' ' -f2)
 version=$(pip show ${name} | grep -E '^Version: ' | cut -d' ' -f2)
 summary=$(pip show ${name} | grep -E '^Summary: ' | cut -d' ' -f2)
 author=$(pip show ${name} | grep -E '^Author: ' | cut -d' ' -f2)
 email=$(pip show ${name} | grep -E '^Author-email: ' | cut -d' ' -f2)
 pip_depends=$(pip show ${name} | grep -E '^Requires: ' | cut -d' ' -f2)
 arch=$(dpkg --print-architecture)
 
 #Struct Package
-msg "[*] Struct Package"
+msg "Struct Package"
 build_dir="${name}${pythonpath}"
 build_prefix="${name}${prefix}"
 debian_dir="${name}/DEBIAN"
 control_file="${debian_dir}/control"
 
 # Create Folder and Build distribution
 mkdir -p ${build_dir} ${debian_dir}
 touch ${control_file}
 
 # Install PIP Module to build_dir
-msg "[*] Install PIP Module to build_dir"
+msg "Install PIP Module to build_dir"
 pip install ${name} --target ${build_dir} &>/dev/null
 
 # Check for Bin in build_dir
-msg "[*] Check for Bin in build_dir"
+msg "Check for Bin in build_dir"
 if [ -d "${build_dir}/bin" ]; then
-    msg "[*] Bin Folder Found"
+    msg "${green}Bin Folder Found"
     mkdir -p ${build_prefix}/bin
     cp -rf ${build_dir}/bin/* ${build_prefix}/bin
     rm -rf ${build_dir}/bin
 else
-    msg "[*] Bin Folder Not Foun"
+    msg "${red}Bin Folder Not Found"
 fi
 
-# Install Requires Seperate
-msg "[*] Install Requirements Seperate"
-for dep in ${pip_depends}; do
-    pip2deb-sub ${dep} ${distro}
-    rm -rf ${build_dir}/${dep}*
-done
-
 # Create Control File and Give him Correct Rights
-msg "[*] Create Control File and Give Rights"
+msg "Create Control File and Give Rights"
 cat <<EOF > ${control_file}
 Package: ${name}
 Version: ${version}
 Architecture: ${arch}
 Maintainer: ${author} <${email}>
 Depends: ${depends}
 Description: ${summary}
 EOF
 
 # Create Debian Package
-msg "[*] Create Debian Package"
+msg "Create Debian Package"
 chmod -R 755 ${name}
 dpkg-deb --build ${name} &>/dev/null
-package_name="${name}_${version}_${arch}.deb"
+package_name="${name}_${version}_${arch}_${distro}.deb"
 mv ${name}.deb ${package_name}
 
-msg "[*] Package Created: ${package_name}, for distro: ${distro}:${arch}"
-msg "[*] Cleaning Up"
+msg "Package Created: ${package_name}, for distro: ${distro}:${arch}"
+msg "Cleaning Up"
 rm -rf ${name} .tmp-venv
 
-msg "[*] Done"
+msg "${green}Done"
```

### Comparing `pip2deb-1.7/pip2deb.egg-info/PKG-INFO` & `pip2deb-1.8/pip2deb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip2deb
-Version: 1.7
+Version: 1.8
 Home-page: https://github.com/pacspedd/pip2deb
 Author: PacSpedd
 Author-email: pacspedd@outlook.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pip2deb-1.7/setup.py` & `pip2deb-1.8/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 def readme():
     with open('README.rst', 'r') as f:
         content = f.read()
     return content
 
 setup(
     name="pip2deb",
-    version="1.7",
+    version="1.8",
     decription="A Simple Tool to Pack Python Project into a Debian Package, For Debian/Ubuntu and Termux",
     long_description=readme(),
     url='https://github.com/pacspedd/pip2deb',
     author="PacSpedd",
     author_email="pacspedd@outlook.com",
     license='MIT',
     classifiers=[
```

