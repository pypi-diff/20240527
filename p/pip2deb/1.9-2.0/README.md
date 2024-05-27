# Comparing `tmp/pip2deb-1.9.tar.gz` & `tmp/pip2deb-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pip2deb-1.9.tar", last modified: Mon May 27 14:56:50 2024, max compression
+gzip compressed data, was "pip2deb-2.0.tar", last modified: Mon May 27 15:09:15 2024, max compression
```

## Comparing `pip2deb-1.9.tar` & `pip2deb-2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 whoami    (1002) whoami    (1002)        0 2024-05-27 14:56:50.789019 pip2deb-1.9/
--rw-r--r--   0 whoami    (1002) whoami    (1002)     3397 2024-05-26 20:11:06.000000 pip2deb-1.9/LICENSE
--rw-r--r--   0 whoami    (1002) whoami    (1002)     1415 2024-05-27 14:56:50.789019 pip2deb-1.9/PKG-INFO
--rw-r--r--   0 whoami    (1002) whoami    (1002)      976 2024-05-26 20:09:37.000000 pip2deb-1.9/README.rst
--rwxr-xr-x   0 whoami    (1002) whoami    (1002)     2772 2024-05-27 14:55:09.000000 pip2deb-1.9/pip2deb
-drwxr-xr-x   0 whoami    (1002) whoami    (1002)        0 2024-05-27 14:56:50.789019 pip2deb-1.9/pip2deb.egg-info/
--rw-r--r--   0 whoami    (1002) whoami    (1002)     1415 2024-05-27 14:56:50.000000 pip2deb-1.9/pip2deb.egg-info/PKG-INFO
--rw-r--r--   0 whoami    (1002) whoami    (1002)      159 2024-05-27 14:56:50.000000 pip2deb-1.9/pip2deb.egg-info/SOURCES.txt
--rw-r--r--   0 whoami    (1002) whoami    (1002)        1 2024-05-27 14:56:50.000000 pip2deb-1.9/pip2deb.egg-info/dependency_links.txt
--rw-r--r--   0 whoami    (1002) whoami    (1002)        1 2024-05-27 14:56:50.000000 pip2deb-1.9/pip2deb.egg-info/top_level.txt
--rw-r--r--   0 whoami    (1002) whoami    (1002)       38 2024-05-27 14:56:50.789019 pip2deb-1.9/setup.cfg
--rw-r--r--   0 whoami    (1002) whoami    (1002)      789 2024-05-27 14:56:38.000000 pip2deb-1.9/setup.py
+drwxr-xr-x   0 whoami    (1002) whoami    (1002)        0 2024-05-27 15:09:15.796549 pip2deb-2.0/
+-rw-r--r--   0 whoami    (1002) whoami    (1002)     3397 2024-05-26 20:11:06.000000 pip2deb-2.0/LICENSE
+-rw-r--r--   0 whoami    (1002) whoami    (1002)     1415 2024-05-27 15:09:15.796549 pip2deb-2.0/PKG-INFO
+-rw-r--r--   0 whoami    (1002) whoami    (1002)      976 2024-05-26 20:09:37.000000 pip2deb-2.0/README.rst
+-rwxr-xr-x   0 whoami    (1002) whoami    (1002)     3022 2024-05-27 15:06:42.000000 pip2deb-2.0/pip2deb
+drwxr-xr-x   0 whoami    (1002) whoami    (1002)        0 2024-05-27 15:09:15.796549 pip2deb-2.0/pip2deb.egg-info/
+-rw-r--r--   0 whoami    (1002) whoami    (1002)     1415 2024-05-27 15:09:15.000000 pip2deb-2.0/pip2deb.egg-info/PKG-INFO
+-rw-r--r--   0 whoami    (1002) whoami    (1002)      159 2024-05-27 15:09:15.000000 pip2deb-2.0/pip2deb.egg-info/SOURCES.txt
+-rw-r--r--   0 whoami    (1002) whoami    (1002)        1 2024-05-27 15:09:15.000000 pip2deb-2.0/pip2deb.egg-info/dependency_links.txt
+-rw-r--r--   0 whoami    (1002) whoami    (1002)        1 2024-05-27 15:09:15.000000 pip2deb-2.0/pip2deb.egg-info/top_level.txt
+-rw-r--r--   0 whoami    (1002) whoami    (1002)       38 2024-05-27 15:09:15.796549 pip2deb-2.0/setup.cfg
+-rw-r--r--   0 whoami    (1002) whoami    (1002)      789 2024-05-27 15:06:49.000000 pip2deb-2.0/setup.py
```

### Comparing `pip2deb-1.9/LICENSE` & `pip2deb-2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pip2deb-1.9/PKG-INFO` & `pip2deb-2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip2deb
-Version: 1.9
+Version: 2.0
 Home-page: https://github.com/pacspedd/pip2deb
 Author: PacSpedd
 Author-email: pacspedd@outlook.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pip2deb-1.9/README.rst` & `pip2deb-2.0/README.rst`

 * *Files identical despite different names*

### Comparing `pip2deb-1.9/pip2deb` & `pip2deb-2.0/pip2deb`

 * *Files 24% similar despite different names*

```diff
@@ -13,14 +13,19 @@
 cursive="\033[01;33m"
 bold="\033[01m"
 
 msg() {
     echo -e "${green}[${red}*${green}]${cyan} ${@:1} ${reset}" 2>&1
 }
 
