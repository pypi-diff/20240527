# Comparing `tmp/txdpy-8.8.9.tar.gz` & `tmp/txdpy-8.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "txdpy-8.8.9.tar", last modified: Mon May 27 03:25:33 2024, max compression
+gzip compressed data, was "txdpy-8.9.0.tar", last modified: Mon May 27 07:18:21 2024, max compression
```

## Comparing `txdpy-8.8.9.tar` & `txdpy-8.9.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 03:25:33.886618 txdpy-8.8.9/
--rw-rw-rw-   0        0        0      333 2024-05-27 03:25:33.885619 txdpy-8.8.9/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-27 03:25:33.886618 txdpy-8.8.9/setup.cfg
--rw-rw-rw-   0        0        0      340 2024-05-27 03:25:09.000000 txdpy-8.8.9/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-27 03:25:33.870348 txdpy-8.8.9/txdpy/
--rw-rw-rw-   0        0        0     3233 2024-05-27 02:38:25.000000 txdpy-8.8.9/txdpy/__init__.py
--rw-rw-rw-   0        0        0    27637 2024-05-27 02:45:02.000000 txdpy-8.8.9/txdpy/bk_179.py
--rw-rw-rw-   0        0        0    29116 2024-05-27 00:25:40.000000 txdpy-8.8.9/txdpy/excel数据或mysql操作.py
--rw-rw-rw-   0        0        0      930 2024-05-25 06:52:11.000000 txdpy-8.8.9/txdpy/列表操作.py
--rw-rw-rw-   0        0        0     2183 2024-05-25 06:52:11.000000 txdpy-8.8.9/txdpy/字符串类型的判断和提取.py
--rw-rw-rw-   0        0        0     6240 2024-05-25 06:53:20.000000 txdpy-8.8.9/txdpy/数据库操作.py
--rw-rw-rw-   0        0        0     5308 2024-05-25 06:52:11.000000 txdpy-8.8.9/txdpy/文本括号及引号不匹配检查.py
--rw-rw-rw-   0        0        0      699 2024-05-25 06:52:11.000000 txdpy-8.8.9/txdpy/文本错别字检查.py
--rw-rw-rw-   0        0        0     5882 2024-05-25 06:52:11.000000 txdpy-8.8.9/txdpy/爬虫辅助功能.py
--rw-rw-rw-   0        0        0     3548 2024-05-25 06:53:40.000000 txdpy-8.8.9/txdpy/百度ai接口使用.py
--rw-rw-rw-   0        0        0     2459 2024-05-25 06:52:11.000000 txdpy-8.8.9/txdpy/省市区名称的提取或判断.py
-drwxrwxrwx   0        0        0        0 2024-05-27 03:25:33.883618 txdpy-8.8.9/txdpy.egg-info/
--rw-rw-rw-   0        0        0      333 2024-05-27 03:25:33.000000 txdpy-8.8.9/txdpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      489 2024-05-27 03:25:33.000000 txdpy-8.8.9/txdpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 03:25:33.000000 txdpy-8.8.9/txdpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       86 2024-05-27 03:25:33.000000 txdpy-8.8.9/txdpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-27 03:25:33.000000 txdpy-8.8.9/txdpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-27 07:18:21.318690 txdpy-8.9.0/
+-rw-rw-rw-   0        0        0      333 2024-05-27 07:18:21.317689 txdpy-8.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-27 07:18:21.318690 txdpy-8.9.0/setup.cfg
+-rw-rw-rw-   0        0        0      340 2024-05-27 07:18:00.000000 txdpy-8.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 07:18:21.303347 txdpy-8.9.0/txdpy/
+-rw-rw-rw-   0        0        0     3287 2024-05-27 06:54:38.000000 txdpy-8.9.0/txdpy/__init__.py
+-rw-rw-rw-   0        0        0    27787 2024-05-27 07:11:53.000000 txdpy-8.9.0/txdpy/bk_179.py
+-rw-rw-rw-   0        0        0    28796 2024-05-27 07:16:13.000000 txdpy-8.9.0/txdpy/excel数据或mysql操作.py
+-rw-rw-rw-   0        0        0      930 2024-05-25 06:52:11.000000 txdpy-8.9.0/txdpy/列表操作.py
+-rw-rw-rw-   0        0        0     2183 2024-05-25 06:52:11.000000 txdpy-8.9.0/txdpy/字符串类型的判断和提取.py
+-rw-rw-rw-   0        0        0     6240 2024-05-25 06:53:20.000000 txdpy-8.9.0/txdpy/数据库操作.py
+-rw-rw-rw-   0        0        0     5308 2024-05-25 06:52:11.000000 txdpy-8.9.0/txdpy/文本括号及引号不匹配检查.py
+-rw-rw-rw-   0        0        0      263 2024-05-27 06:52:44.000000 txdpy-8.9.0/txdpy/文本错别字检查.py
+-rw-rw-rw-   0        0        0     5882 2024-05-25 06:52:11.000000 txdpy-8.9.0/txdpy/爬虫辅助功能.py
+-rw-rw-rw-   0        0        0     3546 2024-05-27 06:56:43.000000 txdpy-8.9.0/txdpy/百度ai接口使用.py
+-rw-rw-rw-   0        0        0     2459 2024-05-25 06:52:11.000000 txdpy-8.9.0/txdpy/省市区名称的提取或判断.py
+drwxrwxrwx   0        0        0        0 2024-05-27 07:18:21.315689 txdpy-8.9.0/txdpy.egg-info/
+-rw-rw-rw-   0        0        0      333 2024-05-27 07:18:21.000000 txdpy-8.9.0/txdpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      489 2024-05-27 07:18:21.000000 txdpy-8.9.0/txdpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 07:18:21.000000 txdpy-8.9.0/txdpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       86 2024-05-27 07:18:21.000000 txdpy-8.9.0/txdpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-27 07:18:21.000000 txdpy-8.9.0/txdpy.egg-info/top_level.txt
```

### Comparing `txdpy-8.8.9/txdpy/__init__.py` & `txdpy-8.9.0/txdpy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 __all__ = ['prurar_code', 'convert_pc', 'convert_kl', 'delete_flase_empty', 'txdavg', 'txdpercavg', 'txdmin', 'txdperc',
            'QueryScoreRank', 'timer', 'exenla', 'getexcelth', 'ExtractEnrollmentLabels', 'UpdateName', 'sortedlbys',
            'GetSchoolNameBz', 'GetMajorNameBz', 'unify_keys', 'school_ljdm', 'prvadepl', 'optstr', 'MysqlConn',
            'read_excel', 'ReadData', 'gen_excel', 'liduel', 'list_dupl', 'get_chinese', 'get_letter', 'get_bletter',
            'get_sletter', 'get_num', 'get_num_letter', 'is_num', 'is_sletter',
            'is_bletter', 'is_letter', 'is_num_letter', 'is_chinese', 'PyMySQL', '文本括号及引号不匹配检查', 'req',
            'format_string_dict', 'webptablesl', 'dow_file', 'TextSimilar', 'translate', '文本错别字检查方法二',
-           'get_ssq', 'is_ssq', 'is_school'
+           'get_ssq', 'is_ssq', 'is_school', 'get_major_name'
            ]
 
 from .bk_179 import prurar_code
 from .bk_179 import convert_pc
 from .bk_179 import convert_kl
 from .bk_179 import delete_flase_empty
 from .bk_179 import txdavg
