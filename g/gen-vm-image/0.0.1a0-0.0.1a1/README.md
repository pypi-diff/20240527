# Comparing `tmp/gen_vm_image-0.0.1a0.tar.gz` & `tmp/gen_vm_image-0.0.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gen_vm_image-0.0.1a0.tar", last modified: Mon May 27 15:30:39 2024, max compression
+gzip compressed data, was "gen_vm_image-0.0.1a1.tar", last modified: Mon May 27 18:54:50 2024, max compression
```

## Comparing `gen_vm_image-0.0.1a0.tar` & `gen_vm_image-0.0.1a1.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-sr-x   0 go        (1000) root         (0)        0 2024-05-27 15:30:39.873492 gen_vm_image-0.0.1a0/
--rw-r--r--   0 go        (1000) root         (0)     5432 2024-05-27 15:30:39.873492 gen_vm_image-0.0.1a0/PKG-INFO
--rw-r--r--   0 go        (1000) root         (0)     4365 2024-05-27 15:30:25.000000 gen_vm_image-0.0.1a0/README.rst
-drwxr-sr-x   0 go        (1000) root         (0)        0 2024-05-27 15:30:39.870492 gen_vm_image-0.0.1a0/gen_vm_image/
--rw-r--r--   0 go        (1000) root         (0)        0 2024-05-27 15:30:25.000000 gen_vm_image-0.0.1a0/gen_vm_image/__init__.py
--rw-r--r--   0 go        (1000) root         (0)     1557 2024-05-27 15:30:25.000000 gen_vm_image-0.0.1a0/gen_vm_image/architecture.py
-drwxr-sr-x   0 go        (1000) root         (0)        0 2024-05-27 15:30:39.871492 gen_vm_image-0.0.1a0/gen_vm_image/cli/
--rw-r--r--   0 go        (1000) root         (0)        0 2024-05-27 15:30:25.000000 gen_vm_image-0.0.1a0/gen_vm_image/cli/__init__.py
--rw-r--r--   0 go        (1000) root         (0)    15925 2024-05-27 15:30:25.000000 gen_vm_image-0.0.1a0/gen_vm_image/cli/build_image.py
-drwxr-sr-x   0 go        (1000) root         (0)        0 2024-05-27 15:30:39.871492 gen_vm_image-0.0.1a0/gen_vm_image/common/
--rw-r--r--   0 go        (1000) root         (0)        0 2024-05-27 15:30:25.000000 gen_vm_image-0.0.1a0/gen_vm_image/common/__init__.py
--rw-r--r--   0 go        (1000) root         (0)      362 2024-05-27 15:30:25.000000 gen_vm_image-0.0.1a0/gen_vm_image/common/defaults.py
--rw-r--r--   0 go        (1000) root         (0)      484 2024-05-27 15:30:25.000000 gen_vm_image-0.0.1a0/gen_vm_image/common/errors.py
-drwxr-sr-x   0 go        (1000) root         (0)        0 2024-05-27 15:30:39.872492 gen_vm_image-0.0.1a0/gen_vm_image/utils/
--rw-r--r--   0 go        (1000) root         (0)        0 2024-05-27 15:30:25.000000 gen_vm_image-0.0.1a0/gen_vm_image/utils/__init__.py
--rw-r--r--   0 go        (1000) root         (0)     3938 2024-05-27 15:30:25.000000 gen_vm_image-0.0.1a0/gen_vm_image/utils/io.py
--rw-r--r--   0 go        (1000) root         (0)     1623 2024-05-27 15:30:25.000000 gen_vm_image-0.0.1a0/gen_vm_image/utils/job.py
--rw-r--r--   0 go        (1000) root         (0)      759 2024-05-27 15:30:25.000000 gen_vm_image-0.0.1a0/gen_vm_image/utils/user.py
-drwxr-sr-x   0 go        (1000) root         (0)        0 2024-05-27 15:30:39.872492 gen_vm_image-0.0.1a0/gen_vm_image.egg-info/
--rw-r--r--   0 go        (1000) root         (0)     5432 2024-05-27 15:30:39.000000 gen_vm_image-0.0.1a0/gen_vm_image.egg-info/PKG-INFO
--rw-r--r--   0 go        (1000) root         (0)      614 2024-05-27 15:30:39.000000 gen_vm_image-0.0.1a0/gen_vm_image.egg-info/SOURCES.txt
--rw-r--r--   0 go        (1000) root         (0)        1 2024-05-27 15:30:39.000000 gen_vm_image-0.0.1a0/gen_vm_image.egg-info/dependency_links.txt
--rw-r--r--   0 go        (1000) root         (0)       66 2024-05-27 15:30:39.000000 gen_vm_image-0.0.1a0/gen_vm_image.egg-info/entry_points.txt
--rw-r--r--   0 go        (1000) root         (0)      109 2024-05-27 15:30:39.000000 gen_vm_image-0.0.1a0/gen_vm_image.egg-info/requires.txt
--rw-r--r--   0 go        (1000) root         (0)       13 2024-05-27 15:30:39.000000 gen_vm_image-0.0.1a0/gen_vm_image.egg-info/top_level.txt
--rw-r--r--   0 go        (1000) root         (0)       38 2024-05-27 15:30:39.873492 gen_vm_image-0.0.1a0/setup.cfg
--rw-r--r--   0 go        (1000) root         (0)     1690 2024-05-27 15:30:25.000000 gen_vm_image-0.0.1a0/setup.py
-drwxr-sr-x   0 go        (1000) root         (0)        0 2024-05-27 15:30:39.872492 gen_vm_image-0.0.1a0/tests/
--rw-r--r--   0 go        (1000) root         (0)     3324 2024-05-27 15:30:25.000000 gen_vm_image-0.0.1a0/tests/test_image_architecture.py
--rw-r--r--   0 go        (1000) root         (0)     2781 2024-05-27 15:30:25.000000 gen_vm_image-0.0.1a0/tests/test_image_build.py
+drwxr-sr-x   0 go        (1000) root         (0)        0 2024-05-27 18:54:50.267986 gen_vm_image-0.0.1a1/
+-rw-r--r--   0 go        (1000) root         (0)     5391 2024-05-27 18:54:50.267986 gen_vm_image-0.0.1a1/PKG-INFO
+-rw-r--r--   0 go        (1000) root         (0)     4324 2024-05-27 18:54:35.000000 gen_vm_image-0.0.1a1/README.rst
+drwxr-sr-x   0 go        (1000) root         (0)        0 2024-05-27 18:54:50.263986 gen_vm_image-0.0.1a1/gen_vm_image/
+-rw-r--r--   0 go        (1000) root         (0)        0 2024-05-27 18:54:35.000000 gen_vm_image-0.0.1a1/gen_vm_image/__init__.py
+-rw-r--r--   0 go        (1000) root         (0)     1557 2024-05-27 18:54:35.000000 gen_vm_image-0.0.1a1/gen_vm_image/architecture.py
+drwxr-sr-x   0 go        (1000) root         (0)        0 2024-05-27 18:54:50.264986 gen_vm_image-0.0.1a1/gen_vm_image/cli/
+-rw-r--r--   0 go        (1000) root         (0)        0 2024-05-27 18:54:35.000000 gen_vm_image-0.0.1a1/gen_vm_image/cli/__init__.py
+-rw-r--r--   0 go        (1000) root         (0)    15468 2024-05-27 18:54:35.000000 gen_vm_image-0.0.1a1/gen_vm_image/cli/build_image.py
+drwxr-sr-x   0 go        (1000) root         (0)        0 2024-05-27 18:54:50.265986 gen_vm_image-0.0.1a1/gen_vm_image/common/
+-rw-r--r--   0 go        (1000) root         (0)        0 2024-05-27 18:54:35.000000 gen_vm_image-0.0.1a1/gen_vm_image/common/__init__.py
+-rw-r--r--   0 go        (1000) root         (0)      362 2024-05-27 18:54:35.000000 gen_vm_image-0.0.1a1/gen_vm_image/common/defaults.py
+-rw-r--r--   0 go        (1000) root         (0)      611 2024-05-27 18:54:35.000000 gen_vm_image-0.0.1a1/gen_vm_image/common/errors.py
+drwxr-sr-x   0 go        (1000) root         (0)        0 2024-05-27 18:54:50.266986 gen_vm_image-0.0.1a1/gen_vm_image/utils/
+-rw-r--r--   0 go        (1000) root         (0)        0 2024-05-27 18:54:35.000000 gen_vm_image-0.0.1a1/gen_vm_image/utils/__init__.py
+-rw-r--r--   0 go        (1000) root         (0)     3939 2024-05-27 18:54:35.000000 gen_vm_image-0.0.1a1/gen_vm_image/utils/io.py
+-rw-r--r--   0 go        (1000) root         (0)     1623 2024-05-27 18:54:35.000000 gen_vm_image-0.0.1a1/gen_vm_image/utils/job.py
+-rw-r--r--   0 go        (1000) root         (0)      491 2024-05-27 18:54:35.000000 gen_vm_image-0.0.1a1/gen_vm_image/utils/net.py
+-rw-r--r--   0 go        (1000) root         (0)      759 2024-05-27 18:54:35.000000 gen_vm_image-0.0.1a1/gen_vm_image/utils/user.py
+drwxr-sr-x   0 go        (1000) root         (0)        0 2024-05-27 18:54:50.266986 gen_vm_image-0.0.1a1/gen_vm_image.egg-info/
+-rw-r--r--   0 go        (1000) root         (0)     5391 2024-05-27 18:54:50.000000 gen_vm_image-0.0.1a1/gen_vm_image.egg-info/PKG-INFO
+-rw-r--r--   0 go        (1000) root         (0)      640 2024-05-27 18:54:50.000000 gen_vm_image-0.0.1a1/gen_vm_image.egg-info/SOURCES.txt
+-rw-r--r--   0 go        (1000) root         (0)        1 2024-05-27 18:54:50.000000 gen_vm_image-0.0.1a1/gen_vm_image.egg-info/dependency_links.txt
+-rw-r--r--   0 go        (1000) root         (0)       66 2024-05-27 18:54:50.000000 gen_vm_image-0.0.1a1/gen_vm_image.egg-info/entry_points.txt
+-rw-r--r--   0 go        (1000) root         (0)      109 2024-05-27 18:54:50.000000 gen_vm_image-0.0.1a1/gen_vm_image.egg-info/requires.txt
+-rw-r--r--   0 go        (1000) root         (0)       13 2024-05-27 18:54:50.000000 gen_vm_image-0.0.1a1/gen_vm_image.egg-info/top_level.txt
+-rw-r--r--   0 go        (1000) root         (0)       38 2024-05-27 18:54:50.267986 gen_vm_image-0.0.1a1/setup.cfg
+-rw-r--r--   0 go        (1000) root         (0)     1690 2024-05-27 18:54:35.000000 gen_vm_image-0.0.1a1/setup.py
+drwxr-sr-x   0 go        (1000) root         (0)        0 2024-05-27 18:54:50.266986 gen_vm_image-0.0.1a1/tests/
+-rw-r--r--   0 go        (1000) root         (0)     3324 2024-05-27 18:54:35.000000 gen_vm_image-0.0.1a1/tests/test_image_architecture.py
+-rw-r--r--   0 go        (1000) root         (0)     2781 2024-05-27 18:54:35.000000 gen_vm_image-0.0.1a1/tests/test_image_build.py
```

### Comparing `gen_vm_image-0.0.1a0/PKG-INFO` & `gen_vm_image-0.0.1a1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen-vm-image
-Version: 0.0.1a0
+Version: 0.0.1a1
 Summary: This tool can be used for generating virtual machine images.
 Home-page: https://github.com/ucphhpc/gen-vm-image
 Author: Rasmus Munk
 Author-email: munk1@live.dk
 License: MIT
 Keywords: Virtual Machine,VM,Images
 Classifier: Intended Audience :: Developers
