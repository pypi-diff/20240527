# Comparing `tmp/txdpy-8.8.8.tar.gz` & `tmp/txdpy-8.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "txdpy-8.8.8.tar", last modified: Sat May 25 06:48:01 2024, max compression
+gzip compressed data, was "txdpy-8.8.9.tar", last modified: Mon May 27 03:25:33 2024, max compression
```

## Comparing `txdpy-8.8.8.tar` & `txdpy-8.8.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-25 06:48:01.775488 txdpy-8.8.8/
--rw-rw-rw-   0        0        0      333 2024-05-25 06:48:01.773348 txdpy-8.8.8/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-25 06:48:01.775488 txdpy-8.8.8/setup.cfg
--rw-rw-rw-   0        0        0      340 2024-05-25 06:41:05.000000 txdpy-8.8.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-25 06:48:01.758752 txdpy-8.8.8/txdpy/
--rw-rw-rw-   0        0        0     3191 2024-05-25 06:40:36.000000 txdpy-8.8.8/txdpy/__init__.py
--rw-rw-rw-   0        0        0    27537 2024-05-25 06:32:25.000000 txdpy-8.8.8/txdpy/bk_179.py
--rw-rw-rw-   0        0        0    29897 2024-05-25 06:40:36.000000 txdpy-8.8.8/txdpy/excel数据或mysql操作.py
--rw-rw-rw-   0        0        0      930 2024-05-25 05:19:32.000000 txdpy-8.8.8/txdpy/列表操作.py
--rw-rw-rw-   0        0        0     2183 2024-05-25 06:40:36.000000 txdpy-8.8.8/txdpy/字符串类型的判断和提取.py
--rw-rw-rw-   0        0        0     6224 2024-05-25 06:40:36.000000 txdpy-8.8.8/txdpy/数据库操作.py
--rw-rw-rw-   0        0        0     5308 2024-05-25 06:40:36.000000 txdpy-8.8.8/txdpy/文本括号及引号不匹配检查.py
--rw-rw-rw-   0        0        0      699 2024-05-25 06:40:36.000000 txdpy-8.8.8/txdpy/文本错别字检查.py
--rw-rw-rw-   0        0        0     5882 2024-05-25 06:08:49.000000 txdpy-8.8.8/txdpy/爬虫辅助功能.py
--rw-rw-rw-   0        0        0     3549 2024-05-25 06:40:36.000000 txdpy-8.8.8/txdpy/百度ai接口使用.py
--rw-rw-rw-   0        0        0     2459 2024-05-25 02:50:56.000000 txdpy-8.8.8/txdpy/省市区名称的提取或判断.py
-drwxrwxrwx   0        0        0        0 2024-05-25 06:48:01.772348 txdpy-8.8.8/txdpy.egg-info/
--rw-rw-rw-   0        0        0      333 2024-05-25 06:48:01.000000 txdpy-8.8.8/txdpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      489 2024-05-25 06:48:01.000000 txdpy-8.8.8/txdpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-25 06:48:01.000000 txdpy-8.8.8/txdpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       86 2024-05-25 06:48:01.000000 txdpy-8.8.8/txdpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-25 06:48:01.000000 txdpy-8.8.8/txdpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-27 03:25:33.886618 txdpy-8.8.9/
+-rw-rw-rw-   0        0        0      333 2024-05-27 03:25:33.885619 txdpy-8.8.9/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-27 03:25:33.886618 txdpy-8.8.9/setup.cfg
+-rw-rw-rw-   0        0        0      340 2024-05-27 03:25:09.000000 txdpy-8.8.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 03:25:33.870348 txdpy-8.8.9/txdpy/
+-rw-rw-rw-   0        0        0     3233 2024-05-27 02:38:25.000000 txdpy-8.8.9/txdpy/__init__.py
+-rw-rw-rw-   0        0        0    27637 2024-05-27 02:45:02.000000 txdpy-8.8.9/txdpy/bk_179.py
+-rw-rw-rw-   0        0        0    29116 2024-05-27 00:25:40.000000 txdpy-8.8.9/txdpy/excel数据或mysql操作.py
+-rw-rw-rw-   0        0        0      930 2024-05-25 06:52:11.000000 txdpy-8.8.9/txdpy/列表操作.py
+-rw-rw-rw-   0        0        0     2183 2024-05-25 06:52:11.000000 txdpy-8.8.9/txdpy/字符串类型的判断和提取.py
+-rw-rw-rw-   0        0        0     6240 2024-05-25 06:53:20.000000 txdpy-8.8.9/txdpy/数据库操作.py
+-rw-rw-rw-   0        0        0     5308 2024-05-25 06:52:11.000000 txdpy-8.8.9/txdpy/文本括号及引号不匹配检查.py
+-rw-rw-rw-   0        0        0      699 2024-05-25 06:52:11.000000 txdpy-8.8.9/txdpy/文本错别字检查.py
+-rw-rw-rw-   0        0        0     5882 2024-05-25 06:52:11.000000 txdpy-8.8.9/txdpy/爬虫辅助功能.py
+-rw-rw-rw-   0        0        0     3548 2024-05-25 06:53:40.000000 txdpy-8.8.9/txdpy/百度ai接口使用.py
+-rw-rw-rw-   0        0        0     2459 2024-05-25 06:52:11.000000 txdpy-8.8.9/txdpy/省市区名称的提取或判断.py
+drwxrwxrwx   0        0        0        0 2024-05-27 03:25:33.883618 txdpy-8.8.9/txdpy.egg-info/
+-rw-rw-rw-   0        0        0      333 2024-05-27 03:25:33.000000 txdpy-8.8.9/txdpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      489 2024-05-27 03:25:33.000000 txdpy-8.8.9/txdpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 03:25:33.000000 txdpy-8.8.9/txdpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       86 2024-05-27 03:25:33.000000 txdpy-8.8.9/txdpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-27 03:25:33.000000 txdpy-8.8.9/txdpy.egg-info/top_level.txt
```

### Comparing `txdpy-8.8.8/txdpy/__init__.py` & `txdpy-8.8.9/txdpy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 __all__ = ['prurar_code', 'convert_pc', 'convert_kl', 'delete_flase_empty', 'txdavg', 'txdpercavg', 'txdmin', 'txdperc',
            'QueryScoreRank', 'timer', 'exenla', 'getexcelth', 'ExtractEnrollmentLabels', 'UpdateName', 'sortedlbys',
            'GetSchoolNameBz', 'GetMajorNameBz', 'unify_keys', 'school_ljdm', 'prvadepl', 'optstr', 'MysqlConn',
            'read_excel', 'ReadData', 'gen_excel', 'liduel', 'list_dupl', 'get_chinese', 'get_letter', 'get_bletter',
            'get_sletter', 'get_num', 'get_num_letter', 'is_num', 'is_sletter',
            'is_bletter', 'is_letter', 'is_num_letter', 'is_chinese', 'PyMySQL', '文本括号及引号不匹配检查', 'req',
            'format_string_dict', 'webptablesl', 'dow_file', 'TextSimilar', 'translate', '文本错别字检查方法二',
-           'get_ssq', 'is_ssq'
+           'get_ssq', 'is_ssq', 'is_school'
            ]
 
 from .bk_179 import prurar_code
 from .bk_179 import convert_pc
 from .bk_179 import convert_kl
 from .bk_179 import delete_flase_empty
 from .bk_179 import txdavg
