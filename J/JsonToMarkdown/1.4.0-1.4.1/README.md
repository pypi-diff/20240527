# Comparing `tmp/JsonToMarkdown-1.4.0.tar.gz` & `tmp/JsonToMarkdown-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/JsonToMarkdown-1.4.0.tar", last modified: Thu Jun 16 07:51:41 2022, max compression
+gzip compressed data, was "dist/JsonToMarkdown-1.4.1.tar", last modified: Mon May 27 08:11:58 2024, max compression
```

## Comparing `JsonToMarkdown-1.4.0.tar` & `JsonToMarkdown-1.4.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 rapha      (501) staff       (20)        0 2022-06-16 07:51:41.000000 JsonToMarkdown-1.4.0/
-drwxr-xr-x   0 rapha      (501) staff       (20)        0 2022-06-16 07:51:41.000000 JsonToMarkdown-1.4.0/JsonToMarkdown/
--rw-r--r--   0 rapha      (501) staff       (20)        0 2022-06-16 07:50:49.000000 JsonToMarkdown-1.4.0/JsonToMarkdown/__init__.py
--rw-r--r--   0 rapha      (501) staff       (20)      570 2022-06-16 07:50:49.000000 JsonToMarkdown-1.4.0/JsonToMarkdown/cat.py
--rw-r--r--   0 rapha      (501) staff       (20)     6789 2022-06-16 07:50:49.000000 JsonToMarkdown-1.4.0/JsonToMarkdown/check_obs.py
--rw-r--r--   0 rapha      (501) staff       (20)    22174 2022-06-16 07:50:49.000000 JsonToMarkdown-1.4.0/JsonToMarkdown/json_to_obs.py
--rw-r--r--   0 rapha      (501) staff       (20)     8903 2022-06-16 07:50:49.000000 JsonToMarkdown-1.4.0/JsonToMarkdown/libmd.py
--rw-r--r--   0 rapha      (501) staff       (20)     9705 2022-06-16 07:50:49.000000 JsonToMarkdown-1.4.0/JsonToMarkdown/libsvg.py
--rw-r--r--   0 rapha      (501) staff       (20)    32525 2022-06-16 07:51:19.000000 JsonToMarkdown-1.4.0/JsonToMarkdown/main.py
--rw-r--r--   0 rapha      (501) staff       (20)      402 2022-06-16 07:50:49.000000 JsonToMarkdown-1.4.0/JsonToMarkdown/preprocess.py
-drwxr-xr-x   0 rapha      (501) staff       (20)        0 2022-06-16 07:51:41.000000 JsonToMarkdown-1.4.0/JsonToMarkdown.egg-info/
--rw-r--r--   0 rapha      (501) staff       (20)      315 2022-06-16 07:51:40.000000 JsonToMarkdown-1.4.0/JsonToMarkdown.egg-info/PKG-INFO
--rw-r--r--   0 rapha      (501) staff       (20)      416 2022-06-16 07:51:40.000000 JsonToMarkdown-1.4.0/JsonToMarkdown.egg-info/SOURCES.txt
--rw-r--r--   0 rapha      (501) staff       (20)        1 2022-06-16 07:51:40.000000 JsonToMarkdown-1.4.0/JsonToMarkdown.egg-info/dependency_links.txt
--rw-r--r--   0 rapha      (501) staff       (20)      140 2022-06-16 07:51:40.000000 JsonToMarkdown-1.4.0/JsonToMarkdown.egg-info/entry_points.txt
--rw-r--r--   0 rapha      (501) staff       (20)       15 2022-06-16 07:51:40.000000 JsonToMarkdown-1.4.0/JsonToMarkdown.egg-info/top_level.txt
--rw-r--r--   0 rapha      (501) staff       (20)      315 2022-06-16 07:51:41.000000 JsonToMarkdown-1.4.0/PKG-INFO
--rw-r--r--   0 rapha      (501) staff       (20)        0 2020-07-14 01:39:49.000000 JsonToMarkdown-1.4.0/README
--rw-r--r--   0 rapha      (501) staff       (20)       38 2022-06-16 07:51:41.000000 JsonToMarkdown-1.4.0/setup.cfg
--rw-r--r--   0 rapha      (501) staff       (20)      798 2022-06-16 07:51:35.000000 JsonToMarkdown-1.4.0/setup.py
+drwxr-xr-x   0 rapha      (501) staff       (20)        0 2024-05-27 08:11:58.000000 JsonToMarkdown-1.4.1/
+drwxr-xr-x   0 rapha      (501) staff       (20)        0 2024-05-27 08:11:58.000000 JsonToMarkdown-1.4.1/JsonToMarkdown/
+-rw-r--r--   0 rapha      (501) staff       (20)        0 2022-06-16 07:50:49.000000 JsonToMarkdown-1.4.1/JsonToMarkdown/__init__.py
+-rw-r--r--   0 rapha      (501) staff       (20)      570 2022-06-16 07:50:49.000000 JsonToMarkdown-1.4.1/JsonToMarkdown/cat.py
+-rw-r--r--   0 rapha      (501) staff       (20)     6789 2022-06-16 07:50:49.000000 JsonToMarkdown-1.4.1/JsonToMarkdown/check_obs.py
+-rw-r--r--   0 rapha      (501) staff       (20)    22174 2022-06-16 07:50:49.000000 JsonToMarkdown-1.4.1/JsonToMarkdown/json_to_obs.py
+-rw-r--r--   0 rapha      (501) staff       (20)     8903 2022-06-16 07:50:49.000000 JsonToMarkdown-1.4.1/JsonToMarkdown/libmd.py
+-rw-r--r--   0 rapha      (501) staff       (20)     9705 2022-06-16 07:50:49.000000 JsonToMarkdown-1.4.1/JsonToMarkdown/libsvg.py
+-rw-r--r--   0 rapha      (501) staff       (20)    33576 2024-05-27 08:11:15.000000 JsonToMarkdown-1.4.1/JsonToMarkdown/main.py
+-rw-r--r--   0 rapha      (501) staff       (20)      402 2022-06-16 07:50:49.000000 JsonToMarkdown-1.4.1/JsonToMarkdown/preprocess.py
+drwxr-xr-x   0 rapha      (501) staff       (20)        0 2024-05-27 08:11:58.000000 JsonToMarkdown-1.4.1/JsonToMarkdown.egg-info/
+-rw-r--r--   0 rapha      (501) staff       (20)      315 2024-05-27 08:11:58.000000 JsonToMarkdown-1.4.1/JsonToMarkdown.egg-info/PKG-INFO
+-rw-r--r--   0 rapha      (501) staff       (20)      416 2024-05-27 08:11:58.000000 JsonToMarkdown-1.4.1/JsonToMarkdown.egg-info/SOURCES.txt
+-rw-r--r--   0 rapha      (501) staff       (20)        1 2024-05-27 08:11:58.000000 JsonToMarkdown-1.4.1/JsonToMarkdown.egg-info/dependency_links.txt
+-rw-r--r--   0 rapha      (501) staff       (20)      140 2024-05-27 08:11:58.000000 JsonToMarkdown-1.4.1/JsonToMarkdown.egg-info/entry_points.txt
+-rw-r--r--   0 rapha      (501) staff       (20)       15 2024-05-27 08:11:58.000000 JsonToMarkdown-1.4.1/JsonToMarkdown.egg-info/top_level.txt
+-rw-r--r--   0 rapha      (501) staff       (20)      315 2024-05-27 08:11:58.000000 JsonToMarkdown-1.4.1/PKG-INFO
+-rw-r--r--   0 rapha      (501) staff       (20)        0 2020-07-14 01:39:49.000000 JsonToMarkdown-1.4.1/README
+-rw-r--r--   0 rapha      (501) staff       (20)       38 2024-05-27 08:11:58.000000 JsonToMarkdown-1.4.1/setup.cfg
+-rw-r--r--   0 rapha      (501) staff       (20)      798 2024-05-27 08:11:49.000000 JsonToMarkdown-1.4.1/setup.py
```

### Comparing `JsonToMarkdown-1.4.0/JsonToMarkdown/cat.py` & `JsonToMarkdown-1.4.1/JsonToMarkdown/cat.py`

 * *Files identical despite different names*

### Comparing `JsonToMarkdown-1.4.0/JsonToMarkdown/check_obs.py` & `JsonToMarkdown-1.4.1/JsonToMarkdown/check_obs.py`

 * *Files identical despite different names*

### Comparing `JsonToMarkdown-1.4.0/JsonToMarkdown/json_to_obs.py` & `JsonToMarkdown-1.4.1/JsonToMarkdown/json_to_obs.py`

 * *Files identical despite different names*

### Comparing `JsonToMarkdown-1.4.0/JsonToMarkdown/libmd.py` & `JsonToMarkdown-1.4.1/JsonToMarkdown/libmd.py`

 * *Files identical despite different names*

### Comparing `JsonToMarkdown-1.4.0/JsonToMarkdown/libsvg.py` & `JsonToMarkdown-1.4.1/JsonToMarkdown/libsvg.py`

 * *Files identical despite different names*

### Comparing `JsonToMarkdown-1.4.0/JsonToMarkdown/main.py` & `JsonToMarkdown-1.4.1/JsonToMarkdown/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 sys.path.append(BASE_DIR)
 import preprocess
 import libsvg
 import libmd
 import cat as cat
 import json_to_obs as jo
 