@@ -29,15 +29,15 @@
 Requires-Dist: docutils==0.18.1; extra == "dev"
 Requires-Dist: flake8==6.0.0; extra == "dev"
 
 ============
 gen-vm-image
 ============
 
-This package can be used for generating and configuring virtual machine images.
+This package can be used for generating virtual machine images.
 
 ------------
 Dependencies
 ------------
 
 The dependencies required to use this package to generate virtual machine images
 can be found in the ``dep`` directory for the supported distributions.
@@ -93,19 +93,19 @@
                                  [--generate-gocd-config]
                                  [--gocd-config-name GOCD_CONFIG_NAME]
                                  [--gocd-build-branch GOCD_BUILD_BRANCH]
 
         optional arguments:
         -h, --help            show this help message and exit
         --architecture-path ARCHITECTURE_PATH
-                                The path to the architecture file that is used to configure the images to be built (default: architecture.yml)
+                                The path to the architecture file that is used to build images (default: architecture.yml)
         --image-output-path IMAGE_OUTPUT_PATH
                                 The output path of the built image (default: generated-images/image.qcow2)
         --generated-image-owner GENERATED_IMAGE_OWNER
-                                Set the uid owner of the configured image (default: qemu)
+                                Set the uid owner of the built image (default: qemu)
         --generate-gocd-config
                                 Generate a GoCD config based on the architecture file (default: False)
         --gocd-config-name GOCD_CONFIG_NAME
                                 Name of the generated gocd config file (default: 1.gocd.yml)
         --gocd-build-branch GOCD_BUILD_BRANCH
                                 The branch that GoCD should use to build images (default: main)
