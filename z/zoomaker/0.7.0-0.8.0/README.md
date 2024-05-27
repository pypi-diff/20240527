# Comparing `tmp/zoomaker-0.7.0.tar.gz` & `tmp/zoomaker-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zoomaker-0.7.0.tar", max compression
+gzip compressed data, was "zoomaker-0.8.0.tar", max compression
```

## Comparing `zoomaker-0.7.0.tar` & `zoomaker-0.8.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     7265 2023-06-01 06:47:52.245774 zoomaker-0.7.0/README.md
--rw-r--r--   0        0        0      587 2023-06-01 08:47:31.698214 zoomaker-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     8056 2023-06-01 08:47:27.180009 zoomaker-0.7.0/zoomaker.py
--rw-r--r--   0        0        0     7972 1970-01-01 00:00:00.000000 zoomaker-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     6370 2024-05-27 11:52:22.984041 zoomaker-0.8.0/README.md
+-rw-r--r--   0        0        0      587 2024-05-27 11:52:22.984292 zoomaker-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     8622 2024-05-27 11:52:22.984818 zoomaker-0.8.0/zoomaker.py
+-rw-r--r--   0        0        0     7077 1970-01-01 00:00:00.000000 zoomaker-0.8.0/PKG-INFO
```

### Comparing `zoomaker-0.7.0/README.md` & `zoomaker-0.8.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -4,22 +4,21 @@
 ========
 
 Zoomaker is a command-line tool that helps install AI models, git repositories and run scripts.
 
 - **single source of truth**: all resources are neatly defined in the `zoo.yaml` file
 - **freeze versions**: know exactly which revision of a resources is installed at any time
 - **only download once**: optimize bandwidth and cache your models locally
-- **optimize disk usage**: downloaded models are symlinked to the installation folder (small files <5MB are duplicate)
+- **optimize disk usage**: downloaded models are cached
 
 ## 😻 TL;DR
 
 1. Install Zoomaker `pip install zoomaker`
 2. Define your resources in the `zoo.yaml` file
 3. Run `zoomaker install` to install them