-__version__ = 'v1.4.0'
+__version__ = 'v1.4.1'
 
 class TranslateJson(object):
     def __init__(self, js_file, link_path, dir_type, output_md, output_gitbook, output_xmind, \
             save_dir):
         self.js_file = js_file
         self.json_output_dir = os.path.join(link_path, '_json_output')
         self.save_dir = save_dir
@@ -354,19 +354,19 @@
             os.system("mv " + svg_name + " " + self.gitbookpath)
             #register_data += '\n<br>\n'
             register_data += '\n'
             self.reg_data += register_data + '\n'
             self.reg_rst += '   ' + name + '.md\n'
 
             file_path = os.path.join(self.gitbookpath, name + '.md')
-            with open(file_path, 'w') as fd:
-                fd.write(register_data)
-                for i in range(fields_len):
-                    f = fields[i]
-                    fd.write('\n' + '### ' + f['name'])
+            #with open(file_path, 'w') as fd:
+            #    fd.write(register_data)
+            #    for i in range(fields_len):
+            #        f = fields[i]
+            #        fd.write('\n' + '### ' + f['name'])
 
     def add_xmind_md(self, name, des):
         self.xmind_md += '* ' + name + '\n'
         des = des.replace('：',':').replace('；',';')
         if re.findall(';[0-9]:|。[0-9]:', des):
             for tmp_des in re.split('[;。]', des):
                 tmp_des = tmp_des.strip(' ')