```

### Comparing `gen_vm_image-0.0.1a0/README.rst` & `gen_vm_image-0.0.1a1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ============
 gen-vm-image
 ============
 
-This package can be used for generating and configuring virtual machine images.
+This package can be used for generating virtual machine images.
 
 ------------
 Dependencies
 ------------
 
 The dependencies required to use this package to generate virtual machine images
 can be found in the ``dep`` directory for the supported distributions.
@@ -62,19 +62,19 @@
                                  [--generate-gocd-config]
                                  [--gocd-config-name GOCD_CONFIG_NAME]
                                  [--gocd-build-branch GOCD_BUILD_BRANCH]
 
         optional arguments:
         -h, --help            show this help message and exit
         --architecture-path ARCHITECTURE_PATH
-                                The path to the architecture file that is used to configure the images to be built (default: architecture.yml)
+                                The path to the architecture file that is used to build images (default: architecture.yml)
         --image-output-path IMAGE_OUTPUT_PATH
                                 The output path of the built image (default: generated-images/image.qcow2)
         --generated-image-owner GENERATED_IMAGE_OWNER
-                                Set the uid owner of the configured image (default: qemu)
+                                Set the uid owner of the built image (default: qemu)
         --generate-gocd-config
                                 Generate a GoCD config based on the architecture file (default: False)
         --gocd-config-name GOCD_CONFIG_NAME
                                 Name of the generated gocd config file (default: 1.gocd.yml)
         --gocd-build-branch GOCD_BUILD_BRANCH
                                 The branch that GoCD should use to build images (default: main)
