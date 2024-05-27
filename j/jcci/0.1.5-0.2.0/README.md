# Comparing `tmp/jcci-0.1.5.tar.gz` & `tmp/jcci-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jcci-0.1.5.tar", last modified: Tue Apr 16 05:43:53 2024, max compression
+gzip compressed data, was "jcci-0.2.0.tar", last modified: Mon May 27 07:40:15 2024, max compression
```

## Comparing `jcci-0.1.5.tar` & `jcci-0.2.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 05:43:53.849041 jcci-0.1.5/
--rw-rw-rw-   0        0        0    11541 2024-04-03 09:49:05.000000 jcci-0.1.5/LICENSE
--rw-rw-rw-   0        0        0    15384 2024-04-16 05:43:53.847043 jcci-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     4700 2024-04-10 09:22:17.000000 jcci-0.1.5/README.md
--rw-rw-rw-   0        0        0     1592 2024-04-08 09:44:49.000000 jcci-0.1.5/README.pypi.md
--rw-rw-rw-   0        0        0      763 2024-04-12 09:32:17.000000 jcci-0.1.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-16 05:43:53.849041 jcci-0.1.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-16 05:43:53.797042 jcci-0.1.5/src/
-drwxrwxrwx   0        0        0        0 2024-04-16 05:43:53.831040 jcci-0.1.5/src/jcci/
--rw-rw-rw-   0        0        0        0 2024-04-09 03:17:36.000000 jcci-0.1.5/src/jcci/__init__.py
--rw-rw-rw-   0        0        0    43941 2024-04-12 09:31:08.000000 jcci-0.1.5/src/jcci/analyze.py
--rw-rw-rw-   0        0        0      249 2024-03-25 10:13:40.000000 jcci-0.1.5/src/jcci/config.py
--rw-rw-rw-   0        0        0      702 2024-04-12 03:25:49.000000 jcci-0.1.5/src/jcci/constant.py
--rw-rw-rw-   0        0        0     5344 2024-04-09 06:57:19.000000 jcci-0.1.5/src/jcci/database.py
--rw-rw-rw-   0        0        0     1985 2024-04-03 09:15:20.000000 jcci-0.1.5/src/jcci/diff_parse.py
--rw-rw-rw-   0        0        0     7933 2024-04-12 09:31:08.000000 jcci-0.1.5/src/jcci/graph.py
--rw-rw-rw-   0        0        0    41979 2024-04-12 09:15:24.000000 jcci-0.1.5/src/jcci/java_parse.py
--rw-rw-rw-   0        0        0     4516 2024-04-11 11:59:35.000000 jcci-0.1.5/src/jcci/mapper_parse.py
--rw-rw-rw-   0        0        0     2027 2024-03-25 09:09:49.000000 jcci-0.1.5/src/jcci/sql.py
-drwxrwxrwx   0        0        0        0 2024-04-16 05:43:53.844041 jcci-0.1.5/src/jcci.egg-info/
--rw-rw-rw-   0        0        0    15384 2024-04-16 05:43:53.000000 jcci-0.1.5/src/jcci.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      431 2024-04-16 05:43:53.000000 jcci-0.1.5/src/jcci.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 05:43:53.000000 jcci-0.1.5/src/jcci.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2024-04-16 05:43:53.000000 jcci-0.1.5/src/jcci.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-16 05:43:53.000000 jcci-0.1.5/src/jcci.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-16 05:43:53.842046 jcci-0.1.5/test/
--rw-rw-rw-   0        0        0        0 2024-04-08 06:40:37.000000 jcci-0.1.5/test/test_case.py
+drwxrwxrwx   0        0        0        0 2024-05-27 07:40:15.418904 jcci-0.2.0/
+-rw-rw-rw-   0        0        0    11541 2024-04-03 09:49:05.000000 jcci-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0    15416 2024-05-27 07:40:15.416900 jcci-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3679 2024-05-27 03:00:00.000000 jcci-0.2.0/README.md
+-rw-rw-rw-   0        0        0     1612 2024-05-15 07:56:19.000000 jcci-0.2.0/README.pypi.md
+-rw-rw-rw-   0        0        0      775 2024-05-27 07:39:38.000000 jcci-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-27 07:40:15.418904 jcci-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-27 07:40:15.379259 jcci-0.2.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-27 07:40:15.404902 jcci-0.2.0/src/jcci/
+-rw-rw-rw-   0        0        0        0 2024-04-09 03:17:36.000000 jcci-0.2.0/src/jcci/__init__.py
+-rw-rw-rw-   0        0        0    50225 2024-05-27 02:59:56.000000 jcci-0.2.0/src/jcci/analyze.py
+-rw-rw-rw-   0        0        0      289 2024-05-06 05:41:58.000000 jcci-0.2.0/src/jcci/config.py
+-rw-rw-rw-   0        0        0     1677 2024-05-15 07:56:19.000000 jcci-0.2.0/src/jcci/constant.py
+-rw-rw-rw-   0        0        0     5531 2024-05-15 07:56:19.000000 jcci-0.2.0/src/jcci/database.py
+-rw-rw-rw-   0        0        0     1985 2024-04-03 09:15:20.000000 jcci-0.2.0/src/jcci/diff_parse.py
+-rw-rw-rw-   0        0        0     8521 2024-05-27 02:59:56.000000 jcci-0.2.0/src/jcci/graph.py
+-rw-rw-rw-   0        0        0    62842 2024-05-27 03:00:00.000000 jcci-0.2.0/src/jcci/java_parse.py
+-rw-rw-rw-   0        0        0     4528 2024-05-15 07:56:19.000000 jcci-0.2.0/src/jcci/mapper_parse.py
+-rw-rw-rw-   0        0        0     2027 2024-03-25 09:09:49.000000 jcci-0.2.0/src/jcci/sql.py
+drwxrwxrwx   0        0        0        0 2024-05-27 07:40:15.415899 jcci-0.2.0/src/jcci.egg-info/
+-rw-rw-rw-   0        0        0    15416 2024-05-27 07:40:15.000000 jcci-0.2.0/src/jcci.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      431 2024-05-27 07:40:15.000000 jcci-0.2.0/src/jcci.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 07:40:15.000000 jcci-0.2.0/src/jcci.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2024-05-27 07:40:15.000000 jcci-0.2.0/src/jcci.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-27 07:40:15.000000 jcci-0.2.0/src/jcci.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-27 07:40:15.413901 jcci-0.2.0/test/
+-rw-rw-rw-   0        0        0        0 2024-04-08 06:40:37.000000 jcci-0.2.0/test/test_case.py
```

### Comparing `jcci-0.1.5/LICENSE` & `jcci-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jcci-0.1.5/PKG-INFO` & `jcci-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jcci
-Version: 0.1.5
+Version: 0.2.0
 Summary: Java code commit impact, java code change impact analysis, java代码改动影响范围分析工具
 Author-email: Oliver Li <441640312@qq.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -203,30 +203,29 @@
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
 Project-URL: Homepage, https://github.com/baikaishuipp/jcci
 Project-URL: Bug Tracker, https://github.com/baikaishuipp/jcci/issues
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: javalang>=0.13.0
 Requires-Dist: unidiff>=0.7.4
 
 #### Description
 Java code commit impact analysis, is a pure python library that analyzes the impact of two git submissions of Java projects on the project and generates tree chart data.
 
 Github: [jcci](https://github.com/baikaishuipp/jcci)
-#### Installation
-```
-pip install jcci
-```
+
+#### Achieve Effect
+![效果图](./images/cii-result-tree.png)
 
 #### Instructions
 Start a new python project, add a new python file, code example:
 
 ```
 from jcci.analyze import JCCI
```

### Comparing `jcci-0.1.5/README.pypi.md` & `jcci-0.2.0/README.pypi.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #### Description
 Java code commit impact analysis, is a pure python library that analyzes the impact of two git submissions of Java projects on the project and generates tree chart data.
 
 Github: [jcci](https://github.com/baikaishuipp/jcci)
-#### Installation
-```
-pip install jcci
-```
+
+#### Achieve Effect
+![效果图](./images/cii-result-tree.png)
 
 #### Instructions
 Start a new python project, add a new python file, code example:
 
 ```
 from jcci.analyze import JCCI
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `jcci-0.1.5/pyproject.toml` & `jcci-0.2.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jcci"
-version = "0.1.5"
+version = "0.2.0"
 authors = [
   { name="Oliver Li", email="441640312@qq.com" },
 ]
 description = "Java code commit impact, java code change impact analysis, java代码改动影响范围分析工具"
 readme = "README.pypi.md"
 license = { file="LICENSE" }
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
+    "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "javalang >= 0.13.0",
     "unidiff >= 0.7.4"
 ]
```

### Comparing `jcci-0.1.5/src/jcci/analyze.py` & `jcci-0.2.0/src/jcci/analyze.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,27 +4,28 @@
 import time
 import atexit
 import logging
 import datetime
 import fnmatch
 from . import config as config
 from .database import SqliteHelper
-from .java_parse import JavaParse
+from .java_parse import JavaParse, calculate_similar_score_method_params
 from . import mapper_parse as mapper_parse
 from . import diff_parse as diff_parse
 from . import graph as graph
 from . import constant as constant
 
 logging.basicConfig(format='%(asctime)s %(message)s', level=logging.DEBUG)
 
 
 class JCCI(object):
     def __init__(self, git_url, username):
         self.git_url = git_url
         self.username: str = username
+        # self.git_token = git_token
         self.branch_name: str = ''
         self.commit_or_branch_new: str = ''
         self.commit_or_branch_old: str = ''
         self.project_id: int = -1
         self.cci_filepath: str = ''
         self.project_name: str = ''
         self.file_path: str = ''
@@ -119,15 +120,15 @@
         time.sleep(2)
         xml_parse_result_old = self._parse_xml_file(diff_xml_file_path)
         for key in self.diff_parse_map.keys():
             matched_file_path_list = [filepath for filepath in file_path_list if filepath.endswith(key)]
             if not matched_file_path_list:
                 continue
             matched_file_path = matched_file_path_list[0]
-            java_parse.parse_java_file(matched_file_path, old_commit_or_branch)
+            java_parse.parse_java_file(matched_file_path, old_commit_or_branch, parse_import_first=False)
         return xml_parse_result_new, xml_parse_result_old
 
     # Step 3
     def _parse_branch_project(self, project_dir, new_branch, old_branch):
         # 解析最新的项目文件
         os.system(f'cd {project_dir} && git checkout {new_branch}')
         time.sleep(2)
@@ -141,15 +142,15 @@
         time.sleep(2)
         xml_parse_result_old = self._parse_xml_file(diff_xml_file_path)
         for key in self.diff_parse_map.keys():
             matched_file_path_list = [filepath for filepath in file_path_list if filepath.endswith(key)]
             if not matched_file_path_list:
                 continue
             matched_file_path = matched_file_path_list[0]
-            java_parse.parse_java_file(matched_file_path, old_branch)
+            java_parse.parse_java_file(matched_file_path, old_branch, parse_import_first=False)
         return xml_parse_result_new, xml_parse_result_old
 
     # Step 3.1 get all java files
     def _get_project_files(self, project_dir):
         file_lists = []
         for root, dirs, files in os.walk(project_dir):
             if '.git' in root or os.path.join('src', 'test') in root:
@@ -159,15 +160,16 @@
                 filepath = os.path.join(root, file)
                 for pattern in config.ignore_file:
                     if fnmatch.fnmatch(filepath, pattern):
                         ignore = True
                         break
                 if ignore:
                     continue
-                file_lists.append(filepath.replace('\\', '/'))
+                filepath = filepath.replace('\\', '/')
+                file_lists.append(filepath)
         return file_lists
 
     # Step 3.3
     def _parse_xml_file(self, file_path_list):
         xml_parse_results = {}
         for filepath in file_path_list:
             if filepath.endswith('.xml'):
@@ -231,177 +233,204 @@
             line_num_in_method = True
         return line_num_in_method
 
     # Step 4.2
     def _java_diff_analyze(self, patch_filepath: str, diff_parse_obj: dict):
         # new branch or commit
         class_db = self.sqlite.select_data(f'''SELECT * FROM class WHERE project_id = {self.project_id} and commit_or_branch = "{self.commit_or_branch_new}" and filepath LIKE "%{patch_filepath}"''')
-        if class_db:
-            class_db_obj = class_db[0]
+        for class_db_obj in class_db:
             self._java_field_method_diff_analyze(class_db_obj, diff_parse_obj['line_num_added'], diff_parse_obj['line_content_added'], self.commit_or_branch_new)
         # old branch or commit
         if not self.commit_or_branch_old:
             return
         class_db = self.sqlite.select_data(f'SELECT * FROM class WHERE project_id = {self.project_id} and commit_or_branch = "{self.commit_or_branch_old}" and filepath LIKE "%{patch_filepath}"')
-        if class_db:
-            class_db_obj = class_db[0]
+        for class_db_obj in class_db:
             self._java_field_method_diff_analyze(class_db_obj, diff_parse_obj['line_num_removed'], diff_parse_obj['line_content_removed'], self.commit_or_branch_old)
 
     # Step 4.2.1
     def _java_field_method_diff_analyze(self, class_db: dict, line_num_list: list, line_content_list: list, commit_or_branch: str or None):
         if not commit_or_branch:
             return
         class_name = class_db['class_name']
         class_filepath = class_db['filepath']
         is_controller = class_db['is_controller']
         data_in_annotation = [annotation for annotation in json.loads(class_db['annotations']) if annotation['name'] in ['Data', 'Getter', 'Setter', 'Builder', 'NoArgsConstructor', 'AllArgsConstructor']]
         for line_num in line_num_list:
             diff_content = line_content_list[line_num_list.index(line_num)]
-            fields_list = self.sqlite.select_data(f'SELECT * FROM field WHERE class_id = {class_db["class_id"]} AND start_line <={line_num} AND end_line >= {line_num} order by start_line asc limit 1')
-            methods_list = self.sqlite.select_data(f'SELECT * FROM methods WHERE class_id = {class_db["class_id"]} AND start_line <={line_num} AND end_line >= {line_num} order by start_line asc limit 1')
+            fields_list = self.sqlite.select_data(f'SELECT field_id, class_id, field_type, field_name, documentation, is_static FROM field WHERE class_id = {class_db["class_id"]} AND start_line <={line_num} AND end_line >= {line_num} order by start_line asc limit 1')
+            methods_list = self.sqlite.select_data(f'SELECT method_id, class_id, method_name, parameters, return_type, is_api, api_path, documentation, body FROM methods WHERE class_id = {class_db["class_id"]} AND start_line <={line_num} AND end_line >= {line_num} order by start_line asc limit 1')
+            class_node_id = None
             if fields_list:
                 is_not_static_fields = [field for field in fields_list if field.get('is_static') == 'False']
                 if is_not_static_fields and data_in_annotation:
                     self._add_to_need_analyze_obj_list('java', f'{class_db["package_name"]}.{class_name}', None, None, commit_or_branch, class_db)
+                    class_node_id = self.view.create_node_category(class_name, 'entity', constant.NODE_TYPE_CLASS, constant.DIFF_TYPE_CHANGED, '', self.file_path, '', '', {})
                 elif is_not_static_fields and not data_in_annotation:
                     field_method_name = []
                     for field in is_not_static_fields:
                         field_name = field['field_name']
                         field_name_capitalize = field_name[0].upper() + field_name[1:]
                         field_method_name += ['get' + field_name_capitalize, 'set' + field_name_capitalize, 'is' + field_name_capitalize]
                     field_method_name_str = '"' + '","'.join(field_method_name) + '"'
-                    field_method_db = self.sqlite.select_data(f'SELECT * FROM methods WHERE class_id = {class_db["class_id"]} AND method_name in ({field_method_name_str})')
+                    field_method_db = self.sqlite.select_data(f'SELECT method_id FROM methods WHERE class_id = {class_db["class_id"]} AND method_name in ({field_method_name_str})')
                     if field_method_db:
                         self._add_to_need_analyze_obj_list('java', f'{class_db["package_name"]}.{class_name}', None, None, commit_or_branch, class_db)
+                        class_node_id = self.view.create_node_category(class_name, 'entity', constant.NODE_TYPE_CLASS, constant.DIFF_TYPE_CHANGED, '', self.file_path, '', '', {})
             for field_db in fields_list:
                 node_id = self.view.create_node_category(class_name, field_db['field_name'], constant.NODE_TYPE_FIELD, constant.DIFF_TYPE_CHANGED, diff_content, class_filepath, field_db['documentation'], '', {})
                 field_db['field_node_id'] = node_id
                 self._add_to_need_analyze_obj_list('java', f'{class_db["package_name"]}.{class_name}', field_db['field_name'], None, commit_or_branch, field_db)
+                if class_node_id:
+                    self.view.create_node_link(node_id, class_node_id)
             for method_db in methods_list:
                 node_extend_dict = {'is_api': False}
                 if is_controller and method_db['is_api']:
                     node_extend_dict = {
                         'is_api': True,
                         'api_path': method_db['api_path']
                     }
                 method_name_param = f'{method_db["method_name"]}({",".join([param["parameter_type"] for param in json.loads(method_db["parameters"])])})'
-                node_id = self.view.create_node_category(class_name, method_name_param, constant.NODE_TYPE_METHOD, constant.DIFF_TYPE_CHANGED, diff_content, class_filepath, method_db['documentation'], method_db['body'], node_extend_dict)
+                node_id = self.view.create_node_category(class_name, method_name_param, constant.NODE_TYPE_METHOD, constant.DIFF_TYPE_CHANGED, diff_content, class_filepath, method_db.get('documentation'), method_db.get('body'), node_extend_dict)
                 method_db['method_node_id'] = node_id
                 self._add_to_need_analyze_obj_list('java', f'{class_db["package_name"]}.{class_name}', None, method_name_param, commit_or_branch, method_db)
 
     # Step 5
     def _impacted_analyze(self, need_analyze_obj: dict):
         file_type = need_analyze_obj['file_type']
         package_class = need_analyze_obj['package_class']
         commit_or_branch = need_analyze_obj['commit_or_branch']
         package_name = '.'.join(package_class.split('.')[0: -1])
         class_name = package_class.split('.')[-1]
-        class_db_list = self.sqlite.select_data(f'SELECT * FROM class WHERE project_id = {self.project_id} and class_name="{class_name}" and package_name="{package_name}"')
+        class_db_list = self.sqlite.select_data(f'SELECT class_id, filepath, commit_or_branch, is_controller, annotations, extends_class, implements '
+                                                f' FROM class WHERE project_id = {self.project_id} and class_name="{class_name}" and package_name="{package_name}"')
         class_entity = self._get_right_class_entity(class_db_list, commit_or_branch)
         if not class_entity:
             return
         class_filepath = class_entity['filepath']
         class_id = class_entity["class_id"]
         # gengxin
         commit_or_branch = class_entity['commit_or_branch']
         is_controller = class_entity['is_controller']
         # todo 粗查，待细化
         if file_type == 'xml':
             method_name = need_analyze_obj['method_param']
             mapper_method_node_id = need_analyze_obj['method_node_id']
-            impacted_methods = self.sqlite.select_data(f'SELECT * FROM methods WHERE class_id={class_id} and method_name="{method_name}"')
+            impacted_methods = self.sqlite.select_data(f'SELECT method_id, class_id, method_name, parameters, return_type, is_api, api_path, documentation, body '
+                                                       f'FROM methods WHERE class_id={class_id} and method_name="{method_name}"')
             if not impacted_methods:
                 return
             for impacted_method in impacted_methods:
                 node_extend_dict = {'is_api': False}
                 if is_controller and impacted_method['is_api']:
                     node_extend_dict = {
                         'is_api': True,
                         'api_path': impacted_method['api_path']
                     }
                 method_name_param = f'{impacted_method["method_name"]}({",".join([param["parameter_type"] for param in json.loads(impacted_method["parameters"])])})'
                 impacted_method_node_id = self.view.create_node_category(class_name, method_name_param,
                                                                          constant.NODE_TYPE_METHOD, constant.DIFF_TYPE_IMPACTED,
-                                                                         impacted_method['body'], class_filepath, impacted_method['documentation'],
-                                                                         impacted_method['body'], node_extend_dict)
+                                                                         impacted_method.get('body'), class_filepath, impacted_method.get('documentation'),
+                                                                         impacted_method.get('body'), node_extend_dict)
                 self.view.create_node_link(mapper_method_node_id, impacted_method_node_id)
                 extend_dict = {'method_node_id': impacted_method_node_id}
                 extend_dict.update(impacted_method)
                 self._add_to_need_analyze_obj_list('java', package_class, None, self._get_method_param_string(impacted_method), commit_or_branch, extend_dict)
         else:
             # analyze entity use
             entity_impacted_methods = []
