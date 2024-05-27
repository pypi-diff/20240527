# Comparing `tmp/wagtail_translatableforms-0.1.4.tar.gz` & `tmp/wagtail_translatableforms-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_translatableforms-0.1.4.tar", max compression
+gzip compressed data, was "wagtail_translatableforms-0.1.5.tar", max compression
```

## Comparing `wagtail_translatableforms-0.1.4.tar` & `wagtail_translatableforms-0.1.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1069 2024-05-21 15:01:21.958783 wagtail_translatableforms-0.1.4/LICENSE
--rw-r--r--   0        0        0    12199 2024-05-23 07:35:22.442416 wagtail_translatableforms-0.1.4/README.md
--rw-r--r--   0        0        0      567 2024-05-23 07:35:25.314419 wagtail_translatableforms-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      977 2024-05-22 11:16:42.552643 wagtail_translatableforms-0.1.4/wagtail_translatableforms/__init__.py
--rw-r--r--   0        0        0     4656 2024-05-22 14:05:58.582858 wagtail_translatableforms-0.1.4/wagtail_translatableforms/apps.py
--rw-r--r--   0        0        0     1467 2024-05-22 11:16:42.556643 wagtail_translatableforms-0.1.4/wagtail_translatableforms/blocks.py
--rw-r--r--   0        0        0     8600 2024-05-22 11:16:42.556643 wagtail_translatableforms-0.1.4/wagtail_translatableforms/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2024-05-22 11:16:42.556643 wagtail_translatableforms-0.1.4/wagtail_translatableforms/migrations/__init__.py
--rw-r--r--   0        0        0     5689 2024-05-22 11:16:42.560643 wagtail_translatableforms-0.1.4/wagtail_translatableforms/models.py
--rw-r--r--   0        0        0     1777 2024-05-22 11:32:03.624558 wagtail_translatableforms-0.1.4/wagtail_translatableforms/serializers.py
--rw-r--r--   0        0        0     1046 2024-05-22 11:16:42.564643 wagtail_translatableforms-0.1.4/wagtail_translatableforms/templates/customforms/confirm_delete.html
--rw-r--r--   0        0        0     4945 2024-05-22 11:16:42.564643 wagtail_translatableforms-0.1.4/wagtail_translatableforms/templates/customforms/index.html
--rw-r--r--   0        0        0     4124 2024-05-22 11:16:42.564643 wagtail_translatableforms-0.1.4/wagtail_translatableforms/templates/customforms/index_submissions.html
--rw-r--r--   0        0        0     1047 2024-05-22 11:16:42.564643 wagtail_translatableforms-0.1.4/wagtail_translatableforms/templates/customforms/result_list.html
--rw-r--r--   0        0        0        0 2024-05-22 11:16:42.564643 wagtail_translatableforms-0.1.4/wagtail_translatableforms/templatetags/__init__.py
--rw-r--r--   0        0        0     4593 2024-05-22 11:16:42.568643 wagtail_translatableforms-0.1.4/wagtail_translatableforms/templatetags/custom_tags.py
--rw-r--r--   0        0        0      405 2024-05-22 11:16:42.568643 wagtail_translatableforms-0.1.4/wagtail_translatableforms/urls.py
--rw-r--r--   0        0        0     1155 2024-05-22 11:16:42.568643 wagtail_translatableforms-0.1.4/wagtail_translatableforms/utils.py
--rw-r--r--   0        0        0     4137 2024-05-22 11:16:42.568643 wagtail_translatableforms-0.1.4/wagtail_translatableforms/views.py
--rw-r--r--   0        0        0    13004 1970-01-01 00:00:00.000000 wagtail_translatableforms-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-21 15:01:21.958783 wagtail_translatableforms-0.1.5/LICENSE
+-rw-r--r--   0        0        0    13858 2024-05-27 13:21:54.940057 wagtail_translatableforms-0.1.5/README.md
+-rw-r--r--   0        0        0      597 2024-05-27 13:22:59.811205 wagtail_translatableforms-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      977 2024-05-22 11:16:42.552643 wagtail_translatableforms-0.1.5/wagtail_translatableforms/__init__.py
+-rw-r--r--   0        0        0     4810 2024-05-27 13:17:12.257411 wagtail_translatableforms-0.1.5/wagtail_translatableforms/apps.py
+-rw-r--r--   0        0        0     1467 2024-05-22 11:16:42.556643 wagtail_translatableforms-0.1.5/wagtail_translatableforms/blocks.py
+-rw-r--r--   0        0        0     8600 2024-05-22 11:16:42.556643 wagtail_translatableforms-0.1.5/wagtail_translatableforms/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-05-22 11:16:42.556643 wagtail_translatableforms-0.1.5/wagtail_translatableforms/migrations/__init__.py
+-rw-r--r--   0        0        0     5712 2024-05-27 09:05:02.925948 wagtail_translatableforms-0.1.5/wagtail_translatableforms/models.py
+-rw-r--r--   0        0        0     1777 2024-05-22 11:32:03.624558 wagtail_translatableforms-0.1.5/wagtail_translatableforms/serializers.py
+-rw-r--r--   0        0        0     1046 2024-05-22 11:16:42.564643 wagtail_translatableforms-0.1.5/wagtail_translatableforms/templates/customforms/confirm_delete.html
+-rw-r--r--   0        0        0     4945 2024-05-22 11:16:42.564643 wagtail_translatableforms-0.1.5/wagtail_translatableforms/templates/customforms/index.html
+-rw-r--r--   0        0        0     4124 2024-05-22 11:16:42.564643 wagtail_translatableforms-0.1.5/wagtail_translatableforms/templates/customforms/index_submissions.html
+-rw-r--r--   0        0        0     1047 2024-05-22 11:16:42.564643 wagtail_translatableforms-0.1.5/wagtail_translatableforms/templates/customforms/result_list.html
+-rw-r--r--   0        0        0        0 2024-05-22 11:16:42.564643 wagtail_translatableforms-0.1.5/wagtail_translatableforms/templatetags/__init__.py
+-rw-r--r--   0        0        0     4593 2024-05-22 11:16:42.568643 wagtail_translatableforms-0.1.5/wagtail_translatableforms/templatetags/custom_tags.py
+-rw-r--r--   0        0        0      405 2024-05-22 11:16:42.568643 wagtail_translatableforms-0.1.5/wagtail_translatableforms/urls.py
+-rw-r--r--   0        0        0     1155 2024-05-22 11:16:42.568643 wagtail_translatableforms-0.1.5/wagtail_translatableforms/utils.py
+-rw-r--r--   0        0        0     4137 2024-05-22 11:16:42.568643 wagtail_translatableforms-0.1.5/wagtail_translatableforms/views.py
+-rw-r--r--   0        0        0    14714 1970-01-01 00:00:00.000000 wagtail_translatableforms-0.1.5/PKG-INFO
```

### Comparing `wagtail_translatableforms-0.1.4/LICENSE` & `wagtail_translatableforms-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_translatableforms-0.1.4/README.md` & `wagtail_translatableforms-0.1.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 * django = "^4.2.11";
 * djangorestframework = ^3.15.0";
 * drf_spectacular = "^0.27.1"
 * wagtailstreamforms = "^4.1.0"
 * wagtail-localize = "^1.8.2"
 * wagtail = "^5.2.3"