@@ -24,14 +24,15 @@
 from .bk_179 import UpdateName
 from .bk_179 import sortedlbys
 from .bk_179 import GetSchoolNameBz
 from .bk_179 import GetMajorNameBz
 from .bk_179 import unify_keys
 from .bk_179 import school_ljdm
 from .bk_179 import is_school
+from .bk_179 import get_major_name
 from .excel数据或mysql操作 import prvadepl
 from .excel数据或mysql操作 import optstr
 from .excel数据或mysql操作 import MysqlConn
 from .excel数据或mysql操作 import read_excel
 from .excel数据或mysql操作 import ReadData
 from .excel数据或mysql操作 import gen_excel
 from .列表操作 import liduel
```

### Comparing `txdpy-8.8.9/txdpy/bk_179.py` & `txdpy-8.9.0/txdpy/bk_179.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     prurar_code={"北京": 11, "天津": 12, "河北": 13, "山西": 14, "内蒙古": 15, "辽宁": 21, "吉林": 22, "黑龙江": 23,
            "上海": 31, "江苏": 32, "浙江": 33, "安徽": 34, "福建": 35, "江西": 36, "山东": 37, "河南": 41, "湖北": 42,
            "湖南": 43, "广东": 44, "广西": 45, "海南": 46, "重庆": 50, "四川": 51, "贵州": 52, "云南": 53, "西藏": 54,
            "陕西": 61, "甘肃": 62, "青海": 63, "宁夏": 64, "新疆": 65}
     if ssq:
         return prurar_code[ssq]
     if gkle in ('专业类','专业组','新高考','老高考','综合'):