+            entity_impacted_fields = []
             source_node_id = None
             if not need_analyze_obj.get('field_name') and not need_analyze_obj.get('method_param'):
                 class_node_id = self.view.create_node_category(class_name, 'entity', constant.NODE_TYPE_CLASS, constant.DIFF_TYPE_IMPACTED, '', self.file_path, '', '', {})
                 entity_impacted_methods = self._get_entity_invocation_in_methods_table(package_class)
+                entity_impacted_fields = self._get_entity_invocation_in_field_table(package_class)
                 source_node_id = class_node_id
             elif need_analyze_obj.get('field_name'):
                 annotations: list = json.loads(class_entity['annotations'])
-                entity_impacted_methods = self._get_field_invocation_in_methods_table(package_class, need_analyze_obj, annotations, commit_or_branch)
+                entity_impacted_methods = self._get_field_invocation_in_methods_table(package_class, need_analyze_obj, annotations, commit_or_branch, class_id)
                 source_node_id = need_analyze_obj.get('field_node_id')
             elif need_analyze_obj.get('method_param'):
                 method_param = need_analyze_obj.get('method_param')
                 method_name: str = method_param.split('(')[0]
                 method_node_id = need_analyze_obj.get('method_node_id')
                 source_node_id = method_node_id
                 entity_impacted_methods = self._get_method_invocation_in_methods_table(package_class, method_param, commit_or_branch)
-                method_db = self.sqlite.select_data(f'SELECT * FROM methods WHERE method_id = {need_analyze_obj.get("method_id")}')[0]
+                method_db = self.sqlite.select_data(f'SELECT annotations FROM methods WHERE method_id = {need_analyze_obj.get("method_id")}')[0]
                 is_override_method = 'Override' in method_db['annotations']
                 if is_override_method:
 
                     if class_entity['extends_class']:
-                        abstract_package_class = self._is_method_param_in_extends_package_class(method_param, class_entity['extends_class'], 'True', commit_or_branch)
+                        abstract_package_class, method_params = self._is_method_param_in_extends_package_class(method_param, class_entity['extends_class'], 'True', commit_or_branch)
                         if abstract_package_class:
-                            extends_methods = self._get_method_invocation_in_methods_table(abstract_package_class, method_param, commit_or_branch)
-                            for method in extends_methods:
-                                method['class_id'] = class_id
+                            extends_methods = self._get_method_invocation_in_methods_table(abstract_package_class, method_params, commit_or_branch)
+                            # for method in extends_methods:
+                            #     method['class_id'] = class_id
                             entity_impacted_methods += extends_methods
 
                     if class_entity['implements']:
                         class_implements = class_entity['implements'].split(',')
                         class_implements_obj = self.sqlite.select_data(f'''select c.package_name , c.class_name from methods m left join class c on c.class_id = m.class_id 
                                                 where c.project_id = {self.project_id} and m.method_name = '{method_name}' and c.class_name in ("{'","'.join(class_implements)}")''')
                         if class_implements_obj:
                             implements_package_class = class_implements_obj[0].get('package_name') + '.' + class_implements_obj[0].get('class_name')
-                            implements_methods = self._get_method_invocation_in_methods_table(implements_package_class, method_param, commit_or_branch)
-                            entity_impacted_methods += implements_methods
+                            implements_package_class, method_params = self._is_method_param_in_extends_package_class(method_param, implements_package_class, 'False', commit_or_branch)
+                            if implements_package_class:
+                                implements_methods = self._get_method_invocation_in_methods_table(implements_package_class, method_params, commit_or_branch)
+                                # implements_methods = self._get_method_invocation_in_methods_table(implements_package_class, method_param, commit_or_branch)
+                                entity_impacted_methods += implements_methods
                 else:
-                    class_method_db = self.sqlite.select_data(f'SELECT * FROM methods WHERE class_id = {class_id} and method_name = "{method_name}"')
+                    class_method_db = self.sqlite.select_data(f'SELECT method_id FROM methods WHERE class_id = {class_id} and method_name = "{method_name}"')
                     if not class_method_db:
-                        extends_package_class = self._is_method_param_in_extends_package_class(method_param, class_entity['extends_class'], 'False', commit_or_branch)
+                        extends_package_class, method_params = self._is_method_param_in_extends_package_class(method_param, class_entity['extends_class'], 'False', commit_or_branch)
                         if extends_package_class:
-                            extends_methods = self._get_method_invocation_in_methods_table(extends_package_class, method_param, commit_or_branch)
+                            extends_methods = self._get_method_invocation_in_methods_table(extends_package_class, method_params, commit_or_branch)
                             entity_impacted_methods += extends_methods
-            if not entity_impacted_methods:
-                return
             self._handle_impacted_methods(entity_impacted_methods, source_node_id)
+            self._handle_impacted_fields(entity_impacted_fields, source_node_id)
 
     def _is_method_param_in_extends_package_class(self, method_param, extends_package_class, is_abstract, commit_or_branch):
         method_name: str = method_param.split('(')[0]
+        method_arguments = method_param.split('(')[1].split(')')[0].split(',')
+        method_arguments = [ma for ma in method_arguments if ma]
         extends_package = '.'.join(extends_package_class.split('.')[0: -1])
         extends_class_name = extends_package_class.split('.')[-1]
-        extends_class_db = self.sqlite.select_data(f'SELECT * FROM class WHERE package_name = "{extends_package}" and class_name = "{extends_class_name}" and project_id = {self.project_id} and commit_or_branch = "{commit_or_branch}"')
+        extends_class_db = self.sqlite.select_data(f'SELECT class_id, extends_class FROM class WHERE package_name = "{extends_package}" and class_name = "{extends_class_name}" and project_id = {self.project_id} and commit_or_branch = "{commit_or_branch}"')
         if not extends_class_db:
-            extends_class_db = self.sqlite.select_data(f'SELECT * FROM class WHERE package_name = "{extends_package}" and class_name = "{extends_class_name}" and project_id = {self.project_id}')
+            extends_class_db = self.sqlite.select_data(f'SELECT class_id, extends_class FROM class WHERE package_name = "{extends_package}" and class_name = "{extends_class_name}" and project_id = {self.project_id}')
             if not extends_class_db:
-                return None
+                return None, None
         extends_class_id = extends_class_db[0]['class_id']
-        methods_db = self.sqlite.select_data(f'SELECT * FROM methods WHERE class_id = {extends_class_id} and method_name = "{method_name}" and is_abstract = "{is_abstract}"')
-        if methods_db:
-            return extends_package_class
-        else:
+        methods_db_list = self.sqlite.select_data(f'SELECT * FROM methods WHERE class_id = {extends_class_id} and method_name = "{method_name}" and is_abstract = "{is_abstract}"')
+        filter_methods = [method for method in methods_db_list if len(json.loads(method.get('parameters', '[]'))) == len(method_arguments)]
+        if not filter_methods:
             if extends_class_db[0]['extends_class']:
                 return self._is_method_param_in_extends_package_class(method_param, extends_class_db[0]['extends_class'], is_abstract, commit_or_branch)
             else:
-                return None
+                return None, None
+        if len(filter_methods) == 1:
+            method_db = filter_methods[0]
+            method_params = f'{method_db.get("method_name", method_name)}({",".join([param["parameter_type"] for param in json.loads(method_db.get("parameters", "[]"))])})'
+            return extends_package_class, method_params
+        else:
+            max_score = -float('inf')
+            max_score_method = None
+            for method_db in filter_methods:
+                method_db_params = [param["parameter_type"] for param in json.loads(method_db.get("parameters", "[]"))]
+                score = calculate_similar_score_method_params(method_arguments, method_db_params)
+                if score > max_score:
+                    max_score = score
+                    max_score_method = method_db
+            if max_score_method is None:
+                max_score_method = filter_methods[0]
+            method_params = f'{max_score_method.get("method_name", method_name)}({",".join([param["parameter_type"] for param in json.loads(max_score_method.get("parameters", "[]"))])})'
+            return extends_package_class, method_params
 
     def _get_extends_package_class(self, package_class):
         extends_package_class_list = []
-        extends_package_class_db = self.sqlite.select_data(f'SELECT * FROM class WHERE project_id = {self.project_id} AND extends_class="{package_class}"')
+        extends_package_class_db = self.sqlite.select_data(f'SELECT package_name, class_name FROM class WHERE project_id = {self.project_id} AND extends_class="{package_class}"')
         if extends_package_class_db:
             extends_package_class_list = [f'{class_item["package_name"]}.{class_item["class_name"]}' for class_item in extends_package_class_db]
             for extends_package_class in extends_package_class_list:
                 extends_package_class_list += self._get_extends_package_class(extends_package_class)
         return extends_package_class_list
 
     # Step 5.1
@@ -409,24 +438,28 @@
         right_class_entity = next((item for item in class_db_list if item.get("commit_or_branch") == commit_or_branch), None)
         if right_class_entity is None:
             right_class_entity = next((item for item in class_db_list if item.get("commit_or_branch") == self.commit_or_branch_new), None)
         return right_class_entity
 
     # Step 5.2
     def _get_entity_invocation_in_methods_table(self, package_class: str):
-        return self.sqlite.select_data(f'''SELECT * FROM methods WHERE project_id = {self.project_id} AND json_extract(method_invocation_map, '$."{package_class}".entity') IS NOT NULL''')
+        return self.sqlite.select_data(f'''SELECT method_id, class_id, method_name, parameters, return_type, is_api, api_path, documentation, body FROM methods WHERE project_id = {self.project_id} AND json_extract(method_invocation_map, '$."{package_class}".entity') IS NOT NULL''')
+
+    # Step 5.2
+    def _get_entity_invocation_in_field_table(self, package_class: str):
+        return self.sqlite.select_data(f'''SELECT field_id, class_id, annotations, field_type, field_name, is_static, documentation FROM field WHERE project_id = {self.project_id} AND field_type = "{package_class}"''')
 
     # Step 5.3
-    def _get_field_invocation_in_methods_table(self, package_class, field_obj, annotations, commit_or_branch):
+    def _get_field_invocation_in_methods_table(self, package_class, field_obj, annotations, commit_or_branch, class_id):
         is_static = field_obj['is_static']
         field_name = field_obj['field_name']
+        field_name_capitalize = field_name[0].upper() + field_name[1:]
         if not is_static:
             # todo static maybe has bug
             field_methods_set = set()
-            field_name_capitalize = field_name[0].upper() + field_name[1:]
             for annotation in annotations:
                 annotation_name = annotation.get('name')
                 if annotation_name == 'Data':
                     field_methods_set.add(f'get{field_name_capitalize}(')
                     field_methods_set.add(f'set{field_name_capitalize}(')
                 elif annotation_name == 'Getter':
                     field_methods_set.add(f'get{field_name_capitalize}(')
@@ -436,43 +469,47 @@
                     continue
             if not field_methods_set:
                 return []
             json_extract_sql_list = []
             for field_method in field_methods_set:
                 sql_part = f'''json_extract(method_invocation_map, '$."{package_class}".methods.keys(@.startsWith("{field_method}"))') IS NOT NULL'''
                 json_extract_sql_list.append(sql_part)
-            sql = f'SELECT * FROM methods WHERE project_id = {self.project_id} AND (' + ' OR '.join(json_extract_sql_list) + ')'
+            sql = f'SELECT method_id, class_id, method_name, parameters, return_type, is_api, api_path, documentation, body FROM methods WHERE project_id = {self.project_id} AND (' + ' OR '.join(json_extract_sql_list) + ')'
         else:
-            sql = f'''SELECT * FROM methods WHERE project_id = {self.project_id} AND json_extract(method_invocation_map, '$."{package_class}".fields.{field_name}') IS NOT NULL'''
+            sql = f'''SELECT method_id, class_id, method_name, parameters, return_type, is_api, api_path, documentation, body FROM methods 
+            WHERE project_id = {self.project_id} AND 
+            (json_extract(method_invocation_map, '$."{package_class}".fields.{field_name}') IS NOT NULL OR json_extract(method_invocation_map, '$."{package_class}.{field_name}"') IS NOT NULL)'''
         methods = self.sqlite.select_data(sql)
         if not methods:
-            return []
+            field_method_name_list = ['get' + field_name_capitalize, 'set' + field_name_capitalize, 'is' + field_name_capitalize]
+            field_method_name_str = '"' + '","'.join(field_method_name_list) + '"'
+            methods = self.sqlite.select_data(f'SELECT method_id, class_id, method_name, parameters, return_type, is_api, api_path, documentation, body FROM methods WHERE class_id = {class_id} AND method_name in ({field_method_name_str})')
         class_ids = [str(method['class_id']) for method in methods]
-        class_sql = f'SELECT * FROM class WHERE class_id in ({", ".join(class_ids)}) and commit_or_branch ="{commit_or_branch}"'
+        class_sql = f'SELECT class_id FROM class WHERE class_id in ({", ".join(class_ids)}) and commit_or_branch ="{commit_or_branch}"'
         class_db = self.sqlite.select_data(class_sql)
         class_db_id = [class_item['class_id'] for class_item in class_db]
         return [method for method in methods if method['class_id'] in class_db_id]
 
     # Step 5.4
     def _get_method_invocation_in_methods_table(self, package_class, method_param, commit_or_branch):
         all_possible_method_param_type_list = self._gen_all_possible_method_param_list(method_param)
         json_extract_sql_list = []
         for param_type in all_possible_method_param_type_list:
             sql_part = f'''json_extract(method_invocation_map, '$."{package_class}".methods."{param_type}"') IS NOT NULL'''
             json_extract_sql_list.append(sql_part)
         if len(json_extract_sql_list) > 1000:
             json_extract_sql_list = json_extract_sql_list[0: 995]
-        sql = f'SELECT * FROM methods WHERE project_id = {self.project_id} AND (' + ' OR '.join(json_extract_sql_list) + ')'
+        sql = f'SELECT method_id, class_id, method_name, parameters, return_type, is_api, api_path, documentation, body FROM methods WHERE project_id = {self.project_id} AND (' + ' OR '.join(json_extract_sql_list) + ')'
         logging.info(f'{package_class} {method_param} invocation sql: {sql}')
         methods = self.sqlite.select_data(sql)
         class_ids = [str(method['class_id']) for method in methods]
-        class_sql = f'SELECT * FROM class WHERE class_id in ({", ".join(class_ids)}) and commit_or_branch ="{commit_or_branch}"'
+        class_sql = f'SELECT class_id FROM class WHERE class_id in ({", ".join(class_ids)}) and commit_or_branch ="{commit_or_branch}"'
         class_db = self.sqlite.select_data(class_sql)
         if not class_db:
-            class_sql = f'SELECT * FROM class WHERE class_id in ({", ".join(class_ids)})'
+            class_sql = f'SELECT class_id FROM class WHERE class_id in ({", ".join(class_ids)})'
             class_db = self.sqlite.select_data(class_sql)
         class_db_id = [class_item['class_id'] for class_item in class_db]
         return [method for method in methods if method['class_id'] in class_db_id]
 
     # Step 5.4.1
     def _gen_all_possible_method_param_list(self, method_param):
         method_param_list = []
@@ -508,39 +545,50 @@
             if len(results) > 1000:
                 break
             if item not in replaced_list:
                 replaced_list.append(item)
                 self._replace_params_with_unknown(item['list'], results, item['index'], need_replace_list)
         return list(results)
 
+    def _replace_param_switch(self, param: str):
+        if 'int' in param.lower():
+            if param == 'int':
+                param = 'Integer'
+            else:
+                param = 'int'
+        else:
+            if param[0].isupper():
+                param = param[0].lower() + param[1:]
+            else:
+                param = param[0].upper() + param[1:]
+        return param
+
     def _replace_params_with_unknown(self, lst: list, results: set, idx: int, need_replace_list: list):
         # data = [item.split('<')[0].replace('<', '').replace('>', '') for item in data]
         for i in range(idx, len(lst)):
             new_lst = lst[:]
             results.add(tuple(new_lst))
+            new_lst2 = new_lst[:]
             if new_lst[i].lower() not in constant.JAVA_BASIC_TYPE:
-                new_lst2 = new_lst[:]
                 if new_lst[i].startswith('List'):
                     new_lst2[i] = 'ArrayList'
                 elif new_lst[i].startswith('Map'):
                     new_lst2[i] = 'HashMap'
                 elif new_lst[i].startswith('Set'):
                     new_lst2[i] = 'HashSet'
-                if tuple(new_lst2) not in results:
-                    results.add(tuple(new_lst2))
-                    if {'list': new_lst2, 'index': idx} not in need_replace_list:
-                        need_replace_list.append({'list': new_lst2, 'index': idx})
-            # else:
-            #     if new_lst[i][0].isupper() and new_lst[i] != 'String':
-            #         new_lst2 = new_lst[:]
-            #         new_lst2[i] = new_lst[i][0].lower() + new_lst[i][1:]
-            #         if tuple(new_lst2) not in results:
-            #             results.add(tuple(new_lst2))
-            #             if {'list': new_lst2, 'index': idx} not in need_replace_list:
-            #                 need_replace_list.append({'list': new_lst2, 'index': idx})
+            else:
+                if new_lst[i].lower() in constant.JAVA_BASIC_TYPE_SWITCH:
+                    new_lst2 = new_lst[:]
+                    param = self._replace_param_switch(new_lst[i])
+                    new_lst2[i] = param
+            if tuple(new_lst2) not in results:
+                results.add(tuple(new_lst2))
+                if {'list': new_lst2, 'index': idx} not in need_replace_list:
+                    need_replace_list.append({'list': new_lst2, 'index': idx})
+
             for el in ['null', 'unknown']:
                 new_lst_tmp = new_lst[:]
                 new_lst_tmp[i] = el
                 if tuple(new_lst_tmp) not in results:
                     results.add(tuple(new_lst_tmp))
                     if {'list': new_lst_tmp, 'index': min(idx, len(new_lst) - 1)} not in need_replace_list:
                         need_replace_list.append({'list': new_lst_tmp, 'index': min(idx, len(new_lst) - 1)})
@@ -548,32 +596,49 @@
     # Step 5.5
     def _get_method_param_string(self, method_db: dict):
         method_name: str = method_db['method_name']
         params: list = json.loads(method_db['parameters'])
         params_type_list = [param['parameter_type'] for param in params]
         return f'{method_name}({",".join(params_type_list)})'
 
+    def _handle_impacted_fields(self, impacted_fields: list, source_node_id):
+        for impacted_field in impacted_fields:
+            class_id = impacted_field['class_id']
+            class_entity = self.sqlite.select_data(f'SELECT package_name, class_name, commit_or_branch, filepath FROM class WHERE class_id={class_id}')[0]
+            class_name = class_entity['class_name']
+            package_name = class_entity['package_name']
+            package_class = f'{package_name}.{class_name}'
+            commit_or_branch = class_entity['commit_or_branch']
+            class_filepath = class_entity['filepath']
+            impacted_field_node_id = self.view.create_node_category(class_name, impacted_field['field_name'], constant.NODE_TYPE_FIELD, constant.DIFF_TYPE_IMPACTED, None, class_filepath, impacted_field['documentation'], '', {})
+            self.view.create_node_link(source_node_id, impacted_field_node_id)
+            extend_dict = {'field_node_id': impacted_field_node_id, 'class_filepath': class_filepath}
+            extend_dict.update(impacted_field)
+            self._add_to_need_analyze_obj_list('java', package_class, impacted_field['field_name'], None, commit_or_branch, extend_dict)
+            if impacted_field['is_static'] == 'False':
+                self._add_to_need_analyze_obj_list('java', package_class, None, None, commit_or_branch, class_entity)
+                class_node_id = self.view.create_node_category(class_name, 'entity', constant.NODE_TYPE_CLASS, constant.DIFF_TYPE_IMPACTED, '', self.file_path, '', '', {})
+                self.view.create_node_link(impacted_field_node_id, class_node_id)
+
     # Step 5.9
     def _handle_impacted_methods(self, impacted_methods: list, source_node_id):
         for impacted_method in impacted_methods:
-            node_extend_dict = {'is_api': False}
-            if impacted_method.get('is_api') == 'True':
-                node_extend_dict = {
-                    'is_api': True,
-                    'api_path': impacted_method['api_path']
-                }
+            is_api = impacted_method.get('is_api') == 'True'
+            node_extend_dict = impacted_method
+            node_extend_dict['is_api'] = is_api
             class_id = impacted_method['class_id']
-            class_entity = self.sqlite.select_data(f'SELECT * FROM class WHERE class_id={class_id}')[0]
+            class_entity = self.sqlite.select_data(f'SELECT package_name, class_name, commit_or_branch, filepath FROM class WHERE class_id={class_id}')[0]
             class_name = class_entity['class_name']
             package_name = class_entity['package_name']
             package_class = f'{package_name}.{class_name}'
             commit_or_branch = class_entity['commit_or_branch']
             class_filepath = class_entity['filepath']
