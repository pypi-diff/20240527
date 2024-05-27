# Comparing `tmp/conflict_rpa-0.0.8.tar.gz` & `tmp/conflict_rpa-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conflict_rpa-0.0.8.tar", last modified: Mon May 27 04:27:11 2024, max compression
+gzip compressed data, was "conflict_rpa-0.0.9.tar", last modified: Mon May 27 06:27:23 2024, max compression
```

## Comparing `conflict_rpa-0.0.8.tar` & `conflict_rpa-0.0.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 04:27:11.169345 conflict_rpa-0.0.8/
--rw-rw-rw-   0        0        0       51 2024-05-26 09:50:21.000000 conflict_rpa-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     6967 2024-05-27 04:27:11.168344 conflict_rpa-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     6701 2024-05-27 04:01:46.000000 conflict_rpa-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-27 04:27:11.146345 conflict_rpa-0.0.8/conflict_rpa/
--rw-rw-rw-   0        0        0        0 2024-05-24 13:02:31.000000 conflict_rpa-0.0.8/conflict_rpa/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-27 04:27:11.165346 conflict_rpa-0.0.8/conflict_rpa/__pycache__/
--rw-rw-rw-   0        0        0      139 2024-05-26 08:54:35.000000 conflict_rpa-0.0.8/conflict_rpa/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     2874 2024-05-26 08:54:35.000000 conflict_rpa-0.0.8/conflict_rpa/__pycache__/content_rpa.cpython-310.pyc
--rw-rw-rw-   0        0        0     8202 2024-05-26 08:54:35.000000 conflict_rpa-0.0.8/conflict_rpa/__pycache__/correcting_framework.cpython-310.pyc
--rw-rw-rw-   0        0        0     2083 2024-05-26 08:54:35.000000 conflict_rpa-0.0.8/conflict_rpa/__pycache__/file_operation.cpython-310.pyc
--rw-rw-rw-   0        0        0     2683 2024-05-26 08:54:35.000000 conflict_rpa-0.0.8/conflict_rpa/__pycache__/get_running_env.cpython-310.pyc
--rw-rw-rw-   0        0        0     1286 2024-05-26 08:54:35.000000 conflict_rpa-0.0.8/conflict_rpa/__pycache__/rpa.cpython-310.pyc
--rw-rw-rw-   0        0        0     3242 2024-05-26 08:54:35.000000 conflict_rpa-0.0.8/conflict_rpa/__pycache__/utils.cpython-310.pyc
--rw-rw-rw-   0        0        0     1852 2024-05-26 11:07:22.000000 conflict_rpa-0.0.8/conflict_rpa/config.py
--rw-rw-rw-   0        0        0     3446 2024-05-27 01:00:53.000000 conflict_rpa-0.0.8/conflict_rpa/content_rpa.py
--rw-rw-rw-   0        0        0    10864 2024-05-27 04:24:04.000000 conflict_rpa-0.0.8/conflict_rpa/correcting_framework.py
--rw-rw-rw-   0        0        0     3596 2024-05-27 02:59:24.000000 conflict_rpa-0.0.8/conflict_rpa/environment_setting.py
--rw-rw-rw-   0        0        0     2436 2024-05-25 10:32:15.000000 conflict_rpa-0.0.8/conflict_rpa/file_operation.py
--rw-rw-rw-   0        0        0     2926 2024-05-25 10:32:16.000000 conflict_rpa-0.0.8/conflict_rpa/get_running_env.py
--rw-rw-rw-   0        0        0     3736 2024-05-27 01:00:54.000000 conflict_rpa-0.0.8/conflict_rpa/link_rpa.py
--rw-rw-rw-   0        0        0     2537 2024-05-27 04:24:13.000000 conflict_rpa-0.0.8/conflict_rpa/rpa.py
--rw-rw-rw-   0        0        0     3309 2024-05-26 23:39:44.000000 conflict_rpa-0.0.8/conflict_rpa/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-27 04:27:11.167345 conflict_rpa-0.0.8/conflict_rpa.egg-info/
--rw-rw-rw-   0        0        0     6967 2024-05-27 04:27:10.000000 conflict_rpa-0.0.8/conflict_rpa.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      912 2024-05-27 04:27:11.000000 conflict_rpa-0.0.8/conflict_rpa.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 04:27:10.000000 conflict_rpa-0.0.8/conflict_rpa.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-05-27 04:27:10.000000 conflict_rpa-0.0.8/conflict_rpa.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       32 2024-05-27 04:27:10.000000 conflict_rpa-0.0.8/conflict_rpa.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-27 04:27:10.000000 conflict_rpa-0.0.8/conflict_rpa.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       95 2024-05-25 13:49:40.000000 conflict_rpa-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-27 04:27:11.169345 conflict_rpa-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      565 2024-05-27 04:27:05.000000 conflict_rpa-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 06:27:23.441803 conflict_rpa-0.0.9/
+-rw-rw-rw-   0        0        0       51 2024-05-26 09:50:21.000000 conflict_rpa-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     7707 2024-05-27 06:27:23.439803 conflict_rpa-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     7443 2024-05-27 05:48:11.000000 conflict_rpa-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 06:27:23.411805 conflict_rpa-0.0.9/conflict_rpa/
+-rw-rw-rw-   0        0        0        0 2024-05-24 13:02:31.000000 conflict_rpa-0.0.9/conflict_rpa/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 06:27:23.436804 conflict_rpa-0.0.9/conflict_rpa/__pycache__/
+-rw-rw-rw-   0        0        0      139 2024-05-26 08:54:35.000000 conflict_rpa-0.0.9/conflict_rpa/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2874 2024-05-26 08:54:35.000000 conflict_rpa-0.0.9/conflict_rpa/__pycache__/content_rpa.cpython-310.pyc
+-rw-rw-rw-   0        0        0     8202 2024-05-26 08:54:35.000000 conflict_rpa-0.0.9/conflict_rpa/__pycache__/correcting_framework.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2083 2024-05-26 08:54:35.000000 conflict_rpa-0.0.9/conflict_rpa/__pycache__/file_operation.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2683 2024-05-26 08:54:35.000000 conflict_rpa-0.0.9/conflict_rpa/__pycache__/get_running_env.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1286 2024-05-26 08:54:35.000000 conflict_rpa-0.0.9/conflict_rpa/__pycache__/rpa.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3242 2024-05-26 08:54:35.000000 conflict_rpa-0.0.9/conflict_rpa/__pycache__/utils.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1852 2024-05-26 11:07:22.000000 conflict_rpa-0.0.9/conflict_rpa/config.py
+-rw-rw-rw-   0        0        0     3446 2024-05-27 01:00:53.000000 conflict_rpa-0.0.9/conflict_rpa/content_rpa.py
+-rw-rw-rw-   0        0        0    11651 2024-05-27 06:16:20.000000 conflict_rpa-0.0.9/conflict_rpa/correcting_framework.py
+-rw-rw-rw-   0        0        0     4486 2024-05-27 05:01:26.000000 conflict_rpa-0.0.9/conflict_rpa/environment_setting.py
+-rw-rw-rw-   0        0        0     2436 2024-05-25 10:32:15.000000 conflict_rpa-0.0.9/conflict_rpa/file_operation.py
+-rw-rw-rw-   0        0        0     2985 2024-05-27 05:17:01.000000 conflict_rpa-0.0.9/conflict_rpa/get_running_env.py
+-rw-rw-rw-   0        0        0     3736 2024-05-27 01:00:54.000000 conflict_rpa-0.0.9/conflict_rpa/link_rpa.py
+-rw-rw-rw-   0        0        0     2537 2024-05-27 04:24:13.000000 conflict_rpa-0.0.9/conflict_rpa/rpa.py
+-rw-rw-rw-   0        0        0     3184 2024-05-27 05:51:09.000000 conflict_rpa-0.0.9/conflict_rpa/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-27 06:27:23.438806 conflict_rpa-0.0.9/conflict_rpa.egg-info/
+-rw-rw-rw-   0        0        0     7707 2024-05-27 06:27:23.000000 conflict_rpa-0.0.9/conflict_rpa.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      912 2024-05-27 06:27:23.000000 conflict_rpa-0.0.9/conflict_rpa.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 06:27:23.000000 conflict_rpa-0.0.9/conflict_rpa.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-05-27 06:27:23.000000 conflict_rpa-0.0.9/conflict_rpa.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       32 2024-05-27 06:27:23.000000 conflict_rpa-0.0.9/conflict_rpa.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-27 06:27:23.000000 conflict_rpa-0.0.9/conflict_rpa.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       95 2024-05-25 13:49:40.000000 conflict_rpa-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-27 06:27:23.441803 conflict_rpa-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      565 2024-05-27 06:26:56.000000 conflict_rpa-0.0.9/setup.py
```

### Comparing `conflict_rpa-0.0.8/PKG-INFO` & `conflict_rpa-0.0.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: conflict_rpa
-Version: 0.0.8
-Summary: A tool to rpa in your shell
-Author: FanYangli
-Author-email: yong.feng@centurygame.com
-Description-Content-Type: text/markdown
-Requires-Dist: openai>=1.28.1
-Requires-Dist: requests>=2.22.0
-
 # Conflict RPA
 
 ```shell
   ____ ____  ____   _
  / ___|  _ \|  _ \ / \
 | |   | |_) | |_) / _ \
 | |___|  _ <|  __/ ___ \
@@ -155,36 +145,44 @@
 
 这里的自动化执行在很多时候都有一些小问题，比如你需要提前 `git clone` 文件，预先安装`docker`等等。祝你好运。
 
 ### 自然语言命令
 
 在实现以上功能之后，这个工具可以实现进一步的功能——实现自然语言交互! 这确实是在设计之外的事情
 
+#### Case 1
+
 ```shell
 ➜ crpa -i 查询当前端口占用
 # after a sequence of analysis logs
 程序执行成功
 bash命令 sudo netstat -tuln
 被修改的文件: []
 执行结果:
 Active Internet connections (only servers) Proto Recv-Q Send-Q Local Address           Foreign Address         State udp        0      0 127.0.0.1:323           0.0.0.0:* udp6       0      0 ::1:323                 :::*
 ```
+
 其实也可以这样调用:
+
 ```shell
 ➜ 查询当前端口占用
 # 一段报错
 ➜ crpa
 # after a sequence of analysis logs
 程序执行成功
 bash命令 sudo netstat -tuln
 被修改的文件: []
 执行结果:
 Active Internet connections (only servers) Proto Recv-Q Send-Q Local Address           Foreign Address         State udp        0      0 127.0.0.1:323           0.0.0.0:* udp6       0      0 ::1:323                 :::*
 ```
 
+**这种是其实这样调用更好一些，毕竟你可以在里面加入空格**
+
+#### Case 2
+
 它实现的功能可以更加复杂(因为bash确实又很多很神奇的指令)
 
 ```shell
 ➜ crpa -i  抓取github trending 中的所有链接到log
 # after a sequence of analysis logs
 程序执行成功
 bash命令 curl -s https://github.com/trending | grep -Eo '<a [^>]+>' | grep -Eo 'href="[^"]+"' | awk -F'"' '{print $2}' > log