+* wagtail-modeladmin = "^2.0.0"
 
 ## Installation
 
 1. Install using pip:
 
 ```
 pip install wagtail_translatableforms
@@ -255,8 +256,40 @@
     Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 
     Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 
     Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
 
 THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+```
+
+We use [wagtail-modeladmin](https://pypi.org/project/wagtail-modeladmin/), below is a quote from their license agreement:
+
+```
+Copyright (c) 2023, Wagtail Core Team
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without modification,
+are permitted provided that the following conditions are met:
+
+* Redistributions of source code must retain the above copyright notice, this
+  list of conditions and the following disclaimer.
+
+* Redistributions in binary form must reproduce the above copyright notice, this
+  list of conditions and the following disclaimer in the documentation and/or
+  other materials provided with the distribution.
+
+* Neither the name of the copyright holder nor the names of its
+  contributors may be used to endorse or promote products derived from this
+  software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
+ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
+WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED.
+IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT,
+INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING,
+BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
+DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY
+OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
+OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED
+OF THE POSSIBILITY OF SUCH DAMAGE.
 ```
```

### Comparing `wagtail_translatableforms-0.1.4/pyproject.toml` & `wagtail_translatableforms-0.1.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "wagtail_translatableforms"
-version = "0.1.4"
+version = "0.1.5"
 description = "Add translatableforms to wagtail projects"
 authors = ["Egor Nikitin <eanikitin90@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/BenderEg/wagtail-translatableforms"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">=3.11"
 django = "^4.2.11"
 djangorestframework = "^3.15.0"
 drf_spectacular = "^0.27.1"
 wagtailstreamforms = "^4.1.0"
 wagtail-localize = "^1.8.2"
 wagtail = "^5.2.3"
+wagtail-modeladmin = "^2.0.0"
```

### Comparing `wagtail_translatableforms-0.1.4/wagtail_translatableforms/__init__.py` & `wagtail_translatableforms-0.1.5/wagtail_translatableforms/__init__.py`

 * *Files identical despite different names*

### Comparing `wagtail_translatableforms-0.1.4/wagtail_translatableforms/apps.py` & `wagtail_translatableforms-0.1.5/wagtail_translatableforms/apps.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,14 +7,18 @@
     def ready(self) -> None:
 
         from django.conf import settings
         from django.core.exceptions import ImproperlyConfigured
 
         for app in (
             'django.contrib.admin',
+            'django.contrib.admin',
+            'django.contrib.contenttypes',
+            'django.contrib.sites',
+            'django.contrib.messages',
             'rest_framework',
             'drf_spectacular',
             'wagtail_modeladmin',
             'wagtail.snippets',
             'wagtail',
             'wagtail_localize',
             'wagtailstreamforms',
```

### Comparing `wagtail_translatableforms-0.1.4/wagtail_translatableforms/blocks.py` & `wagtail_translatableforms-0.1.5/wagtail_translatableforms/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_translatableforms-0.1.4/wagtail_translatableforms/migrations/0001_initial.py` & `wagtail_translatableforms-0.1.5/wagtail_translatableforms/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail_translatableforms-0.1.4/wagtail_translatableforms/models.py` & `wagtail_translatableforms-0.1.5/wagtail_translatableforms/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -129,33 +129,34 @@
 
         return form_copy
 
     def get_submission_class(self):
         """Returns submission class."""
         return CustomFormSubmission
 
+    @transaction.atomic()
     def delete(self, **kwargs) -> tuple[int, dict[str, int]]:
         content = get_translation_source_content()
         filtered = list(
             filter(
                 lambda x: (tmp := loads(x))["pk"] == self.pk
                 and tmp["translation_key"] == str(self.translation_key),
                 content,
             ),
         )
         if filtered:
-            related_forms = self.__class__.objects.filter(
+            related_forms = self.__class__.objects.exclude(pk=self.pk).filter(
                 translation_key=self.translation_key,
             )
             with transaction.atomic():
                 for ele in related_forms:
                     ele.delete()
-            return None
         return super().delete(**kwargs)
 
+
     def process_form_submission(self, form, ip_addr=None):
         """Runs each hook if selected in the form."""
 
         for fn in hooks.get_hooks("process_form_submission"):
             if fn.__name__ in self.process_form_submission_hooks:
                 fn(self, form, ip_addr)
```

### Comparing `wagtail_translatableforms-0.1.4/wagtail_translatableforms/serializers.py` & `wagtail_translatableforms-0.1.5/wagtail_translatableforms/serializers.py`

 * *Files identical despite different names*

### Comparing `wagtail_translatableforms-0.1.4/wagtail_translatableforms/templates/customforms/confirm_delete.html` & `wagtail_translatableforms-0.1.5/wagtail_translatableforms/templates/customforms/confirm_delete.html`

 * *Files identical despite different names*

### Comparing `wagtail_translatableforms-0.1.4/wagtail_translatableforms/templates/customforms/index.html` & `wagtail_translatableforms-0.1.5/wagtail_translatableforms/templates/customforms/index.html`

 * *Files identical despite different names*

### Comparing `wagtail_translatableforms-0.1.4/wagtail_translatableforms/templates/customforms/index_submissions.html` & `wagtail_translatableforms-0.1.5/wagtail_translatableforms/templates/customforms/index_submissions.html`

 * *Files identical despite different names*

### Comparing `wagtail_translatableforms-0.1.4/wagtail_translatableforms/templates/customforms/result_list.html` & `wagtail_translatableforms-0.1.5/wagtail_translatableforms/templates/customforms/result_list.html`

 * *Files identical despite different names*

### Comparing `wagtail_translatableforms-0.1.4/wagtail_translatableforms/templatetags/custom_tags.py` & `wagtail_translatableforms-0.1.5/wagtail_translatableforms/templatetags/custom_tags.py`

 * *Files identical despite different names*

### Comparing `wagtail_translatableforms-0.1.4/wagtail_translatableforms/utils.py` & `wagtail_translatableforms-0.1.5/wagtail_translatableforms/utils.py`

 * *Files identical despite different names*

### Comparing `wagtail_translatableforms-0.1.4/wagtail_translatableforms/views.py` & `wagtail_translatableforms-0.1.5/wagtail_translatableforms/views.py`

 * *Files identical despite different names*

### Comparing `wagtail_translatableforms-0.1.4/PKG-INFO` & `wagtail_translatableforms-0.1.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_translatableforms
-Version: 0.1.4
+Version: 0.1.5
 Summary: Add translatableforms to wagtail projects
 Home-page: https://github.com/BenderEg/wagtail-translatableforms
 License: MIT
 Author: Egor Nikitin
 Author-email: eanikitin90@gmail.com
 Requires-Python: >=3.11
 Classifier: License :: OSI Approved :: MIT License
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: django (>=4.2.11,<5.0.0)
 Requires-Dist: djangorestframework (>=3.15.0,<4.0.0)
 Requires-Dist: drf_spectacular (>=0.27.1,<0.28.0)
 Requires-Dist: wagtail (>=5.2.3,<6.0.0)
 Requires-Dist: wagtail-localize (>=1.8.2,<2.0.0)
+Requires-Dist: wagtail-modeladmin (>=2.0.0,<3.0.0)
 Requires-Dist: wagtailstreamforms (>=4.1.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # WAGTAIL_TRANSLATABLEFORMS
 
 Wagtail Translatableforms is an additional plagin for [Wagtail CMS](https://wagtail.org/).
 It is based on [Wagtail Localize](https://pypi.org/project/wagtail-localize/), [Wagtailstreamforms](https://pypi.org/project/wagtailstreamforms/) and [Django](https://www.djangoproject.com/).
@@ -38,14 +39,15 @@
 
 * django = "^4.2.11";
 * djangorestframework = ^3.15.0";
 * drf_spectacular = "^0.27.1"
 * wagtailstreamforms = "^4.1.0"
 * wagtail-localize = "^1.8.2"
 * wagtail = "^5.2.3"
+* wagtail-modeladmin = "^2.0.0"
 
 ## Installation
 
 1. Install using pip:
 
 ```
 pip install wagtail_translatableforms
@@ -277,7 +279,39 @@
 
     Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 
     Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
 
 THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 ```
+
+We use [wagtail-modeladmin](https://pypi.org/project/wagtail-modeladmin/), below is a quote from their license agreement:
+
+```
+Copyright (c) 2023, Wagtail Core Team
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without modification,
+are permitted provided that the following conditions are met:
+
+* Redistributions of source code must retain the above copyright notice, this
+  list of conditions and the following disclaimer.
+
+* Redistributions in binary form must reproduce the above copyright notice, this
+  list of conditions and the following disclaimer in the documentation and/or
+  other materials provided with the distribution.
+
+* Neither the name of the copyright holder nor the names of its
+  contributors may be used to endorse or promote products derived from this
+  software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
+ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
+WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED.
+IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT,
+INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING,
+BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
+DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY
+OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
+OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED
+OF THE POSSIBILITY OF SUCH DAMAGE.
+```
```