+            node_extend_dict['class_annotations'] = class_entity['annotations']
             method_name_param = f'{impacted_method["method_name"]}({",".join([param["parameter_type"] for param in json.loads(impacted_method["parameters"])])})'
-            impacted_method_node_id = self.view.create_node_category(class_name, method_name_param, constant.NODE_TYPE_METHOD, constant.DIFF_TYPE_IMPACTED, impacted_method['body'], class_filepath, impacted_method['documentation'], impacted_method['body'], node_extend_dict)
+            impacted_method_node_id = self.view.create_node_category(class_name, method_name_param, constant.NODE_TYPE_METHOD, constant.DIFF_TYPE_IMPACTED, impacted_method.get('body'), class_filepath, impacted_method.get('documentation'), impacted_method.get('body'), node_extend_dict)
             self.view.create_node_link(source_node_id, impacted_method_node_id)
             extend_dict = {'method_node_id': impacted_method_node_id, 'class_filepath': class_filepath}
             extend_dict.update(impacted_method)
             self._add_to_need_analyze_obj_list('java', package_class, None, self._get_method_param_string(impacted_method), commit_or_branch, extend_dict)
 
     def _add_to_need_analyze_obj_list(self, file_type: str, package_class: str, field_name: str or None, method_param: str or None, commit_or_branch: str, mapper_extend_dict: dict):
         need_analyze_entity: dict = {
@@ -696,16 +761,14 @@
             os.system(f'git clone -b {self.branch_name} {self.git_url} {self.file_path}')
         self._occupy_project()
 
         logging.info('Git pull project to HEAD')
         os.system(f'cd {self.file_path} && git checkout {branch} && git pull')
         time.sleep(1)
 
-        self.xml_parse_results_new, self.xml_parse_results_old = self._parse_project(self.file_path, self.commit_or_branch_new, None)
-
         if not method_nums:
             method_nums_all = []
             # todo
             class_db = self.sqlite.select_data('SELECT * FROM class WHERE project_id = ' + str(self.project_id) + ' and filepath LIKE "%' + package_class + '"')
             if not class_db:
                 logging.error(f'Can not find {package_class} in db')
             class_id = class_db[0]['class_id']
@@ -719,8 +782,10 @@
         self.diff_parse_map[package_class] = {
             'line_num_added': method_nums_all,
             'line_content_added': method_nums_all,
             'line_num_removed': [],
             'line_content_removed': []
         }
 
+        self.xml_parse_results_new, self.xml_parse_results_old = self._parse_project(self.file_path, self.commit_or_branch_new, None)
+
         self._start_analysis_diff_and_impact()
```

### Comparing `jcci-0.1.5/src/jcci/database.py` & `jcci-0.2.0/src/jcci/database.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from .sql import create_tables
 
 logging.basicConfig(format='%(asctime)s %(message)s', level=logging.DEBUG)
 
 class SqliteHelper(object):
     def __init__(self, db_path):
         self.db_path = db_path
+        self.sql_result_map = {}
 
     def connect(self):
         try:
             if not os.path.exists(os.path.dirname(self.db_path)):
                 os.makedirs(os.path.dirname(self.db_path))
             if not os.path.exists(self.db_path):
                 db_file = open(self.db_path, "x")
@@ -66,22 +67,25 @@
             return class_id, True
         except Exception as e:
             logging.error(e)
             logging.error(f'add_class fail')
 
     def select_data(self, sql):
         try:
+            if sql in self.sql_result_map.keys():
+                return self.sql_result_map.get(sql)
             conn = self.connect()
             c = conn.cursor()
             cursor = c.execute(sql)
             res = cursor.fetchall()
             columns = cursor.description
             field = [column_name[0] for column_name in columns]
             zip_data = [dict(zip(field, item)) for item in res]
             conn.close()
+            self.sql_result_map[sql] = zip_data
             return zip_data
         except Exception as e:
             logging.error(f'select_data fail')
             raise e
 
     def update_data(self, sql):
         try:
```

### Comparing `jcci-0.1.5/src/jcci/diff_parse.py` & `jcci-0.2.0/src/jcci/diff_parse.py`

 * *Files identical despite different names*

### Comparing `jcci-0.1.5/src/jcci/graph.py` & `jcci-0.2.0/src/jcci/graph.py`

 * *Files 7% similar despite different names*

```diff
@@ -103,14 +103,18 @@
             changed_node['label'] = {
                 'show': True,
                 'formatter': changed_node["name"].split("(")[0]
             }
             tooltip = f'{changed_node["name"].split("(")[0]}<br>[Changed]{changed_node.get("diff_content", "")}'
             if changed_node.get('is_api'):
                 tooltip = tooltip + f'<br>[API]{changed_node.get("api_path")}'
+            if changed_node.get("annotations"):
+                tooltip += f'<br>[annotations]{changed_node.get("annotations", "")}'
+            if changed_node.get("class_annotations"):
+                tooltip += f'<br>[class_annotations]{changed_node.get("class_annotations", "")}'
             changed_node['tooltip'] = {
                 'show': True,
                 'position': 'right',
                 'formatter': tooltip
             }
             all_node.append(changed_node)
         max_link_count = max([value for key, value in result.items()]) if result else 1
@@ -126,21 +130,26 @@
             level_node_index = level_node_list.index(impacted_node['id']) if impacted_node['id'] in level_node_list else 1
             impacted_node['x'] = 100 + ((canvas_width - 100) / max_link_count) * (path_level + 1)
             impacted_node['y'] = (canvas_height / len(count_node_result.get(str(path_level), [1]))) * level_node_index
             impacted_node['label'] = {
                 'show': True,
                 'formatter': impacted_node["name"].split("(")[0]
             }
+            tooltip = f'{impacted_node["name"].split("(")[0]}'
             if impacted_node.get('is_api'):
-                tooltip = f'{impacted_node["name"].split("(")[0]}<br>[API]{impacted_node.get("api_path")}'
-                impacted_node['tooltip'] = {
-                    'show': True,
-                    'position': 'right',
-                    'formatter': tooltip
-                }
+                tooltip += f'<br>[API]{impacted_node.get("api_path")}'
+            if impacted_node.get("annotations"):
+                tooltip += f'<br>[annotations]{impacted_node.get("annotations", "")}'
+            if impacted_node.get("class_annotations"):
+                tooltip += f'<br>[class_annotations]{impacted_node.get("class_annotations", "")}'
+            impacted_node['tooltip'] = {
+                'show': True,
+                'position': 'right',
+                'formatter': tooltip
+            }
             all_node.append(impacted_node)
         self.nodes = all_node
 
 if __name__ == '__main__':
     data = [{'source': '62', 'target': '61'}, {'source': '63', 'target': '64'}, {'source': '63', 'target': '65'}, {'source': '63', 'target': '66'}, {'source': '63', 'target': '67'}, {'source': '9', 'target': '8'}, {'source': '68', 'target': '25'}, {'source': '21', 'target': '18'}, {'source': '21', 'target': '19'}, {'source': '26', 'target': '25'}, {'source': '27', 'target': '25'}, {'source': '72', 'target': '5'}, {'source': '72', 'target': '8'}, {'source': '72', 'target': '9'}, {'source': '73', 'target': '18'}, {'source': '73', 'target': '19'}, {'source': '73', 'target': '20'}, {'source': '73', 'target': '21'}, {'source': '74', 'target': '17'}, {'source': '74', 'target': '54'}, {'source': '75', 'target': '76'}, {'source': '75', 'target': '3'}, {'source': '75', 'target': '77'}, {'source': '75', 'target': '5'}, {'source': '75', 'target': '78'}, {'source': '75', 'target': '79'}, {'source': '75', 'target': '6'}, {'source': '75', 'target': '80'}, {'source': '75', 'target': '8'}, {'source': '75', 'target': '9'}, {'source': '75', 'target': '81'}, {'source': '46', 'target': '47'}, {'source': '46', 'target': '60'}, {'source': '47', 'target': '61'}, {'source': '48', 'target': '47'}, {'source': '49', 'target': '46'}, {'source': '50', 'target': '46'}, {'source': '83', 'target': '17'}, {'source': '83', 'target': '18'}, {'source': '54', 'target': '17'}, {'source': '55', 'target': '18'}, {'source': '56', 'target': '55'}, {'source': '57', 'target': '55'}, {'source': '58', 'target': '56'}, {'source': '58', 'target': '57'}, {'source': '59', 'target': '54'}, {'source': '59', 'target': '55'}, {'source': '59', 'target': '56'}, {'source': '59', 'target': '57'}, {'source': '64', 'target': '66'}, {'source': '65', 'target': '64'}]
     bb = max_relationship_length(data)
```

### Comparing `jcci-0.1.5/src/jcci/java_parse.py` & `jcci-0.2.0/src/jcci/java_parse.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,45 @@
 import os
+import sys
 import logging
 import json
 import javalang
+from concurrent.futures import ThreadPoolExecutor, as_completed
 from .database import SqliteHelper
-from .constant import ENTITY, RETURN_TYPE, PARAMETERS, BODY, METHODS, FIELDS, PARAMETER_TYPE_METHOD_INVOCATION_UNKNOWN, JAVA_BASIC_TYPE, MAPPING_LIST
+from .constant import ENTITY, RETURN_TYPE, PARAMETERS, BODY, METHODS, FIELDS, \
+    PARAMETER_TYPE_METHOD_INVOCATION_UNKNOWN, JAVA_BASIC_TYPE, MAPPING_LIST, JAVA_UTIL_TYPE
+from . import config as config
 
+sys.setrecursionlimit(10000)
 logging.basicConfig(format='%(asctime)s %(message)s', level=logging.DEBUG)
 
+
+def calculate_similar_score_method_params(except_method_param_list, method_param_list):
+    score = 0
+    positions = {}
+
+    # 记录list1中每个元素的位置
+    for i, item in enumerate(except_method_param_list):
+        positions[item] = i
+
+    # 遍历list2,计算分数
+    for i, item in enumerate(method_param_list):
+        if item in positions:
+            score += 1
+            score -= abs(i - positions[item])
+
+    return score
+
+
 class JavaParse(object):
     def __init__(self, db_path, project_id):
         self.project_id = project_id
         self.sqlite = SqliteHelper(db_path)
+        self.sibling_dirs = []
+        self.parsed_filepath = []
 
     def _handle_extends(self, extends, import_list: list, package_name):
         if isinstance(extends, list):
             extends_package_class_list = []
             extends_class = extends[0].name
             extends_package_class = self._get_extends_class_full_package(extends_class, import_list, package_name)
             extends_package_class_list.append(extends_package_class)
@@ -36,35 +61,33 @@
             extends_class = self._get_extends_class_full_package(extends.name, import_list, package_name)
             return extends_class, [extends_class]
 
     def _get_extends_class_full_package(self, extends_class, import_list, package_name):
         extends_in_imports = [import_obj for import_obj in import_list if extends_class in import_obj['import_path']]
         return extends_in_imports[0]['import_path'] if extends_in_imports else package_name + '.' + extends_class
 
-    def _parse_class(self, node, filepath: str, package_name: str, import_list: list, commit_or_branch: str):
+    def _parse_class(self, node, filepath: str, package_name: str, import_list: list, commit_or_branch: str, parse_import_first):
         # 处理class信息
         documentation = node.documentation
         class_name = node.name
         package_class = package_name + '.' + node.name
         class_type = type(node).__name__.replace('Declaration', '')
         access_modifier = [m for m in list(node.modifiers) if m.startswith('p')][0] if list([m for m in list(node.modifiers) if m.startswith('p')]) else 'public'
         annotations_json = json.dumps(node.annotations, default=lambda obj: obj.__dict__)
         is_controller, controller_base_url = self._judge_is_controller(node.annotations)
         extends_package_class = None
         if 'extends' in node.attrs and node.extends:
             extends_package_class, extends_package_class_list = self._handle_extends(node.extends, import_list, package_name)
             package_path = package_class.replace('.', '/') + '.java'
             base_filepath = filepath.replace(package_path, '')
             for extends_package_class_item in extends_package_class_list:
-                extends_package = '.'.join(extends_package_class_item.split('.')[0: -1])
-                extends_class_name = extends_package_class_item.split('.')[-1]
+                if extends_package_class_item == package_class:
+                    continue
                 extends_class_filepath = base_filepath + extends_package_class_item.replace('.', '/') + '.java'
-                extends_class_db = self.sqlite.select_data(f'SELECT * FROM class WHERE project_id={self.project_id} and package_name = "{extends_package}" and class_name = "{extends_class_name}" and filepath= "{extends_class_filepath}"')
-                if not extends_class_db:
-                    self.parse_java_file(extends_class_filepath, commit_or_branch)
+                self.parse_java_file(extends_class_filepath, commit_or_branch, parse_import_first=parse_import_first)
         implements = ','.join([implement.name for implement in node.implements]) if 'implements' in node.attrs and node.implements else None
         class_id, new_add = self.sqlite.add_class(filepath.replace('\\', '/'), access_modifier, class_type, class_name, package_name, extends_package_class, self.project_id, implements, annotations_json, documentation, is_controller, controller_base_url, commit_or_branch)
         return class_id, new_add
 
     def _parse_imports(self, imports):
         import_list = []
         for import_decl in imports:
@@ -74,31 +97,53 @@
                 'is_wildcard': import_decl.wildcard,
                 'start_line': import_decl.position.line,
                 'end_line': import_decl.position.line
             }
             import_list.append(import_obj)
         return import_list
 
-    def _parse_fields(self, fields, package_name, class_id, import_map):
+    def _parse_fields(self, fields, package_name, class_name, class_id, import_map, filepath):
         field_list = []
+        package_class = package_name + "." + class_name
         for field_obj in fields:
             field_annotations = json.dumps(field_obj.annotations, default=lambda obj: obj.__dict__)
-            access_modifier = [m for m in list(field_obj.modifiers) if m.startswith('p')][0] if list([m for m in list(field_obj.modifiers) if m.startswith('p')]) else 'public'
+            access_modifier = next((m for m in list(field_obj.modifiers) if m.startswith('p')), 'public')
             field_name = field_obj.declarators[0].name
             field_type: str = field_obj.type.name