@@ -23,14 +23,15 @@
 from .bk_179 import ExtractEnrollmentLabels
 from .bk_179 import UpdateName
 from .bk_179 import sortedlbys
 from .bk_179 import GetSchoolNameBz
 from .bk_179 import GetMajorNameBz
 from .bk_179 import unify_keys
 from .bk_179 import school_ljdm
+from .bk_179 import is_school
 from .excel数据或mysql操作 import prvadepl
 from .excel数据或mysql操作 import optstr
 from .excel数据或mysql操作 import MysqlConn
 from .excel数据或mysql操作 import read_excel
 from .excel数据或mysql操作 import ReadData
 from .excel数据或mysql操作 import gen_excel
 from .列表操作 import liduel
@@ -54,8 +55,8 @@
 from .爬虫辅助功能 import webptablesl
 from .爬虫辅助功能 import dow_file
 from .百度ai接口使用 import TextSimilar
 from .百度ai接口使用 import translate
 from .百度ai接口使用 import 文本错别字检查方法二
 from .省市区名称的提取或判断 import get_ssq
 from .省市区名称的提取或判断 import is_ssq
-# from .文本错别字检查 import 文本错别字检查方法一
+# from .文本错别字检查 import 文本错别字检查方法一
```

### Comparing `txdpy-8.8.8/txdpy/bk_179.py` & `txdpy-8.8.9/txdpy/bk_179.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
 # @File  : 通用代码.py
 # @Time  : 2023/6/9 13:12
 # @Author: 唐旭东
-from txdpy import optstr, ReadData
+from .excel数据或mysql操作 import optstr, ReadData, prvadepl
 import sys,re,json
 from loguru import logger