-(on Windows: `zoomaker install --no-symlinks`, see [hints](https://github.com/hfg-gmuend/zoomaker#%EF%B8%8F-limitations-on-windows) below)
 
 
 ## 📦 Installation
 
 ```bash
 pip install zoomaker
 ```
@@ -117,15 +116,15 @@
 ```
 
 ```yaml
 scripts:
   start_webui: |
     conda activate automatic1111
     cd /home/$(whoami)/stable-diffusion-webui/
-    ./webui.sh --theme dark --xformers --no-half
+    ./webui.sh --xformers --no-half
 ```
 </details>
 
 <details>
 <summary>`zoo.yaml` with web download</summary>
 
 ```yaml
@@ -134,15 +133,15 @@
     - name: analog-diffusion-v1
       src: https://civitai.com/api/download/models/1344
       type: download
       install_to: ./stable-diffusion-webui/models/Stable-diffusion/
       rename_to: analog-diffusion-v1.safetensors
 ```
 Please note:
-The resource `type: download` can be seen as the last resort. Currently there is no caching or symlinking of web downloads. Recommended to avoid it :)
+The resource `type: download` can be seen as the last resort. Existing web downloads are skipped, but no other caching. It is recommended to avoid web downloads :)
 </details>
 
 ## 🧮 zoo.yaml Structure
 
 <details>
 <summary>Top level:</summary>
 
@@ -167,29 +166,27 @@
 
 | Command                | Action                                           |
 | :--------------------- | :----------------------------------------------- |
 | `zoomaker install`          | Installs resources as defined in `zoo.yaml` |
 | `zoomaker run <script_name>`    | Run CLI scripts as defined in `zoo.yaml` |
 | `zoomaker --help` | Get help using the Zoomaker CLI                     |
 | `zoomaker --version` | Show current Zoomaker version                     |
-| `zoomaker --no-symlinks` | Do not use symlinks for installing resources  |
 
-## ⚠️ Limitations on Windows
-Symlinks are not widely supported on Windows, which limits the caching mechanism used by Zoomaker. To work around this limitation, you can disable symlinks by using the `--no-symlinks` flag with the install command:
 
-```bash
-zoomaker install --no-symlinks
-```
-
-This will still use the cache directory for checking if files are already cached, but if not, they will be downloaded and duplicated directly to the installation directory, saving bandwidth but increasing disk usage. Alternatively, you can use the [Windows Subsystem for Linux "WSL"](https://docs.microsoft.com/en-us/windows/wsl/install-win10) (don't forget to [enable developer mode](https://docs.microsoft.com/en-us/windows/apps/get-started/enable-your-device-for-development)) or run Zoomaker as an administrator to enable symlink support on Windows.
-
-## 🤗 Hugging Face Access Token
+## 🤗 Hugging Face Access Token and Custom Cache Location
 
 You might be asked for a [Hugging Face Access Token](https://huggingface.co/docs/hub/security-tokens) during `zoomaker install`. Some resources on Hugging Face require accepting the terms of use of the model. You can set your access token by running this command in a terminal. The command `huggingface-cli` is automatically shipped alongside zoomaker.
 
 ```bash
 huggingface-cli login
 ```
 
+You can specify a custom cache location by setting the HF_HOME environment variable. The default cache location is `~/.cache/huggingface/`.
+
+```bash
+export HF_HOME=/path/to/your/cache
+zoomaker install
+```
+
 ## 🙏 Acknowledgements
 - Most of the internal heavy lifting is done be the [huggingface_hub library](https://huggingface.co/docs/huggingface_hub/guides/download) by Hugging Face. Thanks!
 - "Zoomaker Safari Hacker Cat" cover image by Alia Tasler, based on this [OpenMoji](https://openmoji.org/library/emoji-1F431-200D-1F4BB/). Thanks!
```

### Comparing `zoomaker-0.7.0/pyproject.toml` & `zoomaker-0.8.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "zoomaker"
-version = "0.7.0"
+version = "0.8.0"
 description = "Zoomaker - Friendly house keeping for your AI model zoo and related resources."
 authors = ["Benedikt Groß"]
 readme = "README.md"
 homepage = "https://github.com/hfg-gmuend/zoomaker"
 documentation = "https://github.com/hfg-gmuend/zoomaker"
 repository = "https://github.com/hfg-gmuend/zoomaker"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-huggingface-hub = "^0.14.0"
-GitPython = "^3.1.31"
+huggingface-hub = "^0.23.0"
+GitPython = "^3.1.43"
 
 [tool.poetry.scripts]
 zoomaker = 'zoomaker:main'
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `zoomaker-0.7.0/PKG-INFO` & `zoomaker-0.8.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,41 @@
 Metadata-Version: 2.1
 Name: zoomaker
-Version: 0.7.0
+Version: 0.8.0
 Summary: Zoomaker - Friendly house keeping for your AI model zoo and related resources.
 Home-page: https://github.com/hfg-gmuend/zoomaker
 Author: Benedikt Groß
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: GitPython (>=3.1.31,<4.0.0)
-Requires-Dist: huggingface-hub (>=0.14.0,<0.15.0)
+Requires-Dist: GitPython (>=3.1.43,<4.0.0)
+Requires-Dist: huggingface-hub (>=0.23.0,<0.24.0)
 Project-URL: Documentation, https://github.com/hfg-gmuend/zoomaker
 Project-URL: Repository, https://github.com/hfg-gmuend/zoomaker
 Description-Content-Type: text/markdown
 
 ![zoomaker_social_keyvisual](https://github.com/hfg-gmuend/zoomaker/assets/480224/75d3d492-fe54-4711-afbf-02768bbb4033)
 
 Zoomaker - Friendly house keeping for your AI model zoo and related resources.
 ========
 
 Zoomaker is a command-line tool that helps install AI models, git repositories and run scripts.
 
 - **single source of truth**: all resources are neatly defined in the `zoo.yaml` file
 - **freeze versions**: know exactly which revision of a resources is installed at any time
 - **only download once**: optimize bandwidth and cache your models locally
-- **optimize disk usage**: downloaded models are symlinked to the installation folder (small files <5MB are duplicate)
+- **optimize disk usage**: downloaded models are cached
 
 ## 😻 TL;DR
 
 1. Install Zoomaker `pip install zoomaker`
 2. Define your resources in the `zoo.yaml` file
 3. Run `zoomaker install` to install them
-(on Windows: `zoomaker install --no-symlinks`, see [hints](https://github.com/hfg-gmuend/zoomaker#%EF%B8%8F-limitations-on-windows) below)
 
 
 ## 📦 Installation
 
 ```bash
 pip install zoomaker
 ```
@@ -134,15 +133,15 @@
 ```
 
 ```yaml
 scripts:
   start_webui: |
     conda activate automatic1111
     cd /home/$(whoami)/stable-diffusion-webui/
-    ./webui.sh --theme dark --xformers --no-half
+    ./webui.sh --xformers --no-half
 ```
 </details>
 
 <details>
 <summary>`zoo.yaml` with web download</summary>
 
 ```yaml
@@ -151,15 +150,15 @@
     - name: analog-diffusion-v1
       src: https://civitai.com/api/download/models/1344
       type: download
       install_to: ./stable-diffusion-webui/models/Stable-diffusion/
       rename_to: analog-diffusion-v1.safetensors
 ```
 Please note:
-The resource `type: download` can be seen as the last resort. Currently there is no caching or symlinking of web downloads. Recommended to avoid it :)
+The resource `type: download` can be seen as the last resort. Existing web downloads are skipped, but no other caching. It is recommended to avoid web downloads :)
 </details>
 
 ## 🧮 zoo.yaml Structure
 
 <details>
 <summary>Top level:</summary>
 