-        prurar_dict = {x[0]: x[1] for x in ReadData('各省份高考分类').data[1:]}
+        prurar_dict = {x[0]: x[1] for x in ReadData('各省份高考分类').data}
         return json.loads(prurar_dict.get(gkle))
     return prurar_code
 
 #转换批次名称
 def convert_pc(pc,prurar=None):
     if prurar:
         new_pc = batch_dict1.get(pc) if prurar in prurar_code('老高考省份') else batch_dict2.get(pc)
@@ -178,15 +178,15 @@
         self.get_frac_rank()#获取当前年份所有省份所有科类所有批次分数排名生成字典数据
 
     def get_batch_xian(self):
         """
         获取当前年份所有省份所有科类批次线生成字典数据
         """
         batch_dict = {'本科批': '本科', '本科一批(普通类)': '本科一批', '本科二批(普通类)': '本科二批','专科批(普通类)': '专科', }
-        batch_xians = ReadData('批次线表', ['region_name', 'kelei_name', 'batch', 'batch_fen'],select_sql=f"`year` = '{self.year}'", replace_th=False).data[1:]
+        batch_xians = ReadData('批次线表', ['region_name', 'kelei_name', 'batch', 'batch_fen'],select_sql=f"`year` = '{self.year}'", replace_th=False).data
         if self.simplify_pcname:
             # 将批次转换为只有本专科
             for batch_xian in batch_xians:
                 pc = batch_dict.get(batch_xian[2], batch_xian[2])
                 pc = '专科' if '专科' in convert_pc(pc) else '本科'
                 pc = "专科" if ("专科" in pc or "二段" in pc) else "本科"
                 key = f'{batch_xian[0]}_{pc}_{convert_kl(batch_xian[1])}'
@@ -201,15 +201,15 @@
                 self.batch_xian_dict[f"{batchds[0]}_{batchds[2]}_{batchds[1]}"] = int(batchds[-1])
                 self.batch_xian_dict[f"{batchds[0]}_{batchds[2]}_{batchds[1]}"] = int(batchds[-1])
 
     def get_frac_rank(self):
         """
         获取当前年份所有省份所有科类所有批次分数排名生成字典数据
         """
-        frac_ranks = ReadData('一分一段表', ['region_name','kelei_name','tag','gaokaofen','paim'],select_sql=f"`year` = '{self.year}'",replace_th=False).data[1:]
+        frac_ranks = ReadData('一分一段表', ['region_name','kelei_name','tag','gaokaofen','paim'],select_sql=f"`year` = '{self.year}'",replace_th=False).data
         for frac_rank in frac_ranks:
             region_name=frac_rank[0]
             if region_name in ['北京','天津','山西','上海','江苏','江西','广东']:
                 # print(region_name)
                 if region_name in ['江苏','山西']:
                     key = f'{region_name}_{convert_kl(frac_rank[1])}_{"本科" if "一" in frac_rank[2] else "专科"}'
                 else:
@@ -388,15 +388,15 @@
     ht='招生标签' if ht=='招生类型' else ht
     ht='科类' if ht=='文\理科' else ht
     raise ValueError(f'表头中未找到“{ht}”相关字段名称，可以将“{ht}”字段添加至表中或将相应字段修改为“{ht}”')
 
 #提取专业名称中专业名称和括号部分内容，根据需要返回一级大类和二级大类
 class ExtractEnrollmentLabels:
     def __init__(self):
