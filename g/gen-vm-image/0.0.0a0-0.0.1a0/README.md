# Comparing `tmp/gen-vm-image-0.0.0a0.tar.gz` & `tmp/gen_vm_image-0.0.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gen-vm-image-0.0.0a0.tar", last modified: Thu Apr 11 11:02:57 2024, max compression
+gzip compressed data, was "gen_vm_image-0.0.1a0.tar", last modified: Mon May 27 15:30:39 2024, max compression
```

## Comparing `gen-vm-image-0.0.0a0.tar` & `gen_vm_image-0.0.1a0.tar`

### file list

```diff
@@ -1,26 +1,30 @@
-drwxr-xr-x   0 rasmunk   (1001) wheel       (10)        0 2024-04-11 11:02:57.898384 gen-vm-image-0.0.0a0/
--rw-r--r--   0 rasmunk   (1001) wheel       (10)     8965 2024-04-11 11:02:57.898384 gen-vm-image-0.0.0a0/PKG-INFO
--rw-r--r--   0 rasmunk   (1001) wheel       (10)     7968 2024-04-11 11:00:32.000000 gen-vm-image-0.0.0a0/README.rst
-drwxr-xr-x   0 rasmunk   (1001) wheel       (10)        0 2024-04-11 11:02:57.898384 gen-vm-image-0.0.0a0/gen_vm_image.egg-info/
--rw-r--r--   0 rasmunk   (1001) wheel       (10)     8965 2024-04-11 11:02:57.000000 gen-vm-image-0.0.0a0/gen_vm_image.egg-info/PKG-INFO
--rw-r--r--   0 rasmunk   (1001) wheel       (10)      442 2024-04-11 11:02:57.000000 gen-vm-image-0.0.0a0/gen_vm_image.egg-info/SOURCES.txt
--rw-r--r--   0 rasmunk   (1001) wheel       (10)        1 2024-04-11 11:02:57.000000 gen-vm-image-0.0.0a0/gen_vm_image.egg-info/dependency_links.txt
--rw-r--r--   0 rasmunk   (1001) wheel       (10)      134 2024-04-11 11:02:57.000000 gen-vm-image-0.0.0a0/gen_vm_image.egg-info/entry_points.txt
--rw-r--r--   0 rasmunk   (1001) wheel       (10)      109 2024-04-11 11:02:57.000000 gen-vm-image-0.0.0a0/gen_vm_image.egg-info/requires.txt
--rw-r--r--   0 rasmunk   (1001) wheel       (10)        4 2024-04-11 11:02:57.000000 gen-vm-image-0.0.0a0/gen_vm_image.egg-info/top_level.txt
--rw-r--r--   0 rasmunk   (1001) wheel       (10)       38 2024-04-11 11:02:57.898384 gen-vm-image-0.0.0a0/setup.cfg
--rw-r--r--   0 rasmunk   (1001) wheel       (10)     1713 2024-04-11 11:02:51.000000 gen-vm-image-0.0.0a0/setup.py
-drwxr-xr-x   0 rasmunk   (1001) wheel       (10)        0 2024-04-11 11:02:57.897384 gen-vm-image-0.0.0a0/src/
--rw-r--r--   0 rasmunk   (1001) wheel       (10)        0 2024-04-11 09:44:00.000000 gen-vm-image-0.0.0a0/src/__init__.py
-drwxr-xr-x   0 rasmunk   (1001) wheel       (10)        0 2024-04-11 11:02:57.897384 gen-vm-image-0.0.0a0/src/cli/
--rw-r--r--   0 rasmunk   (1001) wheel       (10)        0 2024-04-11 09:44:00.000000 gen-vm-image-0.0.0a0/src/cli/__init__.py
--rw-r--r--   0 rasmunk   (1001) wheel       (10)    11716 2024-04-11 09:44:00.000000 gen-vm-image-0.0.0a0/src/cli/build_image.py
--rw-r--r--   0 rasmunk   (1001) wheel       (10)     9123 2024-04-11 09:44:00.000000 gen-vm-image-0.0.0a0/src/cli/configure_image.py
-drwxr-xr-x   0 rasmunk   (1001) wheel       (10)        0 2024-04-11 11:02:57.897384 gen-vm-image-0.0.0a0/src/common/
--rw-r--r--   0 rasmunk   (1001) wheel       (10)        0 2024-04-11 09:44:00.000000 gen-vm-image-0.0.0a0/src/common/__init__.py
--rw-r--r--   0 rasmunk   (1001) wheel       (10)      362 2024-04-11 09:44:00.000000 gen-vm-image-0.0.0a0/src/common/defaults.py
-drwxr-xr-x   0 rasmunk   (1001) wheel       (10)        0 2024-04-11 11:02:57.897384 gen-vm-image-0.0.0a0/src/utils/
--rw-r--r--   0 rasmunk   (1001) wheel       (10)        0 2024-04-11 09:44:00.000000 gen-vm-image-0.0.0a0/src/utils/__init__.py
--rw-r--r--   0 rasmunk   (1001) wheel       (10)     3642 2024-04-11 09:44:00.000000 gen-vm-image-0.0.0a0/src/utils/io.py
--rw-r--r--   0 rasmunk   (1001) wheel       (10)     1623 2024-04-11 09:44:00.000000 gen-vm-image-0.0.0a0/src/utils/job.py
--rw-r--r--   0 rasmunk   (1001) wheel       (10)      434 2024-04-11 09:44:00.000000 gen-vm-image-0.0.0a0/src/utils/user.py
+drwxr-sr-x   0 go        (1000) root         (0)        0 2024-05-27 15:30:39.873492 gen_vm_image-0.0.1a0/
+-rw-r--r--   0 go        (1000) root         (0)     5432 2024-05-27 15:30:39.873492 gen_vm_image-0.0.1a0/PKG-INFO
+-rw-r--r--   0 go        (1000) root         (0)     4365 2024-05-27 15:30:25.000000 gen_vm_image-0.0.1a0/README.rst
+drwxr-sr-x   0 go        (1000) root         (0)        0 2024-05-27 15:30:39.870492 gen_vm_image-0.0.1a0/gen_vm_image/
+-rw-r--r--   0 go        (1000) root         (0)        0 2024-05-27 15:30:25.000000 gen_vm_image-0.0.1a0/gen_vm_image/__init__.py
+-rw-r--r--   0 go        (1000) root         (0)     1557 2024-05-27 15:30:25.000000 gen_vm_image-0.0.1a0/gen_vm_image/architecture.py
+drwxr-sr-x   0 go        (1000) root         (0)        0 2024-05-27 15:30:39.871492 gen_vm_image-0.0.1a0/gen_vm_image/cli/
+-rw-r--r--   0 go        (1000) root         (0)        0 2024-05-27 15:30:25.000000 gen_vm_image-0.0.1a0/gen_vm_image/cli/__init__.py
+-rw-r--r--   0 go        (1000) root         (0)    15925 2024-05-27 15:30:25.000000 gen_vm_image-0.0.1a0/gen_vm_image/cli/build_image.py
+drwxr-sr-x   0 go        (1000) root         (0)        0 2024-05-27 15:30:39.871492 gen_vm_image-0.0.1a0/gen_vm_image/common/
+-rw-r--r--   0 go        (1000) root         (0)        0 2024-05-27 15:30:25.000000 gen_vm_image-0.0.1a0/gen_vm_image/common/__init__.py
+-rw-r--r--   0 go        (1000) root         (0)      362 2024-05-27 15:30:25.000000 gen_vm_image-0.0.1a0/gen_vm_image/common/defaults.py
+-rw-r--r--   0 go        (1000) root         (0)      484 2024-05-27 15:30:25.000000 gen_vm_image-0.0.1a0/gen_vm_image/common/errors.py
+drwxr-sr-x   0 go        (1000) root         (0)        0 2024-05-27 15:30:39.872492 gen_vm_image-0.0.1a0/gen_vm_image/utils/
+-rw-r--r--   0 go        (1000) root         (0)        0 2024-05-27 15:30:25.000000 gen_vm_image-0.0.1a0/gen_vm_image/utils/__init__.py
+-rw-r--r--   0 go        (1000) root         (0)     3938 2024-05-27 15:30:25.000000 gen_vm_image-0.0.1a0/gen_vm_image/utils/io.py
+-rw-r--r--   0 go        (1000) root         (0)     1623 2024-05-27 15:30:25.000000 gen_vm_image-0.0.1a0/gen_vm_image/utils/job.py
+-rw-r--r--   0 go        (1000) root         (0)      759 2024-05-27 15:30:25.000000 gen_vm_image-0.0.1a0/gen_vm_image/utils/user.py
+drwxr-sr-x   0 go        (1000) root         (0)        0 2024-05-27 15:30:39.872492 gen_vm_image-0.0.1a0/gen_vm_image.egg-info/
+-rw-r--r--   0 go        (1000) root         (0)     5432 2024-05-27 15:30:39.000000 gen_vm_image-0.0.1a0/gen_vm_image.egg-info/PKG-INFO
+-rw-r--r--   0 go        (1000) root         (0)      614 2024-05-27 15:30:39.000000 gen_vm_image-0.0.1a0/gen_vm_image.egg-info/SOURCES.txt
+-rw-r--r--   0 go        (1000) root         (0)        1 2024-05-27 15:30:39.000000 gen_vm_image-0.0.1a0/gen_vm_image.egg-info/dependency_links.txt
+-rw-r--r--   0 go        (1000) root         (0)       66 2024-05-27 15:30:39.000000 gen_vm_image-0.0.1a0/gen_vm_image.egg-info/entry_points.txt
+-rw-r--r--   0 go        (1000) root         (0)      109 2024-05-27 15:30:39.000000 gen_vm_image-0.0.1a0/gen_vm_image.egg-info/requires.txt
+-rw-r--r--   0 go        (1000) root         (0)       13 2024-05-27 15:30:39.000000 gen_vm_image-0.0.1a0/gen_vm_image.egg-info/top_level.txt
+-rw-r--r--   0 go        (1000) root         (0)       38 2024-05-27 15:30:39.873492 gen_vm_image-0.0.1a0/setup.cfg
+-rw-r--r--   0 go        (1000) root         (0)     1690 2024-05-27 15:30:25.000000 gen_vm_image-0.0.1a0/setup.py
+drwxr-sr-x   0 go        (1000) root         (0)        0 2024-05-27 15:30:39.872492 gen_vm_image-0.0.1a0/tests/
+-rw-r--r--   0 go        (1000) root         (0)     3324 2024-05-27 15:30:25.000000 gen_vm_image-0.0.1a0/tests/test_image_architecture.py
+-rw-r--r--   0 go        (1000) root         (0)     2781 2024-05-27 15:30:25.000000 gen_vm_image-0.0.1a0/tests/test_image_build.py
```

### Comparing `gen-vm-image-0.0.0a0/setup.py` & `gen_vm_image-0.0.1a0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     exec(f.read(), {}, version_ns)
 
 
 long_description = open("README.rst").read()
 setup(
     name="gen-vm-image",
     version=version_ns["__version__"],
-    description="",
+    description="This tool can be used for generating virtual machine images.",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     author="Rasmus Munk",
     author_email="munk1@live.dk",
     packages=find_packages(),
     url="https://github.com/ucphhpc/gen-vm-image",
     license="MIT",
@@ -37,16 +37,15 @@
     install_requires=read_req("requirements.txt"),
     extras_require={
         "test": read_req("tests/requirements.txt"),
         "dev": read_req("requirements-dev.txt"),
     },
     entry_points={
         "console_scripts": [
-            "gen-vm-image = src.cli.build_image:run_build_image",
-            "configure-vm-image = src.cli.configure_image:run_configure_image",
+            "gen-vm-image = gen_vm_image.cli.build_image:cli",
         ]
     },
     classifiers=[
         "Intended Audience :: Developers",
         "Intended Audience :: System Administrators",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.8",
```

### Comparing `gen-vm-image-0.0.0a0/src/cli/build_image.py` & `gen_vm_image-0.0.1a0/gen_vm_image/cli/build_image.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,37 @@
 import argparse
 import os
 import yaml
 import requests
 import shutil
 from tqdm.auto import tqdm
-from src.common.defaults import (
+from gen_vm_image.common.defaults import (
     GOCD_GROUP,
     GOCD_TEMPLATE,
     REPO_NAME,
     PACKAGE_NAME,
     GENERATED_IMAGE_DIR,
     TMP_DIR,
     GOCD_FORMAT_VERSION,
     GO_REVISION_COMMIT_VAR,
 )
-from src.utils.io import load, exists, makedirs, write, chown, hashsum
-from src.utils.user import lookup_uid, lookup_gid
-from src.utils.job import run
+from gen_vm_image.common.errors import (
+    PATH_NOT_FOUND_ERROR,
+    PATH_NOT_FOUND_ERROR_MSG,
+    PATH_CREATE_ERROR,
+    PATH_CREATE_ERROR_MSG,
+    MISSING_ATTRIBUTE_ERROR,
+    MISSING_ATTRIBUTE_ERROR_MSG,
+    INVALID_ATTRIBUTE_TYPE_ERROR,
+    INVALID_ATTRIBUTE_TYPE_ERROR_MSG,
+    CHECKSUM_ERROR,
+)
+from gen_vm_image.architecture import load_architecture, correct_architecture_structure
+from gen_vm_image.utils.io import exists, makedirs, write, hashsum
+from gen_vm_image.utils.job import run
 
 
 current_dir = os.path.abspath(os.path.dirname(__file__))
 parent_dir = os.path.dirname(current_dir)
 
 
 def get_pipelines(images):
@@ -86,256 +97,346 @@
     materials.update(common_materials)
     if upstream_pipeline and stage:
         upstream_materials = get_upstream_materials(name, upstream_pipeline, stage)
         materials.update(upstream_materials)
     return materials
 
 
-def run_build_image():
-    parser = argparse.ArgumentParser(
-        prog=PACKAGE_NAME, formatter_class=argparse.ArgumentDefaultsHelpFormatter
-    )
-    parser.add_argument(
-        "--architecture-path",
-        default="architecture.yml",
-        help="The path to the architecture file that is used to configure the images to be built",
-    )
-    parser.add_argument(
-        "--image-output-path",
-        default=os.path.join(GENERATED_IMAGE_DIR, "image.qcow2"),
-        help="The output path of the built image",
-    )
-    parser.add_argument(
-        "--generated-image-owner",
-        default="qemu",
-        help="Set the uid owner of the configured image",
-    )
-    parser.add_argument(
-        "--generate-gocd-config",
-        action="store_true",
-        help="Generate a GoCD config based on the architecture file",
-    )
-    parser.add_argument(
-        "--gocd-config-name",
-        default="1.gocd.yml",
-        help="Name of the generated gocd config file",
-    )
-    parser.add_argument(
-        "--gocd-build-branch",
-        default="main",
-        help="The branch that GoCD should use to build images",
-    )
-    args = parser.parse_args()
+def create_image(name, version, size, image_format="qcow2"):
+    image_name = "{}-{}.{}".format(name, version, image_format)
+    create_image_command = ["qemu-img", "create", "-f", image_format, image_name, size]
+    created_result = run(create_image_command, format_output_str=True)
+    if created_result["returncode"] != "0":
+        return PATH_CREATE_ERROR, PATH_CREATE_ERROR_MSG.format(
+            image_name, created_result["error"]
+        )
+    return created_result, None
 
-    architecture_path = args.architecture_path
-    image_output_path = args.image_output_path
-    generated_image_owner = args.generated_image_owner
-    generate_gocd_config = args.generate_gocd_config
-    gocd_config_name = args.gocd_config_name
-    gocd_build_branch = args.gocd_build_branch
 
-    image_output_dir = os.path.dirname(image_output_path)
-    temporary_image_dir = TMP_DIR
+def convert_image(input_path, output_path, input_format="qcow2", output_format="qcow2"):
+    convert_image_command = [
+        "qemu-img",
+        "convert",
+        "-f",
+        input_format,
+        "-O",
+        output_format,
+        input_path,
+        output_path,
+    ]
+    converted_result = run(convert_image_command, format_output_str=True)
+    if converted_result["returncode"] != "0":
+        return PATH_CREATE_ERROR, PATH_CREATE_ERROR_MSG.format(
+            input_path, converted_result["error"]
+        )
+    return converted_result, None
+
+
+def build_gocd_config(architecture, gocd_name, branch, verbose):
+    images = architecture.get("images", [])
+
+    # GOCD file
+    list_images = list(images.keys())
+
+    # Get all pipelines
+    pipelines = get_pipelines(list_images)
+
+    # GOCD environment
+    common_environments = get_common_environment(pipelines)
+
+    # Common GOCD pipeline params
+    common_pipeline_attributes = get_common_pipeline()
+
+    generated_config = {
+        "format_version": GOCD_FORMAT_VERSION,
+        **common_environments,
+        "pipelines": {},
+    }
+    # Generate the GOCD build config
+    for build, build_data in images.items():
+        name = build_data.get("name", None)
+        version = build_data.get("version", None)
+        materials = get_materials(name, branch=branch)
+
+        build_version_name = build
+        build_pipeline = {
+            **common_pipeline_attributes,
+            "materials": materials,
+            "parameters": {
+                "IMAGE": name,
+                "IMAGE_PIPELINE": build_version_name,
+                "DEFAULT_TAG": version,
+                "SRC_DIRECTORY": REPO_NAME,
+                "TEST_DIRECTORY": REPO_NAME,
+                "PUSH_DIRECTORY": "publish-docker-scripts",
+                "COMMIT_TAG": GO_REVISION_COMMIT_VAR,
+                "ARGS": "",
+            },
+        }
+        generated_config["pipelines"][build_version_name] = build_pipeline
 
+    gocd_config_path = os.path.join(current_dir, gocd_name)
+    if not write(gocd_config_path, generated_config, handler=yaml):
+        print(
+            PATH_CREATE_ERROR_MSG.format(gocd_config_path, "Failed to save gocd config")
+        )
+        exit(PATH_CREATE_ERROR)
+    if verbose:
+        print("Generated a new GOCD config in: {}".format(gocd_config_path))
+
+
+def build_architecture(architecture_path, images_output_directory, verbose):
     # Load the architecture file
-    architecture = load(architecture_path, handler=yaml, Loader=yaml.FullLoader)
-    if not architecture:
-        print("Failed to load architecture file: {}".format(architecture_path))
-        exit(-1)
-
-    owner = architecture.get("owner", None)
-    if not owner:
-        print("Failed to find architecture the owner in: {}".format(architecture_path))
-        exit(-1)
-
-    images = architecture.get("images", None)
-    if not images:
-        print("Failed to find 'images' in: {}".format(architecture_path))
-        exit(-1)
+    architecture, load_error_msg = load_architecture(architecture_path)
+    if load_error_msg:
+        print(load_error_msg)
+        exit(architecture)
+
+    correct_architecture, correct_error_msg = correct_architecture_structure(
+        architecture
+    )
+    if not correct_architecture:
+        print(correct_error_msg)
+        exit(correct_architecture)
+
+    # Create the destination directory where the images will be saved
+    if not exists(images_output_directory):
+        created, msg = makedirs(images_output_directory)
+        if not created:
+            print(PATH_CREATE_ERROR_MSG.format(images_output_directory, msg))
+            exit(PATH_CREATE_ERROR)
 
-    required_attributes = ["name", "version", "get_url", "checksum", "size"]
-    required_checksum_attributes = ["type", "value"]
+    images = architecture.get("images", [])
     # Generate the image configuration
     for build, build_data in images.items():
-        for attr in required_attributes:
-            if attr not in build_data:
-                print("Missing required attribute '{}': in {}".format(attr, build_data))
-                exit(-2)
+        # Base command used to either create or convert an image
+        disc_action = ["qemu-img"]
         vm_name = build_data["name"]
         vm_version = build_data["version"]
-        vm_image_url = build_data["get_url"]
         vm_size = build_data["size"]
 
-        vm_checksum = build_data["checksum"]
-        if not isinstance(vm_checksum, dict):
-            print("Invalid checksum format: {}".format(vm_checksum))
-            exit(-3)
-        for attr in required_checksum_attributes:
-            if attr not in vm_checksum:
+        # Optional attributes for each image configuration
+        vm_output_format = build_data.get("format", "qcow2")
+        vm_input, vm_input_format = None, "qcow2"
+        if "input" in build_data:
+            vm_input = build_data["input"]
+            if not isinstance(vm_input, str) and not isinstance(vm_input, dict):
                 print(
-                    "Missing required attribute '{}': in {}".format(attr, vm_checksum)
-                )
-                exit(-4)
-
-        # Prepare the temporary directory
-        # where the image will be prepared
-        if not exists(temporary_image_dir):
-            created, msg = makedirs(temporary_image_dir)
-            if not created:
-                print(
-                    "Failed to create temporary image directory: {} - {}".format(
-                        temporary_image_dir, msg
+                    INVALID_ATTRIBUTE_TYPE_ERROR_MSG.format(
+                        type(vm_input), vm_input, "string or dictionary"
                     )
                 )
+                exit(INVALID_ATTRIBUTE_TYPE_ERROR)
 
-        # Download the image and save it into
-        # a tmp directory
-        get_url_filename = vm_image_url.split("/")[-1]
-        get_url_path = os.path.join(temporary_image_dir, get_url_filename)
-        cloud_image = None
-        if not exists(get_url_path):
-            print("Downloading image from: {}".format(vm_image_url))
-            with requests.get(vm_image_url, stream=True) as r:
-                # check header to get content length, in bytes
-                total_length = int(r.headers.get("Content-Length"))
-                # implement progress bar via tqdm
-                with tqdm.wrapattr(r.raw, "read", total=total_length, desc="") as raw:
-                    # Save the output
-                    with open(get_url_path, "wb") as output:
-                        shutil.copyfileobj(raw, output)
-
-        checksum_type = vm_checksum["type"]
-        checksum_value = vm_checksum["value"]
-        calculated_checksum = hashsum(get_url_path, algorithm=checksum_type)
-        if not calculated_checksum:
-            print("Failed to calculate the checksum of the downloaded image")
-            exit(-5)
-
-        if calculated_checksum != checksum_value:
-            print(
-                "The checksum of the downloaded image does not match the expected checksum: {} != {}".format(
-                    calculated_checksum, checksum_value
-                )
-            )
-            exit(-6)
-        print(
-            "The calculated checksum: {} matches the defined checksum: {}".format(
-                calculated_checksum, checksum_value
-            )
+        vm_output_path = os.path.join(
+            images_output_directory,
+            "{}-{}.{}".format(vm_name, vm_version, vm_output_format),
         )
 
-        # Create an image based on the downloaded image
-        if not exists(image_output_dir):
-            created, msg = makedirs(image_output_dir)
-            if not created:
-                print(
-                    "Failed to create disk directory: {} - {}".format(
-                        image_output_dir, msg
+        if vm_input:
+            if isinstance(vm_input, dict):
+                if "url" not in vm_input:
+                    print(MISSING_ATTRIBUTE_ERROR_MSG.format("url", vm_input))
+                    exit(MISSING_ATTRIBUTE_ERROR)
+                if not isinstance(vm_input["url"], str):
+                    print(
+                        INVALID_ATTRIBUTE_TYPE_ERROR_MSG.format(
+                            type(vm_input["url"]), vm_input["url"], "string"
+                        )
                     )
-                )
+                    exit(INVALID_ATTRIBUTE_TYPE_ERROR)
 
-        create_disk_command = [
-            "qemu-img",
-            "convert",
-            "-f",
-            "qcow2",
-            "-O",
-            "qcow2",
-            get_url_path,
-            image_output_path,
-        ]
-        create_disk_result = run(create_disk_command)
-        if create_disk_result["returncode"] != 0:
+                if "checksum" not in vm_input:
+                    print(MISSING_ATTRIBUTE_ERROR_MSG.format("checksum", vm_input))
+                    exit(MISSING_ATTRIBUTE_ERROR)
+                if not isinstance(vm_input["checksum"], dict):
+                    print(
+                        INVALID_ATTRIBUTE_TYPE_ERROR_MSG.format(
+                            type(vm_input["checksum"]),
+                            vm_input["checksum"],
+                            "dictionary",
+                        )
+                    )
+                    exit(INVALID_ATTRIBUTE_TYPE_ERROR)
+                required_checksum_attributes = ["type", "value"]
+                for attr in required_checksum_attributes:
+                    if attr not in vm_input["checksum"]:
+                        print(
+                            MISSING_ATTRIBUTE_ERROR_MSG.format(
+                                attr, vm_input["checksum"]
+                            )
+                        )
+                        exit(MISSING_ATTRIBUTE_ERROR)
+                    if not isinstance(vm_input["checksum"][attr], str):
+                        print(
+                            INVALID_ATTRIBUTE_TYPE_ERROR_MSG.format(
+                                type(vm_input["checksum"][attr]),
+                                vm_input["checksum"][attr],
+                                "string",
+                            )
+                        )
+                        exit(INVALID_ATTRIBUTE_TYPE_ERROR)
+
+                vm_input_url = vm_input["url"]
+                vm_input_checksum = vm_input["checksum"]
+                # Download the specified Url and save it into
+                # a tmp directory.
+                # First prepare the temporary directory
+                # where the downloaded image will be prepared
+                if not exists(TMP_DIR):
+                    created, msg = makedirs(TMP_DIR)
+                    if not created:
+                        print(PATH_CREATE_ERROR_MSG.format(TMP_DIR, msg))
+                        exit(PATH_CREATE_ERROR)
+
+                input_url_filename = vm_input_url.split("/")[-1]
+                input_vm_path = os.path.join(TMP_DIR, input_url_filename)
+                if not exists(input_vm_path):
+                    if verbose:
+                        print("Downloading image from: {}".format(vm_input_url))
+                    with requests.get(vm_input_url, stream=True) as r:
+                        # check header to get content length, in bytes
+                        total_length = int(r.headers.get("Content-Length"))
+                        # implement progress bar via tqdm
+                        with tqdm.wrapattr(
+                            r.raw, "read", total=total_length, desc=""
+                        ) as raw:
+                            # Save the output
+                            with open(input_vm_path, "wb") as output:
+                                shutil.copyfileobj(raw, output)
+
+                checksum_type = vm_input_checksum["type"]
+                checksum_value = vm_input_checksum["value"]
+                calculated_checksum = hashsum(input_vm_path, algorithm=checksum_type)
+                if not calculated_checksum:
+                    print("Failed to calculate the checksum of the downloaded image")
+                    exit(CHECKSUM_ERROR)
+
+                if calculated_checksum != checksum_value:
+                    print(
+                        "The checksum of the downloaded image does not match the expected checksum: {} != {}".format(
+                            calculated_checksum, checksum_value
+                        )
+                    )
+                    exit(CHECKSUM_ERROR)
+                if verbose:
+                    print(
+                        "The calculated checksum: {} matches the defined checksum: {}".format(
+                            calculated_checksum, checksum_value
+                        )
+                    )
+            else:
+                if not exists(vm_input):
+                    print(
+                        PATH_NOT_FOUND_ERROR_MSG.format(
+                            vm_input, "the defined input path to the does not exist"
+                        )
+                    )
+                    exit(PATH_NOT_FOUND_ERROR)
+            convert_action = [
+                "convert",
+                "-f",
+                vm_input_format,
+                "-O",
+                vm_output_format,
+                input_vm_path,
+                vm_output_path,
+            ]
+            disc_action.extend(convert_action)
+        else:
+            # If no input is specified, then we assume that we are creating a new disc image
+            new_action = ["create", "-f", vm_output_format, vm_output_path, vm_size]
+            disc_action.extend(new_action)
+
+        disc_action_result = run(disc_action)
+        if disc_action_result["returncode"] != 0:
             print(
-                "Failed to create a VM disk: {} - {}".format(
-                    create_disk_result["error"], create_disk_result["returncode"]
+                PATH_CREATE_ERROR_MSG.format(
+                    vm_output_path, disc_action_result["error"]
                 )
             )
+            exit(PATH_CREATE_ERROR)
         else:
-            print(
-                "Created VM disk image at: {}".format(
-                    os.path.abspath(image_output_path)
+            if verbose:
+                print(
+                    "Created VM disk image at: {}".format(
+                        os.path.abspath(vm_output_path)
+                    )
                 )
-            )
 
         # Amend to qcow2 version 3 which is required in RHEL 9
-        amend_command = ["qemu-img", "amend", "-o", "compat=v3", image_output_path]
+        amend_command = ["qemu-img", "amend", "-o", "compat=v3", vm_output_path]
         amended_result = run(amend_command)
         if amended_result["returncode"] != 0:
-            print("Failed to amend a VM disk: {}".format(amended_result["error"]))
+            print(PATH_CREATE_ERROR_MSG.format(vm_output_path, amended_result["error"]))
 
         # Resize the vm disk image
-        resize_command = ["qemu-img", "resize", image_output_path, vm_size]
+        resize_command = ["qemu-img", "resize", vm_output_path, vm_size]
         resize_result = run(resize_command)
         if resize_result["returncode"] != 0:
             print(
                 "Failed to resize the downloaded image: {}".format(
                     resize_result["error"]
                 )
             )
 
         # Check that the vm disk is consistent
-        check_command = ["qemu-img", "check", "-f", "qcow2", image_output_path]
+        check_command = ["qemu-img", "check", "-f", vm_output_format, vm_output_path]
         check_result = run(check_command)
         if check_result["returncode"] != 0:
             print("The check of the vm disk failed: {}".format(check_result["error"]))
 
-        # Set the owner of the image
-        user_uid = lookup_uid(generated_image_owner)
-        user_gid = lookup_gid(generated_image_owner)
-        if user_uid and user_gid:
-            chown_result = chown(image_output_path, user_uid, user_gid)
-            if not chown_result[0]:
-                print(
-                    "Failed to set the owner of the image: {}".format(chown_result[1])
-                )
-
-    if generate_gocd_config:
-        # GOCD file
-        list_images = list(images.keys())
-
-        # Get all pipelines
-        pipelines = get_pipelines(list_images)
 
-        # GOCD environment
-        common_environments = get_common_environment(pipelines)
+def cli():
+    parser = argparse.ArgumentParser(
+        prog=PACKAGE_NAME, formatter_class=argparse.ArgumentDefaultsHelpFormatter
+    )
+    parser.add_argument(
+        "--architecture-path",
+        default="architecture.yml",
+        help="The path to the architecture file that defines the images to build",
+    )
+    parser.add_argument(
+        "--images-output-directory",
+        default=GENERATED_IMAGE_DIR,
+        help="The path to the output directory where the images will be saved",
+    )
+    parser.add_argument(
+        "--generate-gocd-config",
+        action="store_true",
+        help="Generate a GoCD config based on the architecture file",
+    )
+    parser.add_argument(
+        "--gocd-config-name",
+        default="1.gocd.yml",
+        help="Name of the generated gocd config file",
+    )
+    parser.add_argument(
+        "--gocd-build-branch",
+        default="main",
+        help="The branch that GoCD should use to build images",
+    )
+    parser.add_argument(
+        "--verbose",
+        "-v",
+        action="store_true",
+        help="Print verbose output",
+    )
+    args = parser.parse_args()
 
-        # Common GOCD pipeline params
-        common_pipeline_attributes = get_common_pipeline()
-
-        generated_config = {
-            "format_version": GOCD_FORMAT_VERSION,
-            **common_environments,
-            "pipelines": {},
-        }
-        # Generate the GOCD build config
-        for build, build_data in images.items():
-            name = build_data.get("name", None)
-            version = build_data.get("version", None)
-            materials = get_materials(name, branch=gocd_build_branch)
-
-            build_version_name = build
-            build_pipeline = {
-                **common_pipeline_attributes,
-                "materials": materials,
-                "parameters": {
-                    "IMAGE": name,
-                    "IMAGE_PIPELINE": build_version_name,
-                    "DEFAULT_TAG": version,
-                    "SRC_DIRECTORY": REPO_NAME,
-                    "TEST_DIRECTORY": REPO_NAME,
-                    "PUSH_DIRECTORY": "publish-docker-scripts",
-                    "COMMIT_TAG": GO_REVISION_COMMIT_VAR,
-                    "ARGS": "",
-                },
-            }
-            generated_config["pipelines"][build_version_name] = build_pipeline
+    architecture_path = args.architecture_path
+    images_output_directory = args.images_output_directory
+    generate_gocd_config = args.generate_gocd_config
+    gocd_config_name = args.gocd_config_name
+    gocd_build_branch = args.gocd_build_branch
+    verbose = args.verbose
 
-        gocd_config_path = os.path.join(current_dir, gocd_config_name)
-        if not write(gocd_config_path, generated_config, handler=yaml):
-            print("Failed to save config")
-            exit(-1)
-        print("Generated a new GOCD config in: {}".format(gocd_config_path))
+    build_architecture(architecture_path, images_output_directory, verbose)
+    if generate_gocd_config:
+        build_gocd_config(
+            architecture_path, gocd_config_name, gocd_build_branch, verbose
+        )
+    exit(0)
 
 
 if __name__ == "__main__":
-    run_build_image()
+    cli()
```

### Comparing `gen-vm-image-0.0.0a0/src/utils/io.py` & `gen_vm_image-0.0.1a0/gen_vm_image/utils/io.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import shutil
+import re
 
 
 def makedirs(path):
     try:
         os.makedirs(os.path.expanduser(path))
         return True, "Created: {}".format(path)
     except Exception as err:
@@ -65,14 +66,18 @@
     return False, "Failed to remove directory: {}".format(path)
 
 
 def exists(path):
     return os.path.exists(os.path.expanduser(path))
 
 
+def join(path, *paths):
+    return os.path.join(path, *paths)
+
+
 def which(command):
     return shutil.which(command)
 
 
 def chmod(path, mode, **kwargs):
     try:
         os.chmod(os.path.expanduser(path), mode, **kwargs)
@@ -113,7 +118,16 @@
         with open(path, "rb") as fh:
             for chunk in iter(lambda: fh.read(buffer_size), b""):
                 hash_algorithm.update(chunk)
         return hash_algorithm.hexdigest()
     except Exception as err:
         print("Failed to calculate hashsum: {} - {}".format(path, err))
     return False
+
+
+def find(directory_path, regex_name):
+    found = []
+    for root, dirs, files in os.walk(directory_path):
+        for f in files:
+            if re.match(regex_name, f):
+                found.append(f)
+    return found
```

### Comparing `gen-vm-image-0.0.0a0/src/utils/job.py` & `gen_vm_image-0.0.1a0/gen_vm_image/utils/job.py`

 * *Files identical despite different names*

