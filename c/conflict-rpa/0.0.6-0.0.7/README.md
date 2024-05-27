# Comparing `tmp/conflict_rpa-0.0.6.tar.gz` & `tmp/conflict_rpa-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conflict_rpa-0.0.6.tar", last modified: Mon May 27 03:15:03 2024, max compression
+gzip compressed data, was "conflict_rpa-0.0.7.tar", last modified: Mon May 27 04:03:03 2024, max compression
```

## Comparing `conflict_rpa-0.0.6.tar` & `conflict_rpa-0.0.7.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0 fanyangli  (1000) fanyangli  (1000)        0 2024-05-27 03:15:03.725314 conflict_rpa-0.0.6/
--rwxrwxrwx   0 fanyangli  (1000) fanyangli  (1000)       51 2024-05-26 09:50:21.000000 conflict_rpa-0.0.6/MANIFEST.in
--rwxrwxrwx   0 fanyangli  (1000) fanyangli  (1000)     6202 2024-05-27 03:15:03.720315 conflict_rpa-0.0.6/PKG-INFO
--rwxrwxrwx   0 fanyangli  (1000) fanyangli  (1000)     6169 2024-05-27 03:14:35.000000 conflict_rpa-0.0.6/README.md
-drwxrwxrwx   0 fanyangli  (1000) fanyangli  (1000)        0 2024-05-27 03:15:03.523755 conflict_rpa-0.0.6/conflict_rpa/
--rwxrwxrwx   0 fanyangli  (1000) fanyangli  (1000)        0 2024-05-24 13:02:31.000000 conflict_rpa-0.0.6/conflict_rpa/__init__.py
-drwxrwxrwx   0 fanyangli  (1000) fanyangli  (1000)        0 2024-05-27 03:15:03.697313 conflict_rpa-0.0.6/conflict_rpa/__pycache__/
--rwxrwxrwx   0 fanyangli  (1000) fanyangli  (1000)      139 2024-05-26 08:54:35.000000 conflict_rpa-0.0.6/conflict_rpa/__pycache__/__init__.cpython-310.pyc
--rwxrwxrwx   0 fanyangli  (1000) fanyangli  (1000)     2874 2024-05-26 08:54:35.000000 conflict_rpa-0.0.6/conflict_rpa/__pycache__/content_rpa.cpython-310.pyc
--rwxrwxrwx   0 fanyangli  (1000) fanyangli  (1000)     8202 2024-05-26 08:54:35.000000 conflict_rpa-0.0.6/conflict_rpa/__pycache__/correcting_framework.cpython-310.pyc
--rwxrwxrwx   0 fanyangli  (1000) fanyangli  (1000)     2083 2024-05-26 08:54:35.000000 conflict_rpa-0.0.6/conflict_rpa/__pycache__/file_operation.cpython-310.pyc
--rwxrwxrwx   0 fanyangli  (1000) fanyangli  (1000)     2683 2024-05-26 08:54:35.000000 conflict_rpa-0.0.6/conflict_rpa/__pycache__/get_running_env.cpython-310.pyc
--rwxrwxrwx   0 fanyangli  (1000) fanyangli  (1000)     1286 2024-05-26 08:54:35.000000 conflict_rpa-0.0.6/conflict_rpa/__pycache__/rpa.cpython-310.pyc
--rwxrwxrwx   0 fanyangli  (1000) fanyangli  (1000)     3242 2024-05-26 08:54:35.000000 conflict_rpa-0.0.6/conflict_rpa/__pycache__/utils.cpython-310.pyc
--rwxrwxrwx   0 fanyangli  (1000) fanyangli  (1000)     1852 2024-05-26 11:07:22.000000 conflict_rpa-0.0.6/conflict_rpa/config.py
--rwxrwxrwx   0 fanyangli  (1000) fanyangli  (1000)     3446 2024-05-27 01:00:53.000000 conflict_rpa-0.0.6/conflict_rpa/content_rpa.py
--rwxrwxrwx   0 fanyangli  (1000) fanyangli  (1000)    10579 2024-05-27 01:24:04.000000 conflict_rpa-0.0.6/conflict_rpa/correcting_framework.py
--rwxrwxrwx   0 fanyangli  (1000) fanyangli  (1000)     3596 2024-05-27 02:59:24.000000 conflict_rpa-0.0.6/conflict_rpa/environment_setting.py
--rwxrwxrwx   0 fanyangli  (1000) fanyangli  (1000)     2436 2024-05-25 10:32:15.000000 conflict_rpa-0.0.6/conflict_rpa/file_operation.py
--rwxrwxrwx   0 fanyangli  (1000) fanyangli  (1000)     2926 2024-05-25 10:32:16.000000 conflict_rpa-0.0.6/conflict_rpa/get_running_env.py
--rwxrwxrwx   0 fanyangli  (1000) fanyangli  (1000)     3736 2024-05-27 01:00:54.000000 conflict_rpa-0.0.6/conflict_rpa/link_rpa.py
--rwxrwxrwx   0 fanyangli  (1000) fanyangli  (1000)     2598 2024-05-27 03:09:26.000000 conflict_rpa-0.0.6/conflict_rpa/rpa.py
--rwxrwxrwx   0 fanyangli  (1000) fanyangli  (1000)     3309 2024-05-26 23:39:44.000000 conflict_rpa-0.0.6/conflict_rpa/utils.py
-drwxrwxrwx   0 fanyangli  (1000) fanyangli  (1000)        0 2024-05-27 03:15:03.713312 conflict_rpa-0.0.6/conflict_rpa.egg-info/
--rwxrwxrwx   0 fanyangli  (1000) fanyangli  (1000)     6202 2024-05-27 03:15:03.000000 conflict_rpa-0.0.6/conflict_rpa.egg-info/PKG-INFO
--rwxrwxrwx   0 fanyangli  (1000) fanyangli  (1000)      912 2024-05-27 03:15:03.000000 conflict_rpa-0.0.6/conflict_rpa.egg-info/SOURCES.txt
--rwxrwxrwx   0 fanyangli  (1000) fanyangli  (1000)        1 2024-05-27 03:15:03.000000 conflict_rpa-0.0.6/conflict_rpa.egg-info/dependency_links.txt
--rwxrwxrwx   0 fanyangli  (1000) fanyangli  (1000)       54 2024-05-27 03:15:03.000000 conflict_rpa-0.0.6/conflict_rpa.egg-info/entry_points.txt
--rwxrwxrwx   0 fanyangli  (1000) fanyangli  (1000)       16 2024-05-27 03:15:03.000000 conflict_rpa-0.0.6/conflict_rpa.egg-info/requires.txt
--rwxrwxrwx   0 fanyangli  (1000) fanyangli  (1000)       13 2024-05-27 03:15:03.000000 conflict_rpa-0.0.6/conflict_rpa.egg-info/top_level.txt
--rwxrwxrwx   0 fanyangli  (1000) fanyangli  (1000)       95 2024-05-25 13:49:40.000000 conflict_rpa-0.0.6/pyproject.toml
--rwxrwxrwx   0 fanyangli  (1000) fanyangli  (1000)       38 2024-05-27 03:15:03.726314 conflict_rpa-0.0.6/setup.cfg
--rwxrwxrwx   0 fanyangli  (1000) fanyangli  (1000)      564 2024-05-27 03:10:10.000000 conflict_rpa-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 04:03:03.388539 conflict_rpa-0.0.7/
+-rw-rw-rw-   0        0        0       51 2024-05-26 09:50:21.000000 conflict_rpa-0.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     6967 2024-05-27 04:03:03.386543 conflict_rpa-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     6701 2024-05-27 04:01:46.000000 conflict_rpa-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 04:03:03.354620 conflict_rpa-0.0.7/conflict_rpa/
+-rw-rw-rw-   0        0        0        0 2024-05-24 13:02:31.000000 conflict_rpa-0.0.7/conflict_rpa/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 04:03:03.381538 conflict_rpa-0.0.7/conflict_rpa/__pycache__/
+-rw-rw-rw-   0        0        0      139 2024-05-26 08:54:35.000000 conflict_rpa-0.0.7/conflict_rpa/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2874 2024-05-26 08:54:35.000000 conflict_rpa-0.0.7/conflict_rpa/__pycache__/content_rpa.cpython-310.pyc
+-rw-rw-rw-   0        0        0     8202 2024-05-26 08:54:35.000000 conflict_rpa-0.0.7/conflict_rpa/__pycache__/correcting_framework.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2083 2024-05-26 08:54:35.000000 conflict_rpa-0.0.7/conflict_rpa/__pycache__/file_operation.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2683 2024-05-26 08:54:35.000000 conflict_rpa-0.0.7/conflict_rpa/__pycache__/get_running_env.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1286 2024-05-26 08:54:35.000000 conflict_rpa-0.0.7/conflict_rpa/__pycache__/rpa.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3242 2024-05-26 08:54:35.000000 conflict_rpa-0.0.7/conflict_rpa/__pycache__/utils.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1852 2024-05-26 11:07:22.000000 conflict_rpa-0.0.7/conflict_rpa/config.py
+-rw-rw-rw-   0        0        0     3446 2024-05-27 01:00:53.000000 conflict_rpa-0.0.7/conflict_rpa/content_rpa.py
+-rw-rw-rw-   0        0        0    10608 2024-05-27 03:54:41.000000 conflict_rpa-0.0.7/conflict_rpa/correcting_framework.py
+-rw-rw-rw-   0        0        0     3596 2024-05-27 02:59:24.000000 conflict_rpa-0.0.7/conflict_rpa/environment_setting.py
+-rw-rw-rw-   0        0        0     2436 2024-05-25 10:32:15.000000 conflict_rpa-0.0.7/conflict_rpa/file_operation.py
+-rw-rw-rw-   0        0        0     2926 2024-05-25 10:32:16.000000 conflict_rpa-0.0.7/conflict_rpa/get_running_env.py
+-rw-rw-rw-   0        0        0     3736 2024-05-27 01:00:54.000000 conflict_rpa-0.0.7/conflict_rpa/link_rpa.py
+-rw-rw-rw-   0        0        0     2539 2024-05-27 03:31:27.000000 conflict_rpa-0.0.7/conflict_rpa/rpa.py
+-rw-rw-rw-   0        0        0     3309 2024-05-26 23:39:44.000000 conflict_rpa-0.0.7/conflict_rpa/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-27 04:03:03.384543 conflict_rpa-0.0.7/conflict_rpa.egg-info/
+-rw-rw-rw-   0        0        0     6967 2024-05-27 04:03:03.000000 conflict_rpa-0.0.7/conflict_rpa.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      912 2024-05-27 04:03:03.000000 conflict_rpa-0.0.7/conflict_rpa.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 04:03:03.000000 conflict_rpa-0.0.7/conflict_rpa.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-05-27 04:03:03.000000 conflict_rpa-0.0.7/conflict_rpa.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       32 2024-05-27 04:03:03.000000 conflict_rpa-0.0.7/conflict_rpa.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-27 04:03:03.000000 conflict_rpa-0.0.7/conflict_rpa.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       95 2024-05-25 13:49:40.000000 conflict_rpa-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-27 04:03:03.388539 conflict_rpa-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      565 2024-05-27 04:02:24.000000 conflict_rpa-0.0.7/setup.py
```

### Comparing `conflict_rpa-0.0.6/PKG-INFO` & `conflict_rpa-0.0.7/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,217 +1,217 @@
-Metadata-Version: 2.1
-Name: conflict_rpa
-Version: 0.0.6
-Summary: A tool to rpa in your shell
-Author: FanYangli
-Author-email: yong.feng@centurygame.com
-Description-Content-Type: text/markdown
-Requires-Dist: openai
-Requires-Dist: requests
-
-# Conflict RPA
-
-```shell
-  ____ ____  ____   _
- / ___|  _ \|  _ \ / \
-| |   | |_) | |_) / _ \
-| |___|  _ <|  __/ ___ \
- \____|_| \_\_| /_/   \_\
-```
-
-* 一个应用在 `bash/zsh/powershell` 上的python包，利用[GPT](https://github.com/openai/openai-python)
-  实现与[thefuck](https://github.com/nvbn/thefuck)略有不同的效果
-* 功能可以概括为两类
-    * 通过修正bash 指令或者代码使其运行不出现报错
-    * 将自然语言转化为bash指令直到正确执行
-*
-    * <span style="color:red; font-weight:bold;">Warning</span> 因为该工具确实会自动执行额外的操作，(虽然没有遇到过)
-      目前难以排除他会执行一些恶性操作的风险。以此为免责声明。
-
-## 安装
-
-建议`python>=3.10`
-
-```shell
-pip install conflict_rpa
-conflict_rpa
-# 进行相关配置
-# source ~/.bashrc 或重启bash
-crpa
-```
-
-* 源码安装
-
-```shell
-pip install --upgrade pip setuptools 
-pip install .
-```
-
-source ~/.bashrc或重启bash以生效
-
-## 运行
-
-```shell
-crpa -h
-```
-
-* 第一次执行时需要用户填入 `OPENAI API`配置
-
-## 功能
-
-### 命令行纠错
-
-```shell
-➜  git coomot -am
-git: 'coomot' is not a git command. See 'git --help'.
-
-The most similar command is
-        commit
-
-➜  crpa
-# after a sequence of analysis logs
-程序执行成功
-bash命令“ git config --global user.email "you@example.com"
-git config --global user.name "Your Name"; git commit -am 'your commit message'
-被修改的文件: []
-执行结果:
-[main 242105a] your commit message 11 files changed, 843 insertions(+), 863 deletions(-) rewrite README.md (100%)
-```
-
-### 代码纠错
-
-* 在`test`文件夹下做了一些代码修复样例
-* 纠错过程中会修改原始文件，但会保留所有被修改文件的备份`*.bak`
-
-``` shell
-➜  python test/test_for_multifile/main.py
-Traceback (most recent call last):
-  File "test/test_for_multifile/main.py", line 1, in <module>
-    from test.test_for_multifile.count import count
-ModuleNotFoundError: No module named 'test.test_for_multifile'
-
-➜  crpa
-# after a sequence of analysis logs
-程序执行成功
-bash命令“ export PYTHONPATH=$(pwd)/test; python test/test_for_multifile/main.py; export PYTHONPATH=$(pwd); python test/test_for_multifile/main.py
-被修改的文件: ['test/test_for_multifile/main.py', 'test/test_for_multifile/count.py']
-执行结果:
-3 3
-
-```
-
-原始文件
-
-```python
-# count.py
-def count(a: int, b: int):
-    assert isinstance(a, str)
-    return a + b
-
-
-# main.py
-from test.test_for_multifile.count import count
-
-print(count(1, 2))
-```
-
-修改后文件
-
-```python
-# count.py
-def count(a: int, b: int):
-    assert isinstance(a, int)
-    return a + b
-
-
-# main.py
-from count import count
-
-print(count(1, 2))
-```
-
-### 自动执行教程
-
-如果从 `stackoverflow`, `github`, `CSDN`上找到一些教程链接，可能是关于如何安装新项目或者修改配置的bash指令，那么就可以试试这个功能
-
-```shell
-➜  crpa -l https://github.com/danielmiessler/fabric
-此网站的信息:  fabric: An open-source framework for augmenting humans using AI
-环境需求: Ensure you have at least python3.10 installed on your operating system.
-将执行以下指令:
-* cd . 
-* git clone https://github.com/danielmiessler/fabric.git
-* cd fabric
-* pipx install . # 因为有操作系统信息，所以这里会直接执行wsl命令
-* fabric --help
-Do you want to continue? (yes/no): # 你可以检验一下命令是否正确之后顺序执行
-```
-
-必须承认，现在LLM的能力还没有达到能够完美完成大量操作的地步。以下给出另一个调用方法。从教程中复制指令列，来缩小让`crpa`
-自动执行的范围
-
-```shell
-➜  crpa -t <<EOF
-{你想要贴入的教程，这样可以多行粘贴}
-EOF
-```
-
-这里的自动化执行在很多时候都有一些小问题，比如你需要提前 `git clone` 文件，预先安装`docker`等等。祝你好运。
-
-### 自然语言命令
-
-在实现以上功能之后，这个工具可以实现进一步的功能——实现自然语言交互! 这确实是在设计之外的事情
-
-```shell
-➜ crpa -i 查询当前端口占用
-# after a sequence of analysis logs
-程序执行成功
-bash命令“ sudo netstat -tuln
-被修改的文件: []
-执行结果:
-Active Internet connections (only servers) Proto Recv-Q Send-Q Local Address           Foreign Address         State udp        0      0 127.0.0.1:323           0.0.0.0:* udp6       0      0 ::1:323                 :::*
-```
-
-它实现的功能可以更加复杂(因为bash确实又很多很神奇的指令)
-
-```shell
-➜ crpa -i  抓取github trending 中的所有链接到log
-# after a sequence of analysis logs
-程序执行成功
-bash命令“ curl -s https://github.com/trending | grep -Eo '<a [^>]+>' | grep -Eo 'href="[^"]+"' | awk -F'"' '{print $2}' > log
-被修改的文件: []
-执行结果:
-```
-
-log 中的内容
-
-```shell
-#start-of-content
-https://github.com/
-https://github.com/features/actions
-https://github.com/features/packages
-https://github.com/features/security
-https://github.com/features/codespaces
-# 等等
-```
-
-好像也可以产生一些可执行的文件?
-
-```shell
-➜  crpa -i 产生一个可以打印出 ASCII艺术字符格式的"CRPA" 的python脚本
-bash命令 pip install pyfiglet; echo 'import pyfiglet
-print(pyfiglet.figlet_format("CRPA"))' > print_crpa.py && python3 print_crpa.py
-被修改的文件: []
-执行结果:
-Looking in indexes: https://pypi.tuna.tsinghua.edu.cn/simple Requirement already satisfied: pyfiglet in python3.10/site-packages (1.0.2) ____ ____  ____   _ / ___|  _ \|  _ \ / \ | |   | |_) | |_) / _ \ | |___|  _ <|  __/ ___ \ \____|_| \_\_| /_/   \_\
-```
-
-产生了一个叫做`print_crpa.py`的脚本，帮你装好了库
-
-```shell
-import pyfiglet
-print(pyfiglet.figlet_format("CRPA"))
-```
-
-于是它可以打印出最上方的艺术字
-
-祝您玩得愉快，就在刚刚，它帮我解决了提交冲突，感谢这个工具，希望它也对你有用
+# Conflict RPA
+
+```shell
+  ____ ____  ____   _
+ / ___|  _ \|  _ \ / \
+| |   | |_) | |_) / _ \
+| |___|  _ <|  __/ ___ \
+ \____|_| \_\_| /_/   \_\
+```
+
+* 一个应用在 `bash/zsh/powershell` 上的python包，利用[GPT](https://github.com/openai/openai-python)
+  实现与[thefuck](https://github.com/nvbn/thefuck)略有不同的效果，尤其是解决一些类似于依赖冲突这样不费脑子但是很费时间的问题。
+* 功能可以概括为两类
+    * 通过修正bash 指令或者代码使其运行不出现报错
+    * 将自然语言转化为bash指令直到正确执行
+    * <span style="color:red; font-weight:bold;">Warning</span> 因为该工具确实会自动执行额外的操作，(虽然没有遇到过)
+      目前难以排除他会执行一些恶性操作的风险。以此为免责声明。
+
+## 安装
+
+建议`python>=3.10`
+
+```shell
+pip install conflict_rpa
+conflict_rpa
+# 进行相关配置
+# source ~/.bashrc 或重启bash
+crpa
+```
+
+* 源码安装
+
+```shell
+pip install --upgrade pip setuptools 
+pip install .
+```
+
+source ~/.bashrc或重启bash以生效
+
+## 运行
+
+```shell
+crpa -h
+```
+
+* 第一次执行时需要用户填入 `OPENAI API`配置
+
+## 功能
+
+### 命令行纠错
+
+```shell
+➜  git coomot -am
+git: 'coomot' is not a git command. See 'git --help'.
+
+The most similar command is
+        commit
+
+➜  crpa
+# after a sequence of analysis logs
+程序执行成功
+bash命令“ git config --global user.email "you@example.com"
+git config --global user.name "Your Name"; git commit -am 'your commit message'
+被修改的文件: []
+执行结果:
+[main 242105a] your commit message 11 files changed, 843 insertions(+), 863 deletions(-) rewrite README.md (100%)
+```
+
+### 代码纠错
+
+* 在`test`文件夹下做了一些代码修复样例
+* 纠错过程中会修改原始文件，但会保留所有被修改文件的备份`*.bak`
+
+``` shell
+➜  python test/test_for_multifile/main.py
+Traceback (most recent call last):
+  File "test/test_for_multifile/main.py", line 1, in <module>
+    from test.test_for_multifile.count import count
+ModuleNotFoundError: No module named 'test.test_for_multifile'
+
+➜  crpa
+# after a sequence of analysis logs
+程序执行成功
+bash命令“ export PYTHONPATH=$(pwd)/test; python test/test_for_multifile/main.py; export PYTHONPATH=$(pwd); python test/test_for_multifile/main.py
+被修改的文件: ['test/test_for_multifile/main.py', 'test/test_for_multifile/count.py']
+执行结果:
+3 3
+```
+
+原始文件
+
+```python
+# count.py
+def count(a: int, b: int):
+    assert isinstance(a, str)
+    return a + b
+
+
+# main.py
+from test.test_for_multifile.count import count
+
+print(count(1, 2))
+```
+
+修改后文件
+
+```python
+# count.py
+def count(a: int, b: int):
+    assert isinstance(a, int)
+    return a + b
+
+
+# main.py
+from count import count
+
+print(count(1, 2))
+```
+
+### 自动执行教程
+
+如果从 `stackoverflow`, `github`, `CSDN`上找到一些教程链接，可能是关于如何安装新项目或者修改配置的bash指令，那么就可以试试这个功能
+
+```shell
+➜  crpa -l https://github.com/danielmiessler/fabric
+此网站的信息:  fabric: An open-source framework for augmenting humans using AI
+环境需求: Ensure you have at least python3.10 installed on your operating system.
+将执行以下指令:
+* cd . 
+* git clone https://github.com/danielmiessler/fabric.git
+* cd fabric
+* pipx install . # 因为有操作系统信息，所以这里会直接执行wsl命令
+* fabric --help
+Do you want to continue? (yes/no): # 你可以检验一下命令是否正确之后顺序执行
+```
+
+必须承认，现在LLM的能力还没有达到能够完美完成大量操作的地步。以下给出另一个调用方法。从教程中复制指令列，来缩小让`crpa`
+自动执行的范围
+
+```shell
+➜  crpa -t <<EOF
+{你想要贴入的教程，这样可以多行粘贴}
+EOF
+```
+
+这里的自动化执行在很多时候都有一些小问题，比如你需要提前 `git clone` 文件，预先安装`docker`等等。祝你好运。
+
+### 自然语言命令
+
+在实现以上功能之后，这个工具可以实现进一步的功能——实现自然语言交互! 这确实是在设计之外的事情
+
+```shell
+➜ crpa -i 查询当前端口占用
+# after a sequence of analysis logs
+程序执行成功
+bash命令 sudo netstat -tuln
+被修改的文件: []
+执行结果:
+Active Internet connections (only servers) Proto Recv-Q Send-Q Local Address           Foreign Address         State udp        0      0 127.0.0.1:323           0.0.0.0:* udp6       0      0 ::1:323                 :::*
+```
+其实也可以这样调用:
+```shell
+➜ 查询当前端口占用
+# 一段报错
+➜ crpa
+# after a sequence of analysis logs
+程序执行成功
+bash命令 sudo netstat -tuln
+被修改的文件: []
+执行结果:
+Active Internet connections (only servers) Proto Recv-Q Send-Q Local Address           Foreign Address         State udp        0      0 127.0.0.1:323           0.0.0.0:* udp6       0      0 ::1:323                 :::*
+```
+
+它实现的功能可以更加复杂(因为bash确实又很多很神奇的指令)
+
+```shell
+➜ crpa -i  抓取github trending 中的所有链接到log
+# after a sequence of analysis logs
+程序执行成功
+bash命令 curl -s https://github.com/trending | grep -Eo '<a [^>]+>' | grep -Eo 'href="[^"]+"' | awk -F'"' '{print $2}' > log
+被修改的文件: []
+执行结果:
+```
+
+log 中的内容
+
+```shell
+#start-of-content
+https://github.com/
+https://github.com/features/actions
+https://github.com/features/packages
+https://github.com/features/security
+https://github.com/features/codespaces
+# 等等
+```
+
+好像也可以产生一些可执行的文件?
+
+```shell
+➜  crpa -i 产生一个可以打印出 ASCII艺术字符格式的"CRPA" 的python脚本
+bash命令 pip install pyfiglet; echo 'import pyfiglet'
+print(pyfiglet.figlet_format("CRPA"))' > print_crpa.py && python3 print_crpa.py
+被修改的文件: []
+执行结果:
+Looking in indexes: https://pypi.tuna.tsinghua.edu.cn/simple Requirement already satisfied: pyfiglet in python3.10/site-packages (1.0.2) ____ ____  ____   _ / ___|  _ \|  _ \ / \ | |   | |_) | |_) / _ \ | |___|  _ <|  __/ ___ \ \____|_| \_\_| /_/   \_\
+```
+
+产生了一个叫做`print_crpa.py`的脚本，帮你装好了库
+
+```shell
+import pyfiglet
+print(pyfiglet.figlet_format("CRPA"))
+```
+
+于是它可以打印出最上方的艺术字
+
+祝您玩得愉快，就在刚刚，它帮我解决了提交冲突，感谢这个工具，希望它也对你有用
```

### Comparing `conflict_rpa-0.0.6/README.md` & `conflict_rpa-0.0.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,32 @@
+Metadata-Version: 2.1
+Name: conflict_rpa
+Version: 0.0.7
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
  \____|_| \_\_| /_/   \_\
 ```
 
 * 一个应用在 `bash/zsh/powershell` 上的python包，利用[GPT](https://github.com/openai/openai-python)
-  实现与[thefuck](https://github.com/nvbn/thefuck)略有不同的效果
+  实现与[thefuck](https://github.com/nvbn/thefuck)略有不同的效果，尤其是解决一些类似于依赖冲突这样不费脑子但是很费时间的问题。
 * 功能可以概括为两类
     * 通过修正bash 指令或者代码使其运行不出现报错
     * 将自然语言转化为bash指令直到正确执行
-*
     * <span style="color:red; font-weight:bold;">Warning</span> 因为该工具确实会自动执行额外的操作，(虽然没有遇到过)
       目前难以排除他会执行一些恶性操作的风险。以此为免责声明。
 
 ## 安装
 
 建议`python>=3.10`
 
@@ -82,15 +91,14 @@
 ➜  crpa
 # after a sequence of analysis logs
 程序执行成功
 bash命令“ export PYTHONPATH=$(pwd)/test; python test/test_for_multifile/main.py; export PYTHONPATH=$(pwd); python test/test_for_multifile/main.py
 被修改的文件: ['test/test_for_multifile/main.py', 'test/test_for_multifile/count.py']
 执行结果:
 3 3
-
 ```
 
 原始文件
 
 ```python
 # count.py
 def count(a: int, b: int):
@@ -151,27 +159,39 @@
 
 在实现以上功能之后，这个工具可以实现进一步的功能——实现自然语言交互! 这确实是在设计之外的事情
 
 ```shell
 ➜ crpa -i 查询当前端口占用
 # after a sequence of analysis logs
 程序执行成功
-bash命令“ sudo netstat -tuln
+bash命令 sudo netstat -tuln
+被修改的文件: []
+执行结果:
+Active Internet connections (only servers) Proto Recv-Q Send-Q Local Address           Foreign Address         State udp        0      0 127.0.0.1:323           0.0.0.0:* udp6       0      0 ::1:323                 :::*
+```
+其实也可以这样调用:
+```shell
+➜ 查询当前端口占用
+# 一段报错
+➜ crpa
+# after a sequence of analysis logs
+程序执行成功
+bash命令 sudo netstat -tuln
 被修改的文件: []
 执行结果:
 Active Internet connections (only servers) Proto Recv-Q Send-Q Local Address           Foreign Address         State udp        0      0 127.0.0.1:323           0.0.0.0:* udp6       0      0 ::1:323                 :::*
 ```
 
 它实现的功能可以更加复杂(因为bash确实又很多很神奇的指令)
 
 ```shell
 ➜ crpa -i  抓取github trending 中的所有链接到log
 # after a sequence of analysis logs
 程序执行成功
-bash命令“ curl -s https://github.com/trending | grep -Eo '<a [^>]+>' | grep -Eo 'href="[^"]+"' | awk -F'"' '{print $2}' > log
+bash命令 curl -s https://github.com/trending | grep -Eo '<a [^>]+>' | grep -Eo 'href="[^"]+"' | awk -F'"' '{print $2}' > log
 被修改的文件: []
 执行结果:
 ```
 
 log 中的内容
 
 ```shell
@@ -184,15 +204,15 @@
 # 等等
 ```
 
 好像也可以产生一些可执行的文件?
 
 ```shell
 ➜  crpa -i 产生一个可以打印出 ASCII艺术字符格式的"CRPA" 的python脚本
-bash命令 pip install pyfiglet; echo 'import pyfiglet
+bash命令 pip install pyfiglet; echo 'import pyfiglet'
 print(pyfiglet.figlet_format("CRPA"))' > print_crpa.py && python3 print_crpa.py
 被修改的文件: []
 执行结果:
 Looking in indexes: https://pypi.tuna.tsinghua.edu.cn/simple Requirement already satisfied: pyfiglet in python3.10/site-packages (1.0.2) ____ ____  ____   _ / ___|  _ \|  _ \ / \ | |   | |_) | |_) / _ \ | |___|  _ <|  __/ ___ \ \____|_| \_\_| /_/   \_\
 ```
 
 产生了一个叫做`print_crpa.py`的脚本，帮你装好了库
@@ -200,8 +220,8 @@
 ```shell
 import pyfiglet
 print(pyfiglet.figlet_format("CRPA"))
 ```
 
 于是它可以打印出最上方的艺术字
 
-祝您玩得愉快，就在刚刚，它帮我解决了提交冲突，感谢这个工具，希望它也对你有用
+祝您玩得愉快，就在刚刚，它帮我解决了提交冲突，感谢这个工具，希望它也对你有用
```

### Comparing `conflict_rpa-0.0.6/conflict_rpa/__pycache__/content_rpa.cpython-310.pyc` & `conflict_rpa-0.0.7/conflict_rpa/__pycache__/content_rpa.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `conflict_rpa-0.0.6/conflict_rpa/__pycache__/correcting_framework.cpython-310.pyc` & `conflict_rpa-0.0.7/conflict_rpa/__pycache__/correcting_framework.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `conflict_rpa-0.0.6/conflict_rpa/__pycache__/file_operation.cpython-310.pyc` & `conflict_rpa-0.0.7/conflict_rpa/__pycache__/file_operation.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `conflict_rpa-0.0.6/conflict_rpa/__pycache__/get_running_env.cpython-310.pyc` & `conflict_rpa-0.0.7/conflict_rpa/__pycache__/get_running_env.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `conflict_rpa-0.0.6/conflict_rpa/__pycache__/rpa.cpython-310.pyc` & `conflict_rpa-0.0.7/conflict_rpa/__pycache__/rpa.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `conflict_rpa-0.0.6/conflict_rpa/__pycache__/utils.cpython-310.pyc` & `conflict_rpa-0.0.7/conflict_rpa/__pycache__/utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `conflict_rpa-0.0.6/conflict_rpa/config.py` & `conflict_rpa-0.0.7/conflict_rpa/config.py`

 * *Files identical despite different names*

### Comparing `conflict_rpa-0.0.6/conflict_rpa/content_rpa.py` & `conflict_rpa-0.0.7/conflict_rpa/content_rpa.py`

 * *Files identical despite different names*

### Comparing `conflict_rpa-0.0.6/conflict_rpa/correcting_framework.py` & `conflict_rpa-0.0.7/conflict_rpa/correcting_framework.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 def DEBUG(*args, **kwargs):
     if debug:
         print(*args)
 
 
 def operate_script(script):
     env = dict(os.environ)
-
+    env["LANG"] = "zh_CN.UTF-8"
     # 使用 subprocess.Popen 执行 Bash 命令并捕获输出
     process = subprocess.Popen(script, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True, env=env,
                                encoding='utf-8')
     outputs = ''
     # 实时地将输出同步到标准输出中
     while True:
         output = process.stdout.readline()
@@ -250,15 +250,15 @@
 {script}''')
 
         correct_res, output = check_correctness(script)
         if correct_res == 'timeout':
             return
         if correct_res['correctness']:
             print('程序执行成功')
-            print(f"命令“ {script}")
+            print(f"命令: {script}")
             print(f"被修改的文件: {changed_file_list}")
             print("执行结果:")
             print(output)
             return
     # 恢复被GPT弄到乱七八糟的文件
     for file_path in changed_file_list:
         recover_file(file_path)
```

### Comparing `conflict_rpa-0.0.6/conflict_rpa/environment_setting.py` & `conflict_rpa-0.0.7/conflict_rpa/environment_setting.py`

 * *Files identical despite different names*

### Comparing `conflict_rpa-0.0.6/conflict_rpa/file_operation.py` & `conflict_rpa-0.0.7/conflict_rpa/file_operation.py`

 * *Files identical despite different names*

### Comparing `conflict_rpa-0.0.6/conflict_rpa/get_running_env.py` & `conflict_rpa-0.0.7/conflict_rpa/get_running_env.py`

 * *Files identical despite different names*

### Comparing `conflict_rpa-0.0.6/conflict_rpa/link_rpa.py` & `conflict_rpa-0.0.7/conflict_rpa/link_rpa.py`

 * *Files identical despite different names*

### Comparing `conflict_rpa-0.0.6/conflict_rpa/rpa.py` & `conflict_rpa-0.0.7/conflict_rpa/rpa.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 
 def rpa():
     openai_config = read_all_config()
     if openai_config is None:
         environment_setting()
         print('环境设置完成')
-        subprocess.run('post_install_script', shell=True)
         print('需要初始化OPENAI配置')
         init_config()
         print('配置完成，`source ~/.bashrc`或重启后可执行`crpa`操作')
         return
     parser = argparse.ArgumentParser()
     parser.add_argument('-l', '--link', type=str, help="提供链接进行自动化操作", default=None)
     parser.add_argument('-t', '--tutorial', type=str, help="希望自动化操作的流程文本，不需要整理地很好", default=None)
```

### Comparing `conflict_rpa-0.0.6/conflict_rpa/utils.py` & `conflict_rpa-0.0.7/conflict_rpa/utils.py`

 * *Files identical despite different names*

### Comparing `conflict_rpa-0.0.6/conflict_rpa.egg-info/PKG-INFO` & `conflict_rpa-0.0.7/conflict_rpa.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,217 +1,227 @@
-Metadata-Version: 2.1
-Name: conflict_rpa
-Version: 0.0.6
-Summary: A tool to rpa in your shell
-Author: FanYangli
-Author-email: yong.feng@centurygame.com
-Description-Content-Type: text/markdown
-Requires-Dist: openai
-Requires-Dist: requests
-
-# Conflict RPA
-
-```shell
-  ____ ____  ____   _
- / ___|  _ \|  _ \ / \
-| |   | |_) | |_) / _ \
-| |___|  _ <|  __/ ___ \
- \____|_| \_\_| /_/   \_\
-```
-
-* 一个应用在 `bash/zsh/powershell` 上的python包，利用[GPT](https://github.com/openai/openai-python)
-  实现与[thefuck](https://github.com/nvbn/thefuck)略有不同的效果
-* 功能可以概括为两类
-    * 通过修正bash 指令或者代码使其运行不出现报错
-    * 将自然语言转化为bash指令直到正确执行
-*
-    * <span style="color:red; font-weight:bold;">Warning</span> 因为该工具确实会自动执行额外的操作，(虽然没有遇到过)
-      目前难以排除他会执行一些恶性操作的风险。以此为免责声明。
-
-## 安装
-
-建议`python>=3.10`
-
-```shell
-pip install conflict_rpa
-conflict_rpa
-# 进行相关配置
-# source ~/.bashrc 或重启bash
-crpa
-```
-
-* 源码安装
-
-```shell
-pip install --upgrade pip setuptools 
-pip install .
-```
-
-source ~/.bashrc或重启bash以生效
-
-## 运行
-
-```shell
-crpa -h
-```
-
-* 第一次执行时需要用户填入 `OPENAI API`配置
-
-## 功能
-
-### 命令行纠错
-
-```shell
-➜  git coomot -am
-git: 'coomot' is not a git command. See 'git --help'.
-
-The most similar command is
-        commit
-
-➜  crpa
-# after a sequence of analysis logs
-程序执行成功
-bash命令“ git config --global user.email "you@example.com"
-git config --global user.name "Your Name"; git commit -am 'your commit message'
-被修改的文件: []
-执行结果:
-[main 242105a] your commit message 11 files changed, 843 insertions(+), 863 deletions(-) rewrite README.md (100%)
-```
-
-### 代码纠错
-
-* 在`test`文件夹下做了一些代码修复样例
-* 纠错过程中会修改原始文件，但会保留所有被修改文件的备份`*.bak`
-
-``` shell
-➜  python test/test_for_multifile/main.py
-Traceback (most recent call last):
-  File "test/test_for_multifile/main.py", line 1, in <module>
-    from test.test_for_multifile.count import count
-ModuleNotFoundError: No module named 'test.test_for_multifile'
-
-➜  crpa
-# after a sequence of analysis logs
-程序执行成功
-bash命令“ export PYTHONPATH=$(pwd)/test; python test/test_for_multifile/main.py; export PYTHONPATH=$(pwd); python test/test_for_multifile/main.py
-被修改的文件: ['test/test_for_multifile/main.py', 'test/test_for_multifile/count.py']
-执行结果:
-3 3
-
-```
-
-原始文件
-
-```python
-# count.py
-def count(a: int, b: int):
-    assert isinstance(a, str)
-    return a + b
-
-
-# main.py
-from test.test_for_multifile.count import count
-
-print(count(1, 2))
-```
-
-修改后文件
-
-```python
-# count.py
-def count(a: int, b: int):
-    assert isinstance(a, int)
-    return a + b
-
-
-# main.py
-from count import count
-
-print(count(1, 2))
-```
-
-### 自动执行教程
-
-如果从 `stackoverflow`, `github`, `CSDN`上找到一些教程链接，可能是关于如何安装新项目或者修改配置的bash指令，那么就可以试试这个功能
-
-```shell
-➜  crpa -l https://github.com/danielmiessler/fabric
-此网站的信息:  fabric: An open-source framework for augmenting humans using AI
-环境需求: Ensure you have at least python3.10 installed on your operating system.
-将执行以下指令:
-* cd . 
-* git clone https://github.com/danielmiessler/fabric.git
-* cd fabric
-* pipx install . # 因为有操作系统信息，所以这里会直接执行wsl命令
-* fabric --help
-Do you want to continue? (yes/no): # 你可以检验一下命令是否正确之后顺序执行
-```
-
-必须承认，现在LLM的能力还没有达到能够完美完成大量操作的地步。以下给出另一个调用方法。从教程中复制指令列，来缩小让`crpa`
-自动执行的范围
-
-```shell
-➜  crpa -t <<EOF
-{你想要贴入的教程，这样可以多行粘贴}
-EOF
-```
-
-这里的自动化执行在很多时候都有一些小问题，比如你需要提前 `git clone` 文件，预先安装`docker`等等。祝你好运。
-
-### 自然语言命令
-
-在实现以上功能之后，这个工具可以实现进一步的功能——实现自然语言交互! 这确实是在设计之外的事情
-
-```shell
-➜ crpa -i 查询当前端口占用
-# after a sequence of analysis logs
-程序执行成功
-bash命令“ sudo netstat -tuln
-被修改的文件: []
-执行结果:
-Active Internet connections (only servers) Proto Recv-Q Send-Q Local Address           Foreign Address         State udp        0      0 127.0.0.1:323           0.0.0.0:* udp6       0      0 ::1:323                 :::*
-```
-
-它实现的功能可以更加复杂(因为bash确实又很多很神奇的指令)
-
-```shell
-➜ crpa -i  抓取github trending 中的所有链接到log
-# after a sequence of analysis logs
-程序执行成功
-bash命令“ curl -s https://github.com/trending | grep -Eo '<a [^>]+>' | grep -Eo 'href="[^"]+"' | awk -F'"' '{print $2}' > log
-被修改的文件: []
-执行结果:
-```
-
-log 中的内容
-
-```shell
-#start-of-content
-https://github.com/
-https://github.com/features/actions
-https://github.com/features/packages
-https://github.com/features/security
-https://github.com/features/codespaces
-# 等等
-```
-
-好像也可以产生一些可执行的文件?
-
-```shell
-➜  crpa -i 产生一个可以打印出 ASCII艺术字符格式的"CRPA" 的python脚本
-bash命令 pip install pyfiglet; echo 'import pyfiglet
-print(pyfiglet.figlet_format("CRPA"))' > print_crpa.py && python3 print_crpa.py
-被修改的文件: []
-执行结果:
-Looking in indexes: https://pypi.tuna.tsinghua.edu.cn/simple Requirement already satisfied: pyfiglet in python3.10/site-packages (1.0.2) ____ ____  ____   _ / ___|  _ \|  _ \ / \ | |   | |_) | |_) / _ \ | |___|  _ <|  __/ ___ \ \____|_| \_\_| /_/   \_\
-```
-
-产生了一个叫做`print_crpa.py`的脚本，帮你装好了库
-
-```shell
-import pyfiglet
-print(pyfiglet.figlet_format("CRPA"))
-```
-
-于是它可以打印出最上方的艺术字
-
-祝您玩得愉快，就在刚刚，它帮我解决了提交冲突，感谢这个工具，希望它也对你有用
+Metadata-Version: 2.1
+Name: conflict_rpa
+Version: 0.0.7
+Summary: A tool to rpa in your shell
+Author: FanYangli
+Author-email: yong.feng@centurygame.com
+Description-Content-Type: text/markdown
+Requires-Dist: openai>=1.28.1
+Requires-Dist: requests>=2.22.0
+
+# Conflict RPA
+
+```shell
+  ____ ____  ____   _
+ / ___|  _ \|  _ \ / \
+| |   | |_) | |_) / _ \
+| |___|  _ <|  __/ ___ \
+ \____|_| \_\_| /_/   \_\
+```
+
+* 一个应用在 `bash/zsh/powershell` 上的python包，利用[GPT](https://github.com/openai/openai-python)
+  实现与[thefuck](https://github.com/nvbn/thefuck)略有不同的效果，尤其是解决一些类似于依赖冲突这样不费脑子但是很费时间的问题。
+* 功能可以概括为两类
+    * 通过修正bash 指令或者代码使其运行不出现报错
+    * 将自然语言转化为bash指令直到正确执行
+    * <span style="color:red; font-weight:bold;">Warning</span> 因为该工具确实会自动执行额外的操作，(虽然没有遇到过)
+      目前难以排除他会执行一些恶性操作的风险。以此为免责声明。
+
+## 安装
+
+建议`python>=3.10`
+
+```shell
+pip install conflict_rpa
+conflict_rpa
+# 进行相关配置
+# source ~/.bashrc 或重启bash
+crpa
+```
+
+* 源码安装
+
+```shell
+pip install --upgrade pip setuptools 
+pip install .
+```
+
+source ~/.bashrc或重启bash以生效
+
+## 运行
+
+```shell
+crpa -h
+```
+
+* 第一次执行时需要用户填入 `OPENAI API`配置
+
+## 功能
+
+### 命令行纠错
+
+```shell
+➜  git coomot -am
+git: 'coomot' is not a git command. See 'git --help'.
+
+The most similar command is
+        commit
+
+➜  crpa
+# after a sequence of analysis logs
+程序执行成功
+bash命令“ git config --global user.email "you@example.com"
+git config --global user.name "Your Name"; git commit -am 'your commit message'
+被修改的文件: []
+执行结果:
+[main 242105a] your commit message 11 files changed, 843 insertions(+), 863 deletions(-) rewrite README.md (100%)
+```
+
+### 代码纠错
+
+* 在`test`文件夹下做了一些代码修复样例
+* 纠错过程中会修改原始文件，但会保留所有被修改文件的备份`*.bak`
+
+``` shell
+➜  python test/test_for_multifile/main.py
+Traceback (most recent call last):
+  File "test/test_for_multifile/main.py", line 1, in <module>
+    from test.test_for_multifile.count import count
+ModuleNotFoundError: No module named 'test.test_for_multifile'
+
+➜  crpa
+# after a sequence of analysis logs
+程序执行成功
+bash命令“ export PYTHONPATH=$(pwd)/test; python test/test_for_multifile/main.py; export PYTHONPATH=$(pwd); python test/test_for_multifile/main.py
+被修改的文件: ['test/test_for_multifile/main.py', 'test/test_for_multifile/count.py']
+执行结果:
+3 3
+```
+
+原始文件
+
+```python
+# count.py
+def count(a: int, b: int):
+    assert isinstance(a, str)
+    return a + b
+
+
+# main.py
+from test.test_for_multifile.count import count
+
+print(count(1, 2))
+```
+
+修改后文件
+
+```python
+# count.py
+def count(a: int, b: int):
+    assert isinstance(a, int)
+    return a + b
+
+
+# main.py
+from count import count
+
+print(count(1, 2))
+```
+
+### 自动执行教程
+
+如果从 `stackoverflow`, `github`, `CSDN`上找到一些教程链接，可能是关于如何安装新项目或者修改配置的bash指令，那么就可以试试这个功能
+
+```shell
+➜  crpa -l https://github.com/danielmiessler/fabric
+此网站的信息:  fabric: An open-source framework for augmenting humans using AI
+环境需求: Ensure you have at least python3.10 installed on your operating system.
+将执行以下指令:
+* cd . 
+* git clone https://github.com/danielmiessler/fabric.git
+* cd fabric
+* pipx install . # 因为有操作系统信息，所以这里会直接执行wsl命令
+* fabric --help
+Do you want to continue? (yes/no): # 你可以检验一下命令是否正确之后顺序执行
+```
+
+必须承认，现在LLM的能力还没有达到能够完美完成大量操作的地步。以下给出另一个调用方法。从教程中复制指令列，来缩小让`crpa`
+自动执行的范围
+
+```shell
+➜  crpa -t <<EOF
+{你想要贴入的教程，这样可以多行粘贴}
+EOF
+```
+
+这里的自动化执行在很多时候都有一些小问题，比如你需要提前 `git clone` 文件，预先安装`docker`等等。祝你好运。
+
+### 自然语言命令
+
+在实现以上功能之后，这个工具可以实现进一步的功能——实现自然语言交互! 这确实是在设计之外的事情
+
+```shell
+➜ crpa -i 查询当前端口占用
+# after a sequence of analysis logs
+程序执行成功
+bash命令 sudo netstat -tuln
+被修改的文件: []
+执行结果:
+Active Internet connections (only servers) Proto Recv-Q Send-Q Local Address           Foreign Address         State udp        0      0 127.0.0.1:323           0.0.0.0:* udp6       0      0 ::1:323                 :::*
+```
+其实也可以这样调用:
+```shell
+➜ 查询当前端口占用
+# 一段报错
+➜ crpa
+# after a sequence of analysis logs
+程序执行成功
+bash命令 sudo netstat -tuln
+被修改的文件: []
+执行结果:
+Active Internet connections (only servers) Proto Recv-Q Send-Q Local Address           Foreign Address         State udp        0      0 127.0.0.1:323           0.0.0.0:* udp6       0      0 ::1:323                 :::*
+```
+
+它实现的功能可以更加复杂(因为bash确实又很多很神奇的指令)
+
+```shell
+➜ crpa -i  抓取github trending 中的所有链接到log
+# after a sequence of analysis logs
+程序执行成功
+bash命令 curl -s https://github.com/trending | grep -Eo '<a [^>]+>' | grep -Eo 'href="[^"]+"' | awk -F'"' '{print $2}' > log
+被修改的文件: []
+执行结果:
+```
+
+log 中的内容
+
+```shell
+#start-of-content
+https://github.com/
+https://github.com/features/actions
+https://github.com/features/packages
+https://github.com/features/security
+https://github.com/features/codespaces
+# 等等
+```
+
+好像也可以产生一些可执行的文件?
+
+```shell
+➜  crpa -i 产生一个可以打印出 ASCII艺术字符格式的"CRPA" 的python脚本
+bash命令 pip install pyfiglet; echo 'import pyfiglet'
+print(pyfiglet.figlet_format("CRPA"))' > print_crpa.py && python3 print_crpa.py
+被修改的文件: []
+执行结果:
+Looking in indexes: https://pypi.tuna.tsinghua.edu.cn/simple Requirement already satisfied: pyfiglet in python3.10/site-packages (1.0.2) ____ ____  ____   _ / ___|  _ \|  _ \ / \ | |   | |_) | |_) / _ \ | |___|  _ <|  __/ ___ \ \____|_| \_\_| /_/   \_\
+```
+
+产生了一个叫做`print_crpa.py`的脚本，帮你装好了库
+
+```shell
+import pyfiglet
+print(pyfiglet.figlet_format("CRPA"))
+```
+
+于是它可以打印出最上方的艺术字
+
+祝您玩得愉快，就在刚刚，它帮我解决了提交冲突，感谢这个工具，希望它也对你有用
```

### Comparing `conflict_rpa-0.0.6/conflict_rpa.egg-info/SOURCES.txt` & `conflict_rpa-0.0.7/conflict_rpa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `conflict_rpa-0.0.6/setup.py` & `conflict_rpa-0.0.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,16 @@
-import sys
-
 from setuptools import setup, find_packages
 
-
 setup(
     name='conflict_rpa',
-    version='0.0.6',
+    version='0.0.7',
     packages=find_packages(),
     install_requires=[
-        'openai',
-        'requests'
+        'openai>=1.28.1',
+        'requests>=2.22.0',
     ],
     author='FanYangli',
     author_email='yong.feng@centurygame.com',
     description="A tool to rpa in your shell",
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type="text/markdown",
     entry_points='''
```