```

### Comparing `gen_vm_image-0.0.1a0/gen_vm_image/architecture.py` & `gen_vm_image-0.0.1a1/gen_vm_image/architecture.py`

 * *Files identical despite different names*

### Comparing `gen_vm_image-0.0.1a0/gen_vm_image/cli/build_image.py` & `gen_vm_image-0.0.1a1/gen_vm_image/cli/build_image.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 import argparse
 import os
 import yaml
-import requests
-import shutil
-from tqdm.auto import tqdm
 from gen_vm_image.common.defaults import (
     GOCD_GROUP,
     GOCD_TEMPLATE,
     REPO_NAME,
     PACKAGE_NAME,
     GENERATED_IMAGE_DIR,
     TMP_DIR,
@@ -20,18 +17,23 @@
     PATH_CREATE_ERROR,
     PATH_CREATE_ERROR_MSG,
     MISSING_ATTRIBUTE_ERROR,
     MISSING_ATTRIBUTE_ERROR_MSG,
     INVALID_ATTRIBUTE_TYPE_ERROR,
     INVALID_ATTRIBUTE_TYPE_ERROR_MSG,
     CHECKSUM_ERROR,
+    RESIZE_ERROR,
+    RESIZE_ERROR_MSG,
+    CHECK_ERROR,
+    CHECK_ERROR_MSG,
 )
 from gen_vm_image.architecture import load_architecture, correct_architecture_structure
 from gen_vm_image.utils.io import exists, makedirs, write, hashsum
 from gen_vm_image.utils.job import run
+from gen_vm_image.utils.net import download_file
 
 
 current_dir = os.path.abspath(os.path.dirname(__file__))
 parent_dir = os.path.dirname(current_dir)
 
 
 def get_pipelines(images):
