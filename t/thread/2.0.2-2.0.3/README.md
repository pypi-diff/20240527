# Comparing `tmp/thread-2.0.2.tar.gz` & `tmp/thread-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thread-2.0.2.tar", max compression
+gzip compressed data, was "thread-2.0.3.tar", max compression
```

## Comparing `thread-2.0.2.tar` & `thread-2.0.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1496 2024-05-25 13:15:28.335379 thread-2.0.2/LICENSE.txt
--rw-r--r--   0        0        0     4657 2024-05-25 13:15:28.335379 thread-2.0.2/README.md
--rw-r--r--   0        0        0     1685 2024-05-25 13:15:28.335379 thread-2.0.2/pyproject.toml
--rw-r--r--   0        0        0      675 2024-05-25 13:15:28.335379 thread-2.0.2/src/thread/__init__.py
--rw-r--r--   0        0        0      139 2024-05-25 13:15:28.335379 thread-2.0.2/src/thread/__main__.py
--rw-r--r--   0        0        0       33 2024-05-25 13:15:28.335379 thread-2.0.2/src/thread/__version__.py
--rw-r--r--   0        0        0     1470 2024-05-25 13:15:28.335379 thread-2.0.2/src/thread/_types.py
--rw-r--r--   0        0        0      272 2024-05-25 13:15:28.335379 thread-2.0.2/src/thread/cli.py
--rw-r--r--   0        0        0       93 2024-05-25 13:15:28.335379 thread-2.0.2/src/thread/decorators/__init__.py
--rw-r--r--   0        0        0     4794 2024-05-25 13:15:28.335379 thread-2.0.2/src/thread/decorators/_processor.py
--rw-r--r--   0        0        0     3837 2024-05-25 13:15:28.335379 thread-2.0.2/src/thread/decorators/_threaded.py
--rw-r--r--   0        0        0     2144 2024-05-25 13:15:28.335379 thread-2.0.2/src/thread/exceptions.py
--rw-r--r--   0        0        0        0 2024-05-25 13:15:28.335379 thread-2.0.2/src/thread/py.typed
--rw-r--r--   0        0        0    21956 2024-05-25 13:15:28.335379 thread-2.0.2/src/thread/thread.py
--rw-r--r--   0        0        0      123 2024-05-25 13:15:28.335379 thread-2.0.2/src/thread/utils/__init__.py
--rw-r--r--   0        0        0     1385 2024-05-25 13:15:28.335379 thread-2.0.2/src/thread/utils/algorithm.py
--rw-r--r--   0        0        0     4586 2024-05-25 13:15:28.335379 thread-2.0.2/src/thread/utils/config.py
--rw-r--r--   0        0        0      183 2024-05-25 13:15:28.335379 thread-2.0.2/src/thread/utils/meta.py
--rw-r--r--   0        0        0      101 2024-05-25 13:15:28.335379 thread-2.0.2/src/thread/version.py
--rw-r--r--   0        0        0       61 2024-05-25 13:15:28.335379 thread-2.0.2/tests/conftest.py
--rw-r--r--   0        0        0      280 2024-05-25 13:15:28.335379 thread-2.0.2/tests/library/test_version.py
--rw-r--r--   0        0        0     1232 2024-05-25 13:15:28.335379 thread-2.0.2/tests/test_algorithm.py
--rw-r--r--   0        0        0     1816 2024-05-25 13:15:28.335379 thread-2.0.2/tests/test_concurrentprocessing.py
--rw-r--r--   0        0        0     9467 2024-05-25 13:15:28.335379 thread-2.0.2/tests/test_dataframe_compatibility.py
--rw-r--r--   0        0        0     2114 2024-05-25 13:15:28.335379 thread-2.0.2/tests/test_decorator.py
--rw-r--r--   0        0        0     3405 2024-05-25 13:15:28.335379 thread-2.0.2/tests/test_thread.py
--rw-r--r--   0        0        0     1480 2024-05-25 13:15:28.335379 thread-2.0.2/tests/test_verbosity.py
--rw-r--r--   0        0        0     6111 1970-01-01 00:00:00.000000 thread-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1496 2024-05-27 02:45:46.620231 thread-2.0.3/LICENSE.txt
+-rw-r--r--   0        0        0     4833 2024-05-27 02:45:46.620231 thread-2.0.3/README.md
+-rw-r--r--   0        0        0     1701 2024-05-27 02:45:46.632231 thread-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0      675 2024-05-27 02:45:46.632231 thread-2.0.3/src/thread/__init__.py
+-rw-r--r--   0        0        0      139 2024-05-27 02:45:46.632231 thread-2.0.3/src/thread/__main__.py
+-rw-r--r--   0        0        0       33 2024-05-27 02:45:46.632231 thread-2.0.3/src/thread/__version__.py
+-rw-r--r--   0        0        0     1470 2024-05-27 02:45:46.632231 thread-2.0.3/src/thread/_types.py
+-rw-r--r--   0        0        0      272 2024-05-27 02:45:46.632231 thread-2.0.3/src/thread/cli.py
+-rw-r--r--   0        0        0       93 2024-05-27 02:45:46.632231 thread-2.0.3/src/thread/decorators/__init__.py
+-rw-r--r--   0        0        0     4782 2024-05-27 02:45:46.632231 thread-2.0.3/src/thread/decorators/_processor.py
+-rw-r--r--   0        0        0     3825 2024-05-27 02:45:46.632231 thread-2.0.3/src/thread/decorators/_threaded.py
+-rw-r--r--   0        0        0     2144 2024-05-27 02:45:46.632231 thread-2.0.3/src/thread/exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-27 02:45:46.632231 thread-2.0.3/src/thread/py.typed
+-rw-r--r--   0        0        0    21924 2024-05-27 02:45:46.632231 thread-2.0.3/src/thread/thread.py
+-rw-r--r--   0        0        0      123 2024-05-27 02:45:46.632231 thread-2.0.3/src/thread/utils/__init__.py
+-rw-r--r--   0        0        0     1385 2024-05-27 02:45:46.632231 thread-2.0.3/src/thread/utils/algorithm.py
+-rw-r--r--   0        0        0     4586 2024-05-27 02:45:46.632231 thread-2.0.3/src/thread/utils/config.py
+-rw-r--r--   0        0        0      183 2024-05-27 02:45:46.632231 thread-2.0.3/src/thread/utils/meta.py
+-rw-r--r--   0        0        0      101 2024-05-27 02:45:46.632231 thread-2.0.3/src/thread/version.py
+-rw-r--r--   0        0        0       61 2024-05-27 02:45:46.632231 thread-2.0.3/tests/conftest.py
+-rw-r--r--   0        0        0      280 2024-05-27 02:45:46.632231 thread-2.0.3/tests/library/test_version.py
+-rw-r--r--   0        0        0     1232 2024-05-27 02:45:46.632231 thread-2.0.3/tests/test_algorithm.py
+-rw-r--r--   0        0        0     1816 2024-05-27 02:45:46.632231 thread-2.0.3/tests/test_concurrentprocessing.py
+-rw-r--r--   0        0        0     9451 2024-05-27 02:45:46.632231 thread-2.0.3/tests/test_dataframe_compatibility.py
+-rw-r--r--   0        0        0     2114 2024-05-27 02:45:46.632231 thread-2.0.3/tests/test_decorator.py
+-rw-r--r--   0        0        0     3405 2024-05-27 02:45:46.632231 thread-2.0.3/tests/test_thread.py
+-rw-r--r--   0        0        0     1480 2024-05-27 02:45:46.632231 thread-2.0.3/tests/test_verbosity.py
+-rw-r--r--   0        0        0     6287 1970-01-01 00:00:00.000000 thread-2.0.3/PKG-INFO
```

### Comparing `thread-2.0.2/LICENSE.txt` & `thread-2.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `thread-2.0.2/README.md` & `thread-2.0.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,23 @@
-<a name="readme-top"></a>
+<!-- Allow HTML -->
+<!-- markdownlint-disable MD033 -->
 
+<!-- Allow HTML top-level heading -->
+<!-- markdownlint-disable MD041 -->
 
+<a name="readme-top"></a>
 
 <!-- PROJECT SHIELDS -->
 <div align="center">
 
-  <a href="[pypi-url]">[![PYPI - Version][version-shield]][pypi-url]</a>
-  <a href="[pypi-url]">[![PYPI - Downloads][downloads-shield]][pypi-url]</a>
-  <a href="[forks-url]">[![Forks][forks-shield]][forks-url]</a>
-  <a href="[stars-url]">[![Stargazers][stars-shield]][stars-url]</a>
-  <a href="[license-url]">[![BSD-3-Clause License][license-shield]][license-url]</a>
+<a href="[pypi-url]">[![PYPI - Version][version-shield]][pypi-url]</a>
+<a href="[pypi-url]">[![PYPI - Downloads][downloads-shield]][pypi-url]</a>
+<a href="[forks-url]">[![Forks][forks-shield]][forks-url]</a>
+<a href="[stars-url]">[![Stargazers][stars-shield]][stars-url]</a>
+<a href="[license-url]">[![BSD-3-Clause License][license-shield]][license-url]</a>
 
 </div>
 
 <!-- PROJECT LOGO -->
 <br />
 <div align="center">
   <a href="https://github.com/python-thread/thread">
@@ -30,117 +34,123 @@
     <br />
     <a href="https://github.com/python-thread/thread/issues">Report Bug</a>
     ·
     <a href="https://github.com/python-thread/thread/issues">Request Feature</a>
   </p>
 </div>
 
-
-
 <!-- ABOUT THE PROJECT -->
+
 ## About The Project
 
 [![Social Card][socialcard]](https://thread.ngjx.org)
 
-Strictly type-safe and Wraps around the python threading library and provides extra functionality
+Strictly type-safe and Wraps around the python threading library
+and provides extra functionality
 
-Fully compatible with the threading library, this project hopes to provide a more out-of-the-box solution with multi-threaded processing and fetching values from a completed thread, etc.
+Fully compatible with the threading library, this project hopes to
+provide a more out-of-the-box solution with multi-threaded processing
+and fetching values from a completed thread, etc.
 
 <br />
 
 **!! Important !!**<br />
 This project is in it's very early stages of development and bugs are to be expected.
 
 <br />
 
 I hope thread will become your threading solution! ♡⸜(˶˃ ᵕ ˂˶)⸝♡
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
-
-
 <!-- GETTING STARTED -->
+
 ## Getting Started
 
 This is an example of how you can set up your project locally.
 To get a local copy up and running follow these simple example steps.
 
 ### Prerequisites
 
-* Python 3.9+
+- Python 3.9+
 
 ### Installation
 
 _Below is an example of how you can install and use thread._
 
-1. Install the package
-   ```sh
-   pip install -U thread
-   ```
-2. Import thread into your library!
-   ```py
-   import thread
-   from thread import Thread, ConcurrentProcessing
-   ```
-
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
+#### 1. Install the package
 
+```sh
+pip install -U thread
+```
+
+#### 2. Import thread into your library
+
+```py
+import thread
+from thread import Thread, ConcurrentProcessing
+```
 
+<p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 <!-- CONTRIBUTING -->
-## Contributing
 
-Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**. ( ˶ˆᗜˆ˵ )
+## Contributing
 
-If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
+Contributions are what make the open source community
+such an amazing place to learn, inspire, and create.
+Any contributions you make are **greatly appreciated**. ( ˶ˆᗜˆ˵ )
+
+If you have a suggestion that would make this better,
+please fork the repo and create a pull request.
+You can also simply open an issue with the tag "enhancement".
 Don't forget to give the project a star! Thanks again!
 
 1. Fork the Project
 2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
 3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
 4. Push to the Branch (`git push origin feature/AmazingFeature`)
 5. Open a Pull Request
 
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
-
+Read our [contributing guide](./CONTRIBUTING.md) for more information.
 
+<p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 <!-- LICENSE -->
+
 ## License
 
-Distributed under the BSD-3-Clause License. See [LICENSE.txt](./LICENSE.txt) for more information.
+Distributed under the BSD-3-Clause License.
+See [LICENSE.txt](./LICENSE.txt) for more information.
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
-
-
 <!-- CONTACT -->
+
 ## Contact
 
 Alex - [contact@thread.ngjx.org](mailto:contact@thread.ngjx.org)
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
-
-
 <!-- ACKNOWLEDGMENTS -->
+
 ## Acknowledgments
 
-* [Choose an Open Source License](https://choosealicense.com)
-* [GitHub Emoji Cheat Sheet](https://www.webpagefx.com/tools/emoji-cheat-sheet)
-* [Malven's Flexbox Cheatsheet](https://flexbox.malven.co/)
-* [Malven's Grid Cheatsheet](https://grid.malven.co/)
-* [Img Shields](https://shields.io)
+- [Choose an Open Source License](https://choosealicense.com)
+- [GitHub Emoji Cheat Sheet](https://www.webpagefx.com/tools/emoji-cheat-sheet)
+- [Malven's Flexbox Cheatsheet](https://flexbox.malven.co/)
+- [Malven's Grid Cheatsheet](https://grid.malven.co/)
+- [Img Shields](https://shields.io)
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
-
-
 <!-- MARKDOWN LINKS & IMAGES -->
 <!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
+
 [version-shield]: https://img.shields.io/pypi/v/thread.svg?style=for-the-badge&color=efd0cd
 [downloads-shield]: https://img.shields.io/pypi/dm/thread.svg?style=for-the-badge
 [pypi-url]: https://pypi.org/project/thread/
 [forks-shield]: https://img.shields.io/github/forks/python-thread/thread.svg?style=for-the-badge
 [forks-url]: https://github.com/python-thread/thread/network/members
 [stars-shield]: https://img.shields.io/github/stars/python-thread/thread.svg?style=for-the-badge&color=yellow
 [stars-url]: https://github.com/python-thread/thread/stargazers
```