-            if field_type.lower() not in JAVA_BASIC_TYPE:
-                if field_type in import_map.keys():
-                    field_type = import_map.get(field_type)
+            if field_type.lower() in JAVA_BASIC_TYPE:
+                pass
+            elif field_type in JAVA_UTIL_TYPE and ('java.util' in import_map.values() or 'java.util.' + field_type in import_map.values()):
+                var_declarator_type_arguments = self._deal_arguments_type(field_obj.type.arguments, FIELDS, {}, {}, {}, import_map, {}, package_name, filepath, [], {}, class_id)
+                if var_declarator_type_arguments:
+                    field_type = field_type + '<' + '#'.join(var_declarator_type_arguments) + '>'
+            elif field_type in import_map.keys():
+                field_type = import_map.get(field_type)
+            else:
+                in_import = False
+                for key in import_map.keys():
+                    if key[0].isupper():
+                        continue
+                    field_type_db = self.sqlite.select_data(f'select class_id from class where project_id={self.project_id} and package_name = "{import_map.get(key)}" and class_name = "{field_type}" limit 1')
+                    if field_type_db:
+                        field_type = f'{import_map.get(key)}.{field_type}'
+                        in_import = True
+                        break
+                if not in_import:
+                    field_type_db = self.sqlite.select_data(f'select class_id from class where project_id={self.project_id} and package_name = "{package_class}" and class_name = "{field_type}" limit 1')
+                    if field_type_db:
+                        field_type = f'{package_class}.{field_type}'
+                    else:
+                        field_type = package_name + '.' + field_type
+                    import_map[field_obj.type.name] = field_type
                 else:
-                    import_map[field_obj.type.name] = package_name + '.' + field_obj.type.name
-                    field_type = package_name + '.' + field_type
+                    import_map[field_obj.type.name] = field_type
             is_static = 'static' in list(field_obj.modifiers)
             documentation = field_obj.documentation
             start_line = field_obj.position.line if not field_obj.annotations else field_obj.annotations[0].position.line
-            end_line = field_obj.position.line
+            end_line = self._get_method_end_line(field_obj)
             field_obj = {
                 'class_id': class_id,
                 'project_id': self.project_id,
                 'annotations': field_annotations,
                 'access_modifier': access_modifier,
                 'field_type': field_type,
                 'field_name': field_name,
@@ -108,126 +153,270 @@
                 'end_line': end_line
             }
             field_list.append(field_obj)
         self.sqlite.update_data(f'DELETE FROM field where class_id={class_id}')
         self.sqlite.insert_data('field', field_list)
         return field_list
 
+    def _parse_method_body_variable(self, node, parameters_map, variable_map, field_map, import_map, method_invocation, package_name, filepath, methods, method_name_entity_map, class_id):
+        var_declarator = node.declarators[0].name
+        var_declarator_type = self._deal_declarator_type(node.type, BODY, parameters_map, variable_map, field_map, import_map, method_invocation, package_name, filepath, methods, method_name_entity_map, class_id)
+        variable_map[var_declarator] = var_declarator_type
+        initializer = node.declarators[0].initializer
+        if self._is_valid_prefix(var_declarator_type):
+            self._add_entity_used_to_method_invocation(method_invocation, var_declarator_type, BODY)
+        if not initializer:
+            return var_declarator_type
+        for init_path, init_node in initializer.filter(javalang.tree.MemberReference):
+            self._deal_member_reference(init_node, parameters_map, variable_map, field_map, import_map, method_invocation, BODY, package_name, filepath)
+        return var_declarator_type
+
+    def _parse_method_body_class_creator(self, node, parameters_map, variable_map, field_map, import_map, method_invocation, package_name, filepath, methods, method_name_entity_map, class_id):
+        qualifier = node.type.name
+        node_line = node.position.line if node.position else None
+        qualifier_type = self._get_var_type(qualifier, parameters_map, variable_map, field_map, import_map, method_invocation, BODY, package_name, filepath)
+        node_arguments = self._deal_var_type(node.arguments, BODY, parameters_map, variable_map, field_map, import_map, method_invocation, package_name, filepath, methods, method_name_entity_map, class_id)
+        if node.selectors is None or not node_arguments:
+            self._add_entity_used_to_method_invocation(method_invocation, qualifier_type, BODY)
+        else:
+            if node_arguments:
+                qualifier_package_class, method_params, method_db = self._find_method_in_package_class(qualifier_type, qualifier, node_arguments)
+                if not method_db:
+                    return qualifier_type
+                self._add_method_used_to_method_invocation(method_invocation, qualifier_type, method_params, [node_line])
+            self._parse_node_selectors(node.selectors, qualifier_type, parameters_map, variable_map, field_map, import_map, method_invocation, package_name, filepath, methods, method_name_entity_map, class_id)
+        if self._is_valid_prefix(qualifier_type):
+            self._add_entity_used_to_method_invocation(method_invocation, qualifier_type, BODY)
+        return qualifier_type
+
+    def _parse_method_body_method_invocation(self, node, parameters_map, variable_map, field_map, import_map, method_invocation, package_name, filepath, methods, method_name_entity_map, class_id):
+        qualifier = node.qualifier
+        member = node.member
+        return_type = PARAMETER_TYPE_METHOD_INVOCATION_UNKNOWN
+        # 类静态方法调用
+        if not qualifier and not member[0].islower():
+            qualifier_type = self._get_var_type(member, parameters_map, variable_map, field_map, import_map, method_invocation, BODY, package_name, filepath)
+            # todo a.b.c
+            qualifier_type = self._parse_node_selectors(node.selectors, qualifier_type, parameters_map, variable_map, field_map, import_map, method_invocation, package_name, filepath, methods, method_name_entity_map, class_id)
+            return_type = qualifier_type
+        elif qualifier:
+            qualifier_type = self._get_var_type(qualifier, parameters_map, variable_map, field_map, import_map, method_invocation, BODY, package_name, filepath)
+            node_arguments = self._deal_var_type(node.arguments, BODY, parameters_map, variable_map, field_map, import_map, method_invocation, package_name, filepath, methods, method_name_entity_map, class_id)
+            node_line = node.position.line
+            node_arguments = [n for n in node_arguments if n]
+            node_method = f'{member}({",".join(node_arguments)})'
+            self._add_method_used_to_method_invocation(method_invocation, qualifier_type, node_method, [node_line])
+            if self._is_valid_prefix(qualifier_type):
+                qualifier_package_class, method_params, method_db = self._find_method_in_package_class(qualifier_type, member, node_arguments)
+                if not method_db:
+                    return qualifier_type
+                if method_params != node_method:
+                    self._add_method_used_to_method_invocation(method_invocation, qualifier_type, method_params, [node_line])
+                method_db_type = method_db.get("return_type", method_db.get("field_type"))
+            elif qualifier_type.startswith('Map<') and member == 'get':
+                method_db_type = qualifier_type.split('#')[1].split('>')[0]
+            else:
+                method_db_type = qualifier_type
+            method_db_type = self._parse_node_selectors(node.selectors, method_db_type, parameters_map, variable_map, field_map, import_map, method_invocation, package_name, filepath, methods, method_name_entity_map, class_id)
+            return_type = method_db_type
+        # 在一个类的方法或父类方法
+        elif member:
+            class_db = self.sqlite.select_data(f'SELECT package_name, class_name, extends_class FROM class where project_id = {self.project_id} and class_id={class_id} limit 1')[0]
+            package_class = class_db['package_name'] + '.' + class_db['class_name']
+            node_line = node.position.line
+            node_arguments = self._deal_var_type(node.arguments, BODY, parameters_map, variable_map, field_map, import_map, method_invocation, package_name, filepath, methods, method_name_entity_map, class_id)
+            # todo 同级方法, 判断参数长度，不精确
+            if method_name_entity_map.get(member):
+                same_class_method = None
+                max_score = -float('inf')
+                for method_item in methods:
+                    if method_item.name != member or len(node.arguments) != len(method_item.parameters):
+                        continue
+                    method_item_param_types = [self._deal_declarator_type(parameter.type, PARAMETERS, parameters_map, variable_map, field_map, import_map, method_invocation, package_name, filepath, methods, method_name_entity_map, class_id) for parameter in method_item.parameters]
+                    score = calculate_similar_score_method_params(node_arguments, method_item_param_types)
+                    if score > max_score:
+                        max_score = score
+                        same_class_method = method_item
+                if same_class_method:
+                    node_arguments = self._deal_var_type(same_class_method.parameters, BODY, parameters_map, variable_map, field_map, import_map, method_invocation, package_name, filepath, methods, method_name_entity_map, class_id)
+                    node_method = f'{member}({",".join(node_arguments)})'
+                    self._add_method_used_to_method_invocation(method_invocation, package_class, node_method, [node_line])
+                    return_type = self._deal_declarator_type(same_class_method.return_type, BODY, parameters_map, variable_map, field_map, import_map, method_invocation, package_name, filepath, methods, method_name_entity_map, class_id)
+            # todo 继承方法
+            elif class_db['extends_class']:
+                extends_package_class, method_params, method_db = self._find_method_in_package_class(class_db['extends_class'], member, node_arguments)
+                if extends_package_class:
+                    self._add_method_used_to_method_invocation(method_invocation, extends_package_class, method_params, [node_line])
+                    return_type = method_db.get("return_type", method_db.get("field_type"))
+        return return_type
+
+    def _parse_node_selectors(self, selectors, qualifier_type, parameters_map, variable_map, field_map, import_map, method_invocation, package_name, filepath, methods, method_name_entity_map, class_id):
+        if not selectors:
+            return qualifier_type
+        selector_qualifier_type = qualifier_type
+        for selector in selectors:
+            if type(selector) == javalang.tree.ArraySelector:
+                continue
+            selector_member = selector.member
+            if type(selector) == javalang.tree.MethodInvocation:
+                self._parse_method_body_method_invocation(selector, parameters_map, variable_map, field_map, import_map, method_invocation, package_name, filepath, methods, method_name_entity_map, class_id)
+                selector_arguments = self._deal_var_type(selector.arguments, BODY, parameters_map, variable_map, field_map, import_map, method_invocation, package_name, filepath, methods, method_name_entity_map, class_id)
+                selector_line = selector.position.line
+                selector_method = f'{selector_member}({",".join(selector_arguments)})'
+                if self._is_valid_prefix(selector_qualifier_type):
+                    self._add_method_used_to_method_invocation(method_invocation, selector_qualifier_type, selector_method, [selector_line])
+                selector_package_class, method_params, method_db = self._find_method_in_package_class(selector_qualifier_type, selector_member, selector_arguments)
+                if not method_db:
+                    continue
+                method_db_type = method_db.get("return_type", method_db.get("field_type"))
+                selector_qualifier_type = method_db_type
+            elif type(selector) == javalang.tree.MemberReference:
+                self._deal_member_reference(selector, parameters_map, variable_map, field_map, import_map, method_invocation, BODY, package_name, filepath)
+                selector_qualifier_type = self._get_var_type(selector_member, parameters_map, variable_map, field_map, import_map, method_invocation, BODY, package_name, filepath)
+                if self._is_valid_prefix(selector_qualifier_type):
+                    self._add_field_used_to_method_invocation(method_invocation, selector_qualifier_type, selector_member, [None])
+        return selector_qualifier_type
+
+    def _parse_enum(self, enum_body, lines, class_id, import_map, field_map, package_name, filepath):
+        constants = enum_body.constants
+        field_list = []
+        init_line = 0
+        for constant in constants:
+            constant_type = 'ENUM'
+            constant_name = constant.name
+            arguments = constant.arguments
+            start_text = constant_name if not arguments else constant_name + '('
+            start_lines = [lines.index(line) for line in lines if line.strip().startswith(start_text)]
+            if start_lines:
+                start_line = start_lines[0] + 1
+                init_line = start_line
+            else:
+                start_line = init_line
+            end_line = start_line
+            field_obj = {
+                'class_id': class_id,
+                'project_id': self.project_id,
+                'annotations': None,
+                'access_modifier': 'public',
+                'field_type': constant_type,
+                'field_name': constant_name,
+                'is_static': True,
+                'documentation': None,
+                'start_line': start_line,
+                'end_line': end_line
+            }
+            field_list.append(field_obj)
+        self.sqlite.insert_data('field', field_list)
+
+    def _parse_constructors(self, constructors, lines, class_id, import_map, field_map, package_name, filepath):
+        all_method = []
+        for constructor in constructors:
+            method_invocation = {}
+            cs_name = constructor.name
+            annotations = json.dumps(constructor.annotations, default=lambda obj: obj.__dict__)  # annotations
+
+            access_modifier = [m for m in list(constructor.modifiers) if m.startswith('p')][0] if list([m for m in list(constructor.modifiers) if m.startswith('p')]) else 'public'
+            parameters = []
+            parameters_map = {}
+            for parameter in constructor.parameters:
+                parameter_obj = {
+                    'parameter_type': self._deal_declarator_type(parameter.type, PARAMETERS, parameters_map, {}, field_map, import_map, method_invocation, package_name, filepath, [], {}, class_id),
+                    'parameter_name': parameter.name,
+                    'parameter_varargs': parameter.varargs
+                }
+                parameters.append(parameter_obj)
+            parameters_map = {parameter['parameter_name']: parameter['parameter_type'] for parameter in parameters}
+            return_type = package_name + '.' + cs_name
+            start_line = constructor.position.line
+            if constructor.annotations:
+                start_line = constructor.annotations[0].position.line
+            end_line = self._get_method_end_line(constructor)
+            cs_body = lines[start_line - 1: end_line + 1]
+            for body in constructor.body:
+                for path, node in body.filter(javalang.tree.This):
+                    self._parse_node_selectors(node.selectors, None, {}, {}, field_map, import_map, method_invocation, package_name, filepath, [], {}, class_id)
+
+            method_db = {
+                'class_id': class_id,
+                'project_id': self.project_id,
+                'annotations': annotations,
+                'access_modifier': access_modifier,
+                'return_type': return_type,
+                'method_name': cs_name,
+                'parameters': json.dumps(parameters),
+                'body': json.dumps(cs_body),
+                'method_invocation_map': json.dumps(method_invocation),
+                'is_static': False,
+                'is_abstract': False,
+                'is_api': False,
+                'api_path': None,
+                'start_line': start_line,
+                'end_line': end_line,
+                'documentation': constructor.documentation
+            }
+            all_method.append(method_db)
+        self.sqlite.insert_data('methods', all_method)
+
     def _parse_method(self, methods, lines, class_id, import_map, field_map, package_name, filepath):
         # 处理 methods
         all_method = []
