# Comparing `tmp/lyyguifunction-1.7.tar.gz` & `tmp/lyyguifunction-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lyyguifunction-1.7.tar", last modified: Thu May  2 12:53:31 2024, max compression
+gzip compressed data, was "lyyguifunction-1.8.tar", last modified: Mon May 27 09:48:26 2024, max compression
```

## Comparing `lyyguifunction-1.7.tar` & `lyyguifunction-1.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 12:53:31.403126 lyyguifunction-1.7/
--rw-rw-rw-   0        0        0     1090 2023-09-21 00:20:00.000000 lyyguifunction-1.7/LICENSE
--rw-rw-rw-   0        0        0      151 2024-05-02 12:53:31.402123 lyyguifunction-1.7/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-09-21 00:18:05.000000 lyyguifunction-1.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-02 12:53:31.401620 lyyguifunction-1.7/lyyguifunction.egg-info/
--rw-rw-rw-   0        0        0      151 2024-05-02 12:53:31.000000 lyyguifunction-1.7/lyyguifunction.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2024-05-02 12:53:31.000000 lyyguifunction-1.7/lyyguifunction.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 12:53:31.000000 lyyguifunction-1.7/lyyguifunction.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-02 12:53:31.000000 lyyguifunction-1.7/lyyguifunction.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-02 12:53:31.000000 lyyguifunction-1.7/lyyguifunction.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1343 2024-05-02 12:53:18.000000 lyyguifunction-1.7/lyyguifunction.py
--rw-rw-rw-   0        0        0       42 2024-05-02 12:53:31.403126 lyyguifunction-1.7/setup.cfg
--rw-rw-rw-   0        0        0      276 2024-05-02 12:53:30.000000 lyyguifunction-1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 09:48:26.045725 lyyguifunction-1.8/
+-rw-rw-rw-   0        0        0     1090 2023-09-21 00:20:00.000000 lyyguifunction-1.8/LICENSE
+-rw-rw-rw-   0        0        0      178 2024-05-27 09:48:26.044722 lyyguifunction-1.8/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2023-09-21 00:18:05.000000 lyyguifunction-1.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 09:48:26.042723 lyyguifunction-1.8/lyyguifunction.egg-info/
+-rw-rw-rw-   0        0        0      178 2024-05-27 09:48:25.000000 lyyguifunction-1.8/lyyguifunction.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2024-05-27 09:48:25.000000 lyyguifunction-1.8/lyyguifunction.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 09:48:25.000000 lyyguifunction-1.8/lyyguifunction.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-27 09:48:25.000000 lyyguifunction-1.8/lyyguifunction.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-27 09:48:25.000000 lyyguifunction-1.8/lyyguifunction.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1326 2024-05-22 05:48:41.000000 lyyguifunction-1.8/lyyguifunction.py
+-rw-rw-rw-   0        0        0       42 2024-05-27 09:48:26.046724 lyyguifunction-1.8/setup.cfg
+-rw-rw-rw-   0        0        0      276 2024-05-27 09:48:25.000000 lyyguifunction-1.8/setup.py
```

### Comparing `lyyguifunction-1.7/LICENSE` & `lyyguifunction-1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `lyyguifunction-1.7/lyyguifunction.py` & `lyyguifunction-1.8/lyyguifunction.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,37 @@
+import os
+from datetime import datetime
+import tkinter as tk
+import lyycfg 
 
-class gui_ico_class:
+class windget_function_class:
     def __init__(self, main_module) -> None:
         self.main_module = main_module
 
-
     def read_notice(self):
-        text = self.main_module.文本框_笔记.get("1.0", tk.END)
+        text = self.main_module.textbox_rule.get("1.0", tk.END)
 
     def load_notice(self):
         with open("notice\\notice.txt", "r", encoding="utf-8") as f:
             lines = f.readlines()
             # 获取最后10行
             # 将最后10行显示在self.main_module.文本框中
-            self.main_module.文本框_笔记.insert("1.0", "".join(lines))
+            self.main_module.textbox_rule.insert("1.0", "".join(lines))
 
     def set_notice(self, text):
-        self.main_module.文本框_笔记.insert(tk.END, text)
+        self.main_module.textbox_rule.insert(tk.END, text)
 
     def save_notice(self):
         # 先备份原来的
         # new_file=os.path.join(path,"project30.jpg")
 
-        newfile = f1999cfg.resource_path + "\\notice" + "\\notice" + "_" + datetime.now().strftime("%Y-%m-%d") + ".txt"
+        newfile =  "notice" + "\\notice" + "_" + datetime.now().strftime("%Y-%m-%d") + ".txt"
         if not os.path.isfile(newfile):
-            os.rename(f1999cfg.resource_path + "\\notice" + "\\notice.txt", newfile)
+            os.rename("notice" + "\\notice.txt", newfile)
 
-        alltext = self.main_module.文本框_笔记.get("1.0", "end-1c")
-        with open(f1999cfg.resource_path + "\\notice" + "\\notice.txt", "w", encoding="utf-8") as f:
+        alltext = self.main_module.textbox_rule.get("1.0", "end-1c")
+        with open("notice" + "\\notice.txt", "w", encoding="utf-8") as f:
             f.write(alltext)
-            self.main_module.状态栏文本变量1.set("保存完毕")    
+            self.main_module.status_bar_var.set("保存完毕")    
 if __name__ == "__main__":    
     show_msg_once()
     #show_toast()
```