@@ -200,14 +198,16 @@
 https://github.com/features/actions
 https://github.com/features/packages
 https://github.com/features/security
 https://github.com/features/codespaces
 # 等等
 ```
 
+#### Case 3
+
 好像也可以产生一些可执行的文件?
 
 ```shell
 ➜  crpa -i 产生一个可以打印出 ASCII艺术字符格式的"CRPA" 的python脚本
 bash命令 pip install pyfiglet; echo 'import pyfiglet'
 print(pyfiglet.figlet_format("CRPA"))' > print_crpa.py && python3 print_crpa.py
 被修改的文件: []
@@ -220,8 +220,19 @@
 ```shell
 import pyfiglet
 print(pyfiglet.figlet_format("CRPA"))
 ```
 
 于是它可以打印出最上方的艺术字
 
+#### Case 4
+
+Bash 中也是有与UI交互的指令，所以，它在执行一些操作时会有恍惚间有一种真正RPA的感觉
+```shell
+crpa -i 使用Edge打开百度主页
+```
 祝您玩得愉快，就在刚刚，它帮我解决了提交冲突，感谢这个工具，希望它也对你有用
+
+## 额外说明
+* 显然，这只是一个非常简陋的小项目，完全的桌面自动化是不可能只靠一下午时间摸鱼解决的，希望这个行为艺术可以为大家通向AGI打开一些思路。
+* 目前不支持`cmd`，在`powershell`中的智能好像没有bash高，所以在windows上最好使用WSL
+* 网页抓取使用了[jina-ai/reader](https://github.com/jina-ai/reader) 非常感谢
```

### Comparing `conflict_rpa-0.0.8/README.md` & `conflict_rpa-0.0.9/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: conflict_rpa
+Version: 0.0.9
+Summary: A tool to rpa in your shell
+Author: FanYangli
+Author-email: yong.feng@centurygame.com
+Description-Content-Type: text/markdown
+Requires-Dist: openai>=1.28.1
+Requires-Dist: requests>=2.22.0
+
 # Conflict RPA
 
 ```shell
   ____ ____  ____   _
  / ___|  _ \|  _ \ / \
 | |   | |_) | |_) / _ \
 | |___|  _ <|  __/ ___ \
@@ -145,36 +155,44 @@
 
 这里的自动化执行在很多时候都有一些小问题，比如你需要提前 `git clone` 文件，预先安装`docker`等等。祝你好运。
 
 ### 自然语言命令
 
 在实现以上功能之后，这个工具可以实现进一步的功能——实现自然语言交互! 这确实是在设计之外的事情
 
+#### Case 1
+
 ```shell
 ➜ crpa -i 查询当前端口占用
 # after a sequence of analysis logs
 程序执行成功
 bash命令 sudo netstat -tuln
 被修改的文件: []
 执行结果:
 Active Internet connections (only servers) Proto Recv-Q Send-Q Local Address           Foreign Address         State udp        0      0 127.0.0.1:323           0.0.0.0:* udp6       0      0 ::1:323                 :::*
 ```
+
 其实也可以这样调用:
+
 ```shell
 ➜ 查询当前端口占用
 # 一段报错
 ➜ crpa
 # after a sequence of analysis logs
 程序执行成功
 bash命令 sudo netstat -tuln
 被修改的文件: []
 执行结果:
 Active Internet connections (only servers) Proto Recv-Q Send-Q Local Address           Foreign Address         State udp        0      0 127.0.0.1:323           0.0.0.0:* udp6       0      0 ::1:323                 :::*
 ```
 
+**这种是其实这样调用更好一些，毕竟你可以在里面加入空格**
+
+#### Case 2
+
 它实现的功能可以更加复杂(因为bash确实又很多很神奇的指令)
 
 ```shell
 ➜ crpa -i  抓取github trending 中的所有链接到log
 # after a sequence of analysis logs
 程序执行成功
 bash命令 curl -s https://github.com/trending | grep -Eo '<a [^>]+>' | grep -Eo 'href="[^"]+"' | awk -F'"' '{print $2}' > log
@@ -190,14 +208,16 @@
 https://github.com/features/actions
 https://github.com/features/packages
 https://github.com/features/security
 https://github.com/features/codespaces
 # 等等
 ```
 
+#### Case 3
+
 好像也可以产生一些可执行的文件?
 
 ```shell
 ➜  crpa -i 产生一个可以打印出 ASCII艺术字符格式的"CRPA" 的python脚本
 bash命令 pip install pyfiglet; echo 'import pyfiglet'
 print(pyfiglet.figlet_format("CRPA"))' > print_crpa.py && python3 print_crpa.py
 被修改的文件: []
@@ -210,8 +230,19 @@
 ```shell
 import pyfiglet
 print(pyfiglet.figlet_format("CRPA"))
 ```
 
 于是它可以打印出最上方的艺术字
 
-祝您玩得愉快，就在刚刚，它帮我解决了提交冲突，感谢这个工具，希望它也对你有用
+#### Case 4
+
+Bash 中也是有与UI交互的指令，所以，它在执行一些操作时会有恍惚间有一种真正RPA的感觉
+```shell
+crpa -i 使用Edge打开百度主页
+```
+祝您玩得愉快，就在刚刚，它帮我解决了提交冲突，感谢这个工具，希望它也对你有用
+
+## 额外说明
+* 显然，这只是一个非常简陋的小项目，完全的桌面自动化是不可能只靠一下午时间摸鱼解决的，希望这个行为艺术可以为大家通向AGI打开一些思路。
+* 目前不支持`cmd`，在`powershell`中的智能好像没有bash高，所以在windows上最好使用WSL
+* 网页抓取使用了[jina-ai/reader](https://github.com/jina-ai/reader) 非常感谢
```

### Comparing `conflict_rpa-0.0.8/conflict_rpa/__pycache__/content_rpa.cpython-310.pyc` & `conflict_rpa-0.0.9/conflict_rpa/__pycache__/content_rpa.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `conflict_rpa-0.0.8/conflict_rpa/__pycache__/correcting_framework.cpython-310.pyc` & `conflict_rpa-0.0.9/conflict_rpa/__pycache__/correcting_framework.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `conflict_rpa-0.0.8/conflict_rpa/__pycache__/file_operation.cpython-310.pyc` & `conflict_rpa-0.0.9/conflict_rpa/__pycache__/file_operation.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `conflict_rpa-0.0.8/conflict_rpa/__pycache__/get_running_env.cpython-310.pyc` & `conflict_rpa-0.0.9/conflict_rpa/__pycache__/get_running_env.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `conflict_rpa-0.0.8/conflict_rpa/__pycache__/rpa.cpython-310.pyc` & `conflict_rpa-0.0.9/conflict_rpa/__pycache__/rpa.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `conflict_rpa-0.0.8/conflict_rpa/__pycache__/utils.cpython-310.pyc` & `conflict_rpa-0.0.9/conflict_rpa/__pycache__/utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `conflict_rpa-0.0.8/conflict_rpa/config.py` & `conflict_rpa-0.0.9/conflict_rpa/config.py`

 * *Files identical despite different names*

### Comparing `conflict_rpa-0.0.8/conflict_rpa/content_rpa.py` & `conflict_rpa-0.0.9/conflict_rpa/content_rpa.py`

 * *Files identical despite different names*

### Comparing `conflict_rpa-0.0.8/conflict_rpa/correcting_framework.py` & `conflict_rpa-0.0.9/conflict_rpa/correcting_framework.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,48 +27,61 @@
         shell_name = 'zsh'
 else:
     if platform.system() == 'Windows':
         comspec = os.getenv('ComSpec')
         if comspec:
             print(comspec)
             if 'cmd.exe' in comspec.lower():
-                shell_name = 'powershell'
+                shell_name = 'cmd'
 
 
 def DEBUG(*args, **kwargs):
     if debug:
         print(*args)
 
 
 def operate_script(script):
     env = dict(os.environ)
     # 使用 subprocess.Popen 执行 Bash 命令并捕获输出
     try:
         process = subprocess.Popen(script, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True,
                                    env=env,
                                    encoding='utf-8')
-
+        outputs = ''
+        # 实时地将输出同步到标准输出中
+        while True:
+            output = process.stdout.readline()
+            if output == '' and process.poll() is not None:
+                break
+            if output:
+                print(output.strip())
+                outputs += output.strip() + ' '
+        # 捕获并打印任何错误输出
+        stderr = process.communicate()[1]
+        if stderr:
+            print(stderr.strip())
+            outputs += stderr.strip() + ' '
     except UnicodeDecodeError as e:
         print('尝试使用unicode编码')
-    process = subprocess.Popen(script, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True,
-                               env=env)
-    outputs = ''
-    # 实时地将输出同步到标准输出中
-    while True:
-        output = process.stdout.readline()
-        if output == '' and process.poll() is not None:
-            break
-        if output:
-            print(output.strip())
-            outputs += output.strip() + ' '
-    # 捕获并打印任何错误输出
-    stderr = process.communicate()[1]
-    if stderr:
-        print(stderr.strip())
-        outputs += stderr.strip() + ' '
+        process = subprocess.Popen(script, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True,
+                                   env=env)
+        outputs = ''
+        # 实时地将输出同步到标准输出中
+        while True:
+            output = process.stdout.readline()
+            if output == '' and process.poll() is not None:
+                break
+            if output:
+                print(output.strip())
+                outputs += output.strip() + ' '
+        # 捕获并打印任何错误输出
+        stderr = process.communicate()[1]
+        if stderr:
+            print(stderr.strip())
+            outputs += stderr.strip() + ' '
 
     return outputs
 
 
 def generate(prompt: str, json_mode=False):
     messages = [
         {
@@ -76,14 +89,18 @@
             'content': prompt}
     ]
     output = asyncio.run(async_chat(messages, LLMParams(json_mode=json_mode, model="gpt-4o", max_tokens=4096)))
     return output
 
 
 def check_correctness(script):
+    # PIPE OPEN 后的环境已经是conda 内的环境了吗
+    # conda_env = os.getenv('CONDA_DEFAULT_ENV')
+    # if conda_env:
+    #     script = f'conda   conda activate {conda_env}; ' + script
     output = operate_script(script)
     if output == 'timeout':
         return output, None
     prompt = f'''在以下的{shell_name}执行环境下
 ```
 {get_running_env()}
 ```
```

### Comparing `conflict_rpa-0.0.8/conflict_rpa/environment_setting.py` & `conflict_rpa-0.0.9/conflict_rpa/environment_setting.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 from setuptools.command.install import install
 
 
 def cmd_install():
     home_dir = os.path.expanduser("~")
     profile_path = os.path.join(home_dir, 'Documents', 'WindowsPowerShell', 'Microsoft.PowerShell_profile.ps1')
     script_source = os.path.join(home_dir, 'record_last_command.psm1')
+    cmd_auto_run_path = os.path.join(home_dir, 'record_last_command.cmd')
+
     script = '''function crpa
 {
     param (
         [string[]]$Args
     )
 
     # Get the last command from the history
@@ -51,14 +53,38 @@
     else:
         with open(profile_path, "w") as profile_file:
             profile_file.write(f'import-module "$HOME\\record_last_command.psm1"\n')
             print(f"Created PowerShell profile and added module import command")
 
     print('done')
 
+    # CMD script
+    cmd_script = '''
+    @echo off
+    :: This command captures the last command in the history and runs the user-defined action
+    doskey /history > "%TEMP%\\cmd_history.txt"
+    for /f "delims=" %%a in (%TEMP%\\cmd_history.txt) do set "last_cmd=%%a"
+    set last_cmd=%last_cmd:~0,-1%
+    set new_cmd=conflict_rpa %last_cmd%
+    echo Executing: %new_cmd%
+    :: Call your function here
+    :: %new_cmd%
+    '''
+
+    # Write the CMD autorun script
+    with open(cmd_auto_run_path, 'w') as f:
+        f.write(cmd_script)
+
+    # Set AutoRun environment variable for CMD
+    os.system(
+        f'reg add "HKCU\\Software\\Microsoft\\Command Processor" /v AutoRun /t REG_SZ /d "{cmd_auto_run_path}" /f')
+    print(f"Added CMD AutoRun command to registry")
+
+    print('done')
+
 
 def add_bashrc_content():
     shell = os.getenv('SHELL')
     if shell:
         shellrc_content = """
 crpa() {
     local last_command=$(fc -ln -1)
```

### Comparing `conflict_rpa-0.0.8/conflict_rpa/file_operation.py` & `conflict_rpa-0.0.9/conflict_rpa/file_operation.py`

 * *Files identical despite different names*

### Comparing `conflict_rpa-0.0.8/conflict_rpa/get_running_env.py` & `conflict_rpa-0.0.9/conflict_rpa/get_running_env.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,23 +72,25 @@
             else:
                 return "Command Prompt (cmd.exe)"
         return "Unknown"
     except Exception as e:
         return str(e)
 
 
+
 def get_running_env():
     config = {
         "bash_version": get_bash_version(),
         # "cpu_info": get_cpu_info(),
         "gpu_info": get_gpu_info(),
         "docker_version": check_docker(),
         "python_version": get_python_version(),
         "npm_version": get_npm_version(),
         "shell_type": get_shell_type(),
+        "conda_env_now": os.getenv('CONDA_DEFAULT_ENV')
     }
 
     config_string = json.dumps(config, indent=4)
     return config_string
 
 
 if __name__ == "__main__":
```

### Comparing `conflict_rpa-0.0.8/conflict_rpa/link_rpa.py` & `conflict_rpa-0.0.9/conflict_rpa/link_rpa.py`

 * *Files identical despite different names*

### Comparing `conflict_rpa-0.0.8/conflict_rpa/rpa.py` & `conflict_rpa-0.0.9/conflict_rpa/rpa.py`

 * *Files identical despite different names*

### Comparing `conflict_rpa-0.0.8/conflict_rpa/utils.py` & `conflict_rpa-0.0.9/conflict_rpa/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,31 +18,31 @@
 def UserMessage(content):
     return _base_message("user", content)
 
 
 class LLMParams:
     def __init__(
             self,
-            model: str = "gpt-4-turbo-preview",
-            temperature: float = 0.2,
-            max_tokens: int = 1024,
-            top_p: float = 1,
-            frequency_penalty: float = 0,
-            presence_penalty: float = 0,
-            json_mode: bool = False,
+            model="gpt-4-turbo-preview",
+            temperature=0.2,
+            max_tokens=1024,
+            top_p=1,
+            frequency_penalty=0,
+            presence_penalty=0,
+            json_mode=False,
     ):
         self.model = model
         self.temperature = temperature
         self.max_tokens = max_tokens
         self.top_p = top_p
         self.frequency_penalty = frequency_penalty
         self.presence_penalty = presence_penalty
         self.json_mode = json_mode
 
-    def from_dict(params: dict):
+    def from_dict(params):
         model = params.get("model", "gpt-4-1106-preview")
         temperature = params.get("temperature", 0.2)
         max_tokens = params.get("max_tokens", 256)
         top_p = params.get("top_p", 1)
         frequency_penalty = params.get("frequency_penalty", 0)
         presence_penalty = params.get("presence_penalty", 0)
         json_mode = params.get("json_mode", False)
@@ -61,15 +61,15 @@
 
     def copy(self, **params):
         # copy一份和当前参数一样的数据，并且支持参数的调整
         new_params = self.to_dict().copy()
         new_params.update(params)
         return LLMParams(**new_params)
 
-    def on_attempt(self, attempt: int):
+    def on_attempt(self, attempt):
         """根据重试次数自适应参数变化"""
         # 改变温度
         assert attempt >= 0
         if self.temperature <= 0.9:
             new_temperature = self.temperature + 0.01 * attempt
 
         new_model = self.model
@@ -77,20 +77,20 @@
             new_model = "gpt-4-1106-preview"
             if attempt >= 4:
                 new_model = "gpt-4-0613"
         return self.copy(model=new_model, temperature=new_temperature)
 
 
 async def async_chat(
-        messages: list[dict],
-        llm_params: LLMParams = LLMParams(),
-        stream: bool = False,
-        auto_decode: bool = False,
-        auto_retry: bool = True,
-) -> str:
+        messages,
+        llm_params=LLMParams(),
+        stream=False,
+        auto_decode=False,
+        auto_retry=True,
+):
     """异步聊天"""
     response = client.chat.completions.create(
         messages=messages,
         model=llm_params.model if llm_params.model else 'gpt-4-1106-preview',
         response_format={"type": "json_object"} if llm_params.json_mode else NOT_GIVEN
     )
```

### Comparing `conflict_rpa-0.0.8/conflict_rpa.egg-info/PKG-INFO` & `conflict_rpa-0.0.9/conflict_rpa.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conflict_rpa
-Version: 0.0.8
+Version: 0.0.9
 Summary: A tool to rpa in your shell
 Author: FanYangli
 Author-email: yong.feng@centurygame.com
 Description-Content-Type: text/markdown
 Requires-Dist: openai>=1.28.1
 Requires-Dist: requests>=2.22.0
 
@@ -155,36 +155,44 @@
 
 这里的自动化执行在很多时候都有一些小问题，比如你需要提前 `git clone` 文件，预先安装`docker`等等。祝你好运。
 
 ### 自然语言命令
 
 在实现以上功能之后，这个工具可以实现进一步的功能——实现自然语言交互! 这确实是在设计之外的事情
 
+#### Case 1
+
 ```shell
 ➜ crpa -i 查询当前端口占用
 # after a sequence of analysis logs
 程序执行成功
 bash命令 sudo netstat -tuln
 被修改的文件: []
 执行结果:
 Active Internet connections (only servers) Proto Recv-Q Send-Q Local Address           Foreign Address         State udp        0      0 127.0.0.1:323           0.0.0.0:* udp6       0      0 ::1:323                 :::*
 ```
+
 其实也可以这样调用:
+
 ```shell
 ➜ 查询当前端口占用
 # 一段报错
 ➜ crpa
 # after a sequence of analysis logs
 程序执行成功
 bash命令 sudo netstat -tuln
 被修改的文件: []
 执行结果:
 Active Internet connections (only servers) Proto Recv-Q Send-Q Local Address           Foreign Address         State udp        0      0 127.0.0.1:323           0.0.0.0:* udp6       0      0 ::1:323                 :::*
 ```
 
+**这种是其实这样调用更好一些，毕竟你可以在里面加入空格**
+
+#### Case 2
+
 它实现的功能可以更加复杂(因为bash确实又很多很神奇的指令)
 
 ```shell
 ➜ crpa -i  抓取github trending 中的所有链接到log
 # after a sequence of analysis logs
 程序执行成功
 bash命令 curl -s https://github.com/trending | grep -Eo '<a [^>]+>' | grep -Eo 'href="[^"]+"' | awk -F'"' '{print $2}' > log
@@ -200,14 +208,16 @@
 https://github.com/features/actions
 https://github.com/features/packages
 https://github.com/features/security
 https://github.com/features/codespaces
 # 等等
 ```
 
+#### Case 3
+
 好像也可以产生一些可执行的文件?
 
 ```shell
 ➜  crpa -i 产生一个可以打印出 ASCII艺术字符格式的"CRPA" 的python脚本
 bash命令 pip install pyfiglet; echo 'import pyfiglet'
 print(pyfiglet.figlet_format("CRPA"))' > print_crpa.py && python3 print_crpa.py
 被修改的文件: []
@@ -220,8 +230,19 @@
 ```shell
 import pyfiglet
 print(pyfiglet.figlet_format("CRPA"))
 ```
 
 于是它可以打印出最上方的艺术字
 
+#### Case 4
+
+Bash 中也是有与UI交互的指令，所以，它在执行一些操作时会有恍惚间有一种真正RPA的感觉
+```shell
+crpa -i 使用Edge打开百度主页
+```
 祝您玩得愉快，就在刚刚，它帮我解决了提交冲突，感谢这个工具，希望它也对你有用
+
+## 额外说明
+* 显然，这只是一个非常简陋的小项目，完全的桌面自动化是不可能只靠一下午时间摸鱼解决的，希望这个行为艺术可以为大家通向AGI打开一些思路。
+* 目前不支持`cmd`，在`powershell`中的智能好像没有bash高，所以在windows上最好使用WSL
+* 网页抓取使用了[jina-ai/reader](https://github.com/jina-ai/reader) 非常感谢
```

### Comparing `conflict_rpa-0.0.8/conflict_rpa.egg-info/SOURCES.txt` & `conflict_rpa-0.0.9/conflict_rpa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `conflict_rpa-0.0.8/setup.py` & `conflict_rpa-0.0.9/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='conflict_rpa',
-    version='0.0.8',
+    version='0.0.9',
     packages=find_packages(),
     install_requires=[
         'openai>=1.28.1',
         'requests>=2.22.0',
     ],
     author='FanYangli',
     author_email='yong.feng@centurygame.com',
```