#### html2text {}

```diff
@@ -16,38 +16,39 @@
 **!! Important !!**
 This project is in it's very early stages of development and bugs are to be
 expected.
 I hope thread will become your threading solution! â¡â¸(Ë¶Ë áµ ËË¶)â¸â¡
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Getting Started This is an example of how you can set up your project
 locally. To get a local copy up and running follow these simple example steps.
-### Prerequisites * Python 3.9+ ### Installation _Below is an example of how
-you can install and use thread._ 1. Install the package ```sh pip install -
-U thread ``` 2. Import thread into your library! ```py import thread from
+### Prerequisites - Python 3.9+ ### Installation _Below is an example of how
+you can install and use thread._ #### 1. Install the package ```sh pip install
+-U thread ``` #### 2. Import thread into your library ```py import thread from
 thread import Thread, ConcurrentProcessing ```
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Contributing Contributions are what make the open source community such an
 amazing place to learn, inspire, and create. Any contributions you make are
 **greatly appreciated**. ( Ë¶ËáËËµ ) If you have a suggestion that would
 make this better, please fork the repo and create a pull request. You can also
 simply open an issue with the tag "enhancement". Don't forget to give the
 project a star! Thanks again! 1. Fork the Project 2. Create your Feature Branch
 (`git checkout -b feature/AmazingFeature`) 3. Commit your Changes (`git commit
 -m 'Add some AmazingFeature'`) 4. Push to the Branch (`git push origin feature/