@@ -99,40 +101,56 @@
         upstream_materials = get_upstream_materials(name, upstream_pipeline, stage)
         materials.update(upstream_materials)
     return materials
 
 
 def create_image(name, version, size, image_format="qcow2"):
     image_name = "{}-{}.{}".format(name, version, image_format)
-    create_image_command = ["qemu-img", "create", "-f", image_format, image_name, size]
-    created_result = run(create_image_command, format_output_str=True)
-    if created_result["returncode"] != "0":
+    command = ["qemu-img", "create", "-f", image_format, image_name, size]
+    result = run(command, format_output_str=True)
+    if result["returncode"] != "0":
         return PATH_CREATE_ERROR, PATH_CREATE_ERROR_MSG.format(
-            image_name, created_result["error"]
+            image_name, result["error"]
         )
-    return created_result, None
+    return result, None
 
 
 def convert_image(input_path, output_path, input_format="qcow2", output_format="qcow2"):
-    convert_image_command = [
+    command = [
         "qemu-img",
         "convert",
         "-f",
         input_format,
         "-O",
         output_format,
         input_path,
         output_path,
     ]
-    converted_result = run(convert_image_command, format_output_str=True)
-    if converted_result["returncode"] != "0":
+    result = run(command, format_output_str=True)
+    if result["returncode"] != "0":
         return PATH_CREATE_ERROR, PATH_CREATE_ERROR_MSG.format(
-            input_path, converted_result["error"]
+            input_path, result["error"]
         )
-    return converted_result, None
+    return result, None
+
+
+def resize_image(path, size):
+    command = ["qemu-img", "resize", path, size]
+    result = run(command, format_output_str=True)
+    if result["returncode"] != "0":
+        return RESIZE_ERROR, RESIZE_ERROR_MSG.format(result["error"])
+    return result, None
+
+
+def check_image(path, image_format="qcow2"):
+    command = ["qemu-img", "check", "-f", image_format, path]
+    result = run(command, format_output_str=True)
+    if result["returncode"] != "0":
+        return CHECK_ERROR, CHECK_ERROR_MSG.format(result["error"])
+    return result, None
 
 
 def build_gocd_config(architecture, gocd_name, branch, verbose):
     images = architecture.get("images", [])
 
     # GOCD file
     list_images = list(images.keys())
@@ -163,15 +181,15 @@
             "materials": materials,
             "parameters": {
                 "IMAGE": name,
                 "IMAGE_PIPELINE": build_version_name,
                 "DEFAULT_TAG": version,
                 "SRC_DIRECTORY": REPO_NAME,
                 "TEST_DIRECTORY": REPO_NAME,
-                "PUSH_DIRECTORY": "publish-docker-scripts",
+                "PUSH_DIRECTORY": "publish-python-scripts",
                 "COMMIT_TAG": GO_REVISION_COMMIT_VAR,
                 "ARGS": "",
             },
         }
         generated_config["pipelines"][build_version_name] = build_pipeline
 
     gocd_config_path = os.path.join(current_dir, gocd_name)
@@ -204,16 +222,14 @@
         if not created:
             print(PATH_CREATE_ERROR_MSG.format(images_output_directory, msg))
             exit(PATH_CREATE_ERROR)
 
     images = architecture.get("images", [])
     # Generate the image configuration
     for build, build_data in images.items():
-        # Base command used to either create or convert an image
-        disc_action = ["qemu-img"]
         vm_name = build_data["name"]
         vm_version = build_data["version"]
         vm_size = build_data["size"]
 
         # Optional attributes for each image configuration
         vm_output_format = build_data.get("format", "qcow2")
         vm_input, vm_input_format = None, "qcow2"
@@ -289,24 +305,15 @@
                         exit(PATH_CREATE_ERROR)
 
                 input_url_filename = vm_input_url.split("/")[-1]
                 input_vm_path = os.path.join(TMP_DIR, input_url_filename)
                 if not exists(input_vm_path):
                     if verbose:
                         print("Downloading image from: {}".format(vm_input_url))