@@ -184,30 +183,28 @@
 
 | Command                | Action                                           |
 | :--------------------- | :----------------------------------------------- |
 | `zoomaker install`          | Installs resources as defined in `zoo.yaml` |
 | `zoomaker run <script_name>`    | Run CLI scripts as defined in `zoo.yaml` |
 | `zoomaker --help` | Get help using the Zoomaker CLI                     |
 | `zoomaker --version` | Show current Zoomaker version                     |
-| `zoomaker --no-symlinks` | Do not use symlinks for installing resources  |
 
-## ⚠️ Limitations on Windows
-Symlinks are not widely supported on Windows, which limits the caching mechanism used by Zoomaker. To work around this limitation, you can disable symlinks by using the `--no-symlinks` flag with the install command:
 
-```bash
-zoomaker install --no-symlinks
-```
-
-This will still use the cache directory for checking if files are already cached, but if not, they will be downloaded and duplicated directly to the installation directory, saving bandwidth but increasing disk usage. Alternatively, you can use the [Windows Subsystem for Linux "WSL"](https://docs.microsoft.com/en-us/windows/wsl/install-win10) (don't forget to [enable developer mode](https://docs.microsoft.com/en-us/windows/apps/get-started/enable-your-device-for-development)) or run Zoomaker as an administrator to enable symlink support on Windows.
-
-## 🤗 Hugging Face Access Token
+## 🤗 Hugging Face Access Token and Custom Cache Location
 
 You might be asked for a [Hugging Face Access Token](https://huggingface.co/docs/hub/security-tokens) during `zoomaker install`. Some resources on Hugging Face require accepting the terms of use of the model. You can set your access token by running this command in a terminal. The command `huggingface-cli` is automatically shipped alongside zoomaker.
 
 ```bash
 huggingface-cli login
 ```
 
+You can specify a custom cache location by setting the HF_HOME environment variable. The default cache location is `~/.cache/huggingface/`.
+
+```bash
+export HF_HOME=/path/to/your/cache
+zoomaker install
+```
+
 ## 🙏 Acknowledgements
 - Most of the internal heavy lifting is done be the [huggingface_hub library](https://huggingface.co/docs/huggingface_hub/guides/download) by Hugging Face. Thanks!
 - "Zoomaker Safari Hacker Cat" cover image by Alia Tasler, based on this [OpenMoji](https://openmoji.org/library/emoji-1F431-200D-1F4BB/). Thanks!
```