+abort() {
+    msg "Unsuccessful, Canceling..."
+    exit 1
+}
+
 if [ "$#" -ne 2 ]; then
     msg "Usage: $0 <name> <distro>"
     exit 1
 fi
 
 case "${distro}" in
     debian|ubuntu)
@@ -37,70 +42,70 @@
         msg "Unsupported distribution: ${distro}"
         exit 1
         ;;
 esac
 
 # Creating Virtual Environment and install Module there
 msg "Setting up Venv ..."
-python -m venv .tmp-venv &>/dev/null
-source .tmp-venv/bin/activate
-pip install ${name} &>/dev/null
+python -m venv .tmp-venv &>/dev/null || abort
+source .tmp-venv/bin/activate || abort
+pip install ${name} &>/dev/null || abort
 
 # Grep Meta Data from Module
 msg "Grep Meta Data from Module"
-package=$(pip show ${name} | grep -E '^Name: ' | cut -d' ' -f2)
-version=$(pip show ${name} | grep -E '^Version: ' | cut -d' ' -f2)
-summary=$(pip show ${name} | grep -E '^Summary: ' | cut -d' ' -f2)
-author=$(pip show ${name} | grep -E '^Author: ' | cut -d' ' -f2)
-email=$(pip show ${name} | grep -E '^Author-email: ' | cut -d' ' -f2)
-pip_depends=$(pip show ${name} | grep -E '^Requires: ' | cut -d' ' -f2)
-arch=$(dpkg --print-architecture)
+package=$(pip show ${name} | grep -E '^Name: ' | cut -d' ' -f2) || abort
+version=$(pip show ${name} | grep -E '^Version: ' | cut -d' ' -f2) || abort
+summary=$(pip show ${name} | grep -E '^Summary: ' | cut -d' ' -f2) || abort
+author=$(pip show ${name} | grep -E '^Author: ' | cut -d' ' -f2) || abort
+email=$(pip show ${name} | grep -E '^Author-email: ' | cut -d' ' -f2) || abort
+pip_depends=$(pip show ${name} | grep -E '^Requires: ' | cut -d' ' -f2) || abort
+arch=$(dpkg --print-architecture) || abort
 
 #Struct Package
 msg "Struct Package"
 build_dir="${name}${pythonpath}"
 build_prefix="${name}${prefix}"
 debian_dir="${name}/DEBIAN"
 control_file="${debian_dir}/control"
 
 # Create Folder and Build distribution
-mkdir -p ${build_dir} ${debian_dir}
-touch ${control_file}
+mkdir -p ${build_dir} ${debian_dir} || abort
+touch ${control_file} || abort
 
 # Install PIP Module to build_dir
 msg "Install PIP Module to build_dir"
-pip install ${name} --target ${build_dir} &>/dev/null
+pip install ${name} --target ${build_dir} &>/dev/null || abort
 
 # Check for Bin in build_dir
 msg "Check for Bin in build_dir"
 if [ -d "${build_dir}/bin" ]; then
     msg "${green}Bin Folder Found"
-    mkdir -p ${build_prefix}/bin
-    cp -rf ${build_dir}/bin/* ${build_prefix}/bin
-    rm -rf ${build_dir}/bin
+    mkdir -p ${build_prefix}/bin || abort
+    cp -rf ${build_dir}/bin/* ${build_prefix}/bin || abort
+    rm -rf ${build_dir}/bin || abort
 else
     msg "${red}Bin Folder Not Found"
 fi
 
 # Create Control File and Give him Correct Rights
 msg "Create Control File and Give Rights"
-cat <<EOF > ${control_file}
+cat <<EOF > ${control_file} || abort
 Package: ${name}
 Version: ${version}
 Architecture: ${arch}
 Maintainer: ${author} <${email}>
 Depends: ${depends}
 Description: ${summary}
 EOF
 
 # Create Debian Package
 msg "Create Debian Package"
-chmod -R 755 ${name}
-dpkg-deb --build ${name} &>/dev/null
+chmod -R 755 ${name} || abort
+dpkg-deb --build ${name} &>/dev/null || abort
 package_name="${name}_${version}_${arch}_${distro}.deb"
-mv ${name}.deb ${package_name}
+mv ${name}.deb ${package_name} || abort
 
 msg "Package Created: ${package_name}, for distro: ${distro}:${arch}"
 msg "Cleaning Up"
-rm -rf ${name} .tmp-venv
+rm -rf ${name} .tmp-venv || abort
 
 msg "${green}Done"
```

### Comparing `pip2deb-1.9/pip2deb.egg-info/PKG-INFO` & `pip2deb-2.0/pip2deb.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip2deb
-Version: 1.9
+Version: 2.0
 Home-page: https://github.com/pacspedd/pip2deb
 Author: PacSpedd
 Author-email: pacspedd@outlook.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pip2deb-1.9/setup.py` & `pip2deb-2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 def readme():
     with open('README.rst', 'r') as f:
         content = f.read()
     return content
 
 setup(
     name="pip2deb",
-    version="1.9",
+    version="2.0",
     decription="A Simple Tool to Pack Python Project into a Debian Package, For Debian/Ubuntu and Termux",
     long_description=readme(),
     url='https://github.com/pacspedd/pip2deb',
     author="PacSpedd",
     author_email="pacspedd@outlook.com",
     license='MIT',
     classifiers=[
```