-AmazingFeature`) 5. Open a Pull Request
+AmazingFeature`) 5. Open a Pull Request Read our [contributing guide](./
+CONTRIBUTING.md) for more information.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## License Distributed under the BSD-3-Clause License. See [LICENSE.txt](./
 LICENSE.txt) for more information.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Contact Alex - [contact@thread.ngjx.org](mailto:contact@thread.ngjx.org)
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
-## Acknowledgments * [Choose an Open Source License](https://
-choosealicense.com) * [GitHub Emoji Cheat Sheet](https://www.webpagefx.com/
-tools/emoji-cheat-sheet) * [Malven's Flexbox Cheatsheet](https://
-flexbox.malven.co/) * [Malven's Grid Cheatsheet](https://grid.malven.co/) *
+## Acknowledgments - [Choose an Open Source License](https://
+choosealicense.com) - [GitHub Emoji Cheat Sheet](https://www.webpagefx.com/
+tools/emoji-cheat-sheet) - [Malven's Flexbox Cheatsheet](https://
+flexbox.malven.co/) - [Malven's Grid Cheatsheet](https://grid.malven.co/) -
 [Img Shields](https://shields.io)
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 [version-shield]: https://img.shields.io/pypi/v/thread.svg?style=for-the-
 badge&color=efd0cd [downloads-shield]: https://img.shields.io/pypi/dm/
 thread.svg?style=for-the-badge [pypi-url]: https://pypi.org/project/thread/
 [forks-shield]: https://img.shields.io/github/forks/python-thread/
 thread.svg?style=for-the-badge [forks-url]: https://github.com/python-thread/
```

### Comparing `thread-2.0.2/pyproject.toml` & `thread-2.0.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "thread"
-version = "2.0.2"
+version = "2.0.3"
 description = "Threading module extension"
 authors = ["Alex <contact@ngjx.org>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 packages = [
   { include = "thread", from = "src" },
   { include = "thread/py.typed", from = "src" },
@@ -26,28 +26,28 @@
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: Implementation :: CPython",
   "Typing :: Typed",
 ]
 
 [tool.poetry.urls]
 Homepage = "https://thread.ngjx.org"
-Documentation = "https://thread.ngjx.org/docs/v2.0.2"
+Documentation = "https://thread.ngjx.org/docs/v2.0.3"
 Source = "https://github.com/python-thread/thread"
 Download = "https://pypi.org/project/thread/#files"
 "Release Notes" = "https://github.com/python-thread/thread/releases"
 "Bug Tracker" = "https://github.com/python-thread/thread/issues"
 
 [tool.poetry.scripts]
 thread = "thread.__main__:app"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 typing-extensions = "^4.9.0"
 importlib-metadata = { version = ">=4.4", python = "<3.10" }
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.4.3"
-ruff = "^0.1.5"
+pytest = ">=7.4.3,<9.0.0"
+ruff = ">=0.1.5,<0.5.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `thread-2.0.2/src/thread/__init__.py` & `thread-2.0.3/src/thread/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 ## Thread Library
-Documentation at https://thread.ngjx.org/docs/2.0.2
+Documentation at https://thread.ngjx.org/docs/2.0.3
 
 
 ---
 
 Released under the BSD-3 License
 
 Copyright (c) thread.ngjx.org, All rights reserved
```

### Comparing `thread-2.0.2/src/thread/_types.py` & `thread-2.0.3/src/thread/_types.py`

 * *Files identical despite different names*

### Comparing `thread-2.0.2/src/thread/decorators/_processor.py` & `thread-2.0.3/src/thread/decorators/_processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,41 +38,38 @@
     ConcurrentProcessing[_TargetP, _TargetT, _DataT],
 ]
 
 
 @overload
 def processor(
     __function: TargetFunction[_DataT, _TargetP, _TargetT],
-) -> NoParamReturn[_DataT, _TargetP, _TargetT]:
-    ...
+) -> NoParamReturn[_DataT, _TargetP, _TargetT]: ...
 
 
 @overload
 def processor(
     *,
     args: Sequence[Data_In] = (),
     kwargs: Mapping[str, Data_In] = {},
     ignore_errors: Sequence[type[Exception]] = (),
     suppress_errors: bool = False,
     **overflow_kwargs: Overflow_In,
-) -> WithParamReturn[_DataT, _TargetP, _TargetT]:
-    ...
+) -> WithParamReturn[_DataT, _TargetP, _TargetT]: ...
 
 
 @overload
 def processor(
     __function: TargetFunction[_DataT, _TargetP, _TargetT],
     *,
     args: Sequence[Data_In] = (),
     kwargs: Mapping[str, Data_In] = {},
     ignore_errors: Sequence[type[Exception]] = (),
     suppress_errors: bool = False,
     **overflow_kwargs: Overflow_In,
-) -> FullParamReturn[_DataT, _TargetP, _TargetT]:
-    ...
+) -> FullParamReturn[_DataT, _TargetP, _TargetT]: ...
 
 
 def processor(
     __function: Optional[TargetFunction[_DataT, _TargetP, _TargetT]] = None,
     *,
     args: Sequence[Data_In] = (),
     kwargs: Mapping[str, Data_In] = {},
```

### Comparing `thread-2.0.2/src/thread/decorators/_threaded.py` & `thread-2.0.3/src/thread/decorators/_threaded.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,41 +17,38 @@
 
 NoParamReturn = Callable[P, Thread[P, T]]
 WithParamReturn = Callable[[TargetFunction[P, T]], NoParamReturn[P, T]]
 FullParamReturn = Callable[P, Thread[P, T]]
 
 
 @overload
-def threaded(__function: TargetFunction[P, T]) -> NoParamReturn[P, T]:
-    ...
+def threaded(__function: TargetFunction[P, T]) -> NoParamReturn[P, T]: ...
 
 
 @overload
 def threaded(
     *,
     args: Sequence[Data_In] = (),
     kwargs: Mapping[str, Data_In] = {},
     ignore_errors: Sequence[type[Exception]] = (),
     suppress_errors: bool = False,
     **overflow_kwargs: Overflow_In,
-) -> WithParamReturn[P, T]:
-    ...
+) -> WithParamReturn[P, T]: ...
 
 
 @overload
 def threaded(
     __function: TargetFunction[P, T],
     *,
     args: Sequence[Data_In] = (),
     kwargs: Mapping[str, Data_In] = {},
     ignore_errors: Sequence[type[Exception]] = (),
     suppress_errors: bool = False,
     **overflow_kwargs: Overflow_In,
-) -> FullParamReturn[P, T]:
-    ...
+) -> FullParamReturn[P, T]: ...
 
 
 def threaded(
     __function: Optional[TargetFunction[P, T]] = None,
     *,
     args: Sequence[Data_In] = (),
     kwargs: Mapping[str, Data_In] = {},
```

### Comparing `thread-2.0.2/src/thread/exceptions.py` & `thread-2.0.3/src/thread/exceptions.py`

 * *Files identical despite different names*

### Comparing `thread-2.0.2/src/thread/thread.py` & `thread-2.0.3/src/thread/thread.py`

 * *Files 2% similar despite different names*

```diff
@@ -367,58 +367,54 @@
         function: DatasetFunction[_Dataset_T, _Target_P, _Target_T],
         dataset: LengthandGetLike_T,
         max_threads: int = 8,
         *overflow_args: Overflow_In,
         _get_value: Optional[Callable[[LengthandGetLike_T, int], _Dataset_T]] = None,
         _length: Optional[Union[int, Callable[[Any], int]]] = None,
         **overflow_kwargs: Overflow_In,
-    ) -> None:
-        ...
+    ) -> None: ...
 
     # Has __len__, require _get_value to be set
     @overload
     def __init__(
         self,
         function: DatasetFunction[_Dataset_T, _Target_P, _Target_T],
         dataset: LengthLike_T,
         max_threads: int = 8,
         *overflow_args: Overflow_In,
         _get_value: Callable[[LengthLike_T, int], _Dataset_T],
         _length: Optional[Union[int, Callable[[Any], int]]] = None,
         **overflow_kwargs: Overflow_In,
-    ) -> None:
-        ...
+    ) -> None: ...
 
     # Has __getitem__, require _length to be set
     @overload
     def __init__(
         self,
         function: DatasetFunction[_Dataset_T, _Target_P, _Target_T],
         dataset: GetLike_T,
         max_threads: int = 8,
         *overflow_args: Overflow_In,
         _get_value: Optional[Callable[[GetLike_T, int], _Dataset_T]] = None,
         _length: Union[int, Callable[[GetLike_T], int]],
         **overflow_kwargs: Overflow_In,
-    ) -> None:
-        ...
+    ) -> None: ...
 
     # Does not support __getitem__ and __len__
     @overload
     def __init__(
         self,
         function: DatasetFunction[_Dataset_T, _Target_P, _Target_T],
         dataset: Any,
         max_threads: int = 8,
         *overflow_args: Overflow_In,
         _get_value: Callable[[Any, int], _Dataset_T],
         _length: Union[int, Callable[[Any], int]],
         **overflow_kwargs: Overflow_In,
-    ) -> None:
-        ...
+    ) -> None: ...
 
     def __init__(
         self,
         function: DatasetFunction[_Dataset_T, _Target_P, _Target_T],
         dataset: Union[
             SupportsLengthGetItem[_Dataset_T],
             SupportsGetItem[_Dataset_T],
```

### Comparing `thread-2.0.2/src/thread/utils/algorithm.py` & `thread-2.0.3/src/thread/utils/algorithm.py`

 * *Files identical despite different names*

### Comparing `thread-2.0.2/src/thread/utils/config.py` & `thread-2.0.3/src/thread/utils/config.py`

 * *Files identical despite different names*

### Comparing `thread-2.0.2/tests/test_algorithm.py` & `thread-2.0.3/tests/test_algorithm.py`

 * *Files identical despite different names*

### Comparing `thread-2.0.2/tests/test_concurrentprocessing.py` & `thread-2.0.3/tests/test_concurrentprocessing.py`

 * *Files identical despite different names*

### Comparing `thread-2.0.2/tests/test_dataframe_compatibility.py` & `thread-2.0.3/tests/test_dataframe_compatibility.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,21 +29,19 @@
 
     def __init__(self, length: typing.Any, dataset: list):
         DummyLengthOnly.__init__(self, length)
         DummyGetOnly.__init__(self, dataset)
 
 
 class DummyUnlikeSequence1:
-    def __init__(self) -> None:
-        ...
+    def __init__(self) -> None: ...
 
 
 class DummyUnlikeSequence2:
-    def __init__(self) -> None:
-        ...
+    def __init__(self) -> None: ...
 
     def __str__(self) -> str:
         return 'invalid'
 
 
 # >>>>>>>>>> Length Only <<<<<<<<<< #
 def test_LO_init() -> None:
```

### Comparing `thread-2.0.2/tests/test_decorator.py` & `thread-2.0.3/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `thread-2.0.2/tests/test_thread.py` & `thread-2.0.3/tests/test_thread.py`

 * *Files identical despite different names*

### Comparing `thread-2.0.2/tests/test_verbosity.py` & `thread-2.0.3/tests/test_verbosity.py`

 * *Files identical despite different names*

### Comparing `thread-2.0.2/PKG-INFO` & `thread-2.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thread
-Version: 2.0.2
+Version: 2.0.3
 Summary: Threading module extension
 License: BSD-3-Clause
 Keywords: thread,threading,extension,multiprocessing
 Author: Alex
 Author-email: contact@ngjx.org
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -20,33 +20,37 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
 Requires-Dist: importlib-metadata (>=4.4) ; python_version < "3.10"
 Requires-Dist: typing-extensions (>=4.9.0,<5.0.0)
 Project-URL: Bug Tracker, https://github.com/python-thread/thread/issues
-Project-URL: Documentation, https://thread.ngjx.org/docs/v2.0.2
+Project-URL: Documentation, https://thread.ngjx.org/docs/v2.0.3
 Project-URL: Download, https://pypi.org/project/thread/#files
 Project-URL: Homepage, https://thread.ngjx.org
 Project-URL: Release Notes, https://github.com/python-thread/thread/releases
 Project-URL: Source, https://github.com/python-thread/thread
 Description-Content-Type: text/markdown
 
-<a name="readme-top"></a>
+<!-- Allow HTML -->
+<!-- markdownlint-disable MD033 -->
 
+<!-- Allow HTML top-level heading -->
+<!-- markdownlint-disable MD041 -->
 
+<a name="readme-top"></a>
 
 <!-- PROJECT SHIELDS -->
 <div align="center">
 
-  <a href="[pypi-url]">[![PYPI - Version][version-shield]][pypi-url]</a>
-  <a href="[pypi-url]">[![PYPI - Downloads][downloads-shield]][pypi-url]</a>
-  <a href="[forks-url]">[![Forks][forks-shield]][forks-url]</a>
-  <a href="[stars-url]">[![Stargazers][stars-shield]][stars-url]</a>
-  <a href="[license-url]">[![BSD-3-Clause License][license-shield]][license-url]</a>
+<a href="[pypi-url]">[![PYPI - Version][version-shield]][pypi-url]</a>
+<a href="[pypi-url]">[![PYPI - Downloads][downloads-shield]][pypi-url]</a>
+<a href="[forks-url]">[![Forks][forks-shield]][forks-url]</a>
+<a href="[stars-url]">[![Stargazers][stars-shield]][stars-url]</a>
+<a href="[license-url]">[![BSD-3-Clause License][license-shield]][license-url]</a>
 
 </div>
 
 <!-- PROJECT LOGO -->
 <br />
 <div align="center">
   <a href="https://github.com/python-thread/thread">
@@ -63,117 +67,123 @@
     <br />
     <a href="https://github.com/python-thread/thread/issues">Report Bug</a>
     ·
     <a href="https://github.com/python-thread/thread/issues">Request Feature</a>
   </p>
 </div>
 
-
-
 <!-- ABOUT THE PROJECT -->
+
 ## About The Project
 
 [![Social Card][socialcard]](https://thread.ngjx.org)
 
-Strictly type-safe and Wraps around the python threading library and provides extra functionality
+Strictly type-safe and Wraps around the python threading library
+and provides extra functionality
 
-Fully compatible with the threading library, this project hopes to provide a more out-of-the-box solution with multi-threaded processing and fetching values from a completed thread, etc.
+Fully compatible with the threading library, this project hopes to
+provide a more out-of-the-box solution with multi-threaded processing
+and fetching values from a completed thread, etc.
 
 <br />
 
 **!! Important !!**<br />
 This project is in it's very early stages of development and bugs are to be expected.
 
 <br />
 
 I hope thread will become your threading solution! ♡⸜(˶˃ ᵕ ˂˶)⸝♡
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
-
-
 <!-- GETTING STARTED -->
+
 ## Getting Started
 
 This is an example of how you can set up your project locally.
 To get a local copy up and running follow these simple example steps.
 
 ### Prerequisites
 
-* Python 3.9+
+- Python 3.9+
 
 ### Installation
 
 _Below is an example of how you can install and use thread._
 
-1. Install the package
-   ```sh
-   pip install -U thread
-   ```
-2. Import thread into your library!
-   ```py
-   import thread
-   from thread import Thread, ConcurrentProcessing
-   ```
-
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
+#### 1. Install the package
 
+```sh
+pip install -U thread
+```
+
+#### 2. Import thread into your library
+
+```py
+import thread
+from thread import Thread, ConcurrentProcessing
+```
 
+<p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 <!-- CONTRIBUTING -->
-## Contributing
 
-Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**. ( ˶ˆᗜˆ˵ )
+## Contributing
 
-If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
+Contributions are what make the open source community
+such an amazing place to learn, inspire, and create.
+Any contributions you make are **greatly appreciated**. ( ˶ˆᗜˆ˵ )
+
+If you have a suggestion that would make this better,
+please fork the repo and create a pull request.
+You can also simply open an issue with the tag "enhancement".
 Don't forget to give the project a star! Thanks again!
 
 1. Fork the Project
 2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
 3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
 4. Push to the Branch (`git push origin feature/AmazingFeature`)
 5. Open a Pull Request
 
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
-
+Read our [contributing guide](./CONTRIBUTING.md) for more information.
 
+<p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 <!-- LICENSE -->
+
 ## License
 
-Distributed under the BSD-3-Clause License. See [LICENSE.txt](./LICENSE.txt) for more information.
+Distributed under the BSD-3-Clause License.
+See [LICENSE.txt](./LICENSE.txt) for more information.
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
-
-
 <!-- CONTACT -->
+
 ## Contact
 
 Alex - [contact@thread.ngjx.org](mailto:contact@thread.ngjx.org)
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
-
-
 <!-- ACKNOWLEDGMENTS -->
+
 ## Acknowledgments
 
-* [Choose an Open Source License](https://choosealicense.com)
-* [GitHub Emoji Cheat Sheet](https://www.webpagefx.com/tools/emoji-cheat-sheet)
-* [Malven's Flexbox Cheatsheet](https://flexbox.malven.co/)
-* [Malven's Grid Cheatsheet](https://grid.malven.co/)
-* [Img Shields](https://shields.io)
+- [Choose an Open Source License](https://choosealicense.com)
+- [GitHub Emoji Cheat Sheet](https://www.webpagefx.com/tools/emoji-cheat-sheet)
+- [Malven's Flexbox Cheatsheet](https://flexbox.malven.co/)
+- [Malven's Grid Cheatsheet](https://grid.malven.co/)
+- [Img Shields](https://shields.io)
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
-
-
 <!-- MARKDOWN LINKS & IMAGES -->
 <!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
+
 [version-shield]: https://img.shields.io/pypi/v/thread.svg?style=for-the-badge&color=efd0cd
 [downloads-shield]: https://img.shields.io/pypi/dm/thread.svg?style=for-the-badge
 [pypi-url]: https://pypi.org/project/thread/
 [forks-shield]: https://img.shields.io/github/forks/python-thread/thread.svg?style=for-the-badge
 [forks-url]: https://github.com/python-thread/thread/network/members
 [stars-shield]: https://img.shields.io/github/stars/python-thread/thread.svg?style=for-the-badge&color=yellow
 [stars-url]: https://github.com/python-thread/thread/stargazers
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: thread Version: 2.0.2 Summary: Threading module
+Metadata-Version: 2.1 Name: thread Version: 2.0.3 Summary: Threading module
 extension License: BSD-3-Clause Keywords:
 thread,threading,extension,multiprocessing Author: Alex Author-email:
 contact@ngjx.org Requires-Python: >=3.9,<4.0 Classifier: Development Status ::
 4 - Beta Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: BSD License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
 Python :: Implementation :: CPython Classifier: Topic :: Software Development
 Classifier: Typing :: Typed Requires-Dist: importlib-metadata (>=4.4) ;
 python_version < "3.10" Requires-Dist: typing-extensions (>=4.9.0,<5.0.0)
 Project-URL: Bug Tracker, https://github.com/python-thread/thread/issues
-Project-URL: Documentation, https://thread.ngjx.org/docs/v2.0.2 Project-URL:
+Project-URL: Documentation, https://thread.ngjx.org/docs/v2.0.3 Project-URL:
 Download, https://pypi.org/project/thread/#files Project-URL: Homepage, https:/
 /thread.ngjx.org Project-URL: Release Notes, https://github.com/python-thread/
 thread/releases Project-URL: Source, https://github.com/python-thread/thread
 Description-Content-Type: text/markdown
  _[_!_[_P_Y_P_I_ _-_ _V_e_r_s_i_o_n_]_[_v_e_r_s_i_o_n_-_s_h_i_e_l_d_]_]_[_p_y_p_i_-_u_r_l_] _[_!_[_P_Y_P_I_ _-_ _D_o_w_n_l_o_a_d_s_]_[_d_o_w_n_l_o_a_d_s_-
  _s_h_i_e_l_d_]_]_[_p_y_p_i_-_u_r_l_] _[_!_[_F_o_r_k_s_]_[_f_o_r_k_s_-_s_h_i_e_l_d_]_]_[_f_o_r_k_s_-_u_r_l_] _[_!_[_S_t_a_r_g_a_z_e_r_s_]_[_s_t_a_r_s_-
   _s_h_i_e_l_d_]_]_[_s_t_a_r_s_-_u_r_l_] _[_!_[_B_S_D_-_3_-_C_l_a_u_s_e_ _L_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_-_s_h_i_e_l_d_]_]_[_l_i_c_e_n_s_e_-_u_r_l_]
@@ -36,38 +36,39 @@
 **!! Important !!**
 This project is in it's very early stages of development and bugs are to be
 expected.
 I hope thread will become your threading solution! â¡â¸(Ë¶Ë áµ ËË¶)â¸â¡
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Getting Started This is an example of how you can set up your project
 locally. To get a local copy up and running follow these simple example steps.
-### Prerequisites * Python 3.9+ ### Installation _Below is an example of how
-you can install and use thread._ 1. Install the package ```sh pip install -
-U thread ``` 2. Import thread into your library! ```py import thread from
+### Prerequisites - Python 3.9+ ### Installation _Below is an example of how
+you can install and use thread._ #### 1. Install the package ```sh pip install
+-U thread ``` #### 2. Import thread into your library ```py import thread from
 thread import Thread, ConcurrentProcessing ```
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Contributing Contributions are what make the open source community such an
 amazing place to learn, inspire, and create. Any contributions you make are
 **greatly appreciated**. ( Ë¶ËáËËµ ) If you have a suggestion that would
 make this better, please fork the repo and create a pull request. You can also
 simply open an issue with the tag "enhancement". Don't forget to give the
 project a star! Thanks again! 1. Fork the Project 2. Create your Feature Branch
 (`git checkout -b feature/AmazingFeature`) 3. Commit your Changes (`git commit
 -m 'Add some AmazingFeature'`) 4. Push to the Branch (`git push origin feature/
-AmazingFeature`) 5. Open a Pull Request
+AmazingFeature`) 5. Open a Pull Request Read our [contributing guide](./
+CONTRIBUTING.md) for more information.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## License Distributed under the BSD-3-Clause License. See [LICENSE.txt](./
 LICENSE.txt) for more information.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Contact Alex - [contact@thread.ngjx.org](mailto:contact@thread.ngjx.org)
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
-## Acknowledgments * [Choose an Open Source License](https://
-choosealicense.com) * [GitHub Emoji Cheat Sheet](https://www.webpagefx.com/
-tools/emoji-cheat-sheet) * [Malven's Flexbox Cheatsheet](https://
-flexbox.malven.co/) * [Malven's Grid Cheatsheet](https://grid.malven.co/) *
+## Acknowledgments - [Choose an Open Source License](https://
+choosealicense.com) - [GitHub Emoji Cheat Sheet](https://www.webpagefx.com/
+tools/emoji-cheat-sheet) - [Malven's Flexbox Cheatsheet](https://
+flexbox.malven.co/) - [Malven's Grid Cheatsheet](https://grid.malven.co/) -
 [Img Shields](https://shields.io)
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 [version-shield]: https://img.shields.io/pypi/v/thread.svg?style=for-the-
 badge&color=efd0cd [downloads-shield]: https://img.shields.io/pypi/dm/
 thread.svg?style=for-the-badge [pypi-url]: https://pypi.org/project/thread/
 [forks-shield]: https://img.shields.io/github/forks/python-thread/
 thread.svg?style=for-the-badge [forks-url]: https://github.com/python-thread/
```