-                    with requests.get(vm_input_url, stream=True) as r:
-                        # check header to get content length, in bytes
-                        total_length = int(r.headers.get("Content-Length"))
-                        # implement progress bar via tqdm
-                        with tqdm.wrapattr(
-                            r.raw, "read", total=total_length, desc=""
-                        ) as raw:
-                            # Save the output
-                            with open(input_vm_path, "wb") as output:
-                                shutil.copyfileobj(raw, output)
+                    download_file(vm_input_url, input_vm_path)
 
                 checksum_type = vm_input_checksum["type"]
                 checksum_value = vm_input_checksum["value"]
                 calculated_checksum = hashsum(input_vm_path, algorithm=checksum_type)
                 if not calculated_checksum:
                     print("Failed to calculate the checksum of the downloaded image")
                     exit(CHECKSUM_ERROR)
@@ -328,66 +335,57 @@
                 if not exists(vm_input):
                     print(
                         PATH_NOT_FOUND_ERROR_MSG.format(
                             vm_input, "the defined input path to the does not exist"
                         )
                     )
                     exit(PATH_NOT_FOUND_ERROR)
-            convert_action = [
-                "convert",
-                "-f",
-                vm_input_format,
-                "-O",
-                vm_output_format,
+
+            converted_result, msg = convert_image(
                 input_vm_path,
                 vm_output_path,
-            ]
-            disc_action.extend(convert_action)
+                input_format=vm_input_format,
+                output_format=vm_output_format,
+            )
+            if not converted_result:
+                print(msg)
+                exit(converted_result)
+
+            # Resize the vm disk image
+            resized_result, resized_msg = resize_image(vm_output_path, vm_size)
+            if not resized_result:
+                print(resized_msg)
+                exit(resized_result)
         else:
             # If no input is specified, then we assume that we are creating a new disc image