-        class_db = self.sqlite.select_data(f'SELECT * FROM class WHERE class_id = {class_id}')[0]
+        class_db = self.sqlite.select_data(f'SELECT controller_base_url FROM class WHERE project_id = {self.project_id} and class_id = {class_id}')[0]
         base_url = class_db['controller_base_url'] if class_db['controller_base_url'] else ''
         method_name_entity_map = {method.name: method for method in methods}
         for method_obj in methods:
             method_invocation = {}
             variable_map = {}
             method_name = method_obj.name
             documentation = method_obj.documentation  # document
             annotations = json.dumps(method_obj.annotations, default=lambda obj: obj.__dict__)  # annotations
             is_api, api_path = self._judge_is_api(method_obj.annotations, base_url, method_name)
             access_modifier = [m for m in list(method_obj.modifiers) if m.startswith('p')][0] if list([m for m in list(method_obj.modifiers) if m.startswith('p')]) else 'public'
             is_static = 'static' in list(method_obj.modifiers)
             is_abstract = 'abstract' in list(method_obj.modifiers)
-            # 处理返回对象
-            return_type = self._deal_declarator_type(method_obj.return_type, import_map, method_invocation, RETURN_TYPE, package_name, filepath)
-            method_start_line = method_obj.position.line
-            if method_obj.annotations:
-                method_start_line = method_obj.annotations[0].position.line
-            method_end_line = self._get_method_end_line(method_obj)
-            method_body = lines[method_start_line - 1: method_end_line + 1]
-            # 处理参数
             parameters = []
+            parameters_map = {}
+            type_parameters = method_obj.type_parameters if method_obj.type_parameters else []
+            for type_parameter in type_parameters:
+                type_parameter_name = type_parameter.name
+                type_parameter_extends_name = type_parameter.extends[0].name if type_parameter.extends else None
+                if type_parameter_extends_name:
+                    type_parameter_extends_name_type = self._deal_declarator_type(type_parameter.extends[0], PARAMETERS, parameters_map, variable_map, field_map, import_map, method_invocation, package_name, filepath, methods, method_name_entity_map, class_id)
+                else:
+                    type_parameter_extends_name_type = type_parameter_name
+                parameters_map[type_parameter_name] = type_parameter_extends_name_type
             for parameter in method_obj.parameters:
                 parameter_obj = {
-                    'parameter_type': self._deal_declarator_type(parameter.type, import_map, method_invocation, PARAMETERS, package_name, filepath),
+                    'parameter_type': self._deal_declarator_type(parameter.type, PARAMETERS, parameters_map, variable_map, field_map, import_map, method_invocation, package_name, filepath, methods, method_name_entity_map, class_id),
                     'parameter_name': parameter.name,
                     'parameter_varargs': parameter.varargs
                 }
                 parameters.append(parameter_obj)
-            parameters_map = {parameter['parameter_name']: parameter['parameter_type'] for parameter in parameters}
+            parameters_map.update({parameter['parameter_name']: parameter['parameter_type'] for parameter in parameters})
+            # 处理返回对象
+            return_type = self._deal_declarator_type(method_obj.return_type, RETURN_TYPE, parameters_map, variable_map, field_map, import_map, method_invocation, package_name, filepath, methods, method_name_entity_map, class_id)
+            if self._is_valid_prefix(return_type):
+                self._add_entity_used_to_method_invocation(method_invocation, return_type, RETURN_TYPE)
+            method_start_line = method_obj.position.line
+            if method_obj.annotations:
+                method_start_line = method_obj.annotations[0].position.line
+            method_end_line = self._get_method_end_line(method_obj)
+            method_body = lines[method_start_line - 1: method_end_line + 1]
 
             # 处理方法体
-            if method_obj.body:
-                for body in method_obj.body:
-                    for path, node in body.filter(javalang.tree.VariableDeclaration):
-                        var_declarator = node.declarators[0].name
-                        var_declarator_type = self._deal_declarator_type(node.type, import_map, method_invocation, BODY, package_name, filepath)
-                        variable_map[var_declarator] = var_declarator_type
-                    for path, node in body.filter(javalang.tree.ClassCreator):
-                        qualifier = node.type.name
-                        qualifier_type = self._get_var_type(qualifier, parameters_map, variable_map, field_map, import_map, method_invocation, BODY, package_name, filepath)
-                        if node.selectors is None:
-                            self._add_entity_used_to_method_invocation(method_invocation, qualifier_type, BODY)
-                        else:
-                            for selector in node.selectors:
-                                if type(selector) != javalang.tree.MethodInvocation:
-                                    continue
-                                selector_member = selector.member
-                                selector_arguments = self._deal_var_type(selector.arguments, parameters_map, variable_map, field_map, import_map, method_invocation, BODY, package_name, filepath)
-                                selector_line = selector.position.line
-                                selector_method = f'{selector_member}({",".join(selector_arguments)})'
-                                self._add_method_used_to_method_invocation(method_invocation, qualifier_type, selector_method, [selector_line])
-                    for path, node in body.filter(javalang.tree.MethodInvocation):
-                        qualifier = node.qualifier
-                        member = node.member
-                        # 类静态方法调用
-                        if not qualifier and not member[0].islower():
-                            qualifier_type = self._get_var_type(member, parameters_map, variable_map, field_map, import_map, method_invocation, BODY, package_name, filepath)
-                            # todo a.b.c
-                            if node.selectors is None:
-                                continue
-                            for selector in node.selectors:
-                                selector_member = selector.member
-                                selector_arguments = self._deal_var_type(selector.arguments, parameters_map, variable_map, field_map, import_map, method_invocation, BODY, package_name, filepath)
-                                selector_line = selector.position.line
-                                selector_method = f'{selector_member}({",".join(selector_arguments)})'
-                                self._add_method_used_to_method_invocation(method_invocation, qualifier_type, selector_method, [selector_line])
-                        elif qualifier:
-                            qualifier_type = self._get_var_type(qualifier, parameters_map, variable_map, field_map, import_map, method_invocation, BODY, package_name, filepath)
-                            node_arguments = self._deal_var_type(node.arguments, parameters_map, variable_map, field_map, import_map, method_invocation, BODY, package_name, filepath)
-                            node_line = node.position.line
-                            node_method = f'{member}({",".join(node_arguments)})'
-                            self._add_method_used_to_method_invocation(method_invocation, qualifier_type, node_method, [node_line])
-                        # 在一个类的方法或父类方法
-                        elif member:
-                            class_db = self.sqlite.select_data(f'SELECT * FROM class where class_id={class_id} limit 1')[0]
-                            package_class = class_db['package_name'] + '.' + class_db['class_name']
-                            node_line = node.position.line
-                            node_arguments = self._deal_var_type(node.arguments, parameters_map, variable_map, field_map, import_map, method_invocation, BODY, package_name, filepath)
-                            # todo 同级方法, 判断参数长度，不精确
-                            if method_name_entity_map.get(member):
-                                same_class_method = None
-                                max_score = -float('inf')
-                                for method_item in methods:
-                                    if method_item.name != member or len(node.arguments) != len(method_item.parameters):
-                                        continue
-                                    method_item_param_types = [self._deal_declarator_type(parameter.type, import_map, method_invocation, PARAMETERS, package_name, filepath) for parameter in method_item.parameters]
-                                    score = self._calculate_similar_score_method_params(node_arguments, method_item_param_types)
-                                    if score > max_score:
-                                        max_score = score
-                                        same_class_method = method_item
-                                if same_class_method:
-                                    node_arguments = self._deal_var_type(same_class_method.parameters, parameters_map, variable_map, field_map, import_map, method_invocation, BODY, package_name, filepath)
-                                    node_method = f'{member}({",".join(node_arguments)})'
-                                    self._add_method_used_to_method_invocation(method_invocation, package_class, node_method, [node_line])
-                            # todo 继承方法
-                            elif class_db['extends_class']:
-                                extends_package_class, method_params = self._find_method_in_extends(class_db['extends_class'], member, node_arguments)
-                                if extends_package_class:
-                                    self._add_method_used_to_method_invocation(method_invocation, extends_package_class, method_params, [node_line])
-
-                    # for path, node in body.filter(javalang.tree.SuperMethodInvocation):
-                    #     print(node)
-                    # for path, node in body.filter(javalang.tree.TypeArgument):
-                    #     print(node)
-                    # for path, node in body.filter(javalang.tree.TypeParameter):
-                    #     print(node)
-                    # for path, node in body.filter(javalang.tree.FieldDeclaration):
-                    #     print(node)
+            if not method_obj.body:
+                method_obj.body = []
+            for body in method_obj.body:
+                for path, node in body.filter(javalang.tree.VariableDeclaration):
+                    self._parse_method_body_variable(node, parameters_map, variable_map, field_map, import_map, method_invocation, package_name, filepath, methods, method_name_entity_map, class_id)
+                for path, node in body.filter(javalang.tree.ClassCreator):
+                    self._parse_method_body_class_creator(node, parameters_map, variable_map, field_map, import_map, method_invocation, package_name, filepath, methods, method_name_entity_map, class_id)
+                for path, node in body.filter(javalang.tree.This):
+                    self._parse_node_selectors(node.selectors, None, parameters_map, variable_map, field_map, import_map, method_invocation, package_name, filepath, methods, method_name_entity_map, class_id)
+                for path, node in body.filter(javalang.tree.MethodInvocation):
+                    self._parse_method_body_method_invocation(node, parameters_map, variable_map, field_map, import_map, method_invocation, package_name, filepath, methods, method_name_entity_map, class_id)
             method_db = {
                 'class_id': class_id,
                 'project_id': self.project_id,
                 'annotations': annotations,
                 'access_modifier': access_modifier,
                 'return_type': return_type,
                 'method_name': method_name,
@@ -242,78 +431,67 @@
                 'end_line': method_end_line,
                 'documentation': documentation
             }
             all_method.append(method_db)
         self.sqlite.update_data(f'DELETE FROM methods where class_id={class_id}')
         self.sqlite.insert_data('methods', all_method)
 
-    def _find_method_in_extends(self, extend_package_class: str, method_name: str, method_arguments):
-        if not extend_package_class:
-            return None, None
+    def _find_method_in_package_class(self, package_class: str, method_name: str, method_arguments):
+        if not package_class or not self._is_valid_prefix(package_class):
+            return None, None, None
         # 查表有没有记录