-from txdpy import is_num
-from txdpy import list_dupl
+from .字符串类型的判断和提取 import is_num
+from .列表操作 import list_dupl
 
 #老高考批次
 batch_dict1 = {'本科一批A': '本科一批', '专科': '专科', '本科一批A1': '本科一批', '本科一批B': '本科一批',
                  '本科二批A': '本科二批', '本科二批B': '本科二批', '本科二批C': '本科二批', '高本贯通批': '专科',
                  '本科提前A': '本科一批', '本科提前批A': '本科一批', '本科提前批B': '本科一批', '本科提前B': '本科一批',
                  '本科一批': '本科一批', '蒙授本科一批': '本科一批', '本科二批': '本科二批', '蒙授本科二批': '本科二批',
                  '专科提前': '专科', '专科提前批': '专科', '蒙授本科提前A': '本科一批', '蒙授本科提前批A': '本科一批',
@@ -164,15 +164,15 @@
     """
     查询分数位次，省份批次线
     """
     def __init__(self,year,simplify_pcname=True):
         """
         :param year:年份
         :param mysql:mysql连接对象
-        :param simplify_pcname:将批次转换为只有本专科
+        :param simplify_pcname:是否将批次转换为只有本专科，默认为True
         """
         self.year=year
         self.simplify_pcname=simplify_pcname
         self.batch_xian_dict={}
         self.frac_rank_dict={'北京':{},'天津':{},'上海':{},'江苏':{},'山西':{},'广东':{},'江西':{},'other':{}}
         self.get_batch_xian()#获取当前年份所有省份所有科类批次线生成字典数据
         self.get_frac_rank()#获取当前年份所有省份所有科类所有批次分数排名生成字典数据
@@ -461,30 +461,30 @@
                 for major in self.bk_majors:
                     if re_name[0]==major[0]:
                         return major[0]+re_name[1]
         return name
 
 class GetSchoolNameBz():
     def __init__(self):
-        school_names = [school[0] for school in ReadData('院校名称')]
+        school_names = [school[0] for school in ReadData('院校名称').data]
         self.school_names = sorted(school_names, key=lambda x: len(x), reverse=True)
 
     def __call__(self,v):
         for school_name in self.school_names:
             if v.startswith(school_name):
                 备注 = v.replace(school_name, '', 1) or None
                 if 备注:
                     if 备注.startswith('('):
                         备注 = 备注.strip('(').strip(')')
                 return [school_name,备注]
         raise ValueError(f'{v} 字符串中未获取到学校名称')
 
 class GetMajorNameBz():
     def __init__(self):
-        major_names = [major[0] for major in ReadData('专业名称')]
+        major_names = [major[0] for major in ReadData('专业名称').data]
         self.major_names = sorted(major_names, key=lambda x: len(x), reverse=True)
 
     def __call__(self,v):
         for major_name in self.major_names:
             if v.startswith(major_name):
                 备注 = v.replace(major_name, '', 1) or None
                 if 备注:
```

### Comparing `txdpy-8.8.8/txdpy/excel数据或mysql操作.py` & `txdpy-8.8.9/txdpy/excel数据或mysql操作.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,50 +42,37 @@
             value = prvadepl(value)
             if type(value) == str:
                 values.values()[i] = format_str(value)
     return values
 
 
 def read_excel(file_path):
-    """读取.xlsx、.xls以及htm格式的文件数据
+    """读取.xlsx、.xls以及htm格式的文件数据，默认读取第一个sheet
     :param file_path:文件路径
     :return:表格数据
     """
-
-    def choose_sheet(sheet_names):
-        if len(sheet_names) > 1:
-            prompt_info = '发现多个“sheet”：'
-            for i, sheet_name in enumerate(sheet_names):
-                prompt_info += f'{i + 1}:{sheet_name}  '
-            print(prompt_info)
-            sheet_index = eval(input('请输入以上sheet对应序号选择sheet(直接按回车默认第1个)：') or "1")
-            while 1:
-                if type(sheet_index) == int and 0 < sheet_index <= len(sheet_names):
-                    return sheet_index - 1
-                sheet_index = eval(input('输入有误，请重新输入：'))
-
     datas = []
     if file_path.endswith('.xlsx'):
         from openpyxl import load_workbook
         import zipfile
         try:
             workbook = load_workbook(filename=file_path, read_only=True)
             sheet_names = workbook.sheetnames
-            sheet = workbook[sheet_names[choose_sheet(sheet_names)]]
+            sheet = workbook[sheet_names[0]]
             for row in sheet.iter_rows():
                 datas.append([prvadepl(cell.value) if isinstance(cell.value, float) else cell.value for cell in row])
         except zipfile.BadZipFile:
             from txdpy import webptablesl
             with open(file_path, 'r', encoding='utf-8') as f:
                 datas = webptablesl(f.read(), '//table')
     elif file_path.endswith('.xls'):
         import xlrd
         workbook = xlrd.open_workbook(file_path)
         sheet_names = workbook.sheet_names()
-        sheet = workbook.sheet_by_index(choose_sheet(sheet_names))
+        sheet = workbook.sheet_by_index(0)
         for row_idx in range(sheet.nrows):
             datas.append([prvadepl(cell) if isinstance(cell, float) else cell for cell in sheet.row_values(row_idx)])
     if datas:
         i = [i for i, l in enumerate(datas[0]) if not l and datas[0][i - 1]]
 
         data = []
         if i:
@@ -151,36 +138,33 @@
                 raise ValueError('数据必须是二维列表')
         elif data_info.endswith('.xlsx') or data_info.endswith('.xls'):  # 判断是否为.xlsx文件读取数据
             self.read_excel(data_info)
 
         else:
             self.read_mysql(data_info, select_sql)  # 当做查询数据库数据
 
-        self.data = self.data[1:]  # 所有数据以二维列表存放，不包括表头
-        self.columns = self.data[0]  # 表头
+        if not self.data:
+            raise ValueError('表格数据为空')
 
-        # 替换表头字段名称为中文
-        self.data[0] = self.replace_th_name(self.data[0])
-
-        if len(self.data) == 0:
-            raise ValueError('表格数据为空，此类(ReadData)读取数据第一行必须用作为索引')
+        self.columns = self.replace_th_name(self.data[0])# 替换表头字段名称为中文
+        self.data = self.data[1:]  # 所有数据以二维列表存放，不包括表头
 
-        self.columns_index = {field: i for i, field in enumerate(self.data[0])}  # 创建列索引
+        self.columns_index = {field: i for i, field in enumerate(self.columns)}  # 创建列索引
 
         if needful_field:  # 判断是否有需要保留的字段，按保留的字段保留数据
             self.reserve_needful_field(needful_field)
 
         for k, v in self.columns_index.items():
             try:
                 exec(f'self.{k}={v}')
             except:
                 pass
 
         self.len_row = len(self.data)  # 行数
-        self.len_col = len(self.data[0])  # 列数
+        self.len_col = len(self.columns)  # 列数
 
     def connect_mysql(self):
         self.db = pymysql.connect(host=self.mysql_config["1"]['host'], port=3306, user='root',
                                   password=self.mysql_config["1"]['password'],
                                   database=self.mysql_config["1"]['database'])
         self.cursor = self.db.cursor()
         self.cursor.execute("""select * from 公司表名称对应关系""")
```

### Comparing `txdpy-8.8.8/txdpy/列表操作.py` & `txdpy-8.8.9/txdpy/列表操作.py`

 * *Files identical despite different names*

### Comparing `txdpy-8.8.8/txdpy/字符串类型的判断和提取.py` & `txdpy-8.8.9/txdpy/字符串类型的判断和提取.py`

 * *Files identical despite different names*

### Comparing `txdpy-8.8.8/txdpy/数据库操作.py` & `txdpy-8.8.9/txdpy/数据库操作.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding:utf-8
 import re, pymysql, sys
 from pymysql.converters import escape_string
 from loguru import logger
 from typing import Union, List
 import json
 from sshtunnel import SSHTunnelForwarder
-from txdpy import translate
+from .百度ai接口使用 import translate
 
 
 class PyMySQL:
     def __init__(self, host: str = 'localhost', port=3306, user: str = 'root', password: str = '', database: str = '',
                  auto_add_key=False):
         """
         :param host: 默认本地地址
```

### Comparing `txdpy-8.8.8/txdpy/文本括号及引号不匹配检查.py` & `txdpy-8.8.9/txdpy/文本括号及引号不匹配检查.py`

 * *Files identical despite different names*

### Comparing `txdpy-8.8.8/txdpy/文本错别字检查.py` & `txdpy-8.8.9/txdpy/文本错别字检查.py`

 * *Files identical despite different names*

### Comparing `txdpy-8.8.8/txdpy/爬虫辅助功能.py` & `txdpy-8.8.9/txdpy/爬虫辅助功能.py`

 * *Files identical despite different names*

### Comparing `txdpy-8.8.8/txdpy/百度ai接口使用.py` & `txdpy-8.8.9/txdpy/百度ai接口使用.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 # @Time  : 2024/5/25 下午1:20
 # @Author: 唐旭东
 from requests import post, request, get
 from hashlib import md5
 from random import randint
 from time import sleep
 from json import dumps
-
-from excel数据或mysql操作 import ReadData
+from .excel数据或mysql操作 import ReadData
 
 
 class TextSimilar:
     def __init__(self):
         params = {"grant_type": "client_credentials", "client_id": "7eb6Ee3o8FLh9ce3ATX1MA1S",
                   "client_secret": "O44grcUdKtKSXXAMTkgpoDamFeweeGy7"}
         self.access_token = str(
```

### Comparing `txdpy-8.8.8/txdpy/省市区名称的提取或判断.py` & `txdpy-8.8.9/txdpy/省市区名称的提取或判断.py`

 * *Files identical despite different names*