-            new_action = ["create", "-f", vm_output_format, vm_output_path, vm_size]
-            disc_action.extend(new_action)
-
-        disc_action_result = run(disc_action)
-        if disc_action_result["returncode"] != 0:
-            print(
-                PATH_CREATE_ERROR_MSG.format(
-                    vm_output_path, disc_action_result["error"]
-                )
+            create_image_result, msg = create_image(
+                vm_input, vm_version, vm_size, image_format=vm_output_format
             )
-            exit(PATH_CREATE_ERROR)
-        else:
-            if verbose:
-                print(
-                    "Created VM disk image at: {}".format(
-                        os.path.abspath(vm_output_path)
+            if not create_image_result:
+                print(msg)
+                exit(create_image_result)
+            else:
+                if verbose:
+                    print(
+                        "Generated image at: {}".format(os.path.abspath(vm_output_path))
                     )
-                )
 
+        # TODO, check if the image in question is a rhel9 based image
         # Amend to qcow2 version 3 which is required in RHEL 9
         amend_command = ["qemu-img", "amend", "-o", "compat=v3", vm_output_path]
-        amended_result = run(amend_command)
-        if amended_result["returncode"] != 0:
+        amended_result = run(amend_command, format_output_str=True)
+        if amended_result["returncode"] != "0":
             print(PATH_CREATE_ERROR_MSG.format(vm_output_path, amended_result["error"]))
 
-        # Resize the vm disk image
-        resize_command = ["qemu-img", "resize", vm_output_path, vm_size]
-        resize_result = run(resize_command)
-        if resize_result["returncode"] != 0:
-            print(
-                "Failed to resize the downloaded image: {}".format(
-                    resize_result["error"]
-                )
-            )
-
-        # Check that the vm disk is consistent
-        check_command = ["qemu-img", "check", "-f", vm_output_format, vm_output_path]
-        check_result = run(check_command)
-        if check_result["returncode"] != 0:
-            print("The check of the vm disk failed: {}".format(check_result["error"]))
+        check_result, check_msg = check_image(
+            vm_output_path, image_format=vm_output_format
+        )
+        if not check_result:
+            print(check_msg)
+            exit(check_result)
 
 
 def cli():
     parser = argparse.ArgumentParser(
         prog=PACKAGE_NAME, formatter_class=argparse.ArgumentDefaultsHelpFormatter
     )
     parser.add_argument(
```

### Comparing `gen_vm_image-0.0.1a0/gen_vm_image/utils/io.py` & `gen_vm_image-0.0.1a1/gen_vm_image/utils/io.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,14 +111,15 @@
 
 # Read chunks of a file, default to 64KB
 def hashsum(path, algorithm="sha1", buffer_size=65536):
     try:
         import hashlib
 
         hash_algorithm = hashlib.new(algorithm)
+
         with open(path, "rb") as fh:
             for chunk in iter(lambda: fh.read(buffer_size), b""):
                 hash_algorithm.update(chunk)
         return hash_algorithm.hexdigest()
     except Exception as err:
         print("Failed to calculate hashsum: {} - {}".format(path, err))
     return False
```

### Comparing `gen_vm_image-0.0.1a0/gen_vm_image/utils/job.py` & `gen_vm_image-0.0.1a1/gen_vm_image/utils/job.py`

 * *Files identical despite different names*

### Comparing `gen_vm_image-0.0.1a0/gen_vm_image/utils/user.py` & `gen_vm_image-0.0.1a1/gen_vm_image/utils/user.py`

 * *Files identical despite different names*

### Comparing `gen_vm_image-0.0.1a0/gen_vm_image.egg-info/PKG-INFO` & `gen_vm_image-0.0.1a1/gen_vm_image.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen-vm-image
-Version: 0.0.1a0
+Version: 0.0.1a1
 Summary: This tool can be used for generating virtual machine images.
 Home-page: https://github.com/ucphhpc/gen-vm-image
 Author: Rasmus Munk
 Author-email: munk1@live.dk
 License: MIT
 Keywords: Virtual Machine,VM,Images
 Classifier: Intended Audience :: Developers
@@ -29,15 +29,15 @@
 Requires-Dist: docutils==0.18.1; extra == "dev"
 Requires-Dist: flake8==6.0.0; extra == "dev"
 
 ============
 gen-vm-image
 ============
 
-This package can be used for generating and configuring virtual machine images.
+This package can be used for generating virtual machine images.
 
 ------------
 Dependencies
 ------------
 
 The dependencies required to use this package to generate virtual machine images
 can be found in the ``dep`` directory for the supported distributions.
@@ -93,19 +93,19 @@
                                  [--generate-gocd-config]
                                  [--gocd-config-name GOCD_CONFIG_NAME]
                                  [--gocd-build-branch GOCD_BUILD_BRANCH]
 
         optional arguments:
         -h, --help            show this help message and exit
         --architecture-path ARCHITECTURE_PATH
-                                The path to the architecture file that is used to configure the images to be built (default: architecture.yml)
+                                The path to the architecture file that is used to build images (default: architecture.yml)
         --image-output-path IMAGE_OUTPUT_PATH
                                 The output path of the built image (default: generated-images/image.qcow2)
         --generated-image-owner GENERATED_IMAGE_OWNER
-                                Set the uid owner of the configured image (default: qemu)
+                                Set the uid owner of the built image (default: qemu)
         --generate-gocd-config
                                 Generate a GoCD config based on the architecture file (default: False)
         --gocd-config-name GOCD_CONFIG_NAME
                                 Name of the generated gocd config file (default: 1.gocd.yml)
         --gocd-build-branch GOCD_BUILD_BRANCH
                                 The branch that GoCD should use to build images (default: main)
```

### Comparing `gen_vm_image-0.0.1a0/gen_vm_image.egg-info/SOURCES.txt` & `gen_vm_image-0.0.1a1/gen_vm_image.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -12,10 +12,11 @@
 gen_vm_image/cli/build_image.py
 gen_vm_image/common/__init__.py
 gen_vm_image/common/defaults.py
 gen_vm_image/common/errors.py
 gen_vm_image/utils/__init__.py
 gen_vm_image/utils/io.py
 gen_vm_image/utils/job.py
+gen_vm_image/utils/net.py
 gen_vm_image/utils/user.py
 tests/test_image_architecture.py
 tests/test_image_build.py
```

### Comparing `gen_vm_image-0.0.1a0/setup.py` & `gen_vm_image-0.0.1a1/setup.py`

 * *Files identical despite different names*

### Comparing `gen_vm_image-0.0.1a0/tests/test_image_architecture.py` & `gen_vm_image-0.0.1a1/tests/test_image_architecture.py`

 * *Files identical despite different names*

### Comparing `gen_vm_image-0.0.1a0/tests/test_image_build.py` & `gen_vm_image-0.0.1a1/tests/test_image_build.py`

 * *Files identical despite different names*