@@ -678,14 +678,28 @@
                     path_msg = os.path.join("_json_output/", self.dirname, str(file_msg))
                 else:
                     path_msg = "_json_output/" + str(file_msg)
                 if not os.path.exists(self.gitbookpath):
                     os.system("mkdir -p " + self.gitbookpath)
                 readme = os.path.join(self.gitbookpath, 'README.md')
                 summary = os.path.join(self.gitbookpath, 'SUMMARY.md')
+                regrst = os.path.join(self.link_path, 'register.rst')
+                if not os.path.exists(regrst):
+                    with open(regrst, 'w') as fd:
+                        fd.write("寄存器说明\n====================\n\n.. toctree::\n\n")
+                        all_line = "   " + file_msg + "寄存器列表 <" + file_msg + "/all_register.md>\n" 
+                        detail_line = "   " + file_msg + "寄存器详细说明 <" + file_msg + "/detail.md>\n" 
+                        fd.write(all_line)
+                        fd.write(detail_line)
+                else:
+                    with open(regrst, 'a') as fd:
+                        all_line = "   " + file_msg + "寄存器列表 <" + file_msg + "/all_register.md>\n" 
+                        detail_line = "   " + file_msg + "寄存器详细说明 <" + file_msg + "/detail.md>\n" 
+                        fd.write(all_line)
+                        fd.write(detail_line)
                 if not os.path.exists(readme):
                     with open(readme, 'w') as fd:
                         fd.write("   ")
                 with open(summary, 'w') as fd:
                     fd.write('# Summary \n\n')
                     reg_list_path = os.path.join(path_msg, "all_register.md") 
                     reg_detail_path = os.path.join(path_msg, "detail.md") 
@@ -715,23 +729,25 @@
                     self.create_all_reg_data(lm)
                     gitlog = ''
                     try:
                         gitlog = self.get_gitlog()
                     except:
                         pass
                     with open(os.path.join(self.gitbookpath, 'all_register.md'), 'w') as fc:
-                        fc.write("## 寄存器列表\n\n" + self.all_reg_data)
-                    with open(os.path.join(self.gitbookpath, 'all_register_tex.md'), 'w') as fc:
-                        fc.write("## 寄存器列表\n\n" + self.all_reg_tex_data)
+                        fc.write("# 寄存器列表\n\n" + self.all_reg_data)
+                    #with open(os.path.join(self.gitbookpath, 'all_register_tex.md'), 'w') as fc:
+                    #    fc.write("## 寄存器列表\n\n" + self.all_reg_tex_data)
                     with open(os.path.join(self.gitbookpath, 'detail.md'), 'w') as fc:
                         fc.write(self.reg_data)
                     #with open(os.path.join(self.gitbookpath, 'detail.rst'), 'w') as fc:
                     #    fc.write(self.reg_rst)
-                self.check_file('README.md')
-                self.check_file('SUMMARY.md')
+                #self.check_file('README.md')
+                #self.check_file('SUMMARY.md')
+                os.system('rm ' + readme)
+                os.system('rm ' + summary)
                 print("\n\tcreate " + self.gitbookpath +" success") 
         if self.output_md:
             #self.markdownpath = "./_json_output/" + file_msg
             self.markdownpath = os.path.join("./_json_output/markdwon/", file_msg)
             if not os.path.exists(self.markdownpath):
                 os.system("mkdir -p " + self.markdownpath)
             md_file = os.path.join(self.markdownpath, file_msg + ".md")
@@ -815,7 +831,8 @@
     #        output_xmind,save_dir)
     #tjo.main()
     #
     #cat.cat_md(link_path, tj.file_msg)
 
 if __name__ == "__main__":
     main()
+
```

### Comparing `JsonToMarkdown-1.4.0/setup.py` & `JsonToMarkdown-1.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 def main():
     setup(
         name="JsonToMarkdown",
         description="Convert Json to Markdown",
         keywords="json markdown",
         long_description=long_description,
-        version="1.4.0",
+        version="1.4.1",
         author="zhaobk",
         author_email="zhaobk@nationalchip.com",
         packages=find_packages(),
         #packages=["JsonToMarkdown"],
         package_data={},
         entry_points={
             'console_scripts':[
```