-        extend_package = '.'.join(extend_package_class.split('.')[0: -1])
-        extend_class = extend_package_class.split('.')[-1]
-        extend_class_db = self.sqlite.select_data(f'SELECT * FROM class WHERE package_name="{extend_package}" '
+        extend_package = '.'.join(package_class.split('.')[0: -1])
+        extend_class = package_class.split('.')[-1]
+        extend_class_db = self.sqlite.select_data(f'SELECT class_id, package_name, class_name, extends_class, annotations '
+                                                  f'FROM class WHERE package_name="{extend_package}" '
                                                   f'AND class_name="{extend_class}" '
                                                   f'AND project_id={self.project_id} limit 1')
 
         if not extend_class_db:
-            return None, None
+            return None, None, None
         extend_class_entity = extend_class_db[0]
         extend_class_id = extend_class_entity['class_id']
-        methods_db_list = self.sqlite.select_data(f'SELECT * FROM methods WHERE class_id={extend_class_id} and method_name = "{method_name}"')
+        methods_db_list = self.sqlite.select_data(f'SELECT method_name, parameters, return_type FROM methods WHERE project_id = {self.project_id} and class_id={extend_class_id} and method_name = "{method_name}"')
+        data_in_annotation = [annotation for annotation in json.loads(extend_class_entity['annotations']) if annotation['name'] in ['Data', 'Getter', 'Setter', 'Builder', 'NoArgsConstructor', 'AllArgsConstructor']]
+        if not methods_db_list and data_in_annotation and (method_name.startswith('get') or method_name.startswith('set')):
+            field_name = method_name[3:]
+            field_name = field_name[0].lower() + field_name[1:] if len(field_name) > 1 else field_name[0].lower()
+            methods_db_list = self.sqlite.select_data(f'SELECT field_name, field_type FROM field WHERE project_id = {self.project_id} and class_id={extend_class_id} and field_name = "{field_name}"')
         if not methods_db_list and not extend_class_entity['extends_class']:
-            return None, None
+            return None, None, None
         if not methods_db_list:
-            return self._find_method_in_extends(extend_class_entity['extends_class'], method_name, method_arguments)
+            return self._find_method_in_package_class(extend_class_entity['extends_class'], method_name, method_arguments)
         else:
-            filter_methods = [method for method in methods_db_list if len(json.loads(method['parameters'])) == len(method_arguments)]
+            filter_methods = [method for method in methods_db_list if len(json.loads(method.get('parameters', '[]'))) == len(method_arguments)]
             if not filter_methods:
-                return self._find_method_in_extends(extend_class_entity['extends_class'], method_name, method_arguments)
-            package_class = extend_class_entity['package_name'] + '.' + extend_class_entity['class_name']
+                return self._find_method_in_package_class(extend_class_entity['extends_class'], method_name, method_arguments)
+            # package_class = extend_class_entity['package_name'] + '.' + extend_class_entity['class_name']
             if len(filter_methods) == 1:
                 method_db = filter_methods[0]
-                method_params = f'{method_db["method_name"]}({",".join([param["parameter_type"] for param in json.loads(method_db["parameters"])])})'
-                return package_class, method_params
+                method_params = f'{method_db.get("method_name", method_name)}({",".join([param["parameter_type"] for param in json.loads(method_db.get("parameters", "[]"))])})'
+                return package_class, method_params, method_db
             else:
                 max_score = -float('inf')
                 max_score_method = None
                 for method_db in filter_methods:
-                    method_db_params = [param["parameter_type"] for param in json.loads(method_db["parameters"])]
-                    score = self._calculate_similar_score_method_params(method_arguments, method_db_params)
+                    method_db_params = [param["parameter_type"] for param in json.loads(method_db.get("parameters", "[]"))]
+                    score = calculate_similar_score_method_params(method_arguments, method_db_params)
                     if score > max_score:
                         max_score = score
                         max_score_method = method_db
                 if max_score_method is None:
                     max_score_method = filter_methods[0]
-                method_params = f'{max_score_method["method_name"]}({",".join([param["parameter_type"] for param in json.loads(max_score_method["parameters"])])})'
-                return package_class, method_params
-
-    def _calculate_similar_score_method_params(self, except_method_param_list, method_param_list):
-        score = 0
-        positions = {}
-
-        # 记录list1中每个元素的位置
-        for i, item in enumerate(except_method_param_list):
-            positions[item] = i
-
-        # 遍历list2,计算分数
-        for i, item in enumerate(method_param_list):
-            if item in positions:
-                score += 1
-                score -= abs(i - positions[item])
-
-        return score
+                method_params = f'{max_score_method.get("method_name", method_name)}({",".join([param["parameter_type"] for param in json.loads(max_score_method.get("parameters", "[]"))])})'
+                return package_class, method_params, max_score_method
 
     def _get_method_end_line(self, method_obj):
         method_end_line = method_obj.position.line
         while True:
             if isinstance(method_obj, list):
-                if None in method_obj:
-                    method_obj.remove(None)
+                method_obj = [obj for obj in method_obj if obj and not isinstance(obj, str)]
                 if len(method_obj) == 0:
                     break
                 length = len(method_obj)
                 for i in range(0, length):
                     temp = method_obj[length - 1 - i]
                     if temp is not None:
                         method_obj = temp
@@ -480,70 +658,75 @@
         elif FIELDS not in method_invocation[package_class].keys():
             method_invocation[package_class][FIELDS] = {field: lines}
         elif field not in method_invocation[package_class][FIELDS].keys():
             method_invocation[package_class][FIELDS][field] = lines
         else:
             method_invocation[package_class][FIELDS][field] += lines
 
-    def _deal_declarator_type(self, node_type, import_map, method_invocation, section, package_name, filepath):
+    def _deal_declarator_type(self, node_type, section, parameters_map, variable_map, field_map, import_map, method_invocation, package_name, filepath, methods, method_name_entity_map, class_id):
         if node_type is None:
             return node_type
         if type(node_type) == javalang.tree.BasicType:
             node_name = node_type.name
-            node_name = node_name[0].upper() + node_name[1:]
+            if node_name != 'int':
+                node_name = node_name[0].upper() + node_name[1:]
             return node_name
-        var_declarator_type = node_type.name
-        if var_declarator_type in import_map.keys():
-            var_declarator_type = import_map.get(var_declarator_type)
-            self._add_entity_used_to_method_invocation(method_invocation, var_declarator_type, section)
-        else:
-            node_path = "/".join(filepath.split("/")[0: -1]) + "/" + var_declarator_type + ".java"
-            if os.path.exists(node_path):
-                var_declarator_type = f'{package_name}.{var_declarator_type}'
-            else:
-                var_declarator_type = var_declarator_type[0].upper() + var_declarator_type[1:]
-        var_declarator_type_arguments = self._deal_arguments_type(node_type.arguments, import_map, method_invocation, section, package_name, filepath)
+        var_declarator_type = self._parse_sub_type(node_type)
+        var_declarator_type = self._get_var_type(var_declarator_type, parameters_map, variable_map, field_map, import_map, method_invocation, section, package_name, filepath)
+        var_declarator_type_arguments = self._deal_arguments_type(node_type.arguments, section, parameters_map, variable_map, field_map, import_map, method_invocation, package_name, filepath, methods, method_name_entity_map, class_id)
         if var_declarator_type_arguments:
             var_declarator_type = var_declarator_type + '<' + '#'.join(var_declarator_type_arguments) + '>'
         return var_declarator_type
 
-    def _deal_arguments_type(self, arguments, import_map, method_invocation, section, package_name, filepath):
+    def _parse_sub_type(self, type_obj):
+        type_name = type_obj.name
+        if 'sub_type' in type_obj.attrs and type_obj.sub_type:
+            type_name = type_name + '.' + self._parse_sub_type(type_obj.sub_type)
+        return type_name
+
+    def _deal_arguments_type(self, arguments, section, parameters_map, variable_map, field_map, import_map, method_invocation, package_name, filepath, methods, method_name_entity_map, class_id):
         var_declarator_type_arguments_new = []
         if not arguments:
             return var_declarator_type_arguments_new
         var_declarator_type_arguments = []
         for argument in arguments:
-            if type(argument) == javalang.tree.MethodInvocation:
-                var_declarator_type_arguments.append(PARAMETER_TYPE_METHOD_INVOCATION_UNKNOWN)
-                continue
-            var_declarator_type_argument = self._deal_type(argument)
-            if var_declarator_type_argument in import_map.keys():
-                var_declarator_type_argument = import_map.get(var_declarator_type_argument)
-                self._add_entity_used_to_method_invocation(method_invocation, var_declarator_type_argument, section)
+            argument_type = type(argument)
+            if argument_type == javalang.tree.MethodInvocation:
+                var_declarator_type_argument = self._parse_method_body_method_invocation(argument, parameters_map, variable_map, field_map, import_map, method_invocation, package_name, filepath, methods, method_name_entity_map, class_id)
+            elif argument_type == javalang.tree.This:
+                var_declarator_type_argument = self._parse_node_selectors(argument.selectors, None, parameters_map, variable_map, field_map, import_map, method_invocation, package_name, filepath, methods, method_name_entity_map, class_id)
             else:
-                node_path = "/".join(filepath.split("/")[0: -1]) + "/" + var_declarator_type_argument + ".java"
-                if os.path.exists(node_path):
-                    var_declarator_type_argument = f'{package_name}.{var_declarator_type_argument}'
-                elif var_declarator_type_argument != PARAMETER_TYPE_METHOD_INVOCATION_UNKNOWN:
-                    var_declarator_type_argument = var_declarator_type_argument[0].upper() + var_declarator_type_argument[1:]
+                var_declarator_type_argument = self._deal_type(argument)
+                var_declarator_type_argument = self._get_var_type(var_declarator_type_argument, parameters_map, variable_map, field_map, import_map, method_invocation, section, package_name, filepath)
+            if self._is_valid_prefix(var_declarator_type_argument):
+                self._add_entity_used_to_method_invocation(method_invocation, var_declarator_type_argument, section)
             var_declarator_type_arguments.append(var_declarator_type_argument)
         return var_declarator_type_arguments
 
+    def _deal_member_reference(self, member_reference, parameters_map, variable_map, field_map, import_map, method_invocation, section, package_name, filepath):
+        member = member_reference.member
+        qualifier: str = member_reference.qualifier
+        if not qualifier:
+            qualifier_type = self._get_var_type(member, parameters_map, variable_map, field_map, import_map, method_invocation, section, package_name, filepath)
+        else:
+            qualifier_type = self._get_var_type(qualifier, parameters_map, variable_map, field_map, import_map, method_invocation, section, package_name, filepath)
+        if self._is_valid_prefix(qualifier_type):
+            self._add_field_used_to_method_invocation(method_invocation, qualifier_type, member, [None])
+        return qualifier_type
+
     def _deal_type(self, argument):
         if not argument:
             return None
         argument_type = type(argument)
         if argument_type == javalang.tree.MemberReference:
             var_declarator_type_argument = argument.member
         elif argument_type == javalang.tree.ClassCreator:
             var_declarator_type_argument = argument.type.name
         elif argument_type == javalang.tree.Literal:
             var_declarator_type_argument = self._deal_literal_type(argument.value)
-        elif argument_type == javalang.tree.This:
-            var_declarator_type_argument = PARAMETER_TYPE_METHOD_INVOCATION_UNKNOWN
         elif argument_type == javalang.tree.LambdaExpression:
             var_declarator_type_argument = PARAMETER_TYPE_METHOD_INVOCATION_UNKNOWN
         elif argument_type == javalang.tree.BinaryOperation:
             # todo BinaryOperation temp set string
             var_declarator_type_argument = 'String'
         elif argument_type == javalang.tree.MethodReference or argument_type == javalang.tree.TernaryExpression:
             # todo MethodReference temp set unknown
@@ -568,135 +751,249 @@
     def _deal_literal_type(self, text):
         if 'true' == text or 'false' == text:
             return 'Boolean'
         if text.isdigit():
             return 'Int'
         return 'String'
 
-    def _deal_var_type(self, arguments, parameters_map, variable_map, field_map, import_map, method_invocation, section, package_name, filepath):
+    def _deal_var_type(self, arguments, section, parameters_map, variable_map, field_map, import_map, method_invocation, package_name, filepath, methods, method_name_entity_map, class_id):
         var_declarator_type_arguments_new = []
         if not arguments:
             return var_declarator_type_arguments_new
         var_declarator_type_arguments = []
         for argument in arguments:
             argument_type = type(argument)
             if argument_type == javalang.tree.MethodInvocation:
-                var_declarator_type_arguments.append(PARAMETER_TYPE_METHOD_INVOCATION_UNKNOWN)
-                continue
-            elif argument_type == javalang.tree.MemberReference and argument.qualifier:
-                var_declarator_type_arguments.append(PARAMETER_TYPE_METHOD_INVOCATION_UNKNOWN)
-                continue
-            var_declarator_type_argument = self._deal_type(argument)
-            var_declarator_type_argument = self._get_var_type(var_declarator_type_argument, parameters_map, variable_map, field_map, import_map, method_invocation, section, package_name, filepath)
-            type_arguments = self._deal_arguments_type(argument.type.arguments, import_map, method_invocation, section, package_name, filepath) \
+                var_declarator_type_argument = self._parse_method_body_method_invocation(argument, parameters_map, variable_map, field_map, import_map, method_invocation, package_name, filepath, methods, method_name_entity_map, class_id)
+            elif argument_type == javalang.tree.MemberReference:
+                var_declarator_type_argument = self._deal_member_reference(argument, parameters_map, variable_map, field_map, import_map, method_invocation, section, package_name, filepath)
+            elif argument_type == javalang.tree.This:
+                var_declarator_type_argument = self._parse_node_selectors(argument.selectors, None, parameters_map, variable_map, field_map, import_map, method_invocation, package_name, filepath, methods, method_name_entity_map, class_id)
+                if var_declarator_type_argument is None:
+                    var_declarator_type_argument = PARAMETER_TYPE_METHOD_INVOCATION_UNKNOWN
+            else:
+                var_declarator_type_argument = self._deal_type(argument)
+                var_declarator_type_argument = self._get_var_type(var_declarator_type_argument, parameters_map, variable_map, field_map, import_map, method_invocation, section, package_name, filepath)
+            type_arguments = self._deal_arguments_type(argument.type.arguments, section, parameters_map, variable_map, field_map, import_map, method_invocation, package_name, filepath, methods, method_name_entity_map, class_id) \
                 if 'type' in argument.attrs \
                    and not isinstance(argument.type, str) \
                    and 'arguments' in argument.type.attrs \
                    and argument.type.arguments \
                 else []
             if type_arguments:
                 var_declarator_type_argument = var_declarator_type_argument + '<' + '#'.join(type_arguments) + '>'
             var_declarator_type_arguments.append(var_declarator_type_argument)
         return var_declarator_type_arguments
 
     def _get_var_type(self, var, parameters_map, variable_map, field_map, import_map, method_invocation, section, package_name, filepath):
         if not var:
             return var
+        if var.lower() in JAVA_BASIC_TYPE or var in JAVA_UTIL_TYPE:
+            return var
+        var_path = "/".join(filepath.split("/")[0: -1]) + "/" + var + ".java"
         if var in parameters_map.keys():
             return parameters_map.get(var)
-        if var in variable_map.keys():
+        elif var in variable_map.keys():
             return variable_map.get(var)
-        if var in field_map.keys():
+        elif var in field_map.keys():
             field_type = field_map.get(var)['field_type']
             package_class = field_map.get(var)['package_class']
             start_line = field_map.get(var)['start_line']
             self._add_field_used_to_method_invocation(method_invocation, package_class, var, [start_line])
             return field_type
-        if var in import_map.keys():
+        elif var in import_map.keys():
+            if '.' in var:
+                return self._parse_layer_call_var_type(var, import_map, method_invocation)
             var_type = import_map.get(var)
-            self._add_entity_used_to_method_invocation(method_invocation, var_type, section)
             return var_type
-        else:
-            var_path = "/".join(filepath.split("/")[0: -1]) + "/" + var + ".java"
-            if os.path.exists(var_path):
-                var_type = f'{package_name}.{var}'
+        elif os.path.exists(var_path):
+            var_type = f'{package_name}.{var}'
+            return var_type
+        if '.' not in var:
+            sql = "select package_name, class_name from class where project_id = {} and class_name=\"{}\" and filepath = \"{}\"".format(self.project_id, var, filepath)
+            var_class_db = self.sqlite.select_data(sql)
+            if var_class_db:
+                return var_class_db[0]['package_name'] + '.' + var_class_db[0]['class_name']
+        return self._parse_layer_call_var_type(var, import_map, method_invocation)
+
+    def _parse_layer_call_var_type(self, var, import_map, method_invocation):
+        ## 判断是否内部类
+        var_split = var.split('.')
+        var_class = var_split[-1]
+        if var_class.lower() in JAVA_BASIC_TYPE or var_class in JAVA_UTIL_TYPE:
+            return var
+        elif len(var_split) > 1:
+            var_field = var_split[-1]
+            var_class = var_split[-2]
+            if var_class in import_map.keys():
+                var_type = import_map.get(var_class)
+                var_type_package = '.'.join(var_type.split('.')[0: -1])
+                var_field_db = self.sqlite.select_data(f'select field_type from field where project_id={self.project_id} and field_name="{var_field}" '
+                                                       f'and class_id in (select class_id from class where project_id={self.project_id} and class_name="{var_class}" and package_name="{var_type_package}")')
+                if var_field_db:
+                    self._add_field_used_to_method_invocation(method_invocation, var_type, var_field, [None])
+                    field_type = var_field_db[0]['field_type']
+                    if field_type == 'ENUM':
+                        return var_type
+                    return field_type
+            var_package_end = '.'.join(var_split[0: -1])
+            sql = "select package_name, class_name from class where project_id = {} and class_name=\"{}\" and package_name like \"%{}\"".format(self.project_id, var_field, var_package_end)
+            var_class_db = self.sqlite.select_data(sql)
+            if var_class_db:
+                var_type = var_class_db[0]['package_name'] + '.' + var_class_db[0]['class_name']
                 return var_type
-            elif var != PARAMETER_TYPE_METHOD_INVOCATION_UNKNOWN:
-                var = var[0].upper() + var[1:]
+        elif var != PARAMETER_TYPE_METHOD_INVOCATION_UNKNOWN:
+            return var[0].upper() + var[1:]
         return var
 
     def _get_extends_class_fields_map(self, class_id: int):
-        class_db = self.sqlite.select_data(f'SELECT * FROM class WHERE class_id = {class_id}')[0]
+        class_db = self.sqlite.select_data(f'SELECT extends_class FROM class WHERE project_id = {self.project_id} and class_id = {class_id}')[0]
         extend_package_class = class_db['extends_class']
         if not extend_package_class:
             return {}
         extend_package = '.'.join(extend_package_class.split('.')[0: -1])
         extend_class = extend_package_class.split('.')[-1]
-        extend_class_db = self.sqlite.select_data(f'SELECT * FROM class WHERE package_name="{extend_package}" '
+        extend_class_db = self.sqlite.select_data(f'SELECT class_id, extends_class FROM class WHERE package_name="{extend_package}" '
                                                   f'AND class_name="{extend_class}" '
                                                   f'AND project_id={self.project_id} limit 1')
         if not extend_class_db:
             return {}
         extend_class_entity = extend_class_db[0]
         extend_class_id = extend_class_entity['class_id']
-        extend_class_fields = self.sqlite.select_data(f'SELECT * FROM field WHERE class_id = {extend_class_id}')
+        extend_class_fields = self.sqlite.select_data(f'SELECT field_name, field_type, start_line  FROM field WHERE project_id = {self.project_id} and class_id = {extend_class_id}')
         extend_class_fields_map = {field_obj['field_name']: {'field_type': field_obj['field_type'], 'package_class': extend_package_class, 'start_line': field_obj['start_line']} for field_obj in extend_class_fields}
         if not extend_class_entity['extends_class']:
             return extend_class_fields_map
         else:
             extend_new_map = self._get_extends_class_fields_map(extend_class_id)
             extend_new_map.update(extend_class_fields_map)
             return extend_new_map
 
-    def parse_java_file(self, filepath: str, commit_or_branch: str):
-        if not filepath.endswith('.java'):
-            return
-        try:
-            with open(filepath, encoding='UTF-8') as fp:
-                file_content = fp.read()
-        except:
-            return
-        logging.info(f'Parsing java file: {filepath}')
-        lines = file_content.split('\n')
-        try:
-            tree = javalang.parse.parse(file_content)
-            if not tree.types:
-                return
-        except Exception as e:
-            logging.error(f"Error parsing {filepath}: {e}")
-            return
-        # 处理包信息
-        package_name = tree.package.name if tree.package else 'unknown'
-        class_name = tree.types[0].name
+    def _is_valid_prefix(self, import_str):
+        for prefix in config.package_prefix:
+            if import_str and import_str.startswith(prefix):
+                return True
+        return False
+
+    def _get_sibling_dirs(self, path):
+        parent_dir = os.path.abspath(os.path.join(path, os.pardir))
+        dirs = [os.path.join(parent_dir, d).replace('\\', '/') for d in os.listdir(parent_dir) if os.path.isdir(os.path.join(parent_dir, d)) and not d.startswith('.')]
+        return dirs
+
+    def _list_files(self, directory):
+        # 使用 os.listdir() 获取目录下所有文件和文件夹名
+        all_contents = os.listdir(directory)
+
+        # 完整的文件路径列表
+        full_paths = [os.path.join(directory, f) for f in all_contents]
+
+        # 筛选出是文件的路径
+        only_files = [f.replace('\\', '/') for f in full_paths if os.path.isfile(f)]
+
+        return only_files
+
+    def _parse_import_file(self, imports, commit_or_branch, parse_import_first):
+        for import_decl in imports:
+            import_path = import_decl.path
+            is_static = import_decl.static
+            is_wildcard = import_decl.wildcard
+            if not self._is_valid_prefix(import_path):
+                continue
+            if is_static:
+                import_path = '.'.join(import_path.split('.')[0:-1])
+            java_files = []
+            if is_wildcard:
+                import_filepaths = [file_path + '/src/main/java/' + import_path.replace('.', '/') for file_path in self.sibling_dirs]
+                for import_filepath in import_filepaths:
+                    if not os.path.exists(import_filepath):
+                        continue
+                    java_files += self._list_files(import_filepath)
+            else:
+                java_files = [file_path + '/src/main/java/' + import_path.replace('.', '/') + '.java' for file_path in self.sibling_dirs]
+            for import_filepath in java_files:
+                if not os.path.exists(import_filepath):
+                    continue
+                self.parse_java_file(import_filepath, commit_or_branch, parse_import_first=parse_import_first)
+
+    def _parse_tree_class(self, class_declaration, filepath, tree_imports, package_name, commit_or_branch, lines, parse_import_first):
+        class_name = class_declaration.name
         package_class = package_name + '.' + class_name
-        # 处理 import 信息
-        import_list = self._parse_imports(tree.imports)
+        import_list = self._parse_imports(tree_imports)
         import_map = {import_obj['import_path'].split('.')[-1]: import_obj['import_path'] for import_obj in import_list}
 
         # 处理 class 信息
-        class_id, new_add = self._parse_class(tree.types[0], filepath, package_name, import_list, commit_or_branch)
+        class_type = type(class_declaration).__name__.replace('Declaration', '')
+        class_id, new_add = self._parse_class(class_declaration, filepath, package_name, import_list, commit_or_branch, parse_import_first)
         # 已经处理过了，返回
         # if not new_add:
         #     return
         # 导入import
         imports = [dict(import_obj, class_id=class_id, project_id=self.project_id) for import_obj in import_list]
         self.sqlite.update_data(f'DELETE FROM import WHERE class_id={class_id}')
         self.sqlite.insert_data('import', imports)
 
+        # 处理 inner class
+        inner_class_declarations = [inner_class for inner_class in class_declaration.body
+                                    if type(inner_class) == javalang.tree.ClassDeclaration
+                                    or type(inner_class) == javalang.tree.InterfaceDeclaration]
+        for inner_class_obj in inner_class_declarations:
+            self._parse_tree_class(inner_class_obj, filepath, tree_imports, package_class, commit_or_branch, lines, parse_import_first)
+
         # 处理 field 信息
-        field_list = self._parse_fields(tree.types[0].fields, package_name, class_id, import_map)
+        field_list = self._parse_fields(class_declaration.fields, package_name, class_name, class_id, import_map, filepath)
         field_map = {field_obj['field_name']: {'field_type': field_obj['field_type'], 'package_class': package_class, 'start_line': field_obj['start_line']} for field_obj in field_list}
-        import_map = dict((k, v) for k, v in import_map.items() if v.startswith('com.') or v.startswith('cn.'))
+        import_map = dict((k, v) for k, v in import_map.items() if self._is_valid_prefix(v))
 
         # 将extend class的field导进来
         extends_class_fields_map = self._get_extends_class_fields_map(class_id)
         extends_class_fields_map.update(field_map)
+
+        if class_type == 'Enum':
+            self._parse_enum(class_declaration.body, lines, class_id, import_map, field_map, package_name, filepath)
+
         # 处理 methods 信息
-        self._parse_method(tree.types[0].methods, lines, class_id, import_map, extends_class_fields_map, package_name, filepath)
+        self._parse_method(class_declaration.methods, lines, class_id, import_map, extends_class_fields_map, package_name, filepath)
+
+        self._parse_constructors(class_declaration.constructors, lines, class_id, import_map, extends_class_fields_map, package_name, filepath)
+
+    def parse_java_file(self, filepath: str, commit_or_branch: str, parse_import_first=True):
+        if filepath + '_' + commit_or_branch in self.parsed_filepath or not filepath.endswith('.java'):
+            return
+        self.parsed_filepath.append(filepath + '_' + commit_or_branch)
+        try:
+            with open(filepath, encoding='UTF-8') as fp:
+                file_content = fp.read()
+        except:
+            return
+        lines = file_content.split('\n')
+        try:
+            tree = javalang.parse.parse(file_content)
+            if not tree.types:
+                return
+        except Exception as e:
+            logging.error(f"Error parsing {filepath}: {e}")
+            return
+
+        # 处理包信息
+        package_name = tree.package.name if tree.package else 'unknown'
+        class_declaration = tree.types[0]
+        class_name = class_declaration.name
+        package_class = package_name + '.' + class_name
+        if not self.sibling_dirs:
+            package_path = package_class.replace('.', '/') + '.java'
+            base_filepath = filepath.replace(package_path, '')
+            self.sibling_dirs = self._get_sibling_dirs(base_filepath.replace('src/main/java/', ''))
+        # 处理 import 信息
+        if parse_import_first:
+            self._parse_import_file(tree.imports, commit_or_branch, parse_import_first)
+        logging.info(f'Parsing java file: {filepath}')
+        self._parse_tree_class(class_declaration, filepath, tree.imports, package_name, commit_or_branch, lines, parse_import_first)
 
     def parse_java_file_list(self, filepath_list: list, commit_or_branch: str):
-        for file_path in filepath_list:
-            self.parse_java_file(file_path, commit_or_branch)
+        with ThreadPoolExecutor(max_workers=4) as executor:
+            futures = [executor.submit(self.parse_java_file, file, commit_or_branch) for file in filepath_list]
+            for _ in as_completed(futures):
+                continue
 
 
 if __name__ == '__main__':
     print('jcci')
```

### Comparing `jcci-0.1.5/src/jcci/mapper_parse.py` & `jcci-0.2.0/src/jcci/mapper_parse.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,25 +25,25 @@
     def __init__(self, id, type, start_line, end_line, content, statement_tag, result_map, include_sql):
         super(MapperStatement, self).__init__(id, type, start_line, end_line, content)
         self.statement_tag = statement_tag
         self.result_map = result_map
         self.include_sql = include_sql
 
 def extract_value(string, tag):
-    pattern = tag + r'\s*=\s*"(\w+)"'
+    pattern = tag + r'\s*=\s*[\'"](\w+)[\'"]'
     match = re.search(pattern, string)
     if match:
         value = match.group(1)
         return value
     else:
         return None
 
 
 def check_string(tag, id_str, string):
-    pattern = r'^' + tag + '.*?id\s*=\s*"' + id_str + '"'
+    pattern = r'^' + tag + '.*?id\s*=\s*[\'"]' + id_str + '[\'"]'
     match = re.search(pattern, string)
     return bool(match)
 
 def parse(filepath):
     # 读取XML文件内容
     try:
         with open(filepath, "r", encoding="utf-8") as file:
@@ -102,19 +102,18 @@
         start_line = 0
         end_line = 0
         result_map = None
         include_sql = None
         for i, line in enumerate(xml_content.splitlines(), start=1):
             if check_string('<' + statement_element.tag, statement_id, line.strip()):
                 start_line = i
-            if f'resultMap="' in line and start_line != 0:
+            if f'resultMap' in line and start_line != 0:
                 result_map = extract_value(line, 'resultMap')
             if line.strip().startswith('<include') and start_line != 0:
                 include_sql = extract_value(line, 'refid')
             if f'</{statement_element.tag}>' in line and start_line != 0:
                 end_line = i
                 break
         content = xml_content.splitlines()[start_line - 1: end_line]
         statement_info.append(MapperStatement(statement_id, 'statement', start_line, end_line, content, statement_element.tag, result_map, include_sql))
 
     return Mapper(namespace, result_map_info, sql_info, statement_info)
-
```

### Comparing `jcci-0.1.5/src/jcci/sql.py` & `jcci-0.2.0/src/jcci/sql.py`

 * *Files identical despite different names*

### Comparing `jcci-0.1.5/src/jcci.egg-info/PKG-INFO` & `jcci-0.2.0/src/jcci.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jcci
-Version: 0.1.5
+Version: 0.2.0
 Summary: Java code commit impact, java code change impact analysis, java代码改动影响范围分析工具
 Author-email: Oliver Li <441640312@qq.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -203,30 +203,29 @@
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
 Project-URL: Homepage, https://github.com/baikaishuipp/jcci
 Project-URL: Bug Tracker, https://github.com/baikaishuipp/jcci/issues
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: javalang>=0.13.0
 Requires-Dist: unidiff>=0.7.4
 
 #### Description
 Java code commit impact analysis, is a pure python library that analyzes the impact of two git submissions of Java projects on the project and generates tree chart data.
 
 Github: [jcci](https://github.com/baikaishuipp/jcci)
-#### Installation
-```
-pip install jcci
-```
+
+#### Achieve Effect
+![效果图](./images/cii-result-tree.png)
 
 #### Instructions
 Start a new python project, add a new python file, code example:
 
 ```
 from jcci.analyze import JCCI
```