-        self.data={f'{v[0]}_{v[1]}':v[1:] for v in ReadData('专业、大类以及逻辑代码').data[1:]}
+        self.data={f'{v[0]}_{v[1]}':v[1:] for v in ReadData('专业、大类以及逻辑代码').data}
 
     def exmana(self,major,batch,school_name):
         """
         :param major:专业名称
         :param batch:批次
         :param school_name:学校名称，学校名称中有“职业”关键字优先在职业本科查找专业名称信息
         :return:专业名称、专业名称逻辑代码、二级大类、二级大类逻辑代码、一级大类、一级大类逻辑代码
@@ -425,18 +425,18 @@
     return sorted_lists
 
 class UpdateName():
     """
     更新院校名称和专业名称
     """
     def __init__(self):
-        schools=ReadData('更新院校名称名单')
+        schools=ReadData('更新院校名称名单').data
         self.schools = sorted(list(schools), key=lambda x: len(x[0]), reverse=True)
         zk_majors, bk_majors = [], []
-        majors=ReadData('更新专业名称名单')
+        majors=ReadData('更新专业名称名单').data
         for v in majors:
             if v[0] == '本科':
                 bk_majors.append(v[1:])
             elif v[0] == '专科' and v[1] != '汽车检测与维修技术':
                 zk_majors.append(v[1:])
         self.zk_majors = sorted(zk_majors, key=lambda x: len(x[0]), reverse=True)
         self.bk_majors = sorted(bk_majors, key=lambda x: len(x[0]), reverse=True)
@@ -503,32 +503,38 @@
         if re_string.endswith('大学') or re_string.endswith('学院') or re_string.endswith('学校') or re_string.endswith('分校'):
             return True
 
 def unify_keys(ks):
     """
     统一表头字段名称
     """
-    key_dict={x[0]: x[1] for x in ReadData('读取数据时表头字段统一化参考表').data[1:]}
+    key_dict={x[0]: x[1] for x in ReadData('读取数据时表头字段统一化参考表').data}
     for i,k1 in enumerate(ks):
         for k2,ys in key_dict.items():
             for y in ys.split(','):
                 if y==k1:
                     ks[i]=k2
                     break
     return ks
 
 def school_ljdm():
     """
     :return: 返回院校逻辑代码字典
     """
-    schools = [x[0] for x in ReadData('院校名称').data[1:]]
+    schools = [x[0] for x in ReadData('院校名称').data]
     school_dict = {}
-    for x in ReadData('院校库', ['院校逻辑代码', '院校名称']).data[1:]:
+    for x in ReadData('院校库', ['院校逻辑代码', '院校名称']).data:
         school_name = optstr(x[1])
         x_0_re = re.search('\((.+?)\)', school_name)
         if x_0_re:
             old_school_name = x_0_re.group(1)
             if old_school_name.strip('原') in schools:
                 school_name = school_name.replace(f'({old_school_name})', '')
                 school_dict[old_school_name.strip('原')] = x[0]
         school_dict[school_name] = x[0]
-    return school_dict
+    return school_dict
+
+def get_major_name(major):
+    major_re = re.search('([\u4e00-\u9fa5、]+)(.*)',major)
+    if major_re:
+        return major_re.groups(1)
+    return [None,None]
```

### Comparing `txdpy-8.8.9/txdpy/excel数据或mysql操作.py` & `txdpy-8.9.0/txdpy/excel数据或mysql操作.py`

 * *Files 1% similar despite different names*

```diff
@@ -321,20 +321,15 @@
             else:
                 data[key] = [row]
         return data
 
     def save(self, fp=None):
         if not fp:
             fp = self.table_name
-        workbook = xlsxwriter.Workbook(fp if fp.endswith('.xlsx') else f'{fp}.xlsx')
-        sheet = workbook.add_worksheet()
-        for row_num, row_data in enumerate(tqdm(self.data, desc=f'{os.path.basename(fp)}')):
-            for col_num, col_value in enumerate(row_data):
-                sheet.write(row_num, col_num, col_value)
-        workbook.close()
+        gen_excel(self.data,fp,self.columns)
 
     def __str__(self):
         return '你很牛逼，你很棒！'
 
     def __del__(self):
         if self.db:
             try:
```

### Comparing `txdpy-8.8.9/txdpy/列表操作.py` & `txdpy-8.9.0/txdpy/列表操作.py`

 * *Files identical despite different names*

### Comparing `txdpy-8.8.9/txdpy/字符串类型的判断和提取.py` & `txdpy-8.9.0/txdpy/字符串类型的判断和提取.py`

 * *Files identical despite different names*

### Comparing `txdpy-8.8.9/txdpy/数据库操作.py` & `txdpy-8.9.0/txdpy/数据库操作.py`

 * *Files identical despite different names*

### Comparing `txdpy-8.8.9/txdpy/文本括号及引号不匹配检查.py` & `txdpy-8.9.0/txdpy/文本括号及引号不匹配检查.py`

 * *Files identical despite different names*

### Comparing `txdpy-8.8.9/txdpy/爬虫辅助功能.py` & `txdpy-8.9.0/txdpy/爬虫辅助功能.py`

 * *Files identical despite different names*

### Comparing `txdpy-8.8.9/txdpy/百度ai接口使用.py` & `txdpy-8.9.0/txdpy/百度ai接口使用.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -83,8 +83,8 @@
         })
         headers = {
             'Content-Type': 'application/json',
             'Accept': 'application/json'
         }
         response = request("POST", url, headers=headers, data=payload).json()
         return ([(v['ori_frag'], v['correct_frag'], v['begin_pos']) for v in response['item']['vec_fragment'] if
-                 '(' not in v['ori_frag'] and ')' not in v['ori_frag'] and v['ori_frag'] != v['correct_frag']] or None)
+                 '(' not in v['ori_frag'] and ')' not in v['ori_frag'] and v['ori_frag'] != v['correct_frag']] or None)
```

### Comparing `txdpy-8.8.9/txdpy/省市区名称的提取或判断.py` & `txdpy-8.9.0/txdpy/省市区名称的提取或判断.py`

 * *Files identical despite different names*

